# Comparing `tmp/noteshrunk-1.4.2.tar.gz` & `tmp/noteshrunk-1.5.0.tar.gz`

## Comparing `noteshrunk-1.4.2.tar` & `noteshrunk-1.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 noteshrunk-1.4.2/CHANGELOG.md
--rwxr-xr-x   0        0        0    25034 2020-02-02 00:00:00.000000 noteshrunk-1.4.2/src/noteshrunk.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 noteshrunk-1.4.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 noteshrunk-1.4.2/LICENSE
--rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 noteshrunk-1.4.2/README.md
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 noteshrunk-1.4.2/pyproject.toml
--rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 noteshrunk-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 noteshrunk-1.5.0/CHANGELOG.md
+-rwxr-xr-x   0        0        0    30901 2020-02-02 00:00:00.000000 noteshrunk-1.5.0/src/noteshrunk.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 noteshrunk-1.5.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 noteshrunk-1.5.0/LICENSE
+-rw-r--r--   0        0        0     8085 2020-02-02 00:00:00.000000 noteshrunk-1.5.0/README.md
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 noteshrunk-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    49283 2020-02-02 00:00:00.000000 noteshrunk-1.5.0/PKG-INFO
```

### Comparing `noteshrunk-1.4.2/CHANGELOG.md` & `noteshrunk-1.5.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.5] - 2024-04-21
+
+### Fixed
+
+- Processing of grayscale and black-and-white images.
+
+### Changed
+
+- Changed from `print()` to `logging`.
+
 ## [1.4] - 2024-04-20
 
 ### Added
 
 - `--unsharp_mask`
 
 Helps enhance fine textures.
```

### Comparing `noteshrunk-1.4.2/src/noteshrunk.py` & `noteshrunk-1.5.0/src/noteshrunk.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
-VERSION = '1.4.2'
+VERSION = '1.5.0'
 
 import argparse
 from concurrent.futures import ThreadPoolExecutor
+import logging
 import os
 from pathlib import Path
 import random
 import re
+import shutil
 import string
+import sys
 import subprocess
 import tempfile
 
 import argcomplete
 import numpy as np
 from PIL import Image
 from scipy.ndimage import median_filter
@@ -81,15 +84,15 @@
         action='store_true',
         default=False,
         help='Create an individual color palette for each image (by sampling a -p percentage of the pixels of that image) instead of a global palette (by sampling a -p percentage of the pixels of each input image).')
     parser.add_argument(
         "-p",
         "--percentage",
         type=float,
-        default=10,
+        default=100,
         help="Percentage of pixels to sample from each image.")
     parser.add_argument(
         "-j",
         "--jobs",
         type=int,
         default=os.cpu_count(),
         help="Number of processes to use (default: number of CPU cores)")
@@ -98,22 +101,26 @@
         '--overwrite',
         action='store_true',
         default=False,
         help='Overwrite existing files without asking.')
     parser.add_argument(
         "-ts",
         "--threshold_saturation",
-        type=float,
+        type=int,
         default=15,
+        choices=range(0, 101),  # Allow values between 0 and 100
+        metavar="[1-100]",
         help="HSV saturation threshold (in percent) used for the background detection.")
     parser.add_argument(
         "-tv",
         "--threshold_value",
-        type=float,
+        type=int,
         default=20,
+        choices=range(0, 101),  # Allow values between 0 and 100
+        metavar="[1-100]",
         help="HSV value threshold (in percent) used for the background detection.")
     parser.add_argument(
         '--denoise_median',
         action='store_true',
         default=False,
         help='Apply median denoising.')
     parser.add_argument(
@@ -155,16 +162,16 @@
         '--keep_intermediate',
         action='store_true',
         default=False,
         help='Do not delete intermediate (single-page) PDFs afterwards.')
     parser.add_argument(
         '-v',
         '--verbose',
-        action='store_true',
-        default=False,
+        action="count",
+        default=0,
         help='Verbose output')
     parser.add_argument(
         '--version',
         action='version',
         version=VERSION,
         help='Show program version and exit')
 
@@ -206,43 +213,60 @@
     Sample a given percentage of pixels in the image.
 
     Args:
         image (np.array): The image to sample pixels from.
         percentage (float): Percentage of pixels to sample
 
     Returns:
-        np.array: The sampled pixels.
-    """
-    total_pixels = image.shape[0] * image.shape[1]
-    sample_size = int(total_pixels * (percentage / 100))
-    rng = np.random.default_rng(0)
-    indices = rng.choice(total_pixels, size=sample_size, replace=False)
-    return image.reshape((-1, 3))[indices]
+        np.array: The sampled pixels of shape
+                    (N*M, 3) in case of color images
+                    (N*M, 1) in case of grayscale and black-and-white images
+    """
+    if percentage == 100:
+        if len(image.shape) == 2:
+            return image.reshape((-1, 1))
+        else:
+            return image.reshape((-1, 3))
+
+    else:
+        total_pixels = image.shape[0] * image.shape[1]
+        sample_size = int(total_pixels * (percentage / 100))
+        rng = np.random.default_rng(0)
+        indices = rng.choice(total_pixels, size=sample_size, replace=False)
+        # black-and-white images
+        if len(image.shape) == 2:
+            return image.reshape((-1, 1))[indices]
+        else:
+            return image.reshape((-1, 3))[indices]
 
 
-def perform_kmeans(image, n_clusters, args):
+def perform_kmeans(pixels, n_clusters, args):
     """
     Performs k-means clustering on the image and return the cluster centers and the model.
 
     Args:
         image (np.array): The image to perform k-means clustering on.
+                          Shape: (N*M, 3) or (N*M, 1)
         n_clusters (int): The number of clusters.
+        args (argparse.Namespace): The command line arguments.
 
     Returns:
         tuple: The cluster centers and the fitted KMeans model.
     """
-    flattened_image = image.reshape((-1, 3))
+    assert pixels.shape[-1] in [1, 3]
+
     kmeans = KMeans(
         init = 'k-means++',
         n_init=1,
         n_clusters=n_clusters,
         copy_x = False,
         random_state=np.random.RandomState(0),
-        verbose = args.verbose
-        ).fit(flattened_image)
+        verbose = True if args.verbose else False
+        ).fit(pixels)
+
     return kmeans.cluster_centers_, kmeans
 
 
 def pack_rgb(rgb):
     """
     Pack a 24-bit RGB triple into a single integer.
 
@@ -309,93 +333,139 @@
                            out=np.zeros_like(rgb_max, dtype=float))
 
     value = rgb_max / 255.0
 
     return saturation, value
 
 
-def create_palette(image_s, args, use_global_palette=False):
+def create_palette(image_s, args, idx=None, use_global_palette=False):
     """
     Create a color palette from an image or a list of images.
 
     Args:
         image_s (np.array / list of filenames): Image file or list of image filenames if use_global_palette == True.
         args (argparse.Namespace): The command line arguments.
         use_global_palette (bool): Sample the color palette from a list of files instead of a single file
 
     Returns:
         tuple: The color palette and the fitted KMeans model.
     """
 
     if use_global_palette and isinstance(image_s, list):
-        verbose_print(args, 'Determining global color palette ...')
-        sampled_pixels = np.vstack(
-            [sample_pixels(io.imread(img), args.percentage) for img in image_s])
+        logging.info('Determining global color palette ...')
+        sampled_pixels = [sample_pixels(io.imread(img), args.percentage) for img in image_s]
+
+        # In case of mixed images types (color, grayscale, boolean / black-and-white),
+        contains_bool  = any(arr.dtype == bool                           for arr in sampled_pixels)
+        contains_gray  = any(arr.shape[-1] == 1 and arr.dtype == 'uint8' for arr in sampled_pixels)
+        contains_color = any(arr.shape[-1] == 3                          for arr in sampled_pixels)
+
+        if contains_color and (contains_gray or contains_bool):
+            sampled_pixels = [np.array(Image.fromarray(arr).convert('RGB')) for arr in sampled_pixels
+                                if arr.dtype == bool or (arr.shape[-1] == 1 and arr.dtype == 'uint8')]
+            logging.warning('You have mixed color images with grayscale and / or black-and-white images while instructing to create a global palette.'
+                +'This results in larger file sizes because all images are converted to color. Make sure this is what you want.')
+
+        # Only color images
+        elif contains_color and not (contains_gray or contains_bool):
+            pass
+
+        elif contains_gray and contains_bool:
+            sampled_pixels = [np.array(Image.fromarray(arr).convert('L')) for arr in sampled_pixels
+                                if arr.dtype == bool ]
+            logging.warning('You have mixed grayscale images with black-and-white images while instructing to create a global palette.'
+                +'This results in larger file sizes because all images are converted to grayscale. Make sure this is what you want.')
+
+        # Only grayscale images
+        elif contains_gray and not contains_bool:
+            pass
+
+        # Only black-and-white / boolean images
+        else:
+            pass
+
+        sampled_pixels = np.vstack(sampled_pixels)
 
     elif not use_global_palette and isinstance(image_s, np.ndarray):
-        verbose_print(args, 'Determining color palette ...')
+        logging.info('Page {}: Determining color palette ...'.format(idx))
         sampled_pixels = sample_pixels(image_s, args.percentage)
 
     else:
         raise RuntimeError('Programming error. Map map map map.')
 
     background_color = get_background_color(sampled_pixels)
-    foreground_mask = get_foreground_mask(
-        sampled_pixels,
-        background_color=background_color,
-        threshold_saturation=args.threshold_saturation,
-        threshold_value=args.threshold_value)
-    foreground_pixels = sampled_pixels[foreground_mask]
-
-    kmeans_colors, kmeans_model = perform_kmeans(
-        foreground_pixels, args.n_colors - 1, args)
-
-    if args.white_background:
-        color_palette = np.vstack(
-            [[255, 255, 255], kmeans_colors]).round(0).astype('uint8')
-    else:
-        color_palette = np.vstack(
-            [background_color, kmeans_colors]).round(0).astype('uint8')
-
-    verbose_print(
-        args,
-        'Found',
-        'global' if use_global_palette else '',
-        'colors:',
-        color_palette.tolist())
+    logging.info('Page {}:'.format(idx) if idx is not None else '' + 'Found background color {}'.format(background_color))
+
+    if not background_color.dtype == bool:
+        foreground_mask = get_foreground_mask(
+            sampled_pixels,
+            background_color=background_color,
+            threshold_saturation=args.threshold_saturation,
+            threshold_value=args.threshold_value)
+
+        foreground_pixels = sampled_pixels[foreground_mask]
+
+        logging.info('Page {}:'.format(idx) if idx is not None else '' + 'Clustering colors ...')
+        kmeans_colors, kmeans_model = perform_kmeans(
+            foreground_pixels, args.n_colors - 1, args)
+
+        if args.white_background:
+            color_palette = np.vstack(
+                [[255, 255, 255] if len(sampled_pixels[0]) == 3 else [255], kmeans_colors]).round(0).astype('uint8')
+        else:
+            color_palette = np.vstack(
+                [background_color, kmeans_colors]).round(0).astype('uint8')
 
-    return color_palette, kmeans_model
+        logging.info('Found {}colors: {}'.format('global ' if use_global_palette else '', color_palette.tolist()))
+
+        return color_palette, kmeans_model
+
+    else:
+        return np.vstack([True, False]), None
 
 
 def get_foreground_mask(
         image,
         background_color,
         threshold_saturation,
         threshold_value):
     """
     Get a binary mask of the foreground.
 
     Args:
         image (np.array): The image to get the foreground mask for.
+                          Shape: (N*M, 3) or (N*M, 1)
         background_color (np.array): The background color.
         threshold_saturation (foat): The HSV Saturation threshold used for foreground-background discrimination.
         threshold_value (foat): The HSV value threshold used for foreground-background discrimination.
 
     Returns:
         np.array: The binary mask of the foreground.
     """
-    saturation_bg, value_bg = rgb_to_sv(background_color)
-    saturation_image, value_image = rgb_to_sv(image)
+    assert image.shape[-1] in [1, 3]
+
+    # color images
+    if image.shape[-1] == 3:
+        saturation_bg, value_bg = rgb_to_sv(background_color)
+        saturation_image, value_image = rgb_to_sv(image)
+
+        saturation_diff = np.abs(saturation_bg - saturation_image)
+        value_diff = np.abs(value_bg - value_image)
 
-    saturation_diff = np.abs(saturation_bg - saturation_image)
-    value_diff = np.abs(value_bg - value_image)
+        return ((value_diff >= (threshold_value / 100)) |
+                (saturation_diff >= (threshold_saturation / 100)))
 
-    return ((value_diff >= threshold_value / 100) |
-            (saturation_diff >= threshold_saturation / 100))
+    # Grayscale images
+    elif image.shape[-1] == 1 and image.dtype == 'uint8':
+        value_diff = np.abs(background_color / 255. - image / 255.)
+        return np.squeeze( value_diff >= (threshold_value / 100) )
 
+    # black-and-white images
+    else:
+        raise RuntimeError('This should not happen.')
 
 def quantize_colors(image, color_depth=6):
     """
     Reduce the number of colors in an image by reducing the number of bits per channel.
 
     Args:
         image (numpy.ndarray): The input image.
@@ -419,98 +489,144 @@
 
     Args:
         pixels (numpy.ndarray): The RGB input pixels.
         bits_per_channel (int): The number of bits per channel.
 
     Returns:
         numpy.ndarray: An RGB tuple representing the background color.
+                       [R, G, B] in case of color
+                       [int] in case of grayscale
+                       [True] in case of black-and-white (boolean)
     """
 
-    assert pixels.shape[-1] == 3
+    # image was rolled out to shape (N*M, 3) (color) or (N*M, 1) (grayscale)
+    assert pixels.shape[-1] in [1, 3]
+
+    if pixels.shape[-1] == 3:
+        quantized = quantize_colors(pixels, bits_per_channel).astype(np.uint32)
+        packed = pack_rgb(quantized)
 
-    quantized = quantize_colors(pixels, bits_per_channel).astype(np.uint32)
-    packed = pack_rgb(quantized)
+        unique, counts = np.unique(packed, return_counts=True)
 
-    unique, counts = np.unique(packed, return_counts=True)
+        packed_background_color = unique[counts.argmax()]
 
-    packed_background_color = unique[counts.argmax()]
+        return unpack_rgb(packed_background_color)
 
-    return unpack_rgb(packed_background_color)
+    else:
+        # Grayscale images
+        if pixels.dtype == 'uint8':
+            quantized = quantize_colors(pixels, bits_per_channel).astype(np.uint32)
+            unique, counts = np.unique(quantized, return_counts=True)
+            return np.array( [ unique[counts.argmax()] ], dtype='uint8' )
+
+        elif pixels.dtype == bool:
+            # background color is white in black-and-white images
+            return np.array([True])
 
 
-def apply_color_palette(image, color_palette, kmeans_model, args):
+def apply_color_palette(image, color_palette, kmeans_model, args, idx):
     """
     Apply the color palette to the image using KMeans.predict.
 
     Args:
-        image (np.array): The image to apply the color palette to.
+        image (np.array): The image of shape (N, M), (N, M, 1) or (N, M, 3) to apply the color palette to.
         color_palette (np.array): The color palette.
         kmeans_model (KMeans): The fitted KMeans model.
         args (argparse.Namespace): The command line arguments.
 
     Returns:
         np.array: The image with the color palette applied.
     """
     shape = image.shape
-    image = image.reshape((-1, 3))
-    foreground_mask = get_foreground_mask(
-        image,
-        background_color=color_palette[0],
-        threshold_saturation=args.threshold_saturation,
-        threshold_value=args.threshold_value)
+    assert len(shape) in [2, 3]
+
+    if len(shape) == 3:
+        image = image.reshape((-1, 3))
+    else:
+        image = image.reshape((-1, 1))
+
+    if image.dtype == bool:
+        foreground_mask = ~image.copy()
+
+    else:
+        foreground_mask = get_foreground_mask(
+            image,
+            background_color=color_palette[0],
+            threshold_saturation=args.threshold_saturation,
+            threshold_value=args.threshold_value)
 
     # morphological opening of the binary foreground mask to remove e.g. dust speckles
     if args.denoise_opening:
-        verbose_print(args, 'Applying opening ...')
+        logging.info('Page {}: Applying opening ...'.format(idx))
         # disk(<1) results in id-operation or zero-matrix and is hence useless
         kernel = disk(
             args.opening_strength) if args.opening_strength >= 1 else square(2)
         foreground_mask = binary_opening(
             foreground_mask.reshape(shape[:-1]), kernel).flatten()
 
-    labels = np.zeros(image.shape[0], dtype='uint8')
-
-    verbose_print(args, 'Applying color palette ...')
-    labels[foreground_mask] = kmeans_model.predict(image[foreground_mask]) + 1
+    if image.dtype != bool:
+        labels = np.zeros(image.shape[0], dtype='uint8')
 
-    if args.saturate:
-        verbose_print(args, 'Maximizing saturation ...')
-        color_palette = color_palette.astype(float)
-        pmin = color_palette.min()
-        pmax = color_palette.max()
-        color_palette = 255 * (color_palette - pmin) / (pmax - pmin)
-        color_palette = color_palette.round(0).astype('uint8')
+        logging.info('Page {}: Applying color palette ...'.format(idx))
+        # If the image is a solid color, the foreground has shape (0, 3)
+        if image[foreground_mask].shape[0] != 0:
+            labels[foreground_mask] = kmeans_model.predict(image[foreground_mask]) + 1
+
+        if args.saturate:
+            logging.info('Page {}: Maximizing saturation ...'.format(idx))
+            color_palette = color_palette.astype(float)
+            pmin = color_palette.min()
+            pmax = color_palette.max()
+            color_palette = 255 * (color_palette - pmin) / (pmax - pmin)
+            color_palette = color_palette.round(0).astype('uint8')
 
-    image = color_palette[labels]
+        image = color_palette[labels]
 
     # set background to the background color
     image[~foreground_mask] = color_palette[0]
 
     if args.unsharp_mask:
-        verbose_print(args, 'Applying unsharp mask filtering ...')
+        logging.info('Page {}: Applying unsharp mask filtering ...'.format(idx))
 
-        image = np.array( Image.fromarray(image.reshape(shape), mode='RGB').convert('HSV') )
+        if len(shape) == 3:
+            image = np.array( Image.fromarray(image.reshape(shape), mode='RGB').convert('HSV') )
+
+            # unsharp_mask returns in range [0, 1] and preserve_range seems broken
+            tmp_max = np.max(image[:,:,2])
+            image[:,:,2] = (unsharp_mask(image[:,:,2],
+                                        radius=args.unsharp_radius,
+                                        amount=args.unsharp_amount) * tmp_max).round(0).astype('uint8')
+            image = np.array( Image.fromarray(image, mode='HSV').convert('RGB') ).reshape((-1,3))
+
+        elif len(shape) == 2 and image.dtype != bool:
+            tmp_max = np.max(image)
+            image = (unsharp_mask(image.reshape(shape),
+                                        radius=args.unsharp_radius,
+                                        amount=args.unsharp_amount) * tmp_max).round(0).astype('uint8').reshape((-1,1))
+
+        elif len(shape) == 2 and image.dtype == bool:
+            logging.warning('Unsharp masking has no effect on binary / black-and-white images. Hence I skip this step ...')
 
-        #
-        tmp_max = np.max(image[:,:,2])
-        image[:,:,2] = (unsharp_mask(image[:,:,2],
-                                    radius=args.unsharp_radius,
-                                    amount=args.unsharp_amount) * tmp_max).round(0).astype('uint8')
-        image = np.array( Image.fromarray(image, mode='HSV').convert('RGB') ).reshape((-1,3))
 
     if args.denoise_median:
-        verbose_print(args, 'Applying median filtering ...')
+        logging.info('Page {}: Applying median filtering ...'.format(idx))
         # Median filtering is per color channel. In RGB space this would lead
         # to color deviations.
-        image = Image.fromarray(image.reshape(shape), mode='RGB').convert('HSV')
-        image = median_filter(
-            image,
-            size=(args.median_strength, args.median_strength, 1)
-        )
-        image = Image.fromarray(image, mode='HSV').convert('RGB')
+        if len(shape) == 3:
+            image = Image.fromarray(image.reshape(shape), mode='RGB').convert('HSV')
+            image = median_filter(
+                image,
+                size=(args.median_strength, args.median_strength, 1))
+            image = Image.fromarray(image, mode='HSV').convert('RGB')
+
+        else:
+            image = median_filter(
+                image.reshape(shape),
+                size=(args.median_strength, args.median_strength))
+
         return np.array(image)
 
     else:
         return image.reshape(shape)
 
 
 def generate_random_string(length=8):
@@ -557,18 +673,18 @@
         filename (pathlib.Path): A new filename that does not conflict with existing files.
     """
 
     if filename.exists():
         while True:
             filename_new = rename_with_random_string(filename)
             if not filename_new.exists():
-                print(f"Renaming the file to: {filename_new}")
+                logging.info(f"Renaming the file to: {filename_new}")
                 return filename_new  # Return the non-conflicting filename
             else:
-                print("Random name still results in a conflict. Generating a new name.")
+                logging.info("Random name still results in a conflict. Generating a new name.")
     else:
         return filename
 
 
 def check_file_and_prompt(filename):
     """
     Check if a file exists and prompt the user to overwrite, exit, or rename the file.
@@ -601,51 +717,35 @@
             elif choice == '' or choice == 'r':
                 filename = handle_file_conflict(filename)
                 break
 
     return filename
 
 
-def save_as_pdf(image, filename, args):
+def save_as_pdf(image, filename, args, idx):
     """
     Saves a single <image> as a PDF <filename>.
 
     Args:
         image (np.array): The image to save
         filename (pathlib.Path): The output file
         args (argparse.Namespace): The command line arguments
 
     Returns:
         None
     """
 
-    verbose_print(args, 'Saving page as {} ...'.format(filename))
+    logging.info('Page {}: Saving page as {} ...'.format(idx, filename))
     pdf = Image.fromarray(image)
     pdf.save(filename, 'PDF',
              dpi=(args.dpi, args.dpi),
              quality=args.quality,
              optimize=True)
 
 
-def verbose_print(args, *message, conditions=[]):
-    """
-    Prints a <message> if all given <conditions> are True.
-
-    Args:
-        args (argparse.Namespace): The command line arguments
-        message (str): The message to be printed.
-        conditions (list of bool): A list of boolean constraints that must all be True for the message to be printed.
-
-    Returns:
-        None
-    """
-    if args.verbose and all(conditions):
-        print(*message)
-
-
 def merge_pdfs(filename_paths, args):
     """
     Merges multiple PDF files <filename_paths> into a single PDF file <args.output> using external ghostscript.
 
     Args:
         filename_paths (list of str / pathlib.Path): The list of the pdf file paths to merge.
         args (argparse.Namespace): The command line arguments
@@ -654,30 +754,30 @@
         None
     """
     filename = args.output
 
     if not args.overwrite:
         filename = check_file_and_prompt(filename)
 
-    verbose_print(args, 'Merging single pages to {} ...'.format(filename))
+    logging.info('Merging single pages to {} ...'.format(filename))
     try:
         command = ['gs',
                    '-dNOPAUSE',
                    '-sDEVICE=pdfwrite',
                    '-sOUTPUTFILE={}'.format(filename),
                    '-dBATCH'] + [str(f) for f in filename_paths]
 
         subprocess.run(command, check=True, capture_output=True)
 
     except subprocess.CalledProcessError as e:
-        print(f"Error: {e}")
-        print("Error:", e.stderr.decode('utf-8') if e.stderr is not None else None)
-        print("Stdout was:", e.stdout.decode('utf-8') if e.stdout is not None else None)
+        logging.critical(f"Error: {e}")
+        logging.critical("Error: {}".format( e.stderr.decode('utf-8') if e.stderr is not None else None) )
+        logging.critical("Stdout was: {}".format( e.stdout.decode('utf-8') if e.stdout is not None else None) )
 
-    verbose_print(args, 'Output written to', args.output)
+    logging.info('Output written to {}'.format(args.output))
 
 
 def process_image(file, output_filename, idx, args, global_palette=None):
     """
     Process a single image and save it as a PDF.
 
     This function performs the following steps:
@@ -697,24 +797,24 @@
     Returns:
         None
     """
     image = io.imread(file)
 
     processed_images = []
 
-    verbose_print(args, 'Processing image {}'.format(idx + 1))
+    logging.info('Processing image {}'.format(idx))
 
     if args.local_palette:
-        color_palette, kmeans_model = create_palette(image, args)
+        color_palette, kmeans_model = create_palette(image, args, idx + 1)
     else:
         color_palette, kmeans_model = global_palette
 
-    image = apply_color_palette(image, color_palette, kmeans_model, args)
+    image = apply_color_palette(image, color_palette, kmeans_model, args, idx + 1)
 
-    save_as_pdf(image, output_filename, args)
+    save_as_pdf(image, output_filename, args, idx + 1)
 
 
 def check_file_existence(files):
     """
     Checks if a file / a list of files exist and raises an error if any are missing.
 
     Args:
@@ -730,20 +830,41 @@
 
     for file in files:
         path = Path(file)
         if not path.exists():
             raise FileNotFoundError(f"File not found: {file}")
 
 
+def check_command_exists(command_name: str):
+    """
+    Checks if a given command exists in the system's PATH.
+
+    Args:
+        command_name (str): The name of the command to check.
+
+    Returns:
+        bool: True if the command is found in the PATH, False otherwise.
+    """
+    if not (shutil.which(command_name) is not None):
+        raise RuntimeError('"{}" not found in PATH! Is it installed?'.format(command_name))
+
+
 def main():
     """
     The main function of the program.
     """
     args = parse_args()
 
+    if args.verbose == 1:
+        logging.basicConfig(encoding='utf-8', format="%(levelname)s:%(message)s", level=logging.INFO)
+    if args.verbose == 2:
+        logging.basicConfig(encoding='utf-8', format="%(lineno)d-%(levelname)s:%(message)s", level=logging.DEBUG)
+
+    check_command_exists('gs')
+
     file_paths = sort_filenames(args.files)
     check_file_existence(file_paths)
 
     # Create a temporary folder at the output file location for storing intermediate PDFs.
     # This way the intermediate files are automatically deleted upon program exit.
     # Each image is converted to a single-page PDF before concatenation
     # afterwards, which reduces the memory footprint.
@@ -771,21 +892,19 @@
                 intermediate_pdf_paths.append(output_filename)
 
             executor.shutdown(wait=True)
             try:
                 for f in threads:
                     f.result()  # This will raise a ValueError in case the thread crashed
             except ValueError as e:
-                print(f"Caught an error: {e}")
+                logging.critical(f"Caught an error: {e}")
+                sys.exit(1)
 
 
-        verbose_print(
-            args,
-            'Skipping the deletion of intermediate PDFs (folder {}).'.format(temp_dir),
-            conditions=[args.keep_intermediate]
-        )
+        if args.keep_intermediate:
+            logging.info('Skipping the deletion of intermediate PDFs (folder {}).'.format(temp_dir))
 
         merge_pdfs(intermediate_pdf_paths, args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `noteshrunk-1.4.2/.gitignore` & `noteshrunk-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.4.2/LICENSE` & `noteshrunk-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.4.2/README.md` & `noteshrunk-1.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 # noteshrunk - Document Color Palette Compression
 
 This Python script compresses images by reducing the number of colors and optimizing the image representation.
-It leverages KMeans clustering for color quantization and offers various options to customize the compression process.
+The idea of the program is to optimize scanned documents.
+It uses KMeans clustering to reduce the number of colors (higher contrast, smaller file size) and offers various options to customize the compression process.
 All supplied images are then saved as a multi-page PDF.
 
-The idea of the program is to optimize scanned documents.
+The color space of the input image (black-and-white / grayscale / color) is preserved as long as you use a local (per page) color palette.
+Otherwise, images with smaller color spaces will be adapted (black-and-white -> grayscale / color or grayscale -> color) to the color space of the image with the largest color space.
+For saving black-and-white images, I recommend having libtiff installed, otherwise it will fall back to using embedded jpeg.
+
 This is a complete and improved rewrite of [mzucker's](https://github.com/mzucker/noteshrink) noteshrink.
 
 ## Features
 
-* **Color Quantization:** Reduces the number of colors in the document using KMeans clustering, leading to smaller file sizes.
-* **Background Detection and Removal:** Identifies and removes the background color.
-* **Customizable Palette:** Allows you to specify the number of colors in the output palette and choose between a global palette for all pages or individual palettes for each page.
-* **Color Control:** Offers the option to maximize saturation in the output image as well as to remove the background (replace with white), enhancing visual clarity.
-* **Denoising Options:** Provides median filtering, morphological opening and unsharp masking to reduce noise and improve image quality.
-* **Parallel processing:** Utilizes multiple CPU cores for faster processing of multiple images.
+* **Color Quantization:** Reduces the number of colors in the document using KMeans clustering, leading to smaller file sizes and higher contrast.
+* **Background Detection and Removal:** Identifies and removes the background color (replace with white), enhancing visual clarity.
+* **Customizable Palette:** Allows you to specify the number of colors in the output palette, maximize saturation and choose between a global palette for all pages or individual palettes for each page.
+* **Denoising Options:** Provides [median filtering](https://en.wikipedia.org/wiki/Median_filter), [morphological opening](https://en.wikipedia.org/wiki/Opening_(morphology)) and [unsharp masking](https://en.wikipedia.org/wiki/Unsharp_masking) to reduce noise and improve image quality.
+* **Parallel processing:** Multi-threading for faster processing of multiple images.
+* **Low memory profile**: Trys to keep memory usage as small as possible. This is done by:
+  * Each page is converted separately
+  * The intermediate files are stored in the current working directory (so that you can choose between disk and RAM [e.g. `/tmp`])
+  * The library functions and programs used are specifically chosen to have the smallest overhead
+  * The input color space is preserved, if possible.
 
 ## Examples
 
 ### Generic Example
 
 <table>
   <tr>
@@ -104,14 +112,18 @@
 - scikit-learn
 - SciPy
 
 ### Other
 
 - Ghostscript (executable `gs` in PATH - for PDF merging)
 
+### Optional Dependencies
+
+- `libtiff` for much smaller file sizes on black-and-white images.
+
 ## Installation
 
 ```bash
 pipx install noteshrunk
 ```
 
 ## Usage
```

#### html2text {}

```diff
@@ -1,25 +1,37 @@
 # noteshrunk - Document Color Palette Compression This Python script compresses
 images by reducing the number of colors and optimizing the image
-representation. It leverages KMeans clustering for color quantization and
-offers various options to customize the compression process. All supplied
-images are then saved as a multi-page PDF. The idea of the program is to
-optimize scanned documents. This is a complete and improved rewrite of
-[mzucker's](https://github.com/mzucker/noteshrink) noteshrink. ## Features *
-**Color Quantization:** Reduces the number of colors in the document using
-KMeans clustering, leading to smaller file sizes. * **Background Detection and
-Removal:** Identifies and removes the background color. * **Customizable
-Palette:** Allows you to specify the number of colors in the output palette and
-choose between a global palette for all pages or individual palettes for each
-page. * **Color Control:** Offers the option to maximize saturation in the
-output image as well as to remove the background (replace with white),
-enhancing visual clarity. * **Denoising Options:** Provides median filtering,
-morphological opening and unsharp masking to reduce noise and improve image
-quality. * **Parallel processing:** Utilizes multiple CPU cores for faster
-processing of multiple images. ## Examples ### Generic Example
+representation. The idea of the program is to optimize scanned documents. It
+uses KMeans clustering to reduce the number of colors (higher contrast, smaller
+file size) and offers various options to customize the compression process. All
+supplied images are then saved as a multi-page PDF. The color space of the
+input image (black-and-white / grayscale / color) is preserved as long as you
+use a local (per page) color palette. Otherwise, images with smaller color
+spaces will be adapted (black-and-white -> grayscale / color or grayscale -
+> color) to the color space of the image with the largest color space. For
+saving black-and-white images, I recommend having libtiff installed, otherwise
+it will fall back to using embedded jpeg. This is a complete and improved
+rewrite of [mzucker's](https://github.com/mzucker/noteshrink) noteshrink. ##
+Features * **Color Quantization:** Reduces the number of colors in the document
+using KMeans clustering, leading to smaller file sizes and higher contrast. *
+**Background Detection and Removal:** Identifies and removes the background
+color (replace with white), enhancing visual clarity. * **Customizable Palette:
+** Allows you to specify the number of colors in the output palette, maximize
+saturation and choose between a global palette for all pages or individual
+palettes for each page. * **Denoising Options:** Provides [median filtering]
+(https://en.wikipedia.org/wiki/Median_filter), [morphological opening](https://
+en.wikipedia.org/wiki/Opening_(morphology)) and [unsharp masking](https://
+en.wikipedia.org/wiki/Unsharp_masking) to reduce noise and improve image
+quality. * **Parallel processing:** Multi-threading for faster processing of
+multiple images. * **Low memory profile**: Trys to keep memory usage as small
+as possible. This is done by: * Each page is converted separately * The
+intermediate files are stored in the current working directory (so that you can
+choose between disk and RAM [e.g. `/tmp`]) * The library functions and programs
+used are specifically chosen to have the smallest overhead * The input color
+space is preserved, if possible. ## Examples ### Generic Example
 [Original Image] [Processed Image]
 Original Image   noteshrunk -w -s --unsharp_mask -ur 2 -ua 1
 Image Source: https://commons.wikimedia.org/wiki/File:BREAKFAST_
 (held_by)_NIPPON_YUSEN_KAISHA_-_S.S.KOBE_MARU_(at)_EN_ROUTE_(SS)_(NYPL_Hades-
 274833-469108).jpg ### Fine / Low Resolution Text Morphological Opening
 swallows fine structures, but unsharp masking helps preserve them.
 [Original Image]
@@ -37,44 +49,46 @@
 Examples 1. Compress a single image with default settings: ```bash noteshrunk
 input.png ``` 2. Compress multiple images with a white background and 16
 colors: ```bash noteshrunk -w -n 16 image1.jpg image2.png ``` 3. Compress
 images using a local color palette and keep intermediate files while disabling
 multi-threading: ```bash noteshrunk -l -j 1 -k *.jpg ``` ## Requirements ###
 Python Packages - argcomplete - NumPy - Pillow (PIL Fork) - Python 3 - scikit-
 image - scikit-learn - SciPy ### Other - Ghostscript (executable `gs` in PATH -
-for PDF merging) ## Installation ```bash pipx install noteshrunk ``` ## Usage
-``` noteshrunk [-h] [-o OUTPUT] [-w] [-s] [-n N_COLORS] [-d DPI] [-q [1-100]]
-[-l] [-p PERCENTAGE] [-j JOBS] [-y] [-ts THRESHOLD_SATURATION] [-tv
-THRESHOLD_VALUE] [--denoise_median] [--denoise_opening] [--unsharp_mask] [-ms
-MEDIAN_STRENGTH] [-cs CLOSING_STRENGTH] [-ua UNSHARP_AMOUNT] [-ur
-UNSHARP_RADIUS] [-k] [-v] [--version] files [files ...] ``` ### Arguments *
-`files`: A list of paths to the input image files. * `-o`, `--output`: Path to
-the output PDF file (default: `output.pdf`). * `-w`, `--white_background`: Use
-white background instead of dominant color. * `-s`, `--saturate`: Maximize
-saturation in the output image. * `-n`, `--n_colors`: Number of colors in the
-palette (default: 8). * `-d`, `--dpi`: DPI value of the input images (default:
-300). * `-q`, `--quality`: JPEG quality of the images embedded in the PDF (1-
-100, default: 75). * `-l`, `--local_palette`: Create an individual color
-palette for each image (by sampling a -p percentage of the pixels of that
-image) instead of a global palette (by sampling a -p percentage of the pixels
-of each input image). * `-p`, `--percentage`: Percentage of pixels to sample
-from each input image for color palette creation (default: 10). * `-j`, `--
-jobs`: Number of threads to use for multi-threading (default: number of CPU
-cores). * `-y`, `--overwrite`: Overwrite existing files without asking. * `-
-ts`, `--threshold_saturation`: HSV saturation threshold (in percent) used for
-background detection (default: 15). * `-tv`, `--threshold_value`: HSV value
-threshold (in percent) used for background detection (default: 25). * `--
-denoise_median`: Apply median denoising on the output image with strength `-
-ms`. * `-ms`, `--median_strength`: Strength of median filtering (default: 3). *
-`--denoise_opening`: Apply morphological opening on the background mask with
-strength `-os`. * `-os`, `--opening_strength`: Strength of opening filtering /
-radius of the structuring element (disk, default: 3). * `--unsharp_mask`: Apply
-unsharp masking on the final image with radius `-ur` and amount `-ua`. * `-ur`,
-`-ua`: Radius and Amount used for unsharp masking. * `-k`, `--
-keep_intermediate`: Keep the intermediate single-page PDFs. * `-v`, `--
-verbose`: Verbose output. * `--version`: Show program version and exit. ##
-Contributing Contributions are welcome! Please feel free to submit issues or
-pull requests on the GitHub repository. ## Acknowledgements This project
-utilizes open-source software from the Python community. Special thanks to the
-developers and maintainers of the required libraries as well as [mzucker's]
-(https://github.com/mzucker/noteshrink) initial program. ## License This
-project is licensed under the MIT License. See the `LICENSE` file for details.
+for PDF merging) ### Optional Dependencies - `libtiff` for much smaller file
+sizes on black-and-white images. ## Installation ```bash pipx install
+noteshrunk ``` ## Usage ``` noteshrunk [-h] [-o OUTPUT] [-w] [-s] [-n N_COLORS]
+[-d DPI] [-q [1-100]] [-l] [-p PERCENTAGE] [-j JOBS] [-y] [-ts
+THRESHOLD_SATURATION] [-tv THRESHOLD_VALUE] [--denoise_median] [--
+denoise_opening] [--unsharp_mask] [-ms MEDIAN_STRENGTH] [-cs CLOSING_STRENGTH]
+[-ua UNSHARP_AMOUNT] [-ur UNSHARP_RADIUS] [-k] [-v] [--version] files [files
+...] ``` ### Arguments * `files`: A list of paths to the input image files. *
+`-o`, `--output`: Path to the output PDF file (default: `output.pdf`). * `-w`,
+`--white_background`: Use white background instead of dominant color. * `-s`,
+`--saturate`: Maximize saturation in the output image. * `-n`, `--n_colors`:
+Number of colors in the palette (default: 8). * `-d`, `--dpi`: DPI value of the
+input images (default: 300). * `-q`, `--quality`: JPEG quality of the images
+embedded in the PDF (1-100, default: 75). * `-l`, `--local_palette`: Create an
+individual color palette for each image (by sampling a -p percentage of the
+pixels of that image) instead of a global palette (by sampling a -p percentage
+of the pixels of each input image). * `-p`, `--percentage`: Percentage of
+pixels to sample from each input image for color palette creation (default:
+10). * `-j`, `--jobs`: Number of threads to use for multi-threading (default:
+number of CPU cores). * `-y`, `--overwrite`: Overwrite existing files without
+asking. * `-ts`, `--threshold_saturation`: HSV saturation threshold (in
+percent) used for background detection (default: 15). * `-tv`, `--
+threshold_value`: HSV value threshold (in percent) used for background
+detection (default: 25). * `--denoise_median`: Apply median denoising on the
+output image with strength `-ms`. * `-ms`, `--median_strength`: Strength of
+median filtering (default: 3). * `--denoise_opening`: Apply morphological
+opening on the background mask with strength `-os`. * `-os`, `--
+opening_strength`: Strength of opening filtering / radius of the structuring
+element (disk, default: 3). * `--unsharp_mask`: Apply unsharp masking on the
+final image with radius `-ur` and amount `-ua`. * `-ur`, `-ua`: Radius and
+Amount used for unsharp masking. * `-k`, `--keep_intermediate`: Keep the
+intermediate single-page PDFs. * `-v`, `--verbose`: Verbose output. * `--
+version`: Show program version and exit. ## Contributing Contributions are
+welcome! Please feel free to submit issues or pull requests on the GitHub
+repository. ## Acknowledgements This project utilizes open-source software from
+the Python community. Special thanks to the developers and maintainers of the
+required libraries as well as [mzucker's](https://github.com/mzucker/
+noteshrink) initial program. ## License This project is licensed under the MIT
+License. See the `LICENSE` file for details.
```

### Comparing `noteshrunk-1.4.2/pyproject.toml` & `noteshrunk-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "noteshrunk"
-version = "1.4.2"
+version = "1.5.0"
 description = "Document Color Palette Compression"
 readme = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "suuuehgi"}
 ]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `noteshrunk-1.4.2/PKG-INFO` & `noteshrunk-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: noteshrunk
-Version: 1.4.2
+Version: 1.5.0
 Summary: Document Color Palette Compression
 Project-URL: Homepage, https://github.com/suuuehgi/noteshrunk
 Project-URL: Issues, https://github.com/suuuehgi/noteshrunk/issues
 Author: suuuehgi
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -679,40 +679,48 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Requires-Dist: argcomplete
 Requires-Dist: numpy
 Requires-Dist: pillow
 Requires-Dist: scikit-image
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Description-Content-Type: text/markdown
 
 # noteshrunk - Document Color Palette Compression
 
 This Python script compresses images by reducing the number of colors and optimizing the image representation.
-It leverages KMeans clustering for color quantization and offers various options to customize the compression process.
+The idea of the program is to optimize scanned documents.
+It uses KMeans clustering to reduce the number of colors (higher contrast, smaller file size) and offers various options to customize the compression process.
 All supplied images are then saved as a multi-page PDF.
 
-The idea of the program is to optimize scanned documents.
+The color space of the input image (black-and-white / grayscale / color) is preserved as long as you use a local (per page) color palette.
+Otherwise, images with smaller color spaces will be adapted (black-and-white -> grayscale / color or grayscale -> color) to the color space of the image with the largest color space.
+For saving black-and-white images, I recommend having libtiff installed, otherwise it will fall back to using embedded jpeg.
+
 This is a complete and improved rewrite of [mzucker's](https://github.com/mzucker/noteshrink) noteshrink.
 
 ## Features
 
-* **Color Quantization:** Reduces the number of colors in the document using KMeans clustering, leading to smaller file sizes.
-* **Background Detection and Removal:** Identifies and removes the background color.
-* **Customizable Palette:** Allows you to specify the number of colors in the output palette and choose between a global palette for all pages or individual palettes for each page.
-* **Color Control:** Offers the option to maximize saturation in the output image as well as to remove the background (replace with white), enhancing visual clarity.
-* **Denoising Options:** Provides median filtering, morphological opening and unsharp masking to reduce noise and improve image quality.
-* **Parallel processing:** Utilizes multiple CPU cores for faster processing of multiple images.
+* **Color Quantization:** Reduces the number of colors in the document using KMeans clustering, leading to smaller file sizes and higher contrast.
+* **Background Detection and Removal:** Identifies and removes the background color (replace with white), enhancing visual clarity.
+* **Customizable Palette:** Allows you to specify the number of colors in the output palette, maximize saturation and choose between a global palette for all pages or individual palettes for each page.
+* **Denoising Options:** Provides [median filtering](https://en.wikipedia.org/wiki/Median_filter), [morphological opening](https://en.wikipedia.org/wiki/Opening_(morphology)) and [unsharp masking](https://en.wikipedia.org/wiki/Unsharp_masking) to reduce noise and improve image quality.
+* **Parallel processing:** Multi-threading for faster processing of multiple images.
+* **Low memory profile**: Trys to keep memory usage as small as possible. This is done by:
+  * Each page is converted separately
+  * The intermediate files are stored in the current working directory (so that you can choose between disk and RAM [e.g. `/tmp`])
+  * The library functions and programs used are specifically chosen to have the smallest overhead
+  * The input color space is preserved, if possible.
 
 ## Examples
 
 ### Generic Example
 
 <table>
   <tr>
@@ -798,14 +806,18 @@
 - scikit-learn
 - SciPy
 
 ### Other
 
 - Ghostscript (executable `gs` in PATH - for PDF merging)
 
+### Optional Dependencies
+
+- `libtiff` for much smaller file sizes on black-and-white images.
+
 ## Installation
 
 ```bash
 pipx install noteshrunk
 ```
 
 ## Usage
```


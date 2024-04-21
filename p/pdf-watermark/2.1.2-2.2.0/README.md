# Comparing `tmp/pdf-watermark-2.1.2.tar.gz` & `tmp/pdf_watermark-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf-watermark-2.1.2.tar", last modified: Fri Mar 29 17:55:17 2024, max compression
+gzip compressed data, was "pdf_watermark-2.2.0.tar", last modified: Sun Apr 21 11:31:57 2024, max compression
```

## Comparing `pdf-watermark-2.1.2.tar` & `pdf_watermark-2.2.0.tar`

### file list

```diff
@@ -1,40 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:55:17.285547 pdf-watermark-2.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:55:17.277547 pdf-watermark-2.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:55:17.281547 pdf-watermark-2.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/.github/workflows/lint-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-03-29 17:55:17.285547 pdf-watermark-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:55:17.281547 pdf-watermark-2.1.2/images/
--rw-r--r--   0 runner    (1001) docker     (127)   241473 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/images/before.png
--rw-r--r--   0 runner    (1001) docker     (127)   361202 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/images/image.png
--rw-r--r--   0 runner    (1001) docker     (127)   272309 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/images/text.png
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 17:55:17.285547 pdf-watermark-2.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:55:17.277547 pdf-watermark-2.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:55:17.281547 pdf-watermark-2.1.2/src/pdf_watermark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/src/pdf_watermark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-29 17:55:17.000000 pdf-watermark-2.1.2/src/pdf_watermark/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/src/pdf_watermark/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/src/pdf_watermark/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/src/pdf_watermark/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/src/pdf_watermark/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/src/pdf_watermark/watermark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:55:17.285547 pdf-watermark-2.1.2/src/pdf_watermark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-03-29 17:55:17.000000 pdf-watermark-2.1.2/src/pdf_watermark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-29 17:55:17.000000 pdf-watermark-2.1.2/src/pdf_watermark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 17:55:17.000000 pdf-watermark-2.1.2/src/pdf_watermark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-29 17:55:17.000000 pdf-watermark-2.1.2/src/pdf_watermark.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-29 17:55:17.000000 pdf-watermark-2.1.2/src/pdf_watermark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-29 17:55:17.000000 pdf-watermark-2.1.2/src/pdf_watermark.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:55:17.281547 pdf-watermark-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:55:17.285547 pdf-watermark-2.1.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/tests/fixtures/0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/tests/fixtures/1.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/tests/fixtures/input.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-03-29 17:55:12.000000 pdf-watermark-2.1.2/tests/test_add_watermark_from_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.470016 pdf_watermark-2.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.462016 pdf_watermark-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.466016 pdf_watermark-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/.github/workflows/lint-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-04-21 11:31:57.470016 pdf_watermark-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8766 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.466016 pdf_watermark-2.2.0/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   241473 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/images/before.png
+-rw-r--r--   0 runner    (1001) docker     (127)   361202 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/images/image.png
+-rw-r--r--   0 runner    (1001) docker     (127)   272309 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/images/text.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 11:31:57.470016 pdf_watermark-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.462016 pdf_watermark-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.470016 pdf_watermark-2.2.0/src/pdf_watermark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/src/pdf_watermark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 11:31:57.000000 pdf_watermark-2.2.0/src/pdf_watermark/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/src/pdf_watermark/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/src/pdf_watermark/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/src/pdf_watermark/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/src/pdf_watermark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/src/pdf_watermark/watermark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.470016 pdf_watermark-2.2.0/src/pdf_watermark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-04-21 11:31:57.000000 pdf_watermark-2.2.0/src/pdf_watermark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-21 11:31:57.000000 pdf_watermark-2.2.0/src/pdf_watermark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 11:31:57.000000 pdf_watermark-2.2.0/src/pdf_watermark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-21 11:31:57.000000 pdf_watermark-2.2.0/src/pdf_watermark.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-21 11:31:57.000000 pdf_watermark-2.2.0/src/pdf_watermark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 11:31:57.000000 pdf_watermark-2.2.0/src/pdf_watermark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.470016 pdf_watermark-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.470016 pdf_watermark-2.2.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/fixtures/0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/fixtures/1.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/fixtures/different_sizes_input.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/fixtures/different_sizes_output.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/fixtures/input.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/test_add_watermark_from_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/test_different_page_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/utils.py
```

### Comparing `pdf-watermark-2.1.2/.github/workflows/lint-and-test.yml` & `pdf_watermark-2.2.0/.github/workflows/lint-and-test.yml`

 * *Files identical despite different names*

### Comparing `pdf-watermark-2.1.2/.github/workflows/publish-to-pypi.yml` & `pdf_watermark-2.2.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pdf-watermark-2.1.2/LICENSE` & `pdf_watermark-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdf-watermark-2.1.2/PKG-INFO` & `pdf_watermark-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-watermark
-Version: 2.1.2
+Version: 2.2.0
 Summary: A python CLI tool to add watermarks to a PDF
 Author-email: Bastien Le Chenadec <bastien.lechenadec@gmail.com>
 License: MIT License
         
         Copyright (c) [2023] [Bastien Le Chenadec]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -77,14 +77,21 @@
 
 ```
 pip install pdf-watermark
 ```
 
 ### Usage
 
+**TLDR**
+```bash
+watermark grid input.pdf "watermark text" -s output.pdf # Grid pattern for a single file
+watermark insert input_folder "watermark_image.png" # Insert image for a whole directory, overwriting the input files
+```
+
+**Detailed usage**
 ```
 Usage: watermark [OPTIONS] COMMAND [ARGS]...
 
   Add a watermark to one or more PDF files.
 
   The watermark can be repeated in a grid pattern using the grid command, or
   inserted at a specific position using the insert command.
@@ -225,14 +232,16 @@
     * Add **insert** command.
 * 2.1.0
     * Add --unselectable and --save-as-image options.
     * Fix bug with temporary files on Windows.
 * 2.1.2
     * Fix missing Poppler dependancy.
     * Add test and lint to CI.
+* 2.2.0
+    * Support PDFs with pages of different sizes.
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Acknowledgments
```

### Comparing `pdf-watermark-2.1.2/README.md` & `pdf_watermark-2.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,21 @@
 
 ```
 pip install pdf-watermark
 ```
 
 ### Usage
 
+**TLDR**
+```bash
+watermark grid input.pdf "watermark text" -s output.pdf # Grid pattern for a single file
+watermark insert input_folder "watermark_image.png" # Insert image for a whole directory, overwriting the input files
+```
+
+**Detailed usage**
 ```
 Usage: watermark [OPTIONS] COMMAND [ARGS]...
 
   Add a watermark to one or more PDF files.
 
   The watermark can be repeated in a grid pattern using the grid command, or
   inserted at a specific position using the insert command.
@@ -184,14 +191,16 @@
     * Add **insert** command.
 * 2.1.0
     * Add --unselectable and --save-as-image options.
     * Fix bug with temporary files on Windows.
 * 2.1.2
     * Fix missing Poppler dependancy.
     * Add test and lint to CI.
+* 2.2.0
+    * Support PDFs with pages of different sizes.
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Acknowledgments
```

### Comparing `pdf-watermark-2.1.2/images/before.png` & `pdf_watermark-2.2.0/images/before.png`

 * *Files identical despite different names*

### Comparing `pdf-watermark-2.1.2/images/image.png` & `pdf_watermark-2.2.0/images/image.png`

 * *Files identical despite different names*

### Comparing `pdf-watermark-2.1.2/images/text.png` & `pdf_watermark-2.2.0/images/text.png`

 * *Files identical despite different names*

### Comparing `pdf-watermark-2.1.2/pyproject.toml` & `pdf_watermark-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdf-watermark-2.1.2/src/pdf_watermark/draw.py` & `pdf_watermark-2.2.0/src/pdf_watermark/draw.py`

 * *Files identical despite different names*

### Comparing `pdf-watermark-2.1.2/src/pdf_watermark/handler.py` & `pdf_watermark-2.2.0/src/pdf_watermark/handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,59 +7,71 @@
 from pdf_watermark.draw import draw_watermarks
 from pdf_watermark.options import (
     DrawingOptions,
     FilesOptions,
     GridOptions,
     InsertOptions,
 )
-from pdf_watermark.utils import convert_content_to_images
+from pdf_watermark.utils import convert_content_to_images, sort_pages
 
 
 def add_watermark_to_pdf(
     input: str,
     output: str,
     drawing_options: DrawingOptions,
     specific_options: Union[GridOptions, InsertOptions],
 ):
+    pdf_writer = pypdf.PdfWriter()
     pdf_to_transform = pypdf.PdfReader(input)
-    pdf_box = pdf_to_transform.pages[0].mediabox
-    page_width = pdf_box.width
-    page_height = pdf_box.height
-
-    with NamedTemporaryFile(delete=False) as temporary_file:
-        # The watermark is stored in a temporary pdf file
-        draw_watermarks(
-            temporary_file.name,
-            page_width,
-            page_height,
-            drawing_options,
-            specific_options,
-        )
-
-        if drawing_options.unselectable and not drawing_options.save_as_image:
-            convert_content_to_images(
-                temporary_file.name, page_width, page_height, drawing_options.dpi
+
+    page_sizes = []
+    for page in pdf_to_transform.pages:
+        page_sizes.append((page.mediabox.width, page.mediabox.height))
+
+    order = []
+    # Only one watermark is computed per page size
+    for watermark_width, watermark_height in set(page_sizes):
+        with NamedTemporaryFile(delete=False) as temporary_file:
+            # The watermark is stored in a temporary pdf file
+            draw_watermarks(
+                temporary_file.name,
+                watermark_width,
+                watermark_height,
+                drawing_options,
+                specific_options,
             )
 
-        watermark_pdf = pypdf.PdfReader(temporary_file.name)
-        pdf_writer = pypdf.PdfWriter()
+            if drawing_options.unselectable and not drawing_options.save_as_image:
+                convert_content_to_images(
+                    temporary_file.name,
+                    drawing_options.dpi,
+                )
+
+            watermark_pdf = pypdf.PdfReader(temporary_file.name)
+
+            # Add watermark to pages with the same size
+            for index, (page, (page_width, page_height)) in enumerate(
+                zip(pdf_to_transform.pages, page_sizes)
+            ):
+                if page_width == watermark_width and page_height == watermark_height:
+                    page.merge_page(watermark_pdf.pages[0])
+                    pdf_writer.add_page(page)
+                    order.append(index)
+
+            # Remove temp file - https://stackoverflow.com/questions/23212435/permission-denied-to  -write-to-my-temporary-file
+            temporary_file.close()
+            os.unlink(temporary_file.name)
 
-        for page in pdf_to_transform.pages:
-            page.merge_page(watermark_pdf.pages[0])
-            pdf_writer.add_page(page)
-
-        # Remove temp file - https://stackoverflow.com/questions/23212435/permission-denied-to-write-to-my-temporary-file
-        temporary_file.close()
-        os.unlink(temporary_file.name)
+    pdf_writer = sort_pages(pdf_writer, order)
 
     with open(output, "wb") as f:
         pdf_writer.write(f)
 
     if drawing_options.save_as_image:
-        convert_content_to_images(output, page_width, page_height, drawing_options.dpi)
+        convert_content_to_images(output, drawing_options.dpi)
 
 
 def add_watermark_from_options(
     files_options: FilesOptions,
     drawing_options: DrawingOptions,
     specific_options: Union[GridOptions, InsertOptions],
 ):
```

### Comparing `pdf-watermark-2.1.2/src/pdf_watermark/options.py` & `pdf_watermark-2.2.0/src/pdf_watermark/options.py`

 * *Files identical despite different names*

### Comparing `pdf-watermark-2.1.2/src/pdf_watermark/utils.py` & `pdf_watermark-2.2.0/src/pdf_watermark/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from io import BytesIO
-from typing import Tuple
+from typing import List, Tuple
 
 import numpy as np
+import pypdf
 from pdf2image import convert_from_path
 from pdf2image.exceptions import PopplerNotInstalledError
 from reportlab.lib.utils import ImageReader
 from reportlab.pdfgen import canvas
 
 
 def draw_centered_image(
@@ -47,35 +48,50 @@
 
     image_width *= scale
     image_height *= scale
 
     return image_width, image_height
 
 
-def convert_content_to_images(
-    file_name: str, page_width: int, page_height: int, dpi: int
-):
+def convert_content_to_images(file_name: str, dpi: int):
+    # load pages as images
     try:
         images = convert_from_path(file_name, dpi=dpi, fmt="png", transparent=True)
     except PopplerNotInstalledError:
         print(
             "Warning : the --save-as-image and --unselectable options require poppler to be installed. Proceeding without these options. Pleaser refer to the documentation for more information."
         )
         return None
 
-    pdf = canvas.Canvas(file_name, pagesize=(page_width, page_height))
+    # get the page sizes
+    pdf_to_transform = pypdf.PdfReader(file_name)
+    page_sizes = []
+    for page in pdf_to_transform.pages:
+        page_sizes.append((page.mediabox.width, page.mediabox.height))
+
+    # create new pdf
+    pdf = canvas.Canvas(file_name)
 
-    for image in images:
+    for image, (page_width, page_height) in zip(images, page_sizes):
+        pdf.setPageSize((page_width, page_height))
         compressed = BytesIO()
         image.save(compressed, format="png", optimize=True, quality=dpi // 10)
 
         pdf.drawImage(
             ImageReader(compressed),
             0,
             0,
             width=page_width,
             height=page_height,
             mask="auto",
         )
         pdf.showPage()
 
     pdf.save()
+
+
+def sort_pages(pdf: pypdf.PdfWriter, order: List[int]):
+    output = pypdf.PdfWriter()
+    for index in np.argsort(order):
+        output.add_page(pdf.pages[int(index)])
+
+    return output
```

### Comparing `pdf-watermark-2.1.2/src/pdf_watermark/watermark.py` & `pdf_watermark-2.2.0/src/pdf_watermark/watermark.py`

 * *Files identical despite different names*

### Comparing `pdf-watermark-2.1.2/src/pdf_watermark.egg-info/PKG-INFO` & `pdf_watermark-2.2.0/src/pdf_watermark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-watermark
-Version: 2.1.2
+Version: 2.2.0
 Summary: A python CLI tool to add watermarks to a PDF
 Author-email: Bastien Le Chenadec <bastien.lechenadec@gmail.com>
 License: MIT License
         
         Copyright (c) [2023] [Bastien Le Chenadec]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -77,14 +77,21 @@
 
 ```
 pip install pdf-watermark
 ```
 
 ### Usage
 
+**TLDR**
+```bash
+watermark grid input.pdf "watermark text" -s output.pdf # Grid pattern for a single file
+watermark insert input_folder "watermark_image.png" # Insert image for a whole directory, overwriting the input files
+```
+
+**Detailed usage**
 ```
 Usage: watermark [OPTIONS] COMMAND [ARGS]...
 
   Add a watermark to one or more PDF files.
 
   The watermark can be repeated in a grid pattern using the grid command, or
   inserted at a specific position using the insert command.
@@ -225,14 +232,16 @@
     * Add **insert** command.
 * 2.1.0
     * Add --unselectable and --save-as-image options.
     * Fix bug with temporary files on Windows.
 * 2.1.2
     * Fix missing Poppler dependancy.
     * Add test and lint to CI.
+* 2.2.0
+    * Support PDFs with pages of different sizes.
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Acknowledgments
```

### Comparing `pdf-watermark-2.1.2/src/pdf_watermark.egg-info/SOURCES.txt` & `pdf_watermark-2.2.0/src/pdf_watermark.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -20,10 +20,14 @@
 src/pdf_watermark.egg-info/SOURCES.txt
 src/pdf_watermark.egg-info/dependency_links.txt
 src/pdf_watermark.egg-info/entry_points.txt
 src/pdf_watermark.egg-info/requires.txt
 src/pdf_watermark.egg-info/top_level.txt
 tests/__init__.py
 tests/test_add_watermark_from_options.py
+tests/test_different_page_sizes.py
+tests/utils.py
 tests/fixtures/0.pdf
 tests/fixtures/1.pdf
+tests/fixtures/different_sizes_input.pdf
+tests/fixtures/different_sizes_output.pdf
 tests/fixtures/input.pdf
```

### Comparing `pdf-watermark-2.1.2/tests/fixtures/0.pdf` & `pdf_watermark-2.2.0/tests/fixtures/0.pdf`

 * *Files identical despite different names*

### Comparing `pdf-watermark-2.1.2/tests/fixtures/1.pdf` & `pdf_watermark-2.2.0/tests/fixtures/1.pdf`

 * *Files identical despite different names*

### Comparing `pdf-watermark-2.1.2/tests/fixtures/input.pdf` & `pdf_watermark-2.2.0/tests/fixtures/input.pdf`

 * *Files identical despite different names*

### Comparing `pdf-watermark-2.1.2/tests/test_add_watermark_from_options.py` & `pdf_watermark-2.2.0/tests/test_add_watermark_from_options.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
 Test the outputs of the CLI with a bunch of different options on simple features. These tests are far from perfect.
 """
 
 import os
 
-import numpy as np
 import pytest
-from pdf2image import convert_from_path
 
 from pdf_watermark.handler import add_watermark_from_options
 from pdf_watermark.options import (
     DrawingOptions,
     FilesOptions,
     GridOptions,
     InsertOptions,
 )
 from pdf_watermark.watermark import DEFAULTS
+from tests.utils import assert_pdfs_are_close
 
 INPUT = "tests/fixtures/input.pdf"
 OUTPUT = "output.pdf"
 FIXTURES = ["tests/fixtures/0.pdf", "tests/fixtures/1.pdf"]
 
 
 @pytest.fixture(autouse=True)
@@ -58,23 +57,14 @@
         y=DEFAULTS.y,
         x=DEFAULTS.x,
         horizontal_alignment=DEFAULTS.horizontal_alignment,
     )
 ]
 
 
-def assert_pdfs_are_close(path_1: str, path_2: str, epsilon: float = 1e-10):
-    """This function checks that two PDFs are close enough. We chose to convert the PDFs to images and then compare their L1 norms, because other techniques (hashing for instance) might break easily."""
-    images_1 = convert_from_path(path_1)
-    images_2 = convert_from_path(path_2)
-
-    for im1, im2 in zip(images_1, images_2):
-        assert np.sum(np.abs(np.array(im1) - np.array(im2))) < epsilon
-
-
 def test_add_watermark_from_options():
     index = 0
     for files_options in FILES_OPTIONS_FIXTURES:
         for drawing_options in DRAWING_OPTIONS_FIXTURES:
             for specific_options in GRID_OPTIONS_FIXTURES + INSERT_OPTIONS_FIXTURES:
                 add_watermark_from_options(
                     files_options=files_options,
```


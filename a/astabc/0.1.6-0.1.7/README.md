# Comparing `tmp/astabc-0.1.6.tar.gz` & `tmp/astabc-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astabc-0.1.6.tar", last modified: Sat Apr 20 11:18:58 2024, max compression
+gzip compressed data, was "astabc-0.1.7.tar", last modified: Sun Apr 21 00:14:45 2024, max compression
```

## Comparing `astabc-0.1.6.tar` & `astabc-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-20 11:18:58.321298 astabc-0.1.6/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-04-12 07:46:41.000000 astabc-0.1.6/LICENSE
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1120 2024-04-20 11:18:58.321298 astabc-0.1.6/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      701 2024-04-12 07:32:42.000000 astabc-0.1.6/README.md
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-20 11:18:58.321298 astabc-0.1.6/astabc/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       58 2024-04-12 07:32:31.000000 astabc-0.1.6/astabc/__init__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2512 2024-04-20 11:18:46.000000 astabc-0.1.6/astabc/astabc.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-20 11:18:58.321298 astabc-0.1.6/astabc.egg-info/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1120 2024-04-20 11:18:58.000000 astabc-0.1.6/astabc.egg-info/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      265 2024-04-20 11:18:58.000000 astabc-0.1.6/astabc.egg-info/SOURCES.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-04-20 11:18:58.000000 astabc-0.1.6/astabc.egg-info/dependency_links.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       71 2024-04-20 11:18:58.000000 astabc-0.1.6/astabc.egg-info/entry_points.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       14 2024-04-20 11:18:58.000000 astabc-0.1.6/astabc.egg-info/requires.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        7 2024-04-20 11:18:58.000000 astabc-0.1.6/astabc.egg-info/top_level.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-04-20 11:18:58.321298 astabc-0.1.6/setup.cfg
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      755 2024-04-20 11:18:56.000000 astabc-0.1.6/setup.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-20 11:18:58.321298 astabc-0.1.6/tests/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1313 2024-04-12 07:32:38.000000 astabc-0.1.6/tests/test_astabc.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-21 00:14:45.055856 astabc-0.1.7/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-04-12 07:46:41.000000 astabc-0.1.7/LICENSE
+-rw-r--r--   0 jgi       (1000) jgi       (1000)     1149 2024-04-21 00:14:45.055856 astabc-0.1.7/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      701 2024-04-12 07:32:42.000000 astabc-0.1.7/README.md
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-21 00:14:45.055856 astabc-0.1.7/astabc/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       58 2024-04-12 07:32:31.000000 astabc-0.1.7/astabc/__init__.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2648 2024-04-21 00:14:16.000000 astabc-0.1.7/astabc/astabc.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-21 00:14:45.055856 astabc-0.1.7/astabc.egg-info/
+-rw-r--r--   0 jgi       (1000) jgi       (1000)     1149 2024-04-21 00:14:44.000000 astabc-0.1.7/astabc.egg-info/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      265 2024-04-21 00:14:45.000000 astabc-0.1.7/astabc.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-04-21 00:14:44.000000 astabc-0.1.7/astabc.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       71 2024-04-21 00:14:44.000000 astabc-0.1.7/astabc.egg-info/entry_points.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       14 2024-04-21 00:14:44.000000 astabc-0.1.7/astabc.egg-info/requires.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        7 2024-04-21 00:14:44.000000 astabc-0.1.7/astabc.egg-info/top_level.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-04-21 00:14:45.055856 astabc-0.1.7/setup.cfg
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      755 2024-04-21 00:14:43.000000 astabc-0.1.7/setup.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-21 00:14:45.055856 astabc-0.1.7/tests/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1313 2024-04-12 07:32:38.000000 astabc-0.1.7/tests/test_astabc.py
```

### Comparing `astabc-0.1.6/LICENSE` & `astabc-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `astabc-0.1.6/PKG-INFO` & `astabc-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: astabc
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python module for automatic brightness and contrast optimization
 Home-page: https://github.com/jgwill/gia-abc
 Author: Guillaume Descoteaux-Isabelle
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: opencv-python
 
 # astabc
 
 The `astabc` module is a Python module that provides functions for automatic brightness and contrast optimization of images.
 
 ## Installation
```

### Comparing `astabc-0.1.6/README.md` & `astabc-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `astabc-0.1.6/astabc/astabc.py` & `astabc-0.1.7/astabc/astabc.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,40 +30,47 @@
         maximum_gray -= 1
     
     alpha = 255 / (maximum_gray - minimum_gray)
     beta = -minimum_gray * alpha
     
     auto_result = cv2.convertScaleAbs(image, alpha=alpha, beta=beta)
     return (auto_result, alpha, beta)
+
 def correct(filename, abc=25, output_filename=None):
     img = _read_image(filename)
     img, alpha, beta = _automatic_brightness_and_contrast(img, abc)
     
     file_extension = filename.split(".")[-1].lower()
     abc_fn_suffix = str(abc).zfill(2)
     
     new_filename = output_filename if output_filename else filename.replace("." + file_extension, "_abc" + abc_fn_suffix + "." + file_extension)
     cv2.imwrite(new_filename, img)
     print("Brightness and contrast corrected image saved as", new_filename)
     
-    return img, alpha, beta
+    return img, alpha, beta, new_filename
 
 def main():
     parser = argparse.ArgumentParser(description='Image Brightness and Contrast Correction\nby Guillaume D. Isabelle, 2024\n')
     
     parser.add_argument('filename', type=str, help='input image filename')
     parser.add_argument('abc', type=int, nargs='?', default=15, help='automatic brightness and contrast percentage (default: 25)')
     parser.add_argument('-o','--output', type=str, help='output image filename')
     #argument flag --feh to open the image with feh
     parser.add_argument('--feh', action='store_true', help='open the image with feh')
 
     
     args = parser.parse_args()
     
-    correct(args.filename, args.abc, args.output)
+    filename = args.filename
+    abc_value = args.abc
+    
+    
+    target_output = args.output
+    
+    img, alpha, beta, outfile=correct(filename, abc_value, target_output)
     if args.feh:
         import subprocess
-        subprocess.run(['feh', args.output])
+        subprocess.run(['feh', outfile])
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `astabc-0.1.6/astabc.egg-info/PKG-INFO` & `astabc-0.1.7/astabc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: astabc
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python module for automatic brightness and contrast optimization
 Home-page: https://github.com/jgwill/gia-abc
 Author: Guillaume Descoteaux-Isabelle
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: opencv-python
 
 # astabc
 
 The `astabc` module is a Python module that provides functions for automatic brightness and contrast optimization of images.
 
 ## Installation
```

### Comparing `astabc-0.1.6/setup.py` & `astabc-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="astabc",
-    version="0.1.6",
+    version="0.1.7",
     author="Guillaume Descoteaux-Isabelle",
     description="A Python module for automatic brightness and contrast optimization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jgwill/gia-abc",
     packages=["astabc"],
     entry_points={
```

### Comparing `astabc-0.1.6/tests/test_astabc.py` & `astabc-0.1.7/tests/test_astabc.py`

 * *Files identical despite different names*


# Comparing `tmp/standard_imghdr-3.10.14.tar.gz` & `tmp/standard_imghdr-3.11.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_imghdr-3.10.14.tar", last modified: Sun Apr 21 18:51:28 2024, max compression
+gzip compressed data, was "standard_imghdr-3.11.9.tar", last modified: Sun Apr 21 19:04:49 2024, max compression
```

## Comparing `standard_imghdr-3.10.14.tar` & `standard_imghdr-3.11.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:28.806662 standard_imghdr-3.10.14/
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_imghdr-3.10.14/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     3809 2024-04-21 18:51:28.806418 standard_imghdr-3.10.14/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_imghdr-3.10.14/README.rst
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:28.805117 standard_imghdr-3.10.14/imghdr/
--rw-r--r--   0 user       (501) staff       (20)     3808 2024-04-21 18:45:39.000000 standard_imghdr-3.10.14/imghdr/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      709 2024-04-21 18:45:39.000000 standard_imghdr-3.10.14/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 18:51:28.806712 standard_imghdr-3.10.14/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:28.806145 standard_imghdr-3.10.14/standard_imghdr.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3809 2024-04-21 18:51:28.000000 standard_imghdr-3.10.14/standard_imghdr.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      229 2024-04-21 18:51:28.000000 standard_imghdr-3.10.14/standard_imghdr.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 18:51:28.000000 standard_imghdr-3.10.14/standard_imghdr.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        7 2024-04-21 18:51:28.000000 standard_imghdr-3.10.14/standard_imghdr.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:28.805797 standard_imghdr-3.10.14/tests/
--rw-r--r--   0 user       (501) staff       (20)     4802 2024-04-21 18:45:39.000000 standard_imghdr-3.10.14/tests/test_imghdr.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:49.258440 standard_imghdr-3.11.9/
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_imghdr-3.11.9/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     3808 2024-04-21 19:04:49.258174 standard_imghdr-3.11.9/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_imghdr-3.11.9/README.rst
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:49.256668 standard_imghdr-3.11.9/imghdr/
+-rw-r--r--   0 user       (501) staff       (20)     3952 2024-04-21 19:00:01.000000 standard_imghdr-3.11.9/imghdr/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      708 2024-04-21 19:00:01.000000 standard_imghdr-3.11.9/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 19:04:49.258491 standard_imghdr-3.11.9/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:49.257861 standard_imghdr-3.11.9/standard_imghdr.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3808 2024-04-21 19:04:49.000000 standard_imghdr-3.11.9/standard_imghdr.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      229 2024-04-21 19:04:49.000000 standard_imghdr-3.11.9/standard_imghdr.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 19:04:49.000000 standard_imghdr-3.11.9/standard_imghdr.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        7 2024-04-21 19:04:49.000000 standard_imghdr-3.11.9/standard_imghdr.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:49.257514 standard_imghdr-3.11.9/tests/
+-rw-r--r--   0 user       (501) staff       (20)     4929 2024-04-21 19:00:01.000000 standard_imghdr-3.11.9/tests/test_imghdr.py
```

### Comparing `standard_imghdr-3.10.14/LICENSE` & `standard_imghdr-3.11.9/LICENSE`

 * *Files identical despite different names*

### Comparing `standard_imghdr-3.10.14/PKG-INFO` & `standard_imghdr-3.11.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-imghdr
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library imghdr redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_imghdr-3.10.14/imghdr/__init__.py` & `standard_imghdr-3.11.9/imghdr/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 """Recognize image file formats based on their first few bytes."""
 
 from os import PathLike
+import warnings
 
 __all__ = ["what"]
 
+
+warnings._deprecated(__name__, remove=(3, 13))
+
+
 #-------------------------#
 # Recognize image headers #
 #-------------------------#
 
 def what(file, h=None):
     f = None
     try:
@@ -31,17 +36,19 @@
 #---------------------------------#
 # Subroutines per image file type #
 #---------------------------------#
 
 tests = []
 
 def test_jpeg(h, f):
-    """JPEG data in JFIF or Exif format"""
+    """JPEG data with JFIF or Exif markers; and raw JPEG"""
     if h[6:10] in (b'JFIF', b'Exif'):
         return 'jpeg'
+    elif h[:4] == b'\xff\xd8\xff\xdb':
+        return 'jpeg'
 
 tests.append(test_jpeg)
 
 def test_png(h, f):
     if h.startswith(b'\211PNG\r\n\032\n'):
         return 'png'
```

### Comparing `standard_imghdr-3.10.14/pyproject.toml` & `standard_imghdr-3.11.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "standard-imghdr"
-version = "3.10.14"
+version = "3.11.9"
 description = "Standard library imghdr redistribution. \"dead battery\"."
 keywords = ["stdlib"]
 authors = [
     { name = "Python Devleopers", email = "python-deadlib@youknowone.org" }
 ]
 readme = "README.rst"
 license = {name = "PSF", file = "LICENSE"}
```

### Comparing `standard_imghdr-3.10.14/standard_imghdr.egg-info/PKG-INFO` & `standard_imghdr-3.11.9/standard_imghdr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-imghdr
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library imghdr redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_imghdr-3.10.14/tests/test_imghdr.py` & `standard_imghdr-3.11.9/tests/test_imghdr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-import imghdr
 import io
 import os
 import pathlib
 import unittest
 import warnings
-from test.support import findfile
+from test.support import findfile, warnings_helper
 from test.support.os_helper import TESTFN, unlink
 
+imghdr = warnings_helper.import_deprecated("imghdr")
+
 
 TEST_FILES = (
     ('python.png', 'png'),
     ('python.gif', 'gif'),
     ('python.bmp', 'bmp'),
     ('python.ppm', 'ppm'),
     ('python.pgm', 'pgm'),
     ('python.pbm', 'pbm'),
     ('python.jpg', 'jpeg'),
+    ('python-raw.jpg', 'jpeg'),  # raw JPEG without JFIF/EXIF markers
     ('python.ras', 'rast'),
     ('python.sgi', 'rgb'),
     ('python.tiff', 'tiff'),
     ('python.xbm', 'xbm'),
     ('python.webp', 'webp'),
     ('python.exr', 'exr'),
 )
```


# Comparing `tmp/standard_crypt-3.10.14.tar.gz` & `tmp/standard_crypt-3.11.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_crypt-3.10.14.tar", last modified: Sun Apr 21 18:51:25 2024, max compression
+gzip compressed data, was "standard_crypt-3.11.9.tar", last modified: Sun Apr 21 19:04:45 2024, max compression
```

## Comparing `standard_crypt-3.10.14.tar` & `standard_crypt-3.11.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:25.689853 standard_crypt-3.10.14/
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_crypt-3.10.14/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     3807 2024-04-21 18:51:25.689589 standard_crypt-3.10.14/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_crypt-3.10.14/README.rst
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:25.688478 standard_crypt-3.10.14/crypt/
--rw-r--r--   0 user       (501) staff       (20)     3848 2024-04-21 18:45:39.000000 standard_crypt-3.10.14/crypt/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      706 2024-04-21 18:45:39.000000 standard_crypt-3.10.14/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 18:51:25.689898 standard_crypt-3.10.14/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:25.689332 standard_crypt-3.10.14/standard_crypt.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3807 2024-04-21 18:51:25.000000 standard_crypt-3.10.14/standard_crypt.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      223 2024-04-21 18:51:25.000000 standard_crypt-3.10.14/standard_crypt.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 18:51:25.000000 standard_crypt-3.10.14/standard_crypt.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        6 2024-04-21 18:51:25.000000 standard_crypt-3.10.14/standard_crypt.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:25.689104 standard_crypt-3.10.14/tests/
--rw-r--r--   0 user       (501) staff       (20)     4237 2024-04-21 18:45:39.000000 standard_crypt-3.10.14/tests/test_crypt.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:45.884870 standard_crypt-3.11.9/
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_crypt-3.11.9/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     3806 2024-04-21 19:04:45.884637 standard_crypt-3.11.9/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_crypt-3.11.9/README.rst
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:45.883534 standard_crypt-3.11.9/crypt/
+-rw-r--r--   0 user       (501) staff       (20)     3913 2024-04-21 19:00:01.000000 standard_crypt-3.11.9/crypt/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      705 2024-04-21 19:00:01.000000 standard_crypt-3.11.9/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 19:04:45.884909 standard_crypt-3.11.9/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:45.884446 standard_crypt-3.11.9/standard_crypt.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3806 2024-04-21 19:04:45.000000 standard_crypt-3.11.9/standard_crypt.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      223 2024-04-21 19:04:45.000000 standard_crypt-3.11.9/standard_crypt.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 19:04:45.000000 standard_crypt-3.11.9/standard_crypt.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        6 2024-04-21 19:04:45.000000 standard_crypt-3.11.9/standard_crypt.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:45.884202 standard_crypt-3.11.9/tests/
+-rw-r--r--   0 user       (501) staff       (20)     4292 2024-04-21 19:00:01.000000 standard_crypt-3.11.9/tests/test_crypt.py
```

### Comparing `standard_crypt-3.10.14/LICENSE` & `standard_crypt-3.11.9/LICENSE`

 * *Files identical despite different names*

### Comparing `standard_crypt-3.10.14/PKG-INFO` & `standard_crypt-3.11.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-crypt
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library crypt redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_crypt-3.10.14/crypt/__init__.py` & `standard_crypt-3.11.9/crypt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,22 @@
     if _sys.platform == 'win32':
         raise ImportError("The crypt module is not supported on Windows")
     else:
         raise ImportError("The required _crypt module was not built as part of CPython")
 
 import errno
 import string as _string
+import warnings
 from random import SystemRandom as _SystemRandom
 from collections import namedtuple as _namedtuple
 
 
+warnings._deprecated(__name__, remove=(3, 13))
+
+
 _saltchars = _string.ascii_letters + _string.digits + './'
 _sr = _SystemRandom()
 
 
 class _Method(_namedtuple('_Method', 'name ident salt_chars total_size')):
 
     """Class representing a salt method per the Modular Crypt Format or the
```

### Comparing `standard_crypt-3.10.14/pyproject.toml` & `standard_crypt-3.11.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "standard-crypt"
-version = "3.10.14"
+version = "3.11.9"
 description = "Standard library crypt redistribution. \"dead battery\"."
 keywords = ["stdlib"]
 authors = [
     { name = "Python Devleopers", email = "python-deadlib@youknowone.org" }
 ]
 readme = "README.rst"
 license = {name = "PSF", file = "LICENSE"}
```

### Comparing `standard_crypt-3.10.14/standard_crypt.egg-info/PKG-INFO` & `standard_crypt-3.11.9/standard_crypt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-crypt
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library crypt redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_crypt-3.10.14/tests/test_crypt.py` & `standard_crypt-3.11.9/tests/test_crypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sys
 import unittest
-from test.support import check_sanitizer
+from test.support import check_sanitizer, warnings_helper
 
 
 try:
     if check_sanitizer(address=True, memory=True):
         raise unittest.SkipTest("The crypt module SEGFAULTs on ASAN/MSAN builds")
-    import crypt
+    crypt = warnings_helper.import_deprecated("crypt")
     IMPORT_ERROR = None
 except ImportError as ex:
     if sys.platform != 'win32':
         raise unittest.SkipTest(str(ex))
     crypt = None
     IMPORT_ERROR = str(ex)
```


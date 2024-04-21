# Comparing `tmp/standard_pipes-3.10.14.tar.gz` & `tmp/standard_pipes-3.11.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_pipes-3.10.14.tar", last modified: Sun Apr 21 18:51:56 2024, max compression
+gzip compressed data, was "standard_pipes-3.11.9.tar", last modified: Sun Apr 21 19:05:15 2024, max compression
```

## Comparing `standard_pipes-3.10.14.tar` & `standard_pipes-3.11.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:56.749371 standard_pipes-3.10.14/
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_pipes-3.10.14/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     3807 2024-04-21 18:51:56.749117 standard_pipes-3.10.14/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_pipes-3.10.14/README.rst
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:56.747923 standard_pipes-3.10.14/pipes/
--rw-r--r--   0 user       (501) staff       (20)     8914 2024-04-21 18:45:39.000000 standard_pipes-3.10.14/pipes/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      706 2024-04-21 18:45:39.000000 standard_pipes-3.10.14/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 18:51:56.749414 standard_pipes-3.10.14/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:56.748864 standard_pipes-3.10.14/standard_pipes.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3807 2024-04-21 18:51:56.000000 standard_pipes-3.10.14/standard_pipes.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      223 2024-04-21 18:51:56.000000 standard_pipes-3.10.14/standard_pipes.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 18:51:56.000000 standard_pipes-3.10.14/standard_pipes.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        6 2024-04-21 18:51:56.000000 standard_pipes-3.10.14/standard_pipes.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:56.748633 standard_pipes-3.10.14/tests/
--rw-r--r--   0 user       (501) staff       (20)     6868 2024-04-21 18:45:39.000000 standard_pipes-3.10.14/tests/test_pipes.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:15.227505 standard_pipes-3.11.9/
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_pipes-3.11.9/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     3806 2024-04-21 19:05:15.227302 standard_pipes-3.11.9/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_pipes-3.11.9/README.rst
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:15.226225 standard_pipes-3.11.9/pipes/
+-rw-r--r--   0 user       (501) staff       (20)     8978 2024-04-21 19:00:01.000000 standard_pipes-3.11.9/pipes/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      705 2024-04-21 19:00:01.000000 standard_pipes-3.11.9/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 19:05:15.227544 standard_pipes-3.11.9/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:15.227105 standard_pipes-3.11.9/standard_pipes.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3806 2024-04-21 19:05:15.000000 standard_pipes-3.11.9/standard_pipes.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      223 2024-04-21 19:05:15.000000 standard_pipes-3.11.9/standard_pipes.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 19:05:15.000000 standard_pipes-3.11.9/standard_pipes.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        6 2024-04-21 19:05:15.000000 standard_pipes-3.11.9/standard_pipes.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:15.226878 standard_pipes-3.11.9/tests/
+-rw-r--r--   0 user       (501) staff       (20)     6950 2024-04-21 19:00:01.000000 standard_pipes-3.11.9/tests/test_pipes.py
```

### Comparing `standard_pipes-3.10.14/LICENSE` & `standard_pipes-3.11.9/LICENSE`

 * *Files identical despite different names*

### Comparing `standard_pipes-3.10.14/PKG-INFO` & `standard_pipes-3.11.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-pipes
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library pipes redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_pipes-3.10.14/pipes/__init__.py` & `standard_pipes-3.11.9/pipes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,18 +56,21 @@
    t2 = t.clone()
 """                                     # '
 
 
 import re
 import os
 import tempfile
+import warnings
 # we import the quote function rather than the module for backward compat
 # (quote used to be an undocumented but used function in pipes)
 from shlex import quote
 
+warnings._deprecated(__name__, remove=(3, 13))
+
 __all__ = ["Template"]
 
 # Conversion step kinds
 
 FILEIN_FILEOUT = 'ff'                   # Must read & write real files
 STDIN_FILEOUT  = '-f'                   # Must write a real file
 FILEIN_STDOUT  = 'f-'                   # Must read a real file
```

### Comparing `standard_pipes-3.10.14/pyproject.toml` & `standard_pipes-3.11.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "standard-pipes"
-version = "3.10.14"
+version = "3.11.9"
 description = "Standard library pipes redistribution. \"dead battery\"."
 keywords = ["stdlib"]
 authors = [
     { name = "Python Devleopers", email = "python-deadlib@youknowone.org" }
 ]
 readme = "README.rst"
 license = {name = "PSF", file = "LICENSE"}
```

### Comparing `standard_pipes-3.10.14/standard_pipes.egg-info/PKG-INFO` & `standard_pipes-3.11.9/standard_pipes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-pipes
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library pipes redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_pipes-3.10.14/tests/test_pipes.py` & `standard_pipes-3.11.9/tests/test_pipes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-import pipes
 import os
 import string
 import unittest
 import shutil
 from test.support import reap_children, unix_shell
 from test.support.os_helper import TESTFN, unlink
+from test.support.warnings_helper import import_deprecated
+
+pipes = import_deprecated("pipes")
 
 
 if os.name != 'posix':
     raise unittest.SkipTest('pipes module only works on posix')
 
 if not (unix_shell and os.path.exists(unix_shell)):
     raise unittest.SkipTest('pipes module requires a shell')
```


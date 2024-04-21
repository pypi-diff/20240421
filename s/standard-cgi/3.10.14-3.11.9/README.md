# Comparing `tmp/standard_cgi-3.10.14.tar.gz` & `tmp/standard_cgi-3.11.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_cgi-3.10.14.tar", last modified: Sun Apr 21 18:51:19 2024, max compression
+gzip compressed data, was "standard_cgi-3.11.9.tar", last modified: Sun Apr 21 19:04:38 2024, max compression
```

## Comparing `standard_cgi-3.10.14.tar` & `standard_cgi-3.11.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:19.065427 standard_cgi-3.10.14/
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_cgi-3.10.14/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     3803 2024-04-21 18:51:19.065142 standard_cgi-3.10.14/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_cgi-3.10.14/README.rst
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:19.063452 standard_cgi-3.10.14/cgi/
--rwxr-xr-x   0 user       (501) staff       (20)    34099 2024-04-21 18:45:39.000000 standard_cgi-3.10.14/cgi/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      700 2024-04-21 18:45:39.000000 standard_cgi-3.10.14/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 18:51:19.065480 standard_cgi-3.10.14/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:19.064839 standard_cgi-3.10.14/standard_cgi.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3803 2024-04-21 18:51:19.000000 standard_cgi-3.10.14/standard_cgi.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      211 2024-04-21 18:51:19.000000 standard_cgi-3.10.14/standard_cgi.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 18:51:19.000000 standard_cgi-3.10.14/standard_cgi.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        4 2024-04-21 18:51:19.000000 standard_cgi-3.10.14/standard_cgi.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:19.064133 standard_cgi-3.10.14/tests/
--rw-r--r--   0 user       (501) staff       (20)    22798 2024-04-21 18:45:39.000000 standard_cgi-3.10.14/tests/test_cgi.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:38.862896 standard_cgi-3.11.9/
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_cgi-3.11.9/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     3802 2024-04-21 19:04:38.862673 standard_cgi-3.11.9/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_cgi-3.11.9/README.rst
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:38.861580 standard_cgi-3.11.9/cgi/
+-rwxr-xr-x   0 user       (501) staff       (20)    34420 2024-04-21 19:00:01.000000 standard_cgi-3.11.9/cgi/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      699 2024-04-21 19:00:01.000000 standard_cgi-3.11.9/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 19:04:38.862937 standard_cgi-3.11.9/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:38.862465 standard_cgi-3.11.9/standard_cgi.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3802 2024-04-21 19:04:38.000000 standard_cgi-3.11.9/standard_cgi.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      211 2024-04-21 19:04:38.000000 standard_cgi-3.11.9/standard_cgi.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 19:04:38.000000 standard_cgi-3.11.9/standard_cgi.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        4 2024-04-21 19:04:38.000000 standard_cgi-3.11.9/standard_cgi.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:38.862267 standard_cgi-3.11.9/tests/
+-rw-r--r--   0 user       (501) staff       (20)    22805 2024-04-21 19:00:01.000000 standard_cgi-3.11.9/tests/test_cgi.py
```

### Comparing `standard_cgi-3.10.14/LICENSE` & `standard_cgi-3.11.9/LICENSE`

 * *Files identical despite different names*

### Comparing `standard_cgi-3.10.14/PKG-INFO` & `standard_cgi-3.11.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-cgi
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library cgi redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_cgi-3.10.14/cgi/__init__.py` & `standard_cgi-3.11.9/cgi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 # /usr/bin.  So let those vendors patch cgi.py to match their choice
 # of installation.
 
 """Support module for CGI (Common Gateway Interface) scripts.
 
 This module defines a number of utilities for use by CGI scripts
 written in Python.
+
+The global variable maxlen can be set to an integer indicating the maximum size
+of a POST request. POST requests larger than this size will result in a
+ValueError being raised during parsing. The default value of this variable is 0,
+meaning the request size is unlimited.
 """
 
 # History
 # -------
 #
 # Michael McLay started this module.  Steve Majewski changed the
 # interface to SvFormContentDict and FormContentDict.  The multipart
@@ -44,14 +49,17 @@
 import warnings
 
 __all__ = ["MiniFieldStorage", "FieldStorage", "parse", "parse_multipart",
            "parse_header", "test", "print_exception", "print_environ",
            "print_form", "print_directory", "print_arguments",
            "print_environ_usage"]
 
+
+warnings._deprecated(__name__, remove=(3,13))
+
 # Logging support
 # ===============
 
 logfile = ""            # Filename to log to, if not empty
 logfp = None            # File object to log to, if not None
 
 def initlog(*allargs):
```

### Comparing `standard_cgi-3.10.14/pyproject.toml` & `standard_cgi-3.11.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "standard-cgi"
-version = "3.10.14"
+version = "3.11.9"
 description = "Standard library cgi redistribution. \"dead battery\"."
 keywords = ["stdlib"]
 authors = [
     { name = "Python Devleopers", email = "python-deadlib@youknowone.org" }
 ]
 readme = "README.rst"
 license = {name = "PSF", file = "LICENSE"}
```

### Comparing `standard_cgi-3.10.14/standard_cgi.egg-info/PKG-INFO` & `standard_cgi-3.11.9/standard_cgi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-cgi
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library cgi redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_cgi-3.10.14/tests/test_cgi.py` & `standard_cgi-3.11.9/tests/test_cgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-import cgi
 import os
 import sys
 import tempfile
 import unittest
 from collections import namedtuple
 from io import StringIO, BytesIO
 from test import support
 from test.support import warnings_helper
 
+cgi = warnings_helper.import_deprecated("cgi")
+
+
 class HackedSysModule:
     # The regression test will have real values in sys.argv, which
     # will completely confuse the test of the cgi module
     argv = []
     stdin = sys.stdin
 
 cgi.sys = HackedSysModule()
@@ -47,15 +49,15 @@
         raise ValueError("unknown method: %s" % method)
     try:
         return cgi.parse(fp, env, strict_parsing=1)
     except Exception as err:
         return ComparableException(err)
 
 parse_strict_test_cases = [
-    ("", ValueError("bad query field: ''")),
+    ("", {}),
     ("&", ValueError("bad query field: ''")),
     ("&&", ValueError("bad query field: ''")),
     # Should the next few really be valid?
     ("=", {}),
     ("=&=", {}),
     # This rest seem to make sense
     ("=a", {'': ['a']}),
```


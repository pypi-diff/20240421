# Comparing `tmp/lichesspy-6.0.4.dev2.tar.gz` & `tmp/lichesspy-6.0.4.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lichesspy-6.0.4.dev2.tar", last modified: Sun Apr 21 18:57:01 2024, max compression
+gzip compressed data, was "lichesspy-6.0.4.dev3.tar", last modified: Sun Apr 21 19:11:08 2024, max compression
```

## Comparing `lichesspy-6.0.4.dev2.tar` & `lichesspy-6.0.4.dev3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:57:01.040243 lichesspy-6.0.4.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 18:56:55.000000 lichesspy-6.0.4.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-21 18:57:01.040243 lichesspy-6.0.4.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-21 18:56:55.000000 lichesspy-6.0.4.dev2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:57:01.036242 lichesspy-6.0.4.dev2/lichesspy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:56:55.000000 lichesspy-6.0.4.dev2/lichesspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14310 2024-04-21 18:56:55.000000 lichesspy-6.0.4.dev2/lichesspy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-21 18:56:55.000000 lichesspy-6.0.4.dev2/lichesspy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-21 18:56:55.000000 lichesspy-6.0.4.dev2/lichesspy/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-21 18:56:55.000000 lichesspy-6.0.4.dev2/lichesspy/pgn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:57:01.040243 lichesspy-6.0.4.dev2/lichesspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-21 18:57:01.000000 lichesspy-6.0.4.dev2/lichesspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 18:57:01.000000 lichesspy-6.0.4.dev2/lichesspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 18:57:01.000000 lichesspy-6.0.4.dev2/lichesspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-21 18:57:01.000000 lichesspy-6.0.4.dev2/lichesspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 18:57:01.000000 lichesspy-6.0.4.dev2/lichesspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 18:57:01.040243 lichesspy-6.0.4.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-21 18:56:55.000000 lichesspy-6.0.4.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:11:08.279570 lichesspy-6.0.4.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 19:11:03.000000 lichesspy-6.0.4.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-21 19:11:08.279570 lichesspy-6.0.4.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-21 19:11:03.000000 lichesspy-6.0.4.dev3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:11:08.275570 lichesspy-6.0.4.dev3/lichesspy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:11:03.000000 lichesspy-6.0.4.dev3/lichesspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-04-21 19:11:03.000000 lichesspy-6.0.4.dev3/lichesspy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-21 19:11:03.000000 lichesspy-6.0.4.dev3/lichesspy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-21 19:11:03.000000 lichesspy-6.0.4.dev3/lichesspy/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-21 19:11:03.000000 lichesspy-6.0.4.dev3/lichesspy/pgn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:11:08.279570 lichesspy-6.0.4.dev3/lichesspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-21 19:11:08.000000 lichesspy-6.0.4.dev3/lichesspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 19:11:08.000000 lichesspy-6.0.4.dev3/lichesspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:11:08.000000 lichesspy-6.0.4.dev3/lichesspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-21 19:11:08.000000 lichesspy-6.0.4.dev3/lichesspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 19:11:08.000000 lichesspy-6.0.4.dev3/lichesspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:11:08.279570 lichesspy-6.0.4.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-21 19:11:03.000000 lichesspy-6.0.4.dev3/setup.py
```

### Comparing `lichesspy-6.0.4.dev2/LICENSE` & `lichesspy-6.0.4.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.4.dev2/PKG-INFO` & `lichesspy-6.0.4.dev3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: lichesspy
-Version: 6.0.4.dev2
+Version: 6.0.4.dev3
 Summary: Python wrapper for lichess
 Home-page: https://github.com/eskopp/lichesspy
 Author: eskopp
 Author-email: skopp.erik+lichesspy@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: six==1.16.0
-Requires-Dist: python-chess==1.999
 Requires-Dist: chess==1.10.0
 
 A client for the lichess.org API
 ================================================
 This is a client library for the Lichess API.
 It is designed to be:
```

### Comparing `lichesspy-6.0.4.dev2/README.rst` & `lichesspy-6.0.4.dev3/README.rst`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.4.dev2/lichesspy/api.py` & `lichesspy-6.0.4.dev3/lichesspy/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import requests
 import time
 from six.moves import urllib
-import lichess.format
-import lichess.auth
+import lichesspy.format as lichess
+import lichesspy.auth as lichess
 
 
 class ApiError(Exception):
     """The base class for API exceptions."""
 
 
 class ApiHttpError(ApiError):
```

### Comparing `lichesspy-6.0.4.dev2/lichesspy/format.py` & `lichesspy-6.0.4.dev3/lichesspy/format.py`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.4.dev2/lichesspy/pgn.py` & `lichesspy-6.0.4.dev3/lichesspy/pgn.py`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.4.dev2/lichesspy.egg-info/PKG-INFO` & `lichesspy-6.0.4.dev3/lichesspy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: lichesspy
-Version: 6.0.4.dev2
+Version: 6.0.4.dev3
 Summary: Python wrapper for lichess
 Home-page: https://github.com/eskopp/lichesspy
 Author: eskopp
 Author-email: skopp.erik+lichesspy@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: six==1.16.0
-Requires-Dist: python-chess==1.999
 Requires-Dist: chess==1.10.0
 
 A client for the lichess.org API
 ================================================
 This is a client library for the Lichess API.
 It is designed to be:
```

### Comparing `lichesspy-6.0.4.dev2/setup.py` & `lichesspy-6.0.4.dev3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     if readme_path.exists():
         return readme_path.read_text(encoding="utf-8")
     return "Long description could not be read from README.rst"
 
 
 setuptools.setup(
     name="lichesspy",
-    version="6.0.4.dev2",
+    version="6.0.4.dev3",
     author="eskopp",
     author_email="skopp.erik+lichesspy@gmail.com",
     description="Python wrapper for lichess",
     long_description=load_readme(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/eskopp/lichesspy",
```


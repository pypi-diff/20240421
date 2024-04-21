# Comparing `tmp/lichesspy-6.0.2.tar.gz` & `tmp/lichesspy-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lichesspy-6.0.2.tar", last modified: Sun Apr 21 03:44:24 2024, max compression
+gzip compressed data, was "lichesspy-6.0.3.tar", last modified: Sun Apr 21 03:52:06 2024, max compression
```

## Comparing `lichesspy-6.0.2.tar` & `lichesspy-6.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:44:24.001411 lichesspy-6.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 03:44:18.000000 lichesspy-6.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-21 03:44:23.997411 lichesspy-6.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-21 03:44:18.000000 lichesspy-6.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:44:23.997411 lichesspy-6.0.2/lichesspy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:44:18.000000 lichesspy-6.0.2/lichesspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14355 2024-04-21 03:44:18.000000 lichesspy-6.0.2/lichesspy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-21 03:44:18.000000 lichesspy-6.0.2/lichesspy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-21 03:44:18.000000 lichesspy-6.0.2/lichesspy/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-21 03:44:18.000000 lichesspy-6.0.2/lichesspy/pgn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:44:23.997411 lichesspy-6.0.2/lichesspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-21 03:44:23.000000 lichesspy-6.0.2/lichesspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 03:44:23.000000 lichesspy-6.0.2/lichesspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 03:44:23.000000 lichesspy-6.0.2/lichesspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-21 03:44:23.000000 lichesspy-6.0.2/lichesspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 03:44:23.000000 lichesspy-6.0.2/lichesspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 03:44:24.001411 lichesspy-6.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-21 03:44:18.000000 lichesspy-6.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:52:06.571783 lichesspy-6.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 03:52:01.000000 lichesspy-6.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-21 03:52:06.571783 lichesspy-6.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-21 03:52:01.000000 lichesspy-6.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:52:06.571783 lichesspy-6.0.3/lichesspy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:52:01.000000 lichesspy-6.0.3/lichesspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14355 2024-04-21 03:52:01.000000 lichesspy-6.0.3/lichesspy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-21 03:52:01.000000 lichesspy-6.0.3/lichesspy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-21 03:52:01.000000 lichesspy-6.0.3/lichesspy/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-21 03:52:01.000000 lichesspy-6.0.3/lichesspy/pgn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:52:06.571783 lichesspy-6.0.3/lichesspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-21 03:52:06.000000 lichesspy-6.0.3/lichesspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 03:52:06.000000 lichesspy-6.0.3/lichesspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 03:52:06.000000 lichesspy-6.0.3/lichesspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-21 03:52:06.000000 lichesspy-6.0.3/lichesspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 03:52:06.000000 lichesspy-6.0.3/lichesspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 03:52:06.571783 lichesspy-6.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-21 03:52:01.000000 lichesspy-6.0.3/setup.py
```

### Comparing `lichesspy-6.0.2/LICENSE` & `lichesspy-6.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.2/PKG-INFO` & `lichesspy-6.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: lichesspy
-Version: 6.0.2
+Version: 6.0.3
 Summary: Python wrapper for lichess
 Home-page: https://github.com/eskopp/lichesspy
 Author: eskopp
 Author-email: skopp.erik@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests==2.31.0
-Requires-Dist: six==1.16.0
-Requires-Dist: python-chess==1.999
-Requires-Dist: chess==1.10.0
+Requires-Dist: requests>=2.31.0
+Requires-Dist: six>=1.16.0
+Requires-Dist: python-chess>=1.999
+Requires-Dist: chess>=1.10.0
 
 A client for the lichess.org API
 ================================================
 This is a client library for the Lichess API.
 It is designed to be:
 
 * Easy to use
```

### Comparing `lichesspy-6.0.2/README.rst` & `lichesspy-6.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.2/lichesspy/api.py` & `lichesspy-6.0.3/lichesspy/api.py`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.2/lichesspy/format.py` & `lichesspy-6.0.3/lichesspy/format.py`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.2/lichesspy/pgn.py` & `lichesspy-6.0.3/lichesspy/pgn.py`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.2/lichesspy.egg-info/PKG-INFO` & `lichesspy-6.0.3/lichesspy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: lichesspy
-Version: 6.0.2
+Version: 6.0.3
 Summary: Python wrapper for lichess
 Home-page: https://github.com/eskopp/lichesspy
 Author: eskopp
 Author-email: skopp.erik@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests==2.31.0
-Requires-Dist: six==1.16.0
-Requires-Dist: python-chess==1.999
-Requires-Dist: chess==1.10.0
+Requires-Dist: requests>=2.31.0
+Requires-Dist: six>=1.16.0
+Requires-Dist: python-chess>=1.999
+Requires-Dist: chess>=1.10.0
 
 A client for the lichess.org API
 ================================================
 This is a client library for the Lichess API.
 It is designed to be:
 
 * Easy to use
```


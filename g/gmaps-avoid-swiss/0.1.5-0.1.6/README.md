# Comparing `tmp/gmaps_avoid_swiss-0.1.5.tar.gz` & `tmp/gmaps_avoid_swiss-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmaps_avoid_swiss-0.1.5.tar", last modified: Sun Apr 21 03:28:16 2024, max compression
+gzip compressed data, was "gmaps_avoid_swiss-0.1.6.tar", last modified: Sun Apr 21 03:33:08 2024, max compression
```

## Comparing `gmaps_avoid_swiss-0.1.5.tar` & `gmaps_avoid_swiss-0.1.6.tar`

### file list

```diff
@@ -1,44 +1,50 @@
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:28:16.026257 gmaps_avoid_swiss-0.1.5/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      162 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/AUTHORS.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     3851 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/CONTRIBUTING.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       89 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/HISTORY.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1072 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/LICENSE
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      262 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/MANIFEST.in
--rw-r--r--   0 gregor    (1000) gregor    (1000)     2876 2024-04-21 03:28:16.026257 gmaps_avoid_swiss-0.1.5/PKG-INFO
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1845 2024-04-21 03:27:56.000000 gmaps_avoid_swiss-0.1.5/README.rst
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:28:16.026257 gmaps_avoid_swiss-0.1.5/docs/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      618 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/docs/Makefile
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/docs/authors.rst
--rwxrwxr-x   0 gregor    (1000) gregor    (1000)     4934 2024-04-21 02:19:23.000000 gmaps_avoid_swiss-0.1.5/docs/conf.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       33 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/docs/contributing.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1152 2024-04-20 18:21:23.000000 gmaps_avoid_swiss-0.1.5/docs/geos.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      881 2024-04-21 02:16:02.000000 gmaps_avoid_swiss-0.1.5/docs/gmaps_avoid_swiss.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/docs/history.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      343 2024-04-21 02:19:08.000000 gmaps_avoid_swiss-0.1.5/docs/index.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1211 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/docs/installation.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      815 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/docs/make.bat
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       88 2024-04-21 02:16:02.000000 gmaps_avoid_swiss-0.1.5/docs/modules.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       27 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/docs/readme.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1237 2024-04-21 02:18:54.000000 gmaps_avoid_swiss-0.1.5/docs/usage.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1408 2024-04-21 03:20:40.000000 gmaps_avoid_swiss-0.1.5/pyproject.toml
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       38 2024-04-21 03:28:16.026257 gmaps_avoid_swiss-0.1.5/setup.cfg
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1023 2024-04-21 03:20:40.000000 gmaps_avoid_swiss-0.1.5/setup.py
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:28:16.022257 gmaps_avoid_swiss-0.1.5/src/
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:28:16.026257 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      307 2024-04-21 03:20:40.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss/__init__.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      674 2024-04-20 16:51:38.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss/client.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     4030 2024-04-21 02:11:49.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss/geo_check.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     7470 2024-04-21 02:11:04.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss/routes.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     2540 2024-04-20 16:57:41.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss/waypoints.py
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:28:16.026257 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss.egg-info/
--rw-r--r--   0 gregor    (1000) gregor    (1000)     2876 2024-04-21 03:28:16.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss.egg-info/PKG-INFO
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      829 2024-04-21 03:28:16.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss.egg-info/SOURCES.txt
--rw-rw-r--   0 gregor    (1000) gregor    (1000)        1 2024-04-21 03:28:16.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss.egg-info/dependency_links.txt
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       76 2024-04-21 03:28:16.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss.egg-info/requires.txt
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       18 2024-04-21 03:28:16.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss.egg-info/top_level.txt
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:28:16.026257 gmaps_avoid_swiss-0.1.5/tests/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       47 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/tests/__init__.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1383 2024-04-21 03:10:41.000000 gmaps_avoid_swiss-0.1.5/tests/test_geo_check.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1460 2024-04-21 03:00:26.000000 gmaps_avoid_swiss-0.1.5/tests/test_gmaps_avoid_swiss.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1550 2024-04-21 03:19:07.000000 gmaps_avoid_swiss-0.1.5/tests/test_routes.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1202 2024-04-19 19:57:47.000000 gmaps_avoid_swiss-0.1.5/tests/test_waypoints.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:33:08.165749 gmaps_avoid_swiss-0.1.6/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      162 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.6/AUTHORS.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     3851 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.6/CONTRIBUTING.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       89 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.6/HISTORY.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1072 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.6/LICENSE
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      262 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.6/MANIFEST.in
+-rw-r--r--   0 gregor    (1000) gregor    (1000)     2896 2024-04-21 03:33:08.165749 gmaps_avoid_swiss-0.1.6/PKG-INFO
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1865 2024-04-21 03:33:06.000000 gmaps_avoid_swiss-0.1.6/README.rst
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:33:08.161749 gmaps_avoid_swiss-0.1.6/docs/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      618 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.6/docs/Makefile
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:33:08.161749 gmaps_avoid_swiss-0.1.6/docs/_build/
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:33:08.161749 gmaps_avoid_swiss-0.1.6/docs/_build/html/
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:33:08.161749 gmaps_avoid_swiss-0.1.6/docs/_build/html/_static/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      286 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.6/docs/_build/html/_static/file.png
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       90 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.6/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       90 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.6/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.6/docs/authors.rst
+-rwxrwxr-x   0 gregor    (1000) gregor    (1000)     4934 2024-04-21 02:19:23.000000 gmaps_avoid_swiss-0.1.6/docs/conf.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       33 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.6/docs/contributing.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1152 2024-04-20 18:21:23.000000 gmaps_avoid_swiss-0.1.6/docs/geos.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      881 2024-04-21 03:31:07.000000 gmaps_avoid_swiss-0.1.6/docs/gmaps_avoid_swiss.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.6/docs/history.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      343 2024-04-21 02:19:08.000000 gmaps_avoid_swiss-0.1.6/docs/index.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1211 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.6/docs/installation.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      815 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.6/docs/make.bat
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       88 2024-04-21 03:31:07.000000 gmaps_avoid_swiss-0.1.6/docs/modules.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       27 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.6/docs/readme.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1237 2024-04-21 02:18:54.000000 gmaps_avoid_swiss-0.1.6/docs/usage.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1408 2024-04-21 03:32:28.000000 gmaps_avoid_swiss-0.1.6/pyproject.toml
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       38 2024-04-21 03:33:08.165749 gmaps_avoid_swiss-0.1.6/setup.cfg
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1023 2024-04-21 03:32:28.000000 gmaps_avoid_swiss-0.1.6/setup.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:33:08.161749 gmaps_avoid_swiss-0.1.6/src/
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:33:08.161749 gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      307 2024-04-21 03:32:28.000000 gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss/__init__.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      674 2024-04-20 16:51:38.000000 gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss/client.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     4030 2024-04-21 02:11:49.000000 gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss/geo_check.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     7470 2024-04-21 02:11:04.000000 gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss/routes.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     2540 2024-04-20 16:57:41.000000 gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss/waypoints.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:33:08.161749 gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss.egg-info/
+-rw-r--r--   0 gregor    (1000) gregor    (1000)     2896 2024-04-21 03:33:08.000000 gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss.egg-info/PKG-INFO
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      932 2024-04-21 03:33:08.000000 gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss.egg-info/SOURCES.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)        1 2024-04-21 03:33:08.000000 gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss.egg-info/dependency_links.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       76 2024-04-21 03:33:08.000000 gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss.egg-info/requires.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       18 2024-04-21 03:33:08.000000 gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss.egg-info/top_level.txt
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:33:08.161749 gmaps_avoid_swiss-0.1.6/tests/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       47 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.6/tests/__init__.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1383 2024-04-21 03:10:41.000000 gmaps_avoid_swiss-0.1.6/tests/test_geo_check.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1460 2024-04-21 03:00:26.000000 gmaps_avoid_swiss-0.1.6/tests/test_gmaps_avoid_swiss.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1550 2024-04-21 03:19:07.000000 gmaps_avoid_swiss-0.1.6/tests/test_routes.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1202 2024-04-19 19:57:47.000000 gmaps_avoid_swiss-0.1.6/tests/test_waypoints.py
```

### Comparing `gmaps_avoid_swiss-0.1.5/CONTRIBUTING.rst` & `gmaps_avoid_swiss-0.1.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.5/LICENSE` & `gmaps_avoid_swiss-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.5/PKG-INFO` & `gmaps_avoid_swiss-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmaps_avoid_swiss
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python package that customizes Google Maps routing to avoid Swiss routes unless the origin, destination, or waypoints include locations within Switzerland.
 Home-page: https://github.com/xbencat/gmaps_avoid_swiss
 Author: Gregor Bencat
 Author-email: Gregor Bencat <bencat.gregor@gmail.com>
 Maintainer-email: Gregor Bencat <bencat.gregor@gmail.com>
 License: MIT license
 Project-URL: bugs, https://github.com/xbencat/gmaps_avoid_swiss/issues
@@ -45,15 +45,15 @@
 * Documentation: https://gmaps-avoid-swiss.readthedocs.io.
 
 
 Dependencies
 ____________
 
 This package requires the GEOS library as it utilizes Shapely for geographic operations.
-For installation instructions and more details, please refer to our GEOS for more details.
+For installation instructions and more details, please refer to our `Geos <geos.html>`_ page for more details.
 
 
 Features
 --------
 
 * Calculates duration, transit time, and encoded path from origin to destination
 * Avoids routing through Switzerland by dynamically selecting alternative cities
```

### Comparing `gmaps_avoid_swiss-0.1.5/README.rst` & `gmaps_avoid_swiss-0.1.6/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 * Documentation: https://gmaps-avoid-swiss.readthedocs.io.
 
 
 Dependencies
 ____________
 
 This package requires the GEOS library as it utilizes Shapely for geographic operations.
-For installation instructions and more details, please refer to our GEOS for more details.
+For installation instructions and more details, please refer to our `Geos <geos.html>`_ page for more details.
 
 
 Features
 --------
 
 * Calculates duration, transit time, and encoded path from origin to destination
 * Avoids routing through Switzerland by dynamically selecting alternative cities
```

### Comparing `gmaps_avoid_swiss-0.1.5/docs/Makefile` & `gmaps_avoid_swiss-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.5/docs/conf.py` & `gmaps_avoid_swiss-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.5/docs/geos.rst` & `gmaps_avoid_swiss-0.1.6/docs/geos.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.5/docs/gmaps_avoid_swiss.rst` & `gmaps_avoid_swiss-0.1.6/docs/gmaps_avoid_swiss.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.5/docs/installation.rst` & `gmaps_avoid_swiss-0.1.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.5/docs/make.bat` & `gmaps_avoid_swiss-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.5/docs/usage.rst` & `gmaps_avoid_swiss-0.1.6/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.5/pyproject.toml` & `gmaps_avoid_swiss-0.1.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gmaps_avoid_swiss"
-version = "0.1.5"
+version = "0.1.6"
 description = "A Python package that customizes Google Maps routing to avoid Swiss routes unless the origin, destination, or waypoints include locations within Switzerland."
 readme = "README.rst"
 authors = [
   {name = "Gregor Bencat", email = "bencat.gregor@gmail.com"}
 ]
 maintainers = [
   {name = "Gregor Bencat", email = "bencat.gregor@gmail.com"}
```

### Comparing `gmaps_avoid_swiss-0.1.5/setup.py` & `gmaps_avoid_swiss-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gmaps_avoid_swiss',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     url='https://github.com/xbencat/gmaps_avoid_swiss',
     license='MIT',
     author='Gregor Bencat',
     author_email='bencat.gregor@gmail.com',
     description='A Python package that customizes Google Maps routing to avoid Swiss routes.',
```

### Comparing `gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss/client.py` & `gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss/client.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss/geo_check.py` & `gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss/geo_check.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss/routes.py` & `gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss/routes.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss/waypoints.py` & `gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss/waypoints.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss.egg-info/PKG-INFO` & `gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmaps-avoid-swiss
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python package that customizes Google Maps routing to avoid Swiss routes unless the origin, destination, or waypoints include locations within Switzerland.
 Home-page: https://github.com/xbencat/gmaps_avoid_swiss
 Author: Gregor Bencat
 Author-email: Gregor Bencat <bencat.gregor@gmail.com>
 Maintainer-email: Gregor Bencat <bencat.gregor@gmail.com>
 License: MIT license
 Project-URL: bugs, https://github.com/xbencat/gmaps_avoid_swiss/issues
@@ -45,15 +45,15 @@
 * Documentation: https://gmaps-avoid-swiss.readthedocs.io.
 
 
 Dependencies
 ____________
 
 This package requires the GEOS library as it utilizes Shapely for geographic operations.
-For installation instructions and more details, please refer to our GEOS for more details.
+For installation instructions and more details, please refer to our `Geos <geos.html>`_ page for more details.
 
 
 Features
 --------
 
 * Calculates duration, transit time, and encoded path from origin to destination
 * Avoids routing through Switzerland by dynamically selecting alternative cities
```

### Comparing `gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss.egg-info/SOURCES.txt` & `gmaps_avoid_swiss-0.1.6/src/gmaps_avoid_swiss.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/modules.rst
 docs/readme.rst
 docs/usage.rst
+docs/_build/html/_static/file.png
+docs/_build/html/_static/minus.png
+docs/_build/html/_static/plus.png
 src/gmaps_avoid_swiss/__init__.py
 src/gmaps_avoid_swiss/client.py
 src/gmaps_avoid_swiss/geo_check.py
 src/gmaps_avoid_swiss/routes.py
 src/gmaps_avoid_swiss/waypoints.py
 src/gmaps_avoid_swiss.egg-info/PKG-INFO
 src/gmaps_avoid_swiss.egg-info/SOURCES.txt
```

### Comparing `gmaps_avoid_swiss-0.1.5/tests/test_geo_check.py` & `gmaps_avoid_swiss-0.1.6/tests/test_geo_check.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.5/tests/test_gmaps_avoid_swiss.py` & `gmaps_avoid_swiss-0.1.6/tests/test_gmaps_avoid_swiss.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.5/tests/test_routes.py` & `gmaps_avoid_swiss-0.1.6/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.5/tests/test_waypoints.py` & `gmaps_avoid_swiss-0.1.6/tests/test_waypoints.py`

 * *Files identical despite different names*


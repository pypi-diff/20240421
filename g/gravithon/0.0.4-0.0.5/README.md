# Comparing `tmp/gravithon-0.0.4.tar.gz` & `tmp/gravithon-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravithon-0.0.4.tar", last modified: Sat Mar 30 19:51:47 2024, max compression
+gzip compressed data, was "gravithon-0.0.5.tar", last modified: Sun Apr 21 15:27:42 2024, max compression
```

## Comparing `gravithon-0.0.4.tar` & `gravithon-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,37 @@
-drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-03-30 19:51:47.863596 gravithon-0.0.4/
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)     1071 2024-03-22 09:00:56.000000 gravithon-0.0.4/LICENSE
--rw-r--r--   0 yehuda    (1000) yehuda    (1000)      847 2024-03-30 19:51:47.863596 gravithon-0.0.4/PKG-INFO
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      256 2024-03-29 00:17:55.000000 gravithon-0.0.4/README.md
-drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-03-30 19:51:47.859596 gravithon-0.0.4/gravithon/
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)     1005 2024-03-30 19:13:38.000000 gravithon-0.0.4/gravithon/Body.py
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)     2118 2024-03-30 19:48:41.000000 gravithon-0.0.4/gravithon/Space.py
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      387 2024-03-30 19:15:02.000000 gravithon-0.0.4/gravithon/Sphere.py
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)       52 2024-03-30 19:24:41.000000 gravithon-0.0.4/gravithon/__init__.py
-drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-03-30 19:51:47.859596 gravithon-0.0.4/gravithon/constants/
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)        0 2024-03-30 19:32:15.000000 gravithon-0.0.4/gravithon/constants/__init__.py
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)       67 2024-03-29 10:44:41.000000 gravithon-0.0.4/gravithon/constants/astrophisics.py
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      447 2024-03-30 19:21:09.000000 gravithon-0.0.4/gravithon/errors.py
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      555 2024-03-30 19:26:31.000000 gravithon-0.0.4/gravithon/formulas.py
-drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-03-30 19:51:47.863596 gravithon-0.0.4/gravithon/units/
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      366 2024-03-30 19:51:02.000000 gravithon-0.0.4/gravithon/units/length.py
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      240 2024-03-30 19:51:12.000000 gravithon-0.0.4/gravithon/units/mass.py
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      393 2024-03-29 09:54:52.000000 gravithon-0.0.4/gravithon/units/prefixes.py
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      231 2024-03-30 19:51:12.000000 gravithon-0.0.4/gravithon/units/time.py
-drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-03-30 19:51:47.863596 gravithon-0.0.4/gravithon.egg-info/
--rw-r--r--   0 yehuda    (1000) yehuda    (1000)      847 2024-03-30 19:51:47.000000 gravithon-0.0.4/gravithon.egg-info/PKG-INFO
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      501 2024-03-30 19:51:47.000000 gravithon-0.0.4/gravithon.egg-info/SOURCES.txt
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)        1 2024-03-30 19:51:47.000000 gravithon-0.0.4/gravithon.egg-info/dependency_links.txt
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)       23 2024-03-30 19:51:47.000000 gravithon-0.0.4/gravithon.egg-info/requires.txt
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)       10 2024-03-30 19:51:47.000000 gravithon-0.0.4/gravithon.egg-info/top_level.txt
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      804 2024-03-30 19:51:43.000000 gravithon-0.0.4/pyproject.toml
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)       38 2024-03-30 19:51:47.863596 gravithon-0.0.4/setup.cfg
-drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-03-30 19:51:47.863596 gravithon-0.0.4/tests/
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      131 2024-03-29 13:24:59.000000 gravithon-0.0.4/tests/test.py
+drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-04-21 15:27:42.561766 gravithon-0.0.5/
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)     1071 2024-03-22 09:00:56.000000 gravithon-0.0.5/LICENSE
+-rw-r--r--   0 yehuda    (1000) yehuda    (1000)      870 2024-04-21 15:27:42.561766 gravithon-0.0.5/PKG-INFO
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      256 2024-04-01 11:51:18.000000 gravithon-0.0.5/README.md
+drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-04-21 15:27:42.557765 gravithon-0.0.5/gravithon/
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)     3430 2024-04-21 10:42:44.000000 gravithon-0.0.5/gravithon/Body.py
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)     3605 2024-04-21 15:20:57.000000 gravithon-0.0.5/gravithon/Screen.py
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)     5129 2024-04-21 15:19:27.000000 gravithon-0.0.5/gravithon/Space.py
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      500 2024-04-21 15:24:09.000000 gravithon-0.0.5/gravithon/Sphere.py
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      113 2024-04-05 10:23:02.000000 gravithon-0.0.5/gravithon/__init__.py
+drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-04-21 15:27:42.557765 gravithon-0.0.5/gravithon/astronomy/
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      806 2024-04-20 20:50:33.000000 gravithon-0.0.5/gravithon/astronomy/Planet.py
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)     3270 2024-04-21 10:04:39.000000 gravithon-0.0.5/gravithon/astronomy/Planets.py
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      810 2024-04-05 10:57:23.000000 gravithon-0.0.5/gravithon/astronomy/Satellite.py
+drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-04-21 15:27:42.557765 gravithon-0.0.5/gravithon/constants/
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)        0 2024-03-30 19:32:15.000000 gravithon-0.0.5/gravithon/constants/__init__.py
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      296 2024-04-21 10:04:57.000000 gravithon-0.0.5/gravithon/constants/astrophisics.py
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)     1953 2024-04-21 07:48:47.000000 gravithon-0.0.5/gravithon/errors.py
+drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-04-21 15:27:42.557765 gravithon-0.0.5/gravithon/fields/
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      290 2024-04-21 15:23:00.000000 gravithon-0.0.5/gravithon/fields/Field.py
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      283 2024-04-21 15:24:51.000000 gravithon-0.0.5/gravithon/fields/GravitationalField.py
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)     1635 2024-04-21 10:27:45.000000 gravithon-0.0.5/gravithon/formulas.py
+drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-04-21 15:27:42.557765 gravithon-0.0.5/gravithon/units/
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      366 2024-03-30 19:51:02.000000 gravithon-0.0.5/gravithon/units/length.py
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      241 2024-04-01 11:51:18.000000 gravithon-0.0.5/gravithon/units/mass.py
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      417 2024-03-31 06:04:47.000000 gravithon-0.0.5/gravithon/units/prefixes.py
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      355 2024-04-05 09:18:57.000000 gravithon-0.0.5/gravithon/units/time.py
+drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-04-21 15:27:42.561766 gravithon-0.0.5/gravithon.egg-info/
+-rw-r--r--   0 yehuda    (1000) yehuda    (1000)      870 2024-04-21 15:27:42.000000 gravithon-0.0.5/gravithon.egg-info/PKG-INFO
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      680 2024-04-21 15:27:42.000000 gravithon-0.0.5/gravithon.egg-info/SOURCES.txt
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)        1 2024-04-21 15:27:42.000000 gravithon-0.0.5/gravithon.egg-info/dependency_links.txt
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)       31 2024-04-21 15:27:42.000000 gravithon-0.0.5/gravithon.egg-info/requires.txt
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)       10 2024-04-21 15:27:42.000000 gravithon-0.0.5/gravithon.egg-info/top_level.txt
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      819 2024-04-21 15:27:32.000000 gravithon-0.0.5/pyproject.toml
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)       38 2024-04-21 15:27:42.561766 gravithon-0.0.5/setup.cfg
+drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-04-21 15:27:42.557765 gravithon-0.0.5/tests/
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      131 2024-03-29 13:24:59.000000 gravithon-0.0.5/tests/test.py
```

### Comparing `gravithon-0.0.4/LICENSE` & `gravithon-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gravithon-0.0.4/PKG-INFO` & `gravithon-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: gravithon
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create multy-dimensional python spaces
 Author-email: Yehuda Elyasaf <30yehuda26@gmail.com>
 Maintainer-email: Yehuda Elyasaf <30yehuda26@gmail.com>
 Project-URL: Homepage, https://github.com/YehudaElyasaf/gravithon
 Project-URL: Issues, https://github.com/YehudaElyasaf/gravithon/issues
 Keywords: physics,2d,3d,engine
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: multipledispatch
+Requires-Dist: tkinter
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-C06524)](https://github.com/YehudaElyasaf/gravithon/blob/master/LICENSE)
 [![PyPI - Version](https://img.shields.io/pypi/v/gravithon.svg)](https://pypi.org/project/gravithon/)
 
 <!--
 TODO: readme
 -->
```

### Comparing `gravithon-0.0.4/gravithon.egg-info/PKG-INFO` & `gravithon-0.0.5/gravithon.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: gravithon
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create multy-dimensional python spaces
 Author-email: Yehuda Elyasaf <30yehuda26@gmail.com>
 Maintainer-email: Yehuda Elyasaf <30yehuda26@gmail.com>
 Project-URL: Homepage, https://github.com/YehudaElyasaf/gravithon
 Project-URL: Issues, https://github.com/YehudaElyasaf/gravithon/issues
 Keywords: physics,2d,3d,engine
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: multipledispatch
+Requires-Dist: tkinter
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-C06524)](https://github.com/YehudaElyasaf/gravithon/blob/master/LICENSE)
 [![PyPI - Version](https://img.shields.io/pypi/v/gravithon.svg)](https://pypi.org/project/gravithon/)
 
 <!--
 TODO: readme
 -->
```

### Comparing `gravithon-0.0.4/pyproject.toml` & `gravithon-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 [tool.setuptools]
 package-data = {"sample" = ["*.dat"]}
 
 
 [project]
 name = 'gravithon'
 keywords = ['physics', '2d', '3d', 'engine'] #TODO
-version = '0.0.4'
+version = '0.0.5'
 description = 'Create multy-dimensional python spaces' #TODO
 readme = 'README.md'
 
 dependencies = [
     'numpy',
-    'multipledispatch'
+    'multipledispatch',
+    'tkinter'
 ]
 
 authors = [
   { name='Yehuda Elyasaf', email='30yehuda26@gmail.com' },
 ]
 maintainers = [
   { name='Yehuda Elyasaf', email='30yehuda26@gmail.com' },
```


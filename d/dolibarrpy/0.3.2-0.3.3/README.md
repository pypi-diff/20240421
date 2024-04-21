# Comparing `tmp/dolibarrpy-0.3.2.tar.gz` & `tmp/dolibarrpy-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolibarrpy-0.3.2.tar", last modified: Sun Apr 21 08:55:37 2024, max compression
+gzip compressed data, was "dolibarrpy-0.3.3.tar", last modified: Sun Apr 21 10:18:35 2024, max compression
```

## Comparing `dolibarrpy-0.3.2.tar` & `dolibarrpy-0.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-21 08:55:37.581931 dolibarrpy-0.3.2/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.3.2/LICENSE.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-21 08:55:37.582094 dolibarrpy-0.3.2/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.3.2/README.md
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-21 08:55:37.579890 dolibarrpy-0.3.2/dolibarrpy/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)    31093 2024-04-21 08:53:57.000000 dolibarrpy-0.3.2/dolibarrpy/Dolibarrpy.py
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.3.2/dolibarrpy/__init__.py
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-21 08:55:37.581652 dolibarrpy-0.3.2/dolibarrpy.egg-info/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-21 08:55:37.000000 dolibarrpy-0.3.2/dolibarrpy.egg-info/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-21 08:55:37.000000 dolibarrpy-0.3.2/dolibarrpy.egg-info/SOURCES.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-21 08:55:37.000000 dolibarrpy-0.3.2/dolibarrpy.egg-info/dependency_links.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-21 08:55:37.000000 dolibarrpy-0.3.2/dolibarrpy.egg-info/top_level.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-21 08:55:37.582573 dolibarrpy-0.3.2/setup.cfg
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-21 08:55:27.000000 dolibarrpy-0.3.2/setup.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-21 10:18:35.910857 dolibarrpy-0.3.3/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.3.3/LICENSE.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-21 10:18:35.911013 dolibarrpy-0.3.3/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.3.3/README.md
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-21 10:18:35.908926 dolibarrpy-0.3.3/dolibarrpy/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)    36977 2024-04-21 10:12:40.000000 dolibarrpy-0.3.3/dolibarrpy/Dolibarrpy.py
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.3.3/dolibarrpy/__init__.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-21 10:18:35.910588 dolibarrpy-0.3.3/dolibarrpy.egg-info/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-21 10:18:35.000000 dolibarrpy-0.3.3/dolibarrpy.egg-info/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-21 10:18:35.000000 dolibarrpy-0.3.3/dolibarrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-21 10:18:35.000000 dolibarrpy-0.3.3/dolibarrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-21 10:18:35.000000 dolibarrpy-0.3.3/dolibarrpy.egg-info/top_level.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-21 10:18:35.911468 dolibarrpy-0.3.3/setup.cfg
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-21 10:18:29.000000 dolibarrpy-0.3.3/setup.py
```

### Comparing `dolibarrpy-0.3.2/LICENSE.txt` & `dolibarrpy-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolibarrpy-0.3.2/PKG-INFO` & `dolibarrpy-0.3.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.3.2/dolibarrpy.egg-info/PKG-INFO` & `dolibarrpy-0.3.3/dolibarrpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.3.2/setup.py` & `dolibarrpy-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import os
 
 setup(
     name='dolibarrpy',
     packages=['dolibarrpy'],
-    version="0.3.2",
+    version="0.3.3",
     license='MIT',
     description='Python wrapper for Dolibarr API',
     long_description='Python wrapper for Dolibarr',
     long_description_content_type='text/markdown',
     author='Jon Bendtsen',
     author_email='jon.bendtsen.github@jonb.dk',
     url='https://github.com/JonBendtsen/dolibarrpy.git',
```


# Comparing `tmp/python_optimization-0.0.1.tar.gz` & `tmp/python_optimization-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_optimization-0.0.1.tar", last modified: Sun Apr 21 15:18:32 2024, max compression
+gzip compressed data, was "python_optimization-0.0.2.tar", last modified: Sun Apr 21 15:49:59 2024, max compression
```

## Comparing `python_optimization-0.0.1.tar` & `python_optimization-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 15:18:32.771651 python_optimization-0.0.1/
--rw-rw-rw-   0        0        0      557 2024-04-21 15:18:32.771651 python_optimization-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-21 15:18:32.739643 python_optimization-0.0.1/python_optimization/
--rw-rw-rw-   0        0        0       26 2024-04-21 15:12:25.000000 python_optimization-0.0.1/python_optimization/__init__.py
--rw-rw-rw-   0        0        0    21539 2024-04-21 15:09:08.000000 python_optimization-0.0.1/python_optimization/python_optimization.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:18:32.767675 python_optimization-0.0.1/python_optimization.egg-info/
--rw-rw-rw-   0        0        0      557 2024-04-21 15:18:32.000000 python_optimization-0.0.1/python_optimization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-04-21 15:18:32.000000 python_optimization-0.0.1/python_optimization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 15:18:32.000000 python_optimization-0.0.1/python_optimization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-21 15:18:32.000000 python_optimization-0.0.1/python_optimization.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 15:18:32.771651 python_optimization-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      867 2024-04-21 15:15:55.000000 python_optimization-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:49:59.677997 python_optimization-0.0.2/
+-rw-rw-rw-   0        0        0      557 2024-04-21 15:49:59.673996 python_optimization-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-21 15:49:59.649990 python_optimization-0.0.2/python_optimization/
+-rw-rw-rw-   0        0        0      114 2024-04-21 15:46:41.000000 python_optimization-0.0.2/python_optimization/__init__.py
+-rw-rw-rw-   0        0        0    21539 2024-04-21 15:09:08.000000 python_optimization-0.0.2/python_optimization/python_optimization.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:49:59.673996 python_optimization-0.0.2/python_optimization.egg-info/
+-rw-rw-rw-   0        0        0      557 2024-04-21 15:49:59.000000 python_optimization-0.0.2/python_optimization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-04-21 15:49:59.000000 python_optimization-0.0.2/python_optimization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 15:49:59.000000 python_optimization-0.0.2/python_optimization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-21 15:49:59.000000 python_optimization-0.0.2/python_optimization.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 15:49:59.677997 python_optimization-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      867 2024-04-21 15:48:22.000000 python_optimization-0.0.2/setup.py
```

### Comparing `python_optimization-0.0.1/PKG-INFO` & `python_optimization-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_optimization
-Version: 0.0.1
+Version: 0.0.2
 Summary: python optimization
 Author: NeuralNine (Florian Dedov)
 Author-email: <mail@neuralnine.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python_optimization-0.0.1/python_optimization/python_optimization.py` & `python_optimization-0.0.2/python_optimization/python_optimization.py`

 * *Files identical despite different names*

### Comparing `python_optimization-0.0.1/python_optimization.egg-info/PKG-INFO` & `python_optimization-0.0.2/python_optimization.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-optimization
-Version: 0.0.1
+Version: 0.0.2
 Summary: python optimization
 Author: NeuralNine (Florian Dedov)
 Author-email: <mail@neuralnine.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python_optimization-0.0.1/setup.py` & `python_optimization-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'python optimization'
 LONG_DESCRIPTION = 'A package that allows python optimization'
 
 # Setting up
 setup(
     name="python_optimization",
     version=VERSION,
```


# Comparing `tmp/python_optimization-0.0.4.tar.gz` & `tmp/python_optimization-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_optimization-0.0.4.tar", last modified: Sun Apr 21 15:59:59 2024, max compression
+gzip compressed data, was "python_optimization-0.0.5.tar", last modified: Sun Apr 21 16:07:07 2024, max compression
```

## Comparing `python_optimization-0.0.4.tar` & `python_optimization-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 15:59:59.995561 python_optimization-0.0.4/
--rw-rw-rw-   0        0        0      557 2024-04-21 15:59:59.995561 python_optimization-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-21 15:59:59.971551 python_optimization-0.0.4/python_optimization/
--rw-rw-rw-   0        0        0        0 2024-04-21 15:59:43.000000 python_optimization-0.0.4/python_optimization/__init__.py
--rw-rw-rw-   0        0        0    21539 2024-04-21 15:09:08.000000 python_optimization-0.0.4/python_optimization/python_optimization.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:59:59.991559 python_optimization-0.0.4/python_optimization.egg-info/
--rw-rw-rw-   0        0        0      557 2024-04-21 15:59:59.000000 python_optimization-0.0.4/python_optimization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-04-21 15:59:59.000000 python_optimization-0.0.4/python_optimization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 15:59:59.000000 python_optimization-0.0.4/python_optimization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-21 15:59:59.000000 python_optimization-0.0.4/python_optimization.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 15:59:59.995561 python_optimization-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      867 2024-04-21 15:59:51.000000 python_optimization-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 16:07:07.909820 python_optimization-0.0.5/
+-rw-rw-rw-   0        0        0      557 2024-04-21 16:07:07.905817 python_optimization-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-21 16:07:07.885823 python_optimization-0.0.5/python_optimization/
+-rw-rw-rw-   0        0        0      326 2024-04-21 16:03:34.000000 python_optimization-0.0.5/python_optimization/__init__.py
+-rw-rw-rw-   0        0        0    21539 2024-04-21 15:09:08.000000 python_optimization-0.0.5/python_optimization/python_optimization.py
+drwxrwxrwx   0        0        0        0 2024-04-21 16:07:07.905817 python_optimization-0.0.5/python_optimization.egg-info/
+-rw-rw-rw-   0        0        0      557 2024-04-21 16:07:07.000000 python_optimization-0.0.5/python_optimization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-04-21 16:07:07.000000 python_optimization-0.0.5/python_optimization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 16:07:07.000000 python_optimization-0.0.5/python_optimization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-21 16:07:07.000000 python_optimization-0.0.5/python_optimization.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 16:07:07.909820 python_optimization-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      867 2024-04-21 16:06:44.000000 python_optimization-0.0.5/setup.py
```

### Comparing `python_optimization-0.0.4/PKG-INFO` & `python_optimization-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_optimization
-Version: 0.0.4
+Version: 0.0.5
 Summary: python optimization
 Author: NeuralNine (Florian Dedov)
 Author-email: <mail@neuralnine.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python_optimization-0.0.4/python_optimization/python_optimization.py` & `python_optimization-0.0.5/python_optimization/python_optimization.py`

 * *Files identical despite different names*

### Comparing `python_optimization-0.0.4/python_optimization.egg-info/PKG-INFO` & `python_optimization-0.0.5/python_optimization.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-optimization
-Version: 0.0.4
+Version: 0.0.5
 Summary: python optimization
 Author: NeuralNine (Florian Dedov)
 Author-email: <mail@neuralnine.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python_optimization-0.0.4/setup.py` & `python_optimization-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'python optimization'
 LONG_DESCRIPTION = 'A package that allows python optimization'
 
 # Setting up
 setup(
     name="python_optimization",
     version=VERSION,
```


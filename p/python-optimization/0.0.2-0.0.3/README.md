# Comparing `tmp/python_optimization-0.0.2.tar.gz` & `tmp/python_optimization-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_optimization-0.0.2.tar", last modified: Sun Apr 21 15:49:59 2024, max compression
+gzip compressed data, was "python_optimization-0.0.3.tar", last modified: Sun Apr 21 15:57:59 2024, max compression
```

## Comparing `python_optimization-0.0.2.tar` & `python_optimization-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 15:49:59.677997 python_optimization-0.0.2/
--rw-rw-rw-   0        0        0      557 2024-04-21 15:49:59.673996 python_optimization-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-21 15:49:59.649990 python_optimization-0.0.2/python_optimization/
--rw-rw-rw-   0        0        0      114 2024-04-21 15:46:41.000000 python_optimization-0.0.2/python_optimization/__init__.py
--rw-rw-rw-   0        0        0    21539 2024-04-21 15:09:08.000000 python_optimization-0.0.2/python_optimization/python_optimization.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:49:59.673996 python_optimization-0.0.2/python_optimization.egg-info/
--rw-rw-rw-   0        0        0      557 2024-04-21 15:49:59.000000 python_optimization-0.0.2/python_optimization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-04-21 15:49:59.000000 python_optimization-0.0.2/python_optimization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 15:49:59.000000 python_optimization-0.0.2/python_optimization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-21 15:49:59.000000 python_optimization-0.0.2/python_optimization.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 15:49:59.677997 python_optimization-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      867 2024-04-21 15:48:22.000000 python_optimization-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:57:59.296027 python_optimization-0.0.3/
+-rw-rw-rw-   0        0        0      557 2024-04-21 15:57:59.296027 python_optimization-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-21 15:57:59.292003 python_optimization-0.0.3/python_optimization.egg-info/
+-rw-rw-rw-   0        0        0      557 2024-04-21 15:57:58.000000 python_optimization-0.0.3/python_optimization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2024-04-21 15:57:59.000000 python_optimization-0.0.3/python_optimization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 15:57:58.000000 python_optimization-0.0.3/python_optimization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 15:57:58.000000 python_optimization-0.0.3/python_optimization.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 15:57:59.296027 python_optimization-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      867 2024-04-21 15:57:48.000000 python_optimization-0.0.3/setup.py
```

### Comparing `python_optimization-0.0.2/PKG-INFO` & `python_optimization-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_optimization
-Version: 0.0.2
+Version: 0.0.3
 Summary: python optimization
 Author: NeuralNine (Florian Dedov)
 Author-email: <mail@neuralnine.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python_optimization-0.0.2/python_optimization.egg-info/PKG-INFO` & `python_optimization-0.0.3/python_optimization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-optimization
-Version: 0.0.2
+Version: 0.0.3
 Summary: python optimization
 Author: NeuralNine (Florian Dedov)
 Author-email: <mail@neuralnine.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python_optimization-0.0.2/setup.py` & `python_optimization-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'python optimization'
 LONG_DESCRIPTION = 'A package that allows python optimization'
 
 # Setting up
 setup(
     name="python_optimization",
     version=VERSION,
```


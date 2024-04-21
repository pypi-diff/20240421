# Comparing `tmp/cerbogen-0.0.48.tar.gz` & `tmp/cerbogen-0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.48.tar", last modified: Sun Apr 21 06:45:53 2024, max compression
+gzip compressed data, was "cerbogen-0.0.50.tar", last modified: Sun Apr 21 07:12:25 2024, max compression
```

## Comparing `cerbogen-0.0.48.tar` & `cerbogen-0.0.50.tar`

### file list

```diff
@@ -1,28 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 06:45:53.678162 cerbogen-0.0.48/
--rw-rw-rw-   0        0        0      680 2024-04-21 06:45:53.677165 cerbogen-0.0.48/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.48/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 06:45:53.656709 cerbogen-0.0.48/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-21 05:43:23.000000 cerbogen-0.0.48/cerbogen/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 06:45:53.653716 cerbogen-0.0.48/cerbogen/data/
-drwxrwxrwx   0        0        0        0 2024-04-21 06:45:53.667679 cerbogen-0.0.48/cerbogen/data/img/
--rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.48/cerbogen/data/img/logo.ico
--rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.48/cerbogen/data/img/logo.png
-drwxrwxrwx   0        0        0        0 2024-04-21 06:45:53.672666 cerbogen-0.0.48/cerbogen/install/
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.48/cerbogen/install/check.py
--rw-rw-rw-   0        0        0      594 2024-04-21 05:43:25.000000 cerbogen-0.0.48/cerbogen/install/install.py
--rw-rw-rw-   0        0        0     2930 2024-04-20 16:38:30.000000 cerbogen-0.0.48/cerbogen/install/install_ffmpeg.py
--rw-rw-rw-   0        0        0     2212 2024-04-21 05:38:09.000000 cerbogen-0.0.48/cerbogen/install/install_location.py
--rw-rw-rw-   0        0        0       35 2024-04-21 06:40:08.000000 cerbogen-0.0.48/cerbogen/install/try.py
--rw-rw-rw-   0        0        0    11588 2024-04-21 05:44:23.000000 cerbogen-0.0.48/cerbogen/main.py
-drwxrwxrwx   0        0        0        0 2024-04-21 06:45:53.675658 cerbogen-0.0.48/cerbogen/mod/
--rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.48/cerbogen/mod/__init__.py
--rw-rw-rw-   0        0        0     9057 2024-04-21 04:45:42.000000 cerbogen-0.0.48/cerbogen/mod/cerbogen.py
--rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.48/cerbogen/mod/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-21 06:45:53.676172 cerbogen-0.0.48/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      680 2024-04-21 06:45:53.000000 cerbogen-0.0.48/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2024-04-21 06:45:53.000000 cerbogen-0.0.48/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 06:45:53.000000 cerbogen-0.0.48/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-21 06:45:53.000000 cerbogen-0.0.48/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-21 06:45:53.000000 cerbogen-0.0.48/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 06:45:53.678162 cerbogen-0.0.48/setup.cfg
--rw-rw-rw-   0        0        0     1593 2024-04-21 06:45:53.000000 cerbogen-0.0.48/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 07:12:25.601954 cerbogen-0.0.50/
+-rw-rw-rw-   0        0        0      639 2024-04-21 07:12:25.600958 cerbogen-0.0.50/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.50/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 07:12:25.585000 cerbogen-0.0.50/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-21 05:43:23.000000 cerbogen-0.0.50/cerbogen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 07:12:25.582008 cerbogen-0.0.50/cerbogen/data/
+drwxrwxrwx   0        0        0        0 2024-04-21 07:12:25.597965 cerbogen-0.0.50/cerbogen/data/img/
+-rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.50/cerbogen/data/img/logo.ico
+-rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.50/cerbogen/data/img/logo.png
+-rw-rw-rw-   0        0        0    11564 2024-04-21 07:01:06.000000 cerbogen-0.0.50/cerbogen/main.py
+drwxrwxrwx   0        0        0        0 2024-04-21 07:12:25.599961 cerbogen-0.0.50/cerbogen/mod/
+-rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.50/cerbogen/mod/__init__.py
+-rw-rw-rw-   0        0        0     9057 2024-04-21 04:45:42.000000 cerbogen-0.0.50/cerbogen/mod/cerbogen.py
+-rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.50/cerbogen/mod/plot.py
+drwxrwxrwx   0        0        0        0 2024-04-21 07:12:25.600958 cerbogen-0.0.50/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      639 2024-04-21 07:12:25.000000 cerbogen-0.0.50/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2024-04-21 07:12:25.000000 cerbogen-0.0.50/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 07:12:25.000000 cerbogen-0.0.50/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-21 07:12:25.000000 cerbogen-0.0.50/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-21 07:12:25.000000 cerbogen-0.0.50/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 07:12:25.601954 cerbogen-0.0.50/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2024-04-21 07:12:24.000000 cerbogen-0.0.50/setup.py
```

### Comparing `cerbogen-0.0.48/PKG-INFO` & `cerbogen-0.0.50/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.48
+Version: 0.0.50
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
-Description-Content-Type: text/markdown
 Requires-Dist: matplotlib
 Requires-Dist: pydub
 Requires-Dist: numpy
 Requires-Dist: librosa
```

### Comparing `cerbogen-0.0.48/cerbogen/data/img/logo.ico` & `cerbogen-0.0.50/cerbogen/data/img/logo.ico`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.48/cerbogen/data/img/logo.png` & `cerbogen-0.0.50/cerbogen/data/img/logo.png`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.48/cerbogen/main.py` & `cerbogen-0.0.50/cerbogen/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import subprocess
-import pkg_resources
-
 import tkinter as tk
 from tkinter import ttk
 from tkinter import messagebox
 
 from cerbogen.mod.cerbogen import binbeats
 from cerbogen.mod.plot import Plot
```

### Comparing `cerbogen-0.0.48/cerbogen/mod/cerbogen.py` & `cerbogen-0.0.50/cerbogen/mod/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.48/cerbogen/mod/plot.py` & `cerbogen-0.0.50/cerbogen/mod/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.48/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.50/cerbogen.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.48
+Version: 0.0.50
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
-Description-Content-Type: text/markdown
 Requires-Dist: matplotlib
 Requires-Dist: pydub
 Requires-Dist: numpy
 Requires-Dist: librosa
```


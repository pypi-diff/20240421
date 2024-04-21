# Comparing `tmp/textile_metric-0.0.1.tar.gz` & `tmp/textile_metric-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textile_metric-0.0.1.tar", last modified: Sun Apr 21 09:33:15 2024, max compression
+gzip compressed data, was "textile_metric-0.0.2.tar", last modified: Sun Apr 21 09:40:24 2024, max compression
```

## Comparing `textile_metric-0.0.1.tar` & `textile_metric-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 09:33:15.074255 textile_metric-0.0.1/
--rw-rw-rw-   0        0        0     1103 2024-04-20 09:48:15.000000 textile_metric-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4100 2024-04-21 09:33:15.072749 textile_metric-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3216 2024-04-21 09:29:24.000000 textile_metric-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-21 09:33:15.074255 textile_metric-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1032 2024-04-21 09:32:59.000000 textile_metric-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:33:15.065600 textile_metric-0.0.1/textile/
--rw-rw-rw-   0        0        0        0 2024-04-20 09:56:47.000000 textile_metric-0.0.1/textile/__init__.py
--rw-rw-rw-   0        0        0     3133 2024-04-21 09:22:02.000000 textile_metric-0.0.1/textile/textile.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:33:15.072749 textile_metric-0.0.1/textile_metric.egg-info/
--rw-rw-rw-   0        0        0     4100 2024-04-21 09:33:15.000000 textile_metric-0.0.1/textile_metric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-04-21 09:33:15.000000 textile_metric-0.0.1/textile_metric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 09:33:15.000000 textile_metric-0.0.1/textile_metric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-04-21 09:33:15.000000 textile_metric-0.0.1/textile_metric.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-21 09:33:15.000000 textile_metric-0.0.1/textile_metric.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 09:40:24.727284 textile_metric-0.0.2/
+-rw-rw-rw-   0        0        0     1103 2024-04-20 09:48:15.000000 textile_metric-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4100 2024-04-21 09:40:24.726265 textile_metric-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3216 2024-04-21 09:29:24.000000 textile_metric-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-21 09:40:24.727284 textile_metric-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2024-04-21 09:40:19.000000 textile_metric-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:40:24.713102 textile_metric-0.0.2/textile/
+-rw-rw-rw-   0        0        0        0 2024-04-20 09:56:47.000000 textile_metric-0.0.2/textile/__init__.py
+-rw-rw-rw-   0        0        0     3133 2024-04-21 09:22:02.000000 textile_metric-0.0.2/textile/textile.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:40:24.725163 textile_metric-0.0.2/textile_metric.egg-info/
+-rw-rw-rw-   0        0        0     4100 2024-04-21 09:40:24.000000 textile_metric-0.0.2/textile_metric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-04-21 09:40:24.000000 textile_metric-0.0.2/textile_metric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 09:40:24.000000 textile_metric-0.0.2/textile_metric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-04-21 09:40:24.000000 textile_metric-0.0.2/textile_metric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-21 09:40:24.000000 textile_metric-0.0.2/textile_metric.egg-info/top_level.txt
```

### Comparing `textile_metric-0.0.1/LICENSE` & `textile_metric-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.1/PKG-INFO` & `textile_metric-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textile-metric
-Version: 0.0.1
+Version: 0.0.2
 Summary: TexTile: A Differentiable Metric for Texture Tileability
 Home-page: https://github.com/crp94/textile
 Author: Carlos Rodriguez-Pardo
 Author-email: carlos.rodriguezpardo.jimenez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `textile_metric-0.0.1/README.md` & `textile_metric-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.1/setup.py` & `textile_metric-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='textile-metric',
-     version='0.0.1',
+     version='0.0.2',
      author="Carlos Rodriguez-Pardo",
      author_email="carlos.rodriguezpardo.jimenez@gmail.com",
      description="TexTile: A Differentiable Metric for Texture Tileability",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/crp94/textile",
      packages=['textile'],
```

### Comparing `textile_metric-0.0.1/textile/textile.py` & `textile_metric-0.0.2/textile/textile.py`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.1/textile_metric.egg-info/PKG-INFO` & `textile_metric-0.0.2/textile_metric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textile-metric
-Version: 0.0.1
+Version: 0.0.2
 Summary: TexTile: A Differentiable Metric for Texture Tileability
 Home-page: https://github.com/crp94/textile
 Author: Carlos Rodriguez-Pardo
 Author-email: carlos.rodriguezpardo.jimenez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```


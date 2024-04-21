# Comparing `tmp/textile_metric-0.0.4.tar.gz` & `tmp/textile_metric-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textile_metric-0.0.4.tar", last modified: Sun Apr 21 09:50:30 2024, max compression
+gzip compressed data, was "textile_metric-0.0.5.tar", last modified: Sun Apr 21 09:55:15 2024, max compression
```

## Comparing `textile_metric-0.0.4.tar` & `textile_metric-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 09:50:30.654006 textile_metric-0.0.4/
--rw-rw-rw-   0        0        0     1103 2024-04-20 09:48:15.000000 textile_metric-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     4147 2024-04-21 09:50:30.652882 textile_metric-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3263 2024-04-21 09:42:25.000000 textile_metric-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-21 09:50:30.655058 textile_metric-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1126 2024-04-21 09:50:23.000000 textile_metric-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:50:30.622301 textile_metric-0.0.4/textile/
--rw-rw-rw-   0        0        0       99 2024-04-21 09:49:56.000000 textile_metric-0.0.4/textile/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:50:30.633078 textile_metric-0.0.4/textile/data/
--rw-rw-rw-   0        0        0  4087314 2024-04-21 08:42:09.000000 textile_metric-0.0.4/textile/data/teaser.png
--rw-rw-rw-   0        0        0  1289541 2024-04-21 09:06:31.000000 textile_metric-0.0.4/textile/data/texture_368.jpg
--rw-rw-rw-   0        0        0     3131 2024-04-21 09:50:23.000000 textile_metric-0.0.4/textile/textile.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:50:30.651897 textile_metric-0.0.4/textile_metric.egg-info/
--rw-rw-rw-   0        0        0     4147 2024-04-21 09:50:30.000000 textile_metric-0.0.4/textile_metric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2024-04-21 09:50:30.000000 textile_metric-0.0.4/textile_metric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 09:50:30.000000 textile_metric-0.0.4/textile_metric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-04-21 09:50:30.000000 textile_metric-0.0.4/textile_metric.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-21 09:50:30.000000 textile_metric-0.0.4/textile_metric.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 09:55:15.927023 textile_metric-0.0.5/
+-rw-rw-rw-   0        0        0     1103 2024-04-20 09:48:15.000000 textile_metric-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4147 2024-04-21 09:55:15.925166 textile_metric-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3263 2024-04-21 09:42:25.000000 textile_metric-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-21 09:55:15.927023 textile_metric-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1126 2024-04-21 09:55:04.000000 textile_metric-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:55:15.901408 textile_metric-0.0.5/textile/
+-rw-rw-rw-   0        0        0      213 2024-04-21 09:54:11.000000 textile_metric-0.0.5/textile/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:55:15.907591 textile_metric-0.0.5/textile/data/
+-rw-rw-rw-   0        0        0  4087314 2024-04-21 08:42:09.000000 textile_metric-0.0.5/textile/data/teaser.png
+-rw-rw-rw-   0        0        0  1289541 2024-04-21 09:06:31.000000 textile_metric-0.0.5/textile/data/texture_368.jpg
+-rw-rw-rw-   0        0        0     3193 2024-04-21 09:53:50.000000 textile_metric-0.0.5/textile/textile.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:55:15.923758 textile_metric-0.0.5/textile_metric.egg-info/
+-rw-rw-rw-   0        0        0     4147 2024-04-21 09:55:15.000000 textile_metric-0.0.5/textile_metric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-04-21 09:55:15.000000 textile_metric-0.0.5/textile_metric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 09:55:15.000000 textile_metric-0.0.5/textile_metric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-04-21 09:55:15.000000 textile_metric-0.0.5/textile_metric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-21 09:55:15.000000 textile_metric-0.0.5/textile_metric.egg-info/top_level.txt
```

### Comparing `textile_metric-0.0.4/LICENSE` & `textile_metric-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.4/PKG-INFO` & `textile_metric-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textile-metric
-Version: 0.0.4
+Version: 0.0.5
 Summary: TexTile: A Differentiable Metric for Texture Tileability
 Home-page: https://github.com/crp94/textile
 Author: Carlos Rodriguez-Pardo
 Author-email: carlos.rodriguezpardo.jimenez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `textile_metric-0.0.4/README.md` & `textile_metric-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.4/setup.py` & `textile_metric-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='textile-metric',
-     version='0.0.4',
+     version='0.0.5',
      author="Carlos Rodriguez-Pardo",
      author_email="carlos.rodriguezpardo.jimenez@gmail.com",
      description="TexTile: A Differentiable Metric for Texture Tileability",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/crp94/textile",
      packages=['textile'],
```

### Comparing `textile_metric-0.0.4/textile/data/teaser.png` & `textile_metric-0.0.5/textile/data/teaser.png`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.4/textile/data/texture_368.jpg` & `textile_metric-0.0.5/textile/data/texture_368.jpg`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.4/textile/textile.py` & `textile_metric-0.0.5/textile/textile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+from __future__ import absolute_import
+
+
 import os
 from torchvision import transforms
 
 import numpy as np
 import torch
 from torch import nn
 
+import textile
+
 from textile.utils.misc import MyProgressBar
 from textile.utils.create_model import CreateModel
 
 class Textile(nn.Module):
     def __init__(self, model_path: str = "textile/models/textile.pth", lambda_value: float = 0.25, resolution = (512, 512), number_tiles = 2):
         """
         Implementation of TexTile: A Differentiable Metric for Texture Tileability
```

### Comparing `textile_metric-0.0.4/textile_metric.egg-info/PKG-INFO` & `textile_metric-0.0.5/textile_metric.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textile-metric
-Version: 0.0.4
+Version: 0.0.5
 Summary: TexTile: A Differentiable Metric for Texture Tileability
 Home-page: https://github.com/crp94/textile
 Author: Carlos Rodriguez-Pardo
 Author-email: carlos.rodriguezpardo.jimenez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```


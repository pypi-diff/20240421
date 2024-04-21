# Comparing `tmp/textile_metric-0.0.3.tar.gz` & `tmp/textile_metric-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textile_metric-0.0.3.tar", last modified: Sun Apr 21 09:45:22 2024, max compression
+gzip compressed data, was "textile_metric-0.0.4.tar", last modified: Sun Apr 21 09:50:30 2024, max compression
```

## Comparing `textile_metric-0.0.3.tar` & `textile_metric-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 09:45:22.546179 textile_metric-0.0.3/
--rw-rw-rw-   0        0        0     1103 2024-04-20 09:48:15.000000 textile_metric-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     4147 2024-04-21 09:45:22.545182 textile_metric-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3263 2024-04-21 09:42:25.000000 textile_metric-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-21 09:45:22.546179 textile_metric-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1126 2024-04-21 09:45:15.000000 textile_metric-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:45:22.514650 textile_metric-0.0.3/textile/
--rw-rw-rw-   0        0        0        0 2024-04-20 09:56:47.000000 textile_metric-0.0.3/textile/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:45:22.524275 textile_metric-0.0.3/textile/data/
--rw-rw-rw-   0        0        0  4087314 2024-04-21 08:42:09.000000 textile_metric-0.0.3/textile/data/teaser.png
--rw-rw-rw-   0        0        0  1289541 2024-04-21 09:06:31.000000 textile_metric-0.0.3/textile/data/texture_368.jpg
--rw-rw-rw-   0        0        0     3133 2024-04-21 09:22:02.000000 textile_metric-0.0.3/textile/textile.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:45:22.544184 textile_metric-0.0.3/textile_metric.egg-info/
--rw-rw-rw-   0        0        0     4147 2024-04-21 09:45:22.000000 textile_metric-0.0.3/textile_metric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2024-04-21 09:45:22.000000 textile_metric-0.0.3/textile_metric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 09:45:22.000000 textile_metric-0.0.3/textile_metric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-04-21 09:45:22.000000 textile_metric-0.0.3/textile_metric.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-21 09:45:22.000000 textile_metric-0.0.3/textile_metric.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 09:50:30.654006 textile_metric-0.0.4/
+-rw-rw-rw-   0        0        0     1103 2024-04-20 09:48:15.000000 textile_metric-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4147 2024-04-21 09:50:30.652882 textile_metric-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3263 2024-04-21 09:42:25.000000 textile_metric-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-21 09:50:30.655058 textile_metric-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1126 2024-04-21 09:50:23.000000 textile_metric-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:50:30.622301 textile_metric-0.0.4/textile/
+-rw-rw-rw-   0        0        0       99 2024-04-21 09:49:56.000000 textile_metric-0.0.4/textile/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:50:30.633078 textile_metric-0.0.4/textile/data/
+-rw-rw-rw-   0        0        0  4087314 2024-04-21 08:42:09.000000 textile_metric-0.0.4/textile/data/teaser.png
+-rw-rw-rw-   0        0        0  1289541 2024-04-21 09:06:31.000000 textile_metric-0.0.4/textile/data/texture_368.jpg
+-rw-rw-rw-   0        0        0     3131 2024-04-21 09:50:23.000000 textile_metric-0.0.4/textile/textile.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:50:30.651897 textile_metric-0.0.4/textile_metric.egg-info/
+-rw-rw-rw-   0        0        0     4147 2024-04-21 09:50:30.000000 textile_metric-0.0.4/textile_metric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-04-21 09:50:30.000000 textile_metric-0.0.4/textile_metric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 09:50:30.000000 textile_metric-0.0.4/textile_metric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-04-21 09:50:30.000000 textile_metric-0.0.4/textile_metric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-21 09:50:30.000000 textile_metric-0.0.4/textile_metric.egg-info/top_level.txt
```

### Comparing `textile_metric-0.0.3/LICENSE` & `textile_metric-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.3/PKG-INFO` & `textile_metric-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textile-metric
-Version: 0.0.3
+Version: 0.0.4
 Summary: TexTile: A Differentiable Metric for Texture Tileability
 Home-page: https://github.com/crp94/textile
 Author: Carlos Rodriguez-Pardo
 Author-email: carlos.rodriguezpardo.jimenez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `textile_metric-0.0.3/README.md` & `textile_metric-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.3/setup.py` & `textile_metric-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='textile-metric',
-     version='0.0.3',
+     version='0.0.4',
      author="Carlos Rodriguez-Pardo",
      author_email="carlos.rodriguezpardo.jimenez@gmail.com",
      description="TexTile: A Differentiable Metric for Texture Tileability",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/crp94/textile",
      packages=['textile'],
```

### Comparing `textile_metric-0.0.3/textile/data/teaser.png` & `textile_metric-0.0.4/textile/data/teaser.png`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.3/textile/data/texture_368.jpg` & `textile_metric-0.0.4/textile/data/texture_368.jpg`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.3/textile/textile.py` & `textile_metric-0.0.4/textile/textile.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import numpy as np
 import torch
 from torch import nn
 
 from textile.utils.misc import MyProgressBar
 from textile.utils.create_model import CreateModel
 
-
 class Textile(nn.Module):
     def __init__(self, model_path: str = "textile/models/textile.pth", lambda_value: float = 0.25, resolution = (512, 512), number_tiles = 2):
         """
         Implementation of TexTile: A Differentiable Metric for Texture Tileability
         :param model_path: Path to pretrained model
         :param lambda_value: Lambda value to transform the unbounded model prediction to the (0, 1) range. Higher lambdas provide more sensitive predictions. Check our supplementary material for more details.
         :param resolution: Resolution of the image provided to the model after tiling.
```

### Comparing `textile_metric-0.0.3/textile_metric.egg-info/PKG-INFO` & `textile_metric-0.0.4/textile_metric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textile-metric
-Version: 0.0.3
+Version: 0.0.4
 Summary: TexTile: A Differentiable Metric for Texture Tileability
 Home-page: https://github.com/crp94/textile
 Author: Carlos Rodriguez-Pardo
 Author-email: carlos.rodriguezpardo.jimenez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```


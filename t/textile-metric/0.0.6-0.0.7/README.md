# Comparing `tmp/textile_metric-0.0.6.tar.gz` & `tmp/textile_metric-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textile_metric-0.0.6.tar", last modified: Sun Apr 21 10:00:20 2024, max compression
+gzip compressed data, was "textile_metric-0.0.7.tar", last modified: Sun Apr 21 10:08:37 2024, max compression
```

## Comparing `textile_metric-0.0.6.tar` & `textile_metric-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 10:00:20.871134 textile_metric-0.0.6/
--rw-rw-rw-   0        0        0     1103 2024-04-20 09:48:15.000000 textile_metric-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     4147 2024-04-21 10:00:20.869631 textile_metric-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3263 2024-04-21 09:42:25.000000 textile_metric-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-21 10:00:20.871134 textile_metric-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1126 2024-04-21 10:00:18.000000 textile_metric-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 10:00:20.840120 textile_metric-0.0.6/textile/
--rw-rw-rw-   0        0        0      213 2024-04-21 09:54:11.000000 textile_metric-0.0.6/textile/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 10:00:20.844710 textile_metric-0.0.6/textile/data/
--rw-rw-rw-   0        0        0  4087314 2024-04-21 08:42:09.000000 textile_metric-0.0.6/textile/data/teaser.png
--rw-rw-rw-   0        0        0  1289541 2024-04-21 09:06:31.000000 textile_metric-0.0.6/textile/data/texture_368.jpg
--rw-rw-rw-   0        0        0     3177 2024-04-21 10:00:06.000000 textile_metric-0.0.6/textile/textile.py
-drwxrwxrwx   0        0        0        0 2024-04-21 10:00:20.867639 textile_metric-0.0.6/textile_metric.egg-info/
--rw-rw-rw-   0        0        0     4147 2024-04-21 10:00:20.000000 textile_metric-0.0.6/textile_metric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2024-04-21 10:00:20.000000 textile_metric-0.0.6/textile_metric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 10:00:20.000000 textile_metric-0.0.6/textile_metric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-04-21 10:00:20.000000 textile_metric-0.0.6/textile_metric.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-21 10:00:20.000000 textile_metric-0.0.6/textile_metric.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 10:08:37.209396 textile_metric-0.0.7/
+-rw-rw-rw-   0        0        0     1103 2024-04-20 09:48:15.000000 textile_metric-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4147 2024-04-21 10:08:37.208398 textile_metric-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3263 2024-04-21 09:42:25.000000 textile_metric-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-21 10:08:37.209396 textile_metric-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-04-21 10:06:36.000000 textile_metric-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:08:37.187720 textile_metric-0.0.7/textile/
+-rw-rw-rw-   0        0        0      311 2024-04-21 10:03:59.000000 textile_metric-0.0.7/textile/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:08:37.188717 textile_metric-0.0.7/textile/architectures/
+-rw-rw-rw-   0        0        0        0 2024-04-20 09:56:55.000000 textile_metric-0.0.7/textile/architectures/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:08:37.188717 textile_metric-0.0.7/textile/architectures/layers/
+-rw-rw-rw-   0        0        0        0 2024-04-20 09:57:58.000000 textile_metric-0.0.7/textile/architectures/layers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:08:37.190224 textile_metric-0.0.7/textile/architectures/layers/attention/
+-rw-rw-rw-   0        0        0        0 2024-04-20 09:58:11.000000 textile_metric-0.0.7/textile/architectures/layers/attention/__init__.py
+-rw-rw-rw-   0        0        0     1692 2024-04-20 10:44:38.000000 textile_metric-0.0.7/textile/architectures/layers/attention/attention.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:08:37.195307 textile_metric-0.0.7/textile/data/
+-rw-rw-rw-   0        0        0  4087314 2024-04-21 08:42:09.000000 textile_metric-0.0.7/textile/data/teaser.png
+-rw-rw-rw-   0        0        0  1289541 2024-04-21 09:06:31.000000 textile_metric-0.0.7/textile/data/texture_368.jpg
+-rw-rw-rw-   0        0        0     3135 2024-04-21 10:03:59.000000 textile_metric-0.0.7/textile/textile.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:08:37.200815 textile_metric-0.0.7/textile/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-20 10:01:22.000000 textile_metric-0.0.7/textile/utils/__init__.py
+-rw-rw-rw-   0        0        0     1278 2024-04-20 10:44:38.000000 textile_metric-0.0.7/textile/utils/create_model.py
+-rw-rw-rw-   0        0        0     1223 2024-04-20 10:17:53.000000 textile_metric-0.0.7/textile/utils/dataset.py
+-rw-rw-rw-   0        0        0      296 2024-04-21 09:16:14.000000 textile_metric-0.0.7/textile/utils/image_utils.py
+-rw-rw-rw-   0        0        0      454 2024-04-21 09:02:07.000000 textile_metric-0.0.7/textile/utils/misc.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:08:37.207402 textile_metric-0.0.7/textile_metric.egg-info/
+-rw-rw-rw-   0        0        0     4147 2024-04-21 10:08:37.000000 textile_metric-0.0.7/textile_metric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2024-04-21 10:08:37.000000 textile_metric-0.0.7/textile_metric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 10:08:37.000000 textile_metric-0.0.7/textile_metric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-04-21 10:08:37.000000 textile_metric-0.0.7/textile_metric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-21 10:08:37.000000 textile_metric-0.0.7/textile_metric.egg-info/top_level.txt
```

### Comparing `textile_metric-0.0.6/LICENSE` & `textile_metric-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.6/PKG-INFO` & `textile_metric-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textile-metric
-Version: 0.0.6
+Version: 0.0.7
 Summary: TexTile: A Differentiable Metric for Texture Tileability
 Home-page: https://github.com/crp94/textile
 Author: Carlos Rodriguez-Pardo
 Author-email: carlos.rodriguezpardo.jimenez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `textile_metric-0.0.6/README.md` & `textile_metric-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.6/setup.py` & `textile_metric-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='textile-metric',
-     version='0.0.6',
+     version='0.0.7',
      author="Carlos Rodriguez-Pardo",
      author_email="carlos.rodriguezpardo.jimenez@gmail.com",
      description="TexTile: A Differentiable Metric for Texture Tileability",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/crp94/textile",
      packages=['textile'],
-     package_data={'textile': ['data/*.png','data/*.jpg']},
+     package_data={'textile': ['data/*.png','data/*.jpg', 'utils/*.py', 'architectures/*.py', 'architectures/layers/*.py', 'architectures/layers/attention/*.py']},
      include_package_data=True,
      install_requires=["torch>=1.2.0", "torchvision>=0.17.1", "einops>=0.7.0", "numpy>=1.14.3", "opencv-python>=2.4.11", "kornia>=0.7.2", "progressbar>=2.5"],
      classifiers=[
          "Programming Language :: Python :: 3",
          "Operating System :: OS Independent",
          "Development Status :: 4 - Beta",
          "License :: OSI Approved :: MIT License",
```

### Comparing `textile_metric-0.0.6/textile/data/teaser.png` & `textile_metric-0.0.7/textile/data/teaser.png`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.6/textile/data/texture_368.jpg` & `textile_metric-0.0.7/textile/data/texture_368.jpg`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.6/textile/textile.py` & `textile_metric-0.0.7/textile/textile.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 import torch
 from torch import nn
 
 import textile
 
 from utils.misc import MyProgressBar
-from utils.create_model import CreateModel
+
 
 class Textile(nn.Module):
     def __init__(self, model_path: str = "textile/models/textile.pth", lambda_value: float = 0.25, resolution = (512, 512), number_tiles = 2):
         """
         Implementation of TexTile: A Differentiable Metric for Texture Tileability
         :param model_path: Path to pretrained model
         :param lambda_value: Lambda value to transform the unbounded model prediction to the (0, 1) range. Higher lambdas provide more sensitive predictions. Check our supplementary material for more details.
```

### Comparing `textile_metric-0.0.6/textile_metric.egg-info/PKG-INFO` & `textile_metric-0.0.7/textile_metric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textile-metric
-Version: 0.0.6
+Version: 0.0.7
 Summary: TexTile: A Differentiable Metric for Texture Tileability
 Home-page: https://github.com/crp94/textile
 Author: Carlos Rodriguez-Pardo
 Author-email: carlos.rodriguezpardo.jimenez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```


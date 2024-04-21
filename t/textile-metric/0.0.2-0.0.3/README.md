# Comparing `tmp/textile_metric-0.0.2.tar.gz` & `tmp/textile_metric-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textile_metric-0.0.2.tar", last modified: Sun Apr 21 09:40:24 2024, max compression
+gzip compressed data, was "textile_metric-0.0.3.tar", last modified: Sun Apr 21 09:45:22 2024, max compression
```

## Comparing `textile_metric-0.0.2.tar` & `textile_metric-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 09:40:24.727284 textile_metric-0.0.2/
--rw-rw-rw-   0        0        0     1103 2024-04-20 09:48:15.000000 textile_metric-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4100 2024-04-21 09:40:24.726265 textile_metric-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3216 2024-04-21 09:29:24.000000 textile_metric-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-21 09:40:24.727284 textile_metric-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1032 2024-04-21 09:40:19.000000 textile_metric-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:40:24.713102 textile_metric-0.0.2/textile/
--rw-rw-rw-   0        0        0        0 2024-04-20 09:56:47.000000 textile_metric-0.0.2/textile/__init__.py
--rw-rw-rw-   0        0        0     3133 2024-04-21 09:22:02.000000 textile_metric-0.0.2/textile/textile.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:40:24.725163 textile_metric-0.0.2/textile_metric.egg-info/
--rw-rw-rw-   0        0        0     4100 2024-04-21 09:40:24.000000 textile_metric-0.0.2/textile_metric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-04-21 09:40:24.000000 textile_metric-0.0.2/textile_metric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 09:40:24.000000 textile_metric-0.0.2/textile_metric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-04-21 09:40:24.000000 textile_metric-0.0.2/textile_metric.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-21 09:40:24.000000 textile_metric-0.0.2/textile_metric.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 09:45:22.546179 textile_metric-0.0.3/
+-rw-rw-rw-   0        0        0     1103 2024-04-20 09:48:15.000000 textile_metric-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4147 2024-04-21 09:45:22.545182 textile_metric-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3263 2024-04-21 09:42:25.000000 textile_metric-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-21 09:45:22.546179 textile_metric-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1126 2024-04-21 09:45:15.000000 textile_metric-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:45:22.514650 textile_metric-0.0.3/textile/
+-rw-rw-rw-   0        0        0        0 2024-04-20 09:56:47.000000 textile_metric-0.0.3/textile/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:45:22.524275 textile_metric-0.0.3/textile/data/
+-rw-rw-rw-   0        0        0  4087314 2024-04-21 08:42:09.000000 textile_metric-0.0.3/textile/data/teaser.png
+-rw-rw-rw-   0        0        0  1289541 2024-04-21 09:06:31.000000 textile_metric-0.0.3/textile/data/texture_368.jpg
+-rw-rw-rw-   0        0        0     3133 2024-04-21 09:22:02.000000 textile_metric-0.0.3/textile/textile.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:45:22.544184 textile_metric-0.0.3/textile_metric.egg-info/
+-rw-rw-rw-   0        0        0     4147 2024-04-21 09:45:22.000000 textile_metric-0.0.3/textile_metric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-04-21 09:45:22.000000 textile_metric-0.0.3/textile_metric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 09:45:22.000000 textile_metric-0.0.3/textile_metric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-04-21 09:45:22.000000 textile_metric-0.0.3/textile_metric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-21 09:45:22.000000 textile_metric-0.0.3/textile_metric.egg-info/top_level.txt
```

### Comparing `textile_metric-0.0.2/LICENSE` & `textile_metric-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.2/PKG-INFO` & `textile_metric-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textile-metric
-Version: 0.0.2
+Version: 0.0.3
 Summary: TexTile: A Differentiable Metric for Texture Tileability
 Home-page: https://github.com/crp94/textile
 Author: Carlos Rodriguez-Pardo
 Author-email: carlos.rodriguezpardo.jimenez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -21,20 +21,20 @@
 Requires-Dist: kornia>=0.7.2
 Requires-Dist: progressbar>=2.5
 
 # TexTile: A Differentiable Metric for Texture Tileability
 
 Official repository of "TexTile: A Differentiable Metric for Texture Tileability" [CVPR 2024]
 
-[Carlos Rodriguez-Pardo](https://richzhang.github.io/), [Dan Casas](https://dancasas.github.io/), [Elena Garces](https://www.elenagarces.es/), [Jorge Lopez-Moreno](http://www.jorg3.com/)
+[Carlos Rodriguez-Pardo](https://carlosrodriguezpardo.es/), [Dan Casas](https://dancasas.github.io/), [Elena Garces](https://www.elenagarces.es/), [Jorge Lopez-Moreno](http://www.jorg3.com/)
 
 In [CVPR](https://arxiv.org/abs/2403.12961v1), 2024.
 
 
-<img src='textile/data/teaser.png' width=1200>
+<img src='https://github.com/crp94/textile/blob/main/textile/data/teaser.png' width=1200>
 
 We introduce TexTile, a novel differentiable metric to quantify the degree upon which a texture image can be concatenated with itself without introducing repeating artifacts (i.e., the tileability). Existing methods for tileable texture synthesis focus on general texture quality, but lack explicit analysis of the intrinsic repeatability properties of a texture. In contrast, our TexTile metric effectively evaluates the tileable properties of a texture, opening the door to more informed synthesis and analysis of tileable textures. Under the hood, TexTile is formulated as a binary classifier carefully built from a large dataset of textures of different styles, semantics, regularities, and human annotations. Key to our method is a set of architectural modifications to baseline pre-train image classifiers to overcome their shortcomings at measuring tileability, along with a custom data augmentation and training regime aimed at increasing robustness and accuracy. We demonstrate that TexTile can be plugged into different state-of-the-art texture synthesis methods, including diffusion-based strategies, and generate tileable textures while keeping or even improving the overall texture quality. Furthermore, we show that TexTile can objectively evaluate any tileable texture synthesis method, whereas the current mix of existing metrics produces uncorrelated scores which heavily hinders progress in the field.
 
 
 ### Quick start
 
 Run `pip install textile-metric`. The following Python code is all you need. Note that models are downloaded automatically.
```

### Comparing `textile_metric-0.0.2/README.md` & `textile_metric-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # TexTile: A Differentiable Metric for Texture Tileability
 
 Official repository of "TexTile: A Differentiable Metric for Texture Tileability" [CVPR 2024]
 
-[Carlos Rodriguez-Pardo](https://richzhang.github.io/), [Dan Casas](https://dancasas.github.io/), [Elena Garces](https://www.elenagarces.es/), [Jorge Lopez-Moreno](http://www.jorg3.com/)
+[Carlos Rodriguez-Pardo](https://carlosrodriguezpardo.es/), [Dan Casas](https://dancasas.github.io/), [Elena Garces](https://www.elenagarces.es/), [Jorge Lopez-Moreno](http://www.jorg3.com/)
 
 In [CVPR](https://arxiv.org/abs/2403.12961v1), 2024.
 
 
-<img src='textile/data/teaser.png' width=1200>
+<img src='https://github.com/crp94/textile/blob/main/textile/data/teaser.png' width=1200>
 
 We introduce TexTile, a novel differentiable metric to quantify the degree upon which a texture image can be concatenated with itself without introducing repeating artifacts (i.e., the tileability). Existing methods for tileable texture synthesis focus on general texture quality, but lack explicit analysis of the intrinsic repeatability properties of a texture. In contrast, our TexTile metric effectively evaluates the tileable properties of a texture, opening the door to more informed synthesis and analysis of tileable textures. Under the hood, TexTile is formulated as a binary classifier carefully built from a large dataset of textures of different styles, semantics, regularities, and human annotations. Key to our method is a set of architectural modifications to baseline pre-train image classifiers to overcome their shortcomings at measuring tileability, along with a custom data augmentation and training regime aimed at increasing robustness and accuracy. We demonstrate that TexTile can be plugged into different state-of-the-art texture synthesis methods, including diffusion-based strategies, and generate tileable textures while keeping or even improving the overall texture quality. Furthermore, we show that TexTile can objectively evaluate any tileable texture synthesis method, whereas the current mix of existing metrics produces uncorrelated scores which heavily hinders progress in the field.
 
 
 ### Quick start
 
 Run `pip install textile-metric`. The following Python code is all you need. Note that models are downloaded automatically.
```

### Comparing `textile_metric-0.0.2/setup.py` & `textile_metric-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='textile-metric',
-     version='0.0.2',
+     version='0.0.3',
      author="Carlos Rodriguez-Pardo",
      author_email="carlos.rodriguezpardo.jimenez@gmail.com",
      description="TexTile: A Differentiable Metric for Texture Tileability",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/crp94/textile",
      packages=['textile'],
+     package_data={'textile': ['data/*.png','data/*.jpg']},
+     include_package_data=True,
      install_requires=["torch>=1.2.0", "torchvision>=0.17.1", "einops>=0.7.0", "numpy>=1.14.3", "opencv-python>=2.4.11", "kornia>=0.7.2", "progressbar>=2.5"],
      classifiers=[
          "Programming Language :: Python :: 3",
          "Operating System :: OS Independent",
          "Development Status :: 4 - Beta",
          "License :: OSI Approved :: MIT License",
          "Topic :: Scientific/Engineering :: Image Processing",
```

### Comparing `textile_metric-0.0.2/textile/textile.py` & `textile_metric-0.0.3/textile/textile.py`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.2/textile_metric.egg-info/PKG-INFO` & `textile_metric-0.0.3/textile_metric.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textile-metric
-Version: 0.0.2
+Version: 0.0.3
 Summary: TexTile: A Differentiable Metric for Texture Tileability
 Home-page: https://github.com/crp94/textile
 Author: Carlos Rodriguez-Pardo
 Author-email: carlos.rodriguezpardo.jimenez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -21,20 +21,20 @@
 Requires-Dist: kornia>=0.7.2
 Requires-Dist: progressbar>=2.5
 
 # TexTile: A Differentiable Metric for Texture Tileability
 
 Official repository of "TexTile: A Differentiable Metric for Texture Tileability" [CVPR 2024]
 
-[Carlos Rodriguez-Pardo](https://richzhang.github.io/), [Dan Casas](https://dancasas.github.io/), [Elena Garces](https://www.elenagarces.es/), [Jorge Lopez-Moreno](http://www.jorg3.com/)
+[Carlos Rodriguez-Pardo](https://carlosrodriguezpardo.es/), [Dan Casas](https://dancasas.github.io/), [Elena Garces](https://www.elenagarces.es/), [Jorge Lopez-Moreno](http://www.jorg3.com/)
 
 In [CVPR](https://arxiv.org/abs/2403.12961v1), 2024.
 
 
-<img src='textile/data/teaser.png' width=1200>
+<img src='https://github.com/crp94/textile/blob/main/textile/data/teaser.png' width=1200>
 
 We introduce TexTile, a novel differentiable metric to quantify the degree upon which a texture image can be concatenated with itself without introducing repeating artifacts (i.e., the tileability). Existing methods for tileable texture synthesis focus on general texture quality, but lack explicit analysis of the intrinsic repeatability properties of a texture. In contrast, our TexTile metric effectively evaluates the tileable properties of a texture, opening the door to more informed synthesis and analysis of tileable textures. Under the hood, TexTile is formulated as a binary classifier carefully built from a large dataset of textures of different styles, semantics, regularities, and human annotations. Key to our method is a set of architectural modifications to baseline pre-train image classifiers to overcome their shortcomings at measuring tileability, along with a custom data augmentation and training regime aimed at increasing robustness and accuracy. We demonstrate that TexTile can be plugged into different state-of-the-art texture synthesis methods, including diffusion-based strategies, and generate tileable textures while keeping or even improving the overall texture quality. Furthermore, we show that TexTile can objectively evaluate any tileable texture synthesis method, whereas the current mix of existing metrics produces uncorrelated scores which heavily hinders progress in the field.
 
 
 ### Quick start
 
 Run `pip install textile-metric`. The following Python code is all you need. Note that models are downloaded automatically.
```


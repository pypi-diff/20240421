# Comparing `tmp/textile_metric-0.0.8.tar.gz` & `tmp/textile_metric-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textile_metric-0.0.8.tar", last modified: Sun Apr 21 10:11:52 2024, max compression
+gzip compressed data, was "textile_metric-0.0.9.tar", last modified: Sun Apr 21 10:20:07 2024, max compression
```

## Comparing `textile_metric-0.0.8.tar` & `textile_metric-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 10:11:52.175042 textile_metric-0.0.8/
--rw-rw-rw-   0        0        0     1103 2024-04-20 09:48:15.000000 textile_metric-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     4104 2024-04-21 10:11:52.174044 textile_metric-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3220 2024-04-21 10:10:12.000000 textile_metric-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-21 10:11:52.175042 textile_metric-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-04-21 10:11:48.000000 textile_metric-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 10:11:52.139147 textile_metric-0.0.8/textile/
--rw-rw-rw-   0        0        0      311 2024-04-21 10:03:59.000000 textile_metric-0.0.8/textile/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 10:11:52.140144 textile_metric-0.0.8/textile/architectures/
--rw-rw-rw-   0        0        0        0 2024-04-20 09:56:55.000000 textile_metric-0.0.8/textile/architectures/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 10:11:52.140144 textile_metric-0.0.8/textile/architectures/layers/
--rw-rw-rw-   0        0        0        0 2024-04-20 09:57:58.000000 textile_metric-0.0.8/textile/architectures/layers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 10:11:52.141142 textile_metric-0.0.8/textile/architectures/layers/attention/
--rw-rw-rw-   0        0        0        0 2024-04-20 09:58:11.000000 textile_metric-0.0.8/textile/architectures/layers/attention/__init__.py
--rw-rw-rw-   0        0        0     1692 2024-04-20 10:44:38.000000 textile_metric-0.0.8/textile/architectures/layers/attention/attention.py
-drwxrwxrwx   0        0        0        0 2024-04-21 10:11:52.151846 textile_metric-0.0.8/textile/data/
--rw-rw-rw-   0        0        0  4087314 2024-04-21 08:42:09.000000 textile_metric-0.0.8/textile/data/teaser.png
--rw-rw-rw-   0        0        0  1289541 2024-04-21 09:06:31.000000 textile_metric-0.0.8/textile/data/texture_368.jpg
--rw-rw-rw-   0        0        0     3195 2024-04-21 10:11:48.000000 textile_metric-0.0.8/textile/textile.py
-drwxrwxrwx   0        0        0        0 2024-04-21 10:11:52.159466 textile_metric-0.0.8/textile/utils/
--rw-rw-rw-   0        0        0        0 2024-04-20 10:01:22.000000 textile_metric-0.0.8/textile/utils/__init__.py
--rw-rw-rw-   0        0        0     1278 2024-04-20 10:44:38.000000 textile_metric-0.0.8/textile/utils/create_model.py
--rw-rw-rw-   0        0        0     1223 2024-04-20 10:17:53.000000 textile_metric-0.0.8/textile/utils/dataset.py
--rw-rw-rw-   0        0        0      296 2024-04-21 09:16:14.000000 textile_metric-0.0.8/textile/utils/image_utils.py
--rw-rw-rw-   0        0        0      454 2024-04-21 09:02:07.000000 textile_metric-0.0.8/textile/utils/misc.py
-drwxrwxrwx   0        0        0        0 2024-04-21 10:11:52.173054 textile_metric-0.0.8/textile_metric.egg-info/
--rw-rw-rw-   0        0        0     4104 2024-04-21 10:11:52.000000 textile_metric-0.0.8/textile_metric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      617 2024-04-21 10:11:52.000000 textile_metric-0.0.8/textile_metric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 10:11:52.000000 textile_metric-0.0.8/textile_metric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-04-21 10:11:52.000000 textile_metric-0.0.8/textile_metric.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-21 10:11:52.000000 textile_metric-0.0.8/textile_metric.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 10:20:07.127710 textile_metric-0.0.9/
+-rw-rw-rw-   0        0        0     1103 2024-04-20 09:48:15.000000 textile_metric-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4153 2024-04-21 10:20:07.126713 textile_metric-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3269 2024-04-21 10:16:44.000000 textile_metric-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-21 10:20:07.127710 textile_metric-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-04-21 10:20:04.000000 textile_metric-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:20:07.098927 textile_metric-0.0.9/textile/
+-rw-rw-rw-   0        0        0      311 2024-04-21 10:03:59.000000 textile_metric-0.0.9/textile/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:20:07.099928 textile_metric-0.0.9/textile/architectures/
+-rw-rw-rw-   0        0        0        0 2024-04-20 09:56:55.000000 textile_metric-0.0.9/textile/architectures/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:20:07.100928 textile_metric-0.0.9/textile/architectures/layers/
+-rw-rw-rw-   0        0        0        0 2024-04-20 09:57:58.000000 textile_metric-0.0.9/textile/architectures/layers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:20:07.101920 textile_metric-0.0.9/textile/architectures/layers/attention/
+-rw-rw-rw-   0        0        0        0 2024-04-20 09:58:11.000000 textile_metric-0.0.9/textile/architectures/layers/attention/__init__.py
+-rw-rw-rw-   0        0        0     1692 2024-04-20 10:44:38.000000 textile_metric-0.0.9/textile/architectures/layers/attention/attention.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:20:07.107560 textile_metric-0.0.9/textile/data/
+-rw-rw-rw-   0        0        0  4087314 2024-04-21 08:42:09.000000 textile_metric-0.0.9/textile/data/teaser.png
+-rw-rw-rw-   0        0        0  1289541 2024-04-21 09:06:31.000000 textile_metric-0.0.9/textile/data/texture_368.jpg
+-rw-rw-rw-   0        0        0     3313 2024-04-21 10:20:04.000000 textile_metric-0.0.9/textile/textile.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:20:07.112057 textile_metric-0.0.9/textile/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-20 10:01:22.000000 textile_metric-0.0.9/textile/utils/__init__.py
+-rw-rw-rw-   0        0        0     1278 2024-04-20 10:44:38.000000 textile_metric-0.0.9/textile/utils/create_model.py
+-rw-rw-rw-   0        0        0     1223 2024-04-20 10:17:53.000000 textile_metric-0.0.9/textile/utils/dataset.py
+-rw-rw-rw-   0        0        0      296 2024-04-21 09:16:14.000000 textile_metric-0.0.9/textile/utils/image_utils.py
+-rw-rw-rw-   0        0        0      454 2024-04-21 09:02:07.000000 textile_metric-0.0.9/textile/utils/misc.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:20:07.126713 textile_metric-0.0.9/textile_metric.egg-info/
+-rw-rw-rw-   0        0        0     4153 2024-04-21 10:20:06.000000 textile_metric-0.0.9/textile_metric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2024-04-21 10:20:07.000000 textile_metric-0.0.9/textile_metric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 10:20:06.000000 textile_metric-0.0.9/textile_metric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-04-21 10:20:06.000000 textile_metric-0.0.9/textile_metric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-21 10:20:06.000000 textile_metric-0.0.9/textile_metric.egg-info/top_level.txt
```

### Comparing `textile_metric-0.0.8/LICENSE` & `textile_metric-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.8/PKG-INFO` & `textile_metric-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textile-metric
-Version: 0.0.8
+Version: 0.0.9
 Summary: TexTile: A Differentiable Metric for Texture Tileability
 Home-page: https://github.com/crp94/textile
 Author: Carlos Rodriguez-Pardo
 Author-email: carlos.rodriguezpardo.jimenez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -25,16 +25,16 @@
 
 Official repository of "TexTile: A Differentiable Metric for Texture Tileability" [CVPR 2024]
 
 [Carlos Rodriguez-Pardo](https://carlosrodriguezpardo.es/), [Dan Casas](https://dancasas.github.io/), [Elena Garces](https://www.elenagarces.es/), [Jorge Lopez-Moreno](http://www.jorg3.com/)
 
 In [CVPR](https://arxiv.org/abs/2403.12961v1), 2024.
 
+![Textile-Teaser](https://raw.githubusercontent.com/crp94/textile/main/textile/data/teaser.png)
 
-<img src='textile/data/teaser.png' width=1200>
 
 We introduce TexTile, a novel differentiable metric to quantify the degree upon which a texture image can be concatenated with itself without introducing repeating artifacts (i.e., the tileability). Existing methods for tileable texture synthesis focus on general texture quality, but lack explicit analysis of the intrinsic repeatability properties of a texture. In contrast, our TexTile metric effectively evaluates the tileable properties of a texture, opening the door to more informed synthesis and analysis of tileable textures. Under the hood, TexTile is formulated as a binary classifier carefully built from a large dataset of textures of different styles, semantics, regularities, and human annotations. Key to our method is a set of architectural modifications to baseline pre-train image classifiers to overcome their shortcomings at measuring tileability, along with a custom data augmentation and training regime aimed at increasing robustness and accuracy. We demonstrate that TexTile can be plugged into different state-of-the-art texture synthesis methods, including diffusion-based strategies, and generate tileable textures while keeping or even improving the overall texture quality. Furthermore, we show that TexTile can objectively evaluate any tileable texture synthesis method, whereas the current mix of existing metrics produces uncorrelated scores which heavily hinders progress in the field.
 
 
 ### Quick start
 
 Run `pip install textile-metric`. The following Python code is all you need. Note that models are downloaded automatically.
```

### Comparing `textile_metric-0.0.8/README.md` & `textile_metric-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 Official repository of "TexTile: A Differentiable Metric for Texture Tileability" [CVPR 2024]
 
 [Carlos Rodriguez-Pardo](https://carlosrodriguezpardo.es/), [Dan Casas](https://dancasas.github.io/), [Elena Garces](https://www.elenagarces.es/), [Jorge Lopez-Moreno](http://www.jorg3.com/)
 
 In [CVPR](https://arxiv.org/abs/2403.12961v1), 2024.
 
+![Textile-Teaser](https://raw.githubusercontent.com/crp94/textile/main/textile/data/teaser.png)
 
-<img src='textile/data/teaser.png' width=1200>
 
 We introduce TexTile, a novel differentiable metric to quantify the degree upon which a texture image can be concatenated with itself without introducing repeating artifacts (i.e., the tileability). Existing methods for tileable texture synthesis focus on general texture quality, but lack explicit analysis of the intrinsic repeatability properties of a texture. In contrast, our TexTile metric effectively evaluates the tileable properties of a texture, opening the door to more informed synthesis and analysis of tileable textures. Under the hood, TexTile is formulated as a binary classifier carefully built from a large dataset of textures of different styles, semantics, regularities, and human annotations. Key to our method is a set of architectural modifications to baseline pre-train image classifiers to overcome their shortcomings at measuring tileability, along with a custom data augmentation and training regime aimed at increasing robustness and accuracy. We demonstrate that TexTile can be plugged into different state-of-the-art texture synthesis methods, including diffusion-based strategies, and generate tileable textures while keeping or even improving the overall texture quality. Furthermore, we show that TexTile can objectively evaluate any tileable texture synthesis method, whereas the current mix of existing metrics produces uncorrelated scores which heavily hinders progress in the field.
 
 
 ### Quick start
 
 Run `pip install textile-metric`. The following Python code is all you need. Note that models are downloaded automatically.
```

### Comparing `textile_metric-0.0.8/setup.py` & `textile_metric-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='textile-metric',
-     version='0.0.8',
+     version='0.0.9',
      author="Carlos Rodriguez-Pardo",
      author_email="carlos.rodriguezpardo.jimenez@gmail.com",
      description="TexTile: A Differentiable Metric for Texture Tileability",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/crp94/textile",
      packages=['textile'],
```

### Comparing `textile_metric-0.0.8/textile/architectures/layers/attention/attention.py` & `textile_metric-0.0.9/textile/architectures/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.8/textile/data/teaser.png` & `textile_metric-0.0.9/textile/data/teaser.png`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.8/textile/data/texture_368.jpg` & `textile_metric-0.0.9/textile/data/texture_368.jpg`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.8/textile/textile.py` & `textile_metric-0.0.9/textile/textile.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,17 @@
         assert lambda_value >= 0 and lambda_value <= 1
 
 
         is_model_on_disc = os.path.exists(model_path)
         if not is_model_on_disc:
             try:
                 import urllib.request
+                from pathlib import Path
                 print('Model not found, downloading pretrained model:')
+                Path("textile/models/").mkdir(parents=True, exist_ok=True)
                 urllib.request.urlretrieve("https://carlosrodriguezpardo.es/projects/TexTile/models/textile_v3.pth", model_path, MyProgressBar())
             except Exception as e:
                 print('Could not retrieve pretrained model')
                 raise e
 
         self.model = CreateModel(model_path).cuda().eval()
         self.lambda_value = torch.tensor(lambda_value)
```

### Comparing `textile_metric-0.0.8/textile/utils/create_model.py` & `textile_metric-0.0.9/textile/utils/create_model.py`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.8/textile/utils/dataset.py` & `textile_metric-0.0.9/textile/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `textile_metric-0.0.8/textile_metric.egg-info/PKG-INFO` & `textile_metric-0.0.9/textile_metric.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textile-metric
-Version: 0.0.8
+Version: 0.0.9
 Summary: TexTile: A Differentiable Metric for Texture Tileability
 Home-page: https://github.com/crp94/textile
 Author: Carlos Rodriguez-Pardo
 Author-email: carlos.rodriguezpardo.jimenez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -25,16 +25,16 @@
 
 Official repository of "TexTile: A Differentiable Metric for Texture Tileability" [CVPR 2024]
 
 [Carlos Rodriguez-Pardo](https://carlosrodriguezpardo.es/), [Dan Casas](https://dancasas.github.io/), [Elena Garces](https://www.elenagarces.es/), [Jorge Lopez-Moreno](http://www.jorg3.com/)
 
 In [CVPR](https://arxiv.org/abs/2403.12961v1), 2024.
 
+![Textile-Teaser](https://raw.githubusercontent.com/crp94/textile/main/textile/data/teaser.png)
 
-<img src='textile/data/teaser.png' width=1200>
 
 We introduce TexTile, a novel differentiable metric to quantify the degree upon which a texture image can be concatenated with itself without introducing repeating artifacts (i.e., the tileability). Existing methods for tileable texture synthesis focus on general texture quality, but lack explicit analysis of the intrinsic repeatability properties of a texture. In contrast, our TexTile metric effectively evaluates the tileable properties of a texture, opening the door to more informed synthesis and analysis of tileable textures. Under the hood, TexTile is formulated as a binary classifier carefully built from a large dataset of textures of different styles, semantics, regularities, and human annotations. Key to our method is a set of architectural modifications to baseline pre-train image classifiers to overcome their shortcomings at measuring tileability, along with a custom data augmentation and training regime aimed at increasing robustness and accuracy. We demonstrate that TexTile can be plugged into different state-of-the-art texture synthesis methods, including diffusion-based strategies, and generate tileable textures while keeping or even improving the overall texture quality. Furthermore, we show that TexTile can objectively evaluate any tileable texture synthesis method, whereas the current mix of existing metrics produces uncorrelated scores which heavily hinders progress in the field.
 
 
 ### Quick start
 
 Run `pip install textile-metric`. The following Python code is all you need. Note that models are downloaded automatically.
```

### Comparing `textile_metric-0.0.8/textile_metric.egg-info/SOURCES.txt` & `textile_metric-0.0.9/textile_metric.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/remote_sensing_analysis-0.1.0.tar.gz` & `tmp/remote_sensing_analysis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/remote_sensing_analysis-0.1.0.tar", last modified: Sun Apr 21 05:58:15 2024, max compression
+gzip compressed data, was "dist/remote_sensing_analysis-0.1.1.tar", last modified: Sun Apr 21 06:17:42 2024, max compression
```

## Comparing `remote_sensing_analysis-0.1.0.tar` & `remote_sensing_analysis-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 aidenchang   (501) staff       (20)        0 2024-04-21 05:58:15.198857 remote_sensing_analysis-0.1.0/
--rw-r--r--   0 aidenchang   (501) staff       (20)     1068 2024-04-21 05:23:11.000000 remote_sensing_analysis-0.1.0/LICENSE
--rw-r--r--   0 aidenchang   (501) staff       (20)      178 2024-04-21 05:48:25.000000 remote_sensing_analysis-0.1.0/MANIFEST.in
--rw-r--r--   0 aidenchang   (501) staff       (20)     3249 2024-04-21 05:58:15.198608 remote_sensing_analysis-0.1.0/PKG-INFO
--rw-r--r--   0 aidenchang   (501) staff       (20)     2638 2024-04-21 05:52:47.000000 remote_sensing_analysis-0.1.0/README.md
-drwxr-xr-x   0 aidenchang   (501) staff       (20)        0 2024-04-21 05:58:15.194787 remote_sensing_analysis-0.1.0/assets/
--rw-r--r--   0 aidenchang   (501) staff       (20)   672300 2024-04-21 05:23:11.000000 remote_sensing_analysis-0.1.0/assets/DejaVuSans-Bold.ttf
--rw-r--r--   0 aidenchang   (501) staff       (20)       38 2024-04-21 05:58:15.198906 remote_sensing_analysis-0.1.0/setup.cfg
--rw-r--r--   0 aidenchang   (501) staff       (20)      806 2024-04-21 05:30:58.000000 remote_sensing_analysis-0.1.0/setup.py
-drwxr-xr-x   0 aidenchang   (501) staff       (20)        0 2024-04-21 05:58:15.193798 remote_sensing_analysis-0.1.0/src/
-drwxr-xr-x   0 aidenchang   (501) staff       (20)        0 2024-04-21 05:58:15.197451 remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis/
--rw-r--r--   0 aidenchang   (501) staff       (20)     5268 2024-04-21 05:43:03.000000 remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis/ImageProcessor.py
--rw-r--r--   0 aidenchang   (501) staff       (20)     2796 2024-04-21 05:23:11.000000 remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis/ImageTextAnalytics.py
--rw-r--r--   0 aidenchang   (501) staff       (20)     4214 2024-04-21 05:23:11.000000 remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis/ImageToTextConverter.py
--rw-r--r--   0 aidenchang   (501) staff       (20)     2221 2024-04-21 05:41:52.000000 remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis/YOLOInference.py
--rw-r--r--   0 aidenchang   (501) staff       (20)       43 2024-04-21 05:37:06.000000 remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis/__init__.py
--rw-r--r--   0 aidenchang   (501) staff       (20)        0 2024-04-21 05:23:11.000000 remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis/enhance_imagery.py
-drwxr-xr-x   0 aidenchang   (501) staff       (20)        0 2024-04-21 05:58:15.198351 remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis.egg-info/
--rw-r--r--   0 aidenchang   (501) staff       (20)     3249 2024-04-21 05:58:15.000000 remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis.egg-info/PKG-INFO
--rw-r--r--   0 aidenchang   (501) staff       (20)      599 2024-04-21 05:58:15.000000 remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis.egg-info/SOURCES.txt
--rw-r--r--   0 aidenchang   (501) staff       (20)        1 2024-04-21 05:58:15.000000 remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis.egg-info/dependency_links.txt
--rw-r--r--   0 aidenchang   (501) staff       (20)      118 2024-04-21 05:58:15.000000 remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis.egg-info/requires.txt
--rw-r--r--   0 aidenchang   (501) staff       (20)       24 2024-04-21 05:58:15.000000 remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis.egg-info/top_level.txt
+drwxr-xr-x   0 aidenchang   (501) staff       (20)        0 2024-04-21 06:17:42.985562 remote_sensing_analysis-0.1.1/
+-rw-r--r--   0 aidenchang   (501) staff       (20)     1068 2024-04-21 05:23:11.000000 remote_sensing_analysis-0.1.1/LICENSE
+-rw-r--r--   0 aidenchang   (501) staff       (20)      178 2024-04-21 05:48:25.000000 remote_sensing_analysis-0.1.1/MANIFEST.in
+-rw-r--r--   0 aidenchang   (501) staff       (20)     2997 2024-04-21 06:17:42.985318 remote_sensing_analysis-0.1.1/PKG-INFO
+-rw-r--r--   0 aidenchang   (501) staff       (20)     2386 2024-04-21 06:15:07.000000 remote_sensing_analysis-0.1.1/README.md
+drwxr-xr-x   0 aidenchang   (501) staff       (20)        0 2024-04-21 06:17:42.980638 remote_sensing_analysis-0.1.1/assets/
+-rw-r--r--   0 aidenchang   (501) staff       (20)   672300 2024-04-21 05:23:11.000000 remote_sensing_analysis-0.1.1/assets/DejaVuSans-Bold.ttf
+-rw-r--r--   0 aidenchang   (501) staff       (20)       38 2024-04-21 06:17:42.985615 remote_sensing_analysis-0.1.1/setup.cfg
+-rw-r--r--   0 aidenchang   (501) staff       (20)      806 2024-04-21 06:16:37.000000 remote_sensing_analysis-0.1.1/setup.py
+drwxr-xr-x   0 aidenchang   (501) staff       (20)        0 2024-04-21 06:17:42.979570 remote_sensing_analysis-0.1.1/src/
+drwxr-xr-x   0 aidenchang   (501) staff       (20)        0 2024-04-21 06:17:42.983907 remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis/
+-rw-r--r--   0 aidenchang   (501) staff       (20)     5268 2024-04-21 05:43:03.000000 remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis/ImageProcessor.py
+-rw-r--r--   0 aidenchang   (501) staff       (20)     2796 2024-04-21 05:23:11.000000 remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis/ImageTextAnalytics.py
+-rw-r--r--   0 aidenchang   (501) staff       (20)     4214 2024-04-21 05:23:11.000000 remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis/ImageToTextConverter.py
+-rw-r--r--   0 aidenchang   (501) staff       (20)     2221 2024-04-21 05:41:52.000000 remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis/YOLOInference.py
+-rw-r--r--   0 aidenchang   (501) staff       (20)       43 2024-04-21 05:37:06.000000 remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis/__init__.py
+-rw-r--r--   0 aidenchang   (501) staff       (20)        0 2024-04-21 05:23:11.000000 remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis/enhance_imagery.py
+drwxr-xr-x   0 aidenchang   (501) staff       (20)        0 2024-04-21 06:17:42.985010 remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis.egg-info/
+-rw-r--r--   0 aidenchang   (501) staff       (20)     2997 2024-04-21 06:17:42.000000 remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis.egg-info/PKG-INFO
+-rw-r--r--   0 aidenchang   (501) staff       (20)      599 2024-04-21 06:17:42.000000 remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 aidenchang   (501) staff       (20)        1 2024-04-21 06:17:42.000000 remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 aidenchang   (501) staff       (20)      118 2024-04-21 06:17:42.000000 remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis.egg-info/requires.txt
+-rw-r--r--   0 aidenchang   (501) staff       (20)       24 2024-04-21 06:17:42.000000 remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis.egg-info/top_level.txt
```

### Comparing `remote_sensing_analysis-0.1.0/LICENSE` & `remote_sensing_analysis-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `remote_sensing_analysis-0.1.0/PKG-INFO` & `remote_sensing_analysis-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Remote_Sensing_Analysis
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library that conducts analysis on Satellite Imagery
 Home-page: http://github.com/aiden200/Remote_Sensing_Analysis
 Author: Aiden Chang
 Author-email: aidenchang@gmail.com
 License: MIT
 Keywords: Machine-Learning Remote-Sensing Object-detection
 Requires-Python: >=3.9
@@ -19,31 +19,23 @@
 
 # Remote Sensing Analysis
 
 This package provides tools for processing and analyzing satellite imagery, utilizing advanced machine learning techniques for object detection, image enhancement, and text analytics from images.
 
 ## Installation
 
-To install the Remote Sensing Analysis package, follow these steps:
+1. **Download Package**:
 
-1. **Clone the Repository**:
+To install the Remote Sensing Analysis package, simply run the following command:
 
-   ```bash
-   git clone https://github.com/aiden200/Remote_Sensing_Analysis.git
-   cd Remote_Sensing_Analysis
-   ```
+```bash
+pip install Remote-Sensing-Analysis
+```
 
-2. **Install the Package**:
-   Use pip to install the package in editable mode, which is particularly useful for making changes to the code and testing.
-
-   ```bash
-   pip install -e .
-   ```
-
-3. **Download Model Weights**:
+2. **Download Model Weights**:
    The package requires specific model weights to function correctly. Download the model weights from the following Google Drive link:
    [Download Model Weights](https://drive.google.com/file/d/1KL3H-Fe1SVoCEFaO4KM4J_FMRF4ocoCz/view?usp=sharing)
 
    After downloading, place the weights under the `pretrained` folder.
 
 ## Usage
```

### Comparing `remote_sensing_analysis-0.1.0/README.md` & `remote_sensing_analysis-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 # Remote Sensing Analysis
 
 This package provides tools for processing and analyzing satellite imagery, utilizing advanced machine learning techniques for object detection, image enhancement, and text analytics from images.
 
 ## Installation
 
-To install the Remote Sensing Analysis package, follow these steps:
+1. **Download Package**:
 
-1. **Clone the Repository**:
+To install the Remote Sensing Analysis package, simply run the following command:
 
-   ```bash
-   git clone https://github.com/aiden200/Remote_Sensing_Analysis.git
-   cd Remote_Sensing_Analysis
-   ```
+```bash
+pip install Remote-Sensing-Analysis
+```
 
-2. **Install the Package**:
-   Use pip to install the package in editable mode, which is particularly useful for making changes to the code and testing.
-
-   ```bash
-   pip install -e .
-   ```
-
-3. **Download Model Weights**:
+2. **Download Model Weights**:
    The package requires specific model weights to function correctly. Download the model weights from the following Google Drive link:
    [Download Model Weights](https://drive.google.com/file/d/1KL3H-Fe1SVoCEFaO4KM4J_FMRF4ocoCz/view?usp=sharing)
 
    After downloading, place the weights under the `pretrained` folder.
 
 ## Usage
```

### Comparing `remote_sensing_analysis-0.1.0/assets/DejaVuSans-Bold.ttf` & `remote_sensing_analysis-0.1.1/assets/DejaVuSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `remote_sensing_analysis-0.1.0/setup.py` & `remote_sensing_analysis-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Remote_Sensing_Analysis',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         'pillow==10.3.0',
         'ultralytics==8.2.2',
         'transformers==4.40.0',
         'sentence_transformers==2.7.0',
```

### Comparing `remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis/ImageProcessor.py` & `remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis/ImageProcessor.py`

 * *Files identical despite different names*

### Comparing `remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis/ImageTextAnalytics.py` & `remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis/ImageTextAnalytics.py`

 * *Files identical despite different names*

### Comparing `remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis/ImageToTextConverter.py` & `remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis/ImageToTextConverter.py`

 * *Files identical despite different names*

### Comparing `remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis/YOLOInference.py` & `remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis/YOLOInference.py`

 * *Files identical despite different names*

### Comparing `remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis.egg-info/PKG-INFO` & `remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Remote_Sensing_Analysis
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library that conducts analysis on Satellite Imagery
 Home-page: http://github.com/aiden200/Remote_Sensing_Analysis
 Author: Aiden Chang
 Author-email: aidenchang@gmail.com
 License: MIT
 Keywords: Machine-Learning Remote-Sensing Object-detection
 Requires-Python: >=3.9
@@ -19,31 +19,23 @@
 
 # Remote Sensing Analysis
 
 This package provides tools for processing and analyzing satellite imagery, utilizing advanced machine learning techniques for object detection, image enhancement, and text analytics from images.
 
 ## Installation
 
-To install the Remote Sensing Analysis package, follow these steps:
+1. **Download Package**:
 
-1. **Clone the Repository**:
+To install the Remote Sensing Analysis package, simply run the following command:
 
-   ```bash
-   git clone https://github.com/aiden200/Remote_Sensing_Analysis.git
-   cd Remote_Sensing_Analysis
-   ```
+```bash
+pip install Remote-Sensing-Analysis
+```
 
-2. **Install the Package**:
-   Use pip to install the package in editable mode, which is particularly useful for making changes to the code and testing.
-
-   ```bash
-   pip install -e .
-   ```
-
-3. **Download Model Weights**:
+2. **Download Model Weights**:
    The package requires specific model weights to function correctly. Download the model weights from the following Google Drive link:
    [Download Model Weights](https://drive.google.com/file/d/1KL3H-Fe1SVoCEFaO4KM4J_FMRF4ocoCz/view?usp=sharing)
 
    After downloading, place the weights under the `pretrained` folder.
 
 ## Usage
```

### Comparing `remote_sensing_analysis-0.1.0/src/Remote_Sensing_Analysis.egg-info/SOURCES.txt` & `remote_sensing_analysis-0.1.1/src/Remote_Sensing_Analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*


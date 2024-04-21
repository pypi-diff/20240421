# Comparing `tmp/emgflow-1.0.8.tar.gz` & `tmp/emgflow-1.0.9.tar.gz`

## Comparing `emgflow-1.0.8.tar` & `emgflow-1.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6070 2020-02-02 00:00:00.000000 emgflow-1.0.8/src/EMGFlow/OutlierFinder.py
--rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 emgflow-1.0.8/src/EMGFlow/PlotSignals.py
--rw-r--r--   0        0        0    49356 2020-02-02 00:00:00.000000 emgflow-1.0.8/src/EMGFlow/SignalFilterer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 emgflow-1.0.8/src/EMGFlow/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 emgflow-1.0.8/.gitignore
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 emgflow-1.0.8/README.md
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 emgflow-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 emgflow-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6070 2020-02-02 00:00:00.000000 emgflow-1.0.9/src/EMGFlow/OutlierFinder.py
+-rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 emgflow-1.0.9/src/EMGFlow/PlotSignals.py
+-rw-r--r--   0        0        0    49356 2020-02-02 00:00:00.000000 emgflow-1.0.9/src/EMGFlow/SignalFilterer.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 emgflow-1.0.9/src/EMGFlow/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 emgflow-1.0.9/.gitignore
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 emgflow-1.0.9/README.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 emgflow-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 emgflow-1.0.9/PKG-INFO
```

### Comparing `emgflow-1.0.8/src/EMGFlow/OutlierFinder.py` & `emgflow-1.0.9/src/EMGFlow/OutlierFinder.py`

 * *Files identical despite different names*

### Comparing `emgflow-1.0.8/src/EMGFlow/PlotSignals.py` & `emgflow-1.0.9/src/EMGFlow/PlotSignals.py`

 * *Files identical despite different names*

### Comparing `emgflow-1.0.8/src/EMGFlow/SignalFilterer.py` & `emgflow-1.0.9/src/EMGFlow/SignalFilterer.py`

 * *Files identical despite different names*

### Comparing `emgflow-1.0.8/README.md` & `emgflow-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -73,11 +73,11 @@
 
 ```bibtex
 @software{Conley_EMGFlow_2024,
   author = {Conley {\tt william@cconley.ca}, William and Livingstone, Steven R},
   month = {03},
   title = {{EMGFlow Package}},
   url = {https://github.com/WiIIson/EMGFlow-Python-Package},
-  version = {1.0.8},
+  version = {1.0.9},
   year = {2024}
 }
 ```
```

### Comparing `emgflow-1.0.8/pyproject.toml` & `emgflow-1.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EMGFlow"
-version = "1.0.8"
+version = "1.0.9"
 dependencies = [
     "pandas",
     "numpy",
     "scipy",
     "matplotlib",
     "opencv-python", 
     "tqdm",
-    "webbrowser",
     "shiny",
 ]
 requires-python = ">=3.8"
 authors = [
     {name = "William Conley and Steven Livingstone", email = "william@cconley.ca"}
 ]
 description = "A general EMG processing and feature extraction package."
```

### Comparing `emgflow-1.0.8/PKG-INFO` & `emgflow-1.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.3
 Name: EMGFlow
-Version: 1.0.8
+Version: 1.0.9
 Summary: A general EMG processing and feature extraction package.
 Project-URL: Home, https://github.com/WiIIson/EMGFlow-Python-Package
 Author-email: William Conley and Steven Livingstone <william@cconley.ca>
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: opencv-python
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: shiny
 Requires-Dist: tqdm
-Requires-Dist: webbrowser
 Description-Content-Type: text/markdown
 
 <img src="https://raw.githubusercontent.com/WiIIson/EMGFlow-Python-Package/main/HexSticker.png"  width="100" height="110" style="float: right;">
 
 # EMGFlow
 
 The open workflow for EMG signal processing and feature extraction.
@@ -93,11 +92,11 @@
 
 ```bibtex
 @software{Conley_EMGFlow_2024,
   author = {Conley {\tt william@cconley.ca}, William and Livingstone, Steven R},
   month = {03},
   title = {{EMGFlow Package}},
   url = {https://github.com/WiIIson/EMGFlow-Python-Package},
-  version = {1.0.8},
+  version = {1.0.9},
   year = {2024}
 }
 ```
```


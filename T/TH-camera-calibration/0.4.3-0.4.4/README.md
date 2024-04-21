# Comparing `tmp/TH_camera_calibration-0.4.3.tar.gz` & `tmp/TH_camera_calibration-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TH_camera_calibration-0.4.3.tar", last modified: Sun Apr 21 06:56:47 2024, max compression
+gzip compressed data, was "TH_camera_calibration-0.4.4.tar", last modified: Sun Apr 21 07:06:38 2024, max compression
```

## Comparing `TH_camera_calibration-0.4.3.tar` & `TH_camera_calibration-0.4.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 06:56:47.719071 TH_camera_calibration-0.4.3/
--rw-rw-rw-   0        0        0     2612 2024-04-21 06:56:47.717072 TH_camera_calibration-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     5004 2024-04-21 06:01:28.000000 TH_camera_calibration-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 06:56:47.702024 TH_camera_calibration-0.4.3/TH_camera_calibration/
--rw-rw-rw-   0        0        0       51 2024-04-21 06:12:27.000000 TH_camera_calibration-0.4.3/TH_camera_calibration/__init__.py
--rw-rw-rw-   0        0        0    13214 2024-04-21 05:58:38.000000 TH_camera_calibration-0.4.3/TH_camera_calibration/camera_calibration.py
-drwxrwxrwx   0        0        0        0 2024-04-21 06:56:47.715070 TH_camera_calibration-0.4.3/TH_camera_calibration.egg-info/
--rw-rw-rw-   0        0        0     2612 2024-04-21 06:56:47.000000 TH_camera_calibration-0.4.3/TH_camera_calibration.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-04-21 06:56:47.000000 TH_camera_calibration-0.4.3/TH_camera_calibration.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 06:56:47.000000 TH_camera_calibration-0.4.3/TH_camera_calibration.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-04-21 06:56:47.000000 TH_camera_calibration-0.4.3/TH_camera_calibration.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-21 06:56:47.000000 TH_camera_calibration-0.4.3/TH_camera_calibration.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 06:56:47.719071 TH_camera_calibration-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      481 2024-04-21 06:56:40.000000 TH_camera_calibration-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 07:06:38.707107 TH_camera_calibration-0.4.4/
+-rw-rw-rw-   0        0        0     2729 2024-04-21 07:06:38.705108 TH_camera_calibration-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5238 2024-04-21 07:06:15.000000 TH_camera_calibration-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 07:06:38.675935 TH_camera_calibration-0.4.4/TH_camera_calibration/
+-rw-rw-rw-   0        0        0       51 2024-04-21 06:12:27.000000 TH_camera_calibration-0.4.4/TH_camera_calibration/__init__.py
+-rw-rw-rw-   0        0        0    13214 2024-04-21 05:58:38.000000 TH_camera_calibration-0.4.4/TH_camera_calibration/camera_calibration.py
+drwxrwxrwx   0        0        0        0 2024-04-21 07:06:38.702110 TH_camera_calibration-0.4.4/TH_camera_calibration.egg-info/
+-rw-rw-rw-   0        0        0     2729 2024-04-21 07:06:38.000000 TH_camera_calibration-0.4.4/TH_camera_calibration.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-04-21 07:06:38.000000 TH_camera_calibration-0.4.4/TH_camera_calibration.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 07:06:38.000000 TH_camera_calibration-0.4.4/TH_camera_calibration.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2024-04-21 07:06:38.000000 TH_camera_calibration-0.4.4/TH_camera_calibration.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-21 07:06:38.000000 TH_camera_calibration-0.4.4/TH_camera_calibration.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 07:06:38.707107 TH_camera_calibration-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      481 2024-04-21 07:06:21.000000 TH_camera_calibration-0.4.4/setup.py
```

### Comparing `TH_camera_calibration-0.4.3/PKG-INFO` & `TH_camera_calibration-0.4.4/TH_camera_calibration.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: TH_camera_calibration
-Version: 0.4.3
+Name: TH-camera-calibration
+Version: 0.4.4
 Description-Content-Type: text/markdown
 
 # Calibration_camera
 
 Created on Sunday, April 21, 2024  
 Author: Tung Nguyen - Handsome  
 Reference: Camera Calibration by OpenCV ([OpenCV Tutorial](https://docs.opencv.org/4.x/dc/dbb/tutorial_py_calibration.html))
@@ -19,14 +19,20 @@
 
 - Calculate camera calibration data based on a set of images.
 - Save and load the camera calibration data.
 - Undistort images or points using the calibration data.
 
 ## Usage
 
+Using this command for install package (or clone this repository):
+
+```
+pip install TH-camera-calibration
+```
+
 ### Requirements
 
 - Python 3.x
 - OpenCV
 - Numpy
 - PyYAML (For working with YAML files)
   To set up the environment, install all the required libraries by using this command:
```

### Comparing `TH_camera_calibration-0.4.3/README.md` & `TH_camera_calibration-0.4.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 
 - Calculate camera calibration data based on a set of images.
 - Save and load the camera calibration data.
 - Undistort images or points using the calibration data.
 
 ## Usage
 
+Using this command for install package (or clone this repository):
+
+```
+pip install TH-camera-calibration
+```
+
 ### Requirements
 
 - Python 3.x
 - OpenCV
 - Numpy
 - PyYAML (For working with YAML files)
   To set up the environment, install all the required libraries by using this command:
```

### Comparing `TH_camera_calibration-0.4.3/TH_camera_calibration/camera_calibration.py` & `TH_camera_calibration-0.4.4/TH_camera_calibration/camera_calibration.py`

 * *Files identical despite different names*

### Comparing `TH_camera_calibration-0.4.3/TH_camera_calibration.egg-info/PKG-INFO` & `TH_camera_calibration-0.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: TH-camera-calibration
-Version: 0.4.3
+Name: TH_camera_calibration
+Version: 0.4.4
 Description-Content-Type: text/markdown
 
 # Calibration_camera
 
 Created on Sunday, April 21, 2024  
 Author: Tung Nguyen - Handsome  
 Reference: Camera Calibration by OpenCV ([OpenCV Tutorial](https://docs.opencv.org/4.x/dc/dbb/tutorial_py_calibration.html))
@@ -19,14 +19,20 @@
 
 - Calculate camera calibration data based on a set of images.
 - Save and load the camera calibration data.
 - Undistort images or points using the calibration data.
 
 ## Usage
 
+Using this command for install package (or clone this repository):
+
+```
+pip install TH-camera-calibration
+```
+
 ### Requirements
 
 - Python 3.x
 - OpenCV
 - Numpy
 - PyYAML (For working with YAML files)
   To set up the environment, install all the required libraries by using this command:
```


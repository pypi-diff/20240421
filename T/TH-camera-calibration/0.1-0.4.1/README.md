# Comparing `tmp/TH_camera_calibration-0.1.tar.gz` & `tmp/TH_camera_calibration-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TH_camera_calibration-0.1.tar", last modified: Sun Apr 21 06:18:45 2024, max compression
+gzip compressed data, was "TH_camera_calibration-0.4.1.tar", last modified: Sun Apr 21 06:49:59 2024, max compression
```

## Comparing `TH_camera_calibration-0.1.tar` & `TH_camera_calibration-0.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 06:18:45.235306 TH_camera_calibration-0.1/
--rw-rw-rw-   0        0        0       66 2024-04-21 06:18:45.233223 TH_camera_calibration-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5004 2024-04-21 06:01:28.000000 TH_camera_calibration-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 06:18:45.210588 TH_camera_calibration-0.1/TH_camera_calibration/
--rw-rw-rw-   0        0        0       51 2024-04-21 06:12:27.000000 TH_camera_calibration-0.1/TH_camera_calibration/__init__.py
--rw-rw-rw-   0        0        0    13214 2024-04-21 05:58:38.000000 TH_camera_calibration-0.1/TH_camera_calibration/camera_calibration.py
-drwxrwxrwx   0        0        0        0 2024-04-21 06:18:45.230228 TH_camera_calibration-0.1/TH_camera_calibration.egg-info/
--rw-rw-rw-   0        0        0       66 2024-04-21 06:18:44.000000 TH_camera_calibration-0.1/TH_camera_calibration.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-04-21 06:18:45.000000 TH_camera_calibration-0.1/TH_camera_calibration.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 06:18:44.000000 TH_camera_calibration-0.1/TH_camera_calibration.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-04-21 06:18:44.000000 TH_camera_calibration-0.1/TH_camera_calibration.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-21 06:18:44.000000 TH_camera_calibration-0.1/TH_camera_calibration.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 06:18:45.235459 TH_camera_calibration-0.1/setup.cfg
--rw-rw-rw-   0        0        0      308 2024-04-21 06:18:16.000000 TH_camera_calibration-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:49:59.420249 TH_camera_calibration-0.4.1/
+-rw-rw-rw-   0        0        0     5315 2024-04-21 06:49:59.420249 TH_camera_calibration-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5004 2024-04-21 06:01:28.000000 TH_camera_calibration-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 06:49:59.404373 TH_camera_calibration-0.4.1/TH_camera_calibration/
+-rw-rw-rw-   0        0        0       51 2024-04-21 06:12:27.000000 TH_camera_calibration-0.4.1/TH_camera_calibration/__init__.py
+-rw-rw-rw-   0        0        0    13214 2024-04-21 05:58:38.000000 TH_camera_calibration-0.4.1/TH_camera_calibration/camera_calibration.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:49:59.420249 TH_camera_calibration-0.4.1/TH_camera_calibration.egg-info/
+-rw-rw-rw-   0        0        0     5315 2024-04-21 06:49:59.000000 TH_camera_calibration-0.4.1/TH_camera_calibration.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-04-21 06:49:59.000000 TH_camera_calibration-0.4.1/TH_camera_calibration.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 06:49:59.000000 TH_camera_calibration-0.4.1/TH_camera_calibration.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2024-04-21 06:49:59.000000 TH_camera_calibration-0.4.1/TH_camera_calibration.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-21 06:49:59.000000 TH_camera_calibration-0.4.1/TH_camera_calibration.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 06:49:59.420249 TH_camera_calibration-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      462 2024-04-21 06:49:46.000000 TH_camera_calibration-0.4.1/setup.py
```

### Comparing `TH_camera_calibration-0.1/README.md` & `TH_camera_calibration-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `TH_camera_calibration-0.1/TH_camera_calibration/camera_calibration.py` & `TH_camera_calibration-0.4.1/TH_camera_calibration/camera_calibration.py`

 * *Files identical despite different names*


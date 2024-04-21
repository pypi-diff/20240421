# Comparing `tmp/dem_roughness_calculator-1.0.0.tar.gz` & `tmp/dem_roughness_calculator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dem_roughness_calculator-1.0.0.tar", last modified: Sun Apr 21 16:37:03 2024, max compression
+gzip compressed data, was "dem_roughness_calculator-1.0.3.tar", last modified: Sun Apr 21 19:28:50 2024, max compression
```

## Comparing `dem_roughness_calculator-1.0.0.tar` & `dem_roughness_calculator-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:37:03.937521 dem_roughness_calculator-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 16:36:52.000000 dem_roughness_calculator-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-21 16:37:03.937521 dem_roughness_calculator-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-21 16:36:52.000000 dem_roughness_calculator-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:37:03.937521 dem_roughness_calculator-1.0.0/dem_roughness_calculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-21 16:37:03.000000 dem_roughness_calculator-1.0.0/dem_roughness_calculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-21 16:37:03.000000 dem_roughness_calculator-1.0.0/dem_roughness_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 16:37:03.000000 dem_roughness_calculator-1.0.0/dem_roughness_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-21 16:37:03.000000 dem_roughness_calculator-1.0.0/dem_roughness_calculator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:37:03.937521 dem_roughness_calculator-1.0.0/roughness_calculator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 16:36:52.000000 dem_roughness_calculator-1.0.0/roughness_calculator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:37:03.937521 dem_roughness_calculator-1.0.0/roughness_calculator/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 16:36:52.000000 dem_roughness_calculator-1.0.0/roughness_calculator/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13925 2024-04-21 16:36:52.000000 dem_roughness_calculator-1.0.0/roughness_calculator/classes/application_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    24761 2024-04-21 16:36:52.000000 dem_roughness_calculator-1.0.0/roughness_calculator/classes/geo_tiff_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-21 16:36:52.000000 dem_roughness_calculator-1.0.0/roughness_calculator/cli_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    18854 2024-04-21 16:36:52.000000 dem_roughness_calculator-1.0.0/roughness_calculator/gui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-21 16:36:52.000000 dem_roughness_calculator-1.0.0/roughness_calculator/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 16:37:03.937521 dem_roughness_calculator-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-21 16:36:52.000000 dem_roughness_calculator-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:37:03.937521 dem_roughness_calculator-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 16:36:52.000000 dem_roughness_calculator-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-21 16:36:52.000000 dem_roughness_calculator-1.0.0/tests/test_application_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:28:50.371871 dem_roughness_calculator-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 19:28:36.000000 dem_roughness_calculator-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-21 19:28:50.371871 dem_roughness_calculator-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-21 19:28:36.000000 dem_roughness_calculator-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:28:50.371871 dem_roughness_calculator-1.0.3/dem_roughness_calculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-21 19:28:50.000000 dem_roughness_calculator-1.0.3/dem_roughness_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-21 19:28:50.000000 dem_roughness_calculator-1.0.3/dem_roughness_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:28:50.000000 dem_roughness_calculator-1.0.3/dem_roughness_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-21 19:28:50.000000 dem_roughness_calculator-1.0.3/dem_roughness_calculator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-21 19:28:50.000000 dem_roughness_calculator-1.0.3/dem_roughness_calculator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-21 19:28:50.000000 dem_roughness_calculator-1.0.3/dem_roughness_calculator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:28:50.371871 dem_roughness_calculator-1.0.3/roughness_calculator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:28:36.000000 dem_roughness_calculator-1.0.3/roughness_calculator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:28:50.371871 dem_roughness_calculator-1.0.3/roughness_calculator/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:28:36.000000 dem_roughness_calculator-1.0.3/roughness_calculator/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13925 2024-04-21 19:28:36.000000 dem_roughness_calculator-1.0.3/roughness_calculator/classes/application_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24761 2024-04-21 19:28:36.000000 dem_roughness_calculator-1.0.3/roughness_calculator/classes/geo_tiff_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-21 19:28:36.000000 dem_roughness_calculator-1.0.3/roughness_calculator/cli_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18854 2024-04-21 19:28:36.000000 dem_roughness_calculator-1.0.3/roughness_calculator/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-21 19:28:36.000000 dem_roughness_calculator-1.0.3/roughness_calculator/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:28:50.371871 dem_roughness_calculator-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-21 19:28:36.000000 dem_roughness_calculator-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:28:50.371871 dem_roughness_calculator-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:28:36.000000 dem_roughness_calculator-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-21 19:28:36.000000 dem_roughness_calculator-1.0.3/tests/test_application_driver.py
```

### Comparing `dem_roughness_calculator-1.0.0/LICENSE` & `dem_roughness_calculator-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.0.0/README.md` & `dem_roughness_calculator-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.0.0/dem_roughness_calculator.egg-info/SOURCES.txt` & `dem_roughness_calculator-1.0.3/dem_roughness_calculator.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE
 README.md
 setup.py
 dem_roughness_calculator.egg-info/PKG-INFO
 dem_roughness_calculator.egg-info/SOURCES.txt
 dem_roughness_calculator.egg-info/dependency_links.txt
+dem_roughness_calculator.egg-info/entry_points.txt
+dem_roughness_calculator.egg-info/requires.txt
 dem_roughness_calculator.egg-info/top_level.txt
 roughness_calculator/__init__.py
 roughness_calculator/cli_main.py
 roughness_calculator/gui_main.py
 roughness_calculator/log_config.py
 roughness_calculator/classes/__init__.py
 roughness_calculator/classes/application_driver.py
```

### Comparing `dem_roughness_calculator-1.0.0/roughness_calculator/classes/application_driver.py` & `dem_roughness_calculator-1.0.3/roughness_calculator/classes/application_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 application_driver.py
 ---------------------
-Version: 1.0.2
+Version: 1.0.3
 Author: Lukas Batschelet
 Date: 21.04.2024
 ---------------------
 This module contains the ApplicationDriver class which is responsible for running the application.
 It acts as a sort of interface between the calling User Interface (UI) and the GeoTIFFProcessor class.
 This enables the separation of concerns and allows for easier testing and maintenance of the code.
 (i.e. the UI does not need to know how the processing is done, it just needs to know how to call the processing.)
```

### Comparing `dem_roughness_calculator-1.0.0/roughness_calculator/classes/geo_tiff_processor.py` & `dem_roughness_calculator-1.0.3/roughness_calculator/classes/geo_tiff_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 geo_tiff_processor.py
 ---------------------
-Version: 1.0.2
+Version: 1.0.3
 Author: Lukas Batschelet
 Date: 21.04.2024
 ---------------------
 This module contains the GeoTIFFProcessor class which is responsible for processing GeoTIFF files.
 It provides methods for loading, processing, and saving GeoTIFF files.
 Until now, only a method to calculate the roughness of a GeoTIFF file has been implemented.
 """
```

### Comparing `dem_roughness_calculator-1.0.0/roughness_calculator/cli_main.py` & `dem_roughness_calculator-1.0.3/roughness_calculator/cli_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 cli_main.py
 -----------
-Version: 1.0.2
+Version: 1.0.3
 Author: Lukas Batschelet
 Date: 21.04.2024
 -----------
 """
 import argparse
 from roughness_calculator.classes.application_driver import ApplicationDriver
 import logging
```

### Comparing `dem_roughness_calculator-1.0.0/roughness_calculator/gui_main.py` & `dem_roughness_calculator-1.0.3/roughness_calculator/gui_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 gui_main.py
 -----------
-Version: 1.0.2
+Version: 1.0.3
 Author: Lukas Batschelet
 Date: 21.04.2024
 -----------
 This module contains the ApplicationGUI class which is
 responsible for creating the graphical user interface (GUI) of the application.
 """
 from PIL import Image, ImageTk
```

### Comparing `dem_roughness_calculator-1.0.0/roughness_calculator/log_config.py` & `dem_roughness_calculator-1.0.3/roughness_calculator/log_config.py`

 * *Files identical despite different names*


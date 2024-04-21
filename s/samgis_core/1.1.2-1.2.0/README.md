# Comparing `tmp/samgis_core-1.1.2.tar.gz` & `tmp/samgis_core-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samgis_core-1.1.2.tar", max compression
+gzip compressed data, was "samgis_core-1.2.0.tar", max compression
```

## Comparing `samgis_core-1.1.2.tar` & `samgis_core-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      262 2024-01-27 16:18:49.002975 samgis_core-1.1.2/README.md
--rw-r--r--   0        0        0      632 2024-04-16 19:06:29.883454 samgis_core-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      351 2024-01-31 18:31:46.678851 samgis_core-1.1.2/samgis_core/__init__.py
--rw-r--r--   0        0        0       94 2024-04-15 09:18:13.959941 samgis_core-1.1.2/samgis_core/__version__.py
--rw-r--r--   0        0        0       57 2024-01-26 19:56:25.000000 samgis_core-1.1.2/samgis_core/prediction_api/__init__.py
--rw-r--r--   0        0        0    15320 2024-04-16 18:51:41.442736 samgis_core-1.1.2/samgis_core/prediction_api/sam_onnx.py
--rw-r--r--   0        0        0       32 2024-01-26 19:56:25.000000 samgis_core-1.1.2/samgis_core/utilities/__init__.py
--rw-r--r--   0        0        0      157 2024-01-27 14:15:17.000000 samgis_core-1.1.2/samgis_core/utilities/constants.py
--rw-r--r--   0        0        0      650 2024-04-15 21:25:49.690475 samgis_core-1.1.2/samgis_core/utilities/fastapi_logger.py
--rw-r--r--   0        0        0     2689 2024-04-16 18:49:10.489577 samgis_core-1.1.2/samgis_core/utilities/serialize.py
--rw-r--r--   0        0        0      845 2024-04-16 18:51:41.468695 samgis_core-1.1.2/samgis_core/utilities/type_hints.py
--rw-r--r--   0        0        0     2434 2024-01-27 14:15:17.000000 samgis_core-1.1.2/samgis_core/utilities/utilities.py
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 samgis_core-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      262 2024-01-27 16:18:49.002975 samgis_core-1.2.0/README.md
+-rw-r--r--   0        0        0      786 2024-04-21 19:58:55.703678 samgis_core-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      351 2024-01-31 18:31:46.678851 samgis_core-1.2.0/samgis_core/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-21 19:58:55.709199 samgis_core-1.2.0/samgis_core/__version__.py
+-rw-r--r--   0        0        0       57 2024-01-26 19:56:25.000000 samgis_core-1.2.0/samgis_core/prediction_api/__init__.py
+-rw-r--r--   0        0        0    15320 2024-04-21 19:58:55.714518 samgis_core-1.2.0/samgis_core/prediction_api/sam_onnx.py
+-rw-r--r--   0        0        0       32 2024-01-26 19:56:25.000000 samgis_core-1.2.0/samgis_core/utilities/__init__.py
+-rw-r--r--   0        0        0      157 2024-01-27 14:15:17.000000 samgis_core-1.2.0/samgis_core/utilities/constants.py
+-rw-r--r--   0        0        0      650 2024-04-21 19:58:55.718527 samgis_core-1.2.0/samgis_core/utilities/fastapi_logger.py
+-rw-r--r--   0        0        0     2689 2024-04-21 19:58:55.721439 samgis_core-1.2.0/samgis_core/utilities/serialize.py
+-rw-r--r--   0        0        0      845 2024-04-21 19:58:55.725860 samgis_core-1.2.0/samgis_core/utilities/type_hints.py
+-rw-r--r--   0        0        0     2434 2024-01-27 14:15:17.000000 samgis_core-1.2.0/samgis_core/utilities/utilities.py
+-rw-r--r--   0        0        0     1088 1970-01-01 00:00:00.000000 samgis_core-1.2.0/PKG-INFO
```

### Comparing `samgis_core-1.1.2/samgis_core/prediction_api/sam_onnx.py` & `samgis_core-1.2.0/samgis_core/prediction_api/sam_onnx.py`

 * *Files identical despite different names*

### Comparing `samgis_core-1.1.2/samgis_core/utilities/fastapi_logger.py` & `samgis_core-1.2.0/samgis_core/utilities/fastapi_logger.py`

 * *Files identical despite different names*

### Comparing `samgis_core-1.1.2/samgis_core/utilities/serialize.py` & `samgis_core-1.2.0/samgis_core/utilities/serialize.py`

 * *Files identical despite different names*

### Comparing `samgis_core-1.1.2/samgis_core/utilities/type_hints.py` & `samgis_core-1.2.0/samgis_core/utilities/type_hints.py`

 * *Files identical despite different names*

### Comparing `samgis_core-1.1.2/samgis_core/utilities/utilities.py` & `samgis_core-1.2.0/samgis_core/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `samgis_core-1.1.2/PKG-INFO` & `samgis_core-1.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: samgis_core
-Version: 1.1.2
+Version: 1.2.0
 Summary: SamGIS CORE
 License: MIT
 Author: alessandro trinca tornidor
 Author-email: alessandro@trinca.tornidor.com
-Requires-Python: >=3.10,<3.11
+Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bson (>=0.5.10,<0.6.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: numpy (==1.25.2)
+Requires-Dist: numpy (==1.25.2) ; python_version >= "3.10" and python_version < "3.11"
+Requires-Dist: numpy (>=1.26,<2.0) ; python_version >= "3.11" and python_version < "3.12"
 Requires-Dist: onnxruntime (==1.16.3)
 Requires-Dist: opencv-python-headless (==4.8.1.78)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Description-Content-Type: text/markdown
 
 # SamGIS CORE
```


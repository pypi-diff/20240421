# Comparing `tmp/data_transformation_yfhsi-0.5.1a0.tar.gz` & `tmp/data_transformation_yfhsi-0.6.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_transformation_yfhsi-0.5.1a0.tar", max compression
+gzip compressed data, was "data_transformation_yfhsi-0.6.1a0.tar", max compression
```

## Comparing `data_transformation_yfhsi-0.5.1a0.tar` & `data_transformation_yfhsi-0.6.1a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-08 12:26:59.435701 data_transformation_yfhsi-0.5.1a0/data_transformation_yfhsi/__init__.py
--rw-r--r--   0        0        0     2529 2024-04-21 10:13:44.666166 data_transformation_yfhsi-0.5.1a0/data_transformation_yfhsi/cross_correlation.py
--rw-r--r--   0        0        0     2140 2024-04-21 10:35:15.189271 data_transformation_yfhsi-0.5.1a0/data_transformation_yfhsi/time_series_windowing.py
--rw-r--r--   0        0        0     1325 2024-04-21 10:11:57.003016 data_transformation_yfhsi-0.5.1a0/data_transformation_yfhsi/transpose.py
--rw-r--r--   0        0        0      475 2024-04-21 12:18:43.046505 data_transformation_yfhsi-0.5.1a0/pyproject.toml
--rw-r--r--   0        0        0      925 2024-04-21 12:18:18.585343 data_transformation_yfhsi-0.5.1a0/README.md
--rw-r--r--   0        0        0     1296 1970-01-01 00:00:00.000000 data_transformation_yfhsi-0.5.1a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-08 12:26:59.435701 data_transformation_yfhsi-0.6.1a0/data_transformation_yfhsi/__init__.py
+-rw-r--r--   0        0        0     2529 2024-04-21 10:13:44.666166 data_transformation_yfhsi-0.6.1a0/data_transformation_yfhsi/cross_correlation.py
+-rw-r--r--   0        0        0     2140 2024-04-21 10:35:15.189271 data_transformation_yfhsi-0.6.1a0/data_transformation_yfhsi/time_series_windowing.py
+-rw-r--r--   0        0        0     1325 2024-04-21 10:11:57.003016 data_transformation_yfhsi-0.6.1a0/data_transformation_yfhsi/transpose.py
+-rw-r--r--   0        0        0      475 2024-04-21 12:20:31.693576 data_transformation_yfhsi-0.6.1a0/pyproject.toml
+-rw-r--r--   0        0        0      915 2024-04-21 12:20:22.424635 data_transformation_yfhsi-0.6.1a0/README.md
+-rw-r--r--   0        0        0     1289 1970-01-01 00:00:00.000000 data_transformation_yfhsi-0.6.1a0/PKG-INFO
```

### Comparing `data_transformation_yfhsi-0.5.1a0/data_transformation_yfhsi/cross_correlation.py` & `data_transformation_yfhsi-0.6.1a0/data_transformation_yfhsi/cross_correlation.py`

 * *Files identical despite different names*

### Comparing `data_transformation_yfhsi-0.5.1a0/data_transformation_yfhsi/time_series_windowing.py` & `data_transformation_yfhsi-0.6.1a0/data_transformation_yfhsi/time_series_windowing.py`

 * *Files identical despite different names*

### Comparing `data_transformation_yfhsi-0.5.1a0/data_transformation_yfhsi/transpose.py` & `data_transformation_yfhsi-0.6.1a0/data_transformation_yfhsi/transpose.py`

 * *Files identical despite different names*

### Comparing `data_transformation_yfhsi-0.5.1a0/README.md` & `data_transformation_yfhsi-0.6.1a0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 The Data Transformation Libraries package contains three modules:<br>
 transpose<br>
 time_series_windowing<br>
 cross_correlation<br>
-<br>
-<br>
+
 ### transpose<br>
 The transpose module includes the "transpose2d" function, which switches the axes of a 2D tensor.<br>
-Transpose function has signature: transpose2d(input_matrix: list[list[float]]) -> list<br>
-<br>
+Transpose function has signature: **transpose2d(input_matrix: list[list[float]]) -> list**<br>
 ### time_series_windowing<br>
 The time_series_windowing module includes the "window1d" function for time series windowing.<br>
-Time series windowing function has signature: window1d(input_array: list | np.ndarray, size: int, shift: int = 1, stride: int = 1) -> list[list | np.ndarray]<br>
-<br>
+Time series windowing function has signature: **window1d(input_array: list | np.ndarray, size: int, shift: int = 1, stride: int = 1) -> list[list | np.ndarray]**<br>
 ### cross_correlation<br>
 The cross_correlation module includes the "convolution2d" function for cross-correlation.<br>
-Cross correlation function has signature: convolution2d(input_matrix: np.ndarray, kernel: np.ndarray, stride : int = 1) -> np.ndarray<br>
+Cross correlation function has signature: **convolution2d(input_matrix: np.ndarray, kernel: np.ndarray, stride : int = 1) -> np.ndarray**<br>
```

### Comparing `data_transformation_yfhsi-0.5.1a0/PKG-INFO` & `data_transformation_yfhsi-0.6.1a0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: data-transformation-yfhsi
-Version: 0.5.1a0
+Version: 0.6.1a0
 Summary: 
 Author: skaival
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Description-Content-Type: text/markdown
 
 The Data Transformation Libraries package contains three modules:<br>
 transpose<br>
 time_series_windowing<br>
 cross_correlation<br>
-<br>
-<br>
+
 ### transpose<br>
 The transpose module includes the "transpose2d" function, which switches the axes of a 2D tensor.<br>
-Transpose function has signature: transpose2d(input_matrix: list[list[float]]) -> list<br>
-<br>
+Transpose function has signature: **transpose2d(input_matrix: list[list[float]]) -> list**<br>
 ### time_series_windowing<br>
 The time_series_windowing module includes the "window1d" function for time series windowing.<br>
-Time series windowing function has signature: window1d(input_array: list | np.ndarray, size: int, shift: int = 1, stride: int = 1) -> list[list | np.ndarray]<br>
-<br>
+Time series windowing function has signature: **window1d(input_array: list | np.ndarray, size: int, shift: int = 1, stride: int = 1) -> list[list | np.ndarray]**<br>
 ### cross_correlation<br>
 The cross_correlation module includes the "convolution2d" function for cross-correlation.<br>
-Cross correlation function has signature: convolution2d(input_matrix: np.ndarray, kernel: np.ndarray, stride : int = 1) -> np.ndarray<br>
+Cross correlation function has signature: **convolution2d(input_matrix: np.ndarray, kernel: np.ndarray, stride : int = 1) -> np.ndarray**<br>
```


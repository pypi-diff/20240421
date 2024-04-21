# Comparing `tmp/data_transformation_yfhsi-0.2.1a0.tar.gz` & `tmp/data_transformation_yfhsi-0.3.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_transformation_yfhsi-0.2.1a0.tar", max compression
+gzip compressed data, was "data_transformation_yfhsi-0.3.1a0.tar", max compression
```

## Comparing `data_transformation_yfhsi-0.2.1a0.tar` & `data_transformation_yfhsi-0.3.1a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-08 12:26:59.435701 data_transformation_yfhsi-0.2.1a0/data_transformation_yfhsi/__init__.py
--rw-r--r--   0        0        0     2529 2024-04-21 10:13:44.666166 data_transformation_yfhsi-0.2.1a0/data_transformation_yfhsi/cross_correlation.py
--rw-r--r--   0        0        0     2140 2024-04-21 10:11:51.084540 data_transformation_yfhsi-0.2.1a0/data_transformation_yfhsi/time_series_windowing.py
--rw-r--r--   0        0        0     1325 2024-04-21 10:11:57.003016 data_transformation_yfhsi-0.2.1a0/data_transformation_yfhsi/transpose.py
--rw-r--r--   0        0        0      477 2024-04-21 10:23:56.570625 data_transformation_yfhsi-0.2.1a0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-08 12:26:59.436699 data_transformation_yfhsi-0.2.1a0/README.md
--rw-r--r--   0        0        0      387 1970-01-01 00:00:00.000000 data_transformation_yfhsi-0.2.1a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-08 12:26:59.435701 data_transformation_yfhsi-0.3.1a0/data_transformation_yfhsi/__init__.py
+-rw-r--r--   0        0        0     2529 2024-04-21 10:13:44.666166 data_transformation_yfhsi-0.3.1a0/data_transformation_yfhsi/cross_correlation.py
+-rw-r--r--   0        0        0     2140 2024-04-21 10:35:15.189271 data_transformation_yfhsi-0.3.1a0/data_transformation_yfhsi/time_series_windowing.py
+-rw-r--r--   0        0        0     1325 2024-04-21 10:11:57.003016 data_transformation_yfhsi-0.3.1a0/data_transformation_yfhsi/transpose.py
+-rw-r--r--   0        0        0      477 2024-04-21 10:37:20.556681 data_transformation_yfhsi-0.3.1a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-08 12:26:59.436699 data_transformation_yfhsi-0.3.1a0/README.md
+-rw-r--r--   0        0        0      387 1970-01-01 00:00:00.000000 data_transformation_yfhsi-0.3.1a0/PKG-INFO
```

### Comparing `data_transformation_yfhsi-0.2.1a0/data_transformation_yfhsi/cross_correlation.py` & `data_transformation_yfhsi-0.3.1a0/data_transformation_yfhsi/cross_correlation.py`

 * *Files identical despite different names*

### Comparing `data_transformation_yfhsi-0.2.1a0/data_transformation_yfhsi/time_series_windowing.py` & `data_transformation_yfhsi-0.3.1a0/data_transformation_yfhsi/time_series_windowing.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 console_handler.setLevel(logging.INFO)
 formatter = logging.Formatter("%(levelname)s - %(message)s")
 console_handler.setFormatter(formatter)
 logger.addHandler(console_handler)
 
 
 def window1d(
-    input_array: list | np.ndarray, size: int, shift: int = 3, stride: int = 2
+    input_array: list | np.ndarray, size: int, shift: int = 1, stride: int = 1
 ) -> list[list | np.ndarray]:
     """
     The time series windowing function.
     """
     try:
         if np.array(input_array).ndim == 1:
             if isinstance(input_array, list) or isinstance(input_array,
```

### Comparing `data_transformation_yfhsi-0.2.1a0/data_transformation_yfhsi/transpose.py` & `data_transformation_yfhsi-0.3.1a0/data_transformation_yfhsi/transpose.py`

 * *Files identical despite different names*


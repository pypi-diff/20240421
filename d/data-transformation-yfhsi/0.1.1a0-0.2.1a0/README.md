# Comparing `tmp/data_transformation_yfhsi-0.1.1a0.tar.gz` & `tmp/data_transformation_yfhsi-0.2.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_transformation_yfhsi-0.1.1a0.tar", max compression
+gzip compressed data, was "data_transformation_yfhsi-0.2.1a0.tar", max compression
```

## Comparing `data_transformation_yfhsi-0.1.1a0.tar` & `data_transformation_yfhsi-0.2.1a0.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-08 12:26:59.435701 data_transformation_yfhsi-0.1.1a0/data_transformation_yfhsi/__init__.py
--rw-r--r--   0        0        0     1361 2024-04-08 12:31:09.023571 data_transformation_yfhsi-0.1.1a0/data_transformation_yfhsi/transpose.py
--rw-r--r--   0        0        0      292 2024-04-20 07:20:33.408730 data_transformation_yfhsi-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-08 12:26:59.436699 data_transformation_yfhsi-0.1.1a0/README.md
--rw-r--r--   0        0        0      348 1970-01-01 00:00:00.000000 data_transformation_yfhsi-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-08 12:26:59.435701 data_transformation_yfhsi-0.2.1a0/data_transformation_yfhsi/__init__.py
+-rw-r--r--   0        0        0     2529 2024-04-21 10:13:44.666166 data_transformation_yfhsi-0.2.1a0/data_transformation_yfhsi/cross_correlation.py
+-rw-r--r--   0        0        0     2140 2024-04-21 10:11:51.084540 data_transformation_yfhsi-0.2.1a0/data_transformation_yfhsi/time_series_windowing.py
+-rw-r--r--   0        0        0     1325 2024-04-21 10:11:57.003016 data_transformation_yfhsi-0.2.1a0/data_transformation_yfhsi/transpose.py
+-rw-r--r--   0        0        0      477 2024-04-21 10:23:56.570625 data_transformation_yfhsi-0.2.1a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-08 12:26:59.436699 data_transformation_yfhsi-0.2.1a0/README.md
+-rw-r--r--   0        0        0      387 1970-01-01 00:00:00.000000 data_transformation_yfhsi-0.2.1a0/PKG-INFO
```

### Comparing `data_transformation_yfhsi-0.1.1a0/data_transformation_yfhsi/transpose.py` & `data_transformation_yfhsi-0.2.1a0/data_transformation_yfhsi/transpose.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import logging
 
 logger = logging.getLogger()
-logger.setLevel(logging.INFO)  # Set the logging level to INFO
+logger.setLevel(logging.INFO)
 console_handler = logging.StreamHandler()
-console_handler.setLevel(logging.INFO)  # Set the handler's logging level to INFO
-formatter = logging.Formatter('%(levelname)s - %(message)s')
-console_handler.setFormatter(formatter)  # Assign the formatter to the handler
+console_handler.setLevel(logging.INFO)
+formatter = logging.Formatter("%(levelname)s - %(message)s")
+console_handler.setFormatter(formatter)
 logger.addHandler(console_handler)
 
 
 def transpose2d(input_matrix: list[list[float]]) -> list:
     """
-    Blah
+    The transpose function for a 2D matrix.
     """
     try:
         if all(isinstance(row, list) for row in input_matrix):
             for row in range(len(input_matrix)):
                 if len(input_matrix[0]) != len(input_matrix[row]):
                     raise ValueError("The matrix has an inhomogeneous shape.")
             for row in input_matrix:
                 if not all(isinstance(item, float) for item in row):
-                    raise ValueError("All matrix items must be floating-point numbers.")
+                    raise ValueError(
+                        "All matrix items must be floating-point numbers."
+                    )
         else:
             raise ValueError("Submitted matrix is not 2D.")
+
         transposed_matrix = []
         for column_index in range(len(input_matrix[0])):
             column = [row[column_index] for row in input_matrix]
             transposed_matrix.append(column)
+
         return transposed_matrix
 
     except Exception as error:
         logging.error(error)
-
```


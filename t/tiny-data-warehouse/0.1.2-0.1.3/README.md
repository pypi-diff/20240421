# Comparing `tmp/tiny_data_warehouse-0.1.2.tar.gz` & `tmp/tiny_data_warehouse-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_data_warehouse-0.1.2.tar", max compression
+gzip compressed data, was "tiny_data_warehouse-0.1.3.tar", max compression
```

## Comparing `tiny_data_warehouse-0.1.2.tar` & `tiny_data_warehouse-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       55 2024-04-20 14:50:59.621598 tiny_data_warehouse-0.1.2/README.md
--rw-r--r--   0        0        0      481 2024-04-20 14:52:02.321786 tiny_data_warehouse-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2552 2024-04-20 14:48:18.086281 tiny_data_warehouse-0.1.2/tiny_data_warehouse/data_warehouse.py
--rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 tiny_data_warehouse-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       55 2024-04-20 14:50:59.621598 tiny_data_warehouse-0.1.3/README.md
+-rw-r--r--   0        0        0      482 2024-04-21 05:22:24.539713 tiny_data_warehouse-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2552 2024-04-20 14:48:18.086281 tiny_data_warehouse-0.1.3/tiny_data_warehouse/data_warehouse.py
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 tiny_data_warehouse-0.1.3/PKG-INFO
```

### Comparing `tiny_data_warehouse-0.1.2/tiny_data_warehouse/data_warehouse.py` & `tiny_data_warehouse-0.1.3/tiny_data_warehouse/data_warehouse.py`

 * *Files identical despite different names*

### Comparing `tiny_data_warehouse-0.1.2/PKG-INFO` & `tiny_data_warehouse-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: tiny-data-warehouse
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Jean Carlo Machado
 Author-email: jean.machado@getyourguide.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: fire (>=0.5.0,<0.6.0)
+Requires-Dist: fire (>=0.6.0,<0.7.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Installation
 
 ```
 pip install tiny-data-warehouse
```


# Comparing `tmp/tiny_data_warehouse-0.1.1.tar.gz` & `tmp/tiny_data_warehouse-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_data_warehouse-0.1.1.tar", max compression
+gzip compressed data, was "tiny_data_warehouse-0.1.2.tar", max compression
```

## Comparing `tiny_data_warehouse-0.1.1.tar` & `tiny_data_warehouse-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2024-02-25 02:16:42.523466 tiny_data_warehouse-0.1.1/README.md
--rw-r--r--   0        0        0      475 2024-04-20 14:47:30.809898 tiny_data_warehouse-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2552 2024-04-20 14:48:18.086281 tiny_data_warehouse-0.1.1/tiny_data_warehouse/data_warehouse.py
--rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 tiny_data_warehouse-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       55 2024-04-20 14:50:59.621598 tiny_data_warehouse-0.1.2/README.md
+-rw-r--r--   0        0        0      481 2024-04-20 14:52:02.321786 tiny_data_warehouse-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2552 2024-04-20 14:48:18.086281 tiny_data_warehouse-0.1.2/tiny_data_warehouse/data_warehouse.py
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 tiny_data_warehouse-0.1.2/PKG-INFO
```

### Comparing `tiny_data_warehouse-0.1.1/tiny_data_warehouse/data_warehouse.py` & `tiny_data_warehouse-0.1.2/tiny_data_warehouse/data_warehouse.py`

 * *Files identical despite different names*


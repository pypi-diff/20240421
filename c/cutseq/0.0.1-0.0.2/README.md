# Comparing `tmp/cutseq-0.0.1.tar.gz` & `tmp/cutseq-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cutseq-0.0.1.tar", max compression
+gzip compressed data, was "cutseq-0.0.2.tar", max compression
```

## Comparing `cutseq-0.0.1.tar` & `cutseq-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        9 2024-04-20 09:45:43.564643 cutseq-0.0.1/README.md
--rw-r--r--   0        0        0    13807 2024-04-20 09:55:59.674508 cutseq-0.0.1/cutseq/run.py
--rw-r--r--   0        0        0      508 2024-04-20 10:12:28.924304 cutseq-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 cutseq-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        9 2024-04-20 10:24:14.412740 cutseq-0.0.2/README.md
+-rw-r--r--   0        0        0    13807 2024-04-20 10:24:14.412740 cutseq-0.0.2/cutseq/run.py
+-rw-r--r--   0        0        0      510 2024-04-20 10:24:14.412740 cutseq-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      791 1970-01-01 00:00:00.000000 cutseq-0.0.2/PKG-INFO
```

### Comparing `cutseq-0.0.1/cutseq/run.py` & `cutseq-0.0.2/cutseq/run.py`

 * *Files identical despite different names*

### Comparing `cutseq-0.0.1/PKG-INFO` & `cutseq-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cutseq
-Version: 0.0.1
-Summary: Automatic cutadapter and barcode process for NGS data
+Version: 0.0.2
+Summary: Automatically cut adapter / barcode / UMI from NGS data
 Home-page: https://github.com/y9c/cutseq
 License: MIT
 Keywords: bioinformatics,NGS,adapter,barcode,UMI
 Author: Ye Chang
 Author-email: yech1990@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


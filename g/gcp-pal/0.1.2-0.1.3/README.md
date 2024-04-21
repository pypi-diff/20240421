# Comparing `tmp/gcp_pal-0.1.2.tar.gz` & `tmp/gcp_pal-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp_pal-0.1.2.tar", max compression
+gzip compressed data, was "gcp_pal-0.1.3.tar", max compression
```

## Comparing `gcp_pal-0.1.2.tar` & `gcp_pal-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0    23152 2024-04-21 16:55:08.608993 gcp_pal-0.1.2/README.md
--rw-r--r--   0        0        0      451 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/__init__.py
--rw-r--r--   0        0        0    31402 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/bigquery.py
--rw-r--r--   0        0        0    13156 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/cloudfunctions.py
--rw-r--r--   0        0        0    13855 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/cloudrun.py
--rw-r--r--   0        0        0     7754 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/cloudscheduler.py
--rw-r--r--   0        0        0       42 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/config/__init__.py
--rw-r--r--   0        0        0      895 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/config/vars.py
--rw-r--r--   0        0        0    12490 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/firestore.py
--rw-r--r--   0        0        0     1674 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/pubsub.py
--rw-r--r--   0        0        0     3873 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/pydocker.py
--rw-r--r--   0        0        0     6860 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/pylogging.py
--rw-r--r--   0        0        0     4737 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/request.py
--rw-r--r--   0        0        0    23631 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/schema.py
--rw-r--r--   0        0        0     6332 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/secretmanager.py
--rw-r--r--   0        0        0       88 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/storage/__init__.py
--rw-r--r--   0        0        0     8735 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/storage/parquet.py
--rw-r--r--   0        0        0    17133 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/storage/storage.py
--rw-r--r--   0        0        0       33 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/utils/__init__.py
--rw-r--r--   0        0        0    10833 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/gcp_pal/utils/utils.py
--rw-r--r--   0        0        0      916 2024-04-21 16:55:08.612993 gcp_pal-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    23542 1970-01-01 00:00:00.000000 gcp_pal-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    23152 2024-04-21 17:25:42.399769 gcp_pal-0.1.3/README.md
+-rw-r--r--   0        0        0      760 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/__init__.py
+-rw-r--r--   0        0        0    31402 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/bigquery.py
+-rw-r--r--   0        0        0    13156 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/cloudfunctions.py
+-rw-r--r--   0        0        0    13855 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/cloudrun.py
+-rw-r--r--   0        0        0     7754 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/cloudscheduler.py
+-rw-r--r--   0        0        0       42 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/config/__init__.py
+-rw-r--r--   0        0        0      895 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/config/vars.py
+-rw-r--r--   0        0        0    12490 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/firestore.py
+-rw-r--r--   0        0        0     1674 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/pubsub.py
+-rw-r--r--   0        0        0     3873 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/pydocker.py
+-rw-r--r--   0        0        0     6860 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/pylogging.py
+-rw-r--r--   0        0        0     4737 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/request.py
+-rw-r--r--   0        0        0    23631 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/schema.py
+-rw-r--r--   0        0        0     6332 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/secretmanager.py
+-rw-r--r--   0        0        0       88 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/storage/__init__.py
+-rw-r--r--   0        0        0     8735 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/storage/parquet.py
+-rw-r--r--   0        0        0    17133 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/storage/storage.py
+-rw-r--r--   0        0        0       82 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/utils/__init__.py
+-rw-r--r--   0        0        0      935 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/utils/lazy_loader.py
+-rw-r--r--   0        0        0    10833 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/gcp_pal/utils/utils.py
+-rw-r--r--   0        0        0      916 2024-04-21 17:25:42.403769 gcp_pal-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    23542 1970-01-01 00:00:00.000000 gcp_pal-0.1.3/PKG-INFO
```

### Comparing `gcp_pal-0.1.2/README.md` & `gcp_pal-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gcp_pal-0.1.2/gcp_pal/bigquery.py` & `gcp_pal-0.1.3/gcp_pal/bigquery.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-0.1.2/gcp_pal/cloudfunctions.py` & `gcp_pal-0.1.3/gcp_pal/cloudfunctions.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-0.1.2/gcp_pal/cloudrun.py` & `gcp_pal-0.1.3/gcp_pal/cloudrun.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-0.1.2/gcp_pal/cloudscheduler.py` & `gcp_pal-0.1.3/gcp_pal/cloudscheduler.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-0.1.2/gcp_pal/config/vars.py` & `gcp_pal-0.1.3/gcp_pal/config/vars.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-0.1.2/gcp_pal/firestore.py` & `gcp_pal-0.1.3/gcp_pal/firestore.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-0.1.2/gcp_pal/pubsub.py` & `gcp_pal-0.1.3/gcp_pal/pubsub.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-0.1.2/gcp_pal/pydocker.py` & `gcp_pal-0.1.3/gcp_pal/pydocker.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-0.1.2/gcp_pal/pylogging.py` & `gcp_pal-0.1.3/gcp_pal/pylogging.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-0.1.2/gcp_pal/request.py` & `gcp_pal-0.1.3/gcp_pal/request.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-0.1.2/gcp_pal/schema.py` & `gcp_pal-0.1.3/gcp_pal/schema.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-0.1.2/gcp_pal/secretmanager.py` & `gcp_pal-0.1.3/gcp_pal/secretmanager.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-0.1.2/gcp_pal/storage/parquet.py` & `gcp_pal-0.1.3/gcp_pal/storage/parquet.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-0.1.2/gcp_pal/storage/storage.py` & `gcp_pal-0.1.3/gcp_pal/storage/storage.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-0.1.2/gcp_pal/utils/utils.py` & `gcp_pal-0.1.3/gcp_pal/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-0.1.2/pyproject.toml` & `gcp_pal-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcp-pal"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["VitaminB16 <artemiy.nosov@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gcp_pal-0.1.2/PKG-INFO` & `gcp_pal-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-pal
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: VitaminB16
 Author-email: artemiy.nosov@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


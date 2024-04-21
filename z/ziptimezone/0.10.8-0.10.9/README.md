# Comparing `tmp/ziptimezone-0.10.8.tar.gz` & `tmp/ziptimezone-0.10.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziptimezone-0.10.8.tar", max compression
+gzip compressed data, was "ziptimezone-0.10.9.tar", max compression
```

## Comparing `ziptimezone-0.10.8.tar` & `ziptimezone-0.10.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-0.10.8/LICENSE
--rw-r--r--   0        0        0      553 2024-04-20 20:39:01.001177 ziptimezone-0.10.8/pyproject.toml
--rw-r--r--   0        0        0      320 2024-04-20 11:29:25.216037 ziptimezone-0.10.8/README.md
--rw-r--r--   0        0        0     1156 2024-04-20 17:39:07.779806 ziptimezone-0.10.8/ziptimezone/__init__.py
--rw-r--r--   0        0        0     1908 2024-04-20 17:38:55.281645 ziptimezone-0.10.8/ziptimezone/batch_processor.py
--rw-r--r--   0        0        0     1777 2024-04-20 17:22:42.377535 ziptimezone-0.10.8/ziptimezone/core.py
--rw-r--r--   0        0        0     2780 2024-04-20 20:35:18.371359 ziptimezone-0.10.8/ziptimezone/data_manager.py
--rw-r--r--   0        0        0     1099 2024-04-20 12:33:29.828260 ziptimezone-0.10.8/ziptimezone/geocode.py
--rw-r--r--   0        0        0     1297 2024-04-20 17:32:08.297733 ziptimezone-0.10.8/ziptimezone/globals.py
--rw-r--r--   0        0        0     1873 2024-04-20 11:29:25.238387 ziptimezone-0.10.8/ziptimezone/mappings.py
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 ziptimezone-0.10.8/PKG-INFO
+-rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-0.10.9/LICENSE
+-rw-r--r--   0        0        0      553 2024-04-20 21:16:18.699967 ziptimezone-0.10.9/pyproject.toml
+-rw-r--r--   0        0        0      320 2024-04-20 11:29:25.216037 ziptimezone-0.10.9/README.md
+-rw-r--r--   0        0        0     1156 2024-04-20 17:39:07.779806 ziptimezone-0.10.9/ziptimezone/__init__.py
+-rw-r--r--   0        0        0     1908 2024-04-20 17:38:55.281645 ziptimezone-0.10.9/ziptimezone/batch_processor.py
+-rw-r--r--   0        0        0     1777 2024-04-20 17:22:42.377535 ziptimezone-0.10.9/ziptimezone/core.py
+-rw-r--r--   0        0        0     2780 2024-04-20 20:35:18.371359 ziptimezone-0.10.9/ziptimezone/data_manager.py
+-rw-r--r--   0        0        0     1099 2024-04-20 12:33:29.828260 ziptimezone-0.10.9/ziptimezone/geocode.py
+-rw-r--r--   0        0        0     1297 2024-04-20 17:32:08.297733 ziptimezone-0.10.9/ziptimezone/globals.py
+-rw-r--r--   0        0        0     1873 2024-04-20 11:29:25.238387 ziptimezone-0.10.9/ziptimezone/mappings.py
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 ziptimezone-0.10.9/PKG-INFO
```

### Comparing `ziptimezone-0.10.8/pyproject.toml` & `ziptimezone-0.10.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ziptimezone"
-version = "0.10.8"
+version = "0.10.9"
 description = "A package to convert ZIP codes to time zones and get geographic coordinates."
 readme = "README.md"
 authors = ["Manjunath Bettadapura <manjunathbettadapura412@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <4.0"
```

### Comparing `ziptimezone-0.10.8/ziptimezone/__init__.py` & `ziptimezone-0.10.9/ziptimezone/__init__.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.8/ziptimezone/batch_processor.py` & `ziptimezone-0.10.9/ziptimezone/batch_processor.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.8/ziptimezone/core.py` & `ziptimezone-0.10.9/ziptimezone/core.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.8/ziptimezone/data_manager.py` & `ziptimezone-0.10.9/ziptimezone/data_manager.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.8/ziptimezone/geocode.py` & `ziptimezone-0.10.9/ziptimezone/geocode.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.8/ziptimezone/globals.py` & `ziptimezone-0.10.9/ziptimezone/globals.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.8/ziptimezone/mappings.py` & `ziptimezone-0.10.9/ziptimezone/mappings.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.8/PKG-INFO` & `ziptimezone-0.10.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziptimezone
-Version: 0.10.8
+Version: 0.10.9
 Summary: A package to convert ZIP codes to time zones and get geographic coordinates.
 License: MIT
 Author: Manjunath Bettadapura
 Author-email: manjunathbettadapura412@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


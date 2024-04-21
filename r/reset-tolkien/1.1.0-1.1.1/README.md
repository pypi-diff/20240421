# Comparing `tmp/reset-tolkien-1.1.0.tar.gz` & `tmp/reset_tolkien-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reset-tolkien-1.1.0.tar", last modified: Sat Apr 13 07:59:38 2024, max compression
+gzip compressed data, was "reset_tolkien-1.1.1.tar", last modified: Sun Apr 21 09:59:25 2024, max compression
```

## Comparing `reset-tolkien-1.1.0.tar` & `reset_tolkien-1.1.1.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 aethlios  (1000) aethlios  (1000)        0 2024-04-13 07:59:38.939850 reset-tolkien-1.1.0/
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)     1073 2024-03-29 16:44:20.000000 reset-tolkien-1.1.0/LICENSE
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)    16830 2024-04-13 07:59:38.939850 reset-tolkien-1.1.0/PKG-INFO
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)    13517 2024-04-06 18:13:01.000000 reset-tolkien-1.1.0/README.md
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)     2146 2024-04-13 07:53:32.000000 reset-tolkien-1.1.0/pyproject.toml
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)       38 2024-04-13 07:59:38.939850 reset-tolkien-1.1.0/setup.cfg
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)       37 2024-03-29 16:43:47.000000 reset-tolkien-1.1.0/setup.py
-drwxr-xr-x   0 aethlios  (1000) aethlios  (1000)        0 2024-04-13 07:59:38.927849 reset-tolkien-1.1.0/src/
-drwxr-xr-x   0 aethlios  (1000) aethlios  (1000)        0 2024-04-13 07:59:38.935850 reset-tolkien-1.1.0/src/resetTolkien/
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)      221 2024-04-06 17:47:14.000000 reset-tolkien-1.1.0/src/resetTolkien/__init__.py
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)       72 2024-03-29 16:43:15.000000 reset-tolkien-1.1.0/src/resetTolkien/__main__.py
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)    13573 2024-03-29 16:43:15.000000 reset-tolkien-1.1.0/src/resetTolkien/cli.py
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)     2278 2024-04-03 09:36:23.000000 reset-tolkien-1.1.0/src/resetTolkien/constants.py
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)    24743 2024-04-06 17:16:56.000000 reset-tolkien-1.1.0/src/resetTolkien/format.py
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)     1525 2024-03-29 16:43:15.000000 reset-tolkien-1.1.0/src/resetTolkien/hashes.py
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)    16200 2024-04-06 17:16:18.000000 reset-tolkien-1.1.0/src/resetTolkien/resetTolkien.py
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)    15513 2024-04-03 09:23:27.000000 reset-tolkien-1.1.0/src/resetTolkien/utils.py
-drwxr-xr-x   0 aethlios  (1000) aethlios  (1000)        0 2024-04-13 07:59:38.939850 reset-tolkien-1.1.0/src/reset_tolkien.egg-info/
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)    16830 2024-04-13 07:59:38.000000 reset-tolkien-1.1.0/src/reset_tolkien.egg-info/PKG-INFO
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)      537 2024-04-13 07:59:38.000000 reset-tolkien-1.1.0/src/reset_tolkien.egg-info/SOURCES.txt
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)        1 2024-04-13 07:59:38.000000 reset-tolkien-1.1.0/src/reset_tolkien.egg-info/dependency_links.txt
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)       52 2024-04-13 07:59:38.000000 reset-tolkien-1.1.0/src/reset_tolkien.egg-info/entry_points.txt
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)      249 2024-04-13 07:59:38.000000 reset-tolkien-1.1.0/src/reset_tolkien.egg-info/requires.txt
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)       22 2024-04-13 07:59:38.000000 reset-tolkien-1.1.0/src/reset_tolkien.egg-info/top_level.txt
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)       72 2024-03-29 16:56:55.000000 reset-tolkien-1.1.0/src/run.py
--rw-r--r--   0 aethlios  (1000) aethlios  (1000)    15201 2024-03-29 16:54:13.000000 reset-tolkien-1.1.0/src/test.py
+drwxr-xr-x   0 aethlios  (1000) aethlios  (1000)        0 2024-04-21 09:59:25.710996 reset_tolkien-1.1.1/
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)     1073 2024-03-29 16:44:20.000000 reset_tolkien-1.1.1/LICENSE
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)       34 2024-04-21 09:51:51.000000 reset_tolkien-1.1.1/MANIFEST.in
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)    16830 2024-04-21 09:59:25.710996 reset_tolkien-1.1.1/PKG-INFO
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)    13517 2024-04-06 18:13:01.000000 reset_tolkien-1.1.1/README.md
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)     2146 2024-04-21 09:55:48.000000 reset_tolkien-1.1.1/pyproject.toml
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)       38 2024-04-21 09:59:25.710996 reset_tolkien-1.1.1/setup.cfg
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)       37 2024-03-29 16:43:47.000000 reset_tolkien-1.1.1/setup.py
+drwxr-xr-x   0 aethlios  (1000) aethlios  (1000)        0 2024-04-21 09:59:25.698996 reset_tolkien-1.1.1/src/
+drwxr-xr-x   0 aethlios  (1000) aethlios  (1000)        0 2024-04-21 09:59:25.706996 reset_tolkien-1.1.1/src/resetTolkien/
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)      221 2024-04-21 09:33:36.000000 reset_tolkien-1.1.1/src/resetTolkien/__init__.py
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)       72 2024-03-29 16:43:15.000000 reset_tolkien-1.1.1/src/resetTolkien/__main__.py
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)    13573 2024-04-21 09:22:35.000000 reset_tolkien-1.1.1/src/resetTolkien/cli.py
+drwxr-xr-x   0 aethlios  (1000) aethlios  (1000)        0 2024-04-21 09:59:25.706996 reset_tolkien-1.1.1/src/resetTolkien/config/
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)      739 2024-03-29 16:43:43.000000 reset_tolkien-1.1.1/src/resetTolkien/config/default.yml
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)     2394 2024-04-21 09:44:32.000000 reset_tolkien-1.1.1/src/resetTolkien/constants.py
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)    24743 2024-04-06 17:16:56.000000 reset_tolkien-1.1.1/src/resetTolkien/format.py
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)     1525 2024-03-29 16:43:15.000000 reset_tolkien-1.1.1/src/resetTolkien/hashes.py
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)    16200 2024-04-06 17:16:18.000000 reset_tolkien-1.1.1/src/resetTolkien/resetTolkien.py
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)    15513 2024-04-03 09:23:27.000000 reset_tolkien-1.1.1/src/resetTolkien/utils.py
+drwxr-xr-x   0 aethlios  (1000) aethlios  (1000)        0 2024-04-21 09:59:25.710996 reset_tolkien-1.1.1/src/reset_tolkien.egg-info/
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)    16830 2024-04-21 09:59:25.000000 reset_tolkien-1.1.1/src/reset_tolkien.egg-info/PKG-INFO
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)      585 2024-04-21 09:59:25.000000 reset_tolkien-1.1.1/src/reset_tolkien.egg-info/SOURCES.txt
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)        1 2024-04-21 09:59:25.000000 reset_tolkien-1.1.1/src/reset_tolkien.egg-info/dependency_links.txt
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)       52 2024-04-21 09:59:25.000000 reset_tolkien-1.1.1/src/reset_tolkien.egg-info/entry_points.txt
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)      249 2024-04-21 09:59:25.000000 reset_tolkien-1.1.1/src/reset_tolkien.egg-info/requires.txt
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)       22 2024-04-21 09:59:25.000000 reset_tolkien-1.1.1/src/reset_tolkien.egg-info/top_level.txt
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)       72 2024-03-29 16:56:55.000000 reset_tolkien-1.1.1/src/run.py
+-rw-r--r--   0 aethlios  (1000) aethlios  (1000)    15201 2024-03-29 16:54:13.000000 reset_tolkien-1.1.1/src/test.py
```

### Comparing `reset-tolkien-1.1.0/LICENSE` & `reset_tolkien-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reset-tolkien-1.1.0/PKG-INFO` & `reset_tolkien-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reset-tolkien
-Version: 1.1.0
+Version: 1.1.1
 Summary: Unsecure time-based secret exploitation and Sandwich attack implementation.
 Author-email: Tom CHAMBARETAUD <tom.chambaretaud@protonmail.com>
 Maintainer-email: Tom CHAMBARETAUD <tom.chambaretaud@protonmail.com>
 License: MIT License
         
         Copyright (c) 2024 Tom Chambaretaud
```

### Comparing `reset-tolkien-1.1.0/README.md` & `reset_tolkien-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `reset-tolkien-1.1.0/pyproject.toml` & `reset_tolkien-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reset-tolkien-1.1.0/src/resetTolkien/cli.py` & `reset_tolkien-1.1.1/src/resetTolkien/cli.py`

 * *Files identical despite different names*

### Comparing `reset-tolkien-1.1.0/src/resetTolkien/constants.py` & `reset_tolkien-1.1.1/src/resetTolkien/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Author: Aethlios <tom.chambaretaud@protonmail.com>
 
-from os import cpu_count
+from os import cpu_count, path
 
 OUTPUT_STRINGS = {
     "ROLEPLAY": {
         "TIMESTAMP_FOUND": "We found my precious! {timestamp} (prefix: {prefix} / suffix: {suffix})",
         "TOKEN_FORMAT": 'The way to get my precious is "{formats}"',
         "OUTPUT_IN_FILE": 'I\'ve hidden my precious ones in this dark corner: "{output}"',
         "INT_TIMESTAMP": "Please set you precious with --only-int-timestamp",
@@ -36,15 +36,16 @@
 DEFAULT_THREAD_NUMBER = cpu if cpu else 1
 MIN_DEPTH_LEVEL = 1
 MAX_DEPTH_LEVEL = 3
 DEFAULT_DEPTH_LEVEL = MAX_DEPTH_LEVEL
 MAX_VERBOSITY_LEVEL = 2
 DEFAULT_VERBOSITY_LEVEL = 0
 
-DEFAULT_CONFIG_FILE = "default.yml"
+DEFAULT_CONFIG_FILENAME = "default.yml"
+DEFAULT_CONFIG_FILE = path.join(path.dirname(path.realpath(__file__)), "config", DEFAULT_CONFIG_FILENAME)
 
 SERVER_DATE_FORMAT = "%a, %d %b %Y %H:%M:%S %Z"
 
 PARTIAL_FUNC_NAME_REGEX = r"functools\.partial\(<bound method Formatter\.([a-zA-Z_]*) of <src\.format\.Formatter object at [0-9a-fx]*>>, (.*)\)"
 
 # 12/12/2023 or 5/5/2023 or 12/12/23 or 2023/12/12
 DATE_SLASH_REGEX = r"[0-9]{1,4}\/[0-9]{1,2}\/[0-9]{1,4}"
```

### Comparing `reset-tolkien-1.1.0/src/resetTolkien/format.py` & `reset_tolkien-1.1.1/src/resetTolkien/format.py`

 * *Files identical despite different names*

### Comparing `reset-tolkien-1.1.0/src/resetTolkien/hashes.py` & `reset_tolkien-1.1.1/src/resetTolkien/hashes.py`

 * *Files identical despite different names*

### Comparing `reset-tolkien-1.1.0/src/resetTolkien/resetTolkien.py` & `reset_tolkien-1.1.1/src/resetTolkien/resetTolkien.py`

 * *Files identical despite different names*

### Comparing `reset-tolkien-1.1.0/src/resetTolkien/utils.py` & `reset_tolkien-1.1.1/src/resetTolkien/utils.py`

 * *Files identical despite different names*

### Comparing `reset-tolkien-1.1.0/src/reset_tolkien.egg-info/PKG-INFO` & `reset_tolkien-1.1.1/src/reset_tolkien.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reset-tolkien
-Version: 1.1.0
+Version: 1.1.1
 Summary: Unsecure time-based secret exploitation and Sandwich attack implementation.
 Author-email: Tom CHAMBARETAUD <tom.chambaretaud@protonmail.com>
 Maintainer-email: Tom CHAMBARETAUD <tom.chambaretaud@protonmail.com>
 License: MIT License
         
         Copyright (c) 2024 Tom Chambaretaud
```

### Comparing `reset-tolkien-1.1.0/src/reset_tolkien.egg-info/SOURCES.txt` & `reset_tolkien-1.1.1/src/reset_tolkien.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/run.py
 src/test.py
 src/resetTolkien/__init__.py
 src/resetTolkien/__main__.py
 src/resetTolkien/cli.py
 src/resetTolkien/constants.py
 src/resetTolkien/format.py
 src/resetTolkien/hashes.py
 src/resetTolkien/resetTolkien.py
 src/resetTolkien/utils.py
+src/resetTolkien/config/default.yml
 src/reset_tolkien.egg-info/PKG-INFO
 src/reset_tolkien.egg-info/SOURCES.txt
 src/reset_tolkien.egg-info/dependency_links.txt
 src/reset_tolkien.egg-info/entry_points.txt
 src/reset_tolkien.egg-info/requires.txt
 src/reset_tolkien.egg-info/top_level.txt
```

### Comparing `reset-tolkien-1.1.0/src/test.py` & `reset_tolkien-1.1.1/src/test.py`

 * *Files identical despite different names*


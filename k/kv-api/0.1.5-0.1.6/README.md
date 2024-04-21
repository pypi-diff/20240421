# Comparing `tmp/kv_api-0.1.5.tar.gz` & `tmp/kv_api-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_api-0.1.5.tar", last modified: Sat Apr 20 18:04:02 2024, max compression
+gzip compressed data, was "kv_api-0.1.6.tar", last modified: Sun Apr 21 07:39:16 2024, max compression
```

## Comparing `kv_api-0.1.5.tar` & `kv_api-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:02.820967 kv_api-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      423 2024-04-20 18:04:02.820967 kv_api-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       46 2024-04-05 12:42:30.000000 kv_api-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      603 2024-04-20 18:04:00.000000 kv_api-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-20 18:04:02.820967 kv_api-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:02.810967 kv_api-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:02.810967 kv_api-0.1.5/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:02.810967 kv_api-0.1.5/src/kv/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      122 2024-04-20 17:32:30.000000 kv_api-0.1.5/src/kv/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2491 2024-04-20 17:54:31.000000 kv_api-0.1.5/src/kv/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:02.810967 kv_api-0.1.5/src/kv/api/append/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       79 2024-04-20 17:37:34.000000 kv_api-0.1.5/src/kv/api/append/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      818 2024-04-20 17:34:19.000000 kv_api-0.1.5/src/kv/api/append/append.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      646 2024-04-20 17:38:48.000000 kv_api-0.1.5/src/kv/api/append/simple.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:02.810967 kv_api-0.1.5/src/kv/api/errors/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       81 2024-04-10 05:52:43.000000 kv_api-0.1.5/src/kv/api/errors/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      791 2024-04-20 05:01:50.000000 kv_api-0.1.5/src/kv/api/errors/errors.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1598 2024-04-20 17:32:02.000000 kv_api-0.1.5/src/kv/api/simple.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:02.820967 kv_api-0.1.5/src/kv_api.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      423 2024-04-20 18:04:02.000000 kv_api-0.1.5/src/kv_api.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      399 2024-04-20 18:04:02.000000 kv_api-0.1.5/src/kv_api.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-20 18:04:02.000000 kv_api-0.1.5/src/kv_api.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-04-20 18:04:02.000000 kv_api-0.1.5/src/kv_api.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-20 18:04:02.000000 kv_api-0.1.5/src/kv_api.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 07:39:16.777275 kv_api-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      490 2024-04-21 07:39:16.777275 kv_api-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       46 2024-04-05 12:42:30.000000 kv_api-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      646 2024-04-21 07:39:14.000000 kv_api-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-21 07:39:16.777275 kv_api-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 07:39:16.777275 kv_api-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 07:39:16.777275 kv_api-0.1.6/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 07:39:16.777275 kv_api-0.1.6/src/kv/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      122 2024-04-20 17:32:30.000000 kv_api-0.1.6/src/kv/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2491 2024-04-20 17:54:31.000000 kv_api-0.1.6/src/kv/api/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 07:39:16.777275 kv_api-0.1.6/src/kv/api/append/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       79 2024-04-20 17:37:34.000000 kv_api-0.1.6/src/kv/api/append/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      818 2024-04-20 17:34:19.000000 kv_api-0.1.6/src/kv/api/append/append.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      646 2024-04-20 17:38:48.000000 kv_api-0.1.6/src/kv/api/append/simple.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 07:39:16.777275 kv_api-0.1.6/src/kv/api/errors/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       81 2024-04-10 05:52:43.000000 kv_api-0.1.6/src/kv/api/errors/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      791 2024-04-20 05:01:50.000000 kv_api-0.1.6/src/kv/api/errors/errors.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1598 2024-04-20 17:32:02.000000 kv_api-0.1.6/src/kv/api/simple.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 07:39:16.777275 kv_api-0.1.6/src/kv_api.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      490 2024-04-21 07:39:16.000000 kv_api-0.1.6/src/kv_api.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      399 2024-04-21 07:39:16.000000 kv_api-0.1.6/src/kv_api.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-21 07:39:16.000000 kv_api-0.1.6/src/kv_api.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       55 2024-04-21 07:39:16.000000 kv_api-0.1.6/src/kv_api.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-21 07:39:16.000000 kv_api-0.1.6/src/kv_api.egg-info/top_level.txt
```

### Comparing `kv_api-0.1.5/src/kv/api/api.py` & `kv_api-0.1.6/src/kv/api/api.py`

 * *Files identical despite different names*

### Comparing `kv_api-0.1.5/src/kv/api/append/append.py` & `kv_api-0.1.6/src/kv/api/append/append.py`

 * *Files identical despite different names*

### Comparing `kv_api-0.1.5/src/kv/api/append/simple.py` & `kv_api-0.1.6/src/kv/api/append/simple.py`

 * *Files identical despite different names*

### Comparing `kv_api-0.1.5/src/kv/api/errors/errors.py` & `kv_api-0.1.6/src/kv/api/errors/errors.py`

 * *Files identical despite different names*

### Comparing `kv_api-0.1.5/src/kv/api/simple.py` & `kv_api-0.1.6/src/kv/api/simple.py`

 * *Files identical despite different names*


# Comparing `tmp/qfpy-6.0.0.tar.gz` & `tmp/qfpy-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfpy-6.0.0.tar", last modified: Sun Apr 21 04:49:30 2024, max compression
+gzip compressed data, was "qfpy-6.0.1.tar", last modified: Sun Apr 21 04:51:04 2024, max compression
```

## Comparing `qfpy-6.0.0.tar` & `qfpy-6.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 04:49:30.334000 qfpy-6.0.0/
--rw-rw-rw-   0        0        0      159 2024-04-21 04:49:30.331067 qfpy-6.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-21 04:49:07.000000 qfpy-6.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-21 04:49:30.334000 qfpy-6.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-21 04:49:30.292880 qfpy-6.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-21 04:49:30.317417 qfpy-6.0.0/src/qfpy/
--rw-rw-rw-   0        0        0       29 2024-03-06 16:44:46.000000 qfpy-6.0.0/src/qfpy/__init__.py
--rw-rw-rw-   0        0        0      149 2024-04-21 04:48:34.000000 qfpy-6.0.0/src/qfpy/character.py
--rw-rw-rw-   0        0        0     1393 2024-03-27 09:56:39.000000 qfpy-6.0.0/src/qfpy/exif.py
--rw-rw-rw-   0        0        0     3124 2024-04-21 04:46:11.000000 qfpy-6.0.0/src/qfpy/ffmpeg.py
--rw-rw-rw-   0        0        0      611 2024-04-21 04:47:36.000000 qfpy-6.0.0/src/qfpy/folder.py
--rw-rw-rw-   0        0        0      845 2024-03-23 10:23:45.000000 qfpy-6.0.0/src/qfpy/function.py
--rw-rw-rw-   0        0        0      804 2024-03-23 10:20:43.000000 qfpy-6.0.0/src/qfpy/process.py
-drwxrwxrwx   0        0        0        0 2024-04-21 04:49:30.329110 qfpy-6.0.0/src/qfpy.egg-info/
--rw-rw-rw-   0        0        0      159 2024-04-21 04:49:30.000000 qfpy-6.0.0/src/qfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-04-21 04:49:30.000000 qfpy-6.0.0/src/qfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 04:49:30.000000 qfpy-6.0.0/src/qfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-21 04:49:30.000000 qfpy-6.0.0/src/qfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 04:51:04.182348 qfpy-6.0.1/
+-rw-rw-rw-   0        0        0      159 2024-04-21 04:51:04.180400 qfpy-6.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-21 04:50:53.000000 qfpy-6.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-21 04:51:04.182348 qfpy-6.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-21 04:51:04.154474 qfpy-6.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-21 04:51:04.169136 qfpy-6.0.1/src/qfpy/
+-rw-rw-rw-   0        0        0       29 2024-03-06 16:44:46.000000 qfpy-6.0.1/src/qfpy/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-21 04:50:44.000000 qfpy-6.0.1/src/qfpy/character.py
+-rw-rw-rw-   0        0        0     1393 2024-03-27 09:56:39.000000 qfpy-6.0.1/src/qfpy/exif.py
+-rw-rw-rw-   0        0        0     3124 2024-04-21 04:46:11.000000 qfpy-6.0.1/src/qfpy/ffmpeg.py
+-rw-rw-rw-   0        0        0      611 2024-04-21 04:47:36.000000 qfpy-6.0.1/src/qfpy/folder.py
+-rw-rw-rw-   0        0        0      845 2024-03-23 10:23:45.000000 qfpy-6.0.1/src/qfpy/function.py
+-rw-rw-rw-   0        0        0      804 2024-03-23 10:20:43.000000 qfpy-6.0.1/src/qfpy/process.py
+drwxrwxrwx   0        0        0        0 2024-04-21 04:51:04.178439 qfpy-6.0.1/src/qfpy.egg-info/
+-rw-rw-rw-   0        0        0      159 2024-04-21 04:51:04.000000 qfpy-6.0.1/src/qfpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-04-21 04:51:04.000000 qfpy-6.0.1/src/qfpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 04:51:04.000000 qfpy-6.0.1/src/qfpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-21 04:51:04.000000 qfpy-6.0.1/src/qfpy.egg-info/top_level.txt
```

### Comparing `qfpy-6.0.0/src/qfpy/exif.py` & `qfpy-6.0.1/src/qfpy/exif.py`

 * *Files identical despite different names*

### Comparing `qfpy-6.0.0/src/qfpy/ffmpeg.py` & `qfpy-6.0.1/src/qfpy/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `qfpy-6.0.0/src/qfpy/folder.py` & `qfpy-6.0.1/src/qfpy/folder.py`

 * *Files identical despite different names*

### Comparing `qfpy-6.0.0/src/qfpy/function.py` & `qfpy-6.0.1/src/qfpy/function.py`

 * *Files identical despite different names*

### Comparing `qfpy-6.0.0/src/qfpy/process.py` & `qfpy-6.0.1/src/qfpy/process.py`

 * *Files identical despite different names*


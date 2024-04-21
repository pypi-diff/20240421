# Comparing `tmp/pure-cv-0.1.7.tar.gz` & `tmp/pure_cv-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure-cv-0.1.7.tar", last modified: Fri Apr 12 05:52:45 2024, max compression
+gzip compressed data, was "pure_cv-0.1.8.tar", last modified: Sun Apr 21 16:49:48 2024, max compression
```

## Comparing `pure-cv-0.1.7.tar` & `pure_cv-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-12 05:52:45.531650 pure-cv-0.1.7/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      402 2024-04-12 05:52:45.531650 pure-cv-0.1.7/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       45 2024-04-07 16:01:13.000000 pure-cv-0.1.7/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      472 2024-04-12 05:52:39.000000 pure-cv-0.1.7/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-12 05:52:45.531650 pure-cv-0.1.7/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-12 05:52:45.521650 pure-cv-0.1.7/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-12 05:52:45.531650 pure-cv-0.1.7/src/pure_cv/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-12 05:52:26.000000 pure-cv-0.1.7/src/pure_cv/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      280 2024-04-07 16:01:25.000000 pure-cv-0.1.7/src/pure_cv/colors.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-12 05:52:45.531650 pure-cv-0.1.7/src/pure_cv/draw/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       59 2024-04-07 16:01:25.000000 pure-cv-0.1.7/src/pure_cv/draw/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1803 2024-04-07 16:01:25.000000 pure-cv-0.1.7/src/pure_cv/draw/draw.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      853 2024-04-07 16:02:42.000000 pure-cv-0.1.7/src/pure_cv/encoding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      180 2024-04-07 16:01:25.000000 pure-cv-0.1.7/src/pure_cv/misc.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1114 2024-04-07 16:01:25.000000 pure-cv-0.1.7/src/pure_cv/opencv.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1360 2024-04-07 16:01:25.000000 pure-cv-0.1.7/src/pure_cv/plot.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      491 2024-04-07 16:01:25.000000 pure-cv-0.1.7/src/pure_cv/rescaling.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      462 2024-04-12 05:51:59.000000 pure-cv-0.1.7/src/pure_cv/rotation.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-12 05:52:45.531650 pure-cv-0.1.7/src/pure_cv.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      402 2024-04-12 05:52:45.000000 pure-cv-0.1.7/src/pure_cv.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-04-12 05:52:45.000000 pure-cv-0.1.7/src/pure_cv.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-12 05:52:45.000000 pure-cv-0.1.7/src/pure_cv.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       45 2024-04-12 05:52:45.000000 pure-cv-0.1.7/src/pure_cv.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        8 2024-04-12 05:52:45.000000 pure-cv-0.1.7/src/pure_cv.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:49:48.819880 pure_cv-0.1.8/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-04-21 16:49:48.819880 pure_cv-0.1.8/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       45 2024-04-07 16:01:13.000000 pure_cv-0.1.8/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      491 2024-04-21 16:49:42.000000 pure_cv-0.1.8/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-21 16:49:48.819880 pure_cv-0.1.8/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:49:48.819880 pure_cv-0.1.8/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:49:48.819880 pure_cv-0.1.8/src/pure_cv/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 16:47:02.000000 pure_cv-0.1.8/src/pure_cv/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      613 2024-04-21 16:46:54.000000 pure_cv-0.1.8/src/pure_cv/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      280 2024-04-07 16:01:25.000000 pure_cv-0.1.8/src/pure_cv/colors.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:49:48.819880 pure_cv-0.1.8/src/pure_cv/draw/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       59 2024-04-07 16:01:25.000000 pure_cv-0.1.8/src/pure_cv/draw/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1803 2024-04-07 16:01:25.000000 pure_cv-0.1.8/src/pure_cv/draw/draw.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      853 2024-04-07 16:02:42.000000 pure_cv-0.1.8/src/pure_cv/encoding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      180 2024-04-07 16:01:25.000000 pure_cv-0.1.8/src/pure_cv/misc.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1114 2024-04-07 16:01:25.000000 pure_cv-0.1.8/src/pure_cv/opencv.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1360 2024-04-07 16:01:25.000000 pure_cv-0.1.8/src/pure_cv/plot.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      491 2024-04-07 16:01:25.000000 pure_cv-0.1.8/src/pure_cv/rescaling.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      462 2024-04-12 05:51:59.000000 pure_cv-0.1.8/src/pure_cv/rotation.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:49:48.819880 pure_cv-0.1.8/src/pure_cv.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      429 2024-04-21 16:49:48.000000 pure_cv-0.1.8/src/pure_cv.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      458 2024-04-21 16:49:48.000000 pure_cv-0.1.8/src/pure_cv.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-21 16:49:48.000000 pure_cv-0.1.8/src/pure_cv.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       57 2024-04-21 16:49:48.000000 pure_cv-0.1.8/src/pure_cv.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        8 2024-04-21 16:49:48.000000 pure_cv-0.1.8/src/pure_cv.egg-info/top_level.txt
```

### Comparing `pure-cv-0.1.7/src/pure_cv/draw/draw.py` & `pure_cv-0.1.8/src/pure_cv/draw/draw.py`

 * *Files identical despite different names*

### Comparing `pure-cv-0.1.7/src/pure_cv/encoding.py` & `pure_cv-0.1.8/src/pure_cv/encoding.py`

 * *Files identical despite different names*

### Comparing `pure-cv-0.1.7/src/pure_cv/opencv.py` & `pure_cv-0.1.8/src/pure_cv/opencv.py`

 * *Files identical despite different names*

### Comparing `pure-cv-0.1.7/src/pure_cv/plot.py` & `pure_cv-0.1.8/src/pure_cv/plot.py`

 * *Files identical despite different names*


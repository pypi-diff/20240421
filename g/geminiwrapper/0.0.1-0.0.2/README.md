# Comparing `tmp/geminiwrapper-0.0.1.tar.gz` & `tmp/geminiwrapper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geminiwrapper-0.0.1.tar", last modified: Sun Apr 21 07:22:42 2024, max compression
+gzip compressed data, was "geminiwrapper-0.0.2.tar", last modified: Sun Apr 21 07:27:10 2024, max compression
```

## Comparing `geminiwrapper-0.0.1.tar` & `geminiwrapper-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 07:22:42.469035 geminiwrapper-0.0.1/
--rw-rw-rw-   0        0        0      459 2024-04-21 07:22:42.469035 geminiwrapper-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-21 00:03:59.000000 geminiwrapper-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 07:22:42.448961 geminiwrapper-0.0.1/geminiwrapper/
--rw-rw-rw-   0        0        0      160 2024-04-20 20:48:54.000000 geminiwrapper-0.0.1/geminiwrapper/__init__.py
--rw-rw-rw-   0        0        0     1425 2024-04-21 01:29:01.000000 geminiwrapper-0.0.1/geminiwrapper/json_wrapper.py
--rw-rw-rw-   0        0        0     2328 2024-04-21 01:09:14.000000 geminiwrapper-0.0.1/geminiwrapper/object_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:22:42.468204 geminiwrapper-0.0.1/geminiwrapper.egg-info/
--rw-rw-rw-   0        0        0      459 2024-04-21 07:22:42.000000 geminiwrapper-0.0.1/geminiwrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-04-21 07:22:42.000000 geminiwrapper-0.0.1/geminiwrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 07:22:42.000000 geminiwrapper-0.0.1/geminiwrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-21 07:22:42.000000 geminiwrapper-0.0.1/geminiwrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-21 07:22:42.000000 geminiwrapper-0.0.1/geminiwrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 07:22:42.469035 geminiwrapper-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      658 2024-04-21 07:21:58.000000 geminiwrapper-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 07:27:10.636540 geminiwrapper-0.0.2/
+-rw-rw-rw-   0        0        0      459 2024-04-21 07:27:10.636540 geminiwrapper-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-21 00:03:59.000000 geminiwrapper-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 07:27:10.620113 geminiwrapper-0.0.2/geminiwrapper/
+-rw-rw-rw-   0        0        0       82 2024-04-21 07:26:39.000000 geminiwrapper-0.0.2/geminiwrapper/__init__.py
+-rw-rw-rw-   0        0        0     1425 2024-04-21 01:29:01.000000 geminiwrapper-0.0.2/geminiwrapper/json_wrapper.py
+-rw-rw-rw-   0        0        0     2328 2024-04-21 01:09:14.000000 geminiwrapper-0.0.2/geminiwrapper/object_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-21 07:27:10.636540 geminiwrapper-0.0.2/geminiwrapper.egg-info/
+-rw-rw-rw-   0        0        0      459 2024-04-21 07:27:10.000000 geminiwrapper-0.0.2/geminiwrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-04-21 07:27:10.000000 geminiwrapper-0.0.2/geminiwrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 07:27:10.000000 geminiwrapper-0.0.2/geminiwrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-21 07:27:10.000000 geminiwrapper-0.0.2/geminiwrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-21 07:27:10.000000 geminiwrapper-0.0.2/geminiwrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 07:27:10.636540 geminiwrapper-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      658 2024-04-21 07:27:06.000000 geminiwrapper-0.0.2/setup.py
```

### Comparing `geminiwrapper-0.0.1/geminiwrapper/json_wrapper.py` & `geminiwrapper-0.0.2/geminiwrapper/json_wrapper.py`

 * *Files identical despite different names*

### Comparing `geminiwrapper-0.0.1/geminiwrapper/object_wrapper.py` & `geminiwrapper-0.0.2/geminiwrapper/object_wrapper.py`

 * *Files identical despite different names*

### Comparing `geminiwrapper-0.0.1/setup.py` & `geminiwrapper-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="geminiwrapper",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(),
     install_requires=[
         "google-generativeai",
     ],
     description="Library for generating consistent Gemini API outputs and wrapping them with json and python objects",
     author="Min Htet Naing",
     author_email="minhtetnaing25mhn@gmail.com",
```


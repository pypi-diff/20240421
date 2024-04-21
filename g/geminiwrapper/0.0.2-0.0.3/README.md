# Comparing `tmp/geminiwrapper-0.0.2.tar.gz` & `tmp/geminiwrapper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geminiwrapper-0.0.2.tar", last modified: Sun Apr 21 07:27:10 2024, max compression
+gzip compressed data, was "geminiwrapper-0.0.3.tar", last modified: Sun Apr 21 09:15:47 2024, max compression
```

## Comparing `geminiwrapper-0.0.2.tar` & `geminiwrapper-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 07:27:10.636540 geminiwrapper-0.0.2/
--rw-rw-rw-   0        0        0      459 2024-04-21 07:27:10.636540 geminiwrapper-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-21 00:03:59.000000 geminiwrapper-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 07:27:10.620113 geminiwrapper-0.0.2/geminiwrapper/
--rw-rw-rw-   0        0        0       82 2024-04-21 07:26:39.000000 geminiwrapper-0.0.2/geminiwrapper/__init__.py
--rw-rw-rw-   0        0        0     1425 2024-04-21 01:29:01.000000 geminiwrapper-0.0.2/geminiwrapper/json_wrapper.py
--rw-rw-rw-   0        0        0     2328 2024-04-21 01:09:14.000000 geminiwrapper-0.0.2/geminiwrapper/object_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:27:10.636540 geminiwrapper-0.0.2/geminiwrapper.egg-info/
--rw-rw-rw-   0        0        0      459 2024-04-21 07:27:10.000000 geminiwrapper-0.0.2/geminiwrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-04-21 07:27:10.000000 geminiwrapper-0.0.2/geminiwrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 07:27:10.000000 geminiwrapper-0.0.2/geminiwrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-21 07:27:10.000000 geminiwrapper-0.0.2/geminiwrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-21 07:27:10.000000 geminiwrapper-0.0.2/geminiwrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 07:27:10.636540 geminiwrapper-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      658 2024-04-21 07:27:06.000000 geminiwrapper-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:15:47.353779 geminiwrapper-0.0.3/
+-rw-rw-rw-   0        0        0     3670 2024-04-21 09:15:47.352803 geminiwrapper-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3168 2024-04-21 09:07:04.000000 geminiwrapper-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 09:15:47.331898 geminiwrapper-0.0.3/geminiwrapper/
+-rw-rw-rw-   0        0        0       82 2024-04-21 07:26:39.000000 geminiwrapper-0.0.3/geminiwrapper/__init__.py
+-rw-rw-rw-   0        0        0     1425 2024-04-21 01:29:01.000000 geminiwrapper-0.0.3/geminiwrapper/json_wrapper.py
+-rw-rw-rw-   0        0        0     2328 2024-04-21 01:09:14.000000 geminiwrapper-0.0.3/geminiwrapper/object_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:15:47.351805 geminiwrapper-0.0.3/geminiwrapper.egg-info/
+-rw-rw-rw-   0        0        0     3670 2024-04-21 09:15:47.000000 geminiwrapper-0.0.3/geminiwrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-04-21 09:15:47.000000 geminiwrapper-0.0.3/geminiwrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 09:15:47.000000 geminiwrapper-0.0.3/geminiwrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-21 09:15:47.000000 geminiwrapper-0.0.3/geminiwrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-21 09:15:47.000000 geminiwrapper-0.0.3/geminiwrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 09:15:47.353779 geminiwrapper-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      885 2024-04-21 09:15:42.000000 geminiwrapper-0.0.3/setup.py
```

### Comparing `geminiwrapper-0.0.2/geminiwrapper/json_wrapper.py` & `geminiwrapper-0.0.3/geminiwrapper/json_wrapper.py`

 * *Files identical despite different names*

### Comparing `geminiwrapper-0.0.2/geminiwrapper/object_wrapper.py` & `geminiwrapper-0.0.3/geminiwrapper/object_wrapper.py`

 * *Files identical despite different names*

### Comparing `geminiwrapper-0.0.2/setup.py` & `geminiwrapper-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+import pathlib
 from setuptools import setup, find_packages
 
+here = pathlib.Path(__file__).parent.resolve()
+long_description = (here / "README.md").read_text(encoding="utf-8")
+
 setup(
     name="geminiwrapper",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(),
     install_requires=[
         "google-generativeai",
     ],
     description="Library for generating consistent Gemini API outputs and wrapping them with json and python objects",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     author="Min Htet Naing",
     author_email="minhtetnaing25mhn@gmail.com",
     url="https://github.com/Osbertt-19/gemini-wrapper",
     keywords="gemini, object, json, wrapper, consistent",
     classifiers=[
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Programming Language :: Python",
```


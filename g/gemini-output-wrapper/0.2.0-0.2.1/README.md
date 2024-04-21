# Comparing `tmp/gemini-output-wrapper-0.2.0.tar.gz` & `tmp/gemini-output-wrapper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini-output-wrapper-0.2.0.tar", last modified: Sun Apr 21 02:02:40 2024, max compression
+gzip compressed data, was "gemini-output-wrapper-0.2.1.tar", last modified: Sun Apr 21 02:14:33 2024, max compression
```

## Comparing `gemini-output-wrapper-0.2.0.tar` & `gemini-output-wrapper-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 02:02:40.705665 gemini-output-wrapper-0.2.0/
--rw-rw-rw-   0        0        0      281 2024-04-21 02:02:40.705665 gemini-output-wrapper-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-21 00:03:59.000000 gemini-output-wrapper-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 02:02:40.704673 gemini-output-wrapper-0.2.0/gemini_output_wrapper.egg-info/
--rw-rw-rw-   0        0        0      281 2024-04-21 02:02:40.000000 gemini-output-wrapper-0.2.0/gemini_output_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-04-21 02:02:40.000000 gemini-output-wrapper-0.2.0/gemini_output_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 02:02:40.000000 gemini-output-wrapper-0.2.0/gemini_output_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-21 02:02:40.000000 gemini-output-wrapper-0.2.0/gemini_output_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 02:02:40.000000 gemini-output-wrapper-0.2.0/gemini_output_wrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 02:02:40.706182 gemini-output-wrapper-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      523 2024-04-21 02:00:15.000000 gemini-output-wrapper-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:14:33.725051 gemini-output-wrapper-0.2.1/
+-rw-rw-rw-   0        0        0      305 2024-04-21 02:14:33.724581 gemini-output-wrapper-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-21 00:03:59.000000 gemini-output-wrapper-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 02:14:33.723562 gemini-output-wrapper-0.2.1/gemini_output_wrapper.egg-info/
+-rw-rw-rw-   0        0        0      305 2024-04-21 02:14:33.000000 gemini-output-wrapper-0.2.1/gemini_output_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-04-21 02:14:33.000000 gemini-output-wrapper-0.2.1/gemini_output_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 02:14:33.000000 gemini-output-wrapper-0.2.1/gemini_output_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-21 02:14:33.000000 gemini-output-wrapper-0.2.1/gemini_output_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 02:14:33.000000 gemini-output-wrapper-0.2.1/gemini_output_wrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 02:14:33.725051 gemini-output-wrapper-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      553 2024-04-21 02:12:24.000000 gemini-output-wrapper-0.2.1/setup.py
```

### Comparing `gemini-output-wrapper-0.2.0/setup.py` & `gemini-output-wrapper-0.2.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="gemini-output-wrapper",
-    version="0.2.0",
+    version="0.2.1",
     packages=find_packages(),
+    python_requires=">=3.8",
     install_requires=[
         "importlib",
         "typing",
         "json",
         "google-generativeai",
         "inspect",
     ],
```


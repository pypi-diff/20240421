# Comparing `tmp/gemini-output-wrapper-0.2.1.tar.gz` & `tmp/gemini-output-wrapper-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini-output-wrapper-0.2.1.tar", last modified: Sun Apr 21 02:14:33 2024, max compression
+gzip compressed data, was "gemini-output-wrapper-0.2.2.tar", last modified: Sun Apr 21 02:16:56 2024, max compression
```

## Comparing `gemini-output-wrapper-0.2.1.tar` & `gemini-output-wrapper-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 02:14:33.725051 gemini-output-wrapper-0.2.1/
--rw-rw-rw-   0        0        0      305 2024-04-21 02:14:33.724581 gemini-output-wrapper-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-21 00:03:59.000000 gemini-output-wrapper-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 02:14:33.723562 gemini-output-wrapper-0.2.1/gemini_output_wrapper.egg-info/
--rw-rw-rw-   0        0        0      305 2024-04-21 02:14:33.000000 gemini-output-wrapper-0.2.1/gemini_output_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-04-21 02:14:33.000000 gemini-output-wrapper-0.2.1/gemini_output_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 02:14:33.000000 gemini-output-wrapper-0.2.1/gemini_output_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-21 02:14:33.000000 gemini-output-wrapper-0.2.1/gemini_output_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 02:14:33.000000 gemini-output-wrapper-0.2.1/gemini_output_wrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 02:14:33.725051 gemini-output-wrapper-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      553 2024-04-21 02:12:24.000000 gemini-output-wrapper-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:16:56.243538 gemini-output-wrapper-0.2.2/
+-rw-rw-rw-   0        0        0      305 2024-04-21 02:16:56.243030 gemini-output-wrapper-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-21 00:03:59.000000 gemini-output-wrapper-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 02:16:56.242038 gemini-output-wrapper-0.2.2/gemini_output_wrapper.egg-info/
+-rw-rw-rw-   0        0        0      305 2024-04-21 02:16:56.000000 gemini-output-wrapper-0.2.2/gemini_output_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-04-21 02:16:56.000000 gemini-output-wrapper-0.2.2/gemini_output_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 02:16:56.000000 gemini-output-wrapper-0.2.2/gemini_output_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-21 02:16:56.000000 gemini-output-wrapper-0.2.2/gemini_output_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 02:16:56.000000 gemini-output-wrapper-0.2.2/gemini_output_wrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 02:16:56.244022 gemini-output-wrapper-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      536 2024-04-21 02:16:36.000000 gemini-output-wrapper-0.2.2/setup.py
```

### Comparing `gemini-output-wrapper-0.2.1/setup.py` & `gemini-output-wrapper-0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="gemini-output-wrapper",
-    version="0.2.1",
+    version="0.2.2",
     packages=find_packages(),
     python_requires=">=3.8",
     install_requires=[
         "importlib",
         "typing",
-        "json",
         "google-generativeai",
         "inspect",
     ],
     description="Library for wrapping Gemini API output with Json and Python objects",
     author="Min Htet Naing",
     author_email="minhtetnaing25mhn@gmail.com",
     url="https://github.com/Osbertt-19/gemini-output-wrapper.git",
```


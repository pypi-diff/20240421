# Comparing `tmp/pdf_tools_sdk-1.5.0rc1.tar.gz` & `tmp/pdf_tools_sdk-1.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_tools_sdk-1.5.0rc1.tar", last modified: Sun Apr 21 14:35:40 2024, max compression
+gzip compressed data, was "pdf_tools_sdk-1.5.0rc2.tar", last modified: Sun Apr 21 15:20:04 2024, max compression
```

## Comparing `pdf_tools_sdk-1.5.0rc1.tar` & `pdf_tools_sdk-1.5.0rc2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 14:35:40.057559 pdf_tools_sdk-1.5.0rc1/
--rw-rw-rw-   0        0        0      260 2024-04-21 12:28:42.000000 pdf_tools_sdk-1.5.0rc1/MANIFEST.in
--rw-rw-rw-   0        0        0      105 2024-04-21 14:35:40.053562 pdf_tools_sdk-1.5.0rc1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-21 14:35:39.594448 pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk/
--rw-rw-rw-   0        0        0     3339 2024-04-17 07:20:00.000000 pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk/Streams.py
--rw-rw-rw-   0        0        0        0 2024-04-21 12:28:42.000000 pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 14:35:39.582450 pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk/lib/
-drwxrwxrwx   0        0        0        0 2024-04-21 14:35:39.989176 pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk/lib/win-x64/
--rw-rw-rw-   0        0        0 26051072 2024-04-21 14:23:49.000000 pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk/lib/win-x64/PdfToolsSdk.dll
--rw-rw-rw-   0        0        0   200416 2024-04-21 12:28:42.000000 pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk/py_ctypes.py
--rw-rw-rw-   0        0        0     1491 2024-04-21 12:28:42.000000 pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-21 14:35:40.049554 pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk.egg-info/
--rw-rw-rw-   0        0        0      105 2024-04-21 14:35:39.000000 pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-04-21 14:35:39.000000 pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 14:35:39.000000 pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-21 14:35:39.000000 pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2024-04-21 14:35:39.000000 pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 14:35:40.057559 pdf_tools_sdk-1.5.0rc1/setup.cfg
--rw-rw-rw-   0        0        0      493 2024-04-21 14:03:15.000000 pdf_tools_sdk-1.5.0rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:20:04.286396 pdf_tools_sdk-1.5.0rc2/
+-rw-rw-rw-   0        0        0      260 2024-04-21 12:28:42.000000 pdf_tools_sdk-1.5.0rc2/MANIFEST.in
+-rw-rw-rw-   0        0        0      105 2024-04-21 15:20:04.283395 pdf_tools_sdk-1.5.0rc2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-21 15:20:04.231333 pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk/
+-rw-rw-rw-   0        0        0        0 2024-04-21 12:28:42.000000 pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:20:04.220333 pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk/lib/
+drwxrwxrwx   0        0        0        0 2024-04-21 15:20:04.246864 pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk/lib/win-x64/
+-rw-rw-rw-   0        0        0 26051072 2024-04-21 14:23:49.000000 pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk/lib/win-x64/PdfToolsSdk.dll
+-rw-rw-rw-   0        0        0   200416 2024-04-21 12:28:42.000000 pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk/py_ctypes.py
+-rw-rw-rw-   0        0        0     3339 2024-04-17 07:20:00.000000 pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk/streams.py
+-rw-rw-rw-   0        0        0     1491 2024-04-21 12:28:42.000000 pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:20:04.282389 pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk.egg-info/
+-rw-rw-rw-   0        0        0      105 2024-04-21 15:20:04.000000 pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-04-21 15:20:04.000000 pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 15:20:04.000000 pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-21 15:20:04.000000 pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2024-04-21 15:20:04.000000 pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 15:20:04.287397 pdf_tools_sdk-1.5.0rc2/setup.cfg
+-rw-rw-rw-   0        0        0      493 2024-04-21 15:07:35.000000 pdf_tools_sdk-1.5.0rc2/setup.py
```

### Comparing `pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk/Streams.py` & `pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk/streams.py`

 * *Files identical despite different names*

### Comparing `pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk/lib/win-x64/PdfToolsSdk.dll` & `pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk/lib/win-x64/PdfToolsSdk.dll`

 * *Files identical despite different names*

### Comparing `pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk/py_ctypes.py` & `pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk/py_ctypes.py`

 * *Files identical despite different names*

### Comparing `pdf_tools_sdk-1.5.0rc1/pdf_tools_sdk/utils.py` & `pdf_tools_sdk-1.5.0rc2/pdf_tools_sdk/utils.py`

 * *Files identical despite different names*


# Comparing `tmp/filerev-0.0.1.2.tar.gz` & `tmp/filerev-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filerev-0.0.1.2.tar", max compression
+gzip compressed data, was "filerev-0.0.2.tar", max compression
```

## Comparing `filerev-0.0.1.2.tar` & `filerev-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 filerev-0.0.1.2/LICENSE
--rw-r--r--   0        0        0     1399 2024-04-16 13:14:33.651061 filerev-0.0.1.2/filerev/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 filerev-0.0.1.2/filerev/py.typed
--rw-r--r--   0        0        0     1094 2024-04-16 14:56:55.865739 filerev-0.0.1.2/pyproject.toml
--rw-r--r--   0        0        0      173 2024-04-16 13:03:42.719892 filerev-0.0.1.2/readme.md
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 filerev-0.0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 filerev-0.0.2/LICENSE
+-rwxr-xr-x   0        0        0     1399 2024-04-21 16:18:32.073685 filerev-0.0.2/filerev/__init__.py
+-rw-r--r--   0        0        0     1027 2024-04-21 16:18:05.226697 filerev-0.0.2/filerev/__main__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 filerev-0.0.2/filerev/py.typed
+-rw-r--r--   0        0        0     1137 2024-04-21 16:18:40.016617 filerev-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      173 2024-04-16 13:03:42.719892 filerev-0.0.2/readme.md
+-rw-r--r--   0        0        0     1289 1970-01-01 00:00:00.000000 filerev-0.0.2/PKG-INFO
```

### Comparing `filerev-0.0.1.2/LICENSE` & `filerev-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `filerev-0.0.1.2/filerev/__init__.py` & `filerev-0.0.2/filerev/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 1)
+__version__ = (0, 0, 2)
 __all__ = ["file_reviter"]
 
 
 from collections.abc import Generator, Iterator
 from io import TextIOWrapper
 from typing import overload, BinaryIO
```

### Comparing `filerev-0.0.1.2/pyproject.toml` & `filerev-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "filerev"
-version = "0.0.1.2"
+version = "0.0.2"
 description = "Reversed iterator for files."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/filerev"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/filerev"
 keywords = ["file", "reverse", "iter"]
@@ -21,13 +21,16 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = [
     "LICENSE",
 ]
 
+[tool.poetry.dependencies]
+python = "^3.10"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.packages]]
 include = "filerev"
```


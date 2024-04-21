# Comparing `tmp/mytestpkgfranktcao-0.1.0.tar.gz` & `tmp/mytestpkgfranktcao-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mytestpkgfranktcao-0.1.0.tar", max compression
+gzip compressed data, was "mytestpkgfranktcao-0.1.1.tar", max compression
```

## Comparing `mytestpkgfranktcao-0.1.0.tar` & `mytestpkgfranktcao-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1068 2024-04-20 21:50:45.919993 mytestpkgfranktcao-0.1.0/LICENSE
--rw-r--r--   0        0        0      627 2024-04-20 21:50:45.930404 mytestpkgfranktcao-0.1.0/README.md
--rw-r--r--   0        0        0      705 2024-04-20 23:57:42.177045 mytestpkgfranktcao-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      111 2024-04-20 21:50:45.961683 mytestpkgfranktcao-0.1.0/src/mytestpkgfranktcao/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 23:42:07.777774 mytestpkgfranktcao-0.1.0/src/mytestpkgfranktcao/mytestpkg.py
--rw-r--r--   0        0        0     1025 1970-01-01 00:00:00.000000 mytestpkgfranktcao-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1068 2024-04-20 21:50:45.919993 mytestpkgfranktcao-0.1.1/LICENSE
+-rw-r--r--   0        0        0      627 2024-04-20 21:50:45.930404 mytestpkgfranktcao-0.1.1/README.md
+-rw-r--r--   0        0        0      705 2024-04-20 23:58:48.920529 mytestpkgfranktcao-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      111 2024-04-20 21:50:45.961683 mytestpkgfranktcao-0.1.1/src/mytestpkgfranktcao/__init__.py
+-rw-r--r--   0        0        0       36 2024-04-20 23:58:41.006471 mytestpkgfranktcao-0.1.1/src/mytestpkgfranktcao/mytestpkg.py
+-rw-r--r--   0        0        0     1025 1970-01-01 00:00:00.000000 mytestpkgfranktcao-0.1.1/PKG-INFO
```

### Comparing `mytestpkgfranktcao-0.1.0/LICENSE` & `mytestpkgfranktcao-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mytestpkgfranktcao-0.1.0/README.md` & `mytestpkgfranktcao-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mytestpkgfranktcao-0.1.0/pyproject.toml` & `mytestpkgfranktcao-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mytestpkgfranktcao"
-version = "0.1.0"
+version = "0.1.1"
 description = "Test publishing on PyPI"
 authors = ["Frank Cao"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `mytestpkgfranktcao-0.1.0/PKG-INFO` & `mytestpkgfranktcao-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mytestpkgfranktcao
-Version: 0.1.0
+Version: 0.1.1
 Summary: Test publishing on PyPI
 License: MIT
 Author: Frank Cao
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```


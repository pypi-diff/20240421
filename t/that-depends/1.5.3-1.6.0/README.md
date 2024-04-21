# Comparing `tmp/that_depends-1.5.3.tar.gz` & `tmp/that_depends-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "that_depends-1.5.3.tar", max compression
+gzip compressed data, was "that_depends-1.6.0.tar", max compression
```

## Comparing `that_depends-1.5.3.tar` & `that_depends-1.6.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     6711 2024-04-16 18:31:17.949107 that_depends-1.5.3/README.md
--rw-r--r--   0        0        0     1482 2024-04-17 05:55:36.116872 that_depends-1.5.3/pyproject.toml
--rw-r--r--   0        0        0      164 2024-03-18 09:15:04.223171 that_depends-1.5.3/that_depends/__init__.py
--rw-r--r--   0        0        0      747 2024-04-11 11:51:20.009107 that_depends-1.5.3/that_depends/container.py
--rw-r--r--   0        0        0     1013 2024-04-15 19:32:21.955087 that_depends-1.5.3/that_depends/injection.py
--rw-r--r--   0        0        0      484 2024-04-16 06:00:55.731335 that_depends-1.5.3/that_depends/providers/__init__.py
--rw-r--r--   0        0        0      642 2024-04-16 06:00:18.298948 that_depends-1.5.3/that_depends/providers/base.py
--rw-r--r--   0        0        0      465 2024-04-16 06:00:22.046508 that_depends-1.5.3/that_depends/providers/collections.py
--rw-r--r--   0        0        0     1365 2024-04-16 06:00:22.046739 that_depends-1.5.3/that_depends/providers/factories.py
--rw-r--r--   0        0        0     2584 2024-04-17 05:54:39.373410 that_depends-1.5.3/that_depends/providers/resources.py
--rw-r--r--   0        0        0      993 2024-04-17 05:36:03.299156 that_depends-1.5.3/that_depends/providers/singleton.py
--rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.5.3/that_depends/py.typed
--rw-r--r--   0        0        0     7191 1970-01-01 00:00:00.000000 that_depends-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     6711 2024-04-16 18:31:17.949107 that_depends-1.6.0/README.md
+-rw-r--r--   0        0        0     1482 2024-04-21 11:37:07.035917 that_depends-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      164 2024-03-18 09:15:04.223171 that_depends-1.6.0/that_depends/__init__.py
+-rw-r--r--   0        0        0      747 2024-04-11 11:51:20.009107 that_depends-1.6.0/that_depends/container.py
+-rw-r--r--   0        0        0     1013 2024-04-15 19:32:21.955087 that_depends-1.6.0/that_depends/injection.py
+-rw-r--r--   0        0        0      670 2024-04-21 11:20:54.815386 that_depends-1.6.0/that_depends/providers/__init__.py
+-rw-r--r--   0        0        0      642 2024-04-16 06:00:18.298948 that_depends-1.6.0/that_depends/providers/base.py
+-rw-r--r--   0        0        0      465 2024-04-16 06:00:22.046508 that_depends-1.6.0/that_depends/providers/collections.py
+-rw-r--r--   0        0        0     3023 2024-04-21 11:29:23.822434 that_depends-1.6.0/that_depends/providers/context_resources.py
+-rw-r--r--   0        0        0     1365 2024-04-16 06:00:22.046739 that_depends-1.6.0/that_depends/providers/factories.py
+-rw-r--r--   0        0        0     2584 2024-04-19 13:06:26.477052 that_depends-1.6.0/that_depends/providers/resources.py
+-rw-r--r--   0        0        0      993 2024-04-17 05:36:03.299156 that_depends-1.6.0/that_depends/providers/singleton.py
+-rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.6.0/that_depends/py.typed
+-rw-r--r--   0        0        0     7191 1970-01-01 00:00:00.000000 that_depends-1.6.0/PKG-INFO
```

### Comparing `that_depends-1.5.3/README.md` & `that_depends-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `that_depends-1.5.3/pyproject.toml` & `that_depends-1.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "that-depends"
-version = "1.5.3"
+version = "1.6.0"
 description = "Simple Dependency Injection framework"
 authors = ["Artur Shiriev <me@shiriev.ru>"]
 readme = "README.md"
 homepage = "https://github.com/modern-python/that-depends"
 packages = [
     { include = "that_depends" },
 ]
```

### Comparing `that_depends-1.5.3/that_depends/container.py` & `that_depends-1.6.0/that_depends/container.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.5.3/that_depends/injection.py` & `that_depends-1.6.0/that_depends/injection.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.5.3/that_depends/providers/base.py` & `that_depends-1.6.0/that_depends/providers/base.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.5.3/that_depends/providers/factories.py` & `that_depends-1.6.0/that_depends/providers/factories.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.5.3/that_depends/providers/resources.py` & `that_depends-1.6.0/that_depends/providers/resources.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.5.3/that_depends/providers/singleton.py` & `that_depends-1.6.0/that_depends/providers/singleton.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.5.3/PKG-INFO` & `that_depends-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: that-depends
-Version: 1.5.3
+Version: 1.6.0
 Summary: Simple Dependency Injection framework
 Home-page: https://github.com/modern-python/that-depends
 Author: Artur Shiriev
 Author-email: me@shiriev.ru
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```


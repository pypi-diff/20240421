# Comparing `tmp/shinylive_auth-2024.4.20.tar.gz` & `tmp/shinylive_auth-2024.4.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinylive_auth-2024.4.20.tar", last modified: Sun Apr 21 02:32:09 2024, max compression
+gzip compressed data, was "shinylive_auth-2024.4.21.tar", last modified: Sun Apr 21 02:45:57 2024, max compression
```

## Comparing `shinylive_auth-2024.4.20.tar` & `shinylive_auth-2024.4.21.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:32:09.299233 shinylive_auth-2024.4.20/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 02:32:04.000000 shinylive_auth-2024.4.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-21 02:32:09.295233 shinylive_auth-2024.4.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-21 02:32:04.000000 shinylive_auth-2024.4.20/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-21 02:32:04.000000 shinylive_auth-2024.4.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 02:32:09.299233 shinylive_auth-2024.4.20/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:32:09.295233 shinylive_auth-2024.4.20/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:32:09.295233 shinylive_auth-2024.4.20/src/shinylive_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-21 02:32:09.000000 shinylive_auth-2024.4.20/src/shinylive_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-21 02:32:09.000000 shinylive_auth-2024.4.20/src/shinylive_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 02:32:09.000000 shinylive_auth-2024.4.20/src/shinylive_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-21 02:32:09.000000 shinylive_auth-2024.4.20/src/shinylive_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 02:32:09.000000 shinylive_auth-2024.4.20/src/shinylive_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-21 02:32:04.000000 shinylive_auth-2024.4.20/src/shinylive_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:45:57.826335 shinylive_auth-2024.4.21/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 02:45:52.000000 shinylive_auth-2024.4.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-21 02:45:57.822334 shinylive_auth-2024.4.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-21 02:45:52.000000 shinylive_auth-2024.4.21/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-21 02:45:52.000000 shinylive_auth-2024.4.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 02:45:57.826335 shinylive_auth-2024.4.21/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:45:57.822334 shinylive_auth-2024.4.21/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:45:57.822334 shinylive_auth-2024.4.21/src/shinylive_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-21 02:45:57.000000 shinylive_auth-2024.4.21/src/shinylive_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-21 02:45:57.000000 shinylive_auth-2024.4.21/src/shinylive_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 02:45:57.000000 shinylive_auth-2024.4.21/src/shinylive_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-21 02:45:57.000000 shinylive_auth-2024.4.21/src/shinylive_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 02:45:57.000000 shinylive_auth-2024.4.21/src/shinylive_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-21 02:45:52.000000 shinylive_auth-2024.4.21/src/shinylive_auth.py
```

### Comparing `shinylive_auth-2024.4.20/LICENSE` & `shinylive_auth-2024.4.21/LICENSE`

 * *Files identical despite different names*

### Comparing `shinylive_auth-2024.4.20/PKG-INFO` & `shinylive_auth-2024.4.21/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: shinylive_auth
-Version: 2024.4.20
+Version: 2024.4.21
 Summary: View and server modules to facility shinylive authentication using a class protocal and local storage.
 Author-email: darrida <darrida.py@gmail.com>
 Project-URL: Homepage, https://github.com/darrida/py-shinylive-authentication
 Project-URL: Issues, https://github.com/darrida/py-shinylive-authentication/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: shiny
-Requires-Dist: shinylive
 Requires-Dist: shinyswatch
 Requires-Dist: pydantic<2.0
 Requires-Dist: python_version<=3.8
 Provides-Extra: tests
 Requires-Dist: fastapi; extra == "tests"
 Requires-Dist: loguru; extra == "tests"
 Requires-Dist: pyfetch_mimic==0.0.3; extra == "tests"
 Requires-Dist: httpx; extra == "tests"
+Requires-Dist: shinylive; extra == "tests"
 
 # py-shinylive-authentication
 
 ## Preliminary Release
 - Documentation is scarse at this point. 
 - For usage, see docstrings on the `src.shiny_auth.AuthProtocol` class methods.
 - For examples, see code in:
```

### Comparing `shinylive_auth-2024.4.20/pyproject.toml` & `shinylive_auth-2024.4.21/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [project]
 name = "shinylive_auth"
-version = "2024.04.20"
+version = "2024.04.21"
 authors = [
   {name="darrida", email="darrida.py@gmail.com"}
 ]
 description = "View and server modules to facility shinylive authentication using a class protocal and local storage."
 readme = "README.md"
 
 dependencies = [
   'shiny',
-  'shinylive',
   'shinyswatch',
   'pydantic < 2.0',
   'python_version <= 3.8',
 ]
 
 [project.optional-dependencies]
 tests = [
   'fastapi',
   'loguru',
   'pyfetch_mimic == 0.0.3',
-  'httpx'
+  'httpx',
+  'shinylive'
 ]
 
 [project.urls]
 Homepage = "https://github.com/darrida/py-shinylive-authentication"
 Issues = "https://github.com/darrida/py-shinylive-authentication/issues"
 
 [build-system]
```

### Comparing `shinylive_auth-2024.4.20/src/shinylive_auth.egg-info/PKG-INFO` & `shinylive_auth-2024.4.21/src/shinylive_auth.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: shinylive_auth
-Version: 2024.4.20
+Version: 2024.4.21
 Summary: View and server modules to facility shinylive authentication using a class protocal and local storage.
 Author-email: darrida <darrida.py@gmail.com>
 Project-URL: Homepage, https://github.com/darrida/py-shinylive-authentication
 Project-URL: Issues, https://github.com/darrida/py-shinylive-authentication/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: shiny
-Requires-Dist: shinylive
 Requires-Dist: shinyswatch
 Requires-Dist: pydantic<2.0
 Requires-Dist: python_version<=3.8
 Provides-Extra: tests
 Requires-Dist: fastapi; extra == "tests"
 Requires-Dist: loguru; extra == "tests"
 Requires-Dist: pyfetch_mimic==0.0.3; extra == "tests"
 Requires-Dist: httpx; extra == "tests"
+Requires-Dist: shinylive; extra == "tests"
 
 # py-shinylive-authentication
 
 ## Preliminary Release
 - Documentation is scarse at this point. 
 - For usage, see docstrings on the `src.shiny_auth.AuthProtocol` class methods.
 - For examples, see code in:
```

### Comparing `shinylive_auth-2024.4.20/src/shinylive_auth.py` & `shinylive_auth-2024.4.21/src/shinylive_auth.py`

 * *Files identical despite different names*


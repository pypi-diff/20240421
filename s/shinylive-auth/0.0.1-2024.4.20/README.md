# Comparing `tmp/shinylive_auth-0.0.1.tar.gz` & `tmp/shinylive_auth-2024.4.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinylive_auth-0.0.1.tar", last modified: Sun Mar 24 23:37:56 2024, max compression
+gzip compressed data, was "shinylive_auth-2024.4.20.tar", last modified: Sun Apr 21 02:32:09 2024, max compression
```

## Comparing `shinylive_auth-0.0.1.tar` & `shinylive_auth-2024.4.20.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:37:56.084800 shinylive_auth-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-24 23:37:49.000000 shinylive_auth-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-24 23:37:56.084800 shinylive_auth-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-24 23:37:49.000000 shinylive_auth-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-24 23:37:49.000000 shinylive_auth-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 23:37:56.084800 shinylive_auth-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:37:56.084800 shinylive_auth-0.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-03-24 23:37:49.000000 shinylive_auth-0.0.1/src/shiny_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:37:56.084800 shinylive_auth-0.0.1/src/shinylive_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-24 23:37:56.000000 shinylive_auth-0.0.1/src/shinylive_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-24 23:37:56.000000 shinylive_auth-0.0.1/src/shinylive_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 23:37:56.000000 shinylive_auth-0.0.1/src/shinylive_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-24 23:37:56.000000 shinylive_auth-0.0.1/src/shinylive_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-24 23:37:56.000000 shinylive_auth-0.0.1/src/shinylive_auth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:32:09.299233 shinylive_auth-2024.4.20/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 02:32:04.000000 shinylive_auth-2024.4.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-21 02:32:09.295233 shinylive_auth-2024.4.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-21 02:32:04.000000 shinylive_auth-2024.4.20/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-21 02:32:04.000000 shinylive_auth-2024.4.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 02:32:09.299233 shinylive_auth-2024.4.20/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:32:09.295233 shinylive_auth-2024.4.20/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:32:09.295233 shinylive_auth-2024.4.20/src/shinylive_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-21 02:32:09.000000 shinylive_auth-2024.4.20/src/shinylive_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-21 02:32:09.000000 shinylive_auth-2024.4.20/src/shinylive_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 02:32:09.000000 shinylive_auth-2024.4.20/src/shinylive_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-21 02:32:09.000000 shinylive_auth-2024.4.20/src/shinylive_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 02:32:09.000000 shinylive_auth-2024.4.20/src/shinylive_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-21 02:32:04.000000 shinylive_auth-2024.4.20/src/shinylive_auth.py
```

### Comparing `shinylive_auth-0.0.1/LICENSE` & `shinylive_auth-2024.4.20/LICENSE`

 * *Files identical despite different names*

### Comparing `shinylive_auth-0.0.1/PKG-INFO` & `shinylive_auth-2024.4.20/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: shinylive_auth
-Version: 0.0.1
+Version: 2024.4.20
 Summary: View and server modules to facility shinylive authentication using a class protocal and local storage.
 Author-email: darrida <darrida.py@gmail.com>
 Project-URL: Homepage, https://github.com/darrida/py-shinylive-authentication
 Project-URL: Issues, https://github.com/darrida/py-shinylive-authentication/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: shiny
 Requires-Dist: shinylive
 Requires-Dist: shinyswatch
 Requires-Dist: pydantic<2.0
 Requires-Dist: python_version<=3.8
 Provides-Extra: tests
 Requires-Dist: fastapi; extra == "tests"
 Requires-Dist: loguru; extra == "tests"
-Requires-Dist: pyfetch_mimic==0.0.1; extra == "tests"
+Requires-Dist: pyfetch_mimic==0.0.3; extra == "tests"
 Requires-Dist: httpx; extra == "tests"
 
 # py-shinylive-authentication
 
 ## Preliminary Release
 - Documentation is scarse at this point. 
 - For usage, see docstrings on the `src.shiny_auth.AuthProtocol` class methods.
```

### Comparing `shinylive_auth-0.0.1/pyproject.toml` & `shinylive_auth-2024.4.20/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "shinylive_auth"
-version = "0.0.1"
+version = "2024.04.20"
 authors = [
   {name="darrida", email="darrida.py@gmail.com"}
 ]
 description = "View and server modules to facility shinylive authentication using a class protocal and local storage."
 readme = "README.md"
 
 dependencies = [
@@ -15,15 +15,15 @@
   'python_version <= 3.8',
 ]
 
 [project.optional-dependencies]
 tests = [
   'fastapi',
   'loguru',
-  'pyfetch_mimic == 0.0.1',
+  'pyfetch_mimic == 0.0.3',
   'httpx'
 ]
 
 [project.urls]
 Homepage = "https://github.com/darrida/py-shinylive-authentication"
 Issues = "https://github.com/darrida/py-shinylive-authentication/issues"
```

### Comparing `shinylive_auth-0.0.1/src/shiny_auth.py` & `shinylive_auth-2024.4.20/src/shinylive_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
             ui.notification_show("'username' and 'password' fields are both required.", type="warning")
             return
         
         # Use `AuthProtocol.get_auth` to validate provided credentials
         try:
             token = await app_auth.get_auth(username, password)
         except app_auth.ShinyLiveAuthFailed:
-            ui.notification_show("Invalud username or password", type="warning")
+            ui.notification_show("Invalid username or password", type="warning")
             return
         except app_auth.ShinyLivePermissions:
             ui.notification_show("Insufficient permissions. Check with IT and then try again.", type="warning")
             session_auth.login_prompt.set(True)
             return
 
         # Code to return/assign a token here (i.e., an endpoint that produces JWT)
```

### Comparing `shinylive_auth-0.0.1/src/shinylive_auth.egg-info/PKG-INFO` & `shinylive_auth-2024.4.20/src/shinylive_auth.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: shinylive_auth
-Version: 0.0.1
+Version: 2024.4.20
 Summary: View and server modules to facility shinylive authentication using a class protocal and local storage.
 Author-email: darrida <darrida.py@gmail.com>
 Project-URL: Homepage, https://github.com/darrida/py-shinylive-authentication
 Project-URL: Issues, https://github.com/darrida/py-shinylive-authentication/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: shiny
 Requires-Dist: shinylive
 Requires-Dist: shinyswatch
 Requires-Dist: pydantic<2.0
 Requires-Dist: python_version<=3.8
 Provides-Extra: tests
 Requires-Dist: fastapi; extra == "tests"
 Requires-Dist: loguru; extra == "tests"
-Requires-Dist: pyfetch_mimic==0.0.1; extra == "tests"
+Requires-Dist: pyfetch_mimic==0.0.3; extra == "tests"
 Requires-Dist: httpx; extra == "tests"
 
 # py-shinylive-authentication
 
 ## Preliminary Release
 - Documentation is scarse at this point. 
 - For usage, see docstrings on the `src.shiny_auth.AuthProtocol` class methods.
```


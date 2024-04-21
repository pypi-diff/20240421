# Comparing `tmp/lichesspy-6.0.3.tar.gz` & `tmp/lichesspy-6.0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lichesspy-6.0.3.tar", last modified: Sun Apr 21 03:52:06 2024, max compression
+gzip compressed data, was "lichesspy-6.0.4.dev0.tar", last modified: Sun Apr 21 17:58:41 2024, max compression
```

## Comparing `lichesspy-6.0.3.tar` & `lichesspy-6.0.4.dev0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:52:06.571783 lichesspy-6.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 03:52:01.000000 lichesspy-6.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-21 03:52:06.571783 lichesspy-6.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-21 03:52:01.000000 lichesspy-6.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:52:06.571783 lichesspy-6.0.3/lichesspy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:52:01.000000 lichesspy-6.0.3/lichesspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14355 2024-04-21 03:52:01.000000 lichesspy-6.0.3/lichesspy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-21 03:52:01.000000 lichesspy-6.0.3/lichesspy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-21 03:52:01.000000 lichesspy-6.0.3/lichesspy/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-21 03:52:01.000000 lichesspy-6.0.3/lichesspy/pgn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:52:06.571783 lichesspy-6.0.3/lichesspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-21 03:52:06.000000 lichesspy-6.0.3/lichesspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 03:52:06.000000 lichesspy-6.0.3/lichesspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 03:52:06.000000 lichesspy-6.0.3/lichesspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-21 03:52:06.000000 lichesspy-6.0.3/lichesspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 03:52:06.000000 lichesspy-6.0.3/lichesspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 03:52:06.571783 lichesspy-6.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-21 03:52:01.000000 lichesspy-6.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:58:41.397268 lichesspy-6.0.4.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 17:58:36.000000 lichesspy-6.0.4.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-21 17:58:41.397268 lichesspy-6.0.4.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-21 17:58:36.000000 lichesspy-6.0.4.dev0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:58:41.397268 lichesspy-6.0.4.dev0/lichesspy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 17:58:36.000000 lichesspy-6.0.4.dev0/lichesspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-04-21 17:58:36.000000 lichesspy-6.0.4.dev0/lichesspy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-21 17:58:36.000000 lichesspy-6.0.4.dev0/lichesspy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-21 17:58:36.000000 lichesspy-6.0.4.dev0/lichesspy/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-21 17:58:36.000000 lichesspy-6.0.4.dev0/lichesspy/pgn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:58:41.397268 lichesspy-6.0.4.dev0/lichesspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-21 17:58:41.000000 lichesspy-6.0.4.dev0/lichesspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 17:58:41.000000 lichesspy-6.0.4.dev0/lichesspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 17:58:41.000000 lichesspy-6.0.4.dev0/lichesspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-21 17:58:41.000000 lichesspy-6.0.4.dev0/lichesspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 17:58:41.000000 lichesspy-6.0.4.dev0/lichesspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 17:58:41.397268 lichesspy-6.0.4.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-21 17:58:36.000000 lichesspy-6.0.4.dev0/setup.py
```

### Comparing `lichesspy-6.0.3/LICENSE` & `lichesspy-6.0.4.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.3/PKG-INFO` & `lichesspy-6.0.4.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: lichesspy
-Version: 6.0.3
+Version: 6.0.4.dev0
 Summary: Python wrapper for lichess
 Home-page: https://github.com/eskopp/lichesspy
 Author: eskopp
 Author-email: skopp.erik@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-Requires-Dist: six>=1.16.0
-Requires-Dist: python-chess>=1.999
-Requires-Dist: chess>=1.10.0
+Requires-Dist: requests==2.31.0
+Requires-Dist: six==1.16.0
+Requires-Dist: python-chess==1.999
+Requires-Dist: chess==1.10.0
 
 A client for the lichess.org API
 ================================================
 This is a client library for the Lichess API.
 It is designed to be:
 
 * Easy to use
@@ -79,7 +79,10 @@
 ```
 
 Installing
 ----------
 ```shell
 pip install lichesspy
 ```
+
+
+# Farewell
```

### Comparing `lichesspy-6.0.3/README.rst` & `lichesspy-6.0.4.dev0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -60,7 +60,10 @@
 ```
 
 Installing
 ----------
 ```shell
 pip install lichesspy
 ```
+
+
+# Farewell
```

### Comparing `lichesspy-6.0.3/lichesspy/api.py` & `lichesspy-6.0.4.dev0/lichesspy/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 class DefaultApiClient(object):
     """
     The default API client, with immediate HTTP calls and basic rate-limiting functionality.
     """
 
     _first_call = True
 
-    base_url = "https://lichesspy.org/"
+    base_url = "https://lichess.org/"
     """The base lichess API URL.
 
     This does not include the /api/ prefix, since some APIs don't use it.
     """
 
     max_retries = -1
     """The maximum number of retries after rate-limiting before an exception is raised. -1 for infinite retries."""
```

### Comparing `lichesspy-6.0.3/lichesspy/format.py` & `lichesspy-6.0.4.dev0/lichesspy/format.py`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.3/lichesspy/pgn.py` & `lichesspy-6.0.4.dev0/lichesspy/pgn.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,25 +38,25 @@
         raise ValueError(
             "The provided game doesn't have any moves. Maybe you forgot to set with_moves=1 on the API call?"
         )
 
     result = (
         "1/2-1/2"
         if _node(g, "status") == "draw"
-        else (
-            "1-0"
-            if _node(g, "winner") == "white"
-            else "0-1" if _node(g, "winner") == "black" else "*"
-        )
+        else "1-0"
+        if _node(g, "winner") == "white"
+        else "0-1"
+        if _node(g, "winner") == "black"
+        else "*"
     )
     h = []
     h.append(
         ("Event", "%s %s game" % ("Rated" if g["rated"] else "Casual", g["speed"]))
     )
-    h.append(("Site", "https://lichesspy.org/%s" % g["id"]))
+    h.append(("Site", "https://lichess.org/%s" % g["id"]))
     h.append(
         (
             "Date",
             datetime.fromtimestamp(int(g["createdAt"]) / 1000.0).strftime("%Y.%m.%d"),
         )
     )
     h.append(("Round", "?"))
```

### Comparing `lichesspy-6.0.3/lichesspy.egg-info/PKG-INFO` & `lichesspy-6.0.4.dev0/lichesspy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: lichesspy
-Version: 6.0.3
+Version: 6.0.4.dev0
 Summary: Python wrapper for lichess
 Home-page: https://github.com/eskopp/lichesspy
 Author: eskopp
 Author-email: skopp.erik@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-Requires-Dist: six>=1.16.0
-Requires-Dist: python-chess>=1.999
-Requires-Dist: chess>=1.10.0
+Requires-Dist: requests==2.31.0
+Requires-Dist: six==1.16.0
+Requires-Dist: python-chess==1.999
+Requires-Dist: chess==1.10.0
 
 A client for the lichess.org API
 ================================================
 This is a client library for the Lichess API.
 It is designed to be:
 
 * Easy to use
@@ -79,7 +79,10 @@
 ```
 
 Installing
 ----------
 ```shell
 pip install lichesspy
 ```
+
+
+# Farewell
```


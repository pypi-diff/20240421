# Comparing `tmp/lichesspy-6.0.4.dev1.tar.gz` & `tmp/lichesspy-6.0.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lichesspy-6.0.4.dev1.tar", last modified: Sun Apr 21 18:28:06 2024, max compression
+gzip compressed data, was "lichesspy-6.0.4.dev2.tar", last modified: Sun Apr 21 18:57:01 2024, max compression
```

## Comparing `lichesspy-6.0.4.dev1.tar` & `lichesspy-6.0.4.dev2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:28:06.803569 lichesspy-6.0.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 18:28:01.000000 lichesspy-6.0.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-21 18:28:06.803569 lichesspy-6.0.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-21 18:28:01.000000 lichesspy-6.0.4.dev1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:28:06.803569 lichesspy-6.0.4.dev1/lichesspy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:28:01.000000 lichesspy-6.0.4.dev1/lichesspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14310 2024-04-21 18:28:01.000000 lichesspy-6.0.4.dev1/lichesspy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-21 18:28:01.000000 lichesspy-6.0.4.dev1/lichesspy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-21 18:28:01.000000 lichesspy-6.0.4.dev1/lichesspy/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-21 18:28:01.000000 lichesspy-6.0.4.dev1/lichesspy/pgn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:28:06.803569 lichesspy-6.0.4.dev1/lichesspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-21 18:28:06.000000 lichesspy-6.0.4.dev1/lichesspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 18:28:06.000000 lichesspy-6.0.4.dev1/lichesspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 18:28:06.000000 lichesspy-6.0.4.dev1/lichesspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-21 18:28:06.000000 lichesspy-6.0.4.dev1/lichesspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 18:28:06.000000 lichesspy-6.0.4.dev1/lichesspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 18:28:06.803569 lichesspy-6.0.4.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-21 18:28:01.000000 lichesspy-6.0.4.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:57:01.040243 lichesspy-6.0.4.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 18:56:55.000000 lichesspy-6.0.4.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-21 18:57:01.040243 lichesspy-6.0.4.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-21 18:56:55.000000 lichesspy-6.0.4.dev2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:57:01.036242 lichesspy-6.0.4.dev2/lichesspy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:56:55.000000 lichesspy-6.0.4.dev2/lichesspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14310 2024-04-21 18:56:55.000000 lichesspy-6.0.4.dev2/lichesspy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-21 18:56:55.000000 lichesspy-6.0.4.dev2/lichesspy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-21 18:56:55.000000 lichesspy-6.0.4.dev2/lichesspy/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-21 18:56:55.000000 lichesspy-6.0.4.dev2/lichesspy/pgn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:57:01.040243 lichesspy-6.0.4.dev2/lichesspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-21 18:57:01.000000 lichesspy-6.0.4.dev2/lichesspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 18:57:01.000000 lichesspy-6.0.4.dev2/lichesspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 18:57:01.000000 lichesspy-6.0.4.dev2/lichesspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-21 18:57:01.000000 lichesspy-6.0.4.dev2/lichesspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 18:57:01.000000 lichesspy-6.0.4.dev2/lichesspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 18:57:01.040243 lichesspy-6.0.4.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-21 18:56:55.000000 lichesspy-6.0.4.dev2/setup.py
```

### Comparing `lichesspy-6.0.4.dev1/LICENSE` & `lichesspy-6.0.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.4.dev1/PKG-INFO` & `lichesspy-6.0.4.dev2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lichesspy
-Version: 6.0.4.dev1
+Version: 6.0.4.dev2
 Summary: Python wrapper for lichess
 Home-page: https://github.com/eskopp/lichesspy
 Author: eskopp
-Author-email: skopp.erik@gmail.com
+Author-email: skopp.erik+lichesspy@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -39,16 +39,16 @@
 ```
 Checking who's online and playing:
 
 ```python
 >>> import lichesspy.api
 >>>
 >>> users = list(lichesspy.api.users_status(['thibault', 'cyanfish']))
->>> online = [u['id'] for u in users if u['online']]
->>> playing = [u['id'] for u in users if u['playing']]
+>>> online = [u['id'] for u in users if u.get('online', False)]
+>>> playing = [u['id'] for u in users if u.get('playing', False)]
 >>> print(online, playing)
 ['thibault', 'cyanfish'] ['cyanfish']
 ```
 
 Saving a PGN of a user's last 200 games:
 
 ```python
```

### Comparing `lichesspy-6.0.4.dev1/README.rst` & `lichesspy-6.0.4.dev2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 ```
 Checking who's online and playing:
 
 ```python
 >>> import lichesspy.api
 >>>
 >>> users = list(lichesspy.api.users_status(['thibault', 'cyanfish']))
->>> online = [u['id'] for u in users if u['online']]
->>> playing = [u['id'] for u in users if u['playing']]
+>>> online = [u['id'] for u in users if u.get('online', False)]
+>>> playing = [u['id'] for u in users if u.get('playing', False)]
 >>> print(online, playing)
 ['thibault', 'cyanfish'] ['cyanfish']
 ```
 
 Saving a PGN of a user's last 200 games:
 
 ```python
```

### Comparing `lichesspy-6.0.4.dev1/lichesspy/api.py` & `lichesspy-6.0.4.dev2/lichesspy/api.py`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.4.dev1/lichesspy/format.py` & `lichesspy-6.0.4.dev2/lichesspy/format.py`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.4.dev1/lichesspy/pgn.py` & `lichesspy-6.0.4.dev2/lichesspy/pgn.py`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.4.dev1/lichesspy.egg-info/PKG-INFO` & `lichesspy-6.0.4.dev2/lichesspy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lichesspy
-Version: 6.0.4.dev1
+Version: 6.0.4.dev2
 Summary: Python wrapper for lichess
 Home-page: https://github.com/eskopp/lichesspy
 Author: eskopp
-Author-email: skopp.erik@gmail.com
+Author-email: skopp.erik+lichesspy@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -39,16 +39,16 @@
 ```
 Checking who's online and playing:
 
 ```python
 >>> import lichesspy.api
 >>>
 >>> users = list(lichesspy.api.users_status(['thibault', 'cyanfish']))
->>> online = [u['id'] for u in users if u['online']]
->>> playing = [u['id'] for u in users if u['playing']]
+>>> online = [u['id'] for u in users if u.get('online', False)]
+>>> playing = [u['id'] for u in users if u.get('playing', False)]
 >>> print(online, playing)
 ['thibault', 'cyanfish'] ['cyanfish']
 ```
 
 Saving a PGN of a user's last 200 games:
 
 ```python
```


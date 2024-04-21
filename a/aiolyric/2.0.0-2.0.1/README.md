# Comparing `tmp/aiolyric-2.0.0.tar.gz` & `tmp/aiolyric-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiolyric-2.0.0.tar", last modified: Mon Apr  1 13:38:37 2024, max compression
+gzip compressed data, was "aiolyric-2.0.1.tar", last modified: Sun Apr 21 18:38:09 2024, max compression
```

## Comparing `aiolyric-2.0.0.tar` & `aiolyric-2.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:38:37.892058 aiolyric-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 13:38:16.000000 aiolyric-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-01 13:38:37.892058 aiolyric-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-01 13:38:16.000000 aiolyric-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:38:37.888058 aiolyric-2.0.0/aiolyric/
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:38:37.888058 aiolyric-2.0.0/aiolyric/objects/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/objects/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/objects/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/objects/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/objects/priority.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:38:37.892058 aiolyric-2.0.0/aiolyric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-01 13:38:37.000000 aiolyric-2.0.0/aiolyric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-01 13:38:37.000000 aiolyric-2.0.0/aiolyric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:38:37.000000 aiolyric-2.0.0/aiolyric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-01 13:38:37.000000 aiolyric-2.0.0/aiolyric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 13:38:37.000000 aiolyric-2.0.0/aiolyric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-04-01 13:38:16.000000 aiolyric-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:38:37.892058 aiolyric-2.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1011 2024-04-01 13:38:16.000000 aiolyric-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:38:37.888058 aiolyric-2.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:38:37.892058 aiolyric-2.0.0/tests/objects/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-01 13:38:16.000000 aiolyric-2.0.0/tests/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-01 13:38:16.000000 aiolyric-2.0.0/tests/objects/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    11160 2024-04-01 13:38:16.000000 aiolyric-2.0.0/tests/objects/test_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-01 13:38:16.000000 aiolyric-2.0.0/tests/objects/test_priority.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-01 13:38:16.000000 aiolyric-2.0.0/tests/test__version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-01 13:38:16.000000 aiolyric-2.0.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-01 13:38:16.000000 aiolyric-2.0.0/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:38:09.195487 aiolyric-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 18:37:45.000000 aiolyric-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-21 18:38:09.195487 aiolyric-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-21 18:37:45.000000 aiolyric-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:38:09.191487 aiolyric-2.0.1/aiolyric/
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-21 18:37:45.000000 aiolyric-2.0.1/aiolyric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-21 18:38:07.000000 aiolyric-2.0.1/aiolyric/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-21 18:37:45.000000 aiolyric-2.0.1/aiolyric/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 18:37:45.000000 aiolyric-2.0.1/aiolyric/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-21 18:37:45.000000 aiolyric-2.0.1/aiolyric/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:38:09.191487 aiolyric-2.0.1/aiolyric/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-21 18:37:45.000000 aiolyric-2.0.1/aiolyric/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 18:37:45.000000 aiolyric-2.0.1/aiolyric/objects/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-04-21 18:37:45.000000 aiolyric-2.0.1/aiolyric/objects/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-21 18:37:45.000000 aiolyric-2.0.1/aiolyric/objects/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-21 18:37:45.000000 aiolyric-2.0.1/aiolyric/objects/priority.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:38:09.195487 aiolyric-2.0.1/aiolyric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-21 18:38:09.000000 aiolyric-2.0.1/aiolyric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-21 18:38:09.000000 aiolyric-2.0.1/aiolyric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 18:38:09.000000 aiolyric-2.0.1/aiolyric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-21 18:38:09.000000 aiolyric-2.0.1/aiolyric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 18:38:09.000000 aiolyric-2.0.1/aiolyric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-04-21 18:37:45.000000 aiolyric-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 18:38:09.195487 aiolyric-2.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1011 2024-04-21 18:37:45.000000 aiolyric-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:38:09.191487 aiolyric-2.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:38:09.195487 aiolyric-2.0.1/tests/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-21 18:37:45.000000 aiolyric-2.0.1/tests/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-21 18:37:45.000000 aiolyric-2.0.1/tests/objects/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11160 2024-04-21 18:37:45.000000 aiolyric-2.0.1/tests/objects/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-21 18:37:45.000000 aiolyric-2.0.1/tests/objects/test_priority.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-21 18:37:45.000000 aiolyric-2.0.1/tests/test__version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-21 18:37:45.000000 aiolyric-2.0.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-21 18:37:45.000000 aiolyric-2.0.1/tests/test_init.py
```

### Comparing `aiolyric-2.0.0/LICENSE` & `aiolyric-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiolyric-2.0.0/PKG-INFO` & `aiolyric-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiolyric
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python package for the Honeywell Lyric Platform
 Home-page: https://github.com/timmo001/aiolyric
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: aiolyric,api,async,asyncio,honeywell lyric,honeywell,lyric,integration
 Requires-Python: >=3.11
```

### Comparing `aiolyric-2.0.0/aiolyric/__init__.py` & `aiolyric-2.0.1/aiolyric/__init__.py`

 * *Files identical despite different names*

### Comparing `aiolyric-2.0.0/aiolyric/client.py` & `aiolyric-2.0.1/aiolyric/client.py`

 * *Files identical despite different names*

### Comparing `aiolyric-2.0.0/aiolyric/objects/base.py` & `aiolyric-2.0.1/aiolyric/objects/base.py`

 * *Files identical despite different names*

### Comparing `aiolyric-2.0.0/aiolyric/objects/device.py` & `aiolyric-2.0.1/aiolyric/objects/device.py`

 * *Files identical despite different names*

### Comparing `aiolyric-2.0.0/aiolyric/objects/location.py` & `aiolyric-2.0.1/aiolyric/objects/location.py`

 * *Files identical despite different names*

### Comparing `aiolyric-2.0.0/aiolyric/objects/priority.py` & `aiolyric-2.0.1/aiolyric/objects/priority.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Lyric priority."""
 
 from .base import LyricBaseObject
 
 
-class LyricAccessories(LyricBaseObject):
-    """Lyric accessories."""
+class LyricAccessory(LyricBaseObject):
+    """Lyric accessory."""
 
     @property
     def id(self):
         """Get the ID of the accessory."""
         return self.attributes.get("id", None)
 
     @property
@@ -69,15 +69,15 @@
     def overall_motion(self):
         """Check if motion is detected in the room."""
         return self.attributes.get("overallMotion", False)
 
     @property
     def accessories(self):
         """Get the list of accessories in the room."""
-        return [LyricAccessories(x) for x in self.attributes.get("accessories", [])]
+        return [LyricAccessory(x) for x in self.attributes.get("accessories", [])]
 
 
 class CurrentPriority(LyricBaseObject):
     """Class representing the current priority."""
 
     @property
     def priority_type(self):
```

### Comparing `aiolyric-2.0.0/aiolyric.egg-info/PKG-INFO` & `aiolyric-2.0.1/aiolyric.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiolyric
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python package for the Honeywell Lyric Platform
 Home-page: https://github.com/timmo001/aiolyric
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: aiolyric,api,async,asyncio,honeywell lyric,honeywell,lyric,integration
 Requires-Python: >=3.11
```

### Comparing `aiolyric-2.0.0/aiolyric.egg-info/SOURCES.txt` & `aiolyric-2.0.1/aiolyric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiolyric-2.0.0/pyproject.toml` & `aiolyric-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiolyric-2.0.0/setup.py` & `aiolyric-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `aiolyric-2.0.0/tests/objects/test_device.py` & `aiolyric-2.0.1/tests/objects/test_device.py`

 * *Files identical despite different names*

### Comparing `aiolyric-2.0.0/tests/objects/test_location.py` & `aiolyric-2.0.1/tests/objects/test_location.py`

 * *Files identical despite different names*

### Comparing `aiolyric-2.0.0/tests/objects/test_priority.py` & `aiolyric-2.0.1/tests/objects/test_priority.py`

 * *Files identical despite different names*

### Comparing `aiolyric-2.0.0/tests/test_client.py` & `aiolyric-2.0.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aiolyric-2.0.0/tests/test_init.py` & `aiolyric-2.0.1/tests/test_init.py`

 * *Files identical despite different names*


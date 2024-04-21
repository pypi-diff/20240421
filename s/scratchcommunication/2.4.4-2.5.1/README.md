# Comparing `tmp/scratchcommunication-2.4.4.tar.gz` & `tmp/scratchcommunication-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchcommunication-2.4.4.tar", last modified: Sun Apr 21 13:40:51 2024, max compression
+gzip compressed data, was "scratchcommunication-2.5.1.tar", last modified: Sun Apr 21 13:53:08 2024, max compression
```

## Comparing `scratchcommunication-2.4.4.tar` & `scratchcommunication-2.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:40:51.979123 scratchcommunication-2.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15966 2024-04-21 13:40:51.979123 scratchcommunication-2.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15136 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:40:51.979123 scratchcommunication-2.4.4/scratchcommunication/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/cloud_socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:40:51.979123 scratchcommunication-2.4.4/scratchcommunication/cloudrequests/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/cloudrequests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/cloudrequests/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/cloudrequests/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:40:51.979123 scratchcommunication-2.4.4/scratchcommunication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15966 2024-04-21 13:40:51.000000 scratchcommunication-2.4.4/scratchcommunication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-21 13:40:51.000000 scratchcommunication-2.4.4/scratchcommunication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:40:51.000000 scratchcommunication-2.4.4/scratchcommunication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-21 13:40:51.000000 scratchcommunication-2.4.4/scratchcommunication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-21 13:40:51.000000 scratchcommunication-2.4.4/scratchcommunication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 13:40:51.979123 scratchcommunication-2.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:40:51.979123 scratchcommunication-2.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:53:08.264007 scratchcommunication-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-21 13:53:05.000000 scratchcommunication-2.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-21 13:53:08.264007 scratchcommunication-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-21 13:53:05.000000 scratchcommunication-2.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:53:08.264007 scratchcommunication-2.5.1/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-21 13:53:05.000000 scratchcommunication-2.5.1/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-04-21 13:53:05.000000 scratchcommunication-2.5.1/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-21 13:53:05.000000 scratchcommunication-2.5.1/scratchcommunication/cloud_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:53:08.264007 scratchcommunication-2.5.1/scratchcommunication/cloudrequests/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 13:53:05.000000 scratchcommunication-2.5.1/scratchcommunication/cloudrequests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-21 13:53:05.000000 scratchcommunication-2.5.1/scratchcommunication/cloudrequests/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8749 2024-04-21 13:53:05.000000 scratchcommunication-2.5.1/scratchcommunication/cloudrequests/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-21 13:53:05.000000 scratchcommunication-2.5.1/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-21 13:53:05.000000 scratchcommunication-2.5.1/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-21 13:53:05.000000 scratchcommunication-2.5.1/scratchcommunication/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-21 13:53:05.000000 scratchcommunication-2.5.1/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:53:08.264007 scratchcommunication-2.5.1/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-21 13:53:08.000000 scratchcommunication-2.5.1/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-21 13:53:08.000000 scratchcommunication-2.5.1/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:53:08.000000 scratchcommunication-2.5.1/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-21 13:53:08.000000 scratchcommunication-2.5.1/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-21 13:53:08.000000 scratchcommunication-2.5.1/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 13:53:08.264007 scratchcommunication-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-21 13:53:05.000000 scratchcommunication-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:53:08.264007 scratchcommunication-2.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-21 13:53:05.000000 scratchcommunication-2.5.1/tests/test1.py
```

### Comparing `scratchcommunication-2.4.4/LICENSE` & `scratchcommunication-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.4/PKG-INFO` & `scratchcommunication-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.4.4
+Version: 2.5.1
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -263,15 +263,16 @@
 ## Starting the cloud requests handler
 
 Start the cloud requests handler using the `start` method.
 
 ```python
 cloud_requests.start(
     thread = None, # (Optional) Whether to use a thread; If None then it defaults to the used_thread value used at creation of the cloud requests handler
-    daemon_thread = False # (Optional) Whether the thread is daemon
+    daemon_thread = False, # (Optional) Whether the thread is daemon
+    duration = None # (Optional) How long to run the cloud requests
 )
 ```
 
 ## Stopping the cloud requests handler
 
 Stop the cloud requests handler using the `stop` method. (Only if the cloud requests handler is running in a thread)
```

### Comparing `scratchcommunication-2.4.4/README.md` & `scratchcommunication-2.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,16 @@
 ## Starting the cloud requests handler
 
 Start the cloud requests handler using the `start` method.
 
 ```python
 cloud_requests.start(
     thread = None, # (Optional) Whether to use a thread; If None then it defaults to the used_thread value used at creation of the cloud requests handler
-    daemon_thread = False # (Optional) Whether the thread is daemon
+    daemon_thread = False, # (Optional) Whether the thread is daemon
+    duration = None # (Optional) How long to run the cloud requests
 )
 ```
 
 ## Stopping the cloud requests handler
 
 Stop the cloud requests handler using the `stop` method. (Only if the cloud requests handler is running in a thread)
```

### Comparing `scratchcommunication-2.4.4/scratchcommunication/cloud.py` & `scratchcommunication-2.5.1/scratchcommunication/cloud.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.4/scratchcommunication/cloud_socket.py` & `scratchcommunication-2.5.1/scratchcommunication/cloud_socket.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.4/scratchcommunication/cloudrequests/basetypes.py` & `scratchcommunication-2.5.1/scratchcommunication/cloudrequests/basetypes.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.4/scratchcommunication/cloudrequests/requests.py` & `scratchcommunication-2.5.1/scratchcommunication/cloudrequests/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Submodule for handling incoming requests.
 """
-import re, warnings, ast, inspect, traceback
-from typing import Union, Mapping, Sequence, Any, Iterable
+import re, warnings, ast, inspect, traceback, time
+from typing import Union, Mapping, Sequence, Any
 from types import FunctionType
 from func_timeout import StoppableThread
 from scratchcommunication.cloud_socket import CloudSocketConnection, CloudSocket
 from .basetypes import BaseRequestHandler, StopRequestHandler, NotUsingAThread
 
 class RequestHandler(BaseRequestHandler):
     """
@@ -39,26 +39,27 @@
         """
         func.__name__ = name or func.__name__
         func.auto_convert = auto_convert
         func.allow_python_syntax = allow_python_syntax
         func.thread = thread
         self.requests[func.__name__] = func
     
-    def start(self, *, thread : bool = None, daemon_thread : bool = False):
+    def start(self, *, thread : bool = None, daemon_thread : bool = False, duration : Union[float, int, None] = None):
         """
         Method for starting the request handler.
         """
         self.cloud_socket.listen()
         if thread or (thread is None and self.uses_thread):
             self.uses_thread = True
             self.thread = StoppableThread(target=lambda : self.start(thread=False), daemon=daemon_thread)
             self.thread.start()
             return
         clients : list[tuple[CloudSocketConnection, str]] = []
-        while True:
+        end_time = duration and (time.time() + duration)
+        while (not end_time) or time.time() < end_time:
             try:
                 try:
                     clients.append(self.cloud_socket.accept(timeout=0))
                 except TimeoutError:
                     pass
                 for client, username in clients:
                     try:
```

### Comparing `scratchcommunication-2.4.4/scratchcommunication/security.py` & `scratchcommunication-2.5.1/scratchcommunication/security.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.4/scratchcommunication/session.py` & `scratchcommunication-2.5.1/scratchcommunication/session.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.4/scratchcommunication.egg-info/PKG-INFO` & `scratchcommunication-2.5.1/scratchcommunication.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.4.4
+Version: 2.5.1
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -263,15 +263,16 @@
 ## Starting the cloud requests handler
 
 Start the cloud requests handler using the `start` method.
 
 ```python
 cloud_requests.start(
     thread = None, # (Optional) Whether to use a thread; If None then it defaults to the used_thread value used at creation of the cloud requests handler
-    daemon_thread = False # (Optional) Whether the thread is daemon
+    daemon_thread = False, # (Optional) Whether the thread is daemon
+    duration = None # (Optional) How long to run the cloud requests
 )
 ```
 
 ## Stopping the cloud requests handler
 
 Stop the cloud requests handler using the `stop` method. (Only if the cloud requests handler is running in a thread)
```

### Comparing `scratchcommunication-2.4.4/scratchcommunication.egg-info/SOURCES.txt` & `scratchcommunication-2.5.1/scratchcommunication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.4/setup.py` & `scratchcommunication-2.5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '2.4.4'
+VERSION = '2.5.1'
 
 setup(
     name='scratchcommunication',
     version=VERSION,
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for communicating with scratch projects',
```

### Comparing `scratchcommunication-2.4.4/tests/test1.py` & `scratchcommunication-2.5.1/tests/test1.py`

 * *Files identical despite different names*


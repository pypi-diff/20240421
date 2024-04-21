# Comparing `tmp/scratchcommunication-2.4.3.tar.gz` & `tmp/scratchcommunication-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchcommunication-2.4.3.tar", last modified: Fri Apr 19 13:34:32 2024, max compression
+gzip compressed data, was "scratchcommunication-2.4.4.tar", last modified: Sun Apr 21 13:40:51 2024, max compression
```

## Comparing `scratchcommunication-2.4.3.tar` & `scratchcommunication-2.4.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:34:32.426413 scratchcommunication-2.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-19 13:34:29.000000 scratchcommunication-2.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15966 2024-04-19 13:34:32.426413 scratchcommunication-2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15136 2024-04-19 13:34:29.000000 scratchcommunication-2.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:34:32.422413 scratchcommunication-2.4.3/scratchcommunication/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-19 13:34:29.000000 scratchcommunication-2.4.3/scratchcommunication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-04-19 13:34:29.000000 scratchcommunication-2.4.3/scratchcommunication/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-19 13:34:29.000000 scratchcommunication-2.4.3/scratchcommunication/cloud_socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:34:32.426413 scratchcommunication-2.4.3/scratchcommunication/cloudrequests/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-19 13:34:29.000000 scratchcommunication-2.4.3/scratchcommunication/cloudrequests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-19 13:34:29.000000 scratchcommunication-2.4.3/scratchcommunication/cloudrequests/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-19 13:34:29.000000 scratchcommunication-2.4.3/scratchcommunication/cloudrequests/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 13:34:29.000000 scratchcommunication-2.4.3/scratchcommunication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-19 13:34:29.000000 scratchcommunication-2.4.3/scratchcommunication/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-19 13:34:29.000000 scratchcommunication-2.4.3/scratchcommunication/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-19 13:34:29.000000 scratchcommunication-2.4.3/scratchcommunication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:34:32.426413 scratchcommunication-2.4.3/scratchcommunication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15966 2024-04-19 13:34:32.000000 scratchcommunication-2.4.3/scratchcommunication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-19 13:34:32.000000 scratchcommunication-2.4.3/scratchcommunication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:34:32.000000 scratchcommunication-2.4.3/scratchcommunication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:34:32.000000 scratchcommunication-2.4.3/scratchcommunication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 13:34:32.000000 scratchcommunication-2.4.3/scratchcommunication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:34:32.426413 scratchcommunication-2.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-19 13:34:29.000000 scratchcommunication-2.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:34:32.426413 scratchcommunication-2.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-19 13:34:29.000000 scratchcommunication-2.4.3/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:40:51.979123 scratchcommunication-2.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15966 2024-04-21 13:40:51.979123 scratchcommunication-2.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15136 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:40:51.979123 scratchcommunication-2.4.4/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/cloud_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:40:51.979123 scratchcommunication-2.4.4/scratchcommunication/cloudrequests/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/cloudrequests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/cloudrequests/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/cloudrequests/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:40:51.979123 scratchcommunication-2.4.4/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15966 2024-04-21 13:40:51.000000 scratchcommunication-2.4.4/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-21 13:40:51.000000 scratchcommunication-2.4.4/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:40:51.000000 scratchcommunication-2.4.4/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-21 13:40:51.000000 scratchcommunication-2.4.4/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-21 13:40:51.000000 scratchcommunication-2.4.4/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 13:40:51.979123 scratchcommunication-2.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:40:51.979123 scratchcommunication-2.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-21 13:40:48.000000 scratchcommunication-2.4.4/tests/test1.py
```

### Comparing `scratchcommunication-2.4.3/LICENSE` & `scratchcommunication-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.3/PKG-INFO` & `scratchcommunication-2.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.4.3
+Version: 2.4.4
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.4.3/README.md` & `scratchcommunication-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.3/scratchcommunication/cloud.py` & `scratchcommunication-2.4.4/scratchcommunication/cloud.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.3/scratchcommunication/cloud_socket.py` & `scratchcommunication-2.4.4/scratchcommunication/cloud_socket.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.3/scratchcommunication/cloudrequests/basetypes.py` & `scratchcommunication-2.4.4/scratchcommunication/cloudrequests/basetypes.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.3/scratchcommunication/cloudrequests/requests.py` & `scratchcommunication-2.4.4/scratchcommunication/cloudrequests/requests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Submodule for handling incoming requests.
 """
 import re, warnings, ast, inspect, traceback
-from typing import Union, Mapping, Sequence, Any
+from typing import Union, Mapping, Sequence, Any, Iterable
 from types import FunctionType
 from func_timeout import StoppableThread
 from scratchcommunication.cloud_socket import CloudSocketConnection, CloudSocket
 from .basetypes import BaseRequestHandler, StopRequestHandler, NotUsingAThread
 
 class RequestHandler(BaseRequestHandler):
     """
@@ -96,19 +96,23 @@
         request_handling_function = self.requests[name]
         return_converter = lambda x : x
         if request_handling_function.auto_convert:
             for idx, (arg, annotation) in enumerate(inspect.signature(request_handling_function).parameters.items()):
                 if inspect.Parameter.empty == annotation.annotation:
                     continue
                 if not arg in kwargs:
+                    if not annotation.kind.value in [0, 1]:
+                        raise ValueError("Signature doesn't match")
                     try:
                         args[idx] = annotation.annotation(args[idx])
                     except IndexError:
                         pass
                     continue
+                if not annotation.kind.value in [1, 3]:
+                    raise ValueError("Signature doesn't match")
                 kwargs[arg] = annotation.annotation(kwargs[arg])
             if inspect.signature(request_handling_function).return_annotation != inspect.Signature.empty:
                 return_converter = inspect.signature(request_handling_function).return_annotation
         def respond():
             client.send(str(return_converter(request_handling_function(*args, **kwargs))))
         if request_handling_function.thread:
             thread = StoppableThread(target=respond)
```

### Comparing `scratchcommunication-2.4.3/scratchcommunication/security.py` & `scratchcommunication-2.4.4/scratchcommunication/security.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.3/scratchcommunication/session.py` & `scratchcommunication-2.4.4/scratchcommunication/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         
     def create_cloudconnection(self, project_id : int, **kwargs) -> cloud.CloudConnection:
         '''
         Create a cloud connection to a project.
         '''
         return cloud.CloudConnection(project_id=project_id, session=self, **kwargs)
     
-    def create_turbowarp_cloudconnection(self, project_id : int, *, username = None, **kwargs) -> cloud.TwCloudConnection:
+    def create_turbowarp_cloudconnection(self, project_id : str, *, username = None, **kwargs) -> cloud.TwCloudConnection:
         '''
         Create a cloud connection to a turbowarp project.
         '''
         username = username or self.username
         return cloud.TwCloudConnection(project_id=project_id, username=username, session=self, **kwargs)
     
     def create_tw_cloudconnection(self, *args, **kwargs):
@@ -103,15 +103,15 @@
 
     def create_cloud_socket(self, project_id : int, *, packet_size : int = 220, cloudconnection_kwargs : dict = None, security : tuple = None, **kwargs):
         '''
         Create a cloud socket to a project.
         '''
         return cloud_socket.CloudSocket(cloud=self.create_cloudconnection(project_id, warning_type=ErrorInCloudSocket, **(cloudconnection_kwargs if cloudconnection_kwargs else {})), packet_size=packet_size, security=security, **kwargs)
 
-    def create_turbowarp_cloud_socket(self, contact_info : str, project_id : int, *, packet_size : int = 90000, cloudconnection_kwargs : dict = None, security : tuple = None, **kwargs):
+    def create_turbowarp_cloud_socket(self, contact_info : str, project_id : str, *, packet_size : int = 90000, cloudconnection_kwargs : dict = None, security : tuple = None, **kwargs):
         '''
         Create a cloud socket to a turbowarp project.
         '''
         return cloud_socket.CloudSocket(cloud=self.create_tw_cloudconnection(project_id, contact_info=contact_info, warning_type=ErrorInCloudSocket, **(cloudconnection_kwargs if cloudconnection_kwargs else {})), packet_size=packet_size, security=security, **kwargs)
     
     def create_tw_cloud_socket(self, *args, **kwargs):
         '''
```

### Comparing `scratchcommunication-2.4.3/scratchcommunication.egg-info/PKG-INFO` & `scratchcommunication-2.4.4/scratchcommunication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.4.3
+Version: 2.4.4
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.4.3/scratchcommunication.egg-info/SOURCES.txt` & `scratchcommunication-2.4.4/scratchcommunication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.4.3/setup.py` & `scratchcommunication-2.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '2.4.3'
+VERSION = '2.4.4'
 
 setup(
     name='scratchcommunication',
     version=VERSION,
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for communicating with scratch projects',
```

### Comparing `scratchcommunication-2.4.3/tests/test1.py` & `scratchcommunication-2.4.4/tests/test1.py`

 * *Files identical despite different names*


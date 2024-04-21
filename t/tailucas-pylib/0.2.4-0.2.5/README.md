# Comparing `tmp/tailucas_pylib-0.2.4.tar.gz` & `tmp/tailucas_pylib-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailucas_pylib-0.2.4.tar", max compression
+gzip compressed data, was "tailucas_pylib-0.2.5.tar", max compression
```

## Comparing `tailucas_pylib-0.2.4.tar` & `tailucas_pylib-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.2.4/LICENSE
--rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.2.4/README.md
--rw-r--r--   0        0        0      565 2024-02-25 13:23:35.231362 tailucas_pylib-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     5454 2024-01-07 20:24:45.999553 tailucas_pylib-0.2.4/tailucas_pylib/__init__.py
--rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.2.4/tailucas_pylib/app.py
--rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.2.4/tailucas_pylib/aws/__init__.py
--rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.2.4/tailucas_pylib/aws/metrics.py
--rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.2.4/tailucas_pylib/aws/swf.py
--rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.4/tailucas_pylib/bluetooth.py
--rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.2.4/tailucas_pylib/data.py
--rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.4/tailucas_pylib/datetime.py
--rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.2.4/tailucas_pylib/handler.py
--rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.4/tailucas_pylib/process.py
--rw-r--r--   0        0        0     9521 2023-09-03 07:12:39.509088 tailucas_pylib-0.2.4/tailucas_pylib/rabbit.py
--rw-r--r--   0        0        0     5232 2024-01-09 19:38:40.728310 tailucas_pylib-0.2.4/tailucas_pylib/threads.py
--rw-r--r--   0        0        0     3302 2023-12-10 05:04:22.026794 tailucas_pylib-0.2.4/tailucas_pylib/zmq.py
--rw-r--r--   0        0        0    12338 1970-01-01 00:00:00.000000 tailucas_pylib-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.2.5/LICENSE
+-rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.2.5/README.md
+-rw-r--r--   0        0        0      565 2024-04-21 11:15:07.341871 tailucas_pylib-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     5454 2024-01-07 20:24:45.999553 tailucas_pylib-0.2.5/tailucas_pylib/__init__.py
+-rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.2.5/tailucas_pylib/app.py
+-rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.2.5/tailucas_pylib/aws/__init__.py
+-rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.2.5/tailucas_pylib/aws/metrics.py
+-rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.2.5/tailucas_pylib/aws/swf.py
+-rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.5/tailucas_pylib/bluetooth.py
+-rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.2.5/tailucas_pylib/data.py
+-rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.5/tailucas_pylib/datetime.py
+-rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.2.5/tailucas_pylib/handler.py
+-rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.2.5/tailucas_pylib/process.py
+-rw-r--r--   0        0        0     9521 2023-09-03 07:12:39.509088 tailucas_pylib-0.2.5/tailucas_pylib/rabbit.py
+-rw-r--r--   0        0        0     5232 2024-01-09 19:38:40.728310 tailucas_pylib-0.2.5/tailucas_pylib/threads.py
+-rw-r--r--   0        0        0     3387 2024-04-21 11:13:24.751872 tailucas_pylib-0.2.5/tailucas_pylib/zmq.py
+-rw-r--r--   0        0        0    12338 1970-01-01 00:00:00.000000 tailucas_pylib-0.2.5/PKG-INFO
```

### Comparing `tailucas_pylib-0.2.4/LICENSE` & `tailucas_pylib-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.4/README.md` & `tailucas_pylib-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.4/pyproject.toml` & `tailucas_pylib-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tailucas-pylib"
-version = "0.2.4"
+version = "0.2.5"
 description = "Common Python utility modules"
 authors = ["Tai Lucas <tglucas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `tailucas_pylib-0.2.4/tailucas_pylib/__init__.py` & `tailucas_pylib-0.2.5/tailucas_pylib/__init__.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.4/tailucas_pylib/app.py` & `tailucas_pylib-0.2.5/tailucas_pylib/app.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.4/tailucas_pylib/aws/__init__.py` & `tailucas_pylib-0.2.5/tailucas_pylib/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.4/tailucas_pylib/aws/metrics.py` & `tailucas_pylib-0.2.5/tailucas_pylib/aws/metrics.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.4/tailucas_pylib/aws/swf.py` & `tailucas_pylib-0.2.5/tailucas_pylib/aws/swf.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.4/tailucas_pylib/bluetooth.py` & `tailucas_pylib-0.2.5/tailucas_pylib/bluetooth.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.4/tailucas_pylib/data.py` & `tailucas_pylib-0.2.5/tailucas_pylib/data.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.4/tailucas_pylib/datetime.py` & `tailucas_pylib-0.2.5/tailucas_pylib/datetime.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.4/tailucas_pylib/handler.py` & `tailucas_pylib-0.2.5/tailucas_pylib/handler.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.4/tailucas_pylib/process.py` & `tailucas_pylib-0.2.5/tailucas_pylib/process.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.4/tailucas_pylib/rabbit.py` & `tailucas_pylib-0.2.5/tailucas_pylib/rabbit.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.4/tailucas_pylib/threads.py` & `tailucas_pylib-0.2.5/tailucas_pylib/threads.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.2.4/tailucas_pylib/zmq.py` & `tailucas_pylib-0.2.5/tailucas_pylib/zmq.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,15 +37,17 @@
     zmq_sockets[socket] = location
     return socket
 
 
 def zmq_term():
     log.info(f'Shutting down ZMQ context...')
     zmq_context.term()
+    global zmq_async_context
     if zmq_async_context:
+        log.info(f'Shutting down async ZMQ context...')
         try:
             zmq_async_context.term()
         except Exception:
             log.debug('Error closing async ZMQ context.', exc_info=True)
     log.info(f'ZMQ shutdown complete.')
```

### Comparing `tailucas_pylib-0.2.4/PKG-INFO` & `tailucas_pylib-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailucas-pylib
-Version: 0.2.4
+Version: 0.2.5
 Summary: Common Python utility modules
 License: MIT
 Author: Tai Lucas
 Author-email: tglucas@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


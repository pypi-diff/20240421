# Comparing `tmp/terncy-0.3.9.tar.gz` & `tmp/terncy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terncy-0.3.9.tar", last modified: Mon Nov  6 11:13:09 2023, max compression
+gzip compressed data, was "terncy-0.4.0.tar", last modified: Sun Apr 21 04:41:54 2024, max compression
```

## Comparing `terncy-0.3.9.tar` & `terncy-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 raymond   (1000) raymond   (1000)        0 2023-11-06 11:13:09.567811 terncy-0.3.9/
--rw-rw-r--   0 raymond   (1000) raymond   (1000)     1062 2023-11-04 15:40:09.000000 terncy-0.3.9/LICENSE
--rw-rw-r--   0 raymond   (1000) raymond   (1000)     2796 2023-11-06 11:13:09.567811 terncy-0.3.9/PKG-INFO
--rw-rw-r--   0 raymond   (1000) raymond   (1000)     1971 2023-11-06 10:57:23.000000 terncy-0.3.9/README.md
--rw-rw-r--   0 raymond   (1000) raymond   (1000)      104 2023-11-04 15:41:47.000000 terncy-0.3.9/pyproject.toml
--rw-rw-r--   0 raymond   (1000) raymond   (1000)       38 2023-11-06 11:13:09.567811 terncy-0.3.9/setup.cfg
--rw-rw-r--   0 raymond   (1000) raymond   (1000)     1368 2023-11-06 09:43:16.000000 terncy-0.3.9/setup.py
-drwxrwxr-x   0 raymond   (1000) raymond   (1000)        0 2023-11-06 11:13:09.567811 terncy-0.3.9/terncy/
--rw-rw-r--   0 raymond   (1000) raymond   (1000)      219 2023-11-04 15:40:09.000000 terncy-0.3.9/terncy/__init__.py
--rw-rw-r--   0 raymond   (1000) raymond   (1000)      335 2023-11-04 15:40:09.000000 terncy-0.3.9/terncy/event.py
--rw-rw-r--   0 raymond   (1000) raymond   (1000)    12021 2023-11-06 11:12:30.000000 terncy-0.3.9/terncy/terncy.py
--rw-rw-r--   0 raymond   (1000) raymond   (1000)       69 2023-11-06 11:12:46.000000 terncy-0.3.9/terncy/version.py
-drwxrwxr-x   0 raymond   (1000) raymond   (1000)        0 2023-11-06 11:13:09.567811 terncy-0.3.9/terncy.egg-info/
--rw-rw-r--   0 raymond   (1000) raymond   (1000)     2796 2023-11-06 11:13:09.000000 terncy-0.3.9/terncy.egg-info/PKG-INFO
--rw-rw-r--   0 raymond   (1000) raymond   (1000)      260 2023-11-06 11:13:09.000000 terncy-0.3.9/terncy.egg-info/SOURCES.txt
--rw-rw-r--   0 raymond   (1000) raymond   (1000)        1 2023-11-06 11:13:09.000000 terncy-0.3.9/terncy.egg-info/dependency_links.txt
--rw-rw-r--   0 raymond   (1000) raymond   (1000)       19 2023-11-06 11:13:09.000000 terncy-0.3.9/terncy.egg-info/requires.txt
--rw-rw-r--   0 raymond   (1000) raymond   (1000)        7 2023-11-06 11:13:09.000000 terncy-0.3.9/terncy.egg-info/top_level.txt
+drwxr-xr-x   0 raymond    (502) staff       (20)        0 2024-04-21 04:41:54.356690 terncy-0.4.0/
+-rw-r--r--   0 raymond    (502) staff       (20)     1062 2023-02-06 15:33:02.000000 terncy-0.4.0/LICENSE
+-rw-r--r--   0 raymond    (502) staff       (20)     2845 2024-04-21 04:41:54.356489 terncy-0.4.0/PKG-INFO
+-rw-r--r--   0 raymond    (502) staff       (20)     1971 2024-04-21 02:48:04.000000 terncy-0.4.0/README.md
+-rw-r--r--   0 raymond    (502) staff       (20)      104 2024-04-21 02:48:04.000000 terncy-0.4.0/pyproject.toml
+-rw-r--r--   0 raymond    (502) staff       (20)       38 2024-04-21 04:41:54.356730 terncy-0.4.0/setup.cfg
+-rw-r--r--   0 raymond    (502) staff       (20)     1368 2024-04-21 02:48:04.000000 terncy-0.4.0/setup.py
+drwxr-xr-x   0 raymond    (502) staff       (20)        0 2024-04-21 04:41:54.355526 terncy-0.4.0/terncy/
+-rw-r--r--   0 raymond    (502) staff       (20)      219 2023-02-06 15:33:02.000000 terncy-0.4.0/terncy/__init__.py
+-rw-r--r--   0 raymond    (502) staff       (20)      335 2023-02-06 15:33:02.000000 terncy-0.4.0/terncy/event.py
+-rw-r--r--   0 raymond    (502) staff       (20)    13120 2024-04-21 02:51:52.000000 terncy-0.4.0/terncy/terncy.py
+-rw-r--r--   0 raymond    (502) staff       (20)       69 2024-04-21 04:39:31.000000 terncy-0.4.0/terncy/version.py
+drwxr-xr-x   0 raymond    (502) staff       (20)        0 2024-04-21 04:41:54.356263 terncy-0.4.0/terncy.egg-info/
+-rw-r--r--   0 raymond    (502) staff       (20)     2845 2024-04-21 04:41:54.000000 terncy-0.4.0/terncy.egg-info/PKG-INFO
+-rw-r--r--   0 raymond    (502) staff       (20)      260 2024-04-21 04:41:54.000000 terncy-0.4.0/terncy.egg-info/SOURCES.txt
+-rw-r--r--   0 raymond    (502) staff       (20)        1 2024-04-21 04:41:54.000000 terncy-0.4.0/terncy.egg-info/dependency_links.txt
+-rw-r--r--   0 raymond    (502) staff       (20)       19 2024-04-21 04:41:54.000000 terncy-0.4.0/terncy.egg-info/requires.txt
+-rw-r--r--   0 raymond    (502) staff       (20)        7 2024-04-21 04:41:54.000000 terncy-0.4.0/terncy.egg-info/top_level.txt
```

### Comparing `terncy-0.3.9/LICENSE` & `terncy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terncy-0.3.9/PKG-INFO` & `terncy-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terncy
-Version: 0.3.9
+Version: 0.4.0
 Summary: A Python library for controlling Terncy home automation system.
 Home-page: https://github.com/rxwen/python-terncy/
 Author: Ruixiong Wen
 Author-email: rx.wen218@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: enum-compat
+Requires-Dist: future
 
 # python-terncy
 A python library for control ***[Terncy](https://www.terncy.com/)*** devices.
 
 [![PyPI version](https://badge.fury.io/py/terncy.svg)](https://badge.fury.io/py/terncy) [![Build Status](https://travis-ci.org/rxwen/python-terncy.svg?branch=master)](https://travis-ci.org/rxwen/python-terncy)
 
 ## Installation
```

### Comparing `terncy-0.3.9/README.md` & `terncy-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `terncy-0.3.9/setup.py` & `terncy-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `terncy-0.3.9/terncy/terncy.py` & `terncy-0.4.0/terncy/terncy.py`

 * *Files 4% similar despite different names*

```diff
@@ -297,61 +297,85 @@
         method,
         wait_result=False,
         timeout=WAIT_RESP_TIMEOUT_SEC,
     ):
         if self._connection is None:
             _LOGGER.info(f"no connection with {self.dev_id}")
             return None
-        req_id = _next_req_id()
-        data = {
-            "reqId": req_id,
-            "intent": "execute",
-            "entities": [
-                {
-                    "id": ent_id,
-                    "attributes": [
-                        {
-                            "attr": attr,
-                            "value": attr_val,
-                            "method": method,
-                        }
-                    ],
-                }
-            ],
-        }
-        await self._connection.send(json.dumps(data))
-        if wait_result:
-            return await self._wait_for_response(req_id, data, timeout)
+        try:
+            req_id = _next_req_id()
+            data = {
+                "reqId": req_id,
+                "intent": "execute",
+                "entities": [
+                    {
+                        "id": ent_id,
+                        "attributes": [
+                            {
+                                "attr": attr,
+                                "value": attr_val,
+                                "method": method,
+                            }
+                        ],
+                    }
+                ],
+            }
+            await self._connection.send(json.dumps(data))
+            if wait_result:
+                return await self._wait_for_response(req_id, data, timeout)
+        except (
+            aiohttp.client_exceptions.ClientConnectionError,
+            websockets.exceptions.ConnectionClosedError,
+            ConnectionRefusedError,
+            OSError,
+            websockets.exceptions.InvalidStatusCode,
+        ) as e:
+            _LOGGER.info(f"disconnect when set attr {e}")
+            if self._event_handler:
+                self._event_handler(self, event.Disconnected())
+            self._connection = None
 
     async def set_attributes(
         self,
         ent_id,
         attrs: list[dict],
         method,
         wait_result=False,
         timeout=WAIT_RESP_TIMEOUT_SEC,
     ):
-        print(attrs)
         if self._connection is None:
             _LOGGER.info(f"no connection with {self.dev_id}")
             return None
-        req_id = _next_req_id()
-        data = {
-            "reqId": req_id,
-            "intent": "execute",
-            "entities": [
-                {
-                    "id": ent_id,
-                    "attributes": [
-                        {
-                            "attr": av["attr"],
-                            "value": av["value"],
-                            "method": method,
-                        }
-                        for av in attrs
-                    ],
-                }
-            ],
-        }
-        await self._connection.send(json.dumps(data))
-        if wait_result:
-            return await self._wait_for_response(req_id, data, timeout)
+        try:
+            req_id = _next_req_id()
+            data = {
+                "reqId": req_id,
+                "intent": "execute",
+                "entities": [
+                    {
+                        "id": ent_id,
+                        "attributes": [
+                            {
+                                "attr": av["attr"],
+                                "value": av["value"],
+                                "method": method,
+                            }
+                            for av in attrs
+                        ],
+                    }
+                ],
+            }
+            await self._connection.send(json.dumps(data))
+            if wait_result:
+                return await self._wait_for_response(req_id, data, timeout)
+        except (
+            aiohttp.client_exceptions.ClientConnectionError,
+            websockets.exceptions.ConnectionClosedError,
+            ConnectionRefusedError,
+            OSError,
+            websockets.exceptions.InvalidStatusCode,
+        ) as e:
+            _LOGGER.info(f"disconnect when set attrs {e}")
+            if self._event_handler:
+                self._event_handler(self, event.Disconnected())
+            self._connection = None
+            return
```

### Comparing `terncy-0.3.9/terncy.egg-info/PKG-INFO` & `terncy-0.4.0/terncy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terncy
-Version: 0.3.9
+Version: 0.4.0
 Summary: A Python library for controlling Terncy home automation system.
 Home-page: https://github.com/rxwen/python-terncy/
 Author: Ruixiong Wen
 Author-email: rx.wen218@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: enum-compat
+Requires-Dist: future
 
 # python-terncy
 A python library for control ***[Terncy](https://www.terncy.com/)*** devices.
 
 [![PyPI version](https://badge.fury.io/py/terncy.svg)](https://badge.fury.io/py/terncy) [![Build Status](https://travis-ci.org/rxwen/python-terncy.svg?branch=master)](https://travis-ci.org/rxwen/python-terncy)
 
 ## Installation
```


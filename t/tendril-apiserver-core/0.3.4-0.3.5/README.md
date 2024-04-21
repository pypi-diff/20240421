# Comparing `tmp/tendril_apiserver_core-0.3.4.tar.gz` & `tmp/tendril_apiserver_core-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril_apiserver_core-0.3.4.tar", last modified: Thu Apr 18 22:06:12 2024, max compression
+gzip compressed data, was "tendril_apiserver_core-0.3.5.tar", last modified: Sun Apr 21 18:14:11 2024, max compression
```

## Comparing `tendril_apiserver_core-0.3.4.tar` & `tendril_apiserver_core-0.3.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.267438 tendril_apiserver_core-0.3.4/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/MANIFEST.in
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5911 2024-04-18 22:06:12.267438 tendril_apiserver_core-0.3.4/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2302 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/README.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-18 22:06:12.267438 tendril_apiserver_core-0.3.4/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3479 2023-08-10 00:50:44.000000 tendril_apiserver_core-0.3.4/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.247438 tendril_apiserver_core-0.3.4/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.251438 tendril_apiserver_core-0.3.4/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.251438 tendril_apiserver_core-0.3.4/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/src/tendril/apiserver/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       52 2023-02-18 23:08:41.000000 tendril_apiserver_core-0.3.4/src/tendril/apiserver/core.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.251438 tendril_apiserver_core-0.3.4/src/tendril/apiserver/exceptions/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:26.000000 tendril_apiserver_core-0.3.4/src/tendril/apiserver/exceptions/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      428 2023-03-15 16:01:26.000000 tendril_apiserver_core-0.3.4/src/tendril/apiserver/exceptions/common.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.255438 tendril_apiserver_core-0.3.4/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 20:27:06.000000 tendril_apiserver_core-0.3.4/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2115 2024-02-04 15:59:51.000000 tendril_apiserver_core-0.3.4/src/tendril/apiserver/routers/diagnostics.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1075 2023-09-06 11:25:54.000000 tendril_apiserver_core-0.3.4/src/tendril/apiserver/routers/system.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5669 2023-09-06 12:16:17.000000 tendril_apiserver_core-0.3.4/src/tendril/apiserver/server.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.255438 tendril_apiserver_core-0.3.4/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:36:13.000000 tendril_apiserver_core-0.3.4/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.255438 tendril_apiserver_core-0.3.4/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 21:00:43.000000 tendril_apiserver_core-0.3.4/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      153 2022-11-28 19:36:13.000000 tendril_apiserver_core-0.3.4/src/tendril/authz/scopes/system.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.255438 tendril_apiserver_core-0.3.4/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:26.000000 tendril_apiserver_core-0.3.4/src/tendril/common/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      143 2024-04-17 22:39:46.000000 tendril_apiserver_core-0.3.4/src/tendril/common/exceptions.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.255438 tendril_apiserver_core-0.3.4/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3083 2023-03-16 05:14:37.000000 tendril_apiserver_core-0.3.4/src/tendril/config/server.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.259438 tendril_apiserver_core-0.3.4/src/tendril/resources/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1302 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/src/tendril/resources/test_certificate.pem
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1704 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/src/tendril/resources/test_key.pem
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.259438 tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5911 2024-04-18 22:06:12.000000 tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1052 2024-04-18 22:06:12.000000 tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-18 22:06:12.000000 tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2024-04-18 22:06:12.000000 tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/entry_points.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      772 2024-04-18 22:06:12.000000 tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-18 22:06:12.000000 tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/top_level.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      829 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 18:14:11.178544 tendril_apiserver_core-0.3.5/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.5/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.5/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.5/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.5/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.5/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.5/MANIFEST.in
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5911 2024-04-21 18:14:11.178544 tendril_apiserver_core-0.3.5/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2302 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.5/README.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-21 18:14:11.178544 tendril_apiserver_core-0.3.5/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3479 2023-08-10 00:50:44.000000 tendril_apiserver_core-0.3.5/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 18:14:11.162544 tendril_apiserver_core-0.3.5/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 18:14:11.166544 tendril_apiserver_core-0.3.5/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.5/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 18:14:11.166544 tendril_apiserver_core-0.3.5/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.5/src/tendril/apiserver/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       52 2023-02-18 23:08:41.000000 tendril_apiserver_core-0.3.5/src/tendril/apiserver/core.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 18:14:11.166544 tendril_apiserver_core-0.3.5/src/tendril/apiserver/exceptions/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:26.000000 tendril_apiserver_core-0.3.5/src/tendril/apiserver/exceptions/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      428 2023-03-15 16:01:26.000000 tendril_apiserver_core-0.3.5/src/tendril/apiserver/exceptions/common.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 18:14:11.166544 tendril_apiserver_core-0.3.5/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 20:27:06.000000 tendril_apiserver_core-0.3.5/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2115 2024-02-04 15:59:51.000000 tendril_apiserver_core-0.3.5/src/tendril/apiserver/routers/diagnostics.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1075 2023-09-06 11:25:54.000000 tendril_apiserver_core-0.3.5/src/tendril/apiserver/routers/system.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6181 2024-04-21 17:58:57.000000 tendril_apiserver_core-0.3.5/src/tendril/apiserver/server.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 18:14:11.170544 tendril_apiserver_core-0.3.5/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:36:13.000000 tendril_apiserver_core-0.3.5/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 18:14:11.170544 tendril_apiserver_core-0.3.5/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 21:00:43.000000 tendril_apiserver_core-0.3.5/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      153 2022-11-28 19:36:13.000000 tendril_apiserver_core-0.3.5/src/tendril/authz/scopes/system.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 18:14:11.170544 tendril_apiserver_core-0.3.5/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:26.000000 tendril_apiserver_core-0.3.5/src/tendril/common/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      143 2024-04-17 22:39:46.000000 tendril_apiserver_core-0.3.5/src/tendril/common/exceptions.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 18:14:11.170544 tendril_apiserver_core-0.3.5/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.5/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3083 2023-03-16 05:14:37.000000 tendril_apiserver_core-0.3.5/src/tendril/config/server.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 18:14:11.170544 tendril_apiserver_core-0.3.5/src/tendril/resources/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1302 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.5/src/tendril/resources/test_certificate.pem
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1704 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.5/src/tendril/resources/test_key.pem
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 18:14:11.174544 tendril_apiserver_core-0.3.5/src/tendril_apiserver_core.egg-info/
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5911 2024-04-21 18:14:11.000000 tendril_apiserver_core-0.3.5/src/tendril_apiserver_core.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1052 2024-04-21 18:14:11.000000 tendril_apiserver_core-0.3.5/src/tendril_apiserver_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-21 18:14:11.000000 tendril_apiserver_core-0.3.5/src/tendril_apiserver_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2024-04-21 18:14:11.000000 tendril_apiserver_core-0.3.5/src/tendril_apiserver_core.egg-info/entry_points.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      772 2024-04-21 18:14:11.000000 tendril_apiserver_core-0.3.5/src/tendril_apiserver_core.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-21 18:14:11.000000 tendril_apiserver_core-0.3.5/src/tendril_apiserver_core.egg-info/top_level.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      829 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.5/tox.ini
```

### Comparing `tendril_apiserver_core-0.3.4/.gitignore` & `tendril_apiserver_core-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril_apiserver_core-0.3.4/.readthedocs.yml` & `tendril_apiserver_core-0.3.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril_apiserver_core-0.3.4/.travis.yml` & `tendril_apiserver_core-0.3.5/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril_apiserver_core-0.3.4/LICENSE` & `tendril_apiserver_core-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril_apiserver_core-0.3.4/PKG-INFO` & `tendril_apiserver_core-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-apiserver-core
-Version: 0.3.4
+Version: 0.3.5
 Summary: Tendril API Server Core Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-apiserver-core
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-apiserver-core.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-apiserver-core/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-apiserver-core
```

### Comparing `tendril_apiserver_core-0.3.4/README.rst` & `tendril_apiserver_core-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `tendril_apiserver_core-0.3.4/setup.py` & `tendril_apiserver_core-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `tendril_apiserver_core-0.3.4/src/tendril/apiserver/routers/diagnostics.py` & `tendril_apiserver_core-0.3.5/src/tendril/apiserver/routers/diagnostics.py`

 * *Files identical despite different names*

### Comparing `tendril_apiserver_core-0.3.4/src/tendril/apiserver/routers/system.py` & `tendril_apiserver_core-0.3.5/src/tendril/apiserver/routers/system.py`

 * *Files identical despite different names*

### Comparing `tendril_apiserver_core-0.3.4/src/tendril/apiserver/server.py` & `tendril_apiserver_core-0.3.5/src/tendril/apiserver/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 
 
 import os
 import importlib
 import inflection
 
 from uvicorn import Config, Server
+from fastapi.requests import Request
+from fastapi.responses import JSONResponse
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi_pagination import add_pagination
 from fastapi.openapi.utils import get_openapi
 
 from tendril.config import INSTANCE_ROOT
 from tendril.config import INSTANCE_NAME
 from tendril.config import COMPONENT_NAME
@@ -66,15 +68,14 @@
         return _default_certificates()
 
     return {
         'ssl_keyfile': APISERVER_SSL_KEYFILE,
         'ssl_certfile': APISERVER_SSL_CERTFILE
     }
 
-
 def prepare_app():
     from tendril.config import APISERVER_CORS_ORIGINS
     from tendril.config import APISERVER_CORS_METHODS
     from tendril.config import APISERVER_CORS_HEADERS
 
     apiserver.add_middleware(
         CORSMiddleware,
@@ -161,14 +162,27 @@
             for exc_class, handler in m.handlers.items():
                 logger.info("Adding Translator "
                             "{0} from {1}".format(exc_class.__name__, p))
                 api_root.add_exception_handler(exc_class, handler)
         except ImportError:
             raise
 
+    @api_root.exception_handler(Exception)
+    async def catchall_exception_handler(request: Request, exc: Exception):
+        logger.exception(exc)
+        return JSONResponse(
+            status_code=500,
+            content={
+                "message": (
+                    f"Failed method {request.method} at URL {request.url}.\n"
+                    f" Exception message: \n{exc!r}."
+                )
+            }
+        )
+
     # logger.info("Preparing Swagger UI")
     # api_root.openapi_schema = tendril_openapi(api_root)
 
 
 def run_server():
     from tendril.config import APISERVER_ENABLED
```

### Comparing `tendril_apiserver_core-0.3.4/src/tendril/config/__init__.py` & `tendril_apiserver_core-0.3.5/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril_apiserver_core-0.3.4/src/tendril/config/server.py` & `tendril_apiserver_core-0.3.5/src/tendril/config/server.py`

 * *Files identical despite different names*

### Comparing `tendril_apiserver_core-0.3.4/src/tendril/resources/test_certificate.pem` & `tendril_apiserver_core-0.3.5/src/tendril/resources/test_certificate.pem`

 * *Files identical despite different names*

### Comparing `tendril_apiserver_core-0.3.4/src/tendril/resources/test_key.pem` & `tendril_apiserver_core-0.3.5/src/tendril/resources/test_key.pem`

 * *Files identical despite different names*

### Comparing `tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/PKG-INFO` & `tendril_apiserver_core-0.3.5/src/tendril_apiserver_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-apiserver-core
-Version: 0.3.4
+Version: 0.3.5
 Summary: Tendril API Server Core Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-apiserver-core
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-apiserver-core.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-apiserver-core/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-apiserver-core
```

### Comparing `tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/SOURCES.txt` & `tendril_apiserver_core-0.3.5/src/tendril_apiserver_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/requires.txt` & `tendril_apiserver_core-0.3.5/src/tendril_apiserver_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril_apiserver_core-0.3.4/tox.ini` & `tendril_apiserver_core-0.3.5/tox.ini`

 * *Files identical despite different names*


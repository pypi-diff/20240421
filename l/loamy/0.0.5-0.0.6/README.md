# Comparing `tmp/loamy-0.0.5.tar.gz` & `tmp/loamy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loamy-0.0.5.tar", max compression
+gzip compressed data, was "loamy-0.0.6.tar", max compression
```

## Comparing `loamy-0.0.5.tar` & `loamy-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-04-19 01:49:02.431992 loamy-0.0.5/LICENSE
--rw-r--r--   0        0        0     2776 2024-04-19 01:49:02.431992 loamy-0.0.5/README.md
--rw-r--r--   0        0        0     1298 2024-04-19 01:49:02.431992 loamy-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-19 01:49:02.431992 loamy-0.0.5/src/loamy/__init__.py
--rw-r--r--   0        0        0     5990 2024-04-19 01:49:02.431992 loamy-0.0.5/src/loamy/session.py
--rw-r--r--   0        0        0     3525 1970-01-01 00:00:00.000000 loamy-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-21 00:14:10.021277 loamy-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2776 2024-04-21 00:14:10.021277 loamy-0.0.6/README.md
+-rw-r--r--   0        0        0     1316 2024-04-21 00:14:10.021277 loamy-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-21 00:14:10.021277 loamy-0.0.6/src/loamy/__init__.py
+-rw-r--r--   0        0        0     6055 2024-04-21 00:14:10.021277 loamy-0.0.6/src/loamy/session.py
+-rw-r--r--   0        0        0     3525 1970-01-01 00:00:00.000000 loamy-0.0.6/PKG-INFO
```

### Comparing `loamy-0.0.5/LICENSE` & `loamy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `loamy-0.0.5/README.md` & `loamy-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `loamy-0.0.5/pyproject.toml` & `loamy-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "loamy"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = ["Zach Fuller <zach.fuller1222@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/fullerzz/loamy"
 packages = [{include = "loamy", from = "src"}]
 
@@ -20,14 +20,15 @@
 pre-commit = "3.5.0"
 pytest = "^7.4.4"
 pytest-asyncio = "^0.21.1"
 blacksheep = "^2.0.7"
 uvicorn = "^0.24.0.post1"
 mypy = "^1.9.0"
 pip-audit = "^2.7.2"
+httpx = "^0.27.0"
 
 [tool.poetry.extras]
 uvloop = ["uvloop"]
 
 [tool.ruff]
 extend-exclude = ["tests"]
 line-length = 88
```

### Comparing `loamy-0.0.5/src/loamy/session.py` & `loamy-0.0.6/src/loamy/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,16 @@
                     responses.append(
                         RequestResponse(
                             request_map=self._requestMaps[i],
                             status_code=418,
                             error=resp,
                         )
                     )
+                else:
+                    responses.append(resp)
             return responses
 
     async def _route_request(
         self, req_map: RequestMap, session: aiohttp.ClientSession
     ) -> RequestResponse:
         response: RequestResponse = RequestResponse(request_map=req_map, status_code=0)
         try:
```

### Comparing `loamy-0.0.5/PKG-INFO` & `loamy-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loamy
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Home-page: https://github.com/fullerzz/loamy
 License: MIT
 Author: Zach Fuller
 Author-email: zach.fuller1222@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


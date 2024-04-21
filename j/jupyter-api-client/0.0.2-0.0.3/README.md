# Comparing `tmp/jupyter-api-client-0.0.2.tar.gz` & `tmp/jupyter-api-client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-api-client-0.0.2.tar", last modified: Sat Apr  6 02:25:43 2024, max compression
+gzip compressed data, was "jupyter-api-client-0.0.3.tar", last modified: Sun Apr 21 01:48:49 2024, max compression
```

## Comparing `jupyter-api-client-0.0.2.tar` & `jupyter-api-client-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:25:43.976045 jupyter-api-client-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 02:25:34.000000 jupyter-api-client-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-06 02:25:43.976045 jupyter-api-client-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-06 02:25:34.000000 jupyter-api-client-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:25:43.976045 jupyter-api-client-0.0.2/jupyter_api/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-06 02:25:34.000000 jupyter-api-client-0.0.2/jupyter_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-04-06 02:25:34.000000 jupyter-api-client-0.0.2/jupyter_api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:25:43.976045 jupyter-api-client-0.0.2/jupyter_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-06 02:25:43.000000 jupyter-api-client-0.0.2/jupyter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-06 02:25:43.000000 jupyter-api-client-0.0.2/jupyter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:25:43.000000 jupyter-api-client-0.0.2/jupyter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-06 02:25:43.000000 jupyter-api-client-0.0.2/jupyter_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 02:25:43.000000 jupyter-api-client-0.0.2/jupyter_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 02:25:43.976045 jupyter-api-client-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-06 02:25:34.000000 jupyter-api-client-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:48:49.262313 jupyter-api-client-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-21 01:48:36.000000 jupyter-api-client-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-21 01:48:49.262313 jupyter-api-client-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-21 01:48:36.000000 jupyter-api-client-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:48:49.262313 jupyter-api-client-0.0.3/jupyter_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-21 01:48:36.000000 jupyter-api-client-0.0.3/jupyter_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8161 2024-04-21 01:48:36.000000 jupyter-api-client-0.0.3/jupyter_api/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:48:49.262313 jupyter-api-client-0.0.3/jupyter_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-21 01:48:49.000000 jupyter-api-client-0.0.3/jupyter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-21 01:48:49.000000 jupyter-api-client-0.0.3/jupyter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 01:48:49.000000 jupyter-api-client-0.0.3/jupyter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-21 01:48:49.000000 jupyter-api-client-0.0.3/jupyter_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 01:48:49.000000 jupyter-api-client-0.0.3/jupyter_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 01:48:49.262313 jupyter-api-client-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-21 01:48:36.000000 jupyter-api-client-0.0.3/setup.py
```

### Comparing `jupyter-api-client-0.0.2/LICENSE` & `jupyter-api-client-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-api-client-0.0.2/PKG-INFO` & `jupyter-api-client-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-api-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unofficial Python API client for Jupyter
 Home-page: https://github.com/tatsuiman/jupyter-api-client
 Author: tatsuiman
 License: UNKNOWN
 Description: # Jupyter API Client
         
         ## Setup
```

### Comparing `jupyter-api-client-0.0.2/README.md` & `jupyter-api-client-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-api-client-0.0.2/jupyter_api/client.py` & `jupyter-api-client-0.0.3/jupyter_api/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,15 +101,14 @@
         else:
             logging.error(update_response.text)
             logging.error("Failed to update notebook.")
 
     def execute_code(self, code, kernel_id, timeout=20, cell=True):
         output = ""
         outputs = []
-        execute_reply = False
         # JupyterサーバーのWebSocket URL
         session_id = uuid.uuid1().hex
         ws_url = f"{self.ws_schema}://{self.host}/api/kernels/{kernel_id}/channels?session_id={session_id}"
         # WebSocket接続の開始
         ws = websocket.create_connection(ws_url, header=self.headers, timeout=timeout)
         try:
             # 実行するコード
@@ -152,39 +151,39 @@
 
                 if msg_type == "stream":
                     text = response["content"]["text"]
                     outputs.append(
                         {"output_type": "stream", "name": "stdout", "text": text}
                     )
                     output += text
-                    if execute_reply:
-                        break
 
                 if msg_type == "display_data":
                     imgdata = response["content"]["data"]
                     outputs.append(
                         {
                             "output_type": "display_data",
                             "data": {
                                 "text/plain": [imgdata["text/plain"]],
                                 "image/png": imgdata["image/png"],
                             },
                             "metadata": {},
                         }
                     )
 
+                if msg_type == "execute_result":
+                    text = response["content"]["data"]["text/plain"]
+                    output += text
+                    outputs.append(
+                        {"output_type": "stream", "name": "stdout", "text": text}
+                    )
+
                 if msg_type == "execute_reply":
-                    execute_reply = True
+                    break
 
                 if msg_type == "status":
-                    if (
-                        response["content"]["execution_state"] == "idle"
-                        and execute_reply
-                    ):
-                        break
                     if response["content"]["execution_state"] == "restarting":
                         break
 
         except websocket._exceptions.WebSocketTimeoutException:
             pass
         finally:
             if cell:
```

### Comparing `jupyter-api-client-0.0.2/jupyter_api_client.egg-info/PKG-INFO` & `jupyter-api-client-0.0.3/jupyter_api_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-api-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unofficial Python API client for Jupyter
 Home-page: https://github.com/tatsuiman/jupyter-api-client
 Author: tatsuiman
 License: UNKNOWN
 Description: # Jupyter API Client
         
         ## Setup
```

### Comparing `jupyter-api-client-0.0.2/setup.py` & `jupyter-api-client-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         return reqs
 
 
 install_requires = get_requirements("requirements.txt")
 
 setuptools.setup(
     name="jupyter-api-client",
-    version="0.0.2",
+    version="0.0.3",
     author="tatsuiman",
     description="Unofficial Python API client for Jupyter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tatsuiman/jupyter-api-client",
     install_requires=install_requires,
     include_package_data=True,
```


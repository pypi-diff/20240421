# Comparing `tmp/logoo-1.4.0.tar.gz` & `tmp/logoo-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logoo-1.4.0.tar", last modified: Sat Apr  6 03:41:16 2024, max compression
+gzip compressed data, was "logoo-1.5.0.tar", last modified: Sun Apr 21 05:11:51 2024, max compression
```

## Comparing `logoo-1.4.0.tar` & `logoo-1.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2024-04-06 03:41:16.972739 logoo-1.4.0/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1071 2024-03-02 13:40:11.000000 logoo-1.4.0/LICENSE
--rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2830 2024-04-06 03:41:16.972739 logoo-1.4.0/PKG-INFO
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2240 2024-03-07 09:08:45.000000 logoo-1.4.0/README.md
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2024-04-06 03:41:16.968739 logoo-1.4.0/logoo/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      372 2024-04-06 03:36:57.000000 logoo-1.4.0/logoo/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       66 2024-03-02 13:50:49.000000 logoo-1.4.0/logoo/data.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2402 2024-04-06 03:23:07.000000 logoo-1.4.0/logoo/logger.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     5538 2024-04-06 03:14:06.000000 logoo-1.4.0/logoo/primary_logger.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2024-04-06 03:41:16.972739 logoo-1.4.0/logoo.egg-info/
--rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2830 2024-04-06 03:41:16.000000 logoo-1.4.0/logoo.egg-info/PKG-INFO
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      242 2024-04-06 03:41:16.000000 logoo-1.4.0/logoo.egg-info/SOURCES.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)        1 2024-04-06 03:41:16.000000 logoo-1.4.0/logoo.egg-info/dependency_links.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       36 2024-04-06 03:41:16.000000 logoo-1.4.0/logoo.egg-info/requires.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)        6 2024-04-06 03:41:16.000000 logoo-1.4.0/logoo.egg-info/top_level.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       38 2024-04-06 03:41:16.972739 logoo-1.4.0/setup.cfg
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1377 2024-03-04 06:21:58.000000 logoo-1.4.0/setup.py
+drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2024-04-21 05:11:51.203868 logoo-1.5.0/
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1071 2024-03-02 13:40:11.000000 logoo-1.5.0/LICENSE
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2830 2024-04-21 05:11:51.199868 logoo-1.5.0/PKG-INFO
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2240 2024-03-07 09:08:45.000000 logoo-1.5.0/README.md
+drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2024-04-21 05:11:51.199868 logoo-1.5.0/logoo/
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      372 2024-04-21 05:09:29.000000 logoo-1.5.0/logoo/__init__.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       66 2024-03-02 13:50:49.000000 logoo-1.5.0/logoo/data.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2402 2024-04-06 03:23:07.000000 logoo-1.5.0/logoo/logger.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     6022 2024-04-21 05:04:15.000000 logoo-1.5.0/logoo/primary_logger.py
+drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2024-04-21 05:11:51.199868 logoo-1.5.0/logoo.egg-info/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2830 2024-04-21 05:11:51.000000 logoo-1.5.0/logoo.egg-info/PKG-INFO
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      242 2024-04-21 05:11:51.000000 logoo-1.5.0/logoo.egg-info/SOURCES.txt
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)        1 2024-04-21 05:11:51.000000 logoo-1.5.0/logoo.egg-info/dependency_links.txt
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       36 2024-04-21 05:11:51.000000 logoo-1.5.0/logoo.egg-info/requires.txt
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)        6 2024-04-21 05:11:51.000000 logoo-1.5.0/logoo.egg-info/top_level.txt
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       38 2024-04-21 05:11:51.203868 logoo-1.5.0/setup.cfg
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1377 2024-03-04 06:21:58.000000 logoo-1.5.0/setup.py
```

### Comparing `logoo-1.4.0/LICENSE` & `logoo-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logoo-1.4.0/PKG-INFO` & `logoo-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logoo
-Version: 1.4.0
+Version: 1.5.0
 Summary: Openobserve log ingestion made simple.
 Author: Skelmis
 Author-email: skelmis.craft@gmail.com
 Project-URL: Issue tracker, https://github.com/Skelmis/logoo/issues
 Project-URL: Homepage, https://github.com/Skelmis/logoo
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `logoo-1.4.0/README.md` & `logoo-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `logoo-1.4.0/logoo/logger.py` & `logoo-1.5.0/logoo/logger.py`

 * *Files identical despite different names*

### Comparing `logoo-1.4.0/logoo/primary_logger.py` & `logoo-1.5.0/logoo/primary_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,66 +94,73 @@
 
     async def start_consumer(self):
         """Start the log sending task."""
         if self.__task is None:
             self.__task = asyncio.create_task(self._consume())
 
     async def _consume(self):
-        try:
-            while True:
-                await asyncio.sleep(self.poll_time)
-
-                while data_queue.qsize() != 0:
-                    data_stream = []
-                    for _ in range(self.logs_per_call):
-                        try:
-                            data = data_queue.get_nowait()
-                            if self.global_metadata is not None:
-                                data = {**data, **self.global_metadata}
-
-                            data_stream.append(data)
-                            data_queue.task_done()
-                        except QueueEmpty:
-                            break
-
-                    log.debug(
-                        "Attempting to send %s logs to %s instance",
-                        len(data_stream),
-                        self.__url,
-                    )
-
-                    resp: httpx.Response = await self.__client.post(
-                        self.__url,
-                        data=orjson.dumps(data_stream),  # type: ignore
-                    )
-                    del data_stream
-
-                    if resp.status_code != 200:
-                        log.error(
-                            "Failed to send logs to host with status code %s and response %s",
-                            resp.status_code,
-                            resp.text,
+        while True:
+            try:
+                while True:
+                    await asyncio.sleep(self.poll_time)
+
+                    while data_queue.qsize() != 0:
+                        data_stream = []
+                        for _ in range(self.logs_per_call):
+                            try:
+                                data = data_queue.get_nowait()
+                                if self.global_metadata is not None:
+                                    data = {**data, **self.global_metadata}
+
+                                data_stream.append(data)
+                                data_queue.task_done()
+                            except QueueEmpty:
+                                break
+
+                        log.debug(
+                            "Attempting to send %s logs to %s instance",
+                            len(data_stream),
+                            self.__url,
                         )
-                        continue
 
-                    resp_body = resp.json()
-                    if resp_body.get("code") == 200:
-                        for stream in resp_body.get("status", []):
-                            success = int(stream.get("successful", 0))
-                            failure = int(stream.get("failed", 0))
-                            log.debug(
-                                "Sent %s logs to stream %s. %s successful, %s failed%s",
-                                success + failure,
-                                stream.get("name"),
-                                success,
-                                failure,
-                                f'\n\tError: {stream.get("error")}' if stream.get("error") is not None else ""
-                            )
+                        resp: httpx.Response = await self.__client.post(
+                            self.__url,
+                            data=orjson.dumps(data_stream),  # type: ignore
+                        )
+                        del data_stream
 
-                    else:
-                        log.error("Something went wrong uploading logs: %s", resp_body)
+                        if resp.status_code != 200:
+                            log.error(
+                                "Failed to send logs to host with status code %s and response %s",
+                                resp.status_code,
+                                resp.text,
+                            )
+                            continue
 
-        except Exception as e:
-            log.critical(
-                "Something went wrong in the dispatcher which caused it to crash.\n%s",
-                commons.exception_as_string(e),
-            )
+                        resp_body = resp.json()
+                        if resp_body.get("code") == 200:
+                            for stream in resp_body.get("status", []):
+                                success = int(stream.get("successful", 0))
+                                failure = int(stream.get("failed", 0))
+                                log.debug(
+                                    "Sent %s logs to stream %s. %s successful, %s failed%s",
+                                    success + failure,
+                                    stream.get("name"),
+                                    success,
+                                    failure,
+                                    f'\n\tError: {stream.get("error")}' if stream.get("error") is not None else ""
+                                )
+
+                        else:
+                            log.error("Something went wrong uploading logs: %s", resp_body)
+
+            except Exception as e:
+                log.critical(
+                    "Something went wrong in the dispatcher which caused it to crash.\n%s",
+                    commons.exception_as_string(e),
+                )
+            finally:
+                await self.__client.aclose()
+                self.__client: httpx.AsyncClient = httpx.AsyncClient(
+                    headers=self.__headers,
+                )
+                log.debug("Reconfigured new instance client")
```

### Comparing `logoo-1.4.0/logoo.egg-info/PKG-INFO` & `logoo-1.5.0/logoo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logoo
-Version: 1.4.0
+Version: 1.5.0
 Summary: Openobserve log ingestion made simple.
 Author: Skelmis
 Author-email: skelmis.craft@gmail.com
 Project-URL: Issue tracker, https://github.com/Skelmis/logoo/issues
 Project-URL: Homepage, https://github.com/Skelmis/logoo
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `logoo-1.4.0/setup.py` & `logoo-1.5.0/setup.py`

 * *Files identical despite different names*


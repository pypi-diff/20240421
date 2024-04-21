# Comparing `tmp/pjrpc-1.8.3.tar.gz` & `tmp/pjrpc-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pjrpc-1.8.3.tar", max compression
+gzip compressed data, was "pjrpc-1.9.0.tar", max compression
```

## Comparing `pjrpc-1.8.3.tar` & `pjrpc-1.9.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1210 2023-12-15 13:23:46.983139 pjrpc-1.8.3/LICENSE
--rw-r--r--   0        0        0    19282 2023-12-15 13:23:46.983139 pjrpc-1.8.3/README.rst
--rw-r--r--   0        0        0      242 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/__about__.py
--rw-r--r--   0        0        0      807 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/__init__.py
--rw-r--r--   0        0        0      347 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/client/__init__.py
--rw-r--r--   0        0        0       42 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/client/backend/__init__.py
--rw-r--r--   0        0        0     6042 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/client/backend/aio_pika.py
--rw-r--r--   0        0        0     2103 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/client/backend/aiohttp.py
--rw-r--r--   0        0        0     3848 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/client/backend/httpx.py
--rw-r--r--   0        0        0     4750 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/client/backend/kombu.py
--rw-r--r--   0        0        0     1869 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/client/backend/requests.py
--rw-r--r--   0        0        0    24089 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/client/client.py
--rw-r--r--   0        0        0       46 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/client/integrations/__init__.py
--rw-r--r--   0        0        0    10207 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/client/integrations/pytest.py
--rw-r--r--   0        0        0     5652 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/client/retry.py
--rw-r--r--   0        0        0     2053 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/client/tracer.py
--rw-r--r--   0        0        0     1414 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/common/__init__.py
--rw-r--r--   0        0        0     1291 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/common/common.py
--rw-r--r--   0        0        0     5762 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/common/exceptions.py
--rw-r--r--   0        0        0     1288 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/common/generators.py
--rw-r--r--   0        0        0      685 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/common/typedefs.py
--rw-r--r--   0        0        0       76 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/common/v10.py
--rw-r--r--   0        0        0    19950 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/common/v20.py
--rw-r--r--   0        0        0        0 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/py.typed
--rw-r--r--   0        0        0      339 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/server/__init__.py
--rw-r--r--   0        0        0    21756 2023-12-15 13:23:46.991139 pjrpc-1.8.3/pjrpc/server/dispatcher.py
--rw-r--r--   0        0        0       48 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/integration/__init__.py
--rw-r--r--   0        0        0     3183 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/integration/aio_pika.py
--rw-r--r--   0        0        0     4920 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/integration/aiohttp.py
--rw-r--r--   0        0        0       34 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/integration/django/__init__.py
--rw-r--r--   0        0        0      153 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/integration/django/apps.py
--rw-r--r--   0        0        0     5393 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/integration/django/sites.py
--rw-r--r--   0        0        0      141 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/integration/django/urls.py
--rw-r--r--   0        0        0     5409 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/integration/flask.py
--rw-r--r--   0        0        0     2948 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/integration/kombu.py
--rw-r--r--   0        0        0     5243 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/integration/starlette.py
--rw-r--r--   0        0        0     1849 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/integration/werkzeug.py
--rw-r--r--   0        0        0     2090 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/specs/__init__.py
--rw-r--r--   0        0        0     3978 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/specs/extractors/__init__.py
--rw-r--r--   0        0        0     3764 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/specs/extractors/docstring.py
--rw-r--r--   0        0        0     5269 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/specs/extractors/pydantic.py
--rw-r--r--   0        0        0    37677 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/specs/openapi.py
--rw-r--r--   0        0        0    14862 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/specs/openrpc.py
--rw-r--r--   0        0        0     1766 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/typedefs.py
--rw-r--r--   0        0        0     1557 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/utils.py
--rw-r--r--   0        0        0      156 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/validators/__init__.py
--rw-r--r--   0        0        0     3193 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/validators/base.py
--rw-r--r--   0        0        0     1407 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/validators/jsonschema.py
--rw-r--r--   0        0        0     3491 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pjrpc/server/validators/pydantic.py
--rw-r--r--   0        0        0     3677 2023-12-15 13:23:46.995139 pjrpc-1.8.3/pyproject.toml
--rw-r--r--   0        0        0    22468 1970-01-01 00:00:00.000000 pjrpc-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1210 2024-04-21 19:33:40.214543 pjrpc-1.9.0/LICENSE
+-rw-r--r--   0        0        0    19282 2024-04-21 19:33:40.214543 pjrpc-1.9.0/README.rst
+-rw-r--r--   0        0        0      242 2024-04-21 19:33:40.218543 pjrpc-1.9.0/pjrpc/__about__.py
+-rw-r--r--   0        0        0      807 2024-04-21 19:33:40.218543 pjrpc-1.9.0/pjrpc/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-21 19:33:40.218543 pjrpc-1.9.0/pjrpc/client/__init__.py
+-rw-r--r--   0        0        0       42 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/client/backend/__init__.py
+-rw-r--r--   0        0        0     6042 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/client/backend/aio_pika.py
+-rw-r--r--   0        0        0     2103 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/client/backend/aiohttp.py
+-rw-r--r--   0        0        0     3848 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/client/backend/httpx.py
+-rw-r--r--   0        0        0     4750 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/client/backend/kombu.py
+-rw-r--r--   0        0        0     1869 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/client/backend/requests.py
+-rw-r--r--   0        0        0    24089 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/client/client.py
+-rw-r--r--   0        0        0       46 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/client/integrations/__init__.py
+-rw-r--r--   0        0        0    10207 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/client/integrations/pytest.py
+-rw-r--r--   0        0        0     5652 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/client/retry.py
+-rw-r--r--   0        0        0     2053 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/client/tracer.py
+-rw-r--r--   0        0        0     1414 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/common/__init__.py
+-rw-r--r--   0        0        0     1291 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/common/common.py
+-rw-r--r--   0        0        0     5762 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/common/exceptions.py
+-rw-r--r--   0        0        0     1288 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/common/generators.py
+-rw-r--r--   0        0        0      685 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/common/typedefs.py
+-rw-r--r--   0        0        0       76 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/common/v10.py
+-rw-r--r--   0        0        0    19950 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/common/v20.py
+-rw-r--r--   0        0        0        0 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/py.typed
+-rw-r--r--   0        0        0      339 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/__init__.py
+-rw-r--r--   0        0        0    21756 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/dispatcher.py
+-rw-r--r--   0        0        0       48 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/integration/__init__.py
+-rw-r--r--   0        0        0     4096 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/integration/aio_pika.py
+-rw-r--r--   0        0        0     4920 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/integration/aiohttp.py
+-rw-r--r--   0        0        0       34 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/integration/django/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/integration/django/apps.py
+-rw-r--r--   0        0        0     5393 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/integration/django/sites.py
+-rw-r--r--   0        0        0      141 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/integration/django/urls.py
+-rw-r--r--   0        0        0     5409 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/integration/flask.py
+-rw-r--r--   0        0        0     2948 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/integration/kombu.py
+-rw-r--r--   0        0        0     5243 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/integration/starlette.py
+-rw-r--r--   0        0        0     1849 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/integration/werkzeug.py
+-rw-r--r--   0        0        0     2090 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/specs/__init__.py
+-rw-r--r--   0        0        0     3978 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/specs/extractors/__init__.py
+-rw-r--r--   0        0        0     3764 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/specs/extractors/docstring.py
+-rw-r--r--   0        0        0     5269 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/specs/extractors/pydantic.py
+-rw-r--r--   0        0        0    37677 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/specs/openapi.py
+-rw-r--r--   0        0        0    14862 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/specs/openrpc.py
+-rw-r--r--   0        0        0     1766 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/typedefs.py
+-rw-r--r--   0        0        0     1557 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/utils.py
+-rw-r--r--   0        0        0      156 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/validators/__init__.py
+-rw-r--r--   0        0        0     3193 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/validators/base.py
+-rw-r--r--   0        0        0     1407 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/validators/jsonschema.py
+-rw-r--r--   0        0        0     3491 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pjrpc/server/validators/pydantic.py
+-rw-r--r--   0        0        0     3677 2024-04-21 19:33:40.222543 pjrpc-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    22468 1970-01-01 00:00:00.000000 pjrpc-1.9.0/PKG-INFO
```

### Comparing `pjrpc-1.8.3/LICENSE` & `pjrpc-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/README.rst` & `pjrpc-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/__init__.py` & `pjrpc-1.9.0/pjrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/client/backend/aio_pika.py` & `pjrpc-1.9.0/pjrpc/client/backend/aio_pika.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/client/backend/aiohttp.py` & `pjrpc-1.9.0/pjrpc/client/backend/aiohttp.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/client/backend/httpx.py` & `pjrpc-1.9.0/pjrpc/client/backend/httpx.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/client/backend/kombu.py` & `pjrpc-1.9.0/pjrpc/client/backend/kombu.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/client/backend/requests.py` & `pjrpc-1.9.0/pjrpc/client/backend/requests.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/client/client.py` & `pjrpc-1.9.0/pjrpc/client/client.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/client/integrations/pytest.py` & `pjrpc-1.9.0/pjrpc/client/integrations/pytest.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/client/retry.py` & `pjrpc-1.9.0/pjrpc/client/retry.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/client/tracer.py` & `pjrpc-1.9.0/pjrpc/client/tracer.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/common/__init__.py` & `pjrpc-1.9.0/pjrpc/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/common/common.py` & `pjrpc-1.9.0/pjrpc/common/common.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/common/exceptions.py` & `pjrpc-1.9.0/pjrpc/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/common/generators.py` & `pjrpc-1.9.0/pjrpc/common/generators.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/common/typedefs.py` & `pjrpc-1.9.0/pjrpc/common/typedefs.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/common/v20.py` & `pjrpc-1.9.0/pjrpc/common/v20.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/server/dispatcher.py` & `pjrpc-1.9.0/pjrpc/server/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/server/integration/aio_pika.py` & `pjrpc-1.9.0/pjrpc/server/integration/kombu.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,98 +1,93 @@
+"""
+kombu JSON-RPC server integration.
+"""
+
 import logging
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional, Type
 
-import aio_pika
-from yarl import URL
+import kombu.mixins
+from kombu.transport import virtual
 
 import pjrpc.server
 
 logger = logging.getLogger(__package__)
 
 
-class Executor:
+class Executor(kombu.mixins.ConsumerProducerMixin):
     """
-    `aio_pika <https://aio-pika.readthedocs.io/en/latest/>`_ based JSON-RPC server.
+    `kombu <http://kombu.readthedocs.org/>`_ based JSON-RPC server.
 
     :param broker_url: broker connection url
     :param queue_name: requests queue name
+    :param conn_args: additional connection arguments
+    :param queue_args: queue arguments
+    :param publish_args: message publish additional arguments
     :param prefetch_count: worker prefetch count
     :param kwargs: dispatcher additional arguments
     """
 
-    def __init__(self, broker_url: URL, queue_name: str, prefetch_count: int = 0, **kwargs: Any):
-        self._broker_url = broker_url
-        self._queue_name = queue_name
-        self._prefetch_count = prefetch_count
-
-        self._connection = aio_pika.connection.Connection(broker_url)
-        self._channel: Optional[aio_pika.abc.AbstractChannel] = None
+    def __init__(
+        self,
+        broker_url: str,
+        queue_name: str,
+        conn_args: Optional[Dict[str, Any]] = None,
+        queue_args: Optional[Dict[str, Any]] = None,
+        publish_args: Optional[Dict[str, Any]] = None,
+        prefetch_count: int = 0,
+        **kwargs: Any,
+    ):
+        self.connection = kombu.Connection(broker_url, **(conn_args or {}))
 
-        self._queue: Optional[aio_pika.abc.AbstractQueue] = None
-        self._consumer_tag: Optional[str] = None
+        self._rpc_queue = kombu.Queue(queue_name, **(queue_args or {}))
+        self._prefetch_count = prefetch_count
+        self._publish_args = publish_args
 
-        self._dispatcher = pjrpc.server.AsyncDispatcher(**kwargs)
+        self._dispatcher = pjrpc.server.Dispatcher(**kwargs)
 
     @property
-    def dispatcher(self) -> pjrpc.server.AsyncDispatcher:
+    def dispatcher(self) -> pjrpc.server.Dispatcher:
         """
         JSON-RPC method dispatcher.
         """
 
         return self._dispatcher
 
-    async def start(self, queue_args: Optional[Dict[str, Any]] = None) -> None:
-        """
-        Starts executor.
-
-        :param queue_args: queue arguments
-        """
-
-        await self._connection.connect()
-        self._channel = channel = await self._connection.channel()
-
-        self._queue = queue = await channel.declare_queue(self._queue_name, **(queue_args or {}))
-        await channel.set_qos(prefetch_count=self._prefetch_count)
-        self._consumer_tag = await queue.consume(self._rpc_handle)
-
-    async def shutdown(self) -> None:
-        """
-        Stops executor.
-        """
-
-        if self._consumer_tag and self._queue:
-            await self._queue.cancel(self._consumer_tag)
-        if self._channel:
-            await self._channel.close()
-
-        await self._connection.close()
+    def get_consumers(self, Consumer: Type[kombu.Consumer], channel: virtual.AbstractChannel) -> List[kombu.Consumer]:
+        return [
+            Consumer(
+                channel=channel,
+                queues=[self._rpc_queue],
+                on_message=self._rpc_handle,
+                accept={pjrpc.common.DEFAULT_CONTENT_TYPE},
+                prefetch_count=self._prefetch_count,
+            ),
+        ]
 
-    async def _rpc_handle(self, message: aio_pika.abc.AbstractIncomingMessage) -> None:
+    def _rpc_handle(self, message: kombu.Message) -> None:
         """
         Handles JSON-RPC request.
 
-        :param message: incoming message
+        :param message: kombu message :py:class:`kombu.message.Message`
         """
 
         try:
-            reply_to = message.reply_to
-            response_text = await self._dispatcher.dispatch(message.body.decode(), context=message)
+            reply_to = message.properties.get('reply_to')
+            response_text = self._dispatcher.dispatch(message.body, context=message)
 
             if response_text is not None:
                 if reply_to is None:
                     logger.warning("property 'reply_to' is missing")
                 else:
-                    async with self._connection.channel() as channel:
-                        await channel.default_exchange.publish(
-                            aio_pika.Message(
-                                body=response_text.encode(),
-                                reply_to=reply_to,
-                                correlation_id=message.correlation_id,
-                                content_type=pjrpc.common.DEFAULT_CONTENT_TYPE,
-                            ),
-                            routing_key=reply_to,
-                        )
+                    self.producer.publish(
+                        response_text,
+                        routing_key=reply_to,
+                        correlation_id=message.properties.get('correlation_id'),
+                        content_type=pjrpc.common.DEFAULT_CONTENT_TYPE,
+                        content_encoding='utf8',
+                        **(self._publish_args or {}),
+                    )
 
-            await message.ack()
+            message.ack()
 
         except Exception as e:
             logger.exception("jsonrpc request handling error: %s", e)
```

### Comparing `pjrpc-1.8.3/pjrpc/server/integration/aiohttp.py` & `pjrpc-1.9.0/pjrpc/server/integration/aiohttp.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/server/integration/django/sites.py` & `pjrpc-1.9.0/pjrpc/server/integration/django/sites.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/server/integration/flask.py` & `pjrpc-1.9.0/pjrpc/server/integration/flask.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/server/integration/starlette.py` & `pjrpc-1.9.0/pjrpc/server/integration/starlette.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/server/integration/werkzeug.py` & `pjrpc-1.9.0/pjrpc/server/integration/werkzeug.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/server/specs/__init__.py` & `pjrpc-1.9.0/pjrpc/server/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/server/specs/extractors/__init__.py` & `pjrpc-1.9.0/pjrpc/server/specs/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/server/specs/extractors/docstring.py` & `pjrpc-1.9.0/pjrpc/server/specs/extractors/docstring.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/server/specs/extractors/pydantic.py` & `pjrpc-1.9.0/pjrpc/server/specs/extractors/pydantic.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/server/specs/openapi.py` & `pjrpc-1.9.0/pjrpc/server/specs/openapi.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/server/specs/openrpc.py` & `pjrpc-1.9.0/pjrpc/server/specs/openrpc.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/server/typedefs.py` & `pjrpc-1.9.0/pjrpc/server/typedefs.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/server/utils.py` & `pjrpc-1.9.0/pjrpc/server/utils.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/server/validators/base.py` & `pjrpc-1.9.0/pjrpc/server/validators/base.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/server/validators/jsonschema.py` & `pjrpc-1.9.0/pjrpc/server/validators/jsonschema.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pjrpc/server/validators/pydantic.py` & `pjrpc-1.9.0/pjrpc/server/validators/pydantic.py`

 * *Files identical despite different names*

### Comparing `pjrpc-1.8.3/pyproject.toml` & `pjrpc-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pjrpc"
-version = "1.8.3"
+version = "1.9.0"
 description = "Extensible JSON-RPC library"
 authors = ["Dmitry Pershin <dapper1291@gmail.com>"]
 license = "Unlicense"
 readme = "README.rst"
 homepage = "https://github.com/dapper91/pjrpc"
 repository = "https://github.com/dapper91/pjrpc"
 documentation = "https://pjrpc.readthedocs.io"
```

### Comparing `pjrpc-1.8.3/PKG-INFO` & `pjrpc-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pjrpc
-Version: 1.8.3
+Version: 1.9.0
 Summary: Extensible JSON-RPC library
 Home-page: https://github.com/dapper91/pjrpc
 License: Unlicense
 Keywords: json-rpc,rpc,jsonrpc-client,jsonrpc-server,requests,aiohttp,flask,httpx,aio-pika,kombu,openapi,openrpc,starlette,django
 Author: Dmitry Pershin
 Author-email: dapper1291@gmail.com
 Requires-Python: >=3.8,<4.0
```


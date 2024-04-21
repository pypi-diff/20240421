# Comparing `tmp/minimax_client-0.5.4.tar.gz` & `tmp/minimax_client-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minimax_client-0.5.4.tar", last modified: Thu Apr 18 06:18:53 2024, max compression
+gzip compressed data, was "minimax_client-0.5.5.tar", last modified: Sun Apr 21 12:40:45 2024, max compression
```

## Comparing `minimax_client-0.5.4.tar` & `minimax_client-0.5.5.tar`

### file list

```diff
@@ -1,25 +1,29 @@
--rw-r--r--   0        0        0     1076 2024-03-06 04:02:14.299362 minimax_client-0.5.4/LICENSE.md
--rw-r--r--   0        0        0    12307 2024-04-18 06:12:14.577504 minimax_client-0.5.4/README.md
--rw-r--r--   0        0        0     2337 2024-04-18 06:18:53.053586 minimax_client-0.5.4/pyproject.toml
--rw-r--r--   0        0        0       78 2024-03-13 04:59:39.590202 minimax_client-0.5.4/src/minimax_client/__init__.py
--rw-r--r--   0        0        0       47 2024-04-18 06:17:40.850643 minimax_client-0.5.4/src/minimax_client/__version__.py
--rw-r--r--   0        0        0     5995 2024-04-12 06:44:51.187297 minimax_client-0.5.4/src/minimax_client/client.py
--rw-r--r--   0        0        0        0 2024-03-12 08:42:19.334547 minimax_client-0.5.4/src/minimax_client/entities/__init__.py
--rw-r--r--   0        0        0     2840 2024-04-12 09:41:25.234703 minimax_client-0.5.4/src/minimax_client/entities/assistant.py
--rw-r--r--   0        0        0     1431 2024-03-27 06:52:42.426086 minimax_client-0.5.4/src/minimax_client/entities/chat_completion.py
--rw-r--r--   0        0        0      651 2024-03-26 08:25:32.233150 minimax_client-0.5.4/src/minimax_client/entities/common.py
--rw-r--r--   0        0        0      288 2024-03-27 06:51:31.873794 minimax_client-0.5.4/src/minimax_client/entities/embedding.py
--rw-r--r--   0        0        0     1144 2024-03-27 06:50:23.603022 minimax_client-0.5.4/src/minimax_client/entities/file.py
--rw-r--r--   0        0        0     1956 2024-03-27 09:21:05.226495 minimax_client-0.5.4/src/minimax_client/entities/fine_tuning.py
--rw-r--r--   0        0        0     8261 2024-04-18 06:04:51.025280 minimax_client-0.5.4/src/minimax_client/entities/thread.py
--rw-r--r--   0        0        0        0 2024-03-12 08:49:51.948241 minimax_client-0.5.4/src/minimax_client/interfaces/__init__.py
--rw-r--r--   0        0        0    23479 2024-04-12 05:59:39.461781 minimax_client-0.5.4/src/minimax_client/interfaces/assistant.py
--rw-r--r--   0        0        0      532 2024-03-15 09:50:38.059327 minimax_client-0.5.4/src/minimax_client/interfaces/base.py
--rw-r--r--   0        0        0     8842 2024-04-18 06:15:41.712616 minimax_client-0.5.4/src/minimax_client/interfaces/chat_completion.py
--rw-r--r--   0        0        0     3168 2024-03-21 09:42:08.928420 minimax_client-0.5.4/src/minimax_client/interfaces/embedding.py
--rw-r--r--   0        0        0     8150 2024-03-27 06:44:53.186708 minimax_client-0.5.4/src/minimax_client/interfaces/file.py
--rw-r--r--   0        0        0    12362 2024-03-27 07:04:43.648435 minimax_client-0.5.4/src/minimax_client/interfaces/fine_tuning.py
--rw-r--r--   0        0        0    35334 2024-04-18 06:14:48.411198 minimax_client-0.5.4/src/minimax_client/interfaces/thread.py
--rw-r--r--   0        0        0        0 2024-03-06 03:45:59.529113 minimax_client-0.5.4/tests/__init__.py
--rw-r--r--   0        0        0     2412 2024-03-25 11:51:29.057995 minimax_client-0.5.4/tests/test_client.py
--rw-r--r--   0        0        0    13244 1970-01-01 00:00:00.000000 minimax_client-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-03-06 04:02:14.299362 minimax_client-0.5.5/LICENSE.md
+-rw-r--r--   0        0        0    12307 2024-04-18 06:12:14.577504 minimax_client-0.5.5/README.md
+-rw-r--r--   0        0        0     2337 2024-04-21 12:40:45.799953 minimax_client-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-03-13 04:59:39.590202 minimax_client-0.5.5/src/minimax_client/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-21 12:40:07.030057 minimax_client-0.5.5/src/minimax_client/__version__.py
+-rw-r--r--   0        0        0     6268 2024-04-19 08:40:24.666388 minimax_client-0.5.5/src/minimax_client/client.py
+-rw-r--r--   0        0        0        0 2024-03-12 08:42:19.334547 minimax_client-0.5.5/src/minimax_client/entities/__init__.py
+-rw-r--r--   0        0        0     2840 2024-04-12 09:41:25.234703 minimax_client-0.5.5/src/minimax_client/entities/assistant.py
+-rw-r--r--   0        0        0     1743 2024-04-19 09:30:46.794875 minimax_client-0.5.5/src/minimax_client/entities/audio.py
+-rw-r--r--   0        0        0     1431 2024-03-27 06:52:42.426086 minimax_client-0.5.5/src/minimax_client/entities/chat_completion.py
+-rw-r--r--   0        0        0      651 2024-03-26 08:25:32.233150 minimax_client-0.5.5/src/minimax_client/entities/common.py
+-rw-r--r--   0        0        0      288 2024-03-27 06:51:31.873794 minimax_client-0.5.5/src/minimax_client/entities/embedding.py
+-rw-r--r--   0        0        0     1157 2024-04-19 08:29:50.222873 minimax_client-0.5.5/src/minimax_client/entities/file.py
+-rw-r--r--   0        0        0     1956 2024-03-27 09:21:05.226495 minimax_client-0.5.5/src/minimax_client/entities/fine_tuning.py
+-rw-r--r--   0        0        0       28 2024-04-18 09:58:33.261586 minimax_client-0.5.5/src/minimax_client/entities/retrieval.py
+-rw-r--r--   0        0        0     8261 2024-04-18 06:04:51.025280 minimax_client-0.5.5/src/minimax_client/entities/thread.py
+-rw-r--r--   0        0        0        0 2024-03-12 08:49:51.948241 minimax_client-0.5.5/src/minimax_client/interfaces/__init__.py
+-rw-r--r--   0        0        0    23479 2024-04-12 05:59:39.461781 minimax_client-0.5.5/src/minimax_client/interfaces/assistant.py
+-rw-r--r--   0        0        0    29506 2024-04-19 09:52:33.881222 minimax_client-0.5.5/src/minimax_client/interfaces/audio.py
+-rw-r--r--   0        0        0      532 2024-03-15 09:50:38.059327 minimax_client-0.5.5/src/minimax_client/interfaces/base.py
+-rw-r--r--   0        0        0     8842 2024-04-18 06:15:41.712616 minimax_client-0.5.5/src/minimax_client/interfaces/chat_completion.py
+-rw-r--r--   0        0        0     3168 2024-03-21 09:42:08.928420 minimax_client-0.5.5/src/minimax_client/interfaces/embedding.py
+-rw-r--r--   0        0        0     8150 2024-04-19 08:40:42.905673 minimax_client-0.5.5/src/minimax_client/interfaces/file.py
+-rw-r--r--   0        0        0    12362 2024-03-27 07:04:43.648435 minimax_client-0.5.5/src/minimax_client/interfaces/fine_tuning.py
+-rw-r--r--   0        0        0       28 2024-04-18 09:59:03.537448 minimax_client-0.5.5/src/minimax_client/interfaces/retrieval.py
+-rw-r--r--   0        0        0    35341 2024-04-18 09:36:27.802413 minimax_client-0.5.5/src/minimax_client/interfaces/thread.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:45:59.529113 minimax_client-0.5.5/tests/__init__.py
+-rw-r--r--   0        0        0     2412 2024-03-25 11:51:29.057995 minimax_client-0.5.5/tests/test_client.py
+-rw-r--r--   0        0        0    13244 1970-01-01 00:00:00.000000 minimax_client-0.5.5/PKG-INFO
```

### Comparing `minimax_client-0.5.4/LICENSE.md` & `minimax_client-0.5.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.4/README.md` & `minimax_client-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.4/pyproject.toml` & `minimax_client-0.5.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP",
     "Typing :: Typed",
 ]
 dynamic = []
-version = "0.5.4"
+version = "0.5.5"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 dev = [
     "pytest>=8.1.1,<9",
```

### Comparing `minimax_client-0.5.4/src/minimax_client/client.py` & `minimax_client-0.5.5/src/minimax_client/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 from typing import Optional
 
 import httpx
 from dotenv import find_dotenv, load_dotenv
 
 from minimax_client.interfaces.assistant import Assistant, AsyncAssistant
+from minimax_client.interfaces.audio import AsyncAudio, Audio
 from minimax_client.interfaces.chat_completion import AsyncChat, Chat
 from minimax_client.interfaces.embedding import AsyncEmbedding, Embedding
 from minimax_client.interfaces.file import AsyncFiles, Files
 from minimax_client.interfaces.fine_tuning import (
     AsyncFineTuning,
     AsyncModel,
     FineTuning,
@@ -78,24 +79,26 @@
 
 
 class MiniMax(BaseMiniMaxClient):
     """MiniMax client"""
 
     http_client: httpx.Client
     assistants: Assistant
+    audio: Audio
     chat: Chat
     embeddings: Embedding
     files: Files
     fine_tuning: FineTuning
     model: Model
     threads: Threads
 
     def __init__(self, *, api_key: Optional[str] = None, timeout: float = 60) -> None:
         super().__init__(api_key=api_key, timeout=timeout)
         self.assistants = Assistant(http_client=self.http_client)
+        self.audio = Audio(http_client=self.http_client)
         self.chat = Chat(http_client=self.http_client)
         self.embeddings = Embedding(http_client=self.http_client)
         self.files = Files(http_client=self.http_client)
         self.fine_tuning = FineTuning(http_client=self.http_client)
         self.model = Model(http_client=self.http_client)
         self.threads = Threads(http_client=self.http_client)
 
@@ -114,33 +117,36 @@
 
         Returns:
             httpx.Client: The synchronous HTTP client.
         """
         return httpx.Client(
             base_url=BASE_URL,
             headers={"Authorization": f"Bearer {self.api_key}"},
+            params={"GroupId": self.group_id},
             timeout=self.timeout,
         )
 
 
 class AsyncMiniMax(BaseMiniMaxClient):
     """MiniMax async client"""
 
     http_client: httpx.AsyncClient
     assistants: AsyncAssistant
+    audio: AsyncAudio
     chat: AsyncChat
     embeddings: AsyncEmbedding
     files: AsyncFiles
     fine_tuning: AsyncFineTuning
     model: AsyncModel
     threads: AsyncThreads
 
     def __init__(self, *, api_key: Optional[str] = None, timeout: float = 60) -> None:
         super().__init__(api_key=api_key, timeout=timeout)
         self.assistants = AsyncAssistant(http_client=self.http_client)
+        self.audio = AsyncAudio(http_client=self.http_client)
         self.chat = AsyncChat(http_client=self.http_client)
         self.embeddings = AsyncEmbedding(http_client=self.http_client)
         self.files = AsyncFiles(http_client=self.http_client)
         self.fine_tuning = AsyncFineTuning(http_client=self.http_client)
         self.model = AsyncModel(http_client=self.http_client)
         self.threads = AsyncThreads(http_client=self.http_client)
```

### Comparing `minimax_client-0.5.4/src/minimax_client/entities/assistant.py` & `minimax_client-0.5.5/src/minimax_client/entities/assistant.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.4/src/minimax_client/entities/chat_completion.py` & `minimax_client-0.5.5/src/minimax_client/entities/chat_completion.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.4/src/minimax_client/entities/common.py` & `minimax_client-0.5.5/src/minimax_client/entities/common.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.4/src/minimax_client/entities/file.py` & `minimax_client-0.5.5/src/minimax_client/entities/file.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """file.py"""
 
 from typing import List, Optional
 
-from pydantic import BaseModel, NonNegativeInt
+from pydantic import BaseModel, HttpUrl, NonNegativeInt
 
 from minimax_client.entities.common import BareResponse
 
 
 class File(BaseModel):
     """
     File entity
@@ -20,15 +20,15 @@
     """
 
     file_id: NonNegativeInt
     bytes: NonNegativeInt
     created_at: int
     filename: str
     purpose: str
-    download_url: Optional[str] = None
+    download_url: Optional[HttpUrl] = None
 
 
 class FileCreateResponse(BareResponse):
     """File Create Response"""
 
     file: File
```

### Comparing `minimax_client-0.5.4/src/minimax_client/entities/fine_tuning.py` & `minimax_client-0.5.5/src/minimax_client/entities/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.4/src/minimax_client/entities/thread.py` & `minimax_client-0.5.5/src/minimax_client/entities/thread.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.4/src/minimax_client/interfaces/assistant.py` & `minimax_client-0.5.5/src/minimax_client/interfaces/assistant.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.4/src/minimax_client/interfaces/base.py` & `minimax_client-0.5.5/src/minimax_client/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.4/src/minimax_client/interfaces/chat_completion.py` & `minimax_client-0.5.5/src/minimax_client/interfaces/chat_completion.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.4/src/minimax_client/interfaces/embedding.py` & `minimax_client-0.5.5/src/minimax_client/interfaces/embedding.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.4/src/minimax_client/interfaces/file.py` & `minimax_client-0.5.5/src/minimax_client/interfaces/file.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.4/src/minimax_client/interfaces/fine_tuning.py` & `minimax_client-0.5.5/src/minimax_client/interfaces/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.4/src/minimax_client/interfaces/thread.py` & `minimax_client-0.5.5/src/minimax_client/interfaces/thread.py`

 * *Files 0% similar despite different names*

```diff
@@ -796,15 +796,15 @@
 
         if metadata:
             json_body["metadata"] = metadata
 
         async with self.client.stream(
             method="post", url=f"{self.url_path}/create_stream", json=json_body
         ) as resp:
-            for data_text in resp.iter_text():
+            async for data_text in resp.aiter_text():
                 if not data_text.startswith("data:"):
                     continue
 
                 data_json = json.loads(data_text.split("data: ", 2)[1])
 
                 if not data_json.get("data"):
                     continue
```

### Comparing `minimax_client-0.5.4/tests/test_client.py` & `minimax_client-0.5.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.4/PKG-INFO` & `minimax_client-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minimax-client
-Version: 0.5.4
+Version: 0.5.5
 Summary: An (unofficial) python native client for easy interaction with MiniMax Open Platform
 Keywords: web,api,llm
 Author-Email: Zeyang Lin <4020306+linzeyang@users.noreply.github.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```


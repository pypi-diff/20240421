# Comparing `tmp/async_VKsher-1.7.1.tar.gz` & `tmp/async_VKsher-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_VKsher-1.7.1.tar", last modified: Sat Apr 20 15:46:57 2024, max compression
+gzip compressed data, was "async_VKsher-1.7.2.tar", last modified: Sun Apr 21 17:41:52 2024, max compression
```

## Comparing `async_VKsher-1.7.1.tar` & `async_VKsher-1.7.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 15:46:57.621492 async_VKsher-1.7.1/
--rw-rw-rw-   0        0        0    35149 2022-07-25 16:43:52.000000 async_VKsher-1.7.1/LICENSE
--rw-rw-rw-   0        0        0    28089 2024-04-20 15:46:57.620494 async_VKsher-1.7.1/PKG-INFO
--rw-rw-rw-   0        0        0    27096 2024-04-20 15:22:35.000000 async_VKsher-1.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 15:46:57.609523 async_VKsher-1.7.1/asyncVK/
--rw-rw-rw-   0        0        0     4177 2024-04-20 14:40:33.000000 async_VKsher-1.7.1/asyncVK/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:46:57.610520 async_VKsher-1.7.1/asyncVK/asyncDB/
--rw-rw-rw-   0        0        0     1199 2021-12-13 13:50:31.000000 async_VKsher-1.7.1/asyncVK/asyncDB/__init__.py
--rw-rw-rw-   0        0        0     1557 2022-07-26 07:13:15.000000 async_VKsher-1.7.1/asyncVK/chain.py
--rw-rw-rw-   0        0        0     1912 2021-12-13 12:57:10.000000 async_VKsher-1.7.1/asyncVK/condition.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:46:57.612515 async_VKsher-1.7.1/asyncVK/core/
--rw-rw-rw-   0        0        0     2364 2024-04-20 15:15:28.000000 async_VKsher-1.7.1/asyncVK/core/__init__.py
--rw-rw-rw-   0        0        0     3639 2024-04-20 14:56:50.000000 async_VKsher-1.7.1/asyncVK/dispatcher.py
--rw-rw-rw-   0        0        0     2690 2024-04-20 15:13:40.000000 async_VKsher-1.7.1/asyncVK/handlers.py
--rw-rw-rw-   0        0        0      731 2021-02-02 06:00:48.000000 async_VKsher-1.7.1/asyncVK/keyboard.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:46:57.612515 async_VKsher-1.7.1/asyncVK/upload/
--rw-rw-rw-   0        0        0       91 2022-07-26 07:31:37.000000 async_VKsher-1.7.1/asyncVK/upload/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:46:57.619496 async_VKsher-1.7.1/async_VKsher.egg-info/
--rw-rw-rw-   0        0        0    28089 2024-04-20 15:46:57.000000 async_VKsher-1.7.1/async_VKsher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2024-04-20 15:46:57.000000 async_VKsher-1.7.1/async_VKsher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 15:46:57.000000 async_VKsher-1.7.1/async_VKsher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-20 15:46:57.000000 async_VKsher-1.7.1/async_VKsher.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-20 15:46:57.000000 async_VKsher-1.7.1/async_VKsher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 15:46:57.622489 async_VKsher-1.7.1/setup.cfg
--rw-rw-rw-   0        0        0      805 2024-04-20 15:46:50.000000 async_VKsher-1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 17:41:52.397068 async_VKsher-1.7.2/
+-rw-rw-rw-   0        0        0    35149 2022-07-25 16:43:52.000000 async_VKsher-1.7.2/LICENSE
+-rw-rw-rw-   0        0        0    28118 2024-04-21 17:41:52.394479 async_VKsher-1.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0    27096 2024-04-20 15:22:35.000000 async_VKsher-1.7.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 17:41:52.374927 async_VKsher-1.7.2/asyncVK/
+-rw-rw-rw-   0        0        0     4050 2024-04-21 16:26:30.000000 async_VKsher-1.7.2/asyncVK/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 17:41:52.376922 async_VKsher-1.7.2/asyncVK/asyncDB/
+-rw-rw-rw-   0        0        0     1199 2021-12-13 13:50:31.000000 async_VKsher-1.7.2/asyncVK/asyncDB/__init__.py
+-rw-rw-rw-   0        0        0     1548 2024-04-21 15:33:16.000000 async_VKsher-1.7.2/asyncVK/chain.py
+-rw-rw-rw-   0        0        0     1912 2021-12-13 12:57:10.000000 async_VKsher-1.7.2/asyncVK/condition.py
+drwxrwxrwx   0        0        0        0 2024-04-21 17:41:52.378880 async_VKsher-1.7.2/asyncVK/core/
+-rw-rw-rw-   0        0        0     2364 2024-04-20 15:15:28.000000 async_VKsher-1.7.2/asyncVK/core/__init__.py
+-rw-rw-rw-   0        0        0     2859 2024-04-21 16:28:22.000000 async_VKsher-1.7.2/asyncVK/dispatcher.py
+-rw-rw-rw-   0        0        0     2672 2024-04-21 15:29:06.000000 async_VKsher-1.7.2/asyncVK/handlers.py
+-rw-rw-rw-   0        0        0      731 2021-02-02 06:00:48.000000 async_VKsher-1.7.2/asyncVK/keyboard.py
+drwxrwxrwx   0        0        0        0 2024-04-21 17:41:52.392379 async_VKsher-1.7.2/async_VKsher.egg-info/
+-rw-rw-rw-   0        0        0    28118 2024-04-21 17:41:52.000000 async_VKsher-1.7.2/async_VKsher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2024-04-21 17:41:52.000000 async_VKsher-1.7.2/async_VKsher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 17:41:52.000000 async_VKsher-1.7.2/async_VKsher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-21 17:41:52.000000 async_VKsher-1.7.2/async_VKsher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-21 17:41:52.000000 async_VKsher-1.7.2/async_VKsher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 17:41:52.397068 async_VKsher-1.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      821 2024-04-21 17:41:31.000000 async_VKsher-1.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 17:41:52.389439 async_VKsher-1.7.2/upload/
+-rw-rw-rw-   0        0        0      786 2024-04-21 17:36:26.000000 async_VKsher-1.7.2/upload/__init__.py
```

### Comparing `async_VKsher-1.7.1/LICENSE` & `async_VKsher-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.1/PKG-INFO` & `async_VKsher-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: async_VKsher
-Version: 1.7.1
+Version: 1.7.2
 Summary: asyncVK is asynchronous library for creating a bot in VK
 Home-page: https://github.com/Ekventor/asyncVK
 Author: Kulenov Islam
 Author-email: kit.werr34@gmail.com
 Keywords: vk vkontakte вк вконтакте бот bot
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asyncio>=3
 Requires-Dist: aiohttp>=3
+Requires-Dist: aiofiles>=22
 
 asyncVK – асинхронный фреймворк для создания ботов ВК. Преимущества: удобство, скорость выигрываемая за счёт асинхронности.
 =
 
 Бот создаётся за счёт шести структурных единиц: 
 1) Bot – это самая главная структурная единица. Это собственно сам бот, который подаёт ивенты     обработчикам.
 2) Handler – эта структурная единица отвечает за обработку ивентов.
```

### Comparing `async_VKsher-1.7.1/README.md` & `async_VKsher-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.1/asyncVK/__init__.py` & `async_VKsher-1.7.2/asyncVK/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,104 +1,102 @@
 import asyncio
 import aiohttp
 import traceback
 import sys
 
-from typing import Union
-
 from . import handlers
 from .chain import Chain
 from .core import VERSION, get_event_params
 
 
 class Handler:
     on = handlers.Handlers
 
 
 class Bot:
     def __init__(self, token: str, group_id: int):
+        self.session = aiohttp.ClientSession()
         self.token = token
         self.group_id = group_id
         self.config = {}
         self.handlers = []
         self.users_in_chain = []
         self.chains = []
         self.bound_chains = []
 
-    def handle(self, handler: Union[handlers.Handler]) -> handlers.Handler:
+    def handle(self, handler: handlers.Handler) -> handlers.Handler:
         self.handlers.append(handler)
         return handler
 
     def add_chain(self, chain: Chain) -> Chain:
         self.chains.append(chain)
         return chain
 
     async def run_polling(self) -> None:
-        async with aiohttp.ClientSession() as session:
-            async with session.get("https://api.vk.com/method/groups.getLongPollServer",
-                                   params=f"group_id={self.group_id}&access_token={self.token}&v={VERSION}") as response:
-                config = await response.json()
-                print(config)
-                self.config = config["response"]
-                self.config["server"] = self.config["server"].replace("https://", "")
-
-                async with session.get("https://api.vk.com/method/groups.getLongPollSettings",
-                                       params=f"group_id={self.group_id}&access_token={self.token}&v={VERSION}") as response:
-                    print(await response.json())
-
-                while True:
-                    try:
-                        async with session.get(f"https://%s?act=a_check&key=%s&ts=%s&wait=60&mode=2&version={VERSION}" % (
-                        self.config["server"], self.config["key"], self.config["ts"])) as response:
-                            event = await response.json()
-                            updates = event["updates"]
-                            if len(updates) == 0:
-                                continue
-                            print(updates)
+        async with self.session.get("https://api.vk.com/method/groups.getLongPollServer",
+                                    params=f"group_id={self.group_id}&access_token={self.token}&v={VERSION}") as response:
+            config = await response.json()
+            print(config)
+            self.config = config["response"]
+            self.config["server"] = self.config["server"].replace("https://", "")
+
+            async with self.session.get("https://api.vk.com/method/groups.getLongPollSettings",
+                                        params=f"group_id={self.group_id}&access_token={self.token}&v={VERSION}") as response:
+                print(await response.json())
+
+            while True:
+                try:
+                    async with self.session.get(f"https://%s?act=a_check&key=%s&ts=%s&wait=60&mode=2&version={VERSION}" % (
+                               self.config["server"], self.config["key"], self.config["ts"])) as response:
+                        event = await response.json()
+                        updates = event["updates"]
+                        if len(updates) == 0:
+                            continue
+                        print(updates)
 
-                            self.config["ts"] = event["ts"]
+                        self.config["ts"] = event["ts"]
 
-                            asyncio.create_task(self.send_event(updates[0]))
+                        asyncio.create_task(self.send_event(updates[0]))
 
-                    except:
-                        sys.stderr.write(f"\n\n{traceback.format_exc()}\n\n")
+                except:
+                    sys.stderr.write(f"\n\n{traceback.format_exc()}\n\n")
 
     async def send_event(self, event: dict) -> None:
         event_type = event["type"]
         event_params = get_event_params(event, event_type)
 
         if event_params["user_id"] not in self.users_in_chain:
             for chain in self.chains:
                 if chain.is_trigger(event_params):
                     self.bound_chains.append(chain.bind_chain(event_params["user_id"]))
                     self.users_in_chain.append(event_params["user_id"])
                     break
 
         active_chains = [chain for chain in self.bound_chains if chain.is_trigger(event_type, event_params["user_id"])]
-        tasks = [asyncio.create_task(chain.new_event(self.token, event, event_params))
+        tasks = [asyncio.create_task(chain.new_event(self, event, event_params))
                  for chain in active_chains]
 
         for future in asyncio.as_completed(tasks):
             result = await future
             if not result[0]:
                 self.bound_chains.remove(result[1])
                 self.users_in_chain.remove(event_params["user_id"])
 
         active_handlers = [handler for handler in self.handlers if handler.is_trigger(event_params)]
-        tasks = [asyncio.create_task(handler.new_event(self.token, event, event_params))
+        tasks = [asyncio.create_task(handler.new_event(self, event, event_params))
                  for handler in active_handlers]
         await asyncio.gather(*tasks)
 
     async def execute(self, method: str, **params) -> dict:
         query = f"https://api.vk.com/method/{method}?"
         for key, value in params.items():
-            query += f"{key}={value}&"
+            if value is not None:
+                query += f"{key}={value}&"
         query += f"access_token={self.token}&v={VERSION}"
 
-        async with aiohttp.ClientSession() as session:
-            async with session.get(query) as response:
-                return await response.json()
+        async with self.session.get(query) as response:
+            return await response.json()
 
 
 def run_polling(bot: Bot) -> None:
     loop = asyncio.get_event_loop()
     loop.run_until_complete(bot.run_polling())
```

### Comparing `async_VKsher-1.7.1/asyncVK/asyncDB/__init__.py` & `async_VKsher-1.7.2/asyncVK/asyncDB/__init__.py`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.1/asyncVK/chain.py` & `async_VKsher-1.7.2/asyncVK/chain.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,18 @@
         self.handlers = handlers
         self.user_id = user_id
         self.data = None
 
     def is_trigger(self, event_type: str, user_id: int) -> bool:
         return event_type == self.handlers[0].event_type and user_id == self.user_id
 
-    async def new_event(self, token: str, event: dict, event_params: dict) -> Tuple:
+    async def new_event(self, bot, event: dict, event_params: dict) -> Tuple:
         handler = self.handlers[0]
         if handler.is_trigger(event_params):
-            data = await handler.new_event(token, event, event_params, self.data)
+            data = await handler.new_event(bot, event, event_params, self.data)
             if isinstance(data, Reject):
                 return False, self
         else:
             return False, self
 
         if not isinstance(data, Reset):
             self.handlers.pop(0)
```

### Comparing `async_VKsher-1.7.1/asyncVK/condition.py` & `async_VKsher-1.7.2/asyncVK/condition.py`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.1/asyncVK/core/__init__.py` & `async_VKsher-1.7.2/asyncVK/core/__init__.py`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.1/asyncVK/dispatcher.py` & `async_VKsher-1.7.2/asyncVK/dispatcher.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,57 @@
 from typing import Any
-import aiohttp
-
-from .core import VERSION
 
 
 class Dispatcher:
-    def __init__(self, event: dict, token: str, text: str = None, user_id: int = None, peer_id: int = None,
+    def __init__(self, event: dict, bot, text: str = None, user_id: int = None, peer_id: int = None,
                  post_id: int = None, owner_id: int = None, reply_text: str = None, reply_user_id: int = None,
                  reply_peer_id: int = None, chain_data: Any = None):
-        self.token = token
+        self.bot = bot
         self.user_id = user_id
         self.peer_id = peer_id
+        self.chat_id = peer_id - 2000000000
         self.post_id = post_id
         self.owner_id = owner_id
         self.event = event
         self.text = text
         self.reply_text = reply_text
         self.reply_user_id = reply_user_id
         self.reply_peer_id = reply_peer_id
         self.chain_data = chain_data
 
-    async def answer(self, text: str, attachment: str = None, keyboard: str = None) -> None:
-        params = f"user_id={self.user_id}&message={text}&random_id=0"
-        if attachment is not None:
-            params += f"&attachment={attachment}"
-        if keyboard is not None:
-            params += f"keyboard={keyboard}"
-        params += f"&access_token={self.token}&v={VERSION}"
-
-        async with aiohttp.ClientSession() as session:
-            await session.post("https://api.vk.com/method/messages.send", params=params)
-
-    async def send_message(self, text: str, attachment: str = None, keyboard: str = None) -> None:
-        params = f"peer_id={self.peer_id}&message={text}&random_id=0"
-        if attachment is not None:
-            params += f"&attachment={attachment}"
-        if keyboard is not None:
-            params += f"&keyboard={keyboard}"
-        params += f"&access_token={self.token}&v={VERSION}"
-
-        async with aiohttp.ClientSession() as session:
-            await session.post("https://api.vk.com/method/messages.send", params=params)
-
-    async def send_comment(self, text: str, attachment: str = None) -> None:
-        params = f"owner_id={self.owner_id}&post_id={self.post_id}&message={text}"
-        if attachment is not None:
-            params += f"&attachment={attachment}"
-        params += f"&access_token={self.token}&v={VERSION}"
-
-        async with aiohttp.ClientSession() as session:
-            await session.post("https://api.vk.com/method/wall.createComment", params=params)
+    async def answer(self, text: str = None, attachment: str = None, keyboard: str = None) -> None:
+        await self.bot.execute("messages.send", message=text, user_id=self.user_id,
+                               random_id=0, attachment=attachment, keyboard=keyboard)
+
+    async def send_message(self, text: str = None, attachment: str = None, keyboard: str = None) -> None:
+        await self.bot.execute("messages.send", message=text, peer_id=self.peer_id,
+                               random_id=0, attachment=attachment, keyboard=keyboard)
+
+    async def send_comment(self, text: str = None, attachment: str = None) -> None:
+        await self.bot.execute("wall.createComment",
+                               owner_id=self.owner_id, post_id=self.post_id, message=text, attachment=attachment)
 
     async def mark_as_read(self) -> None:
-        params = f"peer_id={self.peer_id}&access_token={self.token}&v={VERSION}"
-
-        async with aiohttp.ClientSession() as session:
-            await session.post("https://api.vk.com/method/messages.markAsRead", params=params)
+        await self.bot.execute("messages.markAsRead", peer_id=self.peer_id)
 
     async def set_typing_status(self, typing_status: str = "typing") -> None:
-        params = f"peer_id={self.peer_id}&type={typing_status}&access_token={self.token}&v={VERSION}"
+        await self.bot.execute("messages.setActivity", peer_id=self.peer_id, type=typing_status)
+
+    async def kick_user(self, member_id: int) -> None:
+        await self.bot.execute("messages.removeChatUser", chat_id=self.chat_id, member_id=member_id)
 
-        async with aiohttp.ClientSession() as session:
-            await session.post("https://api.vk.com/method/messages.setActivity", params=params)
+    async def edit_chat_name(self, title: str) -> None:
+        await self.bot.execute("messages.editChat", chat_id=self.chat_id, title=title)
 
 
-def get_dispatcher_by_event(token: str, event: dict, event_params: dict, chain_data: Any) -> Dispatcher:
+def get_dispatcher_by_event(bot, event: dict, event_params: dict, chain_data: Any) -> Dispatcher:
     text = event_params["text"]
     user_id = event_params["user_id"]
     peer_id = event_params["peer_id"]
     post_id = event_params["post_id"]
     owner_id = event_params["owner_id"]
     reply_message = event_params["reply_message"]
 
-    return Dispatcher(event=event, token=token, text=text, user_id=user_id, peer_id=peer_id,
+    return Dispatcher(event=event, bot=bot, text=text, user_id=user_id, peer_id=peer_id,
                       post_id=post_id, owner_id=owner_id, reply_text=reply_message.get("text"),
                       reply_peer_id=reply_message.get("peer_id"), reply_user_id=reply_message.get("user_id"),
                       chain_data=chain_data)
```

### Comparing `async_VKsher-1.7.1/asyncVK/handlers.py` & `async_VKsher-1.7.2/asyncVK/handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 
     def __init__(self, condition: Union[Condition, And, Or] = None, is_lower: bool = False, func=None):
         self.condition = condition
         self.is_lower = is_lower
         self.func = func
 
     def __call__(self, func):
-        async def wrapper(token: str, event: dict, event_params: dict, chain_data: Any):
-            return await func(get_dispatcher_by_event(token, event, event_params, chain_data))
+        async def wrapper(bot, event: dict, event_params: dict, chain_data: Any):
+            return await func(get_dispatcher_by_event(bot, event, event_params, chain_data))
 
         return type(self)(self.condition, self.is_lower, wrapper)
 
     def is_trigger(self, event_params: dict) -> bool:
         if event_params["type"] != self.event_type:
             return False
 
         if self.is_lower:
             if event_params["text"]:
                 event_params["text"] = event_params["text"].lower()
 
         return self.condition is None or self.condition.new_event(event_params)
 
-    async def new_event(self, token: str, event: dict, event_params: dict, chain_data: Any = None) -> Any:
+    async def new_event(self, bot, event: dict, event_params: dict, chain_data: Any = None) -> Any:
         try:
-            return await self.func(token, event, event_params, chain_data)
+            return await self.func(bot, event, event_params, chain_data)
         except:
             sys.stderr.write(f"\n\n{traceback.format_exc()}\n\n")
 
 
 class CustomHandler(Handler):
     def __call__(self, func):
         async def wrapper(token: str, event: dict, event_params: dict, chain_data: Any):
```

### Comparing `async_VKsher-1.7.1/asyncVK/keyboard.py` & `async_VKsher-1.7.2/asyncVK/keyboard.py`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.1/async_VKsher.egg-info/PKG-INFO` & `async_VKsher-1.7.2/async_VKsher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: async_VKsher
-Version: 1.7.1
+Version: 1.7.2
 Summary: asyncVK is asynchronous library for creating a bot in VK
 Home-page: https://github.com/Ekventor/asyncVK
 Author: Kulenov Islam
 Author-email: kit.werr34@gmail.com
 Keywords: vk vkontakte вк вконтакте бот bot
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asyncio>=3
 Requires-Dist: aiohttp>=3
+Requires-Dist: aiofiles>=22
 
 asyncVK – асинхронный фреймворк для создания ботов ВК. Преимущества: удобство, скорость выигрываемая за счёт асинхронности.
 =
 
 Бот создаётся за счёт шести структурных единиц: 
 1) Bot – это самая главная структурная единица. Это собственно сам бот, который подаёт ивенты     обработчикам.
 2) Handler – эта структурная единица отвечает за обработку ивентов.
```

### Comparing `async_VKsher-1.7.1/setup.py` & `async_VKsher-1.7.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 
 with open("README.md", "r", encoding="UTF-8") as file:
     readme = file.read()
 
 
-requirements = ["asyncio>=3", "aiohttp>=3"]
+requirements = ["asyncio>=3", "aiohttp>=3", "aiofiles>=22"]
 
 
 setup(
     name="async_VKsher",
-    version="1.7.1",
+    version="1.7.2",
     author="Kulenov Islam",
     author_email="kit.werr34@gmail.com",
     description="asyncVK is asynchronous library for creating a bot in VK",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/Ekventor/asyncVK",
     packages=find_packages(),
```


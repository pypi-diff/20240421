# Comparing `tmp/queue_api-0.1.1.tar.gz` & `tmp/queue_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queue_api-0.1.1.tar", last modified: Thu Apr 18 18:44:03 2024, max compression
+gzip compressed data, was "queue_api-0.1.2.tar", last modified: Sun Apr 21 18:04:12 2024, max compression
```

## Comparing `queue_api-0.1.1.tar` & `queue_api-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,34 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 18:44:03.746510 queue_api-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      291 2024-04-18 18:44:03.736510 queue_api-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       34 2024-04-15 16:36:13.000000 queue_api-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      505 2024-04-18 18:43:58.000000 queue_api-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-18 18:44:03.746510 queue_api-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 18:44:03.726510 queue_api-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 18:44:03.726510 queue_api-0.1.1/src/q/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 18:44:03.726510 queue_api-0.1.1/src/q/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      150 2024-04-18 18:43:49.000000 queue_api-0.1.1/src/q/api/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 18:44:03.736510 queue_api-0.1.1/src/q/api/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-04-18 18:43:45.000000 queue_api-0.1.1/src/q/api/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      217 2024-04-18 18:43:40.000000 queue_api-0.1.1/src/q/api/api/connect_.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      172 2024-04-15 16:36:13.000000 queue_api-0.1.1/src/q/api/api/queue.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5912 2024-04-18 17:03:04.000000 queue_api-0.1.1/src/q/api/api/read.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2543 2024-04-17 17:55:51.000000 queue_api-0.1.1/src/q/api/api/write.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 18:44:03.736510 queue_api-0.1.1/src/q/api/extensions/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       52 2024-04-15 18:48:24.000000 queue_api-0.1.1/src/q/api/extensions/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      653 2024-04-15 18:48:19.000000 queue_api-0.1.1/src/q/api/extensions/appendable.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 18:44:03.736510 queue_api-0.1.1/src/q/api/extensions/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-04-15 17:52:29.000000 queue_api-0.1.1/src/q/api/extensions/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1121 2024-04-15 18:48:13.000000 queue_api-0.1.1/src/q/api/extensions/ops/bounding.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 18:44:03.736510 queue_api-0.1.1/src/q/api/impl/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-04-15 16:36:13.000000 queue_api-0.1.1/src/q/api/impl/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      385 2024-04-15 16:36:13.000000 queue_api-0.1.1/src/q/api/impl/empty.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1200 2024-04-15 16:36:13.000000 queue_api-0.1.1/src/q/api/impl/simple.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 18:44:03.736510 queue_api-0.1.1/src/q/api/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      142 2024-04-15 17:52:36.000000 queue_api-0.1.1/src/q/api/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1112 2024-04-15 17:52:34.000000 queue_api-0.1.1/src/q/api/ops/bounding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1495 2024-04-15 16:36:13.000000 queue_api-0.1.1/src/q/api/ops/interleaving.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1741 2024-04-15 16:36:13.000000 queue_api-0.1.1/src/q/api/ops/merging.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1984 2024-04-15 16:36:13.000000 queue_api-0.1.1/src/q/api/ops/splitting.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 18:44:03.736510 queue_api-0.1.1/src/queue_api.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      291 2024-04-18 18:44:03.000000 queue_api-0.1.1/src/queue_api.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      666 2024-04-18 18:44:03.000000 queue_api-0.1.1/src/queue_api.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-18 18:44:03.000000 queue_api-0.1.1/src/queue_api.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-04-18 18:44:03.000000 queue_api-0.1.1/src/queue_api.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:12.519883 queue_api-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-21 18:04:12.519883 queue_api-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-04-21 17:59:12.000000 queue_api-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      565 2024-04-21 18:04:09.000000 queue_api-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-21 18:04:12.519883 queue_api-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:12.509883 queue_api-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:12.509883 queue_api-0.1.2/src/q/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:12.509883 queue_api-0.1.2/src/q/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      149 2024-04-21 18:00:51.000000 queue_api-0.1.2/src/q/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      228 2024-04-21 18:01:43.000000 queue_api-0.1.2/src/q/api/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:12.509883 queue_api-0.1.2/src/q/api/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      131 2024-04-21 18:01:20.000000 queue_api-0.1.2/src/q/api/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      649 2024-04-21 17:59:44.000000 queue_api-0.1.2/src/q/api/api/append.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      172 2024-04-15 16:36:13.000000 queue_api-0.1.2/src/q/api/api/queue.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5901 2024-04-21 17:48:09.000000 queue_api-0.1.2/src/q/api/api/read.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2723 2024-04-21 17:48:29.000000 queue_api-0.1.2/src/q/api/api/write.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:12.509883 queue_api-0.1.2/src/q/api/impl/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-04-15 16:36:13.000000 queue_api-0.1.2/src/q/api/impl/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      385 2024-04-15 16:36:13.000000 queue_api-0.1.2/src/q/api/impl/empty.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1180 2024-04-21 17:50:16.000000 queue_api-0.1.2/src/q/api/impl/simple.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:12.519883 queue_api-0.1.2/src/q/api/ops/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 17:58:36.000000 queue_api-0.1.2/src/q/api/ops/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      286 2024-04-21 17:59:26.000000 queue_api-0.1.2/src/q/api/ops/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1113 2024-04-21 17:58:13.000000 queue_api-0.1.2/src/q/api/ops/append_bounding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1105 2024-04-21 17:50:36.000000 queue_api-0.1.2/src/q/api/ops/bounding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1479 2024-04-21 17:50:49.000000 queue_api-0.1.2/src/q/api/ops/interleaving.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1735 2024-04-21 17:51:01.000000 queue_api-0.1.2/src/q/api/ops/merging.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1978 2024-04-21 17:51:05.000000 queue_api-0.1.2/src/q/api/ops/splitting.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:12.519883 queue_api-0.1.2/src/queue_api.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-21 18:04:12.000000 queue_api-0.1.2/src/queue_api.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      641 2024-04-21 18:04:12.000000 queue_api-0.1.2/src/queue_api.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-21 18:04:12.000000 queue_api-0.1.2/src/queue_api.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       23 2024-04-21 18:04:12.000000 queue_api-0.1.2/src/queue_api.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-04-21 18:04:12.000000 queue_api-0.1.2/src/queue_api.egg-info/top_level.txt
```

### Comparing `queue_api-0.1.1/src/q/api/api/read.py` & `queue_api-0.1.2/src/q/api/api/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Generic, Never, TypeVar, Callable, Awaitable, overload, AsyncIterable, AsyncIterator, TypeGuard
-from haskellian.asyn.iter import AsyncIter
-from haskellian.asyn.promises import of
+from haskellian import AsyncIter, promise as P
 from abc import ABC, abstractmethod
 
 A = TypeVar('A', covariant=True)
 B = TypeVar('B', covariant=True)
 
 class ReadQueue(ABC, AsyncIterator[tuple[str, A]], Generic[A]):
   
@@ -58,27 +57,27 @@
         yield x
     return AsyncIter(iterate())
   
   __aiter__ = iter
   
   def map(self, f: Callable[[A], B]) -> 'ReadQueue[B]':
     """Maps `f` over self. Returns a new queue, but `self` is still mutated when popping from the new queue"""
-    return MappedQueue(self, lambda kv: of((kv[0], f(kv[1]))))
+    return MappedQueue(self, lambda kv: P.of((kv[0], f(kv[1]))))
   
   def map_kv(self, f: Callable[[str, A], B]) -> 'ReadQueue[B]':
     """Map but `f` receives both key and value"""
-    return MappedQueue(self, lambda kv: of((kv[0], f(*kv))))
+    return MappedQueue(self, lambda kv: P.of((kv[0], f(*kv))))
   
   def map_k(self, f: Callable[[str], B]) -> 'ReadQueue[B]':
     """Map but `f` receives the key"""
-    return MappedQueue(self, lambda kv: of((kv[0], f(kv[0]))))
+    return MappedQueue(self, lambda kv: P.of((kv[0], f(kv[0]))))
   
   def map_kvt(self, f: Callable[[tuple[str, A]], B]) -> 'ReadQueue[B]':
     """Map but `f` receives both key and value as a tuple"""
-    return MappedQueue(self, lambda kv: of((kv[0], f(kv))))
+    return MappedQueue(self, lambda kv: P.of((kv[0], f(kv))))
   
   def amap(self, f: Callable[[A], Awaitable[B]]) -> 'ReadQueue[B]':
     """Map but `f` is asynchronous"""
     async def mapper(kv: tuple[str, A]):
       return kv[0], await f(kv[1])
     return MappedQueue(self, mapper)
   
@@ -100,15 +99,15 @@
       return kv[0], await f(kv)
     return MappedQueue(self, mapper)
 
   @overload
   def filter(self, pred: Callable[[A], TypeGuard[B]]) -> 'ReadQueue[B]': ...
   @overload
   def filter(self, pred: Callable[[A], bool]) -> 'ReadQueue[A]': ...
-  def filter(self, pred):
+  def filter(self, pred): # type: ignore
     return FilteredQueue(self, lambda _, v: pred(v))
   
   @overload
   def filter(self, pred: Callable[[str, A], TypeGuard[B]]) -> 'ReadQueue[B]': ...
   @overload
   def filter(self, pred: Callable[[str, A], bool]) -> 'ReadQueue[A]': ...
   def filter_kv(self, pred):
@@ -116,15 +115,15 @@
   
   def partition(self, pred: Callable[[A], bool]) -> 'tuple[ReadQueue[A], ReadQueue[A]]':
     """Returns `self.filter(pred), self.filter(!pred)`"""
     return self.filter(pred), self.filter(lambda x: not pred(x))
   
   def partition_kv(self, pred: Callable[[str, A], bool]) -> 'tuple[ReadQueue[A], ReadQueue[A]]':
     """Returns `self.filter_kv(pred), self.filter_kv(!pred)`"""
-    return self.filter_kv(pred), self.filter_kv(lambda x: not pred(x))
+    return self.filter_kv(pred), self.filter_kv(lambda *x: not pred(*x))
   
   
 class MappedQueue(ReadQueue[B], Generic[A, B]):
   
   def __init__(self, q: ReadQueue[A], f: Callable[[tuple[str, A]], Awaitable[tuple[str, B]]]):
     self._wrapped = q
     self._mapper = f
```

### Comparing `queue_api-0.1.1/src/q/api/api/write.py` & `queue_api-0.1.2/src/q/api/api/write.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,43 @@
-from typing import Generic, TypeVar, Callable, Awaitable
-from haskellian.asyn.promises import of
+from typing import Generic, TypeVar, Callable, Awaitable, AsyncIterable
+from haskellian import promise as P
 from abc import ABC, abstractmethod
 
 A = TypeVar('A', contravariant=True)
 B = TypeVar('B', contravariant=True)
 
 class WriteQueue(ABC, Generic[A]):
 
+  async def iterate(self, items: AsyncIterable[tuple[str, A]]):
+    """Push all `items`"""
+    async for key, value in items:
+      await self.push(key, value)
+
   @abstractmethod
   async def push(self, key: str, value: A):
     ...
 
   def pusher(self, key: str) -> Callable[[A], Awaitable[None]]:
     """Partially applied `push`"""
     return lambda value: self.push(key, value)
   
   def premap(self, f: Callable[[B], A]) -> 'WriteQueue[B]':
-    return PremappedQueue(self, lambda kv: of((kv[0], f(kv[1]))))
+    return PremappedQueue(self, lambda kv: P.of((kv[0], f(kv[1]))))
   
   def premap_kv(self, f: Callable[[str, B], A]) -> 'WriteQueue[B]':
     """Map but `f` receives both key and value"""
-    return PremappedQueue(self, lambda kv: of((kv[0], f(*kv))))
+    return PremappedQueue(self, lambda kv: P.of((kv[0], f(*kv))))
   
   def premap_k(self, f: Callable[[str], A]) -> 'WriteQueue':
     """Map but `f` receives the key"""
-    return PremappedQueue(self, lambda kv: of((kv[0], f(kv[0]))))
+    return PremappedQueue(self, lambda kv: P.of((kv[0], f(kv[0]))))
   
   def premap_kvt(self, f: Callable[[tuple[str, B]], A]) -> 'WriteQueue[B]':
     """Map but `f` receives both key and value as a tuple"""
-    return PremappedQueue(self, lambda kv: of((kv[0], f(kv))))
+    return PremappedQueue(self, lambda kv: P.of((kv[0], f(kv))))
   
   def apremap(self, f: Callable[[B], Awaitable[A]]) -> 'WriteQueue[B]':
     """Map but `f` is asynchronous"""
     async def mapper(kv: tuple[str, B]):
       return kv[0], await f(kv[1])
     return PremappedQueue(self, mapper)
```

### Comparing `queue_api-0.1.1/src/q/api/extensions/appendable.py` & `queue_api-0.1.2/src/q/api/api/append.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Generic, TypeVar, overload, Literal
 from abc import abstractmethod
-from ..api import WriteQueue, Queue
+from . import WriteQueue, Queue
 
 T = TypeVar('T')
 
 class AppendQueue(WriteQueue[list[T]], Generic[T]):
   @overload
   @abstractmethod
   async def append(self, id: str, values: list[T], *, create: Literal[False]) -> bool:
```

### Comparing `queue_api-0.1.1/src/q/api/extensions/ops/bounding.py` & `queue_api-0.1.2/src/q/api/ops/append_bounding.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TypeVar, Generic
 import asyncio
-import haskellian.asyn.promises as P
-from ..appendable import AppendableQueue
-from ...ops.bounding import Bounded
+from haskellian import ManagedPromise
+from ..api.append import AppendableQueue
+from .bounding import Bounded
 
 T = TypeVar('T')
 
 class AppendBounded(AppendableQueue[T], Bounded[list[T]], Generic[T]):
   def __init__(self, queue: AppendableQueue[T], max_items: int):
     super().__init__(queue, max_items)
     self._queue = queue
@@ -17,15 +17,15 @@
     await self._queue.append(k, vs, create=create)
 
   async def append(self, id: str, values: list[T], *, create = True):
     if create:
       await self._append_buffer.put((id, values, create))
       while self.num_items >= self.max_items:
         if self._promise.resolved:
-          self._promise = P.ManagedAwaitable()
+          self._promise = ManagedPromise()
       self.num_items += 1
       await self._append_advance()
     else:
       return await self._queue.append(id, values, create=False)
     
-def bounded(queue: AppendableQueue[T], max_items: int) -> AppendableQueue[T]:
+def abounded(queue: AppendableQueue[T], max_items: int) -> AppendableQueue[T]:
   return AppendBounded(queue, max_items)
```

### Comparing `queue_api-0.1.1/src/q/api/impl/simple.py` & `queue_api-0.1.2/src/q/api/impl/simple.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from typing import Generic, TypeVar, AsyncIterable
 from collections import OrderedDict
 from ..api import ReadQueue, WriteQueue
-from haskellian.asyn.promises import ManagedAwaitable
+from haskellian import ManagedPromise
 
 A = TypeVar('A')
 B = TypeVar('B')
 
 class SimpleQueue(WriteQueue[A], ReadQueue[A], Generic[A]):
   """Dead simple in-memory implementation backed by an `OrderedDict`"""
 
   def __init__(self):
     self.xs: OrderedDict[str, A] = OrderedDict()
-    self._next = ManagedAwaitable()
+    self._next = ManagedPromise()
 
   def __len__(self):
     return len(self.xs) # type: ignore
 
   async def _read(self, id: str | None = None, remove: bool = False) -> None | tuple[str, A]:
     if id is None:
       if len(self.xs) == 0:
         await self._next
-        self._next = ManagedAwaitable()
+        self._next = ManagedPromise()
         return await self._read(id, remove)
       elif remove:
         return self.xs.popitem()
       else:
         return next(iter(self.xs.items()))
     elif id in self.xs:
       v = self.xs.pop(id) if remove else self.xs[id]
```

### Comparing `queue_api-0.1.1/src/q/api/ops/bounding.py` & `queue_api-0.1.2/src/q/api/ops/bounding.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from typing import TypeVar, Generic
 import asyncio
-import haskellian.asyn.promises as P
+from haskellian import ManagedPromise
 from ..api import Queue
 
 T = TypeVar('T')
 Q = TypeVar('Q', bound=Queue)
 
 class Bounded(Queue[T], Generic[T]):
   
   def __init__(self, queue: Queue[T], max_items: int):
     self._queue = queue
     self.num_items = 0
     self.max_items = max_items
     self._buffer = asyncio.Queue[tuple[str, T]]()
-    self._promise = P.ManagedAwaitable()
+    self._promise = ManagedPromise()
 
   async def _advance(self):
     k, v = await self._buffer.get()
     await self._queue.push(k, v)
 
   async def push(self, key: str, value: T):
     await self._buffer.put((key, value))
     while self.num_items >= self.max_items:
       if self._promise.resolved:
-        self._promise = P.ManagedAwaitable()
+        self._promise = ManagedPromise()
       await self._promise
     self.num_items += 1
     await self._advance()
   
   def _read(self, id: str | None, remove: bool):
     if remove:
       self.num_items -= 1
```

### Comparing `queue_api-0.1.1/src/q/api/ops/interleaving.py` & `queue_api-0.1.2/src/q/api/ops/interleaving.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import TypeVar, Generic, AsyncIterable
 import asyncio
-from haskellian.asyn.iter import ManagedIterable
+from haskellian import ManagedAsync
 from ..api import ReadQueue
 from ..impl import SimpleQueue
 
 A = TypeVar('A')
 B = TypeVar('B')
 C = TypeVar('C')
 
@@ -27,15 +27,15 @@
     else:
       for q in self._queues:
         x = await q._read(id, remove)
         if x is not None:
           return x
   
   def _items(self) -> AsyncIterable[tuple[str, A]]:
-    out = ManagedIterable[tuple[str, A]]()
+    out = ManagedAsync[tuple[str, A]]()
     async def iterate(xs: AsyncIterable[tuple[str, A]]):
       async for x in xs:
         out.push(x)
 
     async def iterate_all():
       async for x in self._buffer.items():
         out.push(x)
```

### Comparing `queue_api-0.1.1/src/q/api/ops/merging.py` & `queue_api-0.1.2/src/q/api/ops/merging.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import TypeVar, Generic, AsyncIterable, Callable, Awaitable
 import asyncio
-import haskellian.asyn.promises as P
+import haskellian.promise as P
 from q.api import ReadQueue
 
 A = TypeVar('A')
 B = TypeVar('B')
 C = TypeVar('C')
```

### Comparing `queue_api-0.1.1/src/q/api/ops/splitting.py` & `queue_api-0.1.2/src/q/api/ops/splitting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import TypeVar, Generic, AsyncIterable, Callable, Awaitable
-import haskellian.asyn.promises as P
+import haskellian.promise as P
 from ..api import ReadQueue, WriteQueue
 from ..impl import SimpleQueue
 from .interleaving import interleave
 
 A = TypeVar('A')
 B = TypeVar('B')
 C = TypeVar('C')
```

### Comparing `queue_api-0.1.1/src/queue_api.egg-info/SOURCES.txt` & `queue_api-0.1.2/src/queue_api.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 README.md
 pyproject.toml
 src/q/api/__init__.py
+src/q/api/__init__.pyi
 src/q/api/api/__init__.py
-src/q/api/api/connect_.py
+src/q/api/api/append.py
 src/q/api/api/queue.py
 src/q/api/api/read.py
 src/q/api/api/write.py
-src/q/api/extensions/__init__.py
-src/q/api/extensions/appendable.py
-src/q/api/extensions/ops/__init__.py
-src/q/api/extensions/ops/bounding.py
 src/q/api/impl/__init__.py
 src/q/api/impl/empty.py
 src/q/api/impl/simple.py
 src/q/api/ops/__init__.py
+src/q/api/ops/__init__.pyi
+src/q/api/ops/append_bounding.py
 src/q/api/ops/bounding.py
 src/q/api/ops/interleaving.py
 src/q/api/ops/merging.py
 src/q/api/ops/splitting.py
 src/queue_api.egg-info/PKG-INFO
 src/queue_api.egg-info/SOURCES.txt
 src/queue_api.egg-info/dependency_links.txt
+src/queue_api.egg-info/requires.txt
 src/queue_api.egg-info/top_level.txt
```


# Comparing `tmp/rate_control-2.0.0.tar.gz` & `tmp/rate_control-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rate_control-2.0.0.tar", max compression
+gzip compressed data, was "rate_control-3.0.0.tar", max compression
```

## Comparing `rate_control-2.0.0.tar` & `rate_control-3.0.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0     1101 2024-04-16 18:30:46.785962 rate_control-2.0.0/LICENSE
--rw-r--r--   0        0        0     3822 2024-04-16 18:30:46.785962 rate_control-2.0.0/README.rst
--rw-r--r--   0        0        0     2872 2024-04-16 18:31:01.737882 rate_control-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      622 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/__init__.py
--rw-r--r--   0        0        0     3718 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_bucket_group.py
--rw-r--r--   0        0        0      330 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/__init__.py
--rw-r--r--   0        0        0      344 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_base/__init__.py
--rw-r--r--   0        0        0     1942 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_base/_abc.py
--rw-r--r--   0        0        0     2479 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_base/_base_rate.py
--rw-r--r--   0        0        0      805 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_base/_capacity_updating.py
--rw-r--r--   0        0        0      906 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_base/_token_based.py
--rw-r--r--   0        0        0      977 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_base/_windowed.py
--rw-r--r--   0        0        0     1034 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_fixed_window_counter.py
--rw-r--r--   0        0        0     1372 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_leaky_bucket.py
--rw-r--r--   0        0        0      659 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_sliding_window_log.py
--rw-r--r--   0        0        0      653 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_buckets/_unlimited.py
--rw-r--r--   0        0        0      179 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_controllers/__init__.py
--rw-r--r--   0        0        0     4657 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_controllers/_abc.py
--rw-r--r--   0        0        0     1046 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_controllers/_rate_limiter.py
--rw-r--r--   0        0        0     8709 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_controllers/_scheduler.py
--rw-r--r--   0        0        0      111 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_enums/__init__.py
--rw-r--r--   0        0        0      262 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_enums/_duration.py
--rw-r--r--   0        0        0      350 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_enums/_priority.py
--rw-r--r--   0        0        0      297 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_errors.py
--rw-r--r--   0        0        0      105 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_helpers/__init__.py
--rw-r--r--   0        0        0      781 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_helpers/_mk_repr.py
--rw-r--r--   0        0        0      472 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_helpers/_protocols.py
--rw-r--r--   0        0        0     1502 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_helpers/_request.py
--rw-r--r--   0        0        0     2162 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/_helpers/_validation.py
--rw-r--r--   0        0        0        0 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/py.typed
--rw-r--r--   0        0        0      202 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/queues/__init__.py
--rw-r--r--   0        0        0     1540 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/queues/_abc.py
--rw-r--r--   0        0        0     1336 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/queues/_fifo.py
--rw-r--r--   0        0        0     1311 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/queues/_lifo.py
--rw-r--r--   0        0        0     1658 2024-04-16 18:30:46.789962 rate_control-2.0.0/rate_control/queues/_priority.py
--rw-r--r--   0        0        0     5042 1970-01-01 00:00:00.000000 rate_control-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-21 05:06:56.403097 rate_control-3.0.0/LICENSE
+-rw-r--r--   0        0        0     3822 2024-04-21 05:06:56.403097 rate_control-3.0.0/README.rst
+-rw-r--r--   0        0        0     2872 2024-04-21 05:07:01.275188 rate_control-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      582 2024-04-21 05:06:56.403097 rate_control-3.0.0/rate_control/__init__.py
+-rw-r--r--   0        0        0     3673 2024-04-21 05:06:56.403097 rate_control-3.0.0/rate_control/_bucket_group.py
+-rw-r--r--   0        0        0      267 2024-04-21 05:06:56.403097 rate_control-3.0.0/rate_control/_buckets/__init__.py
+-rw-r--r--   0        0        0      344 2024-04-21 05:06:56.403097 rate_control-3.0.0/rate_control/_buckets/_base/__init__.py
+-rw-r--r--   0        0        0     2005 2024-04-21 05:06:56.403097 rate_control-3.0.0/rate_control/_buckets/_base/_abc.py
+-rw-r--r--   0        0        0     2479 2024-04-21 05:06:56.403097 rate_control-3.0.0/rate_control/_buckets/_base/_base_rate.py
+-rw-r--r--   0        0        0      805 2024-04-21 05:06:56.403097 rate_control-3.0.0/rate_control/_buckets/_base/_capacity_updating.py
+-rw-r--r--   0        0        0      906 2024-04-21 05:06:56.403097 rate_control-3.0.0/rate_control/_buckets/_base/_token_based.py
+-rw-r--r--   0        0        0      977 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_buckets/_base/_windowed.py
+-rw-r--r--   0        0        0     1034 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_buckets/_fixed_window_counter.py
+-rw-r--r--   0        0        0     1372 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_buckets/_leaky_bucket.py
+-rw-r--r--   0        0        0      659 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_buckets/_sliding_window_log.py
+-rw-r--r--   0        0        0      179 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_controllers/__init__.py
+-rw-r--r--   0        0        0     4972 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_controllers/_abc.py
+-rw-r--r--   0        0        0     1088 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_controllers/_rate_limiter.py
+-rw-r--r--   0        0        0     8773 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_controllers/_scheduler.py
+-rw-r--r--   0        0        0      111 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_enums/__init__.py
+-rw-r--r--   0        0        0      262 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_enums/_duration.py
+-rw-r--r--   0        0        0      350 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_enums/_priority.py
+-rw-r--r--   0        0        0      297 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_errors.py
+-rw-r--r--   0        0        0      105 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_helpers/__init__.py
+-rw-r--r--   0        0        0      781 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_helpers/_mk_repr.py
+-rw-r--r--   0        0        0      472 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_helpers/_protocols.py
+-rw-r--r--   0        0        0     1502 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_helpers/_request.py
+-rw-r--r--   0        0        0     1709 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/_helpers/_validation.py
+-rw-r--r--   0        0        0        0 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/py.typed
+-rw-r--r--   0        0        0      202 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/queues/__init__.py
+-rw-r--r--   0        0        0     1540 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/queues/_abc.py
+-rw-r--r--   0        0        0     1336 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/queues/_fifo.py
+-rw-r--r--   0        0        0     1311 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/queues/_lifo.py
+-rw-r--r--   0        0        0     1658 2024-04-21 05:06:56.407097 rate_control-3.0.0/rate_control/queues/_priority.py
+-rw-r--r--   0        0        0     5042 1970-01-01 00:00:00.000000 rate_control-3.0.0/PKG-INFO
```

### Comparing `rate_control-2.0.0/LICENSE` & `rate_control-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rate_control-2.0.0/README.rst` & `rate_control-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `rate_control-2.0.0/pyproject.toml` & `rate_control-3.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rate-control"
-version = "2.0.0"
+version = "3.0.0"
 description = "Versatile rate controlling in Python"
 authors = ["Corentin Régent <corentin.regent.pro@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/corentin-regent/rate-control"
 repository = "https://github.com/corentin-regent/rate-control"
 documentation = "https://rate-control.readthedocs.io/"
@@ -46,15 +46,15 @@
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 anyio = {version = "*", extras = ["trio"]}
 mypy = "^1.6"
-ruff = "^0.3.0"
+ruff = "^0.4.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 aiofastforward = "^0.0.26"
 anyio = {version = "*", extras = ["trio"]}
```

### Comparing `rate_control-2.0.0/rate_control/__init__.py` & `rate_control-3.0.0/rate_control/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     'Priority',
     'RateController',
     'RateLimit',
     'RateLimiter',
     'ReachedMaxPending',
     'Scheduler',
     'SlidingWindowLog',
-    'UnlimitedBucket',
 ]
 
 from rate_control._bucket_group import BucketGroup
-from rate_control._buckets import Bucket, FixedWindowCounter, LeakyBucket, SlidingWindowLog, UnlimitedBucket
+from rate_control._buckets import Bucket, FixedWindowCounter, LeakyBucket, SlidingWindowLog
 from rate_control._controllers import RateController, RateLimiter, Scheduler
 from rate_control._enums import Duration, Priority
 from rate_control._errors import RateLimit, ReachedMaxPending
```

### Comparing `rate_control-2.0.0/rate_control/_bucket_group.py` & `rate_control-3.0.0/rate_control/_bucket_group.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from contextlib import AsyncExitStack, suppress
 from typing import Any, Iterator
 
 from anyio import WouldBlock, create_memory_object_stream, create_task_group
 
 from rate_control._buckets import Bucket
 from rate_control._helpers import mk_repr
-from rate_control._helpers._validation import validate_buckets
 
 if sys.version_info >= (3, 9):
     from collections.abc import Iterable
 else:
     from typing import Iterable
 
 if sys.version_info >= (3, 11):
@@ -36,15 +35,14 @@
         Args:
             buckets: The buckets to aggregate within this bucket group.
             should_enter_context: Whether entering the context of the bucket group
                 should also enter the context of the underlying buckets.
                 Defaults to `True`.
         """
         super().__init__(**kwargs)
-        validate_buckets(buckets)
         self._buckets = buckets
         self._should_enter_context = should_enter_context
         self._send_stream, self._recv_stream = create_memory_object_stream[Bucket]()
 
     @override
     def __repr__(self) -> str:
         return mk_repr(self, *self._buckets, should_enter_context=self._should_enter_context)
@@ -85,15 +83,16 @@
             while True:
                 refilled_bucket = self._recv_stream.receive_nowait()
                 self._listen_for_refill(refilled_bucket)
         await self._recv_stream.receive()
 
     @override
     def can_acquire(self, tokens: float) -> bool:
-        """
+        """Whether the given amount of tokens can be acquired.
+
         Args:
             tokens: The amount of tokens that we want to acquire.
 
         Returns:
             Whether all the underlying buckets can acquire the given amount of tokens.
         """
         return all(bucket.can_acquire(tokens) for bucket in self._buckets)
```

### Comparing `rate_control-2.0.0/rate_control/_buckets/_base/_abc.py` & `rate_control-3.0.0/rate_control/_buckets/_base/_abc.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,20 +42,21 @@
 
     @abstractmethod
     async def wait_for_refill(self) -> None:
         """Wait until some tokens are replenished."""
 
     @abstractmethod
     def can_acquire(self, tokens: float) -> bool:
-        """
+        """Whether the given amount of tokens can be acquired.
+
         Args:
             tokens: The amount of tokens that we want to acquire.
 
         Returns:
-            Whether the given amount of tokens is available.
+            Whether the given amount of tokens is available to consume.
         """
 
     @abstractmethod
     def acquire(self, tokens: float) -> None:
         """Acquire the given amount of tokens.
 
         Args:
```

### Comparing `rate_control-2.0.0/rate_control/_buckets/_base/_base_rate.py` & `rate_control-3.0.0/rate_control/_buckets/_base/_base_rate.py`

 * *Files identical despite different names*

### Comparing `rate_control-2.0.0/rate_control/_buckets/_base/_capacity_updating.py` & `rate_control-3.0.0/rate_control/_buckets/_base/_capacity_updating.py`

 * *Files identical despite different names*

### Comparing `rate_control-2.0.0/rate_control/_buckets/_base/_token_based.py` & `rate_control-3.0.0/rate_control/_buckets/_base/_token_based.py`

 * *Files identical despite different names*

### Comparing `rate_control-2.0.0/rate_control/_buckets/_base/_windowed.py` & `rate_control-3.0.0/rate_control/_buckets/_base/_windowed.py`

 * *Files identical despite different names*

### Comparing `rate_control-2.0.0/rate_control/_buckets/_fixed_window_counter.py` & `rate_control-3.0.0/rate_control/_buckets/_fixed_window_counter.py`

 * *Files identical despite different names*

### Comparing `rate_control-2.0.0/rate_control/_buckets/_leaky_bucket.py` & `rate_control-3.0.0/rate_control/_buckets/_leaky_bucket.py`

 * *Files identical despite different names*

### Comparing `rate_control-2.0.0/rate_control/_buckets/_sliding_window_log.py` & `rate_control-3.0.0/rate_control/_buckets/_sliding_window_log.py`

 * *Files identical despite different names*

### Comparing `rate_control-2.0.0/rate_control/_controllers/_abc.py` & `rate_control-3.0.0/rate_control/_controllers/_abc.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from contextlib import asynccontextmanager, contextmanager
 from typing import Any, Optional
 
 from rate_control._bucket_group import BucketGroup
 from rate_control._buckets import Bucket
 from rate_control._errors import RateLimit
 from rate_control._helpers import mk_repr
-from rate_control._helpers._validation import validate_buckets, validate_max_concurrency
+from rate_control._helpers._validation import validate_max_concurrency
 
 if sys.version_info >= (3, 9):
     from collections.abc import AsyncIterator, Iterator
 else:
     from typing import AsyncIterator, Iterator
 
 if sys.version_info >= (3, 11):
@@ -37,67 +37,77 @@
         *buckets: Bucket,
         should_enter_context: bool = True,
         max_concurrency: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         """
         Args:
-            bucket: The buckets that will be managed by the rate controller.
+            buckets: The buckets that will be managed by the rate controller, optional.
             should_enter_context: Whether entering the context of the rate controller
-                should also enter the context of the underlying buckets.
+                should also enter the context of the underlying buckets, if any.
                 Defaults to True.
             max_concurrency: The maximum amount of concurrent requests allowed.
                 Defaults to `None` (no limit).
         """
         super().__init__(**kwargs)
-        validate_buckets(buckets)
         validate_max_concurrency(max_concurrency)
         self._bucket = (
-            buckets[0] if len(buckets) == 1 else BucketGroup(*buckets, should_enter_context=should_enter_context)
+            None
+            if not buckets
+            else buckets[0]
+            if len(buckets) == 1
+            else BucketGroup(*buckets, should_enter_context=should_enter_context)
         )
         self._should_enter_context = should_enter_context
         self._max_concurrency = max_concurrency
         self._concurrent_requests = 0
 
     async def __aenter__(self) -> Self:
         """Enter the controller's context.
 
         Also enters the context of the underlying buckets,
         if the `should_enter_context` flag was set to `True`.
         """
-        if self._should_enter_context:
+        if self._should_enter_context and self._bucket is not None:
             await self._bucket.__aenter__()
         return self
 
     async def __aexit__(self, *exc_info: Any) -> Optional[bool]:
         """Exit the controller's context.
 
         Also exits the context of the underlying buckets,
         if the `should_enter_context` flag was set to `True`.
         """
-        if self._should_enter_context:
+        if self._should_enter_context and self._bucket is not None:
             await self._bucket.__aexit__(*exc_info)
         return False
 
     @override
     def __repr__(self) -> str:
-        return mk_repr(
-            self, self._bucket, should_enter_context=self._should_enter_context, max_concurrency=self._max_concurrency
+        return (
+            mk_repr(
+                self,
+                self._bucket,
+                should_enter_context=self._should_enter_context,
+                max_concurrency=self._max_concurrency,
+            )
+            if self._bucket is not None
+            else mk_repr(self, max_concurrency=self._max_concurrency)
         )
 
     def can_acquire(self, tokens: float = 1) -> bool:
         """
         Args:
             tokens: The amount of tokens to acquire for the request.
                 Defaults to `1`.
 
         Returns:
             Whether a request for the given amount of tokens can be processed instantly.
         """
-        return not self._is_concurrency_limited and self._bucket.can_acquire(tokens)
+        return not self._is_concurrency_limited and (self._bucket is None or self._bucket.can_acquire(tokens))
 
     @asynccontextmanager
     @abstractmethod
     async def request(self, tokens: float = 1) -> AsyncIterator[None]:
         """Asynchronous context manager that requests the given amount of tokens before the execution.
 
         Args:
```

### Comparing `rate_control-2.0.0/rate_control/_controllers/_rate_limiter.py` & `rate_control-3.0.0/rate_control/_controllers/_rate_limiter.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     @override
     async def request(self, tokens: float = 1) -> AsyncIterator[None]:
         """Context manager that acquires the given amount of tokens while holding concurrency.
 
         Args:
             tokens: The number of tokens to acquire.
                 Defaults to `1`.
+
         Raises:
             RateLimit: The request cannot be fulfilled instantly.
         """
         self._assert_can_acquire(tokens)
-        self._bucket.acquire(tokens)
+        if self._bucket is not None:
+            self._bucket.acquire(tokens)
         with self._hold_concurrency():
             yield
```

### Comparing `rate_control-2.0.0/rate_control/_controllers/_scheduler.py` & `rate_control-3.0.0/rate_control/_controllers/_scheduler.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,17 +43,17 @@
         max_concurrency: Optional[int] = None,
         max_pending: Optional[int] = None,
         queue_factory: Callable[[], Queue[Request]] = PriorityQueue,
         **kwargs: Any,
     ) -> None:
         """
         Args:
-            buckets: The buckets that will be managed by the rate controller.
+            buckets: The buckets that will be managed by the rate controller, optional.
             should_enter_context: Whether entering the context of the rate controller
-                should also enter the context of the underlying buckets.
+                should also enter the context of the underlying buckets, if any.
                 Defaults to True.
             max_concurrency: The maximum amount of concurrent requests allowed.
                 Defaults to `None` (no limit).
             max_pending: The maximum amount of requests waiting to be processed.
                 Defaults to `None` (no limit).
             queue_factory: The factory for initializing the request queues.
                 Defaults to :class:`.PriorityQueue`: requests are processed by ascending weight.
@@ -65,38 +65,44 @@
         self._queues = [queue_factory() for _ in Priority]
         self._is_processing_requests = False
 
     @override
     async def __aenter__(self) -> Self:
         await super().__aenter__()
         self._task_group = await create_task_group().__aenter__()
-        self._task_group.start_soon(self._listen_to_refills)
+        if self._bucket is not None:
+            self._task_group.start_soon(self._listen_to_refills)
         return self
 
     async def _listen_to_refills(self) -> NoReturn:
         """Process queued requests every time new tokens are available."""
+        assert self._bucket is not None
         while True:
             await self._bucket.wait_for_refill()
             await self._process_queued_requests()
             await checkpoint()
 
     @override
     async def __aexit__(self, *exc_info: Any) -> Optional[bool]:
         self._task_group.cancel_scope.cancel()
         await self._task_group.__aexit__(*exc_info)
         return await super().__aexit__(*exc_info)
 
     @override
     def __repr__(self) -> str:
-        return mk_repr(
-            self,
-            self._bucket,
-            should_enter_context=self._should_enter_context,
-            max_concurrency=self._max_concurrency,
-            max_pending=self._max_pending,
+        return (
+            mk_repr(
+                self,
+                self._bucket,
+                should_enter_context=self._should_enter_context,
+                max_concurrency=self._max_concurrency,
+                max_pending=self._max_pending,
+            )
+            if self._bucket is not None
+            else mk_repr(self, max_concurrency=self._max_concurrency, max_pending=self._max_pending)
         )
 
     @asynccontextmanager
     @override
     async def request(
         self,
         tokens: float = 1,
@@ -125,60 +131,61 @@
         """
         if not hasattr(self, '_task_group'):
             raise RuntimeError(f"Make sure to enter the scheduler's context using 'async with {self}'")
         if not self.can_acquire(tokens):
             if fill_or_kill:
                 raise RateLimit(f'Cannot process the request for {tokens} tokens.')
             else:
-                await self._perform_request(tokens, priority)
-        self._bucket.acquire(tokens)
+                await self._schedule_request(tokens, priority)
+        if self._bucket is not None:
+            self._bucket.acquire(tokens)
         with self._hold_concurrency():
             yield
 
     @override
     def _on_concurrency_release(self) -> None:
-        if self._max_concurrency is not None and self._concurrent_requests == self._max_concurrency - 1:
+        if self._max_concurrency is not None and self._concurrent_requests < self._max_concurrency:
             self._task_group.start_soon(self._process_queued_requests)
 
     async def _process_queued_requests(self) -> None:
         """Pop and start queued requests while it is possible."""
-        if self._is_processing_requests:
-            return
-        with self._hold_request_processing():
-            await self._process_queues()
-
-    async def _process_queues(self) -> None:
-        while True:
-            try:
-                queue = next(filter(lambda queue: self.can_acquire(queue.head().cost), filter(None, self._queues)))
-            except StopIteration:
-                break
-            else:
-                await self._process_next_request(queue)
+        if not self._is_processing_requests:
+            with self._hold_request_processing():
+                await self._process_queues()
 
     @contextmanager
     def _hold_request_processing(self) -> Iterator[None]:
         self._is_processing_requests = True
         try:
             yield
         finally:
             self._is_processing_requests = False
 
+    async def _process_queues(self) -> None:
+        while True:
+            try:
+                queue = next(queue for queue in filter(None, self._queues) if self.can_acquire(queue.head().cost))
+            except StopIteration:
+                break
+            else:
+                await self._process_next_request(queue)
+
     async def _process_next_request(self, queue: Queue[Request]) -> None:
         """Fire the next request from the queue and wait until the underlying tokens are acquired.
 
         Tokens are not acquired directly in this method,
         in order to support request cancellation.
         """
-        request = self._pop(queue)
+        request = queue.pop()
+        self._pending_requests -= 1
         request.fire()
         await request.wait_for_ack()
 
-    async def _perform_request(self, tokens: float, priority: Priority) -> None:
-        """Perform a request to acquire the given amount of tokens, with the given priority.
+    async def _schedule_request(self, tokens: float, priority: Priority) -> None:
+        """Schedule an internal request to acquire the given amount of tokens, with the given priority.
 
         Args:
             tokens: The amount of tokens to acquire.
             priority: The request priority.
 
         Raises:
             ReachedMaxPending: The limit of pending requests was reached.
@@ -199,37 +206,28 @@
         Args:
             request: The request to schedule.
             priority: The priority of the request.
 
         Raises:
             ReachedMaxPending: The limit of pending requests was reached.
         """
-        self._check_pending_limit()
+        if self._is_pending_limited:
+            raise ReachedMaxPending
         queue = self._queues[priority]
         queue.add(request)
         self._pending_requests += 1
 
+    @property
+    def _is_pending_limited(self) -> bool:
+        return self._max_pending is not None and self._pending_requests >= self._max_pending
+
     def _discard(self, request: Request, priority: Priority) -> None:
         """Remove the given request from the queue, if it exists.
 
         Args:
             request: The request to unschedule.
             priority: The priority with which the request was originally scheduled.
         """
         queue = self._queues[priority]
         with suppress(ValueError):
             queue.remove(request)
             self._pending_requests -= 1
-
-    def _pop(self, queue: Queue[Request]) -> Request:
-        request = queue.pop()
-        self._pending_requests -= 1
-        return request
-
-    def _check_pending_limit(self) -> None:
-        """Make sure that a new pending request can be scheduled.
-
-        Raises:
-            ReachedMaxPending: The limit of pending requests was reached.
-        """
-        if self._max_pending is not None and self._max_pending <= self._pending_requests:
-            raise ReachedMaxPending
```

### Comparing `rate_control-2.0.0/rate_control/_helpers/_mk_repr.py` & `rate_control-3.0.0/rate_control/_helpers/_mk_repr.py`

 * *Files identical despite different names*

### Comparing `rate_control-2.0.0/rate_control/_helpers/_request.py` & `rate_control-3.0.0/rate_control/_helpers/_request.py`

 * *Files identical despite different names*

### Comparing `rate_control-2.0.0/rate_control/_helpers/_validation.py` & `rate_control-3.0.0/rate_control/_helpers/_validation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,18 @@
 from __future__ import annotations
 
 __all__ = [
-    'validate_buckets',
     'validate_capacity',
     'validate_delay',
     'validate_max_concurrency',
     'validate_max_pending',
     'validate_tokens',
 ]
 
-import sys
-from typing import TYPE_CHECKING, Optional
-
-if sys.version_info >= (3, 9):
-    from collections.abc import Collection
-else:
-    from typing import Collection
-
-if TYPE_CHECKING:
-    from rate_control._buckets import Bucket
-
-
-def validate_buckets(buckets: Collection[Bucket]) -> None:
-    """
-    Raises:
-        ValueError: No bucket was provided.
-    """
-    if not buckets:
-        raise ValueError('At least one token bucket must be provided')
+from typing import Optional
 
 
 def validate_capacity(capacity: float) -> None:
     """
     Raises:
         ValueError: Negative or zero capacity was provided.
     """
```

### Comparing `rate_control-2.0.0/rate_control/queues/_abc.py` & `rate_control-3.0.0/rate_control/queues/_abc.py`

 * *Files identical despite different names*

### Comparing `rate_control-2.0.0/rate_control/queues/_fifo.py` & `rate_control-3.0.0/rate_control/queues/_fifo.py`

 * *Files identical despite different names*

### Comparing `rate_control-2.0.0/rate_control/queues/_lifo.py` & `rate_control-3.0.0/rate_control/queues/_lifo.py`

 * *Files identical despite different names*

### Comparing `rate_control-2.0.0/rate_control/queues/_priority.py` & `rate_control-3.0.0/rate_control/queues/_priority.py`

 * *Files identical despite different names*

### Comparing `rate_control-2.0.0/PKG-INFO` & `rate_control-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rate-control
-Version: 2.0.0
+Version: 3.0.0
 Summary: Versatile rate controlling in Python
 Home-page: https://github.com/corentin-regent/rate-control
 License: MIT
 Keywords: async,rate limit,schedule,throttle,token bucket
 Author: Corentin Régent
 Author-email: corentin.regent.pro@gmail.com
 Requires-Python: >=3.8,<4.0
```


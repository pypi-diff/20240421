# Comparing `tmp/thread-1.1.1.tar.gz` & `tmp/thread-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thread-1.1.1.tar", max compression
+gzip compressed data, was "thread-2.0.0.tar", max compression
```

## Comparing `thread-1.1.1.tar` & `thread-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1496 2024-03-17 15:06:21.514939 thread-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0     5327 2024-03-17 15:06:21.514939 thread-1.1.1/README.md
--rw-r--r--   0        0        0     1625 2024-03-17 15:06:21.514939 thread-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      654 2024-03-17 15:06:21.514939 thread-1.1.1/src/thread/__init__.py
--rw-r--r--   0        0        0      139 2024-03-17 15:06:21.514939 thread-1.1.1/src/thread/__main__.py
--rw-r--r--   0        0        0     1522 2024-03-17 15:06:21.514939 thread-1.1.1/src/thread/_types.py
--rw-r--r--   0        0        0      272 2024-03-17 15:06:21.514939 thread-1.1.1/src/thread/cli.py
--rw-r--r--   0        0        0       93 2024-03-17 15:06:21.514939 thread-1.1.1/src/thread/decorators/__init__.py
--rw-r--r--   0        0        0     4824 2024-03-17 15:06:21.514939 thread-1.1.1/src/thread/decorators/_processor.py
--rw-r--r--   0        0        0     3877 2024-03-17 15:06:21.514939 thread-1.1.1/src/thread/decorators/_threaded.py
--rw-r--r--   0        0        0     2196 2024-03-17 15:06:21.514939 thread-1.1.1/src/thread/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-17 15:06:21.514939 thread-1.1.1/src/thread/py.typed
--rw-r--r--   0        0        0    22228 2024-03-17 15:06:21.514939 thread-1.1.1/src/thread/thread.py
--rw-r--r--   0        0        0      123 2024-03-17 15:06:21.514939 thread-1.1.1/src/thread/utils/__init__.py
--rw-r--r--   0        0        0     1381 2024-03-17 15:06:21.514939 thread-1.1.1/src/thread/utils/algorithm.py
--rw-r--r--   0        0        0     4527 2024-03-17 15:06:21.514939 thread-1.1.1/src/thread/utils/config.py
--rw-r--r--   0        0        0       50 2024-03-17 15:06:21.514939 thread-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0       65 2024-03-17 15:06:21.514939 thread-1.1.1/tests/conftest.py
--rw-r--r--   0        0        0     1144 2024-03-17 15:06:21.514939 thread-1.1.1/tests/test_algorithm.py
--rw-r--r--   0        0        0     9362 2024-03-17 15:06:21.514939 thread-1.1.1/tests/test_dataframe_compatibility.py
--rw-r--r--   0        0        0     2118 2024-03-17 15:06:21.514939 thread-1.1.1/tests/test_decorator.py
--rw-r--r--   0        0        0     1810 2024-03-17 15:06:21.514939 thread-1.1.1/tests/test_parallelprocessing.py
--rw-r--r--   0        0        0     3386 2024-03-17 15:06:21.514939 thread-1.1.1/tests/test_thread.py
--rw-r--r--   0        0        0     1484 2024-03-17 15:06:21.514939 thread-1.1.1/tests/test_verbosity.py
--rw-r--r--   0        0        0     6713 1970-01-01 00:00:00.000000 thread-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1496 2024-04-21 04:10:29.955723 thread-2.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     5329 2024-04-21 04:10:29.955723 thread-2.0.0/README.md
+-rw-r--r--   0        0        0     1625 2024-04-21 04:10:29.955723 thread-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      657 2024-04-21 04:10:29.955723 thread-2.0.0/src/thread/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-21 04:10:29.955723 thread-2.0.0/src/thread/__main__.py
+-rw-r--r--   0        0        0     1522 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/_types.py
+-rw-r--r--   0        0        0      272 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/cli.py
+-rw-r--r--   0        0        0       93 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/decorators/__init__.py
+-rw-r--r--   0        0        0     4846 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/decorators/_processor.py
+-rw-r--r--   0        0        0     3889 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/decorators/_threaded.py
+-rw-r--r--   0        0        0     2196 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/py.typed
+-rw-r--r--   0        0        0    22008 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/thread.py
+-rw-r--r--   0        0        0      123 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/utils/__init__.py
+-rw-r--r--   0        0        0     1381 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/utils/algorithm.py
+-rw-r--r--   0        0        0     4527 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/utils/config.py
+-rw-r--r--   0        0        0       50 2024-04-21 04:10:29.959723 thread-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-21 04:10:29.959723 thread-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     1144 2024-04-21 04:10:29.959723 thread-2.0.0/tests/test_algorithm.py
+-rw-r--r--   0        0        0     1820 2024-04-21 04:10:29.959723 thread-2.0.0/tests/test_concurrentprocessing.py
+-rw-r--r--   0        0        0     9471 2024-04-21 04:10:29.959723 thread-2.0.0/tests/test_dataframe_compatibility.py
+-rw-r--r--   0        0        0     2118 2024-04-21 04:10:29.959723 thread-2.0.0/tests/test_decorator.py
+-rw-r--r--   0        0        0     3409 2024-04-21 04:10:29.959723 thread-2.0.0/tests/test_thread.py
+-rw-r--r--   0        0        0     1484 2024-04-21 04:10:29.959723 thread-2.0.0/tests/test_verbosity.py
+-rw-r--r--   0        0        0     6715 1970-01-01 00:00:00.000000 thread-2.0.0/PKG-INFO
```

### Comparing `thread-1.1.1/LICENSE.txt` & `thread-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thread-1.1.1/README.md` & `thread-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 1. Install the package
    ```sh
    pip install -U thread
    ```
 2. Import thread into your library!
    ```py
    import thread
-   from thread import Thread, ParallelProcessing
+   from thread import Thread, ConcurrentProcessing
    ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- DOCS -->
@@ -94,15 +94,15 @@
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- ROADMAP -->
 ## Roadmap
 
-- [x] v1.1.1 Release
+- [x] v2.0.0 Release
 - [ ] Bug fixes
 - [ ] New features
 - [ ] Testing
 - [ ] Next release...
 
 See the [open issues](https://github.com/python-thread/thread/issues) for a full list of proposed features (and known issues).
```

#### html2text {}

```diff
@@ -19,19 +19,19 @@
 I hope thread will become your threading solution! â¡â¸(Ë¶Ë áµ ËË¶)â¸â¡
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Getting Started This is an example of how you can set up your project
 locally. To get a local copy up and running follow these simple example steps.
 ### Prerequisites * Python 3.9+ ### Installation _Below is an example of how
 you can install and use thread._ 1. Install the package ```sh pip install -
 U thread ``` 2. Import thread into your library! ```py import thread from
-thread import Thread, ParallelProcessing ```
+thread import Thread, ConcurrentProcessing ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Documentation Our docs are [here!](https://thread.ngjx.org)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Roadmap - [x] v1.1.1 Release - [ ] Bug fixes - [ ] New features - [ ]
+## Roadmap - [x] v2.0.0 Release - [ ] Bug fixes - [ ] New features - [ ]
 Testing - [ ] Next release... See the [open issues](https://github.com/python-
 thread/thread/issues) for a full list of proposed features (and known issues).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. ( Ë¶ËáËËµ ) If you have a suggestion that would
 make this better, please fork the repo and create a pull request. You can also
```

### Comparing `thread-1.1.1/pyproject.toml` & `thread-2.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thread"
-version = "1.1.1"
+version = "2.0.0"
 description = "Threading module extension"
 authors = ["Alex <contact@ngjx.org>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [
   { include = "thread", from = "src" },
   { include = "thread/py.typed", from = "src" },
@@ -26,15 +26,15 @@
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: Implementation :: CPython",
   "Typing :: Typed",
 ]
 
 [tool.poetry.urls]
 Homepage = "https://thread.ngjx.org"
-Documentation = "https://thread.ngjx.org/docs/v1.1.1"
+Documentation = "https://thread.ngjx.org/docs/v2.0.0"
 Source = "https://github.com/python-thread/thread"
 Download = "https://pypi.org/project/thread/#files"
 "Release Notes" = "https://github.com/python-thread/thread/releases"
 "Bug Tracker" = "https://github.com/python-thread/thread/issues"
 
 [tool.poetry.scripts]
 thread = "thread.__main__:app"
```

### Comparing `thread-1.1.1/src/thread/__init__.py` & `thread-2.0.0/src/thread/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """
 ## Thread Library
-Documentation at https://thread.ngjx.org/docs/v1.1.1
+Documentation at https://thread.ngjx.org/docs/2.0.0
 
 
 ---
 
-Released under the GPG-3 License
+Released under the BSD-3 License
 
 Copyright (c) thread.ngjx.org, All rights reserved
 """
 
 """
 This file contains the exports to
 ```py
 import thread
 ```
 """
 
 
-__version__ = '1.1.1'
+__version__ = '2.0.0'
 
 
 # Export Core
-from .thread import Thread, ParallelProcessing
+from .thread import Thread, ConcurrentProcessing
 
 
 from . import _types as types, exceptions
 
 
 # Export decorators
 from .decorators import threaded, processor
@@ -35,15 +35,15 @@
 # Configuration
 from .utils import Settings
 
 
 # Wildcard Export
 __all__ = [
     'Thread',
-    'ParallelProcessing',
+    'ConcurrentProcessing',
     'threaded',
     'processor',
     'types',
     'exceptions',
     'Settings',
     '__version__',
 ]
```

### Comparing `thread-1.1.1/src/thread/_types.py` & `thread-2.0.0/src/thread/_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 ## Types
 
-Documentation: https://thread.ngjx.org/docs/v1.1.1
+Documentation: https://thread.ngjx.org/docs/v2.0.0
 """
 
 from typing import Any, Literal, Callable, Union, Sized
 from typing_extensions import (
     ParamSpec,
     TypeVar,
     Concatenate,
```

### Comparing `thread-1.1.1/src/thread/decorators/_processor.py` & `thread-2.0.0/src/thread/decorators/_processor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 ## Processor
 
-Documentation: https://thread.ngjx.org/docs/v1.1.1
+Documentation: https://thread.ngjx.org/docs/v2.0.0
 """
 
 from functools import wraps
-from ..thread import ParallelProcessing
+from ..thread import ConcurrentProcessing
 
 from .._types import (
     Overflow_In,
     Data_In,
     SupportsGetItem,
     SupportsLength,
     SupportsLengthGetItem,
@@ -25,53 +25,56 @@
 Dataset = Union[
     SupportsLengthGetItem[_DataT], SupportsGetItem[_DataT], SupportsLength, Any
 ]
 
 
 NoParamReturn = Callable[
     Concatenate[Dataset[_DataT], _TargetP],
-    ParallelProcessing[_TargetP, _TargetT, _DataT],
+    ConcurrentProcessing[_TargetP, _TargetT, _DataT],
 ]
 WithParamReturn = Callable[
     [TargetFunction[_DataT, _TargetP, _TargetT]],
     NoParamReturn[_DataT, _TargetP, _TargetT],
 ]
 FullParamReturn = Callable[
     Concatenate[Dataset[_DataT], _TargetP],
-    ParallelProcessing[_TargetP, _TargetT, _DataT],
+    ConcurrentProcessing[_TargetP, _TargetT, _DataT],
 ]
 
 
 @overload
 def processor(
     __function: TargetFunction[_DataT, _TargetP, _TargetT],
-) -> NoParamReturn[_DataT, _TargetP, _TargetT]: ...
+) -> NoParamReturn[_DataT, _TargetP, _TargetT]:
+    ...
 
 
 @overload
 def processor(
     *,
     args: Sequence[Data_In] = (),
     kwargs: Mapping[str, Data_In] = {},
     ignore_errors: Sequence[type[Exception]] = (),
     suppress_errors: bool = False,
     **overflow_kwargs: Overflow_In,
-) -> WithParamReturn[_DataT, _TargetP, _TargetT]: ...
+) -> WithParamReturn[_DataT, _TargetP, _TargetT]:
+    ...
 
 
 @overload
 def processor(
     __function: TargetFunction[_DataT, _TargetP, _TargetT],
     *,
     args: Sequence[Data_In] = (),
     kwargs: Mapping[str, Data_In] = {},
     ignore_errors: Sequence[type[Exception]] = (),
     suppress_errors: bool = False,
     **overflow_kwargs: Overflow_In,
-) -> FullParamReturn[_DataT, _TargetP, _TargetT]: ...
+) -> FullParamReturn[_DataT, _TargetP, _TargetT]:
+    ...
 
 
 def processor(
     __function: Optional[TargetFunction[_DataT, _TargetP, _TargetT]] = None,
     *,
     args: Sequence[Data_In] = (),
     kwargs: Mapping[str, Data_In] = {},
@@ -146,23 +149,23 @@
     kwargs = dict(kwargs)
 
     @wraps(__function)
     def wrapped(
         data: Dataset[_DataT],
         *parsed_args: _TargetP.args,
         **parsed_kwargs: _TargetP.kwargs,
-    ) -> ParallelProcessing[_TargetP, _TargetT, _DataT]:
+    ) -> ConcurrentProcessing[_TargetP, _TargetT, _DataT]:
         kwargs.update(parsed_kwargs)
 
         processed_args = (*args, *parsed_args)
         processed_kwargs = {
             i: v for i, v in kwargs.items() if i not in ['args', 'kwargs']
         }
 
-        job = ParallelProcessing(
+        job = ConcurrentProcessing(
             function=__function,
             dataset=data,
             args=processed_args,
             kwargs=processed_kwargs,
             **overflow_kwargs,
         )
         job.start()
```

### Comparing `thread-1.1.1/src/thread/decorators/_threaded.py` & `thread-2.0.0/src/thread/decorators/_threaded.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 ## Threaded
 
-Documentation: https://thread.ngjx.org/docs/v1.1.1
+Documentation: https://thread.ngjx.org/docs/v2.0.0
 """
 
 from functools import wraps
 from ..thread import Thread
 
 from .._types import Overflow_In, Data_In
 from typing import Callable, Mapping, Sequence, Optional, Union, overload
@@ -19,38 +19,41 @@
 
 NoParamReturn = Callable[P, Thread[P, T]]
 WithParamReturn = Callable[[TargetFunction[P, T]], NoParamReturn[P, T]]
 FullParamReturn = Callable[P, Thread[P, T]]
 
 
 @overload
-def threaded(__function: TargetFunction[P, T]) -> NoParamReturn[P, T]: ...
+def threaded(__function: TargetFunction[P, T]) -> NoParamReturn[P, T]:
+    ...
 
 
 @overload
 def threaded(
     *,
     args: Sequence[Data_In] = (),
     kwargs: Mapping[str, Data_In] = {},
     ignore_errors: Sequence[type[Exception]] = (),
     suppress_errors: bool = False,
     **overflow_kwargs: Overflow_In,
-) -> WithParamReturn[P, T]: ...
+) -> WithParamReturn[P, T]:
+    ...
 
 
 @overload
 def threaded(
     __function: TargetFunction[P, T],
     *,
     args: Sequence[Data_In] = (),
     kwargs: Mapping[str, Data_In] = {},
     ignore_errors: Sequence[type[Exception]] = (),
     suppress_errors: bool = False,
     **overflow_kwargs: Overflow_In,
-) -> FullParamReturn[P, T]: ...
+) -> FullParamReturn[P, T]:
+    ...
 
 
 def threaded(
     __function: Optional[TargetFunction[P, T]] = None,
     *,
     args: Sequence[Data_In] = (),
     kwargs: Mapping[str, Data_In] = {},
```

### Comparing `thread-1.1.1/src/thread/exceptions.py` & `thread-2.0.0/src/thread/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 ## Thread Exceptions
 
-Documentation: https://thread.ngjx.org/docs/v1.1.1
+Documentation: https://thread.ngjx.org/docs/v2.0.0
 """
 
 import traceback
 from typing import Any, Optional, Sequence, Tuple
 
 
 class ErrorBase(Exception):
```

### Comparing `thread-1.1.1/src/thread/thread.py` & `thread-2.0.0/src/thread/thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 ## Core of thread
 
 ```py
 class Thread: ...
 
 
-class ParallelProcessing: ...
+class ConcurrentProcessing: ...
 ```
 
-Documentation: https://thread.ngjx.org/docs/v1.1.1
+Documentation: https://thread.ngjx.org/docs/v2.0.0
 """
 
 import sys
 import time
 import ctypes
 import signal
 import threading
@@ -226,40 +226,35 @@
 
         Parameters
         ----------
         :param hook: This should be a function which takes the output value of `target` and should return None
         """
         self.hooks.append(hook)
 
-    def join(self, timeout: Optional[float] = None) -> bool:
+    def join(self, timeout: Optional[float] = None) -> None:
         """
         Halts the current thread execution until a thread completes or exceeds the timeout
 
         Parameters
         ----------
         :param timeout: The maximum time allowed to halt the thread
 
-        Returns
-        -------
-        :returns bool: True if the thread is no-longer alive
-
         Raises
         ------
         ThreadNotInitializedError: If the thread is not initialized
         ThreadNotRunningError: If the thread is not running
         """
         if not self._initialized:
             raise exceptions.ThreadNotInitializedError()
 
         if self.status == ['Idle', 'Killed']:
             raise exceptions.ThreadNotRunningError()
 
         super().join(timeout)
         self._handle_exceptions()
-        return not self.is_alive()
 
     def get_return_value(self) -> _Target_T:
         """
         Halts the current thread execution until the thread completes
 
         Returns
         -------
@@ -337,17 +332,17 @@
     thread: Thread
 
     def __init__(self, thread: Thread, progress: float = 0) -> None:
         self.thread = thread
         self.progress = progress
 
 
-class ParallelProcessing(Generic[_Target_P, _Target_T, _Dataset_T]):
+class ConcurrentProcessing(Generic[_Target_P, _Target_T, _Dataset_T]):
     """
-    Multi-Threaded Parallel Processing
+    Concurrent Processing
     ---------------------------------------
 
     Type-Safe and provides more functionality on top
     """
 
     _length: int
     _retrieve_value: Callable[[Any, int], _Dataset_T]
@@ -374,54 +369,58 @@
         function: DatasetFunction[_Dataset_T, _Target_P, _Target_T],
         dataset: LengthandGetLike_T,
         max_threads: int = 8,
         *overflow_args: Overflow_In,
         _get_value: Optional[Callable[[LengthandGetLike_T, int], _Dataset_T]] = None,
         _length: Optional[Union[int, Callable[[Any], int]]] = None,
         **overflow_kwargs: Overflow_In,
-    ) -> None: ...
+    ) -> None:
+        ...
 
     # Has __len__, require _get_value to be set
     @overload
     def __init__(
         self,
         function: DatasetFunction[_Dataset_T, _Target_P, _Target_T],
         dataset: LengthLike_T,
         max_threads: int = 8,
         *overflow_args: Overflow_In,
         _get_value: Callable[[LengthLike_T, int], _Dataset_T],
         _length: Optional[Union[int, Callable[[Any], int]]] = None,
         **overflow_kwargs: Overflow_In,
-    ) -> None: ...
+    ) -> None:
+        ...
 
     # Has __getitem__, require _length to be set
     @overload
     def __init__(
         self,
         function: DatasetFunction[_Dataset_T, _Target_P, _Target_T],
         dataset: GetLike_T,
         max_threads: int = 8,
         *overflow_args: Overflow_In,
         _get_value: Optional[Callable[[GetLike_T, int], _Dataset_T]] = None,
         _length: Union[int, Callable[[GetLike_T], int]],
         **overflow_kwargs: Overflow_In,
-    ) -> None: ...
+    ) -> None:
+        ...
 
     # Does not support __getitem__ and __len__
     @overload
     def __init__(
         self,
         function: DatasetFunction[_Dataset_T, _Target_P, _Target_T],
         dataset: Any,
         max_threads: int = 8,
         *overflow_args: Overflow_In,
         _get_value: Callable[[Any, int], _Dataset_T],
         _length: Union[int, Callable[[Any], int]],
         **overflow_kwargs: Overflow_In,
-    ) -> None: ...
+    ) -> None:
+        ...
 
     def __init__(
         self,
         function: DatasetFunction[_Dataset_T, _Target_P, _Target_T],
         dataset: Union[
             SupportsLengthGetItem[_Dataset_T],
             SupportsGetItem[_Dataset_T],
@@ -438,18 +437,18 @@
                 Callable[[Any, int], _Dataset_T],
             ]
         ] = None,
         _length: Optional[Union[int, Callable[[Any], int]]] = None,
         **overflow_kwargs: Overflow_In,
     ) -> None:
         """
-        Initializes a new Multi-Threaded Pool\n
+        Initializes a new Concurrent Process\n
         Best for data processing
 
-        Splits a dataset as evenly as it can among the threads and run them in parallel
+        Splits a dataset as evenly as it can among the threads and run them concurrently
 
         Parameters
         ----------
         :param function: This should be the function to validate each data entry in the `dataset`, the first argument parsed will be a value of the dataset
         :param dataset: This should be an iterable sequence of data entries
         :param max_threads: This should be an integer value of the max threads allowed
         :param *: These are arguments parsed to `threading.Thread` and `Thread`
@@ -594,36 +593,31 @@
         """
         results: List[Data_Out] = []
         for entry in self._threads:
             entry.thread.join()
             results += entry.thread.result
         return results
 
-    def join(self) -> bool:
+    def join(self) -> None:
         """
         Halts the current thread execution until a thread completes or exceeds the timeout
 
-        Returns
-        -------
-        :returns bool: True if the thread is no-longer alive
-
         Raises
         ------
         ThreadNotInitializedError: If the thread is not initialized
         ThreadNotRunningError: If the thread is not running
         """
         if len(self._threads) == 0:
             raise exceptions.ThreadNotInitializedError()
 
         if self.status == 'Idle':
             raise exceptions.ThreadNotRunningError()
 
         for entry in self._threads:
             entry.thread.join()
-        return True
 
     def kill(self) -> None:
         """
         Kills the threads
 
         Raises
         ------
```

### Comparing `thread-1.1.1/src/thread/utils/algorithm.py` & `thread-2.0.0/src/thread/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `thread-1.1.1/src/thread/utils/config.py` & `thread-2.0.0/src/thread/utils/config.py`

 * *Files identical despite different names*

### Comparing `thread-1.1.1/tests/test_algorithm.py` & `thread-2.0.0/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `thread-1.1.1/tests/test_dataframe_compatibility.py` & `thread-2.0.0/tests/test_dataframe_compatibility.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing
 import pytest
-from src.thread import ParallelProcessing
+from src.thread import ConcurrentProcessing
 
 
 class DummyLengthOnly:
     length: typing.Any
 
     def __init__(self, length: typing.Any):
         self.length = length
@@ -29,362 +29,367 @@
 
     def __init__(self, length: typing.Any, dataset: list):
         DummyLengthOnly.__init__(self, length)
         DummyGetOnly.__init__(self, dataset)
 
 
 class DummyUnlikeSequence1:
-    def __init__(self) -> None: ...
+    def __init__(self) -> None:
+        ...
 
 
 class DummyUnlikeSequence2:
-    def __init__(self) -> None: ...
+    def __init__(self) -> None:
+        ...
+
     def __str__(self) -> str:
         return 'invalid'
 
 
 # >>>>>>>>>> Length Only <<<<<<<<<< #
 def test_LO_init() -> None:
-    ParallelProcessing(
+    ConcurrentProcessing(
         function=lambda x: x,
         dataset=DummyLengthOnly(10),
         _get_value=lambda *_: _,
     )
 
 
 def test_LO_init_missingGetValueError_nothing() -> None:
     with pytest.raises(TypeError):
-        ParallelProcessing(
+        ConcurrentProcessing(
             function=lambda x: x,
             dataset=DummyLengthOnly(10),  # type: ignore
         )
 
 
 def test_LO_init_missingGetValueError_lengthNum() -> None:
     with pytest.raises(TypeError):
-        ParallelProcessing(
+        ConcurrentProcessing(
             function=lambda x: x,
             dataset=DummyLengthOnly(10),  # type: ignore
             _length=1,
         )
 
 
 def test_LO_init_missingGetValueError_lengthFunc() -> None:
     with pytest.raises(TypeError):
-        ParallelProcessing(
+        ConcurrentProcessing(
             function=lambda x: x,
             dataset=DummyLengthOnly(10),  # type: ignore
             _length=lambda _: 1,
         )
 
 
 def test_LO_init_invalidLengthValueError_negative() -> None:
     with pytest.raises(ValueError):
-        ParallelProcessing(
+        ConcurrentProcessing(
             function=lambda x: x,
             dataset=DummyLengthOnly(-10),
             _get_value=lambda *_: _,
         )
 
 
 def test_LO_init_invalidLengthValueError_zero() -> None:
     with pytest.raises(ValueError):
-        ParallelProcessing(
+        ConcurrentProcessing(
             function=lambda x: x,
             dataset=DummyLengthOnly(0),
             _get_value=lambda *_: _,
         )
 
 
 def test_LO_init_nonIntLengthError_numLike() -> None:
     with pytest.raises(TypeError):
-        ParallelProcessing(
+        ConcurrentProcessing(
             function=lambda x: x,
             dataset=DummyLengthOnly(10.5),
             _get_value=lambda *_: _,
         )
 
 
 def test_LO_init_nonIntLengthError() -> None:
     with pytest.raises(TypeError):
-        ParallelProcessing(
+        ConcurrentProcessing(
             function=lambda x: x,
             dataset=DummyLengthOnly('10'),
             _get_value=lambda *_: _,
         )
 
 
 def test_LO_enforceTypes() -> None:
     def validate(x, i):
         assert isinstance(x, DummyLengthOnly)
         assert isinstance(i, int)
 
-    process = ParallelProcessing(
+    process = ConcurrentProcessing(
         function=lambda x: x,
         dataset=DummyLengthOnly(10),
         _get_value=validate,
     )
     process.start()
     process.join()
 
 
 def test_LO_len() -> None:
-    process = ParallelProcessing(
+    process = ConcurrentProcessing(
         function=lambda x: x,
         dataset=DummyLengthOnly(10),
         _get_value=lambda *_: _,
     )
     assert process._length == 10
 
 
 # >>>>>>>>>> Get Only <<<<<<<<<< #
 def test_GO_init_int() -> None:
-    ParallelProcessing(function=lambda x: x, dataset=DummyGetOnly([1, 2, 3]), _length=3)
+    ConcurrentProcessing(
+        function=lambda x: x, dataset=DummyGetOnly([1, 2, 3]), _length=3
+    )
 
 
 def test_GO_init_func() -> None:
-    ParallelProcessing(
+    ConcurrentProcessing(
         function=lambda x: x, dataset=DummyGetOnly([1, 2, 3]), _length=lambda _: 3
     )
 
 
 def test_GO_init_missingLengthError() -> None:
     with pytest.raises(TypeError):
-        ParallelProcessing(
+        ConcurrentProcessing(
             function=lambda x: x,
             dataset=DummyGetOnly([1, 2, 3]),  # type: ignore
         )
 
 
 def test_GO_init_nonIntLengthError_strLike() -> None:
     with pytest.raises(TypeError):
-        ParallelProcessing(
+        ConcurrentProcessing(
             function=lambda x: x,
             dataset=DummyGetOnly([1, 2, 3]),
             _length='10',  # type: ignore
         )
 
 
 def test_GO_init_nonIntLengthError_numLike() -> None:
     with pytest.raises(TypeError):
-        ParallelProcessing(
+        ConcurrentProcessing(
             function=lambda x: x,
             dataset=DummyGetOnly([1, 2, 3]),
             _length=10.5,  # type: ignore
         )
 
 
 def test_GO_init_nonIntLengthError_negative() -> None:
     with pytest.raises(ValueError):
-        ParallelProcessing(
+        ConcurrentProcessing(
             function=lambda x: x,
             dataset=DummyGetOnly([1, 2, 3]),
             _length=-10,  # type: ignore
         )
 
 
 def test_GO_enforceTypes() -> None:
     def validate(x, i):
         assert isinstance(x, DummyGetOnly)
         assert isinstance(i, int)
 
-    process = ParallelProcessing(
+    process = ConcurrentProcessing(
         function=lambda x: x,
         dataset=DummyGetOnly([1, 2, 3]),
         _length=3,
         _get_value=validate,
     )
     process.start()
     process.join()
 
 
 def test_GO_len() -> None:
-    process = ParallelProcessing(
+    process = ConcurrentProcessing(
         function=lambda x: x,
         dataset=DummyGetOnly([1, 2, 3]),
         _length=3,
         _get_value=lambda *_: _,
     )
     assert process._length == 3
 
 
 def test_GO_get() -> None:
     def get(*_):
         return _
 
-    process = ParallelProcessing(
+    process = ConcurrentProcessing(
         function=lambda x: x,
         dataset=DummyGetOnly([1, 2, 3]),
         _length=3,
         _get_value=get,
     )
     assert process._retrieve_value == get
 
 
 # >>>>>>>> Sequence Like <<<<<<<< #
 def test_SO_init() -> None:
-    ParallelProcessing(
+    ConcurrentProcessing(
         function=lambda x: x,
         dataset=DummySequenceLike(10, list(range(10))),
     )
 
 
 def test_SO_init_list() -> None:
-    ParallelProcessing(
+    ConcurrentProcessing(
         function=lambda x: x,
         dataset=[1, 2, 3],
     )
 
 
 def test_SO_init_tuple() -> None:
-    ParallelProcessing(
+    ConcurrentProcessing(
         function=lambda x: x,
         dataset=(1, 2, 3),
     )
 
 
 def test_SO_init_set() -> None:
     with pytest.raises(TypeError):
-        ParallelProcessing(
+        ConcurrentProcessing(
             function=lambda x: x,
             dataset=set([1, 2, 3]),  # type: ignore
         )
 
 
 def test_SO_init_dict() -> None:
-    ParallelProcessing(
+    ConcurrentProcessing(
         function=lambda x: x,
         dataset={1: 1, 2: 2, 3: 3},  # type: ignore
     )
 
 
 def test_SO_init_str() -> None:
-    ParallelProcessing(
+    ConcurrentProcessing(
         function=lambda x: x,
         dataset='123',
     )
 
 
 def test_SO_init_withLength() -> None:
-    ParallelProcessing(
+    ConcurrentProcessing(
         function=lambda x: x,
         dataset=DummySequenceLike(10, list(range(10))),
         _length=10,
     )
 
 
 def test_SO_init_withGet() -> None:
-    ParallelProcessing(
+    ConcurrentProcessing(
         function=lambda x: x,
         dataset=DummySequenceLike(10, list(range(10))),
         _get_value=lambda *_: _,
     )
 
 
 def test_SO_init_withLengthAndGet() -> None:
-    ParallelProcessing(
+    ConcurrentProcessing(
         function=lambda x: x,
         dataset=DummySequenceLike(10, list(range(10))),
         _length=10,
         _get_value=lambda *_: _,
     )
 
 
 def test_SO_len() -> None:
-    process = ParallelProcessing(
+    process = ConcurrentProcessing(
         function=lambda x: x,
         dataset=DummySequenceLike(10, list(range(10))),
     )
     assert process._length == 10
 
 
 def test_SO_enforceTypes() -> None:
     def validate(x, i):
         assert isinstance(x, DummySequenceLike)
         assert isinstance(i, int)
 
-    process = ParallelProcessing(
+    process = ConcurrentProcessing(
         function=lambda x: x,
         dataset=DummySequenceLike(10, list(range(10))),
         _get_value=validate,
     )
     process.start()
     process.join()
 
 
 # >>>>>>>>>> Unlike Sequence <<<<<<<<<< #
 def test_UO_init_clean() -> None:
     with pytest.raises(TypeError):
-        ParallelProcessing(
+        ConcurrentProcessing(
             function=lambda x: x,
             dataset=DummyUnlikeSequence1(),  # type: ignore
         )
 
 
 def test_UO_init_withOtherMethods() -> None:
     with pytest.raises(TypeError):
-        ParallelProcessing(
+        ConcurrentProcessing(
             function=lambda x: x,
             dataset=DummyUnlikeSequence2(),  # type: ignore
         )
 
 
 def test_UO_init_onlyLength() -> None:
     with pytest.raises(TypeError):
-        ParallelProcessing(
+        ConcurrentProcessing(
             function=lambda x: x,
             dataset=DummyUnlikeSequence1(),  # type: ignore
             _length=10,
         )
 
 
 def test_UO_init_onlyGet() -> None:
     with pytest.raises(TypeError):
-        ParallelProcessing(
+        ConcurrentProcessing(
             function=lambda x: x,
             dataset=DummyUnlikeSequence1(),  # type: ignore
             _get_value=lambda *_: _,
         )
 
 
 def test_UO_init_onlyLengthAndGet() -> None:
-    ParallelProcessing(
+    ConcurrentProcessing(
         function=lambda x: x,
         dataset=DummyUnlikeSequence1(),  # type: ignore
         _length=10,
         _get_value=lambda *_: _,
     )
 
 
 def test_UO_lengthInt() -> None:
-    process = ParallelProcessing(
+    process = ConcurrentProcessing(
         function=lambda x: x,
         dataset=DummyUnlikeSequence1(),
         _length=10,
         _get_value=lambda *_: _,
     )
     assert process._length == 10
 
 
 def test_UO_lengthFunc() -> None:
-    process = ParallelProcessing(
+    process = ConcurrentProcessing(
         function=lambda x: x,
         dataset=DummyUnlikeSequence1(),
         _length=lambda _: 10,
         _get_value=lambda *_: _,
     )
     assert process._length == 10
 
 
 def test_UO_enforceTypes() -> None:
     def validate(x, i):
         assert isinstance(x, DummyUnlikeSequence1)
         assert isinstance(i, int)
 
-    process = ParallelProcessing(
+    process = ConcurrentProcessing(
         function=lambda x: x,
         dataset=DummyUnlikeSequence1(),
         _length=10,
         _get_value=validate,
     )
     process.start()
     process.join()
```

### Comparing `thread-1.1.1/tests/test_decorator.py` & `thread-2.0.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `thread-1.1.1/tests/test_parallelprocessing.py` & `thread-2.0.0/tests/test_concurrentprocessing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 import pytest
-from src.thread import ParallelProcessing, exceptions
+from src.thread import ConcurrentProcessing, exceptions
 
 
 # >>>>>>>>>> Dummy Functions <<<<<<<<<< #
 def _dummy_dataProcessor(data_in: int, delay: float = 0) -> int:
     time.sleep(delay)
     return data_in
 
@@ -14,49 +14,49 @@
     raise x
 
 
 # >>>>>>>>>> General Use <<<<<<<<<< #
 def test_threadsScaleDown():
     """This test is for testing if threads scale down `max_threads` when the dataset is lesser than the thread count"""
     dataset = list(range(0, 2))
-    new = ParallelProcessing(
+    new = ConcurrentProcessing(
         function=_dummy_dataProcessor,
         dataset=dataset,
         max_threads=4,
         kwargs={'delay': 2},
         daemon=True,
     )
     new.start()
     assert len(new._threads) == 2
 
 
 def test_threadsProcessing():
     """This test is for testing if threads correctly order data in the `dataset` arrangement"""
     dataset = list(range(0, 500))
-    new = ParallelProcessing(
+    new = ConcurrentProcessing(
         function=_dummy_dataProcessor, dataset=dataset, args=[0.001], daemon=True
     )
     new.start()
     assert new.get_return_values() == dataset
 
 
 # >>>>>>>>>> Raising Exceptions <<<<<<<<<< #
 def test_raises_StillRunningError():
     """This test should raise ThreadStillRunningError"""
     dataset = list(range(0, 8))
-    new = ParallelProcessing(
+    new = ConcurrentProcessing(
         function=_dummy_dataProcessor, dataset=dataset, args=[1], daemon=True
     )
     new.start()
     with pytest.raises(exceptions.ThreadStillRunningError):
         _ = new.results
 
 
 def test_raises_RunTimeError():
     """This test should raise a RunTimeError"""
     dataset = [RuntimeError()] * 8
-    new = ParallelProcessing(
+    new = ConcurrentProcessing(
         function=_dummy_raiseException, dataset=dataset, args=[0.01], daemon=True
     )
     with pytest.raises(RuntimeError):
         new.start()
         new.join()
```

### Comparing `thread-1.1.1/tests/test_thread.py` & `thread-2.0.0/tests/test_thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 # >>>>>>>>>> General Use <<<<<<<<<< #
 def test_threadCreation():
     """This test is for testing parsing of args and kwargs and `.join()` method"""
     new = Thread(
         target=_dummy_target_raiseToPower, args=[4], kwargs={'power': 2}, daemon=True
     )
     new.start()
-    assert new.join()
+    new.join()
+    assert not new.is_alive()
     assert new.result == 16
 
 
 def test_threadingThreadParsing():
     """This test is for testing parsing arguments to `threading.Thead`"""
     new = Thread(
         target=_dummy_target_raiseToPower,
```

### Comparing `thread-1.1.1/tests/test_verbosity.py` & `thread-2.0.0/tests/test_verbosity.py`

 * *Files identical despite different names*

### Comparing `thread-1.1.1/PKG-INFO` & `thread-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thread
-Version: 1.1.1
+Version: 2.0.0
 Summary: Threading module extension
 License: BSD-3-Clause
 Keywords: thread,threading,extension,multiprocessing
 Author: Alex
 Author-email: contact@ngjx.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/python-thread/thread/issues
-Project-URL: Documentation, https://thread.ngjx.org/docs/v1.1.1
+Project-URL: Documentation, https://thread.ngjx.org/docs/v2.0.0
 Project-URL: Download, https://pypi.org/project/thread/#files
 Project-URL: Homepage, https://thread.ngjx.org
 Project-URL: Release Notes, https://github.com/python-thread/thread/releases
 Project-URL: Source, https://github.com/python-thread/thread
 Description-Content-Type: text/markdown
 
 <a name="readme-top"></a>
@@ -107,15 +107,15 @@
 1. Install the package
    ```sh
    pip install -U thread
    ```
 2. Import thread into your library!
    ```py
    import thread
-   from thread import Thread, ParallelProcessing
+   from thread import Thread, ConcurrentProcessing
    ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- DOCS -->
@@ -126,15 +126,15 @@
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- ROADMAP -->
 ## Roadmap
 
-- [x] v1.1.1 Release
+- [x] v2.0.0 Release
 - [ ] Bug fixes
 - [ ] New features
 - [ ] Testing
 - [ ] Next release...
 
 See the [open issues](https://github.com/python-thread/thread/issues) for a full list of proposed features (and known issues).
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: thread Version: 1.1.1 Summary: Threading module
+Metadata-Version: 2.1 Name: thread Version: 2.0.0 Summary: Threading module
 extension License: BSD-3-Clause Keywords:
 thread,threading,extension,multiprocessing Author: Alex Author-email:
 contact@ngjx.org Requires-Python: >=3.9,<4.0 Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: BSD License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Topic :: Software Development
 Classifier: Typing :: Typed Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/python-thread/thread/issues
-Project-URL: Documentation, https://thread.ngjx.org/docs/v1.1.1 Project-URL:
+Project-URL: Documentation, https://thread.ngjx.org/docs/v2.0.0 Project-URL:
 Download, https://pypi.org/project/thread/#files Project-URL: Homepage, https:/
 /thread.ngjx.org Project-URL: Release Notes, https://github.com/python-thread/
 thread/releases Project-URL: Source, https://github.com/python-thread/thread
 Description-Content-Type: text/markdown
  _[_!_[_P_Y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_v_e_r_s_i_o_n_-_s_h_i_e_l_d_]_]_[_p_y_p_i_-_u_r_l_] _[_!_[_P_Y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]_[_d_o_w_n_l_o_a_d_s_-
  _s_h_i_e_l_d_]_]_[_p_y_p_i_-_u_r_l_] _[_!_[_F_o_r_k_s_]_[_f_o_r_k_s_-_s_h_i_e_l_d_]_]_[_f_o_r_k_s_-_u_r_l_] _[_!_[_S_t_a_r_g_a_z_e_r_s_]_[_s_t_a_r_s_-
   _s_h_i_e_l_d_]_]_[_s_t_a_r_s_-_u_r_l_] _[_!_[_B_S_D_-_3_-_C_l_a_u_s_e_ _L_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_-_s_h_i_e_l_d_]_]_[_l_i_c_e_n_s_e_-_u_r_l_]
@@ -38,19 +38,19 @@
 I hope thread will become your threading solution! â¡â¸(Ë¶Ë áµ ËË¶)â¸â¡
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Getting Started This is an example of how you can set up your project
 locally. To get a local copy up and running follow these simple example steps.
 ### Prerequisites * Python 3.9+ ### Installation _Below is an example of how
 you can install and use thread._ 1. Install the package ```sh pip install -
 U thread ``` 2. Import thread into your library! ```py import thread from
-thread import Thread, ParallelProcessing ```
+thread import Thread, ConcurrentProcessing ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Documentation Our docs are [here!](https://thread.ngjx.org)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Roadmap - [x] v1.1.1 Release - [ ] Bug fixes - [ ] New features - [ ]
+## Roadmap - [x] v2.0.0 Release - [ ] Bug fixes - [ ] New features - [ ]
 Testing - [ ] Next release... See the [open issues](https://github.com/python-
 thread/thread/issues) for a full list of proposed features (and known issues).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. ( Ë¶ËáËËµ ) If you have a suggestion that would
 make this better, please fork the repo and create a pull request. You can also
```


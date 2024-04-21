# Comparing `tmp/fsspec_xrootd-0.2.4.tar.gz` & `tmp/fsspec_xrootd-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsspec_xrootd-0.2.4.tar", last modified: Fri Dec 22 20:55:30 2023, max compression
+gzip compressed data, was "fsspec_xrootd-0.3.0.tar", last modified: Sun Apr 21 14:42:50 2024, max compression
```

## Comparing `fsspec_xrootd-0.2.4.tar` & `fsspec_xrootd-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:55:30.384029 fsspec_xrootd-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:55:30.376028 fsspec_xrootd-0.2.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:55:30.380028 fsspec_xrootd-0.2.4/.github/matchers/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/.github/matchers/pylint.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:55:30.380028 fsspec_xrootd-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2023-12-22 20:55:30.384029 fsspec_xrootd-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:55:30.380028 fsspec_xrootd-0.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      759 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2023-12-22 20:55:30.384029 fsspec_xrootd-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:55:30.376028 fsspec_xrootd-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:55:30.380028 fsspec_xrootd-0.2.4/src/fsspec_xrootd/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/src/fsspec_xrootd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-22 20:55:30.000000 fsspec_xrootd-0.2.4/src/fsspec_xrootd/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/src/fsspec_xrootd/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/src/fsspec_xrootd/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    27268 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/src/fsspec_xrootd/xrootd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:55:30.380028 fsspec_xrootd-0.2.4/src/fsspec_xrootd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2023-12-22 20:55:30.000000 fsspec_xrootd-0.2.4/src/fsspec_xrootd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-12-22 20:55:30.000000 fsspec_xrootd-0.2.4/src/fsspec_xrootd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 20:55:30.000000 fsspec_xrootd-0.2.4/src/fsspec_xrootd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-22 20:55:30.000000 fsspec_xrootd-0.2.4/src/fsspec_xrootd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-22 20:55:30.000000 fsspec_xrootd-0.2.4/src/fsspec_xrootd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-22 20:55:30.000000 fsspec_xrootd-0.2.4/src/fsspec_xrootd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:55:30.380028 fsspec_xrootd-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14483 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/tests/test_basicio.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-22 20:55:23.000000 fsspec_xrootd-0.2.4/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:42:50.380331 fsspec_xrootd-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:42:50.372331 fsspec_xrootd-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:42:50.372331 fsspec_xrootd-0.3.0/.github/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/.github/matchers/pylint.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:42:50.372331 fsspec_xrootd-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-21 14:42:50.380331 fsspec_xrootd-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:42:50.376331 fsspec_xrootd-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-21 14:42:50.380331 fsspec_xrootd-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:42:50.372331 fsspec_xrootd-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:42:50.376331 fsspec_xrootd-0.3.0/src/fsspec_xrootd/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/src/fsspec_xrootd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 14:42:50.000000 fsspec_xrootd-0.3.0/src/fsspec_xrootd/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/src/fsspec_xrootd/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/src/fsspec_xrootd/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    30187 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/src/fsspec_xrootd/xrootd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:42:50.376331 fsspec_xrootd-0.3.0/src/fsspec_xrootd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-21 14:42:50.000000 fsspec_xrootd-0.3.0/src/fsspec_xrootd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-21 14:42:50.000000 fsspec_xrootd-0.3.0/src/fsspec_xrootd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 14:42:50.000000 fsspec_xrootd-0.3.0/src/fsspec_xrootd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-21 14:42:50.000000 fsspec_xrootd-0.3.0/src/fsspec_xrootd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-21 14:42:50.000000 fsspec_xrootd-0.3.0/src/fsspec_xrootd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 14:42:50.000000 fsspec_xrootd-0.3.0/src/fsspec_xrootd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:42:50.376331 fsspec_xrootd-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    16577 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/tests/test_basicio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-21 14:42:46.000000 fsspec_xrootd-0.3.0/tests/test_package.py
```

### Comparing `fsspec_xrootd-0.2.4/.github/CONTRIBUTING.md` & `fsspec_xrootd-0.3.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fsspec_xrootd-0.2.4/.github/matchers/pylint.json` & `fsspec_xrootd-0.3.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `fsspec_xrootd-0.2.4/.github/workflows/ci.yml` & `fsspec_xrootd-0.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fsspec_xrootd-0.2.4/.github/workflows/docs.yml` & `fsspec_xrootd-0.3.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `fsspec_xrootd-0.2.4/LICENSE` & `fsspec_xrootd-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fsspec_xrootd-0.2.4/PKG-INFO` & `fsspec_xrootd-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsspec_xrootd
-Version: 0.2.4
+Version: 0.3.0
 Summary: xrootd implementation for fsspec
 Home-page: https://github.com/CoffeaTeam/fsspec-xrootd
 Author: Scott Demarest
 Author-email: rockets1194@gmail.com
 Maintainer: CoffeaTeam admins
 Maintainer-email: rockets1194@gmail.com
 License: BSD-3-Clause
@@ -48,15 +48,15 @@
 ```bash
 pip install fsspec-xrootd
 ```
 
 ## Purpose
 
 To allow fsspec to use XRootD accessible storage systems. Install fsspec-xrootd
-alongside fsspec and have easy access to files stored on XRootD serevrs. Once
+alongside fsspec and have easy access to files stored on XRootD servers. Once
 installed, fsspec will be able to work with urls with the 'root' protocol. Only
 tested with Linux at this time.
 
 ## Documentation
 
 Please refer to [RTD](https://coffeateam.github.io/fsspec-xrootd/)
```

### Comparing `fsspec_xrootd-0.2.4/README.md` & `fsspec_xrootd-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ```bash
 pip install fsspec-xrootd
 ```
 
 ## Purpose
 
 To allow fsspec to use XRootD accessible storage systems. Install fsspec-xrootd
-alongside fsspec and have easy access to files stored on XRootD serevrs. Once
+alongside fsspec and have easy access to files stored on XRootD servers. Once
 installed, fsspec will be able to work with urls with the 'root' protocol. Only
 tested with Linux at this time.
 
 ## Documentation
 
 Please refer to [RTD](https://coffeateam.github.io/fsspec-xrootd/)
```

### Comparing `fsspec_xrootd-0.2.4/docs/Makefile` & `fsspec_xrootd-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fsspec_xrootd-0.2.4/docs/conf.py` & `fsspec_xrootd-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fsspec_xrootd-0.2.4/docs/index.rst` & `fsspec_xrootd-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fsspec_xrootd-0.2.4/docs/make.bat` & `fsspec_xrootd-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fsspec_xrootd-0.2.4/noxfile.py` & `fsspec_xrootd-0.3.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `fsspec_xrootd-0.2.4/pyproject.toml` & `fsspec_xrootd-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 files = "src"
 python_version = "3.7"
 warn_unused_configs = true
 strict = true
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
+ignore_missing_imports = true
 
 
 [tool.check-manifest]
 ignore = [
     ".github/**",
     "docs/**",
     ".pre-commit-config.yaml",
```

### Comparing `fsspec_xrootd-0.2.4/setup.cfg` & `fsspec_xrootd-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fsspec_xrootd-0.2.4/src/fsspec_xrootd/xrootd.py` & `fsspec_xrootd-0.3.0/src/fsspec_xrootd/xrootd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,86 +1,77 @@
 from __future__ import annotations
 
 import asyncio
 import io
 import os.path
+import time
 import warnings
+import weakref
 from collections import defaultdict
+from dataclasses import dataclass
 from enum import IntEnum
-from functools import partial
-from typing import Any, Callable, Iterable
+from typing import Any, Callable, Coroutine, Iterable, TypeVar
 
-from fsspec.asyn import (  # type: ignore[import-not-found]
-    AsyncFileSystem,
-    _run_coros_in_chunks,
-    sync_wrapper,
-)
-from fsspec.spec import AbstractBufferedFile  # type: ignore[import-not-found]
-from XRootD import client  # type: ignore[import-not-found]
-from XRootD.client.flags import (  # type: ignore[import-not-found]
+from fsspec.asyn import AsyncFileSystem, _run_coros_in_chunks, sync, sync_wrapper
+from fsspec.exceptions import FSTimeoutError
+from fsspec.spec import AbstractBufferedFile
+from XRootD import client
+from XRootD.client.flags import (
     DirListFlags,
     MkDirFlags,
     OpenFlags,
     QueryCode,
     StatInfoFlags,
 )
-from XRootD.client.responses import (  # type: ignore[import-not-found]
-    HostList,
-    XRootDStatus,
-)
+from XRootD.client.responses import HostList, XRootDStatus
 
 
 class ErrorCodes(IntEnum):
     INVALID_PATH = 400
 
 
-def _handle(
-    future: asyncio.Future[tuple[XRootDStatus, Any]],
-    status: XRootDStatus,
-    content: Any,
-    servers: HostList,
-) -> None:
-    """Sets result of _async_wrap() future.
-
-    Parameters
-    ----------
-    future: asyncio future, created in _async_wrap()
-    status: XRootDStatus, pyxrootd response object
-    content: any, whatever was returned from pyxrootd function
-    servers: Hostlist, iterable list of host info (currently unused)
-
-    Returns
-    -------
-    Sets the future result.
-    """
-    if future.cancelled():
-        return
-    try:
-        future.get_loop().call_soon_threadsafe(future.set_result, (status, content))
-    except Exception as exc:
-        future.get_loop().call_soon_threadsafe(future.set_exception, exc)
+T = TypeVar("T")
+# TODO: Protocol typing when kwargs is supported
 
 
-async def _async_wrap(func: Callable[..., Any], *args: Any) -> Any:
-    """Wraps pyxrootd functions to run asynchronously. Returns future to be awiated.
+def _async_wrap(
+    func: Callable[..., XRootDStatus | tuple[XRootDStatus, T]]
+) -> Callable[..., Coroutine[Any, Any, tuple[XRootDStatus, T]]]:
+    """Wraps pyxrootd functions to run asynchronously. Returns an async callable
 
     Parameters
     ----------
-    func: pyxrootd function, needs to have a callback option
-    args: non-keyworded arguments for pyxrootd function
+    func: XRootD function that implements, needs to have a callback option
 
     Returns
     -------
-    An asyncio future. Result is set when _handle() is called back.
+    A function with the same signature as func, but with an implicit `callback` argument
     """
-    future = asyncio.get_running_loop().create_future()
-    status = func(*args, callback=partial(_handle, future))
-    if not status.ok:
-        raise OSError(status.message.strip())
-    return await future
+    future: asyncio.Future[tuple[XRootDStatus, T]] = (
+        asyncio.get_running_loop().create_future()
+    )
+
+    def callback(status: XRootDStatus, content: T, servers: HostList) -> None:
+        if future.cancelled():
+            return
+        loop = future.get_loop()
+        try:
+            loop.call_soon_threadsafe(future.set_result, (status, content))
+        except Exception as exc:
+            loop.call_soon_threadsafe(future.set_exception, exc)
+
+    async def wrapped(*args: Any, **kwargs: Any) -> tuple[XRootDStatus, T]:
+        submit_status: XRootDStatus = func(*args, **kwargs, callback=callback)
+        if not submit_status.ok:
+            raise OSError(
+                f"Failed to submit {func!r} request: {submit_status.message.strip()}"
+            )
+        return await future
+
+    return wrapped
 
 
 def _chunks_to_vectors(
     file_ranges: list[tuple[int, int]],
     max_num_chunks: int,
     max_chunk_size: int,
 ) -> list[list[tuple[int, int]]]:
@@ -140,27 +131,113 @@
         chunk_data = b""
         while len(chunk_data) < chunk_length:
             chunk_data += next(subchunks).buffer
         deets.append(chunk_data)
     return deets
 
 
+@dataclass
+class _CacheItem:
+    accessed: float
+    handle: client.File
+
+
+class ReadonlyFileHandleCache:
+    def __init__(self, loop: Any, max_items: int | None, ttl: int):
+        self.loop = loop
+        self._max_items = max_items
+        self._ttl = int(ttl)
+        self._cache: dict[str, _CacheItem] = {}
+        sync(loop, self._start_pruner)
+        weakref.finalize(self, self._close_all, loop, self._cache)
+
+    @staticmethod
+    def _close_all(loop: Any, cache: dict[str, _CacheItem]) -> None:
+        if loop is not None and loop.is_running():
+
+            async def closure() -> None:
+                await asyncio.gather(
+                    *(_async_wrap(item.handle.close)() for item in cache.values())
+                )
+
+            try:
+                sync(loop, closure, timeout=0.5)
+            except (TimeoutError, FSTimeoutError, NotImplementedError):
+                pass
+        else:
+            # fire and forget
+            for item in cache.values():
+                item.handle.close(callback=lambda *args: None)
+        cache.clear()
+
+    def close_all(self) -> None:
+        self._close_all(self.loop, self._cache)
+
+    async def _close(self, url: str, timeout: int) -> None:
+        item = self._cache.pop(url, None)
+        if item:
+            status, _ = await _async_wrap(item.handle.close)(timeout=timeout)
+            if not status.ok:
+                raise OSError(f"Failed to close file: {status.message}")
+
+    close = sync_wrapper(_close)
+
+    async def _start_pruner(self) -> None:
+        self._prune_task = asyncio.create_task(self._pruner())
+
+    async def _pruner(self) -> None:
+        while True:
+            await self._prune_cache(self._ttl // 2)
+            await asyncio.sleep(self._ttl)
+
+    async def _prune_cache(self, timeout: int) -> None:
+        now = time.monotonic()
+        oldest_keys = sorted((item.accessed, key) for key, item in self._cache.items())
+        to_close = []
+        if self._max_items:
+            to_close += oldest_keys[: -self._max_items]
+            oldest_keys = oldest_keys[-self._max_items :]
+        for last_access, key in oldest_keys:
+            if now - last_access > self._ttl:
+                to_close.append((last_access, key))
+        await asyncio.gather(*(self._close(key, timeout) for _, key in to_close))
+
+    async def _open(self, url: str, timeout: int) -> Any:  # client.File
+        if url in self._cache:
+            item = self._cache[url]
+            item.accessed = time.monotonic()
+            return item.handle
+        handle = client.File()
+        status, _ = await _async_wrap(handle.open)(
+            url,
+            OpenFlags.READ,
+            timeout=timeout,
+        )
+        if not status.ok:
+            raise OSError(f"Failed to open file: {status.message}")
+        self._cache[url] = _CacheItem(accessed=time.monotonic(), handle=handle)
+        await self._prune_cache(timeout)
+        return handle
+
+
 class XRootDFileSystem(AsyncFileSystem):  # type: ignore[misc]
     protocol = "root"
     root_marker = "/"
     default_timeout = 60
     async_impl = True
+    default_max_num_chunks = 1024
+    default_max_chunk_size = 2097136
 
     _dataserver_info_cache: dict[str, Any] = defaultdict(dict)
 
     def __init__(
         self,
         hostid: str,
         asynchronous: bool = False,
-        loop: Any = None,
+        loop: asyncio.AbstractEventLoop | None = None,
         **storage_options: Any,
     ) -> None:
         """
         Direct construction of XRootDFileSystem
 
         Parameters
         ----------
@@ -176,23 +253,32 @@
         self.timeout = storage_options.get("timeout", XRootDFileSystem.default_timeout)
         self.hostid = hostid
         self._myclient = client.FileSystem("root://" + hostid)
         if not self._myclient.url.is_valid():
             raise ValueError(f"Invalid hostid: {hostid!r}")
         storage_options.setdefault("listing_expiry_time", 0)
         self.storage_options = storage_options
+        self._readonly_filehandle_cache = ReadonlyFileHandleCache(
+            self.loop,
+            max_items=storage_options.get("filehandle_cache_size", 256),
+            ttl=storage_options.get("filehandle_cache_ttl", 30),
+        )
 
     def invalidate_cache(self, path: str | None = None) -> None:
         if path is None:
             self.dircache.clear()
+            self._readonly_filehandle_cache.close_all()
         else:
             try:
                 del self.dircache[path]
             except KeyError:
                 pass
+            self._readonly_filehandle_cache.close(
+                self.unstrip_protocol(path), self.timeout
+            )
 
     @staticmethod
     def _get_kwargs_from_urls(u: str) -> dict[Any, Any]:
         url = client.URL(u)
         # The hostid encapsulates user,pass,host,port in one string
         return {"hostid": url.hostid}
 
@@ -205,36 +291,41 @@
             return path.rstrip("/") or cls.root_marker
         elif isinstance(path, list):
             return [cls._strip_protocol(item) for item in path]
         else:
             raise ValueError("Strip protocol not given string or list")
 
     def unstrip_protocol(self, name: str) -> str:
-        return f"{self.protocol}://{self.hostid}/{name}"
+        prefix = f"{self.protocol}://{self.hostid}/"
+        if name.startswith(prefix):
+            return name
+        return prefix + name
 
     async def _mkdir(
         self, path: str, create_parents: bool = True, **kwargs: Any
     ) -> None:
         if create_parents:
-            status, n = await _async_wrap(
-                self._myclient.mkdir, path, MkDirFlags.MAKEPATH, self.timeout
+            status, _ = await _async_wrap(self._myclient.mkdir)(
+                path, flags=MkDirFlags.MAKEPATH, timeout=self.timeout
             )
         else:
-            status, n = await _async_wrap(self._myclient.mkdir, path, self.timeout)
+            status, _ = await _async_wrap(self._myclient.mkdir)(
+                path, timeout=self.timeout
+            )
         if not status.ok:
             raise OSError(f"Directory not made properly: {status.message}")
 
     async def _makedirs(self, path: str, exist_ok: bool = False) -> None:
         if not exist_ok:
             if await self._exists(path):
                 raise OSError(
                     "Location already exists and exist_ok arg was set to false"
                 )
-        status, n = await _async_wrap(
-            self._myclient.mkdir, path, MkDirFlags.MAKEPATH, self.timeout
+        status, _ = await _async_wrap(self._myclient.mkdir)(
+            path, MkDirFlags.MAKEPATH, timeout=self.timeout
         )
         if not status.ok and not (status.code == ErrorCodes.INVALID_PATH and exist_ok):
             raise OSError(f"Directory not made properly: {status.message}")
 
     async def _rm(
         self,
         path: str,
@@ -249,56 +340,55 @@
         return await _run_coros_in_chunks(
             [self._rm_file(p, **kwargs) for p in reversed(path)],
             batch_size=batch_size,
             nofiles=True,
         )
 
     async def _rmdir(self, path: str) -> None:
-        status, n = await _async_wrap(self._myclient.rmdir, path, self.timeout)
+        status, _ = await _async_wrap(self._myclient.rmdir)(path, self.timeout)
         if not status.ok:
             raise OSError(f"Directory not removed properly: {status.message}")
 
     rmdir = sync_wrapper(_rmdir)
 
     async def _rm_file(self, path: str, **kwargs: Any) -> None:
-        status, n = await _async_wrap(self._myclient.rm, path, self.timeout)
+        status, _ = await _async_wrap(self._myclient.rm)(path, self.timeout)
         if not status.ok:
             raise OSError(f"File not removed properly: {status.message}")
 
     async def _touch(self, path: str, truncate: bool = False, **kwargs: Any) -> None:
         if truncate or not await self._exists(path):
-            status, _ = await _async_wrap(
-                self._myclient.truncate, path, 0, self.timeout
+            status, _ = await _async_wrap(self._myclient.truncate)(
+                path, size=0, timeout=self.timeout
             )
             if not status.ok:
                 raise OSError(f"File not touched properly: {status.message}")
         else:
             len = await self._info(path)
-            status, _ = await _async_wrap(
-                self._myclient.truncate,
+            status, _ = await _async_wrap(self._myclient.truncate)(
                 path,
-                len.get("size"),
-                self.timeout,
+                size=len.get("size"),
+                timeout=self.timeout,
             )
             if not status.ok:
                 raise OSError(f"File not touched properly: {status.message}")
 
     touch = sync_wrapper(_touch)
 
     async def _modified(self, path: str) -> Any:
-        status, statInfo = await _async_wrap(self._myclient.stat, path, self.timeout)
+        status, statInfo = await _async_wrap(self._myclient.stat)(path, self.timeout)  # type: ignore[var-annotated]
         return statInfo.modtime
 
     modified = sync_wrapper(_modified)
 
     async def _exists(self, path: str, **kwargs: Any) -> bool:
         if path in self.dircache:
             return True
         else:
-            status, _ = await _async_wrap(self._myclient.stat, path, self.timeout)
+            status, _ = await _async_wrap(self._myclient.stat)(path, self.timeout)
             if status.code == ErrorCodes.INVALID_PATH:
                 return False
             elif not status.ok:
                 raise OSError(f"status check failed with message: {status.message}")
             return True
 
     async def _info(self, path: str, **kwargs: Any) -> dict[str, Any]:
@@ -310,15 +400,15 @@
                     return {
                         "name": path,
                         "size": item["size"],
                         "type": item["type"],
                     }
             raise OSError("_ls_from_cache() failed to function")
         else:
-            status, deet = await _async_wrap(self._myclient.stat, path, self.timeout)
+            status, deet = await _async_wrap(self._myclient.stat)(path, self.timeout)
             if not status.ok:
                 raise OSError(f"File stat request failed: {status.message}")
             if deet.flags & StatInfoFlags.IS_DIR:
                 ret = {
                     "name": path,
                     "size": deet.size,
                     "type": "directory",
@@ -344,16 +434,16 @@
                 listing = self._ls_from_cache(path)
                 return listing
             else:
                 return [
                     os.path.basename(item["name"]) for item in self._ls_from_cache(path)
                 ]
         else:
-            status, deets = await _async_wrap(
-                self._myclient.dirlist, path, DirListFlags.STAT, self.timeout
+            status, deets = await _async_wrap(self._myclient.dirlist)(  # type: ignore[var-annotated]
+                path, DirListFlags.STAT, self.timeout
             )
             if not status.ok:
                 raise OSError(
                     f"Server failed to provide directory info: {status.message}"
                 )
             for item in deets:
                 if item.statinfo.flags & StatInfoFlags.IS_DIR:
@@ -382,106 +472,101 @@
                     )
             self.dircache[path] = listing
             if detail:
                 return listing
             else:
                 return [os.path.basename(item["name"].rstrip("/")) for item in listing]
 
-    async def _cat_file(self, path: str, start: int, end: int, **kwargs: Any) -> Any:
-        _myFile = client.File()
-        try:
-            status, _n = await _async_wrap(
-                _myFile.open,
-                self.unstrip_protocol(path),
-                OpenFlags.READ,
-                self.timeout,
-            )
-            if not status.ok:
-                raise OSError(f"File failed to read: {status.message}")
-            status, data = await _async_wrap(
-                _myFile.read,
-                start,
-                end - start,
-                self.timeout,
-            )
-            if not status.ok:
-                raise OSError(f"Bytes failed to read from open file: {status.message}")
-            return data
-        finally:
-            status, _n = await _async_wrap(
-                _myFile.close,
-                self.timeout,
-            )
+    async def _cat_file(
+        self, path: str, start: int | None, end: int | None, **kwargs: Any
+    ) -> Any:
+        _myFile = await self._readonly_filehandle_cache._open(
+            self.unstrip_protocol(path),
+            self.timeout,
+        )
+        n_bytes = end
+        if start is not None and end is not None:
+            n_bytes = end - start
+
+        status, data = await _async_wrap(_myFile.read)(  # type: ignore[var-annotated]
+            start or 0,
+            n_bytes or 0,
+            self.timeout,
+        )
+        if not status.ok:
+            raise OSError(f"Bytes failed to read from open file: {status.message}")
+        return data
 
     async def _get_file(
         self, rpath: str, lpath: str, chunk_size: int = 262_144, **kwargs: Any
     ) -> None:
         # Open the remote file for reading
-        remote_file = client.File()
-
-        try:
-            status, _n = await _async_wrap(
-                remote_file.open,
-                self.unstrip_protocol(rpath),
-                OpenFlags.READ,
-                self.timeout,
-            )
-            if not status.ok:
-                raise OSError(f"Remote file failed to open: {status.message}")
-
-            with open(lpath, "wb") as local_file:
-                start: int = 0
-                while True:
-                    # Read a chunk of content from the remote file
-                    status, chunk = await _async_wrap(
-                        remote_file.read, start, chunk_size, self.timeout
-                    )
-                    start += chunk_size
+        remote_file = await self._readonly_filehandle_cache._open(
+            self.unstrip_protocol(rpath),
+            self.timeout,
+        )
 
-                    if not status.ok:
-                        raise OSError(f"Remote file failed to read: {status.message}")
+        with open(lpath, "wb") as local_file:
+            start: int = 0
+            while True:
+                # Read a chunk of content from the remote file
+                status, chunk = await _async_wrap(remote_file.read)(  # type: ignore[var-annotated]
+                    start, chunk_size, self.timeout
+                )
+                start += chunk_size
 
-                    # Break if there is no more content
-                    if not chunk:
-                        break
+                if not status.ok:
+                    raise OSError(f"Remote file failed to read: {status.message}")
 
-                    # Write the chunk to the local file
-                    local_file.write(chunk)
+                # Break if there is no more content
+                if not chunk:
+                    break
 
-        finally:
-            # Close the remote file
-            await _async_wrap(remote_file.close, self.timeout)
+                # Write the chunk to the local file
+                local_file.write(chunk)
 
-    async def _get_max_chunk_info(self, file: Any) -> tuple[int, int]:
+    @classmethod
+    async def _get_max_chunk_info(cls, file: Any) -> tuple[int, int]:
         """Queries the XRootD server for info required for pyxrootd vector_read() function.
         Queries for maximum number of chunks and the maximum chunk size allowed by the server.
 
         Parameters
         ----------
         file: xrootd client.File() object
 
         Returns
         -------
         Tuple of max chunk size and max number of chunks. Both ints.
         """
         data_server = file.get_property("DataServer")
-        if data_server not in XRootDFileSystem._dataserver_info_cache:
-            status, result = await _async_wrap(
-                self._myclient.query, QueryCode.CONFIG, "readv_iov_max readv_ior_max"
+        if data_server == "":
+            return cls.default_max_num_chunks, cls.default_max_chunk_size
+        # Normalize to URL
+        data_server = client.URL(data_server)
+        data_server = f"{data_server.protocol}://{data_server.hostid}/"
+        if data_server not in cls._dataserver_info_cache:
+            fs = client.FileSystem(data_server)
+            status, result = await _async_wrap(fs.query)(  # type: ignore[var-annotated]
+                QueryCode.CONFIG, "readv_iov_max readv_ior_max"
             )
             if not status.ok:
                 raise OSError(
                     f"Server query for vector read info failed: {status.message}"
                 )
-            max_num_chunks, max_chunk_size = map(int, result.split(b"\n", 1))
-            XRootDFileSystem._dataserver_info_cache[data_server] = {
-                "max_num_chunks": int(max_num_chunks),
-                "max_chunk_size": int(max_chunk_size),
+            try:
+                max_num_chunks, max_chunk_size = map(int, result.split(b"\n", 1))
+            except ValueError:
+                raise OSError(
+                    f"Server query for vector read info failed: could not parse {result!r}"
+                ) from None
+            cls._dataserver_info_cache[data_server] = {
+                "max_num_chunks": max_num_chunks,
+                "max_chunk_size": max_chunk_size,
             }
-        info = XRootDFileSystem._dataserver_info_cache[data_server]
+        info = cls._dataserver_info_cache[data_server]
         return (info["max_num_chunks"], info["max_chunk_size"])
 
     async def _cat_vector_read(
         self,
         path: str,
         chunks: list[tuple[int, int]],
         batch_size: int,
@@ -495,47 +580,32 @@
         batch_size: int, upper limit on simultainious vector reads
 
         Returns
         -------
         Tuple containing path name and a list of returned
         bytes in the same order as requested.
         """
-        try:
-            _myFile = client.File()
-            status, _n = await _async_wrap(
-                _myFile.open,
-                self.protocol + "://" + self.storage_options["hostid"] + "/" + path,
-                OpenFlags.READ,
-                self.timeout,
-            )
-            if not status.ok:
-                raise OSError(f"File did not open properly: {status.message}")
+        _myFile = await self._readonly_filehandle_cache._open(
+            self.unstrip_protocol(path),
+            self.timeout,
+        )
 
-            max_num_chunks, max_chunk_size = await self._get_max_chunk_info(_myFile)
-            vectors = _chunks_to_vectors(chunks, max_num_chunks, max_chunk_size)
+        max_num_chunks, max_chunk_size = await self._get_max_chunk_info(_myFile)
+        vectors = _chunks_to_vectors(chunks, max_num_chunks, max_chunk_size)
 
-            coros = [_async_wrap(_myFile.vector_read, v, self.timeout) for v in vectors]
+        coros = [_async_wrap(_myFile.vector_read)(v, self.timeout) for v in vectors]  # type: ignore[var-annotated]
 
-            results = await _run_coros_in_chunks(
-                coros, batch_size=batch_size, nofiles=True
-            )
-            result_bufs = []
-            for status, buffers in results:
-                if not status.ok:
-                    raise OSError(
-                        f"File did not vector_read properly: {status.message}"
-                    )
-                result_bufs.append(buffers)
-            deets = _vectors_to_chunks(chunks, result_bufs)
+        results = await _run_coros_in_chunks(coros, batch_size=batch_size, nofiles=True)
+        result_bufs = []
+        for status, buffers in results:
+            if not status.ok:
+                raise OSError(f"File did not vector_read properly: {status.message}")
+            result_bufs.append(buffers)
+        deets = _vectors_to_chunks(chunks, result_bufs)
 
-        finally:
-            status, _n = await _async_wrap(
-                _myFile.close,
-                self.timeout,
-            )
         return (path, deets)
 
     async def _cat_ranges(
         self,
         paths: list[str],
         starts: list[int],
         ends: list[int],
@@ -638,18 +708,16 @@
                 mode=mode,
                 block_size=block_size,
                 autocommit=ac,
                 cache_options=cache_options,
                 **kwargs,
             )
             if compression is not None:
-                from fsspec.compression import compr  # type: ignore[import-not-found]
-                from fsspec.core import (  # type: ignore[import-not-found]
-                    get_compression,
-                )
+                from fsspec.compression import compr
+                from fsspec.core import get_compression
 
                 compression = get_compression(path, compression)
                 compress = compr[compression]
                 f = compress(f, mode=mode[0])
 
             if not ac and "r" not in mode:
                 self.transaction.files.append(f)
@@ -684,21 +752,22 @@
             self.mode = OpenFlags.READ
         else:
             raise NotImplementedError
 
         if not isinstance(path, str):
             raise ValueError(f"Path expected to be string, path: {path}")
 
+        # Ensure any read-only handle is closed
+        fs.invalidate_cache(path)
         self._myFile = client.File()
-        status, _n = self._myFile.open(
-            fs.protocol + "://" + fs.storage_options["hostid"] + "/" + path,
+        status, _ = self._myFile.open(
+            fs.unstrip_protocol(path),
             self.mode,
             timeout=self.timeout,
         )
-
         if not status.ok:
             raise OSError(f"File did not open properly: {status.message}")
 
         self.metaOffset = 0
         if "a" in mode:
             _stats, _deets = self._myFile.stat(timeout=self.timeout)
             self.metaOffset = _deets.size
```

### Comparing `fsspec_xrootd-0.2.4/src/fsspec_xrootd.egg-info/PKG-INFO` & `fsspec_xrootd-0.3.0/src/fsspec_xrootd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fsspec-xrootd
-Version: 0.2.4
+Name: fsspec_xrootd
+Version: 0.3.0
 Summary: xrootd implementation for fsspec
 Home-page: https://github.com/CoffeaTeam/fsspec-xrootd
 Author: Scott Demarest
 Author-email: rockets1194@gmail.com
 Maintainer: CoffeaTeam admins
 Maintainer-email: rockets1194@gmail.com
 License: BSD-3-Clause
@@ -48,15 +48,15 @@
 ```bash
 pip install fsspec-xrootd
 ```
 
 ## Purpose
 
 To allow fsspec to use XRootD accessible storage systems. Install fsspec-xrootd
-alongside fsspec and have easy access to files stored on XRootD serevrs. Once
+alongside fsspec and have easy access to files stored on XRootD servers. Once
 installed, fsspec will be able to work with urls with the 'root' protocol. Only
 tested with Linux at this time.
 
 ## Documentation
 
 Please refer to [RTD](https://coffeateam.github.io/fsspec-xrootd/)
```

### Comparing `fsspec_xrootd-0.2.4/src/fsspec_xrootd.egg-info/SOURCES.txt` & `fsspec_xrootd-0.3.0/src/fsspec_xrootd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fsspec_xrootd-0.2.4/tests/test_basicio.py` & `fsspec_xrootd-0.3.0/tests/test_basicio.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,63 @@
 """Test basic IO against a xrootd server fixture"""
+
 from __future__ import annotations
 
+import asyncio
 import os
 import shutil
+import socket
 import subprocess
 import time
 
 import fsspec
 import pytest
 
 from fsspec_xrootd.xrootd import (
     XRootDFileSystem,
     _chunks_to_vectors,
     _vectors_to_chunks,
 )
 
+XROOTD_PORT = 1094
 TESTDATA1 = "apple\nbanana\norange\ngrape"
 TESTDATA2 = "red\ngreen\nyellow\nblue"
 sleep_time = 0.2
 expiry_time = 0.1
 
 
+def require_port_availability(port: int) -> bool:
+    """Raise an exception if the given port is already in use."""
+    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+        if s.connect_ex(("localhost", port)) == 0:
+            raise RuntimeError(f"This test requires port {port} to be available")
+
+
 @pytest.fixture(scope="module")
 def localserver(tmpdir_factory):
+    require_port_availability(XROOTD_PORT)
+
     srvdir = tmpdir_factory.mktemp("srv")
     tempPath = os.path.join(srvdir, "Folder")
     os.mkdir(tempPath)
     xrdexe = shutil.which("xrootd")
-    proc = subprocess.Popen([xrdexe, srvdir])
+    proc = subprocess.Popen([xrdexe, "-p", str(XROOTD_PORT), srvdir])
     time.sleep(2)  # give it some startup
     yield "root://localhost/" + str(tempPath), tempPath
     proc.terminate()
     proc.wait(timeout=10)
 
 
 @pytest.fixture()
 def clear_server(localserver):
     remoteurl, localpath = localserver
+    fs, _, _ = fsspec.get_fs_token_paths(remoteurl)
+    # The open file handles on client side imply an open file handle on the server,
+    # so removing the directory doesn't actually work until the client closes its handles!
+    fs.invalidate_cache()
     shutil.rmtree(localpath)
     os.mkdir(localpath)
     yield
 
 
 def test_ping(localserver, clear_server):
     remoteurl, localpath = localserver
@@ -153,14 +170,25 @@
     with fsspec.open(remoteurl + "/testfile.txt", "wt") as f:
         f.write(TESTDATA1)
         f.flush()
     with open(localpath + "/testfile.txt") as f:
         assert f.read() == TESTDATA1
 
 
+@pytest.mark.parametrize("start, end", [(None, None), (None, 10), (1, None), (1, 10)])
+def test_read_bytes_fsspec(localserver, clear_server, start, end):
+    remoteurl, localpath = localserver
+    with open(localpath + "/testfile.txt", "w") as fout:
+        fout.write(TESTDATA1)
+
+    fs, _ = fsspec.core.url_to_fs(remoteurl)
+    data = fs.read_bytes(localpath + "/testfile.txt", start=start, end=end)
+    assert data == TESTDATA1.encode("utf-8")[start:end]
+
+
 def test_append_fsspec(localserver, clear_server):
     remoteurl, localpath = localserver
     with open(localpath + "/testfile.txt", "w") as fout:
         fout.write(TESTDATA1)
     with fsspec.open(remoteurl + "/testfile.txt", "at") as f:
         f.write(TESTDATA2)
         f.flush()
@@ -440,7 +468,38 @@
         contents = f.read()
         assert contents == TESTDATA1.encode("utf-8")
 
     assert len(os.listdir(cache_directory)) == 1
     with open(cache_directory / os.listdir(cache_directory)[0], "rb") as f:
         contents = f.read()
         assert contents == TESTDATA1.encode("utf-8")
+
+
+def test_close_while_reading(localserver, clear_server):
+    remoteurl, localpath = localserver
+    data = TESTDATA1 * int(1e8 / len(TESTDATA1))
+    with open(localpath + "/testfile.txt", "w") as fout:
+        fout.write(data)
+
+    fs, _, (path,) = fsspec.get_fs_token_paths(remoteurl + "/testfile.txt")
+
+    async def reader():
+        tic = time.monotonic()
+        await fs._cat_file(path, start=0, end=None)
+        toc = time.monotonic()
+        return tic, toc
+
+    async def closer():
+        await asyncio.sleep(0.001)
+        tic = time.monotonic()
+        await fs._readonly_filehandle_cache._close(path, 1)
+        toc = time.monotonic()
+        return tic, toc
+
+    async def run():
+        (read_start, read_stop), (close_start, close_stop) = await asyncio.gather(
+            reader(), closer()
+        )
+        assert read_start < close_start < read_stop
+        assert read_start < close_stop < read_stop
+
+    asyncio.run(run())
```


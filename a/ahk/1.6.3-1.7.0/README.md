# Comparing `tmp/ahk-1.6.3.tar.gz` & `tmp/ahk-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahk-1.6.3.tar", last modified: Fri Apr 19 22:39:07 2024, max compression
+gzip compressed data, was "ahk-1.7.0.tar", last modified: Sun Apr 21 04:01:09 2024, max compression
```

## Comparing `ahk-1.6.3.tar` & `ahk-1.7.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:39:07.955873 ahk-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-19 22:39:00.000000 ahk-1.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 22:39:00.000000 ahk-1.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28013 2024-04-19 22:39:07.955873 ahk-1.6.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:39:07.951873 ahk-1.6.3/ahk/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:39:07.955873 ahk-1.6.3/ahk/_async/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   207901 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/_async/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    49798 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/_async/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    30508 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/_async/window.py
--rw-r--r--   0 runner    (1001) docker     (127)   171011 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17089 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/_hotkey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:39:07.955873 ahk-1.6.3/ahk/_sync/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   201181 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/_sync/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    44850 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/_sync/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    27717 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/_sync/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/directives.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/message.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:39:07.955873 ahk-1.6.3/ahk/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    80096 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/templates/daemon-v2.ahk
--rw-r--r--   0 runner    (1001) docker     (127)    80517 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/templates/daemon.ahk
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/templates/hotkeys-v2.ahk
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-19 22:39:00.000000 ahk-1.6.3/ahk/templates/hotkeys.ahk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:39:07.955873 ahk-1.6.3/ahk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28013 2024-04-19 22:39:07.000000 ahk-1.6.3/ahk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-19 22:39:07.000000 ahk-1.6.3/ahk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 22:39:07.000000 ahk-1.6.3/ahk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-19 22:39:07.000000 ahk-1.6.3/ahk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 22:39:07.000000 ahk-1.6.3/ahk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-19 22:39:00.000000 ahk-1.6.3/buildunasync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:39:07.955873 ahk-1.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    26719 2024-04-19 22:39:00.000000 ahk-1.6.3/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-19 22:39:00.000000 ahk-1.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-19 22:39:07.955873 ahk-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 22:39:00.000000 ahk-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:01:09.800737 ahk-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-21 04:01:00.000000 ahk-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-21 04:01:00.000000 ahk-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28092 2024-04-21 04:01:09.800737 ahk-1.7.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:01:09.796737 ahk-1.7.0/ahk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:01:09.796737 ahk-1.7.0/ahk/_async/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   206741 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/_async/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47611 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30507 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/_async/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)   171011 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17089 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/_hotkey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:01:09.796737 ahk-1.7.0/ahk/_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   199988 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/_sync/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42661 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/_sync/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27714 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/_sync/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/directives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:01:09.796737 ahk-1.7.0/ahk/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    80096 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/templates/daemon-v2.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)    80517 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/templates/daemon.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/templates/hotkeys-v2.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-21 04:01:00.000000 ahk-1.7.0/ahk/templates/hotkeys.ahk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:01:09.800737 ahk-1.7.0/ahk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28092 2024-04-21 04:01:09.000000 ahk-1.7.0/ahk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-21 04:01:09.000000 ahk-1.7.0/ahk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 04:01:09.000000 ahk-1.7.0/ahk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-21 04:01:09.000000 ahk-1.7.0/ahk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-21 04:01:09.000000 ahk-1.7.0/ahk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-21 04:01:00.000000 ahk-1.7.0/buildunasync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:01:09.800737 ahk-1.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    26719 2024-04-21 04:01:00.000000 ahk-1.7.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-21 04:01:00.000000 ahk-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-21 04:01:09.800737 ahk-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 04:01:00.000000 ahk-1.7.0/setup.py
```

### Comparing `ahk-1.6.3/LICENSE` & `ahk-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ahk-1.6.3/PKG-INFO` & `ahk-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.6.3
+Version: 1.7.0
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://ahk.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/spyoungtech/
 Project-URL: Source, https://github.com/spyoungtech/ahk
@@ -17,14 +17,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_extensions; python_version < "3.11"
 Requires-Dist: jinja2>=3.0
 Provides-Extra: binary
 Requires-Dist: ahk-binary==2023.9.0; extra == "binary"
```

### Comparing `ahk-1.6.3/ahk/_async/engine.py` & `ahk-1.7.0/ahk/_async/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,75 +48,33 @@
 from ..keys import Key
 from .transport import AsyncDaemonProcessTransport
 from .transport import AsyncFutureResult
 from .transport import AsyncTransport
 from .window import AsyncControl
 from .window import AsyncWindow
 
-# from .window import AsyncGui
-from ahk.message import Position
-
+from ahk._types import (
+    Position,
+    CoordModeTargets,
+    CoordModeRelativeTo,
+    TitleMatchMode,
+    _BUTTONS,
+    MouseButton,
+    SendMode,
+    Coordinates,
+)
 
 async_sleep = asyncio.sleep  # unasync: remove
 sleep = time.sleep
 
 AsyncFilterFunc: TypeAlias = Callable[[AsyncWindow], Awaitable[bool]]  # unasync: remove
 SyncFilterFunc: TypeAlias = Callable[[AsyncWindow], bool]
 
-CoordModeTargets: TypeAlias = Union[
-    Literal['ToolTip'], Literal['Pixel'], Literal['Mouse'], Literal['Caret'], Literal['Menu']
-]
-CoordModeRelativeTo: TypeAlias = Union[Literal['Screen', 'Relative', 'Window', 'Client', '']]
-
-CoordMode: TypeAlias = Union[CoordModeTargets, Tuple[CoordModeTargets, CoordModeRelativeTo]]
-
-MatchModes: TypeAlias = Literal[1, 2, 3, 'RegEx', '']
-MatchSpeeds: TypeAlias = Literal['Fast', 'Slow', '']
-
-TitleMatchMode: TypeAlias = Optional[
-    Union[MatchModes, MatchSpeeds, Tuple[Union[MatchModes, MatchSpeeds], Union[MatchSpeeds, MatchModes]]]
-]
-
-_BUTTONS: dict[Union[str, int], str] = {
-    1: 'L',
-    2: 'R',
-    3: 'M',
-    'left': 'L',
-    'right': 'R',
-    'middle': 'M',
-    'wheelup': 'WU',
-    'wheeldown': 'WD',
-    'wheelleft': 'WL',
-    'wheelright': 'WR',
-}
-
-MouseButton: TypeAlias = Union[
-    int,
-    Literal[
-        'L',
-        'R',
-        'M',
-        'left',
-        'right',
-        'middle',
-        'wheelup',
-        'WU',
-        'wheeldown',
-        'WD',
-        'wheelleft',
-        'WL',
-        'wheelright',
-        'WR',
-    ],
-]
-
-SendMode: TypeAlias = Literal['Event', 'Input', 'InputThenPlay', 'Play', '']
-
-AsyncPropertyReturnTupleIntInt: TypeAlias = Coroutine[None, None, Tuple[int, int]]  # unasync: remove
-SyncPropertyReturnTupleIntInt: TypeAlias = Tuple[int, int]
+AsyncPropertyReturnTupleIntInt: TypeAlias = Coroutine[None, None, Coordinates]  # unasync: remove
+SyncPropertyReturnTupleIntInt: TypeAlias = Coordinates
 
 AsyncPropertyReturnOptionalAsyncWindow: TypeAlias = Coroutine[None, None, Optional[AsyncWindow]]  # unasync: remove
 SyncPropertyReturnOptionalAsyncWindow: TypeAlias = Optional[AsyncWindow]
 
 _PROPERTY_DEPRECATION_WARNING_MESSAGE = 'Use of the {0} property is not recommended (in the async API only) and may be removed in a future version. Use the get_{0} method instead'
 
 
@@ -733,25 +691,25 @@
             detect_hidden_windows=detect_hidden_windows,
         )
         resp = await self._transport.function_call('AHKWindowList', args, engine=self, blocking=blocking)
         return resp
 
     # fmt: off
     @overload
-    async def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: Literal[True]) -> Tuple[int, int]: ...
+    async def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: Literal[True]) -> Coordinates: ...
     @overload
-    async def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: Literal[False]) -> AsyncFutureResult[Tuple[int, int]]: ...
+    async def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: Literal[False]) -> AsyncFutureResult[Coordinates]: ...
     @overload
-    async def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None) -> Tuple[int, int]: ...
+    async def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None) -> Coordinates: ...
     @overload
-    async def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: bool = True) -> Union[Tuple[int, int], AsyncFutureResult[Tuple[int, int]]]: ...
+    async def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: bool = True) -> Union[Coordinates, AsyncFutureResult[Coordinates]]: ...
     # fmt: on
     async def get_mouse_position(
         self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: bool = True
-    ) -> Union[Tuple[int, int], AsyncFutureResult[Tuple[int, int]]]:
+    ) -> Union[Coordinates, AsyncFutureResult[Coordinates]]:
         """
         Analog for `MouseGetPos <https://www.autohotkey.com/docs/commands/MouseGetPos.htm>`_
         """
         if coord_mode:
             args = [str(coord_mode)]
         else:
             args = []
@@ -2866,36 +2824,36 @@
             send_mode = ''
         args = [str(x), str(y), button, str(click_count), direction or '', r, coord_mode, str(send_mode)]
         resp = await self._transport.function_call('AHKClick', args, blocking=blocking)
         return resp
 
     # fmt: off
     @overload
-    async def image_search(self, image_path: str, upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0), lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None, *, color_variation: Optional[int] = None, coord_mode: Optional[CoordModeRelativeTo] = None, scale_height: Optional[int] = None, scale_width: Optional[int] = None, transparent: Optional[str] = None, icon: Optional[int] = None) -> Optional[Tuple[int, int]]: ...
+    async def image_search(self, image_path: str, upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0), lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None, *, color_variation: Optional[int] = None, coord_mode: Optional[CoordModeRelativeTo] = None, scale_height: Optional[int] = None, scale_width: Optional[int] = None, transparent: Optional[str] = None, icon: Optional[int] = None) -> Optional[Coordinates]: ...
     @overload
-    async def image_search(self, image_path: str, upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0), lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None, *, color_variation: Optional[int] = None, coord_mode: Optional[CoordModeRelativeTo] = None, scale_height: Optional[int] = None, scale_width: Optional[int] = None, transparent: Optional[str] = None, icon: Optional[int] = None, blocking: Literal[False]) -> AsyncFutureResult[Optional[Tuple[int, int]]]: ...
+    async def image_search(self, image_path: str, upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0), lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None, *, color_variation: Optional[int] = None, coord_mode: Optional[CoordModeRelativeTo] = None, scale_height: Optional[int] = None, scale_width: Optional[int] = None, transparent: Optional[str] = None, icon: Optional[int] = None, blocking: Literal[False]) -> AsyncFutureResult[Optional[Coordinates]]: ...
     @overload
-    async def image_search(self, image_path: str, upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0), lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None, *, color_variation: Optional[int] = None, coord_mode: Optional[CoordModeRelativeTo] = None, scale_height: Optional[int] = None, scale_width: Optional[int] = None, transparent: Optional[str] = None, icon: Optional[int] = None, blocking: Literal[True]) -> Optional[Tuple[int, int]]: ...
+    async def image_search(self, image_path: str, upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0), lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None, *, color_variation: Optional[int] = None, coord_mode: Optional[CoordModeRelativeTo] = None, scale_height: Optional[int] = None, scale_width: Optional[int] = None, transparent: Optional[str] = None, icon: Optional[int] = None, blocking: Literal[True]) -> Optional[Coordinates]: ...
     @overload
-    async def image_search(self, image_path: str, upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0), lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None, *, color_variation: Optional[int] = None, coord_mode: Optional[CoordModeRelativeTo] = None, scale_height: Optional[int] = None, scale_width: Optional[int] = None, transparent: Optional[str] = None, icon: Optional[int] = None, blocking: bool = True) -> Union[Tuple[int, int], None, AsyncFutureResult[Optional[Tuple[int, int]]]]: ...
+    async def image_search(self, image_path: str, upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0), lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None, *, color_variation: Optional[int] = None, coord_mode: Optional[CoordModeRelativeTo] = None, scale_height: Optional[int] = None, scale_width: Optional[int] = None, transparent: Optional[str] = None, icon: Optional[int] = None, blocking: bool = True) -> Union[Coordinates, None, AsyncFutureResult[Optional[Coordinates]]]: ...
     # fmt: on
     async def image_search(
         self,
         image_path: str,
         upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0),
         lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None,
         *,
         color_variation: Optional[int] = None,
         coord_mode: Optional[CoordModeRelativeTo] = None,
         scale_height: Optional[int] = None,
         scale_width: Optional[int] = None,
         transparent: Optional[str] = None,
         icon: Optional[int] = None,
         blocking: bool = True,
-    ) -> Union[Tuple[int, int], None, AsyncFutureResult[Optional[Tuple[int, int]]]]:
+    ) -> Union[Coordinates, None, AsyncFutureResult[Optional[Coordinates]]]:
         """
         Analog for `ImageSearch <https://www.autohotkey.com/docs/commands/ImageSearch.htm>`_
         """
 
         if scale_height and not scale_width:
             scale_width = -1
         elif scale_width and not scale_height:
@@ -3022,34 +2980,34 @@
         args.append(options)
 
         resp = await self._transport.function_call('AHKPixelGetColor', args, blocking=blocking)
         return resp
 
     # fmt: off
     @overload
-    async def pixel_search(self, search_region_start: Tuple[int, int], search_region_end: Tuple[int, int], color: Union[str, int], variation: int = 0, *, coord_mode: Optional[CoordModeRelativeTo] = None, fast: bool = True, rgb: bool = True) -> Optional[Tuple[int, int]]: ...
+    async def pixel_search(self, search_region_start: Tuple[int, int], search_region_end: Tuple[int, int], color: Union[str, int], variation: int = 0, *, coord_mode: Optional[CoordModeRelativeTo] = None, fast: bool = True, rgb: bool = True) -> Optional[Coordinates]: ...
     @overload
-    async def pixel_search(self, search_region_start: Tuple[int, int], search_region_end: Tuple[int, int], color: Union[str, int], variation: int = 0, *, coord_mode: Optional[CoordModeRelativeTo] = None, fast: bool = True, rgb: bool = True, blocking: Literal[True]) -> Optional[Tuple[int, int]]: ...
+    async def pixel_search(self, search_region_start: Tuple[int, int], search_region_end: Tuple[int, int], color: Union[str, int], variation: int = 0, *, coord_mode: Optional[CoordModeRelativeTo] = None, fast: bool = True, rgb: bool = True, blocking: Literal[True]) -> Optional[Coordinates]: ...
     @overload
-    async def pixel_search(self, search_region_start: Tuple[int, int], search_region_end: Tuple[int, int], color: Union[str, int], variation: int = 0, *, coord_mode: Optional[CoordModeRelativeTo] = None, fast: bool = True, rgb: bool = True, blocking: Literal[False]) -> AsyncFutureResult[Optional[Tuple[int, int]]]: ...
+    async def pixel_search(self, search_region_start: Tuple[int, int], search_region_end: Tuple[int, int], color: Union[str, int], variation: int = 0, *, coord_mode: Optional[CoordModeRelativeTo] = None, fast: bool = True, rgb: bool = True, blocking: Literal[False]) -> AsyncFutureResult[Optional[Coordinates]]: ...
     @overload
-    async def pixel_search(self, search_region_start: Tuple[int, int], search_region_end: Tuple[int, int], color: Union[str, int], variation: int = 0, *, coord_mode: Optional[CoordModeRelativeTo] = None, fast: bool = True, rgb: bool = True, blocking: bool = True) -> Union[Optional[Tuple[int, int]], AsyncFutureResult[Optional[Tuple[int, int]]]]: ...
+    async def pixel_search(self, search_region_start: Tuple[int, int], search_region_end: Tuple[int, int], color: Union[str, int], variation: int = 0, *, coord_mode: Optional[CoordModeRelativeTo] = None, fast: bool = True, rgb: bool = True, blocking: bool = True) -> Union[Optional[Coordinates], AsyncFutureResult[Optional[Coordinates]]]: ...
     # fmt: on
     async def pixel_search(
         self,
         search_region_start: Tuple[int, int],
         search_region_end: Tuple[int, int],
         color: Union[str, int],
         variation: int = 0,
         *,
         coord_mode: Optional[CoordModeRelativeTo] = None,
         fast: bool = True,
         rgb: bool = True,
         blocking: bool = True,
-    ) -> Union[Optional[Tuple[int, int]], AsyncFutureResult[Optional[Tuple[int, int]]]]:
+    ) -> Union[Optional[Coordinates], AsyncFutureResult[Optional[Coordinates]]]:
         """
         Analog for `PixelSearch <https://www.autohotkey.com/docs/commands/PixelSearch.htm>`_
         """
         x1, y1 = search_region_start
         x2, y2 = search_region_end
         args = [str(x1), str(y1), str(x2), str(y2), str(color), str(variation)]
         mode = ' '.join(word for word, val in zip(('Fast', 'RGB'), (fast, rgb)) if val)
```

### Comparing `ahk-1.6.3/ahk/_async/transport.py` & `ahk-1.7.0/ahk/_async/transport.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import subprocess
 import sys
 import tempfile
 import threading
 import warnings
 from abc import ABC
 from abc import abstractmethod
+from concurrent.futures import Future
+from concurrent.futures import ThreadPoolExecutor
 from io import BytesIO
 from typing import Any
 from typing import Callable
 from typing import Generic
 from typing import List
 from typing import Literal
 from typing import Optional
@@ -23,41 +25,43 @@
 from typing import runtime_checkable
 from typing import Tuple
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
+import jinja2
+
+from ahk._constants import DAEMON_SCRIPT_TEMPLATE as _DAEMON_SCRIPT_TEMPLATE
+from ahk._constants import DAEMON_SCRIPT_V2_TEMPLATE as _DAEMON_SCRIPT_V2_TEMPLATE
+from ahk._hotkey import Hotkey
+from ahk._hotkey import Hotstring
+from ahk._hotkey import ThreadedHotkeyTransport
+from ahk._types import Coordinates
+from ahk._types import FunctionName
+from ahk._types import Position
+from ahk._utils import _version_detection_script
+from ahk.directives import Directive
+from ahk.exceptions import AHKProtocolError
+from ahk.extensions import _resolve_includes
+from ahk.extensions import Extension
+from ahk.message import _message_registry
+from ahk.message import RequestMessage
+from ahk.message import ResponseMessage
+
+
 if TYPE_CHECKING:
     from ahk import AsyncControl
     from ahk import AsyncWindow
 
 if sys.version_info < (3, 10):
     from typing_extensions import TypeAlias, TypeGuard
 else:
     from typing import TypeAlias, TypeGuard
 
-import jinja2
-
-from ahk.extensions import Extension, _resolve_includes
-from ahk._hotkey import ThreadedHotkeyTransport, Hotkey, Hotstring
-from ahk.message import RequestMessage
-from ahk.message import ResponseMessage
-from ahk.message import Position
-from ahk.message import _message_registry
-from ahk._constants import (
-    DAEMON_SCRIPT_TEMPLATE as _DAEMON_SCRIPT_TEMPLATE,
-    DAEMON_SCRIPT_V2_TEMPLATE as _DAEMON_SCRIPT_V2_TEMPLATE,
-)
-from ahk._utils import _version_detection_script
-from ahk.directives import Directive
-from ahk.exceptions import AHKProtocolError
-
-from concurrent.futures import Future, ThreadPoolExecutor
-
 
 T_AsyncFuture = TypeVar('T_AsyncFuture')  # unasync: remove
 T_SyncFuture = TypeVar('T_SyncFuture')
 
 
 class AsyncFutureResult(Generic[T_AsyncFuture]):  # unasync: remove
     def __init__(self, task: asyncio.Task[T_AsyncFuture]):
@@ -76,123 +80,14 @@
 
 
 AsyncIOProcess: TypeAlias = asyncio.subprocess.Process  # unasync: remove
 
 SyncIOProcess: TypeAlias = 'subprocess.Popen[bytes]'
 
 
-FunctionName = Literal[
-    'AHKBlockInput',
-    'AHKClipWait',
-    'AHKControlClick',
-    'AHKControlGetPos',
-    'AHKControlGetText',
-    'AHKControlSend',
-    'AHKFileSelectFile',
-    'AHKFileSelectFolder',
-    'AHKGetClipboard',
-    'AHKGetClipboardAll',
-    'AHKGetCoordMode',
-    'AHKGetSendLevel',
-    'AHKGetSendMode',
-    'AHKGetTitleMatchMode',
-    'AHKGetTitleMatchSpeed',
-    'AHKGetVolume',
-    'AHKGuiNew',
-    'AHKImageSearch',
-    'AHKInputBox',
-    'AHKKeyState',
-    'AHKKeyWait',
-    'AHKMenuTrayIcon',
-    'AHKMenuTrayShow',
-    'AHKMenuTrayHide',
-    'AHKMenuTrayTip',
-    'AHKMsgBox',
-    'AHKMouseClickDrag',
-    'AHKMouseGetPos',
-    'AHKMouseMove',
-    'AHKPixelGetColor',
-    'AHKPixelSearch',
-    'AHKRegRead',
-    'AHKRegWrite',
-    'AHKRegDelete',
-    'AHKSend',
-    'AHKSendEvent',
-    'AHKSendInput',
-    'AHKSendPlay',
-    'AHKSendRaw',
-    'AHKSetClipboard',
-    'AHKSetClipboardAll',
-    'AHKSetCoordMode',
-    'AHKSetDetectHiddenWindows',
-    'AHKSetSendLevel',
-    'AHKSetSendMode',
-    'AHKSetTitleMatchMode',
-    'AHKSetVolume',
-    'AHKShowToolTip',
-    'AHKSoundBeep',
-    'AHKSoundGet',
-    'AHKSoundPlay',
-    'AHKSoundSet',
-    'AHKTrayTip',
-    'AHKWinActivate',
-    'AHKWinClose',
-    'AHKWinExist',
-    'AHKWinFromMouse',
-    'AHKWinGetControlList',
-    'AHKWinGetControlListHwnd',
-    'AHKWinGetCount',
-    'AHKWinGetExStyle',
-    'AHKWinGetID',
-    'AHKWinGetIDLast',
-    'AHKWinGetList',
-    'AHKWinGetMinMax',
-    'AHKWinGetPID',
-    'AHKWinGetPos',
-    'AHKWinGetProcessName',
-    'AHKWinGetProcessPath',
-    'AHKWinGetStyle',
-    'AHKWinGetText',
-    'AHKWinGetTitle',
-    'AHKWinGetTransColor',
-    'AHKWinGetTransparent',
-    'AHKWinHide',
-    'AHKWinIsActive',
-    'AHKWinIsAlwaysOnTop',
-    'AHKWinMove',
-    'AHKWinSetAlwaysOnTop',
-    'AHKWinSetBottom',
-    'AHKWinSetDisable',
-    'AHKWinSetEnable',
-    'AHKWinSetExStyle',
-    'AHKWinSetRedraw',
-    'AHKWinSetRegion',
-    'AHKWinSetStyle',
-    'AHKWinSetTitle',
-    'AHKWinSetTop',
-    'AHKWinSetTransColor',
-    'AHKWinSetTransparent',
-    'AHKWinShow',
-    'AHKWindowList',
-    'AHKWinWait',
-    'AHKWinWaitActive',
-    'AHKWinWaitClose',
-    'AHKWinWaitNotActive',
-    'AHKClick',
-    'AHKSetCapsLockState',
-    'SetKeyDelay',
-    'WinActivateBottom',
-    'AHKWinGetClass',
-    'AHKWinKill',
-    'AHKWinMaximize',
-    'AHKWinMinimize',
-    'AHKWinRestore',
-]
-
-
 @runtime_checkable
 class Killable(Protocol):
     def kill(self) -> None: ...
 
 
 def kill(proc: Killable) -> None:
     try:
@@ -200,15 +95,17 @@
     except:  # noqa
         pass
 
 
 def async_assert_send_nonblocking_type_correct(
     obj: Any,
 ) -> TypeGuard[
-    Future[Union[None, Tuple[int, int], int, str, bool, AsyncWindow, List[AsyncWindow], List[AsyncControl]]]
+    Future[
+        Union[None, Coordinates, Tuple[int, int], int, str, bool, AsyncWindow, List[AsyncWindow], List[AsyncControl]]
+    ]
 ]:
     return True
 
 
 class Communicable(Protocol):
     runargs: List[str]
 
@@ -403,21 +300,21 @@
     ) -> Union[str, AsyncFutureResult[str]]:
         return NotImplemented
 
     # fmt: off
     @overload
     async def function_call(self, function_name: Literal['AHKWinExist'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[bool, AsyncFutureResult[bool]]: ...
     @overload
-    async def function_call(self, function_name: Literal['AHKImageSearch'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[Tuple[int, int], None, AsyncFutureResult[Union[Tuple[int, int], None]]]: ...
+    async def function_call(self, function_name: Literal['AHKImageSearch'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[Coordinates, None, AsyncFutureResult[Union[Coordinates, None]]]: ...
     @overload
     async def function_call(self, function_name: Literal['AHKPixelGetColor'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[str, AsyncFutureResult[str]]: ...
     @overload
-    async def function_call(self, function_name: Literal['AHKPixelSearch'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[Optional[Tuple[int, int]], AsyncFutureResult[Optional[Tuple[int, int]]]]: ...
+    async def function_call(self, function_name: Literal['AHKPixelSearch'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[Optional[Coordinates], AsyncFutureResult[Optional[Coordinates]]]: ...
     @overload
-    async def function_call(self, function_name: Literal['AHKMouseGetPos'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[Tuple[int, int], AsyncFutureResult[Tuple[int, int]]]: ...
+    async def function_call(self, function_name: Literal['AHKMouseGetPos'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[Coordinates, AsyncFutureResult[Coordinates]]: ...
     @overload
     async def function_call(self, function_name: Literal['AHKKeyState'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[int, float, str, None, AsyncFutureResult[None], AsyncFutureResult[str], AsyncFutureResult[int], AsyncFutureResult[float]]: ...
     @overload
     async def function_call(self, function_name: Literal['AHKMouseMove'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[None, AsyncFutureResult[None]]: ...
     @overload
     async def function_call(self, function_name: Literal['AHKClick'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[None, AsyncFutureResult[None]]: ...
     @overload
```

### Comparing `ahk-1.6.3/ahk/_async/window.py` & `ahk-1.7.0/ahk/_async/window.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from typing import Sequence
 from typing import Tuple
 from typing import TYPE_CHECKING
 from typing import TypedDict
 from typing import TypeVar
 from typing import Union
 
+from ahk._types import Position
 from ahk.exceptions import WindowNotFoundException
-from ahk.message import Position
 
 if sys.version_info < (3, 10):
     from typing_extensions import TypeAlias
 else:
     from typing import TypeAlias
 
 if sys.version_info < (3, 11):
```

### Comparing `ahk-1.6.3/ahk/_constants.py` & `ahk-1.7.0/ahk/_constants.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.3/ahk/_hotkey.py` & `ahk-1.7.0/ahk/_hotkey.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.3/ahk/_sync/engine.py` & `ahk-1.7.0/ahk/_sync/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,72 +48,21 @@
 from ..keys import Key
 from .transport import DaemonProcessTransport
 from .transport import FutureResult
 from .transport import Transport
 from .window import Control
 from .window import Window
 
-# from .window import AsyncGui
-from ahk.message import Position
-
+from ahk._types import Position, CoordModeTargets, CoordModeRelativeTo, TitleMatchMode, _BUTTONS, MouseButton, SendMode, Coordinates
 
 sleep = time.sleep
 
 SyncFilterFunc: TypeAlias = Callable[[Window], bool]
 
-CoordModeTargets: TypeAlias = Union[
-    Literal['ToolTip'], Literal['Pixel'], Literal['Mouse'], Literal['Caret'], Literal['Menu']
-]
-CoordModeRelativeTo: TypeAlias = Union[Literal['Screen', 'Relative', 'Window', 'Client', '']]
-
-CoordMode: TypeAlias = Union[CoordModeTargets, Tuple[CoordModeTargets, CoordModeRelativeTo]]
-
-MatchModes: TypeAlias = Literal[1, 2, 3, 'RegEx', '']
-MatchSpeeds: TypeAlias = Literal['Fast', 'Slow', '']
-
-TitleMatchMode: TypeAlias = Optional[
-    Union[MatchModes, MatchSpeeds, Tuple[Union[MatchModes, MatchSpeeds], Union[MatchSpeeds, MatchModes]]]
-]
-
-_BUTTONS: dict[Union[str, int], str] = {
-    1: 'L',
-    2: 'R',
-    3: 'M',
-    'left': 'L',
-    'right': 'R',
-    'middle': 'M',
-    'wheelup': 'WU',
-    'wheeldown': 'WD',
-    'wheelleft': 'WL',
-    'wheelright': 'WR',
-}
-
-MouseButton: TypeAlias = Union[
-    int,
-    Literal[
-        'L',
-        'R',
-        'M',
-        'left',
-        'right',
-        'middle',
-        'wheelup',
-        'WU',
-        'wheeldown',
-        'WD',
-        'wheelleft',
-        'WL',
-        'wheelright',
-        'WR',
-    ],
-]
-
-SendMode: TypeAlias = Literal['Event', 'Input', 'InputThenPlay', 'Play', '']
-
-SyncPropertyReturnTupleIntInt: TypeAlias = Tuple[int, int]
+SyncPropertyReturnTupleIntInt: TypeAlias = Coordinates
 
 SyncPropertyReturnOptionalAsyncWindow: TypeAlias = Optional[Window]
 
 _PROPERTY_DEPRECATION_WARNING_MESSAGE = 'Use of the {0} property is not recommended (in the async API only) and may be removed in a future version. Use the get_{0} method instead'
 
 
 def _resolve_button(button: Union[str, int]) -> str:
@@ -728,25 +677,25 @@
             detect_hidden_windows=detect_hidden_windows,
         )
         resp = self._transport.function_call('AHKWindowList', args, engine=self, blocking=blocking)
         return resp
 
     # fmt: off
     @overload
-    def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: Literal[True]) -> Tuple[int, int]: ...
+    def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: Literal[True]) -> Coordinates: ...
     @overload
-    def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: Literal[False]) -> FutureResult[Tuple[int, int]]: ...
+    def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: Literal[False]) -> FutureResult[Coordinates]: ...
     @overload
-    def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None) -> Tuple[int, int]: ...
+    def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None) -> Coordinates: ...
     @overload
-    def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: bool = True) -> Union[Tuple[int, int], FutureResult[Tuple[int, int]]]: ...
+    def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: bool = True) -> Union[Coordinates, FutureResult[Coordinates]]: ...
     # fmt: on
     def get_mouse_position(
         self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: bool = True
-    ) -> Union[Tuple[int, int], FutureResult[Tuple[int, int]]]:
+    ) -> Union[Coordinates, FutureResult[Coordinates]]:
         """
         Analog for `MouseGetPos <https://www.autohotkey.com/docs/commands/MouseGetPos.htm>`_
         """
         if coord_mode:
             args = [str(coord_mode)]
         else:
             args = []
@@ -2854,36 +2803,36 @@
             send_mode = ''
         args = [str(x), str(y), button, str(click_count), direction or '', r, coord_mode, str(send_mode)]
         resp = self._transport.function_call('AHKClick', args, blocking=blocking)
         return resp
 
     # fmt: off
     @overload
-    def image_search(self, image_path: str, upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0), lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None, *, color_variation: Optional[int] = None, coord_mode: Optional[CoordModeRelativeTo] = None, scale_height: Optional[int] = None, scale_width: Optional[int] = None, transparent: Optional[str] = None, icon: Optional[int] = None) -> Optional[Tuple[int, int]]: ...
+    def image_search(self, image_path: str, upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0), lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None, *, color_variation: Optional[int] = None, coord_mode: Optional[CoordModeRelativeTo] = None, scale_height: Optional[int] = None, scale_width: Optional[int] = None, transparent: Optional[str] = None, icon: Optional[int] = None) -> Optional[Coordinates]: ...
     @overload
-    def image_search(self, image_path: str, upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0), lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None, *, color_variation: Optional[int] = None, coord_mode: Optional[CoordModeRelativeTo] = None, scale_height: Optional[int] = None, scale_width: Optional[int] = None, transparent: Optional[str] = None, icon: Optional[int] = None, blocking: Literal[False]) -> FutureResult[Optional[Tuple[int, int]]]: ...
+    def image_search(self, image_path: str, upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0), lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None, *, color_variation: Optional[int] = None, coord_mode: Optional[CoordModeRelativeTo] = None, scale_height: Optional[int] = None, scale_width: Optional[int] = None, transparent: Optional[str] = None, icon: Optional[int] = None, blocking: Literal[False]) -> FutureResult[Optional[Coordinates]]: ...
     @overload
-    def image_search(self, image_path: str, upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0), lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None, *, color_variation: Optional[int] = None, coord_mode: Optional[CoordModeRelativeTo] = None, scale_height: Optional[int] = None, scale_width: Optional[int] = None, transparent: Optional[str] = None, icon: Optional[int] = None, blocking: Literal[True]) -> Optional[Tuple[int, int]]: ...
+    def image_search(self, image_path: str, upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0), lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None, *, color_variation: Optional[int] = None, coord_mode: Optional[CoordModeRelativeTo] = None, scale_height: Optional[int] = None, scale_width: Optional[int] = None, transparent: Optional[str] = None, icon: Optional[int] = None, blocking: Literal[True]) -> Optional[Coordinates]: ...
     @overload
-    def image_search(self, image_path: str, upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0), lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None, *, color_variation: Optional[int] = None, coord_mode: Optional[CoordModeRelativeTo] = None, scale_height: Optional[int] = None, scale_width: Optional[int] = None, transparent: Optional[str] = None, icon: Optional[int] = None, blocking: bool = True) -> Union[Tuple[int, int], None, FutureResult[Optional[Tuple[int, int]]]]: ...
+    def image_search(self, image_path: str, upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0), lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None, *, color_variation: Optional[int] = None, coord_mode: Optional[CoordModeRelativeTo] = None, scale_height: Optional[int] = None, scale_width: Optional[int] = None, transparent: Optional[str] = None, icon: Optional[int] = None, blocking: bool = True) -> Union[Coordinates, None, FutureResult[Optional[Coordinates]]]: ...
     # fmt: on
     def image_search(
         self,
         image_path: str,
         upper_bound: Tuple[Union[int, str], Union[int, str]] = (0, 0),
         lower_bound: Optional[Tuple[Union[int, str], Union[int, str]]] = None,
         *,
         color_variation: Optional[int] = None,
         coord_mode: Optional[CoordModeRelativeTo] = None,
         scale_height: Optional[int] = None,
         scale_width: Optional[int] = None,
         transparent: Optional[str] = None,
         icon: Optional[int] = None,
         blocking: bool = True,
-    ) -> Union[Tuple[int, int], None, FutureResult[Optional[Tuple[int, int]]]]:
+    ) -> Union[Coordinates, None, FutureResult[Optional[Coordinates]]]:
         """
         Analog for `ImageSearch <https://www.autohotkey.com/docs/commands/ImageSearch.htm>`_
         """
 
         if scale_height and not scale_width:
             scale_width = -1
         elif scale_width and not scale_height:
@@ -3010,34 +2959,34 @@
         args.append(options)
 
         resp = self._transport.function_call('AHKPixelGetColor', args, blocking=blocking)
         return resp
 
     # fmt: off
     @overload
-    def pixel_search(self, search_region_start: Tuple[int, int], search_region_end: Tuple[int, int], color: Union[str, int], variation: int = 0, *, coord_mode: Optional[CoordModeRelativeTo] = None, fast: bool = True, rgb: bool = True) -> Optional[Tuple[int, int]]: ...
+    def pixel_search(self, search_region_start: Tuple[int, int], search_region_end: Tuple[int, int], color: Union[str, int], variation: int = 0, *, coord_mode: Optional[CoordModeRelativeTo] = None, fast: bool = True, rgb: bool = True) -> Optional[Coordinates]: ...
     @overload
-    def pixel_search(self, search_region_start: Tuple[int, int], search_region_end: Tuple[int, int], color: Union[str, int], variation: int = 0, *, coord_mode: Optional[CoordModeRelativeTo] = None, fast: bool = True, rgb: bool = True, blocking: Literal[True]) -> Optional[Tuple[int, int]]: ...
+    def pixel_search(self, search_region_start: Tuple[int, int], search_region_end: Tuple[int, int], color: Union[str, int], variation: int = 0, *, coord_mode: Optional[CoordModeRelativeTo] = None, fast: bool = True, rgb: bool = True, blocking: Literal[True]) -> Optional[Coordinates]: ...
     @overload
-    def pixel_search(self, search_region_start: Tuple[int, int], search_region_end: Tuple[int, int], color: Union[str, int], variation: int = 0, *, coord_mode: Optional[CoordModeRelativeTo] = None, fast: bool = True, rgb: bool = True, blocking: Literal[False]) -> FutureResult[Optional[Tuple[int, int]]]: ...
+    def pixel_search(self, search_region_start: Tuple[int, int], search_region_end: Tuple[int, int], color: Union[str, int], variation: int = 0, *, coord_mode: Optional[CoordModeRelativeTo] = None, fast: bool = True, rgb: bool = True, blocking: Literal[False]) -> FutureResult[Optional[Coordinates]]: ...
     @overload
-    def pixel_search(self, search_region_start: Tuple[int, int], search_region_end: Tuple[int, int], color: Union[str, int], variation: int = 0, *, coord_mode: Optional[CoordModeRelativeTo] = None, fast: bool = True, rgb: bool = True, blocking: bool = True) -> Union[Optional[Tuple[int, int]], FutureResult[Optional[Tuple[int, int]]]]: ...
+    def pixel_search(self, search_region_start: Tuple[int, int], search_region_end: Tuple[int, int], color: Union[str, int], variation: int = 0, *, coord_mode: Optional[CoordModeRelativeTo] = None, fast: bool = True, rgb: bool = True, blocking: bool = True) -> Union[Optional[Coordinates], FutureResult[Optional[Coordinates]]]: ...
     # fmt: on
     def pixel_search(
         self,
         search_region_start: Tuple[int, int],
         search_region_end: Tuple[int, int],
         color: Union[str, int],
         variation: int = 0,
         *,
         coord_mode: Optional[CoordModeRelativeTo] = None,
         fast: bool = True,
         rgb: bool = True,
         blocking: bool = True,
-    ) -> Union[Optional[Tuple[int, int]], FutureResult[Optional[Tuple[int, int]]]]:
+    ) -> Union[Optional[Coordinates], FutureResult[Optional[Coordinates]]]:
         """
         Analog for `PixelSearch <https://www.autohotkey.com/docs/commands/PixelSearch.htm>`_
         """
         x1, y1 = search_region_start
         x2, y2 = search_region_end
         args = [str(x1), str(y1), str(x2), str(y2), str(color), str(variation)]
         mode = ' '.join(word for word, val in zip(('Fast', 'RGB'), (fast, rgb)) if val)
```

### Comparing `ahk-1.6.3/ahk/_sync/transport.py` & `ahk-1.7.0/ahk/_sync/transport.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import subprocess
 import sys
 import tempfile
 import threading
 import warnings
 from abc import ABC
 from abc import abstractmethod
+from concurrent.futures import Future
+from concurrent.futures import ThreadPoolExecutor
 from io import BytesIO
 from typing import Any
 from typing import Callable
 from typing import Generic
 from typing import List
 from typing import Literal
 from typing import Optional
@@ -23,170 +25,61 @@
 from typing import runtime_checkable
 from typing import Tuple
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
+import jinja2
+
+from ahk._constants import DAEMON_SCRIPT_TEMPLATE as _DAEMON_SCRIPT_TEMPLATE
+from ahk._constants import DAEMON_SCRIPT_V2_TEMPLATE as _DAEMON_SCRIPT_V2_TEMPLATE
+from ahk._hotkey import Hotkey
+from ahk._hotkey import Hotstring
+from ahk._hotkey import ThreadedHotkeyTransport
+from ahk._types import Coordinates
+from ahk._types import FunctionName
+from ahk._types import Position
+from ahk._utils import _version_detection_script
+from ahk.directives import Directive
+from ahk.exceptions import AHKProtocolError
+from ahk.extensions import _resolve_includes
+from ahk.extensions import Extension
+from ahk.message import _message_registry
+from ahk.message import RequestMessage
+from ahk.message import ResponseMessage
+
+
 if TYPE_CHECKING:
     from ahk import Control
     from ahk import Window
 
 if sys.version_info < (3, 10):
     from typing_extensions import TypeAlias, TypeGuard
 else:
     from typing import TypeAlias, TypeGuard
 
-import jinja2
-
-from ahk.extensions import Extension, _resolve_includes
-from ahk._hotkey import ThreadedHotkeyTransport, Hotkey, Hotstring
-from ahk.message import RequestMessage
-from ahk.message import ResponseMessage
-from ahk.message import Position
-from ahk.message import _message_registry
-from ahk._constants import (
-    DAEMON_SCRIPT_TEMPLATE as _DAEMON_SCRIPT_TEMPLATE,
-    DAEMON_SCRIPT_V2_TEMPLATE as _DAEMON_SCRIPT_V2_TEMPLATE,
-)
-from ahk._utils import _version_detection_script
-from ahk.directives import Directive
-from ahk.exceptions import AHKProtocolError
-
-from concurrent.futures import Future, ThreadPoolExecutor
-
 
 T_SyncFuture = TypeVar('T_SyncFuture')
 
 
 
 
-
-
 class FutureResult(Generic[T_SyncFuture]):
     def __init__(self, future: Future[T_SyncFuture]):
         self._fut: Future[T_SyncFuture] = future
 
     def result(self, timeout: Optional[float] = None) -> T_SyncFuture:
         return self._fut.result(timeout=timeout)
 
 
 
 SyncIOProcess: TypeAlias = 'subprocess.Popen[bytes]'
 
 
-FunctionName = Literal[
-    'AHKBlockInput',
-    'AHKClipWait',
-    'AHKControlClick',
-    'AHKControlGetPos',
-    'AHKControlGetText',
-    'AHKControlSend',
-    'AHKFileSelectFile',
-    'AHKFileSelectFolder',
-    'AHKGetClipboard',
-    'AHKGetClipboardAll',
-    'AHKGetCoordMode',
-    'AHKGetSendLevel',
-    'AHKGetSendMode',
-    'AHKGetTitleMatchMode',
-    'AHKGetTitleMatchSpeed',
-    'AHKGetVolume',
-    'AHKGuiNew',
-    'AHKImageSearch',
-    'AHKInputBox',
-    'AHKKeyState',
-    'AHKKeyWait',
-    'AHKMenuTrayIcon',
-    'AHKMenuTrayShow',
-    'AHKMenuTrayHide',
-    'AHKMenuTrayTip',
-    'AHKMsgBox',
-    'AHKMouseClickDrag',
-    'AHKMouseGetPos',
-    'AHKMouseMove',
-    'AHKPixelGetColor',
-    'AHKPixelSearch',
-    'AHKRegRead',
-    'AHKRegWrite',
-    'AHKRegDelete',
-    'AHKSend',
-    'AHKSendEvent',
-    'AHKSendInput',
-    'AHKSendPlay',
-    'AHKSendRaw',
-    'AHKSetClipboard',
-    'AHKSetClipboardAll',
-    'AHKSetCoordMode',
-    'AHKSetDetectHiddenWindows',
-    'AHKSetSendLevel',
-    'AHKSetSendMode',
-    'AHKSetTitleMatchMode',
-    'AHKSetVolume',
-    'AHKShowToolTip',
-    'AHKSoundBeep',
-    'AHKSoundGet',
-    'AHKSoundPlay',
-    'AHKSoundSet',
-    'AHKTrayTip',
-    'AHKWinActivate',
-    'AHKWinClose',
-    'AHKWinExist',
-    'AHKWinFromMouse',
-    'AHKWinGetControlList',
-    'AHKWinGetControlListHwnd',
-    'AHKWinGetCount',
-    'AHKWinGetExStyle',
-    'AHKWinGetID',
-    'AHKWinGetIDLast',
-    'AHKWinGetList',
-    'AHKWinGetMinMax',
-    'AHKWinGetPID',
-    'AHKWinGetPos',
-    'AHKWinGetProcessName',
-    'AHKWinGetProcessPath',
-    'AHKWinGetStyle',
-    'AHKWinGetText',
-    'AHKWinGetTitle',
-    'AHKWinGetTransColor',
-    'AHKWinGetTransparent',
-    'AHKWinHide',
-    'AHKWinIsActive',
-    'AHKWinIsAlwaysOnTop',
-    'AHKWinMove',
-    'AHKWinSetAlwaysOnTop',
-    'AHKWinSetBottom',
-    'AHKWinSetDisable',
-    'AHKWinSetEnable',
-    'AHKWinSetExStyle',
-    'AHKWinSetRedraw',
-    'AHKWinSetRegion',
-    'AHKWinSetStyle',
-    'AHKWinSetTitle',
-    'AHKWinSetTop',
-    'AHKWinSetTransColor',
-    'AHKWinSetTransparent',
-    'AHKWinShow',
-    'AHKWindowList',
-    'AHKWinWait',
-    'AHKWinWaitActive',
-    'AHKWinWaitClose',
-    'AHKWinWaitNotActive',
-    'AHKClick',
-    'AHKSetCapsLockState',
-    'SetKeyDelay',
-    'WinActivateBottom',
-    'AHKWinGetClass',
-    'AHKWinKill',
-    'AHKWinMaximize',
-    'AHKWinMinimize',
-    'AHKWinRestore',
-]
-
-
 @runtime_checkable
 class Killable(Protocol):
     def kill(self) -> None: ...
 
 
 def kill(proc: Killable) -> None:
     try:
@@ -194,15 +87,17 @@
     except:  # noqa
         pass
 
 
 def async_assert_send_nonblocking_type_correct(
     obj: Any,
 ) -> TypeGuard[
-    Future[Union[None, Tuple[int, int], int, str, bool, Window, List[Window], List[Control]]]
+    Future[
+        Union[None, Coordinates, Tuple[int, int], int, str, bool, Window, List[Window], List[Control]]
+    ]
 ]:
     return True
 
 
 class Communicable(Protocol):
     runargs: List[str]
 
@@ -378,21 +273,21 @@
     ) -> Union[str, FutureResult[str]]:
         return NotImplemented
 
     # fmt: off
     @overload
     def function_call(self, function_name: Literal['AHKWinExist'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[bool, FutureResult[bool]]: ...
     @overload
-    def function_call(self, function_name: Literal['AHKImageSearch'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[Tuple[int, int], None, FutureResult[Union[Tuple[int, int], None]]]: ...
+    def function_call(self, function_name: Literal['AHKImageSearch'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[Coordinates, None, FutureResult[Union[Coordinates, None]]]: ...
     @overload
     def function_call(self, function_name: Literal['AHKPixelGetColor'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[str, FutureResult[str]]: ...
     @overload
-    def function_call(self, function_name: Literal['AHKPixelSearch'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[Optional[Tuple[int, int]], FutureResult[Optional[Tuple[int, int]]]]: ...
+    def function_call(self, function_name: Literal['AHKPixelSearch'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[Optional[Coordinates], FutureResult[Optional[Coordinates]]]: ...
     @overload
-    def function_call(self, function_name: Literal['AHKMouseGetPos'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[Tuple[int, int], FutureResult[Tuple[int, int]]]: ...
+    def function_call(self, function_name: Literal['AHKMouseGetPos'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[Coordinates, FutureResult[Coordinates]]: ...
     @overload
     def function_call(self, function_name: Literal['AHKKeyState'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[int, float, str, None, FutureResult[None], FutureResult[str], FutureResult[int], FutureResult[float]]: ...
     @overload
     def function_call(self, function_name: Literal['AHKMouseMove'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[None, FutureResult[None]]: ...
     @overload
     def function_call(self, function_name: Literal['AHKClick'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[None, FutureResult[None]]: ...
     @overload
```

### Comparing `ahk-1.6.3/ahk/_sync/window.py` & `ahk-1.7.0/ahk/_sync/window.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from typing import Sequence
 from typing import Tuple
 from typing import TYPE_CHECKING
 from typing import TypedDict
 from typing import TypeVar
 from typing import Union
 
+from ahk._types import Position
 from ahk.exceptions import WindowNotFoundException
-from ahk.message import Position
 
 if sys.version_info < (3, 10):
     from typing_extensions import TypeAlias
 else:
     from typing import TypeAlias
 
 if sys.version_info < (3, 11):
@@ -28,16 +28,14 @@
     from typing import NotRequired
 
 if TYPE_CHECKING:
     from .engine import AHK
     from .transport import FutureResult
 
 
-
-
 SyncPropertyReturnStr: TypeAlias = str
 
 SyncPropertyReturnInt: TypeAlias = int
 
 SyncPropertyReturnTupleIntInt: TypeAlias = Tuple[int, int]
 
 SyncPropertyReturnBool: TypeAlias = bool
```

### Comparing `ahk-1.6.3/ahk/_utils.py` & `ahk-1.7.0/ahk/_utils.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.3/ahk/directives.py` & `ahk-1.7.0/ahk/directives.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.3/ahk/extensions.py` & `ahk-1.7.0/ahk/extensions.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.3/ahk/keys.py` & `ahk-1.7.0/ahk/keys.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.3/ahk/message.py` & `ahk-1.7.0/ahk/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import ast
 import base64
 import itertools
 import string
 import sys
 from abc import abstractmethod
 from base64 import b64encode
-from collections import namedtuple
 from typing import Any
 from typing import cast
 from typing import Generator
 from typing import List
 from typing import NoReturn
 from typing import Optional
 from typing import Protocol
@@ -24,22 +23,20 @@
     from typing import TypeGuard
 else:
     from typing_extensions import TypeGuard
 from typing import TypeVar
 from typing import Union
 
 from ahk.exceptions import AHKExecutionException
+from ahk._types import Position, Coordinates
 
 
 class OutOfMessageTypes(Exception): ...
 
 
-Position = namedtuple('Position', ('x', 'y', 'width', 'height'))
-
-
 @runtime_checkable
 class BytesLineReadable(Protocol):
     def readline(self) -> bytes: ...
 
 
 def is_window_control_list_response(resp_obj: object) -> TypeGuard[Tuple[str, List[Tuple[str, str]]]]:
     if not isinstance(resp_obj, tuple):
@@ -153,20 +150,20 @@
         s = self._raw_content.decode(encoding='utf-8')
         val = ast.literal_eval(s)
         assert isinstance(val, tuple)
         return val
 
 
 class CoordinateResponseMessage(ResponseMessage):
-    def unpack(self) -> Tuple[int, int]:
+    def unpack(self) -> Coordinates:
         s = self._raw_content.decode(encoding='utf-8')
         val = ast.literal_eval(s)
         assert isinstance(val, tuple)
         x, y = cast(Tuple[int, int], val)
-        return x, y
+        return Coordinates(x, y)
 
 
 class IntegerResponseMessage(ResponseMessage):
     def unpack(self) -> int:
         s = self._raw_content.decode(encoding='utf-8')
         val = ast.literal_eval(s)
         assert isinstance(val, int)
```

### Comparing `ahk-1.6.3/ahk/templates/daemon-v2.ahk` & `ahk-1.7.0/ahk/templates/daemon-v2.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.6.3/ahk/templates/daemon.ahk` & `ahk-1.7.0/ahk/templates/daemon.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.6.3/ahk/templates/hotkeys-v2.ahk` & `ahk-1.7.0/ahk/templates/hotkeys-v2.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.6.3/ahk/templates/hotkeys.ahk` & `ahk-1.7.0/ahk/templates/hotkeys.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.6.3/ahk.egg-info/PKG-INFO` & `ahk-1.7.0/ahk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.6.3
+Version: 1.7.0
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://ahk.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/spyoungtech/
 Project-URL: Source, https://github.com/spyoungtech/ahk
@@ -17,14 +17,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_extensions; python_version < "3.11"
 Requires-Dist: jinja2>=3.0
 Provides-Extra: binary
 Requires-Dist: ahk-binary==2023.9.0; extra == "binary"
```

### Comparing `ahk-1.6.3/ahk.egg-info/SOURCES.txt` & `ahk-1.7.0/ahk.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 buildunasync.py
 pyproject.toml
 setup.cfg
 setup.py
 ahk/__init__.py
 ahk/_constants.py
 ahk/_hotkey.py
+ahk/_types.py
 ahk/_utils.py
 ahk/directives.py
 ahk/exceptions.py
 ahk/extensions.py
 ahk/keys.py
 ahk/message.py
 ahk/py.typed
```

### Comparing `ahk-1.6.3/buildunasync.py` & `ahk-1.7.0/buildunasync.py`

 * *Files identical despite different names*

### Comparing `ahk-1.6.3/docs/README.md` & `ahk-1.7.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `ahk-1.6.3/setup.cfg` & `ahk-1.7.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ahk
-version = 1.6.3
+version = 1.7.0
 author_email = spencer.young@spyoung.com
 author = Spencer Young
 description = A Python wrapper for AHK
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 url = https://github.com/spyoungtech/ahk
 project_urls = 
@@ -29,14 +29,16 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
+	Typing :: Typed
 
 [options]
 include_package_data = True
 python_requires = >=3.8.0
 packages = 
 	ahk
 	ahk.templates
```


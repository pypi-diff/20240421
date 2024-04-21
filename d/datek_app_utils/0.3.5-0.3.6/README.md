# Comparing `tmp/datek_app_utils-0.3.5.tar.gz` & `tmp/datek_app_utils-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datek_app_utils-0.3.5.tar", max compression
+gzip compressed data, was "datek_app_utils-0.3.6.tar", max compression
```

## Comparing `datek_app_utils-0.3.5.tar` & `datek_app_utils-0.3.6.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1073 2022-12-15 08:30:28.864878 datek_app_utils-0.3.5/LICENSE
--rw-r--r--   0        0        0     1877 2022-12-15 08:30:28.864878 datek_app_utils-0.3.5/README.md
--rw-r--r--   0        0        0        0 2022-12-15 08:30:28.864878 datek_app_utils-0.3.5/datek_app_utils/__init__.py
--rw-r--r--   0        0        0     2097 2022-12-15 08:30:28.864878 datek_app_utils-0.3.5/datek_app_utils/async_utils.py
--rw-r--r--   0        0        0        0 2022-12-15 08:30:28.864878 datek_app_utils-0.3.5/datek_app_utils/env_config/__init__.py
--rw-r--r--   0        0        0     1658 2022-12-15 08:30:28.864878 datek_app_utils-0.3.5/datek_app_utils/env_config/base.py
--rw-r--r--   0        0        0      948 2022-12-15 08:30:28.864878 datek_app_utils-0.3.5/datek_app_utils/env_config/errors.py
--rw-r--r--   0        0        0      375 2022-12-15 08:30:28.864878 datek_app_utils-0.3.5/datek_app_utils/env_config/types.py
--rw-r--r--   0        0        0      977 2022-12-15 08:30:28.864878 datek_app_utils-0.3.5/datek_app_utils/env_config/utils.py
--rw-r--r--   0        0        0     1078 2022-12-15 08:30:28.864878 datek_app_utils-0.3.5/datek_app_utils/log.py
--rw-r--r--   0        0        0        0 2022-12-15 08:30:28.864878 datek_app_utils-0.3.5/datek_app_utils/py.typed
--rw-r--r--   0        0        0      730 2022-12-15 08:30:56.781024 datek_app_utils-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2576 1970-01-01 00:00:00.000000 datek_app_utils-0.3.5/setup.py
--rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 datek_app_utils-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-21 15:21:52.190423 datek_app_utils-0.3.6/LICENSE
+-rw-r--r--   0        0        0     1863 2024-04-21 15:21:52.190423 datek_app_utils-0.3.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-21 15:21:52.190423 datek_app_utils-0.3.6/datek_app_utils/__init__.py
+-rw-r--r--   0        0        0     2356 2024-04-21 15:21:52.190423 datek_app_utils-0.3.6/datek_app_utils/async_utils.py
+-rw-r--r--   0        0        0        0 2024-04-21 15:21:52.190423 datek_app_utils-0.3.6/datek_app_utils/env_config/__init__.py
+-rw-r--r--   0        0        0     1658 2024-04-21 15:21:52.190423 datek_app_utils-0.3.6/datek_app_utils/env_config/base.py
+-rw-r--r--   0        0        0      948 2024-04-21 15:21:52.190423 datek_app_utils-0.3.6/datek_app_utils/env_config/errors.py
+-rw-r--r--   0        0        0      375 2024-04-21 15:21:52.190423 datek_app_utils-0.3.6/datek_app_utils/env_config/types.py
+-rw-r--r--   0        0        0      977 2024-04-21 15:21:52.190423 datek_app_utils-0.3.6/datek_app_utils/env_config/utils.py
+-rw-r--r--   0        0        0     1106 2024-04-21 15:21:52.190423 datek_app_utils-0.3.6/datek_app_utils/log.py
+-rw-r--r--   0        0        0        0 2024-04-21 15:21:52.190423 datek_app_utils-0.3.6/datek_app_utils/py.typed
+-rw-r--r--   0        0        0      710 2024-04-21 15:22:14.318263 datek_app_utils-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     2576 1970-01-01 00:00:00.000000 datek_app_utils-0.3.6/PKG-INFO
```

### Comparing `datek_app_utils-0.3.5/LICENSE` & `datek_app_utils-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datek_app_utils-0.3.5/README.md` & `datek_app_utils-0.3.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![codecov](https://codecov.io/gh/DAtek/datek-app-utils/branch/master/graph/badge.svg?token=UR0G0I41LD)](https://codecov.io/gh/DAtek/datek-app-utils)
+[![codecov](https://codecov.io/gh/DAtek/datek-app-utils/graph/badge.svg?token=UR0G0I41LD)](https://codecov.io/gh/DAtek/datek-app-utils)
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://github.com/psf/black/blob/main/LICENSE"><img alt="License: MIT" src="https://black.readthedocs.io/en/stable/_static/license.svg"></a>
 
 # Utilities for building applications.
 
 ## Contains:
 - Config loading from environment
```

### Comparing `datek_app_utils-0.3.5/datek_app_utils/async_utils.py` & `datek_app_utils-0.3.6/datek_app_utils/async_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+import sys
 from abc import abstractmethod
 from asyncio import Task, sleep, CancelledError, create_task, gather, Future
 from functools import wraps
-from typing import Callable, Optional
+from typing import Callable, Optional, TypeVar
+
+if sys.version_info >= (3, 10):  # pragma: no cover
+    from typing import ParamSpec
+else:  # pragma: no cover
+    from typing_extensions import ParamSpec
 
 
 class AsyncWorker:
-    def __init__(self):
+    def __init__(self) -> None:
         self._task: Optional[Task] = None
-        self._started = Future()
+        self._started: Future = Future()
 
     @abstractmethod
     async def run(self):  # pragma: no cover
         pass
 
     @abstractmethod
     async def handle_error(self, error: Exception):  # pragma: no cover
@@ -38,18 +44,22 @@
             except Exception as error:
                 await self.handle_error(error)
 
     def __await__(self):
         return self._task.__await__()
 
 
+P = ParamSpec("P")
+T = TypeVar("T")
+
+
 def async_timeout(seconds: float):
-    def decorator(func: Callable):
+    def decorator(func: Callable[P, T]):
         @wraps(func)
-        async def wrapper(*args, **kwargs):
+        async def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
             timeout_task: Optional[Task] = None
             main_task: Optional[Task] = None
 
             async def raise_timeout_error():
                 try:
                     await sleep(seconds)
                 except CancelledError:
```

### Comparing `datek_app_utils-0.3.5/datek_app_utils/env_config/base.py` & `datek_app_utils-0.3.6/datek_app_utils/env_config/base.py`

 * *Files identical despite different names*

### Comparing `datek_app_utils-0.3.5/datek_app_utils/env_config/errors.py` & `datek_app_utils-0.3.6/datek_app_utils/env_config/errors.py`

 * *Files identical despite different names*

### Comparing `datek_app_utils-0.3.5/datek_app_utils/env_config/utils.py` & `datek_app_utils-0.3.6/datek_app_utils/env_config/utils.py`

 * *Files identical despite different names*

### Comparing `datek_app_utils-0.3.5/datek_app_utils/log.py` & `datek_app_utils-0.3.6/datek_app_utils/log.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import sys
 from logging import Formatter, StreamHandler, getLogger, Logger, INFO, Handler
 
 
 class LogHandler:
-    _handler: Handler = StreamHandler()
+    _handler: Handler = StreamHandler(stream=sys.stdout)
 
     @classmethod
     def set(cls, handler: Handler):
         cls._handler = handler
 
     @classmethod
     def get(cls) -> Handler:
```

### Comparing `datek_app_utils-0.3.5/setup.py` & `datek_app_utils-0.3.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 2764 6174 656b 5f61 7070 5f75   \.['datek_app_u
-00000050: 7469 6c73 272c 2027 6461 7465 6b5f 6170  tils', 'datek_ap
-00000060: 705f 7574 696c 732e 656e 765f 636f 6e66  p_utils.env_conf
-00000070: 6967 275d 0a0a 7061 636b 6167 655f 6461  ig']..package_da
-00000080: 7461 203d 205c 0a7b 2727 3a20 5b27 2a27  ta = \.{'': ['*'
-00000090: 5d7d 0a0a 7365 7475 705f 6b77 6172 6773  ]}..setup_kwargs
-000000a0: 203d 207b 0a20 2020 2027 6e61 6d65 273a   = {.    'name':
-000000b0: 2027 6461 7465 6b2d 6170 702d 7574 696c   'datek-app-util
-000000c0: 7327 2c0a 2020 2020 2776 6572 7369 6f6e  s',.    'version
-000000d0: 273a 2027 302e 332e 3527 2c0a 2020 2020  ': '0.3.5',.    
-000000e0: 2764 6573 6372 6970 7469 6f6e 273a 2027  'description': '
-000000f0: 5574 696c 6974 6965 7320 666f 7220 6275  Utilities for bu
-00000100: 696c 6469 6e67 2061 7070 6c69 6361 7469  ilding applicati
-00000110: 6f6e 7327 2c0a 2020 2020 276c 6f6e 675f  ons',.    'long_
-00000120: 6465 7363 7269 7074 696f 6e27 3a20 275b  description': '[
-00000130: 215b 636f 6465 636f 765d 2868 7474 7073  ![codecov](https
-00000140: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
-00000150: 2f44 4174 656b 2f64 6174 656b 2d61 7070  /DAtek/datek-app
-00000160: 2d75 7469 6c73 2f62 7261 6e63 682f 6d61  -utils/branch/ma
-00000170: 7374 6572 2f67 7261 7068 2f62 6164 6765  ster/graph/badge
-00000180: 2e73 7667 3f74 6f6b 656e 3d55 5230 4730  .svg?token=UR0G0
-00000190: 4934 314c 4429 5d28 6874 7470 733a 2f2f  I41LD)](https://
-000001a0: 636f 6465 636f 762e 696f 2f67 682f 4441  codecov.io/gh/DA
-000001b0: 7465 6b2f 6461 7465 6b2d 6170 702d 7574  tek/datek-app-ut
-000001c0: 696c 7329 5c6e 3c61 2068 7265 663d 2268  ils)\n<a href="h
-000001d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000001e0: 6d2f 7073 662f 626c 6163 6b22 3e3c 696d  m/psf/black"><im
-000001f0: 6720 616c 743d 2243 6f64 6520 7374 796c  g alt="Code styl
-00000200: 653a 2062 6c61 636b 2220 7372 633d 2268  e: black" src="h
-00000210: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000220: 6473 2e69 6f2f 6261 6467 652f 636f 6465  ds.io/badge/code
-00000230: 2532 3073 7479 6c65 2d62 6c61 636b 2d30  %20style-black-0
-00000240: 3030 3030 302e 7376 6722 3e3c 2f61 3e5c  00000.svg"></a>\
-00000250: 6e3c 6120 6872 6566 3d22 6874 7470 733a  n<a href="https:
-00000260: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7366  //github.com/psf
-00000270: 2f62 6c61 636b 2f62 6c6f 622f 6d61 696e  /black/blob/main
-00000280: 2f4c 4943 454e 5345 223e 3c69 6d67 2061  /LICENSE"><img a
-00000290: 6c74 3d22 4c69 6365 6e73 653a 204d 4954  lt="License: MIT
-000002a0: 2220 7372 633d 2268 7474 7073 3a2f 2f62  " src="https://b
-000002b0: 6c61 636b 2e72 6561 6474 6865 646f 6373  lack.readthedocs
-000002c0: 2e69 6f2f 656e 2f73 7461 626c 652f 5f73  .io/en/stable/_s
-000002d0: 7461 7469 632f 6c69 6365 6e73 652e 7376  tatic/license.sv
-000002e0: 6722 3e3c 2f61 3e5c 6e5c 6e23 2055 7469  g"></a>\n\n# Uti
-000002f0: 6c69 7469 6573 2066 6f72 2062 7569 6c64  lities for build
-00000300: 696e 6720 6170 706c 6963 6174 696f 6e73  ing applications
-00000310: 2e5c 6e5c 6e23 2320 436f 6e74 6169 6e73  .\n\n## Contains
-00000320: 3a5c 6e2d 2043 6f6e 6669 6720 6c6f 6164  :\n- Config load
-00000330: 696e 6720 6672 6f6d 2065 6e76 6972 6f6e  ing from environ
-00000340: 6d65 6e74 5c6e 2d20 426f 6f74 7374 7261  ment\n- Bootstra
-00000350: 7020 666f 7220 6c6f 6767 696e 675c 6e2d  p for logging\n-
-00000360: 2042 6173 6520 636c 6173 7320 666f 7220   Base class for 
-00000370: 6372 6561 7469 6e67 2061 7379 6e63 2077  creating async w
-00000380: 6f72 6b65 7273 5c6e 2d20 4173 796e 6320  orkers\n- Async 
-00000390: 7469 6d65 6f75 7420 6465 636f 7261 746f  timeout decorato
-000003a0: 722c 2077 6869 6368 2069 7320 7665 7279  r, which is very
-000003b0: 2075 7365 6675 6c20 666f 7220 7772 6974   useful for writ
-000003c0: 696e 6720 6173 796e 6320 7465 7374 735c  ing async tests\
-000003d0: 6e5c 6e23 2320 4578 616d 706c 6573 3a5c  n\n## Examples:\
-000003e0: 6e5c 6e23 2323 2045 6e76 2063 6f6e 6669  n\n### Env confi
-000003f0: 675c 6e60 6060 7079 7468 6f6e 5c6e 696d  g\n```python\nim
-00000400: 706f 7274 206f 735c 6e5c 6e66 726f 6d20  port os\n\nfrom 
-00000410: 6461 7465 6b5f 6170 705f 7574 696c 732e  datek_app_utils.
-00000420: 656e 765f 636f 6e66 6967 2e62 6173 6520  env_config.base 
-00000430: 696d 706f 7274 2042 6173 6543 6f6e 6669  import BaseConfi
-00000440: 675c 6e5c 6e6f 732e 656e 7669 726f 6e5b  g\n\nos.environ[
-00000450: 2243 4f4c 4f52 225d 203d 2022 5245 4422  "COLOR"] = "RED"
-00000460: 5c6e 6f73 2e65 6e76 6972 6f6e 5b22 5445  \nos.environ["TE
-00000470: 4d50 4552 4154 5552 4522 5d20 3d20 2235  MPERATURE"] = "5
-00000480: 3022 5c6e 5c6e 5c6e 636c 6173 7320 436f  0"\n\n\nclass Co
-00000490: 6e66 6967 2842 6173 6543 6f6e 6669 6729  nfig(BaseConfig)
-000004a0: 3a5c 6e20 2020 2043 4f4c 4f52 3a20 7374  :\n    COLOR: st
-000004b0: 725c 6e20 2020 2054 454d 5045 5241 5455  r\n    TEMPERATU
-000004c0: 5245 3a20 696e 745c 6e5c 6e5c 6e61 7373  RE: int\n\n\nass
-000004d0: 6572 7420 436f 6e66 6967 2e43 4f4c 4f52  ert Config.COLOR
-000004e0: 203d 3d20 2252 4544 225c 6e61 7373 6572   == "RED"\nasser
-000004f0: 7420 436f 6e66 6967 2e54 454d 5045 5241  t Config.TEMPERA
-00000500: 5455 5245 203d 3d20 3530 5c6e 6060 605c  TURE == 50\n```\
-00000510: 6e5c 6e54 6865 2060 436f 6e66 6967 6020  n\nThe `Config` 
-00000520: 636c 6173 7320 6361 7374 7320 7468 6520  class casts the 
-00000530: 7661 6c75 6573 2061 7574 6f6d 6174 6963  values automatic
-00000540: 616c 6c79 2e5c 6e4d 6f72 656f 7665 722c  ally.\nMoreover,
-00000550: 2079 6f75 2063 616e 2074 6573 7420 7768   you can test wh
-00000560: 6574 6865 7220 616c 6c20 7468 6520 6d61  ether all the ma
-00000570: 6e64 6174 6f72 7920 7661 7269 6162 6c65  ndatory variable
-00000580: 7320 6861 7665 2062 6565 6e20 7365 7420  s have been set 
-00000590: 6f72 206e 6f74 2e5c 6e5c 6e60 6060 7079  or not.\n\n```py
-000005a0: 7468 6f6e 5c6e 696d 706f 7274 206f 735c  thon\nimport os\
-000005b0: 6e5c 6e66 726f 6d20 6461 7465 6b5f 6170  n\nfrom datek_ap
-000005c0: 705f 7574 696c 732e 656e 765f 636f 6e66  p_utils.env_conf
-000005d0: 6967 2e62 6173 6520 696d 706f 7274 2042  ig.base import B
-000005e0: 6173 6543 6f6e 6669 675c 6e66 726f 6d20  aseConfig\nfrom 
-000005f0: 6461 7465 6b5f 6170 705f 7574 696c 732e  datek_app_utils.
-00000600: 656e 765f 636f 6e66 6967 2e75 7469 6c73  env_config.utils
-00000610: 2069 6d70 6f72 7420 7661 6c69 6461 7465   import validate
-00000620: 5f63 6f6e 6669 675c 6e66 726f 6d20 6461  _config\nfrom da
-00000630: 7465 6b5f 6170 705f 7574 696c 732e 656e  tek_app_utils.en
-00000640: 765f 636f 6e66 6967 2e65 7272 6f72 7320  v_config.errors 
-00000650: 696d 706f 7274 2056 616c 6964 6174 696f  import Validatio
-00000660: 6e45 7272 6f72 5c6e 5c6e 6f73 2e65 6e76  nError\n\nos.env
-00000670: 6972 6f6e 5b22 434f 4c4f 5222 5d20 3d20  iron["COLOR"] = 
-00000680: 2252 4544 225c 6e5c 6e5c 6e63 6c61 7373  "RED"\n\n\nclass
-00000690: 2043 6f6e 6669 6728 4261 7365 436f 6e66   Config(BaseConf
-000006a0: 6967 293a 5c6e 2020 2020 434f 4c4f 523a  ig):\n    COLOR:
-000006b0: 2073 7472 5c6e 2020 2020 5445 4d50 4552   str\n    TEMPER
-000006c0: 4154 5552 453a 2069 6e74 5c6e 2020 2020  ATURE: int\n    
-000006d0: 414d 4f55 4e54 3a20 696e 7420 3d20 4e6f  AMOUNT: int = No
-000006e0: 6e65 5c6e 5c6e 5c6e 7472 793a 5c6e 2020  ne\n\n\ntry:\n  
-000006f0: 2020 7661 6c69 6461 7465 5f63 6f6e 6669    validate_confi
-00000700: 6728 436f 6e66 6967 295c 6e65 7863 6570  g(Config)\nexcep
-00000710: 7420 5661 6c69 6461 7469 6f6e 4572 726f  t ValidationErro
-00000720: 7220 6173 2065 7272 6f72 3a5c 6e20 2020  r as error:\n   
-00000730: 2066 6f72 2061 7474 7269 6275 7465 5f65   for attribute_e
-00000740: 7272 6f72 2069 6e20 6572 726f 722e 6572  rror in error.er
-00000750: 726f 7273 3a5c 6e20 2020 2020 2020 2070  rors:\n        p
-00000760: 7269 6e74 2861 7474 7269 6275 7465 5f65  rint(attribute_e
-00000770: 7272 6f72 295c 6e5c 6e60 6060 5c6e 4f75  rror)\n\n```\nOu
-00000780: 7470 7574 3a5c 6e60 6060 5c6e 5445 4d50  tput:\n```\nTEMP
-00000790: 4552 4154 5552 453a 204e 6f74 2073 6574  ERATURE: Not set
-000007a0: 2e20 5265 7175 6972 6564 2074 7970 653a  . Required type:
-000007b0: 203c 636c 6173 7320 5c27 696e 745c 273e   <class \'int\'>
-000007c0: 5c6e 6060 605c 6e5c 6e23 2323 2041 7379  \n```\n\n### Asy
-000007d0: 6e63 2074 696d 656f 7574 2064 6563 6f72  nc timeout decor
-000007e0: 6174 6f72 5c6e 5c6e 6060 6070 7974 686f  ator\n\n```pytho
-000007f0: 6e5c 6e66 726f 6d20 6173 796e 6369 6f20  n\nfrom asyncio 
-00000800: 696d 706f 7274 2073 6c65 6570 2c20 7275  import sleep, ru
-00000810: 6e5c 6e66 726f 6d20 6461 7465 6b5f 6170  n\nfrom datek_ap
-00000820: 705f 7574 696c 732e 6173 796e 635f 7574  p_utils.async_ut
-00000830: 696c 7320 696d 706f 7274 2061 7379 6e63  ils import async
-00000840: 5f74 696d 656f 7574 5c6e 5c6e 5c6e 4061  _timeout\n\n\n@a
-00000850: 7379 6e63 5f74 696d 656f 7574 2830 2e31  sync_timeout(0.1
-00000860: 295c 6e61 7379 6e63 2064 6566 2073 6c65  )\nasync def sle
-00000870: 6570 5f6f 6e65 5f73 6563 2829 3a5c 6e20  ep_one_sec():\n 
-00000880: 2020 2061 7761 6974 2073 6c65 6570 2831     await sleep(1
-00000890: 295c 6e5c 6e20 2020 205c 6e72 756e 2873  )\n\n    \nrun(s
-000008a0: 6c65 6570 5f6f 6e65 5f73 6563 2829 295c  leep_one_sec())\
-000008b0: 6e5c 6e60 6060 5c6e 4f75 7470 7574 3a5c  n\n```\nOutput:\
-000008c0: 6e60 6060 5c6e 5469 6d65 6f75 7445 7272  n```\nTimeoutErr
-000008d0: 6f72 5c6e 6060 605c 6e27 2c0a 2020 2020  or\n```\n',.    
-000008e0: 2761 7574 686f 7227 3a20 2741 7474 696c  'author': 'Attil
-000008f0: 6120 4475 6461 7327 2c0a 2020 2020 2761  a Dudas',.    'a
-00000900: 7574 686f 725f 656d 6169 6c27 3a20 2764  uthor_email': 'd
-00000910: 7564 6173 6137 4067 6d61 696c 2e63 6f6d  udasa7@gmail.com
-00000920: 272c 0a20 2020 2027 6d61 696e 7461 696e  ',.    'maintain
-00000930: 6572 273a 2027 4e6f 6e65 272c 0a20 2020  er': 'None',.   
-00000940: 2027 6d61 696e 7461 696e 6572 5f65 6d61   'maintainer_ema
-00000950: 696c 273a 2027 4e6f 6e65 272c 0a20 2020  il': 'None',.   
-00000960: 2027 7572 6c27 3a20 2768 7474 7073 3a2f   'url': 'https:/
-00000970: 2f67 6974 6875 622e 636f 6d2f 4441 7465  /github.com/DAte
-00000980: 6b2f 6461 7465 6b2d 6170 702d 7574 696c  k/datek-app-util
-00000990: 732f 272c 0a20 2020 2027 7061 636b 6167  s/',.    'packag
-000009a0: 6573 273a 2070 6163 6b61 6765 732c 0a20  es': packages,. 
-000009b0: 2020 2027 7061 636b 6167 655f 6461 7461     'package_data
-000009c0: 273a 2070 6163 6b61 6765 5f64 6174 612c  ': package_data,
-000009d0: 0a20 2020 2027 7079 7468 6f6e 5f72 6571  .    'python_req
-000009e0: 7569 7265 7327 3a20 273e 3d33 2e38 2c3c  uires': '>=3.8,<
-000009f0: 342e 3027 2c0a 7d0a 0a0a 7365 7475 7028  4.0',.}...setup(
-00000a00: 2a2a 7365 7475 705f 6b77 6172 6773 290a  **setup_kwargs).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6461 7465  : 2.1.Name: date
+00000020: 6b5f 6170 705f 7574 696c 730a 5665 7273  k_app_utils.Vers
+00000030: 696f 6e3a 2030 2e33 2e36 0a53 756d 6d61  ion: 0.3.6.Summa
+00000040: 7279 3a20 5574 696c 6974 6965 7320 666f  ry: Utilities fo
+00000050: 7220 6275 696c 6469 6e67 2061 7070 6c69  r building appli
+00000060: 6361 7469 6f6e 730a 486f 6d65 2d70 6167  cations.Home-pag
+00000070: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
+00000080: 622e 636f 6d2f 4441 7465 6b2f 6461 7465  b.com/DAtek/date
+00000090: 6b2d 6170 702d 7574 696c 732f 0a4c 6963  k-app-utils/.Lic
+000000a0: 656e 7365 3a20 4d49 540a 4175 7468 6f72  ense: MIT.Author
+000000b0: 3a20 4174 7469 6c61 2044 7564 6173 0a41  : Attila Dudas.A
+000000c0: 7574 686f 722d 656d 6169 6c3a 2064 7564  uthor-email: dud
+000000d0: 6173 6137 4067 6d61 696c 2e63 6f6d 0a52  asa7@gmail.com.R
+000000e0: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
+000000f0: 3e3d 332e 382c 3c33 2e31 330a 436c 6173  >=3.8,<3.13.Clas
+00000100: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
+00000110: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000120: 3a3a 204d 4954 204c 6963 656e 7365 0a43  :: MIT License.C
+00000130: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000140: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000150: 3a3a 2050 7974 686f 6e20 3a3a 2033 0a43  :: Python :: 3.C
+00000160: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000170: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000180: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+00000190: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000001a0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001b0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001c0: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
+000001d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000001e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000001f0: 2033 2e31 300a 436c 6173 7369 6669 6572   3.10.Classifier
+00000200: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000210: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000220: 203a 3a20 332e 3131 0a43 6c61 7373 6966   :: 3.11.Classif
+00000230: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000240: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000250: 686f 6e20 3a3a 2033 2e31 320a 5072 6f6a  hon :: 3.12.Proj
+00000260: 6563 742d 5552 4c3a 2052 6570 6f73 6974  ect-URL: Reposit
+00000270: 6f72 792c 2068 7474 7073 3a2f 2f67 6974  ory, https://git
+00000280: 6875 622e 636f 6d2f 4441 7465 6b2f 6461  hub.com/DAtek/da
+00000290: 7465 6b2d 6170 702d 7574 696c 732f 0a44  tek-app-utils/.D
+000002a0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
+000002b0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
+000002c0: 726b 646f 776e 0a0a 5b21 5b63 6f64 6563  rkdown..[![codec
+000002d0: 6f76 5d28 6874 7470 733a 2f2f 636f 6465  ov](https://code
+000002e0: 636f 762e 696f 2f67 682f 4441 7465 6b2f  cov.io/gh/DAtek/
+000002f0: 6461 7465 6b2d 6170 702d 7574 696c 732f  datek-app-utils/
+00000300: 6772 6170 682f 6261 6467 652e 7376 673f  graph/badge.svg?
+00000310: 746f 6b65 6e3d 5552 3047 3049 3431 4c44  token=UR0G0I41LD
+00000320: 295d 2868 7474 7073 3a2f 2f63 6f64 6563  )](https://codec
+00000330: 6f76 2e69 6f2f 6768 2f44 4174 656b 2f64  ov.io/gh/DAtek/d
+00000340: 6174 656b 2d61 7070 2d75 7469 6c73 290a  atek-app-utils).
+00000350: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000360: 2f67 6974 6875 622e 636f 6d2f 7073 662f  /github.com/psf/
+00000370: 626c 6163 6b22 3e3c 696d 6720 616c 743d  black"><img alt=
+00000380: 2243 6f64 6520 7374 796c 653a 2062 6c61  "Code style: bla
+00000390: 636b 2220 7372 633d 2268 7474 7073 3a2f  ck" src="https:/
+000003a0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000003b0: 6261 6467 652f 636f 6465 2532 3073 7479  badge/code%20sty
+000003c0: 6c65 2d62 6c61 636b 2d30 3030 3030 302e  le-black-000000.
+000003d0: 7376 6722 3e3c 2f61 3e0a 3c61 2068 7265  svg"></a>.<a hre
+000003e0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+000003f0: 622e 636f 6d2f 7073 662f 626c 6163 6b2f  b.com/psf/black/
+00000400: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
+00000410: 4522 3e3c 696d 6720 616c 743d 224c 6963  E"><img alt="Lic
+00000420: 656e 7365 3a20 4d49 5422 2073 7263 3d22  ense: MIT" src="
+00000430: 6874 7470 733a 2f2f 626c 6163 6b2e 7265  https://black.re
+00000440: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00000450: 7374 6162 6c65 2f5f 7374 6174 6963 2f6c  stable/_static/l
+00000460: 6963 656e 7365 2e73 7667 223e 3c2f 613e  icense.svg"></a>
+00000470: 0a0a 2320 5574 696c 6974 6965 7320 666f  ..# Utilities fo
+00000480: 7220 6275 696c 6469 6e67 2061 7070 6c69  r building appli
+00000490: 6361 7469 6f6e 732e 0a0a 2323 2043 6f6e  cations...## Con
+000004a0: 7461 696e 733a 0a2d 2043 6f6e 6669 6720  tains:.- Config 
+000004b0: 6c6f 6164 696e 6720 6672 6f6d 2065 6e76  loading from env
+000004c0: 6972 6f6e 6d65 6e74 0a2d 2042 6f6f 7473  ironment.- Boots
+000004d0: 7472 6170 2066 6f72 206c 6f67 6769 6e67  trap for logging
+000004e0: 0a2d 2042 6173 6520 636c 6173 7320 666f  .- Base class fo
+000004f0: 7220 6372 6561 7469 6e67 2061 7379 6e63  r creating async
+00000500: 2077 6f72 6b65 7273 0a2d 2041 7379 6e63   workers.- Async
+00000510: 2074 696d 656f 7574 2064 6563 6f72 6174   timeout decorat
+00000520: 6f72 2c20 7768 6963 6820 6973 2076 6572  or, which is ver
+00000530: 7920 7573 6566 756c 2066 6f72 2077 7269  y useful for wri
+00000540: 7469 6e67 2061 7379 6e63 2074 6573 7473  ting async tests
+00000550: 0a0a 2323 2045 7861 6d70 6c65 733a 0a0a  ..## Examples:..
+00000560: 2323 2320 456e 7620 636f 6e66 6967 0a60  ### Env config.`
+00000570: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+00000580: 6f73 0a0a 6672 6f6d 2064 6174 656b 5f61  os..from datek_a
+00000590: 7070 5f75 7469 6c73 2e65 6e76 5f63 6f6e  pp_utils.env_con
+000005a0: 6669 672e 6261 7365 2069 6d70 6f72 7420  fig.base import 
+000005b0: 4261 7365 436f 6e66 6967 0a0a 6f73 2e65  BaseConfig..os.e
+000005c0: 6e76 6972 6f6e 5b22 434f 4c4f 5222 5d20  nviron["COLOR"] 
+000005d0: 3d20 2252 4544 220a 6f73 2e65 6e76 6972  = "RED".os.envir
+000005e0: 6f6e 5b22 5445 4d50 4552 4154 5552 4522  on["TEMPERATURE"
+000005f0: 5d20 3d20 2235 3022 0a0a 0a63 6c61 7373  ] = "50"...class
+00000600: 2043 6f6e 6669 6728 4261 7365 436f 6e66   Config(BaseConf
+00000610: 6967 293a 0a20 2020 2043 4f4c 4f52 3a20  ig):.    COLOR: 
+00000620: 7374 720a 2020 2020 5445 4d50 4552 4154  str.    TEMPERAT
+00000630: 5552 453a 2069 6e74 0a0a 0a61 7373 6572  URE: int...asser
+00000640: 7420 436f 6e66 6967 2e43 4f4c 4f52 203d  t Config.COLOR =
+00000650: 3d20 2252 4544 220a 6173 7365 7274 2043  = "RED".assert C
+00000660: 6f6e 6669 672e 5445 4d50 4552 4154 5552  onfig.TEMPERATUR
+00000670: 4520 3d3d 2035 300a 6060 600a 0a54 6865  E == 50.```..The
+00000680: 2060 436f 6e66 6967 6020 636c 6173 7320   `Config` class 
+00000690: 6361 7374 7320 7468 6520 7661 6c75 6573  casts the values
+000006a0: 2061 7574 6f6d 6174 6963 616c 6c79 2e0a   automatically..
+000006b0: 4d6f 7265 6f76 6572 2c20 796f 7520 6361  Moreover, you ca
+000006c0: 6e20 7465 7374 2077 6865 7468 6572 2061  n test whether a
+000006d0: 6c6c 2074 6865 206d 616e 6461 746f 7279  ll the mandatory
+000006e0: 2076 6172 6961 626c 6573 2068 6176 6520   variables have 
+000006f0: 6265 656e 2073 6574 206f 7220 6e6f 742e  been set or not.
+00000700: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+00000710: 7274 206f 730a 0a66 726f 6d20 6461 7465  rt os..from date
+00000720: 6b5f 6170 705f 7574 696c 732e 656e 765f  k_app_utils.env_
+00000730: 636f 6e66 6967 2e62 6173 6520 696d 706f  config.base impo
+00000740: 7274 2042 6173 6543 6f6e 6669 670a 6672  rt BaseConfig.fr
+00000750: 6f6d 2064 6174 656b 5f61 7070 5f75 7469  om datek_app_uti
+00000760: 6c73 2e65 6e76 5f63 6f6e 6669 672e 7574  ls.env_config.ut
+00000770: 696c 7320 696d 706f 7274 2076 616c 6964  ils import valid
+00000780: 6174 655f 636f 6e66 6967 0a66 726f 6d20  ate_config.from 
+00000790: 6461 7465 6b5f 6170 705f 7574 696c 732e  datek_app_utils.
+000007a0: 656e 765f 636f 6e66 6967 2e65 7272 6f72  env_config.error
+000007b0: 7320 696d 706f 7274 2056 616c 6964 6174  s import Validat
+000007c0: 696f 6e45 7272 6f72 0a0a 6f73 2e65 6e76  ionError..os.env
+000007d0: 6972 6f6e 5b22 434f 4c4f 5222 5d20 3d20  iron["COLOR"] = 
+000007e0: 2252 4544 220a 0a0a 636c 6173 7320 436f  "RED"...class Co
+000007f0: 6e66 6967 2842 6173 6543 6f6e 6669 6729  nfig(BaseConfig)
+00000800: 3a0a 2020 2020 434f 4c4f 523a 2073 7472  :.    COLOR: str
+00000810: 0a20 2020 2054 454d 5045 5241 5455 5245  .    TEMPERATURE
+00000820: 3a20 696e 740a 2020 2020 414d 4f55 4e54  : int.    AMOUNT
+00000830: 3a20 696e 7420 3d20 4e6f 6e65 0a0a 0a74  : int = None...t
+00000840: 7279 3a0a 2020 2020 7661 6c69 6461 7465  ry:.    validate
+00000850: 5f63 6f6e 6669 6728 436f 6e66 6967 290a  _config(Config).
+00000860: 6578 6365 7074 2056 616c 6964 6174 696f  except Validatio
+00000870: 6e45 7272 6f72 2061 7320 6572 726f 723a  nError as error:
+00000880: 0a20 2020 2066 6f72 2061 7474 7269 6275  .    for attribu
+00000890: 7465 5f65 7272 6f72 2069 6e20 6572 726f  te_error in erro
+000008a0: 722e 6572 726f 7273 3a0a 2020 2020 2020  r.errors:.      
+000008b0: 2020 7072 696e 7428 6174 7472 6962 7574    print(attribut
+000008c0: 655f 6572 726f 7229 0a0a 6060 600a 4f75  e_error)..```.Ou
+000008d0: 7470 7574 3a0a 6060 600a 5445 4d50 4552  tput:.```.TEMPER
+000008e0: 4154 5552 453a 204e 6f74 2073 6574 2e20  ATURE: Not set. 
+000008f0: 5265 7175 6972 6564 2074 7970 653a 203c  Required type: <
+00000900: 636c 6173 7320 2769 6e74 273e 0a60 6060  class 'int'>.```
+00000910: 0a0a 2323 2320 4173 796e 6320 7469 6d65  ..### Async time
+00000920: 6f75 7420 6465 636f 7261 746f 720a 0a60  out decorator..`
+00000930: 6060 7079 7468 6f6e 0a66 726f 6d20 6173  ``python.from as
+00000940: 796e 6369 6f20 696d 706f 7274 2073 6c65  yncio import sle
+00000950: 6570 2c20 7275 6e0a 6672 6f6d 2064 6174  ep, run.from dat
+00000960: 656b 5f61 7070 5f75 7469 6c73 2e61 7379  ek_app_utils.asy
+00000970: 6e63 5f75 7469 6c73 2069 6d70 6f72 7420  nc_utils import 
+00000980: 6173 796e 635f 7469 6d65 6f75 740a 0a0a  async_timeout...
+00000990: 4061 7379 6e63 5f74 696d 656f 7574 2830  @async_timeout(0
+000009a0: 2e31 290a 6173 796e 6320 6465 6620 736c  .1).async def sl
+000009b0: 6565 705f 6f6e 655f 7365 6328 293a 0a20  eep_one_sec():. 
+000009c0: 2020 2061 7761 6974 2073 6c65 6570 2831     await sleep(1
+000009d0: 290a 0a20 2020 200a 7275 6e28 736c 6565  )..    .run(slee
+000009e0: 705f 6f6e 655f 7365 6328 2929 0a0a 6060  p_one_sec())..``
+000009f0: 600a 4f75 7470 7574 3a0a 6060 600a 5469  `.Output:.```.Ti
+00000a00: 6d65 6f75 7445 7272 6f72 0a60 6060 0a0a  meoutError.```..
```


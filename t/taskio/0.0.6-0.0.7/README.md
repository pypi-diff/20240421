# Comparing `tmp/taskio-0.0.6.tar.gz` & `tmp/taskio-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskio-0.0.6.tar", last modified: Sat Nov 25 19:48:23 2023, max compression
+gzip compressed data, was "taskio-0.0.7.tar", last modified: Sun Apr 21 03:06:03 2024, max compression
```

## Comparing `taskio-0.0.6.tar` & `taskio-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-11-25 19:48:23.238778 taskio-0.0.6/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    11348 2023-06-16 04:03:25.000000 taskio-0.0.6/LICENSE
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       57 2023-11-25 19:44:49.000000 taskio-0.0.6/MANIFEST.in
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1289 2023-11-25 19:48:23.238778 taskio-0.0.6/PKG-INFO
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      149 2023-06-16 04:03:25.000000 taskio-0.0.6/README.md
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-11-25 19:48:23.236778 taskio-0.0.6/requirements/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       27 2023-11-25 18:38:52.000000 taskio-0.0.6/requirements/basic.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       38 2023-11-25 19:48:23.238778 taskio-0.0.6/setup.cfg
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2877 2023-11-25 19:45:20.000000 taskio-0.0.6/setup.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-11-25 19:48:23.237778 taskio-0.0.6/taskio/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1376 2023-11-25 18:38:09.000000 taskio-0.0.6/taskio/__init__.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      878 2023-06-16 04:03:25.000000 taskio-0.0.6/taskio/config.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     7939 2023-08-22 04:11:12.000000 taskio-0.0.6/taskio/core.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3611 2023-08-22 03:40:16.000000 taskio-0.0.6/taskio/decorators.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3719 2023-08-22 04:12:42.000000 taskio-0.0.6/taskio/process.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-11-25 19:48:23.238778 taskio-0.0.6/taskio.egg-info/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1289 2023-11-25 19:48:23.000000 taskio-0.0.6/taskio.egg-info/PKG-INFO
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      300 2023-11-25 19:48:23.000000 taskio-0.0.6/taskio.egg-info/SOURCES.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        1 2023-11-25 19:48:23.000000 taskio-0.0.6/taskio.egg-info/dependency_links.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       27 2023-11-25 19:48:23.000000 taskio-0.0.6/taskio.egg-info/requires.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        7 2023-11-25 19:48:23.000000 taskio-0.0.6/taskio.egg-info/top_level.txt
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-21 03:06:03.735699 taskio-0.0.7/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    11348 2024-04-20 22:13:21.000000 taskio-0.0.7/LICENSE
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       57 2024-04-20 22:13:12.000000 taskio-0.0.7/MANIFEST.in
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1240 2024-04-21 03:06:03.735699 taskio-0.0.7/PKG-INFO
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      149 2024-04-20 22:13:12.000000 taskio-0.0.7/README.md
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-21 03:06:03.733698 taskio-0.0.7/requirements/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       27 2024-04-20 22:13:12.000000 taskio-0.0.7/requirements/basic.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       38 2024-04-21 03:06:03.735699 taskio-0.0.7/setup.cfg
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2706 2024-04-20 22:20:36.000000 taskio-0.0.7/setup.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-21 03:06:03.733698 taskio-0.0.7/taskio/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1376 2024-04-21 03:05:19.000000 taskio-0.0.7/taskio/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      896 2024-04-20 22:13:21.000000 taskio-0.0.7/taskio/config.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     6674 2024-04-20 22:13:21.000000 taskio-0.0.7/taskio/core.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3611 2024-04-20 22:13:12.000000 taskio-0.0.7/taskio/decorators.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3760 2024-04-20 22:13:21.000000 taskio-0.0.7/taskio/process.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-21 03:06:03.734698 taskio-0.0.7/taskio.egg-info/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1240 2024-04-21 03:06:03.000000 taskio-0.0.7/taskio.egg-info/PKG-INFO
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      300 2024-04-21 03:06:03.000000 taskio-0.0.7/taskio.egg-info/SOURCES.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        1 2024-04-21 03:06:03.000000 taskio-0.0.7/taskio.egg-info/dependency_links.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       27 2024-04-21 03:06:03.000000 taskio-0.0.7/taskio.egg-info/requires.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        7 2024-04-21 03:06:03.000000 taskio-0.0.7/taskio.egg-info/top_level.txt
```

### Comparing `taskio-0.0.6/LICENSE` & `taskio-0.0.7/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2019-2023 Flavio Garcia
+   Copyright 2019-2024 Flavio Garcia
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `taskio-0.0.6/PKG-INFO` & `taskio-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: taskio
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python library for command-line argument processing.
 Home-page: https://github.com/candango/taskio
 Author: Flavio Garcia
 Author-email: piraz@candango.org
 Maintainer: Flavio Garcia
 Maintainer-email: piraz@candango.org
 License: Apache License V2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >= 3.6
+Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cartola>=0.17
 Requires-Dist: click==8.1.7
 
 # Candango Taskio
```

### Comparing `taskio-0.0.6/taskio/__init__.py` & `taskio-0.0.7/taskio/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 __author__ = "Flavio Garcia <piraz@candango.org>"
 __description__ = "A Python library for command-line argument processing."
-__version__ = (0, 0, 6)
+__version__ = (0, 0, 7)
 __licence__ = "Apache License V2.0"
 
 
 def get_version():
     return ".".join(map(str, __version__))
```

### Comparing `taskio-0.0.6/taskio/config.py` & `taskio-0.0.7/taskio/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from cartola.config import get_from_string
 
 
-def resolve_reference(reference):
+def resolve_reference(reference, **kwargs):
     if reference is not None:
         result = get_from_string(reference)
         if result is not None:
             if callable(result):
-                return result()
+                return result(**kwargs)
             return result
     return reference
```

### Comparing `taskio-0.0.6/taskio/core.py` & `taskio-0.0.7/taskio/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,32 @@
-# Copyright 2019-2023 Flavio Garcia
+# Copyright 2019-2024 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import sys
 
 from . import process
 import click
 from click.core import Command, Context, Group, HelpFormatter
 import typing as t
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Callable, List, Optional
+import sys
 
 
 class TaskioContext(Context):
 
-    def __init__(
-            self,
-            command: Command,
-            parent: Optional[Context] = None,
-            info_name: Optional[str] = None,
-            obj: Optional[Any] = None,
-            auto_envvar_prefix: Optional[str] = None,
-            default_map: Optional[Dict[str, Any]] = None,
-            terminal_width: Optional[int] = None,
-            max_content_width: Optional[int] = None,
-            resilient_parsing: bool = False,
-            allow_extra_args: Optional[bool] = None,
-            allow_interspersed_args: Optional[bool] = None,
-            ignore_unknown_options: Optional[bool] = None,
-            help_option_names: Optional[List[str]] = None,
-            token_normalize_func: Optional[Callable[[str], str]] = None,
-            color: Optional[bool] = None,
-            show_default: Optional[bool] = None,
-    ) -> None:
-        super().__init__(command, parent, info_name, obj, auto_envvar_prefix,
-                         default_map, terminal_width, max_content_width,
-                         resilient_parsing, allow_extra_args,
-                         allow_interspersed_args, ignore_unknown_options,
-                         help_option_names, token_normalize_func, color,
-                         show_default)
-        self.loader = None
+    loader: process.TaskioLoader
 
 
 class TaskioRootGroup(Group):
 
     def __init__(
         self,
         name: t.Optional[str] = None,
```

### Comparing `taskio-0.0.6/taskio/decorators.py` & `taskio-0.0.7/taskio/decorators.py`

 * *Files identical despite different names*

### Comparing `taskio-0.0.6/taskio/process.py` & `taskio-0.0.7/taskio/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,54 @@
-# Copyright 2019-2023 Flavio Garcia
+# Copyright 2019-2024 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
+
 
 from .config import resolve_reference
-from . import core
 from cartola import sysexits
 import importlib
 import logging
 import sys
+import typing
 
+if typing.TYPE_CHECKING:
+    from core import TaskioRootGroup
 
 logger = logging.getLogger(__name__)
 
 
 class TaskioLoader(object):
 
     _conf: dict
-    _description: str | None
-    _name: str | None
+    _description: str
+    _name: str
     _root: str
-    _program: "core.TaskioRootGroup"
+    _program: TaskioRootGroup
     _sources: list
-    _version: str | None
+    _version: str
 
-    def __init__(self, conf, program=None, **kwargs):
+    def __init__(self, conf, program: TaskioRootGroup = None, **kwargs):
         self._conf = conf
         self._root = kwargs.get("root", "taskio")
         self._program = program
         self._sources = []
         if not self._conf:
-            print(
-                "Taskio FATAL ERROR:\n Please provide a configuration to the "
-                "command.")
+            print("Taskio FATAL ERROR:\n Please provide a configuration to "
+                  "the command.")
             sys.exit(sysexits.EX_FATAL_ERROR)
         if not self._root or self._root not in self._conf:
             print("Taskio FATAL ERROR:\n  Please add a root to the command "
                   "configuration")
             sys.exit(sysexits.EX_FATAL_ERROR)
 
     def load(self):
@@ -68,31 +71,31 @@
                 )
 
         if "sources" in self.conf:
             for source in self.conf['sources']:
                 self._sources.append(importlib.import_module(source))
 
     @property
-    def program(self) -> "core.TaskioRootGroup":
+    def program(self) -> TaskioRootGroup:
         return self._program
 
     @property
-    def name(self) -> str | None:
+    def name(self) -> str:
         if "program" in self.conf and "name" in self.conf['program']:
             return self.conf['program']['name']
         return None
 
     @property
-    def description(self) -> str | None:
+    def description(self) -> str:
         if "program" in self.conf and "description" in self.conf['program']:
             return self.conf['program']['description']
         return None
 
     @property
-    def version(self) -> str | None:
+    def version(self) -> str:
         if "program" in self.conf and "version" in self.conf['program']:
             return self.conf['program']['version']
         return None
 
     @property
     def full_name(self):
         if self.description:
```

### Comparing `taskio-0.0.6/taskio.egg-info/PKG-INFO` & `taskio-0.0.7/taskio.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: taskio
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python library for command-line argument processing.
 Home-page: https://github.com/candango/taskio
 Author: Flavio Garcia
 Author-email: piraz@candango.org
 Maintainer: Flavio Garcia
 Maintainer-email: piraz@candango.org
 License: Apache License V2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >= 3.6
+Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cartola>=0.17
 Requires-Dist: click==8.1.7
 
 # Candango Taskio
```


# Comparing `tmp/nog642_util-0.2.0.tar.gz` & `tmp/nog642_util-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/nog642/Documents/nog642-python-utils/nog642_util/dist/.tmp-bao2i_ic/nog642_util-0.2.0.tar", last modified: Sun Apr 21 04:35:30 2024, max compression
+gzip compressed data, was "nog642_util-0.2.1.tar", last modified: Sun Apr 21 04:58:04 2024, max compression
```

## Comparing `nog642_util-0.2.0.tar` & `nog642_util-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-21 04:35:30.957190 nog642_util-0.2.0/
--rw-r--r--   0 nog642    (1000) nog642    (1000)      572 2024-04-21 04:35:30.953190 nog642_util-0.2.0/PKG-INFO
--rw-rw-r--   0 nog642    (1000) nog642    (1000)       67 2024-04-20 21:16:31.000000 nog642_util-0.2.0/README.md
--rw-rw-r--   0 nog642    (1000) nog642    (1000)      597 2024-04-21 04:32:19.000000 nog642_util-0.2.0/pyproject.toml
--rw-rw-r--   0 nog642    (1000) nog642    (1000)       38 2024-04-21 04:35:30.957190 nog642_util-0.2.0/setup.cfg
-drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-21 04:35:30.953190 nog642_util-0.2.0/src/
-drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-21 04:35:30.953190 nog642_util-0.2.0/src/nog642_util/
--rw-rw-r--   0 nog642    (1000) nog642    (1000)    12842 2024-04-20 23:01:27.000000 nog642_util-0.2.0/src/nog642_util/__init__.py
-drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-21 04:35:30.953190 nog642_util-0.2.0/src/nog642_util.egg-info/
--rw-r--r--   0 nog642    (1000) nog642    (1000)      572 2024-04-21 04:35:30.000000 nog642_util-0.2.0/src/nog642_util.egg-info/PKG-INFO
--rw-rw-r--   0 nog642    (1000) nog642    (1000)      260 2024-04-21 04:35:30.000000 nog642_util-0.2.0/src/nog642_util.egg-info/SOURCES.txt
--rw-rw-r--   0 nog642    (1000) nog642    (1000)        1 2024-04-21 04:35:30.000000 nog642_util-0.2.0/src/nog642_util.egg-info/dependency_links.txt
--rw-rw-r--   0 nog642    (1000) nog642    (1000)       12 2024-04-21 04:35:30.000000 nog642_util-0.2.0/src/nog642_util.egg-info/top_level.txt
-drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-21 04:35:30.953190 nog642_util-0.2.0/tests/
--rw-rw-r--   0 nog642    (1000) nog642    (1000)      817 2024-04-20 23:13:32.000000 nog642_util-0.2.0/tests/test_StrEnum.py
--rw-rw-r--   0 nog642    (1000) nog642    (1000)     7006 2024-04-20 22:59:17.000000 nog642_util-0.2.0/tests/test_validate_schema.py
+drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-21 04:58:04.869524 nog642_util-0.2.1/
+-rw-r--r--   0 nog642    (1000) nog642    (1000)      573 2024-04-21 04:58:04.869524 nog642_util-0.2.1/PKG-INFO
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)       67 2024-04-20 21:16:31.000000 nog642_util-0.2.1/README.md
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)      598 2024-04-21 04:49:02.000000 nog642_util-0.2.1/pyproject.toml
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)       38 2024-04-21 04:58:04.869524 nog642_util-0.2.1/setup.cfg
+drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-21 04:58:04.865524 nog642_util-0.2.1/src/
+drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-21 04:58:04.865524 nog642_util-0.2.1/src/nog642_util/
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)    12880 2024-04-21 04:53:29.000000 nog642_util-0.2.1/src/nog642_util/__init__.py
+drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-21 04:58:04.869524 nog642_util-0.2.1/src/nog642_util.egg-info/
+-rw-r--r--   0 nog642    (1000) nog642    (1000)      573 2024-04-21 04:58:04.000000 nog642_util-0.2.1/src/nog642_util.egg-info/PKG-INFO
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)      260 2024-04-21 04:58:04.000000 nog642_util-0.2.1/src/nog642_util.egg-info/SOURCES.txt
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)        1 2024-04-21 04:58:04.000000 nog642_util-0.2.1/src/nog642_util.egg-info/dependency_links.txt
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)       12 2024-04-21 04:58:04.000000 nog642_util-0.2.1/src/nog642_util.egg-info/top_level.txt
+drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-21 04:58:04.865524 nog642_util-0.2.1/tests/
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)      817 2024-04-21 04:39:39.000000 nog642_util-0.2.1/tests/test_StrEnum.py
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)     7006 2024-04-21 04:39:39.000000 nog642_util-0.2.1/tests/test_validate_schema.py
```

### Comparing `nog642_util-0.2.0/PKG-INFO` & `nog642_util-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: nog642_util
-Version: 0.2.0
+Version: 0.2.1
 Summary: Various utilities for python.
 Author-email: nog642 <nog642.contact@gmail.com>
 Project-URL: Homepage, https://gitlab.com/nog642-org/nog642-python-utils
 Project-URL: Issues, https://gitlab.com/nog642-org/nog642-python-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # nog642_util
 
 This package contains various utilities for Python.
```

### Comparing `nog642_util-0.2.0/pyproject.toml` & `nog642_util-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nog642_util"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="nog642", email="nog642.contact@gmail.com" },
 ]
 description = "Various utilities for python."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `nog642_util-0.2.0/src/nog642_util/__init__.py` & `nog642_util-0.2.1/src/nog642_util/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 from collections.abc import Collection, Sequence
-from enum import Enum, EnumMeta
+from enum import EnumType
+from enum import StrEnum as enum_StrEnum
 import inspect
 import json
 import sys
 import traceback
 import typing
 from typing import FrozenSet
 from typing import get_origin as typing_get_origin
 from typing import get_args as typing_get_args
 
 
-class _StrEnumMeta(EnumMeta):
+class _StrEnumMeta(EnumType):
     _StrEnum__member_set: FrozenSet[StrEnum]
 
     def __new__(metacls, name, bases, attrs):
-        cls = EnumMeta.__new__(metacls, name, bases, attrs)
+        cls = EnumType.__new__(metacls, name, bases, attrs)
         if len(cls) > 0:  # if the class has any members
             member_set_attr_name = '_StrEnum__member_set'
             if hasattr(cls, member_set_attr_name):
                 raise ValueError(f'StrEnum cannot define value __value_set; '
                                  f'already defined as {getattr(cls, member_set_attr_name)}')
             setattr(cls, member_set_attr_name, frozenset(cls.__members__.values()))
         return cls
 
     def __contains__(cls, item):
         if isinstance(item, cls):
             return True
         return item in cls._StrEnum__member_set
 
 
-class StrEnum(str, Enum, metaclass=_StrEnumMeta):
+class StrEnum(enum_StrEnum, metaclass=_StrEnumMeta):
     """
     To be used for basic string enums.
 
     Major change is that enum instances now compare equal to the string value,
     as opposed to plain enums (because of the str mixin).
 
     Whether a string is a valid enum can be checked using the `in` operator on
```

### Comparing `nog642_util-0.2.0/src/nog642_util.egg-info/PKG-INFO` & `nog642_util-0.2.1/src/nog642_util.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: nog642_util
-Version: 0.2.0
+Version: 0.2.1
 Summary: Various utilities for python.
 Author-email: nog642 <nog642.contact@gmail.com>
 Project-URL: Homepage, https://gitlab.com/nog642-org/nog642-python-utils
 Project-URL: Issues, https://gitlab.com/nog642-org/nog642-python-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # nog642_util
 
 This package contains various utilities for Python.
```

### Comparing `nog642_util-0.2.0/tests/test_StrEnum.py` & `nog642_util-0.2.1/tests/test_StrEnum.py`

 * *Files identical despite different names*

### Comparing `nog642_util-0.2.0/tests/test_validate_schema.py` & `nog642_util-0.2.1/tests/test_validate_schema.py`

 * *Files identical despite different names*


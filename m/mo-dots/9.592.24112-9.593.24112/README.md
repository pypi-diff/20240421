# Comparing `tmp/mo_dots-9.592.24112.tar.gz` & `tmp/mo_dots-9.593.24112.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_dots-9.592.24112.tar", last modified: Sun Apr 21 14:32:02 2024, max compression
+gzip compressed data, was "mo_dots-9.593.24112.tar", last modified: Sun Apr 21 15:00:29 2024, max compression
```

## Comparing `mo_dots-9.592.24112.tar` & `mo_dots-9.593.24112.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 14:32:02.465541 mo_dots-9.592.24112/
--rw-rw-rw-   0        0        0    16725 2022-02-13 20:11:16.000000 mo_dots-9.592.24112/LICENSE
--rw-rw-rw-   0        0        0     5055 2024-04-21 14:32:02.464522 mo_dots-9.592.24112/PKG-INFO
--rw-rw-rw-   0        0        0     3549 2024-04-04 03:46:45.000000 mo_dots-9.592.24112/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 14:32:02.452795 mo_dots-9.592.24112/mo_dots/
--rw-rw-rw-   0        0        0    13989 2024-04-21 14:31:54.000000 mo_dots-9.592.24112/mo_dots/__init__.py
--rw-rw-rw-   0        0        0    16165 2024-04-21 14:31:54.000000 mo_dots-9.592.24112/mo_dots/datas.py
--rw-rw-rw-   0        0        0     4284 2024-03-16 18:16:18.000000 mo_dots-9.592.24112/mo_dots/fields.py
--rw-rw-rw-   0        0        0    10399 2024-04-21 14:31:54.000000 mo_dots-9.592.24112/mo_dots/lists.py
--rw-rw-rw-   0        0        0     6672 2024-04-21 14:31:54.000000 mo_dots-9.592.24112/mo_dots/nones.py
--rw-rw-rw-   0        0        0     5524 2024-04-21 14:31:54.000000 mo_dots-9.592.24112/mo_dots/objects.py
--rw-rw-rw-   0        0        0     1424 2024-03-14 10:01:33.000000 mo_dots-9.592.24112/mo_dots/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-21 14:32:02.462289 mo_dots-9.592.24112/mo_dots.egg-info/
--rw-rw-rw-   0        0        0     5055 2024-04-21 14:32:02.000000 mo_dots-9.592.24112/mo_dots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-04-21 14:32:02.000000 mo_dots-9.592.24112/mo_dots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 14:32:02.000000 mo_dots-9.592.24112/mo_dots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-21 02:12:28.000000 mo_dots-9.592.24112/mo_dots.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      241 2024-04-21 14:32:02.000000 mo_dots-9.592.24112/mo_dots.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-21 14:32:02.000000 mo_dots-9.592.24112/mo_dots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 14:32:02.465592 mo_dots-9.592.24112/setup.cfg
--rw-rw-rw-   0        0        0     4937 2024-04-21 14:31:57.000000 mo_dots-9.592.24112/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:00:29.524028 mo_dots-9.593.24112/
+-rw-rw-rw-   0        0        0    16725 2022-02-13 20:11:16.000000 mo_dots-9.593.24112/LICENSE
+-rw-rw-rw-   0        0        0     5055 2024-04-21 15:00:29.522959 mo_dots-9.593.24112/PKG-INFO
+-rw-rw-rw-   0        0        0     3549 2024-04-04 03:46:45.000000 mo_dots-9.593.24112/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 15:00:29.511287 mo_dots-9.593.24112/mo_dots/
+-rw-rw-rw-   0        0        0    13962 2024-04-21 15:00:21.000000 mo_dots-9.593.24112/mo_dots/__init__.py
+-rw-rw-rw-   0        0        0    16249 2024-04-21 15:00:21.000000 mo_dots-9.593.24112/mo_dots/datas.py
+-rw-rw-rw-   0        0        0     4283 2024-04-21 15:00:21.000000 mo_dots-9.593.24112/mo_dots/fields.py
+-rw-rw-rw-   0        0        0    10399 2024-04-21 15:00:21.000000 mo_dots-9.593.24112/mo_dots/lists.py
+-rw-rw-rw-   0        0        0     6663 2024-04-21 15:00:21.000000 mo_dots-9.593.24112/mo_dots/nones.py
+-rw-rw-rw-   0        0        0     5371 2024-04-21 15:00:21.000000 mo_dots-9.593.24112/mo_dots/objects.py
+-rw-rw-rw-   0        0        0     1423 2024-04-21 15:00:21.000000 mo_dots-9.593.24112/mo_dots/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:00:29.519934 mo_dots-9.593.24112/mo_dots.egg-info/
+-rw-rw-rw-   0        0        0     5055 2024-04-21 15:00:29.000000 mo_dots-9.593.24112/mo_dots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-04-21 15:00:29.000000 mo_dots-9.593.24112/mo_dots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 15:00:29.000000 mo_dots-9.593.24112/mo_dots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-21 02:12:28.000000 mo_dots-9.593.24112/mo_dots.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      241 2024-04-21 15:00:29.000000 mo_dots-9.593.24112/mo_dots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-21 15:00:29.000000 mo_dots-9.593.24112/mo_dots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 15:00:29.524028 mo_dots-9.593.24112/setup.cfg
+-rw-rw-rw-   0        0        0     4937 2024-04-21 15:00:24.000000 mo_dots-9.593.24112/setup.py
```

### Comparing `mo_dots-9.592.24112/LICENSE` & `mo_dots-9.593.24112/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_dots-9.592.24112/PKG-INFO` & `mo_dots-9.593.24112/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.592.24112
+Version: 9.593.24112
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
@@ -16,21 +16,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mo-future==7.584.24095
 Requires-Dist: mo-imports==7.584.24095
 Provides-Extra: tests
-Requires-Dist: mo-logs>=8.562.24075; extra == "tests"
-Requires-Dist: mo-json>=6.562.24075; extra == "tests"
-Requires-Dist: mo-threads>=6.562.24075; extra == "tests"
-Requires-Dist: mo-testing>=7.562.24075; extra == "tests"
+Requires-Dist: mo-logs>=8.584.24095; extra == "tests"
+Requires-Dist: mo-json>=6.589.24111; extra == "tests"
+Requires-Dist: mo-threads>=6.589.24111; extra == "tests"
+Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 Requires-Dist: pyLibrary>=3.264.22338; extra == "tests"
-Requires-Dist: mo-math>=7.562.24075; extra == "tests"
-Requires-Dist: mo-times>=5.562.24075; extra == "tests"
+Requires-Dist: mo-math>=7.589.24111; extra == "tests"
+Requires-Dist: mo-times>=5.589.24111; extra == "tests"
 Requires-Dist: jx-elasticsearch>=3.99.20292; extra == "tests"
 
 
 # More Dots!
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mo-dots.svg)](https://pypi.org/project/mo-dots/)
 [![Build Status](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml)
```

### Comparing `mo_dots-9.592.24112/README.md` & `mo_dots-9.593.24112/README.md`

 * *Files identical despite different names*

### Comparing `mo_dots-9.592.24112/mo_dots/__init__.py` & `mo_dots-9.593.24112/mo_dots/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from mo_dots.datas import *
 from mo_dots.fields import *
 from mo_dots.lists import *
 from mo_dots.nones import *
 from mo_dots.objects import DataObject, DataClass, object_to_data
 from mo_dots.utils import get_module, CLASS, get_logger, SLOT
 
-
 __all__ = [
     "coalesce",
     "concat_field",
     "Data",
     "DataClass",
     "DataObject",
     "datawrap",
@@ -323,15 +322,15 @@
 
     attr_name = path[-1]
 
     # ACTUAL SETTING OF VALUE
     try:
         old_value = _get_attr(obj, [attr_name])
         old_type = _get(old_value, CLASS)
-        if old_value == None or old_type in (bool, int, float, text, binary_type):
+        if old_value == None or old_type in primitive_types:
             old_value = None
             new_value = value
         elif value == None:
             new_value = None
         else:
             new_value = _get(old_value, CLASS)(value)  # TRY TO MAKE INSTANCE OF SAME CLASS
     except Exception:
@@ -349,16 +348,14 @@
             get_logger().error(PATH_NOT_FOUND, cause=[f, e])
 
 
 def lower_match(value, candidates):
     return [v for v in candidates if v.lower() == value.lower()]
 
 
-
-
 def to_data(v=None) -> object:
     """
     WRAP AS Data OBJECT FOR DATA PROCESSING: https://github.com/klahnakoski/mo-dots/tree/dev/docs
     :param v:  THE VALUE TO WRAP
     :return:  Data INSTANCE
     """
 
@@ -379,16 +376,14 @@
     else:
         return v
 
 
 wrap = to_data
 
 
-
-
 def from_data(v):
     if v is None:
         return None
     _type = _get(v, CLASS)
     if _type is NullType:
         return None
     elif _type is Data:
```

### Comparing `mo_dots-9.592.24112/mo_dots/datas.py` & `mo_dots-9.593.24112/mo_dots/datas.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
 from copy import copy, deepcopy
+from datetime import datetime, date
 from decimal import Decimal
 
 from mo_future import (
     generator_types,
     iteritems,
     long,
     text,
     MutableMapping,
     OrderedDict,
     first,
-    binary_type,
 )
 from mo_imports import expect
 
 from mo_dots.fields import split_field, literal_field, concat_field
 from mo_dots.nones import Null, NullType, null_types
 from mo_dots.utils import CLASS, SLOT
 from mo_dots.utils import get_logger
@@ -63,14 +63,16 @@
 
 _get = object.__getattribute__
 _set = object.__setattr__
 _new = object.__new__
 
 DEBUG = False
 
+primitive_types = (text, str, bytes, int, float, bool, Decimal, datetime, date)
+
 
 class Data(object):
     """
     Please see https://github.com/klahnakoski/mo-dots/tree/dev/docs#data-replaces-pythons-dict
     """
 
     __slots__ = [SLOT]
@@ -590,15 +592,15 @@
     """
     RETURN UNWRAPPED STRUCTURES
     """
     if value == None:
         return None
 
     class_ = _get(value, CLASS)
-    if class_ in (text, binary_type, int, float):
+    if class_ in primitive_types:
         return value
 
     if class_ in _data_types:
         if class_ is Data:
             value = from_data(value)
 
         output = {}
```

### Comparing `mo_dots-9.592.24112/mo_dots/fields.py` & `mo_dots-9.593.24112/mo_dots/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,8 +154,7 @@
         return join_field(field_path[common:])
 
     dots = "." * (len(parent_path) - common)
     if tail == ".":
         return "." + dots
     else:
         return "." + dots + tail
-
```

### Comparing `mo_dots-9.592.24112/mo_dots/lists.py` & `mo_dots-9.593.24112/mo_dots/lists.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
-
 import types
 from copy import deepcopy
 
 from mo_future import generator_types, first
 from mo_imports import expect, delay_import, export
 
 from mo_dots.datas import is_missing, hash_value
@@ -371,14 +370,15 @@
     """
     to_data, BUT WITHOUT CHECKS
     """
     output = _new(FlatList)
     _set(output, SLOT, v)
     return output
 
+
 def register_many(_type):
     global _many_types
     _many_types = _many_types + (_type,)
 
 
 export("mo_dots.datas", finite_types)
 export("mo_dots.datas", is_list)
```

### Comparing `mo_dots-9.592.24112/mo_dots/nones.py` & `mo_dots-9.593.24112/mo_dots/nones.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
-
 from mo_future import none_type
-from mo_imports import expect, export
+from mo_imports import expect
 
 from mo_dots.utils import CLASS, KEY, SLOT
 
 to_data, get_attr, is_sequence = expect("to_data", "get_attr", "is_sequence")
 
 _get = object.__getattribute__
 _set = object.__setattr__
@@ -84,15 +83,15 @@
     def __rmul__(self, other):
         return Null
 
     def __int__(self):
         return None
 
     def __float__(self):
-        return float('nan')
+        return float("nan")
 
     def __div__(self, other):
         return Null
 
     def __itruediv__(self, other):
         return Null
```

### Comparing `mo_dots-9.592.24112/mo_dots/objects.py` & `mo_dots-9.593.24112/mo_dots/objects.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,33 +2,21 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-
-
-
 from collections import OrderedDict
 from copy import deepcopy
-from datetime import date, datetime
-from decimal import Decimal
 
-from mo_future import (
-    binary_type,
-    generator_types,
-    get_function_arguments,
-    get_function_defaults,
-    text,
-    Mapping,
-)
+from mo_future import generator_types, get_function_arguments, get_function_defaults, Mapping
 from mo_imports import export, expect
 
-from mo_dots.datas import register_data, Data, _iadd, dict_to_data
+from mo_dots.datas import register_data, Data, _iadd, dict_to_data, primitive_types
 from mo_dots.lists import FlatList, list_to_data
 from mo_dots.nones import NullType, Null
 from mo_dots.utils import CLASS, SLOT, get_logger
 
 get_attr, set_attr, to_data, from_data, set_default = expect(
     "get_attr", "set_attr", "to_data", "from_data", "set_default"
 )
@@ -36,14 +24,15 @@
 _new = object.__new__
 _get = object.__getattribute__
 _set = object.__setattr__
 
 WRAPPED_CLASSES = set()
 known_types = {}  #  map from type to field names
 
+
 class DataObject(Mapping):
     """
     TREAT AN OBJECT LIKE DATA
     """
 
     __slots__ = [SLOT]
 
@@ -143,17 +132,15 @@
     try:
         keys = known_types[_type] = _type.__slots__
         return keys
     except Exception:
         pass
 
     keys = known_types[_type] = tuple(
-        k
-        for k in dir(_type)
-        if getattr(_type, k).__class__.__name__ in ['member_descriptor', 'getset_descriptor']
+        k for k in dir(_type) if getattr(_type, k).__class__.__name__ in ["member_descriptor", "getset_descriptor"]
     )
     return keys
 
 
 def object_to_data(v):
     try:
         if v == None:
@@ -169,15 +156,15 @@
         return m
     elif type_ is tuple:
         return list_to_data(v)
     elif type_ is list:
         return list_to_data(v)
     elif type_ in (Data, DataObject, FlatList, NullType):
         return v
-    elif type_ in (text, binary_type, int, float, Decimal, datetime, date):
+    elif type_ in primitive_types:
         return v
     elif type_ in generator_types:
         return (to_data(vv) for vv in v)
 
     return DataObject(v)
 
 
@@ -220,8 +207,8 @@
     output = {str(k): from_data(settings[k]) for k in params if k in settings}
     return output
 
 
 export("mo_dots.lists", object_to_data)
 export("mo_dots.datas", object_to_data)
 export("mo_dots.datas", DataObject)
-export("mo_dots.datas", get_keys)
+export("mo_dots.datas", get_keys)
```

### Comparing `mo_dots-9.592.24112/mo_dots/utils.py` & `mo_dots-9.593.24112/mo_dots/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
-
 import importlib
 
 from mo_future import STDOUT, STDERR
 
 KEY = str("_key")
 SLOT = str("_internal_value")
 CLASS = str("__class__")
```

### Comparing `mo_dots-9.592.24112/mo_dots.egg-info/PKG-INFO` & `mo_dots-9.593.24112/mo_dots.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.592.24112
+Version: 9.593.24112
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
@@ -16,21 +16,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mo-future==7.584.24095
 Requires-Dist: mo-imports==7.584.24095
 Provides-Extra: tests
-Requires-Dist: mo-logs>=8.562.24075; extra == "tests"
-Requires-Dist: mo-json>=6.562.24075; extra == "tests"
-Requires-Dist: mo-threads>=6.562.24075; extra == "tests"
-Requires-Dist: mo-testing>=7.562.24075; extra == "tests"
+Requires-Dist: mo-logs>=8.584.24095; extra == "tests"
+Requires-Dist: mo-json>=6.589.24111; extra == "tests"
+Requires-Dist: mo-threads>=6.589.24111; extra == "tests"
+Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 Requires-Dist: pyLibrary>=3.264.22338; extra == "tests"
-Requires-Dist: mo-math>=7.562.24075; extra == "tests"
-Requires-Dist: mo-times>=5.562.24075; extra == "tests"
+Requires-Dist: mo-math>=7.589.24111; extra == "tests"
+Requires-Dist: mo-times>=5.589.24111; extra == "tests"
 Requires-Dist: jx-elasticsearch>=3.99.20292; extra == "tests"
 
 
 # More Dots!
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mo-dots.svg)](https://pypi.org/project/mo-dots/)
 [![Build Status](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml)
```

### Comparing `mo_dots-9.592.24112/setup.py` & `mo_dots-9.593.24112/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # THIS FILE IS AUTOGENERATED!
 from setuptools import setup
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 5 - Production/Stable","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More Dots! Dot-access to Python dicts like Javascript',
-    extras_require={"tests":["mo-logs>=8.562.24075","mo-json>=6.562.24075","mo-threads>=6.562.24075","mo-testing>=7.562.24075","pyLibrary>=3.264.22338","mo-math>=7.562.24075","mo-times>=5.562.24075","jx-elasticsearch>=3.99.20292"]},
+    extras_require={"tests":["mo-logs>=8.584.24095","mo-json>=6.589.24111","mo-threads>=6.589.24111","mo-testing>=8.591.24112","pyLibrary>=3.264.22338","mo-math>=7.589.24111","mo-times>=5.589.24111","jx-elasticsearch>=3.99.20292"]},
     include_package_data=True,
     install_requires=["mo-future==7.584.24095","mo-imports==7.584.24095"],
     license='MPL 2.0',
     long_description='\n# More Dots!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-dots.svg)](https://pypi.org/project/mo-dots/)\n[![Build Status](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-dots/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-dots?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-dots/month)](https://pepy.tech/project/mo-dots)\n\n#### Changes in version 9.x.x\n\nEscaping a literal dot (`.`) is no longer (`\\\\.`) rather double-dot (`..`). Escaping a literal dot can still be done with bell (`\\b`) \n\n#### Changes in version 5.x.x\n\nThe `Data()` constructor only accepts keyword parameters. It no longer accepts a dict, nor does it attempt to clean the input.  Replace `Data(my_var)` with `to_data(my_var)`\n  \n\n## Overview\n\nThis library defines a `Data` class that can serve as a replacement for `dict`, and acts much like a null-safe dataclass.\n\n> See the [full documentation](https://github.com/klahnakoski/mo-dots/tree/dev/docs) for all the features of `mo-dots`\n\n### Create instances\n\nDefine `Data` using named parameters, just like you would a `dict`\n\n    >>> from mo_dots import Data\n    >>> Data(b=42, c="hello world")\n    Data({\'b\': 42, \'c\': \'hello world\'})\n\nYou can also wrap existing `dict`s so they can be used like `Data`\n\n    >>> from mo_dots import to_data\n    >>> to_data({\'b\': 42, \'c\': \'hello world\'})\n    Data({\'b\': 42, \'c\': \'hello world\'})\n\n### Dot Access\n\nAccess properties with attribute dots: `a.b == a["b"]`. You have probably seen this before.\n\n### Path Access\n\nAccess properties by dot-delimited path.\n\n\t>>> a = to_data({"b": {"c": 42}})\n\t>>> a["b.c"] == 42\n\tTrue\n\n### Safe Access\n\nIf a property does not exist then return `Null` rather than raising an error.\n\n\t>>> a = Data()\n\t>>> a.b == None\n\tTrue\n\t>>> a.b.c == None\n\tTrue\n\t>>> a[None] == None\n\tTrue\n\n### Path assignment\n\nNo need to make intermediate `dicts`\n\n    >>> a = Data()\n    >>> a["b.c"] = 42   # same as a.b.c = 42\n    a == {"b": {"c": 42}}\n\n### Path accumulation\n\nUse `+=` to add to a property; default zero (`0`)\n\n    >>> a = Data()\n    a == {}\n    >>> a.b.c += 1\n    a == {"b": {"c": 1}}\n    >>> a.b.c += 42\n    a == {"b": {"c": 43}}\n\nUse `+=` with a list (`[]`) to append to a list; default empty list (`[]`)\n\n    >>> a = Data()\n    a == {}\n    >>> a.b.c += [1]\n    a == {"b": {"c": [1]}}\n    >>> a.b.c += [42]\n    a == {"b": {"c": [1, 42]}}\n\n## Serializing to JSON\n\nThe standard Python JSON library does not recognize `Data` as serializable.  You may overcome this by providing `default=from_data`; which converts the data structures in this module into Python primitives of the same. \n\n    from mo_dots import from_data, to_data\n    \n    s = to_data({"a": ["b", 1]})\n    result = json.dumps(s, default=from_data)  \n\nAlternatively, you may consider [mo-json](https://pypi.org/project/mo-json/) which has a function `value2json` that converts a larger number of data structures into JSON.\n\n\n## Summary\n\nThis library is the basis for a data transformation algebra: We want a succinct way of transforming data in Python. We want operations on data to result in yet more data. We do not want data operations to raise exceptions. This library is solves Python\'s lack of consistency (lack of closure) under the dot (`.`) and slice `[::]` operators when operating on data objects. \n\n[Full documentation](https://github.com/klahnakoski/mo-dots/tree/dev/docs)\n',
     long_description_content_type='text/markdown',
     name='mo-dots',
     packages=["mo_dots"],
     url='https://github.com/klahnakoski/mo-dots',
-    version='9.592.24112',
+    version='9.593.24112',
     zip_safe=False
 )
```


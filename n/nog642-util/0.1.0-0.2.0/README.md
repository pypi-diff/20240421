# Comparing `tmp/nog642_util-0.1.0.tar.gz` & `tmp/nog642_util-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/nog642/Documents/nog642-python-utils/nog642_util/dist/.tmp-521ukufe/nog642_util-0.1.0.tar", last modified: Sat Apr 20 21:16:52 2024, max compression
+gzip compressed data, was "/home/nog642/Documents/nog642-python-utils/nog642_util/dist/.tmp-bao2i_ic/nog642_util-0.2.0.tar", last modified: Sun Apr 21 04:35:30 2024, max compression
```

## Comparing `nog642_util-0.1.0.tar` & `nog642_util-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-20 21:16:52.083790 nog642_util-0.1.0/
--rw-r--r--   0 nog642    (1000) nog642    (1000)      572 2024-04-20 21:16:52.083790 nog642_util-0.1.0/PKG-INFO
--rw-rw-r--   0 nog642    (1000) nog642    (1000)       67 2024-04-20 21:16:31.000000 nog642_util-0.1.0/README.md
--rw-rw-r--   0 nog642    (1000) nog642    (1000)      597 2024-04-20 21:16:31.000000 nog642_util-0.1.0/pyproject.toml
--rw-rw-r--   0 nog642    (1000) nog642    (1000)       38 2024-04-20 21:16:52.083790 nog642_util-0.1.0/setup.cfg
-drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-20 21:16:52.079790 nog642_util-0.1.0/src/
-drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-20 21:16:52.079790 nog642_util-0.1.0/src/nog642_util/
--rw-rw-r--   0 nog642    (1000) nog642    (1000)    12853 2024-04-20 21:16:31.000000 nog642_util-0.1.0/src/nog642_util/__init__.py
-drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-20 21:16:52.083790 nog642_util-0.1.0/src/nog642_util.egg-info/
--rw-r--r--   0 nog642    (1000) nog642    (1000)      572 2024-04-20 21:16:52.000000 nog642_util-0.1.0/src/nog642_util.egg-info/PKG-INFO
--rw-rw-r--   0 nog642    (1000) nog642    (1000)      238 2024-04-20 21:16:52.000000 nog642_util-0.1.0/src/nog642_util.egg-info/SOURCES.txt
--rw-rw-r--   0 nog642    (1000) nog642    (1000)        1 2024-04-20 21:16:52.000000 nog642_util-0.1.0/src/nog642_util.egg-info/dependency_links.txt
--rw-rw-r--   0 nog642    (1000) nog642    (1000)       12 2024-04-20 21:16:52.000000 nog642_util-0.1.0/src/nog642_util.egg-info/top_level.txt
-drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-20 21:16:52.083790 nog642_util-0.1.0/tests/
--rw-rw-r--   0 nog642    (1000) nog642    (1000)     7012 2024-04-20 21:16:31.000000 nog642_util-0.1.0/tests/test_validate_schema.py
+drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-21 04:35:30.957190 nog642_util-0.2.0/
+-rw-r--r--   0 nog642    (1000) nog642    (1000)      572 2024-04-21 04:35:30.953190 nog642_util-0.2.0/PKG-INFO
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)       67 2024-04-20 21:16:31.000000 nog642_util-0.2.0/README.md
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)      597 2024-04-21 04:32:19.000000 nog642_util-0.2.0/pyproject.toml
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)       38 2024-04-21 04:35:30.957190 nog642_util-0.2.0/setup.cfg
+drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-21 04:35:30.953190 nog642_util-0.2.0/src/
+drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-21 04:35:30.953190 nog642_util-0.2.0/src/nog642_util/
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)    12842 2024-04-20 23:01:27.000000 nog642_util-0.2.0/src/nog642_util/__init__.py
+drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-21 04:35:30.953190 nog642_util-0.2.0/src/nog642_util.egg-info/
+-rw-r--r--   0 nog642    (1000) nog642    (1000)      572 2024-04-21 04:35:30.000000 nog642_util-0.2.0/src/nog642_util.egg-info/PKG-INFO
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)      260 2024-04-21 04:35:30.000000 nog642_util-0.2.0/src/nog642_util.egg-info/SOURCES.txt
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)        1 2024-04-21 04:35:30.000000 nog642_util-0.2.0/src/nog642_util.egg-info/dependency_links.txt
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)       12 2024-04-21 04:35:30.000000 nog642_util-0.2.0/src/nog642_util.egg-info/top_level.txt
+drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-21 04:35:30.953190 nog642_util-0.2.0/tests/
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)      817 2024-04-20 23:13:32.000000 nog642_util-0.2.0/tests/test_StrEnum.py
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)     7006 2024-04-20 22:59:17.000000 nog642_util-0.2.0/tests/test_validate_schema.py
```

### Comparing `nog642_util-0.1.0/PKG-INFO` & `nog642_util-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nog642_util
-Version: 0.1.0
+Version: 0.2.0
 Summary: Various utilities for python.
 Author-email: nog642 <nog642.contact@gmail.com>
 Project-URL: Homepage, https://gitlab.com/nog642-org/nog642-python-utils
 Project-URL: Issues, https://gitlab.com/nog642-org/nog642-python-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nog642_util-0.1.0/pyproject.toml` & `nog642_util-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nog642_util"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="nog642", email="nog642.contact@gmail.com" },
 ]
 description = "Various utilities for python."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `nog642_util-0.1.0/src/nog642_util/__init__.py` & `nog642_util-0.2.0/src/nog642_util/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,59 @@
 #!/usr/bin/env python3
+from __future__ import annotations
+
 from collections.abc import Collection, Sequence
 from enum import Enum, EnumMeta
 import inspect
 import json
 import sys
 import traceback
 import typing
+from typing import FrozenSet
 from typing import get_origin as typing_get_origin
 from typing import get_args as typing_get_args
 
 
-class _CustomEnumMeta(EnumMeta):
-    # TODO: get rid of this if not necessary
+class _StrEnumMeta(EnumMeta):
+    _StrEnum__member_set: FrozenSet[StrEnum]
 
     def __new__(metacls, name, bases, attrs):
         cls = EnumMeta.__new__(metacls, name, bases, attrs)
-        if name != 'CustomEnum':
-            if hasattr(cls, 'enum_set') and any(base.__name__ == 'CustomEnum' for base in cls.__bases__):
-                raise ValueError('CustomEnum cannot define value enum_set; '
-                                 f'already defined as {cls.enum_set}')
-            # else, CustomEnum is a base class of a base class and existing enum_set was added by CustomEnum already
-            # utility: all the enum values as a set
-            cls.enum_set = set(elem for elem in cls.__members__.values())
+        if len(cls) > 0:  # if the class has any members
+            member_set_attr_name = '_StrEnum__member_set'
+            if hasattr(cls, member_set_attr_name):
+                raise ValueError(f'StrEnum cannot define value __value_set; '
+                                 f'already defined as {getattr(cls, member_set_attr_name)}')
+            setattr(cls, member_set_attr_name, frozenset(cls.__members__.values()))
         return cls
 
+    def __contains__(cls, item):
+        if isinstance(item, cls):
+            return True
+        return item in cls._StrEnum__member_set
+
 
-class CustomEnum(str, Enum, metaclass=_CustomEnumMeta):
+class StrEnum(str, Enum, metaclass=_StrEnumMeta):
     """
     To be used for basic string enums.
 
     Major change is that enum instances now compare equal to the string value,
     as opposed to plain enums (because of the str mixin).
 
-    Also provides extra functionality on top of basic enums (like the
-    cls.enum_set attribute).
+    Whether a string is a valid enum can be checked using the `in` operator on
+    the class directly.
 
     Example usage:
-    >>> class Example(CustomEnum):
+    >>> class Example(StrEnum):
     ...     abc = 'abc'
     ...     XYZ = 'xyz'
     ...
-    >>> Example.enum_set
-    {<Example.XYZ: 'xyz'>, <Example.abc: 'abc'>}
     >>> Example.XYZ == 'xyz'
     True
-    >>> 'xyz' in Example.enum_set
+    >>> 'xyz' in Example
     True
     >>> Example('xyz')
     <Example.XYZ: 'xyz'>
     >>> isinstance(Example.XYZ, str)
     True
     """
 
@@ -155,30 +160,30 @@
             try:
                 if _plain_type_check(data, t, qualname=qualname):
                     return True
             except SchemaValueError:
                 pass
         return False
 
-    # support strings counting as CustomEnum values
+    # support strings counting as StrEnum values
     # and add additional input checks for the definition being processed (data_type must be a type)
     try:
-        subclass_check_result = issubclass(data_type, CustomEnum)
+        subclass_check_result = issubclass(data_type, StrEnum)
     except TypeError as e:
         raise SchemaDefinitionError(f"Expected {data_type!r} to be a python type, found {type(data_type)}, it's "
                                     f'likely you are passing some of the parameters in your schema definition '
                                     f'in the wrong order where this is defined!') from e
     if subclass_check_result:
         if (not isinstance(data, data_type)) and isinstance(data, str):
             # try converting to an enum first
             try:
                 data = data_type(data)
             except Exception as e:
                 raise SchemaValueError(f'{qualname} must be a member of {data_type.__qualname__}: '
-                                       f'one of {data_type.enum_set}, not {data!r}') from e
+                                       f'one of {set(data_type)}, not {data!r}') from e
 
     return isinstance(data, data_type)
 
 
 def validate_schema(data, schema, qualname='data'):
     """
     qualname is the name of the data passed in. It is used to generate error messages.
@@ -211,15 +216,15 @@
     (dict, 'keyvalue', (sub_schema, sub_schema)) is for when the dictionary has an arbitrary/dynamic
         set of keys. Here, you define the schemas for the keys and the values in the form
         (key_schema, value_schema). Often key_schema will just be str.
     (list, 'items', sub_schema) and (set, 'items', sub_schema) are for when you want to define a
         schema for each item in a collection. Any collection (i.e. a subclass of collections.abc.Collection)
         will work here, not just list or set.
 
-    CustomEnum is supported. If the schema is a subclass of CustomEnum, it will accept both enum instances
+    StrEnum is supported. If the schema is a subclass of StrEnum, it will accept both enum instances
         and the corresponding strings as valid values. Regular python enums are not supported yet (they
         are just checked with isinstance).
 
     :param data:
     :param schema:
     :param qualname: name of the data passed in. It is used to generate error messages.
     :return:
```

### Comparing `nog642_util-0.1.0/src/nog642_util.egg-info/PKG-INFO` & `nog642_util-0.2.0/src/nog642_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nog642_util
-Version: 0.1.0
+Version: 0.2.0
 Summary: Various utilities for python.
 Author-email: nog642 <nog642.contact@gmail.com>
 Project-URL: Homepage, https://gitlab.com/nog642-org/nog642-python-utils
 Project-URL: Issues, https://gitlab.com/nog642-org/nog642-python-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nog642_util-0.1.0/tests/test_validate_schema.py` & `nog642_util-0.2.0/tests/test_validate_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 from typing import Optional, Union
 
 import pytest
 
-from nog642_util import (validate_schema, Nullable, SchemaValueError, SchemaTypeError,
-                         CustomEnum, SchemaDefinitionError)
+from nog642_util import (StrEnum, validate_schema, Nullable, SchemaValueError, SchemaTypeError,
+                         SchemaDefinitionError)
 
 
 def test_empty_str():
     assert validate_schema(
         data='',
         schema=str
     ) is None  # success
@@ -148,15 +148,15 @@
     with pytest.raises(SchemaValueError):
         validate_schema(
             data={},
             schema=(dict, 'explicit', {'a': ('required', Nullable(int))})
         )
 
 
-class TestEnum(CustomEnum):
+class TestEnum(StrEnum):
     __test__ = False  # not a test case
     enum_value_a = 'enum_value_a'
     enum_value_b = 'enum_value_b_str'
 
 
 def test_explicit_dict_required_enum_key_invalid_str():
     with pytest.raises(SchemaValueError):
```


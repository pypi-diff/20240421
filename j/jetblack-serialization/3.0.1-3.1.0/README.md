# Comparing `tmp/jetblack-serialization-3.0.1.tar.gz` & `tmp/jetblack-serialization-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetblack-serialization-3.0.1.tar", max compression
+gzip compressed data, was "jetblack-serialization-3.1.0.tar", max compression
```

## Comparing `jetblack-serialization-3.0.1.tar` & `jetblack-serialization-3.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2022-04-27 09:50:02.686185 jetblack-serialization-3.0.1/LICENSE
--rw-r--r--   0        0        0     5284 2022-04-27 09:50:02.686350 jetblack-serialization-3.0.1/README.md
--rw-r--r--   0        0        0      161 2022-09-24 06:31:30.080154 jetblack-serialization-3.0.1/jetblack_serialization/__init__.py
--rw-r--r--   0        0        0     1623 2022-09-24 08:24:38.781842 jetblack-serialization-3.0.1/jetblack_serialization/config.py
--rw-r--r--   0        0        0     2651 2022-09-24 06:31:30.080822 jetblack-serialization-3.0.1/jetblack_serialization/custom_annotations.py
--rw-r--r--   0        0        0      578 2022-09-24 08:24:38.781967 jetblack-serialization-3.0.1/jetblack_serialization/json/__init__.py
--rw-r--r--   0        0        0     2040 2022-04-27 09:50:02.688358 jetblack-serialization-3.0.1/jetblack_serialization/json/annotations.py
--rw-r--r--   0        0        0     1824 2022-09-24 08:24:38.782145 jetblack-serialization-3.0.1/jetblack_serialization/json/serialization.py
--rw-r--r--   0        0        0     7414 2022-09-24 08:24:38.782348 jetblack-serialization-3.0.1/jetblack_serialization/json/typed_deserializer.py
--rw-r--r--   0        0        0     6066 2022-09-24 08:24:38.782525 jetblack-serialization-3.0.1/jetblack_serialization/json/typed_serializer.py
--rw-r--r--   0        0        0     1551 2022-09-24 08:24:38.782648 jetblack-serialization-3.0.1/jetblack_serialization/json/untyped_deserializer.py
--rw-r--r--   0        0        0     1338 2022-09-24 08:24:38.782776 jetblack-serialization-3.0.1/jetblack_serialization/json/untyped_serializer.py
--rw-r--r--   0        0        0       10 2022-04-27 09:50:02.689256 jetblack-serialization-3.0.1/jetblack_serialization/py.typed
--rw-r--r--   0        0        0       77 2022-04-27 09:50:02.689362 jetblack-serialization-3.0.1/jetblack_serialization/types.py
--rw-r--r--   0        0        0     3235 2023-05-07 15:09:34.077443 jetblack-serialization-3.0.1/jetblack_serialization/typing_inspect_ex.py
--rw-r--r--   0        0        0     1405 2022-09-24 08:24:38.782891 jetblack-serialization-3.0.1/jetblack_serialization/utils.py
--rw-r--r--   0        0        0      528 2022-09-24 08:24:38.783012 jetblack-serialization-3.0.1/jetblack_serialization/xml/__init__.py
--rw-r--r--   0        0        0     2047 2022-09-24 08:24:38.783127 jetblack-serialization-3.0.1/jetblack_serialization/xml/annotations.py
--rw-r--r--   0        0        0     1822 2022-09-24 08:24:38.783197 jetblack-serialization-3.0.1/jetblack_serialization/xml/serialization.py
--rw-r--r--   0        0        0     8148 2022-09-24 08:29:33.303404 jetblack-serialization-3.0.1/jetblack_serialization/xml/typed_deserializer.py
--rw-r--r--   0        0        0     7356 2022-09-24 08:24:38.783494 jetblack-serialization-3.0.1/jetblack_serialization/xml/typed_serializer.py
--rw-r--r--   0        0        0     3101 2022-09-24 08:24:38.783613 jetblack-serialization-3.0.1/jetblack_serialization/xml/untyped_deserializer.py
--rw-r--r--   0        0        0     2725 2022-09-24 08:24:38.783726 jetblack-serialization-3.0.1/jetblack_serialization/xml/untyped_serializer.py
--rw-r--r--   0        0        0      873 2023-05-07 15:05:34.350734 jetblack-serialization-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     6410 2023-05-07 15:10:25.552501 jetblack-serialization-3.0.1/setup.py
--rw-r--r--   0        0        0     6229 2023-05-07 15:10:25.552819 jetblack-serialization-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-04-27 09:50:02.686185 jetblack-serialization-3.1.0/LICENSE
+-rw-r--r--   0        0        0     5284 2022-04-27 09:50:02.686350 jetblack-serialization-3.1.0/README.md
+-rw-r--r--   0        0        0      161 2022-09-24 06:31:30.080154 jetblack-serialization-3.1.0/jetblack_serialization/__init__.py
+-rw-r--r--   0        0        0     1823 2024-04-21 15:04:51.150431 jetblack-serialization-3.1.0/jetblack_serialization/config.py
+-rw-r--r--   0        0        0     2651 2022-09-24 06:31:30.080822 jetblack-serialization-3.1.0/jetblack_serialization/custom_annotations.py
+-rw-r--r--   0        0        0      578 2022-09-24 08:24:38.781967 jetblack-serialization-3.1.0/jetblack_serialization/json/__init__.py
+-rw-r--r--   0        0        0     2040 2022-04-27 09:50:02.688358 jetblack-serialization-3.1.0/jetblack_serialization/json/annotations.py
+-rw-r--r--   0        0        0     1824 2022-09-24 08:24:38.782145 jetblack-serialization-3.1.0/jetblack_serialization/json/serialization.py
+-rw-r--r--   0        0        0     7490 2024-04-21 15:04:51.150897 jetblack-serialization-3.1.0/jetblack_serialization/json/typed_deserializer.py
+-rw-r--r--   0        0        0     6140 2024-04-21 15:04:51.151303 jetblack-serialization-3.1.0/jetblack_serialization/json/typed_serializer.py
+-rw-r--r--   0        0        0     1551 2022-09-24 08:24:38.782648 jetblack-serialization-3.1.0/jetblack_serialization/json/untyped_deserializer.py
+-rw-r--r--   0        0        0     1338 2022-09-24 08:24:38.782776 jetblack-serialization-3.1.0/jetblack_serialization/json/untyped_serializer.py
+-rw-r--r--   0        0        0       10 2022-04-27 09:50:02.689256 jetblack-serialization-3.1.0/jetblack_serialization/py.typed
+-rw-r--r--   0        0        0       77 2022-04-27 09:50:02.689362 jetblack-serialization-3.1.0/jetblack_serialization/types.py
+-rw-r--r--   0        0        0     3235 2023-05-07 15:09:34.077443 jetblack-serialization-3.1.0/jetblack_serialization/typing_inspect_ex.py
+-rw-r--r--   0        0        0     1602 2024-04-21 15:04:51.151666 jetblack-serialization-3.1.0/jetblack_serialization/utils.py
+-rw-r--r--   0        0        0      528 2022-09-24 08:24:38.783012 jetblack-serialization-3.1.0/jetblack_serialization/xml/__init__.py
+-rw-r--r--   0        0        0     2047 2022-09-24 08:24:38.783127 jetblack-serialization-3.1.0/jetblack_serialization/xml/annotations.py
+-rw-r--r--   0        0        0     1822 2022-09-24 08:24:38.783197 jetblack-serialization-3.1.0/jetblack_serialization/xml/serialization.py
+-rw-r--r--   0        0        0     8253 2024-04-21 15:04:51.152366 jetblack-serialization-3.1.0/jetblack_serialization/xml/typed_deserializer.py
+-rw-r--r--   0        0        0     7427 2024-04-21 15:04:51.152737 jetblack-serialization-3.1.0/jetblack_serialization/xml/typed_serializer.py
+-rw-r--r--   0        0        0     3101 2022-09-24 08:24:38.783613 jetblack-serialization-3.1.0/jetblack_serialization/xml/untyped_deserializer.py
+-rw-r--r--   0        0        0     2725 2022-09-24 08:24:38.783726 jetblack-serialization-3.1.0/jetblack_serialization/xml/untyped_serializer.py
+-rw-r--r--   0        0        0      873 2024-04-21 15:04:51.153060 jetblack-serialization-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6410 2024-04-21 15:05:04.532879 jetblack-serialization-3.1.0/setup.py
+-rw-r--r--   0        0        0     6229 2024-04-21 15:05:04.533228 jetblack-serialization-3.1.0/PKG-INFO
```

### Comparing `jetblack-serialization-3.0.1/LICENSE` & `jetblack-serialization-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.1/README.md` & `jetblack-serialization-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/config.py` & `jetblack-serialization-3.1.0/jetblack_serialization/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Serializer Config"""
 
 from datetime import datetime, timedelta
 from decimal import Decimal
-from typing import Any, Callable, Dict, Optional, Type
+from typing import Any, Callable, Mapping, Optional, Type
 
 from jetblack_iso8601 import (
     iso8601_to_datetime,
     iso8601_to_timedelta,
     datetime_to_iso8601,
     timedelta_to_iso8601,
 )
@@ -26,36 +26,41 @@
 def to_timedelta(text: str) -> timedelta:
     value = iso8601_to_timedelta(text)
     if value is None:
         raise ValueError('Unable to parse iso8601 timestamp')
     return value
 
 
-VALUE_DESERIALIZERS: Dict[Type, Callable[[str], Any]] = {
-    datetime: to_datetime,
-    timedelta: to_timedelta,
-    Decimal: Decimal
-}
-VALUE_SERIALIZERS: Dict[Type, Callable[[Any], Any]] = {
+ValueSerializer = Callable[[Any], Any]
+ValueDeserializer = Callable[[str], Any]
+ValueSerializers = Mapping[Type, ValueSerializer]
+ValueDeserializers = Mapping[Type, ValueDeserializer]
+
+VALUE_SERIALIZERS: ValueSerializers = {
     datetime: datetime_to_iso8601,
     timedelta: timedelta_to_iso8601,
     Decimal: float
 }
+VALUE_DESERIALIZERS: ValueDeserializers = {
+    datetime: to_datetime,
+    timedelta: to_timedelta,
+    Decimal: Decimal
+}
 
 
 class SerializerConfig:
     """Configuration for serialization"""
 
     def __init__(
         self,
         serialize_key: Optional[Callable[[str], str]],
         deserialize_key: Optional[Callable[[str], str]],
         *,
         pretty_print: bool = False,
-        value_serializers=VALUE_SERIALIZERS,
-        value_deserializers=VALUE_DESERIALIZERS
+        value_serializers: ValueSerializers = VALUE_SERIALIZERS,
+        value_deserializers: ValueDeserializers = VALUE_DESERIALIZERS
     ) -> None:
         self.serialize_key = serialize_key or _same_name
         self.deserialize_key = deserialize_key or _same_name
         self.pretty_print = pretty_print
         self.value_serializers = value_serializers
         self.value_deserializers = value_deserializers
```

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/custom_annotations.py` & `jetblack-serialization-3.1.0/jetblack_serialization/custom_annotations.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/json/__init__.py` & `jetblack-serialization-3.1.0/jetblack_serialization/json/__init__.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/json/annotations.py` & `jetblack-serialization-3.1.0/jetblack_serialization/json/annotations.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/json/serialization.py` & `jetblack-serialization-3.1.0/jetblack_serialization/json/serialization.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/json/typed_deserializer.py` & `jetblack-serialization-3.1.0/jetblack_serialization/json/typed_deserializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     cast
 )
 
 from .. import typing_inspect_ex as typing_inspect
 from ..config import SerializerConfig
 from ..custom_annotations import get_typed_dict_key_default
 from ..types import Annotation
-from ..utils import is_simple_type
+from ..utils import is_value_type
 
 from .annotations import (
     JSONAnnotation,
     JSONValue,
     JSONProperty,
     is_json_annotation,
     get_json_annotation
@@ -131,14 +131,15 @@
         obj: Dict[str, Any],
         dict_annotation: Annotation,
         config: SerializerConfig
 ) -> Dict[str, Any]:
     json_obj: Dict[str, Any] = {}
 
     typed_dict_keys = typing_inspect.typed_dict_keys(dict_annotation)
+    assert typed_dict_keys is not None
     for key, key_annotation in typed_dict_keys.items():
         default = get_typed_dict_key_default(key_annotation)
         if is_json_annotation(key_annotation):
             item_type_annotation, item_json_annotation = get_json_annotation(
                 key_annotation
             )
             if not issubclass(type(item_json_annotation), JSONProperty):
@@ -156,15 +157,15 @@
         if json_property.tag in obj:
             json_obj[key] = _to_any(
                 obj[json_property.tag],
                 item_type_annotation,
                 json_property,
                 config
             )
-        elif default != Parameter.empty:
+        elif default is not Parameter.empty:
             json_obj[key] = _to_any(
                 default,
                 item_type_annotation,
                 json_property,
                 config
             )
         elif typing_inspect.is_optional_type(item_type_annotation):
@@ -179,15 +180,15 @@
 
 def _to_any(
         json_value: Any,
         type_annotation: Annotation,
         json_annotation: JSONAnnotation,
         config: SerializerConfig
 ) -> Any:
-    if is_simple_type(type_annotation):
+    if is_value_type(type_annotation, config.value_deserializers.keys()):
         return _to_value(
             json_value,
             type_annotation,
             config
         )
     elif typing_inspect.is_optional_type(type_annotation):
         return _to_optional(
```

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/json/typed_serializer.py` & `jetblack-serialization-3.1.0/jetblack_serialization/json/typed_serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from inspect import Parameter
 import json
 from typing import Any, Type, Union, cast
 
 import jetblack_serialization.typing_inspect_ex as typing_inspect
 from ..config import SerializerConfig
 from ..types import Annotation
-from ..utils import is_simple_type
+from ..utils import is_value_type
 
 from .annotations import (
     JSONAnnotation,
     JSONValue,
     JSONProperty,
     is_json_annotation,
     get_json_annotation
@@ -120,14 +120,15 @@
         dct: dict,
         type_annotation: Annotation,
         config: SerializerConfig
 ) -> dict:
     json_obj = dict()
 
     typed_dict_keys = typing_inspect.typed_dict_keys(type_annotation)
+    assert typed_dict_keys is not None
     for key, key_annotation in typed_dict_keys.items():
         default = getattr(type_annotation, key, Parameter.empty)
         if typing_inspect.is_annotated_type(key_annotation):
             item_type_annotation, item_json_annotation = get_json_annotation(
                 key_annotation
             )
             if not issubclass(type(item_json_annotation), JSONProperty):
@@ -137,15 +138,15 @@
             property_name = config.serialize_key(
                 key
             ) if isinstance(key, str) else key
             json_property = JSONProperty(property_name)
             item_type_annotation = key_annotation
 
         value = dct.get(key, default)
-        if value != Parameter.empty:
+        if value is not Parameter.empty:
             json_obj[json_property.tag] = _from_any(
                 value,
                 item_type_annotation,
                 json_property,
                 config
             )
         else:
@@ -157,15 +158,15 @@
 
 def _from_any(
         value: Any,
         type_annotation: Annotation,
         json_annotation: JSONAnnotation,
         config: SerializerConfig
 ) -> Any:
-    if is_simple_type(type_annotation):
+    if is_value_type(type_annotation, config.value_serializers.keys()):
         return _from_value(
             value,
             type_annotation,
             config
         )
     elif typing_inspect.is_optional_type(type_annotation):
         return _from_optional(
```

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/json/untyped_deserializer.py` & `jetblack-serialization-3.1.0/jetblack_serialization/json/untyped_deserializer.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/json/untyped_serializer.py` & `jetblack-serialization-3.1.0/jetblack_serialization/json/untyped_serializer.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/typing_inspect_ex.py` & `jetblack-serialization-3.1.0/jetblack_serialization/typing_inspect_ex.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/utils.py` & `jetblack-serialization-3.1.0/jetblack_serialization/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 """Protocol utilities"""
 
 from datetime import datetime, timedelta
 from decimal import Decimal
 from enum import Enum
 from inspect import isclass
-from typing import Any
+from typing import Any, Iterable, Sequence, Type, Union
 
 import jetblack_serialization.typing_inspect_ex as typing_inspect
 from .types import Annotation
 
+BUILTIN_TYPES: Sequence[Type] = (
+    str,
+    bool,
+    int,
+    float
+)
 
-def is_simple_type(annotation: Annotation) -> bool:
-    """Return True if the annotation is a simple type like an int or a str.
+
+def is_value_type(
+        annotation: Union[Annotation, Type],
+        custom_types: Iterable[Type]
+) -> bool:
+    """Return True if the annotation is a value type like an int or a str.
 
     Args:
-        annotation (Any): The annotation
+        annotation (Union[Any, Type]): The annotation
+        custom_types (Iterable[Type]): Any custom types.
 
     Returns:
         bool: True if the annotation is a JSON literal, otherwise False
     """
-    return annotation in (
-        str,
-        bool,
-        int,
-        float,
-        Decimal,
-        datetime,
-        timedelta
-    ) or (isclass(annotation) and issubclass(annotation, Enum))
+    return (
+        annotation in BUILTIN_TYPES or
+        annotation in custom_types or
+        (isclass(annotation) and issubclass(annotation, Enum))
+    )
 
 
 def is_container_type(annotation: Any) -> bool:
     """Return True if this is a JSON container.
 
     A JSON container can be an object (Like a Dict[str, Any]), or a List.
```

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/xml/__init__.py` & `jetblack-serialization-3.1.0/jetblack_serialization/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/xml/annotations.py` & `jetblack-serialization-3.1.0/jetblack_serialization/xml/annotations.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/xml/serialization.py` & `jetblack-serialization-3.1.0/jetblack_serialization/xml/serialization.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/xml/typed_deserializer.py` & `jetblack-serialization-3.1.0/jetblack_serialization/xml/typed_deserializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from lxml import etree
 from lxml.etree import _Element  # pylint: disable=no-name-in-module
 
 from .. import typing_inspect_ex as typing_inspect
 from ..config import SerializerConfig
 from ..custom_annotations import get_typed_dict_key_default
 from ..types import Annotation
-from ..utils import is_simple_type
+from ..utils import is_value_type
 
 from .annotations import (
     XMLAnnotation,
     XMLAttribute,
     XMLEntity,
     get_xml_annotation
 )
@@ -131,14 +131,15 @@
         text = element.text
     else:
         text = element.attrib[xml_annotation.tag]
     if text is None and default is Parameter.empty:
         raise ValueError(f'Expected "{xml_annotation.tag}" to be non-null')
     if isinstance(text, bytes):
         text = text.decode()
+    assert isinstance(text, str)
     return _to_value(text, default, type_annotation, config)
 
 
 def _to_list(
         element: Optional[_Element],
         type_annotation: Annotation,
         xml_annotation: XMLAnnotation,
@@ -183,14 +184,15 @@
 ) -> Optional[Dict[str, Any]]:
     if element is None:
         raise ValueError('Received "None" while deserializing a TypeDict')
 
     typed_dict: Dict[str, Any] = {}
 
     typed_dict_keys = typing_inspect.typed_dict_keys(type_annotation)
+    assert typed_dict_keys is not None
     for key, key_annotation in typed_dict_keys.items():
         default = get_typed_dict_key_default(key_annotation)
         if typing_inspect.is_annotated_type(key_annotation):
             item_type_annotation, item_xml_annotation = get_xml_annotation(
                 key_annotation
             )
         else:
@@ -223,15 +225,15 @@
         element: Optional[_Element],
         default: Optional[Any],
         type_annotation: Annotation,
         xml_annotation: XMLAnnotation,
         config: SerializerConfig
 ) -> Any:
 
-    if is_simple_type(type_annotation):
+    if is_value_type(type_annotation, config.value_deserializers.keys()):
         return _to_simple(
             element,
             default,
             type_annotation,
             xml_annotation,
             config
         )
```

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/xml/typed_serializer.py` & `jetblack-serialization-3.1.0/jetblack_serialization/xml/typed_serializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from lxml import etree
 from lxml.etree import Element, _Element, SubElement  # pylint: disable=no-name-in-module
 
 import jetblack_serialization.typing_inspect_ex as typing_inspect
 from ..types import Annotation
 from ..config import SerializerConfig
-from ..utils import is_simple_type
+from ..utils import is_value_type
 
 from .annotations import (
     XMLAnnotation,
     XMLAttribute,
     XMLEntity,
     get_xml_annotation
 )
@@ -70,15 +70,15 @@
             xml_annotation,
             element,
             config
         )
     else:
         return _from_union(
             obj,
-            Union[tuple(union_types)], # type: ignore
+            Union[tuple(union_types)],  # type: ignore
             xml_annotation,
             element,
             config
         )
 
 
 def _from_union(
@@ -146,14 +146,15 @@
         xml_annotation: XMLAnnotation,
         element: Optional[_Element],
         config: SerializerConfig
 ) -> _Element:
     dict_element = _make_element(element, xml_annotation.tag)
 
     typed_dict_keys = typing_inspect.typed_dict_keys(type_annotation)
+    assert typed_dict_keys is not None
     for key, key_annotation in typed_dict_keys.items():
         default = getattr(type_annotation, key, Parameter.empty)
         if typing_inspect.is_annotated_type(key_annotation):
             item_type_annotation, item_xml_annotation = get_xml_annotation(
                 key_annotation
             )
         else:
@@ -199,15 +200,15 @@
 def _from_obj(
         obj: Any,
         type_annotation: Annotation,
         xml_annotation: XMLAnnotation,
         element: Optional[_Element],
         config: SerializerConfig
 ) -> _Element:
-    if is_simple_type(type_annotation):
+    if is_value_type(type_annotation, config.value_serializers.keys()):
         return _from_simple(
             obj,
             type_annotation,
             xml_annotation,
             element,
             config
         )
```

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/xml/untyped_deserializer.py` & `jetblack-serialization-3.1.0/jetblack_serialization/xml/untyped_deserializer.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.1/jetblack_serialization/xml/untyped_serializer.py` & `jetblack-serialization-3.1.0/jetblack_serialization/xml/untyped_serializer.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.1/pyproject.toml` & `jetblack-serialization-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jetblack-serialization"
-version = "3.0.1"
+version = "3.1.0"
 description = "Serialization for JSON and XML using typing"
 repository = "https://github.com/rob-blackbourn/jetblack-serialization"
 authors = ["Rob Blackbourn <rob.blackbourn@gmail.com>"]
 keywords = ['serialization', 'jetblack', 'json', 'xml', 'typing']
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
```

### Comparing `jetblack-serialization-3.0.1/setup.py` & `jetblack-serialization-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ['jetblack-iso8601>=1.0,<2.0',
  'lxml>=4.9,<5.0',
  'typing-extensions>=4,<5',
  'typing_inspect>=0.8,<0.9']
 
 setup_kwargs = {
     'name': 'jetblack-serialization',
-    'version': '3.0.1',
+    'version': '3.1.0',
     'description': 'Serialization for JSON and XML using typing',
     'long_description': '# jetblack-serialization\n\nSerialization for JSON and XML in Python using typing annotations\n(read the [docs](https://rob-blackbourn.github.io/jetblack-serialization/)).\n\n## Status\n\nIt has been tested with Python 3.7 used the `typing_extensions`\npackage for `TypedDict` and `Annotated`. In Python 3.8 the `TypedDict`\nclass is available in the standard `typing` package.\n\n## Installation\n\nThe package can be installed with pip.\n\n```bash\npip install jetblack-serialization\n```\n\n## Overview\n\nThe package adds support for type annotations when serializing or deserializing\nJSON or XML.\n\n\n### JSON\n\nGiven a typed dictionary:\n\n```python\nfrom datetime import datetime\nfrom typing import List, Optional, TypedDict, Union\n\nclass Book(TypedDict, total=False):\n    book_id: int\n    title: str\n    author: str\n    publication_date: datetime\n    keywords: List[str]\n    phrases: List[str]\n    age: Optional[Union[datetime, int]]\n    pages: Optional[int]\n```\n\n#### Serializing\n\nThis could be serialized to JSON as:\n\n```python\nfrom stringcase import camelcase, snakecase\nfrom jetblack_serialization import SerializerConfig\nfrom jetblack_serialization.json import serialize\n\nobj: Book = {\n    \'author\': \'Chairman Mao\',\n    \'book_id\': 42,\n    \'title\': \'Little Red Book\',\n    \'publication_date\': datetime(1973, 1, 1, 21, 52, 13),\n    \'keywords\': [\'Revolution\', \'Communism\'],\n    \'phrases\': [\n        \'Revolutionary wars are inevitable in class society\',\n        \'War is the continuation of politics\'\n    ],\n    \'age\': 24,\n}\ntext = serialize(\n    obj,\n    Book,\n    SerializerConfig(camelcase, snakecase, pretty_print=True)\n)\nprint(text)\n```\n\ngiving:\n\n```json\n{\n    "bookId": 42,\n    "title": "Little Red Book",\n    "author": "Chairman Mao",\n    "publicationDate": "1973-01-01T21:52:13.00Z",\n    "keywords": ["Revolution", "Communism"],\n    "phrases": ["Revolutionary wars are inevitable in class society", "War is the continuation of politics"],\n    "age": 24,\n    "pages": null\n}\n```\n\nNote the fields have been camel cased, and the publication date has been turned\ninto an ISO 8601 date.\n\n#### Deserializing\n\nWe can deserialize the data as follows:\n\n```python\nfrom stringcase import camelcase, snakecase\nfrom jetblack_serialization import SerializerConfig\nfrom jetblack_serialization.json import deserialize\n\ndct = deserialize(\n    text,\n    Annotated[Book, JSONValue()],\n    SerializerConfig(camelcase, snakecase)\n)\n```\n\n### XML\n\nThe XML version of the typed dictionary might look like this:\n\n```python\nfrom datetime import datetime\nfrom typing import List, Optional, TypedDict, Union\nfrom typing_extensions import Annotated\nfrom jetblack_serialization.xml import XMLEntity, XMLAttribute\n\nclass Book(TypedDict, total=False):\n    book_id: Annotated[int, XMLAttribute("bookId")]\n    title: str\n    author: str\n    publication_date: datetime\n    keywords: Annotated[List[Annotated[str, XMLEntity("Keyword")]], XMLEntity("Keywords")]\n    phrases: List[str]\n    age: Optional[Union[datetime, int]]\n    pages: Optional[int]\n```\n\nNote we have introduced some annotations to control the serialization.\nFor XML we have used pascal-case to serialized the keys and snake-case\nfor deserialization.\n\n#### Serializing\n\nTo serialize we need to provide the containing tag `Book`:\n\n```python\nfrom stringcase import pascalcase, snakecase\nfrom jetblack_serialization import SerializerConfig\nfrom jetblack_serialization.xml import serialize\n\nbook: Book = {\n    \'author\': \'Chairman Mao\',\n    \'book_id\': 42,\n    \'title\': \'Little Red Book\',\n    \'publication_date\': datetime(1973, 1, 1, 21, 52, 13),\n    \'keywords\': [\'Revolution\', \'Communism\'],\n    \'phrases\': [\n        \'Revolutionary wars are inevitable in class society\',\n        \'War is the continuation of politics\'\n    ],\n    \'age\': 24,\n    \'pages\': None\n}\ntext = serialize(\n    book,\n    Annotated[Book, XMLEntity("Book")],\n    SerializerConfig(pascalcase, snakecase)\n)\nprint(text)\n```\n\nProducing:\n\n```xml\n<Book bookId="42">\n    <Title>Little Red Book</Title>\n    <Author>Chairman Mao</Author>\n    <PublicationDate>1973-01-01T21:52:13.00Z</PublicationDate>\n    <Keywords>\n        <Keyword>Revolution</Keyword>\n        <Keyword>Communism</Keyword>\n    </Keywords>\n    <Phrase>Revolutionary wars are inevitable in class society</Phrase>\n    <Phrase>War is the continuation of politics</Phrase>\n    <Age>24</Age>\n</Book>\'\n```\n\nThe annotations are more elaborate here. However, much of the typed dictionary\nrequires no annotation.\n\nFirst we needed the outer document wrapper `XMLEntity("Book")`.\n\nNext we annotated the `book_id` to be an `XMLAttribute`.\n\nFinally we annotated the two lists differently. The `keywords` list used\na nested structure, which we indicated by giving the list a different\n`XMLEntity` tag to the list items. For the phrases we used the default\nin-line behaviour.\n\n#### Deserializing\n\nWe can deserialize the XML as follows:\n\n```python\nfrom stringcase import pascalcase, snakecase\nfrom jetblack_serialization import SerializerConfig\nfrom jetblack_serialization.xml import deserialize\n\ndct = deserialize(\n    text,\n    Annotated[Book, XMLEntity("Book")],\n    SerializerConfig(pascalcase, snakecase)\n)\n```\n\n## Attributes\n\nFor JSON, attributes are typically not required. However\n`JSONProperty(tag: str)` and `JSONValue()` are provided for\ncompleteness.',
     'author': 'Rob Blackbourn',
     'author_email': 'rob.blackbourn@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/rob-blackbourn/jetblack-serialization',
```

### Comparing `jetblack-serialization-3.0.1/PKG-INFO` & `jetblack-serialization-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetblack-serialization
-Version: 3.0.1
+Version: 3.1.0
 Summary: Serialization for JSON and XML using typing
 Home-page: https://github.com/rob-blackbourn/jetblack-serialization
 License: Apache-2.0
 Keywords: serialization,jetblack,json,xml,typing
 Author: Rob Blackbourn
 Author-email: rob.blackbourn@gmail.com
 Requires-Python: >=3.7,<4.0
```


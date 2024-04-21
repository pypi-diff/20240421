# Comparing `tmp/nepattern-0.6.5.tar.gz` & `tmp/nepattern-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepattern-0.6.5.tar", last modified: Sat Feb 24 19:41:00 2024, max compression
+gzip compressed data, was "nepattern-0.7.0.tar", last modified: Sun Apr 21 14:44:42 2024, max compression
```

## Comparing `nepattern-0.6.5.tar` & `nepattern-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1091 2024-02-24 17:08:26.922234 nepattern-0.6.5/LICENSE
--rw-r--r--   0        0        0     2604 2024-02-24 18:54:37.048385 nepattern-0.6.5/nepattern/__init__.py
--rw-r--r--   0        0        0    27536 2024-02-24 17:21:49.653437 nepattern-0.6.5/nepattern/base.py
--rw-r--r--   0        0        0     4148 2024-02-24 17:08:26.923232 nepattern-0.6.5/nepattern/context.py
--rw-r--r--   0        0        0     1447 2024-02-24 17:08:26.923232 nepattern-0.6.5/nepattern/context.pyi
--rw-r--r--   0        0        0    13856 2024-02-24 17:20:13.194160 nepattern-0.6.5/nepattern/core.py
--rw-r--r--   0        0        0    14606 2024-02-24 17:08:26.923232 nepattern-0.6.5/nepattern/core.pyi
--rw-r--r--   0        0        0       63 2024-02-24 17:08:26.924232 nepattern-0.6.5/nepattern/exception.py
--rw-r--r--   0        0        0       26 2024-02-24 17:08:26.924232 nepattern-0.6.5/nepattern/i18n/.config.json
--rw-r--r--   0        0        0      481 2024-02-24 17:08:26.924232 nepattern-0.6.5/nepattern/i18n/en-US.json
--rw-r--r--   0        0        0      470 2024-02-24 17:08:26.924232 nepattern-0.6.5/nepattern/i18n/zh-CN.json
--rw-r--r--   0        0        0     6694 2024-02-24 17:08:26.924232 nepattern-0.6.5/nepattern/main.py
--rw-r--r--   0        0        0     2170 2024-02-24 17:08:26.924232 nepattern-0.6.5/nepattern/main.pyi
--rw-r--r--   0        0        0     1073 2024-02-24 18:59:34.297506 nepattern-0.6.5/nepattern/util.py
--rw-r--r--   0        0        0     2065 2024-02-24 19:01:19.902155 nepattern-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      943 2024-02-24 17:08:26.923232 nepattern-0.6.5/README.md
--rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 nepattern-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-02-24 17:08:26.922234 nepattern-0.7.0/LICENSE
+-rw-r--r--   0        0        0      943 2024-02-24 17:08:26.923232 nepattern-0.7.0/README.md
+-rw-r--r--   0        0        0     2658 2024-04-21 14:43:28.345665 nepattern-0.7.0/nepattern/__init__.py
+-rw-r--r--   0        0        0    29406 2024-04-21 14:34:15.607956 nepattern-0.7.0/nepattern/base.py
+-rw-r--r--   0        0        0     4148 2024-02-24 17:08:26.923232 nepattern-0.7.0/nepattern/context.py
+-rw-r--r--   0        0        0     1507 2024-04-21 13:33:39.317700 nepattern-0.7.0/nepattern/context.pyi
+-rw-r--r--   0        0        0    29177 2024-04-21 13:54:20.184287 nepattern-0.7.0/nepattern/core.py
+-rw-r--r--   0        0        0    23609 2024-04-21 13:54:38.849885 nepattern-0.7.0/nepattern/core.pyi
+-rw-r--r--   0        0        0       63 2024-02-24 17:08:26.924232 nepattern-0.7.0/nepattern/exception.py
+-rw-r--r--   0        0        0       26 2024-02-24 17:08:26.924232 nepattern-0.7.0/nepattern/i18n/.config.json
+-rw-r--r--   0        0        0      481 2024-02-24 17:08:26.924232 nepattern-0.7.0/nepattern/i18n/en-US.json
+-rw-r--r--   0        0        0      470 2024-02-24 17:08:26.924232 nepattern-0.7.0/nepattern/i18n/zh-CN.json
+-rw-r--r--   0        0        0     5579 2024-04-21 14:18:56.246589 nepattern-0.7.0/nepattern/main.py
+-rw-r--r--   0        0        0     2186 2024-04-21 13:37:01.346873 nepattern-0.7.0/nepattern/main.pyi
+-rw-r--r--   0        0        0     1073 2024-02-24 18:59:34.297506 nepattern-0.7.0/nepattern/util.py
+-rw-r--r--   0        0        0     2056 2024-04-21 14:44:42.254194 nepattern-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1693 1970-01-01 00:00:00.000000 nepattern-0.7.0/PKG-INFO
```

### Comparing `nepattern-0.6.5/LICENSE` & `nepattern-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nepattern-0.6.5/nepattern/__init__.py` & `nepattern-0.7.0/nepattern/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from .base import ANY as ANY
 from .base import AntiPattern as AntiPattern
 from .base import AnyString as AnyString
 from .base import BOOLEAN as BOOLEAN
 from .base import BYTES as BYTES
 from .base import DATETIME as DATETIME
+from .base import DelimiterInt as DelimiterInt
 from .base import DICT as DICT
 from .base import DirectPattern as DirectPattern
 from .base import DirectTypePattern as DirectTypePattern
 from .base import EMAIL as EMAIL
 from .base import FLOAT as FLOAT
 from .base import HEX as HEX
 from .base import HEX_COLOR as HEX_COLOR
@@ -30,26 +31,26 @@
 from .base import STRING as STRING
 from .base import SequencePattern as SequencePattern
 from .base import SwitchPattern as SwitchPattern
 from .base import TUPLE as TUPLE
 from .base import URL as URL
 from .base import UnionPattern as UnionPattern
 from .base import WIDE_BOOLEAN as WIDE_BOOLEAN
+from .base import combine as combine
 from .context import Patterns as Patterns
 from .context import all_patterns as all_patterns
 from .context import create_local_patterns as create_local_patterns
 from .context import global_patterns
 from .context import local_patterns as local_patterns
 from .context import reset_local_patterns as reset_local_patterns
 from .context import switch_local_patterns as switch_local_patterns
 from .core import BasePattern as BasePattern
 from .core import MatchMode as MatchMode
 from .core import ValidateResult as ValidateResult
 from .exception import MatchFailed as MatchFailed
-from .main import Bind as Bind
 from .main import parser as parser
 from .util import RawStr as RawStr
 from .util import TPattern as TPattern
 
 type_parser = parser
 
 global_patterns().update(
```

### Comparing `nepattern-0.6.5/nepattern/base.py` & `nepattern-0.7.0/nepattern/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 from enum import Enum
-from decimal import Decimal
 from datetime import datetime
 from pathlib import Path
 import re
 import sys
 from typing import (
     TYPE_CHECKING,
     Any,
@@ -20,25 +19,25 @@
     cast,
     final,
     overload, Generic,
 )
 
 from tarina import DateParser, Empty, lang
 
-from .core import BasePattern, MatchMode, ResultFlag, ValidateResult
+from .core import BasePattern, MatchMode, ResultFlag, ValidateResult, _MATCHES, TMM
 from .exception import MatchFailed
 from .util import TPattern
 
 TOrigin = TypeVar("TOrigin")
 TDefault = TypeVar("TDefault")
 _T = TypeVar("_T")
 _T1 = TypeVar("_T1")
 
 
-class DirectPattern(BasePattern[TOrigin, TOrigin]):
+class DirectPattern(BasePattern[TOrigin, TOrigin, Literal[MatchMode.KEEP]]):
     """直接判断"""
 
     __slots__ = ("target",)
 
     def __init__(self, target: TOrigin, alias: str | None = None):
         self.target = target
         super().__init__(mode=MatchMode.KEEP, origin=type(target), alias=alias or str(target))
@@ -78,15 +77,15 @@
             return ValidateResult(error=e, flag=ResultFlag.ERROR)
         return ValidateResult(default, flag=ResultFlag.DEFAULT)  # type: ignore
 
     def __calc_eq__(self, other):  # pragma: no cover
         return isinstance(other, DirectPattern) and self.target == other.target
 
 
-class DirectTypePattern(BasePattern[TOrigin, TOrigin]):
+class DirectTypePattern(BasePattern[TOrigin, TOrigin, Literal[MatchMode.KEEP]]):
     """直接类型判断"""
 
     __slots__ = ("target",)
 
     def __init__(self, target: type[TOrigin], alias: str | None = None):
         self.target = target
         super().__init__(mode=MatchMode.KEEP, origin=target, alias=alias or target.__name__)
@@ -130,15 +129,15 @@
             return ValidateResult(error=e, flag=ResultFlag.ERROR)
         return ValidateResult(default, flag=ResultFlag.DEFAULT)  # type: ignore
 
     def __calc_eq__(self, other):  # pragma: no cover
         return isinstance(other, DirectTypePattern) and self.target == other.target
 
 
-class RegexPattern(BasePattern[Match[str], str]):
+class RegexPattern(BasePattern[Match[str], str, Literal[MatchMode.REGEX_MATCH]]):
     """针对正则的特化匹配，支持正则组"""
 
     def __init__(self, pattern: str | TPattern, alias: str | None = None):
         super().__init__("", origin=Match[str], alias=alias or "regex[:group]")  # type: ignore
         self.regex_pattern = re.compile(pattern)
         self.pattern = self.regex_pattern.pattern
 
@@ -155,62 +154,62 @@
             lang.require("nepattern", "content_error").format(target=input_, expected=self.pattern)
         )
 
     def __calc_eq__(self, other):  # pragma: no cover
         return isinstance(other, RegexPattern) and self.pattern == other.pattern
 
 
-class UnionPattern(BasePattern[Any, _T]):
+class UnionPattern(BasePattern[Any, _T, Literal[MatchMode.KEEP]]):
     """多类型参数的匹配"""
 
     optional: bool
     for_validate: list[BasePattern]
     for_equal: list[str | object]
 
     __slots__ = ("base", "optional", "for_validate", "for_equal")
 
-    def __init__(self, base: Iterable[BasePattern[Any, _T] | _T]):
+    def __init__(self, base: Iterable[BasePattern[Any, _T, Any] | _T]):
         self.base = list(base)
         self.optional = False
         self.for_validate = []
         self.for_equal = []
 
         for arg in self.base:
             if arg == NONE:
                 self.optional = True
                 self.for_equal.append(None)
             elif isinstance(arg, BasePattern):
                 self.for_validate.append(arg)
             else:
                 self.for_equal.append(arg)
         alias_content = "|".join([repr(a) for a in self.for_validate] + [repr(a) for a in self.for_equal])
-        super().__init__(mode=MatchMode.KEEP, origin=str, alias=alias_content)
+        super().__init__(mode=MatchMode.KEEP, origin=Any, alias=alias_content)
 
-    def match(self, text: Any):
-        if not text:
-            text = None
-        if text not in self.for_equal:
+    def match(self, input_: Any):
+        if not input_:
+            input_ = None
+        if input_ not in self.for_equal:
             for pat in self.for_validate:
-                if (res := pat.validate(text)).success:
+                if (res := pat.validate(input_)).success:
                     return res.value()
             raise MatchFailed(
-                lang.require("nepattern", "content_error").format(target=text, expected=self.alias)
+                lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
             )
-        return text
+        return input_
     
     @classmethod
     def _(cls, *types: type[_T1]) -> UnionPattern[_T1]:
         from .main import parser
 
         return cls([parser(i) for i in types])  # type: ignore
 
     def __calc_repr__(self):
         return "|".join(repr(a) for a in (*self.for_validate, *self.for_equal))
 
-    def __or__(self, other: BasePattern[Any, _T1]) -> UnionPattern[Union[_T, _T1]]:
+    def __or__(self, other: BasePattern[Any, _T1, Any]) -> UnionPattern[Union[_T, _T1]]:
         return UnionPattern([*self.base, other])  # type: ignore
 
     def __calc_eq__(self, other):  # pragma: no cover
         return isinstance(other, UnionPattern) and self.base == other.base
 
 
 TSeq = TypeVar("TSeq", list, tuple, set)
@@ -221,15 +220,15 @@
     SUF = "suf"
     ALL = "all"
 
 
 TIterMode = TypeVar("TIterMode", bound=IterMode)
 
 
-class SequencePattern(BasePattern[TSeq, Union[str, TSeq]], Generic[TSeq, TIterMode]):
+class SequencePattern(BasePattern[TSeq, Union[str, TSeq], Literal[MatchMode.REGEX_CONVERT]], Generic[TSeq, TIterMode]):
     """匹配列表或者元组或者集合"""
 
     base: BasePattern
     itermode: TIterMode
 
     def __init__(self, form: type[TSeq], base: BasePattern, mode: TIterMode = IterMode.ALL):
         self.base = base
@@ -239,17 +238,18 @@
         elif form is tuple:
             super().__init__(r"\((.+?)\)", MatchMode.REGEX_CONVERT, form, alias=f"tuple[{base}]")
         elif form is set:
             super().__init__(r"\{(.+?)\}", MatchMode.REGEX_CONVERT, form, alias=f"set[{base}]")
         else:
             raise ValueError(lang.require("nepattern", "sequence_form_error").format(target=str(form)))
         self.converter = lambda _, x: x[1]  # type: ignore
+        self._match = _MATCHES[MatchMode.REGEX_CONVERT](self)
 
-    def match(self, text: Any):
-        _res = self._MATCHES[MatchMode.REGEX_CONVERT](self, text)  # type: ignore
+    def match(self, input_: Any):
+        _res = self._match(self, input_)  # type: ignore
         _max = 0
         success: list[tuple[int, Any]] = []
         fail: list[tuple[int, MatchFailed]] = []
         for _max, s in enumerate(re.split(r"\s*,\s*", _res) if isinstance(_res, str) else _res):
             try:
                 success.append((_max, self.base.match(s)))
             except MatchFailed:
@@ -272,42 +272,43 @@
 
 
 TKey = TypeVar("TKey")
 TVal = TypeVar("TVal")
 
 
 class MappingPattern(
-    BasePattern[Dict[TKey, TVal], Union[str, Dict[TKey, TVal]]],
+    BasePattern[Dict[TKey, TVal], Union[str, Dict[TKey, TVal]], Literal[MatchMode.REGEX_CONVERT]],
     Generic[TKey, TVal, TIterMode],
 ):
     """匹配字典或者映射表"""
 
-    key: BasePattern[TKey, Any]
-    value: BasePattern[TVal, Any]
+    key: BasePattern[TKey, Any, Any]
+    value: BasePattern[TVal, Any, Any]
     itermode: TIterMode
 
     def __init__(
         self, 
-        arg_key: BasePattern[TKey, Any], 
-        arg_value: BasePattern[TVal, Any],
+        arg_key: BasePattern[TKey, Any, Any], 
+        arg_value: BasePattern[TVal, Any, Any],
         mode: TIterMode = IterMode.ALL
     ):
         self.key = arg_key
         self.value = arg_value
         self.itermode = mode
         super().__init__(
             r"\{(.+?)\}",
             MatchMode.REGEX_CONVERT,
             dict,
             alias=f"dict[{self.key}, {self.value}]",
         )
         self.converter = lambda _, x: x[1]
+        self._match = _MATCHES[MatchMode.REGEX_CONVERT](self)
 
     def match(self, input_: str | dict):
-        _res = self._MATCHES[MatchMode.REGEX_CONVERT](self, input_)  # type: ignore
+        _res = self._match(self, input_)  # type: ignore
         success: list[tuple[int, Any, Any]] = []
         fail: list[tuple[int, MatchFailed]] = []
         _max = 0
 
         def _generator_items(res: str | dict):
             if isinstance(res, dict):
                 yield from res.items()
@@ -342,15 +343,15 @@
         return f"dict[{self.key.origin.__name__}, {self.value}]"
 
 
 _TCase = TypeVar("_TCase")
 _TSwtich = TypeVar("_TSwtich")
 
 
-class SwitchPattern(BasePattern[_TCase, _TSwtich]):
+class SwitchPattern(BasePattern[_TCase, _TSwtich, Literal[MatchMode.TYPE_CONVERT]]):
     switch: dict[_TSwtich | ellipsis, _TCase]
 
     __slots__ = ("switch",)
 
     def __init__(self, data: dict[_TSwtich | ellipsis, _TCase]):
         self.switch = data
         super().__init__(mode=MatchMode.TYPE_CONVERT, origin=type(list(data.values())[0]))
@@ -368,15 +369,15 @@
                 lang.require("nepattern", "content_error").format(target=input_, expected=self._repr)
             ) from e
 
     def __calc_eq__(self, other):  # pragma: no cover
         return isinstance(other, SwitchPattern) and self.switch == other.switch
 
 
-class ForwardRefPattern(BasePattern[Any, Any]):
+class ForwardRefPattern(BasePattern[Any, Any, Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(self, ref: ForwardRef):
         self.ref = ref
         super().__init__(mode=MatchMode.TYPE_CONVERT, origin=Any, alias=ref.__forward_arg__)
 
     def match(self, input_: Any):
         if isinstance(input_, str) and input_ == self.ref.__forward_arg__:
             return input_
@@ -393,17 +394,17 @@
             )
         return input_
 
     def __calc_eq__(self, other):  # pragma: no cover
         return isinstance(other, ForwardRefPattern) and self.ref == other.ref
 
 
-class AntiPattern(BasePattern[TOrigin, Any]):
-    def __init__(self, pattern: BasePattern[TOrigin, Any]):
-        self.base: BasePattern[TOrigin, Any] = pattern
+class AntiPattern(BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]]):
+    def __init__(self, pattern: BasePattern[TOrigin, Any, Any]):
+        self.base: BasePattern[TOrigin, Any, Any] = pattern
         super().__init__(mode=MatchMode.TYPE_CONVERT, origin=pattern.origin, alias=f"!{pattern}")
 
     @overload
     def validate(self, input_: TOrigin) -> ValidateResult[Any, Literal[ResultFlag.ERROR]]:
         ...
 
     @overload
@@ -448,34 +449,34 @@
     def __calc_eq__(self, other):  # pragma: no cover
         return isinstance(other, AntiPattern) and self.base == other.base
 
 
 TInput = TypeVar("TInput")
 
 
-class CustomMatchPattern(BasePattern[TOrigin, TInput]):
+class CustomMatchPattern(BasePattern[TOrigin, TInput, Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(
         self,
         origin: type[TOrigin],
         func: Callable[[BasePattern, TInput], TOrigin | None],
         alias: str | None = None,
     ):
         super().__init__(mode=MatchMode.TYPE_CONVERT, origin=origin, alias=alias or func.__name__)
         self.__func__ = func
         self.match = func.__get__(self)  # type: ignore
 
     def __calc_eq__(self, other):  # pragma: no cover
         return isinstance(other, CustomMatchPattern) and self.__func__ == other.__func__
 
 
-NONE = CustomMatchPattern(type(None), lambda _, x: None, alias="none")  # pragma: no cover
+NONE = CustomMatchPattern(type(None), lambda _, __: None, alias="none")  # pragma: no cover
 
 
 @final
-class AnyPattern(BasePattern[Any, Any]):
+class AnyPattern(BasePattern[Any, Any, Literal[MatchMode.KEEP]]):
     def __init__(self):
         super().__init__(mode=MatchMode.KEEP, origin=Any, alias="any")
 
     def match(self, input_: Any) -> Any:  # pragma: no cover
         return input_
 
     def __calc_eq__(self, other):  # pragma: no cover
@@ -483,15 +484,15 @@
 
 
 ANY = AnyPattern()
 """匹配任意内容的表达式"""
 
 
 @final
-class AnyStrPattern(BasePattern[str, Any]):
+class AnyStrPattern(BasePattern[str, Any, Literal[MatchMode.KEEP]]):
     def __init__(self):
         super().__init__(mode=MatchMode.KEEP, origin=str, alias="any_str")
 
     def match(self, input_: Any) -> str:
         return str(input_)
 
     def __calc_eq__(self, other):  # pragma: no cover
@@ -499,17 +500,17 @@
 
 
 AnyString = AnyStrPattern()
 """匹配任意内容并转为字符串的表达式"""
 
 
 @final
-class StrPattern(BasePattern[str, Any]):
+class StrPattern(BasePattern[str, Union[str, bytes, bytearray], Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(self):
-        super().__init__(mode=MatchMode.KEEP, origin=str, alias="str")
+        super().__init__(mode=MatchMode.TYPE_CONVERT, origin=str, accepts=Union[str, bytes, bytearray], alias="str")
 
     def match(self, input_: Any) -> str:
         if isinstance(input_, str):
             return input_.value if isinstance(input_, Enum) else input_
         elif isinstance(input_, (bytes, bytearray)):
             return input_.decode()
         raise MatchFailed(
@@ -521,21 +522,23 @@
         return other.__class__ is StrPattern
 
 
 STRING = StrPattern()
 
 
 @final
-class BytesPattern(BasePattern[bytes, Any]):
+class BytesPattern(BasePattern[bytes, Union[str, bytes, bytearray], Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(self):
-        super().__init__(mode=MatchMode.KEEP, origin=bytes, alias="bytes")
+        super().__init__(mode=MatchMode.TYPE_CONVERT, origin=bytes, accepts=Union[str, bytes, bytearray], alias="bytes")
 
     def match(self, input_: Any) -> bytes:
         if isinstance(input_, bytes):
             return input_
+        elif isinstance(input_, bytearray):
+            return bytes(input_)
         elif isinstance(input_, str):
             return input_.encode()
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected="bytes | str"
             )
         )
@@ -544,15 +547,15 @@
         return other.__class__ is BytesPattern
 
 
 BYTES = BytesPattern()
 
 
 @final
-class IntPattern(BasePattern[int, Any]):
+class IntPattern(BasePattern[int, Any, Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(self):
         super().__init__(mode=MatchMode.TYPE_CONVERT, origin=int, alias="int")
 
     def match(self, input_: Any) -> int:
         if isinstance(input_, int) and input_ is not True and input_ is not False:
             return input_
         if isinstance(input_, (str, bytes, bytearray)) and len(input_) > 4300:  # pragma: no cover
@@ -569,15 +572,15 @@
 
 
 INTEGER = IntPattern()
 """整形数表达式，只能接受整数样式的量"""
 
 
 @final
-class FloatPattern(BasePattern[float, Any]):
+class FloatPattern(BasePattern[float, Any, Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(self):
         super().__init__(mode=MatchMode.TYPE_CONVERT, origin=float, alias="float")
 
     def match(self, input_: Any) -> float:
         if isinstance(input_, float):
             return input_
 
@@ -593,19 +596,19 @@
 
 
 FLOAT = FloatPattern()
 """浮点数表达式"""
 
 
 @final
-class NumberPattern(BasePattern[Union[int, float], Any]):
+class NumberPattern(BasePattern[Union[int, float], Any, Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(self):
-        super().__init__(mode=MatchMode.TYPE_CONVERT, origin=Union[int, float], alias="number")
+        super().__init__(mode=MatchMode.TYPE_CONVERT, origin=Union[int, float], alias="number")  # type: ignore
 
-    def match(self, input_: Any) -> float:
+    def match(self, input_: Any) -> int | float:
         if isinstance(input_, (float, int)):
             return input_
         try:
             res = float(input_)
             return int(res) if res.is_integer() else res
         except (ValueError, TypeError) as e:
             raise MatchFailed(
@@ -617,15 +620,15 @@
 
 
 NUMBER = NumberPattern()
 """一般数表达式，既可以浮点数也可以整数 """
 
 
 @final
-class BoolPattern(BasePattern[bool, Any]):
+class BoolPattern(BasePattern[bool, Union[str, bytes, bool], Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(self):
         super().__init__(mode=MatchMode.TYPE_CONVERT, origin=bool, alias="bool")
 
     def match(self, input_: Any) -> bool:
         if input_ is True or input_ is False:
             return input_
         if isinstance(input_, bytes):  # pragma: no cover
@@ -645,15 +648,15 @@
 
 
 BOOLEAN = BoolPattern()
 """布尔表达式，只能接受true或false样式的量"""
 
 
 @final
-class WideBoolPattern(BasePattern[bool, Any]):
+class WideBoolPattern(BasePattern[bool, Any, Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(self):
         super().__init__(mode=MatchMode.TYPE_CONVERT, origin=bool, alias="bool")
 
     BOOL_FALSE = {0, '0', 'off', 'f', 'false', 'n', 'no'}
     BOOL_TRUE = {1, '1', 'on', 't', 'true', 'y', 'yes'}
 
     def match(self, input_: Any) -> bool:
@@ -704,15 +707,15 @@
     MatchMode.REGEX_MATCH,
     alias="url",
 )
 """匹配网页链接的表达式"""
 
 
 @final
-class HexPattern(BasePattern[int, str]):
+class HexPattern(BasePattern[int, str, Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(self):
         super().__init__(mode=MatchMode.TYPE_CONVERT, origin=int, alias="hex", accepts=str)
 
     def match(self, input_: str) -> int:
         if not isinstance(input_, str):
             raise MatchFailed(
                 lang.require("nepattern", "type_error").format(
@@ -734,15 +737,15 @@
 """匹配16进制数的表达式"""
 
 HEX_COLOR = BasePattern(r"(#[0-9a-fA-F]{6})", MatchMode.REGEX_CONVERT, str, lambda _, x: x[1][1:], "color")
 """匹配16进制颜色代码的表达式"""
 
 
 @final
-class DateTimePattern(BasePattern[datetime, Union[str, int, float]]):
+class DateTimePattern(BasePattern[datetime, Union[str, int, float], Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(self):
         super().__init__(
             mode=MatchMode.TYPE_CONVERT, origin=datetime, alias="datetime", accepts=Union[str, int, float]
         )
 
     def match(self, input_: Union[str, int, float]) -> datetime:
         if isinstance(input_, (int, float)):
@@ -760,15 +763,15 @@
 
 
 DATETIME = DateTimePattern()
 """匹配时间的表达式"""
 
 
 @final
-class PathPattern(BasePattern[Path, Any]):
+class PathPattern(BasePattern[Path, Any, Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(self):
         super().__init__(mode=MatchMode.TYPE_CONVERT, origin=Path, alias="path")
 
     def match(self, input_: Any) -> Path:
         if isinstance(input_, Path):
             return input_
 
@@ -789,7 +792,36 @@
     mode=MatchMode.TYPE_CONVERT,
     origin=bytes,
     accepts=Path,
     previous=PATH,
     alias="filedata",
     converter=lambda _, x: x.read_bytes() if x.exists() and x.is_file() else None,
 )
+
+
+def combine(
+    current: BasePattern[TOrigin, TInput, TMM],
+    previous: BasePattern[Any, Any, Literal[MatchMode.VALUE_OPERATE]] | None = None,
+    alias: str | None = None,
+    validators: list[Callable[[TOrigin], bool]] | None = None,
+) -> BasePattern[TOrigin, TInput, TMM]:
+    _new = current.copy()
+    if previous:
+        _match = _new.match
+
+        def match(self, input_):
+            return _match(previous.match(input_))
+
+        _new.match = match.__get__(_new)
+    if alias:
+        _new.alias = alias
+        _new.refresh()
+    if validators:
+        _new.validators = validators
+    return _new
+
+
+DelimiterInt = combine(
+    INTEGER,
+    BasePattern(mode=MatchMode.VALUE_OPERATE, origin=str, converter=lambda _, x: x.replace(",", "_")),
+    "DelimInt",
+)
```

### Comparing `nepattern-0.6.5/nepattern/context.py` & `nepattern-0.7.0/nepattern/context.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.6.5/nepattern/context.pyi` & `nepattern-0.7.0/nepattern/context.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 
 from .core import BasePattern
 
 @final
 class Patterns(UserDict[Any, BasePattern]):
     name: str
     def __init__(self, name: str): ...
-    def set(self, target: BasePattern, alias: str | None = None, cover: bool = True, no_alias=False):
+    def set(self, target: BasePattern[Any, Any, Any], alias: str | None = None, cover: bool = True, no_alias=False):
         """
         增加可使用的类型转换器
 
         Args:
             target: 设置的表达式
             alias: 目标类型的别名
             cover: 是否覆盖已有的转换器
             no_alias: 是否不使用目标类型自带的别名
         """
         ...
-    def sets(self, patterns: Iterable[BasePattern], cover: bool = True, no_alias=False): ...
-    def merge(self, patterns: dict[str, BasePattern], no_alias=False): ...
+    def sets(self, patterns: Iterable[BasePattern[Any, Any, Any]], cover: bool = True, no_alias=False): ...
+    def merge(self, patterns: dict[str, BasePattern[Any, Any, Any]], no_alias=False): ...
     def remove(self, origin_type: type, alias: str | None = None): ...
 
 def create_local_patterns(
     name: str,
-    data: dict[Any, BasePattern] | None = None,
+    data: dict[Any, BasePattern[Any, Any, Any]] | None = None,
     set_current: bool = True,
 ) -> Patterns:
     """
     新建一个本地表达式组
 
     Args:
         name: 组名
```

### Comparing `nepattern-0.6.5/nepattern/main.py` & `nepattern-0.7.0/nepattern/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from collections.abc import MutableMapping as ABCMuMap
 from collections.abc import MutableSequence as ABCMuSeq
 from collections.abc import MutableSet as ABCMuSet
 from collections.abc import Sequence as ABCSeq
 from collections.abc import Set as ABCSet
 from contextlib import suppress
 from copy import deepcopy
-from functools import lru_cache
 import inspect
 from types import FunctionType, LambdaType, MethodType
 from typing import Any, ForwardRef, Literal, TypeVar, Union, runtime_checkable
 from typing_extensions import Annotated, get_args, get_origin
 
 from tarina.lang import lang
 
@@ -67,15 +66,15 @@
 def _typevar_parser(item: TypeVar):
     return BasePattern(mode=MatchMode.KEEP, origin=Any, alias=f"{item}"[1:], accepts=item)  # type: ignore
 
 
 def _protocol_parser(item: type):
     if not getattr(item, "_is_runtime_protocol", True):  # pragma: no cover
         item = runtime_checkable(deepcopy(item))  # type: ignore
-    return BasePattern(mode=MatchMode.KEEP, origin=Any, alias=f"{item}", accepts=item)
+    return BasePattern(mode=MatchMode.KEEP, alias=f"{item}", accepts=item)
 
 
 def parser(item: Any, extra: str = "allow") -> BasePattern:
     """对数类型的检查， 将一般数据类型转为 BasePattern 或者特殊类型"""
     if isinstance(item, BasePattern):
         return item
     with suppress(TypeError):
@@ -105,15 +104,15 @@
             return BasePattern(pat, MatchMode.REGEX_MATCH, alias=f"'{pat}'")
         if item.startswith("rep:"):
             pat = item[4:]
             return RegexPattern(pat, alias=f"'{pat}'")
         if "|" in item:
             names = item.split("|")
             return UnionPattern(all_patterns().get(i, i) for i in names if i)
-        return DirectPattern(item)
+        return DirectPattern(item, alias=f"'{item}'")
     if isinstance(item, RawStr):
         return DirectPattern(item.value, alias=f"'{item.value}'")
     if isinstance(item, (list, tuple, set, ABCSeq, ABCMuSeq, ABCSet, ABCMuSet)):  # Args[foo, [123, int]]
         return UnionPattern(map(lambda x: parser(x) if inspect.isclass(x) else x, item))
     if isinstance(item, (dict, ABCMap, ABCMuMap)):
         return SwitchPattern(dict(item))
     if isinstance(item, ForwardRef):
@@ -123,32 +122,8 @@
     if extra == "ignore":
         return ANY
     elif extra == "reject":
         raise TypeError(lang.require("nepattern", "validate_reject").format(target=item))
     return BasePattern.of(item) if inspect.isclass(item) else BasePattern.on(item)
 
 
-class Bind:
-    __slots__ = ()
-
-    def __new__(cls, *args, **kwargs):  # pragma: no cover
-        raise TypeError("Type Bind cannot be instantiated.")
-
-    @classmethod
-    @lru_cache(maxsize=None)
-    def __class_getitem__(cls, params) -> BasePattern:
-        if not isinstance(params, tuple) or len(params) < 2:
-            raise TypeError("Bind[...] should be used with only two arguments (a type and an annotation).")
-        if not (
-            pattern := params[0] if isinstance(params[0], BasePattern) else all_patterns().get(params[0])
-        ):
-            raise ValueError("Bind[...] first argument should be a BasePattern.")
-        if not all(callable(i) or isinstance(i, str) for i in params[1:]):
-            raise TypeError("Bind[...] second argument should be a callable or str.")
-        pattern = deepcopy(pattern)
-        pattern.alias = al[0] if (al := [i for i in params[1:] if isinstance(i, str)]) else pattern.alias
-        pattern.refresh()
-        pattern.validators.extend(filter(callable, params[1:]))
-        return pattern
-
-
-__all__ = ["Bind", "parser"]
+__all__ = ["parser"]
```

### Comparing `nepattern-0.6.5/nepattern/main.pyi` & `nepattern-0.7.0/nepattern/main.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,53 @@
 from collections.abc import Mapping as ABCMap
-from collections.abc import MutableMapping as ABCMuMap
 from collections.abc import MutableSequence as ABCMuSeq
-from collections.abc import MutableSet as ABCMuSet
-from collections.abc import Sequence as ABCSeq
 from collections.abc import Set as ABCSet
-from functools import lru_cache
-from typing import Any, Callable, ForwardRef, Iterable, TypeVar, overload
+from types import UnionType
+from typing import Any, Callable, ForwardRef, Iterable, TypeVar, overload, Literal
 
 from .base import (
     DirectPattern,
     DirectTypePattern,
     ForwardRefPattern,
     MappingPattern,
     RegexPattern,
     SequencePattern,
     SwitchPattern,
     UnionPattern,
+    IterMode
 )
-from .core import BasePattern
+from .core import BasePattern, MatchMode
 from .util import RawStr, TPattern
 
 T1 = TypeVar("T1")
 T2 = TypeVar("T2")
 
 @overload
 def parser(
     item: str, extra: str = "allow"
-) -> BasePattern[str, str] | DirectPattern[str] | RegexPattern | UnionPattern: ...
+) -> BasePattern[str, str, Literal[MatchMode.REGEX_MATCH]] | DirectPattern[str] | RegexPattern | UnionPattern: ...
 @overload
 def parser(item: RawStr, extra: str = "allow") -> DirectPattern[str]: ...
 @overload
 def parser(item: TPattern, extra: str = "allow") -> RegexPattern: ...
 @overload
-def parser(item: type[ABCMap[T1, T2]], extra: str = "allow") -> MappingPattern[T1, T2]: ...
+def parser(item: type[ABCMap[T1, T2]], extra: str = "allow") -> MappingPattern[T1, T2, Literal[IterMode.ALL]]: ...
 @overload
-def parser(item: type[ABCMuSeq[T1]], extra: str = "allow") -> SequencePattern[list[T1]]: ...
+def parser(item: type[ABCMuSeq[T1]], extra: str = "allow") -> SequencePattern[list[T1], Literal[IterMode.ALL]]: ...
 @overload
-def parser(item: type[tuple[T1, ...]], extra: str = "allow") -> SequencePattern[tuple[T1, ...]]: ...
+def parser(item: type[tuple[T1, ...]], extra: str = "allow") -> SequencePattern[tuple[T1, ...], Literal[IterMode.ALL]]: ...
 @overload
-def parser(item: type[ABCSet[T1]], extra: str = "allow") -> SequencePattern[set[T1]]: ...
+def parser(item: type[ABCSet[T1]], extra: str = "allow") -> SequencePattern[set[T1], Literal[IterMode.ALL]]: ...
 @overload
-def parser(item: type[T1], extra: str = "allow") -> BasePattern[T1, Any] | DirectTypePattern[T1]: ...
+def parser(item: type[T1], extra: str = "allow") -> BasePattern[T1, Any, Any] | DirectTypePattern[T1]: ...
 @overload
 def parser(item: ABCMap[T1, T2], extra: str = "allow") -> SwitchPattern[T2, T1]: ...
 @overload
+def parser(item: UnionType, extra: str = "allow") -> UnionPattern[Any]: ...
+@overload
 def parser(item: Iterable[T1 | type[T1]], extra: str = "allow") -> UnionPattern[T1]: ...
 @overload
-def parser(item: ForwardRef, extra: str = "allow") -> ForwardRefPattern[Any, Any]: ...
+def parser(item: ForwardRef, extra: str = "allow") -> ForwardRefPattern: ...
 @overload
-def parser(item: Callable[[T1], T2], extra: str = "allow") -> BasePattern[T2, T1]: ...
+def parser(item: Callable[[T1], T2], extra: str = "allow") -> BasePattern[T2, T1, Literal[MatchMode.TYPE_CONVERT]]: ...
 @overload
-def parser(item: T1, extra: str = "allow") -> BasePattern[T1, T1]: ...
-
-class Bind:
-    @classmethod
-    @lru_cache(maxsize=None)
-    def __class_getitem__(cls, params) -> BasePattern: ...
+def parser(item: T1, extra: str = "allow") -> BasePattern[T1, T1, Literal[MatchMode.KEEP]]: ...
```

### Comparing `nepattern-0.6.5/nepattern/util.py` & `nepattern-0.7.0/nepattern/util.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.6.5/pyproject.toml` & `nepattern-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nepattern"
-version = "0.6.5"
+version = "0.7.0"
 description = "a complex pattern, support typing"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
     "tarina>=0.4.1",
@@ -34,17 +34,17 @@
 [project.urls]
 repository = "https://github.com/ArcletProject/NEPattern"
 
 [project.optional-dependencies]
 
 [build-system]
 requires = [
-    "pdm-pep517>=1.0.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [tool.pdm.build]
 includes = [
     "nepattern",
 ]
 
 [tool.pdm.dev-dependencies]
```

### Comparing `nepattern-0.6.5/README.md` & `nepattern-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `nepattern-0.6.5/PKG-INFO` & `nepattern-0.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: nepattern
-Version: 0.6.5
+Version: 0.7.0
 Summary: a complex pattern, support typing
-License: MIT
 Keywords: typing,pattern,converter,validator
-Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
-Requires-Python: >=3.8
+Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
+License: MIT
+Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Typing :: Typed
-Project-URL: repository, https://github.com/ArcletProject/NEPattern
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Project-URL: Repository, https://github.com/ArcletProject/NEPattern
+Requires-Python: >=3.8
+Requires-Dist: typing-extensions>=4.5.0
+Requires-Dist: tarina>=0.4.1
 Description-Content-Type: text/markdown
 
 # NEPattern
 
 [![Licence](https://img.shields.io/github/license/ArcletProject/NEPattern)](https://github.com/ArcletProject/NEPattern/blob/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/nepattern)](https://pypi.org/project/nepattern)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nepattern)](https://www.python.org/)
@@ -38,8 +40,8 @@
 ```
 
 ## 特点
 
 - 高效的类型转化功能
 - 多种预置的实例
 - 良好的 typing 支持
-- 自由的环境控制
+- 自由的环境控制
```


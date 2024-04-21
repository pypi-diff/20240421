# Comparing `tmp/foamlib-0.3.3.tar.gz` & `tmp/foamlib-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foamlib-0.3.3.tar", last modified: Fri Apr 19 14:34:29 2024, max compression
+gzip compressed data, was "foamlib-0.3.4.tar", last modified: Sun Apr 21 19:24:40 2024, max compression
```

## Comparing `foamlib-0.3.3.tar` & `foamlib-0.3.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:29.014319 foamlib-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-19 14:34:24.000000 foamlib-0.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-19 14:34:29.014319 foamlib-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-19 14:34:24.000000 foamlib-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:29.010319 foamlib-0.3.3/foamlib/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20563 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:29.014319 foamlib-0.3.3/foamlib/_files/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_files/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_files/_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_files/_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_files/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_files/_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_files/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:24.000000 foamlib-0.3.3/foamlib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:29.014319 foamlib-0.3.3/foamlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-19 14:34:29.000000 foamlib-0.3.3/foamlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-19 14:34:29.000000 foamlib-0.3.3/foamlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:34:29.000000 foamlib-0.3.3/foamlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-19 14:34:29.000000 foamlib-0.3.3/foamlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 14:34:29.000000 foamlib-0.3.3/foamlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-19 14:34:24.000000 foamlib-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:34:29.014319 foamlib-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:24:40.089274 foamlib-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-21 19:24:35.000000 foamlib-0.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-21 19:24:40.085273 foamlib-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-21 19:24:35.000000 foamlib-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:24:40.081273 foamlib-0.3.4/foamlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20567 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:24:40.085273 foamlib-0.3.4/foamlib/_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_files/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_files/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_files/_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_files/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_files/_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_files/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:24:40.085273 foamlib-0.3.4/foamlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-21 19:24:40.000000 foamlib-0.3.4/foamlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-21 19:24:40.000000 foamlib-0.3.4/foamlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:24:40.000000 foamlib-0.3.4/foamlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-21 19:24:40.000000 foamlib-0.3.4/foamlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 19:24:40.000000 foamlib-0.3.4/foamlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-21 19:24:35.000000 foamlib-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:24:40.089274 foamlib-0.3.4/setup.cfg
```

### Comparing `foamlib-0.3.3/LICENSE.txt` & `foamlib-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.3/PKG-INFO` & `foamlib-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

### Comparing `foamlib-0.3.3/README.md` & `foamlib-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.3/foamlib/_cases.py` & `foamlib-0.3.4/foamlib/_cases.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         def __len__(self) -> int:
             return len(list(iter(self)))
 
         def __fspath__(self) -> str:
             return str(self.path)
 
         def __repr__(self) -> str:
-            return f"{type(self).__name__}({self.path})"
+            return f"{type(self).__name__}('{self.path}')"
 
         def __str__(self) -> str:
             return str(self.path)
 
     @property
     def _times(self) -> Sequence["FoamCaseBase.TimeDirectory"]:
         times = []
@@ -294,15 +294,15 @@
         """The turbulenceProperties file."""
         return self.file("constant/turbulenceProperties")
 
     def __fspath__(self) -> str:
         return str(self.path)
 
     def __repr__(self) -> str:
-        return f"{type(self).__name__}({self.path})"
+        return f"{type(self).__name__}('{self.path}')"
 
     def __str__(self) -> str:
         return str(self.path)
 
 
 class FoamCase(FoamCaseBase):
     """
```

### Comparing `foamlib-0.3.3/foamlib/_files/_base.py` & `foamlib-0.3.4/foamlib/_files/_base.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.3/foamlib/_files/_fields.py` & `foamlib-0.3.4/foamlib/_files/_fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,20 @@
             "np.ndarray[Tuple[int], np.dtype[np.generic]]",
             "np.ndarray[Tuple[int, int], np.dtype[np.generic]]",
         ]:
             """Alias of `self["value"]`."""
             ret = self["value"]
             if not isinstance(ret, (int, float, Sequence)):
                 raise TypeError("value is not a field")
-            return cast(Union[int, float, Sequence[Union[int, float]]], ret)
+            return cast(
+                Union[
+                    int, float, Sequence[Union[int, float, Sequence[Union[int, float]]]]
+                ],
+                ret,
+            )
 
         @value.setter
         def value(
             self,
             value: Union[
                 int,
                 float,
@@ -107,15 +112,15 @@
             self._setitem(keywords, value, assume_field=True)
         elif keywords == ("dimensions",):
             self._setitem(keywords, value, assume_dimensions=True)
         else:
             self._setitem(keywords, value)
 
     @property
-    def dimensions(self) -> FoamFile.DimensionSet:
+    def dimensions(self) -> Union[FoamFile.DimensionSet, Sequence[Union[int, float]]]:
         """Alias of `self["dimensions"]`."""
         ret = self["dimensions"]
         if not isinstance(ret, FoamFile.DimensionSet):
             raise TypeError("dimensions is not a DimensionSet")
         return ret
 
     @dimensions.setter
```

### Comparing `foamlib-0.3.3/foamlib/_files/_files.py` & `foamlib-0.3.4/foamlib/_files/_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if sys.version_info >= (3, 9):
     from collections.abc import Iterator, Mapping, MutableMapping
 else:
     from typing import Iterator, Mapping, MutableMapping
 
 from ._base import FoamDict
 from ._io import FoamFileIO
-from ._serialization import dumps
+from ._serialization import dumpb
 
 
 class FoamFile(
     FoamDict,
     MutableMapping[
         Union[str, Tuple[str, ...]], Union["FoamFile.Data", "FoamFile.SubDict"]
     ],
@@ -80,15 +80,15 @@
                 super().update(*args, **kwargs)
 
         def clear(self) -> None:
             with self._file:
                 super().clear()
 
         def __repr__(self) -> str:
-            return f"{type(self).__qualname__}({self._file}, {self._keywords})"
+            return f"{type(self).__qualname__}('{self._file}', {self._keywords})"
 
         def as_dict(self) -> FoamDict._Dict:
             """Return a nested dict representation of the dictionary."""
             ret = self._file.as_dict()
 
             for k in self._keywords:
                 assert isinstance(ret, dict)
@@ -109,14 +109,18 @@
         value = parsed[keywords]
 
         if value is ...:
             return FoamFile.SubDict(self, keywords)
         else:
             return value  # type: ignore [return-value]
 
+    @property
+    def _binary(self) -> bool:
+        return self.get(("FoamFile", "format"), None) == "binary"
+
     def _setitem(
         self,
         keywords: Union[str, Tuple[str, ...]],
         data: "FoamFile._SetData",
         *,
         assume_field: bool = False,
         assume_dimensions: bool = False,
@@ -130,24 +134,37 @@
             with self:
                 if isinstance(data, FoamDict):
                     data = data.as_dict()
 
                 start, end = parsed.entry_location(keywords, missing_ok=True)
 
                 self._write(
-                    f"{contents[:start]}\n{dumps({keywords[-1]: {}})}\n{contents[end:]}"
+                    contents[:start]
+                    + b"\n"
+                    + dumpb({keywords[-1]: {}})
+                    + b"\n"
+                    + contents[end:]
                 )
 
                 for k, v in data.items():
                     self[(*keywords, k)] = v
         else:
             start, end = parsed.entry_location(keywords, missing_ok=True)
 
             self._write(
-                f"{contents[:start]}\n{dumps({keywords[-1]: data}, assume_field=assume_field, assume_dimensions=assume_dimensions)}\n{contents[end:]}"
+                contents[:start]
+                + b"\n"
+                + dumpb(
+                    {keywords[-1]: data},
+                    assume_field=assume_field,
+                    assume_dimensions=assume_dimensions,
+                    binary_fields=self._binary,
+                )
+                + b"\n"
+                + contents[end:]
             )
 
     def __setitem__(
         self,
         keywords: Union[str, Tuple[str, ...]],
         data: "FoamFile._SetData",
     ) -> None:
@@ -190,14 +207,11 @@
     def clear(self) -> None:
         with self:
             super().clear()
 
     def __fspath__(self) -> str:
         return str(self.path)
 
-    def __repr__(self) -> str:
-        return f"{type(self).__name__}({self.path})"
-
     def as_dict(self) -> FoamDict._Dict:
         """Return a nested dict representation of the file."""
         _, parsed = self._read()
         return parsed.as_dict()
```

### Comparing `foamlib-0.3.3/foamlib/_files/_io.py` & `foamlib-0.3.4/foamlib/_files/_io.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def __init__(self, path: Union[str, Path]) -> None:
         self.path = Path(path).absolute()
         if self.path.is_dir():
             raise IsADirectoryError(self.path)
         elif not self.path.is_file():
             raise FileNotFoundError(self.path)
 
-        self.__contents: Optional[str] = None
+        self.__contents: Optional[bytes] = None
         self.__parsed: Optional[Parsed] = None
         self.__defer_io = 0
         self.__dirty = False
 
     def __enter__(self) -> Self:
         if self.__defer_io == 0:
             self._read()
@@ -44,30 +44,33 @@
     ) -> None:
         self.__defer_io -= 1
         if self.__defer_io == 0 and self.__dirty:
             assert self.__contents is not None
             self._write(self.__contents)
         assert not self.__dirty
 
-    def _read(self) -> Tuple[str, Parsed]:
+    def _read(self) -> Tuple[bytes, Parsed]:
         if not self.__defer_io:
-            contents = self.path.read_text()
+            contents = self.path.read_bytes()
             if contents != self.__contents:
                 self.__contents = contents
                 self.__parsed = None
 
         assert self.__contents is not None
 
         if self.__parsed is None:
             parsed = Parsed(self.__contents)
             self.__parsed = parsed
 
         return self.__contents, deepcopy(self.__parsed)
 
-    def _write(self, contents: str) -> None:
+    def _write(self, contents: bytes) -> None:
         self.__contents = contents
         self.__parsed = None
         if not self.__defer_io:
-            self.path.write_text(contents)
+            self.path.write_bytes(contents)
             self.__dirty = False
         else:
             self.__dirty = True
+
+    def __repr__(self) -> str:
+        return f"{type(self).__name__}('{self.path}')"
```

### Comparing `foamlib-0.3.3/foamlib/_files/_parsing.py` & `foamlib-0.3.4/foamlib/_files/_parsing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import array
 import sys
 from typing import Tuple, Union
 
 if sys.version_info >= (3, 9):
     from collections.abc import Iterator, Mapping, MutableMapping, Sequence
 else:
     from typing import Iterator, Mapping, MutableMapping, Sequence
 
 if sys.version_info >= (3, 10):
     from types import EllipsisType
 else:
     from typing import Any as EllipsisType
 
 from pyparsing import (
+    CharsNotIn,
     Dict,
     Forward,
     Group,
     Keyword,
     LineEnd,
     Literal,
     Located,
@@ -70,29 +72,81 @@
         keyword_entry = Located(keyword_entry)
 
     subdict <<= Dict(Group(keyword_entry)[...], asdict=not located)
 
     return Dict(Group(keyword_entry)[len], asdict=not located)
 
 
+_binary_contents = Forward()
+
+
+def _binary_field_parse_action(tks: ParseResults) -> None:
+    global _binary_contents
+
+    kind, count = tks
+    if kind == "scalar":
+        elsize = 1
+    elif kind == "vector":
+        elsize = 3
+    elif kind == "symmTensor":
+        elsize = 6
+    elif kind == "tensor":
+        elsize = 9
+
+    def unpack(
+        tks: ParseResults,
+    ) -> Sequence[Union[Sequence[float], Sequence[Sequence[float]]]]:
+        bytes_ = tks[0].encode("latin-1")
+
+        arr = array.array("d", bytes_)
+
+        if elsize != 1:
+            all = [arr[i : i + elsize].tolist() for i in range(0, len(arr), elsize)]
+        else:
+            all = arr.tolist()
+
+        return [all]
+
+    _binary_contents <<= CharsNotIn(exact=count * elsize * 8).set_parse_action(unpack)
+
+    tks.clear()  # type: ignore [no-untyped-call]
+
+
+_BINARY_FIELD = (
+    (
+        Keyword("nonuniform").suppress()
+        + Literal("List").suppress()
+        + Literal("<").suppress()
+        + common.identifier
+        + Literal(">").suppress()
+        + common.integer
+        + Literal("(").suppress()
+    ).set_parse_action(_binary_field_parse_action, call_during_try=True)
+    + _binary_contents
+    + Literal(")").suppress()
+)
+
+
 _SWITCH = (
     Keyword("yes") | Keyword("true") | Keyword("on") | Keyword("y") | Keyword("t")
 ).set_parse_action(lambda: True) | (
     Keyword("no") | Keyword("false") | Keyword("off") | Keyword("n") | Keyword("f")
 ).set_parse_action(lambda: False)
 _DIMENSIONS = (
     Literal("[").suppress() + common.number * 7 + Literal("]").suppress()
 ).set_parse_action(lambda tks: FoamDict.DimensionSet(*tks))
 _TENSOR = _list_of(common.number) | common.number
 _IDENTIFIER = Word(identchars + "$", printables, exclude_chars=";")
 _DIMENSIONED = (Opt(_IDENTIFIER) + _DIMENSIONS + _TENSOR).set_parse_action(
     lambda tks: FoamDict.Dimensioned(*reversed(tks.as_list()))
 )
-_FIELD = (Keyword("uniform").suppress() + _TENSOR) | (
-    Keyword("nonuniform").suppress() + _list_of(_TENSOR)
+_FIELD = (
+    (Keyword("uniform").suppress() + _TENSOR)
+    | (Keyword("nonuniform").suppress() + _list_of(_TENSOR))
+    | _BINARY_FIELD
 )
 _TOKEN = QuotedString('"', unquote_results=False) | _IDENTIFIER
 _DATA = Forward()
 _KEYWORD_ENTRY = _dictionary_of(_TOKEN, _DATA, len=1)
 _DATA_ENTRY = Forward()
 _LIST_ENTRY = _KEYWORD_ENTRY | _DATA_ENTRY
 _LIST = _list_of(_LIST_ENTRY)
@@ -105,24 +159,27 @@
 )
 
 _FILE = (
     _dictionary_of(_TOKEN, Opt(_DATA, default=""), located=True)
     .ignore(c_style_comment)
     .ignore(cpp_style_comment)
     .ignore(Literal("#include") + ... + LineEnd())  # type: ignore [no-untyped-call]
+    .parse_with_tabs()
 )
 
 
 class Parsed(Mapping[Tuple[str, ...], Union[FoamDict.Data, EllipsisType]]):
-    def __init__(self, contents: str) -> None:
+    def __init__(self, contents: bytes) -> None:
         self._parsed: MutableMapping[
             Tuple[str, ...],
             Tuple[int, Union[FoamDict.Data, EllipsisType], int],
         ] = {}
-        for parse_result in _FILE.parse_string(contents, parse_all=True):
+        for parse_result in _FILE.parse_string(
+            contents.decode("latin-1"), parse_all=True
+        ):
             self._parsed.update(self._flatten_result(parse_result))
 
     @staticmethod
     def _flatten_result(
         parse_result: ParseResults, *, _keywords: Tuple[str, ...] = ()
     ) -> Mapping[Tuple[str, ...], Tuple[int, Union[FoamDict.Data, EllipsisType], int]]:
         ret: MutableMapping[
```

### Comparing `foamlib-0.3.3/foamlib/_files/_serialization.py` & `foamlib-0.3.4/foamlib/_files/_serialization.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import array
+import itertools
 import sys
 
 if sys.version_info >= (3, 9):
     from collections.abc import Mapping
 else:
     from typing import Mapping
 
@@ -12,88 +14,125 @@
     import numpy as np
 
     numpy = True
 except ModuleNotFoundError:
     numpy = False
 
 
-def dumps(
+def dumpb(
     data: FoamDict._SetData,
     *,
     assume_field: bool = False,
     assume_dimensions: bool = False,
     assume_data_entries: bool = False,
-) -> str:
+    binary_fields: bool = False,
+) -> bytes:
     if numpy and isinstance(data, np.ndarray):
-        return dumps(
+        return dumpb(
             data.tolist(),
             assume_field=assume_field,
             assume_dimensions=assume_dimensions,
+            assume_data_entries=assume_data_entries,
+            binary_fields=binary_fields,
         )
 
     elif isinstance(data, Mapping):
         entries = []
         for k, v in data.items():
-            s = dumps(
+            b = dumpb(
                 v,
                 assume_field=assume_field,
                 assume_dimensions=assume_dimensions,
                 assume_data_entries=True,
+                binary_fields=binary_fields,
             )
             if isinstance(v, Mapping):
-                entries.append(f"{k}\n{{\n{s}\n}}")
-            elif s:
-                entries.append(f"{k} {s};")
+                entries.append(dumpb(k) + b"\n" + b"{\n" + b + b"\n}")
+            elif b:
+                entries.append(dumpb(k) + b" " + b + b";")
             else:
-                entries.append(f"{k};")
-        return "\n".join(entries)
+                entries.append(dumpb(k) + b";")
+
+        return b"\n".join(entries)
 
     elif isinstance(data, FoamDict.DimensionSet) or (
         assume_dimensions and is_sequence(data) and len(data) == 7
     ):
-        return f"[{' '.join(str(v) for v in data)}]"
+        return b"[" + b" ".join(dumpb(v) for v in data) + b"]"
 
-    elif assume_field and isinstance(data, (int, float)):
-        return f"uniform {data}"
+    elif assume_field and (
+        isinstance(data, (int, float))
+        or is_sequence(data)
+        and data
+        and isinstance(data[0], (int, float))
+        and len(data) in (3, 6, 9)
+    ):
+        return b"uniform " + dumpb(data)
 
     elif assume_field and is_sequence(data):
-        if isinstance(data[0], (int, float)) and len(data) in (3, 6, 9):
-            return f"uniform {dumps(data)}"
-        elif isinstance(data[0], (int, float)):
-            return f"nonuniform List<scalar> {len(data)}{dumps(data)}"
+        if isinstance(data[0], (int, float)):
+            kind = b"scalar"
         elif len(data[0]) == 3:
-            return f"nonuniform List<vector> {len(data)}{dumps(data)}"
+            kind = b"vector"
         elif len(data[0]) == 6:
-            return f"nonuniform List<symmTensor> {len(data)}{dumps(data)}"
+            kind = b"symmTensor"
         elif len(data[0]) == 9:
-            return f"nonuniform List<tensor> {len(data)}{dumps(data)}"
+            kind = b"tensor"
         else:
-            return dumps(
+            return dumpb(
                 data,
                 assume_dimensions=assume_dimensions,
                 assume_data_entries=assume_data_entries,
+                binary_fields=binary_fields,
             )
 
+        if binary_fields:
+            if kind == b"scalar":
+                contents = b"(" + array.array("d", data).tobytes() + b")"
+            else:
+                contents = (
+                    b"("
+                    + array.array("d", itertools.chain.from_iterable(data)).tobytes()
+                    + b")"
+                )
+        else:
+            contents = dumpb(data)
+
+        return b"nonuniform List<" + kind + b"> " + dumpb(len(data)) + contents
+
     elif assume_data_entries and isinstance(data, tuple):
-        return " ".join(
-            dumps(v, assume_field=assume_field, assume_dimensions=assume_dimensions)
+        return b" ".join(
+            dumpb(
+                v,
+                assume_field=assume_field,
+                assume_dimensions=assume_dimensions,
+                binary_fields=binary_fields,
+            )
             for v in data
         )
 
     elif isinstance(data, FoamDict.Dimensioned):
         if data.name is not None:
-            return f"{data.name} {dumps(data.dimensions, assume_dimensions=True)} {dumps(data.value)}"
+            return (
+                dumpb(data.name)
+                + b" "
+                + dumpb(data.dimensions, assume_dimensions=True)
+                + b" "
+                + dumpb(data.value)
+            )
         else:
             return (
-                f"{dumps(data.dimensions, assume_dimensions=True)} {dumps(data.value)}"
+                dumpb(data.dimensions, assume_dimensions=True)
+                + b" "
+                + dumpb(data.value)
             )
 
     elif is_sequence(data):
-        return f"({' '.join(dumps(v) for v in data)})"
+        return b"(" + b" ".join(dumpb(v) for v in data) + b")"
 
     elif data is True:
-        return "yes"
+        return b"yes"
     elif data is False:
-        return "no"
+        return b"no"
 
     else:
-        return str(data)
+        return str(data).encode("latin-1")
```

### Comparing `foamlib-0.3.3/foamlib/_util.py` & `foamlib-0.3.4/foamlib/_util.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.3/foamlib.egg-info/PKG-INFO` & `foamlib-0.3.4/foamlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

### Comparing `foamlib-0.3.3/pyproject.toml` & `foamlib-0.3.4/pyproject.toml`

 * *Files identical despite different names*


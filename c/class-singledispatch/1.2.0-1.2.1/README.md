# Comparing `tmp/class_singledispatch-1.2.0.tar.gz` & `tmp/class_singledispatch-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "class_singledispatch-1.2.0.tar", max compression
+gzip compressed data, was "class_singledispatch-1.2.1.tar", max compression
```

## Comparing `class_singledispatch-1.2.0.tar` & `class_singledispatch-1.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2024-04-20 20:58:52.285433 class_singledispatch-1.2.0/LICENSE
--rw-r--r--   0        0        0     5253 2024-04-20 20:58:52.285433 class_singledispatch-1.2.0/README.md
--rw-r--r--   0        0        0     5873 2024-04-20 20:58:52.285433 class_singledispatch-1.2.0/class_singledispatch/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 20:58:52.285433 class_singledispatch-1.2.0/class_singledispatch/py.typed
--rw-r--r--   0        0        0     5789 2024-04-20 20:58:52.289433 class_singledispatch-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     6356 1970-01-01 00:00:00.000000 class_singledispatch-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-21 12:08:46.311892 class_singledispatch-1.2.1/LICENSE
+-rw-r--r--   0        0        0     5257 2024-04-21 12:08:46.311892 class_singledispatch-1.2.1/README.md
+-rw-r--r--   0        0        0     5895 2024-04-21 12:08:46.311892 class_singledispatch-1.2.1/class_singledispatch/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-21 12:08:46.311892 class_singledispatch-1.2.1/class_singledispatch/py.typed
+-rw-r--r--   0        0        0     5792 2024-04-21 12:08:46.315892 class_singledispatch-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6360 1970-01-01 00:00:00.000000 class_singledispatch-1.2.1/PKG-INFO
```

### Comparing `class_singledispatch-1.2.0/LICENSE` & `class_singledispatch-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `class_singledispatch-1.2.0/README.md` & `class_singledispatch-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # <div align="center">class_singledispatch<br>[![skeleton](https://img.shields.io/badge/0.0.2rc–218–g8123b8a-skeleton?label=%F0%9F%92%80%20skeleton-ci/skeleton-python&labelColor=black&color=grey&link=https%3A//github.com/skeleton-ci/skeleton-python)](https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-218-g8123b8a) [![Supported Python versions](https://img.shields.io/pypi/pyversions/class-singledispatch.svg?logo=python&label=Python)](https://pypi.org/project/class-singledispatch/) [![Package version](https://img.shields.io/pypi/v/class-singledispatch?label=PyPI)](https://pypi.org/project/class-singledispatch/)</div>
 
 [![Tests](https://github.com/bswck/class_singledispatch/actions/workflows/test.yml/badge.svg)](https://github.com/bswck/class_singledispatch/actions/workflows/test.yml)
 [![Coverage](https://coverage-badge.samuelcolvin.workers.dev/bswck/class_singledispatch.svg)](https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/class_singledispatch)
 [![Documentation Status](https://readthedocs.org/projects/class-singledispatch/badge/?version=latest)](https://class-singledispatch.readthedocs.io/en/latest/?badge=latest)
 
-A ``singledispatch()`` for arguments that are classes annotated as specific types.
+A [``singledispatch()``](https://docs.python.org/3/library/functools.html#functools.singledispatch) for arguments that are classes annotated as specific types.
 
 Inspired by https://github.com/python/cpython/issues/100623.
 
 # A Simple Example
-Use `functools.singledispatch` to singledispatch classes as parameters.
-
 While `functools.singledispatch` examines the class of the first user argument,
 `class_singledispatch` uses the first argument as the class itself and performs
 the same task with it as `functools.singledispatch`.
 
 ```python
 from class_singledispatch import class_singledispatch
```

### Comparing `class_singledispatch-1.2.0/class_singledispatch/__init__.py` & `class_singledispatch-1.2.1/class_singledispatch/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 # SPDX-License-Identifier: MIT
 # (C) 2024-present Bartosz Sławecki (bswck)
 """
 `class_singledispatch`.
 
-A ``singledispatch()`` for arguments that are classes annotated as specific types.
+A [`singledispatch`][functools.singledispatch] for arguments that are classes
+annotated as specific types.
+
 https://github.com/python/cpython/issues/100623
 """
 
 from __future__ import annotations
 
 import sys
+from contextlib import suppress
 from functools import partial, singledispatch
-from types import MappingProxyType
 from typing import (
     TYPE_CHECKING,
     Any,
+    ForwardRef,
     Generic,
     Type,
     TypeVar,
     get_args,
     get_origin,
     get_type_hints,
 )
 
 if TYPE_CHECKING:
     from collections.abc import Callable
+    from types import MappingProxyType
     from typing import overload
 
-if sys.version_info < (3, 10):  # pragma: no cover
-    from typing_extensions import ParamSpec
 
-    OldFashionGenericAlias = GenericAlias = type(Type[object])
+OldFashionGenericAlias: type[object] = type(Type[object])
 
-else:  # pragma: no cover
+if sys.version_info < (3, 9):
+    GenericAlias = OldFashionGenericAlias
+else:
     from types import GenericAlias
-    from typing import ParamSpec
 
-    OldFashionGenericAlias = type(Type[object])
 
-try:
-    from eval_type_backport import ForwardRef  # type: ignore  # noqa: PGH003
-except ImportError:  # pragma: no cover
-    from typing import ForwardRef  # type: ignore  # noqa: PGH003
+if sys.version_info < (3, 10):
+    from typing_extensions import ParamSpec
+else:
+    from typing import ParamSpec
+
+with suppress(ImportError):
+    from eval_type_backport import ForwardRef  # noqa: F811
 
 
 __all__ = (
     "class_singledispatch",
     "resolve_annotated_type",
 )
 
@@ -135,15 +140,16 @@
         cls: type[Any] | Callable[..., _R],
         /,
         func: Callable[_P, _R] | None = None,
     ) -> Callable[_P, _R] | partial[Callable[_P, _R]]:
         """
         Register a new function as a dispatcher for `cls`.
 
-        For usage guide, please see the `class_singledispatch` documentation.
+        For usage guide, please see the [`class_singledispatch`][class_singledispatch]
+        documentation.
         """
         if isinstance(cls, type):
             if func is None:
                 return partial(self.register, cls)
         else:
             if func is not None:
                 msg = (
@@ -165,19 +171,20 @@
 
 
 def class_singledispatch(
     func: Callable[..., _R],
     /,
 ) -> _ClassSingleDispatchCallable[_R]:
     """
-    Use `functools.singledispatch` to singledispatch classes as parameters.
+    Use [`functools.singledispatch`][functools.singledispatch] to singledispatch
+    classes as parameters.
 
-    While `functools.singledispatch` examines the class of the first user argument,
-    `class_singledispatch` uses the first argument as the class itself and performs
-    the same task with it as `functools.singledispatch`.
+    While `singledispatch` examines the class of the first user argument,
+    [class_singledispatch][] uses the first argument as the class itself and performs
+    the same task with it as `singledispatch`.
 
     ```python
     class T:
         pass
 
     class OtherT:
         pass
@@ -196,9 +203,9 @@
     def on_some_other_class(cls: type[SomeOtherT], /) -> None:
         print("SomeOtherT!")
 
     on_class(T)  # T!
     on_class(OtherT)  #  OtherT!
     on_class(SomeOtherT)  #  SomeOtherT!
     ```
-    """
+    """  # noqa: D205
     return _ClassSingleDispatchCallable(func)
```

### Comparing `class_singledispatch-1.2.0/pyproject.toml` & `class_singledispatch-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was generated from skeleton-ci/skeleton-python@0.0.2rc-218-g8123b8a.
 # Instead of changing this particular file, you might want to alter the template:
 # https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-218-g8123b8a/project/pyproject.toml.jinja
 
 [tool.poetry]
 name = "class_singledispatch"
-version = "1.2.0"
+version = "1.2.1"
 description = "A ``singledispatch()`` for arguments that are classes annotated as specific types."
 authors = ["bswck <bartoszpiotrslawecki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "class_singledispatch/" }]
 homepage = "https://github.com/bswck/class_singledispatch"
 
@@ -41,14 +41,17 @@
 smokeshow = ">=0.4.0"
 keyring = ">=25.0.0"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
 
 
+
+
+
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 markdown-exec = ">=1.3.0"
 mkdocs-material = ">=8.2,<10.0.0"
 mkdocstrings = { version = ">=0.19.0", extras = ["python"] }
```

### Comparing `class_singledispatch-1.2.0/PKG-INFO` & `class_singledispatch-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: class_singledispatch
-Version: 1.2.0
+Version: 1.2.1
 Summary: A ``singledispatch()`` for arguments that are classes annotated as specific types.
 Home-page: https://github.com/bswck/class_singledispatch
 License: MIT
 Author: bswck
 Author-email: bartoszpiotrslawecki@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -23,21 +23,19 @@
 
 # <div align="center">class_singledispatch<br>[![skeleton](https://img.shields.io/badge/0.0.2rc–218–g8123b8a-skeleton?label=%F0%9F%92%80%20skeleton-ci/skeleton-python&labelColor=black&color=grey&link=https%3A//github.com/skeleton-ci/skeleton-python)](https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-218-g8123b8a) [![Supported Python versions](https://img.shields.io/pypi/pyversions/class-singledispatch.svg?logo=python&label=Python)](https://pypi.org/project/class-singledispatch/) [![Package version](https://img.shields.io/pypi/v/class-singledispatch?label=PyPI)](https://pypi.org/project/class-singledispatch/)</div>
 
 [![Tests](https://github.com/bswck/class_singledispatch/actions/workflows/test.yml/badge.svg)](https://github.com/bswck/class_singledispatch/actions/workflows/test.yml)
 [![Coverage](https://coverage-badge.samuelcolvin.workers.dev/bswck/class_singledispatch.svg)](https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/class_singledispatch)
 [![Documentation Status](https://readthedocs.org/projects/class-singledispatch/badge/?version=latest)](https://class-singledispatch.readthedocs.io/en/latest/?badge=latest)
 
-A ``singledispatch()`` for arguments that are classes annotated as specific types.
+A [``singledispatch()``](https://docs.python.org/3/library/functools.html#functools.singledispatch) for arguments that are classes annotated as specific types.
 
 Inspired by https://github.com/python/cpython/issues/100623.
 
 # A Simple Example
-Use `functools.singledispatch` to singledispatch classes as parameters.
-
 While `functools.singledispatch` examines the class of the first user argument,
 `class_singledispatch` uses the first argument as the class itself and performs
 the same task with it as `functools.singledispatch`.
 
 ```python
 from class_singledispatch import class_singledispatch
```


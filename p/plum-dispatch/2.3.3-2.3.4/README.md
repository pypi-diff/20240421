# Comparing `tmp/plum_dispatch-2.3.3.tar.gz` & `tmp/plum_dispatch-2.3.4.tar.gz`

## Comparing `plum_dispatch-2.3.3.tar` & `plum_dispatch-2.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/plum/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/plum/_version.py
--rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/plum/alias.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/plum/autoreload.py
--rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/plum/dispatcher.py
--rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/plum/function.py
--rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/plum/method.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/plum/overload.py
--rw-r--r--   0        0        0    14753 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/plum/parametric.py
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/plum/promotion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/plum/py.typed
--rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/plum/repr.py
--rw-r--r--   0        0        0    12283 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/plum/resolver.py
--rw-r--r--   0        0        0    13024 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/plum/signature.py
--rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/plum/type.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/plum/typing.py
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/plum/util.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/LICENCE.txt
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/README.md
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/pyproject.toml
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 plum_dispatch-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/plum/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/plum/_version.py
+-rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/plum/alias.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/plum/autoreload.py
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/plum/dispatcher.py
+-rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/plum/function.py
+-rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/plum/method.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/plum/overload.py
+-rw-r--r--   0        0        0    18043 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/plum/parametric.py
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/plum/promotion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/plum/py.typed
+-rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/plum/repr.py
+-rw-r--r--   0        0        0    12283 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/plum/resolver.py
+-rw-r--r--   0        0        0    13024 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/plum/signature.py
+-rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/plum/type.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/plum/typing.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/plum/util.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/LICENCE.txt
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/README.md
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 plum_dispatch-2.3.4/PKG-INFO
```

### Comparing `plum_dispatch-2.3.3/plum/__init__.py` & `plum_dispatch-2.3.4/plum/__init__.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.3/plum/alias.py` & `plum_dispatch-2.3.4/plum/alias.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.3/plum/autoreload.py` & `plum_dispatch-2.3.4/plum/autoreload.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.3/plum/dispatcher.py` & `plum_dispatch-2.3.4/plum/dispatcher.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.3/plum/function.py` & `plum_dispatch-2.3.4/plum/function.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.3/plum/method.py` & `plum_dispatch-2.3.4/plum/method.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.3/plum/parametric.py` & `plum_dispatch-2.3.4/plum/parametric.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-from typing import Union
+from typing import Type, TypeVar, Union
 
 import beartype.door
 from beartype.roar import BeartypeDoorNonpepException
 
 from .dispatcher import Dispatcher
 from .function import _owner_transfer
 from .repr import repr_short
 from .type import resolve_type_hint
 from .util import TypeHint
 
 __all__ = [
     "CovariantMeta",
     "parametric",
     "type_parameter",
+    "type_unparametrized",
     "kind",
     "Kind",
     "Val",
 ]
 
+T = TypeVar("T")
+
 
 _dispatch = Dispatcher()
 
 
 class ParametricTypeMeta(type):
     """Parametric types can be instantiated with indexing.
 
@@ -270,19 +273,90 @@
 
             def class_new(cls, *args, **kw_args):
                 return original_class.__new__(cls)
 
             cls.__new__ = class_new
         super(original_class, cls).__init_subclass__(**kw_args)
 
+    def __class_nonparametric__(cls):
+        """Return the non-parametric type of an object.
+
+        :mod:`plum.parametric` produces parametric subtypes of classes. This
+        method can be used to get the non-parametric type of an object.
+
+        Examples
+        --------
+        >>> from plum import parametric
+        >>> @parametric
+        ... class Obj:
+        ...     @classmethod
+        ...     def __infer_type_parameter__(cls, *arg):
+        ...         return type(arg[0])
+        ...     def __init__(self, x):
+        ...         self.x = x
+        ...     def __repr__(self):
+        ...         return f"Obj({self.x})"
+
+        >>> obj = Obj(1)
+        >>> obj
+        Obj(1)
+
+        >>> type(obj).mro()
+        [Obj[int], Obj, object]
+
+        >>> obj.__class_nonparametric__().mro()
+        [Obj, object]
+        """
+        return original_class
+
+    def __class_unparametrized__(cls):
+        """Return the unparametrized type of an object.
+
+        :mod:`plum.parametric` produces parametric subtypes of classes. This
+        method can be used to get the un-parametrized type of an object.
+
+        Examples
+        --------
+        >>> from plum import parametric
+        >>> @parametric
+        ... class Obj:
+        ...     @classmethod
+        ...     def __infer_type_parameter__(cls, *arg):
+        ...         return type(arg[0])
+        ...     def __init__(self, x):
+        ...         self.x = x
+        ...     def __repr__(self):
+        ...         return f"Obj({self.x})"
+
+        >>> obj = Obj(1)
+        >>> obj
+        Obj(1)
+
+        >>> type(obj).__name__
+        Obj[int]
+
+        >>> obj.__class_unparametrized__().mro()
+        [Obj, Obj, object]
+
+        Note that this is still NOT the 'original' non-`parametric`-wrapped
+        type.  This is the type that is wrapped by :mod:`plum.parametric`, but
+        without the inferred type parameter(s).
+        """
+        return parametric_class
+
     # Create parametric class.
     parametric_class = meta(
         original_class.__name__,
         (original_class,),
-        {"__new__": __new__, "__init_subclass__": __init_subclass__},
+        {
+            "__new__": __new__,
+            "__init_subclass__": __init_subclass__,
+            "__class_nonparametric__": __class_nonparametric__,
+            "__class_unparametrized__": __class_unparametrized__,
+        },
     )
     parametric_class._parametric = True
     parametric_class._concrete = False
     parametric_class.__module__ = original_class.__module__
 
     # When dispatch is used in methods of `original_class`, because we return
     # `parametric_class`, `parametric_class` will be inferred as the owner of those
@@ -352,14 +426,52 @@
         return t.type_parameter
     raise ValueError(
         f"`{x}` is not a concrete parametric type or an instance of a"
         f" concrete parametric type."
     )
 
 
+def type_unparametrized(q: T) -> Type[T]:
+    """Return the unparametrized type of an object.
+
+    :mod:`plum.parametric` produces parametric subtypes of classes.  This
+    function can be used to get the un-parametrized type of an object.
+    This function also works for normal, :mod:`plum.parametric`-wrapped classes.
+
+    Examples
+    --------
+    >>> from plum import parametric
+    >>> @parametric
+    ... class Obj:
+    ...     @classmethod
+    ...     def __infer_type_parameter__(cls, *arg):
+    ...         return type(arg[0])
+    ...     def __init__(self, x):
+    ...         self.x = x
+    ...     def __repr__(self):
+    ...         return f"Obj({self.x})"
+
+    >>> obj = Obj(1)
+    >>> obj
+    Obj(1)
+
+    >>> type(obj).__name__
+    Obj[int]
+
+    >>> type_unparametrized(obj).__name__
+    Obj
+
+    Note that this is still NOT the 'original' non-`parametric`-wrapped type.
+    This is the type that is wrapped by :mod:`plum.parametric`, but without the
+    inferred type parameter(s).
+    """
+    typ = type(q)
+    return q.__class_unparametrized__() if isinstance(typ, ParametricTypeMeta) else typ
+
+
 def kind(SuperClass=object):
     """Create a parametric wrapper type for dispatch purposes.
 
     Args:
         SuperClass (type): Super class.
 
     Returns:
```

### Comparing `plum_dispatch-2.3.3/plum/promotion.py` & `plum_dispatch-2.3.4/plum/promotion.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.3/plum/repr.py` & `plum_dispatch-2.3.4/plum/repr.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.3/plum/resolver.py` & `plum_dispatch-2.3.4/plum/resolver.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.3/plum/signature.py` & `plum_dispatch-2.3.4/plum/signature.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.3/plum/type.py` & `plum_dispatch-2.3.4/plum/type.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.3/plum/typing.py` & `plum_dispatch-2.3.4/plum/typing.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.3/plum/util.py` & `plum_dispatch-2.3.4/plum/util.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.3/LICENCE.txt` & `plum_dispatch-2.3.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.3/README.md` & `plum_dispatch-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.3/pyproject.toml` & `plum_dispatch-2.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.3/PKG-INFO` & `plum_dispatch-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: plum-dispatch
-Version: 2.3.3
+Version: 2.3.4
 Summary: Multiple dispatch in Python
 Project-URL: repository, https://github.com/beartype/plum
 Author-email: Wessel Bruinsma <wessel.p.bruinsma@gmail.com>
 License: MIT
 License-File: LICENCE.txt
 Keywords: multiple dispatch
 Classifier: Development Status :: 5 - Production/Stable
```


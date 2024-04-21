# Comparing `tmp/that_depends-1.6.0.tar.gz` & `tmp/that_depends-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "that_depends-1.6.0.tar", max compression
+gzip compressed data, was "that_depends-1.6.1.tar", max compression
```

## Comparing `that_depends-1.6.0.tar` & `that_depends-1.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     6711 2024-04-16 18:31:17.949107 that_depends-1.6.0/README.md
--rw-r--r--   0        0        0     1482 2024-04-21 11:37:07.035917 that_depends-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      164 2024-03-18 09:15:04.223171 that_depends-1.6.0/that_depends/__init__.py
--rw-r--r--   0        0        0      747 2024-04-11 11:51:20.009107 that_depends-1.6.0/that_depends/container.py
--rw-r--r--   0        0        0     1013 2024-04-15 19:32:21.955087 that_depends-1.6.0/that_depends/injection.py
--rw-r--r--   0        0        0      670 2024-04-21 11:20:54.815386 that_depends-1.6.0/that_depends/providers/__init__.py
--rw-r--r--   0        0        0      642 2024-04-16 06:00:18.298948 that_depends-1.6.0/that_depends/providers/base.py
--rw-r--r--   0        0        0      465 2024-04-16 06:00:22.046508 that_depends-1.6.0/that_depends/providers/collections.py
--rw-r--r--   0        0        0     3023 2024-04-21 11:29:23.822434 that_depends-1.6.0/that_depends/providers/context_resources.py
--rw-r--r--   0        0        0     1365 2024-04-16 06:00:22.046739 that_depends-1.6.0/that_depends/providers/factories.py
--rw-r--r--   0        0        0     2584 2024-04-19 13:06:26.477052 that_depends-1.6.0/that_depends/providers/resources.py
--rw-r--r--   0        0        0      993 2024-04-17 05:36:03.299156 that_depends-1.6.0/that_depends/providers/singleton.py
--rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.6.0/that_depends/py.typed
--rw-r--r--   0        0        0     7191 1970-01-01 00:00:00.000000 that_depends-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     6711 2024-04-16 18:31:17.949107 that_depends-1.6.1/README.md
+-rw-r--r--   0        0        0     1482 2024-04-21 11:48:31.807492 that_depends-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0      164 2024-03-18 09:15:04.223171 that_depends-1.6.1/that_depends/__init__.py
+-rw-r--r--   0        0        0      747 2024-04-11 11:51:20.009107 that_depends-1.6.1/that_depends/container.py
+-rw-r--r--   0        0        0     1013 2024-04-15 19:32:21.955087 that_depends-1.6.1/that_depends/injection.py
+-rw-r--r--   0        0        0      670 2024-04-21 11:20:54.815386 that_depends-1.6.1/that_depends/providers/__init__.py
+-rw-r--r--   0        0        0      642 2024-04-16 06:00:18.298948 that_depends-1.6.1/that_depends/providers/base.py
+-rw-r--r--   0        0        0      465 2024-04-16 06:00:22.046508 that_depends-1.6.1/that_depends/providers/collections.py
+-rw-r--r--   0        0        0     3025 2024-04-21 11:48:02.328277 that_depends-1.6.1/that_depends/providers/context_resources.py
+-rw-r--r--   0        0        0     1365 2024-04-16 06:00:22.046739 that_depends-1.6.1/that_depends/providers/factories.py
+-rw-r--r--   0        0        0     2586 2024-04-21 11:48:02.333485 that_depends-1.6.1/that_depends/providers/resources.py
+-rw-r--r--   0        0        0      993 2024-04-17 05:36:03.299156 that_depends-1.6.1/that_depends/providers/singleton.py
+-rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.6.1/that_depends/py.typed
+-rw-r--r--   0        0        0     7191 1970-01-01 00:00:00.000000 that_depends-1.6.1/PKG-INFO
```

### Comparing `that_depends-1.6.0/README.md` & `that_depends-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.0/pyproject.toml` & `that_depends-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "that-depends"
-version = "1.6.0"
+version = "1.6.1"
 description = "Simple Dependency Injection framework"
 authors = ["Artur Shiriev <me@shiriev.ru>"]
 readme = "README.md"
 homepage = "https://github.com/modern-python/that-depends"
 packages = [
     { include = "that_depends" },
 ]
```

### Comparing `that_depends-1.6.0/that_depends/container.py` & `that_depends-1.6.1/that_depends/container.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.0/that_depends/injection.py` & `that_depends-1.6.1/that_depends/injection.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.0/that_depends/providers/__init__.py` & `that_depends-1.6.1/that_depends/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.0/that_depends/providers/base.py` & `that_depends-1.6.1/that_depends/providers/base.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.0/that_depends/providers/context_resources.py` & `that_depends-1.6.1/that_depends/providers/context_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         await asyncio.gather(*[provider.tear_down() for _, provider in context.get().items()], return_exceptions=True)
         context.reset(token)
 
 
 class ContextResource(AbstractProvider[T]):
     def __init__(
         self,
-        creator: typing.Callable[[], typing.Iterator[T]],
+        creator: typing.Callable[..., typing.Iterator[T]],
         *args: typing.Any,  # noqa: ANN401
         **kwargs: typing.Any,  # noqa: ANN401
     ) -> None:
         if not inspect.isgeneratorfunction(creator):
             msg = "ContextResource must be generator function"
             raise RuntimeError(msg)
 
@@ -57,15 +57,15 @@
 
         return typing.cast(T, await _resource.resolve())
 
 
 class AsyncContextResource(AbstractProvider[T]):
     def __init__(
         self,
-        creator: typing.Callable[[], typing.AsyncIterator[T]],
+        creator: typing.Callable[..., typing.AsyncIterator[T]],
         *args: typing.Any,  # noqa: ANN401
         **kwargs: typing.Any,  # noqa: ANN401
     ) -> None:
         if not inspect.isasyncgenfunction(creator):
             msg = "AsyncContextResource must be async generator function"
             raise RuntimeError(msg)
```

### Comparing `that_depends-1.6.0/that_depends/providers/factories.py` & `that_depends-1.6.1/that_depends/providers/factories.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.0/that_depends/providers/resources.py` & `that_depends-1.6.1/that_depends/providers/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 T = typing.TypeVar("T")
 P = typing.ParamSpec("P")
 
 
 class Resource(AbstractResource[T]):
     def __init__(
         self,
-        creator: typing.Callable[[], typing.Iterator[T]],
+        creator: typing.Callable[..., typing.Iterator[T]],
         *args: typing.Any,  # noqa: ANN401
         **kwargs: typing.Any,  # noqa: ANN401
     ) -> None:
         if not inspect.isgeneratorfunction(creator):
             msg = "Resource must be generator function"
             raise RuntimeError(msg)
 
@@ -46,15 +46,15 @@
             )
         return self._instance
 
 
 class AsyncResource(AbstractResource[T]):
     def __init__(
         self,
-        creator: typing.Callable[[], typing.AsyncIterator[T]],
+        creator: typing.Callable[..., typing.AsyncIterator[T]],
         *args: typing.Any,  # noqa: ANN401
         **kwargs: typing.Any,  # noqa: ANN401
     ) -> None:
         if not inspect.isasyncgenfunction(creator):
             msg = "AsyncResource must be async generator function"
             raise RuntimeError(msg)
```

### Comparing `that_depends-1.6.0/that_depends/providers/singleton.py` & `that_depends-1.6.1/that_depends/providers/singleton.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.0/PKG-INFO` & `that_depends-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: that-depends
-Version: 1.6.0
+Version: 1.6.1
 Summary: Simple Dependency Injection framework
 Home-page: https://github.com/modern-python/that-depends
 Author: Artur Shiriev
 Author-email: me@shiriev.ru
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```


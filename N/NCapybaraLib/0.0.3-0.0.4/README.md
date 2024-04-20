# Comparing `tmp/ncapybaralib-0.0.3.tar.gz` & `tmp/ncapybaralib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncapybaralib-0.0.3.tar", last modified: Fri Apr 19 19:00:15 2024, max compression
+gzip compressed data, was "ncapybaralib-0.0.4.tar", last modified: Sat Apr 20 22:20:34 2024, max compression
```

## Comparing `ncapybaralib-0.0.3.tar` & `ncapybaralib-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 19:00:15.202625 ncapybaralib-0.0.3/
--rw-rw-rw-   0        0        0      963 2024-04-19 19:00:15.199615 ncapybaralib-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-04-19 18:15:16.000000 ncapybaralib-0.0.3/README.md
--rw-rw-rw-   0        0        0      667 2024-04-19 18:58:36.000000 ncapybaralib-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-19 19:00:15.203620 ncapybaralib-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-19 19:00:15.176620 ncapybaralib-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-19 19:00:15.182651 ncapybaralib-0.0.3/src/NCapybaraLib/
--rw-rw-rw-   0        0        0      147 2024-04-19 18:50:49.000000 ncapybaralib-0.0.3/src/NCapybaraLib/String.py
--rw-rw-rw-   0        0        0      204 2024-04-19 18:51:04.000000 ncapybaralib-0.0.3/src/NCapybaraLib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 19:00:15.196618 ncapybaralib-0.0.3/src/NCapybaraLib/_internal/
--rw-rw-rw-   0        0        0      616 2024-04-19 16:30:29.000000 ncapybaralib-0.0.3/src/NCapybaraLib/_internal/String.py
--rw-rw-rw-   0        0        0     1038 2024-04-19 18:35:34.000000 ncapybaralib-0.0.3/src/NCapybaraLib/_internal/init.py
-drwxrwxrwx   0        0        0        0 2024-04-19 19:00:15.198616 ncapybaralib-0.0.3/src/NCapybaraLib.egg-info/
--rw-rw-rw-   0        0        0      963 2024-04-19 19:00:15.000000 ncapybaralib-0.0.3/src/NCapybaraLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-04-19 19:00:15.000000 ncapybaralib-0.0.3/src/NCapybaraLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 19:00:15.000000 ncapybaralib-0.0.3/src/NCapybaraLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-19 19:00:15.000000 ncapybaralib-0.0.3/src/NCapybaraLib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 22:20:34.279440 ncapybaralib-0.0.4/
+-rw-rw-rw-   0        0        0      963 2024-04-20 22:20:34.277442 ncapybaralib-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-04-19 18:15:16.000000 ncapybaralib-0.0.4/README.md
+-rw-rw-rw-   0        0        0      667 2024-04-20 21:21:04.000000 ncapybaralib-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-20 22:20:34.280442 ncapybaralib-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 22:20:34.210442 ncapybaralib-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-20 22:20:34.218444 ncapybaralib-0.0.4/src/NCapybaraLib/
+-rw-rw-rw-   0        0        0      181 2024-04-20 21:50:58.000000 ncapybaralib-0.0.4/src/NCapybaraLib/String.py
+-rw-rw-rw-   0        0        0      219 2024-04-20 21:51:06.000000 ncapybaralib-0.0.4/src/NCapybaraLib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 22:20:34.273438 ncapybaralib-0.0.4/src/NCapybaraLib/_internal/
+-rw-rw-rw-   0        0        0     2825 2024-04-20 22:16:55.000000 ncapybaralib-0.0.4/src/NCapybaraLib/_internal/String.py
+-rw-rw-rw-   0        0        0     1121 2024-04-20 21:51:03.000000 ncapybaralib-0.0.4/src/NCapybaraLib/_internal/init.py
+drwxrwxrwx   0        0        0        0 2024-04-20 22:20:34.276440 ncapybaralib-0.0.4/src/NCapybaraLib.egg-info/
+-rw-rw-rw-   0        0        0      963 2024-04-20 22:20:34.000000 ncapybaralib-0.0.4/src/NCapybaraLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-04-20 22:20:34.000000 ncapybaralib-0.0.4/src/NCapybaraLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 22:20:34.000000 ncapybaralib-0.0.4/src/NCapybaraLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-20 22:20:34.000000 ncapybaralib-0.0.4/src/NCapybaraLib.egg-info/top_level.txt
```

### Comparing `ncapybaralib-0.0.3/PKG-INFO` & `ncapybaralib-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NCapybaraLib
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small library with a bunch of functions and thingies I made for fun.
 Author: NorbCodes
 Project-URL: Github Repo, https://github.com/norbcodes/NCapybaraLib
 Project-URL: Bug Tracker, https://github.com/norbcodes/NCapybaraLib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NCapybaraLib Version: 0.0.3 Summary: A small
+Metadata-Version: 2.1 Name: NCapybaraLib Version: 0.0.4 Summary: A small
 library with a bunch of functions and thingies I made for fun. Author:
 NorbCodes Project-URL: Github Repo, https://github.com/norbcodes/NCapybaraLib
 Project-URL: Bug Tracker, https://github.com/norbcodes/NCapybaraLib/issues
 Classifier: Programming Language :: Python :: 3 Classifier: Natural Language ::
 English Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `ncapybaralib-0.0.3/pyproject.toml` & `ncapybaralib-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=69"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NCapybaraLib"
 description = "A small library with a bunch of functions and thingies I made for fun."
 authors = [{name="NorbCodes"}]
-version = "0.0.3"
+version = "0.0.4"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Natural Language :: English",
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "Programming Language :: Python :: 3.12"
```

### Comparing `ncapybaralib-0.0.3/src/NCapybaraLib/_internal/init.py` & `ncapybaralib-0.0.4/src/NCapybaraLib/_internal/init.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-NCapybaraLib
+NCapybaraLib; By NorbCodes.
 
 A small library with a bunch of functions and thingies I made for fun.
 
 https://pypi.org/project/NCapybaraLib/
 """
 
 from typing import Any, Callable
@@ -17,15 +17,15 @@
 def inject_function(obj: Any, func_name: str, func: Callable[[Any], Any]) -> Any:
     """
     Does exactly what it sounds like. Injects *func* as a method for *obj* under the name *func_name*.
 
     :param obj: The object instance name referring to the object to inject into.
     :param func_name: The method name.
     :param func: The function to inject.
-    :return:
+    :return: The *obj* that was passed in, now with the function injected in it.
     """
     scope = {"target": obj, "injection": func}
     try:
         exec(f"target.{func_name}=classmethod(injection).__get__(None, target)", scope)
     except AttributeError as A:
         raise AttributeError(f"Cannot inject function {func.__name__} as {func_name} into object of type {type(obj)}.") from A
     return scope["target"]
```

### Comparing `ncapybaralib-0.0.3/src/NCapybaraLib.egg-info/PKG-INFO` & `ncapybaralib-0.0.4/src/NCapybaraLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NCapybaraLib
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small library with a bunch of functions and thingies I made for fun.
 Author: NorbCodes
 Project-URL: Github Repo, https://github.com/norbcodes/NCapybaraLib
 Project-URL: Bug Tracker, https://github.com/norbcodes/NCapybaraLib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NCapybaraLib Version: 0.0.3 Summary: A small
+Metadata-Version: 2.1 Name: NCapybaraLib Version: 0.0.4 Summary: A small
 library with a bunch of functions and thingies I made for fun. Author:
 NorbCodes Project-URL: Github Repo, https://github.com/norbcodes/NCapybaraLib
 Project-URL: Bug Tracker, https://github.com/norbcodes/NCapybaraLib/issues
 Classifier: Programming Language :: Python :: 3 Classifier: Natural Language ::
 English Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```


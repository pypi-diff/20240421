# Comparing `tmp/arclet_alconna_tools-0.7.2.tar.gz` & `tmp/arclet_alconna_tools-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet_alconna_tools-0.7.2.tar", last modified: Fri Apr  5 06:52:39 2024, max compression
+gzip compressed data, was "arclet_alconna_tools-0.7.3.tar", last modified: Sun Apr 21 15:03:44 2024, max compression
```

## Comparing `arclet_alconna_tools-0.7.2.tar` & `arclet_alconna_tools-0.7.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1091 2024-02-28 05:17:30.447506 arclet_alconna_tools-0.7.2/LICENSE
--rw-r--r--   0        0        0      749 2024-02-28 05:17:30.447506 arclet_alconna_tools-0.7.2/README.md
--rw-r--r--   0        0        0     1032 2024-04-05 06:52:39.249832 arclet_alconna_tools-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      991 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/__init__.py
--rw-r--r--   0        0        0     2355 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/actions.py
--rw-r--r--   0        0        0      866 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/checker.py
--rw-r--r--   0        0        0       96 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/config.py
--rw-r--r--   0        0        0    35652 2024-03-15 14:38:48.571519 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/construct.py
--rw-r--r--   0        0        0     4703 2024-04-05 06:49:19.105061 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/debug.py
--rw-r--r--   0        0        0    16954 2024-03-15 13:45:46.463804 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/formatter.py
--rw-r--r--   0        0        0       26 2024-02-28 05:17:30.449506 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/i18n/.config.json
--rw-r--r--   0        0        0      822 2024-02-28 05:17:30.449506 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/i18n/en-US.json
--rw-r--r--   0        0        0      783 2024-02-28 05:17:30.449506 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/i18n/zh-CN.json
--rw-r--r--   0        0        0     4394 2024-02-28 05:33:46.955180 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/pattern.py
--rw-r--r--   0        0        0     1014 1970-01-01 00:00:00.000000 arclet_alconna_tools-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-02-28 05:17:30.447506 arclet_alconna_tools-0.7.3/LICENSE
+-rw-r--r--   0        0        0      749 2024-02-28 05:17:30.447506 arclet_alconna_tools-0.7.3/README.md
+-rw-r--r--   0        0        0     1033 2024-04-21 15:03:44.041103 arclet_alconna_tools-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      991 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/__init__.py
+-rw-r--r--   0        0        0     2355 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/actions.py
+-rw-r--r--   0        0        0      866 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/checker.py
+-rw-r--r--   0        0        0       96 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/config.py
+-rw-r--r--   0        0        0    35652 2024-03-15 14:38:48.571519 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/construct.py
+-rw-r--r--   0        0        0     4703 2024-04-05 06:49:19.105061 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/debug.py
+-rw-r--r--   0        0        0    16954 2024-03-15 13:45:46.463804 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/formatter.py
+-rw-r--r--   0        0        0       26 2024-02-28 05:17:30.449506 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/i18n/.config.json
+-rw-r--r--   0        0        0      822 2024-02-28 05:17:30.449506 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/i18n/en-US.json
+-rw-r--r--   0        0        0      783 2024-02-28 05:17:30.449506 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/i18n/zh-CN.json
+-rw-r--r--   0        0        0     4405 2024-04-21 15:02:08.020498 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/pattern.py
+-rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 arclet_alconna_tools-0.7.3/PKG-INFO
```

### Comparing `arclet_alconna_tools-0.7.2/LICENSE` & `arclet_alconna_tools-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.2/README.md` & `arclet_alconna_tools-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.2/pyproject.toml` & `arclet_alconna_tools-0.7.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "arclet-alconna-tools"
-version = "0.7.2"
+version = "0.7.3"
 description = "Builtin Tools for Alconna"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
-    "nepattern<1.0.0,>=0.6.5",
-    "arclet-alconna>=1.8.7",
+    "nepattern<1.0.0,>=0.7.0",
+    "arclet-alconna>=1.8.10",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/__init__.py` & `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/actions.py` & `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/actions.py`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/checker.py` & `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/checker.py`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/construct.py` & `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/construct.py`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/debug.py` & `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/debug.py`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/formatter.py` & `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/formatter.py`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/i18n/en-US.json` & `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/i18n/en-US.json`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/i18n/zh-CN.json` & `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/i18n/zh-CN.json`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/pattern.py` & `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/pattern.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from nepattern.context import global_patterns
 from tarina import lang
 from .debug import analyse_args
 
 TOrigin = TypeVar("TOrigin")
 
 
-class ObjectPattern(BasePattern[TOrigin, Any]):
+class ObjectPattern(BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(
         self,
         origin: Type[TOrigin],
         limit: Tuple[str, ...] = (),
         flag: Literal["urlget", "part", "json", "space"] = "part",
         **suppliers: Callable,
     ):
@@ -50,18 +50,17 @@
             if name in suppliers and inspect.isclass(anno):
                 _s_sig = inspect.signature(suppliers[name])
                 if len(_s_sig.parameters) == 1 or (
                     len(_s_sig.parameters) == 2 and inspect.ismethod(suppliers[name])
                 ):
                     anno = BasePattern(
                         mode=MatchMode.TYPE_CONVERT,
-                        origin=Any,
+                        origin=Any,  # type: ignore
                         converter=lambda _, x: suppliers[name](x),
                         alias=anno.__name__,
-                        accepts=Any,
                     )
                 elif len(_s_sig.parameters) == 0 or (
                     len(_s_sig.parameters) == 1 and inspect.ismethod(suppliers[name])
                 ):
                     default = suppliers[name]()
                 else:
                     raise TypeError(lang.require("tools", "pattern.supplier_params_error"))
```

### Comparing `arclet_alconna_tools-0.7.2/PKG-INFO` & `arclet_alconna_tools-0.7.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-tools
-Version: 0.7.2
+Version: 0.7.3
 Summary: Builtin Tools for Alconna
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
-Requires-Dist: nepattern<1.0.0,>=0.6.5
-Requires-Dist: arclet-alconna>=1.8.7
+Requires-Dist: nepattern<1.0.0,>=0.7.0
+Requires-Dist: arclet-alconna>=1.8.10
 Description-Content-Type: text/markdown
 
 # Alconna Tools
 
 Provider various tools for Alconna
 
 Extensions:
```


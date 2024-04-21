# Comparing `tmp/zenyx-2.1.0.tar.gz` & `tmp/zenyx-2.2.0.tar.gz`

## Comparing `zenyx-2.1.0.tar` & `zenyx-2.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 zenyx-2.1.0/.editorconfig
--rw-r--r--   0        0        0    80912 2020-02-02 00:00:00.000000 zenyx-2.1.0/pyon.debug.md
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 zenyx-2.1.0/src/zenyx/__init__.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 zenyx-2.1.0/src/zenyx/args.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 zenyx-2.1.0/src/zenyx/console.py
--rw-r--r--   0        0        0    15128 2020-02-02 00:00:00.000000 zenyx-2.1.0/src/zenyx/pyon.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 zenyx-2.1.0/src/zenyx/require.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 zenyx-2.1.0/src/zenyx/streams.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 zenyx-2.1.0/tests/databank.py
--rw-r--r--   0        0        0   144790 2020-02-02 00:00:00.000000 zenyx-2.1.0/tests/pyon.debug.md
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 zenyx-2.1.0/tests/test_main.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zenyx-2.1.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 zenyx-2.1.0/LICENSE
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 zenyx-2.1.0/README.md
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 zenyx-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 zenyx-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 zenyx-2.2.0/.editorconfig
+-rw-r--r--   0        0        0   294292 2020-02-02 00:00:00.000000 zenyx-2.2.0/pyon.debug.md
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 zenyx-2.2.0/src/zenyx/__init__.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 zenyx-2.2.0/src/zenyx/args.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 zenyx-2.2.0/src/zenyx/console.py
+-rw-r--r--   0        0        0    15177 2020-02-02 00:00:00.000000 zenyx-2.2.0/src/zenyx/pyon.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 zenyx-2.2.0/src/zenyx/require.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 zenyx-2.2.0/src/zenyx/streams.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 zenyx-2.2.0/tests/databank.py
+-rw-r--r--   0        0        0   144790 2020-02-02 00:00:00.000000 zenyx-2.2.0/tests/pyon.debug.md
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 zenyx-2.2.0/tests/test_main.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zenyx-2.2.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 zenyx-2.2.0/LICENSE
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 zenyx-2.2.0/README.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 zenyx-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 zenyx-2.2.0/PKG-INFO
```

### Comparing `zenyx-2.1.0/src/zenyx/__init__.py` & `zenyx-2.2.0/src/zenyx/__init__.py`

 * *Files identical despite different names*

### Comparing `zenyx-2.1.0/src/zenyx/args.py` & `zenyx-2.2.0/src/zenyx/args.py`

 * *Files identical despite different names*

### Comparing `zenyx-2.1.0/src/zenyx/console.py` & `zenyx-2.2.0/src/zenyx/console.py`

 * *Files identical despite different names*

### Comparing `zenyx-2.1.0/src/zenyx/pyon.py` & `zenyx-2.2.0/src/zenyx/pyon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 import datetime
 import json
 import copy
 from collections import namedtuple
+from recordclass import recordclass 
 from dataclasses import dataclass
 import re
 import os
 
 def is_type(value: any, _type):
     debug.log(f"  **`[TypeCheck]`** Checking Type \n\tValue: `{value}`, \n\tType(s): `{_type}`")
     if type(value) is _type:
@@ -332,15 +333,15 @@
     def __end(text: any):
         debug.log(f"  **`[{xdent}]`** Return Value: \n\t`{text}`")
         debug.log(debug.separator_text(title="End", xdent=xdent, callbackorigin=callbacktime))
         debug.indent = 1
     
     if class_type != "&DICT":
         params["pyon_converted"] = True
-        new_object_initializer = namedtuple(class_type, list(params.keys()))
+        new_object_initializer = recordclass(class_type, ' '.join(list(params.keys())))
         new_object = new_object_initializer(*list(params.values()))
         
         __end(new_object)
         return new_object
     __end(olddict)
```

### Comparing `zenyx-2.1.0/src/zenyx/require.py` & `zenyx-2.2.0/src/zenyx/require.py`

 * *Files identical despite different names*

### Comparing `zenyx-2.1.0/src/zenyx/streams.py` & `zenyx-2.2.0/src/zenyx/streams.py`

 * *Files identical despite different names*

### Comparing `zenyx-2.1.0/tests/pyon.debug.md` & `zenyx-2.2.0/tests/pyon.debug.md`

 * *Files identical despite different names*

### Comparing `zenyx-2.1.0/LICENSE` & `zenyx-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zenyx-2.1.0/pyproject.toml` & `zenyx-2.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zenyx"
-version = "2.1.0"
+version = "2.2.0"
 authors = [
   { name="zewenn", email="zc.fallens@gamil.com" },
 ]
 description = "A multitool python object notation package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `zenyx-2.1.0/PKG-INFO` & `zenyx-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: zenyx
-Version: 2.1.0
+Version: 2.2.0
 Summary: A multitool python object notation package
 Project-URL: Homepage, https://github.com/zewenn/zenyx
 Project-URL: Issues, https://github.com/zewenn/zenyx/issues
 Author-email: zewenn <zc.fallens@gamil.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


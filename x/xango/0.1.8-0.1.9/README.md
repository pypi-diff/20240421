# Comparing `tmp/xango-0.1.8.tar.gz` & `tmp/xango-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xango-0.1.8.tar", last modified: Thu Nov  2 05:22:45 2023, max compression
+gzip compressed data, was "xango-0.1.9.tar", last modified: Fri Nov  3 07:56:53 2023, max compression
```

## Comparing `xango-0.1.8.tar` & `xango-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-11-02 05:22:45.328929 xango-0.1.8/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 xango-0.1.8/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       25 2023-10-24 06:55:36.000000 xango-0.1.8/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1445 2023-11-02 05:22:45.328854 xango-0.1.8/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      934 2023-10-24 06:53:13.000000 xango-0.1.8/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-11-02 05:22:45.329166 xango-0.1.8/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      795 2023-11-02 05:22:25.000000 xango-0.1.8/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-11-02 05:22:45.322926 xango-0.1.8/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-11-02 05:22:45.326743 xango-0.1.8/src/xango/
--rw-r--r--   0 mardix     (501) staff       (20)      516 2023-10-27 04:00:21.000000 xango-0.1.8/src/xango/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    65270 2023-11-02 05:21:08.000000 xango-0.1.8/src/xango/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    15150 2023-11-02 05:21:08.000000 xango-0.1.8/src/xango/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18846 2023-11-02 05:21:08.000000 xango-0.1.8/src/xango/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)      565 2023-11-02 05:21:08.000000 xango-0.1.8/src/xango/exceptions.py
--rw-r--r--   0 mardix     (501) staff       (20)    20378 2023-11-02 05:21:08.000000 xango-0.1.8/src/xango/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    12699 2023-11-02 05:21:08.000000 xango-0.1.8/src/xango/lib_dict.py
--rw-r--r--   0 mardix     (501) staff       (20)    20076 2023-11-02 05:21:08.000000 xango-0.1.8/src/xango/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-11-02 05:22:45.327480 xango-0.1.8/src/xango.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1445 2023-11-02 05:22:45.000000 xango-0.1.8/src/xango.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      499 2023-11-02 05:22:45.000000 xango-0.1.8/src/xango.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-11-02 05:22:45.000000 xango-0.1.8/src/xango.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       60 2023-11-02 05:22:45.000000 xango-0.1.8/src/xango.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        6 2023-11-02 05:22:45.000000 xango-0.1.8/src/xango.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-11-02 05:22:45.328582 xango-0.1.8/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 xango-0.1.8/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      712 2023-10-24 06:55:36.000000 xango-0.1.8/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     2842 2023-10-24 06:55:36.000000 xango-0.1.8/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     4809 2023-10-24 06:55:36.000000 xango-0.1.8/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 xango-0.1.8/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-11-03 07:56:53.260483 xango-0.1.9/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 xango-0.1.9/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       25 2023-10-24 06:55:36.000000 xango-0.1.9/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1445 2023-11-03 07:56:53.260388 xango-0.1.9/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      934 2023-10-24 06:53:13.000000 xango-0.1.9/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-11-03 07:56:53.260767 xango-0.1.9/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      795 2023-11-03 07:56:28.000000 xango-0.1.9/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-11-03 07:56:53.251140 xango-0.1.9/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-11-03 07:56:53.257359 xango-0.1.9/src/xango/
+-rw-r--r--   0 mardix     (501) staff       (20)      516 2023-10-27 04:00:21.000000 xango-0.1.9/src/xango/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    65270 2023-11-02 05:21:08.000000 xango-0.1.9/src/xango/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    13813 2023-11-03 07:55:34.000000 xango-0.1.9/src/xango/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18846 2023-11-02 05:21:08.000000 xango-0.1.9/src/xango/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)      565 2023-11-02 05:21:08.000000 xango-0.1.9/src/xango/exceptions.py
+-rw-r--r--   0 mardix     (501) staff       (20)    20378 2023-11-02 05:21:08.000000 xango-0.1.9/src/xango/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    12116 2023-11-03 07:52:25.000000 xango-0.1.9/src/xango/lib_dict.py
+-rw-r--r--   0 mardix     (501) staff       (20)    20076 2023-11-02 05:21:08.000000 xango-0.1.9/src/xango/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-11-03 07:56:53.258453 xango-0.1.9/src/xango.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1445 2023-11-03 07:56:53.000000 xango-0.1.9/src/xango.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      499 2023-11-03 07:56:53.000000 xango-0.1.9/src/xango.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-11-03 07:56:53.000000 xango-0.1.9/src/xango.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       60 2023-11-03 07:56:53.000000 xango-0.1.9/src/xango.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        6 2023-11-03 07:56:53.000000 xango-0.1.9/src/xango.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-11-03 07:56:53.260085 xango-0.1.9/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 xango-0.1.9/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      712 2023-10-24 06:55:36.000000 xango-0.1.9/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     2842 2023-10-24 06:55:36.000000 xango-0.1.9/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     4809 2023-10-24 06:55:36.000000 xango-0.1.9/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 xango-0.1.9/tests/test_query.py
```

### Comparing `xango-0.1.8/LICENSE` & `xango-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xango-0.1.8/PKG-INFO` & `xango-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xango
-Version: 0.1.8
+Version: 0.1.9
 Summary: xango 
 Home-page: https://github.com/mardix/xango
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `xango-0.1.8/README.md` & `xango-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `xango-0.1.8/setup.py` & `xango-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 setuptools.setup(
     name='xango',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='xango ',
     long_description=long_description(),
```

### Comparing `xango-0.1.8/src/xango/__init__.py` & `xango-0.1.9/src/xango/__init__.py`

 * *Files identical despite different names*

### Comparing `xango-0.1.8/src/xango/database.py` & `xango-0.1.9/src/xango/database.py`

 * *Files identical despite different names*

### Comparing `xango-0.1.8/src/xango/dict_mutator.py` & `xango-0.1.9/src/xango/dict_mutator.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,79 +7,58 @@
 import arrow
 import uuid
 from . import lib, lib_dict, exceptions
 from functools import reduce
 # ----
 
 # Operators that work with list
-LISTTYPES_OPERATORS = ["xadd", "xadd_many", "xrem", "xrem_many", "xpush", "xpush_many", "xpushl", "xpushl_many"]
+LISTTYPES_OPERATORS = ["xadd", "xadd_many", "xrem", "xrem_many", "xpush", "xpush_many", "xpushl", "xpushl_many", "xpop", "xpopl", "xset"]
 
-# _NMutDict: A dict thats aggregates data to be mutated in a nested context
-class _NMutDict(dict): pass
-
-# _NMutList: A list of data to be mutatated in a nested context
-class _NMutList(list): pass
 
 # _FlattenDictType - Data Type flatten_dict
 class _FlattenDictType(dict): pass
 
 # To unset a value from being updated
 class _UnOperableValue(object): pass
 
-# MUTS3 {'d1.location:$set': 'zoomba'} 
+# ListMut is object a list mutations
+class ListMut(dict):
+    def add(self, key, value):
+        self[key] = value
+
+    def unflatten(self):
+        return lib_dict.unflatten(dict(self))
+
 def mutate(mutations: dict, init_data: dict = {}, immuts:list=[], custom_ops:dict={}):
     """
     mutate
 
     Args:
         mutations:dict - data contains operators to update
         init_data:dict - initial data 
         immuts: list - list of keys to not mutate
         custom_ops: dict - dict of custom operations
 
     Returns:
         tuple(updated_data:dict, oplog)
 
     """
-    
-    _muts = _flatten_dict(lib.deepcopy(mutations))
-    _inits = _flatten_dict(lib.deepcopy(init_data))
-    muts = {}
-
-    _restructed = {}
-    for k, v in _muts.items():
-        # since data is flat, let's restructure some data so they can be properly mutated
-        xl = list(filter(lambda v: v, re.split("(\:\$\w+)(?:\.)?", k)))
-        if len(xl) > 2:
-            _op = xl[1].replace(":$", "")
-            if _op in LISTTYPES_OPERATORS:
-                _pathkey = "%s:$%s" % (xl[0], _op)
-                if _pathkey not in _restructed:
-                    _restructed[_pathkey] = _NMutDict()
-                _jpath = ".".join(xl[2:]).replace(".:$", ":$")
-                _restructed[_pathkey][_jpath] = v
-            else:
-                muts[k] = _NMutList([_NMutDict(vv) if isinstance(vv, dict) else vv for vv in v]) if isinstance(v, list) else v
-        else:
-            # by default, data will be a :$set. This will allow inner update
-            k = "%s:$set" % k if ":$" not in k else k
-            muts[k] = _NMutList([_NMutDict(vv) if isinstance(vv, dict) else vv for vv in v]) if isinstance(v, list) else v
 
-    muts.update(_restructed)
-    d, _ = _mutate(mutations=muts, init_data=_inits, immuts=immuts, custom_ops=custom_ops)
+    init_data = lib.deepcopy(init_data)
+    flatten_data = lib_dict.flatten(lib.deepcopy(mutations))
+    d, _ = _mutate(flatten_data=flatten_data, init_data=init_data, immuts=immuts, custom_ops=custom_ops)
 
-    return _unflatten_dict(d), _
+    return lib_dict.unflatten(d), _
 
-
-def _mutate(mutations:_FlattenDictType, init_data:_FlattenDictType={}, immuts:list=[], custom_ops:dict={}):
+def _mutate(flatten_data:_FlattenDictType, init_data:_FlattenDictType={}, immuts:list=[], custom_ops:dict={}):
     """
     Mutation operations
 
     Args:
-        mutations:dict - data contains operators to update
+        flatten_data:dict - data contains operators to update
         init_data:dict - initial data 
         immuts: list - list of keys to not mutate
         custom_ops: dict - dict of custom operations
 
     Returns:
         tuple(updated_data:_FlattenDictType, oplog)
 
@@ -89,48 +68,53 @@
         $decr - to decrease an INT value
         $unset - To remove a property
         $rename - To rename a property
         $copy - To copy the value of property to another one
         $datetime - gen the current datetime. Can manipulate time
         $template - Evalute the string as template
         $uuid4 - gen a UUID4 string, with the dashes
+
+
         $xadd - add item if doesn't exist
         $xadd_many - add many items in the list if not already in the list
         $xrem - remove item
         $xrem_many - remove many items in a list
         $xpush - push item on the right
         $xpush_many - push many items in a list on the right
         $xpushl - push item on the left
         $xpushl_many - push many items in a list on the left
         $xpop - pop an item from a list on the right 
         $xpopl - pop an item from a list on the left
         $xlen - calculate the length of an object
         
+
+        
     Example
         {
            "key:$incr": True|1|Num,
            "key:$decr": True|1|Num,
            "some.key:$unset": True,
            "old.key:$rename: "@new_path",
            "some.key:$copy: "@new_path",
+           "some.datetimefield:$datetime": True,             
+           "some.datetimefield:$datetime": "+1Day +2Hours 5Minutes",
+           "some.key:$template": "Hello {{ name }}!",
+           "some.random.id:$uuid4": True,
+
            "some.list:$xadd": Any,
            "some.list:$xadd_many": [Any, Any, Any, ...],
            "some.list:$xrem": Any,
            "some.list:$xrem_many": [Any, Any, Any, ...],     
            "some.list:$xpush": Any,
            "some.list:$xpush_many": [Any, Any, Any, ...],   
            "some.list:$xpushl": Any,
            "some.list:$xpushl_many": [Any, Any, Any, ...],    
            "some.list:$xpop": True,
            "some.list:$xpopl: False,
            "some.value:$xlen": "@some.data.path",
-           "some.datetimefield:$datetime": True,             
-           "some.datetimefield:$datetime": "+1Day +2Hours 5Minutes",
-           "some.key:$template": "Hello {{ name }}!",
-           "some.random.id:$uuid4": True,
         }
 
     Custom operations
         Extends the dict mutator with custom operations 
 
         It's K/V pair with key being the name of the operation and value a callable with
             def name(data, path, value)
@@ -147,53 +131,66 @@
             ops = {
                 "new_uid:$new_uuid4": True
             }    
     """
     data = init_data
     oplog = {}
     postproc = {}
-    replace_set = {}
+    listops = {}
 
     # disabled immuts
     immuts = []
     
-    for path, value in mutations.items():
+    # flat operation
+    for path, value in flatten_data.items():
 
         # -- skip
         if immuts and path in immuts:
             continue 
 
-        if ":" in path:
-            # -- skip
-            if ":$" not in path:
-                continue
-            
-            if isinstance(value, dict):
-                value = _mutate(value)[0]
-
-            if isinstance(value, list):
-                value = [ _mutate(vv)[0] if isinstance(vv, dict) else vv for vv in value]
-
+        if ":$" in path:
             oppath = path
             oplog_path = path
             path, op = path.split(":$")
 
-            
             # -- skip
             if immuts and path in immuts:
                 continue 
+
+            # listops, list
+            if "." in op:
+                opl, rest_ = op.split(".", 1)
+                new_path = ".".join([path, rest_])
+                oppp = "%s:$%s" % (path, opl)
+                if opl in LISTTYPES_OPERATORS:
+                    if oppp not in listops:
+                        listops[oppp] = ListMut()
+                    listops[oppp].add(rest_, value)
+                continue
+
             
+            if op in LISTTYPES_OPERATORS:
+                listops[oppath] = value
+                continue
+
             # post-process data. To be parsed later
             if op in ["template", "xlen", "rename", "copy"]:
                 postproc[oppath] = value 
                 continue 
 
             # $set. literal assigment, leave as is 
-            if op == "set":
-                pass
+            elif op == "set":
+
+                # potential list
+                if "." in path and path[-1].isdigit():
+                    index_ = int(path[-1])
+                    s_l = path.split(".")
+                    kp_ = ".".join(s_l[:-1])
+                    lib_dict.dict_get(data, kp_)[index_] = value
+                    continue
 
             # $incr
             elif op == "incr":
                 value = _get_int_data(data, path) + \
                     (value if isinstance(value, int) else 1)
                 oplog[oplog_path] = value
 
@@ -226,25 +223,43 @@
                         value = _UnOperableValue()
 
             # $uuid4
             elif op == "uuid4":
                 value = str(uuid.uuid4()) #.replace("-", "")
 
 
-            # LIST operators
+            # $$custom_ops, add to post process
+            elif op in custom_ops:
+                postproc[oppath] = value 
+                continue 
 
-            elif op in (
-                "xadd", "xadd_many",
-                "xrem", "xrem_many",
-                "xpush", "xpush_many",
-                "xpushl", "xpushl_many"
-            ):
+            # _UnOperableValue
+            else:
+                value = _UnOperableValue()
+
+
+        if not isinstance(value, _UnOperableValue):
+            data[path] = value
+
+    # listops
+    # List operations work on list items to add, remove etc
+    if listops:
+        ldata = {}
+        for path, value in listops.items():
+            if isinstance(value, ListMut):
+                value = value.unflatten()
+
+            oppath = path
+            oplog_path = path
+            path, op = path.split(":$")
+
+            if op in ( "xadd", "xadd_many", "xrem", "xrem_many", "xpush", "xpush_many", "xpushl", "xpushl_many"):
                 values = _values_to_mlist(value, many=op.endswith("_many"))
                 v = _get_list_data(data, path)
-
+                
                 # $xadd|$xadd_many
                 if op.startswith("xadd"):
                     for val in values:
                         if val not in v:
                             v.append(val)
                     value = v
 
@@ -266,41 +281,45 @@
 
                 # $xpushl|$xpushl_many
                 elif op in ("xpushl", "xpushl_many"):
                     v2 = list(values)
                     v2.extend(v)
                     value = v2
 
+            elif op == "xset":
+                index_ = int(path[-1])
+                s_l = path.split(".")
+                kp_ = ".".join(s_l[:-1])
+                lib_dict.dict_get(data, kp_)[index_] = value
+                continue
+
             # $xpop
             elif op == "xpop":
                 v = _get_list_data(data, path)
                 if len(v):
                     value = v[:-1]
                     oplog[oplog_path] = v[-1]
 
             # $xpopl
             elif op == "xpopl":
                 v = _get_list_data(data, path)
                 if len(v):
                     value = v[1:]
                     oplog[oplog_path] = v[0]
 
-            # $$custom_ops, add to post process
-            elif op in custom_ops:
-                postproc[oppath] = value 
-                continue 
-
             # _UnOperableValue
             else:
                 value = _UnOperableValue()
 
-        if not isinstance(value, _UnOperableValue):
-            data[path] = value
+            if not isinstance(value, _UnOperableValue):
+                data[path] = value
+
 
     # Post process
+    # final process 
     if postproc:
         for path, value in postproc.items():            
             try:
                 if ":" in path:
                     # -- skip
                     if ":$" not in path:
                         continue
@@ -332,40 +351,40 @@
                     # $rename, requires @ref
                     elif op == "rename" and _is_value_at_ref(value):
                         value = _clean_value_ref(value)
                         data[value] = _pop(data, path)
 
                     # $copy, requires @ref
                     elif op == "copy" and _is_value_at_ref(value):
-                        data[path] = _get(data, _clean_value_ref(value))
+                        value = _clean_value_ref(value)
+                        data[value] = _get(data, path)
 
                     # custom ops
                     elif op in custom_ops:
                         data[path] = custom_ops[op](data, path, value)
 
             except:
                 pass
 
-
     return data, oplog
 
 
 _arrow_date_shifter = lib.arrow_date_shifter
 
 def _get(data:dict, path):
     """
     _get: Alias to get data from a path
     """
-    return lib.dict_get(obj=data, path=path)
+    return lib_dict.dict_get(obj=data, path=path)
 
 def _set(data:dict, path, value):
     """
     _set: Alias to set value in data
     """
-    lib.dict_set(data, path, value)
+    lib_dict.dict_set(data, path, value)
     return data
 
 def _pop(data, path):
     """
     _pop: Alias to remove object from data
     """
     if path in data:
@@ -387,15 +406,15 @@
     """
     _get_list_data: Returns a data LIST, for list types operations
     """
     v = _get(data, path)
     if v is None:
         return []
     if not isinstance(v, list):
-        raise TypeError("Invalid data type for '%s'. Must be 'list' " % path)
+        raise exceptions.MutationTypeError("Invalid data type for '%s'. Must be 'list' " % path)
     return v
 
 def _values_to_mlist(value, many=False) -> list:
     """
     _values_to_mlist: Convert data multiple list items
     """
     return [value] if many is False else value if isinstance(value, (list, tuple)) else [value]
@@ -416,67 +435,15 @@
 def _j2_currdate(format_="ISO_DATETIME", shifter=None):
     dt = _get_datetime()
     if shifter:
         dt = _arrow_date_shifter(dt=dt, stmt=shifter)
     return lib.arrow_date_format(dt, format_)
 
 def _lookup_flat_data(d_flatten, key):
-    return lib.dict_get(obj=_unflatten_dict(d_flatten), path=key)
+    return lib.dict_get(obj=lib_dict.unflatten(d_flatten), path=key)
 
 def _is_value_at_ref(value) -> bool:
     return value and isinstance(value, str) and value.startswith("@")
 
 def _clean_value_ref(value) -> str:
     return value.replace("@", "")
 
-def _flatten_dict(_dict: dict, _str: str = '', reducer=None) -> dict:
-    """
-    To flatten a dict. Nested node will be separated by dot or separator
-    It takes in consideration dict in list and flat them.
-    Non dict stay as is
-
-    Args:
-        ddict:
-        prefix:
-    Returns:
-        dict
-
-    """
-    sep = "."
-    ret_dict = {}
-    for k, v in _dict.items():
-        if isinstance(v, dict):
-            ret_dict.update(_flatten_dict(v, _str=sep.join([_str, k]).strip(sep)))
-        elif isinstance(v, list):
-            _k =  ("%s.%s" % (_str, k)).strip(sep)
-            ret_dict[_k] = [_flatten_dict(item) if isinstance(item, dict) else item for item in v]
-        else:
-            ret_dict[sep.join([_str, k]).strip(sep)] = v
-    return ret_dict
-
-def _unflatten_dict(flatten_dict: dict) -> dict:
-    """
-    To un-flatten a flatten dict
-
-    Args:
-      flatten_dict: A flatten dict
-    Returns:
-      an unflatten dictionnary
-    """
-
-    output = {}
-    for k, v in flatten_dict.items():
-        path = k.split(".")
-        if isinstance(v, list):
-            v = [_unflatten_dict(i2) if isinstance(i2, dict) else i2 for i2 in v]
-        _set_nested(output, path, v, k)
-    return output
-
-def _set_nested(d, path, value, full_path=None):
-    try:
-        _get_nested_default(d, path[:-1])[path[-1]] = value        
-    except (AttributeError, TypeError) as e:
-        raise exceptions.MutationTypeError("MutationTypeError: %s at '%s'" % (e, full_path))
-
-def _get_nested_default(d, path):
-    return reduce(lambda d, k: d.setdefault(k, {}), path, d)
-
```

### Comparing `xango-0.1.8/src/xango/dict_query.py` & `xango-0.1.9/src/xango/dict_query.py`

 * *Files identical despite different names*

### Comparing `xango-0.1.8/src/xango/exceptions.py` & `xango-0.1.9/src/xango/exceptions.py`

 * *Files identical despite different names*

### Comparing `xango-0.1.8/src/xango/lib.py` & `xango-0.1.9/src/xango/lib.py`

 * *Files identical despite different names*

### Comparing `xango-0.1.8/src/xango/lib_dict.py` & `xango-0.1.9/src/xango/lib_dict.py`

 * *Files 9% similar despite different names*

```diff
@@ -280,24 +280,14 @@
 
     for each_key in field_keys:
         field_value = field_dict[each_key]
         processed_key = str(each_key)
         current_key = None
         current_subkey = None
         for i in range(len(processed_key)):
-            if processed_key[i] == "[":
-                current_key = processed_key[:i]
-                start_subscript_index = i + 1
-                end_subscript_index = processed_key.index("]")
-                current_subkey = int(processed_key[start_subscript_index : end_subscript_index])
-
-                # reserve the remainder descendant keys to be processed later in a recursive call
-                if len(processed_key[end_subscript_index:]) > 1:
-                    current_subkey = "{}.{}".format(current_subkey, processed_key[end_subscript_index + 2:])
-                break
 
             # next child key is a dictionary
             if processed_key[i] == ".":
                 split_work = processed_key.split(".", 1)
                 if len(split_work) > 1:
                     current_key, current_subkey = split_work
                 else:
@@ -323,18 +313,19 @@
         # validate the keys can safely converted to a sequential list.
         all_digits &= str(each_key).isdigit()
         if all_digits:
             next_digit = int(each_key)
             if next_digit > highest_digit:
                 highest_digit = next_digit
 
+    
     # If all digits and can be sequential order, convert to list.
     if all_digits and highest_digit == (len(new_field_dict) - 1):
         digit_keys = list(new_field_dict)
-        digit_keys.sort()
+        #digit_keys.sort()
         new_list = []
 
         for k in digit_keys:
             i = int(k)
             if len(new_list) <= i:
                 # Pre-populate missing list elements if the array index keys are out of order
                 # and the current element is ahead of the current length boundary.
```

### Comparing `xango-0.1.8/src/xango/lib_xql.py` & `xango-0.1.9/src/xango/lib_xql.py`

 * *Files identical despite different names*

### Comparing `xango-0.1.8/src/xango.egg-info/PKG-INFO` & `xango-0.1.9/src/xango.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xango
-Version: 0.1.8
+Version: 0.1.9
 Summary: xango 
 Home-page: https://github.com/mardix/xango
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `xango-0.1.8/tests/test_database.py` & `xango-0.1.9/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `xango-0.1.8/tests/test_dict_mutator.py` & `xango-0.1.9/tests/test_dict_mutator.py`

 * *Files identical despite different names*

### Comparing `xango-0.1.8/tests/test_lib.py` & `xango-0.1.9/tests/test_lib.py`

 * *Files identical despite different names*


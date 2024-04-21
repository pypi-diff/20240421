# Comparing `tmp/mo-dots-9.584.24095.tar.gz` & `tmp/mo_dots-9.592.24112.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo-dots-9.584.24095.tar", last modified: Thu Apr  4 12:26:40 2024, max compression
+gzip compressed data, was "mo_dots-9.592.24112.tar", last modified: Sun Apr 21 14:32:02 2024, max compression
```

## Comparing `mo-dots-9.584.24095.tar` & `mo_dots-9.592.24112.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 12:26:40.693418 mo-dots-9.584.24095/
--rw-rw-rw-   0        0        0    16725 2022-02-13 20:11:16.000000 mo-dots-9.584.24095/LICENSE
--rw-rw-rw-   0        0        0     5055 2024-04-04 12:26:40.692339 mo-dots-9.584.24095/PKG-INFO
--rw-rw-rw-   0        0        0     3549 2024-04-04 03:46:45.000000 mo-dots-9.584.24095/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 12:26:40.680857 mo-dots-9.584.24095/mo_dots/
--rw-rw-rw-   0        0        0    13942 2024-03-21 02:15:09.000000 mo-dots-9.584.24095/mo_dots/__init__.py
--rw-rw-rw-   0        0        0    16231 2024-03-18 01:53:34.000000 mo-dots-9.584.24095/mo_dots/datas.py
--rw-rw-rw-   0        0        0     4284 2024-03-16 18:16:18.000000 mo-dots-9.584.24095/mo_dots/fields.py
--rw-rw-rw-   0        0        0    10290 2024-03-16 18:16:18.000000 mo-dots-9.584.24095/mo_dots/lists.py
--rw-rw-rw-   0        0        0     6568 2024-03-16 18:16:18.000000 mo-dots-9.584.24095/mo_dots/nones.py
--rw-rw-rw-   0        0        0     5298 2024-03-16 19:13:23.000000 mo-dots-9.584.24095/mo_dots/objects.py
--rw-rw-rw-   0        0        0     1424 2024-03-14 10:01:33.000000 mo-dots-9.584.24095/mo_dots/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-04 12:26:40.690250 mo-dots-9.584.24095/mo_dots.egg-info/
--rw-rw-rw-   0        0        0     5055 2024-04-04 12:26:40.000000 mo-dots-9.584.24095/mo_dots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-04-04 12:26:40.000000 mo-dots-9.584.24095/mo_dots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 12:26:40.000000 mo-dots-9.584.24095/mo_dots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-21 02:12:28.000000 mo-dots-9.584.24095/mo_dots.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      241 2024-04-04 12:26:40.000000 mo-dots-9.584.24095/mo_dots.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-04 12:26:40.000000 mo-dots-9.584.24095/mo_dots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 12:26:40.693418 mo-dots-9.584.24095/setup.cfg
--rw-rw-rw-   0        0        0     4937 2024-04-04 12:26:35.000000 mo-dots-9.584.24095/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:32:02.465541 mo_dots-9.592.24112/
+-rw-rw-rw-   0        0        0    16725 2022-02-13 20:11:16.000000 mo_dots-9.592.24112/LICENSE
+-rw-rw-rw-   0        0        0     5055 2024-04-21 14:32:02.464522 mo_dots-9.592.24112/PKG-INFO
+-rw-rw-rw-   0        0        0     3549 2024-04-04 03:46:45.000000 mo_dots-9.592.24112/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 14:32:02.452795 mo_dots-9.592.24112/mo_dots/
+-rw-rw-rw-   0        0        0    13989 2024-04-21 14:31:54.000000 mo_dots-9.592.24112/mo_dots/__init__.py
+-rw-rw-rw-   0        0        0    16165 2024-04-21 14:31:54.000000 mo_dots-9.592.24112/mo_dots/datas.py
+-rw-rw-rw-   0        0        0     4284 2024-03-16 18:16:18.000000 mo_dots-9.592.24112/mo_dots/fields.py
+-rw-rw-rw-   0        0        0    10399 2024-04-21 14:31:54.000000 mo_dots-9.592.24112/mo_dots/lists.py
+-rw-rw-rw-   0        0        0     6672 2024-04-21 14:31:54.000000 mo_dots-9.592.24112/mo_dots/nones.py
+-rw-rw-rw-   0        0        0     5524 2024-04-21 14:31:54.000000 mo_dots-9.592.24112/mo_dots/objects.py
+-rw-rw-rw-   0        0        0     1424 2024-03-14 10:01:33.000000 mo_dots-9.592.24112/mo_dots/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:32:02.462289 mo_dots-9.592.24112/mo_dots.egg-info/
+-rw-rw-rw-   0        0        0     5055 2024-04-21 14:32:02.000000 mo_dots-9.592.24112/mo_dots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-04-21 14:32:02.000000 mo_dots-9.592.24112/mo_dots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 14:32:02.000000 mo_dots-9.592.24112/mo_dots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-21 02:12:28.000000 mo_dots-9.592.24112/mo_dots.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      241 2024-04-21 14:32:02.000000 mo_dots-9.592.24112/mo_dots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-21 14:32:02.000000 mo_dots-9.592.24112/mo_dots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 14:32:02.465592 mo_dots-9.592.24112/setup.cfg
+-rw-rw-rw-   0        0        0     4937 2024-04-21 14:31:57.000000 mo_dots-9.592.24112/setup.py
```

### Comparing `mo-dots-9.584.24095/LICENSE` & `mo_dots-9.592.24112/LICENSE`

 * *Files identical despite different names*

### Comparing `mo-dots-9.584.24095/PKG-INFO` & `mo_dots-9.592.24112/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.584.24095
+Version: 9.592.24112
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo-dots-9.584.24095/README.md` & `mo_dots-9.592.24112/README.md`

 * *Files identical despite different names*

### Comparing `mo-dots-9.584.24095/mo_dots/__init__.py` & `mo_dots-9.592.24112/mo_dots/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,16 @@
     "literal_field",
     "missing",
     "Null",
     "NullType",
     "object_to_data",
     "PATH_NOT_FOUND",
     "relative_field",
+    "register_data",
+    "register_many",
     "set_attr",
     "set_default",
     "split_field",
     "startswith_field",
     "tail_field",
     "to_data",
     "tuplewrap",
@@ -122,15 +124,15 @@
 
     UPDATES d WITH THE MERGE RESULT, WHERE MERGE RESULT IS DEFINED AS:
     FOR EACH LEAF, RETURN THE FIRST NOT-NULL LEAF VALUE
 
     :param dicts: dicts IN PRIORITY ORDER, HIGHEST TO LOWEST
     :return: d
     """
-    agg = d if d or _get(d, CLASS) in datas.data_types else {}
+    agg = d if d or _get(d, CLASS) in datas._data_types else {}
     for p in dicts:
         _set_default(agg, p, seen={})
     return to_data(agg)
 
 
 def _set_default(d, default, seen=None):
     """
@@ -145,15 +147,15 @@
         if is_data(d):
             existing_value = d.get(k)
         else:
             existing_value = _get_attr(d, [k])
 
         if existing_value == None:
             if default_value != None:
-                if _get(default_value, CLASS) in datas.data_types:
+                if _get(default_value, CLASS) in datas._data_types:
                     df = seen.get(id(raw_value))
                     if df is not None:
                         _set_attr(d, [k], df)
                     else:
                         copy_dict = {}
                         seen[id(raw_value)] = copy_dict
                         _set_attr(d, [k], copy_dict)
@@ -164,17 +166,17 @@
                         _set_attr(d, [k], default_value)
                     except Exception as e:
                         if PATH_NOT_FOUND not in e:
                             get_logger().error("Can not set attribute {{name}}", name=k, cause=e)
         elif is_list(existing_value) or is_list(default_value):
             _set_attr(d, [k], None)
             _set_attr(d, [k], listwrap(existing_value) + listwrap(default_value))
-        elif (hasattr(existing_value, "__setattr__") or _get(existing_value, CLASS) in datas.data_types) and _get(
+        elif (hasattr(existing_value, "__setattr__") or _get(existing_value, CLASS) in datas._data_types) and _get(
             default_value, CLASS
-        ) in datas.data_types:
+        ) in datas._data_types:
             df = seen.get(id(raw_value))
             if df is not None:
                 _set_attr(d, [k], df)
             else:
                 seen[id(raw_value)] = existing_value
                 _set_default(existing_value, default_value, seen)
 
@@ -489,15 +491,15 @@
 
 
 def is_not_null(t):
     # RETURN True IF EFFECTIVELY SOMETHING
     class_ = t.__class__
     if class_ in null_types:
         return False
-    elif class_ in datas.data_types:
+    elif class_ in datas._data_types:
         return True
     elif class_ in finite_types and t:
         return True
     else:
         return t != None
```

### Comparing `mo-dots-9.584.24095/mo_dots/datas.py` & `mo_dots-9.592.24112/mo_dots/datas.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,26 +36,32 @@
     to_data,
     list_to_data,
     finite_types,
     is_list,
     FlatList,
     is_sequence,
     is_many,
+    DataObject,
+    get_keys,
+    object_to_data,
 ) = expect(
     "_getdefault",
     "coalesce",
     "listwrap",
     "from_data",
     "to_data",
     "list_to_data",
     "finite_types",
     "is_list",
     "FlatList",
     "is_sequence",
     "is_many",
+    "DataObject",
+    "get_keys",
+    "object_to_data",
 )
 
 
 _get = object.__getattribute__
 _set = object.__setattr__
 _new = object.__new__
 
@@ -84,15 +90,15 @@
         else:
             return d != None
 
     __nonzero__ = __bool__
 
     def __contains__(self, item):
         value = Data.__getitem__(self, item)
-        if _get(value, CLASS) in data_types or value:
+        if _get(value, CLASS) in _data_types or value:
             return True
         return False
 
     def __iter__(self):
         d = _get(self, SLOT)
         if _get(d, CLASS) is dict:
             yield from d.items()
@@ -100,15 +106,15 @@
             yield from d.__iter__()
 
     def __getitem__(self, key):
         if key == None:
             return Null
         if key == ".":
             output = _get(self, SLOT)
-            if _get(output, CLASS) in data_types:
+            if _get(output, CLASS) in _data_types:
                 return self
             else:
                 return output
 
         key = str(key)
         d = _get(self, SLOT)
 
@@ -210,54 +216,50 @@
     def __iadd__(self, other):
         return _iadd(self, other)
 
     def __or__(self, other):
         """
         RECURSIVE COALESCE OF DATA PROPERTIES
         """
-        if not _get(other, CLASS) in data_types:
+        if not _get(other, CLASS) in _data_types:
             get_logger().error("Expecting Data")
 
         d = _get(self, SLOT)
         output = Data(**d)  # COPY
         output.__ior__(other)
         return output
 
     def __ror__(self, other):
         """
         RECURSIVE COALESCE OF DATA PROPERTIES
         """
-        if not _get(other, CLASS) in data_types:
+        if not _get(other, CLASS) in _data_types:
             get_logger().error("Expecting Data")
 
         return to_data(other).__or__(self)
 
     def __ior__(self, other):
         """
         RECURSIVE COALESCE OF DATA PROPERTIES
         """
         d = _get(self, SLOT)
-        if not _get(other, CLASS) in data_types:
+        if not _get(other, CLASS) in _data_types:
             if is_missing(d) or (isinstance(d, dict) and not d):
                 _set(self, SLOT, other)
             return self
-        d = _get(self, SLOT)
+
         for ok, ov in other.items():
             if ov == None:
                 continue
 
-            sv = d.get(ok)
+            sv = to_data(d.get(ok))
             if sv == None:
                 d[ok] = ov
-            elif isinstance(sv, Data):
-                sv |= ov
             elif is_data(sv):
-                wv = _new(Data)
-                _set(wv, SLOT, sv)
-                wv |= ov
+                d[ok] = sv | ov
         return self
 
     def __hash__(self):
         d = _get(self, SLOT)
         return hash_value(d)
 
     def __eq__(self, other):
@@ -267,15 +269,15 @@
         d = _get(self, SLOT)
         if _get(d, CLASS) is not dict:
             return d == other
 
         if not d and other == None:
             return False
 
-        if _get(other, CLASS) not in data_types:
+        if _get(other, CLASS) not in _data_types:
             return False
         e = other
         for k, v in d.items():
             if e.get(k) != v:
                 return False
         for k, v in e.items():
             if d.get(k) != v:
@@ -291,15 +293,15 @@
             if default is Null:
                 return NullType(self, key)
             return default
         return v
 
     def items(self):
         d = _get(self, SLOT)
-        return [(k, to_data(v)) for k, v in d.items() if v != None or _get(v, CLASS) in data_types]
+        return [(k, to_data(v)) for k, v in d.items() if v != None or _get(v, CLASS) in _data_types]
 
     def leaves(self, prefix=None):
         """
         LIKE items() BUT RECURSIVE, AND ONLY FOR THE LEAVES (non dict) VALUES
         """
         return leaves(self, prefix)
 
@@ -417,40 +419,37 @@
     SEE leaves_to_data FOR THE INVERSE
 
     :param value: THE Mapping TO TRAVERSE
     :param prefix:  OPTIONAL PREFIX GIVEN TO EACH KEY
     :return: Data, WHICH EACH KEY BEING A PATH INTO value TREE
     """
     if not prefix:
-        yield from _leaves(value, ".")
+        yield from _leaves(".", value)
     else:
-        for k, v in _leaves(value, "."):
+        for k, v in _leaves(".", value):
             yield prefix + k, v
 
 
-def _leaves(value, parent):
-    if isinstance(value, Data):
-        d = _get(value, SLOT)
-        if isinstance(d, dict):
-            items = d.items()
-        else:
-            yield parent, d
-            return
-    else:
-        items = value.items()
+def _leaves(parent, value):
+    value = from_data(value)
+    obj = object_to_data(value)
+    if obj is value:
+        yield parent, value
+        return
 
-    for k, v in items:
+    for k in get_keys(obj):
         try:
+            v = obj[literal_field(k)]
+            if is_missing(v):
+                continue
             kk = concat_field(parent, literal_field(k))
-            if _get(v, CLASS) in data_types:
-                yield from _leaves(v, kk)
-            else:
-                yield kk, to_data(v)
-        except Exception as e:
-            get_logger().error("Do not know how to handle", cause=e)
+            vv = object_to_data(v)
+            yield from _leaves(kk, vv)
+        except Exception as cause:
+            get_logger().error("Do not know how to handle", cause=cause)
 
 
 def _split_field(field):
     """
     SIMPLE SPLIT, NO CHECKS
     """
     return [k.replace("\b", ".") for k in field.replace("..", "\b").split(".")]
@@ -460,15 +459,15 @@
     """
     RECURSIVE ADDITION OF DATA PROPERTIES
     * LISTS ARE CONCATENATED
     * SETS ARE UNIONED
     * NUMBERS ARE ADDED
     """
 
-    if not _get(other, CLASS) in data_types:
+    if not _get(other, CLASS) in _data_types:
         # HAPPENS WHEN _iadd WITH ['.'] SELF REFERENCE
         d = _get(self, SLOT)
         if isinstance(d, dict) and not len(d):
             # LOOKS LIKE A FRESH Data OBJECT (AN IDENTITY ELEMENT)
             # ∀ x, x += {} => x
             d = Data()
         else:
@@ -479,75 +478,75 @@
 
     d = from_data(self)
     for ok, ov in other.items():
         sv = d.get(ok)
         if sv == None:
             d[ok] = from_data(deepcopy(ov))
         elif isinstance(ov, (Decimal, float, long, int)):
-            if _get(sv, CLASS) in data_types:
+            if _get(sv, CLASS) in _data_types:
                 get_logger().error(
                     "can not add {{stype}} with {{otype}",
                     stype=_get(sv, CLASS).__name__,
                     otype=_get(ov, CLASS).__name__,
                 )
             elif is_list(sv):
                 d[ok].append(ov)
             else:
                 d[ok] = sv + ov
         elif is_list(ov):
             d[ok] = from_data(listwrap(sv) + ov)
-        elif _get(ov, CLASS) in data_types:
-            if _get(sv, CLASS) in data_types:
+        elif _get(ov, CLASS) in _data_types:
+            if _get(sv, CLASS) in _data_types:
                 _iadd(sv, ov)
             elif is_list(sv):
                 d[ok].append(ov)
             else:
                 get_logger().error(
                     "can not add {{stype}} with {{otype}",
                     stype=_get(sv, CLASS).__name__,
                     otype=_get(ov, CLASS).__name__,
                 )
         else:
-            if _get(sv, CLASS) in data_types:
+            if _get(sv, CLASS) in _data_types:
                 get_logger().error(
                     "can not add {{stype}} with {{otype}",
                     stype=_get(sv, CLASS).__name__,
                     otype=_get(ov, CLASS).__name__,
                 )
             else:
                 d[ok].append(ov)
     return self
 
 
-data_types = (Data, dict, OrderedDict)  # TYPES TO HOLD DATA
+_data_types = data_types = (Data, dict, OrderedDict)  # TYPES TO HOLD DATA
 
 
 def register_data(type_):
     """
     :param type_:  ADD OTHER TYPE THAT HOLDS DATA
     :return:
     """
-    global data_types
-    data_types = tuple(set(data_types + (type_,)))
+    global _data_types
+    _data_types = tuple(set(_data_types + (type_,)))
 
 
 def is_data(d):
     """
     :param d:
     :return: True IF d IS A TYPE THAT HOLDS DATA
     """
-    return d.__class__ in data_types
+    return d.__class__ in _data_types
 
 
 def is_missing(t) -> bool:
     # RETURN True IF EFFECTIVELY NOTHING
     class_ = t.__class__
     if class_ in null_types:
         return True
-    elif class_ in data_types:
+    elif class_ in _data_types:
         return False
     elif class_ in finite_types and not t:
         return True
     elif class_ is text and not t:
         return True
     else:
         return t == None
@@ -556,15 +555,15 @@
 def exists(value) -> bool:
     return not is_missing(value)
 
 
 def hash_value(v):
     if is_many(v):
         return hash_value(first(v))
-    elif _get(v, CLASS) in data_types:
+    elif _get(v, CLASS) in _data_types:
         return hash_value(first(v.values()))
     else:
         return hash(v)
 
 
 def dict_to_data(d):
     """
@@ -594,15 +593,15 @@
     if value == None:
         return None
 
     class_ = _get(value, CLASS)
     if class_ in (text, binary_type, int, float):
         return value
 
-    if class_ in data_types:
+    if class_ in _data_types:
         if class_ is Data:
             value = from_data(value)
 
         output = {}
         for key, value in value.items():
             value = _leaves_to_data(value)
```

### Comparing `mo-dots-9.584.24095/mo_dots/fields.py` & `mo_dots-9.592.24112/mo_dots/fields.py`

 * *Files identical despite different names*

### Comparing `mo-dots-9.584.24095/mo_dots/lists.py` & `mo_dots-9.592.24112/mo_dots/lists.py`

 * *Files 4% similar despite different names*

```diff
@@ -269,15 +269,15 @@
     def not_right(self, num):
         """
         WITH SLICES BEING FLAT, WE NEED A SIMPLE WAY TO SLICE FROM THE LEFT [:-num:]
         """
         if not num:
             return self
         if num < 0:
-            return Null
+            return self
 
         return FlatList(_get(self, SLOT)[:-num:])
 
     def not_left(self, num):
         """
         NOT REQUIRED, EXISTS AS OPPOSITE OF not_right()
         """
@@ -319,15 +319,15 @@
     return values
 
 
 list_types = (list, FlatList)
 container_types = (list, FlatList, set)
 finite_types = (list, FlatList, set, tuple)
 sequence_types = (list, FlatList, tuple) + generator_types
-many_types = tuple(set(list_types + container_types + sequence_types))
+_many_types = many_types = tuple(set(list_types + container_types + sequence_types))
 
 # ITERATORS THAT ARE CONSIDERED PRIMITIVE
 not_many_names = ("str", "unicode", "binary", "NullType", "NoneType", "dict", "Data")
 
 
 def is_list(l):
     # ORDERED, AND CAN CHANGE CONTENTS
@@ -351,34 +351,38 @@
 
 def is_many(value):
     # REPRESENTS MULTIPLE VALUES
     # TODO: CLEAN UP THIS LOGIC
     # THIS IS COMPLICATED BECAUSE I AM UNSURE ABOUT ALL THE "PRIMITIVE TYPES"
     # I WOULD LIKE TO POSITIVELY CATCH many_types, BUT MAYBE IT IS EASIER TO DETECT: Iterable, BUT NOT PRIMITIVE
     # UNTIL WE HAVE A COMPLETE SLOT, WE KEEP ALL THIS warning() CODE
-    global many_types
+    global _many_types
     type_ = value.__class__
-    if type_ in many_types:
+    if type_ in _many_types:
         return True
 
     if issubclass(type_, types.GeneratorType):
-        many_types = many_types + (type_,)
+        _many_types = _many_types + (type_,)
         Log.warning("is_many() can not detect generator {{type}}", type=type_.__name__)
         return True
     return False
 
 
 def list_to_data(v):
     """
     to_data, BUT WITHOUT CHECKS
     """
     output = _new(FlatList)
     _set(output, SLOT, v)
     return output
 
+def register_many(_type):
+    global _many_types
+    _many_types = _many_types + (_type,)
+
 
 export("mo_dots.datas", finite_types)
 export("mo_dots.datas", is_list)
 export("mo_dots.datas", list_to_data)
 export("mo_dots.datas", FlatList)
 export("mo_dots.datas", is_sequence)
 export("mo_dots.datas", is_many)
```

### Comparing `mo-dots-9.584.24095/mo_dots/nones.py` & `mo_dots-9.592.24112/mo_dots/nones.py`

 * *Files 7% similar despite different names*

```diff
@@ -120,24 +120,31 @@
     def __le__(self, other):
         return Null
 
     def __lt__(self, other):
         return Null
 
     def __eq__(self, other):
-        class_ = _get(other, CLASS)
-        if class_ in null_types:
+        if is_sequence(other) and not other:
             return True
-        elif class_ is list and not other:
+
+        _class = _get(other, CLASS)
+        if _class in null_types:
             return True
         else:
-            return other == None
+            return Null
 
     def __ne__(self, other):
-        return other is not None and _get(other, CLASS) is not NullType and other != None
+        class_ = _get(other, CLASS)
+        if class_ in null_types:
+            return False
+        elif class_ is list and not other:
+            return False
+        else:
+            return Null
 
     def __or__(self, other):
         return other
 
     def __ror__(self, other):
         return other
```

### Comparing `mo-dots-9.584.24095/mo_dots/objects.py` & `mo_dots-9.592.24112/mo_dots/objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,39 +78,15 @@
 
     def get(self, item):
         obj = _get(self, SLOT)
         output = get_attr(obj, item)
         return object_to_data(output)
 
     def keys(self):
-        obj = _get(self, SLOT)
-
-        try:
-            return obj.__dict__.keys()
-        except Exception:
-            pass
-
-        _type = obj.__class__
-        keys = known_types.get(_type)
-        if keys:
-            return keys
-
-        try:
-            keys = _type.__slots__
-            known_types[_type] = keys
-            return keys
-        except Exception:
-            pass
-
-        keys=known_types[_type]=tuple(
-            k
-            for k in dir(_type)
-            if getattr(_type, k).__class__.__name__ in ['member_descriptor', 'getset_descriptor']
-        )
-        return keys
+        return get_keys(self)
 
     def items(self):
         keys = self.keys()
         try:
             for k in keys:
                 yield k, self[k]
         except Exception as cause:
@@ -140,14 +116,48 @@
         obj = _get(self, SLOT)
         return obj(*args, **kwargs)
 
 
 register_data(DataObject)
 
 
+def get_keys(obj):
+    """
+    RETURN keys OF obj, AS IF DATA
+    """
+    while isinstance(obj, (DataObject, Data)):
+        obj = _get(obj, SLOT)
+
+    if isinstance(obj, dict):
+        return obj.keys()
+
+    try:
+        return obj.__dict__.keys()
+    except Exception:
+        pass
+
+    _type = obj.__class__
+    keys = known_types.get(_type)
+    if keys:
+        return keys
+
+    try:
+        keys = known_types[_type] = _type.__slots__
+        return keys
+    except Exception:
+        pass
+
+    keys = known_types[_type] = tuple(
+        k
+        for k in dir(_type)
+        if getattr(_type, k).__class__.__name__ in ['member_descriptor', 'getset_descriptor']
+    )
+    return keys
+
+
 def object_to_data(v):
     try:
         if v == None:
             return Null
     except Exception:
         pass
 
@@ -207,8 +217,11 @@
                 continue
             settings[k] = v
 
     output = {str(k): from_data(settings[k]) for k in params if k in settings}
     return output
 
 
-export("mo_dots.lists", object_to_data)
+export("mo_dots.lists", object_to_data)
+export("mo_dots.datas", object_to_data)
+export("mo_dots.datas", DataObject)
+export("mo_dots.datas", get_keys)
```

### Comparing `mo-dots-9.584.24095/mo_dots/utils.py` & `mo_dots-9.592.24112/mo_dots/utils.py`

 * *Files identical despite different names*

### Comparing `mo-dots-9.584.24095/mo_dots.egg-info/PKG-INFO` & `mo_dots-9.592.24112/mo_dots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.584.24095
+Version: 9.592.24112
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo-dots-9.584.24095/setup.py` & `mo_dots-9.592.24112/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     install_requires=["mo-future==7.584.24095","mo-imports==7.584.24095"],
     license='MPL 2.0',
     long_description='\n# More Dots!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-dots.svg)](https://pypi.org/project/mo-dots/)\n[![Build Status](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-dots/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-dots?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-dots/month)](https://pepy.tech/project/mo-dots)\n\n#### Changes in version 9.x.x\n\nEscaping a literal dot (`.`) is no longer (`\\\\.`) rather double-dot (`..`). Escaping a literal dot can still be done with bell (`\\b`) \n\n#### Changes in version 5.x.x\n\nThe `Data()` constructor only accepts keyword parameters. It no longer accepts a dict, nor does it attempt to clean the input.  Replace `Data(my_var)` with `to_data(my_var)`\n  \n\n## Overview\n\nThis library defines a `Data` class that can serve as a replacement for `dict`, and acts much like a null-safe dataclass.\n\n> See the [full documentation](https://github.com/klahnakoski/mo-dots/tree/dev/docs) for all the features of `mo-dots`\n\n### Create instances\n\nDefine `Data` using named parameters, just like you would a `dict`\n\n    >>> from mo_dots import Data\n    >>> Data(b=42, c="hello world")\n    Data({\'b\': 42, \'c\': \'hello world\'})\n\nYou can also wrap existing `dict`s so they can be used like `Data`\n\n    >>> from mo_dots import to_data\n    >>> to_data({\'b\': 42, \'c\': \'hello world\'})\n    Data({\'b\': 42, \'c\': \'hello world\'})\n\n### Dot Access\n\nAccess properties with attribute dots: `a.b == a["b"]`. You have probably seen this before.\n\n### Path Access\n\nAccess properties by dot-delimited path.\n\n\t>>> a = to_data({"b": {"c": 42}})\n\t>>> a["b.c"] == 42\n\tTrue\n\n### Safe Access\n\nIf a property does not exist then return `Null` rather than raising an error.\n\n\t>>> a = Data()\n\t>>> a.b == None\n\tTrue\n\t>>> a.b.c == None\n\tTrue\n\t>>> a[None] == None\n\tTrue\n\n### Path assignment\n\nNo need to make intermediate `dicts`\n\n    >>> a = Data()\n    >>> a["b.c"] = 42   # same as a.b.c = 42\n    a == {"b": {"c": 42}}\n\n### Path accumulation\n\nUse `+=` to add to a property; default zero (`0`)\n\n    >>> a = Data()\n    a == {}\n    >>> a.b.c += 1\n    a == {"b": {"c": 1}}\n    >>> a.b.c += 42\n    a == {"b": {"c": 43}}\n\nUse `+=` with a list (`[]`) to append to a list; default empty list (`[]`)\n\n    >>> a = Data()\n    a == {}\n    >>> a.b.c += [1]\n    a == {"b": {"c": [1]}}\n    >>> a.b.c += [42]\n    a == {"b": {"c": [1, 42]}}\n\n## Serializing to JSON\n\nThe standard Python JSON library does not recognize `Data` as serializable.  You may overcome this by providing `default=from_data`; which converts the data structures in this module into Python primitives of the same. \n\n    from mo_dots import from_data, to_data\n    \n    s = to_data({"a": ["b", 1]})\n    result = json.dumps(s, default=from_data)  \n\nAlternatively, you may consider [mo-json](https://pypi.org/project/mo-json/) which has a function `value2json` that converts a larger number of data structures into JSON.\n\n\n## Summary\n\nThis library is the basis for a data transformation algebra: We want a succinct way of transforming data in Python. We want operations on data to result in yet more data. We do not want data operations to raise exceptions. This library is solves Python\'s lack of consistency (lack of closure) under the dot (`.`) and slice `[::]` operators when operating on data objects. \n\n[Full documentation](https://github.com/klahnakoski/mo-dots/tree/dev/docs)\n',
     long_description_content_type='text/markdown',
     name='mo-dots',
     packages=["mo_dots"],
     url='https://github.com/klahnakoski/mo-dots',
-    version='9.584.24095',
+    version='9.592.24112',
     zip_safe=False
 )
```


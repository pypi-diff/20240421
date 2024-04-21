# Comparing `tmp/zenyx-1.3.2.tar.gz` & `tmp/zenyx-2.1.0.tar.gz`

## Comparing `zenyx-1.3.2.tar` & `zenyx-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 zenyx-1.3.2/.editorconfig
--rw-r--r--   0        0        0    50890 2020-02-02 00:00:00.000000 zenyx-1.3.2/pyon.debug.md
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 zenyx-1.3.2/src/zenyx/__init__.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 zenyx-1.3.2/src/zenyx/args.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 zenyx-1.3.2/src/zenyx/console.py
--rw-r--r--   0        0        0    15151 2020-02-02 00:00:00.000000 zenyx-1.3.2/src/zenyx/pyon.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 zenyx-1.3.2/src/zenyx/require.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 zenyx-1.3.2/src/zenyx/streams.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 zenyx-1.3.2/tests/databank.py
--rw-r--r--   0        0        0    84842 2020-02-02 00:00:00.000000 zenyx-1.3.2/tests/pyon.debug.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 zenyx-1.3.2/tests/test_main.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zenyx-1.3.2/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 zenyx-1.3.2/LICENSE
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 zenyx-1.3.2/README.md
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 zenyx-1.3.2/pyproject.toml
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 zenyx-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 zenyx-2.1.0/.editorconfig
+-rw-r--r--   0        0        0    80912 2020-02-02 00:00:00.000000 zenyx-2.1.0/pyon.debug.md
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 zenyx-2.1.0/src/zenyx/__init__.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 zenyx-2.1.0/src/zenyx/args.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 zenyx-2.1.0/src/zenyx/console.py
+-rw-r--r--   0        0        0    15128 2020-02-02 00:00:00.000000 zenyx-2.1.0/src/zenyx/pyon.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 zenyx-2.1.0/src/zenyx/require.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 zenyx-2.1.0/src/zenyx/streams.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 zenyx-2.1.0/tests/databank.py
+-rw-r--r--   0        0        0   144790 2020-02-02 00:00:00.000000 zenyx-2.1.0/tests/pyon.debug.md
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 zenyx-2.1.0/tests/test_main.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zenyx-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 zenyx-2.1.0/LICENSE
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 zenyx-2.1.0/README.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 zenyx-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 zenyx-2.1.0/PKG-INFO
```

### Comparing `zenyx-1.3.2/src/zenyx/__init__.py` & `zenyx-2.1.0/src/zenyx/__init__.py`

 * *Files identical despite different names*

### Comparing `zenyx-1.3.2/src/zenyx/args.py` & `zenyx-2.1.0/src/zenyx/args.py`

 * *Files identical despite different names*

### Comparing `zenyx-1.3.2/src/zenyx/console.py` & `zenyx-2.1.0/src/zenyx/console.py`

 * *Files identical despite different names*

### Comparing `zenyx-1.3.2/src/zenyx/pyon.py` & `zenyx-2.1.0/src/zenyx/pyon.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             if debug_file != "":
                 self.debug_file = debug_file
             
             self.debug_path = os.path.join(os.path.dirname(os.path.abspath(self.path)), self.debug_file)
             
             
     
-    debugger: debug_object or None = None
+    debugger: debug_object | None = None
     indent = 1
     
     @staticmethod
     def init(path, *args: str, filename: str = ""):
         """## THIS WILL SLOW DOWN PYON BY ~300%
         Enables the debug feature.
         The debug file will be saved as `pyon.debug.txt`.\n
@@ -231,15 +231,15 @@
     if (not is_type(obj, dict)) and (hasattr(obj, "__dict__") or hasattr(obj, "_asdict")):
         # if it's not a pyon converted named tuple -> it's an object
         if not hasattr(obj, "pyon_converted") or not hasattr(obj, "_asdict"):
             new_dict: dict = copy.deepcopy(obj).__dict__
         else:
             # it's a namedtuple
             new_dict = copy.deepcopy(obj)._asdict()
-        new_dict['PYON_TYPE'] = str(obj.__class__.__name__)
+        new_dict['@class'] = str(obj.__class__.__name__)
     
     if ((not hasattr(obj, "_asdict")) and is_type(obj, tuple)):
         obj = list(obj)
     
     # Handling list[list[list[object]]] edge cases
     if is_type(obj, list):
         for index, element in enumerate(obj):
@@ -274,15 +274,15 @@
     if (xdent == 1):
         debug.indent = 1
     
     return new_dict
 
 
 
-def deep_parse(olddict: dict or list, *args: str, callbacktime: int = 0) -> object or dict:
+def deep_parse(olddict: dict | list, *args: str, callbacktime: int = 0) -> object | dict:
     """
     #### WARNING: IT WILL NOT CONVERT ANY DICTIONARIES WHICH HAVE NOT BEEN SAVED WITH: "__object_to_dict"\n
     Converts the saved dictionary back to the original object
     `Returns` the original object
     """
     class_type: str = ""
     params: dict = {}
@@ -300,17 +300,17 @@
         
     # __debug(f"\n[Deep Parse] Dict/List: {olddict}")
     debug.log(debug.separator_text(title="Start", xdent=xdent, callbackorigin=callbacktime))
     
     if is_type(olddict, list):
         olddict = {"&ORIGINAL_LIST" : olddict}
         
-    if olddict.get('PYON_TYPE'):
-        class_type = olddict["PYON_TYPE"]
-        olddict.pop("PYON_TYPE", None)
+    if olddict.get('@class'):
+        class_type = olddict["@class"]
+        olddict.pop("@class", None)
     else:
         class_type = "&DICT"
         
     # not using is_type() bc of performance
     for key, value in olddict.items():
         if type(value) is dict:
             value = __self_call(value)
@@ -367,46 +367,46 @@
         _json (str): dist json file path
         data (str): the json object waiting to be saved
     """
     with open(_json, "w", encoding="utf-8") as write_file:
         json.dump(data, write_file, indent=4, ensure_ascii=False)
         write_file.write("\n")
 
-def dump(data: dict or list or object, file: str, indent: int = 4):
+def dump(data: dict | list | object, file: str, indent: int = 4):
     """Works the same as the json.dumps function, but exepts objects as data
     Args:
         data (dict or list or object): object or list or object, will be converted to a dict, and into a JSON
         file (str): filepath
         indent (int, optional): the indentation used in the JSON file. Defaults to 4.
     """
     new_data: dict = deep_serialize(data) 
     with open(file, "w", encoding="utf-8") as write_file:
         json.dump(new_data, write_file, indent=indent, ensure_ascii=False)
         write_file.write("\n")
 
-def load(file: str) -> object or dict or list:
+def load(file: str) -> object | dict | list:
     """Loads the json file, and converts all the dictionaries which were objects
     Args:
         file (str): filepath 
     Returns:
         object or dict or list: the decoded json
     """
     with open(file, 'r', encoding="utf-8") as read_file:
         loaddata = json.load(read_file)
         return deep_parse(loaddata)
 
-def dumps(data: object or dict or list) -> str:
+def dumps(data: object | dict | list) -> str:
     """Convert an object into a JSON saveable dict.
     #### THIS ALSO CONVERTS EVERY SUB-OBJECT
     Returns:
         str: the encoded object as a string
     """
     return json.dumps(deep_serialize(data))
 
-def loads(data: str) -> object or dict or list:
+def loads(data: str) -> object | dict | list:
     """Convert the saved JSON string back into objects.
     Args:
         data (str): JSON data
     Returns:
         object or dict or list: decoded JSON object
     """
     return deep_parse(json.loads(data))
```

### Comparing `zenyx-1.3.2/src/zenyx/require.py` & `zenyx-2.1.0/src/zenyx/require.py`

 * *Files identical despite different names*

### Comparing `zenyx-1.3.2/src/zenyx/streams.py` & `zenyx-2.1.0/src/zenyx/streams.py`

 * *Files identical despite different names*

### Comparing `zenyx-1.3.2/tests/pyon.debug.md` & `zenyx-2.1.0/pyon.debug.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,1600 +1,1497 @@
 
-<br>`01:44:06:017` | 
-<br>`01:44:06:017` | **`======================= [Deep Serialize] =======================`**
-<br>`01:44:06:017` | 
-<br>`01:44:06:017` | 
-<br>`01:44:06:017` | 
-<br>`01:44:06:017` | **`========================== [Start: 1] ==========================`**
-<br>`01:44:06:017` | 
-<br>`01:44:06:017` | 
-<br>`01:44:06:017` |   **`[1]`** Original obj input:
-<br>`01:44:06:017` |   	&emsp;`test(param=[test(param={'test': 0}), 'asd'])`
-<br>`01:44:06:017` | 
-<br>`01:44:06:019` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:019` |   	&emsp;Value: `test(param=[test(param={'test': 0}), 'asd'])`, 
-<br>`01:44:06:019` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`01:44:06:019` | 
-<br>`01:44:06:019` |   **`[1]`** Iterability test:
-<br>`01:44:06:019` |   	&emsp;**Params:**
-<br>`01:44:06:019` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': 0}), 'asd'])`
-<br>`01:44:06:019` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`01:44:06:019` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`01:44:06:019` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`01:44:06:019` |   	&emsp;**Final Resoult**: `True`
-<br>`01:44:06:019` | 
-<br>`01:44:06:020` |   **`[1]`** Original Obj Iterability *(can be `False`)*:
-<br>`01:44:06:020` |   	&emsp;Object *(`obj`)*: `test(param=[test(param={'test': 0}), 'asd'])` 
-<br>`01:44:06:020` |   	&emsp;**Is object iterable**: `True`
-<br>`01:44:06:020` | 
-<br>`01:44:06:020` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:020` |   	&emsp;Value: `test(param=[test(param={'test': 0}), 'asd'])`, 
-<br>`01:44:06:020` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`01:44:06:020` | 
-<br>`01:44:06:021` |   **`[1]`** Iterability test:
-<br>`01:44:06:021` |   	&emsp;**Params:**
-<br>`01:44:06:021` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': 0}), 'asd'])`
-<br>`01:44:06:021` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`01:44:06:021` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`01:44:06:021` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`01:44:06:021` |   	&emsp;**Final Resoult**: `True`
-<br>`01:44:06:021` | 
-<br>`01:44:06:021` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:021` |   	&emsp;Value: `test(param=[test(param={'test': 0}), 'asd'])`, 
-<br>`01:44:06:021` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`01:44:06:021` | 
-<br>`01:44:06:022` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:022` |   	&emsp;Value: `test(param=[test(param={'test': 0}), 'asd'])`, 
-<br>`01:44:06:022` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`01:44:06:022` | 
-<br>`01:44:06:023` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:023` |   	&emsp;Value: `test(param=[test(param={'test': 0}), 'asd'])`, 
-<br>`01:44:06:023` |   	&emsp;Type(s): `(<class 'list'>, <class 'tuple'>)`
-<br>`01:44:06:023` | 
-<br>`01:44:06:024` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:024` |   	&emsp;Value: `[test(param={'test': 0}), 'asd']`, 
-<br>`01:44:06:024` |   	&emsp;Type(s): `(<class 'list'>, <class 'tuple'>)`
-<br>`01:44:06:024` | 
-<br>`01:44:06:024` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:024` |   	&emsp;Value: `test(param={'test': 0})`, 
-<br>`01:44:06:024` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`01:44:06:024` | 
-<br>`01:44:06:025` |   **`[1]`** Iterability test:
-<br>`01:44:06:025` |   	&emsp;**Params:**
-<br>`01:44:06:025` |   	&emsp;	&emsp;Value: `test(param={'test': 0})`
-<br>`01:44:06:025` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`01:44:06:025` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`01:44:06:025` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`01:44:06:025` |   	&emsp;**Final Resoult**: `True`
-<br>`01:44:06:025` | 
-<br>`01:44:06:025` | 
-<br>`01:44:06:025` | **`================= [Deep Serialize - Caller: 1] =================`**
-<br>`01:44:06:025` | 
-<br>`01:44:06:025` | 
-<br>`01:44:06:026` | 
-<br>`01:44:06:026` | **`==================== [Start: 2 - Caller: 1] ====================`**
-<br>`01:44:06:026` | 
-<br>`01:44:06:026` | 
-<br>`01:44:06:027` |   **`[2]`** Original obj input:
-<br>`01:44:06:027` |   	&emsp;`test(param={'test': 0})`
-<br>`01:44:06:027` | 
-<br>`01:44:06:027` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:027` |   	&emsp;Value: `test(param={'test': 0})`, 
-<br>`01:44:06:027` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`01:44:06:027` | 
-<br>`01:44:06:027` |   **`[2]`** Iterability test:
-<br>`01:44:06:027` |   	&emsp;**Params:**
-<br>`01:44:06:027` |   	&emsp;	&emsp;Value: `test(param={'test': 0})`
-<br>`01:44:06:027` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`01:44:06:027` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`01:44:06:027` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`01:44:06:027` |   	&emsp;**Final Resoult**: `True`
-<br>`01:44:06:027` | 
-<br>`01:44:06:029` |   **`[2]`** Original Obj Iterability *(can be `False`)*:
-<br>`01:44:06:029` |   	&emsp;Object *(`obj`)*: `test(param={'test': 0})` 
-<br>`01:44:06:029` |   	&emsp;**Is object iterable**: `True`
-<br>`01:44:06:029` | 
-<br>`01:44:06:030` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:030` |   	&emsp;Value: `test(param={'test': 0})`, 
-<br>`01:44:06:030` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`01:44:06:030` | 
-<br>`01:44:06:031` |   **`[2]`** Iterability test:
-<br>`01:44:06:031` |   	&emsp;**Params:**
-<br>`01:44:06:031` |   	&emsp;	&emsp;Value: `test(param={'test': 0})`
-<br>`01:44:06:031` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`01:44:06:031` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`01:44:06:031` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`01:44:06:031` |   	&emsp;**Final Resoult**: `True`
-<br>`01:44:06:031` | 
-<br>`01:44:06:031` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:031` |   	&emsp;Value: `test(param={'test': 0})`, 
-<br>`01:44:06:031` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`01:44:06:031` | 
-<br>`01:44:06:032` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:032` |   	&emsp;Value: `test(param={'test': 0})`, 
-<br>`01:44:06:032` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`01:44:06:032` | 
-<br>`01:44:06:033` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:033` |   	&emsp;Value: `test(param={'test': 0})`, 
-<br>`01:44:06:033` |   	&emsp;Type(s): `(<class 'list'>, <class 'tuple'>)`
-<br>`01:44:06:033` | 
-<br>`01:44:06:034` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:034` |   	&emsp;Value: `{'test': 0}`, 
-<br>`01:44:06:034` |   	&emsp;Type(s): `(<class 'list'>, <class 'tuple'>)`
-<br>`01:44:06:034` | 
-<br>`01:44:06:034` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:034` |   	&emsp;Value: `{'test': 0}`, 
-<br>`01:44:06:034` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`01:44:06:034` | 
-<br>`01:44:06:036` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:036` |   	&emsp;Value: `0`, 
-<br>`01:44:06:036` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`01:44:06:036` | 
-<br>`01:44:06:036` |   **`[2]`** Iterability test:
-<br>`01:44:06:036` |   	&emsp;**Params:**
-<br>`01:44:06:036` |   	&emsp;	&emsp;Value: `0`
-<br>`01:44:06:036` |   	&emsp;	&emsp;@Type: `<class 'int'>`
-<br>`01:44:06:036` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`01:44:06:036` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`01:44:06:036` |   	&emsp;**Final Resoult**: `False`
-<br>`01:44:06:036` | 
-<br>`01:44:06:037` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:037` |   	&emsp;Value: `test`, 
-<br>`01:44:06:037` |   	&emsp;Type(s): `(<class 'list'>, <class 'tuple'>)`
-<br>`01:44:06:037` | 
-<br>`01:44:06:038` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:038` |   	&emsp;Value: `test`, 
-<br>`01:44:06:038` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`01:44:06:038` | 
-<br>`01:44:06:038` |   **`[2]`** **New dict created:**
-<br>`01:44:06:038` |   	&emsp;`{'param': {'test': 0}, 'PYON_TYPE': 'test'}`
-<br>`01:44:06:038` | 
-<br>`01:44:06:039` | 
-<br>`01:44:06:039` | **`===================== [End: 2 - Caller: 1] =====================`**
-<br>`01:44:06:039` | 
-<br>`01:44:06:039` | 
-<br>`01:44:06:040` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:040` |   	&emsp;Value: `asd`, 
-<br>`01:44:06:040` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`01:44:06:040` | 
-<br>`01:44:06:041` |   **`[1]`** Iterability test:
-<br>`01:44:06:041` |   	&emsp;**Params:**
-<br>`01:44:06:041` |   	&emsp;	&emsp;Value: `asd`
-<br>`01:44:06:041` |   	&emsp;	&emsp;@Type: `<class 'str'>`
-<br>`01:44:06:041` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`01:44:06:041` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`01:44:06:041` |   	&emsp;**Final Resoult**: `False`
-<br>`01:44:06:041` | 
-<br>`01:44:06:042` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:042` |   	&emsp;Value: `[{'param': {'test': 0}, 'PYON_TYPE': 'test'}, 'asd']`, 
-<br>`01:44:06:042` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`01:44:06:042` | 
-<br>`01:44:06:043` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:043` |   	&emsp;Value: `test`, 
-<br>`01:44:06:043` |   	&emsp;Type(s): `(<class 'list'>, <class 'tuple'>)`
-<br>`01:44:06:043` | 
-<br>`01:44:06:043` |   **`[TypeCheck]`** Checking Type 
-<br>`01:44:06:043` |   	&emsp;Value: `test`, 
-<br>`01:44:06:043` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`01:44:06:043` | 
-<br>`01:44:06:044` |   **`[1]`** **New dict created:**
-<br>`01:44:06:044` |   	&emsp;`{'param': [{'param': {'test': 0}, 'PYON_TYPE': 'test'}, 'asd'], 'PYON_TYPE': 'test'}`
-<br>`01:44:06:044` | 
-<br>`01:44:06:045` | 
-<br>`01:44:06:045` | **`=========================== [End: 1] ===========================`**
-<br>`01:44:06:045` | 
-<br>`01:44:06:045` | 
-<br>`14:52:51:993` | 
-<br>`14:52:51:993` | **`======================= [Deep Serialize] =======================`**
-<br>`14:52:51:993` | 
-<br>`14:52:51:993` | 
-<br>`14:52:52:006` | 
-<br>`14:52:52:006` | **`========================== [Start: 1] ==========================`**
-<br>`14:52:52:006` | 
-<br>`14:52:52:006` | 
-<br>`14:52:52:007` |   **`[1]`** Original obj input:
-<br>`14:52:52:007` |   	&emsp;`test(param=[test(param={'test': (10, 10)}), 'asd'])`
-<br>`14:52:52:007` | 
-<br>`14:52:52:007` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:007` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:52:52:007` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:52:52:007` | 
-<br>`14:52:52:007` |   **`[1]`** Iterability test:
-<br>`14:52:52:007` |   	&emsp;**Params:**
-<br>`14:52:52:007` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`
-<br>`14:52:52:007` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:52:52:007` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:52:52:007` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:52:52:007` |   	&emsp;**Final Resoult**: `True`
-<br>`14:52:52:007` | 
-<br>`14:52:52:007` |   **`[1]`** Original Obj Iterability *(can be `False`)*:
-<br>`14:52:52:007` |   	&emsp;Object *(`obj`)*: `test(param=[test(param={'test': (10, 10)}), 'asd'])` 
-<br>`14:52:52:007` |   	&emsp;**Is object iterable**: `True`
-<br>`14:52:52:007` | 
-<br>`14:52:52:018` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:018` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:52:52:018` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:52:52:018` | 
-<br>`14:52:52:019` |   **`[1]`** Iterability test:
-<br>`14:52:52:019` |   	&emsp;**Params:**
-<br>`14:52:52:019` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`
-<br>`14:52:52:019` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:52:52:019` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:52:52:019` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:52:52:019` |   	&emsp;**Final Resoult**: `True`
-<br>`14:52:52:019` | 
-<br>`14:52:52:020` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:020` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:52:52:020` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:52:52:020` | 
-<br>`14:52:52:021` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:021` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:52:52:021` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:52:52:021` | 
-<br>`14:52:52:023` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:023` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:52:52:023` |   	&emsp;Type(s): `<class 'tuple'>`
-<br>`14:52:52:023` | 
-<br>`14:52:52:023` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:023` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:52:52:023` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:52:52:023` | 
-<br>`14:52:52:023` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:023` |   	&emsp;Value: `[test(param={'test': (10, 10)}), 'asd']`, 
-<br>`14:52:52:023` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:52:52:023` | 
-<br>`14:52:52:023` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:023` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:52:52:023` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:52:52:023` | 
-<br>`14:52:52:023` |   **`[1]`** Iterability test:
-<br>`14:52:52:023` |   	&emsp;**Params:**
-<br>`14:52:52:023` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
-<br>`14:52:52:023` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:52:52:023` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:52:52:023` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:52:52:023` |   	&emsp;**Final Resoult**: `True`
-<br>`14:52:52:023` | 
-<br>`14:52:52:023` | 
-<br>`14:52:52:023` | **`================= [Deep Serialize - Caller: 1] =================`**
-<br>`14:52:52:023` | 
-<br>`14:52:52:023` | 
-<br>`14:52:52:023` | 
-<br>`14:52:52:023` | **`==================== [Start: 2 - Caller: 1] ====================`**
-<br>`14:52:52:023` | 
-<br>`14:52:52:023` | 
-<br>`14:52:52:023` |   **`[2]`** Original obj input:
-<br>`14:52:52:023` |   	&emsp;`test(param={'test': (10, 10)})`
-<br>`14:52:52:023` | 
-<br>`14:52:52:023` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:023` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:52:52:023` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:52:52:023` | 
-<br>`14:52:52:023` |   **`[2]`** Iterability test:
-<br>`14:52:52:023` |   	&emsp;**Params:**
-<br>`14:52:52:023` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
-<br>`14:52:52:023` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:52:52:023` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:52:52:023` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:52:52:023` |   	&emsp;**Final Resoult**: `True`
-<br>`14:52:52:023` | 
-<br>`14:52:52:023` |   **`[2]`** Original Obj Iterability *(can be `False`)*:
-<br>`14:52:52:023` |   	&emsp;Object *(`obj`)*: `test(param={'test': (10, 10)})` 
-<br>`14:52:52:023` |   	&emsp;**Is object iterable**: `True`
-<br>`14:52:52:023` | 
-<br>`14:52:52:023` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:023` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:52:52:023` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:52:52:023` | 
-<br>`14:52:52:023` |   **`[2]`** Iterability test:
-<br>`14:52:52:023` |   	&emsp;**Params:**
-<br>`14:52:52:023` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
-<br>`14:52:52:023` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:52:52:023` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:52:52:023` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:52:52:023` |   	&emsp;**Final Resoult**: `True`
-<br>`14:52:52:023` | 
-<br>`14:52:52:023` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:023` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:52:52:023` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:52:52:023` | 
-<br>`14:52:52:035` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:035` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:52:52:035` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:52:52:035` | 
-<br>`14:52:52:036` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:036` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:52:52:036` |   	&emsp;Type(s): `<class 'tuple'>`
-<br>`14:52:52:036` | 
-<br>`14:52:52:037` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:037` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:52:52:037` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:52:52:037` | 
-<br>`14:52:52:038` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:038` |   	&emsp;Value: `{'test': (10, 10)}`, 
-<br>`14:52:52:038` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:52:52:038` | 
-<br>`14:52:52:039` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:039` |   	&emsp;Value: `{'test': (10, 10)}`, 
-<br>`14:52:52:039` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:52:52:039` | 
-<br>`14:52:52:041` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:041` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:52:52:041` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:52:52:041` | 
-<br>`14:52:52:041` |   **`[2]`** Iterability test:
-<br>`14:52:52:041` |   	&emsp;**Params:**
-<br>`14:52:52:041` |   	&emsp;	&emsp;Value: `(10, 10)`
-<br>`14:52:52:041` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
-<br>`14:52:52:041` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:52:52:041` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
-<br>`14:52:52:041` |   	&emsp;**Final Resoult**: `True`
-<br>`14:52:52:041` | 
-<br>`14:52:52:041` | 
-<br>`14:52:52:041` | **`================= [Deep Serialize - Caller: 2] =================`**
-<br>`14:52:52:041` | 
-<br>`14:52:52:041` | 
-<br>`14:52:52:041` | 
-<br>`14:52:52:041` | **`==================== [Start: 3 - Caller: 2] ====================`**
-<br>`14:52:52:041` | 
-<br>`14:52:52:041` | 
-<br>`14:52:52:041` |   **`[3]`** Original obj input:
-<br>`14:52:52:041` |   	&emsp;`(10, 10)`
-<br>`14:52:52:041` | 
-<br>`14:52:52:041` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:041` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:52:52:041` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:52:52:041` | 
-<br>`14:52:52:041` |   **`[3]`** Iterability test:
-<br>`14:52:52:041` |   	&emsp;**Params:**
-<br>`14:52:52:041` |   	&emsp;	&emsp;Value: `(10, 10)`
-<br>`14:52:52:041` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
-<br>`14:52:52:041` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:52:52:041` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
-<br>`14:52:52:041` |   	&emsp;**Final Resoult**: `True`
-<br>`14:52:52:041` | 
-<br>`14:52:52:041` |   **`[3]`** Original Obj Iterability *(can be `False`)*:
-<br>`14:52:52:041` |   	&emsp;Object *(`obj`)*: `(10, 10)` 
-<br>`14:52:52:041` |   	&emsp;**Is object iterable**: `True`
-<br>`14:52:52:041` | 
-<br>`14:52:52:041` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:041` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:52:52:041` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:52:52:041` | 
-<br>`14:52:52:041` |   **`[3]`** Iterability test:
-<br>`14:52:52:041` |   	&emsp;**Params:**
-<br>`14:52:52:041` |   	&emsp;	&emsp;Value: `(10, 10)`
-<br>`14:52:52:041` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
-<br>`14:52:52:041` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:52:52:041` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
-<br>`14:52:52:041` |   	&emsp;**Final Resoult**: `True`
-<br>`14:52:52:041` | 
-<br>`14:52:52:041` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:041` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:52:52:041` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:52:52:041` | 
-<br>`14:52:52:051` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:051` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:52:52:051` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:52:52:051` | 
-<br>`14:52:52:052` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:052` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:52:52:052` |   	&emsp;Type(s): `<class 'tuple'>`
-<br>`14:52:52:052` | 
-<br>`14:52:52:054` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:054` |   	&emsp;Value: `[10, 10]`, 
-<br>`14:52:52:054` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` |   **`[3]`** Iterating List/Tuple:
-<br>`14:52:52:054` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
-<br>`14:52:52:054` |   	&emsp;Element: `10`
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:054` |   	&emsp;Value: `10`, 
-<br>`14:52:52:054` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` |   **`[3]`** Iterability test:
-<br>`14:52:52:054` |   	&emsp;**Params:**
-<br>`14:52:52:054` |   	&emsp;	&emsp;Value: `10`
-<br>`14:52:52:054` |   	&emsp;	&emsp;@Type: `<class 'int'>`
-<br>`14:52:52:054` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:52:52:054` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:52:52:054` |   	&emsp;**Final Resoult**: `False`
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` |   **`[3]`** Iterating List/Tuple:
-<br>`14:52:52:054` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
-<br>`14:52:52:054` |   	&emsp;Element: `10`
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:054` |   	&emsp;Value: `10`, 
-<br>`14:52:52:054` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` |   **`[3]`** Iterability test:
-<br>`14:52:52:054` |   	&emsp;**Params:**
-<br>`14:52:52:054` |   	&emsp;	&emsp;Value: `10`
-<br>`14:52:52:054` |   	&emsp;	&emsp;@Type: `<class 'int'>`
-<br>`14:52:52:054` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:52:52:054` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:52:52:054` |   	&emsp;**Final Resoult**: `False`
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` | **`========== [Early End: 3 - Caller: 2] List Serialized ==========`**
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:054` |   	&emsp;Value: `test`, 
-<br>`14:52:52:054` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:054` |   	&emsp;Value: `test`, 
-<br>`14:52:52:054` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` |   **`[2]`** **New dict created:**
-<br>`14:52:52:054` |   	&emsp;`{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}`
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` | **`===================== [End: 2 - Caller: 1] =====================`**
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:054` |   	&emsp;Value: `asd`, 
-<br>`14:52:52:054` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` |   **`[1]`** Iterability test:
-<br>`14:52:52:054` |   	&emsp;**Params:**
-<br>`14:52:52:054` |   	&emsp;	&emsp;Value: `asd`
-<br>`14:52:52:054` |   	&emsp;	&emsp;@Type: `<class 'str'>`
-<br>`14:52:52:054` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:52:52:054` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:52:52:054` |   	&emsp;**Final Resoult**: `False`
-<br>`14:52:52:054` | 
-<br>`14:52:52:054` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:054` |   	&emsp;Value: `[{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}, 'asd']`, 
-<br>`14:52:52:054` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:52:52:054` | 
-<br>`14:52:52:069` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:069` |   	&emsp;Value: `test`, 
-<br>`14:52:52:069` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:52:52:069` | 
-<br>`14:52:52:070` |   **`[TypeCheck]`** Checking Type 
-<br>`14:52:52:070` |   	&emsp;Value: `test`, 
-<br>`14:52:52:070` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:52:52:070` | 
-<br>`14:52:52:070` |   **`[1]`** **New dict created:**
-<br>`14:52:52:070` |   	&emsp;`{'param': [{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}, 'asd'], 'PYON_TYPE': 'test'}`
-<br>`14:52:52:070` | 
-<br>`14:52:52:070` | 
-<br>`14:52:52:070` | **`=========================== [End: 1] ===========================`**
-<br>`14:52:52:070` | 
-<br>`14:52:52:070` | 
-<br>`14:53:36:247` | 
-<br>`14:53:36:247` | **`======================= [Deep Serialize] =======================`**
-<br>`14:53:36:247` | 
-<br>`14:53:36:247` | 
-<br>`14:53:36:248` | 
-<br>`14:53:36:248` | **`========================== [Start: 1] ==========================`**
-<br>`14:53:36:248` | 
-<br>`14:53:36:248` | 
-<br>`14:53:36:249` |   **`[1]`** Original obj input:
-<br>`14:53:36:249` |   	&emsp;`test(param=[test(param={'test': (10, 10)}), 'asd'])`
-<br>`14:53:36:249` | 
-<br>`14:53:36:251` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:251` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:53:36:251` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:251` | 
-<br>`14:53:36:252` |   **`[1]`** Iterability test:
-<br>`14:53:36:252` |   	&emsp;**Params:**
-<br>`14:53:36:252` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`
-<br>`14:53:36:252` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:53:36:252` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:53:36:252` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:53:36:252` |   	&emsp;**Final Resoult**: `True`
-<br>`14:53:36:252` | 
-<br>`14:53:36:252` |   **`[1]`** Original Obj Iterability *(can be `False`)*:
-<br>`14:53:36:252` |   	&emsp;Object *(`obj`)*: `test(param=[test(param={'test': (10, 10)}), 'asd'])` 
-<br>`14:53:36:252` |   	&emsp;**Is object iterable**: `True`
-<br>`14:53:36:252` | 
-<br>`14:53:36:252` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:252` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:53:36:252` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:252` | 
-<br>`14:53:36:252` |   **`[1]`** Iterability test:
-<br>`14:53:36:252` |   	&emsp;**Params:**
-<br>`14:53:36:252` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`
-<br>`14:53:36:252` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:53:36:252` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:53:36:252` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:53:36:252` |   	&emsp;**Final Resoult**: `True`
-<br>`14:53:36:252` | 
-<br>`14:53:36:252` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:252` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:53:36:252` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:252` | 
-<br>`14:53:36:252` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:252` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:53:36:252` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:252` | 
-<br>`14:53:36:252` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:252` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:53:36:252` |   	&emsp;Type(s): `<class 'tuple'>`
-<br>`14:53:36:252` | 
-<br>`14:53:36:252` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:252` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:53:36:252` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:53:36:252` | 
-<br>`14:53:36:252` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:252` |   	&emsp;Value: `[test(param={'test': (10, 10)}), 'asd']`, 
-<br>`14:53:36:252` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:53:36:252` | 
-<br>`14:53:36:252` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:252` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:53:36:252` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:252` | 
-<br>`14:53:36:252` |   **`[1]`** Iterability test:
-<br>`14:53:36:252` |   	&emsp;**Params:**
-<br>`14:53:36:252` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
-<br>`14:53:36:252` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:53:36:252` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:53:36:252` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:53:36:252` |   	&emsp;**Final Resoult**: `True`
-<br>`14:53:36:252` | 
-<br>`14:53:36:252` | 
-<br>`14:53:36:252` | **`================= [Deep Serialize - Caller: 1] =================`**
-<br>`14:53:36:252` | 
-<br>`14:53:36:252` | 
-<br>`14:53:36:252` | 
-<br>`14:53:36:252` | **`==================== [Start: 2 - Caller: 1] ====================`**
-<br>`14:53:36:252` | 
-<br>`14:53:36:252` | 
-<br>`14:53:36:252` |   **`[2]`** Original obj input:
-<br>`14:53:36:252` |   	&emsp;`test(param={'test': (10, 10)})`
-<br>`14:53:36:252` | 
-<br>`14:53:36:268` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:268` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:53:36:268` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:268` | 
-<br>`14:53:36:268` |   **`[2]`** Iterability test:
-<br>`14:53:36:268` |   	&emsp;**Params:**
-<br>`14:53:36:268` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
-<br>`14:53:36:268` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:53:36:268` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:53:36:268` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:53:36:268` |   	&emsp;**Final Resoult**: `True`
-<br>`14:53:36:268` | 
-<br>`14:53:36:268` |   **`[2]`** Original Obj Iterability *(can be `False`)*:
-<br>`14:53:36:268` |   	&emsp;Object *(`obj`)*: `test(param={'test': (10, 10)})` 
-<br>`14:53:36:268` |   	&emsp;**Is object iterable**: `True`
-<br>`14:53:36:268` | 
-<br>`14:53:36:268` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:268` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:53:36:268` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:268` | 
-<br>`14:53:36:268` |   **`[2]`** Iterability test:
-<br>`14:53:36:268` |   	&emsp;**Params:**
-<br>`14:53:36:268` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
-<br>`14:53:36:268` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:53:36:268` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:53:36:268` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:53:36:268` |   	&emsp;**Final Resoult**: `True`
-<br>`14:53:36:268` | 
-<br>`14:53:36:268` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:268` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:53:36:268` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:268` | 
-<br>`14:53:36:268` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:268` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:53:36:268` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:268` | 
-<br>`14:53:36:268` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:268` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:53:36:268` |   	&emsp;Type(s): `<class 'tuple'>`
-<br>`14:53:36:268` | 
-<br>`14:53:36:268` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:268` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:53:36:268` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:53:36:268` | 
-<br>`14:53:36:268` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:268` |   	&emsp;Value: `{'test': (10, 10)}`, 
-<br>`14:53:36:268` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:53:36:268` | 
-<br>`14:53:36:268` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:268` |   	&emsp;Value: `{'test': (10, 10)}`, 
-<br>`14:53:36:268` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:268` | 
-<br>`14:53:36:268` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:268` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:53:36:268` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:268` | 
-<br>`14:53:36:268` |   **`[2]`** Iterability test:
-<br>`14:53:36:268` |   	&emsp;**Params:**
-<br>`14:53:36:268` |   	&emsp;	&emsp;Value: `(10, 10)`
-<br>`14:53:36:268` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
-<br>`14:53:36:268` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:53:36:268` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
-<br>`14:53:36:268` |   	&emsp;**Final Resoult**: `True`
-<br>`14:53:36:268` | 
-<br>`14:53:36:268` | 
-<br>`14:53:36:268` | **`================= [Deep Serialize - Caller: 2] =================`**
-<br>`14:53:36:268` | 
-<br>`14:53:36:268` | 
-<br>`14:53:36:284` | 
-<br>`14:53:36:284` | **`==================== [Start: 3 - Caller: 2] ====================`**
-<br>`14:53:36:284` | 
-<br>`14:53:36:284` | 
-<br>`14:53:36:285` |   **`[3]`** Original obj input:
-<br>`14:53:36:285` |   	&emsp;`(10, 10)`
-<br>`14:53:36:285` | 
-<br>`14:53:36:285` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:285` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:53:36:285` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:285` | 
-<br>`14:53:36:285` |   **`[3]`** Iterability test:
-<br>`14:53:36:285` |   	&emsp;**Params:**
-<br>`14:53:36:285` |   	&emsp;	&emsp;Value: `(10, 10)`
-<br>`14:53:36:285` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
-<br>`14:53:36:285` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:53:36:285` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
-<br>`14:53:36:285` |   	&emsp;**Final Resoult**: `True`
-<br>`14:53:36:285` | 
-<br>`14:53:36:285` |   **`[3]`** Original Obj Iterability *(can be `False`)*:
-<br>`14:53:36:285` |   	&emsp;Object *(`obj`)*: `(10, 10)` 
-<br>`14:53:36:285` |   	&emsp;**Is object iterable**: `True`
-<br>`14:53:36:285` | 
-<br>`14:53:36:285` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:285` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:53:36:285` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:285` | 
-<br>`14:53:36:285` |   **`[3]`** Iterability test:
-<br>`14:53:36:285` |   	&emsp;**Params:**
-<br>`14:53:36:285` |   	&emsp;	&emsp;Value: `(10, 10)`
-<br>`14:53:36:285` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
-<br>`14:53:36:285` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:53:36:285` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
-<br>`14:53:36:285` |   	&emsp;**Final Resoult**: `True`
-<br>`14:53:36:285` | 
-<br>`14:53:36:285` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:285` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:53:36:285` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:285` | 
-<br>`14:53:36:285` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:285` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:53:36:285` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:285` | 
-<br>`14:53:36:285` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:285` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:53:36:285` |   	&emsp;Type(s): `<class 'tuple'>`
-<br>`14:53:36:285` | 
-<br>`14:53:36:285` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:285` |   	&emsp;Value: `[10, 10]`, 
-<br>`14:53:36:285` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:53:36:285` | 
-<br>`14:53:36:285` |   **`[3]`** Iterating List/Tuple:
-<br>`14:53:36:285` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
-<br>`14:53:36:285` |   	&emsp;Element: `10`
-<br>`14:53:36:285` | 
-<br>`14:53:36:285` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:285` |   	&emsp;Value: `10`, 
-<br>`14:53:36:285` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:285` | 
-<br>`14:53:36:285` |   **`[3]`** Iterability test:
-<br>`14:53:36:285` |   	&emsp;**Params:**
-<br>`14:53:36:285` |   	&emsp;	&emsp;Value: `10`
-<br>`14:53:36:285` |   	&emsp;	&emsp;@Type: `<class 'int'>`
-<br>`14:53:36:285` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:53:36:285` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:53:36:285` |   	&emsp;**Final Resoult**: `False`
-<br>`14:53:36:285` | 
-<br>`14:53:36:301` |   **`[3]`** Iterating List/Tuple:
-<br>`14:53:36:301` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
-<br>`14:53:36:301` |   	&emsp;Element: `10`
-<br>`14:53:36:301` | 
-<br>`14:53:36:302` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:302` |   	&emsp;Value: `10`, 
-<br>`14:53:36:302` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` |   **`[3]`** Iterability test:
-<br>`14:53:36:302` |   	&emsp;**Params:**
-<br>`14:53:36:302` |   	&emsp;	&emsp;Value: `10`
-<br>`14:53:36:302` |   	&emsp;	&emsp;@Type: `<class 'int'>`
-<br>`14:53:36:302` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:53:36:302` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:53:36:302` |   	&emsp;**Final Resoult**: `False`
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` | **`========== [Early End: 3 - Caller: 2] List Serialized ==========`**
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:302` |   	&emsp;Value: `test`, 
-<br>`14:53:36:302` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:302` |   	&emsp;Value: `test`, 
-<br>`14:53:36:302` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` |   **`[2]`** **New dict created:**
-<br>`14:53:36:302` |   	&emsp;`{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}`
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` | **`===================== [End: 2 - Caller: 1] =====================`**
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:302` |   	&emsp;Value: `asd`, 
-<br>`14:53:36:302` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` |   **`[1]`** Iterability test:
-<br>`14:53:36:302` |   	&emsp;**Params:**
-<br>`14:53:36:302` |   	&emsp;	&emsp;Value: `asd`
-<br>`14:53:36:302` |   	&emsp;	&emsp;@Type: `<class 'str'>`
-<br>`14:53:36:302` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:53:36:302` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:53:36:302` |   	&emsp;**Final Resoult**: `False`
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:302` |   	&emsp;Value: `[{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}, 'asd']`, 
-<br>`14:53:36:302` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:302` |   	&emsp;Value: `test`, 
-<br>`14:53:36:302` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:302` |   	&emsp;Value: `test`, 
-<br>`14:53:36:302` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` |   **`[1]`** **New dict created:**
-<br>`14:53:36:302` |   	&emsp;`{'param': [{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}, 'asd'], 'PYON_TYPE': 'test'}`
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` | **`=========================== [End: 1] ===========================`**
-<br>`14:53:36:302` | 
-<br>`14:53:36:302` | 
-<br>`14:53:36:317` | 
-<br>`14:53:36:317` | **`======================= [Deep Serialize] =======================`**
-<br>`14:53:36:317` | 
-<br>`14:53:36:317` | 
-<br>`14:53:36:317` | 
-<br>`14:53:36:317` | **`========================== [Start: 1] ==========================`**
-<br>`14:53:36:317` | 
-<br>`14:53:36:317` | 
-<br>`14:53:36:319` |   **`[1]`** Original obj input:
-<br>`14:53:36:319` |   	&emsp;`test(param=[test(param={'test': (10, 10)}), 'asd'])`
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:319` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:53:36:319` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` |   **`[1]`** Iterability test:
-<br>`14:53:36:319` |   	&emsp;**Params:**
-<br>`14:53:36:319` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`
-<br>`14:53:36:319` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:53:36:319` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:53:36:319` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:53:36:319` |   	&emsp;**Final Resoult**: `True`
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` |   **`[1]`** Original Obj Iterability *(can be `False`)*:
-<br>`14:53:36:319` |   	&emsp;Object *(`obj`)*: `test(param=[test(param={'test': (10, 10)}), 'asd'])` 
-<br>`14:53:36:319` |   	&emsp;**Is object iterable**: `True`
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:319` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:53:36:319` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` |   **`[1]`** Iterability test:
-<br>`14:53:36:319` |   	&emsp;**Params:**
-<br>`14:53:36:319` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`
-<br>`14:53:36:319` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:53:36:319` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:53:36:319` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:53:36:319` |   	&emsp;**Final Resoult**: `True`
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:319` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:53:36:319` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:319` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:53:36:319` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:319` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:53:36:319` |   	&emsp;Type(s): `<class 'tuple'>`
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:319` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:53:36:319` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:319` |   	&emsp;Value: `[test(param={'test': (10, 10)}), 'asd']`, 
-<br>`14:53:36:319` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:319` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:53:36:319` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` |   **`[1]`** Iterability test:
-<br>`14:53:36:319` |   	&emsp;**Params:**
-<br>`14:53:36:319` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
-<br>`14:53:36:319` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:53:36:319` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:53:36:319` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:53:36:319` |   	&emsp;**Final Resoult**: `True`
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` | **`================= [Deep Serialize - Caller: 1] =================`**
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` | **`==================== [Start: 2 - Caller: 1] ====================`**
-<br>`14:53:36:319` | 
-<br>`14:53:36:319` | 
-<br>`14:53:36:335` |   **`[2]`** Original obj input:
-<br>`14:53:36:335` |   	&emsp;`test(param={'test': (10, 10)})`
-<br>`14:53:36:335` | 
-<br>`14:53:36:335` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:335` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:53:36:335` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:335` | 
-<br>`14:53:36:335` |   **`[2]`** Iterability test:
-<br>`14:53:36:335` |   	&emsp;**Params:**
-<br>`14:53:36:335` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
-<br>`14:53:36:335` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:53:36:335` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:53:36:335` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:53:36:335` |   	&emsp;**Final Resoult**: `True`
-<br>`14:53:36:335` | 
-<br>`14:53:36:335` |   **`[2]`** Original Obj Iterability *(can be `False`)*:
-<br>`14:53:36:335` |   	&emsp;Object *(`obj`)*: `test(param={'test': (10, 10)})` 
-<br>`14:53:36:335` |   	&emsp;**Is object iterable**: `True`
-<br>`14:53:36:335` | 
-<br>`14:53:36:335` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:335` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:53:36:335` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:335` | 
-<br>`14:53:36:335` |   **`[2]`** Iterability test:
-<br>`14:53:36:335` |   	&emsp;**Params:**
-<br>`14:53:36:335` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
-<br>`14:53:36:335` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:53:36:335` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:53:36:335` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:53:36:335` |   	&emsp;**Final Resoult**: `True`
-<br>`14:53:36:335` | 
-<br>`14:53:36:335` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:335` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:53:36:335` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:335` | 
-<br>`14:53:36:335` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:335` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:53:36:335` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:335` | 
-<br>`14:53:36:335` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:335` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:53:36:335` |   	&emsp;Type(s): `<class 'tuple'>`
-<br>`14:53:36:335` | 
-<br>`14:53:36:335` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:335` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:53:36:335` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:53:36:335` | 
-<br>`14:53:36:335` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:335` |   	&emsp;Value: `{'test': (10, 10)}`, 
-<br>`14:53:36:335` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:53:36:335` | 
-<br>`14:53:36:335` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:335` |   	&emsp;Value: `{'test': (10, 10)}`, 
-<br>`14:53:36:335` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:335` | 
-<br>`14:53:36:335` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:335` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:53:36:335` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:335` | 
-<br>`14:53:36:335` |   **`[2]`** Iterability test:
-<br>`14:53:36:335` |   	&emsp;**Params:**
-<br>`14:53:36:335` |   	&emsp;	&emsp;Value: `(10, 10)`
-<br>`14:53:36:335` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
-<br>`14:53:36:335` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:53:36:335` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
-<br>`14:53:36:335` |   	&emsp;**Final Resoult**: `True`
-<br>`14:53:36:335` | 
-<br>`14:53:36:350` | 
-<br>`14:53:36:350` | **`================= [Deep Serialize - Caller: 2] =================`**
-<br>`14:53:36:350` | 
-<br>`14:53:36:350` | 
-<br>`14:53:36:350` | 
-<br>`14:53:36:350` | **`==================== [Start: 3 - Caller: 2] ====================`**
-<br>`14:53:36:350` | 
-<br>`14:53:36:350` | 
-<br>`14:53:36:352` |   **`[3]`** Original obj input:
-<br>`14:53:36:352` |   	&emsp;`(10, 10)`
-<br>`14:53:36:352` | 
-<br>`14:53:36:353` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:353` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:53:36:353` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:353` | 
-<br>`14:53:36:354` |   **`[3]`** Iterability test:
-<br>`14:53:36:354` |   	&emsp;**Params:**
-<br>`14:53:36:354` |   	&emsp;	&emsp;Value: `(10, 10)`
-<br>`14:53:36:354` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
-<br>`14:53:36:354` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:53:36:354` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
-<br>`14:53:36:354` |   	&emsp;**Final Resoult**: `True`
-<br>`14:53:36:354` | 
-<br>`14:53:36:355` |   **`[3]`** Original Obj Iterability *(can be `False`)*:
-<br>`14:53:36:355` |   	&emsp;Object *(`obj`)*: `(10, 10)` 
-<br>`14:53:36:355` |   	&emsp;**Is object iterable**: `True`
-<br>`14:53:36:355` | 
-<br>`14:53:36:356` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:356` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:53:36:356` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:356` | 
-<br>`14:53:36:357` |   **`[3]`** Iterability test:
-<br>`14:53:36:357` |   	&emsp;**Params:**
-<br>`14:53:36:357` |   	&emsp;	&emsp;Value: `(10, 10)`
-<br>`14:53:36:357` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
-<br>`14:53:36:357` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:53:36:357` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
-<br>`14:53:36:357` |   	&emsp;**Final Resoult**: `True`
-<br>`14:53:36:357` | 
-<br>`14:53:36:358` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:358` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:53:36:358` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:358` | 
-<br>`14:53:36:359` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:359` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:53:36:359` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:359` | 
-<br>`14:53:36:360` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:360` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:53:36:360` |   	&emsp;Type(s): `<class 'tuple'>`
-<br>`14:53:36:360` | 
-<br>`14:53:36:361` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:361` |   	&emsp;Value: `[10, 10]`, 
-<br>`14:53:36:361` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:53:36:361` | 
-<br>`14:53:36:362` |   **`[3]`** Iterating List/Tuple:
-<br>`14:53:36:362` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
-<br>`14:53:36:362` |   	&emsp;Element: `10`
-<br>`14:53:36:362` | 
-<br>`14:53:36:363` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:363` |   	&emsp;Value: `10`, 
-<br>`14:53:36:363` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:363` | 
-<br>`14:53:36:364` |   **`[3]`** Iterability test:
-<br>`14:53:36:364` |   	&emsp;**Params:**
-<br>`14:53:36:364` |   	&emsp;	&emsp;Value: `10`
-<br>`14:53:36:364` |   	&emsp;	&emsp;@Type: `<class 'int'>`
-<br>`14:53:36:364` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:53:36:364` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:53:36:364` |   	&emsp;**Final Resoult**: `False`
-<br>`14:53:36:364` | 
-<br>`14:53:36:365` |   **`[3]`** Iterating List/Tuple:
-<br>`14:53:36:365` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
-<br>`14:53:36:365` |   	&emsp;Element: `10`
-<br>`14:53:36:365` | 
-<br>`14:53:36:366` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:366` |   	&emsp;Value: `10`, 
-<br>`14:53:36:366` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:366` | 
-<br>`14:53:36:367` |   **`[3]`** Iterability test:
-<br>`14:53:36:367` |   	&emsp;**Params:**
-<br>`14:53:36:367` |   	&emsp;	&emsp;Value: `10`
-<br>`14:53:36:367` |   	&emsp;	&emsp;@Type: `<class 'int'>`
-<br>`14:53:36:367` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:53:36:367` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:53:36:367` |   	&emsp;**Final Resoult**: `False`
-<br>`14:53:36:367` | 
-<br>`14:53:36:368` | 
-<br>`14:53:36:368` | **`========== [Early End: 3 - Caller: 2] List Serialized ==========`**
-<br>`14:53:36:368` | 
-<br>`14:53:36:368` | 
-<br>`14:53:36:369` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:369` |   	&emsp;Value: `test`, 
-<br>`14:53:36:369` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:53:36:369` | 
-<br>`14:53:36:370` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:370` |   	&emsp;Value: `test`, 
-<br>`14:53:36:370` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:370` | 
-<br>`14:53:36:371` |   **`[2]`** **New dict created:**
-<br>`14:53:36:371` |   	&emsp;`{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}`
-<br>`14:53:36:371` | 
-<br>`14:53:36:372` | 
-<br>`14:53:36:372` | **`===================== [End: 2 - Caller: 1] =====================`**
-<br>`14:53:36:372` | 
-<br>`14:53:36:372` | 
-<br>`14:53:36:373` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:373` |   	&emsp;Value: `asd`, 
-<br>`14:53:36:373` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:53:36:373` | 
-<br>`14:53:36:374` |   **`[1]`** Iterability test:
-<br>`14:53:36:374` |   	&emsp;**Params:**
-<br>`14:53:36:374` |   	&emsp;	&emsp;Value: `asd`
-<br>`14:53:36:374` |   	&emsp;	&emsp;@Type: `<class 'str'>`
-<br>`14:53:36:374` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:53:36:374` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:53:36:374` |   	&emsp;**Final Resoult**: `False`
-<br>`14:53:36:374` | 
-<br>`14:53:36:375` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:375` |   	&emsp;Value: `[{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}, 'asd']`, 
-<br>`14:53:36:375` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:375` | 
-<br>`14:53:36:376` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:376` |   	&emsp;Value: `test`, 
-<br>`14:53:36:376` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:53:36:376` | 
-<br>`14:53:36:377` |   **`[TypeCheck]`** Checking Type 
-<br>`14:53:36:377` |   	&emsp;Value: `test`, 
-<br>`14:53:36:377` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:53:36:377` | 
-<br>`14:53:36:378` |   **`[1]`** **New dict created:**
-<br>`14:53:36:378` |   	&emsp;`{'param': [{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}, 'asd'], 'PYON_TYPE': 'test'}`
-<br>`14:53:36:378` | 
-<br>`14:53:36:379` | 
-<br>`14:53:36:379` | **`=========================== [End: 1] ===========================`**
-<br>`14:53:36:379` | 
-<br>`14:53:36:379` | 
-<br>`14:54:07:422` | 
-<br>`14:54:07:422` | **`======================= [Deep Serialize] =======================`**
-<br>`14:54:07:422` | 
-<br>`14:54:07:422` | 
-<br>`14:54:07:423` | 
-<br>`14:54:07:423` | **`========================== [Start: 1] ==========================`**
-<br>`14:54:07:423` | 
-<br>`14:54:07:423` | 
-<br>`14:54:07:424` |   **`[1]`** Original obj input:
-<br>`14:54:07:424` |   	&emsp;`test(param=[test(param={'test': (10, 10)}), 'asd'])`
-<br>`14:54:07:424` | 
-<br>`14:54:07:424` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:424` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:54:07:424` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:424` | 
-<br>`14:54:07:424` |   **`[1]`** Iterability test:
-<br>`14:54:07:424` |   	&emsp;**Params:**
-<br>`14:54:07:424` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`
-<br>`14:54:07:424` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:54:07:424` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:54:07:424` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:54:07:424` |   	&emsp;**Final Resoult**: `True`
-<br>`14:54:07:424` | 
-<br>`14:54:07:424` |   **`[1]`** Original Obj Iterability *(can be `False`)*:
-<br>`14:54:07:424` |   	&emsp;Object *(`obj`)*: `test(param=[test(param={'test': (10, 10)}), 'asd'])` 
-<br>`14:54:07:424` |   	&emsp;**Is object iterable**: `True`
-<br>`14:54:07:424` | 
-<br>`14:54:07:424` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:424` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:54:07:424` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:424` | 
-<br>`14:54:07:424` |   **`[1]`** Iterability test:
-<br>`14:54:07:424` |   	&emsp;**Params:**
-<br>`14:54:07:424` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`
-<br>`14:54:07:424` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:54:07:424` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:54:07:424` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:54:07:424` |   	&emsp;**Final Resoult**: `True`
-<br>`14:54:07:424` | 
-<br>`14:54:07:424` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:424` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:54:07:424` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:424` | 
-<br>`14:54:07:424` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:424` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:54:07:424` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:424` | 
-<br>`14:54:07:434` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:434` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:54:07:434` |   	&emsp;Type(s): `<class 'tuple'>`
-<br>`14:54:07:434` | 
-<br>`14:54:07:435` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:435` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:54:07:435` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:54:07:435` | 
-<br>`14:54:07:437` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:437` |   	&emsp;Value: `[test(param={'test': (10, 10)}), 'asd']`, 
-<br>`14:54:07:437` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:54:07:437` | 
-<br>`14:54:07:438` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:438` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:54:07:438` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:438` | 
-<br>`14:54:07:439` |   **`[1]`** Iterability test:
-<br>`14:54:07:439` |   	&emsp;**Params:**
-<br>`14:54:07:439` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
-<br>`14:54:07:439` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:54:07:439` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:54:07:439` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:54:07:439` |   	&emsp;**Final Resoult**: `True`
-<br>`14:54:07:439` | 
-<br>`14:54:07:439` | 
-<br>`14:54:07:439` | **`================= [Deep Serialize - Caller: 1] =================`**
-<br>`14:54:07:439` | 
-<br>`14:54:07:439` | 
-<br>`14:54:07:439` | 
-<br>`14:54:07:439` | **`==================== [Start: 2 - Caller: 1] ====================`**
-<br>`14:54:07:439` | 
-<br>`14:54:07:439` | 
-<br>`14:54:07:439` |   **`[2]`** Original obj input:
-<br>`14:54:07:439` |   	&emsp;`test(param={'test': (10, 10)})`
-<br>`14:54:07:439` | 
-<br>`14:54:07:439` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:439` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:54:07:439` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:439` | 
-<br>`14:54:07:439` |   **`[2]`** Iterability test:
-<br>`14:54:07:439` |   	&emsp;**Params:**
-<br>`14:54:07:439` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
-<br>`14:54:07:439` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:54:07:439` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:54:07:439` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:54:07:439` |   	&emsp;**Final Resoult**: `True`
-<br>`14:54:07:439` | 
-<br>`14:54:07:439` |   **`[2]`** Original Obj Iterability *(can be `False`)*:
-<br>`14:54:07:439` |   	&emsp;Object *(`obj`)*: `test(param={'test': (10, 10)})` 
-<br>`14:54:07:439` |   	&emsp;**Is object iterable**: `True`
-<br>`14:54:07:439` | 
-<br>`14:54:07:439` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:439` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:54:07:439` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:439` | 
-<br>`14:54:07:439` |   **`[2]`** Iterability test:
-<br>`14:54:07:439` |   	&emsp;**Params:**
-<br>`14:54:07:439` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
-<br>`14:54:07:439` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:54:07:439` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:54:07:439` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:54:07:439` |   	&emsp;**Final Resoult**: `True`
-<br>`14:54:07:439` | 
-<br>`14:54:07:439` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:439` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:54:07:439` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:439` | 
-<br>`14:54:07:451` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:451` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:54:07:451` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:451` | 
-<br>`14:54:07:453` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:453` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:54:07:453` |   	&emsp;Type(s): `<class 'tuple'>`
-<br>`14:54:07:453` | 
-<br>`14:54:07:453` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:453` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:54:07:453` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:54:07:453` | 
-<br>`14:54:07:453` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:453` |   	&emsp;Value: `{'test': (10, 10)}`, 
-<br>`14:54:07:453` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:54:07:453` | 
-<br>`14:54:07:453` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:453` |   	&emsp;Value: `{'test': (10, 10)}`, 
-<br>`14:54:07:453` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:453` | 
-<br>`14:54:07:453` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:453` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:54:07:453` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:453` | 
-<br>`14:54:07:453` |   **`[2]`** Iterability test:
-<br>`14:54:07:453` |   	&emsp;**Params:**
-<br>`14:54:07:453` |   	&emsp;	&emsp;Value: `(10, 10)`
-<br>`14:54:07:453` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
-<br>`14:54:07:453` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:54:07:453` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
-<br>`14:54:07:453` |   	&emsp;**Final Resoult**: `True`
-<br>`14:54:07:453` | 
-<br>`14:54:07:453` | 
-<br>`14:54:07:453` | **`================= [Deep Serialize - Caller: 2] =================`**
-<br>`14:54:07:453` | 
-<br>`14:54:07:453` | 
-<br>`14:54:07:453` | 
-<br>`14:54:07:453` | **`==================== [Start: 3 - Caller: 2] ====================`**
-<br>`14:54:07:453` | 
-<br>`14:54:07:453` | 
-<br>`14:54:07:453` |   **`[3]`** Original obj input:
-<br>`14:54:07:453` |   	&emsp;`(10, 10)`
-<br>`14:54:07:453` | 
-<br>`14:54:07:453` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:453` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:54:07:453` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:453` | 
-<br>`14:54:07:453` |   **`[3]`** Iterability test:
-<br>`14:54:07:453` |   	&emsp;**Params:**
-<br>`14:54:07:453` |   	&emsp;	&emsp;Value: `(10, 10)`
-<br>`14:54:07:453` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
-<br>`14:54:07:453` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:54:07:453` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
-<br>`14:54:07:453` |   	&emsp;**Final Resoult**: `True`
-<br>`14:54:07:453` | 
-<br>`14:54:07:453` |   **`[3]`** Original Obj Iterability *(can be `False`)*:
-<br>`14:54:07:453` |   	&emsp;Object *(`obj`)*: `(10, 10)` 
-<br>`14:54:07:453` |   	&emsp;**Is object iterable**: `True`
-<br>`14:54:07:453` | 
-<br>`14:54:07:453` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:453` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:54:07:453` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:453` | 
-<br>`14:54:07:467` |   **`[3]`** Iterability test:
-<br>`14:54:07:467` |   	&emsp;**Params:**
-<br>`14:54:07:467` |   	&emsp;	&emsp;Value: `(10, 10)`
-<br>`14:54:07:467` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
-<br>`14:54:07:467` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:54:07:467` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
-<br>`14:54:07:467` |   	&emsp;**Final Resoult**: `True`
-<br>`14:54:07:467` | 
-<br>`14:54:07:469` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:469` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:54:07:469` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:469` | 
-<br>`14:54:07:470` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:470` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:54:07:470` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:470` | 
-<br>`14:54:07:471` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:471` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:54:07:471` |   	&emsp;Type(s): `<class 'tuple'>`
-<br>`14:54:07:471` | 
-<br>`14:54:07:473` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:473` |   	&emsp;Value: `[10, 10]`, 
-<br>`14:54:07:473` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:54:07:473` | 
-<br>`14:54:07:473` |   **`[3]`** Iterating List/Tuple:
-<br>`14:54:07:473` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
-<br>`14:54:07:473` |   	&emsp;Element: `10`
-<br>`14:54:07:473` | 
-<br>`14:54:07:473` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:473` |   	&emsp;Value: `10`, 
-<br>`14:54:07:473` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:473` | 
-<br>`14:54:07:473` |   **`[3]`** Iterability test:
-<br>`14:54:07:473` |   	&emsp;**Params:**
-<br>`14:54:07:473` |   	&emsp;	&emsp;Value: `10`
-<br>`14:54:07:473` |   	&emsp;	&emsp;@Type: `<class 'int'>`
-<br>`14:54:07:473` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:54:07:473` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:54:07:473` |   	&emsp;**Final Resoult**: `False`
-<br>`14:54:07:473` | 
-<br>`14:54:07:473` |   **`[3]`** Iterating List/Tuple:
-<br>`14:54:07:473` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
-<br>`14:54:07:473` |   	&emsp;Element: `10`
-<br>`14:54:07:473` | 
-<br>`14:54:07:473` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:473` |   	&emsp;Value: `10`, 
-<br>`14:54:07:473` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:473` | 
-<br>`14:54:07:473` |   **`[3]`** Iterability test:
-<br>`14:54:07:473` |   	&emsp;**Params:**
-<br>`14:54:07:473` |   	&emsp;	&emsp;Value: `10`
-<br>`14:54:07:473` |   	&emsp;	&emsp;@Type: `<class 'int'>`
-<br>`14:54:07:473` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:54:07:473` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:54:07:473` |   	&emsp;**Final Resoult**: `False`
-<br>`14:54:07:473` | 
-<br>`14:54:07:473` | 
-<br>`14:54:07:473` | **`========== [Early End: 3 - Caller: 2] List Serialized ==========`**
-<br>`14:54:07:473` | 
-<br>`14:54:07:473` | 
-<br>`14:54:07:473` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:473` |   	&emsp;Value: `test`, 
-<br>`14:54:07:473` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:54:07:473` | 
-<br>`14:54:07:473` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:473` |   	&emsp;Value: `test`, 
-<br>`14:54:07:473` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:473` | 
-<br>`14:54:07:485` |   **`[2]`** **New dict created:**
-<br>`14:54:07:485` |   	&emsp;`{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}`
-<br>`14:54:07:485` | 
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` | **`===================== [End: 2 - Caller: 1] =====================`**
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:486` |   	&emsp;Value: `asd`, 
-<br>`14:54:07:486` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` |   **`[1]`** Iterability test:
-<br>`14:54:07:486` |   	&emsp;**Params:**
-<br>`14:54:07:486` |   	&emsp;	&emsp;Value: `asd`
-<br>`14:54:07:486` |   	&emsp;	&emsp;@Type: `<class 'str'>`
-<br>`14:54:07:486` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:54:07:486` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:54:07:486` |   	&emsp;**Final Resoult**: `False`
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:486` |   	&emsp;Value: `[{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}, 'asd']`, 
-<br>`14:54:07:486` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:486` |   	&emsp;Value: `test`, 
-<br>`14:54:07:486` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:486` |   	&emsp;Value: `test`, 
-<br>`14:54:07:486` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` |   **`[1]`** **New dict created:**
-<br>`14:54:07:486` |   	&emsp;`{'param': [{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}, 'asd'], 'PYON_TYPE': 'test'}`
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` | **`=========================== [End: 1] ===========================`**
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` | **`======================= [Deep Serialize] =======================`**
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` | **`========================== [Start: 1] ==========================`**
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` |   **`[1]`** Original obj input:
-<br>`14:54:07:486` |   	&emsp;`test(param=[test(param={'test': (10, 10)}), 'asd'])`
-<br>`14:54:07:486` | 
-<br>`14:54:07:486` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:486` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:54:07:486` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:486` | 
-<br>`14:54:07:501` |   **`[1]`** Iterability test:
-<br>`14:54:07:501` |   	&emsp;**Params:**
-<br>`14:54:07:501` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`
-<br>`14:54:07:501` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:54:07:501` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:54:07:501` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:54:07:501` |   	&emsp;**Final Resoult**: `True`
-<br>`14:54:07:501` | 
-<br>`14:54:07:502` |   **`[1]`** Original Obj Iterability *(can be `False`)*:
-<br>`14:54:07:502` |   	&emsp;Object *(`obj`)*: `test(param=[test(param={'test': (10, 10)}), 'asd'])` 
-<br>`14:54:07:502` |   	&emsp;**Is object iterable**: `True`
-<br>`14:54:07:502` | 
-<br>`14:54:07:502` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:502` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:54:07:502` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:502` | 
-<br>`14:54:07:502` |   **`[1]`** Iterability test:
-<br>`14:54:07:502` |   	&emsp;**Params:**
-<br>`14:54:07:502` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`
-<br>`14:54:07:502` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:54:07:502` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:54:07:502` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:54:07:502` |   	&emsp;**Final Resoult**: `True`
-<br>`14:54:07:502` | 
-<br>`14:54:07:502` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:502` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:54:07:502` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:502` | 
-<br>`14:54:07:502` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:502` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:54:07:502` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:502` | 
-<br>`14:54:07:502` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:502` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:54:07:502` |   	&emsp;Type(s): `<class 'tuple'>`
-<br>`14:54:07:502` | 
-<br>`14:54:07:502` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:502` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
-<br>`14:54:07:502` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:54:07:502` | 
-<br>`14:54:07:502` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:502` |   	&emsp;Value: `[test(param={'test': (10, 10)}), 'asd']`, 
-<br>`14:54:07:502` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:54:07:502` | 
-<br>`14:54:07:502` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:502` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:54:07:502` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:502` | 
-<br>`14:54:07:502` |   **`[1]`** Iterability test:
-<br>`14:54:07:502` |   	&emsp;**Params:**
-<br>`14:54:07:502` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
-<br>`14:54:07:502` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:54:07:502` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:54:07:502` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:54:07:502` |   	&emsp;**Final Resoult**: `True`
-<br>`14:54:07:502` | 
-<br>`14:54:07:502` | 
-<br>`14:54:07:502` | **`================= [Deep Serialize - Caller: 1] =================`**
-<br>`14:54:07:502` | 
-<br>`14:54:07:502` | 
-<br>`14:54:07:502` | 
-<br>`14:54:07:502` | **`==================== [Start: 2 - Caller: 1] ====================`**
-<br>`14:54:07:502` | 
-<br>`14:54:07:502` | 
-<br>`14:54:07:502` |   **`[2]`** Original obj input:
-<br>`14:54:07:502` |   	&emsp;`test(param={'test': (10, 10)})`
-<br>`14:54:07:502` | 
-<br>`14:54:07:517` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:517` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:54:07:517` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:517` | 
-<br>`14:54:07:518` |   **`[2]`** Iterability test:
-<br>`14:54:07:518` |   	&emsp;**Params:**
-<br>`14:54:07:518` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
-<br>`14:54:07:518` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:54:07:518` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:54:07:518` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:54:07:518` |   	&emsp;**Final Resoult**: `True`
-<br>`14:54:07:518` | 
-<br>`14:54:07:519` |   **`[2]`** Original Obj Iterability *(can be `False`)*:
-<br>`14:54:07:519` |   	&emsp;Object *(`obj`)*: `test(param={'test': (10, 10)})` 
-<br>`14:54:07:519` |   	&emsp;**Is object iterable**: `True`
-<br>`14:54:07:519` | 
-<br>`14:54:07:520` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:520` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:54:07:520` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:520` | 
-<br>`14:54:07:522` |   **`[2]`** Iterability test:
-<br>`14:54:07:522` |   	&emsp;**Params:**
-<br>`14:54:07:522` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
-<br>`14:54:07:522` |   	&emsp;	&emsp;@Type: `<class 'databank.test'>`
-<br>`14:54:07:522` |   	&emsp;Is object *(`__is_object`)*: `True`
-<br>`14:54:07:522` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:54:07:522` |   	&emsp;**Final Resoult**: `True`
-<br>`14:54:07:522` | 
-<br>`14:54:07:523` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:523` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:54:07:523` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:523` | 
-<br>`14:54:07:524` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:524` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:54:07:524` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:524` | 
-<br>`14:54:07:525` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:525` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:54:07:525` |   	&emsp;Type(s): `<class 'tuple'>`
-<br>`14:54:07:525` | 
-<br>`14:54:07:526` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:526` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
-<br>`14:54:07:526` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:54:07:526` | 
-<br>`14:54:07:527` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:527` |   	&emsp;Value: `{'test': (10, 10)}`, 
-<br>`14:54:07:527` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:54:07:527` | 
-<br>`14:54:07:528` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:528` |   	&emsp;Value: `{'test': (10, 10)}`, 
-<br>`14:54:07:528` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:528` | 
-<br>`14:54:07:529` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:529` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:54:07:529` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:529` | 
-<br>`14:54:07:531` |   **`[2]`** Iterability test:
-<br>`14:54:07:531` |   	&emsp;**Params:**
-<br>`14:54:07:531` |   	&emsp;	&emsp;Value: `(10, 10)`
-<br>`14:54:07:531` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
-<br>`14:54:07:531` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:54:07:531` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
-<br>`14:54:07:531` |   	&emsp;**Final Resoult**: `True`
-<br>`14:54:07:531` | 
-<br>`14:54:07:532` | 
-<br>`14:54:07:532` | **`================= [Deep Serialize - Caller: 2] =================`**
-<br>`14:54:07:532` | 
-<br>`14:54:07:532` | 
-<br>`14:54:07:533` | 
-<br>`14:54:07:533` | **`==================== [Start: 3 - Caller: 2] ====================`**
-<br>`14:54:07:533` | 
-<br>`14:54:07:533` | 
-<br>`14:54:07:534` |   **`[3]`** Original obj input:
-<br>`14:54:07:534` |   	&emsp;`(10, 10)`
-<br>`14:54:07:534` | 
-<br>`14:54:07:535` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:535` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:54:07:535` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:535` | 
-<br>`14:54:07:536` |   **`[3]`** Iterability test:
-<br>`14:54:07:536` |   	&emsp;**Params:**
-<br>`14:54:07:536` |   	&emsp;	&emsp;Value: `(10, 10)`
-<br>`14:54:07:536` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
-<br>`14:54:07:536` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:54:07:536` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
-<br>`14:54:07:536` |   	&emsp;**Final Resoult**: `True`
-<br>`14:54:07:536` | 
-<br>`14:54:07:537` |   **`[3]`** Original Obj Iterability *(can be `False`)*:
-<br>`14:54:07:537` |   	&emsp;Object *(`obj`)*: `(10, 10)` 
-<br>`14:54:07:537` |   	&emsp;**Is object iterable**: `True`
-<br>`14:54:07:537` | 
-<br>`14:54:07:538` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:538` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:54:07:538` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:538` | 
-<br>`14:54:07:539` |   **`[3]`** Iterability test:
-<br>`14:54:07:539` |   	&emsp;**Params:**
-<br>`14:54:07:539` |   	&emsp;	&emsp;Value: `(10, 10)`
-<br>`14:54:07:539` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
-<br>`14:54:07:539` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:54:07:539` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
-<br>`14:54:07:539` |   	&emsp;**Final Resoult**: `True`
-<br>`14:54:07:539` | 
-<br>`14:54:07:540` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:540` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:54:07:540` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:540` | 
-<br>`14:54:07:541` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:541` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:54:07:541` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:541` | 
-<br>`14:54:07:542` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:542` |   	&emsp;Value: `(10, 10)`, 
-<br>`14:54:07:542` |   	&emsp;Type(s): `<class 'tuple'>`
-<br>`14:54:07:542` | 
-<br>`14:54:07:543` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:543` |   	&emsp;Value: `[10, 10]`, 
-<br>`14:54:07:543` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:54:07:543` | 
-<br>`14:54:07:544` |   **`[3]`** Iterating List/Tuple:
-<br>`14:54:07:544` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
-<br>`14:54:07:544` |   	&emsp;Element: `10`
-<br>`14:54:07:544` | 
-<br>`14:54:07:545` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:545` |   	&emsp;Value: `10`, 
-<br>`14:54:07:545` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:545` | 
-<br>`14:54:07:546` |   **`[3]`** Iterability test:
-<br>`14:54:07:546` |   	&emsp;**Params:**
-<br>`14:54:07:546` |   	&emsp;	&emsp;Value: `10`
-<br>`14:54:07:546` |   	&emsp;	&emsp;@Type: `<class 'int'>`
-<br>`14:54:07:546` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:54:07:546` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:54:07:546` |   	&emsp;**Final Resoult**: `False`
-<br>`14:54:07:546` | 
-<br>`14:54:07:547` |   **`[3]`** Iterating List/Tuple:
-<br>`14:54:07:547` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
-<br>`14:54:07:547` |   	&emsp;Element: `10`
-<br>`14:54:07:547` | 
-<br>`14:54:07:549` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:549` |   	&emsp;Value: `10`, 
-<br>`14:54:07:549` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:549` | 
-<br>`14:54:07:550` |   **`[3]`** Iterability test:
-<br>`14:54:07:550` |   	&emsp;**Params:**
-<br>`14:54:07:550` |   	&emsp;	&emsp;Value: `10`
-<br>`14:54:07:550` |   	&emsp;	&emsp;@Type: `<class 'int'>`
-<br>`14:54:07:550` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:54:07:550` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:54:07:550` |   	&emsp;**Final Resoult**: `False`
-<br>`14:54:07:550` | 
-<br>`14:54:07:551` | 
-<br>`14:54:07:551` | **`========== [Early End: 3 - Caller: 2] List Serialized ==========`**
-<br>`14:54:07:551` | 
-<br>`14:54:07:551` | 
-<br>`14:54:07:551` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:551` |   	&emsp;Value: `test`, 
-<br>`14:54:07:551` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:54:07:551` | 
-<br>`14:54:07:551` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:551` |   	&emsp;Value: `test`, 
-<br>`14:54:07:551` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:551` | 
-<br>`14:54:07:551` |   **`[2]`** **New dict created:**
-<br>`14:54:07:551` |   	&emsp;`{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}`
-<br>`14:54:07:551` | 
-<br>`14:54:07:551` | 
-<br>`14:54:07:551` | **`===================== [End: 2 - Caller: 1] =====================`**
-<br>`14:54:07:551` | 
-<br>`14:54:07:551` | 
-<br>`14:54:07:551` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:551` |   	&emsp;Value: `asd`, 
-<br>`14:54:07:551` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
-<br>`14:54:07:551` | 
-<br>`14:54:07:551` |   **`[1]`** Iterability test:
-<br>`14:54:07:551` |   	&emsp;**Params:**
-<br>`14:54:07:551` |   	&emsp;	&emsp;Value: `asd`
-<br>`14:54:07:551` |   	&emsp;	&emsp;@Type: `<class 'str'>`
-<br>`14:54:07:551` |   	&emsp;Is object *(`__is_object`)*: `False`
-<br>`14:54:07:551` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
-<br>`14:54:07:551` |   	&emsp;**Final Resoult**: `False`
-<br>`14:54:07:551` | 
-<br>`14:54:07:551` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:551` |   	&emsp;Value: `[{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}, 'asd']`, 
-<br>`14:54:07:551` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:551` | 
-<br>`14:54:07:551` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:551` |   	&emsp;Value: `test`, 
-<br>`14:54:07:551` |   	&emsp;Type(s): `<class 'list'>`
-<br>`14:54:07:551` | 
-<br>`14:54:07:551` |   **`[TypeCheck]`** Checking Type 
-<br>`14:54:07:551` |   	&emsp;Value: `test`, 
-<br>`14:54:07:551` |   	&emsp;Type(s): `<class 'dict'>`
-<br>`14:54:07:551` | 
-<br>`14:54:07:551` |   **`[1]`** **New dict created:**
-<br>`14:54:07:551` |   	&emsp;`{'param': [{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}, 'asd'], 'PYON_TYPE': 'test'}`
-<br>`14:54:07:551` | 
-<br>`14:54:07:551` | 
-<br>`14:54:07:551` | **`=========================== [End: 1] ===========================`**
-<br>`14:54:07:551` | 
-<br>`14:54:07:551` | 
+<br>`17:36:15:782` | 
+<br>`17:36:15:782` | **`======================= [Deep Serialize] =======================`**
+<br>`17:36:15:782` | 
+<br>`17:36:15:782` | 
+<br>`17:36:15:782` | 
+<br>`17:36:15:782` | **`========================== [Start: 1] ==========================`**
+<br>`17:36:15:782` | 
+<br>`17:36:15:782` | 
+<br>`17:36:15:783` |   **`[1]`** Original obj input:
+<br>`17:36:15:783` |   	&emsp;`test(param=[test(param={'test': (10, 10)}), 'asd'])`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:783` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`17:36:15:783` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[1]`** Iterability test:
+<br>`17:36:15:783` |   	&emsp;**Params:**
+<br>`17:36:15:783` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`
+<br>`17:36:15:783` |   	&emsp;	&emsp;@Type: `<class 'tests.databank.test'>`
+<br>`17:36:15:783` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`17:36:15:783` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:783` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[1]`** Original Obj Iterability *(can be `False`)*:
+<br>`17:36:15:783` |   	&emsp;Object *(`obj`)*: `test(param=[test(param={'test': (10, 10)}), 'asd'])` 
+<br>`17:36:15:783` |   	&emsp;**Is object iterable**: `True`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:783` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`17:36:15:783` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[1]`** Iterability test:
+<br>`17:36:15:783` |   	&emsp;**Params:**
+<br>`17:36:15:783` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`
+<br>`17:36:15:783` |   	&emsp;	&emsp;@Type: `<class 'tests.databank.test'>`
+<br>`17:36:15:783` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`17:36:15:783` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:783` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:783` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`17:36:15:783` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:783` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`17:36:15:783` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:783` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`17:36:15:783` |   	&emsp;Type(s): `<class 'tuple'>`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:783` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`17:36:15:783` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:783` |   	&emsp;Value: `[test(param={'test': (10, 10)}), 'asd']`, 
+<br>`17:36:15:783` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:783` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`17:36:15:783` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[1]`** Iterability test:
+<br>`17:36:15:783` |   	&emsp;**Params:**
+<br>`17:36:15:783` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
+<br>`17:36:15:783` |   	&emsp;	&emsp;@Type: `<class 'tests.databank.test'>`
+<br>`17:36:15:783` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`17:36:15:783` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:783` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` | **`================= [Deep Serialize - Caller: 1] =================`**
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` | **`==================== [Start: 2 - Caller: 1] ====================`**
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[2]`** Original obj input:
+<br>`17:36:15:783` |   	&emsp;`test(param={'test': (10, 10)})`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:783` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`17:36:15:783` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[2]`** Iterability test:
+<br>`17:36:15:783` |   	&emsp;**Params:**
+<br>`17:36:15:783` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
+<br>`17:36:15:783` |   	&emsp;	&emsp;@Type: `<class 'tests.databank.test'>`
+<br>`17:36:15:783` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`17:36:15:783` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:783` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[2]`** Original Obj Iterability *(can be `False`)*:
+<br>`17:36:15:783` |   	&emsp;Object *(`obj`)*: `test(param={'test': (10, 10)})` 
+<br>`17:36:15:783` |   	&emsp;**Is object iterable**: `True`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:783` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`17:36:15:783` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[2]`** Iterability test:
+<br>`17:36:15:783` |   	&emsp;**Params:**
+<br>`17:36:15:783` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
+<br>`17:36:15:783` |   	&emsp;	&emsp;@Type: `<class 'tests.databank.test'>`
+<br>`17:36:15:783` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`17:36:15:783` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:783` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:783` | 
+<br>`17:36:15:783` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:783` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`17:36:15:783` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:783` | 
+<br>`17:36:15:799` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:799` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`17:36:15:799` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:799` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`17:36:15:799` |   	&emsp;Type(s): `<class 'tuple'>`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:799` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`17:36:15:799` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:799` |   	&emsp;Value: `{'test': (10, 10)}`, 
+<br>`17:36:15:799` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:799` |   	&emsp;Value: `{'test': (10, 10)}`, 
+<br>`17:36:15:799` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:799` |   	&emsp;Value: `(10, 10)`, 
+<br>`17:36:15:799` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[2]`** Iterability test:
+<br>`17:36:15:799` |   	&emsp;**Params:**
+<br>`17:36:15:799` |   	&emsp;	&emsp;Value: `(10, 10)`
+<br>`17:36:15:799` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
+<br>`17:36:15:799` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:799` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`17:36:15:799` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` | **`================= [Deep Serialize - Caller: 2] =================`**
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` | **`==================== [Start: 3 - Caller: 2] ====================`**
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[3]`** Original obj input:
+<br>`17:36:15:799` |   	&emsp;`(10, 10)`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:799` |   	&emsp;Value: `(10, 10)`, 
+<br>`17:36:15:799` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[3]`** Iterability test:
+<br>`17:36:15:799` |   	&emsp;**Params:**
+<br>`17:36:15:799` |   	&emsp;	&emsp;Value: `(10, 10)`
+<br>`17:36:15:799` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
+<br>`17:36:15:799` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:799` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`17:36:15:799` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[3]`** Original Obj Iterability *(can be `False`)*:
+<br>`17:36:15:799` |   	&emsp;Object *(`obj`)*: `(10, 10)` 
+<br>`17:36:15:799` |   	&emsp;**Is object iterable**: `True`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:799` |   	&emsp;Value: `(10, 10)`, 
+<br>`17:36:15:799` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[3]`** Iterability test:
+<br>`17:36:15:799` |   	&emsp;**Params:**
+<br>`17:36:15:799` |   	&emsp;	&emsp;Value: `(10, 10)`
+<br>`17:36:15:799` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
+<br>`17:36:15:799` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:799` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`17:36:15:799` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:799` |   	&emsp;Value: `(10, 10)`, 
+<br>`17:36:15:799` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:799` |   	&emsp;Value: `(10, 10)`, 
+<br>`17:36:15:799` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:799` |   	&emsp;Value: `(10, 10)`, 
+<br>`17:36:15:799` |   	&emsp;Type(s): `<class 'tuple'>`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:799` |   	&emsp;Value: `[10, 10]`, 
+<br>`17:36:15:799` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[3]`** Iterating List/Tuple:
+<br>`17:36:15:799` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
+<br>`17:36:15:799` |   	&emsp;Element: `10`
+<br>`17:36:15:799` | 
+<br>`17:36:15:799` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:799` |   	&emsp;Value: `10`, 
+<br>`17:36:15:799` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:799` | 
+<br>`17:36:15:814` |   **`[3]`** Iterability test:
+<br>`17:36:15:814` |   	&emsp;**Params:**
+<br>`17:36:15:814` |   	&emsp;	&emsp;Value: `10`
+<br>`17:36:15:814` |   	&emsp;	&emsp;@Type: `<class 'int'>`
+<br>`17:36:15:814` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:814` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:814` |   	&emsp;**Final Resoult**: `False`
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` |   **`[3]`** Iterating List/Tuple:
+<br>`17:36:15:814` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
+<br>`17:36:15:814` |   	&emsp;Element: `10`
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:814` |   	&emsp;Value: `10`, 
+<br>`17:36:15:814` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` |   **`[3]`** Iterability test:
+<br>`17:36:15:814` |   	&emsp;**Params:**
+<br>`17:36:15:814` |   	&emsp;	&emsp;Value: `10`
+<br>`17:36:15:814` |   	&emsp;	&emsp;@Type: `<class 'int'>`
+<br>`17:36:15:814` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:814` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:814` |   	&emsp;**Final Resoult**: `False`
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` | **`========== [Early End: 3 - Caller: 2] List Serialized ==========`**
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:814` |   	&emsp;Value: `test`, 
+<br>`17:36:15:814` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:814` |   	&emsp;Value: `test`, 
+<br>`17:36:15:814` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` |   **`[2]`** **New dict created:**
+<br>`17:36:15:814` |   	&emsp;`{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}`
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` | **`===================== [End: 2 - Caller: 1] =====================`**
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:814` |   	&emsp;Value: `asd`, 
+<br>`17:36:15:814` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` |   **`[1]`** Iterability test:
+<br>`17:36:15:814` |   	&emsp;**Params:**
+<br>`17:36:15:814` |   	&emsp;	&emsp;Value: `asd`
+<br>`17:36:15:814` |   	&emsp;	&emsp;@Type: `<class 'str'>`
+<br>`17:36:15:814` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:814` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:814` |   	&emsp;**Final Resoult**: `False`
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:814` |   	&emsp;Value: `[{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}, 'asd']`, 
+<br>`17:36:15:814` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:814` |   	&emsp;Value: `test`, 
+<br>`17:36:15:814` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:814` |   	&emsp;Value: `test`, 
+<br>`17:36:15:814` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` |   **`[1]`** **New dict created:**
+<br>`17:36:15:814` |   	&emsp;`{'param': [{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}, 'asd'], 'PYON_TYPE': 'test'}`
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` | **`=========================== [End: 1] ===========================`**
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` | **`========================= [Deep Parse] =========================`**
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` | **`========================== [Start: 1] ==========================`**
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` | 
+<br>`17:36:15:814` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:814` |   	&emsp;Value: `{'param': [{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}, 'asd'], 'PYON_TYPE': 'test'}`, 
+<br>`17:36:15:814` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:814` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | **`=================== [Deep Parse - Caller: 1] ===================`**
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | **`==================== [Start: 2 - Caller: 1] ====================`**
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:830` |   	&emsp;Value: `{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}`, 
+<br>`17:36:15:830` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | **`=================== [Deep Parse - Caller: 2] ===================`**
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | **`==================== [Start: 3 - Caller: 2] ====================`**
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:830` |   	&emsp;Value: `{'test': [10, 10]}`, 
+<br>`17:36:15:830` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` |   **`[3]`** Return Value: 
+<br>`17:36:15:830` |   	&emsp;`{'test': [10, 10]}`
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | **`===================== [End: 3 - Caller: 2] =====================`**
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` |   **`[2]`** Return Value: 
+<br>`17:36:15:830` |   	&emsp;`test(param={'test': [10, 10]}, pyon_converted=True)`
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | **`===================== [End: 2 - Caller: 1] =====================`**
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` |   **`[1]`** Return Value: 
+<br>`17:36:15:830` |   	&emsp;`test(param=[test(param={'test': [10, 10]}, pyon_converted=True), 'asd'], pyon_converted=True)`
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | **`=========================== [End: 1] ===========================`**
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | **`======================= [Deep Serialize] =======================`**
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | **`========================== [Start: 1] ==========================`**
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` |   **`[1]`** Original obj input:
+<br>`17:36:15:830` |   	&emsp;`test(param=[test(param={'test': [10, 10]}, pyon_converted=True), 'asd'], pyon_converted=True)`
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:830` |   	&emsp;Value: `test(param=[test(param={'test': [10, 10]}, pyon_converted=True), 'asd'], pyon_converted=True)`, 
+<br>`17:36:15:830` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:830` | 
+<br>`17:36:15:830` |   **`[1]`** Iterability test:
+<br>`17:36:15:830` |   	&emsp;**Params:**
+<br>`17:36:15:830` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': [10, 10]}, pyon_converted=True), 'asd'], pyon_converted=True)`
+<br>`17:36:15:830` |   	&emsp;	&emsp;@Type: `<class 'zenyx.pyon.test'>`
+<br>`17:36:15:830` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`17:36:15:830` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:830` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:830` | 
+<br>`17:36:15:846` |   **`[1]`** Original Obj Iterability *(can be `False`)*:
+<br>`17:36:15:846` |   	&emsp;Object *(`obj`)*: `test(param=[test(param={'test': [10, 10]}, pyon_converted=True), 'asd'], pyon_converted=True)` 
+<br>`17:36:15:846` |   	&emsp;**Is object iterable**: `True`
+<br>`17:36:15:846` | 
+<br>`17:36:15:847` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:847` |   	&emsp;Value: `test(param=[test(param={'test': [10, 10]}, pyon_converted=True), 'asd'], pyon_converted=True)`, 
+<br>`17:36:15:847` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:847` | 
+<br>`17:36:15:848` |   **`[1]`** Iterability test:
+<br>`17:36:15:848` |   	&emsp;**Params:**
+<br>`17:36:15:848` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': [10, 10]}, pyon_converted=True), 'asd'], pyon_converted=True)`
+<br>`17:36:15:848` |   	&emsp;	&emsp;@Type: `<class 'zenyx.pyon.test'>`
+<br>`17:36:15:848` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`17:36:15:848` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:848` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:848` | 
+<br>`17:36:15:849` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:849` |   	&emsp;Value: `test(param=[test(param={'test': [10, 10]}, pyon_converted=True), 'asd'], pyon_converted=True)`, 
+<br>`17:36:15:849` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:849` | 
+<br>`17:36:15:851` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:851` |   	&emsp;Value: `test(param=[test(param={'test': [10, 10]}, pyon_converted=True), 'asd'], pyon_converted=True)`, 
+<br>`17:36:15:851` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:851` | 
+<br>`17:36:15:852` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:852` |   	&emsp;Value: `test(param=[test(param={'test': [10, 10]}, pyon_converted=True), 'asd'], pyon_converted=True)`, 
+<br>`17:36:15:852` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:852` | 
+<br>`17:36:15:853` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:853` |   	&emsp;Value: `[test(param={'test': [10, 10]}, pyon_converted=True), 'asd']`, 
+<br>`17:36:15:853` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:853` | 
+<br>`17:36:15:854` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:854` |   	&emsp;Value: `test(param={'test': [10, 10]}, pyon_converted=True)`, 
+<br>`17:36:15:854` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:854` | 
+<br>`17:36:15:855` |   **`[1]`** Iterability test:
+<br>`17:36:15:855` |   	&emsp;**Params:**
+<br>`17:36:15:855` |   	&emsp;	&emsp;Value: `test(param={'test': [10, 10]}, pyon_converted=True)`
+<br>`17:36:15:855` |   	&emsp;	&emsp;@Type: `<class 'zenyx.pyon.test'>`
+<br>`17:36:15:855` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`17:36:15:855` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:855` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:855` | 
+<br>`17:36:15:856` | 
+<br>`17:36:15:856` | **`================= [Deep Serialize - Caller: 1] =================`**
+<br>`17:36:15:856` | 
+<br>`17:36:15:856` | 
+<br>`17:36:15:857` | 
+<br>`17:36:15:857` | **`==================== [Start: 2 - Caller: 1] ====================`**
+<br>`17:36:15:857` | 
+<br>`17:36:15:857` | 
+<br>`17:36:15:858` |   **`[2]`** Original obj input:
+<br>`17:36:15:858` |   	&emsp;`test(param={'test': [10, 10]}, pyon_converted=True)`
+<br>`17:36:15:858` | 
+<br>`17:36:15:859` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:859` |   	&emsp;Value: `test(param={'test': [10, 10]}, pyon_converted=True)`, 
+<br>`17:36:15:859` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:859` | 
+<br>`17:36:15:860` |   **`[2]`** Iterability test:
+<br>`17:36:15:860` |   	&emsp;**Params:**
+<br>`17:36:15:860` |   	&emsp;	&emsp;Value: `test(param={'test': [10, 10]}, pyon_converted=True)`
+<br>`17:36:15:860` |   	&emsp;	&emsp;@Type: `<class 'zenyx.pyon.test'>`
+<br>`17:36:15:860` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`17:36:15:860` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:860` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:860` | 
+<br>`17:36:15:861` |   **`[2]`** Original Obj Iterability *(can be `False`)*:
+<br>`17:36:15:861` |   	&emsp;Object *(`obj`)*: `test(param={'test': [10, 10]}, pyon_converted=True)` 
+<br>`17:36:15:861` |   	&emsp;**Is object iterable**: `True`
+<br>`17:36:15:861` | 
+<br>`17:36:15:862` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:862` |   	&emsp;Value: `test(param={'test': [10, 10]}, pyon_converted=True)`, 
+<br>`17:36:15:862` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:862` | 
+<br>`17:36:15:863` |   **`[2]`** Iterability test:
+<br>`17:36:15:863` |   	&emsp;**Params:**
+<br>`17:36:15:863` |   	&emsp;	&emsp;Value: `test(param={'test': [10, 10]}, pyon_converted=True)`
+<br>`17:36:15:863` |   	&emsp;	&emsp;@Type: `<class 'zenyx.pyon.test'>`
+<br>`17:36:15:863` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`17:36:15:863` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:863` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:863` | 
+<br>`17:36:15:864` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:864` |   	&emsp;Value: `test(param={'test': [10, 10]}, pyon_converted=True)`, 
+<br>`17:36:15:864` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:864` | 
+<br>`17:36:15:865` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:865` |   	&emsp;Value: `test(param={'test': [10, 10]}, pyon_converted=True)`, 
+<br>`17:36:15:865` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:865` | 
+<br>`17:36:15:866` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:866` |   	&emsp;Value: `test(param={'test': [10, 10]}, pyon_converted=True)`, 
+<br>`17:36:15:866` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:866` | 
+<br>`17:36:15:867` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:867` |   	&emsp;Value: `{'test': [10, 10]}`, 
+<br>`17:36:15:867` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:867` | 
+<br>`17:36:15:869` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:869` |   	&emsp;Value: `{'test': [10, 10]}`, 
+<br>`17:36:15:869` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:869` | 
+<br>`17:36:15:869` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:869` |   	&emsp;Value: `[10, 10]`, 
+<br>`17:36:15:869` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:869` | 
+<br>`17:36:15:869` |   **`[2]`** Iterability test:
+<br>`17:36:15:869` |   	&emsp;**Params:**
+<br>`17:36:15:869` |   	&emsp;	&emsp;Value: `[10, 10]`
+<br>`17:36:15:869` |   	&emsp;	&emsp;@Type: `<class 'list'>`
+<br>`17:36:15:869` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:869` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`17:36:15:869` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:869` | 
+<br>`17:36:15:869` | 
+<br>`17:36:15:869` | **`================= [Deep Serialize - Caller: 2] =================`**
+<br>`17:36:15:869` | 
+<br>`17:36:15:869` | 
+<br>`17:36:15:869` | 
+<br>`17:36:15:869` | **`==================== [Start: 3 - Caller: 2] ====================`**
+<br>`17:36:15:869` | 
+<br>`17:36:15:869` | 
+<br>`17:36:15:869` |   **`[3]`** Original obj input:
+<br>`17:36:15:869` |   	&emsp;`[10, 10]`
+<br>`17:36:15:869` | 
+<br>`17:36:15:869` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:869` |   	&emsp;Value: `[10, 10]`, 
+<br>`17:36:15:869` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:869` | 
+<br>`17:36:15:869` |   **`[3]`** Iterability test:
+<br>`17:36:15:869` |   	&emsp;**Params:**
+<br>`17:36:15:869` |   	&emsp;	&emsp;Value: `[10, 10]`
+<br>`17:36:15:869` |   	&emsp;	&emsp;@Type: `<class 'list'>`
+<br>`17:36:15:869` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:869` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`17:36:15:869` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:869` | 
+<br>`17:36:15:869` |   **`[3]`** Original Obj Iterability *(can be `False`)*:
+<br>`17:36:15:869` |   	&emsp;Object *(`obj`)*: `[10, 10]` 
+<br>`17:36:15:869` |   	&emsp;**Is object iterable**: `True`
+<br>`17:36:15:869` | 
+<br>`17:36:15:869` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:869` |   	&emsp;Value: `[10, 10]`, 
+<br>`17:36:15:869` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:869` | 
+<br>`17:36:15:869` |   **`[3]`** Iterability test:
+<br>`17:36:15:869` |   	&emsp;**Params:**
+<br>`17:36:15:869` |   	&emsp;	&emsp;Value: `[10, 10]`
+<br>`17:36:15:869` |   	&emsp;	&emsp;@Type: `<class 'list'>`
+<br>`17:36:15:869` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:869` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`17:36:15:869` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:869` | 
+<br>`17:36:15:869` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:869` |   	&emsp;Value: `[10, 10]`, 
+<br>`17:36:15:869` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:869` | 
+<br>`17:36:15:880` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:880` |   	&emsp;Value: `[10, 10]`, 
+<br>`17:36:15:880` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:880` | 
+<br>`17:36:15:880` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:880` |   	&emsp;Value: `[10, 10]`, 
+<br>`17:36:15:880` |   	&emsp;Type(s): `<class 'tuple'>`
+<br>`17:36:15:880` | 
+<br>`17:36:15:880` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:880` |   	&emsp;Value: `[10, 10]`, 
+<br>`17:36:15:880` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:880` | 
+<br>`17:36:15:885` |   **`[3]`** Iterating List/Tuple:
+<br>`17:36:15:885` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
+<br>`17:36:15:885` |   	&emsp;Element: `10`
+<br>`17:36:15:885` | 
+<br>`17:36:15:885` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:885` |   	&emsp;Value: `10`, 
+<br>`17:36:15:885` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:885` | 
+<br>`17:36:15:885` |   **`[3]`** Iterability test:
+<br>`17:36:15:885` |   	&emsp;**Params:**
+<br>`17:36:15:885` |   	&emsp;	&emsp;Value: `10`
+<br>`17:36:15:885` |   	&emsp;	&emsp;@Type: `<class 'int'>`
+<br>`17:36:15:885` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:885` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:885` |   	&emsp;**Final Resoult**: `False`
+<br>`17:36:15:885` | 
+<br>`17:36:15:885` |   **`[3]`** Iterating List/Tuple:
+<br>`17:36:15:885` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
+<br>`17:36:15:885` |   	&emsp;Element: `10`
+<br>`17:36:15:885` | 
+<br>`17:36:15:885` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:885` |   	&emsp;Value: `10`, 
+<br>`17:36:15:885` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:885` | 
+<br>`17:36:15:885` |   **`[3]`** Iterability test:
+<br>`17:36:15:885` |   	&emsp;**Params:**
+<br>`17:36:15:885` |   	&emsp;	&emsp;Value: `10`
+<br>`17:36:15:885` |   	&emsp;	&emsp;@Type: `<class 'int'>`
+<br>`17:36:15:885` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:885` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:885` |   	&emsp;**Final Resoult**: `False`
+<br>`17:36:15:885` | 
+<br>`17:36:15:885` | 
+<br>`17:36:15:885` | **`========== [Early End: 3 - Caller: 2] List Serialized ==========`**
+<br>`17:36:15:885` | 
+<br>`17:36:15:885` | 
+<br>`17:36:15:885` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:885` |   	&emsp;Value: `True`, 
+<br>`17:36:15:885` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:885` | 
+<br>`17:36:15:885` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:885` |   	&emsp;Value: `True`, 
+<br>`17:36:15:885` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:885` | 
+<br>`17:36:15:885` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:885` |   	&emsp;Value: `test`, 
+<br>`17:36:15:885` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:885` | 
+<br>`17:36:15:885` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:885` |   	&emsp;Value: `test`, 
+<br>`17:36:15:885` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:885` | 
+<br>`17:36:15:885` |   **`[2]`** **New dict created:**
+<br>`17:36:15:885` |   	&emsp;`{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}`
+<br>`17:36:15:885` | 
+<br>`17:36:15:885` | 
+<br>`17:36:15:885` | **`===================== [End: 2 - Caller: 1] =====================`**
+<br>`17:36:15:885` | 
+<br>`17:36:15:885` | 
+<br>`17:36:15:885` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:885` |   	&emsp;Value: `asd`, 
+<br>`17:36:15:885` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:885` | 
+<br>`17:36:15:901` |   **`[1]`** Iterability test:
+<br>`17:36:15:901` |   	&emsp;**Params:**
+<br>`17:36:15:901` |   	&emsp;	&emsp;Value: `asd`
+<br>`17:36:15:901` |   	&emsp;	&emsp;@Type: `<class 'str'>`
+<br>`17:36:15:901` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:901` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:901` |   	&emsp;**Final Resoult**: `False`
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:901` |   	&emsp;Value: `[{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}, 'asd']`, 
+<br>`17:36:15:901` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:901` |   	&emsp;Value: `True`, 
+<br>`17:36:15:901` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:901` |   	&emsp;Value: `True`, 
+<br>`17:36:15:901` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:901` |   	&emsp;Value: `test`, 
+<br>`17:36:15:901` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:901` |   	&emsp;Value: `test`, 
+<br>`17:36:15:901` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` |   **`[1]`** **New dict created:**
+<br>`17:36:15:901` |   	&emsp;`{'param': [{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}, 'asd'], 'pyon_converted': True, 'PYON_TYPE': 'test'}`
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` | **`=========================== [End: 1] ===========================`**
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` | **`======================= [Deep Serialize] =======================`**
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` | **`========================== [Start: 1] ==========================`**
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` |   **`[1]`** Original obj input:
+<br>`17:36:15:901` |   	&emsp;`{'param': [{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}, 'asd'], 'pyon_converted': True, 'PYON_TYPE': 'test'}`
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:901` |   	&emsp;Value: `{'param': [{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}, 'asd'], 'pyon_converted': True, 'PYON_TYPE': 'test'}`, 
+<br>`17:36:15:901` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` |   **`[1]`** Iterability test:
+<br>`17:36:15:901` |   	&emsp;**Params:**
+<br>`17:36:15:901` |   	&emsp;	&emsp;Value: `{'param': [{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}, 'asd'], 'pyon_converted': True, 'PYON_TYPE': 'test'}`
+<br>`17:36:15:901` |   	&emsp;	&emsp;@Type: `<class 'dict'>`
+<br>`17:36:15:901` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:901` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`17:36:15:901` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:901` | 
+<br>`17:36:15:901` |   **`[1]`** Original Obj Iterability *(can be `False`)*:
+<br>`17:36:15:901` |   	&emsp;Object *(`obj`)*: `{'param': [{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}, 'asd'], 'pyon_converted': True, 'PYON_TYPE': 'test'}` 
+<br>`17:36:15:901` |   	&emsp;**Is object iterable**: `True`
+<br>`17:36:15:901` | 
+<br>`17:36:15:916` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:916` |   	&emsp;Value: `{'param': [{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}, 'asd'], 'pyon_converted': True, 'PYON_TYPE': 'test'}`, 
+<br>`17:36:15:916` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:916` | 
+<br>`17:36:15:916` |   **`[1]`** Iterability test:
+<br>`17:36:15:916` |   	&emsp;**Params:**
+<br>`17:36:15:916` |   	&emsp;	&emsp;Value: `{'param': [{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}, 'asd'], 'pyon_converted': True, 'PYON_TYPE': 'test'}`
+<br>`17:36:15:916` |   	&emsp;	&emsp;@Type: `<class 'dict'>`
+<br>`17:36:15:916` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:916` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`17:36:15:916` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:916` | 
+<br>`17:36:15:916` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:916` |   	&emsp;Value: `{'param': [{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}, 'asd'], 'pyon_converted': True, 'PYON_TYPE': 'test'}`, 
+<br>`17:36:15:916` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:916` | 
+<br>`17:36:15:916` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:916` |   	&emsp;Value: `{'param': [{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}, 'asd'], 'pyon_converted': True, 'PYON_TYPE': 'test'}`, 
+<br>`17:36:15:916` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:916` | 
+<br>`17:36:15:916` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:916` |   	&emsp;Value: `{'param': [{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}, 'asd'], 'pyon_converted': True, 'PYON_TYPE': 'test'}`, 
+<br>`17:36:15:916` |   	&emsp;Type(s): `<class 'tuple'>`
+<br>`17:36:15:916` | 
+<br>`17:36:15:916` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:916` |   	&emsp;Value: `{'param': [{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}, 'asd'], 'pyon_converted': True, 'PYON_TYPE': 'test'}`, 
+<br>`17:36:15:916` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:916` | 
+<br>`17:36:15:916` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:916` |   	&emsp;Value: `[{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}, 'asd']`, 
+<br>`17:36:15:916` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:916` | 
+<br>`17:36:15:916` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:916` |   	&emsp;Value: `{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}`, 
+<br>`17:36:15:916` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:916` | 
+<br>`17:36:15:916` |   **`[1]`** Iterability test:
+<br>`17:36:15:916` |   	&emsp;**Params:**
+<br>`17:36:15:916` |   	&emsp;	&emsp;Value: `{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}`
+<br>`17:36:15:916` |   	&emsp;	&emsp;@Type: `<class 'dict'>`
+<br>`17:36:15:916` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:916` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`17:36:15:916` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:916` | 
+<br>`17:36:15:916` | 
+<br>`17:36:15:916` | **`================= [Deep Serialize - Caller: 1] =================`**
+<br>`17:36:15:916` | 
+<br>`17:36:15:916` | 
+<br>`17:36:15:916` | 
+<br>`17:36:15:916` | **`==================== [Start: 2 - Caller: 1] ====================`**
+<br>`17:36:15:916` | 
+<br>`17:36:15:916` | 
+<br>`17:36:15:916` |   **`[2]`** Original obj input:
+<br>`17:36:15:916` |   	&emsp;`{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}`
+<br>`17:36:15:916` | 
+<br>`17:36:15:916` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:916` |   	&emsp;Value: `{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}`, 
+<br>`17:36:15:916` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:916` | 
+<br>`17:36:15:916` |   **`[2]`** Iterability test:
+<br>`17:36:15:916` |   	&emsp;**Params:**
+<br>`17:36:15:916` |   	&emsp;	&emsp;Value: `{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}`
+<br>`17:36:15:916` |   	&emsp;	&emsp;@Type: `<class 'dict'>`
+<br>`17:36:15:916` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:916` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`17:36:15:916` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:916` | 
+<br>`17:36:15:932` |   **`[2]`** Original Obj Iterability *(can be `False`)*:
+<br>`17:36:15:932` |   	&emsp;Object *(`obj`)*: `{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}` 
+<br>`17:36:15:932` |   	&emsp;**Is object iterable**: `True`
+<br>`17:36:15:932` | 
+<br>`17:36:15:932` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:932` |   	&emsp;Value: `{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}`, 
+<br>`17:36:15:932` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:932` | 
+<br>`17:36:15:932` |   **`[2]`** Iterability test:
+<br>`17:36:15:932` |   	&emsp;**Params:**
+<br>`17:36:15:932` |   	&emsp;	&emsp;Value: `{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}`
+<br>`17:36:15:932` |   	&emsp;	&emsp;@Type: `<class 'dict'>`
+<br>`17:36:15:932` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:932` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`17:36:15:932` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:932` | 
+<br>`17:36:15:932` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:932` |   	&emsp;Value: `{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}`, 
+<br>`17:36:15:932` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:932` | 
+<br>`17:36:15:932` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:932` |   	&emsp;Value: `{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}`, 
+<br>`17:36:15:932` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:932` | 
+<br>`17:36:15:932` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:932` |   	&emsp;Value: `{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}`, 
+<br>`17:36:15:932` |   	&emsp;Type(s): `<class 'tuple'>`
+<br>`17:36:15:932` | 
+<br>`17:36:15:932` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:932` |   	&emsp;Value: `{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}`, 
+<br>`17:36:15:932` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:932` | 
+<br>`17:36:15:932` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:932` |   	&emsp;Value: `{'test': [10, 10]}`, 
+<br>`17:36:15:932` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:932` | 
+<br>`17:36:15:932` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:932` |   	&emsp;Value: `{'test': [10, 10]}`, 
+<br>`17:36:15:932` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:932` | 
+<br>`17:36:15:932` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:932` |   	&emsp;Value: `[10, 10]`, 
+<br>`17:36:15:932` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:932` | 
+<br>`17:36:15:932` |   **`[2]`** Iterability test:
+<br>`17:36:15:932` |   	&emsp;**Params:**
+<br>`17:36:15:932` |   	&emsp;	&emsp;Value: `[10, 10]`
+<br>`17:36:15:932` |   	&emsp;	&emsp;@Type: `<class 'list'>`
+<br>`17:36:15:932` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:932` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`17:36:15:932` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:932` | 
+<br>`17:36:15:932` | 
+<br>`17:36:15:932` | **`================= [Deep Serialize - Caller: 2] =================`**
+<br>`17:36:15:932` | 
+<br>`17:36:15:932` | 
+<br>`17:36:15:932` | 
+<br>`17:36:15:932` | **`==================== [Start: 3 - Caller: 2] ====================`**
+<br>`17:36:15:932` | 
+<br>`17:36:15:932` | 
+<br>`17:36:15:932` |   **`[3]`** Original obj input:
+<br>`17:36:15:932` |   	&emsp;`[10, 10]`
+<br>`17:36:15:932` | 
+<br>`17:36:15:948` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:948` |   	&emsp;Value: `[10, 10]`, 
+<br>`17:36:15:948` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:948` | 
+<br>`17:36:15:948` |   **`[3]`** Iterability test:
+<br>`17:36:15:948` |   	&emsp;**Params:**
+<br>`17:36:15:948` |   	&emsp;	&emsp;Value: `[10, 10]`
+<br>`17:36:15:948` |   	&emsp;	&emsp;@Type: `<class 'list'>`
+<br>`17:36:15:948` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:948` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`17:36:15:948` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:948` | 
+<br>`17:36:15:948` |   **`[3]`** Original Obj Iterability *(can be `False`)*:
+<br>`17:36:15:948` |   	&emsp;Object *(`obj`)*: `[10, 10]` 
+<br>`17:36:15:948` |   	&emsp;**Is object iterable**: `True`
+<br>`17:36:15:948` | 
+<br>`17:36:15:948` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:948` |   	&emsp;Value: `[10, 10]`, 
+<br>`17:36:15:948` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:948` | 
+<br>`17:36:15:948` |   **`[3]`** Iterability test:
+<br>`17:36:15:948` |   	&emsp;**Params:**
+<br>`17:36:15:948` |   	&emsp;	&emsp;Value: `[10, 10]`
+<br>`17:36:15:948` |   	&emsp;	&emsp;@Type: `<class 'list'>`
+<br>`17:36:15:948` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:948` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`17:36:15:948` |   	&emsp;**Final Resoult**: `True`
+<br>`17:36:15:948` | 
+<br>`17:36:15:948` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:948` |   	&emsp;Value: `[10, 10]`, 
+<br>`17:36:15:948` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:948` | 
+<br>`17:36:15:948` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:948` |   	&emsp;Value: `[10, 10]`, 
+<br>`17:36:15:948` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:948` | 
+<br>`17:36:15:948` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:948` |   	&emsp;Value: `[10, 10]`, 
+<br>`17:36:15:948` |   	&emsp;Type(s): `<class 'tuple'>`
+<br>`17:36:15:948` | 
+<br>`17:36:15:948` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:948` |   	&emsp;Value: `[10, 10]`, 
+<br>`17:36:15:948` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:948` | 
+<br>`17:36:15:948` |   **`[3]`** Iterating List/Tuple:
+<br>`17:36:15:948` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
+<br>`17:36:15:948` |   	&emsp;Element: `10`
+<br>`17:36:15:948` | 
+<br>`17:36:15:948` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:948` |   	&emsp;Value: `10`, 
+<br>`17:36:15:948` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:948` | 
+<br>`17:36:15:948` |   **`[3]`** Iterability test:
+<br>`17:36:15:948` |   	&emsp;**Params:**
+<br>`17:36:15:948` |   	&emsp;	&emsp;Value: `10`
+<br>`17:36:15:948` |   	&emsp;	&emsp;@Type: `<class 'int'>`
+<br>`17:36:15:948` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:948` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:948` |   	&emsp;**Final Resoult**: `False`
+<br>`17:36:15:948` | 
+<br>`17:36:15:948` |   **`[3]`** Iterating List/Tuple:
+<br>`17:36:15:948` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
+<br>`17:36:15:948` |   	&emsp;Element: `10`
+<br>`17:36:15:948` | 
+<br>`17:36:15:963` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:963` |   	&emsp;Value: `10`, 
+<br>`17:36:15:963` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:963` | 
+<br>`17:36:15:963` |   **`[3]`** Iterability test:
+<br>`17:36:15:963` |   	&emsp;**Params:**
+<br>`17:36:15:963` |   	&emsp;	&emsp;Value: `10`
+<br>`17:36:15:963` |   	&emsp;	&emsp;@Type: `<class 'int'>`
+<br>`17:36:15:963` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:963` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:963` |   	&emsp;**Final Resoult**: `False`
+<br>`17:36:15:963` | 
+<br>`17:36:15:963` | 
+<br>`17:36:15:963` | **`========== [Early End: 3 - Caller: 2] List Serialized ==========`**
+<br>`17:36:15:963` | 
+<br>`17:36:15:963` | 
+<br>`17:36:15:963` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:963` |   	&emsp;Value: `True`, 
+<br>`17:36:15:963` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:963` | 
+<br>`17:36:15:963` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:963` |   	&emsp;Value: `True`, 
+<br>`17:36:15:963` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:963` | 
+<br>`17:36:15:963` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:963` |   	&emsp;Value: `test`, 
+<br>`17:36:15:963` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:963` | 
+<br>`17:36:15:963` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:963` |   	&emsp;Value: `test`, 
+<br>`17:36:15:963` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:963` | 
+<br>`17:36:15:963` |   **`[2]`** **New dict created:**
+<br>`17:36:15:963` |   	&emsp;`{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}`
+<br>`17:36:15:963` | 
+<br>`17:36:15:963` | 
+<br>`17:36:15:963` | **`===================== [End: 2 - Caller: 1] =====================`**
+<br>`17:36:15:963` | 
+<br>`17:36:15:963` | 
+<br>`17:36:15:963` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:963` |   	&emsp;Value: `asd`, 
+<br>`17:36:15:963` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`17:36:15:963` | 
+<br>`17:36:15:963` |   **`[1]`** Iterability test:
+<br>`17:36:15:963` |   	&emsp;**Params:**
+<br>`17:36:15:963` |   	&emsp;	&emsp;Value: `asd`
+<br>`17:36:15:963` |   	&emsp;	&emsp;@Type: `<class 'str'>`
+<br>`17:36:15:963` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`17:36:15:963` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`17:36:15:963` |   	&emsp;**Final Resoult**: `False`
+<br>`17:36:15:963` | 
+<br>`17:36:15:963` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:963` |   	&emsp;Value: `[{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}, 'asd']`, 
+<br>`17:36:15:963` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:963` | 
+<br>`17:36:15:963` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:963` |   	&emsp;Value: `True`, 
+<br>`17:36:15:963` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:963` | 
+<br>`17:36:15:963` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:963` |   	&emsp;Value: `True`, 
+<br>`17:36:15:963` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:963` | 
+<br>`17:36:15:979` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:979` |   	&emsp;Value: `test`, 
+<br>`17:36:15:979` |   	&emsp;Type(s): `<class 'list'>`
+<br>`17:36:15:979` | 
+<br>`17:36:15:981` |   **`[TypeCheck]`** Checking Type 
+<br>`17:36:15:981` |   	&emsp;Value: `test`, 
+<br>`17:36:15:981` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`17:36:15:981` | 
+<br>`17:36:15:981` |   **`[1]`** **New dict created:**
+<br>`17:36:15:981` |   	&emsp;`{'param': [{'param': {'test': [10, 10]}, 'pyon_converted': True, 'PYON_TYPE': 'test'}, 'asd'], 'pyon_converted': True, 'PYON_TYPE': 'test'}`
+<br>`17:36:15:981` | 
+<br>`17:36:15:981` | 
+<br>`17:36:15:981` | **`=========================== [End: 1] ===========================`**
+<br>`17:36:15:981` | 
+<br>`17:36:15:981` | 
+<br>`13:59:27:267` | 
+<br>`13:59:27:267` | **`======================= [Deep Serialize] =======================`**
+<br>`13:59:27:267` | 
+<br>`13:59:27:267` | 
+<br>`13:59:27:278` | 
+<br>`13:59:27:278` | **`========================== [Start: 1] ==========================`**
+<br>`13:59:27:278` | 
+<br>`13:59:27:278` | 
+<br>`13:59:27:278` |   **`[1]`** Original obj input:
+<br>`13:59:27:278` |   	&emsp;`test(param=[test(param={'test': (10, 10)}), 'asd'])`
+<br>`13:59:27:278` | 
+<br>`13:59:27:278` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:278` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`13:59:27:278` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:27:278` | 
+<br>`13:59:27:279` |   **`[1]`** Iterability test:
+<br>`13:59:27:279` |   	&emsp;**Params:**
+<br>`13:59:27:279` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`
+<br>`13:59:27:279` |   	&emsp;	&emsp;@Type: `<class 'tests.databank.test'>`
+<br>`13:59:27:279` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`13:59:27:279` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`13:59:27:279` |   	&emsp;**Final Resoult**: `True`
+<br>`13:59:27:279` | 
+<br>`13:59:27:279` |   **`[1]`** Original Obj Iterability *(can be `False`)*:
+<br>`13:59:27:279` |   	&emsp;Object *(`obj`)*: `test(param=[test(param={'test': (10, 10)}), 'asd'])` 
+<br>`13:59:27:279` |   	&emsp;**Is object iterable**: `True`
+<br>`13:59:27:279` | 
+<br>`13:59:27:279` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:279` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`13:59:27:279` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:27:279` | 
+<br>`13:59:27:279` |   **`[1]`** Iterability test:
+<br>`13:59:27:279` |   	&emsp;**Params:**
+<br>`13:59:27:279` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`
+<br>`13:59:27:279` |   	&emsp;	&emsp;@Type: `<class 'tests.databank.test'>`
+<br>`13:59:27:279` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`13:59:27:279` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`13:59:27:279` |   	&emsp;**Final Resoult**: `True`
+<br>`13:59:27:279` | 
+<br>`13:59:27:279` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:279` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`13:59:27:279` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:27:279` | 
+<br>`13:59:27:279` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:279` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`13:59:27:279` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:27:279` | 
+<br>`13:59:27:280` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:280` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`13:59:27:280` |   	&emsp;Type(s): `<class 'tuple'>`
+<br>`13:59:27:280` | 
+<br>`13:59:27:280` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:280` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`13:59:27:280` |   	&emsp;Type(s): `<class 'list'>`
+<br>`13:59:27:280` | 
+<br>`13:59:27:280` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:280` |   	&emsp;Value: `[test(param={'test': (10, 10)}), 'asd']`, 
+<br>`13:59:27:280` |   	&emsp;Type(s): `<class 'list'>`
+<br>`13:59:27:280` | 
+<br>`13:59:27:281` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:281` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`13:59:27:281` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:27:281` | 
+<br>`13:59:27:281` |   **`[1]`** Iterability test:
+<br>`13:59:27:281` |   	&emsp;**Params:**
+<br>`13:59:27:281` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
+<br>`13:59:27:281` |   	&emsp;	&emsp;@Type: `<class 'tests.databank.test'>`
+<br>`13:59:27:281` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`13:59:27:281` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`13:59:27:281` |   	&emsp;**Final Resoult**: `True`
+<br>`13:59:27:281` | 
+<br>`13:59:27:281` | 
+<br>`13:59:27:281` | **`================= [Deep Serialize - Caller: 1] =================`**
+<br>`13:59:27:281` | 
+<br>`13:59:27:281` | 
+<br>`13:59:27:281` | 
+<br>`13:59:27:281` | **`==================== [Start: 2 - Caller: 1] ====================`**
+<br>`13:59:27:281` | 
+<br>`13:59:27:281` | 
+<br>`13:59:27:281` |   **`[2]`** Original obj input:
+<br>`13:59:27:281` |   	&emsp;`test(param={'test': (10, 10)})`
+<br>`13:59:27:281` | 
+<br>`13:59:27:281` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:281` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`13:59:27:281` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:27:281` | 
+<br>`13:59:27:281` |   **`[2]`** Iterability test:
+<br>`13:59:27:281` |   	&emsp;**Params:**
+<br>`13:59:27:281` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
+<br>`13:59:27:281` |   	&emsp;	&emsp;@Type: `<class 'tests.databank.test'>`
+<br>`13:59:27:281` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`13:59:27:281` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`13:59:27:281` |   	&emsp;**Final Resoult**: `True`
+<br>`13:59:27:281` | 
+<br>`13:59:27:282` |   **`[2]`** Original Obj Iterability *(can be `False`)*:
+<br>`13:59:27:282` |   	&emsp;Object *(`obj`)*: `test(param={'test': (10, 10)})` 
+<br>`13:59:27:282` |   	&emsp;**Is object iterable**: `True`
+<br>`13:59:27:282` | 
+<br>`13:59:27:282` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:282` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`13:59:27:282` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:27:282` | 
+<br>`13:59:27:282` |   **`[2]`** Iterability test:
+<br>`13:59:27:282` |   	&emsp;**Params:**
+<br>`13:59:27:282` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
+<br>`13:59:27:282` |   	&emsp;	&emsp;@Type: `<class 'tests.databank.test'>`
+<br>`13:59:27:282` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`13:59:27:282` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`13:59:27:282` |   	&emsp;**Final Resoult**: `True`
+<br>`13:59:27:282` | 
+<br>`13:59:27:282` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:282` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`13:59:27:282` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:27:282` | 
+<br>`13:59:27:282` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:282` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`13:59:27:282` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:27:282` | 
+<br>`13:59:27:283` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:283` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`13:59:27:283` |   	&emsp;Type(s): `<class 'tuple'>`
+<br>`13:59:27:283` | 
+<br>`13:59:27:283` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:283` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`13:59:27:283` |   	&emsp;Type(s): `<class 'list'>`
+<br>`13:59:27:283` | 
+<br>`13:59:27:283` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:283` |   	&emsp;Value: `{'test': (10, 10)}`, 
+<br>`13:59:27:283` |   	&emsp;Type(s): `<class 'list'>`
+<br>`13:59:27:283` | 
+<br>`13:59:27:283` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:283` |   	&emsp;Value: `{'test': (10, 10)}`, 
+<br>`13:59:27:283` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:27:283` | 
+<br>`13:59:27:283` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:283` |   	&emsp;Value: `(10, 10)`, 
+<br>`13:59:27:283` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:27:283` | 
+<br>`13:59:27:283` |   **`[2]`** Iterability test:
+<br>`13:59:27:283` |   	&emsp;**Params:**
+<br>`13:59:27:283` |   	&emsp;	&emsp;Value: `(10, 10)`
+<br>`13:59:27:283` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
+<br>`13:59:27:283` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`13:59:27:283` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`13:59:27:283` |   	&emsp;**Final Resoult**: `True`
+<br>`13:59:27:283` | 
+<br>`13:59:27:283` | 
+<br>`13:59:27:283` | **`================= [Deep Serialize - Caller: 2] =================`**
+<br>`13:59:27:283` | 
+<br>`13:59:27:283` | 
+<br>`13:59:27:284` | 
+<br>`13:59:27:284` | **`==================== [Start: 3 - Caller: 2] ====================`**
+<br>`13:59:27:284` | 
+<br>`13:59:27:284` | 
+<br>`13:59:27:284` |   **`[3]`** Original obj input:
+<br>`13:59:27:284` |   	&emsp;`(10, 10)`
+<br>`13:59:27:284` | 
+<br>`13:59:27:284` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:284` |   	&emsp;Value: `(10, 10)`, 
+<br>`13:59:27:284` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:27:284` | 
+<br>`13:59:27:284` |   **`[3]`** Iterability test:
+<br>`13:59:27:284` |   	&emsp;**Params:**
+<br>`13:59:27:284` |   	&emsp;	&emsp;Value: `(10, 10)`
+<br>`13:59:27:284` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
+<br>`13:59:27:284` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`13:59:27:284` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`13:59:27:284` |   	&emsp;**Final Resoult**: `True`
+<br>`13:59:27:284` | 
+<br>`13:59:27:284` |   **`[3]`** Original Obj Iterability *(can be `False`)*:
+<br>`13:59:27:284` |   	&emsp;Object *(`obj`)*: `(10, 10)` 
+<br>`13:59:27:284` |   	&emsp;**Is object iterable**: `True`
+<br>`13:59:27:284` | 
+<br>`13:59:27:284` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:284` |   	&emsp;Value: `(10, 10)`, 
+<br>`13:59:27:284` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:27:284` | 
+<br>`13:59:27:284` |   **`[3]`** Iterability test:
+<br>`13:59:27:284` |   	&emsp;**Params:**
+<br>`13:59:27:284` |   	&emsp;	&emsp;Value: `(10, 10)`
+<br>`13:59:27:284` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
+<br>`13:59:27:284` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`13:59:27:284` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`13:59:27:284` |   	&emsp;**Final Resoult**: `True`
+<br>`13:59:27:284` | 
+<br>`13:59:27:285` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:285` |   	&emsp;Value: `(10, 10)`, 
+<br>`13:59:27:285` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:27:285` | 
+<br>`13:59:27:285` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:285` |   	&emsp;Value: `(10, 10)`, 
+<br>`13:59:27:285` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:27:285` | 
+<br>`13:59:27:285` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:285` |   	&emsp;Value: `(10, 10)`, 
+<br>`13:59:27:285` |   	&emsp;Type(s): `<class 'tuple'>`
+<br>`13:59:27:285` | 
+<br>`13:59:27:285` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:285` |   	&emsp;Value: `[10, 10]`, 
+<br>`13:59:27:285` |   	&emsp;Type(s): `<class 'list'>`
+<br>`13:59:27:285` | 
+<br>`13:59:27:285` |   **`[3]`** Iterating List/Tuple:
+<br>`13:59:27:285` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
+<br>`13:59:27:285` |   	&emsp;Element: `10`
+<br>`13:59:27:285` | 
+<br>`13:59:27:285` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:285` |   	&emsp;Value: `10`, 
+<br>`13:59:27:285` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:27:285` | 
+<br>`13:59:27:285` |   **`[3]`** Iterability test:
+<br>`13:59:27:285` |   	&emsp;**Params:**
+<br>`13:59:27:285` |   	&emsp;	&emsp;Value: `10`
+<br>`13:59:27:285` |   	&emsp;	&emsp;@Type: `<class 'int'>`
+<br>`13:59:27:285` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`13:59:27:285` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`13:59:27:285` |   	&emsp;**Final Resoult**: `False`
+<br>`13:59:27:285` | 
+<br>`13:59:27:286` |   **`[3]`** Iterating List/Tuple:
+<br>`13:59:27:286` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
+<br>`13:59:27:286` |   	&emsp;Element: `10`
+<br>`13:59:27:286` | 
+<br>`13:59:27:286` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:286` |   	&emsp;Value: `10`, 
+<br>`13:59:27:286` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:27:286` | 
+<br>`13:59:27:286` |   **`[3]`** Iterability test:
+<br>`13:59:27:286` |   	&emsp;**Params:**
+<br>`13:59:27:286` |   	&emsp;	&emsp;Value: `10`
+<br>`13:59:27:286` |   	&emsp;	&emsp;@Type: `<class 'int'>`
+<br>`13:59:27:286` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`13:59:27:286` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`13:59:27:286` |   	&emsp;**Final Resoult**: `False`
+<br>`13:59:27:286` | 
+<br>`13:59:27:286` | 
+<br>`13:59:27:286` | **`========== [Early End: 3 - Caller: 2] List Serialized ==========`**
+<br>`13:59:27:286` | 
+<br>`13:59:27:286` | 
+<br>`13:59:27:286` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:286` |   	&emsp;Value: `test`, 
+<br>`13:59:27:286` |   	&emsp;Type(s): `<class 'list'>`
+<br>`13:59:27:286` | 
+<br>`13:59:27:286` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:286` |   	&emsp;Value: `test`, 
+<br>`13:59:27:286` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:27:286` | 
+<br>`13:59:27:286` |   **`[2]`** **New dict created:**
+<br>`13:59:27:286` |   	&emsp;`{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}`
+<br>`13:59:27:286` | 
+<br>`13:59:27:286` | 
+<br>`13:59:27:286` | **`===================== [End: 2 - Caller: 1] =====================`**
+<br>`13:59:27:286` | 
+<br>`13:59:27:286` | 
+<br>`13:59:27:287` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:287` |   	&emsp;Value: `asd`, 
+<br>`13:59:27:287` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:27:287` | 
+<br>`13:59:27:287` |   **`[1]`** Iterability test:
+<br>`13:59:27:287` |   	&emsp;**Params:**
+<br>`13:59:27:287` |   	&emsp;	&emsp;Value: `asd`
+<br>`13:59:27:287` |   	&emsp;	&emsp;@Type: `<class 'str'>`
+<br>`13:59:27:287` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`13:59:27:287` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`13:59:27:287` |   	&emsp;**Final Resoult**: `False`
+<br>`13:59:27:287` | 
+<br>`13:59:27:287` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:287` |   	&emsp;Value: `[{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}, 'asd']`, 
+<br>`13:59:27:287` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:27:287` | 
+<br>`13:59:27:287` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:287` |   	&emsp;Value: `test`, 
+<br>`13:59:27:287` |   	&emsp;Type(s): `<class 'list'>`
+<br>`13:59:27:287` | 
+<br>`13:59:27:287` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:27:287` |   	&emsp;Value: `test`, 
+<br>`13:59:27:287` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:27:287` | 
+<br>`13:59:27:287` |   **`[1]`** **New dict created:**
+<br>`13:59:27:287` |   	&emsp;`{'param': [{'param': {'test': [10, 10]}, 'PYON_TYPE': 'test'}, 'asd'], 'PYON_TYPE': 'test'}`
+<br>`13:59:27:287` | 
+<br>`13:59:27:288` | 
+<br>`13:59:27:288` | **`=========================== [End: 1] ===========================`**
+<br>`13:59:27:288` | 
+<br>`13:59:27:288` | 
+<br>`13:59:35:810` | 
+<br>`13:59:35:810` | **`======================= [Deep Serialize] =======================`**
+<br>`13:59:35:810` | 
+<br>`13:59:35:810` | 
+<br>`13:59:35:810` | 
+<br>`13:59:35:810` | **`========================== [Start: 1] ==========================`**
+<br>`13:59:35:810` | 
+<br>`13:59:35:810` | 
+<br>`13:59:35:810` |   **`[1]`** Original obj input:
+<br>`13:59:35:810` |   	&emsp;`test(param=[test(param={'test': (10, 10)}), 'asd'])`
+<br>`13:59:35:810` | 
+<br>`13:59:35:810` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:810` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`13:59:35:810` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:35:810` | 
+<br>`13:59:35:811` |   **`[1]`** Iterability test:
+<br>`13:59:35:811` |   	&emsp;**Params:**
+<br>`13:59:35:811` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`
+<br>`13:59:35:811` |   	&emsp;	&emsp;@Type: `<class 'tests.databank.test'>`
+<br>`13:59:35:811` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`13:59:35:811` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`13:59:35:811` |   	&emsp;**Final Resoult**: `True`
+<br>`13:59:35:811` | 
+<br>`13:59:35:811` |   **`[1]`** Original Obj Iterability *(can be `False`)*:
+<br>`13:59:35:811` |   	&emsp;Object *(`obj`)*: `test(param=[test(param={'test': (10, 10)}), 'asd'])` 
+<br>`13:59:35:811` |   	&emsp;**Is object iterable**: `True`
+<br>`13:59:35:811` | 
+<br>`13:59:35:811` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:811` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`13:59:35:811` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:35:811` | 
+<br>`13:59:35:811` |   **`[1]`** Iterability test:
+<br>`13:59:35:811` |   	&emsp;**Params:**
+<br>`13:59:35:811` |   	&emsp;	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`
+<br>`13:59:35:811` |   	&emsp;	&emsp;@Type: `<class 'tests.databank.test'>`
+<br>`13:59:35:811` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`13:59:35:811` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`13:59:35:811` |   	&emsp;**Final Resoult**: `True`
+<br>`13:59:35:811` | 
+<br>`13:59:35:811` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:811` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`13:59:35:811` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:35:811` | 
+<br>`13:59:35:811` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:811` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`13:59:35:811` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:35:811` | 
+<br>`13:59:35:811` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:811` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`13:59:35:811` |   	&emsp;Type(s): `<class 'tuple'>`
+<br>`13:59:35:811` | 
+<br>`13:59:35:812` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:812` |   	&emsp;Value: `test(param=[test(param={'test': (10, 10)}), 'asd'])`, 
+<br>`13:59:35:812` |   	&emsp;Type(s): `<class 'list'>`
+<br>`13:59:35:812` | 
+<br>`13:59:35:812` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:812` |   	&emsp;Value: `[test(param={'test': (10, 10)}), 'asd']`, 
+<br>`13:59:35:812` |   	&emsp;Type(s): `<class 'list'>`
+<br>`13:59:35:812` | 
+<br>`13:59:35:812` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:812` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`13:59:35:812` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:35:812` | 
+<br>`13:59:35:812` |   **`[1]`** Iterability test:
+<br>`13:59:35:812` |   	&emsp;**Params:**
+<br>`13:59:35:812` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
+<br>`13:59:35:812` |   	&emsp;	&emsp;@Type: `<class 'tests.databank.test'>`
+<br>`13:59:35:812` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`13:59:35:812` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`13:59:35:812` |   	&emsp;**Final Resoult**: `True`
+<br>`13:59:35:812` | 
+<br>`13:59:35:813` | 
+<br>`13:59:35:813` | **`================= [Deep Serialize - Caller: 1] =================`**
+<br>`13:59:35:813` | 
+<br>`13:59:35:813` | 
+<br>`13:59:35:813` | 
+<br>`13:59:35:813` | **`==================== [Start: 2 - Caller: 1] ====================`**
+<br>`13:59:35:813` | 
+<br>`13:59:35:813` | 
+<br>`13:59:35:813` |   **`[2]`** Original obj input:
+<br>`13:59:35:813` |   	&emsp;`test(param={'test': (10, 10)})`
+<br>`13:59:35:813` | 
+<br>`13:59:35:813` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:813` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`13:59:35:813` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:35:813` | 
+<br>`13:59:35:813` |   **`[2]`** Iterability test:
+<br>`13:59:35:813` |   	&emsp;**Params:**
+<br>`13:59:35:813` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
+<br>`13:59:35:813` |   	&emsp;	&emsp;@Type: `<class 'tests.databank.test'>`
+<br>`13:59:35:813` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`13:59:35:813` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`13:59:35:813` |   	&emsp;**Final Resoult**: `True`
+<br>`13:59:35:813` | 
+<br>`13:59:35:814` |   **`[2]`** Original Obj Iterability *(can be `False`)*:
+<br>`13:59:35:814` |   	&emsp;Object *(`obj`)*: `test(param={'test': (10, 10)})` 
+<br>`13:59:35:814` |   	&emsp;**Is object iterable**: `True`
+<br>`13:59:35:814` | 
+<br>`13:59:35:814` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:814` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`13:59:35:814` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:35:814` | 
+<br>`13:59:35:814` |   **`[2]`** Iterability test:
+<br>`13:59:35:814` |   	&emsp;**Params:**
+<br>`13:59:35:814` |   	&emsp;	&emsp;Value: `test(param={'test': (10, 10)})`
+<br>`13:59:35:814` |   	&emsp;	&emsp;@Type: `<class 'tests.databank.test'>`
+<br>`13:59:35:814` |   	&emsp;Is object *(`__is_object`)*: `True`
+<br>`13:59:35:814` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`13:59:35:814` |   	&emsp;**Final Resoult**: `True`
+<br>`13:59:35:814` | 
+<br>`13:59:35:814` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:814` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`13:59:35:814` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:35:814` | 
+<br>`13:59:35:814` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:814` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`13:59:35:814` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:35:814` | 
+<br>`13:59:35:814` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:814` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`13:59:35:814` |   	&emsp;Type(s): `<class 'tuple'>`
+<br>`13:59:35:814` | 
+<br>`13:59:35:815` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:815` |   	&emsp;Value: `test(param={'test': (10, 10)})`, 
+<br>`13:59:35:815` |   	&emsp;Type(s): `<class 'list'>`
+<br>`13:59:35:815` | 
+<br>`13:59:35:815` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:815` |   	&emsp;Value: `{'test': (10, 10)}`, 
+<br>`13:59:35:815` |   	&emsp;Type(s): `<class 'list'>`
+<br>`13:59:35:815` | 
+<br>`13:59:35:815` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:815` |   	&emsp;Value: `{'test': (10, 10)}`, 
+<br>`13:59:35:815` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:35:815` | 
+<br>`13:59:35:815` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:815` |   	&emsp;Value: `(10, 10)`, 
+<br>`13:59:35:815` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:35:815` | 
+<br>`13:59:35:815` |   **`[2]`** Iterability test:
+<br>`13:59:35:815` |   	&emsp;**Params:**
+<br>`13:59:35:815` |   	&emsp;	&emsp;Value: `(10, 10)`
+<br>`13:59:35:815` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
+<br>`13:59:35:815` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`13:59:35:815` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`13:59:35:815` |   	&emsp;**Final Resoult**: `True`
+<br>`13:59:35:815` | 
+<br>`13:59:35:815` | 
+<br>`13:59:35:815` | **`================= [Deep Serialize - Caller: 2] =================`**
+<br>`13:59:35:815` | 
+<br>`13:59:35:815` | 
+<br>`13:59:35:816` | 
+<br>`13:59:35:816` | **`==================== [Start: 3 - Caller: 2] ====================`**
+<br>`13:59:35:816` | 
+<br>`13:59:35:816` | 
+<br>`13:59:35:816` |   **`[3]`** Original obj input:
+<br>`13:59:35:816` |   	&emsp;`(10, 10)`
+<br>`13:59:35:816` | 
+<br>`13:59:35:816` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:816` |   	&emsp;Value: `(10, 10)`, 
+<br>`13:59:35:816` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:35:816` | 
+<br>`13:59:35:816` |   **`[3]`** Iterability test:
+<br>`13:59:35:816` |   	&emsp;**Params:**
+<br>`13:59:35:816` |   	&emsp;	&emsp;Value: `(10, 10)`
+<br>`13:59:35:816` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
+<br>`13:59:35:816` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`13:59:35:816` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`13:59:35:816` |   	&emsp;**Final Resoult**: `True`
+<br>`13:59:35:816` | 
+<br>`13:59:35:816` |   **`[3]`** Original Obj Iterability *(can be `False`)*:
+<br>`13:59:35:816` |   	&emsp;Object *(`obj`)*: `(10, 10)` 
+<br>`13:59:35:816` |   	&emsp;**Is object iterable**: `True`
+<br>`13:59:35:816` | 
+<br>`13:59:35:817` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:817` |   	&emsp;Value: `(10, 10)`, 
+<br>`13:59:35:817` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:35:817` | 
+<br>`13:59:35:817` |   **`[3]`** Iterability test:
+<br>`13:59:35:817` |   	&emsp;**Params:**
+<br>`13:59:35:817` |   	&emsp;	&emsp;Value: `(10, 10)`
+<br>`13:59:35:817` |   	&emsp;	&emsp;@Type: `<class 'tuple'>`
+<br>`13:59:35:817` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`13:59:35:817` |   	&emsp;Is dict/list/tuple *(`test1`)*: `True`
+<br>`13:59:35:817` |   	&emsp;**Final Resoult**: `True`
+<br>`13:59:35:817` | 
+<br>`13:59:35:817` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:817` |   	&emsp;Value: `(10, 10)`, 
+<br>`13:59:35:817` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:35:817` | 
+<br>`13:59:35:817` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:817` |   	&emsp;Value: `(10, 10)`, 
+<br>`13:59:35:817` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:35:817` | 
+<br>`13:59:35:817` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:817` |   	&emsp;Value: `(10, 10)`, 
+<br>`13:59:35:817` |   	&emsp;Type(s): `<class 'tuple'>`
+<br>`13:59:35:817` | 
+<br>`13:59:35:818` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:818` |   	&emsp;Value: `[10, 10]`, 
+<br>`13:59:35:818` |   	&emsp;Type(s): `<class 'list'>`
+<br>`13:59:35:818` | 
+<br>`13:59:35:818` |   **`[3]`** Iterating List/Tuple:
+<br>`13:59:35:818` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
+<br>`13:59:35:818` |   	&emsp;Element: `10`
+<br>`13:59:35:818` | 
+<br>`13:59:35:818` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:818` |   	&emsp;Value: `10`, 
+<br>`13:59:35:818` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:35:818` | 
+<br>`13:59:35:818` |   **`[3]`** Iterability test:
+<br>`13:59:35:818` |   	&emsp;**Params:**
+<br>`13:59:35:818` |   	&emsp;	&emsp;Value: `10`
+<br>`13:59:35:818` |   	&emsp;	&emsp;@Type: `<class 'int'>`
+<br>`13:59:35:818` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`13:59:35:818` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`13:59:35:818` |   	&emsp;**Final Resoult**: `False`
+<br>`13:59:35:818` | 
+<br>`13:59:35:818` |   **`[3]`** Iterating List/Tuple:
+<br>`13:59:35:818` |   	&emsp;List/Tuple *(`obj`)*: `[10, 10]`
+<br>`13:59:35:818` |   	&emsp;Element: `10`
+<br>`13:59:35:818` | 
+<br>`13:59:35:818` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:818` |   	&emsp;Value: `10`, 
+<br>`13:59:35:818` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:35:818` | 
+<br>`13:59:35:819` |   **`[3]`** Iterability test:
+<br>`13:59:35:819` |   	&emsp;**Params:**
+<br>`13:59:35:819` |   	&emsp;	&emsp;Value: `10`
+<br>`13:59:35:819` |   	&emsp;	&emsp;@Type: `<class 'int'>`
+<br>`13:59:35:819` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`13:59:35:819` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`13:59:35:819` |   	&emsp;**Final Resoult**: `False`
+<br>`13:59:35:819` | 
+<br>`13:59:35:819` | 
+<br>`13:59:35:819` | **`========== [Early End: 3 - Caller: 2] List Serialized ==========`**
+<br>`13:59:35:819` | 
+<br>`13:59:35:819` | 
+<br>`13:59:35:819` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:819` |   	&emsp;Value: `test`, 
+<br>`13:59:35:819` |   	&emsp;Type(s): `<class 'list'>`
+<br>`13:59:35:819` | 
+<br>`13:59:35:819` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:819` |   	&emsp;Value: `test`, 
+<br>`13:59:35:819` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:35:819` | 
+<br>`13:59:35:819` |   **`[2]`** **New dict created:**
+<br>`13:59:35:819` |   	&emsp;`{'param': {'test': [10, 10]}, '@class': 'test'}`
+<br>`13:59:35:819` | 
+<br>`13:59:35:819` | 
+<br>`13:59:35:819` | **`===================== [End: 2 - Caller: 1] =====================`**
+<br>`13:59:35:819` | 
+<br>`13:59:35:819` | 
+<br>`13:59:35:819` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:819` |   	&emsp;Value: `asd`, 
+<br>`13:59:35:819` |   	&emsp;Type(s): `(<class 'dict'>, <class 'list'>, <class 'tuple'>)`
+<br>`13:59:35:819` | 
+<br>`13:59:35:819` |   **`[1]`** Iterability test:
+<br>`13:59:35:819` |   	&emsp;**Params:**
+<br>`13:59:35:819` |   	&emsp;	&emsp;Value: `asd`
+<br>`13:59:35:819` |   	&emsp;	&emsp;@Type: `<class 'str'>`
+<br>`13:59:35:819` |   	&emsp;Is object *(`__is_object`)*: `False`
+<br>`13:59:35:819` |   	&emsp;Is dict/list/tuple *(`test1`)*: `False`
+<br>`13:59:35:819` |   	&emsp;**Final Resoult**: `False`
+<br>`13:59:35:819` | 
+<br>`13:59:35:820` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:820` |   	&emsp;Value: `[{'param': {'test': [10, 10]}, '@class': 'test'}, 'asd']`, 
+<br>`13:59:35:820` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:35:820` | 
+<br>`13:59:35:820` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:820` |   	&emsp;Value: `test`, 
+<br>`13:59:35:820` |   	&emsp;Type(s): `<class 'list'>`
+<br>`13:59:35:820` | 
+<br>`13:59:35:820` |   **`[TypeCheck]`** Checking Type 
+<br>`13:59:35:820` |   	&emsp;Value: `test`, 
+<br>`13:59:35:820` |   	&emsp;Type(s): `<class 'dict'>`
+<br>`13:59:35:820` | 
+<br>`13:59:35:820` |   **`[1]`** **New dict created:**
+<br>`13:59:35:820` |   	&emsp;`{'param': [{'param': {'test': [10, 10]}, '@class': 'test'}, 'asd'], '@class': 'test'}`
+<br>`13:59:35:820` | 
+<br>`13:59:35:821` | 
+<br>`13:59:35:821` | **`=========================== [End: 1] ===========================`**
+<br>`13:59:35:821` | 
+<br>`13:59:35:821` |
```

### Comparing `zenyx-1.3.2/LICENSE` & `zenyx-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zenyx-1.3.2/pyproject.toml` & `zenyx-2.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zenyx"
-version = "1.3.2"
+version = "2.1.0"
 authors = [
   { name="zewenn", email="zc.fallens@gamil.com" },
 ]
 description = "A multitool python object notation package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `zenyx-1.3.2/PKG-INFO` & `zenyx-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: zenyx
-Version: 1.3.2
+Version: 2.1.0
 Summary: A multitool python object notation package
 Project-URL: Homepage, https://github.com/zewenn/zenyx
 Project-URL: Issues, https://github.com/zewenn/zenyx/issues
 Author-email: zewenn <zc.fallens@gamil.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


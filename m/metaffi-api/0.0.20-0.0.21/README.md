# Comparing `tmp/metaffi_api-0.0.20.tar.gz` & `tmp/metaffi_api-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaffi_api-0.0.20.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "metaffi_api-0.0.21.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `metaffi_api-0.0.20.tar` & `metaffi_api-0.0.21.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      205 2024-04-15 06:15:13.341334 metaffi_api-0.0.20/CMakeLists.txt
--rw-r--r--   0        0        0     1096 2022-05-28 09:56:58.251104 metaffi_api-0.0.20/LICENSE
--rw-r--r--   0        0        0       57 2024-01-18 12:19:08.787247 metaffi_api-0.0.20/README.md
--rw-r--r--   0        0        0      428 2024-04-21 09:02:34.475590 metaffi_api-0.0.20/metaffi/__init__.py
--rw-r--r--   0        0        0     1270 2024-02-04 18:44:32.014120 metaffi_api-0.0.20/metaffi/classes_metaffi.puml
--rw-r--r--   0        0        0      122 2024-01-01 14:18:03.539263 metaffi_api-0.0.20/metaffi/metaffi_handle.py
--rw-r--r--   0        0        0     4920 2024-04-21 08:50:29.056725 metaffi_api-0.0.20/metaffi/metaffi_module.py
--rw-r--r--   0        0        0      513 2024-01-01 16:45:39.723929 metaffi_api-0.0.20/metaffi/metaffi_runtime.py
--rw-r--r--   0        0        0     4642 2024-04-21 08:59:16.278139 metaffi_api-0.0.20/metaffi/metaffi_types.py
--rw-r--r--   0        0        0     1471 2024-03-21 09:19:16.794164 metaffi_api-0.0.20/metaffi/pycdts_converter.py
--rw-r--r--   0        0        0     4712 2024-04-21 09:02:26.437120 metaffi_api-0.0.20/metaffi/xllr_wrapper.py
--rw-r--r--   0        0        0      584 2024-04-21 09:03:09.582637 metaffi_api-0.0.20/publish.ps1
--rw-r--r--   0        0        0      535 2024-03-08 20:55:47.528284 metaffi_api-0.0.20/pyproject.toml
--rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 metaffi_api-0.0.20/PKG-INFO
+-rw-r--r--   0        0        0      205 2024-04-15 06:15:13.341334 metaffi_api-0.0.21/CMakeLists.txt
+-rw-r--r--   0        0        0     1096 2022-05-28 09:56:58.251104 metaffi_api-0.0.21/LICENSE
+-rw-r--r--   0        0        0       57 2024-01-18 12:19:08.787247 metaffi_api-0.0.21/README.md
+-rw-r--r--   0        0        0      428 2024-04-21 10:04:11.140239 metaffi_api-0.0.21/metaffi/__init__.py
+-rw-r--r--   0        0        0     1270 2024-02-04 18:44:32.014120 metaffi_api-0.0.21/metaffi/classes_metaffi.puml
+-rw-r--r--   0        0        0      122 2024-01-01 14:18:03.539263 metaffi_api-0.0.21/metaffi/metaffi_handle.py
+-rw-r--r--   0        0        0     5202 2024-04-21 10:03:30.859401 metaffi_api-0.0.21/metaffi/metaffi_module.py
+-rw-r--r--   0        0        0      513 2024-01-01 16:45:39.723929 metaffi_api-0.0.21/metaffi/metaffi_runtime.py
+-rw-r--r--   0        0        0     4642 2024-04-21 08:59:16.278139 metaffi_api-0.0.21/metaffi/metaffi_types.py
+-rw-r--r--   0        0        0     1471 2024-03-21 09:19:16.794164 metaffi_api-0.0.21/metaffi/pycdts_converter.py
+-rw-r--r--   0        0        0     4712 2024-04-21 09:02:26.437120 metaffi_api-0.0.21/metaffi/xllr_wrapper.py
+-rw-r--r--   0        0        0      584 2024-04-21 09:03:09.582637 metaffi_api-0.0.21/publish.ps1
+-rw-r--r--   0        0        0      535 2024-03-08 20:55:47.528284 metaffi_api-0.0.21/pyproject.toml
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 metaffi_api-0.0.21/PKG-INFO
```

### Comparing `metaffi_api-0.0.20/LICENSE` & `metaffi_api-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.20/metaffi/classes_metaffi.puml` & `metaffi_api-0.0.21/metaffi/classes_metaffi.puml`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.20/metaffi/metaffi_module.py` & `metaffi_api-0.0.21/metaffi/metaffi_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,36 +50,39 @@
 
 class MetaFFIModule:
 	def __init__(self, runtime: metaffi.metaffi_runtime.MetaFFIRuntime, xllr: metaffi.xllr_wrapper._XllrWrapper, module_path: str):
 		self.runtime = runtime
 		self.xllr = xllr
 		self.module_path = module_path
 	
-	def load(self, function_path: str, params_metaffi_types: Tuple[metaffi.metaffi_types.metaffi_type_info] | None,
-			retval_metaffi_types: Tuple[metaffi.metaffi_types.metaffi_type_info] | None) -> Callable[..., Tuple[Any, ...]]:
+	def load(self, function_path: str, params_metaffi_types: List[metaffi.metaffi_types.metaffi_type_info] | None,
+			retval_metaffi_types: List[metaffi.metaffi_types.metaffi_type_info] | None) -> Callable[..., Tuple[Any, ...]]:
 		
 		if params_metaffi_types is None:
 			params_metaffi_types = tuple()
 		
 		if retval_metaffi_types is None:
 			retval_metaffi_types = tuple()
 		
 		# Create ctypes arrays for params_metaffi_types and retval_metaffi_types
 		ParamsArray = metaffi.metaffi_types.metaffi_type_info * len(params_metaffi_types)
 		params_array = ParamsArray(*params_metaffi_types)
 		
 		RetvalArray = metaffi.metaffi_types.metaffi_type_info * len(retval_metaffi_types)
 		retval_array = RetvalArray(*retval_metaffi_types)
 		
-		if not isinstance(params_metaffi_types, tuple):
-			params_metaffi_types = tuple(params_metaffi_types)
+		# capsule the metaffi_type_info objects to access them in call_xcall
+		for i in range(len(params_metaffi_types)):
+			params_metaffi_types[i] = ctypes.pythonapi.PyCapsule_New(ctypes.byref(params_metaffi_types[i]), None, None)
 		
-		if not isinstance(retval_metaffi_types, tuple):
-			retval_metaffi_types = tuple(retval_metaffi_types)
+		for i in range(len(retval_metaffi_types)):
+			retval_metaffi_types[i] = ctypes.pythonapi.PyCapsule_New(ctypes.byref(retval_metaffi_types[i]), None, None)
 		
+		params_metaffi_types = tuple(params_metaffi_types)
+		retval_metaffi_types = tuple(retval_metaffi_types)
 		
 		# Call xllr.load_function
 		pxcall_and_context = self.xllr.load_function('xllr.' + self.runtime.runtime_plugin, self.module_path, function_path, params_array, retval_array, len(params_metaffi_types), len(retval_metaffi_types))
 		
 		pxcall_and_context_array = ctypes.cast(pxcall_and_context, ctypes.POINTER(ctypes.c_void_p * 2))
 		
 		pxcall = None
```

### Comparing `metaffi_api-0.0.20/metaffi/metaffi_runtime.py` & `metaffi_api-0.0.21/metaffi/metaffi_runtime.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.20/metaffi/metaffi_types.py` & `metaffi_api-0.0.21/metaffi/metaffi_types.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.20/metaffi/pycdts_converter.py` & `metaffi_api-0.0.21/metaffi/pycdts_converter.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.20/metaffi/xllr_wrapper.py` & `metaffi_api-0.0.21/metaffi/xllr_wrapper.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.20/publish.ps1` & `metaffi_api-0.0.21/publish.ps1`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.20/pyproject.toml` & `metaffi_api-0.0.21/pyproject.toml`

 * *Files identical despite different names*


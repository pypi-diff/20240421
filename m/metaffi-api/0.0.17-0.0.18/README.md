# Comparing `tmp/metaffi_api-0.0.17.tar.gz` & `tmp/metaffi_api-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaffi_api-0.0.17.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "metaffi_api-0.0.18.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `metaffi_api-0.0.17.tar` & `metaffi_api-0.0.18.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1096 2022-05-28 09:56:58.251104 metaffi_api-0.0.17/LICENSE
--rw-r--r--   0        0        0       57 2024-01-18 12:19:08.787247 metaffi_api-0.0.17/README.md
--rw-r--r--   0        0        0      428 2024-03-21 09:28:45.053391 metaffi_api-0.0.17/metaffi/__init__.py
--rw-r--r--   0        0        0     1270 2024-02-04 18:44:32.014120 metaffi_api-0.0.17/metaffi/classes_metaffi.puml
--rw-r--r--   0        0        0      122 2024-01-01 14:18:03.539263 metaffi_api-0.0.17/metaffi/metaffi_handle.py
--rw-r--r--   0        0        0     4707 2024-03-21 09:28:18.607422 metaffi_api-0.0.17/metaffi/metaffi_module.py
--rw-r--r--   0        0        0      513 2024-01-01 16:45:39.723929 metaffi_api-0.0.17/metaffi/metaffi_runtime.py
--rw-r--r--   0        0        0     4645 2024-03-21 09:27:11.932843 metaffi_api-0.0.17/metaffi/metaffi_types.py
--rw-r--r--   0        0        0     1471 2024-03-21 09:19:16.794164 metaffi_api-0.0.17/metaffi/pycdts_converter.py
--rw-r--r--   0        0        0     4737 2024-03-08 22:16:45.684205 metaffi_api-0.0.17/metaffi/xllr_wrapper.py
--rw-r--r--   0        0        0       61 2024-01-18 12:25:18.881655 metaffi_api-0.0.17/publish.ps1
--rw-r--r--   0        0        0      535 2024-03-08 20:55:47.528284 metaffi_api-0.0.17/pyproject.toml
--rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 metaffi_api-0.0.17/PKG-INFO
+-rw-r--r--   0        0        0      205 2024-04-15 06:15:13.341334 metaffi_api-0.0.18/CMakeLists.txt
+-rw-r--r--   0        0        0     1096 2022-05-28 09:56:58.251104 metaffi_api-0.0.18/LICENSE
+-rw-r--r--   0        0        0       57 2024-01-18 12:19:08.787247 metaffi_api-0.0.18/README.md
+-rw-r--r--   0        0        0      428 2024-04-21 08:54:06.172376 metaffi_api-0.0.18/metaffi/__init__.py
+-rw-r--r--   0        0        0     1270 2024-02-04 18:44:32.014120 metaffi_api-0.0.18/metaffi/classes_metaffi.puml
+-rw-r--r--   0        0        0      122 2024-01-01 14:18:03.539263 metaffi_api-0.0.18/metaffi/metaffi_handle.py
+-rw-r--r--   0        0        0     4920 2024-04-21 08:50:29.056725 metaffi_api-0.0.18/metaffi/metaffi_module.py
+-rw-r--r--   0        0        0      513 2024-01-01 16:45:39.723929 metaffi_api-0.0.18/metaffi/metaffi_runtime.py
+-rw-r--r--   0        0        0     4641 2024-03-24 21:04:39.262727 metaffi_api-0.0.18/metaffi/metaffi_types.py
+-rw-r--r--   0        0        0     1471 2024-03-21 09:19:16.794164 metaffi_api-0.0.18/metaffi/pycdts_converter.py
+-rw-r--r--   0        0        0     4737 2024-03-08 22:16:45.684205 metaffi_api-0.0.18/metaffi/xllr_wrapper.py
+-rw-r--r--   0        0        0      369 2024-03-21 09:33:10.677841 metaffi_api-0.0.18/publish.ps1
+-rw-r--r--   0        0        0      535 2024-03-08 20:55:47.528284 metaffi_api-0.0.18/pyproject.toml
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 metaffi_api-0.0.18/PKG-INFO
```

### Comparing `metaffi_api-0.0.17/LICENSE` & `metaffi_api-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.17/metaffi/classes_metaffi.puml` & `metaffi_api-0.0.18/metaffi/classes_metaffi.puml`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.17/metaffi/metaffi_module.py` & `metaffi_api-0.0.18/metaffi/metaffi_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,43 +37,50 @@
 	elif len(params_metaffi_types) == 0 and len(retval_metaffi_types) > 0:
 		pxcall = XCallNoParamsRetType(pxcall_and_context_array.contents[0])
 	else:
 		pxcall = XCallNoParamsNoRetType(pxcall_and_context_array.contents[0])
 	
 	context = pxcall_and_context_array.contents[1]
 	
-	res = create_lambda(pxcall, context, params_array, retvals_array)
+	res = create_lambda(pxcall, context, params_metaffi_types, retval_metaffi_types)
 	setattr(res, 'pxcall_and_context', ctypes.addressof(pxcall_and_context_array.contents))
 	setattr(res, 'params_metaffi_types', params_metaffi_types)
 	setattr(res, 'retval_metaffi_types', retval_metaffi_types)
 	return res
 
 
 class MetaFFIModule:
 	def __init__(self, runtime: metaffi.metaffi_runtime.MetaFFIRuntime, xllr: metaffi.xllr_wrapper._XllrWrapper, module_path: str):
 		self.runtime = runtime
 		self.xllr = xllr
 		self.module_path = module_path
 	
-	def load(self, function_path: str, params_metaffi_types: List[metaffi.metaffi_types.metaffi_type_info] | None,
-			retval_metaffi_types: List[metaffi.metaffi_types.metaffi_type_info] | None) -> Callable[..., Tuple[Any, ...]]:
+	def load(self, function_path: str, params_metaffi_types: Tuple[metaffi.metaffi_types.metaffi_type_info] | None,
+			retval_metaffi_types: Tuple[metaffi.metaffi_types.metaffi_type_info] | None) -> Callable[..., Tuple[Any, ...]]:
 		
 		if params_metaffi_types is None:
-			params_metaffi_types = []
+			params_metaffi_types = tuple()
 		
 		if retval_metaffi_types is None:
-			retval_metaffi_types = []
+			retval_metaffi_types = tuple()
 		
 		# Create ctypes arrays for params_metaffi_types and retval_metaffi_types
 		ParamsArray = metaffi.metaffi_types.metaffi_type_info * len(params_metaffi_types)
 		params_array = ParamsArray(*params_metaffi_types)
 		
 		RetvalArray = metaffi.metaffi_types.metaffi_type_info * len(retval_metaffi_types)
 		retval_array = RetvalArray(*retval_metaffi_types)
 		
+		if not isinstance(params_metaffi_types, tuple):
+			params_metaffi_types = tuple(params_metaffi_types)
+		
+		if not isinstance(retval_metaffi_types, tuple):
+			retval_metaffi_types = tuple(retval_metaffi_types)
+		
+		
 		# Call xllr.load_function
 		pxcall_and_context = self.xllr.load_function('xllr.' + self.runtime.runtime_plugin, self.module_path, function_path, params_array, retval_array, len(params_metaffi_types), len(retval_metaffi_types))
 		
 		pxcall_and_context_array = ctypes.cast(pxcall_and_context, ctypes.POINTER(ctypes.c_void_p * 2))
 		
 		pxcall = None
 		if len(params_metaffi_types) > 0 and len(retval_metaffi_types) > 0:
@@ -83,10 +90,10 @@
 		elif len(params_metaffi_types) == 0 and len(retval_metaffi_types) > 0:
 			pxcall = XCallNoParamsRetType(pxcall_and_context_array.contents[0])
 		else:
 			pxcall = XCallNoParamsNoRetType(pxcall_and_context_array.contents[0])
 		
 		context = pxcall_and_context_array.contents[1]
 		
-		func_lambda: Callable[..., ...] = lambda *args: metaffi.xllr_wrapper.xllr_python3.call_xcall(pxcall, context, params_array, len(params_metaffi_types), retval_array, len(retval_metaffi_types), None if not args else args)
+		func_lambda: Callable[..., ...] = lambda *args: metaffi.xllr_wrapper.xllr_python3.call_xcall(pxcall, context, params_metaffi_types, retval_metaffi_types, None if not args else args)
 		
 		return func_lambda
```

### Comparing `metaffi_api-0.0.17/metaffi/metaffi_runtime.py` & `metaffi_api-0.0.18/metaffi/metaffi_runtime.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.17/metaffi/metaffi_types.py` & `metaffi_api-0.0.18/metaffi/metaffi_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 		else:
 			# If alias is None, set the alias to NULL and alias_length to 0
 			self.alias = None
 			self.alias_length = ctypes.c_uint64(0)
 
 
 # Define the pointer type for metaffi_type_info
-metaffi_type_infos_ptr = ctypes.POINTER(metaffi_type_info)
+metaffi_type_info* = ctypes.POINTER(metaffi_type_info)
 
 pytype_to_metaffi_type_dict = {
 	'str': MetaFFITypes.metaffi_string8_type.value,
 	'int': MetaFFITypes.metaffi_int64_type.value,
 	'float': MetaFFITypes.metaffi_float64_type.value,
 	'bool': MetaFFITypes.metaffi_bool_type.value,
 	'list': MetaFFITypes.metaffi_any_type.value,
```

### Comparing `metaffi_api-0.0.17/metaffi/pycdts_converter.py` & `metaffi_api-0.0.18/metaffi/pycdts_converter.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.17/metaffi/xllr_wrapper.py` & `metaffi_api-0.0.18/metaffi/xllr_wrapper.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.17/pyproject.toml` & `metaffi_api-0.0.18/pyproject.toml`

 * *Files identical despite different names*


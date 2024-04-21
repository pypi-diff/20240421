# Comparing `tmp/metaffi_api-0.0.22.tar.gz` & `tmp/metaffi_api-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaffi_api-0.0.22.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "metaffi_api-0.0.23.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `metaffi_api-0.0.22.tar` & `metaffi_api-0.0.23.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      205 2024-04-15 06:15:13.341334 metaffi_api-0.0.22/CMakeLists.txt
--rw-r--r--   0        0        0     1096 2022-05-28 09:56:58.251104 metaffi_api-0.0.22/LICENSE
--rw-r--r--   0        0        0       57 2024-01-18 12:19:08.787247 metaffi_api-0.0.22/README.md
--rw-r--r--   0        0        0      428 2024-04-21 13:02:16.034284 metaffi_api-0.0.22/metaffi/__init__.py
--rw-r--r--   0        0        0     1270 2024-02-04 18:44:32.014120 metaffi_api-0.0.22/metaffi/classes_metaffi.puml
--rw-r--r--   0        0        0      122 2024-01-01 14:18:03.539263 metaffi_api-0.0.22/metaffi/metaffi_handle.py
--rw-r--r--   0        0        0     4988 2024-04-21 12:58:09.252965 metaffi_api-0.0.22/metaffi/metaffi_module.py
--rw-r--r--   0        0        0      513 2024-01-01 16:45:39.723929 metaffi_api-0.0.22/metaffi/metaffi_runtime.py
--rw-r--r--   0        0        0     4642 2024-04-21 08:59:16.278139 metaffi_api-0.0.22/metaffi/metaffi_types.py
--rw-r--r--   0        0        0     1471 2024-03-21 09:19:16.794164 metaffi_api-0.0.22/metaffi/pycdts_converter.py
--rw-r--r--   0        0        0     4712 2024-04-21 09:02:26.437120 metaffi_api-0.0.22/metaffi/xllr_wrapper.py
--rw-r--r--   0        0        0      584 2024-04-21 10:05:04.530248 metaffi_api-0.0.22/publish.ps1
--rw-r--r--   0        0        0      535 2024-03-08 20:55:47.528284 metaffi_api-0.0.22/pyproject.toml
--rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 metaffi_api-0.0.22/PKG-INFO
+-rw-r--r--   0        0        0      205 2024-04-15 06:15:13.341334 metaffi_api-0.0.23/CMakeLists.txt
+-rw-r--r--   0        0        0     1096 2022-05-28 09:56:58.251104 metaffi_api-0.0.23/LICENSE
+-rw-r--r--   0        0        0       57 2024-01-18 12:19:08.787247 metaffi_api-0.0.23/README.md
+-rw-r--r--   0        0        0      428 2024-04-21 13:25:10.051618 metaffi_api-0.0.23/metaffi/__init__.py
+-rw-r--r--   0        0        0     1270 2024-02-04 18:44:32.014120 metaffi_api-0.0.23/metaffi/classes_metaffi.puml
+-rw-r--r--   0        0        0      122 2024-01-01 14:18:03.539263 metaffi_api-0.0.23/metaffi/metaffi_handle.py
+-rw-r--r--   0        0        0     4988 2024-04-21 12:58:09.252965 metaffi_api-0.0.23/metaffi/metaffi_module.py
+-rw-r--r--   0        0        0      513 2024-01-01 16:45:39.723929 metaffi_api-0.0.23/metaffi/metaffi_runtime.py
+-rw-r--r--   0        0        0     4619 2024-04-21 13:24:41.131761 metaffi_api-0.0.23/metaffi/metaffi_types.py
+-rw-r--r--   0        0        0     1471 2024-03-21 09:19:16.794164 metaffi_api-0.0.23/metaffi/pycdts_converter.py
+-rw-r--r--   0        0        0     4712 2024-04-21 09:02:26.437120 metaffi_api-0.0.23/metaffi/xllr_wrapper.py
+-rw-r--r--   0        0        0      584 2024-04-21 10:05:04.530248 metaffi_api-0.0.23/publish.ps1
+-rw-r--r--   0        0        0      535 2024-03-08 20:55:47.528284 metaffi_api-0.0.23/pyproject.toml
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 metaffi_api-0.0.23/PKG-INFO
```

### Comparing `metaffi_api-0.0.22/LICENSE` & `metaffi_api-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.22/metaffi/classes_metaffi.puml` & `metaffi_api-0.0.23/metaffi/classes_metaffi.puml`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.22/metaffi/metaffi_module.py` & `metaffi_api-0.0.23/metaffi/metaffi_module.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.22/metaffi/metaffi_runtime.py` & `metaffi_api-0.0.23/metaffi/metaffi_runtime.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.22/metaffi/metaffi_types.py` & `metaffi_api-0.0.23/metaffi/metaffi_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,32 +53,32 @@
 		return self.name, self.value
 
 
 # Define the struct metaffi_type_info in Python using ctypes
 class metaffi_type_info(ctypes.Structure):
 	_fields_ = [("type", ctypes.c_uint64),  # metaffi_type is defined as uint64_t
 	            ("alias", ctypes.c_char_p),
-	            ("alias_length", ctypes.c_uint64),
-	            ("dimensions", ctypes.c_int32)]
+	            ("is_free_alias", ctypes.c_bool),
+	            ("fixed_dimensions", ctypes.c_int64)]
 	
 	def __init__(self, metaffi_type: MetaFFITypes = MetaFFITypes.metaffi_null_type, alias: str = None, dims: int = 0):
 		super().__init__()
 		
 		# Set the type
 		self.type = ctypes.c_uint64(metaffi_type.value)
-		self.dimensions = dims
+		self.fixed_dimensions = dims
 		
 		# If alias is not None, set the alias and alias_length
 		if alias is not None:
 			self.alias = ctypes.c_char_p(alias.encode('utf-8'))
-			self.alias_length = ctypes.c_uint64(len(alias))
+			self.is_free_alias = True
 		else:
 			# If alias is None, set the alias to NULL and alias_length to 0
 			self.alias = None
-			self.alias_length = ctypes.c_uint64(0)
+			self.is_free_alias = False
 
 
 # Define the pointer type for metaffi_type_info
 metaffi_type_info_p = ctypes.POINTER(metaffi_type_info)
 
 pytype_to_metaffi_type_dict = {
 	'str': MetaFFITypes.metaffi_string8_type.value,
```

### Comparing `metaffi_api-0.0.22/metaffi/pycdts_converter.py` & `metaffi_api-0.0.23/metaffi/pycdts_converter.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.22/metaffi/xllr_wrapper.py` & `metaffi_api-0.0.23/metaffi/xllr_wrapper.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.22/publish.ps1` & `metaffi_api-0.0.23/publish.ps1`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.22/pyproject.toml` & `metaffi_api-0.0.23/pyproject.toml`

 * *Files identical despite different names*


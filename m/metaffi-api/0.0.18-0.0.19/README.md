# Comparing `tmp/metaffi_api-0.0.18.tar.gz` & `tmp/metaffi_api-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaffi_api-0.0.18.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "metaffi_api-0.0.19.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `metaffi_api-0.0.18.tar` & `metaffi_api-0.0.19.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      205 2024-04-15 06:15:13.341334 metaffi_api-0.0.18/CMakeLists.txt
--rw-r--r--   0        0        0     1096 2022-05-28 09:56:58.251104 metaffi_api-0.0.18/LICENSE
--rw-r--r--   0        0        0       57 2024-01-18 12:19:08.787247 metaffi_api-0.0.18/README.md
--rw-r--r--   0        0        0      428 2024-04-21 08:54:06.172376 metaffi_api-0.0.18/metaffi/__init__.py
--rw-r--r--   0        0        0     1270 2024-02-04 18:44:32.014120 metaffi_api-0.0.18/metaffi/classes_metaffi.puml
--rw-r--r--   0        0        0      122 2024-01-01 14:18:03.539263 metaffi_api-0.0.18/metaffi/metaffi_handle.py
--rw-r--r--   0        0        0     4920 2024-04-21 08:50:29.056725 metaffi_api-0.0.18/metaffi/metaffi_module.py
--rw-r--r--   0        0        0      513 2024-01-01 16:45:39.723929 metaffi_api-0.0.18/metaffi/metaffi_runtime.py
--rw-r--r--   0        0        0     4641 2024-03-24 21:04:39.262727 metaffi_api-0.0.18/metaffi/metaffi_types.py
--rw-r--r--   0        0        0     1471 2024-03-21 09:19:16.794164 metaffi_api-0.0.18/metaffi/pycdts_converter.py
--rw-r--r--   0        0        0     4737 2024-03-08 22:16:45.684205 metaffi_api-0.0.18/metaffi/xllr_wrapper.py
--rw-r--r--   0        0        0      369 2024-03-21 09:33:10.677841 metaffi_api-0.0.18/publish.ps1
--rw-r--r--   0        0        0      535 2024-03-08 20:55:47.528284 metaffi_api-0.0.18/pyproject.toml
--rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 metaffi_api-0.0.18/PKG-INFO
+-rw-r--r--   0        0        0      205 2024-04-15 06:15:13.341334 metaffi_api-0.0.19/CMakeLists.txt
+-rw-r--r--   0        0        0     1096 2022-05-28 09:56:58.251104 metaffi_api-0.0.19/LICENSE
+-rw-r--r--   0        0        0       57 2024-01-18 12:19:08.787247 metaffi_api-0.0.19/README.md
+-rw-r--r--   0        0        0      428 2024-04-21 08:59:24.009263 metaffi_api-0.0.19/metaffi/__init__.py
+-rw-r--r--   0        0        0     1270 2024-02-04 18:44:32.014120 metaffi_api-0.0.19/metaffi/classes_metaffi.puml
+-rw-r--r--   0        0        0      122 2024-01-01 14:18:03.539263 metaffi_api-0.0.19/metaffi/metaffi_handle.py
+-rw-r--r--   0        0        0     4920 2024-04-21 08:50:29.056725 metaffi_api-0.0.19/metaffi/metaffi_module.py
+-rw-r--r--   0        0        0      513 2024-01-01 16:45:39.723929 metaffi_api-0.0.19/metaffi/metaffi_runtime.py
+-rw-r--r--   0        0        0     4642 2024-04-21 08:59:16.278139 metaffi_api-0.0.19/metaffi/metaffi_types.py
+-rw-r--r--   0        0        0     1471 2024-03-21 09:19:16.794164 metaffi_api-0.0.19/metaffi/pycdts_converter.py
+-rw-r--r--   0        0        0     4737 2024-03-08 22:16:45.684205 metaffi_api-0.0.19/metaffi/xllr_wrapper.py
+-rw-r--r--   0        0        0      561 2024-04-21 08:57:15.005087 metaffi_api-0.0.19/publish.ps1
+-rw-r--r--   0        0        0      535 2024-03-08 20:55:47.528284 metaffi_api-0.0.19/pyproject.toml
+-rw-r--r--   0        0        0      296 2024-04-18 10:00:06.775372 metaffi_api-0.0.19/unittest/test_python311_api.py
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 metaffi_api-0.0.19/PKG-INFO
```

### Comparing `metaffi_api-0.0.18/LICENSE` & `metaffi_api-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.18/metaffi/classes_metaffi.puml` & `metaffi_api-0.0.19/metaffi/classes_metaffi.puml`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.18/metaffi/metaffi_module.py` & `metaffi_api-0.0.19/metaffi/metaffi_module.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.18/metaffi/metaffi_runtime.py` & `metaffi_api-0.0.19/metaffi/metaffi_runtime.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.18/metaffi/metaffi_types.py` & `metaffi_api-0.0.19/metaffi/metaffi_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 		else:
 			# If alias is None, set the alias to NULL and alias_length to 0
 			self.alias = None
 			self.alias_length = ctypes.c_uint64(0)
 
 
 # Define the pointer type for metaffi_type_info
-metaffi_type_info* = ctypes.POINTER(metaffi_type_info)
+metaffi_type_info_p = ctypes.POINTER(metaffi_type_info)
 
 pytype_to_metaffi_type_dict = {
 	'str': MetaFFITypes.metaffi_string8_type.value,
 	'int': MetaFFITypes.metaffi_int64_type.value,
 	'float': MetaFFITypes.metaffi_float64_type.value,
 	'bool': MetaFFITypes.metaffi_bool_type.value,
 	'list': MetaFFITypes.metaffi_any_type.value,
```

### Comparing `metaffi_api-0.0.18/metaffi/pycdts_converter.py` & `metaffi_api-0.0.19/metaffi/pycdts_converter.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.18/metaffi/xllr_wrapper.py` & `metaffi_api-0.0.19/metaffi/xllr_wrapper.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.18/pyproject.toml` & `metaffi_api-0.0.19/pyproject.toml`

 * *Files identical despite different names*


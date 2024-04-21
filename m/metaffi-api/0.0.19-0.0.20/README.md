# Comparing `tmp/metaffi_api-0.0.19.tar.gz` & `tmp/metaffi_api-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaffi_api-0.0.19.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "metaffi_api-0.0.20.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `metaffi_api-0.0.19.tar` & `metaffi_api-0.0.20.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0      205 2024-04-15 06:15:13.341334 metaffi_api-0.0.19/CMakeLists.txt
--rw-r--r--   0        0        0     1096 2022-05-28 09:56:58.251104 metaffi_api-0.0.19/LICENSE
--rw-r--r--   0        0        0       57 2024-01-18 12:19:08.787247 metaffi_api-0.0.19/README.md
--rw-r--r--   0        0        0      428 2024-04-21 08:59:24.009263 metaffi_api-0.0.19/metaffi/__init__.py
--rw-r--r--   0        0        0     1270 2024-02-04 18:44:32.014120 metaffi_api-0.0.19/metaffi/classes_metaffi.puml
--rw-r--r--   0        0        0      122 2024-01-01 14:18:03.539263 metaffi_api-0.0.19/metaffi/metaffi_handle.py
--rw-r--r--   0        0        0     4920 2024-04-21 08:50:29.056725 metaffi_api-0.0.19/metaffi/metaffi_module.py
--rw-r--r--   0        0        0      513 2024-01-01 16:45:39.723929 metaffi_api-0.0.19/metaffi/metaffi_runtime.py
--rw-r--r--   0        0        0     4642 2024-04-21 08:59:16.278139 metaffi_api-0.0.19/metaffi/metaffi_types.py
--rw-r--r--   0        0        0     1471 2024-03-21 09:19:16.794164 metaffi_api-0.0.19/metaffi/pycdts_converter.py
--rw-r--r--   0        0        0     4737 2024-03-08 22:16:45.684205 metaffi_api-0.0.19/metaffi/xllr_wrapper.py
--rw-r--r--   0        0        0      561 2024-04-21 08:57:15.005087 metaffi_api-0.0.19/publish.ps1
--rw-r--r--   0        0        0      535 2024-03-08 20:55:47.528284 metaffi_api-0.0.19/pyproject.toml
--rw-r--r--   0        0        0      296 2024-04-18 10:00:06.775372 metaffi_api-0.0.19/unittest/test_python311_api.py
--rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 metaffi_api-0.0.19/PKG-INFO
+-rw-r--r--   0        0        0      205 2024-04-15 06:15:13.341334 metaffi_api-0.0.20/CMakeLists.txt
+-rw-r--r--   0        0        0     1096 2022-05-28 09:56:58.251104 metaffi_api-0.0.20/LICENSE
+-rw-r--r--   0        0        0       57 2024-01-18 12:19:08.787247 metaffi_api-0.0.20/README.md
+-rw-r--r--   0        0        0      428 2024-04-21 09:02:34.475590 metaffi_api-0.0.20/metaffi/__init__.py
+-rw-r--r--   0        0        0     1270 2024-02-04 18:44:32.014120 metaffi_api-0.0.20/metaffi/classes_metaffi.puml
+-rw-r--r--   0        0        0      122 2024-01-01 14:18:03.539263 metaffi_api-0.0.20/metaffi/metaffi_handle.py
+-rw-r--r--   0        0        0     4920 2024-04-21 08:50:29.056725 metaffi_api-0.0.20/metaffi/metaffi_module.py
+-rw-r--r--   0        0        0      513 2024-01-01 16:45:39.723929 metaffi_api-0.0.20/metaffi/metaffi_runtime.py
+-rw-r--r--   0        0        0     4642 2024-04-21 08:59:16.278139 metaffi_api-0.0.20/metaffi/metaffi_types.py
+-rw-r--r--   0        0        0     1471 2024-03-21 09:19:16.794164 metaffi_api-0.0.20/metaffi/pycdts_converter.py
+-rw-r--r--   0        0        0     4712 2024-04-21 09:02:26.437120 metaffi_api-0.0.20/metaffi/xllr_wrapper.py
+-rw-r--r--   0        0        0      584 2024-04-21 09:03:09.582637 metaffi_api-0.0.20/publish.ps1
+-rw-r--r--   0        0        0      535 2024-03-08 20:55:47.528284 metaffi_api-0.0.20/pyproject.toml
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 metaffi_api-0.0.20/PKG-INFO
```

### Comparing `metaffi_api-0.0.19/LICENSE` & `metaffi_api-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.19/metaffi/classes_metaffi.puml` & `metaffi_api-0.0.20/metaffi/classes_metaffi.puml`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.19/metaffi/metaffi_module.py` & `metaffi_api-0.0.20/metaffi/metaffi_module.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.19/metaffi/metaffi_runtime.py` & `metaffi_api-0.0.20/metaffi/metaffi_runtime.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.19/metaffi/metaffi_types.py` & `metaffi_api-0.0.20/metaffi/metaffi_types.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.19/metaffi/pycdts_converter.py` & `metaffi_api-0.0.20/metaffi/pycdts_converter.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.19/metaffi/xllr_wrapper.py` & `metaffi_api-0.0.20/metaffi/xllr_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 		return os.getenv('METAFFI_HOME') + '/' + fname + '.so'  # for everything that is not windows or mac, return .so
 
 
 if platform.system() == 'Windows':
 	os.add_dll_directory(os.getenv('METAFFI_HOME')+'\\bin\\')
 
 xllr_python3 = ctypes.cdll.LoadLibrary(get_dynamic_lib_path_from_metaffi_home('xllr.python311'))
-xllr_python3.call_xcall.argtypes = [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_void_p, ctypes.c_uint64, ctypes.c_void_p, ctypes.c_void_p, py_object]
+xllr_python3.call_xcall.argtypes = [ctypes.c_void_p, ctypes.c_void_p, ctypes.py_object, ctypes.py_object, ctypes.py_object]
 xllr_python3.call_xcall.restype = py_object
 
 xllr = cdll.LoadLibrary(get_dynamic_lib_path_from_metaffi_home('xllr'))
 
 # Set argtypes and restype
 xllr.load_runtime_plugin.argtypes = [ctypes.c_char_p, ctypes.c_uint32, ctypes.POINTER(ctypes.c_char_p), ctypes.POINTER(ctypes.c_uint32)]
 xllr.load_runtime_plugin.restype = None
```

### Comparing `metaffi_api-0.0.19/publish.ps1` & `metaffi_api-0.0.20/publish.ps1`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 
 # Move ./tests directory to parent directory
 Move-Item -Path .\tests -Destination ..
-Move-Item -Path .\unitest -Destination ..
+Move-Item -Path .\unittest -Destination ..
 
 # Publish to pypi
 flit publish --repository pypi --pypirc C:\Users\green\.pyirc
 
 # Move back the "tests" directory from parent directory to current directory
 Move-Item -Path ..\tests -Destination .
-Move-Item -Path ..\unitest -Destination .
+Move-Item -Path ..\unittest -Destination .
 
 # wait for pypi to update
-Write-Host "waiting 10 seconds for pypi to update"
-Start-Sleep -Seconds 10
+Write-Host "waiting 30 seconds for pypi to update"
+Start-Sleep -Seconds 30
 
 # Update metaffi-api pip package
-py -m pip install metaffi-api --upgrade
+py -m pip install metaffi-api --upgrade
+
+Write-Host "done"
```

### Comparing `metaffi_api-0.0.19/pyproject.toml` & `metaffi_api-0.0.20/pyproject.toml`

 * *Files identical despite different names*


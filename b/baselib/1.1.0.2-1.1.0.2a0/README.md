# Comparing `tmp/baselib-1.1.0.2.tar.gz` & `tmp/baselib-1.1.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baselib-1.1.0.2.tar", last modified: Sun Apr 21 10:20:57 2024, max compression
+gzip compressed data, was "baselib-1.1.0.2a0.tar", last modified: Sun Apr 21 13:47:25 2024, max compression
```

## Comparing `baselib-1.1.0.2.tar` & `baselib-1.1.0.2a0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.515686 baselib-1.1.0.2/
--rw-r--r--   0 coreylin   (501) staff       (20)    35149 2023-02-04 13:19:24.000000 baselib-1.1.0.2/LICENSE
--rw-r--r--   0 coreylin   (501) staff       (20)     2326 2024-04-21 10:20:57.515563 baselib-1.1.0.2/PKG-INFO
--rw-r--r--   0 coreylin   (501) staff       (20)     2035 2024-03-10 13:49:43.000000 baselib-1.1.0.2/README.md
-drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.508807 baselib-1.1.0.2/baselib/
--rw-r--r--   0 coreylin   (501) staff       (20)        0 2023-02-04 13:19:24.000000 baselib-1.1.0.2/baselib/__init__.py
-drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.510125 baselib-1.1.0.2/baselib/channel/
--rw-r--r--   0 coreylin   (501) staff       (20)       63 2024-03-10 12:54:47.000000 baselib-1.1.0.2/baselib/channel/__init__.py
--rw-r--r--   0 coreylin   (501) staff       (20)     3771 2024-03-10 12:53:35.000000 baselib-1.1.0.2/baselib/channel/base_channel.py
-drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.510571 baselib-1.1.0.2/baselib/demo/
--rw-r--r--   0 coreylin   (501) staff       (20)       22 2023-02-04 13:19:24.000000 baselib-1.1.0.2/baselib/demo/__init__.py
--rw-r--r--   0 coreylin   (501) staff       (20)       86 2023-02-04 13:19:24.000000 baselib-1.1.0.2/baselib/demo/demo.py
-drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.511042 baselib-1.1.0.2/baselib/feishu/
--rw-r--r--   0 coreylin   (501) staff       (20)       44 2024-03-10 13:48:54.000000 baselib-1.1.0.2/baselib/feishu/__init__.py
--rw-r--r--   0 coreylin   (501) staff       (20)     5759 2024-03-10 13:48:18.000000 baselib-1.1.0.2/baselib/feishu/robot.py
-drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.511557 baselib-1.1.0.2/baselib/json/
--rw-r--r--   0 coreylin   (501) staff       (20)       44 2023-04-05 13:59:51.000000 baselib-1.1.0.2/baselib/json/__init__.py
--rw-r--r--   0 coreylin   (501) staff       (20)     1804 2024-03-10 13:52:12.000000 baselib-1.1.0.2/baselib/json/json_file.py
-drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.512000 baselib-1.1.0.2/baselib/log/
--rw-r--r--   0 coreylin   (501) staff       (20)       40 2023-04-05 13:59:51.000000 baselib-1.1.0.2/baselib/log/__init__.py
--rw-r--r--   0 coreylin   (501) staff       (20)     2219 2023-04-05 13:59:51.000000 baselib-1.1.0.2/baselib/log/file.py
-drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.512218 baselib-1.1.0.2/baselib/py/
--rw-r--r--   0 coreylin   (501) staff       (20)      717 2024-03-10 13:49:43.000000 baselib-1.1.0.2/baselib/py/__init__.py
-drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.512726 baselib-1.1.0.2/baselib/qywx/
--rw-r--r--   0 coreylin   (501) staff       (20)       38 2023-04-05 13:59:51.000000 baselib-1.1.0.2/baselib/qywx/__init__.py
--rw-r--r--   0 coreylin   (501) staff       (20)    13625 2024-03-10 13:49:43.000000 baselib-1.1.0.2/baselib/qywx/qywx.py
-drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.513060 baselib-1.1.0.2/baselib/request/
--rw-r--r--   0 coreylin   (501) staff       (20)        0 2023-04-03 14:48:56.000000 baselib-1.1.0.2/baselib/request/__init__.py
-drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.513157 baselib-1.1.0.2/baselib/system/
--rw-r--r--   0 coreylin   (501) staff       (20)     3384 2024-03-10 13:49:43.000000 baselib-1.1.0.2/baselib/system/__init__.py
-drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.514776 baselib-1.1.0.2/baselib/tests/
--rw-r--r--   0 coreylin   (501) staff       (20)        0 2023-02-04 13:19:24.000000 baselib-1.1.0.2/baselib/tests/__init__.py
--rw-r--r--   0 coreylin   (501) staff       (20)     4989 2023-04-03 14:50:20.000000 baselib-1.1.0.2/baselib/tests/debug.py
--rw-r--r--   0 coreylin   (501) staff       (20)      126 2023-02-04 13:19:24.000000 baselib-1.1.0.2/baselib/tests/demo_test.py
--rw-r--r--   0 coreylin   (501) staff       (20)     1838 2024-03-10 13:49:43.000000 baselib-1.1.0.2/baselib/tests/file_logger_test.py
--rw-r--r--   0 coreylin   (501) staff       (20)      494 2024-03-10 13:49:43.000000 baselib-1.1.0.2/baselib/tests/httplib_test.py
--rw-r--r--   0 coreylin   (501) staff       (20)     1122 2024-03-10 14:01:54.000000 baselib-1.1.0.2/baselib/tests/json_file_test.py
--rw-r--r--   0 coreylin   (501) staff       (20)     2800 2024-03-10 13:49:43.000000 baselib-1.1.0.2/baselib/tests/period_test.py
--rw-r--r--   0 coreylin   (501) staff       (20)     3154 2024-03-10 13:49:43.000000 baselib-1.1.0.2/baselib/tests/qywx_test.py
-drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.515290 baselib-1.1.0.2/baselib/time/
--rw-r--r--   0 coreylin   (501) staff       (20)       39 2023-04-05 13:59:51.000000 baselib-1.1.0.2/baselib/time/__init__.py
--rw-r--r--   0 coreylin   (501) staff       (20)     4480 2023-02-04 13:19:24.000000 baselib-1.1.0.2/baselib/time/period.py
-drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.509618 baselib-1.1.0.2/baselib.egg-info/
--rw-r--r--   0 coreylin   (501) staff       (20)     2326 2024-04-21 10:20:57.000000 baselib-1.1.0.2/baselib.egg-info/PKG-INFO
--rw-r--r--   0 coreylin   (501) staff       (20)      852 2024-04-21 10:20:57.000000 baselib-1.1.0.2/baselib.egg-info/SOURCES.txt
--rw-r--r--   0 coreylin   (501) staff       (20)        1 2024-04-21 10:20:57.000000 baselib-1.1.0.2/baselib.egg-info/dependency_links.txt
--rw-r--r--   0 coreylin   (501) staff       (20)        1 2023-02-10 15:58:03.000000 baselib-1.1.0.2/baselib.egg-info/not-zip-safe
--rw-r--r--   0 coreylin   (501) staff       (20)        8 2024-04-21 10:20:57.000000 baselib-1.1.0.2/baselib.egg-info/top_level.txt
--rw-r--r--   0 coreylin   (501) staff       (20)       38 2024-04-21 10:20:57.515727 baselib-1.1.0.2/setup.cfg
--rw-r--r--   0 coreylin   (501) staff       (20)      830 2024-04-21 10:20:32.000000 baselib-1.1.0.2/setup.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 13:47:25.289753 baselib-1.1.0.2a0/
+-rw-r--r--   0 coreylin   (501) staff       (20)    35149 2023-02-04 13:19:24.000000 baselib-1.1.0.2a0/LICENSE
+-rw-r--r--   0 coreylin   (501) staff       (20)     2328 2024-04-21 13:47:25.289600 baselib-1.1.0.2a0/PKG-INFO
+-rw-r--r--   0 coreylin   (501) staff       (20)     2035 2024-03-10 13:49:43.000000 baselib-1.1.0.2a0/README.md
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 13:47:25.284772 baselib-1.1.0.2a0/baselib/
+-rw-r--r--   0 coreylin   (501) staff       (20)        0 2023-02-04 13:19:24.000000 baselib-1.1.0.2a0/baselib/__init__.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 13:47:25.285939 baselib-1.1.0.2a0/baselib/channel/
+-rw-r--r--   0 coreylin   (501) staff       (20)       63 2024-03-10 12:54:47.000000 baselib-1.1.0.2a0/baselib/channel/__init__.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     3771 2024-03-10 12:53:35.000000 baselib-1.1.0.2a0/baselib/channel/base_channel.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 13:47:25.286444 baselib-1.1.0.2a0/baselib/demo/
+-rw-r--r--   0 coreylin   (501) staff       (20)       22 2023-02-04 13:19:24.000000 baselib-1.1.0.2a0/baselib/demo/__init__.py
+-rw-r--r--   0 coreylin   (501) staff       (20)       86 2023-02-04 13:19:24.000000 baselib-1.1.0.2a0/baselib/demo/demo.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 13:47:25.286726 baselib-1.1.0.2a0/baselib/feishu/
+-rw-r--r--   0 coreylin   (501) staff       (20)       44 2024-03-10 13:48:54.000000 baselib-1.1.0.2a0/baselib/feishu/__init__.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     5759 2024-03-10 13:48:18.000000 baselib-1.1.0.2a0/baselib/feishu/robot.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 13:47:25.287042 baselib-1.1.0.2a0/baselib/json/
+-rw-r--r--   0 coreylin   (501) staff       (20)       44 2023-04-05 13:59:51.000000 baselib-1.1.0.2a0/baselib/json/__init__.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     1804 2024-03-10 13:52:12.000000 baselib-1.1.0.2a0/baselib/json/json_file.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 13:47:25.287274 baselib-1.1.0.2a0/baselib/log/
+-rw-r--r--   0 coreylin   (501) staff       (20)       40 2023-04-05 13:59:51.000000 baselib-1.1.0.2a0/baselib/log/__init__.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     2219 2023-04-05 13:59:51.000000 baselib-1.1.0.2a0/baselib/log/file.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 13:47:25.287389 baselib-1.1.0.2a0/baselib/py/
+-rw-r--r--   0 coreylin   (501) staff       (20)      717 2024-03-10 13:49:43.000000 baselib-1.1.0.2a0/baselib/py/__init__.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 13:47:25.287750 baselib-1.1.0.2a0/baselib/qywx/
+-rw-r--r--   0 coreylin   (501) staff       (20)       38 2023-04-05 13:59:51.000000 baselib-1.1.0.2a0/baselib/qywx/__init__.py
+-rw-r--r--   0 coreylin   (501) staff       (20)    13625 2024-03-10 13:49:43.000000 baselib-1.1.0.2a0/baselib/qywx/qywx.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 13:47:25.287933 baselib-1.1.0.2a0/baselib/request/
+-rw-r--r--   0 coreylin   (501) staff       (20)        0 2023-04-03 14:48:56.000000 baselib-1.1.0.2a0/baselib/request/__init__.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 13:47:25.288032 baselib-1.1.0.2a0/baselib/system/
+-rw-r--r--   0 coreylin   (501) staff       (20)     3384 2024-03-10 13:49:43.000000 baselib-1.1.0.2a0/baselib/system/__init__.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 13:47:25.289092 baselib-1.1.0.2a0/baselib/tests/
+-rw-r--r--   0 coreylin   (501) staff       (20)        0 2023-02-04 13:19:24.000000 baselib-1.1.0.2a0/baselib/tests/__init__.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     4989 2023-04-03 14:50:20.000000 baselib-1.1.0.2a0/baselib/tests/debug.py
+-rw-r--r--   0 coreylin   (501) staff       (20)      126 2023-02-04 13:19:24.000000 baselib-1.1.0.2a0/baselib/tests/demo_test.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     1838 2024-03-10 13:49:43.000000 baselib-1.1.0.2a0/baselib/tests/file_logger_test.py
+-rw-r--r--   0 coreylin   (501) staff       (20)      494 2024-03-10 13:49:43.000000 baselib-1.1.0.2a0/baselib/tests/httplib_test.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     1122 2024-03-10 14:01:54.000000 baselib-1.1.0.2a0/baselib/tests/json_file_test.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     2800 2024-03-10 13:49:43.000000 baselib-1.1.0.2a0/baselib/tests/period_test.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     3154 2024-03-10 13:49:43.000000 baselib-1.1.0.2a0/baselib/tests/qywx_test.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 13:47:25.289315 baselib-1.1.0.2a0/baselib/time/
+-rw-r--r--   0 coreylin   (501) staff       (20)       39 2023-04-05 13:59:51.000000 baselib-1.1.0.2a0/baselib/time/__init__.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     4480 2023-02-04 13:19:24.000000 baselib-1.1.0.2a0/baselib/time/period.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 13:47:25.285664 baselib-1.1.0.2a0/baselib.egg-info/
+-rw-r--r--   0 coreylin   (501) staff       (20)     2328 2024-04-21 13:47:25.000000 baselib-1.1.0.2a0/baselib.egg-info/PKG-INFO
+-rw-r--r--   0 coreylin   (501) staff       (20)      852 2024-04-21 13:47:25.000000 baselib-1.1.0.2a0/baselib.egg-info/SOURCES.txt
+-rw-r--r--   0 coreylin   (501) staff       (20)        1 2024-04-21 13:47:25.000000 baselib-1.1.0.2a0/baselib.egg-info/dependency_links.txt
+-rw-r--r--   0 coreylin   (501) staff       (20)        1 2023-02-10 15:58:03.000000 baselib-1.1.0.2a0/baselib.egg-info/not-zip-safe
+-rw-r--r--   0 coreylin   (501) staff       (20)        8 2024-04-21 13:47:25.000000 baselib-1.1.0.2a0/baselib.egg-info/top_level.txt
+-rw-r--r--   0 coreylin   (501) staff       (20)       38 2024-04-21 13:47:25.289870 baselib-1.1.0.2a0/setup.cfg
+-rw-r--r--   0 coreylin   (501) staff       (20)      831 2024-04-21 13:47:25.000000 baselib-1.1.0.2a0/setup.py
```

### Comparing `baselib-1.1.0.2/LICENSE` & `baselib-1.1.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.2/PKG-INFO` & `baselib-1.1.0.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baselib
-Version: 1.1.0.2
+Version: 1.1.0.2a0
 Summary: base common lib for python
 Home-page: https://github.com/coreylam/base_common_lib
 Author: coreylam
 Author-email: coreylam@163.com
 License: GPL
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
```

### Comparing `baselib-1.1.0.2/README.md` & `baselib-1.1.0.2a0/README.md`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.2/baselib/channel/base_channel.py` & `baselib-1.1.0.2a0/baselib/channel/base_channel.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.2/baselib/feishu/robot.py` & `baselib-1.1.0.2a0/baselib/feishu/robot.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.2/baselib/json/json_file.py` & `baselib-1.1.0.2a0/baselib/json/json_file.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.2/baselib/log/file.py` & `baselib-1.1.0.2a0/baselib/log/file.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.2/baselib/py/__init__.py` & `baselib-1.1.0.2a0/baselib/py/__init__.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.2/baselib/qywx/qywx.py` & `baselib-1.1.0.2a0/baselib/qywx/qywx.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.2/baselib/system/__init__.py` & `baselib-1.1.0.2a0/baselib/system/__init__.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.2/baselib/tests/debug.py` & `baselib-1.1.0.2a0/baselib/tests/debug.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.2/baselib/tests/file_logger_test.py` & `baselib-1.1.0.2a0/baselib/tests/file_logger_test.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.2/baselib/tests/json_file_test.py` & `baselib-1.1.0.2a0/baselib/tests/json_file_test.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.2/baselib/tests/period_test.py` & `baselib-1.1.0.2a0/baselib/tests/period_test.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.2/baselib/tests/qywx_test.py` & `baselib-1.1.0.2a0/baselib/tests/qywx_test.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.2/baselib/time/period.py` & `baselib-1.1.0.2a0/baselib/time/period.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.2/baselib.egg-info/PKG-INFO` & `baselib-1.1.0.2a0/baselib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baselib
-Version: 1.1.0.2
+Version: 1.1.0.2a0
 Summary: base common lib for python
 Home-page: https://github.com/coreylam/base_common_lib
 Author: coreylam
 Author-email: coreylam@163.com
 License: GPL
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
```

### Comparing `baselib-1.1.0.2/baselib.egg-info/SOURCES.txt` & `baselib-1.1.0.2a0/baselib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.2/setup.py` & `baselib-1.1.0.2a0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         with open(filename, "r") as fid:
             desc = fid.read()
     return desc
 
 
 setup(
     name='baselib',
-    version="1.1.0.2",
+    version="1.1.0.2a",
     description='base common lib for python',
     long_description=read_desc(),
     long_description_content_type="text/markdown",
     author='coreylam',
     author_email='coreylam@163.com',
     url='https://github.com/coreylam/base_common_lib',
     license='GPL',
```


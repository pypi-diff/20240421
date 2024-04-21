# Comparing `tmp/baselib-1.1.0.1b0.tar.gz` & `tmp/baselib-1.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baselib-1.1.0.1b0.tar", last modified: Tue Aug 29 02:52:41 2023, max compression
+gzip compressed data, was "baselib-1.1.0.2.tar", last modified: Sun Apr 21 10:20:57 2024, max compression
```

## Comparing `baselib-1.1.0.1b0.tar` & `baselib-1.1.0.2.tar`

### file list

```diff
@@ -1,44 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 02:52:41.189457 baselib-1.1.0.1b0/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2328 2023-08-29 02:52:41.189457 baselib-1.1.0.1b0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2035 2023-08-29 02:52:39.000000 baselib-1.1.0.1b0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 02:52:41.147457 baselib-1.1.0.1b0/baselib/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 02:52:41.152457 baselib-1.1.0.1b0/baselib/demo/
--rw-r--r--   0 root         (0) root         (0)       22 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/demo/__init__.py
--rw-r--r--   0 root         (0) root         (0)       86 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/demo/demo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 02:52:41.156457 baselib-1.1.0.1b0/baselib/json/
--rw-r--r--   0 root         (0) root         (0)       44 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/json/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1687 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/json/json_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 02:52:41.164457 baselib-1.1.0.1b0/baselib/log/
--rw-r--r--   0 root         (0) root         (0)       40 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2219 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/log/file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 02:52:41.166457 baselib-1.1.0.1b0/baselib/py/
--rw-r--r--   0 root         (0) root         (0)      717 2023-08-29 02:52:39.000000 baselib-1.1.0.1b0/baselib/py/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 02:52:41.168457 baselib-1.1.0.1b0/baselib/qywx/
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/qywx/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13625 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/qywx/qywx.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 02:52:41.170457 baselib-1.1.0.1b0/baselib/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 02:52:41.170457 baselib-1.1.0.1b0/baselib/system/
--rw-r--r--   0 root         (0) root         (0)     3384 2023-08-29 02:52:39.000000 baselib-1.1.0.1b0/baselib/system/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 02:52:41.183457 baselib-1.1.0.1b0/baselib/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4989 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/tests/debug.py
--rw-r--r--   0 root         (0) root         (0)      126 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/tests/demo_test.py
--rw-r--r--   0 root         (0) root         (0)     1838 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/tests/file_logger_test.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/tests/httplib_test.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/tests/json_file_test.py
--rw-r--r--   0 root         (0) root         (0)     2800 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/tests/period_test.py
--rw-r--r--   0 root         (0) root         (0)     3154 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/tests/qywx_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 02:52:41.187457 baselib-1.1.0.1b0/baselib/time/
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/time/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4480 2023-08-17 08:24:15.000000 baselib-1.1.0.1b0/baselib/time/period.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 02:52:41.150457 baselib-1.1.0.1b0/baselib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2328 2023-08-29 02:52:40.000000 baselib-1.1.0.1b0/baselib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      741 2023-08-29 02:52:40.000000 baselib-1.1.0.1b0/baselib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-29 02:52:40.000000 baselib-1.1.0.1b0/baselib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-17 08:40:54.000000 baselib-1.1.0.1b0/baselib.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-29 02:52:40.000000 baselib-1.1.0.1b0/baselib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-29 02:52:41.189457 baselib-1.1.0.1b0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      834 2023-08-29 02:52:39.000000 baselib-1.1.0.1b0/setup.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.515686 baselib-1.1.0.2/
+-rw-r--r--   0 coreylin   (501) staff       (20)    35149 2023-02-04 13:19:24.000000 baselib-1.1.0.2/LICENSE
+-rw-r--r--   0 coreylin   (501) staff       (20)     2326 2024-04-21 10:20:57.515563 baselib-1.1.0.2/PKG-INFO
+-rw-r--r--   0 coreylin   (501) staff       (20)     2035 2024-03-10 13:49:43.000000 baselib-1.1.0.2/README.md
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.508807 baselib-1.1.0.2/baselib/
+-rw-r--r--   0 coreylin   (501) staff       (20)        0 2023-02-04 13:19:24.000000 baselib-1.1.0.2/baselib/__init__.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.510125 baselib-1.1.0.2/baselib/channel/
+-rw-r--r--   0 coreylin   (501) staff       (20)       63 2024-03-10 12:54:47.000000 baselib-1.1.0.2/baselib/channel/__init__.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     3771 2024-03-10 12:53:35.000000 baselib-1.1.0.2/baselib/channel/base_channel.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.510571 baselib-1.1.0.2/baselib/demo/
+-rw-r--r--   0 coreylin   (501) staff       (20)       22 2023-02-04 13:19:24.000000 baselib-1.1.0.2/baselib/demo/__init__.py
+-rw-r--r--   0 coreylin   (501) staff       (20)       86 2023-02-04 13:19:24.000000 baselib-1.1.0.2/baselib/demo/demo.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.511042 baselib-1.1.0.2/baselib/feishu/
+-rw-r--r--   0 coreylin   (501) staff       (20)       44 2024-03-10 13:48:54.000000 baselib-1.1.0.2/baselib/feishu/__init__.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     5759 2024-03-10 13:48:18.000000 baselib-1.1.0.2/baselib/feishu/robot.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.511557 baselib-1.1.0.2/baselib/json/
+-rw-r--r--   0 coreylin   (501) staff       (20)       44 2023-04-05 13:59:51.000000 baselib-1.1.0.2/baselib/json/__init__.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     1804 2024-03-10 13:52:12.000000 baselib-1.1.0.2/baselib/json/json_file.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.512000 baselib-1.1.0.2/baselib/log/
+-rw-r--r--   0 coreylin   (501) staff       (20)       40 2023-04-05 13:59:51.000000 baselib-1.1.0.2/baselib/log/__init__.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     2219 2023-04-05 13:59:51.000000 baselib-1.1.0.2/baselib/log/file.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.512218 baselib-1.1.0.2/baselib/py/
+-rw-r--r--   0 coreylin   (501) staff       (20)      717 2024-03-10 13:49:43.000000 baselib-1.1.0.2/baselib/py/__init__.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.512726 baselib-1.1.0.2/baselib/qywx/
+-rw-r--r--   0 coreylin   (501) staff       (20)       38 2023-04-05 13:59:51.000000 baselib-1.1.0.2/baselib/qywx/__init__.py
+-rw-r--r--   0 coreylin   (501) staff       (20)    13625 2024-03-10 13:49:43.000000 baselib-1.1.0.2/baselib/qywx/qywx.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.513060 baselib-1.1.0.2/baselib/request/
+-rw-r--r--   0 coreylin   (501) staff       (20)        0 2023-04-03 14:48:56.000000 baselib-1.1.0.2/baselib/request/__init__.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.513157 baselib-1.1.0.2/baselib/system/
+-rw-r--r--   0 coreylin   (501) staff       (20)     3384 2024-03-10 13:49:43.000000 baselib-1.1.0.2/baselib/system/__init__.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.514776 baselib-1.1.0.2/baselib/tests/
+-rw-r--r--   0 coreylin   (501) staff       (20)        0 2023-02-04 13:19:24.000000 baselib-1.1.0.2/baselib/tests/__init__.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     4989 2023-04-03 14:50:20.000000 baselib-1.1.0.2/baselib/tests/debug.py
+-rw-r--r--   0 coreylin   (501) staff       (20)      126 2023-02-04 13:19:24.000000 baselib-1.1.0.2/baselib/tests/demo_test.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     1838 2024-03-10 13:49:43.000000 baselib-1.1.0.2/baselib/tests/file_logger_test.py
+-rw-r--r--   0 coreylin   (501) staff       (20)      494 2024-03-10 13:49:43.000000 baselib-1.1.0.2/baselib/tests/httplib_test.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     1122 2024-03-10 14:01:54.000000 baselib-1.1.0.2/baselib/tests/json_file_test.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     2800 2024-03-10 13:49:43.000000 baselib-1.1.0.2/baselib/tests/period_test.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     3154 2024-03-10 13:49:43.000000 baselib-1.1.0.2/baselib/tests/qywx_test.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.515290 baselib-1.1.0.2/baselib/time/
+-rw-r--r--   0 coreylin   (501) staff       (20)       39 2023-04-05 13:59:51.000000 baselib-1.1.0.2/baselib/time/__init__.py
+-rw-r--r--   0 coreylin   (501) staff       (20)     4480 2023-02-04 13:19:24.000000 baselib-1.1.0.2/baselib/time/period.py
+drwxr-xr-x   0 coreylin   (501) staff       (20)        0 2024-04-21 10:20:57.509618 baselib-1.1.0.2/baselib.egg-info/
+-rw-r--r--   0 coreylin   (501) staff       (20)     2326 2024-04-21 10:20:57.000000 baselib-1.1.0.2/baselib.egg-info/PKG-INFO
+-rw-r--r--   0 coreylin   (501) staff       (20)      852 2024-04-21 10:20:57.000000 baselib-1.1.0.2/baselib.egg-info/SOURCES.txt
+-rw-r--r--   0 coreylin   (501) staff       (20)        1 2024-04-21 10:20:57.000000 baselib-1.1.0.2/baselib.egg-info/dependency_links.txt
+-rw-r--r--   0 coreylin   (501) staff       (20)        1 2023-02-10 15:58:03.000000 baselib-1.1.0.2/baselib.egg-info/not-zip-safe
+-rw-r--r--   0 coreylin   (501) staff       (20)        8 2024-04-21 10:20:57.000000 baselib-1.1.0.2/baselib.egg-info/top_level.txt
+-rw-r--r--   0 coreylin   (501) staff       (20)       38 2024-04-21 10:20:57.515727 baselib-1.1.0.2/setup.cfg
+-rw-r--r--   0 coreylin   (501) staff       (20)      830 2024-04-21 10:20:32.000000 baselib-1.1.0.2/setup.py
```

### Comparing `baselib-1.1.0.1b0/LICENSE` & `baselib-1.1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.1b0/PKG-INFO` & `baselib-1.1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baselib
-Version: 1.1.0.1b0
+Version: 1.1.0.2
 Summary: base common lib for python
 Home-page: https://github.com/coreylam/base_common_lib
 Author: coreylam
 Author-email: coreylam@163.com
 License: GPL
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
```

### Comparing `baselib-1.1.0.1b0/README.md` & `baselib-1.1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.1b0/baselib/json/json_file.py` & `baselib-1.1.0.2/baselib/json/json_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,41 +3,44 @@
 """
 import os
 import json
 
 
 class JsonFile(object):
 
+    encoding = "utf-8"
+
     @classmethod
     def read(cls, file_path):
         """ 读取 文件路径为 $file_path 的 json 文件
         :param file_path: 文件路径，包括目录，名称，后缀
         :return:
             - 正常情况下，返回 json 文件
             - json 文件不存在，读取失败，以及内容为空时，返回 {}
         """
         if not os.path.isfile(file_path):
             return {}
         try:
-            with open(file_path, 'r') as fid:
+            with open(file_path, 'r', encoding=cls.encoding) as fid:
                 data = json.load(fid)
         except Exception:
             return {}
         return data
 
     @classmethod
     def write(cls, file_path, data, indent=None):
         """ 写入 文件路径为 $file_path 的 json 文件
         :param string file_path: 文件路径，包括目录，名称，后缀
         :param dict data: 要写入的数据
         :param int indent: json 格式对齐，默认为None，不做格式化
         :return: 实际写入的数据（即入参 data）
         """
         with open(file_path, 'w') as fid:
-            fid.writelines(json.dumps(data, indent=indent))
+            # fid.writelines(json.dumps(data, indent=indent))
+            json.dump(data, fid, indent=indent, ensure_ascii=False)
         return data
 
     @classmethod
     def update(cls, file_path, data, indent=None):
         """
         :param string file_path: 文件路径，包括目录，名称，后缀
         :param dict data: 要写入的数据
```

### Comparing `baselib-1.1.0.1b0/baselib/log/file.py` & `baselib-1.1.0.2/baselib/log/file.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.1b0/baselib/py/__init__.py` & `baselib-1.1.0.2/baselib/py/__init__.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.1b0/baselib/qywx/qywx.py` & `baselib-1.1.0.2/baselib/qywx/qywx.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.1b0/baselib/system/__init__.py` & `baselib-1.1.0.2/baselib/system/__init__.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.1b0/baselib/tests/debug.py` & `baselib-1.1.0.2/baselib/tests/debug.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.1b0/baselib/tests/file_logger_test.py` & `baselib-1.1.0.2/baselib/tests/file_logger_test.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.1b0/baselib/tests/period_test.py` & `baselib-1.1.0.2/baselib/tests/period_test.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.1b0/baselib/tests/qywx_test.py` & `baselib-1.1.0.2/baselib/tests/qywx_test.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.1b0/baselib/time/period.py` & `baselib-1.1.0.2/baselib/time/period.py`

 * *Files identical despite different names*

### Comparing `baselib-1.1.0.1b0/baselib.egg-info/PKG-INFO` & `baselib-1.1.0.2/baselib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baselib
-Version: 1.1.0.1b0
+Version: 1.1.0.2
 Summary: base common lib for python
 Home-page: https://github.com/coreylam/base_common_lib
 Author: coreylam
 Author-email: coreylam@163.com
 License: GPL
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
```

### Comparing `baselib-1.1.0.1b0/baselib.egg-info/SOURCES.txt` & `baselib-1.1.0.2/baselib.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 setup.py
 baselib/__init__.py
 baselib.egg-info/PKG-INFO
 baselib.egg-info/SOURCES.txt
 baselib.egg-info/dependency_links.txt
 baselib.egg-info/not-zip-safe
 baselib.egg-info/top_level.txt
+baselib/channel/__init__.py
+baselib/channel/base_channel.py
 baselib/demo/__init__.py
 baselib/demo/demo.py
+baselib/feishu/__init__.py
+baselib/feishu/robot.py
 baselib/json/__init__.py
 baselib/json/json_file.py
 baselib/log/__init__.py
 baselib/log/file.py
 baselib/py/__init__.py
 baselib/qywx/__init__.py
 baselib/qywx/qywx.py
```

### Comparing `baselib-1.1.0.1b0/setup.py` & `baselib-1.1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         with open(filename, "r") as fid:
             desc = fid.read()
     return desc
 
 
 setup(
     name='baselib',
-    version="1.1.0.1beta",
+    version="1.1.0.2",
     description='base common lib for python',
     long_description=read_desc(),
     long_description_content_type="text/markdown",
     author='coreylam',
     author_email='coreylam@163.com',
     url='https://github.com/coreylam/base_common_lib',
     license='GPL',
```


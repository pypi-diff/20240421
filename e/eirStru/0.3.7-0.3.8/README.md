# Comparing `tmp/eirStru-0.3.7.tar.gz` & `tmp/eirStru-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eirStru-0.3.7.tar", last modified: Sun Apr 21 17:23:11 2024, max compression
+gzip compressed data, was "eirStru-0.3.8.tar", last modified: Sun Apr 21 17:25:26 2024, max compression
```

## Comparing `eirStru-0.3.7.tar` & `eirStru-0.3.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 17:23:11.363615 eirStru-0.3.7/
--rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.3.7/LICENSE
--rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.3.7/MANIFEST.in
--rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 17:23:11.363382 eirStru-0.3.7/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.3.7/README.md
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 17:23:11.362680 eirStru-0.3.7/eirStru/
--rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.3.7/eirStru/__init__.py
--rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.3.7/eirStru/__version__.py
--rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.3.7/eirStru/aiomysql_helper.py
--rwxr--r--   0 wangwh     (501) staff       (20)    17768 2024-04-21 17:23:09.000000 eirStru-0.3.7/eirStru/common.py
--rw-r--r--   0 wangwh     (501) staff       (20)     4341 2024-04-19 09:06:12.000000 eirStru-0.3.7/eirStru/eirjob_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     6488 2024-04-19 09:06:12.000000 eirStru-0.3.7/eirStru/eirlogin_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.3.7/eirStru/redis_utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.3.7/eirStru/test.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1389 2024-04-18 23:20:17.000000 eirStru-0.3.7/eirStru/utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.3.7/eirStru/wx_push.py
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 17:23:11.363177 eirStru-0.3.7/eirStru.egg-info/
--rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 17:23:11.000000 eirStru-0.3.7/eirStru.egg-info/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-21 17:23:11.000000 eirStru-0.3.7/eirStru.egg-info/SOURCES.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-21 17:23:11.000000 eirStru-0.3.7/eirStru.egg-info/dependency_links.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-21 17:23:11.000000 eirStru-0.3.7/eirStru.egg-info/top_level.txt
--rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-21 17:23:11.363650 eirStru-0.3.7/setup.cfg
--rw-r--r--   0 wangwh     (501) staff       (20)     3776 2024-04-21 17:23:09.000000 eirStru-0.3.7/setup.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 17:25:26.552600 eirStru-0.3.8/
+-rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.3.8/LICENSE
+-rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.3.8/MANIFEST.in
+-rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 17:25:26.552342 eirStru-0.3.8/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.3.8/README.md
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 17:25:26.551733 eirStru-0.3.8/eirStru/
+-rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.3.8/eirStru/__init__.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.3.8/eirStru/__version__.py
+-rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.3.8/eirStru/aiomysql_helper.py
+-rwxr--r--   0 wangwh     (501) staff       (20)    17773 2024-04-21 17:25:16.000000 eirStru-0.3.8/eirStru/common.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     4341 2024-04-19 09:06:12.000000 eirStru-0.3.8/eirStru/eirjob_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     6488 2024-04-19 09:06:12.000000 eirStru-0.3.8/eirStru/eirlogin_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.3.8/eirStru/redis_utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.3.8/eirStru/test.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1389 2024-04-18 23:20:17.000000 eirStru-0.3.8/eirStru/utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.3.8/eirStru/wx_push.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 17:25:26.552154 eirStru-0.3.8/eirStru.egg-info/
+-rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 17:25:26.000000 eirStru-0.3.8/eirStru.egg-info/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-21 17:25:26.000000 eirStru-0.3.8/eirStru.egg-info/SOURCES.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-21 17:25:26.000000 eirStru-0.3.8/eirStru.egg-info/dependency_links.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-21 17:25:26.000000 eirStru-0.3.8/eirStru.egg-info/top_level.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-21 17:25:26.552642 eirStru-0.3.8/setup.cfg
+-rw-r--r--   0 wangwh     (501) staff       (20)     3776 2024-04-21 17:25:25.000000 eirStru-0.3.8/setup.py
```

### Comparing `eirStru-0.3.7/LICENSE` & `eirStru-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.7/PKG-INFO` & `eirStru-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.3.7
+Version: 0.3.8
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.3.7/README.md` & `eirStru-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.7/eirStru/aiomysql_helper.py` & `eirStru-0.3.8/eirStru/aiomysql_helper.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.7/eirStru/common.py` & `eirStru-0.3.8/eirStru/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
 
     ctntypedigit_list: List[CtnTypeDigit] = []  # eir订单箱型箱量
     is_canceled: bool = False
     is_disabled: bool = False
     is_completed: bool = False
 
     internal_ctns: List[CtnInfo] = []  # 集装箱列表
-    timestamp = 0  # 上一次执行时间
+    timestamp: int = 0  # 上一次执行时间
 
     def check_ctntype_id(self, ctntype_id, ctn_list):
         set1 = set(map(lambda ctn: ctn.ctntype_id, ctn_list))
         ctntypedigit_list = convert_ctntype_tolist(ctntype_id)
         set2 = set(map(lambda ctntypedigit: ctntypedigit.ctntype_id, ctntypedigit_list))
 
         if set2 - set1 and len(set1) == 1 and len(set2) == 1:
```

### Comparing `eirStru-0.3.7/eirStru/eirjob_intf.py` & `eirStru-0.3.8/eirStru/eirjob_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.7/eirStru/eirlogin_intf.py` & `eirStru-0.3.8/eirStru/eirlogin_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.7/eirStru/redis_utils.py` & `eirStru-0.3.8/eirStru/redis_utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.7/eirStru/utils.py` & `eirStru-0.3.8/eirStru/utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.7/eirStru/wx_push.py` & `eirStru-0.3.8/eirStru/wx_push.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.7/eirStru.egg-info/PKG-INFO` & `eirStru-0.3.8/eirStru.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.3.7
+Version: 0.3.8
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.3.7/setup.py` & `eirStru-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'eirStru'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'me@example.com'
 AUTHOR = 'Awesome Soul'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.3.7'
+VERSION = '0.3.8'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```


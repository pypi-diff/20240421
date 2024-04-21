# Comparing `tmp/eirStru-0.3.2.tar.gz` & `tmp/eirStru-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eirStru-0.3.2.tar", last modified: Fri Apr 19 12:07:31 2024, max compression
+gzip compressed data, was "eirStru-0.3.3.tar", last modified: Sun Apr 21 07:56:46 2024, max compression
```

## Comparing `eirStru-0.3.2.tar` & `eirStru-0.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-19 12:07:31.494986 eirStru-0.3.2/
--rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.3.2/LICENSE
--rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.3.2/MANIFEST.in
--rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-19 12:07:31.494714 eirStru-0.3.2/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.3.2/README.md
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-19 12:07:31.493916 eirStru-0.3.2/eirStru/
--rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.3.2/eirStru/__init__.py
--rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.3.2/eirStru/__version__.py
--rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.3.2/eirStru/aiomysql_helper.py
--rwxr--r--   0 wangwh     (501) staff       (20)    18324 2024-04-19 11:29:31.000000 eirStru-0.3.2/eirStru/common.py
--rw-r--r--   0 wangwh     (501) staff       (20)     4341 2024-04-19 09:06:12.000000 eirStru-0.3.2/eirStru/eirjob_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     6488 2024-04-19 09:06:12.000000 eirStru-0.3.2/eirStru/eirlogin_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.3.2/eirStru/redis_utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.3.2/eirStru/test.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1389 2024-04-18 23:20:17.000000 eirStru-0.3.2/eirStru/utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.3.2/eirStru/wx_push.py
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-19 12:07:31.494488 eirStru-0.3.2/eirStru.egg-info/
--rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-19 12:07:31.000000 eirStru-0.3.2/eirStru.egg-info/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-19 12:07:31.000000 eirStru-0.3.2/eirStru.egg-info/SOURCES.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-19 12:07:31.000000 eirStru-0.3.2/eirStru.egg-info/dependency_links.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-19 12:07:31.000000 eirStru-0.3.2/eirStru.egg-info/top_level.txt
--rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-19 12:07:31.495036 eirStru-0.3.2/setup.cfg
--rw-r--r--   0 wangwh     (501) staff       (20)     3776 2024-04-19 12:07:29.000000 eirStru-0.3.2/setup.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 07:56:46.547459 eirStru-0.3.3/
+-rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.3.3/LICENSE
+-rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.3.3/MANIFEST.in
+-rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 07:56:46.547172 eirStru-0.3.3/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.3.3/README.md
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 07:56:46.546315 eirStru-0.3.3/eirStru/
+-rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.3.3/eirStru/__init__.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.3.3/eirStru/__version__.py
+-rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.3.3/eirStru/aiomysql_helper.py
+-rwxr--r--   0 wangwh     (501) staff       (20)    18383 2024-04-21 07:50:15.000000 eirStru-0.3.3/eirStru/common.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     4341 2024-04-19 09:06:12.000000 eirStru-0.3.3/eirStru/eirjob_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     6488 2024-04-19 09:06:12.000000 eirStru-0.3.3/eirStru/eirlogin_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.3.3/eirStru/redis_utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.3.3/eirStru/test.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1389 2024-04-18 23:20:17.000000 eirStru-0.3.3/eirStru/utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.3.3/eirStru/wx_push.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 07:56:46.546946 eirStru-0.3.3/eirStru.egg-info/
+-rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 07:56:46.000000 eirStru-0.3.3/eirStru.egg-info/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-21 07:56:46.000000 eirStru-0.3.3/eirStru.egg-info/SOURCES.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-21 07:56:46.000000 eirStru-0.3.3/eirStru.egg-info/dependency_links.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-21 07:56:46.000000 eirStru-0.3.3/eirStru.egg-info/top_level.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-21 07:56:46.547503 eirStru-0.3.3/setup.cfg
+-rw-r--r--   0 wangwh     (501) staff       (20)     3776 2024-04-21 07:56:42.000000 eirStru-0.3.3/setup.py
```

### Comparing `eirStru-0.3.2/LICENSE` & `eirStru-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.2/PKG-INFO` & `eirStru-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.3.2
+Version: 0.3.3
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.3.2/README.md` & `eirStru-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.2/eirStru/aiomysql_helper.py` & `eirStru-0.3.3/eirStru/aiomysql_helper.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.2/eirStru/common.py` & `eirStru-0.3.3/eirStru/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,15 @@
     ctntype_id: Optional[str] = None  # 箱型
     ctn_digit: Optional[int] = 0  # 箱量
     ctn_digit_applied: Optional[int] = 0  # 已申请量
     ctn_digit_printed: Optional[int] = 0  # 已打印量
     ctn_digit_for_apply: Optional[int] = 0  # 可申请量，未申请
     ctn_digit_for_print: Optional[int] = 0  # 可打印量，已申请未打印
     ctn_digit_need_apply: Optional[int] = 0  # 总申请量,订单传过来的，
+    ctn_list_count: Optional[int] = 0 # 集装箱列表量
     yard_info: Optional[Dict] = {}  # 用于msk，指定堆场
 
     # 总申请量>0 本次需申请量=总申请量-已申请量, 总申请量=0 本次申请量=箱量-可打印量
     # 本次打印量=min(可打印量,箱量)
     def __str__(self):
         return f'{self.ctn_digit}x{self.ctntype_id.upper()}'
```

### Comparing `eirStru-0.3.2/eirStru/eirjob_intf.py` & `eirStru-0.3.3/eirStru/eirjob_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.2/eirStru/eirlogin_intf.py` & `eirStru-0.3.3/eirStru/eirlogin_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.2/eirStru/redis_utils.py` & `eirStru-0.3.3/eirStru/redis_utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.2/eirStru/utils.py` & `eirStru-0.3.3/eirStru/utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.2/eirStru/wx_push.py` & `eirStru-0.3.3/eirStru/wx_push.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.2/eirStru.egg-info/PKG-INFO` & `eirStru-0.3.3/eirStru.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.3.2
+Version: 0.3.3
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.3.2/setup.py` & `eirStru-0.3.3/setup.py`

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
-VERSION = '0.3.2'
+VERSION = '0.3.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```


# Comparing `tmp/eirStru-0.3.4.tar.gz` & `tmp/eirStru-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eirStru-0.3.4.tar", last modified: Sun Apr 21 08:00:21 2024, max compression
+gzip compressed data, was "eirStru-0.3.5.tar", last modified: Sun Apr 21 08:23:36 2024, max compression
```

## Comparing `eirStru-0.3.4.tar` & `eirStru-0.3.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 08:00:21.686451 eirStru-0.3.4/
--rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.3.4/LICENSE
--rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.3.4/MANIFEST.in
--rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 08:00:21.686189 eirStru-0.3.4/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.3.4/README.md
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 08:00:21.685482 eirStru-0.3.4/eirStru/
--rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.3.4/eirStru/__init__.py
--rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.3.4/eirStru/__version__.py
--rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.3.4/eirStru/aiomysql_helper.py
--rwxr--r--   0 wangwh     (501) staff       (20)    18127 2024-04-21 07:59:59.000000 eirStru-0.3.4/eirStru/common.py
--rw-r--r--   0 wangwh     (501) staff       (20)     4341 2024-04-19 09:06:12.000000 eirStru-0.3.4/eirStru/eirjob_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     6488 2024-04-19 09:06:12.000000 eirStru-0.3.4/eirStru/eirlogin_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.3.4/eirStru/redis_utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.3.4/eirStru/test.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1389 2024-04-18 23:20:17.000000 eirStru-0.3.4/eirStru/utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.3.4/eirStru/wx_push.py
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 08:00:21.685948 eirStru-0.3.4/eirStru.egg-info/
--rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 08:00:21.000000 eirStru-0.3.4/eirStru.egg-info/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-21 08:00:21.000000 eirStru-0.3.4/eirStru.egg-info/SOURCES.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-21 08:00:21.000000 eirStru-0.3.4/eirStru.egg-info/dependency_links.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-21 08:00:21.000000 eirStru-0.3.4/eirStru.egg-info/top_level.txt
--rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-21 08:00:21.686500 eirStru-0.3.4/setup.cfg
--rw-r--r--   0 wangwh     (501) staff       (20)     3776 2024-04-21 08:00:19.000000 eirStru-0.3.4/setup.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 08:23:36.677154 eirStru-0.3.5/
+-rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.3.5/LICENSE
+-rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.3.5/MANIFEST.in
+-rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 08:23:36.676922 eirStru-0.3.5/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.3.5/README.md
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 08:23:36.676256 eirStru-0.3.5/eirStru/
+-rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.3.5/eirStru/__init__.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.3.5/eirStru/__version__.py
+-rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.3.5/eirStru/aiomysql_helper.py
+-rwxr--r--   0 wangwh     (501) staff       (20)    18306 2024-04-21 08:23:34.000000 eirStru-0.3.5/eirStru/common.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     4341 2024-04-19 09:06:12.000000 eirStru-0.3.5/eirStru/eirjob_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     6488 2024-04-19 09:06:12.000000 eirStru-0.3.5/eirStru/eirlogin_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.3.5/eirStru/redis_utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.3.5/eirStru/test.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1389 2024-04-18 23:20:17.000000 eirStru-0.3.5/eirStru/utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.3.5/eirStru/wx_push.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 08:23:36.676712 eirStru-0.3.5/eirStru.egg-info/
+-rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 08:23:36.000000 eirStru-0.3.5/eirStru.egg-info/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-21 08:23:36.000000 eirStru-0.3.5/eirStru.egg-info/SOURCES.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-21 08:23:36.000000 eirStru-0.3.5/eirStru.egg-info/dependency_links.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-21 08:23:36.000000 eirStru-0.3.5/eirStru.egg-info/top_level.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-21 08:23:36.677205 eirStru-0.3.5/setup.cfg
+-rw-r--r--   0 wangwh     (501) staff       (20)     3776 2024-04-21 08:23:34.000000 eirStru-0.3.5/setup.py
```

### Comparing `eirStru-0.3.4/LICENSE` & `eirStru-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.4/PKG-INFO` & `eirStru-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.3.4
+Version: 0.3.5
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.3.4/README.md` & `eirStru-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.4/eirStru/aiomysql_helper.py` & `eirStru-0.3.5/eirStru/aiomysql_helper.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.4/eirStru/common.py` & `eirStru-0.3.5/eirStru/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     ctntype_id: Optional[str] = None  # 箱型
     ctn_digit: Optional[int] = 0  # 箱量
     ctn_digit_applied: Optional[int] = 0  # 已申请量
     ctn_digit_printed: Optional[int] = 0  # 已打印量
     ctn_digit_for_apply: Optional[int] = 0  # 可申请量，未申请
     ctn_digit_for_print: Optional[int] = 0  # 可打印量，已申请未打印
     ctn_digit_need_apply: Optional[int] = 0  # 总申请量,订单传过来的，
-    ctn_list_count: Optional[int] = 0 # 集装箱列表量
+    ctn_list_count: Optional[int] = 0  # 集装箱列表量
 
     # 总申请量>0 本次需申请量=总申请量-已申请量, 总申请量=0 本次申请量=箱量-可打印量
     # 本次打印量=min(可打印量,箱量)
     def __str__(self):
         return f'{self.ctn_digit}x{self.ctntype_id.upper()}'
 
 
@@ -317,16 +317,20 @@
         for item in ctntypedigit_dict.values():
             item.ctn_digit = item.ctn_digit or item.ctn_list_count
 
             # 本次打印量=min(已申请量-已打印量,箱量)
             item.ctn_digit_for_print = min(item.ctn_digit_applied - item.ctn_digit_printed, item.ctn_digit)
 
             # 总申请量=0 本次申请量=箱量-可打印量
-            if item.ctn_digit_need_apply == 0 and item.ctn_digit > item.ctn_digit_applied - item.ctn_digit_printed:
-                item.ctn_digit_for_apply = item.ctn_digit - item.ctn_digit_applied + item.ctn_digit_printed
+            if item.ctn_digit_need_apply == 0:
+                if self.ctntype_id:
+                    if item.ctn_digit > item.ctn_digit_applied - item.ctn_digit_printed:
+                        item.ctn_digit_for_apply = item.ctn_digit - item.ctn_digit_applied + item.ctn_digit_printed
+                else:
+                    item.ctn_digit_for_apply = item.ctn_list_count - item.ctn_digit_applied
             # 总申请量>0 本次需申请量=总申请量-已申请量
             elif item.ctn_digit_need_apply > item.ctn_digit_applied:
                 item.ctn_digit_for_apply = item.ctn_digit_need_apply - item.ctn_digit_applied
 
         self.ctntypedigit_list = list(ctntypedigit_dict.values())
 
     @property
```

### Comparing `eirStru-0.3.4/eirStru/eirjob_intf.py` & `eirStru-0.3.5/eirStru/eirjob_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.4/eirStru/eirlogin_intf.py` & `eirStru-0.3.5/eirStru/eirlogin_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.4/eirStru/redis_utils.py` & `eirStru-0.3.5/eirStru/redis_utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.4/eirStru/utils.py` & `eirStru-0.3.5/eirStru/utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.4/eirStru/wx_push.py` & `eirStru-0.3.5/eirStru/wx_push.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.4/eirStru.egg-info/PKG-INFO` & `eirStru-0.3.5/eirStru.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.3.4
+Version: 0.3.5
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.3.4/setup.py` & `eirStru-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'eirStru'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'me@example.com'
 AUTHOR = 'Awesome Soul'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.3.4'
+VERSION = '0.3.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```


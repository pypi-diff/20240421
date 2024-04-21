# Comparing `tmp/eirStru-0.3.3.tar.gz` & `tmp/eirStru-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eirStru-0.3.3.tar", last modified: Sun Apr 21 07:56:46 2024, max compression
+gzip compressed data, was "eirStru-0.3.4.tar", last modified: Sun Apr 21 08:00:21 2024, max compression
```

## Comparing `eirStru-0.3.3.tar` & `eirStru-0.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 07:56:46.547459 eirStru-0.3.3/
--rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.3.3/LICENSE
--rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.3.3/MANIFEST.in
--rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 07:56:46.547172 eirStru-0.3.3/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.3.3/README.md
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 07:56:46.546315 eirStru-0.3.3/eirStru/
--rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.3.3/eirStru/__init__.py
--rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.3.3/eirStru/__version__.py
--rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.3.3/eirStru/aiomysql_helper.py
--rwxr--r--   0 wangwh     (501) staff       (20)    18383 2024-04-21 07:50:15.000000 eirStru-0.3.3/eirStru/common.py
--rw-r--r--   0 wangwh     (501) staff       (20)     4341 2024-04-19 09:06:12.000000 eirStru-0.3.3/eirStru/eirjob_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     6488 2024-04-19 09:06:12.000000 eirStru-0.3.3/eirStru/eirlogin_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.3.3/eirStru/redis_utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.3.3/eirStru/test.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1389 2024-04-18 23:20:17.000000 eirStru-0.3.3/eirStru/utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.3.3/eirStru/wx_push.py
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 07:56:46.546946 eirStru-0.3.3/eirStru.egg-info/
--rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 07:56:46.000000 eirStru-0.3.3/eirStru.egg-info/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-21 07:56:46.000000 eirStru-0.3.3/eirStru.egg-info/SOURCES.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-21 07:56:46.000000 eirStru-0.3.3/eirStru.egg-info/dependency_links.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-21 07:56:46.000000 eirStru-0.3.3/eirStru.egg-info/top_level.txt
--rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-21 07:56:46.547503 eirStru-0.3.3/setup.cfg
--rw-r--r--   0 wangwh     (501) staff       (20)     3776 2024-04-21 07:56:42.000000 eirStru-0.3.3/setup.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 08:00:21.686451 eirStru-0.3.4/
+-rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.3.4/LICENSE
+-rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.3.4/MANIFEST.in
+-rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 08:00:21.686189 eirStru-0.3.4/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.3.4/README.md
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 08:00:21.685482 eirStru-0.3.4/eirStru/
+-rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.3.4/eirStru/__init__.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.3.4/eirStru/__version__.py
+-rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.3.4/eirStru/aiomysql_helper.py
+-rwxr--r--   0 wangwh     (501) staff       (20)    18127 2024-04-21 07:59:59.000000 eirStru-0.3.4/eirStru/common.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     4341 2024-04-19 09:06:12.000000 eirStru-0.3.4/eirStru/eirjob_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     6488 2024-04-19 09:06:12.000000 eirStru-0.3.4/eirStru/eirlogin_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.3.4/eirStru/redis_utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.3.4/eirStru/test.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1389 2024-04-18 23:20:17.000000 eirStru-0.3.4/eirStru/utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.3.4/eirStru/wx_push.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 08:00:21.685948 eirStru-0.3.4/eirStru.egg-info/
+-rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 08:00:21.000000 eirStru-0.3.4/eirStru.egg-info/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-21 08:00:21.000000 eirStru-0.3.4/eirStru.egg-info/SOURCES.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-21 08:00:21.000000 eirStru-0.3.4/eirStru.egg-info/dependency_links.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-21 08:00:21.000000 eirStru-0.3.4/eirStru.egg-info/top_level.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-21 08:00:21.686500 eirStru-0.3.4/setup.cfg
+-rw-r--r--   0 wangwh     (501) staff       (20)     3776 2024-04-21 08:00:19.000000 eirStru-0.3.4/setup.py
```

### Comparing `eirStru-0.3.3/LICENSE` & `eirStru-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.3/PKG-INFO` & `eirStru-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.3.3
+Version: 0.3.4
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.3.3/README.md` & `eirStru-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.3/eirStru/aiomysql_helper.py` & `eirStru-0.3.4/eirStru/aiomysql_helper.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.3/eirStru/common.py` & `eirStru-0.3.4/eirStru/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,14 @@
     ctn_digit: Optional[int] = 0  # 箱量
     ctn_digit_applied: Optional[int] = 0  # 已申请量
     ctn_digit_printed: Optional[int] = 0  # 已打印量
     ctn_digit_for_apply: Optional[int] = 0  # 可申请量，未申请
     ctn_digit_for_print: Optional[int] = 0  # 可打印量，已申请未打印
     ctn_digit_need_apply: Optional[int] = 0  # 总申请量,订单传过来的，
     ctn_list_count: Optional[int] = 0 # 集装箱列表量
-    yard_info: Optional[Dict] = {}  # 用于msk，指定堆场
 
     # 总申请量>0 本次需申请量=总申请量-已申请量, 总申请量=0 本次申请量=箱量-可打印量
     # 本次打印量=min(可打印量,箱量)
     def __str__(self):
         return f'{self.ctn_digit}x{self.ctntype_id.upper()}'
 
 
@@ -309,32 +308,28 @@
                 ctntypedigit = CtnTypeDigit()
                 ctntypedigit.ctntype_id = ctn.ctntype_id
                 ctntypedigit_dict.update({ctn.ctntype_id: ctntypedigit})
             if ctn.is_applied:
                 ctntypedigit.ctn_digit_applied += 1
             if ctn.is_printed:
                 ctntypedigit.ctn_digit_printed += 1
+            ctntypedigit.ctn_list_count += 1
 
         for item in ctntypedigit_dict.values():
+            item.ctn_digit = item.ctn_digit or item.ctn_list_count
 
-            # 整单模式,不需要申请
-            if not self.ctntype_id:
-                item.ctn_digit_for_print = item.ctn_digit_applied - item.ctn_digit_printed
-                item.ctn_digit_need_apply = 0
-            # 指定箱型箱量模式
-            else:
-                # 本次打印量=min(已申请量-已打印量,箱量)
-                item.ctn_digit_for_print = min(item.ctn_digit_applied - item.ctn_digit_printed, item.ctn_digit)
-
-                # 总申请量=0 本次申请量=箱量-可打印量
-                if item.ctn_digit_need_apply == 0 and item.ctn_digit > item.ctn_digit_applied - item.ctn_digit_printed:
-                    item.ctn_digit_for_apply = item.ctn_digit - item.ctn_digit_applied + item.ctn_digit_printed
-                # 总申请量>0 本次需申请量=总申请量-已申请量
-                elif item.ctn_digit_need_apply > item.ctn_digit_applied:
-                    item.ctn_digit_for_apply = item.ctn_digit_need_apply - item.ctn_digit_applied
+            # 本次打印量=min(已申请量-已打印量,箱量)
+            item.ctn_digit_for_print = min(item.ctn_digit_applied - item.ctn_digit_printed, item.ctn_digit)
+
+            # 总申请量=0 本次申请量=箱量-可打印量
+            if item.ctn_digit_need_apply == 0 and item.ctn_digit > item.ctn_digit_applied - item.ctn_digit_printed:
+                item.ctn_digit_for_apply = item.ctn_digit - item.ctn_digit_applied + item.ctn_digit_printed
+            # 总申请量>0 本次需申请量=总申请量-已申请量
+            elif item.ctn_digit_need_apply > item.ctn_digit_applied:
+                item.ctn_digit_for_apply = item.ctn_digit_need_apply - item.ctn_digit_applied
 
         self.ctntypedigit_list = list(ctntypedigit_dict.values())
 
     @property
     def status(self) -> BillStatus:
         if self.is_canceled or self.is_canceled:
             return BillStatus.canceled
```

### Comparing `eirStru-0.3.3/eirStru/eirjob_intf.py` & `eirStru-0.3.4/eirStru/eirjob_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.3/eirStru/eirlogin_intf.py` & `eirStru-0.3.4/eirStru/eirlogin_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.3/eirStru/redis_utils.py` & `eirStru-0.3.4/eirStru/redis_utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.3/eirStru/utils.py` & `eirStru-0.3.4/eirStru/utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.3/eirStru/wx_push.py` & `eirStru-0.3.4/eirStru/wx_push.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.3/eirStru.egg-info/PKG-INFO` & `eirStru-0.3.4/eirStru.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.3.3
+Version: 0.3.4
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.3.3/setup.py` & `eirStru-0.3.4/setup.py`

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
-VERSION = '0.3.3'
+VERSION = '0.3.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```


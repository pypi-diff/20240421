# Comparing `tmp/eirStru-0.3.5.tar.gz` & `tmp/eirStru-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eirStru-0.3.5.tar", last modified: Sun Apr 21 08:23:36 2024, max compression
+gzip compressed data, was "eirStru-0.3.6.tar", last modified: Sun Apr 21 12:31:43 2024, max compression
```

## Comparing `eirStru-0.3.5.tar` & `eirStru-0.3.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 08:23:36.677154 eirStru-0.3.5/
--rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.3.5/LICENSE
--rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.3.5/MANIFEST.in
--rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 08:23:36.676922 eirStru-0.3.5/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.3.5/README.md
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 08:23:36.676256 eirStru-0.3.5/eirStru/
--rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.3.5/eirStru/__init__.py
--rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.3.5/eirStru/__version__.py
--rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.3.5/eirStru/aiomysql_helper.py
--rwxr--r--   0 wangwh     (501) staff       (20)    18306 2024-04-21 08:23:34.000000 eirStru-0.3.5/eirStru/common.py
--rw-r--r--   0 wangwh     (501) staff       (20)     4341 2024-04-19 09:06:12.000000 eirStru-0.3.5/eirStru/eirjob_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     6488 2024-04-19 09:06:12.000000 eirStru-0.3.5/eirStru/eirlogin_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.3.5/eirStru/redis_utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.3.5/eirStru/test.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1389 2024-04-18 23:20:17.000000 eirStru-0.3.5/eirStru/utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.3.5/eirStru/wx_push.py
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 08:23:36.676712 eirStru-0.3.5/eirStru.egg-info/
--rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 08:23:36.000000 eirStru-0.3.5/eirStru.egg-info/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-21 08:23:36.000000 eirStru-0.3.5/eirStru.egg-info/SOURCES.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-21 08:23:36.000000 eirStru-0.3.5/eirStru.egg-info/dependency_links.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-21 08:23:36.000000 eirStru-0.3.5/eirStru.egg-info/top_level.txt
--rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-21 08:23:36.677205 eirStru-0.3.5/setup.cfg
--rw-r--r--   0 wangwh     (501) staff       (20)     3776 2024-04-21 08:23:34.000000 eirStru-0.3.5/setup.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 12:31:43.421488 eirStru-0.3.6/
+-rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.3.6/LICENSE
+-rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.3.6/MANIFEST.in
+-rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 12:31:43.421116 eirStru-0.3.6/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.3.6/README.md
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 12:31:43.420144 eirStru-0.3.6/eirStru/
+-rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.3.6/eirStru/__init__.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.3.6/eirStru/__version__.py
+-rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.3.6/eirStru/aiomysql_helper.py
+-rwxr--r--   0 wangwh     (501) staff       (20)    17725 2024-04-21 12:31:39.000000 eirStru-0.3.6/eirStru/common.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     4341 2024-04-19 09:06:12.000000 eirStru-0.3.6/eirStru/eirjob_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     6488 2024-04-19 09:06:12.000000 eirStru-0.3.6/eirStru/eirlogin_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.3.6/eirStru/redis_utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.3.6/eirStru/test.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1389 2024-04-18 23:20:17.000000 eirStru-0.3.6/eirStru/utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.3.6/eirStru/wx_push.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-21 12:31:43.420879 eirStru-0.3.6/eirStru.egg-info/
+-rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-21 12:31:43.000000 eirStru-0.3.6/eirStru.egg-info/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-21 12:31:43.000000 eirStru-0.3.6/eirStru.egg-info/SOURCES.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-21 12:31:43.000000 eirStru-0.3.6/eirStru.egg-info/dependency_links.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-21 12:31:43.000000 eirStru-0.3.6/eirStru.egg-info/top_level.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-21 12:31:43.421563 eirStru-0.3.6/setup.cfg
+-rw-r--r--   0 wangwh     (501) staff       (20)     3776 2024-04-21 12:31:39.000000 eirStru-0.3.6/setup.py
```

### Comparing `eirStru-0.3.5/LICENSE` & `eirStru-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.5/PKG-INFO` & `eirStru-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.3.5
+Version: 0.3.6
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.3.5/README.md` & `eirStru-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.5/eirStru/aiomysql_helper.py` & `eirStru-0.3.6/eirStru/aiomysql_helper.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.5/eirStru/common.py` & `eirStru-0.3.6/eirStru/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,14 @@
 
     bill_info = 1  # 提单信息
     ctn_list = 2  # 集装箱列表
     apply_eir = 3  # 申请条码
     print_eir = 4  # 打印条码
 
 
-class BillStatus(Enum):
-    canceled = -1  # 已取消
-    unknown = 0  # 未知
-    inited = 1  # 已订舱
-    applied = 2  # 已申请
-    printed = 3  # 已打印
-
-
 def get_f_time(action):
     if action == ActionType.bill_info:
         return 'last_bill_info_time'
     elif action == ActionType.ctn_list:
         return 'last_ctn_list_time'
     elif action == ActionType.apply_eir:
         return 'last_apply_eir_time'
@@ -63,18 +55,19 @@
     响应类
     """
     code: Optional[RespType] = None
     msg: Optional[str] = ''
     data: Optional[Any] = None  # 转换后的数据
     response: Optional[Any] = None  # 原始响应
     log: Optional[bool] = False  # 是否打印日志
+    action: Optional[ActionType] = None  # 动作类型
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        if (self.msg or self.data):
+        if self.msg or self.data:
             if self.code == RespType.task_success:
                 logger.warning(f'{self.msg} {self.data if self.data else ""}')
             elif self.code == RespType.task_failed:
                 logger.error(f'{self.msg} {self.data if self.data else ""}')
             else:
                 logger.info(f'{self.msg} {self.data if self.data else ""}')
 
@@ -329,27 +322,14 @@
                     item.ctn_digit_for_apply = item.ctn_list_count - item.ctn_digit_applied
             # 总申请量>0 本次需申请量=总申请量-已申请量
             elif item.ctn_digit_need_apply > item.ctn_digit_applied:
                 item.ctn_digit_for_apply = item.ctn_digit_need_apply - item.ctn_digit_applied
 
         self.ctntypedigit_list = list(ctntypedigit_dict.values())
 
-    @property
-    def status(self) -> BillStatus:
-        if self.is_canceled or self.is_canceled:
-            return BillStatus.canceled
-        elif not self.bill_info or not self.bill_info.voyage:
-            return BillStatus.unknown
-        elif self.ctns and self.ctns_for_print():
-            return BillStatus.printed
-        elif self.ctns and self.ctns_for_apply():
-            return BillStatus.applied
-        else:
-            return BillStatus.inited
-
     def check_completed(self):
         """
         不需要申请，不需要打印
         """
         return not (self.need_apply or self.need_print)
 
     def ctns_for_apply(self):
```

### Comparing `eirStru-0.3.5/eirStru/eirjob_intf.py` & `eirStru-0.3.6/eirStru/eirjob_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.5/eirStru/eirlogin_intf.py` & `eirStru-0.3.6/eirStru/eirlogin_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.5/eirStru/redis_utils.py` & `eirStru-0.3.6/eirStru/redis_utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.5/eirStru/utils.py` & `eirStru-0.3.6/eirStru/utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.5/eirStru/wx_push.py` & `eirStru-0.3.6/eirStru/wx_push.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.5/eirStru.egg-info/PKG-INFO` & `eirStru-0.3.6/eirStru.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.3.5
+Version: 0.3.6
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.3.5/setup.py` & `eirStru-0.3.6/setup.py`

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
-VERSION = '0.3.5'
+VERSION = '0.3.6'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```


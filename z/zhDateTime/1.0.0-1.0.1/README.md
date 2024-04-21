# Comparing `tmp/zhdatetime-1.0.0.tar.gz` & `tmp/zhdatetime-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhdatetime-1.0.0.tar", last modified: Sun Apr 21 06:38:12 2024, max compression
+gzip compressed data, was "zhdatetime-1.0.1.tar", last modified: Sun Apr 21 09:15:38 2024, max compression
```

## Comparing `zhdatetime-1.0.0.tar` & `zhdatetime-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 06:38:12.828296 zhdatetime-1.0.0/
--rw-rw-rw-   0        0        0    17098 2024-04-04 07:00:32.000000 zhdatetime-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       41 2023-11-18 16:11:48.000000 zhdatetime-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5776 2024-04-21 06:38:12.825305 zhdatetime-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5258 2024-04-21 05:29:41.000000 zhdatetime-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-21 06:38:12.829293 zhdatetime-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      764 2024-04-21 06:37:26.000000 zhdatetime-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 06:38:12.802288 zhdatetime-1.0.0/zhDateTime/
--rw-rw-rw-   0        0        0     1737 2024-04-21 05:25:06.000000 zhdatetime-1.0.0/zhDateTime/__init__.py
--rw-rw-rw-   0        0        0     4455 2024-04-21 05:23:15.000000 zhdatetime-1.0.0/zhDateTime/constants.py
--rw-rw-rw-   0        0        0    23578 2024-04-21 05:03:37.000000 zhdatetime-1.0.0/zhDateTime/main.py
--rw-rw-rw-   0        0        0     1664 2024-04-20 17:40:06.000000 zhdatetime-1.0.0/zhDateTime/types.py
-drwxrwxrwx   0        0        0        0 2024-04-21 06:38:12.822295 zhdatetime-1.0.0/zhDateTime.egg-info/
--rw-rw-rw-   0        0        0     5776 2024-04-21 06:38:12.000000 zhdatetime-1.0.0/zhDateTime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-04-21 06:38:12.000000 zhdatetime-1.0.0/zhDateTime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 06:38:12.000000 zhdatetime-1.0.0/zhDateTime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-21 06:38:12.000000 zhdatetime-1.0.0/zhDateTime.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 09:15:38.661533 zhdatetime-1.0.1/
+-rw-rw-rw-   0        0        0    17098 2024-04-04 07:00:32.000000 zhdatetime-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       41 2023-11-18 16:11:48.000000 zhdatetime-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5773 2024-04-21 09:15:38.658536 zhdatetime-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5255 2024-04-21 07:38:14.000000 zhdatetime-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-21 09:15:38.662519 zhdatetime-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      764 2024-04-21 06:37:26.000000 zhdatetime-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:15:38.639516 zhdatetime-1.0.1/zhDateTime/
+-rw-rw-rw-   0        0        0     1737 2024-04-21 09:14:03.000000 zhdatetime-1.0.1/zhDateTime/__init__.py
+-rw-rw-rw-   0        0        0     4455 2024-04-21 05:23:15.000000 zhdatetime-1.0.1/zhDateTime/constants.py
+-rw-rw-rw-   0        0        0    23554 2024-04-21 09:09:16.000000 zhdatetime-1.0.1/zhDateTime/main.py
+-rw-rw-rw-   0        0        0     1664 2024-04-20 17:40:06.000000 zhdatetime-1.0.1/zhDateTime/types.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:15:38.656590 zhdatetime-1.0.1/zhDateTime.egg-info/
+-rw-rw-rw-   0        0        0     5773 2024-04-21 09:15:38.000000 zhdatetime-1.0.1/zhDateTime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-04-21 09:15:38.000000 zhdatetime-1.0.1/zhDateTime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 09:15:38.000000 zhdatetime-1.0.1/zhDateTime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-21 09:15:38.000000 zhdatetime-1.0.1/zhDateTime.egg-info/top_level.txt
```

### Comparing `zhdatetime-1.0.0/LICENSE` & `zhdatetime-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zhdatetime-1.0.0/PKG-INFO` & `zhdatetime-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhDateTime
-Version: 1.0.0
+Version: 1.0.1
 Summary: 一个简单的小巧的中式日期时间库，附带数字汉字化操作。
 Home-page: https://gitee.com/EillesWan/zhDateTime
 Author: Eilles Wan
 Author-email: EillesWan@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 简易 Python 中式日期时间库
 
 ### 简介
 
-一个简单的小巧的轻量级中式日期时间库，支持农历公历互相转换，支持时辰刻数的时间表达转换，支持整数汉字化。
+一个简单小巧的轻量级中式日期时间库，支持农历公历互相转换，支持时辰刻数的时间表达转换，支持整数汉字化。
 
 ### 用法
 
 1.  农历与公历
 
 ```python
 from zhDateTime import DateTime,zhDateTime
```

### Comparing `zhdatetime-1.0.0/README.md` & `zhdatetime-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # 简易 Python 中式日期时间库
 
 ### 简介
 
-一个简单的小巧的轻量级中式日期时间库，支持农历公历互相转换，支持时辰刻数的时间表达转换，支持整数汉字化。
+一个简单小巧的轻量级中式日期时间库，支持农历公历互相转换，支持时辰刻数的时间表达转换，支持整数汉字化。
 
 ### 用法
 
 1.  农历与公历
 
 ```python
 from zhDateTime import DateTime,zhDateTime
```

### Comparing `zhdatetime-1.0.0/setup.py` & `zhdatetime-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `zhdatetime-1.0.0/zhDateTime/__init__.py` & `zhdatetime-1.0.1/zhDateTime/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Copyright (R) 2024 Eilles Wan
 
 This Source Code Form is subject to the terms of the Mozilla Public
 License, v. 2.0. If a copy of the MPL was not distributed with this
 file, You can obtain one at http://mozilla.org/MPL/2.0/.
 """
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __all__ = [
     # 所用之函数
     "shichen_ke_2_hour_minute",
     "hour_minute_2_shichen_ke",
     "get_lunar_month_list",
     "get_lunar_new_year",
     "verify_lunar_date",
```

### Comparing `zhdatetime-1.0.0/zhDateTime/constants.py` & `zhdatetime-1.0.1/zhDateTime/constants.py`

 * *Files identical despite different names*

### Comparing `zhdatetime-1.0.0/zhDateTime/main.py` & `zhdatetime-1.0.1/zhDateTime/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         month_code: int 当月月份信息，为16位整数数据，其末12位当为一年的大小月排布信息
         leap_days: int 当年闰月之天数，若为0则无闰
 
     返回值
     ------
         Tuple(List[int当月天数, ]当年每月天数, int闰月之月份, )当年每月天数列表及闰月月份
     """
-    leap_month = month_code & 0b1111000000000000
+    leap_month = (month_code & 0b1111000000000000) >> 12
     return (
         [month_days_pusher(month_code, i) for i in range(leap_month)][::-1]
         + [
             leap_days,
         ]
         + [month_days_pusher(month_code, i) for i in range(leap_month, 12)][::-1]
         if leap_month
@@ -176,60 +176,68 @@
 
 返回值
 ------
     Tuple(List[int当月天数, ]当年每月天数, int闰月之月份, )当年每月天数列表及闰月月份
 """
 
 
-verify_lunar_date: Callable[[int, int, bool, int], Tuple[bool, int, int]] = (
-    lambda lunar_year, lunar_month, is_leap, lunar_day: (
-        (
-            (1900 <= lunar_year <= 2100)  # 确认年份范围
-            and (1 <= lunar_month <= 12)  # 确认月份范围
-            and (
-                (  # 当为闰月时
-                    1
-                    <= lunar_day
-                    <= (leap_days := get_lunar_leap_size(lunar_year))  # 获取闰月日数
-                    and (
-                        lunar_month
-                        == (lunar_month_code := get_lunar_month_code(lunar_year))
-                    )  # 确认此月闰月与否
-                )
-                if is_leap
-                else (  # 当非闰月时，确认日期范围
-                    (leap_days := 0)  # 非闰月的闰月日期数位0
-                    < lunar_day
-                    <= (  # 获取当月日数
-                        month_days_pusher(
-                            (lunar_month_code := get_lunar_month_code(lunar_year)),
-                            lunar_month,
-                        )
+def verify_lunar_date(
+    lunar_year: int, lunar_month: int, is_leap: bool, lunar_day: int
+) -> Tuple[
+    bool,
+    List[int],
+    int,
+]:
+    """
+    检查所给出之农历日期是否符合本库之可用性
+
+    参数
+    ----
+        lunar_year: int 农历年份
+        lunar_month: int 农历月份
+        is_leap: bool 当月是否为闰月
+        lunar_day: int 当月天数
+
+    返回值
+    ------
+        Tuple(bool该日期是否可用, List[int]每月天数, int闰月月份)
+    """
+    lunar_month_data = None
+    verify_result = (
+        (1900 <= lunar_year <= 2100)  # 确认年份范围
+        and (1 <= lunar_month <= 12)  # 确认月份范围
+        and (
+            (  # 当为闰月时
+                1 <= lunar_day <= get_lunar_leap_size(lunar_year)  # 获取闰月日数
+                and (
+                    lunar_month
+                    == (lunar_month_data := get_lunar_month_list(lunar_year))[1]
+                )  # 确认此月闰月与否
+            )
+            if is_leap
+            else (  # 当非闰月时，确认日期范围
+                1
+                <= lunar_day
+                <= (  # 获取当月日数
+                    month_days_pusher(
+                        get_lunar_month_code(lunar_year),
+                        lunar_month,
                     )
                 )
             )
+        )
+    )
+    return (
+        verify_result,
+        *(
+            lunar_month_data
+            if lunar_month_data is not None
+            else get_lunar_month_list(lunar_year)
         ),
-        lunar_month_code,
-        leap_days,
     )
-)
-"""
-校验所给出之农历日期是否符合本库之可用性
-
-参数
-----
-    lunar_year: int 农历年份
-    lunar_month: int 农历月份
-    is_leap: bool 当月是否为闰月
-    lunar_day: int 当月天数
-
-返回值
-------
-    Tuple(bool该日期是否可用, int当年农历月份信息码, int当年闰月天数)
-"""
 
 
 def shíchen2int(dìzhī: Union[ShíchenString, XXIVShíChenString], xxiv: bool = False):
     """
     将给出的地支时辰字符串转为时辰数
 
     参数
@@ -744,20 +752,20 @@
                 hour=_hours,
                 minute=_minutes + minutes,
                 second=seconds,
                 microsecond=microseconds,
             ) + datetime.timedelta(
                 days=(
                     sum(
-                        (month_data := decode_lunar_month_code(*lunar_mon_info[1:]))[0][
+                        (lunar_mon_info[1])[
                             : lunar_month
                             - (
                                 not (
-                                    (is_leap and (lunar_month > month_data[1]))
-                                    and month_data[1]
+                                    (is_leap and (lunar_month > lunar_mon_info[2]))
+                                    and lunar_mon_info[2]
                                 )
                             )
                         ]
                     )
                     - 1
                     + lunar_day
                 )
```

### Comparing `zhdatetime-1.0.0/zhDateTime/types.py` & `zhdatetime-1.0.1/zhDateTime/types.py`

 * *Files identical despite different names*

### Comparing `zhdatetime-1.0.0/zhDateTime.egg-info/PKG-INFO` & `zhdatetime-1.0.1/zhDateTime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhDateTime
-Version: 1.0.0
+Version: 1.0.1
 Summary: 一个简单的小巧的中式日期时间库，附带数字汉字化操作。
 Home-page: https://gitee.com/EillesWan/zhDateTime
 Author: Eilles Wan
 Author-email: EillesWan@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 简易 Python 中式日期时间库
 
 ### 简介
 
-一个简单的小巧的轻量级中式日期时间库，支持农历公历互相转换，支持时辰刻数的时间表达转换，支持整数汉字化。
+一个简单小巧的轻量级中式日期时间库，支持农历公历互相转换，支持时辰刻数的时间表达转换，支持整数汉字化。
 
 ### 用法
 
 1.  农历与公历
 
 ```python
 from zhDateTime import DateTime,zhDateTime
```


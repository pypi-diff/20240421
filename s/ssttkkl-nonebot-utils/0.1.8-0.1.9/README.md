# Comparing `tmp/ssttkkl_nonebot_utils-0.1.8.tar.gz` & `tmp/ssttkkl_nonebot_utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssttkkl_nonebot_utils-0.1.8.tar", max compression
+gzip compressed data, was "ssttkkl_nonebot_utils-0.1.9.tar", max compression
```

## Comparing `ssttkkl_nonebot_utils-0.1.8.tar` & `ssttkkl_nonebot_utils-0.1.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0      880 2023-08-31 16:53:04.623681 ssttkkl_nonebot_utils-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-29 15:47:44.002368 ssttkkl_nonebot_utils-0.1.8/README.md
--rw-r--r--   0        0        0       62 2023-08-31 15:33:51.533524 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/__init__.py
--rw-r--r--   0        0        0     1069 2023-08-31 16:22:18.983335 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/config_loader.py
--rw-r--r--   0        0        0        0 2023-08-29 16:16:42.157519 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/errors/__init__.py
--rw-r--r--   0        0        0     2798 2023-08-31 16:53:04.629682 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/errors/error_handler.py
--rw-r--r--   0        0        0      377 2023-08-29 16:16:21.487064 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/errors/errors.py
--rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701000 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/integer.py
--rw-r--r--   0        0        0        0 2023-08-29 16:24:52.873659 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/interceptor/__init__.py
--rw-r--r--   0        0        0      815 2023-08-31 15:50:55.717080 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/interceptor/handle_error.py
--rw-r--r--   0        0        0      646 2023-08-29 16:36:20.848976 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/interceptor/with_handling_reaction.py
--rw-r--r--   0        0        0      836 2023-08-30 14:32:40.849616 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/nonebot.py
--rw-r--r--   0        0        0     1689 2023-08-30 14:33:10.635626 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/__init__.py
--rw-r--r--   0        0        0        0 2023-08-29 16:04:56.748000 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/extract_mention_user/__init__.py
--rw-r--r--   0        0        0        0 2023-08-29 16:05:59.435000 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/extract_mention_user/onebot/__init__.py
--rw-r--r--   0        0        0      251 2023-08-30 13:11:39.946519 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/extract_mention_user/onebot/v11.py
--rw-r--r--   0        0        0      263 2023-08-30 13:11:39.961520 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/extract_mention_user/qqguild.py
--rw-r--r--   0        0        0     1642 2023-08-30 13:58:34.485749 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/func_manager.py
--rw-r--r--   0        0        0      109 2023-08-30 14:38:05.055480 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/get_user_nickname/__init__.py
--rw-r--r--   0        0        0       65 2023-08-30 13:56:52.281798 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/get_user_nickname/cache.py
--rw-r--r--   0        0        0      211 2023-08-30 13:15:43.544541 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/get_user_nickname/fallback.py
--rw-r--r--   0        0        0      551 2023-08-30 13:59:33.058370 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/get_user_nickname/kaiheila.py
--rw-r--r--   0        0        0        0 2023-08-29 16:05:59.435710 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/get_user_nickname/onebot/__init__.py
--rw-r--r--   0        0        0      566 2023-08-29 15:54:08.728157 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/get_user_nickname/onebot/v11.py
--rw-r--r--   0        0        0      551 2023-08-30 13:59:33.054373 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/get_user_nickname/qqguild.py
--rw-r--r--   0        0        0        0 2023-08-29 16:04:56.741619 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/handling_reaction/__init__.py
--rw-r--r--   0        0        0      766 2023-08-30 13:16:36.027707 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/handling_reaction/fallback.py
--rw-r--r--   0        0        0     2016 2023-08-29 17:20:35.177317 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/handling_reaction/kaiheila.py
--rw-r--r--   0        0        0     1752 2023-08-29 17:20:42.523914 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/handling_reaction/qqguild.py
--rw-r--r--   0        0        0      109 2023-08-30 14:38:05.051481 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/is_destination_available/__init__.py
--rw-r--r--   0        0        0     4383 2023-08-29 15:51:13.415992 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/is_destination_available/kaiheila.py
--rw-r--r--   0        0        0        0 2023-08-29 16:05:59.435000 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/is_destination_available/onebot/__init__.py
--rw-r--r--   0        0        0      841 2023-08-29 16:06:29.169653 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/is_destination_available/onebot/v11.py
--rw-r--r--   0        0        0      109 2023-08-30 14:38:05.041479 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/is_group_admin/__init__.py
--rw-r--r--   0        0        0        0 2023-08-29 16:05:59.435000 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/is_group_admin/onebot/__init__.py
--rw-r--r--   0        0        0      499 2023-08-30 13:20:34.952872 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/is_group_admin/onebot/v11.py
--rw-r--r--   0        0        0      506 2023-08-30 13:20:34.962875 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/is_group_admin/qqguild.py
--rw-r--r--   0        0        0        0 2023-08-30 13:14:14.090082 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/send_msgs/__init__.py
--rw-r--r--   0        0        0      242 2023-08-30 14:03:06.851587 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/send_msgs/fallback.py
--rw-r--r--   0        0        0        0 2023-08-30 13:18:25.138730 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/send_msgs/onebot/__init__.py
--rw-r--r--   0        0        0     1705 2023-06-02 00:08:25.908000 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/send_msgs/onebot/v11.py
--rw-r--r--   0        0        0        0 2023-08-30 13:14:14.090000 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/upload_file/__init__.py
--rw-r--r--   0        0        0        0 2023-08-30 13:18:25.138000 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/upload_file/onebot/__init__.py
--rw-r--r--   0        0        0      243 2023-08-30 14:38:05.046479 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/upload_file/onebot/v11.py
--rw-r--r--   0        0        0      212 2023-08-30 14:38:46.596936 ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/requires/__init__.py
--rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 ssttkkl_nonebot_utils-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      880 2023-09-01 13:22:49.496454 ssttkkl_nonebot_utils-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-29 15:47:44.002368 ssttkkl_nonebot_utils-0.1.9/README.md
+-rw-r--r--   0        0        0       62 2023-08-31 15:33:51.533524 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/__init__.py
+-rw-r--r--   0        0        0     1069 2023-08-31 16:22:18.983335 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/config_loader.py
+-rw-r--r--   0        0        0        0 2023-08-29 16:16:42.157519 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/errors/__init__.py
+-rw-r--r--   0        0        0     2798 2023-08-31 16:53:04.629682 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/errors/error_handler.py
+-rw-r--r--   0        0        0      377 2023-08-29 16:16:21.487064 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/errors/errors.py
+-rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701000 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/integer.py
+-rw-r--r--   0        0        0        0 2023-08-29 16:24:52.873659 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/interceptor/__init__.py
+-rw-r--r--   0        0        0      815 2023-08-31 15:50:55.717080 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/interceptor/handle_error.py
+-rw-r--r--   0        0        0      646 2023-08-29 16:36:20.848976 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/interceptor/with_handling_reaction.py
+-rw-r--r--   0        0        0      836 2023-08-30 14:32:40.849616 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/nonebot.py
+-rw-r--r--   0        0        0     1689 2023-08-30 14:33:10.635626 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-29 16:04:56.748000 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/extract_mention_user/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-29 16:05:59.435000 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/extract_mention_user/onebot/__init__.py
+-rw-r--r--   0        0        0      245 2023-09-01 13:22:49.509455 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/extract_mention_user/onebot/v11.py
+-rw-r--r--   0        0        0      257 2023-09-01 13:22:49.485453 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/extract_mention_user/qqguild.py
+-rw-r--r--   0        0        0     1642 2023-08-30 13:58:34.485749 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/func_manager.py
+-rw-r--r--   0        0        0      109 2023-08-30 14:38:05.055480 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/get_user_nickname/__init__.py
+-rw-r--r--   0        0        0       65 2023-08-30 13:56:52.281798 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/get_user_nickname/cache.py
+-rw-r--r--   0        0        0      211 2023-08-30 13:15:43.544541 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/get_user_nickname/fallback.py
+-rw-r--r--   0        0        0      551 2023-08-30 13:59:33.058370 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/get_user_nickname/kaiheila.py
+-rw-r--r--   0        0        0        0 2023-08-29 16:05:59.435710 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/get_user_nickname/onebot/__init__.py
+-rw-r--r--   0        0        0      566 2023-08-29 15:54:08.728157 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/get_user_nickname/onebot/v11.py
+-rw-r--r--   0        0        0      551 2023-08-30 13:59:33.054373 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/get_user_nickname/qqguild.py
+-rw-r--r--   0        0        0        0 2023-08-29 16:04:56.741619 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/handling_reaction/__init__.py
+-rw-r--r--   0        0        0      766 2023-08-30 13:16:36.027707 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/handling_reaction/fallback.py
+-rw-r--r--   0        0        0     2016 2023-08-29 17:20:35.177317 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/handling_reaction/kaiheila.py
+-rw-r--r--   0        0        0     1752 2023-08-29 17:20:42.523914 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/handling_reaction/qqguild.py
+-rw-r--r--   0        0        0      109 2023-08-30 14:38:05.051481 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/is_destination_available/__init__.py
+-rw-r--r--   0        0        0     4383 2023-08-29 15:51:13.415992 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/is_destination_available/kaiheila.py
+-rw-r--r--   0        0        0        0 2023-08-29 16:05:59.435000 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/is_destination_available/onebot/__init__.py
+-rw-r--r--   0        0        0      841 2023-08-29 16:06:29.169653 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/is_destination_available/onebot/v11.py
+-rw-r--r--   0        0        0      109 2023-08-30 14:38:05.041479 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/is_group_admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-29 16:05:59.435000 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/is_group_admin/onebot/__init__.py
+-rw-r--r--   0        0        0      499 2023-08-30 13:20:34.952872 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/is_group_admin/onebot/v11.py
+-rw-r--r--   0        0        0      506 2023-08-30 13:20:34.962875 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/is_group_admin/qqguild.py
+-rw-r--r--   0        0        0        0 2023-08-30 13:14:14.090082 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/send_msgs/__init__.py
+-rw-r--r--   0        0        0      242 2023-08-30 14:03:06.851587 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/send_msgs/fallback.py
+-rw-r--r--   0        0        0        0 2023-08-30 13:18:25.138730 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/send_msgs/onebot/__init__.py
+-rw-r--r--   0        0        0     1705 2023-06-02 00:08:25.908000 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/send_msgs/onebot/v11.py
+-rw-r--r--   0        0        0        0 2023-08-30 13:14:14.090000 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/upload_file/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-30 13:18:25.138000 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/upload_file/onebot/__init__.py
+-rw-r--r--   0        0        0      243 2023-08-30 14:38:05.046479 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/upload_file/onebot/v11.py
+-rw-r--r--   0        0        0      212 2023-08-30 14:38:46.596936 ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/requires/__init__.py
+-rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 ssttkkl_nonebot_utils-0.1.9/PKG-INFO
```

### Comparing `ssttkkl_nonebot_utils-0.1.8/pyproject.toml` & `ssttkkl_nonebot_utils-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssttkkl-nonebot-utils"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "ssttkkl_nonebot_utils" }]
 
 [tool.poetry.dependencies]
```

### Comparing `ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/config_loader.py` & `ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/config_loader.py`

 * *Files identical despite different names*

### Comparing `ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/errors/error_handler.py` & `ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/integer.py` & `ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/integer.py`

 * *Files identical despite different names*

### Comparing `ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/interceptor/handle_error.py` & `ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/interceptor/handle_error.py`

 * *Files identical despite different names*

### Comparing `ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/interceptor/with_handling_reaction.py` & `ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/interceptor/with_handling_reaction.py`

 * *Files identical despite different names*

### Comparing `ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/nonebot.py` & `ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/nonebot.py`

 * *Files identical despite different names*

### Comparing `ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/__init__.py` & `ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/func_manager.py` & `ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/func_manager.py`

 * *Files identical despite different names*

### Comparing `ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/get_user_nickname/kaiheila.py` & `ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/get_user_nickname/kaiheila.py`

 * *Files identical despite different names*

### Comparing `ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/get_user_nickname/onebot/v11.py` & `ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/get_user_nickname/onebot/v11.py`

 * *Files identical despite different names*

### Comparing `ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/get_user_nickname/qqguild.py` & `ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/get_user_nickname/qqguild.py`

 * *Files identical despite different names*

### Comparing `ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/handling_reaction/fallback.py` & `ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/handling_reaction/fallback.py`

 * *Files identical despite different names*

### Comparing `ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/handling_reaction/kaiheila.py` & `ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/handling_reaction/kaiheila.py`

 * *Files identical despite different names*

### Comparing `ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/handling_reaction/qqguild.py` & `ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/handling_reaction/qqguild.py`

 * *Files identical despite different names*

### Comparing `ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/is_destination_available/kaiheila.py` & `ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/is_destination_available/kaiheila.py`

 * *Files identical despite different names*

### Comparing `ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/is_destination_available/onebot/v11.py` & `ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/is_destination_available/onebot/v11.py`

 * *Files identical despite different names*

### Comparing `ssttkkl_nonebot_utils-0.1.8/ssttkkl_nonebot_utils/platform/send_msgs/onebot/v11.py` & `ssttkkl_nonebot_utils-0.1.9/ssttkkl_nonebot_utils/platform/send_msgs/onebot/v11.py`

 * *Files identical despite different names*

### Comparing `ssttkkl_nonebot_utils-0.1.8/PKG-INFO` & `ssttkkl_nonebot_utils-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssttkkl-nonebot-utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


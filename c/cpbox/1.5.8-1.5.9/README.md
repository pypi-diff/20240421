# Comparing `tmp/cpbox-1.5.8.tar.gz` & `tmp/cpbox-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cpbox-1.5.8.tar", last modified: Sat Sep  7 08:37:26 2019, max compression
+gzip compressed data, was "dist/cpbox-1.5.9.tar", last modified: Sat Sep  7 08:51:46 2019, max compression
```

## Comparing `cpbox-1.5.8.tar` & `cpbox-1.5.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 huqiu      (501) staff       (20)        0 2019-09-07 08:37:26.000000 cpbox-1.5.8/
-drwxr-xr-x   0 huqiu      (501) staff       (20)        0 2019-09-07 08:37:26.000000 cpbox-1.5.8/cpbox.egg-info/
--rw-r--r--   0 huqiu      (501) staff       (20)      224 2019-09-07 08:37:26.000000 cpbox-1.5.8/cpbox.egg-info/PKG-INFO
--rw-r--r--   0 huqiu      (501) staff       (20)     1228 2019-09-07 08:37:26.000000 cpbox-1.5.8/cpbox.egg-info/SOURCES.txt
--rw-r--r--   0 huqiu      (501) staff       (20)       74 2019-09-07 08:37:26.000000 cpbox-1.5.8/cpbox.egg-info/requires.txt
--rw-r--r--   0 huqiu      (501) staff       (20)       12 2019-09-07 08:37:26.000000 cpbox-1.5.8/cpbox.egg-info/top_level.txt
--rw-r--r--   0 huqiu      (501) staff       (20)        1 2019-09-07 08:37:26.000000 cpbox-1.5.8/cpbox.egg-info/dependency_links.txt
--rw-r--r--   0 huqiu      (501) staff       (20)      224 2019-09-07 08:37:26.000000 cpbox-1.5.8/PKG-INFO
-drwxr-xr-x   0 huqiu      (501) staff       (20)        0 2019-09-07 08:37:26.000000 cpbox-1.5.8/cpbox/
-drwxr-xr-x   0 huqiu      (501) staff       (20)        0 2019-09-07 08:37:26.000000 cpbox-1.5.8/cpbox/app/
--rw-r--r--   0 huqiu      (501) staff       (20)     1166 2019-08-26 14:17:43.000000 cpbox-1.5.8/cpbox/app/env.py
--rw-r--r--   0 huqiu      (501) staff       (20)      595 2019-08-26 14:13:12.000000 cpbox-1.5.8/cpbox/app/appconfig.py
--rw-r--r--   0 huqiu      (501) staff       (20)     1078 2019-06-28 04:15:52.000000 cpbox-1.5.8/cpbox/app/eventlog.py
--rw-r--r--   0 huqiu      (501) staff       (20)       15 2019-05-17 08:51:35.000000 cpbox-1.5.8/cpbox/app/__init__.py
--rw-r--r--   0 huqiu      (501) staff       (20)     8841 2019-09-07 07:53:33.000000 cpbox-1.5.8/cpbox/app/devops.py
--rw-r--r--   0 huqiu      (501) staff       (20)     6846 2019-09-07 03:54:23.000000 cpbox-1.5.8/cpbox/app/multiuser.py
--rw-r--r--   0 huqiu      (501) staff       (20)       15 2019-05-17 08:51:35.000000 cpbox-1.5.8/cpbox/__init__.py
-drwxr-xr-x   0 huqiu      (501) staff       (20)        0 2019-09-07 08:37:26.000000 cpbox-1.5.8/cpbox/clis/
--rw-r--r--   0 huqiu      (501) staff       (20)     3336 2019-08-11 04:40:55.000000 cpbox-1.5.8/cpbox/clis/mysqlcli.py
--rwxr-xr-x   0 huqiu      (501) staff       (20)        0 2019-02-18 01:36:37.000000 cpbox-1.5.8/cpbox/clis/__init__.py
--rw-r--r--   0 huqiu      (501) staff       (20)     1857 2019-08-11 05:03:08.000000 cpbox-1.5.8/cpbox/clis/rediscli.py
-drwxr-xr-x   0 huqiu      (501) staff       (20)        0 2019-09-07 08:37:26.000000 cpbox-1.5.8/cpbox/tool/
--rw-r--r--   0 huqiu      (501) staff       (20)     1144 2019-05-17 08:51:35.000000 cpbox-1.5.8/cpbox/tool/local_cache.py
--rw-r--r--   0 huqiu      (501) staff       (20)     2530 2019-06-21 09:20:23.000000 cpbox-1.5.8/cpbox/tool/system.py
--rw-r--r--   0 huqiu      (501) staff       (20)     6130 2019-06-22 08:29:51.000000 cpbox-1.5.8/cpbox/tool/concurrent.py
--rw-r--r--   0 huqiu      (501) staff       (20)      284 2019-05-17 08:51:35.000000 cpbox-1.5.8/cpbox/tool/timeutil.py
--rw-r--r--   0 huqiu      (501) staff       (20)      840 2019-06-11 02:49:28.000000 cpbox-1.5.8/cpbox/tool/testutils.py
--rw-r--r--   0 huqiu      (501) staff       (20)    13655 2019-05-17 08:51:35.000000 cpbox-1.5.8/cpbox/tool/crontab.py
--rw-r--r--   0 huqiu      (501) staff       (20)      896 2019-06-26 03:37:16.000000 cpbox-1.5.8/cpbox/tool/net.py
--rw-r--r--   0 huqiu      (501) staff       (20)     4324 2019-05-17 08:51:35.000000 cpbox-1.5.8/cpbox/tool/cache.py
--rw-r--r--   0 huqiu      (501) staff       (20)        0 2019-05-17 08:51:35.000000 cpbox-1.5.8/cpbox/tool/__init__.py
--rw-r--r--   0 huqiu      (501) staff       (20)     2334 2019-08-23 06:49:43.000000 cpbox-1.5.8/cpbox/tool/dockerutil.py
--rw-r--r--   0 huqiu      (501) staff       (20)     1576 2019-09-07 05:04:54.000000 cpbox-1.5.8/cpbox/tool/spec.py
--rw-r--r--   0 huqiu      (501) staff       (20)     8121 2019-06-28 04:14:54.000000 cpbox-1.5.8/cpbox/tool/logger.py
--rw-r--r--   0 huqiu      (501) staff       (20)     3382 2019-06-12 00:48:45.000000 cpbox-1.5.8/cpbox/tool/file.py
--rw-r--r--   0 huqiu      (501) staff       (20)     4746 2019-05-17 08:51:35.000000 cpbox-1.5.8/cpbox/tool/datatypes.py
--rw-r--r--   0 huqiu      (501) staff       (20)     2888 2019-06-18 11:47:14.000000 cpbox-1.5.8/cpbox/tool/utils.py
--rw-r--r--   0 huqiu      (501) staff       (20)      949 2019-05-17 08:51:35.000000 cpbox-1.5.8/cpbox/tool/http.py
--rw-r--r--   0 huqiu      (501) staff       (20)     1587 2019-06-10 13:30:14.000000 cpbox-1.5.8/cpbox/tool/template.py
--rw-r--r--   0 huqiu      (501) staff       (20)      209 2019-05-17 08:51:35.000000 cpbox-1.5.8/cpbox/tool/strjson.py
--rw-r--r--   0 huqiu      (501) staff       (20)     1574 2019-05-17 08:51:35.000000 cpbox-1.5.8/cpbox/tool/redistool.py
--rw-r--r--   0 huqiu      (501) staff       (20)      682 2019-05-17 08:51:35.000000 cpbox-1.5.8/cpbox/tool/array.py
--rw-r--r--   0 huqiu      (501) staff       (20)     1393 2019-07-12 09:52:18.000000 cpbox-1.5.8/cpbox/tool/strings.py
--rw-r--r--   0 huqiu      (501) staff       (20)    12513 2019-06-28 03:20:30.000000 cpbox-1.5.8/cpbox/tool/functocli.py
-drwxr-xr-x   0 huqiu      (501) staff       (20)        0 2019-09-07 08:37:26.000000 cpbox-1.5.8/tests/
--rw-r--r--   0 huqiu      (501) staff       (20)      877 2019-06-10 13:30:14.000000 cpbox-1.5.8/tests/test_utils.py
--rw-r--r--   0 huqiu      (501) staff       (20)      560 2019-06-26 03:41:55.000000 cpbox-1.5.8/tests/test_net.py
--rw-r--r--   0 huqiu      (501) staff       (20)      517 2019-06-11 02:46:30.000000 cpbox-1.5.8/tests/test_eventlog.py
--rw-r--r--   0 huqiu      (501) staff       (20)     1422 2019-05-21 03:57:47.000000 cpbox-1.5.8/tests/test_tool_redis.py
--rw-r--r--   0 huqiu      (501) staff       (20)     1037 2019-05-21 03:57:47.000000 cpbox-1.5.8/tests/test_functocli.py
--rw-r--r--   0 huqiu      (501) staff       (20)      709 2019-05-17 08:51:35.000000 cpbox-1.5.8/tests/test_array.py
--rw-r--r--   0 huqiu      (501) staff       (20)     2501 2019-05-17 08:51:35.000000 cpbox-1.5.8/tests/test_nameiddict.py
--rw-r--r--   0 huqiu      (501) staff       (20)        0 2019-05-17 08:51:35.000000 cpbox-1.5.8/tests/__init__.py
--rw-r--r--   0 huqiu      (501) staff       (20)      877 2019-06-21 09:16:11.000000 cpbox-1.5.8/tests/test_threadpool.py
--rw-r--r--   0 huqiu      (501) staff       (20)      972 2019-05-21 07:07:52.000000 cpbox-1.5.8/tests/test_system.py
--rw-r--r--   0 huqiu      (501) staff       (20)      947 2019-05-21 06:53:58.000000 cpbox-1.5.8/tests/test_file.py
--rw-r--r--   0 huqiu      (501) staff       (20)     3681 2019-05-21 03:57:47.000000 cpbox-1.5.8/tests/test_tool_cache.py
--rw-r--r--   0 huqiu      (501) staff       (20)      277 2019-08-23 06:53:45.000000 cpbox-1.5.8/tests/test_dockerutil.py
--rw-r--r--   0 huqiu      (501) staff       (20)      735 2019-06-21 09:23:40.000000 cpbox-1.5.8/tests/test_timer.py
--rw-r--r--   0 huqiu      (501) staff       (20)     2113 2019-06-21 04:29:43.000000 cpbox-1.5.8/tests/test_concurrent.py
--rw-r--r--   0 huqiu      (501) staff       (20)      394 2019-08-02 04:35:27.000000 cpbox-1.5.8/tests/test_strings.py
--rw-r--r--   0 huqiu      (501) staff       (20)      960 2019-06-11 02:49:28.000000 cpbox-1.5.8/tests/test_template.py
--rw-r--r--   0 huqiu      (501) staff       (20)      545 2019-09-07 08:37:16.000000 cpbox-1.5.8/setup.py
--rw-r--r--   0 huqiu      (501) staff       (20)       59 2019-09-07 08:37:26.000000 cpbox-1.5.8/setup.cfg
+drwxr-xr-x   0 huqiu      (501) staff       (20)        0 2019-09-07 08:51:46.000000 cpbox-1.5.9/
+drwxr-xr-x   0 huqiu      (501) staff       (20)        0 2019-09-07 08:51:46.000000 cpbox-1.5.9/cpbox.egg-info/
+-rw-r--r--   0 huqiu      (501) staff       (20)      224 2019-09-07 08:51:46.000000 cpbox-1.5.9/cpbox.egg-info/PKG-INFO
+-rw-r--r--   0 huqiu      (501) staff       (20)     1228 2019-09-07 08:51:46.000000 cpbox-1.5.9/cpbox.egg-info/SOURCES.txt
+-rw-r--r--   0 huqiu      (501) staff       (20)       74 2019-09-07 08:51:46.000000 cpbox-1.5.9/cpbox.egg-info/requires.txt
+-rw-r--r--   0 huqiu      (501) staff       (20)       12 2019-09-07 08:51:46.000000 cpbox-1.5.9/cpbox.egg-info/top_level.txt
+-rw-r--r--   0 huqiu      (501) staff       (20)        1 2019-09-07 08:51:46.000000 cpbox-1.5.9/cpbox.egg-info/dependency_links.txt
+-rw-r--r--   0 huqiu      (501) staff       (20)      224 2019-09-07 08:51:46.000000 cpbox-1.5.9/PKG-INFO
+drwxr-xr-x   0 huqiu      (501) staff       (20)        0 2019-09-07 08:51:46.000000 cpbox-1.5.9/cpbox/
+drwxr-xr-x   0 huqiu      (501) staff       (20)        0 2019-09-07 08:51:46.000000 cpbox-1.5.9/cpbox/app/
+-rw-r--r--   0 huqiu      (501) staff       (20)     1166 2019-08-26 14:17:43.000000 cpbox-1.5.9/cpbox/app/env.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      595 2019-08-26 14:13:12.000000 cpbox-1.5.9/cpbox/app/appconfig.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     1078 2019-06-28 04:15:52.000000 cpbox-1.5.9/cpbox/app/eventlog.py
+-rw-r--r--   0 huqiu      (501) staff       (20)       15 2019-05-17 08:51:35.000000 cpbox-1.5.9/cpbox/app/__init__.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     8841 2019-09-07 07:53:33.000000 cpbox-1.5.9/cpbox/app/devops.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     6842 2019-09-07 08:48:23.000000 cpbox-1.5.9/cpbox/app/multiuser.py
+-rw-r--r--   0 huqiu      (501) staff       (20)       15 2019-05-17 08:51:35.000000 cpbox-1.5.9/cpbox/__init__.py
+drwxr-xr-x   0 huqiu      (501) staff       (20)        0 2019-09-07 08:51:46.000000 cpbox-1.5.9/cpbox/clis/
+-rw-r--r--   0 huqiu      (501) staff       (20)     3336 2019-08-11 04:40:55.000000 cpbox-1.5.9/cpbox/clis/mysqlcli.py
+-rwxr-xr-x   0 huqiu      (501) staff       (20)        0 2019-02-18 01:36:37.000000 cpbox-1.5.9/cpbox/clis/__init__.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     1857 2019-08-11 05:03:08.000000 cpbox-1.5.9/cpbox/clis/rediscli.py
+drwxr-xr-x   0 huqiu      (501) staff       (20)        0 2019-09-07 08:51:46.000000 cpbox-1.5.9/cpbox/tool/
+-rw-r--r--   0 huqiu      (501) staff       (20)     1144 2019-05-17 08:51:35.000000 cpbox-1.5.9/cpbox/tool/local_cache.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     2530 2019-06-21 09:20:23.000000 cpbox-1.5.9/cpbox/tool/system.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     6130 2019-06-22 08:29:51.000000 cpbox-1.5.9/cpbox/tool/concurrent.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      284 2019-05-17 08:51:35.000000 cpbox-1.5.9/cpbox/tool/timeutil.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      840 2019-06-11 02:49:28.000000 cpbox-1.5.9/cpbox/tool/testutils.py
+-rw-r--r--   0 huqiu      (501) staff       (20)    13655 2019-05-17 08:51:35.000000 cpbox-1.5.9/cpbox/tool/crontab.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      896 2019-06-26 03:37:16.000000 cpbox-1.5.9/cpbox/tool/net.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     4324 2019-05-17 08:51:35.000000 cpbox-1.5.9/cpbox/tool/cache.py
+-rw-r--r--   0 huqiu      (501) staff       (20)        0 2019-05-17 08:51:35.000000 cpbox-1.5.9/cpbox/tool/__init__.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     2334 2019-08-23 06:49:43.000000 cpbox-1.5.9/cpbox/tool/dockerutil.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     1576 2019-09-07 05:04:54.000000 cpbox-1.5.9/cpbox/tool/spec.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     8121 2019-06-28 04:14:54.000000 cpbox-1.5.9/cpbox/tool/logger.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     3382 2019-06-12 00:48:45.000000 cpbox-1.5.9/cpbox/tool/file.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     4746 2019-05-17 08:51:35.000000 cpbox-1.5.9/cpbox/tool/datatypes.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     2888 2019-06-18 11:47:14.000000 cpbox-1.5.9/cpbox/tool/utils.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      949 2019-05-17 08:51:35.000000 cpbox-1.5.9/cpbox/tool/http.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     1587 2019-06-10 13:30:14.000000 cpbox-1.5.9/cpbox/tool/template.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      209 2019-05-17 08:51:35.000000 cpbox-1.5.9/cpbox/tool/strjson.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     1574 2019-05-17 08:51:35.000000 cpbox-1.5.9/cpbox/tool/redistool.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      682 2019-05-17 08:51:35.000000 cpbox-1.5.9/cpbox/tool/array.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     1393 2019-07-12 09:52:18.000000 cpbox-1.5.9/cpbox/tool/strings.py
+-rw-r--r--   0 huqiu      (501) staff       (20)    12513 2019-06-28 03:20:30.000000 cpbox-1.5.9/cpbox/tool/functocli.py
+drwxr-xr-x   0 huqiu      (501) staff       (20)        0 2019-09-07 08:51:46.000000 cpbox-1.5.9/tests/
+-rw-r--r--   0 huqiu      (501) staff       (20)      877 2019-06-10 13:30:14.000000 cpbox-1.5.9/tests/test_utils.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      560 2019-06-26 03:41:55.000000 cpbox-1.5.9/tests/test_net.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      517 2019-06-11 02:46:30.000000 cpbox-1.5.9/tests/test_eventlog.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     1422 2019-05-21 03:57:47.000000 cpbox-1.5.9/tests/test_tool_redis.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     1037 2019-05-21 03:57:47.000000 cpbox-1.5.9/tests/test_functocli.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      709 2019-05-17 08:51:35.000000 cpbox-1.5.9/tests/test_array.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     2501 2019-05-17 08:51:35.000000 cpbox-1.5.9/tests/test_nameiddict.py
+-rw-r--r--   0 huqiu      (501) staff       (20)        0 2019-05-17 08:51:35.000000 cpbox-1.5.9/tests/__init__.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      877 2019-06-21 09:16:11.000000 cpbox-1.5.9/tests/test_threadpool.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      972 2019-05-21 07:07:52.000000 cpbox-1.5.9/tests/test_system.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      947 2019-05-21 06:53:58.000000 cpbox-1.5.9/tests/test_file.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     3681 2019-05-21 03:57:47.000000 cpbox-1.5.9/tests/test_tool_cache.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      277 2019-08-23 06:53:45.000000 cpbox-1.5.9/tests/test_dockerutil.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      735 2019-06-21 09:23:40.000000 cpbox-1.5.9/tests/test_timer.py
+-rw-r--r--   0 huqiu      (501) staff       (20)     2113 2019-06-21 04:29:43.000000 cpbox-1.5.9/tests/test_concurrent.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      394 2019-08-02 04:35:27.000000 cpbox-1.5.9/tests/test_strings.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      960 2019-06-11 02:49:28.000000 cpbox-1.5.9/tests/test_template.py
+-rw-r--r--   0 huqiu      (501) staff       (20)      545 2019-09-07 08:49:27.000000 cpbox-1.5.9/setup.py
+-rw-r--r--   0 huqiu      (501) staff       (20)       59 2019-09-07 08:51:46.000000 cpbox-1.5.9/setup.cfg
```

### Comparing `cpbox-1.5.8/cpbox.egg-info/SOURCES.txt` & `cpbox-1.5.9/cpbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/app/env.py` & `cpbox-1.5.9/cpbox/app/env.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/app/appconfig.py` & `cpbox-1.5.9/cpbox/app/appconfig.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/app/eventlog.py` & `cpbox-1.5.9/cpbox/app/eventlog.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/app/devops.py` & `cpbox-1.5.9/cpbox/app/devops.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/app/multiuser.py` & `cpbox-1.5.9/cpbox/app/multiuser.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self.app_base_name = app_base_name
         self.kwargs = kwargs
         self.determine_developer_name()
         app_name = self.determine_app_name()
         DevOpsAppConfigProvider.__init__(self, app_name)
 
     def determine_developer_name(self):
-        app_config = DevOpsAppConfigProvider.get_project_local_config(self)
+        app_config = DevOpsAppConfigProvider.get_box_local_config(self)
         developer_name = app_config.get('developer_name', None)
         if not developer_name:
             developer_name = getpass.getuser()
         developer_name_from_cmd = self.kwargs.get('developer_name', None)
         self.developer_name = developer_name_from_cmd if developer_name_from_cmd else developer_name
 
     def determine_app_name(self):
```

### Comparing `cpbox-1.5.8/cpbox/clis/mysqlcli.py` & `cpbox-1.5.9/cpbox/clis/mysqlcli.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/clis/rediscli.py` & `cpbox-1.5.9/cpbox/clis/rediscli.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/local_cache.py` & `cpbox-1.5.9/cpbox/tool/local_cache.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/system.py` & `cpbox-1.5.9/cpbox/tool/system.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/concurrent.py` & `cpbox-1.5.9/cpbox/tool/concurrent.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/testutils.py` & `cpbox-1.5.9/cpbox/tool/testutils.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/crontab.py` & `cpbox-1.5.9/cpbox/tool/crontab.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/net.py` & `cpbox-1.5.9/cpbox/tool/net.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/cache.py` & `cpbox-1.5.9/cpbox/tool/cache.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/dockerutil.py` & `cpbox-1.5.9/cpbox/tool/dockerutil.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/spec.py` & `cpbox-1.5.9/cpbox/tool/spec.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/logger.py` & `cpbox-1.5.9/cpbox/tool/logger.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/file.py` & `cpbox-1.5.9/cpbox/tool/file.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/datatypes.py` & `cpbox-1.5.9/cpbox/tool/datatypes.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/utils.py` & `cpbox-1.5.9/cpbox/tool/utils.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/http.py` & `cpbox-1.5.9/cpbox/tool/http.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/template.py` & `cpbox-1.5.9/cpbox/tool/template.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/redistool.py` & `cpbox-1.5.9/cpbox/tool/redistool.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/array.py` & `cpbox-1.5.9/cpbox/tool/array.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/strings.py` & `cpbox-1.5.9/cpbox/tool/strings.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/cpbox/tool/functocli.py` & `cpbox-1.5.9/cpbox/tool/functocli.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/tests/test_utils.py` & `cpbox-1.5.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/tests/test_net.py` & `cpbox-1.5.9/tests/test_net.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/tests/test_eventlog.py` & `cpbox-1.5.9/tests/test_eventlog.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/tests/test_tool_redis.py` & `cpbox-1.5.9/tests/test_tool_redis.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/tests/test_functocli.py` & `cpbox-1.5.9/tests/test_functocli.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/tests/test_array.py` & `cpbox-1.5.9/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/tests/test_nameiddict.py` & `cpbox-1.5.9/tests/test_nameiddict.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/tests/test_threadpool.py` & `cpbox-1.5.9/tests/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/tests/test_system.py` & `cpbox-1.5.9/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/tests/test_file.py` & `cpbox-1.5.9/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/tests/test_tool_cache.py` & `cpbox-1.5.9/tests/test_tool_cache.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/tests/test_timer.py` & `cpbox-1.5.9/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/tests/test_concurrent.py` & `cpbox-1.5.9/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/tests/test_template.py` & `cpbox-1.5.9/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `cpbox-1.5.8/setup.py` & `cpbox-1.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'cpbox',
-    version = '1.5.8',
+    version = '1.5.9',
     keywords = ('cpbox'),
     description = 'cp tool box',
     license = '',
     install_requires = [
         'six',
         'ruamel.yaml',
         'Jinja2',
```


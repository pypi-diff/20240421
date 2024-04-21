# Comparing `tmp/flowdata-0.1.0.tar.gz` & `tmp/flowdata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flowdata-0.1.0.tar", last modified: Sat Apr 20 13:21:39 2024, max compression
+gzip compressed data, was "dist/flowdata-0.1.1.tar", last modified: Sat Apr 20 13:56:18 2024, max compression
```

## Comparing `flowdata-0.1.0.tar` & `flowdata-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 13:21:39.000000 flowdata-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      223 2024-04-20 13:21:39.000000 flowdata-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1348 2024-04-20 13:20:10.000000 flowdata-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 13:21:39.000000 flowdata-0.1.0/flowdata/
--rw-r--r--   0 root         (0) root         (0)      107 2024-04-20 13:02:13.000000 flowdata-0.1.0/flowdata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4184 2024-04-20 06:57:27.000000 flowdata-0.1.0/flowdata/_io.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-04-19 12:06:46.000000 flowdata-0.1.0/flowdata/_logger.py
--rw-r--r--   0 root         (0) root         (0)     3365 2024-04-20 12:48:40.000000 flowdata-0.1.0/flowdata/data_flow.py
--rw-r--r--   0 root         (0) root         (0)     2932 2024-04-20 12:49:07.000000 flowdata-0.1.0/flowdata/data_parallel.py
--rw-r--r--   0 root         (0) root         (0)     6187 2024-04-20 12:40:02.000000 flowdata-0.1.0/flowdata/decorator.py
--rw-r--r--   0 root         (0) root         (0)      651 2024-04-20 13:12:14.000000 flowdata-0.1.0/flowdata/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 13:21:39.000000 flowdata-0.1.0/flowdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)      223 2024-04-20 13:21:39.000000 flowdata-0.1.0/flowdata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      379 2024-04-20 13:21:39.000000 flowdata-0.1.0/flowdata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 13:21:39.000000 flowdata-0.1.0/flowdata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-20 13:21:39.000000 flowdata-0.1.0/flowdata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-20 13:21:39.000000 flowdata-0.1.0/flowdata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 13:21:39.000000 flowdata-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-20 13:13:22.000000 flowdata-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 13:21:39.000000 flowdata-0.1.0/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 03:35:00.000000 flowdata-0.1.0/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      709 2024-04-20 13:02:35.000000 flowdata-0.1.0/test/test_flow.py
--rw-r--r--   0 root         (0) root         (0)      884 2024-04-20 13:11:06.000000 flowdata-0.1.0/test/test_multitask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 13:56:18.000000 flowdata-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     2267 2024-04-20 13:56:18.000000 flowdata-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1398 2024-04-20 13:24:52.000000 flowdata-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 13:56:18.000000 flowdata-0.1.1/flowdata/
+-rw-r--r--   0 root         (0) root         (0)      107 2024-04-20 13:02:13.000000 flowdata-0.1.1/flowdata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4184 2024-04-20 06:57:27.000000 flowdata-0.1.1/flowdata/_io.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-19 12:06:46.000000 flowdata-0.1.1/flowdata/_logger.py
+-rw-r--r--   0 root         (0) root         (0)     3365 2024-04-20 12:48:40.000000 flowdata-0.1.1/flowdata/data_flow.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2024-04-20 12:49:07.000000 flowdata-0.1.1/flowdata/data_parallel.py
+-rw-r--r--   0 root         (0) root         (0)     6187 2024-04-20 12:40:02.000000 flowdata-0.1.1/flowdata/decorator.py
+-rw-r--r--   0 root         (0) root         (0)      651 2024-04-20 13:12:14.000000 flowdata-0.1.1/flowdata/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 13:56:18.000000 flowdata-0.1.1/flowdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2267 2024-04-20 13:56:18.000000 flowdata-0.1.1/flowdata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      379 2024-04-20 13:56:18.000000 flowdata-0.1.1/flowdata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 13:56:18.000000 flowdata-0.1.1/flowdata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-20 13:56:18.000000 flowdata-0.1.1/flowdata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-20 13:56:18.000000 flowdata-0.1.1/flowdata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 13:56:18.000000 flowdata-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      684 2024-04-20 13:56:15.000000 flowdata-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 13:56:18.000000 flowdata-0.1.1/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 03:35:00.000000 flowdata-0.1.1/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      709 2024-04-20 13:02:35.000000 flowdata-0.1.1/test/test_flow.py
+-rw-r--r--   0 root         (0) root         (0)      884 2024-04-20 13:11:06.000000 flowdata-0.1.1/test/test_multitask.py
```

### Comparing `flowdata-0.1.0/README.md` & `flowdata-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # flowdata
 流式数据简易处理工具
 
 本项目支持对流式数据的处理进行多进程加速
 
 
+# 安装 flowdata
+
+```
+pip install flowdata
+```
+
+
 # Quick Start
 
 ## 1、单任务
 代码中通过add_task将任务加载到任务流中，且可以根据需要指定不同进程数量
 
 ```python
```

### Comparing `flowdata-0.1.0/flowdata/_io.py` & `flowdata-0.1.1/flowdata/_io.py`

 * *Files identical despite different names*

### Comparing `flowdata-0.1.0/flowdata/_logger.py` & `flowdata-0.1.1/flowdata/_logger.py`

 * *Files identical despite different names*

### Comparing `flowdata-0.1.0/flowdata/data_flow.py` & `flowdata-0.1.1/flowdata/data_flow.py`

 * *Files identical despite different names*

### Comparing `flowdata-0.1.0/flowdata/data_parallel.py` & `flowdata-0.1.1/flowdata/data_parallel.py`

 * *Files identical despite different names*

### Comparing `flowdata-0.1.0/flowdata/decorator.py` & `flowdata-0.1.1/flowdata/decorator.py`

 * *Files identical despite different names*

### Comparing `flowdata-0.1.0/flowdata/task.py` & `flowdata-0.1.1/flowdata/task.py`

 * *Files identical despite different names*

### Comparing `flowdata-0.1.0/test/test_flow.py` & `flowdata-0.1.1/test/test_flow.py`

 * *Files identical despite different names*

### Comparing `flowdata-0.1.0/test/test_multitask.py` & `flowdata-0.1.1/test/test_multitask.py`

 * *Files identical despite different names*


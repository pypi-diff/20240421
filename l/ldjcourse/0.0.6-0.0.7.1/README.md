# Comparing `tmp/ldjcourse-0.0.6.tar.gz` & `tmp/ldjcourse-0.0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ldjcourse-0.0.6.tar", last modified: Sun Apr 21 15:42:09 2024, max compression
+gzip compressed data, was "dist\ldjcourse-0.0.7.1.tar", last modified: Sun Apr 21 15:53:48 2024, max compression
```

## Comparing `ldjcourse-0.0.6.tar` & `ldjcourse-0.0.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 15:42:09.255663 ldjcourse-0.0.6/
--rw-rw-rw-   0        0        0      166 2024-04-21 15:42:09.249983 ldjcourse-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-21 15:42:09.173121 ldjcourse-0.0.6/ldjcourse/
--rw-rw-rw-   0        0        0        0 2024-04-06 11:24:13.000000 ldjcourse-0.0.6/ldjcourse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:42:09.197745 ldjcourse-0.0.6/ldjcourse/pandas/
--rw-rw-rw-   0        0        0        0 2024-04-20 04:41:18.000000 ldjcourse-0.0.6/ldjcourse/pandas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:42:09.229723 ldjcourse-0.0.6/ldjcourse/pandas/v1_1/
--rw-rw-rw-   0        0        0        0 2024-04-06 11:25:30.000000 ldjcourse-0.0.6/ldjcourse/pandas/v1_1/__init__.py
--rw-rw-rw-   0        0        0      685 2024-04-21 15:42:07.000000 ldjcourse-0.0.6/ldjcourse/pandas/v1_1/api.py
--rw-rw-rw-   0        0        0     1330 2024-04-20 07:04:45.000000 ldjcourse-0.0.6/ldjcourse/pandas/v1_1/data.py
--rw-rw-rw-   0        0        0       22 2024-04-20 04:51:34.000000 ldjcourse-0.0.6/ldjcourse/pandas/v1_1/setting.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:42:09.243942 ldjcourse-0.0.6/ldjcourse.egg-info/
--rw-rw-rw-   0        0        0      166 2024-04-21 15:42:08.000000 ldjcourse-0.0.6/ldjcourse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-04-21 15:42:09.000000 ldjcourse-0.0.6/ldjcourse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 15:42:08.000000 ldjcourse-0.0.6/ldjcourse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-21 15:42:08.000000 ldjcourse-0.0.6/ldjcourse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 15:42:09.256318 ldjcourse-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      580 2024-04-21 15:42:07.000000 ldjcourse-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:53:48.905995 ldjcourse-0.0.7.1/
+-rw-rw-rw-   0        0        0      168 2024-04-21 15:53:48.898790 ldjcourse-0.0.7.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-21 15:53:48.746629 ldjcourse-0.0.7.1/ldjcourse/
+-rw-rw-rw-   0        0        0        0 2024-04-06 11:24:13.000000 ldjcourse-0.0.7.1/ldjcourse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:53:48.796660 ldjcourse-0.0.7.1/ldjcourse/pandas/
+-rw-rw-rw-   0        0        0        0 2024-04-20 04:41:18.000000 ldjcourse-0.0.7.1/ldjcourse/pandas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:53:48.871320 ldjcourse-0.0.7.1/ldjcourse/pandas/v1_1/
+-rw-rw-rw-   0        0        0        0 2024-04-06 11:25:30.000000 ldjcourse-0.0.7.1/ldjcourse/pandas/v1_1/__init__.py
+-rw-rw-rw-   0        0        0      780 2024-04-21 15:52:17.000000 ldjcourse-0.0.7.1/ldjcourse/pandas/v1_1/api.py
+-rw-rw-rw-   0        0        0     1330 2024-04-20 07:04:45.000000 ldjcourse-0.0.7.1/ldjcourse/pandas/v1_1/data.py
+-rw-rw-rw-   0        0        0       22 2024-04-20 04:51:34.000000 ldjcourse-0.0.7.1/ldjcourse/pandas/v1_1/setting.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:53:48.891753 ldjcourse-0.0.7.1/ldjcourse.egg-info/
+-rw-rw-rw-   0        0        0      168 2024-04-21 15:53:48.000000 ldjcourse-0.0.7.1/ldjcourse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-04-21 15:53:48.000000 ldjcourse-0.0.7.1/ldjcourse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 15:53:48.000000 ldjcourse-0.0.7.1/ldjcourse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-21 15:53:48.000000 ldjcourse-0.0.7.1/ldjcourse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 15:53:48.906678 ldjcourse-0.0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      582 2024-04-21 15:52:53.000000 ldjcourse-0.0.7.1/setup.py
```

### Comparing `ldjcourse-0.0.6/ldjcourse/pandas/v1_1/data.py` & `ldjcourse-0.0.7.1/ldjcourse/pandas/v1_1/data.py`

 * *Files identical despite different names*

### Comparing `ldjcourse-0.0.6/setup.py` & `ldjcourse-0.0.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6'
+VERSION = '0.0.7.1'
 
 setup(
     name='ldjcourse',
     version=VERSION,
     author='元蓝先生',
     description='B站：元蓝先生 https://space.bilibili.com/3546564903569609',
     license='MIT',
```


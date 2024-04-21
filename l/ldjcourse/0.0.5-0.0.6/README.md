# Comparing `tmp/ldjcourse-0.0.5.tar.gz` & `tmp/ldjcourse-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ldjcourse-0.0.5.tar", last modified: Sat Apr 20 07:05:03 2024, max compression
+gzip compressed data, was "dist\ldjcourse-0.0.6.tar", last modified: Sun Apr 21 15:42:09 2024, max compression
```

## Comparing `ldjcourse-0.0.5.tar` & `ldjcourse-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 07:05:03.326025 ldjcourse-0.0.5/
--rw-rw-rw-   0        0        0      166 2024-04-20 07:05:03.318678 ldjcourse-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-20 07:05:03.229498 ldjcourse-0.0.5/ldjcourse/
--rw-rw-rw-   0        0        0        0 2024-04-06 11:24:13.000000 ldjcourse-0.0.5/ldjcourse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:05:03.267456 ldjcourse-0.0.5/ldjcourse/pandas/
--rw-rw-rw-   0        0        0        0 2024-04-20 04:41:18.000000 ldjcourse-0.0.5/ldjcourse/pandas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:05:03.300222 ldjcourse-0.0.5/ldjcourse/pandas/v1_1/
--rw-rw-rw-   0        0        0        0 2024-04-06 11:25:30.000000 ldjcourse-0.0.5/ldjcourse/pandas/v1_1/__init__.py
--rw-rw-rw-   0        0        0      295 2024-04-20 05:52:58.000000 ldjcourse-0.0.5/ldjcourse/pandas/v1_1/api.py
--rw-rw-rw-   0        0        0     1330 2024-04-20 07:04:45.000000 ldjcourse-0.0.5/ldjcourse/pandas/v1_1/data.py
--rw-rw-rw-   0        0        0       22 2024-04-20 04:51:34.000000 ldjcourse-0.0.5/ldjcourse/pandas/v1_1/setting.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:05:03.311364 ldjcourse-0.0.5/ldjcourse.egg-info/
--rw-rw-rw-   0        0        0      166 2024-04-20 07:05:03.000000 ldjcourse-0.0.5/ldjcourse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-04-20 07:05:03.000000 ldjcourse-0.0.5/ldjcourse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 07:05:03.000000 ldjcourse-0.0.5/ldjcourse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-20 07:05:03.000000 ldjcourse-0.0.5/ldjcourse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 07:05:03.326669 ldjcourse-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      358 2024-04-20 07:05:00.000000 ldjcourse-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:42:09.255663 ldjcourse-0.0.6/
+-rw-rw-rw-   0        0        0      166 2024-04-21 15:42:09.249983 ldjcourse-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-21 15:42:09.173121 ldjcourse-0.0.6/ldjcourse/
+-rw-rw-rw-   0        0        0        0 2024-04-06 11:24:13.000000 ldjcourse-0.0.6/ldjcourse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:42:09.197745 ldjcourse-0.0.6/ldjcourse/pandas/
+-rw-rw-rw-   0        0        0        0 2024-04-20 04:41:18.000000 ldjcourse-0.0.6/ldjcourse/pandas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:42:09.229723 ldjcourse-0.0.6/ldjcourse/pandas/v1_1/
+-rw-rw-rw-   0        0        0        0 2024-04-06 11:25:30.000000 ldjcourse-0.0.6/ldjcourse/pandas/v1_1/__init__.py
+-rw-rw-rw-   0        0        0      685 2024-04-21 15:42:07.000000 ldjcourse-0.0.6/ldjcourse/pandas/v1_1/api.py
+-rw-rw-rw-   0        0        0     1330 2024-04-20 07:04:45.000000 ldjcourse-0.0.6/ldjcourse/pandas/v1_1/data.py
+-rw-rw-rw-   0        0        0       22 2024-04-20 04:51:34.000000 ldjcourse-0.0.6/ldjcourse/pandas/v1_1/setting.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:42:09.243942 ldjcourse-0.0.6/ldjcourse.egg-info/
+-rw-rw-rw-   0        0        0      166 2024-04-21 15:42:08.000000 ldjcourse-0.0.6/ldjcourse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-04-21 15:42:09.000000 ldjcourse-0.0.6/ldjcourse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 15:42:08.000000 ldjcourse-0.0.6/ldjcourse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-21 15:42:08.000000 ldjcourse-0.0.6/ldjcourse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 15:42:09.256318 ldjcourse-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      580 2024-04-21 15:42:07.000000 ldjcourse-0.0.6/setup.py
```

### Comparing `ldjcourse-0.0.5/ldjcourse/pandas/v1_1/data.py` & `ldjcourse-0.0.6/ldjcourse/pandas/v1_1/data.py`

 * *Files identical despite different names*


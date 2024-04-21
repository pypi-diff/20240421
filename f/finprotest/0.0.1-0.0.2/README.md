# Comparing `tmp/finprotest-0.0.1.tar.gz` & `tmp/finprotest-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finprotest-0.0.1.tar", last modified: Sun Apr 21 10:51:32 2024, max compression
+gzip compressed data, was "finprotest-0.0.2.tar", last modified: Sun Apr 21 12:12:48 2024, max compression
```

## Comparing `finprotest-0.0.1.tar` & `finprotest-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 10:51:32.570872 finprotest-0.0.1/
--rw-rw-rw-   0        0        0     1093 2024-04-21 10:50:30.000000 finprotest-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      328 2024-04-21 10:51:32.569871 finprotest-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-04-21 10:50:41.000000 finprotest-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 10:51:32.568869 finprotest-0.0.1/finprotest.egg-info/
--rw-rw-rw-   0        0        0      328 2024-04-21 10:51:32.000000 finprotest-0.0.1/finprotest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-04-21 10:51:32.000000 finprotest-0.0.1/finprotest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 10:51:32.000000 finprotest-0.0.1/finprotest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-21 10:51:32.000000 finprotest-0.0.1/finprotest.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-21 10:51:32.566868 finprotest-0.0.1/iwanttest/
--rw-rw-rw-   0        0        0       16 2024-04-21 10:51:20.000000 finprotest-0.0.1/iwanttest/__init__.py
--rw-rw-rw-   0        0        0       72 2024-04-21 10:50:47.000000 finprotest-0.0.1/iwanttest/etc.py
--rw-rw-rw-   0        0        0      198 2024-04-21 10:50:53.000000 finprotest-0.0.1/iwanttest/test1.py
--rw-rw-rw-   0        0        0      145 2024-04-21 10:50:50.000000 finprotest-0.0.1/iwanttest/test2.py
--rw-rw-rw-   0        0        0       42 2024-04-21 10:51:32.571872 finprotest-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      488 2024-04-21 10:50:45.000000 finprotest-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 12:12:48.443117 finprotest-0.0.2/
+-rw-rw-rw-   0        0        0     1093 2024-04-21 10:50:30.000000 finprotest-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      328 2024-04-21 12:12:48.441114 finprotest-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-04-21 10:50:41.000000 finprotest-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 12:12:48.440113 finprotest-0.0.2/finprotest.egg-info/
+-rw-rw-rw-   0        0        0      328 2024-04-21 12:12:48.000000 finprotest-0.0.2/finprotest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-04-21 12:12:48.000000 finprotest-0.0.2/finprotest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 12:12:48.000000 finprotest-0.0.2/finprotest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-21 12:12:48.000000 finprotest-0.0.2/finprotest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 12:12:48.439112 finprotest-0.0.2/iwanttest/
+-rw-rw-rw-   0        0        0       16 2024-04-21 10:51:20.000000 finprotest-0.0.2/iwanttest/__init__.py
+-rw-rw-rw-   0        0        0       72 2024-04-21 10:50:47.000000 finprotest-0.0.2/iwanttest/etc.py
+-rw-rw-rw-   0        0        0      198 2024-04-21 10:50:53.000000 finprotest-0.0.2/iwanttest/test1.py
+-rw-rw-rw-   0        0        0      151 2024-04-21 12:07:00.000000 finprotest-0.0.2/iwanttest/test2.py
+-rw-rw-rw-   0        0        0       42 2024-04-21 12:12:48.443117 finprotest-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      488 2024-04-21 12:07:00.000000 finprotest-0.0.2/setup.py
```

### Comparing `finprotest-0.0.1/LICENSE` & `finprotest-0.0.2/LICENSE`

 * *Files identical despite different names*


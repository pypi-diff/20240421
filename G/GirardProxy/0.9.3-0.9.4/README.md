# Comparing `tmp/girardproxy-0.9.3.tar.gz` & `tmp/girardproxy-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girardproxy-0.9.3.tar", last modified: Sun Apr 21 09:49:19 2024, max compression
+gzip compressed data, was "girardproxy-0.9.4.tar", last modified: Sun Apr 21 09:54:30 2024, max compression
```

## Comparing `girardproxy-0.9.3.tar` & `girardproxy-0.9.4.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:19.114388 girardproxy-0.9.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:19.114388 girardproxy-0.9.3/GirardProxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-21 09:49:19.000000 girardproxy-0.9.3/GirardProxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-21 09:49:19.000000 girardproxy-0.9.3/GirardProxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:49:19.000000 girardproxy-0.9.3/GirardProxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-21 09:49:19.000000 girardproxy-0.9.3/GirardProxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:49:19.000000 girardproxy-0.9.3/GirardProxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 09:49:14.000000 girardproxy-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-21 09:49:19.114388 girardproxy-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 09:49:19.114388 girardproxy-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-21 09:49:14.000000 girardproxy-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:54:30.942509 girardproxy-0.9.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:54:30.942509 girardproxy-0.9.4/GirardProxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-21 09:54:30.000000 girardproxy-0.9.4/GirardProxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-21 09:54:30.000000 girardproxy-0.9.4/GirardProxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:54:30.000000 girardproxy-0.9.4/GirardProxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-21 09:54:30.000000 girardproxy-0.9.4/GirardProxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-21 09:54:30.000000 girardproxy-0.9.4/GirardProxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 09:54:27.000000 girardproxy-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-21 09:54:30.942509 girardproxy-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 09:54:30.942509 girardproxy-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-21 09:54:27.000000 girardproxy-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:54:30.942509 girardproxy-0.9.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:54:27.000000 girardproxy-0.9.4/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-21 09:54:27.000000 girardproxy-0.9.4/src/main.py
```

### Comparing `girardproxy-0.9.3/GirardProxy.egg-info/PKG-INFO` & `girardproxy-0.9.4/GirardProxy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GirardProxy
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python module that scrape and retrive working proxy addresses
 Author: Girard
 Author-email: girardhappy.it@gmail.com
 License: MIT
 Keywords: proxy scraper
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
```

### Comparing `girardproxy-0.9.3/LICENSE` & `girardproxy-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `girardproxy-0.9.3/PKG-INFO` & `girardproxy-0.9.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GirardProxy
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python module that scrape and retrive working proxy addresses
 Author: Girard
 Author-email: girardhappy.it@gmail.com
 License: MIT
 Keywords: proxy scraper
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
```


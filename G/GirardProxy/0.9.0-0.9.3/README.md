# Comparing `tmp/girardproxy-0.9.0.tar.gz` & `tmp/girardproxy-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girardproxy-0.9.0.tar", last modified: Sun Apr 21 09:32:42 2024, max compression
+gzip compressed data, was "girardproxy-0.9.3.tar", last modified: Sun Apr 21 09:49:19 2024, max compression
```

## Comparing `girardproxy-0.9.0.tar` & `girardproxy-0.9.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:32:42.717011 girardproxy-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:32:42.717011 girardproxy-0.9.0/GirardProxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-21 09:32:42.000000 girardproxy-0.9.0/GirardProxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-21 09:32:42.000000 girardproxy-0.9.0/GirardProxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:32:42.000000 girardproxy-0.9.0/GirardProxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-21 09:32:42.000000 girardproxy-0.9.0/GirardProxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:32:42.000000 girardproxy-0.9.0/GirardProxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 09:32:38.000000 girardproxy-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-21 09:32:42.717011 girardproxy-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 09:32:42.717011 girardproxy-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-21 09:32:38.000000 girardproxy-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:19.114388 girardproxy-0.9.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:19.114388 girardproxy-0.9.3/GirardProxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-21 09:49:19.000000 girardproxy-0.9.3/GirardProxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-21 09:49:19.000000 girardproxy-0.9.3/GirardProxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:49:19.000000 girardproxy-0.9.3/GirardProxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-21 09:49:19.000000 girardproxy-0.9.3/GirardProxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:49:19.000000 girardproxy-0.9.3/GirardProxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 09:49:14.000000 girardproxy-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-21 09:49:19.114388 girardproxy-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 09:49:19.114388 girardproxy-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-21 09:49:14.000000 girardproxy-0.9.3/setup.py
```

### Comparing `girardproxy-0.9.0/GirardProxy.egg-info/PKG-INFO` & `girardproxy-0.9.3/GirardProxy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GirardProxy
-Version: 0.9.0
+Version: 0.9.3
 Summary: Python module that scrape and retrive working proxy addresses
 Author: Girard
 Author-email: girardhappy.it@gmail.com
 License: MIT
 Keywords: proxy scraper
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
```

### Comparing `girardproxy-0.9.0/LICENSE` & `girardproxy-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `girardproxy-0.9.0/PKG-INFO` & `girardproxy-0.9.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GirardProxy
-Version: 0.9.0
+Version: 0.9.3
 Summary: Python module that scrape and retrive working proxy addresses
 Author: Girard
 Author-email: girardhappy.it@gmail.com
 License: MIT
 Keywords: proxy scraper
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
```

### Comparing `girardproxy-0.9.0/setup.py` & `girardproxy-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "GirardProxy",
-    version = "0.9.0",
+    version = "0.9.3",
     author = "Girard",
     author_email = "girardhappy.it@gmail.com",
     description = ("Python module that scrape and retrive working proxy addresses"),
     license = "MIT",
     keywords = "proxy scraper",
     packages=find_packages('src'),
     long_description="""A module that offer you the possibility to create an object that continuosly request proxies addresses, verify if they work using multithreading and retrive to you one of them <3""",
```


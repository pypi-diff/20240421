# Comparing `tmp/girardproxy-0.9.4.tar.gz` & `tmp/girardproxy-0.9.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girardproxy-0.9.4.tar", last modified: Sun Apr 21 09:54:30 2024, max compression
+gzip compressed data, was "girardproxy-0.9.41.tar", last modified: Sun Apr 21 10:18:03 2024, max compression
```

## Comparing `girardproxy-0.9.4.tar` & `girardproxy-0.9.41.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:54:30.942509 girardproxy-0.9.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:54:30.942509 girardproxy-0.9.4/GirardProxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-21 09:54:30.000000 girardproxy-0.9.4/GirardProxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-21 09:54:30.000000 girardproxy-0.9.4/GirardProxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:54:30.000000 girardproxy-0.9.4/GirardProxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-21 09:54:30.000000 girardproxy-0.9.4/GirardProxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-21 09:54:30.000000 girardproxy-0.9.4/GirardProxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 09:54:27.000000 girardproxy-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-21 09:54:30.942509 girardproxy-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 09:54:30.942509 girardproxy-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-21 09:54:27.000000 girardproxy-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:54:30.942509 girardproxy-0.9.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:54:27.000000 girardproxy-0.9.4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-21 09:54:27.000000 girardproxy-0.9.4/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:18:03.718453 girardproxy-0.9.41/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:18:03.718453 girardproxy-0.9.41/GirardProxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-21 10:18:03.000000 girardproxy-0.9.41/GirardProxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-21 10:18:03.000000 girardproxy-0.9.41/GirardProxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 10:18:03.000000 girardproxy-0.9.41/GirardProxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-21 10:18:03.000000 girardproxy-0.9.41/GirardProxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-21 10:18:03.000000 girardproxy-0.9.41/GirardProxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 10:17:58.000000 girardproxy-0.9.41/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-21 10:18:03.718453 girardproxy-0.9.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 10:18:03.718453 girardproxy-0.9.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-21 10:17:58.000000 girardproxy-0.9.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:18:03.718453 girardproxy-0.9.41/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 10:17:58.000000 girardproxy-0.9.41/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-21 10:17:58.000000 girardproxy-0.9.41/src/main.py
```

### Comparing `girardproxy-0.9.4/GirardProxy.egg-info/PKG-INFO` & `girardproxy-0.9.41/GirardProxy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GirardProxy
-Version: 0.9.4
+Version: 0.9.41
 Summary: Python module that scrape and retrive working proxy addresses
 Author: Girard
 Author-email: girardhappy.it@gmail.com
 License: MIT
 Keywords: proxy scraper
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
```

### Comparing `girardproxy-0.9.4/LICENSE` & `girardproxy-0.9.41/LICENSE`

 * *Files identical despite different names*

### Comparing `girardproxy-0.9.4/PKG-INFO` & `girardproxy-0.9.41/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GirardProxy
-Version: 0.9.4
+Version: 0.9.41
 Summary: Python module that scrape and retrive working proxy addresses
 Author: Girard
 Author-email: girardhappy.it@gmail.com
 License: MIT
 Keywords: proxy scraper
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
```

### Comparing `girardproxy-0.9.4/setup.py` & `girardproxy-0.9.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "GirardProxy",
-    version = "0.9.4",
+    version = "0.9.41",
     author = "Girard",
     author_email = "girardhappy.it@gmail.com",
     description = ("Python module that scrape and retrive working proxy addresses"),
     license = "MIT",
     keywords = "proxy scraper",
     packages=['src'],
     long_description="""A module that offer you the possibility to create an object that continuosly request proxies addresses, verify if they work using multithreading and retrive to you one of them <3""",
```

### Comparing `girardproxy-0.9.4/src/main.py` & `girardproxy-0.9.41/src/main.py`

 * *Files identical despite different names*


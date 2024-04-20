# Comparing `tmp/ryutils-4.0.5.tar.gz` & `tmp/ryutils-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryutils-4.0.5.tar", last modified: Sat Apr 20 22:15:14 2024, max compression
+gzip compressed data, was "ryutils-4.1.0.tar", last modified: Sat Apr 20 22:44:48 2024, max compression
```

## Comparing `ryutils-4.0.5.tar` & `ryutils-4.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:15:14.813786 ryutils-4.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 22:15:10.000000 ryutils-4.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 22:15:10.000000 ryutils-4.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 22:15:14.813786 ryutils-4.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-20 22:15:10.000000 ryutils-4.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 22:15:10.000000 ryutils-4.0.5/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-20 22:15:10.000000 ryutils-4.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-20 22:15:10.000000 ryutils-4.0.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:15:14.813786 ryutils-4.0.5/ryutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:15:10.000000 ryutils-4.0.5/ryutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 22:15:10.000000 ryutils-4.0.5/ryutils/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-20 22:15:10.000000 ryutils-4.0.5/ryutils/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-20 22:15:10.000000 ryutils-4.0.5/ryutils/dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-20 22:15:10.000000 ryutils-4.0.5/ryutils/email_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-20 22:15:10.000000 ryutils-4.0.5/ryutils/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-20 22:15:10.000000 ryutils-4.0.5/ryutils/fmt_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12462 2024-04-20 22:15:10.000000 ryutils-4.0.5/ryutils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-20 22:15:10.000000 ryutils-4.0.5/ryutils/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:15:10.000000 ryutils-4.0.5/ryutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-20 22:15:10.000000 ryutils-4.0.5/ryutils/short_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:15:14.813786 ryutils-4.0.5/ryutils/sms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:15:10.000000 ryutils-4.0.5/ryutils/sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-20 22:15:10.000000 ryutils-4.0.5/ryutils/sms/telegram_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-20 22:15:10.000000 ryutils-4.0.5/ryutils/sms/twilio_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-20 22:15:10.000000 ryutils-4.0.5/ryutils/wait.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-20 22:15:10.000000 ryutils-4.0.5/ryutils/web2_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:15:14.813786 ryutils-4.0.5/ryutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 22:15:14.000000 ryutils-4.0.5/ryutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-20 22:15:14.000000 ryutils-4.0.5/ryutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 22:15:14.000000 ryutils-4.0.5/ryutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 22:15:14.000000 ryutils-4.0.5/ryutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 22:15:14.000000 ryutils-4.0.5/ryutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 22:15:14.813786 ryutils-4.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-20 22:15:10.000000 ryutils-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:44:48.490510 ryutils-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 22:44:41.000000 ryutils-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 22:44:41.000000 ryutils-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 22:44:48.490510 ryutils-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-20 22:44:41.000000 ryutils-4.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 22:44:41.000000 ryutils-4.1.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-20 22:44:41.000000 ryutils-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-20 22:44:41.000000 ryutils-4.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:44:48.486510 ryutils-4.1.0/ryutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:44:41.000000 ryutils-4.1.0/ryutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 22:44:41.000000 ryutils-4.1.0/ryutils/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-20 22:44:41.000000 ryutils-4.1.0/ryutils/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-20 22:44:41.000000 ryutils-4.1.0/ryutils/dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-20 22:44:41.000000 ryutils-4.1.0/ryutils/email_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-20 22:44:41.000000 ryutils-4.1.0/ryutils/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-20 22:44:41.000000 ryutils-4.1.0/ryutils/fmt_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12462 2024-04-20 22:44:41.000000 ryutils-4.1.0/ryutils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-20 22:44:41.000000 ryutils-4.1.0/ryutils/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:44:41.000000 ryutils-4.1.0/ryutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-20 22:44:41.000000 ryutils-4.1.0/ryutils/short_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:44:48.490510 ryutils-4.1.0/ryutils/sms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:44:41.000000 ryutils-4.1.0/ryutils/sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-20 22:44:41.000000 ryutils-4.1.0/ryutils/sms/telegram_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-20 22:44:41.000000 ryutils-4.1.0/ryutils/sms/twilio_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-20 22:44:41.000000 ryutils-4.1.0/ryutils/wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-20 22:44:41.000000 ryutils-4.1.0/ryutils/web2_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:44:48.490510 ryutils-4.1.0/ryutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 22:44:48.000000 ryutils-4.1.0/ryutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-20 22:44:48.000000 ryutils-4.1.0/ryutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 22:44:48.000000 ryutils-4.1.0/ryutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 22:44:48.000000 ryutils-4.1.0/ryutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 22:44:48.000000 ryutils-4.1.0/ryutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 22:44:48.490510 ryutils-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-20 22:44:41.000000 ryutils-4.1.0/setup.py
```

### Comparing `ryutils-4.0.5/LICENSE` & `ryutils-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.5/PKG-INFO` & `ryutils-4.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryutils
-Version: 4.0.5
+Version: 4.1.0
 Summary: A collection of utilities for Python
 Author: Ross Yeager
 Author-email: ryeager12@email.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ryutils-4.0.5/pyproject.toml` & `ryutils-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.5/requirements.txt` & `ryutils-4.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.5/ryutils/async_utils.py` & `ryutils-4.1.0/ryutils/async_utils.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.5/ryutils/csv_logger.py` & `ryutils-4.1.0/ryutils/csv_logger.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.5/ryutils/dict_util.py` & `ryutils-4.1.0/ryutils/dict_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.5/ryutils/email_util.py` & `ryutils-4.1.0/ryutils/email_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.5/ryutils/fmt_util.py` & `ryutils-4.1.0/ryutils/fmt_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.5/ryutils/log.py` & `ryutils-4.1.0/ryutils/log.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.5/ryutils/proxies.py` & `ryutils-4.1.0/ryutils/proxies.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,11 +31,11 @@
 
 class FreeProxyProxy(Proxies):
     """
     https://pypi.org/project/free-proxy/
     """
 
     def get(self, verbose: bool = False) -> T.Dict[str, str]:
-        proxy = {"http": FreeProxy(rand=True).get()}
+        proxy = {"http": FreeProxy(rand=True, https=True).get()}
         if verbose:
             log.print_bright(f"Using proxy: {proxy}")
         return proxy
```

### Comparing `ryutils-4.0.5/ryutils/sms/telegram_util.py` & `ryutils-4.1.0/ryutils/sms/telegram_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.5/ryutils/sms/twilio_util.py` & `ryutils-4.1.0/ryutils/sms/twilio_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.5/ryutils/web2_client.py` & `ryutils-4.1.0/ryutils/web2_client.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.5/ryutils.egg-info/PKG-INFO` & `ryutils-4.1.0/ryutils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryutils
-Version: 4.0.5
+Version: 4.1.0
 Summary: A collection of utilities for Python
 Author: Ross Yeager
 Author-email: ryeager12@email.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ryutils-4.0.5/ryutils.egg-info/SOURCES.txt` & `ryutils-4.1.0/ryutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.5/setup.py` & `ryutils-4.1.0/setup.py`

 * *Files identical despite different names*


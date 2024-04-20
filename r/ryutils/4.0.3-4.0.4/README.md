# Comparing `tmp/ryutils-4.0.3.tar.gz` & `tmp/ryutils-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryutils-4.0.3.tar", last modified: Sat Apr 20 18:11:32 2024, max compression
+gzip compressed data, was "ryutils-4.0.4.tar", last modified: Sat Apr 20 18:22:31 2024, max compression
```

## Comparing `ryutils-4.0.3.tar` & `ryutils-4.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:11:32.064527 ryutils-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 18:11:23.000000 ryutils-4.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 18:11:23.000000 ryutils-4.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 18:11:32.064527 ryutils-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-20 18:11:23.000000 ryutils-4.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 18:11:23.000000 ryutils-4.0.3/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-20 18:11:23.000000 ryutils-4.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-20 18:11:23.000000 ryutils-4.0.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:11:32.064527 ryutils-4.0.3/ryutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/email_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/fmt_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12360 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/short_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:11:32.064527 ryutils-4.0.3/ryutils/sms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/sms/telegram_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/sms/twilio_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/wait.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/web2_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:11:32.064527 ryutils-4.0.3/ryutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 18:11:32.000000 ryutils-4.0.3/ryutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-20 18:11:32.000000 ryutils-4.0.3/ryutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:11:32.000000 ryutils-4.0.3/ryutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 18:11:32.000000 ryutils-4.0.3/ryutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 18:11:32.000000 ryutils-4.0.3/ryutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:11:32.064527 ryutils-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-20 18:11:23.000000 ryutils-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:22:31.033973 ryutils-4.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 18:22:27.000000 ryutils-4.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 18:22:27.000000 ryutils-4.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 18:22:31.033973 ryutils-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-20 18:22:27.000000 ryutils-4.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 18:22:27.000000 ryutils-4.0.4/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-20 18:22:27.000000 ryutils-4.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-20 18:22:27.000000 ryutils-4.0.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:22:31.029973 ryutils-4.0.4/ryutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:22:27.000000 ryutils-4.0.4/ryutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 18:22:27.000000 ryutils-4.0.4/ryutils/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-20 18:22:27.000000 ryutils-4.0.4/ryutils/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-20 18:22:27.000000 ryutils-4.0.4/ryutils/dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-20 18:22:27.000000 ryutils-4.0.4/ryutils/email_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-20 18:22:27.000000 ryutils-4.0.4/ryutils/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-20 18:22:27.000000 ryutils-4.0.4/ryutils/fmt_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12462 2024-04-20 18:22:27.000000 ryutils-4.0.4/ryutils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-20 18:22:27.000000 ryutils-4.0.4/ryutils/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:22:27.000000 ryutils-4.0.4/ryutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-20 18:22:27.000000 ryutils-4.0.4/ryutils/short_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:22:31.033973 ryutils-4.0.4/ryutils/sms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:22:27.000000 ryutils-4.0.4/ryutils/sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-20 18:22:27.000000 ryutils-4.0.4/ryutils/sms/telegram_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-20 18:22:27.000000 ryutils-4.0.4/ryutils/sms/twilio_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-20 18:22:27.000000 ryutils-4.0.4/ryutils/wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-20 18:22:27.000000 ryutils-4.0.4/ryutils/web2_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:22:31.033973 ryutils-4.0.4/ryutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 18:22:31.000000 ryutils-4.0.4/ryutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-20 18:22:31.000000 ryutils-4.0.4/ryutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:22:31.000000 ryutils-4.0.4/ryutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 18:22:31.000000 ryutils-4.0.4/ryutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 18:22:31.000000 ryutils-4.0.4/ryutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:22:31.033973 ryutils-4.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-20 18:22:27.000000 ryutils-4.0.4/setup.py
```

### Comparing `ryutils-4.0.3/LICENSE` & `ryutils-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.3/PKG-INFO` & `ryutils-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryutils
-Version: 4.0.3
+Version: 4.0.4
 Summary: A collection of utilities for Python
 Author: Ross Yeager
 Author-email: ryeager12@email.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ryutils-4.0.3/pyproject.toml` & `ryutils-4.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.3/requirements.txt` & `ryutils-4.0.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.3/ryutils/async_utils.py` & `ryutils-4.0.4/ryutils/async_utils.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.3/ryutils/csv_logger.py` & `ryutils-4.0.4/ryutils/csv_logger.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.3/ryutils/dict_util.py` & `ryutils-4.0.4/ryutils/dict_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.3/ryutils/email_util.py` & `ryutils-4.0.4/ryutils/email_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.3/ryutils/fmt_util.py` & `ryutils-4.0.4/ryutils/fmt_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.3/ryutils/log.py` & `ryutils-4.0.4/ryutils/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,21 +119,27 @@
 def get_log_dir_name(log_dir: str) -> str:
     current_log_dir_name = time.strftime("%Y_%m_%d__%H_%M_%S", time.localtime(time.time()))
     updated_log_dir = os.path.join(log_dir, "logs", current_log_dir_name)
     make_sure_path_exists(path=updated_log_dir)
     return updated_log_dir
 
 
-def setup(log_dir: str, log_level: str, main_thread_name: str) -> None:
+def setup(
+    log_dir: str,
+    log_level: str,
+    main_thread_name: str,
+    always_print: bool = False,
+    downsample_count: int = 1,
+):
     if not os.path.isdir(log_dir):
         os.mkdir(log_dir)
 
     new_log_dir = get_log_dir_name(log_dir)
 
-    setup_log(log_level, new_log_dir, main_thread_name)
+    setup_log(log_level, new_log_dir, main_thread_name, always_print, downsample_count)
 
     logging.getLogger().addHandler(
         MultiHandler(
             new_log_dir,
             ["ThreadPool", "MainThread"],
         )
     )
```

### Comparing `ryutils-4.0.3/ryutils/proxies.py` & `ryutils-4.0.4/ryutils/proxies.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.3/ryutils/sms/telegram_util.py` & `ryutils-4.0.4/ryutils/sms/telegram_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.3/ryutils/sms/twilio_util.py` & `ryutils-4.0.4/ryutils/sms/twilio_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.3/ryutils/web2_client.py` & `ryutils-4.0.4/ryutils/web2_client.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.3/ryutils.egg-info/PKG-INFO` & `ryutils-4.0.4/ryutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryutils
-Version: 4.0.3
+Version: 4.0.4
 Summary: A collection of utilities for Python
 Author: Ross Yeager
 Author-email: ryeager12@email.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ryutils-4.0.3/ryutils.egg-info/SOURCES.txt` & `ryutils-4.0.4/ryutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.3/setup.py` & `ryutils-4.0.4/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/galxiai-0.50.7.tar.gz` & `tmp/galxiai-0.50.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galxiai-0.50.7.tar", last modified: Sun Apr 21 14:53:31 2024, max compression
+gzip compressed data, was "galxiai-0.50.8.tar", last modified: Sun Apr 21 14:59:47 2024, max compression
```

## Comparing `galxiai-0.50.7.tar` & `galxiai-0.50.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 14:53:31.382381 galxiai-0.50.7/
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 galxiai-0.50.7/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      909 2024-04-21 14:53:31.382220 galxiai-0.50.7/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)       64 2024-04-21 07:45:09.000000 galxiai-0.50.7/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 14:53:31.378836 galxiai-0.50.7/galxiai/
--rw-r--r--   0 root         (0) staff       (20)     1321 2024-04-21 14:53:31.000000 galxiai-0.50.7/galxiai/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8647 2024-04-21 07:24:58.000000 galxiai-0.50.7/galxiai/clasreq.py
--rw-r--r--   0 root         (0) staff       (20)     2553 2024-04-21 07:49:17.000000 galxiai-0.50.7/galxiai/const.py
--rw-r--r--   0 root         (0) staff       (20)    15573 2024-04-21 12:50:09.000000 galxiai-0.50.7/galxiai/payload.py
--rw-r--r--   0 root         (0) staff       (20)    35439 2024-04-21 10:28:30.000000 galxiai-0.50.7/galxiai/ql.py
--rw-r--r--   0 root         (0) staff       (20)    12894 2024-04-21 11:24:00.000000 galxiai-0.50.7/galxiai/req.py
--rw-r--r--   0 root         (0) staff       (20)     3265 2024-04-21 07:32:34.000000 galxiai-0.50.7/galxiai/reqbase.py
--rw-r--r--   0 root         (0) staff       (20)    30753 2024-04-21 09:20:35.000000 galxiai-0.50.7/galxiai/sqlite_galxi.py
--rw-r--r--   0 root         (0) staff       (20)     2519 2024-04-21 11:46:34.000000 galxiai-0.50.7/galxiai/ut.py
--rw-r--r--   0 root         (0) staff       (20)     5485 2024-04-21 07:34:26.000000 galxiai-0.50.7/galxiai/xxcl.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 14:53:31.381667 galxiai-0.50.7/galxiai.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      909 2024-04-21 14:53:31.000000 galxiai-0.50.7/galxiai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      367 2024-04-21 14:53:31.000000 galxiai-0.50.7/galxiai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-21 14:53:31.000000 galxiai-0.50.7/galxiai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       30 2024-04-21 14:53:31.000000 galxiai-0.50.7/galxiai.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        8 2024-04-21 14:53:31.000000 galxiai-0.50.7/galxiai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-04-21 14:53:31.382925 galxiai-0.50.7/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2484 2024-04-21 07:48:41.000000 galxiai-0.50.7/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 14:59:47.211858 galxiai-0.50.8/
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 galxiai-0.50.8/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      909 2024-04-21 14:59:47.211616 galxiai-0.50.8/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)       64 2024-04-21 07:45:09.000000 galxiai-0.50.8/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 14:59:47.203398 galxiai-0.50.8/galxiai/
+-rw-r--r--   0 root         (0) staff       (20)     1321 2024-04-21 14:59:46.000000 galxiai-0.50.8/galxiai/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8647 2024-04-21 07:24:58.000000 galxiai-0.50.8/galxiai/clasreq.py
+-rw-r--r--   0 root         (0) staff       (20)     2553 2024-04-21 07:49:17.000000 galxiai-0.50.8/galxiai/const.py
+-rw-r--r--   0 root         (0) staff       (20)    15682 2024-04-21 14:59:36.000000 galxiai-0.50.8/galxiai/payload.py
+-rw-r--r--   0 root         (0) staff       (20)    35439 2024-04-21 10:28:30.000000 galxiai-0.50.8/galxiai/ql.py
+-rw-r--r--   0 root         (0) staff       (20)    12894 2024-04-21 11:24:00.000000 galxiai-0.50.8/galxiai/req.py
+-rw-r--r--   0 root         (0) staff       (20)     3265 2024-04-21 07:32:34.000000 galxiai-0.50.8/galxiai/reqbase.py
+-rw-r--r--   0 root         (0) staff       (20)    30753 2024-04-21 09:20:35.000000 galxiai-0.50.8/galxiai/sqlite_galxi.py
+-rw-r--r--   0 root         (0) staff       (20)     2519 2024-04-21 11:46:34.000000 galxiai-0.50.8/galxiai/ut.py
+-rw-r--r--   0 root         (0) staff       (20)     5485 2024-04-21 07:34:26.000000 galxiai-0.50.8/galxiai/xxcl.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 14:59:47.210930 galxiai-0.50.8/galxiai.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      909 2024-04-21 14:59:47.000000 galxiai-0.50.8/galxiai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      367 2024-04-21 14:59:47.000000 galxiai-0.50.8/galxiai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-21 14:59:47.000000 galxiai-0.50.8/galxiai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       30 2024-04-21 14:59:47.000000 galxiai-0.50.8/galxiai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        8 2024-04-21 14:59:47.000000 galxiai-0.50.8/galxiai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-21 14:59:47.213087 galxiai-0.50.8/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2484 2024-04-21 07:48:41.000000 galxiai-0.50.8/setup.py
```

### Comparing `galxiai-0.50.7/LICENSE` & `galxiai-0.50.8/LICENSE`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.7/PKG-INFO` & `galxiai-0.50.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galxiai
-Version: 0.50.7
+Version: 0.50.8
 Summary: A Python package to manage all my cash in one hand
 Home-page: https://github.com/djsola/galxiai/
 Author: Jun-You MIT & Solomon
 Author-email: solomon@tmp.o66p.com
 License: MIT
 Keywords: ssh galxiai room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `galxiai-0.50.7/galxiai/__init__.py` & `galxiai-0.50.8/galxiai/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.50.7'
+__version__ = '0.50.8'
```

### Comparing `galxiai-0.50.7/galxiai/clasreq.py` & `galxiai-0.50.8/galxiai/clasreq.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.7/galxiai/const.py` & `galxiai-0.50.8/galxiai/const.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.7/galxiai/payload.py` & `galxiai-0.50.8/galxiai/payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,24 +237,28 @@
         return ""
 
     def twitter_verification_message(self):
         user_id = self.db.get_key_res("id")
         return f"Verifying my Twitter account for my #GalxeID gid:{user_id} @Galxe"
 
     def action_twitter_ac_bind(self):
-        if self.db.res_true("hasTwitter") is False:
-            print("============= confirm twitter ac")
+        if self.db.res_true("hasTwitter") is True:
+            print("twitter ac bound.")
+            return
+
+        print("============= confirm twitter ac")
         url = self.action_twitter_action_post_twitter(self.twitter_verification_message())
         _doc = galxeQL(self.session, rq_data_fill_twitter_ac(self.wallet_erc.address, url))
         if "twitterUserID" in _doc and "twitterUserName" in _doc:
             print(".ok 1")
         _doc = galxeQL(self.session, rq_data_twitter_verify(self.wallet_erc.address, url))
         if "twitterUserID" in _doc and "twitterUserName" in _doc:
             print(".ok 2")
-
+            
+        print("twitter is just ac bound.")
         self.action_get_profile()
 
     def action_email_confirm(self):
         print("============= confirm email")
         _doc = None
 
         if self.db.is_email_sent() is False:
```

### Comparing `galxiai-0.50.7/galxiai/ql.py` & `galxiai-0.50.8/galxiai/ql.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.7/galxiai/req.py` & `galxiai-0.50.8/galxiai/req.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.7/galxiai/reqbase.py` & `galxiai-0.50.8/galxiai/reqbase.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.7/galxiai/sqlite_galxi.py` & `galxiai-0.50.8/galxiai/sqlite_galxi.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.7/galxiai/ut.py` & `galxiai-0.50.8/galxiai/ut.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.7/galxiai/xxcl.py` & `galxiai-0.50.8/galxiai/xxcl.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.7/galxiai.egg-info/PKG-INFO` & `galxiai-0.50.8/galxiai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galxiai
-Version: 0.50.7
+Version: 0.50.8
 Summary: A Python package to manage all my cash in one hand
 Home-page: https://github.com/djsola/galxiai/
 Author: Jun-You MIT & Solomon
 Author-email: solomon@tmp.o66p.com
 License: MIT
 Keywords: ssh galxiai room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `galxiai-0.50.7/setup.py` & `galxiai-0.50.8/setup.py`

 * *Files identical despite different names*


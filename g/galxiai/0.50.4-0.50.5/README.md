# Comparing `tmp/galxiai-0.50.4.tar.gz` & `tmp/galxiai-0.50.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galxiai-0.50.4.tar", last modified: Sun Apr 21 09:21:08 2024, max compression
+gzip compressed data, was "galxiai-0.50.5.tar", last modified: Sun Apr 21 09:38:24 2024, max compression
```

## Comparing `galxiai-0.50.4.tar` & `galxiai-0.50.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 09:21:08.711441 galxiai-0.50.4/
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 galxiai-0.50.4/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      909 2024-04-21 09:21:08.711223 galxiai-0.50.4/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)       64 2024-04-21 07:45:09.000000 galxiai-0.50.4/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 09:21:08.707709 galxiai-0.50.4/galxiai/
--rw-r--r--   0 root         (0) staff       (20)     1321 2024-04-21 09:21:08.000000 galxiai-0.50.4/galxiai/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8647 2024-04-21 07:24:58.000000 galxiai-0.50.4/galxiai/clasreq.py
--rw-r--r--   0 root         (0) staff       (20)     2553 2024-04-21 07:49:17.000000 galxiai-0.50.4/galxiai/const.py
--rw-r--r--   0 root         (0) staff       (20)    14575 2024-04-21 07:39:24.000000 galxiai-0.50.4/galxiai/payload.py
--rw-r--r--   0 root         (0) staff       (20)    35030 2024-04-10 04:51:14.000000 galxiai-0.50.4/galxiai/ql.py
--rw-r--r--   0 root         (0) staff       (20)    12062 2024-04-21 07:36:19.000000 galxiai-0.50.4/galxiai/req.py
--rw-r--r--   0 root         (0) staff       (20)     3265 2024-04-21 07:32:34.000000 galxiai-0.50.4/galxiai/reqbase.py
--rw-r--r--   0 root         (0) staff       (20)    30753 2024-04-21 09:20:35.000000 galxiai-0.50.4/galxiai/sqlite_galxi.py
--rw-r--r--   0 root         (0) staff       (20)     1845 2024-04-21 07:36:19.000000 galxiai-0.50.4/galxiai/ut.py
--rw-r--r--   0 root         (0) staff       (20)     5485 2024-04-21 07:34:26.000000 galxiai-0.50.4/galxiai/xxcl.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 09:21:08.710665 galxiai-0.50.4/galxiai.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      909 2024-04-21 09:21:08.000000 galxiai-0.50.4/galxiai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      367 2024-04-21 09:21:08.000000 galxiai-0.50.4/galxiai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-21 09:21:08.000000 galxiai-0.50.4/galxiai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       30 2024-04-21 09:21:08.000000 galxiai-0.50.4/galxiai.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        8 2024-04-21 09:21:08.000000 galxiai-0.50.4/galxiai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-04-21 09:21:08.712124 galxiai-0.50.4/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2484 2024-04-21 07:48:41.000000 galxiai-0.50.4/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 09:38:24.940632 galxiai-0.50.5/
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 galxiai-0.50.5/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      909 2024-04-21 09:38:24.940467 galxiai-0.50.5/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)       64 2024-04-21 07:45:09.000000 galxiai-0.50.5/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 09:38:24.936759 galxiai-0.50.5/galxiai/
+-rw-r--r--   0 root         (0) staff       (20)     1321 2024-04-21 09:38:24.000000 galxiai-0.50.5/galxiai/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8647 2024-04-21 07:24:58.000000 galxiai-0.50.5/galxiai/clasreq.py
+-rw-r--r--   0 root         (0) staff       (20)     2553 2024-04-21 07:49:17.000000 galxiai-0.50.5/galxiai/const.py
+-rw-r--r--   0 root         (0) staff       (20)    14533 2024-04-21 09:38:07.000000 galxiai-0.50.5/galxiai/payload.py
+-rw-r--r--   0 root         (0) staff       (20)    35030 2024-04-10 04:51:14.000000 galxiai-0.50.5/galxiai/ql.py
+-rw-r--r--   0 root         (0) staff       (20)    12062 2024-04-21 07:36:19.000000 galxiai-0.50.5/galxiai/req.py
+-rw-r--r--   0 root         (0) staff       (20)     3265 2024-04-21 07:32:34.000000 galxiai-0.50.5/galxiai/reqbase.py
+-rw-r--r--   0 root         (0) staff       (20)    30753 2024-04-21 09:20:35.000000 galxiai-0.50.5/galxiai/sqlite_galxi.py
+-rw-r--r--   0 root         (0) staff       (20)     1845 2024-04-21 07:36:19.000000 galxiai-0.50.5/galxiai/ut.py
+-rw-r--r--   0 root         (0) staff       (20)     5485 2024-04-21 07:34:26.000000 galxiai-0.50.5/galxiai/xxcl.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 09:38:24.939920 galxiai-0.50.5/galxiai.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      909 2024-04-21 09:38:24.000000 galxiai-0.50.5/galxiai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      367 2024-04-21 09:38:24.000000 galxiai-0.50.5/galxiai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-21 09:38:24.000000 galxiai-0.50.5/galxiai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       30 2024-04-21 09:38:24.000000 galxiai-0.50.5/galxiai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        8 2024-04-21 09:38:24.000000 galxiai-0.50.5/galxiai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-21 09:38:24.941195 galxiai-0.50.5/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2484 2024-04-21 07:48:41.000000 galxiai-0.50.5/setup.py
```

### Comparing `galxiai-0.50.4/LICENSE` & `galxiai-0.50.5/LICENSE`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.4/PKG-INFO` & `galxiai-0.50.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galxiai
-Version: 0.50.4
+Version: 0.50.5
 Summary: A Python package to manage all my cash in one hand
 Home-page: https://github.com/djsola/galxiai/
 Author: Jun-You MIT & Solomon
 Author-email: solomon@tmp.o66p.com
 License: MIT
 Keywords: ssh galxiai room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `galxiai-0.50.4/galxiai/__init__.py` & `galxiai-0.50.5/galxiai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.50.4'
+__version__ = '0.50.5'
```

### Comparing `galxiai-0.50.4/galxiai/clasreq.py` & `galxiai-0.50.5/galxiai/clasreq.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.4/galxiai/const.py` & `galxiai-0.50.5/galxiai/const.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.4/galxiai/payload.py` & `galxiai-0.50.5/galxiai/payload.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,22 +190,25 @@
                 if "credentials" in h:
                     f = h["credentials"]
                     if len(f) > 0:
                         action_call = f[0]
                         do_url = action_call["referenceLink"]
                         cred_it = action_call["id"]
                         sync = action_call["lastSync"]
-                        call_to_actions.append((
-                            cred_it, do_url
-                        ))
-                        if self.db.is_check_point_ready(cred_it) is True or sync == 0:
+                        if self.check_perform_action(camp_id, cred_it, do_url, sync):
                             print("do task", cred_it, do_url)
+                            call_to_actions.append((
+                                cred_it, do_url
+                            ))
                             self.action_call_add_cred(cred_it, camp_id)
         self.tasks = call_to_actions
 
+    def check_perform_action(self, camp_id, cred_id, do_url, sync) -> bool:
+        return self.db.is_check_point_ready(cred_id) is True or sync == 0
+
     def action_check_credentials(self):
         if len(self.tasks) == 0:
             return
         for task_mission in self.tasks:
             (cred_id, url) = task_mission
             if self.db.check_claim_ready(cred_id) is False:
                 raise WaitForClaimPoint()
@@ -342,19 +345,14 @@
             if _doc["galxeIdExist"] is False:
                 print("galxe id is not exist.")
         else:
             Galxi.BEARER = bearer_x
             self.action_check_jwt()
         self.action_register_username()
 
-    def action_fast_account_email(self):
-        found_address_rec = self.db.has_the_address(self.wallet_erc.address)
-        if found_address_rec is True:
-            self.action_checked_email_solana()
-
     def log_failed_verifications(self):
         self.db.log_failed_verifications()
 
     def profile_res_check(self, _d):
         try:
             _info = _d["addressInfo"]
             self.db.update_res_set({
```

### Comparing `galxiai-0.50.4/galxiai/ql.py` & `galxiai-0.50.5/galxiai/ql.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.4/galxiai/req.py` & `galxiai-0.50.5/galxiai/req.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.4/galxiai/reqbase.py` & `galxiai-0.50.5/galxiai/reqbase.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.4/galxiai/sqlite_galxi.py` & `galxiai-0.50.5/galxiai/sqlite_galxi.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.4/galxiai/ut.py` & `galxiai-0.50.5/galxiai/ut.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.4/galxiai/xxcl.py` & `galxiai-0.50.5/galxiai/xxcl.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.4/galxiai.egg-info/PKG-INFO` & `galxiai-0.50.5/galxiai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galxiai
-Version: 0.50.4
+Version: 0.50.5
 Summary: A Python package to manage all my cash in one hand
 Home-page: https://github.com/djsola/galxiai/
 Author: Jun-You MIT & Solomon
 Author-email: solomon@tmp.o66p.com
 License: MIT
 Keywords: ssh galxiai room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `galxiai-0.50.4/setup.py` & `galxiai-0.50.5/setup.py`

 * *Files identical despite different names*


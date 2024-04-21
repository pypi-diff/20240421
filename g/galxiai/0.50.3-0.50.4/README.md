# Comparing `tmp/galxiai-0.50.3.tar.gz` & `tmp/galxiai-0.50.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galxiai-0.50.3.tar", last modified: Sun Apr 21 07:50:17 2024, max compression
+gzip compressed data, was "galxiai-0.50.4.tar", last modified: Sun Apr 21 09:21:08 2024, max compression
```

## Comparing `galxiai-0.50.3.tar` & `galxiai-0.50.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 07:50:17.734290 galxiai-0.50.3/
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 galxiai-0.50.3/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      909 2024-04-21 07:50:17.734064 galxiai-0.50.3/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)       64 2024-04-21 07:45:09.000000 galxiai-0.50.3/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 07:50:17.728523 galxiai-0.50.3/galxiai/
--rw-r--r--   0 root         (0) staff       (20)     1321 2024-04-21 07:50:17.000000 galxiai-0.50.3/galxiai/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8647 2024-04-21 07:24:58.000000 galxiai-0.50.3/galxiai/clasreq.py
--rw-r--r--   0 root         (0) staff       (20)     2553 2024-04-21 07:49:17.000000 galxiai-0.50.3/galxiai/const.py
--rw-r--r--   0 root         (0) staff       (20)    14575 2024-04-21 07:39:24.000000 galxiai-0.50.3/galxiai/payload.py
--rw-r--r--   0 root         (0) staff       (20)    35030 2024-04-10 04:51:14.000000 galxiai-0.50.3/galxiai/ql.py
--rw-r--r--   0 root         (0) staff       (20)    12062 2024-04-21 07:36:19.000000 galxiai-0.50.3/galxiai/req.py
--rw-r--r--   0 root         (0) staff       (20)     3265 2024-04-21 07:32:34.000000 galxiai-0.50.3/galxiai/reqbase.py
--rw-r--r--   0 root         (0) staff       (20)    30978 2024-04-21 07:39:24.000000 galxiai-0.50.3/galxiai/sqlite_galxi.py
--rw-r--r--   0 root         (0) staff       (20)     1845 2024-04-21 07:36:19.000000 galxiai-0.50.3/galxiai/ut.py
--rw-r--r--   0 root         (0) staff       (20)     5485 2024-04-21 07:34:26.000000 galxiai-0.50.3/galxiai/xxcl.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 07:50:17.733142 galxiai-0.50.3/galxiai.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      909 2024-04-21 07:50:17.000000 galxiai-0.50.3/galxiai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      367 2024-04-21 07:50:17.000000 galxiai-0.50.3/galxiai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-21 07:50:17.000000 galxiai-0.50.3/galxiai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       30 2024-04-21 07:50:17.000000 galxiai-0.50.3/galxiai.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        8 2024-04-21 07:50:17.000000 galxiai-0.50.3/galxiai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-04-21 07:50:17.735177 galxiai-0.50.3/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2484 2024-04-21 07:48:41.000000 galxiai-0.50.3/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 09:21:08.711441 galxiai-0.50.4/
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 galxiai-0.50.4/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      909 2024-04-21 09:21:08.711223 galxiai-0.50.4/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)       64 2024-04-21 07:45:09.000000 galxiai-0.50.4/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 09:21:08.707709 galxiai-0.50.4/galxiai/
+-rw-r--r--   0 root         (0) staff       (20)     1321 2024-04-21 09:21:08.000000 galxiai-0.50.4/galxiai/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8647 2024-04-21 07:24:58.000000 galxiai-0.50.4/galxiai/clasreq.py
+-rw-r--r--   0 root         (0) staff       (20)     2553 2024-04-21 07:49:17.000000 galxiai-0.50.4/galxiai/const.py
+-rw-r--r--   0 root         (0) staff       (20)    14575 2024-04-21 07:39:24.000000 galxiai-0.50.4/galxiai/payload.py
+-rw-r--r--   0 root         (0) staff       (20)    35030 2024-04-10 04:51:14.000000 galxiai-0.50.4/galxiai/ql.py
+-rw-r--r--   0 root         (0) staff       (20)    12062 2024-04-21 07:36:19.000000 galxiai-0.50.4/galxiai/req.py
+-rw-r--r--   0 root         (0) staff       (20)     3265 2024-04-21 07:32:34.000000 galxiai-0.50.4/galxiai/reqbase.py
+-rw-r--r--   0 root         (0) staff       (20)    30753 2024-04-21 09:20:35.000000 galxiai-0.50.4/galxiai/sqlite_galxi.py
+-rw-r--r--   0 root         (0) staff       (20)     1845 2024-04-21 07:36:19.000000 galxiai-0.50.4/galxiai/ut.py
+-rw-r--r--   0 root         (0) staff       (20)     5485 2024-04-21 07:34:26.000000 galxiai-0.50.4/galxiai/xxcl.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 09:21:08.710665 galxiai-0.50.4/galxiai.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      909 2024-04-21 09:21:08.000000 galxiai-0.50.4/galxiai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      367 2024-04-21 09:21:08.000000 galxiai-0.50.4/galxiai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-21 09:21:08.000000 galxiai-0.50.4/galxiai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       30 2024-04-21 09:21:08.000000 galxiai-0.50.4/galxiai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        8 2024-04-21 09:21:08.000000 galxiai-0.50.4/galxiai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-21 09:21:08.712124 galxiai-0.50.4/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2484 2024-04-21 07:48:41.000000 galxiai-0.50.4/setup.py
```

### Comparing `galxiai-0.50.3/LICENSE` & `galxiai-0.50.4/LICENSE`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.3/PKG-INFO` & `galxiai-0.50.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galxiai
-Version: 0.50.3
+Version: 0.50.4
 Summary: A Python package to manage all my cash in one hand
 Home-page: https://github.com/djsola/galxiai/
 Author: Jun-You MIT & Solomon
 Author-email: solomon@tmp.o66p.com
 License: MIT
 Keywords: ssh galxiai room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `galxiai-0.50.3/galxiai/__init__.py` & `galxiai-0.50.4/galxiai/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.50.3'
+__version__ = '0.50.4'
```

### Comparing `galxiai-0.50.3/galxiai/clasreq.py` & `galxiai-0.50.4/galxiai/clasreq.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.3/galxiai/const.py` & `galxiai-0.50.4/galxiai/const.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.3/galxiai/payload.py` & `galxiai-0.50.4/galxiai/payload.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.3/galxiai/ql.py` & `galxiai-0.50.4/galxiai/ql.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.3/galxiai/req.py` & `galxiai-0.50.4/galxiai/req.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.3/galxiai/reqbase.py` & `galxiai-0.50.4/galxiai/reqbase.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.3/galxiai/sqlite_galxi.py` & `galxiai-0.50.4/galxiai/sqlite_galxi.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,39 +397,45 @@
         return self._is_time_exists(Galxi.DB_MEMBER, self.user_addr, key)
 
     def set_invalidate_token(self):
         if self.has_the_address(self.user_addr) is False:
             raise Exception("user is not found from the db")
         self._check_point_update("bearer_token_exp", 0)
 
-    def use_insert_user_dat(self, evm_address: str, file: dict) -> bool:
+    def register_new_evm_address(self, evm_address: str, file: dict) -> bool:
         ...
 
-    def set_jwt_token(self, bearer: str):
-        # Decode the JWT token
-        decoded_token = jwt.decode(jwt=bearer, options={"verify_signature": False}, verify=False)
+    def gen_user_id(self):
+        return str(uuid.uuid1())
+
+    def try_to_check_jwt_token(self, token):
+        decoded_token = jwt.decode(jwt=token, options={"verify_signature": False}, verify=False)
         # Get the expiration timestamp from the decoded token
         expiration_timestamp = decoded_token.get('iat')
         if expiration_timestamp is None:
-            if self.has_the_address(self.user_addr) is False:
-                self.use_insert_user_dat(self.user_addr, {
-                    "bearer_token": bearer,
-                })
-            else:
-                self.update_res_kv("bearer_token", bearer)
-            self._check_point_update("bearer_token_exp", 3600)
+            return False, 0
         else:
             expiration_delta = expiration_timestamp - self.get_time_now()
-            if self.has_the_address(self.user_addr) is False:
-                self.use_insert_user_dat(self.user_addr, {
-                    "bearer_token": bearer,
-                })
-            else:
-                self.update_res_kv("bearer_token", bearer)
-            self._check_point_update("bearer_token_exp", expiration_delta)
+            return True, expiration_delta
+
+    def set_jwt_token(self, bearer: str):
+        has_address = self.has_the_address(self.user_addr)
+        jwtdecode = self.try_to_check_jwt_token(bearer)
+        result, delta = jwtdecode
+        if has_address:
+            self.update_res_kv("bearer_token", bearer)
+        else:
+            self.register_new_evm_address(self.user_addr, {
+                "bearer_token": bearer,
+            })
+        if result:
+            self._check_point_update("bearer_token_exp", delta)
+        else:
+            self._check_point_update("bearer_token_exp", 3600)
+
         self.update_col_time()
 
     def check_bearer_token_expired(self) -> bool:
         return self._is_what_ready("bearer_token_exp")
 
     def get_access_token(self):
         if self.has_the_address(self.user_addr) is False:
@@ -628,20 +634,17 @@
 
     def check_point_campaign(self, camp_id: str):
         return self._check_point_update(f"campaign_claimed_{camp_id}", 32400)
 
     def is_check_point_cp_ready(self, camp_id: str):
         return self._is_what_ready(f"campaign_claimed_{camp_id}", False)
 
-    def use_insert_user_dat(self, evm_address: str, file: dict) -> bool:
-        # user_id = file["user"]["id"]
-        # invite_by = "" if file["user"]["invited_by_id"] is None else file["user"]["invited_by_id"]
-        # invite_code = "" if file["user"]["invite_code"] is None else file["user"]["invite_code"]
+    def register_new_evm_address(self, evm_address: str, file: dict) -> bool:
         p = {
-            "member_id": str(uuid.uuid1()),
+            "member_id": self.gen_user_id(),
             "address_evm": self.user_addr,
             "parent_code": "",
             "referral_code": "",
             "next_action": "{}",
             "update_time": self.get_time_now(),
             "res": json.dumps(file)
         }
```

### Comparing `galxiai-0.50.3/galxiai/ut.py` & `galxiai-0.50.4/galxiai/ut.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.3/galxiai/xxcl.py` & `galxiai-0.50.4/galxiai/xxcl.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.3/galxiai.egg-info/PKG-INFO` & `galxiai-0.50.4/galxiai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galxiai
-Version: 0.50.3
+Version: 0.50.4
 Summary: A Python package to manage all my cash in one hand
 Home-page: https://github.com/djsola/galxiai/
 Author: Jun-You MIT & Solomon
 Author-email: solomon@tmp.o66p.com
 License: MIT
 Keywords: ssh galxiai room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `galxiai-0.50.3/setup.py` & `galxiai-0.50.4/setup.py`

 * *Files identical despite different names*


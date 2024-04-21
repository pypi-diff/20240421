# Comparing `tmp/galxiai-0.50.5.tar.gz` & `tmp/galxiai-0.50.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galxiai-0.50.5.tar", last modified: Sun Apr 21 09:38:24 2024, max compression
+gzip compressed data, was "galxiai-0.50.6.tar", last modified: Sun Apr 21 12:50:37 2024, max compression
```

## Comparing `galxiai-0.50.5.tar` & `galxiai-0.50.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 09:38:24.940632 galxiai-0.50.5/
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 galxiai-0.50.5/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      909 2024-04-21 09:38:24.940467 galxiai-0.50.5/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)       64 2024-04-21 07:45:09.000000 galxiai-0.50.5/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 09:38:24.936759 galxiai-0.50.5/galxiai/
--rw-r--r--   0 root         (0) staff       (20)     1321 2024-04-21 09:38:24.000000 galxiai-0.50.5/galxiai/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8647 2024-04-21 07:24:58.000000 galxiai-0.50.5/galxiai/clasreq.py
--rw-r--r--   0 root         (0) staff       (20)     2553 2024-04-21 07:49:17.000000 galxiai-0.50.5/galxiai/const.py
--rw-r--r--   0 root         (0) staff       (20)    14533 2024-04-21 09:38:07.000000 galxiai-0.50.5/galxiai/payload.py
--rw-r--r--   0 root         (0) staff       (20)    35030 2024-04-10 04:51:14.000000 galxiai-0.50.5/galxiai/ql.py
--rw-r--r--   0 root         (0) staff       (20)    12062 2024-04-21 07:36:19.000000 galxiai-0.50.5/galxiai/req.py
--rw-r--r--   0 root         (0) staff       (20)     3265 2024-04-21 07:32:34.000000 galxiai-0.50.5/galxiai/reqbase.py
--rw-r--r--   0 root         (0) staff       (20)    30753 2024-04-21 09:20:35.000000 galxiai-0.50.5/galxiai/sqlite_galxi.py
--rw-r--r--   0 root         (0) staff       (20)     1845 2024-04-21 07:36:19.000000 galxiai-0.50.5/galxiai/ut.py
--rw-r--r--   0 root         (0) staff       (20)     5485 2024-04-21 07:34:26.000000 galxiai-0.50.5/galxiai/xxcl.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 09:38:24.939920 galxiai-0.50.5/galxiai.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      909 2024-04-21 09:38:24.000000 galxiai-0.50.5/galxiai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      367 2024-04-21 09:38:24.000000 galxiai-0.50.5/galxiai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-21 09:38:24.000000 galxiai-0.50.5/galxiai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       30 2024-04-21 09:38:24.000000 galxiai-0.50.5/galxiai.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        8 2024-04-21 09:38:24.000000 galxiai-0.50.5/galxiai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-04-21 09:38:24.941195 galxiai-0.50.5/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2484 2024-04-21 07:48:41.000000 galxiai-0.50.5/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 12:50:37.655261 galxiai-0.50.6/
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 galxiai-0.50.6/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      909 2024-04-21 12:50:37.655078 galxiai-0.50.6/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)       64 2024-04-21 07:45:09.000000 galxiai-0.50.6/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 12:50:37.651241 galxiai-0.50.6/galxiai/
+-rw-r--r--   0 root         (0) staff       (20)     1321 2024-04-21 12:50:37.000000 galxiai-0.50.6/galxiai/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8647 2024-04-21 07:24:58.000000 galxiai-0.50.6/galxiai/clasreq.py
+-rw-r--r--   0 root         (0) staff       (20)     2553 2024-04-21 07:49:17.000000 galxiai-0.50.6/galxiai/const.py
+-rw-r--r--   0 root         (0) staff       (20)    15573 2024-04-21 12:50:09.000000 galxiai-0.50.6/galxiai/payload.py
+-rw-r--r--   0 root         (0) staff       (20)    35439 2024-04-21 10:28:30.000000 galxiai-0.50.6/galxiai/ql.py
+-rw-r--r--   0 root         (0) staff       (20)    12894 2024-04-21 11:24:00.000000 galxiai-0.50.6/galxiai/req.py
+-rw-r--r--   0 root         (0) staff       (20)     3265 2024-04-21 07:32:34.000000 galxiai-0.50.6/galxiai/reqbase.py
+-rw-r--r--   0 root         (0) staff       (20)    30753 2024-04-21 09:20:35.000000 galxiai-0.50.6/galxiai/sqlite_galxi.py
+-rw-r--r--   0 root         (0) staff       (20)     2519 2024-04-21 11:46:34.000000 galxiai-0.50.6/galxiai/ut.py
+-rw-r--r--   0 root         (0) staff       (20)     5485 2024-04-21 07:34:26.000000 galxiai-0.50.6/galxiai/xxcl.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-21 12:50:37.654483 galxiai-0.50.6/galxiai.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      909 2024-04-21 12:50:37.000000 galxiai-0.50.6/galxiai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      367 2024-04-21 12:50:37.000000 galxiai-0.50.6/galxiai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-21 12:50:37.000000 galxiai-0.50.6/galxiai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       30 2024-04-21 12:50:37.000000 galxiai-0.50.6/galxiai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        8 2024-04-21 12:50:37.000000 galxiai-0.50.6/galxiai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-21 12:50:37.655846 galxiai-0.50.6/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2484 2024-04-21 07:48:41.000000 galxiai-0.50.6/setup.py
```

### Comparing `galxiai-0.50.5/LICENSE` & `galxiai-0.50.6/LICENSE`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.5/PKG-INFO` & `galxiai-0.50.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galxiai
-Version: 0.50.5
+Version: 0.50.6
 Summary: A Python package to manage all my cash in one hand
 Home-page: https://github.com/djsola/galxiai/
 Author: Jun-You MIT & Solomon
 Author-email: solomon@tmp.o66p.com
 License: MIT
 Keywords: ssh galxiai room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `galxiai-0.50.5/galxiai/__init__.py` & `galxiai-0.50.6/galxiai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.50.5'
+__version__ = '0.50.6'
```

### Comparing `galxiai-0.50.5/galxiai/clasreq.py` & `galxiai-0.50.6/galxiai/clasreq.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.5/galxiai/const.py` & `galxiai-0.50.6/galxiai/const.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.5/galxiai/payload.py` & `galxiai-0.50.6/galxiai/payload.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # !/usr/bin/env python
 # coding: utf-8
 import time
 
+from galxiai import ut
 from galxiai.req import *
 from galxiai.sqlite_galxi import GalaBox
 from galxiai.const import *
 import random
 import json
 
 
@@ -48,25 +49,16 @@
     def process_loop(self, loop_at: int):
         ...
 
 
 class GalxiRunner(UrlReq, Structure, GalStep):
 
     def get_recap_response(self):
-        try:
-            _captcha_data = self._geetest_mode_ai.get_solution_type_ai()
-        except FailedToProduceCaptchaOutput:
-            time.sleep(10)
-            return self.get_recap_response()
-        except json.decoder.JSONDecodeError:
-            t = self.db.get_time_now()
-            print(f"{t} failed to make verification on captcha")
-            time.sleep(600)
-            return self.get_recap_response()
-        return _captcha_data
+        # need to use your own custom AI captura
+        return {}
 
     def internal_port_vpn(self, k: int):
         # self.capcha_provider.enableProxy(k)
         self.init_ai_module(k)
 
     def init_ai_module(self, port: int):
         ...
@@ -236,14 +228,35 @@
     def action_get_api_token(self):
         if self.db.has_res_key("api_key") is True:
             return
         _doc = galxeQL(self.session, rq_data_update_access_token(self.wallet_erc.address))
         if "updateAccessToken" in _doc:
             self.db.update_res_kv("api_key", _doc["updateAccessToken"]["accessToken"])
 
+    def action_twitter_action_post_twitter(self, text: str):
+
+        return ""
+
+    def twitter_verification_message(self):
+        user_id = self.db.get_key_res("id")
+        return f"Verifying my Twitter account for my #GalxeID gid:{user_id} @Galxe"
+
+    def action_twitter_ac_bind(self):
+        if self.db.res_true("hasTwitter") is False:
+            print("============= confirm twitter ac")
+        url = self.action_twitter_action_post_twitter(self.twitter_verification_message())
+        _doc = galxeQL(self.session, rq_data_fill_twitter_ac(self.wallet_erc.address, url))
+        if "twitterUserID" in _doc and "twitterUserName" in _doc:
+            print(".ok 1")
+        _doc = galxeQL(self.session, rq_data_twitter_verify(self.wallet_erc.address, url))
+        if "twitterUserID" in _doc and "twitterUserName" in _doc:
+            print(".ok 2")
+
+        self.action_get_profile()
+
     def action_email_confirm(self):
         print("============= confirm email")
         _doc = None
 
         if self.db.is_email_sent() is False:
             print("no email has been sent")
             return
@@ -351,23 +364,32 @@
 
     def log_failed_verifications(self):
         self.db.log_failed_verifications()
 
     def profile_res_check(self, _d):
         try:
             _info = _d["addressInfo"]
-            self.db.update_res_set({
+            data = {
                 "id": _info["id"],
-                "username": _info["username"],
-                "address": _info["address"],
-                "hasEmail": bool(_info["hasEmail"]),
-                "solanaAddress": _info["solanaAddress"],
-                "seiAddress": _info["seiAddress"],
-                "bitcoinAddress": _info["bitcoinAddress"],
-            })
+            }
+
+            ut.check_kv_or_update(data, _info, "id")
+            ut.check_kv_or_update(data, _info, "username")
+            ut.check_kv_or_update(data, _info, "address")
+            ut.check_kv_or_update(data, _info, "hasEmail")
+            ut.check_kv_or_update(data, _info, "solanaAddress")
+            ut.check_kv_or_update(data, _info, "seiAddress")
+            ut.check_kv_or_update(data, _info, "bitcoinAddress")
+            ut.check_kv_or_update(data, _info, "twitterUserID")
+            ut.check_kv_or_update(data, _info, "twitterUserName")
+            ut.check_kv_or_update(data, _info, "email")
+            ut.check_kv_or_update(data, _info, "displayNamePref")
+            ut.check_kv_or_update(data, _info, "hasWorldcoin")
+            ut.check_kv_or_update(data, _info, "hasWorldcoin")
+            self.db.update_res_set(data)
             print("profile updated.")
         except ValueError:
             print(_d)
 
     def action_get_profile(self):
         d = galxeQL(self.session, rq_data_get_profile(self.wallet_erc.address))
         self.profile_res_check(d)
```

### Comparing `galxiai-0.50.5/galxiai/ql.py` & `galxiai-0.50.6/galxiai/ql.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,32 @@
   isVerified
   status
   followersCount
   activeCampaignCount
   __typename
 }
 """
+CHECK_TWITTER_AC = """mutation checkTwitterAccount($input: VerifyTwitterAccountInput!) {
+  checkTwitterAccount(input: $input) {
+    address
+    twitterUserID
+    twitterUserName
+    __typename
+  }
+}
+"""
+VERIFY_TWITTER_AC = """mutation VerifyTwitterAccount($input: VerifyTwitterAccountInput!) {
+  verifyTwitterAccount(input: $input) {
+    address
+    twitterUserID
+    twitterUserName
+    __typename
+  }
+}
+"""
 PASSPORTINFO = """query PassportInfo($address: String!) {
   addressInfo(address: $address) {
     id
     passport {
       status
       pendingRedactAt
       id
```

### Comparing `galxiai-0.50.5/galxiai/req.py` & `galxiai-0.50.6/galxiai/req.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,50 @@
 try:
     import tls_client
 except:
     os.system('python -m pip install tls-client')
     import tls_client
 
 
+def rq_data_fill_twitter_ac(address: str, twitter_url: str):
+    return {
+        "operationName": "checkTwitterAccount",
+        "query": CHECK_TWITTER_AC,
+        "variables": {
+            "input": {
+                "address": address,
+                "twitterURL": twitter_url
+            }
+        }
+    }
+
+
+def rq_data_twitter_verify(address: str, twitter_url: str):
+    return {
+        "operationName": "VerifyTwitterAccount",
+        "query": VERIFY_TWITTER_AC,
+        "variables": {
+            "input": {
+                "address": address,
+                "twitterURL": twitter_url
+            }
+        }
+    }
+
+
+def rq_data_check_jwt_cap(_captcha: dict):
+    return {
+        "operationName": "CheckJWT",
+        "query": CHECK_JWT_QL,
+        "variables": {
+            "captchaInput": _captcha,
+        },
+    }
+
+
 def rq_data_address_info(first: int = 30):
     return {
         "query": SPACESINADDRESSINFO,
         "variables": {
             "address": "",
             "listSpaceInput": {"first": first},
             "operationName": "SpacesInAddressInfo",
@@ -39,15 +75,15 @@
 
 def rq_data_check_jwt(_captcha: dict):
     return {
         "query": CHECK_JWT_QL,
         "variables": {
             "captchaInput": _captcha,
             "operationName": "CheckJWT",
-        }
+        },
     }
 
 
 def rq_data_campaign_detail(address: str, campaign_id: str, with_address: bool):
     return {
         "query": CAMPAIGNDETAILALL,
         "operationName": "CampaignDetailAll",
```

### Comparing `galxiai-0.50.5/galxiai/reqbase.py` & `galxiai-0.50.6/galxiai/reqbase.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.5/galxiai/sqlite_galxi.py` & `galxiai-0.50.6/galxiai/sqlite_galxi.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.5/galxiai/xxcl.py` & `galxiai-0.50.6/galxiai/xxcl.py`

 * *Files identical despite different names*

### Comparing `galxiai-0.50.5/galxiai.egg-info/PKG-INFO` & `galxiai-0.50.6/galxiai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galxiai
-Version: 0.50.5
+Version: 0.50.6
 Summary: A Python package to manage all my cash in one hand
 Home-page: https://github.com/djsola/galxiai/
 Author: Jun-You MIT & Solomon
 Author-email: solomon@tmp.o66p.com
 License: MIT
 Keywords: ssh galxiai room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `galxiai-0.50.5/setup.py` & `galxiai-0.50.6/setup.py`

 * *Files identical despite different names*


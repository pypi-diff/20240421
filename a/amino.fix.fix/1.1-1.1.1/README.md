# Comparing `tmp/amino_fix_fix-1.1.tar.gz` & `tmp/amino_fix_fix-1.1.1.tar.gz`

## Comparing `amino_fix_fix-1.1.tar` & `amino_fix_fix-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/__init__.py
--rw-r--r--   0        0        0    24271 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/acm.py
--rw-r--r--   0        0        0   105414 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/client.py
--rw-r--r--   0        0        0    14295 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/socket.py
--rw-r--r--   0        0        0   146160 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/sub_client.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/asyncfixfix/README.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/asyncfixfix/__init__.py
--rw-r--r--   0        0        0    16275 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/asyncfixfix/acm.py
--rw-r--r--   0        0        0    98563 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/asyncfixfix/client.py
--rw-r--r--   0        0        0    14297 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/asyncfixfix/socket.py
--rw-r--r--   0        0        0   109970 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/asyncfixfix/sub_client.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/__init__.py
--rw-r--r--   0        0        0    33502 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/exceptions.py
--rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/headers.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/helpers.py
--rw-r--r--   0        0        0   200156 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/objects.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/facades/__init__.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/facades/aiohttp.py
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/facades/requests.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/facades/unsuccessful_import.py
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/LICENSE
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/README.md
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/pyproject.toml
--rw-r--r--   0        0        0     5302 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/PKG-INFO
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/__init__.py
+-rw-r--r--   0        0        0    23787 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/acm.py
+-rw-r--r--   0        0        0   105414 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/client.py
+-rw-r--r--   0        0        0    14295 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/socket.py
+-rw-r--r--   0        0        0   146233 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/sub_client.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/asyncfixfix/README.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/asyncfixfix/__init__.py
+-rw-r--r--   0        0        0    15813 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/asyncfixfix/acm.py
+-rw-r--r--   0        0        0    98563 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/asyncfixfix/client.py
+-rw-r--r--   0        0        0    14297 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/asyncfixfix/socket.py
+-rw-r--r--   0        0        0   109932 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/asyncfixfix/sub_client.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/lib/__init__.py
+-rw-r--r--   0        0        0    33502 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/lib/exceptions.py
+-rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/lib/headers.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/lib/helpers.py
+-rw-r--r--   0        0        0   200156 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/lib/objects.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/lib/facades/__init__.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/lib/facades/aiohttp.py
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/lib/facades/requests.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/aminofixfix/lib/facades/unsuccessful_import.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/README.md
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 amino_fix_fix-1.1.1/PKG-INFO
```

### Comparing `amino_fix_fix-1.1/aminofixfix/__init__.py` & `amino_fix_fix-1.1.1/aminofixfix/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1"
+__version__ = "1.1.1"
 
 from .acm import ACM
 from .client import Client
 from .sub_client import SubClient
 from .socket import Callbacks, SocketHandler
 from .lib import exceptions, helpers, objects, headers
```

### Comparing `amino_fix_fix-1.1/aminofixfix/acm.py` & `amino_fix_fix-1.1.1/aminofixfix/acm.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             "primaryLanguage": primaryLanguage,
             "tagline": tagline,
             "templateId": 9,
             "themeColor": themeColor,
             "timestamp": inttime()
         })
 
-        response = self.session.post(f"/g/s/community", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/g/s/community", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     def delete_community(self, email: str, password: str, verificationCode: str):
         """
         Deleting community.
 
@@ -117,15 +117,15 @@
                 "type": 1,
                 "identity": email
             },
             "deviceID": self.device_id
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/g/s-x{self.comId}/community/delete-request", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/g/s-x{self.comId}/community/delete-request", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     def list_communities(self, start: int = 0, size: int = 25):
         """
         Getting all communities where you are leader.
 
@@ -135,15 +135,15 @@
         - size: int = 25
             - how much you want to get
 
         Recieving:
         - object `dict`
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
-        response = self.session.get(f"/g/s/community/managed?start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
+        response = self.session.get(f"/g/s/community/managed?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.CommunityList(response.json()["communityList"]).CommunityList
 
     def get_categories(self, start: int = 0, size: int = 25):
         """
         Getting categories of communities.
 
@@ -154,15 +154,15 @@
             - how much you want to get
 
         Recieving:
         - object `dict`
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.get(f"/x{self.comId}/s/blog-category?start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
+        response = self.session.get(f"/x{self.comId}/s/blog-category?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.json()
 
     def change_sidepanel_color(self, color: str):
         """
         Change sidepanel color.
 
@@ -177,28 +177,28 @@
         data = dumps({
             "path": "appearance.leftSidePanel.style.iconColor",
             "value": color if len(color) == 7 else "#000000",
             "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return response.status_code
         else: return response.json()
 
     def get_themepack_info(self):
         """
         This method can be used for getting info about current themepack of community.
 
         Recieving:
         - object
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.get(f"/g/s-x{self.comId}/community/info?withTopicList=1&withInfluencerList=1&influencerListOrderStrategy=fansCount", headers=self.additional_headers(), proxies=self.proxies)
+        response = self.session.get(f"/g/s-x{self.comId}/community/info?withTopicList=1&withInfluencerList=1&influencerListOrderStrategy=fansCount", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.json()['community']['themePack']
     
     def upload_themepack_raw(self, file: BinaryIO):
         """
         Uploading new themepack.
 
@@ -270,15 +270,15 @@
         - file: BinaryIO
 
         Recieving:
         - object
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/media/upload/target/community-theme-pack", data=file.read(), headers=headers.Headers(data=file.read()).s_headers, proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/media/upload/target/community-theme-pack", data=file.read(), headers=headers.Headers(data=file.read()).s_headers)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.json()
 
     def promote(self, userId: str, rank: str):
         """
         Promote user to curator, leader or agent.
 
@@ -293,15 +293,15 @@
         """
         rank = rank.lower().replace("agent", "transfer-agent")
 
         if rank.lower() not in ["transfer-agent", "leader", "curator"]:
             raise exceptions.WrongType(rank)
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/{rank}", headers=self.additional_headers(), proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/{rank}", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     def get_join_requests(self, start: int = 0, size: int = 25):
         """
         Get all requests to join your precious community.
 
@@ -313,15 +313,15 @@
 
         Recieving:
         - object `JoinRequest`
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
 
-        response = self.session.get(f"/x{self.comId}/s/community/membership-request?status=pending&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
+        response = self.session.get(f"/x{self.comId}/s/community/membership-request?status=pending&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.JoinRequest(response.json()).JoinRequest
 
     def accept_join_request(self, userId: str):
         """
         Accept user to join your precious community.
 
@@ -337,15 +337,15 @@
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({})
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/community/membership-request/{userId}/accept", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/community/membership-request/{userId}/accept", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     def reject_join_request(self, userId: str):
         """
         Reject user to join your precious community.
 
@@ -363,29 +363,29 @@
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({})
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/community/membership-request/{userId}/reject", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/community/membership-request/{userId}/reject", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     def get_community_stats(self):
         """
         Get community statistics.
 
         Recieving:
         - object `CommunityStats`
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
 
-        response = self.session.get(f"/x{self.comId}/s/community/stats", headers=self.additional_headers(), proxies=self.proxies)
+        response = self.session.get(f"/x{self.comId}/s/community/stats", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.CommunityStats(response.json()["communityStats"]).CommunityStats
 
     def get_community_user_stats(self, type: str, start: int = 0, size: int = 25):
         """
         Get community user statistics.
 
@@ -403,15 +403,15 @@
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
 
         if type.lower() == "leader": target = "leader"
         elif type.lower() == "curator": target = "curator"
         else: raise exceptions.WrongType(type)
 
-        response = self.session.get(f"/x{self.comId}/s/community/stats/moderation?type={target}&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
+        response = self.session.get(f"/x{self.comId}/s/community/stats/moderation?type={target}&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     def change_welcome_message(self, message: str, isEnabled: bool = True):
         """
         Change welcome message of community.
 
@@ -429,15 +429,15 @@
                 "enabled": isEnabled,
                 "text": message
             },
             "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     def change_amino_id(self, aminoId: str):
         """
         Change AminoID of community.
 
@@ -450,15 +450,15 @@
         """
         data = dumps({
             "endpoint": aminoId,
             "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/community/settings", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/community/settings", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     def change_guidelines(self, message: str):
         """
         Change rules of community.
 
@@ -471,15 +471,15 @@
         """
         data = dumps({
             "content": message,
             "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/community/guideline", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/community/guideline", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     def edit_community(self, name: str = None, description: str = None, aminoId: str = None, primaryLanguage: str = None, themePackUrl: str = None):
         """
         Edit community.
 
@@ -502,15 +502,15 @@
         if aminoId is not None: data["endpoint"] = aminoId
         if primaryLanguage is not None: data["primaryLanguage"] = primaryLanguage
         if themePackUrl is not None: data["themePackUrl"] = themePackUrl
 
         data = dumps(data)
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/community/settings", data=data, headers=self.additional_headers(data=data), proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/community/settings", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     def change_module(self, module: str, isEnabled: bool):
         """
         Enable or disable module.
 
@@ -547,15 +547,15 @@
         data = dumps({
             "path": mod,
             "value": isEnabled,
             "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     def add_influencer(self, userId: str, monthlyFee: int):
         """
         Create fanclub.
 
@@ -570,15 +570,15 @@
         """
         data = dumps({
             "monthlyFee": monthlyFee,
             "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/influencer/{userId}", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/influencer/{userId}", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     def remove_influencer(self, userId: str):
         """
         Delete fanclub.
 
@@ -586,15 +586,15 @@
         - userId: str
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.delete(f"/x{self.comId}/s/influencer/{userId}", headers=self.additional_headers(), proxies=self.proxies)
+        response = self.session.delete(f"/x{self.comId}/s/influencer/{userId}", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     def get_notice_list(self, start: int = 0, size: int = 25):
         """
         Get notices list.
 
@@ -605,15 +605,15 @@
             - how much you want to get
 
         Recieving:
         - object `NoticeList`
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.get(f"/x{self.comId}/s/notice?type=management&status=1&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
+        response = self.session.get(f"/x{self.comId}/s/notice?type=management&status=1&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.NoticeList(response.json()["noticeList"]).NoticeList
 
     def delete_pending_role(self, noticeId: str):
         """
         Delete pending role.
 
@@ -621,10 +621,10 @@
         - noticeId: str
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.delete(f"/x{self.comId}/s/notice/{noticeId}", headers=self.additional_headers(), proxies=self.proxies)
+        response = self.session.delete(f"/x{self.comId}/s/notice/{noticeId}", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
```

### Comparing `amino_fix_fix-1.1/aminofixfix/client.py` & `amino_fix_fix-1.1.1/aminofixfix/client.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.1/aminofixfix/socket.py` & `amino_fix_fix-1.1.1/aminofixfix/socket.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.1/aminofixfix/sub_client.py` & `amino_fix_fix-1.1.1/aminofixfix/sub_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3156,29 +3156,31 @@
         - userId: str
         - time: int
             - time == 1 is 1 hour
             - time == 2 is 4 hours
             - time == 3 is 8 hours
             - time == 4 is 12 hours
             - time == 5 is 24 hours
-            - time == 6 is 72 hours (visually, its 24 hours)
+            - time == 6 is .. hours
+            - time == 7 is .. hours
         - title: str = None
         - reason: str = None
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
 
         if time == 1: time = 3600
         elif time == 2: time = 10800
         elif time == 3: time = 21600
         elif time == 4: time = 43200
         elif time == 5: time = 86400
-        elif time == 6: time = 259200
+        # i will not implement for now strikes higher than 24 hours
+        # fuck you aminoservice
         else: raise exceptions.WrongType(time)
 
         data = dumps({
             "uid": userId,
             "title": title or "You got striked by Knife of Justice!",
             "content": reason or "You got striked by Knife of Justice by this admin! Sadly, there is no reason. Admin thought that amino.fix.fix will forgive this, hehe. :з",
             "attachedObject": {
```

### Comparing `amino_fix_fix-1.1/aminofixfix/asyncfixfix/acm.py` & `amino_fix_fix-1.1.1/aminofixfix/asyncfixfix/acm.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             "primaryLanguage": primaryLanguage,
             "tagline": tagline,
             "templateId": 9,
             "themeColor": themeColor,
             "timestamp": inttime()
         })
 
-        response = await self.session.post(f"/g/s/community", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/g/s/community", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def delete_community(self, email: str, password: str, verificationCode: str):
         data = dumps({
             "secret": f"0 {password}",
             "validationContext": {
@@ -50,47 +50,47 @@
                 "type": 1,
                 "identity": email
             },
             "deviceID": self.device_id
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/g/s-x{self.comId}/community/delete-request", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/g/s-x{self.comId}/community/delete-request", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def list_communities(self, start: int = 0, size: int = 25):
-        response = await self.session.get(f"/g/s/community/managed?start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
+        response = await self.session.get(f"/g/s/community/managed?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.CommunityList(response.json()["communityList"]).CommunityList
 
     async def get_categories(self, start: int = 0, size: int = 25):
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.get(f"/x{self.comId}/s/blog-category?start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
+        response = await self.session.get(f"/x{self.comId}/s/blog-category?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.json()
 
     async def change_sidepanel_color(self, color: str):
         data = dumps({
             "path": "appearance.leftSidePanel.style.iconColor",
             "value": color,
             "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return response.status_code
         else: return response.json()
 
     async def get_themepack_info(self, file: BinaryIO):
         """
         This method can be used for getting info about current themepack of community.
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.get(f"/g/s-x{self.comId}/community/info?withTopicList=1&withInfluencerList=1&influencerListOrderStrategy=fansCount", data=file.read(), headers=headers.Headers(data=file.read()).s_headers, proxies=self.proxies)
+        response = await self.session.get(f"/g/s-x{self.comId}/community/info?withTopicList=1&withInfluencerList=1&influencerListOrderStrategy=fansCount", data=file.read(), headers=headers.Headers(data=file.read()).s_headers)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return await response.json()['community']['themePack']
 
     async def upload_themepack_raw(self, file: BinaryIO):
         """
         Uploading new themepack.
 
@@ -155,93 +155,93 @@
             - "titlebar-image":
                 - w = 320
                 - h = 64
         - you *can* specify "x" and "y" if you want
         - theoretically you can provide different "w" and "h"
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/media/upload/target/community-theme-pack", data=file.read(), headers=headers.Headers(data=file.read()).s_headers, proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/media/upload/target/community-theme-pack", data=file.read(), headers=headers.Headers(data=file.read()).s_headers)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.json()
 
     async def promote(self, userId: str, rank: str):
         rank = rank.lower().replace("agent", "transfer-agent")
 
         if rank.lower() not in ["transfer-agent", "leader", "curator"]:
             raise exceptions.WrongType(rank)
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/user-profile/{userId}/{rank}", headers=self.additional_headers(), proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/user-profile/{userId}/{rank}", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def get_join_requests(self, start: int = 0, size: int = 25):
         if self.comId is None: raise exceptions.CommunityNeeded()
 
-        response = await self.session.get(f"/x{self.comId}/s/community/membership-request?status=pending&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
+        response = await self.session.get(f"/x{self.comId}/s/community/membership-request?status=pending&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.JoinRequest(response.json()).JoinRequest
 
     async def accept_join_request(self, userId: str):
         data = dumps({})
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/community/membership-request/{userId}/accept", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/community/membership-request/{userId}/accept", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def reject_join_request(self, userId: str):
         data = dumps({})
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/community/membership-request/{userId}/reject", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/community/membership-request/{userId}/reject", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def get_community_stats(self):
         if self.comId is None: raise exceptions.CommunityNeeded()
 
-        response = await self.session.get(f"/x{self.comId}/s/community/stats", headers=self.additional_headers(), proxies=self.proxies)
+        response = await self.session.get(f"/x{self.comId}/s/community/stats", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.CommunityStats(response.json()["communityStats"]).CommunityStats
 
     async def get_community_user_stats(self, type: str, start: int = 0, size: int = 25):
         if self.comId is None: raise exceptions.CommunityNeeded()
 
         if type.lower() == "leader": target = "leader"
         elif type.lower() == "curator": target = "curator"
         else: raise exceptions.WrongType(type)
 
-        response = await self.session.get(f"/x{self.comId}/s/community/stats/moderation?type={target}&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
+        response = await self.session.get(f"/x{self.comId}/s/community/stats/moderation?type={target}&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     async def change_welcome_message(self, message: str, isEnabled: bool = True):
         data = dumps({
             "path": "general.welcomeMessage",
             "value": {
                 "enabled": isEnabled,
                 "text": message
             },
             "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def change_guidelines(self, message: str):
         data = dumps({
             "content": message,
             "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/community/guideline", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/community/guideline", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def edit_community(self, name: str = None, description: str = None, aminoId: str = None, primaryLanguage: str = None, themePackUrl: str = None):
         data = {"timestamp": inttime()}
 
         if name is not None: data["name"] = name
@@ -249,15 +249,15 @@
         if aminoId is not None: data["endpoint"] = aminoId
         if primaryLanguage is not None: data["primaryLanguage"] = primaryLanguage
         if themePackUrl is not None: data["themePackUrl"] = themePackUrl
 
         data = dumps(data)
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/community/settings", data=data, headers=self.additional_headers(data=data), proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/community/settings", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def change_module(self, module: str, isEnabled: bool):
         if module.lower() == "chat": mod = "module.chat.enabled"
         elif module.lower() == "livechat": mod = "module.chat.avChat.videoEnabled"
         elif module.lower() == "screeningroom": mod = "module.chat.avChat.screeningRoomEnabled"
@@ -279,39 +279,39 @@
         data = dumps({
             "path": mod,
             "value": isEnabled,
             "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def add_influencer(self, userId: str, monthlyFee: int):
         data = dumps({
             "monthlyFee": monthlyFee,
             "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/influencer/{userId}", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/influencer/{userId}", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def remove_influencer(self, userId: str):
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.delete(f"/x{self.comId}/s/influencer/{userId}", headers=self.additional_headers(), proxies=self.proxies)
+        response = await self.session.delete(f"/x{self.comId}/s/influencer/{userId}", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def get_notice_list(self, start: int = 0, size: int = 25):
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.get(f"/x{self.comId}/s/notice?type=management&status=1&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
+        response = await self.session.get(f"/x{self.comId}/s/notice?type=management&status=1&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.NoticeList(response.json()["noticeList"]).NoticeList
 
     async def delete_pending_role(self, noticeId: str):
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.delete(f"/x{self.comId}/s/notice/{noticeId}", headers=self.additional_headers(), proxies=self.proxies)
+        response = await self.session.delete(f"/x{self.comId}/s/notice/{noticeId}", headers=self.additional_headers())
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
```

### Comparing `amino_fix_fix-1.1/aminofixfix/asyncfixfix/client.py` & `amino_fix_fix-1.1.1/aminofixfix/asyncfixfix/client.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.1/aminofixfix/asyncfixfix/socket.py` & `amino_fix_fix-1.1.1/aminofixfix/asyncfixfix/socket.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.1/aminofixfix/asyncfixfix/sub_client.py` & `amino_fix_fix-1.1.1/aminofixfix/asyncfixfix/sub_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2009,15 +2009,14 @@
     # TODO : List all strike texts
     async def strike(self, userId: str, time: int, title: str = None, reason: str = None):
         if time == 1: time = 86400
         elif time == 2: time = 10800
         elif time == 3: time = 21600
         elif time == 4: time = 43200
         elif time == 5: time = 86400
-        elif time == 6: time = 259200
         else: raise exceptions.WrongType(time)
 
         data = dumps({
             "uid": userId,
             "title": title,
             "content": reason,
             "attachedObject": {
```

### Comparing `amino_fix_fix-1.1/aminofixfix/lib/exceptions.py` & `amino_fix_fix-1.1.1/aminofixfix/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.1/aminofixfix/lib/headers.py` & `amino_fix_fix-1.1.1/aminofixfix/lib/headers.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.1/aminofixfix/lib/helpers.py` & `amino_fix_fix-1.1.1/aminofixfix/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.1/aminofixfix/lib/objects.py` & `amino_fix_fix-1.1.1/aminofixfix/lib/objects.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.1/aminofixfix/lib/facades/aiohttp.py` & `amino_fix_fix-1.1.1/aminofixfix/lib/facades/aiohttp.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.1/aminofixfix/lib/facades/requests.py` & `amino_fix_fix-1.1.1/aminofixfix/lib/facades/requests.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.1/aminofixfix/lib/facades/unsuccessful_import.py` & `amino_fix_fix-1.1.1/aminofixfix/lib/facades/unsuccessful_import.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.1/.gitignore` & `amino_fix_fix-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.1/LICENSE` & `amino_fix_fix-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.1/README.md` & `amino_fix_fix-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![PyPi Version](https://img.shields.io/pypi/v/amino.fix.fix.svg)](https://pypi.python.org/pypi/amino.fix.fix/)
 [![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b4-blue)](https://pypi.org/project/amino.fix.fix/#history)
 ![Python Version](https://img.shields.io/badge/python-%3E%3D3.8-orange)
 [![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
 
-Fork of Amino.fix to improve this library. Also unofficial client to work with Aminoapps.
+Unofficial client to work with Aminoapps, based on Amino.fix and HTTPX. Improved without losing compatibility.
 
 ## Important notices
 
 - in subclient you should pass `client`, **not** `profile`
 - if you have issues with HTTPX [let me know here](https://github.com/imperialwool/Amino.fix.fix/issues/3)
 - `lib/util` -> `lib/`
 - if you have issues in pydroid, reinstall/update it
```

### Comparing `amino_fix_fix-1.1/pyproject.toml` & `amino_fix_fix-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.1/PKG-INFO` & `amino_fix_fix-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: amino.fix.fix
-Version: 1.1
+Version: 1.1.1
 Summary: Unofficial library to work with Aminoapps
 Project-URL: Download, https://github.com/imperialwool/Amino.fix.fix.git
 Project-URL: Homepage, https://github.com/imperialwool/Amino.fix.fix
 Project-URL: Issues, https://github.com/imperialwool/Amino.fix.fix/issues
 Author-email: imperialwool <hi@iwool.dev>
 License-Expression: MIT
 License-File: LICENSE
@@ -43,15 +43,15 @@
 
 [![PyPi Version](https://img.shields.io/pypi/v/amino.fix.fix.svg)](https://pypi.python.org/pypi/amino.fix.fix/)
 [![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b4-blue)](https://pypi.org/project/amino.fix.fix/#history)
 ![Python Version](https://img.shields.io/badge/python-%3E%3D3.8-orange)
 [![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
 
-Fork of Amino.fix to improve this library. Also unofficial client to work with Aminoapps.
+Unofficial client to work with Aminoapps, based on Amino.fix and HTTPX. Improved without losing compatibility.
 
 ## Important notices
 
 - in subclient you should pass `client`, **not** `profile`
 - if you have issues with HTTPX [let me know here](https://github.com/imperialwool/Amino.fix.fix/issues/3)
 - `lib/util` -> `lib/`
 - if you have issues in pydroid, reinstall/update it
```


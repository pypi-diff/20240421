# Comparing `tmp/itchio-1.1.2.tar.gz` & `tmp/itchio-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itchio-1.1.2.tar", last modified: Thu Jul 14 07:46:30 2022, max compression
+gzip compressed data, was "itchio-1.1.3.tar", last modified: Sun Apr 21 14:54:18 2024, max compression
```

## Comparing `itchio-1.1.2.tar` & `itchio-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-07-14 07:46:30.224486 itchio-1.1.2/
--rw-rw-rw-   0        0        0     1091 2021-07-22 08:24:28.000000 itchio-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     1735 2022-07-14 07:46:30.223483 itchio-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1401 2022-07-14 07:26:04.000000 itchio-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2022-07-14 07:46:30.205484 itchio-1.1.2/itchio/
--rw-rw-rw-   0        0        0      772 2022-07-14 07:43:00.000000 itchio-1.1.2/itchio/DownloadKey.py
--rw-rw-rw-   0        0        0      488 2022-07-14 07:43:05.000000 itchio-1.1.2/itchio/Earnings.py
--rw-rw-rw-   0        0        0     5706 2022-07-14 07:43:04.000000 itchio-1.1.2/itchio/Game.py
--rw-rw-rw-   0        0        0      736 2022-07-14 07:43:03.000000 itchio-1.1.2/itchio/GameCollection.py
--rw-rw-rw-   0        0        0     1062 2022-07-14 07:42:10.000000 itchio-1.1.2/itchio/Purchase.py
--rw-rw-rw-   0        0        0      630 2022-07-14 07:40:38.000000 itchio-1.1.2/itchio/Session.py
--rw-rw-rw-   0        0        0     1600 2022-07-14 07:42:16.000000 itchio-1.1.2/itchio/User.py
--rw-rw-rw-   0        0        0      425 2022-07-14 07:40:35.000000 itchio-1.1.2/itchio/UserCollection.py
--rw-rw-rw-   0        0        0      232 2021-07-21 14:07:23.000000 itchio-1.1.2/itchio/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-14 07:46:30.222484 itchio-1.1.2/itchio.egg-info/
--rw-rw-rw-   0        0        0     1735 2022-07-14 07:46:29.000000 itchio-1.1.2/itchio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2022-07-14 07:46:29.000000 itchio-1.1.2/itchio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-14 07:46:29.000000 itchio-1.1.2/itchio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-07-14 07:46:29.000000 itchio-1.1.2/itchio.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-07-14 07:46:29.000000 itchio-1.1.2/itchio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-14 07:46:30.224486 itchio-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      482 2022-07-14 07:40:32.000000 itchio-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:54:18.615954 itchio-1.1.3/
+-rw-rw-rw-   0        0        0     1091 2021-07-22 08:24:28.000000 itchio-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1745 2024-04-21 14:54:18.614953 itchio-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1401 2024-04-21 12:49:48.000000 itchio-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 14:54:18.587529 itchio-1.1.3/itchio/
+-rw-rw-rw-   0        0        0      772 2022-07-14 07:52:10.000000 itchio-1.1.3/itchio/DownloadKey.py
+-rw-rw-rw-   0        0        0      488 2022-07-14 07:52:10.000000 itchio-1.1.3/itchio/Earnings.py
+-rw-rw-rw-   0        0        0     5225 2024-04-21 14:54:09.000000 itchio-1.1.3/itchio/Game.py
+-rw-rw-rw-   0        0        0      736 2022-07-14 07:52:10.000000 itchio-1.1.3/itchio/GameCollection.py
+-rw-rw-rw-   0        0        0     1062 2022-07-14 07:52:10.000000 itchio-1.1.3/itchio/Purchase.py
+-rw-rw-rw-   0        0        0      630 2022-07-14 07:52:10.000000 itchio-1.1.3/itchio/Session.py
+-rw-rw-rw-   0        0        0     1600 2024-04-21 12:37:41.000000 itchio-1.1.3/itchio/User.py
+-rw-rw-rw-   0        0        0      425 2022-07-14 07:52:10.000000 itchio-1.1.3/itchio/UserCollection.py
+-rw-rw-rw-   0        0        0      232 2021-07-21 14:07:23.000000 itchio-1.1.3/itchio/__init__.py
+-rw-rw-rw-   0        0        0      378 2024-04-21 14:54:09.000000 itchio-1.1.3/itchio/utility.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:54:18.612954 itchio-1.1.3/itchio.egg-info/
+-rw-rw-rw-   0        0        0     1745 2024-04-21 14:54:18.000000 itchio-1.1.3/itchio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2024-04-21 14:54:18.000000 itchio-1.1.3/itchio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 14:54:18.000000 itchio-1.1.3/itchio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-21 14:54:18.000000 itchio-1.1.3/itchio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-21 14:54:18.000000 itchio-1.1.3/itchio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 14:54:18.616953 itchio-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      482 2024-04-21 14:54:09.000000 itchio-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:54:18.611954 itchio-1.1.3/tests/
+-rw-rw-rw-   0        0        0     3252 2021-07-21 17:03:01.000000 itchio-1.1.3/tests/test.py
```

### Comparing `itchio-1.1.2/LICENSE` & `itchio-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `itchio-1.1.2/PKG-INFO` & `itchio-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: itchio
-Version: 1.1.2
+Version: 1.1.3
 Summary: Interact with the REST-API of itch.io
 Home-page: https://github.com/Tch1b0/itchio-lib
 Author: Johannes Pour
 Author-email: jpour3006@gmail.com
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.31.0
 
 # itchio-lib
 
 Use the REST-API of itch.io with python in a simple way.
 
 ## Installation
 
@@ -79,9 +79,7 @@
 
 print(me.username)
 ```
 
 ```
 Tch1b0
 ```
-
-
```

### Comparing `itchio-1.1.2/README.md` & `itchio-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `itchio-1.1.2/itchio/DownloadKey.py` & `itchio-1.1.3/itchio/DownloadKey.py`

 * *Files identical despite different names*

### Comparing `itchio-1.1.2/itchio/Game.py` & `itchio-1.1.3/itchio/Game.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List, Union
 from itchio.DownloadKey import DownloadKey
 from itchio.User import User
 from itchio.Purchase import Purchase
 from itchio.Session import Session
 from itchio.Earnings import Earnings
+from .utility import satisfy_dict
 
 
 class Game:
     def __init__(
             self,
             cover_url: str,
             created_at: str,
@@ -120,40 +121,29 @@
         if "errors" in data:
             raise Exception(data["errors"])
         else:
             return DownloadKey.parse_from_dict(data["download_key"])
 
     @classmethod
     def parse_from_dict(cls, data: dict, session: Session):
-        if "purchase_count" not in data:
-            data["purchase_count"] = None
-        if "earnings" not in data:
-            data["earnings"] = None
-        if "downloads_count" not in data:
-            data["downloads_count"] = None
-        if "published" not in data:
-            data["published"] = None
-        if "views_count" not in data:
-            data["views_count"] = None
-        if "title" not in data:
-            data["title"] = None
-        if "cover_url" not in data:
-            data["cover_url"] = None
-        if "created_at" not in data:
-            data["created_at"] = None
-        if "id" not in data:
-            data["id"] = None
-        if "min_price" not in data:
-            data["min_price"] = None
-        if "cover_url" not in data:
-            data["cover_url"] = None
-        if "published_at" not in data:
-            data["published_at"] = None
-        if "short_text" not in data:
-            data["short_text"] = None
+        data = satisfy_dict(data, {
+            "purchase_count": None,
+            "earnings": None,
+            "downloads_count": None,
+            "published": None,
+            "views_count": None,
+            "title": None,
+            "cover_url": None,
+            "created_at": None,
+            "id": None,
+            "min_price": None,
+            "cover_url": None,
+            "published_at": None,
+            "short_text": None,
+        })
 
         return cls(
             cover_url=data["cover_url"],
             created_at=data["created_at"],
             downloads_count=data["downloads_count"],
             id=data["id"],
             min_price=data["min_price"],
```

### Comparing `itchio-1.1.2/itchio/GameCollection.py` & `itchio-1.1.3/itchio/GameCollection.py`

 * *Files identical despite different names*

### Comparing `itchio-1.1.2/itchio/Purchase.py` & `itchio-1.1.3/itchio/Purchase.py`

 * *Files identical despite different names*

### Comparing `itchio-1.1.2/itchio/Session.py` & `itchio-1.1.3/itchio/Session.py`

 * *Files identical despite different names*

### Comparing `itchio-1.1.2/itchio/User.py` & `itchio-1.1.3/itchio/User.py`

 * *Files identical despite different names*

### Comparing `itchio-1.1.2/itchio.egg-info/PKG-INFO` & `itchio-1.1.3/itchio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: itchio
-Version: 1.1.2
+Version: 1.1.3
 Summary: Interact with the REST-API of itch.io
 Home-page: https://github.com/Tch1b0/itchio-lib
 Author: Johannes Pour
 Author-email: jpour3006@gmail.com
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.31.0
 
 # itchio-lib
 
 Use the REST-API of itch.io with python in a simple way.
 
 ## Installation
 
@@ -79,9 +79,7 @@
 
 print(me.username)
 ```
 
 ```
 Tch1b0
 ```
-
-
```


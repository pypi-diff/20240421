# Comparing `tmp/HSS.py-1.1-py3-none-any.whl.zip` & `tmp/HSS.py-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5671 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat    15497 b- defN 24-Mar-31 14:50 HSS/HSS.py
+Zip file size: 5737 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat    15848 b- defN 24-Apr-21 01:02 HSS/HSS.py
 -rw-rw-rw-  2.0 fat     1948 b- defN 24-Mar-31 14:05 HSS/Request_HSSAPI.py
 -rw-rw-rw-  2.0 fat       18 b- defN 24-Mar-31 14:37 HSS/__init__.py
 -rw-rw-rw-  2.0 fat      933 b- defN 24-Mar-31 14:05 HSS/apiurl_lists.py
 -rw-rw-rw-  2.0 fat     1222 b- defN 24-Mar-31 14:05 HSS/errors.py
--rw-rw-rw-  2.0 fat      583 b- defN 24-Mar-31 14:52 HSS.py-1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-31 14:52 HSS.py-1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 24-Mar-31 14:52 HSS.py-1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      645 b- defN 24-Mar-31 14:52 HSS.py-1.1.dist-info/RECORD
-9 files, 20942 bytes uncompressed, 4577 bytes compressed:  78.1%
+-rw-rw-rw-  2.0 fat      585 b- defN 24-Apr-21 01:05 HSS.py-1.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-21 01:05 HSS.py-1.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 24-Apr-21 01:05 HSS.py-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      653 b- defN 24-Apr-21 01:05 HSS.py-1.1.1.dist-info/RECORD
+9 files, 21303 bytes uncompressed, 4627 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: HSS/apiurl_lists.py
 Comment: 
 
 Filename: HSS/errors.py
 Comment: 
 
-Filename: HSS.py-1.1.dist-info/METADATA
+Filename: HSS.py-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: HSS.py-1.1.dist-info/WHEEL
+Filename: HSS.py-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: HSS.py-1.1.dist-info/top_level.txt
+Filename: HSS.py-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: HSS.py-1.1.dist-info/RECORD
+Filename: HSS.py-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## HSS/HSS.py

```diff
@@ -219,28 +219,28 @@
         UserData = self.get_data()
         if UserData['userDatas'] == []:
             return None
         UserData = UserData['userDatas'][number]
         return UserData['defaultTimelineData'][name]
         
     
-    def get_homework(self,number:int,name:str) -> list[dict]:
+    def get_homework(self,number) -> list[dict]:
         """"
         Retrieves the homework data for the specified number.
         
         Args:
             number (int): The number to retrieve the homework data for.
-            name (str): The name of the homework data to retrieve.
         """
         UserData = self.get_data()
         if UserData['userDatas'] == []:
             return None
         UserData = UserData['userDatas'][number]
         return UserData['homework']
-        
+
+
     def get_event(self,number:int,name:str) -> list[dict]:
         """
         Retrieves the event data for the specified number.
 
         Args:
             number (int): The number to retrieve the event data for.
             name (str): The name of the event data to retrieve.
@@ -259,15 +259,24 @@
         if UserData['userDatas'] == []:
             return None
         UserData = UserData['userDatas'][number]
         return UserData['defaultTimelineIndex']
     
     def patch_timeline(self, grade:int, _class:int, date:str, name:str, isEvent:bool,state:str = "add", index:int=None, place:str=None) -> None:
         """ 
-        
+        Retrieves the timeline data.
+        Args:
+            grade (int): The number to retrieve the timeline data for.
+            _class (int): The class number of the timeline data to retrieve.
+            date (str): The date of the timeline data to retrieve.
+            name (str): The name of the timeline data to retrieve.
+            isEvent (bool): The event boolean value of the timeline data to retrieve.
+            state (str): add, update, delete
+            index (int): update, delete only
+            place (str): default None
         """
         url = BASEURL+f"/school/{self.schoolid}/userdatas/{grade}/{_class}/{date}"
         _data = {
             "key":"timelineData",
             "value":{
                 "name":name,
                 "place":place,
@@ -277,28 +286,50 @@
         }
         if index is not None and state != "add":
             _data["index"] = index
             if state == "add":
                 raise TypeError('Cannnot index with state "add"')
         res = Request_HSSAPI.patch_with_token(url, self.token, _data)
         errors.ErrorPrint.handle_http_error(res)
+
+    def update_timelineindex(self, grade:int, _class:int, date:str, index:int) -> None:
+        """
+        Retrieves the homework data for the specified number.
+
+        Args:
+            grade (int): The number to retrieve the homework data for.
+            _class (int): The class number of the homework data to retrieve.
+            date (str): The date of the homework data to retrieve.
+            index (int): The index of the homework data to retrieve.
         
+        Returns:
+            list: The homework data for the specified number.
+        """
+        url = BASEURL+f"/school/{self.schoolid}/userdatas/{grade}/{_class}/{date}"
+        _data = {
+            "key":"defaultTimelineIndex",
+            "value" : index,
+            "state": "update"
+        }
+        res = Request_HSSAPI.patch_with_token(url, self.token, _data)
+        errors.ErrorPrint.handle_http_error(res)
+
     def patch_defaulttimeline(self, grade:int, _class:int, date:str, name:str, isEvent:bool = False,state:str ="add",index:int=None, place:str="なし") -> None:
         """
         Retrieves the default timeline data for the specified number.
 
         Args:
             grade (int): The number to retrieve the default timeline data for.
             _class (int): The class number of the default timeline data to retrieve.
             date (str): The date of the default timeline data to retrieve.
             name (str): The name of the default timeline data to retrieve.
             isEvent (bool): The event boolean value of the default timeline data to retrieve.
-            state (str): The state of the default timeline data to retrieve.
-            index (int): The index of the default timeline data to retrieve.
-            place (str): The place of the default timeline data to retrieve.
+            state (str): add, update, delete
+            index (int): update, delete only
+            place (str): default なし
         
         Returns:
             list: The default timeline data for the specified number.
         """
         url = BASEURL+f"/school/{self.schoolid}/userdatas/{grade}/{_class}/{date}"
         _data = {
             "key":"defaultTimelineData",
@@ -391,30 +422,8 @@
             "state": state
         }
         if index is not None and state != "add":
             _data["index"] = index
             if state == "add":
                 raise TypeError('Cannnot index with state "add"')
         res = Request_HSSAPI.patch_with_token(url, self.token, _data)
-        errors.ErrorPrint.handle_http_error(res)
-
-    def update_timelineindex(self, grade:int, _class:int, date:str, index:int) -> None:
-        """
-        Retrieves the homework data for the specified number.
-
-        Args:
-            grade (int): The number to retrieve the homework data for.
-            _class (int): The class number of the homework data to retrieve.
-            date (str): The date of the homework data to retrieve.
-            index (int): The index of the homework data to retrieve.
-        
-        Returns:
-            list: The homework data for the specified number.
-        """
-        url = BASEURL+f"/school/{self.schoolid}/userdatas/{grade}/{_class}/{date}"
-        _data = {
-            "key":"defaultTimelineIndex",
-            "value" : index,
-            "state": "update"
-        }
-        res = Request_HSSAPI.patch_with_token(url, self.token, _data)
         errors.ErrorPrint.handle_http_error(res)
```

## Comparing `HSS.py-1.1.dist-info/METADATA` & `HSS.py-1.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HSS.py
-Version: 1.1
+Version: 1.1.1
 Summary: Easy to use HSS API.
 Home-page: https://github.com/HSS-Project/HSS.py
 Author: HSS-Project
 Author-email: kazuma1112@munesky.net
 License: MIT
 Keywords: HSS Schedule School
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `HSS.py-1.1.dist-info/RECORD` & `HSS.py-1.1.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-HSS/HSS.py,sha256=kHeGUMV_SX4E2v1BK47Zlnc6vC9HkFIAUsGxTgKH9KY,15497
+HSS/HSS.py,sha256=OujN0ICkfK4Vd7oKVLtNxRBOY0VXIYaA4tDIwYlWGxc,15848
 HSS/Request_HSSAPI.py,sha256=Iy-dJAvDKYehTvUG5nv4_5UnwXHMtjoaPVoTTp8VR7Y,1948
 HSS/__init__.py,sha256=ID99nEkrLJLVryUweyPxYrdFEf2CBf9KFHsC1Lu-VWU,18
 HSS/apiurl_lists.py,sha256=RmVsUsMFN2q5mo4J1Ntgafx5cqvNMr1ieYiZ69zNIps,933
 HSS/errors.py,sha256=KIbxgjwrbC6xzBVIoOC37AFo1IZK_bP6Le5NVc7Wip4,1222
-HSS.py-1.1.dist-info/METADATA,sha256=HMqBlGnoyomfxYGTFrERwV2kMJhmgDPEym-1T-xgoUM,583
-HSS.py-1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-HSS.py-1.1.dist-info/top_level.txt,sha256=OdZsZ9SiQhu2j7pv4YPAKGdtHC1veorhF0ACuyNFGhU,4
-HSS.py-1.1.dist-info/RECORD,,
+HSS.py-1.1.1.dist-info/METADATA,sha256=dgcJX551Hjbw1uAkLL9HPcGBYkxxvHf4LiU2EcGtqiY,585
+HSS.py-1.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+HSS.py-1.1.1.dist-info/top_level.txt,sha256=OdZsZ9SiQhu2j7pv4YPAKGdtHC1veorhF0ACuyNFGhU,4
+HSS.py-1.1.1.dist-info/RECORD,,
```


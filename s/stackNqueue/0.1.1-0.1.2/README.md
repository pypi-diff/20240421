# Comparing `tmp/stackNqueue-0.1.1-py3-none-any.whl.zip` & `tmp/stackNqueue-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4624 bytes, number of entries: 8
+Zip file size: 4630 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat     3746 b- defN 24-Apr-21 06:50 stackNqueue/DoublyCircularLinkedList.py
--rw-rw-rw-  2.0 fat      542 b- defN 24-Apr-21 07:47 stackNqueue/Queue.py
+-rw-rw-rw-  2.0 fat      562 b- defN 24-Apr-21 08:38 stackNqueue/Queue.py
 -rw-rw-rw-  2.0 fat      434 b- defN 24-Apr-21 06:59 stackNqueue/Stack.py
--rw-rw-rw-  2.0 fat     1086 b- defN 24-Apr-21 08:28 stackNqueue-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2130 b- defN 24-Apr-21 08:28 stackNqueue-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-21 08:28 stackNqueue-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-21 08:28 stackNqueue-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      654 b- defN 24-Apr-21 08:28 stackNqueue-0.1.1.dist-info/RECORD
-8 files, 8696 bytes uncompressed, 3478 bytes compressed:  60.0%
+-rw-rw-rw-  2.0 fat     1086 b- defN 24-Apr-21 08:44 stackNqueue-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2132 b- defN 24-Apr-21 08:44 stackNqueue-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-21 08:44 stackNqueue-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-21 08:44 stackNqueue-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      654 b- defN 24-Apr-21 08:44 stackNqueue-0.1.2.dist-info/RECORD
+8 files, 8718 bytes uncompressed, 3484 bytes compressed:  60.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: stackNqueue/Queue.py
 Comment: 
 
 Filename: stackNqueue/Stack.py
 Comment: 
 
-Filename: stackNqueue-0.1.1.dist-info/LICENSE
+Filename: stackNqueue-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: stackNqueue-0.1.1.dist-info/METADATA
+Filename: stackNqueue-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: stackNqueue-0.1.1.dist-info/WHEEL
+Filename: stackNqueue-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: stackNqueue-0.1.1.dist-info/top_level.txt
+Filename: stackNqueue-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: stackNqueue-0.1.1.dist-info/RECORD
+Filename: stackNqueue-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stackNqueue/Queue.py

```diff
@@ -11,10 +11,11 @@
         self.__front = self.head.next
         self.__rear = self.head.prev
     
     def dequeue(self):
         rtn = super().pop()
         self.__front = self.head.next
         self.__rear = self.head.prev
+        return rtn
 
     def rear(self):
         return self.__rear.item
```

## Comparing `stackNqueue-0.1.1.dist-info/LICENSE` & `stackNqueue-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `stackNqueue-0.1.1.dist-info/METADATA` & `stackNqueue-0.1.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: stackNqueue
-Version: 0.1.1
+Version: 0.1.2
 Summary: simple stack, and queue using DoublyCircularLinkedList
 Home-page: https://github.com/dudasdaily/stackNqueue
 Author: dudasdaily
 Author-email: dudasdaily@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/dudasdaily/stackNqueue/releases/tag/0.1
+Download-URL: https://github.com/dudasdaily/stackNqueue/releases/tag/0.1.2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # *Welcome! stackNqueue*
 This packages includes *Stack.py*, *Queue.py*, *DoublyCircularLinkedList.py*
```

## Comparing `stackNqueue-0.1.1.dist-info/RECORD` & `stackNqueue-0.1.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 stackNqueue/DoublyCircularLinkedList.py,sha256=X5fDDLHM-A4j-SiAckhHvAKDnx3aXNvEwT9mjnD8XYU,3746
-stackNqueue/Queue.py,sha256=LgJyOWZPk07bb-H1rHdO0qOTEmDCSR3mISsLmH8RDD8,542
+stackNqueue/Queue.py,sha256=f_ruNdd0z0onDWwLE_PoAb8T4zs47VHvlCoi5Nlwh1Q,562
 stackNqueue/Stack.py,sha256=G4NyoxRV6OGyRtio01lKFysWc0sGnEhbpwijx4l7MFw,434
-stackNqueue-0.1.1.dist-info/LICENSE,sha256=um-l7cISkaJHNrkHcgBd-CuyYP0dn-n8E96pIRSkSew,1086
-stackNqueue-0.1.1.dist-info/METADATA,sha256=tpW79Pgq2-B_jPYaD95eqOh8o39l_ssdeqQtqLzxKdU,2130
-stackNqueue-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-stackNqueue-0.1.1.dist-info/top_level.txt,sha256=IRLAPpnoZUzJzklxJJO8g7tVXrHzBZIedfaZv6sT2YA,12
-stackNqueue-0.1.1.dist-info/RECORD,,
+stackNqueue-0.1.2.dist-info/LICENSE,sha256=um-l7cISkaJHNrkHcgBd-CuyYP0dn-n8E96pIRSkSew,1086
+stackNqueue-0.1.2.dist-info/METADATA,sha256=Amb-114m2fE6lQSwGxgfRse4i2WUppQLEyFeLdVpLeE,2132
+stackNqueue-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+stackNqueue-0.1.2.dist-info/top_level.txt,sha256=IRLAPpnoZUzJzklxJJO8g7tVXrHzBZIedfaZv6sT2YA,12
+stackNqueue-0.1.2.dist-info/RECORD,,
```


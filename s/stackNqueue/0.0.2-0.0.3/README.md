# Comparing `tmp/stackNqueue-0.0.2-py3-none-any.whl.zip` & `tmp/stackNqueue-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 3257 bytes, number of entries: 8
+Zip file size: 3432 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat     3746 b- defN 24-Apr-21 04:10 stackNqueue/DoublyCircularLinkedList.py
--rw-rw-rw-  2.0 fat      571 b- defN 24-Apr-21 05:50 stackNqueue/Queue.py
--rw-rw-rw-  2.0 fat      463 b- defN 24-Apr-21 05:51 stackNqueue/Stack.py
--rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-21 05:53 stackNqueue-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      265 b- defN 24-Apr-21 05:53 stackNqueue-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-21 05:53 stackNqueue-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-21 05:53 stackNqueue-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      651 b- defN 24-Apr-21 05:53 stackNqueue-0.0.2.dist-info/RECORD
-8 files, 5815 bytes uncompressed, 2111 bytes compressed:  63.7%
+-rw-rw-rw-  2.0 fat      488 b- defN 24-Apr-21 06:19 stackNqueue/Queue.py
+-rw-rw-rw-  2.0 fat      379 b- defN 24-Apr-21 06:19 stackNqueue/Stack.py
+-rw-rw-rw-  2.0 fat      113 b- defN 24-Apr-21 06:35 stackNqueue/__init__.py
+-rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-21 06:36 stackNqueue-0.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      265 b- defN 24-Apr-21 06:36 stackNqueue-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-21 06:36 stackNqueue-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-21 06:36 stackNqueue-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      730 b- defN 24-Apr-21 06:36 stackNqueue-0.0.3.dist-info/RECORD
+9 files, 5840 bytes uncompressed, 2164 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -3,23 +3,26 @@
 
 Filename: stackNqueue/Queue.py
 Comment: 
 
 Filename: stackNqueue/Stack.py
 Comment: 
 
-Filename: stackNqueue-0.0.2.dist-info/LICENSE
+Filename: stackNqueue/__init__.py
 Comment: 
 
-Filename: stackNqueue-0.0.2.dist-info/METADATA
+Filename: stackNqueue-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: stackNqueue-0.0.2.dist-info/WHEEL
+Filename: stackNqueue-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: stackNqueue-0.0.2.dist-info/top_level.txt
+Filename: stackNqueue-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: stackNqueue-0.0.2.dist-info/RECORD
+Filename: stackNqueue-0.0.3.dist-info/top_level.txt
+Comment: 
+
+Filename: stackNqueue-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stackNqueue/Queue.py

```diff
@@ -1,9 +1,7 @@
-from stackNqueue.DoublyCircularLinkedList import Node, DoublyCircularLinkedList
-
 class Queue(DoublyCircularLinkedList):
     def __init__(self):
         super().__init__()
         self.__front = self.head
         self.__rear = self.tail
 
     def enqueue(self, x):
```

## stackNqueue/Stack.py

```diff
@@ -1,9 +1,7 @@
-from stackNqueue.DoublyCircularLinkedList import Node, DoublyCircularLinkedList:
-
 class Stack(DoublyCircularLinkedList):
     def __init__(self):
         super().__init__()
         self.__top = self.head
 
     def push(self, x):
         super().append(x)
```

## Comparing `stackNqueue-0.0.2.dist-info/RECORD` & `stackNqueue-0.0.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 stackNqueue/DoublyCircularLinkedList.py,sha256=X5fDDLHM-A4j-SiAckhHvAKDnx3aXNvEwT9mjnD8XYU,3746
-stackNqueue/Queue.py,sha256=ak5Px5Y0aLJCfDhF96RaSRZmW239bPwIRhQhzAoG8Bk,571
-stackNqueue/Stack.py,sha256=-NiDTYOKTQlRRR8OpjZflKjGf5f2-uDFA8S7-2kHy6M,463
-stackNqueue-0.0.2.dist-info/LICENSE,sha256=DHu9bfKrXgXcNuKhv_LfGDX29PIK-oDzbMgvZWS-rqg,15
-stackNqueue-0.0.2.dist-info/METADATA,sha256=tf9864LTeriaXfkxdC8HSrX8Icv2xH9odfkA4pFCSRU,265
-stackNqueue-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-stackNqueue-0.0.2.dist-info/top_level.txt,sha256=IRLAPpnoZUzJzklxJJO8g7tVXrHzBZIedfaZv6sT2YA,12
-stackNqueue-0.0.2.dist-info/RECORD,,
+stackNqueue/Queue.py,sha256=LGAiyisaYE-zWysOEwBPVXqfpFh8hdfrZGVS_dzk_FI,488
+stackNqueue/Stack.py,sha256=NuTT4p0iHgb3Nm_y6_7O41TRatqgCrLpGTMBzVnI374,379
+stackNqueue/__init__.py,sha256=hrjydOBSP9_qSvm5fBGgK8BTIXjASY2DlcVLPMPyY3g,113
+stackNqueue-0.0.3.dist-info/LICENSE,sha256=DHu9bfKrXgXcNuKhv_LfGDX29PIK-oDzbMgvZWS-rqg,15
+stackNqueue-0.0.3.dist-info/METADATA,sha256=MxPrgT7xV576-dAx360oYP9V_cQyh2fpmIVAga-ebJs,265
+stackNqueue-0.0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+stackNqueue-0.0.3.dist-info/top_level.txt,sha256=IRLAPpnoZUzJzklxJJO8g7tVXrHzBZIedfaZv6sT2YA,12
+stackNqueue-0.0.3.dist-info/RECORD,,
```


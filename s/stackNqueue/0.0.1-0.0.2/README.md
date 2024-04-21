# Comparing `tmp/stackNqueue-0.0.1-py3-none-any.whl.zip` & `tmp/stackNqueue-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3226 bytes, number of entries: 8
+Zip file size: 3257 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat     3746 b- defN 24-Apr-21 04:10 stackNqueue/DoublyCircularLinkedList.py
--rw-rw-rw-  2.0 fat      530 b- defN 24-Apr-21 04:50 stackNqueue/Queue.py
--rw-rw-rw-  2.0 fat      421 b- defN 24-Apr-21 04:17 stackNqueue/Stack.py
--rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-21 05:28 stackNqueue-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      265 b- defN 24-Apr-21 05:28 stackNqueue-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-21 05:28 stackNqueue-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-21 05:28 stackNqueue-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      651 b- defN 24-Apr-21 05:28 stackNqueue-0.0.1.dist-info/RECORD
-8 files, 5732 bytes uncompressed, 2080 bytes compressed:  63.7%
+-rw-rw-rw-  2.0 fat      571 b- defN 24-Apr-21 05:50 stackNqueue/Queue.py
+-rw-rw-rw-  2.0 fat      463 b- defN 24-Apr-21 05:51 stackNqueue/Stack.py
+-rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-21 05:53 stackNqueue-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      265 b- defN 24-Apr-21 05:53 stackNqueue-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-21 05:53 stackNqueue-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-21 05:53 stackNqueue-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      651 b- defN 24-Apr-21 05:53 stackNqueue-0.0.2.dist-info/RECORD
+8 files, 5815 bytes uncompressed, 2111 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: stackNqueue/Queue.py
 Comment: 
 
 Filename: stackNqueue/Stack.py
 Comment: 
 
-Filename: stackNqueue-0.0.1.dist-info/LICENSE
+Filename: stackNqueue-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: stackNqueue-0.0.1.dist-info/METADATA
+Filename: stackNqueue-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: stackNqueue-0.0.1.dist-info/WHEEL
+Filename: stackNqueue-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: stackNqueue-0.0.1.dist-info/top_level.txt
+Filename: stackNqueue-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: stackNqueue-0.0.1.dist-info/RECORD
+Filename: stackNqueue-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stackNqueue/Queue.py

```diff
@@ -1,8 +1,8 @@
-from DoublyCircularLinkedList import *
+from stackNqueue.DoublyCircularLinkedList import Node, DoublyCircularLinkedList
 
 class Queue(DoublyCircularLinkedList):
     def __init__(self):
         super().__init__()
         self.__front = self.head
         self.__rear = self.tail
```

## stackNqueue/Stack.py

```diff
@@ -1,8 +1,8 @@
-from DoublyCircularLinkedList import *
+from stackNqueue.DoublyCircularLinkedList import Node, DoublyCircularLinkedList:
 
 class Stack(DoublyCircularLinkedList):
     def __init__(self):
         super().__init__()
         self.__top = self.head
 
     def push(self, x):
```


# Comparing `tmp/min1129-0.0.0.1-py3-none-any.whl.zip` & `tmp/min1129-0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 1511 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat       23 b- defN 24-Apr-21 14:32 min1129/__init__.py
+Zip file size: 3151 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     2964 b- defN 24-Apr-21 15:06 min1129/LinkedList.py
+-rw-rw-rw-  2.0 fat      113 b- defN 24-Apr-21 15:06 min1129/ListNode.py
+-rw-rw-rw-  2.0 fat       34 b- defN 24-Apr-21 15:06 min1129/__init__.py
 -rw-rw-rw-  2.0 fat       51 b- defN 24-Apr-21 14:32 min1129/untitled.py
--rw-rw-rw-  2.0 fat      269 b- defN 24-Apr-21 14:36 min1129-0.0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-21 14:36 min1129-0.0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-21 14:36 min1129-0.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      452 b- defN 24-Apr-21 14:36 min1129-0.0.0.1.dist-info/RECORD
-6 files, 895 bytes uncompressed, 685 bytes compressed:  23.5%
+-rw-rw-rw-  2.0 fat      784 b- defN 24-Apr-21 15:08 min1129-0.0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-21 15:08 min1129-0.0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-21 15:08 min1129-0.0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      605 b- defN 24-Apr-21 15:08 min1129-0.0.0.2.dist-info/RECORD
+8 files, 4651 bytes uncompressed, 2093 bytes compressed:  55.0%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
+Filename: min1129/LinkedList.py
+Comment: 
+
+Filename: min1129/ListNode.py
+Comment: 
+
 Filename: min1129/__init__.py
 Comment: 
 
 Filename: min1129/untitled.py
 Comment: 
 
-Filename: min1129-0.0.0.1.dist-info/METADATA
+Filename: min1129-0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: min1129-0.0.0.1.dist-info/WHEEL
+Filename: min1129-0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: min1129-0.0.0.1.dist-info/top_level.txt
+Filename: min1129-0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: min1129-0.0.0.1.dist-info/RECORD
+Filename: min1129-0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## min1129/__init__.py

```diff
@@ -1 +1 @@
-__all__=['hello_world']
+__all__=['LinkedList', 'ListNode']
```


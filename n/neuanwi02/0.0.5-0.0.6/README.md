# Comparing `tmp/neuanwi02-0.0.5-py3-none-any.whl.zip` & `tmp/neuanwi02-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1507 bytes, number of entries: 6
--rw-r--r--  2.0 unx      238 b- defN 24-Apr-12 05:19 algo/easy.py
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-12 05:20 neuanwi02-0.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      124 b- defN 24-Apr-12 05:20 neuanwi02-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 05:20 neuanwi02-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-12 05:20 neuanwi02-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      460 b- defN 24-Apr-12 05:20 neuanwi02-0.0.5.dist-info/RECORD
-6 files, 936 bytes uncompressed, 667 bytes compressed:  28.7%
+Zip file size: 1678 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      495 b- defN 24-Apr-21 10:41 algo/easy.py
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-21 10:42 neuanwi02-0.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      124 b- defN 24-Apr-21 10:42 neuanwi02-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 10:42 neuanwi02-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-21 10:42 neuanwi02-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      460 b- defN 24-Apr-21 10:42 neuanwi02-0.0.6.dist-info/RECORD
+6 files, 1193 bytes uncompressed, 838 bytes compressed:  29.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: algo/easy.py
 Comment: 
 
-Filename: neuanwi02-0.0.5.dist-info/LICENSE
+Filename: neuanwi02-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: neuanwi02-0.0.5.dist-info/METADATA
+Filename: neuanwi02-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: neuanwi02-0.0.5.dist-info/WHEEL
+Filename: neuanwi02-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: neuanwi02-0.0.5.dist-info/top_level.txt
+Filename: neuanwi02-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: neuanwi02-0.0.5.dist-info/RECORD
+Filename: neuanwi02-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algo/easy.py

```diff
@@ -5,7 +5,13 @@
   h = []
   result = []
   for value in iterable:
     heapq.heappush(h, value)
   for i in range(len(h)):
     result.append(heapq.heappop(h))
   return result
+
+def calCountsByRange(nums, left_value, right_value):
+    r_i = bisect_right(nums, right_value)
+    l_i = bisect_left(nums, left_value)
+    return r_i - l_i
+# 출처: https://programming119.tistory.com/196 [개발자 아저씨들 힘을모아:티스토리]
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


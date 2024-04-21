# Comparing `tmp/Sonihi_K-0.0.1-py3-none-any.whl.zip` & `tmp/Sonihi_K-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1306 bytes, number of entries: 5
--rw-r--r--  2.0 unx      141 b- defN 24-Apr-21 11:08 mycalc/calculator.py
--rw-r--r--  2.0 unx      237 b- defN 24-Apr-21 11:20 Sonihi_K-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 11:20 Sonihi_K-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-21 11:20 Sonihi_K-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      376 b- defN 24-Apr-21 11:20 Sonihi_K-0.0.1.dist-info/RECORD
-5 files, 853 bytes uncompressed, 600 bytes compressed:  29.7%
+Zip file size: 1487 bytes, number of entries: 5
+-rw-r--r--  2.0 unx      473 b- defN 24-Apr-21 13:22 mycalc/calculator.py
+-rw-r--r--  2.0 unx      238 b- defN 24-Apr-21 14:04 Sonihi_K-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 14:04 Sonihi_K-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-21 14:04 Sonihi_K-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      376 b- defN 24-Apr-21 14:04 Sonihi_K-0.2.0.dist-info/RECORD
+5 files, 1186 bytes uncompressed, 781 bytes compressed:  34.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: mycalc/calculator.py
 Comment: 
 
-Filename: Sonihi_K-0.0.1.dist-info/METADATA
+Filename: Sonihi_K-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: Sonihi_K-0.0.1.dist-info/WHEEL
+Filename: Sonihi_K-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: Sonihi_K-0.0.1.dist-info/top_level.txt
+Filename: Sonihi_K-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: Sonihi_K-0.0.1.dist-info/RECORD
+Filename: Sonihi_K-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mycalc/calculator.py

```diff
@@ -1,11 +1,16 @@
-def add(a,b):
-    return a+b
+import numpy as np
+import pandas as pd
+import matplotlib.pyplot as plt
+import webbrowser
 
-def subtract(a,b):
-    return a-b
+def open_naver_sports_baseball_schedule():
+    url = "https://sports.news.naver.com/schedule/scoreBoard.nhn?category=mlb&date=20220416"
+    webbrowser.open(url)
 
-def multiply(a,b):
-    return a*b
+open_naver_sports_baseball_schedule()
 
-def divide(a,b):
-    return a/b
+def open_naver_weather():
+    url = "https://search.naver.com/search.naver?sm=top_hty&fbm=1&ie=utf8&query=오늘+날씨"
+    webbrowser.open(url)
+
+open_naver_weather()
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


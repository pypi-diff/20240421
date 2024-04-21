# Comparing `tmp/ossStudy-0.0.2-py3-none-any.whl.zip` & `tmp/ossStudy-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1386 bytes, number of entries: 4
--rw-r--r--  2.0 unx      727 b- defN 24-Apr-21 10:54 ossStudy-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 10:54 ossStudy-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-21 10:54 ossStudy-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      300 b- defN 24-Apr-21 10:54 ossStudy-0.0.2.dist-info/RECORD
-4 files, 1128 bytes uncompressed, 796 bytes compressed:  29.4%
+Zip file size: 1420 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      769 b- defN 24-Apr-21 10:58 ossStudy-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 10:58 ossStudy-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-21 10:58 ossStudy-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      300 b- defN 24-Apr-21 10:58 ossStudy-0.0.3.dist-info/RECORD
+4 files, 1170 bytes uncompressed, 830 bytes compressed:  29.1%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: ossStudy-0.0.2.dist-info/METADATA
+Filename: ossStudy-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: ossStudy-0.0.2.dist-info/WHEEL
+Filename: ossStudy-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: ossStudy-0.0.2.dist-info/top_level.txt
+Filename: ossStudy-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: ossStudy-0.0.2.dist-info/RECORD
+Filename: ossStudy-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ossStudy-0.0.2.dist-info/METADATA` & `ossStudy-0.0.3.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: ossStudy
-Version: 0.0.2
+Version: 0.0.3
 Summary: oss dev study
 Home-page: https://github.com/bluefrog1413/oss-2024
 Download-URL: https://github.com/bluefrog1413/oss-2024
 Author: hangyeolkim
 Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
 
-이 패키지는 자주사용하는 numpy, pandas, matplotlib 라이브러리 3개가 들어가 있습니다. 
+# 이 패키지는 자주사용하는 numpy, pandas, matplotlib 라이브러리 3개가 들어가 있습니다. 
 또한, today 함수와 lmsSite 함수가 들어 있습니다.
 today 함수는 today(a,b)로 사용하며 a : 월 , b : 일 을 넣어 오늘 코딩한 날짜를 출력할 수 있습니다.
 lmsSite 함수는 코딩중에 모르는 잊어버린 개념을 매번 구글에서 동아대 lms를 칠 필요 없이 lmsSite() 만 치면 바로 접속할 수 있습니다.
```


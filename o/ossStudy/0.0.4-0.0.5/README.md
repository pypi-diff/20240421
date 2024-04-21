# Comparing `tmp/ossStudy-0.0.4-py3-none-any.whl.zip` & `tmp/ossStudy-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
 Zip file size: 1435 bytes, number of entries: 4
--rw-r--r--  2.0 unx      814 b- defN 24-Apr-21 11:02 ossStudy-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 11:02 ossStudy-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-21 11:02 ossStudy-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      300 b- defN 24-Apr-21 11:02 ossStudy-0.0.4.dist-info/RECORD
+-rw-r--r--  2.0 unx      814 b- defN 24-Apr-21 11:03 ossStudy-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 11:03 ossStudy-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-21 11:03 ossStudy-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      300 b- defN 24-Apr-21 11:03 ossStudy-0.0.5.dist-info/RECORD
 4 files, 1215 bytes uncompressed, 845 bytes compressed:  30.5%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: ossStudy-0.0.4.dist-info/METADATA
+Filename: ossStudy-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: ossStudy-0.0.4.dist-info/WHEEL
+Filename: ossStudy-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: ossStudy-0.0.4.dist-info/top_level.txt
+Filename: ossStudy-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: ossStudy-0.0.4.dist-info/RECORD
+Filename: ossStudy-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ossStudy-0.0.4.dist-info/METADATA` & `ossStudy-0.0.5.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: ossStudy
-Version: 0.0.4
+Version: 0.0.5
 Summary: oss dev study
 Home-page: https://github.com/bluefrog1413/oss-2024
 Download-URL: https://github.com/bluefrog1413/oss-2024
 Author: hangyeolkim
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
-# 패키지 설명 이 패키지는 자주사용하는 **numpy, pandas, matplotlib 라이브러리** 3개가 들어가 있습니다. 
+# 패키지 설명
+이 패키지는 자주사용하는 **numpy, pandas, matplotlib 라이브러리** 3개가 들어가 있습니다. 
 또한, **today 함수**와 **lmsSite 함수**가 들어 있습니다.
 **today 함수**는 **today(a,b)**로 사용하며 a : 월 , b : 일 을 넣어 오늘 코딩한 날짜를 출력할 수 있습니다.
 **lmsSite 함수**는 코딩중에 모르는 잊어버린 개념을 매번 구글에서 동아대 lms를 칠 필요 없이 **lmsSite()** 만 치면 바로 접속할 수 있습니다.
```


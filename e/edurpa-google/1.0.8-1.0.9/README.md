# Comparing `tmp/edurpa_google-1.0.8-py3-none-any.whl.zip` & `tmp/edurpa_google-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9221 bytes, number of entries: 11
+Zip file size: 9220 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-17 16:24 EduRPA/__init__.py
 -rw-rw-rw-  2.0 fat    13103 b- defN 24-Apr-18 09:37 EduRPA/Google/Classroom.py
 -rw-rw-rw-  2.0 fat     1549 b- defN 24-Apr-18 09:37 EduRPA/Google/CustomOAuth.py
 -rw-rw-rw-  2.0 fat    11964 b- defN 24-Apr-18 09:38 EduRPA/Google/Form.py
 -rw-rw-rw-  2.0 fat      313 b- defN 24-Apr-17 14:41 EduRPA/Google/Utils.py
--rw-rw-rw-  2.0 fat      117 b- defN 24-Apr-21 02:46 EduRPA/Google/__init__.py
--rw-rw-rw-  2.0 fat     1088 b- defN 24-Apr-21 02:47 edurpa_google-1.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      670 b- defN 24-Apr-21 02:47 edurpa_google-1.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-21 02:47 edurpa_google-1.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-21 02:47 edurpa_google-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      893 b- defN 24-Apr-21 02:47 edurpa_google-1.0.8.dist-info/RECORD
-11 files, 29796 bytes uncompressed, 7705 bytes compressed:  74.1%
+-rw-rw-rw-  2.0 fat      121 b- defN 24-Apr-21 02:51 EduRPA/Google/__init__.py
+-rw-rw-rw-  2.0 fat     1088 b- defN 24-Apr-21 02:51 edurpa_google-1.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      670 b- defN 24-Apr-21 02:51 edurpa_google-1.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-21 02:51 edurpa_google-1.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-21 02:51 edurpa_google-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      893 b- defN 24-Apr-21 02:51 edurpa_google-1.0.9.dist-info/RECORD
+11 files, 29800 bytes uncompressed, 7704 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: EduRPA/Google/Utils.py
 Comment: 
 
 Filename: EduRPA/Google/__init__.py
 Comment: 
 
-Filename: edurpa_google-1.0.8.dist-info/LICENSE
+Filename: edurpa_google-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: edurpa_google-1.0.8.dist-info/METADATA
+Filename: edurpa_google-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: edurpa_google-1.0.8.dist-info/WHEEL
+Filename: edurpa_google-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: edurpa_google-1.0.8.dist-info/top_level.txt
+Filename: edurpa_google-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: edurpa_google-1.0.8.dist-info/RECORD
+Filename: edurpa_google-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## EduRPA/Google/__init__.py

```diff
@@ -1,5 +1,5 @@
 name = 'edurpa_google'
-from Classroom import *
-from CustomOAuth import *
-from Form import *
-from Utils import *
+from .Classroom import *
+from .CustomOAuth import *
+from .Form import *
+from .Utils import *
```

## Comparing `edurpa_google-1.0.8.dist-info/LICENSE` & `edurpa_google-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edurpa_google-1.0.8.dist-info/METADATA` & `edurpa_google-1.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edurpa-google
-Version: 1.0.8
+Version: 1.0.9
 Summary: Education Google RPA Librabry For Education
 Home-page: https://github.com/edu-rpa/edurpa-google
 Author: david
 Author-email: davidhuynh0222@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `edurpa_google-1.0.8.dist-info/RECORD` & `edurpa_google-1.0.9.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 EduRPA/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 EduRPA/Google/Classroom.py,sha256=ZUMo0Dlc46bFwAUnUHKrbOl_RzvOvVHWAQtfa3hJPqQ,13103
 EduRPA/Google/CustomOAuth.py,sha256=mdcF-tqze2HulL4QZ6K-dl-dr-Am8qLSB3opr2F9PkM,1549
 EduRPA/Google/Form.py,sha256=K4SdXFT6VKbreHnNebTjGtEDuJoPC7JnKD4t1xSB55Y,11964
 EduRPA/Google/Utils.py,sha256=isWNWUMrlhzVR8q5MG6XeYs8QI5fOYRCA22xvZd3MbI,313
-EduRPA/Google/__init__.py,sha256=gW7xWpbnvOXRNJuf-YRdAIbUL6sUM0t9V94lHIgSUkw,117
-edurpa_google-1.0.8.dist-info/LICENSE,sha256=YgvlMcXsea3kZqp1y62n8AgkwZp6xXbWSYW17pT58Yg,1088
-edurpa_google-1.0.8.dist-info/METADATA,sha256=69zgRc3S81YOcll4C0qb-IBgL3q5nU4oFno7dz--bmM,670
-edurpa_google-1.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-edurpa_google-1.0.8.dist-info/top_level.txt,sha256=Wl0EDd9il1J3fz62-gLcRCpFYSlEbU4KVE_SNWkcpaI,7
-edurpa_google-1.0.8.dist-info/RECORD,,
+EduRPA/Google/__init__.py,sha256=uBNkcFMNiqfTFJkohc-ob-H8zx05ZZtcLhvgTtdimN4,121
+edurpa_google-1.0.9.dist-info/LICENSE,sha256=YgvlMcXsea3kZqp1y62n8AgkwZp6xXbWSYW17pT58Yg,1088
+edurpa_google-1.0.9.dist-info/METADATA,sha256=8Vc9lmCQvww1wkBSuaR5FLnBuyXwTfStiemJQ7V5tf4,670
+edurpa_google-1.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+edurpa_google-1.0.9.dist-info/top_level.txt,sha256=Wl0EDd9il1J3fz62-gLcRCpFYSlEbU4KVE_SNWkcpaI,7
+edurpa_google-1.0.9.dist-info/RECORD,,
```


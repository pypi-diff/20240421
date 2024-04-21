# Comparing `tmp/mycalculator_report-0.0.2-py3-none-any.whl.zip` & `tmp/mycalculator_report-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1284 bytes, number of entries: 5
--rw-r--r--  2.0 unx       28 b- defN 24-Apr-19 02:13 mycalc/calulator.py
--rw-r--r--  2.0 unx      112 b- defN 24-Apr-19 02:13 mycalculator_report-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 02:13 mycalculator_report-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-19 02:13 mycalculator_report-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      418 b- defN 24-Apr-19 02:13 mycalculator_report-0.0.2.dist-info/RECORD
-5 files, 657 bytes uncompressed, 492 bytes compressed:  25.1%
+Zip file size: 1735 bytes, number of entries: 5
+-rw-r--r--  2.0 unx      913 b- defN 24-Apr-21 11:48 mycalc/calulator.py
+-rw-r--r--  2.0 unx      112 b- defN 24-Apr-21 11:49 mycalculator_report-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 11:49 mycalculator_report-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-21 11:49 mycalculator_report-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      419 b- defN 24-Apr-21 11:49 mycalculator_report-0.0.3.dist-info/RECORD
+5 files, 1543 bytes uncompressed, 943 bytes compressed:  38.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: mycalc/calulator.py
 Comment: 
 
-Filename: mycalculator_report-0.0.2.dist-info/METADATA
+Filename: mycalculator_report-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: mycalculator_report-0.0.2.dist-info/WHEEL
+Filename: mycalculator_report-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: mycalculator_report-0.0.2.dist-info/top_level.txt
+Filename: mycalculator_report-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: mycalculator_report-0.0.2.dist-info/RECORD
+Filename: mycalculator_report-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mycalc/calulator.py

```diff
@@ -1,3 +1,31 @@
 
-def add(a,b):
-  return a+b
+import random
+import string
+
+#자음과 모음을 조합해서 간단한 닉네임을 만들어주는 코드
+def nicknamemake():
+
+    consonants = 'bcdfghjklmnpqrstvwxyz'
+    vowels = 'aeiou'
+
+    nickname = ''
+
+    for _ in range(2):
+        nickname += random.choice(consonants).lower()
+        nickname += random.choice(vowels).lower()
+
+    return nickname
+
+#총 8자리의 비밀번호를 만들어주는 함수 / 1자리=>영어 대문자, 2~4자리=>영어 소문자, 5~6자리=>숫자, 7~8자리=> 특정 특수기호
+def passwordmake():
+
+    first_letter = random.choice(string.ascii_uppercase)
+    rest_letters = ''.join(random.choice(string.ascii_lowercase) for i in range(3))
+
+    digits = ''.join(str(random.randint(0, 9)) for i in range(2))
+
+    special_chars = ''.join(random.choice("~!^*") for i in range(2))
+
+    password = first_letter+ rest_letters+ digits + special_chars
+
+    return password
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


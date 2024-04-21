# Comparing `tmp/Signix-0.0.1-py3-none-any.whl.zip` & `tmp/Signix-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3263 bytes, number of entries: 7
+Zip file size: 3289 bytes, number of entries: 7
 -rw-r--r--  2.0 unx     2649 b- defN 24-Apr-21 07:56 info/Loginator.py
--rw-r--r--  2.0 unx     2649 b- defN 24-Apr-21 08:00 info/Signix.py
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-21 08:01 Signix-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      121 b- defN 24-Apr-21 08:01 Signix-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 08:01 Signix-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-21 08:01 Signix-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      522 b- defN 24-Apr-21 08:01 Signix-0.0.1.dist-info/RECORD
-7 files, 6055 bytes uncompressed, 2339 bytes compressed:  61.4%
+-rw-r--r--  2.0 unx     2597 b- defN 24-Apr-21 08:07 info/Signix.py
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-21 08:08 Signix-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      121 b- defN 24-Apr-21 08:08 Signix-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 08:08 Signix-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-21 08:08 Signix-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      522 b- defN 24-Apr-21 08:08 Signix-0.0.2.dist-info/RECORD
+7 files, 6003 bytes uncompressed, 2365 bytes compressed:  60.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: info/Loginator.py
 Comment: 
 
 Filename: info/Signix.py
 Comment: 
 
-Filename: Signix-0.0.1.dist-info/LICENSE
+Filename: Signix-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: Signix-0.0.1.dist-info/METADATA
+Filename: Signix-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: Signix-0.0.1.dist-info/WHEEL
+Filename: Signix-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: Signix-0.0.1.dist-info/top_level.txt
+Filename: Signix-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: Signix-0.0.1.dist-info/RECORD
+Filename: Signix-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## info/Signix.py

```diff
@@ -1,84 +1,84 @@
 
 import re
 import string
 import pandas as pd
 
-def validate_email(email):
+def check_email(email):
     pattern = r'^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$'
     if re.match(pattern, email):
         return True
     else:
         return False
 
-def format_phone_number(phone_number):
+def check_phone_number(phone_number):
     pattern = r'(\d{3})(\d{3})(\d{4})'
     formatted_number = re.sub(pattern, '\1-\2-\3', phone_number)
     return formatted_number
 
-def validate_name(name):
+def check_name(name):
     if not name:
         return False
     if len(name) <= 8:
         if all(char in string.ascii_letters or char in string.whitespace for char in name):
             return True
     return False
 
-def validate_id(id):
+def check_id(id):
     if not id:
         return False
     if len(id) < 4:
         return False
     if len(id) > 8:
         return False
     pattern = r'^[a-zA-Z]{2,}[0-9]{1,}$'
     if re.match(pattern, id):
         return True
     else:
         return False
 
-def validate_pwd(pwd):
+def check_pwd(pwd):
     if not pwd:
         return False
     if len(pwd) >= 8 and len(pwd) <= 20:
         pattern = r'^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*?&])[A-Za-z\d@$!%*?&]{8,20}$'
         if re.fullmatch(pattern, pwd):
             return True
     else:
         return False
 
-def validate_input(email, name, user_id, password, phone_number):
-    return (validate_email(email) and
-            validate_name(name) and
-            validate_id(user_id) and
-            validate_pwd(password))
+def check_input(email, name, user_id, password, phone_number):
+    return (check_email(email) and
+            check_name(name) and
+            check_id(user_id) and
+            check_pwd(password))
 
 def add_user_info(df, email, name, user_id, password, phone_number):
-    if validate_email(email) and validate_name(name) and validate_id(user_id) and validate_pwd(password):
+    if check_email(email) and check_name(name) and check_id(user_id) and check_pwd(password):
         df = pd.concat([df, pd.DataFrame({
             'name': [name],
             'email': [email],
             'phone_number': [phone_number],
             'id': [user_id],
             'password': [password],
         })], ignore_index=True)
         return df
 
 def check_info(email, name, user_id, password):
     i=0
-    if not validate_email(email):
+    if not check_email(email):
         print("이메일 형식을 확인해주세요.")
         i+=1
-    if not validate_name(name):
+    if not check_name(name):
         print("이름 형식을 확인해주세요.")
         i+=1
-    if not validate_id(user_id):
+    if not check_id(user_id):
         print("아이디 형식을 확인해주세요")
         i+=1
-    if not validate_pwd(password):
+    if not check_pwd(password):
         print("비밀번호 형식을 확인해주세요.")
         i+=1
     if i!=0:
         return False
     else:
         return True
```


# Comparing `tmp/Signix-0.0.2-py3-none-any.whl.zip` & `tmp/Signix-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3289 bytes, number of entries: 7
+Zip file size: 3218 bytes, number of entries: 7
 -rw-r--r--  2.0 unx     2649 b- defN 24-Apr-21 07:56 info/Loginator.py
--rw-r--r--  2.0 unx     2597 b- defN 24-Apr-21 08:07 info/Signix.py
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-21 08:08 Signix-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      121 b- defN 24-Apr-21 08:08 Signix-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 08:08 Signix-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-21 08:08 Signix-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      522 b- defN 24-Apr-21 08:08 Signix-0.0.2.dist-info/RECORD
-7 files, 6003 bytes uncompressed, 2365 bytes compressed:  60.6%
+-rw-r--r--  2.0 unx     2344 b- defN 24-Apr-21 08:14 info/Signix.py
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-21 08:14 Signix-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      121 b- defN 24-Apr-21 08:14 Signix-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 08:14 Signix-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-21 08:14 Signix-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      522 b- defN 24-Apr-21 08:14 Signix-0.0.3.dist-info/RECORD
+7 files, 5750 bytes uncompressed, 2294 bytes compressed:  60.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: info/Loginator.py
 Comment: 
 
 Filename: info/Signix.py
 Comment: 
 
-Filename: Signix-0.0.2.dist-info/LICENSE
+Filename: Signix-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: Signix-0.0.2.dist-info/METADATA
+Filename: Signix-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: Signix-0.0.2.dist-info/WHEEL
+Filename: Signix-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: Signix-0.0.2.dist-info/top_level.txt
+Filename: Signix-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: Signix-0.0.2.dist-info/RECORD
+Filename: Signix-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## info/Signix.py

```diff
@@ -6,19 +6,14 @@
 def check_email(email):
     pattern = r'^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$'
     if re.match(pattern, email):
         return True
     else:
         return False
 
-def check_phone_number(phone_number):
-    pattern = r'(\d{3})(\d{3})(\d{4})'
-    formatted_number = re.sub(pattern, '\1-\2-\3', phone_number)
-    return formatted_number
-
 def check_name(name):
     if not name:
         return False
     if len(name) <= 8:
         if all(char in string.ascii_letters or char in string.whitespace for char in name):
             return True
     return False
@@ -48,20 +43,19 @@
 
 def check_input(email, name, user_id, password, phone_number):
     return (check_email(email) and
             check_name(name) and
             check_id(user_id) and
             check_pwd(password))
 
-def add_user_info(df, email, name, user_id, password, phone_number):
-    if check_email(email) and check_name(name) and check_id(user_id) and check_pwd(password):
+def add_user_info(df, email, name, user_id, password):
+    if check_email(email) and check_name(name) and check_id(user_id):
         df = pd.concat([df, pd.DataFrame({
             'name': [name],
             'email': [email],
-            'phone_number': [phone_number],
             'id': [user_id],
             'password': [password],
         })], ignore_index=True)
         return df
 
 def check_info(email, name, user_id, password):
     i=0
```


# Comparing `tmp/drf_easily_auth-0.1.1.tar.gz` & `tmp/drf_easily_auth-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_easily_auth-0.1.1.tar", max compression
+gzip compressed data, was "drf_easily_auth-0.1.2.tar", max compression
```

## Comparing `drf_easily_auth-0.1.1.tar` & `drf_easily_auth-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1253 2024-04-20 22:47:35.567294 drf_easily_auth-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-20 16:52:04.771826 drf_easily_auth-0.1.1/drf_easily_auth/__init__.py
--rw-r--r--   0        0        0       99 2024-04-20 20:52:30.739037 drf_easily_auth-0.1.1/drf_easily_auth/admin.py
--rw-r--r--   0        0        0      672 2024-04-20 22:47:24.535044 drf_easily_auth-0.1.1/drf_easily_auth/apps.py
--rw-r--r--   0        0        0     2032 2024-04-20 20:51:36.406448 drf_easily_auth-0.1.1/drf_easily_auth/firebase.py
--rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.1/drf_easily_auth/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.1/drf_easily_auth/management/commands/__init__.py
--rw-r--r--   0        0        0     1564 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.1/drf_easily_auth/management/commands/syncfirebaseusers.py
--rw-r--r--   0        0        0      957 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.1/drf_easily_auth/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.1/drf_easily_auth/migrations/__init__.py
--rw-r--r--   0        0        0      473 2024-04-20 20:52:32.875060 drf_easily_auth-0.1.1/drf_easily_auth/models.py
--rw-r--r--   0        0        0       63 2024-04-20 20:51:36.418448 drf_easily_auth-0.1.1/drf_easily_auth/tests.py
--rw-r--r--   0        0        0      674 2024-04-20 22:59:32.272198 drf_easily_auth-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 drf_easily_auth-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1351 2024-04-21 07:13:07.732940 drf_easily_auth-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-20 16:52:04.771826 drf_easily_auth-0.1.2/drf_easily_auth/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-20 20:52:30.739037 drf_easily_auth-0.1.2/drf_easily_auth/admin.py
+-rw-r--r--   0        0        0      672 2024-04-20 22:47:24.535044 drf_easily_auth-0.1.2/drf_easily_auth/apps.py
+-rw-r--r--   0        0        0     1981 2024-04-21 07:03:41.564184 drf_easily_auth-0.1.2/drf_easily_auth/firebase.py
+-rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.2/drf_easily_auth/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.2/drf_easily_auth/management/commands/__init__.py
+-rw-r--r--   0        0        0     1881 2024-04-21 07:03:47.860231 drf_easily_auth-0.1.2/drf_easily_auth/management/commands/syncfirebaseusers.py
+-rw-r--r--   0        0        0      957 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.2/drf_easily_auth/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.2/drf_easily_auth/migrations/__init__.py
+-rw-r--r--   0        0        0      473 2024-04-20 20:52:32.875060 drf_easily_auth-0.1.2/drf_easily_auth/models.py
+-rw-r--r--   0        0        0       63 2024-04-20 20:51:36.418448 drf_easily_auth-0.1.2/drf_easily_auth/tests.py
+-rw-r--r--   0        0        0      915 2024-04-21 07:17:40.129448 drf_easily_auth-0.1.2/drf_easily_auth/utils.py
+-rw-r--r--   0        0        0      366 2024-04-21 07:20:00.404874 drf_easily_auth-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1901 1970-01-01 00:00:00.000000 drf_easily_auth-0.1.2/PKG-INFO
```

### Comparing `drf_easily_auth-0.1.1/drf_easily_auth/apps.py` & `drf_easily_auth-0.1.2/drf_easily_auth/apps.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.1/drf_easily_auth/firebase.py` & `drf_easily_auth-0.1.2/drf_easily_auth/firebase.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,28 @@
         token = auth_header.split(' ').pop()
         try:
             decoded_token = auth.verify_id_token(token, check_revoked=True)
 
             # Extract user data
             uid = decoded_token['uid']
             aud = decoded_token['aud']
-            user_id = decoded_token['user_id']
             email = decoded_token['email']
             email_verified = decoded_token['email_verified']
             provider = decoded_token['firebase']['sign_in_provider']
 
         except auth.InvalidIdTokenError:
             raise exceptions.AuthenticationFailed('Invalid authentication token.')
         except auth.ExpiredIdTokenError:
             raise exceptions.AuthenticationFailed('Expired authentication token.')
         except auth.RevokedIdTokenError:
             raise exceptions.AuthenticationFailed('Revoked authentication token.')
         except Exception as e:
             raise exceptions.AuthenticationFailed(f'Authentication failed: {str(e)}')
 
-        user, created = User.objects.get_or_create(username=user_id, email=email)
+        user, created = User.objects.get_or_create(username=uid, email=email)
         if created:
             # Disable user password
             user.set_unusable_password()
             user.save()
 
             # Firebase user informations (aud, email_verified, sign_in_provider)
             firebase_user = Firebase.objects.create(
```

### Comparing `drf_easily_auth-0.1.1/drf_easily_auth/management/commands/syncfirebaseusers.py` & `drf_easily_auth-0.1.2/drf_easily_auth/management/commands/syncfirebaseusers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 from django.core.management.base import BaseCommand
 from firebase_admin import auth
 from django.contrib.auth.models import User
-from authentication.models import Firebase  
+from drf_easily_auth.models import Firebase  
 
 class Command(BaseCommand):
     """
     Command to synchronise users from Firebase
     
     Usage:
         python3 manage.py syncfirebaseusers
     """
     help = 'Users synchronisation from Firebase'
 
     def handle(self, *args, **options):
         header_message = """
-        ########################################################
-        #                                                      #
-        #           Firebase User Synchronisation              #
-        #                                                      #
-        ########################################################
+########################################################
+#                                                      #
+#           Firebase User Synchronisation              #
+#                                                      #
+########################################################
         """
+        separator = "-" * 50
         self.stdout.write(self.style.SUCCESS(header_message))
         firebase_users = auth.list_users().iterate_all()
 
         for firebase_user in firebase_users:
-            user, created = User.objects.get_or_create(username=firebase_user.uid, email=firebase_user.email)
+            if not firebase_user.email:
+                user, created = User.objects.get_or_create(username=firebase_user.uid)
+            else:
+                user, created = User.objects.get_or_create(username=firebase_user.uid, email=firebase_user.email)
+
             if created:
                 user.set_unusable_password()
                 user.save()
 
                 Firebase.objects.create(
                     user=user,
                     email_verified=firebase_user.email_verified,
                     sign_in_provider=firebase_user.provider_id
                 )
                 self.stdout.write(self.style.SUCCESS(f'User sync > ID: {user.username} > Email: {user.email}'))
-        self.stdout.write(self.style.SUCCESS('Users synchronisation completed'))
+        self.stdout.write(self.style.SUCCESS('Users synchronisation completed'))
+
+        user_count = User.objects.count()
+
+        self.stdout.write(self.style.SUCCESS(separator))
+        self.stdout.write(self.style.SUCCESS(f'Users count: {user_count}'))
```

### Comparing `drf_easily_auth-0.1.1/drf_easily_auth/migrations/0001_initial.py` & `drf_easily_auth-0.1.2/drf_easily_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.1/PKG-INFO` & `drf_easily_auth-0.1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,73 @@
 Metadata-Version: 2.1
 Name: drf-easily-auth
-Version: 0.1.1
-Summary: Votre description ici
-Home-page: https://github.com/alexandre-meline/drf_easily_auth
-Keywords: django,rest-framework,firebase,authentication
+Version: 0.1.2
+Summary: 
 Author: Alexandre Meline
 Author-email: alexandre.meline.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: django (>=5.0.4,<6.0.0)
 Requires-Dist: djangorestframework (>=3.15.1,<4.0.0)
 Requires-Dist: firebase-admin (>=6.5.0,<7.0.0)
-Project-URL: Documentation, https://github.com/alexandre-meline/drf_easily_auth
-Project-URL: Repository, https://github.com/alexandre-meline/drf_easily_auth
 Description-Content-Type: text/markdown
 
 # DRF Firebase Auth
 
-Ce package permet une integration avec Firebase lors de l'authentification hors du contexte Django.
+This package allows integration with Firebase for authentication outside the Django context.
 
-## 1. Firebase configuration
+![Firebase Logo](https://miro.medium.com/max/300/1*R4c8lHBHuH5qyqOtZb3h-w.png)
 
-Créer votre base de donnée [Firebase](https://console.firebase.google.com/), puis télécharger le fichier d'authentification `.json` lié à votre projet.
+## 1. Firebase configuration
 
-- Rendez vous dans les `Paramètres de votre projet`
-- Puis dans la section `Comptes de service`
-- Selectionner `Python` puis télécharger en cliquant sur `Générer une nouvelle clé privée`
-- Charger le fichier `.json` dans votre projet Django
+Create your [Firebase](https://console.firebase.google.com/) database, then download the `.json` authentication file linked to your project.
 
+- Go to `Project settings`
+- Then go to the `Service accounts` section
+- Select `Python` then download by clicking on `Generate new private key`
+- Upload the `.json` file into your Django project
 
 ## 2. Django configuration
 
-**Install authentication app in project**
+**Install authentication app in your project**
+
+```bash
+pip install drf-easily-auth
+```
 
 ```bash
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
 
     # Insert this app
     'drf_easily_auth',
 ]
 
-FIREBASE_CONFIG_FILE = # Your Firebase config file path download in step 1
+FIREBASE_CONFIG_FILE = # Your Firebase config file path downloaded in step 1
 ```
 
-**Configuration custom Firebase authentication in rest framework**
+**Configure custom Firebase authentication in rest framework**
 
 ```bash
 'DEFAULT_AUTHENTICATION_CLASSES': [
     'drf_easily_auth.firebase.FirebaseAuthentication',
 ],
 ```
 
 **Sync all existing users from your Firebase database**
 
 ```bash
 python3 manage.py syncfirebaseusers
 ```
+
+---
+
+Have fun with Firebase Authentication! 🚀
+
```


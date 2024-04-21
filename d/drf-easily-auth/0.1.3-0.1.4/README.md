# Comparing `tmp/drf_easily_auth-0.1.3.tar.gz` & `tmp/drf_easily_auth-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_easily_auth-0.1.3.tar", max compression
+gzip compressed data, was "drf_easily_auth-0.1.4.tar", max compression
```

## Comparing `drf_easily_auth-0.1.3.tar` & `drf_easily_auth-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1351 2024-04-21 07:13:07.732940 drf_easily_auth-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-20 16:52:04.771826 drf_easily_auth-0.1.3/drf_easily_auth/__init__.py
--rw-r--r--   0        0        0       99 2024-04-20 20:52:30.739037 drf_easily_auth-0.1.3/drf_easily_auth/admin.py
--rw-r--r--   0        0        0      672 2024-04-20 22:47:24.535044 drf_easily_auth-0.1.3/drf_easily_auth/apps.py
--rw-r--r--   0        0        0     1981 2024-04-21 07:03:41.564184 drf_easily_auth-0.1.3/drf_easily_auth/firebase.py
--rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.3/drf_easily_auth/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.3/drf_easily_auth/management/commands/__init__.py
--rw-r--r--   0        0        0     1881 2024-04-21 07:03:47.860231 drf_easily_auth-0.1.3/drf_easily_auth/management/commands/syncfirebaseusers.py
--rw-r--r--   0        0        0      957 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.3/drf_easily_auth/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.3/drf_easily_auth/migrations/__init__.py
--rw-r--r--   0        0        0      473 2024-04-20 20:52:32.875060 drf_easily_auth-0.1.3/drf_easily_auth/models.py
--rw-r--r--   0        0        0       63 2024-04-20 20:51:36.418448 drf_easily_auth-0.1.3/drf_easily_auth/tests.py
--rw-r--r--   0        0        0      915 2024-04-21 07:17:40.129448 drf_easily_auth-0.1.3/drf_easily_auth/utils.py
--rw-r--r--   0        0        0      560 2024-04-21 07:22:21.747872 drf_easily_auth-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2019 1970-01-01 00:00:00.000000 drf_easily_auth-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1351 2024-04-21 07:13:07.732940 drf_easily_auth-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-20 16:52:04.771826 drf_easily_auth-0.1.4/drf_easily_auth/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-20 20:52:30.739037 drf_easily_auth-0.1.4/drf_easily_auth/admin.py
+-rw-r--r--   0        0        0      672 2024-04-20 22:47:24.535044 drf_easily_auth-0.1.4/drf_easily_auth/apps.py
+-rw-r--r--   0        0        0     1981 2024-04-21 07:03:41.564184 drf_easily_auth-0.1.4/drf_easily_auth/firebase.py
+-rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.4/drf_easily_auth/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.4/drf_easily_auth/management/commands/__init__.py
+-rw-r--r--   0        0        0     1881 2024-04-21 07:03:47.860231 drf_easily_auth-0.1.4/drf_easily_auth/management/commands/syncfirebaseusers.py
+-rw-r--r--   0        0        0      957 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.4/drf_easily_auth/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.4/drf_easily_auth/migrations/__init__.py
+-rw-r--r--   0        0        0      473 2024-04-20 20:52:32.875060 drf_easily_auth-0.1.4/drf_easily_auth/models.py
+-rw-r--r--   0        0        0       63 2024-04-20 20:51:36.418448 drf_easily_auth-0.1.4/drf_easily_auth/tests.py
+-rw-r--r--   0        0        0      915 2024-04-21 07:17:40.129448 drf_easily_auth-0.1.4/drf_easily_auth/utils.py
+-rw-r--r--   0        0        0      624 2024-04-21 07:24:06.733870 drf_easily_auth-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 drf_easily_auth-0.1.4/PKG-INFO
```

### Comparing `drf_easily_auth-0.1.3/README.md` & `drf_easily_auth-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.3/drf_easily_auth/apps.py` & `drf_easily_auth-0.1.4/drf_easily_auth/apps.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.3/drf_easily_auth/firebase.py` & `drf_easily_auth-0.1.4/drf_easily_auth/firebase.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.3/drf_easily_auth/management/commands/syncfirebaseusers.py` & `drf_easily_auth-0.1.4/drf_easily_auth/management/commands/syncfirebaseusers.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.3/drf_easily_auth/migrations/0001_initial.py` & `drf_easily_auth-0.1.4/drf_easily_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.3/drf_easily_auth/utils.py` & `drf_easily_auth-0.1.4/drf_easily_auth/utils.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.3/pyproject.toml` & `drf_easily_auth-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-easily-auth"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Alexandre Meline <alexandre.meline.dev@gmail.com>"]
 readme = "README.md"
 keywords = [
     "Django",
     "Firebase",
     "Authentication",
@@ -12,14 +12,15 @@
     "DRF", 
     "Python",
     "User Management",
     "Security",
     "API",
     "JSON Web Tokens",
 ]
+homepage="https://github.com/alexandre-meline/drf_easily_auth/"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 django = "^5.0.4"
 djangorestframework = "^3.15.1"
 firebase-admin = "^6.5.0"
```

### Comparing `drf_easily_auth-0.1.3/PKG-INFO` & `drf_easily_auth-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: drf-easily-auth
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
+Home-page: https://github.com/alexandre-meline/drf_easily_auth/
 Keywords: Django,Firebase,Authentication,User Synchronization,DRF,Python,User Management,Security,API,JSON Web Tokens
 Author: Alexandre Meline
 Author-email: alexandre.meline.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


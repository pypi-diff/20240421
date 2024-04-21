# Comparing `tmp/drf_easily_auth-0.1.6.tar.gz` & `tmp/drf_easily_auth-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_easily_auth-0.1.6.tar", max compression
+gzip compressed data, was "drf_easily_auth-0.1.7.tar", max compression
```

## Comparing `drf_easily_auth-0.1.6.tar` & `drf_easily_auth-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1351 2024-04-21 07:13:07.732940 drf_easily_auth-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-04-20 16:52:04.771826 drf_easily_auth-0.1.6/drf_easily_auth/__init__.py
--rw-r--r--   0        0        0       99 2024-04-20 20:52:30.739037 drf_easily_auth-0.1.6/drf_easily_auth/admin.py
--rw-r--r--   0        0        0      672 2024-04-20 22:47:24.535044 drf_easily_auth-0.1.6/drf_easily_auth/apps.py
--rw-r--r--   0        0        0     1981 2024-04-21 07:03:41.564184 drf_easily_auth-0.1.6/drf_easily_auth/firebase.py
--rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.6/drf_easily_auth/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.6/drf_easily_auth/management/commands/__init__.py
--rw-r--r--   0        0        0     1881 2024-04-21 07:03:47.860231 drf_easily_auth-0.1.6/drf_easily_auth/management/commands/syncfirebaseusers.py
--rw-r--r--   0        0        0      957 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.6/drf_easily_auth/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.6/drf_easily_auth/migrations/__init__.py
--rw-r--r--   0        0        0      473 2024-04-20 20:52:32.875060 drf_easily_auth-0.1.6/drf_easily_auth/models.py
--rw-r--r--   0        0        0       63 2024-04-20 20:51:36.418448 drf_easily_auth-0.1.6/drf_easily_auth/tests.py
--rw-r--r--   0        0        0      915 2024-04-21 07:17:40.129448 drf_easily_auth-0.1.6/drf_easily_auth/utils.py
--rw-r--r--   0        0        0      716 2024-04-21 07:42:24.509260 drf_easily_auth-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2175 1970-01-01 00:00:00.000000 drf_easily_auth-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1351 2024-04-21 07:13:07.732940 drf_easily_auth-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-20 16:52:04.771826 drf_easily_auth-0.1.7/drf_easily_auth/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-20 20:52:30.739037 drf_easily_auth-0.1.7/drf_easily_auth/admin.py
+-rw-r--r--   0        0        0      876 2024-04-21 12:38:05.789001 drf_easily_auth-0.1.7/drf_easily_auth/apps.py
+-rw-r--r--   0        0        0     1981 2024-04-21 07:03:41.564184 drf_easily_auth-0.1.7/drf_easily_auth/firebase.py
+-rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.7/drf_easily_auth/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.7/drf_easily_auth/management/commands/__init__.py
+-rw-r--r--   0        0        0     1881 2024-04-21 07:03:47.860231 drf_easily_auth-0.1.7/drf_easily_auth/management/commands/syncfirebaseusers.py
+-rw-r--r--   0        0        0      957 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.7/drf_easily_auth/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.7/drf_easily_auth/migrations/__init__.py
+-rw-r--r--   0        0        0      473 2024-04-20 20:52:32.875060 drf_easily_auth-0.1.7/drf_easily_auth/models.py
+-rw-r--r--   0        0        0       63 2024-04-20 20:51:36.418448 drf_easily_auth-0.1.7/drf_easily_auth/tests.py
+-rw-r--r--   0        0        0      915 2024-04-21 07:17:40.129448 drf_easily_auth-0.1.7/drf_easily_auth/utils.py
+-rw-r--r--   0        0        0      716 2024-04-21 12:40:02.345862 drf_easily_auth-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2175 1970-01-01 00:00:00.000000 drf_easily_auth-0.1.7/PKG-INFO
```

### Comparing `drf_easily_auth-0.1.6/README.md` & `drf_easily_auth-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.6/drf_easily_auth/firebase.py` & `drf_easily_auth-0.1.7/drf_easily_auth/firebase.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.6/drf_easily_auth/management/commands/syncfirebaseusers.py` & `drf_easily_auth-0.1.7/drf_easily_auth/management/commands/syncfirebaseusers.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.6/drf_easily_auth/migrations/0001_initial.py` & `drf_easily_auth-0.1.7/drf_easily_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.6/drf_easily_auth/utils.py` & `drf_easily_auth-0.1.7/drf_easily_auth/utils.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.6/pyproject.toml` & `drf_easily_auth-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-easily-auth"
-version = "0.1.6"
+version = "0.1.7"
 description = "This package allows integration with Firebase for authentication outside the Django context."
 authors = ["Alexandre Meline <alexandre.meline.dev@gmail.com>"]
 readme = "README.md"
 keywords = [
     "Django",
     "Firebase",
     "Authentication",
```

### Comparing `drf_easily_auth-0.1.6/PKG-INFO` & `drf_easily_auth-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-easily-auth
-Version: 0.1.6
+Version: 0.1.7
 Summary: This package allows integration with Firebase for authentication outside the Django context.
 Home-page: https://github.com/alexandre-meline/drf_easily_auth/
 Keywords: Django,Firebase,Authentication,User Synchronization,DRF,Python,User Management,Security,API,JSON Web Tokens
 Author: Alexandre Meline
 Author-email: alexandre.meline.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```


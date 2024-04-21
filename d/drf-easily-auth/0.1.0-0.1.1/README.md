# Comparing `tmp/drf_easily_auth-0.1.0.tar.gz` & `tmp/drf_easily_auth-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_easily_auth-0.1.0.tar", max compression
+gzip compressed data, was "drf_easily_auth-0.1.1.tar", max compression
```

## Comparing `drf_easily_auth-0.1.0.tar` & `drf_easily_auth-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,14 @@
--rw-r--r--   0        0        0     1253 2024-04-20 22:47:35.567294 drf_easily_auth-0.1.0/README.md
--rw-r--r--   0        0        0       23 2024-04-20 22:31:30.743195 drf_easily_auth-0.1.0/drf_easily_auth/.git/HEAD
--rw-r--r--   0        0        0       92 2024-04-20 22:31:30.747195 drf_easily_auth-0.1.0/drf_easily_auth/.git/config
--rw-r--r--   0        0        0       73 2024-04-20 22:31:30.743195 drf_easily_auth-0.1.0/drf_easily_auth/.git/description
--rwxr-xr-x   0        0        0      478 2024-04-20 22:31:30.743195 drf_easily_auth-0.1.0/drf_easily_auth/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0        0        0      896 2024-04-20 22:31:30.743195 drf_easily_auth-0.1.0/drf_easily_auth/.git/hooks/commit-msg.sample
--rwxr-xr-x   0        0        0     4655 2024-04-20 22:31:30.743195 drf_easily_auth-0.1.0/drf_easily_auth/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0        0        0      189 2024-04-20 22:31:30.743195 drf_easily_auth-0.1.0/drf_easily_auth/.git/hooks/post-update.sample
--rwxr-xr-x   0        0        0      424 2024-04-20 22:31:30.743195 drf_easily_auth-0.1.0/drf_easily_auth/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0        0        0     1643 2024-04-20 22:31:30.743195 drf_easily_auth-0.1.0/drf_easily_auth/.git/hooks/pre-commit.sample
--rwxr-xr-x   0        0        0      416 2024-04-20 22:31:30.743195 drf_easily_auth-0.1.0/drf_easily_auth/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0        0        0     1374 2024-04-20 22:31:30.743195 drf_easily_auth-0.1.0/drf_easily_auth/.git/hooks/pre-push.sample
--rwxr-xr-x   0        0        0     4898 2024-04-20 22:31:30.743195 drf_easily_auth-0.1.0/drf_easily_auth/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0        0        0      544 2024-04-20 22:31:30.743195 drf_easily_auth-0.1.0/drf_easily_auth/.git/hooks/pre-receive.sample
--rwxr-xr-x   0        0        0     1492 2024-04-20 22:31:30.743195 drf_easily_auth-0.1.0/drf_easily_auth/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0        0        0     2783 2024-04-20 22:31:30.743195 drf_easily_auth-0.1.0/drf_easily_auth/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0        0        0     3650 2024-04-20 22:31:30.743195 drf_easily_auth-0.1.0/drf_easily_auth/.git/hooks/update.sample
--rw-r--r--   0        0        0      240 2024-04-20 22:31:30.743195 drf_easily_auth-0.1.0/drf_easily_auth/.git/info/exclude
--rw-r--r--   0        0        0        0 2024-04-20 16:52:04.771826 drf_easily_auth-0.1.0/drf_easily_auth/__init__.py
--rw-r--r--   0        0        0       99 2024-04-20 20:52:30.739037 drf_easily_auth-0.1.0/drf_easily_auth/admin.py
--rw-r--r--   0        0        0      672 2024-04-20 22:47:24.535044 drf_easily_auth-0.1.0/drf_easily_auth/apps.py
--rw-r--r--   0        0        0     2032 2024-04-20 20:51:36.406448 drf_easily_auth-0.1.0/drf_easily_auth/firebase.py
--rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.0/drf_easily_auth/management/__init__.py
--rw-r--r--   0        0        0      182 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.0/drf_easily_auth/management/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.0/drf_easily_auth/management/commands/__init__.py
--rw-r--r--   0        0        0      191 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.0/drf_easily_auth/management/commands/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1763 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.0/drf_easily_auth/management/commands/__pycache__/syncfirebaseusers.cpython-310.pyc
--rw-r--r--   0        0        0     1564 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.0/drf_easily_auth/management/commands/syncfirebaseusers.py
--rw-r--r--   0        0        0      957 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.0/drf_easily_auth/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.0/drf_easily_auth/migrations/__init__.py
--rw-r--r--   0        0        0     1073 2024-04-20 20:51:36.390447 drf_easily_auth-0.1.0/drf_easily_auth/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0        0        0      194 2024-04-20 20:51:36.390447 drf_easily_auth-0.1.0/drf_easily_auth/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      473 2024-04-20 20:52:32.875060 drf_easily_auth-0.1.0/drf_easily_auth/models.py
--rw-r--r--   0        0        0       63 2024-04-20 20:51:36.418448 drf_easily_auth-0.1.0/drf_easily_auth/tests.py
--rw-r--r--   0        0        0      366 2024-04-20 22:45:23.024117 drf_easily_auth-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 drf_easily_auth-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1253 2024-04-20 22:47:35.567294 drf_easily_auth-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-20 16:52:04.771826 drf_easily_auth-0.1.1/drf_easily_auth/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-20 20:52:30.739037 drf_easily_auth-0.1.1/drf_easily_auth/admin.py
+-rw-r--r--   0        0        0      672 2024-04-20 22:47:24.535044 drf_easily_auth-0.1.1/drf_easily_auth/apps.py
+-rw-r--r--   0        0        0     2032 2024-04-20 20:51:36.406448 drf_easily_auth-0.1.1/drf_easily_auth/firebase.py
+-rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.1/drf_easily_auth/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.1/drf_easily_auth/management/commands/__init__.py
+-rw-r--r--   0        0        0     1564 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.1/drf_easily_auth/management/commands/syncfirebaseusers.py
+-rw-r--r--   0        0        0      957 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.1/drf_easily_auth/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.1/drf_easily_auth/migrations/__init__.py
+-rw-r--r--   0        0        0      473 2024-04-20 20:52:32.875060 drf_easily_auth-0.1.1/drf_easily_auth/models.py
+-rw-r--r--   0        0        0       63 2024-04-20 20:51:36.418448 drf_easily_auth-0.1.1/drf_easily_auth/tests.py
+-rw-r--r--   0        0        0      674 2024-04-20 22:59:32.272198 drf_easily_auth-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 drf_easily_auth-0.1.1/PKG-INFO
```

### Comparing `drf_easily_auth-0.1.0/README.md` & `drf_easily_auth-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.0/drf_easily_auth/apps.py` & `drf_easily_auth-0.1.1/drf_easily_auth/apps.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.0/drf_easily_auth/firebase.py` & `drf_easily_auth-0.1.1/drf_easily_auth/firebase.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.0/drf_easily_auth/management/commands/syncfirebaseusers.py` & `drf_easily_auth-0.1.1/drf_easily_auth/management/commands/syncfirebaseusers.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.0/drf_easily_auth/migrations/0001_initial.py` & `drf_easily_auth-0.1.1/drf_easily_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.0/PKG-INFO` & `drf_easily_auth-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: drf-easily-auth
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: Votre description ici
+Home-page: https://github.com/alexandre-meline/drf_easily_auth
+Keywords: django,rest-framework,firebase,authentication
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
+Project-URL: Documentation, https://github.com/alexandre-meline/drf_easily_auth
+Project-URL: Repository, https://github.com/alexandre-meline/drf_easily_auth
 Description-Content-Type: text/markdown
 
 # DRF Firebase Auth
 
 Ce package permet une integration avec Firebase lors de l'authentification hors du contexte Django.
 
 ## 1. Firebase configuration
```


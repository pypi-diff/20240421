# Comparing `tmp/async_firebase_rest_api-2.0.0.tar.gz` & `tmp/async_firebase_rest_api-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_firebase_rest_api-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "async_firebase_rest_api-2.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `async_firebase_rest_api-2.0.0.tar` & `async_firebase_rest_api-2.0.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0       66 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/.gitattributes
--rw-r--r--   0        0        0     2762 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      366 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1238 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/.github/ISSUE_TEMPLATE/docs.yml
--rw-r--r--   0        0        0     1698 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0      762 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/.github/ISSUE_TEMPLATE/others.yml
--rw-r--r--   0        0        0      940 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/.github/workflows/greetings.yml
--rw-r--r--   0        0        0      549 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1030 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     3150 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0     2762 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/.gitignore
--rw-r--r--   0        0        0      711 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/.readthedocs.yaml
--rw-r--r--   0        0        0     8732 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1107 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/LICENSE
--rw-r--r--   0        0        0     3248 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/README.md
--rw-r--r--   0        0        0      409 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/docs/_static/css/my-styles.css
--rw-r--r--   0        0        0     2949 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/docs/conf.py
--rw-r--r--   0        0        0      129 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/docs/firebase/firebase.auth.rst
--rw-r--r--   0        0        0      141 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/docs/firebase/firebase.database.rst
--rw-r--r--   0        0        0      144 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/docs/firebase/firebase.firestore.rst
--rw-r--r--   0        0        0       98 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/docs/firebase/firebase.rst
--rw-r--r--   0        0        0      138 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/docs/firebase/firebase.storage.rst
--rw-r--r--   0        0        0      151 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/docs/firebase/modules.rst
--rw-r--r--   0        0        0     9241 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/docs/guide/authentication.rst
--rw-r--r--   0        0        0     8518 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/docs/guide/database.rst
--rw-r--r--   0        0        0     3706 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/docs/guide/firebase-rest-api.rst
--rw-r--r--   0        0        0    10444 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/docs/guide/firestore.rst
--rw-r--r--   0        0        0     3488 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/docs/guide/setup.rst
--rw-r--r--   0        0        0     2097 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/docs/guide/storage.rst
--rw-r--r--   0        0        0     2422 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/docs/index.rst
--rw-r--r--   0        0        0       72 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/docs/requirements.txt
--rw-r--r--   0        0        0     2544 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/firebase/__init__.py
--rw-r--r--   0        0        0      392 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/firebase/_custom_requests.py
--rw-r--r--   0        0        0      581 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/firebase/_exception.py
--rw-r--r--   0        0        0     1305 2024-04-19 02:01:53.199018 async_firebase_rest_api-2.0.0/firebase/_service_account_credentials.py
--rw-r--r--   0        0        0    23933 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/firebase/auth/__init__.py
--rw-r--r--   0        0        0    19139 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/firebase/database/__init__.py
--rw-r--r--   0        0        0     1395 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/firebase/database/_custom_sse_client.py
--rw-r--r--   0        0        0     1562 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/firebase/database/_db_convert.py
--rw-r--r--   0        0        0      645 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/firebase/database/_keep_auth_session.py
--rw-r--r--   0        0        0    20108 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/firebase/firestore/__init__.py
--rw-r--r--   0        0        0     5206 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/firebase/firestore/_utils.py
--rw-r--r--   0        0        0     7816 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/firebase/storage/__init__.py
--rw-r--r--   0        0        0     1747 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      205 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/requirements.txt
--rw-r--r--   0        0        0      219 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1944 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/tests/config.py
--rw-r--r--   0        0        0      678 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/tests/config.template.py
--rw-r--r--   0        0        0     1941 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0      164 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/tests/requirements.txt
--rw-r--r--   0        0        0     3686 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/tests/static/test-file.txt
--rw-r--r--   0        0        0     9278 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/tests/test_auth.py
--rw-r--r--   0        0        0     4618 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/tests/test_database.py
--rw-r--r--   0        0        0    21335 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/tests/test_firestore.py
--rw-r--r--   0        0        0     1028 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/tests/test_setup.py
--rw-r--r--   0        0        0     2561 2024-04-19 02:01:53.203018 async_firebase_rest_api-2.0.0/tests/test_storage.py
--rw-r--r--   0        0        0     5102 1970-01-01 00:00:00.000000 async_firebase_rest_api-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.gitattributes
+-rw-r--r--   0        0        0     2762 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      366 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1238 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/docs.yml
+-rw-r--r--   0        0        0     1698 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0      762 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/others.yml
+-rw-r--r--   0        0        0      940 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/workflows/greetings.yml
+-rw-r--r--   0        0        0      549 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1030 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     3150 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     2762 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.gitignore
+-rw-r--r--   0        0        0      711 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     9127 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1107 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/LICENSE
+-rw-r--r--   0        0        0     3254 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/README.md
+-rw-r--r--   0        0        0      409 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/docs/_static/css/my-styles.css
+-rw-r--r--   0        0        0     2949 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/docs/conf.py
+-rw-r--r--   0        0        0      129 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/docs/firebase/firebase.auth.rst
+-rw-r--r--   0        0        0      141 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/docs/firebase/firebase.database.rst
+-rw-r--r--   0        0        0      144 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/docs/firebase/firebase.firestore.rst
+-rw-r--r--   0        0        0       98 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/docs/firebase/firebase.rst
+-rw-r--r--   0        0        0      138 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/docs/firebase/firebase.storage.rst
+-rw-r--r--   0        0        0      151 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/docs/firebase/modules.rst
+-rw-r--r--   0        0        0     9241 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/docs/guide/authentication.rst
+-rw-r--r--   0        0        0     8518 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/docs/guide/database.rst
+-rw-r--r--   0        0        0     3706 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/docs/guide/firebase-rest-api.rst
+-rw-r--r--   0        0        0    10444 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/docs/guide/firestore.rst
+-rw-r--r--   0        0        0     3488 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/docs/guide/setup.rst
+-rw-r--r--   0        0        0     2097 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/docs/guide/storage.rst
+-rw-r--r--   0        0        0     2422 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/docs/index.rst
+-rw-r--r--   0        0        0       72 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/docs/requirements.txt
+-rw-r--r--   0        0        0     2544 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/__init__.py
+-rw-r--r--   0        0        0      392 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/_custom_requests.py
+-rw-r--r--   0        0        0      581 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/_exception.py
+-rw-r--r--   0        0        0     1305 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/_service_account_credentials.py
+-rw-r--r--   0        0        0    23957 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/auth/__init__.py
+-rw-r--r--   0        0        0    19139 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/database/__init__.py
+-rw-r--r--   0        0        0     1395 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/database/_custom_sse_client.py
+-rw-r--r--   0        0        0     1562 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/database/_db_convert.py
+-rw-r--r--   0        0        0      645 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/database/_keep_auth_session.py
+-rw-r--r--   0        0        0    20108 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/firestore/__init__.py
+-rw-r--r--   0        0        0     5206 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/firestore/_utils.py
+-rw-r--r--   0        0        0     7816 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/storage/__init__.py
+-rw-r--r--   0        0        0     1747 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      205 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/requirements.txt
+-rw-r--r--   0        0        0      219 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     1944 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/config.py
+-rw-r--r--   0        0        0      678 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/config.template.py
+-rw-r--r--   0        0        0     1941 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/conftest.py
+-rw-r--r--   0        0        0      164 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/requirements.txt
+-rw-r--r--   0        0        0     3686 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/static/test-file.txt
+-rw-r--r--   0        0        0     9278 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/test_auth.py
+-rw-r--r--   0        0        0     4618 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/test_database.py
+-rw-r--r--   0        0        0    21335 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/test_firestore.py
+-rw-r--r--   0        0        0     1028 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/test_setup.py
+-rw-r--r--   0        0        0     2561 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/test_storage.py
+-rw-r--r--   0        0        0     5108 1970-01-01 00:00:00.000000 async_firebase_rest_api-2.0.1/PKG-INFO
```

### Comparing `async_firebase_rest_api-2.0.0/.github/ISSUE_TEMPLATE/bug-report.yml` & `async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/.github/ISSUE_TEMPLATE/docs.yml` & `async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/docs.yml`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/.github/ISSUE_TEMPLATE/feature-request.yml` & `async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/.github/ISSUE_TEMPLATE/others.yml` & `async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/others.yml`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/.github/workflows/greetings.yml` & `async_firebase_rest_api-2.0.1/.github/workflows/greetings.yml`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/.github/workflows/publish.yml` & `async_firebase_rest_api-2.0.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/.github/workflows/release.yml` & `async_firebase_rest_api-2.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/.github/workflows/tests.yml` & `async_firebase_rest_api-2.0.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/.gitignore` & `async_firebase_rest_api-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/.readthedocs.yaml` & `async_firebase_rest_api-2.0.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/CHANGELOG.md` & `async_firebase_rest_api-2.0.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+## [2.0.1](https://github.com/matiaskotlik/async-firebase-rest-api/compare/v2.0.0...v2.0.1) (2024-04-20)
+
+
+### Bug Fixes
+
+* fix google and fb signin ([0d62775](https://github.com/matiaskotlik/async-firebase-rest-api/commit/0d627751bd477d7ee0f1ccd968763b051d39d2c0))
+* readme ([becbf9c](https://github.com/matiaskotlik/async-firebase-rest-api/commit/becbf9ce0256f254d742aebabb1693fe17058ca9))
+
+
+
 # [2.0.0](https://github.com/matiaskotlik/async-firebase-rest-api/compare/v1.11.0...v2.0.0) (2024-04-19)
 
 
 ### Bug Fixes
 
 * gha and readme ([071950a](https://github.com/matiaskotlik/async-firebase-rest-api/commit/071950a35038c6a4d3b30ffaaa49e5db40f6a1ed))
```

### Comparing `async_firebase_rest_api-2.0.0/LICENSE` & `async_firebase_rest_api-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/README.md` & `async_firebase_rest_api-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
 # Firebase Realtime Database
 db = app.database()
 
 # Data to save in database
 data = {
    "name": "Robert Downey Jr.",
-   "email": user.get('email')
+   "email": await user.get('email')
 }
 
 # Store data to Firebase Database
 await db.child("users").push(data, user.get('idToken'))
 
 
 # Firebase Storage
```

#### html2text {}

```diff
@@ -15,13 +15,13 @@
 databaseName.firebaseio.com", "projectId": "projectId", "storageBucket":
 "projectId.appspot.com", "messagingSenderId": "messagingSenderId", "appId":
 "appId" } # Instantiates a Firebase app app = firebase.initialize_app(config) #
 Firebase Authentication auth = app.auth() # Create new user and sign in await
 auth.create_user_with_email_and_password(email, password) user = await
 auth.sign_in_with_email_and_password(email, password) # Firebase Realtime
 Database db = app.database() # Data to save in database data = { "name":
-"Robert Downey Jr.", "email": user.get('email') } # Store data to Firebase
-Database await db.child("users").push(data, user.get('idToken')) # Firebase
-Storage storage = app.storage() # File to store in storage file_path = 'static/
-img/example.png' # Store file to Firebase Storage await storage.child(user.get
-('localId')).child('uploaded-picture.png').put(file_path, user.get('idToken'))
-```
+"Robert Downey Jr.", "email": await user.get('email') } # Store data to
+Firebase Database await db.child("users").push(data, user.get('idToken')) #
+Firebase Storage storage = app.storage() # File to store in storage file_path =
+'static/img/example.png' # Store file to Firebase Storage await storage.child
+(user.get('localId')).child('uploaded-picture.png').put(file_path, user.get
+('idToken')) ```
```

### Comparing `async_firebase_rest_api-2.0.0/docs/conf.py` & `async_firebase_rest_api-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/docs/guide/authentication.rst` & `async_firebase_rest_api-2.0.1/docs/guide/authentication.rst`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/docs/guide/database.rst` & `async_firebase_rest_api-2.0.1/docs/guide/database.rst`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/docs/guide/firebase-rest-api.rst` & `async_firebase_rest_api-2.0.1/docs/guide/firebase-rest-api.rst`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/docs/guide/firestore.rst` & `async_firebase_rest_api-2.0.1/docs/guide/firestore.rst`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/docs/guide/setup.rst` & `async_firebase_rest_api-2.0.1/docs/guide/setup.rst`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/docs/guide/storage.rst` & `async_firebase_rest_api-2.0.1/docs/guide/storage.rst`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/docs/index.rst` & `async_firebase_rest_api-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/firebase/__init__.py` & `async_firebase_rest_api-2.0.1/firebase/__init__.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/firebase/_exception.py` & `async_firebase_rest_api-2.0.1/firebase/_exception.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/firebase/_service_account_credentials.py` & `async_firebase_rest_api-2.0.1/firebase/_service_account_credentials.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/firebase/auth/__init__.py` & `async_firebase_rest_api-2.0.1/firebase/auth/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,31 +56,31 @@
 		self.session_id = None
 		self.__code_verifier = None
 		self.__nonce = None
 
 		if client_secret:
 			self.client_secret = _load_client_secret(client_secret)
 
-	def authenticate_login_with_google(self):
+	async def authenticate_login_with_google(self):
 		""" Redirect the user to Google's OAuth 2.0 server to initiate 
 		the authentication and authorization process.
 
 		:return: Google Sign In URL
 		:rtype: str
 		"""
-		return self.create_authentication_uri('google.com')
+		return await self.create_authentication_uri('google.com')
 
-	def authenticate_login_with_facebook(self):
+	async def authenticate_login_with_facebook(self):
 		""" Redirect the user to Facebook's OAuth 2.0 server to
 		initiate the authentication and authorization process.
 
 		:return: Facebook Sign In URL
 		:rtype: str
 		"""
-		return self.create_authentication_uri('facebook.com')
+		return await self.create_authentication_uri('facebook.com')
 
 	async def create_authentication_uri(self, provider_id):
 		""" Creates an authentication URI for the given social
 		provider.
 
 		| For more details:
 		| |section-fetch-providers-for-email|_
```

### Comparing `async_firebase_rest_api-2.0.0/firebase/database/__init__.py` & `async_firebase_rest_api-2.0.1/firebase/database/__init__.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/firebase/database/_custom_sse_client.py` & `async_firebase_rest_api-2.0.1/firebase/database/_custom_sse_client.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/firebase/database/_db_convert.py` & `async_firebase_rest_api-2.0.1/firebase/database/_db_convert.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/firebase/database/_keep_auth_session.py` & `async_firebase_rest_api-2.0.1/firebase/database/_keep_auth_session.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/firebase/firestore/__init__.py` & `async_firebase_rest_api-2.0.1/firebase/firestore/__init__.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/firebase/firestore/_utils.py` & `async_firebase_rest_api-2.0.1/firebase/firestore/_utils.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/firebase/storage/__init__.py` & `async_firebase_rest_api-2.0.1/firebase/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/pyproject.toml` & `async_firebase_rest_api-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "async-firebase-rest-api"
 authors = [
   {name = "Asif Arman Rahman", email = "asifarmanrahman@gmail.com"},
   {name = "Matias Kotlik", email = "mdkotlik@gmail.com"}
 ]
-version = "2.0.0"
+version = "2.0.1"
 readme = "README.md"
 description = "An async python wrapper for Google's Firebase REST API's."
 requires-python = ">=3.11"
 keywords = [
   "firebase",
   "firebase-auth",
   "firebase-database",
```

### Comparing `async_firebase_rest_api-2.0.0/tests/config.py` & `async_firebase_rest_api-2.0.1/tests/config.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/tests/config.template.py` & `async_firebase_rest_api-2.0.1/tests/config.template.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/tests/conftest.py` & `async_firebase_rest_api-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/tests/static/test-file.txt` & `async_firebase_rest_api-2.0.1/tests/static/test-file.txt`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/tests/test_auth.py` & `async_firebase_rest_api-2.0.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/tests/test_database.py` & `async_firebase_rest_api-2.0.1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/tests/test_firestore.py` & `async_firebase_rest_api-2.0.1/tests/test_firestore.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/tests/test_setup.py` & `async_firebase_rest_api-2.0.1/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/tests/test_storage.py` & `async_firebase_rest_api-2.0.1/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.0/PKG-INFO` & `async_firebase_rest_api-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-firebase-rest-api
-Version: 2.0.0
+Version: 2.0.1
 Summary: An async python wrapper for Google's Firebase REST API's.
 Keywords: firebase,firebase-auth,firebase-database,firebase-firestore,firebase-realtime-database,firebase-storage
 Author-email: Asif Arman Rahman <asifarmanrahman@gmail.com>, Matias Kotlik <mdkotlik@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -130,15 +130,15 @@
 
 # Firebase Realtime Database
 db = app.database()
 
 # Data to save in database
 data = {
    "name": "Robert Downey Jr.",
-   "email": user.get('email')
+   "email": await user.get('email')
 }
 
 # Store data to Firebase Database
 await db.child("users").push(data, user.get('idToken'))
 
 
 # Firebase Storage
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: async-firebase-rest-api Version: 2.0.0 Summary: An
+Metadata-Version: 2.1 Name: async-firebase-rest-api Version: 2.0.1 Summary: An
 async python wrapper for Google's Firebase REST API's. Keywords:
 firebase,firebase-auth,firebase-database,firebase-firestore,firebase-realtime-
 database,firebase-storage Author-email: Asif Arman Rahman
 gmail.com>, Matias Kotlik
 gmail.com> Requires-Python: >=3.11 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
@@ -41,13 +41,13 @@
 databaseName.firebaseio.com", "projectId": "projectId", "storageBucket":
 "projectId.appspot.com", "messagingSenderId": "messagingSenderId", "appId":
 "appId" } # Instantiates a Firebase app app = firebase.initialize_app(config) #
 Firebase Authentication auth = app.auth() # Create new user and sign in await
 auth.create_user_with_email_and_password(email, password) user = await
 auth.sign_in_with_email_and_password(email, password) # Firebase Realtime
 Database db = app.database() # Data to save in database data = { "name":
-"Robert Downey Jr.", "email": user.get('email') } # Store data to Firebase
-Database await db.child("users").push(data, user.get('idToken')) # Firebase
-Storage storage = app.storage() # File to store in storage file_path = 'static/
-img/example.png' # Store file to Firebase Storage await storage.child(user.get
-('localId')).child('uploaded-picture.png').put(file_path, user.get('idToken'))
-```
+"Robert Downey Jr.", "email": await user.get('email') } # Store data to
+Firebase Database await db.child("users").push(data, user.get('idToken')) #
+Firebase Storage storage = app.storage() # File to store in storage file_path =
+'static/img/example.png' # Store file to Firebase Storage await storage.child
+(user.get('localId')).child('uploaded-picture.png').put(file_path, user.get
+('idToken')) ```
```


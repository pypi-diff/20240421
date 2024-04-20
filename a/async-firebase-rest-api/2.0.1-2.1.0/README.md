# Comparing `tmp/async_firebase_rest_api-2.0.1.tar.gz` & `tmp/async_firebase_rest_api-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_firebase_rest_api-2.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "async_firebase_rest_api-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `async_firebase_rest_api-2.0.1.tar` & `async_firebase_rest_api-2.1.0.tar`

### file list

```diff
@@ -1,57 +1,60 @@
--rw-r--r--   0        0        0       66 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.gitattributes
--rw-r--r--   0        0        0     2762 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      366 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1238 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/docs.yml
--rw-r--r--   0        0        0     1698 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0      762 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/others.yml
--rw-r--r--   0        0        0      940 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/workflows/greetings.yml
--rw-r--r--   0        0        0      549 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1030 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     3150 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0     2762 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.gitignore
--rw-r--r--   0        0        0      711 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0     9127 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1107 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/LICENSE
--rw-r--r--   0        0        0     3254 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/README.md
--rw-r--r--   0        0        0      409 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/docs/_static/css/my-styles.css
--rw-r--r--   0        0        0     2949 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/docs/conf.py
--rw-r--r--   0        0        0      129 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/docs/firebase/firebase.auth.rst
--rw-r--r--   0        0        0      141 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/docs/firebase/firebase.database.rst
--rw-r--r--   0        0        0      144 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/docs/firebase/firebase.firestore.rst
--rw-r--r--   0        0        0       98 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/docs/firebase/firebase.rst
--rw-r--r--   0        0        0      138 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/docs/firebase/firebase.storage.rst
--rw-r--r--   0        0        0      151 2024-04-20 22:26:53.742890 async_firebase_rest_api-2.0.1/docs/firebase/modules.rst
--rw-r--r--   0        0        0     9241 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/docs/guide/authentication.rst
--rw-r--r--   0        0        0     8518 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/docs/guide/database.rst
--rw-r--r--   0        0        0     3706 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/docs/guide/firebase-rest-api.rst
--rw-r--r--   0        0        0    10444 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/docs/guide/firestore.rst
--rw-r--r--   0        0        0     3488 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/docs/guide/setup.rst
--rw-r--r--   0        0        0     2097 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/docs/guide/storage.rst
--rw-r--r--   0        0        0     2422 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/docs/index.rst
--rw-r--r--   0        0        0       72 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/docs/requirements.txt
--rw-r--r--   0        0        0     2544 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/__init__.py
--rw-r--r--   0        0        0      392 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/_custom_requests.py
--rw-r--r--   0        0        0      581 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/_exception.py
--rw-r--r--   0        0        0     1305 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/_service_account_credentials.py
--rw-r--r--   0        0        0    23957 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/auth/__init__.py
--rw-r--r--   0        0        0    19139 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/database/__init__.py
--rw-r--r--   0        0        0     1395 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/database/_custom_sse_client.py
--rw-r--r--   0        0        0     1562 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/database/_db_convert.py
--rw-r--r--   0        0        0      645 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/database/_keep_auth_session.py
--rw-r--r--   0        0        0    20108 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/firestore/__init__.py
--rw-r--r--   0        0        0     5206 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/firestore/_utils.py
--rw-r--r--   0        0        0     7816 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/firebase/storage/__init__.py
--rw-r--r--   0        0        0     1747 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      205 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/requirements.txt
--rw-r--r--   0        0        0      219 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1944 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/config.py
--rw-r--r--   0        0        0      678 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/config.template.py
--rw-r--r--   0        0        0     1941 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/conftest.py
--rw-r--r--   0        0        0      164 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/requirements.txt
--rw-r--r--   0        0        0     3686 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/static/test-file.txt
--rw-r--r--   0        0        0     9278 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/test_auth.py
--rw-r--r--   0        0        0     4618 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/test_database.py
--rw-r--r--   0        0        0    21335 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/test_firestore.py
--rw-r--r--   0        0        0     1028 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/test_setup.py
--rw-r--r--   0        0        0     2561 2024-04-20 22:26:53.746890 async_firebase_rest_api-2.0.1/tests/test_storage.py
--rw-r--r--   0        0        0     5108 1970-01-01 00:00:00.000000 async_firebase_rest_api-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-20 23:22:02.635442 async_firebase_rest_api-2.1.0/.gitattributes
+-rw-r--r--   0        0        0     2762 2024-04-20 23:22:02.635442 async_firebase_rest_api-2.1.0/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      366 2024-04-20 23:22:02.635442 async_firebase_rest_api-2.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1238 2024-04-20 23:22:02.635442 async_firebase_rest_api-2.1.0/.github/ISSUE_TEMPLATE/docs.yml
+-rw-r--r--   0        0        0     1698 2024-04-20 23:22:02.635442 async_firebase_rest_api-2.1.0/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0      762 2024-04-20 23:22:02.635442 async_firebase_rest_api-2.1.0/.github/ISSUE_TEMPLATE/others.yml
+-rw-r--r--   0        0        0      940 2024-04-20 23:22:02.635442 async_firebase_rest_api-2.1.0/.github/workflows/greetings.yml
+-rw-r--r--   0        0        0      549 2024-04-20 23:22:02.635442 async_firebase_rest_api-2.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1031 2024-04-20 23:22:02.635442 async_firebase_rest_api-2.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     3437 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     2762 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/.gitignore
+-rw-r--r--   0        0        0      711 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0    10227 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1107 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3254 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/README.md
+-rw-r--r--   0        0        0      409 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/docs/_static/css/my-styles.css
+-rw-r--r--   0        0        0     2949 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/docs/conf.py
+-rw-r--r--   0        0        0      129 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/docs/firebase/firebase.auth.rst
+-rw-r--r--   0        0        0      141 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/docs/firebase/firebase.database.rst
+-rw-r--r--   0        0        0      144 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/docs/firebase/firebase.firestore.rst
+-rw-r--r--   0        0        0       98 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/docs/firebase/firebase.rst
+-rw-r--r--   0        0        0      138 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/docs/firebase/firebase.storage.rst
+-rw-r--r--   0        0        0      151 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/docs/firebase/modules.rst
+-rw-r--r--   0        0        0     9241 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/docs/guide/authentication.rst
+-rw-r--r--   0        0        0     8518 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/docs/guide/database.rst
+-rw-r--r--   0        0        0     3706 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/docs/guide/firebase-rest-api.rst
+-rw-r--r--   0        0        0    10444 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/docs/guide/firestore.rst
+-rw-r--r--   0        0        0     3488 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/docs/guide/setup.rst
+-rw-r--r--   0        0        0     2097 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/docs/guide/storage.rst
+-rw-r--r--   0        0        0     2422 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/docs/index.rst
+-rw-r--r--   0        0        0       72 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0     2562 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/firebase/__init__.py
+-rw-r--r--   0        0        0      392 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/firebase/_custom_requests.py
+-rw-r--r--   0        0        0      581 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/firebase/_exception.py
+-rw-r--r--   0        0        0     1305 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/firebase/_service_account_credentials.py
+-rw-r--r--   0        0        0    23298 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/firebase/auth/__init__.py
+-rw-r--r--   0        0        0     1098 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/firebase/auth/oauth_flow.py
+-rw-r--r--   0        0        0    19139 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/firebase/database/__init__.py
+-rw-r--r--   0        0        0     1395 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/firebase/database/_custom_sse_client.py
+-rw-r--r--   0        0        0     1562 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/firebase/database/_db_convert.py
+-rw-r--r--   0        0        0      645 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/firebase/database/_keep_auth_session.py
+-rw-r--r--   0        0        0    20536 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/firebase/firestore/__init__.py
+-rw-r--r--   0        0        0     5206 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/firebase/firestore/_utils.py
+-rw-r--r--   0        0        0     7559 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/firebase/storage/__init__.py
+-rw-r--r--   0        0        0     1747 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      114 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/renovate.json
+-rw-r--r--   0        0        0      205 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/requirements.txt
+-rw-r--r--   0        0        0      219 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1933 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/tests/config.py
+-rw-r--r--   0        0        0      678 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/tests/config.template.py
+-rw-r--r--   0        0        0     2035 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      164 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/tests/requirements.txt
+-rw-r--r--   0        0        0     3686 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/tests/static/test-file.txt
+-rw-r--r--   0        0        0     9754 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/tests/test_auth.py
+-rw-r--r--   0        0        0     4618 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/tests/test_database.py
+-rw-r--r--   0        0        0    22865 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/tests/test_firestore.py
+-rw-r--r--   0        0        0     1028 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/tests/test_setup.py
+-rw-r--r--   0        0        0     2561 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/tests/test_storage.py
+-rw-r--r--   0        0        0      135 2024-04-20 23:22:02.639442 async_firebase_rest_api-2.1.0/tests/utils.py
+-rw-r--r--   0        0        0     5108 1970-01-01 00:00:00.000000 async_firebase_rest_api-2.1.0/PKG-INFO
```

### Comparing `async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/bug-report.yml` & `async_firebase_rest_api-2.1.0/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/docs.yml` & `async_firebase_rest_api-2.1.0/.github/ISSUE_TEMPLATE/docs.yml`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/feature-request.yml` & `async_firebase_rest_api-2.1.0/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/.github/ISSUE_TEMPLATE/others.yml` & `async_firebase_rest_api-2.1.0/.github/ISSUE_TEMPLATE/others.yml`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/.github/workflows/greetings.yml` & `async_firebase_rest_api-2.1.0/.github/workflows/greetings.yml`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/.github/workflows/publish.yml` & `async_firebase_rest_api-2.1.0/.github/workflows/publish.yml`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
     publish:
 
         runs-on: ubuntu-latest
 
         steps:
 
-            -   uses: actions/checkout@v3
+            -   uses: actions/checkout@v4
 
             -   name: Set up Python 3.11
-                uses: actions/setup-python@v3
+                uses: actions/setup-python@v5
                 with:
                     python-version: 3.11
                     cache: pip
 
             -   name: To PyPI using Flit
                 uses: AsifArmanRahman/to-pypi-using-flit@v1
                 with:
```

### Comparing `async_firebase_rest_api-2.0.1/.github/workflows/release.yml` & `async_firebase_rest_api-2.1.0/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 jobs:
 
     github-release:
         runs-on: ubuntu-latest
 
         steps:
-            -   uses: actions/checkout@v2
+            -   uses: actions/checkout@v4
 
             -   name: conventional Changelog Action
                 id: changelog
-                uses: TriPSs/conventional-changelog-action@v3.7.1
+                uses: TriPSs/conventional-changelog-action@v3.19.0
                 with:
                     github-token: ${{ secrets.GITHUB_TOKEN }}
                     version-file: ./pyproject.toml
                     version-path: project.version
                     release-count: 0
 
             -   name: create release
```

### Comparing `async_firebase_rest_api-2.0.1/.github/workflows/tests.yml` & `async_firebase_rest_api-2.1.0/.github/workflows/tests.yml`

 * *Files 23% similar despite different names*

```diff
@@ -24,18 +24,18 @@
         # The type of runner that the job will run on
         runs-on: ubuntu-latest
 
         # Steps represent a sequence of tasks that will be executed as part of the job
         steps:
 
             # Checks-out your repository under $GITHUB_WORKSPACE, so your job can access it
-            -   uses: actions/checkout@v3
+            -   uses: actions/checkout@v4
 
             -   name: Set up Python 3.11
-                uses: actions/setup-python@v3
+                uses: actions/setup-python@v5
                 with:
                     python-version: 3.11
                     cache: pip
 
             -   name: Install dependencies
                 run: |
                     python -m pip install --upgrade pip
@@ -55,20 +55,24 @@
                     FIREBASE_SERVICE_ACCOUNT_PROJECT_ID: ${{ secrets.FIREBASE_SERVICE_ACCOUNT_PROJECT_ID }}
                     FIREBASE_SERVICE_ACCOUNT_PRIVATE_KEY_ID: ${{ secrets.FIREBASE_SERVICE_ACCOUNT_PRIVATE_KEY_ID }}
                     FIREBASE_SERVICE_ACCOUNT_PRIVATE_KEY: ${{ secrets.FIREBASE_SERVICE_ACCOUNT_PRIVATE_KEY }}
                     FIREBASE_SERVICE_ACCOUNT_CLIENT_EMAIL: ${{ secrets.FIREBASE_SERVICE_ACCOUNT_CLIENT_EMAIL }}
                     FIREBASE_SERVICE_ACCOUNT_CLIENT_ID: ${{ secrets.FIREBASE_SERVICE_ACCOUNT_CLIENT_ID }}
                     FIREBASE_SERVICE_ACCOUNT_CLIENT_X509_CERT_URL: ${{ secrets.FIREBASE_SERVICE_ACCOUNT_CLIENT_X509_CERT_URL }}
 
+                    FIREBASE_OAUTH_CLIENT_ID: ${{ secrets.FIREBASE_OAUTH_CLIENT_ID }}
+                    FIREBASE_OAUTH_CLIENT_SECRET: ${{ secrets.FIREBASE_OAUTH_CLIENT_SECRET }}
+                    FIREBASE_OAUTH_CLIENT_REDIRECT_URI: ${{ secrets.FIREBASE_OAUTH_CLIENT_REDIRECT_URI }}
+
                     TEST_USER_EMAIL: ${{ secrets.TEST_USER_EMAIL }}
                     TEST_USER_PASSWORD: ${{ secrets.TEST_USER_PASSWORD }}
 
                     TEST_USER_EMAIL_2: ${{ secrets.TEST_USER_EMAIL_2 }}
                     TEST_USER_PASSWORD_2: ${{ secrets.TEST_USER_PASSWORD_2 }}
 
             -   name: Upload coverage to Codecov
-                uses: codecov/codecov-action@v2
+                uses: codecov/codecov-action@v4
                 with:
                     token: ${{ secrets.CODECOV_TOKEN }}
                     fail_ci_if_error: true
                     files: cov.xml
                     flags: pytest
```

### Comparing `async_firebase_rest_api-2.0.1/.gitignore` & `async_firebase_rest_api-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/.readthedocs.yaml` & `async_firebase_rest_api-2.1.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/CHANGELOG.md` & `async_firebase_rest_api-2.1.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+# [2.1.0](https://github.com/matiaskotlik/async-firebase-rest-api/compare/v2.0.1...v2.1.0) (2024-04-20)
+
+
+### Bug Fixes
+
+* allow concurrent test runs ([9db5272](https://github.com/matiaskotlik/async-firebase-rest-api/commit/9db5272a071b0ef99e79747a0f95ac09f207af7a))
+* allow concurrent test runs ([7e096ab](https://github.com/matiaskotlik/async-firebase-rest-api/commit/7e096ab3ae7f6a96a76105188984e69f132355e5))
+* disable facebook auth uri test ([9ea2d5a](https://github.com/matiaskotlik/async-firebase-rest-api/commit/9ea2d5a6ef890d87e64ab9d9311322a00d6f9b2b))
+* firestore tests ([40ad0c3](https://github.com/matiaskotlik/async-firebase-rest-api/commit/40ad0c38224a69fce391ce957af85891859f8c6c))
+* gha ([e7a0dd3](https://github.com/matiaskotlik/async-firebase-rest-api/commit/e7a0dd340e62d3abdbc256191b6129d14f6b9743))
+* gha ([0981abb](https://github.com/matiaskotlik/async-firebase-rest-api/commit/0981abb2b6e4d49ee7f80d34b1ed0295c6e71a79))
+
+
+### Features
+
+* interactive login ([94995c0](https://github.com/matiaskotlik/async-firebase-rest-api/commit/94995c00ec0d01147cb53d9b418c8bfd6e4a4ddd))
+
+
+
 ## [2.0.1](https://github.com/matiaskotlik/async-firebase-rest-api/compare/v2.0.0...v2.0.1) (2024-04-20)
 
 
 ### Bug Fixes
 
 * fix google and fb signin ([0d62775](https://github.com/matiaskotlik/async-firebase-rest-api/commit/0d627751bd477d7ee0f1ccd968763b051d39d2c0))
 * readme ([becbf9c](https://github.com/matiaskotlik/async-firebase-rest-api/commit/becbf9ce0256f254d742aebabb1693fe17058ca9))
```

### Comparing `async_firebase_rest_api-2.0.1/LICENSE` & `async_firebase_rest_api-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/README.md` & `async_firebase_rest_api-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/docs/conf.py` & `async_firebase_rest_api-2.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/docs/guide/authentication.rst` & `async_firebase_rest_api-2.1.0/docs/guide/authentication.rst`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/docs/guide/database.rst` & `async_firebase_rest_api-2.1.0/docs/guide/database.rst`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/docs/guide/firebase-rest-api.rst` & `async_firebase_rest_api-2.1.0/docs/guide/firebase-rest-api.rst`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/docs/guide/firestore.rst` & `async_firebase_rest_api-2.1.0/docs/guide/firestore.rst`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/docs/guide/setup.rst` & `async_firebase_rest_api-2.1.0/docs/guide/setup.rst`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/docs/guide/storage.rst` & `async_firebase_rest_api-2.1.0/docs/guide/storage.rst`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/docs/index.rst` & `async_firebase_rest_api-2.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/firebase/__init__.py` & `async_firebase_rest_api-2.1.0/firebase/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,29 +49,29 @@
 
 		self.credentials = None
 		self.requests = _custom_request()
 
 		if config.get("serviceAccount"):
 			self.credentials = _service_account_creds_from_secret(config['serviceAccount'])
 
-	def auth(self, client_secret=None):
+	def auth(self, client_id=None, client_secret=None, redirect_uri=None):
 		"""Initializes and returns a new Firebase Authentication
 		instance.
 
-		:type client_secret: str or dict
-		:param client_secret: (Optional) File path to or the dict
-			object from social client secret file, defaults to
-			:data:`None`.
+		:param client_id: OAuth 2.0 client ID
+		:type client_id: str
 
+		:param client_secret: OAuth 2.0 client secret
+		:type client_secret: str
 
 		:return: A newly initialized instance of Auth.
 		:rtype: Auth
 		"""
 
-		return Auth(self.api_key, self.credentials, self.requests, client_secret=client_secret)
+		return Auth(self.api_key, self.credentials, self.requests, client_id, client_secret, redirect_uri)
 
 	def database(self):
 		"""Initializes and returns a new Firebase Realtime Database
 		instance.
 
 		:return: A newly initialized instance of Database.
 		:rtype: Database
```

### Comparing `async_firebase_rest_api-2.0.1/firebase/_exception.py` & `async_firebase_rest_api-2.1.0/firebase/_exception.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/firebase/_service_account_credentials.py` & `async_firebase_rest_api-2.1.0/firebase/_service_account_credentials.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/firebase/auth/__init__.py` & `async_firebase_rest_api-2.1.0/firebase/auth/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,25 +10,29 @@
 `Firebase Authentication REST API`_
 
 .. _Firebase Authentication REST API: https://firebase.google.com/docs/reference/rest/auth
 """
 
 import json
 import math
+import webbrowser
+from http.server import HTTPServer, BaseHTTPRequestHandler
+
 import pkce
 import random
 import datetime
 import python_jwt as jwt
 from hashlib import sha256
 from jwcrypto.jwk import JWK
-from urllib.parse import parse_qs
+from urllib.parse import parse_qs, urlparse
 from google.auth.transport.requests import Request
 from cryptography.hazmat.primitives.serialization import Encoding, NoEncryption, PrivateFormat
 
 from firebase._exception import raise_detailed_error
+from firebase.auth.oauth_flow import start_oauth_flow
 
 
 class Auth:
 	""" Firebase Authentication Service
 
 	:type api_key: str
 	:param api_key: ``apiKey`` from Firebase configuration
@@ -41,46 +45,49 @@
 
 	:type client_secret: str or dict
 	:param client_secret: (Optional) File path to or the dict object
 		from social client secret file, defaults to :data:`None`.
 
 	"""
 
-	def __init__(self, api_key, credentials, requests, client_secret=None):
+	def __init__(self, api_key, credentials, requests, client_id=None, client_secret=None, redirect_uri=None):
 		""" Constructor method """
 
 		self.api_key = api_key
 		self.credentials = credentials
 		self.requests = requests
 
-		self.provider_id = None
 		self.session_id = None
 		self.__code_verifier = None
 		self.__nonce = None
 
-		if client_secret:
-			self.client_secret = _load_client_secret(client_secret)
+		self.client_id = client_id
+		self.client_secret = client_secret
+		self.client_redirect_uri = redirect_uri
 
-	async def authenticate_login_with_google(self):
-		""" Redirect the user to Google's OAuth 2.0 server to initiate 
-		the authentication and authorization process.
+	async def interactive_login_with_provider(self, provider_id):
+		""" Interactive OAuth Login.
 
-		:return: Google Sign In URL
-		:rtype: str
+		:type provider_id: str
+		:param provider_id: The IdP ID. For white listed IdPs it's a
+			short domain name e.g. 'google.com', 'aol.com', 'live.net'
+			and 'yahoo.com'. For other OpenID IdPs it's the OP
+			identifier.
+
+		:return: User account info and Firebase Auth Tokens.
+		:rtype: dict
 		"""
-		return await self.create_authentication_uri('google.com')
 
-	async def authenticate_login_with_facebook(self):
-		""" Redirect the user to Facebook's OAuth 2.0 server to
-		initiate the authentication and authorization process.
+		request_uri = await self.create_authentication_uri(provider_id)
+		webbrowser.open(request_uri)
+		code = await start_oauth_flow(self.client_redirect_uri)
+		if not code:
+			raise ValueError("Authorization failed")
 
-		:return: Facebook Sign In URL
-		:rtype: str
-		"""
-		return await self.create_authentication_uri('facebook.com')
+		return await self.sign_in_with_oauth_credential(provider_id, code)
 
 	async def create_authentication_uri(self, provider_id):
 		""" Creates an authentication URI for the given social
 		provider.
 
 		| For more details:
 		| |section-fetch-providers-for-email|_
@@ -102,17 +109,17 @@
 		:return: The URI used by the IDP to authenticate the user.
 		:rtype: str
 		"""
 
 		request_ref = "https://www.googleapis.com/identitytoolkit/v3/relyingparty/createAuthUri?key={0}".format(self.api_key)
 
 		data = {
-			"clientId": self.client_secret['client_id'],
+			"clientId": self.client_id,
 			"providerId": provider_id,
-			"continueUri": self.client_secret['redirect_uris'][0],
+			"continueUri": self.client_redirect_uri,
 		}
 
 		self.__nonce = "".join(random.choice("ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789") for _ in range(20))
 
 		if provider_id == 'google.com':
 			data['authFlowType'] = 'CODE_FLOW'
 			data['customParameter'] = {"access_type": 'offline', "prompt": 'select_account', "include_granted_scopes": 'true', "nonce": self.__nonce}
@@ -123,15 +130,14 @@
 			data['customParameter'] = {"code_challenge": code_challenge, "code_challenge_method": 'S256', "nonce": sha256(self.__nonce.encode('utf')).hexdigest()}
 
 		headers = {"content-type": "application/json; charset=UTF-8"}
 		request_object = await self.requests.post(request_ref, headers=headers, json=data)
 
 		raise_detailed_error(request_object)
 
-		self.provider_id = provider_id
 		self.session_id = request_object.json()['sessionId']
 
 		return request_object.json()['authUri']
 
 	async def sign_in_with_email_and_password(self, email, password):
 		""" Sign in a user with an email and password.
 
@@ -438,94 +444,88 @@
 		data = {"idToken": id_token}
 		request_object = await self.requests.post(request_ref, headers=headers, json=data)
 
 		raise_detailed_error(request_object)
 
 		return request_object.json()
 
-	async def sign_in_with_oauth_credential(self, oauth2callback_url):
+	async def sign_in_with_oauth_credential(self, provider_id, code):
 		""" Sign In With OAuth credential.
 
 		| For more details:
 		| |section-sign-in-with-oauth-credential|_
 
 		.. |section-sign-in-with-oauth-credential| replace::
 			Firebase Auth REST API | Sign in with OAuth credential
 
 		.. _section-sign-in-with-oauth-credential:
 			https://firebase.google.com/docs/reference/rest/auth#section-sign-in-with-oauth-credential
 
+		:param: provider_id: The provider ID.
+		:type provider_id: str
 
-		:type oauth2callback_url: str
-		:param oauth2callback_url: The URL redirected to after
-			successful authorization from the provider.
+		:param code: The OAuth code to sign in.
+		:type code: str
 
 		:return: User account info and Firebase Auth Tokens.
 		:rtype: dict
 		"""
 
 		request_ref = "https://www.googleapis.com/identitytoolkit/v3/relyingparty/verifyAssertion?key={0}".format(self.api_key)
 
-		token = self._token_from_auth_url(oauth2callback_url)
+		token = await self._token_from_auth_url(provider_id, code)
 		data = {
-			'postBody': f"providerId={self.provider_id}&{token['type']}={token['value']}&nonce={self.__nonce}",
+			'postBody': f"providerId={provider_id}&{token['type']}={token['value']}&nonce={self.__nonce}",
 			'autoCreate': 'true',
-			'requestUri': self.client_secret['redirect_uris'][0],
+			'requestUri': self.client_redirect_uri,
 			'sessionId': self.session_id,
 			'returnSecureToken': 'true',
 			'returnRefreshToken': 'true',
 			'returnIdpCredential': 'false',
 		}
 
 		headers = {"content-type": "application/json; charset=UTF-8"}
 		request_object = await self.requests.post(request_ref, headers=headers, json=data)
 
 		raise_detailed_error(request_object)
 
 		return _token_expire_time(request_object.json())
 
-	async def _token_from_auth_url(self, url):
+	async def _token_from_auth_url(self, provider_id, code):
 		""" Fetch tokens using the authorization code from given URL.
 
 
-		:type url: str
-		:param url: The URL redirected to after successful
-			authorization from the provider.
-
-
 		:return: The OAuth credential (an ID token).
 		:rtype: dict
 		"""
 
-		request_ref = _token_host(self.provider_id)
-
-		auth_url_values = parse_qs(url[url.index('?') + 1:])
+		request_ref = _token_host(provider_id)
 
 		data = {
-			'client_id': self.client_secret['client_id'],
-			'client_secret': self.client_secret['client_secret'],
-			'code': auth_url_values['code'][0],
-			'redirect_uri': self.client_secret['redirect_uris'][0],
+			'client_id': self.client_id,
+			'client_secret': self.client_secret,
+			'code': code,
+			'redirect_uri': self.client_redirect_uri,
 		}
 
-		if self.provider_id == 'google.com':
+		if provider_id == 'google.com':
 			data['grant_type'] = 'authorization_code'
-		elif self.provider_id == 'facebook.com':
+		elif provider_id == 'facebook.com':
 			data['code_verifier'] = self.__code_verifier
 
 		headers = {"content-type": "application/x-www-form-urlencoded; charset=UTF-8"}
-		request_object = await self.requests.post(request_ref, headers=headers, json=data)
+		request_object = await self.requests.post(request_ref, headers=headers, data=data)
 
 		raise_detailed_error(request_object)
 
 		return {
 			'type': 'id_token',
 			'value': request_object.json()['id_token'],
 		}
-	
+
 	async def change_email(self, id_token, email):
 		""" Changes a user's email
 
 		| For more details:
 		| `Firebase Auth REST API | section-change-email`_
 
 		.. _Firebase Auth REST API | section-change-email: https://firebase.google.com/docs/reference/rest/auth#section-change-email
@@ -545,15 +545,15 @@
 		headers = {"content-type": "application/json; charset=UTF-8"}
 		data = {"idToken": id_token, "email": email, "returnSecureToken": True}
 		request_object = await self.requests.post(request_ref, headers=headers, json=data)
 
 		raise_detailed_error(request_object)
 
 		return request_object.json()
-	
+
 	async def change_password(self, id_token, password):
 		""" Changes a user's password
 
 		| For more details:
 		| `Firebase Auth REST API | section-change-password`_
 
 		.. _Firebase Auth REST API | section-change-password: https://firebase.google.com/docs/reference/rest/auth#section-change-password
@@ -666,51 +666,23 @@
 
 		pub_key = JWK.from_pem(bytes(pub_pem.encode('utf-8')))
 		_, claims = jwt.verify_jwt(id_token, pub_key, [header['alg']], checks_optional=True)
 
 		return claims
 
 
-def _load_client_secret(secret):
-	""" Load social providers' client secret from file if file path
-	provided.
-
-	This function also restructures the dict object to make it
-	compatible for usage.
-
-
-	:type secret: str or dict
-	:param secret: File path to or the dict object from social client
-		secret file.
-
-	:return: social client secret
-	:rtype: dict
-	"""
-
-	if type(secret) is str:
-		with open(secret) as file:
-			secret = json.load(file)
-
-	# Google client secrets are stored within 'web' key
-	# We will remove the key, and replace it with the dict type value of it
-	if secret.get('web'):
-		secret = secret['web']
-
-	return secret
-
-
 def _token_expire_time(user):
 	""" Adds expire time of the token in the token dictionary.
 
 	For safety purposes, token is set to expire after 59mins instead
 	of an hour expiry time when received.
 
 	:type user: dict
 	:param user: The token dictionary received after signing in users.
-	
+
 	:return: Token dictionary with an ``expiresAt`` key.
 	:rtype: dict
 	"""
 
 	user['expiresAt'] = math.floor(datetime.datetime.today().timestamp() + int(user.get('expiresIn', 3600)) - 60)
 
 	return user
```

### Comparing `async_firebase_rest_api-2.0.1/firebase/database/__init__.py` & `async_firebase_rest_api-2.1.0/firebase/database/__init__.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/firebase/database/_custom_sse_client.py` & `async_firebase_rest_api-2.1.0/firebase/database/_custom_sse_client.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/firebase/database/_db_convert.py` & `async_firebase_rest_api-2.1.0/firebase/database/_db_convert.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/firebase/database/_keep_auth_session.py` & `async_firebase_rest_api-2.1.0/firebase/database/_keep_auth_session.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/firebase/firestore/__init__.py` & `async_firebase_rest_api-2.1.0/firebase/firestore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,29 @@
 
 			raise_detailed_error(response)
 
 			doc_id = response.json()['name'].split('/')
 
 			return doc_id.pop()
 
+	def collection(self, collection_id):
+		""" A reference to a collection in a Firestore database.
+
+
+		:type collection_id: str
+		:param collection_id: An ID of collection in firestore.
+
+
+		:return: Reference to a collection.
+		:rtype: Collection
+		"""
+
+		self._path.append(collection_id)
+		return Collection(self._path, api_key=self._api_key, credentials=self._credentials, project_id=self._project_id, requests=self._requests)
+
 	def document(self, document_id):
 		""" A reference to a document in a collection.
 
 
 		:type document_id: str
 		:param document_id: An ID of document inside a collection.
```

### Comparing `async_firebase_rest_api-2.0.1/firebase/firestore/_utils.py` & `async_firebase_rest_api-2.1.0/firebase/firestore/_utils.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/firebase/storage/__init__.py` & `async_firebase_rest_api-2.1.0/firebase/storage/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -134,26 +134,23 @@
 		else:
 			file_object = file
 
 		request_ref = self.storage_bucket + "/o?name={0}".format(path)
 
 		if token:
 			headers = {"Authorization": "Firebase " + token}
-			return await asyncio.get_event_loop().run_in_executor(
-				None, upload_file, request_ref, file_object, headers)
+			return await asyncio.to_thread(upload_file, request_ref, file_object, headers)
 
 		elif self.credentials:
 			blob = self.bucket.blob(path)
 			upload_func = blob.upload_from_filename if isinstance(file, str) else blob.upload_from_file
-			return await asyncio.get_event_loop().run_in_executor(
-				None, upload_func, file)
+			return await asyncio.to_thread(upload_func, file)
 
 		else:
-			return await asyncio.get_event_loop().run_in_executor(
-				None, upload_file, request_ref, file_object)
+			return await asyncio.to_thread(upload_file, request_ref, file_object)
 
 	async def delete(self, token=None):
 		""" Delete file from storage.
 
 		| For more details:
 		| |delete_a_file|_
 
@@ -175,15 +172,15 @@
 		self.path = None
 
 		# remove leading backlash
 		if path.startswith('/'):
 			path = path[1:]
 
 		if self.credentials:
-			await asyncio.get_event_loop().run_in_executor(None, self.bucket.delete_blob, path)
+			await asyncio.to_thread(self.bucket.delete_blob, path)
 		else:
 			request_ref = self.storage_bucket + "/o?name={0}".format(path)
 
 			if token:
 				headers = {"Authorization": "Firebase " + token}
 				request_object = await self.requests.delete(request_ref, headers=headers)
 			else:
@@ -219,25 +216,23 @@
 			path = self.path
 			self.path = None
 
 			# remove leading backlash
 			if path.startswith('/'):
 				path = path[1:]
 
-			blob = await asyncio.get_event_loop().run_in_executor(None, self.bucket.get_blob, path)
+			blob = await asyncio.to_thread(self.bucket.get_blob, path)
 			if blob is not None:
-				await asyncio.get_event_loop().run_in_executor(None, blob.download_to_filename, filename)
+				await asyncio.to_thread(blob.download_to_filename, filename)
 
 		elif token:
 			headers = {"Authorization": "Firebase " + token}
-			await asyncio.get_event_loop().run_in_executor(
-				None, download_file, await self.get_url(token), filename, headers)
+			await asyncio.to_thread(download_file, await self.get_url(token), filename, headers)
 		else:
-			await asyncio.get_event_loop().run_in_executor(
-				None, download_file, await self.get_url(), filename)
+			await asyncio.to_thread(download_file, await self.get_url(), filename)
 
 	async def get_url(self, token=None, expiration_hour=24):
 		""" Fetches URL for file.
 
 
 		:type token: str
 		:param token: (Optional) Firebase Auth User ID Token, defaults
```

### Comparing `async_firebase_rest_api-2.0.1/pyproject.toml` & `async_firebase_rest_api-2.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "async-firebase-rest-api"
 authors = [
   {name = "Asif Arman Rahman", email = "asifarmanrahman@gmail.com"},
   {name = "Matias Kotlik", email = "mdkotlik@gmail.com"}
 ]
-version = "2.0.1"
+version = "2.1.0"
 readme = "README.md"
 description = "An async python wrapper for Google's Firebase REST API's."
 requires-python = ">=3.11"
 keywords = [
   "firebase",
   "firebase-auth",
   "firebase-database",
```

### Comparing `async_firebase_rest_api-2.0.1/tests/config.py` & `async_firebase_rest_api-2.1.0/tests/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,13 +39,10 @@
 
 # get this json file from firebase console
 # go to project settings, service accounts tab and click generate new private key
 SERVICE_ACCOUNT_PATH = "firebase-adminsdk.json"
 
 SERVICE_CONFIG_WITH_FILE_PATH = dict(SIMPLE_CONFIG, serviceAccount=SERVICE_ACCOUNT_PATH)
 
-
-TEST_USER_EMAIL = config('TEST_USER_EMAIL')
-TEST_USER_PASSWORD = config('TEST_USER_PASSWORD')
-
-TEST_USER_EMAIL_2 = config('TEST_USER_EMAIL_2')
-TEST_USER_PASSWORD_2 = config('TEST_USER_PASSWORD_2')
+OAUTH_CLIENT_ID = config('FIREBASE_OAUTH_CLIENT_ID')
+OAUTH_CLIENT_SECRET = config('FIREBASE_OAUTH_CLIENT_SECRET')
+OAUTH_CLIENT_REDIRECT_URI = config('FIREBASE_OAUTH_CLIENT_REDIRECT_URI')
```

### Comparing `async_firebase_rest_api-2.0.1/tests/config.template.py` & `async_firebase_rest_api-2.1.0/tests/config.template.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/tests/conftest.py` & `async_firebase_rest_api-2.1.0/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 
 
 import pytest
 import asyncio
 
 from firebase import initialize_app
 from tests import config
-from tests.config import (
-	TEST_USER_EMAIL, TEST_USER_PASSWORD,
-	TEST_USER_EMAIL_2, TEST_USER_PASSWORD_2
-)
+from tests.utils import rand_str
+
 
 @pytest.fixture(scope='session')
 def event_loop():
 	loop = asyncio.get_event_loop()
 	loop.close = lambda: None
 	yield loop
 
@@ -26,52 +24,52 @@
 
 @pytest.fixture(scope='session')
 async def service_app():
 	yield initialize_app(config.SERVICE_CONFIG)
 
 @pytest.fixture(scope='session')
 def auth(client_app):
-	return client_app.auth()
+	return client_app.auth(config.OAUTH_CLIENT_ID, config.OAUTH_CLIENT_SECRET, config.OAUTH_CLIENT_REDIRECT_URI)
 
 @pytest.fixture(scope='session')
 def auth_admin(service_app):
-	return service_app.auth()
+	return service_app.auth(config.OAUTH_CLIENT_ID, config.OAUTH_CLIENT_SECRET, config.OAUTH_CLIENT_REDIRECT_URI)
 
 @pytest.fixture(scope='session')
 async def db(service_app):
 	# To make it easier to test, we keep the test restricted to firebase_tests
 	# Because of the current mutations on calls, we return it as a function.
 	try:
 		yield lambda: service_app.database().child('firebase_tests')
 	finally:
 		await service_app.database().child('firebase_tests').remove()
 
 @pytest.fixture(scope='session')
 def email():
-	return TEST_USER_EMAIL
+	return f'{rand_str()}@gmail.com'
 
 @pytest.fixture(scope='session')
 def email_2():
-	return TEST_USER_EMAIL_2
+	return f'{rand_str()}@gmail.com'
 
 @pytest.fixture(scope='session')
 def ds(client_app):
 	return client_app.firestore()
 
 @pytest.fixture(scope='session')
 def ds_admin(service_app):
 	return service_app.firestore()
 
 @pytest.fixture(scope='session')
 def password():
-	return TEST_USER_PASSWORD
+	return rand_str()
 
 @pytest.fixture(scope='session')
 def password_2():
-	return TEST_USER_PASSWORD_2
+	return rand_str()
 
 @pytest.fixture(scope='session')
 def storage(client_app):
 	return client_app.storage()
 
 @pytest.fixture(scope='session')
 def storage_admin(service_app):
```

### Comparing `async_firebase_rest_api-2.0.1/tests/static/test-file.txt` & `async_firebase_rest_api-2.1.0/tests/static/test-file.txt`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/tests/test_auth.py` & `async_firebase_rest_api-2.1.0/tests/test_auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 #   Copyright (c) 2022 Asif Arman Rahman
 #   Licensed under MIT (https://github.com/AsifArmanRahman/firebase/blob/main/LICENSE)
+import os
 
 # --------------------------------------------------------------------------------------
 
 
 import pytest
 import httpx
 
+interactive = pytest.mark.skipif(bool(os.environ.get('GITHUB_ACTION')), reason="Interactive test")
 
 class TestAuth:
 
 	user = None
 	anonymous_user = None
 
+	@interactive
+	async def test_interactive_google_login(self, auth):
+		user = await auth.interactive_login_with_provider('google.com')
+		assert await auth.get_account_info(user.get('idToken'))
+
+	@pytest.mark.parametrize('provider', ['google.com'])
+	async def test_create_authorization_uri(self, auth, provider):
+		assert await auth.create_authentication_uri(provider)
+
 	async def test_sign_in_with_non_existing_account_email_and_password(self, auth, email, password):
 		with pytest.raises(httpx.HTTPError) as exc_info:
 			await auth.sign_in_with_email_and_password(email, password)
 		assert "INVALID_LOGIN_CREDENTIALS" in str(exc_info.value)
 
 	async def test_create_user_with_email_and_password(self, auth, email, password):
 		assert await auth.create_user_with_email_and_password(email, password)
@@ -65,15 +76,14 @@
 	async def test_send_password_reset_email(self, auth):
 		assert await auth.send_password_reset_email(self.__class__.user.get('email'))
 
 	@pytest.mark.xfail
 	async def test_verify_password_reset_code(self, auth):
 		assert await auth.verify_password_reset_code('123456', 'NewTestPassword123')
 
-
 	async def test_change_email(self, auth, email_2, password):
 		with pytest.raises(httpx.HTTPError) as exc_info:
 			await auth.change_email(self.__class__.user.get('idToken'), email_2)
 		assert "OPERATION_NOT_ALLOWED" in str(exc_info.value)
 
 	async def test_change_password(self, auth,email, password_2):
 		user = await auth.change_password(self.__class__.user.get('idToken'), password_2)
```

### Comparing `async_firebase_rest_api-2.0.1/tests/test_database.py` & `async_firebase_rest_api-2.1.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/tests/test_firestore.py` & `async_firebase_rest_api-2.1.0/tests/test_firestore.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,20 @@
+import pytest
+
+from tests.utils import rand_str
+
 
 #   Copyright (c) 2022 Asif Arman Rahman
 #   Licensed under MIT (https://github.com/AsifArmanRahman/firebase/blob/main/LICENSE)
 
 # --------------------------------------------------------------------------------------
 
+@pytest.fixture(scope='module')
+def test_collection():
+	return f'Marvels_test_{rand_str()}'
 
 class TestFirestoreAdmin:
 	movies1 = {
 		'name': 'Iron Man',
 		'lead': {'name': 'Robert Downey Jr.'},
 		'director': '',
 		'released': False,
@@ -24,82 +31,82 @@
 		'year': 2011,
 		'rating': 7.0,
 		'cast': ['Tom Hiddleston', 'Natalie Portman', 'Anthony Hopkins', 'Jeremy Renner', 'Stellan Skarsgård', 'Idris Elba', 'Kat Dennings']
 	}
 
 	auto_doc_id = None
 
-	async def test_manual_doc_set(self, ds_admin):
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').document('001').set(self.__class__.movies1) is None
+	async def test_manual_doc_set(self, ds_admin, test_collection):
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').document('001').set(self.__class__.movies1) is None
 
-	async def test_auto_doc_add(self, ds_admin):
-		doc_id = await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').add(self.__class__.movies2)
+	async def test_auto_doc_add(self, ds_admin, test_collection):
+		doc_id = await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').add(self.__class__.movies2)
 		assert doc_id
 
 		self.__class__.auto_doc_id = doc_id
 
-	async def test_manual_doc_get(self, ds_admin):
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').document('001').get() == self.__class__.movies1
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').document(self.__class__.auto_doc_id).get() == self.__class__.movies2
+	async def test_manual_doc_get(self, ds_admin, test_collection):
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').document('001').get() == self.__class__.movies1
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').document(self.__class__.auto_doc_id).get() == self.__class__.movies2
 
-	async def test_collection_get(self, ds_admin):
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').get() == [{'001': self.__class__.movies1}, {self.__class__.auto_doc_id: self.__class__.movies2}]
+	async def test_collection_get(self, ds_admin, test_collection):
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').get() == [{'001': self.__class__.movies1}, {self.__class__.auto_doc_id: self.__class__.movies2}]
 
-	async def test_collection_list_document(self, ds_admin):
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').list_of_documents() == ['001', self.__class__.auto_doc_id]
+	async def test_collection_list_document(self, ds_admin, test_collection):
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').list_of_documents() == ['001', self.__class__.auto_doc_id]
 
-	async def test_collection_get_start_after(self, ds_admin):
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').order_by('rating').start_after({'rating': 7.4}).get() == [{'001': self.__class__.movies1}]
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').order_by('rating').start_after({'rating': 6.9}).get() == [{self.__class__.auto_doc_id: self.__class__.movies2}, {'001': self.__class__.movies1}]
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').order_by('rating').start_after({'rating': 8.5}).get() == []
+	async def test_collection_get_start_after(self, ds_admin, test_collection):
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').order_by('rating').start_after({'rating': 7.4}).get() == [{'001': self.__class__.movies1}]
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').order_by('rating').start_after({'rating': 6.9}).get() == [{self.__class__.auto_doc_id: self.__class__.movies2}, {'001': self.__class__.movies1}]
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').order_by('rating').start_after({'rating': 8.5}).get() == []
 
-	async def test_collection_get_start_at(self, ds_admin):
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').order_by('rating').start_at({'rating': 7.4}).get() == [{'001': self.__class__.movies1}]
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').order_by('rating').start_at({'rating': 8.0}).get() == []
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').order_by('rating').start_at({'rating': 7.0}).get() == [{self.__class__.auto_doc_id: self.__class__.movies2}, {'001': self.__class__.movies1}]
+	async def test_collection_get_start_at(self, ds_admin, test_collection):
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').order_by('rating').start_at({'rating': 7.4}).get() == [{'001': self.__class__.movies1}]
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').order_by('rating').start_at({'rating': 8.0}).get() == []
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').order_by('rating').start_at({'rating': 7.0}).get() == [{self.__class__.auto_doc_id: self.__class__.movies2}, {'001': self.__class__.movies1}]
 
-	async def test_collection_get_select(self, ds_admin):
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').select(['lead.name', 'released']).get() == [{'001': {'lead': self.__class__.movies1['lead'], 'released': self.__class__.movies1['released']}}, {self.__class__.auto_doc_id: {'lead': self.__class__.movies2['lead'], 'released': self.__class__.movies2['released']}}]
+	async def test_collection_get_select(self, ds_admin, test_collection):
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').select(['lead.name', 'released']).get() == [{'001': {'lead': self.__class__.movies1['lead'], 'released': self.__class__.movies1['released']}}, {self.__class__.auto_doc_id: {'lead': self.__class__.movies2['lead'], 'released': self.__class__.movies2['released']}}]
 
-	async def test_collection_get_offset(self, ds_admin):
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').order_by('year').offset(1).get() == [{self.__class__.auto_doc_id: self.__class__.movies2}]
+	async def test_collection_get_offset(self, ds_admin, test_collection):
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').order_by('year').offset(1).get() == [{self.__class__.auto_doc_id: self.__class__.movies2}]
 
-	async def test_collection_get_limit_to_first(self, ds_admin):
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').order_by('year').limit_to_first(1).get() == [{'001': self.__class__.movies1}]
+	async def test_collection_get_limit_to_first(self, ds_admin, test_collection):
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').order_by('year').limit_to_first(1).get() == [{'001': self.__class__.movies1}]
 
-	async def test_collection_get_limit_to_last(self, ds_admin):
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').order_by('year', direction='DESCENDING').limit_to_last(1).get() == [{'001': self.__class__.movies1}]
+	async def test_collection_get_limit_to_last(self, ds_admin, test_collection):
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').order_by('year', direction='DESCENDING').limit_to_last(1).get() == [{'001': self.__class__.movies1}]
 
-	async def test_collection_get_end_at(self, ds_admin):
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').order_by('year').end_at({'year': 2010}).get() == [{'001': self.__class__.movies1}]
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').order_by('year').end_at({'year': 2021}).get() == [{'001': self.__class__.movies1}, {self.__class__.auto_doc_id: self.__class__.movies2}]
+	async def test_collection_get_end_at(self, ds_admin, test_collection):
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').order_by('year').end_at({'year': 2010}).get() == [{'001': self.__class__.movies1}]
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').order_by('year').end_at({'year': 2021}).get() == [{'001': self.__class__.movies1}, {self.__class__.auto_doc_id: self.__class__.movies2}]
 
-	async def test_collection_get_end_before(self, ds_admin):
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').order_by('year').end_before({'year': 2023}).get() == [{'001': self.__class__.movies1}, {self.__class__.auto_doc_id: self.__class__.movies2}]
+	async def test_collection_get_end_before(self, ds_admin, test_collection):
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').order_by('year').end_before({'year': 2023}).get() == [{'001': self.__class__.movies1}, {self.__class__.auto_doc_id: self.__class__.movies2}]
 
-	async def test_collection_get_where(self, ds_admin):
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').where('lead.name', 'in',  ['Benedict Cumberbatch', 'Robert Downey Jr.']).get() == [{'001': self.__class__.movies1}]
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').where('rating', '<=', 8.0).order_by('rating', direction='DESCENDING').get() == [{'001': self.__class__.movies1}, {self.__class__.auto_doc_id: self.__class__.movies2}]
+	async def test_collection_get_where(self, ds_admin, test_collection):
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').where('lead.name', 'in',  ['Benedict Cumberbatch', 'Robert Downey Jr.']).get() == [{'001': self.__class__.movies1}]
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').where('rating', '<=', 8.0).order_by('rating', direction='DESCENDING').get() == [{'001': self.__class__.movies1}, {self.__class__.auto_doc_id: self.__class__.movies2}]
 
-	async def test_manual_doc_update(self, ds_admin):
+	async def test_manual_doc_update(self, ds_admin, test_collection):
 		update_data = {'released': True}
 
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').document('001').update(update_data) is None
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').document('001').get(field_paths=['released']) == update_data
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').document('001').update(update_data) is None
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').document('001').get(field_paths=['released']) == update_data
 
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').document(self.__class__.auto_doc_id).update(update_data) is None
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').document(self.__class__.auto_doc_id).get(field_paths=['released']) == update_data
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').document(self.__class__.auto_doc_id).update(update_data) is None
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').document(self.__class__.auto_doc_id).get(field_paths=['released']) == update_data
 
-	async def test_manual_doc_get_filtered(self, ds_admin):
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').document('001').get(field_paths=['name']) == {'name': self.__class__.movies1['name']}
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').document(self.__class__.auto_doc_id).get(field_paths=['name']) == {'name': self.__class__.movies2['name']}
-
-	async def test_manual_doc_delete(self, ds_admin):
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').document('001').delete() is None
-		assert await ds_admin.collection('Marvels').document('Movies').collection('PhaseOne').document(self.__class__.auto_doc_id).delete() is None
+	async def test_manual_doc_get_filtered(self, ds_admin, test_collection):
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').document('001').get(field_paths=['name']) == {'name': self.__class__.movies1['name']}
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').document(self.__class__.auto_doc_id).get(field_paths=['name']) == {'name': self.__class__.movies2['name']}
+
+	async def test_manual_doc_delete(self, ds_admin, test_collection):
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').document('001').delete() is None
+		assert await ds_admin.collection(test_collection).document('Movies').collection('PhaseOne').document(self.__class__.auto_doc_id).delete() is None
 
 
 class TestFirestoreAuth:
 	movies1 = {
 		'name': 'Dr. Strange',
 		'lead': {'name': 'Benedict Cumberbatch'},
 		'director': {},
@@ -126,82 +133,82 @@
 
 	async def test_create_test_user(self, auth):
 		user = await auth.sign_in_anonymous()
 		self.__class__.user = user
 		assert user
 		assert user.get('idToken')
 
-	async def test_manual_doc_set(self, ds):
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').document('014').set(self.__class__.movies1, token=self.__class__.user.get('idToken')) is None
+	async def test_manual_doc_set(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').document('014').set(self.__class__.movies1, token=self.__class__.user.get('idToken')) is None
 
-	async def test_auto_doc_add(self, ds):
-		doc_id = await ds.collection('Marvels').document('Movies').collection('PhaseThree').add(self.__class__.movies2, token=self.__class__.user.get('idToken'))
+	async def test_auto_doc_add(self, ds, test_collection):
+		doc_id = await ds.collection(test_collection).document('Movies').collection('PhaseThree').add(self.__class__.movies2, token=self.__class__.user.get('idToken'))
 		assert doc_id
 
 		self.__class__.auto_doc_id = doc_id
 
-	async def test_manual_doc_get(self, ds):
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').document('014').get(token=self.__class__.user.get('idToken')) == self.__class__.movies1
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').document(self.__class__.auto_doc_id).get(token=self.__class__.user.get('idToken')) == self.__class__.movies2
+	async def test_manual_doc_get(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').document('014').get(token=self.__class__.user.get('idToken')) == self.__class__.movies1
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').document(self.__class__.auto_doc_id).get(token=self.__class__.user.get('idToken')) == self.__class__.movies2
 
-	async def test_collection_get(self, ds):
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}, {self.__class__.auto_doc_id: self.__class__.movies2}]
+	async def test_collection_get(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}, {self.__class__.auto_doc_id: self.__class__.movies2}]
 
-	async def test_collection_list_documents(self, ds):
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').list_of_documents(token=self.__class__.user.get('idToken')) == ['014', self.__class__.auto_doc_id]
+	async def test_collection_list_documents(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').list_of_documents(token=self.__class__.user.get('idToken')) == ['014', self.__class__.auto_doc_id]
 
-	async def test_manual_doc_get_filtered(self, ds):
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').document('014').get(field_paths=['name'], token=self.__class__.user.get('idToken')) == {'name': self.__class__.movies1['name']}
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').document(self.__class__.auto_doc_id).get(field_paths=['name'], token=self.__class__.user.get('idToken')) == {'name': self.__class__.movies2['name']}
+	async def test_manual_doc_get_filtered(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').document('014').get(field_paths=['name'], token=self.__class__.user.get('idToken')) == {'name': self.__class__.movies1['name']}
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').document(self.__class__.auto_doc_id).get(field_paths=['name'], token=self.__class__.user.get('idToken')) == {'name': self.__class__.movies2['name']}
 
-	async def test_collection_get_start_after(self, ds):
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').order_by('rating').start_after({'rating': 7.4}).get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}]
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').order_by('rating').start_after({'rating': 7.2}).get(token=self.__class__.user.get('idToken')) == [{self.__class__.auto_doc_id: self.__class__.movies2}, {'014': self.__class__.movies1}]
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').order_by('rating').start_after({'rating': 8.5}).get(token=self.__class__.user.get('idToken')) == []
+	async def test_collection_get_start_after(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').order_by('rating').start_after({'rating': 7.4}).get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}]
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').order_by('rating').start_after({'rating': 7.2}).get(token=self.__class__.user.get('idToken')) == [{self.__class__.auto_doc_id: self.__class__.movies2}, {'014': self.__class__.movies1}]
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').order_by('rating').start_after({'rating': 8.5}).get(token=self.__class__.user.get('idToken')) == []
 
-	async def test_collection_get_start_at(self, ds):
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').order_by('rating').start_at({'rating': 7.4}).get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}]
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').order_by('rating').start_at({'rating': 8.0}).get(token=self.__class__.user.get('idToken')) == []
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').order_by('rating').start_at({'rating': 7.0}).get(token=self.__class__.user.get('idToken')) == [{self.__class__.auto_doc_id: self.__class__.movies2}, {'014': self.__class__.movies1}]
+	async def test_collection_get_start_at(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').order_by('rating').start_at({'rating': 7.4}).get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}]
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').order_by('rating').start_at({'rating': 8.0}).get(token=self.__class__.user.get('idToken')) == []
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').order_by('rating').start_at({'rating': 7.0}).get(token=self.__class__.user.get('idToken')) == [{self.__class__.auto_doc_id: self.__class__.movies2}, {'014': self.__class__.movies1}]
 
-	async def test_collection_get_select(self, ds):
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').select(['lead.name', 'released']).get(token=self.__class__.user.get('idToken')) == [{'014': {'lead': self.__class__.movies1['lead'], 'released': self.__class__.movies1['released']}}, {self.__class__.auto_doc_id: {'lead': self.__class__.movies2['lead'], 'released': self.__class__.movies2['released']}}]
+	async def test_collection_get_select(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').select(['lead.name', 'released']).get(token=self.__class__.user.get('idToken')) == [{'014': {'lead': self.__class__.movies1['lead'], 'released': self.__class__.movies1['released']}}, {self.__class__.auto_doc_id: {'lead': self.__class__.movies2['lead'], 'released': self.__class__.movies2['released']}}]
 
-	async def test_collection_get_offset(self, ds):
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').order_by('year').offset(1).get(token=self.__class__.user.get('idToken')) == [{self.__class__.auto_doc_id: self.__class__.movies2}]
+	async def test_collection_get_offset(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').order_by('year').offset(1).get(token=self.__class__.user.get('idToken')) == [{self.__class__.auto_doc_id: self.__class__.movies2}]
 
-	async def test_collection_get_limit_to_first(self, ds):
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').order_by('year').limit_to_first(1).get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}]
+	async def test_collection_get_limit_to_first(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').order_by('year').limit_to_first(1).get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}]
 
-	async def test_collection_get_limit_to_last(self, ds):
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').order_by('year').limit_to_last(1).get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}]
+	async def test_collection_get_limit_to_last(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').order_by('year').limit_to_last(1).get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}]
 
-	async def test_collection_get_end_at(self, ds):
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').order_by('year').end_at({'year': 2010}).get(token=self.__class__.user.get('idToken')) == []
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').order_by('year').end_at({'year': 2021}).get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}, {self.__class__.auto_doc_id: self.__class__.movies2}]
+	async def test_collection_get_end_at(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').order_by('year').end_at({'year': 2010}).get(token=self.__class__.user.get('idToken')) == []
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').order_by('year').end_at({'year': 2021}).get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}, {self.__class__.auto_doc_id: self.__class__.movies2}]
 
-	async def test_collection_get_end_before(self, ds):
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').order_by('year').end_before({'year': 2023}).get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}, {self.__class__.auto_doc_id: self.__class__.movies2}]
+	async def test_collection_get_end_before(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').order_by('year').end_before({'year': 2023}).get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}, {self.__class__.auto_doc_id: self.__class__.movies2}]
 
-	async def test_collection_get_where(self, ds):
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').where('lead.name', 'in',  ['Benedict Cumberbatch', 'Robert Downey Jr.']).get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}]
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').where('rating', '<=', 8.0).order_by('rating', direction='DESCENDING').get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}, {self.__class__.auto_doc_id: self.__class__.movies2}]
+	async def test_collection_get_where(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').where('lead.name', 'in',  ['Benedict Cumberbatch', 'Robert Downey Jr.']).get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}]
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').where('rating', '<=', 8.0).order_by('rating', direction='DESCENDING').get(token=self.__class__.user.get('idToken')) == [{'014': self.__class__.movies1}, {self.__class__.auto_doc_id: self.__class__.movies2}]
 
-	async def test_manual_doc_update(self, ds):
+	async def test_manual_doc_update(self, ds, test_collection):
 		update_data = {'released': True}
 
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').document('014').update(update_data, token=self.__class__.user.get('idToken')) is None
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').document('014').get(field_paths=['released'], token=self.__class__.user.get('idToken')) == update_data
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').document('014').update(update_data, token=self.__class__.user.get('idToken')) is None
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').document('014').get(field_paths=['released'], token=self.__class__.user.get('idToken')) == update_data
 
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').document(self.__class__.auto_doc_id).update(update_data, token=self.__class__.user.get('idToken')) is None
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').document(self.__class__.auto_doc_id).get(field_paths=['released'], token=self.__class__.user.get('idToken')) == update_data
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').document(self.__class__.auto_doc_id).update(update_data, token=self.__class__.user.get('idToken')) is None
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').document(self.__class__.auto_doc_id).get(field_paths=['released'], token=self.__class__.user.get('idToken')) == update_data
 
-	async def test_manual_doc_delete(self, ds):
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').document('014').delete(self.__class__.user.get('idToken')) is None
-		assert await ds.collection('Marvels').document('Movies').collection('PhaseThree').document(self.__class__.auto_doc_id).delete(self.__class__.user.get('idToken')) is None
+	async def test_manual_doc_delete(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').document('014').delete(self.__class__.user.get('idToken')) is None
+		assert await ds.collection(test_collection).document('Movies').collection('PhaseThree').document(self.__class__.auto_doc_id).delete(self.__class__.user.get('idToken')) is None
 
 	async def test_delete_test_user(self, auth):
 		assert await auth.delete_user_account(self.__class__.user.get('idToken'))
 
 
 class TestFirestore:
 	series1 = {
@@ -222,75 +229,75 @@
 		'rating': 7.4,
 		'prequel': None,
 		'cast': ['Ethan Hawke', 'May Calamawy', 'F. Murray Abraham']
 	}
 
 	auto_doc_id = None
 
-	async def test_manual_doc_set(self, ds):
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').document('003').set(self.__class__.series1) is None
+	async def test_manual_doc_set(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').document('003').set(self.__class__.series1) is None
 
-	async def test_auto_doc_add(self, ds):
-		doc_id = await ds.collection('Marvels').document('Series').collection('PhaseFour').add(self.__class__.series2)
+	async def test_auto_doc_add(self, ds, test_collection):
+		doc_id = await ds.collection(test_collection).document('Series').collection('PhaseFour').add(self.__class__.series2)
 		assert doc_id
 
 		self.__class__.auto_doc_id = doc_id
 
-	async def test_manual_doc_get(self, ds):
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').document('003').get() == self.__class__.series1
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').document(self.__class__.auto_doc_id).get() == self.__class__.series2
+	async def test_manual_doc_get(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').document('003').get() == self.__class__.series1
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').document(self.__class__.auto_doc_id).get() == self.__class__.series2
 
-	async def test_collection_get(self, ds):
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').get() == [{'003': self.__class__.series1}, {self.__class__.auto_doc_id: self.__class__.series2}]
+	async def test_collection_get(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').get() == [{'003': self.__class__.series1}, {self.__class__.auto_doc_id: self.__class__.series2}]
 
-	async def test_collection_list_documents(self, ds):
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').list_of_documents() == ['003', self.__class__.auto_doc_id]
+	async def test_collection_list_documents(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').list_of_documents() == ['003', self.__class__.auto_doc_id]
 
-	async def test_manual_doc_get_filtered(self, ds):
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').document('003').get(field_paths=['name']) == {'name': self.__class__.series1['name']}
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').document(self.__class__.auto_doc_id).get(field_paths=['name']) == {'name': self.__class__.series2['name']}
+	async def test_manual_doc_get_filtered(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').document('003').get(field_paths=['name']) == {'name': self.__class__.series1['name']}
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').document(self.__class__.auto_doc_id).get(field_paths=['name']) == {'name': self.__class__.series2['name']}
 
-	async def test_collection_get_start_after(self, ds):
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').order_by('rating').start_after({'rating': 7.4}).get() == [{'003': self.__class__.series1}]
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').order_by('rating').start_after({'rating': 7.3}).get() == [{self.__class__.auto_doc_id: self.__class__.series2}, {'003': self.__class__.series1}]
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').order_by('rating').start_after({'rating': 8.5}).get() == []
+	async def test_collection_get_start_after(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').order_by('rating').start_after({'rating': 7.4}).get() == [{'003': self.__class__.series1}]
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').order_by('rating').start_after({'rating': 7.3}).get() == [{self.__class__.auto_doc_id: self.__class__.series2}, {'003': self.__class__.series1}]
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').order_by('rating').start_after({'rating': 8.5}).get() == []
 
-	async def test_collection_get_start_at(self, ds):
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').order_by('rating').start_at({'rating': 7.4}).get() == [{self.__class__.auto_doc_id: self.__class__.series2}, {'003': self.__class__.series1}]
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').order_by('rating').start_at({'rating': 8.0}).get() == [{'003': self.__class__.series1}]
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').order_by('rating').start_at({'rating': 8.5}).get() == []
+	async def test_collection_get_start_at(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').order_by('rating').start_at({'rating': 7.4}).get() == [{self.__class__.auto_doc_id: self.__class__.series2}, {'003': self.__class__.series1}]
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').order_by('rating').start_at({'rating': 8.0}).get() == [{'003': self.__class__.series1}]
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').order_by('rating').start_at({'rating': 8.5}).get() == []
 
-	async def test_collection_get_select(self, ds):
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').select(['lead.name', 'released']).get() == [{'003': {'lead': self.__class__.series1['lead'], 'released': self.__class__.series1['released']}}, {self.__class__.auto_doc_id: {'lead': self.__class__.series2['lead'], 'released': self.__class__.series2['released']}}]
+	async def test_collection_get_select(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').select(['lead.name', 'released']).get() == [{'003': {'lead': self.__class__.series1['lead'], 'released': self.__class__.series1['released']}}, {self.__class__.auto_doc_id: {'lead': self.__class__.series2['lead'], 'released': self.__class__.series2['released']}}]
 
-	async def test_collection_get_offset(self, ds):
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').order_by('year').offset(1).get() == [{self.__class__.auto_doc_id: self.__class__.series2}]
+	async def test_collection_get_offset(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').order_by('year').offset(1).get() == [{self.__class__.auto_doc_id: self.__class__.series2}]
 
-	async def test_collection_get_limit_to_first(self, ds):
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').order_by('year').limit_to_first(1).get() == [{'003': self.__class__.series1}]
+	async def test_collection_get_limit_to_first(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').order_by('year').limit_to_first(1).get() == [{'003': self.__class__.series1}]
 
-	async def test_collection_get_limit_to_last(self, ds):
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').order_by('year').limit_to_last(1).get() == [{'003': self.__class__.series1}]
+	async def test_collection_get_limit_to_last(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').order_by('year').limit_to_last(1).get() == [{'003': self.__class__.series1}]
 
-	async def test_collection_get_end_at(self, ds):
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').order_by('year').end_at({'year': 2010}).get() == []
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').order_by('year').end_at({'year': 2021}).get() == [{'003': self.__class__.series1}]
+	async def test_collection_get_end_at(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').order_by('year').end_at({'year': 2010}).get() == []
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').order_by('year').end_at({'year': 2021}).get() == [{'003': self.__class__.series1}]
 
-	async def test_collection_get_end_before(self, ds):
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').order_by('year').end_before({'year': 2023}).get() == [{'003': self.__class__.series1}, {self.__class__.auto_doc_id: self.__class__.series2}]
+	async def test_collection_get_end_before(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').order_by('year').end_before({'year': 2023}).get() == [{'003': self.__class__.series1}, {self.__class__.auto_doc_id: self.__class__.series2}]
 
-	async def test_collection_get_where(self, ds):
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').where('lead.name', 'in',  ['Benedict Cumberbatch', 'Robert Downey Jr.']).get() == []
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').where('rating', '<=', 8.0).get() == [{self.__class__.auto_doc_id: self.__class__.series2}]
+	async def test_collection_get_where(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').where('lead.name', 'in',  ['Benedict Cumberbatch', 'Robert Downey Jr.']).get() == []
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').where('rating', '<=', 8.0).get() == [{self.__class__.auto_doc_id: self.__class__.series2}]
 
-	async def test_manual_doc_update(self, ds):
+	async def test_manual_doc_update(self, ds, test_collection):
 		update_data = {'released': True}
 
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').document('003').update(update_data) is None
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').document('003').get(field_paths=['released']) == update_data
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').document('003').update(update_data) is None
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').document('003').get(field_paths=['released']) == update_data
 
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').document(self.__class__.auto_doc_id).update(update_data) is None
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').document(self.__class__.auto_doc_id).get(field_paths=['released']) == update_data
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').document(self.__class__.auto_doc_id).update(update_data) is None
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').document(self.__class__.auto_doc_id).get(field_paths=['released']) == update_data
 
-	async def test_manual_doc_delete(self, ds):
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').document('003').delete() is None
-		assert await ds.collection('Marvels').document('Series').collection('PhaseFour').document(self.__class__.auto_doc_id).delete() is None
+	async def test_manual_doc_delete(self, ds, test_collection):
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').document('003').delete() is None
+		assert await ds.collection(test_collection).document('Series').collection('PhaseFour').document(self.__class__.auto_doc_id).delete() is None
```

### Comparing `async_firebase_rest_api-2.0.1/tests/test_setup.py` & `async_firebase_rest_api-2.1.0/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/tests/test_storage.py` & `async_firebase_rest_api-2.1.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `async_firebase_rest_api-2.0.1/PKG-INFO` & `async_firebase_rest_api-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-firebase-rest-api
-Version: 2.0.1
+Version: 2.1.0
 Summary: An async python wrapper for Google's Firebase REST API's.
 Keywords: firebase,firebase-auth,firebase-database,firebase-firestore,firebase-realtime-database,firebase-storage
 Author-email: Asif Arman Rahman <asifarmanrahman@gmail.com>, Matias Kotlik <mdkotlik@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: async-firebase-rest-api Version: 2.0.1 Summary: An
+Metadata-Version: 2.1 Name: async-firebase-rest-api Version: 2.1.0 Summary: An
 async python wrapper for Google's Firebase REST API's. Keywords:
 firebase,firebase-auth,firebase-database,firebase-firestore,firebase-realtime-
 database,firebase-storage Author-email: Asif Arman Rahman
 gmail.com>, Matias Kotlik
 gmail.com> Requires-Python: >=3.11 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```


# Comparing `tmp/python_connector_test-1.0.0.tar.gz` & `tmp/python-connector-test-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_connector_test-1.0.0.tar", last modified: Sun Apr 21 13:39:04 2024, max compression
+gzip compressed data, was "python-connector-test-1.0.1.tar", last modified: Sun Apr 21 13:37:04 2024, max compression
```

## Comparing `python_connector_test-1.0.0.tar` & `python-connector-test-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-21 13:39:04.710045 python_connector_test-1.0.0/
--rw-r--r--   0 dima       (501) staff       (20)     1065 2024-04-19 21:19:47.000000 python_connector_test-1.0.0/LICENSE
--rw-r--r--   0 dima       (501) staff       (20)     6385 2024-04-21 13:39:04.710144 python_connector_test-1.0.0/PKG-INFO
--rw-r--r--   0 dima       (501) staff       (20)     5866 2024-04-21 12:40:28.000000 python_connector_test-1.0.0/README.md
-drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-21 13:39:04.705151 python_connector_test-1.0.0/python-connector/
--rw-r--r--   0 dima       (501) staff       (20)        0 2024-04-21 12:36:33.000000 python_connector_test-1.0.0/python-connector/__init__.py
-drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-21 13:39:04.706626 python_connector_test-1.0.0/python-connector/examples/
--rw-r--r--   0 dima       (501) staff       (20)        0 2024-04-21 12:38:01.000000 python_connector_test-1.0.0/python-connector/examples/__init__.py
--rw-r--r--   0 dima       (501) staff       (20)     1823 2024-04-21 12:38:17.000000 python_connector_test-1.0.0/python-connector/examples/add_password.py
--rw-r--r--   0 dima       (501) staff       (20)      503 2024-04-21 12:38:17.000000 python_connector_test-1.0.0/python-connector/examples/delete_password.py
--rw-r--r--   0 dima       (501) staff       (20)     1706 2024-04-21 12:38:17.000000 python_connector_test-1.0.0/python-connector/examples/get_password.py
--rw-r--r--   0 dima       (501) staff       (20)      992 2024-04-21 12:38:17.000000 python_connector_test-1.0.0/python-connector/examples/search_password.py
--rw-r--r--   0 dima       (501) staff       (20)       42 2024-04-21 12:42:08.000000 python_connector_test-1.0.0/python-connector/main.py
--rw-r--r--   0 dima       (501) staff       (20)     6768 2024-04-19 21:19:47.000000 python_connector_test-1.0.0/python-connector/passwork_api.py
-drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-21 13:39:04.707703 python_connector_test-1.0.0/python-connector/rest_modules/
--rw-r--r--   0 dima       (501) staff       (20)     1056 2024-04-19 21:19:47.000000 python_connector_test-1.0.0/python-connector/rest_modules/__init__.py
--rw-r--r--   0 dima       (501) staff       (20)     3855 2024-04-21 12:38:17.000000 python_connector_test-1.0.0/python-connector/rest_modules/passwords.py
--rw-r--r--   0 dima       (501) staff       (20)     1468 2024-04-21 12:38:17.000000 python_connector_test-1.0.0/python-connector/rest_modules/users.py
--rw-r--r--   0 dima       (501) staff       (20)      437 2024-04-21 12:38:17.000000 python_connector_test-1.0.0/python-connector/rest_modules/vaults.py
--rw-r--r--   0 dima       (501) staff       (20)     1106 2024-04-21 12:23:18.000000 python_connector_test-1.0.0/python-connector/session_options.py
-drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-21 13:39:04.709027 python_connector_test-1.0.0/python-connector/utils/
--rw-r--r--   0 dima       (501) staff       (20)      116 2024-04-19 21:19:47.000000 python_connector_test-1.0.0/python-connector/utils/__init__.py
--rw-r--r--   0 dima       (501) staff       (20)     3954 2024-04-19 21:19:47.000000 python_connector_test-1.0.0/python-connector/utils/base32.py
--rw-r--r--   0 dima       (501) staff       (20)     3206 2024-04-21 12:38:17.000000 python_connector_test-1.0.0/python-connector/utils/crypto_file.py
--rw-r--r--   0 dima       (501) staff       (20)     4274 2024-04-21 12:38:17.000000 python_connector_test-1.0.0/python-connector/utils/crypto_interface.py
--rw-r--r--   0 dima       (501) staff       (20)     3066 2024-04-21 12:38:17.000000 python_connector_test-1.0.0/python-connector/utils/passwork_utils.py
-drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-21 13:39:04.709895 python_connector_test-1.0.0/python_connector_test.egg-info/
--rw-r--r--   0 dima       (501) staff       (20)     6385 2024-04-21 13:39:04.000000 python_connector_test-1.0.0/python_connector_test.egg-info/PKG-INFO
--rw-r--r--   0 dima       (501) staff       (20)      949 2024-04-21 13:39:04.000000 python_connector_test-1.0.0/python_connector_test.egg-info/SOURCES.txt
--rw-r--r--   0 dima       (501) staff       (20)        1 2024-04-21 13:39:04.000000 python_connector_test-1.0.0/python_connector_test.egg-info/dependency_links.txt
--rw-r--r--   0 dima       (501) staff       (20)       52 2024-04-21 13:39:04.000000 python_connector_test-1.0.0/python_connector_test.egg-info/requires.txt
--rw-r--r--   0 dima       (501) staff       (20)       17 2024-04-21 13:39:04.000000 python_connector_test-1.0.0/python_connector_test.egg-info/top_level.txt
--rw-r--r--   0 dima       (501) staff       (20)       38 2024-04-21 13:39:04.710415 python_connector_test-1.0.0/setup.cfg
--rw-r--r--   0 dima       (501) staff       (20)      854 2024-04-21 13:39:02.000000 python_connector_test-1.0.0/setup.py
+drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-21 13:37:04.185196 python-connector-test-1.0.1/
+-rw-r--r--   0 dima       (501) staff       (20)     1065 2024-04-19 21:19:47.000000 python-connector-test-1.0.1/LICENSE
+-rw-r--r--   0 dima       (501) staff       (20)     6385 2024-04-21 13:37:04.185287 python-connector-test-1.0.1/PKG-INFO
+-rw-r--r--   0 dima       (501) staff       (20)     5866 2024-04-21 12:40:28.000000 python-connector-test-1.0.1/README.md
+drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-21 13:37:04.179830 python-connector-test-1.0.1/python-connector/
+-rw-r--r--   0 dima       (501) staff       (20)        0 2024-04-21 12:36:33.000000 python-connector-test-1.0.1/python-connector/__init__.py
+drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-21 13:37:04.181057 python-connector-test-1.0.1/python-connector/examples/
+-rw-r--r--   0 dima       (501) staff       (20)        0 2024-04-21 12:38:01.000000 python-connector-test-1.0.1/python-connector/examples/__init__.py
+-rw-r--r--   0 dima       (501) staff       (20)     1823 2024-04-21 12:38:17.000000 python-connector-test-1.0.1/python-connector/examples/add_password.py
+-rw-r--r--   0 dima       (501) staff       (20)      503 2024-04-21 12:38:17.000000 python-connector-test-1.0.1/python-connector/examples/delete_password.py
+-rw-r--r--   0 dima       (501) staff       (20)     1706 2024-04-21 12:38:17.000000 python-connector-test-1.0.1/python-connector/examples/get_password.py
+-rw-r--r--   0 dima       (501) staff       (20)      992 2024-04-21 12:38:17.000000 python-connector-test-1.0.1/python-connector/examples/search_password.py
+-rw-r--r--   0 dima       (501) staff       (20)       42 2024-04-21 12:42:08.000000 python-connector-test-1.0.1/python-connector/main.py
+-rw-r--r--   0 dima       (501) staff       (20)     6768 2024-04-19 21:19:47.000000 python-connector-test-1.0.1/python-connector/passwork_api.py
+drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-21 13:37:04.182301 python-connector-test-1.0.1/python-connector/rest_modules/
+-rw-r--r--   0 dima       (501) staff       (20)     1056 2024-04-19 21:19:47.000000 python-connector-test-1.0.1/python-connector/rest_modules/__init__.py
+-rw-r--r--   0 dima       (501) staff       (20)     3855 2024-04-21 12:38:17.000000 python-connector-test-1.0.1/python-connector/rest_modules/passwords.py
+-rw-r--r--   0 dima       (501) staff       (20)     1468 2024-04-21 12:38:17.000000 python-connector-test-1.0.1/python-connector/rest_modules/users.py
+-rw-r--r--   0 dima       (501) staff       (20)      437 2024-04-21 12:38:17.000000 python-connector-test-1.0.1/python-connector/rest_modules/vaults.py
+-rw-r--r--   0 dima       (501) staff       (20)     1106 2024-04-21 12:23:18.000000 python-connector-test-1.0.1/python-connector/session_options.py
+drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-21 13:37:04.184008 python-connector-test-1.0.1/python-connector/utils/
+-rw-r--r--   0 dima       (501) staff       (20)      116 2024-04-19 21:19:47.000000 python-connector-test-1.0.1/python-connector/utils/__init__.py
+-rw-r--r--   0 dima       (501) staff       (20)     3954 2024-04-19 21:19:47.000000 python-connector-test-1.0.1/python-connector/utils/base32.py
+-rw-r--r--   0 dima       (501) staff       (20)     3206 2024-04-21 12:38:17.000000 python-connector-test-1.0.1/python-connector/utils/crypto_file.py
+-rw-r--r--   0 dima       (501) staff       (20)     4274 2024-04-21 12:38:17.000000 python-connector-test-1.0.1/python-connector/utils/crypto_interface.py
+-rw-r--r--   0 dima       (501) staff       (20)     3066 2024-04-21 12:38:17.000000 python-connector-test-1.0.1/python-connector/utils/passwork_utils.py
+drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-21 13:37:04.185024 python-connector-test-1.0.1/python_connector_test.egg-info/
+-rw-r--r--   0 dima       (501) staff       (20)     6385 2024-04-21 13:37:04.000000 python-connector-test-1.0.1/python_connector_test.egg-info/PKG-INFO
+-rw-r--r--   0 dima       (501) staff       (20)      949 2024-04-21 13:37:04.000000 python-connector-test-1.0.1/python_connector_test.egg-info/SOURCES.txt
+-rw-r--r--   0 dima       (501) staff       (20)        1 2024-04-21 13:37:04.000000 python-connector-test-1.0.1/python_connector_test.egg-info/dependency_links.txt
+-rw-r--r--   0 dima       (501) staff       (20)       52 2024-04-21 13:37:04.000000 python-connector-test-1.0.1/python_connector_test.egg-info/requires.txt
+-rw-r--r--   0 dima       (501) staff       (20)       17 2024-04-21 13:37:04.000000 python-connector-test-1.0.1/python_connector_test.egg-info/top_level.txt
+-rw-r--r--   0 dima       (501) staff       (20)       38 2024-04-21 13:37:04.185530 python-connector-test-1.0.1/setup.cfg
+-rw-r--r--   0 dima       (501) staff       (20)      854 2024-04-21 13:37:01.000000 python-connector-test-1.0.1/setup.py
```

### Comparing `python_connector_test-1.0.0/LICENSE` & `python-connector-test-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_connector_test-1.0.0/PKG-INFO` & `python-connector-test-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: python_connector_test
-Version: 1.0.0
+Name: python-connector-test
+Version: 1.0.1
 Summary: Test module
 Home-page: https://github.com/dimavladimirov/mini_connector
 Author: dimavladimirov
 Author-email: vladimirovdmitry@mail.ru
 Project-URL: Documentation, https:/www.google.com
 Keywords: example python
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `python_connector_test-1.0.0/README.md` & `python-connector-test-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `python_connector_test-1.0.0/python-connector/examples/add_password.py` & `python-connector-test-1.0.1/python-connector/examples/add_password.py`

 * *Files identical despite different names*

### Comparing `python_connector_test-1.0.0/python-connector/examples/get_password.py` & `python-connector-test-1.0.1/python-connector/examples/get_password.py`

 * *Files identical despite different names*

### Comparing `python_connector_test-1.0.0/python-connector/examples/search_password.py` & `python-connector-test-1.0.1/python-connector/examples/search_password.py`

 * *Files identical despite different names*

### Comparing `python_connector_test-1.0.0/python-connector/passwork_api.py` & `python-connector-test-1.0.1/python-connector/passwork_api.py`

 * *Files identical despite different names*

### Comparing `python_connector_test-1.0.0/python-connector/rest_modules/__init__.py` & `python-connector-test-1.0.1/python-connector/rest_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `python_connector_test-1.0.0/python-connector/rest_modules/passwords.py` & `python-connector-test-1.0.1/python-connector/rest_modules/passwords.py`

 * *Files identical despite different names*

### Comparing `python_connector_test-1.0.0/python-connector/rest_modules/users.py` & `python-connector-test-1.0.1/python-connector/rest_modules/users.py`

 * *Files identical despite different names*

### Comparing `python_connector_test-1.0.0/python-connector/session_options.py` & `python-connector-test-1.0.1/python-connector/session_options.py`

 * *Files identical despite different names*

### Comparing `python_connector_test-1.0.0/python-connector/utils/base32.py` & `python-connector-test-1.0.1/python-connector/utils/base32.py`

 * *Files identical despite different names*

### Comparing `python_connector_test-1.0.0/python-connector/utils/crypto_file.py` & `python-connector-test-1.0.1/python-connector/utils/crypto_file.py`

 * *Files identical despite different names*

### Comparing `python_connector_test-1.0.0/python-connector/utils/crypto_interface.py` & `python-connector-test-1.0.1/python-connector/utils/crypto_interface.py`

 * *Files identical despite different names*

### Comparing `python_connector_test-1.0.0/python-connector/utils/passwork_utils.py` & `python-connector-test-1.0.1/python-connector/utils/passwork_utils.py`

 * *Files identical despite different names*

### Comparing `python_connector_test-1.0.0/python_connector_test.egg-info/PKG-INFO` & `python-connector-test-1.0.1/python_connector_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-connector-test
-Version: 1.0.0
+Version: 1.0.1
 Summary: Test module
 Home-page: https://github.com/dimavladimirov/mini_connector
 Author: dimavladimirov
 Author-email: vladimirovdmitry@mail.ru
 Project-URL: Documentation, https:/www.google.com
 Keywords: example python
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `python_connector_test-1.0.0/python_connector_test.egg-info/SOURCES.txt` & `python-connector-test-1.0.1/python_connector_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_connector_test-1.0.0/setup.py` & `python-connector-test-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
-    name='python_connector_test',
-    version='1.0.0',
+    name='python-connector-test',
+    version='1.0.1',
     author='dimavladimirov',
     author_email='vladimirovdmitry@mail.ru',
     description='Test module',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/dimavladimirov/mini_connector',
     packages=find_packages(),
```


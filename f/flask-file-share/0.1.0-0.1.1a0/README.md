# Comparing `tmp/flask_file_share-0.1.0.tar.gz` & `tmp/flask_file_share-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_file_share-0.1.0.tar", max compression
+gzip compressed data, was "flask_file_share-0.1.1a0.tar", max compression
```

## Comparing `flask_file_share-0.1.0.tar` & `flask_file_share-0.1.1a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     7677 2024-04-21 02:32:54.745636 flask_file_share-0.1.0/README.md
--rw-r--r--   0        0        0     1784 2024-04-21 04:58:18.814195 flask_file_share-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      192 2024-04-21 04:51:11.634967 flask_file_share-0.1.0/src/flask_file_share/__init__.py
--rw-r--r--   0        0        0      388 2024-04-21 04:23:31.800405 flask_file_share-0.1.0/src/flask_file_share/app.py
--rw-r--r--   0        0        0     8111 2024-04-21 04:34:58.592036 flask_file_share-0.1.0/src/flask_file_share/cli.py
--rw-r--r--   0        0        0     8013 2024-04-21 04:41:16.868501 flask_file_share-0.1.0/src/flask_file_share/client.py
--rw-r--r--   0        0        0     2218 2024-04-21 04:22:24.651206 flask_file_share-0.1.0/src/flask_file_share/main.py
--rw-r--r--   0        0        0     4296 2024-04-21 04:35:26.588392 flask_file_share-0.1.0/src/flask_file_share/settings.py
--rw-r--r--   0        0        0      172 2024-04-21 04:31:16.429607 flask_file_share-0.1.0/src/flask_file_share/utils/__init__.py
--rw-r--r--   0        0        0      599 2024-04-21 04:23:30.668388 flask_file_share-0.1.0/src/flask_file_share/utils/mimetype.py
--rw-r--r--   0        0        0      680 2024-04-21 03:52:40.222975 flask_file_share-0.1.0/src/flask_file_share/utils/slugify.py
--rw-r--r--   0        0        0      914 2024-04-21 04:23:30.672389 flask_file_share-0.1.0/src/flask_file_share/utils/zip.py
--rw-r--r--   0        0        0      390 2024-04-21 04:31:19.797642 flask_file_share-0.1.0/src/flask_file_share/web/__init__.py
--rw-r--r--   0        0        0     3451 2024-04-21 04:34:14.623464 flask_file_share-0.1.0/src/flask_file_share/web/auth.py
--rw-r--r--   0        0        0     1030 2024-04-21 04:14:17.646265 flask_file_share-0.1.0/src/flask_file_share/web/config.py
--rw-r--r--   0        0        0     8844 2024-04-21 04:52:11.864058 flask_file_share-0.1.0/src/flask_file_share/web/routes.py
--rw-r--r--   0        0        0     4702 2024-04-21 04:33:50.995218 flask_file_share-0.1.0/src/flask_file_share/web/utils.py
--rw-r--r--   0        0        0      944 2024-04-21 04:34:37.655765 flask_file_share-0.1.0/src/flask_file_share/web/views.py
--rw-r--r--   0        0        0     9087 1970-01-01 00:00:00.000000 flask_file_share-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7677 2024-04-21 02:32:54.745636 flask_file_share-0.1.1a0/README.md
+-rw-r--r--   0        0        0     1607 2024-04-21 04:59:54.231610 flask_file_share-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0      192 2024-04-21 04:51:11.634967 flask_file_share-0.1.1a0/src/flask_file_share/__init__.py
+-rw-r--r--   0        0        0      388 2024-04-21 04:23:31.800405 flask_file_share-0.1.1a0/src/flask_file_share/app.py
+-rw-r--r--   0        0        0     8111 2024-04-21 04:34:58.592036 flask_file_share-0.1.1a0/src/flask_file_share/cli.py
+-rw-r--r--   0        0        0     8013 2024-04-21 04:41:16.868501 flask_file_share-0.1.1a0/src/flask_file_share/client.py
+-rw-r--r--   0        0        0     2218 2024-04-21 04:22:24.651206 flask_file_share-0.1.1a0/src/flask_file_share/main.py
+-rw-r--r--   0        0        0     4296 2024-04-21 04:35:26.588392 flask_file_share-0.1.1a0/src/flask_file_share/settings.py
+-rw-r--r--   0        0        0      172 2024-04-21 04:31:16.429607 flask_file_share-0.1.1a0/src/flask_file_share/utils/__init__.py
+-rw-r--r--   0        0        0      599 2024-04-21 04:23:30.668388 flask_file_share-0.1.1a0/src/flask_file_share/utils/mimetype.py
+-rw-r--r--   0        0        0      680 2024-04-21 03:52:40.222975 flask_file_share-0.1.1a0/src/flask_file_share/utils/slugify.py
+-rw-r--r--   0        0        0      914 2024-04-21 04:23:30.672389 flask_file_share-0.1.1a0/src/flask_file_share/utils/zip.py
+-rw-r--r--   0        0        0      390 2024-04-21 04:31:19.797642 flask_file_share-0.1.1a0/src/flask_file_share/web/__init__.py
+-rw-r--r--   0        0        0     3451 2024-04-21 04:34:14.623464 flask_file_share-0.1.1a0/src/flask_file_share/web/auth.py
+-rw-r--r--   0        0        0     1030 2024-04-21 04:14:17.646265 flask_file_share-0.1.1a0/src/flask_file_share/web/config.py
+-rw-r--r--   0        0        0     8844 2024-04-21 04:52:11.864058 flask_file_share-0.1.1a0/src/flask_file_share/web/routes.py
+-rw-r--r--   0        0        0     4702 2024-04-21 04:33:50.995218 flask_file_share-0.1.1a0/src/flask_file_share/web/utils.py
+-rw-r--r--   0        0        0      944 2024-04-21 04:34:37.655765 flask_file_share-0.1.1a0/src/flask_file_share/web/views.py
+-rw-r--r--   0        0        0     9039 1970-01-01 00:00:00.000000 flask_file_share-0.1.1a0/PKG-INFO
```

### Comparing `flask_file_share-0.1.0/README.md` & `flask_file_share-0.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.0/pyproject.toml` & `flask_file_share-0.1.1a0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask-file-share"
-version = "0.1.0"
+version = "0.1.1a0"
 description = "Flask-based file sharing with web interface, API, and CLI app"
 authors = ["hermann-web <hermannagossou6@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {from = "src", include = "flask_file_share"}
 ]
@@ -15,18 +15,14 @@
 repository = "https://github.com/Hermann-web/simple-file-hosting-with-flask"
 documentation = "https://flask-file-share.readthedocs.io"
 keywords = ["flask", "file sharing", "web interface", "API", "CLI"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
     "Framework :: Flask",
     "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `flask_file_share-0.1.0/src/flask_file_share/cli.py` & `flask_file_share-0.1.1a0/src/flask_file_share/cli.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.0/src/flask_file_share/client.py` & `flask_file_share-0.1.1a0/src/flask_file_share/client.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.0/src/flask_file_share/main.py` & `flask_file_share-0.1.1a0/src/flask_file_share/main.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.0/src/flask_file_share/settings.py` & `flask_file_share-0.1.1a0/src/flask_file_share/settings.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.0/src/flask_file_share/utils/mimetype.py` & `flask_file_share-0.1.1a0/src/flask_file_share/utils/mimetype.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.0/src/flask_file_share/utils/slugify.py` & `flask_file_share-0.1.1a0/src/flask_file_share/utils/slugify.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.0/src/flask_file_share/utils/zip.py` & `flask_file_share-0.1.1a0/src/flask_file_share/utils/zip.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.0/src/flask_file_share/web/auth.py` & `flask_file_share-0.1.1a0/src/flask_file_share/web/auth.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.0/src/flask_file_share/web/config.py` & `flask_file_share-0.1.1a0/src/flask_file_share/web/config.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.0/src/flask_file_share/web/routes.py` & `flask_file_share-0.1.1a0/src/flask_file_share/web/routes.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.0/src/flask_file_share/web/utils.py` & `flask_file_share-0.1.1a0/src/flask_file_share/web/utils.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.0/src/flask_file_share/web/views.py` & `flask_file_share-0.1.1a0/src/flask_file_share/web/views.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.0/PKG-INFO` & `flask_file_share-0.1.1a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-file-share
-Version: 0.1.0
+Version: 0.1.1a0
 Summary: Flask-based file sharing with web interface, API, and CLI app
 Home-page: https://github.com/Hermann-web/simple-file-hosting-with-flask
 License: MIT
 Keywords: flask,file sharing,web interface,API,CLI
 Author: hermann-web
 Author-email: hermannagossou6@gmail.com
 Maintainer: Hermann Agossou
@@ -15,15 +15,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Flask (>=3.0.3,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-slugify (>=8.0.4,<9.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Documentation, https://flask-file-share.readthedocs.io
```


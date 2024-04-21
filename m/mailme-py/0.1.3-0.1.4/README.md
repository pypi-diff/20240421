# Comparing `tmp/mailme-py-0.1.3.tar.gz` & `tmp/mailme-py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mailme-py-0.1.3.tar", last modified: Wed Jan 17 22:55:40 2024, max compression
+gzip compressed data, was "dist/mailme-py-0.1.4.tar", last modified: Sun Apr 21 07:36:46 2024, max compression
```

## Comparing `mailme-py-0.1.3.tar` & `mailme-py-0.1.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 22:55:40.000000 mailme-py-0.1.3/
--rw-r--r--   0 root         (0) root         (0)     1262 2024-01-17 22:55:40.000000 mailme-py-0.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-17 22:55:40.000000 mailme-py-0.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1941 2024-01-17 22:55:28.000000 mailme-py-0.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 22:55:40.000000 mailme-py-0.1.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 22:55:40.000000 mailme-py-0.1.3/src/mailme/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 22:55:40.000000 mailme-py-0.1.3/src/mailme/controllers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 22:55:40.000000 mailme-py-0.1.3/src/mailme/controllers/api/
--rw-r--r--   0 root         (0) root         (0)     1691 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/controllers/api/base.py
--rw-r--r--   0 root         (0) root         (0)      105 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/controllers/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 22:55:40.000000 mailme-py-0.1.3/src/mailme/controllers/web/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/controllers/web/base.py
--rw-r--r--   0 root         (0) root         (0)      159 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/controllers/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1848 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/controllers/web/admin.py
--rw-r--r--   0 root         (0) root         (0)      126 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/controllers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 22:55:40.000000 mailme-py-0.1.3/src/mailme/models/
--rw-r--r--   0 root         (0) root         (0)      136 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/models/base.py
--rw-r--r--   0 root         (0) root         (0)     2400 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/models/message.py
--rw-r--r--   0 root         (0) root         (0)      151 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      197 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 22:55:40.000000 mailme-py-0.1.3/src/mailme/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 22:55:40.000000 mailme-py-0.1.3/src/mailme/templates/styles/
--rw-r--r--   0 root         (0) root         (0)     3228 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/templates/styles/dark.html.tpl
--rw-r--r--   0 root         (0) root         (0)     3101 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/templates/styles/base.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 22:55:40.000000 mailme-py-0.1.3/src/mailme/templates/admin/
--rw-r--r--   0 root         (0) root         (0)     3675 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/templates/admin/applier.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 22:55:40.000000 mailme-py-0.1.3/src/mailme/templates/email/
--rw-r--r--   0 root         (0) root         (0)      736 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/templates/email/macros.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1333 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/templates/email/layout.inline.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1684 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/templates/email/layout.html.tpl
--rw-r--r--   0 root         (0) root         (0)      577 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/templates/email/base.inline.html.tpl
--rw-r--r--   0 root         (0) root         (0)     2106 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/templates/email/test.html.tpl
--rw-r--r--   0 root         (0) root         (0)      461 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/templates/email/base.html.tpl
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-17 22:55:28.000000 mailme-py-0.1.3/src/mailme/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 22:55:40.000000 mailme-py-0.1.3/src/mailme_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1262 2024-01-17 22:55:40.000000 mailme-py-0.1.3/src/mailme_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-17 22:55:40.000000 mailme-py-0.1.3/src/mailme_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      978 2024-01-17 22:55:40.000000 mailme-py-0.1.3/src/mailme_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-17 22:55:37.000000 mailme-py-0.1.3/src/mailme_py.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       43 2024-01-17 22:55:40.000000 mailme-py-0.1.3/src/mailme_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-01-17 22:55:40.000000 mailme-py-0.1.3/src/mailme_py.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1222 2024-01-17 22:55:28.000000 mailme-py-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 07:36:46.000000 mailme-py-0.1.4/
+-rw-r--r--   0 root         (0) root         (0)     1941 2024-04-21 07:36:34.000000 mailme-py-0.1.4/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2024-04-21 07:36:34.000000 mailme-py-0.1.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-21 07:36:46.000000 mailme-py-0.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1262 2024-04-21 07:36:46.000000 mailme-py-0.1.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 07:36:46.000000 mailme-py-0.1.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 07:36:46.000000 mailme-py-0.1.4/src/mailme_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-21 07:36:46.000000 mailme-py-0.1.4/src/mailme_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      978 2024-04-21 07:36:46.000000 mailme-py-0.1.4/src/mailme_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-21 07:36:46.000000 mailme-py-0.1.4/src/mailme_py.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1262 2024-04-21 07:36:46.000000 mailme-py-0.1.4/src/mailme_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-21 07:36:46.000000 mailme-py-0.1.4/src/mailme_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-21 07:36:43.000000 mailme-py-0.1.4/src/mailme_py.egg-info/not-zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 07:36:46.000000 mailme-py-0.1.4/src/mailme/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 07:36:46.000000 mailme-py-0.1.4/src/mailme/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 07:36:46.000000 mailme-py-0.1.4/src/mailme/templates/styles/
+-rw-r--r--   0 root         (0) root         (0)     3228 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/templates/styles/dark.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     3101 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/templates/styles/base.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 07:36:46.000000 mailme-py-0.1.4/src/mailme/templates/email/
+-rw-r--r--   0 root         (0) root         (0)     1333 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/templates/email/layout.inline.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      577 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/templates/email/base.inline.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      736 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/templates/email/macros.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     2106 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/templates/email/test.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1684 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/templates/email/layout.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      461 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/templates/email/base.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 07:36:46.000000 mailme-py-0.1.4/src/mailme/templates/admin/
+-rw-r--r--   0 root         (0) root         (0)     3675 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/templates/admin/applier.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      197 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 07:36:46.000000 mailme-py-0.1.4/src/mailme/controllers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 07:36:46.000000 mailme-py-0.1.4/src/mailme/controllers/api/
+-rw-r--r--   0 root         (0) root         (0)     1691 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/controllers/api/base.py
+-rw-r--r--   0 root         (0) root         (0)      105 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/controllers/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 07:36:46.000000 mailme-py-0.1.4/src/mailme/controllers/web/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/controllers/web/base.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/controllers/web/admin.py
+-rw-r--r--   0 root         (0) root         (0)      159 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/controllers/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      126 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/controllers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 07:36:46.000000 mailme-py-0.1.4/src/mailme/models/
+-rw-r--r--   0 root         (0) root         (0)      136 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/models/base.py
+-rw-r--r--   0 root         (0) root         (0)      151 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2024-04-21 07:36:34.000000 mailme-py-0.1.4/src/mailme/models/message.py
```

### Comparing `mailme-py-0.1.3/PKG-INFO` & `mailme-py-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mailme-py
-Version: 0.1.3
+Version: 0.1.4
 Summary: Mailme
 Home-page: http://pushi.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Keywords: mailme smtp service
```

### Comparing `mailme-py-0.1.3/setup.py` & `mailme-py-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 import os
 import setuptools
 
 setuptools.setup(
     name="mailme-py",
-    version="0.1.3",
+    version="0.1.4",
     author="Hive Solutions Lda.",
     author_email="development@hive.pt",
     description="Mailme",
     license="Apache License, Version 2.0",
     keywords="mailme smtp service",
     url="http://pushi.hive.pt",
     zip_safe=False,
```

### Comparing `mailme-py-0.1.3/src/mailme/controllers/api/base.py` & `mailme-py-0.1.4/src/mailme/controllers/api/base.py`

 * *Files identical despite different names*

### Comparing `mailme-py-0.1.3/src/mailme/controllers/web/base.py` & `mailme-py-0.1.4/src/mailme/controllers/web/base.py`

 * *Files identical despite different names*

### Comparing `mailme-py-0.1.3/src/mailme/controllers/web/admin.py` & `mailme-py-0.1.4/src/mailme/controllers/web/admin.py`

 * *Files identical despite different names*

### Comparing `mailme-py-0.1.3/src/mailme/models/message.py` & `mailme-py-0.1.4/src/mailme/models/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,18 @@
 
     title = appier.field()
 
     subtitle = appier.field()
 
     contents = appier.field()
 
+    html = appier.field()
+
+    plain = appier.field()
+
     copyright = appier.field()
 
     logo_url = appier.field(meta="url")
 
     @classmethod
     def validate(cls):
         return super(Message, cls).validate() + [
@@ -77,11 +81,13 @@
             style=self.style or "base",
             mode=self.mode or "markdown",
             subject=self.subject or "Test email",
             attachments=self.attachments if self.attachments else [],
             title=self.title or self.subject or "Test email",
             subtitle=self.subtitle,
             contents=self.contents,
+            html=self.html,
+            plain=self.plain,
             copyright=self.copyright,
             logo_url=self.logo_url or None,
             **kwargs
         )
```

### Comparing `mailme-py-0.1.3/src/mailme/templates/styles/dark.html.tpl` & `mailme-py-0.1.4/src/mailme/templates/styles/dark.html.tpl`

 * *Files identical despite different names*

### Comparing `mailme-py-0.1.3/src/mailme/templates/styles/base.html.tpl` & `mailme-py-0.1.4/src/mailme/templates/styles/base.html.tpl`

 * *Files identical despite different names*

### Comparing `mailme-py-0.1.3/src/mailme/templates/admin/applier.html.tpl` & `mailme-py-0.1.4/src/mailme/templates/admin/applier.html.tpl`

 * *Files identical despite different names*

### Comparing `mailme-py-0.1.3/src/mailme/templates/email/macros.html.tpl` & `mailme-py-0.1.4/src/mailme/templates/email/macros.html.tpl`

 * *Files identical despite different names*

### Comparing `mailme-py-0.1.3/src/mailme/templates/email/layout.inline.html.tpl` & `mailme-py-0.1.4/src/mailme/templates/email/layout.inline.html.tpl`

 * *Files identical despite different names*

### Comparing `mailme-py-0.1.3/src/mailme/templates/email/layout.html.tpl` & `mailme-py-0.1.4/src/mailme/templates/email/layout.html.tpl`

 * *Files identical despite different names*

### Comparing `mailme-py-0.1.3/src/mailme/templates/email/base.inline.html.tpl` & `mailme-py-0.1.4/src/mailme/templates/email/base.inline.html.tpl`

 * *Files identical despite different names*

### Comparing `mailme-py-0.1.3/src/mailme/templates/email/test.html.tpl` & `mailme-py-0.1.4/src/mailme/templates/email/test.html.tpl`

 * *Files identical despite different names*

### Comparing `mailme-py-0.1.3/src/mailme_py.egg-info/PKG-INFO` & `mailme-py-0.1.4/src/mailme_py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mailme-py
-Version: 0.1.3
+Version: 0.1.4
 Summary: Mailme
 Home-page: http://pushi.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Keywords: mailme smtp service
```

### Comparing `mailme-py-0.1.3/src/mailme_py.egg-info/SOURCES.txt` & `mailme-py-0.1.4/src/mailme_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mailme-py-0.1.3/README.md` & `mailme-py-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# [Mailme](http://mailme.hive.pt)
+# [Mailme 📬](http://mailme.hive.pt)
 
 Simple REST HTTP service to send emails using a simple API.
 
 ## API
 
 ## API Routes
```


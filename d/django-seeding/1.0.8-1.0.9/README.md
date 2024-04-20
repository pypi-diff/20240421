# Comparing `tmp/django-seeding-1.0.8.tar.gz` & `tmp/django-seeding-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-seeding-1.0.8.tar", last modified: Wed Oct 25 12:41:53 2023, max compression
+gzip compressed data, was "django-seeding-1.0.9.tar", last modified: Wed Oct 25 12:44:45 2023, max compression
```

## Comparing `django-seeding-1.0.8.tar` & `django-seeding-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-10-25 12:41:53.291632 django-seeding-1.0.8/
--rw-rw-rw-   0        0        0     1090 2023-10-24 17:13:48.000000 django-seeding-1.0.8/LICENSE
--rw-rw-rw-   0        0        0    18076 2023-10-25 12:41:53.291632 django-seeding-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    17746 2023-10-25 12:41:30.000000 django-seeding-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-10-25 12:41:53.258219 django-seeding-1.0.8/django_seeding/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:34:12.000000 django-seeding-1.0.8/django_seeding/__init__.py
--rw-rw-rw-   0        0        0      160 2023-10-23 09:36:21.000000 django-seeding-1.0.8/django_seeding/admin.py
--rw-rw-rw-   0        0        0      307 2023-10-24 15:27:47.000000 django-seeding-1.0.8/django_seeding/apps.py
--rw-rw-rw-   0        0        0      421 2023-10-24 17:27:18.000000 django-seeding-1.0.8/django_seeding/asgi.py
--rw-rw-rw-   0        0        0      188 2023-10-23 09:36:29.000000 django-seeding-1.0.8/django_seeding/models.py
--rw-rw-rw-   0        0        0     3289 2023-10-24 16:18:02.000000 django-seeding-1.0.8/django_seeding/seeder_registry.py
--rw-rw-rw-   0        0        0    15208 2023-10-23 13:30:01.000000 django-seeding-1.0.8/django_seeding/seeders.py
--rw-rw-rw-   0        0        0     3368 2023-10-24 17:27:18.000000 django-seeding-1.0.8/django_seeding/settings.py
--rw-rw-rw-   0        0        0      792 2023-10-24 17:27:18.000000 django-seeding-1.0.8/django_seeding/urls.py
--rw-rw-rw-   0        0        0      421 2023-10-24 17:27:18.000000 django-seeding-1.0.8/django_seeding/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-10-25 12:41:53.291632 django-seeding-1.0.8/django_seeding.egg-info/
--rw-rw-rw-   0        0        0    18076 2023-10-25 12:41:53.000000 django-seeding-1.0.8/django_seeding.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2023-10-25 12:41:53.000000 django-seeding-1.0.8/django_seeding.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-25 12:41:53.000000 django-seeding-1.0.8/django_seeding.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-10-25 12:41:53.000000 django-seeding-1.0.8/django_seeding.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-10-25 12:41:53.000000 django-seeding-1.0.8/django_seeding.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-25 12:41:53.291632 django-seeding-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      489 2023-10-25 12:41:38.000000 django-seeding-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-25 12:44:45.025859 django-seeding-1.0.9/
+-rw-rw-rw-   0        0        0     1090 2023-10-24 17:13:48.000000 django-seeding-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0    17965 2023-10-25 12:44:45.025859 django-seeding-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    17637 2023-10-25 12:44:27.000000 django-seeding-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-10-25 12:44:44.994099 django-seeding-1.0.9/django_seeding/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:34:12.000000 django-seeding-1.0.9/django_seeding/__init__.py
+-rw-rw-rw-   0        0        0      160 2023-10-23 09:36:21.000000 django-seeding-1.0.9/django_seeding/admin.py
+-rw-rw-rw-   0        0        0      307 2023-10-24 15:27:47.000000 django-seeding-1.0.9/django_seeding/apps.py
+-rw-rw-rw-   0        0        0      421 2023-10-24 17:27:18.000000 django-seeding-1.0.9/django_seeding/asgi.py
+-rw-rw-rw-   0        0        0      188 2023-10-23 09:36:29.000000 django-seeding-1.0.9/django_seeding/models.py
+-rw-rw-rw-   0        0        0     3289 2023-10-24 16:18:02.000000 django-seeding-1.0.9/django_seeding/seeder_registry.py
+-rw-rw-rw-   0        0        0    15208 2023-10-23 13:30:01.000000 django-seeding-1.0.9/django_seeding/seeders.py
+-rw-rw-rw-   0        0        0     3368 2023-10-24 17:27:18.000000 django-seeding-1.0.9/django_seeding/settings.py
+-rw-rw-rw-   0        0        0      792 2023-10-24 17:27:18.000000 django-seeding-1.0.9/django_seeding/urls.py
+-rw-rw-rw-   0        0        0      421 2023-10-24 17:27:18.000000 django-seeding-1.0.9/django_seeding/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-10-25 12:44:45.025859 django-seeding-1.0.9/django_seeding.egg-info/
+-rw-rw-rw-   0        0        0    17965 2023-10-25 12:44:44.000000 django-seeding-1.0.9/django_seeding.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-10-25 12:44:44.000000 django-seeding-1.0.9/django_seeding.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-25 12:44:44.000000 django-seeding-1.0.9/django_seeding.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-10-25 12:44:44.000000 django-seeding-1.0.9/django_seeding.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-10-25 12:44:44.000000 django-seeding-1.0.9/django_seeding.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-10-25 12:44:45.025859 django-seeding-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      489 2023-10-25 12:44:35.000000 django-seeding-1.0.9/setup.py
```

### Comparing `django-seeding-1.0.8/LICENSE` & `django-seeding-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-seeding-1.0.8/PKG-INFO` & `django-seeding-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-seeding
-Version: 1.0.8
+Version: 1.0.9
 Summary: Simple Django Package that helps developer to seed data from files and codes into the database automatically
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django
 Requires-Dist: djangorestframework
 Requires-Dist: pandas
 
@@ -23,24 +23,16 @@
 [![pr][pr-shield]][contributing-url]
 [![hachtoberfest][hachtoberfest-shield]][hacktoberfest-url]
 [![license][license-shield]][license-url]
 
 
 <div align="center">
 <h3>Django Seeding</h3>
-
-[Report Bug][issues-url]
-    Â·
-[Request Feature][issues-url]
-
 </div>
 
-[![photo][photo-url]][demo-url]
-
-***
 
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Installation](#installation)
 - [Simple Example](#simple-example)
 - [Full Usage Documentation](#full-usage-documentation)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-seeding-1.0.8/README.md` & `django-seeding-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,16 @@
 [![pr][pr-shield]][contributing-url]
 [![hachtoberfest][hachtoberfest-shield]][hacktoberfest-url]
 [![license][license-shield]][license-url]
 
 
 <div align="center">
 <h3>Django Seeding</h3>
-
-[Report Bug][issues-url]
-    ·
-[Request Feature][issues-url]
-
 </div>
 
-[![photo][photo-url]][demo-url]
-
-***
 
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Installation](#installation)
 - [Simple Example](#simple-example)
 - [Full Usage Documentation](#full-usage-documentation)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-seeding-1.0.8/django_seeding/seeder_registry.py` & `django-seeding-1.0.9/django_seeding/seeder_registry.py`

 * *Files identical despite different names*

### Comparing `django-seeding-1.0.8/django_seeding/seeders.py` & `django-seeding-1.0.9/django_seeding/seeders.py`

 * *Files identical despite different names*

### Comparing `django-seeding-1.0.8/django_seeding/settings.py` & `django-seeding-1.0.9/django_seeding/settings.py`

 * *Files identical despite different names*

### Comparing `django-seeding-1.0.8/django_seeding/urls.py` & `django-seeding-1.0.9/django_seeding/urls.py`

 * *Files identical despite different names*

### Comparing `django-seeding-1.0.8/django_seeding.egg-info/PKG-INFO` & `django-seeding-1.0.9/django_seeding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-seeding
-Version: 1.0.8
+Version: 1.0.9
 Summary: Simple Django Package that helps developer to seed data from files and codes into the database automatically
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django
 Requires-Dist: djangorestframework
 Requires-Dist: pandas
 
@@ -23,24 +23,16 @@
 [![pr][pr-shield]][contributing-url]
 [![hachtoberfest][hachtoberfest-shield]][hacktoberfest-url]
 [![license][license-shield]][license-url]
 
 
 <div align="center">
 <h3>Django Seeding</h3>
-
-[Report Bug][issues-url]
-    Â·
-[Request Feature][issues-url]
-
 </div>
 
-[![photo][photo-url]][demo-url]
-
-***
 
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Installation](#installation)
 - [Simple Example](#simple-example)
 - [Full Usage Documentation](#full-usage-documentation)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```


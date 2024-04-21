# Comparing `tmp/django-click-2.3.0.tar.gz` & `tmp/django_click-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-click-2.3.0.tar", last modified: Tue Sep  7 19:34:46 2021, max compression
+gzip compressed data, was "django_click-2.4.0.tar", last modified: Sun Apr 21 17:10:27 2024, max compression
```

## Comparing `django-click-2.3.0.tar` & `django_click-2.4.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwx------   0 tallen   (86646) wrds     (60359)        0 2021-09-07 19:34:46.932597 django-click-2.3.0/
--rw-------   0 tallen   (86646) wrds     (60359)      119 2020-07-20 19:27:27.000000 django-click-2.3.0/.gitignore
--rw-------   0 tallen   (86646) wrds     (60359)      288 2021-09-07 19:34:15.000000 django-click-2.3.0/AUTHORS.rst
--rw-------   0 tallen   (86646) wrds     (60359)      948 2020-06-12 11:40:48.000000 django-click-2.3.0/CONTRIBUTING.rst
--rw-------   0 tallen   (86646) wrds     (60359)     1191 2020-06-15 13:46:31.000000 django-click-2.3.0/HISTORY.rst
--rw-------   0 tallen   (86646) wrds     (60359)     1066 2020-06-12 11:41:21.000000 django-click-2.3.0/LICENSE
--rw-------   0 tallen   (86646) wrds     (60359)      273 2020-06-12 11:40:48.000000 django-click-2.3.0/MANIFEST.in
--rw-------   0 tallen   (86646) wrds     (60359)     5296 2021-09-07 19:34:46.932597 django-click-2.3.0/PKG-INFO
--rw-------   0 tallen   (86646) wrds     (60359)     2171 2021-09-07 18:41:28.000000 django-click-2.3.0/README.rst
-drwx------   0 tallen   (86646) wrds     (60359)        0 2021-09-07 19:34:46.928597 django-click-2.3.0/django_click.egg-info/
--rw-------   0 tallen   (86646) wrds     (60359)     5296 2021-09-07 19:34:46.000000 django-click-2.3.0/django_click.egg-info/PKG-INFO
--rw-------   0 tallen   (86646) wrds     (60359)      432 2021-09-07 19:34:46.000000 django-click-2.3.0/django_click.egg-info/SOURCES.txt
--rw-------   0 tallen   (86646) wrds     (60359)        1 2021-09-07 19:34:46.000000 django-click-2.3.0/django_click.egg-info/dependency_links.txt
--rw-------   0 tallen   (86646) wrds     (60359)        1 2020-06-12 20:06:43.000000 django-click-2.3.0/django_click.egg-info/not-zip-safe
--rw-------   0 tallen   (86646) wrds     (60359)      203 2021-09-07 19:34:46.000000 django-click-2.3.0/django_click.egg-info/requires.txt
--rw-------   0 tallen   (86646) wrds     (60359)        8 2021-09-07 19:34:46.000000 django-click-2.3.0/django_click.egg-info/top_level.txt
-drwx------   0 tallen   (86646) wrds     (60359)        0 2021-09-07 19:34:46.928597 django-click-2.3.0/djclick/
--rw-------   0 tallen   (86646) wrds     (60359)      510 2021-09-07 18:47:09.000000 django-click-2.3.0/djclick/__init__.py
--rw-------   0 tallen   (86646) wrds     (60359)     8282 2021-09-07 18:38:38.000000 django-click-2.3.0/djclick/adapter.py
--rw-------   0 tallen   (86646) wrds     (60359)      946 2020-06-15 13:46:31.000000 django-click-2.3.0/djclick/params.py
--rw-------   0 tallen   (86646) wrds     (60359)      205 2020-07-20 19:15:32.000000 django-click-2.3.0/requirements-dev.txt
--rw-------   0 tallen   (86646) wrds     (60359)       78 2020-06-15 13:46:31.000000 django-click-2.3.0/requirements-test.txt
--rw-------   0 tallen   (86646) wrds     (60359)       11 2021-09-07 18:38:38.000000 django-click-2.3.0/requirements.txt
--rw-------   0 tallen   (86646) wrds     (60359)       67 2021-09-07 19:34:46.932597 django-click-2.3.0/setup.cfg
--rwx------   0 tallen   (86646) wrds     (60359)     4635 2021-09-07 19:34:15.000000 django-click-2.3.0/setup.py
+drwxr-xr-x   0 tallen     (503) staff       (20)        0 2024-04-21 17:10:27.016090 django_click-2.4.0/
+-rw-r--r--   0 tallen     (503) staff       (20)      288 2024-04-21 17:02:02.000000 django_click-2.4.0/AUTHORS.rst
+-rw-r--r--   0 tallen     (503) staff       (20)      948 2024-04-21 17:02:02.000000 django_click-2.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 tallen     (503) staff       (20)     1191 2024-04-21 17:02:02.000000 django_click-2.4.0/HISTORY.rst
+-rw-r--r--   0 tallen     (503) staff       (20)     1066 2024-04-21 17:02:02.000000 django_click-2.4.0/LICENSE
+-rw-r--r--   0 tallen     (503) staff       (20)      273 2024-04-21 17:02:02.000000 django_click-2.4.0/MANIFEST.in
+-rw-r--r--   0 tallen     (503) staff       (20)     5472 2024-04-21 17:10:27.016030 django_click-2.4.0/PKG-INFO
+-rw-r--r--   0 tallen     (503) staff       (20)     2058 2024-04-21 17:02:02.000000 django_click-2.4.0/README.rst
+drwxr-xr-x   0 tallen     (503) staff       (20)        0 2024-04-21 17:10:27.015019 django_click-2.4.0/django_click.egg-info/
+-rw-r--r--   0 tallen     (503) staff       (20)     5472 2024-04-21 17:10:27.000000 django_click-2.4.0/django_click.egg-info/PKG-INFO
+-rw-r--r--   0 tallen     (503) staff       (20)      421 2024-04-21 17:10:27.000000 django_click-2.4.0/django_click.egg-info/SOURCES.txt
+-rw-r--r--   0 tallen     (503) staff       (20)        1 2024-04-21 17:10:27.000000 django_click-2.4.0/django_click.egg-info/dependency_links.txt
+-rw-r--r--   0 tallen     (503) staff       (20)        1 2024-04-21 17:02:20.000000 django_click-2.4.0/django_click.egg-info/not-zip-safe
+-rw-r--r--   0 tallen     (503) staff       (20)      275 2024-04-21 17:10:27.000000 django_click-2.4.0/django_click.egg-info/requires.txt
+-rw-r--r--   0 tallen     (503) staff       (20)        8 2024-04-21 17:10:27.000000 django_click-2.4.0/django_click.egg-info/top_level.txt
+drwxr-xr-x   0 tallen     (503) staff       (20)        0 2024-04-21 17:10:27.014851 django_click-2.4.0/djclick/
+-rw-r--r--   0 tallen     (503) staff       (20)      510 2024-04-21 17:05:24.000000 django_click-2.4.0/djclick/__init__.py
+-rw-r--r--   0 tallen     (503) staff       (20)     8282 2024-04-21 17:02:02.000000 django_click-2.4.0/djclick/adapter.py
+-rw-r--r--   0 tallen     (503) staff       (20)      946 2024-04-21 17:02:02.000000 django_click-2.4.0/djclick/params.py
+-rw-r--r--   0 tallen     (503) staff       (20)      205 2024-04-21 17:02:02.000000 django_click-2.4.0/requirements-dev.txt
+-rw-r--r--   0 tallen     (503) staff       (20)       78 2024-04-21 17:02:02.000000 django_click-2.4.0/requirements-test.txt
+-rw-r--r--   0 tallen     (503) staff       (20)       11 2024-04-21 17:02:02.000000 django_click-2.4.0/requirements.txt
+-rw-r--r--   0 tallen     (503) staff       (20)       67 2024-04-21 17:10:27.016257 django_click-2.4.0/setup.cfg
+-rwxr-xr-x   0 tallen     (503) staff       (20)     4635 2024-04-21 17:02:02.000000 django_click-2.4.0/setup.py
```

### Comparing `django-click-2.3.0/CONTRIBUTING.rst` & `django_click-2.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-click-2.3.0/HISTORY.rst` & `django_click-2.4.0/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `django-click-2.3.0/LICENSE` & `django_click-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-click-2.3.0/README.rst` & `django_click-2.4.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -23,23 +23,20 @@
 
 .. image:: https://img.shields.io/coveralls/GaretJax/django-click/master.svg
    :target: https://coveralls.io/r/GaretJax/django-click?branch=master
 
 .. image:: https://img.shields.io/codeclimate/github/GaretJax/django-click.svg
    :target: https://codeclimate.com/github/GaretJax/django-click
 
-.. image:: https://img.shields.io/requires/github/GaretJax/django-click.svg
-   :target: https://requires.io/github/GaretJax/django-click/requirements/?branch=master
-
 ``django-click`` is a library to easily write Django management commands using the
 ``click`` command line library.
 
 * Free software: MIT license
-* Documentation for the Click command line library: http://click.pocoo.org/8/
-* Compatible with Django 2.2, 3.1, or 3.2 running on Python 3.6, 3.7, 3.8, 3.9, and PyPy.
+* Documentation for the Click command line library: https://click.palletsprojects.com/en/8.0.x/
+* Compatible with Django 4.2 and 5.0 running on Python 3.8, 3.9, 3.10, 3.11, and 3.12 (note: 3.10+ required for Django 5.0).
 
 
 Installation
 ============
 
 ::
```

### Comparing `django-click-2.3.0/djclick/adapter.py` & `django_click-2.4.0/djclick/adapter.py`

 * *Files identical despite different names*

### Comparing `django-click-2.3.0/djclick/params.py` & `django_click-2.4.0/djclick/params.py`

 * *Files identical despite different names*

### Comparing `django-click-2.3.0/setup.py` & `django_click-2.4.0/setup.py`

 * *Files identical despite different names*


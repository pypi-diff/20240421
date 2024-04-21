# Comparing `tmp/django-dynamic-raw-id-2.8.tar.gz` & `tmp/django-dynamic-raw-id-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-dynamic-raw-id-2.8.tar", last modified: Wed Dec  2 05:53:43 2020, max compression
+gzip compressed data, was "django-dynamic-raw-id-3.0.tar", last modified: Sun Mar 20 17:46:19 2022, max compression
```

## Comparing `django-dynamic-raw-id-2.8.tar` & `django-dynamic-raw-id-3.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-12-02 05:53:43.091781 django-dynamic-raw-id-2.8/
--rw-r--r--   0 martin     (501) staff       (20)      893 2020-05-02 16:02:24.000000 django-dynamic-raw-id-2.8/.eslintrc.js
--rw-r--r--   0 martin     (501) staff       (20)     1127 2020-12-02 05:53:37.000000 django-dynamic-raw-id-2.8/CHANGELOG.rst
--rw-r--r--   0 martin     (501) staff       (20)     1079 2020-05-02 16:02:24.000000 django-dynamic-raw-id-2.8/LICENSE
--rw-r--r--   0 martin     (501) staff       (20)      189 2020-05-02 16:02:24.000000 django-dynamic-raw-id-2.8/MANIFEST.in
--rw-r--r--   0 martin     (501) staff       (20)     9980 2020-12-02 05:53:43.092131 django-dynamic-raw-id-2.8/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     5841 2020-05-02 18:12:56.000000 django-dynamic-raw-id-2.8/README.rst
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-12-02 05:53:43.057902 django-dynamic-raw-id-2.8/django_dynamic_raw_id.egg-info/
--rw-r--r--   0 martin     (501) staff       (20)     9980 2020-12-02 05:53:42.000000 django-dynamic-raw-id-2.8/django_dynamic_raw_id.egg-info/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     1243 2020-12-02 05:53:42.000000 django-dynamic-raw-id-2.8/django_dynamic_raw_id.egg-info/SOURCES.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2020-12-02 05:53:42.000000 django-dynamic-raw-id-2.8/django_dynamic_raw_id.egg-info/dependency_links.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2020-05-02 16:03:23.000000 django-dynamic-raw-id-2.8/django_dynamic_raw_id.egg-info/not-zip-safe
--rw-r--r--   0 martin     (501) staff       (20)       84 2020-12-02 05:53:42.000000 django-dynamic-raw-id-2.8/django_dynamic_raw_id.egg-info/requires.txt
--rw-r--r--   0 martin     (501) staff       (20)       15 2020-12-02 05:53:42.000000 django-dynamic-raw-id-2.8/django_dynamic_raw_id.egg-info/top_level.txt
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-12-02 05:53:43.059324 django-dynamic-raw-id-2.8/dynamic_raw_id/
--rw-r--r--   0 martin     (501) staff       (20)        0 2020-05-02 16:02:24.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     1119 2020-05-02 18:13:11.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/admin.py
--rw-r--r--   0 martin     (501) staff       (20)     2135 2020-05-02 16:04:47.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/filters.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-12-02 05:53:43.053277 django-dynamic-raw-id-2.8/dynamic_raw_id/static/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-12-02 05:53:43.053359 django-dynamic-raw-id-2.8/dynamic_raw_id/static/dynamic_raw_id/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-12-02 05:53:43.059568 django-dynamic-raw-id-2.8/dynamic_raw_id/static/dynamic_raw_id/js/
--rw-r--r--   0 martin     (501) staff       (20)     3379 2020-12-02 05:45:09.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/static/dynamic_raw_id/js/dynamic_raw_id.js
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-12-02 05:53:43.053582 django-dynamic-raw-id-2.8/dynamic_raw_id/templates/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-12-02 05:53:43.060061 django-dynamic-raw-id-2.8/dynamic_raw_id/templates/dynamic_raw_id/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-12-02 05:53:43.053939 django-dynamic-raw-id-2.8/dynamic_raw_id/templates/dynamic_raw_id/admin/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-12-02 05:53:43.060316 django-dynamic-raw-id-2.8/dynamic_raw_id/templates/dynamic_raw_id/admin/filters/
--rw-r--r--   0 martin     (501) staff       (20)      565 2020-05-02 16:04:47.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/templates/dynamic_raw_id/admin/filters/dynamic_raw_id_filter.html
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-12-02 05:53:43.060563 django-dynamic-raw-id-2.8/dynamic_raw_id/templates/dynamic_raw_id/admin/widgets/
--rw-r--r--   0 martin     (501) staff       (20)      847 2020-08-13 12:22:10.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/templates/dynamic_raw_id/admin/widgets/dynamic_raw_id_field.html
--rw-r--r--   0 martin     (501) staff       (20)       45 2020-05-02 16:02:24.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/templates/dynamic_raw_id/label.html
--rw-r--r--   0 martin     (501) staff       (20)      134 2020-05-02 16:02:24.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/templates/dynamic_raw_id/multi_label.html
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-12-02 05:53:43.088669 django-dynamic-raw-id-2.8/dynamic_raw_id/tests/
--rw-r--r--   0 martin     (501) staff       (20)        0 2020-05-02 16:02:24.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/tests/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     5543 2020-05-02 18:13:11.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/tests/test_integrity.py
--rw-r--r--   0 martin     (501) staff       (20)    10301 2020-05-04 07:14:21.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/tests/test_selenium.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-12-02 05:53:43.090821 django-dynamic-raw-id-2.8/dynamic_raw_id/tests/testapp/
--rw-r--r--   0 martin     (501) staff       (20)        0 2020-05-02 16:02:24.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/tests/testapp/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)      747 2020-05-02 16:02:24.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/tests/testapp/admin.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-12-02 05:53:43.091524 django-dynamic-raw-id-2.8/dynamic_raw_id/tests/testapp/migrations/
--rw-r--r--   0 martin     (501) staff       (20)     2715 2020-05-02 16:02:24.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/tests/testapp/migrations/0001_initial.py
--rw-r--r--   0 martin     (501) staff       (20)        0 2020-05-02 16:02:24.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/tests/testapp/migrations/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     2334 2020-05-02 16:04:47.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/tests/testapp/models.py
--rw-r--r--   0 martin     (501) staff       (20)     1764 2020-05-02 16:04:47.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/tests/testapp/settings.py
--rw-r--r--   0 martin     (501) staff       (20)      200 2020-05-02 16:02:24.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/tests/testapp/urls.py
--rw-r--r--   0 martin     (501) staff       (20)      589 2020-05-02 16:02:24.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/urls.py
--rw-r--r--   0 martin     (501) staff       (20)     3179 2020-05-02 18:13:10.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/views.py
--rw-r--r--   0 martin     (501) staff       (20)     2502 2020-05-02 18:13:11.000000 django-dynamic-raw-id-2.8/dynamic_raw_id/widgets.py
--rw-r--r--   0 martin     (501) staff       (20)     1705 2020-12-02 05:53:43.092945 django-dynamic-raw-id-2.8/setup.cfg
--rwxr-xr-x   0 martin     (501) staff       (20)       59 2020-05-02 16:02:24.000000 django-dynamic-raw-id-2.8/setup.py
--rw-r--r--   0 martin     (501) staff       (20)     1156 2020-12-02 05:42:50.000000 django-dynamic-raw-id-2.8/tox.ini
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-20 17:46:19.102649 django-dynamic-raw-id-3.0/
+-rw-r--r--   0 martin     (501) staff       (20)      893 2022-03-20 12:45:06.000000 django-dynamic-raw-id-3.0/.eslintrc.js
+-rw-r--r--   0 martin     (501) staff       (20)     1409 2022-03-20 17:45:35.000000 django-dynamic-raw-id-3.0/CHANGELOG.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1079 2022-03-20 12:45:06.000000 django-dynamic-raw-id-3.0/LICENSE
+-rw-r--r--   0 martin     (501) staff       (20)      189 2022-03-20 12:45:06.000000 django-dynamic-raw-id-3.0/MANIFEST.in
+-rw-r--r--   0 martin     (501) staff       (20)     7740 2022-03-20 17:46:19.102702 django-dynamic-raw-id-3.0/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)     5548 2022-03-20 17:43:07.000000 django-dynamic-raw-id-3.0/README.rst
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-20 17:46:19.100499 django-dynamic-raw-id-3.0/django_dynamic_raw_id.egg-info/
+-rw-r--r--   0 martin     (501) staff       (20)     7740 2022-03-20 17:46:19.000000 django-dynamic-raw-id-3.0/django_dynamic_raw_id.egg-info/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)     1243 2022-03-20 17:46:19.000000 django-dynamic-raw-id-3.0/django_dynamic_raw_id.egg-info/SOURCES.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2022-03-20 17:46:19.000000 django-dynamic-raw-id-3.0/django_dynamic_raw_id.egg-info/dependency_links.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2022-03-20 12:46:23.000000 django-dynamic-raw-id-3.0/django_dynamic_raw_id.egg-info/not-zip-safe
+-rw-r--r--   0 martin     (501) staff       (20)       71 2022-03-20 17:46:19.000000 django-dynamic-raw-id-3.0/django_dynamic_raw_id.egg-info/requires.txt
+-rw-r--r--   0 martin     (501) staff       (20)       15 2022-03-20 17:46:19.000000 django-dynamic-raw-id-3.0/django_dynamic_raw_id.egg-info/top_level.txt
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-20 17:46:19.101061 django-dynamic-raw-id-3.0/dynamic_raw_id/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-20 12:45:06.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     1017 2022-03-20 15:07:56.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/admin.py
+-rw-r--r--   0 martin     (501) staff       (20)     2092 2022-03-20 16:14:36.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/filters.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-20 17:46:19.098652 django-dynamic-raw-id-3.0/dynamic_raw_id/static/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-20 17:46:19.098692 django-dynamic-raw-id-3.0/dynamic_raw_id/static/dynamic_raw_id/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-20 17:46:19.101166 django-dynamic-raw-id-3.0/dynamic_raw_id/static/dynamic_raw_id/js/
+-rw-r--r--   0 martin     (501) staff       (20)     3379 2022-03-20 12:45:06.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/static/dynamic_raw_id/js/dynamic_raw_id.js
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-20 17:46:19.098794 django-dynamic-raw-id-3.0/dynamic_raw_id/templates/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-20 17:46:19.101379 django-dynamic-raw-id-3.0/dynamic_raw_id/templates/dynamic_raw_id/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-20 17:46:19.098954 django-dynamic-raw-id-3.0/dynamic_raw_id/templates/dynamic_raw_id/admin/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-20 17:46:19.101482 django-dynamic-raw-id-3.0/dynamic_raw_id/templates/dynamic_raw_id/admin/filters/
+-rw-r--r--   0 martin     (501) staff       (20)      565 2022-03-20 12:45:06.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/templates/dynamic_raw_id/admin/filters/dynamic_raw_id_filter.html
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-20 17:46:19.101587 django-dynamic-raw-id-3.0/dynamic_raw_id/templates/dynamic_raw_id/admin/widgets/
+-rw-r--r--   0 martin     (501) staff       (20)      847 2022-03-20 16:16:31.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/templates/dynamic_raw_id/admin/widgets/dynamic_raw_id_field.html
+-rw-r--r--   0 martin     (501) staff       (20)       45 2022-03-20 12:45:06.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/templates/dynamic_raw_id/label.html
+-rw-r--r--   0 martin     (501) staff       (20)      134 2022-03-20 12:45:06.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/templates/dynamic_raw_id/multi_label.html
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-20 17:46:19.101881 django-dynamic-raw-id-3.0/dynamic_raw_id/tests/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-20 12:45:06.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/tests/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     5526 2022-03-20 16:16:01.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/tests/test_integrity.py
+-rw-r--r--   0 martin     (501) staff       (20)     9710 2022-03-20 15:06:05.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/tests/test_selenium.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-20 17:46:19.102371 django-dynamic-raw-id-3.0/dynamic_raw_id/tests/testapp/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-20 12:45:06.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/tests/testapp/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)      747 2022-03-20 12:45:06.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/tests/testapp/admin.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-20 17:46:19.102578 django-dynamic-raw-id-3.0/dynamic_raw_id/tests/testapp/migrations/
+-rw-r--r--   0 martin     (501) staff       (20)     2715 2022-03-20 12:45:06.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/tests/testapp/migrations/0001_initial.py
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-20 12:45:06.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/tests/testapp/migrations/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     2203 2022-03-20 12:50:07.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/tests/testapp/models.py
+-rw-r--r--   0 martin     (501) staff       (20)     1764 2022-03-20 12:45:06.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/tests/testapp/settings.py
+-rw-r--r--   0 martin     (501) staff       (20)      194 2022-03-20 16:14:29.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/tests/testapp/urls.py
+-rw-r--r--   0 martin     (501) staff       (20)      592 2022-03-20 16:14:07.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/urls.py
+-rw-r--r--   0 martin     (501) staff       (20)     2969 2022-03-20 15:06:42.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/views.py
+-rw-r--r--   0 martin     (501) staff       (20)     2403 2022-03-20 15:08:08.000000 django-dynamic-raw-id-3.0/dynamic_raw_id/widgets.py
+-rw-r--r--   0 martin     (501) staff       (20)     1535 2022-03-20 17:46:19.103031 django-dynamic-raw-id-3.0/setup.cfg
+-rwxr-xr-x   0 martin     (501) staff       (20)       59 2022-03-20 12:45:06.000000 django-dynamic-raw-id-3.0/setup.py
+-rw-r--r--   0 martin     (501) staff       (20)      973 2022-03-20 17:44:09.000000 django-dynamic-raw-id-3.0/tox.ini
```

### Comparing `django-dynamic-raw-id-2.8/.eslintrc.js` & `django-dynamic-raw-id-3.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `django-dynamic-raw-id-2.8/CHANGELOG.rst` & `django-dynamic-raw-id-3.0/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 =========
 Changelog
 =========
 
+v3.0 (2022-03-20)
+=======================
+
+- Django 4.0 compatibility and tests.
+- Requires Django 3.2 or up.
+- Requires Python 3.7 or up.
+- *Note:* You may now need to change the order and put the dynamic-raw-id
+  include before the generic admin include. See Readme for details.
+
 v2.8 (2020-12-02)
 =======================
 
 - Django 3.1 compatibility and tests.
 
 v2.7 (2020-05-02)
 =======================
```

### Comparing `django-dynamic-raw-id-2.8/LICENSE` & `django-dynamic-raw-id-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dynamic-raw-id-2.8/README.rst` & `django-dynamic-raw-id-3.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 .. image:: https://img.shields.io/pypi/v/django-dynamic-raw-id.svg
     :target: https://pypi.org/project/django-dynamic-raw-id/
 
-.. image:: https://travis-ci.org/lincolnloop/django-dynamic-raw-id.svg?branch=master
+.. image:: https://github.com/lincolnloop/django-dynamic-raw-id/actions/workflows/test.yml/badge.svg
     :target: https://travis-ci.org/lincolnloop/django-dynamic-raw-id
 
-.. image:: https://api.codacy.com/project/badge/Coverage/bb93482e6a6348058b993a42951a9f19
-    :target: https://www.codacy.com/app/lincolnloop/django-dynamic-raw-id
-
-.. image:: https://api.codacy.com/project/badge/Grade/bb93482e6a6348058b993a42951a9f19
-    :target: https://www.codacy.com/app/lincolnloop/django-dynamic-raw-id
-
-----
-
-.. important:: django-salmonella was renamed to django-dynamic-raw-id and
-   re-released as version 2.1. The latest django-salmonella version was 1.2.
-   Please upgrade your code, see Installation and Usage below.
-
 ----
 
 =====================
 django-dynamic-raw-id
 =====================
 
 A Django admin raw_id_fields widget replacement that handles display of an
 object's string value on change and can be overridden via a template.
 See this example:
 
 .. image:: http://d.pr/i/10GtM.png
     :target: http://d.pr/i/1kv7d.png
 
+Compatibility Matrix:
+=====================
+
+========= === === === ====
+Py/Dj     3.7 3.8 3.9 3.10
+========= === === === ====
+3.2         ✓   ✓   ✓   ✓
+4.0         ✓   ✓   ✓   ✓
+========= === === === ====
+
 Installation
 ============
 
-The app is compatible and tested with Python 2.7 → 3.7 and all versions
-of Django between 1.8 → 2.1.
 
 Install the package with ``pip``:
 
 .. code-block:: bash
 
     $ pip install django-dynamic-raw-id
 
@@ -46,21 +42,23 @@
 .. code-block:: python
 
     INSTALLED_APPS = (
         # ... other apps
         'dynamic_raw_id',
     )
 
-And add the ``urlpattern``:
+And add the ``urlpattern``. Make sure its listed *before* the generic
+``admin.site.urls`` urlpattern include:
 
 .. code-block:: python
 
     urlpatterns = [
         # ...
-        url(r'^admin/dynamic_raw_id/', include('dynamic_raw_id.urls')),
+        path('admin/dynamic_raw_id/', include('dynamic_raw_id.urls')),
+        path("admin/", admin.site.urls),
     ]
 
 ``dynamic_raw_id`` comes with some static files so don't forget to run
 ``manage.py collectstatic``.
 
 Usage
 =====
```

#### html2text {}

```diff
@@ -1,31 +1,27 @@
 .. image:: https://img.shields.io/pypi/v/django-dynamic-raw-id.svg :target:
-https://pypi.org/project/django-dynamic-raw-id/ .. image:: https://travis-
-ci.org/lincolnloop/django-dynamic-raw-id.svg?branch=master :target: https://
-travis-ci.org/lincolnloop/django-dynamic-raw-id .. image:: https://
-api.codacy.com/project/badge/Coverage/bb93482e6a6348058b993a42951a9f19 :target:
-https://www.codacy.com/app/lincolnloop/django-dynamic-raw-id .. image:: https:/
-/api.codacy.com/project/badge/Grade/bb93482e6a6348058b993a42951a9f19 :target:
-https://www.codacy.com/app/lincolnloop/django-dynamic-raw-id ---- ..
-important:: django-salmonella was renamed to django-dynamic-raw-id and re-
-released as version 2.1. The latest django-salmonella version was 1.2. Please
-upgrade your code, see Installation and Usage below. ---- =====================
-django-dynamic-raw-id ===================== A Django admin raw_id_fields widget
-replacement that handles display of an object's string value on change and can
-be overridden via a template. See this example: .. image:: http://d.pr/i/
-10GtM.png :target: http://d.pr/i/1kv7d.png Installation ============ The app is
-compatible and tested with Python 2.7 â 3.7 and all versions of Django
-between 1.8 â 2.1. Install the package with ``pip``: .. code-block:: bash $
-pip install django-dynamic-raw-id Put ``dynamic_raw_id`` to your list of
-``INSTALLED_APPS``: .. code-block:: python INSTALLED_APPS = ( # ... other apps
-'dynamic_raw_id', ) And add the ``urlpattern``: .. code-block:: python
-urlpatterns = [ # ... url(r'^admin/dynamic_raw_id/', include
-('dynamic_raw_id.urls')), ] ``dynamic_raw_id`` comes with some static files so
-don't forget to run ``manage.py collectstatic``. Usage ===== To start using
-django-dynamic-raw-id in your application all you need to do is implement
+https://pypi.org/project/django-dynamic-raw-id/ .. image:: https://github.com/
+lincolnloop/django-dynamic-raw-id/actions/workflows/test.yml/badge.svg :target:
+https://travis-ci.org/lincolnloop/django-dynamic-raw-id ---
+- ===================== django-dynamic-raw-id ===================== A Django
+admin raw_id_fields widget replacement that handles display of an object's
+string value on change and can be overridden via a template. See this example:
+.. image:: http://d.pr/i/10GtM.png :target: http://d.pr/i/1kv7d.png
+Compatibility Matrix: ===================== ========= === === === ==== Py/Dj
+3.7 3.8 3.9 3.10 ========= === === === ==== 3.2 â â â â 4.0 â â â
+â ========= === === === ==== Installation ============ Install the package
+with ``pip``: .. code-block:: bash $ pip install django-dynamic-raw-id Put
+``dynamic_raw_id`` to your list of ``INSTALLED_APPS``: .. code-block:: python
+INSTALLED_APPS = ( # ... other apps 'dynamic_raw_id', ) And add the
+``urlpattern``. Make sure its listed *before* the generic ``admin.site.urls``
+urlpattern include: .. code-block:: python urlpatterns = [ # ... path('admin/
+dynamic_raw_id/', include('dynamic_raw_id.urls')), path("admin/",
+admin.site.urls), ] ``dynamic_raw_id`` comes with some static files so don't
+forget to run ``manage.py collectstatic``. Usage ===== To start using django-
+dynamic-raw-id in your application all you need to do is implement
 ``DynamicRawIDMixin`` in your ``ModelAdmin`` class and add the desired fields
 to a list of ``dynamic_raw_id_fields``: .. code-block:: python from
 dynamic_raw_id.admin import DynamicRawIDMixin class UserProfileAdmin
 (DynamicRawIDMixin, admin.ModelAdmin): dynamic_raw_id_fields = ('user',) You
 can use dynamic_raw_id widgets in a Admin filter as well: .. code-block::
 python from dynamic_raw_id.admin import DynamicRawIDMixin from
 dynamic_raw_id.filters import DynamicRawIDFilter class UserProfileAdmin
```

### Comparing `django-dynamic-raw-id-2.8/django_dynamic_raw_id.egg-info/SOURCES.txt` & `django-dynamic-raw-id-3.0/django_dynamic_raw_id.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-dynamic-raw-id-2.8/dynamic_raw_id/admin.py` & `django-dynamic-raw-id-3.0/dynamic_raw_id/admin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-from django import VERSION
-
 from dynamic_raw_id.widgets import DynamicRawIDMultiIdWidget, DynamicRawIDWidget
 
 
 class DynamicRawIDMixin(object):
     dynamic_raw_id_fields = ()
 
     def formfield_for_foreignkey(self, db_field, request=None, **kwargs):
         if db_field.name in self.dynamic_raw_id_fields:
-            rel = db_field.remote_field if VERSION[0] >= 2 else db_field.rel
-            kwargs['widget'] = DynamicRawIDWidget(rel, self.admin_site)
+            rel = db_field.remote_field
+            kwargs["widget"] = DynamicRawIDWidget(rel, self.admin_site)
             return db_field.formfield(**kwargs)
         return super(DynamicRawIDMixin, self).formfield_for_foreignkey(
             db_field, request, **kwargs
         )
 
     def formfield_for_manytomany(self, db_field, request=None, **kwargs):
         if db_field.name in self.dynamic_raw_id_fields:
-            rel = db_field.remote_field if VERSION[0] >= 2 else db_field.rel
-            kwargs['widget'] = DynamicRawIDMultiIdWidget(rel, self.admin_site)
-            kwargs['help_text'] = ''
+            rel = db_field.remote_field
+            kwargs["widget"] = DynamicRawIDMultiIdWidget(rel, self.admin_site)
+            kwargs["help_text"] = ""
             return db_field.formfield(**kwargs)
         return super(DynamicRawIDMixin, self).formfield_for_manytomany(
             db_field, request, **kwargs
         )
```

### Comparing `django-dynamic-raw-id-2.8/dynamic_raw_id/filters.py` & `django-dynamic-raw-id-3.0/dynamic_raw_id/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # coding: utf-8
 
 """dynamic_raw_id filters."""
 
-from django import VERSION, forms
+from django import forms
 from django.contrib import admin
 
 from dynamic_raw_id.widgets import DynamicRawIDWidget
 
 
 class DynamicRawIDFilterForm(forms.Form):
 
     """Form for dynamic_raw_id filter."""
 
     def __init__(self, rel, admin_site, field_name, **kwargs):
         """Construct field for given field rel."""
         super(DynamicRawIDFilterForm, self).__init__(**kwargs)
-        self.fields['%s' % field_name] = forms.IntegerField(
-            label='',
+        self.fields["%s" % field_name] = forms.IntegerField(
+            label="",
             widget=DynamicRawIDWidget(rel=rel, admin_site=admin_site),
             required=False,
         )
 
 
 class DynamicRawIDFilter(admin.filters.FieldListFilter):
 
     """Filter list queryset by primary key of related object."""
 
-    template = 'dynamic_raw_id/admin/filters/dynamic_raw_id_filter.html'
+    template = "dynamic_raw_id/admin/filters/dynamic_raw_id_filter.html"
 
     def __init__(self, field, request, params, model, model_admin, field_path):
         """Use GET param for lookup and form initialization."""
-        self.lookup_kwarg = '%s' % field_path
+        self.lookup_kwarg = "%s" % field_path
         super(DynamicRawIDFilter, self).__init__(
             field, request, params, model, model_admin, field_path
         )
-        rel = field.remote_field if VERSION[0] >= 2 else field.rel
+        rel = field.remote_field
         self.form = self.get_form(request, rel, model_admin.admin_site)
 
     def choices(self, cl):
         """Filter choices are not available."""
         return []
 
     def expected_parameters(self):
```

### Comparing `django-dynamic-raw-id-2.8/dynamic_raw_id/static/dynamic_raw_id/js/dynamic_raw_id.js` & `django-dynamic-raw-id-3.0/dynamic_raw_id/static/dynamic_raw_id/js/dynamic_raw_id.js`

 * *Files identical despite different names*

### Comparing `django-dynamic-raw-id-2.8/dynamic_raw_id/templates/dynamic_raw_id/admin/filters/dynamic_raw_id_filter.html` & `django-dynamic-raw-id-3.0/dynamic_raw_id/templates/dynamic_raw_id/admin/filters/dynamic_raw_id_filter.html`

 * *Files identical despite different names*

### Comparing `django-dynamic-raw-id-2.8/dynamic_raw_id/templates/dynamic_raw_id/admin/widgets/dynamic_raw_id_field.html` & `django-dynamic-raw-id-3.0/dynamic_raw_id/templates/dynamic_raw_id/admin/widgets/dynamic_raw_id_field.html`

 * *Files identical despite different names*

### Comparing `django-dynamic-raw-id-2.8/dynamic_raw_id/tests/test_integrity.py` & `django-dynamic-raw-id-3.0/dynamic_raw_id/tests/test_integrity.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,48 +4,45 @@
 
 from dynamic_raw_id.tests.testapp.models import (
     CharPrimaryKeyModel,
     DirectPrimaryKeyModel,
     TestModel,
 )
 
-
 class DynamicRawIDTestCase(TestCase):
     """
     Test the basic integrity of the app. We can't test the Javascript side
     and all those fancy popups, but we can load an admin view and check that
     dynamic_raw_id was successfully loaded and displays items properly.
     """
 
     def setUp(self):
         # Create admin and login by default
-        self.admin = User.objects.create_superuser('admin', '', 'admin')
-        self.client.login(username='admin', password='admin')
+        self.admin = User.objects.create_superuser("admin", "", "admin")
+        self.client.login(username="admin", password="admin")
 
         # Create additional staff user without any app permissions
-        self.user_noperm = User.objects.create_user('user', '', 'user')
+        self.user_noperm = User.objects.create_user("user", "", "user")
         self.user_noperm.is_staff = True
         self.user_noperm.save()
 
     def tearDown(self):
         self.client.logout()
 
     def get_labelview_url(self, multi=False):
-        name = multi and 'dynamic_raw_id_multi_label' or 'dynamic_raw_id_label'
-        return reverse(
-            name, kwargs={'app_name': 'testapp', 'model_name': 'testmodel'}
-        )
+        name = multi and "dynamic_raw_id_multi_label" or "dynamic_raw_id_label"
+        return reverse("dynamic_raw_id:{}".format(name), kwargs={"app_name": "testapp", "model_name": "testmodel"})
 
     def create_sample_data(self):
         """
         Create a bit of sample data we can use to assign.
         """
-        self.u1 = User.objects.create_superuser('jon', 'jon@example.com', '')
-        self.u2 = User.objects.create_superuser('jim', 'jim@example.com', '')
-        self.c1 = CharPrimaryKeyModel.objects.create(chr='helloworld')
+        self.u1 = User.objects.create_superuser("jon", "jon@example.com", "")
+        self.u2 = User.objects.create_superuser("jim", "jim@example.com", "")
+        self.c1 = CharPrimaryKeyModel.objects.create(chr="helloworld")
         self.n1 = DirectPrimaryKeyModel.objects.create(num=12345)
 
         self.obj = TestModel.objects.create(
             rawid_fk=self.u1,
             rawid_fk_limited=self.u1,
             rawid_fk_direct_pk=self.n1,
             dynamic_raw_id_fk=self.u1,
@@ -58,27 +55,25 @@
 
     def test_changelist_integrity(self):
         """
         The `DynamicRawIDFilter` is hooked up in the right filter bar of the
         testapp changelist view.
         """
         self.create_sample_data()
-        list_url = reverse('admin:testapp_testmodel_changelist')
+        list_url = reverse("admin:testapp_testmodel_changelist")
         response = self.client.get(list_url)
         self.assertEqual(response.status_code, 200)
 
     def test_change_integrity(self):
         """
         The `DynamicRawIDFilter` is hooked up in the right filter bar of the
         testapp changelist view.
         """
         self.create_sample_data()
-        list_url = reverse(
-            'admin:testapp_testmodel_change', args=(self.obj.pk,)
-        )
+        list_url = reverse("admin:testapp_testmodel_change", args=(self.obj.pk,))
         response = self.client.get(list_url)
         self.assertEqual(response.status_code, 200)
 
     def test_labelview_unauthed(self):
         """
         Label view required authentication and a staff account
         """
@@ -88,60 +83,60 @@
 
     def test_labelview_no_permission(self):
         """
         Valid Label view request is denied if user has
         no change permisson for the app.
         """
         self.client.logout()
-        self.client.login(username='user', password='user')
+        self.client.login(username="user", password="user")
         self.create_sample_data()
         response = self.client.get(
-            self.get_labelview_url(multi=True), {'id': self.obj.pk}, follow=True
+            self.get_labelview_url(multi=True), {"id": self.obj.pk}, follow=True
         )
         self.assertEqual(response.status_code, 403)
 
     def test_labelview(self):
         """
         Call the labelview directly (what usually an Ajax JS call would do)
         and check for proper response.
         """
         self.create_sample_data()
         response = self.client.get(
-            self.get_labelview_url(), {'id': self.obj.pk}, follow=True
+            self.get_labelview_url(), {"id": self.obj.pk}, follow=True
         )
         self.assertEqual(response.status_code, 200)
 
     def test_multi_labelview(self):
         """
         Call the labelview directly (what usually an Ajax JS call would do)
         and check for proper response.
         """
         self.create_sample_data()
         response = self.client.get(
-            self.get_labelview_url(multi=True), {'id': self.obj.pk}, follow=True
+            self.get_labelview_url(multi=True), {"id": self.obj.pk}, follow=True
         )
         self.assertEqual(response.status_code, 200)
 
     def test_invalid_id(self):
         """
         Test invalid id.
         """
         self.create_sample_data()
         response = self.client.get(
-            self.get_labelview_url(), {'id': 'wrong'}, follow=True
+            self.get_labelview_url(), {"id": "wrong"}, follow=True
         )
         self.assertEqual(response.status_code, 400)
 
     def test_id_does_not_exist(self):
         """
         Test model primary key does not exist.
         """
         self.create_sample_data()
         response = self.client.get(
-            self.get_labelview_url(), {'id': '123456'}, follow=True
+            self.get_labelview_url(), {"id": "123456"}, follow=True
         )
         self.assertEqual(response.status_code, 400)
 
     def test_no_id(self):
         """
         Test invalid app/model name.
         """
@@ -150,10 +145,10 @@
         self.assertEqual(response.status_code, 400)
 
     def test_invalid_appname(self):
         """
         Test invalid app/model name.
         """
         self.create_sample_data()
-        url = self.get_labelview_url().replace('testapp', 'foobar')
-        response = self.client.get(url, {'id': self.obj.pk}, follow=True)
+        url = self.get_labelview_url().replace("testapp", "foobar")
+        response = self.client.get(url, {"id": self.obj.pk}, follow=True)
         self.assertEqual(response.status_code, 400)
```

### Comparing `django-dynamic-raw-id-2.8/dynamic_raw_id/tests/test_selenium.py` & `django-dynamic-raw-id-3.0/dynamic_raw_id/tests/test_selenium.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,38 +14,31 @@
 )
 
 logger = getLogger(__file__)
 
 
 def get_webdriver():
     from selenium.webdriver.firefox.webdriver import WebDriver
+
     return WebDriver()
 
 
 class BaseSeleniumTests(StaticLiveServerTestCase):
     def setUp(self):
         super(BaseSeleniumTests, self).setUp()
-        self.admin_user = 'jane'
-        self.jane = User.objects.create_superuser(
-            'jane', 'jane@example.com', 'foobar'
-        )
+        self.admin_user = "jane"
+        self.jane = User.objects.create_superuser("jane", "jane@example.com", "foobar")
 
         # More users for testing m2m relations
-        self.tick = User.objects.create_user(
-            'tick', 'tick@example.com', 'foobar'
-        )
-        self.trick = User.objects.create_user(
-            'trick', 'trick@example.com', 'foobar'
-        )
-        self.track = User.objects.create_user(
-            'track', 'track@example.com', 'foobar'
-        )
+        self.tick = User.objects.create_user("tick", "tick@example.com", "foobar")
+        self.trick = User.objects.create_user("trick", "trick@example.com", "foobar")
+        self.track = User.objects.create_user("track", "track@example.com", "foobar")
 
-        self.add_testmodel_url = '{0}{1}'.format(
-            self.live_server_url, reverse('admin:testapp_testmodel_add')
+        self.add_testmodel_url = "{0}{1}".format(
+            self.live_server_url, reverse("admin:testapp_testmodel_add")
         )
 
     @classmethod
     def setUpClass(cls):
         super(BaseSeleniumTests, cls).setUpClass()
         cls.wd = get_webdriver()
         cls.wd.implicitly_wait(10)
@@ -63,38 +56,36 @@
         time.sleep(seconds)
 
     def _login_admin(self):
         """
         Login into the Django Admin with our Admin credentials
         :return:
         """
-        self.wd.get(
-            '{0}{1}'.format(self.live_server_url, reverse('admin:index'))
-        )
-        self.wd.find_element_by_name("username").send_keys('jane')
-        self.wd.find_element_by_name("password").send_keys('foobar')
-        self.wd.find_element_by_css_selector('input[type=submit]').click()
+        self.wd.get("{0}{1}".format(self.live_server_url, reverse("admin:index")))
+        self.wd.find_element_by_name("username").send_keys("jane")
+        self.wd.find_element_by_name("password").send_keys("foobar")
+        self.wd.find_element_by_css_selector("input[type=submit]").click()
 
         # Wait until index page is loaded
-        self.wd.find_element_by_link_text('TESTAPP')
+        self.wd.find_element_by_link_text("TESTAPP")
 
     def _goto_add_page(self):
         """
         Go to the "TestApp" Add form page
         :return:
         """
         self.wd.get(self.add_testmodel_url)
 
     def _click_lookup_and_choose(self, row_id, link_text):
         """
         Clicks on the little glass icon selector and waits until the
         selector popup opens. Then it selects the given link text.
         """
         # Click on the Glass icon with the id <lookup_id>.
-        self.wd.find_element_by_id('lookup_id_{0}'.format(row_id)).click()
+        self.wd.find_element_by_id("lookup_id_{0}".format(row_id)).click()
 
         #  Activate the popup window with the `window.name = <window_id>`
         self.wd.switch_to.window(self.wd.window_handles[1])
 
         # Click on the username/line item with the link text <link_text>.
         self.wd.find_element_by_link_text(link_text).click()
 
@@ -102,182 +93,154 @@
         self.wd.switch_to.window(self.wd.window_handles[0])
 
     def _save_and_continue(self):
         """
         Hit "Save and continue editing" and make sure
         the response has no error.
         """
-        self.wd.find_element_by_css_selector('input[name=_continue]').click()
+        self.wd.find_element_by_css_selector("input[name=_continue]").click()
 
         # Wait until page is loaded and success message is displayed
         self.assertTrue(
-            self.wd.find_element_by_css_selector('li.success').is_displayed()
+            self.wd.find_element_by_css_selector("li.success").is_displayed()
         )
 
     def test_dynamic_foreignkey(self):
         """
         dynamic_raw_id on a regular ForeignKey field
         """
-        row_id = 'dynamic_raw_id_fk'  # The admin row ID/indicator we test
+        row_id = "dynamic_raw_id_fk"  # The admin row ID/indicator we test
         user_to_test = self.tick
 
         self._login_admin()
         self._goto_add_page()
         self._click_lookup_and_choose(row_id, user_to_test.username)
 
         # user id is inside the input field
         self.assertEqual(
-            self.wd.find_element_by_id('id_{0}'.format(row_id)).get_property(
-                'value'
-            ),
+            self.wd.find_element_by_id("id_{0}".format(row_id)).get_property("value"),
             str(user_to_test.pk),
         )
 
         # username is displayed next to the element
         self.assertEqual(
-            self.wd.find_element_by_id(
-                '{0}_dynamic_raw_id_label'.format(row_id)
-            ).text,
+            self.wd.find_element_by_id("{0}_dynamic_raw_id_label".format(row_id)).text,
             user_to_test.username,
         )
 
         self._save_and_continue()
 
     def test_dynamic_foreignkey_limited(self):
         """
         dynamic_raw_id on a regular ForeignKey field with `limit_choices_to`
         """
-        row_id = (
-            'dynamic_raw_id_fk_limited'  # The admin row ID/indicator we test
-        )
+        row_id = "dynamic_raw_id_fk_limited"  # The admin row ID/indicator we test
         user_to_test = self.jane
 
         self._login_admin()
         self._goto_add_page()
         self._click_lookup_and_choose(row_id, user_to_test.username)
 
         # user id is inside the input field
         self.assertEqual(
-            self.wd.find_element_by_id('id_{0}'.format(row_id)).get_property(
-                'value'
-            ),
+            self.wd.find_element_by_id("id_{0}".format(row_id)).get_property("value"),
             str(user_to_test.pk),
         )
 
         # username is displayed next to the element
         self.assertEqual(
-            self.wd.find_element_by_id(
-                '{0}_dynamic_raw_id_label'.format(row_id)
-            ).text,
+            self.wd.find_element_by_id("{0}_dynamic_raw_id_label".format(row_id)).text,
             user_to_test.username,
         )
 
         self._save_and_continue()
 
     def test_dynamic_many2many(self):
         """
         dynamic_raw_id on a many2many field
         """
-        row_id = 'dynamic_raw_id_many'  # The admin row ID/indicator we test
+        row_id = "dynamic_raw_id_many"  # The admin row ID/indicator we test
 
         self._login_admin()
         self._goto_add_page()
 
         self._click_lookup_and_choose(row_id, self.tick.username)
         self._click_lookup_and_choose(row_id, self.trick.username)
         self._click_lookup_and_choose(row_id, self.track.username)
 
         # the three user ids are inside the element
-        expected = '{0},{1},{2}'.format(
-            self.tick.pk, self.trick.pk, self.track.pk
-        )
+        expected = "{0},{1},{2}".format(self.tick.pk, self.trick.pk, self.track.pk)
         self.assertEqual(
-            self.wd.find_element_by_id('id_{0}'.format(row_id)).get_property(
-                'value'
-            ),
+            self.wd.find_element_by_id("id_{0}".format(row_id)).get_property("value"),
             expected,
         )
 
         # tick, trick and track are now be displayed next to the form field
         # This is actually a bug, same ID for multiple elements
-        expected = '{0},  {1},  {2}'.format(
+        expected = "{0},  {1},  {2}".format(
             self.tick.username, self.trick.username, self.track.username
         )
         self.assertEqual(
-            self.wd.find_element_by_id(
-                '{0}_dynamic_raw_id_label'.format(row_id)
-            ).text,
+            self.wd.find_element_by_id("{0}_dynamic_raw_id_label".format(row_id)).text,
             expected,
         )
 
         self._save_and_continue()
 
     def test_dynamic_direct_charfield(self):
         """
         dynamic_raw_id on a custom Model with a CharField
         """
-        row_id = (
-            'dynamic_raw_id_fk_char_pk'  # The admin row ID/indicator we test
-        )
-        username = 'Hello World'
+        row_id = "dynamic_raw_id_fk_char_pk"  # The admin row ID/indicator we test
+        username = "Hello World"
 
         # Add a test model instances
-        custom_obj = CharPrimaryKeyModel.objects.create(chr='Hello World')
+        custom_obj = CharPrimaryKeyModel.objects.create(chr="Hello World")
 
         self._login_admin()
         self._goto_add_page()
         self._click_lookup_and_choose(row_id, username)
 
         # object id is inside the input field
         self.assertEqual(
-            self.wd.find_element_by_id('id_{0}'.format(row_id)).get_property(
-                'value'
-            ),
+            self.wd.find_element_by_id("id_{0}".format(row_id)).get_property("value"),
             str(custom_obj.pk),
         )
 
         # object label is now be displayed next to the form field
         self.assertEqual(
-            self.wd.find_element_by_id(
-                '{0}_dynamic_raw_id_label'.format(row_id)
-            ).text,
+            self.wd.find_element_by_id("{0}_dynamic_raw_id_label".format(row_id)).text,
             custom_obj.chr,
         )
 
         self._save_and_continue()
 
     def test_dynamic_direct_integerfield(self):
         """
         dynamic_raw_id on a custom Model with an IntegerField
         """
-        row_id = (
-            'dynamic_raw_id_fk_direct_pk'  # The admin row ID/indicator we test
-        )
-        username = '12345'
+        row_id = "dynamic_raw_id_fk_direct_pk"  # The admin row ID/indicator we test
+        username = "12345"
 
         # Add a test model instances
         custom_obj = DirectPrimaryKeyModel.objects.create(num=12345)
 
         self._login_admin()
         self._goto_add_page()
         self._click_lookup_and_choose(row_id, username)
 
         # object id is inside the input field
         self.assertEqual(
-            self.wd.find_element_by_id('id_{0}'.format(row_id)).get_property(
-                'value'
-            ),
+            self.wd.find_element_by_id("id_{0}".format(row_id)).get_property("value"),
             str(custom_obj.pk),
         )
 
         # object label is now be displayed next to the form field
         self.assertEqual(
-            self.wd.find_element_by_id(
-                '{0}_dynamic_raw_id_label'.format(row_id)
-            ).text,
+            self.wd.find_element_by_id("{0}_dynamic_raw_id_label".format(row_id)).text,
             str(custom_obj.num),
         )
 
         self._save_and_continue()
 
     def test_dynamic_filter(self):
         """
@@ -288,38 +251,30 @@
         TestModel.objects.create(dynamic_raw_id_fk=self.tick)
         TestModel.objects.create(dynamic_raw_id_fk=self.trick)
         TestModel.objects.create(dynamic_raw_id_fk=self.track)
 
         self._login_admin()
 
         # Go to the change list page.
-        changelist_url = '{0}{1}'.format(
-            self.live_server_url, reverse('admin:testapp_testmodel_changelist')
+        changelist_url = "{0}{1}".format(
+            self.live_server_url, reverse("admin:testapp_testmodel_changelist")
         )
         self.wd.get(changelist_url)
 
         # tick, trick and track are visible in the changelist table
-        self.assertTrue(
-            self.wd.find_element_by_link_text('tick').is_displayed()
-        )
-        self.assertTrue(
-            self.wd.find_element_by_link_text('trick').is_displayed()
-        )
-        self.assertTrue(
-            self.wd.find_element_by_link_text('track').is_displayed()
-        )
+        self.assertTrue(self.wd.find_element_by_link_text("tick").is_displayed())
+        self.assertTrue(self.wd.find_element_by_link_text("trick").is_displayed())
+        self.assertTrue(self.wd.find_element_by_link_text("track").is_displayed())
 
         # Click on the filter glass icon and choose 'trick'
-        self._click_lookup_and_choose('dynamic_raw_id_fk', 'trick')
+        self._click_lookup_and_choose("dynamic_raw_id_fk", "trick")
 
         # Click the submit icon of the filter panel
         self.wd.find_element_by_css_selector(
-            '#changelist-filter input[type=submit]'
+            "#changelist-filter input[type=submit]"
         ).click()
 
         # Only "trick" is visible in the changelist table
         self.wd.implicitly_wait(0)
-        self.assertTrue(
-            self.wd.find_element_by_link_text('trick').is_displayed()
-        )
-        self.assertTrue(len(self.wd.find_elements_by_link_text('tick')) == 0)
-        self.assertTrue(len(self.wd.find_elements_by_link_text('track')) == 0)
+        self.assertTrue(self.wd.find_element_by_link_text("trick").is_displayed())
+        self.assertTrue(len(self.wd.find_elements_by_link_text("tick")) == 0)
+        self.assertTrue(len(self.wd.find_elements_by_link_text("track")) == 0)
```

### Comparing `django-dynamic-raw-id-2.8/dynamic_raw_id/tests/testapp/admin.py` & `django-dynamic-raw-id-3.0/dynamic_raw_id/tests/testapp/admin.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from dynamic_raw_id.admin import DynamicRawIDMixin
 from dynamic_raw_id.filters import DynamicRawIDFilter
 
 from .models import CharPrimaryKeyModel, DirectPrimaryKeyModel, TestModel
 
 
 class TestModelAdmin(DynamicRawIDMixin, admin.ModelAdmin):
-    raw_id_fields = ('rawid_fk', 'rawid_fk_limited', 'rawid_many')
+    raw_id_fields = ("rawid_fk", "rawid_fk_limited", "rawid_many")
     dynamic_raw_id_fields = (
-        'dynamic_raw_id_fk',
-        'dynamic_raw_id_fk_limited',
-        'dynamic_raw_id_many',
-        'dynamic_raw_id_fk_direct_pk',
-        'dynamic_raw_id_fk_char_pk',
+        "dynamic_raw_id_fk",
+        "dynamic_raw_id_fk_limited",
+        "dynamic_raw_id_many",
+        "dynamic_raw_id_fk_direct_pk",
+        "dynamic_raw_id_fk_char_pk",
     )
-    list_filter = (('dynamic_raw_id_fk', DynamicRawIDFilter),)
+    list_filter = (("dynamic_raw_id_fk", DynamicRawIDFilter),)
 
 
 admin.site.register(DirectPrimaryKeyModel)
 admin.site.register(CharPrimaryKeyModel)
 admin.site.register(TestModel, TestModelAdmin)
```

### Comparing `django-dynamic-raw-id-2.8/dynamic_raw_id/tests/testapp/migrations/0001_initial.py` & `django-dynamic-raw-id-3.0/dynamic_raw_id/tests/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-raw-id-2.8/dynamic_raw_id/tests/testapp/models.py` & `django-dynamic-raw-id-3.0/dynamic_raw_id/tests/testapp/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,92 +1,88 @@
 from django.db import models
-from six import python_2_unicode_compatible
 
 
-@python_2_unicode_compatible
 class DirectPrimaryKeyModel(models.Model):
     num = models.IntegerField("Number", primary_key=True)
 
     def __str__(self):
         return str(self.num)
 
 
-@python_2_unicode_compatible
 class CharPrimaryKeyModel(models.Model):
     chr = models.CharField(max_length=20, primary_key=True)
 
     def __str__(self):
         return self.chr
 
 
-@python_2_unicode_compatible
 class TestModel(models.Model):
     rawid_fk = models.ForeignKey(
-        'auth.User',
-        related_name='rawid_fk',
+        "auth.User",
+        related_name="rawid_fk",
         blank=True,
         null=True,
         on_delete=models.CASCADE,
     )
 
     rawid_fk_limited = models.ForeignKey(
-        'auth.User',
-        related_name='rawid_fk_limited',
-        limit_choices_to={'is_staff': True},
+        "auth.User",
+        related_name="rawid_fk_limited",
+        limit_choices_to={"is_staff": True},
         blank=True,
         null=True,
         on_delete=models.CASCADE,
     )
 
     rawid_many = models.ManyToManyField(
-        'auth.User', related_name='rawid_many', blank=True
+        "auth.User", related_name="rawid_many", blank=True
     )
 
     rawid_fk_direct_pk = models.ForeignKey(
         DirectPrimaryKeyModel,
-        related_name='rawid_fk_direct_pk',
+        related_name="rawid_fk_direct_pk",
         blank=True,
         null=True,
         on_delete=models.CASCADE,
     )
 
     dynamic_raw_id_fk = models.ForeignKey(
-        'auth.User',
-        related_name='dynamic_raw_id_fk',
+        "auth.User",
+        related_name="dynamic_raw_id_fk",
         blank=True,
         null=True,
         on_delete=models.CASCADE,
     )
 
     dynamic_raw_id_fk_limited = models.ForeignKey(
-        'auth.User',
-        related_name='dynamic_raw_id_fk_limited',
-        limit_choices_to={'is_staff': True},
+        "auth.User",
+        related_name="dynamic_raw_id_fk_limited",
+        limit_choices_to={"is_staff": True},
         blank=True,
         null=True,
         on_delete=models.CASCADE,
     )
 
     dynamic_raw_id_many = models.ManyToManyField(
-        'auth.User', related_name='dynamic_raw_id_many', blank=True
+        "auth.User", related_name="dynamic_raw_id_many", blank=True
     )
 
     dynamic_raw_id_fk_direct_pk = models.ForeignKey(
         DirectPrimaryKeyModel,
-        related_name='dynamic_raw_id_fk_direct_pk',
+        related_name="dynamic_raw_id_fk_direct_pk",
         blank=True,
         null=True,
         on_delete=models.CASCADE,
     )
 
     dynamic_raw_id_fk_char_pk = models.ForeignKey(
         CharPrimaryKeyModel,
-        related_name='dynamic_raw_id_fk_char_pk',
+        related_name="dynamic_raw_id_fk_char_pk",
         blank=True,
         null=True,
         on_delete=models.CASCADE,
     )
 
     def __str__(self):
         if self.dynamic_raw_id_fk:
             return self.dynamic_raw_id_fk.username
-        return 'Unnamed Test Instance'
+        return "Unnamed Test Instance"
```

### Comparing `django-dynamic-raw-id-2.8/dynamic_raw_id/tests/testapp/settings.py` & `django-dynamic-raw-id-3.0/dynamic_raw_id/tests/testapp/settings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 DEBUG = True
 
 SECRET_KEY = "super-secret-dynamic_raw_id-key"
 
 DATABASES = {
-    'default': {'ENGINE': 'django.db.backends.sqlite3', 'NAME': 'testapp.db'},
+    "default": {"ENGINE": "django.db.backends.sqlite3", "NAME": "testapp.db"},
 }
 
 TEMPLATES = [
     {
-        'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'DIRS': [],
-        'APP_DIRS': True,
-        'OPTIONS': {
-            'context_processors': [
-                'django.template.context_processors.debug',
-                'django.template.context_processors.request',
-                'django.contrib.auth.context_processors.auth',
-                'django.contrib.messages.context_processors.messages',
+        "BACKEND": "django.template.backends.django.DjangoTemplates",
+        "DIRS": [],
+        "APP_DIRS": True,
+        "OPTIONS": {
+            "context_processors": [
+                "django.template.context_processors.debug",
+                "django.template.context_processors.request",
+                "django.contrib.auth.context_processors.auth",
+                "django.contrib.messages.context_processors.messages",
             ]
         },
     }
 ]
 
 INSTALLED_APPS = [
-    'django.contrib.contenttypes',
-    'django.contrib.admin',
-    'django.contrib.auth',
-    'django.contrib.sessions',
-    'django.contrib.staticfiles',
-    'django.contrib.messages',
-    'dynamic_raw_id',
-    'dynamic_raw_id.tests.testapp',
+    "django.contrib.contenttypes",
+    "django.contrib.admin",
+    "django.contrib.auth",
+    "django.contrib.sessions",
+    "django.contrib.staticfiles",
+    "django.contrib.messages",
+    "dynamic_raw_id",
+    "dynamic_raw_id.tests.testapp",
 ]
 
 MIDDLEWARE = (
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.middleware.common.CommonMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware',
+    "django.contrib.sessions.middleware.SessionMiddleware",
+    "django.contrib.auth.middleware.AuthenticationMiddleware",
+    "django.middleware.common.CommonMiddleware",
+    "django.contrib.messages.middleware.MessageMiddleware",
 )
 
-STATIC_ROOT = '/tmp/dynamic_raw_id_static/'
-STATIC_URL = '/static/'
-ROOT_URLCONF = 'dynamic_raw_id.tests.testapp.urls'
+STATIC_ROOT = "/tmp/dynamic_raw_id_static/"
+STATIC_URL = "/static/"
+ROOT_URLCONF = "dynamic_raw_id.tests.testapp.urls"
 
 STATICFILES_FINDERS = [
-    'django.contrib.staticfiles.finders.FileSystemFinder',
-    'django.contrib.staticfiles.finders.AppDirectoriesFinder',
+    "django.contrib.staticfiles.finders.FileSystemFinder",
+    "django.contrib.staticfiles.finders.AppDirectoriesFinder",
 ]
 
 TEST_SETTINGS = {
-    'DEBUG': DEBUG,
-    'SECRET_KEY': SECRET_KEY,
-    'DATABASES': DATABASES,
-    'TEMPLATES': TEMPLATES,
-    'INSTALLED_APPS': INSTALLED_APPS,
-    'MIDDLEWARE': MIDDLEWARE,
-    'STATIC_ROOT': STATIC_ROOT,
-    'STATIC_URL': STATIC_URL,
-    'ROOT_URLCONF': ROOT_URLCONF,
-    'STATICFILES_FINDERS': STATICFILES_FINDERS,
+    "DEBUG": DEBUG,
+    "SECRET_KEY": SECRET_KEY,
+    "DATABASES": DATABASES,
+    "TEMPLATES": TEMPLATES,
+    "INSTALLED_APPS": INSTALLED_APPS,
+    "MIDDLEWARE": MIDDLEWARE,
+    "STATIC_ROOT": STATIC_ROOT,
+    "STATIC_URL": STATIC_URL,
+    "ROOT_URLCONF": ROOT_URLCONF,
+    "STATICFILES_FINDERS": STATICFILES_FINDERS,
 }
```

### Comparing `django-dynamic-raw-id-2.8/dynamic_raw_id/views.py` & `django-dynamic-raw-id-3.0/dynamic_raw_id/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from django import VERSION
 from django.apps import apps
 from django.conf import settings
 from django.contrib.auth.decorators import user_passes_test
 from django.http import HttpResponseBadRequest, HttpResponseForbidden
 from django.shortcuts import render
 from django.urls import reverse
 
@@ -15,41 +14,37 @@
     template_name="",
     multi=False,
     template_object_name="object",
 ):
 
     # The list of to obtained objects is in GET.id. No need to resume if we
     # didnt get it.
-    if not request.GET.get('id'):
-        msg = 'No list of objects given'
-        return HttpResponseBadRequest(settings.DEBUG and msg or '')
+    if not request.GET.get("id"):
+        msg = "No list of objects given"
+        return HttpResponseBadRequest(settings.DEBUG and msg or "")
 
-    # Given objects are either an integer or a comma-separted list of
+    # Given objects are either an integer or a comma-separated list of
     # integers. Validate them and ignore invalid values. Also strip them
     # in case the user entered values by hand, such as '1, 2,3'.
     object_list = []
-    for pk in request.GET['id'].split(","):
+    for pk in request.GET["id"].split(","):
         object_list.append(pk.strip())
 
     # Make sure this model exists and the user has 'change' permission for it.
     # If he doesnt have this permission, Django would not display the
     # change_list in the popup and the user were never able to select objects.
     try:
         model = apps.get_model(app_name, model_name)
     except LookupError:
-        msg = 'Model %s.%s does not exist.' % (app_name, model_name)
-        return HttpResponseBadRequest(settings.DEBUG and msg or '')
+        msg = "Model %s.%s does not exist." % (app_name, model_name)
+        return HttpResponseBadRequest(settings.DEBUG and msg or "")
 
     # Check 'view' or 'change' permission depending to Django's version
-    if VERSION[0] >= 2 and VERSION[1] >= 1:
-        if not request.user.has_perm('%s.view_%s' % (app_name, model_name)):
-            return HttpResponseForbidden()
-    else:
-        if not request.user.has_perm('%s.change_%s' % (app_name, model_name)):
-            return HttpResponseForbidden()
+    if not request.user.has_perm("%s.view_%s" % (app_name, model_name)):
+        return HttpResponseForbidden()
 
     try:
         if multi:
             model_template = "dynamic_raw_id/%s/multi_%s.html" % (
                 app_name,
                 model_name,
             )
@@ -70,14 +65,14 @@
             obj = model.objects.get(pk=object_list[0])
             change_url = reverse(
                 "admin:%s_%s_change" % (app_name, model_name), args=[obj.pk]
             )
             extra_context = {template_object_name: (obj, change_url)}
     # most likely the pk wasn't convertable
     except ValueError:
-        msg = 'ValueError during lookup'
-        return HttpResponseBadRequest(settings.DEBUG and msg or '')
+        msg = "ValueError during lookup"
+        return HttpResponseBadRequest(settings.DEBUG and msg or "")
     except model.DoesNotExist:
-        msg = 'Model instance does not exist'
-        return HttpResponseBadRequest(settings.DEBUG and msg or '')
+        msg = "Model instance does not exist"
+        return HttpResponseBadRequest(settings.DEBUG and msg or "")
 
     return render(request, (model_template, template_name), extra_context)
```

### Comparing `django-dynamic-raw-id-2.8/dynamic_raw_id/widgets.py` & `django-dynamic-raw-id-3.0/dynamic_raw_id/widgets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,73 @@
-from django import VERSION, forms
+from django import forms
 from django.conf import settings
 from django.contrib.admin import widgets
 from django.core.exceptions import ImproperlyConfigured
 from django.urls import reverse
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 
 
 class DynamicRawIDImproperlyConfigured(ImproperlyConfigured):
     pass
 
 
 class DynamicRawIDWidget(widgets.ForeignKeyRawIdWidget):
-    template_name = 'dynamic_raw_id/admin/widgets/dynamic_raw_id_field.html'
+    template_name = "dynamic_raw_id/admin/widgets/dynamic_raw_id_field.html"
 
     def get_context(self, name, value, attrs):
-        context = super(DynamicRawIDWidget, self).get_context(
-            name, value, attrs
-        )
-        model = self.rel.model if VERSION[0] >= 2 else self.rel.to
+        context = super(DynamicRawIDWidget, self).get_context(name, value, attrs)
+        model = self.rel.model
         related_url = reverse(
-            'admin:{0}_{1}_changelist'.format(
+            "admin:{0}_{1}_changelist".format(
                 model._meta.app_label, model._meta.object_name.lower()
             ),
             current_app=self.admin_site.name,
         )
 
         params = self.url_parameters()
         if params:
-            url = u'?' + u'&'.join(
-                [u'{0}={1}'.format(k, v) for k, v in params.items()]
-            )
+            url = u"?" + u"&".join([u"{0}={1}".format(k, v) for k, v in params.items()])
         else:
-            url = u''
+            url = u""
         if "class" not in attrs:
             attrs[
-                'class'
-            ] = 'vForeignKeyRawIdAdminField'  # The JavaScript looks for this hook.
+                "class"
+            ] = "vForeignKeyRawIdAdminField"  # The JavaScript looks for this hook.
         app_name = model._meta.app_label.strip()
         model_name = model._meta.object_name.lower().strip()
 
         context.update(
             {
-                'name': name,
-                'app_name': app_name,
-                'model_name': model_name,
-                'related_url': related_url,
-                'url': url,
+                "name": name,
+                "app_name": app_name,
+                "model_name": model_name,
+                "related_url": related_url,
+                "url": url,
             }
         )
         return context
 
     @property
     def media(self):
-        extra = '' if settings.DEBUG else '.min'
+        extra = "" if settings.DEBUG else ".min"
         return forms.Media(
             js=[
-                'admin/js/vendor/jquery/jquery{0}.js'.format(extra),
-                'admin/js/jquery.init.js',
-                'admin/js/core.js',
+                "admin/js/vendor/jquery/jquery{0}.js".format(extra),
+                "admin/js/jquery.init.js",
+                "admin/js/core.js",
                 "dynamic_raw_id/js/dynamic_raw_id.js",
             ]
         )
 
 
 class DynamicRawIDMultiIdWidget(DynamicRawIDWidget):
     def value_from_datadict(self, data, files, name):
         value = data.get(name)
         if value:
-            return value.split(u',')
+            return value.split(u",")
 
     def render(self, name, value, attrs, renderer=None):
-        attrs['class'] = 'vManyToManyRawIdAdminField'
-        value = u','.join([force_text(v) for v in value]) if value else ''
+        attrs["class"] = "vManyToManyRawIdAdminField"
+        value = u",".join([force_str(v) for v in value]) if value else ""
         return super(DynamicRawIDMultiIdWidget, self).render(
             name, value, attrs, renderer=renderer
         )
```

### Comparing `django-dynamic-raw-id-2.8/setup.cfg` & `django-dynamic-raw-id-3.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 [metadata]
 name = django-dynamic-raw-id
-version = 2.8
+version = 3.0
 description = raw_id_fields widget replacement that handles display of an object's string value on change.
 long_description = file: README.rst, CHANGELOG.rst
 author = Martin Mahner, Seth Buntin, Yann Malet
 author_email = info@lincolnloop.com
 url = https://github.com/lincolnloop/django-dynamic-raw-id
 keywords = django, widget, field, admin, raw-id, foreignkey
 license = MIT
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
-	Programming Language :: Python :: 2.7
-	Programming Language :: Python :: 3.5
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Framework :: Django
 
 [options]
 packages = find:
 include_package_data = True
 zip_safe = False
-python_requires = >=2.7
+python_requires = >=3.7
 install_requires = 
-	django>=1.11
-	six>=1.10.0
+	django>=3.2
 
 [options.extras_require]
 tests = 
 	selenium
 	coverage
 	pytest
 	pytest-cov
```

### Comparing `django-dynamic-raw-id-2.8/tox.ini` & `django-dynamic-raw-id-3.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 [tox]
 toxworkdir=/tmp/tox/django-dynamic-raw-id
 envlist=
   readme
   begin
-  py{27}-django-{111}
-  py{35,36}-django-{111,20,21,22}
-  py{37}-django-{21,22,30,31}
-  py{38}-django-{22,30,31}
+  py{37,38,39,310}-django-{32,40}
   end
 
 [testenv]
 install_command =
     pip install {opts} {packages}
 setenv =
     DJANGO_SETTINGS_MODULE=dynamic_raw_id.tests.testapp.settings
@@ -18,36 +15,33 @@
 extras=
     tests
 commands=
     {envbindir}/django-admin collectstatic --noinput -v0
     pytest --pyargs --cov={envsitepackagesdir}/dynamic_raw_id dynamic_raw_id
 deps=
     # Django versions
-    django-111: django==1.11.*
-    django-20: django==2.0.*
-    django-21: django==2.1.*
-    django-22: django==2.2.*
-    django-30: django==3.0.*
-    django-31: django==3.1.*
+    django-32: django==3.2.*
+    django-40: django==4.0.*
 
 [testenv:begin]
-basepython = python3.6
+basepython = python
 skip_install = True
 deps = coverage
 commands = coverage erase
 
 [testenv:end]
-basepython = python3.6
+basepython = python
 skip_install = True
 deps = coverage
 commands=
     coverage report
     coverage html
 
 [testenv:readme]
+basepython = python
 skip_install = True
 deps =
     docutils
     Pygments
 commands =
     rst2html.py --report=info --halt=warning README.rst /dev/null
     rst2html.py --report=info --halt=warning CHANGELOG.rst /dev/null
```


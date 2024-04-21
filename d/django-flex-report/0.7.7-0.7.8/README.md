# Comparing `tmp/django-flex-report-0.7.7.tar.gz` & `tmp/django-flex-report-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-flex-report-0.7.7.tar", last modified: Sun Apr 21 08:02:13 2024, max compression
+gzip compressed data, was "django-flex-report-0.7.8.tar", last modified: Sun Apr 21 11:44:48 2024, max compression
```

## Comparing `django-flex-report-0.7.7.tar` & `django-flex-report-0.7.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-21 08:02:13.261693 django-flex-report-0.7.7/
--rw-rw-r--   0 saman     (1000) saman     (1000)     1076 2024-03-28 15:09:39.000000 django-flex-report-0.7.7/LICENSE
--rw-rw-r--   0 saman     (1000) saman     (1000)      721 2024-03-28 15:09:39.000000 django-flex-report-0.7.7/MANIFEST.in
--rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-21 08:02:13.261693 django-flex-report-0.7.7/PKG-INFO
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-21 08:02:13.257692 django-flex-report-0.7.7/django_flex_report.egg-info/
--rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-21 08:02:13.000000 django-flex-report-0.7.7/django_flex_report.egg-info/PKG-INFO
--rw-rw-r--   0 saman     (1000) saman     (1000)     1734 2024-04-21 08:02:13.000000 django-flex-report-0.7.7/django_flex_report.egg-info/SOURCES.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-21 08:02:13.000000 django-flex-report-0.7.7/django_flex_report.egg-info/dependency_links.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-21 08:02:13.000000 django-flex-report-0.7.7/django_flex_report.egg-info/not-zip-safe
--rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-04-21 08:02:13.000000 django-flex-report-0.7.7/django_flex_report.egg-info/requires.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)       19 2024-04-21 08:02:13.000000 django-flex-report-0.7.7/django_flex_report.egg-info/top_level.txt
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-21 08:02:13.257692 django-flex-report-0.7.7/flex_report/
--rw-rw-r--   0 saman     (1000) saman     (1000)     1703 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)       57 2024-04-21 08:02:12.000000 django-flex-report-0.7.7/flex_report/_version.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2423 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/admin.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     4710 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/app_settings.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      149 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/apps.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      256 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/choices.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     3619 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/constants.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      707 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/fields.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     3985 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/filterset.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2483 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/forms.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      223 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/managers.py
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-21 08:02:13.257692 django-flex-report-0.7.7/flex_report/migrations/
--rw-rw-r--   0 saman     (1000) saman     (1000)     8753 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0001_initial.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      413 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0002_alter_column_title.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2362 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      767 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0004_column_creator.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      480 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0005_template_model_user_path.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      475 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0006_tablebutton_query_strings.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      755 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      715 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0008_template_buttons.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      616 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0009_alter_template_buttons.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1311 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0011_alter_template_model_user_path.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1323 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0013_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      573 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0014_alter_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      343 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0015_remove_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      547 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0016_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    14027 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/mixins.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     8886 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/models.py
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-21 08:02:13.257692 django-flex-report-0.7.7/flex_report/templatetags/
--rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/templatetags/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     5819 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/templatetags/flex_report_filters.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1674 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/urls.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    24135 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/utils.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    11732 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/views.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1666 2024-03-28 15:09:39.000000 django-flex-report-0.7.7/pyproject.toml
--rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-03-28 15:09:39.000000 django-flex-report-0.7.7/requirements.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)       38 2024-04-21 08:02:13.261693 django-flex-report-0.7.7/setup.cfg
--rw-rw-r--   0 saman     (1000) saman     (1000)       73 2024-03-28 15:09:39.000000 django-flex-report-0.7.7/setup.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-21 11:44:48.359199 django-flex-report-0.7.8/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1076 2024-03-28 15:09:39.000000 django-flex-report-0.7.8/LICENSE
+-rw-rw-r--   0 saman     (1000) saman     (1000)      721 2024-03-28 15:09:39.000000 django-flex-report-0.7.8/MANIFEST.in
+-rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-21 11:44:48.359199 django-flex-report-0.7.8/PKG-INFO
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-21 11:44:48.359199 django-flex-report-0.7.8/django_flex_report.egg-info/
+-rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-21 11:44:48.000000 django-flex-report-0.7.8/django_flex_report.egg-info/PKG-INFO
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1734 2024-04-21 11:44:48.000000 django-flex-report-0.7.8/django_flex_report.egg-info/SOURCES.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-21 11:44:48.000000 django-flex-report-0.7.8/django_flex_report.egg-info/dependency_links.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-21 11:44:48.000000 django-flex-report-0.7.8/django_flex_report.egg-info/not-zip-safe
+-rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-04-21 11:44:48.000000 django-flex-report-0.7.8/django_flex_report.egg-info/requires.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)       19 2024-04-21 11:44:48.000000 django-flex-report-0.7.8/django_flex_report.egg-info/top_level.txt
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-21 11:44:48.355209 django-flex-report-0.7.8/flex_report/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1703 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)       57 2024-04-21 11:44:47.000000 django-flex-report-0.7.8/flex_report/_version.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2423 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/admin.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     4710 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/app_settings.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      149 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/apps.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      256 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/choices.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     3619 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/constants.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      707 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/fields.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     3985 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/filterset.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2483 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/forms.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      223 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/managers.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-21 11:44:48.359199 django-flex-report-0.7.8/flex_report/migrations/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     8753 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/migrations/0001_initial.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      413 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/migrations/0002_alter_column_title.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2362 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      767 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/migrations/0004_column_creator.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      480 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/migrations/0005_template_model_user_path.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      475 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/migrations/0006_tablebutton_query_strings.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      755 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      715 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/migrations/0008_template_buttons.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      616 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/migrations/0009_alter_template_buttons.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1311 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/migrations/0011_alter_template_model_user_path.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1323 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/migrations/0013_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      573 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/migrations/0014_alter_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      343 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/migrations/0015_remove_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      547 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/migrations/0016_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/migrations/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    14027 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/mixins.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     8886 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/models.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-21 11:44:48.359199 django-flex-report-0.7.8/flex_report/templatetags/
+-rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/templatetags/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     5819 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/templatetags/flex_report_filters.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1674 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/urls.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    23910 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/utils.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    11732 2024-04-21 11:44:39.000000 django-flex-report-0.7.8/flex_report/views.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1666 2024-03-28 15:09:39.000000 django-flex-report-0.7.8/pyproject.toml
+-rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-03-28 15:09:39.000000 django-flex-report-0.7.8/requirements.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)       38 2024-04-21 11:44:48.359199 django-flex-report-0.7.8/setup.cfg
+-rw-rw-r--   0 saman     (1000) saman     (1000)       73 2024-03-28 15:09:39.000000 django-flex-report-0.7.8/setup.py
```

### Comparing `django-flex-report-0.7.7/LICENSE` & `django-flex-report-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/MANIFEST.in` & `django-flex-report-0.7.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/PKG-INFO` & `django-flex-report-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flex-report
-Version: 0.7.7
+Version: 0.7.8
 Summary: A Django app to create flexible reports
 Author-email: Saman Zand Haghighi <samanzandh@gmail.com>
 License: MIT
 Project-URL: Homepage, http://github.com/saman-zand-h/django-flex-report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-flex-report-0.7.7/django_flex_report.egg-info/PKG-INFO` & `django-flex-report-0.7.8/django_flex_report.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flex-report
-Version: 0.7.7
+Version: 0.7.8
 Summary: A Django app to create flexible reports
 Author-email: Saman Zand Haghighi <samanzandh@gmail.com>
 License: MIT
 Project-URL: Homepage, http://github.com/saman-zand-h/django-flex-report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-flex-report-0.7.7/django_flex_report.egg-info/SOURCES.txt` & `django-flex-report-0.7.8/django_flex_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/__init__.py` & `django-flex-report-0.7.8/flex_report/__init__.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/admin.py` & `django-flex-report-0.7.8/flex_report/admin.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/app_settings.py` & `django-flex-report-0.7.8/flex_report/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/constants.py` & `django-flex-report-0.7.8/flex_report/constants.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/fields.py` & `django-flex-report-0.7.8/flex_report/fields.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/filterset.py` & `django-flex-report-0.7.8/flex_report/filterset.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/forms.py` & `django-flex-report-0.7.8/flex_report/forms.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/migrations/0001_initial.py` & `django-flex-report-0.7.8/flex_report/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py` & `django-flex-report-0.7.8/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/migrations/0004_column_creator.py` & `django-flex-report-0.7.8/flex_report/migrations/0004_column_creator.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py` & `django-flex-report-0.7.8/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/migrations/0008_template_buttons.py` & `django-flex-report-0.7.8/flex_report/migrations/0008_template_buttons.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/migrations/0009_alter_template_buttons.py` & `django-flex-report-0.7.8/flex_report/migrations/0009_alter_template_buttons.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py` & `django-flex-report-0.7.8/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/migrations/0011_alter_template_model_user_path.py` & `django-flex-report-0.7.8/flex_report/migrations/0011_alter_template_model_user_path.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py` & `django-flex-report-0.7.8/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/migrations/0013_column_column_type.py` & `django-flex-report-0.7.8/flex_report/migrations/0013_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/migrations/0014_alter_column_column_type.py` & `django-flex-report-0.7.8/flex_report/migrations/0014_alter_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/migrations/0016_column_column_type.py` & `django-flex-report-0.7.8/flex_report/migrations/0016_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/mixins.py` & `django-flex-report-0.7.8/flex_report/mixins.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/models.py` & `django-flex-report-0.7.8/flex_report/models.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/templatetags/flex_report_filters.py` & `django-flex-report-0.7.8/flex_report/templatetags/flex_report_filters.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/urls.py` & `django-flex-report-0.7.8/flex_report/urls.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/flex_report/utils.py` & `django-flex-report-0.7.8/flex_report/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -424,39 +424,30 @@
 
 
 def get_column_cell(obj, name, *, absolute_url=True):
     """
     Takes in an object and a column name, and returns the value of the column for the object.
     If the column is a custom field, it returns the value of the custom field.
     """
-    model = obj._meta.model
+    model = obj._meta.model if hasattr(obj, "meta") else None
     
     if isinstance(name, DynamicSubField):
         return name.get_value(obj)
-    
-    if (
-        (custom_field_part := name.split("."))
-        and len(custom_field_part) > 1
-        and get_column_type(model, (custom_field_function_name := custom_field_part[0]))
-        == FieldTypes.custom
-    ):
-        custom_field_value = get_model_custom_field_value(
-            model, custom_field_function_name
-        )[custom_field_part[1]]
-        custom_field_function = getattr(obj, custom_field_function_name)
-        return custom_field_function(custom_field_value[0])
 
     if callable(name):
         return name(obj, name)
+    
+    if isinstance(obj, dict):
+        return obj.get(name, app_settings.DEFAULT_CELL_VALUE)
 
     attr = nested_getattr(obj, name, None, sep="__")
     if isinstance(attr, bool):
         return attr
 
-    if field := get_model_field(model, name):
+    if model and (field := get_model_field(model, name)):
         if (
             isinstance(attr, datetime.datetime)
             and type(field) in app_settings.TIME_FORMATS
         ):
             attr = jdatetime.datetime.fromgregorian(datetime=attr).strftime(
                 app_settings.TIME_FORMATS[type(field)]
             )
@@ -510,22 +501,25 @@
         
         workbook = xlwt.Workbook(encoding="utf-8")
         default_style = xlwt.XFStyle()
         sheet = workbook.add_sheet(sheet_name or str(nested_getattr(queryset, "model._meta.verbose_name_plural", "sheet")))
 
         for num, column in enumerate(columns):
             style, value = default_style, headers_name.get(column, column)
+            if isinstance(column, DynamicSubField):
+                value = column.get_verbose_name()
             style, value = cell_fn(obj=None, row_number=0, column=column, style=style, value=value)
             sheet.write(0, num, value, style)
         
         for x, obj in enumerate(queryset, start=1):
             for y, column in enumerate(columns):
                 style, value = default_style, get_column_cell(obj, column)
                 style, value = self._apply_cell_style_map(default_style, value)                    
                 style, value = cell_fn(obj=obj, row_number=x, column=column, style=style, value=value)
+                value = str(value).strip("_")
                 sheet.write(x, y, value, style or default_style)
 
         return workbook
 
     def handle(self):
         return self.export()
 
@@ -546,15 +540,14 @@
     def export(self):
         headers_name = self.get_export_headers()
         columns = headers_name.keys()
         queryset = self.get_export_qs()
         
         output = io.StringIO()
         writer = csv.writer(output)
-        breakpoint()
         writer.writerow([headers_name.get(column, column) for column in columns])
         writer.writerows([[get_column_cell(obj, column) for column in columns] for obj in queryset])
         return output
 
     def handle(self, *args, **kwargs):        
         return self.export()
```

### Comparing `django-flex-report-0.7.7/flex_report/views.py` & `django-flex-report-0.7.8/flex_report/views.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.7/pyproject.toml` & `django-flex-report-0.7.8/pyproject.toml`

 * *Files identical despite different names*


# Comparing `tmp/django-flex-report-0.7.6.tar.gz` & `tmp/django-flex-report-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-flex-report-0.7.6.tar", last modified: Fri Apr 19 16:10:04 2024, max compression
+gzip compressed data, was "django-flex-report-0.7.7.tar", last modified: Sun Apr 21 08:02:13 2024, max compression
```

## Comparing `django-flex-report-0.7.6.tar` & `django-flex-report-0.7.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-19 16:10:04.185084 django-flex-report-0.7.6/
--rw-rw-r--   0 saman     (1000) saman     (1000)     1076 2024-03-28 15:09:39.000000 django-flex-report-0.7.6/LICENSE
--rw-rw-r--   0 saman     (1000) saman     (1000)      721 2024-03-28 15:09:39.000000 django-flex-report-0.7.6/MANIFEST.in
--rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-19 16:10:04.185084 django-flex-report-0.7.6/PKG-INFO
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-19 16:10:04.185084 django-flex-report-0.7.6/django_flex_report.egg-info/
--rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-19 16:10:04.000000 django-flex-report-0.7.6/django_flex_report.egg-info/PKG-INFO
--rw-rw-r--   0 saman     (1000) saman     (1000)     1734 2024-04-19 16:10:04.000000 django-flex-report-0.7.6/django_flex_report.egg-info/SOURCES.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-19 16:10:04.000000 django-flex-report-0.7.6/django_flex_report.egg-info/dependency_links.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-19 16:10:04.000000 django-flex-report-0.7.6/django_flex_report.egg-info/not-zip-safe
--rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-04-19 16:10:04.000000 django-flex-report-0.7.6/django_flex_report.egg-info/requires.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)       19 2024-04-19 16:10:04.000000 django-flex-report-0.7.6/django_flex_report.egg-info/top_level.txt
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-19 16:10:04.185084 django-flex-report-0.7.6/flex_report/
--rw-rw-r--   0 saman     (1000) saman     (1000)     1703 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)       57 2024-04-19 16:10:03.000000 django-flex-report-0.7.6/flex_report/_version.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2423 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/admin.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     4710 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/app_settings.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      149 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/apps.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      256 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/choices.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     3745 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/constants.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      707 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/fields.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     3985 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/filterset.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2483 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/forms.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      223 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/managers.py
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-19 16:10:04.185084 django-flex-report-0.7.6/flex_report/migrations/
--rw-rw-r--   0 saman     (1000) saman     (1000)     8753 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0001_initial.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      413 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0002_alter_column_title.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2362 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      767 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0004_column_creator.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      480 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0005_template_model_user_path.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      475 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0006_tablebutton_query_strings.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      755 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      715 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0008_template_buttons.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      616 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0009_alter_template_buttons.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1311 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0011_alter_template_model_user_path.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1323 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0013_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      573 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0014_alter_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      343 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0015_remove_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      547 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0016_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    14027 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/mixins.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     8813 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/models.py
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-19 16:10:04.185084 django-flex-report-0.7.6/flex_report/templatetags/
--rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/templatetags/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     5819 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/templatetags/flex_report_filters.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1674 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/urls.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    24121 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/utils.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    11771 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/views.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1666 2024-03-28 15:09:39.000000 django-flex-report-0.7.6/pyproject.toml
--rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-03-28 15:09:39.000000 django-flex-report-0.7.6/requirements.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)       38 2024-04-19 16:10:04.185084 django-flex-report-0.7.6/setup.cfg
--rw-rw-r--   0 saman     (1000) saman     (1000)       73 2024-03-28 15:09:39.000000 django-flex-report-0.7.6/setup.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-21 08:02:13.261693 django-flex-report-0.7.7/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1076 2024-03-28 15:09:39.000000 django-flex-report-0.7.7/LICENSE
+-rw-rw-r--   0 saman     (1000) saman     (1000)      721 2024-03-28 15:09:39.000000 django-flex-report-0.7.7/MANIFEST.in
+-rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-21 08:02:13.261693 django-flex-report-0.7.7/PKG-INFO
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-21 08:02:13.257692 django-flex-report-0.7.7/django_flex_report.egg-info/
+-rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-21 08:02:13.000000 django-flex-report-0.7.7/django_flex_report.egg-info/PKG-INFO
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1734 2024-04-21 08:02:13.000000 django-flex-report-0.7.7/django_flex_report.egg-info/SOURCES.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-21 08:02:13.000000 django-flex-report-0.7.7/django_flex_report.egg-info/dependency_links.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-21 08:02:13.000000 django-flex-report-0.7.7/django_flex_report.egg-info/not-zip-safe
+-rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-04-21 08:02:13.000000 django-flex-report-0.7.7/django_flex_report.egg-info/requires.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)       19 2024-04-21 08:02:13.000000 django-flex-report-0.7.7/django_flex_report.egg-info/top_level.txt
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-21 08:02:13.257692 django-flex-report-0.7.7/flex_report/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1703 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)       57 2024-04-21 08:02:12.000000 django-flex-report-0.7.7/flex_report/_version.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2423 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/admin.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     4710 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/app_settings.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      149 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/apps.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      256 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/choices.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     3619 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/constants.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      707 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/fields.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     3985 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/filterset.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2483 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/forms.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      223 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/managers.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-21 08:02:13.257692 django-flex-report-0.7.7/flex_report/migrations/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     8753 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0001_initial.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      413 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0002_alter_column_title.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2362 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      767 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0004_column_creator.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      480 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0005_template_model_user_path.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      475 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0006_tablebutton_query_strings.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      755 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      715 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0008_template_buttons.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      616 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0009_alter_template_buttons.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1311 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0011_alter_template_model_user_path.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1323 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0013_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      573 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0014_alter_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      343 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0015_remove_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      547 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/0016_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/migrations/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    14027 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/mixins.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     8886 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/models.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-21 08:02:13.257692 django-flex-report-0.7.7/flex_report/templatetags/
+-rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/templatetags/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     5819 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/templatetags/flex_report_filters.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1674 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/urls.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    24135 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/utils.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    11732 2024-04-21 08:02:07.000000 django-flex-report-0.7.7/flex_report/views.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1666 2024-03-28 15:09:39.000000 django-flex-report-0.7.7/pyproject.toml
+-rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-03-28 15:09:39.000000 django-flex-report-0.7.7/requirements.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)       38 2024-04-21 08:02:13.261693 django-flex-report-0.7.7/setup.cfg
+-rw-rw-r--   0 saman     (1000) saman     (1000)       73 2024-03-28 15:09:39.000000 django-flex-report-0.7.7/setup.py
```

### Comparing `django-flex-report-0.7.6/LICENSE` & `django-flex-report-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/MANIFEST.in` & `django-flex-report-0.7.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/PKG-INFO` & `django-flex-report-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flex-report
-Version: 0.7.6
+Version: 0.7.7
 Summary: A Django app to create flexible reports
 Author-email: Saman Zand Haghighi <samanzandh@gmail.com>
 License: MIT
 Project-URL: Homepage, http://github.com/saman-zand-h/django-flex-report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-flex-report-0.7.6/django_flex_report.egg-info/PKG-INFO` & `django-flex-report-0.7.7/django_flex_report.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flex-report
-Version: 0.7.6
+Version: 0.7.7
 Summary: A Django app to create flexible reports
 Author-email: Saman Zand Haghighi <samanzandh@gmail.com>
 License: MIT
 Project-URL: Homepage, http://github.com/saman-zand-h/django-flex-report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-flex-report-0.7.6/django_flex_report.egg-info/SOURCES.txt` & `django-flex-report-0.7.7/django_flex_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/__init__.py` & `django-flex-report-0.7.7/flex_report/__init__.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/admin.py` & `django-flex-report-0.7.7/flex_report/admin.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/app_settings.py` & `django-flex-report-0.7.7/flex_report/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/constants.py` & `django-flex-report-0.7.7/flex_report/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,19 +41,18 @@
 
 
 class DynamicSubField:
     slug = None
     verbose_name = None
     
     def __init__(self, verbose_name=None):
-        if verbose_name:
-            self.verbose_name = verbose_name
+        self.verbose_name = verbose_name or self.verbose_name
     
     def get_verbose_name(self):
-        return self.verbose_name
+        return str(self.verbose_name)
     
     @abstractmethod
     def get_value(cls, *args, **kwargs):
         pass    
         
 
 class BaseDynamicField:
@@ -71,40 +70,37 @@
     
     @classmethod
     def register(cls, field):
         assert issubclass(field, cls)
         cls.fields.update({field.field_slug: field})
         return field
     
+    @classmethod
     @abstractmethod
-    def unpack_field(self, obj, *args, **kwargs) -> List[DynamicSubField]:
+    def unpack_field(cls, *args, **kwargs) -> List[DynamicSubField]:
         pass
     
 
 class BaseExportFormat:
     formats = {}
     format_slug = None
     format_name = None
     format_ext = None
     export_headers = {}
-    export_columns = []
     export_qs = []
     export_kwargs = {}
     export_filename = None
     
     def __init__(self, user=None, request=None):
         self.user = user
         self.request = request
     
     def get_export_headers(self):
         return self.export_headers
     
-    def get_export_columns(self):
-        return self.export_columns or self.get_export_headers().keys()
-    
     def get_export_kwargs(self):
         return self.export_kwargs
     
     def get_export_filename(self):
         return f"{self.export_filename or self.format_slug}{self.format_ext}"
     
     def get_export_qs(self):
```

### Comparing `django-flex-report-0.7.6/flex_report/fields.py` & `django-flex-report-0.7.7/flex_report/fields.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/filterset.py` & `django-flex-report-0.7.7/flex_report/filterset.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/forms.py` & `django-flex-report-0.7.7/flex_report/forms.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/migrations/0001_initial.py` & `django-flex-report-0.7.7/flex_report/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py` & `django-flex-report-0.7.7/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/migrations/0004_column_creator.py` & `django-flex-report-0.7.7/flex_report/migrations/0004_column_creator.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py` & `django-flex-report-0.7.7/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/migrations/0008_template_buttons.py` & `django-flex-report-0.7.7/flex_report/migrations/0008_template_buttons.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/migrations/0009_alter_template_buttons.py` & `django-flex-report-0.7.7/flex_report/migrations/0009_alter_template_buttons.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py` & `django-flex-report-0.7.7/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/migrations/0011_alter_template_model_user_path.py` & `django-flex-report-0.7.7/flex_report/migrations/0011_alter_template_model_user_path.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py` & `django-flex-report-0.7.7/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/migrations/0013_column_column_type.py` & `django-flex-report-0.7.7/flex_report/migrations/0013_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/migrations/0014_alter_column_column_type.py` & `django-flex-report-0.7.7/flex_report/migrations/0014_alter_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/migrations/0016_column_column_type.py` & `django-flex-report-0.7.7/flex_report/migrations/0016_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/mixins.py` & `django-flex-report-0.7.7/flex_report/mixins.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/models.py` & `django-flex-report-0.7.7/flex_report/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,19 @@
     def get_dynamic_obj(self) -> None | BaseDynamicField:
         if self.column_type != self.COLUMN_TYPES.dynamic:
             return
         
         return dynamic_field.get_by_slug(self.title)
 
     def clean(self):
-        if (column_type:=get_column_type(self.model, self.title)) == FieldTypes.dynamic and self.model != (dynamic_model:=self.get_dynamic_obj().model):
+        if (
+            (column_type:=get_column_type(self.model, self.title)) == FieldTypes.dynamic 
+            and (dynamic_field:=self.get_dynamic_obj()).model
+            and self.model != dynamic_field.model
+        ):
             raise ValidationError({"title": _("This dynamic column has been registered for another model, which is %(title).") % {"title": dynamic_field}})
         
         if column_type and not is_field_valid(self.model.model_class(), self.title):
             raise ValidationError(
                 {
                     "title": _(
                         "The field name is not valid. It should be a field on the model."
```

### Comparing `django-flex-report-0.7.6/flex_report/templatetags/flex_report_filters.py` & `django-flex-report-0.7.7/flex_report/templatetags/flex_report_filters.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/urls.py` & `django-flex-report-0.7.7/flex_report/urls.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.6/flex_report/utils.py` & `django-flex-report-0.7.7/flex_report/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,17 +499,17 @@
         return style, value
     
     def _default_cell_fn(self, style, value, *args, **kwargs):
         return style, value
     
     def export(self):
         headers_name = self.get_export_headers()
-        columns = self.get_export_columns()
+        columns = headers_name.keys()
         queryset = self.get_export_qs()
-        sheet_name = self.get_export_kwargs().get("sheet_name", "default")
+        sheet_name = str(self.get_export_kwargs().get("sheet_name", "default"))
         cell_fn = self.get_export_kwargs().get("cell_fn", self._default_cell_fn)
         
         workbook = xlwt.Workbook(encoding="utf-8")
         default_style = xlwt.XFStyle()
         sheet = workbook.add_sheet(sheet_name or str(nested_getattr(queryset, "model._meta.verbose_name_plural", "sheet")))
 
         for num, column in enumerate(columns):
@@ -541,19 +541,20 @@
 class ExportCsv(BaseExportFormat):
     format_slug = "csv"
     format_name = "CSV"
     format_ext = ".csv"
 
     def export(self):
         headers_name = self.get_export_headers()
-        columns = self.get_export_columns()
+        columns = headers_name.keys()
         queryset = self.get_export_qs()
         
         output = io.StringIO()
         writer = csv.writer(output)
+        breakpoint()
         writer.writerow([headers_name.get(column, column) for column in columns])
         writer.writerows([[get_column_cell(obj, column) for column in columns] for obj in queryset])
         return output
 
     def handle(self, *args, **kwargs):        
         return self.export()
```

### Comparing `django-flex-report-0.7.6/flex_report/views.py` & `django-flex-report-0.7.7/flex_report/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -379,20 +379,19 @@
         columns = OrderedDict()
         for col in self.template_columns:
             if get_column_type(self.report_model, col.title) != FieldTypes.dynamic:
                 columns[col.title] = str(get_column_verbose_name(self.report_model, col.title))
                 continue
                 
             columns.update({
-                subfield: str(subfield.verbose_name)
+                subfield: str(subfield.get_verbose_name())
                 for subfield in col.get_dynamic_obj().unpack_field()
             })
                 
         self.export_qs = self.report_qs
-        self.export_columns = columns.keys()
         self.export_headers = columns
 
         return super().get(*args, **kwargs)
 
     def template_not_ready(self):
         raise Http404
```

### Comparing `django-flex-report-0.7.6/pyproject.toml` & `django-flex-report-0.7.7/pyproject.toml`

 * *Files identical despite different names*


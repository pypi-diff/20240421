# Comparing `tmp/django_log_inspector-0.0.5.tar.gz` & `tmp/django_log_inspector-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_log_inspector-0.0.5.tar", last modified: Tue Apr 16 13:18:06 2024, max compression
+gzip compressed data, was "django_log_inspector-0.0.6.tar", last modified: Sun Apr 21 10:31:17 2024, max compression
```

## Comparing `django_log_inspector-0.0.5.tar` & `django_log_inspector-0.0.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.383461 django_log_inspector-0.0.5/
--rw-r--r--   0 peyman627   (501) staff       (20)     1071 2024-01-23 09:55:45.000000 django_log_inspector-0.0.5/LICENSE
--rw-r--r--   0 peyman627   (501) staff       (20)      100 2024-01-23 12:18:13.000000 django_log_inspector-0.0.5/MANIFEST.in
--rw-r--r--   0 peyman627   (501) staff       (20)     3430 2024-04-16 13:18:06.383265 django_log_inspector-0.0.5/PKG-INFO
--rw-r--r--   0 peyman627   (501) staff       (20)     1838 2024-04-16 13:17:59.000000 django_log_inspector-0.0.5/README.md
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.383080 django_log_inspector-0.0.5/django_log_inspector.egg-info/
--rw-r--r--   0 peyman627   (501) staff       (20)     3430 2024-04-16 13:18:06.000000 django_log_inspector-0.0.5/django_log_inspector.egg-info/PKG-INFO
--rw-r--r--   0 peyman627   (501) staff       (20)     1002 2024-04-16 13:18:06.000000 django_log_inspector-0.0.5/django_log_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 peyman627   (501) staff       (20)        1 2024-04-16 13:18:06.000000 django_log_inspector-0.0.5/django_log_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 peyman627   (501) staff       (20)       14 2024-04-16 13:18:06.000000 django_log_inspector-0.0.5/django_log_inspector.egg-info/top_level.txt
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.378677 django_log_inspector-0.0.5/log_inspector/
--rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.5/log_inspector/__init__.py
--rw-r--r--   0 peyman627   (501) staff       (20)       63 2024-01-23 09:38:31.000000 django_log_inspector-0.0.5/log_inspector/admin.py
--rw-r--r--   0 peyman627   (501) staff       (20)      163 2024-01-23 10:07:05.000000 django_log_inspector-0.0.5/log_inspector/apps.py
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.378905 django_log_inspector-0.0.5/log_inspector/migrations/
--rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.5/log_inspector/migrations/__init__.py
--rw-r--r--   0 peyman627   (501) staff       (20)       57 2024-01-23 09:38:31.000000 django_log_inspector-0.0.5/log_inspector/models.py
--rw-r--r--   0 peyman627   (501) staff       (20)      985 2024-01-23 10:07:05.000000 django_log_inspector-0.0.5/log_inspector/settings.py
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.375085 django_log_inspector-0.0.5/log_inspector/static/
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.375210 django_log_inspector-0.0.5/log_inspector/static/log_inspector/
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.379220 django_log_inspector-0.0.5/log_inspector/static/log_inspector/css/
--rw-r--r--   0 peyman627   (501) staff       (20)     2023 2024-04-16 12:26:40.000000 django_log_inspector-0.0.5/log_inspector/static/log_inspector/css/input.css
--rw-r--r--   0 peyman627   (501) staff       (20)    10025 2024-04-16 13:11:49.000000 django_log_inspector-0.0.5/log_inspector/static/log_inspector/css/output.css
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.380267 django_log_inspector-0.0.5/log_inspector/static/log_inspector/js/
--rw-r--r--   0 peyman627   (501) staff       (20)    43440 2024-01-05 17:19:20.000000 django_log_inspector-0.0.5/log_inspector/static/log_inspector/js/alpinejs.min.js
--rw-r--r--   0 peyman627   (501) staff       (20)    47755 2024-01-05 17:17:16.000000 django_log_inspector-0.0.5/log_inspector/static/log_inspector/js/htmx.min.js
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.375334 django_log_inspector-0.0.5/log_inspector/templates/
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.382711 django_log_inspector-0.0.5/log_inspector/templates/log_inspector/
--rw-r--r--   0 peyman627   (501) staff       (20)     9719 2024-04-16 13:11:49.000000 django_log_inspector-0.0.5/log_inspector/templates/log_inspector/home.html
--rw-r--r--   0 peyman627   (501) staff       (20)     1852 2024-04-16 13:11:49.000000 django_log_inspector-0.0.5/log_inspector/templates/log_inspector/log_entries_data.html
--rw-r--r--   0 peyman627   (501) staff       (20)      686 2024-04-16 10:49:36.000000 django_log_inspector-0.0.5/log_inspector/templates/log_inspector/log_entries_table.html
--rw-r--r--   0 peyman627   (501) staff       (20)      988 2024-04-16 13:11:49.000000 django_log_inspector-0.0.5/log_inspector/templates/log_inspector/log_files.html
--rw-r--r--   0 peyman627   (501) staff       (20)     2645 2024-02-05 11:01:20.000000 django_log_inspector-0.0.5/log_inspector/templates/log_inspector/pagination.html
--rw-r--r--   0 peyman627   (501) staff       (20)     1027 2024-04-16 10:25:08.000000 django_log_inspector-0.0.5/log_inspector/templates/log_inspector/start_live.html
--rw-r--r--   0 peyman627   (501) staff       (20)       60 2024-01-23 09:38:31.000000 django_log_inspector-0.0.5/log_inspector/tests.py
--rw-r--r--   0 peyman627   (501) staff       (20)      700 2024-04-15 12:22:26.000000 django_log_inspector-0.0.5/log_inspector/urls.py
--rw-r--r--   0 peyman627   (501) staff       (20)     2660 2024-04-16 12:09:32.000000 django_log_inspector-0.0.5/log_inspector/utils.py
--rw-r--r--   0 peyman627   (501) staff       (20)     3627 2024-04-16 11:12:12.000000 django_log_inspector-0.0.5/log_inspector/views.py
--rw-r--r--   0 peyman627   (501) staff       (20)      388 2024-04-16 13:17:59.000000 django_log_inspector-0.0.5/pyproject.toml
--rw-r--r--   0 peyman627   (501) staff       (20)       38 2024-04-16 13:18:06.383499 django_log_inspector-0.0.5/setup.cfg
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.066179 django_log_inspector-0.0.6/
+-rw-r--r--   0 peyman627   (501) staff       (20)     1071 2024-01-23 09:55:45.000000 django_log_inspector-0.0.6/LICENSE
+-rw-r--r--   0 peyman627   (501) staff       (20)      100 2024-01-23 12:18:13.000000 django_log_inspector-0.0.6/MANIFEST.in
+-rw-r--r--   0 peyman627   (501) staff       (20)     4109 2024-04-21 10:31:17.065987 django_log_inspector-0.0.6/PKG-INFO
+-rw-r--r--   0 peyman627   (501) staff       (20)     2229 2024-04-21 10:12:03.000000 django_log_inspector-0.0.6/README.md
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.065629 django_log_inspector-0.0.6/django_log_inspector.egg-info/
+-rw-r--r--   0 peyman627   (501) staff       (20)     4109 2024-04-21 10:31:17.000000 django_log_inspector-0.0.6/django_log_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 peyman627   (501) staff       (20)     1002 2024-04-21 10:31:17.000000 django_log_inspector-0.0.6/django_log_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 peyman627   (501) staff       (20)        1 2024-04-21 10:31:17.000000 django_log_inspector-0.0.6/django_log_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 peyman627   (501) staff       (20)       14 2024-04-21 10:31:17.000000 django_log_inspector-0.0.6/django_log_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.059817 django_log_inspector-0.0.6/log_inspector/
+-rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.6/log_inspector/__init__.py
+-rw-r--r--   0 peyman627   (501) staff       (20)       63 2024-01-23 09:38:31.000000 django_log_inspector-0.0.6/log_inspector/admin.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      163 2024-01-23 10:07:05.000000 django_log_inspector-0.0.6/log_inspector/apps.py
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.060217 django_log_inspector-0.0.6/log_inspector/migrations/
+-rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.6/log_inspector/migrations/__init__.py
+-rw-r--r--   0 peyman627   (501) staff       (20)       57 2024-01-23 09:38:31.000000 django_log_inspector-0.0.6/log_inspector/models.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      866 2024-04-21 08:26:12.000000 django_log_inspector-0.0.6/log_inspector/settings.py
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.056187 django_log_inspector-0.0.6/log_inspector/static/
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.056360 django_log_inspector-0.0.6/log_inspector/static/log_inspector/
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.060623 django_log_inspector-0.0.6/log_inspector/static/log_inspector/css/
+-rw-r--r--   0 peyman627   (501) staff       (20)     2023 2024-04-16 12:26:40.000000 django_log_inspector-0.0.6/log_inspector/static/log_inspector/css/input.css
+-rw-r--r--   0 peyman627   (501) staff       (20)    10025 2024-04-16 13:11:49.000000 django_log_inspector-0.0.6/log_inspector/static/log_inspector/css/output.css
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.062240 django_log_inspector-0.0.6/log_inspector/static/log_inspector/js/
+-rw-r--r--   0 peyman627   (501) staff       (20)    43440 2024-01-05 17:19:20.000000 django_log_inspector-0.0.6/log_inspector/static/log_inspector/js/alpinejs.min.js
+-rw-r--r--   0 peyman627   (501) staff       (20)    47755 2024-01-05 17:17:16.000000 django_log_inspector-0.0.6/log_inspector/static/log_inspector/js/htmx.min.js
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.056495 django_log_inspector-0.0.6/log_inspector/templates/
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.065322 django_log_inspector-0.0.6/log_inspector/templates/log_inspector/
+-rw-r--r--   0 peyman627   (501) staff       (20)     9719 2024-04-16 13:11:49.000000 django_log_inspector-0.0.6/log_inspector/templates/log_inspector/home.html
+-rw-r--r--   0 peyman627   (501) staff       (20)     1852 2024-04-16 13:11:49.000000 django_log_inspector-0.0.6/log_inspector/templates/log_inspector/log_entries_data.html
+-rw-r--r--   0 peyman627   (501) staff       (20)      686 2024-04-16 10:49:36.000000 django_log_inspector-0.0.6/log_inspector/templates/log_inspector/log_entries_table.html
+-rw-r--r--   0 peyman627   (501) staff       (20)      988 2024-04-16 13:11:49.000000 django_log_inspector-0.0.6/log_inspector/templates/log_inspector/log_files.html
+-rw-r--r--   0 peyman627   (501) staff       (20)     2645 2024-02-05 11:01:20.000000 django_log_inspector-0.0.6/log_inspector/templates/log_inspector/pagination.html
+-rw-r--r--   0 peyman627   (501) staff       (20)     1027 2024-04-16 10:25:08.000000 django_log_inspector-0.0.6/log_inspector/templates/log_inspector/start_live.html
+-rw-r--r--   0 peyman627   (501) staff       (20)       60 2024-01-23 09:38:31.000000 django_log_inspector-0.0.6/log_inspector/tests.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      700 2024-04-15 12:22:26.000000 django_log_inspector-0.0.6/log_inspector/urls.py
+-rw-r--r--   0 peyman627   (501) staff       (20)     2660 2024-04-16 12:09:32.000000 django_log_inspector-0.0.6/log_inspector/utils.py
+-rw-r--r--   0 peyman627   (501) staff       (20)     3627 2024-04-16 11:12:12.000000 django_log_inspector-0.0.6/log_inspector/views.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      779 2024-04-21 10:28:42.000000 django_log_inspector-0.0.6/pyproject.toml
+-rw-r--r--   0 peyman627   (501) staff       (20)       38 2024-04-21 10:31:17.066333 django_log_inspector-0.0.6/setup.cfg
```

### Comparing `django_log_inspector-0.0.5/LICENSE` & `django_log_inspector-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.5/PKG-INFO` & `django_log_inspector-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: django-log-inspector
-Version: 0.0.5
+Version: 0.0.6
 Summary: Read and Download log files
 Author-email: Peyman Hassani <hassani.peyman627@gmail.com>, Shaghayegh Valadkhani <valadkhani.sh@gmail.com>
+Maintainer-email: Peyman Hassani <hassani.peyman627@gmail.com>, Shaghayegh Valadkhani <valadkhani.sh@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Peyman Hassani
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -22,63 +23,91 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/peyzor/django-log-inspector
+Keywords: Django,logging,log viewer,real-time monitoring,log analysis,troubleshooting,log management,log files,log monitoring,debugging,Python web development,development tool
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Log Inspector
 
 ## _Fast and Live view to your log files_
 
-![version](https://img.shields.io/badge/version-0.0.5-blue.svg)
+![version](https://img.shields.io/badge/version-0.0.6-blue.svg)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 <a href="https://github.com/peyzor/django-log-inspector"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
 
 Django Log Inspector offers real-time monitoring and analysis of log files in Django projects.
-It delivers a fast and live view of log data, eliminating manual page refreshing.
+It delivers a fast and live-view of log data, eliminating manual page refreshing.
 With an intuitive interface and live update functionality, it streamlines log file management for easier issue tracking
 and troubleshooting in Django applications.
 
 Django Log Inspector is available directly from <a href="https://pypi.org/project/django-log-inspector/">PyPI</a>:
 
 ## Installation
 
 ```
 pip install django-log-inspector
-```
+``` 
 
 Add in INSTALLED_APPS
 
 ```
 installed_apps = [
     ...
     'log_inspector',
 ]
 ```
 
 Include in the URLconf
 
 ```
-path('logs/', include('log_inspector.urls')),
+path('logs/', include('log_inspector.urls'))
 ```
 
-
 ## Settings
 
+The directory of log files in your project
+
 ```
- LOG_INSPECTOR_FILES = ['logfile1', 'logfile2', ...]
- LOG_INSPECTOR_FILES_PATTERN = '*.log*'
  LOG_INSPECTOR_FILES_DIR = 'logs/'
- LOG_INSPECTOR_PAGE_LENGTH = 25       # total log lines per-page
- LOG_INSPECTOR_MAX_READ_LINES = 1000  # total log lines will be read
- LOG_INSPECTOR_FILE_LIST_MAX_ITEMS_PER_PAGE = 25 # Max log files loaded in Datatable per page
+```
+
+A file is included if the pattern is matched, or it is specified
+
+```
+ LOG_INSPECTOR_FILES = ['logfile1', 'logfile2', ...] # default: []
+ LOG_INSPECTOR_FILES_PATTERN = '*.log*'            
+```
+
+You must specify the patterns in which your log files start with
+
+```
  LOG_INSPECTOR_PATTERNS = ['[INFO]', '[DEBUG]', '[WARNING]', '[ERROR]', '[CRITICAL]']
- LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None  # String regex expression to exclude the log from line
+```
 
- # Optionally you can set the next variables in order to customize the admin:
- LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title"
- LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css"
+How logs are displayed
+
+```
+ LOG_INSPECTOR_PAGE_LENGTH = 25             # total log lines per-page
+ LOG_INSPECTOR_MAX_READ_LINES = 1000        # total log lines that are read
+ LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None  # String regex expression to exclude the log
+```
+
+Optionally you can set the next variables in order to customize
+
+```
+LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title"               # default: None
+LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css" # default: None
+```
+
+## Login
+
+Logs are only accessible to logged-in superusers.
+If your login URL is different from Django's default, specify it in your settings.
+
+```
+LOGIN_URL = '/my-custom-admin/login/'
 ```
```

#### html2text {}

```diff
@@ -1,10 +1,12 @@
-Metadata-Version: 2.1 Name: django-log-inspector Version: 0.0.5 Summary: Read
+Metadata-Version: 2.1 Name: django-log-inspector Version: 0.0.6 Summary: Read
 and Download log files Author-email: Peyman Hassani
 gmail.com>, Shaghayegh Valadkhani
+gmail.com> Maintainer-email: Peyman Hassani
+gmail.com>, Shaghayegh Valadkhani
 gmail.com> License: MIT License Copyright (c) 2024 Peyman Hassani Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
@@ -12,29 +14,36 @@
 the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/peyzor/
-django-log-inspector Description-Content-Type: text/markdown License-File:
-LICENSE # Django Log Inspector ## _Fast and Live view to your log files_ !
-[version](https://img.shields.io/badge/version-0.0.5-blue.svg) [![Open Source]
-(https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://
-opensource.org/) _[_G_i_t_H_u_b_]Django Log Inspector offers real-time monitoring and
-analysis of log files in Django projects. It delivers a fast and live view of
-log data, eliminating manual page refreshing. With an intuitive interface and
-live update functionality, it streamlines log file management for easier issue
-tracking and troubleshooting in Django applications. Django Log Inspector is
-available directly from _P_y_P_I: ## Installation ``` pip install django-log-
-inspector ``` Add in INSTALLED_APPS ``` installed_apps = [ ... 'log_inspector',
-] ``` Include in the URLconf ``` path('logs/', include('log_inspector.urls')),
-``` ## Settings ``` LOG_INSPECTOR_FILES = ['logfile1', 'logfile2', ...]
-LOG_INSPECTOR_FILES_PATTERN = '*.log*' LOG_INSPECTOR_FILES_DIR = 'logs/
-' LOG_INSPECTOR_PAGE_LENGTH = 25 # total log lines per-page
-LOG_INSPECTOR_MAX_READ_LINES = 1000 # total log lines will be read
-LOG_INSPECTOR_FILE_LIST_MAX_ITEMS_PER_PAGE = 25 # Max log files loaded in
-Datatable per page LOG_INSPECTOR_PATTERNS = ['[INFO]', '[DEBUG]', '[WARNING]',
-'[ERROR]', '[CRITICAL]'] LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None # String
-regex expression to exclude the log from line # Optionally you can set the next
-variables in order to customize the admin: LOG_INSPECTOR_FILE_LIST_TITLE =
-"Custom title" LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css" ```
+django-log-inspector Keywords: Django,logging,log viewer,real-time
+monitoring,log analysis,troubleshooting,log management,log files,log
+monitoring,debugging,Python web development,development tool Description-
+Content-Type: text/markdown License-File: LICENSE # Django Log Inspector ##
+_Fast and Live view to your log files_ ![version](https://img.shields.io/badge/
+version-0.0.6-blue.svg) [![Open Source](https://badges.frapsoft.com/os/v1/open-
+source.svg?v=103)](https://opensource.org/) _[_G_i_t_H_u_b_]Django Log Inspector offers
+real-time monitoring and analysis of log files in Django projects. It delivers
+a fast and live-view of log data, eliminating manual page refreshing. With an
+intuitive interface and live update functionality, it streamlines log file
+management for easier issue tracking and troubleshooting in Django
+applications. Django Log Inspector is available directly from _P_y_P_I: ##
+Installation ``` pip install django-log-inspector ``` Add in INSTALLED_APPS ```
+installed_apps = [ ... 'log_inspector', ] ``` Include in the URLconf ``` path
+('logs/', include('log_inspector.urls')) ``` ## Settings The directory of log
+files in your project ``` LOG_INSPECTOR_FILES_DIR = 'logs/' ``` A file is
+included if the pattern is matched, or it is specified ``` LOG_INSPECTOR_FILES
+= ['logfile1', 'logfile2', ...] # default: [] LOG_INSPECTOR_FILES_PATTERN =
+'*.log*' ``` You must specify the patterns in which your log files start with
+``` LOG_INSPECTOR_PATTERNS = ['[INFO]', '[DEBUG]', '[WARNING]', '[ERROR]', '
+[CRITICAL]'] ``` How logs are displayed ``` LOG_INSPECTOR_PAGE_LENGTH = 25 #
+total log lines per-page LOG_INSPECTOR_MAX_READ_LINES = 1000 # total log lines
+that are read LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None # String regex
+expression to exclude the log ``` Optionally you can set the next variables in
+order to customize ``` LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title" #
+default: None LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css" #
+default: None ``` ## Login Logs are only accessible to logged-in superusers. If
+your login URL is different from Django's default, specify it in your settings.
+``` LOGIN_URL = '/my-custom-admin/login/' ```
```

### Comparing `django_log_inspector-0.0.5/README.md` & `django_log_inspector-0.0.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,80 @@
 # Django Log Inspector
 
 ## _Fast and Live view to your log files_
 
-![version](https://img.shields.io/badge/version-0.0.5-blue.svg)
+![version](https://img.shields.io/badge/version-0.0.6-blue.svg)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 <a href="https://github.com/peyzor/django-log-inspector"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
 
 Django Log Inspector offers real-time monitoring and analysis of log files in Django projects.
-It delivers a fast and live view of log data, eliminating manual page refreshing.
+It delivers a fast and live-view of log data, eliminating manual page refreshing.
 With an intuitive interface and live update functionality, it streamlines log file management for easier issue tracking
 and troubleshooting in Django applications.
 
 Django Log Inspector is available directly from <a href="https://pypi.org/project/django-log-inspector/">PyPI</a>:
 
 ## Installation
 
 ```
 pip install django-log-inspector
-```
+``` 
 
 Add in INSTALLED_APPS
 
 ```
 installed_apps = [
     ...
     'log_inspector',
 ]
 ```
 
 Include in the URLconf
 
 ```
-path('logs/', include('log_inspector.urls')),
+path('logs/', include('log_inspector.urls'))
 ```
 
-
 ## Settings
 
+The directory of log files in your project
+
 ```
- LOG_INSPECTOR_FILES = ['logfile1', 'logfile2', ...]
- LOG_INSPECTOR_FILES_PATTERN = '*.log*'
  LOG_INSPECTOR_FILES_DIR = 'logs/'
- LOG_INSPECTOR_PAGE_LENGTH = 25       # total log lines per-page
- LOG_INSPECTOR_MAX_READ_LINES = 1000  # total log lines will be read
- LOG_INSPECTOR_FILE_LIST_MAX_ITEMS_PER_PAGE = 25 # Max log files loaded in Datatable per page
+```
+
+A file is included if the pattern is matched, or it is specified
+
+```
+ LOG_INSPECTOR_FILES = ['logfile1', 'logfile2', ...] # default: []
+ LOG_INSPECTOR_FILES_PATTERN = '*.log*'            
+```
+
+You must specify the patterns in which your log files start with
+
+```
  LOG_INSPECTOR_PATTERNS = ['[INFO]', '[DEBUG]', '[WARNING]', '[ERROR]', '[CRITICAL]']
- LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None  # String regex expression to exclude the log from line
+```
 
- # Optionally you can set the next variables in order to customize the admin:
- LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title"
- LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css"
+How logs are displayed
+
+```
+ LOG_INSPECTOR_PAGE_LENGTH = 25             # total log lines per-page
+ LOG_INSPECTOR_MAX_READ_LINES = 1000        # total log lines that are read
+ LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None  # String regex expression to exclude the log
+```
+
+Optionally you can set the next variables in order to customize
+
+```
+LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title"               # default: None
+LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css" # default: None
+```
+
+## Login
+
+Logs are only accessible to logged-in superusers.
+If your login URL is different from Django's default, specify it in your settings.
+
+```
+LOGIN_URL = '/my-custom-admin/login/'
 ```
```

#### html2text {}

```diff
@@ -1,21 +1,26 @@
 # Django Log Inspector ## _Fast and Live view to your log files_ ![version]
-(https://img.shields.io/badge/version-0.0.5-blue.svg) [![Open Source](https://
+(https://img.shields.io/badge/version-0.0.6-blue.svg) [![Open Source](https://
 badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 _[_G_i_t_H_u_b_]Django Log Inspector offers real-time monitoring and analysis of log
-files in Django projects. It delivers a fast and live view of log data,
+files in Django projects. It delivers a fast and live-view of log data,
 eliminating manual page refreshing. With an intuitive interface and live update
 functionality, it streamlines log file management for easier issue tracking and
 troubleshooting in Django applications. Django Log Inspector is available
 directly from _P_y_P_I: ## Installation ``` pip install django-log-inspector ```
 Add in INSTALLED_APPS ``` installed_apps = [ ... 'log_inspector', ] ``` Include
-in the URLconf ``` path('logs/', include('log_inspector.urls')), ``` ##
-Settings ``` LOG_INSPECTOR_FILES = ['logfile1', 'logfile2', ...]
-LOG_INSPECTOR_FILES_PATTERN = '*.log*' LOG_INSPECTOR_FILES_DIR = 'logs/
-' LOG_INSPECTOR_PAGE_LENGTH = 25 # total log lines per-page
-LOG_INSPECTOR_MAX_READ_LINES = 1000 # total log lines will be read
-LOG_INSPECTOR_FILE_LIST_MAX_ITEMS_PER_PAGE = 25 # Max log files loaded in
-Datatable per page LOG_INSPECTOR_PATTERNS = ['[INFO]', '[DEBUG]', '[WARNING]',
-'[ERROR]', '[CRITICAL]'] LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None # String
-regex expression to exclude the log from line # Optionally you can set the next
-variables in order to customize the admin: LOG_INSPECTOR_FILE_LIST_TITLE =
-"Custom title" LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css" ```
+in the URLconf ``` path('logs/', include('log_inspector.urls')) ``` ## Settings
+The directory of log files in your project ``` LOG_INSPECTOR_FILES_DIR = 'logs/
+' ``` A file is included if the pattern is matched, or it is specified ```
+LOG_INSPECTOR_FILES = ['logfile1', 'logfile2', ...] # default: []
+LOG_INSPECTOR_FILES_PATTERN = '*.log*' ``` You must specify the patterns in
+which your log files start with ``` LOG_INSPECTOR_PATTERNS = ['[INFO]', '
+[DEBUG]', '[WARNING]', '[ERROR]', '[CRITICAL]'] ``` How logs are displayed ```
+LOG_INSPECTOR_PAGE_LENGTH = 25 # total log lines per-page
+LOG_INSPECTOR_MAX_READ_LINES = 1000 # total log lines that are read
+LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None # String regex expression to exclude
+the log ``` Optionally you can set the next variables in order to customize ```
+LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title" # default: None
+LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css" # default: None
+``` ## Login Logs are only accessible to logged-in superusers. If your login
+URL is different from Django's default, specify it in your settings. ```
+LOGIN_URL = '/my-custom-admin/login/' ```
```

### Comparing `django_log_inspector-0.0.5/django_log_inspector.egg-info/PKG-INFO` & `django_log_inspector-0.0.6/django_log_inspector.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: django-log-inspector
-Version: 0.0.5
+Version: 0.0.6
 Summary: Read and Download log files
 Author-email: Peyman Hassani <hassani.peyman627@gmail.com>, Shaghayegh Valadkhani <valadkhani.sh@gmail.com>
+Maintainer-email: Peyman Hassani <hassani.peyman627@gmail.com>, Shaghayegh Valadkhani <valadkhani.sh@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Peyman Hassani
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -22,63 +23,91 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/peyzor/django-log-inspector
+Keywords: Django,logging,log viewer,real-time monitoring,log analysis,troubleshooting,log management,log files,log monitoring,debugging,Python web development,development tool
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Log Inspector
 
 ## _Fast and Live view to your log files_
 
-![version](https://img.shields.io/badge/version-0.0.5-blue.svg)
+![version](https://img.shields.io/badge/version-0.0.6-blue.svg)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 <a href="https://github.com/peyzor/django-log-inspector"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
 
 Django Log Inspector offers real-time monitoring and analysis of log files in Django projects.
-It delivers a fast and live view of log data, eliminating manual page refreshing.
+It delivers a fast and live-view of log data, eliminating manual page refreshing.
 With an intuitive interface and live update functionality, it streamlines log file management for easier issue tracking
 and troubleshooting in Django applications.
 
 Django Log Inspector is available directly from <a href="https://pypi.org/project/django-log-inspector/">PyPI</a>:
 
 ## Installation
 
 ```
 pip install django-log-inspector
-```
+``` 
 
 Add in INSTALLED_APPS
 
 ```
 installed_apps = [
     ...
     'log_inspector',
 ]
 ```
 
 Include in the URLconf
 
 ```
-path('logs/', include('log_inspector.urls')),
+path('logs/', include('log_inspector.urls'))
 ```
 
-
 ## Settings
 
+The directory of log files in your project
+
 ```
- LOG_INSPECTOR_FILES = ['logfile1', 'logfile2', ...]
- LOG_INSPECTOR_FILES_PATTERN = '*.log*'
  LOG_INSPECTOR_FILES_DIR = 'logs/'
- LOG_INSPECTOR_PAGE_LENGTH = 25       # total log lines per-page
- LOG_INSPECTOR_MAX_READ_LINES = 1000  # total log lines will be read
- LOG_INSPECTOR_FILE_LIST_MAX_ITEMS_PER_PAGE = 25 # Max log files loaded in Datatable per page
+```
+
+A file is included if the pattern is matched, or it is specified
+
+```
+ LOG_INSPECTOR_FILES = ['logfile1', 'logfile2', ...] # default: []
+ LOG_INSPECTOR_FILES_PATTERN = '*.log*'            
+```
+
+You must specify the patterns in which your log files start with
+
+```
  LOG_INSPECTOR_PATTERNS = ['[INFO]', '[DEBUG]', '[WARNING]', '[ERROR]', '[CRITICAL]']
- LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None  # String regex expression to exclude the log from line
+```
 
- # Optionally you can set the next variables in order to customize the admin:
- LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title"
- LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css"
+How logs are displayed
+
+```
+ LOG_INSPECTOR_PAGE_LENGTH = 25             # total log lines per-page
+ LOG_INSPECTOR_MAX_READ_LINES = 1000        # total log lines that are read
+ LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None  # String regex expression to exclude the log
+```
+
+Optionally you can set the next variables in order to customize
+
+```
+LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title"               # default: None
+LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css" # default: None
+```
+
+## Login
+
+Logs are only accessible to logged-in superusers.
+If your login URL is different from Django's default, specify it in your settings.
+
+```
+LOGIN_URL = '/my-custom-admin/login/'
 ```
```

#### html2text {}

```diff
@@ -1,10 +1,12 @@
-Metadata-Version: 2.1 Name: django-log-inspector Version: 0.0.5 Summary: Read
+Metadata-Version: 2.1 Name: django-log-inspector Version: 0.0.6 Summary: Read
 and Download log files Author-email: Peyman Hassani
 gmail.com>, Shaghayegh Valadkhani
+gmail.com> Maintainer-email: Peyman Hassani
+gmail.com>, Shaghayegh Valadkhani
 gmail.com> License: MIT License Copyright (c) 2024 Peyman Hassani Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
@@ -12,29 +14,36 @@
 the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/peyzor/
-django-log-inspector Description-Content-Type: text/markdown License-File:
-LICENSE # Django Log Inspector ## _Fast and Live view to your log files_ !
-[version](https://img.shields.io/badge/version-0.0.5-blue.svg) [![Open Source]
-(https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://
-opensource.org/) _[_G_i_t_H_u_b_]Django Log Inspector offers real-time monitoring and
-analysis of log files in Django projects. It delivers a fast and live view of
-log data, eliminating manual page refreshing. With an intuitive interface and
-live update functionality, it streamlines log file management for easier issue
-tracking and troubleshooting in Django applications. Django Log Inspector is
-available directly from _P_y_P_I: ## Installation ``` pip install django-log-
-inspector ``` Add in INSTALLED_APPS ``` installed_apps = [ ... 'log_inspector',
-] ``` Include in the URLconf ``` path('logs/', include('log_inspector.urls')),
-``` ## Settings ``` LOG_INSPECTOR_FILES = ['logfile1', 'logfile2', ...]
-LOG_INSPECTOR_FILES_PATTERN = '*.log*' LOG_INSPECTOR_FILES_DIR = 'logs/
-' LOG_INSPECTOR_PAGE_LENGTH = 25 # total log lines per-page
-LOG_INSPECTOR_MAX_READ_LINES = 1000 # total log lines will be read
-LOG_INSPECTOR_FILE_LIST_MAX_ITEMS_PER_PAGE = 25 # Max log files loaded in
-Datatable per page LOG_INSPECTOR_PATTERNS = ['[INFO]', '[DEBUG]', '[WARNING]',
-'[ERROR]', '[CRITICAL]'] LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None # String
-regex expression to exclude the log from line # Optionally you can set the next
-variables in order to customize the admin: LOG_INSPECTOR_FILE_LIST_TITLE =
-"Custom title" LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css" ```
+django-log-inspector Keywords: Django,logging,log viewer,real-time
+monitoring,log analysis,troubleshooting,log management,log files,log
+monitoring,debugging,Python web development,development tool Description-
+Content-Type: text/markdown License-File: LICENSE # Django Log Inspector ##
+_Fast and Live view to your log files_ ![version](https://img.shields.io/badge/
+version-0.0.6-blue.svg) [![Open Source](https://badges.frapsoft.com/os/v1/open-
+source.svg?v=103)](https://opensource.org/) _[_G_i_t_H_u_b_]Django Log Inspector offers
+real-time monitoring and analysis of log files in Django projects. It delivers
+a fast and live-view of log data, eliminating manual page refreshing. With an
+intuitive interface and live update functionality, it streamlines log file
+management for easier issue tracking and troubleshooting in Django
+applications. Django Log Inspector is available directly from _P_y_P_I: ##
+Installation ``` pip install django-log-inspector ``` Add in INSTALLED_APPS ```
+installed_apps = [ ... 'log_inspector', ] ``` Include in the URLconf ``` path
+('logs/', include('log_inspector.urls')) ``` ## Settings The directory of log
+files in your project ``` LOG_INSPECTOR_FILES_DIR = 'logs/' ``` A file is
+included if the pattern is matched, or it is specified ``` LOG_INSPECTOR_FILES
+= ['logfile1', 'logfile2', ...] # default: [] LOG_INSPECTOR_FILES_PATTERN =
+'*.log*' ``` You must specify the patterns in which your log files start with
+``` LOG_INSPECTOR_PATTERNS = ['[INFO]', '[DEBUG]', '[WARNING]', '[ERROR]', '
+[CRITICAL]'] ``` How logs are displayed ``` LOG_INSPECTOR_PAGE_LENGTH = 25 #
+total log lines per-page LOG_INSPECTOR_MAX_READ_LINES = 1000 # total log lines
+that are read LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None # String regex
+expression to exclude the log ``` Optionally you can set the next variables in
+order to customize ``` LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title" #
+default: None LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css" #
+default: None ``` ## Login Logs are only accessible to logged-in superusers. If
+your login URL is different from Django's default, specify it in your settings.
+``` LOGIN_URL = '/my-custom-admin/login/' ```
```

### Comparing `django_log_inspector-0.0.5/django_log_inspector.egg-info/SOURCES.txt` & `django_log_inspector-0.0.6/django_log_inspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.5/log_inspector/settings.py` & `django_log_inspector-0.0.6/log_inspector/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 LOG_INSPECTOR_FILES = getattr(settings, "LOG_INSPECTOR_FILES", [])
 LOG_INSPECTOR_FILES_PATTERN = getattr(settings, "LOG_INSPECTOR_FILES_PATTERN", "*.log*")
 LOG_INSPECTOR_FILES_DIR = getattr(settings, "LOG_INSPECTOR_FILES_DIR", "logs/")
 LOG_INSPECTOR_PAGE_LENGTH = getattr(settings, "LOG_INSPECTOR_PAGE_LENGTH", 25)
 LOG_INSPECTOR_MAX_READ_LINES = getattr(settings, "LOG_INSPECTOR_MAX_READ_LINES", 1000)
 LOG_INSPECTOR_FILE_LIST_TITLE = getattr(settings, "LOG_INSPECTOR_FILE_LIST_TITLE", None)
 LOG_INSPECTOR_FILE_LIST_STYLES = getattr(settings, "LOG_INSPECTOR_FILE_LIST_STYLES", None)
-LOG_INSPECTOR_FILE_LIST_MAX_ITEMS_PER_PAGE = getattr(
-    settings, "LOG_INSPECTOR_FILE_LIST_MAX_ITEMS_PER_PAGE", 25
-)
 LOG_INSPECTOR_PATTERNS = getattr(
     settings,
     "LOG_INSPECTOR_PATTERNS",
     ["[INFO]", "[DEBUG]", "[WARNING]", "[ERROR]", "[CRITICAL]"],
 )
 LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = getattr(
     settings, "LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN", None
```

### Comparing `django_log_inspector-0.0.5/log_inspector/static/log_inspector/css/input.css` & `django_log_inspector-0.0.6/log_inspector/static/log_inspector/css/input.css`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.5/log_inspector/static/log_inspector/css/output.css` & `django_log_inspector-0.0.6/log_inspector/static/log_inspector/css/output.css`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.5/log_inspector/static/log_inspector/js/alpinejs.min.js` & `django_log_inspector-0.0.6/log_inspector/static/log_inspector/js/alpinejs.min.js`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.5/log_inspector/static/log_inspector/js/htmx.min.js` & `django_log_inspector-0.0.6/log_inspector/static/log_inspector/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.5/log_inspector/templates/log_inspector/home.html` & `django_log_inspector-0.0.6/log_inspector/templates/log_inspector/home.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.5/log_inspector/templates/log_inspector/log_entries_data.html` & `django_log_inspector-0.0.6/log_inspector/templates/log_inspector/log_entries_data.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.5/log_inspector/templates/log_inspector/log_entries_table.html` & `django_log_inspector-0.0.6/log_inspector/templates/log_inspector/log_entries_table.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.5/log_inspector/templates/log_inspector/log_files.html` & `django_log_inspector-0.0.6/log_inspector/templates/log_inspector/log_files.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.5/log_inspector/templates/log_inspector/pagination.html` & `django_log_inspector-0.0.6/log_inspector/templates/log_inspector/pagination.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.5/log_inspector/templates/log_inspector/start_live.html` & `django_log_inspector-0.0.6/log_inspector/templates/log_inspector/start_live.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.5/log_inspector/urls.py` & `django_log_inspector-0.0.6/log_inspector/urls.py`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.5/log_inspector/utils.py` & `django_log_inspector-0.0.6/log_inspector/utils.py`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.5/log_inspector/views.py` & `django_log_inspector-0.0.6/log_inspector/views.py`

 * *Files identical despite different names*


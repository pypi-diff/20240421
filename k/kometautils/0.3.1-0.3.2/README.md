# Comparing `tmp/kometautils-0.3.1.tar.gz` & `tmp/kometautils-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kometautils-0.3.1.tar", last modified: Tue Apr 16 19:43:32 2024, max compression
+gzip compressed data, was "kometautils-0.3.2.tar", last modified: Sun Apr 21 19:32:08 2024, max compression
```

## Comparing `kometautils-0.3.1.tar` & `kometautils-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:43:32.169215 kometautils-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 19:43:21.000000 kometautils-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-16 19:43:32.169215 kometautils-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-16 19:43:21.000000 kometautils-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:43:32.165215 kometautils-0.3.1/kometautils/
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-16 19:43:21.000000 kometautils-0.3.1/kometautils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-04-16 19:43:21.000000 kometautils-0.3.1/kometautils/args.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-16 19:43:21.000000 kometautils-0.3.1/kometautils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-16 19:43:21.000000 kometautils-0.3.1/kometautils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    31561 2024-04-16 19:43:21.000000 kometautils-0.3.1/kometautils/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-16 19:43:21.000000 kometautils-0.3.1/kometautils/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-16 19:43:21.000000 kometautils-0.3.1/kometautils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:43:32.169215 kometautils-0.3.1/kometautils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-16 19:43:32.000000 kometautils-0.3.1/kometautils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-16 19:43:32.000000 kometautils-0.3.1/kometautils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:43:32.000000 kometautils-0.3.1/kometautils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-16 19:43:32.000000 kometautils-0.3.1/kometautils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 19:43:32.000000 kometautils-0.3.1/kometautils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:43:32.169215 kometautils-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-16 19:43:21.000000 kometautils-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:32:08.759146 kometautils-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 19:31:58.000000 kometautils-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-21 19:32:08.759146 kometautils-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-21 19:31:58.000000 kometautils-0.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:32:08.759146 kometautils-0.3.2/kometautils/
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-21 19:31:58.000000 kometautils-0.3.2/kometautils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-04-21 19:31:58.000000 kometautils-0.3.2/kometautils/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-21 19:31:58.000000 kometautils-0.3.2/kometautils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22098 2024-04-21 19:31:58.000000 kometautils-0.3.2/kometautils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31561 2024-04-21 19:31:58.000000 kometautils-0.3.2/kometautils/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-21 19:31:58.000000 kometautils-0.3.2/kometautils/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-21 19:31:58.000000 kometautils-0.3.2/kometautils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:32:08.759146 kometautils-0.3.2/kometautils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-21 19:32:08.000000 kometautils-0.3.2/kometautils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-21 19:32:08.000000 kometautils-0.3.2/kometautils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:32:08.000000 kometautils-0.3.2/kometautils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-21 19:32:08.000000 kometautils-0.3.2/kometautils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 19:32:08.000000 kometautils-0.3.2/kometautils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:32:08.759146 kometautils-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-21 19:31:58.000000 kometautils-0.3.2/setup.py
```

### Comparing `kometautils-0.3.1/LICENSE` & `kometautils-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kometautils-0.3.1/PKG-INFO` & `kometautils-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: kometautils
-Version: 0.3.1
+Version: 0.3.2
 Summary: Util Methods for Kometa
 Home-page: https://github.com/Kometa-Team/Kometa-Utils
 Author: Nathan Taggart
-Author-email: meisnate12@gmail.com
+Author-email: kometateam@proton.me
 License: MIT License
 Project-URL: Documentation, https://github.com/Kometa-Team/Kometa-Utils
 Project-URL: Funding, https://github.com/sponsors/meisnate12
 Project-URL: Source, https://github.com/Kometa-Team/Kometa-Utils
 Project-URL: Issues, https://github.com/Kometa-Team/Kometa-Utils/issues
 Keywords: kometautils
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kometautils-0.3.1/README.rst` & `kometautils-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `kometautils-0.3.1/kometautils/__init__.py` & `kometautils-0.3.2/kometautils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 __author__ = "Nathan Taggart"
 __credits__ = "meisnate12"
 __package_name__ = "kometautils"
 __project_name__ = "Kometa-Utils"
 __description__ = "Util Methods for Kometa"
 __url__ = "https://github.com/Kometa-Team/Kometa-Utils"
-__email__ = 'meisnate12@gmail.com'
+__email__ = "kometateam@proton.me"
 __license__ = 'MIT License'
 __all__ = [
     "KometaLogger",
     "KometaArgs",
     "Version",
     "Continue",
     "Deleted",
```

### Comparing `kometautils-0.3.1/kometautils/args.py` & `kometautils-0.3.2/kometautils/args.py`

 * *Files identical despite different names*

### Comparing `kometautils-0.3.1/kometautils/logging.py` & `kometautils-0.3.2/kometautils/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,17 +85,17 @@
         self.warnings = {}
         self.errors = {}
         self.criticals = {}
         self.spacing = 0
         self.screen_width = 100
         self.separating_character = "="
         self.filename_spacing = 27
-        self.thumbnail_url = "https://github.com/meisnate12/Plex-Meta-Manager/raw/master/docs/_static/favicon.png"
+        self.thumbnail_url = "https://github.com/Kometa-Team/Kometa/raw/master/docs/_static/favicon.png"
         self.bot_name = "Metabot"
-        self.bot_image_url = "https://github.com/meisnate12/Plex-Meta-Manager/raw/master/.github/pmm.png"
+        self.bot_image_url = "https://github.com/Kometa-Team/Kometa/raw/master/.github/logo.png"
         if not self.log_file:
             self.log_file = f"{self.log_name}.log"
         self.log_path = self.log_dir / self.log_file
         self.log_path.parent.mkdir(exist_ok=True)
         self._logger = logging.getLogger(None if self.log_requests else self.log_name)
         self._logger.setLevel(logging.DEBUG)
         self.cmd_handler = logging.StreamHandler()
```

### Comparing `kometautils-0.3.1/kometautils/schedule.py` & `kometautils-0.3.2/kometautils/schedule.py`

 * *Files identical despite different names*

### Comparing `kometautils-0.3.1/kometautils/util.py` & `kometautils-0.3.2/kometautils/util.py`

 * *Files identical despite different names*

### Comparing `kometautils-0.3.1/kometautils/yaml.py` & `kometautils-0.3.2/kometautils/yaml.py`

 * *Files identical despite different names*

### Comparing `kometautils-0.3.1/kometautils.egg-info/PKG-INFO` & `kometautils-0.3.2/kometautils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: kometautils
-Version: 0.3.1
+Version: 0.3.2
 Summary: Util Methods for Kometa
 Home-page: https://github.com/Kometa-Team/Kometa-Utils
 Author: Nathan Taggart
-Author-email: meisnate12@gmail.com
+Author-email: kometateam@proton.me
 License: MIT License
 Project-URL: Documentation, https://github.com/Kometa-Team/Kometa-Utils
 Project-URL: Funding, https://github.com/sponsors/meisnate12
 Project-URL: Source, https://github.com/Kometa-Team/Kometa-Utils
 Project-URL: Issues, https://github.com/Kometa-Team/Kometa-Utils/issues
 Keywords: kometautils
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kometautils-0.3.1/setup.py` & `kometautils-0.3.2/setup.py`

 * *Files identical despite different names*


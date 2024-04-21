# Comparing `tmp/xdcheckin-2.0.7.tar.gz` & `tmp/xdcheckin-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdcheckin-2.0.7.tar", last modified: Mon Apr 15 12:30:32 2024, max compression
+gzip compressed data, was "xdcheckin-2.0.8.tar", last modified: Sun Apr 21 13:16:51 2024, max compression
```

## Comparing `xdcheckin-2.0.7.tar` & `xdcheckin-2.0.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:32.162099 xdcheckin-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-15 12:30:32.162099 xdcheckin-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 12:30:32.162099 xdcheckin-2.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:32.154099 xdcheckin-2.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:32.162099 xdcheckin-2.0.7/src/Xdcheckin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-15 12:30:32.000000 xdcheckin-2.0.7/src/Xdcheckin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 12:30:32.000000 xdcheckin-2.0.7/src/Xdcheckin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 12:30:32.000000 xdcheckin-2.0.7/src/Xdcheckin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 12:30:32.000000 xdcheckin-2.0.7/src/Xdcheckin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-15 12:30:32.000000 xdcheckin-2.0.7/src/Xdcheckin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 12:30:32.000000 xdcheckin-2.0.7/src/Xdcheckin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:32.158099 xdcheckin-2.0.7/src/xdcheckin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:32.158099 xdcheckin-2.0.7/src/xdcheckin/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33581 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/core/chaoxing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/core/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/core/xidian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:32.158099 xdcheckin-2.0.7/src/xdcheckin/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:32.162099 xdcheckin-2.0.7/src/xdcheckin/server/static/
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/server/static/activity.js
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/server/static/classroom.js
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/server/static/curriculum.js
--rw-r--r--   0 runner    (1001) docker     (127)   249304 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/server/static/g_classroom_urls.js
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/server/static/global.js
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/server/static/location.js
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/server/static/login.js
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/server/static/misc.js
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/server/static/player.js
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/server/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/server/static/util.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:32.162099 xdcheckin-2.0.7/src/xdcheckin/server/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/server/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:32.162099 xdcheckin-2.0.7/src/xdcheckin/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/util/chaoxing_captcha.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-15 12:30:26.000000 xdcheckin-2.0.7/src/xdcheckin/util/encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.119346 xdcheckin-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-21 13:16:51.119346 xdcheckin-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 13:16:51.119346 xdcheckin-2.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.111346 xdcheckin-2.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.119346 xdcheckin-2.0.8/src/Xdcheckin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-21 13:16:51.000000 xdcheckin-2.0.8/src/Xdcheckin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-21 13:16:51.000000 xdcheckin-2.0.8/src/Xdcheckin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:16:51.000000 xdcheckin-2.0.8/src/Xdcheckin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-21 13:16:51.000000 xdcheckin-2.0.8/src/Xdcheckin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-21 13:16:51.000000 xdcheckin-2.0.8/src/Xdcheckin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 13:16:51.000000 xdcheckin-2.0.8/src/Xdcheckin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.111346 xdcheckin-2.0.8/src/xdcheckin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.115346 xdcheckin-2.0.8/src/xdcheckin/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33581 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/core/chaoxing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/core/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/core/xidian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.115346 xdcheckin-2.0.8/src/xdcheckin/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.115346 xdcheckin-2.0.8/src/xdcheckin/server/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/activity.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/classroom.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/curriculum.js
+-rw-r--r--   0 runner    (1001) docker     (127)   249304 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/g_classroom_urls.js
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/global.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/location.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/login.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/misc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/player.js
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/util.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.115346 xdcheckin-2.0.8/src/xdcheckin/server/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.115346 xdcheckin-2.0.8/src/xdcheckin/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/util/chaoxing_captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/util/encryption.py
```

### Comparing `xdcheckin-2.0.7/LICENSE` & `xdcheckin-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.7/PKG-INFO` & `xdcheckin-2.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xdcheckin
-Version: 2.0.7
+Version: 2.0.8
 Summary: Chaoxing Checkin Tool for XDU.
 Author-email: Pairman <pairmanxlr@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/Xdcheckin
 Project-URL: Changelog, https://github.com/Pairman/Xdcheckin/blob/main/CHANGELOG.md
 Keywords: xdu,xidian,chaoxing,livestream
 Classifier: Framework :: Flask
@@ -68,10 +68,11 @@
 
 ### For Windows
 The APP needs [Visual C++ Redistributable Packages for Visual Studio 2013](https://www.microsoft.com/en-US/download/details.aspx?id=40784) to work on Windows. Please install [vcredist_x64.exe](https://download.microsoft.com/download/c/c/2/cc2df5f8-4454-44b4-802d-5ea68d086676/vcredist_x64.exe).
 
 ## Credits
 [w964522982/xxtSign](https://github.com/w964522982/xxtSign) <br>
 [YangRucheng/Chaoxing-AutoSign](https://github.com/YangRucheng/Chaoxing-AutoSign) <br>
+[cxOrz/chaoxing-sign-cli](https://github.com/cxOrz/chaoxing-sign-cli) <br>
 [Reclu3e/xd_learning_live_publish](https://github.com/Reclu3e/xd_learning_live_publish) <br>
 [BenderBlog/traintime_pda](https://github.com/BenderBlog/traintime_pda) <br>
 [xdlinux/libxduauth](https://github.com/xdlinux/libxduauth)
```

### Comparing `xdcheckin-2.0.7/README.md` & `xdcheckin-2.0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -42,10 +42,11 @@
 
 ### For Windows
 The APP needs [Visual C++ Redistributable Packages for Visual Studio 2013](https://www.microsoft.com/en-US/download/details.aspx?id=40784) to work on Windows. Please install [vcredist_x64.exe](https://download.microsoft.com/download/c/c/2/cc2df5f8-4454-44b4-802d-5ea68d086676/vcredist_x64.exe).
 
 ## Credits
 [w964522982/xxtSign](https://github.com/w964522982/xxtSign) <br>
 [YangRucheng/Chaoxing-AutoSign](https://github.com/YangRucheng/Chaoxing-AutoSign) <br>
+[cxOrz/chaoxing-sign-cli](https://github.com/cxOrz/chaoxing-sign-cli) <br>
 [Reclu3e/xd_learning_live_publish](https://github.com/Reclu3e/xd_learning_live_publish) <br>
 [BenderBlog/traintime_pda](https://github.com/BenderBlog/traintime_pda) <br>
 [xdlinux/libxduauth](https://github.com/xdlinux/libxduauth)
```

### Comparing `xdcheckin-2.0.7/pyproject.toml` & `xdcheckin-2.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Xdcheckin"
-version = "2.0.7"
+version = "2.0.8"
 authors = [
 	{name = "Pairman", email = "pairmanxlr@gmail.com"}
 ]
 readme = "README.md"
 description = "Chaoxing Checkin Tool for XDU."
 license = {text = "GNU General Public License v3 (GPLv3)"}
 keywords = ["xdu", "xidian", "chaoxing", "livestream"]
```

### Comparing `xdcheckin-2.0.7/src/Xdcheckin.egg-info/PKG-INFO` & `xdcheckin-2.0.8/src/Xdcheckin.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xdcheckin
-Version: 2.0.7
+Version: 2.0.8
 Summary: Chaoxing Checkin Tool for XDU.
 Author-email: Pairman <pairmanxlr@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/Xdcheckin
 Project-URL: Changelog, https://github.com/Pairman/Xdcheckin/blob/main/CHANGELOG.md
 Keywords: xdu,xidian,chaoxing,livestream
 Classifier: Framework :: Flask
@@ -68,10 +68,11 @@
 
 ### For Windows
 The APP needs [Visual C++ Redistributable Packages for Visual Studio 2013](https://www.microsoft.com/en-US/download/details.aspx?id=40784) to work on Windows. Please install [vcredist_x64.exe](https://download.microsoft.com/download/c/c/2/cc2df5f8-4454-44b4-802d-5ea68d086676/vcredist_x64.exe).
 
 ## Credits
 [w964522982/xxtSign](https://github.com/w964522982/xxtSign) <br>
 [YangRucheng/Chaoxing-AutoSign](https://github.com/YangRucheng/Chaoxing-AutoSign) <br>
+[cxOrz/chaoxing-sign-cli](https://github.com/cxOrz/chaoxing-sign-cli) <br>
 [Reclu3e/xd_learning_live_publish](https://github.com/Reclu3e/xd_learning_live_publish) <br>
 [BenderBlog/traintime_pda](https://github.com/BenderBlog/traintime_pda) <br>
 [xdlinux/libxduauth](https://github.com/xdlinux/libxduauth)
```

### Comparing `xdcheckin-2.0.7/src/Xdcheckin.egg-info/SOURCES.txt` & `xdcheckin-2.0.8/src/Xdcheckin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.7/src/xdcheckin/core/chaoxing.py` & `xdcheckin-2.0.8/src/xdcheckin/core/chaoxing.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 
 from ast import literal_eval as _literal_eval
 from datetime import datetime as _datetime
 from json import dumps as _dumps
 from random import choice as _choice, uniform as _uniform
 from re import findall as _findall, search as _search, DOTALL as _DOTALL
+from threading import Thread as _Thread
 from requests import Response as _Response
 from requests.adapters import HTTPAdapter as _HTTPAdapter
 from requests.exceptions import RequestException as _RequestException
 from requests_cache.session import CachedSession as _CachedSession
-from threading import Thread as _Thread
 from xdcheckin.util.chaoxing_captcha import generate_secrets as _generate_secrets
 from xdcheckin.util.encryption import encrypt_aes as _encrypt_aes
 
 class Chaoxing:
 	"""Common Chaoxing APIs.
 	"""
 	requests_session = name = cookies = courses = logined = None
```

### Comparing `xdcheckin-2.0.7/src/xdcheckin/core/locations.py` & `xdcheckin-2.0.8/src/xdcheckin/core/locations.py`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.7/src/xdcheckin/core/xidian.py` & `xdcheckin-2.0.8/src/xdcheckin/core/xidian.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from re import search as _search
-from requests import Response as _Response, Session as _Session
-from requests.exceptions import RequestException as _RequestException
 from threading import Thread as _Thread
 from time import time as _time
+from requests import Response as _Response, Session as _Session
+from requests.exceptions import RequestException as _RequestException
 from xdcheckin.util.encryption import encrypt_aes as _encrypt_aes
 
 class IDSSession:
 	requests_session = secrets = service = logined = None
 	config = {
 		"requests_headers": {
 			"User-Agent":
```

### Comparing `xdcheckin-2.0.7/src/xdcheckin/server/server.py` & `xdcheckin-2.0.8/src/xdcheckin/server/server.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from flask import Flask as _Flask, render_template as _render_template, \
-	make_response as _make_response, request as _request, session as _session
-from flask_session import Session as _Session
 from importlib.metadata import version as _version
 from io import BytesIO as _BytesIO
 from json import loads as _loads, dumps as _dumps
+from uuid import uuid4
+from flask import Flask as _Flask, render_template as _render_template, \
+	make_response as _make_response, request as _request, session as _session
+from flask_session import Session as _Session
 from PIL.Image import open as _open
 from pyzbar.pyzbar import decode as _decode, ZBarSymbol as _ZBarSymbol
 from requests import get as _get
-from uuid import uuid4
 from xdcheckin.core.chaoxing import Chaoxing as _Chaoxing
 from xdcheckin.core.xidian import IDSSession as _IDSSession, Newesxidian as _Newesxidian
 from xdcheckin.core.locations import locations as _locations
 
 def create_server(config: dict = {}):
 	"""Create a Xdcheckin server.
 	:param config: Server config.
```

### Comparing `xdcheckin-2.0.7/src/xdcheckin/server/static/activity.js` & `xdcheckin-2.0.8/src/xdcheckin/server/static/activity.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -113,15 +113,15 @@
     });
     let data = res.json();
     if (res.status_code != 200) {
         alert(`Checkin error. (Backend error, ${res.status_code})`);
         return;
     }
     alert(unescapeUnicode(data.msg));
-    if (data.msg.includes("'validate'"))
+    if (data.msg.includes("'validate')"))
         chaoxingCheckinCaptcha(data.params, data.captcha,
             "activities");
 }
 
 async function chaoxingCheckinLocationWrapper(activity, b_id) {
     chaoxingCheckinLocation(activity);
     onclickCooldown(b_id);
```

### Comparing `xdcheckin-2.0.7/src/xdcheckin/server/static/classroom.js` & `xdcheckin-2.0.8/src/xdcheckin/server/static/classroom.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.7/src/xdcheckin/server/static/curriculum.js` & `xdcheckin-2.0.8/src/xdcheckin/server/static/curriculum.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.7/src/xdcheckin/server/static/g_classroom_urls.js` & `xdcheckin-2.0.8/src/xdcheckin/server/static/g_classroom_urls.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.7/src/xdcheckin/server/static/location.js` & `xdcheckin-2.0.8/src/xdcheckin/server/static/location.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.7/src/xdcheckin/server/static/login.js` & `xdcheckin-2.0.8/src/xdcheckin/server/static/login.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.7/src/xdcheckin/server/static/misc.js` & `xdcheckin-2.0.8/src/xdcheckin/server/static/misc.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.7/src/xdcheckin/server/static/player.js` & `xdcheckin-2.0.8/src/xdcheckin/server/static/player.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.7/src/xdcheckin/server/static/style.css` & `xdcheckin-2.0.8/src/xdcheckin/server/static/style.css`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.7/src/xdcheckin/server/static/util.js` & `xdcheckin-2.0.8/src/xdcheckin/server/static/util.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.7/src/xdcheckin/server/templates/index.html` & `xdcheckin-2.0.8/src/xdcheckin/server/templates/index.html`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.7/src/xdcheckin/util/chaoxing_captcha.py` & `xdcheckin-2.0.8/src/xdcheckin/util/chaoxing_captcha.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 # -*- coding: utf-8 -*-
 
 from base64 import b64decode as _b64decode
 from random import random as _random
 from zlib import decompress as _decompress
-from PIL.ImageFilter import MinFilter as _MinFilter
 from pyjsbitwise import bwnot as _bwnot, bwand as _bwand, bwor as _bwor, \
 	bwxor as _bwxor, lshift as _lshift, rshift as _rshift, urshift as _urshift
 
 """Generates two blessed strings.
 For some reason I choose to obfuscate this, yet it's simple to deobfuscate.
 Clearsight awaits if you REALLY want to and got SKILLs.
 """
-exec(_decompress(_b64decode(_decompress(b"x\x9c\r\xd45\xa2\xacP\x00\x03\xd0\x05Q\x00\x83\x17\xbf\x18\xdc]\x06:\x9c\x8b\xbb\xad\xfe\xbf\x15\xa4HNJ\xf5\xd9\x07\t=q\xaavo\x14\x96G\\q\x10A_\xd2\xdf\xd6\xdd^.\xf6\x97)\xd8\xd9\x9b\xeb7\x87\xd7\xd1\xab\x1f\xd0D\x14{\xf6)2\xfbGb\xd5\xd9r\xad\xea\x9b\xc98mA\xff\xcd=G\xda(\xf8&\x06\xd7\x95HR/F\xef\x100U[\xfb\n\xd30\xf5\x8b\xf5i\x15a\xd8@\x00\xc8<9\xbfk\xe3\xc6\xa6\xde3z\"\xfd\xb8\xb0\xf2hw\x86Z\xab\x11\xb2\xc6im\xbff\x15\x85\xc8\xc6\x02*\xdc\x19l\xcd\xcb\x83\xce4\xdc\xc2\xb2\xf1\x873T!+\xf8=\x9f\xc8\x99\x15h\x07\xaeH\xba}\r?\xd3\x92\xb1\xb7Wc\xc1I\xc2\x12)\xa5pQ\x9a\x88\x15\"nZ\x07x\xdd\xe8tx->\xce\xc3m\xac6\x95\x8cX&\xed\xbf\xf7\x95\\\x05f\x9f\xd8\xe2`\xacfw,VO\xaadW7\x8c\xaa\x96\xe7\xd3F\xa8\x96\x88E\xf9\x83e\xafq5]n\xef\xf7z\xac\x1a\xd1~9\x0b\xf3z\x1b\xd7\xc3\x08K\x08\xbc\xcdNa\xfd1\xbe\xb2\xff\xa5_\x9f\xd4\x1e\x18\xb5\x83\xcc\x8d2\x80\xaf(\"(\x8dbiv\xa8\xd4\xb0G\x07\xebc\xb0a\xcej\x074\xab\xf0\x0c\x18\x99 \x1e\xc9p#\x12;\xa3\xf1\xe3W\x16\xf0L;+^[\xfeUL\x7f\xfa\x1d\xeeH\xcfb$\xdc`\xcc\xc3\x0b\xe0i\xd6 .\x9e\xd7\xdeA?\xca\x15\xdd\xde\x8e\xae\xc6[\xa5\xf7\xef\xd6\xe2v\xd6*y\xe0\xad\x91\x06\xc7\x87.\x9c\x89\xc1\x0eTG\xd5e\x0b\x0b\x08\x06\x03\'EOa\x06ff\xd2\xf6\x9c\x19\x0b4\xcc\xdfGY\xe9$o\x08]\xb5~\xbd|\xab\x8f/\xf4*\xae(^}\xaa\x06={t-\xe8\x96ez)\x8f\xd1\x06N\\!3\xf2\xb5\xb8\xe6\x99\xc3\xc8\x81\xb9\x9eO&\x17\x154\x83\xc1\xbcg\xf9\xd8*\'\x83\x06\x82\x0fz\x0c\xd5\x1f\t\x03\xf8\xa1X\xaeH^\xa1\xbc\xc2\x86I\xfa<RS\xd2\x0b:\xecH\xfcHbY\xb2\xc0Tldt]\x95[l\xd3\xefm\xe3\x86\"\x9d\x91$\x8e\'.\x8b)\x8b=Q3Y\r\xb3x\xf4$\xb0!.@\x90\x15\xbcI5\x1a\xc8\x94\xbf\\\x96\xf9\xea8]\x89\x1cy(~7\x8d\x8d-\xbcQ\xac\x96K+_\xad{\xc3`k8{\x94\xdbo\xd4\xec\x85\xd6PB\xe0\x1b\xd6\xa1Jd&\xdde\xf8\x08%U\x99\xd7@\x1e \r\x14<\xd9\x14v\xa4\x86\xe6H\x07\x0e\xcf\x07\x86\x96\x9aF\xf7\xc3\x83\x8b\xa8[\xe4\t[\t\x1c?^\x05\x08\xa0\x89xO\x88r/\x19\x12K\xb7\xa5$\x13\xcd\x8a&a\x88\xf7\x1c\x90\xdbr\x8b\x1a\x0c\x02\xf4\xe89\x04\xe5a\x011.\xbas\"\\4\x93\xd7\xb4\xcc\x1e\x95\xc5\\\xce\xff\x1c\xa0\xe4\xb5\xd0\xe3*=)\xd5\x1e\xfa\xab\xfe\x82\x18\xdb\x1b\xb1\xf7\xa2\xb2\xa4\xf8\xc5\x8e\xa0\x99\\\xd8\xabO\xd1\x01\xcfe\xe2V\x0ff\x96\x95\xe2\xba\xd3^\x18\x9bav\x00\xef}!\x91p\xcbcx\x04\xa5\xbb\x03\x8fc\xbc\'\xee\xc4A\x99\x88\x0eG\x94#2\xf3\x1d\xcd/[X\xa0X\xbda\xce\x03\xdb#\xe4\xb6\xa2\xb2\xf0s\rs\x18\xae\x81\x82\xec.\xf4\xdbZ\xcf\xa4\x13\x9c\xadh\xce/\xfd\'\x12/\xecW:\xad\xfc\xf2\xe0\xab\x0e?\xb6\x91\xf7\x05\xd3\xb4\xf9\xb4X\xe5\x0e\x96AjN\x0e\xf7qk\xa2\xb4N\xed\xbcVG\x87a\x97\xa6i\xc5\x15dv\xe9\xfc\xf5\xf6\xd9\xc00\xd5\xfc\t+J<\xa6\xaeFL\xaf<\xf8{\xe8\xd1\xcbO\xe3\xbd\xbb\x88\xaf\x1e\xedF\xf5\xae1\xbc8/\xb2\xe1o\x19o\xaf\xb2\xc5O\xf8\xf4\x92Kg8y8b\x1a\x1e\xee\x17H\x90\xcfF\x06\x97\xecR\xa9\xb8\xc2E#Y\x18\xfd\xfcD\x92s\xdb3j\x84N\x95\xf4\x9a\xd2/\x18iY\xaa\xedE\xbc\xf2f\x05\x8b\x97\x96xd\x7f\xc9u\x0eL\x8c\xa3/\xfe;\x93\xf4\xec\x88\x9e\xaeV\xaczH\x1e\x92e\x811\xa5]\xccfyz\x81mr<\x0b\x17\x1b\xb0\x1feh/\x81\xc4j\xe3S\x8d\x0e\xe8\x07\xe7}\xcc\xfe\x036\xcdoh.\xa9\x1d\xfe\xcc\xdb\x0e\x1d\x12\xf1\xd7\x1f\xc9\xc3\x13r\xc1^\x07v\xba\x9fn\x0e\xfb\xa4\x00t\xbb\xa8\x0fQ\x80HQ\x8c\xb1\xbb\xcdu\xc8\x9d\xb2<\xfaO\xd6\x18\xe26Gs\xf6\x06\'uYx\xb7$GP\xf8s\xb7\x10\xbfr\xcbd\x13\x07<\xc9$\xac\x0be\x06\x80^A@>H\xf9\xe5k\x89|u\xd1D9\xad\xbar\x16\xf4\xe8\xe04\x92\x95\xf1\xa4\xa0g\xf5i\x0c\xaed\xd0\xc3\x12_\xc7\x18W\xfeZL\xd2\x04I\xa1\xdbuR\xfdwn<\xfdIB;\xdb\x00\xc1[fd|\xdf\xde\th3\xbe\xfe\xba\xbf\xb6\r\t\x08O\"\xfdY\x88_$\xbd\x82]]\x18M\xcam |\xe9\x0f@\x9a\x083;\xcf\x87h\xb1q\x8e\x92\x0e9\x1c\x87\xa7d\xf1\x08y]\xde#\xa9-\xe2\x87\xe2\xba\x9b\x91\xb8\xb8\xc1\xc4\xc7J\xdf\xab\xe8\x8a\x83#\x97Q\xf7\xdac\x96yN\xd3\x97\x0fqO\x96aSC\x96a\xc6f\x1bd\xe7\xd2\xe5c\xaf/\x9d)\xc9Y^&D8\x86E\x9b\x10\xf6=\xbc\x13R4\xf3;\xd2\x0f^\xd9\x1b*{\xb3\xe1\xd5\xddn\x13\x80\xb5O\xc7\xa8\xdb_\xac\xcb\x16K\xfeQ\x87a\x9f\x07\xe5\xf7#\n+\xf4\xa7\x1d\xf2wy<\x90\xfaOH\xb7\xd3\xd5\xc9\xa3\x0b\x82s\xe9\x85\t|>\x9e\x0f\x8e3\xd3&\\G\x00`P,\x16\x8e\xb1\xf6\xb82J\x1af>\x16\x13z\xd3Z{\x17\xcd\xa5b\xcc\xb8\xca\xb9\xf0Uf{z\xbd\xbe\x1b\xc3\x0fWv>@\x07\x95\xc0i\xf2\x07%\t\xf60.\xe9-Y\xcb\xde\xe8\x19\xc6\x97>\xe8w\x01\xaaqJ\xdf \xe5\xcb\xdc\x90\xb7\xa4\xde\xe8/\xcf\x8ew\xd7Z9;\xbf\x12\xc2c\xcd7\xffM\x18~\x83\xac\xc5\x0b\xa6\x81\x04\x16\xc4\x07E@\x0c\xb9\xd6\xe1\x84i\xefI\x7fk\x8e\xbf\x94\x87\xf8Q\xaaM\xd7*4\xf0S\xe9.\xde\\\x1dE\x83NcRW7K\x0f\xeb\xcd\x05]\x91CmP\xbc\x9aM\x18Yx8\xc9\xdd\x9f\xd8o\xa9\xde`y\xff\"\xa5C\x97\x0f\xf8\x86\xddz\xb0v{\x92\xd1\xb7TH?\x11\xc6\x92\xa6\xf9\xb1\xba\xb4\xa7\x98\xe0K\xe8d\xf5o\xfe4\xa9\t\xacs\xf7\x02\xbfT\xac\x93\xc4\xbb\xf0\xde\'\x88\x80\xf07\xe2V|\xd3\xd6\x96\xb5Qo\x9d\xe6|,q\xb8Py\x85\x12\xde\xa6\xa6\xd7RH3\x1d\xa6\xcb^+$\xb6\xaff\xd8\xf3\x06\x9c\x14\xf4\"\x16\xdcby\x0b\xa7\xc5\x81\xddX\x96\xc3\x05B\xee\xc9\xf5<}\xb9?\xf0\xc8D\x85\xd2v\x1f\xf8\x9el\xb1B\x8a\xf6E-\x18\x94\x14k\x83\x9f\xbb\xf8\'\xb4\xbc\x1b4V\xe7\x98\x1d\x13Ya[\xf2Y\x8a\xe2\x84\x06\x00_\x8f|\x92v\xa13\x08\xc6\x8bq\xe9\x90\xa9U\xc5\xcc9\xf7\r\x108A\x934\xea\xc5\x93\xe2\x90)\x82\x91O^8\xcb\xaeb\xe4\x9aY,\xe5\xb1\xd1,\xae\x1c\xaf\xed\xec\xee\xfe;yR\xc1\x1e\xf2\x0f\x1a\xacOc\xf7&\xa5\x17g\x19\xfc=\xe7lW\x90\x7f\xff\x01\xa7<\x14C"))))
+exec(_decompress(_b64decode(_decompress(b"x\x9c\r\xd45\xa2\xacP\x00\x03\xd0\x05Q\x00\x83\x17\xbf\x18\xdc]\x06:\x9c\x8b\xbb\xad\xfe\xbf\x15\xa4HNJ\xf5\xd9\x07\t=q\xaavo\x14\x96G\\q\x10A_\xd2\xdf\xd6\xdd^.\xf6\x97)\xd8\xd9\x9b\xeb7\x87\xd7\xd1\xab\x1f\xd0D\x14{\xf6)2\xfbGb\xd5\xd9r\xad\xea\x9b\xc98mA\xff\xcd=G\xda(\xf8&\x06\xd7\x95HR/F\xef\x100U[\xfb\n\xd30\xf5\x8b\xf5i\x15a\xd8@\x00\xc8<9\xbfk\xe3\xc6\xa6\xde3z\"\xfd\xb8\xb0\xf2hw\x86Z\xab\x11\xb2\xc6im\xbff\x15\x85\xc8\xc6\x02*\xdc\x19l\xcd\xcb\x83\xce4\xdc\xc2\xb2\xf1\x873T!+\xf8=\x9f\xc8\x99\x15h\x07\xaeH\xba}\r?\xd3\x92\xb1\xb7Wc\xc1I\xc2\x12)\xa5pQ\x9a\x88\x15\"nZ\x07x\xdd\xe8tx->\xce\xc3m\xac6\x95\x8cX&\xed\xbf\xf7\x95\\\x05f\x9f\xd8\xe2`\xacfw,VO\xaadW7\x8c\xaa\x96\xe7\xd3F\xa8\x96\x88E\xf9\x83e\xafq5]n\xef\xf7z\xac\x1a\xd1~9\x0b\xf3z\x1b\xd7\xc3\x08K\x08\xbc\xcdNa\xfd1\xbe\xb2\xff\xa5_\x9f\xd4\x1e\x18\xb5\x83\xcc\x8d2\x80\xaf(\"(\x8dbiv\xa8\xd4\xb0G\x07\xebc\xb0a\xcej\x074\xab\xf0\x0c\x18\x99 \x1e\xc9p#\x12;\xa3\xf1\xe3W\x16\xf0L;+^[\xfeUL\x7f\xfa\x1d\xeeH\xcfb$\xdc`\xcc\xc3\x0b\xe0i\xd6 .\x9e\xd7\xdeA?\xca\x15\xdd\xde\x8e\xae\xc6[\xa5\xf7\xef\xd6\xe2v\xd6*y\xe0\xad\x91\x06\xc7\x87.\x9c\x89\xc1\x0eTG\xd5e\x0b\x0b\x08\x06\x03'EOa\x06ff\xd2\xf6\x9c\x19\x0b4\xcc\xdfGY\xe9$o\x08]\xb5~\xbd|\xab\x8f/\xf4*\xae(^}\xaa\x06={t-\xe8\x96ez)\x8f\xd1\x06N\\!3\xf2\xb5\xb8\xe6\x99\xc3\xc8\x81\xb9\x9eO&\x17\x154\x83\xc1\xbcg\xf9\xd8*'\x83\x06\x82\x0fz\x0c\xd5\x1f\t\x03\xf8\xa1X\xaeH^\xa1\xbc\xc2\x86I\xfa<RS\xd2\x0b:\xecH\xfcHbY\xb2\xc0Tldt]\x95[l\xd3\xefm\xe3\x86\"\x9d\x91$\x8e'.\x8b)\x8b=Q3Y\r\xb3x\xf4$\xb0!.@\x90\x15\xbcI5\x1a\xc8\x94\xbf\\\x96\xf9\xea8]\x89\x1cy(~7\x8d\x8d-\xbcQ\xac\x96K+_\xad{\xc3`k8{\x94\xdbo\xd4\xec\x85\xd6PB\xe0\x1b\xd6\xa1Jd&\xdde\xf8\x08%U\x99\xd7@\x1e \r\x14<\xd9\x14v\xa4\x86\xe6H\x07\x0e\xcf\x07\x86\x96\x9aF\xf7\xc3\x83\x8b\xa8[\xe4\t[\t\x1c?^\x05\x08\xa0\x89xO\x88r/\x19\x12K\xb7\xa5$\x13\xcd\x8a&a\x88\xf7\x1c\x90\xdbr\x8b\x1a\x0c\x02\xf4\xe89\x04\xe5a\x011.\xbas\"\\4\x93\xd7\xb4\xcc\x1e\x95\xc5\\\xce\xff\x1c\xa0\xe4\xb5\xd0\xe3*=)\xd5\x1e\xfa\xab\xfe\x82\x18\xdb\x1b\xb1\xf7\xa2\xb2\xa4\xf8\xc5\x8e\xa0\x99\\\xd8\xabO\xd1\x01\xcfe\xe2V\x0ff\x96\x95\xe2\xba\xd3^\x18\x9bav\x00\xef}!\x91p\xcbcx\x04\xa5\xbb\x03\x8fc\xbc'\xee\xc4A\x99\x88\x0eG\x94#2\xf3\x1d\xcd/[X\xa0X\xbda\xce\x03\xdb#\xe4\xb6\xa2\xb2\xf0s\rs\x18\xae\x81\x82\xec.\xf4\xdbZ\xcf\xa4\x13\x9c\xadh\xce/\xfd'\x12/\xecW:\xad\xfc\xf2\xe0\xab\x0e?\xb6\x91\xf7\x05\xd3\xb4\xf9\xb4X\xe5\x0e\x96AjN\x0e\xf7qk\xa2\xb4N\xed\xbcVG\x87a\x97\xa6i\xc5\x15dv\xe9\xfc\xf5\xf6\xd9\xc00\xd5\xfc\t+J<\xa6\xaeFL\xaf<\xf8{\xe8\xd1\xcbO\xe3\xbd\xbb\x88\xaf\x1e\xedF\xf5\xae1\xbc8/\xb2\xe1o\x19o\xaf\xb2\xc5O\xf8\xf4\x92Kg8y8b\x1a\x1e\xee\x17H\x90\xcfF\x06\x97\xecR\xa9\xb8\xc2E#Y\x18\xfd\xfcD\x92s\xdb3j\x84N\x95\xf4\x9a\xd2/\x18iY\xaa\xedE\xbc\xf2f\x05\x8b\x97\x96xd\x7f\xc9u\x0eL\x8c\xa3/\xfe;\x93\xf4\xec\x88\x9e\xaeV\xaczH\x1e\x92e\x811\xa5]\xccfyz\x81mr<\x0b\x17\x1b\xb0\x1feh/\x81\xc4j\xe3S\x8d\x0e\xe8\x07\xe7}\xcc\xfe\x036\xcdoh.\xa9\x1d\xfe\xcc\xdb\x0e\x1d\x12\xf1\xd7\x1f\xc9\xc3\x13r\xc1^\x07v\xba\x9fn\x0e\xfb\xa4\x00t\xbb\xa8\x0fQ\x80HQ\x8c\xb1\xbb\xcdu\xc8\x9d\xb2<\xfaO\xd6\x18\xe26Gs\xf6\x06'uYx\xb7$GP\xf8s\xb7\x10\xbfr\xcbd\x13\x07<\xc9$\xac\x0be\x06\x80^A@>H\xf9\xe5k\x89|u\xd1D9\xad\xbar\x16\xf4\xe8\xe04\x92\x95\xf1\xa4\xa0g\xf5i\x0c\xaed\xd0\xc3\x12_\xc7\x18W\xfeZL\xd2\x04I\xa1\xdbuR\xfdwn<\xfdIB;\xdb\x00\xc1[fd|\xdf\xde\th3\xbe\xfe\xba\xbf\xb6\r\t\x08O\"\xfdY\x88_$\xbd\x82]]\x18M\xcam |\xe9\x0f@\x9a\x083;\xcf\x87h\xb1q\x8e\x92\x0e9\x1c\x87\xa7d\xf1\x08y]\xde#\xa9-\xe2\x87\xe2\xba\x9b\x91\xb8\xb8\xc1\xc4\xc7J\xdf\xab\xe8\x8a\x83#\x97Q\xf7\xdac\x96yN\xd3\x97\x0fqO\x96aSC\x96a\xc6f\x1bd\xe7\xd2\xe5c\xaf/\x9d)\xc9Y^&D8\x86E\x9b\x10\xf6=\xbc\x13R4\xf3;\xd2\x0f^\xd9\x1b*{\xb3\xe1\xd5\xddn\x13\x80\xb5O\xc7\xa8\xdb_\xac\xcb\x16K\xfeQ\x87a\x9f\x07\xe5\xf7#\n+\xf4\xa7\x1d\xf2wy<\x90\xfaOH\xb7\xd3\xd5\xc9\xa3\x0b\x82s\xe9\x85\t|>\x9e\x0f\x8e3\xd3&\\G\x00`P,\x16\x8e\xb1\xf6\xb82J\x1af>\x16\x13z\xd3Z{\x17\xcd\xa5b\xcc\xb8\xca\xb9\xf0Uf{z\xbd\xbe\x1b\xc3\x0fWv>@\x07\x95\xc0i\xf2\x07%\t\xf60.\xe9-Y\xcb\xde\xe8\x19\xc6\x97>\xe8w\x01\xaaqJ\xdf \xe5\xcb\xdc\x90\xb7\xa4\xde\xe8/\xcf\x8ew\xd7Z9;\xbf\x12\xc2c\xcd7\xffM\x18~\x83\xac\xc5\x0b\xa6\x81\x04\x16\xc4\x07E@\x0c\xb9\xd6\xe1\x84i\xefI\x7fk\x8e\xbf\x94\x87\xf8Q\xaaM\xd7*4\xf0S\xe9.\xde\\\x1dE\x83NcRW7K\x0f\xeb\xcd\x05]\x91CmP\xbc\x9aM\x18Yx8\xc9\xdd\x9f\xd8o\xa9\xde`y\xff\"\xa5C\x97\x0f\xf8\x86\xddz\xb0v{\x92\xd1\xb7TH?\x11\xc6\x92\xa6\xf9\xb1\xba\xb4\xa7\x98\xe0K\xe8d\xf5o\xfe4\xa9\t\xacs\xf7\x02\xbfT\xac\x93\xc4\xbb\xf0\xde'\x88\x80\xf07\xe2V|\xd3\xd6\x96\xb5Qo\x9d\xe6|,q\xb8Py\x85\x12\xde\xa6\xa6\xd7RH3\x1d\xa6\xcb^+$\xb6\xaff\xd8\xf3\x06\x9c\x14\xf4\"\x16\xdcby\x0b\xa7\xc5\x81\xddX\x96\xc3\x05B\xee\xc9\xf5<}\xb9?\xf0\xc8D\x85\xd2v\x1f\xf8\x9el\xb1B\x8a\xf6E-\x18\x94\x14k\x83\x9f\xbb\xf8'\xb4\xbc\x1b4V\xe7\x98\x1d\x13Ya[\xf2Y\x8a\xe2\x84\x06\x00_\x8f|\x92v\xa13\x08\xc6\x8bq\xe9\x90\xa9U\xc5\xcc9\xf7\r\x108A\x934\xea\xc5\x93\xe2\x90)\x82\x91O^8\xcb\xaeb\xe4\x9aY,\xe5\xb1\xd1,\xae\x1c\xaf\xed\xec\xee\xfe;yR\xc1\x1e\xf2\x0f\x1a\xacOc\xf7&\xa5\x17g\x19\xfc=\xe7lW\x90\x7f\xff\x01\xa7<\x14C"))))
 
-def solve_captcha(big_img: None = None, small_img: None = None):
-	"""Slider CAPTCHA solver.
+def solve_captcha(big_img: None = None, small_img: None = None, border: int = 8):
+	"""Slider CAPTCHA solver based on normalized cross-correlation.
 	:param big_img: Background image with slider piece embedded.
 	:param small_img: Slider image vertically aligned with transparent padding.
+	:param border: Border width of the slider piece. 8 by default for Chaoxing's.
 	:return: Slider offset.
 	"""
 	with small_img.getchannel("A") as alpha:
-		with alpha.filter(_MinFilter(15)) as filter:
-			with filter.point(lambda p: p == 255 and 255 or 0) as point:
-				x_l, y_t, x_r, y_b = point.getbbox()
-	with small_img.convert("L").crop(
-		(x_l, y_t, x_r, y_b)
-	) as crop:
-		template = crop.getdata()
+		with alpha.point(lambda p: p == 255) as point:
+			x_l, y_t, x_r, y_b = point.getbbox()
+	x_l += border
+	y_t += border
+	x_r -= border
+	y_b -= border
+	with small_img.crop((x_l, y_t, x_r, y_b)) as crop:
+		with crop.convert("L") as grayscale:
+			template = grayscale.getdata()
 	mean_tmp = sum(template) / len(template)
 	template = [v - mean_tmp for v in template]
 	maxncc = 0
 	maxx = 0
-	with big_img.convert("L") as grayscale:
-		with grayscale.crop(
-			(x_l, y_t, big_img.width - small_img.width + x_r, y_b)
-		) as img:
-			for x in range(1, img.width - x_r + x_l, 2):
-				with img.crop(
-					(x, 0, x + x_r - x_l, img.height)
+	with big_img.crop(
+		(x_l + 1, y_t, big_img.width - small_img.width + x_r, y_b)
+	) as img:
+		with img.convert("L") as grayscale:
+			for x in range(0, grayscale.width - x_r + x_l, 2):
+				with grayscale.crop(
+					(x, 0, x + x_r - x_l, grayscale.height)
 				) as crop:
 					window = crop.getdata()
-				mean_wd = sum(window) / (x_r - x_l) / img.height
+				mean_wd = sum(window) / len(window)
 				window = [w - mean_wd for w in window]
 				ncc = sum(
 					w * t for w, t in zip(window, template)
-				) / sum(w ** 2 for w in window)
-				maxx = ncc > maxncc and x or maxx
-				maxncc = ncc > maxncc and ncc or maxncc
+				) / sum(w * w for w in window)
+				if ncc > maxncc:
+					maxncc = ncc
+					maxx = x
 	return maxx
```

### Comparing `xdcheckin-2.0.7/src/xdcheckin/util/encryption.py` & `xdcheckin-2.0.8/src/xdcheckin/util/encryption.py`

 * *Files identical despite different names*


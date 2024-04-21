# Comparing `tmp/renardo-1.0.0.dev0.tar.gz` & `tmp/renardo-1.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renardo-1.0.0.dev0.tar", last modified: Sun Apr 21 19:51:19 2024, max compression
+gzip compressed data, was "renardo-1.0.0.dev2.tar", last modified: Sun Apr 21 19:58:26 2024, max compression
```

## Comparing `renardo-1.0.0.dev0.tar` & `renardo-1.0.0.dev2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:19.286677 renardo-1.0.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)    12741 2024-04-21 19:51:19.286677 renardo-1.0.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:19.286677 renardo-1.0.0.dev0/renardo/
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/PulsarInstance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/RenardoApp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/RenardoTUI.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/RenardoTUI.tcss
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/SCFilesHandling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/SuperColliderInstance.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:19.286677 renardo-1.0.0.dev0/renardo/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/widgets/ConfigPane.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/widgets/TutoTabPane.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/widgets/Widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:19.286677 renardo-1.0.0.dev0/renardo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12741 2024-04-21 19:51:19.000000 renardo-1.0.0.dev0/renardo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-21 19:51:19.000000 renardo-1.0.0.dev0/renardo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:51:19.000000 renardo-1.0.0.dev0/renardo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 19:51:19.000000 renardo-1.0.0.dev0/renardo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-21 19:51:19.000000 renardo-1.0.0.dev0/renardo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 19:51:19.000000 renardo-1.0.0.dev0/renardo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:51:19.286677 renardo-1.0.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:26.312961 renardo-1.0.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)    12741 2024-04-21 19:58:26.312961 renardo-1.0.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-04-21 19:58:18.000000 renardo-1.0.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:26.308961 renardo-1.0.0.dev2/renardo/
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-21 19:58:18.000000 renardo-1.0.0.dev2/renardo/PulsarInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-21 19:58:18.000000 renardo-1.0.0.dev2/renardo/RenardoApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-04-21 19:58:18.000000 renardo-1.0.0.dev2/renardo/RenardoTUI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-21 19:58:18.000000 renardo-1.0.0.dev2/renardo/RenardoTUI.tcss
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-21 19:58:18.000000 renardo-1.0.0.dev2/renardo/SCFilesHandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-21 19:58:18.000000 renardo-1.0.0.dev2/renardo/SuperColliderInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-21 19:58:18.000000 renardo-1.0.0.dev2/renardo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-21 19:58:18.000000 renardo-1.0.0.dev2/renardo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:26.312961 renardo-1.0.0.dev2/renardo/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-21 19:58:18.000000 renardo-1.0.0.dev2/renardo/widgets/ConfigPane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-21 19:58:18.000000 renardo-1.0.0.dev2/renardo/widgets/TutoTabPane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-21 19:58:18.000000 renardo-1.0.0.dev2/renardo/widgets/Widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:18.000000 renardo-1.0.0.dev2/renardo/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:26.312961 renardo-1.0.0.dev2/renardo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12741 2024-04-21 19:58:26.000000 renardo-1.0.0.dev2/renardo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-21 19:58:26.000000 renardo-1.0.0.dev2/renardo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:58:26.000000 renardo-1.0.0.dev2/renardo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 19:58:26.000000 renardo-1.0.0.dev2/renardo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-21 19:58:26.000000 renardo-1.0.0.dev2/renardo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 19:58:26.000000 renardo-1.0.0.dev2/renardo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:58:26.312961 renardo-1.0.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-21 19:58:18.000000 renardo-1.0.0.dev2/setup.py
```

### Comparing `renardo-1.0.0.dev0/PKG-INFO` & `renardo-1.0.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: renardo
-Version: 1.0.0.dev0
+Version: 1.0.0.dev2
 Summary: Launcher/config editor for Renardo livecoding environment
 Home-page: http://renardo.org/
 Author: Elie Gavoty
 Author-email: eliegavoty@free.fr
 License: cc-by-sa-4.0
 Description-Content-Type: text/markdown
-Requires-Dist: renardo-lib==1.0.0.dev0
-Requires-Dist: FoxDotEditor==1.0.0.dev0
+Requires-Dist: renardo-lib==1.0.0.dev2
+Requires-Dist: FoxDotEditor==1.0.0.dev2
 Requires-Dist: renardo_gatherer==0.1.3
 Requires-Dist: psutil
 Requires-Dist: textual
 
 Renardo v0.9 - FoxDot fork
 ===========================
```

### Comparing `renardo-1.0.0.dev0/README.md` & `renardo-1.0.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `renardo-1.0.0.dev0/renardo/PulsarInstance.py` & `renardo-1.0.0.dev2/renardo/PulsarInstance.py`

 * *Files identical despite different names*

### Comparing `renardo-1.0.0.dev0/renardo/RenardoApp.py` & `renardo-1.0.0.dev2/renardo/RenardoApp.py`

 * *Files identical despite different names*

### Comparing `renardo-1.0.0.dev0/renardo/RenardoTUI.py` & `renardo-1.0.0.dev2/renardo/RenardoTUI.py`

 * *Files identical despite different names*

### Comparing `renardo-1.0.0.dev0/renardo/SCFilesHandling.py` & `renardo-1.0.0.dev2/renardo/SCFilesHandling.py`

 * *Files identical despite different names*

### Comparing `renardo-1.0.0.dev0/renardo/SuperColliderInstance.py` & `renardo-1.0.0.dev2/renardo/SuperColliderInstance.py`

 * *Files identical despite different names*

### Comparing `renardo-1.0.0.dev0/renardo/widgets/ConfigPane.py` & `renardo-1.0.0.dev2/renardo/widgets/ConfigPane.py`

 * *Files identical despite different names*

### Comparing `renardo-1.0.0.dev0/renardo/widgets/TutoTabPane.py` & `renardo-1.0.0.dev2/renardo/widgets/TutoTabPane.py`

 * *Files identical despite different names*

### Comparing `renardo-1.0.0.dev0/renardo/widgets/Widgets.py` & `renardo-1.0.0.dev2/renardo/widgets/Widgets.py`

 * *Files identical despite different names*

### Comparing `renardo-1.0.0.dev0/renardo.egg-info/PKG-INFO` & `renardo-1.0.0.dev2/renardo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: renardo
-Version: 1.0.0.dev0
+Version: 1.0.0.dev2
 Summary: Launcher/config editor for Renardo livecoding environment
 Home-page: http://renardo.org/
 Author: Elie Gavoty
 Author-email: eliegavoty@free.fr
 License: cc-by-sa-4.0
 Description-Content-Type: text/markdown
-Requires-Dist: renardo-lib==1.0.0.dev0
-Requires-Dist: FoxDotEditor==1.0.0.dev0
+Requires-Dist: renardo-lib==1.0.0.dev2
+Requires-Dist: FoxDotEditor==1.0.0.dev2
 Requires-Dist: renardo_gatherer==0.1.3
 Requires-Dist: psutil
 Requires-Dist: textual
 
 Renardo v0.9 - FoxDot fork
 ===========================
```

### Comparing `renardo-1.0.0.dev0/renardo.egg-info/SOURCES.txt` & `renardo-1.0.0.dev2/renardo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `renardo-1.0.0.dev0/setup.py` & `renardo-1.0.0.dev2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description=f.read()
 
 setup(
     name='renardo',
-    version="1.0.0.dev0",
+    version="1.0.0.dev2",
     description='Launcher/config editor for Renardo livecoding environment',
     author='Elie Gavoty',
     author_email='eliegavoty@free.fr',
     license='cc-by-sa-4.0',
     url='http://renardo.org/',
     packages=[
         'renardo',
@@ -19,16 +19,16 @@
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     # entry_points={'gui_scripts' : ['FoxDotEditor = FoxDotEditor.__init__:main']},
     # data_files=[('', 'LICENSE')],
     package_data = {'renardo': ['RenardoTUI.tcss'],},
     install_requires=[
-        'renardo-lib==1.0.0.dev0',
-        'FoxDotEditor==1.0.0.dev0',
+        'renardo-lib==1.0.0.dev2',
+        'FoxDotEditor==1.0.0.dev2',
         'renardo_gatherer==0.1.3',
         'psutil',
         'textual',
     ],
     entry_points={
         'console_scripts': [
             'renardo = renardo:entrypoint',
```


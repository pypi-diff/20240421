# Comparing `tmp/foxdoteditor-1.0.0.dev0.tar.gz` & `tmp/foxdoteditor-1.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxdoteditor-1.0.0.dev0.tar", last modified: Sun Apr 21 19:51:24 2024, max compression
+gzip compressed data, was "foxdoteditor-1.0.0.dev2.tar", last modified: Sun Apr 21 19:58:21 2024, max compression
```

## Comparing `foxdoteditor-1.0.0.dev0.tar` & `foxdoteditor-1.0.0.dev2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:24.791882 foxdoteditor-1.0.0.dev0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:24.791882 foxdoteditor-1.0.0.dev0/FoxDotEditor/
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/AppFunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/BracketHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/ConfigFile.py
--rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/Console.py
--rw-r--r--   0 runner    (1001) docker     (127)    50923 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/Editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/Format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/LineNumbers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/MenuBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/Prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/SampleChart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:24.791882 foxdoteditor-1.0.0.dev0/FoxDotEditor/Settings/
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/Settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/Settings/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/TextBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:24.791882 foxdoteditor-1.0.0.dev0/FoxDotEditor/img/
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/img/foxdot.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/img/icon.gif
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/img/icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/tkimport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:24.791882 foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-04-21 19:51:24.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-21 19:51:24.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:51:24.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-21 19:51:24.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-21 19:51:24.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 19:51:24.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-04-21 19:51:24.791882 foxdoteditor-1.0.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:51:24.791882 foxdoteditor-1.0.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:21.325597 foxdoteditor-1.0.0.dev2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:21.321597 foxdoteditor-1.0.0.dev2/FoxDotEditor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/AppFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/BracketHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/ConfigFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/Console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50923 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/Editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/Format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/LineNumbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/MenuBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/Prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/SampleChart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:21.321597 foxdoteditor-1.0.0.dev2/FoxDotEditor/Settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/Settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/Settings/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/TextBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:21.321597 foxdoteditor-1.0.0.dev2/FoxDotEditor/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/img/foxdot.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/img/icon.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/img/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor/tkimport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:21.321597 foxdoteditor-1.0.0.dev2/FoxDotEditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-04-21 19:58:21.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-21 19:58:21.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:58:21.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-21 19:58:21.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-21 19:58:21.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 19:58:21.000000 foxdoteditor-1.0.0.dev2/FoxDotEditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-04-21 19:58:21.325597 foxdoteditor-1.0.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:58:21.325597 foxdoteditor-1.0.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-21 19:58:17.000000 foxdoteditor-1.0.0.dev2/setup.py
```

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/AppFunctions.py` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/AppFunctions.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/BracketHandler.py` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/BracketHandler.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/ConfigFile.py` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/ConfigFile.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/Console.py` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/Console.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/Editor.py` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/Editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     def __init__(self, CodeClass):
 
         # Configure Renardo's namespace to include the editor
 
         CodeClass.namespace['GUI'] = self
         CodeClass.namespace['Player'].widget = self
 
-        self.version = this_version = '1.0.0.dev0' 
+        self.version = this_version = '1.0.0.dev2' 
 
         pypi_version = get_pypi_version()
 
         def check_versions():
 
             # if pypi_version is not None and VersionNumber(pypi_version) > VersionNumber(this_version):
```

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/Format.py` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/Format.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/LineNumbers.py` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/LineNumbers.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/MenuBar.py` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/MenuBar.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/Prompt.py` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/Prompt.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/SampleChart.py` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/SampleChart.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/Settings/__init__.py` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/Settings/__init__.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/Settings/conf.py` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/Settings/conf.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/TextBox.py` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/TextBox.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/__init__.py` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/__init__.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/__main__.py` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/__main__.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/img/foxdot.ico` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/img/foxdot.ico`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/img/icon.gif` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/img/icon.gif`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor/img/icon.ico` & `foxdoteditor-1.0.0.dev2/FoxDotEditor/img/icon.ico`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/PKG-INFO` & `foxdoteditor-1.0.0.dev2/FoxDotEditor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: FoxDotEditor
-Version: 1.0.0.dev0
+Version: 1.0.0.dev2
 Summary: Original FoxDot editor extracted from FoxDot Project - Live coding music with SuperCollider
 Home-page: http://foxdot.org/
 Author: Elie Gavoty
 Author-email: eliegavoty@free.fr
 License: cc-by-sa-4.0
 Description-Content-Type: text/markdown
-Requires-Dist: renardo-lib==1.0.0.dev0
+Requires-Dist: renardo-lib==1.0.0.dev2
 Requires-Dist: psutil
 
 FoxDot - Editor
 =====================================
 
 Original FoxDot editor extract from original project for use with separated FoxDot library or renardo fork.
```

### Comparing `foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/SOURCES.txt` & `foxdoteditor-1.0.0.dev2/FoxDotEditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/PKG-INFO` & `foxdoteditor-1.0.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: FoxDotEditor
-Version: 1.0.0.dev0
+Version: 1.0.0.dev2
 Summary: Original FoxDot editor extracted from FoxDot Project - Live coding music with SuperCollider
 Home-page: http://foxdot.org/
 Author: Elie Gavoty
 Author-email: eliegavoty@free.fr
 License: cc-by-sa-4.0
 Description-Content-Type: text/markdown
-Requires-Dist: renardo-lib==1.0.0.dev0
+Requires-Dist: renardo-lib==1.0.0.dev2
 Requires-Dist: psutil
 
 FoxDot - Editor
 =====================================
 
 Original FoxDot editor extract from original project for use with separated FoxDot library or renardo fork.
```

### Comparing `foxdoteditor-1.0.0.dev0/README.md` & `foxdoteditor-1.0.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `foxdoteditor-1.0.0.dev0/setup.py` & `foxdoteditor-1.0.0.dev2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description=f.read()
 
 setup(
     name='FoxDotEditor',
-    version="1.0.0.dev0",
+    version="1.0.0.dev2",
     description='Original FoxDot editor extracted from FoxDot Project - Live coding music with SuperCollider',
     author='Elie Gavoty',
     author_email='eliegavoty@free.fr',
     license='cc-by-sa-4.0',
     url='http://foxdot.org/',
     packages=['FoxDotEditor', 'FoxDotEditor.Settings'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={'gui_scripts' : ['FoxDotEditor = FoxDotEditor.__init__:main']},
     # data_files=[('', 'LICENSE')],
     package_data = {'FoxDotEditor': ['README.md','img/*','tmp/*'],},
     install_requires=[
-        'renardo-lib==1.0.0.dev0',
+        'renardo-lib==1.0.0.dev2',
         'psutil',
     ],
 )
```


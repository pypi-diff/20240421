# Comparing `tmp/foxdoteditor-0.9.9.tar.gz` & `tmp/foxdoteditor-1.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxdoteditor-0.9.9.tar", last modified: Sat Apr 20 17:39:00 2024, max compression
+gzip compressed data, was "foxdoteditor-1.0.0.dev0.tar", last modified: Sun Apr 21 19:51:24 2024, max compression
```

## Comparing `foxdoteditor-0.9.9.tar` & `foxdoteditor-1.0.0.dev0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:39:00.666886 foxdoteditor-0.9.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:39:00.662886 foxdoteditor-0.9.9/FoxDotEditor/
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/AppFunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/BracketHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/ConfigFile.py
--rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/Console.py
--rw-r--r--   0 runner    (1001) docker     (127)    50918 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/Editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/Format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/LineNumbers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/MenuBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/Prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)    15759 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/SampleChart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:39:00.666886 foxdoteditor-0.9.9/FoxDotEditor/Settings/
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/Settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/Settings/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/TextBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:39:00.666886 foxdoteditor-0.9.9/FoxDotEditor/img/
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/img/foxdot.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/img/icon.gif
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/img/icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/tkimport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:39:00.666886 foxdoteditor-0.9.9/FoxDotEditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-20 17:39:00.000000 foxdoteditor-0.9.9/FoxDotEditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-20 17:39:00.000000 foxdoteditor-0.9.9/FoxDotEditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 17:39:00.000000 foxdoteditor-0.9.9/FoxDotEditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-20 17:39:00.000000 foxdoteditor-0.9.9/FoxDotEditor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-20 17:39:00.000000 foxdoteditor-0.9.9/FoxDotEditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-20 17:39:00.000000 foxdoteditor-0.9.9/FoxDotEditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-20 17:39:00.666886 foxdoteditor-0.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 17:39:00.666886 foxdoteditor-0.9.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:24.791882 foxdoteditor-1.0.0.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:24.791882 foxdoteditor-1.0.0.dev0/FoxDotEditor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/AppFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/BracketHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/ConfigFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/Console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50923 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/Editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/Format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/LineNumbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/MenuBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/Prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/SampleChart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:24.791882 foxdoteditor-1.0.0.dev0/FoxDotEditor/Settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/Settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/Settings/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/TextBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:24.791882 foxdoteditor-1.0.0.dev0/FoxDotEditor/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/img/foxdot.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/img/icon.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/img/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor/tkimport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:24.791882 foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-04-21 19:51:24.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-21 19:51:24.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:51:24.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-21 19:51:24.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-21 19:51:24.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 19:51:24.000000 foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-04-21 19:51:24.791882 foxdoteditor-1.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:51:24.791882 foxdoteditor-1.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-21 19:51:20.000000 foxdoteditor-1.0.0.dev0/setup.py
```

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/AppFunctions.py` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/AppFunctions.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/BracketHandler.py` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/BracketHandler.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/ConfigFile.py` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/ConfigFile.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/Console.py` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/Console.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/Editor.py` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/Editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     def __init__(self, CodeClass):
 
         # Configure Renardo's namespace to include the editor
 
         CodeClass.namespace['GUI'] = self
         CodeClass.namespace['Player'].widget = self
 
-        self.version = this_version = '0.9.3' 
+        self.version = this_version = '1.0.0.dev0' 
 
         pypi_version = get_pypi_version()
 
         def check_versions():
 
             # if pypi_version is not None and VersionNumber(pypi_version) > VersionNumber(this_version):
```

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/Format.py` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/Format.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/LineNumbers.py` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/LineNumbers.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/MenuBar.py` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/MenuBar.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/Prompt.py` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/Prompt.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/SampleChart.py` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/SampleChart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 #!/usr/bin/env python
 from __future__ import absolute_import
 
 import multiprocessing
-from playsound import playsound
 from .tkimport import *
 from .Format import *
 from renardo_lib.Settings import *
 from renardo_lib import spack_manager
 from renardo_gatherer.samples_download import nonalpha
 from renardo_gatherer import SAMPLES_DIR_PATH
 
+try:
+    from playsound import playsound
+except:
+    print("playsound library not installed...")
+
 class SampleChart:
 
     def __init__(self):
         # Basic TKinter function
         self.root = Tk()
 
         self.width = 800
@@ -278,15 +282,18 @@
             self.cmd = "loop"
             self.char = os.path.splitext(path)[0]
         else:
             self.char = list(nonalpha.keys())[list(
                 nonalpha.values()).index(self.char)]
             self.path = self.db_path_s + char + "/" + path
             self.cmd = "play"
-        self.p = multiprocessing.Process(target=playsound, args=(self.path,))
+        try:
+            self.p = multiprocessing.Process(target=playsound, args=(self.path,))
+        except:
+            print("playsound library not installed...")
         self.code = f'{self.cmd}("{self.char}", spack={self.spack_num_str}, sample={sample})'
         self.txt.insert(END, self.code)
         self.change_fname(path)
         self.p.start()
         self.processes.append(self.p)
 
     def press_space(self, event):
```

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/Settings/__init__.py` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/Settings/__init__.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/Settings/conf.py` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/Settings/conf.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/TextBox.py` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/TextBox.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/__init__.py` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/__init__.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/__main__.py` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/__main__.py`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/img/foxdot.ico` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/img/foxdot.ico`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/img/icon.gif` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/img/icon.gif`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/FoxDotEditor/img/icon.ico` & `foxdoteditor-1.0.0.dev0/FoxDotEditor/img/icon.ico`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/FoxDotEditor.egg-info/PKG-INFO` & `foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: FoxDotEditor
-Version: 0.9.9
+Version: 1.0.0.dev0
 Summary: Original FoxDot editor extracted from FoxDot Project - Live coding music with SuperCollider
 Home-page: http://foxdot.org/
 Author: Elie Gavoty
 Author-email: eliegavoty@free.fr
 License: cc-by-sa-4.0
 Description-Content-Type: text/markdown
-Requires-Dist: renardo-lib==0.9.9
+Requires-Dist: renardo-lib==1.0.0.dev0
 Requires-Dist: psutil
-Requires-Dist: playsound
 
 FoxDot - Editor
 =====================================
 
 Original FoxDot editor extract from original project for use with separated FoxDot library or renardo fork.
 
 #### Startup
```

### Comparing `foxdoteditor-0.9.9/FoxDotEditor.egg-info/SOURCES.txt` & `foxdoteditor-1.0.0.dev0/FoxDotEditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/PKG-INFO` & `foxdoteditor-1.0.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: FoxDotEditor
-Version: 0.9.9
+Version: 1.0.0.dev0
 Summary: Original FoxDot editor extracted from FoxDot Project - Live coding music with SuperCollider
 Home-page: http://foxdot.org/
 Author: Elie Gavoty
 Author-email: eliegavoty@free.fr
 License: cc-by-sa-4.0
 Description-Content-Type: text/markdown
-Requires-Dist: renardo-lib==0.9.9
+Requires-Dist: renardo-lib==1.0.0.dev0
 Requires-Dist: psutil
-Requires-Dist: playsound
 
 FoxDot - Editor
 =====================================
 
 Original FoxDot editor extract from original project for use with separated FoxDot library or renardo fork.
 
 #### Startup
```

### Comparing `foxdoteditor-0.9.9/README.md` & `foxdoteditor-1.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `foxdoteditor-0.9.9/setup.py` & `foxdoteditor-1.0.0.dev0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description=f.read()
 
 setup(
     name='FoxDotEditor',
-    version="0.9.9",
+    version="1.0.0.dev0",
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
-        'renardo-lib==0.9.9',
+        'renardo-lib==1.0.0.dev0',
         'psutil',
-        'playsound',
     ],
 )
```


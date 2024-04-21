# Comparing `tmp/cerbogen-0.0.47.tar.gz` & `tmp/cerbogen-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.47.tar", last modified: Sun Apr 21 05:10:01 2024, max compression
+gzip compressed data, was "cerbogen-0.0.48.tar", last modified: Sun Apr 21 06:45:53 2024, max compression
```

## Comparing `cerbogen-0.0.47.tar` & `cerbogen-0.0.48.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 05:10:01.321954 cerbogen-0.0.47/
--rw-rw-rw-   0        0        0      680 2024-04-21 05:10:01.321954 cerbogen-0.0.47/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.47/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 05:10:01.296023 cerbogen-0.0.47/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.47/cerbogen/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 05:10:01.289043 cerbogen-0.0.47/cerbogen/data/
-drwxrwxrwx   0        0        0        0 2024-04-21 05:10:01.307990 cerbogen-0.0.47/cerbogen/data/img/
--rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.47/cerbogen/data/img/logo.ico
--rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.47/cerbogen/data/img/logo.png
-drwxrwxrwx   0        0        0        0 2024-04-21 05:10:01.317964 cerbogen-0.0.47/cerbogen/install/
--rw-rw-rw-   0        0        0        0 2024-04-20 16:57:31.000000 cerbogen-0.0.47/cerbogen/install/__init__.py
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.47/cerbogen/install/check.py
--rw-rw-rw-   0        0        0      596 2024-04-21 05:08:13.000000 cerbogen-0.0.47/cerbogen/install/install.py
--rw-rw-rw-   0        0        0     2930 2024-04-20 16:38:30.000000 cerbogen-0.0.47/cerbogen/install/install_ffmpeg.py
--rw-rw-rw-   0        0        0     2212 2024-04-21 05:09:06.000000 cerbogen-0.0.47/cerbogen/install/install_location.py
--rw-rw-rw-   0        0        0    11588 2024-04-21 05:00:38.000000 cerbogen-0.0.47/cerbogen/main.py
-drwxrwxrwx   0        0        0        0 2024-04-21 05:10:01.319958 cerbogen-0.0.47/cerbogen/mod/
--rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.47/cerbogen/mod/__init__.py
--rw-rw-rw-   0        0        0     9057 2024-04-21 04:45:42.000000 cerbogen-0.0.47/cerbogen/mod/cerbogen.py
--rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.47/cerbogen/mod/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-21 05:10:01.320956 cerbogen-0.0.47/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      680 2024-04-21 05:10:01.000000 cerbogen-0.0.47/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      495 2024-04-21 05:10:01.000000 cerbogen-0.0.47/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 05:10:01.000000 cerbogen-0.0.47/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-21 05:10:01.000000 cerbogen-0.0.47/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-21 05:10:01.000000 cerbogen-0.0.47/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 05:10:01.322951 cerbogen-0.0.47/setup.cfg
--rw-rw-rw-   0        0        0     1491 2024-04-21 05:07:15.000000 cerbogen-0.0.47/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:45:53.678162 cerbogen-0.0.48/
+-rw-rw-rw-   0        0        0      680 2024-04-21 06:45:53.677165 cerbogen-0.0.48/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.48/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 06:45:53.656709 cerbogen-0.0.48/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-21 05:43:23.000000 cerbogen-0.0.48/cerbogen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:45:53.653716 cerbogen-0.0.48/cerbogen/data/
+drwxrwxrwx   0        0        0        0 2024-04-21 06:45:53.667679 cerbogen-0.0.48/cerbogen/data/img/
+-rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.48/cerbogen/data/img/logo.ico
+-rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.48/cerbogen/data/img/logo.png
+drwxrwxrwx   0        0        0        0 2024-04-21 06:45:53.672666 cerbogen-0.0.48/cerbogen/install/
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.48/cerbogen/install/check.py
+-rw-rw-rw-   0        0        0      594 2024-04-21 05:43:25.000000 cerbogen-0.0.48/cerbogen/install/install.py
+-rw-rw-rw-   0        0        0     2930 2024-04-20 16:38:30.000000 cerbogen-0.0.48/cerbogen/install/install_ffmpeg.py
+-rw-rw-rw-   0        0        0     2212 2024-04-21 05:38:09.000000 cerbogen-0.0.48/cerbogen/install/install_location.py
+-rw-rw-rw-   0        0        0       35 2024-04-21 06:40:08.000000 cerbogen-0.0.48/cerbogen/install/try.py
+-rw-rw-rw-   0        0        0    11588 2024-04-21 05:44:23.000000 cerbogen-0.0.48/cerbogen/main.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:45:53.675658 cerbogen-0.0.48/cerbogen/mod/
+-rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.48/cerbogen/mod/__init__.py
+-rw-rw-rw-   0        0        0     9057 2024-04-21 04:45:42.000000 cerbogen-0.0.48/cerbogen/mod/cerbogen.py
+-rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.48/cerbogen/mod/plot.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:45:53.676172 cerbogen-0.0.48/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      680 2024-04-21 06:45:53.000000 cerbogen-0.0.48/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2024-04-21 06:45:53.000000 cerbogen-0.0.48/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 06:45:53.000000 cerbogen-0.0.48/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-21 06:45:53.000000 cerbogen-0.0.48/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-21 06:45:53.000000 cerbogen-0.0.48/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 06:45:53.678162 cerbogen-0.0.48/setup.cfg
+-rw-rw-rw-   0        0        0     1593 2024-04-21 06:45:53.000000 cerbogen-0.0.48/setup.py
```

### Comparing `cerbogen-0.0.47/PKG-INFO` & `cerbogen-0.0.48/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.47
+Version: 0.0.48
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.47/cerbogen/data/img/logo.ico` & `cerbogen-0.0.48/cerbogen/data/img/logo.ico`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.47/cerbogen/data/img/logo.png` & `cerbogen-0.0.48/cerbogen/data/img/logo.png`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.47/cerbogen/install/check.py` & `cerbogen-0.0.48/cerbogen/install/check.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.47/cerbogen/install/install.py` & `cerbogen-0.0.48/cerbogen/install/install.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import sys
 import platform
 
-
 # import cerbogen.install.install_ffmpeg
 import cerbogen.install.install_location
 
 
 def install_pywin32():
     if platform.system() == "Windows":
         try:
```

### Comparing `cerbogen-0.0.47/cerbogen/install/install_ffmpeg.py` & `cerbogen-0.0.48/cerbogen/install/install_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.47/cerbogen/install/install_location.py` & `cerbogen-0.0.48/cerbogen/install/install_location.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.47/cerbogen/main.py` & `cerbogen-0.0.48/cerbogen/main.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.47/cerbogen/mod/cerbogen.py` & `cerbogen-0.0.48/cerbogen/mod/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.47/cerbogen/mod/plot.py` & `cerbogen-0.0.48/cerbogen/mod/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.47/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.48/cerbogen.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.47
+Version: 0.0.48
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.47/setup.py` & `cerbogen-0.0.48/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 import subprocess
 import shutil
 import os
 
-class CustomInstall(install):
+class cerbogen(install):
+
     def run(self):
         install.run(self)
         self.custom_code()
     
     def custom_code(self):
         # Run the install.py script located in the 'install' directory
-        install_script_path = os.path.join(os.path.dirname(__file__), 'cerbogen', 'install', 'install.py')
+        install_script_path = os.path.join(os.path.dirname(__file__), 'install', 'try.py')
         subprocess.run(['python', install_script_path])
-        
+
+# Read the contents of README.md for the long description
+with open('README.md', 'r') as f:
+    long_description = f.read()
 
 setup(
     name='cerbogen',
-    version='0.0.47',
+    version = '0.0.48',
     description='A Python package for CerboTech',
-    long_description=open('README.md').read(),
+    long_description=long_description,
     long_description_content_type='text/markdown',
     author='Clarence Parmar',
     author_email='git.clarence@gmail.com',
     url='https://github.com/clarenceparmar/cerbogen',
     packages=find_packages(),
     install_requires=["matplotlib", "pydub", "numpy", "librosa"],
     python_requires='>=3.6',
@@ -33,12 +37,12 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
 
     # Include all files from the 'data' directory
-    package_data={'': ['data/*/*']},
+    package_data={'': ['data/*/*', 'install/*']},
 
     # Use the custom install class
-    cmdclass={'install': CustomInstall},
+    cmdclass={'install': cerbogen},
 )
```


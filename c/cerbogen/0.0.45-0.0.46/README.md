# Comparing `tmp/cerbogen-0.0.45.tar.gz` & `tmp/cerbogen-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.45.tar", last modified: Sun Apr 21 03:59:48 2024, max compression
+gzip compressed data, was "cerbogen-0.0.46.tar", last modified: Sun Apr 21 04:01:32 2024, max compression
```

## Comparing `cerbogen-0.0.45.tar` & `cerbogen-0.0.46.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 03:59:48.505098 cerbogen-0.0.45/
--rw-rw-rw-   0        0        0      680 2024-04-21 03:59:48.505098 cerbogen-0.0.45/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.45/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 03:59:48.488143 cerbogen-0.0.45/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.45/cerbogen/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 03:59:48.501109 cerbogen-0.0.45/cerbogen/install/
--rw-rw-rw-   0        0        0        0 2024-04-20 16:57:31.000000 cerbogen-0.0.45/cerbogen/install/__init__.py
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.45/cerbogen/install/check.py
--rw-rw-rw-   0        0        0     2930 2024-04-20 16:38:30.000000 cerbogen-0.0.45/cerbogen/install/install_ffmpeg.py
--rw-rw-rw-   0        0        0     2450 2024-04-21 03:44:12.000000 cerbogen-0.0.45/cerbogen/install/install_location.py
--rw-rw-rw-   0        0        0      613 2024-04-21 03:58:58.000000 cerbogen-0.0.45/cerbogen/install/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 03:59:48.503103 cerbogen-0.0.45/cerbogen/mod/
--rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.45/cerbogen/mod/__init__.py
--rw-rw-rw-   0        0        0     9097 2024-04-21 03:48:48.000000 cerbogen-0.0.45/cerbogen/mod/cerbogen.py
--rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.45/cerbogen/mod/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-21 03:59:48.504101 cerbogen-0.0.45/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      680 2024-04-21 03:59:48.000000 cerbogen-0.0.45/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2024-04-21 03:59:48.000000 cerbogen-0.0.45/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 03:59:48.000000 cerbogen-0.0.45/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-21 03:59:48.000000 cerbogen-0.0.45/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-21 03:59:48.000000 cerbogen-0.0.45/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 03:59:48.505098 cerbogen-0.0.45/setup.cfg
--rw-rw-rw-   0        0        0     1287 2024-04-21 03:59:47.000000 cerbogen-0.0.45/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 04:01:32.534596 cerbogen-0.0.46/
+-rw-rw-rw-   0        0        0      680 2024-04-21 04:01:32.533598 cerbogen-0.0.46/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.46/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 04:01:32.511656 cerbogen-0.0.46/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.46/cerbogen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 04:01:32.529608 cerbogen-0.0.46/cerbogen/install/
+-rw-rw-rw-   0        0        0        0 2024-04-20 16:57:31.000000 cerbogen-0.0.46/cerbogen/install/__init__.py
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.46/cerbogen/install/check.py
+-rw-rw-rw-   0        0        0     2930 2024-04-20 16:38:30.000000 cerbogen-0.0.46/cerbogen/install/install_ffmpeg.py
+-rw-rw-rw-   0        0        0     2450 2024-04-21 03:44:12.000000 cerbogen-0.0.46/cerbogen/install/install_location.py
+-rw-rw-rw-   0        0        0      618 2024-04-21 04:01:16.000000 cerbogen-0.0.46/cerbogen/install/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 04:01:32.531603 cerbogen-0.0.46/cerbogen/mod/
+-rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.46/cerbogen/mod/__init__.py
+-rw-rw-rw-   0        0        0     9097 2024-04-21 03:48:48.000000 cerbogen-0.0.46/cerbogen/mod/cerbogen.py
+-rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.46/cerbogen/mod/plot.py
+drwxrwxrwx   0        0        0        0 2024-04-21 04:01:32.532601 cerbogen-0.0.46/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      680 2024-04-21 04:01:32.000000 cerbogen-0.0.46/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2024-04-21 04:01:32.000000 cerbogen-0.0.46/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 04:01:32.000000 cerbogen-0.0.46/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-21 04:01:32.000000 cerbogen-0.0.46/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-21 04:01:32.000000 cerbogen-0.0.46/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 04:01:32.534596 cerbogen-0.0.46/setup.cfg
+-rw-rw-rw-   0        0        0     1287 2024-04-21 04:01:31.000000 cerbogen-0.0.46/setup.py
```

### Comparing `cerbogen-0.0.45/PKG-INFO` & `cerbogen-0.0.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.45
+Version: 0.0.46
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.45/cerbogen/install/check.py` & `cerbogen-0.0.46/cerbogen/install/check.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.45/cerbogen/install/install_ffmpeg.py` & `cerbogen-0.0.46/cerbogen/install/install_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.45/cerbogen/install/install_location.py` & `cerbogen-0.0.46/cerbogen/install/install_location.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.45/cerbogen/install/setup.py` & `cerbogen-0.0.46/cerbogen/install/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import os
 import platform
 # import install_ffmpeg
-from install_location import install_location
+from .install_location import install_location
 
 def install_pywin32():
     if platform.system() == "Windows":
         try:
             import win32com.client
         except ImportError:
             print("pywin32 not found. Installing...")
@@ -18,7 +18,9 @@
                 sys.exit(1)
 
 
 if __name__ == "__main__":
     
     install_pywin32()
     install_location()
+
+
```

### Comparing `cerbogen-0.0.45/cerbogen/mod/cerbogen.py` & `cerbogen-0.0.46/cerbogen/mod/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.45/cerbogen/mod/plot.py` & `cerbogen-0.0.46/cerbogen/mod/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.45/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.46/cerbogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.45
+Version: 0.0.46
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.45/setup.py` & `cerbogen-0.0.46/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self.custom_code()
     
     def custom_code(self):
         subprocess.run(['python', '-m', 'cerbogen.install.setup'])
 
 setup(
     name='cerbogen',
-    version = '0.0.45',
+    version = '0.0.46',
     description='A Python package for CerboTech',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Clarence Parmar',
     author_email='git.clarence@gmail.com',
     url='https://github.com/clarenceparmar/cerbogen',
     packages=find_packages(),
```


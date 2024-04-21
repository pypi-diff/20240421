# Comparing `tmp/cerbogen-0.0.41.tar.gz` & `tmp/cerbogen-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.41.tar", last modified: Sat Apr 20 16:53:34 2024, max compression
+gzip compressed data, was "cerbogen-0.0.42.tar", last modified: Sat Apr 20 17:02:25 2024, max compression
```

## Comparing `cerbogen-0.0.41.tar` & `cerbogen-0.0.42.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 16:53:34.141728 cerbogen-0.0.41/
--rw-rw-rw-   0        0        0      680 2024-04-20 16:53:34.140751 cerbogen-0.0.41/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.41/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 16:53:34.109519 cerbogen-0.0.41/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.41/cerbogen/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 16:53:34.107568 cerbogen-0.0.41/cerbogen/data/
-drwxrwxrwx   0        0        0        0 2024-04-20 16:53:34.125136 cerbogen-0.0.41/cerbogen/data/img/
--rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.41/cerbogen/data/img/logo.ico
--rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.41/cerbogen/data/img/logo.png
-drwxrwxrwx   0        0        0        0 2024-04-20 16:53:34.139777 cerbogen-0.0.41/cerbogen/mod/
--rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.41/cerbogen/mod/__init__.py
--rw-rw-rw-   0        0        0     9107 2024-04-20 15:20:54.000000 cerbogen-0.0.41/cerbogen/mod/cerbogen.py
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.41/cerbogen/mod/check.py
--rw-rw-rw-   0        0        0     2930 2024-04-20 16:38:30.000000 cerbogen-0.0.41/cerbogen/mod/install_ffmpeg.py
--rw-rw-rw-   0        0        0     2213 2024-04-20 16:53:16.000000 cerbogen-0.0.41/cerbogen/mod/install_location.py
--rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.41/cerbogen/mod/plot.py
--rw-rw-rw-   0        0        0     2051 2024-04-20 16:41:49.000000 cerbogen-0.0.41/cerbogen/mod/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 16:53:34.140751 cerbogen-0.0.41/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      680 2024-04-20 16:53:33.000000 cerbogen-0.0.41/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2024-04-20 16:53:34.000000 cerbogen-0.0.41/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 16:53:33.000000 cerbogen-0.0.41/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-20 16:53:33.000000 cerbogen-0.0.41/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-20 16:53:33.000000 cerbogen-0.0.41/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 16:53:34.141728 cerbogen-0.0.41/setup.cfg
--rw-rw-rw-   0        0        0     1062 2024-04-20 16:53:33.000000 cerbogen-0.0.41/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 17:02:25.915664 cerbogen-0.0.42/
+-rw-rw-rw-   0        0        0      680 2024-04-20 17:02:25.914688 cerbogen-0.0.42/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.42/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 17:02:25.881505 cerbogen-0.0.42/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.42/cerbogen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 17:02:25.879558 cerbogen-0.0.42/cerbogen/data/
+drwxrwxrwx   0        0        0        0 2024-04-20 17:02:25.904928 cerbogen-0.0.42/cerbogen/data/img/
+-rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.42/cerbogen/data/img/logo.ico
+-rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.42/cerbogen/data/img/logo.png
+drwxrwxrwx   0        0        0        0 2024-04-20 17:02:25.909807 cerbogen-0.0.42/cerbogen/install/
+-rw-rw-rw-   0        0        0        0 2024-04-20 16:57:31.000000 cerbogen-0.0.42/cerbogen/install/__init__.py
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.42/cerbogen/install/check.py
+-rw-rw-rw-   0        0        0     2930 2024-04-20 16:38:30.000000 cerbogen-0.0.42/cerbogen/install/install_ffmpeg.py
+-rw-rw-rw-   0        0        0     2213 2024-04-20 17:01:31.000000 cerbogen-0.0.42/cerbogen/install/install_location.py
+-rw-rw-rw-   0        0        0     2051 2024-04-20 16:41:49.000000 cerbogen-0.0.42/cerbogen/install/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 17:02:25.911759 cerbogen-0.0.42/cerbogen/mod/
+-rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.42/cerbogen/mod/__init__.py
+-rw-rw-rw-   0        0        0     9107 2024-04-20 15:20:54.000000 cerbogen-0.0.42/cerbogen/mod/cerbogen.py
+-rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.42/cerbogen/mod/plot.py
+drwxrwxrwx   0        0        0        0 2024-04-20 17:02:25.913711 cerbogen-0.0.42/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      680 2024-04-20 17:02:25.000000 cerbogen-0.0.42/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      513 2024-04-20 17:02:25.000000 cerbogen-0.0.42/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 17:02:25.000000 cerbogen-0.0.42/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-20 17:02:25.000000 cerbogen-0.0.42/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-20 17:02:25.000000 cerbogen-0.0.42/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 17:02:25.915664 cerbogen-0.0.42/setup.cfg
+-rw-rw-rw-   0        0        0     1097 2024-04-20 17:02:25.000000 cerbogen-0.0.42/setup.py
```

### Comparing `cerbogen-0.0.41/PKG-INFO` & `cerbogen-0.0.42/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.41
+Version: 0.0.42
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.41/cerbogen/data/img/logo.ico` & `cerbogen-0.0.42/cerbogen/data/img/logo.ico`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.41/cerbogen/data/img/logo.png` & `cerbogen-0.0.42/cerbogen/data/img/logo.png`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.41/cerbogen/mod/cerbogen.py` & `cerbogen-0.0.42/cerbogen/mod/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.41/cerbogen/mod/check.py` & `cerbogen-0.0.42/cerbogen/install/check.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.41/cerbogen/mod/install_ffmpeg.py` & `cerbogen-0.0.42/cerbogen/install/install_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.41/cerbogen/mod/install_location.py` & `cerbogen-0.0.42/cerbogen/install/install_location.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.41/cerbogen/mod/plot.py` & `cerbogen-0.0.42/cerbogen/mod/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.41/cerbogen/mod/setup.py` & `cerbogen-0.0.42/cerbogen/install/setup.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.41/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.42/cerbogen.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.41
+Version: 0.0.42
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.41/setup.py` & `cerbogen-0.0.42/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cerbogen',
-    version = '0.0.41',
+    version = '0.0.42',
     description='A Python package for CerboTech',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Clarence Parmar',
     author_email='git.clarence@gmail.com',
     url='https://github.com/clarenceparmar/cerbogen',
     packages=find_packages(),
     
     package_data={
-        '': ['ffmpeg/mac/*', 'data/img/*', 'mod/*']
+
+        '': [ 'install/*' , 'data/img/*', 'mod/*']
     },
 
     install_requires=[
         "matplotlib", "pydub", "numpy", "librosa"
     ],
     
     python_requires='>=3.6',
@@ -26,9 +27,11 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
 
     # Specify the script to be executed during installation
-    scripts=['cerbogen/mod/install_location.py']
+    scripts=[ 'cerbogen/install/install_location.py'
+             
+            ]
 )
```


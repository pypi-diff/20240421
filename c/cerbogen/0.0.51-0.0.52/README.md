# Comparing `tmp/cerbogen-0.0.51.tar.gz` & `tmp/cerbogen-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.51.tar", last modified: Sun Apr 21 07:14:20 2024, max compression
+gzip compressed data, was "cerbogen-0.0.52.tar", last modified: Sun Apr 21 07:16:32 2024, max compression
```

## Comparing `cerbogen-0.0.51.tar` & `cerbogen-0.0.52.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 07:14:20.358563 cerbogen-0.0.51/
--rw-rw-rw-   0        0        0      639 2024-04-21 07:14:20.357566 cerbogen-0.0.51/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.51/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 07:14:20.342606 cerbogen-0.0.51/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-21 05:43:23.000000 cerbogen-0.0.51/cerbogen/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:14:20.339614 cerbogen-0.0.51/cerbogen/data/
-drwxrwxrwx   0        0        0        0 2024-04-21 07:14:20.354575 cerbogen-0.0.51/cerbogen/data/img/
--rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.51/cerbogen/data/img/logo.ico
--rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.51/cerbogen/data/img/logo.png
--rw-rw-rw-   0        0        0    11564 2024-04-21 07:01:06.000000 cerbogen-0.0.51/cerbogen/main.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:14:20.356568 cerbogen-0.0.51/cerbogen/mod/
--rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.51/cerbogen/mod/__init__.py
--rw-rw-rw-   0        0        0     9057 2024-04-21 04:45:42.000000 cerbogen-0.0.51/cerbogen/mod/cerbogen.py
--rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.51/cerbogen/mod/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:14:20.357566 cerbogen-0.0.51/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      639 2024-04-21 07:14:20.000000 cerbogen-0.0.51/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2024-04-21 07:14:20.000000 cerbogen-0.0.51/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 07:14:20.000000 cerbogen-0.0.51/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-21 07:14:20.000000 cerbogen-0.0.51/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-21 07:14:20.000000 cerbogen-0.0.51/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 07:14:20.358563 cerbogen-0.0.51/setup.cfg
--rw-rw-rw-   0        0        0     1073 2024-04-21 07:14:19.000000 cerbogen-0.0.51/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 07:16:32.331352 cerbogen-0.0.52/
+-rw-rw-rw-   0        0        0      639 2024-04-21 07:16:32.330354 cerbogen-0.0.52/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.52/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 07:16:32.307415 cerbogen-0.0.52/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-21 05:43:23.000000 cerbogen-0.0.52/cerbogen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 07:16:32.304423 cerbogen-0.0.52/cerbogen/data/
+drwxrwxrwx   0        0        0        0 2024-04-21 07:16:32.322375 cerbogen-0.0.52/cerbogen/data/img/
+-rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.52/cerbogen/data/img/logo.ico
+-rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.52/cerbogen/data/img/logo.png
+drwxrwxrwx   0        0        0        0 2024-04-21 07:16:32.327362 cerbogen-0.0.52/cerbogen/install/
+-rw-rw-rw-   0        0        0        0 2024-04-21 07:16:05.000000 cerbogen-0.0.52/cerbogen/install/__init__.py
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.52/cerbogen/install/check.py
+-rw-rw-rw-   0        0        0      594 2024-04-21 05:43:25.000000 cerbogen-0.0.52/cerbogen/install/install.py
+-rw-rw-rw-   0        0        0     2930 2024-04-20 16:38:30.000000 cerbogen-0.0.52/cerbogen/install/install_ffmpeg.py
+-rw-rw-rw-   0        0        0     2212 2024-04-21 05:38:09.000000 cerbogen-0.0.52/cerbogen/install/install_location.py
+-rw-rw-rw-   0        0        0    11564 2024-04-21 07:01:06.000000 cerbogen-0.0.52/cerbogen/main.py
+drwxrwxrwx   0        0        0        0 2024-04-21 07:16:32.329356 cerbogen-0.0.52/cerbogen/mod/
+-rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.52/cerbogen/mod/__init__.py
+-rw-rw-rw-   0        0        0     9057 2024-04-21 04:45:42.000000 cerbogen-0.0.52/cerbogen/mod/cerbogen.py
+-rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.52/cerbogen/mod/plot.py
+drwxrwxrwx   0        0        0        0 2024-04-21 07:16:32.330354 cerbogen-0.0.52/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      639 2024-04-21 07:16:32.000000 cerbogen-0.0.52/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2024-04-21 07:16:32.000000 cerbogen-0.0.52/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 07:16:32.000000 cerbogen-0.0.52/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-21 07:16:32.000000 cerbogen-0.0.52/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-21 07:16:32.000000 cerbogen-0.0.52/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 07:16:32.331352 cerbogen-0.0.52/setup.cfg
+-rw-rw-rw-   0        0        0     1073 2024-04-21 07:16:31.000000 cerbogen-0.0.52/setup.py
```

### Comparing `cerbogen-0.0.51/PKG-INFO` & `cerbogen-0.0.52/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.51
+Version: 0.0.52
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.51/cerbogen/data/img/logo.ico` & `cerbogen-0.0.52/cerbogen/data/img/logo.ico`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.51/cerbogen/data/img/logo.png` & `cerbogen-0.0.52/cerbogen/data/img/logo.png`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.51/cerbogen/main.py` & `cerbogen-0.0.52/cerbogen/main.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.51/cerbogen/mod/cerbogen.py` & `cerbogen-0.0.52/cerbogen/mod/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.51/cerbogen/mod/plot.py` & `cerbogen-0.0.52/cerbogen/mod/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.51/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.52/cerbogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.51
+Version: 0.0.52
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.51/setup.py` & `cerbogen-0.0.52/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         print("Hello World")
 
     install_script_path = os.path.join(os.path.dirname(__file__), 'install', 'install.py')
     subprocess.run(['python', install_script_path])
 
 setup(
     name='cerbogen',
-    version = '0.0.51',
+    version = '0.0.52',
     description='A Python package for CerboTech',
     author='Clarence Parmar',
     author_email='git.clarence@gmail.com',
     url='https://github.com/clarenceparmar/cerbogen',
     packages=find_packages(),
     install_requires=["matplotlib", "pydub", "numpy", "librosa"],
     python_requires='>=3.6',
```


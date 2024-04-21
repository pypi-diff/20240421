# Comparing `tmp/cerbogen-0.0.43.tar.gz` & `tmp/cerbogen-0.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.43.tar", last modified: Sun Apr 21 03:40:24 2024, max compression
+gzip compressed data, was "cerbogen-0.0.44.tar", last modified: Sun Apr 21 03:44:47 2024, max compression
```

## Comparing `cerbogen-0.0.43.tar` & `cerbogen-0.0.44.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 03:40:24.624322 cerbogen-0.0.43/
--rw-rw-rw-   0        0        0      680 2024-04-21 03:40:24.623325 cerbogen-0.0.43/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.43/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 03:40:24.604863 cerbogen-0.0.43/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.43/cerbogen/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 03:40:24.618338 cerbogen-0.0.43/cerbogen/install/
--rw-rw-rw-   0        0        0        0 2024-04-20 16:57:31.000000 cerbogen-0.0.43/cerbogen/install/__init__.py
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.43/cerbogen/install/check.py
--rw-rw-rw-   0        0        0     2930 2024-04-20 16:38:30.000000 cerbogen-0.0.43/cerbogen/install/install_ffmpeg.py
--rw-rw-rw-   0        0        0     2428 2024-04-20 17:10:43.000000 cerbogen-0.0.43/cerbogen/install/install_location.py
--rw-rw-rw-   0        0        0     2051 2024-04-21 03:39:40.000000 cerbogen-0.0.43/cerbogen/install/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 03:40:24.621330 cerbogen-0.0.43/cerbogen/mod/
--rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.43/cerbogen/mod/__init__.py
--rw-rw-rw-   0        0        0     9107 2024-04-20 15:20:54.000000 cerbogen-0.0.43/cerbogen/mod/cerbogen.py
--rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.43/cerbogen/mod/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-21 03:40:24.622328 cerbogen-0.0.43/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      680 2024-04-21 03:40:24.000000 cerbogen-0.0.43/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2024-04-21 03:40:24.000000 cerbogen-0.0.43/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 03:40:24.000000 cerbogen-0.0.43/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-21 03:40:24.000000 cerbogen-0.0.43/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-21 03:40:24.000000 cerbogen-0.0.43/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 03:40:24.624322 cerbogen-0.0.43/setup.cfg
--rw-rw-rw-   0        0        0     1287 2024-04-21 03:40:24.000000 cerbogen-0.0.43/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 03:44:47.222352 cerbogen-0.0.44/
+-rw-rw-rw-   0        0        0      680 2024-04-21 03:44:47.221355 cerbogen-0.0.44/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.44/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 03:44:47.205397 cerbogen-0.0.44/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.44/cerbogen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 03:44:47.218363 cerbogen-0.0.44/cerbogen/install/
+-rw-rw-rw-   0        0        0        0 2024-04-20 16:57:31.000000 cerbogen-0.0.44/cerbogen/install/__init__.py
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.44/cerbogen/install/check.py
+-rw-rw-rw-   0        0        0     2930 2024-04-20 16:38:30.000000 cerbogen-0.0.44/cerbogen/install/install_ffmpeg.py
+-rw-rw-rw-   0        0        0     2450 2024-04-21 03:44:12.000000 cerbogen-0.0.44/cerbogen/install/install_location.py
+-rw-rw-rw-   0        0        0      573 2024-04-21 03:44:14.000000 cerbogen-0.0.44/cerbogen/install/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 03:44:47.220358 cerbogen-0.0.44/cerbogen/mod/
+-rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.44/cerbogen/mod/__init__.py
+-rw-rw-rw-   0        0        0     9107 2024-04-20 15:20:54.000000 cerbogen-0.0.44/cerbogen/mod/cerbogen.py
+-rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.44/cerbogen/mod/plot.py
+drwxrwxrwx   0        0        0        0 2024-04-21 03:44:47.221355 cerbogen-0.0.44/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      680 2024-04-21 03:44:47.000000 cerbogen-0.0.44/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2024-04-21 03:44:47.000000 cerbogen-0.0.44/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 03:44:47.000000 cerbogen-0.0.44/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-21 03:44:47.000000 cerbogen-0.0.44/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-21 03:44:47.000000 cerbogen-0.0.44/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 03:44:47.222352 cerbogen-0.0.44/setup.cfg
+-rw-rw-rw-   0        0        0     1287 2024-04-21 03:44:46.000000 cerbogen-0.0.44/setup.py
```

### Comparing `cerbogen-0.0.43/PKG-INFO` & `cerbogen-0.0.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.43
+Version: 0.0.44
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.43/cerbogen/install/check.py` & `cerbogen-0.0.44/cerbogen/install/check.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.43/cerbogen/install/install_ffmpeg.py` & `cerbogen-0.0.44/cerbogen/install/install_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.43/cerbogen/install/install_location.py` & `cerbogen-0.0.44/cerbogen/install/install_location.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,7 +62,10 @@
     install_button.grid(row=0, column=2)
 
     # Install button
     install_button = tk.Button(root, text="Install Cerbogen", command=install_cerbogen)
     install_button.pack(pady=10)
 
     root.mainloop()
+
+
+install_location()
```

### Comparing `cerbogen-0.0.43/cerbogen/mod/cerbogen.py` & `cerbogen-0.0.44/cerbogen/mod/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.43/cerbogen/mod/plot.py` & `cerbogen-0.0.44/cerbogen/mod/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.43/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.44/cerbogen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.43
+Version: 0.0.44
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.43/setup.py` & `cerbogen-0.0.44/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self.custom_code()
     
     def custom_code(self):
         subprocess.run(['python', '-m', 'cerbogen.install.setup'])
 
 setup(
     name='cerbogen',
-    version = '0.0.43',
+    version = '0.0.44',
     description='A Python package for CerboTech',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Clarence Parmar',
     author_email='git.clarence@gmail.com',
     url='https://github.com/clarenceparmar/cerbogen',
     packages=find_packages(),
```


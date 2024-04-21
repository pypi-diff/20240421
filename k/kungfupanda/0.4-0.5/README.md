# Comparing `tmp/kungfupanda-0.4.tar.gz` & `tmp/kungfupanda-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kungfupanda-0.4.tar", last modified: Sun Apr 21 19:20:01 2024, max compression
+gzip compressed data, was "kungfupanda-0.5.tar", last modified: Sun Apr 21 19:25:19 2024, max compression
```

## Comparing `kungfupanda-0.4.tar` & `kungfupanda-0.5.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-21 19:20:01.087346 kungfupanda-0.4/
--rw-r--r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      571 2024-04-21 19:20:01.087346 kungfupanda-0.4/PKG-INFO
-drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-21 19:20:01.087346 kungfupanda-0.4/kungfupanda/
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       27 2024-04-21 18:55:04.000000 kungfupanda-0.4/kungfupanda/__init__.py
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)    16158 2024-04-21 19:04:12.000000 kungfupanda-0.4/kungfupanda/kungfupanda.py
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)     1802 2024-04-21 18:33:00.000000 kungfupanda-0.4/kungfupanda/post_install.py
-drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-21 19:20:01.087346 kungfupanda-0.4/kungfupanda.egg-info/
--rw-r--r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      571 2024-04-21 19:20:01.000000 kungfupanda-0.4/kungfupanda.egg-info/PKG-INFO
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      299 2024-04-21 19:20:01.000000 kungfupanda-0.4/kungfupanda.egg-info/SOURCES.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)        1 2024-04-21 19:20:01.000000 kungfupanda-0.4/kungfupanda.egg-info/dependency_links.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       75 2024-04-21 19:20:01.000000 kungfupanda-0.4/kungfupanda.egg-info/entry_points.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       45 2024-04-21 19:20:01.000000 kungfupanda-0.4/kungfupanda.egg-info/requires.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       12 2024-04-21 19:20:01.000000 kungfupanda-0.4/kungfupanda.egg-info/top_level.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       38 2024-04-21 19:20:01.087346 kungfupanda-0.4/setup.cfg
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      849 2024-04-21 19:19:49.000000 kungfupanda-0.4/setup.py
+drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-21 19:25:19.456008 kungfupanda-0.5/
+-rw-r--r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      571 2024-04-21 19:25:19.456008 kungfupanda-0.5/PKG-INFO
+drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-21 19:25:19.456008 kungfupanda-0.5/kungfupanda/
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       27 2024-04-21 18:55:04.000000 kungfupanda-0.5/kungfupanda/__init__.py
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)    17936 2024-04-21 19:23:52.000000 kungfupanda-0.5/kungfupanda/kungfupanda.py
+drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-21 19:25:19.456008 kungfupanda-0.5/kungfupanda.egg-info/
+-rw-r--r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      571 2024-04-21 19:25:19.000000 kungfupanda-0.5/kungfupanda.egg-info/PKG-INFO
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      271 2024-04-21 19:25:19.000000 kungfupanda-0.5/kungfupanda.egg-info/SOURCES.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)        1 2024-04-21 19:25:19.000000 kungfupanda-0.5/kungfupanda.egg-info/dependency_links.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       80 2024-04-21 19:25:19.000000 kungfupanda-0.5/kungfupanda.egg-info/entry_points.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       45 2024-04-21 19:25:19.000000 kungfupanda-0.5/kungfupanda.egg-info/requires.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       12 2024-04-21 19:25:19.000000 kungfupanda-0.5/kungfupanda.egg-info/top_level.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       38 2024-04-21 19:25:19.456008 kungfupanda-0.5/setup.cfg
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      851 2024-04-21 19:25:12.000000 kungfupanda-0.5/setup.py
```

### Comparing `kungfupanda-0.4/PKG-INFO` & `kungfupanda-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kungfupanda
-Version: 0.4
+Version: 0.5
 Summary: A simple package to make everything easy for programmers for doing everything the cool way
 Home-page: 
 Author: The big fat panda
 Author-email: po_the_big_fat_panda@gmail.com
 Requires-Dist: requests>=2.25.1
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: pandas>=2.2.2
```

### Comparing `kungfupanda-0.4/kungfupanda.egg-info/PKG-INFO` & `kungfupanda-0.5/kungfupanda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kungfupanda
-Version: 0.4
+Version: 0.5
 Summary: A simple package to make everything easy for programmers for doing everything the cool way
 Home-page: 
 Author: The big fat panda
 Author-email: po_the_big_fat_panda@gmail.com
 Requires-Dist: requests>=2.25.1
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: pandas>=2.2.2
```

### Comparing `kungfupanda-0.4/setup.py` & `kungfupanda-0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='kungfupanda',
-    version='0.4',
+    version='0.5',
     author='The big fat panda',
     author_email='po_the_big_fat_panda@gmail.com',
     description="A simple package to make everything easy for programmers for doing everything the cool way",
     long_description="""A simple package for the people who are not bound by society rules 
     made by an cute panda who trained to be a dragon warrior
     For all the story watch the original triology
     Kung Fu Panda 1
@@ -17,13 +17,13 @@
     url='',
     packages=find_packages(),
     install_requires=[
         'requests>=2.25.1',
         'numpy>=1.21.0',
         'pandas>=2.2.2',
     ],
-    entry_points={
+   entry_points={
         'console_scripts': [
-            'kungfupanda_post_install = kungfupanda.post_install:main',
+            'kungfupanda_installed=kungfupanda.kungfupanda:print_message'
         ],
-    }
+    },
 )
```


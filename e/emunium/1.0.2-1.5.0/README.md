# Comparing `tmp/emunium-1.0.2.tar.gz` & `tmp/emunium-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emunium-1.0.2.tar", last modified: Sat Feb 17 07:35:00 2024, max compression
+gzip compressed data, was "emunium-1.5.0.tar", last modified: Sun Apr 21 05:26:24 2024, max compression
```

## Comparing `emunium-1.0.2.tar` & `emunium-1.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-02-17 07:35:00.448685 emunium-1.0.2/
--rw-rw-rw-   0        0        0     1080 2024-02-17 07:34:29.000000 emunium-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       34 2024-02-17 07:15:22.000000 emunium-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4270 2024-02-17 07:35:00.446995 emunium-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3462 2024-02-17 07:15:22.000000 emunium-1.0.2/README.MD
-drwxrwxrwx   0        0        0        0 2024-02-17 07:35:00.440222 emunium-1.0.2/emunium/
--rw-rw-rw-   0        0        0       22 2024-02-17 07:15:22.000000 emunium-1.0.2/emunium/__init__.py
--rw-rw-rw-   0        0        0     5420 2024-02-17 07:33:34.000000 emunium-1.0.2/emunium/emunium.py
-drwxrwxrwx   0        0        0        0 2024-02-17 07:35:00.446995 emunium-1.0.2/emunium.egg-info/
--rw-rw-rw-   0        0        0     4270 2024-02-17 07:35:00.000000 emunium-1.0.2/emunium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2024-02-17 07:35:00.000000 emunium-1.0.2/emunium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-17 07:35:00.000000 emunium-1.0.2/emunium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-02-17 07:35:00.000000 emunium-1.0.2/emunium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-02-17 07:35:00.000000 emunium-1.0.2/emunium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-17 07:35:00.448685 emunium-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1096 2024-02-17 07:34:08.000000 emunium-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 05:26:24.000730 emunium-1.5.0/
+-rw-rw-rw-   0        0        0     1080 2024-04-19 11:50:43.000000 emunium-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-19 11:50:43.000000 emunium-1.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4270 2024-04-21 05:26:24.000730 emunium-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3462 2024-04-21 05:00:46.000000 emunium-1.5.0/README.MD
+drwxrwxrwx   0        0        0        0 2024-04-21 05:26:23.993750 emunium-1.5.0/emunium/
+-rw-rw-rw-   0        0        0       22 2024-04-19 11:50:43.000000 emunium-1.5.0/emunium/__init__.py
+-rw-rw-rw-   0        0        0     7276 2024-04-21 05:25:05.000000 emunium-1.5.0/emunium/emunium.py
+drwxrwxrwx   0        0        0        0 2024-04-21 05:26:23.999733 emunium-1.5.0/emunium.egg-info/
+-rw-rw-rw-   0        0        0     4270 2024-04-21 05:26:23.000000 emunium-1.5.0/emunium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2024-04-21 05:26:23.000000 emunium-1.5.0/emunium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 05:26:23.000000 emunium-1.5.0/emunium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-21 05:26:23.000000 emunium-1.5.0/emunium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-21 05:26:23.000000 emunium-1.5.0/emunium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 05:26:24.001727 emunium-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1096 2024-04-21 05:10:00.000000 emunium-1.5.0/setup.py
```

### Comparing `emunium-1.0.2/LICENSE` & `emunium-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `emunium-1.0.2/PKG-INFO` & `emunium-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emunium
-Version: 1.0.2
+Version: 1.5.0
 Summary: A Python module for automating interactions to mimic human behavior in browsers when using Selenium or Pyppeteer. Provides utilities to programmatically move the mouse cursor, click on page elements, type text, and scroll as if performed by a human user.
 Home-page: https://github.com/DedInc/emunium
 Author: Maehdakvan
 Author-email: visitanimation@google.com
 Project-URL: Bug Tracker, https://github.com/DedInc/emunium/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `emunium-1.0.2/README.MD` & `emunium-1.5.0/README.MD`

 * *Files identical despite different names*

### Comparing `emunium-1.0.2/emunium.egg-info/PKG-INFO` & `emunium-1.5.0/emunium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emunium
-Version: 1.0.2
+Version: 1.5.0
 Summary: A Python module for automating interactions to mimic human behavior in browsers when using Selenium or Pyppeteer. Provides utilities to programmatically move the mouse cursor, click on page elements, type text, and scroll as if performed by a human user.
 Home-page: https://github.com/DedInc/emunium
 Author: Maehdakvan
 Author-email: visitanimation@google.com
 Project-URL: Bug Tracker, https://github.com/DedInc/emunium/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `emunium-1.0.2/setup.py` & `emunium-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='emunium',
-    version='1.0.2',
+    version='1.5.0',
     author='Maehdakvan',
     author_email='visitanimation@google.com',
     description='A Python module for automating interactions to mimic human behavior in browsers when using Selenium or Pyppeteer. Provides utilities to programmatically move the mouse cursor, click on page elements, type text, and scroll as if performed by a human user.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/DedInc/emunium',
     project_urls={
```


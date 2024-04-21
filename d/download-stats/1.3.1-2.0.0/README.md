# Comparing `tmp/download_stats-1.3.1.tar.gz` & `tmp/download_stats-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "download_stats-1.3.1.tar", last modified: Tue Apr 16 11:15:30 2024, max compression
+gzip compressed data, was "download_stats-2.0.0.tar", last modified: Sun Apr 21 07:32:49 2024, max compression
```

## Comparing `download_stats-1.3.1.tar` & `download_stats-2.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:15:30.716811 download_stats-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 11:15:26.000000 download_stats-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-16 11:15:26.000000 download_stats-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-16 11:15:30.716811 download_stats-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-16 11:15:26.000000 download_stats-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:15:30.716811 download_stats-1.3.1/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    15299 2024-04-16 11:15:26.000000 download_stats-1.3.1/assets/compare.png
--rw-r--r--   0 runner    (1001) docker     (127)    68629 2024-04-16 11:15:26.000000 download_stats-1.3.1/assets/download_stats.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:15:30.716811 download_stats-1.3.1/reqs/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-16 11:15:26.000000 download_stats-1.3.1/reqs/app.in
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-16 11:15:26.000000 download_stats-1.3.1/reqs/app.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 11:15:26.000000 download_stats-1.3.1/reqs/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-16 11:15:26.000000 download_stats-1.3.1/reqs/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-16 11:15:30.720811 download_stats-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-16 11:15:26.000000 download_stats-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:15:30.712811 download_stats-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:15:30.716811 download_stats-1.3.1/src/download_stats/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 11:15:26.000000 download_stats-1.3.1/src/download_stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-16 11:15:26.000000 download_stats-1.3.1/src/download_stats/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-16 11:15:26.000000 download_stats-1.3.1/src/download_stats/pepy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-16 11:15:26.000000 download_stats-1.3.1/src/download_stats/pypistats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:15:30.716811 download_stats-1.3.1/src/download_stats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-16 11:15:30.000000 download_stats-1.3.1/src/download_stats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-16 11:15:30.000000 download_stats-1.3.1/src/download_stats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:15:30.000000 download_stats-1.3.1/src/download_stats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-16 11:15:30.000000 download_stats-1.3.1/src/download_stats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-16 11:15:30.000000 download_stats-1.3.1/src/download_stats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 11:15:30.000000 download_stats-1.3.1/src/download_stats.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:15:30.716811 download_stats-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-16 11:15:26.000000 download_stats-1.3.1/tests/test_pepy.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-16 11:15:26.000000 download_stats-1.3.1/tests/test_pypistats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:32:49.250443 download_stats-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 07:32:45.000000 download_stats-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-21 07:32:45.000000 download_stats-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-21 07:32:49.250443 download_stats-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-21 07:32:45.000000 download_stats-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:32:49.246443 download_stats-2.0.0/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    15299 2024-04-21 07:32:45.000000 download_stats-2.0.0/assets/compare.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68629 2024-04-21 07:32:45.000000 download_stats-2.0.0/assets/download_stats.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:32:49.246443 download_stats-2.0.0/reqs/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 07:32:45.000000 download_stats-2.0.0/reqs/app.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-21 07:32:45.000000 download_stats-2.0.0/reqs/app.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 07:32:45.000000 download_stats-2.0.0/reqs/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-21 07:32:45.000000 download_stats-2.0.0/reqs/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-21 07:32:49.250443 download_stats-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-21 07:32:45.000000 download_stats-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:32:49.246443 download_stats-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:32:49.246443 download_stats-2.0.0/src/download_stats/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-21 07:32:45.000000 download_stats-2.0.0/src/download_stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-21 07:32:45.000000 download_stats-2.0.0/src/download_stats/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-21 07:32:45.000000 download_stats-2.0.0/src/download_stats/pepy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-21 07:32:45.000000 download_stats-2.0.0/src/download_stats/pypistats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:32:49.250443 download_stats-2.0.0/src/download_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-21 07:32:49.000000 download_stats-2.0.0/src/download_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-21 07:32:49.000000 download_stats-2.0.0/src/download_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 07:32:49.000000 download_stats-2.0.0/src/download_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-21 07:32:49.000000 download_stats-2.0.0/src/download_stats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 07:32:49.000000 download_stats-2.0.0/src/download_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 07:32:49.000000 download_stats-2.0.0/src/download_stats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:32:49.250443 download_stats-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-21 07:32:45.000000 download_stats-2.0.0/tests/test_pepy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-21 07:32:45.000000 download_stats-2.0.0/tests/test_pypistats.py
```

### Comparing `download_stats-1.3.1/LICENSE` & `download_stats-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `download_stats-1.3.1/PKG-INFO` & `download_stats-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: download_stats
-Version: 1.3.1
+Version: 2.0.0
 Summary: Download stats for Python packages
 Author-email: arj.python@gmail.com
 Project-URL: Bug Reports, https://github.com/Abdur-RahmaanJ/download-stats/issues
 Project-URL: Source, https://github.com/Abdur-RahmaanJ/download-stats/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich
-Requires-Dist: selenium
-Requires-Dist: webdriver_manager>=3.8.6
-Requires-Dist: latest_user_agents>=0.0.3
 Requires-Dist: requests
 
 # download-stats
 
 View your pypi download stats
 
 # cli
```

### Comparing `download_stats-1.3.1/README.md` & `download_stats-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `download_stats-1.3.1/assets/compare.png` & `download_stats-2.0.0/assets/compare.png`

 * *Files identical despite different names*

### Comparing `download_stats-1.3.1/assets/download_stats.png` & `download_stats-2.0.0/assets/download_stats.png`

 * *Files identical despite different names*

### Comparing `download_stats-1.3.1/reqs/app.txt` & `download_stats-2.0.0/reqs/app.txt`

 * *Files identical despite different names*

### Comparing `download_stats-1.3.1/reqs/dev.txt` & `download_stats-2.0.0/reqs/dev.txt`

 * *Files identical despite different names*

### Comparing `download_stats-1.3.1/setup.py` & `download_stats-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 setup(
     name="download_stats",  # Required
-    version="1.3.1",  # Required
+    version="2.0.0",  # Required
     description="Download stats for Python packages",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     # url="https://github.com/Abdur-RahmaanJ/greenBerry",  # Optional
     # author="Abdur-Rahmaan Janhangeer & contributors",  # Optional
     author_email="arj.python@gmail.com",  # Optional
     # Classifiers help users find your project by categorizing it.
@@ -58,14 +58,15 @@
         # These classifiers are *not* checked by 'pip install'. See instead
         # 'python_requires' below.
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     # keywords="",  # Optional
     # You can just specify package directories manually here if your project is
     # simple. Or you can use find_packages().
     #
     # Alternatively, if you just want to distribute a single Python file, use
     # the `py_modules` argument instead as follows, which will expect a file
```

### Comparing `download_stats-1.3.1/src/download_stats/main.py` & `download_stats-2.0.0/src/download_stats/main.py`

 * *Files identical despite different names*

### Comparing `download_stats-1.3.1/src/download_stats/pypistats.py` & `download_stats-2.0.0/src/download_stats/pypistats.py`

 * *Files identical despite different names*

### Comparing `download_stats-1.3.1/src/download_stats.egg-info/PKG-INFO` & `download_stats-2.0.0/src/download_stats.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: download_stats
-Version: 1.3.1
+Version: 2.0.0
 Summary: Download stats for Python packages
 Author-email: arj.python@gmail.com
 Project-URL: Bug Reports, https://github.com/Abdur-RahmaanJ/download-stats/issues
 Project-URL: Source, https://github.com/Abdur-RahmaanJ/download-stats/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich
-Requires-Dist: selenium
-Requires-Dist: webdriver_manager>=3.8.6
-Requires-Dist: latest_user_agents>=0.0.3
 Requires-Dist: requests
 
 # download-stats
 
 View your pypi download stats
 
 # cli
```

### Comparing `download_stats-1.3.1/src/download_stats.egg-info/SOURCES.txt` & `download_stats-2.0.0/src/download_stats.egg-info/SOURCES.txt`

 * *Files identical despite different names*


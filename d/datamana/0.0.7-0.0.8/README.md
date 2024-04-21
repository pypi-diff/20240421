# Comparing `tmp/datamana-0.0.7.tar.gz` & `tmp/datamana-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamana-0.0.7.tar", last modified: Sat Apr 20 01:30:25 2024, max compression
+gzip compressed data, was "datamana-0.0.8.tar", last modified: Sun Apr 21 08:41:46 2024, max compression
```

## Comparing `datamana-0.0.7.tar` & `datamana-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:30:25.805787 datamana-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-20 01:30:17.000000 datamana-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-20 01:30:17.000000 datamana-0.0.7/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-20 01:30:17.000000 datamana-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-20 01:30:17.000000 datamana-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-20 01:30:25.805787 datamana-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:30:17.000000 datamana-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:30:25.805787 datamana-0.0.7/csrc/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-20 01:30:17.000000 datamana-0.0.7/csrc/mqueue.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-20 01:30:17.000000 datamana-0.0.7/csrc/python.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-20 01:30:17.000000 datamana-0.0.7/csrc/semaphore.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:30:25.805787 datamana-0.0.7/datamana/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:30:17.000000 datamana-0.0.7/datamana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:30:17.000000 datamana-0.0.7/datamana/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-20 01:30:17.000000 datamana-0.0.7/datamana/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:30:25.805787 datamana-0.0.7/datamana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-20 01:30:25.000000 datamana-0.0.7/datamana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-20 01:30:25.000000 datamana-0.0.7/datamana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:30:25.000000 datamana-0.0.7/datamana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 01:30:25.000000 datamana-0.0.7/datamana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 01:30:25.000000 datamana-0.0.7/datamana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-20 01:30:17.000000 datamana-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 01:30:25.809787 datamana-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-20 01:30:17.000000 datamana-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:41:46.795148 datamana-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-21 08:41:40.000000 datamana-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-21 08:41:40.000000 datamana-0.0.8/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 08:41:40.000000 datamana-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-21 08:41:40.000000 datamana-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-21 08:41:46.795148 datamana-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 08:41:40.000000 datamana-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:41:46.795148 datamana-0.0.8/csrc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-21 08:41:40.000000 datamana-0.0.8/csrc/mqueue.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-21 08:41:40.000000 datamana-0.0.8/csrc/python.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-21 08:41:40.000000 datamana-0.0.8/csrc/semaphore.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:41:46.795148 datamana-0.0.8/datamana/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 08:41:40.000000 datamana-0.0.8/datamana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 08:41:40.000000 datamana-0.0.8/datamana/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-21 08:41:40.000000 datamana-0.0.8/datamana/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:41:46.795148 datamana-0.0.8/datamana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-21 08:41:46.000000 datamana-0.0.8/datamana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-21 08:41:46.000000 datamana-0.0.8/datamana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 08:41:46.000000 datamana-0.0.8/datamana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 08:41:46.000000 datamana-0.0.8/datamana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 08:41:46.000000 datamana-0.0.8/datamana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-21 08:41:40.000000 datamana-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 08:41:46.795148 datamana-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-21 08:41:40.000000 datamana-0.0.8/setup.py
```

### Comparing `datamana-0.0.7/.gitignore` & `datamana-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `datamana-0.0.7/CMakeLists.txt` & `datamana-0.0.8/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datamana-0.0.7/LICENSE` & `datamana-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `datamana-0.0.7/PKG-INFO` & `datamana-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamana
-Version: 0.0.7
+Version: 0.0.8
 Summary: Dataset Manager
 Author-email: Jiau Zhang <jiauzhang@163.com>
 Project-URL: Homepage, https://github.com/jiauzhang/datamana
 Keywords: Deep Learning,Dataset Manager,Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamana-0.0.7/datamana/torch.py` & `datamana-0.0.8/datamana/torch.py`

 * *Files identical despite different names*

### Comparing `datamana-0.0.7/datamana.egg-info/PKG-INFO` & `datamana-0.0.8/datamana.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamana
-Version: 0.0.7
+Version: 0.0.8
 Summary: Dataset Manager
 Author-email: Jiau Zhang <jiauzhang@163.com>
 Project-URL: Homepage, https://github.com/jiauzhang/datamana
 Keywords: Deep Learning,Dataset Manager,Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamana-0.0.7/pyproject.toml` & `datamana-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "cmake >= 3.15",
     "nanobind >= 1.9.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datamana"
-version = "0.0.7"
+version = "0.0.8"
 description = "Dataset Manager"
 readme = "README.md"
 authors = [
     {name = "Jiau Zhang", email = "jiauzhang@163.com"},
 ]
 classifiers = [
     'Intended Audience :: Developers',
```

### Comparing `datamana-0.0.7/setup.py` & `datamana-0.0.8/setup.py`

 * *Files identical despite different names*


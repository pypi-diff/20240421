# Comparing `tmp/profiles_local-0.0.69.tar.gz` & `tmp/profiles_local-0.0.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profiles_local-0.0.69.tar", last modified: Sun Apr 21 13:58:58 2024, max compression
+gzip compressed data, was "profiles_local-0.0.70.tar", last modified: Sun Apr 21 14:09:13 2024, max compression
```

## Comparing `profiles_local-0.0.69.tar` & `profiles_local-0.0.70.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:58:58.471919 profiles_local-0.0.69/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-21 13:58:58.471919 profiles_local-0.0.69/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-21 13:58:32.000000 profiles_local-0.0.69/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:58:58.467919 profiles_local-0.0.69/profiles_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:58:58.471919 profiles_local-0.0.69/profiles_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:58:32.000000 profiles_local-0.0.69/profiles_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-21 13:58:32.000000 profiles_local-0.0.69/profiles_local/src/comprehensive_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-21 13:58:32.000000 profiles_local-0.0.69/profiles_local/src/constants_profiles_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-04-21 13:58:32.000000 profiles_local-0.0.69/profiles_local/src/profiles_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:58:58.471919 profiles_local-0.0.69/profiles_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-21 13:58:58.000000 profiles_local-0.0.69/profiles_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-21 13:58:58.000000 profiles_local-0.0.69/profiles_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:58:58.000000 profiles_local-0.0.69/profiles_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-21 13:58:58.000000 profiles_local-0.0.69/profiles_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 13:58:58.000000 profiles_local-0.0.69/profiles_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-21 13:58:32.000000 profiles_local-0.0.69/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 13:58:58.471919 profiles_local-0.0.69/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-21 13:58:32.000000 profiles_local-0.0.69/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:09:13.451588 profiles_local-0.0.70/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-21 14:09:13.451588 profiles_local-0.0.70/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-21 14:08:38.000000 profiles_local-0.0.70/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:09:13.447588 profiles_local-0.0.70/profiles_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:09:13.447588 profiles_local-0.0.70/profiles_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 14:08:38.000000 profiles_local-0.0.70/profiles_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-21 14:08:38.000000 profiles_local-0.0.70/profiles_local/src/comprehensive_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-21 14:08:38.000000 profiles_local-0.0.70/profiles_local/src/constants_profiles_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-04-21 14:08:38.000000 profiles_local-0.0.70/profiles_local/src/profiles_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:09:13.451588 profiles_local-0.0.70/profiles_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-21 14:09:13.000000 profiles_local-0.0.70/profiles_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-21 14:09:13.000000 profiles_local-0.0.70/profiles_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 14:09:13.000000 profiles_local-0.0.70/profiles_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-21 14:09:13.000000 profiles_local-0.0.70/profiles_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 14:09:13.000000 profiles_local-0.0.70/profiles_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-21 14:08:38.000000 profiles_local-0.0.70/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 14:09:13.451588 profiles_local-0.0.70/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-21 14:08:38.000000 profiles_local-0.0.70/setup.py
```

### Comparing `profiles_local-0.0.69/PKG-INFO` & `profiles_local-0.0.70/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profiles-local
-Version: 0.0.69
+Version: 0.0.70
 Summary: This is a package for sharing common crud operation to profile schema in the db
 Home-page: https://github.com/circles-zone/profiles-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `profiles_local-0.0.69/README.md` & `profiles_local-0.0.70/README.md`

 * *Files identical despite different names*

### Comparing `profiles_local-0.0.69/profiles_local/src/comprehensive_profile.py` & `profiles_local-0.0.70/profiles_local/src/comprehensive_profile.py`

 * *Files identical despite different names*

### Comparing `profiles_local-0.0.69/profiles_local/src/constants_profiles_local.py` & `profiles_local-0.0.70/profiles_local/src/constants_profiles_local.py`

 * *Files identical despite different names*

### Comparing `profiles_local-0.0.69/profiles_local/src/profiles_local.py` & `profiles_local-0.0.70/profiles_local/src/profiles_local.py`

 * *Files identical despite different names*

### Comparing `profiles_local-0.0.69/profiles_local.egg-info/PKG-INFO` & `profiles_local-0.0.70/profiles_local.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profiles-local
-Version: 0.0.69
+Version: 0.0.70
 Summary: This is a package for sharing common crud operation to profile schema in the db
 Home-page: https://github.com/circles-zone/profiles-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `profiles_local-0.0.69/setup.py` & `profiles_local-0.0.70/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "profiles-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.69',  # https://pypi.org/project/profiles-local/
+    version='0.0.70',  # https://pypi.org/project/profiles-local/
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     description="This is a package for sharing common crud operation to profile schema in the db",
```


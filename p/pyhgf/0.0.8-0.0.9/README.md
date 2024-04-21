# Comparing `tmp/pyhgf-0.0.8.tar.gz` & `tmp/pyhgf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhgf-0.0.8.tar", last modified: Thu Sep  7 09:00:19 2023, max compression
+gzip compressed data, was "pyhgf-0.0.9.tar", last modified: Thu Sep  7 10:56:36 2023, max compression
```

## Comparing `pyhgf-0.0.8.tar` & `pyhgf-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-07 09:00:19.143211 pyhgf-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (999)    34493 2023-09-07 09:00:07.000000 pyhgf-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      104 2023-09-07 09:00:07.000000 pyhgf-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     7618 2023-09-07 09:00:19.143211 pyhgf-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     7043 2023-09-07 09:00:07.000000 pyhgf-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-07 09:00:19.143211 pyhgf-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1963 2023-09-07 09:00:07.000000 pyhgf-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-07 09:00:19.139211 pyhgf-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-07 09:00:19.139211 pyhgf-0.0.8/src/pyhgf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     7618 2023-09-07 09:00:19.000000 pyhgf-0.0.8/src/pyhgf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      389 2023-09-07 09:00:19.000000 pyhgf-0.0.8/src/pyhgf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-07 09:00:19.000000 pyhgf-0.0.8/src/pyhgf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)      123 2023-09-07 09:00:19.000000 pyhgf-0.0.8/src/pyhgf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-07 09:00:19.000000 pyhgf-0.0.8/src/pyhgf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-07 09:00:19.143211 pyhgf-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (999)     5728 2023-09-07 09:00:07.000000 pyhgf-0.0.8/tests/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (999)      994 2023-09-07 09:00:07.000000 pyhgf-0.0.8/tests/test_categorical.py
--rw-r--r--   0 runner    (1001) docker     (999)     8150 2023-09-07 09:00:07.000000 pyhgf-0.0.8/tests/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (999)    12338 2023-09-07 09:00:07.000000 pyhgf-0.0.8/tests/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (999)     5050 2023-09-07 09:00:07.000000 pyhgf-0.0.8/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (999)     4712 2023-09-07 09:00:07.000000 pyhgf-0.0.8/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (999)     1072 2023-09-07 09:00:07.000000 pyhgf-0.0.8/tests/test_responses.py
--rw-r--r--   0 runner    (1001) docker     (999)     3802 2023-09-07 09:00:07.000000 pyhgf-0.0.8/tests/test_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 10:56:36.812018 pyhgf-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    34493 2023-09-07 10:56:10.000000 pyhgf-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2023-09-07 10:56:10.000000 pyhgf-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2023-09-07 10:56:36.812018 pyhgf-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2023-09-07 10:56:10.000000 pyhgf-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-07 10:56:36.812018 pyhgf-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2023-09-07 10:56:10.000000 pyhgf-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 10:56:36.804018 pyhgf-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 10:56:36.808018 pyhgf-0.0.9/src/pyhgf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2023-09-07 10:56:10.000000 pyhgf-0.0.9/src/pyhgf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 10:56:36.812018 pyhgf-0.0.9/src/pyhgf/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     8000 2023-09-07 10:56:10.000000 pyhgf-0.0.9/src/pyhgf/data/binary_input.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8000 2023-09-07 10:56:10.000000 pyhgf-0.0.9/src/pyhgf/data/binary_response.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15350 2023-09-07 10:56:10.000000 pyhgf-0.0.9/src/pyhgf/data/usdchf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21724 2023-09-07 10:56:10.000000 pyhgf-0.0.9/src/pyhgf/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31442 2023-09-07 10:56:10.000000 pyhgf-0.0.9/src/pyhgf/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19040 2023-09-07 10:56:10.000000 pyhgf-0.0.9/src/pyhgf/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21674 2023-09-07 10:56:10.000000 pyhgf-0.0.9/src/pyhgf/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2023-09-07 10:56:10.000000 pyhgf-0.0.9/src/pyhgf/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2023-09-07 10:56:10.000000 pyhgf-0.0.9/src/pyhgf/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 10:56:36.812018 pyhgf-0.0.9/src/pyhgf/updates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 10:56:10.000000 pyhgf-0.0.9/src/pyhgf/updates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22289 2023-09-07 10:56:10.000000 pyhgf-0.0.9/src/pyhgf/updates/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5648 2023-09-07 10:56:10.000000 pyhgf-0.0.9/src/pyhgf/updates/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31596 2023-09-07 10:56:10.000000 pyhgf-0.0.9/src/pyhgf/updates/continuous.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 10:56:36.808018 pyhgf-0.0.9/src/pyhgf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2023-09-07 10:56:36.000000 pyhgf-0.0.9/src/pyhgf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2023-09-07 10:56:36.000000 pyhgf-0.0.9/src/pyhgf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-07 10:56:36.000000 pyhgf-0.0.9/src/pyhgf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2023-09-07 10:56:36.000000 pyhgf-0.0.9/src/pyhgf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-07 10:56:36.000000 pyhgf-0.0.9/src/pyhgf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 10:56:36.812018 pyhgf-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2023-09-07 10:56:10.000000 pyhgf-0.0.9/tests/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2023-09-07 10:56:10.000000 pyhgf-0.0.9/tests/test_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8150 2023-09-07 10:56:10.000000 pyhgf-0.0.9/tests/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12338 2023-09-07 10:56:10.000000 pyhgf-0.0.9/tests/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2023-09-07 10:56:10.000000 pyhgf-0.0.9/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2023-09-07 10:56:10.000000 pyhgf-0.0.9/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-09-07 10:56:10.000000 pyhgf-0.0.9/tests/test_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2023-09-07 10:56:10.000000 pyhgf-0.0.9/tests/test_structure.py
```

### Comparing `pyhgf-0.0.8/LICENSE` & `pyhgf-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.8/PKG-INFO` & `pyhgf-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhgf
-Version: 0.0.8
+Version: 0.0.9
 Summary: The generalized, nodalized HGF for predictive coding.
 Author: ILAB
 Author-email: nicolas.legrand@cas.au.dk
 Maintainer: Nicolas Legrand
 Maintainer-email: nicolas.legrand@cas.au.dk
 License: GPL-3.0
 Description-Content-Type: text/markdown
```

### Comparing `pyhgf-0.0.8/README.md` & `pyhgf-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.8/setup.py` & `pyhgf-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,9 +53,9 @@
         long_description_content_type="text/markdown",
         license="GPL-3.0",
         version=get_version("src/pyhgf/__init__.py"),
         install_requires=get_requirements(),
         include_package_data=True,
         package_dir = {"": "src"},
         package_data={"": ["pyhgf/src/pyhgf/data/*.dat"]},
-        packages=find_packages(),
+        packages=find_packages(where='src'),
     )
```

### Comparing `pyhgf-0.0.8/src/pyhgf.egg-info/PKG-INFO` & `pyhgf-0.0.9/src/pyhgf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhgf
-Version: 0.0.8
+Version: 0.0.9
 Summary: The generalized, nodalized HGF for predictive coding.
 Author: ILAB
 Author-email: nicolas.legrand@cas.au.dk
 Maintainer: Nicolas Legrand
 Maintainer-email: nicolas.legrand@cas.au.dk
 License: GPL-3.0
 Description-Content-Type: text/markdown
```

### Comparing `pyhgf-0.0.8/tests/test_binary.py` & `pyhgf-0.0.9/tests/test_binary.py`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.8/tests/test_categorical.py` & `pyhgf-0.0.9/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.8/tests/test_continuous.py` & `pyhgf-0.0.9/tests/test_continuous.py`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.8/tests/test_distribution.py` & `pyhgf-0.0.9/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.8/tests/test_model.py` & `pyhgf-0.0.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.8/tests/test_plots.py` & `pyhgf-0.0.9/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.8/tests/test_responses.py` & `pyhgf-0.0.9/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.8/tests/test_structure.py` & `pyhgf-0.0.9/tests/test_structure.py`

 * *Files identical despite different names*


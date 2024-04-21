# Comparing `tmp/hfutils-0.2.0.tar.gz` & `tmp/hfutils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfutils-0.2.0.tar", last modified: Sat Apr 20 18:02:02 2024, max compression
+gzip compressed data, was "hfutils-0.2.1.tar", last modified: Sun Apr 21 09:10:43 2024, max compression
```

## Comparing `hfutils-0.2.0.tar` & `hfutils-0.2.1.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.849096 hfutils-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-20 18:01:44.000000 hfutils-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 18:01:44.000000 hfutils-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-04-20 18:02:02.849096 hfutils-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-04-20 18:01:44.000000 hfutils-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.841096 hfutils-0.2.0/hfutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.841096 hfutils-0.2.0/hfutils/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/archive/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/archive/rar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/archive/sevenz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/archive/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/archive/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.841096 hfutils-0.2.0/hfutils/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.841096 hfutils-0.2.0/hfutils/entry/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/entry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/entry/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/entry/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/entry/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/entry/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/entry/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/entry/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.841096 hfutils-0.2.0/hfutils/index/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/index/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/index/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/index/make.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.845096 hfutils-0.2.0/hfutils/operate/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/operate/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/operate/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/operate/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/operate/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.845096 hfutils-0.2.0/hfutils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/utils/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/utils/temp.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/utils/tqdm_.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/utils/walk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.845096 hfutils-0.2.0/hfutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-04-20 18:02:02.000000 hfutils-0.2.0/hfutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-20 18:02:02.000000 hfutils-0.2.0/hfutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:02:02.000000 hfutils-0.2.0/hfutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-20 18:02:02.000000 hfutils-0.2.0/hfutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-20 18:02:02.000000 hfutils-0.2.0/hfutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 18:02:02.000000 hfutils-0.2.0/hfutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-20 18:01:44.000000 hfutils-0.2.0/requirements-7z.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-20 18:01:44.000000 hfutils-0.2.0/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-20 18:01:44.000000 hfutils-0.2.0/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 18:01:44.000000 hfutils-0.2.0/requirements-rar.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-20 18:01:44.000000 hfutils-0.2.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 18:01:44.000000 hfutils-0.2.0/requirements-transfer.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-20 18:01:44.000000 hfutils-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:02:02.849096 hfutils-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-20 18:01:44.000000 hfutils-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:10:43.385848 hfutils-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-21 09:10:21.000000 hfutils-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-21 09:10:21.000000 hfutils-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-04-21 09:10:43.385848 hfutils-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-04-21 09:10:21.000000 hfutils-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:10:43.373848 hfutils-0.2.1/hfutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:10:43.377848 hfutils-0.2.1/hfutils/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/archive/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/archive/rar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/archive/sevenz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/archive/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/archive/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:10:43.377848 hfutils-0.2.1/hfutils/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:10:43.377848 hfutils-0.2.1/hfutils/entry/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/entry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/entry/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/entry/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/entry/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/entry/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/entry/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/entry/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:10:43.377848 hfutils-0.2.1/hfutils/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/index/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/index/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/index/make.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/index/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:10:43.377848 hfutils-0.2.1/hfutils/operate/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/operate/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/operate/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/operate/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/operate/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:10:43.377848 hfutils-0.2.1/hfutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/utils/temp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/utils/tqdm_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-21 09:10:21.000000 hfutils-0.2.1/hfutils/utils/walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:10:43.377848 hfutils-0.2.1/hfutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-04-21 09:10:43.000000 hfutils-0.2.1/hfutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-21 09:10:43.000000 hfutils-0.2.1/hfutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:10:43.000000 hfutils-0.2.1/hfutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-21 09:10:43.000000 hfutils-0.2.1/hfutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-21 09:10:43.000000 hfutils-0.2.1/hfutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 09:10:43.000000 hfutils-0.2.1/hfutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-21 09:10:21.000000 hfutils-0.2.1/requirements-7z.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-21 09:10:21.000000 hfutils-0.2.1/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-21 09:10:21.000000 hfutils-0.2.1/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 09:10:21.000000 hfutils-0.2.1/requirements-rar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-21 09:10:21.000000 hfutils-0.2.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 09:10:21.000000 hfutils-0.2.1/requirements-transfer.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-21 09:10:21.000000 hfutils-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 09:10:43.385848 hfutils-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-21 09:10:21.000000 hfutils-0.2.1/setup.py
```

### Comparing `hfutils-0.2.0/LICENSE` & `hfutils-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/PKG-INFO` & `hfutils-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.2.0
+Version: 0.2.1
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hfutils-0.2.0/README.md` & `hfutils-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/archive/__init__.py` & `hfutils-0.2.1/hfutils/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/archive/base.py` & `hfutils-0.2.1/hfutils/archive/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/archive/rar.py` & `hfutils-0.2.1/hfutils/archive/rar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/archive/sevenz.py` & `hfutils-0.2.1/hfutils/archive/sevenz.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/archive/tar.py` & `hfutils-0.2.1/hfutils/archive/tar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/archive/zip.py` & `hfutils-0.2.1/hfutils/archive/zip.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/entry/base.py` & `hfutils-0.2.1/hfutils/entry/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/entry/dispatch.py` & `hfutils-0.2.1/hfutils/entry/dispatch.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/entry/download.py` & `hfutils-0.2.1/hfutils/entry/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/entry/ls.py` & `hfutils-0.2.1/hfutils/entry/ls.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/entry/upload.py` & `hfutils-0.2.1/hfutils/entry/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/index/fetch.py` & `hfutils-0.2.1/hfutils/index/fetch.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/index/hash.py` & `hfutils-0.2.1/hfutils/index/hash.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/index/make.py` & `hfutils-0.2.1/hfutils/index/make.py`

 * *Files 10% similar despite different names*

```diff
@@ -88,66 +88,88 @@
     body, _ = os.path.splitext(src_tar_file)
     dst_index_file = dst_index_file or f'{body}.json'
     with open(dst_index_file, 'w') as f:
         json.dump(tar_get_index_info(src_tar_file, chunk_for_hash, with_hash, silent), f)
     return dst_index_file
 
 
-def hf_tar_create_index(repo_id: str, filename: str, repo_type: RepoTypeTyping = 'dataset', revision: str = 'main',
-                        idx_repo_id: Optional[str] = None, idx_filename: Optional[str] = None,
+def hf_tar_create_index(repo_id: str, archive_in_repo: str,
+                        repo_type: RepoTypeTyping = 'dataset', revision: str = 'main',
+                        idx_repo_id: Optional[str] = None, idx_file_in_repo: Optional[str] = None,
                         idx_repo_type: Optional[RepoTypeTyping] = None, idx_revision: Optional[str] = None,
-                        chunk_for_hash: int = 1 << 20, with_hash: bool = True, hf_token: Optional[str] = None):
+                        chunk_for_hash: int = 1 << 20, with_hash: bool = True, skip_when_synced: bool = True,
+                        hf_token: Optional[str] = None, ):
     """
     Create an index file for a tar archive file in a Hugging Face repository.
 
     :param repo_id: The identifier of the repository.
     :type repo_id: str
-    :param filename: The path to the tar archive file.
-    :type filename: str
+    :param archive_in_repo: The path to the tar archive file.
+    :type archive_in_repo: str
     :param repo_type: The type of the Hugging Face repository, defaults to 'dataset'.
     :type repo_type: RepoTypeTyping, optional
     :param revision: The revision of the repository, defaults to 'main'.
     :type revision: str, optional
     :param idx_repo_id: The identifier of the index repository, defaults to None.
     :type idx_repo_id: str, optional
-    :param idx_filename: The path to save the index file in the index repository, defaults to None.
-    :type idx_filename: str, optional
+    :param idx_file_in_repo: The path to save the index file in the index repository, defaults to None.
+    :type idx_file_in_repo: str, optional
     :param idx_repo_type: The type of the index repository, defaults to None.
     :type idx_repo_type: RepoTypeTyping, optional
     :param idx_revision: The revision of the index repository, defaults to None.
     :type idx_revision: str, optional
     :param chunk_for_hash: The chunk size for hashing, defaults to 1 << 20 (1 MB).
     :type chunk_for_hash: int, optional
     :param with_hash: Whether to include file hashes in the index, defaults to True.
     :type with_hash: bool, optional
+    :param skip_when_synced: Skip syncing when index is ready, defaults to True.
+    :type skip_when_synced: bool
     :param hf_token: The Hugging Face access token, defaults to None.
     :type hf_token: str, optional
     """
+    body, _ = os.path.splitext(archive_in_repo)
+    default_index_filename = f'{body}.json'
+
+    from .validate import hf_tar_validate
+    if skip_when_synced and hf_tar_validate(
+            repo_id=repo_id,
+            repo_type=repo_type,
+            archive_in_repo=archive_in_repo,
+            revision=revision,
+
+            idx_repo_id=idx_repo_id or repo_id,
+            idx_repo_type=idx_repo_type or repo_type,
+            idx_file_in_repo=idx_file_in_repo or default_index_filename,
+            idx_revision=idx_revision or revision,
+
+            hf_token=hf_token,
+    ):
+        logging.info(f'Entry {repo_type}s/{repo_id}/{archive_in_repo} already indexed, skipped.')
+        return
+
     with TemporaryDirectory() as td:
-        local_tar_file = os.path.join(td, os.path.basename(filename))
+        local_tar_file = os.path.join(td, os.path.basename(archive_in_repo))
         download_file_to_file(
             repo_id=repo_id,
             repo_type=repo_type,
-            file_in_repo=filename,
+            file_in_repo=archive_in_repo,
             local_file=local_tar_file,
             revision=revision,
             hf_token=hf_token,
         )
         dst_index_file = tar_create_index(local_tar_file, chunk_for_hash=chunk_for_hash, with_hash=with_hash)
 
-        body, _ = os.path.splitext(filename)
-        default_index_filename = f'{body}.json'
         upload_file_to_file(
             repo_id=idx_repo_id or repo_id,
             repo_type=idx_repo_type or repo_type,
-            file_in_repo=idx_filename or default_index_filename,
+            file_in_repo=idx_file_in_repo or default_index_filename,
             local_file=dst_index_file,
             revision=idx_revision or revision,
             hf_token=hf_token,
-            message=f'Create index for {repo_type}s/{repo_id}@{revision}/{filename}',
+            message=f'Create index for {repo_type}s/{repo_id}@{revision}/{archive_in_repo}',
         )
 
 
 def hf_tar_create_from_directory(
         repo_id: str, archive_in_repo: str, local_directory: str,
         repo_type: RepoTypeTyping = 'dataset', revision: str = 'main',
         chunk_for_hash: int = 1 << 20, with_hash: bool = True,
```

### Comparing `hfutils-0.2.0/hfutils/operate/base.py` & `hfutils-0.2.1/hfutils/operate/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/operate/download.py` & `hfutils-0.2.1/hfutils/operate/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/operate/upload.py` & `hfutils-0.2.1/hfutils/operate/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/operate/validate.py` & `hfutils-0.2.1/hfutils/operate/validate.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/utils/binary.py` & `hfutils-0.2.1/hfutils/utils/binary.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/utils/download.py` & `hfutils-0.2.1/hfutils/utils/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/utils/temp.py` & `hfutils-0.2.1/hfutils/utils/temp.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/utils/tqdm_.py` & `hfutils-0.2.1/hfutils/utils/tqdm_.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils/utils/walk.py` & `hfutils-0.2.1/hfutils/utils/walk.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/hfutils.egg-info/PKG-INFO` & `hfutils-0.2.1/hfutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.2.0
+Version: 0.2.1
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hfutils-0.2.0/hfutils.egg-info/SOURCES.txt` & `hfutils-0.2.1/hfutils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 hfutils/entry/download.py
 hfutils/entry/ls.py
 hfutils/entry/upload.py
 hfutils/index/__init__.py
 hfutils/index/fetch.py
 hfutils/index/hash.py
 hfutils/index/make.py
+hfutils/index/validate.py
 hfutils/operate/__init__.py
 hfutils/operate/base.py
 hfutils/operate/download.py
 hfutils/operate/upload.py
 hfutils/operate/validate.py
 hfutils/utils/__init__.py
 hfutils/utils/binary.py
```

### Comparing `hfutils-0.2.0/hfutils.egg-info/requires.txt` & `hfutils-0.2.1/hfutils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.0/setup.py` & `hfutils-0.2.1/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/hfutils-0.1.2.tar.gz` & `tmp/hfutils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfutils-0.1.2.tar", last modified: Sat Apr 20 11:18:35 2024, max compression
+gzip compressed data, was "hfutils-0.2.0.tar", last modified: Sat Apr 20 18:02:02 2024, max compression
```

## Comparing `hfutils-0.1.2.tar` & `hfutils-0.2.0.tar`

### file list

```diff
@@ -1,53 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:35.254774 hfutils-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-20 11:18:15.000000 hfutils-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 11:18:15.000000 hfutils-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-20 11:18:35.254774 hfutils-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-20 11:18:15.000000 hfutils-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:35.246775 hfutils-0.1.2/hfutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:35.246775 hfutils-0.1.2/hfutils/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/archive/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/archive/rar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/archive/sevenz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/archive/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/archive/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:35.246775 hfutils-0.1.2/hfutils/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:35.246775 hfutils-0.1.2/hfutils/entry/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/entry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/entry/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/entry/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/entry/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/entry/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/entry/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:35.246775 hfutils-0.1.2/hfutils/operate/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/operate/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/operate/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/operate/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/operate/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:35.246775 hfutils-0.1.2/hfutils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/utils/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/utils/temp.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/utils/tqdm_.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-20 11:18:15.000000 hfutils-0.1.2/hfutils/utils/walk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:35.250774 hfutils-0.1.2/hfutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-20 11:18:35.000000 hfutils-0.1.2/hfutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-20 11:18:35.000000 hfutils-0.1.2/hfutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 11:18:35.000000 hfutils-0.1.2/hfutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-20 11:18:35.000000 hfutils-0.1.2/hfutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-20 11:18:35.000000 hfutils-0.1.2/hfutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 11:18:35.000000 hfutils-0.1.2/hfutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-20 11:18:15.000000 hfutils-0.1.2/requirements-7z.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-20 11:18:15.000000 hfutils-0.1.2/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-20 11:18:15.000000 hfutils-0.1.2/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 11:18:15.000000 hfutils-0.1.2/requirements-rar.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-20 11:18:15.000000 hfutils-0.1.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 11:18:15.000000 hfutils-0.1.2/requirements-transfer.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-20 11:18:15.000000 hfutils-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 11:18:35.254774 hfutils-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-20 11:18:15.000000 hfutils-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.849096 hfutils-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-20 18:01:44.000000 hfutils-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 18:01:44.000000 hfutils-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-04-20 18:02:02.849096 hfutils-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-04-20 18:01:44.000000 hfutils-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.841096 hfutils-0.2.0/hfutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.841096 hfutils-0.2.0/hfutils/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/archive/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/archive/rar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/archive/sevenz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/archive/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/archive/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.841096 hfutils-0.2.0/hfutils/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.841096 hfutils-0.2.0/hfutils/entry/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/entry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/entry/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/entry/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/entry/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/entry/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/entry/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/entry/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.841096 hfutils-0.2.0/hfutils/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/index/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/index/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/index/make.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.845096 hfutils-0.2.0/hfutils/operate/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/operate/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/operate/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/operate/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/operate/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.845096 hfutils-0.2.0/hfutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/utils/temp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/utils/tqdm_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-20 18:01:44.000000 hfutils-0.2.0/hfutils/utils/walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:02:02.845096 hfutils-0.2.0/hfutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-04-20 18:02:02.000000 hfutils-0.2.0/hfutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-20 18:02:02.000000 hfutils-0.2.0/hfutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:02:02.000000 hfutils-0.2.0/hfutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-20 18:02:02.000000 hfutils-0.2.0/hfutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-20 18:02:02.000000 hfutils-0.2.0/hfutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 18:02:02.000000 hfutils-0.2.0/hfutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-20 18:01:44.000000 hfutils-0.2.0/requirements-7z.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-20 18:01:44.000000 hfutils-0.2.0/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-20 18:01:44.000000 hfutils-0.2.0/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 18:01:44.000000 hfutils-0.2.0/requirements-rar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-20 18:01:44.000000 hfutils-0.2.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 18:01:44.000000 hfutils-0.2.0/requirements-transfer.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-20 18:01:44.000000 hfutils-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:02:02.849096 hfutils-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-20 18:01:44.000000 hfutils-0.2.0/setup.py
```

### Comparing `hfutils-0.1.2/LICENSE` & `hfutils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/PKG-INFO` & `hfutils-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.1.2
+Version: 0.2.0
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,18 +17,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hbutils>=0.9.0
-Requires-Dist: huggingface_hub>=0.20
+Requires-Dist: huggingface_hub>=0.22
 Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: click>=7
+Requires-Dist: tzlocal
 Provides-Extra: rar
 Requires-Dist: rarfile; extra == "rar"
 Provides-Extra: test
 Requires-Dist: coverage>=5; extra == "test"
 Requires-Dist: mock>=4.0.3; extra == "test"
 Requires-Dist: flake8~=3.5; extra == "test"
 Requires-Dist: testfixtures>=6.18.5; extra == "test"
@@ -225,14 +226,22 @@
 Explore additional options for downloading:
 
 ```shell
 hfutils download -h
 
 ```
 
+## List Files in Repository
+
+List files in repositories
+
+```shell
+hfutils ls -r your/repository -o /your/local/file -d subdir/in/repo
+```
+
 ## Supported Formats
 
 By default, we support the `zip` and `tar` formats, including `.zip`, `.tar`, `.tar.gz`, `.tar.bz2`, and `.tar.xz`.
 
 If you require support for `rar` and `7z` files, install the extra dependencies using the following command:
 
 ```shell
```

### Comparing `hfutils-0.1.2/README.md` & `hfutils-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,22 @@
 Explore additional options for downloading:
 
 ```shell
 hfutils download -h
 
 ```
 
+## List Files in Repository
+
+List files in repositories
+
+```shell
+hfutils ls -r your/repository -o /your/local/file -d subdir/in/repo
+```
+
 ## Supported Formats
 
 By default, we support the `zip` and `tar` formats, including `.zip`, `.tar`, `.tar.gz`, `.tar.bz2`, and `.tar.xz`.
 
 If you require support for `rar` and `7z` files, install the extra dependencies using the following command:
 
 ```shell
```

### Comparing `hfutils-0.1.2/hfutils/archive/__init__.py` & `hfutils-0.2.0/hfutils/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/archive/base.py` & `hfutils-0.2.0/hfutils/archive/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/archive/rar.py` & `hfutils-0.2.0/hfutils/archive/rar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/archive/sevenz.py` & `hfutils-0.2.0/hfutils/archive/sevenz.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/archive/tar.py` & `hfutils-0.2.0/hfutils/archive/tar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/archive/zip.py` & `hfutils-0.2.0/hfutils/archive/zip.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/entry/base.py` & `hfutils-0.2.0/hfutils/entry/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/entry/dispatch.py` & `hfutils-0.2.0/hfutils/entry/dispatch.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/entry/download.py` & `hfutils-0.2.0/hfutils/entry/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/entry/upload.py` & `hfutils-0.2.0/hfutils/entry/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/operate/base.py` & `hfutils-0.2.0/hfutils/operate/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/operate/download.py` & `hfutils-0.2.0/hfutils/operate/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/operate/upload.py` & `hfutils-0.2.0/hfutils/operate/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/operate/validate.py` & `hfutils-0.2.0/hfutils/operate/validate.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/utils/binary.py` & `hfutils-0.2.0/hfutils/utils/binary.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/utils/download.py` & `hfutils-0.2.0/hfutils/utils/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/utils/temp.py` & `hfutils-0.2.0/hfutils/utils/temp.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/utils/tqdm_.py` & `hfutils-0.2.0/hfutils/utils/tqdm_.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils/utils/walk.py` & `hfutils-0.2.0/hfutils/utils/walk.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.1.2/hfutils.egg-info/PKG-INFO` & `hfutils-0.2.0/hfutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.1.2
+Version: 0.2.0
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,18 +17,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hbutils>=0.9.0
-Requires-Dist: huggingface_hub>=0.20
+Requires-Dist: huggingface_hub>=0.22
 Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: click>=7
+Requires-Dist: tzlocal
 Provides-Extra: rar
 Requires-Dist: rarfile; extra == "rar"
 Provides-Extra: test
 Requires-Dist: coverage>=5; extra == "test"
 Requires-Dist: mock>=4.0.3; extra == "test"
 Requires-Dist: flake8~=3.5; extra == "test"
 Requires-Dist: testfixtures>=6.18.5; extra == "test"
@@ -225,14 +226,22 @@
 Explore additional options for downloading:
 
 ```shell
 hfutils download -h
 
 ```
 
+## List Files in Repository
+
+List files in repositories
+
+```shell
+hfutils ls -r your/repository -o /your/local/file -d subdir/in/repo
+```
+
 ## Supported Formats
 
 By default, we support the `zip` and `tar` formats, including `.zip`, `.tar`, `.tar.gz`, `.tar.bz2`, and `.tar.xz`.
 
 If you require support for `rar` and `7z` files, install the extra dependencies using the following command:
 
 ```shell
```

### Comparing `hfutils-0.1.2/hfutils.egg-info/SOURCES.txt` & `hfutils-0.2.0/hfutils.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,20 @@
 hfutils/config/__init__.py
 hfutils/config/meta.py
 hfutils/entry/__init__.py
 hfutils/entry/base.py
 hfutils/entry/cli.py
 hfutils/entry/dispatch.py
 hfutils/entry/download.py
+hfutils/entry/ls.py
 hfutils/entry/upload.py
+hfutils/index/__init__.py
+hfutils/index/fetch.py
+hfutils/index/hash.py
+hfutils/index/make.py
 hfutils/operate/__init__.py
 hfutils/operate/base.py
 hfutils/operate/download.py
 hfutils/operate/upload.py
 hfutils/operate/validate.py
 hfutils/utils/__init__.py
 hfutils/utils/binary.py
```

### Comparing `hfutils-0.1.2/hfutils.egg-info/requires.txt` & `hfutils-0.2.0/hfutils.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 hbutils>=0.9.0
-huggingface_hub>=0.20
+huggingface_hub>=0.22
 tqdm
 requests
 click>=7
+tzlocal
 
 [7z]
 py7zr
 
 [build]
 pyinstaller<5,>=4.7
```

### Comparing `hfutils-0.1.2/setup.py` & `hfutils-0.2.0/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/wall_e_models-0.8.tar.gz` & `tmp/wall_e_models-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wall_e_models-0.8.tar", last modified: Sat Oct 21 05:26:43 2023, max compression
+gzip compressed data, was "wall_e_models-0.9.tar", last modified: Mon Oct 30 19:25:04 2023, max compression
```

## Comparing `wall_e_models-0.8.tar` & `wall_e_models-0.9.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 jace      (1000) jace      (1000)        0 2023-10-21 05:26:43.183424 wall_e_models-0.8/
--rw-r--r--   0 jace      (1000) jace      (1000)    35149 2023-08-31 04:23:58.000000 wall_e_models-0.8/LICENSE
--rw-r--r--   0 jace      (1000) jace      (1000)       69 2023-08-31 05:41:16.000000 wall_e_models-0.8/MANIFEST.in
--rw-r--r--   0 jace      (1000) jace      (1000)     1409 2023-10-21 05:26:43.183424 wall_e_models-0.8/PKG-INFO
--rw-r--r--   0 jace      (1000) jace      (1000)      356 2023-08-31 19:59:00.000000 wall_e_models-0.8/README.rst
--rw-r--r--   0 jace      (1000) jace      (1000)        0 2023-08-31 04:26:46.000000 wall_e_models-0.8/__init__.py
--rw-r--r--   0 jace      (1000) jace      (1000)       80 2023-08-31 20:50:54.000000 wall_e_models-0.8/pyproject.toml
--rw-r--r--   0 jace      (1000) jace      (1000)      960 2023-10-21 05:26:43.183424 wall_e_models-0.8/setup.cfg
--rw-r--r--   0 jace      (1000) jace      (1000)       37 2023-08-31 04:41:52.000000 wall_e_models-0.8/setup.py
-drwxr-xr-x   0 jace      (1000) jace      (1000)        0 2023-10-21 05:26:43.179424 wall_e_models-0.8/wall_e_models/
--rw-r--r--   0 jace      (1000) jace      (1000)        0 2023-08-31 05:22:02.000000 wall_e_models-0.8/wall_e_models/__init__.py
-drwxr-xr-x   0 jace      (1000) jace      (1000)        0 2023-10-21 05:26:43.179424 wall_e_models-0.8/wall_e_models/__pycache__/
--rw-r--r--   0 jace      (1000) jace      (1000)      161 2023-08-31 06:29:52.000000 wall_e_models-0.8/wall_e_models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jace      (1000) jace      (1000)     1434 2023-08-31 06:37:45.000000 wall_e_models-0.8/wall_e_models/__pycache__/customFields.cpython-39.pyc
--rw-r--r--   0 jace      (1000) jace      (1000)    17631 2023-10-18 07:14:21.000000 wall_e_models-0.8/wall_e_models/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 jace      (1000) jace      (1000)     1945 2023-10-21 05:22:23.000000 wall_e_models-0.8/wall_e_models/customFields.py
-drwxr-xr-x   0 jace      (1000) jace      (1000)        0 2023-10-21 05:26:43.183424 wall_e_models-0.8/wall_e_models/migrations/
--rw-r--r--   0 jace      (1000) jace      (1000)     1367 2023-08-31 04:26:46.000000 wall_e_models-0.8/wall_e_models/migrations/0001_initial.py
--rw-r--r--   0 jace      (1000) jace      (1000)     2104 2023-08-31 06:43:57.000000 wall_e_models-0.8/wall_e_models/migrations/0002_auto_20220203_2111.py
--rw-r--r--   0 jace      (1000) jace      (1000)     1238 2023-08-31 06:44:05.000000 wall_e_models-0.8/wall_e_models/migrations/0003_auto_20220204_2003.py
--rw-r--r--   0 jace      (1000) jace      (1000)     1136 2023-08-31 20:42:40.000000 wall_e_models-0.8/wall_e_models/migrations/0004_auto_20220206_1142.py
--rw-r--r--   0 jace      (1000) jace      (1000)      475 2023-08-31 06:43:44.000000 wall_e_models-0.8/wall_e_models/migrations/0005_auto_20220715_1532.py
--rw-r--r--   0 jace      (1000) jace      (1000)      396 2023-08-31 06:43:34.000000 wall_e_models-0.8/wall_e_models/migrations/0006_auto_20220909_1633.py
--rw-r--r--   0 jace      (1000) jace      (1000)      985 2023-08-31 06:43:19.000000 wall_e_models-0.8/wall_e_models/migrations/0007_auto_20230827_1520.py
--rw-r--r--   0 jace      (1000) jace      (1000)      344 2023-08-31 10:12:56.000000 wall_e_models-0.8/wall_e_models/migrations/0008_rename_banrecords_banrecord.py
--rw-r--r--   0 jace      (1000) jace      (1000)      803 2023-09-25 21:54:45.000000 wall_e_models-0.8/wall_e_models/migrations/0009_helpmessage.py
--rw-r--r--   0 jace      (1000) jace      (1000)      619 2023-10-02 18:54:37.000000 wall_e_models-0.8/wall_e_models/migrations/0010_embedavatar.py
--rw-r--r--   0 jace      (1000) jace      (1000)        0 2023-08-31 04:26:46.000000 wall_e_models-0.8/wall_e_models/migrations/__init__.py
-drwxr-xr-x   0 jace      (1000) jace      (1000)        0 2023-10-21 05:26:43.183424 wall_e_models-0.8/wall_e_models/migrations/__pycache__/
--rw-r--r--   0 jace      (1000) jace      (1000)     1092 2023-08-31 06:35:30.000000 wall_e_models-0.8/wall_e_models/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-r--r--   0 jace      (1000) jace      (1000)     1372 2023-08-31 06:43:59.000000 wall_e_models-0.8/wall_e_models/migrations/__pycache__/0002_auto_20220203_2111.cpython-39.pyc
--rw-r--r--   0 jace      (1000) jace      (1000)      940 2023-08-31 06:44:07.000000 wall_e_models-0.8/wall_e_models/migrations/__pycache__/0003_auto_20220204_2003.cpython-39.pyc
--rw-r--r--   0 jace      (1000) jace      (1000)     1035 2023-08-31 22:57:46.000000 wall_e_models-0.8/wall_e_models/migrations/__pycache__/0004_auto_20220206_1142.cpython-39.pyc
--rw-r--r--   0 jace      (1000) jace      (1000)      687 2023-08-31 06:43:46.000000 wall_e_models-0.8/wall_e_models/migrations/__pycache__/0005_auto_20220715_1532.cpython-39.pyc
--rw-r--r--   0 jace      (1000) jace      (1000)      614 2023-08-31 06:43:35.000000 wall_e_models-0.8/wall_e_models/migrations/__pycache__/0006_auto_20220909_1633.cpython-39.pyc
--rw-r--r--   0 jace      (1000) jace      (1000)      821 2023-08-31 06:43:19.000000 wall_e_models-0.8/wall_e_models/migrations/__pycache__/0007_auto_20230827_1520.cpython-39.pyc
--rw-r--r--   0 jace      (1000) jace      (1000)      588 2023-08-31 06:39:04.000000 wall_e_models-0.8/wall_e_models/migrations/__pycache__/0008_rename_ban_id_banrecords_ban_d.cpython-39.pyc
--rw-r--r--   0 jace      (1000) jace      (1000)      565 2023-08-31 10:13:00.000000 wall_e_models-0.8/wall_e_models/migrations/__pycache__/0008_rename_banrecords_banrecord.cpython-39.pyc
--rw-r--r--   0 jace      (1000) jace      (1000)      860 2023-09-25 22:31:58.000000 wall_e_models-0.8/wall_e_models/migrations/__pycache__/0009_helpmessage.cpython-39.pyc
--rw-r--r--   0 jace      (1000) jace      (1000)      705 2023-09-25 19:56:01.000000 wall_e_models-0.8/wall_e_models/migrations/__pycache__/0010_auto_20230925_1253.cpython-39.pyc
--rw-r--r--   0 jace      (1000) jace      (1000)      757 2023-10-02 18:54:41.000000 wall_e_models-0.8/wall_e_models/migrations/__pycache__/0010_embedavatar.cpython-39.pyc
--rw-r--r--   0 jace      (1000) jace      (1000)      660 2023-09-25 19:56:41.000000 wall_e_models-0.8/wall_e_models/migrations/__pycache__/0011_alter_helpmessage_channel_name.cpython-39.pyc
--rw-r--r--   0 jace      (1000) jace      (1000)      172 2023-08-31 06:29:52.000000 wall_e_models-0.8/wall_e_models/migrations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jace      (1000) jace      (1000)    16655 2023-10-21 05:25:04.000000 wall_e_models-0.8/wall_e_models/models.py
-drwxr-xr-x   0 jace      (1000) jace      (1000)        0 2023-10-21 05:26:43.179424 wall_e_models-0.8/wall_e_models.egg-info/
--rw-r--r--   0 jace      (1000) jace      (1000)     1409 2023-10-21 05:26:43.000000 wall_e_models-0.8/wall_e_models.egg-info/PKG-INFO
--rw-r--r--   0 jace      (1000) jace      (1000)     2090 2023-10-21 05:26:43.000000 wall_e_models-0.8/wall_e_models.egg-info/SOURCES.txt
--rw-r--r--   0 jace      (1000) jace      (1000)        1 2023-10-21 05:26:43.000000 wall_e_models-0.8/wall_e_models.egg-info/dependency_links.txt
--rw-r--r--   0 jace      (1000) jace      (1000)       40 2023-10-21 05:26:43.000000 wall_e_models-0.8/wall_e_models.egg-info/requires.txt
--rw-r--r--   0 jace      (1000) jace      (1000)       14 2023-10-21 05:26:43.000000 wall_e_models-0.8/wall_e_models.egg-info/top_level.txt
+drwxr-xr-x   0 jace      (1000) jace      (1000)        0 2023-10-30 19:25:03.990399 wall_e_models-0.9/
+-rw-r--r--   0 jace      (1000) jace      (1000)    35149 2023-08-31 04:23:58.000000 wall_e_models-0.9/LICENSE
+-rw-r--r--   0 jace      (1000) jace      (1000)       69 2023-08-31 05:41:16.000000 wall_e_models-0.9/MANIFEST.in
+-rw-r--r--   0 jace      (1000) jace      (1000)     1409 2023-10-30 19:25:03.990399 wall_e_models-0.9/PKG-INFO
+-rw-r--r--   0 jace      (1000) jace      (1000)      356 2023-08-31 19:59:00.000000 wall_e_models-0.9/README.rst
+-rw-r--r--   0 jace      (1000) jace      (1000)        0 2023-08-31 04:26:46.000000 wall_e_models-0.9/__init__.py
+-rw-r--r--   0 jace      (1000) jace      (1000)       80 2023-08-31 20:50:54.000000 wall_e_models-0.9/pyproject.toml
+-rw-r--r--   0 jace      (1000) jace      (1000)      960 2023-10-30 19:25:03.994399 wall_e_models-0.9/setup.cfg
+-rw-r--r--   0 jace      (1000) jace      (1000)       37 2023-08-31 04:41:52.000000 wall_e_models-0.9/setup.py
+drwxr-xr-x   0 jace      (1000) jace      (1000)        0 2023-10-30 19:25:03.974400 wall_e_models-0.9/wall_e_models/
+-rw-r--r--   0 jace      (1000) jace      (1000)        0 2023-08-31 05:22:02.000000 wall_e_models-0.9/wall_e_models/__init__.py
+drwxr-xr-x   0 jace      (1000) jace      (1000)        0 2023-10-30 19:25:03.974400 wall_e_models-0.9/wall_e_models/__pycache__/
+-rw-r--r--   0 jace      (1000) jace      (1000)      161 2023-08-31 06:29:52.000000 wall_e_models-0.9/wall_e_models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)     1566 2023-10-30 19:23:07.000000 wall_e_models-0.9/wall_e_models/__pycache__/customFields.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)    17500 2023-10-30 19:23:07.000000 wall_e_models-0.9/wall_e_models/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)     2333 2023-10-30 19:15:35.000000 wall_e_models-0.9/wall_e_models/customFields.py
+drwxr-xr-x   0 jace      (1000) jace      (1000)        0 2023-10-30 19:25:03.982400 wall_e_models-0.9/wall_e_models/migrations/
+-rw-r--r--   0 jace      (1000) jace      (1000)     1367 2023-08-31 04:26:46.000000 wall_e_models-0.9/wall_e_models/migrations/0001_initial.py
+-rw-r--r--   0 jace      (1000) jace      (1000)     2104 2023-08-31 06:43:57.000000 wall_e_models-0.9/wall_e_models/migrations/0002_auto_20220203_2111.py
+-rw-r--r--   0 jace      (1000) jace      (1000)     1238 2023-08-31 06:44:05.000000 wall_e_models-0.9/wall_e_models/migrations/0003_auto_20220204_2003.py
+-rw-r--r--   0 jace      (1000) jace      (1000)     1136 2023-08-31 20:42:40.000000 wall_e_models-0.9/wall_e_models/migrations/0004_auto_20220206_1142.py
+-rw-r--r--   0 jace      (1000) jace      (1000)      475 2023-08-31 06:43:44.000000 wall_e_models-0.9/wall_e_models/migrations/0005_auto_20220715_1532.py
+-rw-r--r--   0 jace      (1000) jace      (1000)      396 2023-08-31 06:43:34.000000 wall_e_models-0.9/wall_e_models/migrations/0006_auto_20220909_1633.py
+-rw-r--r--   0 jace      (1000) jace      (1000)      985 2023-08-31 06:43:19.000000 wall_e_models-0.9/wall_e_models/migrations/0007_auto_20230827_1520.py
+-rw-r--r--   0 jace      (1000) jace      (1000)      344 2023-08-31 10:12:56.000000 wall_e_models-0.9/wall_e_models/migrations/0008_rename_banrecords_banrecord.py
+-rw-r--r--   0 jace      (1000) jace      (1000)      803 2023-09-25 21:54:45.000000 wall_e_models-0.9/wall_e_models/migrations/0009_helpmessage.py
+-rw-r--r--   0 jace      (1000) jace      (1000)      619 2023-10-02 18:54:37.000000 wall_e_models-0.9/wall_e_models/migrations/0010_embedavatar.py
+-rw-r--r--   0 jace      (1000) jace      (1000)        0 2023-08-31 04:26:46.000000 wall_e_models-0.9/wall_e_models/migrations/__init__.py
+drwxr-xr-x   0 jace      (1000) jace      (1000)        0 2023-10-30 19:25:03.990399 wall_e_models-0.9/wall_e_models/migrations/__pycache__/
+-rw-r--r--   0 jace      (1000) jace      (1000)     1092 2023-08-31 06:35:30.000000 wall_e_models-0.9/wall_e_models/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)     1372 2023-08-31 06:43:59.000000 wall_e_models-0.9/wall_e_models/migrations/__pycache__/0002_auto_20220203_2111.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)      940 2023-08-31 06:44:07.000000 wall_e_models-0.9/wall_e_models/migrations/__pycache__/0003_auto_20220204_2003.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)     1035 2023-08-31 22:57:46.000000 wall_e_models-0.9/wall_e_models/migrations/__pycache__/0004_auto_20220206_1142.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)      687 2023-08-31 06:43:46.000000 wall_e_models-0.9/wall_e_models/migrations/__pycache__/0005_auto_20220715_1532.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)      614 2023-08-31 06:43:35.000000 wall_e_models-0.9/wall_e_models/migrations/__pycache__/0006_auto_20220909_1633.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)      821 2023-08-31 06:43:19.000000 wall_e_models-0.9/wall_e_models/migrations/__pycache__/0007_auto_20230827_1520.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)      588 2023-08-31 06:39:04.000000 wall_e_models-0.9/wall_e_models/migrations/__pycache__/0008_rename_ban_id_banrecords_ban_d.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)      565 2023-08-31 10:13:00.000000 wall_e_models-0.9/wall_e_models/migrations/__pycache__/0008_rename_banrecords_banrecord.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)      860 2023-09-25 22:31:58.000000 wall_e_models-0.9/wall_e_models/migrations/__pycache__/0009_helpmessage.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)      705 2023-09-25 19:56:01.000000 wall_e_models-0.9/wall_e_models/migrations/__pycache__/0010_auto_20230925_1253.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)      757 2023-10-02 18:54:41.000000 wall_e_models-0.9/wall_e_models/migrations/__pycache__/0010_embedavatar.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)      660 2023-09-25 19:56:41.000000 wall_e_models-0.9/wall_e_models/migrations/__pycache__/0011_alter_helpmessage_channel_name.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)      693 2023-10-30 19:08:15.000000 wall_e_models-0.9/wall_e_models/migrations/__pycache__/0011_banrecord_unique_active_ban.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)      172 2023-08-31 06:29:52.000000 wall_e_models-0.9/wall_e_models/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jace      (1000) jace      (1000)    16655 2023-10-30 19:22:50.000000 wall_e_models-0.9/wall_e_models/models.py
+drwxr-xr-x   0 jace      (1000) jace      (1000)        0 2023-10-30 19:25:03.974400 wall_e_models-0.9/wall_e_models.egg-info/
+-rw-r--r--   0 jace      (1000) jace      (1000)     1409 2023-10-30 19:25:03.000000 wall_e_models-0.9/wall_e_models.egg-info/PKG-INFO
+-rw-r--r--   0 jace      (1000) jace      (1000)     2175 2023-10-30 19:25:03.000000 wall_e_models-0.9/wall_e_models.egg-info/SOURCES.txt
+-rw-r--r--   0 jace      (1000) jace      (1000)        1 2023-10-30 19:25:03.000000 wall_e_models-0.9/wall_e_models.egg-info/dependency_links.txt
+-rw-r--r--   0 jace      (1000) jace      (1000)       40 2023-10-30 19:25:03.000000 wall_e_models-0.9/wall_e_models.egg-info/requires.txt
+-rw-r--r--   0 jace      (1000) jace      (1000)       14 2023-10-30 19:25:03.000000 wall_e_models-0.9/wall_e_models.egg-info/top_level.txt
```

### Comparing `wall_e_models-0.8/LICENSE` & `wall_e_models-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/PKG-INFO` & `wall_e_models-0.9/wall_e_models.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
-Name: wall_e_models
-Version: 0.8
+Name: wall-e-models
+Version: 0.9
 Summary: A Django app to manage CSSS's discord bot's database
 Home-page: https://github.com/CSSS/wall_e_models
 Author: Jace Manshadi
 Author-email: jaymanshad@proton.me
 License: GNU General Public License v3.0
 Description: ===============
         wall_e_models
```

### Comparing `wall_e_models-0.8/setup.cfg` & `wall_e_models-0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wall_e_models
-version = 0.8
+version = 0.9
 url = https://github.com/CSSS/wall_e_models
 description = A Django app to manage CSSS's discord bot's database
 long_description = file: README.rst
 author = Jace Manshadi
 author_email = jaymanshad@proton.me
 license = GNU General Public License v3.0
 classifiers =
```

### Comparing `wall_e_models-0.8/wall_e_models/__pycache__/customFields.cpython-39.pyc` & `wall_e_models-0.9/wall_e_models/__pycache__/customFields.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Aug 31 06:37:43 2023 UTC, .py size: 1921 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,98 @@
-00000000: 610d 0d0a 0000 0000 3735 f064 8107 0000  a.......75.d....
+00000000: 610d 0d0a 0000 0000 d700 4065 1d09 0000  a.........@e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
+00000020: 0008 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6504 6503 6403 6404 8303  m.Z...e.e.d.d...
-00000050: 5a05 6504 6503 6405 6406 8303 5a06 4700  Z.e.e.d.d...Z.G.
-00000060: 6407 6408 8400 6408 6501 6a07 8303 5a08  d.d...d.e.j...Z.
-00000070: 6409 5300 290a e900 0000 0029 01da 066d  d.S.)......)...m
-00000080: 6f64 656c 7329 01da 0873 6574 7469 6e67  odels)...setting
-00000090: 735a 0b45 4e56 4952 4f4e 4d45 4e54 5a09  sZ.ENVIRONMENTZ.
-000000a0: 4c4f 4341 4c48 4f53 54da 0c50 4f53 5447  LOCALHOST..POSTG
-000000b0: 5245 535f 5351 4c46 6300 0000 0000 0000  RES_SQLFc.......
-000000c0: 0000 0000 0000 0000 0003 0000 0000 0000  ................
-000000d0: 0073 3400 0000 6500 5a01 6400 5a02 6401  .s4...e.Z.d.Z.d.
-000000e0: 5a03 8700 6601 6402 6403 8408 5a04 8700  Z...f.d.d...Z...
-000000f0: 6601 6404 6405 8408 5a05 6406 6407 8400  f.d.d...Z.d.d...
-00000100: 5a06 8700 0400 5a07 5300 2908 da16 4765  Z.....Z.S.)...Ge
-00000110: 6e65 7261 7465 6449 6465 6e74 6974 7946  neratedIdentityF
-00000120: 6965 6c64 7a98 416e 2049 6e74 6567 6572  ieldz.An Integer
-00000130: 2063 6f6c 756d 6e20 7768 6963 6820 7573   column which us
-00000140: 6573 2060 4745 4e45 5241 5445 4420 7b41  es `GENERATED {A
-00000150: 4c57 4159 5320 7c20 4259 2044 4546 4155  LWAYS | BY DEFAU
-00000160: 4c54 7d20 4153 2049 4445 4e54 4954 5960  LT} AS IDENTITY`
-00000170: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-00000180: 2020 2020 4120 6d6f 6465 726e 2061 6c74      A modern alt
-00000190: 6572 6e61 7469 7665 2074 6f20 6042 4947  ernative to `BIG
-000001a0: 5345 5249 414c 6020 6672 6f6d 2074 6865  SERIAL` from the
-000001b0: 2053 514c 2073 7461 6e64 6172 642e 6301   SQL standard.c.
-000001c0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-000001d0: 0000 000f 0000 0073 3000 0000 7c02 a000  .......s0...|...
-000001e0: 6401 6400 a102 0100 7401 6402 6b02 7c00  d.d.....t.d.k.|.
-000001f0: 5f02 7403 7404 7c00 8302 6a05 7c01 6900  _.t.t.|...j.|.i.
-00000200: 7c02 a401 8e01 0100 6400 5300 2903 4eda  |.......d.S.).N.
-00000210: 0661 6c77 6179 735a 0a50 524f 4455 4354  .alwaysZ.PRODUCT
-00000220: 494f 4e29 06da 0370 6f70 da03 454e 5672  ION)...pop..ENVr
-00000230: 0600 0000 da05 7375 7065 7272 0500 0000  ......superr....
-00000240: da08 5f5f 696e 6974 5f5f 2903 da04 7365  ..__init__)...se
-00000250: 6c66 da04 6172 6773 da06 6b77 6172 6773  lf..args..kwargs
-00000260: a901 da09 5f5f 636c 6173 735f 5fa9 00fa  ....__class__...
-00000270: 4a2f 6d65 6469 612f 6a61 6365 2f6a 6163  J/media/jace/jac
-00000280: 655f 646f 6373 2f31 5f43 5353 532f 325f  e_docs/1_CSSS/2_
-00000290: 7761 6c6c 5f65 5f6d 6f64 656c 732f 7761  wall_e_models/wa
-000002a0: 6c6c 5f65 5f6d 6f64 656c 732f 6375 7374  ll_e_models/cust
-000002b0: 6f6d 4669 656c 6473 2e70 7972 0a00 0000  omFields.pyr....
-000002c0: 0c00 0000 7306 0000 0000 030c 060a 027a  ....s..........z
-000002d0: 1f47 656e 6572 6174 6564 4964 656e 7469  .GeneratedIdenti
-000002e0: 7479 4669 656c 642e 5f5f 696e 6974 5f5f  tyField.__init__
-000002f0: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
-00000300: 0004 0000 0003 0000 0073 2800 0000 7400  .........s(...t.
-00000310: 8300 a001 a100 5c04 7d01 7d02 7d03 7d04  ......\.}.}.}.}.
-00000320: 7c00 6a02 7c04 6401 3c00 7c01 7c02 7c03  |.j.|.d.<.|.|.|.
-00000330: 7c04 6604 5300 2902 4e72 0600 0000 2903  |.f.S.).Nr....).
-00000340: 7209 0000 00da 0b64 6563 6f6e 7374 7275  r......deconstru
-00000350: 6374 7206 0000 0029 0572 0b00 0000 da04  ctr....).r......
-00000360: 6e61 6d65 da04 7061 7468 720c 0000 0072  name..pathr....r
-00000370: 0d00 0000 720e 0000 0072 1000 0000 7211  ....r....r....r.
-00000380: 0000 0072 1200 0000 1900 0000 7306 0000  ...r........s...
-00000390: 0000 0112 010a 017a 2247 656e 6572 6174  .......z"Generat
-000003a0: 6564 4964 656e 7469 7479 4669 656c 642e  edIdentityField.
-000003b0: 6465 636f 6e73 7472 7563 7463 0200 0000  deconstructc....
-000003c0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-000003d0: 4300 0000 7322 0000 0074 0072 1a64 017c  C...s"...t.r.d.|
-000003e0: 006a 0172 1064 026e 0264 039b 0064 049d  .j.r.d.n.d...d..
-000003f0: 0353 0064 0553 0064 0053 0029 064e 7a12  .S.d.S.d.S.).Nz.
-00000400: 494e 5445 4745 5220 4745 4e45 5241 5445  INTEGER GENERATE
-00000410: 4420 5a06 414c 5741 5953 7a0a 4259 2044  D Z.ALWAYSz.BY D
-00000420: 4546 4155 4c54 7a0c 2041 5320 4944 454e  EFAULTz. AS IDEN
-00000430: 5449 5459 5a07 494e 5445 4745 5229 0272  TITYZ.INTEGER).r
-00000440: 0400 0000 7206 0000 0029 0272 0b00 0000  ....r....).r....
-00000450: da0a 636f 6e6e 6563 7469 6f6e 7210 0000  ..connectionr...
-00000460: 0072 1000 0000 7211 0000 00da 0764 625f  .r....r......db_
-00000470: 7479 7065 1e00 0000 7306 0000 0000 0104  type....s.......
-00000480: 0116 087a 1e47 656e 6572 6174 6564 4964  ...z.GeneratedId
-00000490: 656e 7469 7479 4669 656c 642e 6462 5f74  entityField.db_t
-000004a0: 7970 6529 08da 085f 5f6e 616d 655f 5fda  ype)...__name__.
-000004b0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000004c0: 7561 6c6e 616d 655f 5fda 0b64 6573 6372  ualname__..descr
-000004d0: 6970 7469 6f6e 720a 0000 0072 1200 0000  iptionr....r....
-000004e0: 7216 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
-000004f0: 6c6c 5f5f 7210 0000 0072 1000 0000 720e  ll__r....r....r.
-00000500: 0000 0072 1100 0000 7205 0000 0008 0000  ...r....r.......
-00000510: 0073 0800 0000 0801 0403 0c0d 0c05 7205  .s............r.
-00000520: 0000 004e 2909 da09 646a 616e 676f 2e64  ...N)...django.d
-00000530: 6272 0200 0000 da0b 646a 616e 676f 2e63  br......django.c
-00000540: 6f6e 6672 0300 0000 da07 6765 7461 7474  onfr......getatt
-00000550: 7272 0800 0000 7204 0000 00da 0941 7574  rr....r......Aut
-00000560: 6f46 6965 6c64 7205 0000 0072 1000 0000  oFieldr....r....
-00000570: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
-00000580: 083c 6d6f 6475 6c65 3e01 0000 0073 0800  .<module>....s..
-00000590: 0000 0c01 0c02 0c01 0c03                 ..........
+00000050: 5a05 6504 6503 6405 6406 8303 5a06 7a24  Z.e.e.d.d...Z.z$
+00000060: 6400 6407 6c07 5a07 6504 6507 6403 6404  d.d.l.Z.e.e.d.d.
+00000070: 8303 5a05 6504 6507 6405 6406 8303 5a06  ..Z.e.e.d.d...Z.
+00000080: 5700 6e12 0400 6508 7966 0100 0100 0100  W.n...e.yf......
+00000090: 5900 6e02 3000 4700 6408 6409 8400 6409  Y.n.0.G.d.d...d.
+000000a0: 6501 6a09 8303 5a0a 6407 5300 290a e900  e.j...Z.d.S.)...
+000000b0: 0000 0029 01da 066d 6f64 656c 7329 01da  ...)...models)..
+000000c0: 0873 6574 7469 6e67 735a 0b45 4e56 4952  .settingsZ.ENVIR
+000000d0: 4f4e 4d45 4e54 5a09 4c4f 4341 4c48 4f53  ONMENTZ.LOCALHOS
+000000e0: 54da 0d64 6174 6162 6173 655f 7479 7065  T..database_type
+000000f0: 5a07 7371 6c69 7465 334e 6300 0000 0000  Z.sqlite3Nc.....
+00000100: 0000 0000 0000 0000 0000 0003 0000 0000  ................
+00000110: 0000 0073 3400 0000 6500 5a01 6400 5a02  ...s4...e.Z.d.Z.
+00000120: 6401 5a03 8700 6601 6402 6403 8408 5a04  d.Z...f.d.d...Z.
+00000130: 8700 6601 6404 6405 8408 5a05 6406 6407  ..f.d.d...Z.d.d.
+00000140: 8400 5a06 8700 0400 5a07 5300 2908 da16  ..Z.....Z.S.)...
+00000150: 4765 6e65 7261 7465 6449 6465 6e74 6974  GeneratedIdentit
+00000160: 7946 6965 6c64 7a98 416e 2049 6e74 6567  yFieldz.An Integ
+00000170: 6572 2063 6f6c 756d 6e20 7768 6963 6820  er column which 
+00000180: 7573 6573 2060 4745 4e45 5241 5445 4420  uses `GENERATED 
+00000190: 7b41 4c57 4159 5320 7c20 4259 2044 4546  {ALWAYS | BY DEF
+000001a0: 4155 4c54 7d20 4153 2049 4445 4e54 4954  AULT} AS IDENTIT
+000001b0: 5960 2e20 2020 2020 2020 2020 2020 2020  Y`.             
+000001c0: 2020 2020 2020 4120 6d6f 6465 726e 2061        A modern a
+000001d0: 6c74 6572 6e61 7469 7665 2074 6f20 6042  lternative to `B
+000001e0: 4947 5345 5249 414c 6020 6672 6f6d 2074  IGSERIAL` from t
+000001f0: 6865 2053 514c 2073 7461 6e64 6172 642e  he SQL standard.
+00000200: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00000210: 0004 0000 000f 0000 0073 3000 0000 7c02  .........s0...|.
+00000220: a000 6401 6400 a102 0100 7401 6402 6b02  ..d.d.....t.d.k.
+00000230: 7c00 5f02 7403 7404 7c00 8302 6a05 7c01  |._.t.t.|...j.|.
+00000240: 6900 7c02 a401 8e01 0100 6400 5300 2903  i.|.......d.S.).
+00000250: 4eda 0661 6c77 6179 735a 0a50 524f 4455  N..alwaysZ.PRODU
+00000260: 4354 494f 4e29 06da 0370 6f70 da03 454e  CTION)...pop..EN
+00000270: 5672 0600 0000 da05 7375 7065 7272 0500  Vr......superr..
+00000280: 0000 da08 5f5f 696e 6974 5f5f 2903 da04  ....__init__)...
+00000290: 7365 6c66 da04 6172 6773 da06 6b77 6172  self..args..kwar
+000002a0: 6773 a901 da09 5f5f 636c 6173 735f 5fa9  gs....__class__.
+000002b0: 00fa 4a2f 6d65 6469 612f 6a61 6365 2f6a  ..J/media/jace/j
+000002c0: 6163 655f 646f 6373 2f31 5f43 5353 532f  ace_docs/1_CSSS/
+000002d0: 325f 7761 6c6c 5f65 5f6d 6f64 656c 732f  2_wall_e_models/
+000002e0: 7761 6c6c 5f65 5f6d 6f64 656c 732f 6375  wall_e_models/cu
+000002f0: 7374 6f6d 4669 656c 6473 2e70 7972 0a00  stomFields.pyr..
+00000300: 0000 1500 0000 7306 0000 0000 030c 060a  ......s.........
+00000310: 027a 1f47 656e 6572 6174 6564 4964 656e  .z.GeneratedIden
+00000320: 7469 7479 4669 656c 642e 5f5f 696e 6974  tityField.__init
+00000330: 5f5f 6301 0000 0000 0000 0000 0000 0005  __c.............
+00000340: 0000 0004 0000 0003 0000 0073 2800 0000  ...........s(...
+00000350: 7400 8300 a001 a100 5c04 7d01 7d02 7d03  t.......\.}.}.}.
+00000360: 7d04 7c00 6a02 7c04 6401 3c00 7c01 7c02  }.|.j.|.d.<.|.|.
+00000370: 7c03 7c04 6604 5300 2902 4e72 0600 0000  |.|.f.S.).Nr....
+00000380: 2903 7209 0000 00da 0b64 6563 6f6e 7374  ).r......deconst
+00000390: 7275 6374 7206 0000 0029 0572 0b00 0000  ructr....).r....
+000003a0: da04 6e61 6d65 da04 7061 7468 720c 0000  ..name..pathr...
+000003b0: 0072 0d00 0000 720e 0000 0072 1000 0000  .r....r....r....
+000003c0: 7211 0000 0072 1200 0000 2200 0000 7306  r....r...."...s.
+000003d0: 0000 0000 0112 010a 017a 2247 656e 6572  .........z"Gener
+000003e0: 6174 6564 4964 656e 7469 7479 4669 656c  atedIdentityFiel
+000003f0: 642e 6465 636f 6e73 7472 7563 7463 0200  d.deconstructc..
+00000400: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00000410: 0000 4300 0000 7326 0000 0074 0064 016b  ..C...s&...t.d.k
+00000420: 0272 1e64 027c 006a 0172 1464 036e 0264  .r.d.|.j.r.d.n.d
+00000430: 049b 0064 059d 0353 0064 0653 0064 0053  ...d...S.d.S.d.S
+00000440: 0029 074e 5a0b 706f 7374 6772 6573 5351  .).NZ.postgresSQ
+00000450: 4c7a 1249 4e54 4547 4552 2047 454e 4552  Lz.INTEGER GENER
+00000460: 4154 4544 205a 0641 4c57 4159 537a 0a42  ATED Z.ALWAYSz.B
+00000470: 5920 4445 4641 554c 547a 0c20 4153 2049  Y DEFAULTz. AS I
+00000480: 4445 4e54 4954 595a 0749 4e54 4547 4552  DENTITYZ.INTEGER
+00000490: 2902 7204 0000 0072 0600 0000 2902 720b  ).r....r....).r.
+000004a0: 0000 00da 0a63 6f6e 6e65 6374 696f 6e72  .....connectionr
+000004b0: 1000 0000 7210 0000 0072 1100 0000 da07  ....r....r......
+000004c0: 6462 5f74 7970 6527 0000 0073 0600 0000  db_type'...s....
+000004d0: 0001 0801 1608 7a1e 4765 6e65 7261 7465  ......z.Generate
+000004e0: 6449 6465 6e74 6974 7946 6965 6c64 2e64  dIdentityField.d
+000004f0: 625f 7479 7065 2908 da08 5f5f 6e61 6d65  b_type)...__name
+00000500: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000510: 5f5f 7175 616c 6e61 6d65 5f5f da0b 6465  __qualname__..de
+00000520: 7363 7269 7074 696f 6e72 0a00 0000 7212  scriptionr....r.
+00000530: 0000 0072 1600 0000 da0d 5f5f 636c 6173  ...r......__clas
+00000540: 7363 656c 6c5f 5f72 1000 0000 7210 0000  scell__r....r...
+00000550: 0072 0e00 0000 7211 0000 0072 0500 0000  .r....r....r....
+00000560: 1100 0000 7308 0000 0008 0104 030c 0d0c  ....s...........
+00000570: 0572 0500 0000 290b da09 646a 616e 676f  .r....)...django
+00000580: 2e64 6272 0200 0000 da0b 646a 616e 676f  .dbr......django
+00000590: 2e63 6f6e 6672 0300 0000 da07 6765 7461  .confr......geta
+000005a0: 7474 7272 0800 0000 7204 0000 00da 0f64  ttrr....r......d
+000005b0: 6a61 6e67 6f5f 7365 7474 696e 6773 da13  jango_settings..
+000005c0: 4d6f 6475 6c65 4e6f 7446 6f75 6e64 4572  ModuleNotFoundEr
+000005d0: 726f 72da 0941 7574 6f46 6965 6c64 7205  ror..AutoFieldr.
+000005e0: 0000 0072 1000 0000 7210 0000 0072 1000  ...r....r....r..
+000005f0: 0000 7211 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000600: 3e01 0000 0073 1400 0000 0c01 0c02 0c01  >....s..........
+00000610: 0c02 0203 0801 0c01 1001 0c01 0603       ..............
```

### Comparing `wall_e_models-0.8/wall_e_models/__pycache__/models.cpython-39.pyc` & `wall_e_models-0.9/wall_e_models/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Oct 18 06:56:08 2023 UTC, .py size: 16712 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8881 2f65 4841 0000  a........./eHA..
+00000000: 610d 0d0a 0000 0000 8a02 4065 0f41 0000  a.........@e.A..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 2c01 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a04 6400  m.Z...d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6400 6403 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c07 5a07 6400 6404 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6400 6405 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
@@ -26,15 +26,15 @@
 00000190: 7474 696e 6773 2901 da06 6d6f 6465 6c73  ttings)...models
 000001a0: 2901 da0d 6d6f 6465 6c5f 746f 5f64 6963  )...model_to_dic
 000001b0: 7429 01da 0874 696d 657a 6f6e 65a9 01da  t)...timezone...
 000001c0: 0274 7a7a 0e43 616e 6164 612f 5061 6369  .tzz.Canada/Paci
 000001d0: 6669 63e9 0100 0000 2901 da16 4765 6e65  fic.....)...Gene
 000001e0: 7261 7465 6449 6465 6e74 6974 7946 6965  ratedIdentityFie
 000001f0: 6c64 6300 0000 0000 0000 0000 0000 0000  ldc.............
-00000200: 0000 0005 0000 0040 0000 0173 3a01 0000  .......@...s:...
+00000200: 0000 0005 0000 0040 0000 0173 2e01 0000  .......@...s....
 00000210: 6500 5a01 6400 5a02 6503 6401 6402 8d01  e.Z.d.Z.e.d.d...
 00000220: 5a04 6505 6a06 6403 6404 6405 8d02 5a07  Z.e.j.d.d.d...Z.
 00000230: 6505 6a08 6404 6406 8d01 5a09 6505 6a06  e.j.d.d...Z.e.j.
 00000240: 6403 6401 6405 8d02 5a0a 6505 6a08 6401  d.d.d...Z.e.j.d.
 00000250: 6406 8d01 5a0b 6505 6a08 6401 6406 8d01  d...Z.e.j.d.d...
 00000260: 5a0c 6505 6a06 6407 6404 6405 8d02 5a0d  Z.e.j.d.d.d...Z.
 00000270: 6505 6a08 6401 6408 6409 8d02 5a0e 4700  e.j.d.d.d...Z.G.
@@ -45,1058 +45,1050 @@
 000002c0: 6414 6415 9c01 6416 6417 8404 8301 8301  d.d...d.d.......
 000002d0: 5a14 6510 6511 640c 6415 9c01 6418 6419  Z.e.e.d.d...d.d.
 000002e0: 8404 8301 8301 5a15 6510 6511 641a 6415  ......Z.e.e.d.d.
 000002f0: 9c01 641b 641c 8404 8301 8301 5a16 6510  ..d.d.......Z.e.
 00000300: 6511 641a 641d 641e 9c02 641f 6420 8404  e.d.d.d...d.d ..
 00000310: 8301 8301 5a17 6510 6511 6421 6415 9c01  ....Z.e.e.d!d...
 00000320: 6422 6423 8404 8301 8301 5a18 641d 6415  d"d#......Z.d.d.
-00000330: 9c01 6424 6425 8404 5a19 6510 6426 6427  ..d$d%..Z.e.d&d'
-00000340: 8400 8301 5a1a 6408 5300 2928 da09 4261  ....Z.d.S.)(..Ba
-00000350: 6e52 6563 6f72 6454 a901 da0b 7072 696d  nRecordT....prim
-00000360: 6172 795f 6b65 79e9 2500 0000 4629 02da  ary_key.%...F)..
-00000370: 0a6d 6178 5f6c 656e 6774 68da 046e 756c  .max_length..nul
-00000380: 6ca9 0172 1200 0000 6900 0200 004e 2902  l..r....i....N).
-00000390: 7212 0000 00da 0764 6566 6175 6c74 6300  r......defaultc.
-000003a0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-000003b0: 0000 0040 0000 0173 1000 0000 6500 5a01  ...@...s....e.Z.
-000003c0: 6400 5a02 6401 5a03 6402 5300 2903 7a0e  d.Z.d.Z.d.S.).z.
-000003d0: 4261 6e52 6563 6f72 642e 4d65 7461 5a19  BanRecord.MetaZ.
-000003e0: 7761 6c6c 5f65 5f6d 6f64 656c 735f 6261  wall_e_models_ba
-000003f0: 6e5f 7265 636f 7264 734e 2904 da08 5f5f  n_recordsN)...__
-00000400: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000410: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000420: da08 6462 5f74 6162 6c65 a900 7219 0000  ..db_table..r...
-00000430: 0072 1900 0000 fa44 2f6d 6564 6961 2f6a  .r.....D/media/j
-00000440: 6163 652f 6a61 6365 5f64 6f63 732f 315f  ace/jace_docs/1_
-00000450: 4353 5353 2f32 5f77 616c 6c5f 652f 7761  CSSS/2_wall_e/wa
-00000460: 6c6c 5f65 2f77 616c 6c5f 655f 6d6f 6465  ll_e/wall_e_mode
-00000470: 6c73 2f6d 6f64 656c 732e 7079 da04 4d65  ls/models.py..Me
-00000480: 7461 2300 0000 7302 0000 0008 0172 1b00  ta#...s......r..
-00000490: 0000 7a0f 4c69 7374 5b42 616e 5265 636f  ..z.List[BanReco
-000004a0: 7264 5dda 044e 6f6e 6529 02da 0772 6563  rd]..None)...rec
-000004b0: 6f72 6473 da06 7265 7475 726e 6302 0000  ords..returnc...
-000004c0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-000004d0: 0043 0000 0173 1000 0000 7400 6a01 a002  .C...s....t.j...
-000004e0: 7c01 a101 0100 6401 5300 a902 7a1d 4164  |.....d.S...z.Ad
-000004f0: 6473 2065 6e74 7279 2074 6f20 4261 6e52  ds entry to BanR
-00000500: 6563 6f72 6420 7461 626c 654e 2903 720d  ecord tableN).r.
-00000510: 0000 00da 076f 626a 6563 7473 da0b 6275  .....objects..bu
-00000520: 6c6b 5f63 7265 6174 6529 02da 0363 6c73  lk_create)...cls
-00000530: 721d 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-00000540: 1a00 0000 da0e 696e 7365 7274 5f72 6563  ......insert_rec
-00000550: 6f72 6473 2600 0000 7302 0000 0000 047a  ords&...s......z
-00000560: 1842 616e 5265 636f 7264 2e69 6e73 6572  .BanRecord.inser
-00000570: 745f 7265 636f 7264 73a9 02da 0672 6563  t_records....rec
-00000580: 6f72 6472 1e00 0000 6302 0000 0000 0000  ordr....c.......
-00000590: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-000005a0: 0173 0c00 0000 7c01 a000 a100 0100 6401  .s....|.......d.
-000005b0: 5300 721f 0000 00a9 01da 0473 6176 65a9  S.r........save.
-000005c0: 0272 2200 0000 7225 0000 0072 1900 0000  .r"...r%...r....
-000005d0: 7219 0000 0072 1a00 0000 da0d 696e 7365  r....r......inse
-000005e0: 7274 5f72 6563 6f72 642c 0000 0073 0200  rt_record,...s..
-000005f0: 0000 0004 7a17 4261 6e52 6563 6f72 642e  ....z.BanRecord.
-00000600: 696e 7365 7274 5f72 6563 6f72 647a 094c  insert_recordz.L
-00000610: 6973 745b 696e 745d 2901 721e 0000 0063  ist[int]).r....c
-00000620: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000630: 0500 0000 4300 0001 731c 0000 0074 0074  ....C...s....t.t
-00000640: 016a 026a 0364 0164 0264 038d 026a 0464  .j.j.d.d.d...j.d
-00000650: 0464 058d 0183 0153 0029 067a 3752 6574  .d.....S.).z7Ret
-00000660: 7572 6e73 206c 6973 7420 6f66 2075 7365  urns list of use
-00000670: 725f 6964 7320 666f 7220 616c 6c20 6375  r_ids for all cu
-00000680: 7272 656e 746c 7920 6261 6e6e 6564 2075  rrently banned u
-00000690: 7365 7273 da07 7573 6572 5f69 6454 2901  sers..user_idT).
-000006a0: da04 666c 6174 4ea9 01da 0a75 6e62 616e  ..flatN....unban
-000006b0: 5f64 6174 6529 05da 046c 6973 7472 0d00  _date)...listr..
-000006c0: 0000 7220 0000 00da 0b76 616c 7565 735f  ..r .....values_
-000006d0: 6c69 7374 da06 6669 6c74 6572 a901 7222  list..filter..r"
-000006e0: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-000006f0: 0000 da1b 6765 745f 616c 6c5f 6163 7469  ....get_all_acti
-00000700: 7665 5f62 616e 5f75 7365 725f 6964 7332  ve_ban_user_ids2
-00000710: 0000 0073 0200 0000 0005 7a25 4261 6e52  ...s......z%BanR
-00000720: 6563 6f72 642e 6765 745f 616c 6c5f 6163  ecord.get_all_ac
-00000730: 7469 7665 5f62 616e 5f75 7365 725f 6964  tive_ban_user_id
-00000740: 7363 0100 0000 0000 0000 0000 0000 0100  sc..............
-00000750: 0000 0500 0000 4300 0001 731a 0000 0074  ......C...s....t
-00000760: 0074 016a 02a0 0364 0164 02a1 026a 0464  .t.j...d.d...j.d
-00000770: 0364 048d 0183 0153 0029 057a 4552 6574  .d.....S.).zERet
-00000780: 7572 6e73 206c 6973 7420 6f66 2075 7365  urns list of use
-00000790: 726e 616d 6573 2061 6e64 2075 7365 725f  rnames and user_
-000007a0: 6964 7320 666f 7220 616c 6c20 6375 7272  ids for all curr
-000007b0: 656e 746c 7920 6261 6e6e 6564 2075 7365  ently banned use
-000007c0: 7273 da08 7573 6572 6e61 6d65 722a 0000  rs..usernamer*..
-000007d0: 004e 722c 0000 0029 0572 2e00 0000 720d  .Nr,...).r....r.
-000007e0: 0000 0072 2000 0000 da06 7661 6c75 6573  ...r .....values
-000007f0: 7230 0000 0072 3100 0000 7219 0000 0072  r0...r1...r....r
-00000800: 1900 0000 721a 0000 00da 1367 6574 5f61  ....r......get_a
-00000810: 6c6c 5f61 6374 6976 655f 6261 6e73 3900  ll_active_bans9.
-00000820: 0000 7302 0000 0000 057a 1d42 616e 5265  ..s......z.BanRe
-00000830: 636f 7264 2e67 6574 5f61 6c6c 5f61 6374  cord.get_all_act
-00000840: 6976 655f 6261 6e73 da03 696e 7463 0100  ive_bans..intc..
-00000850: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00000860: 0000 4300 0001 7312 0000 0074 006a 016a  ..C...s....t.j.j
-00000870: 0264 0164 028d 01a0 03a1 0053 0029 037a  .d.d.......S.).z
-00000880: 2452 6574 7572 6e73 2063 6f75 6e74 206f  $Returns count o
-00000890: 6620 616c 6c20 7468 6520 6163 7469 7665  f all the active
-000008a0: 2062 616e 734e 722c 0000 0029 0472 0d00   bansNr,...).r..
-000008b0: 0000 7220 0000 0072 3000 0000 da05 636f  ..r ...r0.....co
-000008c0: 756e 7472 3100 0000 7219 0000 0072 1900  untr1...r....r..
-000008d0: 0000 721a 0000 00da 1567 6574 5f61 6374  ..r......get_act
-000008e0: 6976 655f 6261 6e73 5f63 6f75 6e74 4000  ive_bans_count@.
-000008f0: 0000 7302 0000 0000 057a 1f42 616e 5265  ..s......z.BanRe
-00000900: 636f 7264 2e67 6574 5f61 6374 6976 655f  cord.get_active_
-00000910: 6261 6e73 5f63 6f75 6e74 da03 7374 7229  bans_count..str)
-00000920: 0272 2a00 0000 721e 0000 0063 0200 0000  .r*...r....c....
-00000930: 0000 0000 0000 0000 0300 0000 0800 0000  ................
-00000940: 4300 0001 7348 0000 007a 1474 006a 016a  C...sH...z.t.j.j
-00000950: 027c 0164 0164 028d 027d 0257 006e 1404  .|.d.d...}.W.n..
-00000960: 0074 0379 2801 0001 0001 0059 0064 0153  .t.y(......Y.d.S
-00000970: 0030 0074 046a 04a0 05a1 00a0 06a1 007c  .0.t.j.........|
-00000980: 025f 077c 02a0 08a1 0001 007c 026a 0953  ._.|.......|.j.S
-00000990: 0029 037a 5453 6574 2061 6374 6976 653d  .).zTSet active=
-000009a0: 4661 6c73 6520 666f 7220 7573 6572 2077  False for user w
-000009b0: 6974 6820 7468 6520 6769 7665 6e20 7573  ith the given us
-000009c0: 6572 5f69 642e 2054 6869 7320 7265 7072  er_id. This repr
-000009d0: 6573 656e 7465 7320 756e 6261 6e6e 696e  esentes unbannin
-000009e0: 6720 6120 7573 6572 2e4e 2902 722a 0000  g a user.N).r*..
-000009f0: 0072 2d00 0000 290a 720d 0000 0072 2000  .r-...).r....r .
-00000a00: 0000 da03 6765 74da 0945 7863 6570 7469  ....get..Excepti
-00000a10: 6f6e da08 6461 7465 7469 6d65 da03 6e6f  on..datetime..no
-00000a20: 77da 0974 696d 6573 7461 6d70 722d 0000  w..timestampr-..
-00000a30: 0072 2700 0000 7233 0000 0029 0372 2200  .r'...r3...).r".
-00000a40: 0000 722a 0000 00da 0475 7365 7272 1900  ..r*.....userr..
-00000a50: 0000 7219 0000 0072 1a00 0000 da0b 756e  ..r....r......un
-00000a60: 6261 6e5f 6279 5f69 6447 0000 0073 0e00  ban_by_idG...s..
-00000a70: 0000 0004 0201 1401 0c01 0802 1001 0801  ................
-00000a80: 7a15 4261 6e52 6563 6f72 642e 756e 6261  z.BanRecord.unba
-00000a90: 6e5f 6279 5f69 64da 0462 6f6f 6c63 0200  n_by_id..boolc..
-00000aa0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00000ab0: 0000 4300 0001 731a 0000 0074 006a 01a0  ..C...s....t.j..
-00000ac0: 02a1 006a 037c 0164 018d 01a0 04a1 0064  ...j.|.d.......d
-00000ad0: 0075 0153 0029 024e a901 722a 0000 0029  .u.S.).N..r*...)
-00000ae0: 0572 0d00 0000 7220 0000 00da 0361 6c6c  .r....r .....all
-00000af0: 7230 0000 00da 0566 6972 7374 2902 7222  r0.....first).r"
-00000b00: 0000 0072 2a00 0000 7219 0000 0072 1900  ...r*...r....r..
-00000b10: 0000 721a 0000 00da 0e75 7365 725f 6973  ..r......user_is
-00000b20: 5f62 616e 6e65 6454 0000 0073 0200 0000  _bannedT...s....
-00000b30: 0003 7a18 4261 6e52 6563 6f72 642e 7573  ..z.BanRecord.us
-00000b40: 6572 5f69 735f 6261 6e6e 6564 6301 0000  er_is_bannedc...
-00000b50: 0000 0000 0000 0000 0001 0000 0011 0000  ................
-00000b60: 0043 0000 0173 4600 0000 6401 7c00 6a00  .C...sF...d.|.j.
-00000b70: 9b00 6402 7c00 6a01 9b00 6403 7c00 6a02  ..d.|.j...d.|.j.
-00000b80: 9b00 6404 7c00 6a03 9b00 6405 7c00 6a04  ..d.|.j...d.|.j.
-00000b90: 9b00 6406 7c00 6a05 9b00 6407 7c00 6a06  ..d.|.j...d.|.j.
-00000ba0: 9b00 6408 7c00 6a07 9b00 6409 9d11 5300  ..d.|.j...d...S.
-00000bb0: 290a 4e7a 0862 616e 5f69 643d 5b7a 0c5d  ).Nz.ban_id=[z.]
-00000bc0: 2075 7365 726e 616d 653d 5b7a 0b5d 2075   username=[z.] u
-00000bd0: 7365 725f 6964 3d5b 7a07 5d20 6d6f 643d  ser_id=[z.] mod=
-00000be0: 5b7a 0a5d 206d 6f64 5f69 643d 5b7a 085d  [z.] mod_id=[z.]
-00000bf0: 2064 6174 653d 5b7a 0a5d 2072 6561 736f   date=[z.] reaso
-00000c00: 6e3d 5b7a 0d5d 756e 6261 6e5f 6461 7465  n=[z.]unban_date
-00000c10: 3d5b fa01 5d29 08da 0662 616e 5f69 6472  =[..])...ban_idr
-00000c20: 3300 0000 722a 0000 00da 036d 6f64 da06  3...r*.....mod..
-00000c30: 6d6f 645f 6964 da08 6261 6e5f 6461 7465  mod_id..ban_date
-00000c40: da06 7265 6173 6f6e 722d 0000 00a9 01da  ..reasonr-......
-00000c50: 0473 656c 6672 1900 0000 7219 0000 0072  .selfr....r....r
-00000c60: 1a00 0000 da07 5f5f 7374 725f 5f59 0000  ......__str__Y..
-00000c70: 0073 1600 0000 0001 1a01 04ff 0401 04ff  .s..............
-00000c80: 0401 04ff 0401 04ff 0402 04fe 7a11 4261  ............z.Ba
-00000c90: 6e52 6563 6f72 642e 5f5f 7374 725f 5f63  nRecord.__str__c
-00000ca0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000cb0: 0100 0000 4300 0001 7304 0000 0064 0053  ....C...s....d.S
-00000cc0: 00a9 014e 7219 0000 0029 0272 2200 0000  ...Nr....).r"...
-00000cd0: da02 6964 7219 0000 0072 1900 0000 721a  ..idr....r....r.
-00000ce0: 0000 00da 0763 6f63 6169 6e65 5e00 0000  .....cocaine^...
-00000cf0: 7302 0000 0000 027a 1142 616e 5265 636f  s......z.BanReco
-00000d00: 7264 2e63 6f63 6169 6e65 291b 7215 0000  rd.cocaine).r...
-00000d10: 0072 1600 0000 7217 0000 0072 0c00 0000  .r....r....r....
-00000d20: 7247 0000 0072 0600 0000 da09 4368 6172  rG...r......Char
-00000d30: 4669 656c 6472 3300 0000 da0f 4269 6749  Fieldr3.....BigI
-00000d40: 6e74 6567 6572 4669 656c 6472 2a00 0000  ntegerFieldr*...
-00000d50: 7248 0000 0072 4900 0000 724a 0000 0072  rH...rI...rJ...r
-00000d60: 4b00 0000 722d 0000 0072 1b00 0000 da0b  K...r-...r......
-00000d70: 636c 6173 736d 6574 686f 6472 0400 0000  classmethodr....
-00000d80: 7223 0000 0072 2900 0000 7232 0000 0072  r#...r)...r2...r
-00000d90: 3500 0000 7238 0000 0072 4000 0000 7245  5...r8...r@...rE
-00000da0: 0000 0072 4e00 0000 7251 0000 0072 1900  ...rN...rQ...r..
-00000db0: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00000dc0: 0072 0d00 0000 1900 0000 7342 0000 0008  .r........sB....
-00000dd0: 010a 010e 010c 010e 010c 010c 010e 010e  ................
-00000de0: 020e 0302 0102 0114 0402 0102 0114 0402  ................
-00000df0: 0102 0112 0502 0102 0112 0502 0102 0112  ................
-00000e00: 0502 0102 0114 0b02 0102 0112 030e 0502  ................
-00000e10: 0172 0d00 0000 6300 0000 0000 0000 0000  .r....c.........
-00000e20: 0000 0000 0000 0005 0000 0000 0000 0173  ...............s
-00000e30: d800 0000 6500 5a01 6400 5a02 6503 6a04  ....e.Z.d.Z.e.j.
-00000e40: 6401 6402 8d01 5a05 6503 6a06 6507 6a08  d.d...Z.e.j.e.j.
-00000e50: 6403 8d01 5a09 6503 6a06 6507 6a08 6403  d...Z.e.j.e.j.d.
-00000e60: 8d01 5a0a 6503 6a06 6507 6a08 6403 8d01  ..Z.e.j.e.j.d...
-00000e70: 5a0b 6503 6a06 6507 6a08 6403 8d01 5a0c  Z.e.j.e.j.d...Z.
-00000e80: 6503 6a0d 6404 6405 6406 8d02 5a0e 6503  e.j.d.d.d...Z.e.
-00000e90: 6a0d 6404 6407 8d01 5a0f 6503 6a0d 6404  j.d.d...Z.e.j.d.
-00000ea0: 6407 8d01 5a10 6503 6a0d 6404 6401 6401  d...Z.e.j.d.d.d.
-00000eb0: 6408 8d03 5a11 6512 6409 640a 8400 8301  d...Z.e.d.d.....
-00000ec0: 5a13 6512 6514 640b 640c 8400 8301 8301  Z.e.e.d.d.......
-00000ed0: 5a15 6512 6514 640d 640e 8400 8301 8301  Z.e.e.d.d.......
-00000ee0: 5a16 6512 6416 6410 6411 8401 8301 5a17  Z.e.d.d.d.....Z.
-00000ef0: 6412 6413 8400 5a18 8700 6601 6414 6415  d.d...Z...f.d.d.
-00000f00: 8408 5a19 8700 0400 5a1a 5300 2917 da0b  ..Z.....Z.S.)...
-00000f10: 436f 6d6d 616e 6453 7461 7454 720e 0000  CommandStatTr...
-00000f20: 00a9 0172 1400 0000 e9d0 0700 00da 024e  ...r...........N
-00000f30: 41a9 0272 1100 0000 7214 0000 00a9 0172  A..r....r......r
-00000f40: 1100 0000 2903 7211 0000 00da 0562 6c61  ....).r......bla
-00000f50: 6e6b 7212 0000 0063 0100 0000 0000 0000  nkr....c........
-00000f60: 0000 0000 0100 0000 0300 0000 4300 0001  ............C...
-00000f70: 7312 0000 0064 0164 0284 0074 0074 0183  s....d.d...t.t..
-00000f80: 0144 0083 0153 0029 034e 6301 0000 0000  .D...S.).Nc.....
-00000f90: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-00000fa0: 0000 0173 1800 0000 6700 7c00 5d10 7d01  ...s....g.|.].}.
-00000fb0: 7c01 6400 6b03 7204 7c01 9102 7104 5300  |.d.k.r.|...q.S.
-00000fc0: 2901 da0a 6570 6f63 685f 7469 6d65 7219  )...epoch_timer.
-00000fd0: 0000 0029 02da 022e 30da 036b 6579 7219  ...)....0..keyr.
-00000fe0: 0000 0072 1900 0000 721a 0000 00da 0a3c  ...r....r......<
-00000ff0: 6c69 7374 636f 6d70 3e84 0000 00f3 0000  listcomp>.......
-00001000: 0000 7a40 436f 6d6d 616e 6453 7461 742e  ..z@CommandStat.
-00001010: 6765 745f 636f 6c75 6d6e 5f68 6561 6465  get_column_heade
-00001020: 7273 5f66 726f 6d5f 6461 7461 6261 7365  rs_from_database
-00001030: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00001040: 6f6d 703e 2902 7207 0000 0072 5500 0000  omp>).r....rU...
-00001050: 7231 0000 0072 1900 0000 7219 0000 0072  r1...r....r....r
-00001060: 1a00 0000 da20 6765 745f 636f 6c75 6d6e  ..... get_column
-00001070: 5f68 6561 6465 7273 5f66 726f 6d5f 6461  _headers_from_da
-00001080: 7461 6261 7365 8200 0000 7302 0000 0000  tabase....s.....
-00001090: 027a 2c43 6f6d 6d61 6e64 5374 6174 2e67  .z,CommandStat.g
-000010a0: 6574 5f63 6f6c 756d 6e5f 6865 6164 6572  et_column_header
-000010b0: 735f 6672 6f6d 5f64 6174 6162 6173 6563  s_from_databasec
-000010c0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000010d0: 0300 0000 4300 0001 730e 0000 0074 0074  ....C...s....t.t
-000010e0: 016a 02a0 03a1 0083 0153 0072 4f00 0000  .j.......S.rO...
-000010f0: 2904 722e 0000 0072 5500 0000 7220 0000  ).r....rU...r ..
-00001100: 0072 4300 0000 7231 0000 0072 1900 0000  .rC...r1...r....
-00001110: 7219 0000 0072 1a00 0000 da0f 6765 745f  r....r......get_
-00001120: 616c 6c5f 656e 7472 6965 7386 0000 0073  all_entries....s
-00001130: 0200 0000 0003 7a1b 436f 6d6d 616e 6453  ......z.CommandS
-00001140: 7461 742e 6765 745f 616c 6c5f 656e 7472  tat.get_all_entr
-00001150: 6965 7363 0200 0000 0000 0000 0000 0000  iesc............
-00001160: 0200 0000 0800 0000 4300 0001 7336 0000  ........C...s6..
-00001170: 007a 0e7c 01a0 00a1 0001 0057 0064 0053  .z.|.......W.d.S
-00001180: 0004 0074 0179 2e01 0001 0001 007c 0104  ...t.y.......|..
-00001190: 006a 0264 0137 0002 005f 0259 0071 0030  .j.d.7..._.Y.q.0
-000011a0: 0071 0064 0053 00a9 024e 720b 0000 0029  .q.d.S...Nr....)
-000011b0: 0372 2700 0000 723b 0000 0072 5c00 0000  .r'...r;...r\...
-000011c0: 2902 7222 0000 00da 0c63 6f6d 6d61 6e64  ).r".....command
-000011d0: 5f73 7461 7472 1900 0000 7219 0000 0072  _statr....r....r
-000011e0: 1a00 0000 da11 7361 7665 5f63 6f6d 6d61  ......save_comma
-000011f0: 6e64 5f73 7461 748b 0000 0073 0a00 0000  nd_stat....s....
-00001200: 0004 0201 0801 0601 0c01 7a1d 436f 6d6d  ..........z.Comm
-00001210: 616e 6453 7461 742e 7361 7665 5f63 6f6d  andStat.save_com
-00001220: 6d61 6e64 5f73 7461 744e 6302 0000 0000  mand_statNc.....
-00001230: 0000 0000 0000 0007 0000 0005 0000 00c3  ................
-00001240: 0000 0173 7400 0000 6900 7d02 7400 a001  ...st...i.}.t...
-00001250: a100 4900 6400 4800 4400 5d5c 7d03 7402  ..I.d.H.D.]\}.t.
-00001260: 7c03 8301 7d03 6401 7d04 7403 7c01 8301  |...}.d.}.t.|...
-00001270: 4400 5d2e 5c02 7d05 7d06 7c04 7c03 7c06  D.].\.}.}.|.|.|.
-00001280: 1900 9b00 3700 7d04 7c05 6402 1700 7404  ....7.}.|.d...t.
-00001290: 7c01 8301 6b00 722a 7c04 6403 3700 7d04  |...k.r*|.d.7.}.
-000012a0: 712a 7c02 a005 7c04 6404 a102 6402 1700  q*|...|.d...d...
-000012b0: 7c02 7c04 3c00 7112 7c02 5300 2905 4eda  |.|.<.q.|.S.).N.
-000012c0: 0072 0b00 0000 fa01 2d72 0100 0000 2906  .r......-r....).
-000012d0: 7255 0000 0072 6200 0000 7207 0000 00da  rU...rb...r.....
-000012e0: 0965 6e75 6d65 7261 7465 da03 6c65 6e72  .enumerate..lenr
-000012f0: 3a00 0000 2907 7222 0000 00da 0766 696c  :...).r".....fil
-00001300: 7465 7273 5a11 6669 6c74 6572 5f73 7461  tersZ.filter_sta
-00001310: 7473 5f64 6963 7472 6400 0000 725e 0000  ts_dictrd...r^..
-00001320: 00da 0369 6478 5a0e 636f 6d6d 616e 645f  ...idxZ.command_
-00001330: 6669 6c74 6572 7219 0000 0072 1900 0000  filterr....r....
-00001340: 721a 0000 00da 1667 6574 5f63 6f6d 6d61  r......get_comma
-00001350: 6e64 5f73 7461 7473 5f64 6963 7495 0000  nd_stats_dict...
-00001360: 0073 1400 0000 0002 0401 1201 0801 0401  .s..............
-00001370: 1001 0e01 1001 0a01 1601 7a22 436f 6d6d  ..........z"Comm
-00001380: 616e 6453 7461 742e 6765 745f 636f 6d6d  andStat.get_comm
-00001390: 616e 645f 7374 6174 735f 6469 6374 6301  and_stats_dictc.
-000013a0: 0000 0000 0000 0000 0000 0001 0000 000d  ................
-000013b0: 0000 0043 0000 0173 3a00 0000 7c00 6a00  ...C...s:...|.j.
-000013c0: 9b00 6401 7c00 6a01 9b00 6402 7c00 6a02  ..d.|.j...d.|.j.
-000013d0: 9b00 6403 7c00 6a03 9b00 6404 7c00 6a04  ..d.|.j...d.|.j.
-000013e0: 9b00 6405 7c00 6a05 9b00 6406 7c00 6a06  ..d.|.j...d.|.j.
-000013f0: 9b00 9d0d 5300 2907 4e7a 0320 2d20 7a11  ....S.).Nz. - z.
-00001400: 2061 7320 696e 766f 6b65 6420 7769 7468   as invoked with
-00001410: 207a 1120 7769 7468 2073 7562 636f 6d6d   z. with subcomm
-00001420: 616e 6420 7a0a 2061 6e64 2079 6561 7220  and z. and year 
-00001430: 7a08 2c20 6d6f 6e74 6820 7a0a 2061 6e64  z., month z. and
-00001440: 2068 6f75 7220 2907 725c 0000 00da 0763   hour ).r\.....c
-00001450: 6f6d 6d61 6e64 da0c 696e 766f 6b65 645f  ommand..invoked_
-00001460: 7769 7468 da12 696e 766f 6b65 645f 7375  with..invoked_su
-00001470: 6263 6f6d 6d61 6e64 da04 7965 6172 da05  bcommand..year..
-00001480: 6d6f 6e74 68da 0468 6f75 7272 4c00 0000  month..hourrL...
-00001490: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-000014a0: 4e00 0000 a200 0000 7314 0000 0000 0218  N.......s.......
-000014b0: 0104 ff04 0104 ff04 0204 fe04 0204 fe04  ................
-000014c0: ff7a 1343 6f6d 6d61 6e64 5374 6174 2e5f  .z.CommandStat._
-000014d0: 5f73 7472 5f5f 6301 0000 0000 0000 0000  _str__c.........
-000014e0: 0000 0003 0000 0004 0000 000f 0000 0173  ...............s
-000014f0: 8200 0000 7400 7c00 6a01 8301 7402 6a02  ....t.|.j...t.j.
-00001500: 6b02 721a 7c00 6a01 6a01 7c00 5f01 7400  k.r.|.j.j.|._.t.
-00001510: 7c00 6a03 8301 7402 6a02 6b02 7234 7c00  |.j...t.j.k.r4|.
-00001520: 6a03 6a03 7c00 5f03 7400 7c00 6a04 8301  j.j.|._.t.|.j...
-00001530: 7402 6a02 6b02 724e 7c00 6a04 6a04 7c00  t.j.k.rN|.j.j.|.
-00001540: 5f04 7400 7c00 6a05 8301 7402 6a02 6b02  _.t.|.j...t.j.k.
-00001550: 7268 7c00 6a05 6a05 7c00 5f05 7406 7407  rh|.j.j.|._.t.t.
-00001560: 7c00 8302 6a08 7c01 6900 7c02 a401 8e01  |...j.|.i.|.....
-00001570: 0100 6400 5300 724f 0000 0029 09da 0474  ..d.S.rO...)...t
-00001580: 7970 6572 7000 0000 723c 0000 0072 7100  yperp...r<...rq.
-00001590: 0000 da03 6461 7972 7200 0000 da05 7375  ....dayrr.....su
-000015a0: 7065 7272 5500 0000 7227 0000 00a9 0372  perrU...r'.....r
-000015b0: 4d00 0000 da04 6172 6773 da06 6b77 6172  M.....args..kwar
-000015c0: 6773 a901 da09 5f5f 636c 6173 735f 5f72  gs....__class__r
-000015d0: 1900 0000 721a 0000 0072 2700 0000 a800  ....r....r'.....
-000015e0: 0000 7312 0000 0000 0110 010a 0110 010a  ..s.............
-000015f0: 0110 010a 0110 010a 017a 1043 6f6d 6d61  .........z.Comma
-00001600: 6e64 5374 6174 2e73 6176 6529 014e 291b  ndStat.save).N).
-00001610: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00001620: 0600 0000 da0c 4269 6741 7574 6f46 6965  ......BigAutoFie
-00001630: 6c64 725c 0000 00da 0c49 6e74 6567 6572  ldr\.....Integer
-00001640: 4669 656c 6472 0800 0000 723d 0000 0072  Fieldr....r=...r
-00001650: 7000 0000 7271 0000 0072 7400 0000 7272  p...rq...rt...rr
-00001660: 0000 0072 5200 0000 da0c 6368 616e 6e65  ...rR.....channe
-00001670: 6c5f 6e61 6d65 726d 0000 0072 6e00 0000  l_namerm...rn...
-00001680: 726f 0000 0072 5400 0000 7261 0000 0072  ro...rT...ra...r
-00001690: 0400 0000 7262 0000 0072 6500 0000 726c  ....rb...re...rl
-000016a0: 0000 0072 4e00 0000 7227 0000 00da 0d5f  ...rN...r'....._
-000016b0: 5f63 6c61 7373 6365 6c6c 5f5f 7219 0000  _classcell__r...
-000016c0: 0072 1900 0000 7279 0000 0072 1a00 0000  .r....ry...r....
-000016d0: 7255 0000 0063 0000 0073 5200 0000 0801  rU...c...sR.....
-000016e0: 0401 02ff 0603 0401 04ff 0603 0401 04ff  ................
-000016f0: 0603 0401 04ff 0603 0401 04ff 0603 0401  ................
-00001700: 0201 02fe 0604 0401 02ff 0603 0401 02ff  ................
-00001710: 0603 0401 0201 04fe 0605 0201 0a03 0201  ................
-00001720: 0201 0c03 0201 0201 0c08 0201 0c0c 0806  ................
-00001730: 7255 0000 0063 0000 0000 0000 0000 0000  rU...c..........
-00001740: 0000 0000 0000 0600 0000 4000 0001 7310  ..........@...s.
-00001750: 0100 0065 005a 0164 005a 0265 036a 0464  ...e.Z.d.Z.e.j.d
-00001760: 0164 028d 015a 0565 03a0 04a1 005a 0665  .d...Z.e.....Z.e
-00001770: 03a0 04a1 005a 0765 03a0 04a1 005a 0865  .....Z.e.....Z.e
-00001780: 036a 0964 0364 048d 015a 0a65 03a0 04a1  .j.d.d...Z.e....
-00001790: 005a 0b65 036a 0c64 0564 048d 015a 0d65  .Z.e.j.d.d...Z.e
-000017a0: 0e64 0664 0784 0083 015a 0f65 1065 0e65  .d.d.....Z.e.e.e
-000017b0: 11a0 1264 0864 09a1 0264 0a65 136a 13a0  ...d.d...d.e.j..
-000017c0: 14a1 0064 0366 0464 0b64 0c84 0183 0183  ...d.f.d.d......
-000017d0: 015a 1565 1664 0d64 0e84 0083 015a 1765  .Z.e.d.d.....Z.e
-000017e0: 0e64 0f64 1084 0083 015a 1865 0e64 1164  .d.d.....Z.e.d.d
-000017f0: 1284 0083 015a 1965 0e64 1364 1484 0083  .....Z.e.d.d....
-00001800: 015a 1a65 0e64 1564 1684 0083 015a 1b65  .Z.e.d.d.....Z.e
-00001810: 0e64 1764 1884 0083 015a 1c65 1065 0e64  .d.d.....Z.e.e.d
-00001820: 1964 1a84 0083 0183 015a 1d65 1065 0e64  .d.......Z.e.e.d
-00001830: 1b64 1c84 0083 0183 015a 1e64 1d64 1e84  .d.......Z.d.d..
-00001840: 005a 1f65 2064 1f64 2084 0083 015a 2165  .Z.e d.d ....Z!e
-00001850: 1065 0e64 2164 2284 0083 0183 015a 2264  .e.d!d"......Z"d
-00001860: 2353 0029 24da 0955 7365 7250 6f69 6e74  #S.)$..UserPoint
-00001870: 54a9 01da 0675 6e69 7175 6572 0100 0000  T....uniquer....
-00001880: 7256 0000 0046 6301 0000 0000 0000 0000  rV...Fc.........
-00001890: 0000 0001 0000 0002 0000 0043 0000 0173  ...........C...s
-000018a0: 0c00 0000 7c00 a000 a100 0100 6400 5300  ....|.......d.S.
-000018b0: 724f 0000 0072 2600 0000 724c 0000 0072  rO...r&...rL...r
-000018c0: 1900 0000 7219 0000 0072 1a00 0000 da0a  ....r....r......
-000018d0: 6173 796e 635f 7361 7665 cb00 0000 7302  async_save....s.
-000018e0: 0000 0000 027a 1455 7365 7250 6f69 6e74  .....z.UserPoint
-000018f0: 2e61 7379 6e63 5f73 6176 65e9 0f00 0000  .async_save.....
-00001900: e919 0000 0072 0b00 0000 6305 0000 0000  .....r....c.....
-00001910: 0000 0000 0000 0006 0000 0008 0000 0043  ...............C
-00001920: 0000 0173 2a00 0000 7400 7c00 7c01 7400  ...s*...t.|.|.t.
-00001930: a001 7c01 a101 7c02 7c03 a002 a100 7c04  ..|...|.|.....|.
-00001940: 6401 8d06 7d05 7c05 a003 a100 0100 7c05  d...}.|.......|.
-00001950: 5300 2902 4e29 0672 2a00 0000 da06 706f  S.).N).r*.....po
-00001960: 696e 7473 da18 6c65 7665 6c5f 7570 5f73  ints..level_up_s
-00001970: 7065 6369 6669 635f 706f 696e 7473 da0d  pecific_points..
-00001980: 6d65 7373 6167 655f 636f 756e 74da 1f6c  message_count..l
-00001990: 6174 6573 745f 7469 6d65 5f78 705f 7761  atest_time_xp_wa
-000019a0: 735f 6561 726e 6564 5f65 706f 6368 da0c  s_earned_epoch..
-000019b0: 6c65 7665 6c5f 6e75 6d62 6572 2904 727f  level_number).r.
-000019c0: 0000 00da 2263 616c 6375 6c61 7465 5f6c  ...."calculate_l
-000019d0: 6576 656c 5f75 705f 7370 6563 6966 6963  evel_up_specific
-000019e0: 5f70 6f69 6e74 7372 3e00 0000 7227 0000  _pointsr>...r'..
-000019f0: 0029 0672 2a00 0000 7285 0000 0072 8700  .).r*...r....r..
-00001a00: 0000 5a19 6c61 7465 7374 5f74 696d 655f  ..Z.latest_time_
-00001a10: 7870 5f77 6173 5f65 6172 6e65 64da 056c  xp_was_earned..l
-00001a20: 6576 656c da0a 7573 6572 5f70 6f69 6e74  evel..user_point
-00001a30: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-00001a40: 1163 7265 6174 655f 7573 6572 5f70 6f69  .create_user_poi
-00001a50: 6e74 cf00 0000 7310 0000 0000 0502 0104  nt....s.........
-00001a60: 0108 0102 0108 fc06 0608 017a 1b55 7365  ...........z.Use
-00001a70: 7250 6f69 6e74 2e63 7265 6174 655f 7573  rPoint.create_us
-00001a80: 6572 5f70 6f69 6e74 6302 0000 0000 0000  er_pointc.......
-00001a90: 0000 0000 0004 0000 0003 0000 0043 0000  .............C..
-00001aa0: 0173 4a00 0000 6401 7d02 7400 6a01 a002  .sJ...d.}.t.j...
-00001ab0: a100 a003 6402 a101 7d03 7c03 7c02 1900  ....d...}.|.|...
-00001ac0: 6a04 7c01 6b00 7246 7c02 7405 7c03 8301  j.|.k.rF|.t.|...
-00001ad0: 6b00 7246 7c01 7c03 7c02 1900 6a04 3800  k.rF|.|.|...j.8.
-00001ae0: 7d01 7c02 6403 3700 7d02 7114 7c01 5300  }.|.d.7.}.q.|.S.
-00001af0: 2904 4e72 0100 0000 da15 746f 7461 6c5f  ).Nr......total_
-00001b00: 706f 696e 7473 5f72 6571 7569 7265 6472  points_requiredr
-00001b10: 0b00 0000 2906 da05 4c65 7665 6c72 2000  ....)...Levelr .
-00001b20: 0000 7243 0000 00da 086f 7264 6572 5f62  ..rC.....order_b
-00001b30: 79da 2378 705f 6e65 6564 6564 5f74 6f5f  y.#xp_needed_to_
-00001b40: 6c65 7665 6c5f 7570 5f74 6f5f 6e65 7874  level_up_to_next
-00001b50: 5f6c 6576 656c 7269 0000 0029 0472 2200  _levelri...).r".
-00001b60: 0000 7285 0000 005a 0469 6e64 785a 066c  ..r....Z.indxZ.l
-00001b70: 6576 656c 7372 1900 0000 7219 0000 0072  evelsr....r....r
-00001b80: 1a00 0000 728a 0000 00dd 0000 0073 0c00  ....r........s..
-00001b90: 0000 0002 0401 1001 1a01 0e01 0a02 7a2c  ..............z,
-00001ba0: 5573 6572 506f 696e 742e 6361 6c63 756c  UserPoint.calcul
-00001bb0: 6174 655f 6c65 7665 6c5f 7570 5f73 7065  ate_level_up_spe
-00001bc0: 6369 6669 635f 706f 696e 7473 6301 0000  cific_pointsc...
-00001bd0: 0000 0000 0000 0000 0004 0000 0004 0000  ................
-00001be0: 0043 0000 0173 a600 0000 6401 7d01 7c00  .C...s....d.}.|.
-00001bf0: a000 a100 72a2 7401 a002 6402 6403 a102  ....r.t...d.d...
-00001c00: 7d02 7c00 0400 6a03 7c02 3700 0200 5f03  }.|...j.|.7..._.
-00001c10: 7c00 0400 6a04 7c02 3700 0200 5f04 7c00  |...j.|.7..._.|.
-00001c20: 0400 6a05 6404 3700 0200 5f05 7c00 6a06  ..j.d.7..._.|.j.
-00001c30: 6405 6b00 728a 7407 6a08 6a09 7c00 6a06  d.k.r.t.j.j.|.j.
-00001c40: 6406 8d01 7d03 7c00 6a04 7c03 6a0a 6b05  d...}.|.j.|.j.k.
-00001c50: 728a 7c00 0400 6a04 7c03 6a0a 3800 0200  r.|...j.|.j.8...
-00001c60: 5f04 7c00 0400 6a06 6404 3700 0200 5f06  _.|...j.d.7..._.
-00001c70: 6407 7d01 740b 6a0b a00c a100 a00d a100  d.}.t.j.........
-00001c80: 7c00 5f0e 7c00 a00f a100 0100 7c01 5300  |._.|.......|.S.
-00001c90: 2908 4e46 7283 0000 0072 8400 0000 720b  ).NFr....r....r.
-00001ca0: 0000 00e9 6400 0000 a901 da06 6e75 6d62  ....d.......numb
-00001cb0: 6572 5429 10da 1d6d 6573 7361 6765 5f63  erT)...message_c
-00001cc0: 6f75 6e74 735f 746f 7761 7264 735f 706f  ounts_towards_po
-00001cd0: 696e 7473 da06 7261 6e64 6f6d da07 7261  ints..random..ra
-00001ce0: 6e64 696e 7472 8500 0000 7286 0000 0072  ndintr....r....r
-00001cf0: 8700 0000 7289 0000 0072 8f00 0000 7220  ....r....r....r 
-00001d00: 0000 0072 3a00 0000 7291 0000 0072 3c00  ...r:...r....r<.
-00001d10: 0000 723d 0000 0072 3e00 0000 7288 0000  ..r=...r>...r...
-00001d20: 0072 2700 0000 2904 724d 0000 005a 0a61  .r'...).rM...Z.a
-00001d30: 6c65 7274 5f75 7365 725a 0570 6f69 6e74  lert_userZ.point
-00001d40: 5a0d 6375 7272 656e 745f 6c65 7665 6c72  Z.current_levelr
-00001d50: 1900 0000 7219 0000 0072 1a00 0000 da10  ....r....r......
-00001d60: 696e 6372 656d 656e 745f 706f 696e 7473  increment_points
-00001d70: e700 0000 731e 0000 0000 0204 0108 010c  ....s...........
-00001d80: 010e 010e 010e 010a 0110 010c 0110 010e  ................
-00001d90: 0104 0110 0108 017a 1a55 7365 7250 6f69  .......z.UserPoi
-00001da0: 6e74 2e69 6e63 7265 6d65 6e74 5f70 6f69  nt.increment_poi
-00001db0: 6e74 7363 0100 0000 0000 0000 0000 0000  ntsc............
-00001dc0: 0300 0000 0400 0000 4300 0001 734e 0000  ........C...sN..
-00001dd0: 0067 007d 0174 006a 01a0 02a1 00a0 0364  .g.}.t.j.......d
-00001de0: 01a1 0144 005d 2c7d 027c 026a 047c 006a  ...D.],}.|.j.|.j
-00001df0: 046b 0372 307c 01a0 057c 02a1 0101 0071  .k.r0|...|.....q
-00001e00: 1474 067c 0183 0164 0217 0002 0001 0053  .t.|...d.......S
-00001e10: 0071 1474 067c 0183 0164 0217 0053 0029  .q.t.|...d...S.)
-00001e20: 034e 7a07 2d70 6f69 6e74 7372 0b00 0000  .Nz.-pointsr....
-00001e30: 2907 727f 0000 0072 2000 0000 7243 0000  ).r....r ...rC..
-00001e40: 0072 9000 0000 722a 0000 00da 0661 7070  .r....r*.....app
-00001e50: 656e 6472 6900 0000 2903 724d 0000 005a  endri...).rM...Z
-00001e60: 1375 7365 7273 5f61 626f 7665 5f69 6e5f  .users_above_in_
-00001e70: 7261 6e6b 723f 0000 0072 1900 0000 7219  rankr?...r....r.
-00001e80: 0000 0072 1a00 0000 da08 6765 745f 7261  ...r......get_ra
-00001e90: 6e6b f900 0000 730c 0000 0000 0204 0114  nk....s.........
-00001ea0: 010c 010c 0212 017a 1255 7365 7250 6f69  .......z.UserPoi
-00001eb0: 6e74 2e67 6574 5f72 616e 6b63 0100 0000  nt.get_rankc....
-00001ec0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00001ed0: 4300 0001 7312 0000 0074 006a 016a 027c  C...s....t.j.j.|
-00001ee0: 006a 0364 018d 016a 0453 0029 024e 7293  .j.d...j.S.).Nr.
-00001ef0: 0000 0029 0572 8f00 0000 7220 0000 0072  ...).r....r ...r
-00001f00: 3a00 0000 7289 0000 0072 9100 0000 724c  :...r....r....rL
-00001f10: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00001f20: 0000 da27 6765 745f 7870 5f6e 6565 6465  ...'get_xp_neede
-00001f30: 645f 746f 5f6c 6576 656c 5f75 705f 746f  d_to_level_up_to
-00001f40: 5f6e 6578 745f 6c65 7665 6c03 0100 0073  _next_level....s
-00001f50: 0200 0000 0002 7a31 5573 6572 506f 696e  ......z1UserPoin
-00001f60: 742e 6765 745f 7870 5f6e 6565 6465 645f  t.get_xp_needed_
-00001f70: 746f 5f6c 6576 656c 5f75 705f 746f 5f6e  to_level_up_to_n
-00001f80: 6578 745f 6c65 7665 6c63 0100 0000 0000  ext_levelc......
-00001f90: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00001fa0: 0001 7312 0000 0064 017c 005f 007c 00a0  ..s....d.|._.|..
-00001fb0: 01a1 0001 0064 0053 0029 024e 54a9 02da  .....d.S.).NT...
-00001fc0: 0668 6964 6465 6e72 2700 0000 724c 0000  .hiddenr'...rL..
-00001fd0: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00001fe0: da07 6869 6465 5f78 7007 0100 0073 0400  ..hide_xp....s..
-00001ff0: 0000 0002 0601 7a11 5573 6572 506f 696e  ......z.UserPoin
-00002000: 742e 6869 6465 5f78 7063 0100 0000 0000  t.hide_xpc......
-00002010: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00002020: 0001 7312 0000 0064 017c 005f 007c 00a0  ..s....d.|._.|..
-00002030: 01a1 0001 0064 0053 0029 024e 4672 9c00  .....d.S.).NFr..
-00002040: 0000 724c 0000 0072 1900 0000 7219 0000  ..rL...r....r...
-00002050: 0072 1a00 0000 da07 7368 6f77 5f78 700c  .r......show_xp.
-00002060: 0100 0073 0400 0000 0002 0601 7a11 5573  ...s........z.Us
-00002070: 6572 506f 696e 742e 7368 6f77 5f78 7063  erPoint.show_xpc
-00002080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002090: 0500 0000 4300 0001 731e 0000 0074 0074  ....C...s....t.t
-000020a0: 0174 026a 03a0 04a1 0064 0064 0185 0219  .t.j.....d.d....
-000020b0: 0083 0183 0164 016b 0253 0072 6300 0000  .....d.k.S.rc...
-000020c0: 2905 7269 0000 0072 2e00 0000 727f 0000  ).ri...r....r...
-000020d0: 0072 2000 0000 7243 0000 0072 1900 0000  .r ...rC...r....
-000020e0: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-000020f0: 1e75 7365 725f 706f 696e 7473 5f68 6176  .user_points_hav
-00002100: 655f 6265 656e 5f69 6d70 6f72 7465 6411  e_been_imported.
-00002110: 0100 0073 0200 0000 0003 7a28 5573 6572  ...s......z(User
-00002120: 506f 696e 742e 7573 6572 5f70 6f69 6e74  Point.user_point
-00002130: 735f 6861 7665 5f62 6565 6e5f 696d 706f  s_have_been_impo
-00002140: 7274 6564 6300 0000 0000 0000 0000 0000  rtedc...........
-00002150: 0000 0000 0002 0000 0043 0000 0173 1200  .........C...s..
-00002160: 0000 7400 6a01 a002 a100 a003 a100 0100  ..t.j...........
-00002170: 6400 5300 724f 0000 0029 0472 7f00 0000  d.S.rO...).r....
-00002180: 7220 0000 0072 4300 0000 da06 6465 6c65  r ...rC.....dele
-00002190: 7465 7219 0000 0072 1900 0000 7219 0000  ter....r....r...
-000021a0: 0072 1a00 0000 da11 636c 6561 725f 616c  .r......clear_al
-000021b0: 6c5f 656e 7472 6965 7316 0100 0073 0200  l_entries....s..
-000021c0: 0000 0003 7a1b 5573 6572 506f 696e 742e  ....z.UserPoint.
-000021d0: 636c 6561 725f 616c 6c5f 656e 7472 6965  clear_all_entrie
-000021e0: 7363 0100 0000 0000 0000 0000 0000 0100  sc..............
-000021f0: 0000 0600 0000 4300 0001 733a 0000 0074  ......C...s:...t
-00002200: 006a 00a0 017c 006a 0274 03a0 0474 056a  .j...|.j.t...t.j
-00002210: 06a1 01a1 0274 006a 0764 0164 028d 0117  .....t.j.d.d....
-00002220: 0074 006a 006a 0874 03a0 0474 056a 06a1  .t.j.j.t...t.j..
-00002230: 0164 038d 016b 0053 0029 044e 720b 0000  .d...k.S.).Nr...
-00002240: 00a9 01da 076d 696e 7574 6573 7209 0000  .....minutesr...
-00002250: 0029 0972 3c00 0000 da0d 6672 6f6d 7469  .).r<.....fromti
-00002260: 6d65 7374 616d 7072 8800 0000 da04 7079  mestampr......py
-00002270: 747a 7208 0000 0072 0500 0000 da09 5449  tzr....r......TI
-00002280: 4d45 5f5a 4f4e 45da 0974 696d 6564 656c  ME_ZONE..timedel
-00002290: 7461 723d 0000 0072 4c00 0000 7219 0000  tar=...rL...r...
-000022a0: 0072 1900 0000 721a 0000 0072 9500 0000  .r....r....r....
-000022b0: 1b01 0000 7310 0000 0000 0106 0104 010a  ....s...........
-000022c0: fe02 030a fd02 0314 fd7a 2755 7365 7250  .........z'UserP
-000022d0: 6f69 6e74 2e6d 6573 7361 6765 5f63 6f75  oint.message_cou
-000022e0: 6e74 735f 746f 7761 7264 735f 706f 696e  nts_towards_poin
-000022f0: 7473 6301 0000 0000 0000 0000 0000 0003  tsc.............
-00002300: 0000 0004 0000 0043 0000 0173 4400 0000  .......C...sD...
-00002310: 6401 7400 6a01 9b00 9d02 6402 6403 9c02  d.t.j.....d.d...
-00002320: 7d01 7402 6a03 6404 7c00 6a04 9b00 9d02  }.t.j.d.|.j.....
-00002330: 7c01 6405 8d02 7d02 6406 7c02 a005 a100  |.d...}.d.|.....
-00002340: 7600 7240 7c02 a005 a100 6406 1900 5300  v.r@|.....d...S.
-00002350: 6407 5300 2908 4e7a 0442 6f74 207a 1061  d.S.).Nz.Bot z.a
-00002360: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e29  pplication/json)
-00002370: 02da 0d41 7574 686f 7269 7a61 7469 6f6e  ...Authorization
-00002380: 7a0c 436f 6e74 656e 742d 5479 7065 7a1e  z.Content-Typez.
-00002390: 6874 7470 733a 2f2f 6469 7363 6f72 642e  https://discord.
-000023a0: 636f 6d2f 6170 692f 7573 6572 732f 2901  com/api/users/).
-000023b0: da07 6865 6164 6572 7372 3300 0000 7258  ..headersr3...rX
-000023c0: 0000 0029 0672 0500 0000 5a11 4449 5343  ...).r....Z.DISC
-000023d0: 4f52 445f 424f 545f 544f 4b45 4eda 0872  ORD_BOT_TOKEN..r
-000023e0: 6571 7565 7374 7372 3a00 0000 722a 0000  equestsr:...r*..
-000023f0: 00da 046a 736f 6e29 0372 4d00 0000 5a0e  ...json).rM...Z.
-00002400: 6469 7363 6f72 645f 6865 6164 6572 da08  discord_header..
-00002410: 7265 7370 6f6e 7365 7219 0000 0072 1900  responser....r..
-00002420: 0000 721a 0000 0072 3300 0000 2101 0000  ..r....r3...!...
-00002430: 7310 0000 0000 030a 0102 fe06 0404 010a  s...............
-00002440: 0102 fe06 057a 1255 7365 7250 6f69 6e74  .....z.UserPoint
-00002450: 2e75 7365 726e 616d 6563 0000 0000 0000  .usernamec......
-00002460: 0000 0000 0000 0000 0000 0300 0000 4300  ..............C.
-00002470: 0001 7314 0000 0064 0164 0284 0074 006a  ..s....d.d...t.j
-00002480: 01a0 02a1 0044 0083 0153 0029 034e 6301  .....D...S.).Nc.
-00002490: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-000024a0: 0000 0053 0000 0173 1400 0000 6900 7c00  ...S...s....i.|.
-000024b0: 5d0c 7d01 7c01 6a00 7c01 9302 7104 5300  ].}.|.j.|...q.S.
-000024c0: 7219 0000 0072 4200 0000 2902 725d 0000  r....rB...).r]..
-000024d0: 0072 8c00 0000 7219 0000 0072 1900 0000  .r....r....r....
-000024e0: 721a 0000 00da 0a3c 6469 6374 636f 6d70  r......<dictcomp
-000024f0: 3e31 0100 0072 6000 0000 7a2a 5573 6572  >1...r`...z*User
-00002500: 506f 696e 742e 6c6f 6164 5f74 6f5f 6469  Point.load_to_di
-00002510: 6374 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  ct.<locals>.<dic
-00002520: 7463 6f6d 703e 2903 727f 0000 0072 2000  tcomp>).r....r .
-00002530: 0000 7243 0000 0072 1900 0000 7219 0000  ..rC...r....r...
-00002540: 0072 1900 0000 721a 0000 00da 0c6c 6f61  .r....r......loa
-00002550: 645f 746f 5f64 6963 742e 0100 0073 0200  d_to_dict....s..
-00002560: 0000 0003 7a16 5573 6572 506f 696e 742e  ....z.UserPoint.
-00002570: 6c6f 6164 5f74 6f5f 6469 6374 4e29 2372  load_to_dictN)#r
-00002580: 1500 0000 7216 0000 0072 1700 0000 7206  ....r....r....r.
-00002590: 0000 00da 1750 6f73 6974 6976 6542 6967  .....PositiveBig
-000025a0: 496e 7465 6765 7246 6965 6c64 722a 0000  IntegerFieldr*..
-000025b0: 0072 8500 0000 7286 0000 0072 8700 0000  .r....r....r....
-000025c0: 7253 0000 0072 8800 0000 7289 0000 00da  rS...r....r.....
-000025d0: 0c42 6f6f 6c65 616e 4669 656c 6472 9d00  .BooleanFieldr..
-000025e0: 0000 7204 0000 0072 8200 0000 da0c 7374  ..r....r......st
-000025f0: 6174 6963 6d65 7468 6f64 7296 0000 0072  aticmethodr....r
-00002600: 9700 0000 723c 0000 0072 3d00 0000 728d  ....r<...r=...r.
-00002610: 0000 0072 5400 0000 728a 0000 0072 9800  ...rT...r....r..
-00002620: 0000 729a 0000 0072 9b00 0000 729e 0000  ..r....r....r...
-00002630: 0072 9f00 0000 72a0 0000 0072 a200 0000  .r....r....r....
-00002640: 7295 0000 00da 0870 726f 7065 7274 7972  r......propertyr
-00002650: 3300 0000 72af 0000 0072 1900 0000 7219  3...r....r....r.
-00002660: 0000 0072 1900 0000 721a 0000 0072 7f00  ...r....r....r..
-00002670: 0000 b400 0000 7358 0000 0008 0104 0102  ......sX........
-00002680: ff06 0308 0308 0308 0304 0102 ff06 0308  ................
-00002690: 0304 0102 ff06 0402 010a 0302 0102 020c  ................
-000026a0: 010a fe0e 0c02 010a 0902 010a 1102 010a  ................
-000026b0: 0902 010a 0302 010a 0402 010a 0402 0102  ................
-000026c0: 010c 0302 0102 010c 0308 0602 010a 0c02  ................
-000026d0: 0102 0172 7f00 0000 6300 0000 0000 0000  ...r....c.......
-000026e0: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
-000026f0: 0173 b800 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
-00002700: 6a04 6401 6402 8d01 5a05 6503 a004 a100  j.d.d...Z.e.....
-00002710: 5a06 6503 a004 a100 5a07 6503 6a04 6401  Z.e.....Z.e.j.d.
-00002720: 6401 6403 8d02 5a08 6503 6a09 6404 6401  d.d...Z.e.j.d.d.
-00002730: 6401 6405 8d03 5a0a 650b 650c 6417 6407  d.d...Z.e.e.d.d.
-00002740: 6408 8401 8301 8301 5a0d 650c 6409 640a  d.......Z.e.d.d.
-00002750: 8400 8301 5a0e 650b 650c 640b 640c 8400  ....Z.e.e.d.d...
-00002760: 8301 8301 5a0f 650b 650c 640d 640e 8400  ....Z.e.e.d.d...
-00002770: 8301 8301 5a10 650b 650c 640f 6410 8400  ....Z.e.e.d.d...
-00002780: 8301 8301 5a11 650c 6411 6412 8400 8301  ....Z.e.d.d.....
-00002790: 5a12 650c 6413 6414 8400 8301 5a13 650c  Z.e.d.d.....Z.e.
-000027a0: 6415 6416 8400 8301 5a14 6406 5300 2918  d.d.....Z.d.S.).
-000027b0: 728f 0000 0054 7280 0000 0029 0272 1200  r....Tr....).r..
-000027c0: 0000 7281 0000 00e9 f401 0000 2903 7211  ..r.........).r.
-000027d0: 0000 0072 1200 0000 7281 0000 004e 6305  ...r....r....Nc.
-000027e0: 0000 0000 0000 0000 0000 0006 0000 0007  ................
-000027f0: 0000 0043 0000 0173 1e00 0000 7400 7c00  ...C...s....t.|.
-00002800: 7c01 7c02 7c03 7c04 6401 8d05 7d05 7c05  |.|.|.|.d...}.|.
-00002810: a001 a100 0100 7c05 5300 2902 4e29 0572  ......|.S.).N).r
-00002820: 9400 0000 728e 0000 0072 9100 0000 da07  ....r....r......
-00002830: 726f 6c65 5f69 64da 0972 6f6c 655f 6e61  role_id..role_na
-00002840: 6d65 2902 728f 0000 0072 2700 0000 2906  me).r....r'...).
-00002850: 7294 0000 0072 8e00 0000 7291 0000 0072  r....r....r....r
-00002860: b500 0000 72b6 0000 0072 8b00 0000 7219  ....r....r....r.
-00002870: 0000 0072 1900 0000 721a 0000 00da 0c63  ...r....r......c
-00002880: 7265 6174 655f 6c65 7665 6c4a 0100 0073  reate_levelJ...s
-00002890: 0e00 0000 0004 0201 0401 0201 04fd 0605  ................
-000028a0: 0801 7a12 4c65 7665 6c2e 6372 6561 7465  ..z.Level.create
-000028b0: 5f6c 6576 656c 6301 0000 0000 0000 0000  _levelc.........
-000028c0: 0000 0001 0000 0002 0000 0043 0000 0173  ...........C...s
-000028d0: 0c00 0000 7c00 a000 a100 0100 6400 5300  ....|.......d.S.
-000028e0: 724f 0000 0072 2600 0000 724c 0000 0072  rO...r&...rL...r
-000028f0: 1900 0000 7219 0000 0072 1a00 0000 7282  ....r....r....r.
-00002900: 0000 0056 0100 0073 0200 0000 0002 7a10  ...V...s......z.
-00002910: 4c65 7665 6c2e 6173 796e 635f 7361 7665  Level.async_save
-00002920: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00002930: 0005 0000 0043 0000 0173 1e00 0000 7400  .....C...s....t.
-00002940: 7401 7402 6a03 a004 a100 6400 6401 8502  t.t.j.....d.d...
-00002950: 1900 8301 8301 6401 6b02 5300 7263 0000  ......d.k.S.rc..
-00002960: 0029 0572 6900 0000 722e 0000 0072 8f00  .).ri...r....r..
-00002970: 0000 7220 0000 0072 4300 0000 7219 0000  ..r ...rC...r...
-00002980: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00002990: da1f 6c65 7665 6c5f 706f 696e 7473 5f68  ..level_points_h
-000029a0: 6176 655f 6265 656e 5f69 6d70 6f72 7465  ave_been_importe
-000029b0: 645a 0100 0073 0200 0000 0003 7a25 4c65  dZ...s......z%Le
-000029c0: 7665 6c2e 6c65 7665 6c5f 706f 696e 7473  vel.level_points
-000029d0: 5f68 6176 655f 6265 656e 5f69 6d70 6f72  _have_been_impor
-000029e0: 7465 6463 0000 0000 0000 0000 0000 0000  tedc............
-000029f0: 0000 0000 0200 0000 4300 0001 7312 0000  ........C...s...
-00002a00: 0074 006a 01a0 02a1 00a0 03a1 0001 0064  .t.j...........d
-00002a10: 0053 0072 4f00 0000 2904 728f 0000 0072  .S.rO...).r....r
-00002a20: 2000 0000 7243 0000 0072 a100 0000 7219   ...rC...r....r.
-00002a30: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00002a40: 0000 72a2 0000 005f 0100 0073 0200 0000  ..r...._...s....
-00002a50: 0003 7a17 4c65 7665 6c2e 636c 6561 725f  ..z.Level.clear_
-00002a60: 616c 6c5f 656e 7472 6965 7363 0000 0000  all_entriesc....
-00002a70: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00002a80: 4300 0001 7314 0000 0064 0164 0284 0074  C...s....d.d...t
-00002a90: 006a 01a0 02a1 0044 0083 0153 0029 034e  .j.....D...S.).N
-00002aa0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00002ab0: 0004 0000 0053 0000 0173 1400 0000 6900  .....S...s....i.
-00002ac0: 7c00 5d0c 7d01 7c01 6a00 7c01 9302 7104  |.].}.|.j.|...q.
-00002ad0: 5300 7219 0000 0072 9300 0000 2902 725d  S.r....r....).r]
-00002ae0: 0000 0072 8b00 0000 7219 0000 0072 1900  ...r....r....r..
-00002af0: 0000 721a 0000 0072 ae00 0000 6701 0000  ..r....r....g...
-00002b00: 7260 0000 007a 264c 6576 656c 2e6c 6f61  r`...z&Level.loa
-00002b10: 645f 746f 5f64 6963 742e 3c6c 6f63 616c  d_to_dict.<local
-00002b20: 733e 2e3c 6469 6374 636f 6d70 3e29 0372  s>.<dictcomp>).r
-00002b30: 8f00 0000 7220 0000 0072 4300 0000 7219  ....r ...rC...r.
-00002b40: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00002b50: 0000 72af 0000 0064 0100 0073 0200 0000  ..r....d...s....
-00002b60: 0003 7a12 4c65 7665 6c2e 6c6f 6164 5f74  ..z.Level.load_t
-00002b70: 6f5f 6469 6374 6303 0000 0000 0000 0000  o_dictc.........
-00002b80: 0000 0003 0000 0002 0000 0043 0000 0173  ...........C...s
-00002b90: 1800 0000 7c01 7c00 5f00 7c02 7c00 5f01  ....|.|._.|.|._.
-00002ba0: 7c00 a002 a100 0100 6400 5300 724f 0000  |.......d.S.rO..
-00002bb0: 00a9 0372 b600 0000 72b5 0000 0072 2700  ...r....r....r'.
-00002bc0: 0000 2903 724d 0000 00da 0d6e 6577 5f72  ..).rM.....new_r
-00002bd0: 6f6c 655f 6e61 6d65 72b5 0000 0072 1900  ole_namer....r..
-00002be0: 0000 7219 0000 0072 1a00 0000 da0e 7365  ..r....r......se
-00002bf0: 745f 6c65 7665 6c5f 6e61 6d65 6901 0000  t_level_namei...
-00002c00: 7306 0000 0000 0206 0106 017a 144c 6576  s..........z.Lev
-00002c10: 656c 2e73 6574 5f6c 6576 656c 5f6e 616d  el.set_level_nam
-00002c20: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
-00002c30: 0000 0200 0000 4300 0001 7312 0000 007c  ......C...s....|
-00002c40: 017c 005f 007c 00a0 01a1 0001 0064 0053  .|._.|.......d.S
-00002c50: 0072 4f00 0000 2902 72b6 0000 0072 2700  .rO...).r....r'.
-00002c60: 0000 2902 724d 0000 0072 ba00 0000 7219  ..).rM...r....r.
-00002c70: 0000 0072 1900 0000 721a 0000 00da 1172  ...r....r......r
-00002c80: 656e 616d 655f 6c65 7665 6c5f 6e61 6d65  ename_level_name
-00002c90: 6f01 0000 7304 0000 0000 0206 017a 174c  o...s........z.L
-00002ca0: 6576 656c 2e72 656e 616d 655f 6c65 7665  evel.rename_leve
-00002cb0: 6c5f 6e61 6d65 6301 0000 0000 0000 0000  l_namec.........
-00002cc0: 0000 0001 0000 0002 0000 0043 0000 0173  ...........C...s
-00002cd0: 1800 0000 6400 7c00 5f00 6400 7c00 5f01  ....d.|._.d.|._.
-00002ce0: 7c00 a002 a100 0100 6400 5300 724f 0000  |.......d.S.rO..
-00002cf0: 0072 b900 0000 724c 0000 0072 1900 0000  .r....rL...r....
-00002d00: 7219 0000 0072 1a00 0000 da0b 7265 6d6f  r....r......remo
-00002d10: 7665 5f72 6f6c 6574 0100 0073 0600 0000  ve_rolet...s....
-00002d20: 0002 0601 0601 7a11 4c65 7665 6c2e 7265  ......z.Level.re
-00002d30: 6d6f 7665 5f72 6f6c 6529 024e 4e29 1572  move_role).NN).r
-00002d40: 1500 0000 7216 0000 0072 1700 0000 7206  ....r....r....r.
-00002d50: 0000 0072 b000 0000 7294 0000 0072 8e00  ...r....r....r..
-00002d60: 0000 7291 0000 0072 b500 0000 7252 0000  ..r....r....rR..
-00002d70: 0072 b600 0000 72b2 0000 0072 0400 0000  .r....r....r....
-00002d80: 72b7 0000 0072 8200 0000 72b8 0000 0072  r....r....r....r
-00002d90: a200 0000 72af 0000 0072 bb00 0000 72bc  ....r....r....r.
-00002da0: 0000 0072 bd00 0000 7219 0000 0072 1900  ...r....r....r..
-00002db0: 0000 7219 0000 0072 1a00 0000 728f 0000  ..r....r....r...
-00002dc0: 0034 0100 0073 4600 0000 0801 0401 02ff  .4...sF.........
-00002dd0: 0603 0804 0804 0401 0201 02fe 0604 0401  ................
-00002de0: 0201 0201 02fd 0606 0201 0202 00ff 0e0a  ................
-00002df0: 0201 0a03 0201 0201 0c03 0201 0201 0c03  ................
-00002e00: 0201 0201 0c03 0201 0a05 0201 0a04 0201  ................
-00002e10: 728f 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00002e20: 0000 0000 0000 0400 0000 4000 0001 73be  ..........@...s.
-00002e30: 0000 0065 005a 0164 005a 0265 036a 0464  ...e.Z.d.Z.e.j.d
-00002e40: 0164 028d 015a 0565 036a 0664 0364 048d  .d...Z.e.j.d.d..
-00002e50: 015a 0765 036a 0864 0564 0664 078d 025a  .Z.e.j.d.d.d...Z
-00002e60: 0965 036a 0664 0364 048d 015a 0a64 0864  .e.j.d.d...Z.d.d
-00002e70: 0984 005a 0b65 0c65 0d64 0a64 0b84 0083  ...Z.e.e.d.d....
-00002e80: 0183 015a 0e65 0c65 0d64 0c64 0d84 0083  ...Z.e.e.d.d....
-00002e90: 0183 015a 0f65 0c65 0d64 0e64 0f84 0083  ...Z.e.e.d.d....
-00002ea0: 0183 015a 1065 0c65 0d64 1064 1184 0083  ...Z.e.e.d.d....
-00002eb0: 0183 015a 1165 0c65 0d64 1264 1384 0083  ...Z.e.e.d.d....
-00002ec0: 0183 015a 1265 0c65 0d64 1464 1584 0083  ...Z.e.e.d.d....
-00002ed0: 0183 015a 1365 0c65 0d64 1664 1784 0083  ...Z.e.e.d.d....
-00002ee0: 0183 015a 1464 1864 1984 005a 1564 1a53  ...Z.d.d...Z.d.S
-00002ef0: 0029 1bda 0852 656d 696e 6465 7254 720e  .)...ReminderTr.
-00002f00: 0000 0072 0100 0000 7256 0000 0072 5700  ...r....rV...rW.
-00002f10: 0000 da07 494e 5641 4c49 4472 5900 0000  ....INVALIDrY...
-00002f20: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00002f30: 0006 0000 0043 0000 0173 1c00 0000 6401  .....C...s....d.
-00002f40: 7c00 6a00 9b00 6402 7c00 6a01 9b00 6403  |.j...d.|.j...d.
-00002f50: 7c00 6a02 9b00 9d06 5300 2904 4e7a 1252  |.j.....S.).Nz.R
-00002f60: 656d 696e 6465 7220 666f 7220 7573 6572  eminder for user
-00002f70: 207a 0920 6f6e 2064 6174 6520 7a0e 2077   z. on date z. w
-00002f80: 6974 6820 6d65 7373 6167 6520 2903 da09  ith message )...
-00002f90: 6175 7468 6f72 5f69 64da 1372 656d 696e  author_id..remin
-00002fa0: 6465 725f 6461 7465 5f65 706f 6368 da07  der_date_epoch..
-00002fb0: 6d65 7373 6167 6572 4c00 0000 7219 0000  messagerL...r...
-00002fc0: 0072 1900 0000 721a 0000 0072 4e00 0000  .r....r....rN...
-00002fd0: 8a01 0000 7302 0000 0000 017a 1052 656d  ....s......z.Rem
-00002fe0: 696e 6465 722e 5f5f 7374 725f 5f63 0100  inder.__str__c..
-00002ff0: 0000 0000 0000 0000 0000 0100 0000 0600  ................
-00003000: 0000 4300 0001 732e 0000 0074 0074 016a  ..C...s....t.t.j
-00003010: 02a0 03a1 006a 0474 056a 056a 0674 07a0  .....j.t.j.j.t..
-00003020: 0874 096a 0a9b 00a1 0164 018d 01a0 0ba1  .t.j.....d......
-00003030: 0064 028d 0183 0153 0029 034e 7209 0000  .d.....S.).Nr...
-00003040: 0029 015a 1872 656d 696e 6465 725f 6461  .).Z.reminder_da
-00003050: 7465 5f65 706f 6368 5f5f 6c74 6529 0c72  te_epoch__lte).r
-00003060: 2e00 0000 72be 0000 0072 2000 0000 7243  ....r....r ...rC
-00003070: 0000 0072 3000 0000 723c 0000 0072 3d00  ...r0...r<...r=.
-00003080: 0000 72a6 0000 0072 0800 0000 7205 0000  ..r....r....r...
-00003090: 0072 a700 0000 723e 0000 0072 3100 0000  .r....r>...r1...
-000030a0: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-000030b0: 1567 6574 5f65 7870 6972 6564 5f72 656d  .get_expired_rem
-000030c0: 696e 6465 7273 8d01 0000 730e 0000 0000  inders....s.....
-000030d0: 0302 010a 0106 010c ff08 ff04 ff7a 1e52  .............z.R
-000030e0: 656d 696e 6465 722e 6765 745f 6578 7069  eminder.get_expi
-000030f0: 7265 645f 7265 6d69 6e64 6572 7363 0200  red_remindersc..
-00003100: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-00003110: 0000 4300 0001 733c 0000 007c 019b 00a0  ..C...s<...|....
-00003120: 00a1 0073 0e64 0053 0074 016a 02a0 03a1  ...s.d.S.t.j....
-00003130: 006a 047c 0164 018d 017d 0274 057c 0283  .j.|.d...}.t.|..
-00003140: 0164 026b 0272 3064 0053 007c 0264 0219  .d.k.r0d.S.|.d..
-00003150: 0053 0064 0053 0029 034e a901 7250 0000  .S.d.S.).N..rP..
-00003160: 0072 0100 0000 2906 da07 6973 6469 6769  .r....)...isdigi
-00003170: 7472 be00 0000 7220 0000 0072 4300 0000  tr....r ...rC...
-00003180: 7230 0000 0072 6900 0000 2903 7222 0000  r0...ri...).r"..
-00003190: 005a 0b72 656d 696e 6465 725f 6964 da09  .Z.reminder_id..
-000031a0: 7265 6d69 6e64 6572 7372 1900 0000 7219  remindersr....r.
-000031b0: 0000 0072 1a00 0000 da12 6765 745f 7265  ...r......get_re
-000031c0: 6d69 6e64 6572 5f62 795f 6964 9801 0000  minder_by_id....
-000031d0: 730c 0000 0000 030a 0104 0112 010c 0104  s...............
-000031e0: 027a 1b52 656d 696e 6465 722e 6765 745f  .z.Reminder.get_
-000031f0: 7265 6d69 6e64 6572 5f62 795f 6964 6302  reminder_by_idc.
-00003200: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00003210: 0000 0043 0000 0173 1a00 0000 7400 6a01  ...C...s....t.j.
-00003220: a002 a100 6a03 7c01 6401 8d01 a004 a100  ....j.|.d.......
-00003230: 0100 6400 5300 2902 4e72 c400 0000 2905  ..d.S.).Nr....).
-00003240: 72be 0000 0072 2000 0000 7243 0000 0072  r....r ...rC...r
-00003250: 3a00 0000 72a1 0000 00a9 0272 2200 0000  :...r......r"...
-00003260: 5a12 7265 6d69 6e64 6572 5f74 6f5f 6465  Z.reminder_to_de
-00003270: 6c65 7465 7219 0000 0072 1900 0000 721a  leter....r....r.
-00003280: 0000 00da 1564 656c 6574 655f 7265 6d69  .....delete_remi
-00003290: 6e64 6572 5f62 795f 6964 a401 0000 7302  nder_by_id....s.
-000032a0: 0000 0000 037a 1e52 656d 696e 6465 722e  .....z.Reminder.
-000032b0: 6465 6c65 7465 5f72 656d 696e 6465 725f  delete_reminder_
-000032c0: 6279 5f69 6463 0200 0000 0000 0000 0000  by_idc..........
-000032d0: 0000 0200 0000 0200 0000 4300 0001 730c  ..........C...s.
-000032e0: 0000 007c 01a0 00a1 0001 0064 0053 0072  ...|.......d.S.r
-000032f0: 4f00 0000 a901 72a1 0000 0072 c800 0000  O.....r....r....
-00003300: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-00003310: 0f64 656c 6574 655f 7265 6d69 6e64 6572  .delete_reminder
-00003320: a901 0000 7302 0000 0000 037a 1852 656d  ....s......z.Rem
-00003330: 696e 6465 722e 6465 6c65 7465 5f72 656d  inder.delete_rem
-00003340: 696e 6465 7263 0200 0000 0000 0000 0000  inderc..........
-00003350: 0000 0200 0000 0400 0000 4300 0001 731c  ..........C...s.
-00003360: 0000 0074 0074 016a 02a0 03a1 006a 047c  ...t.t.j.....j.|
-00003370: 0164 018d 01a0 0564 02a1 0183 0153 0029  .d.....d.....S.)
-00003380: 034e 2901 72c0 0000 0072 c100 0000 2906  .N).r....r....).
-00003390: 722e 0000 0072 be00 0000 7220 0000 0072  r....r....r ...r
-000033a0: 4300 0000 7230 0000 0072 9000 0000 2902  C...r0...r....).
-000033b0: 7222 0000 0072 c000 0000 7219 0000 0072  r"...r....r....r
-000033c0: 1900 0000 721a 0000 00da 1667 6574 5f72  ....r......get_r
-000033d0: 656d 696e 6465 725f 6279 5f61 7574 686f  eminder_by_autho
-000033e0: 72ae 0100 0073 0200 0000 0003 7a1f 5265  r....s......z.Re
-000033f0: 6d69 6e64 6572 2e67 6574 5f72 656d 696e  minder.get_remin
-00003400: 6465 725f 6279 5f61 7574 686f 7263 0100  der_by_authorc..
-00003410: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00003420: 0000 4300 0001 7314 0000 0074 0074 016a  ..C...s....t.t.j
-00003430: 02a0 03a1 00a0 0464 01a1 0183 0153 0029  .......d.....S.)
-00003440: 024e 72c1 0000 0029 0572 2e00 0000 72be  .Nr....).r....r.
-00003450: 0000 0072 2000 0000 7243 0000 0072 9000  ...r ...rC...r..
-00003460: 0000 7231 0000 0072 1900 0000 7219 0000  ..r1...r....r...
-00003470: 0072 1a00 0000 da11 6765 745f 616c 6c5f  .r......get_all_
-00003480: 7265 6d69 6e64 6572 73b4 0100 0073 0200  reminders....s..
-00003490: 0000 0003 7a1a 5265 6d69 6e64 6572 2e67  ....z.Reminder.g
-000034a0: 6574 5f61 6c6c 5f72 656d 696e 6465 7273  et_all_reminders
-000034b0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000034c0: 0002 0000 0043 0000 0173 0c00 0000 7c01  .....C...s....|.
-000034d0: a000 a100 0100 6400 5300 724f 0000 0072  ......d.S.rO...r
-000034e0: 2600 0000 2902 7222 0000 005a 1072 656d  &...).r"...Z.rem
-000034f0: 696e 6465 725f 746f 5f73 6176 6572 1900  inder_to_saver..
-00003500: 0000 7219 0000 0072 1a00 0000 da0d 7361  ..r....r......sa
-00003510: 7665 5f72 656d 696e 6465 72ba 0100 0073  ve_reminder....s
-00003520: 0200 0000 0003 7a16 5265 6d69 6e64 6572  ......z.Reminder
-00003530: 2e73 6176 655f 7265 6d69 6e64 6572 6301  .save_reminderc.
-00003540: 0000 0000 0000 0000 0000 0006 0000 0004  ................
-00003550: 0000 0043 0000 0173 b000 0000 7400 7c00  ...C...s....t.|.
-00003560: 6a01 7402 a002 a100 1800 8301 7d01 7c01  j.t.........}.|.
-00003570: 6401 1a00 7d02 7c01 6401 1600 7d01 7c01  d...}.|.d...}.|.
-00003580: 6402 1a00 7d03 7c01 6402 3b00 7d01 7c01  d...}.|.d.;.}.|.
-00003590: 6403 1a00 7d04 7c01 6403 3b00 7d01 6404  d...}.|.d.;.}.d.
-000035a0: 7d05 7c02 6405 6b04 725e 7c05 6406 7c02  }.|.d.k.r^|.d.|.
-000035b0: 9b00 6407 9d03 3700 7d05 7c03 6405 6b04  ..d...7.}.|.d.k.
-000035c0: 7276 7c05 6406 7c03 9b00 6408 9d03 3700  rv|.d.|...d...7.
-000035d0: 7d05 7c04 6405 6b04 728e 7c05 6406 7c04  }.|.d.k.r.|.d.|.
-000035e0: 9b00 6409 9d03 3700 7d05 7c01 6405 6b04  ..d...7.}.|.d.k.
-000035f0: 72a6 7c05 6406 7c01 9b00 640a 9d03 3700  r.|.d.|...d...7.
-00003600: 7d05 7c05 9b00 640b 9d02 5300 290c 4e69  }.|...d...S.).Ni
-00003610: 8051 0100 6910 0e00 00e9 3c00 0000 7a11  .Q..i.....<...z.
-00003620: 5265 6d69 6e64 6572 2073 6574 2066 6f72  Reminder set for
-00003630: 2072 0100 0000 fa01 207a 0520 6461 7973   r...... z. days
-00003640: 7a06 2068 6f75 7273 7a08 206d 696e 7574  z. hoursz. minut
-00003650: 6573 7a08 2073 6563 6f6e 6473 7a09 2066  esz. secondsz. f
-00003660: 726f 6d20 6e6f 7729 0372 3600 0000 72c1  rom now).r6...r.
-00003670: 0000 00da 0474 696d 6529 0672 4d00 0000  .....time).rM...
-00003680: da07 7365 636f 6e64 7372 7400 0000 7272  ..secondsrt...rr
-00003690: 0000 0072 a400 0000 72c2 0000 0072 1900  ...r....r....r..
-000036a0: 0000 7219 0000 0072 1a00 0000 da0d 6765  ..r....r......ge
-000036b0: 745f 636f 756e 7464 6f77 6ebf 0100 0073  t_countdown....s
-000036c0: 2200 0000 0001 1201 0801 0801 0801 0801  "...............
-000036d0: 0801 0802 0401 0801 1001 0801 1001 0801  ................
-000036e0: 1001 0801 1001 7a16 5265 6d69 6e64 6572  ......z.Reminder
-000036f0: 2e67 6574 5f63 6f75 6e74 646f 776e 4e29  .get_countdownN)
-00003700: 1672 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
-00003710: 7206 0000 0072 7b00 0000 7250 0000 0072  r....r{...rP...r
-00003720: 5300 0000 72c1 0000 0072 5200 0000 72c2  S...r....rR...r.
-00003730: 0000 0072 c000 0000 724e 0000 0072 5400  ...r....rN...rT.
-00003740: 0000 7204 0000 0072 c300 0000 72c7 0000  ..r....r....r...
-00003750: 0072 c900 0000 72cb 0000 0072 cc00 0000  .r....r....r....
-00003760: 72cd 0000 0072 ce00 0000 72d3 0000 0072  r....r....r....r
-00003770: 1900 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
-00003780: 0000 0072 be00 0000 7b01 0000 7348 0000  ...r....{...sH..
-00003790: 0008 0104 0102 ff06 0304 0102 ff06 0304  ................
-000037a0: 0102 0102 fe06 0404 0102 ff06 0408 0302  ................
-000037b0: 0102 010c 0902 0102 010c 0a02 0102 010c  ................
-000037c0: 0302 0102 010c 0302 0102 010c 0402 0102  ................
-000037d0: 010c 0402 0102 010c 0372 be00 0000 6300  .........r....c.
-000037e0: 0000 0000 0000 0000 0000 0000 0000 0005  ................
-000037f0: 0000 0000 0000 0173 c000 0000 6500 5a01  .......s....e.Z.
-00003800: 6400 5a02 6503 6a04 6401 6402 8d01 5a05  d.Z.e.j.d.d...Z.
-00003810: 6503 6a06 6403 6404 8d01 5a07 6503 6a08  e.j.d.d...Z.e.j.
-00003820: 6405 6406 6401 6407 8d03 5a09 6503 6a06  d.d.d.d...Z.e.j.
-00003830: 6403 6404 8d01 5a0a 6503 6a06 6408 6409  d.d...Z.e.j.d.d.
-00003840: 8d01 5a0b 6503 6a06 6408 6409 8d01 5a0c  ..Z.e.j.d.d...Z.
-00003850: 650d 640a 640b 8400 8301 5a0e 650d 640c  e.d.d.....Z.e.d.
-00003860: 640d 8400 8301 5a0f 6510 6511 6400 640e  d.....Z.e.e.d.d.
-00003870: 640f 9c02 6410 6411 8404 8301 8301 5a12  d...d.d.......Z.
-00003880: 6510 6511 6412 6413 8400 8301 8301 5a13  e.e.d.d.......Z.
-00003890: 6510 6511 6414 6415 8400 8301 8301 5a14  e.e.d.d.......Z.
-000038a0: 8700 6601 6416 6417 8408 5a15 6418 6419  ..f.d.d...Z.d.d.
-000038b0: 8400 5a16 8700 0400 5a17 5300 291a da0b  ..Z.....Z.S.)...
-000038c0: 4865 6c70 4d65 7373 6167 6554 720e 0000  HelpMessageTr...
-000038d0: 0046 7213 0000 0072 b400 0000 4e29 0372  .Fr....r....N).r
-000038e0: 1100 0000 7214 0000 0072 1200 0000 7201  ....r....r....r.
-000038f0: 0000 0072 5600 0000 6301 0000 0000 0000  ...rV...c.......
-00003900: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
-00003910: 0173 1200 0000 7400 7401 6a01 a002 7c00  .s....t.t.j...|.
-00003920: 6a03 a101 8301 5300 724f 0000 0029 04da  j.....S.rO...)..
-00003930: 1b63 6f6e 7665 7274 5f75 7463 5f74 696d  .convert_utc_tim
-00003940: 655f 746f 5f70 6163 6966 6963 723c 0000  e_to_pacificr<..
-00003950: 0072 a500 0000 da1c 6865 6c70 5f6d 6573  .r......help_mes
-00003960: 7361 6765 5f65 7870 6972 6174 696f 6e5f  sage_expiration_
-00003970: 6461 7465 724c 0000 0072 1900 0000 7219  daterL...r....r.
-00003980: 0000 0072 1a00 0000 da17 6765 745f 6578  ...r......get_ex
-00003990: 7069 7261 7469 6f6e 5f64 6174 655f 7073  piration_date_ps
-000039a0: 74dc 0100 0073 0200 0000 0002 7a23 4865  t....s......z#He
-000039b0: 6c70 4d65 7373 6167 652e 6765 745f 6578  lpMessage.get_ex
-000039c0: 7069 7261 7469 6f6e 5f64 6174 655f 7073  piration_date_ps
-000039d0: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
-000039e0: 0000 0400 0000 4300 0001 7312 0000 0074  ......C...s....t
-000039f0: 0074 016a 01a0 027c 006a 03a1 0183 0153  .t.j...|.j.....S
-00003a00: 0072 4f00 0000 2904 72d5 0000 0072 3c00  .rO...).r....r<.
-00003a10: 0000 72a5 0000 00da 0c74 696d 655f 6372  ..r......time_cr
-00003a20: 6561 7465 6472 4c00 0000 7219 0000 0072  eatedrL...r....r
-00003a30: 1900 0000 721a 0000 00da 1c67 6574 5f70  ....r......get_p
-00003a40: 7374 5f64 6174 655f 6d65 7373 6167 655f  st_date_message_
-00003a50: 6372 6561 7465 64e0 0100 0073 0200 0000  created....s....
-00003a60: 0002 7a28 4865 6c70 4d65 7373 6167 652e  ..z(HelpMessage.
-00003a70: 6765 745f 7073 745f 6461 7465 5f6d 6573  get_pst_date_mes
-00003a80: 7361 6765 5f63 7265 6174 6564 721c 0000  sage_createdr...
-00003a90: 0072 2400 0000 6302 0000 0000 0000 0000  .r$...c.........
-00003aa0: 0000 0002 0000 0002 0000 0043 0000 0173  ...........C...s
-00003ab0: 0c00 0000 7c01 a000 a100 0100 6401 5300  ....|.......d.S.
-00003ac0: 2902 7a1f 4164 6473 2065 6e74 7279 2074  ).z.Adds entry t
-00003ad0: 6f20 4865 6c70 4d65 7373 6167 6520 7461  o HelpMessage ta
-00003ae0: 626c 654e 7226 0000 0072 2800 0000 7219  bleNr&...r(...r.
-00003af0: 0000 0072 1900 0000 721a 0000 0072 2900  ...r....r....r).
-00003b00: 0000 e401 0000 7302 0000 0000 047a 1948  ......s......z.H
-00003b10: 656c 704d 6573 7361 6765 2e69 6e73 6572  elpMessage.inser
-00003b20: 745f 7265 636f 7264 6302 0000 0000 0000  t_recordc.......
-00003b30: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-00003b40: 0173 0c00 0000 7c01 a000 a100 0100 6400  .s....|.......d.
-00003b50: 5300 724f 0000 0072 ca00 0000 2902 7222  S.rO...r....).r"
-00003b60: 0000 005a 1d68 656c 705f 6d65 7373 6167  ...Z.help_messag
-00003b70: 655f 7265 636f 7264 5f74 6f5f 6465 6c65  e_record_to_dele
-00003b80: 7465 7219 0000 0072 1900 0000 721a 0000  ter....r....r...
-00003b90: 00da 0e64 656c 6574 655f 6d65 7373 6167  ...delete_messag
-00003ba0: 65ea 0100 0073 0200 0000 0003 7a1a 4865  e....s......z.He
-00003bb0: 6c70 4d65 7373 6167 652e 6465 6c65 7465  lpMessage.delete
-00003bc0: 5f6d 6573 7361 6765 6301 0000 0000 0000  _messagec.......
-00003bd0: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
-00003be0: 0173 2400 0000 7400 7401 6a02 a003 a100  .s$...t.t.j.....
-00003bf0: 6a04 7405 7406 6a06 a007 a100 8301 a008  j.t.t.j.........
-00003c00: a100 6401 8d01 8301 5300 2902 4e29 015a  ..d.....S.).N).Z
-00003c10: 2168 656c 705f 6d65 7373 6167 655f 6578  !help_message_ex
-00003c20: 7069 7261 7469 6f6e 5f64 6174 655f 5f6c  piration_date__l
-00003c30: 7465 2909 722e 0000 0072 d400 0000 7220  te).r....r....r 
-00003c40: 0000 0072 4300 0000 7230 0000 0072 d500  ...rC...r0...r..
-00003c50: 0000 723c 0000 0072 3d00 0000 723e 0000  ..r<...r=...r>..
-00003c60: 0072 3100 0000 7219 0000 0072 1900 0000  .r1...r....r....
-00003c70: 721a 0000 00da 1667 6574 5f6d 6573 7361  r......get_messa
-00003c80: 6765 735f 746f 5f64 656c 6574 65ef 0100  ges_to_delete...
-00003c90: 0073 0a00 0000 0003 0201 0a01 10ff 04ff  .s..............
-00003ca0: 7a22 4865 6c70 4d65 7373 6167 652e 6765  z"HelpMessage.ge
-00003cb0: 745f 6d65 7373 6167 6573 5f74 6f5f 6465  t_messages_to_de
-00003cc0: 6c65 7465 6301 0000 0000 0000 0000 0000  letec...........
-00003cd0: 0003 0000 0004 0000 000f 0000 0173 3a00  .............s:.
-00003ce0: 0000 7400 7401 6a01 a002 a100 8301 7401  ..t.t.j.......t.
-00003cf0: 6a03 6401 6402 8d01 1700 a004 a100 7c00  j.d.d.........|.
-00003d00: 5f05 7406 7407 7c00 8302 6a08 7c01 6900  _.t.t.|...j.|.i.
-00003d10: 7c02 a401 8e01 0100 6400 5300 2903 4e72  |.......d.S.).Nr
-00003d20: 0b00 0000 72a3 0000 0029 0972 d500 0000  ....r....).r....
-00003d30: 723c 0000 0072 3d00 0000 72a8 0000 0072  r<...r=...r....r
-00003d40: 3e00 0000 72d6 0000 0072 7500 0000 72d4  >...r....ru...r.
-00003d50: 0000 0072 2700 0000 7276 0000 0072 7900  ...r'...rv...ry.
-00003d60: 0000 7219 0000 0072 1a00 0000 7227 0000  ..r....r....r'..
-00003d70: 00f8 0100 0073 0600 0000 0002 18ff 0803  .....s..........
-00003d80: 7a10 4865 6c70 4d65 7373 6167 652e 7361  z.HelpMessage.sa
-00003d90: 7665 6301 0000 0000 0000 0000 0000 0001  vec.............
-00003da0: 0000 000c 0000 0043 0000 0173 3400 0000  .......C...s4...
-00003db0: 6401 7c00 6a00 9b00 6402 7c00 6a01 9b00  d.|.j...d.|.j...
-00003dc0: 6403 7c00 6a02 9b00 6404 7c00 6a03 9b00  d.|.j...d.|.j...
-00003dd0: 6405 7c00 6a04 a005 6406 a101 9b00 6407  d.|.j...d.....d.
-00003de0: 9d0b 5300 2908 4e7a 0d5b 4865 6c70 4d65  ..S.).Nz.[HelpMe
-00003df0: 7373 6167 6520 7a0e 2066 6f72 2063 6861  ssage z. for cha
-00003e00: 6e6e 656c 2023 fa01 287a 0e29 2061 6e64  nnel #..(z.) and
-00003e10: 206d 6573 7361 6765 207a 1520 7468 6174   message z. that
-00003e20: 2077 6173 2063 7265 6174 6564 206f 6e20   was created on 
-00003e30: 7a18 2559 2025 6220 252d 6420 2549 3a25  z.%Y %b %-d %I:%
-00003e40: 4d3a 2553 2025 7020 255a 7246 0000 0029  M:%S %p %ZrF...)
-00003e50: 0672 5000 0000 727d 0000 00da 0a63 6861  .rP...r}.....cha
-00003e60: 6e6e 656c 5f69 64da 0a6d 6573 7361 6765  nnel_id..message
-00003e70: 5f69 6472 d900 0000 da08 7374 7266 7469  _idr......strfti
-00003e80: 6d65 724c 0000 0072 1900 0000 7219 0000  merL...r....r...
-00003e90: 0072 1a00 0000 724e 0000 00fe 0100 0073  .r....rN.......s
-00003ea0: 0c00 0000 0002 1a01 04ff 0402 0afe 06ff  ................
-00003eb0: 7a13 4865 6c70 4d65 7373 6167 652e 5f5f  z.HelpMessage.__
-00003ec0: 7374 725f 5f29 1872 1500 0000 7216 0000  str__).r....r...
-00003ed0: 0072 1700 0000 7206 0000 0072 7b00 0000  .r....r....r{...
-00003ee0: 7250 0000 0072 5300 0000 72de 0000 0072  rP...rS...r....r
-00003ef0: 5200 0000 727d 0000 0072 dd00 0000 72d6  R...r}...r....r.
-00003f00: 0000 0072 d800 0000 72b3 0000 0072 d700  ...r....r....r..
-00003f10: 0000 72d9 0000 0072 5400 0000 7204 0000  ..r....rT...r...
-00003f20: 0072 2900 0000 72da 0000 0072 db00 0000  .r)...r....r....
-00003f30: 7227 0000 0072 4e00 0000 727e 0000 0072  r'...rN...r~...r
-00003f40: 1900 0000 7219 0000 0072 7900 0000 721a  ....r....ry...r.
-00003f50: 0000 0072 d400 0000 d401 0000 732a 0000  ...r........s*..
-00003f60: 0008 010c 010c 0110 010c 010c 010c 0202  ................
-00003f70: 010a 0302 010a 0302 0102 0114 0402 0102  ................
-00003f80: 010c 0302 0102 010c 070c 0672 d400 0000  ...........r....
-00003f90: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00003fa0: 0003 0000 0043 0000 0173 0a00 0000 7c00  .....C...s....|.
-00003fb0: a000 7401 a101 5300 2901 7ae8 0a20 2020  ..t...S.).z..   
-00003fc0: 2043 6f6e 7665 7274 2074 6865 2067 6976   Convert the giv
-00003fd0: 656e 2055 5443 2074 696d 657a 6f6e 6520  en UTC timezone 
-00003fe0: 6f62 6a65 6374 2074 6f20 6120 5053 5420  object to a PST 
-00003ff0: 7469 6d65 7a6f 6e65 206f 626a 6563 740a  timezone object.
-00004000: 0a20 2020 204b 6579 776f 7264 2041 7267  .    Keyword Arg
-00004010: 756d 656e 7473 0a20 2020 2075 7463 5f64  uments.    utc_d
-00004020: 6174 6574 696d 6520 2d2d 2074 6865 2067  atetime -- the g
-00004030: 6976 656e 2055 5443 2074 696d 657a 6f6e  iven UTC timezon
-00004040: 6520 6f62 6a65 6374 2074 6f20 636f 6e76  e object to conv
-00004050: 6572 740a 0a20 2020 2052 6574 7572 6e0a  ert..    Return.
-00004060: 2020 2020 6461 7465 7469 6d65 202d 2d20      datetime -- 
-00004070: 7468 6520 5053 5420 7469 6d65 7a6f 6e65  the PST timezone
-00004080: 2065 7175 6976 616c 656e 7420 6f66 2074   equivalent of t
-00004090: 6865 2075 7463 5f64 6174 6574 696d 650a  he utc_datetime.
-000040a0: 2020 2020 2902 da0a 6173 7469 6d65 7a6f      )...astimezo
-000040b0: 6e65 da0a 5041 4349 4649 435f 545a 2901  ne..PACIFIC_TZ).
-000040c0: 5a0c 7574 635f 6461 7465 7469 6d65 7219  Z.utc_datetimer.
-000040d0: 0000 0072 1900 0000 721a 0000 0072 d500  ...r....r....r..
-000040e0: 0000 0602 0000 7302 0000 0000 0a72 d500  ......s......r..
-000040f0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00004100: 0000 0005 0000 0040 0000 0173 4c00 0000  .......@...sL...
-00004110: 6500 5a01 6400 5a02 6503 6a04 6401 6402  e.Z.d.Z.e.j.d.d.
-00004120: 8d01 5a05 6503 6a04 6401 6402 8d01 5a06  ..Z.e.j.d.d...Z.
-00004130: 6507 6508 6400 6403 6404 9c02 6405 6406  e.e.d.d.d...d.d.
-00004140: 8404 8301 8301 5a09 6507 6508 6407 6408  ......Z.e.e.d.d.
-00004150: 8400 8301 8301 5a0a 6409 5300 290a da0b  ......Z.d.S.)...
-00004160: 456d 6265 6441 7661 7461 7269 8813 0000  EmbedAvatari....
-00004170: 725a 0000 0072 1c00 0000 7224 0000 0063  rZ...r....r$...c
-00004180: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00004190: 0200 0000 4300 0001 730c 0000 007c 01a0  ....C...s....|..
-000041a0: 00a1 0001 0064 0153 0029 027a 1f41 6464  .....d.S.).z.Add
-000041b0: 7320 656e 7472 7920 746f 2045 6d62 6564  s entry to Embed
-000041c0: 4176 6174 6172 2074 6162 6c65 4e72 2600  Avatar tableNr&.
-000041d0: 0000 7228 0000 0072 1900 0000 7219 0000  ..r(...r....r...
-000041e0: 0072 1a00 0000 7229 0000 001b 0200 0073  .r....r).......s
-000041f0: 0200 0000 0004 7a19 456d 6265 6441 7661  ......z.EmbedAva
-00004200: 7461 722e 696e 7365 7274 5f72 6563 6f72  tar.insert_recor
-00004210: 6463 0200 0000 0000 0000 0000 0000 0300  dc..............
-00004220: 0000 0300 0000 4300 0001 732e 0000 0074  ......C...s....t
-00004230: 006a 01a0 02a1 006a 037c 0164 018d 017d  .j.....j.|.d...}
-00004240: 0274 047c 0283 0164 026b 0272 2264 0053  .t.|...d.k.r"d.S
-00004250: 007c 0264 0219 0053 0064 0053 0029 034e  .|.d...S.d.S.).N
-00004260: 2901 da12 6176 6174 6172 5f64 6973 636f  )...avatar_disco
-00004270: 7264 5f75 726c 7201 0000 0029 0572 e200  rd_urlr....).r..
-00004280: 0000 7220 0000 0072 4300 0000 7230 0000  ..r ...rC...r0..
-00004290: 0072 6900 0000 2903 7222 0000 00da 0375  .ri...).r".....u
-000042a0: 726c 5a07 6176 6174 6172 7372 1900 0000  rlZ.avatarsr....
-000042b0: 7219 0000 0072 1a00 0000 da11 6765 745f  r....r......get_
-000042c0: 6176 6174 6172 5f62 795f 7572 6c21 0200  avatar_by_url!..
-000042d0: 0073 0800 0000 0003 1201 0c01 0402 7a1d  .s............z.
-000042e0: 456d 6265 6441 7661 7461 722e 6765 745f  EmbedAvatar.get_
-000042f0: 6176 6174 6172 5f62 795f 7572 6c4e 290b  avatar_by_urlN).
-00004300: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00004310: 0600 0000 7252 0000 0072 e300 0000 5a1c  ....rR...r....Z.
-00004320: 6176 6174 6172 5f64 6973 636f 7264 5f70  avatar_discord_p
-00004330: 6572 6d61 6e65 6e74 5f75 726c 7254 0000  ermanent_urlrT..
-00004340: 0072 0400 0000 7229 0000 0072 e500 0000  .r....r)...r....
-00004350: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-00004360: 1a00 0000 72e2 0000 0013 0200 0073 1800  ....r........s..
-00004370: 0000 0801 0401 02ff 0603 0401 02ff 0604  ................
-00004380: 0201 0201 1404 0201 0201 72e2 0000 0029  ..........r....)
-00004390: 23da 0a5f 5f66 7574 7572 655f 5f72 0200  #..__future__r..
-000043a0: 0000 da06 7479 7069 6e67 7203 0000 0072  ....typingr....r
-000043b0: 3c00 0000 7296 0000 0072 d100 0000 72a6  <...r....r....r.
-000043c0: 0000 00da 0c61 7367 6972 6566 2e73 796e  .....asgiref.syn
-000043d0: 6372 0400 0000 da0b 646a 616e 676f 2e63  cr......django.c
-000043e0: 6f6e 6672 0500 0000 da09 646a 616e 676f  onfr......django
-000043f0: 2e64 6272 0600 0000 5a0c 646a 616e 676f  .dbr....Z.django
-00004400: 2e66 6f72 6d73 7207 0000 00da 0c64 6a61  .formsr......dja
-00004410: 6e67 6f2e 7574 696c 7372 0800 0000 5a0b  ngo.utilsr....Z.
-00004420: 6461 7465 7574 696c 2e74 7a72 0a00 0000  dateutil.tzr....
-00004430: 72a7 0000 005a 0567 6574 747a 72e1 0000  r....Z.gettzr...
-00004440: 005a 0c63 7573 746f 6d46 6965 6c64 7372  .Z.customFieldsr
-00004450: 0c00 0000 72ab 0000 00da 054d 6f64 656c  ....r......Model
-00004460: 720d 0000 0072 5500 0000 727f 0000 0072  r....rU...r....r
-00004470: 8f00 0000 72be 0000 0072 d400 0000 72d5  ....r....r....r.
-00004480: 0000 0072 e200 0000 7219 0000 0072 1900  ...r....r....r..
-00004490: 0000 7219 0000 0072 1a00 0000 da08 3c6d  ..r....r......<m
-000044a0: 6f64 756c 653e 0300 0000 7330 0000 000c  odule>....s0....
-000044b0: 020c 0108 0108 0108 0108 010c 010c 010c  ................
-000044c0: 010c 010c 010c 0304 010a 020c 0108 0312  ................
-000044d0: 4a12 5112 7f00 0112 4712 5912 3208 0d    J.Q.....G.Y.2..
+00000330: 9c01 6424 6425 8404 5a19 6408 5300 2926  ..d$d%..Z.d.S.)&
+00000340: da09 4261 6e52 6563 6f72 6454 a901 da0b  ..BanRecordT....
+00000350: 7072 696d 6172 795f 6b65 79e9 2500 0000  primary_key.%...
+00000360: 4629 02da 0a6d 6178 5f6c 656e 6774 68da  F)...max_length.
+00000370: 046e 756c 6ca9 0172 1200 0000 6900 0200  .null..r....i...
+00000380: 004e 2902 7212 0000 00da 0764 6566 6175  .N).r......defau
+00000390: 6c74 6300 0000 0000 0000 0000 0000 0000  ltc.............
+000003a0: 0000 0001 0000 0040 0000 0173 1000 0000  .......@...s....
+000003b0: 6500 5a01 6400 5a02 6401 5a03 6402 5300  e.Z.d.Z.d.Z.d.S.
+000003c0: 2903 7a0e 4261 6e52 6563 6f72 642e 4d65  ).z.BanRecord.Me
+000003d0: 7461 5a19 7761 6c6c 5f65 5f6d 6f64 656c  taZ.wall_e_model
+000003e0: 735f 6261 6e5f 7265 636f 7264 734e 2904  s_ban_recordsN).
+000003f0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000400: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000410: 6d65 5f5f da08 6462 5f74 6162 6c65 a900  me__..db_table..
+00000420: 7219 0000 0072 1900 0000 fa44 2f6d 6564  r....r.....D/med
+00000430: 6961 2f6a 6163 652f 6a61 6365 5f64 6f63  ia/jace/jace_doc
+00000440: 732f 315f 4353 5353 2f32 5f77 616c 6c5f  s/1_CSSS/2_wall_
+00000450: 655f 6d6f 6465 6c73 2f77 616c 6c5f 655f  e_models/wall_e_
+00000460: 6d6f 6465 6c73 2f6d 6f64 656c 732e 7079  models/models.py
+00000470: da04 4d65 7461 2300 0000 7302 0000 0008  ..Meta#...s.....
+00000480: 0172 1b00 0000 7a0f 4c69 7374 5b42 616e  .r....z.List[Ban
+00000490: 5265 636f 7264 5dda 044e 6f6e 6529 02da  Record]..None)..
+000004a0: 0772 6563 6f72 6473 da06 7265 7475 726e  .records..return
+000004b0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+000004c0: 0003 0000 0043 0000 0173 1000 0000 7400  .....C...s....t.
+000004d0: 6a01 a002 7c01 a101 0100 6401 5300 a902  j...|.....d.S...
+000004e0: 7a1d 4164 6473 2065 6e74 7279 2074 6f20  z.Adds entry to 
+000004f0: 4261 6e52 6563 6f72 6420 7461 626c 654e  BanRecord tableN
+00000500: 2903 720d 0000 00da 076f 626a 6563 7473  ).r......objects
+00000510: da0b 6275 6c6b 5f63 7265 6174 6529 02da  ..bulk_create)..
+00000520: 0363 6c73 721d 0000 0072 1900 0000 7219  .clsr....r....r.
+00000530: 0000 0072 1a00 0000 da0e 696e 7365 7274  ...r......insert
+00000540: 5f72 6563 6f72 6473 2600 0000 7302 0000  _records&...s...
+00000550: 0000 047a 1842 616e 5265 636f 7264 2e69  ...z.BanRecord.i
+00000560: 6e73 6572 745f 7265 636f 7264 73a9 02da  nsert_records...
+00000570: 0672 6563 6f72 6472 1e00 0000 6302 0000  .recordr....c...
+00000580: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+00000590: 0043 0000 0173 0c00 0000 7c01 a000 a100  .C...s....|.....
+000005a0: 0100 6401 5300 721f 0000 00a9 01da 0473  ..d.S.r........s
+000005b0: 6176 65a9 0272 2200 0000 7225 0000 0072  ave..r"...r%...r
+000005c0: 1900 0000 7219 0000 0072 1a00 0000 da0d  ....r....r......
+000005d0: 696e 7365 7274 5f72 6563 6f72 642c 0000  insert_record,..
+000005e0: 0073 0200 0000 0004 7a17 4261 6e52 6563  .s......z.BanRec
+000005f0: 6f72 642e 696e 7365 7274 5f72 6563 6f72  ord.insert_recor
+00000600: 647a 094c 6973 745b 696e 745d 2901 721e  dz.List[int]).r.
+00000610: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000620: 0100 0000 0500 0000 4300 0001 731c 0000  ........C...s...
+00000630: 0074 0074 016a 026a 0364 0164 0264 038d  .t.t.j.j.d.d.d..
+00000640: 026a 0464 0464 058d 0183 0153 0029 067a  .j.d.d.....S.).z
+00000650: 3752 6574 7572 6e73 206c 6973 7420 6f66  7Returns list of
+00000660: 2075 7365 725f 6964 7320 666f 7220 616c   user_ids for al
+00000670: 6c20 6375 7272 656e 746c 7920 6261 6e6e  l currently bann
+00000680: 6564 2075 7365 7273 da07 7573 6572 5f69  ed users..user_i
+00000690: 6454 2901 da04 666c 6174 4ea9 01da 0a75  dT)...flatN....u
+000006a0: 6e62 616e 5f64 6174 6529 05da 046c 6973  nban_date)...lis
+000006b0: 7472 0d00 0000 7220 0000 00da 0b76 616c  tr....r .....val
+000006c0: 7565 735f 6c69 7374 da06 6669 6c74 6572  ues_list..filter
+000006d0: a901 7222 0000 0072 1900 0000 7219 0000  ..r"...r....r...
+000006e0: 0072 1a00 0000 da1b 6765 745f 616c 6c5f  .r......get_all_
+000006f0: 6163 7469 7665 5f62 616e 5f75 7365 725f  active_ban_user_
+00000700: 6964 7332 0000 0073 0200 0000 0005 7a25  ids2...s......z%
+00000710: 4261 6e52 6563 6f72 642e 6765 745f 616c  BanRecord.get_al
+00000720: 6c5f 6163 7469 7665 5f62 616e 5f75 7365  l_active_ban_use
+00000730: 725f 6964 7363 0100 0000 0000 0000 0000  r_idsc..........
+00000740: 0000 0100 0000 0500 0000 4300 0001 731a  ..........C...s.
+00000750: 0000 0074 0074 016a 02a0 0364 0164 02a1  ...t.t.j...d.d..
+00000760: 026a 0464 0364 048d 0183 0153 0029 057a  .j.d.d.....S.).z
+00000770: 4552 6574 7572 6e73 206c 6973 7420 6f66  EReturns list of
+00000780: 2075 7365 726e 616d 6573 2061 6e64 2075   usernames and u
+00000790: 7365 725f 6964 7320 666f 7220 616c 6c20  ser_ids for all 
+000007a0: 6375 7272 656e 746c 7920 6261 6e6e 6564  currently banned
+000007b0: 2075 7365 7273 da08 7573 6572 6e61 6d65   users..username
+000007c0: 722a 0000 004e 722c 0000 0029 0572 2e00  r*...Nr,...).r..
+000007d0: 0000 720d 0000 0072 2000 0000 da06 7661  ..r....r .....va
+000007e0: 6c75 6573 7230 0000 0072 3100 0000 7219  luesr0...r1...r.
+000007f0: 0000 0072 1900 0000 721a 0000 00da 1367  ...r....r......g
+00000800: 6574 5f61 6c6c 5f61 6374 6976 655f 6261  et_all_active_ba
+00000810: 6e73 3900 0000 7302 0000 0000 057a 1d42  ns9...s......z.B
+00000820: 616e 5265 636f 7264 2e67 6574 5f61 6c6c  anRecord.get_all
+00000830: 5f61 6374 6976 655f 6261 6e73 da03 696e  _active_bans..in
+00000840: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
+00000850: 0000 0300 0000 4300 0001 7312 0000 0074  ......C...s....t
+00000860: 006a 016a 0264 0164 028d 01a0 03a1 0053  .j.j.d.d.......S
+00000870: 0029 037a 2452 6574 7572 6e73 2063 6f75  .).z$Returns cou
+00000880: 6e74 206f 6620 616c 6c20 7468 6520 6163  nt of all the ac
+00000890: 7469 7665 2062 616e 734e 722c 0000 0029  tive bansNr,...)
+000008a0: 0472 0d00 0000 7220 0000 0072 3000 0000  .r....r ...r0...
+000008b0: da05 636f 756e 7472 3100 0000 7219 0000  ..countr1...r...
+000008c0: 0072 1900 0000 721a 0000 00da 1567 6574  .r....r......get
+000008d0: 5f61 6374 6976 655f 6261 6e73 5f63 6f75  _active_bans_cou
+000008e0: 6e74 4000 0000 7302 0000 0000 057a 1f42  nt@...s......z.B
+000008f0: 616e 5265 636f 7264 2e67 6574 5f61 6374  anRecord.get_act
+00000900: 6976 655f 6261 6e73 5f63 6f75 6e74 da03  ive_bans_count..
+00000910: 7374 7229 0272 2a00 0000 721e 0000 0063  str).r*...r....c
+00000920: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00000930: 0800 0000 4300 0001 7348 0000 007a 1474  ....C...sH...z.t
+00000940: 006a 016a 027c 0164 0164 028d 027d 0257  .j.j.|.d.d...}.W
+00000950: 006e 1404 0074 0379 2801 0001 0001 0059  .n...t.y(......Y
+00000960: 0064 0153 0030 0074 046a 04a0 05a1 00a0  .d.S.0.t.j......
+00000970: 06a1 007c 025f 077c 02a0 08a1 0001 007c  ...|._.|.......|
+00000980: 026a 0953 0029 037a 5453 6574 2061 6374  .j.S.).zTSet act
+00000990: 6976 653d 4661 6c73 6520 666f 7220 7573  ive=False for us
+000009a0: 6572 2077 6974 6820 7468 6520 6769 7665  er with the give
+000009b0: 6e20 7573 6572 5f69 642e 2054 6869 7320  n user_id. This 
+000009c0: 7265 7072 6573 656e 7465 7320 756e 6261  representes unba
+000009d0: 6e6e 696e 6720 6120 7573 6572 2e4e 2902  nning a user.N).
+000009e0: 722a 0000 0072 2d00 0000 290a 720d 0000  r*...r-...).r...
+000009f0: 0072 2000 0000 da03 6765 74da 0945 7863  .r .....get..Exc
+00000a00: 6570 7469 6f6e da08 6461 7465 7469 6d65  eption..datetime
+00000a10: da03 6e6f 77da 0974 696d 6573 7461 6d70  ..now..timestamp
+00000a20: 722d 0000 0072 2700 0000 7233 0000 0029  r-...r'...r3...)
+00000a30: 0372 2200 0000 722a 0000 00da 0475 7365  .r"...r*.....use
+00000a40: 7272 1900 0000 7219 0000 0072 1a00 0000  rr....r....r....
+00000a50: da0b 756e 6261 6e5f 6279 5f69 6447 0000  ..unban_by_idG..
+00000a60: 0073 0e00 0000 0004 0201 1401 0c01 0802  .s..............
+00000a70: 1001 0801 7a15 4261 6e52 6563 6f72 642e  ....z.BanRecord.
+00000a80: 756e 6261 6e5f 6279 5f69 64da 0462 6f6f  unban_by_id..boo
+00000a90: 6c63 0200 0000 0000 0000 0000 0000 0200  lc..............
+00000aa0: 0000 0300 0000 4300 0001 731a 0000 0074  ......C...s....t
+00000ab0: 006a 01a0 02a1 006a 037c 0164 018d 01a0  .j.....j.|.d....
+00000ac0: 04a1 0064 0075 0153 0029 024e a901 722a  ...d.u.S.).N..r*
+00000ad0: 0000 0029 0572 0d00 0000 7220 0000 00da  ...).r....r ....
+00000ae0: 0361 6c6c 7230 0000 00da 0566 6972 7374  .allr0.....first
+00000af0: 2902 7222 0000 0072 2a00 0000 7219 0000  ).r"...r*...r...
+00000b00: 0072 1900 0000 721a 0000 00da 0e75 7365  .r....r......use
+00000b10: 725f 6973 5f62 616e 6e65 6454 0000 0073  r_is_bannedT...s
+00000b20: 0200 0000 0003 7a18 4261 6e52 6563 6f72  ......z.BanRecor
+00000b30: 642e 7573 6572 5f69 735f 6261 6e6e 6564  d.user_is_banned
+00000b40: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000b50: 0011 0000 0043 0000 0173 4600 0000 6401  .....C...sF...d.
+00000b60: 7c00 6a00 9b00 6402 7c00 6a01 9b00 6403  |.j...d.|.j...d.
+00000b70: 7c00 6a02 9b00 6404 7c00 6a03 9b00 6405  |.j...d.|.j...d.
+00000b80: 7c00 6a04 9b00 6406 7c00 6a05 9b00 6407  |.j...d.|.j...d.
+00000b90: 7c00 6a06 9b00 6408 7c00 6a07 9b00 6409  |.j...d.|.j...d.
+00000ba0: 9d11 5300 290a 4e7a 0862 616e 5f69 643d  ..S.).Nz.ban_id=
+00000bb0: 5b7a 0c5d 2075 7365 726e 616d 653d 5b7a  [z.] username=[z
+00000bc0: 0b5d 2075 7365 725f 6964 3d5b 7a07 5d20  .] user_id=[z.] 
+00000bd0: 6d6f 643d 5b7a 0a5d 206d 6f64 5f69 643d  mod=[z.] mod_id=
+00000be0: 5b7a 085d 2064 6174 653d 5b7a 0a5d 2072  [z.] date=[z.] r
+00000bf0: 6561 736f 6e3d 5b7a 0d5d 756e 6261 6e5f  eason=[z.]unban_
+00000c00: 6461 7465 3d5b fa01 5d29 08da 0662 616e  date=[..])...ban
+00000c10: 5f69 6472 3300 0000 722a 0000 00da 036d  _idr3...r*.....m
+00000c20: 6f64 da06 6d6f 645f 6964 da08 6261 6e5f  od..mod_id..ban_
+00000c30: 6461 7465 da06 7265 6173 6f6e 722d 0000  date..reasonr-..
+00000c40: 00a9 01da 0473 656c 6672 1900 0000 7219  .....selfr....r.
+00000c50: 0000 0072 1a00 0000 da07 5f5f 7374 725f  ...r......__str_
+00000c60: 5f59 0000 0073 1600 0000 0001 1a01 04ff  _Y...s..........
+00000c70: 0401 04ff 0401 04ff 0401 04ff 0402 04fe  ................
+00000c80: 7a11 4261 6e52 6563 6f72 642e 5f5f 7374  z.BanRecord.__st
+00000c90: 725f 5f29 1a72 1500 0000 7216 0000 0072  r__).r....r....r
+00000ca0: 1700 0000 720c 0000 0072 4700 0000 7206  ....r....rG...r.
+00000cb0: 0000 00da 0943 6861 7246 6965 6c64 7233  .....CharFieldr3
+00000cc0: 0000 00da 0f42 6967 496e 7465 6765 7246  .....BigIntegerF
+00000cd0: 6965 6c64 722a 0000 0072 4800 0000 7249  ieldr*...rH...rI
+00000ce0: 0000 0072 4a00 0000 724b 0000 0072 2d00  ...rJ...rK...r-.
+00000cf0: 0000 721b 0000 00da 0b63 6c61 7373 6d65  ..r......classme
+00000d00: 7468 6f64 7204 0000 0072 2300 0000 7229  thodr....r#...r)
+00000d10: 0000 0072 3200 0000 7235 0000 0072 3800  ...r2...r5...r8.
+00000d20: 0000 7240 0000 0072 4500 0000 724e 0000  ..r@...rE...rN..
+00000d30: 0072 1900 0000 7219 0000 0072 1900 0000  .r....r....r....
+00000d40: 721a 0000 0072 0d00 0000 1900 0000 733e  r....r........s>
+00000d50: 0000 0008 010a 010e 010c 010e 010c 010c  ................
+00000d60: 010e 010e 020e 0302 0102 0114 0402 0102  ................
+00000d70: 0114 0402 0102 0112 0502 0102 0112 0502  ................
+00000d80: 0102 0112 0502 0102 0114 0b02 0102 0112  ................
+00000d90: 0372 0d00 0000 6300 0000 0000 0000 0000  .r....c.........
+00000da0: 0000 0000 0000 0005 0000 0000 0000 0173  ...............s
+00000db0: d800 0000 6500 5a01 6400 5a02 6503 6a04  ....e.Z.d.Z.e.j.
+00000dc0: 6401 6402 8d01 5a05 6503 6a06 6507 6a08  d.d...Z.e.j.e.j.
+00000dd0: 6403 8d01 5a09 6503 6a06 6507 6a08 6403  d...Z.e.j.e.j.d.
+00000de0: 8d01 5a0a 6503 6a06 6507 6a08 6403 8d01  ..Z.e.j.e.j.d...
+00000df0: 5a0b 6503 6a06 6507 6a08 6403 8d01 5a0c  Z.e.j.e.j.d...Z.
+00000e00: 6503 6a0d 6404 6405 6406 8d02 5a0e 6503  e.j.d.d.d...Z.e.
+00000e10: 6a0d 6404 6407 8d01 5a0f 6503 6a0d 6404  j.d.d...Z.e.j.d.
+00000e20: 6407 8d01 5a10 6503 6a0d 6404 6401 6401  d...Z.e.j.d.d.d.
+00000e30: 6408 8d03 5a11 6512 6409 640a 8400 8301  d...Z.e.d.d.....
+00000e40: 5a13 6512 6514 640b 640c 8400 8301 8301  Z.e.e.d.d.......
+00000e50: 5a15 6512 6514 640d 640e 8400 8301 8301  Z.e.e.d.d.......
+00000e60: 5a16 6512 6416 6410 6411 8401 8301 5a17  Z.e.d.d.d.....Z.
+00000e70: 6412 6413 8400 5a18 8700 6601 6414 6415  d.d...Z...f.d.d.
+00000e80: 8408 5a19 8700 0400 5a1a 5300 2917 da0b  ..Z.....Z.S.)...
+00000e90: 436f 6d6d 616e 6453 7461 7454 720e 0000  CommandStatTr...
+00000ea0: 00a9 0172 1400 0000 e9d0 0700 00da 024e  ...r...........N
+00000eb0: 41a9 0272 1100 0000 7214 0000 00a9 0172  A..r....r......r
+00000ec0: 1100 0000 2903 7211 0000 00da 0562 6c61  ....).r......bla
+00000ed0: 6e6b 7212 0000 0063 0100 0000 0000 0000  nkr....c........
+00000ee0: 0000 0000 0100 0000 0300 0000 4300 0001  ............C...
+00000ef0: 7312 0000 0064 0164 0284 0074 0074 0183  s....d.d...t.t..
+00000f00: 0144 0083 0153 0029 034e 6301 0000 0000  .D...S.).Nc.....
+00000f10: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
+00000f20: 0000 0173 1800 0000 6700 7c00 5d10 7d01  ...s....g.|.].}.
+00000f30: 7c01 6400 6b03 7204 7c01 9102 7104 5300  |.d.k.r.|...q.S.
+00000f40: 2901 da0a 6570 6f63 685f 7469 6d65 7219  )...epoch_timer.
+00000f50: 0000 0029 02da 022e 30da 036b 6579 7219  ...)....0..keyr.
+00000f60: 0000 0072 1900 0000 721a 0000 00da 0a3c  ...r....r......<
+00000f70: 6c69 7374 636f 6d70 3e80 0000 00f3 0000  listcomp>.......
+00000f80: 0000 7a40 436f 6d6d 616e 6453 7461 742e  ..z@CommandStat.
+00000f90: 6765 745f 636f 6c75 6d6e 5f68 6561 6465  get_column_heade
+00000fa0: 7273 5f66 726f 6d5f 6461 7461 6261 7365  rs_from_database
+00000fb0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00000fc0: 6f6d 703e 2902 7207 0000 0072 5200 0000  omp>).r....rR...
+00000fd0: 7231 0000 0072 1900 0000 7219 0000 0072  r1...r....r....r
+00000fe0: 1a00 0000 da20 6765 745f 636f 6c75 6d6e  ..... get_column
+00000ff0: 5f68 6561 6465 7273 5f66 726f 6d5f 6461  _headers_from_da
+00001000: 7461 6261 7365 7e00 0000 7302 0000 0000  tabase~...s.....
+00001010: 027a 2c43 6f6d 6d61 6e64 5374 6174 2e67  .z,CommandStat.g
+00001020: 6574 5f63 6f6c 756d 6e5f 6865 6164 6572  et_column_header
+00001030: 735f 6672 6f6d 5f64 6174 6162 6173 6563  s_from_databasec
+00001040: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001050: 0300 0000 4300 0001 730e 0000 0074 0074  ....C...s....t.t
+00001060: 016a 02a0 03a1 0083 0153 00a9 014e 2904  .j.......S...N).
+00001070: 722e 0000 0072 5200 0000 7220 0000 0072  r....rR...r ...r
+00001080: 4300 0000 7231 0000 0072 1900 0000 7219  C...r1...r....r.
+00001090: 0000 0072 1a00 0000 da0f 6765 745f 616c  ...r......get_al
+000010a0: 6c5f 656e 7472 6965 7382 0000 0073 0200  l_entries....s..
+000010b0: 0000 0003 7a1b 436f 6d6d 616e 6453 7461  ....z.CommandSta
+000010c0: 742e 6765 745f 616c 6c5f 656e 7472 6965  t.get_all_entrie
+000010d0: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
+000010e0: 0000 0800 0000 4300 0001 7336 0000 007a  ......C...s6...z
+000010f0: 0e7c 01a0 00a1 0001 0057 0064 0053 0004  .|.......W.d.S..
+00001100: 0074 0179 2e01 0001 0001 007c 0104 006a  .t.y.......|...j
+00001110: 0264 0137 0002 005f 0259 0071 0030 0071  .d.7..._.Y.q.0.q
+00001120: 0064 0053 00a9 024e 720b 0000 0029 0372  .d.S...Nr....).r
+00001130: 2700 0000 723b 0000 0072 5900 0000 2902  '...r;...rY...).
+00001140: 7222 0000 00da 0c63 6f6d 6d61 6e64 5f73  r".....command_s
+00001150: 7461 7472 1900 0000 7219 0000 0072 1a00  tatr....r....r..
+00001160: 0000 da11 7361 7665 5f63 6f6d 6d61 6e64  ....save_command
+00001170: 5f73 7461 7487 0000 0073 0a00 0000 0004  _stat....s......
+00001180: 0201 0801 0601 0c01 7a1d 436f 6d6d 616e  ........z.Comman
+00001190: 6453 7461 742e 7361 7665 5f63 6f6d 6d61  dStat.save_comma
+000011a0: 6e64 5f73 7461 744e 6302 0000 0000 0000  nd_statNc.......
+000011b0: 0000 0000 0007 0000 0005 0000 00c3 0000  ................
+000011c0: 0173 7400 0000 6900 7d02 7400 a001 a100  .st...i.}.t.....
+000011d0: 4900 6400 4800 4400 5d5c 7d03 7402 7c03  I.d.H.D.]\}.t.|.
+000011e0: 8301 7d03 6401 7d04 7403 7c01 8301 4400  ..}.d.}.t.|...D.
+000011f0: 5d2e 5c02 7d05 7d06 7c04 7c03 7c06 1900  ].\.}.}.|.|.|...
+00001200: 9b00 3700 7d04 7c05 6402 1700 7404 7c01  ..7.}.|.d...t.|.
+00001210: 8301 6b00 722a 7c04 6403 3700 7d04 712a  ..k.r*|.d.7.}.q*
+00001220: 7c02 a005 7c04 6404 a102 6402 1700 7c02  |...|.d...d...|.
+00001230: 7c04 3c00 7112 7c02 5300 2905 4eda 0072  |.<.q.|.S.).N..r
+00001240: 0b00 0000 fa01 2d72 0100 0000 2906 7252  ......-r....).rR
+00001250: 0000 0072 6000 0000 7207 0000 00da 0965  ...r`...r......e
+00001260: 6e75 6d65 7261 7465 da03 6c65 6e72 3a00  numerate..lenr:.
+00001270: 0000 2907 7222 0000 00da 0766 696c 7465  ..).r".....filte
+00001280: 7273 5a11 6669 6c74 6572 5f73 7461 7473  rsZ.filter_stats
+00001290: 5f64 6963 7472 6200 0000 725b 0000 00da  _dictrb...r[....
+000012a0: 0369 6478 5a0e 636f 6d6d 616e 645f 6669  .idxZ.command_fi
+000012b0: 6c74 6572 7219 0000 0072 1900 0000 721a  lterr....r....r.
+000012c0: 0000 00da 1667 6574 5f63 6f6d 6d61 6e64  .....get_command
+000012d0: 5f73 7461 7473 5f64 6963 7491 0000 0073  _stats_dict....s
+000012e0: 1400 0000 0002 0401 1201 0801 0401 1001  ................
+000012f0: 0e01 1001 0a01 1601 7a22 436f 6d6d 616e  ........z"Comman
+00001300: 6453 7461 742e 6765 745f 636f 6d6d 616e  dStat.get_comman
+00001310: 645f 7374 6174 735f 6469 6374 6301 0000  d_stats_dictc...
+00001320: 0000 0000 0000 0000 0001 0000 000d 0000  ................
+00001330: 0043 0000 0173 3a00 0000 7c00 6a00 9b00  .C...s:...|.j...
+00001340: 6401 7c00 6a01 9b00 6402 7c00 6a02 9b00  d.|.j...d.|.j...
+00001350: 6403 7c00 6a03 9b00 6404 7c00 6a04 9b00  d.|.j...d.|.j...
+00001360: 6405 7c00 6a05 9b00 6406 7c00 6a06 9b00  d.|.j...d.|.j...
+00001370: 9d0d 5300 2907 4e7a 0320 2d20 7a11 2061  ..S.).Nz. - z. a
+00001380: 7320 696e 766f 6b65 6420 7769 7468 207a  s invoked with z
+00001390: 1120 7769 7468 2073 7562 636f 6d6d 616e  . with subcomman
+000013a0: 6420 7a0a 2061 6e64 2079 6561 7220 7a08  d z. and year z.
+000013b0: 2c20 6d6f 6e74 6820 7a0a 2061 6e64 2068  , month z. and h
+000013c0: 6f75 7220 2907 7259 0000 00da 0763 6f6d  our ).rY.....com
+000013d0: 6d61 6e64 da0c 696e 766f 6b65 645f 7769  mand..invoked_wi
+000013e0: 7468 da12 696e 766f 6b65 645f 7375 6263  th..invoked_subc
+000013f0: 6f6d 6d61 6e64 da04 7965 6172 da05 6d6f  ommand..year..mo
+00001400: 6e74 68da 0468 6f75 7272 4c00 0000 7219  nth..hourrL...r.
+00001410: 0000 0072 1900 0000 721a 0000 0072 4e00  ...r....r....rN.
+00001420: 0000 9e00 0000 7314 0000 0000 0218 0104  ......s.........
+00001430: ff04 0104 ff04 0204 fe04 0204 fe04 ff7a  ...............z
+00001440: 1343 6f6d 6d61 6e64 5374 6174 2e5f 5f73  .CommandStat.__s
+00001450: 7472 5f5f 6301 0000 0000 0000 0000 0000  tr__c...........
+00001460: 0003 0000 0004 0000 000f 0000 0173 8200  .............s..
+00001470: 0000 7400 7c00 6a01 8301 7402 6a02 6b02  ..t.|.j...t.j.k.
+00001480: 721a 7c00 6a01 6a01 7c00 5f01 7400 7c00  r.|.j.j.|._.t.|.
+00001490: 6a03 8301 7402 6a02 6b02 7234 7c00 6a03  j...t.j.k.r4|.j.
+000014a0: 6a03 7c00 5f03 7400 7c00 6a04 8301 7402  j.|._.t.|.j...t.
+000014b0: 6a02 6b02 724e 7c00 6a04 6a04 7c00 5f04  j.k.rN|.j.j.|._.
+000014c0: 7400 7c00 6a05 8301 7402 6a02 6b02 7268  t.|.j...t.j.k.rh
+000014d0: 7c00 6a05 6a05 7c00 5f05 7406 7407 7c00  |.j.j.|._.t.t.|.
+000014e0: 8302 6a08 7c01 6900 7c02 a401 8e01 0100  ..j.|.i.|.......
+000014f0: 6400 5300 725f 0000 0029 09da 0474 7970  d.S.r_...)...typ
+00001500: 6572 6e00 0000 723c 0000 0072 6f00 0000  ern...r<...ro...
+00001510: da03 6461 7972 7000 0000 da05 7375 7065  ..dayrp.....supe
+00001520: 7272 5200 0000 7227 0000 00a9 0372 4d00  rrR...r'.....rM.
+00001530: 0000 da04 6172 6773 da06 6b77 6172 6773  ....args..kwargs
+00001540: a901 da09 5f5f 636c 6173 735f 5f72 1900  ....__class__r..
+00001550: 0000 721a 0000 0072 2700 0000 a400 0000  ..r....r'.......
+00001560: 7312 0000 0000 0110 010a 0110 010a 0110  s...............
+00001570: 010a 0110 010a 017a 1043 6f6d 6d61 6e64  .......z.Command
+00001580: 5374 6174 2e73 6176 6529 014e 291b 7215  Stat.save).N).r.
+00001590: 0000 0072 1600 0000 7217 0000 0072 0600  ...r....r....r..
+000015a0: 0000 da0c 4269 6741 7574 6f46 6965 6c64  ....BigAutoField
+000015b0: 7259 0000 00da 0c49 6e74 6567 6572 4669  rY.....IntegerFi
+000015c0: 656c 6472 0800 0000 723d 0000 0072 6e00  eldr....r=...rn.
+000015d0: 0000 726f 0000 0072 7200 0000 7270 0000  ..ro...rr...rp..
+000015e0: 0072 4f00 0000 da0c 6368 616e 6e65 6c5f  .rO.....channel_
+000015f0: 6e61 6d65 726b 0000 0072 6c00 0000 726d  namerk...rl...rm
+00001600: 0000 0072 5100 0000 725e 0000 0072 0400  ...rQ...r^...r..
+00001610: 0000 7260 0000 0072 6300 0000 726a 0000  ..r`...rc...rj..
+00001620: 0072 4e00 0000 7227 0000 00da 0d5f 5f63  .rN...r'.....__c
+00001630: 6c61 7373 6365 6c6c 5f5f 7219 0000 0072  lasscell__r....r
+00001640: 1900 0000 7277 0000 0072 1a00 0000 7252  ....rw...r....rR
+00001650: 0000 005f 0000 0073 5200 0000 0801 0401  ..._...sR.......
+00001660: 02ff 0603 0401 04ff 0603 0401 04ff 0603  ................
+00001670: 0401 04ff 0603 0401 04ff 0603 0401 0201  ................
+00001680: 02fe 0604 0401 02ff 0603 0401 02ff 0603  ................
+00001690: 0401 0201 04fe 0605 0201 0a03 0201 0201  ................
+000016a0: 0c03 0201 0201 0c08 0201 0c0c 0806 7252  ..............rR
+000016b0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000016c0: 0000 0000 0600 0000 4000 0001 7310 0100  ........@...s...
+000016d0: 0065 005a 0164 005a 0265 036a 0464 0164  .e.Z.d.Z.e.j.d.d
+000016e0: 028d 015a 0565 03a0 04a1 005a 0665 03a0  ...Z.e.....Z.e..
+000016f0: 04a1 005a 0765 03a0 04a1 005a 0865 036a  ...Z.e.....Z.e.j
+00001700: 0964 0364 048d 015a 0a65 03a0 04a1 005a  .d.d...Z.e.....Z
+00001710: 0b65 036a 0c64 0564 048d 015a 0d65 0e64  .e.j.d.d...Z.e.d
+00001720: 0664 0784 0083 015a 0f65 1065 0e65 11a0  .d.....Z.e.e.e..
+00001730: 1264 0864 09a1 0264 0a65 136a 13a0 14a1  .d.d...d.e.j....
+00001740: 0064 0366 0464 0b64 0c84 0183 0183 015a  .d.f.d.d.......Z
+00001750: 1565 1664 0d64 0e84 0083 015a 1765 0e64  .e.d.d.....Z.e.d
+00001760: 0f64 1084 0083 015a 1865 0e64 1164 1284  .d.....Z.e.d.d..
+00001770: 0083 015a 1965 0e64 1364 1484 0083 015a  ...Z.e.d.d.....Z
+00001780: 1a65 0e64 1564 1684 0083 015a 1b65 0e64  .e.d.d.....Z.e.d
+00001790: 1764 1884 0083 015a 1c65 1065 0e64 1964  .d.....Z.e.e.d.d
+000017a0: 1a84 0083 0183 015a 1d65 1065 0e64 1b64  .......Z.e.e.d.d
+000017b0: 1c84 0083 0183 015a 1e64 1d64 1e84 005a  .......Z.d.d...Z
+000017c0: 1f65 2064 1f64 2084 0083 015a 2165 1065  .e d.d ....Z!e.e
+000017d0: 0e64 2164 2284 0083 0183 015a 2264 2353  .d!d"......Z"d#S
+000017e0: 0029 24da 0955 7365 7250 6f69 6e74 54a9  .)$..UserPointT.
+000017f0: 01da 0675 6e69 7175 6572 0100 0000 7253  ...uniquer....rS
+00001800: 0000 0046 6301 0000 0000 0000 0000 0000  ...Fc...........
+00001810: 0001 0000 0002 0000 0043 0000 0173 0c00  .........C...s..
+00001820: 0000 7c00 a000 a100 0100 6400 5300 725f  ..|.......d.S.r_
+00001830: 0000 0072 2600 0000 724c 0000 0072 1900  ...r&...rL...r..
+00001840: 0000 7219 0000 0072 1a00 0000 da0a 6173  ..r....r......as
+00001850: 796e 635f 7361 7665 c700 0000 7302 0000  ync_save....s...
+00001860: 0000 027a 1455 7365 7250 6f69 6e74 2e61  ...z.UserPoint.a
+00001870: 7379 6e63 5f73 6176 65e9 0f00 0000 e919  sync_save.......
+00001880: 0000 0072 0b00 0000 6305 0000 0000 0000  ...r....c.......
+00001890: 0000 0000 0006 0000 0008 0000 0043 0000  .............C..
+000018a0: 0173 2a00 0000 7400 7c00 7c01 7400 a001  .s*...t.|.|.t...
+000018b0: 7c01 a101 7c02 7c03 a002 a100 7c04 6401  |...|.|.....|.d.
+000018c0: 8d06 7d05 7c05 a003 a100 0100 7c05 5300  ..}.|.......|.S.
+000018d0: 2902 4e29 0672 2a00 0000 da06 706f 696e  ).N).r*.....poin
+000018e0: 7473 da18 6c65 7665 6c5f 7570 5f73 7065  ts..level_up_spe
+000018f0: 6369 6669 635f 706f 696e 7473 da0d 6d65  cific_points..me
+00001900: 7373 6167 655f 636f 756e 74da 1f6c 6174  ssage_count..lat
+00001910: 6573 745f 7469 6d65 5f78 705f 7761 735f  est_time_xp_was_
+00001920: 6561 726e 6564 5f65 706f 6368 da0c 6c65  earned_epoch..le
+00001930: 7665 6c5f 6e75 6d62 6572 2904 727d 0000  vel_number).r}..
+00001940: 00da 2263 616c 6375 6c61 7465 5f6c 6576  .."calculate_lev
+00001950: 656c 5f75 705f 7370 6563 6966 6963 5f70  el_up_specific_p
+00001960: 6f69 6e74 7372 3e00 0000 7227 0000 0029  ointsr>...r'...)
+00001970: 0672 2a00 0000 7283 0000 0072 8500 0000  .r*...r....r....
+00001980: 5a19 6c61 7465 7374 5f74 696d 655f 7870  Z.latest_time_xp
+00001990: 5f77 6173 5f65 6172 6e65 64da 056c 6576  _was_earned..lev
+000019a0: 656c da0a 7573 6572 5f70 6f69 6e74 7219  el..user_pointr.
+000019b0: 0000 0072 1900 0000 721a 0000 00da 1163  ...r....r......c
+000019c0: 7265 6174 655f 7573 6572 5f70 6f69 6e74  reate_user_point
+000019d0: cb00 0000 7310 0000 0000 0502 0104 0108  ....s...........
+000019e0: 0102 0108 fc06 0608 017a 1b55 7365 7250  .........z.UserP
+000019f0: 6f69 6e74 2e63 7265 6174 655f 7573 6572  oint.create_user
+00001a00: 5f70 6f69 6e74 6302 0000 0000 0000 0000  _pointc.........
+00001a10: 0000 0004 0000 0003 0000 0043 0000 0173  ...........C...s
+00001a20: 4a00 0000 6401 7d02 7400 6a01 a002 a100  J...d.}.t.j.....
+00001a30: a003 6402 a101 7d03 7c03 7c02 1900 6a04  ..d...}.|.|...j.
+00001a40: 7c01 6b00 7246 7c02 7405 7c03 8301 6b00  |.k.rF|.t.|...k.
+00001a50: 7246 7c01 7c03 7c02 1900 6a04 3800 7d01  rF|.|.|...j.8.}.
+00001a60: 7c02 6403 3700 7d02 7114 7c01 5300 2904  |.d.7.}.q.|.S.).
+00001a70: 4e72 0100 0000 da15 746f 7461 6c5f 706f  Nr......total_po
+00001a80: 696e 7473 5f72 6571 7569 7265 6472 0b00  ints_requiredr..
+00001a90: 0000 2906 da05 4c65 7665 6c72 2000 0000  ..)...Levelr ...
+00001aa0: 7243 0000 00da 086f 7264 6572 5f62 79da  rC.....order_by.
+00001ab0: 2378 705f 6e65 6564 6564 5f74 6f5f 6c65  #xp_needed_to_le
+00001ac0: 7665 6c5f 7570 5f74 6f5f 6e65 7874 5f6c  vel_up_to_next_l
+00001ad0: 6576 656c 7267 0000 0029 0472 2200 0000  evelrg...).r"...
+00001ae0: 7283 0000 005a 0469 6e64 785a 066c 6576  r....Z.indxZ.lev
+00001af0: 656c 7372 1900 0000 7219 0000 0072 1a00  elsr....r....r..
+00001b00: 0000 7288 0000 00d9 0000 0073 0c00 0000  ..r........s....
+00001b10: 0002 0401 1001 1a01 0e01 0a02 7a2c 5573  ............z,Us
+00001b20: 6572 506f 696e 742e 6361 6c63 756c 6174  erPoint.calculat
+00001b30: 655f 6c65 7665 6c5f 7570 5f73 7065 6369  e_level_up_speci
+00001b40: 6669 635f 706f 696e 7473 6301 0000 0000  fic_pointsc.....
+00001b50: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
+00001b60: 0000 0173 a600 0000 6401 7d01 7c00 a000  ...s....d.}.|...
+00001b70: a100 72a2 7401 a002 6402 6403 a102 7d02  ..r.t...d.d...}.
+00001b80: 7c00 0400 6a03 7c02 3700 0200 5f03 7c00  |...j.|.7..._.|.
+00001b90: 0400 6a04 7c02 3700 0200 5f04 7c00 0400  ..j.|.7..._.|...
+00001ba0: 6a05 6404 3700 0200 5f05 7c00 6a06 6405  j.d.7..._.|.j.d.
+00001bb0: 6b00 728a 7407 6a08 6a09 7c00 6a06 6406  k.r.t.j.j.|.j.d.
+00001bc0: 8d01 7d03 7c00 6a04 7c03 6a0a 6b05 728a  ..}.|.j.|.j.k.r.
+00001bd0: 7c00 0400 6a04 7c03 6a0a 3800 0200 5f04  |...j.|.j.8..._.
+00001be0: 7c00 0400 6a06 6404 3700 0200 5f06 6407  |...j.d.7..._.d.
+00001bf0: 7d01 740b 6a0b a00c a100 a00d a100 7c00  }.t.j.........|.
+00001c00: 5f0e 7c00 a00f a100 0100 7c01 5300 2908  _.|.......|.S.).
+00001c10: 4e46 7281 0000 0072 8200 0000 720b 0000  NFr....r....r...
+00001c20: 00e9 6400 0000 a901 da06 6e75 6d62 6572  ..d.......number
+00001c30: 5429 10da 1d6d 6573 7361 6765 5f63 6f75  T)...message_cou
+00001c40: 6e74 735f 746f 7761 7264 735f 706f 696e  nts_towards_poin
+00001c50: 7473 da06 7261 6e64 6f6d da07 7261 6e64  ts..random..rand
+00001c60: 696e 7472 8300 0000 7284 0000 0072 8500  intr....r....r..
+00001c70: 0000 7287 0000 0072 8d00 0000 7220 0000  ..r....r....r ..
+00001c80: 0072 3a00 0000 728f 0000 0072 3c00 0000  .r:...r....r<...
+00001c90: 723d 0000 0072 3e00 0000 7286 0000 0072  r=...r>...r....r
+00001ca0: 2700 0000 2904 724d 0000 005a 0a61 6c65  '...).rM...Z.ale
+00001cb0: 7274 5f75 7365 725a 0570 6f69 6e74 5a0d  rt_userZ.pointZ.
+00001cc0: 6375 7272 656e 745f 6c65 7665 6c72 1900  current_levelr..
+00001cd0: 0000 7219 0000 0072 1a00 0000 da10 696e  ..r....r......in
+00001ce0: 6372 656d 656e 745f 706f 696e 7473 e300  crement_points..
+00001cf0: 0000 731e 0000 0000 0204 0108 010c 010e  ..s.............
+00001d00: 010e 010e 010a 0110 010c 0110 010e 0104  ................
+00001d10: 0110 0108 017a 1a55 7365 7250 6f69 6e74  .....z.UserPoint
+00001d20: 2e69 6e63 7265 6d65 6e74 5f70 6f69 6e74  .increment_point
+00001d30: 7363 0100 0000 0000 0000 0000 0000 0300  sc..............
+00001d40: 0000 0400 0000 4300 0001 734e 0000 0067  ......C...sN...g
+00001d50: 007d 0174 006a 01a0 02a1 00a0 0364 01a1  .}.t.j.......d..
+00001d60: 0144 005d 2c7d 027c 026a 047c 006a 046b  .D.],}.|.j.|.j.k
+00001d70: 0372 307c 01a0 057c 02a1 0101 0071 1474  .r0|...|.....q.t
+00001d80: 067c 0183 0164 0217 0002 0001 0053 0071  .|...d.......S.q
+00001d90: 1474 067c 0183 0164 0217 0053 0029 034e  .t.|...d...S.).N
+00001da0: 7a07 2d70 6f69 6e74 7372 0b00 0000 2907  z.-pointsr....).
+00001db0: 727d 0000 0072 2000 0000 7243 0000 0072  r}...r ...rC...r
+00001dc0: 8e00 0000 722a 0000 00da 0661 7070 656e  ....r*.....appen
+00001dd0: 6472 6700 0000 2903 724d 0000 005a 1375  drg...).rM...Z.u
+00001de0: 7365 7273 5f61 626f 7665 5f69 6e5f 7261  sers_above_in_ra
+00001df0: 6e6b 723f 0000 0072 1900 0000 7219 0000  nkr?...r....r...
+00001e00: 0072 1a00 0000 da08 6765 745f 7261 6e6b  .r......get_rank
+00001e10: f500 0000 730c 0000 0000 0204 0114 010c  ....s...........
+00001e20: 010c 0212 017a 1255 7365 7250 6f69 6e74  .....z.UserPoint
+00001e30: 2e67 6574 5f72 616e 6b63 0100 0000 0000  .get_rankc......
+00001e40: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00001e50: 0001 7312 0000 0074 006a 016a 027c 006a  ..s....t.j.j.|.j
+00001e60: 0364 018d 016a 0453 0029 024e 7291 0000  .d...j.S.).Nr...
+00001e70: 0029 0572 8d00 0000 7220 0000 0072 3a00  .).r....r ...r:.
+00001e80: 0000 7287 0000 0072 8f00 0000 724c 0000  ..r....r....rL..
+00001e90: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00001ea0: da27 6765 745f 7870 5f6e 6565 6465 645f  .'get_xp_needed_
+00001eb0: 746f 5f6c 6576 656c 5f75 705f 746f 5f6e  to_level_up_to_n
+00001ec0: 6578 745f 6c65 7665 6cff 0000 0073 0200  ext_level....s..
+00001ed0: 0000 0002 7a31 5573 6572 506f 696e 742e  ....z1UserPoint.
+00001ee0: 6765 745f 7870 5f6e 6565 6465 645f 746f  get_xp_needed_to
+00001ef0: 5f6c 6576 656c 5f75 705f 746f 5f6e 6578  _level_up_to_nex
+00001f00: 745f 6c65 7665 6c63 0100 0000 0000 0000  t_levelc........
+00001f10: 0000 0000 0100 0000 0200 0000 4300 0001  ............C...
+00001f20: 7312 0000 0064 017c 005f 007c 00a0 01a1  s....d.|._.|....
+00001f30: 0001 0064 0053 0029 024e 54a9 02da 0668  ...d.S.).NT....h
+00001f40: 6964 6465 6e72 2700 0000 724c 0000 0072  iddenr'...rL...r
+00001f50: 1900 0000 7219 0000 0072 1a00 0000 da07  ....r....r......
+00001f60: 6869 6465 5f78 7003 0100 0073 0400 0000  hide_xp....s....
+00001f70: 0002 0601 7a11 5573 6572 506f 696e 742e  ....z.UserPoint.
+00001f80: 6869 6465 5f78 7063 0100 0000 0000 0000  hide_xpc........
+00001f90: 0000 0000 0100 0000 0200 0000 4300 0001  ............C...
+00001fa0: 7312 0000 0064 017c 005f 007c 00a0 01a1  s....d.|._.|....
+00001fb0: 0001 0064 0053 0029 024e 4672 9a00 0000  ...d.S.).NFr....
+00001fc0: 724c 0000 0072 1900 0000 7219 0000 0072  rL...r....r....r
+00001fd0: 1a00 0000 da07 7368 6f77 5f78 7008 0100  ......show_xp...
+00001fe0: 0073 0400 0000 0002 0601 7a11 5573 6572  .s........z.User
+00001ff0: 506f 696e 742e 7368 6f77 5f78 7063 0000  Point.show_xpc..
+00002000: 0000 0000 0000 0000 0000 0000 0000 0500  ................
+00002010: 0000 4300 0001 731e 0000 0074 0074 0174  ..C...s....t.t.t
+00002020: 026a 03a0 04a1 0064 0064 0185 0219 0083  .j.....d.d......
+00002030: 0183 0164 016b 0253 0072 6100 0000 2905  ...d.k.S.ra...).
+00002040: 7267 0000 0072 2e00 0000 727d 0000 0072  rg...r....r}...r
+00002050: 2000 0000 7243 0000 0072 1900 0000 7219   ...rC...r....r.
+00002060: 0000 0072 1900 0000 721a 0000 00da 1e75  ...r....r......u
+00002070: 7365 725f 706f 696e 7473 5f68 6176 655f  ser_points_have_
+00002080: 6265 656e 5f69 6d70 6f72 7465 640d 0100  been_imported...
+00002090: 0073 0200 0000 0003 7a28 5573 6572 506f  .s......z(UserPo
+000020a0: 696e 742e 7573 6572 5f70 6f69 6e74 735f  int.user_points_
+000020b0: 6861 7665 5f62 6565 6e5f 696d 706f 7274  have_been_import
+000020c0: 6564 6300 0000 0000 0000 0000 0000 0000  edc.............
+000020d0: 0000 0002 0000 0043 0000 0173 1200 0000  .......C...s....
+000020e0: 7400 6a01 a002 a100 a003 a100 0100 6400  t.j...........d.
+000020f0: 5300 725f 0000 0029 0472 7d00 0000 7220  S.r_...).r}...r 
+00002100: 0000 0072 4300 0000 da06 6465 6c65 7465  ...rC.....delete
+00002110: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+00002120: 1a00 0000 da11 636c 6561 725f 616c 6c5f  ......clear_all_
+00002130: 656e 7472 6965 7312 0100 0073 0200 0000  entries....s....
+00002140: 0003 7a1b 5573 6572 506f 696e 742e 636c  ..z.UserPoint.cl
+00002150: 6561 725f 616c 6c5f 656e 7472 6965 7363  ear_all_entriesc
+00002160: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00002170: 0600 0000 4300 0001 733a 0000 0074 006a  ....C...s:...t.j
+00002180: 00a0 017c 006a 0274 03a0 0474 056a 06a1  ...|.j.t...t.j..
+00002190: 01a1 0274 006a 0764 0164 028d 0117 0074  ...t.j.d.d.....t
+000021a0: 006a 006a 0874 03a0 0474 056a 06a1 0164  .j.j.t...t.j...d
+000021b0: 038d 016b 0053 0029 044e 720b 0000 00a9  ...k.S.).Nr.....
+000021c0: 01da 076d 696e 7574 6573 7209 0000 0029  ...minutesr....)
+000021d0: 0972 3c00 0000 da0d 6672 6f6d 7469 6d65  .r<.....fromtime
+000021e0: 7374 616d 7072 8600 0000 da04 7079 747a  stampr......pytz
+000021f0: 7208 0000 0072 0500 0000 da09 5449 4d45  r....r......TIME
+00002200: 5f5a 4f4e 45da 0974 696d 6564 656c 7461  _ZONE..timedelta
+00002210: 723d 0000 0072 4c00 0000 7219 0000 0072  r=...rL...r....r
+00002220: 1900 0000 721a 0000 0072 9300 0000 1701  ....r....r......
+00002230: 0000 7310 0000 0000 0106 0104 010a fe02  ..s.............
+00002240: 030a fd02 0314 fd7a 2755 7365 7250 6f69  .......z'UserPoi
+00002250: 6e74 2e6d 6573 7361 6765 5f63 6f75 6e74  nt.message_count
+00002260: 735f 746f 7761 7264 735f 706f 696e 7473  s_towards_points
+00002270: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00002280: 0004 0000 0043 0000 0173 4400 0000 6401  .....C...sD...d.
+00002290: 7400 6a01 9b00 9d02 6402 6403 9c02 7d01  t.j.....d.d...}.
+000022a0: 7402 6a03 6404 7c00 6a04 9b00 9d02 7c01  t.j.d.|.j.....|.
+000022b0: 6405 8d02 7d02 6406 7c02 a005 a100 7600  d...}.d.|.....v.
+000022c0: 7240 7c02 a005 a100 6406 1900 5300 6407  r@|.....d...S.d.
+000022d0: 5300 2908 4e7a 0442 6f74 207a 1061 7070  S.).Nz.Bot z.app
+000022e0: 6c69 6361 7469 6f6e 2f6a 736f 6e29 02da  lication/json)..
+000022f0: 0d41 7574 686f 7269 7a61 7469 6f6e 7a0c  .Authorizationz.
+00002300: 436f 6e74 656e 742d 5479 7065 7a1e 6874  Content-Typez.ht
+00002310: 7470 733a 2f2f 6469 7363 6f72 642e 636f  tps://discord.co
+00002320: 6d2f 6170 692f 7573 6572 732f 2901 da07  m/api/users/)...
+00002330: 6865 6164 6572 7372 3300 0000 7255 0000  headersr3...rU..
+00002340: 0029 0672 0500 0000 5a11 4449 5343 4f52  .).r....Z.DISCOR
+00002350: 445f 424f 545f 544f 4b45 4eda 0872 6571  D_BOT_TOKEN..req
+00002360: 7565 7374 7372 3a00 0000 722a 0000 00da  uestsr:...r*....
+00002370: 046a 736f 6e29 0372 4d00 0000 5a0e 6469  .json).rM...Z.di
+00002380: 7363 6f72 645f 6865 6164 6572 da08 7265  scord_header..re
+00002390: 7370 6f6e 7365 7219 0000 0072 1900 0000  sponser....r....
+000023a0: 721a 0000 0072 3300 0000 1d01 0000 7310  r....r3.......s.
+000023b0: 0000 0000 030a 0102 fe06 0404 010a 0102  ................
+000023c0: fe06 057a 1255 7365 7250 6f69 6e74 2e75  ...z.UserPoint.u
+000023d0: 7365 726e 616d 6563 0000 0000 0000 0000  sernamec........
+000023e0: 0000 0000 0000 0000 0300 0000 4300 0001  ............C...
+000023f0: 7314 0000 0064 0164 0284 0074 006a 01a0  s....d.d...t.j..
+00002400: 02a1 0044 0083 0153 0029 034e 6301 0000  ...D...S.).Nc...
+00002410: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00002420: 0053 0000 0173 1400 0000 6900 7c00 5d0c  .S...s....i.|.].
+00002430: 7d01 7c01 6a00 7c01 9302 7104 5300 7219  }.|.j.|...q.S.r.
+00002440: 0000 0072 4200 0000 2902 725a 0000 0072  ...rB...).rZ...r
+00002450: 8a00 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
+00002460: 0000 00da 0a3c 6469 6374 636f 6d70 3e2d  .....<dictcomp>-
+00002470: 0100 0072 5d00 0000 7a2a 5573 6572 506f  ...r]...z*UserPo
+00002480: 696e 742e 6c6f 6164 5f74 6f5f 6469 6374  int.load_to_dict
+00002490: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
+000024a0: 6f6d 703e 2903 727d 0000 0072 2000 0000  omp>).r}...r ...
+000024b0: 7243 0000 0072 1900 0000 7219 0000 0072  rC...r....r....r
+000024c0: 1900 0000 721a 0000 00da 0c6c 6f61 645f  ....r......load_
+000024d0: 746f 5f64 6963 742a 0100 0073 0200 0000  to_dict*...s....
+000024e0: 0003 7a16 5573 6572 506f 696e 742e 6c6f  ..z.UserPoint.lo
+000024f0: 6164 5f74 6f5f 6469 6374 4e29 2372 1500  ad_to_dictN)#r..
+00002500: 0000 7216 0000 0072 1700 0000 7206 0000  ..r....r....r...
+00002510: 00da 1750 6f73 6974 6976 6542 6967 496e  ...PositiveBigIn
+00002520: 7465 6765 7246 6965 6c64 722a 0000 0072  tegerFieldr*...r
+00002530: 8300 0000 7284 0000 0072 8500 0000 7250  ....r....r....rP
+00002540: 0000 0072 8600 0000 7287 0000 00da 0c42  ...r....r......B
+00002550: 6f6f 6c65 616e 4669 656c 6472 9b00 0000  ooleanFieldr....
+00002560: 7204 0000 0072 8000 0000 da0c 7374 6174  r....r......stat
+00002570: 6963 6d65 7468 6f64 7294 0000 0072 9500  icmethodr....r..
+00002580: 0000 723c 0000 0072 3d00 0000 728b 0000  ..r<...r=...r...
+00002590: 0072 5100 0000 7288 0000 0072 9600 0000  .rQ...r....r....
+000025a0: 7298 0000 0072 9900 0000 729c 0000 0072  r....r....r....r
+000025b0: 9d00 0000 729e 0000 0072 a000 0000 7293  ....r....r....r.
+000025c0: 0000 00da 0870 726f 7065 7274 7972 3300  .....propertyr3.
+000025d0: 0000 72ad 0000 0072 1900 0000 7219 0000  ..r....r....r...
+000025e0: 0072 1900 0000 721a 0000 0072 7d00 0000  .r....r....r}...
+000025f0: b000 0000 7358 0000 0008 0104 0102 ff06  ....sX..........
+00002600: 0308 0308 0308 0304 0102 ff06 0308 0304  ................
+00002610: 0102 ff06 0402 010a 0302 0102 020c 010a  ................
+00002620: fe0e 0c02 010a 0902 010a 1102 010a 0902  ................
+00002630: 010a 0302 010a 0402 010a 0402 0102 010c  ................
+00002640: 0302 0102 010c 0308 0602 010a 0c02 0102  ................
+00002650: 0172 7d00 0000 6300 0000 0000 0000 0000  .r}...c.........
+00002660: 0000 0000 0000 0005 0000 0040 0000 0173  ...........@...s
+00002670: b800 0000 6500 5a01 6400 5a02 6503 6a04  ....e.Z.d.Z.e.j.
+00002680: 6401 6402 8d01 5a05 6503 a004 a100 5a06  d.d...Z.e.....Z.
+00002690: 6503 a004 a100 5a07 6503 6a04 6401 6401  e.....Z.e.j.d.d.
+000026a0: 6403 8d02 5a08 6503 6a09 6404 6401 6401  d...Z.e.j.d.d.d.
+000026b0: 6405 8d03 5a0a 650b 650c 6417 6407 6408  d...Z.e.e.d.d.d.
+000026c0: 8401 8301 8301 5a0d 650c 6409 640a 8400  ......Z.e.d.d...
+000026d0: 8301 5a0e 650b 650c 640b 640c 8400 8301  ..Z.e.e.d.d.....
+000026e0: 8301 5a0f 650b 650c 640d 640e 8400 8301  ..Z.e.e.d.d.....
+000026f0: 8301 5a10 650b 650c 640f 6410 8400 8301  ..Z.e.e.d.d.....
+00002700: 8301 5a11 650c 6411 6412 8400 8301 5a12  ..Z.e.d.d.....Z.
+00002710: 650c 6413 6414 8400 8301 5a13 650c 6415  e.d.d.....Z.e.d.
+00002720: 6416 8400 8301 5a14 6406 5300 2918 728d  d.....Z.d.S.).r.
+00002730: 0000 0054 727e 0000 0029 0272 1200 0000  ...Tr~...).r....
+00002740: 727f 0000 00e9 f401 0000 2903 7211 0000  r.........).r...
+00002750: 0072 1200 0000 727f 0000 004e 6305 0000  .r....r....Nc...
+00002760: 0000 0000 0000 0000 0006 0000 0007 0000  ................
+00002770: 0043 0000 0173 1e00 0000 7400 7c00 7c01  .C...s....t.|.|.
+00002780: 7c02 7c03 7c04 6401 8d05 7d05 7c05 a001  |.|.|.d...}.|...
+00002790: a100 0100 7c05 5300 2902 4e29 0572 9200  ....|.S.).N).r..
+000027a0: 0000 728c 0000 0072 8f00 0000 da07 726f  ..r....r......ro
+000027b0: 6c65 5f69 64da 0972 6f6c 655f 6e61 6d65  le_id..role_name
+000027c0: 2902 728d 0000 0072 2700 0000 2906 7292  ).r....r'...).r.
+000027d0: 0000 0072 8c00 0000 728f 0000 0072 b300  ...r....r....r..
+000027e0: 0000 72b4 0000 0072 8900 0000 7219 0000  ..r....r....r...
+000027f0: 0072 1900 0000 721a 0000 00da 0c63 7265  .r....r......cre
+00002800: 6174 655f 6c65 7665 6c46 0100 0073 0e00  ate_levelF...s..
+00002810: 0000 0004 0201 0401 0201 04fd 0605 0801  ................
+00002820: 7a12 4c65 7665 6c2e 6372 6561 7465 5f6c  z.Level.create_l
+00002830: 6576 656c 6301 0000 0000 0000 0000 0000  evelc...........
+00002840: 0001 0000 0002 0000 0043 0000 0173 0c00  .........C...s..
+00002850: 0000 7c00 a000 a100 0100 6400 5300 725f  ..|.......d.S.r_
+00002860: 0000 0072 2600 0000 724c 0000 0072 1900  ...r&...rL...r..
+00002870: 0000 7219 0000 0072 1a00 0000 7280 0000  ..r....r....r...
+00002880: 0052 0100 0073 0200 0000 0002 7a10 4c65  .R...s......z.Le
+00002890: 7665 6c2e 6173 796e 635f 7361 7665 6300  vel.async_savec.
+000028a0: 0000 0000 0000 0000 0000 0000 0000 0005  ................
+000028b0: 0000 0043 0000 0173 1e00 0000 7400 7401  ...C...s....t.t.
+000028c0: 7402 6a03 a004 a100 6400 6401 8502 1900  t.j.....d.d.....
+000028d0: 8301 8301 6401 6b02 5300 7261 0000 0029  ....d.k.S.ra...)
+000028e0: 0572 6700 0000 722e 0000 0072 8d00 0000  .rg...r....r....
+000028f0: 7220 0000 0072 4300 0000 7219 0000 0072  r ...rC...r....r
+00002900: 1900 0000 7219 0000 0072 1a00 0000 da1f  ....r....r......
+00002910: 6c65 7665 6c5f 706f 696e 7473 5f68 6176  level_points_hav
+00002920: 655f 6265 656e 5f69 6d70 6f72 7465 6456  e_been_importedV
+00002930: 0100 0073 0200 0000 0003 7a25 4c65 7665  ...s......z%Leve
+00002940: 6c2e 6c65 7665 6c5f 706f 696e 7473 5f68  l.level_points_h
+00002950: 6176 655f 6265 656e 5f69 6d70 6f72 7465  ave_been_importe
+00002960: 6463 0000 0000 0000 0000 0000 0000 0000  dc..............
+00002970: 0000 0200 0000 4300 0001 7312 0000 0074  ......C...s....t
+00002980: 006a 01a0 02a1 00a0 03a1 0001 0064 0053  .j...........d.S
+00002990: 0072 5f00 0000 2904 728d 0000 0072 2000  .r_...).r....r .
+000029a0: 0000 7243 0000 0072 9f00 0000 7219 0000  ..rC...r....r...
+000029b0: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
+000029c0: 72a0 0000 005b 0100 0073 0200 0000 0003  r....[...s......
+000029d0: 7a17 4c65 7665 6c2e 636c 6561 725f 616c  z.Level.clear_al
+000029e0: 6c5f 656e 7472 6965 7363 0000 0000 0000  l_entriesc......
+000029f0: 0000 0000 0000 0000 0000 0300 0000 4300  ..............C.
+00002a00: 0001 7314 0000 0064 0164 0284 0074 006a  ..s....d.d...t.j
+00002a10: 01a0 02a1 0044 0083 0153 0029 034e 6301  .....D...S.).Nc.
+00002a20: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00002a30: 0000 0053 0000 0173 1400 0000 6900 7c00  ...S...s....i.|.
+00002a40: 5d0c 7d01 7c01 6a00 7c01 9302 7104 5300  ].}.|.j.|...q.S.
+00002a50: 7219 0000 0072 9100 0000 2902 725a 0000  r....r....).rZ..
+00002a60: 0072 8900 0000 7219 0000 0072 1900 0000  .r....r....r....
+00002a70: 721a 0000 0072 ac00 0000 6301 0000 725d  r....r....c...r]
+00002a80: 0000 007a 264c 6576 656c 2e6c 6f61 645f  ...z&Level.load_
+00002a90: 746f 5f64 6963 742e 3c6c 6f63 616c 733e  to_dict.<locals>
+00002aa0: 2e3c 6469 6374 636f 6d70 3e29 0372 8d00  .<dictcomp>).r..
+00002ab0: 0000 7220 0000 0072 4300 0000 7219 0000  ..r ...rC...r...
+00002ac0: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00002ad0: 72ad 0000 0060 0100 0073 0200 0000 0003  r....`...s......
+00002ae0: 7a12 4c65 7665 6c2e 6c6f 6164 5f74 6f5f  z.Level.load_to_
+00002af0: 6469 6374 6303 0000 0000 0000 0000 0000  dictc...........
+00002b00: 0003 0000 0002 0000 0043 0000 0173 1800  .........C...s..
+00002b10: 0000 7c01 7c00 5f00 7c02 7c00 5f01 7c00  ..|.|._.|.|._.|.
+00002b20: a002 a100 0100 6400 5300 725f 0000 00a9  ......d.S.r_....
+00002b30: 0372 b400 0000 72b3 0000 0072 2700 0000  .r....r....r'...
+00002b40: 2903 724d 0000 00da 0d6e 6577 5f72 6f6c  ).rM.....new_rol
+00002b50: 655f 6e61 6d65 72b3 0000 0072 1900 0000  e_namer....r....
+00002b60: 7219 0000 0072 1a00 0000 da0e 7365 745f  r....r......set_
+00002b70: 6c65 7665 6c5f 6e61 6d65 6501 0000 7306  level_namee...s.
+00002b80: 0000 0000 0206 0106 017a 144c 6576 656c  .........z.Level
+00002b90: 2e73 6574 5f6c 6576 656c 5f6e 616d 6563  .set_level_namec
+00002ba0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00002bb0: 0200 0000 4300 0001 7312 0000 007c 017c  ....C...s....|.|
+00002bc0: 005f 007c 00a0 01a1 0001 0064 0053 0072  ._.|.......d.S.r
+00002bd0: 5f00 0000 2902 72b4 0000 0072 2700 0000  _...).r....r'...
+00002be0: 2902 724d 0000 0072 b800 0000 7219 0000  ).rM...r....r...
+00002bf0: 0072 1900 0000 721a 0000 00da 1172 656e  .r....r......ren
+00002c00: 616d 655f 6c65 7665 6c5f 6e61 6d65 6b01  ame_level_namek.
+00002c10: 0000 7304 0000 0000 0206 017a 174c 6576  ..s........z.Lev
+00002c20: 656c 2e72 656e 616d 655f 6c65 7665 6c5f  el.rename_level_
+00002c30: 6e61 6d65 6301 0000 0000 0000 0000 0000  namec...........
+00002c40: 0001 0000 0002 0000 0043 0000 0173 1800  .........C...s..
+00002c50: 0000 6400 7c00 5f00 6400 7c00 5f01 7c00  ..d.|._.d.|._.|.
+00002c60: a002 a100 0100 6400 5300 725f 0000 0072  ......d.S.r_...r
+00002c70: b700 0000 724c 0000 0072 1900 0000 7219  ....rL...r....r.
+00002c80: 0000 0072 1a00 0000 da0b 7265 6d6f 7665  ...r......remove
+00002c90: 5f72 6f6c 6570 0100 0073 0600 0000 0002  _rolep...s......
+00002ca0: 0601 0601 7a11 4c65 7665 6c2e 7265 6d6f  ....z.Level.remo
+00002cb0: 7665 5f72 6f6c 6529 024e 4e29 1572 1500  ve_role).NN).r..
+00002cc0: 0000 7216 0000 0072 1700 0000 7206 0000  ..r....r....r...
+00002cd0: 0072 ae00 0000 7292 0000 0072 8c00 0000  .r....r....r....
+00002ce0: 728f 0000 0072 b300 0000 724f 0000 0072  r....r....rO...r
+00002cf0: b400 0000 72b0 0000 0072 0400 0000 72b5  ....r....r....r.
+00002d00: 0000 0072 8000 0000 72b6 0000 0072 a000  ...r....r....r..
+00002d10: 0000 72ad 0000 0072 b900 0000 72ba 0000  ..r....r....r...
+00002d20: 0072 bb00 0000 7219 0000 0072 1900 0000  .r....r....r....
+00002d30: 7219 0000 0072 1a00 0000 728d 0000 0030  r....r....r....0
+00002d40: 0100 0073 4600 0000 0801 0401 02ff 0603  ...sF...........
+00002d50: 0804 0804 0401 0201 02fe 0604 0401 0201  ................
+00002d60: 0201 02fd 0606 0201 0202 00ff 0e0a 0201  ................
+00002d70: 0a03 0201 0201 0c03 0201 0201 0c03 0201  ................
+00002d80: 0201 0c03 0201 0a05 0201 0a04 0201 728d  ..............r.
+00002d90: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00002da0: 0000 0000 0400 0000 4000 0001 73be 0000  ........@...s...
+00002db0: 0065 005a 0164 005a 0265 036a 0464 0164  .e.Z.d.Z.e.j.d.d
+00002dc0: 028d 015a 0565 036a 0664 0364 048d 015a  ...Z.e.j.d.d...Z
+00002dd0: 0765 036a 0864 0564 0664 078d 025a 0965  .e.j.d.d.d...Z.e
+00002de0: 036a 0664 0364 048d 015a 0a64 0864 0984  .j.d.d...Z.d.d..
+00002df0: 005a 0b65 0c65 0d64 0a64 0b84 0083 0183  .Z.e.e.d.d......
+00002e00: 015a 0e65 0c65 0d64 0c64 0d84 0083 0183  .Z.e.e.d.d......
+00002e10: 015a 0f65 0c65 0d64 0e64 0f84 0083 0183  .Z.e.e.d.d......
+00002e20: 015a 1065 0c65 0d64 1064 1184 0083 0183  .Z.e.e.d.d......
+00002e30: 015a 1165 0c65 0d64 1264 1384 0083 0183  .Z.e.e.d.d......
+00002e40: 015a 1265 0c65 0d64 1464 1584 0083 0183  .Z.e.e.d.d......
+00002e50: 015a 1365 0c65 0d64 1664 1784 0083 0183  .Z.e.e.d.d......
+00002e60: 015a 1464 1864 1984 005a 1564 1a53 0029  .Z.d.d...Z.d.S.)
+00002e70: 1bda 0852 656d 696e 6465 7254 720e 0000  ...ReminderTr...
+00002e80: 0072 0100 0000 7253 0000 0072 5400 0000  .r....rS...rT...
+00002e90: da07 494e 5641 4c49 4472 5600 0000 6301  ..INVALIDrV...c.
+00002ea0: 0000 0000 0000 0000 0000 0001 0000 0006  ................
+00002eb0: 0000 0043 0000 0173 1c00 0000 6401 7c00  ...C...s....d.|.
+00002ec0: 6a00 9b00 6402 7c00 6a01 9b00 6403 7c00  j...d.|.j...d.|.
+00002ed0: 6a02 9b00 9d06 5300 2904 4e7a 1252 656d  j.....S.).Nz.Rem
+00002ee0: 696e 6465 7220 666f 7220 7573 6572 207a  inder for user z
+00002ef0: 0920 6f6e 2064 6174 6520 7a0e 2077 6974  . on date z. wit
+00002f00: 6820 6d65 7373 6167 6520 2903 da09 6175  h message )...au
+00002f10: 7468 6f72 5f69 64da 1372 656d 696e 6465  thor_id..reminde
+00002f20: 725f 6461 7465 5f65 706f 6368 da07 6d65  r_date_epoch..me
+00002f30: 7373 6167 6572 4c00 0000 7219 0000 0072  ssagerL...r....r
+00002f40: 1900 0000 721a 0000 0072 4e00 0000 8601  ....r....rN.....
+00002f50: 0000 7302 0000 0000 017a 1052 656d 696e  ..s......z.Remin
+00002f60: 6465 722e 5f5f 7374 725f 5f63 0100 0000  der.__str__c....
+00002f70: 0000 0000 0000 0000 0100 0000 0600 0000  ................
+00002f80: 4300 0001 732e 0000 0074 0074 016a 02a0  C...s....t.t.j..
+00002f90: 03a1 006a 0474 056a 056a 0674 07a0 0874  ...j.t.j.j.t...t
+00002fa0: 096a 0a9b 00a1 0164 018d 01a0 0ba1 0064  .j.....d.......d
+00002fb0: 028d 0183 0153 0029 034e 7209 0000 0029  .....S.).Nr....)
+00002fc0: 015a 1872 656d 696e 6465 725f 6461 7465  .Z.reminder_date
+00002fd0: 5f65 706f 6368 5f5f 6c74 6529 0c72 2e00  _epoch__lte).r..
+00002fe0: 0000 72bc 0000 0072 2000 0000 7243 0000  ..r....r ...rC..
+00002ff0: 0072 3000 0000 723c 0000 0072 3d00 0000  .r0...r<...r=...
+00003000: 72a4 0000 0072 0800 0000 7205 0000 0072  r....r....r....r
+00003010: a500 0000 723e 0000 0072 3100 0000 7219  ....r>...r1...r.
+00003020: 0000 0072 1900 0000 721a 0000 00da 1567  ...r....r......g
+00003030: 6574 5f65 7870 6972 6564 5f72 656d 696e  et_expired_remin
+00003040: 6465 7273 8901 0000 730e 0000 0000 0302  ders....s.......
+00003050: 010a 0106 010c ff08 ff04 ff7a 1e52 656d  ...........z.Rem
+00003060: 696e 6465 722e 6765 745f 6578 7069 7265  inder.get_expire
+00003070: 645f 7265 6d69 6e64 6572 7363 0200 0000  d_remindersc....
+00003080: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+00003090: 4300 0001 733c 0000 007c 019b 00a0 00a1  C...s<...|......
+000030a0: 0073 0e64 0053 0074 016a 02a0 03a1 006a  .s.d.S.t.j.....j
+000030b0: 047c 0164 018d 017d 0274 057c 0283 0164  .|.d...}.t.|...d
+000030c0: 026b 0272 3064 0053 007c 0264 0219 0053  .k.r0d.S.|.d...S
+000030d0: 0064 0053 0029 034e a901 da02 6964 7201  .d.S.).N....idr.
+000030e0: 0000 0029 06da 0769 7364 6967 6974 72bc  ...)...isdigitr.
+000030f0: 0000 0072 2000 0000 7243 0000 0072 3000  ...r ...rC...r0.
+00003100: 0000 7267 0000 0029 0372 2200 0000 5a0b  ..rg...).r"...Z.
+00003110: 7265 6d69 6e64 6572 5f69 645a 0972 656d  reminder_idZ.rem
+00003120: 696e 6465 7273 7219 0000 0072 1900 0000  indersr....r....
+00003130: 721a 0000 00da 1267 6574 5f72 656d 696e  r......get_remin
+00003140: 6465 725f 6279 5f69 6494 0100 0073 0c00  der_by_id....s..
+00003150: 0000 0003 0a01 0401 1201 0c01 0402 7a1b  ..............z.
+00003160: 5265 6d69 6e64 6572 2e67 6574 5f72 656d  Reminder.get_rem
+00003170: 696e 6465 725f 6279 5f69 6463 0200 0000  inder_by_idc....
+00003180: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00003190: 4300 0001 731a 0000 0074 006a 01a0 02a1  C...s....t.j....
+000031a0: 006a 037c 0164 018d 01a0 04a1 0001 0064  .j.|.d.........d
+000031b0: 0053 0029 024e 72c2 0000 0029 0572 bc00  .S.).Nr....).r..
+000031c0: 0000 7220 0000 0072 4300 0000 723a 0000  ..r ...rC...r:..
+000031d0: 0072 9f00 0000 a902 7222 0000 005a 1272  .r......r"...Z.r
+000031e0: 656d 696e 6465 725f 746f 5f64 656c 6574  eminder_to_delet
+000031f0: 6572 1900 0000 7219 0000 0072 1a00 0000  er....r....r....
+00003200: da15 6465 6c65 7465 5f72 656d 696e 6465  ..delete_reminde
+00003210: 725f 6279 5f69 64a0 0100 0073 0200 0000  r_by_id....s....
+00003220: 0003 7a1e 5265 6d69 6e64 6572 2e64 656c  ..z.Reminder.del
+00003230: 6574 655f 7265 6d69 6e64 6572 5f62 795f  ete_reminder_by_
+00003240: 6964 6302 0000 0000 0000 0000 0000 0002  idc.............
+00003250: 0000 0002 0000 0043 0000 0173 0c00 0000  .......C...s....
+00003260: 7c01 a000 a100 0100 6400 5300 725f 0000  |.......d.S.r_..
+00003270: 00a9 0172 9f00 0000 72c6 0000 0072 1900  ...r....r....r..
+00003280: 0000 7219 0000 0072 1a00 0000 da0f 6465  ..r....r......de
+00003290: 6c65 7465 5f72 656d 696e 6465 72a5 0100  lete_reminder...
+000032a0: 0073 0200 0000 0003 7a18 5265 6d69 6e64  .s......z.Remind
+000032b0: 6572 2e64 656c 6574 655f 7265 6d69 6e64  er.delete_remind
+000032c0: 6572 6302 0000 0000 0000 0000 0000 0002  erc.............
+000032d0: 0000 0004 0000 0043 0000 0173 1c00 0000  .......C...s....
+000032e0: 7400 7401 6a02 a003 a100 6a04 7c01 6401  t.t.j.....j.|.d.
+000032f0: 8d01 a005 6402 a101 8301 5300 2903 4e29  ....d.....S.).N)
+00003300: 0172 be00 0000 72bf 0000 0029 0672 2e00  .r....r....).r..
+00003310: 0000 72bc 0000 0072 2000 0000 7243 0000  ..r....r ...rC..
+00003320: 0072 3000 0000 728e 0000 0029 0272 2200  .r0...r....).r".
+00003330: 0000 72be 0000 0072 1900 0000 7219 0000  ..r....r....r...
+00003340: 0072 1a00 0000 da16 6765 745f 7265 6d69  .r......get_remi
+00003350: 6e64 6572 5f62 795f 6175 7468 6f72 aa01  nder_by_author..
+00003360: 0000 7302 0000 0000 037a 1f52 656d 696e  ..s......z.Remin
+00003370: 6465 722e 6765 745f 7265 6d69 6e64 6572  der.get_reminder
+00003380: 5f62 795f 6175 7468 6f72 6301 0000 0000  _by_authorc.....
+00003390: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
+000033a0: 0000 0173 1400 0000 7400 7401 6a02 a003  ...s....t.t.j...
+000033b0: a100 a004 6401 a101 8301 5300 2902 4e72  ....d.....S.).Nr
+000033c0: bf00 0000 2905 722e 0000 0072 bc00 0000  ....).r....r....
+000033d0: 7220 0000 0072 4300 0000 728e 0000 0072  r ...rC...r....r
+000033e0: 3100 0000 7219 0000 0072 1900 0000 721a  1...r....r....r.
+000033f0: 0000 00da 1167 6574 5f61 6c6c 5f72 656d  .....get_all_rem
+00003400: 696e 6465 7273 b001 0000 7302 0000 0000  inders....s.....
+00003410: 037a 1a52 656d 696e 6465 722e 6765 745f  .z.Reminder.get_
+00003420: 616c 6c5f 7265 6d69 6e64 6572 7363 0200  all_remindersc..
+00003430: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00003440: 0000 4300 0001 730c 0000 007c 01a0 00a1  ..C...s....|....
+00003450: 0001 0064 0053 0072 5f00 0000 7226 0000  ...d.S.r_...r&..
+00003460: 0029 0272 2200 0000 5a10 7265 6d69 6e64  .).r"...Z.remind
+00003470: 6572 5f74 6f5f 7361 7665 7219 0000 0072  er_to_saver....r
+00003480: 1900 0000 721a 0000 00da 0d73 6176 655f  ....r......save_
+00003490: 7265 6d69 6e64 6572 b601 0000 7302 0000  reminder....s...
+000034a0: 0000 037a 1652 656d 696e 6465 722e 7361  ...z.Reminder.sa
+000034b0: 7665 5f72 656d 696e 6465 7263 0100 0000  ve_reminderc....
+000034c0: 0000 0000 0000 0000 0600 0000 0400 0000  ................
+000034d0: 4300 0001 73b0 0000 0074 007c 006a 0174  C...s....t.|.j.t
+000034e0: 02a0 02a1 0018 0083 017d 017c 0164 011a  .........}.|.d..
+000034f0: 007d 027c 0164 0116 007d 017c 0164 021a  .}.|.d...}.|.d..
+00003500: 007d 037c 0164 023b 007d 017c 0164 031a  .}.|.d.;.}.|.d..
+00003510: 007d 047c 0164 033b 007d 0164 047d 057c  .}.|.d.;.}.d.}.|
+00003520: 0264 056b 0472 5e7c 0564 067c 029b 0064  .d.k.r^|.d.|...d
+00003530: 079d 0337 007d 057c 0364 056b 0472 767c  ...7.}.|.d.k.rv|
+00003540: 0564 067c 039b 0064 089d 0337 007d 057c  .d.|...d...7.}.|
+00003550: 0464 056b 0472 8e7c 0564 067c 049b 0064  .d.k.r.|.d.|...d
+00003560: 099d 0337 007d 057c 0164 056b 0472 a67c  ...7.}.|.d.k.r.|
+00003570: 0564 067c 019b 0064 0a9d 0337 007d 057c  .d.|...d...7.}.|
+00003580: 059b 0064 0b9d 0253 0029 0c4e 6980 5101  ...d...S.).Ni.Q.
+00003590: 0069 100e 0000 e93c 0000 007a 1152 656d  .i.....<...z.Rem
+000035a0: 696e 6465 7220 7365 7420 666f 7220 7201  inder set for r.
+000035b0: 0000 00fa 0120 7a05 2064 6179 737a 0620  ..... z. daysz. 
+000035c0: 686f 7572 737a 0820 6d69 6e75 7465 737a  hoursz. minutesz
+000035d0: 0820 7365 636f 6e64 737a 0920 6672 6f6d  . secondsz. from
+000035e0: 206e 6f77 2903 7236 0000 0072 bf00 0000   now).r6...r....
+000035f0: da04 7469 6d65 2906 724d 0000 00da 0773  ..time).rM.....s
+00003600: 6563 6f6e 6473 7272 0000 0072 7000 0000  econdsrr...rp...
+00003610: 72a2 0000 0072 c000 0000 7219 0000 0072  r....r....r....r
+00003620: 1900 0000 721a 0000 00da 0d67 6574 5f63  ....r......get_c
+00003630: 6f75 6e74 646f 776e bb01 0000 7322 0000  ountdown....s"..
+00003640: 0000 0112 0108 0108 0108 0108 0108 0108  ................
+00003650: 0204 0108 0110 0108 0110 0108 0110 0108  ................
+00003660: 0110 017a 1652 656d 696e 6465 722e 6765  ...z.Reminder.ge
+00003670: 745f 636f 756e 7464 6f77 6e4e 2916 7215  t_countdownN).r.
+00003680: 0000 0072 1600 0000 7217 0000 0072 0600  ...r....r....r..
+00003690: 0000 7279 0000 0072 c300 0000 7250 0000  ..ry...r....rP..
+000036a0: 0072 bf00 0000 724f 0000 0072 c000 0000  .r....rO...r....
+000036b0: 72be 0000 0072 4e00 0000 7251 0000 0072  r....rN...rQ...r
+000036c0: 0400 0000 72c1 0000 0072 c500 0000 72c7  ....r....r....r.
+000036d0: 0000 0072 c900 0000 72ca 0000 0072 cb00  ...r....r....r..
+000036e0: 0000 72cc 0000 0072 d100 0000 7219 0000  ..r....r....r...
+000036f0: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00003700: 72bc 0000 0077 0100 0073 4800 0000 0801  r....w...sH.....
+00003710: 0401 02ff 0603 0401 02ff 0603 0401 0201  ................
+00003720: 02fe 0604 0401 02ff 0604 0803 0201 0201  ................
+00003730: 0c09 0201 0201 0c0a 0201 0201 0c03 0201  ................
+00003740: 0201 0c03 0201 0201 0c04 0201 0201 0c04  ................
+00003750: 0201 0201 0c03 72bc 0000 0063 0000 0000  ......r....c....
+00003760: 0000 0000 0000 0000 0000 0000 0500 0000  ................
+00003770: 0000 0001 73c0 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
+00003780: 0265 036a 0464 0164 028d 015a 0565 036a  .e.j.d.d...Z.e.j
+00003790: 0664 0364 048d 015a 0765 036a 0864 0564  .d.d...Z.e.j.d.d
+000037a0: 0664 0164 078d 035a 0965 036a 0664 0364  .d.d...Z.e.j.d.d
+000037b0: 048d 015a 0a65 036a 0664 0864 098d 015a  ...Z.e.j.d.d...Z
+000037c0: 0b65 036a 0664 0864 098d 015a 0c65 0d64  .e.j.d.d...Z.e.d
+000037d0: 0a64 0b84 0083 015a 0e65 0d64 0c64 0d84  .d.....Z.e.d.d..
+000037e0: 0083 015a 0f65 1065 1164 0064 0e64 0f9c  ...Z.e.e.d.d.d..
+000037f0: 0264 1064 1184 0483 0183 015a 1265 1065  .d.d.......Z.e.e
+00003800: 1164 1264 1384 0083 0183 015a 1365 1065  .d.d.......Z.e.e
+00003810: 1164 1464 1584 0083 0183 015a 1487 0066  .d.d.......Z...f
+00003820: 0164 1664 1784 085a 1564 1864 1984 005a  .d.d...Z.d.d...Z
+00003830: 1687 0004 005a 1753 0029 1ada 0b48 656c  .....Z.S.)...Hel
+00003840: 704d 6573 7361 6765 5472 0e00 0000 4672  pMessageTr....Fr
+00003850: 1300 0000 72b2 0000 004e 2903 7211 0000  ....r....N).r...
+00003860: 0072 1400 0000 7212 0000 0072 0100 0000  .r....r....r....
+00003870: 7253 0000 0063 0100 0000 0000 0000 0000  rS...c..........
+00003880: 0000 0100 0000 0400 0000 4300 0001 7312  ..........C...s.
+00003890: 0000 0074 0074 016a 01a0 027c 006a 03a1  ...t.t.j...|.j..
+000038a0: 0183 0153 0072 5f00 0000 2904 da1b 636f  ...S.r_...)...co
+000038b0: 6e76 6572 745f 7574 635f 7469 6d65 5f74  nvert_utc_time_t
+000038c0: 6f5f 7061 6369 6669 6372 3c00 0000 72a3  o_pacificr<...r.
+000038d0: 0000 00da 1c68 656c 705f 6d65 7373 6167  .....help_messag
+000038e0: 655f 6578 7069 7261 7469 6f6e 5f64 6174  e_expiration_dat
+000038f0: 6572 4c00 0000 7219 0000 0072 1900 0000  erL...r....r....
+00003900: 721a 0000 00da 1767 6574 5f65 7870 6972  r......get_expir
+00003910: 6174 696f 6e5f 6461 7465 5f70 7374 d801  ation_date_pst..
+00003920: 0000 7302 0000 0000 027a 2348 656c 704d  ..s......z#HelpM
+00003930: 6573 7361 6765 2e67 6574 5f65 7870 6972  essage.get_expir
+00003940: 6174 696f 6e5f 6461 7465 5f70 7374 6301  ation_date_pstc.
+00003950: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+00003960: 0000 0043 0000 0173 1200 0000 7400 7401  ...C...s....t.t.
+00003970: 6a01 a002 7c00 6a03 a101 8301 5300 725f  j...|.j.....S.r_
+00003980: 0000 0029 0472 d300 0000 723c 0000 0072  ...).r....r<...r
+00003990: a300 0000 da0c 7469 6d65 5f63 7265 6174  ......time_creat
+000039a0: 6564 724c 0000 0072 1900 0000 7219 0000  edrL...r....r...
+000039b0: 0072 1a00 0000 da1c 6765 745f 7073 745f  .r......get_pst_
+000039c0: 6461 7465 5f6d 6573 7361 6765 5f63 7265  date_message_cre
+000039d0: 6174 6564 dc01 0000 7302 0000 0000 027a  ated....s......z
+000039e0: 2848 656c 704d 6573 7361 6765 2e67 6574  (HelpMessage.get
+000039f0: 5f70 7374 5f64 6174 655f 6d65 7373 6167  _pst_date_messag
+00003a00: 655f 6372 6561 7465 6472 1c00 0000 7224  e_createdr....r$
+00003a10: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00003a20: 0200 0000 0200 0000 4300 0001 730c 0000  ........C...s...
+00003a30: 007c 01a0 00a1 0001 0064 0153 0029 027a  .|.......d.S.).z
+00003a40: 1f41 6464 7320 656e 7472 7920 746f 2048  .Adds entry to H
+00003a50: 656c 704d 6573 7361 6765 2074 6162 6c65  elpMessage table
+00003a60: 4e72 2600 0000 7228 0000 0072 1900 0000  Nr&...r(...r....
+00003a70: 7219 0000 0072 1a00 0000 7229 0000 00e0  r....r....r)....
+00003a80: 0100 0073 0200 0000 0004 7a19 4865 6c70  ...s......z.Help
+00003a90: 4d65 7373 6167 652e 696e 7365 7274 5f72  Message.insert_r
+00003aa0: 6563 6f72 6463 0200 0000 0000 0000 0000  ecordc..........
+00003ab0: 0000 0200 0000 0200 0000 4300 0001 730c  ..........C...s.
+00003ac0: 0000 007c 01a0 00a1 0001 0064 0053 0072  ...|.......d.S.r
+00003ad0: 5f00 0000 72c8 0000 0029 0272 2200 0000  _...r....).r"...
+00003ae0: 5a1d 6865 6c70 5f6d 6573 7361 6765 5f72  Z.help_message_r
+00003af0: 6563 6f72 645f 746f 5f64 656c 6574 6572  ecord_to_deleter
+00003b00: 1900 0000 7219 0000 0072 1a00 0000 da0e  ....r....r......
+00003b10: 6465 6c65 7465 5f6d 6573 7361 6765 e601  delete_message..
+00003b20: 0000 7302 0000 0000 037a 1a48 656c 704d  ..s......z.HelpM
+00003b30: 6573 7361 6765 2e64 656c 6574 655f 6d65  essage.delete_me
+00003b40: 7373 6167 6563 0100 0000 0000 0000 0000  ssagec..........
+00003b50: 0000 0100 0000 0500 0000 4300 0001 7324  ..........C...s$
+00003b60: 0000 0074 0074 016a 02a0 03a1 006a 0474  ...t.t.j.....j.t
+00003b70: 0574 066a 06a0 07a1 0083 01a0 08a1 0064  .t.j...........d
+00003b80: 018d 0183 0153 0029 024e 2901 5a21 6865  .....S.).N).Z!he
+00003b90: 6c70 5f6d 6573 7361 6765 5f65 7870 6972  lp_message_expir
+00003ba0: 6174 696f 6e5f 6461 7465 5f5f 6c74 6529  ation_date__lte)
+00003bb0: 0972 2e00 0000 72d2 0000 0072 2000 0000  .r....r....r ...
+00003bc0: 7243 0000 0072 3000 0000 72d3 0000 0072  rC...r0...r....r
+00003bd0: 3c00 0000 723d 0000 0072 3e00 0000 7231  <...r=...r>...r1
+00003be0: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+00003bf0: 0000 da16 6765 745f 6d65 7373 6167 6573  ....get_messages
+00003c00: 5f74 6f5f 6465 6c65 7465 eb01 0000 730a  _to_delete....s.
+00003c10: 0000 0000 0302 010a 0110 ff04 ff7a 2248  .............z"H
+00003c20: 656c 704d 6573 7361 6765 2e67 6574 5f6d  elpMessage.get_m
+00003c30: 6573 7361 6765 735f 746f 5f64 656c 6574  essages_to_delet
+00003c40: 6563 0100 0000 0000 0000 0000 0000 0300  ec..............
+00003c50: 0000 0400 0000 0f00 0001 733a 0000 0074  ..........s:...t
+00003c60: 0074 016a 01a0 02a1 0083 0174 016a 0364  .t.j.......t.j.d
+00003c70: 0164 028d 0117 00a0 04a1 007c 005f 0574  .d.........|._.t
+00003c80: 0674 077c 0083 026a 087c 0169 007c 02a4  .t.|...j.|.i.|..
+00003c90: 018e 0101 0064 0053 0029 034e 720b 0000  .....d.S.).Nr...
+00003ca0: 0072 a100 0000 2909 72d3 0000 0072 3c00  .r....).r....r<.
+00003cb0: 0000 723d 0000 0072 a600 0000 723e 0000  ..r=...r....r>..
+00003cc0: 0072 d400 0000 7273 0000 0072 d200 0000  .r....rs...r....
+00003cd0: 7227 0000 0072 7400 0000 7277 0000 0072  r'...rt...rw...r
+00003ce0: 1900 0000 721a 0000 0072 2700 0000 f401  ....r....r'.....
+00003cf0: 0000 7306 0000 0000 0218 ff08 037a 1048  ..s..........z.H
+00003d00: 656c 704d 6573 7361 6765 2e73 6176 6563  elpMessage.savec
+00003d10: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00003d20: 0c00 0000 4300 0001 7334 0000 0064 017c  ....C...s4...d.|
+00003d30: 006a 009b 0064 027c 006a 019b 0064 037c  .j...d.|.j...d.|
+00003d40: 006a 029b 0064 047c 006a 039b 0064 057c  .j...d.|.j...d.|
+00003d50: 006a 04a0 0564 06a1 019b 0064 079d 0b53  .j...d.....d...S
+00003d60: 0029 084e 7a0d 5b48 656c 704d 6573 7361  .).Nz.[HelpMessa
+00003d70: 6765 207a 0e20 666f 7220 6368 616e 6e65  ge z. for channe
+00003d80: 6c20 23fa 0128 7a0e 2920 616e 6420 6d65  l #..(z.) and me
+00003d90: 7373 6167 6520 7a15 2074 6861 7420 7761  ssage z. that wa
+00003da0: 7320 6372 6561 7465 6420 6f6e 207a 1825  s created on z.%
+00003db0: 5920 2562 2025 2d64 2025 493a 254d 3a25  Y %b %-d %I:%M:%
+00003dc0: 5320 2570 2025 5a72 4600 0000 2906 72c3  S %p %ZrF...).r.
+00003dd0: 0000 0072 7b00 0000 da0a 6368 616e 6e65  ...r{.....channe
+00003de0: 6c5f 6964 da0a 6d65 7373 6167 655f 6964  l_id..message_id
+00003df0: 72d7 0000 00da 0873 7472 6674 696d 6572  r......strftimer
+00003e00: 4c00 0000 7219 0000 0072 1900 0000 721a  L...r....r....r.
+00003e10: 0000 0072 4e00 0000 fa01 0000 730c 0000  ...rN.......s...
+00003e20: 0000 021a 0104 ff04 020a fe06 ff7a 1348  .............z.H
+00003e30: 656c 704d 6573 7361 6765 2e5f 5f73 7472  elpMessage.__str
+00003e40: 5f5f 2918 7215 0000 0072 1600 0000 7217  __).r....r....r.
+00003e50: 0000 0072 0600 0000 7279 0000 0072 c300  ...r....ry...r..
+00003e60: 0000 7250 0000 0072 dc00 0000 724f 0000  ..rP...r....rO..
+00003e70: 0072 7b00 0000 72db 0000 0072 d400 0000  .r{...r....r....
+00003e80: 72d6 0000 0072 b100 0000 72d5 0000 0072  r....r....r....r
+00003e90: d700 0000 7251 0000 0072 0400 0000 7229  ....rQ...r....r)
+00003ea0: 0000 0072 d800 0000 72d9 0000 0072 2700  ...r....r....r'.
+00003eb0: 0000 724e 0000 0072 7c00 0000 7219 0000  ..rN...r|...r...
+00003ec0: 0072 1900 0000 7277 0000 0072 1a00 0000  .r....rw...r....
+00003ed0: 72d2 0000 00d0 0100 0073 2a00 0000 0801  r........s*.....
+00003ee0: 0c01 0c01 1001 0c01 0c01 0c02 0201 0a03  ................
+00003ef0: 0201 0a03 0201 0201 1404 0201 0201 0c03  ................
+00003f00: 0201 0201 0c07 0c06 72d2 0000 0063 0100  ........r....c..
+00003f10: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00003f20: 0000 4300 0001 730a 0000 007c 00a0 0074  ..C...s....|...t
+00003f30: 01a1 0153 0029 017a e80a 2020 2020 436f  ...S.).z..    Co
+00003f40: 6e76 6572 7420 7468 6520 6769 7665 6e20  nvert the given 
+00003f50: 5554 4320 7469 6d65 7a6f 6e65 206f 626a  UTC timezone obj
+00003f60: 6563 7420 746f 2061 2050 5354 2074 696d  ect to a PST tim
+00003f70: 657a 6f6e 6520 6f62 6a65 6374 0a0a 2020  ezone object..  
+00003f80: 2020 4b65 7977 6f72 6420 4172 6775 6d65    Keyword Argume
+00003f90: 6e74 730a 2020 2020 7574 635f 6461 7465  nts.    utc_date
+00003fa0: 7469 6d65 202d 2d20 7468 6520 6769 7665  time -- the give
+00003fb0: 6e20 5554 4320 7469 6d65 7a6f 6e65 206f  n UTC timezone o
+00003fc0: 626a 6563 7420 746f 2063 6f6e 7665 7274  bject to convert
+00003fd0: 0a0a 2020 2020 5265 7475 726e 0a20 2020  ..    Return.   
+00003fe0: 2064 6174 6574 696d 6520 2d2d 2074 6865   datetime -- the
+00003ff0: 2050 5354 2074 696d 657a 6f6e 6520 6571   PST timezone eq
+00004000: 7569 7661 6c65 6e74 206f 6620 7468 6520  uivalent of the 
+00004010: 7574 635f 6461 7465 7469 6d65 0a20 2020  utc_datetime.   
+00004020: 2029 02da 0a61 7374 696d 657a 6f6e 65da   )...astimezone.
+00004030: 0a50 4143 4946 4943 5f54 5a29 015a 0c75  .PACIFIC_TZ).Z.u
+00004040: 7463 5f64 6174 6574 696d 6572 1900 0000  tc_datetimer....
+00004050: 7219 0000 0072 1a00 0000 72d3 0000 0002  r....r....r.....
+00004060: 0200 0073 0200 0000 000a 72d3 0000 0063  ...s......r....c
+00004070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004080: 0500 0000 4000 0001 734c 0000 0065 005a  ....@...sL...e.Z
+00004090: 0164 005a 0265 036a 0464 0164 028d 015a  .d.Z.e.j.d.d...Z
+000040a0: 0565 036a 0464 0164 028d 015a 0665 0765  .e.j.d.d...Z.e.e
+000040b0: 0864 0064 0364 049c 0264 0564 0684 0483  .d.d.d...d.d....
+000040c0: 0183 015a 0965 0765 0864 0764 0884 0083  ...Z.e.e.d.d....
+000040d0: 0183 015a 0a64 0953 0029 0ada 0b45 6d62  ...Z.d.S.)...Emb
+000040e0: 6564 4176 6174 6172 6988 1300 0072 5700  edAvatari....rW.
+000040f0: 0000 721c 0000 0072 2400 0000 6302 0000  ..r....r$...c...
+00004100: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+00004110: 0043 0000 0173 0c00 0000 7c01 a000 a100  .C...s....|.....
+00004120: 0100 6401 5300 2902 7a1f 4164 6473 2065  ..d.S.).z.Adds e
+00004130: 6e74 7279 2074 6f20 456d 6265 6441 7661  ntry to EmbedAva
+00004140: 7461 7220 7461 626c 654e 7226 0000 0072  tar tableNr&...r
+00004150: 2800 0000 7219 0000 0072 1900 0000 721a  (...r....r....r.
+00004160: 0000 0072 2900 0000 1702 0000 7302 0000  ...r).......s...
+00004170: 0000 047a 1945 6d62 6564 4176 6174 6172  ...z.EmbedAvatar
+00004180: 2e69 6e73 6572 745f 7265 636f 7264 6302  .insert_recordc.
+00004190: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+000041a0: 0000 0043 0000 0173 2e00 0000 7400 6a01  ...C...s....t.j.
+000041b0: a002 a100 6a03 7c01 6401 8d01 7d02 7404  ....j.|.d...}.t.
+000041c0: 7c02 8301 6402 6b02 7222 6400 5300 7c02  |...d.k.r"d.S.|.
+000041d0: 6402 1900 5300 6400 5300 2903 4e29 01da  d...S.d.S.).N)..
+000041e0: 1261 7661 7461 725f 6469 7363 6f72 645f  .avatar_discord_
+000041f0: 7572 6c72 0100 0000 2905 72e0 0000 0072  urlr....).r....r
+00004200: 2000 0000 7243 0000 0072 3000 0000 7267   ...rC...r0...rg
+00004210: 0000 0029 0372 2200 0000 da03 7572 6c5a  ...).r".....urlZ
+00004220: 0761 7661 7461 7273 7219 0000 0072 1900  .avatarsr....r..
+00004230: 0000 721a 0000 00da 1167 6574 5f61 7661  ..r......get_ava
+00004240: 7461 725f 6279 5f75 726c 1d02 0000 7308  tar_by_url....s.
+00004250: 0000 0000 0312 010c 0104 027a 1d45 6d62  ...........z.Emb
+00004260: 6564 4176 6174 6172 2e67 6574 5f61 7661  edAvatar.get_ava
+00004270: 7461 725f 6279 5f75 726c 4e29 0b72 1500  tar_by_urlN).r..
+00004280: 0000 7216 0000 0072 1700 0000 7206 0000  ..r....r....r...
+00004290: 0072 4f00 0000 72e1 0000 005a 1c61 7661  .rO...r....Z.ava
+000042a0: 7461 725f 6469 7363 6f72 645f 7065 726d  tar_discord_perm
+000042b0: 616e 656e 745f 7572 6c72 5100 0000 7204  anent_urlrQ...r.
+000042c0: 0000 0072 2900 0000 72e3 0000 0072 1900  ...r)...r....r..
+000042d0: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
+000042e0: 0072 e000 0000 0f02 0000 7318 0000 0008  .r........s.....
+000042f0: 0104 0102 ff06 0304 0102 ff06 0402 0102  ................
+00004300: 0114 0402 0102 0172 e000 0000 2923 da0a  .......r....)#..
+00004310: 5f5f 6675 7475 7265 5f5f 7202 0000 00da  __future__r.....
+00004320: 0674 7970 696e 6772 0300 0000 723c 0000  .typingr....r<..
+00004330: 0072 9400 0000 72cf 0000 0072 a400 0000  .r....r....r....
+00004340: da0c 6173 6769 7265 662e 7379 6e63 7204  ..asgiref.syncr.
+00004350: 0000 00da 0b64 6a61 6e67 6f2e 636f 6e66  .....django.conf
+00004360: 7205 0000 00da 0964 6a61 6e67 6f2e 6462  r......django.db
+00004370: 7206 0000 005a 0c64 6a61 6e67 6f2e 666f  r....Z.django.fo
+00004380: 726d 7372 0700 0000 da0c 646a 616e 676f  rmsr......django
+00004390: 2e75 7469 6c73 7208 0000 005a 0b64 6174  .utilsr....Z.dat
+000043a0: 6575 7469 6c2e 747a 720a 0000 0072 a500  eutil.tzr....r..
+000043b0: 0000 5a05 6765 7474 7a72 df00 0000 5a0c  ..Z.gettzr....Z.
+000043c0: 6375 7374 6f6d 4669 656c 6473 720c 0000  customFieldsr...
+000043d0: 0072 a900 0000 da05 4d6f 6465 6c72 0d00  .r......Modelr..
+000043e0: 0000 7252 0000 0072 7d00 0000 728d 0000  ..rR...r}...r...
+000043f0: 0072 bc00 0000 72d2 0000 0072 d300 0000  .r....r....r....
+00004400: 72e0 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+00004410: 1900 0000 721a 0000 00da 083c 6d6f 6475  ....r......<modu
+00004420: 6c65 3e03 0000 0073 3000 0000 0c02 0c01  le>....s0.......
+00004430: 0801 0801 0801 0801 0c01 0c01 0c01 0c01  ................
+00004440: 0c01 0c03 0401 0a02 0c01 0803 1246 1251  .............F.Q
+00004450: 127f 0001 1247 1259 1232 080d            .....G.Y.2..
```

### Comparing `wall_e_models-0.8/wall_e_models/customFields.py` & `wall_e_models-0.9/wall_e_models/customFields.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 from django.db import models
 from django.conf import settings
 
 ENV = getattr(settings, "ENVIRONMENT", "LOCALHOST")
 database_type = getattr(settings, "database_type", "sqlite3")
 
+try:
+    # necessary if this is being called from wall_e and therefore the settings need to be picked up from
+    # django_settings instead of the settings file in the wall_e_models repo
+    import django_settings
+    ENV = getattr(django_settings, "ENVIRONMENT", "LOCALHOST")
+    database_type = getattr(django_settings, "database_type", "sqlite3")
+except ModuleNotFoundError:
+    pass
+
 
 class GeneratedIdentityField(models.AutoField):
     description = "An Integer column which uses `GENERATED {ALWAYS | BY DEFAULT} AS IDENTITY`. \
                   A modern alternative to `BIGSERIAL` from the SQL standard."
 
     def __init__(self, *args, **kwargs):
```

### Comparing `wall_e_models-0.8/wall_e_models/migrations/0001_initial.py` & `wall_e_models-0.9/wall_e_models/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/0002_auto_20220203_2111.py` & `wall_e_models-0.9/wall_e_models/migrations/0002_auto_20220203_2111.py`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/0003_auto_20220204_2003.py` & `wall_e_models-0.9/wall_e_models/migrations/0003_auto_20220204_2003.py`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/0004_auto_20220206_1142.py` & `wall_e_models-0.9/wall_e_models/migrations/0004_auto_20220206_1142.py`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/0007_auto_20230827_1520.py` & `wall_e_models-0.9/wall_e_models/migrations/0007_auto_20230827_1520.py`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/0009_helpmessage.py` & `wall_e_models-0.9/wall_e_models/migrations/0009_helpmessage.py`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/0010_embedavatar.py` & `wall_e_models-0.9/wall_e_models/migrations/0010_embedavatar.py`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/__pycache__/0001_initial.cpython-39.pyc` & `wall_e_models-0.9/wall_e_models/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/__pycache__/0002_auto_20220203_2111.cpython-39.pyc` & `wall_e_models-0.9/wall_e_models/migrations/__pycache__/0002_auto_20220203_2111.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/__pycache__/0003_auto_20220204_2003.cpython-39.pyc` & `wall_e_models-0.9/wall_e_models/migrations/__pycache__/0003_auto_20220204_2003.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/__pycache__/0004_auto_20220206_1142.cpython-39.pyc` & `wall_e_models-0.9/wall_e_models/migrations/__pycache__/0004_auto_20220206_1142.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/__pycache__/0005_auto_20220715_1532.cpython-39.pyc` & `wall_e_models-0.9/wall_e_models/migrations/__pycache__/0005_auto_20220715_1532.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/__pycache__/0006_auto_20220909_1633.cpython-39.pyc` & `wall_e_models-0.9/wall_e_models/migrations/__pycache__/0006_auto_20220909_1633.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/__pycache__/0007_auto_20230827_1520.cpython-39.pyc` & `wall_e_models-0.9/wall_e_models/migrations/__pycache__/0007_auto_20230827_1520.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/__pycache__/0008_rename_ban_id_banrecords_ban_d.cpython-39.pyc` & `wall_e_models-0.9/wall_e_models/migrations/__pycache__/0008_rename_ban_id_banrecords_ban_d.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/__pycache__/0008_rename_banrecords_banrecord.cpython-39.pyc` & `wall_e_models-0.9/wall_e_models/migrations/__pycache__/0008_rename_banrecords_banrecord.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/__pycache__/0009_helpmessage.cpython-39.pyc` & `wall_e_models-0.9/wall_e_models/migrations/__pycache__/0009_helpmessage.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/__pycache__/0010_auto_20230925_1253.cpython-39.pyc` & `wall_e_models-0.9/wall_e_models/migrations/__pycache__/0010_auto_20230925_1253.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/__pycache__/0010_embedavatar.cpython-39.pyc` & `wall_e_models-0.9/wall_e_models/migrations/__pycache__/0010_embedavatar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/migrations/__pycache__/0011_alter_helpmessage_channel_name.cpython-39.pyc` & `wall_e_models-0.9/wall_e_models/migrations/__pycache__/0011_alter_helpmessage_channel_name.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models/models.py` & `wall_e_models-0.9/wall_e_models/models.py`

 * *Files identical despite different names*

### Comparing `wall_e_models-0.8/wall_e_models.egg-info/PKG-INFO` & `wall_e_models-0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
-Name: wall-e-models
-Version: 0.8
+Name: wall_e_models
+Version: 0.9
 Summary: A Django app to manage CSSS's discord bot's database
 Home-page: https://github.com/CSSS/wall_e_models
 Author: Jace Manshadi
 Author-email: jaymanshad@proton.me
 License: GNU General Public License v3.0
 Description: ===============
         wall_e_models
```

### Comparing `wall_e_models-0.8/wall_e_models.egg-info/SOURCES.txt` & `wall_e_models-0.9/wall_e_models.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,8 +36,9 @@
 wall_e_models/migrations/__pycache__/0007_auto_20230827_1520.cpython-39.pyc
 wall_e_models/migrations/__pycache__/0008_rename_ban_id_banrecords_ban_d.cpython-39.pyc
 wall_e_models/migrations/__pycache__/0008_rename_banrecords_banrecord.cpython-39.pyc
 wall_e_models/migrations/__pycache__/0009_helpmessage.cpython-39.pyc
 wall_e_models/migrations/__pycache__/0010_auto_20230925_1253.cpython-39.pyc
 wall_e_models/migrations/__pycache__/0010_embedavatar.cpython-39.pyc
 wall_e_models/migrations/__pycache__/0011_alter_helpmessage_channel_name.cpython-39.pyc
+wall_e_models/migrations/__pycache__/0011_banrecord_unique_active_ban.cpython-39.pyc
 wall_e_models/migrations/__pycache__/__init__.cpython-39.pyc
```


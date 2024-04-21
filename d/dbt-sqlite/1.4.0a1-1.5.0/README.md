# Comparing `tmp/dbt-sqlite-1.4.0a1.tar.gz` & `tmp/dbt_sqlite-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-sqlite-1.4.0a1.tar", last modified: Wed Feb  1 07:31:15 2023, max compression
+gzip compressed data, was "dbt_sqlite-1.5.0.tar", last modified: Sun Apr 21 17:41:33 2024, max compression
```

## Comparing `dbt-sqlite-1.4.0a1.tar` & `dbt_sqlite-1.5.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-01 07:31:15.994466 dbt-sqlite-1.4.0a1/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)    11358 2020-07-30 19:40:08.000000 dbt-sqlite-1.4.0a1/LICENSE.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      559 2023-02-01 07:31:15.990466 dbt-sqlite-1.4.0a1/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     8169 2023-02-01 07:29:54.000000 dbt-sqlite-1.4.0a1/README.md
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-01 07:31:15.990466 dbt-sqlite-1.4.0a1/dbt/
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-01 07:31:15.990466 dbt-sqlite-1.4.0a1/dbt/adapters/
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-01 07:31:15.990466 dbt-sqlite-1.4.0a1/dbt/adapters/sqlite/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      383 2020-11-04 22:23:38.000000 dbt-sqlite-1.4.0a1/dbt/adapters/sqlite/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       20 2023-02-01 07:29:54.000000 dbt-sqlite-1.4.0a1/dbt/adapters/sqlite/__version__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     5858 2023-02-01 07:29:54.000000 dbt-sqlite-1.4.0a1/dbt/adapters/sqlite/connections.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     9664 2023-02-01 07:29:54.000000 dbt-sqlite-1.4.0a1/dbt/adapters/sqlite/impl.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      603 2023-02-01 07:29:54.000000 dbt-sqlite-1.4.0a1/dbt/adapters/sqlite/relation.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-01 07:31:15.990466 dbt-sqlite-1.4.0a1/dbt/include/
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-01 07:31:15.990466 dbt-sqlite-1.4.0a1/dbt/include/sqlite/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       51 2020-11-04 21:51:05.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       74 2020-11-04 21:51:05.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/dbt_project.yml
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-01 07:31:15.990466 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     4342 2022-07-16 07:22:37.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/adapters.sql
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      137 2020-11-05 08:14:56.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/catalog.sql
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      443 2020-11-07 19:15:20.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/core_overrides.sql
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-01 07:31:15.990466 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-01 07:31:15.990466 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/incremental/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3268 2023-02-01 06:48:56.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/incremental/incremental.sql
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-01 07:31:15.990466 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/seed/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       74 2022-08-19 15:14:36.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/seed/helpers.sql
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1325 2023-01-11 02:19:29.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/seed/seed.sql
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-01 07:31:15.990466 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/snapshot/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1152 2020-11-08 08:20:07.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/snapshot/snapshot_merge.sql
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      227 2022-07-20 01:22:59.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/snapshot/strategies.sql
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-01 07:31:15.990466 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/table/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1110 2023-02-01 06:47:19.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/table/table.sql
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      444 2021-08-10 23:43:07.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/test.sql
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-01 07:31:15.990466 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/view/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      983 2020-11-07 07:46:25.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/view/view.sql
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-01 07:31:15.990466 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/utils/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       87 2022-08-19 15:14:36.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/utils/any_value.sql
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       85 2022-08-19 15:14:36.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/utils/bool_or.sql
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      160 2022-08-19 15:14:36.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/utils/cast_bool_to_text.sql
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      187 2022-08-19 15:14:36.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/utils/dateadd.sql
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2567 2023-01-17 05:06:43.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/utils/datediff.sql
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      194 2022-08-19 15:14:36.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/utils/hash.sql
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      128 2022-08-19 15:14:36.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/utils/position.sql
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      242 2022-08-19 15:14:36.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/utils/right.sql
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      576 2021-07-08 16:26:54.000000 dbt-sqlite-1.4.0a1/dbt/include/sqlite/sample_profiles.yml
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-02-01 07:31:15.990466 dbt-sqlite-1.4.0a1/dbt_sqlite.egg-info/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      559 2023-02-01 07:31:15.000000 dbt-sqlite-1.4.0a1/dbt_sqlite.egg-info/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1443 2023-02-01 07:31:15.000000 dbt-sqlite-1.4.0a1/dbt_sqlite.egg-info/SOURCES.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2023-02-01 07:31:15.000000 dbt-sqlite-1.4.0a1/dbt_sqlite.egg-info/dependency_links.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       16 2023-02-01 07:31:15.000000 dbt-sqlite-1.4.0a1/dbt_sqlite.egg-info/requires.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        4 2023-02-01 07:31:15.000000 dbt-sqlite-1.4.0a1/dbt_sqlite.egg-info/top_level.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2023-02-01 07:31:15.994466 dbt-sqlite-1.4.0a1/setup.cfg
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1709 2023-02-01 07:29:54.000000 dbt-sqlite-1.4.0a1/setup.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-21 17:41:33.701237 dbt_sqlite-1.5.0/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)    11358 2020-07-30 19:40:08.000000 dbt_sqlite-1.5.0/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      588 2024-04-21 17:41:33.701237 dbt_sqlite-1.5.0/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     8227 2024-04-21 17:37:07.000000 dbt_sqlite-1.5.0/README.md
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-21 17:41:33.697236 dbt_sqlite-1.5.0/dbt/
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-21 17:41:33.697236 dbt_sqlite-1.5.0/dbt/adapters/
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-21 17:41:33.697236 dbt_sqlite-1.5.0/dbt/adapters/sqlite/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      383 2020-11-04 22:23:38.000000 dbt_sqlite-1.5.0/dbt/adapters/sqlite/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       18 2024-04-21 17:37:07.000000 dbt_sqlite-1.5.0/dbt/adapters/sqlite/__version__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     5881 2024-04-21 17:37:07.000000 dbt_sqlite-1.5.0/dbt/adapters/sqlite/connections.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     9664 2023-02-08 02:09:30.000000 dbt_sqlite-1.5.0/dbt/adapters/sqlite/impl.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      603 2023-02-08 02:09:30.000000 dbt_sqlite-1.5.0/dbt/adapters/sqlite/relation.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-21 17:41:33.697236 dbt_sqlite-1.5.0/dbt/include/
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-21 17:41:33.697236 dbt_sqlite-1.5.0/dbt/include/sqlite/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       51 2020-11-04 21:51:05.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       74 2020-11-04 21:51:05.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/dbt_project.yml
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-21 17:41:33.697236 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     4363 2024-04-21 17:37:07.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/adapters.sql
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      137 2020-11-05 08:14:56.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/catalog.sql
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      443 2020-11-07 19:15:20.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/core_overrides.sql
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-21 17:41:33.697236 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-21 17:41:33.697236 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/incremental/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3268 2023-02-01 06:48:56.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/incremental/incremental.sql
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-21 17:41:33.697236 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/seed/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       74 2022-08-19 15:14:36.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/seed/helpers.sql
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1325 2023-01-11 02:19:29.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/seed/seed.sql
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-21 17:41:33.697236 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/snapshot/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1152 2020-11-08 08:20:07.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/snapshot/snapshot_merge.sql
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      227 2022-07-20 01:22:59.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/snapshot/strategies.sql
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-21 17:41:33.697236 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/table/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1110 2023-02-08 02:09:30.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/table/table.sql
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      444 2021-08-10 23:43:07.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/test.sql
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-21 17:41:33.697236 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/view/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      983 2020-11-07 07:46:25.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/view/view.sql
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-21 17:41:33.701237 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/utils/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       87 2022-08-19 15:14:36.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/utils/any_value.sql
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       85 2022-08-19 15:14:36.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/utils/bool_or.sql
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      160 2022-08-19 15:14:36.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/utils/cast_bool_to_text.sql
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      187 2022-08-19 15:14:36.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/utils/dateadd.sql
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2567 2023-01-17 05:06:43.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/utils/datediff.sql
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      194 2022-08-19 15:14:36.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/utils/hash.sql
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      128 2022-08-19 15:14:36.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/utils/position.sql
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      242 2022-08-19 15:14:36.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/utils/right.sql
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      348 2024-04-21 17:37:07.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/macros/utils/timestamps.sql
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      576 2021-07-08 16:26:54.000000 dbt_sqlite-1.5.0/dbt/include/sqlite/sample_profiles.yml
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-21 17:41:33.701237 dbt_sqlite-1.5.0/dbt_sqlite.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      588 2024-04-21 17:41:33.000000 dbt_sqlite-1.5.0/dbt_sqlite.egg-info/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1490 2024-04-21 17:41:33.000000 dbt_sqlite-1.5.0/dbt_sqlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2024-04-21 17:41:33.000000 dbt_sqlite-1.5.0/dbt_sqlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       16 2024-04-21 17:41:33.000000 dbt_sqlite-1.5.0/dbt_sqlite.egg-info/requires.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        4 2024-04-21 17:41:33.000000 dbt_sqlite-1.5.0/dbt_sqlite.egg-info/top_level.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2024-04-21 17:41:33.701237 dbt_sqlite-1.5.0/setup.cfg
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1709 2024-04-21 17:37:07.000000 dbt_sqlite-1.5.0/setup.py
```

### Comparing `dbt-sqlite-1.4.0a1/LICENSE.txt` & `dbt_sqlite-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-sqlite-1.4.0a1/PKG-INFO` & `dbt_sqlite-1.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: dbt-sqlite
-Version: 1.4.0a1
+Version: 1.5.0
 Summary: A SQLite adapter plugin for dbt (data build tool)
 Home-page: https://github.com/codeforkjeff/dbt-sqlite
 Author: Jeff Chiu
 Author-email: jeff@codefork.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 License-File: LICENSE.txt
+Requires-Dist: dbt-core~=1.5.0
 
 Please see the github repository for detailed information
```

### Comparing `dbt-sqlite-1.4.0a1/README.md` & `dbt_sqlite-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 ## How to Use This
 
 Use the right version. Starting with the release of dbt-core 1.0.0,
 versions of dbt-sqlite are aligned to the same major+minor
 [version](https://semver.org/) of dbt-core.
 
+- versions 1.5.x of this adapter work with dbt-core 1.5.x
 - versions 1.4.x of this adapter work with dbt-core 1.4.x
 - versions 1.3.x of this adapter work with dbt-core 1.3.x
 - versions 1.2.x of this adapter work with dbt-core 1.2.x
 - versions 1.1.x of this adapter work with dbt-core 1.1.x
 - versions 1.0.x of this adapter work with dbt-core 1.0.x
 - versions 0.2.x of this adapter work with dbt 0.20.x and 0.21.x
 - versions 0.1.x of this adapter work with dbt 0.19.x
```

### Comparing `dbt-sqlite-1.4.0a1/dbt/adapters/sqlite/connections.py` & `dbt_sqlite-1.5.0/dbt/adapters/sqlite/connections.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 import glob
 import os.path
 import sqlite3
+from socket import gethostname
 from typing import Optional, Tuple, Any, Dict, List
 
 
 from dbt.adapters.base import Credentials
 from dbt.adapters.sql import SQLConnectionManager
 from dbt.contracts.connection import AdapterResponse
 from dbt.contracts.connection import Connection
@@ -33,15 +34,15 @@
 
     @property
     def unique_field(self):
         """
         Hashed and included in anonymous telemetry to track adapter adoption.
         Pick a field that can uniquely identify one team/organization building with this adapter
         """
-        return self.host
+        return gethostname()
 
     def _connection_keys(self):
         """ Keys to show when debugging """
         return ["database", "schema", "schemas_and_paths", "schema_directory" ]
 
 
 class SQLiteConnectionManager(SQLConnectionManager):
@@ -69,15 +70,15 @@
                 raise FailedToConnectError("at least one schema must be called 'main'")
 
             if len(credentials.extensions) > 0:
                 handle.enable_load_extension(True)
 
             for ext_path in credentials.extensions:
                 handle.load_extension(ext_path)
-            
+
             cursor = handle.cursor()
 
             for schema in set(schemas_and_paths.keys()) - set(['main']):
                 path = schemas_and_paths[schema]
                 cursor.execute(f"attach '{path}' as '{schema}'")
                 attached.append(schema)
```

### Comparing `dbt-sqlite-1.4.0a1/dbt/adapters/sqlite/impl.py` & `dbt_sqlite-1.5.0/dbt/adapters/sqlite/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-sqlite-1.4.0a1/dbt/adapters/sqlite/relation.py` & `dbt_sqlite-1.5.0/dbt/adapters/sqlite/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/adapters.sql` & `dbt_sqlite-1.5.0/dbt/include/sqlite/macros/adapters.sql`

 * *Files 17% similar despite different names*

```diff
@@ -75,48 +75,43 @@
         {% endcall %}
 
         {{ return(load_result('empty_table').table) }}
     {% endif %}
 {% endmacro %}
 
 {% macro sqlite__create_table_as(temporary, relation, sql) -%}
-      create {% if temporary -%}
+    {% set contract_config = config.get('contract') %}
+    {% if contract_config.enforced %}
+        {{exceptions.warn("Model contracts cannot be enforced by sqlite!")}}
+    {% endif %}
+    create {% if temporary -%}
         temporary
-      {%- endif %} table {{ relation }}
-      as
+    {%- endif %} table {{ relation }}
+    as
         {{ sql }}
 {% endmacro %}
 
 {% macro sqlite__create_view_as(relation, sql, auto_begin=False) -%}
+    {% set contract_config = config.get('contract') %}
+    {% if contract_config.enforced %}
+        {{exceptions.warn("Model contracts cannot be enforced by sqlite!")}}
+    {% endif %}
     create view {{ relation }} as
     {{ sql }};
 {%- endmacro %}
 
 {% macro sqlite__rename_relation(from_relation, to_relation) -%}
   {# no-op #}  
   {# see SQLiteAdapter.rename_relation() #}
 {% endmacro %}
 
-{% macro sqlite__snapshot_get_time() -%}
-  datetime()
-{%- endmacro %}
-
-{% macro sqlite__snapshot_string_as_time(timestamp) -%}
-    {# just return the string; SQLite doesn't have a timestamp data type per se #}
-    {{ return("'" + timestamp|string + "'") }}
-{%- endmacro %}
-
 {#
 the only allowable schema for temporary tables in SQLite is 'temp', so set
 that here when making the relation and everything else should Just Work
 #}
 {% macro sqlite__make_temp_relation(base_relation, suffix) %}
     {% set tmp_identifier = base_relation.identifier ~ suffix %}
     {% set tmp_relation = base_relation.incorporate(
                                 path={"schema": "temp", "identifier": tmp_identifier}) -%}
 
     {% do return(tmp_relation) %}
 {% endmacro %}
-
-{% macro sqlite__current_timestamp() -%}
-  datetime()
-{%- endmacro %}
```

### Comparing `dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/incremental/incremental.sql` & `dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/seed/seed.sql` & `dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/snapshot/snapshot_merge.sql` & `dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/table/table.sql` & `dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/materializations/view/view.sql` & `dbt_sqlite-1.5.0/dbt/include/sqlite/macros/materializations/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlite-1.4.0a1/dbt/include/sqlite/macros/utils/datediff.sql` & `dbt_sqlite-1.5.0/dbt/include/sqlite/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlite-1.4.0a1/dbt/include/sqlite/sample_profiles.yml` & `dbt_sqlite-1.5.0/dbt/include/sqlite/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-sqlite-1.4.0a1/dbt_sqlite.egg-info/PKG-INFO` & `dbt_sqlite-1.5.0/dbt_sqlite.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: dbt-sqlite
-Version: 1.4.0a1
+Version: 1.5.0
 Summary: A SQLite adapter plugin for dbt (data build tool)
 Home-page: https://github.com/codeforkjeff/dbt-sqlite
 Author: Jeff Chiu
 Author-email: jeff@codefork.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 License-File: LICENSE.txt
+Requires-Dist: dbt-core~=1.5.0
 
 Please see the github repository for detailed information
```

### Comparing `dbt-sqlite-1.4.0a1/dbt_sqlite.egg-info/SOURCES.txt` & `dbt_sqlite-1.5.0/dbt_sqlite.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,12 +24,13 @@
 dbt/include/sqlite/macros/utils/bool_or.sql
 dbt/include/sqlite/macros/utils/cast_bool_to_text.sql
 dbt/include/sqlite/macros/utils/dateadd.sql
 dbt/include/sqlite/macros/utils/datediff.sql
 dbt/include/sqlite/macros/utils/hash.sql
 dbt/include/sqlite/macros/utils/position.sql
 dbt/include/sqlite/macros/utils/right.sql
+dbt/include/sqlite/macros/utils/timestamps.sql
 dbt_sqlite.egg-info/PKG-INFO
 dbt_sqlite.egg-info/SOURCES.txt
 dbt_sqlite.egg-info/dependency_links.txt
 dbt_sqlite.egg-info/requires.txt
 dbt_sqlite.egg-info/top_level.txt
```

### Comparing `dbt-sqlite-1.4.0a1/setup.py` & `dbt_sqlite-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             'macros/**/*.sql',
             'macros/**/**/*.sql',
             'dbt_project.yml',
             'sample_profiles.yml',
         ]
     },
     install_requires=[
-        "dbt-core>=1.4.0"
+        "dbt-core~=1.5.0"
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
 
         'License :: OSI Approved :: Apache Software License',
 
         'Operating System :: Microsoft :: Windows',
```


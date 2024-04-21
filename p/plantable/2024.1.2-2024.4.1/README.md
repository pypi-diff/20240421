# Comparing `tmp/plantable-2024.1.2.tar.gz` & `tmp/plantable-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plantable-2024.1.2.tar", last modified: Sun Jan  7 23:41:56 2024, max compression
+gzip compressed data, was "plantable-2024.4.1.tar", last modified: Sun Apr 21 00:54:31 2024, max compression
```

## Comparing `plantable-2024.1.2.tar` & `plantable-2024.4.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-01-07 23:41:56.613530 plantable-2024.1.2/
--rw-r--r--   0 eugene    (1001) eugene    (1001)      831 2024-01-07 23:41:56.613530 plantable-2024.1.2/PKG-INFO
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     1149 2023-12-02 18:10:28.000000 plantable-2024.1.2/README.md
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      192 2023-12-02 18:10:28.000000 plantable-2024.1.2/pyproject.toml
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      853 2024-01-07 23:41:56.613530 plantable-2024.1.2/setup.cfg
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-01-07 23:41:56.605530 plantable-2024.1.2/src/
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-01-07 23:41:56.609530 plantable-2024.1.2/src/plantable/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      247 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/__init__.py
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-01-07 23:41:56.609530 plantable-2024.1.2/src/plantable/client/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      124 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/client/__init__.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     7939 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/client/account.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)    29740 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/client/admin.py
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-01-07 23:41:56.609530 plantable-2024.1.2/src/plantable/client/base/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       29 2023-12-02 18:56:48.000000 plantable-2024.1.2/src/plantable/client/base/__init__.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)    30799 2024-01-07 23:40:00.000000 plantable-2024.1.2/src/plantable/client/base/base.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)    35825 2023-12-17 02:56:14.000000 plantable-2024.1.2/src/plantable/client/base/builtin.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      326 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/client/conf.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     3310 2023-12-03 03:20:35.000000 plantable-2024.1.2/src/plantable/client/core.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       36 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/client/exception.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)    28076 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/client/user.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      622 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/const.py
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-01-07 23:41:56.609530 plantable-2024.1.2/src/plantable/model/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       84 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/model/__init__.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     3215 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/model/account.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     8255 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/model/column.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)    10046 2023-12-02 18:44:03.000000 plantable-2024.1.2/src/plantable/model/core.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     1088 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/model/event.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     1883 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/model/form.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      909 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/scripts.py
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-01-07 23:41:56.609530 plantable-2024.1.2/src/plantable/serde/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       96 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/serde/__init__.py
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-01-07 23:41:56.609530 plantable-2024.1.2/src/plantable/serde/deserializer/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      107 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/serde/deserializer/__init__.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     7488 2023-12-03 03:02:18.000000 plantable-2024.1.2/src/plantable/serde/deserializer/deserializer.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     4628 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/serde/deserializer/to_avro.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     9795 2023-12-03 02:29:19.000000 plantable-2024.1.2/src/plantable/serde/deserializer/to_postgres.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     8776 2023-12-03 03:04:17.000000 plantable-2024.1.2/src/plantable/serde/deserializer/to_python.py
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-01-07 23:41:56.609530 plantable-2024.1.2/src/plantable/serde/serializer/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       36 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/serde/serializer/__init__.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     3722 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/serde/serializer/from_arrow.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     3822 2024-01-07 07:22:59.000000 plantable-2024.1.2/src/plantable/serde/serializer/from_python.py
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-01-07 23:41:56.609530 plantable-2024.1.2/src/plantable/server/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)        0 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/server/__init__.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     1413 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/server/app.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      578 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/server/conf.py
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-01-07 23:41:56.609530 plantable-2024.1.2/src/plantable/server/router/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       30 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/server/router/__init__.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     1652 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/server/router/api_token.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     2250 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/server/router/user.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     3193 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/server/util.py
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-01-07 23:41:56.609530 plantable-2024.1.2/src/plantable/static/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)        0 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/static/__init__.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     2230 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/templates.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      458 2023-12-02 18:10:28.000000 plantable-2024.1.2/src/plantable/utils.py
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-01-07 23:41:56.609530 plantable-2024.1.2/src/plantable.egg-info/
--rw-r--r--   0 eugene    (1001) eugene    (1001)      831 2024-01-07 23:41:56.000000 plantable-2024.1.2/src/plantable.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     1552 2024-01-07 23:41:56.000000 plantable-2024.1.2/src/plantable.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1001) eugene    (1001)        1 2024-01-07 23:41:56.000000 plantable-2024.1.2/src/plantable.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       58 2024-01-07 23:41:56.000000 plantable-2024.1.2/src/plantable.egg-info/entry_points.txt
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      280 2024-01-07 23:41:56.000000 plantable-2024.1.2/src/plantable.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       10 2024-01-07 23:41:56.000000 plantable-2024.1.2/src/plantable.egg-info/top_level.txt
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-04-21 00:54:31.418772 plantable-2024.4.1/
+-rw-r--r--   0 eugene    (1001) eugene    (1001)      831 2024-04-21 00:54:31.418772 plantable-2024.4.1/PKG-INFO
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1149 2023-12-02 18:10:28.000000 plantable-2024.4.1/README.md
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      192 2023-12-02 18:10:28.000000 plantable-2024.4.1/pyproject.toml
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      853 2024-04-21 00:54:31.418772 plantable-2024.4.1/setup.cfg
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-04-21 00:54:31.414772 plantable-2024.4.1/src/
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-04-21 00:54:31.414772 plantable-2024.4.1/src/plantable/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      247 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/__init__.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-04-21 00:54:31.418772 plantable-2024.4.1/src/plantable/client/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      124 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/client/__init__.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     7965 2024-04-20 23:08:51.000000 plantable-2024.4.1/src/plantable/client/account.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)    29740 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/client/admin.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-04-21 00:54:31.418772 plantable-2024.4.1/src/plantable/client/base/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       29 2023-12-02 18:56:48.000000 plantable-2024.4.1/src/plantable/client/base/__init__.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)    31452 2024-04-20 23:14:51.000000 plantable-2024.4.1/src/plantable/client/base/base.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)    35825 2023-12-17 02:56:14.000000 plantable-2024.4.1/src/plantable/client/base/builtin.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      326 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/client/conf.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     3310 2023-12-03 03:20:35.000000 plantable-2024.4.1/src/plantable/client/core.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       36 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/client/exception.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)    28130 2024-04-20 23:08:51.000000 plantable-2024.4.1/src/plantable/client/user.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      622 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/const.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-04-21 00:54:31.418772 plantable-2024.4.1/src/plantable/model/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       84 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/model/__init__.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     3215 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/model/account.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     8255 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/model/column.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)    10062 2024-04-20 23:08:51.000000 plantable-2024.4.1/src/plantable/model/core.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1088 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/model/event.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1883 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/model/form.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      909 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/scripts.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-04-21 00:54:31.418772 plantable-2024.4.1/src/plantable/serde/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       96 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/serde/__init__.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-04-21 00:54:31.418772 plantable-2024.4.1/src/plantable/serde/deserializer/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      107 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/serde/deserializer/__init__.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     7472 2024-04-20 23:08:51.000000 plantable-2024.4.1/src/plantable/serde/deserializer/deserializer.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     4628 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/serde/deserializer/to_avro.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     9795 2023-12-03 02:29:19.000000 plantable-2024.4.1/src/plantable/serde/deserializer/to_postgres.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     8776 2023-12-03 03:04:17.000000 plantable-2024.4.1/src/plantable/serde/deserializer/to_python.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-04-21 00:54:31.418772 plantable-2024.4.1/src/plantable/serde/serializer/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       36 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/serde/serializer/__init__.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     3767 2024-04-20 23:08:51.000000 plantable-2024.4.1/src/plantable/serde/serializer/from_arrow.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     3822 2024-01-07 07:22:59.000000 plantable-2024.4.1/src/plantable/serde/serializer/from_python.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-04-21 00:54:31.418772 plantable-2024.4.1/src/plantable/server/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)        0 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/server/__init__.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1413 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/server/app.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      578 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/server/conf.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-04-21 00:54:31.418772 plantable-2024.4.1/src/plantable/server/router/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       30 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/server/router/__init__.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1652 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/server/router/api_token.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     2250 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/server/router/user.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     3193 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/server/util.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-04-21 00:54:31.418772 plantable-2024.4.1/src/plantable/static/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)        0 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/static/__init__.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     2230 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/templates.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      458 2023-12-02 18:10:28.000000 plantable-2024.4.1/src/plantable/utils.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2024-04-21 00:54:31.418772 plantable-2024.4.1/src/plantable.egg-info/
+-rw-r--r--   0 eugene    (1001) eugene    (1001)      831 2024-04-21 00:54:31.000000 plantable-2024.4.1/src/plantable.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1552 2024-04-21 00:54:31.000000 plantable-2024.4.1/src/plantable.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)        1 2024-04-21 00:54:31.000000 plantable-2024.4.1/src/plantable.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       58 2024-04-21 00:54:31.000000 plantable-2024.4.1/src/plantable.egg-info/entry_points.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      280 2024-04-21 00:54:31.000000 plantable-2024.4.1/src/plantable.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       10 2024-04-21 00:54:31.000000 plantable-2024.4.1/src/plantable.egg-info/top_level.txt
```

### Comparing `plantable-2024.1.2/PKG-INFO` & `plantable-2024.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantable
-Version: 2024.1.2
+Version: 2024.4.1
 Author: Woojin Cho
 Author-email: w.cho@cj.net
 License: MIT License
 Requires-Python: >=3.8
 Requires-Dist: aioboto3
 Requires-Dist: aiohttp
 Requires-Dist: aiokafka
```

### Comparing `plantable-2024.1.2/README.md` & `plantable-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/setup.cfg` & `plantable-2024.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/client/account.py` & `plantable-2024.4.1/src/plantable/client/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,27 @@
 
 import aiohttp
 import orjson
 import requests
 from pydantic import BaseModel
 from tabulate import tabulate
 
-from ..model import (DTABLE_ICON_COLORS, DTABLE_ICON_LIST, Admin, ApiToken, Base, BaseToken, Column, Table, Team, User,
-                     Webhook)
+from ..model import (
+    DTABLE_ICON_COLORS,
+    DTABLE_ICON_LIST,
+    Admin,
+    ApiToken,
+    Base,
+    BaseToken,
+    Column,
+    Table,
+    Team,
+    User,
+    Webhook,
+)
 from .base import BaseClient
 from .conf import SEATABLE_ACCOUNT_TOKEN, SEATABLE_PASSWORD, SEATABLE_URL, SEATABLE_USERNAME
 from .core import TABULATE_CONF, HttpClient
 
 logger = logging.getLogger()
```

### Comparing `plantable-2024.1.2/src/plantable/client/admin.py` & `plantable-2024.4.1/src/plantable/client/admin.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/client/base/base.py` & `plantable-2024.4.1/src/plantable/client/base/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -206,14 +206,15 @@
     # (OVERRIDE) Update Rows
     async def update_rows(
         self, table_name: str, updates: List[dict], add_link_if_not_exists: bool = False, refresh: bool = True
     ):
         link_columns = await self.list_link_columns(table_name=table_name, refresh=refresh)
         link_column_names = [x.name for x in link_columns]
 
+        # 순서에 따라 동작! asyncio.gather 금지!
         coros_create_row_links = list()
         for up in updates:
             for column_name in link_column_names:
                 if column_name in up["row"]:
                     display_values = up["row"].pop(column_name)
                     kwargs = await self._prep_create_row_links(
                         table_name=table_name,
@@ -249,29 +250,36 @@
             if input_column not in column_names:
                 _msg = f"table {table_name} does not have column '{input_column}'!"
                 raise ColumnNotExists(_msg)
 
     # Upsert Rows - 궁극의 메쏘드!
     # [NOTE] 첫 Column을 Unique하게 사용하기만 한다면, 이 메쏘드 하나만 써서 Append, Update 해결 가능!
     async def upsert_rows(
-        self, table_name: str, rows: List[dict], key_column: str = None, add_link_if_not_exists: bool = False
+        self,
+        table_name: str,
+        rows: List[dict],
+        key_column: str = None,
+        add_link_if_not_exists: bool = False,
+        raise_key_not_unique_error: bool = True,
     ):
         # correct input
         rows = rows if isinstance(rows, list) else [rows]
 
         # validate
         await self._validate_input_columns(table_name=table_name, rows=rows, refresh=True)
 
         # default key column is first column
         if not key_column:
             first_column = await self.get_first_column(table_name=table_name, refresh=False)
             key_column = first_column.name
 
         # get row id map
-        id_map = await self.get_row_id_map(table_name=table_name, key_column=key_column)
+        id_map = await self.get_row_id_map(
+            table_name=table_name, key_column=key_column, raise_key_not_unique_error=raise_key_not_unique_error
+        )
 
         # split updates & appends
         updates, appends = list(), list()
         for row in rows:
             key = row.get(key_column)
             if key is None or key not in id_map:
                 appends.append(row)
@@ -637,15 +645,20 @@
 
         other_rows_ids = prep.pop("other_rows_ids")
         prep.update({"other_table_row_id": other_rows_ids[0]})
         return prep
 
     # Prep - Create Row Links
     async def _prep_create_row_links(
-        self, table_name: str, column_name: str, display_values: list, add_link_if_not_exists: bool = False
+        self,
+        table_name: str,
+        column_name: str,
+        display_values: list,
+        add_link_if_not_exists: bool = False,
+        raise_key_not_unique_error: bool = True,
     ):
         # correct display values
         display_values = display_values if isinstance(display_values, list) else [display_values]
 
         table = await self.get_table(table_name=table_name, refresh=True)
         column = await self.get_column(table_name=table_name, column_name=column_name, refresh=False)
         if column.type != "link":
@@ -661,44 +674,54 @@
             _table = await self.get_table_by_id(table_id=column.data["table_id"], refresh=False)
             _other_table = table
         display_column_key = column.data["display_column_key"]
 
         display_column = await self.get_column_by_id(
             table_id=_other_table.id, column_id=display_column_key, refresh=False
         )
-        row_id_map = await self.get_row_id_map(table_name=_other_table.name, key_column=display_column.name)
+        row_id_map = await self.get_row_id_map(
+            table_name=_other_table.name,
+            key_column=display_column.name,
+            raise_key_not_unique_error=raise_key_not_unique_error,
+        )
 
         other_rows_ids = list()
         for display_value in display_values:
             if display_value not in row_id_map:
                 if not add_link_if_not_exists:
                     _msg = f"display value '{display_value}' not exists. please add this value into table '{_other_table.name}' first."
                     raise LinkValueNotExists(_msg)
                 # add link
                 await self.add_row(table_name=_other_table.name, row={display_column.name: display_value})
-                row_id_map = await self.get_row_id_map(table_name=_other_table.name, key_column=display_column.name)
+                row_id_map = await self.get_row_id_map(
+                    table_name=_other_table.name,
+                    key_column=display_column.name,
+                    raise_key_not_unique_error=raise_key_not_unique_error,
+                )
             other_rows_ids.append(row_id_map[display_value])
 
         return {
             "table_name": _table.name,
             "other_table_name": _other_table.name,
             "link_id": column.data["link_id"],
             "other_rows_ids": other_rows_ids,
         }
 
     # Get Ohter Rows Ids
-    async def get_other_rows_ids(self, table_name, column_name):
+    async def get_other_rows_ids(self, table_name, column_name, raise_key_not_unique_error: bool = True):
         link = await self.get_link(table_name=table_name, column_name=column_name)
         other_table = await self.get_table_by_id(table_id=link["other_table_id"])
         for column in other_table.columns:
             if column.key == link["display_column_key"]:
                 break
         else:
             raise KeyError
-        return await self.get_row_id_map(table_name=other_table.name, key_column=column.name)
+        return await self.get_row_id_map(
+            table_name=other_table.name, key_column=column.name, raise_key_not_unique_error=raise_key_not_unique_error
+        )
 
     ################################################################
     # FILES & IMAGES
     ################################################################
 
     ################################################################
     # TABLES
```

### Comparing `plantable-2024.1.2/src/plantable/client/base/builtin.py` & `plantable-2024.4.1/src/plantable/client/base/builtin.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/client/core.py` & `plantable-2024.4.1/src/plantable/client/core.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/client/user.py` & `plantable-2024.4.1/src/plantable/client/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,34 @@
 from typing import List, Union
 
 import aiohttp
 import orjson
 from pydantic import BaseModel
 from tabulate import tabulate
 
-from ..model import (DTABLE_ICON_COLORS, DTABLE_ICON_LIST, AccountInfo, Activity, Admin, ApiToken, Base, BaseInfo,
-                     BaseToken, Column, File, SharedView, Table, Team, User, UserInfo, Webhook, Workspace)
+from ..model import (
+    DTABLE_ICON_COLORS,
+    DTABLE_ICON_LIST,
+    AccountInfo,
+    Activity,
+    Admin,
+    ApiToken,
+    Base,
+    BaseInfo,
+    BaseToken,
+    Column,
+    File,
+    SharedView,
+    Table,
+    Team,
+    User,
+    UserInfo,
+    Webhook,
+    Workspace,
+)
 from .account import AccountClient
 from .core import parse_name
 
 logger = logging.getLogger()
 
 
 ################################################################
```

### Comparing `plantable-2024.1.2/src/plantable/const.py` & `plantable-2024.4.1/src/plantable/const.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/model/account.py` & `plantable-2024.4.1/src/plantable/model/account.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/model/column.py` & `plantable-2024.4.1/src/plantable/model/column.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/model/core.py` & `plantable-2024.4.1/src/plantable/model/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,17 @@
     contact_email: str = None  # "michael@example.com"
     login_id: str = None  # ""
     group_id: str = None  # 1
     id_in_org: str = None  # ''
     is_admin: bool = None  # true
     role: str = None  # "Owner
     permission: str = None  # "r" or "rw"
-    avatar_url: str = None  # "https://cloud.seatable.io/image-view/avatars/3/7/a0a57575a3ca0c78e8c5b6b0d0dbda/resized/80/cd7f6edd2c75afd3b7299917b3767c0f.png"
+    avatar_url: str = (
+        None  # "https://cloud.seatable.io/image-view/avatars/3/7/a0a57575a3ca0c78e8c5b6b0d0dbda/resized/80/cd7f6edd2c75afd3b7299917b3767c0f.png"
+    )
 
 
 class Base(_Model):
     id: int = None
     workspace_id: int  # 3
     uuid: str  # '166424ad-b023-47a0-9a35-76077f5b629b'
     name: str  # 'employee'
```

### Comparing `plantable-2024.1.2/src/plantable/model/event.py` & `plantable-2024.4.1/src/plantable/model/event.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/model/form.py` & `plantable-2024.4.1/src/plantable/model/form.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/scripts.py` & `plantable-2024.4.1/src/plantable/scripts.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/serde/deserializer/deserializer.py` & `plantable-2024.4.1/src/plantable/serde/deserializer/deserializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,20 +135,18 @@
         self.mtime_column = None
         self.last_modified = None
 
         self.init_columns()
 
     @property
     @abstractmethod
-    def Deserializer(self):
-        ...
+    def Deserializer(self): ...
 
     @abstractmethod
-    def schema(self):
-        ...
+    def schema(self): ...
 
     def generate_table_name(self):
         if self.table_name_prefix:
             return self.table_name_sep.join([self.table_name_prefix, self.table.name])
         return self.table.name
 
     def init_columns(self):
```

### Comparing `plantable-2024.1.2/src/plantable/serde/deserializer/to_avro.py` & `plantable-2024.4.1/src/plantable/serde/deserializer/to_avro.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/serde/deserializer/to_postgres.py` & `plantable-2024.4.1/src/plantable/serde/deserializer/to_postgres.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/serde/deserializer/to_python.py` & `plantable-2024.4.1/src/plantable/serde/deserializer/to_python.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/serde/serializer/from_arrow.py` & `plantable-2024.4.1/src/plantable/serde/serializer/from_arrow.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,38 @@
 import parse
 import pyarrow as pa
 
 from ...const import SYSTEM_FIELDS
-from ...model.column import (AutoNumber, Button, Checkbox, Collaborator, CreationTime, Creator, Date, Datetime,
-                             Duration, Email, File, Formula, Image, Integer, LastModificationTime, LastModifier, Link,
-                             LinkFomula, LongText, MultipleSelect, Number, Rate, SingleSelect, Text, Url)
+from ...model.column import (
+    AutoNumber,
+    Button,
+    Checkbox,
+    Collaborator,
+    CreationTime,
+    Creator,
+    Date,
+    Datetime,
+    Duration,
+    Email,
+    File,
+    Formula,
+    Image,
+    Integer,
+    LastModificationTime,
+    LastModifier,
+    Link,
+    LinkFomula,
+    LongText,
+    MultipleSelect,
+    Number,
+    Rate,
+    SingleSelect,
+    Text,
+    Url,
+)
 
 # Arrow to Seatable Schema
 SCHEMA_MAP = {
     "bool": Checkbox,
     "int8": Integer,
     "int16": Integer,
     "int32": Integer,
```

### Comparing `plantable-2024.1.2/src/plantable/serde/serializer/from_python.py` & `plantable-2024.4.1/src/plantable/serde/serializer/from_python.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/server/app.py` & `plantable-2024.4.1/src/plantable/server/app.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/server/conf.py` & `plantable-2024.4.1/src/plantable/server/conf.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/server/router/api_token.py` & `plantable-2024.4.1/src/plantable/server/router/api_token.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/server/router/user.py` & `plantable-2024.4.1/src/plantable/server/router/user.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/server/util.py` & `plantable-2024.4.1/src/plantable/server/util.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable/templates.py` & `plantable-2024.4.1/src/plantable/templates.py`

 * *Files identical despite different names*

### Comparing `plantable-2024.1.2/src/plantable.egg-info/PKG-INFO` & `plantable-2024.4.1/src/plantable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantable
-Version: 2024.1.2
+Version: 2024.4.1
 Author: Woojin Cho
 Author-email: w.cho@cj.net
 License: MIT License
 Requires-Python: >=3.8
 Requires-Dist: aioboto3
 Requires-Dist: aiohttp
 Requires-Dist: aiokafka
```

### Comparing `plantable-2024.1.2/src/plantable.egg-info/SOURCES.txt` & `plantable-2024.4.1/src/plantable.egg-info/SOURCES.txt`

 * *Files identical despite different names*


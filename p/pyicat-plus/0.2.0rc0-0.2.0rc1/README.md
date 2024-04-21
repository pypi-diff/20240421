# Comparing `tmp/pyicat_plus-0.2.0rc0.tar.gz` & `tmp/pyicat_plus-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyicat_plus-0.2.0rc0.tar", last modified: Thu Apr 18 16:50:17 2024, max compression
+gzip compressed data, was "pyicat_plus-0.2.0rc1.tar", last modified: Fri Apr 19 11:39:30 2024, max compression
```

## Comparing `pyicat_plus-0.2.0rc0.tar` & `pyicat_plus-0.2.0rc1.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.292371 pyicat_plus-0.2.0rc0/
--rw-rw-rw-   0 root         (0) root         (0)     7560 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     3672 2024-04-18 16:50:17.292371 pyicat_plus-0.2.0rc0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1323 2024-04-08 07:20:19.000000 pyicat_plus-0.2.0rc0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1636 2024-04-18 16:50:17.292371 pyicat_plus-0.2.0rc0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.284371 pyicat_plus-0.2.0rc0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.284371 pyicat_plus-0.2.0rc0/src/pyicat_plus/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-18 16:48:56.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.284371 pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 16:50:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2879 2024-04-08 07:20:19.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/icat_as_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/store_from_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/store_processed.py
--rw-rw-rw-   0 root         (0) root         (0)     2728 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/store_raw.py
--rw-rw-rw-   0 root         (0) root         (0)    17512 2024-04-03 00:21:24.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/sync_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.284371 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 16:50:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1138 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/add_files.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/archive.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/bliss.py
--rw-rw-rw-   0 root         (0) root         (0)      647 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     7708 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/elogbook.py
--rw-rw-rw-   0 root         (0) root         (0)     6376 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/interface.py
--rw-rw-rw-   0 root         (0) root         (0)    14265 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/investigation.py
--rw-rw-rw-   0 root         (0) root         (0)    19360 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/main.py
--rw-rw-rw-   0 root         (0) root         (0)     4049 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/messaging.py
--rw-rw-rw-   0 root         (0) root         (0)     2723 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     1731 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/null.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     1714 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/update_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     2763 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/client/xmlns.py
--rw-rw-rw-   0 root         (0) root         (0)     1557 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/concurrency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.288371 pyicat_plus-0.2.0rc0/src/pyicat_plus/metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 16:50:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11075 2024-04-08 07:20:19.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/metadata/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     2168 2024-04-18 15:13:55.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/metadata/namespace_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     2156 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/metadata/nexus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.288371 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 16:50:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      482 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.288371 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 16:50:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11429 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/icat.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/proc.py
--rw-rw-rw-   0 root         (0) root         (0)     3117 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/tcp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.288371 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 16:50:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2858 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/activemq_rest_server.py
--rw-rw-rw-   0 root         (0) root         (0)     4484 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/icat_db.py
--rw-rw-rw-   0 root         (0) root         (0)     9204 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/icatplus_server.py
--rw-rw-rw-   0 root         (0) root         (0)     2386 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/stomp_publisher.py
--rw-rw-rw-   0 root         (0) root         (0)     6660 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/stomp_subscriber.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4054 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     4316 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_elogbook.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_add_files.py
--rw-rw-rw-   0 root         (0) root         (0)     1560 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_archive.py
--rw-rw-rw-   0 root         (0) root         (0)     3806 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_datasets.py
--rw-rw-rw-   0 root         (0) root         (0)      731 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)    15798 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_investigations.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_mockup.py
--rw-rw-rw-   0 root         (0) root         (0)     3800 2024-04-08 07:20:19.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     1434 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_serialize.py
--rw-rw-rw-   0 root         (0) root         (0)    21005 2024-04-03 00:12:57.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_sync.py
--rw-rw-rw-   0 root         (0) root         (0)     4548 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_update_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_maxsizedict.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2024-04-07 16:03:54.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_namespace.py
--rw-rw-rw-   0 root         (0) root         (0)     1620 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_url_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.288371 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 16:50:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/utils/compare.py
--rw-rw-rw-   0 root         (0) root         (0)     1054 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/utils/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.288371 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 16:50:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1253 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/log_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/maxsizedict.py
--rw-rw-rw-   0 root         (0) root         (0)      584 2024-04-02 17:52:39.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/path_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6944 2024-04-02 17:52:39.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/raw_data.py
--rw-rw-rw-   0 root         (0) root         (0)    12868 2024-04-03 00:21:24.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/sync_store.py
--rw-rw-rw-   0 root         (0) root         (0)    12546 2024-04-02 17:52:39.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/sync_types.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:50:17.288371 pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3672 2024-04-18 16:50:17.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2878 2024-04-18 16:50:17.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 16:50:17.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      297 2024-04-18 16:50:17.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      521 2024-04-18 16:50:17.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-18 16:50:17.000000 pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.350351 pyicat_plus-0.2.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     7560 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     3672 2024-04-19 11:39:30.350351 pyicat_plus-0.2.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2024-04-08 07:20:19.000000 pyicat_plus-0.2.0rc1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1636 2024-04-19 11:39:30.350351 pyicat_plus-0.2.0rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.342352 pyicat_plus-0.2.0rc1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.342352 pyicat_plus-0.2.0rc1/src/pyicat_plus/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-19 11:37:04.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.342352 pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 11:39:26.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2879 2024-04-08 07:20:19.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/icat_as_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/store_from_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/store_processed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2728 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/store_raw.py
+-rw-rw-rw-   0 root         (0) root         (0)    17512 2024-04-03 00:21:24.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/sync_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.346351 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 11:39:26.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1138 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/add_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/archive.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/bliss.py
+-rw-rw-rw-   0 root         (0) root         (0)      647 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)     7708 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/elogbook.py
+-rw-rw-rw-   0 root         (0) root         (0)     6376 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/interface.py
+-rw-rw-rw-   0 root         (0) root         (0)    14265 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/investigation.py
+-rw-rw-rw-   0 root         (0) root         (0)    19360 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     4049 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/messaging.py
+-rw-rw-rw-   0 root         (0) root         (0)     2723 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/null.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/update_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2763 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/xmlns.py
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/concurrency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.346351 pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 11:39:26.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11075 2024-04-08 07:20:19.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2024-04-19 05:17:41.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/hdf5_cfg.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2168 2024-04-18 15:13:55.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/namespace_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     2156 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/nexus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.346351 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 11:39:26.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      482 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.346351 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 11:39:26.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11429 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/icat.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/proc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3117 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/tcp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.346351 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 11:39:26.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2858 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/activemq_rest_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     4484 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/icat_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     9204 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/icatplus_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     2386 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/stomp_publisher.py
+-rw-rw-rw-   0 root         (0) root         (0)     6660 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/stomp_subscriber.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4054 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     4316 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_elogbook.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_add_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     3806 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)      731 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15798 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_investigations.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_mockup.py
+-rw-rw-rw-   0 root         (0) root         (0)     3800 2024-04-08 07:20:19.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)    21005 2024-04-03 00:12:57.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_sync.py
+-rw-rw-rw-   0 root         (0) root         (0)     4548 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_update_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_maxsizedict.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2024-04-07 16:03:54.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_namespace.py
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_url_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.346351 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 11:39:26.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/utils/compare.py
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/utils/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.346351 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 11:39:26.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1253 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/log_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      521 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/maxsizedict.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2024-04-02 17:52:39.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/path_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6944 2024-04-02 17:52:39.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/raw_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    12868 2024-04-03 00:21:24.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/sync_store.py
+-rw-rw-rw-   0 root         (0) root         (0)    12546 2024-04-02 17:52:39.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/sync_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.350351 pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3672 2024-04-19 11:39:30.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2916 2024-04-19 11:39:30.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 11:39:30.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      297 2024-04-19 11:39:30.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      521 2024-04-19 11:39:30.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-19 11:39:30.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/top_level.txt
```

### Comparing `pyicat_plus-0.2.0rc0/LICENSE.md` & `pyicat_plus-0.2.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/PKG-INFO` & `pyicat_plus-0.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyicat-plus
-Version: 0.2.0rc0
+Version: 0.2.0rc1
 Summary: Python client to ICAT+
 Home-page: https://gitlab.esrf.fr/icat/pyicat-plus/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/icat/pyicat-plus/
 Project-URL: Documentation, https://pyicat-plus.readthedocs.io/
```

### Comparing `pyicat_plus-0.2.0rc0/README.md` & `pyicat_plus-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/setup.cfg` & `pyicat_plus-0.2.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/icat_as_nexus.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/icat_as_nexus.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/store_from_file.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/store_from_file.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/store_processed.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/store_processed.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/store_raw.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/store_raw.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/apps/sync_raw.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/sync_raw.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/add_files.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/add_files.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/archive.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/archive.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/bliss.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/bliss.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/defaults.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/defaults.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/elogbook.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/elogbook.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/interface.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/interface.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/investigation.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/investigation.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/main.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/main.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/messaging.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/messaging.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/metadata.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/metadata.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/null.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/null.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/serialize.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/serialize.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/update_metadata.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/update_metadata.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/client/xmlns.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/xmlns.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/concurrency.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/concurrency.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/metadata/definitions.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/definitions.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/metadata/namespace_wrapper.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/namespace_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/metadata/nexus.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/nexus.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/icat.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/icat.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/proc.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/proc.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/fixtures/tcp.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/tcp.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/activemq_rest_server.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/activemq_rest_server.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/icat_db.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/icat_db.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/icatplus_server.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/icatplus_server.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/stomp_publisher.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/stomp_publisher.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/servers/stomp_subscriber.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/stomp_subscriber.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_cli.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_elogbook.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_elogbook.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_add_files.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_add_files.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_archive.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_archive.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_datasets.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_datasets.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_definitions.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_definitions.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_investigations.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_investigations.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_nexus.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_nexus.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_serialize.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_serialize.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_sync.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_sync.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_icat_update_metadata.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_update_metadata.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_namespace.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/test_url_utils.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_url_utils.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/utils/compare.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/utils/compare.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/tests/utils/message.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/utils/message.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/log_utils.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/maxsizedict.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/maxsizedict.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/path_utils.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/raw_data.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/raw_data.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/sync_store.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/sync_store.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/sync_types.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/sync_types.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus/utils/url.py` & `pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/url.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/PKG-INFO` & `pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyicat-plus
-Version: 0.2.0rc0
+Version: 0.2.0rc1
 Summary: Python client to ICAT+
 Home-page: https://gitlab.esrf.fr/icat/pyicat-plus/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/icat/pyicat-plus/
 Project-URL: Documentation, https://pyicat-plus.readthedocs.io/
```

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/SOURCES.txt` & `pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 src/pyicat_plus/client/metadata.py
 src/pyicat_plus/client/null.py
 src/pyicat_plus/client/serialize.py
 src/pyicat_plus/client/update_metadata.py
 src/pyicat_plus/client/xmlns.py
 src/pyicat_plus/metadata/__init__.py
 src/pyicat_plus/metadata/definitions.py
+src/pyicat_plus/metadata/hdf5_cfg.xml
 src/pyicat_plus/metadata/namespace_wrapper.py
 src/pyicat_plus/metadata/nexus.py
 src/pyicat_plus/tests/__init__.py
 src/pyicat_plus/tests/conftest.py
 src/pyicat_plus/tests/test_cli.py
 src/pyicat_plus/tests/test_elogbook.py
 src/pyicat_plus/tests/test_icat_add_files.py
```

### Comparing `pyicat_plus-0.2.0rc0/src/pyicat_plus.egg-info/requires.txt` & `pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/requires.txt`

 * *Files identical despite different names*


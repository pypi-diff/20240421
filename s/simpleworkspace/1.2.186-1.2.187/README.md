# Comparing `tmp/simpleworkspace-1.2.186.tar.gz` & `tmp/simpleworkspace-1.2.187.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleworkspace-1.2.186.tar", last modified: Fri Apr 19 16:42:02 2024, max compression
+gzip compressed data, was "simpleworkspace-1.2.187.tar", last modified: Sun Apr 21 08:01:09 2024, max compression
```

## Comparing `simpleworkspace-1.2.186.tar` & `simpleworkspace-1.2.187.tar`

### file list

```diff
@@ -1,105 +1,109 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:02.061323 simpleworkspace-1.2.186/
--rw-rw-rw-   0        0        0       22 2024-01-29 16:35:42.000000 simpleworkspace-1.2.186/MANIFEST.in
--rw-rw-rw-   0        0        0      148 2024-04-19 16:42:02.052811 simpleworkspace-1.2.186/PKG-INFO
--rw-rw-rw-   0        0        0      313 2024-04-19 16:39:50.000000 simpleworkspace-1.2.186/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-19 16:42:02.061323 simpleworkspace-1.2.186/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.225094 simpleworkspace-1.2.186/src/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.391466 simpleworkspace-1.2.186/src/simpleworkspace/
--rw-rw-rw-   0        0        0        0 2024-01-22 08:55:41.000000 simpleworkspace-1.2.186/src/simpleworkspace/__init__.py
--rw-rw-rw-   0        0        0      453 2023-12-11 19:38:16.000000 simpleworkspace-1.2.186/src/simpleworkspace/__lazyimporter__.py
--rw-rw-rw-   0        0        0     2458 2024-02-05 17:50:15.000000 simpleworkspace-1.2.186/src/simpleworkspace/app.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.468494 simpleworkspace-1.2.186/src/simpleworkspace/assets/
--rw-rw-rw-   0        0        0      561 2024-02-24 14:57:44.000000 simpleworkspace-1.2.186/src/simpleworkspace/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.479141 simpleworkspace-1.2.186/src/simpleworkspace/assets/__pycache__/
--rw-rw-rw-   0        0        0      658 2024-01-24 15:01:20.000000 simpleworkspace-1.2.186/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      876 2024-02-24 15:09:13.000000 simpleworkspace-1.2.186/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.254372 simpleworkspace-1.2.186/src/simpleworkspace/assets/audio/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.482373 simpleworkspace-1.2.186/src/simpleworkspace/assets/audio/alarms/
--rw-rw-rw-   0        0        0   115582 2024-02-24 14:31:08.000000 simpleworkspace-1.2.186/src/simpleworkspace/assets/audio/alarms/Siren.wav
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.540544 simpleworkspace-1.2.186/src/simpleworkspace/assets/audio/notifications/
--rw-rw-rw-   0        0        0   168352 2024-02-24 14:26:13.000000 simpleworkspace-1.2.186/src/simpleworkspace/assets/audio/notifications/Completed.wav
--rw-rw-rw-   0        0        0   159276 2021-05-30 12:26:50.000000 simpleworkspace-1.2.186/src/simpleworkspace/assets/audio/notifications/Error.wav
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.663379 simpleworkspace-1.2.186/src/simpleworkspace/assets/icons/
--rw-rw-rw-   0        0        0      864 2024-01-22 08:25:22.000000 simpleworkspace-1.2.186/src/simpleworkspace/assets/icons/ErrorCircle.png
--rw-rw-rw-   0        0        0      738 2024-01-22 09:30:40.000000 simpleworkspace-1.2.186/src/simpleworkspace/assets/icons/InfoCircle.png
--rw-rw-rw-   0        0        0      913 2024-01-22 08:25:22.000000 simpleworkspace-1.2.186/src/simpleworkspace/assets/icons/QuestionCircle.png
--rw-rw-rw-   0        0        0      643 2024-01-22 08:25:22.000000 simpleworkspace-1.2.186/src/simpleworkspace/assets/icons/WarningCircle.png
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.670084 simpleworkspace-1.2.186/src/simpleworkspace/collections/
--rw-rw-rw-   0        0        0        0 2023-12-06 00:49:54.000000 simpleworkspace-1.2.186/src/simpleworkspace/collections/__init__.py
--rw-rw-rw-   0        0        0      217 2023-12-11 19:38:54.000000 simpleworkspace-1.2.186/src/simpleworkspace/collections/loader.py
--rw-rw-rw-   0        0        0     8357 2024-03-10 18:15:07.000000 simpleworkspace-1.2.186/src/simpleworkspace/collections/observables.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.701462 simpleworkspace-1.2.186/src/simpleworkspace/db/
--rw-rw-rw-   0        0        0        0 2023-09-27 17:03:43.000000 simpleworkspace-1.2.186/src/simpleworkspace/db/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-11-10 09:43:08.000000 simpleworkspace-1.2.186/src/simpleworkspace/db/dbfactory.py
--rw-rw-rw-   0        0        0    26868 2024-01-15 18:01:58.000000 simpleworkspace-1.2.186/src/simpleworkspace/db/fluentsqlbuilder.py
--rw-rw-rw-   0        0        0      356 2023-12-11 19:38:54.000000 simpleworkspace-1.2.186/src/simpleworkspace/db/loader.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.735642 simpleworkspace-1.2.186/src/simpleworkspace/gui/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.186/src/simpleworkspace/gui/__init__.py
--rw-rw-rw-   0        0        0    19745 2024-02-03 10:18:03.000000 simpleworkspace-1.2.186/src/simpleworkspace/gui/dialogs.py
--rw-rw-rw-   0        0        0      199 2024-01-15 19:55:06.000000 simpleworkspace-1.2.186/src/simpleworkspace/gui/loader.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.831684 simpleworkspace-1.2.186/src/simpleworkspace/io/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.186/src/simpleworkspace/io/__init__.py
--rw-rw-rw-   0        0        0     9009 2024-02-25 18:43:27.000000 simpleworkspace-1.2.186/src/simpleworkspace/io/archive.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.844250 simpleworkspace-1.2.186/src/simpleworkspace/io/audio/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.186/src/simpleworkspace/io/audio/__init__.py
--rw-rw-rw-   0        0        0      184 2024-02-24 14:54:39.000000 simpleworkspace-1.2.186/src/simpleworkspace/io/audio/loader.py
--rw-rw-rw-   0        0        0      720 2024-02-24 19:58:16.000000 simpleworkspace-1.2.186/src/simpleworkspace/io/audio/play.py
--rw-rw-rw-   0        0        0     5574 2024-02-28 16:08:09.000000 simpleworkspace-1.2.186/src/simpleworkspace/io/directory.py
--rw-rw-rw-   0        0        0     2962 2024-02-07 20:22:40.000000 simpleworkspace-1.2.186/src/simpleworkspace/io/file.py
--rw-rw-rw-   0        0        0      705 2024-02-23 06:39:35.000000 simpleworkspace-1.2.186/src/simpleworkspace/io/loader.py
--rw-rw-rw-   0        0        0     6058 2024-02-21 21:38:25.000000 simpleworkspace-1.2.186/src/simpleworkspace/io/path.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.862053 simpleworkspace-1.2.186/src/simpleworkspace/io/readers/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.186/src/simpleworkspace/io/readers/__init__.py
--rw-rw-rw-   0        0        0     6265 2024-02-12 21:01:46.000000 simpleworkspace-1.2.186/src/simpleworkspace/io/readers/csvreader.py
--rw-rw-rw-   0        0        0      321 2023-12-11 19:38:54.000000 simpleworkspace-1.2.186/src/simpleworkspace/io/readers/loader.py
--rw-rw-rw-   0        0        0     2637 2024-02-25 08:00:45.000000 simpleworkspace-1.2.186/src/simpleworkspace/io/readers/logreader.py
--rw-rw-rw-   0        0        0     1256 2024-01-19 14:38:39.000000 simpleworkspace-1.2.186/src/simpleworkspace/loader.py
--rw-rw-rw-   0        0        0     6464 2024-01-27 23:46:02.000000 simpleworkspace-1.2.186/src/simpleworkspace/logproviders.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.341105 simpleworkspace-1.2.186/src/simpleworkspace/packages/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.866867 simpleworkspace-1.2.186/src/simpleworkspace/packages/debug/
--rw-rw-rw-   0        0        0     2163 2024-01-31 16:09:17.000000 simpleworkspace-1.2.186/src/simpleworkspace/packages/debug/profiler.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.322420 simpleworkspace-1.2.186/src/simpleworkspace/packages/network/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.871428 simpleworkspace-1.2.186/src/simpleworkspace/packages/network/servers/
--rw-rw-rw-   0        0        0    10843 2024-02-04 13:59:24.000000 simpleworkspace-1.2.186/src/simpleworkspace/packages/network/servers/basicserver.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.875602 simpleworkspace-1.2.186/src/simpleworkspace/packages/pythonbundlers/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.881366 simpleworkspace-1.2.186/src/simpleworkspace/packages/pythonbundlers/dependecy/
--rw-rw-rw-   0        0        0        0 2024-01-27 17:48:10.000000 simpleworkspace-1.2.186/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.905839 simpleworkspace-1.2.186/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
--rw-rw-rw-   0        0        0      717 2024-01-27 17:30:09.000000 simpleworkspace-1.2.186/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
--rw-rw-rw-   0        0        0    38758 2024-01-27 17:30:16.000000 simpleworkspace-1.2.186/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
--rw-rw-rw-   0        0        0     9974 2024-01-27 17:30:31.000000 simpleworkspace-1.2.186/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
--rw-rw-rw-   0        0        0      348 2024-01-27 17:30:45.000000 simpleworkspace-1.2.186/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
--rw-rw-rw-   0        0        0      768 2023-10-11 00:54:10.000000 simpleworkspace-1.2.186/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
--rw-rw-rw-   0        0        0     4889 2024-02-12 20:16:17.000000 simpleworkspace-1.2.186/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.919004 simpleworkspace-1.2.186/src/simpleworkspace/packages/taskscheduler/
--rw-rw-rw-   0        0        0       79 2023-09-27 18:18:53.000000 simpleworkspace-1.2.186/src/simpleworkspace/packages/taskscheduler/__init__.py
--rw-rw-rw-   0        0        0     8953 2024-04-19 16:09:12.000000 simpleworkspace-1.2.186/src/simpleworkspace/packages/taskscheduler/manager.py
--rw-rw-rw-   0        0        0     5066 2024-04-19 16:39:22.000000 simpleworkspace-1.2.186/src/simpleworkspace/packages/taskscheduler/model.py
--rw-rw-rw-   0        0        0     7383 2024-02-12 20:00:46.000000 simpleworkspace-1.2.186/src/simpleworkspace/settingsproviders.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:01.982448 simpleworkspace-1.2.186/src/simpleworkspace/types/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.186/src/simpleworkspace/types/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-02-14 19:40:14.000000 simpleworkspace-1.2.186/src/simpleworkspace/types/byte.py
--rw-rw-rw-   0        0        0     5736 2023-09-27 18:18:54.000000 simpleworkspace-1.2.186/src/simpleworkspace/types/iunit.py
--rw-rw-rw-   0        0        0      471 2023-12-11 19:38:54.000000 simpleworkspace-1.2.186/src/simpleworkspace/types/loader.py
--rw-rw-rw-   0        0        0      932 2023-09-27 18:18:54.000000 simpleworkspace-1.2.186/src/simpleworkspace/types/measurement.py
--rw-rw-rw-   0        0        0      556 2024-03-09 13:42:06.000000 simpleworkspace-1.2.186/src/simpleworkspace/types/os.py
--rw-rw-rw-   0        0        0     8243 2023-09-27 18:18:54.000000 simpleworkspace-1.2.186/src/simpleworkspace/types/time.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:02.043370 simpleworkspace-1.2.186/src/simpleworkspace/utility/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.186/src/simpleworkspace/utility/__init__.py
--rw-rw-rw-   0        0        0      237 2023-09-27 18:18:54.000000 simpleworkspace-1.2.186/src/simpleworkspace/utility/bytes.py
--rw-rw-rw-   0        0        0     1915 2023-12-12 18:58:31.000000 simpleworkspace-1.2.186/src/simpleworkspace/utility/cache.py
--rw-rw-rw-   0        0        0     7735 2024-02-08 17:57:55.000000 simpleworkspace-1.2.186/src/simpleworkspace/utility/console.py
--rw-rw-rw-   0        0        0    14495 2024-02-14 19:32:38.000000 simpleworkspace-1.2.186/src/simpleworkspace/utility/linq.py
--rw-rw-rw-   0        0        0      984 2023-12-11 19:38:54.000000 simpleworkspace-1.2.186/src/simpleworkspace/utility/loader.py
--rw-rw-rw-   0        0        0     4548 2024-02-28 20:36:05.000000 simpleworkspace-1.2.186/src/simpleworkspace/utility/module.py
--rw-rw-rw-   0        0        0     1798 2024-01-23 23:38:57.000000 simpleworkspace-1.2.186/src/simpleworkspace/utility/parallel.py
--rw-rw-rw-   0        0        0    11207 2024-03-18 16:44:18.000000 simpleworkspace-1.2.186/src/simpleworkspace/utility/progressbar.py
--rw-rw-rw-   0        0        0     7218 2024-02-20 06:25:57.000000 simpleworkspace-1.2.186/src/simpleworkspace/utility/regex.py
--rw-rw-rw-   0        0        0     1865 2024-02-07 19:12:33.000000 simpleworkspace-1.2.186/src/simpleworkspace/utility/strings.py
--rw-rw-rw-   0        0        0     6758 2024-03-02 16:36:06.000000 simpleworkspace-1.2.186/src/simpleworkspace/utility/time.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:42:02.049115 simpleworkspace-1.2.186/src/simpleworkspace.egg-info/
--rw-rw-rw-   0        0        0      148 2024-04-19 16:42:00.000000 simpleworkspace-1.2.186/src/simpleworkspace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3310 2024-04-19 16:42:01.000000 simpleworkspace-1.2.186/src/simpleworkspace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 16:42:00.000000 simpleworkspace-1.2.186/src/simpleworkspace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-19 16:42:00.000000 simpleworkspace-1.2.186/src/simpleworkspace.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-19 16:42:00.000000 simpleworkspace-1.2.186/src/simpleworkspace.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:09.010374 simpleworkspace-1.2.187/
+-rw-rw-rw-   0        0        0       22 2024-01-29 16:35:42.000000 simpleworkspace-1.2.187/MANIFEST.in
+-rw-rw-rw-   0        0        0      148 2024-04-21 08:01:09.005004 simpleworkspace-1.2.187/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-04-21 07:58:20.000000 simpleworkspace-1.2.187/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-21 08:01:09.020787 simpleworkspace-1.2.187/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:07.083125 simpleworkspace-1.2.187/src/
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:07.373844 simpleworkspace-1.2.187/src/simpleworkspace/
+-rw-rw-rw-   0        0        0        0 2024-01-22 08:55:41.000000 simpleworkspace-1.2.187/src/simpleworkspace/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-12-11 19:38:16.000000 simpleworkspace-1.2.187/src/simpleworkspace/__lazyimporter__.py
+-rw-rw-rw-   0        0        0     2458 2024-02-05 17:50:15.000000 simpleworkspace-1.2.187/src/simpleworkspace/app.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:07.496998 simpleworkspace-1.2.187/src/simpleworkspace/assets/
+-rw-rw-rw-   0        0        0      561 2024-02-24 14:57:44.000000 simpleworkspace-1.2.187/src/simpleworkspace/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:07.516642 simpleworkspace-1.2.187/src/simpleworkspace/assets/__pycache__/
+-rw-rw-rw-   0        0        0      658 2024-01-24 15:01:20.000000 simpleworkspace-1.2.187/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      876 2024-02-24 15:09:13.000000 simpleworkspace-1.2.187/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:07.098576 simpleworkspace-1.2.187/src/simpleworkspace/assets/audio/
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:07.533041 simpleworkspace-1.2.187/src/simpleworkspace/assets/audio/alarms/
+-rw-rw-rw-   0        0        0   115582 2024-02-24 14:31:08.000000 simpleworkspace-1.2.187/src/simpleworkspace/assets/audio/alarms/Siren.wav
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:07.562720 simpleworkspace-1.2.187/src/simpleworkspace/assets/audio/notifications/
+-rw-rw-rw-   0        0        0   168352 2024-02-24 14:26:13.000000 simpleworkspace-1.2.187/src/simpleworkspace/assets/audio/notifications/Completed.wav
+-rw-rw-rw-   0        0        0   159276 2021-05-30 12:26:50.000000 simpleworkspace-1.2.187/src/simpleworkspace/assets/audio/notifications/Error.wav
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:07.608056 simpleworkspace-1.2.187/src/simpleworkspace/assets/icons/
+-rw-rw-rw-   0        0        0      864 2024-01-22 08:25:22.000000 simpleworkspace-1.2.187/src/simpleworkspace/assets/icons/ErrorCircle.png
+-rw-rw-rw-   0        0        0      738 2024-01-22 09:30:40.000000 simpleworkspace-1.2.187/src/simpleworkspace/assets/icons/InfoCircle.png
+-rw-rw-rw-   0        0        0      913 2024-01-22 08:25:22.000000 simpleworkspace-1.2.187/src/simpleworkspace/assets/icons/QuestionCircle.png
+-rw-rw-rw-   0        0        0      643 2024-01-22 08:25:22.000000 simpleworkspace-1.2.187/src/simpleworkspace/assets/icons/WarningCircle.png
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:07.652645 simpleworkspace-1.2.187/src/simpleworkspace/collections/
+-rw-rw-rw-   0        0        0        0 2023-12-06 00:49:54.000000 simpleworkspace-1.2.187/src/simpleworkspace/collections/__init__.py
+-rw-rw-rw-   0        0        0      217 2023-12-11 19:38:54.000000 simpleworkspace-1.2.187/src/simpleworkspace/collections/loader.py
+-rw-rw-rw-   0        0        0     8357 2024-03-10 18:15:07.000000 simpleworkspace-1.2.187/src/simpleworkspace/collections/observables.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:07.729779 simpleworkspace-1.2.187/src/simpleworkspace/db/
+-rw-rw-rw-   0        0        0        0 2023-09-27 17:03:43.000000 simpleworkspace-1.2.187/src/simpleworkspace/db/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-11-10 09:43:08.000000 simpleworkspace-1.2.187/src/simpleworkspace/db/dbfactory.py
+-rw-rw-rw-   0        0        0    26868 2024-01-15 18:01:58.000000 simpleworkspace-1.2.187/src/simpleworkspace/db/fluentsqlbuilder.py
+-rw-rw-rw-   0        0        0      356 2023-12-11 19:38:54.000000 simpleworkspace-1.2.187/src/simpleworkspace/db/loader.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:07.780404 simpleworkspace-1.2.187/src/simpleworkspace/gui/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.187/src/simpleworkspace/gui/__init__.py
+-rw-rw-rw-   0        0        0    19745 2024-02-03 10:18:03.000000 simpleworkspace-1.2.187/src/simpleworkspace/gui/dialogs.py
+-rw-rw-rw-   0        0        0      199 2024-01-15 19:55:06.000000 simpleworkspace-1.2.187/src/simpleworkspace/gui/loader.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:07.949964 simpleworkspace-1.2.187/src/simpleworkspace/io/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.187/src/simpleworkspace/io/__init__.py
+-rw-rw-rw-   0        0        0     9009 2024-02-25 18:43:27.000000 simpleworkspace-1.2.187/src/simpleworkspace/io/archive.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:08.051362 simpleworkspace-1.2.187/src/simpleworkspace/io/audio/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.187/src/simpleworkspace/io/audio/__init__.py
+-rw-rw-rw-   0        0        0      184 2024-02-24 14:54:39.000000 simpleworkspace-1.2.187/src/simpleworkspace/io/audio/loader.py
+-rw-rw-rw-   0        0        0      720 2024-02-24 19:58:16.000000 simpleworkspace-1.2.187/src/simpleworkspace/io/audio/play.py
+-rw-rw-rw-   0        0        0     5574 2024-02-28 16:08:09.000000 simpleworkspace-1.2.187/src/simpleworkspace/io/directory.py
+-rw-rw-rw-   0        0        0     2962 2024-02-07 20:22:40.000000 simpleworkspace-1.2.187/src/simpleworkspace/io/file.py
+-rw-rw-rw-   0        0        0      705 2024-02-23 06:39:35.000000 simpleworkspace-1.2.187/src/simpleworkspace/io/loader.py
+-rw-rw-rw-   0        0        0     6058 2024-02-21 21:38:25.000000 simpleworkspace-1.2.187/src/simpleworkspace/io/path.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:08.168787 simpleworkspace-1.2.187/src/simpleworkspace/io/readers/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.187/src/simpleworkspace/io/readers/__init__.py
+-rw-rw-rw-   0        0        0     6265 2024-02-12 21:01:46.000000 simpleworkspace-1.2.187/src/simpleworkspace/io/readers/csvreader.py
+-rw-rw-rw-   0        0        0      321 2023-12-11 19:38:54.000000 simpleworkspace-1.2.187/src/simpleworkspace/io/readers/loader.py
+-rw-rw-rw-   0        0        0     2637 2024-02-25 08:00:45.000000 simpleworkspace-1.2.187/src/simpleworkspace/io/readers/logreader.py
+-rw-rw-rw-   0        0        0     1256 2024-01-19 14:38:39.000000 simpleworkspace-1.2.187/src/simpleworkspace/loader.py
+-rw-rw-rw-   0        0        0     6464 2024-01-27 23:46:02.000000 simpleworkspace-1.2.187/src/simpleworkspace/logproviders.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:07.201563 simpleworkspace-1.2.187/src/simpleworkspace/packages/
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:08.201124 simpleworkspace-1.2.187/src/simpleworkspace/packages/debug/
+-rw-rw-rw-   0        0        0     2163 2024-01-31 16:09:17.000000 simpleworkspace-1.2.187/src/simpleworkspace/packages/debug/profiler.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:07.178046 simpleworkspace-1.2.187/src/simpleworkspace/packages/network/
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:07.182519 simpleworkspace-1.2.187/src/simpleworkspace/packages/network/servers/
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:08.223284 simpleworkspace-1.2.187/src/simpleworkspace/packages/network/servers/basicserver/
+-rw-rw-rw-   0        0        0       71 2024-04-21 07:34:26.000000 simpleworkspace-1.2.187/src/simpleworkspace/packages/network/servers/basicserver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:08.223284 simpleworkspace-1.2.187/src/simpleworkspace/packages/network/servers/basicserver/model/
+-rw-rw-rw-   0        0        0     3179 2024-04-21 07:55:10.000000 simpleworkspace-1.2.187/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py
+-rw-rw-rw-   0        0        0     9107 2024-04-21 07:55:55.000000 simpleworkspace-1.2.187/src/simpleworkspace/packages/network/servers/basicserver/server.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:08.256976 simpleworkspace-1.2.187/src/simpleworkspace/packages/pythonbundlers/
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:08.256976 simpleworkspace-1.2.187/src/simpleworkspace/packages/pythonbundlers/dependecy/
+-rw-rw-rw-   0        0        0        0 2024-01-27 17:48:10.000000 simpleworkspace-1.2.187/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:08.387976 simpleworkspace-1.2.187/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
+-rw-rw-rw-   0        0        0      717 2024-01-27 17:30:09.000000 simpleworkspace-1.2.187/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
+-rw-rw-rw-   0        0        0    38758 2024-01-27 17:30:16.000000 simpleworkspace-1.2.187/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
+-rw-rw-rw-   0        0        0     9974 2024-01-27 17:30:31.000000 simpleworkspace-1.2.187/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
+-rw-rw-rw-   0        0        0      348 2024-01-27 17:30:45.000000 simpleworkspace-1.2.187/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
+-rw-rw-rw-   0        0        0      768 2023-10-11 00:54:10.000000 simpleworkspace-1.2.187/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
+-rw-rw-rw-   0        0        0     4889 2024-02-12 20:16:17.000000 simpleworkspace-1.2.187/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:08.462957 simpleworkspace-1.2.187/src/simpleworkspace/packages/taskscheduler/
+-rw-rw-rw-   0        0        0       79 2023-09-27 18:18:53.000000 simpleworkspace-1.2.187/src/simpleworkspace/packages/taskscheduler/__init__.py
+-rw-rw-rw-   0        0        0     8953 2024-04-19 16:09:12.000000 simpleworkspace-1.2.187/src/simpleworkspace/packages/taskscheduler/manager.py
+-rw-rw-rw-   0        0        0     5066 2024-04-19 16:39:22.000000 simpleworkspace-1.2.187/src/simpleworkspace/packages/taskscheduler/model.py
+-rw-rw-rw-   0        0        0     7383 2024-02-12 20:00:46.000000 simpleworkspace-1.2.187/src/simpleworkspace/settingsproviders.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:08.652423 simpleworkspace-1.2.187/src/simpleworkspace/types/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.187/src/simpleworkspace/types/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-02-14 19:40:14.000000 simpleworkspace-1.2.187/src/simpleworkspace/types/byte.py
+-rw-rw-rw-   0        0        0     5736 2023-09-27 18:18:54.000000 simpleworkspace-1.2.187/src/simpleworkspace/types/iunit.py
+-rw-rw-rw-   0        0        0      471 2023-12-11 19:38:54.000000 simpleworkspace-1.2.187/src/simpleworkspace/types/loader.py
+-rw-rw-rw-   0        0        0      932 2023-09-27 18:18:54.000000 simpleworkspace-1.2.187/src/simpleworkspace/types/measurement.py
+-rw-rw-rw-   0        0        0      556 2024-03-09 13:42:06.000000 simpleworkspace-1.2.187/src/simpleworkspace/types/os.py
+-rw-rw-rw-   0        0        0     8243 2023-09-27 18:18:54.000000 simpleworkspace-1.2.187/src/simpleworkspace/types/time.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:08.996385 simpleworkspace-1.2.187/src/simpleworkspace/utility/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.187/src/simpleworkspace/utility/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-09-27 18:18:54.000000 simpleworkspace-1.2.187/src/simpleworkspace/utility/bytes.py
+-rw-rw-rw-   0        0        0     1915 2023-12-12 18:58:31.000000 simpleworkspace-1.2.187/src/simpleworkspace/utility/cache.py
+-rw-rw-rw-   0        0        0     7735 2024-02-08 17:57:55.000000 simpleworkspace-1.2.187/src/simpleworkspace/utility/console.py
+-rw-rw-rw-   0        0        0    14495 2024-02-14 19:32:38.000000 simpleworkspace-1.2.187/src/simpleworkspace/utility/linq.py
+-rw-rw-rw-   0        0        0      984 2023-12-11 19:38:54.000000 simpleworkspace-1.2.187/src/simpleworkspace/utility/loader.py
+-rw-rw-rw-   0        0        0     4548 2024-02-28 20:36:05.000000 simpleworkspace-1.2.187/src/simpleworkspace/utility/module.py
+-rw-rw-rw-   0        0        0     1798 2024-01-23 23:38:57.000000 simpleworkspace-1.2.187/src/simpleworkspace/utility/parallel.py
+-rw-rw-rw-   0        0        0    11207 2024-03-18 16:44:18.000000 simpleworkspace-1.2.187/src/simpleworkspace/utility/progressbar.py
+-rw-rw-rw-   0        0        0     7218 2024-02-20 06:25:57.000000 simpleworkspace-1.2.187/src/simpleworkspace/utility/regex.py
+-rw-rw-rw-   0        0        0     1865 2024-02-07 19:12:33.000000 simpleworkspace-1.2.187/src/simpleworkspace/utility/strings.py
+-rw-rw-rw-   0        0        0     6758 2024-03-02 16:36:06.000000 simpleworkspace-1.2.187/src/simpleworkspace/utility/time.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:01:09.005004 simpleworkspace-1.2.187/src/simpleworkspace.egg-info/
+-rw-rw-rw-   0        0        0      148 2024-04-21 08:01:06.000000 simpleworkspace-1.2.187/src/simpleworkspace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3464 2024-04-21 08:01:07.000000 simpleworkspace-1.2.187/src/simpleworkspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 08:01:06.000000 simpleworkspace-1.2.187/src/simpleworkspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-21 08:01:06.000000 simpleworkspace-1.2.187/src/simpleworkspace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-21 08:01:06.000000 simpleworkspace-1.2.187/src/simpleworkspace.egg-info/top_level.txt
```

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/app.py` & `simpleworkspace-1.2.187/src/simpleworkspace/app.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/assets/__init__.py` & `simpleworkspace-1.2.187/src/simpleworkspace/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc` & `simpleworkspace-1.2.187/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc` & `simpleworkspace-1.2.187/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/assets/audio/alarms/Siren.wav` & `simpleworkspace-1.2.187/src/simpleworkspace/assets/audio/alarms/Siren.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/assets/audio/notifications/Completed.wav` & `simpleworkspace-1.2.187/src/simpleworkspace/assets/audio/notifications/Completed.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/assets/audio/notifications/Error.wav` & `simpleworkspace-1.2.187/src/simpleworkspace/assets/audio/notifications/Error.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/assets/icons/ErrorCircle.png` & `simpleworkspace-1.2.187/src/simpleworkspace/assets/icons/ErrorCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/assets/icons/InfoCircle.png` & `simpleworkspace-1.2.187/src/simpleworkspace/assets/icons/InfoCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/assets/icons/QuestionCircle.png` & `simpleworkspace-1.2.187/src/simpleworkspace/assets/icons/QuestionCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/assets/icons/WarningCircle.png` & `simpleworkspace-1.2.187/src/simpleworkspace/assets/icons/WarningCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/collections/observables.py` & `simpleworkspace-1.2.187/src/simpleworkspace/collections/observables.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/db/dbfactory.py` & `simpleworkspace-1.2.187/src/simpleworkspace/db/dbfactory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/db/fluentsqlbuilder.py` & `simpleworkspace-1.2.187/src/simpleworkspace/db/fluentsqlbuilder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/gui/dialogs.py` & `simpleworkspace-1.2.187/src/simpleworkspace/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/io/archive.py` & `simpleworkspace-1.2.187/src/simpleworkspace/io/archive.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/io/audio/play.py` & `simpleworkspace-1.2.187/src/simpleworkspace/io/audio/play.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/io/directory.py` & `simpleworkspace-1.2.187/src/simpleworkspace/io/directory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/io/file.py` & `simpleworkspace-1.2.187/src/simpleworkspace/io/file.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/io/loader.py` & `simpleworkspace-1.2.187/src/simpleworkspace/io/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/io/path.py` & `simpleworkspace-1.2.187/src/simpleworkspace/io/path.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/io/readers/csvreader.py` & `simpleworkspace-1.2.187/src/simpleworkspace/io/readers/csvreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/io/readers/logreader.py` & `simpleworkspace-1.2.187/src/simpleworkspace/io/readers/logreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/loader.py` & `simpleworkspace-1.2.187/src/simpleworkspace/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/logproviders.py` & `simpleworkspace-1.2.187/src/simpleworkspace/logproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/packages/debug/profiler.py` & `simpleworkspace-1.2.187/src/simpleworkspace/packages/debug/profiler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/packages/network/servers/basicserver.py` & `simpleworkspace-1.2.187/src/simpleworkspace/packages/network/servers/basicserver/server.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,121 +1,79 @@
 from base64 import b64encode
 from http import HTTPStatus
-from http.client import HTTPMessage
 from logging import Logger
 import http.server
 import socketserver
 from socketserver import BaseRequestHandler
 from urllib.parse import urlparse, parse_qs
 from simpleworkspace.logproviders import DummyLogger
 import ssl
 import subprocess
-from functools import cached_property
-from io import BytesIO
-
-class _RequestDetails:
-    Headers: HTTPMessage
-    '''Dict like object containing the headers of the incoming request'''
-    Method: str
-    ''' The method used in the request, such as "GET", "POST"... '''
-    Path: str = ''
-    ''' The path part of url, example: "https://example.com/pages/index.html?key1=val1" -> "/pages/index.html" '''
-    Query_GET: dict[str,str] = {}
-    ''' Query params in url, example: "https://example.com/pages/index.html?key1=val1" -> {'key1': 'val1'} '''
-    Query_POST: dict[str,str] = {}
-    ''' Query params in request body '''
-    Body: bytes = None
-    ''' The raw request body '''
-
-    @cached_property
-    def Query_ANY(self):
-        ''' 
-        A combined dictionary consisting of both POST and GET parameters.
-        If a param exists in both POST and GET query, then GET will be preffered
-        '''
-        return {**self.Query_POST, **self.Query_GET}
-
-class _ResponseDetails:
-    Headers: dict[str, str] = {'Content-Type': 'text/html'}
-    ''' Specify headers that will be sent to client. Note: server might additionally add some extra standard headers by default '''
-    StatusCode = HTTPStatus.OK
-    ''' Specifies the status code client will recieve '''
-    Data: BytesIO|bytes|str = BytesIO()
-    ''' The data client will recieve. By default is an BytesIO which can efficently be written to, otherwise you can also directly set Data to be a str or bytes like object '''
-
-    def _GetDataBytes(self):
-        dataType = type(self.Data)
-        if(dataType is str):
-            return self.Data.encode('utf-8')
-        elif(dataType is bytes):
-            return self.Data
-        elif(dataType is BytesIO):
-            return self.Data.getvalue()
-        else:
-            raise TypeError(f'Invalid type supplied in ResponseDetails.Data... Got: {dataType}')
+from http import HTTPStatus
+from .model.commobjects import \
+    CommuncationContainer as _CommuncationContainer, \
+    RequestContainer as _RequestContainer, \
+    ResponseContainer as _ResponseContainer
 
 class BasicRequestHandler(http.server.SimpleHTTPRequestHandler):
     """
     Class should always be derived and supplied into BasicServer
 
     Properties for implementer:
-    - RequestDetails    , contains all necessary request info in one place
-    - ResponseDetails   , set the properties here to alter the final response to the client
+    - COMM.Request    , contains all necessary request info in one place
+    - COMM.Response   , set the properties here to alter the final response to the client
     
     Methods for implementer that may be overridden:
     - BeforeRequest()   , Runs before OnRequest can be overriden to perform routines before processing the request
     - OnRequest()       , this is the main entry point to start processing the request and preparing the response, implementer can override this to suite api needs.
     - GetPage_Index()   , placeholder/boilerplate function runs on entry path '/' with empty query      (if OnRequest is not overriden)
     - OnRequest_Action(), placeholder/boilerplate function that triggers when action param is specified (if OnRequest is not overriden)
     """
 
     server:'BasicServer' = None # just to update intellisense
-    RequestDetails: _RequestDetails
-    ResponseDetails: _ResponseDetails
+    COMM: _CommuncationContainer
 
     class Signals:
         class StopRequest(Exception):
             '''
             Can be used to stop processing of a request in a graceful way by calling
             >>> raise self.Signals.StopRequest()
             '''
 
-
-
     #region Routines
     def _Routine_Authentication_Basic(self):
         if self.server.Config.Authentication._BasicKey is None:
             return # no auth configured
 
-        if(self.RequestDetails.Headers.get('Authorization') == self.server.Config.Authentication._BasicKey):
+        if(self.COMM.Request.Headers.get('Authorization') == self.server.Config.Authentication._BasicKey):
             return
 
-        self.ResponseDetails.Headers['WWW-Authenticate'] = 'Basic realm="Login Required"'
-        self.ResponseDetails.Data = 'Authorization required.'
-        self.ResponseDetails.StatusCode = HTTPStatus.UNAUTHORIZED
+        self.COMM.Response.Headers['WWW-Authenticate'] = 'Basic realm="Login Required"'
+        self.COMM.Response.Data = 'Authorization required.'
+        self.COMM.Response.StatusCode = HTTPStatus.UNAUTHORIZED
         raise self.Signals.StopRequest()
     
     #endregion Routines
 
     def _Default_BeforeRequest(self):
         '''Default Hook before OnRequest has been processed'''
         # when basic auth is enabled, checks if current client is authorized
         self._Routine_Authentication_Basic()
 
     def OnRequest(self):
         '''This can be overriden freely, below is simply implementing boilerplate code'''
-        if(self.RequestDetails.Method == 'GET') and (self.RequestDetails.Path == '/') and len(self.RequestDetails.Query_ANY) == 0:
+        if(self.COMM.Request.Method == 'GET') and (self.COMM.Request.URL.path == '/') and len(self.COMM.Request.Query.ANY) == 0:
             self.GetPage_Index()
-        elif('action' in self.RequestDetails.Query_ANY):
-            data = self.RequestDetails.Query_ANY.get('data', None)
-            self.OnRequest_Action(self.RequestDetails.Query_ANY['action'], data)
+        elif('action' in self.COMM.Request.Query.ANY):
+            data = self.COMM.Request.Query.ANY.get('data', None)
+            self.OnRequest_Action(self.COMM.Request.Query.ANY['action'], data)
         
     def GetPage_Index(self):
         '''boilerplate method'''
-        #self.ResponseDetails.Data = sw.io.file.Read('./index.html')
+        #self.COMM.Request.Data = sw.io.file.Read('./index.html')
 
     def OnRequest_Action(self, action: str, data: str=None):
         '''boilerplate method'''
 
 
     #region Overrides
     # override, original writes to standard outputs, which fails if app is pyw
@@ -140,45 +98,46 @@
                 return
             if not self.raw_requestline:
                 self.close_connection = True
                 return
             if not self.parse_request():
                 return # An error code has been sent, just exit
             
-            parsedUrl = urlparse(self.path)
-            self.RequestDetails = _RequestDetails()
-            self.RequestDetails.Headers = self.headers
-            self.RequestDetails.Method = self.command
-            self.RequestDetails.Path = parsedUrl.path
+            
+            self.COMM = _CommuncationContainer()
+            self.COMM.Request = _RequestContainer()
+            self.COMM.Request.Headers = self.headers
+            self.COMM.Request.Method = self.command
+            self.COMM.Request.URL = urlparse(self.path)
 
-            def ParseUrlEncodedQuery(query:str):
+            def ParseUrlEncodedQuery(query:str) -> dict[str,str]:
                 parsedQuery = parse_qs(query)
                 #only keep the first matching query key, discard duplicates for simplicity
                 for key in parsedQuery.keys():
                     parsedQuery[key] = parsedQuery[key][0]
                 return parsedQuery
             
-            self.RequestDetails.Query_GET = ParseUrlEncodedQuery(parsedUrl.query)
+            self.COMM.Request.Query.GET = ParseUrlEncodedQuery(self.COMM.Request.URL.query)
             if('Content-Length' in self.headers):
-                self.RequestDetails.Body = self.rfile.read(int(self.headers['Content-Length']))
+                self.COMM.Request.Body = self.rfile.read(int(self.headers['Content-Length']))
                 if(self.headers.get('Content-Type') == 'application/x-www-form-urlencoded'):
-                    self.RequestDetails.Query_POST = ParseUrlEncodedQuery(self.RequestDetails.Body.decode('utf-8'))
+                    self.COMM.Request.Query.POST = ParseUrlEncodedQuery(self.COMM.Request.Body.decode('utf-8'))
             
-            self.ResponseDetails = _ResponseDetails()
+            self.COMM.Response = _ResponseContainer()
             try:
                 self._Default_BeforeRequest()
                 self.OnRequest()
             except self.Signals.StopRequest:
                 pass  # a graceful request cancellation
             finally:
-                self.send_response(self.ResponseDetails.StatusCode)
-                for key, value in self.ResponseDetails.Headers.items():
+                self.send_response(self.COMM.Response.StatusCode)
+                for key, value in self.COMM.Response.Headers.items():
                     self.send_header(key, value)
                 self.end_headers()
-                self.wfile.write(self.ResponseDetails._GetDataBytes())
+                self.wfile.write(self.COMM.Response._GetDataBytes())
         except TimeoutError as e:
             # a read or a write timed out.  Discard this connection
             self.server.logger.exception("Request timed out")
             self.close_connection = True
             return
     #endregion Overrides
```

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py` & `simpleworkspace-1.2.187/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py` & `simpleworkspace-1.2.187/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py` & `simpleworkspace-1.2.187/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py` & `simpleworkspace-1.2.187/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py` & `simpleworkspace-1.2.187/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/packages/taskscheduler/manager.py` & `simpleworkspace-1.2.187/src/simpleworkspace/packages/taskscheduler/manager.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/packages/taskscheduler/model.py` & `simpleworkspace-1.2.187/src/simpleworkspace/packages/taskscheduler/model.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/settingsproviders.py` & `simpleworkspace-1.2.187/src/simpleworkspace/settingsproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/types/byte.py` & `simpleworkspace-1.2.187/src/simpleworkspace/types/byte.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/types/iunit.py` & `simpleworkspace-1.2.187/src/simpleworkspace/types/iunit.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/types/measurement.py` & `simpleworkspace-1.2.187/src/simpleworkspace/types/measurement.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/types/os.py` & `simpleworkspace-1.2.187/src/simpleworkspace/types/os.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/types/time.py` & `simpleworkspace-1.2.187/src/simpleworkspace/types/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/utility/cache.py` & `simpleworkspace-1.2.187/src/simpleworkspace/utility/cache.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/utility/console.py` & `simpleworkspace-1.2.187/src/simpleworkspace/utility/console.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/utility/linq.py` & `simpleworkspace-1.2.187/src/simpleworkspace/utility/linq.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/utility/loader.py` & `simpleworkspace-1.2.187/src/simpleworkspace/utility/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/utility/module.py` & `simpleworkspace-1.2.187/src/simpleworkspace/utility/module.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/utility/parallel.py` & `simpleworkspace-1.2.187/src/simpleworkspace/utility/parallel.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/utility/progressbar.py` & `simpleworkspace-1.2.187/src/simpleworkspace/utility/progressbar.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/utility/regex.py` & `simpleworkspace-1.2.187/src/simpleworkspace/utility/regex.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/utility/strings.py` & `simpleworkspace-1.2.187/src/simpleworkspace/utility/strings.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace/utility/time.py` & `simpleworkspace-1.2.187/src/simpleworkspace/utility/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.186/src/simpleworkspace.egg-info/SOURCES.txt` & `simpleworkspace-1.2.187/src/simpleworkspace.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,17 @@
 src/simpleworkspace/io/audio/loader.py
 src/simpleworkspace/io/audio/play.py
 src/simpleworkspace/io/readers/__init__.py
 src/simpleworkspace/io/readers/csvreader.py
 src/simpleworkspace/io/readers/loader.py
 src/simpleworkspace/io/readers/logreader.py
 src/simpleworkspace/packages/debug/profiler.py
-src/simpleworkspace/packages/network/servers/basicserver.py
+src/simpleworkspace/packages/network/servers/basicserver/__init__.py
+src/simpleworkspace/packages/network/servers/basicserver/server.py
+src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py
 src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
 src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
 src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
 src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
 src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
 src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
 src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
```


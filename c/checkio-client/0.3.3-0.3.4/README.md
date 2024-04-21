# Comparing `tmp/checkio_client-0.3.3.tar.gz` & `tmp/checkio_client-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkio_client-0.3.3.tar", last modified: Tue Jun 20 20:13:49 2023, max compression
+gzip compressed data, was "checkio_client-0.3.4.tar", last modified: Sun Apr 21 17:35:44 2024, max compression
```

## Comparing `checkio_client-0.3.3.tar` & `checkio_client-0.3.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2023-06-20 20:13:49.900580 checkio_client-0.3.3/
--rw-r--r--   0 oduvan     (501) staff       (20)    18002 2018-05-14 13:33:13.000000 checkio_client-0.3.3/LICENSE
--rw-r--r--   0 oduvan     (501) staff       (20)      411 2023-06-20 20:13:49.900259 checkio_client-0.3.3/PKG-INFO
--rw-r--r--   0 oduvan     (501) staff       (20)     3914 2021-02-09 10:25:48.000000 checkio_client-0.3.3/README.md
-drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2023-06-20 20:13:49.873701 checkio_client-0.3.3/checkio_client/
--rw-r--r--   0 oduvan     (501) staff       (20)        0 2018-07-12 13:37:25.000000 checkio_client-0.3.3/checkio_client/__init__.py
-drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2023-06-20 20:13:49.885446 checkio_client-0.3.3/checkio_client/actions/
--rw-r--r--   0 oduvan     (501) staff       (20)        0 2018-05-14 14:17:48.000000 checkio_client-0.3.3/checkio_client/actions/__init__.py
--rw-r--r--   0 oduvan     (501) staff       (20)      648 2018-07-12 13:48:51.000000 checkio_client-0.3.3/checkio_client/actions/available.py
--rw-r--r--   0 oduvan     (501) staff       (20)    11752 2023-02-20 21:30:35.000000 checkio_client-0.3.3/checkio_client/actions/check.py
--rw-r--r--   0 oduvan     (501) staff       (20)     3692 2020-05-03 22:30:08.000000 checkio_client-0.3.3/checkio_client/actions/config.py
--rw-r--r--   0 oduvan     (501) staff       (20)     3933 2023-03-07 17:26:58.000000 checkio_client-0.3.3/checkio_client/actions/eoc.py
--rw-r--r--   0 oduvan     (501) staff       (20)      838 2022-07-03 12:03:13.000000 checkio_client-0.3.3/checkio_client/actions/init.py
--rw-r--r--   0 oduvan     (501) staff       (20)      873 2021-02-09 10:14:22.000000 checkio_client-0.3.3/checkio_client/actions/open.py
--rw-r--r--   0 oduvan     (501) staff       (20)     7794 2019-06-30 11:36:29.000000 checkio_client-0.3.3/checkio_client/actions/plugin.py
--rw-r--r--   0 oduvan     (501) staff       (20)     2036 2023-03-07 17:26:58.000000 checkio_client-0.3.3/checkio_client/actions/repo.py
--rw-r--r--   0 oduvan     (501) staff       (20)     8433 2023-06-20 20:13:33.000000 checkio_client-0.3.3/checkio_client/actions/repo_check.py
--rw-r--r--   0 oduvan     (501) staff       (20)     5007 2019-06-21 11:42:57.000000 checkio_client-0.3.3/checkio_client/actions/repo_convert.py
--rw-r--r--   0 oduvan     (501) staff       (20)     1563 2022-07-26 18:23:18.000000 checkio_client-0.3.3/checkio_client/actions/server.py
--rw-r--r--   0 oduvan     (501) staff       (20)     7289 2023-06-20 20:13:33.000000 checkio_client-0.3.3/checkio_client/actions/sync.py
--rw-r--r--   0 oduvan     (501) staff       (20)     4818 2020-12-30 11:27:28.000000 checkio_client-0.3.3/checkio_client/api.py
-drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2023-06-20 20:13:49.889260 checkio_client-0.3.3/checkio_client/eoc/
--rw-r--r--   0 oduvan     (501) staff       (20)        0 2019-05-31 12:50:32.000000 checkio_client-0.3.3/checkio_client/eoc/__init__.py
--rw-r--r--   0 oduvan     (501) staff       (20)     3778 2019-06-01 11:46:59.000000 checkio_client-0.3.3/checkio_client/eoc/folder.py
--rw-r--r--   0 oduvan     (501) staff       (20)     4927 2019-11-18 15:20:38.000000 checkio_client-0.3.3/checkio_client/eoc/getters.py
--rw-r--r--   0 oduvan     (501) staff       (20)      992 2019-06-06 07:49:17.000000 checkio_client-0.3.3/checkio_client/eoc/initial.py
--rw-r--r--   0 oduvan     (501) staff       (20)      852 2019-05-31 12:50:32.000000 checkio_client-0.3.3/checkio_client/eoc/settings.py
--rw-r--r--   0 oduvan     (501) staff       (20)     7576 2019-11-16 15:36:16.000000 checkio_client-0.3.3/checkio_client/eoc/testing.py
--rw-r--r--   0 oduvan     (501) staff       (20)     4236 2019-11-18 15:23:59.000000 checkio_client-0.3.3/checkio_client/eoc_runner.py
--rw-r--r--   0 oduvan     (501) staff       (20)     9650 2023-03-07 17:26:58.000000 checkio_client-0.3.3/checkio_client/runner.py
--rw-r--r--   0 oduvan     (501) staff       (20)     5632 2023-06-20 20:13:33.000000 checkio_client-0.3.3/checkio_client/settings.py
-drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2023-06-20 20:13:49.890233 checkio_client-0.3.3/checkio_client/utils/
--rw-r--r--   0 oduvan     (501) staff       (20)        0 2018-07-04 11:20:22.000000 checkio_client-0.3.3/checkio_client/utils/__init__.py
--rw-r--r--   0 oduvan     (501) staff       (20)     4819 2022-07-06 17:14:47.000000 checkio_client-0.3.3/checkio_client/utils/code.py
-drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2023-06-20 20:13:49.892112 checkio_client-0.3.3/checkio_client/verification/
--rw-r--r--   0 oduvan     (501) staff       (20)        0 2018-07-06 10:10:36.000000 checkio_client-0.3.3/checkio_client/verification/__init__.py
-drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2023-06-20 20:13:49.895563 checkio_client-0.3.3/checkio_client/verification/checkio/
--rw-r--r--   0 oduvan     (501) staff       (20)        0 2017-02-10 12:27:49.000000 checkio_client-0.3.3/checkio_client/verification/checkio/__init__.py
--rw-r--r--   0 oduvan     (501) staff       (20)     3305 2021-11-04 10:20:03.000000 checkio_client-0.3.3/checkio_client/verification/checkio/api.py
--rw-r--r--   0 oduvan     (501) staff       (20)     4637 2022-02-19 17:39:13.000000 checkio_client-0.3.3/checkio_client/verification/checkio/code_template.py
-drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2023-06-20 20:13:49.899799 checkio_client-0.3.3/checkio_client/verification/checkio/referees/
--rw-r--r--   0 oduvan     (501) staff       (20)        0 2017-02-10 12:27:49.000000 checkio_client-0.3.3/checkio_client/verification/checkio/referees/__init__.py
--rw-r--r--   0 oduvan     (501) staff       (20)      620 2022-08-10 15:15:11.000000 checkio_client-0.3.3/checkio_client/verification/checkio/referees/checkers.py
--rw-r--r--   0 oduvan     (501) staff       (20)     2441 2021-11-01 00:20:52.000000 checkio_client-0.3.3/checkio_client/verification/checkio/referees/code.py
--rw-r--r--   0 oduvan     (501) staff       (20)      255 2017-02-10 12:27:49.000000 checkio_client-0.3.3/checkio_client/verification/checkio/referees/cover_codes.py
--rw-r--r--   0 oduvan     (501) staff       (20)      282 2017-02-10 12:27:49.000000 checkio_client-0.3.3/checkio_client/verification/checkio/referees/inspectors.py
--rw-r--r--   0 oduvan     (501) staff       (20)     5627 2021-11-14 22:28:37.000000 checkio_client-0.3.3/checkio_client/verification/checkio/referees/io.py
--rw-r--r--   0 oduvan     (501) staff       (20)     2436 2021-12-15 10:22:29.000000 checkio_client-0.3.3/checkio_client/verification/checkio/referees/io_template.py
--rw-r--r--   0 oduvan     (501) staff       (20)     4579 2017-02-10 12:27:49.000000 checkio_client-0.3.3/checkio_client/verification/checkio/referees/multicall.py
--rw-r--r--   0 oduvan     (501) staff       (20)       78 2017-02-10 12:27:49.000000 checkio_client-0.3.3/checkio_client/verification/checkio/runner_types.py
--rw-r--r--   0 oduvan     (501) staff       (20)      141 2017-02-10 12:27:49.000000 checkio_client-0.3.3/checkio_client/verification/checkio/signals.py
--rw-r--r--   0 oduvan     (501) staff       (20)      487 2017-02-10 12:27:49.000000 checkio_client-0.3.3/checkio_client/verification/checkio/utils.py
--rw-r--r--   0 oduvan     (501) staff       (20)     1619 2023-06-20 20:13:33.000000 checkio_client-0.3.3/checkio_client/verification/echo.py
--rw-r--r--   0 oduvan     (501) staff       (20)      828 2021-07-13 14:00:30.000000 checkio_client-0.3.3/checkio_client/verification/uch.py
--rwxr-xr-x   0 oduvan     (501) staff       (20)     7386 2021-10-11 17:42:31.000000 checkio_client-0.3.3/checkio_client/web_plugin.py
-drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2023-06-20 20:13:49.876642 checkio_client-0.3.3/checkio_client.egg-info/
--rw-r--r--   0 oduvan     (501) staff       (20)      411 2023-06-20 20:13:49.000000 checkio_client-0.3.3/checkio_client.egg-info/PKG-INFO
--rw-r--r--   0 oduvan     (501) staff       (20)     1944 2023-06-20 20:13:49.000000 checkio_client-0.3.3/checkio_client.egg-info/SOURCES.txt
--rw-r--r--   0 oduvan     (501) staff       (20)        1 2023-06-20 20:13:49.000000 checkio_client-0.3.3/checkio_client.egg-info/dependency_links.txt
--rw-r--r--   0 oduvan     (501) staff       (20)       55 2023-06-20 20:13:49.000000 checkio_client-0.3.3/checkio_client.egg-info/entry_points.txt
--rw-r--r--   0 oduvan     (501) staff       (20)      149 2023-06-20 20:13:49.000000 checkio_client-0.3.3/checkio_client.egg-info/requires.txt
--rw-r--r--   0 oduvan     (501) staff       (20)       15 2023-06-20 20:13:49.000000 checkio_client-0.3.3/checkio_client.egg-info/top_level.txt
--rw-r--r--   0 oduvan     (501) staff       (20)       38 2023-06-20 20:13:49.900655 checkio_client-0.3.3/setup.cfg
--rw-r--r--   0 oduvan     (501) staff       (20)      842 2023-06-20 20:13:33.000000 checkio_client-0.3.3/setup.py
+drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2024-04-21 17:35:44.452315 checkio_client-0.3.4/
+-rw-r--r--   0 oduvan     (501) staff       (20)    18002 2018-05-14 13:33:13.000000 checkio_client-0.3.4/LICENSE
+-rw-r--r--   0 oduvan     (501) staff       (20)      456 2024-04-21 17:35:44.450759 checkio_client-0.3.4/PKG-INFO
+-rw-r--r--   0 oduvan     (501) staff       (20)     3914 2021-02-09 10:25:48.000000 checkio_client-0.3.4/README.md
+drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2024-04-21 17:35:44.417642 checkio_client-0.3.4/checkio_client/
+-rw-r--r--   0 oduvan     (501) staff       (20)        0 2018-07-12 13:37:25.000000 checkio_client-0.3.4/checkio_client/__init__.py
+drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2024-04-21 17:35:44.431394 checkio_client-0.3.4/checkio_client/actions/
+-rw-r--r--   0 oduvan     (501) staff       (20)        0 2018-05-14 14:17:48.000000 checkio_client-0.3.4/checkio_client/actions/__init__.py
+-rw-r--r--   0 oduvan     (501) staff       (20)      648 2018-07-12 13:48:51.000000 checkio_client-0.3.4/checkio_client/actions/available.py
+-rw-r--r--   0 oduvan     (501) staff       (20)    11752 2023-02-20 21:30:35.000000 checkio_client-0.3.4/checkio_client/actions/check.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     3692 2020-05-03 22:30:08.000000 checkio_client-0.3.4/checkio_client/actions/config.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     3933 2023-03-07 17:26:58.000000 checkio_client-0.3.4/checkio_client/actions/eoc.py
+-rw-r--r--   0 oduvan     (501) staff       (20)      838 2022-07-03 12:03:13.000000 checkio_client-0.3.4/checkio_client/actions/init.py
+-rw-r--r--   0 oduvan     (501) staff       (20)      873 2021-02-09 10:14:22.000000 checkio_client-0.3.4/checkio_client/actions/open.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     7794 2019-06-30 11:36:29.000000 checkio_client-0.3.4/checkio_client/actions/plugin.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     2036 2023-03-07 17:26:58.000000 checkio_client-0.3.4/checkio_client/actions/repo.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     8433 2023-06-20 20:13:33.000000 checkio_client-0.3.4/checkio_client/actions/repo_check.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     5007 2019-06-21 11:42:57.000000 checkio_client-0.3.4/checkio_client/actions/repo_convert.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     1563 2022-07-26 18:23:18.000000 checkio_client-0.3.4/checkio_client/actions/server.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     7289 2023-06-20 20:13:33.000000 checkio_client-0.3.4/checkio_client/actions/sync.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     4818 2020-12-30 11:27:28.000000 checkio_client-0.3.4/checkio_client/api.py
+drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2024-04-21 17:35:44.435450 checkio_client-0.3.4/checkio_client/eoc/
+-rw-r--r--   0 oduvan     (501) staff       (20)        0 2019-05-31 12:50:32.000000 checkio_client-0.3.4/checkio_client/eoc/__init__.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     3778 2019-06-01 11:46:59.000000 checkio_client-0.3.4/checkio_client/eoc/folder.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     4927 2019-11-18 15:20:38.000000 checkio_client-0.3.4/checkio_client/eoc/getters.py
+-rw-r--r--   0 oduvan     (501) staff       (20)      992 2019-06-06 07:49:17.000000 checkio_client-0.3.4/checkio_client/eoc/initial.py
+-rw-r--r--   0 oduvan     (501) staff       (20)      852 2019-05-31 12:50:32.000000 checkio_client-0.3.4/checkio_client/eoc/settings.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     7576 2019-11-16 15:36:16.000000 checkio_client-0.3.4/checkio_client/eoc/testing.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     4236 2019-11-18 15:23:59.000000 checkio_client-0.3.4/checkio_client/eoc_runner.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     9650 2023-03-07 17:26:58.000000 checkio_client-0.3.4/checkio_client/runner.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     5632 2023-06-20 20:13:33.000000 checkio_client-0.3.4/checkio_client/settings.py
+drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2024-04-21 17:35:44.436477 checkio_client-0.3.4/checkio_client/utils/
+-rw-r--r--   0 oduvan     (501) staff       (20)        0 2018-07-04 11:20:22.000000 checkio_client-0.3.4/checkio_client/utils/__init__.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     4819 2022-07-06 17:14:47.000000 checkio_client-0.3.4/checkio_client/utils/code.py
+drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2024-04-21 17:35:44.438587 checkio_client-0.3.4/checkio_client/verification/
+-rw-r--r--   0 oduvan     (501) staff       (20)        0 2018-07-06 10:10:36.000000 checkio_client-0.3.4/checkio_client/verification/__init__.py
+drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2024-04-21 17:35:44.443215 checkio_client-0.3.4/checkio_client/verification/checkio/
+-rw-r--r--   0 oduvan     (501) staff       (20)        0 2017-02-10 12:27:49.000000 checkio_client-0.3.4/checkio_client/verification/checkio/__init__.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     3305 2021-11-04 10:20:03.000000 checkio_client-0.3.4/checkio_client/verification/checkio/api.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     4637 2022-02-19 17:39:13.000000 checkio_client-0.3.4/checkio_client/verification/checkio/code_template.py
+drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2024-04-21 17:35:44.449447 checkio_client-0.3.4/checkio_client/verification/checkio/referees/
+-rw-r--r--   0 oduvan     (501) staff       (20)        0 2017-02-10 12:27:49.000000 checkio_client-0.3.4/checkio_client/verification/checkio/referees/__init__.py
+-rw-r--r--   0 oduvan     (501) staff       (20)      620 2022-08-10 15:15:11.000000 checkio_client-0.3.4/checkio_client/verification/checkio/referees/checkers.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     2441 2021-11-01 00:20:52.000000 checkio_client-0.3.4/checkio_client/verification/checkio/referees/code.py
+-rw-r--r--   0 oduvan     (501) staff       (20)      255 2017-02-10 12:27:49.000000 checkio_client-0.3.4/checkio_client/verification/checkio/referees/cover_codes.py
+-rw-r--r--   0 oduvan     (501) staff       (20)      282 2017-02-10 12:27:49.000000 checkio_client-0.3.4/checkio_client/verification/checkio/referees/inspectors.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     5627 2021-11-14 22:28:37.000000 checkio_client-0.3.4/checkio_client/verification/checkio/referees/io.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     2436 2021-12-15 10:22:29.000000 checkio_client-0.3.4/checkio_client/verification/checkio/referees/io_template.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     4579 2017-02-10 12:27:49.000000 checkio_client-0.3.4/checkio_client/verification/checkio/referees/multicall.py
+-rw-r--r--   0 oduvan     (501) staff       (20)       78 2017-02-10 12:27:49.000000 checkio_client-0.3.4/checkio_client/verification/checkio/runner_types.py
+-rw-r--r--   0 oduvan     (501) staff       (20)      141 2017-02-10 12:27:49.000000 checkio_client-0.3.4/checkio_client/verification/checkio/signals.py
+-rw-r--r--   0 oduvan     (501) staff       (20)      487 2017-02-10 12:27:49.000000 checkio_client-0.3.4/checkio_client/verification/checkio/utils.py
+-rw-r--r--   0 oduvan     (501) staff       (20)     1619 2023-06-20 20:13:33.000000 checkio_client-0.3.4/checkio_client/verification/echo.py
+-rw-r--r--   0 oduvan     (501) staff       (20)      828 2021-07-13 14:00:30.000000 checkio_client-0.3.4/checkio_client/verification/uch.py
+-rwxr-xr-x   0 oduvan     (501) staff       (20)     7386 2021-10-11 17:42:31.000000 checkio_client-0.3.4/checkio_client/web_plugin.py
+drwxr-xr-x   0 oduvan     (501) staff       (20)        0 2024-04-21 17:35:44.420983 checkio_client-0.3.4/checkio_client.egg-info/
+-rw-r--r--   0 oduvan     (501) staff       (20)      456 2024-04-21 17:35:44.000000 checkio_client-0.3.4/checkio_client.egg-info/PKG-INFO
+-rw-r--r--   0 oduvan     (501) staff       (20)     1944 2024-04-21 17:35:44.000000 checkio_client-0.3.4/checkio_client.egg-info/SOURCES.txt
+-rw-r--r--   0 oduvan     (501) staff       (20)        1 2024-04-21 17:35:44.000000 checkio_client-0.3.4/checkio_client.egg-info/dependency_links.txt
+-rw-r--r--   0 oduvan     (501) staff       (20)       56 2024-04-21 17:35:44.000000 checkio_client-0.3.4/checkio_client.egg-info/entry_points.txt
+-rw-r--r--   0 oduvan     (501) staff       (20)      149 2024-04-21 17:35:44.000000 checkio_client-0.3.4/checkio_client.egg-info/requires.txt
+-rw-r--r--   0 oduvan     (501) staff       (20)       15 2024-04-21 17:35:44.000000 checkio_client-0.3.4/checkio_client.egg-info/top_level.txt
+-rw-r--r--   0 oduvan     (501) staff       (20)       38 2024-04-21 17:35:44.452733 checkio_client-0.3.4/setup.cfg
+-rw-r--r--   0 oduvan     (501) staff       (20)      842 2024-04-17 14:54:36.000000 checkio_client-0.3.4/setup.py
```

### Comparing `checkio_client-0.3.3/LICENSE` & `checkio_client-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/README.md` & `checkio_client-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/actions/available.py` & `checkio_client-0.3.4/checkio_client/actions/available.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/actions/check.py` & `checkio_client-0.3.4/checkio_client/actions/check.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/actions/config.py` & `checkio_client-0.3.4/checkio_client/actions/config.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/actions/eoc.py` & `checkio_client-0.3.4/checkio_client/actions/eoc.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/actions/init.py` & `checkio_client-0.3.4/checkio_client/actions/init.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/actions/open.py` & `checkio_client-0.3.4/checkio_client/actions/open.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/actions/plugin.py` & `checkio_client-0.3.4/checkio_client/actions/plugin.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/actions/repo.py` & `checkio_client-0.3.4/checkio_client/actions/repo.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/actions/repo_check.py` & `checkio_client-0.3.4/checkio_client/actions/repo_check.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/actions/repo_convert.py` & `checkio_client-0.3.4/checkio_client/actions/repo_convert.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/actions/server.py` & `checkio_client-0.3.4/checkio_client/actions/server.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/actions/sync.py` & `checkio_client-0.3.4/checkio_client/actions/sync.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/api.py` & `checkio_client-0.3.4/checkio_client/api.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/eoc/folder.py` & `checkio_client-0.3.4/checkio_client/eoc/folder.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/eoc/getters.py` & `checkio_client-0.3.4/checkio_client/eoc/getters.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/eoc/initial.py` & `checkio_client-0.3.4/checkio_client/eoc/initial.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/eoc/settings.py` & `checkio_client-0.3.4/checkio_client/eoc/settings.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/eoc/testing.py` & `checkio_client-0.3.4/checkio_client/eoc/testing.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/eoc_runner.py` & `checkio_client-0.3.4/checkio_client/eoc_runner.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/runner.py` & `checkio_client-0.3.4/checkio_client/runner.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/settings.py` & `checkio_client-0.3.4/checkio_client/settings.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/utils/code.py` & `checkio_client-0.3.4/checkio_client/utils/code.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/verification/checkio/api.py` & `checkio_client-0.3.4/checkio_client/verification/checkio/api.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/verification/checkio/code_template.py` & `checkio_client-0.3.4/checkio_client/verification/checkio/code_template.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/verification/checkio/referees/checkers.py` & `checkio_client-0.3.4/checkio_client/verification/checkio/referees/checkers.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/verification/checkio/referees/code.py` & `checkio_client-0.3.4/checkio_client/verification/checkio/referees/code.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/verification/checkio/referees/io.py` & `checkio_client-0.3.4/checkio_client/verification/checkio/referees/io.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/verification/checkio/referees/io_template.py` & `checkio_client-0.3.4/checkio_client/verification/checkio/referees/io_template.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/verification/checkio/referees/multicall.py` & `checkio_client-0.3.4/checkio_client/verification/checkio/referees/multicall.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/verification/echo.py` & `checkio_client-0.3.4/checkio_client/verification/echo.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/verification/uch.py` & `checkio_client-0.3.4/checkio_client/verification/uch.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client/web_plugin.py` & `checkio_client-0.3.4/checkio_client/web_plugin.py`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/checkio_client.egg-info/SOURCES.txt` & `checkio_client-0.3.4/checkio_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `checkio_client-0.3.3/setup.py` & `checkio_client-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = f.read().strip().splitlines()
 
 
 source_directory = dirname(abspath(__file__))
 
 setup(
     name='checkio_client',
-    version='0.3.3',
+    version='0.3.4',
     python_requires='>=3.8',
     description='Command line interface for playing CheckiO games',
     author='CheckiO',
     author_email='a.lyabah@checkio.org',
     url='https://github.com/CheckiO/checkio-client',
     packages=find_packages(),
     install_requires=requirements,
```


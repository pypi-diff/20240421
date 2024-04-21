# Comparing `tmp/arrapi-1.4.7.tar.gz` & `tmp/arrapi-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrapi-1.4.7.tar", last modified: Tue Jan  2 20:08:59 2024, max compression
+gzip compressed data, was "arrapi-1.4.8.tar", last modified: Sun Apr 21 18:03:49 2024, max compression
```

## Comparing `arrapi-1.4.7.tar` & `arrapi-1.4.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 20:08:59.952550 arrapi-1.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-02 20:08:50.000000 arrapi-1.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13582 2024-01-02 20:08:59.952550 arrapi-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12541 2024-01-02 20:08:50.000000 arrapi-1.4.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 20:08:59.944550 arrapi-1.4.7/arrapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 20:08:59.948550 arrapi-1.4.7/arrapi/apis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/apis/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/apis/lidarr.py
--rw-r--r--   0 runner    (1001) docker     (127)    20751 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/apis/radarr.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/apis/readarr.py
--rw-r--r--   0 runner    (1001) docker     (127)    24653 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/apis/sonarr.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 20:08:59.948550 arrapi-1.4.7/arrapi/objs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/objs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/objs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    36475 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/objs/reload.py
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/objs/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 20:08:59.948550 arrapi-1.4.7/arrapi/raws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/raws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/raws/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/raws/lidarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/raws/radarr.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/raws/readarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-01-02 20:08:50.000000 arrapi-1.4.7/arrapi/raws/sonarr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 20:08:59.952550 arrapi-1.4.7/arrapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13582 2024-01-02 20:08:59.000000 arrapi-1.4.7/arrapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-01-02 20:08:59.000000 arrapi-1.4.7/arrapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 20:08:59.000000 arrapi-1.4.7/arrapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-02 20:08:59.000000 arrapi-1.4.7/arrapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-02 20:08:59.000000 arrapi-1.4.7/arrapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-02 20:08:59.952550 arrapi-1.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-01-02 20:08:50.000000 arrapi-1.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 20:08:59.948550 arrapi-1.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-01-02 20:08:50.000000 arrapi-1.4.7/tests/test_radarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-01-02 20:08:50.000000 arrapi-1.4.7/tests/test_sonarr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:49.410606 arrapi-1.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 18:03:36.000000 arrapi-1.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13981 2024-04-21 18:03:49.410606 arrapi-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12942 2024-04-21 18:03:36.000000 arrapi-1.4.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:49.402605 arrapi-1.4.8/arrapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:49.406606 arrapi-1.4.8/arrapi/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/apis/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/apis/lidarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20751 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/apis/radarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/apis/readarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24653 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/apis/sonarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:49.406606 arrapi-1.4.8/arrapi/objs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/objs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/objs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36475 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/objs/reload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/objs/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:49.406606 arrapi-1.4.8/arrapi/raws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/raws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/raws/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/raws/lidarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/raws/radarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/raws/readarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-21 18:03:36.000000 arrapi-1.4.8/arrapi/raws/sonarr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:49.406606 arrapi-1.4.8/arrapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13981 2024-04-21 18:03:49.000000 arrapi-1.4.8/arrapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-21 18:03:49.000000 arrapi-1.4.8/arrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 18:03:49.000000 arrapi-1.4.8/arrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 18:03:49.000000 arrapi-1.4.8/arrapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 18:03:49.000000 arrapi-1.4.8/arrapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 18:03:49.410606 arrapi-1.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-21 18:03:36.000000 arrapi-1.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:03:49.406606 arrapi-1.4.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-21 18:03:36.000000 arrapi-1.4.8/tests/test_radarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-04-21 18:03:36.000000 arrapi-1.4.8/tests/test_sonarr.py
```

### Comparing `arrapi-1.4.7/LICENSE` & `arrapi-1.4.8/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 meisnate12
+Copyright (c) 2024 meisnate12
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `arrapi-1.4.7/PKG-INFO` & `arrapi-1.4.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: arrapi
-Version: 1.4.7
+Version: 1.4.8
 Summary: Python wrapper for Radarr and Sonarr APIs:
-Home-page: https://github.com/meisnate12/ArrAPI
+Home-page: https://github.com/Kometa-Team/ArrAPI
 Author: Nathan Taggart
-Author-email: meisnate12@gmail.com
+Author-email: kometateam@proton.me
 License: MIT License
-Project-URL: Documentation, https://arrapi.metamanager.wiki
+Project-URL: Documentation, https://arrapi.kometa.wiki
 Project-URL: Funding, https://github.com/sponsors/meisnate12
-Project-URL: Source, https://github.com/meisnate12/ArrAPI
-Project-URL: Issues, https://github.com/meisnate12/ArrAPI/issues
+Project-URL: Source, https://github.com/Kometa-Team/ArrAPI
+Project-URL: Issues, https://github.com/Kometa-Team/ArrAPI/issues
 Keywords: arrapi,sonarr,radarr,arr,wrapper,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -23,41 +23,55 @@
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: requests
 
 ArrAPI
 ==========================================================
 
-.. image:: https://img.shields.io/travis/com/meisnate12/ArrAPI?style=plastic
-    :target: https://app.travis-ci.com/meisnate12/ArrAPI
-    :alt: Build Testing
+.. image:: https://img.shields.io/github/v/release/Kometa-Team/ArrAPI?style=plastic
+    :target: https://github.com/Kometa-Team/ArrAPI/releases
+    :alt: GitHub release (latest by date)
 
-.. image:: https://img.shields.io/readthedocs/arrapi?style=plastic
-    :target: https://arrapi.metamanager.wiki
-    :alt: Read the Docs
+.. image:: https://img.shields.io/travis/com/Kometa-Team/ArrAPI?style=plastic
+    :target: https://app.travis-ci.com/Kometa-Team/ArrAPI
+    :alt: Build Testing
 
-.. image:: https://img.shields.io/github/v/release/meisnate12/ArrAPI?style=plastic
-    :target: https://github.com/meisnate12/ArrAPI/releases
-    :alt: GitHub release (latest by date)
+.. image:: https://img.shields.io/github/commits-since/Kometa-Team/ArrAPI/latest?style=plastic
+    :target: https://github.com/Kometa-Team/ArrAPI/commits/master
+    :alt: GitHub commits since latest release (by date) for a branch
 
 .. image:: https://img.shields.io/pypi/v/ArrAPI?style=plastic
     :target: https://pypi.org/project/arrapi/
     :alt: PyPI
 
 .. image:: https://img.shields.io/pypi/dm/arrapi.svg?style=plastic
     :target: https://pypi.org/project/arrapi/
     :alt: Downloads
 
-.. image:: https://img.shields.io/github/commits-since/meisnate12/ArrAPI/latest?style=plastic
-    :target: https://github.com/meisnate12/ArrAPI/commits/master
-    :alt: GitHub commits since latest release (by date) for a branch
+|
 
-.. image:: https://img.shields.io/badge/-Sponsor_or_Donate-blueviolet?style=plastic
+.. image:: https://img.shields.io/readthedocs/arrapi?style=plastic
+    :target: https://arrapi.kometa.wiki
+    :alt: Wiki
+
+.. image:: https://img.shields.io/discord/822460010649878528?color=%2300bc8c&label=Discord&style=plastic
+    :target: https://kometa.wiki/en/latest/discord/
+    :alt: Discord
+
+.. image:: https://img.shields.io/reddit/subreddit-subscribers/Kometa?color=%2300bc8c&label=r%2FKometa&style=plastic
+    :target: https://www.reddit.com/r/Kometa/
+    :alt: Reddit
+
+.. image:: https://img.shields.io/github/sponsors/meisnate12?color=%238a2be2&style=plastic
     :target: https://github.com/sponsors/meisnate12
-    :alt: GitHub Sponsor
+    :alt: GitHub Sponsors
+
+.. image:: https://img.shields.io/badge/-Sponsor_or_Donate-blueviolet?style=plastic
+    :target: https://github.com/sponsors/Kometa-Team
+    :alt: Sponsor or Donate
 
 Overview
 ----------------------------------------------------------
 Unofficial Python bindings for the Sonarr and Radarr APIs. The goal is to make interaction with the API as easy as possible while emulating the Web Client as much as possible
 
 
 Installation & Documentation
@@ -65,15 +79,15 @@
 
 .. code-block:: python
 
     pip install arrapi
 
 Documentation_ can be found at Read the Docs.
 
-.. _Documentation: https://arrapi.metamanager.wiki
+.. _Documentation: https://arrapi.kometa.wiki
 
 Connecting to Sonarr
 ==========================================================
 
 Getting a SonarrAPI Instance
 ----------------------------------------------------------
 
@@ -316,77 +330,77 @@
 Hyperlinks
 ----------------------------------------------------------
 
 * `Radarr v3 API Docs <https://radarr.video/docs/api>`_
 * `Sonarr v3 API Docs <https://sonarr.tv/docs/api/>`_
 
 .. |SonarrAPI| replace:: ``SonarrAPI``
-.. _SonarrAPI: https://arrapi.metamanager.wiki/en/latest/sonarr.html#module-arrapi.sonarr
+.. _SonarrAPI: https://arrapi.kometa.wiki/en/latest/sonarr.html#module-arrapi.sonarr
 
 .. |Series| replace:: ``Series``
-.. _Series: https://arrapi.metamanager.wiki/en/latest/objs.html#series
+.. _Series: https://arrapi.kometa.wiki/en/latest/objs.html#series
 
 .. |get_series| replace:: ``get_series``
-.. _get_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.get_series
+.. _get_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.get_series
 
 .. |search_series| replace:: ``search_series``
-.. _search_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.search_series
+.. _search_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.search_series
 
 .. |all_series| replace:: ``all_series``
-.. _all_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.all_series
+.. _all_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.all_series
 
 .. |sonarr_add| replace:: ``add``
-.. _sonarr_add: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Series.add
+.. _sonarr_add: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Series.add
 
 .. |sonarr_edit| replace:: ``edit``
-.. _sonarr_edit: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Series.edit
+.. _sonarr_edit: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Series.edit
 
 .. |sonarr_delete| replace:: ``delete``
-.. _sonarr_delete: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Series.delete
+.. _sonarr_delete: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Series.delete
 
 .. |add_multiple_series| replace:: ``add_multiple_series``
-.. _add_multiple_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.add_multiple_series
+.. _add_multiple_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.add_multiple_series
 
 .. |edit_multiple_series| replace:: ``edit_multiple_series``
-.. _edit_multiple_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.edit_multiple_series
+.. _edit_multiple_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.edit_multiple_series
 
 .. |delete_multiple_series| replace:: ``delete_multiple_series``
-.. _delete_multiple_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.delete_multiple_series
+.. _delete_multiple_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.delete_multiple_series
 
 .. |sonarr_exclusions| replace:: ``sonarr_exclusions``
-.. _sonarr_exclusions: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.respect_list_exclusions_when_adding
+.. _sonarr_exclusions: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.respect_list_exclusions_when_adding
 
 .. |RadarrAPI| replace:: ``RadarrAPI``
-.. _RadarrAPI: https://arrapi.metamanager.wiki/en/latest/radarr.html#module-arrapi.radarr
+.. _RadarrAPI: https://arrapi.kometa.wiki/en/latest/radarr.html#module-arrapi.radarr
 
 .. |Movie| replace:: ``Movie``
-.. _Movie: https://arrapi.metamanager.wiki/en/latest/objs.html#movie
+.. _Movie: https://arrapi.kometa.wiki/en/latest/objs.html#movie
 
 .. |get_movie| replace:: ``get_movie``
-.. _get_movie: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.get_movie
+.. _get_movie: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.get_movie
 
 .. |search_movies| replace:: ``search_movies``
-.. _search_movies: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.search_movies
+.. _search_movies: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.search_movies
 
 .. |all_movies| replace:: ``all_movies``
-.. _all_movies: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.all_movies
+.. _all_movies: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.all_movies
 
 .. |radarr_add| replace:: ``add``
-.. _radarr_add: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Movie.add
+.. _radarr_add: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Movie.add
 
 .. |radarr_edit| replace:: ``edit``
-.. _radarr_edit: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Movie.edit
+.. _radarr_edit: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Movie.edit
 
 .. |radarr_delete| replace:: ``delete``
-.. _radarr_delete: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Movie.delete
+.. _radarr_delete: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Movie.delete
 
 .. |add_multiple_movies| replace:: ``add_multiple_movies``
-.. _add_multiple_movies: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.add_multiple_movies
+.. _add_multiple_movies: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.add_multiple_movies
 
 .. |edit_multiple_movies| replace:: ``edit_multiple_movies``
-.. _edit_multiple_movies: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.edit_multiple_movies
+.. _edit_multiple_movies: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.edit_multiple_movies
 
 .. |delete_multiple_movies| replace:: ``delete_multiple_movies``
-.. _delete_multiple_movies: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.delete_multiple_movies
+.. _delete_multiple_movies: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.delete_multiple_movies
 
 .. |radarr_exclusions| replace:: ``radarr_exclusions``
-.. _radarr_exclusions: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.respect_list_exclusions_when_adding
+.. _radarr_exclusions: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.respect_list_exclusions_when_adding
```

### Comparing `arrapi-1.4.7/README.rst` & `arrapi-1.4.8/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,51 @@
 ArrAPI
 ==========================================================
 
-.. image:: https://img.shields.io/travis/com/meisnate12/ArrAPI?style=plastic
-    :target: https://app.travis-ci.com/meisnate12/ArrAPI
-    :alt: Build Testing
+.. image:: https://img.shields.io/github/v/release/Kometa-Team/ArrAPI?style=plastic
+    :target: https://github.com/Kometa-Team/ArrAPI/releases
+    :alt: GitHub release (latest by date)
 
-.. image:: https://img.shields.io/readthedocs/arrapi?style=plastic
-    :target: https://arrapi.metamanager.wiki
-    :alt: Read the Docs
+.. image:: https://img.shields.io/travis/com/Kometa-Team/ArrAPI?style=plastic
+    :target: https://app.travis-ci.com/Kometa-Team/ArrAPI
+    :alt: Build Testing
 
-.. image:: https://img.shields.io/github/v/release/meisnate12/ArrAPI?style=plastic
-    :target: https://github.com/meisnate12/ArrAPI/releases
-    :alt: GitHub release (latest by date)
+.. image:: https://img.shields.io/github/commits-since/Kometa-Team/ArrAPI/latest?style=plastic
+    :target: https://github.com/Kometa-Team/ArrAPI/commits/master
+    :alt: GitHub commits since latest release (by date) for a branch
 
 .. image:: https://img.shields.io/pypi/v/ArrAPI?style=plastic
     :target: https://pypi.org/project/arrapi/
     :alt: PyPI
 
 .. image:: https://img.shields.io/pypi/dm/arrapi.svg?style=plastic
     :target: https://pypi.org/project/arrapi/
     :alt: Downloads
 
-.. image:: https://img.shields.io/github/commits-since/meisnate12/ArrAPI/latest?style=plastic
-    :target: https://github.com/meisnate12/ArrAPI/commits/master
-    :alt: GitHub commits since latest release (by date) for a branch
+|
 
-.. image:: https://img.shields.io/badge/-Sponsor_or_Donate-blueviolet?style=plastic
+.. image:: https://img.shields.io/readthedocs/arrapi?style=plastic
+    :target: https://arrapi.kometa.wiki
+    :alt: Wiki
+
+.. image:: https://img.shields.io/discord/822460010649878528?color=%2300bc8c&label=Discord&style=plastic
+    :target: https://kometa.wiki/en/latest/discord/
+    :alt: Discord
+
+.. image:: https://img.shields.io/reddit/subreddit-subscribers/Kometa?color=%2300bc8c&label=r%2FKometa&style=plastic
+    :target: https://www.reddit.com/r/Kometa/
+    :alt: Reddit
+
+.. image:: https://img.shields.io/github/sponsors/meisnate12?color=%238a2be2&style=plastic
     :target: https://github.com/sponsors/meisnate12
-    :alt: GitHub Sponsor
+    :alt: GitHub Sponsors
+
+.. image:: https://img.shields.io/badge/-Sponsor_or_Donate-blueviolet?style=plastic
+    :target: https://github.com/sponsors/Kometa-Team
+    :alt: Sponsor or Donate
 
 Overview
 ----------------------------------------------------------
 Unofficial Python bindings for the Sonarr and Radarr APIs. The goal is to make interaction with the API as easy as possible while emulating the Web Client as much as possible
 
 
 Installation & Documentation
@@ -39,15 +53,15 @@
 
 .. code-block:: python
 
     pip install arrapi
 
 Documentation_ can be found at Read the Docs.
 
-.. _Documentation: https://arrapi.metamanager.wiki
+.. _Documentation: https://arrapi.kometa.wiki
 
 Connecting to Sonarr
 ==========================================================
 
 Getting a SonarrAPI Instance
 ----------------------------------------------------------
 
@@ -290,77 +304,77 @@
 Hyperlinks
 ----------------------------------------------------------
 
 * `Radarr v3 API Docs <https://radarr.video/docs/api>`_
 * `Sonarr v3 API Docs <https://sonarr.tv/docs/api/>`_
 
 .. |SonarrAPI| replace:: ``SonarrAPI``
-.. _SonarrAPI: https://arrapi.metamanager.wiki/en/latest/sonarr.html#module-arrapi.sonarr
+.. _SonarrAPI: https://arrapi.kometa.wiki/en/latest/sonarr.html#module-arrapi.sonarr
 
 .. |Series| replace:: ``Series``
-.. _Series: https://arrapi.metamanager.wiki/en/latest/objs.html#series
+.. _Series: https://arrapi.kometa.wiki/en/latest/objs.html#series
 
 .. |get_series| replace:: ``get_series``
-.. _get_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.get_series
+.. _get_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.get_series
 
 .. |search_series| replace:: ``search_series``
-.. _search_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.search_series
+.. _search_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.search_series
 
 .. |all_series| replace:: ``all_series``
-.. _all_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.all_series
+.. _all_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.all_series
 
 .. |sonarr_add| replace:: ``add``
-.. _sonarr_add: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Series.add
+.. _sonarr_add: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Series.add
 
 .. |sonarr_edit| replace:: ``edit``
-.. _sonarr_edit: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Series.edit
+.. _sonarr_edit: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Series.edit
 
 .. |sonarr_delete| replace:: ``delete``
-.. _sonarr_delete: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Series.delete
+.. _sonarr_delete: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Series.delete
 
 .. |add_multiple_series| replace:: ``add_multiple_series``
-.. _add_multiple_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.add_multiple_series
+.. _add_multiple_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.add_multiple_series
 
 .. |edit_multiple_series| replace:: ``edit_multiple_series``
-.. _edit_multiple_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.edit_multiple_series
+.. _edit_multiple_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.edit_multiple_series
 
 .. |delete_multiple_series| replace:: ``delete_multiple_series``
-.. _delete_multiple_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.delete_multiple_series
+.. _delete_multiple_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.delete_multiple_series
 
 .. |sonarr_exclusions| replace:: ``sonarr_exclusions``
-.. _sonarr_exclusions: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.respect_list_exclusions_when_adding
+.. _sonarr_exclusions: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.respect_list_exclusions_when_adding
 
 .. |RadarrAPI| replace:: ``RadarrAPI``
-.. _RadarrAPI: https://arrapi.metamanager.wiki/en/latest/radarr.html#module-arrapi.radarr
+.. _RadarrAPI: https://arrapi.kometa.wiki/en/latest/radarr.html#module-arrapi.radarr
 
 .. |Movie| replace:: ``Movie``
-.. _Movie: https://arrapi.metamanager.wiki/en/latest/objs.html#movie
+.. _Movie: https://arrapi.kometa.wiki/en/latest/objs.html#movie
 
 .. |get_movie| replace:: ``get_movie``
-.. _get_movie: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.get_movie
+.. _get_movie: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.get_movie
 
 .. |search_movies| replace:: ``search_movies``
-.. _search_movies: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.search_movies
+.. _search_movies: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.search_movies
 
 .. |all_movies| replace:: ``all_movies``
-.. _all_movies: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.all_movies
+.. _all_movies: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.all_movies
 
 .. |radarr_add| replace:: ``add``
-.. _radarr_add: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Movie.add
+.. _radarr_add: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Movie.add
 
 .. |radarr_edit| replace:: ``edit``
-.. _radarr_edit: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Movie.edit
+.. _radarr_edit: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Movie.edit
 
 .. |radarr_delete| replace:: ``delete``
-.. _radarr_delete: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Movie.delete
+.. _radarr_delete: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Movie.delete
 
 .. |add_multiple_movies| replace:: ``add_multiple_movies``
-.. _add_multiple_movies: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.add_multiple_movies
+.. _add_multiple_movies: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.add_multiple_movies
 
 .. |edit_multiple_movies| replace:: ``edit_multiple_movies``
-.. _edit_multiple_movies: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.edit_multiple_movies
+.. _edit_multiple_movies: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.edit_multiple_movies
 
 .. |delete_multiple_movies| replace:: ``delete_multiple_movies``
-.. _delete_multiple_movies: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.delete_multiple_movies
+.. _delete_multiple_movies: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.delete_multiple_movies
 
 .. |radarr_exclusions| replace:: ``radarr_exclusions``
-.. _radarr_exclusions: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.respect_list_exclusions_when_adding
+.. _radarr_exclusions: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.respect_list_exclusions_when_adding
```

### Comparing `arrapi-1.4.7/arrapi/__init__.py` & `arrapi-1.4.8/arrapi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 except pkg_resources.DistributionNotFound:
     __version__ = ""
 __author__ = "Nathan Taggart"
 __credits__ = "meisnate12"
 __package_name__ = "arrapi"
 __project_name__ = "ArrAPI"
 __description__ = "Python wrapper for Radarr and Sonarr APIs:"
-__url__ = "https://github.com/meisnate12/ArrAPI"
-__email__ = 'meisnate12@gmail.com'
+__url__ = "https://github.com/Kometa-Team/ArrAPI"
+__email__ = "kometateam@proton.me"
 __license__ = 'MIT License'
 __all__ = [
     "RadarrAPI",
     "SonarrAPI",
     "QualityProfile",
     "LanguageProfile",
     "MetadataProfile",
```

### Comparing `arrapi-1.4.7/arrapi/apis/base.py` & `arrapi-1.4.8/arrapi/apis/base.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.7/arrapi/apis/radarr.py` & `arrapi-1.4.8/arrapi/apis/radarr.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.7/arrapi/apis/sonarr.py` & `arrapi-1.4.8/arrapi/apis/sonarr.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.7/arrapi/exceptions.py` & `arrapi-1.4.8/arrapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.7/arrapi/objs/base.py` & `arrapi-1.4.8/arrapi/objs/base.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.7/arrapi/objs/reload.py` & `arrapi-1.4.8/arrapi/objs/reload.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.7/arrapi/objs/simple.py` & `arrapi-1.4.8/arrapi/objs/simple.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.7/arrapi/raws/base.py` & `arrapi-1.4.8/arrapi/raws/base.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.7/arrapi/raws/radarr.py` & `arrapi-1.4.8/arrapi/raws/radarr.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.7/arrapi/raws/sonarr.py` & `arrapi-1.4.8/arrapi/raws/sonarr.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.7/arrapi.egg-info/PKG-INFO` & `arrapi-1.4.8/arrapi.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: arrapi
-Version: 1.4.7
+Version: 1.4.8
 Summary: Python wrapper for Radarr and Sonarr APIs:
-Home-page: https://github.com/meisnate12/ArrAPI
+Home-page: https://github.com/Kometa-Team/ArrAPI
 Author: Nathan Taggart
-Author-email: meisnate12@gmail.com
+Author-email: kometateam@proton.me
 License: MIT License
-Project-URL: Documentation, https://arrapi.metamanager.wiki
+Project-URL: Documentation, https://arrapi.kometa.wiki
 Project-URL: Funding, https://github.com/sponsors/meisnate12
-Project-URL: Source, https://github.com/meisnate12/ArrAPI
-Project-URL: Issues, https://github.com/meisnate12/ArrAPI/issues
+Project-URL: Source, https://github.com/Kometa-Team/ArrAPI
+Project-URL: Issues, https://github.com/Kometa-Team/ArrAPI/issues
 Keywords: arrapi,sonarr,radarr,arr,wrapper,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -23,41 +23,55 @@
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: requests
 
 ArrAPI
 ==========================================================
 
-.. image:: https://img.shields.io/travis/com/meisnate12/ArrAPI?style=plastic
-    :target: https://app.travis-ci.com/meisnate12/ArrAPI
-    :alt: Build Testing
+.. image:: https://img.shields.io/github/v/release/Kometa-Team/ArrAPI?style=plastic
+    :target: https://github.com/Kometa-Team/ArrAPI/releases
+    :alt: GitHub release (latest by date)
 
-.. image:: https://img.shields.io/readthedocs/arrapi?style=plastic
-    :target: https://arrapi.metamanager.wiki
-    :alt: Read the Docs
+.. image:: https://img.shields.io/travis/com/Kometa-Team/ArrAPI?style=plastic
+    :target: https://app.travis-ci.com/Kometa-Team/ArrAPI
+    :alt: Build Testing
 
-.. image:: https://img.shields.io/github/v/release/meisnate12/ArrAPI?style=plastic
-    :target: https://github.com/meisnate12/ArrAPI/releases
-    :alt: GitHub release (latest by date)
+.. image:: https://img.shields.io/github/commits-since/Kometa-Team/ArrAPI/latest?style=plastic
+    :target: https://github.com/Kometa-Team/ArrAPI/commits/master
+    :alt: GitHub commits since latest release (by date) for a branch
 
 .. image:: https://img.shields.io/pypi/v/ArrAPI?style=plastic
     :target: https://pypi.org/project/arrapi/
     :alt: PyPI
 
 .. image:: https://img.shields.io/pypi/dm/arrapi.svg?style=plastic
     :target: https://pypi.org/project/arrapi/
     :alt: Downloads
 
-.. image:: https://img.shields.io/github/commits-since/meisnate12/ArrAPI/latest?style=plastic
-    :target: https://github.com/meisnate12/ArrAPI/commits/master
-    :alt: GitHub commits since latest release (by date) for a branch
+|
 
-.. image:: https://img.shields.io/badge/-Sponsor_or_Donate-blueviolet?style=plastic
+.. image:: https://img.shields.io/readthedocs/arrapi?style=plastic
+    :target: https://arrapi.kometa.wiki
+    :alt: Wiki
+
+.. image:: https://img.shields.io/discord/822460010649878528?color=%2300bc8c&label=Discord&style=plastic
+    :target: https://kometa.wiki/en/latest/discord/
+    :alt: Discord
+
+.. image:: https://img.shields.io/reddit/subreddit-subscribers/Kometa?color=%2300bc8c&label=r%2FKometa&style=plastic
+    :target: https://www.reddit.com/r/Kometa/
+    :alt: Reddit
+
+.. image:: https://img.shields.io/github/sponsors/meisnate12?color=%238a2be2&style=plastic
     :target: https://github.com/sponsors/meisnate12
-    :alt: GitHub Sponsor
+    :alt: GitHub Sponsors
+
+.. image:: https://img.shields.io/badge/-Sponsor_or_Donate-blueviolet?style=plastic
+    :target: https://github.com/sponsors/Kometa-Team
+    :alt: Sponsor or Donate
 
 Overview
 ----------------------------------------------------------
 Unofficial Python bindings for the Sonarr and Radarr APIs. The goal is to make interaction with the API as easy as possible while emulating the Web Client as much as possible
 
 
 Installation & Documentation
@@ -65,15 +79,15 @@
 
 .. code-block:: python
 
     pip install arrapi
 
 Documentation_ can be found at Read the Docs.
 
-.. _Documentation: https://arrapi.metamanager.wiki
+.. _Documentation: https://arrapi.kometa.wiki
 
 Connecting to Sonarr
 ==========================================================
 
 Getting a SonarrAPI Instance
 ----------------------------------------------------------
 
@@ -316,77 +330,77 @@
 Hyperlinks
 ----------------------------------------------------------
 
 * `Radarr v3 API Docs <https://radarr.video/docs/api>`_
 * `Sonarr v3 API Docs <https://sonarr.tv/docs/api/>`_
 
 .. |SonarrAPI| replace:: ``SonarrAPI``
-.. _SonarrAPI: https://arrapi.metamanager.wiki/en/latest/sonarr.html#module-arrapi.sonarr
+.. _SonarrAPI: https://arrapi.kometa.wiki/en/latest/sonarr.html#module-arrapi.sonarr
 
 .. |Series| replace:: ``Series``
-.. _Series: https://arrapi.metamanager.wiki/en/latest/objs.html#series
+.. _Series: https://arrapi.kometa.wiki/en/latest/objs.html#series
 
 .. |get_series| replace:: ``get_series``
-.. _get_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.get_series
+.. _get_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.get_series
 
 .. |search_series| replace:: ``search_series``
-.. _search_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.search_series
+.. _search_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.search_series
 
 .. |all_series| replace:: ``all_series``
-.. _all_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.all_series
+.. _all_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.all_series
 
 .. |sonarr_add| replace:: ``add``
-.. _sonarr_add: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Series.add
+.. _sonarr_add: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Series.add
 
 .. |sonarr_edit| replace:: ``edit``
-.. _sonarr_edit: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Series.edit
+.. _sonarr_edit: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Series.edit
 
 .. |sonarr_delete| replace:: ``delete``
-.. _sonarr_delete: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Series.delete
+.. _sonarr_delete: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Series.delete
 
 .. |add_multiple_series| replace:: ``add_multiple_series``
-.. _add_multiple_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.add_multiple_series
+.. _add_multiple_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.add_multiple_series
 
 .. |edit_multiple_series| replace:: ``edit_multiple_series``
-.. _edit_multiple_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.edit_multiple_series
+.. _edit_multiple_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.edit_multiple_series
 
 .. |delete_multiple_series| replace:: ``delete_multiple_series``
-.. _delete_multiple_series: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.delete_multiple_series
+.. _delete_multiple_series: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.delete_multiple_series
 
 .. |sonarr_exclusions| replace:: ``sonarr_exclusions``
-.. _sonarr_exclusions: https://arrapi.metamanager.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.respect_list_exclusions_when_adding
+.. _sonarr_exclusions: https://arrapi.kometa.wiki/en/latest/sonarr.html#arrapi.sonarr.SonarrAPI.respect_list_exclusions_when_adding
 
 .. |RadarrAPI| replace:: ``RadarrAPI``
-.. _RadarrAPI: https://arrapi.metamanager.wiki/en/latest/radarr.html#module-arrapi.radarr
+.. _RadarrAPI: https://arrapi.kometa.wiki/en/latest/radarr.html#module-arrapi.radarr
 
 .. |Movie| replace:: ``Movie``
-.. _Movie: https://arrapi.metamanager.wiki/en/latest/objs.html#movie
+.. _Movie: https://arrapi.kometa.wiki/en/latest/objs.html#movie
 
 .. |get_movie| replace:: ``get_movie``
-.. _get_movie: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.get_movie
+.. _get_movie: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.get_movie
 
 .. |search_movies| replace:: ``search_movies``
-.. _search_movies: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.search_movies
+.. _search_movies: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.search_movies
 
 .. |all_movies| replace:: ``all_movies``
-.. _all_movies: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.all_movies
+.. _all_movies: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.all_movies
 
 .. |radarr_add| replace:: ``add``
-.. _radarr_add: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Movie.add
+.. _radarr_add: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Movie.add
 
 .. |radarr_edit| replace:: ``edit``
-.. _radarr_edit: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Movie.edit
+.. _radarr_edit: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Movie.edit
 
 .. |radarr_delete| replace:: ``delete``
-.. _radarr_delete: https://arrapi.metamanager.wiki/en/latest/objs.html#arrapi.objs.Movie.delete
+.. _radarr_delete: https://arrapi.kometa.wiki/en/latest/objs.html#arrapi.objs.Movie.delete
 
 .. |add_multiple_movies| replace:: ``add_multiple_movies``
-.. _add_multiple_movies: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.add_multiple_movies
+.. _add_multiple_movies: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.add_multiple_movies
 
 .. |edit_multiple_movies| replace:: ``edit_multiple_movies``
-.. _edit_multiple_movies: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.edit_multiple_movies
+.. _edit_multiple_movies: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.edit_multiple_movies
 
 .. |delete_multiple_movies| replace:: ``delete_multiple_movies``
-.. _delete_multiple_movies: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.delete_multiple_movies
+.. _delete_multiple_movies: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.delete_multiple_movies
 
 .. |radarr_exclusions| replace:: ``radarr_exclusions``
-.. _radarr_exclusions: https://arrapi.metamanager.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.respect_list_exclusions_when_adding
+.. _radarr_exclusions: https://arrapi.kometa.wiki/en/latest/radarr.html#arrapi.radarr.RadarrAPI.respect_list_exclusions_when_adding
```

### Comparing `arrapi-1.4.7/arrapi.egg-info/SOURCES.txt` & `arrapi-1.4.8/arrapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.7/setup.py` & `arrapi-1.4.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,18 +26,18 @@
     packages=find_packages(),
     python_requires=">=3.8",
     keywords=["arrapi", "sonarr", "radarr", "arr", "wrapper", "api"],
     install_requires=[
         "requests"
     ],
     project_urls={
-        "Documentation": "https://arrapi.metamanager.wiki",
+        "Documentation": "https://arrapi.kometa.wiki",
         "Funding": "https://github.com/sponsors/meisnate12",
-        "Source": "https://github.com/meisnate12/ArrAPI",
-        "Issues": "https://github.com/meisnate12/ArrAPI/issues",
+        "Source": "https://github.com/Kometa-Team/ArrAPI",
+        "Issues": "https://github.com/Kometa-Team/ArrAPI/issues",
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
```

### Comparing `arrapi-1.4.7/tests/test_radarr.py` & `arrapi-1.4.8/tests/test_radarr.py`

 * *Files identical despite different names*

### Comparing `arrapi-1.4.7/tests/test_sonarr.py` & `arrapi-1.4.8/tests/test_sonarr.py`

 * *Files identical despite different names*


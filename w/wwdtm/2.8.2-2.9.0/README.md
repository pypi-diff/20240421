# Comparing `tmp/wwdtm-2.8.2.tar.gz` & `tmp/wwdtm-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwdtm-2.8.2.tar", last modified: Thu Mar 21 02:47:14 2024, max compression
+gzip compressed data, was "wwdtm-2.9.0.tar", last modified: Sun Apr 21 03:50:55 2024, max compression
```

## Comparing `wwdtm-2.8.2.tar` & `wwdtm-2.9.0.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.326202 wwdtm-2.8.2/
--rw-r--r--   0 lpham      (501) staff       (20)    10142 2021-10-14 22:42:34.000000 wwdtm-2.8.2/LICENSE
--rw-r--r--   0 lpham      (501) staff       (20)      267 2022-01-03 00:36:38.000000 wwdtm-2.8.2/MANIFEST.in
--rw-r--r--   0 lpham      (501) staff       (20)     4490 2024-03-21 02:47:14.325976 wwdtm-2.8.2/PKG-INFO
--rw-r--r--   0 lpham      (501) staff       (20)     3497 2024-01-01 01:43:35.000000 wwdtm-2.8.2/README.rst
--rw-r--r--   0 lpham      (501) staff       (20)      344 2022-03-17 03:36:18.000000 wwdtm-2.8.2/config.json.dist
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.308860 wwdtm-2.8.2/docs/
--rw-r--r--   0 lpham      (501) staff       (20)      686 2021-10-14 22:42:34.000000 wwdtm-2.8.2/docs/Makefile
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.296512 wwdtm-2.8.2/docs/_static/
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.309113 wwdtm-2.8.2/docs/_static/css/
--rw-r--r--   0 lpham      (501) staff       (20)     1575 2024-01-12 18:49:15.000000 wwdtm-2.8.2/docs/_static/css/custom.css
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.309381 wwdtm-2.8.2/docs/_templates/
--rw-r--r--   0 lpham      (501) staff       (20)      193 2021-10-14 22:42:34.000000 wwdtm-2.8.2/docs/_templates/layout.html
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.309651 wwdtm-2.8.2/docs/changes/
--rw-r--r--   0 lpham      (501) staff       (20)    10192 2024-03-21 02:45:32.000000 wwdtm-2.8.2/docs/changes/index.rst
--rw-r--r--   0 lpham      (501) staff       (20)     1752 2024-01-12 18:49:15.000000 wwdtm-2.8.2/docs/conf.py
--rw-r--r--   0 lpham      (501) staff       (20)      223 2024-01-01 01:43:35.000000 wwdtm-2.8.2/docs/environment.yaml
--rw-r--r--   0 lpham      (501) staff       (20)     1243 2024-01-12 18:49:15.000000 wwdtm-2.8.2/docs/index.rst
--rw-r--r--   0 lpham      (501) staff       (20)     2927 2022-11-13 00:18:03.000000 wwdtm-2.8.2/docs/known_issues.rst
--rw-r--r--   0 lpham      (501) staff       (20)      795 2021-10-14 22:42:34.000000 wwdtm-2.8.2/docs/make.bat
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.311243 wwdtm-2.8.2/docs/migrating/
--rw-r--r--   0 lpham      (501) staff       (20)     1886 2022-03-17 03:36:18.000000 wwdtm-2.8.2/docs/migrating/guest.rst
--rw-r--r--   0 lpham      (501) staff       (20)     1854 2022-03-17 03:36:18.000000 wwdtm-2.8.2/docs/migrating/host.rst
--rw-r--r--   0 lpham      (501) staff       (20)     2821 2024-01-01 01:43:35.000000 wwdtm-2.8.2/docs/migrating/index.rst
--rw-r--r--   0 lpham      (501) staff       (20)     2320 2022-03-17 03:36:18.000000 wwdtm-2.8.2/docs/migrating/location.rst
--rw-r--r--   0 lpham      (501) staff       (20)     3802 2022-03-17 03:36:18.000000 wwdtm-2.8.2/docs/migrating/panelist.rst
--rw-r--r--   0 lpham      (501) staff       (20)     2050 2022-03-17 03:36:18.000000 wwdtm-2.8.2/docs/migrating/scorekeeper.rst
--rw-r--r--   0 lpham      (501) staff       (20)     2572 2022-03-17 03:36:18.000000 wwdtm-2.8.2/docs/migrating/show.rst
--rw-r--r--   0 lpham      (501) staff       (20)      281 2024-01-12 18:49:15.000000 wwdtm-2.8.2/docs/requirements.txt
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.312927 wwdtm-2.8.2/docs/tests/
--rw-r--r--   0 lpham      (501) staff       (20)      631 2024-01-12 18:49:15.000000 wwdtm-2.8.2/docs/tests/guest.rst
--rw-r--r--   0 lpham      (501) staff       (20)      608 2022-03-17 03:36:18.000000 wwdtm-2.8.2/docs/tests/host.rst
--rw-r--r--   0 lpham      (501) staff       (20)      312 2024-01-12 18:49:15.000000 wwdtm-2.8.2/docs/tests/index.rst
--rw-r--r--   0 lpham      (501) staff       (20)      704 2022-03-17 03:36:18.000000 wwdtm-2.8.2/docs/tests/location.rst
--rw-r--r--   0 lpham      (501) staff       (20)     1064 2022-03-17 03:36:18.000000 wwdtm-2.8.2/docs/tests/panelist.rst
--rw-r--r--   0 lpham      (501) staff       (20)      783 2022-03-17 03:36:18.000000 wwdtm-2.8.2/docs/tests/scorekeeper.rst
--rw-r--r--   0 lpham      (501) staff       (20)      757 2022-03-17 03:36:18.000000 wwdtm-2.8.2/docs/tests/show.rst
--rw-r--r--   0 lpham      (501) staff       (20)      287 2022-03-17 03:36:18.000000 wwdtm-2.8.2/docs/tests/validation.rst
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.314519 wwdtm-2.8.2/docs/wwdtm/
--rw-r--r--   0 lpham      (501) staff       (20)      562 2024-01-12 18:49:15.000000 wwdtm-2.8.2/docs/wwdtm/guest.rst
--rw-r--r--   0 lpham      (501) staff       (20)      579 2024-01-12 18:49:15.000000 wwdtm-2.8.2/docs/wwdtm/host.rst
--rw-r--r--   0 lpham      (501) staff       (20)      435 2022-03-17 03:36:18.000000 wwdtm-2.8.2/docs/wwdtm/index.rst
--rw-r--r--   0 lpham      (501) staff       (20)      664 2024-01-12 18:49:15.000000 wwdtm-2.8.2/docs/wwdtm/location.rst
--rw-r--r--   0 lpham      (501) staff       (20)     1034 2024-01-12 18:49:15.000000 wwdtm-2.8.2/docs/wwdtm/panelist.rst
--rw-r--r--   0 lpham      (501) staff       (20)      712 2024-01-12 18:49:15.000000 wwdtm-2.8.2/docs/wwdtm/scorekeeper.rst
--rw-r--r--   0 lpham      (501) staff       (20)      676 2024-01-12 18:49:15.000000 wwdtm-2.8.2/docs/wwdtm/show.rst
--rw-r--r--   0 lpham      (501) staff       (20)      219 2024-01-12 18:49:15.000000 wwdtm-2.8.2/docs/wwdtm/validation.rst
--rw-r--r--   0 lpham      (501) staff       (20)     2970 2024-03-21 02:45:32.000000 wwdtm-2.8.2/pyproject.toml
--rw-r--r--   0 lpham      (501) staff       (20)       38 2024-03-21 02:47:14.326247 wwdtm-2.8.2/setup.cfg
--rw-r--r--   0 lpham      (501) staff       (20)      255 2024-01-12 18:49:15.000000 wwdtm-2.8.2/setup.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.314713 wwdtm-2.8.2/tests/
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.315353 wwdtm-2.8.2/tests/guest/
--rw-r--r--   0 lpham      (501) staff       (20)     2008 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/guest/test_guest_appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     4192 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/guest/test_guest_guest.py
--rw-r--r--   0 lpham      (501) staff       (20)     4536 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/guest/test_guest_utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.316044 wwdtm-2.8.2/tests/host/
--rw-r--r--   0 lpham      (501) staff       (20)     1999 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/host/test_host_appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     4064 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/host/test_host_host.py
--rw-r--r--   0 lpham      (501) staff       (20)     4346 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/host/test_host_utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.316608 wwdtm-2.8.2/tests/location/
--rw-r--r--   0 lpham      (501) staff       (20)     4541 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/location/test_location_location.py
--rw-r--r--   0 lpham      (501) staff       (20)     2112 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/location/test_location_recordings.py
--rw-r--r--   0 lpham      (501) staff       (20)     8722 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/location/test_location_utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.317877 wwdtm-2.8.2/tests/panelist/
--rw-r--r--   0 lpham      (501) staff       (20)     4016 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/panelist/test_panelist_appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     6795 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/panelist/test_panelist_decimal_scores.py
--rw-r--r--   0 lpham      (501) staff       (20)     5179 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/panelist/test_panelist_panelist.py
--rw-r--r--   0 lpham      (501) staff       (20)     6641 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/panelist/test_panelist_scores.py
--rw-r--r--   0 lpham      (501) staff       (20)     5183 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/panelist/test_panelist_statistics.py
--rw-r--r--   0 lpham      (501) staff       (20)     4688 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/panelist/test_panelist_utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.318428 wwdtm-2.8.2/tests/scorekeeper/
--rw-r--r--   0 lpham      (501) staff       (20)     2236 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/scorekeeper/test_scorekeeper_appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     4834 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/scorekeeper/test_scorekeeper_scorekeeper.py
--rw-r--r--   0 lpham      (501) staff       (20)     5122 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/scorekeeper/test_scorekeeper_utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.319425 wwdtm-2.8.2/tests/show/
--rw-r--r--   0 lpham      (501) staff       (20)     4204 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/show/test_show_info.py
--rw-r--r--   0 lpham      (501) staff       (20)     9501 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/show/test_show_info_multiple.py
--rw-r--r--   0 lpham      (501) staff       (20)    15332 2024-02-12 01:12:44.000000 wwdtm-2.8.2/tests/show/test_show_show.py
--rw-r--r--   0 lpham      (501) staff       (20)     5144 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/show/test_show_utility.py
--rw-r--r--   0 lpham      (501) staff       (20)      848 2024-01-12 18:49:15.000000 wwdtm-2.8.2/tests/test_validation.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.319847 wwdtm-2.8.2/wwdtm/
--rw-r--r--   0 lpham      (501) staff       (20)      792 2024-03-21 02:45:32.000000 wwdtm-2.8.2/wwdtm/__init__.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.321172 wwdtm-2.8.2/wwdtm/guest/
--rw-r--r--   0 lpham      (501) staff       (20)      317 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/guest/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)     4814 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/guest/appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     7500 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/guest/guest.py
--rw-r--r--   0 lpham      (501) staff       (20)     4162 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/guest/utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.321846 wwdtm-2.8.2/wwdtm/host/
--rw-r--r--   0 lpham      (501) staff       (20)      312 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/host/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)     4488 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/host/appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     7345 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/host/host.py
--rw-r--r--   0 lpham      (501) staff       (20)     4133 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/host/utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.322628 wwdtm-2.8.2/wwdtm/location/
--rw-r--r--   0 lpham      (501) staff       (20)      330 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/location/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)     9782 2024-03-21 02:45:32.000000 wwdtm-2.8.2/wwdtm/location/location.py
--rw-r--r--   0 lpham      (501) staff       (20)     4460 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/location/recordings.py
--rw-r--r--   0 lpham      (501) staff       (20)     5472 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/location/utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.323911 wwdtm-2.8.2/wwdtm/panelist/
--rw-r--r--   0 lpham      (501) staff       (20)      460 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/panelist/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)    10466 2024-03-21 02:45:32.000000 wwdtm-2.8.2/wwdtm/panelist/appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)    11473 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/panelist/decimal_scores.py
--rw-r--r--   0 lpham      (501) staff       (20)     9353 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/panelist/panelist.py
--rw-r--r--   0 lpham      (501) staff       (20)    10553 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/panelist/scores.py
--rw-r--r--   0 lpham      (501) staff       (20)    10132 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/panelist/statistics.py
--rw-r--r--   0 lpham      (501) staff       (20)     4315 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/panelist/utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.324614 wwdtm-2.8.2/wwdtm/scorekeeper/
--rw-r--r--   0 lpham      (501) staff       (20)      347 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/scorekeeper/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)     4782 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/scorekeeper/appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     7990 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/scorekeeper/scorekeeper.py
--rw-r--r--   0 lpham      (501) staff       (20)     4530 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/scorekeeper/utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.325501 wwdtm-2.8.2/wwdtm/show/
--rw-r--r--   0 lpham      (501) staff       (20)      342 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/show/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)    15149 2024-03-21 02:45:32.000000 wwdtm-2.8.2/wwdtm/show/info.py
--rw-r--r--   0 lpham      (501) staff       (20)    30399 2024-03-21 02:45:32.000000 wwdtm-2.8.2/wwdtm/show/info_multiple.py
--rw-r--r--   0 lpham      (501) staff       (20)    29362 2024-01-17 00:39:30.000000 wwdtm-2.8.2/wwdtm/show/show.py
--rw-r--r--   0 lpham      (501) staff       (20)     4313 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/show/utility.py
--rw-r--r--   0 lpham      (501) staff       (20)      824 2024-01-12 18:49:15.000000 wwdtm-2.8.2/wwdtm/validation.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-03-21 02:47:14.325677 wwdtm-2.8.2/wwdtm.egg-info/
--rw-r--r--   0 lpham      (501) staff       (20)     4490 2024-03-21 02:47:14.000000 wwdtm-2.8.2/wwdtm.egg-info/PKG-INFO
--rw-r--r--   0 lpham      (501) staff       (20)     3400 2024-03-21 02:47:14.000000 wwdtm-2.8.2/wwdtm.egg-info/SOURCES.txt
--rw-r--r--   0 lpham      (501) staff       (20)        1 2024-03-21 02:47:14.000000 wwdtm-2.8.2/wwdtm.egg-info/dependency_links.txt
--rw-r--r--   0 lpham      (501) staff       (20)       85 2024-03-21 02:47:14.000000 wwdtm-2.8.2/wwdtm.egg-info/requires.txt
--rw-r--r--   0 lpham      (501) staff       (20)        6 2024-03-21 02:47:14.000000 wwdtm-2.8.2/wwdtm.egg-info/top_level.txt
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.591853 wwdtm-2.9.0/
+-rw-r--r--   0 lpham      (501) staff       (20)    10142 2021-10-14 22:42:34.000000 wwdtm-2.9.0/LICENSE
+-rw-r--r--   0 lpham      (501) staff       (20)      267 2022-01-03 00:36:38.000000 wwdtm-2.9.0/MANIFEST.in
+-rw-r--r--   0 lpham      (501) staff       (20)     4484 2024-04-21 03:50:55.591563 wwdtm-2.9.0/PKG-INFO
+-rw-r--r--   0 lpham      (501) staff       (20)     3497 2024-01-01 01:43:35.000000 wwdtm-2.9.0/README.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      344 2022-03-17 03:36:18.000000 wwdtm-2.9.0/config.json.dist
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.574139 wwdtm-2.9.0/docs/
+-rw-r--r--   0 lpham      (501) staff       (20)      686 2021-10-14 22:42:34.000000 wwdtm-2.9.0/docs/Makefile
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.564229 wwdtm-2.9.0/docs/_static/
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.574317 wwdtm-2.9.0/docs/_static/css/
+-rw-r--r--   0 lpham      (501) staff       (20)     1575 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/_static/css/custom.css
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.574552 wwdtm-2.9.0/docs/_templates/
+-rw-r--r--   0 lpham      (501) staff       (20)      193 2021-10-14 22:42:34.000000 wwdtm-2.9.0/docs/_templates/layout.html
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.574949 wwdtm-2.9.0/docs/changes/
+-rw-r--r--   0 lpham      (501) staff       (20)    10676 2024-04-21 03:50:14.000000 wwdtm-2.9.0/docs/changes/index.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     1752 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/conf.py
+-rw-r--r--   0 lpham      (501) staff       (20)      223 2024-01-01 01:43:35.000000 wwdtm-2.9.0/docs/environment.yaml
+-rw-r--r--   0 lpham      (501) staff       (20)     1243 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/index.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     2927 2022-11-13 00:18:03.000000 wwdtm-2.9.0/docs/known_issues.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      795 2021-10-14 22:42:34.000000 wwdtm-2.9.0/docs/make.bat
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.576699 wwdtm-2.9.0/docs/migrating/
+-rw-r--r--   0 lpham      (501) staff       (20)     1886 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/migrating/guest.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     1854 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/migrating/host.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     2821 2024-01-01 01:43:35.000000 wwdtm-2.9.0/docs/migrating/index.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     2320 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/migrating/location.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     3802 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/migrating/panelist.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     2050 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/migrating/scorekeeper.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     2572 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/migrating/show.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      260 2024-04-21 03:50:14.000000 wwdtm-2.9.0/docs/requirements.txt
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.578363 wwdtm-2.9.0/docs/tests/
+-rw-r--r--   0 lpham      (501) staff       (20)      631 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/tests/guest.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      608 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/tests/host.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      312 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/tests/index.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      704 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/tests/location.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     1064 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/tests/panelist.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      783 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/tests/scorekeeper.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      757 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/tests/show.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      287 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/tests/validation.rst
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.579959 wwdtm-2.9.0/docs/wwdtm/
+-rw-r--r--   0 lpham      (501) staff       (20)      562 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/wwdtm/guest.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      579 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/wwdtm/host.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      435 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/wwdtm/index.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      664 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/wwdtm/location.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     1034 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/wwdtm/panelist.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      712 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/wwdtm/scorekeeper.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      676 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/wwdtm/show.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      219 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/wwdtm/validation.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     3004 2024-04-21 03:50:14.000000 wwdtm-2.9.0/pyproject.toml
+-rw-r--r--   0 lpham      (501) staff       (20)       38 2024-04-21 03:50:55.591908 wwdtm-2.9.0/setup.cfg
+-rw-r--r--   0 lpham      (501) staff       (20)      255 2024-01-12 18:49:15.000000 wwdtm-2.9.0/setup.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.580167 wwdtm-2.9.0/tests/
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.581012 wwdtm-2.9.0/tests/guest/
+-rw-r--r--   0 lpham      (501) staff       (20)     2008 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/guest/test_guest_appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4192 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/guest/test_guest_guest.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4536 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/guest/test_guest_utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.581507 wwdtm-2.9.0/tests/host/
+-rw-r--r--   0 lpham      (501) staff       (20)     1999 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/host/test_host_appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     5174 2024-04-21 03:50:14.000000 wwdtm-2.9.0/tests/host/test_host_host.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4346 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/host/test_host_utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.581993 wwdtm-2.9.0/tests/location/
+-rw-r--r--   0 lpham      (501) staff       (20)     5395 2024-04-21 03:50:14.000000 wwdtm-2.9.0/tests/location/test_location_location.py
+-rw-r--r--   0 lpham      (501) staff       (20)     2112 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/location/test_location_recordings.py
+-rw-r--r--   0 lpham      (501) staff       (20)     8722 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/location/test_location_utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.582987 wwdtm-2.9.0/tests/panelist/
+-rw-r--r--   0 lpham      (501) staff       (20)     4016 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/panelist/test_panelist_appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     6795 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/panelist/test_panelist_decimal_scores.py
+-rw-r--r--   0 lpham      (501) staff       (20)     6377 2024-04-21 03:50:14.000000 wwdtm-2.9.0/tests/panelist/test_panelist_panelist.py
+-rw-r--r--   0 lpham      (501) staff       (20)     6641 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/panelist/test_panelist_scores.py
+-rw-r--r--   0 lpham      (501) staff       (20)     5183 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/panelist/test_panelist_statistics.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4688 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/panelist/test_panelist_utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.583490 wwdtm-2.9.0/tests/scorekeeper/
+-rw-r--r--   0 lpham      (501) staff       (20)     2236 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/scorekeeper/test_scorekeeper_appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     6074 2024-04-21 03:50:14.000000 wwdtm-2.9.0/tests/scorekeeper/test_scorekeeper_scorekeeper.py
+-rw-r--r--   0 lpham      (501) staff       (20)     5122 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/scorekeeper/test_scorekeeper_utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.584133 wwdtm-2.9.0/tests/show/
+-rw-r--r--   0 lpham      (501) staff       (20)     4204 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/show/test_show_info.py
+-rw-r--r--   0 lpham      (501) staff       (20)     9501 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/show/test_show_info_multiple.py
+-rw-r--r--   0 lpham      (501) staff       (20)    15332 2024-02-12 01:12:44.000000 wwdtm-2.9.0/tests/show/test_show_show.py
+-rw-r--r--   0 lpham      (501) staff       (20)     5144 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/show/test_show_utility.py
+-rw-r--r--   0 lpham      (501) staff       (20)      848 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/test_validation.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.584559 wwdtm-2.9.0/wwdtm/
+-rw-r--r--   0 lpham      (501) staff       (20)      792 2024-04-21 03:50:14.000000 wwdtm-2.9.0/wwdtm/__init__.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.585996 wwdtm-2.9.0/wwdtm/guest/
+-rw-r--r--   0 lpham      (501) staff       (20)      317 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/guest/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4814 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/guest/appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     7500 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/guest/guest.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4162 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/guest/utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.586823 wwdtm-2.9.0/wwdtm/host/
+-rw-r--r--   0 lpham      (501) staff       (20)      312 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/host/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4488 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/host/appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     7745 2024-04-21 03:50:14.000000 wwdtm-2.9.0/wwdtm/host/host.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4133 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/host/utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.587648 wwdtm-2.9.0/wwdtm/location/
+-rw-r--r--   0 lpham      (501) staff       (20)      330 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/location/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)    10282 2024-04-21 03:50:14.000000 wwdtm-2.9.0/wwdtm/location/location.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4460 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/location/recordings.py
+-rw-r--r--   0 lpham      (501) staff       (20)     5472 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/location/utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.589105 wwdtm-2.9.0/wwdtm/panelist/
+-rw-r--r--   0 lpham      (501) staff       (20)      460 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/panelist/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)    10466 2024-03-21 02:45:32.000000 wwdtm-2.9.0/wwdtm/panelist/appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)    11473 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/panelist/decimal_scores.py
+-rw-r--r--   0 lpham      (501) staff       (20)     9765 2024-04-21 03:50:14.000000 wwdtm-2.9.0/wwdtm/panelist/panelist.py
+-rw-r--r--   0 lpham      (501) staff       (20)    10553 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/panelist/scores.py
+-rw-r--r--   0 lpham      (501) staff       (20)    10132 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/panelist/statistics.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4315 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/panelist/utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.589939 wwdtm-2.9.0/wwdtm/scorekeeper/
+-rw-r--r--   0 lpham      (501) staff       (20)      347 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/scorekeeper/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4782 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/scorekeeper/appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     8468 2024-04-21 03:50:14.000000 wwdtm-2.9.0/wwdtm/scorekeeper/scorekeeper.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4530 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/scorekeeper/utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.591026 wwdtm-2.9.0/wwdtm/show/
+-rw-r--r--   0 lpham      (501) staff       (20)      342 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/show/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)    15317 2024-04-21 03:50:14.000000 wwdtm-2.9.0/wwdtm/show/info.py
+-rw-r--r--   0 lpham      (501) staff       (20)    30759 2024-04-21 03:50:14.000000 wwdtm-2.9.0/wwdtm/show/info_multiple.py
+-rw-r--r--   0 lpham      (501) staff       (20)    29362 2024-01-17 00:39:30.000000 wwdtm-2.9.0/wwdtm/show/show.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4313 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/show/utility.py
+-rw-r--r--   0 lpham      (501) staff       (20)      824 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/validation.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.591229 wwdtm-2.9.0/wwdtm.egg-info/
+-rw-r--r--   0 lpham      (501) staff       (20)     4484 2024-04-21 03:50:55.000000 wwdtm-2.9.0/wwdtm.egg-info/PKG-INFO
+-rw-r--r--   0 lpham      (501) staff       (20)     3400 2024-04-21 03:50:55.000000 wwdtm-2.9.0/wwdtm.egg-info/SOURCES.txt
+-rw-r--r--   0 lpham      (501) staff       (20)        1 2024-04-21 03:50:55.000000 wwdtm-2.9.0/wwdtm.egg-info/dependency_links.txt
+-rw-r--r--   0 lpham      (501) staff       (20)       79 2024-04-21 03:50:55.000000 wwdtm-2.9.0/wwdtm.egg-info/requires.txt
+-rw-r--r--   0 lpham      (501) staff       (20)        6 2024-04-21 03:50:55.000000 wwdtm-2.9.0/wwdtm.egg-info/top_level.txt
```

### Comparing `wwdtm-2.8.2/LICENSE` & `wwdtm-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/PKG-INFO` & `wwdtm-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwdtm
-Version: 2.8.2
+Version: 2.9.0
 Summary: Library used to query data from copy of Wait Wait Stats Database.
 Author-email: Linh Pham <dev@wwdt.me>
 License: Apache-2.0
 Project-URL: Documentation, https://docs.wwdt.me
 Project-URL: Source Code, https://github.com/questionlp/wwdtm
 Project-URL: Changes, https://docs.wwdt.me/latest/changes/
 Project-URL: Stats Page, https://stats.wwdt.me
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: mysql-connector-python==8.2.0
-Requires-Dist: numpy==1.26.3
+Requires-Dist: numpy==1.26.4
 Requires-Dist: python-slugify==8.0.1
-Requires-Dist: pytz==2023.3.post1
+Requires-Dist: pytz==2024.1
 
 ***********************
 Wait Wait Stats Library
 ***********************
 
 Overview
 ========
```

### Comparing `wwdtm-2.8.2/README.rst` & `wwdtm-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/Makefile` & `wwdtm-2.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/_static/css/custom.css` & `wwdtm-2.9.0/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/changes/index.rst` & `wwdtm-2.9.0/docs/changes/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,40 @@
 *******
 Changes
 *******
 
+2.9.0
+=====
+
+Application Changes
+-------------------
+
+* Add `latitude` and `longitude` properties to Locations
+* Add `pronouns` property to Hosts, Panelists and Scorekeepers
+
+Component Changes
+-----------------
+
+* Upgrade numpy from 1.26.3 to 1.26.4
+* Upgrade pytz from 2023.3.post1 to 2024.1
+
+Development Changes
+-------------------
+
+* Upgrade build from 1.0.3 to 1.2.1
+* Upgrade pytest from 7.4.4 to 8.1.1
+* Upgrade ruff from 0.1.13 to 0.3.6
+* Upgrade wheel from 0.42.0 to 0.43.0
+
 2.8.2
 =====
 
 Development Changes
 -------------------
+
 * Upgrade black from 23.12.1 to 24.3.0
 
 2.8.1
 =====
 
 Application Changes
 -------------------
```

### Comparing `wwdtm-2.8.2/docs/conf.py` & `wwdtm-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/index.rst` & `wwdtm-2.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/known_issues.rst` & `wwdtm-2.9.0/docs/known_issues.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/make.bat` & `wwdtm-2.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/migrating/guest.rst` & `wwdtm-2.9.0/docs/migrating/guest.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/migrating/host.rst` & `wwdtm-2.9.0/docs/migrating/host.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/migrating/index.rst` & `wwdtm-2.9.0/docs/migrating/index.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/migrating/location.rst` & `wwdtm-2.9.0/docs/migrating/location.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/migrating/panelist.rst` & `wwdtm-2.9.0/docs/migrating/panelist.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/migrating/scorekeeper.rst` & `wwdtm-2.9.0/docs/migrating/scorekeeper.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/migrating/show.rst` & `wwdtm-2.9.0/docs/migrating/show.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/tests/guest.rst` & `wwdtm-2.9.0/docs/tests/guest.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/tests/host.rst` & `wwdtm-2.9.0/docs/tests/host.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/tests/location.rst` & `wwdtm-2.9.0/docs/tests/location.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/tests/panelist.rst` & `wwdtm-2.9.0/docs/tests/panelist.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/tests/scorekeeper.rst` & `wwdtm-2.9.0/docs/tests/scorekeeper.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/tests/show.rst` & `wwdtm-2.9.0/docs/tests/show.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/wwdtm/guest.rst` & `wwdtm-2.9.0/docs/wwdtm/guest.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/wwdtm/host.rst` & `wwdtm-2.9.0/docs/wwdtm/host.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/wwdtm/location.rst` & `wwdtm-2.9.0/docs/wwdtm/location.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/wwdtm/panelist.rst` & `wwdtm-2.9.0/docs/wwdtm/panelist.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/wwdtm/scorekeeper.rst` & `wwdtm-2.9.0/docs/wwdtm/scorekeeper.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/docs/wwdtm/show.rst` & `wwdtm-2.9.0/docs/wwdtm/show.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/pyproject.toml` & `wwdtm-2.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -12,19 +12,20 @@
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Topic :: Software Development :: Libraries",
 ]
+
 dependencies = [
     "mysql-connector-python==8.2.0",
-    "numpy==1.26.3",
+    "numpy==1.26.4",
     "python-slugify==8.0.1",
-    "pytz==2023.3.post1",
+    "pytz==2024.1",
 ]
 
 [project.urls]
 Documentation = "https://docs.wwdt.me"
 "Source Code" = "https://github.com/questionlp/wwdtm"
 Changes = "https://docs.wwdt.me/latest/changes/"
 "Stats Page" = "https://stats.wwdt.me"
@@ -39,59 +40,43 @@
 
 [tool.black]
 required-version = "24.3.0"
 target-version = ["py310", "py311", "py312"]
 line-length = 88
 
 [tool.pytest.ini_options]
-minversion = "7.4"
+minversion = "8.0"
 filterwarnings = [
     "ignore::DeprecationWarning:mysql.*:",
 ]
 norecursedirs = [
     ".git",
     "venv",
     "dist",
     ".eggs",
     "wwdtm.egg-info",
 ]
 
 [tool.ruff]
 target-version = "py310"
-select = [
-    "B",   # flake8-bugbear
-    "C4",  # flake8-comprehensions
-    "D",   # pydocstyle
-    "E",   # Error
-    "F",   # pyflakes
-    "I",   # isort
-    "ISC", # flake8-implicit-str-concat
-    "N",   # pep8-naming
-    "PGH", # pygrep-hooks
-    "PTH", # flake8-use-pathlib
-    "Q",   # flake8-quotes
-    "S",   # bandit
-    "SIM", # flake8-simplify
-    "TRY", # tryceratops
-    "UP",  # pyupgrade
-    "W",   # Warning
-    "YTT", # flake8-2020
-]
 
 exclude = [
     "migrations",
     "__pycache__",
     "manage.py",
     "settings.py",
     "env",
     ".env",
     "venv",
     ".venv",
 ]
 
+line-length = 88 # Must agree with Black
+
+[tool.ruff.lint]
 ignore = [
     "B905",   # zip strict=True; remove once python <3.10 support is dropped.
     "D100",
     "D101",
     "D102",
     "D103",
     "D104",
@@ -102,32 +87,51 @@
     "D401",
     "E402",
     "E501",
     "F401",
     "TRY003", # Avoid specifying messages outside exception class; overly strict, especially for ValueError
     "S608",
 ]
-line-length = 88 # Must agree with Black
 
-[tool.ruff.flake8-bugbear]
+select = [
+    "B",   # flake8-bugbear
+    "C4",  # flake8-comprehensions
+    "D",   # pydocstyle
+    "E",   # Error
+    "F",   # pyflakes
+    "I",   # isort
+    "ISC", # flake8-implicit-str-concat
+    "N",   # pep8-naming
+    "PGH", # pygrep-hooks
+    "PTH", # flake8-use-pathlib
+    "Q",   # flake8-quotes
+    "S",   # bandit
+    "SIM", # flake8-simplify
+    "TRY", # tryceratops
+    "UP",  # pyupgrade
+    "W",   # Warning
+    "YTT", # flake8-2020
+]
+
+[tool.ruff.lint.flake8-bugbear]
 extend-immutable-calls = ["chr", "typer.Argument", "typer.Option"]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "pep257"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*.py" = [
     "D100",
     "D101",
     "D102",
     "D103",
     "D104",
     "D105",
     "D106",
     "D107",
     "S101",   # use of "assert"
     "S102",   # use of "exec"
     "S106",   # possible hardcoded password.
 ]
 
-[tool.ruff.pep8-naming]
+[tool.ruff.lint.pep8-naming]
 staticmethod-decorators = ["pydantic.validator", "pydantic.root_validator"]
```

### Comparing `wwdtm-2.8.2/tests/guest/test_guest_appearances.py` & `wwdtm-2.9.0/tests/guest/test_guest_appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/guest/test_guest_guest.py` & `wwdtm-2.9.0/tests/guest/test_guest_guest.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/guest/test_guest_utility.py` & `wwdtm-2.9.0/tests/guest/test_guest_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/host/test_host_appearances.py` & `wwdtm-2.9.0/tests/host/test_host_appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/host/test_host_host.py` & `wwdtm-2.9.0/tests/host/test_host_host.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,23 +30,29 @@
 def test_host_retrieve_all():
     """Testing for :py:meth:`wwdtm.host.Host.retrieve_all`."""
     host = Host(connect_dict=get_connect_dict())
     hosts = host.retrieve_all()
 
     assert hosts, "No hosts could be retrieved"
     assert "id" in hosts[0], "'id' was not returned for the first list item"
+    assert "name" in hosts[0], "'name' was not returned for the first list item"
+    assert "slug" in hosts[0], "'slug' was not returned for the first list item"
+    assert "pronouns" in hosts[0], "'pronouns' was not returned for the first list item"
 
 
 def test_host_retrieve_all_details():
     """Testing for :py:meth:`wwdtm.host.Host.retrieve_all_details`."""
     host = Host(connect_dict=get_connect_dict())
     hosts = host.retrieve_all_details()
 
     assert hosts, "No hosts could be retrieved"
     assert "id" in hosts[0], "'id' was not returned for first list item"
+    assert "name" in hosts[0], "'name' was not returned for the first list item"
+    assert "slug" in hosts[0], "'slug' was not returned for the first list item"
+    assert "pronouns" in hosts[0], "'pronouns' was not returned for the first list item"
     assert (
         "appearances" in hosts[0]
     ), "'appearances' was not returned for thefirst list item"
 
 
 def test_host_retrieve_all_ids():
     """Testing for :py:meth:`wwdtm.host.Host.retrieve_all_ids`."""
@@ -71,27 +77,31 @@
     :param host_id: Host ID to test retrieving host information
     """
     host = Host(connect_dict=get_connect_dict())
     info = host.retrieve_by_id(host_id)
 
     assert info, f"Host ID {host_id} not found"
     assert "name" in info, f"'name' was not returned for ID {host_id}"
+    assert "slug" in info, f"'slug' was not returned for ID {host_id}"
+    assert "pronouns" in info, f"'pronouns' was not returned for ID {host_id}"
 
 
 @pytest.mark.parametrize("host_id", [2])
 def test_host_retrieve_details_by_id(host_id: int):
     """Testing for :py:meth:`wwdtm.host.Host.retrieve_details_by_id`.
 
     :param host_id: Host ID to test retrieving host details
     """
     host = Host(connect_dict=get_connect_dict())
     info = host.retrieve_details_by_id(host_id)
 
     assert info, f"Host ID {host_id} not found"
     assert "name" in info, f"'name' was not returned for ID {host_id}"
+    assert "slug" in info, f"'slug' was not returned for ID {host_id}"
+    assert "pronouns" in info, f"'pronouns' was not returned for ID {host_id}"
     assert "appearances" in info, f"'appearances' was not returned for ID {host_id}"
 
 
 @pytest.mark.parametrize("host_slug", ["luke-burbank"])
 def test_host_retrieve_by_slug(host_slug: str):
     """Testing for :py:meth:`wwdtm.host.Host.retrieve_by_slug`.
 
@@ -99,21 +109,25 @@
         information
     """
     host = Host(connect_dict=get_connect_dict())
     info = host.retrieve_by_slug(host_slug)
 
     assert info, f"Host slug {host_slug} not found"
     assert "name" in info, f"'name' was not returned for slug {host_slug}"
+    assert "slug" in info, f"'slug' was not returned for ID {host_slug}"
+    assert "pronouns" in info, f"'pronouns' was not returned for ID {host_slug}"
 
 
 @pytest.mark.parametrize("host_slug", ["luke-burbank"])
 def test_host_retrieve_details_by_slug(host_slug: str):
     """Testing for :py:meth:`wwdtm.host.Host.retrieve_details_by_slug`.
 
     :param host_slug: Host slug string to test retrieving host details
     """
     host = Host(connect_dict=get_connect_dict())
     info = host.retrieve_details_by_slug(host_slug)
 
     assert info, f"Host slug {host_slug} not found"
     assert "name" in info, f"'name' was not returned for slug {host_slug}"
+    assert "slug" in info, f"'slug' was not returned for ID {host_slug}"
+    assert "pronouns" in info, f"'pronouns' was not returned for ID {host_slug}"
     assert "appearances" in info, f"'appearances' was not returned for slug {host_slug}"
```

### Comparing `wwdtm-2.8.2/tests/host/test_host_utility.py` & `wwdtm-2.9.0/tests/host/test_host_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/location/test_location_location.py` & `wwdtm-2.9.0/tests/location/test_location_location.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,23 +30,25 @@
 def test_location_retrieve_all():
     """Testing for :py:meth:`wwdtm.location.Location.retrieve_all`."""
     location = Location(connect_dict=get_connect_dict())
     locations = location.retrieve_all()
 
     assert locations, "No locations could be retrieved"
     assert "id" in locations[0], "'id' was not returned for the first list item"
+    assert "venue" in locations[0], "'venue' was not returned for the first list item"
 
 
 def test_location_retrieve_all_details():
     """Testing for :py:meth:`wwdtm.location.Location.retrieve_all_details`."""
     location = Location(connect_dict=get_connect_dict())
     locations = location.retrieve_all_details()
 
     assert locations, "No locations could be retrieved"
     assert "id" in locations[0], "'id' was not returned for first list item"
+    assert "venue" in locations[0], "'venue' was not returned for the first list item"
     assert (
         "recordings" in locations[0]
     ), "'recordings' was not returned for the first list item"
 
 
 def test_location_retrieve_all_ids():
     """Testing for :py:meth:`wwdtm.location.Location.retrieve_all_ids`."""
@@ -72,27 +74,31 @@
         information
     """
     location = Location(connect_dict=get_connect_dict())
     info = location.retrieve_by_id(location_id)
 
     assert info, f"Location ID {location_id} not found"
     assert "venue" in info, f"'venue' was not returned for ID {location_id}"
+    assert "latitude" in info, f"'latitude' was not returned for ID {location_id}"
+    assert "longitude" in info, f"'longitude' was not returned for ID {location_id}"
 
 
 @pytest.mark.parametrize("location_id", [95])
 def test_location_retrieve_details_by_id(location_id: int):
     """Testing for :py:meth:`wwdtm.location.location.retrieve_details_by_id`.
 
     :param location_id: Location ID to test retrieving location details
     """
     location = Location(connect_dict=get_connect_dict())
     info = location.retrieve_details_by_id(location_id)
 
     assert info, f"Location ID {location_id} not found"
     assert "venue" in info, f"'venue' was not returned for ID {location_id}"
+    assert "latitude" in info, f"'latitude' was not returned for ID {location_id}"
+    assert "longitude" in info, f"'longitude' was not returned for ID {location_id}"
     assert "recordings" in info, f"'recordings' was not returned for ID {location_id}"
 
 
 @pytest.mark.parametrize("location_slug", ["the-chicago-theatre-chicago-il"])
 def test_location_retrieve_by_slug(location_slug: str):
     """Testing for :py:meth:`wwdtm.location.Location.retrieve_by_slug`.
 
@@ -100,24 +106,28 @@
         location information
     """
     location = Location(connect_dict=get_connect_dict())
     info = location.retrieve_by_slug(location_slug)
 
     assert info, f"Location slug {location_slug} not found"
     assert "venue" in info, f"'venue' was not returned for slug {location_slug}"
+    assert "latitude" in info, f"'latitude' was not returned for ID {location_slug}"
+    assert "longitude" in info, f"'longitude' was not returned for ID {location_slug}"
 
 
 @pytest.mark.parametrize("location_slug", ["the-chicago-theatre-chicago-il"])
 def test_location_retrieve_details_by_slug(location_slug: str):
     """Testing for :py:meth:`wwdtm.location.Location.retrieve_details_by_slug`.
 
     :param location_slug: Location slug string to test retrieving
         location details
     """
     location = Location(connect_dict=get_connect_dict())
     info = location.retrieve_details_by_slug(location_slug)
 
     assert info, f"Location slug {location_slug} not found"
     assert "venue" in info, f"'venue' was not returned for slug {location_slug}"
+    assert "latitude" in info, f"'latitude' was not returned for ID {location_slug}"
+    assert "longitude" in info, f"'longitude' was not returned for ID {location_slug}"
     assert (
         "recordings" in info
     ), f"'recordings' was not returned for slug {location_slug}"
```

### Comparing `wwdtm-2.8.2/tests/location/test_location_recordings.py` & `wwdtm-2.9.0/tests/location/test_location_recordings.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/location/test_location_utility.py` & `wwdtm-2.9.0/tests/location/test_location_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/panelist/test_panelist_appearances.py` & `wwdtm-2.9.0/tests/panelist/test_panelist_appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/panelist/test_panelist_decimal_scores.py` & `wwdtm-2.9.0/tests/panelist/test_panelist_decimal_scores.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/panelist/test_panelist_panelist.py` & `wwdtm-2.9.0/tests/panelist/test_panelist_panelist.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,28 +30,38 @@
 def test_panelist_retrieve_all():
     """Testing for :py:meth:`wwdtm.panelist.Panelist.retrieve_all`."""
     panelist = Panelist(connect_dict=get_connect_dict())
     panelists = panelist.retrieve_all()
 
     assert panelists, "No panelists could be retrieved"
     assert "id" in panelists[0], "'id' was not returned for the first list item"
+    assert "name" in panelists[0], "'name' was not returned for the first list item"
+    assert "slug" in panelists[0], "'slug' was not returned for the first list item"
+    assert (
+        "pronouns" in panelists[0]
+    ), "'pronouns' was not returned for the first list item"
 
 
 @pytest.mark.parametrize("use_decimal_scores", [True, False])
 def test_panelist_retrieve_all_details(use_decimal_scores: bool):
     """Testing for :py:meth:`wwdtm.panelist.Panelist.retrieve_all_details`.
 
     :param use_decimal_scores: Flag set to use decimal score columns
         and values
     """
     panelist = Panelist(connect_dict=get_connect_dict())
     panelists = panelist.retrieve_all_details(use_decimal_scores=use_decimal_scores)
 
     assert panelists, "No panelists could be retrieved"
     assert "id" in panelists[0], "'id' was not returned for first list item"
+    assert "name" in panelists[0], "'name' was not returned for the first list item"
+    assert "slug" in panelists[0], "'slug' was not returned for the first list item"
+    assert (
+        "pronouns" in panelists[0]
+    ), "'pronouns' was not returned for the first list item"
     assert (
         "appearances" in panelists[0]
     ), "'appearances' was not returned for the first list item"
 
 
 def test_panelist_retrieve_all_ids():
     """Testing for :py:meth:`wwdtm.panelist.Panelist.retrieve_all_ids`."""
@@ -77,14 +87,16 @@
         information
     """
     panelist = Panelist(connect_dict=get_connect_dict())
     info = panelist.retrieve_by_id(panelist_id)
 
     assert info, f"Panelist ID {panelist_id} not found"
     assert "name" in info, f"'name' was not returned for ID {panelist_id}"
+    assert "slug" in info, f"'slug' was not returned for ID {panelist_id}"
+    assert "pronouns" in info, f"'pronouns' was not returned for ID {panelist_id}"
 
 
 @pytest.mark.parametrize("panelist_id, use_decimal_scores", [(14, True), (14, False)])
 def test_panelist_retrieve_details_by_id(panelist_id: int, use_decimal_scores: bool):
     """Testing for :py:meth:`wwdtm.panelist.Panelist.retrieve_details_by_id`.
 
     :param panelist_id: Panelist ID to test retrieving panelist details
@@ -94,14 +106,16 @@
     panelist = Panelist(connect_dict=get_connect_dict())
     info = panelist.retrieve_details_by_id(
         panelist_id, use_decimal_scores=use_decimal_scores
     )
 
     assert info, f"Panelist ID {panelist_id} not found"
     assert "name" in info, f"'name' was not returned for ID {panelist_id}"
+    assert "slug" in info, f"'slug' was not returned for ID {panelist_id}"
+    assert "pronouns" in info, f"'pronouns' was not returned for ID {panelist_id}"
     assert "appearances" in info, f"'appearances' was not returned for ID {panelist_id}"
 
 
 @pytest.mark.parametrize("panelist_slug", ["luke-burbank", "drew-carey"])
 def test_panelist_retrieve_by_slug(panelist_slug: str):
     """Testing for :py:meth:`wwdtm.panelist.Panelist.retrieve_by_slug`.
 
@@ -109,14 +123,16 @@
         panelist information
     """
     panelist = Panelist(connect_dict=get_connect_dict())
     info = panelist.retrieve_by_slug(panelist_slug)
 
     assert info, f"Panelist slug {panelist_slug} not found"
     assert "name" in info, f"'name' was not returned for slug {panelist_slug}"
+    assert "slug" in info, f"'slug' was not returned for ID {panelist_slug}"
+    assert "pronouns" in info, f"'pronouns' was not returned for ID {panelist_slug}"
 
 
 @pytest.mark.parametrize(
     "panelist_slug, use_decimal_scores",
     [("luke-burbank", True), ("luke-burbank", False)],
 )
 def test_panelist_retrieve_details_by_slug(
@@ -132,10 +148,12 @@
     panelist = Panelist(connect_dict=get_connect_dict())
     info = panelist.retrieve_details_by_slug(
         panelist_slug, use_decimal_scores=use_decimal_scores
     )
 
     assert info, f"Panelist slug {panelist_slug} not found"
     assert "name" in info, f"'name' was not returned for slug {panelist_slug}"
+    assert "slug" in info, f"'slug' was not returned for ID {panelist_slug}"
+    assert "pronouns" in info, f"'pronouns' was not returned for ID {panelist_slug}"
     assert (
         "appearances" in info
     ), f"'appearances' was not returned for slug {panelist_slug}"
```

### Comparing `wwdtm-2.8.2/tests/panelist/test_panelist_scores.py` & `wwdtm-2.9.0/tests/panelist/test_panelist_scores.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/panelist/test_panelist_statistics.py` & `wwdtm-2.9.0/tests/panelist/test_panelist_statistics.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/panelist/test_panelist_utility.py` & `wwdtm-2.9.0/tests/panelist/test_panelist_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/scorekeeper/test_scorekeeper_appearances.py` & `wwdtm-2.9.0/tests/scorekeeper/test_scorekeeper_appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/scorekeeper/test_scorekeeper_utility.py` & `wwdtm-2.9.0/tests/scorekeeper/test_scorekeeper_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/show/test_show_info.py` & `wwdtm-2.9.0/tests/show/test_show_info.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/show/test_show_info_multiple.py` & `wwdtm-2.9.0/tests/show/test_show_info_multiple.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/show/test_show_show.py` & `wwdtm-2.9.0/tests/show/test_show_show.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/show/test_show_utility.py` & `wwdtm-2.9.0/tests/show/test_show_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/tests/test_validation.py` & `wwdtm-2.9.0/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm/__init__.py` & `wwdtm-2.9.0/wwdtm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     PanelistScores,
     PanelistStatistics,
     PanelistUtility,
 )
 from wwdtm.scorekeeper import Scorekeeper, ScorekeeperAppearances, ScorekeeperUtility
 from wwdtm.show import Show, ShowInfo, ShowInfoMultiple, ShowUtility
 
-VERSION = "2.8.2"
+VERSION = "2.9.0"
```

### Comparing `wwdtm-2.8.2/wwdtm/guest/appearances.py` & `wwdtm-2.9.0/wwdtm/guest/appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm/guest/guest.py` & `wwdtm-2.9.0/wwdtm/guest/guest.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm/guest/utility.py` & `wwdtm-2.9.0/wwdtm/guest/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm/host/appearances.py` & `wwdtm-2.9.0/wwdtm/host/appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm/host/host.py` & `wwdtm-2.9.0/wwdtm/host/host.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,17 +48,18 @@
     def retrieve_all(self) -> list[dict[str, int | str]]:
         """Retrieves host information for all hosts.
 
         :return: A list of dictionaries containing host ID, name, slug
             string and gender for each host
         """
         query = """
-            SELECT hostid AS id, host AS name, hostslug AS slug,
-            hostgender AS gender
-            FROM ww_hosts
+            SELECT h.hostid AS id, h.host AS name, h.hostslug AS slug,
+            hostgender AS gender, pn.pronouns
+            FROM ww_hosts h
+            JOIN ww_pronouns pn ON pn.pronounsid = h.hostpronouns
             ORDER BY host ASC;
             """
         cursor = self.database_connection.cursor(named_tuple=True)
         cursor.execute(query)
         results = cursor.fetchall()
         cursor.close()
 
@@ -69,30 +70,32 @@
         for row in results:
             hosts.append(
                 {
                     "id": row.id,
                     "name": row.name,
                     "slug": row.slug if row.slug else slugify(row.name),
                     "gender": row.gender,
+                    "pronouns": row.pronouns,
                 }
             )
 
         return hosts
 
     def retrieve_all_details(self) -> list[dict[str, Any]]:
         """Retrieves host information and appearances for all hosts.
 
         :return: A list of dictionaries containing host ID, name, slug
             string, gender and a list of appearances with show flags for
             each host
         """
         query = """
-            SELECT hostid AS id, host AS name, hostslug AS slug,
-            hostgender AS gender
-            FROM ww_hosts
+            SELECT h.hostid AS id, h.host AS name, h.hostslug AS slug,
+            h.hostgender AS gender, pn.pronouns
+            FROM ww_hosts h
+            JOIN ww_pronouns pn ON pn.pronounsid = h.hostpronouns
             ORDER BY host ASC;
             """
         cursor = self.database_connection.cursor(named_tuple=True)
         cursor.execute(query)
         results = cursor.fetchall()
         cursor.close()
 
@@ -103,14 +106,15 @@
         for row in results:
             hosts.append(
                 {
                     "id": row.id,
                     "name": row.name,
                     "slug": row.slug if row.slug else slugify(row.name),
                     "gender": row.gender,
+                    "pronouns": row.pronouns,
                     "appearances": self.appearances.retrieve_appearances_by_id(row.id),
                 }
             )
 
         return hosts
 
     def retrieve_all_ids(self) -> list[int]:
@@ -153,18 +157,19 @@
         :param host_id: Host ID
         :return: A dictionary containing host ID, name, gender and slug string
         """
         if not valid_int_id(host_id):
             return {}
 
         query = """
-            SELECT hostid AS id, host AS name, hostslug AS slug,
-            hostgender AS gender
-            FROM ww_hosts
-            WHERE hostid = %s
+            SELECT h.hostid AS id, h.host AS name, h.hostslug AS slug,
+            h.hostgender AS gender, pn.pronouns
+            FROM ww_hosts h
+            JOIN ww_pronouns pn on pn.pronounsid = h.hostpronouns
+            WHERE h.hostid = %s
             LIMIT 1;
             """
         cursor = self.database_connection.cursor(named_tuple=True)
         cursor.execute(query, (host_id,))
         result = cursor.fetchone()
         cursor.close()
 
@@ -172,14 +177,15 @@
             return {}
 
         return {
             "id": result.id,
             "name": result.name,
             "slug": result.slug if result.slug else slugify(result.name),
             "gender": result.gender,
+            "pronouns": result.pronouns,
         }
 
     def retrieve_by_slug(self, host_slug: str) -> dict[str, Any]:
         """Retrieves host information.
 
         :param host_slug: Host slug string
         :return: A dictionary containing host ID, name, gender and slug
```

### Comparing `wwdtm-2.8.2/wwdtm/host/utility.py` & `wwdtm-2.9.0/wwdtm/host/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm/location/location.py` & `wwdtm-2.9.0/wwdtm/location/location.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,16 +51,16 @@
 
         :param sort_by_venue: A boolean to determine if the returned
             list is sorted by venue first or by state and city first
         :return: A list of dictionaries containing location ID, venue
             name, city, state and slug string
         """
         query = """
-            SELECT locationid AS id, city, state, venue,
-            locationslug AS slug
+            SELECT locationid AS id, city, state, venue, latitude,
+            longitude, locationslug AS slug
             FROM ww_locations
             """
 
         if sort_by_venue:
             query = query + "ORDER BY venue ASC, city ASC, state ASC;"
         else:
             query = query + "ORDER BY state ASC, city ASC, venue ASC;"
@@ -77,14 +77,16 @@
         for row in results:
             locations.append(
                 {
                     "id": row.id,
                     "city": row.city,
                     "state": row.state,
                     "venue": row.venue,
+                    "latitude": row.latitude if row.latitude else None,
+                    "longitude": row.longitude if row.longitude else None,
                     "slug": (
                         row.slug
                         if row.slug
                         else self.utility.slugify_location(
                             location_id=row.id,
                             venue=row.venue,
                             city=row.city,
@@ -101,16 +103,16 @@
 
         :param sort_by_venue: A boolean to determine if the returned
             list is sorted by venue first or by state and city first
         :return: A list of dictionaries containing location ID, venue
             name, city, state, slug string and a list of recordings
         """
         query = """
-            SELECT locationid AS id, city, state, venue,
-            locationslug AS slug
+            SELECT locationid AS id, city, state, venue, latitude,
+            longitude, locationslug AS slug
             FROM ww_locations
             """
         if sort_by_venue:
             query = query + "ORDER BY venue ASC, city ASC, state ASC;"
         else:
             query = query + "ORDER BY state ASC, city ASC, venue ASC;"
 
@@ -126,14 +128,16 @@
         for row in results:
             locations.append(
                 {
                     "id": row.id,
                     "city": row.city,
                     "state": row.state,
                     "venue": row.venue,
+                    "latitude": row.latitude if row.latitude else None,
+                    "longitude": row.longitude if row.longitude else None,
                     "slug": (
                         row.slug
                         if row.slug
                         else self.utility.slugify_location(
                             location_id=row.id,
                             venue=row.venue,
                             city=row.city,
@@ -199,16 +203,16 @@
         :return: A dictionary containing location ID, venue, city, state
             and slug string
         """
         if not valid_int_id(location_id):
             return {}
 
         query = """
-            SELECT locationid AS id, city, state, venue,
-            locationslug AS slug
+            SELECT locationid AS id, city, state, venue, latitude,
+            longitude, locationslug AS slug
             FROM ww_locations
             WHERE locationid = %s
             LIMIT 1;
             """
         cursor = self.database_connection.cursor(named_tuple=True)
         cursor.execute(query, (location_id,))
         result = cursor.fetchone()
@@ -218,14 +222,16 @@
             return {}
 
         return {
             "id": result.id,
             "city": result.city,
             "state": result.state,
             "venue": result.venue,
+            "latitude": result.latitude if result.latitude else None,
+            "longitude": result.longitude if result.longitude else None,
             "slug": (
                 result.slug
                 if result.slug
                 else self.utility.slugify_location(
                     location_id=result.id,
                     venue=result.venue,
                     city=result.city,
```

### Comparing `wwdtm-2.8.2/wwdtm/location/recordings.py` & `wwdtm-2.9.0/wwdtm/location/recordings.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm/location/utility.py` & `wwdtm-2.9.0/wwdtm/location/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm/panelist/appearances.py` & `wwdtm-2.9.0/wwdtm/panelist/appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm/panelist/decimal_scores.py` & `wwdtm-2.9.0/wwdtm/panelist/decimal_scores.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm/panelist/panelist.py` & `wwdtm-2.9.0/wwdtm/panelist/panelist.py`

 * *Files 15% similar despite different names*

```diff
@@ -54,17 +54,18 @@
     def retrieve_all(self) -> list[dict[str, Any]]:
         """Retrieve panelist information for all panelists.
 
         :return: A list of dictionaries containing panelist ID, name,
             slug string and gender for each panelist
         """
         query = """
-            SELECT panelistid AS id, panelist AS name, panelistslug AS slug,
-            panelistgender AS gender
-            FROM ww_panelists
+            SELECT p.panelistid AS id, p.panelist AS name, p.panelistslug AS slug,
+            panelistgender AS gender, pn.pronouns
+            FROM ww_panelists p
+            JOIN ww_pronouns pn ON pn.pronounsid = p.panelistpronouns
             WHERE panelistslug != 'multiple'
             ORDER BY panelist ASC;
             """
         cursor = self.database_connection.cursor(named_tuple=True)
         cursor.execute(query)
         results = cursor.fetchall()
         cursor.close()
@@ -76,14 +77,15 @@
         for row in results:
             panelists.append(
                 {
                     "id": row.id,
                     "name": row.name,
                     "slug": row.slug if row.slug else slugify(row.name),
                     "gender": row.gender,
+                    "pronouns": row.pronouns,
                 }
             )
 
         return panelists
 
     def retrieve_all_details(
         self, use_decimal_scores: bool = False
@@ -93,17 +95,18 @@
         :param use_decimal_scores: A boolean to determine if decimal
             scores should be used and returned instead of integer scores
         :return: A list of dictionaries containing panelist ID, name,
             slug string, gender, scoring statistics and appearances for
             each panelist
         """
         query = """
-            SELECT panelistid AS id, panelist AS name, panelistslug AS slug,
-            panelistgender AS gender
-            FROM ww_panelists
+            SELECT p.panelistid AS id, p.panelist AS name, p.panelistslug AS slug,
+            p.panelistgender AS gender, pn.pronouns
+            FROM ww_panelists p
+            JOIN ww_pronouns pn ON pn.pronounsid = p.panelistpronouns
             WHERE panelistslug != 'multiple'
             ORDER BY panelist ASC;
             """
         cursor = self.database_connection.cursor(named_tuple=True)
         cursor.execute(query)
         results = cursor.fetchall()
         cursor.close()
@@ -115,14 +118,15 @@
         for row in results:
             panelists.append(
                 {
                     "id": row.id,
                     "name": row.name,
                     "slug": row.slug if row.slug else slugify(row.name),
                     "gender": row.gender,
+                    "pronouns": row.pronouns,
                     "statistics": self.statistics.retrieve_statistics_by_id(
                         row.id, include_decimal_scores=use_decimal_scores
                     ),
                     "bluffs": self.statistics.retrieve_bluffs_by_id(row.id),
                     "appearances": self.appearances.retrieve_appearances_by_id(
                         row.id, use_decimal_scores=use_decimal_scores
                     ),
@@ -178,18 +182,19 @@
         :return: A dictionary containing panelist ID, name, slug string
             and gender
         """
         if not valid_int_id(panelist_id):
             return {}
 
         query = """
-            SELECT panelistid AS id, panelist AS name, panelistslug AS slug,
-            panelistgender AS gender
-            FROM ww_panelists
-            WHERE panelistid = %s
+            SELECT p.panelistid AS id, p.panelist AS name, p.panelistslug AS slug,
+            p.panelistgender AS gender, pn.pronouns
+            FROM ww_panelists p
+            JOIN ww_pronouns pn ON pn.pronounsid = p.panelistpronouns
+            WHERE p.panelistid = %s
             LIMIT 1;
             """
         cursor = self.database_connection.cursor(named_tuple=True)
         cursor.execute(query, (panelist_id,))
         result = cursor.fetchone()
         cursor.close()
 
@@ -197,14 +202,15 @@
             return {}
 
         return {
             "id": result.id,
             "name": result.name,
             "slug": result.slug if result.slug else slugify(result.name),
             "gender": result.gender,
+            "pronouns": result.pronouns,
         }
 
     def retrieve_by_slug(self, panelist_slug: str) -> dict[str, Any]:
         """Retrieves panelist information.
 
         :param panelist_slug: Panelist slug string
         :return: A dictionary containing panelist ID, name, slug string
```

### Comparing `wwdtm-2.8.2/wwdtm/panelist/scores.py` & `wwdtm-2.9.0/wwdtm/panelist/scores.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm/panelist/statistics.py` & `wwdtm-2.9.0/wwdtm/panelist/statistics.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm/panelist/utility.py` & `wwdtm-2.9.0/wwdtm/panelist/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm/scorekeeper/appearances.py` & `wwdtm-2.9.0/wwdtm/scorekeeper/appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm/scorekeeper/utility.py` & `wwdtm-2.9.0/wwdtm/scorekeeper/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm/show/info.py` & `wwdtm-2.9.0/wwdtm/show/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,19 +178,19 @@
         if not valid_int_id(show_id):
             return {}
 
         query = """
             SELECT s.showid AS show_id, s.showdate AS date,
             s.bestof AS best_of, s.repeatshowid AS repeat_show_id,
             s.showurl AS show_url,
-            l.locationid AS location_id, l.city, l.state,
-            l.venue, l.locationslug AS location_slug, h.hostid AS host_id,
-            h.host, h.hostslug AS host_slug, hm.guest as host_guest,
-            sk.scorekeeperid AS scorekeeper_id, sk.scorekeeper,
-            sk.scorekeeperslug AS scorekeeper_slug,
+            l.locationid AS location_id, l.city, l.state, l.latitude,
+            l.longitude, l.venue, l.locationslug AS location_slug,
+            h.hostid AS host_id, h.host, h.hostslug AS host_slug,
+            hm.guest as host_guest, sk.scorekeeperid AS scorekeeper_id,
+            sk.scorekeeper, sk.scorekeeperslug AS scorekeeper_slug,
             skm.guest AS scorekeeper_guest,
             skm.description AS scorekeeper_description,
             sd.showdescription AS show_description,
             sn.shownotes AS show_notes
             FROM ww_shows s
             JOIN ww_showlocationmap lm ON lm.showid = s.showid
             JOIN ww_locations l ON l.locationid = lm.locationid
@@ -213,14 +213,16 @@
 
         location_info = {
             "id": result.location_id,
             "slug": result.location_slug,
             "city": result.city,
             "state": result.state,
             "venue": result.venue,
+            "latitude": result.latitude if result.latitude else None,
+            "longitude": result.longitude if result.longitude else None,
         }
 
         if not result.location_slug:
             location_info["slug"] = self.loc_util.slugify_location(
                 location_id=result.location_id,
                 venue=result.venue,
                 city=result.city,
```

### Comparing `wwdtm-2.8.2/wwdtm/show/info_multiple.py` & `wwdtm-2.9.0/wwdtm/show/info_multiple.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,16 +277,17 @@
             description and notes
         """
         query = """
             SELECT s.showid AS show_id, s.showdate AS date,
             s.bestof AS best_of, s.repeatshowid AS repeat_show_id,
             s.showurl AS show_url,
             l.locationid AS location_id, l.city, l.state,
-            l.venue, l.locationslug AS location_slug, h.hostid AS host_id,
-            h.host, h.hostslug AS host_slug, hm.guest as host_guest,
+            l.venue, l.latitude, l.longitude, l.locationslug AS location_slug,
+            h.hostid AS host_id, h.host, h.hostslug AS host_slug,
+            hm.guest as host_guest,
             sk.scorekeeperid AS scorekeeper_id, sk.scorekeeper,
             sk.scorekeeperslug AS scorekeeper_slug,
             skm.guest AS scorekeeper_guest,
             skm.description AS scorekeeper_description,
             sd.showdescription AS show_description,
             sn.shownotes AS show_notes
             FROM ww_shows s
@@ -312,14 +313,16 @@
         for show in results:
             location_info = {
                 "id": show.location_id,
                 "slug": show.location_slug,
                 "city": show.city,
                 "state": show.state,
                 "venue": show.venue,
+                "latitude": show.latitude if show.latitude else None,
+                "longitude": show.longitude if show.longitude else None,
             }
 
             if not show.location_slug:
                 location_info["slug"] = self.loc_util.slugify_location(
                     location_id=show.location_id,
                     venue=show.venue,
                     city=show.city,
@@ -398,16 +401,17 @@
                 return {}
 
         query = """
             SELECT s.showid AS show_id, s.showdate AS date,
             s.bestof AS best_of, s.repeatshowid AS repeat_show_id,
             s.showurl AS show_url,
             l.locationid AS location_id, l.city, l.state,
-            l.venue, l.locationslug AS location_slug, h.hostid AS host_id,
-            h.host, h.hostslug AS host_slug, hm.guest as host_guest,
+            l.venue, l.latitude, l.longitude, l.locationslug AS location_slug,
+            h.hostid AS host_id, h.host, h.hostslug AS host_slug,
+            hm.guest as host_guest,
             sk.scorekeeperid AS scorekeeper_id, sk.scorekeeper,
             sk.scorekeeperslug AS scorekeeper_slug,
             skm.guest AS scorekeeper_guest,
             skm.description AS scorekeeper_description,
             sd.showdescription AS show_description,
             sn.shownotes AS show_notes
             FROM ww_shows s
@@ -435,14 +439,16 @@
         for show in results:
             location_info = {
                 "id": show.location_id,
                 "slug": show.location_slug,
                 "city": show.city,
                 "state": show.state,
                 "venue": show.venue,
+                "latitude": show.latitude if show.latitude else None,
+                "longitude": show.longitude if show.longitude else None,
             }
 
             if not show.location_slug:
                 location_info["slug"] = self.loc_util.slugify_location(
                     location_id=show.location_id,
                     venue=show.venue,
                     city=show.city,
```

### Comparing `wwdtm-2.8.2/wwdtm/show/show.py` & `wwdtm-2.9.0/wwdtm/show/show.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm/show/utility.py` & `wwdtm-2.9.0/wwdtm/show/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm/validation.py` & `wwdtm-2.9.0/wwdtm/validation.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.8.2/wwdtm.egg-info/PKG-INFO` & `wwdtm-2.9.0/wwdtm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwdtm
-Version: 2.8.2
+Version: 2.9.0
 Summary: Library used to query data from copy of Wait Wait Stats Database.
 Author-email: Linh Pham <dev@wwdt.me>
 License: Apache-2.0
 Project-URL: Documentation, https://docs.wwdt.me
 Project-URL: Source Code, https://github.com/questionlp/wwdtm
 Project-URL: Changes, https://docs.wwdt.me/latest/changes/
 Project-URL: Stats Page, https://stats.wwdt.me
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: mysql-connector-python==8.2.0
-Requires-Dist: numpy==1.26.3
+Requires-Dist: numpy==1.26.4
 Requires-Dist: python-slugify==8.0.1
-Requires-Dist: pytz==2023.3.post1
+Requires-Dist: pytz==2024.1
 
 ***********************
 Wait Wait Stats Library
 ***********************
 
 Overview
 ========
```

### Comparing `wwdtm-2.8.2/wwdtm.egg-info/SOURCES.txt` & `wwdtm-2.9.0/wwdtm.egg-info/SOURCES.txt`

 * *Files identical despite different names*


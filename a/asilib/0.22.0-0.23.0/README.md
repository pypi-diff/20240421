# Comparing `tmp/asilib-0.22.0.tar.gz` & `tmp/asilib-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asilib-0.22.0.tar", last modified: Mon Mar 11 20:48:27 2024, max compression
+gzip compressed data, was "asilib-0.23.0.tar", last modified: Sun Apr 21 15:40:48 2024, max compression
```

## Comparing `asilib-0.22.0.tar` & `asilib-0.23.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:48:27.278529 asilib-0.22.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-11 20:48:18.000000 asilib-0.22.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-11 20:48:18.000000 asilib-0.22.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-03-11 20:48:27.278529 asilib-0.22.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-03-11 20:48:18.000000 asilib-0.22.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:48:27.266528 asilib-0.22.0/asilib/
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:48:27.266528 asilib-0.22.0/asilib/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/analysis/equal_area.py
--rw-r--r--   0 runner    (1001) docker     (127)    15840 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/analysis/keogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/analysis/map.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/analysis/start_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:48:27.266528 asilib-0.22.0/asilib/asi/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/asi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9357 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/asi/fake_asi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/asi/lamp_phantom.py
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/asi/psa_emccd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13551 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/asi/rego.py
--rw-r--r--   0 runner    (1001) docker     (127)    18554 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/asi/themis.py
--rw-r--r--   0 runner    (1001) docker     (127)    32392 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/asi/trex.py
--rw-r--r--   0 runner    (1001) docker     (127)    25000 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/conjunction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:48:27.270528 asilib-0.22.0/asilib/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/data/asi_locations.csv
--rw-r--r--   0 runner    (1001) docker     (127)  3269070 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/data/ne_10m_land.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:48:27.274528 asilib-0.22.0/asilib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/imager.py
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/imagers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:48:27.274528 asilib-0.22.0/asilib/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20141 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/io/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    22349 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/io/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14760 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:48:27.274528 asilib-0.22.0/asilib/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/plot/animate_fisheye.py
--rw-r--r--   0 runner    (1001) docker     (127)    13675 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/plot/animate_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/plot/plot_fisheye.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/plot/plot_keogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    13313 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/plot/plot_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/skymap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:48:27.274528 asilib-0.22.0/asilib/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/tests/mock_footprint.py
--rw-r--r--   0 runner    (1001) docker     (127)    23823 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/tests/test_conjunction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/tests/test_imager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/tests/test_imagers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/tests/test_rego.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/tests/test_skymap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/tests/test_themis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/tests/test_trex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-03-11 20:48:18.000000 asilib-0.22.0/asilib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:48:27.274528 asilib-0.22.0/asilib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-03-11 20:48:27.000000 asilib-0.22.0/asilib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-11 20:48:27.000000 asilib-0.22.0/asilib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 20:48:27.000000 asilib-0.22.0/asilib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-11 20:48:27.000000 asilib-0.22.0/asilib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-11 20:48:27.000000 asilib-0.22.0/asilib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-11 20:48:18.000000 asilib-0.22.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 20:48:27.278529 asilib-0.22.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-11 20:48:18.000000 asilib-0.22.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:40:48.782904 asilib-0.23.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 15:40:40.000000 asilib-0.23.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-21 15:40:40.000000 asilib-0.23.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-21 15:40:48.782904 asilib-0.23.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-21 15:40:40.000000 asilib-0.23.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:40:48.770904 asilib-0.23.0/asilib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:40:48.770904 asilib-0.23.0/asilib/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/analysis/equal_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15840 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/analysis/keogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/analysis/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/analysis/start_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:40:48.770904 asilib-0.23.0/asilib/asi/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/asi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9357 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/asi/fake_asi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/asi/lamp_phantom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/asi/psa_emccd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13551 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/asi/rego.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19196 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/asi/themis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32392 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/asi/trex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25000 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/conjunction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:40:48.770904 asilib-0.23.0/asilib/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/data/asi_locations.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  3269070 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/data/ne_10m_land.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:40:48.778904 asilib-0.23.0/asilib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81906 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/imager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28719 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/imagers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:40:48.778904 asilib-0.23.0/asilib/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/io/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22349 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/io/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14810 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:40:48.778904 asilib-0.23.0/asilib/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/plot/animate_fisheye.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13675 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/plot/animate_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/plot/plot_fisheye.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/plot/plot_keogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13313 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/plot/plot_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/skymap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:40:48.782904 asilib-0.23.0/asilib/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/tests/mock_footprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23823 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/tests/test_conjunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11384 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/tests/test_imager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/tests/test_imagers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/tests/test_rego.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/tests/test_skymap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/tests/test_themis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/tests/test_trex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-21 15:40:40.000000 asilib-0.23.0/asilib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:40:48.782904 asilib-0.23.0/asilib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-21 15:40:48.000000 asilib-0.23.0/asilib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-21 15:40:48.000000 asilib-0.23.0/asilib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 15:40:48.000000 asilib-0.23.0/asilib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-21 15:40:48.000000 asilib-0.23.0/asilib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 15:40:48.000000 asilib-0.23.0/asilib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-21 15:40:40.000000 asilib-0.23.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 15:40:48.782904 asilib-0.23.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-21 15:40:40.000000 asilib-0.23.0/setup.py
```

### Comparing `asilib-0.22.0/LICENSE` & `asilib-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/PKG-INFO` & `asilib-0.23.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asilib
-Version: 0.22.0
+Version: 0.23.0
 Summary: An open source package providing data access and analysis tools for the world's all-sky imager (ASI) data.
 Author-email: Mykhaylo Shumko <msshumko@gmail.com>
 Project-URL: Homepage, https://aurora-asi-lib.readthedocs.io/
 Project-URL: Documentation, https://aurora-asi-lib.readthedocs.io/
 Project-URL: Source, https://github.com/mshumko/asilib
 Project-URL: Issues, https://github.com/mshumko/asilib/issues
 Project-URL: Changelog, https://github.com/mshumko/asilib/blob/main/CHANGELOG.md
@@ -35,14 +35,19 @@
 Requires-Dist: opencv-python<5.0,>=4.8.0
 
 ![Test python package](https://github.com/mshumko/asilib/workflows/Test%20python%20package/badge.svg) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4746447.svg)](https://doi.org/10.5281/zenodo.4746446)
 
 # asilib
 asilib is an open source package providing data access and analysis tools for the world's all-sky imager (ASI) data.
 
+> [!NOTE]  
+> The asilib code on PyPI moved from [aurora-asi-lib](https://pypi.org/project/aurora-asi-lib/) to [asilib](https://pypi.org/project/asilib/). To update to version >=0.22.0, run
+> 1. `python3 -m pip uninstall aurora-asi-lib` and
+> 2. `python3 -m pip install asilib`.
+
 The purpose of this project is to combine data from numerous observational ASI arrays into a single unified framework and is thus not associated with the development and operations of all sky cameras, or the curation of ASI datasets. All data is publicly available and is provided as-is. Please give appropriate credit and coordinate with instrument teams with regards to data issues and/or interpretation. See the [Acknowledgements](https://aurora-asi-lib.readthedocs.io/en/latest/index.html#acknowledgements) section for more information. Currently the supported camera systems (arrays) are: 
 * [Red-line Emission Geospace Observatory (REGO)](https://aurora-asi-lib.readthedocs.io/en/latest/imager_api.html#rego-asi)
 * [Time History of Events and Macroscale Interactions during Substorms (THEMIS)](https://aurora-asi-lib.readthedocs.io/en/latest/imager_api.html#module-asilib.asi.themis)
 * [Transition Region Explorer (TREx)](https://aurora-asi-lib.readthedocs.io/en/latest/imager_api.html#module-asilib.asi.trex)
 
 [Documentation](https://aurora-asi-lib.readthedocs.io/) | [Code on GitHub](https://github.com/mshumko/asilib) | [PyPI archive](https://pypi.org/project/asilib/) | [Zenodo archive](https://doi.org/10.5281/zenodo.4746446)
```

### Comparing `asilib-0.22.0/README.md` & `asilib-0.23.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 ![Test python package](https://github.com/mshumko/asilib/workflows/Test%20python%20package/badge.svg) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4746447.svg)](https://doi.org/10.5281/zenodo.4746446)
 
 # asilib
 asilib is an open source package providing data access and analysis tools for the world's all-sky imager (ASI) data.
 
+> [!NOTE]  
+> The asilib code on PyPI moved from [aurora-asi-lib](https://pypi.org/project/aurora-asi-lib/) to [asilib](https://pypi.org/project/asilib/). To update to version >=0.22.0, run
+> 1. `python3 -m pip uninstall aurora-asi-lib` and
+> 2. `python3 -m pip install asilib`.
+
 The purpose of this project is to combine data from numerous observational ASI arrays into a single unified framework and is thus not associated with the development and operations of all sky cameras, or the curation of ASI datasets. All data is publicly available and is provided as-is. Please give appropriate credit and coordinate with instrument teams with regards to data issues and/or interpretation. See the [Acknowledgements](https://aurora-asi-lib.readthedocs.io/en/latest/index.html#acknowledgements) section for more information. Currently the supported camera systems (arrays) are: 
 * [Red-line Emission Geospace Observatory (REGO)](https://aurora-asi-lib.readthedocs.io/en/latest/imager_api.html#rego-asi)
 * [Time History of Events and Macroscale Interactions during Substorms (THEMIS)](https://aurora-asi-lib.readthedocs.io/en/latest/imager_api.html#module-asilib.asi.themis)
 * [Transition Region Explorer (TREx)](https://aurora-asi-lib.readthedocs.io/en/latest/imager_api.html#module-asilib.asi.trex)
 
 [Documentation](https://aurora-asi-lib.readthedocs.io/) | [Code on GitHub](https://github.com/mshumko/asilib) | [PyPI archive](https://pypi.org/project/asilib/) | [Zenodo archive](https://doi.org/10.5281/zenodo.4746446)
```

### Comparing `asilib-0.22.0/asilib/__init__.py` & `asilib-0.23.0/asilib/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pathlib
 import configparser
 
-__version__ = '0.22.0'
+__version__ = '0.23.0'
 
 # Load the configuration settings.
 HERE = pathlib.Path(__file__).parent.resolve()
 settings = configparser.ConfigParser()
 settings.read(HERE / 'config.ini')
 
 try:
```

### Comparing `asilib-0.22.0/asilib/__main__.py` & `asilib-0.23.0/asilib/__main__.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/analysis/equal_area.py` & `asilib-0.23.0/asilib/analysis/equal_area.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/analysis/keogram.py` & `asilib-0.23.0/asilib/analysis/keogram.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/analysis/map.py` & `asilib-0.23.0/asilib/analysis/map.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/asi/__init__.py` & `asilib-0.23.0/asilib/asi/__init__.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/asi/fake_asi.py` & `asilib-0.23.0/asilib/asi/fake_asi.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/asi/lamp_phantom.py` & `asilib-0.23.0/asilib/asi/lamp_phantom.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/asi/psa_emccd.py` & `asilib-0.23.0/asilib/asi/psa_emccd.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/asi/rego.py` & `asilib-0.23.0/asilib/asi/rego.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/asi/themis.py` & `asilib-0.23.0/asilib/asi/themis.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import os
 import dateutil.parser
 from typing import Tuple, Iterable, List, Union
 
 import numpy as np
 import pandas as pd
 import scipy.io
+import requests
 import themis_imager_readfile
 
 import asilib
 import asilib.utils as utils
 import asilib.io.download as download
 import asilib.skymap
 
@@ -348,21 +349,33 @@
                 else:
                     try:
                         file_paths.append(
                             _download_one_pgm_file(
                                 array, location_code, file_time, base_url, save_dir, redownload
                             )
                         )
-                    except (FileNotFoundError, AssertionError) as err:
+                    except (FileNotFoundError, AssertionError, requests.exceptions.HTTPError) as err:
                         if missing_ok and (
-                            ('does not contain any hyper references containing' in str(err))
-                            or ('Only one href is allowed' in str(err))
+                            ('does not contain any hyper references containing' in str(err)) or
+                            ('Only one href is allowed' in str(err)) or
+                            ('404 Client Error: Not Found for url:' in str(err))
                         ):
                             continue
                         raise
+            if missing_ok and len(file_paths) == 0:
+                if time_range is not None:
+                    warnings.warn(
+                        f'No local or online image files found for {array}-{location_code} '
+                        f'for {time_range=}.'
+                        )
+                else:
+                    warnings.warn(
+                        f'No local or online image files found for {array}-{location_code} '
+                        f'for {time=}.'
+                        )
             return file_paths
 
 
 def _download_one_pgm_file(
     array: str,
     location_code: str,
     time: datetime,
```

### Comparing `asilib-0.22.0/asilib/asi/trex.py` & `asilib-0.23.0/asilib/asi/trex.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/conjunction.py` & `asilib-0.23.0/asilib/conjunction.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/data/asi_locations.csv` & `asilib-0.23.0/asilib/data/asi_locations.csv`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/data/ne_10m_land.zip` & `asilib-0.23.0/asilib/data/ne_10m_land.zip`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/imager.py` & `asilib-0.23.0/asilib/imager.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,16 +177,16 @@
             self._add_azel_contours(ax, color=azel_contour_color)
         if cardinal_directions is not None:
             self._add_cardinal_directions(ax, cardinal_directions, origin=origin)
         return ax, im
 
     def animate_fisheye(self, **kwargs) -> None:
         """
-        A wrapper for the ```animate_fisheye_gen()``` method that animates a series of
-        fisheye images. Any kwargs are passed directly into ```animate_fisheye_gen()```.
+        A wrapper for the ```Imager.animate_fisheye_gen()``` method that animates a series of
+        fisheye images. Any kwargs are passed directly into ```Imager.animate_fisheye_gen()```.
 
         Parameters
         ----------
         ax: plt.Axes
             The optional subplot that will be drawn on.
         label: bool
             Flag to add the "asi_array_code/location_code/image_time" text to the plot.
```

### Comparing `asilib-0.22.0/asilib/io/download.py` & `asilib-0.23.0/asilib/io/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -399,43 +399,30 @@
         asilib.config['ASI_DATA_DIR'], asi_array_code.lower(), file_names[0]
     )
     if redownload or (not download_path.is_file()):
         utils._stream_large_file(server_url, download_path)
     return download_path
 
 
-# TODO: When cleaning up imager, remove all above
+# TODO: When cleaning up Imager, remove all above
 class Downloader:
     """
     Traverses and lists the directory structure on a server and download files.
 
     Parameters
     ----------
     url: str
         The dataset URL. If it points to a folder it must end with a "/".
     download_dir: str or pathlib.Path
         The download directory. Must either specify here, or when you call
         Downloader.download().
 
     Example
     -------
-    | # List all of the SAMPEX-HILT State4 files and download the first one.
-    |
-    | import sampex
-    |
-    | d = sampex.Downloader(
-    |     'https://izw1.caltech.edu/sampex/DataCenter/DATA/HILThires/State4/',
-    |     download_dir=sampex.config['data_dir']
-    | )
-    | paths = d.ls(match='*.txt*')
-    | print(f"The downloaded files are: {paths}")
-    |
-    | print(f"The first file's name is: {paths[0].name} at url {paths[0].url}")
-    | path = paths[0].download(stream=False)
-    | print(f'The file was downloaded to {path}')
+    TODO: Add an example.
     """
 
     def __init__(self, url: str, download_dir=None) -> None:
         self.url = url
         self.download_dir = download_dir
         return
 
@@ -496,15 +483,16 @@
         file_name = pathlib.Path(self.url).name
         download_path = self.download_dir / file_name
 
         if (download_path.exists()) and (not redownload):
             return download_path
 
         if stream:
-            r = requests.get(self.url, stream=True, timeout=5)
+            with requests.Session() as s:
+                r = s.get(self.url, stream=True, timeout=5)
             r.raise_for_status()
             file_size = int(r.headers.get('content-length'))
             downloaded_bites = 0
 
             megabyte = 1024 * 1024
             try:
                 with open(download_path, 'wb') as f:
@@ -563,15 +551,16 @@
             A list of hyper references that matched the match string.
 
         Raises
         ------
         FileNotFoundError
             If no hyper references were found.
         """
-        request = requests.get(url, timeout=5)
+        with requests.Session() as s:
+            request = s.get(url, timeout=5)
         request.raise_for_status()
         soup = BeautifulSoup(request.content, 'html.parser')
 
         match = match.replace('*', '.*')  # regex wildcard
         href_objs = soup.find_all('a', href=re.compile(match))
         # I found "?" to be in the column names so we should ignore them.
         matched_hrefs = [
```

### Comparing `asilib-0.22.0/asilib/io/load.py` & `asilib-0.23.0/asilib/io/load.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/io/utils.py` & `asilib-0.23.0/asilib/io/utils.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/map.py` & `asilib-0.23.0/asilib/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,14 +159,16 @@
             lon_bounds=lon_bounds,
             lat_bounds=lat_bounds,
             fig_ax=fig_ax,
             coast_color=coast_color,
             land_color=land_color,
             ocean_color=ocean_color,
         )
+    if fig_ax is None:
+        plt.tight_layout()
     return ax
 
 
 def create_simple_map(
     lon_bounds: tuple = (-140, -60),
     lat_bounds: tuple = (40, 82),
     fig_ax: Tuple[matplotlib.figure.Figure, int] = None,
```

### Comparing `asilib-0.22.0/asilib/plot/animate_fisheye.py` & `asilib-0.23.0/asilib/plot/animate_fisheye.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/plot/animate_map.py` & `asilib-0.23.0/asilib/plot/animate_map.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/plot/plot_fisheye.py` & `asilib-0.23.0/asilib/plot/plot_fisheye.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/plot/plot_keogram.py` & `asilib-0.23.0/asilib/plot/plot_keogram.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/plot/plot_map.py` & `asilib-0.23.0/asilib/plot/plot_map.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/plot/utils.py` & `asilib-0.23.0/asilib/plot/utils.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/skymap.py` & `asilib-0.23.0/asilib/skymap.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/tests/mock_footprint.py` & `asilib-0.23.0/asilib/tests/mock_footprint.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/tests/test_conjunction.py` & `asilib-0.23.0/asilib/tests/test_conjunction.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/tests/test_downloader.py` & `asilib-0.23.0/asilib/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/tests/test_imager.py` & `asilib-0.23.0/asilib/tests/test_imager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from datetime import datetime
 
 import pytest
 import numpy as np
 import matplotlib.testing.decorators
 
 import asilib
+import asilib.asi
 from asilib.asi.fake_asi import fake_asi
 
 
 ##########################################
 ########## TEST DATA ACCESS ##############
 ##########################################
 def test_time():
```

### Comparing `asilib-0.22.0/asilib/tests/test_map.py` & `asilib-0.23.0/asilib/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/tests/test_rego.py` & `asilib-0.23.0/asilib/tests/test_rego.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/tests/test_skymap.py` & `asilib-0.23.0/asilib/tests/test_skymap.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/tests/test_themis.py` & `asilib-0.23.0/asilib/tests/test_themis.py`

 * *Files 16% similar despite different names*

```diff
@@ -120,14 +120,35 @@
 
     asi = asilib.asi.themis('RANK', time=datetime(2017, 9, 15, 2, 34, 0))
     ax, im = asi.plot_fisheye(cardinal_directions='NE', origin=(0.95, 0.05))
     plt.colorbar(im)
     ax.axis('off')
     return
 
+def test_themis_download_bug_fix():
+    """
+    Test a bug if an imager does not have data for that hour, and that if missing_ok is set,
+    the Imager.keogram() raises a ValueError.
+    """
+    location_code = 'KAPU'
+    time_range = (datetime(2013, 3, 17, 11), datetime(2013, 3, 17, 11, 1))
+
+    with pytest.warns(UserWarning) as warninfo:
+        asi = asilib.asi.themis(location_code, time_range=time_range)
+
+    with pytest.raises(ValueError) as excinfo:
+        asi.plot_keogram()
+    
+    # check that only one warning was raised
+    assert len(warninfo) == 1
+    # check that the message matches
+    assert 'No local or online image files found' in warninfo[0].message.args[0]
+    assert 'The keogram is empty' in str(excinfo.value)
+    return
+
 
 @matplotlib.testing.decorators.image_comparison(
     baseline_images=['test_themis_map'], tol=10, remove_text=True, extensions=['png']
 )
 def test_themis_map():
     """
     Plot a fisheye lens image on a map.
```

### Comparing `asilib-0.22.0/asilib/tests/test_trex.py` & `asilib-0.23.0/asilib/tests/test_trex.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/tests/test_utils.py` & `asilib-0.23.0/asilib/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib/utils.py` & `asilib-0.23.0/asilib/utils.py`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/asilib.egg-info/PKG-INFO` & `asilib-0.23.0/asilib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asilib
-Version: 0.22.0
+Version: 0.23.0
 Summary: An open source package providing data access and analysis tools for the world's all-sky imager (ASI) data.
 Author-email: Mykhaylo Shumko <msshumko@gmail.com>
 Project-URL: Homepage, https://aurora-asi-lib.readthedocs.io/
 Project-URL: Documentation, https://aurora-asi-lib.readthedocs.io/
 Project-URL: Source, https://github.com/mshumko/asilib
 Project-URL: Issues, https://github.com/mshumko/asilib/issues
 Project-URL: Changelog, https://github.com/mshumko/asilib/blob/main/CHANGELOG.md
@@ -35,14 +35,19 @@
 Requires-Dist: opencv-python<5.0,>=4.8.0
 
 ![Test python package](https://github.com/mshumko/asilib/workflows/Test%20python%20package/badge.svg) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4746447.svg)](https://doi.org/10.5281/zenodo.4746446)
 
 # asilib
 asilib is an open source package providing data access and analysis tools for the world's all-sky imager (ASI) data.
 
+> [!NOTE]  
+> The asilib code on PyPI moved from [aurora-asi-lib](https://pypi.org/project/aurora-asi-lib/) to [asilib](https://pypi.org/project/asilib/). To update to version >=0.22.0, run
+> 1. `python3 -m pip uninstall aurora-asi-lib` and
+> 2. `python3 -m pip install asilib`.
+
 The purpose of this project is to combine data from numerous observational ASI arrays into a single unified framework and is thus not associated with the development and operations of all sky cameras, or the curation of ASI datasets. All data is publicly available and is provided as-is. Please give appropriate credit and coordinate with instrument teams with regards to data issues and/or interpretation. See the [Acknowledgements](https://aurora-asi-lib.readthedocs.io/en/latest/index.html#acknowledgements) section for more information. Currently the supported camera systems (arrays) are: 
 * [Red-line Emission Geospace Observatory (REGO)](https://aurora-asi-lib.readthedocs.io/en/latest/imager_api.html#rego-asi)
 * [Time History of Events and Macroscale Interactions during Substorms (THEMIS)](https://aurora-asi-lib.readthedocs.io/en/latest/imager_api.html#module-asilib.asi.themis)
 * [Transition Region Explorer (TREx)](https://aurora-asi-lib.readthedocs.io/en/latest/imager_api.html#module-asilib.asi.trex)
 
 [Documentation](https://aurora-asi-lib.readthedocs.io/) | [Code on GitHub](https://github.com/mshumko/asilib) | [PyPI archive](https://pypi.org/project/asilib/) | [Zenodo archive](https://doi.org/10.5281/zenodo.4746446)
```

### Comparing `asilib-0.22.0/asilib.egg-info/SOURCES.txt` & `asilib-0.23.0/asilib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asilib-0.22.0/pyproject.toml` & `asilib-0.23.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asilib"
-version = "0.22.0"
+version = "0.23.0"
 description = "An open source package providing data access and analysis tools for the world's all-sky imager (ASI) data."
 keywords = [ "aurora", "all sky imager", "REGO", "THEMIS", "TREx",]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 
     "Programming Language :: Python :: 3", 
     "Programming Language :: Python :: 3.9",
```


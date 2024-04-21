# Comparing `tmp/flake8-bugbear-24.1.17.tar.gz` & `tmp/flake8-bugbear-24.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-bugbear-24.1.17.tar", last modified: Wed Jan 17 15:53:15 2024, max compression
+gzip compressed data, was "flake8-bugbear-24.2.6.tar", last modified: Wed Feb  7 04:25:14 2024, max compression
```

## Comparing `flake8-bugbear-24.1.17.tar` & `flake8-bugbear-24.2.6.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 15:53:15.841728 flake8-bugbear-24.1.17/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    30707 2024-01-17 15:53:15.841728 flake8-bugbear-24.1.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    29032 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    77485 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/bugbear.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 15:53:15.841728 flake8-bugbear-24.1.17/flake8_bugbear.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    30707 2024-01-17 15:53:15.000000 flake8-bugbear-24.1.17/flake8_bugbear.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-01-17 15:53:15.000000 flake8-bugbear-24.1.17/flake8_bugbear.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 15:53:15.000000 flake8-bugbear-24.1.17/flake8_bugbear.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-17 15:53:15.000000 flake8-bugbear-24.1.17/flake8_bugbear.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 15:53:15.000000 flake8-bugbear-24.1.17/flake8_bugbear.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-17 15:53:15.000000 flake8-bugbear-24.1.17/flake8_bugbear.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-17 15:53:15.000000 flake8-bugbear-24.1.17/flake8_bugbear.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-17 15:53:15.845728 flake8-bugbear-24.1.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 15:53:15.841728 flake8-bugbear-24.1.17/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b001.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b002.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b003.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b004.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b005.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b006_b008.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b007.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b008_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b009_b010.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b011.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b012.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b013.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b014.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b015.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b016.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b017.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b018_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b018_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b018_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b018_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b019.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b020.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b021.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b022.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b023.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b024.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b025.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b026.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b027.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b028.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b029.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b030.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b031.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b032.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b033.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b034.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b035.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b036.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b037.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b038.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b901.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b902.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b902_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b902_py38.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b903.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b904.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b905_py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b906.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b907.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b908.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/b950.py
--rw-r--r--   0 runner    (1001) docker     (127)    37019 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tests/test_bugbear.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-01-17 15:53:03.000000 flake8-bugbear-24.1.17/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 04:25:14.098866 flake8-bugbear-24.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    31060 2024-02-07 04:25:14.098866 flake8-bugbear-24.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    29386 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    77500 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/bugbear.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 04:25:14.094866 flake8-bugbear-24.2.6/flake8_bugbear.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    31060 2024-02-07 04:25:14.000000 flake8-bugbear-24.2.6/flake8_bugbear.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-02-07 04:25:14.000000 flake8-bugbear-24.2.6/flake8_bugbear.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 04:25:14.000000 flake8-bugbear-24.2.6/flake8_bugbear.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-07 04:25:14.000000 flake8-bugbear-24.2.6/flake8_bugbear.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 04:25:13.000000 flake8-bugbear-24.2.6/flake8_bugbear.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-07 04:25:14.000000 flake8-bugbear-24.2.6/flake8_bugbear.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-07 04:25:14.000000 flake8-bugbear-24.2.6/flake8_bugbear.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-07 04:25:14.098866 flake8-bugbear-24.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 04:25:14.094866 flake8-bugbear-24.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b001.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b002.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b003.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b004.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b005.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b006_b008.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b007.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b008_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b009_b010.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b011.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b012.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b013.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b014.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b015.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b016.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b017.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b018_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b018_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b018_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b018_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b019.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b020.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b021.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b022.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b023.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b024.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b025.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b026.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b027.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b028.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b029.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b030.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b031.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b032.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b033.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b034.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b035.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b036.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b037.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b901.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b902.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b902_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b902_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b903.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b904.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b905_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b906.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b907.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b908.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b909.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/b950.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37019 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tests/test_bugbear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-02-07 04:25:00.000000 flake8-bugbear-24.2.6/tox.ini
```

### Comparing `flake8-bugbear-24.1.17/LICENSE` & `flake8-bugbear-24.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/PKG-INFO` & `flake8-bugbear-24.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-bugbear
-Version: 24.1.17
+Version: 24.2.6
 Summary: A plugin for flake8 finding likely bugs and design problems in your program. Contains warnings that don't belong in pyflakes and pycodestyle.
 Author-email: Łukasz Langa <lukasz@langa.pl>
 License: MIT
 Project-URL: Homepage, https://github.com/PyCQA/flake8-bugbear
 Project-URL: Change Log, https://github.com/PyCQA/flake8-bugbear#change-log
 Keywords: flake8,bugbear,bugs,pyflakes,pylint,linter,qa
 Classifier: Development Status :: 5 - Production/Stable
@@ -233,15 +233,15 @@
 
 **B035**: Found dict comprehension with a static key - either a constant value or variable not from the comprehension expression. This will result in a dict with a single key that was repeatedly overwritten.
 
 **B036**: Found ``except BaseException:`` without re-raising (no ``raise`` in the top-level of the ``except`` block). This catches all kinds of things (Exception, SystemExit, KeyboardInterrupt...) and may prevent a program from exiting as expected.
 
 **B037**: Found ``return <value>``, ``yield``, ``yield <value>``, or ``yield from <value>`` in class ``__init__()`` method. No values should be returned or yielded, only bare ``return``\s are ok.
 
-**B038**: Found a mutation of a mutable loop iterable inside the loop body. Changes to the iterable of a loop such as calls to `list.remove()` or via `del` can cause unintended bugs.
+**B038**: **Moved to B909** - Found a mutation of a mutable loop iterable inside the loop body. Changes to the iterable of a loop such as calls to `list.remove()` or via `del` can cause unintended bugs.
 
 Opinionated warnings
 ~~~~~~~~~~~~~~~~~~~~
 
 The following warnings are disabled by default because they are
 controversial.  They may or may not apply to you, enable them explicitly
 in your configuration if you find them useful.  Read below on how to
@@ -282,14 +282,16 @@
 Will only trigger on function names where the part after ``visit_`` is a valid ``ast`` type with a non-empty ``_fields`` attribute.
 This is meant to be enabled by developers writing visitors using the ``ast`` module, such as flake8 plugin writers.
 
 **B907**: Consider replacing ``f"'{foo}'"`` with ``f"{foo!r}"`` which is both easier to read and will escape quotes inside ``foo`` if that would appear. The check tries to filter out any format specs that are invalid together with ``!r``. If you're using other conversion flags then e.g. ``f"'{foo!a}'"`` can be replaced with ``f"{ascii(foo)!r}"``. Not currently implemented for python<3.8 or ``str.format()`` calls.
 
 **B908**: Contexts with exceptions assertions like ``with self.assertRaises`` or ``with pytest.raises`` should not have multiple top-level statements. Each statement should be in its own context. That way, the test ensures that the exception is raised only in the exact statement where you expect it.
 
+**B909**: **Was B038** - Found a mutation of a mutable loop iterable inside the loop body. Changes to the iterable of a loop such as calls to `list.remove()` or via `del` can cause unintended bugs.
+
 **B950**: Line too long. This is a pragmatic equivalent of
 ``pycodestyle``'s ``E501``: it considers "max-line-length" but only triggers
 when the value has been exceeded by **more than 10%**. ``noqa`` and ``type: ignore`` comments are ignored. You will no
 longer be forced to reformat code due to the closing parenthesis being
 one character too far to satisfy the linter. At the same time, if you do
 significantly violate the line length, you will receive a message that
 states what the actual limit is. This is inspired by Raymond Hettinger's
@@ -349,15 +351,15 @@
 The plugin currently has the following settings:
 
 ``extend-immutable-calls``: Specify a list of additional immutable calls.
 This could be useful, when using other libraries that provide more immutable calls,
 beside those already handled by ``flake8-bugbear``. Calls to these method will no longer
 raise a ``B008`` warning.
 
-``classmethod-decorators``: Specify a list of decorators to additionally mark a method as a ``classmethod`` as used by B902. Default values are ``classmethod, validator, root_validator``, and when an ``@obj.name`` decorator is specified it will match against either ``name`` or ``obj.name``.
+``classmethod-decorators``: Specify a list of decorators to additionally mark a method as a ``classmethod`` as used by B902. The default only checks for ``classmethod``. When an ``@obj.name`` decorator is specified it will match against either ``name`` or ``obj.name``.
 This functions similarly to how `pep8-naming <https://github.com/PyCQA/pep8-naming>` handles it, but with different defaults, and they don't support specifying attributes such that a decorator will never match against a specified value ``obj.name`` even if decorated with ``@obj.name``.
 
 For example::
 
   [flake8]
   max-line-length = 80
   max-complexity = 12
@@ -383,14 +385,20 @@
 
 MIT
 
 
 Change Log
 ----------
 
+24.2.6
+~~~~~~
+
+* B902: Remove decorators named validator and root_validator from B902 checks (#459)
+* B038: Change B038 to B909 and make it optional (#456)
+
 24.1.17
 ~~~~~~~
 
 * B038: Restrict rule to mutation functions only (#453)
 
 24.1.16
 ~~~~~~~
```

### Comparing `flake8-bugbear-24.1.17/README.rst` & `flake8-bugbear-24.2.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 
 **B035**: Found dict comprehension with a static key - either a constant value or variable not from the comprehension expression. This will result in a dict with a single key that was repeatedly overwritten.
 
 **B036**: Found ``except BaseException:`` without re-raising (no ``raise`` in the top-level of the ``except`` block). This catches all kinds of things (Exception, SystemExit, KeyboardInterrupt...) and may prevent a program from exiting as expected.
 
 **B037**: Found ``return <value>``, ``yield``, ``yield <value>``, or ``yield from <value>`` in class ``__init__()`` method. No values should be returned or yielded, only bare ``return``\s are ok.
 
-**B038**: Found a mutation of a mutable loop iterable inside the loop body. Changes to the iterable of a loop such as calls to `list.remove()` or via `del` can cause unintended bugs.
+**B038**: **Moved to B909** - Found a mutation of a mutable loop iterable inside the loop body. Changes to the iterable of a loop such as calls to `list.remove()` or via `del` can cause unintended bugs.
 
 Opinionated warnings
 ~~~~~~~~~~~~~~~~~~~~
 
 The following warnings are disabled by default because they are
 controversial.  They may or may not apply to you, enable them explicitly
 in your configuration if you find them useful.  Read below on how to
@@ -244,14 +244,16 @@
 Will only trigger on function names where the part after ``visit_`` is a valid ``ast`` type with a non-empty ``_fields`` attribute.
 This is meant to be enabled by developers writing visitors using the ``ast`` module, such as flake8 plugin writers.
 
 **B907**: Consider replacing ``f"'{foo}'"`` with ``f"{foo!r}"`` which is both easier to read and will escape quotes inside ``foo`` if that would appear. The check tries to filter out any format specs that are invalid together with ``!r``. If you're using other conversion flags then e.g. ``f"'{foo!a}'"`` can be replaced with ``f"{ascii(foo)!r}"``. Not currently implemented for python<3.8 or ``str.format()`` calls.
 
 **B908**: Contexts with exceptions assertions like ``with self.assertRaises`` or ``with pytest.raises`` should not have multiple top-level statements. Each statement should be in its own context. That way, the test ensures that the exception is raised only in the exact statement where you expect it.
 
+**B909**: **Was B038** - Found a mutation of a mutable loop iterable inside the loop body. Changes to the iterable of a loop such as calls to `list.remove()` or via `del` can cause unintended bugs.
+
 **B950**: Line too long. This is a pragmatic equivalent of
 ``pycodestyle``'s ``E501``: it considers "max-line-length" but only triggers
 when the value has been exceeded by **more than 10%**. ``noqa`` and ``type: ignore`` comments are ignored. You will no
 longer be forced to reformat code due to the closing parenthesis being
 one character too far to satisfy the linter. At the same time, if you do
 significantly violate the line length, you will receive a message that
 states what the actual limit is. This is inspired by Raymond Hettinger's
@@ -311,15 +313,15 @@
 The plugin currently has the following settings:
 
 ``extend-immutable-calls``: Specify a list of additional immutable calls.
 This could be useful, when using other libraries that provide more immutable calls,
 beside those already handled by ``flake8-bugbear``. Calls to these method will no longer
 raise a ``B008`` warning.
 
-``classmethod-decorators``: Specify a list of decorators to additionally mark a method as a ``classmethod`` as used by B902. Default values are ``classmethod, validator, root_validator``, and when an ``@obj.name`` decorator is specified it will match against either ``name`` or ``obj.name``.
+``classmethod-decorators``: Specify a list of decorators to additionally mark a method as a ``classmethod`` as used by B902. The default only checks for ``classmethod``. When an ``@obj.name`` decorator is specified it will match against either ``name`` or ``obj.name``.
 This functions similarly to how `pep8-naming <https://github.com/PyCQA/pep8-naming>` handles it, but with different defaults, and they don't support specifying attributes such that a decorator will never match against a specified value ``obj.name`` even if decorated with ``@obj.name``.
 
 For example::
 
   [flake8]
   max-line-length = 80
   max-complexity = 12
@@ -345,14 +347,20 @@
 
 MIT
 
 
 Change Log
 ----------
 
+24.2.6
+~~~~~~
+
+* B902: Remove decorators named validator and root_validator from B902 checks (#459)
+* B038: Change B038 to B909 and make it optional (#456)
+
 24.1.17
 ~~~~~~~
 
 * B038: Restrict rule to mutation functions only (#453)
 
 24.1.16
 ~~~~~~~
```

### Comparing `flake8-bugbear-24.1.17/bugbear.py` & `flake8-bugbear-24.2.6/bugbear.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from functools import lru_cache, partial
 from keyword import iskeyword
 from typing import Dict, List, Set, Union
 
 import attr
 import pycodestyle
 
-__version__ = "24.1.17"
+__version__ = "24.2.6"
 
 LOG = logging.getLogger("flake8.bugbear")
 CONTEXTFUL_NODES = (
     ast.Module,
     ast.ClassDef,
     ast.AsyncFunctionDef,
     ast.FunctionDef,
@@ -37,15 +37,15 @@
     "assertRaises",
     "assertRaisesRegex",
     "assertRaisesRegexp",
     "assertWarns",
     "assertWarnsRegex",
 }
 
-B902_default_decorators = {"classmethod", "validator", "root_validator"}
+B902_default_decorators = {"classmethod"}
 
 Context = namedtuple("Context", ["node", "stack"])
 
 
 @attr.s(hash=False)
 class BugBearChecker:
     name = "flake8-bugbear"
@@ -520,15 +520,15 @@
         self.generic_visit(node)
 
     def visit_For(self, node):
         self.check_for_b007(node)
         self.check_for_b020(node)
         self.check_for_b023(node)
         self.check_for_b031(node)
-        self.check_for_b038(node)
+        self.check_for_b909(node)
         self.generic_visit(node)
 
     def visit_AsyncFor(self, node):
         self.check_for_b023(node)
         self.generic_visit(node)
 
     def visit_While(self, node):
@@ -1570,38 +1570,38 @@
                 )
 
         if node.func.attr in ("sub", "subn"):
             check(3, "count")
         elif node.func.attr == "split":
             check(2, "maxsplit")
 
-    def check_for_b038(self, node: ast.For):
+    def check_for_b909(self, node: ast.For):
         if isinstance(node.iter, ast.Name):
             name = _to_name_str(node.iter)
         elif isinstance(node.iter, ast.Attribute):
             name = _to_name_str(node.iter)
         else:
             return
-        checker = B038Checker(name)
+        checker = B909Checker(name)
         checker.visit(node.body)
         for mutation in checker.mutations:
-            self.errors.append(B038(mutation.lineno, mutation.col_offset))
+            self.errors.append(B909(mutation.lineno, mutation.col_offset))
 
 
 def compose_call_path(node):
     if isinstance(node, ast.Attribute):
         yield from compose_call_path(node.value)
         yield node.attr
     elif isinstance(node, ast.Call):
         yield from compose_call_path(node.func)
     elif isinstance(node, ast.Name):
         yield node.id
 
 
-class B038Checker(ast.NodeVisitor):
+class B909Checker(ast.NodeVisitor):
     # https://docs.python.org/3/library/stdtypes.html#mutable-sequence-types
     MUTATING_FUNCTIONS = (
         "append",
         "sort",
         "reverse",
         "remove",
         "clear",
@@ -2142,16 +2142,26 @@
 )
 B908 = Error(
     message=(
         "B908 assertRaises-type context should not contain more than one top-level"
         " statement."
     )
 )
-
-B950 = Error(message="B950 line too long ({} > {} characters)")
-
-B038 = Error(
+B909 = Error(
     message=(
-        "B038 editing a loop's mutable iterable often leads to unexpected results/bugs"
+        "B909 editing a loop's mutable iterable often leads to unexpected results/bugs"
     )
 )
-disabled_by_default = ["B901", "B902", "B903", "B904", "B905", "B906", "B908", "B950"]
+B950 = Error(message="B950 line too long ({} > {} characters)")
+
+
+disabled_by_default = [
+    "B901",
+    "B902",
+    "B903",
+    "B904",
+    "B905",
+    "B906",
+    "B908",
+    "B909",
+    "B950",
+]
```

### Comparing `flake8-bugbear-24.1.17/flake8_bugbear.egg-info/PKG-INFO` & `flake8-bugbear-24.2.6/flake8_bugbear.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-bugbear
-Version: 24.1.17
+Version: 24.2.6
 Summary: A plugin for flake8 finding likely bugs and design problems in your program. Contains warnings that don't belong in pyflakes and pycodestyle.
 Author-email: Łukasz Langa <lukasz@langa.pl>
 License: MIT
 Project-URL: Homepage, https://github.com/PyCQA/flake8-bugbear
 Project-URL: Change Log, https://github.com/PyCQA/flake8-bugbear#change-log
 Keywords: flake8,bugbear,bugs,pyflakes,pylint,linter,qa
 Classifier: Development Status :: 5 - Production/Stable
@@ -233,15 +233,15 @@
 
 **B035**: Found dict comprehension with a static key - either a constant value or variable not from the comprehension expression. This will result in a dict with a single key that was repeatedly overwritten.
 
 **B036**: Found ``except BaseException:`` without re-raising (no ``raise`` in the top-level of the ``except`` block). This catches all kinds of things (Exception, SystemExit, KeyboardInterrupt...) and may prevent a program from exiting as expected.
 
 **B037**: Found ``return <value>``, ``yield``, ``yield <value>``, or ``yield from <value>`` in class ``__init__()`` method. No values should be returned or yielded, only bare ``return``\s are ok.
 
-**B038**: Found a mutation of a mutable loop iterable inside the loop body. Changes to the iterable of a loop such as calls to `list.remove()` or via `del` can cause unintended bugs.
+**B038**: **Moved to B909** - Found a mutation of a mutable loop iterable inside the loop body. Changes to the iterable of a loop such as calls to `list.remove()` or via `del` can cause unintended bugs.
 
 Opinionated warnings
 ~~~~~~~~~~~~~~~~~~~~
 
 The following warnings are disabled by default because they are
 controversial.  They may or may not apply to you, enable them explicitly
 in your configuration if you find them useful.  Read below on how to
@@ -282,14 +282,16 @@
 Will only trigger on function names where the part after ``visit_`` is a valid ``ast`` type with a non-empty ``_fields`` attribute.
 This is meant to be enabled by developers writing visitors using the ``ast`` module, such as flake8 plugin writers.
 
 **B907**: Consider replacing ``f"'{foo}'"`` with ``f"{foo!r}"`` which is both easier to read and will escape quotes inside ``foo`` if that would appear. The check tries to filter out any format specs that are invalid together with ``!r``. If you're using other conversion flags then e.g. ``f"'{foo!a}'"`` can be replaced with ``f"{ascii(foo)!r}"``. Not currently implemented for python<3.8 or ``str.format()`` calls.
 
 **B908**: Contexts with exceptions assertions like ``with self.assertRaises`` or ``with pytest.raises`` should not have multiple top-level statements. Each statement should be in its own context. That way, the test ensures that the exception is raised only in the exact statement where you expect it.
 
+**B909**: **Was B038** - Found a mutation of a mutable loop iterable inside the loop body. Changes to the iterable of a loop such as calls to `list.remove()` or via `del` can cause unintended bugs.
+
 **B950**: Line too long. This is a pragmatic equivalent of
 ``pycodestyle``'s ``E501``: it considers "max-line-length" but only triggers
 when the value has been exceeded by **more than 10%**. ``noqa`` and ``type: ignore`` comments are ignored. You will no
 longer be forced to reformat code due to the closing parenthesis being
 one character too far to satisfy the linter. At the same time, if you do
 significantly violate the line length, you will receive a message that
 states what the actual limit is. This is inspired by Raymond Hettinger's
@@ -349,15 +351,15 @@
 The plugin currently has the following settings:
 
 ``extend-immutable-calls``: Specify a list of additional immutable calls.
 This could be useful, when using other libraries that provide more immutable calls,
 beside those already handled by ``flake8-bugbear``. Calls to these method will no longer
 raise a ``B008`` warning.
 
-``classmethod-decorators``: Specify a list of decorators to additionally mark a method as a ``classmethod`` as used by B902. Default values are ``classmethod, validator, root_validator``, and when an ``@obj.name`` decorator is specified it will match against either ``name`` or ``obj.name``.
+``classmethod-decorators``: Specify a list of decorators to additionally mark a method as a ``classmethod`` as used by B902. The default only checks for ``classmethod``. When an ``@obj.name`` decorator is specified it will match against either ``name`` or ``obj.name``.
 This functions similarly to how `pep8-naming <https://github.com/PyCQA/pep8-naming>` handles it, but with different defaults, and they don't support specifying attributes such that a decorator will never match against a specified value ``obj.name`` even if decorated with ``@obj.name``.
 
 For example::
 
   [flake8]
   max-line-length = 80
   max-complexity = 12
@@ -383,14 +385,20 @@
 
 MIT
 
 
 Change Log
 ----------
 
+24.2.6
+~~~~~~
+
+* B902: Remove decorators named validator and root_validator from B902 checks (#459)
+* B038: Change B038 to B909 and make it optional (#456)
+
 24.1.17
 ~~~~~~~
 
 * B038: Restrict rule to mutation functions only (#453)
 
 24.1.16
 ~~~~~~~
```

### Comparing `flake8-bugbear-24.1.17/flake8_bugbear.egg-info/SOURCES.txt` & `flake8-bugbear-24.2.6/flake8_bugbear.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -49,20 +49,20 @@
 tests/b031.py
 tests/b032.py
 tests/b033.py
 tests/b034.py
 tests/b035.py
 tests/b036.py
 tests/b037.py
-tests/b038.py
 tests/b901.py
 tests/b902.py
 tests/b902_extended.py
 tests/b902_py38.py
 tests/b903.py
 tests/b904.py
 tests/b905_py310.py
 tests/b906.py
 tests/b907.py
 tests/b908.py
+tests/b909.py
 tests/b950.py
 tests/test_bugbear.py
```

### Comparing `flake8-bugbear-24.1.17/pyproject.toml` & `flake8-bugbear-24.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b001.py` & `flake8-bugbear-24.2.6/tests/b001.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b005.py` & `flake8-bugbear-24.2.6/tests/b005.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b006_b008.py` & `flake8-bugbear-24.2.6/tests/b006_b008.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b007.py` & `flake8-bugbear-24.2.6/tests/b007.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b009_b010.py` & `flake8-bugbear-24.2.6/tests/b009_b010.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b012.py` & `flake8-bugbear-24.2.6/tests/b012.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b013.py` & `flake8-bugbear-24.2.6/tests/b013.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b014.py` & `flake8-bugbear-24.2.6/tests/b014.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b017.py` & `flake8-bugbear-24.2.6/tests/b017.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b018_classes.py` & `flake8-bugbear-24.2.6/tests/b018_classes.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b018_functions.py` & `flake8-bugbear-24.2.6/tests/b018_functions.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b018_nested.py` & `flake8-bugbear-24.2.6/tests/b018_nested.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b019.py` & `flake8-bugbear-24.2.6/tests/b019.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b020.py` & `flake8-bugbear-24.2.6/tests/b020.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b021.py` & `flake8-bugbear-24.2.6/tests/b021.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b023.py` & `flake8-bugbear-24.2.6/tests/b023.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b024.py` & `flake8-bugbear-24.2.6/tests/b024.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b027.py` & `flake8-bugbear-24.2.6/tests/b027.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b030.py` & `flake8-bugbear-24.2.6/tests/b030.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b031.py` & `flake8-bugbear-24.2.6/tests/b031.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b034.py` & `flake8-bugbear-24.2.6/tests/b034.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b035.py` & `flake8-bugbear-24.2.6/tests/b035.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b036.py` & `flake8-bugbear-24.2.6/tests/b036.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b037.py` & `flake8-bugbear-24.2.6/tests/b037.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b038.py` & `flake8-bugbear-24.2.6/tests/b909.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b901.py` & `flake8-bugbear-24.2.6/tests/b901.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b902.py` & `flake8-bugbear-24.2.6/tests/b902.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b902_extended.py` & `flake8-bugbear-24.2.6/tests/b902_extended.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b902_py38.py` & `flake8-bugbear-24.2.6/tests/b902_py38.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b903.py` & `flake8-bugbear-24.2.6/tests/b903.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b904.py` & `flake8-bugbear-24.2.6/tests/b904.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b905_py310.py` & `flake8-bugbear-24.2.6/tests/b905_py310.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b906.py` & `flake8-bugbear-24.2.6/tests/b906.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b907.py` & `flake8-bugbear-24.2.6/tests/b907.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b908.py` & `flake8-bugbear-24.2.6/tests/b908.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/b950.py` & `flake8-bugbear-24.2.6/tests/b950.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-24.1.17/tests/test_bugbear.py` & `flake8-bugbear-24.2.6/tests/test_bugbear.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,23 +42,23 @@
     B031,
     B032,
     B033,
     B034,
     B035,
     B036,
     B037,
-    B038,
     B901,
     B902,
     B903,
     B904,
     B905,
     B906,
     B907,
     B908,
+    B909,
     B950,
     BugBearChecker,
     BugBearVisitor,
 )
 
 
 class BugbearTestCase(unittest.TestCase):
@@ -965,35 +965,35 @@
             capture_output=True,
             timeout=60,
         )
         self.assertEqual(proc.returncode, 0, proc.stdout.decode("utf8"))
         self.assertEqual(proc.stdout, b"")
         self.assertEqual(proc.stderr, b"")
 
-    def test_b038(self):
-        filename = Path(__file__).absolute().parent / "b038.py"
-        mock_options = Namespace(select=[], extend_select=["B038"])
+    def test_b909(self):
+        filename = Path(__file__).absolute().parent / "b909.py"
+        mock_options = Namespace(select=[], extend_select=["B909"])
         bbc = BugBearChecker(filename=str(filename), options=mock_options)
         errors = list(bbc.run())
         print(errors)
         expected = [
-            B038(11, 8),
-            B038(26, 8),
-            B038(27, 8),
-            B038(41, 8),
-            B038(47, 8),
-            B038(56, 8),
-            B038(57, 8),
-            B038(58, 8),
-            B038(59, 8),
-            B038(60, 8),
-            B038(61, 8),
-            B038(62, 8),
-            B038(63, 8),
-            B038(74, 8),
+            B909(11, 8),
+            B909(26, 8),
+            B909(27, 8),
+            B909(41, 8),
+            B909(47, 8),
+            B909(56, 8),
+            B909(57, 8),
+            B909(58, 8),
+            B909(59, 8),
+            B909(60, 8),
+            B909(61, 8),
+            B909(62, 8),
+            B909(63, 8),
+            B909(74, 8),
         ]
         self.assertEqual(errors, self.errors(*expected))
 
 
 class TestFuzz(unittest.TestCase):
     from hypothesis import HealthCheck, given, settings
     from hypothesmith import from_grammar
```

### Comparing `flake8-bugbear-24.1.17/tox.ini` & `flake8-bugbear-24.2.6/tox.ini`

 * *Files identical despite different names*


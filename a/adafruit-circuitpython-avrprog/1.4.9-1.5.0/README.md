# Comparing `tmp/adafruit-circuitpython-avrprog-1.4.9.tar.gz` & `tmp/adafruit_circuitpython_avrprog-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-avrprog-1.4.9.tar", last modified: Fri Aug 26 02:32:54 2022, max compression
+gzip compressed data, was "adafruit_circuitpython_avrprog-1.5.0.tar", last modified: Sun Apr 21 13:48:04 2024, max compression
```

## Comparing `adafruit-circuitpython-avrprog-1.4.9.tar` & `adafruit_circuitpython_avrprog-1.5.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.097571 adafruit-circuitpython-avrprog-1.4.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.089571 adafruit-circuitpython-avrprog-1.4.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.089571 adafruit-circuitpython-avrprog-1.4.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.093571 adafruit-circuitpython-avrprog-1.4.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.093571 adafruit-circuitpython-avrprog-1.4.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-08-26 02:32:54.097571 adafruit-circuitpython-avrprog-1.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2747 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)    18236 2022-08-26 02:32:45.000000 adafruit-circuitpython-avrprog-1.4.9/adafruit_avrprog.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.093571 adafruit-circuitpython-avrprog-1.4.9/adafruit_circuitpython_avrprog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-08-26 02:32:54.000000 adafruit-circuitpython-avrprog-1.4.9/adafruit_circuitpython_avrprog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-08-26 02:32:54.000000 adafruit-circuitpython-avrprog-1.4.9/adafruit_circuitpython_avrprog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:32:54.000000 adafruit-circuitpython-avrprog-1.4.9/adafruit_circuitpython_avrprog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-26 02:32:54.000000 adafruit-circuitpython-avrprog-1.4.9/adafruit_circuitpython_avrprog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-26 02:32:54.000000 adafruit-circuitpython-avrprog-1.4.9/adafruit_circuitpython_avrprog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.093571 adafruit-circuitpython-avrprog-1.4.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.093571 adafruit-circuitpython-avrprog-1.4.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5553 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      972 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.097571 adafruit-circuitpython-avrprog-1.4.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/examples/attiny13a_blink.hex
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/examples/attiny13a_blink.hex.license
--rw-r--r--   0 runner    (1001) docker     (121)     2290 2022-08-26 02:32:45.000000 adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_program_mega2560.py
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-08-26 02:32:45.000000 adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_program_tiny13a.py
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-08-26 02:32:45.000000 adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_program_trinket85.py
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-08-26 02:32:45.000000 adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_program_uno328.py
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-08-26 02:32:45.000000 adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_read_signature_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/examples/optiboot_atmega328.hex
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/examples/optiboot_atmega328.hex.license
--rw-r--r--   0 runner    (1001) docker     (121)    20548 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/examples/stk500boot_v2_mega2560.hex
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/examples/stk500boot_v2_mega2560.hex.license
--rw-r--r--   0 runner    (1001) docker     (121)     7080 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/examples/trinket_boot.hex
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/examples/trinket_boot.hex.license
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-08-26 02:32:45.000000 adafruit-circuitpython-avrprog-1.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:32:54.097571 adafruit-circuitpython-avrprog-1.4.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.037680 adafruit_circuitpython_avrprog-1.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.029680 adafruit_circuitpython_avrprog-1.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.033680 adafruit_circuitpython_avrprog-1.5.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.033680 adafruit_circuitpython_avrprog-1.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.033680 adafruit_circuitpython_avrprog-1.5.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-21 13:48:04.037680 adafruit_circuitpython_avrprog-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)    18395 2024-04-21 13:48:01.000000 adafruit_circuitpython_avrprog-1.5.0/adafruit_avrprog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.037680 adafruit_circuitpython_avrprog-1.5.0/adafruit_circuitpython_avrprog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-21 13:48:04.000000 adafruit_circuitpython_avrprog-1.5.0/adafruit_circuitpython_avrprog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-21 13:48:04.000000 adafruit_circuitpython_avrprog-1.5.0/adafruit_circuitpython_avrprog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:48:04.000000 adafruit_circuitpython_avrprog-1.5.0/adafruit_circuitpython_avrprog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-21 13:48:04.000000 adafruit_circuitpython_avrprog-1.5.0/adafruit_circuitpython_avrprog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-21 13:48:04.000000 adafruit_circuitpython_avrprog-1.5.0/adafruit_circuitpython_avrprog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.033680 adafruit_circuitpython_avrprog-1.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.037680 adafruit_circuitpython_avrprog-1.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.037680 adafruit_circuitpython_avrprog-1.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/examples/attiny13a_blink.hex
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/examples/attiny13a_blink.hex.license
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-21 13:48:01.000000 adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_program_mega2560.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-21 13:48:01.000000 adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_program_tiny13a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-21 13:48:01.000000 adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_program_trinket85.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-21 13:48:01.000000 adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_program_uno328.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-21 13:48:01.000000 adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_read_signature_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/examples/optiboot_atmega328.hex
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/examples/optiboot_atmega328.hex.license
+-rw-r--r--   0 runner    (1001) docker     (127)    20548 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/examples/stk500boot_v2_mega2560.hex
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/examples/stk500boot_v2_mega2560.hex.license
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/examples/trinket_boot.hex
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/examples/trinket_boot.hex.license
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-21 13:48:01.000000 adafruit_circuitpython_avrprog-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 13:48:04.037680 adafruit_circuitpython_avrprog-1.5.0/setup.cfg
```

### Comparing `adafruit-circuitpython-avrprog-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_avrprog-1.5.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/.gitignore` & `adafruit_circuitpython_avrprog-1.5.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-avrprog-1.4.9/.pre-commit-config.yaml` & `adafruit_circuitpython_avrprog-1.5.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-avrprog-1.4.9/.pylintrc` & `adafruit_circuitpython_avrprog-1.5.0/.pylintrc`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
@@ -394,25 +357,25 @@
 # List of valid names for the first argument in a metaclass class method.
 valid-metaclass-classmethod-first-arg=mcs
 
 
 [DESIGN]
 
 # Maximum number of arguments for function / method
-max-args=6
+max-args=5
 
 # Maximum number of attributes for a class (see R0902).
 # max-attributes=7
 max-attributes=11
 
 # Maximum number of boolean expressions in a if statement
 max-bool-expr=5
 
 # Maximum number of branch for function / method body
-max-branches=15
+max-branches=12
 
 # Maximum number of locals for function / method body
 max-locals=15
 
 # Maximum number of parents for a class (see R0901).
 max-parents=7
 
@@ -429,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-avrprog-1.4.9/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_avrprog-1.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/LICENSE` & `adafruit_circuitpython_avrprog-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_avrprog-1.5.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/LICENSES/MIT.txt` & `adafruit_circuitpython_avrprog-1.5.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/LICENSES/Unlicense.txt` & `adafruit_circuitpython_avrprog-1.5.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/PKG-INFO` & `adafruit_circuitpython_avrprog-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-avrprog
-Version: 1.4.9
+Version: 1.5.0
 Summary: CircuitPython helper library for programming AVR chips.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AVRprog
 Keywords: adafruit,avr,spi,atmega,attiny,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
 License-File: LICENSE
+Requires-Dist: Adafruit-Blinka
+Provides-Extra: optional
 
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-avrprog/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/avrprog/en/latest/
```

### Comparing `adafruit-circuitpython-avrprog-1.4.9/README.rst` & `adafruit_circuitpython_avrprog-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/adafruit_avrprog.py` & `adafruit_circuitpython_avrprog-1.5.0/adafruit_avrprog.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 * Adafruit CircuitPython firmware for the ESP8622 and M0-based boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 # imports
 
-__version__ = "1.4.9"
+__version__ = "1.5.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_AVRprog.git"
 
 from digitalio import Direction, DigitalInOut
 
 _SLOW_CLOCK = 100000
 _FAST_CLOCK = 1000000
 
@@ -67,14 +67,21 @@
         ATmega328p = {
             "name": "ATmega328p",
             "sig": [0x1E, 0x95, 0x0F],
             "flash_size": 32768,
             "page_size": 128,
             "fuse_mask": (0xFF, 0xFF, 0x07, 0x3F),
         }
+        ATmega328pb = {
+            "name": "ATmega328pb",
+            "sig": [0x1E, 0x95, 0x16],
+            "flash_size": 32768,
+            "page_size": 128,
+            "fuse_mask": (0xFF, 0xFF, 0x07, 0x3F),
+        }
         ATmega644pa = {
             "name": "ATmega644pa",
             "sig": [0x1E, 0x96, 0x0A],
             "flash_size": 65536,
             "page_size": 256,
             "fuse_mask": (0xF7, 0x8F, 0xFD, 0xFF),
         }
@@ -110,14 +117,15 @@
         self.end()
         if verbose:
             print("Found signature: %s" % [hex(i) for i in sig])
         if sig != chip["sig"]:
             return False
         return True
 
+    # pylint: disable=too-many-branches
     def program_file(self, chip, file_name, verbose=False, verify=True):
         """
         Perform a chip erase and program from a file that
         contains Intel HEX data. Returns true on verify-success, False on
         verify-failure. If 'verify' is False, return will always be True
         """
         if not self.verify_sig(chip):
@@ -239,33 +247,30 @@
         low = self._transaction((0x50, 0, 0, 0))[2] & mask[0]
         high = self._transaction((0x58, 0x08, 0, 0))[2] & mask[1]
         ext = self._transaction((0x50, 0x08, 0, 0))[2] & mask[2]
         lock = self._transaction((0x58, 0, 0, 0))[2] & mask[3]
         self.end()
         return (low, high, ext, lock)
 
-    # pylint: disable=unused-argument,expression-not-assigned
+    # pylint: disable=unused-argument,too-many-arguments
     def write_fuses(self, chip, low=None, high=None, ext=None, lock=None):
         """
         Write any of the 4 fuses. If the kwarg low/high/ext/lock is not
         passed in or is None, that fuse is skipped
         """
+        transaction_comp = (0xE0, 0xA0, 0xA8, 0xA4)
+        fuses = (lock, low, high, ext)
         self.begin(clock=_SLOW_CLOCK)
-        lock and self._transaction((0xAC, 0xE0, 0, lock))
-        self._busy_wait()
-        low and self._transaction((0xAC, 0xA0, 0, low))
-        self._busy_wait()
-        high and self._transaction((0xAC, 0xA8, 0, high))
-        self._busy_wait()
-        ext and self._transaction((0xAC, 0xA4, 0, ext))
-        self._busy_wait()
+        for fuse, comp in zip(fuses, transaction_comp):
+            if fuse:
+                self._transaction((0xAC, comp, 0, fuse))
+            self._busy_wait()
         self.end()
 
-    # pylint: enable=unused-argument,expression-not-assigned
-
+    # pylint: disable=too-many-arguments
     def verify_fuses(self, chip, low=None, high=None, ext=None, lock=None):
         """
         Verify the 4 fuses. If the kwarg low/high/ext/lock is not
         passed in or is None, that fuse is not checked.
         Each fuse is bitwise-&'s with the chip's fuse mask.
         Returns True on success, False on a fuse verification failure
         """
```

### Comparing `adafruit-circuitpython-avrprog-1.4.9/adafruit_circuitpython_avrprog.egg-info/PKG-INFO` & `adafruit_circuitpython_avrprog-1.5.0/adafruit_circuitpython_avrprog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-avrprog
-Version: 1.4.9
+Version: 1.5.0
 Summary: CircuitPython helper library for programming AVR chips.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AVRprog
 Keywords: adafruit,avr,spi,atmega,attiny,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
 License-File: LICENSE
+Requires-Dist: Adafruit-Blinka
+Provides-Extra: optional
 
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-avrprog/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/avrprog/en/latest/
```

### Comparing `adafruit-circuitpython-avrprog-1.4.9/adafruit_circuitpython_avrprog.egg-info/SOURCES.txt` & `adafruit_circuitpython_avrprog-1.5.0/adafruit_circuitpython_avrprog.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 adafruit_avrprog.py
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_avrprog.egg-info/PKG-INFO
 adafruit_circuitpython_avrprog.egg-info/SOURCES.txt
 adafruit_circuitpython_avrprog.egg-info/dependency_links.txt
 adafruit_circuitpython_avrprog.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-avrprog-1.4.9/docs/_static/favicon.ico` & `adafruit_circuitpython_avrprog-1.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/docs/conf.py` & `adafruit_circuitpython_avrprog-1.5.0/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
 ]
 
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
@@ -92,27 +93,18 @@
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-on_rtd = os.environ.get("READTHEDOCS", None) == "True"
+import sphinx_rtd_theme
 
-if not on_rtd:  # only import and set the theme if we're building docs locally
-    try:
-        import sphinx_rtd_theme
-
-        html_theme = "sphinx_rtd_theme"
-        html_theme_path = [sphinx_rtd_theme.get_html_theme_path(), "."]
-    except:
-        html_theme = "default"
-        html_theme_path = ["."]
-else:
-    html_theme_path = ["."]
+html_theme = "sphinx_rtd_theme"
+html_theme_path = [sphinx_rtd_theme.get_html_theme_path(), "."]
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 # The name of an image file (relative to this directory) to use as a favicon of
```

### Comparing `adafruit-circuitpython-avrprog-1.4.9/docs/examples.rst` & `adafruit_circuitpython_avrprog-1.5.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/docs/index.rst` & `adafruit_circuitpython_avrprog-1.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_program_mega2560.py` & `adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_program_mega2560.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_program_tiny13a.py` & `adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_program_tiny13a.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_program_trinket85.py` & `adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_program_trinket85.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_program_uno328.py` & `adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_program_uno328.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_read_signature_simpletest.py` & `adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_read_signature_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/examples/optiboot_atmega328.hex` & `adafruit_circuitpython_avrprog-1.5.0/examples/optiboot_atmega328.hex`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/examples/stk500boot_v2_mega2560.hex` & `adafruit_circuitpython_avrprog-1.5.0/examples/stk500boot_v2_mega2560.hex`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/examples/trinket_boot.hex` & `adafruit_circuitpython_avrprog-1.5.0/examples/trinket_boot.hex`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.9/pyproject.toml` & `adafruit_circuitpython_avrprog-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-avrprog"
 description = "CircuitPython helper library for programming AVR chips."
-version = "1.4.9"
+version = "1.5.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_AVRprog"}
 keywords = [
     "adafruit",
```


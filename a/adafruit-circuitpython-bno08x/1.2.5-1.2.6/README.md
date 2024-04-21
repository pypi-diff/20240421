# Comparing `tmp/adafruit-circuitpython-bno08x-1.2.5.tar.gz` & `tmp/adafruit_circuitpython_bno08x-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bno08x-1.2.5.tar", last modified: Sat Dec  9 17:17:12 2023, max compression
+gzip compressed data, was "adafruit_circuitpython_bno08x-1.2.6.tar", last modified: Sun Apr 21 13:47:11 2024, max compression
```

## Comparing `adafruit-circuitpython-bno08x-1.2.5.tar` & `adafruit_circuitpython_bno08x-1.2.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:17:12.891130 adafruit-circuitpython-bno08x-1.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:17:12.879130 adafruit-circuitpython-bno08x-1.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:17:12.883130 adafruit-circuitpython-bno08x-1.2.5/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:17:12.883130 adafruit-circuitpython-bno08x-1.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:17:12.883130 adafruit-circuitpython-bno08x-1.2.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2023-12-09 17:17:12.891130 adafruit-circuitpython-bno08x-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:17:12.883130 adafruit-circuitpython-bno08x-1.2.5/adafruit_bno08x/
--rw-r--r--   0 runner    (1001) docker     (127)    40573 2023-12-09 17:17:06.000000 adafruit-circuitpython-bno08x-1.2.5/adafruit_bno08x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2023-12-09 17:17:06.000000 adafruit-circuitpython-bno08x-1.2.5/adafruit_bno08x/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2023-12-09 17:17:06.000000 adafruit-circuitpython-bno08x-1.2.5/adafruit_bno08x/i2c.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2023-12-09 17:17:06.000000 adafruit-circuitpython-bno08x-1.2.5/adafruit_bno08x/spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2023-12-09 17:17:06.000000 adafruit-circuitpython-bno08x-1.2.5/adafruit_bno08x/uart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:17:12.887130 adafruit-circuitpython-bno08x-1.2.5/adafruit_circuitpython_bno08x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2023-12-09 17:17:12.000000 adafruit-circuitpython-bno08x-1.2.5/adafruit_circuitpython_bno08x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-12-09 17:17:12.000000 adafruit-circuitpython-bno08x-1.2.5/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 17:17:12.000000 adafruit-circuitpython-bno08x-1.2.5/adafruit_circuitpython_bno08x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-09 17:17:12.000000 adafruit-circuitpython-bno08x-1.2.5/adafruit_circuitpython_bno08x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-09 17:17:12.000000 adafruit-circuitpython-bno08x-1.2.5/adafruit_circuitpython_bno08x.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:17:12.887130 adafruit-circuitpython-bno08x-1.2.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:17:12.887130 adafruit-circuitpython-bno08x-1.2.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:17:12.887130 adafruit-circuitpython-bno08x-1.2.5/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2023-12-09 17:17:06.000000 adafruit-circuitpython-bno08x-1.2.5/examples/bno08x_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2023-12-09 17:17:06.000000 adafruit-circuitpython-bno08x-1.2.5/examples/bno08x_find_heading.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2023-12-09 17:17:06.000000 adafruit-circuitpython-bno08x-1.2.5/examples/bno08x_more_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2023-12-09 17:17:06.000000 adafruit-circuitpython-bno08x-1.2.5/examples/bno08x_quaternion_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2023-12-09 17:17:06.000000 adafruit-circuitpython-bno08x-1.2.5/examples/bno08x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-09 17:17:06.000000 adafruit-circuitpython-bno08x-1.2.5/examples/bno08x_simpletest_spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2023-12-09 17:17:06.000000 adafruit-circuitpython-bno08x-1.2.5/examples/bno08x_simpletest_uart.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2023-12-09 17:17:06.000000 adafruit-circuitpython-bno08x-1.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-09 17:16:59.000000 adafruit-circuitpython-bno08x-1.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-09 17:17:12.891130 adafruit-circuitpython-bno08x-1.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:47:11.194506 adafruit_circuitpython_bno08x-1.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:47:11.186505 adafruit_circuitpython_bno08x-1.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:47:11.190505 adafruit_circuitpython_bno08x-1.2.6/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:47:11.190505 adafruit_circuitpython_bno08x-1.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:47:11.190505 adafruit_circuitpython_bno08x-1.2.6/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-21 13:47:11.194506 adafruit_circuitpython_bno08x-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:47:11.190505 adafruit_circuitpython_bno08x-1.2.6/adafruit_bno08x/
+-rw-r--r--   0 runner    (1001) docker     (127)    40573 2024-04-21 13:47:08.000000 adafruit_circuitpython_bno08x-1.2.6/adafruit_bno08x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-04-21 13:47:08.000000 adafruit_circuitpython_bno08x-1.2.6/adafruit_bno08x/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-21 13:47:08.000000 adafruit_circuitpython_bno08x-1.2.6/adafruit_bno08x/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-21 13:47:08.000000 adafruit_circuitpython_bno08x-1.2.6/adafruit_bno08x/spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-04-21 13:47:08.000000 adafruit_circuitpython_bno08x-1.2.6/adafruit_bno08x/uart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:47:11.194506 adafruit_circuitpython_bno08x-1.2.6/adafruit_circuitpython_bno08x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-21 13:47:11.000000 adafruit_circuitpython_bno08x-1.2.6/adafruit_circuitpython_bno08x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-21 13:47:11.000000 adafruit_circuitpython_bno08x-1.2.6/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:47:11.000000 adafruit_circuitpython_bno08x-1.2.6/adafruit_circuitpython_bno08x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-21 13:47:11.000000 adafruit_circuitpython_bno08x-1.2.6/adafruit_circuitpython_bno08x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-21 13:47:11.000000 adafruit_circuitpython_bno08x-1.2.6/adafruit_circuitpython_bno08x.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:47:11.194506 adafruit_circuitpython_bno08x-1.2.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:47:11.194506 adafruit_circuitpython_bno08x-1.2.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:47:11.194506 adafruit_circuitpython_bno08x-1.2.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-21 13:47:08.000000 adafruit_circuitpython_bno08x-1.2.6/examples/bno08x_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-21 13:47:08.000000 adafruit_circuitpython_bno08x-1.2.6/examples/bno08x_find_heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-21 13:47:08.000000 adafruit_circuitpython_bno08x-1.2.6/examples/bno08x_more_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-21 13:47:08.000000 adafruit_circuitpython_bno08x-1.2.6/examples/bno08x_quaternion_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-21 13:47:08.000000 adafruit_circuitpython_bno08x-1.2.6/examples/bno08x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-21 13:47:08.000000 adafruit_circuitpython_bno08x-1.2.6/examples/bno08x_simpletest_spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-21 13:47:08.000000 adafruit_circuitpython_bno08x-1.2.6/examples/bno08x_simpletest_uart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-21 13:47:08.000000 adafruit_circuitpython_bno08x-1.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-21 13:47:02.000000 adafruit_circuitpython_bno08x-1.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 13:47:11.194506 adafruit_circuitpython_bno08x-1.2.6/setup.cfg
```

### Comparing `adafruit-circuitpython-bno08x-1.2.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_bno08x-1.2.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/.gitignore` & `adafruit_circuitpython_bno08x-1.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/.pre-commit-config.yaml` & `adafruit_circuitpython_bno08x-1.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/.pylintrc` & `adafruit_circuitpython_bno08x-1.2.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_bno08x-1.2.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/LICENSE` & `adafruit_circuitpython_bno08x-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_bno08x-1.2.6/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/LICENSES/MIT.txt` & `adafruit_circuitpython_bno08x-1.2.6/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/LICENSES/Unlicense.txt` & `adafruit_circuitpython_bno08x-1.2.6/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/PKG-INFO` & `adafruit_circuitpython_bno08x-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bno08x
-Version: 1.2.5
+Version: 1.2.6
 Summary: Helper library for the Hillcrest Laboratories BNO08x IMUs
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BNO08x
 Keywords: adafruit,blinka,circuitpython,micropython,bno080,IMU,BNO055,SENSOR,FUSION,VR,MOTION,TRACK,BNO085
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bno08x-1.2.5/README.rst` & `adafruit_circuitpython_bno08x-1.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/adafruit_bno08x/__init__.py` & `adafruit_circuitpython_bno08x-1.2.6/adafruit_bno08x/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 * Adafruit CircuitPython firmware for the supported boards:
   https:# github.com/adafruit/circuitpython/releases
 
 * `Adafruit's Bus Device library <https:# github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
 """
 from __future__ import annotations
 
-__version__ = "1.2.5"
+__version__ = "1.2.6"
 __repo__ = "https:# github.com/adafruit/Adafruit_CircuitPython_BNO08x.git"
 
 from struct import unpack_from, pack_into
 from collections import namedtuple
 import time
 from micropython import const
```

### Comparing `adafruit-circuitpython-bno08x-1.2.5/adafruit_bno08x/debug.py` & `adafruit_circuitpython_bno08x-1.2.6/adafruit_bno08x/debug.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/adafruit_bno08x/i2c.py` & `adafruit_circuitpython_bno08x-1.2.6/adafruit_bno08x/i2c.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/adafruit_bno08x/spi.py` & `adafruit_circuitpython_bno08x-1.2.6/adafruit_bno08x/spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/adafruit_bno08x/uart.py` & `adafruit_circuitpython_bno08x-1.2.6/adafruit_bno08x/uart.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/adafruit_circuitpython_bno08x.egg-info/PKG-INFO` & `adafruit_circuitpython_bno08x-1.2.6/adafruit_circuitpython_bno08x.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bno08x
-Version: 1.2.5
+Version: 1.2.6
 Summary: Helper library for the Hillcrest Laboratories BNO08x IMUs
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BNO08x
 Keywords: adafruit,blinka,circuitpython,micropython,bno080,IMU,BNO055,SENSOR,FUSION,VR,MOTION,TRACK,BNO085
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bno08x-1.2.5/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt` & `adafruit_circuitpython_bno08x-1.2.6/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/docs/_static/favicon.ico` & `adafruit_circuitpython_bno08x-1.2.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/docs/conf.py` & `adafruit_circuitpython_bno08x-1.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/docs/index.rst` & `adafruit_circuitpython_bno08x-1.2.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/examples/bno08x_calibration.py` & `adafruit_circuitpython_bno08x-1.2.6/examples/bno08x_calibration.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/examples/bno08x_find_heading.py` & `adafruit_circuitpython_bno08x-1.2.6/examples/bno08x_find_heading.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/examples/bno08x_more_reports.py` & `adafruit_circuitpython_bno08x-1.2.6/examples/bno08x_more_reports.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/examples/bno08x_quaternion_service.py` & `adafruit_circuitpython_bno08x-1.2.6/examples/bno08x_quaternion_service.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/examples/bno08x_simpletest.py` & `adafruit_circuitpython_bno08x-1.2.6/examples/bno08x_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/examples/bno08x_simpletest_spi.py` & `adafruit_circuitpython_bno08x-1.2.6/examples/bno08x_simpletest_spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.5/examples/bno08x_simpletest_uart.py` & `adafruit_circuitpython_bno08x-1.2.6/examples/bno08x_simpletest_uart.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 import board  # pylint:disable=wrong-import-order
 import busio  # pylint:disable=wrong-import-order
 
 uart = busio.UART(board.TX, board.RX, baudrate=3000000, receiver_buffer_size=2048)
 
 # uncomment and comment out the above for use with Raspberry Pi
 # import serial
-# uart = serial.Serial("/dev/serial0", 115200)
+# uart = serial.Serial("/dev/serial0", 3000000)
 
-# for a USB Serial cable:
+# for USB Serial (via FTDI cable):
 # import serial
-# uart = serial.Serial("/dev/ttyUSB0", baudrate=115200)
+# uart = serial.Serial("/dev/ttyUSB0", baudrate=3000000)
 
 bno = BNO08X_UART(uart)
 
 bno.enable_feature(adafruit_bno08x.BNO_REPORT_ACCELEROMETER)
 bno.enable_feature(adafruit_bno08x.BNO_REPORT_GYROSCOPE)
 bno.enable_feature(adafruit_bno08x.BNO_REPORT_MAGNETOMETER)
 bno.enable_feature(adafruit_bno08x.BNO_REPORT_ROTATION_VECTOR)
```

### Comparing `adafruit-circuitpython-bno08x-1.2.5/pyproject.toml` & `adafruit_circuitpython_bno08x-1.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-bno08x"
 description = "Helper library for the Hillcrest Laboratories BNO08x IMUs"
-version = "1.2.5"
+version = "1.2.6"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BNO08x"}
 keywords = [
     "adafruit",
```


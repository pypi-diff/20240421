# Comparing `tmp/adafruit-circuitpython-irremote-4.1.9.tar.gz` & `tmp/adafruit_circuitpython_irremote-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-irremote-4.1.9.tar", last modified: Mon Aug 22 18:41:19 2022, max compression
+gzip compressed data, was "adafruit_circuitpython_irremote-5.0.0.tar", last modified: Sun Apr 21 14:24:39 2024, max compression
```

## Comparing `adafruit-circuitpython-irremote-4.1.9.tar` & `adafruit_circuitpython_irremote-5.0.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:19.462977 adafruit-circuitpython-irremote-4.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:19.458977 adafruit-circuitpython-irremote-4.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:19.458977 adafruit-circuitpython-irremote-4.1.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:19.458977 adafruit-circuitpython-irremote-4.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:19.458977 adafruit-circuitpython-irremote-4.1.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4239 2022-08-22 18:41:19.462977 adafruit-circuitpython-irremote-4.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3465 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:19.462977 adafruit-circuitpython-irremote-4.1.9/adafruit_circuitpython_irremote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4239 2022-08-22 18:41:19.000000 adafruit-circuitpython-irremote-4.1.9/adafruit_circuitpython_irremote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-08-22 18:41:19.000000 adafruit-circuitpython-irremote-4.1.9/adafruit_circuitpython_irremote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:41:19.000000 adafruit-circuitpython-irremote-4.1.9/adafruit_circuitpython_irremote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-22 18:41:19.000000 adafruit-circuitpython-irremote-4.1.9/adafruit_circuitpython_irremote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-22 18:41:19.000000 adafruit-circuitpython-irremote-4.1.9/adafruit_circuitpython_irremote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    14029 2022-08-22 18:41:11.000000 adafruit-circuitpython-irremote-4.1.9/adafruit_irremote.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:19.462977 adafruit-circuitpython-irremote-4.1.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:19.462977 adafruit-circuitpython-irremote-4.1.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5111 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:19.462977 adafruit-circuitpython-irremote-4.1.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1209 2022-08-22 18:41:11.000000 adafruit-circuitpython-irremote-4.1.9/examples/irremote_nonblocking.py
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-08-22 18:41:11.000000 adafruit-circuitpython-irremote-4.1.9/examples/irremote_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-08-22 18:41:11.000000 adafruit-circuitpython-irremote-4.1.9/examples/irremote_transmit.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-08-22 18:41:11.000000 adafruit-circuitpython-irremote-4.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:40:59.000000 adafruit-circuitpython-irremote-4.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:41:19.462977 adafruit-circuitpython-irremote-4.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.798521 adafruit_circuitpython_irremote-5.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.786522 adafruit_circuitpython_irremote-5.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.790521 adafruit_circuitpython_irremote-5.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.790521 adafruit_circuitpython_irremote-5.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.794521 adafruit_circuitpython_irremote-5.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-21 14:24:39.794521 adafruit_circuitpython_irremote-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.794521 adafruit_circuitpython_irremote-5.0.0/adafruit_circuitpython_irremote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-21 14:24:39.000000 adafruit_circuitpython_irremote-5.0.0/adafruit_circuitpython_irremote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-21 14:24:39.000000 adafruit_circuitpython_irremote-5.0.0/adafruit_circuitpython_irremote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 14:24:39.000000 adafruit_circuitpython_irremote-5.0.0/adafruit_circuitpython_irremote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 14:24:39.000000 adafruit_circuitpython_irremote-5.0.0/adafruit_circuitpython_irremote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-21 14:24:39.000000 adafruit_circuitpython_irremote-5.0.0/adafruit_circuitpython_irremote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-04-21 14:24:37.000000 adafruit_circuitpython_irremote-5.0.0/adafruit_irremote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.794521 adafruit_circuitpython_irremote-5.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.794521 adafruit_circuitpython_irremote-5.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.794521 adafruit_circuitpython_irremote-5.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-21 14:24:37.000000 adafruit_circuitpython_irremote-5.0.0/examples/irremote_nonblocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-21 14:24:37.000000 adafruit_circuitpython_irremote-5.0.0/examples/irremote_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-21 14:24:37.000000 adafruit_circuitpython_irremote-5.0.0/examples/irremote_transmit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-21 14:24:37.000000 adafruit_circuitpython_irremote-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 14:24:39.798521 adafruit_circuitpython_irremote-5.0.0/setup.cfg
```

### Comparing `adafruit-circuitpython-irremote-4.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_irremote-5.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-irremote-4.1.9/.gitignore` & `adafruit_circuitpython_irremote-5.0.0/.gitignore`

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

### Comparing `adafruit-circuitpython-irremote-4.1.9/.pre-commit-config.yaml` & `adafruit_circuitpython_irremote-5.0.0/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-irremote-4.1.9/.pylintrc` & `adafruit_circuitpython_irremote-5.0.0/.pylintrc`

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
@@ -429,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-irremote-4.1.9/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_irremote-5.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-irremote-4.1.9/LICENSE` & `adafruit_circuitpython_irremote-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-irremote-4.1.9/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_irremote-5.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-irremote-4.1.9/LICENSES/MIT.txt` & `adafruit_circuitpython_irremote-5.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-irremote-4.1.9/LICENSES/Unlicense.txt` & `adafruit_circuitpython_irremote-5.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-irremote-4.1.9/PKG-INFO` & `adafruit_circuitpython_irremote-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-irremote
-Version: 4.1.9
+Version: 5.0.0
 Summary: CircuitPython library for infrared transmit and receive.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IRRemote
 Keywords: adafruit,infrared,transmit,receive,tx,rx,ir,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
 License-File: LICENSE
+Provides-Extra: optional
 
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-irremote/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/irremote/en/latest/
```

### Comparing `adafruit-circuitpython-irremote-4.1.9/README.rst` & `adafruit_circuitpython_irremote-5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-irremote-4.1.9/adafruit_circuitpython_irremote.egg-info/PKG-INFO` & `adafruit_circuitpython_irremote-5.0.0/adafruit_circuitpython_irremote.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-irremote
-Version: 4.1.9
+Version: 5.0.0
 Summary: CircuitPython library for infrared transmit and receive.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IRRemote
 Keywords: adafruit,infrared,transmit,receive,tx,rx,ir,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
 License-File: LICENSE
+Provides-Extra: optional
 
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-irremote/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/irremote/en/latest/
```

### Comparing `adafruit-circuitpython-irremote-4.1.9/adafruit_circuitpython_irremote.egg-info/SOURCES.txt` & `adafruit_circuitpython_irremote-5.0.0/adafruit_circuitpython_irremote.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 adafruit_irremote.py
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
 adafruit_circuitpython_irremote.egg-info/PKG-INFO
 adafruit_circuitpython_irremote.egg-info/SOURCES.txt
 adafruit_circuitpython_irremote.egg-info/dependency_links.txt
 adafruit_circuitpython_irremote.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-irremote-4.1.9/adafruit_irremote.py` & `adafruit_circuitpython_irremote-5.0.0/adafruit_irremote.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # SPDX-FileCopyrightText: 2017 Scott Shawcroft for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
+# pylint: disable=missing-module-docstring
+from __future__ import annotations
+
+import array
+from collections import namedtuple
+import time
+
+try:
+    from typing import List, NamedTuple, Optional, Tuple
+    from pulseio import PulseOut
+except ImportError:
+    pass
+
 """
 `adafruit_irremote`
 ====================================================
 
 Demo code for Circuit Playground Express:
 
 .. code-block:: python
@@ -46,31 +59,28 @@
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the ESP8622 and M0-based boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
-import array
-from collections import namedtuple
-import time
 
-__version__ = "4.1.9"
+__version__ = "5.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_IRRemote.git"
 
 
 class IRDecodeException(Exception):
     """Generic decode exception"""
 
 
 class IRNECRepeatException(Exception):
     """Exception when a NEC repeat is decoded"""
 
 
-def bin_data(pulses):
+def bin_data(pulses: List) -> List[List]:
     """Compute bins of pulse lengths where pulses are +-25% of the average.
 
     :param list pulses: Input pulse lengths
     """
     bins = [[pulses[0], 0]]
 
     for _, pulse in enumerate(pulses):
@@ -85,15 +95,15 @@
                 break
         if not matchedbin:
             bins.append([pulse, 1])
         # print(bins)
     return bins
 
 
-def decode_bits(pulses):
+def decode_bits(pulses: List) -> NamedTuple:
     """Decode the pulses into bits."""
     # pylint: disable=too-many-branches,too-many-statements
 
     # TODO The name pulses is redefined several times below, so we'll stash the
     # original in a separate variable for now. It might be worth refactoring to
     # avoid redefining pulses, for the sake of readability.
     input_pulses = tuple(pulses)
@@ -157,17 +167,17 @@
         # skip outliers
         pulses = [
             p for p in pulses if not (outliers[0] * 0.75) <= p <= (outliers[0] * 1.25)
         ]
     # convert marks/spaces to 0 and 1
     for i, pulse_length in enumerate(pulses):
         if (space * 0.75) <= pulse_length <= (space * 1.25):
-            pulses[i] = False
-        elif (mark * 0.75) <= pulse_length <= (mark * 1.25):
             pulses[i] = True
+        elif (mark * 0.75) <= pulse_length <= (mark * 1.25):
+            pulses[i] = False
         else:
             msg = UnparseableIRMessage(input_pulses, reason="Pulses outside mark/space")
             raise FailedToDecode(msg)
 
     # convert bits to bytes!
     output = [0] * ((len(pulses) + 7) // 8)
     for i, pulse_length in enumerate(pulses):
@@ -197,83 +207,81 @@
 
     :param ~pulseio.PulseIn input_pulses: Object to read pulses from
     :param int max_pulse: Pulse duration to end a burst.  Units are microseconds.
 
     >>> pulses = PulseIn(...)
     >>> decoder = NonblockingGenericDecoder(pulses)
     >>> for message in decoder.read():
-    ...     if isinstace(message, IRMessage):
+    ...     if isinstance(message, IRMessage):
     ...         message.code  # TA-DA! Do something with this in your application.
     ...     else:
     ...         # message is either NECRepeatIRMessage or
     ...         # UnparseableIRMessage. You may decide to ignore it, raise
     ...         # an error, or log the issue to a file. If you raise or log,
     ...         # it may be helpful to include message.pulses in the error message.
     ...         ...
     """
 
-    def __init__(self, pulses, max_pulse=10_000):
+    def __init__(self, pulses: List, max_pulse: int = 10_000) -> None:
         self.pulses = pulses  # PulseIn
         self.max_pulse = max_pulse
         self._unparsed_pulses = []  # internal buffer of partial messages
 
-    def read(self):
+    def read(self) -> None:
         """
         Consume all pulses from PulseIn. Yield decoded messages, if any.
 
         If a partial message is received, this does not block to wait for the
         rest. It stashes the partial message, to be continued the next time it
         is called.
         """
         # Consume from PulseIn.
         while self.pulses:
             pulse = self.pulses.popleft()
-            self._unparsed_pulses.append(pulse)
-            if pulse > self.max_pulse:
+            if pulse <= self.max_pulse:
+                self._unparsed_pulses.append(pulse)
+            else:
                 # End of message! Decode it and yield a BaseIRMessage.
+                result = None
                 try:
-                    yield decode_bits(self._unparsed_pulses)
+                    result = decode_bits(self._unparsed_pulses)
                 except FailedToDecode as err:
                     # If you want to debug failed decodes, this would be a good
                     # place to print/log or (re-)raise.
-                    (unparseable_message,) = err.args
-                    yield unparseable_message
+                    result = err.args[0]
+
                 self._unparsed_pulses.clear()
-                # TODO Do we need to consume and throw away more pulses here?
-                # I'm unclear about the role that "pruning" plays in the
-                # original implementation in GenericDecode._read_pulses_non_blocking.
-        # When we reach here, we have consumed everything from PulseIn.
-        # If there are some pulses in self._unparsed_pulses, they represent
-        # partial messages. We'll finish them next time read() is called.
+                yield result
 
 
 class GenericDecode:
     """Generic decoding of infrared signals"""
 
     # Note: pylint's complaint about the following three methods (no self-use)
     # is absolutely correct, which is why the code was refactored, but we need
     # this here for back-compat, hence we disable pylint for that specific
     # complaint.
 
-    def bin_data(self, pulses):  # pylint: disable=no-self-use
+    def bin_data(self, pulses: List) -> List[List]:  # pylint: disable=no-self-use
         "Wraps the top-level function bin_data for backward-compatibility."
         return bin_data(pulses)
 
-    def decode_bits(self, pulses):  # pylint: disable=no-self-use
+    def decode_bits(self, pulses: List) -> Tuple:  # pylint: disable=no-self-use
         "Wraps the top-level function decode_bits for backward-compatibility."
-        result = decode_bits(pulses)
+        try:
+            result = decode_bits(pulses)
+        except FailedToDecode as err:
+            raise IRDecodeException from err
         if isinstance(result, NECRepeatIRMessage):
             raise IRNECRepeatException()
-        if isinstance(result, UnparseableIRMessage):
-            raise IRDecodeException("10 pulses minimum")
         return result.code
 
-    def _read_pulses_non_blocking(
-        self, input_pulses, max_pulse=10000, pulse_window=0.10
-    ):  # pylint: disable=no-self-use
+    def _read_pulses_non_blocking(  # pylint: disable=no-self-use
+        self, input_pulses: List, max_pulse: int = 10000, pulse_window: float = 0.10
+    ) -> Optional[List]:
         """Read out a burst of pulses without blocking until pulses stop for a specified
         period (pulse_window), pruning pulses after a pulse longer than ``max_pulse``.
 
         :param ~pulseio.PulseIn input_pulses: Object to read pulses from
         :param int max_pulse: Pulse duration to end a burst
         :param float pulse_window: pulses are collected for this period of time
         """
@@ -299,21 +307,21 @@
             if recent_count == 0:
                 return received
             recent_count = 0
             time.sleep(pulse_window)
 
     def read_pulses(
         self,
-        input_pulses,
+        input_pulses: list,
         *,
-        max_pulse=10000,
-        blocking=True,
-        pulse_window=0.10,
-        blocking_delay=0.10,
-    ):
+        max_pulse: int = 10000,
+        blocking: bool = True,
+        pulse_window: float = 0.10,
+        blocking_delay: float = 0.10,
+    ) -> Optional[List]:
         """Read out a burst of pulses until pulses stop for a specified
         period (pulse_window), pruning pulses after a pulse longer than ``max_pulse``.
 
         :param ~pulseio.PulseIn input_pulses: Object to read pulses from
         :param int max_pulse: Pulse duration to end a burst
         :param bool blocking: If True, will block until pulses found.
             If False, will return None if no pulses.
@@ -330,51 +338,70 @@
                 continue
             return pulses
 
 
 class GenericTransmit:
     """Generic infrared transmit class that handles encoding.
 
-    :param int header: The length of header in microseconds
-    :param int one: The length of a one in microseconds
-    :param int zero: The length of a zero in microseconds
+    :param List[int] header: The length of header in microseconds, the length should be even
+    :param List[int] one: The length of a one in microseconds
+    :param List[int] zero: The length of a zero in microseconds
     :param int trail: The length of the trail in microseconds, set to None to disable
     :param bool debug: Enable debug output, default False
     """
 
-    def __init__(self, header, one, zero, trail, *, debug=False):
+    def __init__(
+        self,
+        header: List[int],
+        one: List[int],
+        zero: List[int],
+        trail: int,
+        *,
+        debug: bool = False,
+    ) -> None:
         self.header = header
         self.one = one
         self.zero = zero
         self.trail = trail
         self.debug = debug
 
-    def transmit(self, pulseout, data, *, repeat=0, delay=0, nbits=None):
+    def transmit(
+        self,
+        pulseout: PulseOut,
+        data: bytearray,
+        *,
+        repeat: int = 0,
+        delay: float = 0.0,
+        nbits: Optional[int] = None,
+    ) -> None:
         """Transmit the ``data`` using the ``pulseout``.
 
         :param pulseio.PulseOut pulseout: PulseOut to transmit on
         :param bytearray data: Data to transmit
         :param int repeat: Number of additional retransmissions of the data, default 0
-        :param float delay: Delay between any retransmissions, default 0
+        :param float delay: Delay between any retransmissions, default 0.0
         :param int nbits: Optional number of bits to send,
             useful to send fewer bits than in the data bytes
         """
         bits_to_send = len(data) * 8
         if nbits is not None and nbits < bits_to_send:
             bits_to_send = nbits
 
         durations = array.array(
-            "H", [0] * (2 + bits_to_send * 2 + (0 if self.trail is None else 1))
+            "H",
+            [0]
+            * (len(self.header) + bits_to_send * 2 + (0 if self.trail is None else 1)),
         )
 
-        durations[0] = self.header[0]
-        durations[1] = self.header[1]
+        for i, _ in enumerate(self.header):
+            durations[i] = self.header[i]
+
         if self.trail is not None:
             durations[-1] = self.trail
-        out = 2
+        out = len(self.header)
         bit_count = 0
         for byte_index, _ in enumerate(data):
             for i in range(7, -1, -1):
                 if (data[byte_index] & 1 << i) > 0:
                     durations[out] = self.one[0]
                     durations[out + 1] = self.one[1]
                 else:
```

### Comparing `adafruit-circuitpython-irremote-4.1.9/docs/_static/favicon.ico` & `adafruit_circuitpython_irremote-5.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-irremote-4.1.9/docs/conf.py` & `adafruit_circuitpython_irremote-5.0.0/docs/conf.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
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
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "CircuitPython": ("https://docs.circuitpython.org/en/latest/", None),
@@ -31,15 +33,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit IRREMOTE Library"
-copyright = "2017 Scott Shawcroft"
+creation_year = "2017"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Scott Shawcroft"
 author = "Scott Shawcroft"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
@@ -79,27 +88,18 @@
 
 
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

### Comparing `adafruit-circuitpython-irremote-4.1.9/docs/index.rst` & `adafruit_circuitpython_irremote-5.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-irremote-4.1.9/examples/irremote_nonblocking.py` & `adafruit_circuitpython_irremote-5.0.0/examples/irremote_nonblocking.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-irremote-4.1.9/examples/irremote_simpletest.py` & `adafruit_circuitpython_irremote-5.0.0/examples/irremote_simpletest.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,11 +15,14 @@
     pulses = decoder.read_pulses(pulsein)
     print("Heard", len(pulses), "Pulses:", pulses)
     try:
         code = decoder.decode_bits(pulses)
         print("Decoded:", code)
     except adafruit_irremote.IRNECRepeatException:  # unusual short code!
         print("NEC repeat!")
-    except adafruit_irremote.IRDecodeException as e:  # failed to decode
+    except (
+        adafruit_irremote.IRDecodeException,
+        adafruit_irremote.FailedToDecode,
+    ) as e:  # failed to decode
         print("Failed to decode: ", e.args)
 
     print("----------------------------")
```

### Comparing `adafruit-circuitpython-irremote-4.1.9/examples/irremote_transmit.py` & `adafruit_circuitpython_irremote-5.0.0/examples/irremote_transmit.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 button.direction = digitalio.Direction.INPUT
 button.pull = digitalio.Pull.DOWN
 
 # Create a 'PulseOut' to send infrared signals on the IR transmitter @ 38KHz
 pulseout = pulseio.PulseOut(board.IR_TX, frequency=38000, duty_cycle=2**15)
 # Create an encoder that will take numbers and turn them into NEC IR pulses
 encoder = adafruit_irremote.GenericTransmit(
-    header=[9500, 4500], one=[550, 550], zero=[550, 1700], trail=0
+    header=[9000, 4500], one=[560, 1700], zero=[560, 1700], trail=560
 )
 
 while True:
     if button.value:
         print("IR signal sent!")
         encoder.transmit(pulseout, [255, 2, 255, 0])
         time.sleep(0.2)
```

### Comparing `adafruit-circuitpython-irremote-4.1.9/pyproject.toml` & `adafruit_circuitpython_irremote-5.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-irremote"
 description = "CircuitPython library for infrared transmit and receive."
-version = "4.1.9"
+version = "5.0.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_IRRemote"}
 keywords = [
     "adafruit",
```


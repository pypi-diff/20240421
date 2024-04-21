# Comparing `tmp/redflag-0.4.2rc1.tar.gz` & `tmp/redflag-0.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redflag-0.4.2rc1.tar", last modified: Sun Dec 10 08:12:26 2023, max compression
+gzip compressed data, was "redflag-0.5.0rc1.tar", last modified: Sun Apr 21 09:38:53 2024, max compression
```

## Comparing `redflag-0.4.2rc1.tar` & `redflag-0.5.0rc1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 08:12:26.543010 redflag-0.4.2rc1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 08:12:26.531010 redflag-0.4.2rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 08:12:26.535010 redflag-0.4.2rc1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/.github/ISSUE_TEMPLATE/bug_report.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 08:12:26.535010 redflag-0.4.2rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/.github/workflows/build-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      587 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/.github/workflows/publish-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    11729 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17266 2023-12-10 08:12:26.543010 redflag-0.4.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 08:12:26.535010 redflag-0.4.2rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 08:12:26.535010 redflag-0.4.2rc1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    62347 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/_static/redflag.svg
--rw-r--r--   0 runner    (1001) docker     (127)    52830 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/_static/redflag_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   109883 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/_static/redflag_social.svg
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      602 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 08:12:26.539010 redflag-0.4.2rc1/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)   288191 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/notebooks/Basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    93997 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/notebooks/Tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13590 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/notebooks/Using_redflag_with_Pandas.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   116051 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/notebooks/Using_redflag_with_sklearn.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20563 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/notebooks/_Pandas_accessor.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/post_process_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/pre_process_ipynb.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/redflag.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/docs/what_is_redflag.md
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-10 08:12:26.543010 redflag-0.4.2rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 08:12:26.531010 redflag-0.4.2rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 08:12:26.539010 redflag-0.4.2rc1/src/redflag/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/src/redflag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-12-10 08:12:26.000000 redflag-0.4.2rc1/src/redflag/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    18501 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/src/redflag/distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10918 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/src/redflag/imbalance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/src/redflag/importance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/src/redflag/independence.py
--rw-r--r--   0 runner    (1001) docker     (127)    13294 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/src/redflag/markov.py
--rw-r--r--   0 runner    (1001) docker     (127)     9980 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/src/redflag/outliers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/src/redflag/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    40890 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/src/redflag/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10854 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/src/redflag/target.py
--rw-r--r--   0 runner    (1001) docker     (127)    19480 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/src/redflag/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 08:12:26.543010 redflag-0.4.2rc1/src/redflag.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17266 2023-12-10 08:12:26.000000 redflag-0.4.2rc1/src/redflag.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2023-12-10 08:12:26.000000 redflag-0.4.2rc1/src/redflag.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-10 08:12:26.000000 redflag-0.4.2rc1/src/redflag.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-12-10 08:12:26.000000 redflag-0.4.2rc1/src/redflag.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-10 08:12:26.000000 redflag-0.4.2rc1/src/redflag.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 08:12:26.543010 redflag-0.4.2rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      879 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/tests/test_markov.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/tests/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    11097 2023-12-10 08:11:21.000000 redflag-0.4.2rc1/tests/test_sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:38:53.633740 redflag-0.5.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:38:53.621740 redflag-0.5.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:38:53.621740 redflag-0.5.0rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/.github/ISSUE_TEMPLATE/bug_report.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:38:53.621740 redflag-0.5.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/.github/workflows/build-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/.github/workflows/publish-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12542 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17248 2024-04-21 09:38:53.633740 redflag-0.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:38:53.625740 redflag-0.5.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:38:53.625740 redflag-0.5.0rc1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    62347 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/_static/redflag.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    52830 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/_static/redflag_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   109883 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/_static/redflag_social.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:38:53.629740 redflag-0.5.0rc1/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)   286868 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/notebooks/Basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   929099 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/notebooks/Demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   110335 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/notebooks/Tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/notebooks/Using_redflag_with_Pandas.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   128421 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/notebooks/Using_redflag_with_sklearn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20563 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/notebooks/_Pandas_accessor.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/post_process_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/pre_process_ipynb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/redflag.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/docs/what_is_redflag.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 09:38:53.633740 redflag-0.5.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:38:53.621740 redflag-0.5.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:38:53.629740 redflag-0.5.0rc1/src/redflag/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/src/redflag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20482 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/src/redflag/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/src/redflag/imbalance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/src/redflag/importance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/src/redflag/independence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14941 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/src/redflag/markov.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11703 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/src/redflag/outliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/src/redflag/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40890 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/src/redflag/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/src/redflag/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23044 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/src/redflag/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:38:53.633740 redflag-0.5.0rc1/src/redflag.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17248 2024-04-21 09:38:53.000000 redflag-0.5.0rc1/src/redflag.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-21 09:38:53.000000 redflag-0.5.0rc1/src/redflag.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:38:53.000000 redflag-0.5.0rc1/src/redflag.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-21 09:38:53.000000 redflag-0.5.0rc1/src/redflag.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 09:38:53.000000 redflag-0.5.0rc1/src/redflag.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:38:53.633740 redflag-0.5.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/tests/test_markov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11097 2024-04-21 09:37:57.000000 redflag-0.5.0rc1/tests/test_sklearn.py
```

### Comparing `redflag-0.4.2rc1/.github/ISSUE_TEMPLATE/bug_report.md` & `redflag-0.5.0rc1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/.github/workflows/build-test.yml` & `redflag-0.5.0rc1/.github/workflows/build-test.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Build and test
+name: Tests
 
 on:
   workflow_call:
   workflow_dispatch:
   push:
     branches: [ main, develop ]
   pull_request:
@@ -18,15 +18,15 @@
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
 
     - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
         allow-prereleases: true
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
```

### Comparing `redflag-0.4.2rc1/.github/workflows/publish-docs.yml` & `redflag-0.5.0rc1/.github/workflows/publish-docs.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-name: Publish docs
+name: Docs
 
 on:
   workflow_call:
   workflow_dispatch:
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
 
     - uses: actions/checkout@v4
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
 
     - name: Install package
       run: |
         python -m pip install --upgrade pip
         pip install .[dev]
```

### Comparing `redflag-0.4.2rc1/.github/workflows/pypi-publish.yml` & `redflag-0.5.0rc1/.github/workflows/pypi-publish.yml`

 * *Files 14% similar despite different names*

```diff
@@ -12,18 +12,18 @@
     uses: ./.github/workflows/publish-docs.yml
 
   deploy:
     needs: [tests, docs]
     runs-on: ubuntu-latest
     steps:
 
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
 
     - name: Install package
       run: |
         python -m pip install --upgrade pip
         pip install .[dev]
```

### Comparing `redflag-0.4.2rc1/.gitignore` & `redflag-0.5.0rc1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Mac
+.DS_Store
+
 # Version file autocreated in pyproject.toml and redflag/__init__.py
 _version.py
 
 # Processed docs
 _notebooks
 
 # API docs are built
```

### Comparing `redflag-0.4.2rc1/CHANGELOG.md` & `redflag-0.5.0rc1/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+
+## 0.5.0, 21 April 2024
+
+- This release makes more changes to the tests and documentation in reponse to the review process for [the submission](https://joss.theoj.org/papers/e1ca575ec0c5344144f87176539ef547) to JOSS (see below).
+- In particular, see the following issue: [#97](https://github.com/scienxlab/redflag/issues/97)
+- Changed the method of handling dynamic versioning. For now the package `__version__` attribute is still defined, but it is deprecated and will be removed in `0.6.0`. Use `from importlib.metadata.version('redflag')` to get the version information instead.
+- Changed the default `get_outliers()` method from isolation forest (`'iso'`) to Mahalanobis (`'mah'`) to match other functions, eg `has_outliers()` and the `sklearn` pipeline object.
+- Updated `actions/setup-python` to use v5.
+
+
 ## 0.4.2, 10 December 2023
 
 - This is a minor release making changes to the tests and documentation in reponse to the review process for [a submission](https://joss.theoj.org/papers/e1ca575ec0c5344144f87176539ef547) to [The Journal of Open Source Software](https://joss.theoj.org) (JOSS).
 - See the following issues: [#89](https://github.com/scienxlab/redflag/issues/89), [#90](https://github.com/scienxlab/redflag/issues/90), [#91](https://github.com/scienxlab/redflag/issues/91), [#92](https://github.com/scienxlab/redflag/issues/92), [#93](https://github.com/scienxlab/redflag/issues/93), [#94](https://github.com/scienxlab/redflag/issues/94) and [#95](https://github.com/scienxlab/redflag/issues/95).
 - Now building and testing on Windows and MacOS as well as Linux.
 - Python version `3.12` added to package classifiers
 - Python version `3.12` tested during CI
```

### Comparing `redflag-0.4.2rc1/CODE_OF_CONDUCT.md` & `redflag-0.5.0rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/CONTRIBUTING.md` & `redflag-0.5.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/LICENSE` & `redflag-0.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/PKG-INFO` & `redflag-0.5.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redflag
-Version: 0.4.2rc1
+Version: 0.5.0rc1
 Summary: Safety net for machine learning pipelines.
 Author-email: Matt Hall <kwinkunks@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -216,16 +216,16 @@
 Requires-Dist: myst_nb; extra == "dev"
 Requires-Dist: jupyter; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: seaborn; extra == "dev"
 
 # redflag
 
-[![Build and test](https://github.com/scienxlab/redflag/actions/workflows/build-test.yml/badge.svg)](https://github.com/scienxlab/redflag/actions/workflows/build-test.yml)
-[![Documentation](https://github.com/scienxlab/redflag/actions/workflows/publish-docs.yml/badge.svg)](https://github.com/scienxlab/redflag/actions/workflows/publish-docs.yml)
+[![Tests](https://github.com/scienxlab/redflag/actions/workflows/build-test.yml/badge.svg)](https://github.com/scienxlab/redflag/actions/workflows/build-test.yml)
+[![Docs](https://github.com/scienxlab/redflag/actions/workflows/publish-docs.yml/badge.svg)](https://github.com/scienxlab/redflag/actions/workflows/publish-docs.yml)
 [![PyPI version](https://img.shields.io/pypi/v/redflag.svg)](https://pypi.org/project/redflag/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/redflag.svg)](https://anaconda.org/conda-forge/redflag)
 [![PyPI versions](https://img.shields.io/pypi/pyversions/redflag.svg)](https://pypi.org/project/redflag/)
 [![PyPI license](https://img.shields.io/pypi/l/redflag.svg)](https://pypi.org/project/redflag/)
 
 🚩 `redflag` aims to be an automatic safety net for machine learning datasets. The vision is to accept input of a Pandas `DataFrame` or NumPy `ndarray` representing the input `X` and target `y` in a machine learning task. `redflag` will provide an analysis of each feature, and of the target, including aspects such as class imbalance, leakage, outliers, anomalous data patterns, threats to the IID assumption, and so on. The goal is to complement other projects like `pandas-profiling` and `greatexpectations`.
```

### Comparing `redflag-0.4.2rc1/README.md` & `redflag-0.5.0rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # redflag
 
-[![Build and test](https://github.com/scienxlab/redflag/actions/workflows/build-test.yml/badge.svg)](https://github.com/scienxlab/redflag/actions/workflows/build-test.yml)
-[![Documentation](https://github.com/scienxlab/redflag/actions/workflows/publish-docs.yml/badge.svg)](https://github.com/scienxlab/redflag/actions/workflows/publish-docs.yml)
+[![Tests](https://github.com/scienxlab/redflag/actions/workflows/build-test.yml/badge.svg)](https://github.com/scienxlab/redflag/actions/workflows/build-test.yml)
+[![Docs](https://github.com/scienxlab/redflag/actions/workflows/publish-docs.yml/badge.svg)](https://github.com/scienxlab/redflag/actions/workflows/publish-docs.yml)
 [![PyPI version](https://img.shields.io/pypi/v/redflag.svg)](https://pypi.org/project/redflag/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/redflag.svg)](https://anaconda.org/conda-forge/redflag)
 [![PyPI versions](https://img.shields.io/pypi/pyversions/redflag.svg)](https://pypi.org/project/redflag/)
 [![PyPI license](https://img.shields.io/pypi/l/redflag.svg)](https://pypi.org/project/redflag/)
 
 🚩 `redflag` aims to be an automatic safety net for machine learning datasets. The vision is to accept input of a Pandas `DataFrame` or NumPy `ndarray` representing the input `X` and target `y` in a machine learning task. `redflag` will provide an analysis of each feature, and of the target, including aspects such as class imbalance, leakage, outliers, anomalous data patterns, threats to the IID assumption, and so on. The goal is to complement other projects like `pandas-profiling` and `greatexpectations`.
```

### Comparing `redflag-0.4.2rc1/docs/Makefile` & `redflag-0.5.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/docs/_static/custom.css` & `redflag-0.5.0rc1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/docs/_static/favicon.ico` & `redflag-0.5.0rc1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/docs/_static/redflag.svg` & `redflag-0.5.0rc1/docs/_static/redflag.svg`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/docs/_static/redflag_logo.png` & `redflag-0.5.0rc1/docs/_static/redflag_logo.png`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/docs/_static/redflag_social.svg` & `redflag-0.5.0rc1/docs/_static/redflag_social.svg`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/docs/conf.py` & `redflag-0.5.0rc1/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import sys
 sys.path.insert(0, os.path.abspath('../src'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'redflag'
-copyright = '2023, The Redflag Authors'
+copyright = '2024, The Redflag Authors'
 author = 'The Redflag Authors'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
```

### Comparing `redflag-0.4.2rc1/docs/development.md` & `redflag-0.5.0rc1/docs/development.md`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/docs/index.rst` & `redflag-0.5.0rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/docs/installation.md` & `redflag-0.5.0rc1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/docs/notebooks/Basic_usage.ipynb` & `redflag-0.5.0rc1/docs/notebooks/Basic_usage.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9891833614664771%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'data': {'text/plain': "*

 * *            '["\'0.4.2rc2.dev14+g54704af.d20240421\'"]}}}}, 3: {\'execution_count\': 3, '*

 * *            '\'outputs\': {0: {\'execution_count\': 3}}, \'source\': {insert: [(2, "df = '*

 * *            'pd.read_csv(\'https://raw.githubusercontent.com/scienxlab/datasets/main/kgs/panoma-training-data.csv\')\\n")], '*

 * *            "delete: [2]}}, 6: {'execution_count': 4}, 9: {'execution_count': 5, 'outputs': {0: "*

 * *            "{'execution_count': 5}}}, 12: {'exe […]*

```diff
@@ -21,15 +21,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'0.3.1.dev18+g743d11f.d20230927'"
+                            "'0.4.2rc2.dev14+g54704af.d20240421'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -44,15 +44,15 @@
             "metadata": {},
             "source": [
                 "## Load some data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -258,23 +258,23 @@
                             "Facies        4.000000     6.000000     9.000000  \n",
                             "LATITUDE     37.500380    37.910583    38.063373  \n",
                             "LONGITUDE  -101.325130  -101.106045  -100.987305  \n",
                             "ILD_log10     0.634000     0.823750     1.507000  \n",
                             "RHOB       2342.202051  2434.166399  2802.871147  "
                         ]
                     },
-                    "execution_count": 2,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import pandas as pd\n",
                 "\n",
-                "df = pd.read_csv('https://raw.githubusercontent.com/scienxlab/datasets/main/kgs/Panoma_training_data.csv')\n",
+                "df = pd.read_csv('https://raw.githubusercontent.com/scienxlab/datasets/main/kgs/panoma-training-data.csv')\n",
                 "\n",
                 "# Look at the transposed summary: each column in the DataFrame is a row here.\n",
                 "df.describe().T"
             ]
         },
         {
             "cell_type": "markdown",
@@ -288,15 +288,15 @@
             "metadata": {},
             "source": [
                 "It's fairly easy to tell if a column is numeric or not, but harder to decide if it's continuous or categorical. We can use `is_continuous()` to check if a feature (or the target) is continuous. It uses heuristics and is definitely not foolproof. `redflag` uses it internally sometimes to decide how to treat a feature or target."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "           Well Name ... False\n",
@@ -339,24 +339,24 @@
                 "## Imbalance metrics\n",
                 "\n",
                 "First, we'll look at measuring imbalance in the target using `rf.class_imbalance()`. For binary targets, the metric is imbalace ratio (ratio between majority and minority class). For multiclass targets, the metric is imbalance degree [(Ortigosa-Hernandez et al, 2017)](https://doi.org/10.1016/j.patrec.2017.08.002), a single-value measure that explains (a) how many minority classes there are and (b) how skewed the supports are."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "3.378593040846633"
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "rf.imbalance_degree(df['Lithology'])"
             ]
@@ -380,24 +380,24 @@
             "metadata": {},
             "source": [
                 "We can get the minority classes, which are those with fewer samples than expected. These are returned in order, smallest first:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array(['dolomite', 'sandstone', 'mudstone', 'wackestone'], dtype='<U10')"
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "rf.minority_classes(df['Lithology'])"
             ]
@@ -407,25 +407,25 @@
             "metadata": {},
             "source": [
                 "We can get the 'empirical distribution', which returns the observed frequencies `\u03b6` and the expectations `e`. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([0.39989914, 0.18582955, 0.15834594, 0.04790721, 0.13691377,\n",
                             "       0.07110439])"
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "\u03b6, e = rf.empirical_distribution(df['Lithology'])\n",
                 "\u03b6"
@@ -436,25 +436,25 @@
             "metadata": {},
             "source": [
                 "These are in the same order as `df['Lithology'].unique()` (note that this is different from the order of `np.unique()`, which is sorted)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array(['siltstone', 'limestone', 'wackestone', 'dolomite', 'mudstone',\n",
                             "       'sandstone'], dtype=object)"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df['Lithology'].unique()"
             ]
@@ -464,30 +464,30 @@
             "metadata": {},
             "source": [
                 "We can also inspect the distribution using Pandas; note that this display is sorted by count:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<matplotlib.lines.Line2D at 0x7fcc98669790>"
+                            "<matplotlib.lines.Line2D at 0x132608800>"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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IkK//vqr3WWUCux43ePee+/VokWL9Oijj9pdSqnwzTff6KuvvlLLli3tLsVobCuvzcyZMyWdn9jzySeflK+vr80VuR/nwJSwZcuWady4cXrxxRfVqFEjl5k6JcnPz8+myswzYMAA3X777ex4r1F8fLwmT56smJiYi/5NDh061KbKzBQeHq6vv/5a9evXt7sUo7GtxOUQYEqYh8f5yY//eFiZE9OuHDte9wgPD//TPofDwTkbV+jDDz/Uf//7X82aNUvly5e3uxxjsa28erfddpuWLl2qSpUqqUmTJpf8GdPkk/T5CamEfffdd3aXUGrMmDFDFSpU0IoVK7RixQqXPofDQYApor1799pdQqny6quv6ueff1ZwcLBq1qxZKFibvMMoSWwrr17Xrl2tk3a7detmbzHFiCMwACwXNgeceHr1JkyYcMn+Z555poQqAUo3AowNTpw4offee087duyQJDVo0ECPPPKIddY4rhw73msze/ZsvfLKK9qzZ48kqU6dOho1apQefvhhmyvDjYxtpXvl5OQUuqzf5HOJuBt1CduwYYNq1aqlKVOm6NixYzp27JgmT56sWrVqcWj5KsyePVuNGjVSuXLlVK5cOd1yyy364IMP7C7LKJMnT9Zjjz2mTp066ZNPPtEnn3yijh076tFHH9WUKVPsLs9Yqamp+vDDD/Xhhx9q06ZNdpdjHLaV7rF3717FxMTI19dX/v7+qlSpkipVqqSAgABVqlTJ7vKuCUdgSljr1q11880365133rHuTXHu3DkNHDhQv/zyi5KTk22u0ByTJ0/W+PHjFRsba12y+v3332vatGl6/vnnNXz4cJsrNEN4eLgmTJigPn36uLTPmjVLzz77LOfIXKHMzEz16tVLy5cvV0BAgKTzRxLatm2rjz76qNCMqLg4tpXu0bJlSzmdTg0bNkzBwcGFjlLfeeedNlXmBk6UKB8fH+eOHTsKtW/fvt1Zrlw5GyoyV82aNZ2zZs0q1J6YmOisWbOmDRWZydvb27lnz55C7bt373Z6e3vbUJHZ7rvvPmezZs2cP/74o9W2fft2Z7NmzZy9evWysTKzsK10D19fX+fOnTvtLqNY8BNSCfPz89OBAwcKtaelpalixYo2VGSuI0eOXHQq7DvuuENHjhyxoSIz3Xzzzfrkk08KtX/88ceqXbu2DRWZLSkpSW+++abLPDARERGaNm2avvnmGxsrMwvbSve4/fbblZaWZncZxYLLqEvY/fffrwEDBmjSpEnWznfVqlUaNWqUHnjgAZurM8uFHe+///1vl3Z2vFdmwoQJuv/++5WcnGz9FLdq1SotXbr0osEGl1ZQUFDo0mlJKlu2bKETKPHn2Fa6x7vvvqtHH31Uhw4dUsOGDQv9bd5yyy02VXbtOAemhJ09e1ajRo3S9OnTde7cOUnnN2yPPfaYXnrpJZcbbuHSPv/8c91///2Kioq66I63e/fuNldojtTUVE2ZMsW62qN+/foaOXKkmjRpYnNl5unatatOnDih//u//1NoaKgk6dChQ+rdu7cqVaqkefPm2VyhGdhWuseaNWv04IMPat++fVabw+EoFRMCEmBscvr0af3888+SpFq1ajFj51Vix4vrTVpamrp06aLt27crLCzMamvYsKG+/PJL/eUvf7G5QrOwrbw2ERERql+/vp566qmLnsRbo0YNmyq7dgSYEvbII4/o9ddfL/Qb7qlTp/T444/r/ffft6ky3KjKlCmjI0eOKCgoyKX9t99+U1BQkNH/Q7OL0+nUkiVLtHPnTknng3VUVJTNVZmFbaV7+Pr6asuWLbr55pvtLsXtCDAl7M92Fr/++qtCQkKsQ6W4PHa87uHh4aH09PRC6/Hw4cOqVauW/ve//9lUmZlmz56t+++/v9BPHGfPntVHH31U6HJ1XBzbSvfo3Lmz+vXrp549e9pdittxEm8Jyc7OltPplNPp1MmTJ+Xj42P15efn6+uvvy70RcWl/Vn2zs3NlZeXVwlXY56pU6dKOv97+LvvvqsKFSpYffn5+UpOTla9evXsKs9Y/fv3V8eOHQt9n0+ePKn+/fsTYC6DbaV7de7cWcOHD9e2bdsuetPbLl262FTZtSPAlJCAgAA5HA45HA7VqVOnUL/D4bjsPVRwHjte97gwy67T6dT06dNVpkwZq8/Ly0s1a9bU9OnT7SrPWBdOjvyjgwcPMgV+EbCtdK9HH31UkjRx4sRCfaafxEuAKSHfffednE6n2rVrp88//1yBgYFWn5eXl2rUqGFdsYBLY8frHhdm2G3btq2++OIL46cVt1uTJk2sHW/79u2t2WOl88F679696tixo40VmoFtpXuV5kv3OQemhO3fv1/Vq1fnpoNuwI63eOTn52vbtm2qUaMG6/YKXDgqMGHCBI0cOdLlyOCFYN2zZ09+3iwitpW4HAJMCUtKSlKFChXUqlUrSdK0adP0zjvvWDN1ssO4eux4r84TTzyhRo0aacCAAcrPz1ebNm2UkpKi8uXLa+HChbrrrrvsLtEos2bNUq9evZin5BqxrXSfFStWaNKkSdZ0ExERERo1apRat25tc2XXhlsJlLBRo0YpOztbkrRt2zaNGDFCnTp10t69ezVixAibqzPLE088offee0+SrB3vbbfdprCwMC1fvtze4gzy6aefqnHjxpKkBQsWaN++fdq5c6eGDx+up59+2ubqzNOuXTsdPXrUer5u3To98cQTmjFjho1VmYdtpXt8+OGHioqKUvny5TV06FANHTpU5cqVU/v27TV37ly7y7s2JXfbJTid52+stXfvXqfT6XQ+88wzzp49ezqdTqczNTXVGRwcbGNl5gkNDXWuX7/e6XQ6nfPmzXOGhoY6d+3a5Rw3bpzzjjvusLk6c3h7ezvT0tKcTqfTOWjQIOewYcOcTqfT+csvvzgrVqxoY2VmatWqlXP27NlOp9PpPHLkiLNixYrOyMhIZ5UqVZwTJkywuTpzsK10j3r16jknT55cqP3VV1911qtXz4aK3IcjMCXMy8tLp0+fliQtWbJEHTp0kCQFBgZa/9tA0fz2228KCQmRJH399de69957VadOHT3yyCPatm2bzdWZIzg4WD/++KPy8/OVlJSkv//975LOz4D6+xOkUTQ//PCD/va3v0mSPvnkEzVq1EirV6/WnDlzlJiYaG9xBmFb6R6//PKLOnfuXKi9S5cu1on8puIqpBLWqlUrjRgxQi1bttS6dev08ccfS5J2797NFONX6MKOt2rVqkpKStJbb70liR3vlerfv7/uu+8+Va1aVQ6Hw5oxdu3atVyOfhXy8vKs81+WLFlizbNRr1497pJ+BdhWukdYWJiWLl1aaCbeJUuWWLe6MBUBpoT95z//0b/+9S999tlneuutt1StWjVJ0jfffMMllleIHa97PPvss2rYsKHS0tJ07733WjvfMmXKaMyYMTZXZ54GDRpo+vTpiomJ0eLFi/Xcc89JOj+zceXKlW2uzhxsK91j5MiRGjp0qDZv3uxyV+/ExES9/vrrNld3bbgKCUb77LPPrB3vhf+VzZo1SwEBAeratavN1ZnnzJkzLjOf4sotX75c3bt3V3Z2tvr27Wvds+ff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76/WrVvbVaJb8BNSCbvllls0cOBAde/eXQ0bNlRSUpIiIyOVmpqqmJgYpaen212iMSIiIlS/fn099dRTFz2Jl5100cTHxys4OFiPPPKIS/v777+vo0ePavTo0TZVZqY/3gnY6XTq5MmTKleunObMmcORA5SoatWqadGiRWrQoIFL+w8//KAOHTro8OHDNlV27TgCU8Li4uL04IMPavjw4Wrfvr11t9pFixZx/54rtH//fn355Zel4mQ0O7399tuaO3duofYGDRqoV69eBJgrNGXKFJcA4+HhoZtuuknNmzfnJq4ocdnZ2Tp69Gih9qNHj150fhiTcATGBunp6Tpy5IgaN24sDw8PSefv8eHn56d69erZXJ05OnfurH79+qlnz552l2I0Hx8f7dixQ+Hh4S7tv/zyiyIiIlzm2EHRnDlzRlu3br3oBGwcgSm6U6dOacWKFTpw4IDOnj3r0jd06FCbqjJLnz59tHLlSr366qsu88CMGjVKrVu31qxZs2yu8OpxBMYGISEhCgkJcWm78IeFouvcubOGDx+ubdu2cZLfNQgLC9OqVasKBZhVq1YpNDTUpqrMlZSUpD59+ui3337TH/9/yLkbRbdp0yZ16tRJp0+f1qlTpxQYGKhff/1V5cuXV1BQEAGmiKZPn64nn3xSDz74oPLy8iRJnp6eGjBggF555RWbq7s2HIGBsS4cvboYdhRFl5CQoISEBL3yyitq166dJGnp0qV66qmnNHLkSI0dO9bmCs1Su3ZtdejQQXFxcQoODra7HGPdddddqlOnjqZPny5/f39t2bJFZcuW1UMPPaRhw4ZddlZzuDp16pR+/vlnSVKtWrWsuchMRoABbnBOp1NjxozR1KlTrcP0Pj4+Gj16tOLi4myuzjx+fn7atGmTatWqZXcpRgsICNDatWtVt25dBQQEKCUlRfXr19fatWvVt29f6w7VuHH9+X9hAdwQHA6HXn75ZR09elRr1qzRli1bdOzYMcLLVfrHP/6h5cuX212G8cqWLWsdZQ0KCtKBAwcknb8dS1pamp2l4TrBERgYZerUqRo8eLB8fHw0derUS47lN3LY4fTp07r33nt10003XfTcLP4ui6ZDhw7q16+fHnzwQQ0aNEhbt27V0KFD9cEHH+j48eNau3at3SXCZgQYGCU8PFwbNmxQ5cqVC510+nsOh0O//PJLCVZm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",
+                        "image/png": "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IkK//vqr3WWUCux43ePee+/VokWL9Oijj9pdSqnwzTff6KuvvlLLli3tLsVobCuvzcyZMyWdn9jzySeflK+vr80VuR/nwJSwZcuWady4cXrxxRfVqFEjl5k6JcnPz8+myswzYMAA3X777ex4r1F8fLwmT56smJiYi/5NDh061KbKzBQeHq6vv/5a9evXt7sUo7GtxOUQYEqYh8f5yY//eFiZE9OuHDte9wgPD//TPofDwTkbV+jDDz/Uf//7X82aNUvly5e3uxxjsa28erfddpuWLl2qSpUqqUmTJpf8GdPkk/T5CamEfffdd3aXUGrMmDFDFSpU0IoVK7RixQqXPofDQYApor1799pdQqny6quv6ueff1ZwcLBq1qxZKFibvMMoSWwrr17Xrl2tk3a7detmbzHFiCMwACwXNgeceHr1JkyYcMn+Z555poQqAUo3AowNTpw4offee087duyQJDVo0ECPPPKIddY4rhw73msze/ZsvfLKK9qzZ48kqU6dOho1apQefvhhmyvDjYxtpXvl5OQUuqzf5HOJuBt1CduwYYNq1aqlKVOm6NixYzp27JgmT56sWrVqcWj5KsyePVuNGjVSuXLlVK5cOd1yyy364IMP7C7LKJMnT9Zjjz2mTp066ZNPPtEnn3yijh076tFHH9WUKVPsLs9Yqamp+vDDD/Xhhx9q06ZNdpdjHLaV7rF3717FxMTI19dX/v7+qlSpkipVqqSAgABVqlTJ7vKuCUdgSljr1q11880365133rHuTXHu3DkNHDhQv/zyi5KTk22u0ByTJ0/W+PHjFRsba12y+v3332vatGl6/vnnNXz4cJsrNEN4eLgmTJigPn36uLTPmjVLzz77LOfIXKHMzEz16tVLy5cvV0BAgKTzRxLatm2rjz76qNCMqLg4tpXu0bJlSzmdTg0bNkzBwcGFjlLfeeedNlXmBk6UKB8fH+eOHTsKtW/fvt1Zrlw5GyoyV82aNZ2zZs0q1J6YmOisWbOmDRWZydvb27lnz55C7bt373Z6e3vbUJHZ7rvvPmezZs2cP/74o9W2fft2Z7NmzZy9evWysTKzsK10D19fX+fOnTvtLqNY8BNSCfPz89OBAwcKtaelpalixYo2VGSuI0eOXHQq7DvuuENHjhyxoSIz3Xzzzfrkk08KtX/88ceqXbu2DRWZLSkpSW+++abLPDARERGaNm2avvnmGxsrMwvbSve4/fbblZaWZncZxYLLqEvY/fffrwEDBmjSpEnWznfVqlUaNWqUHnjgAZurM8uFHe+///1vl3Z2vFdmwoQJuv/++5WcnGz9FLdq1SotXbr0osEGl1ZQUFDo0mlJKlu2bKETKPHn2Fa6x7vvvqtHH31Uhw4dUsOGDQv9bd5yyy02VXbtOAemhJ09e1ajRo3S9OnTde7cOUnnN2yPPfaYXnrpJZcbbuHSPv/8c91///2Kioq66I63e/fuNldojtTUVE2ZMsW62qN+/foaOXKkmjRpYnNl5unatatOnDih//u//1NoaKgk6dChQ+rdu7cqVaqkefPm2VyhGdhWuseaNWv04IMPat++fVabw+EoFRMCEmBscvr0af3888+SpFq1ajFj51Vix4vrTVpamrp06aLt27crLCzMamvYsKG+/PJL/eUvf7G5QrOwrbw2ERERql+/vp566qmLnsRbo0YNmyq7dgSYEvbII4/o9ddfL/Qb7qlTp/T444/r/ffft6ky3KjKlCmjI0eOKCgoyKX9t99+U1BQkNH/Q7OL0+nUkiVLtHPnTknng3VUVJTNVZmFbaV7+Pr6asuWLbr55pvtLsXtCDAl7M92Fr/++qtCQkKsQ6W4PHa87uHh4aH09PRC6/Hw4cOqVauW/ve//9lUmZlmz56t+++/v9BPHGfPntVHH31U6HJ1XBzbSvfo3Lmz+vXrp549e9pdittxEm8Jyc7OltPplNPp1MmTJ+Xj42P15efn6+uvvy70RcWl/Vn2zs3NlZeXVwlXY56pU6dKOv97+LvvvqsKFSpYffn5+UpOTla9evXsKs9Y/fv3V8eOHQt9n0+ePKn+/fsTYC6DbaV7de7cWcOHD9e2bdsuetPbLl262FTZtSPAlJCAgAA5HA45HA7VqVOnUL/D4bjsPVRwHjte97gwy67T6dT06dNVpkwZq8/Ly0s1a9bU9OnT7SrPWBdOjvyjgwcPMgV+EbCtdK9HH31UkjRx4sRCfaafxEuAKSHfffednE6n2rVrp88//1yBgYFWn5eXl2rUqGFdsYBLY8frHhdm2G3btq2++OIL46cVt1uTJk2sHW/79u2t2WOl88F679696tixo40VmoFtpXuV5kv3OQemhO3fv1/Vq1fnpoNuwI63eOTn52vbtm2qUaMG6/YKXDgqMGHCBI0cOdLlyOCFYN2zZ09+3iwitpW4HAJMCUtKSlKFChXUqlUrSdK0adP0zjvvWDN1ssO4eux4r84TTzyhRo0aacCAAcrPz1ebNm2UkpKi8uXLa+HChbrrrrvsLtEos2bNUq9evZin5BqxrXSfFStWaNKkSdZ0ExERERo1apRat25tc2XXhlsJlLBRo0YpOztbkrRt2zaNGDFCnTp10t69ezVixAibqzPLE088offee0+SrB3vbbfdprCwMC1fvtze4gzy6aefqnHjxpKkBQsWaN++fdq5c6eGDx+up59+2ubqzNOuXTsdPXrUer5u3To98cQTmjFjho1VmYdtpXt8+OGHioqKUvny5TV06FANHTpU5cqVU/v27TV37ly7y7s2JXfbJTid52+stXfvXqfT6XQ+88wzzp49ezqdTqczNTXVGRwcbGNl5gkNDXWuX7/e6XQ6nfPmzXOGhoY6d+3a5Rw3bpzzjjvusLk6c3h7ezvT0tKcTqfTOWjQIOewYcOcTqfT+csvvzgrVqxoY2VmatWqlXP27NlOp9PpPHLkiLNixYrOyMhIZ5UqVZwTJkywuTpzsK10j3r16jknT55cqP3VV1911qtXz4aK3IcjMCXMy8tLp0+fliQtWbJEHTp0kCQFBgZa/9tA0fz2228KCQmRJH399de69957VadOHT3yyCPatm2bzdWZIzg4WD/++KPy8/OVlJSkv//975LOz4D6+xOkUTQ//PCD/va3v0mSPvnkEzVq1EirV6/WnDlzlJiYaG9xBmFb6R6//PKLOnfuXKi9S5cu1on8puIqpBLWqlUrjRgxQi1bttS6dev08ccfS5J2797NFONX6MKOt2rVqkpKStJbb70liR3vlerfv7/uu+8+Va1aVQ6Hw5oxdu3atVyOfhXy8vKs81+WLFlizbNRr1497pJ+BdhWukdYWJiWLl1aaCbeJUuWWLe6MBUBpoT95z//0b/+9S999tlneuutt1StWjVJ0jfffMMllleIHa97PPvss2rYsKHS0tJ07733WjvfMmXKaMyYMTZXZ54GDRpo+vTpiomJ0eLFi/Xcc89JOj+zceXKlW2uzhxsK91j5MiRGjp0qDZv3uxyV+/ExES9/vrrNld3bbgKCUb77LPPrB3vhf+VzZo1SwEBAeratavN1ZnnzJkzLjOf4sotX75c3bt3V3Z2tvr27Wvds+ff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76/WrVvbVaJb8BNSCbvllls0cOBAde/eXQ0bNlRSUpIiIyOVmpqqmJgYpaen212iMSIiIlS/fn099dRTFz2Jl5100cTHxys4OFiPPPKIS/v777+vo0ePavTo0TZVZqY/3gnY6XTq5MmTKleunObMmcORA5SoatWqadGiRWrQoIFL+w8//KAOHTro8OHDNlV27TgCU8Li4uL04IMPavjw4Wrfvr11t9pFixZx/54rtH//fn355Zel4mQ0O7399tuaO3duofYGDRqoV69eBJgrNGXKFJcA4+HhoZtuuknNmzfnJq4ocdnZ2Tp69Gih9qNHj150fhiTcATGBunp6Tpy5IgaN24sDw8PSefv8eHn56d69erZXJ05OnfurH79+qlnz552l2I0Hx8f7dixQ+Hh4S7tv/zyiyIiIlzm2EHRnDlzRlu3br3oBGwcgSm6U6dOacWKFTpw4IDOnj3r0jd06FCbqjJLnz59tHLlSr366qsu88CMGjVKrVu31qxZs2yu8OpxBMYGISEhCgkJcWm78IeFouvcubOGDx+ubdu2cZLfNQgLC9OqVasKBZhVq1YpNDTUpqrMlZSUpD59+ui3337TH/9/yLkbRbdp0yZ16tRJp0+f1qlTpxQYGKhff/1V5cuXV1BQEAGmiKZPn64nn3xSDz74oPLy8iRJnp6eGjBggF555RWbq7s2HIGBsS4cvboYdhRFl5CQoISEBL3yyitq166dJGnp0qV66qmnNHLkSI0dO9bmCs1Su3ZtdejQQXFxcQoODra7HGPdddddqlOnjqZPny5/f39t2bJFZcuW1UMPPaRhw4ZddlZzuDp16pR+/vlnSVKtWrWsuchMRoABbnBOp1NjxozR1KlTrcP0Pj4+Gj16tOLi4myuzjx+fn7atGmTatWqZXcpRgsICNDatWtVt25dBQQEKCUlRfXr19fatWvVt29f6w7VuHH9+X9hAdwQHA6HXn75ZR09elRr1qzRli1bdOzYMcLLVfrHP/6h5cuX212G8cqWLWsdZQ0KCtKBAwcknb8dS1pamp2l4TrBERgYZerUqRo8eLB8fHw0derUS47lN3LY4fTp07r33nt10003XfTcLP4ui6ZDhw7q16+fHnzwQQ0aNEhbt27V0KFD9cEHH+j48eNau3at3SXCZgQYGCU8PFwbNmxQ5cqVC510+nsOh0O//PJLCVZm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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -506,27 +506,42 @@
                 "## Outliers\n",
                 "\n",
                 "The `get_outliers()` function detects outliers, returning the indices of outlier points."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "The default method for get_outliers has changed to \"mah\". Please specify the method explicitly to avoid this warning.\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/plain": [
-                            "array([ 301,  302,  303,  415,  416,  417,  418,  799,  896,  897,  898,\n",
-                            "        899,  996,  997, 1843, 2278, 2279, 2280, 2638, 2639, 2640, 2641,\n",
-                            "       2642, 2643, 2920, 2921, 2922, 3070, 3071, 3074, 3075, 3076, 3078,\n",
-                            "       3079, 3080, 3212, 3580, 3581, 3582, 3583])"
+                            "array([ 262,  289,  301,  302,  303,  304,  310,  311,  312,  414,  415,\n",
+                            "        416,  417,  418,  797,  798,  799,  800,  896,  897,  898,  899,\n",
+                            "        900,  901,  933,  934,  935,  936,  937,  995,  996,  997,  998,\n",
+                            "        999, 1352, 1353, 1354, 1357, 1358, 1359, 1360, 1841, 1842, 1843,\n",
+                            "       1844, 1845, 1846, 2177, 2178, 2179, 2180, 2186, 2187, 2188, 2189,\n",
+                            "       2276, 2277, 2278, 2279, 2280, 2281, 2282, 2637, 2638, 2639, 2640,\n",
+                            "       2641, 2642, 2643, 2644, 2645, 2738, 2739, 2740, 2741, 2742, 2919,\n",
+                            "       2920, 2921, 2922, 2923, 2951, 2952, 2953, 2959, 2960, 3069, 3070,\n",
+                            "       3071, 3073, 3074, 3075, 3076, 3077, 3078, 3079, 3080, 3081, 3082,\n",
+                            "       3083, 3209, 3210, 3211, 3212, 3213, 3214, 3579, 3580, 3581, 3582,\n",
+                            "       3583, 3584, 3585, 3643, 3644, 3645, 3804, 3805, 3806, 3934, 3935,\n",
+                            "       3936, 3937, 3938])"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "outliers = rf.get_outliers(df['GR'])\n",
                 "outliers"
@@ -537,40 +552,30 @@
             "metadata": {},
             "source": [
                 "We can see where these lie in the distribution:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "use_inf_as_na option is deprecated and will be removed in a future version. Convert inf values to NaN before operating instead.\n",
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "use_inf_as_na option is deprecated and will be removed in a future version. Convert inf values to NaN before operating instead.\n"
-                    ]
-                },
-                {
                     "data": {
                         "text/plain": [
                             "<Axes: xlabel='GR', ylabel='Density'>"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAlEAAAGwCAYAAACJjDBkAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8g+/7EAAAACXBIWXMAAA9hAAAPYQGoP6dpAABpMElEQVR4nO3de1xUdf4/8NfMwMxwv8MAIqCQeEFQFEQtayOxbIsuu+ZWml/TdnPbiq72K21rv9lN1y5urltpfcs0W7Mys4guliIKindRlIsKw1UYGO4zn98fw4yNogICZ2Z4PR+PeajnfM4575nD5eXnfM7nyIQQAkRERETULXKpCyAiIiKyRwxRRERERD3AEEVERETUAwxRRERERD3AEEVERETUAwxRRERERD3AEEVERETUA05SF+DIjEYjSktL4eHhAZlMJnU5RERE1AVCCNTX1yMkJARy+cX7mxii+lBpaSnCwsKkLoOIiIh64NSpUxg0aNBF1zNE9SEPDw8AppPg6ekpcTVERETUFTqdDmFhYZbf4xfDENWHzJfwPD09GaKIiIjszOWG4nBgOREREVEPMEQRERER9QBDFBEREVEPMEQRERER9QBDFBEREVEPMEQRERER9QBDFBEREVEPMEQRERER9QBDFBEREVEPMEQRERER9QBDFBEREVEPMEQRERER9QBDFBEREVEPMEQRERER9QBDFBEREVEPMEQRERER9QBDFBEREVEPMEQRERER9QBDFBEREVEPMEQRERER9QBDFBEREVEPMEQRERER9QBDFBEREVEPMEQRERER9QBDFBEREVEPMEQRERER9QBDFBEREVEPMEQRERER9QBDFBEREVEPOEldABFJp7XdiANnalHf3I52g8D4CF94uTpLXRYRkV2QvCdqxYoViIiIgFqtRlJSEnbt2nXJ9hs2bEBMTAzUajViY2OxZcsWq/UbN27E1KlT4efnB5lMhry8PKv1RUVFkMlknb42bNhgadfZ+nXr1vXa+yaS2v7TtbjpzV9wxztZuG/1btz/YQ4mv/ID3vj+OOqb26Quj4jI5kkaotavX4/09HQsXrwYe/bsQVxcHFJTU1FRUdFp+x07dmDmzJmYO3cu9u7di7S0NKSlpeHgwYOWNnq9HpMnT8Yrr7zS6T7CwsJQVlZm9fr73/8Od3d33HjjjVZtV69ebdUuLS2t1947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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -589,55 +594,30 @@
                 "By default it uses an [**isolation forest**](https://scikit-learn.org/stable/modules/outlier_detection.html#isolation-forest) to detect the outliers at the 99% confidence level, but you can also opt to use **local outlier factor**, **elliptic envelope**, or **Mahalanobis distance**, setting the confidence level to choose how many outliers you will see, or (equivalently) setting the `threshold` to the number of standard deviations away from the mean you regard as signal.\n",
                 "\n",
                 "The function accepts univariate or multivariate data:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "use_inf_as_na option is deprecated and will be removed in a future version. Convert inf values to NaN before operating instead.\n",
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "use_inf_as_na option is deprecated and will be removed in a future version. Convert inf values to NaN before operating instead.\n"
-                    ]
-                },
-                {
                     "data": {
                         "text/plain": [
-                            "<seaborn.axisgrid.JointGrid at 0x7fcc8f97d490>"
+                            "<seaborn.axisgrid.JointGrid at 0x132e88110>"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "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bvLz82loaKCgoMB3n++++w6Px+P7hd4TlZaWUltbS1xcHNBz5klRFO68804+/vhjvvvuO9LS0vyuH83PW35+Phs2bPALKhcuXIjFYiErK6trXkgX+Lm5CmTt2rUAfu+rnjBXPUJ3Z473FO+9955iMBiUN954Q9m8ebNyyy23KGFhYX6nH3qa+++/X1m8eLGye/du5ccff1TGjRunREZGKlVVVYqiKMptt92mJCcnK999952yevVqJT8/X8nPz+/mUXeN5uZmpbCwUCksLFQA5ZlnnlEKCwuV4uJiRVEU5cknn1TCwsKU+fPnK+vXr1cuvvhiJS0tTWlvb/c9x8SJE5XBgwcrK1asUH744QelV69eypQpU7rrJZ0QR5qn5uZm5YEHHlCWLVum7N69W/nmm2+UIUOGKL169VJsNpvvOXrCPN1+++1KaGiosnjxYqW8vNz31dbW5rvPz/28uVwuJTs7Wxk/fryydu1aZcGCBUpUVJTy8MMPd8dLOmF+bq527NihPP7448rq1auV3bt3K/Pnz1fS09OV0aNH+56jp8xVTyBBUhf697//rSQnJyt6vV4ZPny4snz58u4eUre66qqrlLi4OEWv1ysJCQnKVVddpezYscN3vb29XbnjjjsUq9WqmEwm5ZJLLlHKy8u7ccRdZ9GiRQrQ4Wv69OmKonjLAPzxj39UYmJiFIPBoIwdO1YpKirye47a2lplypQpitlsViwWi3LDDTcozc3N3fBqTpwjzVNbW5syfvx4JSoqStHpdEpKSooyY8aMDn+Y9IR5CjRHgPL666/77nM0P2979uxRJk2apBiNRiUyMlK5//77FafT2cWv5sT6ubnau3evMnr0aCU8PFwxGAxKZmam8uCDDyqNjY1+z9MT5qonUCmKonTdupUQQgghxKlBcpKEEEIIIQKQIEkIIYQQIgAJkoQQQgghApAgSQghhBAiAAmShBBCCCECkCBJCCGEECIACZKEEEIIIQKQIEkIIYQQIgAJkoQQQgghApAgSQjRqYqKCu6++24yMzMJCgoiJiaGUaNG8eKLL9LW1gZAamoqKpUKlUqFyWQiJyeHV155pZtHLoQQx07b3QMQQpycdu3axahRowgLC+Nvf/sbOTk5GAwGNmzYwMsvv0xCQgIXXXQRAI8//jgzZsygra2NefPmMWPGDBISEpg0aVI3vwohhPj1pHebECKgiRMnsmnTJrZu3UpwcHCH64qioFKpSE1N5Z577uGee+7xXYuIiGD69Ok888wzXThiIYQ4vmS7TQjRQW1tLV9//TUzZ84MGCABqFSqDrd5PB4+/PBD6uvr0ev1J3qYQghxQkmQJIToYMeOHSiKQp8+ffxuj4yMxGw2Yzabeeihh3y3P/TQQ5jNZgwGA5dffjlWq5Wbb765q4cthBDHlQRJQoijtnLlStauXUv//v2x2+2+2x988EHWrl3Ld999R15eHv/617/IzMzsxpEKIcSxk8RtIUQHmZmZqFQqioqK/G5PT08HwGg0+t0eGRlJZmYmmZmZzJs3j5ycHHJzc8nKyuqyMQshxPEmK0lCiA4iIiI499xzef7552ltbf1Fj01KSuKqq67i4YcfPkGjE0KIriFBkhAioBdeeAGXy0Vubi7vv/8+W7ZsoaioiHfeeYetW7ei0Wg6fezdd9/Np59+yurVq7twxEIIcXxJCQAhRKfKy8v529/+xueff05paSkGg4GsrCyuuOIK7rjjDkwmU8ASAOAtIaBWq/niiy+6Z/BCCHGMJEgSQgghhAhAttuEEEIIIQKQIEkIIYQQIgAJkoQQQgghApAgSQghhBAiAAmShBBCCCECkCBJCCGEECIACZKEEEIIIQKQIEkIIYQQIgAJkoQQQgghApAgSQghhBAiAAmShBBCCCECkCBJCCGEECKA/w+NoHu8bW0e9gAAAABJRU5ErkJggg==",
                         "text/plain": [
                             "<Figure size 600x600 with 3 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -655,15 +635,15 @@
             "metadata": {},
             "source": [
                 "A helper function can compute the number of expected outliers, given the dataset size and assuming a Gaussian distribution of samples."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "We have 80 outliers, but expect:\n"
@@ -671,15 +651,15 @@
                 },
                 {
                     "data": {
                         "text/plain": [
                             "44"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "print(f\"We have {len(outliers)} outliers, but expect:\")\n",
                 "rf.expected_outliers(*df[features].shape, threshold=3)"
@@ -690,73 +670,64 @@
             "metadata": {},
             "source": [
                 "So we have more than expected &mdash; because the distribution of GR has a lot of clipped samples at a value of 200. A dataset with truncated tails will have fewer than expected outliers; we can test this directly with the `has_outliers()` function, which compares the results of `expected_outliers()` with `get_outliers()`:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "100"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import numpy as np\n",
                 "\n",
                 "data = np.random.normal(size=10_000)\n",
                 "\n",
                 "rf.expected_outliers(len(data), d=1, p=0.99)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Truncate\n",
                 "data = data[(-2.5 < data) & (data <  2.5)]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "use_inf_as_na option is deprecated and will be removed in a future version. Convert inf values to NaN before operating instead.\n",
-                        "The figure layout has changed to tight\n"
-                    ]
-                },
-                {
                     "data": {
                         "text/plain": [
-                            "<seaborn.axisgrid.FacetGrid at 0x7fcc8d7666d0>"
+                            "<seaborn.axisgrid.FacetGrid at 0x134fab650>"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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+uijevLJJzV79myLJrdGW54vAIGVlZWl48ePa+PGjVaPYqlOcYGNru4nP/mJnn322WbXDB061Pfv8vJyTZo0Sffff7/eeeeddp7OPK19vtAUl4dFe5szZ462b9+ugwcPasCAAVaPYyki3Qn07dtXffv2bdHasrIyTZo0SWPGjNH69esVHNz1Dqa05vnCtf778rCNJ0A1Xh52zpw51g6HDs3r9So7O1tbtmzR/v37NWTIEKtHshyR7kLKysr00EMPadCgQXrjjTd04cIF3zZeAV1faWmpLl68qNLSUnk8Hh09elSSdMcddyg8PNza4SzE5WFb7vLlyzpz5ozv/rlz53T06FFFR0dr4MCBFk5mnqysLOXn5+v9999XRESE7xwHm82mXr16WTydRbzoMtavX++VdN0bri8jI+O6z9e+ffusHs1yq1at8g4cONAbEhLive+++7xFRUVWj2Skffv2Xfd/QxkZGVaPZpwb/fdp/fr1Vo9mGT4nDQCAobreG5IAAHQQRBoAAEMRaQAADEWkAQAwFJEGAMBQRBoAAEMRaQAADEWkAQAwFJEGAMBQRBoAAEMRaQAADPX/AH3We9VkYukRAAAAAElFTkSuQmCC",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 500x500 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -770,24 +741,24 @@
             "metadata": {},
             "source": [
                 "This truncated normal distribution has no outliers (there are only about 60, compared to the 100 we expect at this confidence level of 99% on this dataset of 10,000 records)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "False"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "rf.has_outliers(data, p=0.99)"
             ]
@@ -799,59 +770,50 @@
                 "## Clipping\n",
                 "\n",
                 "If a feature has been clipped, it will have multiple instances at its min and/or max value. There are legitimate reasons why this might happen, for example the feature may be naturally bounded (e.g. porosity is always greater than 0), or the feature may have been deliberately clipped as part of the data preparation process."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "True"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "rf.is_clipped(df['GR'])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "use_inf_as_na option is deprecated and will be removed in a future version. Convert inf values to NaN before operating instead.\n",
-                        "The figure layout has changed to tight\n"
-                    ]
-                },
-                {
                     "data": {
                         "text/plain": [
-                            "<seaborn.axisgrid.FacetGrid at 0x7fcc8d7521d0>"
+                            "<seaborn.axisgrid.FacetGrid at 0x134fcc0e0>"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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TEzU8uXLOXEMl6Sph3iUl3/vx2oAwCzNCmm3233BM6QlqVOnTnK73S0uCu1HUw/xeGs2f/QBaL+aFdI33XSTZs+erbVr1youLk6S9O2332ru3LkaN26cTwtE8GpqK1liSxkAGtOskP7zn/+s2267TX379lV8fLwk6fjx4xoyZIhee+01nxaI4NXUVrLEljIANKZZIR0fH69PP/1UW7du1RdffCFJGjx4sFJSUnxaHAAA7dklnd29fft2JSYmyuVyyWaz6eabb9asWbM0a9YsjRo1Stdcc40+/vjj1qoVAIB25ZJC+rnnntOMGTMUHh5+QVtERIR+97vfaenSpT4rDgCA9uySQvp///d/NX78+AbbU1NTVVBQ0OKiAADAJR6TLi0trffSK8+Hdeyo7777rsVFofVx5jUAmO+SQvryyy/XoUOHNGDAgHrbDxw4oNjYWJ8UhtbFmdcAYL5L2t19yy23aP78+Tp37twFbT/88IOeeOIJ/epXv/JZcQAAtGeXtCX9+OOP6+2339bVV1+tmTNnauDAgZKkL774QsuXL1ddXZ3+5V/+pVUKBQCgvbmkLemYmBjt2rVLQ4YMUU5Oju644w7dcccdeuyxxzRkyBDt3LlTMTExF/15H330kW699VbFxcXJZrNp/fr1Xu333nuvbDab1/TzE9fKy8s1depUhYeHKzIyUtOnT9fp06cvZVgAABjpkm9mkpCQoE2bNun777/XkSNHZFmWrrrqKl122WWXvPAzZ85o2LBhuv/++zVp0qR6+4wfP16rVq3yvA4LC/Nqnzp1qkpKSrRlyxbV1NTovvvu04MPPqg1a9Zccj0AAJikWXcck6TLLrtMo0aNatHC09PTlZ6e3mifsLAw2e32ets+//xzbd68WXv37tXIkSMlSS+88IJuueUW/elPf/LcVxwAgGDUrOdJ+1Nubq6io6M1cOBAPfzwwzp58qSnLT8/X5GRkZ6AlqSUlBSFhIRoz549DX5mVVWVXC6X1wQAgGmMDunx48frr3/9q7Zt26Z/+7d/U15entLT01VXVydJcjqdio6O9npPx44dFRUVJWcj1wAvXrxYERERnun8Q0IAADBJs3d3+8PkyZM9PyclJWno0KG68sorlZub26JHYubk5CgrK8vz2uVyEdQAAOMYvSX9c/3791evXr105MgRSZLdbldZWZlXn9raWpWX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",
+                        "image/png": "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TEzU8uXLOXEMl6Sph3iUl3/vx2oAwCzNCmm3233BM6QlqVOnTnK73S0uCu1HUw/xeGs2f/QBaL+aFdI33XSTZs+erbVr1youLk6S9O2332ru3LkaN26cTwtE8GpqK1liSxkAGtOskP7zn/+s2267TX379lV8fLwk6fjx4xoyZIhee+01nxaI4NXUVrLEljIANKZZIR0fH69PP/1UW7du1RdffCFJGjx4sFJSUnxaHAAA7dklnd29fft2JSYmyuVyyWaz6eabb9asWbM0a9YsjRo1Stdcc40+/vjj1qoVAIB25ZJC+rnnntOMGTMUHh5+QVtERIR+97vfaenSpT4rDgCA9uySQvp///d/NX78+AbbU1NTVVBQ0OKiAADAJR6TLi0trffSK8+Hdeyo7777rsVFofVx5jUAmO+SQvryyy/XoUOHNGDAgHrbDxw4oNjYWJ8UhtbFmdcAYL5L2t19yy23aP78+Tp37twFbT/88IOeeOIJ/epXv/JZcQAAtGeXtCX9+OOP6+2339bVV1+tmTNnauDAgZKkL774QsuXL1ddXZ3+5V/+pVUKBQCgvbmkLemYmBjt2rVLQ4YMUU5Oju644w7dcccdeuyxxzRkyBDt3LlTMTExF/15H330kW699VbFxcXJZrNp/fr1Xu333nuvbDab1/TzE9fKy8s1depUhYeHKzIyUtOnT9fp06cvZVgAABjpkm9mkpCQoE2bNun777/XkSNHZFmWrrrqKl122WWXvPAzZ85o2LBhuv/++zVp0qR6+4wfP16rVq3yvA4LC/Nqnzp1qkpKSrRlyxbV1NTovvvu04MPPqg1a9Zccj0AAJikWXcck6TLLrtMo0aNatHC09PTlZ6e3mifsLAw2e32ets+//xzbd68WXv37tXIkSMlSS+88IJuueUW/elPf/LcVxwAgGDUrOdJ+1Nubq6io6M1cOBAPfzwwzp58qSnLT8/X5GRkZ6AlqSUlBSFhIRoz549DX5mVVWVXC6X1wQAgGmMDunx48frr3/9q7Zt26Z/+7d/U15entLT01VXVydJcjqdio6O9npPx44dFRUVJWcj1wAvXrxYERERnun8Q0IAADBJs3d3+8PkyZM9PyclJWno0KG68sorlZub26JHYubk5CgrK8vz2uVyEdQAAOMYvSX9c/3791evXr105MgRSZLdbldZWZlXn9raWpWX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",
                         "text/plain": [
                             "<Figure size 500x500 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -885,24 +847,24 @@
                 "The name is returned, along with the shape parameters (if any), location and scale.\n",
                 "\n",
                 "In spite of the outliers, we find that the distribution of GR values is nearly normal:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 20,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "Distribution(name='norm', shape=[], loc=64.36789939485628, scale=28.411020184908292)"
                         ]
                     },
-                    "execution_count": 19,
+                    "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "rf.best_distribution(df['GR'])"
             ]
@@ -912,59 +874,50 @@
             "metadata": {},
             "source": [
                 "In contrast, the PHIND data is skewed andbest modeled by the [Gumbel distribution](https://en.wikipedia.org/wiki/Gumbel_distribution)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 21,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "Distribution(name='gumbel_r', shape=[], loc=10.040572536302586, scale=4.93432972751726)"
                         ]
                     },
-                    "execution_count": 20,
+                    "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "rf.best_distribution(df['PHIND'])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 22,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "use_inf_as_na option is deprecated and will be removed in a future version. Convert inf values to NaN before operating instead.\n",
-                        "The figure layout has changed to tight\n"
-                    ]
-                },
-                {
                     "data": {
                         "text/plain": [
-                            "<seaborn.axisgrid.FacetGrid at 0x7fcc8fa18310>"
+                            "<seaborn.axisgrid.FacetGrid at 0x1350c3e90>"
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": 22,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAekAAAHpCAYAAACmzsSXAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8g+/7EAAAACXBIWXMAAA9hAAAPYQGoP6dpAAAq5klEQVR4nO3df1RU953/8dcogj+BoMJAFcUmEVHRrD9wGpsapeKPpFpJjrY2MbtGNy6aKClr2Pg73SXVbmLjom6PrbZnQ23siaayiUZRMalolIRV/MFRDwYSGYhxBbUBFe73j3yddeKIAYeZD/B8nHPP4d7PZ+6870eOL+5vm2VZlgAAgHHa+LsAAADgGSENAIChCGkAAAxFSAMAYChCGgAAQxHSAAAYipAGAMBQhLQky7JUVVUlbhkHAJiEkJZ0+fJlhYSE6PLly/4uBQAAF0IaAABDEdIAABiKkAYAwFCENAAAhiKkAQAwFCENAIChCGkAAAxFSAMAYChCGgAAQxHSAAAYipAGAMBQhDQAAIYipAEAMBQhDQCAoQhpAAAMRUgDAGAov4b0unXrFB8fr+DgYAUHB8vhcOi9995ztVdXVyslJUVdu3ZV586dlZycrPLycrd1lJSUaOLEierYsaPCw8OVlpamGzdu+HpTAADwOr+GdI8ePfTqq68qPz9fR44c0ejRozVp0iQdP35ckrRgwQJt375dW7ZsUW5urs6fP68pU6a4Pl9bW6uJEyfq2rVrOnDggH7/+99r06ZNWrJkib82CQAAr7FZlmX5u4hbhYWFadWqVXriiSfUvXt3ZWVl6YknnpAknTp1Sv369VNeXp5GjBih9957T4899pjOnz+viIgISdL69eu1cOFCffHFFwoMDPT4HTU1NaqpqXHNV1VVqWfPnqqsrFRwcHDTbyQAAN9CgL8LuKm2tlZbtmzR1atX5XA4lJ+fr+vXrysxMdHVJzY2VtHR0a6QzsvL08CBA10BLUlJSUmaM2eOjh8/roceesjjd2VkZGj58uVNvk1omKTHJqus4oLHtsjwbtqZvc23BQGAn/k9pI8dOyaHw6Hq6mp17txZW7duVVxcnAoKChQYGKjQ0FC3/hEREXI6nZIkp9PpFtA322+23Ul6erpSU1Nd8zf3pOFfZRUXFPfsKo9tJzak+bgaAPA/v4d03759VVBQoMrKSv35z3/WjBkzlJub26TfGRQUpKCgoCb9DgAA7pXfQzowMFD333+/JGnIkCE6fPiwfv3rX2vq1Km6du2aLl265LY3XV5eLrvdLkmy2+366KOP3NZ38+rvm30AAGiujLtPuq6uTjU1NRoyZIjatWunnJwcV1tRUZFKSkrkcDgkSQ6HQ8eOHVNFRYWrz65duxQcHKy4uDif1w4AgDf5dU86PT1d48ePV3R0tC5fvqysrCzt27dPO3fuVEhIiGbOnKnU1FSFhYUpODhY8+bNk8Ph0IgRIyRJY8eOVVxcnJ566imtXLlSTqdTixYtUkpKCoezAQDNnl9DuqKiQk8//bTKysoUEhKi+Ph47dy5Uz/84Q8lSa+//rratGmj5ORk1dTUKCkpSWvXrnV9vm3btsrOztacOXPkcDjUqVMnzZgxQytWrPDXJgEA4DXG3SftD1VVVQoJCeE+aT+LHz6y3qu7j370oY8rAgD/Mu6cNAAA+BohDQCAoQhpAAAMRUgDAGAoQhoAAEMR0gAAGIqQBgDAUIQ0AACGIqQBADAUIQ0AgKEIaQAADEVIAwBgKEIaAABDEdIAABiKkAYAwFCENAAAhiKkAQAwFCENAIChCGkAAAxFSAMAYChCGgAAQxHSAAAYipAGAMBQhDQAAIYipAEAMFSAvwtA65L02GSVVVzw2PZpaanifFwPAJiMkIZH9YVpZHg37cze1qj1llVcUNyzqzy2nX35yUatEwBaKkIaHtUXpic2pPm4GgBonTgnDQCAoQhpAAAMRUgDAGAoQhoAAEMR0gAAGIqru9Fg584VK374SI9t93J7FgDAHSGNBqu1bNyeBQA+wOFuAAAMRUgDAGAoDne3YjxHGwDMRki3Ys3pOdpcrAagNSKk0SxwsRqA1ohz0gAAGIqQBgDAUIQ0AACGIqQBADAUIQ0AgKEIaQAADEVIAwBgKEIaAABDEdIAABiKkAYAwFCENAAAhiKkAQAwFCENAIChCGkAAAxFSAMAYChCGgAAQxHSAAAYyq8hnZGRoWHDhqlLly4KDw/X5MmTVVRU5NZn1KhRstlsbtNzzz3n1qekpEQTJ05Ux44dFR4errS0NN24ccOXmwIAgNcF+PPLc3NzlZKSomHDhunGjRv6l3/5F40dO1YnTpxQp06dXP1mzZqlFStWuOY7duzo+rm2tlYTJ06U3W7XgQMHVFZWpqefflrt2rXTv/3bv/l0ewAA8Ca/hvSOHTvc5jdt2qTw8HDl5+frkUcecS3v2LGj7Ha7x3W8//77OnHihHbv3q2IiAgNHjxYr7zyihYuXKhly5YpMDDwts/U1NSopqbGNV9VVeWlLQIAwHuMOiddWVkpSQoLC3Nb/uabb6pbt24aMGCA0tPT9be//c3VlpeXp4EDByoiIsK1LCkpSVVVVTp+/LjH78nIyFBISIhr6tmzZxNsDQAA98ave9K3qqur0/z58/Xwww9rwIABruU//elP1atXL0VFReno0aNauHChioqK9Pbbb0uSnE6nW0BLcs07nU6P35Wenq7U1FTXfFVVFUENADCOMSGdkpKiwsJCffjhh27LZ8+e7fp54MCBioyM1JgxY3T27Fl997vfbdR3BQUFKSgo6J7qBQCgqRlxuHvu3LnKzs7W3r171aNHj3r7JiQkSJLOnDkjSbLb7SovL3frc3P+TuexAQBoDvwa0pZlae7cudq6dav27NmjmJiYu36moKBAkhQZGSlJcjgcOnbsmCoqKlx9du3apeDgYMXFxTVJ3QAA+IJfD3enpKQoKytL77zzjrp06eI6hxwSEqIOHTro7NmzysrK0oQJE9S1a1cdPXpUCxYs0COPPKL4+HhJ0tixYxUXF6ennnpKK1eulNPp1KJFi5SSksIhbQBAs+bXPel169apsrJSo0aNUmRkpGv605/+JEkKDAzU7t27NXbsWMXGxurFF19UcnKytm/f7lpH27ZtlZ2drbZt28rhcOhnP/uZnn76abf7qgEAaI78uidtWVa97T179lRubu5d19OrVy+9++673ioLAAAjGHHhGAAAuB0hDQCAoQhpAAAMRUgDAGAoQhoAAEMR0gAAGIqQBgDAUIQ0AACGIqQBADAUIQ0AgKEIaQAADEVIAwBgKEIaAABDEdIAABiKkAYAwFCENAAAhiKkAQAwFCENAIChCGkAAAwV4O8CgHt17lyx4oeP9NgWGd5NO7O3+bYgAPASQhrNXq1lU9yzqzy2ndiQ5uNqAMB7ONwNAIChCGkAAAxFSAMAYChCGgAAQxHSAAAYiqu74VX13Q4lSZ+WlirOh/UAQHNGSMOr6rsdSpLOvvykD6sBgOaNw90AABiKkAYAwFCENAAAhiKkAQAwFCENAIChCGkAAAxFSAMAYChCGgAAQxHSAAAYipAGAMBQhDQAAIYipAEAMBQhDQCAoQhpAAAMRUgDAGAoQhoAAEMR0gAAGIqQBgDAUAH+LgBoSufOFSt++EiPbZHh3bQze5tvCwKABiCk0aLVWjbFPbvKY9uJDWk+rgYAGobD3QAAGIqQBgDAUIQ0AACGIqQBADAUIQ0AgKEIaQAADEVIAwBgKEIaAABD+TWkMzIyNGzYMHXp0kXh4eGaPHmyioqK3PpUV1crJSVFXbt2VefOnZWcnKzy8nK3PiUlJZo4caI6duyo8PBwpaWl6caNG77cFAAAvM6vIZ2bm6uUlBQdPHhQu3bt0vXr1zV27FhdvXrV1WfBggXavn27tmzZotzcXJ0/f15TpkxxtdfW1mrixIm6du2aDhw4oN///vfatGmTlixZ4o9NAgDAa/z6WNAdO3a4zW/atEnh4eHKz8/XI488osrKSv32t79VVlaWRo8eLUnauHGj+vXrp4MHD2rEiBF6//33deLECe3evVsREREaPHiwXnnlFS1cuFDLli1TYGCgPzYNAIB7ZtQ56crKSklSWFiYJCk/P1/Xr19XYmKiq09sbKyio6OVl5cnScrLy9PAgQMVERHh6pOUlKSqqiodP37c4/fU1NSoqqrKbQIAwDTGhHRdXZ3mz5+vhx9+WAMGDJAkOZ1OBQYGKjQ01K1vRESEnE6nq8+tAX2z/WabJxkZGQoJCXFNPXv29PLWAABw74wJ6ZSUFBUWFmrz5s1N/l3p6emqrKx0TaWlpU3+nQAANJQRr6qcO3eusrOztX//fvXo0cO13G6369q1a7p06ZLb3nR5ebnsdrurz0cffeS2vptXf9/s801BQUEKCgry8lYAAOBdft2TtixLc+fO1datW7Vnzx7FxMS4tQ8ZMkTt2rVTTk6Oa1lRUZFKSkrkcDgkSQ6HQ8eOHVNFRYWrz65duxQcHKy4uDjfbAgAAE3Ar3vSKSkpysrK0jvvvKMuXbq4ziGHhISoQ4cOCgkJ0cyZM5WamqqwsDAFBwdr3rx5cjgcGjFihCRp7NixiouL01NPPaWVK1fK6XRq0aJFSklJYW8ZANCs+TWk161bJ0kaNWqU2/KNGzfqmWeekSS9/vrratOmjZKTk1VTU6OkpCStXbvW1bdt27bKzs7WnDlz5HA41KlTJ82YMUMrVqzw1WYAANAk/BrSlmXdtU/79u2VmZmpzMzMO/bp1auX3n33XW+WBgCA3xlzdTcAAHBHSAMAYChCGgAAQxHSAAAYipAGAMBQhDQAAIYy4rGgaDpJj01WWcUFj22flpaKZ7IBgLkI6RaurOKC4p5d5bHt7MtP+rgaAEBDcLgbAABDEdIAABiKkAYAwFCENAAAhiKkAQAwFCENAIChCGkAAAxFSAMAYChCGgAAQxHSAAAYipAGAMBQhDQAAIYipAEAMBQhDQCAoQhpAAAMRUgDAGAoQhoAAEMR0gAAGIqQBgDAUAH+LgDwl3PnihU/fKTHtsjwbtqZvc23BQHANxDSaLVqLZvinl3lse3EhjQfVwMAt+NwNwAAhiKkAQAwFCENAIChCGkAAAzVqJDu06ePvvzyy9uWX7p0SX369LnnogAAQCND+ty5c6qtrb1teU1NjT7//PN7LgoAADTwFqy//OUvrp937typkJAQ13xtba1ycnLUu3dvrxUHAEBr1qCQnjx5siTJZrNpxowZbm3t2rVT79699e///u9eKw4AgNasQSFdV1cnSYqJidHhw4fVrVu3JikKAAA08oljxcXF3q4DAAB8Q6MfC5qTk6OcnBxVVFS49rBv+t3vfnfPhQEA0No1KqSXL1+uFStWaOjQoYqMjJTNZvN2XQAAtHqNCun169dr06ZNeuqpp7xdDwAA+P8adZ/0tWvX9L3vfc/btQAAgFs0KqSfffZZZWVlebsWAABwi0Yd7q6urtZvfvMb7d69W/Hx8WrXrp1b+2uvveaV4gAAaM0aFdJHjx7V4MGDJUmFhYVubVxEBgCAdzQqpPfu3evtOgCjnDtXrPjhIz22RYZ3087sbb4tCECr1Oj7pGGOpMcmq6zigse2T0tLFefjelqCWsumuGdXeWw7sSHNx9UAaK0aFdKPPvpovYe19+zZ0+iC0HBlFRfuGChnX37Sx9UAALylUSF983z0TdevX1dBQYEKCwtve/EGAABonEaF9Ouvv+5x+bJly3TlypV7KggAAHytUfdJ38nPfvYzntsNAICXeDWk8/Ly1L59e2+uEgCAVqtRh7unTJniNm9ZlsrKynTkyBEtXrzYK4UBANDaNSqkQ0JC3ObbtGmjvn37asWKFRo7dqxXCgMAoLVrVEhv3LjR23UAAIBvuKeHmeTn5+vkyZOSpP79++uhhx7ySlEAAKCRF45VVFRo9OjRGjZsmJ5//nk9//zzGjJkiMaMGaMvvvjiW69n//79evzxxxUVFSWbzaZt27a5tT/zzDOy2Wxu07hx49z6XLx4UdOnT1dwcLBCQ0M1c+ZMbgMDALQIjQrpefPm6fLlyzp+/LguXryoixcvqrCwUFVVVXr++ee/9XquXr2qQYMGKTMz8459xo0bp7KyMtf0xz/+0a19+vTpOn78uHbt2qXs7Gzt379fs2fPbsxmAQBglEYd7t6xY4d2796tfv36uZbFxcUpMzOzQReOjR8/XuPHj6+3T1BQkOx2u8e2kydPaseOHTp8+LCGDh0qSVqzZo0mTJigX/3qV4qKivrWtQAAYJpG7UnX1dXd9g5pSWrXrp3q6uruuahb7du3T+Hh4erbt6/mzJmjL7/80tWWl5en0NBQV0BLUmJiotq0aaNDhw7dcZ01NTWqqqpymwAAME2jQnr06NF64YUXdP78edeyzz//XAsWLNCYMWO8Vty4ceP0hz/8QTk5OfrlL3+p3NxcjR8/XrW1tZIkp9Op8PBwt88EBAQoLCxMTqfzjuvNyMhQSEiIa+rZs6fXagYAwFsadbj7P/7jP/SjH/1IvXv3dgVcaWmpBgwYoP/6r//yWnHTpk1z/Txw4EDFx8fru9/9rvbt23dPfwykp6crNTXVNV9VVUVQAwCM06iQ7tmzpz7++GPt3r1bp06dkiT169dPiYmJXi3um/r06aNu3brpzJkzGjNmjOx2uyoqKtz63LhxQxcvXrzjeWzp6/PcQUFBTVorAAD3qkGHu/fs2aO4uDhVVVXJZrPphz/8oebNm6d58+Zp2LBh6t+/vz744IOmqlWfffaZvvzyS0VGRkqSHA6HLl26pPz8fLca6+rqlJCQ0GR1AADgCw0K6dWrV2vWrFkKDg6+rS0kJET/+I//qNdee+1br+/KlSsqKChQQUGBJKm4uFgFBQUqKSnRlStXlJaWpoMHD+rcuXPKycnRpEmTdP/99yspKUnS13vv48aN06xZs/TRRx/pr3/9q+bOnatp06ZxZTcAoNlrUEj/z//8z20PE7nV2LFj3fZq7+bIkSN66KGHXE8qS01N1UMPPaQlS5aobdu2Onr0qH70ox/pwQcf1MyZMzVkyBB98MEHboeq33zzTcXGxmrMmDGaMGGCRo4cqd/85jcN2SwAAIzUoHPS5eXlHm+9cq0sIKBBTxwbNWqULMu6Y/vOnTvvuo6wsDBlZWV96+8EAKC5aNCe9He+8x0VFhbesf3o0aOu88UAAODeNCikJ0yYoMWLF6u6uvq2tq+++kpLly7VY4895rXiAABozRp0uHvRokV6++239eCDD2ru3Lnq27evJOnUqVPKzMxUbW2tXn755SYpFACA1qZBIR0REaEDBw5ozpw5Sk9Pd51PttlsSkpKUmZmpiIiIpqkUAAAWpsGP8ykV69eevfdd/W///u/OnPmjCzL0gMPPKD77ruvKeoDAKDVatQTxyTpvvvu07Bhw7xZCwAAuEWjQxporc6dK1b88JEe2yLDu2ln9jbfFgSgxSKkgQaqtWyKe3aVx7YTG9J8XA2AlqxRr6oEAABNj5AGAMBQhDQAAIYipAEAMBQhDQCAoQhpAAAMRUgDAGAoQhoAAEMR0gAAGIqQBgDAUIQ0AACGIqQBADAUIQ0AgKEIaQAADEVIAwBgKEIaAABDEdIAABiKkAYAwFCENAAAhiKkAQAwFCENAIChCGkAAAxFSAMAYChCGgAAQxHSAAAYipAGAMBQhDQAAIYipAEAMBQhDQCAoQhpAAAMRUgDAGAoQhoAAEMR0gAAGIqQBgDAUIQ0AACGIqQBADAUIQ0AgKEIaQAADEVIAwBgKEIaAABDEdIAABiKkAYAwFCENAAAhiKkAQAwFCENAIChCGkAAAxFSAMAYChCGgAAQxHSAAAYyq8hvX//fj3++OOKioqSzWbTtm3b3Noty9KSJUsUGRmpDh06KDExUadPn3brc/HiRU2fPl3BwcEKDQ3VzJkzdeXKFR9uBQAATcOvIX316lUNGjRImZmZHttXrlypN954Q+vXr9ehQ4fUqVMnJSUlqbq62tVn+vTpOn78uHbt2qXs7Gzt379fs2fP9tUmAADQZAL8+eXjx4/X+PHjPbZZlqXVq1dr0aJFmjRpkiTpD3/4gyIiIrRt2zZNmzZNJ0+e1I4dO3T48GENHTpUkrRmzRpNmDBBv/rVrxQVFeVx3TU1NaqpqXHNV1VVeXnLAM+SHpussooLHtsiw7tpZ/Y23xYEwGh+Den6FBcXy+l0KjEx0bUsJCRECQkJysvL07Rp05SXl6fQ0FBXQEtSYmKi2rRpo0OHDunHP/6xx3VnZGRo+fLlTb4NwDeVVVxQ3LOrPLad2JDm42oAmM7YC8ecTqckKSIiwm15RESEq83pdCo8PNytPSAgQGFhYa4+nqSnp6uystI1lZaWerl6AADunbF70k0pKChIQUFB/i4DAIB6GbsnbbfbJUnl5eVuy8vLy11tdrtdFRUVbu03btzQxYsXXX0AAGiujA3pmJgY2e125eTkuJZVVVXp0KFDcjgckiSHw6FLly4pPz/f1WfPnj2qq6tTQkKCz2sGAMCb/Hq4+8qVKzpz5oxrvri4WAUFBQoLC1N0dLTmz5+vX/ziF3rggQcUExOjxYsXKyoqSpMnT5Yk9evXT+PGjdOsWbO0fv16Xb9+XXPnztW0adPueGU3AADNhV9D+siRI3r00Udd86mpqZKkGTNmaNOmTfrnf/5nXb16VbNnz9alS5c0cuRI7dixQ+3bt3d95s0339TcuXM1ZswYtWnTRsnJyXrjjTd8vi1Nrb5bdz4tLVWcj+sBADQ9v4b0qFGjZFnWHdttNptWrFihFStW3LFPWFiYsrKymqI8o9R3687Zl5/0cTUAAF8w9pw0AACtHSENAIChCGkAAAxFSAMAYKhW+cQxoKmcO1es+OEj79jOlfgAGoKQBryo1rLd8Sp8iSvxATQMh7sBADAUIQ0AgKEIaQAADEVIAwBgKEIaAABDEdIAABiKkAYAwFCENAAAhiKkAQAwFCENAIChCGkAAAxFSAMAYChCGgAAQ/EWLMAQ9b3mMjK8m3Zmb/NtQQD8jpAGDFHfay5PbEjzcTUATMDhbgAADEVIAwBgKEIaAABDEdIAABiKkAYAwFCENAAAhiKkAQAwFCENAIChCGkAAAxFSAMAYChCGgAAQxHSAAAYipAGAMBQhDQAAIYipAEAMBQhDQCAoQhpAAAMRUgDAGAoQhoAAEMR0gAAGIqQBgDAUIQ0AACGIqQBADAUIQ0AgKEIaQAADEVIAwBgKEIaAABDEdIAABiKkAYAwFCENAAAhiKkAQAwVIC/CwBwd+fOFSt++EiPbZHh3bQze5tvCwLgE4Q00AzUWjbFPbvKY9uJDWk+rgaAr3C4GwAAQxHSAAAYyuiQXrZsmWw2m9sUGxvraq+urlZKSoq6du2qzp07Kzk5WeXl5X6sGAAA7zE6pCWpf//+Kisrc00ffvihq23BggXavn27tmzZotzcXJ0/f15TpkzxY7UAAHiP8ReOBQQEyG6337a8srJSv/3tb5WVlaXRo0dLkjZu3Kh+/frp4MGDGjFihK9LBQDAq4zfkz59+rSioqLUp08fTZ8+XSUlJZKk/Px8Xb9+XYmJia6+sbGxio6OVl5eXr3rrKmpUVVVldsEAIBpjN6TTkhI0KZNm9S3b1+VlZVp+fLl+v73v6/CwkI5nU4FBgYqNDTU7TMRERFyOp31rjcjI0PLly9vwsobJ+mxySqruOCx7dPSUsX5uB4AgH8ZHdLjx493/RwfH6+EhAT16tVLb731ljp06NDo9aanpys1NdU1X1VVpZ49e95Trd5QVnHhjvfCnn35SR9XAwDwN+MPd98qNDRUDz74oM6cOSO73a5r167p0qVLbn3Ky8s9nsO+VVBQkIKDg90mAABM06xC+sqVKzp79qwiIyM1ZMgQtWvXTjk5Oa72oqIilZSUyOFw+LFKAAC8w+jD3T//+c/1+OOPq1evXjp//ryWLl2qtm3b6ic/+YlCQkI0c+ZMpaamKiwsTMHBwZo3b54cDgdXdgMAWgSjQ/qzzz7TT37yE3355Zfq3r27Ro4cqYMHD6p79+6SpNdff11t2rRRcnKyampqlJSUpLVr1/q5agAAvMPokN68eXO97e3bt1dmZqYyMzN9VBEAAL7TrM5JAwDQmhDSAAAYipAGAMBQhDQAAIYipAEAMBQhDQCAoQhpAAAMZfR90gDuTX1vVosM76ad2dt8WxCABiGkgRasvjerndiQ5uNqADQUh7sBADAUIQ0AgKE43A20UufOFSt++EiPbZyvBsxASAOtVK1l43w1YDgOdwMAYChCGgAAQ3G4G2jm6ju3/GlpqeJ8XA8A7yGkgWauvnPLZ19+0sfVAPAmDncDAGAoQhoAAEMR0gAAGIqQBgDAUIQ0AACGIqQBADAUIQ0AgKEIaQAADEVIAwBgKEIaAABDEdIAABiKZ3cDuE19L+2IDO+mndnbfFsQ0EoR0gBuU99LO05sSPNxNUDrxeFuAAAMxZ40AK9JemyyyioueGzjMDnQcIQ0AK8pq7hwx8Pk7y564o7nuSVCHPCEkAbgE/Wd55Y41w14wjlpAAAMxZ40gAap7/asT0tLFefjeoCWjJAG0CD1HbY++/KTPq4GaNk43A0AgKEIaQAADMXhbgCtEvd0ozkgpAEYrykCtb57urkdDKYgpAEYj0BFa8U5aQAADMWeNIBmjddqoiUjpAEYobEPSeG1mmjJCGkARuAhKcDtCGkfq+8qVR6pCAC4FSHtY/VdpcreAgDgVlzdDQCAodiTBoAGqO+UVdn5zxUZ9R2PbfdypTlPR2u9CGkAaIC7nbJq7JXmd7teZfzyzY1aL5o3QhoAvsEf78zmehV4QkgDwDdwOxhMQUgDaLH8sUcMeBMhDaDFag17xPX9IdJUF7LBdwhpAGjG7vaHCI9Mbd64TxoAAEO1mD3pzMxMrVq1Sk6nU4MGDdKaNWs0fPhwf5cFAJLqPywtNZ9z5E11nzj3gnvWIkL6T3/6k1JTU7V+/XolJCRo9erVSkpKUlFRkcLDw/1dHgDUe1ha8v058sa+4rOp7hOvb731fbaxfzQ0ts3XfzC0iJB+7bXXNGvWLP393/+9JGn9+vX67//+b/3ud7/TSy+95NNa6vuFkZrPX8sAWrb6/mh4d9ETRl0Vf7er9O/0oJf6/mhobJuvz+U3+5C+du2a8vPzlZ6e7lrWpk0bJSYmKi8vz+NnampqVFNT45qvrKyUJFVVVd1zPZ+VORX79C/u2H5mxdO6/tVVj21WXV2LbjOtHrbfnDbT6mnt23+j1tID05d5bGvs/2G1tTfq/T+2tvaGT+tpbNvdtqOhunTpIpvNducOVjP3+eefW5KsAwcOuC1PS0uzhg8f7vEzS5cutSQxMTExMTH5daqsrKw345r9nnRjpKenKzU11TVfV1enixcvqmvXrvX/RfMNVVVV6tmzp0pLSxUcHNwUpTZ7jNHdMUZ3xxjVj/G5O1PHqEuXLvW2N/uQ7tatm9q2bavy8nK35eXl5bLb7R4/ExQUpKCgILdloaGhja4hODjYqH90EzFGd8cY3R1jVD/G5+6a2xg1+/ukAwMDNWTIEOXk5LiW1dXVKScnRw6Hw4+VAQBwb5r9nrQkpaamasaMGRo6dKiGDx+u1atX6+rVq66rvQEAaI5aREhPnTpVX3zxhZYsWSKn06nBgwdrx44dioiIaNLvDQoK0tKlS287dI7/wxjdHWN0d4xR/Rifu2uuY2SzLMvydxEAAOB2zf6cNAAALRUhDQCAoQhpAAAMRUgDAGAoQvoeZGZmqnfv3mrfvr0SEhL00Ucf+bskv9m/f78ef/xxRUVFyWazadu2bW7tlmVpyZIlioyMVIcOHZSYmKjTp0/7p1g/yMjI0LBhw9SlSxeFh4dr8uTJKioqcutTXV2tlJQUde3aVZ07d1ZycvJtD+lpydatW6f4+HjXwyYcDofee+89V3trH59vevXVV2Wz2TR//nzXstY+RsuWLZPNZnObYmNjXe3NcXwI6Ua6+XrMpUuX6uOPP9agQYOUlJSkiooKf5fmF1evXtWgQYOUmZnpsX3lypV64403tH79eh06dEidOnVSUlKSqqurfVypf+Tm5iolJUUHDx7Url27dP36dY0dO1ZXr/7fQ/wXLFig7du3a8uWLcrNzdX58+c1ZcoUP1btWz169NCrr76q/Px8HTlyRKNHj9akSZN0/PhxSYzPrQ4fPqz//M//VHx8vNtyxkjq37+/ysrKXNOHH37oamuW4+Od11y0PsOHD7dSUlJc87W1tVZUVJSVkZHhx6rMIMnaunWra76urs6y2+3WqlWrXMsuXbpkBQUFWX/84x/9UKH/VVRUWJKs3Nxcy7K+Ho927dpZW7ZscfU5efKkJcnKy8vzV5l+d99991kbNmxgfG5x+fJl64EHHrB27dpl/eAHP7BeeOEFy7L4HbKsr1+eNGjQII9tzXV82JNuhJuvx0xMTHQtu9vrMVuz4uJiOZ1Ot/EKCQlRQkJCqx2vm69HDQsLkyTl5+fr+vXrbmMUGxur6OjoVjlGtbW12rx5s65evSqHw8H43CIlJUUTJ050GwuJ36GbTp8+raioKPXp00fTp09XSUmJpOY7Pi3iiWO+duHCBdXW1t72RLOIiAidOnXKT1WZy+l0SpLH8brZ1prU1dVp/vz5evjhhzVgwABJX49RYGDgbS96aW1jdOzYMTkcDlVXV6tz587aunWr4uLiVFBQwPhI2rx5sz7++GMdPnz4tjZ+h6SEhARt2rRJffv2VVlZmZYvX67vf//7KiwsbLbjQ0gDPpaSkqLCwkK3c2X4Wt++fVVQUKDKykr9+c9/1owZM5Sbm+vvsoxQWlqqF154Qbt27VL79u39XY6Rxo8f7/o5Pj5eCQkJ6tWrl9566y116NDBj5U1Hoe7G6Exr8dszW6OCeMlzZ07V9nZ2dq7d6969OjhWm6323Xt2jVdunTJrX9rG6PAwEDdf//9GjJkiDIyMjRo0CD9+te/Znz09eHaiooK/d3f/Z0CAgIUEBCg3NxcvfHGGwoICFBERESrH6NvCg0N1YMPPqgzZ840298hQroReD1mw8TExMhut7uNV1VVlQ4dOtRqxsuyLM2dO1dbt27Vnj17FBMT49Y+ZMgQtWvXzm2MioqKVFJS0mrGyJO6ujrV1NQwPpLGjBmjY8eOqaCgwDUNHTpU06dPd/3c2sfom65cuaKzZ88qMjKy+f4O+fvKteZq8+bNVlBQkLVp0ybrxIkT1uzZs63Q0FDL6XT6uzS/uHz5svXJJ59Yn3zyiSXJeu2116xPPvnE+vTTTy3LsqxXX33VCg0Ntd555x3r6NGj1qRJk6yYmBjrq6++8nPlvjFnzhwrJCTE2rdvn1VWVuaa/va3v7n6PPfcc1Z0dLS1Z88e68iRI5bD4bAcDocfq/atl156ycrNzbWKi4uto0ePWi+99JJls9ms999/37IsxseTW6/utizG6MUXX7T27dtnFRcXW3/961+txMREq1u3blZFRYVlWc1zfAjpe7BmzRorOjraCgwMtIYPH24dPHjQ3yX5zd69ey1Jt00zZsywLOvr27AWL15sRUREWEFBQdaYMWOsoqIi/xbtQ57GRpK1ceNGV5+vvvrK+qd/+ifrvvvuszp27Gj9+Mc/tsrKyvxXtI/9wz/8g9WrVy8rMDDQ6t69uzVmzBhXQFsW4+PJN0O6tY/R1KlTrcjISCswMND6zne+Y02dOtU6c+aMq705jg+vqgQAwFCckwYAwFCENAAAhiKkAQAwFCENAIChCGkAAAxFSAMAYChCGgAAQxHSAAAYipAGAMBQhDTQijzzzDOy2Wyy2WyuN06tWLFCN27c0L59+2Sz2W57S5Ak9e7dW6tXr6533maz6eDBg26fmz9/vkaNGuWaX7Zsmev7AwIC1K1bNz3yyCNavXq1ampqvLy1QPNHSAOtzLhx41RWVqbTp0/rxRdf1LJly7Rq1ap7Xm/79u21cOHCu/br37+/ysrKVFJSor179+rJJ59URkaGvve97+ny5cv3XAfQkhDSQCsTFBQku92uXr16ac6cOUpMTNRf/vKXe17v7NmzdfDgQb377rv19gsICJDdbldUVJQGDhyoefPmKTc3V4WFhfrlL395z3UALQkhDbRyHTp00LVr1+55PTExMXruueeUnp6uurq6Bn02NjZW48eP19tvv33PdQAtCSENtFKWZWn37t3auXOnRo8e7Vreo0cPde7c2W0qKSn5VutctGiRiouL9eabbza4ntjYWJ07d67BnwNasgB/FwDAt7Kzs9W5c2ddv35ddXV1+ulPf6ply5bp8OHDkqQPPvhAXbp0cfvMrRd/1ad79+76+c9/riVLlmjq1KkNqsuyLNlstgZ9BmjpCGmglXn00Ue1bt06BQYGKioqSgEB7v8NxMTEKDQ01G3ZN/vUJzU1VWvXrtXatWsbVNfJkycVExPToM8ALR2Hu4FWplOnTrr//vsVHR3doPD9tjp37qzFixfrX//1X7/11dqnTp3Sjh07lJyc7PV6gOaMkAbgdbNnz1ZISIiysrJua7tx44acTqfOnz+vY8eOac2aNfrBD36gwYMHKy0tzQ/VAuYipAF4Xbt27fTKK6+ourr6trbjx48rMjJS0dHRGjVqlN566y2lp6frgw8+UOfOnf1QLWAum2VZlr+LAAAAt2NPGgAAQxHSAAAYipAGAMBQhDQAAIYipAEAMBQhDQCAoQhpAAAMRUgDAGAoQhoAAEMR0gAAGIqQBgDAUP8Ps7KfTa3ldgEAAAAASUVORK5CYII=",
                         "text/plain": [
                             "<Figure size 500x500 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -982,15 +935,15 @@
                 "We'd often like to test the implicit assumption that our data are 'identically distributed' across various groups, with respect to both the labels and the features.\n",
                 "\n",
                 "`redflag.wasserstein()` facilitates calculating the first Wasserstein distance (aka earth-mover's distance) between groups, e.g. between train and test datasets. It returns a score for each feature; scores greater than 1 can be interpreted as substantial differences in the distribution."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 23,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[0.25985545, 0.28404634, 0.49139232, 0.33701782],\n",
                             "       [0.22736457, 0.13473663, 0.33672956, 0.20969657],\n",
@@ -999,15 +952,15 @@
                             "       [0.19913347, 0.21828753, 0.26995735, 0.33063277],\n",
                             "       [0.24612402, 0.23889923, 0.26699721, 0.2350674 ],\n",
                             "       [0.20666445, 0.44112543, 0.16229232, 0.63527036],\n",
                             "       [0.18187639, 0.34992043, 0.19400917, 0.74988182],\n",
                             "       [0.31761526, 0.27206283, 0.30255291, 0.24779581]])"
                         ]
                     },
-                    "execution_count": 22,
+                    "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "wells = df['Well Name']\n",
                 "features = ['GR', 'RHOB', 'ILD_log10', 'PE']\n",
@@ -1021,30 +974,30 @@
             "metadata": {},
             "source": [
                 "You could plot this as a heatmap:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 24,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<Axes: >"
                         ]
                     },
-                    "execution_count": 23,
+                    "execution_count": 24,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 640x480 with 2 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -1053,29 +1006,29 @@
                 "sns.heatmap(w, yticklabels=np.unique(wells), xticklabels=features)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This shows us that the distributions of the PE log in well indices 6 and 7 are somewhat different and may be anomalous. It also suggests that the CROSS H CATTLE well is different from the others."
+                "This shows us that the distributions of the PE log in the wells SHANKLE and SHRIMPLIN are somewhat different and may be anomalous. It also suggests that the CROSS H CATTLE well is different from the others, because all of the logs' distributions have relatively high distance to those in the other wells."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Already split out group arrays\n",
                 "\n",
                 "If you have groups that are already split out, e.g. train and test datasets:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 25,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from sklearn.model_selection import train_test_split\n",
                 "from sklearn.preprocessing import StandardScaler\n",
                 "\n",
                 "X_train, X_ = train_test_split(df[features], test_size=0.4, random_state=42)\n",
@@ -1096,26 +1049,26 @@
             "metadata": {},
             "source": [
                 "In this case, you can pass them into the function as a list or tuple:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 26,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[0.03860982, 0.02506236, 0.04321734, 0.03437337],\n",
                             "       [0.04402681, 0.02528225, 0.0385111 , 0.05694201],\n",
                             "       [0.04388196, 0.049464  , 0.05560379, 0.04002712]])"
                         ]
                     },
-                    "execution_count": 25,
+                    "execution_count": 26,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "rf.wasserstein([X_train, X_val, X_test])"
             ]
@@ -1134,24 +1087,24 @@
                 "## Independence assumption\n",
                 "\n",
                 "If a feature is correlated to lagged (shifted) versions of itself, then the dataset may be ordered by that feature, or the records may not be independent. If several features are correlated to themselves, then the data instances may not be independent."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 27,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "True"
                         ]
                     },
-                    "execution_count": 26,
+                    "execution_count": 27,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "rf.is_correlated(df['GR'])"
             ]
@@ -1161,50 +1114,57 @@
             "metadata": {},
             "source": [
                 "This is order-dependent. That is, shuffling the data removes the correlation, but does not mean the records are independent."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 28,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "False"
                         ]
                     },
-                    "execution_count": 27,
+                    "execution_count": 28,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "gr = df['GR'].to_numpy(copy=True)\n",
                 "np.random.shuffle(gr)\n",
                 "rf.is_correlated(gr)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "See [the Tutorial](Tutorial.ipynb) for more about this function."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "## Feature importance\n",
                 "\n",
                 "We'd like to know which features are the most important.\n",
                 "\n",
                 "`redflag` trains a series of models on your data, assessing which features are most important. It then normalizes and averages the results. \n",
                 "\n",
                 "To serve as a 'control', let's add a column of small random numbers that we know is not useful. We'd expect this column to come out with very low importance (i.e. close to zero)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 29,
             "metadata": {},
             "outputs": [],
             "source": [
                 "df['Random'] = np.random.normal(scale=0.1, size=len(df))\n",
                 "df['Constant'] = -1"
             ]
         },
@@ -1213,24 +1173,24 @@
             "metadata": {},
             "source": [
                 "First, a **classification task**. Imagine we're trying to predict lithology from well logs. Which are the most important logs?"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 30,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "array([0.28547027, 0.28342166, 0.32686674, 0.09151957, 0.        ])"
+                            "array([0.38370363, 0.25078171, 0.29262816, 0.0728865 , 0.        ])"
                         ]
                     },
-                    "execution_count": 29,
+                    "execution_count": 30,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "features = ['GR', 'ILD_log10', 'PE', 'Random', 'Constant']\n",
                 "\n",
@@ -1248,24 +1208,24 @@
                 "This tells us that the most important features are, in order: PE, ILD, GR, with the random and constant variables unsurprisingly useless.\n",
                 "\n",
                 "There's a function to help us decide which are the least important features; it returns the indices of the least useful features, in order (least useful first):"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": 31,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([4, 3])"
                         ]
                     },
-                    "execution_count": 30,
+                    "execution_count": 31,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "rf.least_important_features(importances)"
             ]
@@ -1275,24 +1235,24 @@
             "metadata": {},
             "source": [
                 "And a complementary function reporting the most important:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": 32,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "array([2, 0, 1, 3])"
+                            "array([0, 2, 1])"
                         ]
                     },
-                    "execution_count": 31,
+                    "execution_count": 32,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "rf.most_important_features(importances)"
             ]
@@ -1302,24 +1262,24 @@
             "metadata": {},
             "source": [
                 "Now we'll look at a **regression task**. We'll try to predict RHOB from the other logs (including the dummy variables). The function guesses that this is a regression task:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": 33,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "array([0.08772211, 0.35620195, 0.53119438, 0.02488155, 0.        ])"
+                            "array([0.09183559, 0.36166718, 0.51483025, 0.03166698, 0.        ])"
                         ]
                     },
-                    "execution_count": 32,
+                    "execution_count": 33,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "features = ['GR', 'ILD_log10', 'PE', 'Random', 'Constant']\n",
                 "\n",
@@ -1329,15 +1289,17 @@
                 "rf.feature_importances(X, y)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The most predictive features are PE and ILD, with GR substantially less important. Again, the random and constant variables are the least important feature."
+                "The most predictive features are PE and ILD, with GR substantially less important. Again, the random and constant variables are the least important feature.\n",
+                "\n",
+                "See [the Tutorial](Tutorial.ipynb) for more about this function."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "redflag",
             "language": "python",
@@ -1349,15 +1311,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.5"
+            "version": "3.12.0"
         },
         "vscode": {
             "interpreter": {
                 "hash": "3ad933181bd8a04b432d3370b9dc3b0662ad032c4dfaa4e4f1596c548f763858"
             }
         }
     },
```

### Comparing `redflag-0.4.2rc1/docs/notebooks/Tutorial.ipynb` & `redflag-0.5.0rc1/docs/notebooks/Tutorial.ipynb`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9837127701228311%*

 * *Differences: {"'cells'": "{1: {'execution_count': 6, 'outputs': {0: {'execution_count': 6}}}, 3: "*

 * *            "{'execution_count': 7, 'outputs': {0: {'execution_count': 7}}}, 5: "*

 * *            "{'execution_count': 8, 'outputs': {0: {'data': {'text/plain': "*

 * *            '["array([\'ms\', \'ss\'], dtype=\'<U2\')"]}, \'execution_count\': 8}}}, 7: '*

 * *            "{'execution_count': 9, 'outputs': {0: {'data': {'text/plain': "*

 * *            '["\'0.4.2rc2.dev14+g54704af.d20240421\'"]}, \'execution_count\': 9}}}, 9: '*

 * *            […]*

```diff
@@ -18,24 +18,24 @@
                 "## A simple ML workflow\n",
                 "\n",
                 "First, let's see how we can burn ourselves:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array(['ss', 'ss', 'ss', 'ms', 'ms', 'ss'], dtype='<U2')"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "X = [[19], [23], [35], [64], [59], [31]]  # The smallest gamma-ray log.\n",
                 "y = ['ss', 'ss', 'ss', 'ms', 'ms', 'ss']\n",
@@ -54,24 +54,24 @@
                 "So far so good. We're predicting on the training data, but everything is at least working.\n",
                 "\n",
                 "Now someone tells us we should scale our training data."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array(['ms', 'ms', 'ms', 'ms', 'ms', 'ms'], dtype='<U2')"
                         ]
                     },
-                    "execution_count": 2,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from sklearn.preprocessing import StandardScaler\n",
                 "\n",
@@ -90,24 +90,24 @@
                 "Easily done. There are lots of people on Stack Overflow and Cross Validated wondering why all their predictions are the same. It's often because they've done something like this.\n",
                 "\n",
                 "Even easier is this common pattern:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "array(['ss', 'ss'], dtype='<U2')"
+                            "array(['ms', 'ss'], dtype='<U2')"
                         ]
                     },
-                    "execution_count": 3,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from sklearn.model_selection import train_test_split\n",
                 "\n",
@@ -140,24 +140,24 @@
                 "## A quick look at `redflag`\n",
                 "\n",
                 "First make sure you have `redflag` v0.1.10 at least, otherwise do `python -m pip install -U redflag` in your environment."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'0.3.1.dev18+g743d11f.d20230927'"
+                            "'0.4.2rc2.dev14+g54704af.d20240421'"
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import redflag as rf\n",
                 "\n",
@@ -169,15 +169,15 @@
             "metadata": {},
             "source": [
                 "## Load some data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -346,37 +346,37 @@
                             "0  2393.499945  siliciclastic           True  \n",
                             "1  2416.119814  siliciclastic           True  \n",
                             "2  2404.576056  siliciclastic           True  \n",
                             "3  2393.249071  siliciclastic           True  \n",
                             "4  2382.602601  siliciclastic           True  "
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import pandas as pd\n",
                 "\n",
-                "df = pd.read_csv('https://raw.githubusercontent.com/scienxlab/datasets/main/kgs/Panoma_training_data.csv')\n",
+                "df = pd.read_csv('https://raw.githubusercontent.com/scienxlab/datasets/main/kgs/panoma-training-data.csv')\n",
                 "\n",
                 "df.head()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "For later use, I'm going to add a spurious column to the data:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
                 "rng = np.random.default_rng(42)\n",
                 "\n",
@@ -398,24 +398,24 @@
                 "- Feature importance\n",
                 "\n",
                 "Let's look at imbalance first."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "3.378593040846633"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "rf.imbalance_degree(df['Lithology'])"
             ]
@@ -439,24 +439,24 @@
             "metadata": {},
             "source": [
                 "We can get the minority classes, which are those with fewer samples than expected. These are returned in order, smallest first:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array(['dolomite', 'sandstone', 'mudstone', 'wackestone'], dtype='<U10')"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "rf.minority_classes(df['Lithology'])"
             ]
@@ -468,121 +468,116 @@
                 "## Clipping\n",
                 "\n",
                 "If a feature has been clipped, it will have multiple instances at its min and/or max value. There are legitimate reasons why this might happen, for example the feature may be naturally bounded (e.g. porosity is always greater than 0), or the feature may have been deliberately clipped as part of the data preparation process."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "True"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "rf.is_clipped(df['GR'])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "use_inf_as_na option is deprecated and will be removed in a future version. Convert inf values to NaN before operating instead.\n",
-                        "The figure layout has changed to tight\n"
-                    ]
-                },
-                {
                     "data": {
                         "text/plain": [
-                            "<seaborn.axisgrid.FacetGrid at 0x7efc2f1dff10>"
+                            "<seaborn.axisgrid.FacetGrid at 0x12d8028d0>"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAekAAAHpCAYAAACmzsSXAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8pXeV/AAAACXBIWXMAAA9hAAAPYQGoP6dpAAAuT0lEQVR4nO3de3BUZZ7/8U8HSLgmMUDSiYYAokAkIAMYenFclJgQGRWJs8Iwioo4OoEBokw2rqDClrg4C64Owlqj4JSCDq7igohyS5QlIESyXNSUsGhQ0olFTJqL5Nbn94dD/2zJBZJO99PJ+1V1qtLnebrP98mB/uTcbZZlWQIAAMYJCXQBAACgfoQ0AACGIqQBADAUIQ0AgKEIaQAADEVIAwBgKEIaAABDEdKSLMuSy+USl4wDAExCSEs6deqUIiIidOrUqUCXAgCAByENAIChCGkAAAxFSAMAYChCGgAAQxHSAAAYipAGAMBQhDQAAIYipAEAMBQhDQCAoQhpAAAMRUgDAGAoQhoAAEMR0gAAGIqQBgDAUIQ0AACGIqQBADAUIQ0AgKEIaQAADEVIAwBgqI6BLgAItOGjRqvE6Wy0T6zdrv17d/upIgD4ESGNdq/E6dTY+Wsb7ZO7aIqfqgGA/4/d3QAAGIqQBgDAUIQ0AACGIqQBADAUIQ0AgKEIaQAADEVIAwBgKEIaAABDEdIAABiKkAYAwFCENAAAhiKkAQAwFCENAIChCGkAAAxFSAMAYChCGgAAQxHSAAAYipAGAMBQhDQAAIYipAEAMBQhDQCAoQhpAAAMRUgDAGAoQhoAAEMFNKRXrFihoUOHKjw8XOHh4XI4HHr//fc97efOnVNmZqZ69uyp7t27KyMjQ6WlpV6fUVxcrAkTJqhr166Kjo7WvHnzVFtb6++hAADgcwEN6SuuuELPPPOMCgoKtG/fPt100026/fbbdfjwYUnS3LlztWHDBq1bt055eXk6ceKEJk2a5Hl/XV2dJkyYoOrqau3atUuvvvqqVq9erQULFgRqSAAA+IzNsiwr0EX8VFRUlJ599lndeeed6t27t9asWaM777xTkvTFF19o8ODBys/P1+jRo/X+++/rV7/6lU6cOKGYmBhJ0sqVK5Wdna3vvvtOoaGh9S6jqqpKVVVVntcul0vx8fGqrKxUeHh46w8SRrHH99XY+Wsb7ZO7aIqcx7/yT0EA8HfGHJOuq6vTG2+8oTNnzsjhcKigoEA1NTVKSUnx9Bk0aJD69Omj/Px8SVJ+fr6SkpI8AS1JaWlpcrlcnq3x+ixevFgRERGeKT4+vvUGBgBAMwU8pA8ePKju3bsrLCxMDz30kN555x0lJibK6XQqNDRUkZGRXv1jYmLkdDolSU6n0yugz7efb2tITk6OKisrPdPx48d9OygAAHygY6ALGDhwoAoLC1VZWam33npL06ZNU15eXqsuMywsTGFhYa26DAAAWirgIR0aGqoBAwZIkkaMGKG9e/fqP/7jP3TXXXepurpaFRUVXlvTpaWlstvtkiS73a5PPvnE6/POn/19vg8AAMEq4Lu7f87tdquqqkojRoxQp06dtG3bNk9bUVGRiouL5XA4JEkOh0MHDx5UWVmZp8+WLVsUHh6uxMREv9cOMw0fNVr2+L4NTuXl3we6RACoV0C3pHNycpSenq4+ffro1KlTWrNmjXJzc/XBBx8oIiJC06dPV1ZWlqKiohQeHq5Zs2bJ4XBo9OjRkqTU1FQlJibq7rvv1pIlS+R0OvX4448rMzOT3dnwKHE6Gz17+63ZqX6sBgAuXkBDuqysTPfcc49KSkoUERGhoUOH6oMPPtDNN98sSVq2bJlCQkKUkZGhqqoqpaWl6cUXX/S8v0OHDtq4caMefvhhORwOdevWTdOmTdPChQsDNSQAAHwmoCH98ssvN9reuXNnLV++XMuXL2+wT0JCgjZt2uTr0gAACDjjjkkDAIAfEdIAABiKkAYAwFCENAAAhiKkAQAwFCENAIChCGkAAAxFSAMAYChCGgAAQxHSAAAYipAGAMBQhDQAAIYipAEAMBQhDQCAoQhpAAAMRUgDAGAoQhoAAEMR0gAAGIqQBgDAUIQ0AACG6hjoAoBgUF5eLnt83wbbT7lc6hEe3mB7rN2u/Xt3t0JlANoyQhq4CG63pbHz1zbY/tbsVN3aSHvuoimtURaANo7d3QAAGIqQBgDAUIQ0AACG4pg0gt7wUaNV4nQ22F5e/r0fqwEA3yGkEfRKnM4mT+oCgGDE7m4AAAxFSAMAYChCGgAAQxHSAAAYipAGAMBQhDQAAIYipAEAMBQhDQCAoQhpAAAMRUgDAGAoQhoAAEMR0gAAGIqQBgDAUIQ0AACGIqQBADAUIQ0AgKEIaQAADEVIAwBgKEIaAABDEdIAABiKkAYAwFCENAAAhiKkAQAwFCENAIChCGkAAAwV0JBevHixRo0apR49eig6OloTJ05UUVGRV5+xY8fKZrN5TQ899JBXn+LiYk2YMEFdu3ZVdHS05s2bp9raWn8OBQAAn+sYyIXn5eUpMzNTo0aNUm1trR577DGlpqbqs88+U7du3Tz9ZsyYoYULF3ped+3a1fNzXV2dJkyYILvdrl27dqmkpET33HOPOnXqpKefftqv4wEAwJcCGtKbN2/2er169WpFR0eroKBAN9xwg2d+165dZbfb6/2MDz/8UJ999pm2bt2qmJgYXXvttVq0aJGys7P15JNPKjQ09IL3VFVVqaqqyvPa5XL5aEQAAPiOUcekKysrJUlRUVFe819//XX16tVLQ4YMUU5Ojs6ePetpy8/PV1JSkmJiYjzz0tLS5HK5dPjw4XqXs3jxYkVERHim+Pj4VhgNAAAtE9At6Z9yu92aM2eOxowZoyFDhnjm/+Y3v1FCQoLi4uJ04MABZWdnq6ioSG+//bYkyel0egW0JM9rp9NZ77JycnKUlZXlee1yuQhqAIBxjAnpzMxMHTp0SDt37vSa/+CDD3p+TkpKUmxsrMaNG6ejR4/qyiuvbNaywsLCFBYW1qJ6AQBobUbs7p45c6Y2btyoHTt26Iorrmi0b3JysiTpyJEjkiS73a7S0lKvPudfN3QcGwCAYBDQkLYsSzNnztQ777yj7du3q1+/fk2+p7CwUJIUGxsrSXI4HDp48KDKyso8fbZs2aLw8HAlJia2St0AAPhDQHd3Z2Zmas2aNXr33XfVo0cPzzHkiIgIdenSRUePHtWaNWt0yy23qGfPnjpw4IDmzp2rG264QUOHDpUkpaamKjExUXfffbeWLFkip9Opxx9/XJmZmezSBgAEtYBuSa9YsUKVlZUaO3asYmNjPdObb74pSQoNDdXWrVuVmpqqQYMG6ZFHHlFGRoY2bNjg+YwOHTpo48aN6tChgxwOh37729/qnnvu8bquGgCAYBTQLWnLshptj4+PV15eXpOfk5CQoE2bNvmqLAAAjGDEiWMAAOBChDQAAIYipAEAMBQhDQCAoQhpAAAMRUgDAGAoQhoAAEMR0gAAGIqQBgDAUIQ0AACGIqQBADAUIQ0AgKEIaQAADEVIAwBgqIA+qhJoL8rLy2WP79ton1i7Xfv37vZPQQCCAiEN+IHbbWns/LWN9sldNMVP1QAIFuzuBgDAUIQ0AACGIqQBADAUIQ0AgKEIaQAADEVIAwBgKEIaAABDEdIAABiKkAYAwFCENAAAhiKkAQAwFCENAIChCGkAAAxFSAMAYChCGgAAQxHSAAAYipAGAMBQhDQAAIYipAEAMBQhDQCAoQhpAAAMRUgDAGAoQhoAAEMR0gAAGKpjoAsA8KPy8nLZ4/s22B5rt2v/3t3+KwhAwBHSgCHcbktj569tsD130RQ/VgPABOzuBgDAUIQ0AACGYnc3jDZ81GiVOJ2N9ikv/95P1QCAfxHSMFqJ09nocVpJemt2qp+qAQD/Ync3AACGIqQBADAUIQ0AgKEIaQAADEVIAwBgKEIaAABDBTSkFy9erFGjRqlHjx6Kjo7WxIkTVVRU5NXn3LlzyszMVM+ePdW9e3dlZGSotLTUq09xcbEmTJigrl27Kjo6WvPmzVNtba0/hwIAgM8FNKTz8vKUmZmp3bt3a8uWLaqpqVFqaqrOnDnj6TN37lxt2LBB69atU15enk6cOKFJkyZ52uvq6jRhwgRVV1dr165devXVV7V69WotWLAgEEMCAMBnAnozk82bN3u9Xr16taKjo1VQUKAbbrhBlZWVevnll7VmzRrddNNNkqRVq1Zp8ODB2r17t0aPHq0PP/xQn332mbZu3aqYmBhde+21WrRokbKzs/Xkk08qNDT0guVWVVWpqqrK89rlcrXuQAEAaAajjklXVlZKkqKioiRJBQUFqqmpUUpKiqfPoEGD1KdPH+Xn50uS8vPzlZSUpJiYGE+ftLQ0uVwuHT58uN7lLF68WBEREZ4pPj6+tYYEAECzGRPSbrdbc+bM0ZgxYzRkyBBJktPpVGhoqCIjI736xsTEyPn3+zk7nU6vgD7ffr6tPjk5OaqsrPRMx48f9/FoAABoOWPu3Z2ZmalDhw5p586drb6ssLAwhYWFtfpyAABoCSO2pGfOnKmNGzdqx44duuKKKzzz7Xa7qqurVVFR4dW/tLRUdrvd0+fnZ3uff32+DwAAwSigIW1ZlmbOnKl33nlH27dvV79+/bzaR4wYoU6dOmnbtm2eeUVFRSouLpbD4ZAkORwOHTx4UGVlZZ4+W7ZsUXh4uBITE/0zEAAAWkFAd3dnZmZqzZo1evfdd9WjRw/PMeSIiAh16dJFERERmj59urKyshQVFaXw8HDNmjVLDodDo0ePliSlpqYqMTFRd999t5YsWSKn06nHH39cmZmZ7NIGAAS1gIb0ihUrJEljx471mr9q1Srde++9kqRly5YpJCREGRkZqqqqUlpaml588UVP3w4dOmjjxo16+OGH5XA41K1bN02bNk0LFy701zAAAGgVAQ1py7Ka7NO5c2ctX75cy5cvb7BPQkKCNm3a5MvSAAAIOCNOHAMAABcipAEAMBQhDQCAoQhpAAAMRUgDAGAoQhoAAEMR0gAAGIqQBgDAUIQ0AACGIqQBADAUIQ0AgKEIaQAADEVIAwBgqGaFdP/+/XXy5MkL5ldUVKh///4tLgoAADQzpL/66ivV1dVdML+qqkrffvtti4sCAACX+Dzp//7v//b8/MEHHygiIsLzuq6uTtu2bVPfvn19VhwAAO3ZJYX0xIkTJUk2m03Tpk3zauvUqZP69u2rf//3f/dZcQAAtGeXFNJut1uS1K9fP+3du1e9evVqlaIAAMAlhvR5x44d83UdAADgZ5oV0pK0bds2bdu2TWVlZZ4t7PNeeeWVFhcGAEB716yQfuqpp7Rw4UKNHDlSsbGxstlsvq4LAIB2r1khvXLlSq1evVp33323r+sBAAB/16zrpKurq/UP//APvq4FAAD8RLNC+oEHHtCaNWt8XQsAAPiJZu3uPnfunF566SVt3bpVQ4cOVadOnbzaly5d6pPiAABoz5oV0gcOHNC1114rSTp06JBXGyeRAQDgG80K6R07dvi6Dhho+KjRKnE6G2yPtdu1f+9uP1YEAO1Ls6+TRttX4nRq7Py1DbbnLprix2oAoP1pVkjfeOONje7W3r59e7MLAgAAP2pWSJ8/Hn1eTU2NCgsLdejQoQsevAEAAJqnWSG9bNmyeuc/+eSTOn36dIsKAgAAP2rWddIN+e1vf8t9uwEA8BGfhnR+fr46d+7sy48EAKDdatbu7kmTJnm9tixLJSUl2rdvn+bPn++TwgAAaO+aFdIRERFer0NCQjRw4EAtXLhQqampPikMAID2rlkhvWrVKl/XAQAAfqZFNzMpKCjQ559/Lkm65pprNHz4cJ8UBQAAmhnSZWVlmjx5snJzcxUZGSlJqqio0I033qg33nhDvXv39mWNAAC0S806u3vWrFk6deqUDh8+rPLycpWXl+vQoUNyuVz6wx/+4OsaAQBol5q1Jb1582Zt3bpVgwcP9sxLTEzU8uXLOXEMl6Sph3iUl3/vx2oAwCzNCmm3233BM6QlqVOnTnK73S0uCu1HUw/xeGs2f/QBaL+aFdI33XSTZs+erbVr1youLk6S9O2332ru3LkaN26cTwtE8GpqK1liSxkAGtOskP7zn/+s2267TX379lV8fLwk6fjx4xoyZIhee+01nxaI4NXUVrLEljIANKZZIR0fH69PP/1UW7du1RdffCFJGjx4sFJSUnxaHAAA7dklnd29fft2JSYmyuVyyWaz6eabb9asWbM0a9YsjRo1Stdcc40+/vjj1qoVAIB25ZJC+rnnntOMGTMUHh5+QVtERIR+97vfaenSpT4rDgCA9uySQvp///d/NX78+AbbU1NTVVBQ0OKiAADAJR6TLi0trffSK8+Hdeyo7777rsVFofVx5jUAmO+SQvryyy/XoUOHNGDAgHrbDxw4oNjYWJ8UhtbFmdcAYL5L2t19yy23aP78+Tp37twFbT/88IOeeOIJ/epXv/JZcQAAtGeXtCX9+OOP6+2339bVV1+tmTNnauDAgZKkL774QsuXL1ddXZ3+5V/+pVUKBQCgvbmkLemYmBjt2rVLQ4YMUU5Oju644w7dcccdeuyxxzRkyBDt3LlTMTExF/15H330kW699VbFxcXJZrNp/fr1Xu333nuvbDab1/TzE9fKy8s1depUhYeHKzIyUtOnT9fp06cvZVgAABjpkm9mkpCQoE2bNun777/XkSNHZFmWrrrqKl122WWXvPAzZ85o2LBhuv/++zVp0qR6+4wfP16rVq3yvA4LC/Nqnzp1qkpKSrRlyxbV1NTovvvu04MPPqg1a9Zccj0AAJikWXcck6TLLrtMo0aNatHC09PTlZ6e3mifsLAw2e32ets+//xzbd68WXv37tXIkSMlSS+88IJuueUW/elPf/LcVxwAgGDUrOdJ+1Nubq6io6M1cOBAPfzwwzp58qSnLT8/X5GRkZ6AlqSUlBSFhIRoz549DX5mVVWVXC6X1wQAgGmMDunx48frr3/9q7Zt26Z/+7d/U15entLT01VXVydJcjqdio6O9npPx44dFRUVJWcj1wAvXrxYERERnun8Q0IAADBJs3d3+8PkyZM9PyclJWno0KG68sorlZub26JHYubk5CgrK8vz2uVyEdQAAOMYvSX9c/3791evXr105MgRSZLdbldZWZlXn9raWpWX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",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 500x500 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "import seaborn as sns\n",
                 "\n",
-                "sns.displot(df['GR'])"
+                "sns.displot(df['GR'], lw=0, kde=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Independence assumption\n",
                 "\n",
-                "If a feature is correlated to lagged (shifted) versions of itself, then the dataset may be ordered by that feature, or the records may not be independent. If several features are correlated to themselves, then the data instances may not be independent."
+                "If a feature is correlated to lagged (shifted) versions of itself (i.e. 'autocorrelated'), then the dataset may be ordered by that feature, or the records may not be independent. For example, samples collected along a borehole are ordered by depth, and since the earth is organized, not random, this means that neighbouring samples will be correlated. Similarly, samples collected through time (the weather every hour) are often autocorrelated \u2014\u00a0you can predict the weather in an hour quite accurately by predicting it to be the same as the weather now.\n",
+                "\n",
+                "If several features are correlated to themselves, then the data instances may not be independent, breaking the IID assumption.\n",
+                "\n",
+                "Let's see if our gamma-ray data are autocorrelated:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "True"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "rf.is_correlated(df['GR'])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This is order-dependent. That is, shuffling the data removes the correlation:"
+                "The property of being detectably autocorrelated is order-dependent. That is, shuffling the data apparently removes the correlation because the samples are now in random order, so any sample-to-sample correspondence appears to be gone:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 20,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "False"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import numpy as np\n",
                 "\n",
@@ -591,53 +586,114 @@
                 "rf.is_correlated(gr)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "But this does not mean the records are independent &mdash; the only way around this issue is to split the data differently."
+                "But this does not mean the records are independent &mdash; only that you cannot tell that the records are autocorrelated.\n",
+                "\n",
+                "A common way to deal with autocorrelation is to split the data differently. For example, if you have 1000 samples from 100 locations (or patients), with about 10 samples from each location (or patient), then it may be better (i.e. fairer) to split _locations_ (or patients) into train and test sets, not _samples_. If you simply split samples, you will have records from inviduals locations (or patients) in both train and test, which is a common source of leakage."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Importance\n",
                 "\n",
                 "We might like to see which of our features are more useful. There's a function for that:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 21,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "array([0.41495144, 0.20256686, 0.3156612 , 0.0668205 ])"
+                            "array([0.40331202, 0.21106044, 0.31756576, 0.06806178])"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "features = ['GR', 'RHOB', 'PE', 'Noise']\n",
                 "\n",
                 "rf.feature_importances(df[features], df['Lithology'])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "As we'd hope, the `'Noise'` attribute is shown to be not very useful."
+                "As we'd hope, the `'Noise'` attribute is shown to be not very useful.\n",
+                "\n",
+                "The relative importance of your features (dataset columns) for making accurate predictions is not a perfectly well-defined thing. Accordingly, there are several ways to measure feature importance. The `feature_importances` function aggregates three different measures of feature importance. The underlying models it uses depend on the type of task.\n",
+                "\n",
+                "**Classification tasks** use the following:\n",
+                "\n",
+                "- A logistic regression model (using the absolute values of the coefficients).\n",
+                "- A random forest classifier (based on [mean reduction in impurity](https://scikit-learn.org/stable/auto_examples/ensemble/plot_forest_importances.html) or Gini importance).\n",
+                "- A K-nearest neighbours classifier (based on [permutation feature importance](https://scikit-learn.org/stable/modules/permutation_importance.html) with F1 score objective).\n",
+                "\n",
+                "**Regression tasks** are assessed with the following:\n",
+                "\n",
+                "- A linear regression (using the absolute coefficients).\n",
+                "- A random forest regressor, again using Gini importance.\n",
+                "- A K-nearest neighbours, again with permutation importance but with mean squared error objective.\n",
+                "\n",
+                "The aggregation function sums the normalized scores of the tests, and normalizes the result so that it sums to one."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Distributions\n",
+                "\n",
+                "A common problem in the search for models is a mismatch between the distribution of the training and validation datasets. This might happen for several reasons, for example because of how the dataset is organized, how it was split, or because of how it was handled after splitting. \n",
+                "\n",
+                "One simple error that can go unnoticed is fitting the model to scaled data, then forgetting to scale new data before prediction. Let's see how `redflag` checks for this, with the `wasserstein` function."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 22,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "array([[0.25985545, 0.28404634, 0.49139232, 0.33701782],\n",
+                            "       [0.22736457, 0.13473663, 0.33672956, 0.20969657],\n",
+                            "       [0.41216725, 0.34568777, 0.39729747, 0.48092099],\n",
+                            "       [0.0801856 , 0.10675027, 0.13740318, 0.10325295],\n",
+                            "       [0.19913347, 0.21828753, 0.26995735, 0.33063277],\n",
+                            "       [0.24612402, 0.23889923, 0.26699721, 0.2350674 ],\n",
+                            "       [0.20666445, 0.44112543, 0.16229232, 0.63527036],\n",
+                            "       [0.18187639, 0.34992043, 0.19400917, 0.74988182],\n",
+                            "       [0.31761526, 0.27206283, 0.30255291, 0.24779581]])"
+                        ]
+                    },
+                    "execution_count": 22,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "wells = df['Well Name']\n",
+                "features = ['GR', 'RHOB', 'ILD_log10', 'PE']\n",
+                "\n",
+                "w = rf.wasserstein(df[features], groups=wells, standardize=True)\n",
+                "w"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Pipelines"
@@ -652,15 +708,15 @@
                 "Redflag's smoke alarms won't be able to catch everything, however. For example if the data are shuffled and/or randomly sampled in a split, it might be very hard to spot self-correlation. I'm not sure how to alert the user to that kind of error, other than by potentially providing a wrapped version of `train_test_split()`.\n",
                 "\n",
                 "Anyway, let's split our data in a sensible way: by well."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 23,
             "metadata": {},
             "outputs": [],
             "source": [
                 "features = ['GR', 'RHOB', 'PE', 'Noise']\n",
                 "test_wells = ['CRAWFORD', 'STUART']\n",
                 "\n",
                 "test_flag = df['Well Name'].isin(test_wells)\n",
@@ -669,15 +725,15 @@
                 "y_test = df.loc[test_flag, 'Lithology']\n",
                 "X_train = df.loc[~test_flag, features]\n",
                 "y_train = df.loc[~test_flag, 'Lithology']"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 24,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style>#sk-container-id-1 {color: black;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>Pipeline(steps=[(&#x27;rf.imbalance&#x27;, ImbalanceDetector()),\n",
                             "                (&#x27;rf.clip&#x27;, ClipDetector()),\n",
@@ -702,15 +758,15 @@
                             "                ('rf.multimodality', MultimodalityDetector()),\n",
                             "                ('rf.outlier', OutlierDetector()),\n",
                             "                ('rf.distributions', DistributionComparator()),\n",
                             "                ('rf.importance', ImportanceDetector()),\n",
                             "                ('rf.dummy', DummyPredictor())])"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 24,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "rf.pipeline"
             ]
@@ -720,15 +776,15 @@
             "metadata": {},
             "source": [
                 "We can include this in other pipelines:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 25,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style>#sk-container-id-2 {color: black;}#sk-container-id-2 pre{padding: 0;}#sk-container-id-2 div.sk-toggleable {background-color: white;}#sk-container-id-2 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-2 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-2 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-2 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-2 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-2 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-2 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-2 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-2 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-2 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-2 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-2 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-2 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-2 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-2 div.sk-item {position: relative;z-index: 1;}#sk-container-id-2 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-2 div.sk-item::before, #sk-container-id-2 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-2 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-2 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-2 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-2 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-2 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-2 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-2 div.sk-label-container {text-align: center;}#sk-container-id-2 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-2 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-2\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>Pipeline(steps=[(&#x27;standardscaler&#x27;, StandardScaler()),\n",
                             "                (&#x27;pipeline&#x27;,\n",
@@ -769,43 +825,43 @@
                             "                                 ('rf.outlier', OutlierDetector()),\n",
                             "                                 ('rf.distributions', DistributionComparator()),\n",
                             "                                 ('rf.importance', ImportanceDetector()),\n",
                             "                                 ('rf.dummy', DummyPredictor())])),\n",
                             "                ('svc', SVC())])"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 25,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from sklearn.pipeline import make_pipeline\n",
                 "\n",
                 "pipe = make_pipeline(StandardScaler(), rf.pipeline, SVC())\n",
                 "pipe"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 26,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "\ud83d\udea9 The labels are imbalanced by more than the threshold (0.420 > 0.400). See self.minority_classes_ for the minority classes.\n",
                         "\ud83d\udea9 Features 0, 1 have samples that may be clipped.\n",
                         "\ud83d\udea9 Features 0, 1, 2 have samples that may be correlated.\n",
                         "\ud83d\udea9 Feature 0 has a multimodal distribution.\n",
-                        "\u26a0\ufe0f Multimodality detection may not have succeeded for all groups in all features.\n",
+                        "\u2139\ufe0f Multimodality detection may not have succeeded for all groups in all features.\n",
                         "\ud83d\udea9 There are more outliers than expected in the training data (316 vs 31).\n",
                         "\ud83d\udea9 Feature 3 has low importance; check for relevance.\n",
-                        "\u2139\ufe0f Dummy classifier scores: {'f1': 0.2777104337392946, 'roc_auc': 0.5013219070647543} (stratified strategy).\n"
+                        "\u2139\ufe0f Dummy classifier scores: {'f1': 0.25609045854904466, 'roc_auc': 0.5021169500369603} (stratified strategy).\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<style>#sk-container-id-3 {color: black;}#sk-container-id-3 pre{padding: 0;}#sk-container-id-3 div.sk-toggleable {background-color: white;}#sk-container-id-3 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-3 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-3 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-3 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-3 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-3 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-3 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-3 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-3 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-3 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-3 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-3 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-3 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-3 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-3 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-3 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-3 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-3 div.sk-item {position: relative;z-index: 1;}#sk-container-id-3 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-3 div.sk-item::before, #sk-container-id-3 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-3 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-3 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-3 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-3 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-3 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-3 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-3 div.sk-label-container {text-align: center;}#sk-container-id-3 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-3 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-3\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>Pipeline(steps=[(&#x27;standardscaler&#x27;, StandardScaler()),\n",
                             "                (&#x27;pipeline&#x27;,\n",
@@ -849,26 +905,26 @@
                             "                                  OutlierDetector(threshold=3.643721188696941)),\n",
                             "                                 ('rf.distributions', DistributionComparator()),\n",
                             "                                 ('rf.importance', ImportanceDetector()),\n",
                             "                                 ('rf.dummy', DummyPredictor())])),\n",
                             "                ('svc', SVC())])"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 26,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "pipe.fit(X_train, y_train)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 27,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "\ud83d\udea9 Feature 0 has samples that may be clipped.\n",
@@ -1045,15 +1101,15 @@
                             "       'siltstone', 'siltstone', 'mudstone', 'siltstone', 'siltstone',\n",
                             "       'siltstone', 'siltstone', 'siltstone', 'siltstone', 'siltstone',\n",
                             "       'siltstone', 'siltstone', 'siltstone', 'siltstone', 'siltstone',\n",
                             "       'siltstone', 'siltstone', 'siltstone', 'siltstone', 'siltstone',\n",
                             "       'siltstone', 'siltstone', 'siltstone', 'siltstone'], dtype=object)"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 27,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "pipe.predict(X_test)"
             ]
@@ -1063,44 +1119,44 @@
             "metadata": {},
             "source": [
                 "## Making your own tests"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 28,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "\ud83d\udea9 Feature 3 has samples that are negative.\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<style>#sk-container-id-4 {color: black;}#sk-container-id-4 pre{padding: 0;}#sk-container-id-4 div.sk-toggleable {background-color: white;}#sk-container-id-4 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-4 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-4 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-4 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-4 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-4 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-4 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-4 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-4 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-4 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-4 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-4 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-4 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-4 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-4 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-4 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-4 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-4 div.sk-item {position: relative;z-index: 1;}#sk-container-id-4 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-4 div.sk-item::before, #sk-container-id-4 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-4 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-4 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-4 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-4 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-4 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-4 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-4 div.sk-label-container {text-align: center;}#sk-container-id-4 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-4 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-4\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>Pipeline(steps=[(&#x27;detector&#x27;,\n",
-                            "                 Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x7efc26efbf60&gt;,\n",
+                            "                 Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x12efbb880&gt;,\n",
                             "                          message=&#x27;are negative&#x27;)),\n",
                             "                (&#x27;svc&#x27;, SVC())])</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item sk-dashed-wrapped\"><div class=\"sk-label-container\"><div class=\"sk-label sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-34\" type=\"checkbox\" ><label for=\"sk-estimator-id-34\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">Pipeline</label><div class=\"sk-toggleable__content\"><pre>Pipeline(steps=[(&#x27;detector&#x27;,\n",
-                            "                 Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x7efc26efbf60&gt;,\n",
+                            "                 Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x12efbb880&gt;,\n",
                             "                          message=&#x27;are negative&#x27;)),\n",
-                            "                (&#x27;svc&#x27;, SVC())])</pre></div></div></div><div class=\"sk-serial\"><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-35\" type=\"checkbox\" ><label for=\"sk-estimator-id-35\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">Detector</label><div class=\"sk-toggleable__content\"><pre>Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x7efc26efbf60&gt;,\n",
+                            "                (&#x27;svc&#x27;, SVC())])</pre></div></div></div><div class=\"sk-serial\"><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-35\" type=\"checkbox\" ><label for=\"sk-estimator-id-35\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">Detector</label><div class=\"sk-toggleable__content\"><pre>Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x12efbb880&gt;,\n",
                             "         message=&#x27;are negative&#x27;)</pre></div></div></div><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-36\" type=\"checkbox\" ><label for=\"sk-estimator-id-36\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">SVC</label><div class=\"sk-toggleable__content\"><pre>SVC()</pre></div></div></div></div></div></div></div>"
                         ],
                         "text/plain": [
                             "Pipeline(steps=[('detector',\n",
-                            "                 Detector(func=<function BaseRedflagDetector.__init__.<locals>.<lambda> at 0x7efc26efbf60>,\n",
+                            "                 Detector(func=<function BaseRedflagDetector.__init__.<locals>.<lambda> at 0x12efbb880>,\n",
                             "                          message='are negative')),\n",
                             "                ('svc', SVC())])"
                         ]
                     },
-                    "execution_count": 19,
+                    "execution_count": 28,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from redflag import Detector\n",
                 "\n",
@@ -1136,15 +1192,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.5"
+            "version": "3.12.0"
         },
         "vscode": {
             "interpreter": {
                 "hash": "3ad933181bd8a04b432d3370b9dc3b0662ad032c4dfaa4e4f1596c548f763858"
             }
         }
     },
```

### Comparing `redflag-0.4.2rc1/docs/notebooks/Using_redflag_with_Pandas.ipynb` & `redflag-0.5.0rc1/docs/notebooks/Using_redflag_with_Pandas.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9917730524227235%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(2, "As well as using `redflag`\'s functions directly (see '*

 * *            '`Basic_usage.ipynb`), or with `sklearn` (see `Using_redflag_with_Pandas.ipynb`), '*

 * *            "`redflag` has some Pandas 'accessors' that give you access to some `redflag` "*

 * *            'functions almost as if they were methods on Pandas objects.\\n")], delete: [2]}}, 1: '*

 * *            "{'execution_count': 4, 'outputs': {0: {'data': {'text/plain': "*

 * *            '["\'0.4.2rc2.dev14+g54704af.d2024 […]*

```diff
@@ -3,47 +3,47 @@
         {
             "cell_type": "markdown",
             "id": "a8d12712-5c7b-4acb-bb8b-e73efcb9b5dc",
             "metadata": {},
             "source": [
                 "# \ud83d\udea9 Using `redflag` with Pandas\n",
                 "\n",
-                "As well as using `redflag`'s functions directly (see [`Basic_usage.ipynb`](`./Basic_usage.ipynb`)), or with `sklearn` (see `Using_redflag_with_Pandas.ipynb`), `redflag` has some Pandas 'accessors' that give you access to some `redflag` functions almost as if they were methods on Pandas objects.\n",
+                "As well as using `redflag`'s functions directly (see `Basic_usage.ipynb`), or with `sklearn` (see `Using_redflag_with_Pandas.ipynb`), `redflag` has some Pandas 'accessors' that give you access to some `redflag` functions almost as if they were methods on Pandas objects.\n",
                 "\n",
                 "The best way to get the idea is to look at an example.\n",
                 "\n",
                 "First, even though we may not use it directly, we have to import `redflag` to get access to its functions. As long as you have `pandas` installed, it will register the accessors."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 4,
             "id": "77aa7f67-0bc7-48e9-87f4-183aa2dc2c35",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'0.4.1.dev4+ga088506.d20231002'"
+                            "'0.4.2rc2.dev14+g54704af.d20240421'"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import redflag as rf\n",
                 "\n",
                 "rf.__version__"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 5,
             "id": "3dbcf6e1-1cb5-4ca5-b64a-bc1d9e7b174f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -213,23 +213,23 @@
                             "0  2393.499945  siliciclastic           True  \n",
                             "1  2416.119814  siliciclastic           True  \n",
                             "2  2404.576056  siliciclastic           True  \n",
                             "3  2393.249071  siliciclastic           True  \n",
                             "4  2382.602601  siliciclastic           True  "
                         ]
                     },
-                    "execution_count": 2,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import pandas as pd\n",
                 "\n",
-                "df = pd.read_csv('https://raw.githubusercontent.com/scienxlab/datasets/main/kgs/Panoma_training_data.csv')\n",
+                "df = pd.read_csv('https://raw.githubusercontent.com/scienxlab/datasets/main/kgs/panoma-training-data.csv')\n",
                 "\n",
                 "df.head()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d77e460b-b925-4dec-b56d-d3f18ed1ecbb",
@@ -244,15 +244,15 @@
             "metadata": {},
             "source": [
                 "For the time being, there are only accessors on Pandas `Series` objects. For example:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 6,
             "id": "1b17a7e8-1d28-4e1b-9b7d-ecdbbe750aaf",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Call the Series s for simplicity:\n",
                 "s = df['Lithology']"
             ]
@@ -263,25 +263,25 @@
             "metadata": {},
             "source": [
                 "Now we can call the `redflag` function `imbalance_degree()` as if it were a method (but notice the extra `redflag` we have to insert to access the method):"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 7,
             "id": "6af691f4-90a3-4a8e-b842-a20f70c72314",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "3.378593040846633"
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s.redflag.imbalance_degree()"
             ]
@@ -292,28 +292,28 @@
             "metadata": {},
             "source": [
                 "Or we can ask for the new 'dummy' scores:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 8,
             "id": "5897e460-cc15-4858-939b-b91b19fafc9f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{'f1': 0.24829855151480457,\n",
-                            " 'roc_auc': 0.50211405767246,\n",
+                            "{'f1': 0.24566600930871996,\n",
+                            " 'roc_auc': 0.5021684735059516,\n",
                             " 'strategy': 'stratified',\n",
                             " 'task': 'classification'}"
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s.redflag.dummy_scores()"
             ]
@@ -324,28 +324,28 @@
             "metadata": {},
             "source": [
                 "Let's try that on a regression target like `df['RHOB']`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 9,
             "id": "f734bb50-15e9-43c3-b31f-1a078e398dc3",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'mean_squared_error': 47528.78263092096,\n",
                             " 'r2': 0.0,\n",
                             " 'strategy': 'mean',\n",
                             " 'task': 'regression'}"
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df['RHOB'].redflag.dummy_scores()"
             ]
@@ -356,26 +356,44 @@
             "metadata": {},
             "source": [
                 "Or we can ask for a 'report' (very simple for now):"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 10,
             "id": "02380595-2b47-4718-9b58-ef6b170f29b1",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Continuous data suitable for regression\n",
-                        "Outliers:    [  34   35  136  140  141  142  143  145  147  180  181  182  532  583\n",
-                        "  633  662  757  768  769  801 1316 1547 1731 1732 1744 1754 1756 1779\n",
-                        " 1780 1788 2884 2932 2973 2974 3004 3079 3080 3087 3094 3109]\n",
+                        "Outliers:    [  95   96  132  175  176  177  222  223  263  526  527  531  532  533\n",
+                        "  534  575  576  577  578  579  580  581  582  583  584  585  586  587\n",
+                        "  588  621  622  633  634  635  636  652  653  654  660  661  662  663\n",
+                        "  711  712  713  756  757  758  759  760  768  769  770  771  772  773\n",
+                        "  774  775  776  777  778  779  780  781  782  800  801  802  803  804\n",
+                        "  818  819  821  822  823  824  835  836  841  842  843  844  845  846\n",
+                        "  849  850  934  935  936  937  938 1039 1040 1044 1048 1049 1113 1114\n",
+                        " 1115 1116 1145 1146 1147 1148 1149 1150 1151 1216 1217 1218 1221 1222\n",
+                        " 1223 1224 1225 1304 1313 1314 1315 1316 1368 1369 1370 1371 1372 1373\n",
+                        " 1374 1375 1446 1447 1496 1497 1498 1499 1546 1547 1548 1549 1567 1568\n",
+                        " 1622 1623 1624 1662 1663 1664 1665 1666 1722 1723 1724 1725 1726 1735\n",
+                        " 1739 1740 1741 1742 1743 1744 1745 1746 1747 1748 1753 1754 1755 1756\n",
+                        " 1757 1777 1778 1779 1780 1781 1782 1783 1784 1785 1786 1787 1788 1789\n",
+                        " 1790 1805 1806 1807 1808 1809 1810 1812 1813 1866 1868 1869 1870 1981\n",
+                        " 1982 2054 2055 2139 2327 2415 2416 2417 2418 2488 2489 2490 2867 2868\n",
+                        " 2869 2870 2871 2872 2873 2882 2883 2884 2888 2889 2921 2922 2923 2924\n",
+                        " 2925 2926 2927 2928 2929 2930 2931 2932 2933 2972 2973 2974 2975 2976\n",
+                        " 3004 3087 3088 3089 3090 3091 3092 3093 3094 3095 3096 3097 3098 3099\n",
+                        " 3100 3101 3102 3109 3110 3111 3112 3113 3114 3115 3341 3429 3430 3443\n",
+                        " 3444 3515 3516 3517 3861 3862 3863 3905 3906 3907 3931 3932 3933 3934\n",
+                        " 3935]\n",
                         "Correlated:  True\n",
                         "Dummy scores:{'mean': {'mean_squared_error': 47528.78263092096, 'r2': 0.0}}\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
@@ -398,48 +416,48 @@
                 "## DataFrame accessor\n",
                 "\n",
                 "Experimental feature: so far only `feature_importances` and `correlation_detector` are implemented."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 11,
             "id": "274cc24d-69ad-49ef-8606-cc9b77b154dc",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "array([0.23209524, 0.21793961, 0.34387713, 0.20608802])"
+                            "array([0.29029061, 0.18151719, 0.30409475, 0.22409746])"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "features = ['GR', 'RHOB', 'PE', 'ILD_log10']\n",
                 "df.redflag.feature_importances(features, target='Lithology')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 12,
             "id": "12e3e4ee-e8df-47ba-810d-3bff492d5389",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Feature 0 appears to be autocorrelated.\n",
-                        "Feature 1 appears to be autocorrelated.\n",
-                        "Feature 2 appears to be autocorrelated.\n",
-                        "Feature 3 appears to be autocorrelated.\n"
+                        "\ud83d\udea9 Feature 0 appears to be autocorrelated.\n",
+                        "\ud83d\udea9 Feature 1 appears to be autocorrelated.\n",
+                        "\ud83d\udea9 Feature 2 appears to be autocorrelated.\n",
+                        "\ud83d\udea9 Feature 3 appears to be autocorrelated.\n"
                     ]
                 }
             ],
             "source": [
                 "df.redflag.correlation_detector(features, target=None)"
             ]
         },
@@ -464,13 +482,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.5"
+            "version": "3.12.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `redflag-0.4.2rc1/docs/notebooks/Using_redflag_with_sklearn.ipynb` & `redflag-0.5.0rc1/docs/notebooks/Using_redflag_with_sklearn.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9918410213492934%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(2, "df = '*

 * *            'pd.read_csv(\'https://raw.githubusercontent.com/scienxlab/datasets/main/kgs/panoma-training-data.csv\')\\n")], '*

 * *            "delete: [2]}}, 3: {'execution_count': 3, 'outputs': {0: {'execution_count': 3}, 1: "*

 * *            "{'data': {'image/png': "*

 * *            "'iVBORw0KGgoAAAANSUhEUgAAAjsAAAGwCAYAAABPSaTdAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8g+/7EAAAACXBIWXMAAA9hAAAPYQGoP6dpAABUA0lEQVR4nO3deXyU […]*

```diff
@@ -233,15 +233,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import pandas as pd\n",
                 "\n",
-                "df = pd.read_csv('https://raw.githubusercontent.com/scienxlab/datasets/main/kgs/Panoma_training_data.csv')\n",
+                "df = pd.read_csv('https://raw.githubusercontent.com/scienxlab/datasets/main/kgs/panoma-training-data.csv')\n",
                 "\n",
                 "# Look at the transposed summary: each column in the DataFrame is a row here.\n",
                 "df.describe().T"
             ]
         },
         {
             "cell_type": "markdown",
@@ -250,64 +250,54 @@
                 "Note that the features (e.g. GR, RHOB) are not **independent** records; they are correlated to themselves in depth.\n",
                 "\n",
                 "Furthermore, some of these features are clipped, e.g. the GR feature is clipped at a max value of 200:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/home/matt/miniconda3/envs/redflag/lib/python3.11/site-packages/seaborn/_oldcore.py:1498: FutureWarning: is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead\n",
-                        "  if pd.api.types.is_categorical_dtype(vector):\n",
-                        "/home/matt/miniconda3/envs/redflag/lib/python3.11/site-packages/seaborn/_oldcore.py:1119: FutureWarning: use_inf_as_na option is deprecated and will be removed in a future version. Convert inf values to NaN before operating instead.\n",
-                        "  with pd.option_context('mode.use_inf_as_na', True):\n"
-                    ]
-                },
-                {
                     "data": {
                         "text/plain": [
                             "<Axes: xlabel='GR', ylabel='Count'>"
                         ]
                     },
-                    "execution_count": 2,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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Qw891FlDuCgXGu+pU6f0+eef64knntDnn3+ut99+W+Xl5br99tvP6btw4UKvfT5r1qzOKP+itbZ/JWncuHFeY3nzzTe92k3Zv5K8xllVVaVXX31VNptNeXl5Xv2CYf+25buntb/HZ86c0fjx49XQ0KDi4mK99tprWrlypebPn+/7gn3yNE4EjJqaGkuStW3bNs+6v/u7v7MeeeQR/xXlQ08++aQ1bNiwFttqa2ut8PBwa82aNZ51X375pSXJKikp6aQKO9Yjjzxi9e/f32pubrYsy6x9K8l65513PK+bm5sth8NhPfvss551tbW1lt1ut958803Lsixr//79liRr586dnj7vv/++ZbPZrO+++67Tam+Pn463JZ999pklyfr2228961JTU62lS5d2bHEdoKXxTpkyxbrjjjvO+x7T9+8dd9xh3XzzzV7rgnX//vS7py1/j9evX2+FhIRYLpfL02fZsmVWVFSUVV9f79P6mNkxTF1dnSQpNjbWa/0bb7yhXr16aciQISosLNSpU6f8UZ5PfP3110pMTFS/fv00efJkVVRUSJJKS0vV2NiorKwsT99BgwYpJSVFJSUl/irXZxoaGvT666/rgQce8HpgrUn79scOHTokl8vltT+jo6OVmZnp2Z8lJSWKiYnRyJEjPX2ysrIUEhKiHTt2dHrNvlZXVyebzXbOs/ueeeYZ9ezZU8OHD9ezzz7bIdP+nWXr1q2Ki4vTwIEDNWPGDB09etTTZvL+ra6u1l/+8hdNnTr1nLZg3L8//e5py9/jkpISZWRkeN0AOCcnR263W/v27fNpfUbcQRl/09zcrNmzZ+uGG27QkCFDPOt/9atfKTU1VYmJidq9e7fmzZun8vJyvf32236stn0yMzO1cuVKDRw4UFVVVXrqqaf085//XHv37pXL5VJERMQ5Xwzx8fFyuVz+KdiH3n33XdXW1uq+++7zrDNp3/7U2X320zuh/3h/ulwuxcXFebWHhYUpNjY26Pf56dOnNW/ePN19991eD0/87W9/q5/97GeKjY1VcXGxCgsLVVVVpSVLlvix2vYZN26cJkyYoLS0NB08eFCPPfaYcnNzVVJSotDQUKP372uvvaYePXqcc5g9GPdvS989bfl77HK5Wvz9PtvmS4Qdg+Tn52vv3r1e57BI8jq+nZGRoYSEBI0dO1YHDx5U//79O7vMS5Kbm+v5eejQocrMzFRqaqr+/Oc/q2vXrn6srOO98sorys3NVWJiomedSfsW/6+xsVH/8A//IMuytGzZMq+2goICz89Dhw5VRESEpk+frkWLFgXd4wcmTZrk+TkjI0NDhw5V//79tXXrVo0dO9aPlXW8V199VZMnT1aXLl281gfj/j3fd08g4TCWIWbOnKl169bpo48+Up8+fS7YNzMzU5J04MCBziitQ8XExOiqq67SgQMH5HA41NDQoNraWq8+1dXVcjgc/inQR7799ltt2rRJDz744AX7mbRvz+6zn1698eP96XA4VFNT49Xe1NSkY8eOBe0+Pxt0vv32W23cuNFrVqclmZmZampq0jfffNM5BXagfv36qVevXp7/vybuX0n65JNPVF5e3urvsxT4+/d83z1t+XvscDha/P0+2+ZLhJ0gZ1mWZs6cqXfeeUdbtmxRWlpaq+8pKyuTJCUkJHRwdR3vxIkTOnjwoBISEjRixAiFh4dr8+bNnvby8nJVVFTI6XT6scpLt2LFCsXFxWn8+PEX7GfSvk1LS5PD4fDan263Wzt27PDsT6fTqdraWpWWlnr6bNmyRc3NzZ7gF0zOBp2vv/5amzZtUs+ePVt9T1lZmUJCQs453BOMjhw5oqNHj3r+/5q2f8965ZVXNGLECA0bNqzVvoG6f1v77mnL32On06k9e/Z4BdqzAT89Pd3nBSOIzZgxw4qOjra2bt1qVVVVeZZTp05ZlmVZBw4csBYuXGjt2rXLOnTokPXee+9Z/fr1s0aPHu3nytvn0UcftbZu3WodOnTI+s///E8rKyvL6tWrl1VTU2NZlmU9/PDDVkpKirVlyxZr165dltPptJxOp5+rvjRnzpyxUlJSrHnz5nmtN2HfHj9+3Priiy+sL774wpJkLVmyxPriiy88Vx8988wzVkxMjPXee+9Zu3fvtu644w4rLS3N+uGHHzzbGDdunDV8+HBrx44d1qeffmpdeeWV1t133+2vIV3Qhcbb0NBg3X777VafPn2ssrIyr9/ns1emFBcXW0uXLrXKysqsgwcPWq+//rrVu3dv69577/XzyFp2ofEeP37c+t3vfmeVlJRYhw4dsjZt2mT97Gc/s6688krr9OnTnm2Ysn/PqqursyIjI61ly5ad8/5g2r+tffdYVut/j5uamqwhQ4ZY2dnZVllZmbVhwward+/eVmFhoc/rJewEOUktLitWrLAsy7IqKiqs0aNHW7GxsZbdbrcGDBhgzZ0716qrq/Nv4e00ceJEKyEhwYqIiLCSkpKsiRMnWgcOHPC0//DDD9ZvfvMb64orrrAiIyOtv//7v7eqqqr8WPGl++CDDyxJVnl5udd6E/btRx991OL/3ylTpliW9bfLz5944gkrPj7estvt1tixY8/5dzh69Kh19913W927d7eioqKs+++/3zp+/LgfRtO6C4330KFD5/19/uijjyzLsqzS0lIrMzPTio6Otrp06WINHjzYevrpp73CQSC50HhPnTplZWdnW71797bCw8Ot1NRUa9q0aV6XIVuWOfv3rJdeesnq2rWrVVtbe877g2n/tvbdY1lt+3v8zTffWLm5uVbXrl2tXr16WY8++qjV2Njo83pt/1c0AACAkThnBwAAGI2wAwAAjEbYAQAARiPsAAAAoxF2AACA0Qg7AADAaIQdAABgNMIOAAAwGmEHAAAYjbADIOi5XC498sgjGjBggLp06aL4+HjdcMMNWrZsmU6dOiVJ6tu3r2w2m2w2myIjI5WRkaF//dd/9XPlADpDmL8LAIBL8d///d+64YYbFBMTo6effloZGRmy2+3as2ePXn75ZSUlJen222+XJC1cuFDTpk3TqVOntGbNGk2bNk1JSUnKzc318ygAdCSejQUgqI0bN0779u3TV199pW7dup3TblmWbDab+vbtq9mzZ2v27Nmetp49e2rKlClasmRJJ1YMoLNxGAtA0Dp69Kg+/PBD5efntxh0JMlms52zrrm5Wf/+7/+u//mf/1FERERHlwnAzwg7AILWgQMHZFmWBg4c6LW+V69e6t69u7p376558+Z51s+bN0/du3eX3W7XXXfdpSuuuEIPPvhgZ5cNoJMRdgAY57PPPlNZWZmuvvpq1dfXe9bPnTtXZWVl2rJlizIzM7V06VINGDDAj5UC6AycoAwgaA0YMEA2m03l5eVe6/v16ydJ6tq1q9f6Xr16acCAARowYIDWrFmjjIwMjRw5Uunp6Z1WM4DOx8wOgKDVs2dP3XLLLfrTn/6kkydPXtR7k5OTNXHiRBUWFnZQdQACBWEHQFB78cUX1dTUpJEjR2r16tX68ssvVV5ertdff11fffWVQkNDz/veRx55RGvXrtWuXbs6sWIAnY1LzwEEvaqqKj399NP6y1/+oiNHjshutys9PV2//OUv9Zvf/EaRkZEtXnou/e3S9ZCQEK1fv94/xQPocIQdAABgNA5jAQAAoxF2AACA0Qg7AADAaIQdAABgNMIOAAAwGmEHAAAYjbADAACMRtgBAABGI+wAAACjEXYAAIDRCDsAAMBo/wtrVGNMX6SWNwAAAABJRU5ErkJggg==",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "import seaborn as sns\n",
                 "\n",
-                "sns.histplot(df['GR'])"
+                "sns.histplot(df['GR'], lw=0, kde=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We will split this dataset by group (well name):"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "features = ['GR', 'RHOB', 'PE']\n",
                 "\n",
                 "test_wells = ['CRAWFORD', 'STUART']\n",
                 "\n",
@@ -361,15 +351,15 @@
                 "The `ImbalanceComparator`, is not compatible with ordinary `Pipeline` objects, because it requires `y` (class imbalance comparison only works on the target vector). An `RfPipeline` object is available to use with this comparator... but it will not work as part of another ordinary `Pipeline`, so if you compose a multi-pipeline pipeline, make sure to use `RfPipeline` for all of it. Please note there is also a `make_rf_pipeline()` function that works just like `make_pipeline`, but it uses `RfPipeline` instead.\n",
                 "\n",
                 "For now, we'll carry on with the standard `sklearn` pipeline. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style>#sk-container-id-1 {color: black;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>Pipeline(steps=[(&#x27;rf.imbalance&#x27;, ImbalanceDetector()),\n",
                             "                (&#x27;rf.clip&#x27;, ClipDetector()),\n",
@@ -394,15 +384,15 @@
                             "                ('rf.multimodality', MultimodalityDetector()),\n",
                             "                ('rf.outlier', OutlierDetector()),\n",
                             "                ('rf.distributions', DistributionComparator()),\n",
                             "                ('rf.importance', ImportanceDetector()),\n",
                             "                ('rf.dummy', DummyPredictor())])"
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import redflag as rf\n",
                 "\n",
@@ -414,15 +404,15 @@
             "metadata": {},
             "source": [
                 "We can use this in another pipeline:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style>#sk-container-id-2 {color: black;}#sk-container-id-2 pre{padding: 0;}#sk-container-id-2 div.sk-toggleable {background-color: white;}#sk-container-id-2 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-2 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-2 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-2 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-2 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-2 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-2 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-2 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-2 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-2 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-2 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-2 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-2 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-2 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-2 div.sk-item {position: relative;z-index: 1;}#sk-container-id-2 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-2 div.sk-item::before, #sk-container-id-2 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-2 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-2 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-2 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-2 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-2 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-2 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-2 div.sk-label-container {text-align: center;}#sk-container-id-2 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-2 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-2\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>Pipeline(steps=[(&#x27;standardscaler&#x27;, StandardScaler()),\n",
                             "                (&#x27;pipeline&#x27;,\n",
@@ -463,15 +453,15 @@
                             "                                 ('rf.outlier', OutlierDetector()),\n",
                             "                                 ('rf.distributions', DistributionComparator()),\n",
                             "                                 ('rf.importance', ImportanceDetector()),\n",
                             "                                 ('rf.dummy', DummyPredictor())])),\n",
                             "                ('svc', SVC())])"
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from sklearn.pipeline import make_pipeline\n",
                 "from sklearn.preprocessing import StandardScaler\n",
@@ -490,28 +480,28 @@
                 "- Check the target `y` for imbalance (if it is categorical).\n",
                 "- Check the input features `X` for issues like clipping and self-correlation.\n",
                 "- Learn the input feature distributions for later comparison."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "\ud83d\udea9 The labels are imbalanced by more than the threshold (0.420 > 0.400). See self.minority_classes_ for the minority classes.\n",
                         "\ud83d\udea9 Features 0, 1 have samples that may be clipped.\n",
                         "\ud83d\udea9 Features 0, 1, 2 have samples that may be correlated.\n",
                         "\ud83d\udea9 Feature 0 has a multimodal distribution.\n",
-                        "\u26a0\ufe0f Multimodality detection may not have succeeded for all groups in all features.\n",
+                        "\u2139\ufe0f Multimodality detection may not have succeeded for all groups in all features.\n",
                         "\ud83d\udea9 There are more outliers than expected in the training data (349 vs 31).\n",
-                        "\u2139\ufe0f Dummy classifier scores: {'f1': 0.26046769220198457, 'roc_auc': 0.5059272862867259} (stratified strategy).\n"
+                        "\u2139\ufe0f Dummy classifier scores: {'f1': 0.2559627467209994, 'roc_auc': 0.504671110755004} (stratified strategy).\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<style>#sk-container-id-3 {color: black;}#sk-container-id-3 pre{padding: 0;}#sk-container-id-3 div.sk-toggleable {background-color: white;}#sk-container-id-3 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-3 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-3 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-3 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-3 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-3 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-3 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-3 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-3 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-3 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-3 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-3 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-3 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-3 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-3 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-3 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-3 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-3 div.sk-item {position: relative;z-index: 1;}#sk-container-id-3 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-3 div.sk-item::before, #sk-container-id-3 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-3 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-3 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-3 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-3 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-3 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-3 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-3 div.sk-label-container {text-align: center;}#sk-container-id-3 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-3 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-3\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>Pipeline(steps=[(&#x27;standardscaler&#x27;, StandardScaler()),\n",
                             "                (&#x27;pipeline&#x27;,\n",
@@ -555,15 +545,15 @@
                             "                                  OutlierDetector(threshold=3.3682141715600706)),\n",
                             "                                 ('rf.distributions', DistributionComparator()),\n",
                             "                                 ('rf.importance', ImportanceDetector()),\n",
                             "                                 ('rf.dummy', DummyPredictor())])),\n",
                             "                ('svc', SVC())])"
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "pipe.fit(X_train, y_train)"
             ]
@@ -576,15 +566,15 @@
                 "\n",
                 "- Check for first-order issues, e.g. for clipping, or self-correlation.\n",
                 "- Compare statistics to the training data, e.g. to compare the distribution of the data or look for outliers."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "\ud83d\udea9 Feature 0 has samples that may be clipped.\n",
@@ -599,15 +589,15 @@
                             "array(['siltstone', 'siltstone', 'siltstone', 'siltstone', 'siltstone',\n",
                             "       'siltstone', 'siltstone', 'siltstone', 'siltstone', 'siltstone',\n",
                             "       'siltstone', 'siltstone', 'siltstone', 'siltstone', 'siltstone',\n",
                             "       'siltstone', 'siltstone', 'siltstone', 'siltstone', 'siltstone'],\n",
                             "      dtype=object)"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "y_pred = pipe.predict(X_test)\n",
                 "y_pred[:20]"
@@ -629,15 +619,15 @@
                 "Let's construct a pipeline from `redflag`'s transformers directly.\n",
                 "\n",
                 "Let's drop the clipped records of the GR log."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [],
             "source": [
                 "df = df.loc[df['GR'] < 200]\n",
                 "\n",
                 "test_flag = df['Well Name'].isin(test_wells)\n",
                 "\n",
@@ -661,15 +651,15 @@
                 "Finally, we'll lower the threshold for the distribution comparison. This is the minimum Wasserstein distance required to trigger the warning.\n",
                 "\n",
                 "So here's the new pipeline:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [],
             "source": [
                 "pipe = make_pipeline(StandardScaler(),\n",
                 "                     rf.ImbalanceDetector(threshold=0.5),\n",
                 "                     rf.ClipDetector(),\n",
                 "                     rf.OutlierDetector(p=0.80),\n",
@@ -682,15 +672,15 @@
             "metadata": {},
             "source": [
                 "Remember, feature 0 is no longer clipped, and the correlation detection is not being run. So we expect to see only the outlier issue, and the clipping issue with the RHOB column:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "\ud83d\udea9 Feature 1 has samples that may be clipped.\n",
@@ -723,15 +713,15 @@
                             "                ('outlierdetector',\n",
                             "                 OutlierDetector(p=0.8, threshold=2.154443705823081)),\n",
                             "                ('distributioncomparator',\n",
                             "                 DistributionComparator(threshold=0.25)),\n",
                             "                ('svc', SVC())])"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "pipe.fit(X_train, y_train)"
             ]
@@ -741,15 +731,15 @@
             "metadata": {},
             "source": [
                 "The test dataset does not trigger the higher threshold for outliers. But with the new lower Wasserstein threshold, the distribution comparison fails for all of the features:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "\ud83d\udea9 Features 0, 1, 2 have distributions that are different from training.\n"
@@ -771,27 +761,27 @@
                 "There is also a `make_rf_pipeline()` function that works just like `make_pipeline`, but it uses `RfPipeline` instead.\n",
                 "\n",
                 "Let's use it to check whether the imbalance in our test data is similar to the imbalance in the training data. When fitting a model, the comparator will never trigger:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style>#sk-container-id-5 {color: black;}#sk-container-id-5 pre{padding: 0;}#sk-container-id-5 div.sk-toggleable {background-color: white;}#sk-container-id-5 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-5 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-5 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-5 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-5 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-5 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-5 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-5 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-5 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-5 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-5 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-5 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-5 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-5 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-5 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-5 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-5 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-5 div.sk-item {position: relative;z-index: 1;}#sk-container-id-5 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-5 div.sk-item::before, #sk-container-id-5 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-5 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-5 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-5 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-5 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-5 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-5 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-5 div.sk-label-container {text-align: center;}#sk-container-id-5 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-5 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-5\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>RfPipeline(steps=[(&#x27;imbalancecomparator&#x27;, ImbalanceComparator())])</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item sk-dashed-wrapped\"><div class=\"sk-label-container\"><div class=\"sk-label sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-41\" type=\"checkbox\" ><label for=\"sk-estimator-id-41\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">RfPipeline</label><div class=\"sk-toggleable__content\"><pre>RfPipeline(steps=[(&#x27;imbalancecomparator&#x27;, ImbalanceComparator())])</pre></div></div></div><div class=\"sk-serial\"><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-42\" type=\"checkbox\" ><label for=\"sk-estimator-id-42\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">ImbalanceComparator</label><div class=\"sk-toggleable__content\"><pre>ImbalanceComparator()</pre></div></div></div></div></div></div></div>"
                         ],
                         "text/plain": [
                             "RfPipeline(steps=[('imbalancecomparator', ImbalanceComparator())])"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "pipe = rf.make_rf_pipeline(rf.ImbalanceComparator())\n",
                 "\n",
@@ -803,38 +793,38 @@
             "metadata": {},
             "source": [
                 "But during transformation (therefore during prediction or other inference phases), it checks the imbalance is the same:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "\ud83d\udea9 There is a different number of minority classes (2) compared to the training data (4).\n",
-                        "\ud83d\udea9 The minority classes (dolomite, sandstone) are different from those in the training data (dolomite, mudstone, sandstone, wackestone).\n"
+                        "\ud83d\udea9 The minority classes (dolomite, sandstone) are different from those in the training data (wackestone, mudstone, sandstone, dolomite).\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
                             "array([[  66.276     , 2359.73324716,    3.591     ],\n",
                             "       [  77.252     , 2354.54679144,    3.341     ],\n",
                             "       [  82.899     , 2330.35783664,    3.064     ],\n",
                             "       ...,\n",
                             "       [  90.49      , 2193.06953439,    3.168     ],\n",
                             "       [  90.975     , 2192.32922081,    3.154     ],\n",
                             "       [  90.108     , 2176.62535394,    3.125     ]])"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "pipe.transform(X_test, y_test)"
             ]
@@ -851,37 +841,37 @@
             "metadata": {},
             "source": [
                 "You can pass a detection function to a generic `Detector`, along with a warning to emit when it is triggered:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style>#sk-container-id-6 {color: black;}#sk-container-id-6 pre{padding: 0;}#sk-container-id-6 div.sk-toggleable {background-color: white;}#sk-container-id-6 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-6 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-6 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-6 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-6 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-6 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-6 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-6 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-6 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-6 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-6 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-6 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-6 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-6 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-6 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-6 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-6 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-6 div.sk-item {position: relative;z-index: 1;}#sk-container-id-6 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-6 div.sk-item::before, #sk-container-id-6 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-6 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-6 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-6 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-6 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-6 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-6 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-6 div.sk-label-container {text-align: center;}#sk-container-id-6 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-6 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-6\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>Pipeline(steps=[(&#x27;detector&#x27;,\n",
-                            "                 Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x7fd2fa8d4f40&gt;,\n",
+                            "                 Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x13a283380&gt;,\n",
                             "                          message=&#x27;are NaNs&#x27;)),\n",
                             "                (&#x27;svc&#x27;, SVC())])</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item sk-dashed-wrapped\"><div class=\"sk-label-container\"><div class=\"sk-label sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-43\" type=\"checkbox\" ><label for=\"sk-estimator-id-43\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">Pipeline</label><div class=\"sk-toggleable__content\"><pre>Pipeline(steps=[(&#x27;detector&#x27;,\n",
-                            "                 Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x7fd2fa8d4f40&gt;,\n",
+                            "                 Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x13a283380&gt;,\n",
                             "                          message=&#x27;are NaNs&#x27;)),\n",
-                            "                (&#x27;svc&#x27;, SVC())])</pre></div></div></div><div class=\"sk-serial\"><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-44\" type=\"checkbox\" ><label for=\"sk-estimator-id-44\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">Detector</label><div class=\"sk-toggleable__content\"><pre>Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x7fd2fa8d4f40&gt;,\n",
+                            "                (&#x27;svc&#x27;, SVC())])</pre></div></div></div><div class=\"sk-serial\"><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-44\" type=\"checkbox\" ><label for=\"sk-estimator-id-44\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">Detector</label><div class=\"sk-toggleable__content\"><pre>Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x13a283380&gt;,\n",
                             "         message=&#x27;are NaNs&#x27;)</pre></div></div></div><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-45\" type=\"checkbox\" ><label for=\"sk-estimator-id-45\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">SVC</label><div class=\"sk-toggleable__content\"><pre>SVC()</pre></div></div></div></div></div></div></div>"
                         ],
                         "text/plain": [
                             "Pipeline(steps=[('detector',\n",
-                            "                 Detector(func=<function BaseRedflagDetector.__init__.<locals>.<lambda> at 0x7fd2fa8d4f40>,\n",
+                            "                 Detector(func=<function BaseRedflagDetector.__init__.<locals>.<lambda> at 0x13a283380>,\n",
                             "                          message='are NaNs')),\n",
                             "                ('svc', SVC())])"
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from redflag import Detector\n",
                 "import numpy as np\n",
@@ -903,15 +893,15 @@
                 "There are no NaNs.\n",
                 "\n",
                 "You can use `make_detector_pipeline` to combine several tests into a single pipeline."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "\ud83d\udea9 Features 0, 2 have samples that fail custom func has_outliers().\n"
@@ -919,55 +909,55 @@
                 },
                 {
                     "data": {
                         "text/html": [
                             "<style>#sk-container-id-7 {color: black;}#sk-container-id-7 pre{padding: 0;}#sk-container-id-7 div.sk-toggleable {background-color: white;}#sk-container-id-7 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-7 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-7 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-7 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-7 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-7 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-7 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-7 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-7 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-7 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-7 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-7 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-7 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-7 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-7 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-7 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-7 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-7 div.sk-item {position: relative;z-index: 1;}#sk-container-id-7 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-7 div.sk-item::before, #sk-container-id-7 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-7 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-7 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-7 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-7 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-7 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-7 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-7 div.sk-label-container {text-align: center;}#sk-container-id-7 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-7 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-7\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>Pipeline(steps=[(&#x27;standardscaler&#x27;, StandardScaler()),\n",
                             "                (&#x27;pipeline&#x27;,\n",
                             "                 Pipeline(steps=[(&#x27;detector-1&#x27;,\n",
-                            "                                  Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x7fd2fa8d5a80&gt;,\n",
+                            "                                  Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x13a283240&gt;,\n",
                             "                                           message=&#x27;fail custom func &#x27;\n",
                             "                                                   &#x27;has_nans()&#x27;)),\n",
                             "                                 (&#x27;detector-2&#x27;,\n",
-                            "                                  Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x7fd2fa8d54e0&gt;,\n",
+                            "                                  Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x13a2837e0&gt;,\n",
                             "                                           message=&#x27;fail custom func &#x27;\n",
                             "                                                   &#x27;has_outliers()&#x27;))])),\n",
                             "                (&#x27;svc&#x27;, SVC())])</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item sk-dashed-wrapped\"><div class=\"sk-label-container\"><div class=\"sk-label sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-46\" type=\"checkbox\" ><label for=\"sk-estimator-id-46\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">Pipeline</label><div class=\"sk-toggleable__content\"><pre>Pipeline(steps=[(&#x27;standardscaler&#x27;, StandardScaler()),\n",
                             "                (&#x27;pipeline&#x27;,\n",
                             "                 Pipeline(steps=[(&#x27;detector-1&#x27;,\n",
-                            "                                  Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x7fd2fa8d5a80&gt;,\n",
+                            "                                  Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x13a283240&gt;,\n",
                             "                                           message=&#x27;fail custom func &#x27;\n",
                             "                                                   &#x27;has_nans()&#x27;)),\n",
                             "                                 (&#x27;detector-2&#x27;,\n",
-                            "                                  Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x7fd2fa8d54e0&gt;,\n",
+                            "                                  Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x13a2837e0&gt;,\n",
                             "                                           message=&#x27;fail custom func &#x27;\n",
                             "                                                   &#x27;has_outliers()&#x27;))])),\n",
                             "                (&#x27;svc&#x27;, SVC())])</pre></div></div></div><div class=\"sk-serial\"><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-47\" type=\"checkbox\" ><label for=\"sk-estimator-id-47\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">StandardScaler</label><div class=\"sk-toggleable__content\"><pre>StandardScaler()</pre></div></div></div><div class=\"sk-item\"><div class=\"sk-label-container\"><div class=\"sk-label sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-48\" type=\"checkbox\" ><label for=\"sk-estimator-id-48\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">pipeline: Pipeline</label><div class=\"sk-toggleable__content\"><pre>Pipeline(steps=[(&#x27;detector-1&#x27;,\n",
-                            "                 Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x7fd2fa8d5a80&gt;,\n",
+                            "                 Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x13a283240&gt;,\n",
                             "                          message=&#x27;fail custom func has_nans()&#x27;)),\n",
                             "                (&#x27;detector-2&#x27;,\n",
-                            "                 Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x7fd2fa8d54e0&gt;,\n",
-                            "                          message=&#x27;fail custom func has_outliers()&#x27;))])</pre></div></div></div><div class=\"sk-serial\"><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-49\" type=\"checkbox\" ><label for=\"sk-estimator-id-49\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">Detector</label><div class=\"sk-toggleable__content\"><pre>Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x7fd2fa8d5a80&gt;,\n",
-                            "         message=&#x27;fail custom func has_nans()&#x27;)</pre></div></div></div><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-50\" type=\"checkbox\" ><label for=\"sk-estimator-id-50\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">Detector</label><div class=\"sk-toggleable__content\"><pre>Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x7fd2fa8d54e0&gt;,\n",
+                            "                 Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x13a2837e0&gt;,\n",
+                            "                          message=&#x27;fail custom func has_outliers()&#x27;))])</pre></div></div></div><div class=\"sk-serial\"><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-49\" type=\"checkbox\" ><label for=\"sk-estimator-id-49\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">Detector</label><div class=\"sk-toggleable__content\"><pre>Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x13a283240&gt;,\n",
+                            "         message=&#x27;fail custom func has_nans()&#x27;)</pre></div></div></div><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-50\" type=\"checkbox\" ><label for=\"sk-estimator-id-50\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">Detector</label><div class=\"sk-toggleable__content\"><pre>Detector(func=&lt;function BaseRedflagDetector.__init__.&lt;locals&gt;.&lt;lambda&gt; at 0x13a2837e0&gt;,\n",
                             "         message=&#x27;fail custom func has_outliers()&#x27;)</pre></div></div></div></div></div><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-51\" type=\"checkbox\" ><label for=\"sk-estimator-id-51\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">SVC</label><div class=\"sk-toggleable__content\"><pre>SVC()</pre></div></div></div></div></div></div></div>"
                         ],
                         "text/plain": [
                             "Pipeline(steps=[('standardscaler', StandardScaler()),\n",
                             "                ('pipeline',\n",
                             "                 Pipeline(steps=[('detector-1',\n",
-                            "                                  Detector(func=<function BaseRedflagDetector.__init__.<locals>.<lambda> at 0x7fd2fa8d5a80>,\n",
+                            "                                  Detector(func=<function BaseRedflagDetector.__init__.<locals>.<lambda> at 0x13a283240>,\n",
                             "                                           message='fail custom func '\n",
                             "                                                   'has_nans()')),\n",
                             "                                 ('detector-2',\n",
-                            "                                  Detector(func=<function BaseRedflagDetector.__init__.<locals>.<lambda> at 0x7fd2fa8d54e0>,\n",
+                            "                                  Detector(func=<function BaseRedflagDetector.__init__.<locals>.<lambda> at 0x13a2837e0>,\n",
                             "                                           message='fail custom func '\n",
                             "                                                   'has_outliers()'))])),\n",
                             "                ('svc', SVC())])"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from redflag import make_detector_pipeline\n",
                 "\n",
@@ -1066,13 +1056,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.5"
+            "version": "3.12.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `redflag-0.4.2rc1/docs/notebooks/_Pandas_accessor.ipynb` & `redflag-0.5.0rc1/docs/notebooks/_Pandas_accessor.ipynb`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/docs/post_process_html.py` & `redflag-0.5.0rc1/docs/post_process_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     """
     Replace the credit part of the HTML footer. Return the new text.
     """
     s = r"""<a class="muted-link" href="https://pradyunsg.me">@pradyunsg</a>'s"""
     pattern = re.compile(s)
     html = pattern.sub(r'', html)
 
-    s = r'Copyright &#169; 2023, The Redflag Authors'
+    s = r'Copyright &#169; 2024, The Redflag Authors'
     pattern = re.compile(s)
-    new_s = '&#169; 2023, The Redflag Authors | <a href="https://creativecommons.org/licenses/by/4.0/">CC BY</a>'
+    new_s = '&#169; 2024, The Redflag Authors | <a href="https://creativecommons.org/licenses/by/4.0/">CC BY</a>'
     html = pattern.sub(new_s, html)
 
     return html
 
 
 def add_analytics(html):
     """
```

### Comparing `redflag-0.4.2rc1/docs/pre_process_ipynb.py` & `redflag-0.5.0rc1/docs/pre_process_ipynb.py`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/docs/what_is_redflag.md` & `redflag-0.5.0rc1/docs/what_is_redflag.md`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/pyproject.toml` & `redflag-0.5.0rc1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 ]
 
 [project.urls]
 "documentation" = "https://scienxlab.org/redflag"
 "repository" = "https://github.com/scienxlab/redflag"
 
 [tool.setuptools_scm]
-write_to = "src/redflag/_version.py"
+# Empty section, required for dynamic versioning.
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.mypy]
 warn_return_any = true
 ignore_missing_imports = true
@@ -73,9 +73,8 @@
     "ignore:Deprecated call to `pkg_resources.declare_namespace:DeprecationWarning",
 ]
 
 [tool.coverage.run]
 # coverage configuration: https://coverage.readthedocs.io/
 omit = [
     "src/redflag/__init__.py",
-    "src/redflag/_version.py",
 ]
```

### Comparing `redflag-0.4.2rc1/src/redflag/distributions.py` & `redflag-0.5.0rc1/src/redflag/distributions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Functions related to understanding distributions.
 
 Author: Matt Hall, scienxlab.org
 Licence: Apache 2.0
 
-Copyright 2023 Redflag contributors
+Copyright 2024 Redflag contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -42,15 +42,22 @@
          'powerlaw', 'triang', 'trapz', 'uniform',
          ]
 
 def best_distribution(a: ArrayLike, bins: Optional[int]=None) -> NamedTuple:
     """
     Model data by finding best fit distribution to data.
 
-    Returns the best fit distribution and its parameters.
+    By default, the following distributions are tried: normal, cosine,
+    exponential, exponential power, gamma, left-skewed Gumbel, right-skewed
+    Gumbel, power law, triangular, trapezoidal, and uniform.
+
+    The best fit is determined by the sum of squared errors (SSE) between the
+    histogram and the probability density function (PDF) of the distribution.
+
+    Returns the best fit distribution and its parameters in a named tuple.
 
     Args:
         a (array): The data.
         bins (int): The number of bins to use for the histogram.
 
     Returns:
         tuple: The best fit distribution and its parameters.
@@ -86,15 +93,20 @@
     Distribution = namedtuple('Distribution', ['name', 'shape', 'loc', 'scale'])
     return Distribution(best_dist.name, shape, μ, σ)
 
 
 def wasserstein_ovr(a: ArrayLike, groups: ArrayLike=None, standardize: bool=False) -> np.ndarray:
     """
     First Wasserstein distance between each group in `a` vs the rest of `a`
-    ('one vs rest' or OVR).
+    ('one vs rest' or OVR). The groups are provided by `groups`, which must be
+    a 1D array of group labels, the same length as `a`.
+
+    The Wasserstein distance is a measure of the distance between two
+    probability distributions. It is also known as the earth mover's distance.
+    This function uses the implementation in `scipy.stats.wasserstein_distance`.
 
     The results are in `np.unique(a)` order.
 
     Data should be standardized for results you can compare across different
     measurements. The function does not apply standardization by default.
 
     Returns K scores for K groups.
@@ -121,15 +133,20 @@
         dists.append(dist)
     return np.array(dists)
 
 
 def wasserstein_ovo(a: ArrayLike, groups: ArrayLike=None, standardize: bool=False) -> np.ndarray:
     """
     First Wasserstein distance between each group in `a` vs each other group
-    ('one vs one' or OVO).
+    ('one vs one' or OVO). The groups are provided by `groups`, which must be
+    a 1D array of group labels, the same length as `a`.
+
+    The Wasserstein distance is a measure of the distance between two
+    probability distributions. It is also known as the earth mover's distance.
+    This function uses the implementation in `scipy.stats.wasserstein_distance`.
 
     The results are in the order given by `combinations(np.unique(groups),
     r=2)`, which matches the order of `scipy.spatial.distance` metrics.
 
     Data should be standardized for results you can compare across different
     measurements. The function does not apply standardization by default.
 
@@ -161,32 +178,14 @@
     dists = []
     for (group_1, group_2) in combinations(np.unique(groups), r=2):
         dist = wasserstein_distance(a[groups==group_1], a[groups==group_2])
         dists.append(dist)
     return np.array(dists)
 
 
-def wasserstein_multi(X: ArrayLike, groups: ArrayLike=None) -> np.ndarray:
-    """
-    Compute the multivariate (first) Wasserstein distance between groups.
-
-    Returns the distance matrix for all pairwise distances ('squareform').
-
-    Args:
-        X (array): The data. Must be a 2D array, or a sequence of 2D arrays.
-            If the latter, then the groups are implicitly assumed to be the
-            datasets in the sequence and the `groups` argument is ignored.
-        groups (array): The group labels.
-
-    Returns:
-        array: The 2D array of pairwise Wasserstein distance scores.
-    """
-    raise NotImplementedError()
-
-
 def wasserstein(X: ArrayLike,
                 groups: ArrayLike=None,
                 method: str='ovr', 
                 standardize: bool=False,
                 reducer: Callable=None) -> np.ndarray:
     """
     Step over all features and apply the distance function to the groups.
@@ -195,14 +194,18 @@
 
     The function `reducer` is applied to the ovo result to reduce it to one
     value per group per feature. If you want the full array of each group
     against each other, either pass the identity function (`lambda x: x`,
     which adds an axis) or use `wasserstein_ovo()` directly, one feature at
     a time. Default function: `np.mean`.
 
+    The Wasserstein distance is a measure of the distance between two
+    probability distributions. It is also known as the earth mover's distance.
+    This function uses the implementation in `scipy.stats.wasserstein_distance`.
+
     Args:
         X (array): The data. Must be a 2D array, or a sequence of 2D arrays.
             If the latter, then the groups are implicitly assumed to be the
             datasets in the sequence and the `groups` argument is ignored.
         groups (array): The group labels.
         method (str or func): The method to use. Can be 'ovr', 'ovo', or a
             function.
@@ -262,17 +265,14 @@
     if groups is None:
         raise ValueError("Must provide a 1D array of group labels if X is a 2D array.")
     n_groups = np.unique(groups).size
 
     if n_groups < 2:
         raise ValueError("Must have 2 or more groups.")
 
-    if method == 'multi':
-        return wasserstein_multi(X, groups=groups)
-
     methods = {
         'ovr': wasserstein_ovr,
         'ovo': wasserstein_ovo,
     }
     func = methods.get(method, method)
 
     if reducer is None:
@@ -288,15 +288,16 @@
         dist_arrs.append(dists)
 
     return np.swapaxes(dist_arrs, 0, 1)
 
 
 def bw_silverman(a: ArrayLike) -> float:
     """
-    Calculate the Silverman bandwidth.
+    Calculate the Silverman bandwidth, a popular rule of thumb for kernel
+    density estimation bandwidth.
 
     Silverman, BW (1981), "Using kernel density estimates to investigate
     multimodality", Journal of the Royal Statistical Society. Series B Vol. 43,
     No. 1 (1981), pp. 97-99.
 
     Args:
         a (array): The data.
@@ -311,15 +312,16 @@
     """
     n, d = np.array(a).size, 1
     return np.power(n, -1 / (d + 4))
 
 
 def bw_scott(a: ArrayLike) -> float:
     """
-    Calculate the Scott bandwidth.
+    Calculate the Scott bandwidth, a popular rule of thumb for kernel
+    density estimation bandwidth.
 
     Args:
         a (array): The data.
     
     Returns:
         float: The Scott bandwidth.
 
@@ -333,14 +335,17 @@
 
 
 def cv_kde(a: ArrayLike, n_bandwidths: int=20, cv: int=10) -> float:
     """
     Run a cross validation grid search to identify the optimal bandwidth for
     the kernel density estimation.
 
+    Searches between half the minimum of the Silverman and Scott bandwidths,
+    and twice the maximum. Checks `n_bandwidths` bandwidths, default 20.
+
     Args:
         a (array): The data.
         n_bandwidths (int): The number of bandwidths to try. Default 20.
         cv (int): The number of cross validation folds. Default 10.
 
     Returns:
         float. The optimal bandwidth.
@@ -412,15 +417,20 @@
     log_density = model.score_samples(x)
 
     return np.squeeze(x), np.exp(log_density)
 
 
 def get_kde(a: ArrayLike, method: str='scott') -> tuple[np.ndarray, np.ndarray]:
     """
-    Get the kernel density estimation for the data.
+    Get a kernel density estimation for the data. By default, the bandwidth is
+    estimated using the Scott rule of thumb. Other options are the Silverman
+    rule of thumb, or cross validation (using the `cv_kde()` function).
+
+    This function is a wrapper for `fit_kde()`, with convenient options for
+    bandwidth estimation.
 
     Args:
         a (array): The data.
         method (str): The rule of thumb for bandwidth estimation. Must be one
             of 'silverman', 'scott', or 'cv'. Default 'scott'.
 
     Returns:
@@ -444,14 +454,17 @@
 
 def find_large_peaks(x: ArrayLike, y: ArrayLike, threshold: float=0.1) -> tuple[np.ndarray, np.ndarray]:
     """
     Find the peaks in the array. Returns the values of x and y at the largest
     peaks, using threshold &times; max(peak amplitudes) as the cut-off. That is,
     peaks smaller than that are not returned.
 
+    Uses `scipy.signal.find_peaks()`, with convenient options for thresholding,
+    and returns the x and y values of the peaks in a named tuple.
+
     Args:
         x (array): The x values.
         y (array): The y values.
         threshold (float): The threshold for peak amplitude. Default 0.1.
 
     Returns:
         tuple: (x_peaks, y_peaks). Arrays representing the x and y values of
@@ -475,15 +488,21 @@
         z, h = np.array([]), np.array([])
     Peaks = namedtuple('Peaks', ['positions', 'heights'])
     return Peaks(z, h)
 
 
 def kde_peaks(a: ArrayLike, method: str='scott', threshold: float=0.1) -> tuple[np.ndarray, np.ndarray]:
     """
-    Find the peaks in the kernel density estimation.
+    Find the peaks in the kernel density estimation. This might help you
+    identify the modes in the data.
+
+    Wraps `get_kde()` and  `find_large_peaks()` to find the peaks in the
+    kernel density estimation. By default, the bandwidth is estimated using
+    the Scott rule of thumb. Other options are the Silverman rule of thumb, or
+    cross validation (using the `cv_kde()` function).        
 
     Args:
         a (array): The data.
         method (str): The rule of thumb for bandwidth estimation. Must be one
             of 'silverman', 'scott', or 'cv'. Default 'scott'.
         threshold (float): The threshold for peak amplitude. Default 0.1.
 
@@ -504,15 +523,22 @@
 
 
 def is_multimodal(a: ArrayLike,
                   groups:Optional[ArrayLike]=None,
                   method: str='scott',
                   threshold: float=0.1) -> Union[bool, np.ndarray]:
     """
-    Test if the data is multimodal.
+    Test if the data is multimodal by looking for peaks in the kernel density
+    estimation. If there is more than one peak, the data are considered
+    multimodal.
+
+    If groups are passed, the data are partitioned by group and tested
+    separately. The result is an array of booleans, one per group.
+
+    Wraps `kde_peaks()` to find the peaks in the kernel density estimation.
 
     Args:
         a (array): The data.
         groups (array): Group labels, if the data is to be partitioned before
             testing.
         method (str): The rule of thumb for bandwidth estimation. Must be one
             of 'silverman', 'scott', or 'cv'. Default 'scott'.
```

### Comparing `redflag-0.4.2rc1/src/redflag/imbalance.py` & `redflag-0.5.0rc1/src/redflag/imbalance.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Measuring the Class-imbalance Extent of Multi-class Problems
 Pattern Recognition Letters 98 (2017)
 https://doi.org/10.1016/j.patrec.2017.08.002
 
 Author: Matt Hall, scienxlab.org
 Licence: Apache 2.0
 
-Copyright 2023 Redflag contributors
+Copyright 2024 Redflag contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -128,22 +128,23 @@
     """
     ζ, e = empirical_distribution(a, classes=classes)
     return sum(ζ >= e), sum(ζ < e)
 
 
 def divergence(method: str='hellinger') -> Callable:
     """
-    Compute the divergence between two discrete probability distributions. 
+    Provides a function for computing the divergence between two discrete
+    probability distributions. Used by `imbalance_degree()`.
 
     `method` can be a string from:
-        -  hellinger: Recommended.
-        - euclidean: Not recommended.
-        - manhattan: Recommended.
-        - kl: Not recommended.
-        - tv: Recommended.
+        - `hellinger`: Recommended by Ortigosa-Hernandez et al. (2017).
+        - `euclidean`: Not recommended.
+        - `manhattan`: Recommended.
+        - `kl`: Not recommended.
+        - `tv`: Recommended.
 
     If `method` is a function, this function just hands it back.
 
     Args:
         ζ (array): The actual distribution.
         e (array): The expected distribution.
         method (str): The method to use.
@@ -162,15 +163,16 @@
         'tv': lambda x, y: np.sum(np.abs(x - y)) / 2,  # Total variation.
     }
     return functions.get(method, method)
 
 
 def furthest_distribution(a: ArrayLike, classes: Optional[ArrayLike]=None) -> np.ndarray:
     """
-    Compute the IR. Equation 6 in Ortigosa-Hernandez et al. (2017).
+    Compute the furthest distribution from `a`; used by `imbalance_degree()`.
+    See Ortigosa-Hernandez et al. (2017).
 
     Args:
         a (array): A list of class labels.
         classes (array): A list of classes, in the event that `a` does not
             contain all of the classes, or if you want to ignore some classes
             in `a` (not recommended) you can omit them from this list.
 
@@ -245,15 +247,16 @@
     div = divergence(method)
     epsilon = 1e-12
     return (div(ζ, e) / (epsilon + div(i, e))) + (m - 1)
 
 
 def minority_classes(a: ArrayLike, classes: Optional[ArrayLike]=None) -> np.ndarray:
     """
-    Get the minority classes.
+    Get the minority classes, based on the empirical distribution.
+    The classes are listed in order of increasing frequency.
 
     Args:
         a (array): A list of class labels.
         classes (array): A list of classes, in the event that `a` does not
             contain all of the classes, or if you want to ignore some classes
             in `a` (not recommended) you can omit them from this list.
```

### Comparing `redflag-0.4.2rc1/src/redflag/importance.py` & `redflag-0.5.0rc1/src/redflag/importance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Feature importance metrics.
 
 Author: Matt Hall, scienxlab.org
 Licence: Apache 2.0
 
-Copyright 2023 Redflag contributors
+Copyright 2024 Redflag contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -19,106 +19,101 @@
 limitations under the License.
 """
 from typing import Optional
 
 import numpy as np
 from numpy.typing import ArrayLike
 from sklearn.inspection import permutation_importance
-from sklearn.linear_model import Lasso
+from sklearn.linear_model import LinearRegression
 from sklearn.ensemble import RandomForestRegressor
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.neighbors import KNeighborsRegressor
 from sklearn.linear_model import LogisticRegression
 from sklearn.ensemble import RandomForestClassifier
 
 from .target import is_continuous
 from .utils import split_and_standardize
+from .utils import aggregate
 
 
 def feature_importances(X: ArrayLike, y: ArrayLike=None,
-                        n: int=3, task: Optional[str]=None,
+                        task: Optional[str]=None,
                         random_state: Optional[int]=None,
-                        standardize: bool=True) -> np.ndarray:
+    ) -> np.ndarray:
     """
-    Measure feature importances on a task, given X and y.
+    Estimate feature importances on a supervised task, given X and y.
 
     Classification tasks are assessed with logistic regression, a random
     forest, and KNN permutation importance. Regression tasks are assessed with
-    lasso regression, a random forest, and KNN permutation importance. In each
-    case, the `n` normalized importances with the most variance are averaged.
+    lasso regression, a random forest, and KNN permutation importance.
+
+    The scores from these assessments are normalized, and the normalized
+    sum is returned.
+
+    See the Tutorial in the documentation for more information.
 
     Args:
         X (array): an array representing the data.
         y (array or None): an array representing the target. If None, the task
             is assumed to be an unsupervised clustering task.
-        n (int): the number of tests to average. Only the n tests with the
-            highest variance across features are kept.
         task (str or None): either 'classification' or 'regression'. If None,
             the task will be inferred from the labels and a warning will show
             the assumption being made.
         random_state (int or None): the random state to use.
-        standardize (bool): whether to standardize the data. Default is True.
 
     Returns:
         array: The importance of the features, in the order in which they
             appear in X.
 
     Examples:
         >>> X = [[0, 0, 0], [0, 1, 1], [0, 2, 0], [0, 3, 1], [0, 4, 0], [0, 5, 1], [0, 7, 0], [0, 8, 1], [0, 8, 0]]
         >>> y = [5, 15, 25, 35, 45, 55, 80, 85, 90]
         >>> feature_importances(X, y, task='regression', random_state=42)
-        array([0.        , 0.99416839, 0.00583161])
+        array([0.       , 0.9831828, 0.0168172])
         >>> y = ['a', 'a', 'a', 'b', 'b', 'b', 'c', 'c', 'c']
         >>> x0, x1, x2 = feature_importances(X, y, task='classification', random_state=42)
         >>> x1 > x2 > x0  # See Issue #49 for why this test is like this.
         True
     """
     if y is None:
         raise NotImplementedError('Unsupervised importance is not yet implemented.')
 
     if task is None:
         task = 'regression' if is_continuous(y) else 'classification'
 
     # Split the data and ensure it is standardized.
-    if standardize:
-        X, X_train, X_val, y, y_train, y_val = split_and_standardize(X, y, random_state=random_state)
+    X, X_train, X_val, y, y_train, y_val = split_and_standardize(X, y, random_state=random_state)
 
     # Train three models and gather the importances.
     imps: list = []
     if task == 'classification':
         imps.append(np.abs(LogisticRegression(random_state=random_state).fit(X, y).coef_.sum(axis=0)))
         imps.append(RandomForestClassifier(random_state=random_state).fit(X, y).feature_importances_)
         model = KNeighborsClassifier().fit(X_train, y_train)
         r = permutation_importance(model, X_val, y_val, n_repeats=8, scoring='f1_weighted', random_state=random_state)
         imps.append(r.importances_mean)
     elif task == 'regression':
-        # Need data to be scaled, but don't necessarily want to scale entire dataset.
-        imps.append(np.abs(Lasso(random_state=random_state).fit(X, y).coef_))
+        imps.append(np.abs(LinearRegression().fit(X, y).coef_))
         imps.append(RandomForestRegressor(random_state=random_state).fit(X, y).feature_importances_)
         model = KNeighborsRegressor().fit(X_train, y_train)
         r = permutation_importance(model, X_val, y_val, n_repeats=8, scoring='neg_mean_squared_error', random_state=random_state)
-        if not all(r.importances_mean < 0):
-            r.importances_mean[r.importances_mean < 0] = 1e-9
-            imps.append(r.importances_mean)
+        imps.append(r.importances_mean)
 
+    # Eliminate negative values and aggregate.
     imps = np.array(imps)
-
-    # Normalize the rows by the sum of *only positive* elements.
-    normalizer = np.where(imps>0, imps, 0).sum(axis=1)
-    imps /= normalizer[:, None]
-
-    # Drop imps with smallest variance and take mean of what's left.
-    return np.nanmean(sorted(imps, key=lambda row: np.std(row))[-n:], axis=0)
+    imps[imps < 0] = 0
+    return aggregate(imps, normalize_input=True, normalize_output=True)
 
 
 def least_important_features(importances: ArrayLike,
                              threshold: Optional[float]=None) -> np.ndarray:
     """
     Returns the least important features, in order of importance (least
-        important first).
+    important first). The threshold controls how many features are returned.
+    Set it to None to set it automatically.
 
     Args:
         importances (array): the importance of the features, in the order in
             which they appear in X.
         threshold (float or None): the cutoff for the importance. If None, the
             cutoff is set to half the expectation of the importance (i.e. 0.5/M
             where M is the number of features).
@@ -144,15 +139,16 @@
     return np.array(list(least_important)).astype(int)
 
 
 def most_important_features(importances: ArrayLike,
                              threshold: Optional[float]=None) -> np.ndarray         :
     """
     Returns the indices of the most important features, in reverse order of
-        importance (most important first).
+    importance (most important first). The threshold controls how many features
+    are returned. Set it to None to set it automatically.
  
     Args:
         importances (array): the importance of the features, in the order in
             which they appear in X.
         threshold (float or None): the cutoff for the importance. If None,
             the cutoff is set to (M-1)/M where M is the number of features.
```

### Comparing `redflag-0.4.2rc1/src/redflag/independence.py` & `redflag-0.5.0rc1/src/redflag/independence.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Functions related to understanding row independence.
 
 Author: Matt Hall, scienxlab.org
 Licence: Apache 2.0
 
-Copyright 2023 Redflag contributors
+Copyright 2024 Redflag contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -20,24 +20,42 @@
 """
 import numpy as np
 from numpy.typing import ArrayLike
 
 
 def is_correlated(a: ArrayLike, n: int=20, s: int=20, threshold: float=0.1) -> bool:
     """
-    Check if a dataset is correlated. Uses s chunks of n samples.
+    Check if a dataset is auto-correlated. This function returns True if
+    the 1D input array `a` appears to be correlated to itself, perhaps
+    because it consists of measurements sampled at neighbouring points
+    in time or space, at a spacing short enough that samples are correlated.
+
+    If samples are correlated in this way, then the records in your dataset
+    may break the IID assumption implicit in much of statistics (though not
+    in specialist geostatistics or timeseries algorithms). This is not
+    necessarily a big problem, but it does mean you need to be careful
+    about how you split your data, for example a random split between train
+    and test will leak information from train to test, because neighbouring
+    samples are correlated.
+
+    This function inspects s random chunks of n samples, averaging the
+    autocorrelation coefficients across chunks. If the mean first non-zero
+    lag is greater than the threshold, the array may be autocorrelated.
+
+    See the Tutorial in the documentation for more about how to use this
+    function.
 
     Args:
         a (array): The data.
         n (int): The number of samples per chunk.
         s (int): The number of chunks.
         threshold (float): The auto-correlation threshold.
 
     Returns:
-        bool: True if the data are correlated.
+        bool: True if the data are autocorrelated.
 
     Examples:
         >>> is_correlated([7, 1, 6, 8, 7, 6, 2, 9, 4, 2])
         False
         >>> is_correlated([1, 2, 1, 7, 6, 8, 6, 2, 1, 1])
         True
     """
```

### Comparing `redflag-0.4.2rc1/src/redflag/markov.py` & `redflag-0.5.0rc1/src/redflag/markov.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Functions related to Markov chains. This code was originally implemented in
 https://github.com/agilescientific/striplog.
 
 Author: Matt Hall, scienxlab.org
 Licence: Apache 2.0
 
-Copyright 2023 Matt Hall
+Copyright 2024 Matt Hall
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -24,29 +24,48 @@
 import numpy as np
 import scipy.stats
 
 
 def observations(seq_of_seqs, states, step=1, include_self=False):
     """
     Compute observation matrix.
+
+    Returns the matrix of transition counts between states.
+
+    Args:
+        seq_of_seqs (list-like): A list-like, or list-like of list-likes.
+            The inner list-likes represent sequences of states.
+            For example, can be a string or list of strings, or
+            a list or list of lists.
+        states (list-like): A list or array of the names of the states.
+            If not provided, it will be inferred from the data.
+        step (integer): The distance to step. Default is 1: use
+            the previous state only. If 2, then the previous-but-
+            one state is used as well as the previous state (and
+            the matrix has one more dimension).
+        include_self (bool): Whether to include self-to-self
+            transitions (default is `False`: do not include them).
+
+    Returns:
+        ndarray. The observation matrix.
     """
     O = np.zeros(tuple(states.size for _ in range(step+1)))
     for seq in seq_of_seqs:
         seq = np.array(seq)
         _, integer_seq = np.where(seq.reshape(-1, 1) == states)
         for idx in zip(*[integer_seq[n:] for n in range(step+1)]):
             if (not include_self) and (0 in np.diff(idx)):
                 continue
             O[idx] += 1
     return O
 
 
 def hollow_matrix(M):
     """
-    Return hollow matrix (zeros on diagonal).
+    Utility funtion to return hollow matrix (zeros on diagonal).
 
     Args
         M (ndarray): a 'square' ndarray.
 
     Returns
         ndarray. The same array with zeros on the diagonal.
     """
@@ -151,56 +170,80 @@
         Compute frequencies from counts.
         """
         epsilon = 1e-12
         return (C.T / (epsilon+np.sum(C.T, axis=0))).T
 
     @staticmethod
     def _stop_iter(a, b, tol=0.01):
+        """
+        Stopping criterion for Powers & Easterling method.
+        """
         a_small = np.all(np.abs(a[-1] - a[-2]) < tol*a[-1])
         b_small = np.all(np.abs(b[-1] - b[-2]) < tol*b[-1])
         return (a_small and b_small)
 
     @property
     def _index_dict(self):
+        """
+        A dictionary mapping the states to their indices.
+        """
         if self.states is None:
             return {}
         return {self.states[index]: index for index in range(len(self.states))}
 
     @property
     def _state_dict(self):
+        """
+        A dictionary mapping the indices to their states.
+        """
         if self.states is None:
             return {}
         return {index: self.states[index] for index in range(len(self.states))}
 
     @property
     def observed_freqs(self):
+        """
+        The observed frequencies of each state, given the previous state.
+        """
         return self._compute_freqs(self.observed_counts)
 
     @property
     def expected_freqs(self):
+        """
+        The expected frequencies of each state, given the previous state.
+        """
         return self._compute_freqs(self.expected_counts)
 
     @property
     def _state_counts(self):
+        """
+        The number of times each state occurs.
+        """
         s = self.observed_counts.copy()
 
         # Deal with more than 2 dimensions.
         for _ in range(self.observed_counts.ndim - 2):
             s = np.sum(s, axis=0)
 
         a = np.sum(s, axis=0)
         b = np.sum(s, axis=1)
         return np.maximum(a, b)
 
     @property
     def _state_probs(self):
+        """
+        The probability of each state.
+        """
         return self._state_counts / np.sum(self._state_counts)
 
     @property
     def normalized_difference(self):
+        """
+        The normalized difference between observed and expected counts.
+        """
         O = self.observed_counts
         E = self.expected_counts
         epsilon = 1e-12
         return (O - E) / np.sqrt(E + epsilon)
 
     @classmethod
     def from_sequence(cls,
@@ -209,15 +252,15 @@
                       strings_are_states=False,
                       include_self=False,
                       step=1,
                       ):
         """
         Parse a sequence and make the transition matrix of the specified order.
 
-        **Provide sequence(s) ordered in upwards direction.**
+        You must provide sequence(s) in causal order (e.g. time order).
 
         Args:
             sequence (list-like): A list-like, or list-like of list-likes.
                 The inner list-likes represent sequences of states.
                 For example, can be a string or list of strings, or
                 a list or list of lists.
             states (list-like): A list or array of the names of the states.
@@ -269,15 +312,15 @@
         Returns:
             str. One realization of the next state.
         """
         return np.random.choice(self.states,
                                 p=self._conditional_probs(current_state)
                                 )
 
-    def generate_states(self, n=10, current_state=None):
+    def generate_states(self, n: int = 10, current_state=None):
         """
         Generates the next states of the system.
 
         Args:
             n (int): The number of future states to generate.
             current_state (str): The state of the current random variable.
 
@@ -303,15 +346,15 @@
         try:
             E = self._compute_expected_pe()
         except:
             E = self._compute_expected_mc()
 
         return E
 
-    def _compute_expected_mc(self, n=100000):
+    def _compute_expected_mc(self, n: int = 100000):
         """
         If we can't use Powers & Easterling's method, and it's possible there's
         a way to extend it to higher dimensions (which we have for step > 1),
         the next best thing might be to use brute force and just compute a lot
         of random sequence transitions, given the observed proportions. This is
         what P & E's method tries to estimate iteratively.
 
@@ -320,15 +363,15 @@
         """
         seq = np.random.choice(self.states, size=n, p=self._state_probs)
         E = observations(np.atleast_2d(seq), self.states, step=self.step, include_self=self.include_self)
         if not self.include_self:
             E = hollow_matrix(E)
         return np.sum(self.observed_counts) * E / np.sum(E)
 
-    def _compute_expected_pe(self, max_iter=100):
+    def _compute_expected_pe(self, max_iter: int = 100):
         """
         Compute the independent trials matrix, using method of
         Powers & Easterling 1982.
         """
         m = len(self.states)
         M = self.observed_counts
         a, b = [], []
@@ -357,33 +400,33 @@
             return E
 
     @property
     def degrees_of_freedom(self) -> int:
         m = len(self.states)
         return (m - 1)**2 - m
 
-    def _chi_squared_critical(self, q=0.95, df=None):
+    def _chi_squared_critical(self, q: float = 0.95, df: int = None) -> float:
         """
         The chi-squared critical value for a confidence level q
         and degrees of freedom df.
         """
         if df is None:
             df = self.degrees_of_freedom
         return scipy.stats.chi2.ppf(q=q, df=df)
 
-    def _chi_squared_percentile(self, x, df=None):
+    def _chi_squared_percentile(self, x: float, df: int = None) -> float:
         """
-        The chi-squared critical value for a confidence level q
-        and degrees of freedom df.
+        The chi-squared percentile for a value x and degrees of
+        freedom df.
         """
         if df is None:
             df = self.degrees_of_freedom
         return scipy.stats.chi2.cdf(x, df=df)
 
-    def chi_squared(self, q=0.95):
+    def chi_squared(self, q: float = 0.95) -> tuple:
         """
         The chi-squared statistic for the given transition
         frequencies.
 
         Also returns the critical statistic at the given confidence
         level q (default 95%).
```

### Comparing `redflag-0.4.2rc1/src/redflag/outliers.py` & `redflag-0.5.0rc1/src/redflag/outliers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Functions related to understanding features.
 
 Author: Matt Hall, scienxlab.org
 Licence: Apache 2.0
 
-Copyright 2023 Redflag contributors
+Copyright 2024 Redflag contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -18,28 +18,34 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from __future__ import annotations
 
 from typing import Optional
 from functools import reduce, partial
+import warnings
 
 import numpy as np
 from numpy.typing import ArrayLike
 from sklearn.neighbors import LocalOutlierFactor
 from sklearn.ensemble import IsolationForest
 from sklearn.covariance import EllipticEnvelope
 
 from .utils import stdev_to_proportion, proportion_to_stdev
 from .utils import get_idx
 
 
 def mahalanobis(X: ArrayLike, correction: bool=False) -> np.ndarray:
     """
-    Compute the Mahalanobis distances of a dataset.
+    Compute the Mahalanobis distances of every record (row) in a 2D dataset.
+
+    If X has a single feature, this is equivalent to computing the Z-scores
+    of the data. For more features, the Mahalanobis distance is the distance
+    of each point from the centroid of the data, in units analogous to the
+    standard deviation. It is a multivariate analog of the Z-score.
 
     The empirical covariance correction factor suggested by Rousseeuw and
     Van Driessen may be optionally applied by setting `correction=True`.
 
     Args:
         X (array): The data. Must be a 2D array, shape (n_samples, n_features).
         correction (bool): Whether to apply the empirical covariance correction.
@@ -71,20 +77,21 @@
                          p: float=0.99,
                          threshold: Optional[float]=None,
                          ) -> np.ndarray:
     """
     Find outliers given samples and a threshold in multiples of stdev.
     Returns -1 for outliers and 1 for inliers (to match the sklearn API).
 
-    For univariate data, we expect this many points outside:
-        - 1 sd: expect 31.7 points in 100
-        - 2 sd: 4.55 in 100
-        - 3 sd: 2.70 in 1000
-        - 4 sd: 6.3 in 100,000
-        - 4.89163847 sd: 1 in 1 million
+    For univariate data, we expect this many points outside (in units of
+    standard deviation, and with equivalent p-values):
+        - 1 sd: expect 31.7 points in 100 (p = 1 - 0.317 = 0.683)
+        - 2 sd: 4.55 in 100 (p = 1 - 0.0455 = 0.9545)
+        - 3 sd: 2.70 in 1000 (p = 1 - 0.0027 = 0.9973)
+        - 4 sd: 6.3 in 100,000 (p = 1 - 0.000063 = 0.999937)
+        - 4.89163847 sd: 1 in 1 million (p = 1 - 0.000001 = 0.999999)
         - 5 sd: 5.7 in 10 million datapoints
         - 6 sd: 2.0 in 1 billion points
 
     Args:
         X (array): The data. Can be a 2D array, shape (n_samples, n_features),
             or a 1D array, shape (n_samples).
         p (float): The probability threshold, in the range [0, 1]. This value
@@ -122,37 +129,38 @@
     outliers = np.full(z.shape, 1)
     outliers[idx] = -1
 
     return outliers
 
 
 def get_outliers(a: ArrayLike,
-                 method: str='iso',
+                 method: Optional[str]=None, # Can change to 'mah' in 0.6.0.
                  p: float=0.99,
                  threshold: Optional[float]=None,
                  ) -> np.ndarray:
     """
     Returns outliers in the data, considering all of the features. What counts
     as an outlier is determined by the threshold, which is in multiples of
     the standard deviation. (The conversion to 'contamination' is approximate.)
 
-    This function requires the scikit-learn package.
-
-    Methods: 'iso' (isolation forest), 'lof' (local outlier factor), 'ee'
-    (elliptic envelope), or 'mah' (Mahanalobis distance, the default), or pass
-    a function that returns an array of outlier flags (-1 for outliers and 1
+    Methods: 'iso' (isolation forest), 'lof' (local outlier factor),
+    'ee' (elliptic envelope), or 'mah' (Mahanalobis distance, the default), or
+    pass a function that returns an array of outlier flags (-1 for outliers and 1
     for inliers, matching the `sklearn` convention). You can also pass 'any',
     which will try all three outlier detection methods and return the outliers
     which are detected by any of them, or 'all', which will return the outliers
-    which are common to all four methods.
+    which are common to all four methods. That is, 'all' is a rather conservative
+    outlier detector, 'any' is rather liberal, and both of these are slower
+    than choosing a single algorithm.
 
     Args:
         a (array): The data.
-        method (str): The method to use. Can be 'iso', 'lof', 'ee', 'mah',
-            or a function that returns a Boolean array of outlier flags.
+        method (str): The method to use. Can be 'mah' (the default), 'iso', 'lof',
+            'ee', 'any', 'all', or a function that returns a Boolean array of
+            outlier flags.
         p (float): The probability threshold, in the range [0, 1]. This value
             is ignored if `threshold` is not None; in this case, `p` will be
             computed using `utils.stdev_to_proportion(threshold)`.
         threshold (float): The threshold in Mahalanobis distance, analogous to
             multiples of standard deviation for a single variable. If not None,
             the threshold will be used to compute `p`.
 
@@ -168,14 +176,20 @@
         >>> get_outliers(3 * data + [100], method='mah')
         array([33])
         >>> get_outliers(3 * data + [100], method='any')
         array([33])
         >>> get_outliers(3 * data + [100], method='all')
         array([33])
     """
+    if method is None:
+        # Was called with the default method, which changed in 0.4.3
+        method = 'mah'
+        warnings.warn('The default method for get_outliers has changed to "mah". '
+                      'Please specify the method explicitly to avoid this warning.',
+                      DeprecationWarning, stacklevel=2)
     if p >= 1 or p < 0:
         raise ValueError('p must be in the range [0, 1).')
     a = np.asarray(a)
     if a.ndim == 1:
         a = a.reshape(-1, 1)
     if threshold is None:
         expect = 1 - p
@@ -202,15 +216,21 @@
 
 def expected_outliers(n: int,
                       d: int=1,
                       p: float=0.99,
                       threshold: Optional[float]=None,
                       ) -> int:
     """
-    Expected number of outliers in a dataset.
+    Expected number of outliers in a dataset, under the assumption that the
+    data are multivariate-normally distributed. What counts as an outlier is
+    determined by the threshold, which is in multiples of the standard
+    deviation, or by the p-value, which is the probability of a point being
+    an outlier. Note that passing p = 0.99 does not necessarily mean that
+    1% of the points will be outliers, only that 1% of the points are expected
+    to be outliers, on average, if the data are normally distributed.
     
     Args:
         n (int): The number of samples.
         d (int): The number of features. Note that if threshold is None, this
             value is not used in the calculation. Default: 1.
         p (float): The probability threshold, in the range [0, 1]. This value
             is ignored if `threshold` is not None and `p` will be computed
@@ -235,17 +255,19 @@
                  p: float=0.99,
                  threshold: Optional[float]=None,
                  factor: float=1.0,
                  ) -> bool:
     """
     Use Mahalanobis distance to determine if there are more outliers than
     expected at the given confidence level or Mahalanobis distance threshold.
+    A Boolean wrapper around `expected_outliers` and `get_outliers`.
 
     Args:
-        a (array): The data.
+        a (array): The data. If 2D, the rows are samples and the columns are
+            features. If 1D, the data are assumed to be univariate.
         p (float): The probability threshold, in the range [0, 1]. This value
             is ignored if `threshold` is not None and `p` will be computed
             using `utils.stdev_to_proportion(threshold)`. Default: 0.99.
         threshold (float): The threshold in Mahalanobis distance, analogous to
             multiples of standard deviation for a single variable. If not None,
             the threshold will be used to compute `p`.
         factor (float): The factor by which to multiply the expected number of
```

### Comparing `redflag-0.4.2rc1/src/redflag/pandas.py` & `redflag-0.5.0rc1/src/redflag/pandas.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Pandas accessors.
 
 Author: Matt Hall, scienxlab.org
 Licence: Apache 2.0
 
-Copyright 2023 Redflag contributors
+Copyright 2024 Redflag contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -85,16 +85,14 @@
                              threshold=threshold,
                              method=method,
                              classes=classes
                              )
 
     @docstring_from(is_ordered)
     def is_ordered(self, q=0.95):
-        if is_continuous(self._obj):
-            warnings.warn('The Series does not seem categorical.')
         return is_ordered(self._obj, q=q)
 
     @docstring_from(dummy_scores)
     def dummy_scores(self, task='auto', random_state=None):
         return dummy_scores(self._obj, task=task, random_state=random_state)
 
     def report(self, random_state=None):
@@ -117,34 +115,35 @@
 @register_dataframe_accessor("redflag")
 class DataFrameAccessor:
     def __init__(self, pandas_obj):
         self._obj = pandas_obj
 
     @docstring_from(feature_importances)
     def feature_importances(self, features=None, target=None,
-                            n: int=3, task: Optional[str]=None,
+                            task: Optional[str]=None,
                             random_state: Optional[int]=None,
-                            standardize: bool=True):
+                            ):
         if target is None:
             raise ValueError('You must provide a target column.')
         else:
             y_ = self._obj[target]
             if is_continuous(y_):
                 task = 'regression'
             else:
                 task = 'classification'
         if len(y_.shape) > 1:
             raise NotImplementedError('Multilabel targets are not supported.')
         if features is None and target is not None:
             X_ = self._obj.drop(columns=target)
         else:
             X_ = self._obj[features]
-        return feature_importances(X_, y_, n=n, task=task,
-                                   random_state=random_state,
-                                   standardize=standardize)
+        return feature_importances(X_, y_,
+                                   task=task,
+                                   random_state=random_state
+                                   )
 
 
     def correlation_detector(self, features=None, target=None, n=20, s=20, threshold=0.1):
         """
         This is an experimental feature.
         """
         if target is not None:
@@ -157,11 +156,11 @@
         if features is None and target is not None:
             X_ = self._obj.drop(target, axis=1).values
         else:
             X_ = self._obj[features].values
 
         for i, x in enumerate(X_.T):
             if is_correlated(x, n=n, s=s, threshold=threshold):
-                warnings.warn(f'Feature {i} appears to be autocorrelated.',stacklevel=2)
+                warnings.warn(f'🚩 Feature {i} appears to be autocorrelated.', stacklevel=2)
 
         # There is probably something more useful to return.
         return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `redflag-0.4.2rc1/src/redflag/sklearn.py` & `redflag-0.5.0rc1/src/redflag/sklearn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Scikit-learn components.
 
 Author: Matt Hall, scienxlab.org
 Licence: Apache 2.0
 
-Copyright 2023 Redflag contributors
+Copyright 2024 Redflag contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `redflag-0.4.2rc1/src/redflag/target.py` & `redflag-0.5.0rc1/src/redflag/target.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Functions related to understanding the target and the type of task.
 
 Author: Matt Hall, scienxlab.org
 Licence: Apache 2.0
 
-Copyright 2023 Redflag contributors
+Copyright 2024 Redflag contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -215,16 +215,17 @@
         random_state (int): A seed for the random number generator.
 
     Returns:
         dict: A dictionary of scores.
 
     Examples:
         >>> y = [1, 1, 1, 1, 1, 2, 2, 2, 3, 3]
-        >>> dummy_classification_scores(y, random_state=42)
-        {'most_frequent': {'f1': 0.3333333333333333, 'roc_auc': 0.5}, 'stratified': {'f1': 0.20000000000000004, 'roc_auc': 0.35654761904761906}}
+        >>> scores = dummy_classification_scores(y, random_state=42)
+        >>> scores['most_frequent']  # Precision issue with stratified test.
+        {'f1': 0.3333333333333333, 'roc_auc': 0.5}
     """
     result = {'most_frequent': {}, 'stratified': {}}
     y = np.asanyarray(y)
     if y.ndim > 1:
         raise ValueError("Multilabel target is not supported.")
     X = np.ones_like(y).reshape(-1, 1)  # X is not used by the model.
     for method, scores in result.items():
@@ -268,16 +269,21 @@
         scores['mean_squared_error'] = mean_squared_error(y, y_pred)
         scores['r2'] = r2_score(y, y_pred)
     return result
 
 
 def dummy_scores(y: ArrayLike, task='auto', random_state:Optional[int]=None) -> dict:
     """
-    Automatically decide whether y is continuous or categorical and call the
-    appropriate scoring function.
+    Provide scores from a 'dummy' (naive) model. This can be useful for
+    understanding the difficulty of the task. For example, if the dummy
+    model does well, then the task is probably easy and you should be
+    suspicious of any model that does not do well.
+
+    The function automatically decides whether y is continuous or categorical
+    and calls the appropriate scoring function.
 
     Args:
         y (array): A list of class labels.
         task (str): What kind of task: 'regression' or 'classification', or 'auto'
             to decide automatically. In general regression tasks predict continuous
             variables (e.g. temperature tomorrow), while classification tasks predict
             categorical variables (e.g. rain, cloud or sun).
```

### Comparing `redflag-0.4.2rc1/src/redflag/utils.py` & `redflag-0.5.0rc1/src/redflag/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Utility functions.
 
 Author: Matt Hall, scienxlab.org
 Licence: Apache 2.0
 
-Copyright 2023 Redflag contributors
+Copyright 2024 Redflag contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -398,15 +398,15 @@
 
     Returns:
         bool: True if the feature appears to be a Z-score.
 
     Example:
         >>> rng= np.random.default_rng(13)
         >>> a = rng.normal(size=100)
-        >>> is_standardized(a, atol=0.1)
+        >>> is_standardized(a, atol=0.1)   # doctest: +SKIP
         True
     """
     μ, σ = np.nanmean(a), np.nanstd(a)
     return bool((np.abs(μ) < atol) and (np.abs(σ - 1) < atol))
 
 
 def is_standard_normal(a: ArrayLike, confidence: float=0.8) -> bool:
@@ -638,7 +638,101 @@
         >>> has_monotonic([1, 1, 1, 2, 3, 4, 5, 5, 5])
         array([2, 3, 4, 5, 6])
     """
     a = np.diff(a)
     zeros = get_idx(np.diff(a) == 0)
     flats = [list(x)+[x[-1]+1, x[-1]+2] for x in consecutive(zeros) if x.size >= tolerance]
     return np.array(list(flatten(flats)), dtype=int)
+
+
+def aggregate(arr,
+              absolute=False,
+              rank_input=False,
+              rank_output=False,
+              normalize_input=False,
+              normalize_output=False,
+    ):
+    """
+    Compute the Borda count ranking from an N x M matrix representing 
+    N sets of rankings (or scores) for M candidates. This function 
+    aggregates the scores for each candidate and optionally normalizes 
+    them so that they sum to 1. The absolute value of the scores is 
+    considered if 'absolute' is set to True.
+
+    If you are providing rankings like [1 (best), 2, 3] and so on,
+    then set `rank=True`. If you also set `normalize_output` to `False`,
+    you will get Borda ranking scores.
+
+    If your score arrays contain negative numbers and you want a
+    large negative number to be considered 'strong', then set
+    `normalize_input` to `True`.
+
+    Arguments:
+        arr (array-like): An N x M matrix where N is the number of sets 
+            of rankings or scores, and M is the number of candidates. Each 
+            element represents the score of a candidate in a particular set.
+
+        absolute (bool, optional): If True, the absolute value of each 
+            score is considered. This is useful when a large negative 
+            number should be considered as a strong score. Defaults to False.
+
+        rank_input (bool, optional): If True, them the input is transformed
+            input ranking (such as [4 (best), 2, 3, ...]). Defaults to False.
+
+        rank_output (bool, optional): If True, the output will be the 
+            rankings of the aggregated scores instead of the scores themselves.
+            This converts the aggregated scores into a rank format (such as 
+            [3 (best), 1, 2, ...]). Defaults to False.
+
+        normalize_input (bool, optional): If True, each row of the input 
+            array will be normalized before aggregation. This is useful when 
+            the input array contains values in different ranges or units and 
+            should be normalized to a common scale. Defaults to False.
+
+        normalize_output (bool, optional): If True, the aggregated scores 
+            will be normalized so that they sum to 1. This is useful to 
+            understand the relative importance of each candidate's score. 
+            Defaults to False.
+
+    Returns:
+        numpy.ndarray: An array of length M containing the aggregated (and 
+            optionally normalized) scores for each of the M candidates.
+
+
+    Example:
+    >>> scores = ([
+    ...     [ 1,  0.25, 0],
+    ...     [ 4,  1.5,  0],
+    ...     [ 1, -0.25, 0]
+    ... ])
+    >>> aggregate(scores, normalize_output=True)
+    array([0.8, 0.2, 0. ])
+    >>> aggregate(scores, absolute=True, normalize_output=True)
+    array([0.75, 0.25, 0.  ])
+    >>> scores = ([
+    ...     [ 1,  0.25, 0],
+    ...     [ 4,  1.5,  0],
+    ...     [ 1, -0.25, 0]
+    ... ])
+    >>> aggregate(scores, rank_input=True, rank_output=True)
+    array([2, 1, 0])
+    """
+    arr = np.abs(arr) if absolute else np.array(arr)
+
+    if rank_input:
+        arr = np.argsort(np.argsort(arr, axis=1), axis=1)
+
+    if normalize_input:
+        s = arr.sum(axis=1)
+        s[s == 0] = 1e-12  # Division by zero.
+        arr = (arr.T / s).T
+        return aggregate(arr, normalize_output=normalize_output)
+
+    scores = np.atleast_2d(arr).sum(axis=0)
+
+    if rank_output:
+        scores = np.argsort(np.argsort(scores))
+    elif normalize_output:
+        s = np.sum(scores) or 1e-12
+        scores = scores / s
+
+    return scores
```

### Comparing `redflag-0.4.2rc1/src/redflag.egg-info/PKG-INFO` & `redflag-0.5.0rc1/src/redflag.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redflag
-Version: 0.4.2rc1
+Version: 0.5.0rc1
 Summary: Safety net for machine learning pipelines.
 Author-email: Matt Hall <kwinkunks@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -216,16 +216,16 @@
 Requires-Dist: myst_nb; extra == "dev"
 Requires-Dist: jupyter; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: seaborn; extra == "dev"
 
 # redflag
 
-[![Build and test](https://github.com/scienxlab/redflag/actions/workflows/build-test.yml/badge.svg)](https://github.com/scienxlab/redflag/actions/workflows/build-test.yml)
-[![Documentation](https://github.com/scienxlab/redflag/actions/workflows/publish-docs.yml/badge.svg)](https://github.com/scienxlab/redflag/actions/workflows/publish-docs.yml)
+[![Tests](https://github.com/scienxlab/redflag/actions/workflows/build-test.yml/badge.svg)](https://github.com/scienxlab/redflag/actions/workflows/build-test.yml)
+[![Docs](https://github.com/scienxlab/redflag/actions/workflows/publish-docs.yml/badge.svg)](https://github.com/scienxlab/redflag/actions/workflows/publish-docs.yml)
 [![PyPI version](https://img.shields.io/pypi/v/redflag.svg)](https://pypi.org/project/redflag/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/redflag.svg)](https://anaconda.org/conda-forge/redflag)
 [![PyPI versions](https://img.shields.io/pypi/pyversions/redflag.svg)](https://pypi.org/project/redflag/)
 [![PyPI license](https://img.shields.io/pypi/l/redflag.svg)](https://pypi.org/project/redflag/)
 
 🚩 `redflag` aims to be an automatic safety net for machine learning datasets. The vision is to accept input of a Pandas `DataFrame` or NumPy `ndarray` representing the input `X` and target `y` in a machine learning task. `redflag` will provide an analysis of each feature, and of the target, including aspects such as class imbalance, leakage, outliers, anomalous data patterns, threats to the IID assumption, and so on. The goal is to complement other projects like `pandas-profiling` and `greatexpectations`.
```

### Comparing `redflag-0.4.2rc1/src/redflag.egg-info/SOURCES.txt` & `redflag-0.5.0rc1/src/redflag.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 docs/what_is_redflag.md
 docs/_static/custom.css
 docs/_static/favicon.ico
 docs/_static/redflag.svg
 docs/_static/redflag_logo.png
 docs/_static/redflag_social.svg
 docs/notebooks/Basic_usage.ipynb
+docs/notebooks/Demo.ipynb
 docs/notebooks/Tutorial.ipynb
 docs/notebooks/Using_redflag_with_Pandas.ipynb
 docs/notebooks/Using_redflag_with_sklearn.ipynb
 docs/notebooks/_Pandas_accessor.ipynb
 src/redflag/__init__.py
-src/redflag/_version.py
 src/redflag/distributions.py
 src/redflag/imbalance.py
 src/redflag/importance.py
 src/redflag/independence.py
 src/redflag/markov.py
 src/redflag/outliers.py
 src/redflag/pandas.py
```

### Comparing `redflag-0.4.2rc1/tests/README.md` & `redflag-0.5.0rc1/tests/README.md`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/tests/conftest.py` & `redflag-0.5.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/tests/test_markov.py` & `redflag-0.5.0rc1/tests/test_markov.py`

 * *Files identical despite different names*

### Comparing `redflag-0.4.2rc1/tests/test_pandas.py` & `redflag-0.5.0rc1/tests/test_pandas.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     @null_decorator('foo')
     def f():
         return None
     assert f() is None
 
 
 def test_dummy_scores():
-    c_scores = c.redflag.dummy_scores()
-    r_scores = r.redflag.dummy_scores()
+    c_scores = c.redflag.dummy_scores(random_state=42)
+    r_scores = r.redflag.dummy_scores(random_state=42)
 
     assert c_scores['roc_auc'] - 0.6801587301587301 < 1e-12
     assert r_scores['mean_squared_error'] - 0.5710743801652893 < 1e-12
 
 
 def test_imbalance():
     assert c.redflag.is_imbalanced(threshold=0.24, method='tv')
@@ -31,15 +31,18 @@
 
     imb_degree = c.redflag.imbalance_degree()
     assert imb_degree - 1.25 < 1e-9
 
 
 def test_is_ordered():
     assert c.redflag.is_ordered()
-    with pytest.raises(ValueError, match="Cannot check order of continuous data."):
+
+
+def test_is_ordered_warns_for_continuous_data():
+    with pytest.raises(ValueError, match='Cannot check order of continuous data.'):
         r.redflag.is_ordered()
 
 
 def test_warnings():
     with pytest.warns(UserWarning, match="The Series does not seem categorical."):
         r.redflag.minority_classes()
     with pytest.warns(UserWarning, match="The Series does not seem categorical."):
@@ -54,8 +57,8 @@
 def test_series_continuous_report():
     report_r = r.redflag.report()
     assert 'Continuous' in report_r
 
 
 def test_feature_importances_docstring():
     s = pd.DataFrame([c, r]).redflag.feature_importances.__doc__
-    assert s.strip().startswith("Measure feature importances on a task, given X and y.")
+    assert s.strip().startswith("Estimate feature importances on a supervised task, given X and y.")
```

### Comparing `redflag-0.4.2rc1/tests/test_sklearn.py` & `redflag-0.5.0rc1/tests/test_sklearn.py`

 * *Files identical despite different names*


# Comparing `tmp/altimate-datapilot-cli-0.0.8.tar.gz` & `tmp/altimate-datapilot-cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altimate-datapilot-cli-0.0.8.tar", last modified: Wed Apr  3 19:22:39 2024, max compression
+gzip compressed data, was "altimate-datapilot-cli-0.0.9.tar", last modified: Fri Apr 12 01:49:51 2024, max compression
```

## Comparing `altimate-datapilot-cli-0.0.8.tar` & `altimate-datapilot-cli-0.0.9.tar`

### file list

```diff
@@ -1,249 +1,254 @@
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.952925 altimate-datapilot-cli-0.0.8/
--rw-r--r--   0 anandgupta   (501) staff       (20)      420 2024-04-02 00:54:06.000000 altimate-datapilot-cli-0.0.8/.bumpversion.cfg
--rw-r--r--   0 anandgupta   (501) staff       (20)     1992 2024-04-03 19:21:49.000000 altimate-datapilot-cli-0.0.8/.cookiecutterrc
--rw-r--r--   0 anandgupta   (501) staff       (20)      149 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/.coveragerc
--rw-r--r--   0 anandgupta   (501) staff       (20)      353 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/.editorconfig
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.918909 altimate-datapilot-cli-0.0.8/.github/
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.924560 altimate-datapilot-cli-0.0.8/.github/workflows/
--rw-r--r--   0 anandgupta   (501) staff       (20)    10794 2024-01-25 04:30:47.000000 altimate-datapilot-cli-0.0.8/.github/workflows/github-actions.yml
--rw-r--r--   0 anandgupta   (501) staff       (20)      688 2024-01-30 03:12:39.000000 altimate-datapilot-cli-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 anandgupta   (501) staff       (20)      204 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/.pre-commit-hooks.yaml
--rw-r--r--   0 anandgupta   (501) staff       (20)      282 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/.readthedocs.yml
--rw-r--r--   0 anandgupta   (501) staff       (20)       50 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/AUTHORS.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)       86 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/CHANGELOG.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     2332 2024-01-25 04:45:20.000000 altimate-datapilot-cli-0.0.8/CONTRIBUTING.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     1100 2024-01-25 04:37:04.000000 altimate-datapilot-cli-0.0.8/LICENSE
--rw-r--r--   0 anandgupta   (501) staff       (20)      495 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/MANIFEST.in
--rw-r--r--   0 anandgupta   (501) staff       (20)     2167 2024-04-03 19:22:39.952778 altimate-datapilot-cli-0.0.8/PKG-INFO
--rw-r--r--   0 anandgupta   (501) staff       (20)    11535 2024-04-03 19:22:11.000000 altimate-datapilot-cli-0.0.8/README.md
--rw-r--r--   0 anandgupta   (501) staff       (20)     1579 2024-04-03 19:22:16.000000 altimate-datapilot-cli-0.0.8/README.rst
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.924845 altimate-datapilot-cli-0.0.8/ci/
--rwxr-xr-x   0 anandgupta   (501) staff       (20)     2867 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/ci/bootstrap.py
--rw-r--r--   0 anandgupta   (501) staff       (20)       72 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/ci/requirements.txt
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.919085 altimate-datapilot-cli-0.0.8/ci/templates/
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.919129 altimate-datapilot-cli-0.0.8/ci/templates/.github/
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.924977 altimate-datapilot-cli-0.0.8/ci/templates/.github/workflows/
--rw-r--r--   0 anandgupta   (501) staff       (20)     1965 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.926941 altimate-datapilot-cli-0.0.8/docs/
--rw-r--r--   0 anandgupta   (501) staff       (20)       28 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/docs/authors.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)       30 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/docs/changelog.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     1099 2024-04-02 00:54:06.000000 altimate-datapilot-cli-0.0.8/docs/conf.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2433 2024-01-31 00:25:08.000000 altimate-datapilot-cli-0.0.8/docs/configuration.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)       33 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/docs/contributing.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     1776 2024-03-09 02:10:20.000000 altimate-datapilot-cli-0.0.8/docs/features.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     1635 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/docs/hooks.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)      221 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/docs/index.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)    35144 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/docs/insights.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     1088 2024-04-03 19:22:27.000000 altimate-datapilot-cli-0.0.8/docs/installation.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     2361 2024-01-31 00:25:08.000000 altimate-datapilot-cli-0.0.8/docs/introduction.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     1926 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/docs/performance.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)       27 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/docs/readme.rst
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.927164 altimate-datapilot-cli-0.0.8/docs/reference/
--rw-r--r--   0 anandgupta   (501) staff       (20)      106 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/docs/reference/datapilot.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)       61 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/docs/reference/index.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)       29 2024-01-31 00:25:08.000000 altimate-datapilot-cli-0.0.8/docs/requirements.txt
--rw-r--r--   0 anandgupta   (501) staff       (20)      109 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/docs/spelling_wordlist.txt
--rw-r--r--   0 anandgupta   (501) staff       (20)       70 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/docs/usage.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     1194 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/pyproject.toml
--rw-r--r--   0 anandgupta   (501) staff       (20)      903 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/pytest.ini
--rw-r--r--   0 anandgupta   (501) staff       (20)       38 2024-04-03 19:22:39.952970 altimate-datapilot-cli-0.0.8/setup.cfg
--rwxr-xr-x   0 anandgupta   (501) staff       (20)     3047 2024-04-03 19:22:22.000000 altimate-datapilot-cli-0.0.8/setup.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.919419 altimate-datapilot-cli-0.0.8/src/
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.928100 altimate-datapilot-cli-0.0.8/src/altimate_datapilot_cli.egg-info/
--rw-r--r--   0 anandgupta   (501) staff       (20)     2167 2024-04-03 19:22:39.000000 altimate-datapilot-cli-0.0.8/src/altimate_datapilot_cli.egg-info/PKG-INFO
--rw-r--r--   0 anandgupta   (501) staff       (20)     9745 2024-04-03 19:22:39.000000 altimate-datapilot-cli-0.0.8/src/altimate_datapilot_cli.egg-info/SOURCES.txt
--rw-r--r--   0 anandgupta   (501) staff       (20)        1 2024-04-03 19:22:39.000000 altimate-datapilot-cli-0.0.8/src/altimate_datapilot_cli.egg-info/dependency_links.txt
--rw-r--r--   0 anandgupta   (501) staff       (20)      141 2024-04-03 19:22:39.000000 altimate-datapilot-cli-0.0.8/src/altimate_datapilot_cli.egg-info/entry_points.txt
--rw-r--r--   0 anandgupta   (501) staff       (20)        1 2024-04-03 19:22:38.000000 altimate-datapilot-cli-0.0.8/src/altimate_datapilot_cli.egg-info/not-zip-safe
--rw-r--r--   0 anandgupta   (501) staff       (20)      110 2024-04-03 19:22:39.000000 altimate-datapilot-cli-0.0.8/src/altimate_datapilot_cli.egg-info/requires.txt
--rw-r--r--   0 anandgupta   (501) staff       (20)       10 2024-04-03 19:22:39.000000 altimate-datapilot-cli-0.0.8/src/altimate_datapilot_cli.egg-info/top_level.txt
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.928338 altimate-datapilot-cli-0.0.8/src/datapilot/
--rw-r--r--   0 anandgupta   (501) staff       (20)       22 2024-04-02 00:54:06.000000 altimate-datapilot-cli-0.0.8/src/datapilot/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      380 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/__main__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.928550 altimate-datapilot-cli-0.0.8/src/datapilot/cli/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/cli/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      181 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/cli/main.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.928662 altimate-datapilot-cli-0.0.8/src/datapilot/clients/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-02-14 00:53:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/clients/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.928948 altimate-datapilot-cli-0.0.8/src/datapilot/clients/altimate/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-02-14 00:53:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/clients/altimate/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3107 2024-02-14 00:53:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/clients/altimate/client.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2629 2024-02-14 00:53:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/clients/altimate/utils.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.929275 altimate-datapilot-cli-0.0.8/src/datapilot/config/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/config/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      403 2024-02-14 00:53:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/config/config.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1146 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/config/utils.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.929391 altimate-datapilot-cli-0.0.8/src/datapilot/core/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.929856 altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/
--rw-r--r--   0 anandgupta   (501) staff       (20)       18 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.930070 altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/base/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/base/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      883 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/base/insight.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      596 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/report.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      413 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/schema.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.930191 altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/sql/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/sql/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.930400 altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/sql/base/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/sql/base/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      471 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/sql/base/insight.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.930534 altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/sql/runtime/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/sql/runtime/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.930642 altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/sql/static/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/sql/static/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      535 2024-02-14 00:53:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/utils.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.930749 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.931639 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.931931 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/cli/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/cli/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4146 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/cli/cli.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      502 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/constants.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      110 2024-03-09 02:10:20.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/exceptions.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     6562 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/executor.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1095 2024-01-30 03:15:47.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/factory.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1638 2024-01-30 03:15:47.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/formatting.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.932171 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/hooks/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/hooks/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2966 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/hooks/executor_hook.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.932681 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/
--rw-r--r--   0 anandgupta   (501) staff       (20)     7547 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5260 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/base.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.937059 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      824 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/base.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4609 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_column_desc_are_same.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     7222 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_column_name_contract.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3185 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_macro_args_have_desc.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2802 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_macro_has_desc.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4277 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_all_columns.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5183 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_labels_keys.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5016 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_meta_keys.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2968 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_properties_file.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5706 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_group.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5187 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_name.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5590 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_type.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     6098 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_materialization_by_childs.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     6037 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_name_contract.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     6319 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_and_childs.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4665 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_database.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4658 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_schema.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3555 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_tags.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4254 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_childs.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4453 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_columns_have_desc.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4650 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_all_columns.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4111 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_freshness.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5256 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_labels_keys.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2772 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_loader.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5246 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_meta_keys.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3711 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5550 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_group.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5159 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_name.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5566 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_type.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2852 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_table_has_description.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3117 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_tags.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.937477 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/dbt_test/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/dbt_test/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      739 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/dbt_test/base.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5672 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/dbt_test/missing_primary_key_tests.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5216 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/dbt_test/test_coverage.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.938576 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 03:15:47.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      743 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/base.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5718 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/documentation_on_stale_columns.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4306 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/exposures_dependent_on_private_models.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4100 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/public_models_without_contracts.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     6394 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/undocumented_columns.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5092 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/undocumented_public_models.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.940699 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/
--rw-r--r--   0 anandgupta   (501) staff       (20)      419 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/README.md
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 03:15:47.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1009 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/base.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     6585 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/direct_join_to_source.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5790 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/downstream_models_dependent_on_source.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3937 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/duplicate_sources.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3671 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/hard_coded_references.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3937 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/joining_of_upstream_concepts.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5223 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/model_fanout.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3753 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/multiple_sources_joined.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3993 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/root_model.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4550 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/source_fanout.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4976 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/staging_model_dependent_on_downstream_models.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4261 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/staging_model_dependent_on_staging_models.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2780 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/unused_sources.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.941475 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/performance/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/performance/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      829 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/performance/base.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3627 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/performance/chain_view_linking.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4689 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/performance/exposure_parent_materializations.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2657 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/schema.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.942398 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1101 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/base.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4382 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/model_directories_structure.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4999 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/model_naming_conventions.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3675 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/source_directories_structure.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3484 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/test_directory_structure.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      267 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/utils.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.942764 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/schemas/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/schemas/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1878 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/schemas/catalog.py
--rw-r--r--   0 anandgupta   (501) staff       (20)    14117 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/schemas/manifest.py
--rw-r--r--   0 anandgupta   (501) staff       (20)    18577 2024-03-09 02:10:20.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/utils.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.942926 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.943112 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/catalog/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/catalog/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.943344 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/catalog/v1/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/catalog/v1/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      832 2024-01-30 03:15:47.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/catalog/v1/wrapper.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      196 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/catalog/wrapper.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.943614 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.943984 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1523 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/schemas.py
--rw-r--r--   0 anandgupta   (501) staff       (20)    17274 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/wrapper.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1078 2024-01-30 03:15:47.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/wrapper.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.944254 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/run_results/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/run_results/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1267 2024-01-30 03:15:47.000000 altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/run_results/run_results.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.944473 altimate-datapilot-cli-0.0.8/src/datapilot/exceptions/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/exceptions/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      162 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/exceptions/exceptions.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.944941 altimate-datapilot-cli-0.0.8/src/datapilot/schemas/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/schemas/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      190 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/schemas/constants.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      319 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/schemas/nodes.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      193 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/schemas/sql.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.945183 altimate-datapilot-cli-0.0.8/src/datapilot/utils/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/utils/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.945467 altimate-datapilot-cli-0.0.8/src/datapilot/utils/formatting/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/utils/formatting/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1377 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/src/datapilot/utils/formatting/utils.py
--rw-r--r--   0 anandgupta   (501) staff       (20)    11150 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.8/src/datapilot/utils/utils.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.921947 altimate-datapilot-cli-0.0.8/tests/
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.945579 altimate-datapilot-cli-0.0.8/tests/core/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/tests/core/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.945665 altimate-datapilot-cli-0.0.8/tests/core/platform/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/tests/core/platform/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.945947 altimate-datapilot-cli-0.0.8/tests/core/platform/dbt/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/tests/core/platform/dbt/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1298 2024-02-14 00:53:49.000000 altimate-datapilot-cli-0.0.8/tests/core/platform/dbt/test_cli.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5717 2024-01-30 03:15:47.000000 altimate-datapilot-cli-0.0.8/tests/core/platform/dbt/test_utils.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.946420 altimate-datapilot-cli-0.0.8/tests/data/
--rw-r--r--   0 anandgupta   (501) staff       (20)   181355 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.8/tests/data/catalog_v1.json
--rw-r--r--   0 anandgupta   (501) staff       (20)      397 2024-01-30 02:44:52.000000 altimate-datapilot-cli-0.0.8/tests/data/config.yml
--rw-r--r--   0 anandgupta   (501) staff       (20)  2187651 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.8/tests/data/manifest_v11.json
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.949714 altimate-datapilot-cli-0.0.8/tests/data/manifests/
--rw-r--r--   0 anandgupta   (501) staff       (20)   440290 2024-01-30 22:07:56.000000 altimate-datapilot-cli-0.0.8/tests/data/manifests/manifest_js.json
--rw-r--r--   0 anandgupta   (501) staff       (20)   496433 2024-01-30 22:07:56.000000 altimate-datapilot-cli-0.0.8/tests/data/manifests/manifest_js2.json
--rw-r--r--   0 anandgupta   (501) staff       (20)   451985 2024-01-30 22:07:56.000000 altimate-datapilot-cli-0.0.8/tests/data/manifests/manifest_js3.json
--rw-r--r--   0 anandgupta   (501) staff       (20)   451995 2024-01-30 22:07:56.000000 altimate-datapilot-cli-0.0.8/tests/data/manifests/manifest_tuva.json
--rw-r--r--   0 anandgupta   (501) staff       (20)   511945 2024-01-30 22:07:56.000000 altimate-datapilot-cli-0.0.8/tests/data/manifests/manifest_tuva2.json
--rw-r--r--   0 anandgupta   (501) staff       (20)  3176176 2024-01-30 22:07:56.000000 altimate-datapilot-cli-0.0.8/tests/data/manifests/manifest_tuva3.json
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-03 19:22:39.952560 altimate-datapilot-cli-0.0.8/tests/utils/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.8/tests/utils/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2491 2024-03-09 02:10:20.000000 altimate-datapilot-cli-0.0.8/tests/utils/test_utils.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1764 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.8/tox.ini
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.082237 altimate-datapilot-cli-0.0.9/
+-rw-r--r--   0 anandgupta   (501) staff       (20)      420 2024-04-12 01:49:43.000000 altimate-datapilot-cli-0.0.9/.bumpversion.cfg
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1992 2024-04-03 19:43:26.000000 altimate-datapilot-cli-0.0.9/.cookiecutterrc
+-rw-r--r--   0 anandgupta   (501) staff       (20)      149 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/.coveragerc
+-rw-r--r--   0 anandgupta   (501) staff       (20)      353 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/.editorconfig
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.047623 altimate-datapilot-cli-0.0.9/.github/
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.052904 altimate-datapilot-cli-0.0.9/.github/workflows/
+-rw-r--r--   0 anandgupta   (501) staff       (20)    10794 2024-01-25 04:30:47.000000 altimate-datapilot-cli-0.0.9/.github/workflows/github-actions.yml
+-rw-r--r--   0 anandgupta   (501) staff       (20)      688 2024-01-30 03:12:39.000000 altimate-datapilot-cli-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 anandgupta   (501) staff       (20)      204 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/.pre-commit-hooks.yaml
+-rw-r--r--   0 anandgupta   (501) staff       (20)      282 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/.readthedocs.yml
+-rw-r--r--   0 anandgupta   (501) staff       (20)       50 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/AUTHORS.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)       86 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/CHANGELOG.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2336 2024-04-03 19:43:26.000000 altimate-datapilot-cli-0.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1100 2024-01-25 04:37:04.000000 altimate-datapilot-cli-0.0.9/LICENSE
+-rw-r--r--   0 anandgupta   (501) staff       (20)      495 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/MANIFEST.in
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2180 2024-04-12 01:49:51.082099 altimate-datapilot-cli-0.0.9/PKG-INFO
+-rw-r--r--   0 anandgupta   (501) staff       (20)    11535 2024-04-03 19:43:26.000000 altimate-datapilot-cli-0.0.9/README.md
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1587 2024-04-03 19:43:26.000000 altimate-datapilot-cli-0.0.9/README.rst
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.053147 altimate-datapilot-cli-0.0.9/ci/
+-rwxr-xr-x   0 anandgupta   (501) staff       (20)     2867 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/ci/bootstrap.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)       72 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/ci/requirements.txt
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.047799 altimate-datapilot-cli-0.0.9/ci/templates/
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.047844 altimate-datapilot-cli-0.0.9/ci/templates/.github/
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.053269 altimate-datapilot-cli-0.0.9/ci/templates/.github/workflows/
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1965 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.055027 altimate-datapilot-cli-0.0.9/docs/
+-rw-r--r--   0 anandgupta   (501) staff       (20)       28 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/docs/authors.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)       30 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/docs/changelog.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1117 2024-04-12 01:49:43.000000 altimate-datapilot-cli-0.0.9/docs/conf.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2433 2024-01-31 00:25:08.000000 altimate-datapilot-cli-0.0.9/docs/configuration.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)       33 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/docs/contributing.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1841 2024-04-12 01:49:40.000000 altimate-datapilot-cli-0.0.9/docs/features.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1643 2024-04-03 19:43:26.000000 altimate-datapilot-cli-0.0.9/docs/hooks.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)      221 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/docs/index.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)    35144 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/docs/insights.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1088 2024-04-03 19:43:26.000000 altimate-datapilot-cli-0.0.9/docs/installation.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2361 2024-01-31 00:25:08.000000 altimate-datapilot-cli-0.0.9/docs/introduction.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1926 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/docs/performance.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)       27 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/docs/readme.rst
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.055243 altimate-datapilot-cli-0.0.9/docs/reference/
+-rw-r--r--   0 anandgupta   (501) staff       (20)      106 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/docs/reference/datapilot.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)       61 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/docs/reference/index.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)       29 2024-01-31 00:25:08.000000 altimate-datapilot-cli-0.0.9/docs/requirements.txt
+-rw-r--r--   0 anandgupta   (501) staff       (20)      109 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/docs/spelling_wordlist.txt
+-rw-r--r--   0 anandgupta   (501) staff       (20)       70 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/docs/usage.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1194 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/pyproject.toml
+-rw-r--r--   0 anandgupta   (501) staff       (20)      903 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/pytest.ini
+-rw-r--r--   0 anandgupta   (501) staff       (20)       38 2024-04-12 01:49:51.082291 altimate-datapilot-cli-0.0.9/setup.cfg
+-rwxr-xr-x   0 anandgupta   (501) staff       (20)     3056 2024-04-12 01:49:43.000000 altimate-datapilot-cli-0.0.9/setup.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.048132 altimate-datapilot-cli-0.0.9/src/
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.058127 altimate-datapilot-cli-0.0.9/src/altimate_datapilot_cli.egg-info/
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2180 2024-04-12 01:49:51.000000 altimate-datapilot-cli-0.0.9/src/altimate_datapilot_cli.egg-info/PKG-INFO
+-rw-r--r--   0 anandgupta   (501) staff       (20)     9973 2024-04-12 01:49:51.000000 altimate-datapilot-cli-0.0.9/src/altimate_datapilot_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 anandgupta   (501) staff       (20)        1 2024-04-12 01:49:51.000000 altimate-datapilot-cli-0.0.9/src/altimate_datapilot_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 anandgupta   (501) staff       (20)      141 2024-04-12 01:49:51.000000 altimate-datapilot-cli-0.0.9/src/altimate_datapilot_cli.egg-info/entry_points.txt
+-rw-r--r--   0 anandgupta   (501) staff       (20)        1 2024-04-12 01:49:49.000000 altimate-datapilot-cli-0.0.9/src/altimate_datapilot_cli.egg-info/not-zip-safe
+-rw-r--r--   0 anandgupta   (501) staff       (20)      110 2024-04-12 01:49:51.000000 altimate-datapilot-cli-0.0.9/src/altimate_datapilot_cli.egg-info/requires.txt
+-rw-r--r--   0 anandgupta   (501) staff       (20)       10 2024-04-12 01:49:51.000000 altimate-datapilot-cli-0.0.9/src/altimate_datapilot_cli.egg-info/top_level.txt
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.058395 altimate-datapilot-cli-0.0.9/src/datapilot/
+-rw-r--r--   0 anandgupta   (501) staff       (20)       22 2024-04-12 01:49:43.000000 altimate-datapilot-cli-0.0.9/src/datapilot/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      380 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/__main__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.058606 altimate-datapilot-cli-0.0.9/src/datapilot/cli/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/cli/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      181 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/cli/main.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.058730 altimate-datapilot-cli-0.0.9/src/datapilot/clients/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-02-14 00:53:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/clients/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.059049 altimate-datapilot-cli-0.0.9/src/datapilot/clients/altimate/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-02-14 00:53:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/clients/altimate/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3107 2024-02-14 00:53:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/clients/altimate/client.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2629 2024-02-14 00:53:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/clients/altimate/utils.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.059394 altimate-datapilot-cli-0.0.9/src/datapilot/config/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/config/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      403 2024-02-14 00:53:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/config/config.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1146 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/config/utils.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.059505 altimate-datapilot-cli-0.0.9/src/datapilot/core/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.059957 altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/
+-rw-r--r--   0 anandgupta   (501) staff       (20)       18 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.060164 altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/base/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/base/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      883 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/base/insight.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      596 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/report.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      413 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/schema.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.060273 altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/sql/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/sql/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.060463 altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/sql/base/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/sql/base/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      471 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/sql/base/insight.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.060580 altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/sql/runtime/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/sql/runtime/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.060675 altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/sql/static/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/sql/static/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      535 2024-02-14 00:53:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/utils.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.060761 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.061608 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.061899 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/cli/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/cli/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4146 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/cli/cli.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      502 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/constants.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      110 2024-03-09 02:10:20.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/exceptions.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     6562 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/executor.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1331 2024-04-12 01:49:40.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/factory.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1638 2024-01-30 03:15:47.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/formatting.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.062121 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/hooks/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/hooks/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2966 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/hooks/executor_hook.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.062616 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/
+-rw-r--r--   0 anandgupta   (501) staff       (20)     7547 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5260 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/base.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.066768 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      824 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/base.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4609 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_column_desc_are_same.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     7222 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_column_name_contract.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3185 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_macro_args_have_desc.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2802 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_macro_has_desc.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4277 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_all_columns.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5183 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_labels_keys.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5016 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_meta_keys.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2968 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_properties_file.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5706 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_group.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5187 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_name.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5590 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_type.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     6098 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_materialization_by_childs.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     6037 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_name_contract.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     6319 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_and_childs.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4665 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_database.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4658 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_schema.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3555 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_tags.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4254 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_childs.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4453 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_columns_have_desc.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4650 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_all_columns.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4111 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_freshness.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5256 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_labels_keys.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2772 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_loader.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5246 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_meta_keys.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3711 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5550 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_group.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5159 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_name.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5566 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_type.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2852 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_table_has_description.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3117 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_tags.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.067240 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/dbt_test/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/dbt_test/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      739 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/dbt_test/base.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5672 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/dbt_test/missing_primary_key_tests.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5216 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/dbt_test/test_coverage.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.068097 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/governance/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 03:15:47.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/governance/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      743 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/governance/base.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5718 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/governance/documentation_on_stale_columns.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4306 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/governance/exposures_dependent_on_private_models.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4100 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/governance/public_models_without_contracts.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     6394 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/governance/undocumented_columns.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5092 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/governance/undocumented_public_models.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.069851 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/
+-rw-r--r--   0 anandgupta   (501) staff       (20)      419 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/README.md
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 03:15:47.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1009 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/base.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     6585 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/direct_join_to_source.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5790 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/downstream_models_dependent_on_source.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3937 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/duplicate_sources.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3671 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/hard_coded_references.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3937 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/joining_of_upstream_concepts.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5223 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/model_fanout.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3753 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/multiple_sources_joined.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3993 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/root_model.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4550 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/source_fanout.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4976 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/staging_model_dependent_on_downstream_models.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4261 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/staging_model_dependent_on_staging_models.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2780 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/unused_sources.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.070269 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/performance/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/performance/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      829 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/performance/base.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3627 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/performance/chain_view_linking.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4689 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/performance/exposure_parent_materializations.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2657 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/schema.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.070961 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/structure/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/structure/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1101 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/structure/base.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4382 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/structure/model_directories_structure.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4999 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/structure/model_naming_conventions.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3675 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/structure/source_directories_structure.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3484 2024-04-02 00:54:00.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/structure/test_directory_structure.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      267 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/utils.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.071264 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/schemas/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/schemas/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1878 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/schemas/catalog.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)    14117 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/schemas/manifest.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)    18577 2024-03-09 02:10:20.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/utils.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.071444 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.071621 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/catalog/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/catalog/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.071827 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/catalog/v1/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/catalog/v1/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      832 2024-01-30 03:15:47.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/catalog/v1/wrapper.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      196 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/catalog/wrapper.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.072058 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/manifest/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/manifest/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.072384 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/manifest/v10/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:40.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/manifest/v10/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1523 2024-04-12 01:49:40.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/manifest/v10/schemas.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)    17274 2024-04-12 01:49:40.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/manifest/v10/wrapper.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.072724 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1523 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/schemas.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)    17274 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/wrapper.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1078 2024-01-30 03:15:47.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/manifest/wrapper.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.072951 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/run_results/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/run_results/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1267 2024-01-30 03:15:47.000000 altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/run_results/run_results.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.073150 altimate-datapilot-cli-0.0.9/src/datapilot/exceptions/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/exceptions/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      162 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/exceptions/exceptions.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.073577 altimate-datapilot-cli-0.0.9/src/datapilot/schemas/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/schemas/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      190 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/schemas/constants.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      319 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/schemas/nodes.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      193 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/schemas/sql.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.073813 altimate-datapilot-cli-0.0.9/src/datapilot/utils/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/utils/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.074059 altimate-datapilot-cli-0.0.9/src/datapilot/utils/formatting/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/utils/formatting/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1377 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/src/datapilot/utils/formatting/utils.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)    11150 2024-03-29 16:47:02.000000 altimate-datapilot-cli-0.0.9/src/datapilot/utils/utils.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.050766 altimate-datapilot-cli-0.0.9/tests/
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.074188 altimate-datapilot-cli-0.0.9/tests/core/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/tests/core/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.074289 altimate-datapilot-cli-0.0.9/tests/core/platform/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/tests/core/platform/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.074622 altimate-datapilot-cli-0.0.9/tests/core/platform/dbt/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/tests/core/platform/dbt/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1828 2024-04-12 01:49:40.000000 altimate-datapilot-cli-0.0.9/tests/core/platform/dbt/test_cli.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5717 2024-01-30 03:15:47.000000 altimate-datapilot-cli-0.0.9/tests/core/platform/dbt/test_utils.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.075556 altimate-datapilot-cli-0.0.9/tests/data/
+-rw-r--r--   0 anandgupta   (501) staff       (20)   181355 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.9/tests/data/catalog_v1.json
+-rw-r--r--   0 anandgupta   (501) staff       (20)      397 2024-01-30 02:44:52.000000 altimate-datapilot-cli-0.0.9/tests/data/config.yml
+-rw-r--r--   0 anandgupta   (501) staff       (20)   474415 2024-04-12 01:49:40.000000 altimate-datapilot-cli-0.0.9/tests/data/manifest_v10.json
+-rw-r--r--   0 anandgupta   (501) staff       (20)  2187651 2024-01-30 04:41:49.000000 altimate-datapilot-cli-0.0.9/tests/data/manifest_v11.json
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.080249 altimate-datapilot-cli-0.0.9/tests/data/manifests/
+-rw-r--r--   0 anandgupta   (501) staff       (20)   440290 2024-01-30 22:07:56.000000 altimate-datapilot-cli-0.0.9/tests/data/manifests/manifest_js.json
+-rw-r--r--   0 anandgupta   (501) staff       (20)   496433 2024-01-30 22:07:56.000000 altimate-datapilot-cli-0.0.9/tests/data/manifests/manifest_js2.json
+-rw-r--r--   0 anandgupta   (501) staff       (20)   451985 2024-01-30 22:07:56.000000 altimate-datapilot-cli-0.0.9/tests/data/manifests/manifest_js3.json
+-rw-r--r--   0 anandgupta   (501) staff       (20)   451995 2024-01-30 22:07:56.000000 altimate-datapilot-cli-0.0.9/tests/data/manifests/manifest_tuva.json
+-rw-r--r--   0 anandgupta   (501) staff       (20)   511945 2024-01-30 22:07:56.000000 altimate-datapilot-cli-0.0.9/tests/data/manifests/manifest_tuva2.json
+-rw-r--r--   0 anandgupta   (501) staff       (20)  3176176 2024-01-30 22:07:56.000000 altimate-datapilot-cli-0.0.9/tests/data/manifests/manifest_tuva3.json
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-12 01:49:51.081903 altimate-datapilot-cli-0.0.9/tests/utils/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-cli-0.0.9/tests/utils/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2491 2024-03-09 02:10:20.000000 altimate-datapilot-cli-0.0.9/tests/utils/test_utils.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1764 2024-01-25 04:30:38.000000 altimate-datapilot-cli-0.0.9/tox.ini
```

### Comparing `altimate-datapilot-cli-0.0.8/.cookiecutterrc` & `altimate-datapilot-cli-0.0.9/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/.github/workflows/github-actions.yml` & `altimate-datapilot-cli-0.0.9/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/.pre-commit-config.yaml` & `altimate-datapilot-cli-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/CONTRIBUTING.rst` & `altimate-datapilot-cli-0.0.9/CONTRIBUTING.rst`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 * Remember that this is a volunteer-driven project, and that code contributions are welcome :)
 
 Development
 ===========
 
 To set up `datapilot` for local development:
 
-1. Fork `datapilot <https://github.com/AltimateAI/datapilot>`_
+1. Fork `datapilot <https://github.com/AltimateAI/datapilot-cli>`_
    (look for the "Fork" button).
 2. Clone your fork locally::
 
     git clone git@github.com:YOURGITHUBNAME/datapilot.git
 
 3. Create a branch for local development::
```

### Comparing `altimate-datapilot-cli-0.0.8/LICENSE` & `altimate-datapilot-cli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/PKG-INFO` & `altimate-datapilot-cli-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: altimate-datapilot-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: Assistant for Data Teams
-Home-page: https://github.com/AltimateAI/datapilot
-Author: Anand Gupta
+Home-page: https://github.com/AltimateAI/datapilot-cli
+Author: Altimate Inc
 Author-email: info@altimate.ai
 License: MIT
 Project-URL: Documentation, https://datapilot.readthedocs.io/
 Project-URL: Changelog, https://datapilot.readthedocs.io/en/latest/changelog.html
-Project-URL: Issue Tracker, https://github.com/AltimateAI/datapilot/issues
+Project-URL: Issue Tracker, https://github.com/AltimateAI/datapilot-cli/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
@@ -46,15 +46,15 @@
 
 ::
 
     pip install altimate-datapilot-cli
 
 You can also install the in-development version with::
 
-    pip install https://github.com/AltimateAI/datapilot/archive/main.zip
+    pip install https://github.com/AltimateAI/datapilot-cli/archive/main.zip
 
 
 Documentation
 =============
 
 
 https://datapilot.readthedocs.io/
```

### Comparing `altimate-datapilot-cli-0.0.8/README.md` & `altimate-datapilot-cli-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/README.rst` & `altimate-datapilot-cli-0.0.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     * - package
       - | |version| |wheel| |supported-versions| |supported-implementations|
         | |commits-since|
 .. |docs| image:: https://readthedocs.org/projects/datapilot/badge/?style=flat
     :target: https://datapilot.readthedocs.io/
     :alt: Documentation Status
 
-.. |github-actions| image:: https://github.com/AltimateAI/datapilot/actions/workflows/github-actions.yml/badge.svg
+.. |github-actions| image:: https://github.com/AltimateAI/datapilot-cli/actions/workflows/github-actions.yml/badge.svg
     :alt: GitHub Actions Build Status
     :target: https://github.com/AltimateAI/datapilot/actions
 
 .. |codecov| image:: https://codecov.io/gh/anandgupta42/datapilot/branch/main/graphs/badge.svg?branch=main
     :alt: Coverage Status
     :target: https://app.codecov.io/github/anandgupta42/datapilot
 
@@ -42,15 +42,15 @@
 
 ::
 
     pip install altimate-datapilot-cli
 
 You can also install the in-development version with::
 
-    pip install https://github.com/AltimateAI/datapilot/archive/main.zip
+    pip install https://github.com/AltimateAI/datapilot-cli/archive/main.zip
 
 
 Documentation
 =============
 
 
 https://datapilot.readthedocs.io/
```

### Comparing `altimate-datapilot-cli-0.0.8/ci/bootstrap.py` & `altimate-datapilot-cli-0.0.9/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/ci/templates/.github/workflows/github-actions.yml` & `altimate-datapilot-cli-0.0.9/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/docs/conf.py` & `altimate-datapilot-cli-0.0.9/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     "sphinx.ext.ifconfig",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
     "sphinx.ext.viewcode",
 ]
 source_suffix = ".rst"
 master_doc = "index"
-project = "datapilot"
+project = "datapilot-cli"
 year = "2024"
-author = "Anand Gupta"
+author = "Altimate Inc."
 copyright = f"{year}, {author}"
-version = release = "0.0.8"
+version = release = "0.0.9"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
-    "issue": ("https://github.com/AltimateAI/datapilot/issues/%s", "#"),
-    "pr": ("https://github.com/AltimateAI/datapilot/pull/%s", "PR #"),
+    "issue": ("https://github.com/AltimateAI/datapilot-cli/issues/%s", "#"),
+    "pr": ("https://github.com/AltimateAI/datapilot-cli/pull/%s", "PR #"),
 }
 html_theme = "sphinx_rtd_theme"
 # html_theme_path = [furo.get_html_theme_path()]
 # html_theme_options = {
-#     "githuburl": "https://github.com/AltimateAI/datapilot/",
+#     "githuburl": "https://github.com/AltimateAI/datapilot-cli/",
 # }
 
 html_use_smartypants = True
 html_last_updated_fmt = "%b %d, %Y"
 html_split_index = False
 html_sidebars = {
     "**": ["searchbox.html", "globaltoc.html", "sourcelink.html"],
```

### Comparing `altimate-datapilot-cli-0.0.8/docs/configuration.rst` & `altimate-datapilot-cli-0.0.9/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/docs/features.rst` & `altimate-datapilot-cli-0.0.9/docs/features.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 dbt
 ===
 
 project-health
 --------------
 
-The ``project-health`` feature in DataPilot is a comprehensive tool designed to analyze and report on various aspects of your dbt project.
+The ``project-health`` feature in DataPilot is a comprehensive tool designed to analyze and report on various aspects of your dbt project. This feature is currently supported for dbt version 1.6 and 1.7.
 
 How to Use
 ^^^^^^^^^^
 
 To use the ``project-health`` feature, run the following command in your dbt project directory:
 
 Step 1: Generate a manifest file for your dbt project.
```

### Comparing `altimate-datapilot-cli-0.0.8/docs/hooks.rst` & `altimate-datapilot-cli-0.0.9/docs/hooks.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 pip install pre-commit
 ```
 
 2. Add the following configuration to your .pre-commit-config.yaml file in the root of your repository:
 
 ```
     repos:
-  - repo: https://github.com/AltimateAI/datapilot
+  - repo: https://github.com/AltimateAI/datapilot-cli
     rev: <revision>
     hooks:
       - id: datapilot_run_dbt_checks
         args: ["--config-path", "path/to/your/config/file"]
 ```
 
 Replace <revision> with the desired revision of the DataPilot repository and "path/to/your/config/file" with the path to your configuration file.
@@ -42,10 +42,10 @@
 
 If you want to manually run all pre-commit hooks on a repository, run `pre-commit run --all-files`. To run individual hooks use `pre-commit run <hook_id>`.
 
 
 Feedback and Contributions
 --------------------------
 
-If you encounter any issues or have suggestions for improvements, please feel free to open an issue or pull request on the DataPilot GitHub repository at https://github.com/AltimateAI/datapilot.
+If you encounter any issues or have suggestions for improvements, please feel free to open an issue or pull request on the DataPilot GitHub repository at https://github.com/AltimateAI/datapilot-cli.
 
 Thank you for using DataPilot!
```

### Comparing `altimate-datapilot-cli-0.0.8/docs/insights.rst` & `altimate-datapilot-cli-0.0.9/docs/insights.rst`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/docs/installation.rst` & `altimate-datapilot-cli-0.0.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/docs/introduction.rst` & `altimate-datapilot-cli-0.0.9/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/docs/performance.rst` & `altimate-datapilot-cli-0.0.9/docs/performance.rst`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/pyproject.toml` & `altimate-datapilot-cli-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/pytest.ini` & `altimate-datapilot-cli-0.0.9/pytest.ini`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/setup.py` & `altimate-datapilot-cli-0.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="altimate-datapilot-cli",
-    version="0.0.8",
+    version="0.0.9",
     license="MIT",
     description="Assistant for Data Teams",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
-    author="Anand Gupta",
+    author="Altimate Inc",
     author_email="info@altimate.ai",
-    url="https://github.com/AltimateAI/datapilot",
+    url="https://github.com/AltimateAI/datapilot-cli",
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=[path.stem for path in Path("src").glob("*.py")],
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
@@ -51,15 +51,15 @@
         # "Programming Language :: Python :: Implementation :: Jython",
         # "Programming Language :: Python :: Implementation :: Stackless",
         "Topic :: Utilities",
     ],
     project_urls={
         "Documentation": "https://datapilot.readthedocs.io/",
         "Changelog": "https://datapilot.readthedocs.io/en/latest/changelog.html",
-        "Issue Tracker": "https://github.com/AltimateAI/datapilot/issues",
+        "Issue Tracker": "https://github.com/AltimateAI/datapilot-cli/issues",
     },
     keywords=[
         # eg: "keyword1", "keyword2", "keyword3",
     ],
     python_requires=">=3.8",
     install_requires=[
         "click==8.1.7",
```

### Comparing `altimate-datapilot-cli-0.0.8/src/altimate_datapilot_cli.egg-info/PKG-INFO` & `altimate-datapilot-cli-0.0.9/src/altimate_datapilot_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: altimate-datapilot-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: Assistant for Data Teams
-Home-page: https://github.com/AltimateAI/datapilot
-Author: Anand Gupta
+Home-page: https://github.com/AltimateAI/datapilot-cli
+Author: Altimate Inc
 Author-email: info@altimate.ai
 License: MIT
 Project-URL: Documentation, https://datapilot.readthedocs.io/
 Project-URL: Changelog, https://datapilot.readthedocs.io/en/latest/changelog.html
-Project-URL: Issue Tracker, https://github.com/AltimateAI/datapilot/issues
+Project-URL: Issue Tracker, https://github.com/AltimateAI/datapilot-cli/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
@@ -46,15 +46,15 @@
 
 ::
 
     pip install altimate-datapilot-cli
 
 You can also install the in-development version with::
 
-    pip install https://github.com/AltimateAI/datapilot/archive/main.zip
+    pip install https://github.com/AltimateAI/datapilot-cli/archive/main.zip
 
 
 Documentation
 =============
 
 
 https://datapilot.readthedocs.io/
```

### Comparing `altimate-datapilot-cli-0.0.8/src/altimate_datapilot_cli.egg-info/SOURCES.txt` & `altimate-datapilot-cli-0.0.9/src/altimate_datapilot_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,17 @@
 src/datapilot/core/platforms/dbt/wrappers/__init__.py
 src/datapilot/core/platforms/dbt/wrappers/catalog/__init__.py
 src/datapilot/core/platforms/dbt/wrappers/catalog/wrapper.py
 src/datapilot/core/platforms/dbt/wrappers/catalog/v1/__init__.py
 src/datapilot/core/platforms/dbt/wrappers/catalog/v1/wrapper.py
 src/datapilot/core/platforms/dbt/wrappers/manifest/__init__.py
 src/datapilot/core/platforms/dbt/wrappers/manifest/wrapper.py
+src/datapilot/core/platforms/dbt/wrappers/manifest/v10/__init__.py
+src/datapilot/core/platforms/dbt/wrappers/manifest/v10/schemas.py
+src/datapilot/core/platforms/dbt/wrappers/manifest/v10/wrapper.py
 src/datapilot/core/platforms/dbt/wrappers/manifest/v11/__init__.py
 src/datapilot/core/platforms/dbt/wrappers/manifest/v11/schemas.py
 src/datapilot/core/platforms/dbt/wrappers/manifest/v11/wrapper.py
 src/datapilot/core/platforms/dbt/wrappers/run_results/__init__.py
 src/datapilot/core/platforms/dbt/wrappers/run_results/run_results.py
 src/datapilot/exceptions/__init__.py
 src/datapilot/exceptions/exceptions.py
@@ -180,14 +183,15 @@
 tests/core/__init__.py
 tests/core/platform/__init__.py
 tests/core/platform/dbt/__init__.py
 tests/core/platform/dbt/test_cli.py
 tests/core/platform/dbt/test_utils.py
 tests/data/catalog_v1.json
 tests/data/config.yml
+tests/data/manifest_v10.json
 tests/data/manifest_v11.json
 tests/data/manifests/manifest_js.json
 tests/data/manifests/manifest_js2.json
 tests/data/manifests/manifest_js3.json
 tests/data/manifests/manifest_tuva.json
 tests/data/manifests/manifest_tuva2.json
 tests/data/manifests/manifest_tuva3.json
```

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/clients/altimate/client.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/clients/altimate/client.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/clients/altimate/utils.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/clients/altimate/utils.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/config/utils.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/config/utils.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/base/insight.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/base/insight.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/report.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/report.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/insights/utils.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/insights/utils.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/cli/cli.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/cli/cli.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/executor.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/executor.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/factory.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from dbt_artifacts_parser.parsers.catalog.catalog_v1 import CatalogV1
+from dbt_artifacts_parser.parsers.manifest.manifest_v10 import ManifestV10
 from dbt_artifacts_parser.parsers.manifest.manifest_v11 import ManifestV11
 
 from datapilot.core.platforms.dbt.schemas.manifest import Catalog
 from datapilot.core.platforms.dbt.schemas.manifest import Manifest
 from datapilot.core.platforms.dbt.wrappers.catalog.v1.wrapper import CatalogV1Wrapper
+from datapilot.core.platforms.dbt.wrappers.manifest.v10.wrapper import ManifestV10Wrapper
 from datapilot.core.platforms.dbt.wrappers.manifest.v11.wrapper import ManifestV11Wrapper
 from datapilot.exceptions.exceptions import AltimateNotSupportedError
 
 
 class DBTFactory:
     @classmethod
     def get_manifest_wrapper(cls, manifest: Manifest):
         if isinstance(manifest, ManifestV11):
             return ManifestV11Wrapper(manifest)
-        raise AltimateNotSupportedError(f"Manifest version {manifest.metadata.dbt_schema_version} not supported")
+        if isinstance(manifest, ManifestV10):
+            return ManifestV10Wrapper(manifest)
+        raise AltimateNotSupportedError(f"dbt version {manifest.metadata.dbt_version} not supported")
 
     @classmethod
     def get_catalog_wrapper(cls, catalog: Catalog):
         if isinstance(catalog, CatalogV1):
             return CatalogV1Wrapper(catalog)
-        raise AltimateNotSupportedError(f"Catalog version {catalog.metadata.dbt_schema_version} not supported")
+        raise AltimateNotSupportedError(f"dbt version {catalog.metadata.dbt_version} not supported")
```

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/formatting.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/formatting.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/hooks/executor_hook.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/hooks/executor_hook.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/__init__.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/__init__.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/base.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/base.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/base.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/base.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_column_desc_are_same.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_column_desc_are_same.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_column_name_contract.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_column_name_contract.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_macro_args_have_desc.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_macro_args_have_desc.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_macro_has_desc.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_macro_has_desc.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_all_columns.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_all_columns.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_labels_keys.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_labels_keys.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_meta_keys.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_meta_keys.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_properties_file.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_properties_file.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_group.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_group.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_name.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_name.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_type.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_type.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_materialization_by_childs.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_materialization_by_childs.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_name_contract.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_name_contract.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_and_childs.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_and_childs.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_database.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_database.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_schema.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_schema.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_tags.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_model_tags.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_childs.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_childs.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_columns_have_desc.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_columns_have_desc.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_all_columns.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_all_columns.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_freshness.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_freshness.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_labels_keys.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_labels_keys.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_loader.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_loader.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_meta_keys.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_meta_keys.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_group.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_group.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_name.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_name.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_type.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_type.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_table_has_description.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_table_has_description.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_tags.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/checks/check_source_tags.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/dbt_test/base.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/dbt_test/base.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/dbt_test/missing_primary_key_tests.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/dbt_test/missing_primary_key_tests.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/dbt_test/test_coverage.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/dbt_test/test_coverage.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/base.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/governance/base.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/documentation_on_stale_columns.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/governance/documentation_on_stale_columns.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/exposures_dependent_on_private_models.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/governance/exposures_dependent_on_private_models.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/public_models_without_contracts.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/governance/public_models_without_contracts.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/undocumented_columns.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/governance/undocumented_columns.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/undocumented_public_models.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/governance/undocumented_public_models.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/base.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/base.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/direct_join_to_source.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/direct_join_to_source.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/downstream_models_dependent_on_source.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/downstream_models_dependent_on_source.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/duplicate_sources.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/duplicate_sources.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/hard_coded_references.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/hard_coded_references.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/joining_of_upstream_concepts.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/joining_of_upstream_concepts.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/model_fanout.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/model_fanout.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/multiple_sources_joined.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/multiple_sources_joined.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/root_model.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/root_model.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/source_fanout.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/source_fanout.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/staging_model_dependent_on_downstream_models.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/staging_model_dependent_on_downstream_models.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/staging_model_dependent_on_staging_models.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/staging_model_dependent_on_staging_models.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/unused_sources.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/modelling/unused_sources.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/performance/base.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/performance/base.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/performance/chain_view_linking.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/performance/chain_view_linking.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/performance/exposure_parent_materializations.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/performance/exposure_parent_materializations.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/schema.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/schema.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/base.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/structure/base.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/model_directories_structure.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/structure/model_directories_structure.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/model_naming_conventions.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/structure/model_naming_conventions.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/source_directories_structure.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/structure/source_directories_structure.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/test_directory_structure.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/insights/structure/test_directory_structure.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/schemas/catalog.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/schemas/catalog.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/schemas/manifest.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/utils.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/utils.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/catalog/v1/wrapper.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/catalog/v1/wrapper.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/schemas.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/schemas.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/wrapper.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/wrapper.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/wrapper.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/manifest/wrapper.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/core/platforms/dbt/wrappers/run_results/run_results.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/core/platforms/dbt/wrappers/run_results/run_results.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/utils/formatting/utils.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/utils/formatting/utils.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/src/datapilot/utils/utils.py` & `altimate-datapilot-cli-0.0.9/src/datapilot/utils/utils.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/tests/core/platform/dbt/test_cli.py` & `altimate-datapilot-cli-0.0.9/tests/core/platform/dbt/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,7 +31,25 @@
             manifest_path,
         ],
     )
 
     assert result.exit_code == 0  # Ensure the command executed successfully
     # Validate behavior for when only the required argument is provided
     assert "-----------" in result.output
+
+
+def test_project_health_with_only_required_arg_version1_6():
+    runner = CliRunner()
+    manifest_path = "tests/data/manifest_v10.json"
+
+    # Simulate command invocation without optional arguments
+    result = runner.invoke(
+        project_health,
+        [
+            "--manifest-path",
+            manifest_path,
+        ],
+    )
+
+    assert result.exit_code == 0  # Ensure the command executed successfully
+    # Validate behavior for when only the required argument is provided
+    assert "-----------" in result.output
```

### Comparing `altimate-datapilot-cli-0.0.8/tests/core/platform/dbt/test_utils.py` & `altimate-datapilot-cli-0.0.9/tests/core/platform/dbt/test_utils.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/tests/data/catalog_v1.json` & `altimate-datapilot-cli-0.0.9/tests/data/catalog_v1.json`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/tests/data/manifest_v11.json` & `altimate-datapilot-cli-0.0.9/tests/data/manifest_v11.json`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/tests/data/manifests/manifest_js.json` & `altimate-datapilot-cli-0.0.9/tests/data/manifests/manifest_js.json`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/tests/data/manifests/manifest_js2.json` & `altimate-datapilot-cli-0.0.9/tests/data/manifests/manifest_js2.json`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/tests/data/manifests/manifest_js3.json` & `altimate-datapilot-cli-0.0.9/tests/data/manifests/manifest_js3.json`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/tests/data/manifests/manifest_tuva.json` & `altimate-datapilot-cli-0.0.9/tests/data/manifests/manifest_tuva.json`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/tests/data/manifests/manifest_tuva2.json` & `altimate-datapilot-cli-0.0.9/tests/data/manifests/manifest_tuva2.json`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/tests/data/manifests/manifest_tuva3.json` & `altimate-datapilot-cli-0.0.9/tests/data/manifests/manifest_tuva3.json`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/tests/utils/test_utils.py` & `altimate-datapilot-cli-0.0.9/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-cli-0.0.8/tox.ini` & `altimate-datapilot-cli-0.0.9/tox.ini`

 * *Files identical despite different names*


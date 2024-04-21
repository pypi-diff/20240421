# Comparing `tmp/kedro_pandera-0.1.0.tar.gz` & `tmp/kedro_pandera-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_pandera-0.1.0.tar", last modified: Sun Sep  3 07:08:54 2023, max compression
+gzip compressed data, was "kedro_pandera-0.2.0.tar", last modified: Sun Apr 21 19:01:54 2024, max compression
```

## Comparing `kedro_pandera-0.1.0.tar` & `kedro_pandera-0.2.0.tar`

### file list

```diff
@@ -1,122 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.662665 kedro_pandera-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (999)      174 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.654665 kedro_pandera-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.654665 kedro_pandera-0.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (999)     1689 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (999)      621 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (999)     1295 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (999)      125 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.654665 kedro_pandera-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)      452 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/.github/workflows/check-links.yml
--rw-r--r--   0 runner    (1001) docker     (999)     2754 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/.github/workflows/prepare-release.yml
--rw-r--r--   0 runner    (1001) docker     (999)     2561 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1642 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1872 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)      688 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/.gitpod.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1331 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      583 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1310 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (999)     3288 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (999)     2874 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (999)    11357 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      116 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (999)     8860 2023-09-03 07:08:54.662665 kedro_pandera-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     7959 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (999)       40 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.654665 kedro_pandera-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (999)      634 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (999)     2835 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.654665 kedro_pandera-0.1.0/docs/imgs/
--rw-r--r--   0 runner    (1001) docker     (999)    19781 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/docs/imgs/failed_validation_during_kedro_run.png
--rw-r--r--   0 runner    (1001) docker     (999)    33287 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/docs/imgs/log_failed_validation_during_kedro_run.png
--rw-r--r--   0 runner    (1001) docker     (999)    55203 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/docs/imgs/successful_validation_during_kedro_run.png
--rw-r--r--   0 runner    (1001) docker     (999)      325 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)      760 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.650664 kedro_pandera-0.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/docs/source/01_tutorials/
--rw-r--r--   0 runner    (1001) docker     (999)     8798 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/docs/source/01_tutorials/01_getting_started.md
--rw-r--r--   0 runner    (1001) docker     (999)     1241 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/docs/source/01_tutorials/02_dataframe_model.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/kedro_pandera/
--rw-r--r--   0 runner    (1001) docker     (999)      111 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/kedro_pandera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/kedro_pandera/framework/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/kedro_pandera/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/kedro_pandera/framework/cli/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/kedro_pandera/framework/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4320 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/kedro_pandera/framework/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/kedro_pandera/framework/config/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/kedro_pandera/framework/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1344 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/kedro_pandera/framework/config/resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/kedro_pandera/framework/hooks/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/kedro_pandera/framework/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2874 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/kedro_pandera/framework/hooks/pandera_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/kedro_pandera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     8860 2023-09-03 07:08:54.000000 kedro_pandera-0.1.0/kedro_pandera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     3900 2023-09-03 07:08:54.000000 kedro_pandera-0.1.0/kedro_pandera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-03 07:08:54.000000 kedro_pandera-0.1.0/kedro_pandera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)      168 2023-09-03 07:08:54.000000 kedro_pandera-0.1.0/kedro_pandera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-03 07:08:54.000000 kedro_pandera-0.1.0/kedro_pandera.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)      365 2023-09-03 07:08:54.000000 kedro_pandera-0.1.0/kedro_pandera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       14 2023-09-03 07:08:54.000000 kedro_pandera-0.1.0/kedro_pandera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       61 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/mlc_config.json
--rw-r--r--   0 runner    (1001) docker     (999)      259 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       39 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)      399 2023-09-03 07:08:54.662665 kedro_pandera-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     2785 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.650664 kedro_pandera-0.1.0/tests/_data/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/tests/_data/pandas-iris/
--rw-r--r--   0 runner    (1001) docker     (999)      301 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/cookiecutter.json
--rw-r--r--   0 runner    (1001) docker     (999)      331 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/prompts.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/
--rw-r--r--   0 runner    (1001) docker     (999)     1778 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)     4080 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/
--rw-r--r--   0 runner    (1001) docker     (999)     1080 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/
--rw-r--r--   0 runner    (1001) docker     (999)     1488 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
--rw-r--r--   0 runner    (1001) docker     (999)      854 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/logging.yml
--rw-r--r--   0 runner    (1001) docker     (999)       59 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/local/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.650664 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/01_raw/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (999)     3858 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/01_raw/iris.csv
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/02_intermediate/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/03_primary/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/04_feature/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.658665 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/05_model_input/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.662665 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/06_models/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.662665 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/07_model_output/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.662665 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/08_reporting/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (999)      446 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       47 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.662665 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/
--rw-r--r--   0 runner    (1001) docker     (999)      343 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)     1198 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.662665 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/
--rw-r--r--   0 runner    (1001) docker     (999)     1892 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/README.md
--rw-r--r--   0 runner    (1001) docker     (999)       60 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1535 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2061 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/nodes.py
--rw-r--r--   0 runner    (1001) docker     (999)      919 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (999)      399 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
--rw-r--r--   0 runner    (1001) docker     (999)     1540 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
--rw-r--r--   0 runner    (1001) docker     (999)     1582 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.662665 kedro_pandera-0.1.0/tests/framework/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.662665 kedro_pandera-0.1.0/tests/framework/cli/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/framework/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      886 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/framework/cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (999)      785 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/framework/cli/test_cli_infer_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:54.662665 kedro_pandera-0.1.0/tests/framework/config/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/framework/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3667 2023-09-03 07:08:43.000000 kedro_pandera-0.1.0/tests/framework/config/test_resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.901532 kedro_pandera-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.889532 kedro_pandera-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.889532 kedro_pandera-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.github/workflows/check-links.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.github/workflows/prepare-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.gitpod.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-21 19:01:54.901532 kedro_pandera-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/docs/imgs/
+-rw-r--r--   0 runner    (1001) docker     (127)    19781 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/imgs/failed_validation_during_kedro_run.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33287 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/imgs/log_failed_validation_during_kedro_run.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55203 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/imgs/successful_validation_during_kedro_run.png
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/docs/source/01_tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/source/01_tutorials/01_getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/source/01_tutorials/02_dataframe_model.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/source/migration_guide.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/kedro_pandera/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/kedro_pandera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/kedro_pandera/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/kedro_pandera/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/kedro_pandera/framework/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/kedro_pandera/framework/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/kedro_pandera/framework/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/kedro_pandera/framework/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/kedro_pandera/framework/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/kedro_pandera/framework/config/resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/kedro_pandera/framework/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/kedro_pandera/framework/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/kedro_pandera/framework/hooks/pandera_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/kedro_pandera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-21 19:01:54.000000 kedro_pandera-0.2.0/kedro_pandera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-21 19:01:54.000000 kedro_pandera-0.2.0/kedro_pandera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:01:54.000000 kedro_pandera-0.2.0/kedro_pandera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-21 19:01:54.000000 kedro_pandera-0.2.0/kedro_pandera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:01:54.000000 kedro_pandera-0.2.0/kedro_pandera.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-21 19:01:54.000000 kedro_pandera-0.2.0/kedro_pandera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 19:01:54.000000 kedro_pandera-0.2.0/kedro_pandera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/mlc_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-21 19:01:54.901532 kedro_pandera-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.885532 kedro_pandera-0.2.0/tests/_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/cookiecutter.json
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/prompts.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/logging.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.885532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/01_raw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/01_raw/iris.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/02_intermediate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/03_primary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/04_feature/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/05_model_input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/06_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/07_model_output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/08_reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.901532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.901532 kedro_pandera-0.2.0/tests/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.901532 kedro_pandera-0.2.0/tests/framework/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/framework/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/framework/cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/framework/cli/test_cli_infer_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.901532 kedro_pandera-0.2.0/tests/framework/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/framework/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/framework/config/test_resolvers.py
```

### Comparing `kedro_pandera-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `kedro_pandera-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `kedro_pandera-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/.github/PULL_REQUEST_TEMPLATE.md` & `kedro_pandera-0.2.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/.github/workflows/prepare-release.yml` & `kedro_pandera-0.2.0/.github/workflows/prepare-release.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 name: create-release-candidate
 
 on:
   workflow_dispatch:
     inputs:
       version_part:
         description: The part of the version to update (patch, minor or major)
+        type: choice
+        options:
+        - patch
+        - minor
+        - major
+        default: 'patch'
         required: true
-        default: 'minor'
 
 jobs:
   prepare-release:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.10"]
+        python-version: [3.11]
     env:
       PYTHON_PACKAGE: kedro_pandera
     steps:
-    - uses: actions/checkout@v2
-    - name: Set up Python  ${{ matrix.python-version }}
-      uses: actions/setup-python@v1
+    - uses: actions/checkout@v4
+    - name: Set up Python ${{ matrix.python-version }}
+      uses: actions/setup-python@v4
       with:
-        python-version:  ${{ matrix.python-version }}
+        python-version: ${{ matrix.python-version }}
     - name: Validate inputs
       run: |
-        echo "INPUT_VERSION_PART:  ${{ github.event.inputs.version_part }}"
-        python -c "if '${{ github.event.inputs.version_part }}' not in ['patch', 'minor', 'major']:   raise ValueError(\"'${{ github.event.inputs.version_part }}' must be one of ['patch', 'minor', 'major'])\")"
+        echo "INPUT_VERSION_PART: ${{ github.event.inputs.version_part }}"
     - name: Bump the version number  # bump2version is a maintained fork of original bumpversion
       id: bump_version
       run: |
-        pip install bump2version
-        bump2version ${{ github.event.inputs.version_part }}
-        echo "::set-output name=package_version::$(cat $PYTHON_PACKAGE/__init__.py | grep -Po  '\d+\.\d+\.\d+')"
+        pip install bump-my-version
+        bump-my-version bump ${{ github.event.inputs.version_part }}
+        echo "package_version=$(cat $PYTHON_PACKAGE/__init__.py | grep -Po  '\d+\.\d+\.\d+')" >> $GITHUB_OUTPUT
     - name: Update the CHANGELOG according to 'Keep a Changelog' guidelines
       uses: thomaseizinger/keep-a-changelog-new-release@v1
       with:
         version: ${{ steps.bump_version.outputs.package_version }}
     - name: Create a new release branch
       run: |
         git config user.name github-actions
@@ -44,19 +48,16 @@
         git push -u origin release-${{ steps.bump_version.outputs.package_version }}
     - name: Commit the changes
       run: |
         git commit -am "Bump version and CHANGELOG for release ${{ steps.bump_version.outputs.package_version }}"
         git push
     - name: Open a PR to merge the release to main
       id: open_pr
-      uses: vsoch/pull-request-action@1.0.12
+      run: |
+        gh pr create -B main -H release-${{ steps.bump_version.outputs.package_version }} --title "Release ${{ steps.bump_version.outputs.package_version }}" --body "Bump version and CHANGELOG for next release." --assignee "${{ github.repository_owner }}"
+        echo "pull_request_number=$(gh pr list --base main --json number,createdAt --jq 'sort_by(.createdAt) | reverse | .[0].number')" >> $GITHUB_OUTPUT
       env:
-        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-        PULL_REQUEST_BRANCH: main
-        PULL_REQUEST_FROM_BRANCH: release-${{ steps.bump_version.outputs.package_version }}
-        PULL_REQUEST_TITLE: "Release ${{ steps.bump_version.outputs.package_version }}"
-        PULL_REQUEST_BODY: "Bump version and CHANGELOG for next release."
-        PULL_REQUEST_ASSIGNEES: "${{ github.repository_owner }}"
+        GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
     - name: Change the commit message to add PR number
       run: |
         git commit -a --amend -m ":rocket: Bump version and CHANGELOG for release ${{ steps.bump_version.outputs.package_version }} (#${{ steps.open_pr.outputs.pull_request_number }})"
         git push -f
```

### Comparing `kedro_pandera-0.1.0/.github/workflows/publish.yml` & `kedro_pandera-0.2.0/.github/workflows/publish.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 name: publish
 
 on: workflow_dispatch
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
-    env:
-      PYTHON_PACKAGE: kedro_pandera
+    environment:
+      name: release
     permissions:
+      contents: write  # IMPORTANT: this permission is mandatory to enable creating a release
       id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
-      contents: write  # IMPORTANT: this permission is mandatory for creating a release
+    env:
+      PYTHON_PACKAGE: kedro_pandera
     steps:
     - name: Checkout the repo
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
       with:
         fetch-depth: 0  # necessary to enable merging, all the history is needed
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: "3.10"
+        python-version: "3.11"
     - name: Build package dist from source # A better way will be : https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/ but pep 517 is still marked as experimental
       run: |
-        python setup.py sdist
-    - name: Set dynamically package version as output variable # see https://github.com/actions/create-release/issues/39
-      # see https://docs.github.com/en/free-pro-team@latest/actions/reference/workflow-commands-for-github-actions#setting-an-environment-variable
+        pip install wheel
+        python setup.py sdist bdist_wheel
+    - name: Set dynamically package version as output variable
+      # see https://docs.github.com/en/actions/using-workflows/workflow-commands-for-github-actions#example-of-setting-an-output-parameter
       id: set_package_version
       run: |
-        echo "PACKAGE_VERSION=$(cat $PYTHON_PACKAGE/__init__.py | grep -Po  '\d+\.\d+\.\d+')" >> $GITHUB_OUTPUT
+        echo "PACKAGE_VERSION=$(cat $PYTHON_PACKAGE/__init__.py | grep -Po  '\d+\.\d+\.\d+')" >> "$GITHUB_OUTPUT"
     - name: Create temporary file with the body content for the release
       run: |
         grep -Poz "## \[${{steps.set_package_version.outputs.PACKAGE_VERSION}}] - \d{4}-\d{2}-\d{2}[\S\s]+?(?=## \[\d+\.\d+\.\d+\]|\[.+\]:)" CHANGELOG.md > release_body.md
-    - name: Create Release # https://github.com/actions/create-release
+    - name: Create Release
       id: create_release
-      uses: actions/create-release@v1.1.4
+      uses: softprops/action-gh-release@v2
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }} # This token is provided by Actions, you do not need to create your own token
       with:
         tag_name: ${{ steps.set_package_version.outputs.PACKAGE_VERSION }}
-        release_name: Release ${{ steps.set_package_version.outputs.PACKAGE_VERSION }}
+        name: Release ${{ steps.set_package_version.outputs.PACKAGE_VERSION }}
         body_path: ./release_body.md
         draft: false
         prerelease: false
     - name: Rollback Release in case of run failure
       if: failure() && steps.create_release.outputs.id != ''
       uses: author/action-rollback@stable
       with:
         # Using a known release ID
         release_id: ${{ steps.create_release.outputs.id }}
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-    - name: Publish package distributions to PyPI
+
+    - name: Publish package distributions to Test PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         verbose: true  # trace if the upload fails
```

### Comparing `kedro_pandera-0.1.0/.github/workflows/test.yml` & `kedro_pandera-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/.gitignore` & `kedro_pandera-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/.gitpod.yml` & `kedro_pandera-0.2.0/.gitpod.yml`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/.readthedocs.yml` & `kedro_pandera-0.2.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/CHANGELOG.md` & `kedro_pandera-0.2.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 # Changelog
 
 ## [Unreleased]
 
+## [0.2.0] - 2024-04-19
+
+### Changed
+
+-   :boom: :sparkles: :arrow_up: Drop support for `kedro==0.18.x` and add support for `kedro==0.19.x` ([#46](https://github.com/Galileo-Galilei/kedro-pandera/issues/46))
+
 ## [0.1.0] - 2023-09-02
 
 ### Added
 
 -   :sparkles: Add a CLI command to infer the schema of a dataset and persist it to a file ([#4](https://github.com/Galileo-Galilei/kedro-pandera/pull/4))
 -   :sparkles: Automatically register customer resolvers `pa.dict`, `pa.yaml` to make schema declaration easier in the catalog  ([#13](https://github.com/Galileo-Galilei/kedro-pandera/pull/13))
--  :sparkles: Automatically register customer resolver `pa.python` to enable schema declaration in the catalog from a ``DataframeModel`` class ([#32](https://github.com/Galileo-Galilei/kedro-pandera/pull/32))
+-   :sparkles: Automatically register customer resolver `pa.python` to enable schema declaration in the catalog from a `DataframeModel` class ([#32](https://github.com/Galileo-Galilei/kedro-pandera/pull/32))
 -   :sparkles: Add runtime validation : before running each node, data is validated against the schema declared in the catalog ([#13](https://github.com/Galileo-Galilei/kedro-pandera/pull/13))
 -   :loud_sound: `kedro-pandera` logs defaults is set to `INFO` so it is visible by default in the kedro logs ([#13](https://github.com/Galileo-Galilei/kedro-pandera/pull/13))
 -   :memo: Add a tutorial for using `kedro-pandera` ([#5](https://github.com/Galileo-Galilei/kedro-pandera/pull/5))
 
-[Unreleased]: https://github.com/Galileo-Galilei/kedro-pandera/compare/0.1.0...HEAD
+[Unreleased]: https://github.com/Galileo-Galilei/kedro-pandera/compare/0.2.0...HEAD
+
+[0.2.0]: https://github.com/Galileo-Galilei/kedro-pandera/compare/0.1.0...0.2.0
 
 [0.1.0]: https://github.com/Galileo-Galilei/kedro-pandera/compare/dcba7c128e5187c1a9b26430cddb274064ac96a4...0.1.0
```

### Comparing `kedro_pandera-0.1.0/CODE_OF_CONDUCT.md` & `kedro_pandera-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/CONTRIBUTING.md` & `kedro_pandera-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/LICENSE` & `kedro_pandera-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/PKG-INFO` & `kedro_pandera-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro_pandera
-Version: 0.1.0
+Version: 0.2.0
 Summary: A kedro plugin to use pandera in your kedro projects
 Home-page: https://github.com/Galileo-Galilei/kedro-pandera
 Author: Yolan Honoré-Rougé
 License: Apache Software License (Apache 2.0)
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,28 +21,28 @@
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 **General informations**
 
-[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://pypi.org/project/kedro-pandera/) [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
+[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://pypi.org/project/kedro-pandera/) [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/license/apache-2-0/) [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
 [![SemVer](https://img.shields.io/badge/semver-2.0.0-green)](https://semver.org/)
 
 ----------------------------------------------------------
 | Software repository | Latest release                                                                                                                             | Total downloads                                                                                                                    |
 | ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------- |
 | Pypi                | [![PyPI version](https://badge.fury.io/py/kedro-pandera.svg)](https://pypi.org/project/kedro-pandera/) | [![Downloads](https://pepy.tech/badge/kedro-pandera)](https://pepy.tech/project/kedro-pandera) |
 
 **Code health**
 
 ----------------------------------------------------------
 | Branch                                | Tests                                                                                                                                                                                                                                    | Coverage                                                                                                                                                                                                                                                                                               | Links                                                                                                                                                                                                                                                                                                                                                 | Documentation                                                                                                                                                                 | Deployment                                                                                                                                                                                                                                                                                                                                      | Activity                                                                                                                                                                                                                                                                     |
 | ------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `main` | [![test](https://github.com/Galileo-Galilei/kedro-pandera/workflows/test/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Atest+branch%3Amain) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main) | [![links](https://github.com/Galileo-Galilei/kedro-pandera/workflows/check-links/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Acheck-links+branch%3Amain) | [![Documentation](https://readthedocs.org/projects/kedro-pandera/badge/?version=stable)](https://kedro-pandera.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-pandera/workflows/publish/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=branch%3Amain+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-pandera/0.1.0)](https://github.com/Galileo-Galilei/kedro-pandera/compare/0.1.0...main) |
+| `main` | [![test](https://github.com/Galileo-Galilei/kedro-pandera/workflows/test/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Atest+branch%3Amain) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main) | [![links](https://github.com/Galileo-Galilei/kedro-pandera/workflows/check-links/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Acheck-links+branch%3Amain) | [![Documentation](https://readthedocs.org/projects/kedro-pandera/badge/?version=stable)](https://kedro-pandera.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-pandera/workflows/publish/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=branch%3Amain+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-pandera/0.2.0)](https://github.com/Galileo-Galilei/kedro-pandera/compare/0.2.0...main) |
 
 # What is kedro-pandera?
 
 
 # How do I install kedro-pandera?
 
 
@@ -69,15 +69,15 @@
 
 The [release history](https://github.com/Galileo-Galilei/kedro-pandera/blob/main/CHANGELOG.md) centralizes packages improvements across time. The main features coming in next releases are [listed on github milestones](https://github.com/Galileo-Galilei/kedro-pandera/milestones). Feel free to upvote/downvote and discuss prioritization in associated issues.
 
 # Disclaimer
 
 This package is still in active development. We use [SemVer](https://semver.org/) principles to version our releases. Until we reach `1.0.0` milestone, breaking changes will lead to `<minor>` version number increment, while releases which do not introduce breaking changes in the API will lead to `<patch>` version number increment.
 
-If you want to see how to migrate from one version of `kedro-pandera` to another, see the [migration guide](../docs/migration_guide.md).
+If you want to see how to migrate from one version of `kedro-pandera` to another, see the [migration guide](./docs/source/migration_guide.md).
 
 # Can I contribute?
 
 We'd be happy to receive help to maintain and improve the package. Any PR will be considered (from typo in the docs to core features add-on) Please check the [contributing guidelines](https://github.com/Galileo-Galilei/kedro-pandera/blob/main/CONTRIBUTING.md).
 
 # Main contributors
```

### Comparing `kedro_pandera-0.1.0/README.md` & `kedro_pandera-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 **General informations**
 
-[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://pypi.org/project/kedro-pandera/) [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
+[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://pypi.org/project/kedro-pandera/) [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/license/apache-2-0/) [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
 [![SemVer](https://img.shields.io/badge/semver-2.0.0-green)](https://semver.org/)
 
 ----------------------------------------------------------
 | Software repository | Latest release                                                                                                                             | Total downloads                                                                                                                    |
 | ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------- |
 | Pypi                | [![PyPI version](https://badge.fury.io/py/kedro-pandera.svg)](https://pypi.org/project/kedro-pandera/) | [![Downloads](https://pepy.tech/badge/kedro-pandera)](https://pepy.tech/project/kedro-pandera) |
 
 **Code health**
 
 ----------------------------------------------------------
 | Branch                                | Tests                                                                                                                                                                                                                                    | Coverage                                                                                                                                                                                                                                                                                               | Links                                                                                                                                                                                                                                                                                                                                                 | Documentation                                                                                                                                                                 | Deployment                                                                                                                                                                                                                                                                                                                                      | Activity                                                                                                                                                                                                                                                                     |
 | ------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `main` | [![test](https://github.com/Galileo-Galilei/kedro-pandera/workflows/test/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Atest+branch%3Amain) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main) | [![links](https://github.com/Galileo-Galilei/kedro-pandera/workflows/check-links/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Acheck-links+branch%3Amain) | [![Documentation](https://readthedocs.org/projects/kedro-pandera/badge/?version=stable)](https://kedro-pandera.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-pandera/workflows/publish/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=branch%3Amain+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-pandera/0.1.0)](https://github.com/Galileo-Galilei/kedro-pandera/compare/0.1.0...main) |
+| `main` | [![test](https://github.com/Galileo-Galilei/kedro-pandera/workflows/test/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Atest+branch%3Amain) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main) | [![links](https://github.com/Galileo-Galilei/kedro-pandera/workflows/check-links/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Acheck-links+branch%3Amain) | [![Documentation](https://readthedocs.org/projects/kedro-pandera/badge/?version=stable)](https://kedro-pandera.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-pandera/workflows/publish/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=branch%3Amain+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-pandera/0.2.0)](https://github.com/Galileo-Galilei/kedro-pandera/compare/0.2.0...main) |
 
 # What is kedro-pandera?
 
 
 # How do I install kedro-pandera?
 
 
@@ -44,15 +44,15 @@
 
 The [release history](https://github.com/Galileo-Galilei/kedro-pandera/blob/main/CHANGELOG.md) centralizes packages improvements across time. The main features coming in next releases are [listed on github milestones](https://github.com/Galileo-Galilei/kedro-pandera/milestones). Feel free to upvote/downvote and discuss prioritization in associated issues.
 
 # Disclaimer
 
 This package is still in active development. We use [SemVer](https://semver.org/) principles to version our releases. Until we reach `1.0.0` milestone, breaking changes will lead to `<minor>` version number increment, while releases which do not introduce breaking changes in the API will lead to `<patch>` version number increment.
 
-If you want to see how to migrate from one version of `kedro-pandera` to another, see the [migration guide](../docs/migration_guide.md).
+If you want to see how to migrate from one version of `kedro-pandera` to another, see the [migration guide](./docs/source/migration_guide.md).
 
 # Can I contribute?
 
 We'd be happy to receive help to maintain and improve the package. Any PR will be considered (from typo in the docs to core features add-on) Please check the [contributing guidelines](https://github.com/Galileo-Galilei/kedro-pandera/blob/main/CONTRIBUTING.md).
 
 # Main contributors
```

### Comparing `kedro_pandera-0.1.0/docs/Makefile` & `kedro_pandera-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/docs/conf.py` & `kedro_pandera-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/docs/imgs/failed_validation_during_kedro_run.png` & `kedro_pandera-0.2.0/docs/imgs/failed_validation_during_kedro_run.png`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/docs/imgs/log_failed_validation_during_kedro_run.png` & `kedro_pandera-0.2.0/docs/imgs/log_failed_validation_during_kedro_run.png`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/docs/imgs/successful_validation_during_kedro_run.png` & `kedro_pandera-0.2.0/docs/imgs/successful_validation_during_kedro_run.png`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/docs/make.bat` & `kedro_pandera-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/docs/source/01_tutorials/01_getting_started.md` & `kedro_pandera-0.2.0/docs/source/01_tutorials/01_getting_started.md`

 * *Files 0% similar despite different names*

```diff
@@ -70,29 +70,29 @@
 
 ```bash
 kedro pandera infer -d example_iris_data
 ```
 You should see the following message:
 
 ```bash
-[08/09/23 15:24:01] INFO     Loading data from 'example_iris_data' (CSVDataSet)...                                                  data_catalog.py:475
+[08/09/23 15:24:01] INFO     Loading data from 'example_iris_data' (CSVDataset)...                                                  data_catalog.py:475
 The schema is written to /path/to/project/pandas-iris/conf/base/catalog_example_iris_data.yml
 ```
 
 This will create a file ``/path/to/project/pandas-iris/conf/base/catalog_example_iris_data.yml`` with the default configuration.
 
 ```{warning}
 This CLI is a helper to avoid you to write the schema manually which is tedious but the documentation clearly states that "_these inferred schemas are **rough drafts** that shouldn’t be used for validation without modification_" (https://pandera.readthedocs.io/en/stable/schema_inference.html)
 ```
 
 ### Step 2: Update the catalog
 
 ```yaml
 example_iris_data:
-  type: pandas.CSVDataSet
+  type: pandas.CSVDataset
   filepath: data/01_raw/iris.csv
   metadata:
     pandera:
       schema: ${pa.yaml:_example_iris_data_schema}
 ```
 
 ```{note}
```

### Comparing `kedro_pandera-0.1.0/docs/source/01_tutorials/02_dataframe_model.md` & `kedro_pandera-0.2.0/docs/source/01_tutorials/02_dataframe_model.md`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ├── __init__.py
 └── example_iris_data.py
 ```
 
 ### Update the catalog
 ```yaml
 example_iris_data:
-  type: pandas.CSVDataSet
+  type: pandas.CSVDataset
   filepath: data/01_raw/iris.csv
   metadata:
     pandera:
       schema: ${pa.python:kedro_pandera_tutorial.schemas.ExampleIrisDataSchema}
 ```
 
 Here you will use the `pa.python` resolver to resolve the Python-based schema class.
```

### Comparing `kedro_pandera-0.1.0/kedro_pandera/framework/cli/cli.py` & `kedro_pandera-0.2.0/kedro_pandera/framework/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
+
 from pathlib import Path
-from typing import Optional
 
 import click
 import frictionless  # noqa: F401
 import yaml
 from kedro.framework.project import settings
 from kedro.framework.session import KedroSession
 from kedro.framework.startup import bootstrap_project
@@ -59,15 +60,15 @@
     default=None,
     help="The name of the file where the schema will be stored. Its extension must be '.yml' or '.py'. Default to 'dataset_name.yml'. ",
 )
 def infer_dataset_schema(
     dataset_name: str,
     use_python_ext: bool = False,
     env: str = "base",
-    outfile: Optional[str] = None,
+    outfile: str | None = None,
 ):
     """Infer the schema of a dataset and dump it in a catalog file
     so that it will enable validation at runtime.
     """
 
     project_path = Path().cwd()
     bootstrap_project(project_path)
```

### Comparing `kedro_pandera-0.1.0/kedro_pandera/framework/config/resolvers.py` & `kedro_pandera-0.2.0/kedro_pandera/framework/config/resolvers.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,9 +28,8 @@
 
 
 def resolve_dataframe_model(schema_name):
     import importlib
 
     module, _, schema = schema_name.rpartition(".")
     module = importlib.import_module(module)
-    print(f"{module=} {getattr(module, schema)=}")
     return getattr(module, schema)
```

### Comparing `kedro_pandera-0.1.0/kedro_pandera/framework/hooks/pandera_hook.py` & `kedro_pandera-0.2.0/kedro_pandera/framework/hooks/pandera_hook.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 
 from kedro.framework.context import KedroContext
 from kedro.framework.hooks import hook_impl
 from pandera.errors import SchemaError
 
 from kedro_pandera.framework.config.resolvers import (
+    resolve_dataframe_model,
     resolve_interpolated_yaml_schema,
     resolve_yaml_schema,
-    resolve_dataframe_model,
 )
 
 # if we do not import ``frictionless`` manually here, we get
 # >  ImportError: ('# ERROR: failed to register fsspec file#systems', TypeError("argument of type '_Cached' is not iterable"))
 # if we try to use ``Schema.to_yaml()`` after ``context.catalog``
 # The command ``kedro pandera infer-schema -d example_iris_data``
 # then raises the very useless error:
```

### Comparing `kedro_pandera-0.1.0/kedro_pandera.egg-info/PKG-INFO` & `kedro_pandera-0.2.0/kedro_pandera.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-pandera
-Version: 0.1.0
+Version: 0.2.0
 Summary: A kedro plugin to use pandera in your kedro projects
 Home-page: https://github.com/Galileo-Galilei/kedro-pandera
 Author: Yolan Honoré-Rougé
 License: Apache Software License (Apache 2.0)
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,28 +21,28 @@
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 **General informations**
 
-[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://pypi.org/project/kedro-pandera/) [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
+[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://pypi.org/project/kedro-pandera/) [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/license/apache-2-0/) [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
 [![SemVer](https://img.shields.io/badge/semver-2.0.0-green)](https://semver.org/)
 
 ----------------------------------------------------------
 | Software repository | Latest release                                                                                                                             | Total downloads                                                                                                                    |
 | ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------- |
 | Pypi                | [![PyPI version](https://badge.fury.io/py/kedro-pandera.svg)](https://pypi.org/project/kedro-pandera/) | [![Downloads](https://pepy.tech/badge/kedro-pandera)](https://pepy.tech/project/kedro-pandera) |
 
 **Code health**
 
 ----------------------------------------------------------
 | Branch                                | Tests                                                                                                                                                                                                                                    | Coverage                                                                                                                                                                                                                                                                                               | Links                                                                                                                                                                                                                                                                                                                                                 | Documentation                                                                                                                                                                 | Deployment                                                                                                                                                                                                                                                                                                                                      | Activity                                                                                                                                                                                                                                                                     |
 | ------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `main` | [![test](https://github.com/Galileo-Galilei/kedro-pandera/workflows/test/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Atest+branch%3Amain) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main) | [![links](https://github.com/Galileo-Galilei/kedro-pandera/workflows/check-links/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Acheck-links+branch%3Amain) | [![Documentation](https://readthedocs.org/projects/kedro-pandera/badge/?version=stable)](https://kedro-pandera.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-pandera/workflows/publish/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=branch%3Amain+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-pandera/0.1.0)](https://github.com/Galileo-Galilei/kedro-pandera/compare/0.1.0...main) |
+| `main` | [![test](https://github.com/Galileo-Galilei/kedro-pandera/workflows/test/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Atest+branch%3Amain) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main) | [![links](https://github.com/Galileo-Galilei/kedro-pandera/workflows/check-links/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Acheck-links+branch%3Amain) | [![Documentation](https://readthedocs.org/projects/kedro-pandera/badge/?version=stable)](https://kedro-pandera.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-pandera/workflows/publish/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=branch%3Amain+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-pandera/0.2.0)](https://github.com/Galileo-Galilei/kedro-pandera/compare/0.2.0...main) |
 
 # What is kedro-pandera?
 
 
 # How do I install kedro-pandera?
 
 
@@ -69,15 +69,15 @@
 
 The [release history](https://github.com/Galileo-Galilei/kedro-pandera/blob/main/CHANGELOG.md) centralizes packages improvements across time. The main features coming in next releases are [listed on github milestones](https://github.com/Galileo-Galilei/kedro-pandera/milestones). Feel free to upvote/downvote and discuss prioritization in associated issues.
 
 # Disclaimer
 
 This package is still in active development. We use [SemVer](https://semver.org/) principles to version our releases. Until we reach `1.0.0` milestone, breaking changes will lead to `<minor>` version number increment, while releases which do not introduce breaking changes in the API will lead to `<patch>` version number increment.
 
-If you want to see how to migrate from one version of `kedro-pandera` to another, see the [migration guide](../docs/migration_guide.md).
+If you want to see how to migrate from one version of `kedro-pandera` to another, see the [migration guide](./docs/source/migration_guide.md).
 
 # Can I contribute?
 
 We'd be happy to receive help to maintain and improve the package. Any PR will be considered (from typo in the docs to core features add-on) Please check the [contributing guidelines](https://github.com/Galileo-Galilei/kedro-pandera/blob/main/CONTRIBUTING.md).
 
 # Main contributors
```

### Comparing `kedro_pandera-0.1.0/kedro_pandera.egg-info/SOURCES.txt` & `kedro_pandera-0.2.0/kedro_pandera.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/imgs/failed_validation_during_kedro_run.png
 docs/imgs/log_failed_validation_during_kedro_run.png
 docs/imgs/successful_validation_during_kedro_run.png
+docs/source/migration_guide.md
 docs/source/01_tutorials/01_getting_started.md
 docs/source/01_tutorials/02_dataframe_model.md
 kedro_pandera/__init__.py
 kedro_pandera.egg-info/PKG-INFO
 kedro_pandera.egg-info/SOURCES.txt
 kedro_pandera.egg-info/dependency_links.txt
 kedro_pandera.egg-info/entry_points.txt
```

### Comparing `kedro_pandera-0.1.0/setup.py` & `kedro_pandera-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # Get the long description from the README file
 with open((HERE / "README.md").as_posix(), encoding="utf-8") as file_handler:
     README = file_handler.read()
 
 
 setup(
     name=NAME,
-    version="0.1.0",  # this will be bumped automatically by bump2version
+    version="0.2.0",  # this will be bumped automatically by bump2version
     description="A kedro plugin to use pandera in your kedro projects",
     license="Apache Software License (Apache 2.0)",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Galileo-Galilei/kedro-pandera",
     python_requires=">=3.8, <3.12",
     packages=find_packages(exclude=["docs*", "tests*"]),
@@ -44,19 +44,21 @@
             "sphinx-click>=3.1,<4.5",
             "sphinx_copybutton~=0.5.0",
             # "sphinx-sitemap",
             "sphinx-design",
             "myst-parser>=0.17.2,<2.1.0",
         ],
         "test": [
+            "ruff>=0.4.0, <0.5.0",
             "pytest>=7.0.0, <8.0.0",
             "pytest-cov>=4.0.0, <5.0.0",
             "pytest-mock",
             "pre-commit>=2.0.0,<4.0.0",
             "cookiecutter",
+            "kedro-datasets",
         ],
         "dev": [
             "pre-commit>=2.0.0,<4.0.0",
             "jupyter>=1.0.0,<2.0.0",
         ],
     },
     author="Yolan Honoré-Rougé",
```

### Comparing `kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/.gitignore` & `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/.gitignore`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/README.md` & `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/README.md`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/README.md` & `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 ## Instructions
 
 
 
 
 
 ## Find out more
-You can find out more about configuration from the [user guide documentation](https://kedro.readthedocs.io/en/stable/user_guide/configuration.html).
+You can find out more about configuration from the [user guide documentation](https://docs.kedro.org/en/stable/configuration/configuration_basics.html).
```

### Comparing `kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/catalog.yml` & `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/catalog.yml`

 * *Files 9% similar despite different names*

```diff
@@ -4,44 +4,44 @@
 # Link: https://kedro.readthedocs.io/en/stable/data/data_catalog.html
 #
 # We support interacting with a variety of data stores including local file systems, cloud, network and HDFS
 #
 # An example data set definition can look as follows:
 #
 #bikes:
-#  type: pandas.CSVDataSet
+#  type: pandas.CSVDataset
 #  filepath: "data/01_raw/bikes.csv"
 #
 #weather:
-#  type: spark.SparkDataSet
+#  type: spark.SparkDataset
 #  filepath: s3a://your_bucket/data/01_raw/weather*
 #  file_format: csv
 #  credentials: dev_s3
 #  load_args:
 #    header: True
 #    inferSchema: True
 #  save_args:
 #    sep: '|'
 #    header: True
 #
 #scooters:
-#  type: pandas.SQLTableDataSet
+#  type: pandas.SQLTableDataset
 #  credentials: scooters_credentials
 #  table_name: scooters
 #  load_args:
 #    index_col: ['name']
 #    columns: ['name', 'gear']
 #  save_args:
 #    if_exists: 'replace'
 #    # if_exists: 'fail'
 #    # if_exists: 'append'
 #
-# The Data Catalog supports being able to reference the same file using two different DataSet implementations
+# The Data Catalog supports being able to reference the same file using two different Dataset implementations
 # (transcoding), templating and a way to reuse arguments that are frequently repeated. See more here:
 # https://kedro.readthedocs.io/en/stable/data/data_catalog.html
 #
 # This is a data set used by the "Hello World" example pipeline provided with the project
 # template. Please feel free to remove it once you remove the example pipeline.
 
 example_iris_data:
-  type: pandas.CSVDataSet
+  type: pandas.CSVDataset
   filepath: data/01_raw/iris.csv
```

### Comparing `kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/logging.yml` & `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/logging.yml`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/01_raw/iris.csv` & `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/01_raw/iris.csv`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/setup.py` & `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/setup.py`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/README.md` & `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ## Pipeline inputs
 
 ### `example_iris_data`
 
 |      |                    |
 | ---- | ------------------ |
-| Type | `pandas.CSVDataSet` |
+| Type | `pandas.CSVDataset` |
 | Description | Example iris data containing columns |
 
 
 ### `parameters`
 
 |      |                    |
 | ---- | ------------------ |
```

### Comparing `kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py` & `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """{{ cookiecutter.project_name }} file for ensuring the package is executable
 as `{{ cookiecutter.repo_name }}` and `python -m {{ cookiecutter.python_package }}`
 """
+
 import importlib
 from pathlib import Path
 
 from kedro.framework.cli.utils import KedroCliError, load_entry_points
 from kedro.framework.project import configure_project
```

### Comparing `kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/nodes.py` & `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/nodes.py`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline.py` & `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline.py`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py` & `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/tests/conftest.py` & `kedro_pandera-0.2.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     }
 
     cookiecutter(
         str(TEMPLATE_PATH),
         output_dir=config["output_dir"],
         no_input=True,
         extra_context=config,
+        accept_hooks=False,
     )
     return tmp_path / _FAKE_REPO_NAME
 
 
 @pytest.fixture
 def kedro_project_iris(tmp_path):
     # TODO : this is also an integration test since this depends from the kedro version
```

### Comparing `kedro_pandera-0.1.0/tests/framework/cli/test_cli.py` & `kedro_pandera-0.2.0/tests/framework/cli/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,13 +14,13 @@
     for cmd_detailed in cmd_list_detailed:
         cmd_match = re.search(r"[\w-]+(?=  )", string=cmd_detailed)
         if cmd_match is not None:
             cmd_list.append(cmd_match.group(0))
     return cmd_list
 
 
-def test_mlflow_commands_inside_kedro_project(monkeypatch, kedro_project):
+def test_pandera_commands_inside_kedro_project(monkeypatch, kedro_project):
     monkeypatch.chdir(kedro_project)
     # launch the command to initialize the project
     cli_runner = CliRunner()
     result = cli_runner.invoke(cli_pandera)
     assert {"infer"} == set(extract_cmd_from_help(result.output))
```

### Comparing `kedro_pandera-0.1.0/tests/framework/cli/test_cli_infer_schema.py` & `kedro_pandera-0.2.0/tests/framework/cli/test_cli_infer_schema.py`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.1.0/tests/framework/config/test_resolvers.py` & `kedro_pandera-0.2.0/tests/framework/config/test_resolvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
 def test_resolve_yaml_schema_works_as_resolver():
     # maybe not a useful test: after all, this is OmegaConf responsibility
     with register_temporary_resolver("pa.dict", resolve_yaml_schema):
         config = OmegaConf.create(
             {
                 "my_data": {
-                    "type": "pandas.CSVDataSet",
+                    "type": "pandas.CSVDataset",
                     "filepath": "path/to/data.csv",
                     "metadata": {
                         "pandera": {
                             "schema": "${pa.dict:${oc.select:_data_schema,null}}",
                         }
                     },
                 },
@@ -104,15 +104,15 @@
         assert isinstance(config.my_data.metadata.pandera.schema, DataFrameSchema)
 
 
 def test_resolve_interpolated_yaml_schema():
     config = OmegaConf.create(
         {
             "my_data": {
-                "type": "pandas.CSVDataSet",
+                "type": "pandas.CSVDataset",
                 "filepath": "path/to/data.csv",
                 "metadata": {
                     "pandera": {
                         "schema": "${_data_schema}",
                     }
                 },
             },
```


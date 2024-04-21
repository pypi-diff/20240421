# Comparing `tmp/map_with_stats-0.1.2.tar.gz` & `tmp/map_with_stats-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "map_with_stats-0.1.2.tar", last modified: Mon Jul 31 17:32:22 2023, max compression
+gzip compressed data, was "map_with_stats-0.2.0.tar", last modified: Sun Apr 21 17:51:37 2024, max compression
```

## Comparing `map_with_stats-0.1.2.tar` & `map_with_stats-0.2.0.tar`

### file list

```diff
@@ -1,51 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.132650 map_with_stats-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.124651 map_with_stats-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.128651 map_with_stats-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/.github/workflows/publish_prod.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/.github/workflows/publish_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/.github/workflows/publish_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.128651 map_with_stats-0.1.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-31 17:32:22.132650 map_with_stats-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.128651 map_with_stats-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.128651 map_with_stats-0.1.2/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/docs/assets/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/docs/assets/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/docs/faq.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.128651 map_with_stats-0.1.2/docs/figs/
--rw-r--r--   0 runner    (1001) docker     (123)  1021823 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/docs/figs/map_screenshot.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/docs/quick_start.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.128651 map_with_stats-0.1.2/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/environment/linux.env
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/environment/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/environment/requirements_lib.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/environment/windows.env
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 17:32:22.132650 map_with_stats-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.124651 map_with_stats-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.132650 map_with_stats-0.1.2/src/map_with_stats/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/src/map_with_stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 17:32:21.000000 map_with_stats-0.1.2/src/map_with_stats/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/src/map_with_stats/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/src/map_with_stats/map.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/src/map_with_stats/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/src/map_with_stats/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.132650 map_with_stats-0.1.2/src/map_with_stats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-31 17:32:22.000000 map_with_stats-0.1.2/src/map_with_stats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-31 17:32:22.000000 map_with_stats-0.1.2/src/map_with_stats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:32:22.000000 map_with_stats-0.1.2/src/map_with_stats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-31 17:32:22.000000 map_with_stats-0.1.2/src/map_with_stats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 17:32:22.000000 map_with_stats-0.1.2/src/map_with_stats.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.132650 map_with_stats-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:51:37.720744 map_with_stats-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:51:37.712745 map_with_stats-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:51:37.716745 map_with_stats-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/.github/workflows/publish_prod.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/.github/workflows/publish_template.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/.github/workflows/publish_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:51:37.716745 map_with_stats-0.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-21 17:51:37.720744 map_with_stats-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:51:37.716745 map_with_stats-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:51:37.716745 map_with_stats-0.2.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/docs/assets/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/docs/assets/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/docs/faq.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:51:37.716745 map_with_stats-0.2.0/docs/figs/
+-rw-r--r--   0 runner    (1001) docker     (127)  1021823 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/docs/figs/map_screenshot.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/docs/quick_start.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:51:37.716745 map_with_stats-0.2.0/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/environment/linux.env
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/environment/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/environment/requirements_lib.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/environment/windows.env
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:51:37.712745 map_with_stats-0.2.0/overrides/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:51:37.712745 map_with_stats-0.2.0/overrides/partials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:51:37.712745 map_with_stats-0.2.0/overrides/partials/integrations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:51:37.716745 map_with_stats-0.2.0/overrides/partials/integrations/analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/overrides/partials/integrations/analytics/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/overrides/partials/integrations/analytics/custom.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 17:51:37.720744 map_with_stats-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:51:37.712745 map_with_stats-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:51:37.720744 map_with_stats-0.2.0/src/map_with_stats/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/src/map_with_stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 17:51:37.000000 map_with_stats-0.2.0/src/map_with_stats/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/src/map_with_stats/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/src/map_with_stats/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/src/map_with_stats/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/src/map_with_stats/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:51:37.720744 map_with_stats-0.2.0/src/map_with_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-21 17:51:37.000000 map_with_stats-0.2.0/src/map_with_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-21 17:51:37.000000 map_with_stats-0.2.0/src/map_with_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 17:51:37.000000 map_with_stats-0.2.0/src/map_with_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-21 17:51:37.000000 map_with_stats-0.2.0/src/map_with_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 17:51:37.000000 map_with_stats-0.2.0/src/map_with_stats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:51:37.720744 map_with_stats-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 17:51:32.000000 map_with_stats-0.2.0/tests/test_utils.py
```

### Comparing `map_with_stats-0.1.2/.github/workflows/docs.yml` & `map_with_stats-0.2.0/.github/workflows/docs.yml`

 * *Files 24% similar despite different names*

```diff
@@ -5,20 +5,20 @@
       - main
 permissions:
   contents: write
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: 🐍 Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.9
-      - uses: actions/cache@v2
+      - uses: actions/cache@v4
         with:
           key: ${{ github.ref }}
           path: .cache
       - name: 💻 Install build dependencies
         run: pip install mkdocs-material>=9.0.0 mkdocstrings[python]
       - name: 📖 Publish HTML into GitHub Pages branch
         run: mkdocs gh-deploy --force
```

### Comparing `map_with_stats-0.1.2/.github/workflows/publish_template.yml` & `map_with_stats-0.2.0/.github/workflows/publish_template.yml`

 * *Files 10% similar despite different names*

```diff
@@ -21,19 +21,19 @@
   publish:
     name: Upload release to PyPI
     runs-on: ubuntu-latest
     environment:
       name: ${{ inputs.environment-name }}
       url: ${{ inputs.environment-url }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0 # Needs all tags to compute dynamic version
       - name: 🐍 Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.9"
       - name: 💻 Install dependencies
         run: pip install build
       - name: 🔨 Build distribution
         run: python -m build
       - name: 🚀 Publish package distributions to PyPI
```

### Comparing `map_with_stats-0.1.2/.github/workflows/test.yml` & `map_with_stats-0.2.0/.github/workflows/test.yml`

 * *Files 15% similar despite different names*

```diff
@@ -14,41 +14,41 @@
     strategy:
       fail-fast: false
       matrix:
         os:
           - macos-latest
           - ubuntu-latest
           - windows-latest
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
     runs-on: ${{ matrix.os }}
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: 🐍 Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: 💻 Install dependencies
         run: |
           pip install pytest pytest-cov
           pip install .
       - name: 🧪 Test with pytest
         run: pytest
 
   test_local_code:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: 🐍 Set up Python 3.9
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.9"
       - name: 💻 Install dependencies
         run: pip install -r requirements.txt
-      - name: 🧪 Lint with pylint
-        run: find src -type f -name "*.py" | xargs pylint -E -r y
+      - name: 🧪 Lint with ruff
+        run: ruff check .
       - name: 🧪 Test with pytest
         run: |
           export PYTHONPATH=$PWD/src:$PYTHONPATH
           pytest
       - name: 🧪 Code typing
         run: mypy
```

### Comparing `map_with_stats-0.1.2/.gitignore` & `map_with_stats-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.2/.pre-commit-config.yaml` & `map_with_stats-0.2.0/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,19 @@
     rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: check-added-large-files
       - id: check-docstring-first
       - id: check-merge-conflict
       - id: detect-private-key
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: b9787ef94f0d06972b93b36730548f0d928f26f9 # frozen: v0.0.285
+    hooks:
+      - id: ruff
+        args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/psf/black
     rev: ae2c0758c9e61a385df9700dc9c231bf54887041 # frozen: 22.3.0
     hooks:
       - id: black
         # skip-magic-trailing-comma: do not enforce splitting line if it ends with comma
         args: [--skip-magic-trailing-comma]
   - repo: https://github.com/timothycrosley/isort
```

### Comparing `map_with_stats-0.1.2/LICENSE` & `map_with_stats-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.2/PKG-INFO` & `map_with_stats-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: map_with_stats
-Version: 0.1.2
+Version: 0.2.0
 Summary: Interactive map with a choropleth displaying some statistics as color per hectare
 Author: Mischa Lisovyi
 License: MIT License
         
         Copyright (c) 2023 Mischa Lisovyi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,31 +29,34 @@
 Project-URL: Documentation, https://mlisovyi.github.io/map_with_stats/
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: folium<1.0,>=0.10
+Requires-Dist: geopandas<1.0,>=0.10
 
 # Map with statistics
 
 
 <!-- [![coverage report](https://git.intern.migros.net/analytics/optimizers/store_profile_common/badges/main/coverage.svg)](https://git.intern.migros.net/analytics/optimizers/store_profile_common/-/commits/main) -->
 [![release @ PYPI](http://img.shields.io/pypi/v/map_with_stats?color=brightgreen&logo=pypi&logoColor=949DA5)](https://pypi.python.org/pypi/map_with_stats)
-[![python version](https://img.shields.io/badge/python-3.7,3.8,3.9,3.10,3.11-blue.svg?logo=python&logoColor=949DA5)](https://www.python.org/downloads/)
+[![python version](https://img.shields.io/badge/python-3.7,3.8,3.9,3.10,3.11,3.12-blue.svg?logo=python&logoColor=949DA5)](https://www.python.org/downloads/)
 ![platform](https://img.shields.io/badge/platform-linux%20|%20macos%20|%20windows-lightgray.svg)
 [![CI status](https://github.com/mlisovyi/map_with_stats/actions/workflows/test.yml/badge.svg?labelColor=555555?event=push)](https://github.com/mlisovyi/map_with_stats)
 [![Docs status](https://github.com/mlisovyi/map_with_stats/actions/workflows/docs.yml/badge.svg)](https://github.com/mlisovyi/map_with_stats)
-[![linter](https://img.shields.io/badge/code%20linting-pylint-blue.svg)](https://github.com/PyCQA/pylint)
+[![linter](https://img.shields.io/badge/code%20linting-ruff-blue.svg)](https://github.com/astral-sh/ruff)
 [![testing](https://img.shields.io/badge/code%20testing-pytest-blue.svg)](https://github.com/pytest-dev/pytest)
 [![typing](https://img.shields.io/badge/code%20typing-mypy-blue.svg)](http://mypy-lang.org/)
 [![docs](https://img.shields.io/badge/documentation-mkdocs--material-blue.svg)](https://squidfunk.github.io/mkdocs-material/)
 [![versioning](https://img.shields.io/badge/versioning-setuptools--scm-blue.svg)](https://github.com/pypa/setuptools_scm)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![documentation](https://img.shields.io/badge/_-documentation-blueviolet?logo=githubpages)](https://mlisovyi.github.io/map_with_stats)
```

### Comparing `map_with_stats-0.1.2/README.md` & `map_with_stats-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Map with statistics
 
 
 <!-- [![coverage report](https://git.intern.migros.net/analytics/optimizers/store_profile_common/badges/main/coverage.svg)](https://git.intern.migros.net/analytics/optimizers/store_profile_common/-/commits/main) -->
 [![release @ PYPI](http://img.shields.io/pypi/v/map_with_stats?color=brightgreen&logo=pypi&logoColor=949DA5)](https://pypi.python.org/pypi/map_with_stats)
-[![python version](https://img.shields.io/badge/python-3.7,3.8,3.9,3.10,3.11-blue.svg?logo=python&logoColor=949DA5)](https://www.python.org/downloads/)
+[![python version](https://img.shields.io/badge/python-3.7,3.8,3.9,3.10,3.11,3.12-blue.svg?logo=python&logoColor=949DA5)](https://www.python.org/downloads/)
 ![platform](https://img.shields.io/badge/platform-linux%20|%20macos%20|%20windows-lightgray.svg)
 [![CI status](https://github.com/mlisovyi/map_with_stats/actions/workflows/test.yml/badge.svg?labelColor=555555?event=push)](https://github.com/mlisovyi/map_with_stats)
 [![Docs status](https://github.com/mlisovyi/map_with_stats/actions/workflows/docs.yml/badge.svg)](https://github.com/mlisovyi/map_with_stats)
-[![linter](https://img.shields.io/badge/code%20linting-pylint-blue.svg)](https://github.com/PyCQA/pylint)
+[![linter](https://img.shields.io/badge/code%20linting-ruff-blue.svg)](https://github.com/astral-sh/ruff)
 [![testing](https://img.shields.io/badge/code%20testing-pytest-blue.svg)](https://github.com/pytest-dev/pytest)
 [![typing](https://img.shields.io/badge/code%20typing-mypy-blue.svg)](http://mypy-lang.org/)
 [![docs](https://img.shields.io/badge/documentation-mkdocs--material-blue.svg)](https://squidfunk.github.io/mkdocs-material/)
 [![versioning](https://img.shields.io/badge/versioning-setuptools--scm-blue.svg)](https://github.com/pypa/setuptools_scm)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![documentation](https://img.shields.io/badge/_-documentation-blueviolet?logo=githubpages)](https://mlisovyi.github.io/map_with_stats)
```

### Comparing `map_with_stats-0.1.2/docs/assets/favicon-16x16.png` & `map_with_stats-0.2.0/docs/assets/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.2/docs/assets/favicon-32x32.png` & `map_with_stats-0.2.0/docs/assets/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.2/docs/faq.md` & `map_with_stats-0.2.0/docs/faq.md`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.2/docs/figs/map_screenshot.jpeg` & `map_with_stats-0.2.0/docs/figs/map_screenshot.jpeg`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.2/docs/index.md` & `map_with_stats-0.2.0/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Map with statistics
 
 
 <!-- [![coverage report](https://git.intern.migros.net/analytics/optimizers/store_profile_common/badges/main/coverage.svg)](https://git.intern.migros.net/analytics/optimizers/store_profile_common/-/commits/main) -->
 [![release @ PYPI](http://img.shields.io/pypi/v/map_with_stats?color=brightgreen&logo=pypi&logoColor=949DA5)](https://pypi.python.org/pypi/map_with_stats)
-[![python version](https://img.shields.io/badge/python-3.7,3.8,3.9,3.10,3.11-blue.svg?logo=python&logoColor=949DA5)](https://www.python.org/downloads/)
+[![python version](https://img.shields.io/badge/python-3.7,3.8,3.9,3.10,3.11,3.12-blue.svg?logo=python&logoColor=949DA5)](https://www.python.org/downloads/)
 ![platform](https://img.shields.io/badge/platform-linux%20|%20macos%20|%20windows-lightgray.svg)
 [![CI status](https://github.com/mlisovyi/map_with_stats/actions/workflows/test.yml/badge.svg?labelColor=555555?event=push)](https://github.com/mlisovyi/map_with_stats)
 [![Docs status](https://github.com/mlisovyi/map_with_stats/actions/workflows/docs.yml/badge.svg)](https://github.com/mlisovyi/map_with_stats)
-[![linter](https://img.shields.io/badge/code%20linting-pylint-blue.svg)](https://github.com/PyCQA/pylint)
+[![linter](https://img.shields.io/badge/code%20linting-ruff-blue.svg)](https://github.com/astral-sh/ruff)
 [![testing](https://img.shields.io/badge/code%20testing-pytest-blue.svg)](https://github.com/pytest-dev/pytest)
 [![typing](https://img.shields.io/badge/code%20typing-mypy-blue.svg)](http://mypy-lang.org/)
 [![docs](https://img.shields.io/badge/documentation-mkdocs--material-blue.svg)](https://squidfunk.github.io/mkdocs-material/)
 [![versioning](https://img.shields.io/badge/versioning-setuptools--scm-blue.svg)](https://github.com/pypa/setuptools_scm)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![documentation](https://img.shields.io/badge/_-documentation-blueviolet?logo=githubpages)](https://mlisovyi.github.io/map_with_stats)
```

### Comparing `map_with_stats-0.1.2/docs/quick_start.md` & `map_with_stats-0.2.0/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.2/mkdocs.yml` & `map_with_stats-0.2.0/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,30 @@
   - Introduction: "index.md"
   - Quick start guide: "quick_start.md"
   - FAQ: "faq.md"
   - API: "api.md"
 
 theme:
   name: material
+  # this parameter defines where to find HTML that will overwrite or complement the pages from the theme
+  custom_dir: overrides
   features:
     # enables annotations, see https://squidfunk.github.io/mkdocs-material/reference/code-blocks/#code-annotations
     - content.code.annotate
     # for navigation features see https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/
     - navigation.top
     - navigation.tracking
     # keep all sections in the navigation expanded by default
     - navigation.expand
     # add icon and link to the document on gihub for each page
     - content.action.edit
+    # add highlighting of search words
+    - search.highlight
+    # add autocomplete to the search bar
+    - search.suggest
   icon:
     logo: fontawesome/solid/map
     # icon for the git repository link on the top-right
     repo: fontawesome/brands/github
     # icon for the view of the current page in the repository
     edit: material/eye
   favicon: assets/favicon-32x32.png
@@ -74,16 +80,21 @@
 
 plugins:
   - search
   - mkdocstrings:
       handlers:
         python:
           # where to look for python modules. not strictly required, but helps, if building from an arbitrary folder
-          paths: [src]
+          # paths: [src]
           options:
             docstring_style: google
             show_if_no_docstring: True
             show_root_toc_entry: False
 
 # auto-reload on changes in the following folders outside of the docs (for development of docs)
 watch:
   - src
+
+# add analytics
+extra:
+  analytics:
+    provider: custom
```

### Comparing `map_with_stats-0.1.2/pyproject.toml` & `map_with_stats-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -8,70 +8,94 @@
 write_to = "src/map_with_stats/_version.py"
 version_scheme = "post-release"
 local_scheme = "no-local-version"
 
 [project]
 name = "map_with_stats"
 dynamic = ["version"]
-authors = [{name="Mischa Lisovyi"}]
+authors = [{ name = "Mischa Lisovyi" }]
 description = "Interactive map with a choropleth displaying some statistics as color per hectare"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Typing :: Typed",
 ]
 dependencies = ["folium>=0.10,<1.0", "geopandas>=0.10,<1.0"]
 
 [project.urls]
 "Homepage" = "https://github.com/mlisovyi/map_with_stats"
 "Documentation" = "https://mlisovyi.github.io/map_with_stats/"
 
 [tool.setuptools.dynamic]
-version = {attr = "map_with_stats._version.__version__"}
+version = { attr = "map_with_stats._version.__version__" }
 
 [tool.setuptools.packages.find]
-where = ["src"]  # ["."] by default
+where = ["src"]               # ["."] by default
 include = ["map_with_stats*"]
-namespaces = false  # true by default
+namespaces = false            # true by default
 
 [tool.setuptools.package-data]
 map_with_stats = ["py.typed"]
 
 [tool.pytest.ini_options]
 norecursedirs = '.*'
 # add --cov-report=html to generate an html report
 # in the html page one can well see which code is (not) covered
 # coverege report will be added to pytest run
 addopts = "--cov=src/map_with_stats --cov-report=term --cov-config=pyproject.toml --no-cov-on-fail"
 # pytest issues PytestDeprecationWarning about hooks in pytest_cov, so we filter those out
-filterwarnings = ["ignore::FutureWarning", "ignore::pytest.PytestDeprecationWarning"]
-testpaths=["tests"]
+filterwarnings = [
+    "ignore::FutureWarning",
+    "ignore::pytest.PytestDeprecationWarning",
+]
+testpaths = ["tests"]
 
 [tool.coverage.run]
 # skip module and any further custom files
-omit =["*/__init__.py", "_version.py"]
+omit = ["*/__init__.py", "_version.py"]
+
+[tool.ruff]
+select = [
+    "E",   # pycodestyle
+    "W",   # pycodestyle
+    "F",   # pyflakes
+    "N",   # naming according to PEP8
+    "D",   # pydocstyle
+    "PD",  # pandas linter
+    "NPY", # numpy linter
+]
+ignore = [
+    "E501", # line length is regulated by black
+    "D100", # modules typically have no doc-string in this project
+    "D104", # packages typically have no doc-string in this project
+]
+# used for resolution of first- vs third-party imports
+src = ["src"]
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["F403"]
+# don't complain about missing doc strings and usage of variable names in tests
+"tests/**/*.py" = ["D103", "N806", "PD901"]
+
+[tool.ruff.pydocstyle]
+convention = "google"
 
 [tool.mypy]
 # What files should be included.
-files =["src"]
+files = ["src"]
 # We want to be as strict as possible but allow reexports
 strict = true
 implicit_reexport = true
 
 [[tool.mypy.overrides]]
-module = [
-    "pandas",
-    "shapely",
-    "folium",
-    "geopandas",
-    "shapely.ops"
-]
-ignore_missing_imports = true
+module = ["pandas", "shapely", "folium", "geopandas", "shapely.ops"]
+ignore_missing_imports = true
```

### Comparing `map_with_stats-0.1.2/src/map_with_stats/data.py` & `map_with_stats-0.2.0/src/map_with_stats/data.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,43 +24,58 @@
     mask_x = df["X"].between(ch_x_min, ch_x_max)
     mask_y = df["Y"].between(ch_y_min, ch_y_max)
     mask_in_range = mask_x & mask_y
     return df[mask_in_range]
 
 
 def create_geo_df_with_hectar_polygons(
-    df: pd.DataFrame, col_value: str, crs_out: str = "EPSG:4326"
+    df: pd.DataFrame,
+    col_value: str,
+    crs_out: str = "EPSG:4326",
+    crs_in: str = "EPSG:21781",
+    grid_size: int = 100,
 ) -> gpd.GeoDataFrame:
-    """Given a pandas dataframe with _"X", "Y"_ coordinates of the bottom-left (south-west) corner
+    """Generate hectare polygons.
+
+    Given a pandas dataframe with _"X", "Y"_ coordinates of the bottom-left (south-west) corner
     of the hectares and a column `col_value` with values, create a geopandas geodataframe with
-    hectare polygons and the selected column with values
+    hectare polygons and the selected column with values.
 
     Args:
         df (pd.DataFrame): input data. The code expects to find the following columns: _"X", "Y", `col_value`_.
         col_value (str): column name with some values
-        crs_out (_type_, optional): coordinate system to which output polygons are transformed.
+        crs_out (str, optional): coordinate system to which output polygons are transformed.
             Defaults to "EPSG:4326".
+        crs_in (str, optional): coordinate system of the input data. Defaults to "EPSG:21781" (=LV03).
+        grid_size (int, optional): grid size in meters. Defaults to 100 ()i.e. hectar.
 
     Returns:
         gpd.GeoDataFrame: a table with hectare polygons and the values.
     """
     _check_cols_in_df(df, ["X", "Y", col_value])
     polygons = []
     for row in df.itertuples():
         x, y = row.X, row.Y
         polygons.append(
-            shapely.Polygon([(x, y), (x + 100, y), (x + 100, y + 100), (x, y + 100)])
+            shapely.Polygon(
+                [
+                    (x, y),
+                    (x + grid_size, y),
+                    (x + grid_size, y + grid_size),
+                    (x, y + grid_size),
+                ]
+            )
         )
     gdf_stats = gpd.GeoDataFrame(
         {
             "geometry": polygons,
             "value": df[col_value],
-            "hectare_id": df["X"] // 100 * 10_000 + df["Y"] // 100,
+            "hectare_id": df["X"] // grid_size * 10_000 + df["Y"] // grid_size,
             "X": df["X"],
             "Y": df["Y"],
         },
         index=df.index,
-        crs="EPSG:21781",  # LV03 coordinate system
+        crs=crs_in,
     )
     # transform into the desired coordinate system
     gdf_stats = gdf_stats.to_crs(crs_out)
     return gdf_stats
```

### Comparing `map_with_stats-0.1.2/src/map_with_stats/map.py` & `map_with_stats-0.2.0/src/map_with_stats/map.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     clip_quantile: Optional[float] = 0.01,
     map_tiles_provider: str = "OpenStreetMap",
     optimise_choropleth_size: bool = True,
     coordinates_start: Tuple[float, float] = (47.39, 8.53),
     zoom_start: int = 15,
     max_n_hectares_to_display: Optional[int] = None,
     plot_boundaries: bool = False,
+    fill_opacity: float = 0.6,
 ) -> folium.Map:
     """Generate a folium map with the some statistics per hectare added as a choropleth alayer on top.
 
     See [FAQ](faq) for detailed explanation and typical use-cases of more complex attributes.
 
     Args:
         gdf_stats (gpd.GeoDataFrame): input table with the hectare polygons and statistics values.
@@ -45,22 +46,22 @@
             Defaults to (47.39, 8.53) [Zürich].
         zoom_start (int, optional): starting zoom. Defaults to 15.
         max_n_hectares_to_display (Optional[int], optional): the top-N hectares to display.
             Defaults to None.
         plot_boundaries (bool, optional): set to True to display boundaries between choroplet elements.
             This is useful if you visualise not hectares but some administrative entities.
             Defaults to False.
+        fill_opacity (float, optional): opacity of the choropleth. Defaults to 0.6.
 
     Raises:
         ValueError: unsupported `bins_type` provided.
 
     Returns:
         folium.Map: the map with cholopleth layer
     """
-
     _check_cols_in_df(gdf_stats, ["geometry", "value"])
 
     # make a copy to avoid modifying input data in-place
     gdf = gdf_stats.copy(deep=True)
 
     ch_map = folium.Map(
         location=coordinates_start, zoom_start=zoom_start, tiles=map_tiles_provider
@@ -105,15 +106,15 @@
     # coloured choropleth with the colour reflecting the statistics value
     # for example squares in the case of hectares
     choropleth = folium.Choropleth(
         geo_data=gdf,
         data=cliped_values,
         key_on="feature.id",  # index of the geodataframe is transformed into `id` field
         fill_color="YlOrBr",
-        fill_opacity=0.6,
+        fill_opacity=fill_opacity,
         bins=bins,
         line_weight=line_weight,
         line_color=line_color,
         nan_fill_opacity=1,  # fully transparent hectares if the valueis mising
         legend_name=title,  # title under the color scale
         name=title,  # name of thew layer, e.g. in the layer control
     ).add_to(ch_map)
```

### Comparing `map_with_stats-0.1.2/src/map_with_stats/utils.py` & `map_with_stats-0.2.0/src/map_with_stats/utils.py`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.2/src/map_with_stats.egg-info/PKG-INFO` & `map_with_stats-0.2.0/src/map_with_stats.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: map-with-stats
-Version: 0.1.2
+Name: map_with_stats
+Version: 0.2.0
 Summary: Interactive map with a choropleth displaying some statistics as color per hectare
 Author: Mischa Lisovyi
 License: MIT License
         
         Copyright (c) 2023 Mischa Lisovyi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,31 +29,34 @@
 Project-URL: Documentation, https://mlisovyi.github.io/map_with_stats/
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: folium<1.0,>=0.10
+Requires-Dist: geopandas<1.0,>=0.10
 
 # Map with statistics
 
 
 <!-- [![coverage report](https://git.intern.migros.net/analytics/optimizers/store_profile_common/badges/main/coverage.svg)](https://git.intern.migros.net/analytics/optimizers/store_profile_common/-/commits/main) -->
 [![release @ PYPI](http://img.shields.io/pypi/v/map_with_stats?color=brightgreen&logo=pypi&logoColor=949DA5)](https://pypi.python.org/pypi/map_with_stats)
-[![python version](https://img.shields.io/badge/python-3.7,3.8,3.9,3.10,3.11-blue.svg?logo=python&logoColor=949DA5)](https://www.python.org/downloads/)
+[![python version](https://img.shields.io/badge/python-3.7,3.8,3.9,3.10,3.11,3.12-blue.svg?logo=python&logoColor=949DA5)](https://www.python.org/downloads/)
 ![platform](https://img.shields.io/badge/platform-linux%20|%20macos%20|%20windows-lightgray.svg)
 [![CI status](https://github.com/mlisovyi/map_with_stats/actions/workflows/test.yml/badge.svg?labelColor=555555?event=push)](https://github.com/mlisovyi/map_with_stats)
 [![Docs status](https://github.com/mlisovyi/map_with_stats/actions/workflows/docs.yml/badge.svg)](https://github.com/mlisovyi/map_with_stats)
-[![linter](https://img.shields.io/badge/code%20linting-pylint-blue.svg)](https://github.com/PyCQA/pylint)
+[![linter](https://img.shields.io/badge/code%20linting-ruff-blue.svg)](https://github.com/astral-sh/ruff)
 [![testing](https://img.shields.io/badge/code%20testing-pytest-blue.svg)](https://github.com/pytest-dev/pytest)
 [![typing](https://img.shields.io/badge/code%20typing-mypy-blue.svg)](http://mypy-lang.org/)
 [![docs](https://img.shields.io/badge/documentation-mkdocs--material-blue.svg)](https://squidfunk.github.io/mkdocs-material/)
 [![versioning](https://img.shields.io/badge/versioning-setuptools--scm-blue.svg)](https://github.com/pypa/setuptools_scm)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![documentation](https://img.shields.io/badge/_-documentation-blueviolet?logo=githubpages)](https://mlisovyi.github.io/map_with_stats)
```

### Comparing `map_with_stats-0.1.2/src/map_with_stats.egg-info/SOURCES.txt` & `map_with_stats-0.2.0/src/map_with_stats.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 docs/assets/favicon-16x16.png
 docs/assets/favicon-32x32.png
 docs/figs/map_screenshot.jpeg
 environment/linux.env
 environment/requirements_dev.txt
 environment/requirements_lib.txt
 environment/windows.env
+overrides/partials/integrations/analytics/.gitignore
+overrides/partials/integrations/analytics/custom.html
 src/map_with_stats/__init__.py
 src/map_with_stats/_version.py
 src/map_with_stats/data.py
 src/map_with_stats/map.py
 src/map_with_stats/py.typed
 src/map_with_stats/utils.py
 src/map_with_stats.egg-info/PKG-INFO
```

### Comparing `map_with_stats-0.1.2/tests/test_utils.py` & `map_with_stats-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*


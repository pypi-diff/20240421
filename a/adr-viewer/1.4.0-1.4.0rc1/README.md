# Comparing `tmp/adr_viewer-1.4.0.tar.gz` & `tmp/adr-viewer-1.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adr_viewer-1.4.0.tar", last modified: Sun Apr 21 13:27:30 2024, max compression
+gzip compressed data, was "adr-viewer-1.4.0rc1.tar", last modified: Sun Aug 20 09:13:48 2023, max compression
```

## Comparing `adr_viewer-1.4.0.tar` & `adr-viewer-1.4.0rc1.tar`

### file list

```diff
@@ -1,50 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:30.595960 adr_viewer-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:30.591960 adr_viewer-1.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:30.591960 adr_viewer-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/.github/workflows/pre-merge-checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-21 13:27:30.595960 adr_viewer-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:30.591960 adr_viewer-1.4.0/adr_viewer/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/adr_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/adr_viewer/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/adr_viewer/render.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/adr_viewer/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:30.591960 adr_viewer-1.4.0/adr_viewer/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/adr_viewer/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/adr_viewer/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/adr_viewer/test_render.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:30.595960 adr_viewer-1.4.0/adr_viewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-21 13:27:30.000000 adr_viewer-1.4.0/adr_viewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-21 13:27:30.000000 adr_viewer-1.4.0/adr_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:27:30.000000 adr_viewer-1.4.0/adr_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 13:27:30.000000 adr_viewer-1.4.0/adr_viewer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-21 13:27:30.000000 adr_viewer-1.4.0/adr_viewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 13:27:30.000000 adr_viewer-1.4.0/adr_viewer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:30.587960 adr_viewer-1.4.0/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:30.595960 adr_viewer-1.4.0/doc/adr/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/doc/adr/0001-record-architecture-decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/doc/adr/0002-expose-command-line-interface.md
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/doc/adr/0003-use-same-colour-for-all-headers.md
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/doc/adr/0004-distinguish-superseded-records-with-colour.md
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/doc/adr/0005-distinguish-amendments-to-records-with-colour.md
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/doc/adr/0006-accessibility-as-a-first-class-concern.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:30.595960 adr_viewer-1.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/docs/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:30.595960 adr_viewer-1.4.0/images/
--rw-r--r--   0 runner    (1001) docker     (127)    85272 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/images/example.png
--rw-r--r--   0 runner    (1001) docker     (127)    15055 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/images/record_types.png
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/pa11y.json
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 13:27:30.595960 adr_viewer-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:30.587960 adr_viewer-1.4.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:30.595960 adr_viewer-1.4.0/test/adr/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/test/adr/0001-unknown-status.md
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/test/adr/0002-pending-status.md
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/test/adr/0003-bad-formatting.md
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/test/adr/0004-proposed-status.md
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-21 13:27:19.000000 adr_viewer-1.4.0/test/adr/0005-has-mermaid.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 09:13:48.038475 adr-viewer-1.4.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 09:13:48.026474 adr-viewer-1.4.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 09:13:48.034475 adr-viewer-1.4.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/.github/workflows/pre-merge-checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-08-20 09:13:48.038475 adr-viewer-1.4.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 09:13:48.034475 adr-viewer-1.4.0rc1/adr_viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/adr_viewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 09:13:48.034475 adr-viewer-1.4.0rc1/adr_viewer/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/adr_viewer/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/adr_viewer/test_adr_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 09:13:48.034475 adr-viewer-1.4.0rc1/adr_viewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-08-20 09:13:47.000000 adr-viewer-1.4.0rc1/adr_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-20 09:13:47.000000 adr-viewer-1.4.0rc1/adr_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-20 09:13:47.000000 adr-viewer-1.4.0rc1/adr_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-20 09:13:47.000000 adr-viewer-1.4.0rc1/adr_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-20 09:13:47.000000 adr-viewer-1.4.0rc1/adr_viewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-20 09:13:47.000000 adr-viewer-1.4.0rc1/adr_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 09:13:48.030475 adr-viewer-1.4.0rc1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 09:13:48.038475 adr-viewer-1.4.0rc1/doc/adr/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/doc/adr/0001-record-architecture-decisions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/doc/adr/0002-expose-command-line-interface.md
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/doc/adr/0003-use-same-colour-for-all-headers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/doc/adr/0004-distinguish-superseded-records-with-colour.md
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/doc/adr/0005-distinguish-amendments-to-records-with-colour.md
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/doc/adr/0006-accessibility-as-a-first-class-concern.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 09:13:48.038475 adr-viewer-1.4.0rc1/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    85272 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/images/example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15055 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/images/record_types.png
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/pa11y.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-20 09:13:48.042476 adr-viewer-1.4.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 09:13:48.030475 adr-viewer-1.4.0rc1/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-20 09:13:48.038475 adr-viewer-1.4.0rc1/test/adr/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/test/adr/0001-unknown-status.md
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/test/adr/0002-pending-status.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-20 09:13:35.000000 adr-viewer-1.4.0rc1/test/adr/0003-bad-formatting.md
```

### Comparing `adr_viewer-1.4.0/.github/workflows/pre-merge-checks.yaml` & `adr-viewer-1.4.0rc1/.github/workflows/pre-merge-checks.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -12,31 +12,23 @@
   pre-merge-checks:
     name: Pre-merge checks (Python ${{ matrix.python_version }})
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python_version:
+          - '3.7'
           - '3.8'
           - '3.9'
           - '3.10'
           - '3.11'
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: "${{ matrix.python_version}}"
     - name: Install dependencies
       run: |
         pip install -r requirements.txt
-    - name: Check formatting
-      run: black --check adr_viewer
     - name: Run tests
       run: pytest
-    - name: Run typecheck
-      run: |
-        mypy adr_viewer \
-          --install-types \
-          --non-interactive \
-          --ignore-missing-imports \
-          --pretty
```

### Comparing `adr_viewer-1.4.0/.github/workflows/publish.yml` & `adr-viewer-1.4.0rc1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `adr_viewer-1.4.0/LICENSE` & `adr-viewer-1.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `adr_viewer-1.4.0/PKG-INFO` & `adr-viewer-1.4.0rc1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 Metadata-Version: 2.1
 Name: adr-viewer
-Version: 1.4.0
+Version: 1.4.0rc1
 Summary: A visualisation tool for Architecture Decision Records
 Home-page: https://github.com/mrwilson/adr-viewer
 Author: Alex Wilson
 Author-email: a.wilson@alumni.warwick.ac.uk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: mistune
-Requires-Dist: bs4
-Requires-Dist: jinja2
-Requires-Dist: bottle
 
 # adr-viewer
 
-[![Latest Version](https://img.shields.io/pypi/v/adr-viewer)](https://pypi.org/project/adr-viewer/)
+[![Build Status](https://travis-ci.org/mrwilson/adr-viewer.svg?branch=master)](https://travis-ci.org/mrwilson/adr-viewer)
 
 Show off your Architecture Decision Records with an easy-to-navigate web page, either as a local web-server or generated static content.
-Include diagrams in [Mermaid](https://mermaid.js.org) format using code blocks/fences, e.g. [test ADR 5](test/adr/0005-has-mermaid.md).
 
 ## Examples
 
-<img src="https://github.com/mrwilson/adr-viewer/raw/master/images/example.png" height="500px"/>
+<img src="images/example.png" height="500px"/>
 
 * Example above using Nat Pryce's [adr-tools](https://github.com/npryce/adr-tools) project
 * This project exposes its own Architecture Decision Records [here](https://mrwilson.github.io/adr-viewer/index.html)
 
 ## Installation
 
 ### From PyPI
@@ -75,8 +68,8 @@
   --help           Show this message and exit.
 ```
 
 The default for `--adr-path` is `doc/adr/` because this is the default path generated by `adr-tools`.
 
 ## Supported Record Types
 
-<img src="https://github.com/mrwilson/adr-viewer/raw/master/images/record_types.png"/>
+<img src="images/record_types.png"/>
```

### Comparing `adr_viewer-1.4.0/README.md` & `adr-viewer-1.4.0rc1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # adr-viewer
 
-[![Latest Version](https://img.shields.io/pypi/v/adr-viewer)](https://pypi.org/project/adr-viewer/)
+[![Build Status](https://travis-ci.org/mrwilson/adr-viewer.svg?branch=master)](https://travis-ci.org/mrwilson/adr-viewer)
 
 Show off your Architecture Decision Records with an easy-to-navigate web page, either as a local web-server or generated static content.
-Include diagrams in [Mermaid](https://mermaid.js.org) format using code blocks/fences, e.g. [test ADR 5](test/adr/0005-has-mermaid.md).
 
 ## Examples
 
-<img src="https://github.com/mrwilson/adr-viewer/raw/master/images/example.png" height="500px"/>
+<img src="images/example.png" height="500px"/>
 
 * Example above using Nat Pryce's [adr-tools](https://github.com/npryce/adr-tools) project
 * This project exposes its own Architecture Decision Records [here](https://mrwilson.github.io/adr-viewer/index.html)
 
 ## Installation
 
 ### From PyPI
@@ -52,8 +51,8 @@
   --help           Show this message and exit.
 ```
 
 The default for `--adr-path` is `doc/adr/` because this is the default path generated by `adr-tools`.
 
 ## Supported Record Types
 
-<img src="https://github.com/mrwilson/adr-viewer/raw/master/images/record_types.png"/>
+<img src="images/record_types.png"/>
```

### Comparing `adr_viewer-1.4.0/adr_viewer.egg-info/PKG-INFO` & `adr-viewer-1.4.0rc1/adr_viewer.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 Metadata-Version: 2.1
 Name: adr-viewer
-Version: 1.4.0
+Version: 1.4.0rc1
 Summary: A visualisation tool for Architecture Decision Records
 Home-page: https://github.com/mrwilson/adr-viewer
 Author: Alex Wilson
 Author-email: a.wilson@alumni.warwick.ac.uk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: mistune
-Requires-Dist: bs4
-Requires-Dist: jinja2
-Requires-Dist: bottle
 
 # adr-viewer
 
-[![Latest Version](https://img.shields.io/pypi/v/adr-viewer)](https://pypi.org/project/adr-viewer/)
+[![Build Status](https://travis-ci.org/mrwilson/adr-viewer.svg?branch=master)](https://travis-ci.org/mrwilson/adr-viewer)
 
 Show off your Architecture Decision Records with an easy-to-navigate web page, either as a local web-server or generated static content.
-Include diagrams in [Mermaid](https://mermaid.js.org) format using code blocks/fences, e.g. [test ADR 5](test/adr/0005-has-mermaid.md).
 
 ## Examples
 
-<img src="https://github.com/mrwilson/adr-viewer/raw/master/images/example.png" height="500px"/>
+<img src="images/example.png" height="500px"/>
 
 * Example above using Nat Pryce's [adr-tools](https://github.com/npryce/adr-tools) project
 * This project exposes its own Architecture Decision Records [here](https://mrwilson.github.io/adr-viewer/index.html)
 
 ## Installation
 
 ### From PyPI
@@ -75,8 +68,8 @@
   --help           Show this message and exit.
 ```
 
 The default for `--adr-path` is `doc/adr/` because this is the default path generated by `adr-tools`.
 
 ## Supported Record Types
 
-<img src="https://github.com/mrwilson/adr-viewer/raw/master/images/record_types.png"/>
+<img src="images/record_types.png"/>
```

### Comparing `adr_viewer-1.4.0/adr_viewer.egg-info/SOURCES.txt` & `adr-viewer-1.4.0rc1/adr_viewer.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,28 @@
 .gitignore
 LICENSE
 README.md
 pa11y.json
 requirements.txt
 setup.py
-.github/dependabot.yml
 .github/workflows/pre-merge-checks.yaml
 .github/workflows/publish.yml
 adr_viewer/__init__.py
-adr_viewer/parse.py
-adr_viewer/render.py
-adr_viewer/server.py
-adr_viewer/test_parse.py
-adr_viewer/test_render.py
+adr_viewer/test_adr_viewer.py
 adr_viewer.egg-info/PKG-INFO
 adr_viewer.egg-info/SOURCES.txt
 adr_viewer.egg-info/dependency_links.txt
 adr_viewer.egg-info/entry_points.txt
 adr_viewer.egg-info/requires.txt
 adr_viewer.egg-info/top_level.txt
 adr_viewer/templates/index.html
 doc/adr/0001-record-architecture-decisions.md
 doc/adr/0002-expose-command-line-interface.md
 doc/adr/0003-use-same-colour-for-all-headers.md
 doc/adr/0004-distinguish-superseded-records-with-colour.md
 doc/adr/0005-distinguish-amendments-to-records-with-colour.md
 doc/adr/0006-accessibility-as-a-first-class-concern.md
-docs/index.html
 images/example.png
 images/record_types.png
 test/adr/0001-unknown-status.md
 test/adr/0002-pending-status.md
-test/adr/0003-bad-formatting.md
-test/adr/0004-proposed-status.md
-test/adr/0005-has-mermaid.md
+test/adr/0003-bad-formatting.md
```

### Comparing `adr_viewer-1.4.0/doc/adr/0002-expose-command-line-interface.md` & `adr-viewer-1.4.0rc1/doc/adr/0002-expose-command-line-interface.md`

 * *Files identical despite different names*

### Comparing `adr_viewer-1.4.0/doc/adr/0004-distinguish-superseded-records-with-colour.md` & `adr-viewer-1.4.0rc1/doc/adr/0004-distinguish-superseded-records-with-colour.md`

 * *Files identical despite different names*

### Comparing `adr_viewer-1.4.0/doc/adr/0005-distinguish-amendments-to-records-with-colour.md` & `adr-viewer-1.4.0rc1/doc/adr/0005-distinguish-amendments-to-records-with-colour.md`

 * *Files identical despite different names*

### Comparing `adr_viewer-1.4.0/doc/adr/0006-accessibility-as-a-first-class-concern.md` & `adr-viewer-1.4.0rc1/doc/adr/0006-accessibility-as-a-first-class-concern.md`

 * *Files identical despite different names*

### Comparing `adr_viewer-1.4.0/images/example.png` & `adr-viewer-1.4.0rc1/images/example.png`

 * *Files identical despite different names*

### Comparing `adr_viewer-1.4.0/images/record_types.png` & `adr-viewer-1.4.0rc1/images/record_types.png`

 * *Files identical despite different names*

### Comparing `adr_viewer-1.4.0/setup.py` & `adr-viewer-1.4.0rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     entry_points={
         'console_scripts': ['adr-viewer=adr_viewer:main']
     },
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Topic :: Software Development',
         'Topic :: Software Development :: Documentation',
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
     ],
     use_scm_version=True,
     setup_requires=["setuptools_scm"],
 )
```


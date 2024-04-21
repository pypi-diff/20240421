# Comparing `tmp/blastpipe-2024.0.4.tar.gz` & `tmp/blastpipe-2024.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blastpipe-2024.0.4.tar", last modified: Sat Apr 13 18:59:40 2024, max compression
+gzip compressed data, was "blastpipe-2024.0.5.tar", last modified: Sun Apr 21 17:42:48 2024, max compression
```

## Comparing `blastpipe-2024.0.4.tar` & `blastpipe-2024.0.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:59:40.217923 blastpipe-2024.0.4/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     2889 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     5869 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.github/workflows/ozi.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3061 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.github/workflows/scorecards.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.pre-commit-config.yaml
--rw-rw-r--   0 runner    (1001) docker     (127)    69217 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/LICENSE.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-13 18:59:40.217923 blastpipe-2024.0.4/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/README.rst
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/
--rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/__init__.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/backports.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/buffer.py
--rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/buffer.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/loop.py
--rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/loop.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/malloc.py
--rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/malloc.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1235 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/mixin.py
--rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/mixin.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/sequence.py
--rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/sequence.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/tailcall.py
--rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/tailcall.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3175 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     8329 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/LICENSE.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/_static/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/_static/css/
--rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/_static/css/custom.css
--rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/_static/css/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/_static/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/_templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/_templates/layout.html
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/_templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/conf.cfg
--rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/index.rst
--rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      122 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/ozi.wrap
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/tests/test_backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/tests/test_fuzz.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/tests/test_tailcall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:42:48.214041 blastpipe-2024.0.5/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5869 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.github/workflows/ozi.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.github/workflows/scorecards.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.pre-commit-config.yaml
+-rw-rw-r--   0 runner    (1001) docker     (127)    74141 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/LICENSE.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-21 17:42:48.214041 blastpipe-2024.0.5/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/README.rst
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/__init__.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/backports.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/buffer.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/buffer.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/loop.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/loop.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/malloc.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/malloc.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1235 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/mixin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/mixin.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/sequence.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/sequence.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/tailcall.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/tailcall.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3175 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     8329 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/LICENSE.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/_static/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/_static/css/
+-rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/_static/css/custom.css
+-rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/_static/css/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/_static/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/_templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/_templates/layout.html
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/_templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/conf.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/index.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      122 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/ozi.wrap
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/tests/test_backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/tests/test_fuzz.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/tests/test_tailcall.py
```

### Comparing `blastpipe-2024.0.4/.github/workflows/codeql.yml` & `blastpipe-2024.0.5/.github/workflows/codeql.yml`

 * *Files 14% similar despite different names*

```diff
@@ -42,37 +42,37 @@
     steps:
       - name: Harden Runner
         uses: step-security/harden-runner@63c24ba6bd7ba022e95695ff85de572c04a18142 # v2.7.0
         with:
           egress-policy: audit
 
       - name: Checkout repository
-        uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
+        uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f # v4.1.3
 
       # Initializes the CodeQL tools for scanning.
       - name: Initialize CodeQL
-        uses: github/codeql-action/init@4355270be187e1b672a7a1c7c7bae5afdc1ab94a # v3.24.10
+        uses: github/codeql-action/init@c7f9125735019aa87cfc361530512d50ea439c71 # v3.25.1
         with:
           languages: ${{ matrix.language }}
           # If you wish to specify custom queries, you can do so here or in a config file.
           # By default, queries listed here will override any specified in a config file.
           # Prefix the list here with "+" to use these queries and those in the config file.
 
       # Autobuild attempts to build any compiled languages  (C/C++, C#, or Java).
       # If this step fails, then you should remove it and run the build manually (see below)
       - name: Autobuild
-        uses: github/codeql-action/autobuild@4355270be187e1b672a7a1c7c7bae5afdc1ab94a # v3.24.10
+        uses: github/codeql-action/autobuild@c7f9125735019aa87cfc361530512d50ea439c71 # v3.25.1
 
       # ℹ️ Command-line programs to run using the OS shell.
       # 📚 See https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idstepsrun
 
       #   If the Autobuild fails above, remove it and uncomment the following three lines.
       #   modify them (or add more) to build your code if your project, please refer to the EXAMPLE below for guidance.
 
       # - run: |
       #   echo "Run, Build Application using script"
       #   ./location_of_script_within_repo/buildscript.sh
 
       - name: Perform CodeQL Analysis
-        uses: github/codeql-action/analyze@4355270be187e1b672a7a1c7c7bae5afdc1ab94a # v3.24.10
+        uses: github/codeql-action/analyze@c7f9125735019aa87cfc361530512d50ea439c71 # v3.25.1
         with:
           category: "/language:${{matrix.language}}"
```

### Comparing `blastpipe-2024.0.4/.github/workflows/dependency-review.yml` & `blastpipe-2024.0.5/.github/workflows/dependency-review.yml`

 * *Files 27% similar despite different names*

```diff
@@ -18,10 +18,10 @@
     steps:
       - name: Harden Runner
         uses: step-security/harden-runner@63c24ba6bd7ba022e95695ff85de572c04a18142 # v2.7.0
         with:
           egress-policy: audit
 
       - name: 'Checkout Repository'
-        uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
+        uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f # v4.1.3
       - name: 'Dependency Review'
         uses: actions/dependency-review-action@5bbc3ba658137598168acb2ab73b21c432dd411b # v4.2.5
```

### Comparing `blastpipe-2024.0.4/.github/workflows/ozi.yml` & `blastpipe-2024.0.5/.github/workflows/ozi.yml`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             pypi.org:443
             registry.npmjs.org:443
             objects.githubusercontent.com:443
             fulcio.sigstore.dev:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/checkpoint@91c27e2c333d718d7b87992e19511ff5b00cd16e
+      - uses: OZI-Project/checkpoint@8b7d897024b918d4bb4d44bbaec23a22f357182e
         with:
           python-version: "3.10"
 
   checkpoint-cp311-ubuntu-latest:
     name: checkpoint (Python 3.11 on ubuntu-latest)
     runs-on: ubuntu-latest
     strategy:
@@ -62,15 +62,15 @@
             pypi.org:443
             registry.npmjs.org:443
             objects.githubusercontent.com:443
             fulcio.sigstore.dev:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/checkpoint@91c27e2c333d718d7b87992e19511ff5b00cd16e
+      - uses: OZI-Project/checkpoint@8b7d897024b918d4bb4d44bbaec23a22f357182e
         with:
           python-version: "3.11"
 
   checkpoint-cp312-ubuntu-latest:
     name: checkpoint (Python 3.12 on ubuntu-latest)
     runs-on: ubuntu-latest
     strategy:
@@ -90,15 +90,15 @@
             pypi.org:443
             registry.npmjs.org:443
             objects.githubusercontent.com:443
             fulcio.sigstore.dev:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/checkpoint@91c27e2c333d718d7b87992e19511ff5b00cd16e
+      - uses: OZI-Project/checkpoint@8b7d897024b918d4bb4d44bbaec23a22f357182e
         with:
           python-version: "3.12"
 
   checkpoint:
     runs-on: ubuntu-latest
     needs: [checkpoint-cp310-ubuntu-latest, checkpoint-cp311-ubuntu-latest, checkpoint-cp312-ubuntu-latest]
     steps:
@@ -138,15 +138,15 @@
             files.pythonhosted.org:443
             fulcio.sigstore.dev:443
             github.com:443
             pypi.org:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/release@945b312031019d0d85c5674721327f894131d898
+      - uses: OZI-Project/release@f0e0a8b837c2d247b920fbc1997a8d3247b14455
         id: release
         with:
           python-dist: ${{ matrix.py }}
           github-token: ${{ secrets.GITHUB_TOKEN }}
 
   generate-provenance:
     needs: [release, checkpoint]
```

### Comparing `blastpipe-2024.0.4/.github/workflows/scorecards.yml` & `blastpipe-2024.0.5/.github/workflows/scorecards.yml`

 * *Files 11% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     steps:
       - name: Harden Runner
         uses: step-security/harden-runner@63c24ba6bd7ba022e95695ff85de572c04a18142 # v2.7.0
         with:
           egress-policy: audit
 
       - name: "Checkout code"
-        uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
+        uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f # v4.1.3
         with:
           persist-credentials: false
 
       - name: "Run analysis"
         uses: ossf/scorecard-action@0864cf19026789058feabb7e87baa5f140aac736 # v2.3.1
         with:
           results_file: results.sarif
@@ -59,18 +59,18 @@
           #   - `publish_results` will always be set to `false`, regardless
           #     of the value entered here.
           publish_results: true
 
       # Upload the results as artifacts (optional). Commenting out will disable uploads of run results in SARIF
       # format to the repository Actions tab.
       - name: "Upload artifact"
-        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # v4.3.1
+        uses: actions/upload-artifact@1746f4ab65b179e0ea60a494b83293b640dd5bba # v4.3.2
         with:
           name: SARIF file
           path: results.sarif
           retention-days: 5
 
       # Upload the results to GitHub's code scanning dashboard.
       - name: "Upload to code-scanning"
-        uses: github/codeql-action/upload-sarif@4355270be187e1b672a7a1c7c7bae5afdc1ab94a # v3.24.10
+        uses: github/codeql-action/upload-sarif@c7f9125735019aa87cfc361530512d50ea439c71 # v3.25.1
         with:
           sarif_file: results.sarif
```

### Comparing `blastpipe-2024.0.4/.gitignore` & `blastpipe-2024.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/CHANGELOG.md` & `blastpipe-2024.0.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,117 @@
 # CHANGELOG
 
 
 
+## v2024.0.5 (2024-04-21)
+
+### :arrow_up:
+
+* :arrow_up: Bump actions/checkout from 4.1.1 to 4.1.3
+
+Bumps [actions/checkout](https://github.com/actions/checkout) from 4.1.1 to 4.1.3.
+- [Release notes](https://github.com/actions/checkout/releases)
+- [Changelog](https://github.com/actions/checkout/blob/main/CHANGELOG.md)
+- [Commits](https://github.com/actions/checkout/compare/b4ffde65f46336ab88eb53be808477a3936bae11...1d96c772d19495a3b5c517cd2bc0cb401ea0529f)
+
+---
+updated-dependencies:
+- dependency-name: actions/checkout
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`a2f8815`](https://github.com/OZI-Project/blastpipe/commit/a2f88158906517d20dacc8335282408e6d798edf))
+
+* :arrow_up: Bump actions/upload-artifact from 4.3.1 to 4.3.2
+
+Bumps [actions/upload-artifact](https://github.com/actions/upload-artifact) from 4.3.1 to 4.3.2.
+- [Release notes](https://github.com/actions/upload-artifact/releases)
+- [Commits](https://github.com/actions/upload-artifact/compare/5d5d22a31266ced268874388b861e4b58bb5c2f3...1746f4ab65b179e0ea60a494b83293b640dd5bba)
+
+---
+updated-dependencies:
+- dependency-name: actions/upload-artifact
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`d0f9d7a`](https://github.com/OZI-Project/blastpipe/commit/d0f9d7a79a8699f017dc9861f5b696b84a502b08))
+
+* :arrow_up: Bump github/codeql-action from 3.24.10 to 3.25.1
+
+Bumps [github/codeql-action](https://github.com/github/codeql-action) from 3.24.10 to 3.25.1.
+- [Release notes](https://github.com/github/codeql-action/releases)
+- [Changelog](https://github.com/github/codeql-action/blob/main/CHANGELOG.md)
+- [Commits](https://github.com/github/codeql-action/compare/4355270be187e1b672a7a1c7c7bae5afdc1ab94a...c7f9125735019aa87cfc361530512d50ea439c71)
+
+---
+updated-dependencies:
+- dependency-name: github/codeql-action
+  dependency-type: direct:production
+  update-type: version-update:semver-minor
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`fbe5c3b`](https://github.com/OZI-Project/blastpipe/commit/fbe5c3bac753b872c21c837a3085170534bc6b35))
+
+* :arrow_up: Bump OZI-Project/checkpoint from 0.1.3 to 0.1.4
+
+Bumps [OZI-Project/checkpoint](https://github.com/ozi-project/checkpoint) from 0.1.3 to 0.1.4.
+- [Release notes](https://github.com/ozi-project/checkpoint/releases)
+- [Commits](https://github.com/ozi-project/checkpoint/compare/91c27e2c333d718d7b87992e19511ff5b00cd16e...8b7d897024b918d4bb4d44bbaec23a22f357182e)
+
+---
+updated-dependencies:
+- dependency-name: OZI-Project/checkpoint
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`f573e1e`](https://github.com/OZI-Project/blastpipe/commit/f573e1e75dbfe0cd18fab98e51c2e44b66188257))
+
+* :arrow_up: Bump OZI-Project/release from 0.1.14 to 0.1.15
+
+Bumps [OZI-Project/release](https://github.com/ozi-project/release) from 0.1.14 to 0.1.15.
+- [Release notes](https://github.com/ozi-project/release/releases)
+- [Commits](https://github.com/ozi-project/release/compare/945b312031019d0d85c5674721327f894131d898...f0e0a8b837c2d247b920fbc1997a8d3247b14455)
+
+---
+updated-dependencies:
+- dependency-name: OZI-Project/release
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`6528401`](https://github.com/OZI-Project/blastpipe/commit/6528401f75d5f68228734c2787d43c9c439aa884))
+
+### :pushpin:
+
+* :pushpin: Merge pull request #57 from OZI-Project/dependabot/github_actions/OZI-Project/release-0.1.15
+
+⬆️ Bump OZI-Project/release from 0.1.14 to 0.1.15 ([`d809c35`](https://github.com/OZI-Project/blastpipe/commit/d809c3577aa3a0f0160bf682a9fcf6a03b5392cf))
+
+* :pushpin: Merge pull request #58 from OZI-Project/dependabot/github_actions/OZI-Project/checkpoint-0.1.4
+
+⬆️ Bump OZI-Project/checkpoint from 0.1.3 to 0.1.4 ([`b04d131`](https://github.com/OZI-Project/blastpipe/commit/b04d1312f8e331c16bef78ef1f53ed3b2f4aa978))
+
+### Other
+
+* Merge pull request #61 from OZI-Project/dependabot/github_actions/actions/checkout-4.1.3
+
+⬆️ Bump actions/checkout from 4.1.1 to 4.1.3 ([`1658a31`](https://github.com/OZI-Project/blastpipe/commit/1658a3150da171997cebf378cf33c1b1f067cab7))
+
+* Merge pull request #60 from OZI-Project/dependabot/github_actions/actions/upload-artifact-4.3.2
+
+⬆️ Bump actions/upload-artifact from 4.3.1 to 4.3.2 ([`4f99092`](https://github.com/OZI-Project/blastpipe/commit/4f99092b91a88b9066417ab393b07a5cca79101d))
+
+* Merge pull request #59 from OZI-Project/dependabot/github_actions/github/codeql-action-3.25.1
+
+⬆️ Bump github/codeql-action from 3.24.10 to 3.25.1 ([`f381c15`](https://github.com/OZI-Project/blastpipe/commit/f381c15a9d1efa16d441fabaaca0db3963262cfb))
+
+
 ## v2024.0.4 (2024-04-13)
 
 ### :arrow_up:
 
 * :arrow_up: Bump OZI-Project/release from 0.1.13 to 0.1.14
 
 Bumps [OZI-Project/release](https://github.com/ozi-project/release) from 0.1.13 to 0.1.14.
```

### Comparing `blastpipe-2024.0.4/LICENSE.txt` & `blastpipe-2024.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/NOTICE.md` & `blastpipe-2024.0.5/NOTICE.md`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/PKG-INFO` & `blastpipe-2024.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: blastpipe
-Version: 2024.0.4
+Version: 2024.0.5
 Summary: OZI integrated test library.
 Home-page: https://oziproject.dev
 Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
-Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.0.4.tar.gz
+Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.0.5.tar.gz
 Requires-Python: >=3.10, <3.13
 Keywords: ozi,meson
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `blastpipe-2024.0.4/README.rst` & `blastpipe-2024.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/blastpipe/__init__.py` & `blastpipe-2024.0.5/blastpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/blastpipe/backports.py` & `blastpipe-2024.0.5/blastpipe/backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/blastpipe/backports.pyi` & `blastpipe-2024.0.5/blastpipe/backports.pyi`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/blastpipe/buffer.py` & `blastpipe-2024.0.5/blastpipe/buffer.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/blastpipe/loop.py` & `blastpipe-2024.0.5/blastpipe/loop.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/blastpipe/malloc.py` & `blastpipe-2024.0.5/blastpipe/malloc.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/blastpipe/meson.build` & `blastpipe-2024.0.5/blastpipe/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/blastpipe/mixin.py` & `blastpipe-2024.0.5/blastpipe/mixin.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/blastpipe/sequence.py` & `blastpipe-2024.0.5/blastpipe/sequence.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/blastpipe/tailcall.py` & `blastpipe-2024.0.5/blastpipe/tailcall.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/meson.build` & `blastpipe-2024.0.5/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/meson.options` & `blastpipe-2024.0.5/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/pyproject.toml` & `blastpipe-2024.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/subprojects/docs/LICENSE.txt` & `blastpipe-2024.0.5/subprojects/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/subprojects/docs/_static/css/custom.css` & `blastpipe-2024.0.5/subprojects/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/subprojects/docs/_static/css/meson.build` & `blastpipe-2024.0.5/subprojects/docs/_static/css/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/subprojects/docs/_static/meson.build` & `blastpipe-2024.0.5/subprojects/docs/_static/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/subprojects/docs/_templates/layout.html` & `blastpipe-2024.0.5/subprojects/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/subprojects/docs/_templates/meson.build` & `blastpipe-2024.0.5/subprojects/docs/_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/subprojects/docs/conf.cfg` & `blastpipe-2024.0.5/subprojects/docs/conf.cfg`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/subprojects/docs/index.rst` & `blastpipe-2024.0.5/subprojects/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/subprojects/docs/meson.build` & `blastpipe-2024.0.5/subprojects/docs/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/subprojects/docs/meson.options` & `blastpipe-2024.0.5/subprojects/docs/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/tests/meson.build` & `blastpipe-2024.0.5/tests/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/tests/test_backports.py` & `blastpipe-2024.0.5/tests/test_backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/tests/test_fuzz.py` & `blastpipe-2024.0.5/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.4/tests/test_tailcall.py` & `blastpipe-2024.0.5/tests/test_tailcall.py`

 * *Files identical despite different names*


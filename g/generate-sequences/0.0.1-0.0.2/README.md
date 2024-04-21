# Comparing `tmp/generate_sequences-0.0.1.tar.gz` & `tmp/generate_sequences-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generate_sequences-0.0.1.tar", last modified: Thu Apr 18 14:46:18 2024, max compression
+gzip compressed data, was "generate_sequences-0.0.2.tar", last modified: Sun Apr 21 10:07:17 2024, max compression
```

## Comparing `generate_sequences-0.0.1.tar` & `generate_sequences-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:18.988746 generate_sequences-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-18 14:43:56.000000 generate_sequences-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-04-18 14:46:18.988746 generate_sequences-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 14:43:56.000000 generate_sequences-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:18.984746 generate_sequences-0.0.1/generate_sequences/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-18 14:43:56.000000 generate_sequences-0.0.1/generate_sequences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-18 14:43:56.000000 generate_sequences-0.0.1/generate_sequences/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:43:56.000000 generate_sequences-0.0.1/generate_sequences/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 14:43:56.000000 generate_sequences-0.0.1/generate_sequences/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:46:18.984746 generate_sequences-0.0.1/generate_sequences.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-04-18 14:46:18.000000 generate_sequences-0.0.1/generate_sequences.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-18 14:46:18.000000 generate_sequences-0.0.1/generate_sequences.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:46:18.000000 generate_sequences-0.0.1/generate_sequences.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-18 14:46:18.000000 generate_sequences-0.0.1/generate_sequences.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 14:46:18.000000 generate_sequences-0.0.1/generate_sequences.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-18 14:43:56.000000 generate_sequences-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:46:18.988746 generate_sequences-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:07:17.954053 generate_sequences-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-21 10:03:34.000000 generate_sequences-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-04-21 10:07:17.954053 generate_sequences-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-21 10:03:34.000000 generate_sequences-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:07:17.950053 generate_sequences-0.0.2/generate_sequences/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-21 10:03:34.000000 generate_sequences-0.0.2/generate_sequences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9791 2024-04-21 10:03:34.000000 generate_sequences-0.0.2/generate_sequences/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:03:34.000000 generate_sequences-0.0.2/generate_sequences/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-21 10:03:34.000000 generate_sequences-0.0.2/generate_sequences/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:07:17.950053 generate_sequences-0.0.2/generate_sequences.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-04-21 10:07:17.000000 generate_sequences-0.0.2/generate_sequences.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-21 10:07:17.000000 generate_sequences-0.0.2/generate_sequences.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 10:07:17.000000 generate_sequences-0.0.2/generate_sequences.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-21 10:07:17.000000 generate_sequences-0.0.2/generate_sequences.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-21 10:07:17.000000 generate_sequences-0.0.2/generate_sequences.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-21 10:03:34.000000 generate_sequences-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 10:07:17.954053 generate_sequences-0.0.2/setup.cfg
```

### Comparing `generate_sequences-0.0.1/LICENSE` & `generate_sequences-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `generate_sequences-0.0.1/PKG-INFO` & `generate_sequences-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-sequences
-Version: 0.0.1
+Version: 0.0.2
 Author-email: "Maged S. Al-Shaibani" <mageedsaeed1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -226,22 +226,22 @@
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine>=1.11.0; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
-Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev"
+Requires-Dist: Sphinx<7.4.0,>=4.3.0; extra == "dev"
 Requires-Dist: furo==2024.1.29; extra == "dev"
 Requires-Dist: myst-parser<2.1,>=1.0; extra == "dev"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints==2.0.0; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
 Requires-Dist: pre-commit==3.5.0; extra == "dev"
 Requires-Dist: evaluate==0.4.*; extra == "dev"
 Requires-Dist: sacrebleu==2.4.*; extra == "dev"
 Requires-Dist: sacremoses==0.1.*; extra == "dev"
 Requires-Dist: sentencepiece==0.2.*; extra == "dev"
-Requires-Dist: transformers==4.39.*; extra == "dev"
+Requires-Dist: transformers<4.41,>=4.39; extra == "dev"
 
 # generate-sequences
```

### Comparing `generate_sequences-0.0.1/generate_sequences.egg-info/PKG-INFO` & `generate_sequences-0.0.2/generate_sequences.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-sequences
-Version: 0.0.1
+Version: 0.0.2
 Author-email: "Maged S. Al-Shaibani" <mageedsaeed1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -226,22 +226,22 @@
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine>=1.11.0; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
-Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev"
+Requires-Dist: Sphinx<7.4.0,>=4.3.0; extra == "dev"
 Requires-Dist: furo==2024.1.29; extra == "dev"
 Requires-Dist: myst-parser<2.1,>=1.0; extra == "dev"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints==2.0.0; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
 Requires-Dist: pre-commit==3.5.0; extra == "dev"
 Requires-Dist: evaluate==0.4.*; extra == "dev"
 Requires-Dist: sacrebleu==2.4.*; extra == "dev"
 Requires-Dist: sacremoses==0.1.*; extra == "dev"
 Requires-Dist: sentencepiece==0.2.*; extra == "dev"
-Requires-Dist: transformers==4.39.*; extra == "dev"
+Requires-Dist: transformers<4.41,>=4.39; extra == "dev"
 
 # generate-sequences
```

### Comparing `generate_sequences-0.0.1/pyproject.toml` & `generate_sequences-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -39,28 +39,28 @@
   "pytest",
   "pytest-sphinx",
   "pytest-cov",
   "twine>=1.11.0",
   "build",
   "setuptools",
   "wheel",
-  "Sphinx>=4.3.0,<7.3.0",
+  "Sphinx>=4.3.0,<7.4.0",
   "furo==2024.1.29",
   "myst-parser>=1.0,<2.1",
   "sphinx-copybutton==0.5.2",
   "sphinx-autobuild==2021.3.14",
   "sphinx-autodoc-typehints==2.0.0",
   "packaging",
   "pre-commit==3.5.0",
   # added for testing
   "evaluate==0.4.*",
   "sacrebleu==2.4.*",
   "sacremoses==0.1.*",
   "sentencepiece==0.2.*",
-  "transformers==4.39.*",
+  "transformers>=4.39,<4.41",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["*.tests", "*.tests.*", "tests.*", "tests", "docs*", "scripts*"]
 
 [tool.setuptools]
 include-package-data = true
```


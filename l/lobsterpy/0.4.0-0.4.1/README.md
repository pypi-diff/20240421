# Comparing `tmp/lobsterpy-0.4.0.tar.gz` & `tmp/lobsterpy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lobsterpy-0.4.0.tar", last modified: Tue Mar 12 17:00:05 2024, max compression
+gzip compressed data, was "lobsterpy-0.4.1.tar", last modified: Sun Apr 21 14:27:01 2024, max compression
```

## Comparing `lobsterpy-0.4.0.tar` & `lobsterpy-0.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:00:05.576331 lobsterpy-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-12 16:59:10.000000 lobsterpy-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-03-12 17:00:05.576331 lobsterpy-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-03-12 16:59:10.000000 lobsterpy-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:00:05.572331 lobsterpy-0.4.0/lobsterpy/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-12 16:59:11.000000 lobsterpy-0.4.0/lobsterpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42392 2024-03-12 16:59:11.000000 lobsterpy-0.4.0/lobsterpy/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:00:05.572331 lobsterpy-0.4.0/lobsterpy/cohp/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-12 16:59:11.000000 lobsterpy-0.4.0/lobsterpy/cohp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    78176 2024-03-12 16:59:11.000000 lobsterpy-0.4.0/lobsterpy/cohp/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)    37449 2024-03-12 16:59:11.000000 lobsterpy-0.4.0/lobsterpy/cohp/describe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:00:05.572331 lobsterpy-0.4.0/lobsterpy/featurize/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-12 16:59:11.000000 lobsterpy-0.4.0/lobsterpy/featurize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32633 2024-03-12 16:59:11.000000 lobsterpy-0.4.0/lobsterpy/featurize/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    47979 2024-03-12 16:59:11.000000 lobsterpy-0.4.0/lobsterpy/featurize/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-03-12 16:59:11.000000 lobsterpy-0.4.0/lobsterpy/featurize/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:00:05.572331 lobsterpy-0.4.0/lobsterpy/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)    47583 2024-03-12 16:59:11.000000 lobsterpy-0.4.0/lobsterpy/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-03-12 16:59:11.000000 lobsterpy-0.4.0/lobsterpy/plotting/layout_dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-12 16:59:11.000000 lobsterpy-0.4.0/lobsterpy/plotting/lobsterpy_base.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:00:05.572331 lobsterpy-0.4.0/lobsterpy/structuregraph/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-12 16:59:11.000000 lobsterpy-0.4.0/lobsterpy/structuregraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-03-12 16:59:11.000000 lobsterpy-0.4.0/lobsterpy/structuregraph/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:00:05.572331 lobsterpy-0.4.0/lobsterpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-03-12 17:00:05.000000 lobsterpy-0.4.0/lobsterpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-12 17:00:05.000000 lobsterpy-0.4.0/lobsterpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 17:00:05.000000 lobsterpy-0.4.0/lobsterpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-12 17:00:05.000000 lobsterpy-0.4.0/lobsterpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-12 17:00:05.000000 lobsterpy-0.4.0/lobsterpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-12 17:00:05.000000 lobsterpy-0.4.0/lobsterpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-03-12 16:59:11.000000 lobsterpy-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 17:00:05.576331 lobsterpy-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:27:01.677927 lobsterpy-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-21 14:26:02.000000 lobsterpy-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9771 2024-04-21 14:27:01.677927 lobsterpy-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-21 14:26:02.000000 lobsterpy-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:27:01.673927 lobsterpy-0.4.1/lobsterpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-21 14:26:02.000000 lobsterpy-0.4.1/lobsterpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41947 2024-04-21 14:26:02.000000 lobsterpy-0.4.1/lobsterpy/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:27:01.673927 lobsterpy-0.4.1/lobsterpy/cohp/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-21 14:26:02.000000 lobsterpy-0.4.1/lobsterpy/cohp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78180 2024-04-21 14:26:02.000000 lobsterpy-0.4.1/lobsterpy/cohp/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37915 2024-04-21 14:26:02.000000 lobsterpy-0.4.1/lobsterpy/cohp/describe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:27:01.677927 lobsterpy-0.4.1/lobsterpy/featurize/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-21 14:26:02.000000 lobsterpy-0.4.1/lobsterpy/featurize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32633 2024-04-21 14:26:02.000000 lobsterpy-0.4.1/lobsterpy/featurize/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47979 2024-04-21 14:26:02.000000 lobsterpy-0.4.1/lobsterpy/featurize/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-21 14:26:02.000000 lobsterpy-0.4.1/lobsterpy/featurize/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:27:01.677927 lobsterpy-0.4.1/lobsterpy/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)    47583 2024-04-21 14:26:02.000000 lobsterpy-0.4.1/lobsterpy/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-21 14:26:02.000000 lobsterpy-0.4.1/lobsterpy/plotting/layout_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-21 14:26:02.000000 lobsterpy-0.4.1/lobsterpy/plotting/lobsterpy_base.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:27:01.677927 lobsterpy-0.4.1/lobsterpy/structuregraph/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-21 14:26:02.000000 lobsterpy-0.4.1/lobsterpy/structuregraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-04-21 14:26:02.000000 lobsterpy-0.4.1/lobsterpy/structuregraph/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:27:01.677927 lobsterpy-0.4.1/lobsterpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9771 2024-04-21 14:27:01.000000 lobsterpy-0.4.1/lobsterpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-21 14:27:01.000000 lobsterpy-0.4.1/lobsterpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 14:27:01.000000 lobsterpy-0.4.1/lobsterpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-21 14:27:01.000000 lobsterpy-0.4.1/lobsterpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-21 14:27:01.000000 lobsterpy-0.4.1/lobsterpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 14:27:01.000000 lobsterpy-0.4.1/lobsterpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-04-21 14:26:02.000000 lobsterpy-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 14:27:01.677927 lobsterpy-0.4.1/setup.cfg
```

### Comparing `lobsterpy-0.4.0/LICENSE` & `lobsterpy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.0/PKG-INFO` & `lobsterpy-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lobsterpy
-Version: 0.4.0
+Version: 0.4.1
 Summary: Package for automatic bonding analysis with Lobster/VASP
 Author-email: Janine George <janine.george@bam.de>
 License: BSD 3-Clause
 Project-URL: homepage, https://jageo.github.io/LobsterPy/
 Project-URL: repository, https://github.com/JaGeo/LobsterPy
 Project-URL: documentation, https://jageo.github.io/LobsterPy/
 Project-URL: changelog, https://jageo.github.io/LobsterPy/about/changelog.html
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pymatgen>=2024.2.23
+Requires-Dist: pymatgen>=2024.4.13
 Requires-Dist: numpy
 Requires-Dist: typing
 Provides-Extra: featurizer
 Requires-Dist: mendeleev==0.15.0; extra == "featurizer"
 Provides-Extra: dev
 Requires-Dist: pre-commit>=2.12.1; extra == "dev"
 Provides-Extra: tests
@@ -32,21 +32,20 @@
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: pytest-split; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinx<6,>=5; extra == "docs"
 Requires-Dist: sphinx_design==0.5.0; extra == "docs"
-Requires-Dist: myst-nb==1.0.0; extra == "docs"
+Requires-Dist: myst-nb==1.1.0; extra == "docs"
 Requires-Dist: sphinx-book-theme==1.1.2; extra == "docs"
 Requires-Dist: sphinx-argparse==0.4.0; extra == "docs"
 Requires-Dist: sphinx-toolbox==3.5.0; extra == "docs"
 
-![CI Status](https://github.com/JaGeo/LobsterPy/actions/workflows/python-package.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/JaGeo/LobsterPy/main.svg)](https://results.pre-commit.ci/latest/github/JaGeo/LobsterPy/main) [![codecov](https://codecov.io/gh/JaGeo/LobsterPy/graph/badge.svg?token=MC5BRXVEGW)](https://codecov.io/gh/JaGeo/LobsterPy) [![build-docs](https://github.com/JaGeo/LobsterPy/actions/workflows/docs.yml/badge.svg)](https://jageo.github.io/LobsterPy/) [![PyPI version](https://badge.fury.io/py/lobsterpy.svg)](https://badge.fury.io/py/lobsterpy) [![PyPI downloads](https://img.shields.io/pypi/dm/lobsterpy?style=flat&color=blue&label=pypi%20downloads)](https://pypi.org/project/lobsterpy) [![Downloads](https://pepy.tech/badge/lobsterpy)](https://pepy.tech/project/lobsterpy) [![DOI](https://zenodo.org/badge/343384088.svg)](https://zenodo.org/badge/latestdoi/343384088) [![status](https://joss.theoj.org/papers/4e8524125e36486c65a4b435bbfe2df2/status.svg)](https://joss.theoj.org/papers/4e8524125e36486c65a4b435bbfe2df2)
-
+![CI Status](https://github.com/JaGeo/LobsterPy/actions/workflows/python-package.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/JaGeo/LobsterPy/main.svg)](https://results.pre-commit.ci/latest/github/JaGeo/LobsterPy/main) [![codecov](https://codecov.io/gh/JaGeo/LobsterPy/graph/badge.svg?token=MC5BRXVEGW)](https://codecov.io/gh/JaGeo/LobsterPy) [![build-docs](https://github.com/JaGeo/LobsterPy/actions/workflows/docs.yml/badge.svg)](https://jageo.github.io/LobsterPy/) [![PyPI version](https://badge.fury.io/py/lobsterpy.svg)](https://badge.fury.io/py/lobsterpy) [![PyPI downloads](https://img.shields.io/pypi/dm/lobsterpy?style=flat&color=blue&label=pypi%20downloads)](https://pypi.org/project/lobsterpy) [![Downloads](https://pepy.tech/badge/lobsterpy)](https://pepy.tech/project/lobsterpy) ![supported python versions](https://img.shields.io/pypi/pyversions/lobsterpy) [![DOI](https://zenodo.org/badge/343384088.svg)](https://zenodo.org/badge/latestdoi/343384088) [![status](https://joss.theoj.org/papers/4e8524125e36486c65a4b435bbfe2df2/status.svg)](https://joss.theoj.org/papers/4e8524125e36486c65a4b435bbfe2df2)
 # Getting started
 <img src="https://raw.githubusercontent.com/JaGeo/LobsterPy/main/LobsterPyLogo.png" alt="LobsterPy Logo which consists of a green Python and a red Lobster" width="200"/>
 
 LobsterPy is a package that enables automatic analysis of LOBSTER outputs to get summarized bonding information and relevant bond plots. Additionally, one can also generate features for machine learning studies from LOBSTER outputs. One can download LOBSTER from [http://www.cohp.de](http://www.cohp.de).
 
 <div style="border: 1px solid #52a5ab; padding: 5px; position: relative;">
     <div style="background-color: #52a5ab; color: #ffffff; padding: 0px; position: absolute; top: 0; left: 0; right: 0; text-align: center;">
@@ -61,14 +60,18 @@
 
 Please note that LobsterPy relies on the LOBSTER computation output files. Thus, it will be only able to analyze data that has been computed in the LOBSTER run.
 
 ![LobsterPyAnimation](https://github.com/JaGeo/LobsterPy/assets/22094846/8f06b84c-db6d-414c-8590-aa04c957c728)
 
 
 ## Installation
+
+### Python version
+Before the installation, please make sure that you are using one of the supported Python versions (see [pyproject.toml](https://github.com/JaGeo/LobsterPy/blob/main/pyproject.toml)).
+
 ### Standard installation
 Install using ``pip install lobsterpy``
 
 ### Installation with featurizer
 Install using ``pip install lobsterpy[featurizer]``
 
 
@@ -84,15 +87,15 @@
 You can also switch the automatic analysis to use the ICOBIs or ICOOPs. You need to add `--cobis` or `--coops` along with the mentioned commands
 for e.g.like  ``lobsterpy description --cobis``
 
 An interactive plotter is available via ``lobsterpy automatic-plot-ia``.
 
 Currently, the computed Mulliken charges will be used to determine cations and anions. If no ``CHARGE.lobster`` is available, the algorithm will fall back to the BondValence analysis from pymatgen.
 
-*Please be aware that LobsterPy can only analyze bonds that have been included in the initial Lobster computation. Thus, please use the cohpgenerator within Lobster (i.e.,put "cohpGenerator from 0.1 to 5.0" to *lobsterin*).*
+*Please be aware that LobsterPy can only analyze bonds that have been included in the initial Lobster computation. Thus, please use the cohpgenerator within Lobster (i.e., put `cohpGenerator from 0.1 to 5.0` in the *lobsterin*).*
 
 
 It is also possible to start this automatic analysis from a Python script. See "examples" for scripts.
 
 * **Plotting DOS from LOBSTER computations:**
 
   To plot densities of states obtained from LOBSTER use ``lobsterpy plot-dos``.
```

### Comparing `lobsterpy-0.4.0/README.md` & `lobsterpy-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-![CI Status](https://github.com/JaGeo/LobsterPy/actions/workflows/python-package.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/JaGeo/LobsterPy/main.svg)](https://results.pre-commit.ci/latest/github/JaGeo/LobsterPy/main) [![codecov](https://codecov.io/gh/JaGeo/LobsterPy/graph/badge.svg?token=MC5BRXVEGW)](https://codecov.io/gh/JaGeo/LobsterPy) [![build-docs](https://github.com/JaGeo/LobsterPy/actions/workflows/docs.yml/badge.svg)](https://jageo.github.io/LobsterPy/) [![PyPI version](https://badge.fury.io/py/lobsterpy.svg)](https://badge.fury.io/py/lobsterpy) [![PyPI downloads](https://img.shields.io/pypi/dm/lobsterpy?style=flat&color=blue&label=pypi%20downloads)](https://pypi.org/project/lobsterpy) [![Downloads](https://pepy.tech/badge/lobsterpy)](https://pepy.tech/project/lobsterpy) [![DOI](https://zenodo.org/badge/343384088.svg)](https://zenodo.org/badge/latestdoi/343384088) [![status](https://joss.theoj.org/papers/4e8524125e36486c65a4b435bbfe2df2/status.svg)](https://joss.theoj.org/papers/4e8524125e36486c65a4b435bbfe2df2)
-
+![CI Status](https://github.com/JaGeo/LobsterPy/actions/workflows/python-package.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/JaGeo/LobsterPy/main.svg)](https://results.pre-commit.ci/latest/github/JaGeo/LobsterPy/main) [![codecov](https://codecov.io/gh/JaGeo/LobsterPy/graph/badge.svg?token=MC5BRXVEGW)](https://codecov.io/gh/JaGeo/LobsterPy) [![build-docs](https://github.com/JaGeo/LobsterPy/actions/workflows/docs.yml/badge.svg)](https://jageo.github.io/LobsterPy/) [![PyPI version](https://badge.fury.io/py/lobsterpy.svg)](https://badge.fury.io/py/lobsterpy) [![PyPI downloads](https://img.shields.io/pypi/dm/lobsterpy?style=flat&color=blue&label=pypi%20downloads)](https://pypi.org/project/lobsterpy) [![Downloads](https://pepy.tech/badge/lobsterpy)](https://pepy.tech/project/lobsterpy) ![supported python versions](https://img.shields.io/pypi/pyversions/lobsterpy) [![DOI](https://zenodo.org/badge/343384088.svg)](https://zenodo.org/badge/latestdoi/343384088) [![status](https://joss.theoj.org/papers/4e8524125e36486c65a4b435bbfe2df2/status.svg)](https://joss.theoj.org/papers/4e8524125e36486c65a4b435bbfe2df2)
 # Getting started
 <img src="https://raw.githubusercontent.com/JaGeo/LobsterPy/main/LobsterPyLogo.png" alt="LobsterPy Logo which consists of a green Python and a red Lobster" width="200"/>
 
 LobsterPy is a package that enables automatic analysis of LOBSTER outputs to get summarized bonding information and relevant bond plots. Additionally, one can also generate features for machine learning studies from LOBSTER outputs. One can download LOBSTER from [http://www.cohp.de](http://www.cohp.de).
 
 <div style="border: 1px solid #52a5ab; padding: 5px; position: relative;">
     <div style="background-color: #52a5ab; color: #ffffff; padding: 0px; position: absolute; top: 0; left: 0; right: 0; text-align: center;">
@@ -18,14 +17,18 @@
 
 Please note that LobsterPy relies on the LOBSTER computation output files. Thus, it will be only able to analyze data that has been computed in the LOBSTER run.
 
 ![LobsterPyAnimation](https://github.com/JaGeo/LobsterPy/assets/22094846/8f06b84c-db6d-414c-8590-aa04c957c728)
 
 
 ## Installation
+
+### Python version
+Before the installation, please make sure that you are using one of the supported Python versions (see [pyproject.toml](https://github.com/JaGeo/LobsterPy/blob/main/pyproject.toml)).
+
 ### Standard installation
 Install using ``pip install lobsterpy``
 
 ### Installation with featurizer
 Install using ``pip install lobsterpy[featurizer]``
 
 
@@ -41,15 +44,15 @@
 You can also switch the automatic analysis to use the ICOBIs or ICOOPs. You need to add `--cobis` or `--coops` along with the mentioned commands
 for e.g.like  ``lobsterpy description --cobis``
 
 An interactive plotter is available via ``lobsterpy automatic-plot-ia``.
 
 Currently, the computed Mulliken charges will be used to determine cations and anions. If no ``CHARGE.lobster`` is available, the algorithm will fall back to the BondValence analysis from pymatgen.
 
-*Please be aware that LobsterPy can only analyze bonds that have been included in the initial Lobster computation. Thus, please use the cohpgenerator within Lobster (i.e.,put "cohpGenerator from 0.1 to 5.0" to *lobsterin*).*
+*Please be aware that LobsterPy can only analyze bonds that have been included in the initial Lobster computation. Thus, please use the cohpgenerator within Lobster (i.e., put `cohpGenerator from 0.1 to 5.0` in the *lobsterin*).*
 
 
 It is also possible to start this automatic analysis from a Python script. See "examples" for scripts.
 
 * **Plotting DOS from LOBSTER computations:**
 
   To plot densities of states obtained from LOBSTER use ``lobsterpy plot-dos``.
```

### Comparing `lobsterpy-0.4.0/lobsterpy/cli.py` & `lobsterpy-0.4.1/lobsterpy/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) lobsterpy development team
 # Distributed under the terms of a BSD 3-Clause "New" or "Revised" License
 
 """Script to analyze Lobster outputs from the command line."""
+
 from __future__ import annotations
 
 import argparse
 import json
 import os
 from math import log, sqrt
 from pathlib import Path
@@ -936,17 +937,17 @@
 
         ax = plt.gca()
         ax.set_title(args.title)
 
         if not args.hideplot and not args.save_plot:
             plt.show()
         elif args.save_plot and not args.hideplot:
-            plt.show()
             fig = plt.gcf()
             fig.savefig(args.save_plot)
+            plt.show()
         if args.save_plot and args.hideplot:
             plt.savefig(args.save_plot)
 
     if args.action in ["create-inputs", "createinputs"]:
         from pymatgen.core.structure import Structure
         from pymatgen.io.lobster import Lobsterin
 
@@ -1054,26 +1055,24 @@
             bva_files = get_file_paths(path_to_lobster_calc=Path(os.getcwd()), requested_files=["charge"])
             for arg_name in bva_files:
                 setattr(args, arg_name, bva_files[arg_name])
 
         dos_comparison = args.doscomp
 
         if dos_comparison:
-            dos_files = get_file_paths(path_to_lobster_calc=Path(os.getcwd()), requested_files=["doscar", "vasprun"])
+            if "DOSCAR.LSO.lobster" in args.doscar.name:
+                dos_files = get_file_paths(
+                    path_to_lobster_calc=Path(os.getcwd()), requested_files=["vasprun", "doscar"], use_lso_dos=True
+                )
+            else:
+                dos_files = get_file_paths(
+                    path_to_lobster_calc=Path(os.getcwd()), requested_files=["vasprun", "doscar"]
+                )
             for arg_name in dos_files:
-                if arg_name == "doscar":
-                    file_path = getattr(args, arg_name)
-                    if not file_path.exists():
-                        gz_file_path = file_path.with_name(zpath(file_path.name))
-                        if gz_file_path.exists():
-                            setattr(args, arg_name, gz_file_path)
-                        else:
-                            raise ValueError(f"{file_path} or {gz_file_path} not found in current directory")
-                else:
-                    setattr(args, arg_name, dos_files[arg_name])
+                setattr(args, arg_name, dos_files[arg_name])
 
         potcar_file_path = args.potcar
 
         quality_dict = Analysis.get_lobster_calc_quality_summary(
             path_to_poscar=args.structure,
             path_to_charge=args.charge,
             path_to_lobsterout=args.lobsterout,
@@ -1093,27 +1092,23 @@
         Description.write_calc_quality_description(quality_text)
 
         if args.file_calc_quality_json is not None:
             with open(args.file_calc_quality_json, "w") as fd:
                 json.dump(quality_dict, fd)
 
     if args.action in ["plot-dos", "plotdos"]:
-        req_files = get_file_paths(path_to_lobster_calc=Path(os.getcwd()), requested_files=["structure", "doscar"])
+        if "DOSCAR.LSO.lobster" in args.doscar.name:
+            req_files = get_file_paths(
+                path_to_lobster_calc=Path(os.getcwd()), requested_files=["structure", "doscar"], use_lso_dos=True
+            )
+        else:
+            req_files = get_file_paths(path_to_lobster_calc=Path(os.getcwd()), requested_files=["structure", "doscar"])
 
         for arg_name in req_files:
-            if arg_name == "doscar":
-                file_path = getattr(args, arg_name)
-                if not file_path.exists():
-                    gz_file_path = file_path.with_name(zpath(file_path.name))
-                    if gz_file_path.exists():
-                        setattr(args, arg_name, gz_file_path)
-                    else:
-                        raise ValueError(f"{file_path} or {gz_file_path} not found in current directory")
-            else:
-                setattr(args, arg_name, req_files[arg_name])
+            setattr(args, arg_name, req_files[arg_name])
 
         from pymatgen.io.lobster import Doscar
 
         lobs_dos = Doscar(doscar=args.doscar, structure_file=args.structure).completedos
 
         dos_plotter = PlainDosPlotter(summed=args.summedspins, sigma=args.sigma)
         if args.addtotal:
@@ -1166,17 +1161,17 @@
 
         ax = plt.gca()
         ax.set_title(args.title)
 
         if not args.hideplot and not args.save_plot:
             plt.show()
         elif args.save_plot and not args.hideplot:
-            plt.show()
             fig = plt.gcf()
             fig.savefig(args.save_plot)
+            plt.show()
         if args.save_plot and args.hideplot:
             plt.savefig(args.save_plot)
 
     if args.action in ["plot-icohp-distance", "ploticohpdistance"]:
         if args.cobis:
             filename = get_file_paths(path_to_lobster_calc=Path(os.getcwd()), requested_files=["icobilist"]).get(
                 "icobilist"
@@ -1208,16 +1203,16 @@
 
         ax = plt.gca()
         ax.set_title(args.title)
 
         if not args.hideplot and not args.save_plot:
             plt.show()
         elif args.save_plot and not args.hideplot:
-            plt.show()
             fig = plt.gcf()
             fig.savefig(args.save_plot)
+            plt.show()
         if args.save_plot and args.hideplot:
             plt.savefig(args.save_plot)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `lobsterpy-0.4.0/lobsterpy/cohp/analyze.py` & `lobsterpy-0.4.1/lobsterpy/cohp/analyze.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) lobsterpy development team
 # Distributed under the terms of a BSD 3-Clause "New" or "Revised" License
 
 """This module defines classes to analyze the COHPs automatically."""
+
 from __future__ import annotations
 
 import warnings
 from collections import Counter
 from pathlib import Path
 
 import numpy as np
@@ -636,17 +637,17 @@
                     inx
                     for inx, orb_anti_per in enumerate(orb_contri_antibndg)
                     if orb_anti_per == max_orb_contri_antibndg
                 ]
                 max_antibndg_contri_dict = {}
                 for inx in max_antibndg_contri_inxs:
                     max_antibndg_contri_dict[orb_pairs_antibndg[inx]] = orb_contri_antibndg[inx]
-                orbital_summary_stats["orbital_summary_stats"][
-                    "max_antibonding_contribution"
-                ] = max_antibndg_contri_dict
+                orbital_summary_stats["orbital_summary_stats"]["max_antibonding_contribution"] = (
+                    max_antibndg_contri_dict
+                )
 
         return orbital_summary_stats
 
     def get_site_orbital_resolved_labels(self):
         """
         Return relevant orbitals and bond labels for each symmetrically independent site.
```

### Comparing `lobsterpy-0.4.0/lobsterpy/cohp/describe.py` & `lobsterpy-0.4.1/lobsterpy/cohp/describe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) lobsterpy development team
 # Distributed under the terms of a BSD 3-Clause "New" or "Revised" License
 
 """This module defines classes to describe the COHPs automatically."""
+
 from __future__ import annotations
 
+import warnings
 from pathlib import Path
 
 from lobsterpy.plotting import InteractiveCohpPlotter, PlainCohpPlotter
 
 
 class Description:
     """
@@ -431,14 +433,26 @@
         if self.analysis_object.which_bonds == "cation-anion":
             seq_ineq_cations = self.analysis_object.seq_ineq_ions
         elif self.analysis_object.which_bonds == "all":
             seq_ineq_cations = self.analysis_object.seq_ineq_ions
         seq_labels = self.analysis_object.seq_labels_cohps
         structure = self.analysis_object.structure
 
+        if len(seq_ineq_cations) >= 20:
+            warnings.warn(
+                "We will switch of displaying all plots "
+                "as there are more than 20 inequivalent ions. "
+                "We will instead save them in files called "
+                "'automatic-analysis-*.png'."
+            )
+            hide = True
+            save = True
+            if filename is None:
+                filename = "./automatic_analysis.png"
+
         for iplot, (ication, labels, cohps) in enumerate(zip(seq_ineq_cations, seq_labels, seq_cohps)):
             namecation = str(structure[ication].specie)
 
             cp = PlainCohpPlotter(
                 are_coops=self.analysis_object.are_coops,
                 are_cobis=self.analysis_object.are_cobis,
             )
@@ -458,19 +472,18 @@
                         filename = Path(filename)  # type: ignore
                     filename_new = (
                         filename.parent / f"{filename.stem}-{iplot}{filename.suffix}"  # type: ignore
                     )
                 else:
                     filename_new = filename
                 plot.savefig(filename_new)
+                if hide:
+                    plot.close()
         if not hide:
             plot.show()
-        else:
-            if not save:
-                plot.close()
 
     def plot_interactive_cohps(
         self,
         ylim: list[float] | None = None,
         xlim: list[float] | None = None,
         save_as_html: bool = False,
         filename: str | None = None,
```

### Comparing `lobsterpy-0.4.0/lobsterpy/featurize/batch.py` & `lobsterpy-0.4.1/lobsterpy/featurize/batch.py`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.0/lobsterpy/featurize/core.py` & `lobsterpy-0.4.1/lobsterpy/featurize/core.py`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.0/lobsterpy/featurize/utils.py` & `lobsterpy-0.4.1/lobsterpy/featurize/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) lobsterpy development team
 # Distributed under the terms of a BSD 3-Clause "New" or "Revised" License
 
 """This package provides the modules for featurzing Lobster data ready for ML studies."""
+
 from __future__ import annotations
 
 from pathlib import Path
 
 from monty.os.path import zpath
```

### Comparing `lobsterpy-0.4.0/lobsterpy/plotting/__init__.py` & `lobsterpy-0.4.1/lobsterpy/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.0/lobsterpy/plotting/layout_dicts.py` & `lobsterpy-0.4.1/lobsterpy/plotting/layout_dicts.py`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.0/lobsterpy/structuregraph/graph.py` & `lobsterpy-0.4.1/lobsterpy/structuregraph/graph.py`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.0/lobsterpy.egg-info/PKG-INFO` & `lobsterpy-0.4.1/lobsterpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lobsterpy
-Version: 0.4.0
+Version: 0.4.1
 Summary: Package for automatic bonding analysis with Lobster/VASP
 Author-email: Janine George <janine.george@bam.de>
 License: BSD 3-Clause
 Project-URL: homepage, https://jageo.github.io/LobsterPy/
 Project-URL: repository, https://github.com/JaGeo/LobsterPy
 Project-URL: documentation, https://jageo.github.io/LobsterPy/
 Project-URL: changelog, https://jageo.github.io/LobsterPy/about/changelog.html
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pymatgen>=2024.2.23
+Requires-Dist: pymatgen>=2024.4.13
 Requires-Dist: numpy
 Requires-Dist: typing
 Provides-Extra: featurizer
 Requires-Dist: mendeleev==0.15.0; extra == "featurizer"
 Provides-Extra: dev
 Requires-Dist: pre-commit>=2.12.1; extra == "dev"
 Provides-Extra: tests
@@ -32,21 +32,20 @@
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: pytest-split; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinx<6,>=5; extra == "docs"
 Requires-Dist: sphinx_design==0.5.0; extra == "docs"
-Requires-Dist: myst-nb==1.0.0; extra == "docs"
+Requires-Dist: myst-nb==1.1.0; extra == "docs"
 Requires-Dist: sphinx-book-theme==1.1.2; extra == "docs"
 Requires-Dist: sphinx-argparse==0.4.0; extra == "docs"
 Requires-Dist: sphinx-toolbox==3.5.0; extra == "docs"
 
-![CI Status](https://github.com/JaGeo/LobsterPy/actions/workflows/python-package.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/JaGeo/LobsterPy/main.svg)](https://results.pre-commit.ci/latest/github/JaGeo/LobsterPy/main) [![codecov](https://codecov.io/gh/JaGeo/LobsterPy/graph/badge.svg?token=MC5BRXVEGW)](https://codecov.io/gh/JaGeo/LobsterPy) [![build-docs](https://github.com/JaGeo/LobsterPy/actions/workflows/docs.yml/badge.svg)](https://jageo.github.io/LobsterPy/) [![PyPI version](https://badge.fury.io/py/lobsterpy.svg)](https://badge.fury.io/py/lobsterpy) [![PyPI downloads](https://img.shields.io/pypi/dm/lobsterpy?style=flat&color=blue&label=pypi%20downloads)](https://pypi.org/project/lobsterpy) [![Downloads](https://pepy.tech/badge/lobsterpy)](https://pepy.tech/project/lobsterpy) [![DOI](https://zenodo.org/badge/343384088.svg)](https://zenodo.org/badge/latestdoi/343384088) [![status](https://joss.theoj.org/papers/4e8524125e36486c65a4b435bbfe2df2/status.svg)](https://joss.theoj.org/papers/4e8524125e36486c65a4b435bbfe2df2)
-
+![CI Status](https://github.com/JaGeo/LobsterPy/actions/workflows/python-package.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/JaGeo/LobsterPy/main.svg)](https://results.pre-commit.ci/latest/github/JaGeo/LobsterPy/main) [![codecov](https://codecov.io/gh/JaGeo/LobsterPy/graph/badge.svg?token=MC5BRXVEGW)](https://codecov.io/gh/JaGeo/LobsterPy) [![build-docs](https://github.com/JaGeo/LobsterPy/actions/workflows/docs.yml/badge.svg)](https://jageo.github.io/LobsterPy/) [![PyPI version](https://badge.fury.io/py/lobsterpy.svg)](https://badge.fury.io/py/lobsterpy) [![PyPI downloads](https://img.shields.io/pypi/dm/lobsterpy?style=flat&color=blue&label=pypi%20downloads)](https://pypi.org/project/lobsterpy) [![Downloads](https://pepy.tech/badge/lobsterpy)](https://pepy.tech/project/lobsterpy) ![supported python versions](https://img.shields.io/pypi/pyversions/lobsterpy) [![DOI](https://zenodo.org/badge/343384088.svg)](https://zenodo.org/badge/latestdoi/343384088) [![status](https://joss.theoj.org/papers/4e8524125e36486c65a4b435bbfe2df2/status.svg)](https://joss.theoj.org/papers/4e8524125e36486c65a4b435bbfe2df2)
 # Getting started
 <img src="https://raw.githubusercontent.com/JaGeo/LobsterPy/main/LobsterPyLogo.png" alt="LobsterPy Logo which consists of a green Python and a red Lobster" width="200"/>
 
 LobsterPy is a package that enables automatic analysis of LOBSTER outputs to get summarized bonding information and relevant bond plots. Additionally, one can also generate features for machine learning studies from LOBSTER outputs. One can download LOBSTER from [http://www.cohp.de](http://www.cohp.de).
 
 <div style="border: 1px solid #52a5ab; padding: 5px; position: relative;">
     <div style="background-color: #52a5ab; color: #ffffff; padding: 0px; position: absolute; top: 0; left: 0; right: 0; text-align: center;">
@@ -61,14 +60,18 @@
 
 Please note that LobsterPy relies on the LOBSTER computation output files. Thus, it will be only able to analyze data that has been computed in the LOBSTER run.
 
 ![LobsterPyAnimation](https://github.com/JaGeo/LobsterPy/assets/22094846/8f06b84c-db6d-414c-8590-aa04c957c728)
 
 
 ## Installation
+
+### Python version
+Before the installation, please make sure that you are using one of the supported Python versions (see [pyproject.toml](https://github.com/JaGeo/LobsterPy/blob/main/pyproject.toml)).
+
 ### Standard installation
 Install using ``pip install lobsterpy``
 
 ### Installation with featurizer
 Install using ``pip install lobsterpy[featurizer]``
 
 
@@ -84,15 +87,15 @@
 You can also switch the automatic analysis to use the ICOBIs or ICOOPs. You need to add `--cobis` or `--coops` along with the mentioned commands
 for e.g.like  ``lobsterpy description --cobis``
 
 An interactive plotter is available via ``lobsterpy automatic-plot-ia``.
 
 Currently, the computed Mulliken charges will be used to determine cations and anions. If no ``CHARGE.lobster`` is available, the algorithm will fall back to the BondValence analysis from pymatgen.
 
-*Please be aware that LobsterPy can only analyze bonds that have been included in the initial Lobster computation. Thus, please use the cohpgenerator within Lobster (i.e.,put "cohpGenerator from 0.1 to 5.0" to *lobsterin*).*
+*Please be aware that LobsterPy can only analyze bonds that have been included in the initial Lobster computation. Thus, please use the cohpgenerator within Lobster (i.e., put `cohpGenerator from 0.1 to 5.0` in the *lobsterin*).*
 
 
 It is also possible to start this automatic analysis from a Python script. See "examples" for scripts.
 
 * **Plotting DOS from LOBSTER computations:**
 
   To plot densities of states obtained from LOBSTER use ``lobsterpy plot-dos``.
```

### Comparing `lobsterpy-0.4.0/lobsterpy.egg-info/SOURCES.txt` & `lobsterpy-0.4.1/lobsterpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.0/pyproject.toml` & `lobsterpy-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 [project]
 name = "lobsterpy"
 description = "Package for automatic bonding analysis with Lobster/VASP"
 readme = "README.md"
 keywords = ["high-throughput", "automated", "lobsteroutput", "bonding-analysis"]
 license = { text = "BSD 3-Clause" }
 authors = [{ name = "Janine George", email = "janine.george@bam.de" }]
-version = "0.4.0"
+version = "0.4.1"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.9,<3.12"
 dependencies = [
-     "pymatgen>=2024.2.23",
+     "pymatgen>=2024.4.13",
      "numpy",
      "typing",
 ]
 
 [tool.setuptools.package-data]
 "lobsterpy.plotting" = ["lobsterpy_base.mplstyle"]
 
@@ -46,15 +46,15 @@
 featurizer = ["mendeleev==0.15.0"]
 dev = ["pre-commit>=2.12.1"]
 tests = ["flake8", "pytest", "pytest-mock", "pytest-split", "pytest-cov"]
 docs = [
     "sphinx-copybutton==0.5.2",
     "sphinx>=5,<6",
     "sphinx_design==0.5.0",
-    "myst-nb==1.0.0",
+    "myst-nb==1.1.0",
     "sphinx-book-theme==1.1.2",
     "sphinx-argparse==0.4.0",
     "sphinx-toolbox==3.5.0",
 ]
 
 [project.scripts]
 lobsterpy = "lobsterpy.cli:main"
```


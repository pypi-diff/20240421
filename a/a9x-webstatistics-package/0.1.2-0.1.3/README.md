# Comparing `tmp/a9x_webstatistics_package-0.1.2.tar.gz` & `tmp/a9x_webstatistics_package-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a9x_webstatistics_package-0.1.2.tar", last modified: Thu Apr 18 15:01:36 2024, max compression
+gzip compressed data, was "a9x_webstatistics_package-0.1.3.tar", last modified: Sun Apr 21 13:57:10 2024, max compression
```

## Comparing `a9x_webstatistics_package-0.1.2.tar` & `a9x_webstatistics_package-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:01:36.327001 a9x_webstatistics_package-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16687 2024-04-18 15:01:36.327001 a9x_webstatistics_package-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/dist_del
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 15:01:36.327001 a9x_webstatistics_package-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:01:36.323001 a9x_webstatistics_package-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:01:36.323001 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics/module1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:01:36.327001 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics_package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16687 2024-04-18 15:01:36.000000 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics_package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-18 15:01:36.000000 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics_package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:01:36.000000 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics_package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 15:01:36.000000 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics_package.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 15:01:36.000000 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics_package.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:01:36.327001 a9x_webstatistics_package-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/tests/test_main001.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/tests/test_main010.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/tests/test_module1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:57:10.302893 a9x_webstatistics_package-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-21 13:57:01.000000 a9x_webstatistics_package-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-21 13:57:01.000000 a9x_webstatistics_package-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-04-21 13:57:10.302893 a9x_webstatistics_package-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-04-21 13:57:01.000000 a9x_webstatistics_package-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:57:01.000000 a9x_webstatistics_package-0.1.3/dist_del
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-21 13:57:01.000000 a9x_webstatistics_package-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-21 13:57:10.302893 a9x_webstatistics_package-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-21 13:57:01.000000 a9x_webstatistics_package-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:57:10.298893 a9x_webstatistics_package-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:57:10.302893 a9x_webstatistics_package-0.1.3/src/a9x_webstatistics/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-21 13:57:01.000000 a9x_webstatistics_package-0.1.3/src/a9x_webstatistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-21 13:57:01.000000 a9x_webstatistics_package-0.1.3/src/a9x_webstatistics/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-21 13:57:01.000000 a9x_webstatistics_package-0.1.3/src/a9x_webstatistics/module1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-21 13:57:01.000000 a9x_webstatistics_package-0.1.3/src/a9x_webstatistics/updatestatistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:57:10.302893 a9x_webstatistics_package-0.1.3/src/a9x_webstatistics_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-04-21 13:57:10.000000 a9x_webstatistics_package-0.1.3/src/a9x_webstatistics_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-21 13:57:10.000000 a9x_webstatistics_package-0.1.3/src/a9x_webstatistics_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:57:10.000000 a9x_webstatistics_package-0.1.3/src/a9x_webstatistics_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 13:57:10.000000 a9x_webstatistics_package-0.1.3/src/a9x_webstatistics_package.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-21 13:57:10.000000 a9x_webstatistics_package-0.1.3/src/a9x_webstatistics_package.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:57:10.302893 a9x_webstatistics_package-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-21 13:57:01.000000 a9x_webstatistics_package-0.1.3/tests/test_main001.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-21 13:57:01.000000 a9x_webstatistics_package-0.1.3/tests/test_main010.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-21 13:57:01.000000 a9x_webstatistics_package-0.1.3/tests/test_module1.py
```

### Comparing `a9x_webstatistics_package-0.1.2/LICENSE` & `a9x_webstatistics_package-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics_package-0.1.2/PKG-INFO` & `a9x_webstatistics_package-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a9x_webstatistics_package
-Version: 0.1.2
+Version: 0.1.3
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
@@ -25,38 +25,43 @@
 
 # Web Statistics and Analytics
 
 This package produces web statics and analytical output based on nginx access log files.
 
 [![PyPI package](https://img.shields.io/badge/pip%20install-example--pypi--package-brightgreen)](https://pypi.org/project/a9x-webstatistics-package/) [![version number](https://img.shields.io/pypi/v/example-pypi-package?color=green&label=version)](https://github.com/ava007/a9x-webstatistics/releases) [![Actions Status](https://github.com/ava007/a9x-webstatistics/workflows/Test/badge.svg)](https://github.com/ava007/a9x-webstatistics/actions) [![License](https://img.shields.io/github/license/ava007/a9x-webstatistics)](https://github.com/ava007/a9x-webstatistics/blob/main/LICENSE)
 
+## Installation
 
+```bash
+pip install a9x-webstatistics-package
+```
 
+
+<details>
 ----------------
 ## old content from template starts here
 
 [![PyPI package](https://img.shields.io/badge/pip%20install-example--pypi--package-brightgreen)](https://pypi.org/project/example-pypi-package/) [![version number](https://img.shields.io/pypi/v/example-pypi-package?color=green&label=version)](https://github.com/tomchen/example_pypi_package/releases) [![Actions Status](https://github.com/tomchen/example_pypi_package/workflows/Test/badge.svg)](https://github.com/tomchen/example_pypi_package/actions) [![License](https://img.shields.io/github/license/tomchen/example_pypi_package)](https://github.com/tomchen/example_pypi_package/blob/main/LICENSE)
 
 This is an example [PyPI](https://pypi.org/) (Python Package Index) package set up with automated tests and package publishing workflow using GitHub Actions CI/CD. It is made primarily for GitHub + VS Code (Windows / Mac / Linux) users who are about to write and publish their first PyPI package. The package could serve as a starter / boilerplate / demo and the tutorial could give you a quick and concise explaination to solve some small but annoying problems you might encounter, such as package / module name confusion, and VS Code test configuration issues.
-
-<details><summary><strong>Differences from pypa/sampleproject (click to show/hide)</strong></summary>
+<summary><strong>Differences from pypa/sampleproject (click to show/hide)</strong></summary>
 
 This example package is inspired by / based on the [official sample project pypa/sampleproject](https://github.com/pypa/sampleproject), but this package:
 
 - is a simplified version of pypa/sampleproject (and the [official Python Packaging User Guide](https://packaging.python.org/))
 - uses GitHub Actions for both testing and publishing, instead of Travis CI
 - is tested when pushing `master` or `main` branch, and is published when create a release
 - includes test files in the source distribution
 - uses **setup.cfg** for [version single-sourcing](https://packaging.python.org/guides/single-sourcing-package-version/) (setuptools 46.4.0+)
 - has **.vscode\settings.json** and **vscode.env** which adds **src/** folder to `PYTHONPATH`, so that test files don't have linting errors and may run with pytest in VS Code
 - does not use flake8 for automated linting - it is sometimes too strict and inflexible, you may use pylint locally instead
 - has this tutorial that covers everything you need to know in one page. Everything that might not be very useful, is hidden in collapsible sections that you can click to show
 - has **[.editorconfig](https://editorconfig.org/#download)** file
 
-</details>
+
 
 ## Make necessary changes
 
 ### Use as a template
 
 [![Use the template](https://img.shields.io/static/v1?label=&message=Click%20here%20to%20use%20this%20package%20as%20a%20template%20to%20start%20a%20new%20repo%20on%20GitHub&color=brightgreen&style=for-the-badge)](https://github.com/tomchen/example_pypi_package/generate)
 
@@ -285,8 +290,9 @@
 ## References
 
 - [Python Packaging Authority (PyPA)'s sample project](https://github.com/pypa/sampleproject)
 - [PyPA's Python Packaging User Guide](https://packaging.python.org/tutorials/packaging-projects/)
 - [Stackoverflow questions and answers](https://stackoverflow.com/questions/41093648/how-to-test-that-pypi-install-will-work-before-pushing-to-pypi-python)
 - [GitHub Actions Guides: Building and testing Python](https://docs.github.com/en/free-pro-team@latest/actions/guides/building-and-testing-python)
 
-Btw, if you want to publish TypeScript (JavaScript) package to the npm registry, go to [Example TypeScript Package ready to be published on npm for 2021](https://github.com/tomchen/example-typescript-package).
+
+</details>
```

### Comparing `a9x_webstatistics_package-0.1.2/README.md` & `a9x_webstatistics_package-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 # Web Statistics and Analytics
 
 This package produces web statics and analytical output based on nginx access log files.
 
 [![PyPI package](https://img.shields.io/badge/pip%20install-example--pypi--package-brightgreen)](https://pypi.org/project/a9x-webstatistics-package/) [![version number](https://img.shields.io/pypi/v/example-pypi-package?color=green&label=version)](https://github.com/ava007/a9x-webstatistics/releases) [![Actions Status](https://github.com/ava007/a9x-webstatistics/workflows/Test/badge.svg)](https://github.com/ava007/a9x-webstatistics/actions) [![License](https://img.shields.io/github/license/ava007/a9x-webstatistics)](https://github.com/ava007/a9x-webstatistics/blob/main/LICENSE)
 
+## Installation
 
+```bash
+pip install a9x-webstatistics-package
+```
 
+
+<details>
 ----------------
 ## old content from template starts here
 
 [![PyPI package](https://img.shields.io/badge/pip%20install-example--pypi--package-brightgreen)](https://pypi.org/project/example-pypi-package/) [![version number](https://img.shields.io/pypi/v/example-pypi-package?color=green&label=version)](https://github.com/tomchen/example_pypi_package/releases) [![Actions Status](https://github.com/tomchen/example_pypi_package/workflows/Test/badge.svg)](https://github.com/tomchen/example_pypi_package/actions) [![License](https://img.shields.io/github/license/tomchen/example_pypi_package)](https://github.com/tomchen/example_pypi_package/blob/main/LICENSE)
 
 This is an example [PyPI](https://pypi.org/) (Python Package Index) package set up with automated tests and package publishing workflow using GitHub Actions CI/CD. It is made primarily for GitHub + VS Code (Windows / Mac / Linux) users who are about to write and publish their first PyPI package. The package could serve as a starter / boilerplate / demo and the tutorial could give you a quick and concise explaination to solve some small but annoying problems you might encounter, such as package / module name confusion, and VS Code test configuration issues.
-
-<details><summary><strong>Differences from pypa/sampleproject (click to show/hide)</strong></summary>
+<summary><strong>Differences from pypa/sampleproject (click to show/hide)</strong></summary>
 
 This example package is inspired by / based on the [official sample project pypa/sampleproject](https://github.com/pypa/sampleproject), but this package:
 
 - is a simplified version of pypa/sampleproject (and the [official Python Packaging User Guide](https://packaging.python.org/))
 - uses GitHub Actions for both testing and publishing, instead of Travis CI
 - is tested when pushing `master` or `main` branch, and is published when create a release
 - includes test files in the source distribution
 - uses **setup.cfg** for [version single-sourcing](https://packaging.python.org/guides/single-sourcing-package-version/) (setuptools 46.4.0+)
 - has **.vscode\settings.json** and **vscode.env** which adds **src/** folder to `PYTHONPATH`, so that test files don't have linting errors and may run with pytest in VS Code
 - does not use flake8 for automated linting - it is sometimes too strict and inflexible, you may use pylint locally instead
 - has this tutorial that covers everything you need to know in one page. Everything that might not be very useful, is hidden in collapsible sections that you can click to show
 - has **[.editorconfig](https://editorconfig.org/#download)** file
 
-</details>
+
 
 ## Make necessary changes
 
 ### Use as a template
 
 [![Use the template](https://img.shields.io/static/v1?label=&message=Click%20here%20to%20use%20this%20package%20as%20a%20template%20to%20start%20a%20new%20repo%20on%20GitHub&color=brightgreen&style=for-the-badge)](https://github.com/tomchen/example_pypi_package/generate)
 
@@ -260,8 +265,9 @@
 ## References
 
 - [Python Packaging Authority (PyPA)'s sample project](https://github.com/pypa/sampleproject)
 - [PyPA's Python Packaging User Guide](https://packaging.python.org/tutorials/packaging-projects/)
 - [Stackoverflow questions and answers](https://stackoverflow.com/questions/41093648/how-to-test-that-pypi-install-will-work-before-pushing-to-pypi-python)
 - [GitHub Actions Guides: Building and testing Python](https://docs.github.com/en/free-pro-team@latest/actions/guides/building-and-testing-python)
 
-Btw, if you want to publish TypeScript (JavaScript) package to the npm registry, go to [Example TypeScript Package ready to be published on npm for 2021](https://github.com/tomchen/example-typescript-package).
+
+</details>
```

### Comparing `a9x_webstatistics_package-0.1.2/setup.py` & `a9x_webstatistics_package-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics_package-0.1.2/src/a9x_webstatistics_package.egg-info/PKG-INFO` & `a9x_webstatistics_package-0.1.3/src/a9x_webstatistics_package.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a9x_webstatistics_package
-Version: 0.1.2
+Version: 0.1.3
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
@@ -25,38 +25,43 @@
 
 # Web Statistics and Analytics
 
 This package produces web statics and analytical output based on nginx access log files.
 
 [![PyPI package](https://img.shields.io/badge/pip%20install-example--pypi--package-brightgreen)](https://pypi.org/project/a9x-webstatistics-package/) [![version number](https://img.shields.io/pypi/v/example-pypi-package?color=green&label=version)](https://github.com/ava007/a9x-webstatistics/releases) [![Actions Status](https://github.com/ava007/a9x-webstatistics/workflows/Test/badge.svg)](https://github.com/ava007/a9x-webstatistics/actions) [![License](https://img.shields.io/github/license/ava007/a9x-webstatistics)](https://github.com/ava007/a9x-webstatistics/blob/main/LICENSE)
 
+## Installation
 
+```bash
+pip install a9x-webstatistics-package
+```
 
+
+<details>
 ----------------
 ## old content from template starts here
 
 [![PyPI package](https://img.shields.io/badge/pip%20install-example--pypi--package-brightgreen)](https://pypi.org/project/example-pypi-package/) [![version number](https://img.shields.io/pypi/v/example-pypi-package?color=green&label=version)](https://github.com/tomchen/example_pypi_package/releases) [![Actions Status](https://github.com/tomchen/example_pypi_package/workflows/Test/badge.svg)](https://github.com/tomchen/example_pypi_package/actions) [![License](https://img.shields.io/github/license/tomchen/example_pypi_package)](https://github.com/tomchen/example_pypi_package/blob/main/LICENSE)
 
 This is an example [PyPI](https://pypi.org/) (Python Package Index) package set up with automated tests and package publishing workflow using GitHub Actions CI/CD. It is made primarily for GitHub + VS Code (Windows / Mac / Linux) users who are about to write and publish their first PyPI package. The package could serve as a starter / boilerplate / demo and the tutorial could give you a quick and concise explaination to solve some small but annoying problems you might encounter, such as package / module name confusion, and VS Code test configuration issues.
-
-<details><summary><strong>Differences from pypa/sampleproject (click to show/hide)</strong></summary>
+<summary><strong>Differences from pypa/sampleproject (click to show/hide)</strong></summary>
 
 This example package is inspired by / based on the [official sample project pypa/sampleproject](https://github.com/pypa/sampleproject), but this package:
 
 - is a simplified version of pypa/sampleproject (and the [official Python Packaging User Guide](https://packaging.python.org/))
 - uses GitHub Actions for both testing and publishing, instead of Travis CI
 - is tested when pushing `master` or `main` branch, and is published when create a release
 - includes test files in the source distribution
 - uses **setup.cfg** for [version single-sourcing](https://packaging.python.org/guides/single-sourcing-package-version/) (setuptools 46.4.0+)
 - has **.vscode\settings.json** and **vscode.env** which adds **src/** folder to `PYTHONPATH`, so that test files don't have linting errors and may run with pytest in VS Code
 - does not use flake8 for automated linting - it is sometimes too strict and inflexible, you may use pylint locally instead
 - has this tutorial that covers everything you need to know in one page. Everything that might not be very useful, is hidden in collapsible sections that you can click to show
 - has **[.editorconfig](https://editorconfig.org/#download)** file
 
-</details>
+
 
 ## Make necessary changes
 
 ### Use as a template
 
 [![Use the template](https://img.shields.io/static/v1?label=&message=Click%20here%20to%20use%20this%20package%20as%20a%20template%20to%20start%20a%20new%20repo%20on%20GitHub&color=brightgreen&style=for-the-badge)](https://github.com/tomchen/example_pypi_package/generate)
 
@@ -285,8 +290,9 @@
 ## References
 
 - [Python Packaging Authority (PyPA)'s sample project](https://github.com/pypa/sampleproject)
 - [PyPA's Python Packaging User Guide](https://packaging.python.org/tutorials/packaging-projects/)
 - [Stackoverflow questions and answers](https://stackoverflow.com/questions/41093648/how-to-test-that-pypi-install-will-work-before-pushing-to-pypi-python)
 - [GitHub Actions Guides: Building and testing Python](https://docs.github.com/en/free-pro-team@latest/actions/guides/building-and-testing-python)
 
-Btw, if you want to publish TypeScript (JavaScript) package to the npm registry, go to [Example TypeScript Package ready to be published on npm for 2021](https://github.com/tomchen/example-typescript-package).
+
+</details>
```

### Comparing `a9x_webstatistics_package-0.1.2/tests/test_main001.py` & `a9x_webstatistics_package-0.1.3/tests/test_main001.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import unittest
 from pathlib import Path
 
 from a9x_webstatistics.main import *
+from a9x_webstatistics.updatestatistics import upd
 
 class TestMain(unittest.TestCase):
 
     def test_main(self):
         print("home: " + str(Path.home()) )
         # calling runws expecting return 0
         assert runws() == 0
         file = Path("webstat.json")  
         with open(file) as f:  
             file_data = f.read()  
         print(str(file_data))
         contents = json.loads(file_data)
-        assert '19991231235959' in contents['timelastrec']
+        assert '20240130144922' in contents['timelastrec']
 
 if __name__ == '__main__':
     unittest.main()
```


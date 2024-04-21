# Comparing `tmp/snickerdoodle-0.1.9.tar.gz` & `tmp/snickerdoodle-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snickerdoodle-0.1.9.tar", last modified: Wed Sep 20 17:46:49 2023, max compression
+gzip compressed data, was "snickerdoodle-0.2.0.tar", last modified: Sun Apr 21 03:34:05 2024, max compression
```

## Comparing `snickerdoodle-0.1.9.tar` & `snickerdoodle-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      589 2023-09-20 17:46:30.582908 snickerdoodle-0.1.9/LICENSE
--rwxr-xr-x   0        0        0    12843 2023-09-20 17:46:30.582908 snickerdoodle-0.1.9/README.md
--rw-r--r--   0        0        0     3385 2023-09-20 17:46:49.514962 snickerdoodle-0.1.9/pyproject.toml
--rwxr-xr-x   0        0        0      168 2023-09-20 17:46:30.590908 snickerdoodle-0.1.9/tests/test_main.py
--rw-r--r--   0        0        0    14019 1970-01-01 00:00:00.000000 snickerdoodle-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      589 2024-04-21 03:33:52.955791 snickerdoodle-0.2.0/LICENSE
+-rwxr-xr-x   0        0        0    12835 2024-04-21 03:33:52.955791 snickerdoodle-0.2.0/README.md
+-rw-r--r--   0        0        0     4001 2024-04-21 03:34:05.907776 snickerdoodle-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0      168 2024-04-21 03:33:52.963791 snickerdoodle-0.2.0/tests/test_main.py
+-rw-r--r--   0        0        0    14062 1970-01-01 00:00:00.000000 snickerdoodle-0.2.0/PKG-INFO
```

### Comparing `snickerdoodle-0.1.9/LICENSE` & `snickerdoodle-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snickerdoodle-0.1.9/README.md` & `snickerdoodle-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,44 +11,44 @@
 | Documentation | [![Hosted By](https://img.shields.io/badge/hosted_by-GitHub_Pages-blue?style=for-the-badge&color=navy&logo=github)](https://withprecedent.github.io/snickerdoodle)
 | Compatibility | [![Compatible Python Versions](https://img.shields.io/pypi/pyversions/snickerdoodle?style=for-the-badge&color=steelblue&label=Python&logo=python&logoColor=yellow)](https://pypi.python.org/pypi/snickerdoodle/) [![Linux](https://img.shields.io/badge/Linux-lightseagreen?style=for-the-badge&logo=linux&labelColor=gray&logoColor=white)](https://www.linux.org/) [![MacOS](https://img.shields.io/badge/MacOS-snow?style=for-the-badge&logo=apple&labelColor=gray)](https://www.apple.com/macos/) [![Windows](https://img.shields.io/badge/windows-blue?style=for-the-badge&logo=Windows&labelColor=gray&color=orangered)](https://www.microsoft.com/en-us/windows?r=1)
 | Stats | [![PyPI Download Rate (per month)](https://img.shields.io/pypi/dm/snickerdoodle?style=for-the-badge&color=steelblue&label=Downloads%20💾&logo=pypi&logoColor=yellow)](https://pypi.org/project/snickerdoodle) [![GitHub Stars](https://img.shields.io/github/stars/withprecedent/snickerdoodle?style=for-the-badge&color=navy&label=Stars%20⭐&logo=github)](https://github.com/withprecedent/snickerdoodle/stargazers) [![GitHub Contributors](https://img.shields.io/github/contributors/withprecedent/snickerdoodle?style=for-the-badge&color=navy&label=Contributors%20🙋&logo=github)](https://github.com/withprecedent/snickerdoodle/graphs/contributors) [![GitHub Issues](https://img.shields.io/github/issues/withprecedent/snickerdoodle?style=for-the-badge&color=navy&label=Issues%20📘&logo=github)](https://github.com/withprecedent/snickerdoodle/graphs/contributors) [![GitHub Forks](https://img.shields.io/github/forks/withprecedent/snickerdoodle?style=for-the-badge&color=navy&label=Forks%20🍴&logo=github)](https://github.com/withprecedent/snickerdoodle/forks) |
 | | |
 
 ## What is snickerdoodle?
 
-`snickerdoodle`is an easy-to-use, general-purpose cookiecutter template for
+`snickerdoodle` is an easy-to-use, general-purpose cookiecutter template for
 Python projects utilizing modern tools and best practices. To see an example repository using this template,
 check out
 [`snickerdoodle_demo`](https://github.com/withprecedent/snickerdoodle_demo).
-  
+
 ## Why use snickerdoodle?
 
 There are a lot of cookiecutter templates. However, many are difficult to use,
 overly opinionated, or underdocumented. I created `snickerdoodle` because I
 couldn't
 find another `cookiecutter` template meeting these criteria:
 
-* **Modern**: follows best practices, using modern, actively developed tools
-* **Batteries Included**: allows you to start coding immediately
-* **Flexible**: no required usage of any external services
-  (SonarCloud, Travis, CircleCI, Tox, etc.)
+* **Modern**: follows best practices, using modern, actively developed tools.
+* **Batteries Included**: allows you to start coding immediately.
+* **Flexible**: no required usage of any external services.
+  (SonarCloud, Travis, CircleCI, Tox, etc.).
 * **Low-Maintenance**: every commit automatically deploys the documentation as
   well as
-  lints, formats, and tests the repository
+  lints, formats, and tests the repository.
 * **Well-Documented**: the
   [documentation](https://withprecedent.github.io/snickerdoodle) includes
-  complete guides for [new](https://withprecedent.github.io/snickerdoodle/tutorial/) and [advanced](https://withprecedent.github.io/snickerdoodle/advanced/) users
+  complete guides for [new](https://withprecedent.github.io/snickerdoodle/tutorial/) and [advanced](https://withprecedent.github.io/snickerdoodle/advanced/) users.
 * **PEP-Compliant**: all included tools follow accepted
   [PEPs](https://peps.python.org/pep-0001/) (unfortunately, that ruled out using
   `poetry`, which is [still not](https://github.com/python-poetry/roadmap/issues/3) [PEP 621](https://peps.python.org/pep-0621/) or
   [PEP 631](https://peps.python.org/pep-0631/)
   compliant, three years after they were accepted,
   [resulting in compatibility](https://github.com/python-poetry/poetry/issues/496)
   [problems because of its](https://github.com/python-poetry/poetry/issues/3332)
-  [non-standard `pyproject.toml` format](https://github.com/python-poetry/poetry/issues/8415))
+  [non-standard `pyproject.toml` format](https://github.com/python-poetry/poetry/issues/8415)).
 
 ### Tools
 
 To accomplish those goals, `snickerdoodle` includes modern, stable tools for package construction and
 management that do not require any external services or costs:
 
 * Dependency Management: [![Dependency Manager](https://img.shields.io/badge/PDM-mediumpurple?style=flat-square&logo=affinity&labelColor=gray)](https://PDM.fming.dev) and [![Dependency Maintainer](https://img.shields.io/badge/dependabot-navy?style=flat-square&logo=dependabot&logoColor=white&labelColor=gray)](https://github.com/dependabot)
@@ -115,17 +115,16 @@
 * [Repository Layout](https://withprecedent.github.io/snickerdoodle/advanced/#repository-layout)
 * [Versioning](https://withprecedent.github.io/snickerdoodle/advanced/#versioning)
 
 ## Contributing
 
 Contributors are always welcome and should find `snickerdoodle` easy to work
 with. The template is highly documented so that users and developers can adapt
-or extend`snickerdoodle` to work with their projects. So, forking and creating
-different template spins is encouraged. If you want to contribute directly to
-the project, feel free to grab an [issue](https://github.com/WithPrecedent/snickerdoodle/issues) to work on
+or extend `snickerdoodle` to work with their projects. So, forking and creating
+different template spins is encouraged. If you want to contribute directly, feel free to grab an [issue](https://github.com/WithPrecedent/snickerdoodle/issues) to work on
 or make a suggested improvement. If you wish to contribute, please read the
 [Contribution Guide](./contributing.md) and [Code of
 Conduct](./code_of_conduct.md).
 
 ## Similar Projects
 
 These are other `cookiecutter` templates using `pdm` as their dependency manager:
```

### Comparing `snickerdoodle-0.1.9/pyproject.toml` & `snickerdoodle-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [project]
 name = "snickerdoodle"
 description = "Easy-to-use, general-purpose, modern cookiecutter template for Python"
 authors = [
     { name = "coreyrayburnyung", email = "coreyrayburnyung@gmail.com" },
 ]
-version = "0.1.9"
+version = "0.2.0"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Pre-processors",
 ]
 keywords = []
 dependencies = []
 
@@ -90,14 +91,18 @@
     "docs",
     "scripts",
     "site",
     "tests",
     ".*.*",
 ]
 fix = true
+line-length = 80
+
+[tool.ruff.lint]
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 fixable = [
     "ALL",
 ]
 ignore = [
     "A001",
     "ANN101",
     "ANN102",
@@ -120,19 +125,19 @@
     "PTH123",
     "PLR0911",
     "PLR0912",
     "PLR0913",
     "PLR0915",
     "PLR1711",
     "Q000",
+    "RET505",
     "SLF001",
     "TID252",
     "TRY003",
 ]
-line-length = 80
 select = [
     "A",
     "ANN",
     "ARG",
     "B",
     "BLE",
     "C",
@@ -176,16 +181,40 @@
     "TCH",
     "TID",
     "TRY",
     "UP",
     "W",
     "YTT",
 ]
+task-tags = [
+    "To Do:",
+]
+
+[tool.ruff.lint.flake8-annotations]
+suppress-none-returning = true
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 docstring-quotes = "double"
+inline-quotes = "double"
+multiline-quotes = "double"
+
+[tool.ruff.lint.flake8-type-checking]
+exempt-modules = [
+    "typing",
+    "typing_extensions",
+]
+
+[tool.ruff.lint.flake8-unused-arguments]
+ignore-variadic-names = true
+
+[tool.ruff.lint.isort]
+case-sensitive = true
+required-imports = [
+    "from __future__ import annotations",
+]
+split-on-trailing-comma = false
 
-[tool.ruff.isort]
-force-wrap-aliases = true
-known-first-party = [
-    "snickerdoodle",
+[tool.ruff.lint.pydocstyle]
+convention = "google"
+ignore-decorators = [
+    "typing.overload",
 ]
```

### Comparing `snickerdoodle-0.1.9/PKG-INFO` & `snickerdoodle-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: snickerdoodle
-Version: 0.1.9
+Version: 0.2.0
 Summary: Easy-to-use, general-purpose, modern cookiecutter template for Python
 Author-Email: coreyrayburnyung <coreyrayburnyung@gmail.com>
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Pre-processors
 Project-URL: Documentation, https://WithPrecedent.github.io/snickerdoodle
 Project-URL: Repository, https://github.com/WithPrecedent/snickerdoodle
 Project-URL: Issues, https://github.com/WithPrecedent/snickerdoodle/issues
 Project-URL: Changelog, https://WithPrecedent.github.io/snickerdoodle/changelog
@@ -36,44 +37,44 @@
 | Documentation | [![Hosted By](https://img.shields.io/badge/hosted_by-GitHub_Pages-blue?style=for-the-badge&color=navy&logo=github)](https://withprecedent.github.io/snickerdoodle)
 | Compatibility | [![Compatible Python Versions](https://img.shields.io/pypi/pyversions/snickerdoodle?style=for-the-badge&color=steelblue&label=Python&logo=python&logoColor=yellow)](https://pypi.python.org/pypi/snickerdoodle/) [![Linux](https://img.shields.io/badge/Linux-lightseagreen?style=for-the-badge&logo=linux&labelColor=gray&logoColor=white)](https://www.linux.org/) [![MacOS](https://img.shields.io/badge/MacOS-snow?style=for-the-badge&logo=apple&labelColor=gray)](https://www.apple.com/macos/) [![Windows](https://img.shields.io/badge/windows-blue?style=for-the-badge&logo=Windows&labelColor=gray&color=orangered)](https://www.microsoft.com/en-us/windows?r=1)
 | Stats | [![PyPI Download Rate (per month)](https://img.shields.io/pypi/dm/snickerdoodle?style=for-the-badge&color=steelblue&label=Downloads%20💾&logo=pypi&logoColor=yellow)](https://pypi.org/project/snickerdoodle) [![GitHub Stars](https://img.shields.io/github/stars/withprecedent/snickerdoodle?style=for-the-badge&color=navy&label=Stars%20⭐&logo=github)](https://github.com/withprecedent/snickerdoodle/stargazers) [![GitHub Contributors](https://img.shields.io/github/contributors/withprecedent/snickerdoodle?style=for-the-badge&color=navy&label=Contributors%20🙋&logo=github)](https://github.com/withprecedent/snickerdoodle/graphs/contributors) [![GitHub Issues](https://img.shields.io/github/issues/withprecedent/snickerdoodle?style=for-the-badge&color=navy&label=Issues%20📘&logo=github)](https://github.com/withprecedent/snickerdoodle/graphs/contributors) [![GitHub Forks](https://img.shields.io/github/forks/withprecedent/snickerdoodle?style=for-the-badge&color=navy&label=Forks%20🍴&logo=github)](https://github.com/withprecedent/snickerdoodle/forks) |
 | | |
 
 ## What is snickerdoodle?
 
-`snickerdoodle`is an easy-to-use, general-purpose cookiecutter template for
+`snickerdoodle` is an easy-to-use, general-purpose cookiecutter template for
 Python projects utilizing modern tools and best practices. To see an example repository using this template,
 check out
 [`snickerdoodle_demo`](https://github.com/withprecedent/snickerdoodle_demo).
-  
+
 ## Why use snickerdoodle?
 
 There are a lot of cookiecutter templates. However, many are difficult to use,
 overly opinionated, or underdocumented. I created `snickerdoodle` because I
 couldn't
 find another `cookiecutter` template meeting these criteria:
 
-* **Modern**: follows best practices, using modern, actively developed tools
-* **Batteries Included**: allows you to start coding immediately
-* **Flexible**: no required usage of any external services
-  (SonarCloud, Travis, CircleCI, Tox, etc.)
+* **Modern**: follows best practices, using modern, actively developed tools.
+* **Batteries Included**: allows you to start coding immediately.
+* **Flexible**: no required usage of any external services.
+  (SonarCloud, Travis, CircleCI, Tox, etc.).
 * **Low-Maintenance**: every commit automatically deploys the documentation as
   well as
-  lints, formats, and tests the repository
+  lints, formats, and tests the repository.
 * **Well-Documented**: the
   [documentation](https://withprecedent.github.io/snickerdoodle) includes
-  complete guides for [new](https://withprecedent.github.io/snickerdoodle/tutorial/) and [advanced](https://withprecedent.github.io/snickerdoodle/advanced/) users
+  complete guides for [new](https://withprecedent.github.io/snickerdoodle/tutorial/) and [advanced](https://withprecedent.github.io/snickerdoodle/advanced/) users.
 * **PEP-Compliant**: all included tools follow accepted
   [PEPs](https://peps.python.org/pep-0001/) (unfortunately, that ruled out using
   `poetry`, which is [still not](https://github.com/python-poetry/roadmap/issues/3) [PEP 621](https://peps.python.org/pep-0621/) or
   [PEP 631](https://peps.python.org/pep-0631/)
   compliant, three years after they were accepted,
   [resulting in compatibility](https://github.com/python-poetry/poetry/issues/496)
   [problems because of its](https://github.com/python-poetry/poetry/issues/3332)
-  [non-standard `pyproject.toml` format](https://github.com/python-poetry/poetry/issues/8415))
+  [non-standard `pyproject.toml` format](https://github.com/python-poetry/poetry/issues/8415)).
 
 ### Tools
 
 To accomplish those goals, `snickerdoodle` includes modern, stable tools for package construction and
 management that do not require any external services or costs:
 
 * Dependency Management: [![Dependency Manager](https://img.shields.io/badge/PDM-mediumpurple?style=flat-square&logo=affinity&labelColor=gray)](https://PDM.fming.dev) and [![Dependency Maintainer](https://img.shields.io/badge/dependabot-navy?style=flat-square&logo=dependabot&logoColor=white&labelColor=gray)](https://github.com/dependabot)
@@ -140,17 +141,16 @@
 * [Repository Layout](https://withprecedent.github.io/snickerdoodle/advanced/#repository-layout)
 * [Versioning](https://withprecedent.github.io/snickerdoodle/advanced/#versioning)
 
 ## Contributing
 
 Contributors are always welcome and should find `snickerdoodle` easy to work
 with. The template is highly documented so that users and developers can adapt
-or extend`snickerdoodle` to work with their projects. So, forking and creating
-different template spins is encouraged. If you want to contribute directly to
-the project, feel free to grab an [issue](https://github.com/WithPrecedent/snickerdoodle/issues) to work on
+or extend `snickerdoodle` to work with their projects. So, forking and creating
+different template spins is encouraged. If you want to contribute directly, feel free to grab an [issue](https://github.com/WithPrecedent/snickerdoodle/issues) to work on
 or make a suggested improvement. If you wish to contribute, please read the
 [Contribution Guide](./contributing.md) and [Code of
 Conduct](./code_of_conduct.md).
 
 ## Similar Projects
 
 These are other `cookiecutter` templates using `pdm` as their dependency manager:
```


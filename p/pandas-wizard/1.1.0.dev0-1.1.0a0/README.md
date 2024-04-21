# Comparing `tmp/pandas-wizard-1.1.0.dev0.tar.gz` & `tmp/pandas-wizard-1.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-wizard-1.1.0.dev0.tar", last modified: Sat Apr 20 08:24:32 2024, max compression
+gzip compressed data, was "pandas-wizard-1.1.0a0.tar", last modified: Sun Apr 21 12:25:40 2024, max compression
```

## Comparing `pandas-wizard-1.1.0.dev0.tar` & `pandas-wizard-1.1.0a0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 08:24:32.549343 pandas-wizard-1.1.0.dev0/
--rw-rw-rw-   0        0        0     3423 2024-04-20 08:16:27.000000 pandas-wizard-1.1.0.dev0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2024-04-19 13:29:01.000000 pandas-wizard-1.1.0.dev0/LICENSE
--rw-rw-rw-   0        0        0      101 2024-04-19 13:29:01.000000 pandas-wizard-1.1.0.dev0/MANIFEST.in
--rw-rw-rw-   0        0        0     4018 2024-04-20 08:24:32.549343 pandas-wizard-1.1.0.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     2496 2024-04-19 18:51:23.000000 pandas-wizard-1.1.0.dev0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 08:24:32.545316 pandas-wizard-1.1.0.dev0/pandas_wizard.egg-info/
--rw-rw-rw-   0        0        0     4018 2024-04-20 08:24:31.000000 pandas-wizard-1.1.0.dev0/pandas_wizard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-04-20 08:24:32.000000 pandas-wizard-1.1.0.dev0/pandas_wizard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 08:24:31.000000 pandas-wizard-1.1.0.dev0/pandas_wizard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-20 08:24:31.000000 pandas-wizard-1.1.0.dev0/pandas_wizard.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-20 08:24:32.547326 pandas-wizard-1.1.0.dev0/pandaswizard/
--rw-rw-rw-   0        0        0      565 2024-04-20 08:08:39.000000 pandas-wizard-1.1.0.dev0/pandaswizard/__init__.py
--rw-rw-rw-   0        0        0    10798 2024-04-20 07:46:16.000000 pandas-wizard-1.1.0.dev0/pandaswizard/aggregate.py
--rw-rw-rw-   0        0        0       42 2024-04-20 08:24:32.550320 pandas-wizard-1.1.0.dev0/setup.cfg
--rw-rw-rw-   0        0        0     2045 2024-04-19 15:50:53.000000 pandas-wizard-1.1.0.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 12:25:40.045028 pandas-wizard-1.1.0a0/
+-rw-rw-rw-   0        0        0     4071 2024-04-21 12:11:57.000000 pandas-wizard-1.1.0a0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2024-04-19 13:29:01.000000 pandas-wizard-1.1.0a0/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-04-19 13:29:01.000000 pandas-wizard-1.1.0a0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5556 2024-04-21 12:25:40.044033 pandas-wizard-1.1.0a0/PKG-INFO
+-rw-rw-rw-   0        0        0     2548 2024-04-20 20:33:34.000000 pandas-wizard-1.1.0a0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 12:25:40.040037 pandas-wizard-1.1.0a0/pandas_wizard.egg-info/
+-rw-rw-rw-   0        0        0     5556 2024-04-21 12:25:39.000000 pandas-wizard-1.1.0a0/pandas_wizard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-04-21 12:25:39.000000 pandas-wizard-1.1.0a0/pandas_wizard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 12:25:39.000000 pandas-wizard-1.1.0a0/pandas_wizard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-21 12:25:39.000000 pandas-wizard-1.1.0a0/pandas_wizard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 12:25:40.043034 pandas-wizard-1.1.0a0/pandaswizard/
+-rw-rw-rw-   0        0        0      597 2024-04-21 12:12:43.000000 pandas-wizard-1.1.0a0/pandaswizard/__init__.py
+-rw-rw-rw-   0        0        0    11559 2024-04-21 09:43:53.000000 pandas-wizard-1.1.0a0/pandaswizard/aggregate.py
+-rw-rw-rw-   0        0        0     3456 2024-04-21 08:45:22.000000 pandas-wizard-1.1.0a0/pandaswizard/wrappers.py
+-rw-rw-rw-   0        0        0     1747 2024-04-21 12:25:07.000000 pandas-wizard-1.1.0a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-21 12:25:40.045028 pandas-wizard-1.1.0a0/setup.cfg
+-rw-rw-rw-   0        0        0     2199 2024-04-21 12:20:54.000000 pandas-wizard-1.1.0a0/setup.py
```

### Comparing `pandas-wizard-1.1.0.dev0/CHANGELOG.md` & `pandas-wizard-1.1.0a0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -47,21 +47,33 @@
   * 💣 - **Code Refactoring** : a breakable change often associated with `major` version bump.
 
 ### Version 1.0.0
 
 We're pleased to annouce the first major release and preview-built for **`pandaswizard`**! This version mainly focuses on enduser
 feedback and basic setup for the module.
 
+### Version 1.1.0a0 | Release Date:
+
+Moving from `development` release to `alpha` testing release, the version brings the additional new features and/or enhancements for
+the module:
+
+  * 🎉 Added **`pdw.wrappers`** module housing useful decorators,
+  * 🛠️ ([#7](https://github.com/sharkutilities/pandas-wizard/issues/7)) For legacy/`np < 1.22` try to return the aggregated
+    value using "interpolation" attribute.
+  * 🎉📃 Basic code documentation is now available, hosted using
+    [readthedocs/pandas-wizard](https://pandas-wizard.readthedocs.io/en/latest/index.html)
+
 ### Version 1.1.0.dev0 | Release Date: 20.04.2024
 
 Major enhancement of the preview built, also created an favicon and logo for the project. The logo is modified from the original
 pandas logo.
 
   * ⚙️ Added two new functions `__set_method__()` and `__calculate_quantile__()` to reduce code duplicacy,
-  * ✨ (#3) Added the ability to choose from either `pandas` or `numpy` to calculate grouped result:
+  * ✨ ([#3](https://github.com/sharkutilities/pandas-wizard/issues/3)) Added the ability to choose from either `pandas` or `numpy`
+    to calculate grouped result:
     - ✨ allows the user to choose any of the *method* to calculate based on `numpy` documentations,
     - 💣 numpy version requirement is `numpy >= 1.22` due to argument change `interpolation` to `method`
       more [details](https://github.com/numpy/numpy/issues/21283).
 
 #### Version 1.0.1.dev0 | Release Date: 19.04.2024
 
 The first `dev` or `preview-build` for `v1.0.0` focusing on function development and objective documentation. The version
```

### Comparing `pandas-wizard-1.1.0.dev0/LICENSE` & `pandas-wizard-1.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-wizard-1.1.0.dev0/README.md` & `pandas-wizard-1.1.0a0/README.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-<h1 align = "center">
-  <img alt = "favicon" src = "favicon.png" height = 250px><br>
-  pandas-wizard
-</h1>
-
-<div align = "justify">
-
-[**Pandas-Wizard (`pandaswizard`)**](https://github.com/sharkutilities/pandas-wizard) is a simple Python module for providing
-utility functions and wrappers for the `pandas` module. The module is kept simple and use of external dependencies is minimized
-unless needed to enhance performance.
-
-This is a relatively new repository, and if you find any performance or improvement scope please check the
-[contributing guidelines](https://github.com/sharkutilities/.github/blob/master/.github/CONTRIBUTING.md) for the organization.
-All help and criticism are appreciated. If you find any additional use cases please create a pull request or submit for a
-new feature.
-
-## Getting Started
-
-The source code is currently hosted at GitHub: [**sharkutilities/pandas-wizard**](https://github.com/sharkutilities/pandas-wizard).
-The binary installers for the latest release are available at the [Python Package Index (PyPI)](https://pypi.org/project/pandas-wizard/).
-
-```bash
-pip install -U pandas-wizard
-```
-
-The list of changes between each release is available [here](./CHANGELOG.md).
-
-The purpose of the below guide is to illustrate the main features of **pandas-wizard** and assume the working knowledge of
-the [`pandas`](https://pypi.org/project/pandas/) module and use cases. The below example calculates the percentile of
-`pandas.DataFrameGroupBy` object using [`np.percentile`](https://numpy.org/doc/stable/reference/generated/numpy.percentile.html).
-
-```python
-import pandaswizard as pdw # attempt to create an ubiquitous naming
-
-# let's calculate the 50th-percentile, i.e. the median for each group
-percentiles = df.groupby("group").agg({"A" : pdw.percentile(50)})
-percentiles.head()
-
-# or, preferred usage is to use in conjunture with other aggregation function like
-statistics = df.groupby("group").agg({"A" : [sum, pdw.percentile(50), pdw.quantile(0.95)]})
-statistics.head()
-```
-
-The above function calculates the 50th percentile, i.e., the median of the feature "A" based on the grouped column "group" from the data frame.
-
----
-
-**Footnote:** The [favicon](./favicon.png) is designed from the original [`pandas`](https://pandas.pydata.org/static/img/pandas.svg) logo and no
-copyright infringement is intended. Since the main objective is to provide a utility function for `pandas` the logo is re-used and developed
-using [canva](https://www.canva.com/).
-
-</div>
+<h1 align = "center">
+  <img alt = "favicon" src = "favicon.png" height = 250px><br>
+  pandas-wizard
+</h1>
+
+<div align = "justify">
+
+[**Pandas-Wizard (`pandaswizard`)**](https://github.com/sharkutilities/pandas-wizard) is a simple Python module for providing
+utility functions and wrappers for the `pandas` module. The module is kept simple and use of external dependencies is minimized
+unless needed to enhance performance.
+
+This is a relatively new repository, and if you find any performance or improvement scope please check the
+[contributing guidelines](https://github.com/sharkutilities/.github/blob/master/.github/CONTRIBUTING.md) for the organization.
+All help and criticism are appreciated. If you find any additional use cases please create a pull request or submit for a
+new feature.
+
+## Getting Started
+
+The source code is currently hosted at GitHub: [**sharkutilities/pandas-wizard**](https://github.com/sharkutilities/pandas-wizard).
+The binary installers for the latest release are available at the [Python Package Index (PyPI)](https://pypi.org/project/pandas-wizard/).
+
+```bash
+pip install -U pandas-wizard
+```
+
+The list of changes between each release is available [here](./CHANGELOG.md).
+
+The purpose of the below guide is to illustrate the main features of **pandas-wizard** and assume the working knowledge of
+the [`pandas`](https://pypi.org/project/pandas/) module and use cases. The below example calculates the percentile of
+`pandas.DataFrameGroupBy` object using [`np.percentile`](https://numpy.org/doc/stable/reference/generated/numpy.percentile.html).
+
+```python
+import pandaswizard as pdw # attempt to create an ubiquitous naming
+
+# let's calculate the 50th-percentile, i.e. the median for each group
+percentiles = df.groupby("group").agg({"A" : pdw.percentile(50)})
+percentiles.head()
+
+# or, preferred usage is to use in conjunture with other aggregation function like
+statistics = df.groupby("group").agg({"A" : [sum, pdw.percentile(50), pdw.quantile(0.95)]})
+statistics.head()
+```
+
+The above function calculates the 50th percentile, i.e., the median of the feature "A" based on the grouped column "group" from the data frame.
+
+---
+
+**Footnote:** The [favicon](./favicon.png) is designed from the original [`pandas`](https://pandas.pydata.org/static/img/pandas.svg) logo and no
+copyright infringement is intended. Since the main objective is to provide a utility function for `pandas` the logo is re-used and developed
+using [canva](https://www.canva.com/).
+
+</div>
```

### Comparing `pandas-wizard-1.1.0.dev0/pandaswizard/__init__.py` & `pandas-wizard-1.1.0a0/pandaswizard/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 The :mod:`pdwizard` module includes functions, wrappers and other
 utility functions for `pandas` module. The package is kept simple and
 minimalistic such that external dependencies are reduced.
 """
 
 # ? package follows https://peps.python.org/pep-0440/
 # ? https://python-semver.readthedocs.io/en/latest/advanced/convert-pypi-to-semver.html
-__version__ = "1.1.0.dev0"
+__version__ = "1.1.0a0"
 
 # init-time options registrations
 from pandaswizard.aggregate import (
     quantile,
     percentile
 )
+
+from pandaswizard import wrappers
```

### Comparing `pandas-wizard-1.1.0.dev0/pandaswizard/aggregate.py` & `pandas-wizard-1.1.0a0/pandaswizard/aggregate.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Utility Function(s) Related to a Grouped/Aggregated Data Frame
 
 The basic syntax for the groupby aggregation is `pd.groupby().agg({})`
 and the utility functions provided here can be applied under the
 aggregation section.
 """
 
+import warnings
 import numpy as np
 import pandas as pd
 
 def __set_method__(kwargs : dict) -> str:
     """
     Set "Method"/"Interpolation" Attribute for Aggregated Function(s)
 
@@ -73,16 +74,30 @@
                 True : np.nanquantile,
                 False : np.quantile
             }
         }
 
         try:
             retval = __func_dispatcher__[func][dropna](x, n, method = method)
-        except TypeError:
-            raise SystemError("This may be due to `np < 1.22`, https://github.com/numpy/numpy/issues/21283")
+        except TypeError as err:
+            __ref_issue = "https://github.com/numpy/numpy/issues/21283"
+            warnings.warn(
+                f"NumPy/np Version < 1.22, {__ref_issue} Error: {err}",
+                FutureWarning
+            )
+
+            # ? for older version, try with attribute `interpolation`, else
+            # ! this should not raise error, unless legacy numpy version, OR
+            # method/interpolation value is given for a newer version, not available
+            try:
+                retval = __func_dispatcher__[func][dropna](x, n, interpolation = method)
+            except Exception as err:
+                __warn_message = f"Cannot call attribute `method/interpolation` = {err}"
+                warnings.warn(f"{__warn_message}. Returning value w/o argument", SyntaxWarning)
+                retval = __func_dispatcher__[func][dropna](x, n)
 
     return retval
 
 
 def percentile(n : float, outname : str = None, **kwargs) -> float:
     """
     Compute the n-th Percentile for the Grouped Data Series
```

### Comparing `pandas-wizard-1.1.0.dev0/setup.py` & `pandas-wizard-1.1.0a0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 #
 # Copywright (C) 2024 Debmalya Pramanik <neuralNOD@gmail.com>
 # LICENSE: MIT License
 
 from setuptools import setup
 from setuptools import find_packages
 
-import pandaswizard
+import pandaswizard as pdw
 
 setup(
     name = "pandas-wizard",
-    version = pandaswizard.__version__,
+    version = pdw.__version__,
     author = "shark-utilities developers",
     author_email = "neuralNOD@outlook.com",
     description = "Utility Functions, Wrappers for pandas Module",
     long_description = open("README.md", "r").read(),
     long_description_content_type = "text/markdown",
     url = "https://github.com/sharkutilities/pandas-wizard",
     packages = find_packages(),
@@ -35,15 +35,17 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License"
     ],
     project_urls = {
-        "Issue Tracker" : "https://github.com/sharkutilities/pandas-wizard/issues"
+        "Issue Tracker" : "https://github.com/sharkutilities/pandas-wizard/issues",
+        "Code Documentations" : "https://pandas-wizard.readthedocs.io/en/latest/index.html",
+        "Org. Homepage" : "https://github.com/sharkutilities"
     },
     keywords = [
         # keywords for finding the package::
         "pandas", "utility", "utilities", "util", "utils",
         # keywords for finding the package relevant to usecases::
         "wrappers", "data science", "data analysis", "data scientist", "data analyst",
         # keywords as per available functionalities::
```


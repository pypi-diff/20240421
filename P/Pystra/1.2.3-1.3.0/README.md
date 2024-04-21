# Comparing `tmp/Pystra-1.2.3.tar.gz` & `tmp/pystra-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pystra-1.2.3.tar", last modified: Tue Sep 26 08:58:52 2023, max compression
+gzip compressed data, was "pystra-1.3.0.tar", last modified: Sun Apr 21 13:47:11 2024, max compression
```

## Comparing `Pystra-1.2.3.tar` & `pystra-1.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:58:52.772030 Pystra-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2023-09-26 08:58:41.000000 Pystra-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2023-09-26 08:58:52.772030 Pystra-1.2.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2869 2023-09-26 08:58:41.000000 Pystra-1.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2023-09-26 08:58:41.000000 Pystra-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-26 08:58:52.772030 Pystra-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-09-26 08:58:41.000000 Pystra-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:58:52.764030 Pystra-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:58:52.768030 Pystra-1.2.3/src/Pystra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2023-09-26 08:58:52.000000 Pystra-1.2.3/src/Pystra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2023-09-26 08:58:52.000000 Pystra-1.2.3/src/Pystra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 08:58:52.000000 Pystra-1.2.3/src/Pystra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-09-26 08:58:52.000000 Pystra-1.2.3/src/Pystra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-26 08:58:52.000000 Pystra-1.2.3/src/Pystra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:58:52.768030 Pystra-1.2.3/src/pystra/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    33813 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/correlation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:58:52.772030 Pystra-1.2.3/src/pystra/distributions/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/chisquare.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/gamma.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/gumbel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/lognormal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/parent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/scipydist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/shiftedexponential.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/shiftedrayleigh.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/typeiiismallestvalue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/typeiilargestvalue.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/typeilargestvalue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/typeismallestvalue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/weibull.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/distributions/zeroinflated.py
--rw-r--r--   0 runner    (1001) docker     (127)    12481 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/loadcomb.py
--rw-r--r--   0 runner    (1001) docker     (127)    20513 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/mc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7488 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/quadrature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)    13298 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/sorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2023-09-26 08:58:41.000000 Pystra-1.2.3/src/pystra/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:58:52.772030 Pystra-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2023-09-26 08:58:41.000000 Pystra-1.2.3/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    21273 2023-09-26 08:58:41.000000 Pystra-1.2.3/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2023-09-26 08:58:41.000000 Pystra-1.2.3/tests/test_ddm.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-09-26 08:58:41.000000 Pystra-1.2.3/tests/test_distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:47:11.156221 pystra-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-21 13:47:06.000000 pystra-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-21 13:47:11.156221 pystra-1.3.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2869 2024-04-21 13:47:06.000000 pystra-1.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-21 13:47:06.000000 pystra-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 13:47:11.156221 pystra-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-21 13:47:06.000000 pystra-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:47:11.148221 pystra-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:47:11.156221 pystra-1.3.0/src/Pystra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-21 13:47:11.000000 pystra-1.3.0/src/Pystra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-21 13:47:11.000000 pystra-1.3.0/src/Pystra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:47:11.000000 pystra-1.3.0/src/Pystra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-21 13:47:11.000000 pystra-1.3.0/src/Pystra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 13:47:11.000000 pystra-1.3.0/src/Pystra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:47:11.152221 pystra-1.3.0/src/pystra/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50933 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/correlation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:47:11.156221 pystra-1.3.0/src/pystra/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/chisquare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/gumbel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/lognormal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/parent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/scipydist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/shiftedexponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/shiftedrayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/typeiiismallestvalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/typeiilargestvalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/typeilargestvalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/typeismallestvalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/weibull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/distributions/zeroinflated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12481 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/loadcomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20513 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/mc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13298 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/sorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-21 13:47:06.000000 pystra-1.3.0/src/pystra/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:47:11.156221 pystra-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-21 13:47:06.000000 pystra-1.3.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-04-21 13:47:06.000000 pystra-1.3.0/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-21 13:47:06.000000 pystra-1.3.0/tests/test_ddm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-21 13:47:06.000000 pystra-1.3.0/tests/test_distribution.py
```

### Comparing `Pystra-1.2.3/LICENSE` & `pystra-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/PKG-INFO` & `pystra-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pystra
-Version: 1.2.3
+Version: 1.3.0
 Summary: Python Structural Reliability Analysis
 Author-email: Colin Caprani <colin.caprani@monash.edu>, "M. Shihab Khan" <shihab.khan@monash.edu>, Jürgen Hackl <hackl.science@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://pystra.github.io/pystra/
 Project-URL: Documentation, https://pystra.github.io/pystra/
 Project-URL: Source, https://github.com/pystra/pystra/
 Project-URL: Tracker, https://github.com/pystra/pystra/issues/
```

### Comparing `Pystra-1.2.3/README.rst` & `pystra-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/pyproject.toml` & `pystra-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/Pystra.egg-info/PKG-INFO` & `pystra-1.3.0/src/Pystra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pystra
-Version: 1.2.3
+Version: 1.3.0
 Summary: Python Structural Reliability Analysis
 Author-email: Colin Caprani <colin.caprani@monash.edu>, "M. Shihab Khan" <shihab.khan@monash.edu>, Jürgen Hackl <hackl.science@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://pystra.github.io/pystra/
 Project-URL: Documentation, https://pystra.github.io/pystra/
 Project-URL: Source, https://github.com/pystra/pystra/
 Project-URL: Tracker, https://github.com/pystra/pystra/issues/
```

### Comparing `Pystra-1.2.3/src/Pystra.egg-info/SOURCES.txt` & `pystra-1.3.0/src/Pystra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/analysis.py` & `pystra-1.3.0/src/pystra/analysis.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/calibration.py` & `pystra-1.3.0/src/pystra/calibration.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import pandas as pd
 from scipy.optimize import fsolve
 from .distributions import Constant
+from .model import LimitState, StochasticModel
+from .form import Form
+import matplotlib.pyplot as plt
 
 
 class Calibration:
-    r"""Class for calibrating partial and comination factors.
+    r"""Class for calibrating partial and combination factors.
 
     The factors are: :math:`\\phi`, :math:`\\gamma`, and :math:`\\psi`
     factors for a given load combination instance and target reliability.
 
     Attributes
     ----------
     betaT : float
@@ -25,15 +28,15 @@
     df_Xstar : DataFrame
         A dataframe of design point values
     df_phi : DataFrame
         A dataframe of partial factors for resistances
     df_gamma : DataFrame
         A dataframe of partial factors for loads
     df_psi : DataFrame
-        A dataframe of load combiantion factors
+        A dataframe of load combination factors
     dict_nom : dict
         Dictionary of nominal values
     est_method : str
         The estimation method
     label_comb_vrs : str
         Labels of combination variables
     label_comb_cases : str
@@ -973,7 +976,653 @@
         print("\n")
         print("=" * n)
         print("X* = \n", self.dfXstarcal.round(precision))
         print("\nphi = ", "\n", self.df_phi.round(precision))
         print("\ngamma =", "\n", self.df_gamma.round(precision))
         print("\npsi = ", "\n", self.df_psi.round(precision))
         print("=" * n)
+
+
+class GenericModel:
+    """
+    A probability model for generic calibration.
+    """
+
+    def __init__(self):
+        """
+        Initialize the class which holds all the probability model info.
+
+        Returns
+        -------
+        None.
+
+        """
+        self.phi = None
+        self.gamma_g = None
+        self.gamma_q = None
+        self.gamma_p = None
+        self.wR = None
+        self.wS = None
+        self.R = None
+        self.G = None
+        self.P = None
+        self.Q = None
+        self.Rk = None
+        self.Gk = None
+        self.Pk = None
+        self.Qk = None
+
+    def set_factors(self, phi, gamma_g, gamma_p, gamma_q):
+        """
+        Assign the partial factors to the generic probability model.
+
+        Parameters
+        ----------
+        phi : float
+            Capacity reduction factor.
+        gamma_g : float
+            Dead load factor.
+        gamma_p : float
+            Permanent load factor.
+        gamma_q : float
+            Live load factor.
+
+        Returns
+        -------
+        None.
+
+        """
+        self.phi = phi
+        self.gamma_g = gamma_g
+        self.gamma_p = gamma_p
+        self.gamma_q = gamma_q
+
+    def set_distributions(self, wR, wS, R, G, P, Q):
+        """
+        Assign the PySTRA distribution objects
+
+        Parameters
+        ----------
+        wR : PySTRA distribution object
+            Model error for resistance.
+        wS : PySTRA distribution object
+            Model error for loading/analysis.
+        R : PySTRA distribution object
+            Resistance distribution.
+        G : PySTRA distribution object
+            Dead load distribution.
+        P : PySTRA distribution object
+            Permanent load distribution.
+        Q : PySTRA distribution object
+            Live load distribution.
+
+        Returns
+        -------
+        None.
+
+        """
+        self.wR = wR
+        self.wS = wS
+        self.R = R
+        self.G = G
+        self.P = P
+        self.Q = Q
+
+    def set_nominals(self, Rk, Gk, Pk, Qk):
+        """
+        Set the nominal values of the parameters for use in design.
+
+        Parameters
+        ----------
+        Rk : float
+            Characteristic value of resistance.
+        Gk : float
+            Characteristic value of dead load.
+        Pk : float
+            Characteristic value of permanent load.
+        Qk : float
+            Characteristic value of live load.
+
+        Returns
+        -------
+        None.
+
+        """
+        self.Rk = Rk
+        self.Gk = Gk
+        self.Pk = Pk
+        self.Qk = Qk
+
+    def set_model_errors(self, wR, wS):
+        """
+        Set the model errors
+
+        Parameters
+        ----------
+        wR : PySTRA distribution object
+            Model error for resistance.
+        wS : PySTRA distribution object
+            Model error for loading/analysis.
+
+        Returns
+        -------
+        None.
+
+        """
+
+        self.wR = wR
+        self.wS = wS
+
+    def set_resistance_params(self, R, Rk, phi):
+        """
+        Set the resistance model parameters.
+
+        Parameters
+        ----------
+        R : PySTRA distribution object
+            Resistance distribution.
+        Rk : float
+            Characteristic value of resistance.
+        phi : float
+            Capacity reduction factor.
+
+        Returns
+        -------
+        None.
+
+        """
+
+        self.R = R
+        self.Rk = Rk
+        self.phi = phi
+
+    def set_dead_params(self, G, Gk, gamma_g):
+        """
+        Set the dead load model parameters.
+
+        Parameters
+        ----------
+        G : PySTRA distribution object
+            Dead load distribution.
+        Gk : float
+            Characteristic value of dead load.
+        gamma_g : float
+            Partial factor for dead load.
+
+        Returns
+        -------
+        None.
+
+        """
+
+        self.G = G
+        self.Gk = Gk
+        self.gamma_g = gamma_g
+
+    def set_permanent_params(self, P, Pk, gamma_p):
+        """
+        Set the permanent load model parameters.
+
+        Parameters
+        ----------
+        P : PySTRA distribution object
+            Permanent load distribution.
+        Pk : float
+            Characteristic value of permanent load.
+        gamma_p : float
+            Partial factor for permanent load.
+
+        Returns
+        -------
+        None.
+
+        """
+
+        self.P = P
+        self.Pk = Pk
+        self.gamma_p = gamma_p
+
+    def set_live_params(self, Q, Qk, gamma_q):
+        """
+        Set the dead load model parameters.
+
+        Parameters
+        ----------
+        Q : PySTRA distribution object
+            Live load distribution.
+        Qk : float
+            Characteristic value of live load.
+        gamma_q : float
+            Partial factor for live load.
+
+        Returns
+        -------
+        None.
+
+        """
+
+        self.Q = Q
+        self.Qk = Qk
+        self.gamma_q = gamma_q
+
+    def get(self):
+        """
+        Return a tuple of all the probability model parameters
+
+        Returns
+        -------
+        phi : float
+            Capacity reduction factor.
+        gamma_g : float
+            Dead load factor.
+        gamma_p : float
+            Permanent load factor.
+        gamma_q : float
+            Live load factor.
+        wR : PySTRA distribution object
+            Model error for resistance.
+        wS : PySTRA distribution object
+            Model error for loading/analysis.
+        R : PySTRA distribution object
+            Resistance distribution.
+        G : PySTRA distribution object
+            Dead load distribution.
+        P : PySTRA distribution object
+            Permanent load distribution.
+        Q : PySTRA distribution object
+            Live load distribution.
+        Rk : float
+            Characteristic value of resistance.
+        Gk : float
+            Characteristic value of dead load.
+        Pk : float
+            Characteristic value of permanent load.
+        Qk : float
+            Characteristic value of live load.
+
+        """
+        return (
+            self.phi,
+            self.gamma_g,
+            self.gamma_p,
+            self.gamma_q,
+            self.wR,
+            self.wS,
+            self.R,
+            self.G,
+            self.P,
+            self.Q,
+            self.Rk,
+            self.Gk,
+            self.Pk,
+            self.Qk,
+        )
+
+
+class GenericCalibration:
+    """
+    A generic code calibration
+    """
+
+    def __init__(self, aq_points, ag_points):
+        """
+        Initialize the generic code calibration class with the calculation points.
+
+        Parameters
+        ----------
+        q_points : nd.array
+            The grid of points to use for the live load ratio.
+        g_points : nd.array
+            The grid of points to use for the dead load ratio.
+
+        Returns
+        -------
+        None.
+
+        """
+        self.aq_points = aq_points
+        self.ag_points = ag_points
+        self.prob_models = []
+        self.is_analysed = False
+
+    def add_model(self, model, color, label):
+        """
+        Add a probability model to the calibration.
+
+        Parameters
+        ----------
+        model : GenericModel object
+            A probability model.
+        color : str
+            Matplotlib string representation of a colour for plotting.
+        label : str
+            Label for use in plot legend.
+
+        Returns
+        -------
+        None.
+
+        """
+        self.is_analysed = False
+        model_dict = {"model": model, "betas": None, "color": color, "label": label}
+        self.prob_models.append(model_dict)
+
+    def lsf(self, z, aq, ag, wR, R, wS, G, P, Q):
+        """
+        Limit state function for the generic code calibration problem.
+
+        Parameters
+        ----------
+        z : float
+            Design parameter.
+        aq : float
+            Ratio of dead to total dead and permanent load.
+        ag : float
+            Ratio of live to total loads.
+        wR : float
+            Model error for resistance.
+        R : float
+            Normalized resistance.
+        wS : float
+            Model error for loading/analysis.
+        G : float
+            Normalized dead load.
+        P : float
+            Normalized permanent load.
+        Q : float
+            Normalized live load.
+
+        Returns
+        -------
+        float
+            Evaluation of the limit state.
+
+        """
+        return z * wR * R - wS * ((1 - aq) * (ag * G + (1 - ag) * P) + aq * Q)
+
+    def design(self, aq, ag, phi, gamma_g, gamma_p, gamma_q, Rk, Gk, Pk, Qk):
+        """
+        Do a structural design for z, the design parameter, based on the code rules.
+
+        Parameters
+        ----------
+        aq : float
+            Ratio of dead to total dead and permanent load.
+        ag : float
+            Ratio of live to total loads.
+        phi : float
+            Capacity reduction factor.
+        gamma_g : float
+            Dead load factor.
+        gamma_p : float
+            Permanent load factor.
+        gamma_q : float
+            Live load factor.
+        Rk : float
+            Characteristic value of resistance.
+        Gk : float
+            Characteristic value of dead load.
+        Pk : float
+            Characteristic value of permanent load.
+        Qk : float
+            Characteristic value of live load.
+
+        Returns
+        -------
+        z : float
+            Design parameter.
+
+        """
+        z = (1 / (phi * Rk)) * (
+            (1 - aq) * (ag * gamma_g * Gk + (1 - ag) * gamma_p * Pk) + aq * gamma_q * Qk
+        )
+        return z
+
+    def analyse_design(self, z, aq, ag, wR, R, wS, G, P, Q):
+        """
+        Reliability analysis of the design according to the code rules.
+
+        Parameters
+        ----------
+        z : float
+            Design parameter.
+        aq : float
+            Ratio of dead to total dead and permanent load.
+        ag : float
+            Ratio of live to total loads.
+        wR : float
+            Model error for resistance.
+        R : float
+            Normalized resistance.
+        wS : float
+            Model error for loading/analysis.
+        G : float
+            Normalized dead load.
+        P : float
+            Normalized permanent load.
+        Q : float
+            Normalized live load.
+
+        Returns
+        -------
+        float
+            The reliability index, beta.
+
+        """
+        limit_state = LimitState(self.lsf)
+
+        stochastic_model = StochasticModel()
+        stochastic_model.addVariable(wR)
+        stochastic_model.addVariable(R)
+        stochastic_model.addVariable(wS)
+        stochastic_model.addVariable(G)
+        stochastic_model.addVariable(P)
+        stochastic_model.addVariable(Q)
+
+        stochastic_model.addVariable(Constant("z", z))
+        stochastic_model.addVariable(Constant("aq", aq))
+        stochastic_model.addVariable(Constant("ag", ag))
+
+        form = Form(
+            stochastic_model=stochastic_model,
+            limit_state=limit_state,
+        )
+        form.run()
+        return form.getBeta()
+
+    def get_reliabilities(self, Aq, Ag, model):
+        """
+        Determine the reliabilities across the full range of dead and live load ratios.
+
+        Parameters
+        ----------
+        Aq : nd.array
+            The grid of live load ratio points.
+        Ag : nd.array
+            The grid of dead load ratio points.
+        model : GenericModel
+            Probability model and code rules for analysis.
+
+        Returns
+        -------
+        beta : nd.array
+            Reliability indices at each dead and live load ratio grid point.
+
+        """
+        beta = np.zeros((Ag.size, Aq.size))
+        for i, ag in enumerate(Ag):
+            for j, aq in enumerate(Aq):
+                (
+                    phi,
+                    gamma_g,
+                    gamma_p,
+                    gamma_q,
+                    wR,
+                    wS,
+                    R,
+                    G,
+                    P,
+                    Q,
+                    Rk,
+                    Gk,
+                    Pk,
+                    Qk,
+                ) = model.get()
+                z = self.design(aq, ag, phi, gamma_g, gamma_p, gamma_q, Rk, Gk, Pk, Qk)
+                beta[i, j] = self.analyse_design(z, aq, ag, wR, R, wS, G, P, Q)
+        return beta
+
+    def analyse(self):
+        """
+        Analyse the code calibration problem given the probability models.
+
+        Raises
+        ------
+        ValueError
+            If there are no probability models assigned.
+
+        Returns
+        -------
+        None.
+
+        """
+        if not self.prob_models:
+            raise ValueError("No probability models assigned")
+
+        for pm in self.prob_models:
+            pm["betas"] = self.get_reliabilities(
+                self.aq_points, self.ag_points, pm["model"]
+            )
+
+        self.is_analysed = True
+
+    def add_range(self, ax, xl, xu, ytext, text, alpha):
+        def range_text(ax, x1, y1, x2, y2, text):
+            ax.annotate(
+                text="",
+                xy=(x1, y1),
+                xytext=(x2, y2),
+                arrowprops=dict(arrowstyle="<->", shrinkA=0, shrinkB=0),
+            )
+            ax.text(
+                x1 + (x2 - x1) / 2,
+                1.01 * y1 + (y2 - y1) / 2,
+                text,
+                ha="center",
+                va="bottom",
+            )
+
+        ax.axvspan(xl, xu, facecolor="k", alpha=alpha)
+        range_text(ax, xl, ytext, xu, ytext, text)
+
+    def plot_region(self, ax, x, beta, facecolor, label):
+        """
+        Plots a region of reliability indices, and adds a line for the smallest
+        dead load ratio.
+
+        Parameters
+        ----------
+        ax : Matplotlib Axes object
+            The axes to plot on.
+        x : nd.array
+            Vector of live load ratio points.
+        beta : nd.array
+            Matrix of reliability indices correspond go the dead and live ratios grid.
+        facecolor : str
+            Matplotlib string description of a colour.
+        label : str
+            Label for the plot legend.
+
+        Returns
+        -------
+        None.
+
+        """
+        ax.fill_between(
+            x,
+            beta.min(axis=0),
+            beta.max(axis=0),
+            alpha=0.5,
+            facecolor=facecolor,
+            label=label,
+        )
+        ax.plot(x, beta[-1], color=facecolor, ls=":")
+
+    def beta_region_plot(self, Aq, data, beta_t, ranges, figsize=(12, 9), **kwargs):
+        """
+        The main plotting function.
+
+        Parameters
+        ----------
+        Aq : nd.array
+            Vector of live load ratio points..
+        data : List[Dict{GemericModel}]
+            List of dictionaries of GenericModels, plotting info, and results.
+        beta_t : float
+            Target reliability index.
+        ranges : Dict
+            A dictionary of range information with the following keys:
+                xl, xu, ytext, text, alpha
+            defining the lower and upper aq values, the position of the text, the text,
+            and the alpha of the range colouring.
+        figsize : Tuple(float), optional
+            The figure size in inches. The default is (12, 9).
+
+        Returns
+        -------
+        fig : Matplotlib Figure object
+            The figure.
+        ax : Matplotlib Axes object
+            The axes.
+
+        """
+        x = Aq
+
+        fig, ax = plt.subplots(figsize=figsize, **kwargs)
+        ax.set_axisbelow(True)
+        ax.grid(which="both", ls=":", color="k")
+
+        if ranges:
+            for r in ranges:
+                self.add_range(ax, **r)
+
+        for d in data:
+            self.plot_region(ax, x, d["betas"], d["color"], d["label"])
+        ax.axhline(beta_t, color="k", ls="--")
+        t = ax.text(0.01, 0.99 * beta_t, rf"$\beta_T = {beta_t}$", ha="left", va="top")
+        t.set_bbox(dict(edgecolor="w", facecolor="w", alpha=0.8, pad=0))
+        ax.set_xlabel(r"Variable load ratio, $a_q = Q/(G+P+Q)$")
+        ax.set_ylabel(r"Reliability index, $\beta$")
+        ax.legend(loc="upper left")
+        return fig, ax
+
+    def plot(self, beta_t=4.7, ranges=None, **kwargs):
+        """
+        Plot the region for each probability model with their descriptions.
+
+        Parameters
+        ----------
+        beta_t : float
+            Target reliability index.
+        ranges : Dict
+            A dictionary of range information with the following keys:
+                xl, xu, ytext, text, alpha
+            defining the lower and upper aq values, the position of the text, the text,
+            and the alpha of the range colouring.
+
+        Raises
+        ------
+        ValueError
+            If there are no analysis results.
+
+        Returns
+        -------
+        fig,ax : Tuple(Matplotlib Figure, Matplotlib Axes)
+            The figure and axes.
+
+        """
+        if not self.is_analysed:
+            raise ValueError("Must be analysed before plotting")
+
+        return self.beta_region_plot(
+            self.aq_points, self.prob_models, beta_t, ranges, **kwargs
+        )
```

### Comparing `Pystra-1.2.3/src/pystra/correlation.py` & `pystra-1.3.0/src/pystra/correlation.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/__init__.py` & `pystra-1.3.0/src/pystra/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/beta.py` & `pystra-1.3.0/src/pystra/distributions/beta.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/chisquare.py` & `pystra-1.3.0/src/pystra/distributions/chisquare.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/distribution.py` & `pystra-1.3.0/src/pystra/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/gamma.py` & `pystra-1.3.0/src/pystra/distributions/gamma.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/gumbel.py` & `pystra-1.3.0/src/pystra/distributions/gumbel.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/lognormal.py` & `pystra-1.3.0/src/pystra/distributions/lognormal.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/maximum.py` & `pystra-1.3.0/src/pystra/distributions/maximum.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/normal.py` & `pystra-1.3.0/src/pystra/distributions/normal.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/parent.py` & `pystra-1.3.0/src/pystra/distributions/parent.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/scipydist.py` & `pystra-1.3.0/src/pystra/distributions/scipydist.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/shiftedexponential.py` & `pystra-1.3.0/src/pystra/distributions/shiftedexponential.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/shiftedrayleigh.py` & `pystra-1.3.0/src/pystra/distributions/shiftedrayleigh.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/typeiiismallestvalue.py` & `pystra-1.3.0/src/pystra/distributions/typeiiismallestvalue.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/typeiilargestvalue.py` & `pystra-1.3.0/src/pystra/distributions/typeiilargestvalue.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/typeilargestvalue.py` & `pystra-1.3.0/src/pystra/distributions/typeilargestvalue.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/typeismallestvalue.py` & `pystra-1.3.0/src/pystra/distributions/typeismallestvalue.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/uniform.py` & `pystra-1.3.0/src/pystra/distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/weibull.py` & `pystra-1.3.0/src/pystra/distributions/weibull.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/distributions/zeroinflated.py` & `pystra-1.3.0/src/pystra/distributions/zeroinflated.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/form.py` & `pystra-1.3.0/src/pystra/form.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/integration.py` & `pystra-1.3.0/src/pystra/integration.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/loadcomb.py` & `pystra-1.3.0/src/pystra/loadcomb.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/mc.py` & `pystra-1.3.0/src/pystra/mc.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/model.py` & `pystra-1.3.0/src/pystra/model.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/quadrature.py` & `pystra-1.3.0/src/pystra/quadrature.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/sensitivity.py` & `pystra-1.3.0/src/pystra/sensitivity.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/sorm.py` & `pystra-1.3.0/src/pystra/sorm.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/src/pystra/transformation.py` & `pystra-1.3.0/src/pystra/transformation.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/tests/test_basic.py` & `pystra-1.3.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/tests/test_calibration.py` & `pystra-1.3.0/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `Pystra-1.2.3/tests/test_ddm.py` & `pystra-1.3.0/tests/test_ddm.py`

 * *Files identical despite different names*


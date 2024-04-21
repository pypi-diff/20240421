# Comparing `tmp/moval-0.3.3.tar.gz` & `tmp/moval-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/zejuli/Local/Imperial/MOVAL/dist/.tmp-nkfy3qqo/moval-0.3.3.tar", last modified: Sun Apr 21 14:51:45 2024, max compression
+gzip compressed data, was "/Users/zejuli/Local/Imperial/MOVAL/dist/.tmp-w9opkzr1/moval-0.3.4.tar", last modified: Sun Apr 21 14:57:02 2024, max compression
```

## Comparing `moval-0.3.3.tar` & `moval-0.3.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 14:51:45.436104 moval-0.3.3/
--rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-21 14:51:45.436004 moval-0.3.3/PKG-INFO
--rw-r--r--   0 zejuli     (501) staff       (20)     2259 2024-01-19 15:02:41.000000 moval-0.3.3/README.md
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 14:51:45.432194 moval-0.3.3/moval/
--rw-r--r--   0 zejuli     (501) staff       (20)      706 2024-04-21 14:51:22.000000 moval-0.3.3/moval/__init__.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 14:51:45.433083 moval-0.3.3/moval/integrations/
--rw-r--r--   0 zejuli     (501) staff       (20)       68 2023-07-28 01:11:44.000000 moval-0.3.3/moval/integrations/__init__.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 14:51:45.433366 moval-0.3.3/moval/integrations/sklearn/
--rw-r--r--   0 zejuli     (501) staff       (20)      462 2023-10-26 14:28:12.000000 moval-0.3.3/moval/integrations/sklearn/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)    41094 2024-04-15 02:33:08.000000 moval-0.3.3/moval/integrations/sklearn/moval.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 14:51:45.434702 moval-0.3.3/moval/models/
--rw-r--r--   0 zejuli     (501) staff       (20)      447 2023-11-09 00:55:21.000000 moval-0.3.3/moval/models/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)     6840 2023-11-26 14:30:38.000000 moval-0.3.3/moval/models/confidences.py
--rw-r--r--   0 zejuli     (501) staff       (20)    44718 2024-04-17 02:22:33.000000 moval-0.3.3/moval/models/model.py
--rw-r--r--   0 zejuli     (501) staff       (20)     1631 2024-01-08 19:28:25.000000 moval-0.3.3/moval/models/solver_temperature.py
--rw-r--r--   0 zejuli     (501) staff       (20)    10804 2024-04-20 02:13:02.000000 moval-0.3.3/moval/models/utils.py
--rw-r--r--   0 zejuli     (501) staff       (20)    15406 2023-11-08 14:02:19.000000 moval-0.3.3/moval/registry.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 14:51:45.435446 moval-0.3.3/moval/solvers/
--rw-r--r--   0 zejuli     (501) staff       (20)      429 2023-11-09 00:58:57.000000 moval-0.3.3/moval/solvers/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)    11235 2024-04-15 02:36:06.000000 moval-0.3.3/moval/solvers/criterions.py
--rw-r--r--   0 zejuli     (501) staff       (20)    28955 2024-04-21 14:50:38.000000 moval-0.3.3/moval/solvers/solver.py
--rw-r--r--   0 zejuli     (501) staff       (20)     3054 2024-04-08 23:54:48.000000 moval-0.3.3/moval/solvers/utils.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 14:51:45.435670 moval-0.3.3/moval.egg-info/
--rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-21 14:51:45.000000 moval-0.3.3/moval.egg-info/PKG-INFO
--rw-r--r--   0 zejuli     (501) staff       (20)      553 2024-04-21 14:51:45.000000 moval-0.3.3/moval.egg-info/SOURCES.txt
--rw-r--r--   0 zejuli     (501) staff       (20)        1 2024-04-21 14:51:45.000000 moval-0.3.3/moval.egg-info/dependency_links.txt
--rw-r--r--   0 zejuli     (501) staff       (20)       61 2024-04-21 14:51:45.000000 moval-0.3.3/moval.egg-info/requires.txt
--rw-r--r--   0 zejuli     (501) staff       (20)        6 2024-04-21 14:51:45.000000 moval-0.3.3/moval.egg-info/top_level.txt
--rw-r--r--   0 zejuli     (501) staff       (20)    15479 2023-12-08 04:03:18.000000 moval-0.3.3/pyproject.toml
--rw-r--r--   0 zejuli     (501) staff       (20)      896 2024-04-21 14:51:45.436516 moval-0.3.3/setup.cfg
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 14:57:02.564825 moval-0.3.4/
+-rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-21 14:57:02.564768 moval-0.3.4/PKG-INFO
+-rw-r--r--   0 zejuli     (501) staff       (20)     2259 2024-01-19 15:02:41.000000 moval-0.3.4/README.md
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 14:57:02.561527 moval-0.3.4/moval/
+-rw-r--r--   0 zejuli     (501) staff       (20)      706 2024-04-21 14:56:33.000000 moval-0.3.4/moval/__init__.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 14:57:02.562485 moval-0.3.4/moval/integrations/
+-rw-r--r--   0 zejuli     (501) staff       (20)       68 2023-07-28 01:11:44.000000 moval-0.3.4/moval/integrations/__init__.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 14:57:02.562783 moval-0.3.4/moval/integrations/sklearn/
+-rw-r--r--   0 zejuli     (501) staff       (20)      462 2023-10-26 14:28:12.000000 moval-0.3.4/moval/integrations/sklearn/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    41094 2024-04-15 02:33:08.000000 moval-0.3.4/moval/integrations/sklearn/moval.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 14:57:02.563692 moval-0.3.4/moval/models/
+-rw-r--r--   0 zejuli     (501) staff       (20)      447 2023-11-09 00:55:21.000000 moval-0.3.4/moval/models/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     6840 2023-11-26 14:30:38.000000 moval-0.3.4/moval/models/confidences.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    44718 2024-04-17 02:22:33.000000 moval-0.3.4/moval/models/model.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     1631 2024-01-08 19:28:25.000000 moval-0.3.4/moval/models/solver_temperature.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    10804 2024-04-20 02:13:02.000000 moval-0.3.4/moval/models/utils.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    15406 2023-11-08 14:02:19.000000 moval-0.3.4/moval/registry.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 14:57:02.564346 moval-0.3.4/moval/solvers/
+-rw-r--r--   0 zejuli     (501) staff       (20)      429 2023-11-09 00:58:57.000000 moval-0.3.4/moval/solvers/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    11235 2024-04-15 02:36:06.000000 moval-0.3.4/moval/solvers/criterions.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    28951 2024-04-21 14:56:01.000000 moval-0.3.4/moval/solvers/solver.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     3054 2024-04-08 23:54:48.000000 moval-0.3.4/moval/solvers/utils.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 14:57:02.564528 moval-0.3.4/moval.egg-info/
+-rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-21 14:57:02.000000 moval-0.3.4/moval.egg-info/PKG-INFO
+-rw-r--r--   0 zejuli     (501) staff       (20)      553 2024-04-21 14:57:02.000000 moval-0.3.4/moval.egg-info/SOURCES.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)        1 2024-04-21 14:57:02.000000 moval-0.3.4/moval.egg-info/dependency_links.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)       61 2024-04-21 14:57:02.000000 moval-0.3.4/moval.egg-info/requires.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)        6 2024-04-21 14:57:02.000000 moval-0.3.4/moval.egg-info/top_level.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)    15479 2023-12-08 04:03:18.000000 moval-0.3.4/pyproject.toml
+-rw-r--r--   0 zejuli     (501) staff       (20)      896 2024-04-21 14:57:02.565148 moval-0.3.4/setup.cfg
```

### Comparing `moval-0.3.3/PKG-INFO` & `moval-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moval
-Version: 0.3.3
+Version: 0.3.4
 Summary: Model evaluation without manual labels
 Home-page: https://github.com/ZerojumpLine/MOVAL
 Author: Zeju Li
 Author-email: lizeju8@gmail.com
 Project-URL: Bug Tracker, https://github.com/ZerojumpLine/MOVAL/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moval Version: 0.3.3 Summary: Model evaluation
+Metadata-Version: 2.1 Name: moval Version: 0.3.4 Summary: Model evaluation
 without manual labels Home-page: https://github.com/ZerojumpLine/MOVAL Author:
 Zeju Li Author-email: lizeju8@gmail.com Project-URL: Bug Tracker, https://
 github.com/ZerojumpLine/MOVAL/issues Classifier: Development Status :: 3 -
 Alpha Classifier: Environment :: GPU :: NVIDIA CUDA Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: License :: Free
```

### Comparing `moval-0.3.3/README.md` & `moval-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `moval-0.3.3/moval/__init__.py` & `moval-0.3.4/moval/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 try:
     from moval.integrations.sklearn.moval import MOVAL
 except ImportError as e:
     # silently fail for now
     pass
 
-__version__ = "0.3.3"
+__version__ = "0.3.4"
 __all__ = ["MOVAL"]
 
 def __getattr__(key):
     """Lazy import of moval submodules and -packages.
 
     Once :py:mod:`moval` is imported, it is possible to lazy import
```

### Comparing `moval-0.3.3/moval/integrations/sklearn/moval.py` & `moval-0.3.4/moval/integrations/sklearn/moval.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.3/moval/models/confidences.py` & `moval-0.3.4/moval/models/confidences.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.3/moval/models/model.py` & `moval-0.3.4/moval/models/model.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.3/moval/models/solver_temperature.py` & `moval-0.3.4/moval/models/solver_temperature.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.3/moval/models/utils.py` & `moval-0.3.4/moval/models/utils.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.3/moval/registry.py` & `moval-0.3.4/moval/registry.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.3/moval/solvers/criterions.py` & `moval-0.3.4/moval/solvers/criterions.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.3/moval/solvers/solver.py` & `moval-0.3.4/moval/solvers/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,25 +442,25 @@
 
                         if optimization_result.fun > search_threshold:
                             # change the initial state, if we are not satisfied with the optimization results.
                             print(f"Not satisfied with initial optimization results of param_ext for class {opt_kcls}, trying more initial states...")
                             # change atc to be consistent with the range of confidence score
                             # get the max and min value here.
                             score = self.model.calibrate(inp, midstage = True)
+                            score_ = []
                             if self.model.mode == "classification":
                                 for kcls in range(self.batch * opt_kcls, np.min((self.batch * (opt_kcls + 1), self.model.num_class))):
                                     score_.append(score[np.argmax(inp, axis = 1) == kcls])
                                 score_ = np.concatenate(score_)
                                 initial_conditions_atc = [np.array([np.percentile(score_, 20)]), 
                                                             np.array([np.percentile(score_, 40)]), 
                                                             np.array([np.percentile(score_, 50)]), 
                                                             np.array([np.percentile(score_, 60)]), 
                                                             np.array([np.percentile(score_, 80)])]
                             else:
-                                score_ = []
                                 for n_case in range(len(inp)):
                                     score_flatten = score[n_case].flatten() # ``n``
                                     pred_flatten = np.argmax(inp[n_case], axis = 0).flatten()
                                     score_.append(score_flatten[pred_flatten == opt_kcls])
                                 score_ = np.concatenate(score_)
                                 initial_conditions_atc = [np.array([np.percentile(score_, 20)]), 
                                                             np.array([np.percentile(score_, 50)])]
```

### Comparing `moval-0.3.3/moval/solvers/utils.py` & `moval-0.3.4/moval/solvers/utils.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.3/moval.egg-info/PKG-INFO` & `moval-0.3.4/moval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moval
-Version: 0.3.3
+Version: 0.3.4
 Summary: Model evaluation without manual labels
 Home-page: https://github.com/ZerojumpLine/MOVAL
 Author: Zeju Li
 Author-email: lizeju8@gmail.com
 Project-URL: Bug Tracker, https://github.com/ZerojumpLine/MOVAL/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moval Version: 0.3.3 Summary: Model evaluation
+Metadata-Version: 2.1 Name: moval Version: 0.3.4 Summary: Model evaluation
 without manual labels Home-page: https://github.com/ZerojumpLine/MOVAL Author:
 Zeju Li Author-email: lizeju8@gmail.com Project-URL: Bug Tracker, https://
 github.com/ZerojumpLine/MOVAL/issues Classifier: Development Status :: 3 -
 Alpha Classifier: Environment :: GPU :: NVIDIA CUDA Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: License :: Free
```

### Comparing `moval-0.3.3/moval.egg-info/SOURCES.txt` & `moval-0.3.4/moval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moval-0.3.3/pyproject.toml` & `moval-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moval-0.3.3/setup.cfg` & `moval-0.3.4/setup.cfg`

 * *Files identical despite different names*


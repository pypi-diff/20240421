# Comparing `tmp/mlpro-int-sb3-0.1.1.tar.gz` & `tmp/mlpro_int_sb3-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpro-int-sb3-0.1.1.tar", last modified: Fri Apr  5 09:20:07 2024, max compression
+gzip compressed data, was "mlpro_int_sb3-1.0.0.tar", last modified: Sun Apr 21 15:10:25 2024, max compression
```

## Comparing `mlpro-int-sb3-0.1.1.tar` & `mlpro_int_sb3-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:20:07.417007 mlpro-int-sb3-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-05 09:19:59.000000 mlpro-int-sb3-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-05 09:20:07.417007 mlpro-int-sb3-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-05 09:19:59.000000 mlpro-int-sb3-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 09:19:59.000000 mlpro-int-sb3-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-05 09:20:07.421007 mlpro-int-sb3-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:20:07.413007 mlpro-int-sb3-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:20:07.417007 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:19:59.000000 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:20:07.417007 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 09:19:59.000000 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23250 2024-04-05 09:19:59.000000 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3/wrappers/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:20:07.417007 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-05 09:20:07.000000 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-05 09:20:07.000000 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:20:07.000000 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-05 09:20:07.000000 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 09:20:07.000000 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:20:07.417007 mlpro-int-sb3-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-05 09:19:59.000000 mlpro-int-sb3-0.1.1/test/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-04-05 09:19:59.000000 mlpro-int-sb3-0.1.1/test/test_sb3_policy_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:10:25.509834 mlpro_int_sb3-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-21 15:10:21.000000 mlpro_int_sb3-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-21 15:10:25.509834 mlpro_int_sb3-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-21 15:10:21.000000 mlpro_int_sb3-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-21 15:10:21.000000 mlpro_int_sb3-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-21 15:10:25.509834 mlpro_int_sb3-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:10:25.505834 mlpro_int_sb3-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:10:25.505834 mlpro_int_sb3-1.0.0/src/mlpro_int_sb3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 15:10:21.000000 mlpro_int_sb3-1.0.0/src/mlpro_int_sb3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:10:25.505834 mlpro_int_sb3-1.0.0/src/mlpro_int_sb3/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-21 15:10:21.000000 mlpro_int_sb3-1.0.0/src/mlpro_int_sb3/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23308 2024-04-21 15:10:21.000000 mlpro_int_sb3-1.0.0/src/mlpro_int_sb3/wrappers/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:10:25.505834 mlpro_int_sb3-1.0.0/src/mlpro_int_sb3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-21 15:10:25.000000 mlpro_int_sb3-1.0.0/src/mlpro_int_sb3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-21 15:10:25.000000 mlpro_int_sb3-1.0.0/src/mlpro_int_sb3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 15:10:25.000000 mlpro_int_sb3-1.0.0/src/mlpro_int_sb3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-21 15:10:25.000000 mlpro_int_sb3-1.0.0/src/mlpro_int_sb3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 15:10:25.000000 mlpro_int_sb3-1.0.0/src/mlpro_int_sb3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:10:25.505834 mlpro_int_sb3-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-21 15:10:21.000000 mlpro_int_sb3-1.0.0/test/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-04-21 15:10:21.000000 mlpro_int_sb3-1.0.0/test/test_sb3_policy_wrapper.py
```

### Comparing `mlpro-int-sb3-0.1.1/LICENSE` & `mlpro_int_sb3-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpro-int-sb3-0.1.1/PKG-INFO` & `mlpro_int_sb3-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: mlpro-int-sb3
-Version: 0.1.1
+Version: 1.0.0
 Summary: MLPro: Integration StableBaselines3
 Home-page: https://mlpro-int-sb3.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-sb3.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
-Requires-Dist: mlpro[full]>=1.3.1; extra == "full"
-Requires-Dist: mlpro_int_gymnasium>=0.1.0; extra == "full"
-Requires-Dist: stable_baselines3>=2.1.0; extra == "full"
-Requires-Dist: gymnasium>=0.29; extra == "full"
+Requires-Dist: mlpro[full]>=1.4.0; extra == "full"
+Requires-Dist: stable_baselines3>=2.3.0; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro-Int-SB3/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro-Int-SB3/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro-int-sb3/badge/?version=latest)](https://mlpro-int-sb3.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro-int-sb3.svg)](https://badge.fury.io/py/mlpro-int-sb3)
 <!---
 [![Anaconda-Version Badge](https://anaconda.org/mlpro-int-sb3/mlpro-int-sb3/badges/version.svg)](https://anaconda.org/mlpro-int-sb3/mlpro)
 [![Anaconda-Downloads Badge](https://img.shields.io/conda/dn/mlpro-int-sb3/mlpro-int-sb3?color=green&label=Anaconda.org%20Total%20downloads&style=flat-square)](https://anaconda.org/mlpro-int-pettingzoo/mlpro-int-pettingzoo)
 --->
-[![PyPI Total Downloads](https://static.pepy.tech/personalized-badge/mlpro-int-sb3?period=total&units=international_system&left_color=blue&right_color=orange&left_text=PyPI%20Total%20Downloads)](https://pepy.tech/project/mlpro-int-pettingzoo)
-[![PyPI Last Month Downloads](https://static.pepy.tech/personalized-badge/mlpro-int-sb3?period=month&units=international_system&left_color=blue&right_color=orange&left_text=PyPI%20Last%20Month%20Downloads)](https://pepy.tech/project/mlpro-int-pettingzoo)
+[![PyPI Total Downloads](https://static.pepy.tech/personalized-badge/mlpro-int-sb3?period=total&units=international_system&left_color=blue&right_color=orange&left_text=PyPI%20Total%20Downloads)](https://pepy.tech/project/mlpro-int-sb3)
+[![PyPI Last Month Downloads](https://static.pepy.tech/personalized-badge/mlpro-int-sb3?period=month&units=international_system&left_color=blue&right_color=orange&left_text=PyPI%20Last%20Month%20Downloads)](https://pepy.tech/project/mlpro-int-sb3)
 
 
 <img src="https://github.com/fhswf/MLPro-Int-SB3/blob/main/doc/logo/original/logo.png?raw=True" align="right" width="40%"/>
 
 # MLPro-Int-SB3 - Integration of Stable-Baselines3 into MLPro 
 Welcome to MLPro-Int-SB3, an extension to MLPro to integrate the Stable-Baselines3 package. MLPro is a middleware framework for standardized machine learning in Python. It is  developed by the South Westphalia University of Applied Sciences, Germany, and provides  standards, templates, and processes for hybrid machine learning applications. Stable-Baselines3, in turn, provides a diverse suite of reliable implementations of reinforcement learning algorithms in PyTorch.
```

### Comparing `mlpro-int-sb3-0.1.1/README.md` & `mlpro_int_sb3-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [![CI](https://github.com/fhswf/MLPro-Int-SB3/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro-Int-SB3/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro-int-sb3/badge/?version=latest)](https://mlpro-int-sb3.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro-int-sb3.svg)](https://badge.fury.io/py/mlpro-int-sb3)
 <!---
 [![Anaconda-Version Badge](https://anaconda.org/mlpro-int-sb3/mlpro-int-sb3/badges/version.svg)](https://anaconda.org/mlpro-int-sb3/mlpro)
 [![Anaconda-Downloads Badge](https://img.shields.io/conda/dn/mlpro-int-sb3/mlpro-int-sb3?color=green&label=Anaconda.org%20Total%20downloads&style=flat-square)](https://anaconda.org/mlpro-int-pettingzoo/mlpro-int-pettingzoo)
 --->
-[![PyPI Total Downloads](https://static.pepy.tech/personalized-badge/mlpro-int-sb3?period=total&units=international_system&left_color=blue&right_color=orange&left_text=PyPI%20Total%20Downloads)](https://pepy.tech/project/mlpro-int-pettingzoo)
-[![PyPI Last Month Downloads](https://static.pepy.tech/personalized-badge/mlpro-int-sb3?period=month&units=international_system&left_color=blue&right_color=orange&left_text=PyPI%20Last%20Month%20Downloads)](https://pepy.tech/project/mlpro-int-pettingzoo)
+[![PyPI Total Downloads](https://static.pepy.tech/personalized-badge/mlpro-int-sb3?period=total&units=international_system&left_color=blue&right_color=orange&left_text=PyPI%20Total%20Downloads)](https://pepy.tech/project/mlpro-int-sb3)
+[![PyPI Last Month Downloads](https://static.pepy.tech/personalized-badge/mlpro-int-sb3?period=month&units=international_system&left_color=blue&right_color=orange&left_text=PyPI%20Last%20Month%20Downloads)](https://pepy.tech/project/mlpro-int-sb3)
 
 
 <img src="https://github.com/fhswf/MLPro-Int-SB3/blob/main/doc/logo/original/logo.png?raw=True" align="right" width="40%"/>
 
 # MLPro-Int-SB3 - Integration of Stable-Baselines3 into MLPro 
 Welcome to MLPro-Int-SB3, an extension to MLPro to integrate the Stable-Baselines3 package. MLPro is a middleware framework for standardized machine learning in Python. It is  developed by the South Westphalia University of Applied Sciences, Germany, and provides  standards, templates, and processes for hybrid machine learning applications. Stable-Baselines3, in turn, provides a diverse suite of reliable implementations of reinforcement learning algorithms in PyTorch.
```

### Comparing `mlpro-int-sb3-0.1.1/setup.cfg` & `mlpro_int_sb3-1.0.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlpro-int-sb3
-version = 0.1.1
+version = 1.0.0
 author = MLPro Team
 author_email = mlpro@listen.fh-swf.de
 description = MLPro: Integration StableBaselines3
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mlpro-int-sb3.readthedocs.io
 project_urls = 
@@ -22,16 +22,14 @@
 include_package_data = True
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 full = 
-	mlpro[full]>=1.3.1
-	mlpro_int_gymnasium>=0.1.0
-	stable_baselines3>=2.1.0
-	gymnasium>=0.29
+	mlpro[full]>=1.4.0
+	stable_baselines3>=2.3.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mlpro-int-sb3-0.1.1/src/mlpro_int_sb3/wrappers/basics.py` & `mlpro_int_sb3-1.0.0/src/mlpro_int_sb3/wrappers/basics.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,32 +25,33 @@
 ## -- 2022-10-08  1.2.3     SY       Bug fixing
 ## -- 2022-11-02  1.2.4     DA       Refactoring: methods adapt(), _adapt()
 ## -- 2022-11-07  1.2.5     DA       Class WrPolicySB32MLPro: new parameter p_visualize
 ## -- 2023-02-16  1.2.6     SY       Bug fixing: observation_space recognization for integer
 ## -- 2023-04-19  1.2.7     MRD      Refactor module import gym to gymnasium
 ## -- 2023-09-25  1.2.8     DA       Set minimum version for sb3 to 2.1.0
 ## -- 2024-02-16  1.3.0     SY       Wrapper Relocation from MLPro to MLPro-Int-PettingZoo
+## -- 2024-04-19  1.4.0     DA       Alignment with MLPro 1.4.0
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.3.0 (2024-02-16)
+Ver. 1.4.0 (2024-04-19)
 
 This module provides wrapper classes for integrating stable baselines3 policy algorithms.
 
 See also: https://pypi.org/project/stable-baselines3/
 
 """
 
 
 import gymnasium as gym
 import torch
 import numpy as np
 from stable_baselines3.common import utils
 from stable_baselines3.common.on_policy_algorithm import OnPolicyAlgorithm
-from mlpro.wrappers.models import Wrapper
+from mlpro.wrappers import Wrapper
 from stable_baselines3.common.vec_env.base_vec_env import VecEnv, VecEnvStepReturn, VecEnvWrapper
 from stable_baselines3.common.vec_env import DummyVecEnv
 from stable_baselines3 import HerReplayBuffer
 from collections import OrderedDict
 from mlpro.rl import *
 from typing import Any, Dict, Optional, Union
 
@@ -148,15 +149,15 @@
         Number of environments, specifically for vectorized environment.
     p_desired_goals : list, Optional
         Desired state goals for Hindsight Experience Replay (HER).
     """
 
     C_TYPE              = 'Wrapper SB3 -> MLPro'
     C_WRAPPED_PACKAGE   = 'stable_baselines3'
-    C_MINIMUM_VERSION   = '2.1.0'
+    C_MINIMUM_VERSION   = '2.3.0'
 
 ## -------------------------------------------------------------------------------------------------
     def __init__(self, p_sb3_policy, p_cycle_limit, p_observation_space:MSpace,
                  p_action_space:MSpace, p_ada:bool=True, p_visualize:bool=False, 
                  p_logging=Log.C_LOG_ALL, p_num_envs:int=1, p_desired_goals=None):
         # Set Name
         WrPolicySB32MLPro.C_NAME = "Policy " + type(p_sb3_policy).__name__
```

### Comparing `mlpro-int-sb3-0.1.1/src/mlpro_int_sb3.egg-info/PKG-INFO` & `mlpro_int_sb3-1.0.0/src/mlpro_int_sb3.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: mlpro-int-sb3
-Version: 0.1.1
+Version: 1.0.0
 Summary: MLPro: Integration StableBaselines3
 Home-page: https://mlpro-int-sb3.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-sb3.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
-Requires-Dist: mlpro[full]>=1.3.1; extra == "full"
-Requires-Dist: mlpro_int_gymnasium>=0.1.0; extra == "full"
-Requires-Dist: stable_baselines3>=2.1.0; extra == "full"
-Requires-Dist: gymnasium>=0.29; extra == "full"
+Requires-Dist: mlpro[full]>=1.4.0; extra == "full"
+Requires-Dist: stable_baselines3>=2.3.0; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro-Int-SB3/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro-Int-SB3/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro-int-sb3/badge/?version=latest)](https://mlpro-int-sb3.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro-int-sb3.svg)](https://badge.fury.io/py/mlpro-int-sb3)
 <!---
 [![Anaconda-Version Badge](https://anaconda.org/mlpro-int-sb3/mlpro-int-sb3/badges/version.svg)](https://anaconda.org/mlpro-int-sb3/mlpro)
 [![Anaconda-Downloads Badge](https://img.shields.io/conda/dn/mlpro-int-sb3/mlpro-int-sb3?color=green&label=Anaconda.org%20Total%20downloads&style=flat-square)](https://anaconda.org/mlpro-int-pettingzoo/mlpro-int-pettingzoo)
 --->
-[![PyPI Total Downloads](https://static.pepy.tech/personalized-badge/mlpro-int-sb3?period=total&units=international_system&left_color=blue&right_color=orange&left_text=PyPI%20Total%20Downloads)](https://pepy.tech/project/mlpro-int-pettingzoo)
-[![PyPI Last Month Downloads](https://static.pepy.tech/personalized-badge/mlpro-int-sb3?period=month&units=international_system&left_color=blue&right_color=orange&left_text=PyPI%20Last%20Month%20Downloads)](https://pepy.tech/project/mlpro-int-pettingzoo)
+[![PyPI Total Downloads](https://static.pepy.tech/personalized-badge/mlpro-int-sb3?period=total&units=international_system&left_color=blue&right_color=orange&left_text=PyPI%20Total%20Downloads)](https://pepy.tech/project/mlpro-int-sb3)
+[![PyPI Last Month Downloads](https://static.pepy.tech/personalized-badge/mlpro-int-sb3?period=month&units=international_system&left_color=blue&right_color=orange&left_text=PyPI%20Last%20Month%20Downloads)](https://pepy.tech/project/mlpro-int-sb3)
 
 
 <img src="https://github.com/fhswf/MLPro-Int-SB3/blob/main/doc/logo/original/logo.png?raw=True" align="right" width="40%"/>
 
 # MLPro-Int-SB3 - Integration of Stable-Baselines3 into MLPro 
 Welcome to MLPro-Int-SB3, an extension to MLPro to integrate the Stable-Baselines3 package. MLPro is a middleware framework for standardized machine learning in Python. It is  developed by the South Westphalia University of Applied Sciences, Germany, and provides  standards, templates, and processes for hybrid machine learning applications. Stable-Baselines3, in turn, provides a diverse suite of reliable implementations of reinforcement learning algorithms in PyTorch.
```

### Comparing `mlpro-int-sb3-0.1.1/test/test_examples.py` & `mlpro_int_sb3-1.0.0/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `mlpro-int-sb3-0.1.1/test/test_sb3_policy_wrapper.py` & `mlpro_int_sb3-1.0.0/test/test_sb3_policy_wrapper.py`

 * *Files identical despite different names*


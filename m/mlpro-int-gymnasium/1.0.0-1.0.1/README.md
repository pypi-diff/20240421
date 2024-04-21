# Comparing `tmp/mlpro_int_gymnasium-1.0.0.tar.gz` & `tmp/mlpro_int_gymnasium-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpro_int_gymnasium-1.0.0.tar", last modified: Fri Apr 19 05:21:26 2024, max compression
+gzip compressed data, was "mlpro_int_gymnasium-1.0.1.tar", last modified: Sun Apr 21 13:29:39 2024, max compression
```

## Comparing `mlpro_int_gymnasium-1.0.0.tar` & `mlpro_int_gymnasium-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:26.721201 mlpro_int_gymnasium-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/boards/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/boards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/boards/multicartpole.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/envs/multicartpole.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22969 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/wrappers/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-19 05:21:26.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-19 05:21:26.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 05:21:26.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 05:21:26.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 05:21:26.000000 mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:21:26.725201 mlpro_int_gymnasium-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/test/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-19 05:21:22.000000 mlpro_int_gymnasium-1.0.0/test/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:29:39.729827 mlpro_int_gymnasium-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-21 13:29:35.000000 mlpro_int_gymnasium-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-21 13:29:39.729827 mlpro_int_gymnasium-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-21 13:29:35.000000 mlpro_int_gymnasium-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-21 13:29:35.000000 mlpro_int_gymnasium-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-21 13:29:39.729827 mlpro_int_gymnasium-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:29:39.721827 mlpro_int_gymnasium-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:29:39.725827 mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:29:35.000000 mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:29:39.725827 mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium/boards/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:29:35.000000 mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium/boards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-21 13:29:35.000000 mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium/boards/multicartpole.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:29:39.725827 mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:29:35.000000 mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-04-21 13:29:35.000000 mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium/envs/multicartpole.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:29:39.725827 mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-21 13:29:35.000000 mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23223 2024-04-21 13:29:35.000000 mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium/wrappers/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:29:39.725827 mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-21 13:29:39.000000 mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-21 13:29:39.000000 mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:29:39.000000 mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-21 13:29:39.000000 mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-21 13:29:39.000000 mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:29:39.725827 mlpro_int_gymnasium-1.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-21 13:29:35.000000 mlpro_int_gymnasium-1.0.1/test/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-21 13:29:35.000000 mlpro_int_gymnasium-1.0.1/test/test_examples.py
```

### Comparing `mlpro_int_gymnasium-1.0.0/LICENSE` & `mlpro_int_gymnasium-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpro_int_gymnasium-1.0.0/PKG-INFO` & `mlpro_int_gymnasium-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro-int-gymnasium
-Version: 1.0.0
+Version: 1.0.1
 Summary: MLPro: Integration Gymnasium
 Home-page: https://mlpro-int-gymnasium.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-gymnasium.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mlpro_int_gymnasium-1.0.0/README.md` & `mlpro_int_gymnasium-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mlpro_int_gymnasium-1.0.0/setup.cfg` & `mlpro_int_gymnasium-1.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlpro-int-gymnasium
-version = 1.0.0
+version = 1.0.1
 author = MLPro Team
 author_email = mlpro@listen.fh-swf.de
 description = MLPro: Integration Gymnasium
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mlpro-int-gymnasium.readthedocs.io
 project_urls =
```

### Comparing `mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/boards/multicartpole.py` & `mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium/boards/multicartpole.py`

 * *Files identical despite different names*

### Comparing `mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/envs/multicartpole.py` & `mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium/envs/multicartpole.py`

 * *Files identical despite different names*

### Comparing `mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium/wrappers/basics.py` & `mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium/wrappers/basics.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2023-04-09  0.0.0     MRD      Copied from openai_gym wrapper
 ## -- 2023-04-10  1.0.0     MRD      First Release 
 ## -- 2023-04-19  1.0.1     MRD      Refactor reset function
 ## -- 2023-08-21  1.0.2     MRD      Saving the seed in variable self._p_seed
 ## -- 2024-02-16  1.0.3     SY       Relocation from MLPro to MLPro-Int-Gymnasium
 ## -- 2024-04-19  1.0.4     DA       Alignment with MLPro 1.4.0
+## -- 2024-04-21  1.0.5     DA       Method WrEnvGYM2MLPro._complete_state(): recovery of render mode
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.0.4 (2024-04-19)
+Ver. 1.0.5 (2024-04-21)
 
 This module provides wrapper classes for Gym environments from Farama-Foundation Gymnasium.
 
 See also: https://github.com/Farama-Foundation/Gymnasium
 
 """
 
@@ -54,26 +55,27 @@
     C_TYPE              = 'Wrapper Gym2MLPro'
     C_WRAPPED_PACKAGE   = 'gymnasium'
     C_MINIMUM_VERSION   = '0.28.1'
     C_PLOT_ACTIVE: bool = True
 
 ## -------------------------------------------------------------------------------------------------
     def __init__(self,
-                 p_gym_env,  
+                 p_gym_env:gym.Env,  
                  p_state_space: MSpace = None,  
                  p_action_space: MSpace = None,  
                  p_seed=None,
                  p_visualize:bool=True,
                  p_logging=Log.C_LOG_ALL):
 
-        self._gym_env = p_gym_env
-        self._p_seed = p_seed
+        self._gym_env             = p_gym_env
+        self._p_seed              = p_seed
             
-        self._gym_env_id = self._gym_env.env.spec.id
-        self.C_NAME      = '(' + self._gym_env_id + ')'
+        self._gym_env_id          = self._gym_env.env.spec.id
+        self._gym_env_render_mode = self._gym_env.render_mode
+        self.C_NAME               = '(' + self._gym_env_id + ')'
 
         Environment.__init__(self, p_mode=Environment.C_MODE_SIM, p_latency=None, p_visualize=p_visualize, p_logging=p_logging)
         Wrapper.__init__(self, p_logging=p_logging)
 
         if p_state_space is not None:
             self._state_space = p_state_space
         else:
@@ -110,15 +112,15 @@
         """
 
         p_state['_gym_env'] = None
 
 
 ## -------------------------------------------------------------------------------------------------
     def _complete_state(self, p_path:str, p_os_sep:str, p_filename_stub:str):
-        self._gym_env = gym.make(self._gym_env_id)
+        self._gym_env = gym.make(self._gym_env_id, render_mode=self._gym_env_render_mode)
 
 
 ## -------------------------------------------------------------------------------------------------
     @staticmethod
     def recognize_space(p_gym_space) -> ESpace:
         """
         Detecting a gym space and transform it to MLPro space. Hence, the transformed space can be
```

### Comparing `mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium.egg-info/PKG-INFO` & `mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro-int-gymnasium
-Version: 1.0.0
+Version: 1.0.1
 Summary: MLPro: Integration Gymnasium
 Home-page: https://mlpro-int-gymnasium.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-gymnasium.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mlpro_int_gymnasium-1.0.0/src/mlpro_int_gymnasium.egg-info/SOURCES.txt` & `mlpro_int_gymnasium-1.0.1/src/mlpro_int_gymnasium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpro_int_gymnasium-1.0.0/test/test_environment.py` & `mlpro_int_gymnasium-1.0.1/test/test_environment.py`

 * *Files identical despite different names*

### Comparing `mlpro_int_gymnasium-1.0.0/test/test_examples.py` & `mlpro_int_gymnasium-1.0.1/test/test_examples.py`

 * *Files identical despite different names*


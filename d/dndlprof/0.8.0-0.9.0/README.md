# Comparing `tmp/dndlprof-0.8.0.tar.gz` & `tmp/dndlprof-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dndlprof-0.8.0.tar", last modified: Thu Feb 22 04:25:14 2024, max compression
+gzip compressed data, was "dndlprof-0.9.0.tar", last modified: Sun Apr 21 05:57:35 2024, max compression
```

## Comparing `dndlprof-0.8.0.tar` & `dndlprof-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:25:14.533308 dndlprof-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-22 04:25:06.000000 dndlprof-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-22 04:25:14.533308 dndlprof-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-22 04:25:06.000000 dndlprof-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:25:14.533308 dndlprof-0.8.0/dnd/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 04:25:06.000000 dndlprof-0.8.0/dnd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-02-22 04:25:06.000000 dndlprof-0.8.0/dnd/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-22 04:25:06.000000 dndlprof-0.8.0/dnd/bench.py
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-02-22 04:25:06.000000 dndlprof-0.8.0/dnd/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-02-22 04:25:06.000000 dndlprof-0.8.0/dnd/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-02-22 04:25:06.000000 dndlprof-0.8.0/dnd/nvtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-02-22 04:25:06.000000 dndlprof-0.8.0/dnd/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-02-22 04:25:06.000000 dndlprof-0.8.0/dnd/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-22 04:25:06.000000 dndlprof-0.8.0/dnd/sample_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-02-22 04:25:06.000000 dndlprof-0.8.0/dnd/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:25:14.533308 dndlprof-0.8.0/dndlprof.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-22 04:25:14.000000 dndlprof-0.8.0/dndlprof.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-02-22 04:25:14.000000 dndlprof-0.8.0/dndlprof.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 04:25:14.000000 dndlprof-0.8.0/dndlprof.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-22 04:25:14.000000 dndlprof-0.8.0/dndlprof.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-22 04:25:14.000000 dndlprof-0.8.0/dndlprof.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-22 04:25:14.000000 dndlprof-0.8.0/dndlprof.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 04:25:14.533308 dndlprof-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-02-22 04:25:06.000000 dndlprof-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:57:35.844272 dndlprof-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 05:57:28.000000 dndlprof-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-21 05:57:35.844272 dndlprof-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-21 05:57:28.000000 dndlprof-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:57:35.840272 dndlprof-0.9.0/dnd/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 05:57:28.000000 dndlprof-0.9.0/dnd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-21 05:57:28.000000 dndlprof-0.9.0/dnd/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-21 05:57:28.000000 dndlprof-0.9.0/dnd/bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-04-21 05:57:28.000000 dndlprof-0.9.0/dnd/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-21 05:57:28.000000 dndlprof-0.9.0/dnd/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-21 05:57:28.000000 dndlprof-0.9.0/dnd/nvtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-21 05:57:28.000000 dndlprof-0.9.0/dnd/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-21 05:57:28.000000 dndlprof-0.9.0/dnd/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-21 05:57:28.000000 dndlprof-0.9.0/dnd/sample_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-21 05:57:28.000000 dndlprof-0.9.0/dnd/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:57:35.844272 dndlprof-0.9.0/dndlprof.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-21 05:57:35.000000 dndlprof-0.9.0/dndlprof.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-21 05:57:35.000000 dndlprof-0.9.0/dndlprof.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 05:57:35.000000 dndlprof-0.9.0/dndlprof.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-21 05:57:35.000000 dndlprof-0.9.0/dndlprof.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-21 05:57:35.000000 dndlprof-0.9.0/dndlprof.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-21 05:57:35.000000 dndlprof-0.9.0/dndlprof.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 05:57:35.844272 dndlprof-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-21 05:57:28.000000 dndlprof-0.9.0/setup.py
```

### Comparing `dndlprof-0.8.0/LICENSE` & `dndlprof-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dndlprof-0.8.0/PKG-INFO` & `dndlprof-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dndlprof
-Version: 0.8.0
+Version: 0.9.0
 Summary: A simple tool for profiling and tracing PyTorch programs on NVIDIA GPUs
 Author: Michael Davies
 Author-email: michaelstoby@gmail.com
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: torch
```

### Comparing `dndlprof-0.8.0/README.md` & `dndlprof-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dndlprof-0.8.0/dnd/api.py` & `dndlprof-0.9.0/dnd/api.py`

 * *Files identical despite different names*

### Comparing `dndlprof-0.8.0/dnd/bench.py` & `dndlprof-0.9.0/dnd/bench.py`

 * *Files identical despite different names*

### Comparing `dndlprof-0.8.0/dnd/common.py` & `dndlprof-0.9.0/dnd/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import sys
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from distutils.spawn import find_executable
 import functools
 import json
 import yaml
 import subprocess
 import tempfile
 from contextlib import contextmanager
@@ -49,25 +49,27 @@
     if delete: os.remove(fname)
 
 dnd_config_file = get_optional_env('DND_CONFIG', '~/.dnd-config.yaml')
 
 @dataclass
 class GlobalConfig:
     ncu_replay_mode : str = 'application'
+    ncu_extra_cli : list[str] = field(default_factory=list)
     nsys_num_samples : int = 10
 
     @staticmethod
     def from_file(fname : str):
         with open(fname, 'r') as f:
             yd = yaml.safe_load(f)
 
         defconfig = GlobalConfig()
 
         return GlobalConfig(
             ncu_replay_mode=yd.get('ncu_replay_mode', defconfig.ncu_replay_mode),
+            ncu_extra_cli=yd.get('ncu_extra_cli', defconfig.ncu_extra_cli),
             nsys_num_samples=yd.get('nsys_num_samples', defconfig.nsys_num_samples)
         )
 
 dnd_config_file = os.path.expanduser(dnd_config_file)
 if os.path.exists(dnd_config_file):
     dnd_config = GlobalConfig.from_file(dnd_config_file)
 else:
```

### Comparing `dndlprof-0.8.0/dnd/env.py` & `dndlprof-0.9.0/dnd/env.py`

 * *Files identical despite different names*

### Comparing `dndlprof-0.8.0/dnd/nvtools.py` & `dndlprof-0.9.0/dnd/nvtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,19 +99,18 @@
     else:
         nvtx_args = []
 
     cmdline = [
         NCU_PATH,
         '--csv',
         *nvtx_args,
-        '--target-processes', 'all',
         '--profile-from-start', 'no' if use_cuda_profiler_api else 'yes',
         '--replay-mode', ncu_config.replay_mode,
         '--metrics', ','.join(ncu_config.metrics)
-    ] + prog_args
+    ] + dnd_config.ncu_extra_cli + prog_args
 
     with check_subprocess():
         ncu_output = subprocess.check_output(cmdline, env=ncu_env).decode()
 
     if not quiet:print('>>> Done!')
 
     return pd.read_csv(
```

### Comparing `dndlprof-0.8.0/dnd/reports.py` & `dndlprof-0.9.0/dnd/reports.py`

 * *Files identical despite different names*

### Comparing `dndlprof-0.8.0/dnd/run.py` & `dndlprof-0.9.0/dnd/run.py`

 * *Files identical despite different names*

### Comparing `dndlprof-0.8.0/dnd/tracer.py` & `dndlprof-0.9.0/dnd/tracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         return outs
 
 def trace_compile_fn(gm : torch.fx.GraphModule, args):
     def wrapper(*args, **kwargs):
         return KernelTracer(gm).run(*args, **kwargs)
 
-    return make_boxed_func(wrapper)
+    return wrapper
 
 def aot_compile_fn(gm : torch.fx.GraphModule, args):
     return aot_module(gm, trace_compile_fn)
 
 region_active = False
 
 @contextmanager
```

### Comparing `dndlprof-0.8.0/dndlprof.egg-info/PKG-INFO` & `dndlprof-0.9.0/dndlprof.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dndlprof
-Version: 0.8.0
+Version: 0.9.0
 Summary: A simple tool for profiling and tracing PyTorch programs on NVIDIA GPUs
 Author: Michael Davies
 Author-email: michaelstoby@gmail.com
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: torch
```

### Comparing `dndlprof-0.8.0/setup.py` & `dndlprof-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dndlprof',
-    version='0.8.0',
+    version='0.9.0',
     author='Michael Davies',
     author_email='michaelstoby@gmail.com',
     description='A simple tool for profiling and tracing PyTorch programs on NVIDIA GPUs',
     long_description=open('README.md').read(),
     packages=find_packages(),
     install_requires=['numpy', 'pandas', 'torch'],
     entry_points = {
```


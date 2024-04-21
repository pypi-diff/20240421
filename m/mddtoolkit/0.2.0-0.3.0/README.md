# Comparing `tmp/mddtoolkit-0.2.0.tar.gz` & `tmp/mddtoolkit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mddtoolkit-0.2.0.tar", last modified: Thu Jan  4 04:07:17 2024, max compression
+gzip compressed data, was "mddtoolkit-0.3.0.tar", last modified: Sun Apr 21 17:43:14 2024, max compression
```

## Comparing `mddtoolkit-0.2.0.tar` & `mddtoolkit-0.3.0.tar`

### file list

```diff
@@ -1,45 +1,40 @@
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-01-04 04:07:17.884182 mddtoolkit-0.2.0/
--rw-r--r--   0 josh       (501) staff       (20)     3140 2024-01-04 02:03:48.000000 mddtoolkit-0.2.0/.gitignore
--rw-r--r--   0 josh       (501) staff       (20)     1068 2023-12-30 17:21:08.000000 mddtoolkit-0.2.0/LISENCE
--rw-r--r--   0 josh       (501) staff       (20)     1641 2024-01-04 04:07:17.883906 mddtoolkit-0.2.0/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     1122 2024-01-04 01:34:22.000000 mddtoolkit-0.2.0/README.md
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-01-04 04:07:17.878123 mddtoolkit-0.2.0/example/
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-01-04 04:07:17.879546 mddtoolkit-0.2.0/example/beginner_users/
--rw-r--r--   0 josh       (501) staff       (20)      148 2024-01-04 01:38:33.000000 mddtoolkit-0.2.0/example/beginner_users/config.yaml
--rw-r--r--   0 josh       (501) staff       (20)     1415 2024-01-04 01:34:22.000000 mddtoolkit-0.2.0/example/beginner_users/sample_synthetic_data.csv
--rw-r--r--   0 josh       (501) staff       (20)      801 2024-01-04 03:58:24.000000 mddtoolkit-0.2.0/pyproject.toml
--rw-r--r--   0 josh       (501) staff       (20)       38 2024-01-04 04:07:17.884234 mddtoolkit-0.2.0/setup.cfg
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-01-04 04:07:17.878670 mddtoolkit-0.2.0/src/
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-01-04 04:07:17.879829 mddtoolkit-0.2.0/src/diffusion_kinetics/
--rw-r--r--   0 josh       (501) staff       (20)       22 2024-01-04 04:07:15.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)      646 2024-01-04 01:34:22.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/cli.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-01-04 04:07:17.880751 mddtoolkit-0.2.0/src/diffusion_kinetics/optimization/
--rw-r--r--   0 josh       (501) staff       (20)      202 2023-12-29 19:55:09.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/optimization/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     1200 2023-12-29 16:32:38.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/optimization/conHe_Param.py
--rw-r--r--   0 josh       (501) staff       (20)     1245 2023-12-29 16:32:38.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/optimization/dataset.py
--rw-r--r--   0 josh       (501) staff       (20)    11866 2024-01-04 01:34:22.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/optimization/diffusion_objective.py
--rw-r--r--   0 josh       (501) staff       (20)     3089 2024-01-04 01:34:22.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/optimization/diffusion_optimizer.py
--rw-r--r--   0 josh       (501) staff       (20)     7364 2024-01-04 01:34:22.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/optimization/forward_model_kinetics.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-01-04 04:07:17.881638 mddtoolkit-0.2.0/src/diffusion_kinetics/pipeline/
--rw-r--r--   0 josh       (501) staff       (20)      172 2023-12-29 16:32:38.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/pipeline/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     1658 2023-12-29 16:32:38.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/pipeline/base_pipeline.py
--rw-r--r--   0 josh       (501) staff       (20)     4724 2024-01-04 01:34:22.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/pipeline/multi_pipeline.py
--rw-r--r--   0 josh       (501) staff       (20)    15275 2024-01-04 01:34:22.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/pipeline/pipeline_config.py
--rw-r--r--   0 josh       (501) staff       (20)     3805 2024-01-04 01:34:22.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/pipeline/pipeline_output.py
--rw-r--r--   0 josh       (501) staff       (20)     3968 2024-01-04 01:34:22.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/pipeline/single_pipeline.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-01-04 04:07:17.881952 mddtoolkit-0.2.0/src/diffusion_kinetics/preprocessing/
--rw-r--r--   0 josh       (501) staff       (20)     7259 2024-01-04 01:34:22.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/preprocessing/calculate_experimental_results.py
--rw-r--r--   0 josh       (501) staff       (20)     2092 2024-01-04 01:34:22.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/preprocessing/generate_inputs.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-01-04 04:07:17.882446 mddtoolkit-0.2.0/src/diffusion_kinetics/utils/
--rw-r--r--   0 josh       (501) staff       (20)     1571 2023-12-30 17:21:08.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/utils/kinetics_dataframe.py
--rw-r--r--   0 josh       (501) staff       (20)     1504 2024-01-04 01:34:22.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/utils/organize_x.py
--rw-r--r--   0 josh       (501) staff       (20)     7992 2024-01-04 01:34:22.000000 mddtoolkit-0.2.0/src/diffusion_kinetics/utils/plot_results.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-01-04 04:07:17.883618 mddtoolkit-0.2.0/src/mddtoolkit.egg-info/
--rw-r--r--   0 josh       (501) staff       (20)     1641 2024-01-04 04:07:17.000000 mddtoolkit-0.2.0/src/mddtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     1340 2024-01-04 04:07:17.000000 mddtoolkit-0.2.0/src/mddtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2024-01-04 04:07:17.000000 mddtoolkit-0.2.0/src/mddtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (501) staff       (20)       59 2024-01-04 04:07:17.000000 mddtoolkit-0.2.0/src/mddtoolkit.egg-info/entry_points.txt
--rw-r--r--   0 josh       (501) staff       (20)       66 2024-01-04 04:07:17.000000 mddtoolkit-0.2.0/src/mddtoolkit.egg-info/requires.txt
--rw-r--r--   0 josh       (501) staff       (20)       19 2024-01-04 04:07:17.000000 mddtoolkit-0.2.0/src/mddtoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-01-04 04:07:17.883420 mddtoolkit-0.2.0/tests/
--rw-r--r--   0 josh       (501) staff       (20)     2208 2023-12-29 16:32:38.000000 mddtoolkit-0.2.0/tests/test_pipeline_config.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-04-21 17:43:14.776347 mddtoolkit-0.3.0/
+-rw-r--r--   0 josh       (501) staff       (20)     3128 2024-01-23 23:52:10.000000 mddtoolkit-0.3.0/.gitignore
+-rw-r--r--   0 josh       (501) staff       (20)     1068 2023-12-30 17:21:08.000000 mddtoolkit-0.3.0/LISENCE
+-rw-r--r--   0 josh       (501) staff       (20)     8216 2024-04-21 17:43:14.776087 mddtoolkit-0.3.0/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     7697 2024-04-21 17:30:31.000000 mddtoolkit-0.3.0/README.md
+-rw-r--r--   0 josh       (501) staff       (20)      716 2024-04-21 17:42:37.000000 mddtoolkit-0.3.0/pyproject.toml
+-rw-r--r--   0 josh       (501) staff       (20)       38 2024-04-21 17:43:14.776393 mddtoolkit-0.3.0/setup.cfg
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-04-21 17:43:14.771216 mddtoolkit-0.3.0/src/
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-04-21 17:43:14.771996 mddtoolkit-0.3.0/src/diffusion_kinetics/
+-rw-r--r--   0 josh       (501) staff       (20)      646 2024-01-04 01:34:22.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/cli.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-04-21 17:43:14.772882 mddtoolkit-0.3.0/src/diffusion_kinetics/optimization/
+-rw-r--r--   0 josh       (501) staff       (20)      202 2023-12-29 19:55:09.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/optimization/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     1200 2023-12-29 16:32:38.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/optimization/conHe_Param.py
+-rw-r--r--   0 josh       (501) staff       (20)     1245 2023-12-29 16:32:38.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/optimization/dataset.py
+-rw-r--r--   0 josh       (501) staff       (20)    11849 2024-01-24 00:01:22.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/optimization/diffusion_objective.py
+-rw-r--r--   0 josh       (501) staff       (20)     3089 2024-01-04 01:34:22.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/optimization/diffusion_optimizer.py
+-rw-r--r--   0 josh       (501) staff       (20)     7364 2024-01-04 01:34:22.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/optimization/forward_model_kinetics.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-04-21 17:43:14.773779 mddtoolkit-0.3.0/src/diffusion_kinetics/pipeline/
+-rw-r--r--   0 josh       (501) staff       (20)      172 2023-12-29 16:32:38.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/pipeline/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     1658 2023-12-29 16:32:38.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/pipeline/base_pipeline.py
+-rw-r--r--   0 josh       (501) staff       (20)     4728 2024-01-24 00:01:22.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/pipeline/multi_pipeline.py
+-rw-r--r--   0 josh       (501) staff       (20)    15314 2024-01-24 00:01:22.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/pipeline/pipeline_config.py
+-rw-r--r--   0 josh       (501) staff       (20)     3780 2024-01-24 00:01:22.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/pipeline/pipeline_output.py
+-rw-r--r--   0 josh       (501) staff       (20)     3968 2024-01-04 01:34:22.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/pipeline/single_pipeline.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-04-21 17:43:14.774069 mddtoolkit-0.3.0/src/diffusion_kinetics/preprocessing/
+-rw-r--r--   0 josh       (501) staff       (20)     7250 2024-01-24 00:01:22.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/preprocessing/calculate_experimental_results.py
+-rw-r--r--   0 josh       (501) staff       (20)     1683 2024-01-24 00:01:22.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/preprocessing/generate_inputs.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-04-21 17:43:14.774496 mddtoolkit-0.3.0/src/diffusion_kinetics/utils/
+-rw-r--r--   0 josh       (501) staff       (20)     1571 2023-12-30 17:21:08.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/utils/kinetics_dataframe.py
+-rw-r--r--   0 josh       (501) staff       (20)     1495 2024-01-24 00:01:22.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/utils/organize_x.py
+-rw-r--r--   0 josh       (501) staff       (20)    13254 2024-01-24 00:01:22.000000 mddtoolkit-0.3.0/src/diffusion_kinetics/utils/plot_results.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-04-21 17:43:14.775838 mddtoolkit-0.3.0/src/mddtoolkit.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)     8216 2024-04-21 17:43:14.000000 mddtoolkit-0.3.0/src/mddtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     1221 2024-04-21 17:43:14.000000 mddtoolkit-0.3.0/src/mddtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2024-04-21 17:43:14.000000 mddtoolkit-0.3.0/src/mddtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)       59 2024-04-21 17:43:14.000000 mddtoolkit-0.3.0/src/mddtoolkit.egg-info/entry_points.txt
+-rw-r--r--   0 josh       (501) staff       (20)       66 2024-04-21 17:43:14.000000 mddtoolkit-0.3.0/src/mddtoolkit.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)       19 2024-04-21 17:43:14.000000 mddtoolkit-0.3.0/src/mddtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-04-21 17:43:14.775657 mddtoolkit-0.3.0/tests/
+-rw-r--r--   0 josh       (501) staff       (20)     2208 2023-12-29 16:32:38.000000 mddtoolkit-0.3.0/tests/test_pipeline_config.py
```

### Comparing `mddtoolkit-0.2.0/.gitignore` & `mddtoolkit-0.3.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,14 @@
 
 # IPython
 profile_default/
 ipython_config.py
 
 /output/**
 /results/**
-/publish.sh
 
 # pyenv
 #   For a library or package, you might want to ignore these files since the code is
 #   intended to run in multiple environments; otherwise, check them in:
 # .python-version
 
 # pipenv
```

### Comparing `mddtoolkit-0.2.0/LISENCE` & `mddtoolkit-0.3.0/LISENCE`

 * *Files identical despite different names*

### Comparing `mddtoolkit-0.2.0/pyproject.toml` & `mddtoolkit-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name='mddtoolkit'
 requires-python = ">= 3.9"
-dynamic = ["version"]
+version='0.3.0'
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
@@ -27,12 +27,9 @@
 #url='https://github.com/dgorin1/diffusion_code_final'
 description='A package for modelling diffusion processes.'
 readme="README.md"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
-[tool.setuptools.dynamic]
-version = {attr = "diffusion_kinetics.__version__"}
-
 [project.scripts]
 mddtoolkit = "diffusion_kinetics.cli:main"
```

### Comparing `mddtoolkit-0.2.0/src/diffusion_kinetics/cli.py` & `mddtoolkit-0.3.0/src/diffusion_kinetics/cli.py`

 * *Files identical despite different names*

### Comparing `mddtoolkit-0.2.0/src/diffusion_kinetics/optimization/conHe_Param.py` & `mddtoolkit-0.3.0/src/diffusion_kinetics/optimization/conHe_Param.py`

 * *Files identical despite different names*

### Comparing `mddtoolkit-0.2.0/src/diffusion_kinetics/optimization/dataset.py` & `mddtoolkit-0.3.0/src/diffusion_kinetics/optimization/dataset.py`

 * *Files identical despite different names*

### Comparing `mddtoolkit-0.2.0/src/diffusion_kinetics/optimization/diffusion_objective.py` & `mddtoolkit-0.3.0/src/diffusion_kinetics/optimization/diffusion_objective.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,18 +56,15 @@
         self.lnd0aa = torch.tensor(self.dataset["ln(D/a^2)"])
         self.lnd0aa[-1] = 0
 
         indices = np.where(np.isinf(self.lnd0aa))
         self.lnd0aa[self.lnd0aa == -np.inf] = 0
         self.lnd0aa[self.lnd0aa == -np.inf] = 0
         self.lnd0aa[torch.isnan(self.lnd0aa)] = 0
-
-        self.omitValueIndices = torch.isin(
-            torch.arange(len(self.dataset)), torch.tensor(omitValueIndices)
-        ).to(torch.int)
+        self.omitValueIndices = torch.isin(   torch.arange(len(self.dataset)), torch.tensor(omitValueIndices)   ).to(torch.int)
         omitValueIndices_lnd0aa = omitValueIndices + (indices[0].tolist())
         self.omitValueIndices_lnd0aa = torch.isin(
             torch.arange(len(self.dataset)), torch.tensor(omitValueIndices_lnd0aa)
         ).to(torch.int)
 
         # Add locations where uncertainty (and measurement value) is zero to the list of values to ignore
         indices_chisq = np.where(data.uncert == 0)
```

### Comparing `mddtoolkit-0.2.0/src/diffusion_kinetics/optimization/diffusion_optimizer.py` & `mddtoolkit-0.3.0/src/diffusion_kinetics/optimization/diffusion_optimizer.py`

 * *Files identical despite different names*

### Comparing `mddtoolkit-0.2.0/src/diffusion_kinetics/optimization/forward_model_kinetics.py` & `mddtoolkit-0.3.0/src/diffusion_kinetics/optimization/forward_model_kinetics.py`

 * *Files identical despite different names*

### Comparing `mddtoolkit-0.2.0/src/diffusion_kinetics/pipeline/base_pipeline.py` & `mddtoolkit-0.3.0/src/diffusion_kinetics/pipeline/base_pipeline.py`

 * *Files identical despite different names*

### Comparing `mddtoolkit-0.2.0/src/diffusion_kinetics/pipeline/multi_pipeline.py` & `mddtoolkit-0.3.0/src/diffusion_kinetics/pipeline/multi_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,26 +14,26 @@
         self,
         output:Union[str, PipelineOutput]=None,
     ):
         self.output = MultiPipeline._create_output(output)
     
     def run(self, config:Union[str, dict, MultiProcessPipelineConfig], dataset:str):
         results = []
-        combined_df = None
         config = MultiPipeline._load_config(config)
         
         filename = Path(dataset).stem
         input_dataset = generate_inputs(dataset, self.output.get_generated_input_path(filename), config.geometry)
         self.dataset = MultiPipeline._load_dataset(input_dataset)
         
         pipeline = SinglePipeline(self.dataset, output=self.output)
         print("\n\033[1m\033[4mRunning multi pipeline with config:\033[0m")
         print(config, "\n")
         
         for misfit_type in config.single_pipeline_configs.keys():
+            combined_df = None
             print(f"{'='*80}", "\n\033[1mRunning pipeline for misfit type:", misfit_type, "\033[0m", f"\n{'='*80}")
             configs_for_each_domain_list = config.single_pipeline_configs[misfit_type]
             for single_pipeline_config in configs_for_each_domain_list:
                 print(f"\n\033[1m\033[4mFitting model with {single_pipeline_config.num_domains} domains\033[0m")
                 res = pipeline.run(single_pipeline_config)
                 # save the combined csv
                 if combined_df is None:
```

### Comparing `mddtoolkit-0.2.0/src/diffusion_kinetics/pipeline/pipeline_config.py` & `mddtoolkit-0.3.0/src/diffusion_kinetics/pipeline/pipeline_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         assert isinstance(self.geometry,str), "geometry must be a string"
         assert isinstance(self.omit_value_indices,list), "omit_value_indices must be a list"
         assert isinstance(self.max_iters,(float,int)), "max_iters must be a float or int"
         assert isinstance(self.punish_degas_early,bool), "punish_degas_early must be a bool"
         assert len(self.lnd0aa_bounds) == 2, "lnd0aa_bounds must be a list of length 2"
         assert len(self.ea_bounds) == 2, "ea_bounds must be a list of length 2"
         assert self.lnd0aa_bounds[0] < self.lnd0aa_bounds[1], "lnd0aa_bounds must be in increasing order"
-        assert self.ea_bounds[0] < self.ea_bounds[1], "ea_bounds must be in increasing order"        
+        assert self.ea_bounds[0] <= self.ea_bounds[1], "ea_bounds must be in increasing order, or equal to one another for fixed Ea"        
         assert self.geometry in ["spherical","plane sheet"], "geometry must be either 'spherical' or 'plane sheet'"
         assert self.max_iters > 0, "max_iters must be greater than 0"  
         assert self.num_domains >= 0, "num_domains must be greater than 0"
         assert self.misfit_stat in MISFIT_STAT_LIST, f"misfit_stat must be a valid misfit statistic. got {self.misfit_stat}"  
         assert self.repeat_iterations > 0, "repeat_iterations must be greater than 0"
         assert self.repeat_iterations == int(self.repeat_iterations), "repeat_iterations must be an integer"
         assert self.seed == None or self.seed == int(self.seed), "seed must be an integer"
```

### Comparing `mddtoolkit-0.2.0/src/diffusion_kinetics/pipeline/pipeline_output.py` & `mddtoolkit-0.3.0/src/diffusion_kinetics/pipeline/pipeline_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,10 +100,9 @@
         )
 
         plot_results(
             organize_x(results.x),
             dataset,
             objective,
             self.get_plot_path(config),
-            quiet=quiet,
         )
```

### Comparing `mddtoolkit-0.2.0/src/diffusion_kinetics/pipeline/single_pipeline.py` & `mddtoolkit-0.3.0/src/diffusion_kinetics/pipeline/single_pipeline.py`

 * *Files identical despite different names*

### Comparing `mddtoolkit-0.2.0/src/diffusion_kinetics/preprocessing/calculate_experimental_results.py` & `mddtoolkit-0.3.0/src/diffusion_kinetics/preprocessing/calculate_experimental_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,14 @@
             
             # If first step is < 0.85 (Ginster, 2018) 
             else:
                 DR2_uncert[0] = (1/(math.pi**2*cumtsec[0]*np.sum(M))) * np.sqrt(delM[0]**2 + (Fi[0]/(1-Fi[0]))**2 * np.sum(delM[1:]**2))
 
                 
         elif geometry == "plane sheet":
-        
             # Initialize D/r^2
             DR2_a = np.zeros([nstep])
             DR2_b = np.zeros([nstep])
 
             
             #Fechtig and Kalbitzer Equation 5a
             DR2_a[0] = ((((Fi[0]**2) - 0**2))*math.pi)/(4*tsec[0])
```

### Comparing `mddtoolkit-0.2.0/src/diffusion_kinetics/preprocessing/generate_inputs.py` & `mddtoolkit-0.3.0/src/diffusion_kinetics/preprocessing/generate_inputs.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,19 +34,8 @@
     expResults = D0calc_MonteCarloErrors(expData, geometry)
 
     # Combine the diffusion parameters with the experimental setup (T, thr, M, delM)
     # to get a final dataframe that will be passed into the optimizer
     diffusionExperimentResults = expData.join(expResults)
     # Write dataframe to a .csv file
     diffusionExperimentResults.to_csv(nameOfExperimentalResultsFile)
-    return diffusionExperimentResults
-
-
-# # main
-# if __name__ == "__main__":
-#     # generate some results
-#     dir_path = os.path.dirname(os.path.realpath(__file__))
-#     breakpoint()
-#     nameOfInputCSVFile = f"{dir_path}/N13ksp_python_test.csv"
-#     nameOfExperimentalResultsFile = f"{dir_path}/input_N13ksp_python_test.csv"
-#     geometry = "plane sheet"
-#     generate_inputs(nameOfInputCSVFile, nameOfExperimentalResultsFile, geometry)
+    return diffusionExperimentResults
```

### Comparing `mddtoolkit-0.2.0/src/diffusion_kinetics/utils/kinetics_dataframe.py` & `mddtoolkit-0.3.0/src/diffusion_kinetics/utils/kinetics_dataframe.py`

 * *Files identical despite different names*

### Comparing `mddtoolkit-0.2.0/src/diffusion_kinetics/utils/organize_x.py` & `mddtoolkit-0.3.0/src/diffusion_kinetics/utils/organize_x.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,20 +32,18 @@
         for j in range(0, n - i - 1):
             # Traverse the array from 0 to n-i-1
             # Swap if the element found is greater than the next element
             if lnd0aa[j] < lnd0aa[j + 1]:
                 lnd0aa[j], lnd0aa[j + 1] = lnd0aa[j + 1], lnd0aa[j]
                 fracs[j], fracs[j + 1] = fracs[j + 1], fracs[j]
 
-    if "moles" in locals():
+    if ~np.isnan(moles):
         output = np.append(moles, Ea)
     else:
         output = Ea
     output = np.append(output, lnd0aa)
     if chop_fracs == True:
         output = np.append(output, fracs[0:-1])
     else:
         output = np.append(output, fracs)
 
-    return output
-
-    
+    return output
```

### Comparing `mddtoolkit-0.2.0/src/mddtoolkit.egg-info/SOURCES.txt` & `mddtoolkit-0.3.0/src/mddtoolkit.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 .gitignore
 LISENCE
 README.md
 pyproject.toml
-example/beginner_users/config.yaml
-example/beginner_users/sample_synthetic_data.csv
-src/diffusion_kinetics/__init__.py
 src/diffusion_kinetics/cli.py
 src/diffusion_kinetics/optimization/__init__.py
 src/diffusion_kinetics/optimization/conHe_Param.py
 src/diffusion_kinetics/optimization/dataset.py
 src/diffusion_kinetics/optimization/diffusion_objective.py
 src/diffusion_kinetics/optimization/diffusion_optimizer.py
 src/diffusion_kinetics/optimization/forward_model_kinetics.py
```

### Comparing `mddtoolkit-0.2.0/tests/test_pipeline_config.py` & `mddtoolkit-0.3.0/tests/test_pipeline_config.py`

 * *Files identical despite different names*


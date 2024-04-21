# Comparing `tmp/teaspoon-1.4.8.tar.gz` & `tmp/teaspoon-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teaspoon-1.4.8.tar", last modified: Wed Jan 17 19:16:01 2024, max compression
+gzip compressed data, was "teaspoon-1.5.2.tar", last modified: Sun Apr 21 19:14:20 2024, max compression
```

## Comparing `teaspoon-1.4.8.tar` & `teaspoon-1.5.2.tar`

### file list

```diff
@@ -1,79 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:16:01.928588 teaspoon-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35142 2024-01-17 19:14:15.000000 teaspoon-1.4.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-01-17 19:16:01.928588 teaspoon-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-01-17 19:14:15.000000 teaspoon-1.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-01-17 19:14:17.000000 teaspoon-1.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-17 19:16:01.928588 teaspoon-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-01-17 19:14:17.000000 teaspoon-1.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:16:01.856587 teaspoon-1.4.8/teaspoon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:16:01.860587 teaspoon-1.4.8/teaspoon/teaspoon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:16:01.860587 teaspoon-1.4.8/teaspoon/teaspoon/ML/
--rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/ML/Base.py
--rw-r--r--   0 runner    (1001) docker     (127)    29657 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/ML/PD_Classification.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       77 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/ML/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:16:01.908587 teaspoon-1.4.8/teaspoon/teaspoon/ML/datasets/
--rw-r--r--   0 runner    (1001) docker     (127) 21567451 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/ML/datasets/mnist.pickle
--rw-r--r--   0 runner    (1001) docker     (127) 20646231 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/ML/datasets/mpeg7.pickle
--rw-r--r--   0 runner    (1001) docker     (127)  8765120 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/ML/datasets/shrec14.pickle
--rw-r--r--   0 runner    (1001) docker     (127)    41181 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/ML/feature_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/ML/load_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:16:01.920587 teaspoon-1.4.8/teaspoon/teaspoon/MakeData/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:16:01.924587 teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/DynSysLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/UserGuide.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37504 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/autonomous_dissipative_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/conservative_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/delayed_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    17123 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/driven_dissipative_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    23405 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/medical_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/noise_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/periodic_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21965 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/MakeData/PointCloud.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/MakeData/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:16:01.924587 teaspoon-1.4.8/teaspoon/teaspoon/SP/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/SP/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26581 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/SP/adaptivePart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:16:01.924587 teaspoon-1.4.8/teaspoon/teaspoon/SP/information/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/SP/information/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/SP/information/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/SP/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/SP/network_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    15592 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/SP/texture_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    27456 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/SP/tsa_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:16:01.924587 teaspoon-1.4.8/teaspoon/teaspoon/TDA/
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/TDA/Distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/TDA/Draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/TDA/PHN.py
--rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/TDA/Persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/TDA/SLSP.py
--rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/TDA/SLSP_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/TDA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/TDA/c_profile_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:16:01.928588 teaspoon-1.4.8/teaspoon/teaspoon/parameter_selection/
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/parameter_selection/FNN_n.py
--rw-r--r--   0 runner    (1001) docker     (127)    23996 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/parameter_selection/MI_delay.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/parameter_selection/MsPE.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/parameter_selection/PAMI_delay.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/parameter_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/parameter_selection/autocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-01-17 19:14:17.000000 teaspoon-1.4.8/teaspoon/teaspoon/parameter_selection/delay_LMS.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:16:01.928588 teaspoon-1.4.8/teaspoon/teaspoon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-01-17 19:16:01.000000 teaspoon-1.4.8/teaspoon/teaspoon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-01-17 19:16:01.000000 teaspoon-1.4.8/teaspoon/teaspoon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-17 19:16:01.000000 teaspoon-1.4.8/teaspoon/teaspoon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-17 19:16:01.000000 teaspoon-1.4.8/teaspoon/teaspoon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-17 19:16:01.000000 teaspoon-1.4.8/teaspoon/teaspoon.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:16:01.928588 teaspoon-1.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-01-17 19:14:17.000000 teaspoon-1.4.8/tests/test_MakeData.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-01-17 19:14:17.000000 teaspoon-1.4.8/tests/test_OrdinalPartition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-01-17 19:14:17.000000 teaspoon-1.4.8/tests/test_PointSummariesPHN.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-01-17 19:14:17.000000 teaspoon-1.4.8/tests/test_SLSP.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-01-17 19:14:17.000000 teaspoon-1.4.8/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-01-17 19:14:17.000000 teaspoon-1.4.8/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-01-17 19:14:17.000000 teaspoon-1.4.8/tests/test_featureFunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-01-17 19:14:17.000000 teaspoon-1.4.8/tests/test_parameterSelection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-01-17 19:14:17.000000 teaspoon-1.4.8/tests/test_signalProcessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-01-17 19:14:17.000000 teaspoon-1.4.8/tests/test_texture_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.193150 teaspoon-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35142 2024-04-21 19:13:08.000000 teaspoon-1.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-21 19:14:20.193150 teaspoon-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-21 19:13:08.000000 teaspoon-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-21 19:13:09.000000 teaspoon-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-21 19:14:20.193150 teaspoon-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-21 19:13:09.000000 teaspoon-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.117150 teaspoon-1.5.2/teaspoon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.121150 teaspoon-1.5.2/teaspoon/teaspoon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.121150 teaspoon-1.5.2/teaspoon/teaspoon/ML/
+-rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/Base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29657 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/PD_Classification.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       77 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.173150 teaspoon-1.5.2/teaspoon/teaspoon/ML/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127) 21567451 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/datasets/mnist.pickle
+-rw-r--r--   0 runner    (1001) docker     (127) 20646231 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/datasets/mpeg7.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)  8765120 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/datasets/shrec14.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)    51886 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/feature_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/load_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.185150 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.185150 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/
+-rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/DynSysLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/UserGuide.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37504 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/autonomous_dissipative_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/conservative_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/delayed_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17123 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/driven_dissipative_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23405 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/medical_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/noise_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/periodic_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21965 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/PointCloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.185150 teaspoon-1.5.2/teaspoon/teaspoon/SP/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/SP/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26581 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/SP/adaptivePart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.185150 teaspoon-1.5.2/teaspoon/teaspoon/SP/information/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/SP/information/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/SP/information/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/SP/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/SP/network_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15583 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/SP/texture_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27456 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/SP/tsa_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.189150 teaspoon-1.5.2/teaspoon/teaspoon/TDA/
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/Distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/Draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/Magnitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/PHN.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/Persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/SLSP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/SLSP_tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/c_profile_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.189150 teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/FNN_n.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23996 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/MI_delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/MsPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/PAMI_delay.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/autocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/delay_LMS.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.193150 teaspoon-1.5.2/teaspoon/teaspoon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-21 19:14:20.000000 teaspoon-1.5.2/teaspoon/teaspoon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-21 19:14:20.000000 teaspoon-1.5.2/teaspoon/teaspoon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-21 19:14:20.000000 teaspoon-1.5.2/teaspoon/teaspoon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-21 19:14:20.000000 teaspoon-1.5.2/teaspoon/teaspoon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 19:14:20.000000 teaspoon-1.5.2/teaspoon/teaspoon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.193150 teaspoon-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_MakeData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_OrdinalPartition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_PointSummariesPHN.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_SLSP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_featureFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_magnitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_parameterSelection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_signalProcessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_texture_analysis.py
```

### Comparing `teaspoon-1.4.8/LICENSE.txt` & `teaspoon-1.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/PKG-INFO` & `teaspoon-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teaspoon
-Version: 1.4.8
+Version: 1.5.2
 Summary: A Topological Signal Processing Package
 Author-email: Elizabeth Munch <muncheli@msu.edu>
 Project-URL: repository, https://github.com/TeaspoonTDA/teaspoon
 Project-URL: homepage, https://github.com/TeaspoonTDA/teaspoon
 Project-URL: documentation, https://teaspoontda.github.io/teaspoon/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -27,18 +27,19 @@
 Requires-Dist: scikit-learn>=1.1.1
 Requires-Dist: scipy>=1.8.1
 Requires-Dist: six>=1.16.0
 Requires-Dist: threadpoolctl>=3.1.0
 Requires-Dist: ripser>=0.6.4
 Requires-Dist: sympy>=1.11.1
 Requires-Dist: sortedcontainers>=2.4.0
-Requires-Dist: giotto-tda>=0.5.0
 Requires-Dist: persim
-Requires-Dist: pandas
+Requires-Dist: pandas>=1.4.1
 Requires-Dist: gudhi
+Requires-Dist: numba
+Requires-Dist: importlib_resources
 
 Description
 ==============
 
 The emerging field of topological signal processing brings methods from Topological Data Analysis (TDA) to create new tools for signal processing by incorporating aspects of shape.
 This python package, teaspoon for tsp or topological signal processing, brings together available software for computing persistent homology, the main workhorse of TDA, with modules that expand the functionality of teaspoon as a state-of-the-art topological signal processing tool.
 These modules include methods for incorporating tools from machine learning, complex networks, information, and parameter selection along with a dynamical systems library to streamline the creation and benchmarking of new methods.
```

### Comparing `teaspoon-1.4.8/README.md` & `teaspoon-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/pyproject.toml` & `teaspoon-1.5.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build]
 
 [project]
 name = "teaspoon"
-version = "1.4.8"
+version = "1.5.2"
 authors = [
   { name="Elizabeth Munch", email="muncheli@msu.edu" },
 ]
 description = "A Topological Signal Processing Package"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
@@ -30,18 +30,19 @@
                 "scikit-learn>=1.1.1",
                 "scipy>=1.8.1",
                 "six>=1.16.0",
                 "threadpoolctl>=3.1.0",
                 "ripser>=0.6.4", 
                 "sympy>=1.11.1",
                 "sortedcontainers>=2.4.0",
-                "giotto-tda>=0.5.0",
                 "persim",
-                "pandas",
-                "gudhi"
+                "pandas>=1.4.1",
+                "gudhi",
+                "numba",
+                "importlib_resources"
             ]
 
 [tool.setuptools.packages.find]
 where = ["teaspoon"]
 
 [tool.setuptools.package-data]
 teaspoon = ["ML/datasets/*.pickle"]
```

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/ML/Base.py` & `teaspoon-1.5.2/teaspoon/teaspoon/ML/Base.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/ML/PD_Classification.py` & `teaspoon-1.5.2/teaspoon/teaspoon/ML/PD_Classification.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/ML/datasets/mnist.pickle` & `teaspoon-1.5.2/teaspoon/teaspoon/ML/datasets/mnist.pickle`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/ML/datasets/mpeg7.pickle` & `teaspoon-1.5.2/teaspoon/teaspoon/ML/datasets/mpeg7.pickle`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/ML/datasets/shrec14.pickle` & `teaspoon-1.5.2/teaspoon/teaspoon/ML/datasets/shrec14.pickle`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/ML/feature_functions.py` & `teaspoon-1.5.2/teaspoon/teaspoon/ML/feature_functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 import math
 from math import pi
 from numpy.linalg import norm as lnorm
 from sympy.abc import t
 from sympy import Piecewise
 from sympy import diff, integrate
 from itertools import combinations
+from numba import guvectorize
+from sklearn import mixture
+import copy
 
 # -------------------------------------------- #
 # -------------------------------------------- #
 # ----------Featurization--------------------- #
 # -------------------------------------------- #
 # -------------------------------------------- #
 
@@ -358,14 +361,23 @@
     elif dgm_type == 'BirthLifetime':
         A = Dgm
     else:
         print('Your choices for type are "BirthDeath" or "BirthLifetime".')
         print('Exiting...')
         return
 
+    if params.partitions == None:
+        xmin = A[:, 0].min()
+        xmax = A[:, 0].max()
+        ymin = A[:, 1].min()
+        ymax = A[:, 1].max()
+    
+        box = {'nodes': np.array([xmin, xmax, ymin, ymax]), 'npts': A.shape[0]}
+        params.partitions = [box]
+
     # first, get the entries in Dgm that are within each partition
     for partition in params.partitions:
         query_Dgm_pts = getSubset(A, partition)
 
         # get the number of query points
         num_query_pts = len(query_Dgm_pts)
 
@@ -1148,8 +1160,283 @@
         id = index
         tid = labels
     for r in range(0,rows):
         for c in range(0,cols):
             img = ndimage.rotate(pers_img[id[i]], 90, reshape=True)
             axs[r,c].imshow(img)
             axs[r,c].set(xlabel='birth',ylabel='persistence',xticks=([]),yticks=([]), title=tid[i])
-            i += 1
+            i += 1
+
+@guvectorize(["void(float64[:,:,:], float64[:,:], float64, float64[:])",],"(p,m,n), (m,n), ()->(p)", target='parallel', nopython=True)
+def kernel_distance_parallel(dgms0, dgms1, sigma, result):
+    """
+
+    This function computes (in parallel) the multiscale heat kernel distance for an array of persistence diagrams based on the formula provided in Ref. :cite:`5 <Reininghaus2015>`.
+    There are three inputs and these are two persistence diagram arrays and the kernel scale sigma.  This function should be used for medium size datasets.    
+
+    Parameters
+    ----------
+    dgms0 : ndarray
+        Object array that includes first persistence diagram set.
+    dgms1 : ndarray
+        Object array that includes second persistence diagram set.
+    sigma : float
+        Kernel scale.
+
+    Returns
+    -------
+    result : np array
+        The kernel matrix
+
+    """
+    n_train = len(dgms0)
+    for i in range(n_train):
+        dgm0=dgms0[i]
+        dgm1 = dgms1
+        kSigma0 = 0
+        kSigma1 = 0
+        kSigma2 = 0
+        for k in range(dgm0.shape[0]):
+            p = dgm0[k,0:2]
+            if np.sum(p)==-2:
+                continue
+            for l in range(dgm0.shape[0]):
+                q = dgm0[l,0:2]
+                if np.sum(q)==-2:
+                    continue
+                qc = dgm0[l, 1::-1]
+                pq = (p[0] - q[0])**2 + (p[1] - q[1])**2
+                pqc = (p[0] - qc[0])**2 + (p[1] - qc[1])**2
+                kSigma0 += math.exp(-( pq) / (8 * sigma)) - math.exp(-(pqc) / (8 * sigma))
+        for k in range(dgm1.shape[0]):
+            p = dgm1[k,0:2]
+            if np.sum(p)==-2:
+                continue
+            for l in range(dgm1.shape[0]):
+                q = dgm1[l,0:2]
+                if np.sum(q)==-2:
+                    continue
+                qc = dgm1[l, 1::-1]
+                pq = (p[0] - q[0])**2 + (p[1] - q[1])**2
+                pqc = (p[0] - qc[0])**2 + (p[1] - qc[1])**2
+                kSigma1 += math.exp(-( pq) / (8 * sigma)) - math.exp(-(pqc) / (8 * sigma))
+        for k in range(dgm0.shape[0]):
+            p = dgm0[k,0:2]
+            if np.sum(p)==-2:
+                continue
+            for l in range(dgm1.shape[0]):
+                q = dgm1[l,0:2]
+                if np.sum(q)==-2:
+                    continue
+                qc = dgm1[l, 1::-1]
+                pq = (p[0] - q[0])**2 + (p[1] - q[1])**2
+                pqc = (p[0] - qc[0])**2 + (p[1] - qc[1])**2
+                kSigma2 += math.exp(-( pq) / (8 * sigma)) - math.exp(-(pqc) / (8 * sigma))
+
+        kSigma0 = kSigma0/(8 * np.pi * sigma)
+        kSigma1 = kSigma1/(8 * np.pi * sigma)
+        kSigma2 = kSigma2/(8 * np.pi * sigma)
+        result[i] = math.sqrt(kSigma1 + kSigma0-2*kSigma2)
+
+@guvectorize(["void(float64[:,:,:], float64[:,:], float64, float64[:])",],"(p,m,n), (m,n), ()->(p)", target='cpu', nopython=True)
+def kernel_distance(dgms0, dgms1, s, result):
+    """
+
+    This function computes the multiscale heat kernel distance for an array of persistence diagrams based on the formula provided in Ref. :cite:`5 <Reininghaus2015>`.
+    There are three inputs and these are two persistence diagram arrays and the kernel scale sigma.  This function should be used for small size datasets.  
+
+    Parameters
+    ----------
+    dgms0 : ndarray
+        Object array that includes first persistence diagram set.
+    dgms1 : ndarray
+        Object array that includes second persistence diagram set.
+    sigma : float
+        Kernel scale.
+
+    Returns
+    -------
+    result : np array
+        The kernel matrix
+
+    """
+    n_train = len(dgms0)
+    for i in range(n_train):
+        dgm0=dgms0[i]
+        dgm1 = dgms1
+        kSigma0 = 0
+        kSigma1 = 0
+        kSigma2 = 0
+        sigma = s
+        for k in range(dgm0.shape[0]):
+            p = dgm0[k,0:2]
+            if np.sum(p)==-2:
+                continue
+            for l in range(dgm0.shape[0]):
+                q = dgm0[l,0:2]
+                if np.sum(q)==-2:
+                    continue
+                qc = dgm0[l, 1::-1]
+                pq = (p[0] - q[0])**2 + (p[1] - q[1])**2
+                pqc = (p[0] - qc[0])**2 + (p[1] - qc[1])**2
+                kSigma0 += math.exp(-( pq) / (8 * sigma)) - math.exp(-(pqc) / (8 * sigma))
+        for k in range(dgm1.shape[0]):
+            p = dgm1[k,0:2]
+            if np.sum(p)==-2:
+                continue
+            for l in range(dgm1.shape[0]):
+                q = dgm1[l,0:2]
+                if np.sum(q)==-2:
+                    continue
+                qc = dgm1[l, 1::-1]
+                pq = (p[0] - q[0])**2 + (p[1] - q[1])**2
+                pqc = (p[0] - qc[0])**2 + (p[1] - qc[1])**2
+                kSigma1 += math.exp(-( pq) / (8 * sigma)) - math.exp(-(pqc) / (8 * sigma))
+        for k in range(dgm0.shape[0]):
+            p = dgm0[k,0:2]
+            if np.sum(p)==-2:
+                continue
+            for l in range(dgm1.shape[0]):
+                q = dgm1[l,0:2]
+                if np.sum(q)==-2:
+                    continue
+                qc = dgm1[l, 1::-1]
+                pq = (p[0] - q[0])**2 + (p[1] - q[1])**2
+                pqc = (p[0] - qc[0])**2 + (p[1] - qc[1])**2
+                kSigma2 += math.exp(-( pq) / (8 * sigma)) - math.exp(-(pqc) / (8 * sigma))
+
+        kSigma0 = kSigma0/(8 * np.pi * sigma)
+        kSigma1 = kSigma1/(8 * np.pi * sigma)
+        kSigma2 = kSigma2/(8 * np.pi * sigma)
+        result[i] = math.sqrt(kSigma1 + kSigma0-2*kSigma2)
+
+def f_dgm(dgm, function, **keyargs):
+	'''
+	Given a persistence diagram :math:`D = (S,\mu)` and a compactly supported function in :math:`\mathbb{R}^2`, this function computes
+	.. math::
+		\\nu_{D}(f) = \sum_{x\in S} f(x)\mu(x)
+	:param dgm: persistent diagram, array of points in :math:`\mathbb{R}^2`.
+	:type dgm: Numpy array
+	:param function: Compactly supported function in :math:`\mathbb{R}^2`.
+	:type function: function
+	:param keyargs: Additional arguments required by `funciton`
+	:type keyargs: Dicctionary
+	:return: float -- value of :math:`\\nu_{D}(f)`.
+	'''
+
+	temp = function(dgm, **keyargs)
+
+	return sum(temp)
+
+def f_ellipse (x, center=np.array([0,0]), axis=np.array([1,1]), rotation=np.array([[1,0],[0,1]])):
+	'''
+	Computes a bump function centered with an ellipsoidal domain centered ac `c`, rotaded by 'rotation' and with axis given by 'axis'. The bump function is computed using the gollowing formula 
+	.. math::
+		f_{A,c} (x) = \max \\left\{ 0, 1 - (x - c)^T A (x - c)\\right\}
+	:param x: point to avelatuate the function :math:`f_{A,c}`
+	:type z: Numpy array
+	:param center: center of the ellipse
+	:type center: Numpy array
+	:param axis: Size f themjor an minor axis of the ellipse
+	:type axis: Numpy array
+	:param rotation: Rotation matrix for the ellipse
+	:type rotation: Numpy array
+	:return: float -- value of :math:`f_{A,c} (x)`.
+	'''
+	sigma = np.diag(np.power(axis, -2))
+	x_centered = np.subtract(x, center)
+	temp = x_centered@rotation@sigma@np.transpose(rotation)@np.transpose(x_centered)
+	temp = np.diag(temp)
+
+	return np.maximum(0, 1-temp)
+def adaptive_feature(list_dgms, function, **keyargs):
+	'''
+	Given a collection of persistent diagrams and a compactly supported function in :math:`\mathbb{R}^2`, computes :math:`\\nu_{D}(f)` for each diagram :math:`D` in the collection.
+	:param list_dgms: list of persistent diagrams
+	:type list_dgms: list
+	:param function: Compactly supported function in :math:`\mathbb{R}^2`.
+	:type function: function
+	:param keyargs: Additional arguments required by `funciton`
+	:type keyargs: Dicctionary
+	:return: Numpy array -- Array of values :math:`\\nu_{D}(f)` for each diagram :math:`D` in the collection `list_dgms`.
+	'''
+	num_diagrams = len(list_dgms)
+
+	feat = np.zeros(num_diagrams)
+	for i in range(num_diagrams):
+		feat[i] = f_dgm(list_dgms[i], function, **keyargs)
+
+	return feat
+
+def adaptive_template_functions(train_dgms, d=25, threshold=.05):
+    """
+
+    This function computes adaptive template functions as in the paper :cite:`6 <polanco2019adaptive>` from a training set and returns the ellipses needed to fit features to a training and testing dataset.
+
+    Parameters
+    ----------
+    train_dgms : ndarray
+        Object array that includes training diagrams
+    d : integer
+        maximum number of functions.
+    threshold: float
+        cutoff for inclusion as
+
+    Returns
+    -------
+    ellipses : list
+        list of ellipses that are the adaptive template functions
+
+    """
+	#### Combine all diagrams
+    X_train_temp = np.vstack(train_dgms)
+	### return means for scoring
+    gmm = mixture.BayesianGaussianMixture(n_components=d, covariance_type='full', max_iter=int(10e4)).fit(X_train_temp)
+    ellipses = []
+    for i in range(len(gmm.means_)):
+        L, v = np.linalg.eig(gmm.covariances_[i])
+        temp = {'mean':gmm.means_[i], 'std':np.sqrt(L), 'rotation':v.transpose(), 'radius':max(np.sqrt(L)), 'entropy':gmm.weights_[i]}
+        temp['std'] = 3*temp['std']
+        ellipses.append(temp)
+
+    return ellipses
+
+def adaptive_template_features(list_dgms, list_ellipses, function=f_ellipse):
+	'''
+	This function computes all the features for a collection of persistent diagrams given a list ot ellipses.
+	:param list_dgms: list of persistent diagrams
+	:type list_dgms: list
+	:param list_ellipses: List of dicctionaries. Each dicctionary represents a ellipse. It must have the following keys: `mean`, `std` and `rotation`.
+	:type list_ellipses: list
+	:param function: Compactly supported function in :math:`\mathbb{R}^2`.
+	:type function: function
+	:return: Numpy array -- 
+	'''
+	features = np.zeros((len(list_dgms), len(list_ellipses)))
+	for i in range(len(list_ellipses)):
+		args = {key:list_ellipses[i][key] for key in ['mean', 'std', 'rotation']}
+		args['center'] = args.pop('mean')
+		args['axis'] = args.pop('std')
+
+		features[:,i] = adaptive_feature(list_dgms, function, **args)
+
+	return features
+
+def reshape_to_array(diagrams):
+    ndgms = copy.deepcopy(diagrams)
+    d0 = len(ndgms)
+    d1 = 0
+    d2 = 2
+    for i in range(0, d0):
+        d1 = max(d1, len(ndgms[i]))
+    for i in range(0,d0):
+        d = len(ndgms[i])
+        if d==d1:
+            continue
+        ndgms[i] = list(ndgms[i])
+        for k in range(0, d1-d):
+            ndgms[i].append([-1,-1])
+    dgms_array = []
+    for i in range(0, d0):
+        dgms_array.append(np.array(ndgms[i]))
+    return np.reshape(dgms_array, (d0, d1, d2))
+
```

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/DynSysLib.py` & `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/DynSysLib.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/UserGuide.py` & `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/UserGuide.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/autonomous_dissipative_flows.py` & `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/autonomous_dissipative_flows.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/conservative_flows.py` & `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/conservative_flows.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/delayed_flows.py` & `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/delayed_flows.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/driven_dissipative_flows.py` & `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/driven_dissipative_flows.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/maps.py` & `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/maps.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/medical_data.py` & `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/medical_data.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/noise_models.py` & `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/noise_models.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/MakeData/DynSysLib/periodic_functions.py` & `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/periodic_functions.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/MakeData/PointCloud.py` & `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/PointCloud.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/SP/adaptivePart.py` & `teaspoon-1.5.2/teaspoon/teaspoon/SP/adaptivePart.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/SP/information/entropy.py` & `teaspoon-1.5.2/teaspoon/teaspoon/SP/information/entropy.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/SP/network.py` & `teaspoon-1.5.2/teaspoon/teaspoon/SP/network.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/SP/network_tools.py` & `teaspoon-1.5.2/teaspoon/teaspoon/SP/network_tools.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/SP/texture_analysis.py` & `teaspoon-1.5.2/teaspoon/teaspoon/SP/texture_analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib import rc
 from ripser import ripser
 import matplotlib.gridspec as gridspec
-from gtda.homology import CubicalPersistence
+from gudhi.sklearn.cubical_persistence import CubicalPersistence
+from gudhi.representations import DiagramSelector
+from sklearn.pipeline import Pipeline
 from scipy import stats
 from scipy import ndimage as sp
 from scipy import integrate
 
 # Set Font
 rc('font', **{'family': 'sans-serif', 'sans-serif': ['Helvetica']})
 rc('text', usetex=True)
@@ -396,19 +398,18 @@
         dim: int
         Desired dimension of persistence.
     Returns
     -------
     Persistence pairs of desired dimension on the input image.
 
     """
-    cubical_persistence = CubicalPersistence(n_jobs=-1, reduced_homology=True)
-    pdgm = cubical_persistence.fit_transform(np.array([img]))
-    pdgm = pdgm[0].astype(np.float64)
-    dgms = []
 
-    # Filter persistence diagram to return desired dimension
-    for n, item in enumerate(pdgm):
-        if item[2] == dim:
-            dgms.append(np.array(pdgm[n, :]))
+    pipe = Pipeline(
+    [
+        ("cub_pers", CubicalPersistence(homology_dimensions=dim, n_jobs=-2)),
+        ("finite_diags", DiagramSelector(use=True, point_type="finite")),
+    ]
+)
+    pdgm = pipe.fit_transform(np.array([img]))
+    pdgm = pdgm[0].astype(np.float64)
 
-    dgms = np.array(dgms)
-    return dgms
+    return pdgm
```

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/SP/tsa_tools.py` & `teaspoon-1.5.2/teaspoon/teaspoon/SP/tsa_tools.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/TDA/Distance.py` & `teaspoon-1.5.2/teaspoon/teaspoon/TDA/Distance.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/TDA/Draw.py` & `teaspoon-1.5.2/teaspoon/teaspoon/TDA/Draw.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/TDA/PHN.py` & `teaspoon-1.5.2/teaspoon/teaspoon/TDA/PHN.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/TDA/Persistence.py` & `teaspoon-1.5.2/teaspoon/teaspoon/TDA/Persistence.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/TDA/SLSP.py` & `teaspoon-1.5.2/teaspoon/teaspoon/TDA/SLSP.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/TDA/SLSP_tools.py` & `teaspoon-1.5.2/teaspoon/teaspoon/TDA/SLSP_tools.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/parameter_selection/FNN_n.py` & `teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/FNN_n.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/parameter_selection/MI_delay.py` & `teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/MI_delay.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/parameter_selection/MsPE.py` & `teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/MsPE.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/parameter_selection/PAMI_delay.py` & `teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/PAMI_delay.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/parameter_selection/autocorrelation.py` & `teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/autocorrelation.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon/parameter_selection/delay_LMS.py` & `teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/delay_LMS.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon.egg-info/PKG-INFO` & `teaspoon-1.5.2/teaspoon/teaspoon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teaspoon
-Version: 1.4.8
+Version: 1.5.2
 Summary: A Topological Signal Processing Package
 Author-email: Elizabeth Munch <muncheli@msu.edu>
 Project-URL: repository, https://github.com/TeaspoonTDA/teaspoon
 Project-URL: homepage, https://github.com/TeaspoonTDA/teaspoon
 Project-URL: documentation, https://teaspoontda.github.io/teaspoon/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -27,18 +27,19 @@
 Requires-Dist: scikit-learn>=1.1.1
 Requires-Dist: scipy>=1.8.1
 Requires-Dist: six>=1.16.0
 Requires-Dist: threadpoolctl>=3.1.0
 Requires-Dist: ripser>=0.6.4
 Requires-Dist: sympy>=1.11.1
 Requires-Dist: sortedcontainers>=2.4.0
-Requires-Dist: giotto-tda>=0.5.0
 Requires-Dist: persim
-Requires-Dist: pandas
+Requires-Dist: pandas>=1.4.1
 Requires-Dist: gudhi
+Requires-Dist: numba
+Requires-Dist: importlib_resources
 
 Description
 ==============
 
 The emerging field of topological signal processing brings methods from Topological Data Analysis (TDA) to create new tools for signal processing by incorporating aspects of shape.
 This python package, teaspoon for tsp or topological signal processing, brings together available software for computing persistent homology, the main workhorse of TDA, with modules that expand the functionality of teaspoon as a state-of-the-art topological signal processing tool.
 These modules include methods for incorporating tools from machine learning, complex networks, information, and parameter selection along with a dynamical systems library to streamline the creation and benchmarking of new methods.
```

### Comparing `teaspoon-1.4.8/teaspoon/teaspoon.egg-info/SOURCES.txt` & `teaspoon-1.5.2/teaspoon/teaspoon.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 teaspoon/teaspoon.egg-info/requires.txt
 teaspoon/teaspoon.egg-info/top_level.txt
 teaspoon/teaspoon/ML/Base.py
 teaspoon/teaspoon/ML/PD_Classification.py
 teaspoon/teaspoon/ML/__init__.py
 teaspoon/teaspoon/ML/feature_functions.py
 teaspoon/teaspoon/ML/load_datasets.py
+teaspoon/teaspoon/ML/datasets/__init__.py
 teaspoon/teaspoon/ML/datasets/mnist.pickle
 teaspoon/teaspoon/ML/datasets/mpeg7.pickle
 teaspoon/teaspoon/ML/datasets/shrec14.pickle
 teaspoon/teaspoon/MakeData/PointCloud.py
 teaspoon/teaspoon/MakeData/__init__.py
 teaspoon/teaspoon/MakeData/DynSysLib/DynSysLib.py
 teaspoon/teaspoon/MakeData/DynSysLib/UserGuide.py
@@ -36,14 +37,15 @@
 teaspoon/teaspoon/SP/network_tools.py
 teaspoon/teaspoon/SP/texture_analysis.py
 teaspoon/teaspoon/SP/tsa_tools.py
 teaspoon/teaspoon/SP/information/__init__.py
 teaspoon/teaspoon/SP/information/entropy.py
 teaspoon/teaspoon/TDA/Distance.py
 teaspoon/teaspoon/TDA/Draw.py
+teaspoon/teaspoon/TDA/Magnitude.py
 teaspoon/teaspoon/TDA/PHN.py
 teaspoon/teaspoon/TDA/Persistence.py
 teaspoon/teaspoon/TDA/SLSP.py
 teaspoon/teaspoon/TDA/SLSP_tools.py
 teaspoon/teaspoon/TDA/__init__.py
 teaspoon/teaspoon/TDA/c_profile_test.py
 teaspoon/teaspoon/parameter_selection/FNN_n.py
@@ -56,10 +58,11 @@
 tests/test_MakeData.py
 tests/test_OrdinalPartition.py
 tests/test_PointSummariesPHN.py
 tests/test_SLSP.py
 tests/test_basics.py
 tests/test_classification.py
 tests/test_featureFunctions.py
+tests/test_magnitude.py
 tests/test_parameterSelection.py
 tests/test_signalProcessing.py
 tests/test_texture_analysis.py
```

### Comparing `teaspoon-1.4.8/tests/test_MakeData.py` & `teaspoon-1.5.2/tests/test_MakeData.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/tests/test_OrdinalPartition.py` & `teaspoon-1.5.2/tests/test_OrdinalPartition.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/tests/test_PointSummariesPHN.py` & `teaspoon-1.5.2/tests/test_PointSummariesPHN.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/tests/test_SLSP.py` & `teaspoon-1.5.2/tests/test_SLSP.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/tests/test_basics.py` & `teaspoon-1.5.2/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/tests/test_classification.py` & `teaspoon-1.5.2/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/tests/test_parameterSelection.py` & `teaspoon-1.5.2/tests/test_parameterSelection.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/tests/test_signalProcessing.py` & `teaspoon-1.5.2/tests/test_signalProcessing.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.4.8/tests/test_texture_analysis.py` & `teaspoon-1.5.2/tests/test_texture_analysis.py`

 * *Files identical despite different names*


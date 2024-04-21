# Comparing `tmp/ploteries-0.1.0.tar.gz` & `tmp/ploteries-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploteries-0.1.0.tar", last modified: Sat Apr 20 23:36:52 2024, max compression
+gzip compressed data, was "ploteries-0.1.1.tar", last modified: Sun Apr 21 05:16:30 2024, max compression
```

## Comparing `ploteries-0.1.0.tar` & `ploteries-0.1.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 23:36:52.336274 ploteries-0.1.0/
--rw-r--r--   0 jazs       (501) staff       (20)     1087 2024-04-20 23:24:11.000000 ploteries-0.1.0/LICENSE
--rw-r--r--   0 jazs       (501) staff       (20)      385 2024-04-20 23:36:52.336089 ploteries-0.1.0/PKG-INFO
--rw-r--r--   0 jazs       (501) staff       (20)      803 2024-04-20 23:24:11.000000 ploteries-0.1.0/README.md
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 23:36:52.327558 ploteries-0.1.0/ploteries/
--rw-r--r--   0 jazs       (501) staff       (20)      132 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/__init__.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 23:36:52.329331 ploteries-0.1.0/ploteries/_bin_helpers/
--rw-r--r--   0 jazs       (501) staff       (20)      142 2024-04-19 21:27:07.000000 ploteries-0.1.0/ploteries/_bin_helpers/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)    13698 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/_bin_helpers/launch.py
--rw-r--r--   0 jazs       (501) staff       (20)      160 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/_bin_helpers/main.py
--rw-r--r--   0 jazs       (501) staff       (20)     5917 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/_bin_helpers/mock_generator.py
--rw-r--r--   0 jazs       (501) staff       (20)      851 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/_bin_helpers/utils.py
--rw-r--r--   0 jazs       (501) staff       (20)       52 2024-04-19 21:27:07.000000 ploteries-0.1.0/ploteries/_table_handler_cli_interface.py
--rw-r--r--   0 jazs       (501) staff       (20)     8462 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/base_handlers.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 23:36:52.329465 ploteries-0.1.0/ploteries/bin/
--rwxr-xr-x   0 jazs       (501) staff       (20)      125 2024-04-19 21:27:07.000000 ploteries-0.1.0/ploteries/bin/ploteries
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 23:36:52.330755 ploteries-0.1.0/ploteries/cli_interface/
--rw-r--r--   0 jazs       (501) staff       (20)      210 2024-04-19 21:27:07.000000 ploteries-0.1.0/ploteries/cli_interface/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     1574 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/cli_interface/abstract_hook.py
--rw-r--r--   0 jazs       (501) staff       (20)     4750 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/cli_interface/cli_interface.py
--rw-r--r--   0 jazs       (501) staff       (20)    11125 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/cli_interface/figure_handler_hook.py
--rw-r--r--   0 jazs       (501) staff       (20)     4530 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/cli_interface/table_handler_hook.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 23:36:52.331209 ploteries-0.1.0/ploteries/data_store/
--rw-r--r--   0 jazs       (501) staff       (20)      167 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/data_store/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     2321 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/data_store/_legacy_type_deserializers.py
--rw-r--r--   0 jazs       (501) staff       (20)    16493 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/data_store/data_store.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 23:36:52.332184 ploteries-0.1.0/ploteries/figure_handler/
--rw-r--r--   0 jazs       (501) staff       (20)      127 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/figure_handler/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     4643 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/figure_handler/figure_handler.py
--rw-r--r--   0 jazs       (501) staff       (20)     1494 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/figure_handler/helpers.py
--rw-r--r--   0 jazs       (501) staff       (20)     3570 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/figure_handler/scalars_figure_handler.py
--rw-r--r--   0 jazs       (501) staff       (20)     8885 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/figure_handler/table_handler.py
--rw-r--r--   0 jazs       (501) staff       (20)    11226 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/ndarray_data_handlers.py
--rw-r--r--   0 jazs       (501) staff       (20)      532 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/serializable_data_handler.py
--rw-r--r--   0 jazs       (501) staff       (20)     5287 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/train_manager_visualizations.py
--rw-r--r--   0 jazs       (501) staff       (20)    17375 2024-04-20 23:24:11.000000 ploteries-0.1.0/ploteries/writer.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 23:36:52.334563 ploteries-0.1.0/ploteries.egg-info/
--rw-r--r--   0 jazs       (501) staff       (20)      385 2024-04-20 23:36:52.000000 ploteries-0.1.0/ploteries.egg-info/PKG-INFO
--rw-r--r--   0 jazs       (501) staff       (20)     1744 2024-04-20 23:36:52.000000 ploteries-0.1.0/ploteries.egg-info/SOURCES.txt
--rw-r--r--   0 jazs       (501) staff       (20)        1 2024-04-20 23:36:52.000000 ploteries-0.1.0/ploteries.egg-info/dependency_links.txt
--rw-r--r--   0 jazs       (501) staff       (20)      107 2024-04-20 23:36:52.000000 ploteries-0.1.0/ploteries.egg-info/requires.txt
--rw-r--r--   0 jazs       (501) staff       (20)       16 2024-04-20 23:36:52.000000 ploteries-0.1.0/ploteries.egg-info/top_level.txt
--rw-r--r--   0 jazs       (501) staff       (20)       38 2024-04-20 23:36:52.336309 ploteries-0.1.0/setup.cfg
--rw-r--r--   0 jazs       (501) staff       (20)      532 2024-04-20 23:24:43.000000 ploteries-0.1.0/setup.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 23:36:52.325041 ploteries-0.1.0/tests/
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 23:36:52.332917 ploteries-0.1.0/tests/ploteries/
--rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-19 21:27:07.000000 ploteries-0.1.0/tests/ploteries/__init__.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 23:36:52.333119 ploteries-0.1.0/tests/ploteries/_bin_helpers/
--rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-19 21:27:07.000000 ploteries-0.1.0/tests/ploteries/_bin_helpers/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)      610 2024-04-20 23:24:11.000000 ploteries-0.1.0/tests/ploteries/_bin_helpers/launch.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 23:36:52.333358 ploteries-0.1.0/tests/ploteries/cli_interface/
--rw-r--r--   0 jazs       (501) staff       (20)        1 2024-04-19 21:27:07.000000 ploteries-0.1.0/tests/ploteries/cli_interface/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     3471 2024-04-20 23:24:11.000000 ploteries-0.1.0/tests/ploteries/cli_interface/figure_handler_hook.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 23:36:52.333611 ploteries-0.1.0/tests/ploteries/data_store/
--rw-r--r--   0 jazs       (501) staff       (20)       99 2024-04-19 21:27:07.000000 ploteries-0.1.0/tests/ploteries/data_store/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     8772 2024-04-20 23:24:11.000000 ploteries-0.1.0/tests/ploteries/data_store/data_store.py
-drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-20 23:36:52.334392 ploteries-0.1.0/tests/ploteries/figure_handler/
--rw-r--r--   0 jazs       (501) staff       (20)       80 2024-04-20 23:24:11.000000 ploteries-0.1.0/tests/ploteries/figure_handler/__init__.py
--rw-r--r--   0 jazs       (501) staff       (20)     5487 2024-04-20 23:24:11.000000 ploteries-0.1.0/tests/ploteries/figure_handler/figure_handler.py
--rw-r--r--   0 jazs       (501) staff       (20)     1158 2024-04-20 23:24:11.000000 ploteries-0.1.0/tests/ploteries/figure_handler/scalars_figure_handler.py
--rw-r--r--   0 jazs       (501) staff       (20)     3664 2024-04-20 23:24:11.000000 ploteries-0.1.0/tests/ploteries/figure_handler/table_handler.py
--rw-r--r--   0 jazs       (501) staff       (20)     4330 2024-04-20 23:24:11.000000 ploteries-0.1.0/tests/ploteries/ndarray_data_handlers.py
--rw-r--r--   0 jazs       (501) staff       (20)     1952 2024-04-20 23:24:11.000000 ploteries-0.1.0/tests/ploteries/serializable_data_handler.py
--rw-r--r--   0 jazs       (501) staff       (20)     3473 2024-04-20 23:24:11.000000 ploteries-0.1.0/tests/ploteries/writer.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-21 05:16:30.579477 ploteries-0.1.1/
+-rw-r--r--   0 jazs       (501) staff       (20)     1087 2024-04-20 23:24:11.000000 ploteries-0.1.1/LICENSE
+-rw-r--r--   0 jazs       (501) staff       (20)     1362 2024-04-21 05:16:30.579297 ploteries-0.1.1/PKG-INFO
+-rw-r--r--   0 jazs       (501) staff       (20)      803 2024-04-20 23:24:11.000000 ploteries-0.1.1/README.md
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-21 05:16:30.571275 ploteries-0.1.1/ploteries/
+-rw-r--r--   0 jazs       (501) staff       (20)      132 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/__init__.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-21 05:16:30.573218 ploteries-0.1.1/ploteries/_bin_helpers/
+-rw-r--r--   0 jazs       (501) staff       (20)      142 2024-04-19 21:27:07.000000 ploteries-0.1.1/ploteries/_bin_helpers/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)    13698 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/_bin_helpers/launch.py
+-rw-r--r--   0 jazs       (501) staff       (20)      160 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/_bin_helpers/main.py
+-rw-r--r--   0 jazs       (501) staff       (20)     5917 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/_bin_helpers/mock_generator.py
+-rw-r--r--   0 jazs       (501) staff       (20)      851 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/_bin_helpers/utils.py
+-rw-r--r--   0 jazs       (501) staff       (20)       52 2024-04-19 21:27:07.000000 ploteries-0.1.1/ploteries/_table_handler_cli_interface.py
+-rw-r--r--   0 jazs       (501) staff       (20)     8462 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/base_handlers.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-21 05:16:30.573505 ploteries-0.1.1/ploteries/bin/
+-rwxr-xr-x   0 jazs       (501) staff       (20)      125 2024-04-19 21:27:07.000000 ploteries-0.1.1/ploteries/bin/ploteries
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-21 05:16:30.574940 ploteries-0.1.1/ploteries/cli_interface/
+-rw-r--r--   0 jazs       (501) staff       (20)      210 2024-04-19 21:27:07.000000 ploteries-0.1.1/ploteries/cli_interface/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1574 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/cli_interface/abstract_hook.py
+-rw-r--r--   0 jazs       (501) staff       (20)     4750 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/cli_interface/cli_interface.py
+-rw-r--r--   0 jazs       (501) staff       (20)    11125 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/cli_interface/figure_handler_hook.py
+-rw-r--r--   0 jazs       (501) staff       (20)     4530 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/cli_interface/table_handler_hook.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-21 05:16:30.575700 ploteries-0.1.1/ploteries/data_store/
+-rw-r--r--   0 jazs       (501) staff       (20)      167 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/data_store/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     2321 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/data_store/_legacy_type_deserializers.py
+-rw-r--r--   0 jazs       (501) staff       (20)    16493 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/data_store/data_store.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-21 05:16:30.576679 ploteries-0.1.1/ploteries/figure_handler/
+-rw-r--r--   0 jazs       (501) staff       (20)      127 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/figure_handler/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     4643 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/figure_handler/figure_handler.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1494 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/figure_handler/helpers.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3570 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/figure_handler/scalars_figure_handler.py
+-rw-r--r--   0 jazs       (501) staff       (20)     8885 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/figure_handler/table_handler.py
+-rw-r--r--   0 jazs       (501) staff       (20)    11226 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/ndarray_data_handlers.py
+-rw-r--r--   0 jazs       (501) staff       (20)      532 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/serializable_data_handler.py
+-rw-r--r--   0 jazs       (501) staff       (20)     5287 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/train_manager_visualizations.py
+-rw-r--r--   0 jazs       (501) staff       (20)    17375 2024-04-20 23:24:11.000000 ploteries-0.1.1/ploteries/writer.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-21 05:16:30.579089 ploteries-0.1.1/ploteries.egg-info/
+-rw-r--r--   0 jazs       (501) staff       (20)     1362 2024-04-21 05:16:30.000000 ploteries-0.1.1/ploteries.egg-info/PKG-INFO
+-rw-r--r--   0 jazs       (501) staff       (20)     1744 2024-04-21 05:16:30.000000 ploteries-0.1.1/ploteries.egg-info/SOURCES.txt
+-rw-r--r--   0 jazs       (501) staff       (20)        1 2024-04-21 05:16:30.000000 ploteries-0.1.1/ploteries.egg-info/dependency_links.txt
+-rw-r--r--   0 jazs       (501) staff       (20)      107 2024-04-21 05:16:30.000000 ploteries-0.1.1/ploteries.egg-info/requires.txt
+-rw-r--r--   0 jazs       (501) staff       (20)       16 2024-04-21 05:16:30.000000 ploteries-0.1.1/ploteries.egg-info/top_level.txt
+-rw-r--r--   0 jazs       (501) staff       (20)       38 2024-04-21 05:16:30.579514 ploteries-0.1.1/setup.cfg
+-rw-r--r--   0 jazs       (501) staff       (20)      825 2024-04-20 23:50:41.000000 ploteries-0.1.1/setup.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-21 05:16:30.568740 ploteries-0.1.1/tests/
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-21 05:16:30.577361 ploteries-0.1.1/tests/ploteries/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-19 21:27:07.000000 ploteries-0.1.1/tests/ploteries/__init__.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-21 05:16:30.577593 ploteries-0.1.1/tests/ploteries/_bin_helpers/
+-rw-r--r--   0 jazs       (501) staff       (20)        0 2024-04-19 21:27:07.000000 ploteries-0.1.1/tests/ploteries/_bin_helpers/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)      610 2024-04-20 23:24:11.000000 ploteries-0.1.1/tests/ploteries/_bin_helpers/launch.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-21 05:16:30.577853 ploteries-0.1.1/tests/ploteries/cli_interface/
+-rw-r--r--   0 jazs       (501) staff       (20)        1 2024-04-19 21:27:07.000000 ploteries-0.1.1/tests/ploteries/cli_interface/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3471 2024-04-20 23:24:11.000000 ploteries-0.1.1/tests/ploteries/cli_interface/figure_handler_hook.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-21 05:16:30.578080 ploteries-0.1.1/tests/ploteries/data_store/
+-rw-r--r--   0 jazs       (501) staff       (20)       99 2024-04-19 21:27:07.000000 ploteries-0.1.1/tests/ploteries/data_store/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     8772 2024-04-20 23:24:11.000000 ploteries-0.1.1/tests/ploteries/data_store/data_store.py
+drwxr-xr-x   0 jazs       (501) staff       (20)        0 2024-04-21 05:16:30.578921 ploteries-0.1.1/tests/ploteries/figure_handler/
+-rw-r--r--   0 jazs       (501) staff       (20)       80 2024-04-20 23:24:11.000000 ploteries-0.1.1/tests/ploteries/figure_handler/__init__.py
+-rw-r--r--   0 jazs       (501) staff       (20)     5487 2024-04-20 23:24:11.000000 ploteries-0.1.1/tests/ploteries/figure_handler/figure_handler.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1158 2024-04-20 23:24:11.000000 ploteries-0.1.1/tests/ploteries/figure_handler/scalars_figure_handler.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3664 2024-04-20 23:24:11.000000 ploteries-0.1.1/tests/ploteries/figure_handler/table_handler.py
+-rw-r--r--   0 jazs       (501) staff       (20)     4330 2024-04-20 23:24:11.000000 ploteries-0.1.1/tests/ploteries/ndarray_data_handlers.py
+-rw-r--r--   0 jazs       (501) staff       (20)     1952 2024-04-20 23:24:11.000000 ploteries-0.1.1/tests/ploteries/serializable_data_handler.py
+-rw-r--r--   0 jazs       (501) staff       (20)     3473 2024-04-20 23:24:11.000000 ploteries-0.1.1/tests/ploteries/writer.py
```

### Comparing `ploteries-0.1.0/LICENSE` & `ploteries-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/README.md` & `ploteries-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/_bin_helpers/launch.py` & `ploteries-0.1.1/ploteries/_bin_helpers/launch.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/_bin_helpers/mock_generator.py` & `ploteries-0.1.1/ploteries/_bin_helpers/mock_generator.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/_bin_helpers/utils.py` & `ploteries-0.1.1/ploteries/_bin_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/base_handlers.py` & `ploteries-0.1.1/ploteries/base_handlers.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/cli_interface/abstract_hook.py` & `ploteries-0.1.1/ploteries/cli_interface/abstract_hook.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/cli_interface/cli_interface.py` & `ploteries-0.1.1/ploteries/cli_interface/cli_interface.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/cli_interface/figure_handler_hook.py` & `ploteries-0.1.1/ploteries/cli_interface/figure_handler_hook.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/cli_interface/table_handler_hook.py` & `ploteries-0.1.1/ploteries/cli_interface/table_handler_hook.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/data_store/_legacy_type_deserializers.py` & `ploteries-0.1.1/ploteries/data_store/_legacy_type_deserializers.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/data_store/data_store.py` & `ploteries-0.1.1/ploteries/data_store/data_store.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/figure_handler/figure_handler.py` & `ploteries-0.1.1/ploteries/figure_handler/figure_handler.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/figure_handler/helpers.py` & `ploteries-0.1.1/ploteries/figure_handler/helpers.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/figure_handler/scalars_figure_handler.py` & `ploteries-0.1.1/ploteries/figure_handler/scalars_figure_handler.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/figure_handler/table_handler.py` & `ploteries-0.1.1/ploteries/figure_handler/table_handler.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/ndarray_data_handlers.py` & `ploteries-0.1.1/ploteries/ndarray_data_handlers.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/serializable_data_handler.py` & `ploteries-0.1.1/ploteries/serializable_data_handler.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/train_manager_visualizations.py` & `ploteries-0.1.1/ploteries/train_manager_visualizations.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries/writer.py` & `ploteries-0.1.1/ploteries/writer.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/ploteries.egg-info/SOURCES.txt` & `ploteries-0.1.1/ploteries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/tests/ploteries/_bin_helpers/launch.py` & `ploteries-0.1.1/tests/ploteries/_bin_helpers/launch.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/tests/ploteries/cli_interface/figure_handler_hook.py` & `ploteries-0.1.1/tests/ploteries/cli_interface/figure_handler_hook.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/tests/ploteries/data_store/data_store.py` & `ploteries-0.1.1/tests/ploteries/data_store/data_store.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/tests/ploteries/figure_handler/figure_handler.py` & `ploteries-0.1.1/tests/ploteries/figure_handler/figure_handler.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/tests/ploteries/figure_handler/scalars_figure_handler.py` & `ploteries-0.1.1/tests/ploteries/figure_handler/scalars_figure_handler.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/tests/ploteries/figure_handler/table_handler.py` & `ploteries-0.1.1/tests/ploteries/figure_handler/table_handler.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/tests/ploteries/ndarray_data_handlers.py` & `ploteries-0.1.1/tests/ploteries/ndarray_data_handlers.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/tests/ploteries/serializable_data_handler.py` & `ploteries-0.1.1/tests/ploteries/serializable_data_handler.py`

 * *Files identical despite different names*

### Comparing `ploteries-0.1.0/tests/ploteries/writer.py` & `ploteries-0.1.1/tests/ploteries/writer.py`

 * *Files identical despite different names*


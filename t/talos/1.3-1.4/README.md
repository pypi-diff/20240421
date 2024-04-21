# Comparing `tmp/talos-1.3.tar.gz` & `tmp/talos-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talos-1.3.tar", last modified: Sat May 28 10:07:33 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `talos-1.3.tar` & `talos-1.4.tar`

### file list

```diff
@@ -1,93 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:33.794333 talos-1.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-05-28 10:07:24.000000 talos-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-05-28 10:07:33.794333 talos-1.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     6429 2022-05-28 10:07:24.000000 talos-1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-05-28 10:07:33.794333 talos-1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2772 2022-05-28 10:07:24.000000 talos-1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:33.786333 talos-1.3/talos/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1103 2022-05-28 10:07:24.000000 talos-1.3/talos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:33.786333 talos-1.3/talos/autom8/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-05-28 10:07:24.000000 talos-1.3/talos/autom8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4610 2022-05-28 10:07:24.000000 talos-1.3/talos/autom8/automodel.py
--rw-r--r--   0 runner    (1001) docker     (121)     8781 2022-05-28 10:07:24.000000 talos-1.3/talos/autom8/autoparams.py
--rw-r--r--   0 runner    (1001) docker     (121)     4425 2022-05-28 10:07:24.000000 talos-1.3/talos/autom8/autopredict.py
--rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-05-28 10:07:24.000000 talos-1.3/talos/autom8/autoscan.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:33.786333 talos-1.3/talos/callbacks/
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-05-28 10:07:24.000000 talos-1.3/talos/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-05-28 10:07:24.000000 talos-1.3/talos/callbacks/experiment_log.py
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-05-28 10:07:24.000000 talos-1.3/talos/callbacks/power_draw.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:33.790333 talos-1.3/talos/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:24.000000 talos-1.3/talos/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7000 2022-05-28 10:07:24.000000 talos-1.3/talos/commands/analyze.py
--rw-r--r--   0 runner    (1001) docker     (121)     3937 2022-05-28 10:07:24.000000 talos-1.3/talos/commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3674 2022-05-28 10:07:24.000000 talos-1.3/talos/commands/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3154 2022-05-28 10:07:24.000000 talos-1.3/talos/commands/predict.py
--rw-r--r--   0 runner    (1001) docker     (121)     1728 2022-05-28 10:07:24.000000 talos-1.3/talos/commands/restore.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:33.790333 talos-1.3/talos/logging/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:24.000000 talos-1.3/talos/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-05-28 10:07:24.000000 talos-1.3/talos/logging/logging_finish.py
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-05-28 10:07:24.000000 talos-1.3/talos/logging/logging_run.py
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-05-28 10:07:24.000000 talos-1.3/talos/logging/results.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:33.790333 talos-1.3/talos/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:24.000000 talos-1.3/talos/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1436 2022-05-28 10:07:24.000000 talos-1.3/talos/metrics/entropy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3014 2022-05-28 10:07:24.000000 talos-1.3/talos/metrics/keras_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:33.790333 talos-1.3/talos/model/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-05-28 10:07:24.000000 talos-1.3/talos/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1730 2022-05-28 10:07:24.000000 talos-1.3/talos/model/early_stopper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1728 2022-05-28 10:07:24.000000 talos-1.3/talos/model/hidden_layers.py
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-05-28 10:07:24.000000 talos-1.3/talos/model/ingest_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1824 2022-05-28 10:07:24.000000 talos-1.3/talos/model/network_shape.py
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-05-28 10:07:24.000000 talos-1.3/talos/model/normalizers.py
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-05-28 10:07:24.000000 talos-1.3/talos/model/output_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:33.790333 talos-1.3/talos/parameters/
--rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-05-28 10:07:24.000000 talos-1.3/talos/parameters/DistributeParamSpace.py
--rw-r--r--   0 runner    (1001) docker     (121)     7521 2022-05-28 10:07:24.000000 talos-1.3/talos/parameters/ParamSpace.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:24.000000 talos-1.3/talos/parameters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:33.790333 talos-1.3/talos/reducers/
--rw-r--r--   0 runner    (1001) docker     (121)     2761 2022-05-28 10:07:24.000000 talos-1.3/talos/reducers/GamifyMap.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:24.000000 talos-1.3/talos/reducers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1587 2022-05-28 10:07:24.000000 talos-1.3/talos/reducers/correlation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-05-28 10:07:24.000000 talos-1.3/talos/reducers/forrest.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-05-28 10:07:24.000000 talos-1.3/talos/reducers/gamify.py
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-05-28 10:07:24.000000 talos-1.3/talos/reducers/limit_by_metric.py
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-05-28 10:07:24.000000 talos-1.3/talos/reducers/local_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2887 2022-05-28 10:07:24.000000 talos-1.3/talos/reducers/reduce_run.py
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-05-28 10:07:24.000000 talos-1.3/talos/reducers/reduce_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2022-05-28 10:07:24.000000 talos-1.3/talos/reducers/sample_reducer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1742 2022-05-28 10:07:24.000000 talos-1.3/talos/reducers/trees.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:33.790333 talos-1.3/talos/scan/
--rwxr-xr-x   0 runner    (1001) docker     (121)     7448 2022-05-28 10:07:24.000000 talos-1.3/talos/scan/Scan.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:24.000000 talos-1.3/talos/scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4722 2022-05-28 10:07:24.000000 talos-1.3/talos/scan/scan_addon.py
--rw-r--r--   0 runner    (1001) docker     (121)     2316 2022-05-28 10:07:24.000000 talos-1.3/talos/scan/scan_finish.py
--rw-r--r--   0 runner    (1001) docker     (121)     2228 2022-05-28 10:07:24.000000 talos-1.3/talos/scan/scan_prepare.py
--rw-r--r--   0 runner    (1001) docker     (121)     2050 2022-05-28 10:07:24.000000 talos-1.3/talos/scan/scan_round.py
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-05-28 10:07:24.000000 talos-1.3/talos/scan/scan_run.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-05-28 10:07:24.000000 talos-1.3/talos/scan/scan_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:33.794333 talos-1.3/talos/templates/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-28 10:07:24.000000 talos-1.3/talos/templates/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5094 2022-05-28 10:07:24.000000 talos-1.3/talos/templates/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     5584 2022-05-28 10:07:24.000000 talos-1.3/talos/templates/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2674 2022-05-28 10:07:24.000000 talos-1.3/talos/templates/params.py
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-05-28 10:07:24.000000 talos-1.3/talos/templates/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:33.794333 talos-1.3/talos/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-05-28 10:07:24.000000 talos-1.3/talos/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-05-28 10:07:24.000000 talos-1.3/talos/utils/best_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-05-28 10:07:24.000000 talos-1.3/talos/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-05-28 10:07:24.000000 talos-1.3/talos/utils/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-05-28 10:07:24.000000 talos-1.3/talos/utils/gpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-05-28 10:07:24.000000 talos-1.3/talos/utils/load_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-05-28 10:07:24.000000 talos-1.3/talos/utils/power_draw_append.py
--rw-r--r--   0 runner    (1001) docker     (121)     3198 2022-05-28 10:07:24.000000 talos-1.3/talos/utils/recover_best_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-05-28 10:07:24.000000 talos-1.3/talos/utils/rescale_meanzero.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-05-28 10:07:24.000000 talos-1.3/talos/utils/sequence_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-05-28 10:07:24.000000 talos-1.3/talos/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-05-28 10:07:24.000000 talos-1.3/talos/utils/torch_history.py
--rw-r--r--   0 runner    (1001) docker     (121)     2448 2022-05-28 10:07:24.000000 talos-1.3/talos/utils/validation_split.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 10:07:33.786333 talos-1.3/talos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-05-28 10:07:33.000000 talos-1.3/talos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-05-28 10:07:33.000000 talos-1.3/talos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-28 10:07:33.000000 talos-1.3/talos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-05-28 10:07:33.000000 talos-1.3/talos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-05-28 10:07:33.000000 talos-1.3/talos.egg-info/top_level.txt
+-rwxr-xr-x   0        0        0     1103 2020-02-02 00:00:00.000000 talos-1.4/talos/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 talos-1.4/talos/autom8/__init__.py
+-rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 talos-1.4/talos/autom8/automodel.py
+-rw-r--r--   0        0        0     8778 2020-02-02 00:00:00.000000 talos-1.4/talos/autom8/autoparams.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 talos-1.4/talos/autom8/autopredict.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 talos-1.4/talos/autom8/autoscan.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 talos-1.4/talos/callbacks/__init__.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 talos-1.4/talos/callbacks/experiment_log.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 talos-1.4/talos/callbacks/power_draw.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 talos-1.4/talos/commands/__init__.py
+-rw-r--r--   0        0        0     7000 2020-02-02 00:00:00.000000 talos-1.4/talos/commands/analyze.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 talos-1.4/talos/commands/deploy.py
+-rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 talos-1.4/talos/commands/evaluate.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 talos-1.4/talos/commands/predict.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 talos-1.4/talos/commands/restore.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 talos-1.4/talos/logging/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 talos-1.4/talos/logging/logging_finish.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 talos-1.4/talos/logging/logging_run.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 talos-1.4/talos/logging/results.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 talos-1.4/talos/metrics/__init__.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 talos-1.4/talos/metrics/entropy.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 talos-1.4/talos/metrics/keras_metrics.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 talos-1.4/talos/model/__init__.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 talos-1.4/talos/model/early_stopper.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 talos-1.4/talos/model/hidden_layers.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 talos-1.4/talos/model/ingest_model.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 talos-1.4/talos/model/network_shape.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 talos-1.4/talos/model/normalizers.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 talos-1.4/talos/model/output_layer.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 talos-1.4/talos/parameters/DistributeParamSpace.py
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 talos-1.4/talos/parameters/ParamSpace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 talos-1.4/talos/parameters/__init__.py
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 talos-1.4/talos/reducers/GamifyMap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 talos-1.4/talos/reducers/__init__.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 talos-1.4/talos/reducers/correlation.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 talos-1.4/talos/reducers/forrest.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 talos-1.4/talos/reducers/gamify.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 talos-1.4/talos/reducers/limit_by_metric.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 talos-1.4/talos/reducers/local_strategy.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 talos-1.4/talos/reducers/reduce_run.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 talos-1.4/talos/reducers/reduce_utils.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 talos-1.4/talos/reducers/sample_reducer.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 talos-1.4/talos/reducers/trees.py
+-rwxr-xr-x   0        0        0     7448 2020-02-02 00:00:00.000000 talos-1.4/talos/scan/Scan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 talos-1.4/talos/scan/__init__.py
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 talos-1.4/talos/scan/scan_addon.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 talos-1.4/talos/scan/scan_finish.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 talos-1.4/talos/scan/scan_prepare.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 talos-1.4/talos/scan/scan_round.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 talos-1.4/talos/scan/scan_run.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 talos-1.4/talos/scan/scan_utils.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 talos-1.4/talos/templates/__init__.py
+-rwxr-xr-x   0        0        0     5299 2020-02-02 00:00:00.000000 talos-1.4/talos/templates/datasets.py
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 talos-1.4/talos/templates/models.py
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 talos-1.4/talos/templates/params.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 talos-1.4/talos/templates/pipelines.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 talos-1.4/talos/utils/__init__.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 talos-1.4/talos/utils/best_model.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 talos-1.4/talos/utils/exceptions.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 talos-1.4/talos/utils/generator.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 talos-1.4/talos/utils/gpu_utils.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 talos-1.4/talos/utils/load_model.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 talos-1.4/talos/utils/power_draw_append.py
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 talos-1.4/talos/utils/recover_best_model.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 talos-1.4/talos/utils/rescale_meanzero.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 talos-1.4/talos/utils/sequence_generator.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 talos-1.4/talos/utils/test_utils.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 talos-1.4/talos/utils/torch_history.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 talos-1.4/talos/utils/validation_split.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 talos-1.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 talos-1.4/LICENSE
+-rwxr-xr-x   0        0        0     6429 2020-02-02 00:00:00.000000 talos-1.4/README.md
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 talos-1.4/pyproject.toml
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 talos-1.4/PKG-INFO
```

### Comparing `talos-1.3/LICENSE` & `talos-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `talos-1.3/README.md` & `talos-1.4/README.md`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/__init__.py` & `talos-1.4/talos/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,8 @@
         if key.startswith('__') is False:
             if key not in keep_from_templates:
                 delattr(sub, key)
 
 del commands, scan, model, metrics, key
 del sub, keep_from_templates, template_sub, warnings
 
-__version__ = "1.3"
+__version__ = "1.4"
```

### Comparing `talos-1.3/talos/autom8/automodel.py` & `talos-1.4/talos/autom8/automodel.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/autom8/autoparams.py` & `talos-1.4/talos/autom8/autoparams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
-from tensorflow.keras.optimizers import Adam, Nadam, Adadelta, SGD
+from tensorflow.keras.optimizers.legacy import Adam, Adagrad, SGD
 
 
-loss = {'binary': ['binary_crossentropy', 'logcosh'],
+loss = {'binary': ['binary_crossentropy', 'LogCosh'],
         'multi_class': ['sparse_categorical_crossentropy'],
         'multi_label': ['categorical_crossentropy'],
         'continuous': ['mae']}
 
 last_activation = {'binary': ['sigmoid'],
                    'multi_class': ['softmax'],
                    'multi_label': ['softmax'],
@@ -118,15 +118,15 @@
 
         '''If `optimizers='auto'` then optimizers will be picked based on
         automatically. Otherwise input a list with one or
         more optimizers will be used.
         '''
 
         if optimizers == 'auto':
-            self._append_params('optimizer', [Adam, Nadam, Adadelta, SGD])
+            self._append_params('optimizer', [Adam, Adagrad, SGD])
         else:
             self._append_params('optimizer', optimizers)
 
     def activations(self, activations='auto'):
 
         '''If `activations='auto'` then activations will be picked based on
         automatically. Otherwise input a list with one or
@@ -164,27 +164,27 @@
 
     def batch_size(self, min_size=8, max_size=None, steps=None):
 
         '''`max_size` and `steps` has to be either `None` or
         integer value at the same time.'''
 
         if max_size is None and steps is None:
-            values = [int(np.exp2(i/2)) for i in range(3, 15)]
+            values = [int(np.exp2(i / 2)) for i in range(3, 15)]
         else:
             values = list(range(min_size, max_size, steps))
 
         self._append_params('batch_size', values)
 
     def epochs(self, min_epochs=50, max_epochs=None, steps=None):
 
         '''`max_epochs` and `steps` has to be either `None` or
         integer value at the same time.'''
 
         if max_epochs is None and steps is None:
-            values = [int(np.exp2(i/2))+50 for i in range(3, 15)]
+            values = [int(np.exp2(i / 2)) + 50 for i in range(3, 15)]
         else:
             values = list(range(min_epochs, max_epochs, steps))
 
         self._append_params('epochs', values)
 
     def kernel_initializers(self, kernel_inits='auto'):
```

### Comparing `talos-1.3/talos/autom8/autopredict.py` & `talos-1.4/talos/autom8/autopredict.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/autom8/autoscan.py` & `talos-1.4/talos/autom8/autoscan.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/callbacks/experiment_log.py` & `talos-1.4/talos/callbacks/experiment_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,28 +8,30 @@
                  params):
 
         '''Takes as input the name of the experiment which will be
         used for creating a .log file with the outputs and the params
         dictionary from the input model in `Scan()`
 
         experiment_name | str | must match the experiment_name in `Scan()`
+        params | dict | the params dictionary from the input model in `Scan()
 
         '''
 
         super(ExperimentLog, self).__init__()
 
         import glob
         import os
 
         # get the experiment id first
         list_of_files = glob.glob('./' + experiment_name + '/*.csv')
+
         try:
             latest_file = max(list_of_files, key=os.path.getmtime)
         except ValueError:
-            print("\n TALOS ERROR: `experiment_name` has to match `Scan(experiment_name)`\n")
+            print("\nERROR: `experiment_name` has to match `Scan(experiment_name)`\n")
 
         self.name = latest_file.replace('.csv', '') + '.log'
 
         # rest of the config variables
         self.params = params
         self.counter = 1
         self.new_file = True
```

### Comparing `talos-1.3/talos/callbacks/power_draw.py` & `talos-1.4/talos/callbacks/power_draw.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/commands/analyze.py` & `talos-1.4/talos/commands/analyze.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/commands/deploy.py` & `talos-1.4/talos/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/commands/evaluate.py` & `talos-1.4/talos/commands/evaluate.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/commands/predict.py` & `talos-1.4/talos/commands/predict.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/commands/restore.py` & `talos-1.4/talos/commands/restore.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/logging/logging_run.py` & `talos-1.4/talos/logging/logging_run.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/logging/results.py` & `talos-1.4/talos/logging/results.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/metrics/entropy.py` & `talos-1.4/talos/metrics/entropy.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/metrics/keras_metrics.py` & `talos-1.4/talos/metrics/keras_metrics.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/model/early_stopper.py` & `talos-1.4/talos/model/early_stopper.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/model/hidden_layers.py` & `talos-1.4/talos/model/hidden_layers.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/model/network_shape.py` & `talos-1.4/talos/model/network_shape.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/model/normalizers.py` & `talos-1.4/talos/model/normalizers.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,23 +7,21 @@
     ----------
     lr : float
         The learning rate.
     optimizer : keras optimizer
         The optimizer. For example, Adagrad, Adam, RMSprop.
     """
 
-    from tensorflow.keras.optimizers import SGD, Adam, Adadelta, Adagrad, Adamax, RMSprop
-    from tensorflow.keras.optimizers import Nadam
+    from tensorflow.keras.optimizers.legacy import SGD, Adam, Adagrad, Adamax, RMSprop
+    from tensorflow.keras.optimizers.legacy import Adagrad
     from talos.utils.exceptions import TalosModelError
 
-    if optimizer == Adadelta:
-        pass
-    elif optimizer == SGD or optimizer == Adagrad:
+    if optimizer == SGD or optimizer == Adagrad:
         lr /= 100.0
     elif optimizer == Adam or optimizer == RMSprop:
         lr /= 1000.0
-    elif optimizer == Adamax or optimizer == Nadam:
+    elif optimizer == Adamax:
         lr /= 500.0
     else:
         raise TalosModelError(str(optimizer) + " is not supported by lr_normalizer")
 
     return lr
```

### Comparing `talos-1.3/talos/model/output_layer.py` & `talos-1.4/talos/model/output_layer.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/parameters/DistributeParamSpace.py` & `talos-1.4/talos/parameters/DistributeParamSpace.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/parameters/ParamSpace.py` & `talos-1.4/talos/parameters/ParamSpace.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/reducers/GamifyMap.py` & `talos-1.4/talos/reducers/GamifyMap.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/reducers/correlation.py` & `talos-1.4/talos/reducers/correlation.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/reducers/forrest.py` & `talos-1.4/talos/reducers/forrest.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/reducers/gamify.py` & `talos-1.4/talos/reducers/gamify.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/reducers/limit_by_metric.py` & `talos-1.4/talos/reducers/limit_by_metric.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/reducers/reduce_run.py` & `talos-1.4/talos/reducers/reduce_run.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/reducers/reduce_utils.py` & `talos-1.4/talos/reducers/reduce_utils.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/reducers/sample_reducer.py` & `talos-1.4/talos/reducers/sample_reducer.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/reducers/trees.py` & `talos-1.4/talos/reducers/trees.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/scan/Scan.py` & `talos-1.4/talos/scan/Scan.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/scan/scan_addon.py` & `talos-1.4/talos/scan/scan_addon.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/scan/scan_finish.py` & `talos-1.4/talos/scan/scan_finish.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/scan/scan_prepare.py` & `talos-1.4/talos/scan/scan_prepare.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/scan/scan_round.py` & `talos-1.4/talos/scan/scan_round.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/scan/scan_run.py` & `talos-1.4/talos/scan/scan_run.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/scan/scan_utils.py` & `talos-1.4/talos/scan/scan_utils.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/templates/datasets.py` & `talos-1.4/talos/templates/datasets.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,54 +14,60 @@
     quantile is for transforming the otherwise continuous y variables into
     labels so that higher value is stronger. If set to 0 then original
     continuous will be returned.'''
 
     import wrangle
     import pandas as pd
 
-    df = pd.read_csv('https://raw.githubusercontent.com/autonomio/examples/master/telco_churn/telco_churn_for_sensitivity.csv')
+    base_url = 'https://raw.githubusercontent.com/autonomio/'
+    url = 'examples/master/telco_churn/telco_churn_for_sensitivity.csv'
+    df = pd.read_csv(base_url + url)
 
-    df = df.drop(['val_acc', 'loss', 'f1score', 'acc', 'round_epochs'], 1)
+    df = df.drop(['val_acc', 'loss', 'f1score', 'acc', 'round_epochs'], axis=1)
 
     for col in df.iloc[:, 2:].columns:
         df = wrangle.col_to_multilabel(df, col)
 
     df = wrangle.df_rename_cols(df)
 
     if quantile > 0:
         y1 = (df.C0 < df.C0.quantile(quantile)).astype(int).values
         y2 = (df.C1 > df.C1.quantile(quantile)).astype(int).values
     else:
         y1 = df.C0.values
         y2 = df.C1.values
 
-    x = df.drop(['C0', 'C1'], 1).values
+    x = df.drop(['C0', 'C1'], axis=1).values
 
     return x, [y1, y2]
 
 
 def icu_mortality(samples=None):
 
     import pandas as pd
-    base = 'https://raw.githubusercontent.com/autonomio/datasets/master/autonomio-datasets/'
-    df = pd.read_csv(base + 'icu_mortality.csv')
+
+    base_url = 'https://raw.githubusercontent.com/autonomio/'
+    url = 'datasets/master/autonomio-datasets/'
+    df = pd.read_csv(base_url + url + 'icu_mortality.csv')
     df = df.dropna(thresh=3580, axis=1)
     df = df.dropna()
     df = df.sample(frac=1).head(samples)
     y = df['hospitalmortality'].astype(int).values
     x = df.drop('hospitalmortality', axis=1).values
 
     return x, y
 
 
 def titanic():
 
     import pandas as pd
-    base = 'https://raw.githubusercontent.com/autonomio/datasets/master/autonomio-datasets/'
-    df = pd.read_csv(base + 'titanic.csv')
+
+    base_url = 'https://raw.githubusercontent.com/autonomio/'
+    url = 'datasets/master/autonomio-datasets/'
+    df = pd.read_csv(base_url + url + 'titanic.csv')
 
     y = df.survived.values
 
     x = df[['age', 'sibsp', 'parch']]
     cols = ['class', 'embark_town', 'who', 'deck', 'sex']
 
     for col in cols:
@@ -77,16 +83,18 @@
     return x, y
 
 
 def iris():
 
     import pandas as pd
     from tensorflow.keras.utils import to_categorical
-    base = 'https://raw.githubusercontent.com/autonomio/datasets/master/autonomio-datasets/'
-    df = pd.read_csv(base + 'iris.csv')
+
+    base_url = 'https://raw.githubusercontent.com/autonomio/'
+    url = 'datasets/master/autonomio-datasets/'
+    df = pd.read_csv(base_url + url + 'iris.csv')
     df['species'] = df['species'].factorize()[0]
     df = df.sample(len(df))
     y = to_categorical(df['species'])
     x = df.iloc[:, :-1].values
 
     y = to_categorical(df['species'])
     x = df.iloc[:, :-1].values
@@ -94,16 +102,18 @@
     return x, y
 
 
 def cervical_cancer():
 
     import pandas as pd
     from numpy import nan
-    base = 'https://raw.githubusercontent.com/autonomio/datasets/master/autonomio-datasets/'
-    df = pd.read_csv(base + 'cervical_cancer.csv')
+
+    base_url = 'https://raw.githubusercontent.com/autonomio/'
+    url = 'datasets/master/autonomio-datasets/'
+    df = pd.read_csv(base_url + url + 'cervical_cancer.csv')
     df = df.replace('?', nan)
     df = df.drop(['citology', 'hinselmann', 'biopsy'], axis=1)
     df = df.drop(['since_first_diagnosis',
                   'since_last_diagnosis'], axis=1).dropna()
 
     df = df.astype(float)
 
@@ -112,16 +122,18 @@
 
     return x, y
 
 
 def breast_cancer():
 
     import pandas as pd
-    base = 'https://raw.githubusercontent.com/autonomio/datasets/master/autonomio-datasets/'
-    df = pd.read_csv(base + 'breast_cancer.csv')
+
+    base_url = 'https://raw.githubusercontent.com/autonomio/'
+    url = 'datasets/master/autonomio-datasets/'
+    df = pd.read_csv(base_url + url + 'breast_cancer.csv')
 
     # then some minimal data cleanup
     df.drop("Unnamed: 32", axis=1, inplace=True)
     df.drop("id", axis=1, inplace=True)
 
     # separate to x and y
     y = df.diagnosis.values
```

### Comparing `talos-1.3/talos/templates/models.py` & `talos-1.4/talos/templates/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,20 +99,21 @@
 
     # here are using a learning rate boundary
     model.compile(optimizer=params['optimizer'],
                   loss=params['losses'],
                   metrics=['acc'])
 
     # here we are also using the early_stopper function for a callback
-    out = model.fit(x=x_train,
-                    y=y_train,
+    out = model.fit(x=x_train.astype('float32'),
+                    y=y_train.astype('float32'),
                     batch_size=params['batch_size'],
                     epochs=params['epochs'],
                     verbose=0,
-                    validation_data=(x_val, y_val))
+                    validation_data=(x_val.astype('float32'),
+                                     y_val.astype('float32')))
 
     return out, model
 
 
 def iris(x_train, y_train, x_val, y_val, params):
 
     from tensorflow.keras.models import Sequential
```

### Comparing `talos-1.3/talos/templates/params.py` & `talos-1.4/talos/templates/params.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,79 @@
 def titanic(debug=False):
 
-    from tensorflow.keras.optimizers import Adam, Nadam
+    from tensorflow.keras.optimizers.legacy import Adam, Adagrad
 
     # here use a standard 2d dictionary for inputting the param boundaries
     p = {'lr': (0.5, 5, 10),
          'first_neuron': [4, 8, 16],
          'batch_size': [20, 30, 40],
          'dropout': (0, 0.5, 5),
-         'optimizer': [Adam(), Nadam()],
+         'optimizer': [Adam(), Adagrad()],
          'epochs': [50, 100, 150],
-         'losses': ['logcosh', 'binary_crossentropy'],
+         'losses': ['LogCosh', 'binary_crossentropy'],
          'shapes': ['brick', 'triangle', 0.2],
          'hidden_layers': [0, 1, 2, 3, 4],
          'activation': ['relu', 'elu'],
          'last_activation': ['sigmoid']}
 
     if debug:
          
         p = {'lr': [0.1, 0.2],
-            'first_neuron': [4, 8],
-            'batch_size': [20, 30],
-            'dropout': [0.2, 0.3],
-            'optimizer': [Adam(), Nadam()],
-            'epochs': [50, 100],
-            'losses': ['logcosh', 'binary_crossentropy'],
-            'shapes': ['brick', 'triangle', 0.2],
-            'hidden_layers': [0, 1],
-            'activation': ['relu', 'elu'],
-            'last_activation': ['sigmoid']}
+             'first_neuron': [4, 8],
+             'batch_size': [20, 30],
+             'dropout': [0.2, 0.3],
+             'optimizer': [Adam(), Adagrad()],
+             'epochs': [50, 100],
+             'losses': ['LogCosh', 'binary_crossentropy'],
+             'shapes': ['brick', 'triangle', 0.2],
+             'hidden_layers': [0, 1],
+             'activation': ['relu', 'elu'],
+             'last_activation': ['sigmoid']}
 
     return p
 
 
 def iris():
 
-    from tensorflow.keras.optimizers import Adam, Nadam
-    from tensorflow.keras.losses import logcosh, categorical_crossentropy
+    from tensorflow.keras.optimizers.legacy import Adam, Adagrad
     from tensorflow.keras.activations import relu, elu, softmax
 
     # here use a standard 2d dictionary for inputting the param boundaries
     p = {'lr': (0.5, 5, 10),
          'first_neuron': [4, 8, 16, 32, 64],
          'hidden_layers': [0, 1, 2, 3, 4],
          'batch_size': (2, 30, 10),
          'epochs': [50, 100, 150],
          'dropout': (0, 0.5, 5),
          'weight_regulizer': [None],
          'emb_output_dims': [None],
          'shapes': ['brick', 'triangle', 0.2],
-         'optimizer': [Adam, Nadam],
-         'losses': [logcosh, categorical_crossentropy],
+         'optimizer': [Adam, Adagrad],
+         'losses': ['LogCosh', 'categorical_crossentropy'],
          'activation': [relu, elu],
          'last_activation': [softmax]}
 
     return p
 
 
 def breast_cancer():
 
-    from tensorflow.keras.optimizers import Adam, Nadam, RMSprop
-    from tensorflow.keras.losses import logcosh, binary_crossentropy
+    from tensorflow.keras.optimizers.legacy import Adam, Adagrad, RMSprop
     from tensorflow.keras.activations import relu, elu, sigmoid
 
     # then we can go ahead and set the parameter space
     p = {'lr': (0.5, 5, 10),
          'first_neuron': [4, 8, 16, 32, 64],
          'hidden_layers': [0, 1, 2],
          'batch_size': (2, 30, 10),
          'epochs': [50, 100, 150],
          'dropout': (0, 0.5, 5),
          'shapes': ['brick', 'triangle', 'funnel'],
-         'optimizer': [Adam, Nadam, RMSprop],
-         'losses': [logcosh, binary_crossentropy],
+         'optimizer': [Adam, Adagrad, RMSprop],
+         'losses': ['LogCosh', 'binary_crossentropy'],
          'activation': [relu, elu],
          'last_activation': [sigmoid]}
 
     return p
 
 
 def cervical_cancer():
```

### Comparing `talos-1.3/talos/templates/pipelines.py` & `talos-1.4/talos/templates/pipelines.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,16 +40,17 @@
     return scan_object
 
 
 def titanic(round_limit=2, random_method='uniform_mersenne', debug=False):
 
     '''Performs a Scan with Iris dataset and simple dense net'''
     import talos as ta
-    scan_object = ta.Scan(ta.templates.datasets.titanic()[0],
-                          ta.templates.datasets.titanic()[1],
+
+    scan_object = ta.Scan(ta.templates.datasets.titanic()[0].astype('float32'),
+                          ta.templates.datasets.titanic()[1].astype('float32'),
                           ta.templates.params.titanic(debug),
                           ta.templates.models.titanic,
                           'test',
                           random_method=random_method,
                           round_limit=round_limit)
 
     return scan_object
```

### Comparing `talos-1.3/talos/utils/__init__.py` & `talos-1.4/talos/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/utils/best_model.py` & `talos-1.4/talos/utils/best_model.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/utils/generator.py` & `talos-1.4/talos/utils/generator.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/utils/gpu_utils.py` & `talos-1.4/talos/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/utils/load_model.py` & `talos-1.4/talos/utils/load_model.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/utils/power_draw_append.py` & `talos-1.4/talos/utils/power_draw_append.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/utils/recover_best_model.py` & `talos-1.4/talos/utils/recover_best_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     results = []
     models = []
 
     for i in range(n_models):
 
         # get the params for the model and train it
         params = df.sort_values(metric, ascending=False)
-        params = params.drop(metric, 1).iloc[i].to_dict()
+        params = params.drop(metric, axis=1).iloc[i].to_dict()
         _history, model = input_model(x_train, y_train, x_val, y_val, params)
 
         # start kfold cross-validation
         out = []
         folds = 5
         kx, ky = kfold(x_cross, y_cross, folds, True, multi_input)
```

### Comparing `talos-1.3/talos/utils/sequence_generator.py` & `talos-1.4/talos/utils/sequence_generator.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/utils/test_utils.py` & `talos-1.4/talos/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/utils/torch_history.py` & `talos-1.4/talos/utils/torch_history.py`

 * *Files identical despite different names*

### Comparing `talos-1.3/talos/utils/validation_split.py` & `talos-1.4/talos/utils/validation_split.py`

 * *Files identical despite different names*


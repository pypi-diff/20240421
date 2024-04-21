# Comparing `tmp/sequifier-1.1.4.tar.gz` & `tmp/sequifier-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequifier-1.1.4.tar", max compression
+gzip compressed data, was "sequifier-2.0.0.tar", max compression
```

## Comparing `sequifier-1.1.4.tar` & `sequifier-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1669 2023-03-04 16:53:28.333432 sequifier-1.1.4/LICENSE
--rw-r--r--   0        0        0     5327 2024-02-29 20:03:33.409992 sequifier-1.1.4/README.md
--rw-r--r--   0        0        0      859 2024-03-19 02:32:18.195922 sequifier-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1982 2024-02-29 20:03:33.518000 sequifier-1.1.4/src/sequifier/config/infer_config.py
--rw-r--r--   0        0        0     1071 2024-02-29 20:03:33.518000 sequifier-1.1.4/src/sequifier/config/preprocess_config.py
--rw-r--r--   0        0        0     5246 2024-03-06 20:00:52.776995 sequifier-1.1.4/src/sequifier/config/train_config.py
--rw-r--r--   0        0        0     1255 2024-03-19 02:32:18.195922 sequifier-1.1.4/src/sequifier/helpers.py
--rw-r--r--   0        0        0     6061 2024-02-29 20:03:33.522000 sequifier-1.1.4/src/sequifier/infer.py
--rw-r--r--   0        0        0     7200 2024-03-18 17:52:21.993151 sequifier-1.1.4/src/sequifier/preprocess.py
--rw-r--r--   0        0        0     2004 2024-02-29 20:03:33.522000 sequifier-1.1.4/src/sequifier/sequifier.py
--rw-r--r--   0        0        0    15921 2024-03-19 01:59:55.528378 sequifier-1.1.4/src/sequifier/train.py
--rw-r--r--   0        0        0     6507 1970-01-01 00:00:00.000000 sequifier-1.1.4/setup.py
--rw-r--r--   0        0        0     6415 1970-01-01 00:00:00.000000 sequifier-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1669 2024-04-06 10:15:07.075618 sequifier-2.0.0/LICENSE
+-rw-r--r--   0        0        0     5162 2024-04-20 13:01:12.270656 sequifier-2.0.0/README.md
+-rw-r--r--   0        0        0      919 2024-04-20 13:01:12.276139 sequifier-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4392 2024-04-20 13:01:12.276497 sequifier-2.0.0/src/sequifier/config/infer_config.py
+-rw-r--r--   0        0        0     2154 2024-04-20 13:01:12.276844 sequifier-2.0.0/src/sequifier/config/preprocess_config.py
+-rw-r--r--   0        0        0     7002 2024-04-20 13:01:12.277183 sequifier-2.0.0/src/sequifier/config/train_config.py
+-rw-r--r--   0        0        0     2321 2024-04-20 13:01:12.277557 sequifier-2.0.0/src/sequifier/helpers.py
+-rw-r--r--   0        0        0    17469 2024-04-20 13:01:12.278025 sequifier-2.0.0/src/sequifier/infer.py
+-rw-r--r--   0        0        0    12294 2024-04-20 13:01:12.278244 sequifier-2.0.0/src/sequifier/preprocess.py
+-rw-r--r--   0        0        0     2234 2024-04-20 13:01:12.278568 sequifier-2.0.0/src/sequifier/sequifier.py
+-rw-r--r--   0        0        0    22884 2024-04-20 13:01:12.278993 sequifier-2.0.0/src/sequifier/train.py
+-rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 sequifier-2.0.0/PKG-INFO
```

### Comparing `sequifier-1.1.4/LICENSE` & `sequifier-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sequifier-1.1.4/README.md` & `sequifier-2.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 \
 \
 \
 ## Overview
 The sequifier package enables:
   - the extraction of sequences for training
-  - the configuration and training of a transformer classification model
+  - the configuration and training of a transformer classification or regression model
+  - using multiple input and output sequences
   - inference on data with a trained model
 
 
 ## Other materials 
 If you want to first get a more specific understanding of the transformer architecture, have a look at
 the [Wikipedia article.](https://en.wikipedia.org/wiki/Transformer_(machine_learning_model))
 
@@ -33,49 +34,47 @@
 pip install sequifier
 ```
 2. create a new project folder (at a path referred to as `PROJECT PATH` later) and a `configs` subfolder
 3. copy default configs from repository for preprocessing, training and inference
 4. adapt preprocess config to take the path to the data you want to preprocess and set `project_path` to`PROJECT PATH`
 5. run 
 ```console
-sequifier --preprocess --config_path=[PROJECT PATH]/configs/preprocess.yaml
+sequifier preprocess --config_path=[PROJECT PATH]/configs/preprocess.yaml
 ```
 6. the preprocessing step outputs a "data driven config" at `[PROJECT PATH]/configs/ddconfigs/[FILE NAME]`. It contains the number of classes found in the data, a map of classes to indices and the oaths to train, validation and test splits of data. Adapt the `dd_config` parameter in `train-on-preprocessed.yaml` and `infer.yaml` in to the path `[PROJECT PATH]/configs/ddconfigs/[FILE NAME]`and set `project_path` to `PROJECT PATH` in both configs
 7. run
 ```console
-sequifier --train --on-preprocessed --config_path=[PROJECT PATH]/configs/train-on-preprocessed.yaml
+sequifier train --config_path=[PROJECT PATH]/configs/train-on-preprocessed.yaml
 ```
-8. adapt `inference_data_path` in `infer.yaml`
+8. adapt `data_path` in `infer.yaml`
 9. run
 ```console
-sequifier --infer --config_path=[PROJECT PATH]/configs/infer.yaml
+sequifier infer --config_path=[PROJECT PATH]/configs/infer.yaml
 ```
-10. find your predictions at `[PROJECT PATH]/outputs/predictions/sequifier-default-best_predictions.csv`
+10. find your predictions at `[PROJECT PATH]/outputs/predictions/sequifier-default-best-predictions.csv`
 
 
 ## More detailed explanations of the three steps
 #### Preprocessing of data into sequences for training
 
 The preprocessing step is designed for scenarios where for timeseries or timeseries-like data,
-the prediction of the next data point of a particular variable from prior values of that variable
-and (optionally) other variables is of interest.
-In cases of sequences where only the last item is a valid target, the preprocessing
-step should not be executed.
+the prediction of the next data point of one or more variables from prior values of these
+variables and (optionally) other variables is of interest.
 
 This step presupposes input data with three columns: "sequenceId" and "itemPosition", and a column
 with the variable that is the prediction target.
 "sequenceId" separates different sequences and the itemPosition column
 provides values that enable sequential sorting. Often this will simply be a timestamp.
 You can find an example of the preprocessing input data at [documentation/example_inputs/preprocessing_input.csv](./documentation/example_inputs/preprocessing_input.csv)
 
 The data can then be processed and split into training, validation and testing datasets of all
 valid subsequences in the original data with the command:
 
 ```console
-sequifier --preprocess --config_path=[CONFIG PATH]
+sequifier preprocess --config_path=[CONFIG PATH]
 ```
 
 The config path specifies the path to the preprocessing config and the project
 path the path to the (preferably empty) folder the output files of the different
 steps are written to.
 
 The default config can be found on this path:
@@ -85,44 +84,42 @@
 
 
 #### Configuring and training the sequence classification model
 
 The training step is executed with the command:
 
 ```console
-sequifier --train --config_path=[CONFIG PATH]
+sequifier train --config_path=[CONFIG PATH]
 ```
 
-If the data on which the model is trained comes from the preprocessing step, the flag
+If the data on which the model is trained DOES NOT come from the preprocessing step, the flag
 
 ```console
---on-preprocessed
+--on-unprocessed
 ```
 
-should also be added.
+should be added.
 
 If the training data does not come from the preprocessing step, both train and validation
 data have to take the form of a csv file with the columns "sequenceId", "subsequenceId", "col_name", [SEQ LENGTH], [SEQ LENGTH - 1],...,"1", "target".
 You can find an example of the preprocessing input data at [documentation/example_inputs/training_input.csv](./documentation/example_inputs/training_input.csv)
 
 The training step is configured using the config. The two default configs can be found here:
 
 [configs/train.yaml](./configs/train.yaml)
 
-[configs/train-on-preprocessed.yaml](./configs/train-on-preprocessed.yaml)
-
 depending on whether the preprocessing step was executed.
 
 
 #### Inferring on test data using the trained model
 
 Inference is done using the command:
 
 ```console
-sequifier --infer --config_path=[CONFIG PATH]
+sequifier infer --config_path=[CONFIG PATH]
 ```
 
 and configured using a config file. The default version can be found here:
 
 [configs/infer.yaml](./configs/infer.yaml)
```

### Comparing `sequifier-1.1.4/pyproject.toml` & `sequifier-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sequifier"
-version = "1.1.4"
+version = "2.0.0"
 authors = ["Leon Luithlen <leontimnaluithlen@gmail.com>"]
 description = "Train a transformer model with the command line"
 keywords = ["transformer", "sequence classification", "machine learning", "sequence", "sequence modelling", "nlp", "language", "language modelling", "torch", "pytorch"]
 readme = "README.md"
 license = "BSD 3-Clause"
 homepage = "https://github.com/0xideas/sequifier"
 repository = "https://github.com/0xideas/sequifier"
@@ -20,14 +20,17 @@
 torch = "^2.0"
 onnx = "^1.15.0"
 onnxruntime = "^1.17"
 pyyaml = "^6.0"
 pydantic = "^1.10"
 poetry = "^1.3"
 pytest = "^7.2"
+csvkit = "^1.0"
+pyarrow = "^15.0"
+fastparquet = "^2024.2.0"
 
 [tool.poetry.scripts]
 sequifier = 'sequifier.sequifier:main'
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `sequifier-1.1.4/src/sequifier/config/train_config.py` & `sequifier-2.0.0/src/sequifier/config/train_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,51 @@
 import copy
 import json
 import os
 from dataclasses import dataclass
 from typing import Dict, Optional, Union
 
+import numpy as np
 import yaml
 from pydantic import BaseModel, validator
 
+from sequifier.helpers import normalize_path
+
 ANYTYPE = Union[str, int, float]
 
 
-class DotDict(dict):
-    """dot.notation access to dictionary attributes"""
+def load_transformer_config(config_path, args_config, on_unprocessed):
+    with open(config_path, "r") as f:
+        config_values = yaml.safe_load(f)
 
-    __getattr__ = dict.get
-    __setattr__ = dict.__setitem__
-    __delattr__ = dict.__delitem__
+    config_values.update(args_config)
 
-    def __deepcopy__(self, memo=None):
-        return DotDict(copy.deepcopy(dict(self), memo=memo))
+    if not on_unprocessed:
+        dd_config_path = config_values.pop("ddconfig_path")
 
+        with open(
+            normalize_path(dd_config_path, config_values["project_path"]), "r"
+        ) as f:
+            dd_config = json.loads(f.read())
+
+        config_values["column_types"] = dd_config["column_types"]
+        config_values["categorical_columns"] = [
+            col for col, type_ in dd_config["column_types"].items() if type_ == "int64"
+        ]
+        config_values["real_columns"] = [
+            col
+            for col, type_ in dd_config["column_types"].items()
+            if type_ == "float64"
+        ]
+        config_values["n_classes"] = dd_config["n_classes"]
+        config_values["training_data_path"] = dd_config["split_paths"][0]
+        config_values["validation_data_path"] = dd_config["split_paths"][1]
+
+    return TransformerModel(**config_values)
 
-CustomValidation = Optional
 
 VALID_LOSS_FUNCTIONS = [
     "L1Loss",
     "MSELoss",
     "CrossEntropyLoss",
     "CTCLoss",
     "NLLLoss",
@@ -76,44 +96,68 @@
     "ReduceLROnPlateau",
     "CyclicLR",
     "OneCycleLR",
     "CosineAnnealingWarmRestarts",
 ]
 
 
+class DotDict(dict):
+    """dot.notation access to dictionary attributes"""
+
+    __getattr__ = dict.get
+    __setattr__ = dict.__setitem__
+    __delattr__ = dict.__delitem__
+
+    def __deepcopy__(self, memo=None):
+        return DotDict(copy.deepcopy(dict(self), memo=memo))
+
+
+CustomValidation = Optional
+
+
 @dataclass
 class TrainingSpecModel(BaseModel):
     device: str
     epochs: int
+    log_interval: int = 10
+    early_stopping_epochs: Optional[int]
     iter_save: int
     batch_size: int
     lr: float  # learning rate
-    dropout: float
-    criterion: str
-    optimizer: CustomValidation[DotDict]  # mandatory
-    scheduler: CustomValidation[DotDict]  # mandatory
-    continue_training: bool
+    criterion: dict[str, str]
+    accumulation_steps: Optional[int]
+    dropout: float = 0.0
+    loss_weights: Optional[dict[str, float]]
+    optimizer: CustomValidation[DotDict]  # mandatory; default value in __init__
+    scheduler: CustomValidation[DotDict]  # mandatory; default value in __init__
+    continue_training: bool = True
 
     def __init__(self, **kwargs):
 
         super().__init__(
             **{k: v for k, v in kwargs.items() if k not in ["optimizer", "scheduler"]}
         )
 
-        optimizer = kwargs.get("optimizer")
-        scheduler = kwargs.get("scheduler")
+        optimizer = kwargs.get("optimizer", {"name": "Adam"})
+        scheduler = kwargs.get(
+            "scheduler", {"name": "StepLR", "step_size": 1, "gamma": 0.99}
+        )
+
         self.validate_optimizer_config(optimizer)
         self.optimizer = DotDict(optimizer)
         self.validate_scheduler_config(scheduler)
         self.scheduler = DotDict(scheduler)
 
     @validator("criterion")
     def validate_criterion(cls, v):
-        if v not in VALID_LOSS_FUNCTIONS:
-            raise ValueError(f"criterion must be in {VALID_LOSS_FUNCTIONS}")
+        for vv in v.values():
+            if vv not in VALID_LOSS_FUNCTIONS:
+                raise ValueError(
+                    f"criterion must be in {VALID_LOSS_FUNCTIONS}, {vv} isn't"
+                )
         return v
 
     @staticmethod
     def validate_optimizer_config(v):
         if "name" not in v:
             raise ValueError("optimizer dict must specify 'name' field")
         if v["name"] not in VALID_OPTIMIZERS:
@@ -133,66 +177,69 @@
     d_hid: int
     nlayers: int
 
 
 class TransformerModel(BaseModel):
     project_path: str
     model_name: Optional[str]
-    seq_length: int
-    n_classes: dict[str, int]
     training_data_path: str
     validation_data_path: str
-    seed: int
+    read_format: str = "parquet"
+
+    selected_columns: Optional[list[str]]
     column_types: dict[str, str]
     categorical_columns: list[str]
     real_columns: list[str]
-    target_column: str
-    target_column_type: str
-    log_interval: int
+    target_columns: list[str]
+    target_column_types: dict[str, str]
+
+    seq_length: int
+    n_classes: dict[str, int]
+    inference_batch_size: int
+    seed: int
+
+    export_onnx: bool = True
+    export_pt: bool = False
+    export_with_dropout: bool = False
 
     model_spec: CustomValidation[ModelSpecModel]
     training_spec: CustomValidation[TrainingSpecModel]
 
-    @validator("target_column_type")
-    def validate_target_column_type(cls, v):
-        assert v in ["categorical", "real"]
+    @validator("target_column_types", always=True)
+    def validate_target_column_types(cls, v, values):
+        assert np.all([vv in ["categorical", "real"] for vv in v.values()])
+        assert np.all(
+            np.array(list(v.keys())) == np.array(values["target_columns"])
+        ), "target_columns and target_column_types must contain the same values/keys in the same order"
+        return v
+
+    @validator("read_format", always=True)
+    def validate_read_format(cls, v):
+        assert v in [
+            "csv",
+            "parquet",
+        ], "Currently only 'csv' and 'parquet' are supported"
         return v
 
     def __init__(self, **kwargs):
         super().__init__(
             **{
                 k: v
                 for k, v in kwargs.items()
                 if k not in ["model_spec", "training_spec"]
             }
         )
         self.model_spec = ModelSpecModel(**kwargs.get("model_spec"))
         self.training_spec = TrainingSpecModel(**kwargs.get("training_spec"))
 
-
-def load_transformer_config(config_path, args_config, on_preprocessed):
-    with open(config_path, "r") as f:
-        config_values = yaml.safe_load(f)
-
-    config_values.update(args_config)
-
-    if on_preprocessed:
-        dd_config_path = os.path.join(
-            config_values["project_path"], config_values.pop("ddconfig_path")
-        )
-        with open(dd_config_path, "r") as f:
-            dd_config = json.loads(f.read())
-
-        config_values["column_types"] = dd_config["column_types"]
-        config_values["categorical_columns"] = [
-            col for col, type_ in dd_config["column_types"].items() if type_ == "int64"
+        assert np.all(
+            np.array(self.target_columns)
+            == np.array(list(self.training_spec.criterion.keys()))
+        ), "target_columns and criterion must contain the same values/keys in the same order"
+
+        column_ordered = np.array(list(self.column_types.keys()))
+        columns_ordered_filtered = column_ordered[
+            np.array([c in self.target_columns for c in column_ordered])
         ]
-        config_values["real_columns"] = [
-            col
-            for col, type_ in dd_config["column_types"].items()
-            if type_ == "float64"
-        ]
-        config_values["n_classes"] = dd_config["n_classes"]
-        config_values["training_data_path"] = dd_config["split_paths"][0]
-        config_values["validation_data_path"] = dd_config["split_paths"][1]
-
-    return TransformerModel(**config_values)
+        assert np.all(
+            columns_ordered_filtered == np.array(self.target_columns)
+        ), f"{columns_ordered_filtered = } != {self.target_columns = }"
```

### Comparing `sequifier-1.1.4/src/sequifier/helpers.py` & `sequifier-2.0.0/src/sequifier/helpers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,81 @@
+import os
 import subprocess
 
+import numpy as np
+import pandas as pd
 import torch
 from torch import tensor
 
 PANDAS_TO_TORCH_TYPES = {"int64": torch.int64, "float64": torch.float32}
 
 
-def numpy_to_pytorch(data, column_types, target_column, seq_length, device):
+def read_data(path, read_format, columns=None):
+    if read_format == "csv":
+        return pd.read_csv(path, sep=",", decimal=".", index_col=False)
+    if read_format == "parquet":
+        return pd.read_parquet(path, columns=columns)
 
-    sequence = {
-        col: (
-            tensor(
-                data.query(f"inputCol=='{col}'")[
-                    [str(c) for c in range(seq_length, 0, -1)]
-                ].values
-            )
-            .to(column_types[col])
-            .to(device)
-        )
-        for col in column_types.keys()
-    }
+
+def write_data(data, path, write_format, **kwargs):
+    if write_format == "csv":
+        return data.to_csv(path, sep=",", decimal=".", index=False, **kwargs)
+    if write_format == "parquet":
+        return data.to_parquet(path)
+
+
+def subset_to_selected_columns(data, selected_columns):
+    column_filters = [
+        (data["inputCol"].values == input_col) for input_col in selected_columns
+    ]
+    filter_ = np.logical_or.reduce(column_filters)
+    return data.loc[filter_, :]
+
+
+def numpy_to_pytorch(data, column_types, target_columns, seq_length, device, to_device):
 
     if "target" in data:
-        target = (
-            tensor(data.query(f"inputCol=='{target_column}'")["target"].values)
-            .to(column_types[target_column])
-            .to(device)
-        )
+        targets = {}
+        for target_column in target_columns:
+            target = tensor(
+                data.query(f"inputCol=='{target_column}'")["target"].values
+            ).to(column_types[target_column])
+            if to_device:
+                target = target.to(device)
+            else:
+                target = None
+            targets[target_column] = target
     else:
-        target = None
+        targets = None
 
-    return (sequence, target)
+    sequence = {}
+    for col in column_types.keys():
+        f = data["inputCol"].values == col
+        data_subset = data.loc[f, [str(c) for c in range(seq_length, 0, -1)]].values
+        tens = tensor(data_subset).to(column_types[col])
+
+        if to_device:
+            tens = tens.to(device)
+
+        sequence[col] = tens
+
+    return (sequence, targets)
 
 
 class LogFile(object):
     def __init__(self, path, open_mode):
         self._file = open(path, open_mode)
         self._path = path
 
     def write(self, string):
         self._file.write(f"{string}\n")
         self._file.flush()
-        n_lines = string.count("\n")
-        output = subprocess.check_output(
-            f"tail -{n_lines} {self._path}", shell=True, text=True
-        )
-        print(output)
+        print(string)
 
     def close(self):
         self._file.close()
+
+
+def normalize_path(path, project_path):
+    project_path_normalized = (project_path + os.sep).replace(os.sep + os.sep, os.sep)
+    path2 = os.path.join(project_path, path.replace(project_path_normalized, ""))
+    return path2
```

### Comparing `sequifier-1.1.4/setup.py` & `sequifier-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,157 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sequifier
+Version: 2.0.0
+Summary: Train a transformer model with the command line
+Home-page: https://github.com/0xideas/sequifier
+License: BSD 3-Clause
+Keywords: transformer,sequence classification,machine learning,sequence,sequence modelling,nlp,language,language modelling,torch,pytorch
+Author: Leon Luithlen
+Author-email: leontimnaluithlen@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: csvkit (>=1.0,<2.0)
+Requires-Dist: fastparquet (>=2024.2.0,<2025.0.0)
+Requires-Dist: numpy (>=1.23,<2.0)
+Requires-Dist: onnx (>=1.15.0,<2.0.0)
+Requires-Dist: onnxruntime (>=1.17,<2.0)
+Requires-Dist: pandas (>=2.0,<3.0)
+Requires-Dist: poetry (>=1.3,<2.0)
+Requires-Dist: pyarrow (>=15.0,<16.0)
+Requires-Dist: pydantic (>=1.10,<2.0)
+Requires-Dist: pytest (>=7.2,<8.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: torch (>=2.0,<3.0)
+Project-URL: Repository, https://github.com/0xideas/sequifier
+Description-Content-Type: text/markdown
+
+<img src="./design/sequifier.png">
+
+
+### one-to-one and many-to-one autoregression made easy
+
+Sequifier enables sequence classification or regression for time based sequences using transformer models, via CLI.
+The specific configuration of preprocessing, which takes a single or multi-variable columnar data file and creates
+training, validation and test sequences, training, which trains a transformer model, and inference, which calculates
+model outputs for data (usually the test data from preprocessing), is done via configuration yaml files.
+
+\
+\
+\
+## Overview
+The sequifier package enables:
+  - the extraction of sequences for training
+  - the configuration and training of a transformer classification or regression model
+  - using multiple input and output sequences
+  - inference on data with a trained model
+
+
+## Other materials 
+If you want to first get a more specific understanding of the transformer architecture, have a look at
+the [Wikipedia article.](https://en.wikipedia.org/wiki/Transformer_(machine_learning_model))
+
+If you want to see a benchmark on a small synthetic dataset with 10k cases, agains a random forest,
+an xgboost model and a logistic regression, check out [this notebook.](./documentation/demos/benchmark-small-data.ipynb)
+
+
+## Complete example how to build and apply a transformer sequence classifier with sequifier
+
+1. create a conda environment with python >=3.9 activate and run
+```console
+pip install sequifier
+```
+2. create a new project folder (at a path referred to as `PROJECT PATH` later) and a `configs` subfolder
+3. copy default configs from repository for preprocessing, training and inference
+4. adapt preprocess config to take the path to the data you want to preprocess and set `project_path` to`PROJECT PATH`
+5. run 
+```console
+sequifier preprocess --config_path=[PROJECT PATH]/configs/preprocess.yaml
+```
+6. the preprocessing step outputs a "data driven config" at `[PROJECT PATH]/configs/ddconfigs/[FILE NAME]`. It contains the number of classes found in the data, a map of classes to indices and the oaths to train, validation and test splits of data. Adapt the `dd_config` parameter in `train-on-preprocessed.yaml` and `infer.yaml` in to the path `[PROJECT PATH]/configs/ddconfigs/[FILE NAME]`and set `project_path` to `PROJECT PATH` in both configs
+7. run
+```console
+sequifier train --config_path=[PROJECT PATH]/configs/train-on-preprocessed.yaml
+```
+8. adapt `data_path` in `infer.yaml`
+9. run
+```console
+sequifier infer --config_path=[PROJECT PATH]/configs/infer.yaml
+```
+10. find your predictions at `[PROJECT PATH]/outputs/predictions/sequifier-default-best-predictions.csv`
+
+
+## More detailed explanations of the three steps
+#### Preprocessing of data into sequences for training
+
+The preprocessing step is designed for scenarios where for timeseries or timeseries-like data,
+the prediction of the next data point of one or more variables from prior values of these
+variables and (optionally) other variables is of interest.
+
+This step presupposes input data with three columns: "sequenceId" and "itemPosition", and a column
+with the variable that is the prediction target.
+"sequenceId" separates different sequences and the itemPosition column
+provides values that enable sequential sorting. Often this will simply be a timestamp.
+You can find an example of the preprocessing input data at [documentation/example_inputs/preprocessing_input.csv](./documentation/example_inputs/preprocessing_input.csv)
+
+The data can then be processed and split into training, validation and testing datasets of all
+valid subsequences in the original data with the command:
+
+```console
+sequifier preprocess --config_path=[CONFIG PATH]
+```
+
+The config path specifies the path to the preprocessing config and the project
+path the path to the (preferably empty) folder the output files of the different
+steps are written to.
+
+The default config can be found on this path:
+
+[configs/preprocess.yaml](./configs/preprocess.yaml)
+
+
+
+#### Configuring and training the sequence classification model
+
+The training step is executed with the command:
+
+```console
+sequifier train --config_path=[CONFIG PATH]
+```
+
+If the data on which the model is trained DOES NOT come from the preprocessing step, the flag
+
+```console
+--on-unprocessed
+```
+
+should be added.
+
+If the training data does not come from the preprocessing step, both train and validation
+data have to take the form of a csv file with the columns "sequenceId", "subsequenceId", "col_name", [SEQ LENGTH], [SEQ LENGTH - 1],...,"1", "target".
+You can find an example of the preprocessing input data at [documentation/example_inputs/training_input.csv](./documentation/example_inputs/training_input.csv)
+
+The training step is configured using the config. The two default configs can be found here:
+
+[configs/train.yaml](./configs/train.yaml)
+
+depending on whether the preprocessing step was executed.
+
+
+#### Inferring on test data using the trained model
+
+Inference is done using the command:
+
+```console
+sequifier infer --config_path=[CONFIG PATH]
+```
 
-package_dir = \
-{'': 'src'}
+and configured using a config file. The default version can be found here:
 
-packages = \
-['sequifier', 'sequifier.config']
+[configs/infer.yaml](./configs/infer.yaml)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['numpy>=1.23,<2.0',
- 'onnx>=1.15.0,<2.0.0',
- 'onnxruntime>=1.17,<2.0',
- 'pandas>=2.0,<3.0',
- 'poetry>=1.3,<2.0',
- 'pydantic>=1.10,<2.0',
- 'pytest>=7.2,<8.0',
- 'pyyaml>=6.0,<7.0',
- 'torch>=2.0,<3.0']
-
-entry_points = \
-{'console_scripts': ['sequifier = sequifier.sequifier:main']}
-
-setup_kwargs = {
-    'name': 'sequifier',
-    'version': '1.1.4',
-    'description': 'Train a transformer model with the command line',
-    'long_description': '<img src="./design/sequifier.png">\n\n\n### one-to-one and many-to-one autoregression made easy\n\nSequifier enables sequence classification or regression for time based sequences using transformer models, via CLI.\nThe specific configuration of preprocessing, which takes a single or multi-variable columnar data file and creates\ntraining, validation and test sequences, training, which trains a transformer model, and inference, which calculates\nmodel outputs for data (usually the test data from preprocessing), is done via configuration yaml files.\n\n\\\n\\\n\\\n## Overview\nThe sequifier package enables:\n  - the extraction of sequences for training\n  - the configuration and training of a transformer classification model\n  - inference on data with a trained model\n\n\n## Other materials \nIf you want to first get a more specific understanding of the transformer architecture, have a look at\nthe [Wikipedia article.](https://en.wikipedia.org/wiki/Transformer_(machine_learning_model))\n\nIf you want to see a benchmark on a small synthetic dataset with 10k cases, agains a random forest,\nan xgboost model and a logistic regression, check out [this notebook.](./documentation/demos/benchmark-small-data.ipynb)\n\n\n## Complete example how to build and apply a transformer sequence classifier with sequifier\n\n1. create a conda environment with python >=3.9 activate and run\n```console\npip install sequifier\n```\n2. create a new project folder (at a path referred to as `PROJECT PATH` later) and a `configs` subfolder\n3. copy default configs from repository for preprocessing, training and inference\n4. adapt preprocess config to take the path to the data you want to preprocess and set `project_path` to`PROJECT PATH`\n5. run \n```console\nsequifier --preprocess --config_path=[PROJECT PATH]/configs/preprocess.yaml\n```\n6. the preprocessing step outputs a "data driven config" at `[PROJECT PATH]/configs/ddconfigs/[FILE NAME]`. It contains the number of classes found in the data, a map of classes to indices and the oaths to train, validation and test splits of data. Adapt the `dd_config` parameter in `train-on-preprocessed.yaml` and `infer.yaml` in to the path `[PROJECT PATH]/configs/ddconfigs/[FILE NAME]`and set `project_path` to `PROJECT PATH` in both configs\n7. run\n```console\nsequifier --train --on-preprocessed --config_path=[PROJECT PATH]/configs/train-on-preprocessed.yaml\n```\n8. adapt `inference_data_path` in `infer.yaml`\n9. run\n```console\nsequifier --infer --config_path=[PROJECT PATH]/configs/infer.yaml\n```\n10. find your predictions at `[PROJECT PATH]/outputs/predictions/sequifier-default-best_predictions.csv`\n\n\n## More detailed explanations of the three steps\n#### Preprocessing of data into sequences for training\n\nThe preprocessing step is designed for scenarios where for timeseries or timeseries-like data,\nthe prediction of the next data point of a particular variable from prior values of that variable\nand (optionally) other variables is of interest.\nIn cases of sequences where only the last item is a valid target, the preprocessing\nstep should not be executed.\n\nThis step presupposes input data with three columns: "sequenceId" and "itemPosition", and a column\nwith the variable that is the prediction target.\n"sequenceId" separates different sequences and the itemPosition column\nprovides values that enable sequential sorting. Often this will simply be a timestamp.\nYou can find an example of the preprocessing input data at [documentation/example_inputs/preprocessing_input.csv](./documentation/example_inputs/preprocessing_input.csv)\n\nThe data can then be processed and split into training, validation and testing datasets of all\nvalid subsequences in the original data with the command:\n\n```console\nsequifier --preprocess --config_path=[CONFIG PATH]\n```\n\nThe config path specifies the path to the preprocessing config and the project\npath the path to the (preferably empty) folder the output files of the different\nsteps are written to.\n\nThe default config can be found on this path:\n\n[configs/preprocess.yaml](./configs/preprocess.yaml)\n\n\n\n#### Configuring and training the sequence classification model\n\nThe training step is executed with the command:\n\n```console\nsequifier --train --config_path=[CONFIG PATH]\n```\n\nIf the data on which the model is trained comes from the preprocessing step, the flag\n\n```console\n--on-preprocessed\n```\n\nshould also be added.\n\nIf the training data does not come from the preprocessing step, both train and validation\ndata have to take the form of a csv file with the columns "sequenceId", "subsequenceId", "col_name", [SEQ LENGTH], [SEQ LENGTH - 1],...,"1", "target".\nYou can find an example of the preprocessing input data at [documentation/example_inputs/training_input.csv](./documentation/example_inputs/training_input.csv)\n\nThe training step is configured using the config. The two default configs can be found here:\n\n[configs/train.yaml](./configs/train.yaml)\n\n[configs/train-on-preprocessed.yaml](./configs/train-on-preprocessed.yaml)\n\ndepending on whether the preprocessing step was executed.\n\n\n#### Inferring on test data using the trained model\n\nInference is done using the command:\n\n```console\nsequifier --infer --config_path=[CONFIG PATH]\n```\n\nand configured using a config file. The default version can be found here:\n\n[configs/infer.yaml](./configs/infer.yaml)\n\n\n',
-    'author': 'Leon Luithlen',
-    'author_email': 'leontimnaluithlen@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/0xideas/sequifier',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
 
 
-setup(**setup_kwargs)
```


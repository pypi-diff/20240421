# Comparing `tmp/neuralnetlib-2.1.0.tar.gz` & `tmp/neuralnetlib-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralnetlib-2.1.0.tar", last modified: Sun Apr 21 01:33:55 2024, max compression
+gzip compressed data, was "neuralnetlib-2.2.0.tar", last modified: Sun Apr 21 13:25:18 2024, max compression
```

## Comparing `neuralnetlib-2.1.0.tar` & `neuralnetlib-2.2.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:55.892687 neuralnetlib-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 01:33:47.000000 neuralnetlib-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-21 01:33:55.892687 neuralnetlib-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-21 01:33:47.000000 neuralnetlib-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:55.892687 neuralnetlib-2.1.0/neuralnetlib/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-21 01:33:47.000000 neuralnetlib-2.1.0/neuralnetlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-21 01:33:47.000000 neuralnetlib-2.1.0/neuralnetlib/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)    18057 2024-04-21 01:33:47.000000 neuralnetlib-2.1.0/neuralnetlib/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-21 01:33:47.000000 neuralnetlib-2.1.0/neuralnetlib/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-21 01:33:47.000000 neuralnetlib-2.1.0/neuralnetlib/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-21 01:33:47.000000 neuralnetlib-2.1.0/neuralnetlib/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-04-21 01:33:47.000000 neuralnetlib-2.1.0/neuralnetlib/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-21 01:33:47.000000 neuralnetlib-2.1.0/neuralnetlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:55.892687 neuralnetlib-2.1.0/neuralnetlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-21 01:33:55.000000 neuralnetlib-2.1.0/neuralnetlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-21 01:33:55.000000 neuralnetlib-2.1.0/neuralnetlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 01:33:55.000000 neuralnetlib-2.1.0/neuralnetlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 01:33:55.000000 neuralnetlib-2.1.0/neuralnetlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 01:33:55.000000 neuralnetlib-2.1.0/neuralnetlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-21 01:33:55.892687 neuralnetlib-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-21 01:33:47.000000 neuralnetlib-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:25:18.445149 neuralnetlib-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 13:25:10.000000 neuralnetlib-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-21 13:25:18.445149 neuralnetlib-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-21 13:25:10.000000 neuralnetlib-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:25:18.441149 neuralnetlib-2.2.0/neuralnetlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-21 13:25:10.000000 neuralnetlib-2.2.0/neuralnetlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-21 13:25:10.000000 neuralnetlib-2.2.0/neuralnetlib/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18065 2024-04-21 13:25:10.000000 neuralnetlib-2.2.0/neuralnetlib/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-21 13:25:10.000000 neuralnetlib-2.2.0/neuralnetlib/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-21 13:25:10.000000 neuralnetlib-2.2.0/neuralnetlib/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-04-21 13:25:10.000000 neuralnetlib-2.2.0/neuralnetlib/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-04-21 13:25:10.000000 neuralnetlib-2.2.0/neuralnetlib/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-04-21 13:25:10.000000 neuralnetlib-2.2.0/neuralnetlib/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-21 13:25:10.000000 neuralnetlib-2.2.0/neuralnetlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:25:18.445149 neuralnetlib-2.2.0/neuralnetlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-21 13:25:18.000000 neuralnetlib-2.2.0/neuralnetlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-21 13:25:18.000000 neuralnetlib-2.2.0/neuralnetlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:25:18.000000 neuralnetlib-2.2.0/neuralnetlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 13:25:18.000000 neuralnetlib-2.2.0/neuralnetlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 13:25:18.000000 neuralnetlib-2.2.0/neuralnetlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-21 13:25:18.445149 neuralnetlib-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-21 13:25:10.000000 neuralnetlib-2.2.0/setup.py
```

### Comparing `neuralnetlib-2.1.0/LICENSE` & `neuralnetlib-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.1.0/PKG-INFO` & `neuralnetlib-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.1.0
+Version: 2.2.0
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -31,15 +31,15 @@
 
 Remember that this library is not optimized for performance, but for learning purposes (although I tried to make it as fast as possible).
 
 I intend to improve the neural networks and add more features in the future.
 
 ## 📦 Features
 
-- Many layers (input, activation, dense, conv2d, maxpooling2d, flatten) 🧠
+- Many layers (input, activation, dense, dropout, conv2d, maxpooling2d, flatten) 🧠
 - Many activation functions (sigmoid, tanh, relu, leaky relu, softmax, linear, elu, selu) 📈
 - Many loss functions (mean squared error, mean absolute error, categorical crossentropy, binary crossentropy, huber loss) 📉
 - Many optimizers (sgd, momentum, rmsprop, adam) 📊
 - Supports binary classification, multiclass classification and regression 📖
 - Save and load models 📁
 - Simple to use 📚
```

### Comparing `neuralnetlib-2.1.0/README.md` & `neuralnetlib-2.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Remember that this library is not optimized for performance, but for learning purposes (although I tried to make it as fast as possible).
 
 I intend to improve the neural networks and add more features in the future.
 
 ## 📦 Features
 
-- Many layers (input, activation, dense, conv2d, maxpooling2d, flatten) 🧠
+- Many layers (input, activation, dense, dropout, conv2d, maxpooling2d, flatten) 🧠
 - Many activation functions (sigmoid, tanh, relu, leaky relu, softmax, linear, elu, selu) 📈
 - Many loss functions (mean squared error, mean absolute error, categorical crossentropy, binary crossentropy, huber loss) 📉
 - Many optimizers (sgd, momentum, rmsprop, adam) 📊
 - Supports binary classification, multiclass classification and regression 📖
 - Save and load models 📁
 - Simple to use 📚
```

### Comparing `neuralnetlib-2.1.0/neuralnetlib/activations.py` & `neuralnetlib-2.2.0/neuralnetlib/activations.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.1.0/neuralnetlib/layers.py` & `neuralnetlib-2.2.0/neuralnetlib/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 
 import numpy as np
 
 from neuralnetlib.activations import ActivationFunction
-from neuralnetlib.utils import im2col, col2im
+from neuralnetlib.preprocessing import im2col, col2im
 
 
 class Layer:
     def __init__(self):
         self.input = None
         self.output = None
```

### Comparing `neuralnetlib-2.1.0/neuralnetlib/losses.py` & `neuralnetlib-2.2.0/neuralnetlib/losses.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.1.0/neuralnetlib/metrics.py` & `neuralnetlib-2.2.0/neuralnetlib/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from neuralnetlib.utils import apply_threshold
+from neuralnetlib.preprocessing import apply_threshold
 
 
 def accuracy_score(y_pred: np.ndarray, y_true: np.ndarray, threshold: float = 0.5) -> float:
     if y_pred.ndim == 1 or y_pred.shape[1] == 1:  # Binary classification
         y_pred_classes = apply_threshold(y_pred, threshold).ravel()
     else:  # Multiclass classification-regression
         y_pred_classes = np.argmax(y_pred, axis=1)
```

### Comparing `neuralnetlib-2.1.0/neuralnetlib/model.py` & `neuralnetlib-2.2.0/neuralnetlib/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import time
 
 import numpy as np
 
 from neuralnetlib.layers import Layer, Input, Activation, Dense, Flatten, Conv2D, Dropout
 from neuralnetlib.losses import LossFunction, CategoricalCrossentropy
-from neuralnetlib.metrics import accuracy_score
 from neuralnetlib.optimizers import Optimizer
 from neuralnetlib.utils import shuffle, progress_bar
+from neuralnetlib.metrics import accuracy_score
 
 
 class Model:
     def __init__(self):
         self.layers = []
         self.loss_function = None
         self.optimizer = None
@@ -24,14 +24,17 @@
         for i, layer in enumerate(self.layers):
             model_summary += f'Layer {i + 1}: {str(layer)}\n'
         model_summary += '-------------------------------------------------\n'
         model_summary += f'Loss function: {str(self.loss_function)}\n'
         model_summary += f'Optimizer: {str(self.optimizer)}\n'
         model_summary += '-------------------------------------------------\n'
         return model_summary
+    
+    def summary(self):
+        print(str(self))
 
     def add(self, layer: Layer):
         if self.layers and len(self.layers) != 0 and not isinstance(self.layers[-1], Input) and isinstance(layer,
                                                                                                            Dense):
             prev_layer = [l for l in self.layers if isinstance(l, (Input, Dense, Conv2D, Flatten))][-1]
             if isinstance(prev_layer, Flatten):
                 prev_layer = [l for l in self.layers if isinstance(l, (Dense, Conv2D))][-1]
@@ -39,15 +42,15 @@
                 raise ValueError(
                     f'Layer input size {layer.input_size} does not match previous layer output size {prev_layer.output_size}.')
         elif self.layers and isinstance(layer, Dropout):
             if isinstance(self.layers[-1], Dropout):
                 raise ValueError("Cannot add consecutive Dropout layers.")
         self.layers.append(layer)
 
-    def compile(self, loss_function: LossFunction, optimizer: Optimizer, verbose: bool = True):
+    def compile(self, loss_function: LossFunction, optimizer: Optimizer, verbose: bool = False):
         self.loss_function = loss_function
         self.optimizer = optimizer
         if verbose:
             print(str(self))
 
     def forward_pass(self, X: np.ndarray, training: bool = True) -> np.ndarray:
         for layer in self.layers:
```

### Comparing `neuralnetlib-2.1.0/neuralnetlib/optimizers.py` & `neuralnetlib-2.2.0/neuralnetlib/optimizers.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.1.0/neuralnetlib/utils.py` & `neuralnetlib-2.2.0/neuralnetlib/preprocessing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import sys
-import time
-
 import numpy as np
 
 
 def one_hot_encode(labels: np.ndarray, num_classes: int) -> np.ndarray:
     """One hot encoded labels are binary vectors representing categorical values,
     with exactly one high (or "hot" = 1) bit indicating the presence of a specific category
     and all other bits low (or "cold" = 0)."""
@@ -13,39 +10,19 @@
 
     labels = labels.astype(int)
     one_hot = np.zeros((labels.size, num_classes))
     one_hot[np.arange(labels.size), labels] = 1
     return one_hot
 
 
-def dict_with_ndarray_to_dict_with_list(d: dict) -> dict:
-    for k, v in d.items():
-        if isinstance(v, np.ndarray):
-            d[k] = v.tolist()
-    return d
-
-
-def dict_with_list_to_dict_with_ndarray(d: dict) -> dict:
-    for k, v in d.items():
-        if isinstance(v, list):
-            d[k] = np.array(v)
-    return d
-
-
 def apply_threshold(y_pred, threshold: float = 0.5):
     """Applies a threshold to the predictions. Typically used for binary classification."""
     return (y_pred > threshold).astype(int)
 
 
-def shuffle(x, y, random_state: int = None) -> tuple:
-    rng = np.random.default_rng(random_state if random_state is not None else int(time.time_ns()))
-    indices = rng.permutation(len(x))
-    return x[indices], y[indices]
-
-
 def im2col(input_data, filter_h, filter_w, stride=1, pad=0):
     """
     Transform 4 dimensional images to 2 dimensional array.
 
     Args:
         input_data (np.ndarray): 4 dimensional input images (The number of images, The number of channels, Height, Width)
         filter_h (int): height of filter
@@ -138,13 +115,54 @@
         for x in range(filter_w):
             x_max = x + stride_w * out_w
             image[:, :, y:y_max:stride_h, x:x_max:stride_w] += col[:, :, y, x, :, :]
 
     return image[:, :, pad_h:H + pad_h, pad_w:W + pad_w]
 
 
-def progress_bar(current: int, total: int, width: int = 30, message: str = "") -> None:
-    progress = current / total
-    bar = '=' * int(width * progress) + '-' * (width - int(width * progress))
-    percent = int(100 * progress)
-    sys.stdout.write(f'\r[{bar}] {percent}% {message}')
-    sys.stdout.flush()
+class StandardScaler:
+    def __init__(self):
+        self.mean_ = None
+        self.scale_ = None
+
+    def fit(self, X):
+        self.mean_ = np.mean(X, axis=0)
+        self.scale_ = np.std(X, axis=0)
+
+    def transform(self, X):
+        if self.mean_ is None or self.scale_ is None:
+            raise ValueError("StandardScaler has not been fitted yet.")
+        return (X - self.mean_) / self.scale_
+
+    def fit_transform(self, X):
+        self.fit(X)
+        return self.transform(X)
+
+    def inverse_transform(self, X):
+        if self.mean_ is None or self.scale_ is None:
+            raise ValueError("StandardScaler has not been fitted yet.")
+        return X * self.scale_ + self.mean_
+    
+    
+class MinMaxScaler:
+    def __init__(self, feature_range=(0, 1)):
+        self.feature_range = feature_range
+        self.min_ = None
+        self.scale_ = None
+
+    def fit(self, X):
+        self.min_ = np.min(X, axis=0)
+        self.scale_ = np.max(X, axis=0) - self.min_
+
+    def transform(self, X):
+        if self.min_ is None or self.scale_ is None:
+            raise ValueError("MinMaxScaler has not been fitted yet.")
+        return (X - self.min_) / self.scale_ * (self.feature_range[1] - self.feature_range[0]) + self.feature_range[0]
+
+    def fit_transform(self, X):
+        self.fit(X)
+        return self.transform(X)
+
+    def inverse_transform(self, X):
+        if self.min_ is None or self.scale_ is None:
+            raise ValueError("MinMaxScaler has not been fitted yet.")
+        return (X - self.feature_range[0]) / (self.feature_range[1] - self.feature_range[0]) * self.scale_ + self.min_
```

### Comparing `neuralnetlib-2.1.0/neuralnetlib.egg-info/PKG-INFO` & `neuralnetlib-2.2.0/neuralnetlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.1.0
+Version: 2.2.0
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -31,15 +31,15 @@
 
 Remember that this library is not optimized for performance, but for learning purposes (although I tried to make it as fast as possible).
 
 I intend to improve the neural networks and add more features in the future.
 
 ## 📦 Features
 
-- Many layers (input, activation, dense, conv2d, maxpooling2d, flatten) 🧠
+- Many layers (input, activation, dense, dropout, conv2d, maxpooling2d, flatten) 🧠
 - Many activation functions (sigmoid, tanh, relu, leaky relu, softmax, linear, elu, selu) 📈
 - Many loss functions (mean squared error, mean absolute error, categorical crossentropy, binary crossentropy, huber loss) 📉
 - Many optimizers (sgd, momentum, rmsprop, adam) 📊
 - Supports binary classification, multiclass classification and regression 📖
 - Save and load models 📁
 - Simple to use 📚
```

### Comparing `neuralnetlib-2.1.0/setup.py` & `neuralnetlib-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='neuralnetlib',
-    version='2.1.0',
+    version='2.2.0',
     author='Marc Pinet',
     description='A simple convolutional neural network library with only numpy as dependency',
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/marcpinet/handmade-neuralnetwork',
     packages=find_packages(),
     install_requires=[
```


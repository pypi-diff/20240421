# Comparing `tmp/neuralnetlib-1.0.1.tar.gz` & `tmp/neuralnetlib-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralnetlib-1.0.1.tar", last modified: Tue Nov 14 11:26:01 2023, max compression
+gzip compressed data, was "neuralnetlib-2.0.0.tar", last modified: Sat Apr 20 23:48:04 2024, max compression
```

## Comparing `neuralnetlib-1.0.1.tar` & `neuralnetlib-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:26:01.856284 neuralnetlib-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-11-14 11:25:52.000000 neuralnetlib-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2023-11-14 11:26:01.856284 neuralnetlib-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2023-11-14 11:25:52.000000 neuralnetlib-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:26:01.856284 neuralnetlib-1.0.1/neuralnetlib/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-11-14 11:25:52.000000 neuralnetlib-1.0.1/neuralnetlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2023-11-14 11:25:52.000000 neuralnetlib-1.0.1/neuralnetlib/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2023-11-14 11:25:52.000000 neuralnetlib-1.0.1/neuralnetlib/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2023-11-14 11:25:52.000000 neuralnetlib-1.0.1/neuralnetlib/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2023-11-14 11:25:52.000000 neuralnetlib-1.0.1/neuralnetlib/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6249 2023-11-14 11:25:52.000000 neuralnetlib-1.0.1/neuralnetlib/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2023-11-14 11:25:52.000000 neuralnetlib-1.0.1/neuralnetlib/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2023-11-14 11:25:52.000000 neuralnetlib-1.0.1/neuralnetlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:26:01.856284 neuralnetlib-1.0.1/neuralnetlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2023-11-14 11:26:01.000000 neuralnetlib-1.0.1/neuralnetlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      409 2023-11-14 11:26:01.000000 neuralnetlib-1.0.1/neuralnetlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 11:26:01.000000 neuralnetlib-1.0.1/neuralnetlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-14 11:26:01.000000 neuralnetlib-1.0.1/neuralnetlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-14 11:26:01.000000 neuralnetlib-1.0.1/neuralnetlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-11-14 11:26:01.856284 neuralnetlib-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2023-11-14 11:25:52.000000 neuralnetlib-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 23:48:04.238343 neuralnetlib-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-20 23:47:55.000000 neuralnetlib-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-20 23:48:04.238343 neuralnetlib-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-20 23:47:55.000000 neuralnetlib-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 23:48:04.238343 neuralnetlib-2.0.0/neuralnetlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-20 23:47:55.000000 neuralnetlib-2.0.0/neuralnetlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-20 23:47:55.000000 neuralnetlib-2.0.0/neuralnetlib/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-04-20 23:47:55.000000 neuralnetlib-2.0.0/neuralnetlib/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-20 23:47:55.000000 neuralnetlib-2.0.0/neuralnetlib/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-20 23:47:55.000000 neuralnetlib-2.0.0/neuralnetlib/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-04-20 23:47:55.000000 neuralnetlib-2.0.0/neuralnetlib/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-04-20 23:47:55.000000 neuralnetlib-2.0.0/neuralnetlib/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-20 23:47:55.000000 neuralnetlib-2.0.0/neuralnetlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 23:48:04.238343 neuralnetlib-2.0.0/neuralnetlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-20 23:48:04.000000 neuralnetlib-2.0.0/neuralnetlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-20 23:48:04.000000 neuralnetlib-2.0.0/neuralnetlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 23:48:04.000000 neuralnetlib-2.0.0/neuralnetlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 23:48:04.000000 neuralnetlib-2.0.0/neuralnetlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-20 23:48:04.000000 neuralnetlib-2.0.0/neuralnetlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-20 23:48:04.238343 neuralnetlib-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-20 23:47:55.000000 neuralnetlib-2.0.0/setup.py
```

### Comparing `neuralnetlib-1.0.1/LICENSE` & `neuralnetlib-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralnetlib-1.0.1/PKG-INFO` & `neuralnetlib-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 1.0.1
-Summary: A simple neural network library with only numpy as dependency
+Version: 2.0.0
+Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -15,28 +15,31 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Handmade NeuralNetwork lib
+# Neuralnetlib
 
 ## 📝 Description
 
-This is a handmade neural network library, made in python, **using numpy as the only dependency**.
+This is a handmade convolutional neural network library, made in python, **using numpy as the only dependency**.
 
 I made it to challenge myself and to learn more about neural networks, how they work in depth.
 
 The big part of this project was made in 4 hours and a half. The save and load features, and the binary classification support were added later.
 
+Remember that this library is not optimized for performance, but for learning purposes (although I tried to make it as fast as possible).
+
 I intend to improve the neural networks and add more features in the future.
 
 ## 📦 Features
 
+- Many layers (input, activation, dense, conv2d, maxpooling2d, flatten) 🧠
 - Many activation functions (sigmoid, tanh, relu, leaky relu, softmax, linear, elu, selu) 📈
 - Many loss functions (mean squared error, mean absolute error, categorical crossentropy, binary crossentropy, huber loss) 📉
 - Many optimizers (sgd, momentum, rmsprop, adam) 📊
 - Supports binary classification, multiclass classification and regression 📖
 - Save and load models 📁
 - Simple to use 📚
 
@@ -46,30 +49,35 @@
 
 ```bash
 pip install neuralnetlib
 ```
 
 ## 💡 How to use
 
-See [this file](examples/simple_mnist_example.py) for a simple example of how to use the library.
+See [this file](examples/classification-regression/simple_mnist_multiclass.py) for a simple example of how to use the library.
+For a more advanced example, see [this file](examples/cnn-classification/simple_cnn_classification_mnist.py).
+
 More examples in [this folder](examples).
 
 You are free to tweak the hyperparameters and the network architecture to see how it affects the results.
 
 I used the [MNIST dataset](https://en.wikipedia.org/wiki/MNIST_database) to test the library, but you can use any dataset you want.
 
 ## 📜 Output of the example file
 
+Here is an example of a model training using the library
+
 ![cli](resources/img/cli.png)
 
-Here is an example with Tkinter:
+Here is an example of a loaded model used with Tkinter:
 
 ![gui](resources/img/gui.gif)
 
 Here, I decided to print the first 10 predictions and their respective labels to see how the network is performing.
 
 ![plot](resources/img/plot.png)
 
+**You can __of course__ use the library for any dataset you want.**
 
 ## ✍️ Authors
 
 - Marc Pinet - *Initial work* - [marcpinet](https://github.com/marcpinet)
```

### Comparing `neuralnetlib-1.0.1/README.md` & `neuralnetlib-2.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-# Handmade NeuralNetwork lib
+# Neuralnetlib
 
 ## 📝 Description
 
-This is a handmade neural network library, made in python, **using numpy as the only dependency**.
+This is a handmade convolutional neural network library, made in python, **using numpy as the only dependency**.
 
 I made it to challenge myself and to learn more about neural networks, how they work in depth.
 
 The big part of this project was made in 4 hours and a half. The save and load features, and the binary classification support were added later.
 
+Remember that this library is not optimized for performance, but for learning purposes (although I tried to make it as fast as possible).
+
 I intend to improve the neural networks and add more features in the future.
 
 ## 📦 Features
 
+- Many layers (input, activation, dense, conv2d, maxpooling2d, flatten) 🧠
 - Many activation functions (sigmoid, tanh, relu, leaky relu, softmax, linear, elu, selu) 📈
 - Many loss functions (mean squared error, mean absolute error, categorical crossentropy, binary crossentropy, huber loss) 📉
 - Many optimizers (sgd, momentum, rmsprop, adam) 📊
 - Supports binary classification, multiclass classification and regression 📖
 - Save and load models 📁
 - Simple to use 📚
 
@@ -25,30 +28,35 @@
 
 ```bash
 pip install neuralnetlib
 ```
 
 ## 💡 How to use
 
-See [this file](examples/simple_mnist_example.py) for a simple example of how to use the library.
+See [this file](examples/classification-regression/simple_mnist_multiclass.py) for a simple example of how to use the library.
+For a more advanced example, see [this file](examples/cnn-classification/simple_cnn_classification_mnist.py).
+
 More examples in [this folder](examples).
 
 You are free to tweak the hyperparameters and the network architecture to see how it affects the results.
 
 I used the [MNIST dataset](https://en.wikipedia.org/wiki/MNIST_database) to test the library, but you can use any dataset you want.
 
 ## 📜 Output of the example file
 
+Here is an example of a model training using the library
+
 ![cli](resources/img/cli.png)
 
-Here is an example with Tkinter:
+Here is an example of a loaded model used with Tkinter:
 
 ![gui](resources/img/gui.gif)
 
 Here, I decided to print the first 10 predictions and their respective labels to see how the network is performing.
 
 ![plot](resources/img/plot.png)
 
+**You can __of course__ use the library for any dataset you want.**
 
 ## ✍️ Authors
 
-- Marc Pinet - *Initial work* - [marcpinet](https://github.com/marcpinet)
+- Marc Pinet - *Initial work* - [marcpinet](https://github.com/marcpinet)
```

### Comparing `neuralnetlib-1.0.1/neuralnetlib/activations.py` & `neuralnetlib-2.0.0/neuralnetlib/activations.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-1.0.1/neuralnetlib/losses.py` & `neuralnetlib-2.0.0/neuralnetlib/losses.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,44 +33,57 @@
     def __call__(self, y_true: np.ndarray, y_pred: np.ndarray) -> float:
         return np.mean(np.power(y_true - y_pred, 2))
 
     def derivative(self, y_true: np.ndarray, y_pred: np.ndarray) -> np.ndarray:
         y_true_reshaped = y_true.reshape(-1, 1)
         return 2 * (y_pred - y_true_reshaped) / y_true.shape[0]
 
+    def __str__(self):
+        return "MeanSquaredError"
+
+
 class BinaryCrossentropy(LossFunction):
     def __call__(self, y_true: np.ndarray, y_pred: np.ndarray) -> float:
         y_pred = np.clip(y_pred, LossFunction.EPSILON, 1 - LossFunction.EPSILON)
         return -np.mean(y_true * np.log(y_pred) + (1 - y_true) * np.log(1 - y_pred))
 
     def derivative(self, y_true: np.ndarray, y_pred: np.ndarray) -> np.ndarray:
         y_pred = np.clip(y_pred, LossFunction.EPSILON, 1 - LossFunction.EPSILON)
         return y_pred - y_true
 
+    def __str__(self):
+        return "BinaryCrossentropy"
+
 
 class CategoricalCrossentropy(LossFunction):
     def __call__(self, y_true: np.ndarray, y_pred: np.ndarray) -> float:
         y_pred = np.clip(y_pred, LossFunction.EPSILON, 1 - LossFunction.EPSILON)
         return -np.sum(y_true * np.log(y_pred)) / y_true.shape[0]
 
     def derivative(self, y_true: np.ndarray, y_pred: np.ndarray) -> np.ndarray:
         try:
             y_pred = np.clip(y_pred, LossFunction.EPSILON, 1 - LossFunction.EPSILON)
             return (y_pred - y_true) / y_true.shape[0]
         except Exception as e:
             print(e, "Make sure to one-hot encode your labels.", sep="\n")
 
+    def __str__(self):
+        return "CategoricalCrossentropy"
+
 
 class MeanAbsoluteError(LossFunction):
     def __call__(self, y_true: np.ndarray, y_pred: np.ndarray) -> float:
         return np.mean(np.abs(y_true - y_pred))
 
     def derivative(self, y_true: np.ndarray, y_pred: np.ndarray) -> np.ndarray:
         return np.where(y_pred > y_true, 1, -1)
 
+    def __str__(self):
+        return "MeanAbsoluteError"
+
 
 class HuberLoss(LossFunction):
     def __init__(self, delta: float = 1.0):
         super().__init__()
         self.delta = delta
 
     def __call__(self, y_true: np.ndarray, y_pred: np.ndarray) -> float:
@@ -80,9 +93,12 @@
         linear_loss = self.delta * (np.abs(error) - 0.5 * self.delta)
         return np.mean(np.where(is_small_error, squared_loss, linear_loss))
 
     def derivative(self, y_true: np.ndarray, y_pred: np.ndarray) -> np.ndarray:
         error = y_true - y_pred
         return np.where(np.abs(error) <= self.delta, error, self.delta * np.sign(error))
 
+    def __str__(self):
+        return f"HuberLoss(delta={self.delta})"
+
     def get_config(self) -> dict:
         return {"name": self.__class__.__name__, "delta": self.delta}
```

### Comparing `neuralnetlib-1.0.1/neuralnetlib/metrics.py` & `neuralnetlib-2.0.0/neuralnetlib/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 from neuralnetlib.utils import apply_threshold
 
 
 def accuracy_score(y_pred: np.ndarray, y_true: np.ndarray, threshold: float = 0.5) -> float:
     if y_pred.ndim == 1 or y_pred.shape[1] == 1:  # Binary classification
         y_pred_classes = apply_threshold(y_pred, threshold).ravel()
-    else:  # Multiclass classification
+    else:  # Multiclass classification-regression
         y_pred_classes = np.argmax(y_pred, axis=1)
 
     if y_true.ndim == 1 or y_true.shape[1] == 1:  # If y_true is not one-hot encoded
         y_true_classes = y_true.ravel()
     else:
         y_true_classes = np.argmax(y_true, axis=1)
 
     return np.mean(y_pred_classes == y_true_classes)
 
+
 def f1_score(y_pred: np.ndarray, y_true: np.ndarray, threshold: float = 0.5) -> float:
     precision = precision_score(y_pred, y_true, threshold)
     recall = recall_score(y_pred, y_true, threshold)
     return 2 * (precision * recall) / (precision + recall) if (precision + recall) > 0 else 0
 
 
 def recall_score(y_pred: np.ndarray, y_true: np.ndarray, threshold: float = 0.5) -> float:
@@ -53,15 +54,15 @@
 
     return np.mean(precision_scores)
 
 
 def confusion_matrix(y_pred: np.ndarray, y_true: np.ndarray, threshold: float = 0.5) -> np.ndarray:
     if y_pred.ndim == 1 or y_pred.shape[1] == 1:  # Binary classification
         y_pred_classes = apply_threshold(y_pred, threshold).ravel()
-    else:  # Multiclass classification
+    else:  # Multiclass classification-regression
         y_pred_classes = np.argmax(y_pred, axis=1)
 
     if y_true.ndim == 1 or y_true.shape[1] == 1:  # If y_true is not one-hot encoded
         y_true_classes = y_true.ravel()
     else:
         y_true_classes = np.argmax(y_true, axis=1)
```

### Comparing `neuralnetlib-1.0.1/neuralnetlib/model.py` & `neuralnetlib-2.0.0/neuralnetlib/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import json
 import time
 
 import numpy as np
 
-from neuralnetlib.layers import Layer, Activation, Dense
+from neuralnetlib.layers import Layer, Input, Activation, Dense, Flatten, Conv2D
 from neuralnetlib.losses import LossFunction, CategoricalCrossentropy
+from neuralnetlib.metrics import accuracy_score
 from neuralnetlib.optimizers import Optimizer
-from neuralnetlib.utils import shuffle
+from neuralnetlib.utils import shuffle, progress_bar
 
 
 class Model:
     def __init__(self):
         self.layers = []
         self.loss_function = None
         self.optimizer = None
@@ -25,27 +26,23 @@
         model_summary += '-------------------------------------------------\n'
         model_summary += f'Loss function: {str(self.loss_function)}\n'
         model_summary += f'Optimizer: {str(self.optimizer)}\n'
         model_summary += '-------------------------------------------------\n'
         return model_summary
 
     def add(self, layer: Layer):
-        if self.layers and isinstance(layer, Dense):
-            prev_layer = [l for l in self.layers if isinstance(l, Dense)][-1]
+        if self.layers and len(self.layers) != 0 and not isinstance(self.layers[-1], Input) and isinstance(layer, Dense):
+            prev_layer = [l for l in self.layers if isinstance(l, (Input, Dense, Conv2D, Flatten))][-1]
+            if isinstance(prev_layer, Flatten):
+                prev_layer = [l for l in self.layers if isinstance(l, (Dense, Conv2D))][-1]
             if hasattr(prev_layer, 'output_size') and prev_layer.output_size != layer.input_size:
                 raise ValueError(
                     f'Layer input size {layer.input_size} does not match previous layer output size {prev_layer.output_size}.')
         self.layers.append(layer)
 
-    def __check_layer_compatability(self, layer: Dense) -> bool:
-        if len(self.layers) == 0:
-            return True
-        else:
-            return layer.input_size == [l for l in self.layers if isinstance(l, Dense)][-1].output_size
-
     def compile(self, loss_function: LossFunction, optimizer: Optimizer, verbose: bool = True):
         self.loss_function = loss_function
         self.optimizer = optimizer
         if verbose:
             print(str(self))
 
     def forward_pass(self, X: np.ndarray) -> np.ndarray:
@@ -68,20 +65,26 @@
 
     def train_on_batch(self, x_batch: np.ndarray, y_batch: np.ndarray) -> float:
         self.y_true = y_batch
         self.predictions = self.forward_pass(x_batch)
         predictions = self.predictions.copy()
         loss = self.loss_function(y_batch, predictions)
         error = self.loss_function.derivative(y_batch, predictions)
+
+        if error.ndim == 1:
+            error = error[:, None]
+
         self.backward_pass(error)
         return loss
 
     def train(self, x_train: np.ndarray, y_train: np.ndarray, epochs: int, batch_size: int = None,
-              verbose: bool = True, metrics: list = None, random_state: int = None):
+              verbose: bool = True, metrics: list = None, random_state: int = None, validation_data: tuple = None):
         for i in range(epochs):
+            start_time = time.time()
+
             # Shuffling the data to avoid overfitting
             x_train_shuffled, y_train_shuffled = shuffle(x_train, y_train, random_state=random_state)
 
             error = 0
             predictions_list = []
             y_true_list = []
 
@@ -94,33 +97,47 @@
                     # Reshape if it's a regression (single output neuron)
                     if y_batch.ndim == 1:
                         y_batch = y_batch.reshape(-1, 1)
                     error += self.train_on_batch(x_batch, y_batch)
                     predictions_list.append(self.predictions)
                     y_true_list.append(y_batch)
 
+                    if verbose:
+                        metrics_str = ''
+                        if metrics is not None:
+                            for metric in metrics:
+                                metric_value = metric(np.vstack(predictions_list), np.vstack(y_true_list))
+                                metrics_str += f'{metric.__name__}: {metric_value:.4f} - '
+                        progress_bar(j / batch_size + 1, num_batches,
+                                     message=f'Epoch {i + 1}/{epochs} - loss: {error / (j / batch_size + 1):.4f} - {metrics_str[:-3]} - {time.time() - start_time:.2f}s')
+
                 error /= num_batches
             else:
                 error = self.train_on_batch(x_train, y_train)
                 predictions_list.append(self.predictions)
                 y_true_list.append(y_train)
 
-            # Concatenate all predictions and true labels
-            all_predictions = np.vstack(predictions_list)
-            all_y_true = np.vstack(y_true_list)
+                if verbose:
+                    metrics_str = ''
+                    if metrics is not None:
+                        for metric in metrics:
+                            metric_value = metric(np.vstack(predictions_list), np.vstack(y_true_list))
+                            metrics_str += f'{metric.__name__}: {metric_value:.4f} - '
+                    progress_bar(1, 1,
+                                 message=f'Epoch {i + 1}/{epochs} - loss: {error:.4f} - {metrics_str[:-3]} - {time.time() - start_time:.2f}s')
+
+            if validation_data is not None:
+                x_test, y_test = validation_data
+                val_predictions = self.predict(x_test)
+                val_accuracy = accuracy_score(val_predictions, y_test)
+                if verbose:
+                    print(f' - val_accuracy: {val_accuracy:.4f}', end='')
 
             if verbose:
-                if metrics is not None:
-                    metrics_str = ''
-                    for metric in metrics:
-                        metric_value = metric(all_predictions, all_y_true)
-                        metrics_str += f'{metric.__name__}: {metric_value} - '
-                    print(f'Epoch {i + 1}/{epochs} - loss: {error} - {metrics_str[:-3]}')
-                else:
-                    print(f'Epoch {i + 1}/{epochs} - loss: {error}')
+                print()
 
     def evaluate(self, x_test: np.ndarray, y_test: np.ndarray) -> float:
         predictions = self.forward_pass(x_test)
         loss = self.loss_function(y_test, predictions)
         return loss
 
     def predict(self, X: np.ndarray) -> np.ndarray:
```

### Comparing `neuralnetlib-1.0.1/neuralnetlib/optimizers.py` & `neuralnetlib-2.0.0/neuralnetlib/optimizers.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,17 @@
                bias_grad: np.ndarray):
         weights -= self.learning_rate * weights_grad
         bias -= self.learning_rate * bias_grad
 
     def get_config(self) -> dict:
         return {"name": self.__class__.__name__, "learning_rate": self.learning_rate}
 
+    def __str__(self):
+        return f"{self.__class__.__name__}(learning_rate={self.learning_rate})"
+
     @staticmethod
     def from_config(config: dict):
         return SGD(config['learning_rate'])
 
 
 class Momentum(Optimizer):
     def __init__(self, learning_rate: float = 0.01, momentum: float = 0.9):
@@ -62,14 +65,17 @@
         self.velocity_b = self.momentum * self.velocity_b - self.learning_rate * bias_grad
         bias += self.velocity_b
 
     def get_config(self) -> dict:
         return {"name": self.__class__.__name__, "learning_rate": self.learning_rate, "momentum": self.momentum,
                 "velocity": self.velocity}
 
+    def __str__(self):
+        return f"{self.__class__.__name__}(learning_rate={self.learning_rate}, momentum={self.momentum})"
+
     @staticmethod
     def from_config(config: dict):
         return Momentum(config['learning_rate'], config['momentum'])
 
 
 class RMSprop(Optimizer):
     def __init__(self, learning_rate: float = 0.01, rho: float = 0.9, epsilon: float = 1e-8):
@@ -96,14 +102,17 @@
         return {"name": self.__class__.__name__, "learning_rate": self.learning_rate, "rho": self.rho,
                 "epsilon": self.epsilon, "sq_grads": self.sq_grads}
 
     @staticmethod
     def from_config(config: dict):
         return RMSprop(config['learning_rate'], config['rho'], config['epsilon'])
 
+    def __str__(self):
+        return f"{self.__class__.__name__}(learning_rate={self.learning_rate}, rho={self.rho}, epsilon={self.epsilon})"
+
 
 class Adam(Optimizer):
     def __init__(self, learning_rate=0.001, beta_1=0.9, beta_2=0.999, epsilon=1e-8):
         super().__init__(learning_rate)
         self.beta_1 = beta_1
         self.beta_2 = beta_2
         self.epsilon = epsilon
@@ -151,7 +160,10 @@
         adam = Adam(config['learning_rate'], config['beta_1'], config['beta_2'], config['epsilon'])
         adam.t = config['t']
         adam.m_w = dict_with_list_to_dict_with_ndarray(config['m_w'])
         adam.v_w = dict_with_list_to_dict_with_ndarray(config['v_w'])
         adam.m_b = dict_with_list_to_dict_with_ndarray(config['m_b'])
         adam.v_b = dict_with_list_to_dict_with_ndarray(config['v_b'])
         return adam
+
+    def __str__(self):
+        return f"{self.__class__.__name__}(learning_rate={self.learning_rate}, beta_1={self.beta_1}, beta_2={self.beta_2}, epsilon={self.epsilon})"
```

### Comparing `neuralnetlib-1.0.1/neuralnetlib.egg-info/PKG-INFO` & `neuralnetlib-2.0.0/neuralnetlib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 1.0.1
-Summary: A simple neural network library with only numpy as dependency
+Version: 2.0.0
+Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -15,28 +15,31 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Handmade NeuralNetwork lib
+# Neuralnetlib
 
 ## 📝 Description
 
-This is a handmade neural network library, made in python, **using numpy as the only dependency**.
+This is a handmade convolutional neural network library, made in python, **using numpy as the only dependency**.
 
 I made it to challenge myself and to learn more about neural networks, how they work in depth.
 
 The big part of this project was made in 4 hours and a half. The save and load features, and the binary classification support were added later.
 
+Remember that this library is not optimized for performance, but for learning purposes (although I tried to make it as fast as possible).
+
 I intend to improve the neural networks and add more features in the future.
 
 ## 📦 Features
 
+- Many layers (input, activation, dense, conv2d, maxpooling2d, flatten) 🧠
 - Many activation functions (sigmoid, tanh, relu, leaky relu, softmax, linear, elu, selu) 📈
 - Many loss functions (mean squared error, mean absolute error, categorical crossentropy, binary crossentropy, huber loss) 📉
 - Many optimizers (sgd, momentum, rmsprop, adam) 📊
 - Supports binary classification, multiclass classification and regression 📖
 - Save and load models 📁
 - Simple to use 📚
 
@@ -46,30 +49,35 @@
 
 ```bash
 pip install neuralnetlib
 ```
 
 ## 💡 How to use
 
-See [this file](examples/simple_mnist_example.py) for a simple example of how to use the library.
+See [this file](examples/classification-regression/simple_mnist_multiclass.py) for a simple example of how to use the library.
+For a more advanced example, see [this file](examples/cnn-classification/simple_cnn_classification_mnist.py).
+
 More examples in [this folder](examples).
 
 You are free to tweak the hyperparameters and the network architecture to see how it affects the results.
 
 I used the [MNIST dataset](https://en.wikipedia.org/wiki/MNIST_database) to test the library, but you can use any dataset you want.
 
 ## 📜 Output of the example file
 
+Here is an example of a model training using the library
+
 ![cli](resources/img/cli.png)
 
-Here is an example with Tkinter:
+Here is an example of a loaded model used with Tkinter:
 
 ![gui](resources/img/gui.gif)
 
 Here, I decided to print the first 10 predictions and their respective labels to see how the network is performing.
 
 ![plot](resources/img/plot.png)
 
+**You can __of course__ use the library for any dataset you want.**
 
 ## ✍️ Authors
 
 - Marc Pinet - *Initial work* - [marcpinet](https://github.com/marcpinet)
```

### Comparing `neuralnetlib-1.0.1/setup.py` & `neuralnetlib-2.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='neuralnetlib',
-    version='1.0.1',
+    version='2.0.0',
     author='Marc Pinet',
-    description='A simple neural network library with only numpy as dependency',
+    description='A simple convolutional neural network library with only numpy as dependency',
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/marcpinet/handmade-neuralnetwork',
     packages=find_packages(),
     install_requires=[
         'numpy',
     ],
```


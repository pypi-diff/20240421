# Comparing `tmp/tensorsequence-0.1.0.tar.gz` & `tmp/tensorsequence-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorsequence-0.1.0.tar", last modified: Fri Apr 19 23:06:42 2024, max compression
+gzip compressed data, was "tensorsequence-0.2.0.tar", last modified: Sun Apr 21 17:41:25 2024, max compression
```

## Comparing `tensorsequence-0.1.0.tar` & `tensorsequence-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:06:42.184057 tensorsequence-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-19 23:06:42.184057 tensorsequence-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-19 23:06:38.000000 tensorsequence-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 23:06:42.184057 tensorsequence-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-19 23:06:38.000000 tensorsequence-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:06:42.180057 tensorsequence-0.1.0/tensorsequence/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 23:06:38.000000 tensorsequence-0.1.0/tensorsequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-19 23:06:38.000000 tensorsequence-0.1.0/tensorsequence/tensorsequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:06:42.184057 tensorsequence-0.1.0/tensorsequence/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 23:06:38.000000 tensorsequence-0.1.0/tensorsequence/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-19 23:06:38.000000 tensorsequence-0.1.0/tensorsequence/tests/test_tensorsequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:06:42.184057 tensorsequence-0.1.0/tensorsequence.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-19 23:06:42.000000 tensorsequence-0.1.0/tensorsequence.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-19 23:06:42.000000 tensorsequence-0.1.0/tensorsequence.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 23:06:42.000000 tensorsequence-0.1.0/tensorsequence.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 23:06:42.000000 tensorsequence-0.1.0/tensorsequence.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 23:06:42.000000 tensorsequence-0.1.0/tensorsequence.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:41:25.688464 tensorsequence-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-21 17:41:25.688464 tensorsequence-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-21 17:41:22.000000 tensorsequence-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 17:41:25.688464 tensorsequence-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-21 17:41:22.000000 tensorsequence-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:41:25.688464 tensorsequence-0.2.0/tensorsequence/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-21 17:41:22.000000 tensorsequence-0.2.0/tensorsequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-21 17:41:22.000000 tensorsequence-0.2.0/tensorsequence/tensorsequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:41:25.688464 tensorsequence-0.2.0/tensorsequence/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 17:41:22.000000 tensorsequence-0.2.0/tensorsequence/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-21 17:41:22.000000 tensorsequence-0.2.0/tensorsequence/tests/test_tensorsequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:41:25.688464 tensorsequence-0.2.0/tensorsequence.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-21 17:41:25.000000 tensorsequence-0.2.0/tensorsequence.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-21 17:41:25.000000 tensorsequence-0.2.0/tensorsequence.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 17:41:25.000000 tensorsequence-0.2.0/tensorsequence.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 17:41:25.000000 tensorsequence-0.2.0/tensorsequence.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 17:41:25.000000 tensorsequence-0.2.0/tensorsequence.egg-info/top_level.txt
```

### Comparing `tensorsequence-0.1.0/PKG-INFO` & `tensorsequence-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorsequence
-Version: 0.1.0
+Version: 0.2.0
 Summary: manipulate sequences of tensors
 Home-page: https://github.com/theAdamColton/tensorsequence
 Author: Adam Colton
 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.0.1
 
 # tensorsequence
@@ -49,15 +49,15 @@
 They all have matching leading dimensions for batch_size and sequence length. 
 TensorSequence is a container for these related multi-dimensional sequences. 
 TensorSequence makes this kind of manipulation very easy and ergonomic.
 
 ```python
 from tensorsequence import TensorSequence
 inputs = TensorSequence(input_ids, input_embeds, key_pad_mask, is_whitespace_mask, sequence_dim=1)
-truncated_inputs = inputs[:, :length]
+truncated_inputs = inputs.iloc[:, :length]
 ```
 
 
 # Features
 
 Stack related TensorSets to create larger batches
 
@@ -68,9 +68,9 @@
                 torch.randn(sequence_length, 1024),
                 sequence_dim=0
             )
 sequence_2 = TensorSet(torch.randn(sequence_length, 512), torch.randn(sequence_length, 1024), sequence_dim=0)
 batch = TensorSet.stack(sequence_1, sequence_2)
 
 print(batch.sequence_length) # Prints 20
-print(batch.leading_shape[0]) # Prints 2
+print(batch.leading_shape[0]) # This is the batch size, Prints 2
 ```
```

### Comparing `tensorsequence-0.1.0/README.md` & `tensorsequence-0.2.0/tensorsequence.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: tensorsequence
+Version: 0.2.0
+Summary: manipulate sequences of tensors
+Home-page: https://github.com/theAdamColton/tensorsequence
+Author: Adam Colton
+Description-Content-Type: text/markdown
+Requires-Dist: torch>=2.0.1
+
 # tensorsequence
 
 tensorsequence is a pytorch library that lets you perform operations on related sequences using a unified `TensorSequence` object.
 
 It aims to reduce the complexity of using multiple related sequences. Sequences like these are very commonly used as inputs to a transformer model:
 ```python
 import torch
@@ -40,15 +49,15 @@
 They all have matching leading dimensions for batch_size and sequence length. 
 TensorSequence is a container for these related multi-dimensional sequences. 
 TensorSequence makes this kind of manipulation very easy and ergonomic.
 
 ```python
 from tensorsequence import TensorSequence
 inputs = TensorSequence(input_ids, input_embeds, key_pad_mask, is_whitespace_mask, sequence_dim=1)
-truncated_inputs = inputs[:, :length]
+truncated_inputs = inputs.iloc[:, :length]
 ```
 
 
 # Features
 
 Stack related TensorSets to create larger batches
 
@@ -59,9 +68,9 @@
                 torch.randn(sequence_length, 1024),
                 sequence_dim=0
             )
 sequence_2 = TensorSet(torch.randn(sequence_length, 512), torch.randn(sequence_length, 1024), sequence_dim=0)
 batch = TensorSet.stack(sequence_1, sequence_2)
 
 print(batch.sequence_length) # Prints 20
-print(batch.leading_shape[0]) # Prints 2
+print(batch.leading_shape[0]) # This is the batch size, Prints 2
 ```
```

### Comparing `tensorsequence-0.1.0/tensorsequence/tensorsequence.py` & `tensorsequence-0.2.0/tensorsequence/tensorsequence.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,25 @@
         for i, (s, c_s) in enumerate(zip(shape, c_shape)):
             if s != c_s:
                 raise ValueError(
                     f"column number {c_i} has incompatible shape at dimension {i}, {s} != {c_s}"
                 )
 
 
+class _IlocIndexer:
+    def __init__(self, tensorsequence):
+        self.tensorsequence = tensorsequence
+
+    def __getitem__(self, key):
+        return TensorSequence(
+            list(c[key] for c in self.tensorsequence.columns),
+            {k: c[key] for k, c in self.tensorsequence.named_columns.items()},
+        )
+
+
 class TensorSequence:
     """
     A small wrapper allowing manipulation of a set of columns,
     each column with the same sequence length (rows)
 
     """
 
@@ -98,19 +109,32 @@
             return tuple()
         return self.all_columns[0].shape[: self.sequence_dim + 1]
 
     @property
     def num_columns(self):
         return len(self.all_columns)
 
+    @property
+    def iloc(self):
+        """
+        Index into the rows of all of the columns of this tensorset.
+        """
+        return _IlocIndexer(self)
+
     def __getitem__(self, key):
-        return TensorSequence(
-            list(c[key] for c in self.columns),
-            {k: c[key] for k, c in self.named_columns.items()},
-        )
+        """
+        Access the columns of this tensorset, using either integer keys (to access self.columns)
+            or string keys (to access self.named_columns)
+        """
+        if isinstance(key, str):
+            return self.named_columns[key]
+        elif isinstance(key, int):
+            return self.columns[key]
+        else:
+            raise ValueError(key)
 
     @staticmethod
     def _run_func(tensorsequences, func, axis=None, new_sequence_dim=None):
         """
         make a new tensorsequence by running func across each columns of all tensorsequences
         """
         validate_tensor_sets_broadcastable(tensorsequences)
```

### Comparing `tensorsequence-0.1.0/tensorsequence.egg-info/PKG-INFO` & `tensorsequence-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: tensorsequence
-Version: 0.1.0
-Summary: manipulate sequences of tensors
-Home-page: https://github.com/theAdamColton/tensorsequence
-Author: Adam Colton
-Description-Content-Type: text/markdown
-Requires-Dist: torch>=2.0.1
-
 # tensorsequence
 
 tensorsequence is a pytorch library that lets you perform operations on related sequences using a unified `TensorSequence` object.
 
 It aims to reduce the complexity of using multiple related sequences. Sequences like these are very commonly used as inputs to a transformer model:
 ```python
 import torch
@@ -49,15 +40,15 @@
 They all have matching leading dimensions for batch_size and sequence length. 
 TensorSequence is a container for these related multi-dimensional sequences. 
 TensorSequence makes this kind of manipulation very easy and ergonomic.
 
 ```python
 from tensorsequence import TensorSequence
 inputs = TensorSequence(input_ids, input_embeds, key_pad_mask, is_whitespace_mask, sequence_dim=1)
-truncated_inputs = inputs[:, :length]
+truncated_inputs = inputs.iloc[:, :length]
 ```
 
 
 # Features
 
 Stack related TensorSets to create larger batches
 
@@ -68,9 +59,9 @@
                 torch.randn(sequence_length, 1024),
                 sequence_dim=0
             )
 sequence_2 = TensorSet(torch.randn(sequence_length, 512), torch.randn(sequence_length, 1024), sequence_dim=0)
 batch = TensorSet.stack(sequence_1, sequence_2)
 
 print(batch.sequence_length) # Prints 20
-print(batch.leading_shape[0]) # Prints 2
+print(batch.leading_shape[0]) # This is the batch size, Prints 2
 ```
```


# Comparing `tmp/bitmat_tl-0.3.6.tar.gz` & `tmp/bitmat_tl-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmat_tl-0.3.6.tar", last modified: Tue Apr 16 14:59:21 2024, max compression
+gzip compressed data, was "bitmat_tl-0.3.7.tar", last modified: Sun Apr 21 13:45:59 2024, max compression
```

## Comparing `bitmat_tl-0.3.6.tar` & `bitmat_tl-0.3.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:59:21.882697 bitmat_tl-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-16 14:59:21.882697 bitmat_tl-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:59:21.874697 bitmat_tl-0.3.6/bitmat/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/bitlinear.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:59:21.878697 bitmat_tl-0.3.6/bitmat/triton_kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/triton_kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/triton_kernels/bitmat_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/triton_kernels/rmsnorm_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/triton_kernels/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:59:21.878697 bitmat_tl-0.3.6/bitmat/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/utils/bitmat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/utils/convert_hf_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/utils/custom_autotune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:59:21.878697 bitmat_tl-0.3.6/bitmat/utils/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/utils/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/utils/modeling/automodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:59:21.878697 bitmat_tl-0.3.6/bitmat/utils/modeling/model_hijacks/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/utils/modeling/model_hijacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61145 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/utils/modeling/model_hijacks/gemma_1_58b.py
--rw-r--r--   0 runner    (1001) docker     (127)    73363 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/utils/modeling/model_hijacks/llama_1_58b.py
--rw-r--r--   0 runner    (1001) docker     (127)    64382 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/utils/modeling/model_hijacks/mistral_1_58b.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/utils/pack_model_before_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/utils/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 14:59:13.000000 bitmat_tl-0.3.6/bitmat/utils/rmsnorm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:59:21.882697 bitmat_tl-0.3.6/bitmat_tl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-16 14:59:21.000000 bitmat_tl-0.3.6/bitmat_tl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-16 14:59:21.000000 bitmat_tl-0.3.6/bitmat_tl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:59:21.000000 bitmat_tl-0.3.6/bitmat_tl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 14:59:21.000000 bitmat_tl-0.3.6/bitmat_tl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 14:59:21.000000 bitmat_tl-0.3.6/bitmat_tl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:59:21.882697 bitmat_tl-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-16 14:59:21.000000 bitmat_tl-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:59.905841 bitmat_tl-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-21 13:45:59.905841 bitmat_tl-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:59.901841 bitmat_tl-0.3.7/bitmat/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/bitlinear.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:59.901841 bitmat_tl-0.3.7/bitmat/triton_kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/triton_kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/triton_kernels/bitmat_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/triton_kernels/rmsnorm_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/triton_kernels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:59.905841 bitmat_tl-0.3.7/bitmat/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/utils/bitmat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/utils/convert_hf_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/utils/custom_autotune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:59.905841 bitmat_tl-0.3.7/bitmat/utils/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/utils/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/utils/modeling/automodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:59.905841 bitmat_tl-0.3.7/bitmat/utils/modeling/model_hijacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/utils/modeling/model_hijacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61145 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/utils/modeling/model_hijacks/gemma_1_58b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73363 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/utils/modeling/model_hijacks/llama_1_58b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64382 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/utils/modeling/model_hijacks/mistral_1_58b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/utils/pack_model_before_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/utils/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-21 13:45:51.000000 bitmat_tl-0.3.7/bitmat/utils/rmsnorm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:59.905841 bitmat_tl-0.3.7/bitmat_tl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-21 13:45:59.000000 bitmat_tl-0.3.7/bitmat_tl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-21 13:45:59.000000 bitmat_tl-0.3.7/bitmat_tl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:45:59.000000 bitmat_tl-0.3.7/bitmat_tl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 13:45:59.000000 bitmat_tl-0.3.7/bitmat_tl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 13:45:59.000000 bitmat_tl-0.3.7/bitmat_tl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 13:45:59.905841 bitmat_tl-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-21 13:45:59.000000 bitmat_tl-0.3.7/setup.py
```

### Comparing `bitmat_tl-0.3.6/LICENSE` & `bitmat_tl-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.6/PKG-INFO` & `bitmat_tl-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.3.6
+Version: 0.3.7
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bitmat_tl-0.3.6/README.md` & `bitmat_tl-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.6/bitmat/__init__.py` & `bitmat_tl-0.3.7/bitmat/__init__.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.6/bitmat/bitlinear.py` & `bitmat_tl-0.3.7/bitmat/bitlinear.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self.dtype = dtype
         self.register_buffer('weight', torch.zeros((out_features, in_features), dtype=torch.int8))
         self.scale_w = torch.nn.Parameter(torch.Tensor(1))
         if bias:
             self.bias = torch.nn.Parameter(torch.Tensor(out_features))
         else:
             self.register_parameter('bias', None)
-        self.norm = RMSLayerNorm(out_features, eps) # added this in favor of models like gemma that needs hp normalization
+        self.norm = RMSLayerNorm(in_features, eps)
         self.keep_rms_in_32b = keep_rms_in_32b
         self._post_init()
 
 
     """
     def a .to() to keep eps precision
     """
```

### Comparing `bitmat_tl-0.3.6/bitmat/triton_kernels/bitmat_kernel.py` & `bitmat_tl-0.3.7/bitmat/triton_kernels/bitmat_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.6/bitmat/triton_kernels/rmsnorm_kernel.py` & `bitmat_tl-0.3.7/bitmat/triton_kernels/rmsnorm_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.6/bitmat/triton_kernels/utils.py` & `bitmat_tl-0.3.7/bitmat/triton_kernels/utils.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.6/bitmat/utils/bitmat.py` & `bitmat_tl-0.3.7/bitmat/utils/bitmat.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.6/bitmat/utils/convert_hf_model.py` & `bitmat_tl-0.3.7/bitmat/utils/convert_hf_model.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.6/bitmat/utils/custom_autotune.py` & `bitmat_tl-0.3.7/bitmat/utils/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.6/bitmat/utils/modeling/automodel.py` & `bitmat_tl-0.3.7/bitmat/utils/modeling/automodel.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.6/bitmat/utils/modeling/model_hijacks/gemma_1_58b.py` & `bitmat_tl-0.3.7/bitmat/utils/modeling/model_hijacks/gemma_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.6/bitmat/utils/modeling/model_hijacks/llama_1_58b.py` & `bitmat_tl-0.3.7/bitmat/utils/modeling/model_hijacks/llama_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.6/bitmat/utils/modeling/model_hijacks/mistral_1_58b.py` & `bitmat_tl-0.3.7/bitmat/utils/modeling/model_hijacks/mistral_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.6/bitmat/utils/packing.py` & `bitmat_tl-0.3.7/bitmat/utils/packing.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.6/bitmat_tl.egg-info/PKG-INFO` & `bitmat_tl-0.3.7/bitmat_tl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.3.6
+Version: 0.3.7
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bitmat_tl-0.3.6/bitmat_tl.egg-info/SOURCES.txt` & `bitmat_tl-0.3.7/bitmat_tl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.6/setup.py` & `bitmat_tl-0.3.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bitmat-tl',
-    version='0.3.6',
+    version='0.3.7',
     author='Marco Lironi',
     author_email='marcolironi@astramind.ai',
     description='An efficent implementation for the paper: "The Era of 1-bit LLMs"',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/astramind-ai/BitMat/tree/main',
     packages=find_packages(),
```


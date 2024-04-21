# Comparing `tmp/BS-RoFormer-0.4.0.tar.gz` & `tmp/bs_roformer-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BS-RoFormer-0.4.0.tar", last modified: Tue Dec 12 16:31:40 2023, max compression
+gzip compressed data, was "bs_roformer-0.4.1.tar", last modified: Sun Apr 21 16:44:22 2024, max compression
```

## Comparing `BS-RoFormer-0.4.0.tar` & `bs_roformer-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 16:31:40.734708 BS-RoFormer-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 16:31:40.734708 BS-RoFormer-0.4.0/BS_RoFormer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2023-12-12 16:31:40.000000 BS-RoFormer-0.4.0/BS_RoFormer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      306 2023-12-12 16:31:40.000000 BS-RoFormer-0.4.0/BS_RoFormer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 16:31:40.000000 BS-RoFormer-0.4.0/BS_RoFormer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-12 16:31:40.000000 BS-RoFormer-0.4.0/BS_RoFormer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-12 16:31:40.000000 BS-RoFormer-0.4.0/BS_RoFormer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-12-12 16:31:30.000000 BS-RoFormer-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      833 2023-12-12 16:31:40.734708 BS-RoFormer-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2023-12-12 16:31:30.000000 BS-RoFormer-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 16:31:40.734708 BS-RoFormer-0.4.0/bs_roformer/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-12 16:31:30.000000 BS-RoFormer-0.4.0/bs_roformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2023-12-12 16:31:30.000000 BS-RoFormer-0.4.0/bs_roformer/attend.py
--rw-r--r--   0 runner    (1001) docker     (127)    13936 2023-12-12 16:31:30.000000 BS-RoFormer-0.4.0/bs_roformer/bs_roformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18487 2023-12-12 16:31:30.000000 BS-RoFormer-0.4.0/bs_roformer/mel_band_roformer.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-12 16:31:40.734708 BS-RoFormer-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-12-12 16:31:30.000000 BS-RoFormer-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:44:22.514892 bs_roformer-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:44:22.514892 bs_roformer-0.4.1/BS_RoFormer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-21 16:44:22.000000 bs_roformer-0.4.1/BS_RoFormer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-21 16:44:22.000000 bs_roformer-0.4.1/BS_RoFormer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 16:44:22.000000 bs_roformer-0.4.1/BS_RoFormer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-21 16:44:22.000000 bs_roformer-0.4.1/BS_RoFormer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 16:44:22.000000 bs_roformer-0.4.1/BS_RoFormer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-21 16:44:18.000000 bs_roformer-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-21 16:44:22.514892 bs_roformer-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-04-21 16:44:18.000000 bs_roformer-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:44:22.510892 bs_roformer-0.4.1/bs_roformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-21 16:44:18.000000 bs_roformer-0.4.1/bs_roformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-21 16:44:18.000000 bs_roformer-0.4.1/bs_roformer/attend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13936 2024-04-21 16:44:18.000000 bs_roformer-0.4.1/bs_roformer/bs_roformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18636 2024-04-21 16:44:18.000000 bs_roformer-0.4.1/bs_roformer/mel_band_roformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 16:44:22.514892 bs_roformer-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-21 16:44:18.000000 bs_roformer-0.4.1/setup.py
```

### Comparing `BS-RoFormer-0.4.0/BS_RoFormer.egg-info/PKG-INFO` & `bs_roformer-0.4.1/BS_RoFormer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BS-RoFormer
-Version: 0.4.0
+Version: 0.4.1
 Summary: BS-RoFormer - Band-Split Rotary Transformer for SOTA Music Source Separation
 Home-page: https://github.com/lucidrains/BS-RoFormer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,music source separation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `BS-RoFormer-0.4.0/LICENSE` & `bs_roformer-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BS-RoFormer-0.4.0/PKG-INFO` & `bs_roformer-0.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BS-RoFormer
-Version: 0.4.0
+Version: 0.4.1
 Summary: BS-RoFormer - Band-Split Rotary Transformer for SOTA Music Source Separation
 Home-page: https://github.com/lucidrains/BS-RoFormer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,music source separation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `BS-RoFormer-0.4.0/README.md` & `bs_roformer-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `BS-RoFormer-0.4.0/bs_roformer/attend.py` & `bs_roformer-0.4.1/bs_roformer/attend.py`

 * *Files identical despite different names*

### Comparing `BS-RoFormer-0.4.0/bs_roformer/bs_roformer.py` & `bs_roformer-0.4.1/bs_roformer/bs_roformer.py`

 * *Files identical despite different names*

### Comparing `BS-RoFormer-0.4.0/bs_roformer/mel_band_roformer.py` & `bs_roformer-0.4.1/bs_roformer/mel_band_roformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         self.norm = RMSNorm(dim)
 
         self.to_qkv = nn.Sequential(
             nn.Linear(dim, dim_inner * 3, bias = False),
             Rearrange('b n (qkv h d) -> qkv b h d n', qkv = 3, h = heads)
         )
 
-        self.temperature = nn.Parameter(torch.ones(heads, 1, 1))
+        self.temperature = nn.Parameter(torch.zeros(heads, 1, 1))
 
         self.attend = Attend(
             scale = scale,
             dropout = dropout,
             flash = flash
         )
 
@@ -319,14 +319,15 @@
         linear_transformer_depth = 1,
         num_bands = 60,
         dim_head = 64,
         heads = 8,
         attn_dropout = 0.1,
         ff_dropout = 0.1,
         flash_attn = True,
+        linear_flash_attn = None,
         dim_freqs_in = 1025,
         sample_rate = 44100,     # needed for mel filter bank from librosa
         stft_n_fft = 2048,
         stft_hop_length = 512,   # 10ms at 44100Hz, from sections 4.1, 4.4 in the paper - @faroit recommends // 2 or // 4 for better reconstruction
         stft_win_length = 2048,
         stft_normalized = False,
         stft_window_fn: Optional[Callable] = None,
@@ -348,25 +349,26 @@
 
         transformer_kwargs = dict(
             dim = dim,
             heads = heads,
             dim_head = dim_head,
             attn_dropout = attn_dropout,
             ff_dropout = ff_dropout,
-            flash_attn = flash_attn
         )
 
         time_rotary_embed = RotaryEmbedding(dim = dim_head)
         freq_rotary_embed = RotaryEmbedding(dim = dim_head)
 
+        linear_flash_attn = default(linear_flash_attn, flash_attn)
+
         for _ in range(depth):
             self.layers.append(nn.ModuleList([
-                Transformer(depth = linear_transformer_depth, linear_attn = True, **transformer_kwargs) if linear_transformer_depth > 0 else None,
-                Transformer(depth = time_transformer_depth, rotary_embed = time_rotary_embed, **transformer_kwargs),
-                Transformer(depth = freq_transformer_depth, rotary_embed = freq_rotary_embed, **transformer_kwargs)
+                Transformer(depth = linear_transformer_depth, linear_attn = True, flash_attn = linear_flash_attn, **transformer_kwargs) if linear_transformer_depth > 0 else None,
+                Transformer(depth = time_transformer_depth, rotary_embed = time_rotary_embed, flash_attn = flash_attn, **transformer_kwargs),
+                Transformer(depth = freq_transformer_depth, rotary_embed = freq_rotary_embed, flash_attn = flash_attn, **transformer_kwargs)
             ]))
 
         self.stft_window_fn = partial(default(stft_window_fn, torch.hann_window), stft_win_length)
 
         self.stft_kwargs = dict(
             n_fft = stft_n_fft,
             hop_length = stft_hop_length,
```

### Comparing `BS-RoFormer-0.4.0/setup.py` & `bs_roformer-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'BS-RoFormer',
   packages = find_packages(exclude=[]),
-  version = '0.4.0',
+  version = '0.4.1',
   license='MIT',
   description = 'BS-RoFormer - Band-Split Rotary Transformer for SOTA Music Source Separation',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/BS-RoFormer',
   keywords = [
```


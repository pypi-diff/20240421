# Comparing `tmp/sae_lens-0.5.1.tar.gz` & `tmp/sae_lens-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-0.5.1.tar", max compression
+gzip compressed data, was "sae_lens-0.6.0.tar", max compression
```

## Comparing `sae_lens-0.5.1.tar` & `sae_lens-0.6.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1069 2024-04-19 11:04:19.539424 sae_lens-0.5.1/LICENSE
--rw-r--r--   0        0        0     2553 2024-04-19 11:04:19.539424 sae_lens-0.5.1/README.md
--rw-r--r--   0        0        0     1775 2024-04-19 11:04:20.771440 sae_lens-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      943 2024-04-19 11:04:20.771440 sae_lens-0.5.1/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15645 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0      992 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    17944 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     5562 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0        0 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/__init__.py
--rw-r--r--   0        0        0    16793 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     2849 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0     9804 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/config.py
--rw-r--r--   0        0        0     6169 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     1528 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     1020 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/load_model.py
--rw-r--r--   0        0        0     3675 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/optim.py
--rw-r--r--   0        0        0     8052 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     2319 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    14328 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     3276 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    17362 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    19031 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     4888 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0     1628 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/utils.py
--rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 sae_lens-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-21 14:42:33.992668 sae_lens-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2553 2024-04-21 14:42:33.992668 sae_lens-0.6.0/README.md
+-rw-r--r--   0        0        0     1773 2024-04-21 14:42:35.020676 sae_lens-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      943 2024-04-21 14:42:35.020676 sae_lens-0.6.0/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0    15645 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/analysis/dashboard_runner.py
+-rw-r--r--   0        0        0     3535 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0      992 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    17944 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     6645 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0        0 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0      471 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/activation_functions.py
+-rw-r--r--   0        0        0    16793 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     2849 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/cache_activations_runner.py
+-rw-r--r--   0        0        0     9927 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/config.py
+-rw-r--r--   0        0        0     6169 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/evals.py
+-rw-r--r--   0        0        0     3747 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     1528 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/lm_runner.py
+-rw-r--r--   0        0        0     1020 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/load_model.py
+-rw-r--r--   0        0        0     3675 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/optim.py
+-rw-r--r--   0        0        0     8052 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/sae_group.py
+-rw-r--r--   0        0        0     2319 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/session_loader.py
+-rw-r--r--   0        0        0    15324 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     3276 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/toy_model_runner.py
+-rw-r--r--   0        0        0    17362 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0    19179 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/train_sae_on_language_model.py
+-rw-r--r--   0        0        0     5002 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/train_sae_on_toy_model.py
+-rw-r--r--   0        0        0     1628 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/utils.py
+-rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 sae_lens-0.6.0/PKG-INFO
```

### Comparing `sae_lens-0.5.1/LICENSE` & `sae_lens-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/README.md` & `sae_lens-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/pyproject.toml` & `sae_lens-0.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "0.5.1"
+version = "0.6.0"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -30,19 +30,19 @@
 safetensors = "^0.4.2"
 typer = "^0.12.3"
 mamba-lens = { version = "^0.0.4", optional = true }
 pyzmq = "26.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
-black = "^24.2.0"
+black = "24.4.0"
 pytest = "^8.0.2"
 pytest-cov = "^4.1.0"
 pre-commit = "^3.6.2"
-flake8 = "^7.0.0"
+flake8 = "7.0.0"
 isort = "5.13.2"
 pyright = "^1.1.351"
 mamba-lens = "^0.0.4"
 
 [tool.poetry.extras]
 mamba = ["mamba-lens"]
```

### Comparing `sae_lens-0.5.1/sae_lens/__init__.py` & `sae_lens-0.6.0/sae_lens/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.5.1"
+__version__ = "0.6.0"
 
 from .training.activations_store import ActivationsStore
 from .training.cache_activations_runner import cache_activations_runner
 from .training.config import CacheActivationsRunnerConfig, LanguageModelSAERunnerConfig
 from .training.evals import run_evals
 from .training.lm_runner import language_model_sae_runner
 from .training.sae_group import SparseAutoencoderDictionary
```

### Comparing `sae_lens-0.5.1/sae_lens/analysis/dashboard_runner.py` & `sae_lens-0.6.0/sae_lens/analysis/dashboard_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/sae_lens/analysis/feature_statistics.py` & `sae_lens-0.6.0/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/sae_lens/analysis/neuronpedia_integration.py` & `sae_lens-0.6.0/sae_lens/analysis/neuronpedia_integration.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-0.6.0/sae_lens/analysis/neuronpedia_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/sae_lens/analysis/tsea.py` & `sae_lens-0.6.0/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-0.6.0/sae_lens/toolkit/pretrained_saes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+import pathlib
 from typing import Optional, Tuple
 
 import torch
 from huggingface_hub import hf_hub_download, list_files_info
 from safetensors import safe_open
 from tqdm import tqdm
 
@@ -131,14 +132,43 @@
     )
 
     ae_alt = SparseAutoencoder(cfg)
     ae_alt.load_state_dict(state_dict)
     return ae_alt
 
 
+def convert_old_to_modern_saelens_format(
+    pytorch_file: str, out_folder: str = "", force: bool = False
+):
+    """
+    Reads a pretrained SAE from the old pickle-style SAELens .pt format, then saves a modern-format SAELens SAE.
+
+    Arguments:
+    ----------
+    pytorch_file: str
+        Path of old format file to open.
+    out_folder: str, optional
+        Path where new SAE will be stored; if None, out_folder = pytorch_file with the '.pt' removed.
+    force: bool, optional
+        If out_folder already exists, this function will not save unless force=True.
+    """
+    file_path = pathlib.Path(pytorch_file)
+    if out_folder == "":
+        out_f = file_path.parent / file_path.stem
+    else:
+        out_f = pathlib.Path(out_folder)
+    if (not force) and out_f.exists():
+        raise FileExistsError(f"{out_folder} already exists and force=False")
+    out_f.mkdir(exist_ok=True, parents=True)
+
+    # Load model & save in new format.
+    autoencoder = SparseAutoencoder.load_from_pretrained_legacy(str(file_path))
+    autoencoder.save_model(str(out_f))
+
+
 def get_gpt2_small_ckrk_attn_out_saes() -> dict[str, SparseAutoencoder]:
 
     REPO_ID = "ckkissane/attn-saes-gpt2-small-all-layers"
 
     # list all files in repo
     saes_weights = {}
     sae_configs = {}
```

### Comparing `sae_lens-0.5.1/sae_lens/training/activations_store.py` & `sae_lens-0.6.0/sae_lens/training/activations_store.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/sae_lens/training/cache_activations_runner.py` & `sae_lens-0.6.0/sae_lens/training/cache_activations_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/sae_lens/training/config.py` & `sae_lens-0.6.0/sae_lens/training/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,17 @@
     )
 
     # SAE Parameters
     d_in: int = 512
     d_sae: Optional[int] = None
     b_dec_init_method: str = "geometric_median"
     expansion_factor: int | list[int] = 4
+    activation_fn: str = "relu"  # relu, tanh-relu
+    normalize_sae_decoder: bool = True
+    noise_scale: float = 0.0
     from_pretrained_path: Optional[str] = None
     apply_b_dec_to_input: bool = True
     decoder_orthogonal_init: bool = False
 
     # Activation Store Parameters
     n_batches_in_buffer: int = 20
     training_tokens: int = 2_000_000
@@ -163,18 +166,18 @@
             print(
                 f"Run name: {self.d_sae}-L1-{self.l1_coefficient}-LR-{self.lr}-Tokens-{self.training_tokens:3.3e}"
             )
             # Print out some useful info:
             n_tokens_per_buffer = (
                 self.store_batch_size * self.context_size * self.n_batches_in_buffer
             )
-            print(f"n_tokens_per_buffer (millions): {n_tokens_per_buffer / 10 **6}")
+            print(f"n_tokens_per_buffer (millions): {n_tokens_per_buffer / 10 ** 6}")
             n_contexts_per_buffer = self.store_batch_size * self.n_batches_in_buffer
             print(
-                f"Lower bound: n_contexts_per_buffer (millions): {n_contexts_per_buffer / 10 **6}"
+                f"Lower bound: n_contexts_per_buffer (millions): {n_contexts_per_buffer / 10 ** 6}"
             )
 
             total_training_steps = (
                 self.training_tokens + self.finetuning_tokens
             ) // self.train_batch_size
             print(f"Total training steps: {total_training_steps}")
 
@@ -183,18 +186,18 @@
 
             # how many times will we sample dead neurons?
             # assert self.dead_feature_window <= self.feature_sampling_window, "dead_feature_window must be smaller than feature_sampling_window"
             n_feature_window_samples = (
                 total_training_steps // self.feature_sampling_window
             )
             print(
-                f"n_tokens_per_feature_sampling_window (millions): {(self.feature_sampling_window * self.context_size * self.train_batch_size) / 10 **6}"
+                f"n_tokens_per_feature_sampling_window (millions): {(self.feature_sampling_window * self.context_size * self.train_batch_size) / 10 ** 6}"
             )
             print(
-                f"n_tokens_per_dead_feature_window (millions): {(self.dead_feature_window * self.context_size * self.train_batch_size) / 10 **6}"
+                f"n_tokens_per_dead_feature_window (millions): {(self.dead_feature_window * self.context_size * self.train_batch_size) / 10 ** 6}"
             )
             print(
                 f"We will reset the sparsity calculation {n_feature_window_samples} times."
             )
             # print("Number tokens in dead feature calculation window: ", self.dead_feature_window * self.train_batch_size)
             print(
                 f"Number tokens in sparsity calculation window: {self.feature_sampling_window * self.train_batch_size:.2e}"
```

### Comparing `sae_lens-0.5.1/sae_lens/training/evals.py` & `sae_lens-0.6.0/sae_lens/training/evals.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/sae_lens/training/geometric_median.py` & `sae_lens-0.6.0/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/sae_lens/training/lm_runner.py` & `sae_lens-0.6.0/sae_lens/training/lm_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/sae_lens/training/load_model.py` & `sae_lens-0.6.0/sae_lens/training/load_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/sae_lens/training/optim.py` & `sae_lens-0.6.0/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/sae_lens/training/sae_group.py` & `sae_lens-0.6.0/sae_lens/training/sae_group.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/sae_lens/training/session_loader.py` & `sae_lens-0.6.0/sae_lens/training/session_loader.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/sae_lens/training/sparse_autoencoder.py` & `sae_lens-0.6.0/sae_lens/training/sparse_autoencoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 https://github.com/ArthurConmy/sae/blob/main/sae/model.py
 """
 
 import gzip
 import json
 import os
 import pickle
-from typing import NamedTuple, Optional
+from typing import Callable, NamedTuple, Optional
 
 import einops
 import torch
 from safetensors import safe_open
 from safetensors.torch import save_file
 from torch import nn
 from transformer_lens.hook_points import HookedRootModule, HookPoint
 
+from sae_lens.training.activation_functions import get_activation_fn
 from sae_lens.training.config import LanguageModelSAERunnerConfig
 from sae_lens.training.utils import BackwardsCompatiblePickleClass
 
 
 class ForwardOutput(NamedTuple):
     sae_out: torch.Tensor
     feature_acts: torch.Tensor
@@ -31,17 +32,20 @@
 class SparseAutoencoder(HookedRootModule):
     """ """
 
     l1_coefficient: float
     lp_norm: float
     d_sae: int
     use_ghost_grads: bool
+    normalize_sae_decoder: bool
     hook_point_layer: int
     dtype: torch.dtype
     device: str | torch.device
+    noise_scale: float
+    activation_fn: Callable[[torch.Tensor], torch.Tensor]
 
     def __init__(
         self,
         cfg: LanguageModelSAERunnerConfig,
     ):
         super().__init__()
         self.cfg = cfg
@@ -65,15 +69,18 @@
 
         self.d_sae = cfg.d_sae
         self.l1_coefficient = cfg.l1_coefficient
         self.lp_norm = cfg.lp_norm
         self.dtype = cfg.dtype
         self.device = cfg.device
         self.use_ghost_grads = cfg.use_ghost_grads
+        self.normalize_sae_decoder = cfg.normalize_sae_decoder
         self.hook_point_layer = cfg.hook_point_layer
+        self.noise_scale = cfg.noise_scale
+        self.activation_fn = get_activation_fn(cfg.activation_fn)
 
         # NOTE: if using resampling neurons method, you must ensure that we initialise the weights in the order W_enc, b_enc, W_dec, b_dec
         self.W_enc = nn.Parameter(
             torch.nn.init.kaiming_uniform_(
                 torch.empty(self.d_in, self.d_sae, dtype=self.dtype, device=self.device)
             )
         )
@@ -86,17 +93,18 @@
                 torch.empty(self.d_sae, self.d_in, dtype=self.dtype, device=self.device)
             )
         )
 
         if self.cfg.decoder_orthogonal_init:
             self.W_dec.data = nn.init.orthogonal_(self.W_dec.data.T).T
 
-        with torch.no_grad():
-            # Anthropic normalize this to have unit columns
-            self.set_decoder_norm_to_unit_norm()
+        if self.normalize_sae_decoder:
+            with torch.no_grad():
+                # Anthropic normalize this to have unit columns
+                self.set_decoder_norm_to_unit_norm()
 
         self.b_dec = nn.Parameter(
             torch.zeros(self.d_in, dtype=self.dtype, device=self.device)
         )
 
         # scaling factor for fine-tuning (not to be used in initial training)
         self.scaling_factor = nn.Parameter(
@@ -121,15 +129,19 @@
             einops.einsum(
                 sae_in,
                 self.W_enc,
                 "... d_in, d_in d_sae -> ... d_sae",
             )
             + self.b_enc
         )
-        feature_acts = self.hook_hidden_post(torch.nn.functional.relu(hidden_pre))
+        noisy_hidden_pre = hidden_pre
+        if self.noise_scale > 0:
+            noise = torch.randn_like(hidden_pre) * self.noise_scale
+            noisy_hidden_pre = hidden_pre + noise
+        feature_acts = self.hook_hidden_post(self.activation_fn(noisy_hidden_pre))
 
         sae_out = self.hook_sae_out(
             einops.einsum(
                 feature_acts
                 * self.scaling_factor,  # need to make sure this handled when loading old models.
                 self.W_dec,
                 "... d_sae, d_sae d_in -> ... d_in",
@@ -276,18 +288,19 @@
                     state_dict = torch.load(
                         path,
                         map_location="mps",
                         pickle_module=BackwardsCompatiblePickleClass,
                     )
                     state_dict["cfg"].device = "mps"
                 else:
-                    state_dict = torch.load(path)
+                    state_dict = torch.load(
+                        path, pickle_module=BackwardsCompatiblePickleClass
+                    )
             except Exception as e:
                 raise IOError(f"Error loading the state dictionary from .pt file: {e}")
-
         elif path.endswith(".pkl.gz"):
             try:
                 with gzip.open(path, "rb") as f:
                     state_dict = pickle.load(f)
             except Exception as e:
                 raise IOError(
                     f"Error loading the state dictionary from .pkl.gz file: {e}"
@@ -307,15 +320,20 @@
         if "cfg" not in state_dict or "state_dict" not in state_dict:
             raise ValueError(
                 "The loaded state dictionary must contain 'cfg' and 'state_dict' keys"
             )
 
         # Create an instance of the class using the loaded configuration
         instance = cls(cfg=state_dict["cfg"])
-        instance.load_state_dict(state_dict["state_dict"])
+        if "scaling_factor" not in state_dict["state_dict"]:
+            assert isinstance(instance.cfg.d_sae, int)
+            state_dict["state_dict"]["scaling_factor"] = torch.ones(
+                instance.cfg.d_sae, dtype=instance.cfg.dtype, device=instance.cfg.device
+            )
+        instance.load_state_dict(state_dict["state_dict"], strict=True)
 
         return instance
 
     @classmethod
     def load_from_pretrained(cls, path: str, device: str = "cpu"):
 
         config_path = os.path.join(path, "cfg.json")
```

### Comparing `sae_lens-0.5.1/sae_lens/training/toy_model_runner.py` & `sae_lens-0.6.0/sae_lens/training/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/sae_lens/training/toy_models.py` & `sae_lens-0.6.0/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/sae_lens/training/train_sae_on_language_model.py` & `sae_lens-0.6.0/sae_lens/training/train_sae_on_language_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,15 +373,16 @@
 ) -> TrainStepOutput:
     assert sparse_autoencoder.cfg.d_sae is not None  # keep pyright happy
     layer_id = all_layers.index(sparse_autoencoder.hook_point_layer)
     sae_in = layer_acts[:, layer_id, :]
 
     sparse_autoencoder.train()
     # Make sure the W_dec is still zero-norm
-    sparse_autoencoder.set_decoder_norm_to_unit_norm()
+    if sparse_autoencoder.normalize_sae_decoder:
+        sparse_autoencoder.set_decoder_norm_to_unit_norm()
 
     # log and then reset the feature sparsity every feature_sampling_window steps
     if (n_training_steps + 1) % feature_sampling_window == 0:
         feature_sparsity = ctx.feature_sparsity
         log_feature_sparsity = _log_feature_sparsity(feature_sparsity)
 
         if use_wandb:
@@ -428,15 +429,16 @@
     with torch.no_grad():
         # Calculate the sparsities, and add it to a list, calculate sparsity metrics
         ctx.act_freq_scores += (feature_acts.abs() > 0).float().sum(0)
         ctx.n_frac_active_tokens += batch_size
 
     ctx.optimizer.zero_grad()
     loss.backward()
-    sparse_autoencoder.remove_gradient_parallel_to_decoder_directions()
+    if sparse_autoencoder.normalize_sae_decoder:
+        sparse_autoencoder.remove_gradient_parallel_to_decoder_directions()
     ctx.optimizer.step()
     ctx.scheduler.step()
 
     return TrainStepOutput(
         sae_in=sae_in,
         sae_out=sae_out,
         feature_acts=feature_acts,
@@ -500,15 +502,16 @@
 
     checkpoint_path = f"{sae_group.cfg.checkpoint_path}/{checkpoint_name}"
     os.makedirs(checkpoint_path, exist_ok=True)
     for name, sae in sae_group.autoencoders.items():
 
         ctx = train_contexts[name]
         path = f"{checkpoint_path}/{name}"
-        sae.set_decoder_norm_to_unit_norm()
+        if sae.normalize_sae_decoder:
+            sae.set_decoder_norm_to_unit_norm()
         sae.save_model(path)
         log_feature_sparsities = {"sparsity": ctx.log_feature_sparsity}
 
         log_feature_sparsity_path = f"{path}/sparsity.safetensors"
         save_file(log_feature_sparsities, log_feature_sparsity_path)
 
         if sae_group.cfg.log_to_wandb and os.path.exists(log_feature_sparsity_path):
```

### Comparing `sae_lens-0.5.1/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-0.6.0/sae_lens/training/train_sae_on_toy_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,21 +33,23 @@
     n_training_steps = 0
     n_training_tokens = 0
 
     pbar = tqdm(dataloader, desc="Training SAE")
     for _, batch in enumerate(pbar):
         batch = next(dataloader)
         # Make sure the W_dec is still zero-norm
-        sparse_autoencoder.set_decoder_norm_to_unit_norm()
+        if sparse_autoencoder.normalize_sae_decoder:
+            sparse_autoencoder.set_decoder_norm_to_unit_norm()
 
         # Forward and Backward Passes
         optimizer.zero_grad()
         sae_out, feature_acts, loss, mse_loss, l1_loss, _ = sparse_autoencoder(batch)
         loss.backward()
-        sparse_autoencoder.remove_gradient_parallel_to_decoder_directions()
+        if sparse_autoencoder.normalize_sae_decoder:
+            sparse_autoencoder.remove_gradient_parallel_to_decoder_directions()
         optimizer.step()
 
         n_training_tokens += batch_size
 
         with torch.no_grad():
             # Calculate the sparsities, and add it to a list
             act_freq_scores = (feature_acts.abs() > 0).float().sum(0)
```

### Comparing `sae_lens-0.5.1/sae_lens/training/utils.py` & `sae_lens-0.6.0/sae_lens/training/utils.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.1/PKG-INFO` & `sae_lens-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 0.5.1
+Version: 0.6.0
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```


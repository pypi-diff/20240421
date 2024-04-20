# Comparing `tmp/token_trace-0.1.0.tar.gz` & `tmp/token_trace-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "token_trace-0.1.0.tar", last modified: Thu Apr 18 01:32:22 2024, max compression
+gzip compressed data, was "token_trace-0.2.1.tar", last modified: Sat Apr 20 22:08:37 2024, max compression
```

## Comparing `token_trace-0.1.0.tar` & `token_trace-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,29 @@
--rw-r--r--   0        0        0     1068 2024-04-18 01:31:15.794864 token_trace-0.1.0/LICENSE
--rw-r--r--   0        0        0     1593 2024-04-18 01:31:15.794864 token_trace-0.1.0/README.md
--rw-r--r--   0        0        0     1193 2024-04-18 01:32:22.370679 token_trace-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 01:31:15.794864 token_trace-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      445 2024-04-18 01:31:15.794864 token_trace-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1940 2024-04-18 01:31:15.794864 token_trace-0.1.0/tests/helpers.py
--rw-r--r--   0        0        0     2005 2024-04-18 01:31:15.794864 token_trace-0.1.0/tests/test_sae_circuit.py
--rw-r--r--   0        0        0     5295 2024-04-18 01:31:15.794864 token_trace-0.1.0/tests/test_sae_patcher.py
--rw-r--r--   0        0        0      111 2024-04-18 01:31:15.794864 token_trace-0.1.0/token_trace/__init__.py
--rw-r--r--   0        0        0     4314 2024-04-18 01:31:15.794864 token_trace-0.1.0/token_trace/compute_node_attribution.py
--rw-r--r--   0        0        0     2468 2024-04-18 01:31:15.794864 token_trace-0.1.0/token_trace/get_data.py
--rw-r--r--   0        0        0     5796 2024-04-18 01:31:15.794864 token_trace-0.1.0/token_trace/print_prompt_info.py
--rw-r--r--   0        0        0     4062 2024-04-18 01:31:15.794864 token_trace-0.1.0/token_trace/sae_circuit.py
--rw-r--r--   0        0        0     4694 2024-04-18 01:31:15.794864 token_trace-0.1.0/token_trace/sae_patcher.py
--rw-r--r--   0        0        0     1735 2024-04-18 01:31:15.794864 token_trace-0.1.0/token_trace/utils.py
--rw-r--r--   0        0        0     1969 1970-01-01 00:00:00.000000 token_trace-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-13 13:14:05.229465 token_trace-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1602 2024-04-19 22:14:54.225885 token_trace-0.2.1/README.md
+-rw-r--r--   0        0        0     1994 2024-04-20 22:08:37.124901 token_trace-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 13:20:18.948778 token_trace-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      174 2024-04-20 20:47:20.249121 token_trace-0.2.1/tests/app/test_get_data.py
+-rw-r--r--   0        0        0      733 2024-04-20 20:47:20.249121 token_trace-0.2.1/tests/circuit/test_edge_attribution.py
+-rw-r--r--   0        0        0      631 2024-04-20 20:47:20.249121 token_trace-0.2.1/tests/circuit/test_node_attribution.py
+-rw-r--r--   0        0        0     1698 2024-04-20 20:47:20.249121 token_trace-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     1940 2024-04-18 00:33:32.206128 token_trace-0.2.1/tests/helpers.py
+-rw-r--r--   0        0        0      940 2024-04-20 20:47:20.249121 token_trace-0.2.1/tests/test_sae_activation_cache.py
+-rw-r--r--   0        0        0     5255 2024-04-20 20:47:20.249121 token_trace-0.2.1/tests/test_sae_patcher.py
+-rw-r--r--   0        0        0     1073 2024-04-19 15:47:33.361295 token_trace-0.2.1/tests/test_utils.py
+-rw-r--r--   0        0        0       22 2024-04-20 21:26:04.157785 token_trace-0.2.1/token_trace/__init__.py
+-rw-r--r--   0        0        0       55 2024-04-19 22:20:43.704861 token_trace-0.2.1/token_trace/app/__init__.py
+-rw-r--r--   0        0        0     2052 2024-04-20 21:54:12.996159 token_trace-0.2.1/token_trace/app/get_circuit.py
+-rw-r--r--   0        0        0     1066 2024-04-20 20:47:20.249121 token_trace-0.2.1/token_trace/app/process_data.py
+-rw-r--r--   0        0        0    12078 2024-04-20 21:37:36.207679 token_trace-0.2.1/token_trace/app/run_app.py
+-rw-r--r--   0        0        0      176 2024-04-20 21:56:44.029372 token_trace-0.2.1/token_trace/circuit/__init__.py
+-rw-r--r--   0        0        0     6024 2024-04-20 21:57:57.925590 token_trace-0.2.1/token_trace/circuit/edge_attribution.py
+-rw-r--r--   0        0        0     4449 2024-04-20 21:57:50.421566 token_trace-0.2.1/token_trace/circuit/node_attribution.py
+-rw-r--r--   0        0        0     6709 2024-04-20 21:56:23.349268 token_trace-0.2.1/token_trace/circuit/sparse_feature_circuit.py
+-rw-r--r--   0        0        0      296 2024-04-20 20:47:20.249121 token_trace-0.2.1/token_trace/constants.py
+-rw-r--r--   0        0        0     2353 2024-04-20 20:47:20.249121 token_trace-0.2.1/token_trace/load_pretrained_model.py
+-rw-r--r--   0        0        0     5796 2024-04-18 00:33:45.182230 token_trace-0.2.1/token_trace/print_prompt_info.py
+-rw-r--r--   0        0        0     1628 2024-04-20 20:47:20.249121 token_trace-0.2.1/token_trace/sae_activation_cache.py
+-rw-r--r--   0        0        0     4608 2024-04-20 20:47:20.249121 token_trace-0.2.1/token_trace/sae_patcher.py
+-rw-r--r--   0        0        0      708 2024-04-20 20:47:20.249121 token_trace-0.2.1/token_trace/types.py
+-rw-r--r--   0        0        0     2614 2024-04-20 21:44:38.319271 token_trace-0.2.1/token_trace/utils.py
+-rw-r--r--   0        0        0     2242 1970-01-01 00:00:00.000000 token_trace-0.2.1/PKG-INFO
```

### Comparing `token_trace-0.1.0/LICENSE` & `token_trace-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `token_trace-0.1.0/README.md` & `token_trace-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-# token-trace
+# Token-Trace
 
 A tool and UI to construct prompt-centric views of SAE feature attributions.
 
 Main functionality:
 - We use this tool to identify which SAE features have the most 'attribution' towards decreasing the model loss. 
 - In combination with Neuronpedia, we can identify what each SAE feature represents; this then gives us a rough idea of what computation the model is performing. 
 
 This tool is a first step towards discovering information flow between the features / layers of a transformer
 
+
+# Quickstart
+
 ## Installation
 
 ```
-git clone https://github.com/interp-hack/token-trace.git
-pip install -e .
-``` 
-
-## Quickstart
+pip install token-trace
+```
+## Example Usage
 
 ```
 from token_trace import compute_node_attribution
 
 text = "When John and Mary went to the shops, John gave the bag to Mary"
 
 df: pd.DataFrame = compute_node_attribution(
     model_name = "gpt2",
     text
 )
 ```
 
 Each row of `df` describes one node corresponding to an SAE feature or error term. 
 
-## Front-end
+## Visualizing SAE attribution statistics in frontend. 
 
 We use [Streamlit](https://streamlit.io/) to create a UI. Start the app as follows:
 ```
 streamlit run app/token_trace_app.py
 ```
 
 ## Methodology
```

### Comparing `token_trace-0.1.0/tests/helpers.py` & `token_trace-0.2.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.1.0/tests/test_sae_patcher.py` & `token_trace-0.2.1/tests/test_sae_patcher.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,151 +3,151 @@
 from sae_lens import SparseAutoencoder
 from transformer_lens import HookedTransformer
 
 from token_trace.sae_patcher import SAEPatcher
 
 
 def test_sae_patcher_hook_forward_hook_only(
-    model: HookedTransformer, sae: SparseAutoencoder, prompt: str
+    model: HookedTransformer, sae: SparseAutoencoder, text: str
 ):
-    orig_loss = model(prompt, return_type="loss")
+    orig_loss = model(text, return_type="loss")
     sae_patcher = SAEPatcher(sae)
 
     with model.hooks(
         fwd_hooks=[sae_patcher.get_forward_hook()],
     ):
-        patched_loss = model(prompt, return_type="loss")
+        patched_loss = model(text, return_type="loss")
 
     assert torch.isclose(orig_loss, patched_loss, atol=1e-6)
 
 
 def test_sae_patcher_backward_hook_only(
-    model: HookedTransformer, sae: SparseAutoencoder, prompt: str
+    model: HookedTransformer, sae: SparseAutoencoder, text: str
 ):
-    orig_loss = model(prompt, return_type="loss")
+    orig_loss = model(text, return_type="loss")
     sae_patcher = SAEPatcher(sae)
 
     with model.hooks(
         bwd_hooks=[sae_patcher.get_backward_hook()],
     ):
-        patched_loss = model(prompt, return_type="loss")
+        patched_loss = model(text, return_type="loss")
 
     assert torch.isclose(orig_loss, patched_loss, atol=1e-6)
 
 
 def get_grads(model: nn.Module) -> list[tuple[str, torch.Tensor]]:
     grads = []
     for name, param in model.named_parameters():
         assert param.grad is not None
         grads.append((name, param.grad))
     return grads
 
 
 def test_sae_patcher_preserves_cached_model_activations(
-    model: HookedTransformer, sae: SparseAutoencoder, prompt: str
+    model: HookedTransformer, sae: SparseAutoencoder, text: str
 ):
-    _, orig_cache = model.run_with_cache(prompt, return_type="loss")
+    _, orig_cache = model.run_with_cache(text, return_type="loss")
     sae_patcher = SAEPatcher(sae)
 
     with model.hooks(
         fwd_hooks=[sae_patcher.get_forward_hook()],
         bwd_hooks=[sae_patcher.get_backward_hook()],
     ):
-        _, patched_cache = model.run_with_cache(prompt, return_type="loss")
+        _, patched_cache = model.run_with_cache(text, return_type="loss")
 
     for orig_name, patched_name in zip(orig_cache, patched_cache):
         assert orig_name == patched_name
         orig_act = orig_cache[orig_name]
         patched_act = patched_cache[patched_name]
         assert torch.allclose(orig_act, patched_act, atol=1e-4, rtol=1e-4)
 
 
 def test_sae_patcher_preserves_model_grad(
-    model: HookedTransformer, sae: SparseAutoencoder, prompt: str
+    model: HookedTransformer, sae: SparseAutoencoder, text: str
 ):
-    orig_loss = model(prompt, return_type="loss")
+    orig_loss = model(text, return_type="loss")
     orig_loss.backward()
     orig_grads = get_grads(model)
     sae_patcher = SAEPatcher(sae)
 
     with model.hooks(
         fwd_hooks=[sae_patcher.get_forward_hook()],
         bwd_hooks=[sae_patcher.get_backward_hook()],
     ):
-        patched_loss = model(prompt, return_type="loss")
+        patched_loss = model(text, return_type="loss")
         patched_loss.backward()
         patched_grads = get_grads(model)
 
     for (orig_name, orig_grad), (patched_name, patched_grad) in zip(
         orig_grads, patched_grads
     ):
         assert orig_name == patched_name
         assert torch.allclose(orig_grad, patched_grad, atol=1e-5)
 
 
 def test_sae_patcher_fields_have_grad(
-    model: HookedTransformer, sae: SparseAutoencoder, prompt: str
+    model: HookedTransformer, sae: SparseAutoencoder, text: str
 ):
     sae_patcher = SAEPatcher(sae)
     assert sae_patcher.sae_feature_acts.grad is None
     assert sae_patcher.sae_errors.grad is None
 
     with model.hooks(
         fwd_hooks=[sae_patcher.get_forward_hook()],
         bwd_hooks=[sae_patcher.get_backward_hook()],
     ):
-        patched_loss = model(prompt, return_type="loss")
+        patched_loss = model(text, return_type="loss")
         patched_loss.backward()
 
     assert sae_patcher.sae_feature_acts.grad is not None
     assert sae_patcher.sae_errors.grad is not None
 
 
 def test_sae_patcher_get_node_values(
-    model: HookedTransformer, sae: SparseAutoencoder, prompt: str
+    model: HookedTransformer, sae: SparseAutoencoder, text: str
 ):
     # Get the batch size and number of tokens hackily
-    loss = model(prompt, return_type="loss", loss_per_token=True)
+    loss = model(text, return_type="loss", loss_per_token=True)
     assert len(loss.shape) == 2
     n_batch, n_token = loss.shape
     # Next-token prediction loss shape is actually n_token-1 so we add one
     n_token += 1
 
     sae_patcher = SAEPatcher(sae)
     with model.hooks(
         fwd_hooks=[sae_patcher.get_forward_hook()],
         bwd_hooks=[sae_patcher.get_backward_hook()],
     ):
-        patched_loss = model(prompt, return_type="loss")
+        patched_loss = model(text, return_type="loss")
         patched_loss.backward()
 
     feature_node_vals = sae_patcher.get_node_values("feature")
     assert feature_node_vals.shape == (n_batch, n_token, sae.d_sae)
     error_node_vals = sae_patcher.get_node_values("error")
     assert error_node_vals.shape == (n_batch, n_token, sae.d_in)
     all_node_vals = sae_patcher.get_node_values("all")
     assert all_node_vals.shape == (n_batch, n_token, sae.d_sae + sae.d_in)
 
 
 def test_sae_patcher_get_node_grads(
-    model: HookedTransformer, sae: SparseAutoencoder, prompt: str
+    model: HookedTransformer, sae: SparseAutoencoder, text: str
 ):
     # Get the batch size and number of tokens hackily
-    loss = model(prompt, return_type="loss", loss_per_token=True)
+    loss = model(text, return_type="loss", loss_per_token=True)
     assert len(loss.shape) == 2
     n_batch, n_token = loss.shape
     # Next-token prediction loss shape is actually n_token-1 so we add one
     n_token += 1
 
     sae_patcher = SAEPatcher(sae)
     with model.hooks(
         fwd_hooks=[sae_patcher.get_forward_hook()],
         bwd_hooks=[sae_patcher.get_backward_hook()],
     ):
-        patched_loss = model(prompt, return_type="loss")
+        patched_loss = model(text, return_type="loss")
         patched_loss.backward()
 
     feature_node_grads = sae_patcher.get_node_grads("feature")
     assert feature_node_grads.shape == (n_batch, n_token, sae.d_sae)
     error_node_grads = sae_patcher.get_node_grads("error")
     assert error_node_grads.shape == (n_batch, n_token, sae.d_in)
     all_node_grads = sae_patcher.get_node_grads("all")
```

### Comparing `token_trace-0.1.0/token_trace/print_prompt_info.py` & `token_trace-0.2.1/token_trace/print_prompt_info.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.1.0/token_trace/sae_patcher.py` & `token_trace-0.2.1/token_trace/sae_patcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         self.sae_feature_acts = z_sae
         self.sae_errors = a_err
 
         a_rec = a_sae + a_err
         return a_rec
 
     @property
-    def sae_nodes(self) -> Float[torch.Tensor, "n_batch n_token (d_sae + d_model)"]:
+    def sae_nodes(self) -> Float[torch.Tensor, "n_batch n_token (d_sae+d_model)"]:
         return torch.cat([self.sae_feature_acts, self.sae_errors], dim=-1)
 
     def _backward_hook_fn(
         self,
         orig: Float[torch.Tensor, "n_batch n_token d_model"],
         hook: HookPoint,  # noqa: ARG002
     ) -> tuple[Float[torch.Tensor, "n_batch n_token d_model"]]:
@@ -105,34 +105,32 @@
         """Return a backward hook that patches the gradients."""
         return (self.sae.cfg.hook_point, self._backward_hook_fn)
 
     def get_node_values(
         self, node_type: NodeType = "all"
     ) -> Float[torch.Tensor, "n_batch n_token n_nodes"]:
         if node_type == "feature":
-            return self.sae_feature_acts.detach()
+            return self.sae_feature_acts
         elif node_type == "error":
-            return self.sae_errors.detach()
+            return self.sae_errors
         elif node_type == "all":
-            return torch.cat([self.sae_feature_acts, self.sae_errors], dim=-1).detach()
+            return torch.cat([self.sae_feature_acts, self.sae_errors], dim=-1)
         else:
             raise ValueError(f"Invalid node_type: {node_type}")
 
     def get_node_grads(
         self, node_type: NodeType = "all"
     ) -> Float[torch.Tensor, "n_batch n_token n_nodes"]:
         if node_type == "feature":
             if self.sae_feature_acts.grad is None:
                 raise RuntimeError("Gradients are not available.")
-            return self.sae_feature_acts.grad.detach()
+            return self.sae_feature_acts.grad
         elif node_type == "error":
             if self.sae_errors.grad is None:
                 raise RuntimeError("Gradients are not available.")
-            return self.sae_errors.grad.detach()
+            return self.sae_errors.grad
         elif node_type == "all":
             if self.sae_feature_acts.grad is None or self.sae_errors.grad is None:
                 raise RuntimeError("Gradients are not available.")
-            return torch.cat(
-                [self.sae_feature_acts.grad, self.sae_errors.grad], dim=-1
-            ).detach()
+            return torch.cat([self.sae_feature_acts.grad, self.sae_errors.grad], dim=-1)
         else:
             raise ValueError(f"Invalid node_type: {node_type}")
```

### Comparing `token_trace-0.1.0/PKG-INFO` & `token_trace-0.2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 Metadata-Version: 2.1
 Name: token-trace
-Version: 0.1.0
+Version: 0.2.1
 Summary: Transformer token flow visualizer
 Author-Email: "Seongho Son, Liza Karmannaya, Daniel Tan, David Chanin" <chanindav@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: transformers>=4.39.3
 Requires-Dist: transformer-lens>=1.15.0
 Requires-Dist: sae-lens>=0.2.0
+Requires-Dist: pandera>=0.18.3
+Requires-Dist: streamlit>=1.33.0; extra == "client"
+Requires-Dist: st-annotated-text>=4.0.1; extra == "client"
+Requires-Dist: pytest>=8.1.1; extra == "client"
+Requires-Dist: graphviz>=0.20.3; extra == "client"
+Provides-Extra: client
 Description-Content-Type: text/markdown
 
-# token-trace
+# Token-Trace
 
 A tool and UI to construct prompt-centric views of SAE feature attributions.
 
 Main functionality:
 - We use this tool to identify which SAE features have the most 'attribution' towards decreasing the model loss. 
 - In combination with Neuronpedia, we can identify what each SAE feature represents; this then gives us a rough idea of what computation the model is performing. 
 
 This tool is a first step towards discovering information flow between the features / layers of a transformer
 
+
+# Quickstart
+
 ## Installation
 
 ```
-git clone https://github.com/interp-hack/token-trace.git
-pip install -e .
-``` 
-
-## Quickstart
+pip install token-trace
+```
+## Example Usage
 
 ```
 from token_trace import compute_node_attribution
 
 text = "When John and Mary went to the shops, John gave the bag to Mary"
 
 df: pd.DataFrame = compute_node_attribution(
     model_name = "gpt2",
     text
 )
 ```
 
 Each row of `df` describes one node corresponding to an SAE feature or error term. 
 
-## Front-end
+## Visualizing SAE attribution statistics in frontend. 
 
 We use [Streamlit](https://streamlit.io/) to create a UI. Start the app as follows:
 ```
 streamlit run app/token_trace_app.py
 ```
 
 ## Methodology
```


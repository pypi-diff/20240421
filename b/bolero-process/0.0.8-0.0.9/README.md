# Comparing `tmp/bolero_process-0.0.8.tar.gz` & `tmp/bolero_process-0.0.9.tar.gz`

## Comparing `bolero_process-0.0.8.tar` & `bolero_process-0.0.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 bolero_process-0.0.8/.codecov.yaml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bolero_process-0.0.8/.cruft.json
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 bolero_process-0.0.8/.editorconfig
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 bolero_process-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 bolero_process-0.0.8/.readthedocs.yaml
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 bolero_process-0.0.8/CHANGELOG.md
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 bolero_process-0.0.8/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 bolero_process-0.0.8/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 bolero_process-0.0.8/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 bolero_process-0.0.8/.github/workflows/build.yaml
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 bolero_process-0.0.8/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 bolero_process-0.0.8/.github/workflows/test.yaml
--rwxr-xr-x   0        0        0     7290 2020-02-02 00:00:00.000000 bolero_process-0.0.8/datasets/Li2023Science-HumanBrain/fragment_urls.txt
--rwxr-xr-x   0        0        0     9118 2020-02-02 00:00:00.000000 bolero_process-0.0.8/datasets/Zhang2021Cell-HumanTissue/fragment_urls.txt
--rw-r--r--   0        0        0    29354 2020-02-02 00:00:00.000000 bolero_process-0.0.8/datasets/Zu2023Nature-WMB/fragment_urls.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bolero_process-0.0.8/docs/Makefile
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 bolero_process-0.0.8/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bolero_process-0.0.8/docs/changelog.md
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 bolero_process-0.0.8/docs/conf.py
--rw-r--r--   0        0        0     7075 2020-02-02 00:00:00.000000 bolero_process-0.0.8/docs/contributing.md
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bolero_process-0.0.8/docs/index.md
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 bolero_process-0.0.8/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 bolero_process-0.0.8/docs/references.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bolero_process-0.0.8/docs/_static/.gitkeep
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 bolero_process-0.0.8/docs/_static/css/custom.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bolero_process-0.0.8/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 bolero_process-0.0.8/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 bolero_process-0.0.8/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 bolero_process-0.0.8/docs/notebooks/example.ipynb
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 bolero_process-0.0.8/envs/setup_vm.sh
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 bolero_process-0.0.8/envs/sky-gpu.yaml
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 bolero_process-0.0.8/envs/sky-jupyter-large-spot.yaml
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 bolero_process-0.0.8/envs/sky-jupyter-large.yaml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bolero_process-0.0.8/envs/sky-jupyter-spot.yaml
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 bolero_process-0.0.8/envs/sky-jupyter.yaml
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 bolero_process-0.0.8/envs/sky-mapping-large-spot.yaml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 bolero_process-0.0.8/src/bolero_process/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bolero_process-0.0.8/src/bolero_process/atac/__init__.py
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 bolero_process-0.0.8/src/bolero_process/atac/bulk/Snakefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bolero_process-0.0.8/src/bolero_process/atac/bulk/__init__.py
--rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 bolero_process-0.0.8/src/bolero_process/atac/bulk/bulk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bolero_process-0.0.8/src/bolero_process/atac/sc/__init__.py
--rw-r--r--   0        0        0    13818 2020-02-02 00:00:00.000000 bolero_process-0.0.8/src/bolero_process/atac/sc/fragments_to_zarr.py
--rw-r--r--   0        0        0     8711 2020-02-02 00:00:00.000000 bolero_process-0.0.8/src/bolero_process/atac/sc/zarr_io.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 bolero_process-0.0.8/tests/test_basic.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 bolero_process-0.0.8/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 bolero_process-0.0.8/LICENSE
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 bolero_process-0.0.8/README.md
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 bolero_process-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 bolero_process-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 bolero_process-0.0.9/.codecov.yaml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bolero_process-0.0.9/.cruft.json
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 bolero_process-0.0.9/.editorconfig
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 bolero_process-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 bolero_process-0.0.9/.readthedocs.yaml
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 bolero_process-0.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 bolero_process-0.0.9/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 bolero_process-0.0.9/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 bolero_process-0.0.9/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 bolero_process-0.0.9/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 bolero_process-0.0.9/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 bolero_process-0.0.9/.github/workflows/test.yaml
+-rwxr-xr-x   0        0        0     7290 2020-02-02 00:00:00.000000 bolero_process-0.0.9/datasets/Li2023Science-HumanBrain/fragment_urls.txt
+-rwxr-xr-x   0        0        0     9118 2020-02-02 00:00:00.000000 bolero_process-0.0.9/datasets/Zhang2021Cell-HumanTissue/fragment_urls.txt
+-rw-r--r--   0        0        0    29354 2020-02-02 00:00:00.000000 bolero_process-0.0.9/datasets/Zu2023Nature-WMB/fragment_urls.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bolero_process-0.0.9/docs/Makefile
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 bolero_process-0.0.9/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bolero_process-0.0.9/docs/changelog.md
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 bolero_process-0.0.9/docs/conf.py
+-rw-r--r--   0        0        0     7075 2020-02-02 00:00:00.000000 bolero_process-0.0.9/docs/contributing.md
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bolero_process-0.0.9/docs/index.md
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 bolero_process-0.0.9/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 bolero_process-0.0.9/docs/references.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bolero_process-0.0.9/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 bolero_process-0.0.9/docs/_static/css/custom.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bolero_process-0.0.9/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 bolero_process-0.0.9/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 bolero_process-0.0.9/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 bolero_process-0.0.9/docs/notebooks/example.ipynb
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 bolero_process-0.0.9/envs/setup_vm.sh
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 bolero_process-0.0.9/envs/sky-gpu.yaml
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 bolero_process-0.0.9/envs/sky-jupyter-large-spot.yaml
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 bolero_process-0.0.9/envs/sky-jupyter-large.yaml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bolero_process-0.0.9/envs/sky-jupyter-spot.yaml
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 bolero_process-0.0.9/envs/sky-jupyter.yaml
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 bolero_process-0.0.9/envs/sky-mapping-large-spot.yaml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 bolero_process-0.0.9/src/bolero_process/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bolero_process-0.0.9/src/bolero_process/atac/__init__.py
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 bolero_process-0.0.9/src/bolero_process/atac/bulk/Snakefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bolero_process-0.0.9/src/bolero_process/atac/bulk/__init__.py
+-rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 bolero_process-0.0.9/src/bolero_process/atac/bulk/bulk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bolero_process-0.0.9/src/bolero_process/atac/sc/__init__.py
+-rw-r--r--   0        0        0    13838 2020-02-02 00:00:00.000000 bolero_process-0.0.9/src/bolero_process/atac/sc/fragments_to_zarr.py
+-rw-r--r--   0        0        0     8711 2020-02-02 00:00:00.000000 bolero_process-0.0.9/src/bolero_process/atac/sc/zarr_io.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 bolero_process-0.0.9/tests/test_basic.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 bolero_process-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 bolero_process-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 bolero_process-0.0.9/README.md
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 bolero_process-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 bolero_process-0.0.9/PKG-INFO
```

### Comparing `bolero_process-0.0.8/.cruft.json` & `bolero_process-0.0.9/.cruft.json`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/.pre-commit-config.yaml` & `bolero_process-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/.github/ISSUE_TEMPLATE/bug_report.yml` & `bolero_process-0.0.9/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/.github/workflows/build.yaml` & `bolero_process-0.0.9/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/.github/workflows/release.yaml` & `bolero_process-0.0.9/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/.github/workflows/test.yaml` & `bolero_process-0.0.9/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/datasets/Li2023Science-HumanBrain/fragment_urls.txt` & `bolero_process-0.0.9/datasets/Li2023Science-HumanBrain/fragment_urls.txt`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/datasets/Zhang2021Cell-HumanTissue/fragment_urls.txt` & `bolero_process-0.0.9/datasets/Zhang2021Cell-HumanTissue/fragment_urls.txt`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/datasets/Zu2023Nature-WMB/fragment_urls.txt` & `bolero_process-0.0.9/datasets/Zu2023Nature-WMB/fragment_urls.txt`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/docs/Makefile` & `bolero_process-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/docs/conf.py` & `bolero_process-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/docs/contributing.md` & `bolero_process-0.0.9/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/docs/references.bib` & `bolero_process-0.0.9/docs/references.bib`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/docs/_templates/autosummary/class.rst` & `bolero_process-0.0.9/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/docs/extensions/typed_returns.py` & `bolero_process-0.0.9/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/docs/notebooks/example.ipynb` & `bolero_process-0.0.9/docs/notebooks/example.ipynb`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/envs/setup_vm.sh` & `bolero_process-0.0.9/envs/setup_vm.sh`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/envs/sky-gpu.yaml` & `bolero_process-0.0.9/envs/sky-gpu.yaml`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/envs/sky-jupyter-large-spot.yaml` & `bolero_process-0.0.9/envs/sky-jupyter-large-spot.yaml`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/envs/sky-jupyter-large.yaml` & `bolero_process-0.0.9/envs/sky-jupyter-large.yaml`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/envs/sky-jupyter-spot.yaml` & `bolero_process-0.0.9/envs/sky-jupyter-spot.yaml`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/envs/sky-jupyter.yaml` & `bolero_process-0.0.9/envs/sky-jupyter.yaml`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/envs/sky-mapping-large-spot.yaml` & `bolero_process-0.0.9/envs/sky-mapping-large-spot.yaml`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/src/bolero_process/atac/bulk/Snakefile` & `bolero_process-0.0.9/src/bolero_process/atac/bulk/Snakefile`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/src/bolero_process/atac/bulk/bulk.py` & `bolero_process-0.0.9/src/bolero_process/atac/bulk/bulk.py`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/src/bolero_process/atac/sc/fragments_to_zarr.py` & `bolero_process-0.0.9/src/bolero_process/atac/sc/fragments_to_zarr.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 def _sort_fragments_by_barcode(path):
     # Generate a random string of length 10
     random_string = "".join(random.choices(string.ascii_letters + string.digits, k=10))
     temp_dir = "/tmp"
 
     unzip_cmd = f"gunzip -c {path} > {temp_dir}/{random_string}.tsv"
     sort_cmd = (
-        f"sort --parallel 2 -k4,4 {temp_dir}/{random_string}.tsv "
+        f"sort -S 4G -T {temp_dir} --parallel 2 -k4,4 {temp_dir}/{random_string}.tsv "
         f"> {temp_dir}/{random_string}.sort.tsv "
         f"&& rm -f {temp_dir}/{random_string}.tsv"
     )
     gzip_cmd = f"gzip {temp_dir}/{random_string}.sort.tsv"
 
     subprocess.check_call(unzip_cmd, shell=True)
     subprocess.check_call(sort_cmd, shell=True)
```

### Comparing `bolero_process-0.0.8/src/bolero_process/atac/sc/zarr_io.py` & `bolero_process-0.0.9/src/bolero_process/atac/sc/zarr_io.py`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/LICENSE` & `bolero_process-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/README.md` & `bolero_process-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/pyproject.toml` & `bolero_process-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bolero_process-0.0.8/PKG-INFO` & `bolero_process-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bolero-process
-Version: 0.0.8
+Version: 0.0.9
 Summary: Data preprocessing for bolero package
 Project-URL: Documentation, https://bolero-process.readthedocs.io/
 Project-URL: Source, https://github.com/lhqing/bolero-process
 Project-URL: Home-page, https://github.com/lhqing/bolero-process
 Author: Hanqing Liu
 Maintainer-email: Hanqing Liu <hanqingliu@fas.harvard.edu>
 License: MIT License
```


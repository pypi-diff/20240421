# Comparing `tmp/tarandm_analytics-0.0.9.tar.gz` & `tmp/tarandm_analytics-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarandm_analytics-0.0.9.tar", max compression
+gzip compressed data, was "tarandm_analytics-0.1.1.tar", max compression
```

## Comparing `tarandm_analytics-0.0.9.tar` & `tarandm_analytics-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0      980 2023-07-13 15:47:19.469697 tarandm_analytics-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     6370 2023-06-29 09:18:17.981136 tarandm_analytics-0.0.9/README.md
--rw-r--r--   0        0        0       23 2023-07-13 15:47:19.463079 tarandm_analytics-0.0.9/tarandm_analytics/__init__.py
--rw-r--r--   0        0        0      911 2023-07-05 14:43:36.988316 tarandm_analytics-0.0.9/tarandm_analytics/base_class.py
--rw-r--r--   0        0        0        0 2023-07-03 15:26:41.279844 tarandm_analytics-0.0.9/tarandm_analytics/export_predictive_model/__init__.py
--rw-r--r--   0        0        0      207 2023-07-04 06:21:18.742105 tarandm_analytics-0.0.9/tarandm_analytics/export_predictive_model/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    26102 2023-07-09 09:25:00.464160 tarandm_analytics-0.0.9/tarandm_analytics/export_predictive_model/__pycache__/create_predictive_model.cpython-310.pyc
--rw-r--r--   0        0        0     4053 2023-07-09 09:25:00.865805 tarandm_analytics-0.0.9/tarandm_analytics/export_predictive_model/__pycache__/model_visualization.cpython-310.pyc
--rw-r--r--   0        0        0    38307 2023-07-13 15:47:19.450919 tarandm_analytics-0.0.9/tarandm_analytics/export_predictive_model/create_predictive_model.py
--rw-r--r--   0        0        0     4728 2023-07-08 18:58:26.203186 tarandm_analytics-0.0.9/tarandm_analytics/export_predictive_model/model_visualization.py
--rw-r--r--   0        0        0      342 2023-07-06 11:25:46.354702 tarandm_analytics-0.0.9/tarandm_analytics/utils.py
--rw-r--r--   0        0        0     6882 1970-01-01 00:00:00.000000 tarandm_analytics-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1156 2024-04-21 13:01:41.064138 tarandm_analytics-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6370 2023-06-29 09:18:17.981136 tarandm_analytics-0.1.1/README.md
+-rw-r--r--   0        0        0       23 2024-04-21 13:01:41.065138 tarandm_analytics-0.1.1/tarandm_analytics/__init__.py
+-rw-r--r--   0        0        0     7255 2023-08-09 07:42:22.869869 tarandm_analytics-0.1.1/tarandm_analytics/attribute_evaluator/.ipynb_checkpoints/evaluate_attributes-checkpoint.py
+-rw-r--r--   0        0        0        0 2023-08-05 16:30:40.047983 tarandm_analytics-0.1.1/tarandm_analytics/attribute_evaluator/__init__.py
+-rw-r--r--   0        0        0     8617 2024-04-12 16:54:37.332921 tarandm_analytics-0.1.1/tarandm_analytics/attribute_evaluator/evaluate_attributes.py
+-rw-r--r--   0        0        0     1264 2023-12-13 08:09:32.412051 tarandm_analytics-0.1.1/tarandm_analytics/base_class.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:26:41.279844 tarandm_analytics-0.1.1/tarandm_analytics/export_predictive_model/__init__.py
+-rw-r--r--   0        0        0    73718 2024-04-21 13:01:41.067139 tarandm_analytics-0.1.1/tarandm_analytics/export_predictive_model/create_predictive_model.py
+-rw-r--r--   0        0        0     4836 2023-12-13 08:09:32.415094 tarandm_analytics-0.1.1/tarandm_analytics/export_predictive_model/model_visualization.py
+-rw-r--r--   0        0        0        0 2024-01-09 18:26:05.741943 tarandm_analytics-0.1.1/tarandm_analytics/plots/__init__.py
+-rw-r--r--   0        0        0     3624 2024-04-12 16:54:37.335945 tarandm_analytics-0.1.1/tarandm_analytics/plots/plot_functions.py
+-rw-r--r--   0        0        0      350 2023-12-13 08:09:32.417149 tarandm_analytics-0.1.1/tarandm_analytics/utils.py
+-rw-r--r--   0        0        0     7066 1970-01-01 00:00:00.000000 tarandm_analytics-0.1.1/PKG-INFO
```

### Comparing `tarandm_analytics-0.0.9/pyproject.toml` & `tarandm_analytics-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 [tool.poetry]
 name = "tarandm_analytics"
-version = "0.0.9"
-description = "Package links analytics in Pytjon with TaranDM software."
+version = "0.1.1"
+description = "Package links analytics in Python with TaranDM software."
 authors = ["Marek Teller <mteller@taran.ai>"]
 readme = "README.md"
 packages = [
     { include = "tarandm_analytics" }
 ]
 
 [tool.poetry.dependencies]
-python = "~3.10"
+python = ">=3.9"
 pandas = {version = "*", source = "pypi"}
-scikit-learn = {version = "1.2.2", source = "pypi"}
+scikit-learn = {version = "*", source = "pypi"}
 requests = {version = "*", source = "pypi"}
 llvmlite = {version = "*", source = "pypi"}
-numba = {version = "==0.56.4", source = "pypi"}
+numba = {version = "*", source = "pypi"}
 shap = {version = "*", source = "pypi"}
 matplotlib = {version = "*", source = "pypi"}
 path = {version = "*", source = "pypi"}
 xgboost = {version = "*", source = "pypi"}
 structlog = {version="*", source = "pypi"}
+importlib = {version="*", source = "pypi"}
+pydantic = {version="*", source = "pypi"}
+sklearn2pmml = {version="*", source = "pypi"}
+sklearn_pmml_model = {version="*", source = "pypi"}
 
 [tool.poetry.dev-dependencies]
-python = "~3.10"
+python = ">=3.9"
 typing = {version = "*", source = "pypi"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
```

### Comparing `tarandm_analytics-0.0.9/README.md` & `tarandm_analytics-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tarandm_analytics-0.0.9/tarandm_analytics/export_predictive_model/model_visualization.py` & `tarandm_analytics-0.1.1/tarandm_analytics/export_predictive_model/model_visualization.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from io import BytesIO
-from typing import List, Optional, Dict
+from typing import Optional, Dict, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    import pandas as pd
+    from xgboost import Booster
+    from sklearn.linear_model import LogisticRegression
+    from sklearn.ensemble import RandomForestClassifier
 
-import pandas as pd
 import structlog
-from sklearn.ensemble import RandomForestClassifier
-from sklearn.linear_model import LogisticRegression
-from xgboost import Booster
 
 
 logger = structlog.get_logger(__name__)
 
 
-def shap_summary_plot_logistic_regression(
-    model: LogisticRegression, data: "pd.DataFrame", attributes: List[str]
-) -> BytesIO:
+def shap_summary_plot_logistic_regression(model: "LogisticRegression", data: "pd.DataFrame") -> BytesIO:
     import shap
     import matplotlib.pyplot as plt
 
+    attributes = model.feature_names_in_
     masker = shap.maskers.Independent(data=data[attributes])
     explainer = shap.LinearExplainer(model, masker=masker)
     shap_values = explainer.shap_values(data[attributes])
 
     shap.summary_plot(
         shap_values,
         data[attributes],
@@ -39,48 +40,49 @@
     image_stream = BytesIO()
     plt.savefig(image_stream, format="svg", bbox_inches="tight")
     plt.close()
 
     return image_stream
 
 
-def shap_summary_plot_xgboost(model: Booster, data: "pd.DataFrame", attributes: List[str]) -> BytesIO:
+def shap_summary_plot_xgboost(model: "Booster", data: "pd.DataFrame") -> BytesIO:
     import shap
     import matplotlib.pyplot as plt
 
+    attributes = model.feature_names
     explainer = shap.TreeExplainer(model)
     shap_values = explainer.shap_values(data[attributes])
-    shap.summary_plot(shap_values, data[attributes], max_display=15, show=False)
+    shap.summary_plot(shap_values, data[attributes], max_display=20, show=False)
 
     ax = plt.gca()
     if ax.get_legend():
         ax.get_legend().remove()
 
     image_stream = BytesIO()
     plt.savefig(image_stream, format="svg", bbox_inches="tight")
     plt.close()
 
     return image_stream
 
 
-def learning_curves_plot(model: Booster, evaluations_result: Dict, metric: Optional[str] = None) -> BytesIO:
+def learning_curves_plot(model: "Booster", evaluations_result: Dict, metric: Optional[str] = None) -> BytesIO:
     import matplotlib.pyplot as plt
 
     if metric is None:
         metric_final = list(evaluations_result[list(evaluations_result.keys())[0]].keys())[0]
         logger.info(
-            f"Learning curves plot: Metric to plot was not provided. Automatically assigned metric '{metric_final}'."
+            f"Learning curves plot: Metric to be plotted was not provided. Automatically assigned metric '{metric_final}'."
         )
     # elif metric not in evaluations_result
     else:
         metric_final = metric
 
     total_iteration_count = len(evaluations_result[list(evaluations_result.keys())[0]][metric_final])
     best_score = getattr(model, "best_score", None)
-    best_iteration = getattr(model, "best_iteration", None) + 1
+    best_iteration = getattr(model, "best_iteration", None)
     taran_rgb = (10 / 255, 134 / 255, 132 / 255)
 
     ax = plt.subplot(1, 1, 1)
     for sample, vals in evaluations_result.items():
         ax.plot(range(1, total_iteration_count + 1), vals[metric_final], label=sample)
 
     if best_score:
@@ -88,19 +90,19 @@
             [1, total_iteration_count],
             [best_score, best_score],
             color="black",
             ls="--",
             lw=1,
         )
 
-        ax.scatter([best_iteration], [best_score], color="black")
+        ax.scatter([best_iteration + 1], [best_score], color="black")
         ax.annotate(
             "{:d}; {:0.3f}".format(best_iteration, best_score),
-            xy=(best_iteration, best_score),
-            xytext=(best_iteration, best_score + 0.005),
+            xy=(best_iteration + 1, best_score),
+            xytext=(best_iteration + 1, best_score + 0.005),
         )
 
     ax.set_xlabel("ITERATION", color="gray")
     ax.set_ylabel(metric_final.upper(), color="gray")
     ax.set_title(f"Model training - {metric_final} curves", color=taran_rgb)
 
     ax.spines["top"].set_visible(False)
@@ -115,23 +117,23 @@
     plt.savefig(image_stream, format="svg")
     plt.close()
 
     return image_stream
 
 
 def shap_summary_plot_random_forest(
-    model: RandomForestClassifier,
+    model: "RandomForestClassifier",
     data: "pd.DataFrame",
-    attributes: List[str],
     target_class: Optional[str],
 ) -> BytesIO:
     import shap
     import matplotlib.pyplot as plt
 
     class_index = [str(c) for c in model.classes_].index(target_class)
+    attributes = model.feature_names_in_
 
     explainer = shap.TreeExplainer(model)
     shap_values = explainer.shap_values(data[attributes])
 
     shap.summary_plot(
         [shap_values[class_index]],
         data[attributes],
```

### Comparing `tarandm_analytics-0.0.9/PKG-INFO` & `tarandm_analytics-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: tarandm-analytics
-Version: 0.0.9
-Summary: Package links analytics in Pytjon with TaranDM software.
+Version: 0.1.1
+Summary: Package links analytics in Python with TaranDM software.
 Author: Marek Teller
 Author-email: mteller@taran.ai
-Requires-Python: >=3.10,<3.11
+Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: importlib
 Requires-Dist: llvmlite
 Requires-Dist: matplotlib
-Requires-Dist: numba (==0.56.4)
+Requires-Dist: numba
 Requires-Dist: pandas
 Requires-Dist: path
+Requires-Dist: pydantic
 Requires-Dist: requests
-Requires-Dist: scikit-learn (==1.2.2)
+Requires-Dist: scikit-learn
 Requires-Dist: shap
+Requires-Dist: sklearn2pmml
+Requires-Dist: sklearn_pmml_model
 Requires-Dist: structlog
 Requires-Dist: xgboost
 Description-Content-Type: text/markdown
 
 # Predictive model support
```


# Comparing `tmp/bellek-0.94.0.tar.gz` & `tmp/bellek-0.94.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bellek-0.94.0.tar", last modified: Sat Apr 20 18:41:53 2024, max compression
+gzip compressed data, was "bellek-0.94.1.tar", last modified: Sun Apr 21 08:22:26 2024, max compression
```

## Comparing `bellek-0.94.0.tar` & `bellek-0.94.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.965558 bellek-0.94.0/
--rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.94.0/LICENSE
--rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.94.0/MANIFEST.in
--rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-20 18:41:53.965056 bellek-0.94.0/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)      184 2023-04-09 15:45:53.000000 bellek-0.94.0/README.md
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.903569 bellek-0.94.0/bellek/
--rw-r--r--   0 bdsaglam   (501) staff       (20)       23 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    54814 2024-04-20 18:41:50.000000 bellek-0.94.0/bellek/_modidx.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.911389 bellek-0.94.0/bellek/hf/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/hf/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.912232 bellek-0.94.0/bellek/hf/datasets/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/hf/datasets/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1193 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/hf/datasets/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.917043 bellek-0.94.0/bellek/hf/transformers/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/hf/transformers/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    12917 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/hf/transformers/experiment.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2039 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/hf/transformers/llama2.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      790 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/hf/transformers/llama3.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2934 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/hf/transformers/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.930143 bellek-0.94.0/bellek/jerx/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/jerx/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1314 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/jerx/dataset.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3386 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/jerx/eval.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.931264 bellek-0.94.0/bellek/jerx/fewshot/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/jerx/fewshot/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     5821 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/jerx/fewshot/llm.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     4110 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/jerx/prompt.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.932325 bellek-0.94.0/bellek/jerx/reward/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/jerx/reward/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2550 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/jerx/reward/gpt.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1186 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/jerx/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.939081 bellek-0.94.0/bellek/lang/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/lang/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1575 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/lang/dataset.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2160 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/lang/qdecomp.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.941066 bellek-0.94.0/bellek/langchain/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/langchain/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      915 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/langchain/cache.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1271 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/langchain/obs.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.947092 bellek-0.94.0/bellek/llama_index/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/llama_index/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.948434 bellek-0.94.0/bellek/llama_index/data_structs/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/llama_index/data_structs/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2483 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/llama_index/data_structs/data_structs.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.949828 bellek-0.94.0/bellek/llama_index/graph_stores/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/llama_index/graph_stores/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9059 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/llama_index/graph_stores/kuzu.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.950555 bellek-0.94.0/bellek/llama_index/indices/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/llama_index/indices/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.952418 bellek-0.94.0/bellek/llama_index/indices/knowledge_graph/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    13058 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    14785 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/llama_index/indices/knowledge_graph/retrievers.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      855 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/llama_index/llms.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1420 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/llama_index/obs.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      779 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/logging.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.961769 bellek-0.94.0/bellek/ml/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/ml/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/ml/clip.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     8515 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/ml/coop.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/ml/data.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/ml/evaluation.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3231 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/ml/experiment.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/ml/layer.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/ml/loss.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/ml/mcd.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/ml/vision.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.962810 bellek-0.94.0/bellek/musique/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/musique/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3081 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/musique/eval.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/testing.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.963858 bellek-0.94.0/bellek/text/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/text/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/text/utils.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     4864 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/utils.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      823 2024-04-20 18:41:49.000000 bellek-0.94.0/bellek/wandb.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 18:41:53.910741 bellek-0.94.0/bellek.egg-info/
--rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-20 18:41:53.000000 bellek-0.94.0/bellek.egg-info/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1748 2024-04-20 18:41:53.000000 bellek-0.94.0/bellek.egg-info/SOURCES.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2024-04-20 18:41:53.000000 bellek-0.94.0/bellek.egg-info/dependency_links.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)       34 2024-04-20 18:41:53.000000 bellek-0.94.0/bellek.egg-info/entry_points.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.94.0/bellek.egg-info/not-zip-safe
--rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-20 18:41:53.000000 bellek-0.94.0/bellek.egg-info/requires.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2024-04-20 18:41:53.000000 bellek-0.94.0/bellek.egg-info/top_level.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1316 2024-04-20 18:41:18.000000 bellek-0.94.0/settings.ini
--rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2024-04-20 18:41:53.965734 bellek-0.94.0/setup.cfg
--rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.94.0/setup.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.591615 bellek-0.94.1/
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.94.1/LICENSE
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.94.1/MANIFEST.in
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-21 08:22:26.591246 bellek-0.94.1/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      184 2023-04-09 15:45:53.000000 bellek-0.94.1/README.md
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.557722 bellek-0.94.1/bellek/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       23 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    54814 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/_modidx.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.562366 bellek-0.94.1/bellek/hf/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/hf/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.563713 bellek-0.94.1/bellek/hf/datasets/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/hf/datasets/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1193 2024-04-21 08:22:21.000000 bellek-0.94.1/bellek/hf/datasets/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.566782 bellek-0.94.1/bellek/hf/transformers/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/hf/transformers/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    12972 2024-04-21 08:22:21.000000 bellek-0.94.1/bellek/hf/transformers/experiment.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2039 2024-04-21 08:22:21.000000 bellek-0.94.1/bellek/hf/transformers/llama2.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      790 2024-04-21 08:22:21.000000 bellek-0.94.1/bellek/hf/transformers/llama3.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2934 2024-04-21 08:22:21.000000 bellek-0.94.1/bellek/hf/transformers/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.570509 bellek-0.94.1/bellek/jerx/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/jerx/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1314 2024-04-21 08:22:21.000000 bellek-0.94.1/bellek/jerx/dataset.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3386 2024-04-21 08:22:21.000000 bellek-0.94.1/bellek/jerx/eval.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.571362 bellek-0.94.1/bellek/jerx/fewshot/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/jerx/fewshot/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     5821 2024-04-21 08:22:21.000000 bellek-0.94.1/bellek/jerx/fewshot/llm.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     4110 2024-04-21 08:22:21.000000 bellek-0.94.1/bellek/jerx/prompt.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.572297 bellek-0.94.1/bellek/jerx/reward/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/jerx/reward/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2550 2024-04-21 08:22:21.000000 bellek-0.94.1/bellek/jerx/reward/gpt.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1186 2024-04-21 08:22:21.000000 bellek-0.94.1/bellek/jerx/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.573533 bellek-0.94.1/bellek/lang/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/lang/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1575 2024-04-21 08:22:21.000000 bellek-0.94.1/bellek/lang/dataset.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2160 2024-04-21 08:22:21.000000 bellek-0.94.1/bellek/lang/qdecomp.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.575212 bellek-0.94.1/bellek/langchain/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/langchain/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      915 2024-04-21 08:22:21.000000 bellek-0.94.1/bellek/langchain/cache.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1271 2024-04-21 08:22:21.000000 bellek-0.94.1/bellek/langchain/obs.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.576793 bellek-0.94.1/bellek/llama_index/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/llama_index/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.577633 bellek-0.94.1/bellek/llama_index/data_structs/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/llama_index/data_structs/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2483 2024-04-21 08:22:21.000000 bellek-0.94.1/bellek/llama_index/data_structs/data_structs.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.578950 bellek-0.94.1/bellek/llama_index/graph_stores/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/llama_index/graph_stores/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9059 2024-04-21 08:22:21.000000 bellek-0.94.1/bellek/llama_index/graph_stores/kuzu.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.579589 bellek-0.94.1/bellek/llama_index/indices/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/llama_index/indices/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.581180 bellek-0.94.1/bellek/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    13058 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    14785 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/llama_index/indices/knowledge_graph/retrievers.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      855 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/llama_index/llms.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1420 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/llama_index/obs.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      779 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/logging.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.588321 bellek-0.94.1/bellek/ml/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/ml/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/ml/clip.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     8515 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/ml/coop.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/ml/data.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/ml/evaluation.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3231 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/ml/experiment.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/ml/layer.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/ml/loss.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/ml/mcd.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/ml/vision.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.589442 bellek-0.94.1/bellek/musique/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/musique/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3081 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/musique/eval.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/testing.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.590458 bellek-0.94.1/bellek/text/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/text/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/text/utils.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     4864 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/utils.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      823 2024-04-21 08:22:22.000000 bellek-0.94.1/bellek/wandb.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:22:26.561866 bellek-0.94.1/bellek.egg-info/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-21 08:22:26.000000 bellek-0.94.1/bellek.egg-info/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1748 2024-04-21 08:22:26.000000 bellek-0.94.1/bellek.egg-info/SOURCES.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2024-04-21 08:22:26.000000 bellek-0.94.1/bellek.egg-info/dependency_links.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       34 2024-04-21 08:22:26.000000 bellek-0.94.1/bellek.egg-info/entry_points.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.94.1/bellek.egg-info/not-zip-safe
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-21 08:22:26.000000 bellek-0.94.1/bellek.egg-info/requires.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2024-04-21 08:22:26.000000 bellek-0.94.1/bellek.egg-info/top_level.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1316 2024-04-21 07:58:07.000000 bellek-0.94.1/settings.ini
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2024-04-21 08:22:26.591747 bellek-0.94.1/setup.cfg
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.94.1/setup.py
```

### Comparing `bellek-0.94.0/LICENSE` & `bellek-0.94.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/PKG-INFO` & `bellek-0.94.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellek
-Version: 0.94.0
+Version: 0.94.1
 Summary: My digital memory
 Home-page: https://github.com/bdsaglam/bellek
 Author: Barış Deniz Sağlam
 Author-email: bdsaglam@gmail.com
 License: Apache Software License 2.0
 Keywords: notebook
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bellek-0.94.0/bellek/_modidx.py` & `bellek-0.94.1/bellek/_modidx.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/hf/datasets/utils.py` & `bellek-0.94.1/bellek/hf/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/hf/transformers/experiment.py` & `bellek-0.94.1/bellek/hf/transformers/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
 def predict(
     pipe,
     dataset,
     *,
     output_parse_fn: Callable[[str], Any] | None = None,
     **generation_kwargs,
 ):
-    log.info(f"Running pipeline on dataset with {len(dataset)} samples...")
+    output_parse_fn = output_parse_fn or (lambda x: x)
 
     # Setup generation parameters
     generation_kwargs["return_full_text"] = False
 
     if "max_new_tokens" not in generation_kwargs:
         tokenized_outputs = dataset.map(lambda examples: pipe.tokenizer(examples["output"]), batched=True)
         token_counts = [len(input_ids) for input_ids in tokenized_outputs["input_ids"]]
@@ -269,14 +269,15 @@
         elif isinstance(terminator, str):
             eos_token_ids.add(pipe.tokenizer.convert_tokens_to_ids(terminator))
         else:
             raise ValueError(f"Invalid terminator token {terminator}.")
     generation_kwargs["eos_token_id"] = sorted(eos_token_ids)
 
     # Generate text
+    log.info(f"Running pipeline on dataset with {len(dataset)} samples...")
     generations = flat_pipeline(pipe)(dataset["input"], **generation_kwargs)
 
     # Parse outputs
     predictions = [output_parse_fn(text) for text in generations]
     references = [output_parse_fn(text) for text in dataset["output"]]
 
     # Create dataframe
```

### Comparing `bellek-0.94.0/bellek/hf/transformers/llama2.py` & `bellek-0.94.1/bellek/hf/transformers/llama2.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/hf/transformers/llama3.py` & `bellek-0.94.1/bellek/hf/transformers/llama3.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/hf/transformers/utils.py` & `bellek-0.94.1/bellek/hf/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/jerx/dataset.py` & `bellek-0.94.1/bellek/jerx/dataset.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/jerx/eval.py` & `bellek-0.94.1/bellek/jerx/eval.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/jerx/fewshot/llm.py` & `bellek-0.94.1/bellek/jerx/fewshot/llm.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/jerx/prompt.py` & `bellek-0.94.1/bellek/jerx/prompt.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/jerx/reward/gpt.py` & `bellek-0.94.1/bellek/jerx/reward/gpt.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/jerx/utils.py` & `bellek-0.94.1/bellek/jerx/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/lang/dataset.py` & `bellek-0.94.1/bellek/lang/dataset.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/lang/qdecomp.py` & `bellek-0.94.1/bellek/lang/qdecomp.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/langchain/cache.py` & `bellek-0.94.1/bellek/langchain/cache.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/langchain/obs.py` & `bellek-0.94.1/bellek/langchain/obs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/llama_index/data_structs/data_structs.py` & `bellek-0.94.1/bellek/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/llama_index/graph_stores/kuzu.py` & `bellek-0.94.1/bellek/llama_index/graph_stores/kuzu.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/llama_index/indices/knowledge_graph/base.py` & `bellek-0.94.1/bellek/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/llama_index/indices/knowledge_graph/retrievers.py` & `bellek-0.94.1/bellek/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/llama_index/llms.py` & `bellek-0.94.1/bellek/llama_index/llms.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/llama_index/obs.py` & `bellek-0.94.1/bellek/llama_index/obs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/logging.py` & `bellek-0.94.1/bellek/logging.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/ml/clip.py` & `bellek-0.94.1/bellek/ml/clip.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/ml/coop.py` & `bellek-0.94.1/bellek/ml/coop.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/ml/data.py` & `bellek-0.94.1/bellek/ml/data.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/ml/evaluation.py` & `bellek-0.94.1/bellek/ml/evaluation.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/ml/experiment.py` & `bellek-0.94.1/bellek/ml/experiment.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/ml/layer.py` & `bellek-0.94.1/bellek/ml/layer.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/ml/loss.py` & `bellek-0.94.1/bellek/ml/loss.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/ml/mcd.py` & `bellek-0.94.1/bellek/ml/mcd.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/ml/vision.py` & `bellek-0.94.1/bellek/ml/vision.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/musique/eval.py` & `bellek-0.94.1/bellek/musique/eval.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/testing.py` & `bellek-0.94.1/bellek/testing.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/utils.py` & `bellek-0.94.1/bellek/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek/wandb.py` & `bellek-0.94.1/bellek/wandb.py`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/bellek.egg-info/PKG-INFO` & `bellek-0.94.1/bellek.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellek
-Version: 0.94.0
+Version: 0.94.1
 Summary: My digital memory
 Home-page: https://github.com/bdsaglam/bellek
 Author: Barış Deniz Sağlam
 Author-email: bdsaglam@gmail.com
 License: Apache Software License 2.0
 Keywords: notebook
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bellek-0.94.0/bellek.egg-info/SOURCES.txt` & `bellek-0.94.1/bellek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bellek-0.94.0/settings.ini` & `bellek-0.94.1/settings.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = bellek
 lib_name = bellek
-version = 0.94.0
+version = 0.94.1
 min_python = 3.10
 license = apache2
 doc_path = _docs
 lib_path = bellek
 nbs_path = nbs
 recursive = True
 tst_flags = notest
```

### Comparing `bellek-0.94.0/setup.py` & `bellek-0.94.1/setup.py`

 * *Files identical despite different names*


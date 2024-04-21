# Comparing `tmp/bellek-0.95.0.tar.gz` & `tmp/bellek-0.96.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bellek-0.95.0.tar", last modified: Sun Apr 21 08:54:33 2024, max compression
+gzip compressed data, was "bellek-0.96.0.tar", last modified: Sun Apr 21 09:48:45 2024, max compression
```

## Comparing `bellek-0.95.0.tar` & `bellek-0.96.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.656526 bellek-0.95.0/
--rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.95.0/LICENSE
--rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.95.0/MANIFEST.in
--rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-21 08:54:33.655817 bellek-0.95.0/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)      184 2023-04-09 15:45:53.000000 bellek-0.95.0/README.md
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.621610 bellek-0.95.0/bellek/
--rw-r--r--   0 bdsaglam   (501) staff       (20)       23 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    54814 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/_modidx.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.627448 bellek-0.95.0/bellek/hf/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/hf/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.628390 bellek-0.95.0/bellek/hf/datasets/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/hf/datasets/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1193 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/hf/datasets/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.630613 bellek-0.95.0/bellek/hf/transformers/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/hf/transformers/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    12968 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/hf/transformers/experiment.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2039 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/hf/transformers/llama2.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      790 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/hf/transformers/llama3.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2934 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/hf/transformers/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.633636 bellek-0.95.0/bellek/jerx/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/jerx/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1314 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/jerx/dataset.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3386 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/jerx/eval.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.635711 bellek-0.95.0/bellek/jerx/fewshot/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/jerx/fewshot/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     5821 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/jerx/fewshot/llm.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     4110 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/jerx/prompt.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.637018 bellek-0.95.0/bellek/jerx/reward/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/jerx/reward/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2550 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/jerx/reward/gpt.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1186 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/jerx/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.638864 bellek-0.95.0/bellek/lang/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/lang/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1575 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/lang/dataset.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2160 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/lang/qdecomp.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.640467 bellek-0.95.0/bellek/langchain/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/langchain/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      915 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/langchain/cache.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1271 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/langchain/obs.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.642526 bellek-0.95.0/bellek/llama_index/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/llama_index/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.643716 bellek-0.95.0/bellek/llama_index/data_structs/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/llama_index/data_structs/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2483 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/llama_index/data_structs/data_structs.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.644637 bellek-0.95.0/bellek/llama_index/graph_stores/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/llama_index/graph_stores/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9059 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/llama_index/graph_stores/kuzu.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.645218 bellek-0.95.0/bellek/llama_index/indices/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/llama_index/indices/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.646649 bellek-0.95.0/bellek/llama_index/indices/knowledge_graph/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    13058 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    14785 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/llama_index/indices/knowledge_graph/retrievers.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      855 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/llama_index/llms.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1420 2024-04-21 08:54:29.000000 bellek-0.95.0/bellek/llama_index/obs.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      779 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/logging.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.653229 bellek-0.95.0/bellek/ml/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/ml/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/ml/clip.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     8515 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/ml/coop.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/ml/data.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/ml/evaluation.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3231 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/ml/experiment.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/ml/layer.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/ml/loss.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/ml/mcd.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/ml/vision.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.654179 bellek-0.95.0/bellek/musique/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/musique/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3081 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/musique/eval.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/testing.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.655103 bellek-0.95.0/bellek/text/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/text/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/text/utils.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     4864 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/utils.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      823 2024-04-21 08:54:30.000000 bellek-0.95.0/bellek/wandb.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 08:54:33.626813 bellek-0.95.0/bellek.egg-info/
--rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-21 08:54:33.000000 bellek-0.95.0/bellek.egg-info/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1748 2024-04-21 08:54:33.000000 bellek-0.95.0/bellek.egg-info/SOURCES.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2024-04-21 08:54:33.000000 bellek-0.95.0/bellek.egg-info/dependency_links.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)       34 2024-04-21 08:54:33.000000 bellek-0.95.0/bellek.egg-info/entry_points.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.95.0/bellek.egg-info/not-zip-safe
--rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-21 08:54:33.000000 bellek-0.95.0/bellek.egg-info/requires.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2024-04-21 08:54:33.000000 bellek-0.95.0/bellek.egg-info/top_level.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1316 2024-04-21 08:39:23.000000 bellek-0.95.0/settings.ini
--rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2024-04-21 08:54:33.656726 bellek-0.95.0/setup.cfg
--rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.95.0/setup.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.322674 bellek-0.96.0/
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.96.0/LICENSE
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.96.0/MANIFEST.in
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-21 09:48:45.322058 bellek-0.96.0/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      184 2023-04-09 15:45:53.000000 bellek-0.96.0/README.md
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.266313 bellek-0.96.0/bellek/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       23 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    54814 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/_modidx.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.275479 bellek-0.96.0/bellek/hf/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/hf/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.276653 bellek-0.96.0/bellek/hf/datasets/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/hf/datasets/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1193 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/hf/datasets/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.282507 bellek-0.96.0/bellek/hf/transformers/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/hf/transformers/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    12968 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/hf/transformers/experiment.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2039 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/hf/transformers/llama2.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      790 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/hf/transformers/llama3.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2934 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/hf/transformers/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.286715 bellek-0.96.0/bellek/jerx/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/jerx/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1314 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/jerx/dataset.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3386 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/jerx/eval.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.288404 bellek-0.96.0/bellek/jerx/fewshot/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/jerx/fewshot/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     6478 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/jerx/fewshot/llm.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     4110 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/jerx/prompt.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.290181 bellek-0.96.0/bellek/jerx/reward/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/jerx/reward/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2550 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/jerx/reward/gpt.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1186 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/jerx/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.293835 bellek-0.96.0/bellek/lang/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/lang/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1575 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/lang/dataset.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2160 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/lang/qdecomp.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.296900 bellek-0.96.0/bellek/langchain/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/langchain/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      915 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/langchain/cache.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1271 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/langchain/obs.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.300220 bellek-0.96.0/bellek/llama_index/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/llama_index/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.302106 bellek-0.96.0/bellek/llama_index/data_structs/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/llama_index/data_structs/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2483 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/llama_index/data_structs/data_structs.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.304128 bellek-0.96.0/bellek/llama_index/graph_stores/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/llama_index/graph_stores/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9059 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/llama_index/graph_stores/kuzu.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.305074 bellek-0.96.0/bellek/llama_index/indices/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/llama_index/indices/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.307131 bellek-0.96.0/bellek/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    13058 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    14785 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/llama_index/indices/knowledge_graph/retrievers.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      855 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/llama_index/llms.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1420 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/llama_index/obs.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      779 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/logging.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.316460 bellek-0.96.0/bellek/ml/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/ml/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/ml/clip.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     8515 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/ml/coop.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/ml/data.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/ml/evaluation.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3231 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/ml/experiment.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/ml/layer.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/ml/loss.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/ml/mcd.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/ml/vision.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.318439 bellek-0.96.0/bellek/musique/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/musique/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3081 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/musique/eval.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2024-04-21 09:48:38.000000 bellek-0.96.0/bellek/testing.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.320699 bellek-0.96.0/bellek/text/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/text/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/text/utils.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     4864 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/utils.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      823 2024-04-21 09:48:39.000000 bellek-0.96.0/bellek/wandb.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 09:48:45.273425 bellek-0.96.0/bellek.egg-info/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-21 09:48:44.000000 bellek-0.96.0/bellek.egg-info/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1748 2024-04-21 09:48:45.000000 bellek-0.96.0/bellek.egg-info/SOURCES.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2024-04-21 09:48:44.000000 bellek-0.96.0/bellek.egg-info/dependency_links.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       34 2024-04-21 09:48:44.000000 bellek-0.96.0/bellek.egg-info/entry_points.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.96.0/bellek.egg-info/not-zip-safe
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-21 09:48:44.000000 bellek-0.96.0/bellek.egg-info/requires.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2024-04-21 09:48:44.000000 bellek-0.96.0/bellek.egg-info/top_level.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1316 2024-04-21 09:48:24.000000 bellek-0.96.0/settings.ini
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2024-04-21 09:48:45.322843 bellek-0.96.0/setup.cfg
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.96.0/setup.py
```

### Comparing `bellek-0.95.0/LICENSE` & `bellek-0.96.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/PKG-INFO` & `bellek-0.96.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellek
-Version: 0.95.0
+Version: 0.96.0
 Summary: My digital memory
 Home-page: https://github.com/bdsaglam/bellek
 Author: Barış Deniz Sağlam
 Author-email: bdsaglam@gmail.com
 License: Apache Software License 2.0
 Keywords: notebook
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bellek-0.95.0/bellek/_modidx.py` & `bellek-0.96.0/bellek/_modidx.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/hf/datasets/utils.py` & `bellek-0.96.0/bellek/hf/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/hf/transformers/experiment.py` & `bellek-0.96.0/bellek/hf/transformers/experiment.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/hf/transformers/llama2.py` & `bellek-0.96.0/bellek/hf/transformers/llama2.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/hf/transformers/llama3.py` & `bellek-0.96.0/bellek/hf/transformers/llama3.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/hf/transformers/utils.py` & `bellek-0.96.0/bellek/hf/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/jerx/dataset.py` & `bellek-0.96.0/bellek/jerx/dataset.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/jerx/eval.py` & `bellek-0.96.0/bellek/jerx/eval.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/jerx/fewshot/llm.py` & `bellek-0.96.0/bellek/jerx/fewshot/llm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../../nbs/jerx.fewshot.llm.ipynb.
 
 # %% auto 0
-__all__ = ['log', 'DEFAULT_JERX_SYSTEM_MESSAGE_TEMPLATE', 'DEFAULT_JERX_USER_MESSAGE_TEMPLATE',
-           'DEFAULT_JERX_ASSISTANT_MESSAGE_TEMPLATE', 'DEFAULT_JERX_CHAT_TEMPLATE', 'make_kg_triplet_extract_fn']
+__all__ = ['log', 'DEFAULT_JERX_SYSTEM_MESSAGE_TEMPLATE', 'DEFAULT_JERX_CHAT_TEMPLATE', 'make_kg_triplet_extract_fn']
 
 # %% ../../../nbs/jerx.fewshot.llm.ipynb 3
 from llama_index.prompts import ChatPromptTemplate
 from llama_index.llms import ChatMessage, OpenAI, LLM
 from ..utils import parse_triplets
 from ...logging import get_logger
 
 log = get_logger(__name__)
 
 # %% ../../../nbs/jerx.fewshot.llm.ipynb 5
 DEFAULT_JERX_SYSTEM_MESSAGE_TEMPLATE = """
-Your task is to perform detailed entity-relation extraction from a document, creating a network of entities and their interrelations that enables answering complex, multi-hop questions. This requires careful analysis to identify and categorize entities (such as individuals, locations, organizations) and the specific, nuanced relationships between them.
-
-Extract up to {max_knowledge_triplets} entity-relation-entity triplets from the given text.
+You are an excellent joint entity-relation extraction algorithm. Your extract knowledge triplets in the form of (subject, relation, object) from user's messages. The goal is to create a network of entities and their interrelations that enables answering complex, multi-hop questions. This requires careful analysis to identify and categorize entities (such as individuals, locations, organizations) and the specific, nuanced relationships between them.
 
 # Guidelines
 The goal is to build a detailed and accurate map of entities and their interrelations, enabling a comprehensive understanding of the document's content and supporting the answering of detailed, multi-hop questions derived from or related to the document. Prepare to adapt your extraction techniques to the nuances and specifics presented by the document, recognizing the diversity in structures and styles across documents.
 
-# Core Objectives:
+# Core Objectives
 - **Comprehensive Entity and Relation Identification**: Systematically identify all relevant entities and their relationships within the document. Each entity and relation must be captured with precision, reflecting the document's depth of information.
 
 - **Entity Differentiation and Categorization**: Distinguish between different types of entities, avoiding the amalgamation of distinct entities into a single category. For instance, separate individuals from their professions or titles and define their relationship clearly.
 
 - **Clarification of Relationships and Avoidance of Redundancy**: Ensure each relationship is clearly defined, avoiding duplicate information. Relations should form a coherent, logical network, mapping connections between entities accurately, especially in hierarchical or geographic contexts.
 
 - **Inference of Implicit Relations**: Infer and articulate relations that are implied but not explicitly stated within the document. This nuanced understanding allows for a richer, more interconnected entity-relation map.
@@ -39,38 +36,51 @@
 
 # Formatting
 - Avoid stopwords.
 - Encode dates in the format: January 1, 1990
 - Employ the format: `entity1 | relation | entity2` for each extracted relation, ensuring clarity and precision in representation. Each triplet should be in a new line.
 """.strip()
 
-DEFAULT_JERX_USER_MESSAGE_TEMPLATE = """
+
+DEFAULT_JERX_CHAT_TEMPLATE = ChatPromptTemplate(
+    message_templates=[
+        ChatMessage(role="system", content=DEFAULT_JERX_SYSTEM_MESSAGE_TEMPLATE),
+        ChatMessage(
+            role="user",
+            content="""
 Glenhis Hernández (born 7 October 1990 in Havana) is a taekwondo practitioner from Cuba. She was the 2013 World
 Champion in middleweight.
 
 The current mayor of Havana ("President of the People's Power Provincial Assembly") is Marta Hernández Romero, she
 was elected on March 5, 2011.
-""".strip()
-
-DEFAULT_JERX_ASSISTANT_MESSAGE_TEMPLATE = """
+""".strip(),
+        ),
+        ChatMessage(
+            role="assistant",
+            content="""
 Glenhis Hernández (Athlete) | born on | October 7, 1990
-Glenhis Hernández (Athlete) | born in | Havana
+Glenhis Hernández (Athlete) | birth place | Havana
 Glenhis Hernández (Athlete) | specializes in | taekwondo
 Glenhis Hernández (Athlete) | won | 2013 World Champion title (Middleweight)
 Marta Hernández Romero (Politician) | serves as | mayor of Havana
 Marta Hernández Romero (Politician) | holds | the position of "President of the People's Power Provincial Assembly"
 Marta Hernández Romero (Politician) | elected on | March 5, 2011.
-""".strip()
-
-DEFAULT_JERX_CHAT_TEMPLATE = ChatPromptTemplate(
-    message_templates=[
-        ChatMessage(role='system', content=DEFAULT_JERX_SYSTEM_MESSAGE_TEMPLATE),
-        ChatMessage(role='user', content=DEFAULT_JERX_USER_MESSAGE_TEMPLATE),
-        ChatMessage(role='assistant', content=DEFAULT_JERX_ASSISTANT_MESSAGE_TEMPLATE),
-        ChatMessage(role='user', content="{text}"),
+""".strip(),
+        ),
+        ChatMessage(role="user", content="Alvinegro is the nickname of Agremiação Sportiva Arapiraquense."),
+        ChatMessage(role="assistant", content="Agremiação Sportiva Arapiraquense | nickname | Alvinegro"),
+        ChatMessage(
+            role="user",
+            content="Sausage is a main ingredient of Bacon Explosion but it also uses bacon. The icebreaker Aleksey Chirikov is 99.83 metres long. The country of Akron, Ohio, is United States, where Asian Americans are one of the ethnic groups.",
+        ),
+        ChatMessage(
+            role="assistant",
+            content="Bacon Explosion | ingredient | Bacon\nBacon Explosion | main ingredient | Sausage\nAleksey Chirikov (icebreaker) | length | 99.83\nUnited States | ethnic group | Asian Americans\nAkron, Ohio | country | United States",
+        ),
+        ChatMessage(role="user", content="{text}"),
     ]
 )
 
 # %% ../../../nbs/jerx.fewshot.llm.ipynb 6
 def make_kg_triplet_extract_fn(
     *,
     max_knowledge_triplets: int = 10,
```

### Comparing `bellek-0.95.0/bellek/jerx/prompt.py` & `bellek-0.96.0/bellek/jerx/prompt.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/jerx/reward/gpt.py` & `bellek-0.96.0/bellek/jerx/reward/gpt.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/jerx/utils.py` & `bellek-0.96.0/bellek/jerx/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/lang/dataset.py` & `bellek-0.96.0/bellek/lang/dataset.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/lang/qdecomp.py` & `bellek-0.96.0/bellek/lang/qdecomp.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/langchain/cache.py` & `bellek-0.96.0/bellek/langchain/cache.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/langchain/obs.py` & `bellek-0.96.0/bellek/langchain/obs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/llama_index/data_structs/data_structs.py` & `bellek-0.96.0/bellek/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/llama_index/graph_stores/kuzu.py` & `bellek-0.96.0/bellek/llama_index/graph_stores/kuzu.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/llama_index/indices/knowledge_graph/base.py` & `bellek-0.96.0/bellek/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/llama_index/indices/knowledge_graph/retrievers.py` & `bellek-0.96.0/bellek/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/llama_index/llms.py` & `bellek-0.96.0/bellek/llama_index/llms.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/llama_index/obs.py` & `bellek-0.96.0/bellek/llama_index/obs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/logging.py` & `bellek-0.96.0/bellek/logging.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/ml/clip.py` & `bellek-0.96.0/bellek/ml/clip.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/ml/coop.py` & `bellek-0.96.0/bellek/ml/coop.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/ml/data.py` & `bellek-0.96.0/bellek/ml/data.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/ml/evaluation.py` & `bellek-0.96.0/bellek/ml/evaluation.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/ml/experiment.py` & `bellek-0.96.0/bellek/ml/experiment.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/ml/layer.py` & `bellek-0.96.0/bellek/ml/layer.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/ml/loss.py` & `bellek-0.96.0/bellek/ml/loss.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/ml/mcd.py` & `bellek-0.96.0/bellek/ml/mcd.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/ml/vision.py` & `bellek-0.96.0/bellek/ml/vision.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/musique/eval.py` & `bellek-0.96.0/bellek/musique/eval.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/testing.py` & `bellek-0.96.0/bellek/testing.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/utils.py` & `bellek-0.96.0/bellek/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek/wandb.py` & `bellek-0.96.0/bellek/wandb.py`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/bellek.egg-info/PKG-INFO` & `bellek-0.96.0/bellek.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellek
-Version: 0.95.0
+Version: 0.96.0
 Summary: My digital memory
 Home-page: https://github.com/bdsaglam/bellek
 Author: Barış Deniz Sağlam
 Author-email: bdsaglam@gmail.com
 License: Apache Software License 2.0
 Keywords: notebook
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bellek-0.95.0/bellek.egg-info/SOURCES.txt` & `bellek-0.96.0/bellek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bellek-0.95.0/settings.ini` & `bellek-0.96.0/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = bellek
 lib_name = bellek
-version = 0.95.0
+version = 0.96.0
 min_python = 3.10
 license = apache2
 doc_path = _docs
 lib_path = bellek
 nbs_path = nbs
 recursive = True
 tst_flags = notest
```

### Comparing `bellek-0.95.0/setup.py` & `bellek-0.96.0/setup.py`

 * *Files identical despite different names*


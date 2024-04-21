# Comparing `tmp/deepllm-1.4.7.tar.gz` & `tmp/deepllm-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepllm-1.4.7.tar", last modified: Mon Apr  8 23:13:23 2024, max compression
+gzip compressed data, was "deepllm-1.5.0.tar", last modified: Sun Apr 21 00:13:20 2024, max compression
```

## Comparing `deepllm-1.4.7.tar` & `deepllm-1.5.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-08 23:13:23.929919 deepllm-1.4.7/
--rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-1.4.7/LICENSE
--rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-04-08 23:13:23.929415 deepllm-1.4.7/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     4366 2023-07-18 14:36:48.000000 deepllm-1.4.7/README.md
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-08 23:13:23.906865 deepllm-1.4.7/deepllm/
--rw-r--r--   0 tarau      (503) staff       (20)       22 2024-04-08 22:23:55.000000 deepllm-1.4.7/deepllm/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     2188 2024-03-22 05:04:24.000000 deepllm-1.4.7/deepllm/api.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-08 23:13:23.913019 deepllm-1.4.7/deepllm/apps/
--rw-r--r--   0 tarau      (503) staff       (20)       51 2023-07-08 16:25:29.000000 deepllm-1.4.7/deepllm/apps/README.md
--rw-r--r--   0 tarau      (503) staff       (20)     3615 2024-03-25 00:43:56.000000 deepllm-1.4.7/deepllm/apps/app.py
--rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-08-09 18:23:15.000000 deepllm-1.4.7/deepllm/apps/app.sh
--rwxr-xr-x   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.4.7/deepllm/apps/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)    11175 2024-03-25 01:01:26.000000 deepllm-1.4.7/deepllm/apps/rel_graph.html
--rw-r--r--   0 tarau      (503) staff       (20)       18 2024-03-16 22:29:32.000000 deepllm-1.4.7/deepllm/apps/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)      663 2024-01-01 16:38:49.000000 deepllm-1.4.7/deepllm/configurator.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-08 23:13:23.916043 deepllm-1.4.7/deepllm/demos/
--rw-r--r--   0 tarau      (503) staff       (20)       98 2023-07-10 19:44:29.000000 deepllm-1.4.7/deepllm/demos/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.4.7/deepllm/demos/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     2151 2024-02-25 03:35:53.000000 deepllm-1.4.7/deepllm/demos/demo.py
--rwxr-xr-x   0 tarau      (503) staff       (20)       75 2024-01-02 02:47:22.000000 deepllm-1.4.7/deepllm/demos/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)       44 2024-01-02 02:54:03.000000 deepllm-1.4.7/deepllm/demos/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)     1951 2023-10-04 22:28:27.000000 deepllm-1.4.7/deepllm/demos/viz.py
--rw-r--r--   0 tarau      (503) staff       (20)     3825 2023-10-13 02:28:54.000000 deepllm-1.4.7/deepllm/horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)    10875 2024-03-04 01:12:04.000000 deepllm-1.4.7/deepllm/interactors.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-08 23:13:23.920099 deepllm-1.4.7/deepllm/local_llms/
--rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-1.4.7/deepllm/local_llms/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.4.7/deepllm/local_llms/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.4.7/deepllm/local_llms/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-1.4.7/deepllm/local_llms/local_runs.py
--rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-1.4.7/deepllm/local_llms/requirements.txt
--rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-1.4.7/deepllm/local_llms/server.sh
--rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-08-12 16:50:59.000000 deepllm-1.4.7/deepllm/local_llms/test_vicuna.py
--rw-r--r--   0 tarau      (503) staff       (20)     3708 2024-03-24 18:59:54.000000 deepllm-1.4.7/deepllm/params.py
--rw-r--r--   0 tarau      (503) staff       (20)     9716 2024-04-07 21:18:58.000000 deepllm-1.4.7/deepllm/prompters.py
--rw-r--r--   0 tarau      (503) staff       (20)     4061 2024-02-26 23:53:37.000000 deepllm-1.4.7/deepllm/questmaker.py
--rw-r--r--   0 tarau      (503) staff       (20)    10784 2024-03-25 00:48:51.000000 deepllm-1.4.7/deepllm/recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     6758 2024-04-07 20:07:59.000000 deepllm-1.4.7/deepllm/refiners.py
--rw-r--r--   0 tarau      (503) staff       (20)       59 2024-03-22 20:57:32.000000 deepllm-1.4.7/deepllm/requirements.txt
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-08 23:13:23.928422 deepllm-1.4.7/deepllm/tests/
--rw-r--r--   0 tarau      (503) staff       (20)      126 2023-07-08 20:37:56.000000 deepllm-1.4.7/deepllm/tests/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-1.4.7/deepllm/tests/__init__.py
--rwxr-xr-x   0 tarau      (503) staff       (20)      596 2024-03-15 13:54:55.000000 deepllm-1.4.7/deepllm/tests/test_all.py
--rw-r--r--   0 tarau      (503) staff       (20)      906 2023-08-13 18:57:17.000000 deepllm-1.4.7/deepllm/tests/test_api.py
--rw-r--r--   0 tarau      (503) staff       (20)      381 2023-07-15 20:32:09.000000 deepllm-1.4.7/deepllm/tests/test_configurator.py
--rw-r--r--   0 tarau      (503) staff       (20)      526 2024-03-16 00:51:59.000000 deepllm-1.4.7/deepllm/tests/test_embedders.py
--rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-1.4.7/deepllm/tests/test_horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)      499 2023-07-19 14:10:18.000000 deepllm-1.4.7/deepllm/tests/test_interactors.py
--rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-1.4.7/deepllm/tests/test_params.py
--rw-r--r--   0 tarau      (503) staff       (20)     1216 2024-01-29 22:45:46.000000 deepllm-1.4.7/deepllm/tests/test_recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     2284 2023-07-08 20:38:27.000000 deepllm-1.4.7/deepllm/tests/test_refiners.py
--rw-r--r--   0 tarau      (503) staff       (20)     1287 2023-12-28 01:58:47.000000 deepllm-1.4.7/deepllm/tools.py
--rw-r--r--   0 tarau      (503) staff       (20)      882 2024-03-22 20:43:06.000000 deepllm-1.4.7/deepllm/vis.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-08 23:13:23.909058 deepllm-1.4.7/deepllm.egg-info/
--rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-04-08 23:13:23.000000 deepllm-1.4.7/deepllm.egg-info/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     1319 2024-04-08 23:13:23.000000 deepllm-1.4.7/deepllm.egg-info/SOURCES.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-08 23:13:23.000000 deepllm-1.4.7/deepllm.egg-info/dependency_links.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-08 23:13:23.000000 deepllm-1.4.7/deepllm.egg-info/not-zip-safe
--rw-r--r--   0 tarau      (503) staff       (20)       59 2024-04-08 23:13:23.000000 deepllm-1.4.7/deepllm.egg-info/requires.txt
--rw-r--r--   0 tarau      (503) staff       (20)        8 2024-04-08 23:13:23.000000 deepllm-1.4.7/deepllm.egg-info/top_level.txt
--rw-r--r--   0 tarau      (503) staff       (20)       38 2024-04-08 23:13:23.930115 deepllm-1.4.7/setup.cfg
--rw-r--r--   0 tarau      (503) staff       (20)      967 2023-11-08 02:45:22.000000 deepllm-1.4.7/setup.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-21 00:13:20.575532 deepllm-1.5.0/
+-rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-1.5.0/LICENSE
+-rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-04-21 00:13:20.575225 deepllm-1.5.0/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     4366 2023-07-18 14:36:48.000000 deepllm-1.5.0/README.md
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-21 00:13:20.553520 deepllm-1.5.0/deepllm/
+-rw-r--r--   0 tarau      (503) staff       (20)       22 2024-04-20 15:13:25.000000 deepllm-1.5.0/deepllm/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2188 2024-03-22 05:04:24.000000 deepllm-1.5.0/deepllm/api.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-21 00:13:20.560501 deepllm-1.5.0/deepllm/apps/
+-rw-r--r--   0 tarau      (503) staff       (20)       51 2023-07-08 16:25:29.000000 deepllm-1.5.0/deepllm/apps/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)     3615 2024-03-25 00:43:56.000000 deepllm-1.5.0/deepllm/apps/app.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-08-09 18:23:15.000000 deepllm-1.5.0/deepllm/apps/app.sh
+-rwxr-xr-x   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.5.0/deepllm/apps/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)   295587 2024-04-20 16:17:38.000000 deepllm-1.5.0/deepllm/apps/rel_graph.html
+-rw-r--r--   0 tarau      (503) staff       (20)       18 2024-03-16 22:29:32.000000 deepllm-1.5.0/deepllm/apps/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)      663 2024-01-01 16:38:49.000000 deepllm-1.5.0/deepllm/configurator.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-21 00:13:20.563022 deepllm-1.5.0/deepllm/demos/
+-rw-r--r--   0 tarau      (503) staff       (20)       98 2023-07-10 19:44:29.000000 deepllm-1.5.0/deepllm/demos/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.5.0/deepllm/demos/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2151 2024-02-25 03:35:53.000000 deepllm-1.5.0/deepllm/demos/demo.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)       75 2024-01-02 02:47:22.000000 deepllm-1.5.0/deepllm/demos/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       44 2024-01-02 02:54:03.000000 deepllm-1.5.0/deepllm/demos/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)     1951 2023-10-04 22:28:27.000000 deepllm-1.5.0/deepllm/demos/viz.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3825 2023-10-13 02:28:54.000000 deepllm-1.5.0/deepllm/horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)    11151 2024-04-20 21:22:06.000000 deepllm-1.5.0/deepllm/interactors.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-21 00:13:20.566918 deepllm-1.5.0/deepllm/local_llms/
+-rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-1.5.0/deepllm/local_llms/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.5.0/deepllm/local_llms/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.5.0/deepllm/local_llms/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-1.5.0/deepllm/local_llms/local_runs.py
+-rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-1.5.0/deepllm/local_llms/requirements.txt
+-rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-1.5.0/deepllm/local_llms/server.sh
+-rw-r--r--   0 tarau      (503) staff       (20)     1005 2024-04-20 00:01:10.000000 deepllm-1.5.0/deepllm/local_llms/test_llama3.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-08-12 16:50:59.000000 deepllm-1.5.0/deepllm/local_llms/test_vicuna.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3966 2024-04-20 23:33:01.000000 deepllm-1.5.0/deepllm/params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     9716 2024-04-07 21:18:58.000000 deepllm-1.5.0/deepllm/prompters.py
+-rw-r--r--   0 tarau      (503) staff       (20)     4061 2024-02-26 23:53:37.000000 deepllm-1.5.0/deepllm/questmaker.py
+-rw-r--r--   0 tarau      (503) staff       (20)    10784 2024-03-25 00:48:51.000000 deepllm-1.5.0/deepllm/recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     6758 2024-04-07 20:07:59.000000 deepllm-1.5.0/deepllm/refiners.py
+-rw-r--r--   0 tarau      (503) staff       (20)       59 2024-03-22 20:57:32.000000 deepllm-1.5.0/deepllm/requirements.txt
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-21 00:13:20.574500 deepllm-1.5.0/deepllm/tests/
+-rw-r--r--   0 tarau      (503) staff       (20)      126 2023-07-08 20:37:56.000000 deepllm-1.5.0/deepllm/tests/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-1.5.0/deepllm/tests/__init__.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)      596 2024-03-15 13:54:55.000000 deepllm-1.5.0/deepllm/tests/test_all.py
+-rw-r--r--   0 tarau      (503) staff       (20)      906 2023-08-13 18:57:17.000000 deepllm-1.5.0/deepllm/tests/test_api.py
+-rw-r--r--   0 tarau      (503) staff       (20)      381 2023-07-15 20:32:09.000000 deepllm-1.5.0/deepllm/tests/test_configurator.py
+-rw-r--r--   0 tarau      (503) staff       (20)      526 2024-03-16 00:51:59.000000 deepllm-1.5.0/deepllm/tests/test_embedders.py
+-rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-1.5.0/deepllm/tests/test_horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)      499 2023-07-19 14:10:18.000000 deepllm-1.5.0/deepllm/tests/test_interactors.py
+-rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-1.5.0/deepllm/tests/test_params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1216 2024-01-29 22:45:46.000000 deepllm-1.5.0/deepllm/tests/test_recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2284 2023-07-08 20:38:27.000000 deepllm-1.5.0/deepllm/tests/test_refiners.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1287 2023-12-28 01:58:47.000000 deepllm-1.5.0/deepllm/tools.py
+-rw-r--r--   0 tarau      (503) staff       (20)      882 2024-03-22 20:43:06.000000 deepllm-1.5.0/deepllm/vis.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-21 00:13:20.555923 deepllm-1.5.0/deepllm.egg-info/
+-rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-04-21 00:13:20.000000 deepllm-1.5.0/deepllm.egg-info/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     1353 2024-04-21 00:13:20.000000 deepllm-1.5.0/deepllm.egg-info/SOURCES.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-21 00:13:20.000000 deepllm-1.5.0/deepllm.egg-info/dependency_links.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-21 00:13:20.000000 deepllm-1.5.0/deepllm.egg-info/not-zip-safe
+-rw-r--r--   0 tarau      (503) staff       (20)       59 2024-04-21 00:13:20.000000 deepllm-1.5.0/deepllm.egg-info/requires.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        8 2024-04-21 00:13:20.000000 deepllm-1.5.0/deepllm.egg-info/top_level.txt
+-rw-r--r--   0 tarau      (503) staff       (20)       38 2024-04-21 00:13:20.575642 deepllm-1.5.0/setup.cfg
+-rw-r--r--   0 tarau      (503) staff       (20)      967 2023-11-08 02:45:22.000000 deepllm-1.5.0/setup.py
```

### Comparing `deepllm-1.4.7/LICENSE` & `deepllm-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/PKG-INFO` & `deepllm-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 1.4.7
+Version: 1.5.0
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: GPL-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deepllm-1.4.7/README.md` & `deepllm-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/api.py` & `deepllm-1.5.0/deepllm/api.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/apps/app.py` & `deepllm-1.5.0/deepllm/apps/app.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/configurator.py` & `deepllm-1.5.0/deepllm/configurator.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/demos/demo.py` & `deepllm-1.5.0/deepllm/demos/demo.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/demos/viz.py` & `deepllm-1.5.0/deepllm/demos/viz.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/horn_prover.py` & `deepllm-1.5.0/deepllm/horn_prover.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/interactors.py` & `deepllm-1.5.0/deepllm/interactors.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,32 @@
         return r.choices[i].message.content.strip()
 
     client = openai.OpenAI(
         api_key=ensure_openai_api_key(),
         base_url=CF.API_BASE
     )
 
-    r = client.chat.completions.create(
-        messages=mes,
-        model=model,
-        temperature=temperature,
-        n=n
-    )
+    extra_body = fix_eos()
+
+    if extra_body is not None:
+        r = client.chat.completions.create(
+            messages=mes,
+            model=model,
+            temperature=temperature,
+            n=n,
+            extra_body=extra_body
+        )
+    else:
+        r = client.chat.completions.create(
+            messages=mes,
+            model=model,
+            temperature=temperature,
+            n=n
+        )
+
     # print('!!!!>>> OPENAI RESULT:',r)
 
     results = r.choices
     pt = r.usage.prompt_tokens
     ct = r.usage.completion_tokens
 
     answers = [llm_res(r, i) for i in range(n)]
@@ -107,15 +119,15 @@
         self.cacher()
         self.tuner()
         self.talker()
         self.name = name
         self.CACHES = None
         self.TRACE = None
         self.initiator = None
-        PARAMS()(self) # overrides defaults from global params
+        PARAMS()(self)  # overrides defaults from global params
         # print('AGENT !!!!',self.__dict__)
 
     def tuner(self,
               model="gpt-3.5-turbo",
               temperature=0.2,
               n=1,
               max_toks=4000):
@@ -192,15 +204,15 @@
            avoids calling the API twice on the same quary that it retrives
            from its memory
            """
         self.short_mem = dict()
         self.long_mem = dict()
         self.prompt_toks = 0
         self.compl_toks = 0
-        self.processing_time=0
+        self.processing_time = 0
 
     def to_message(self, quest):
         """
         uses its past interaction in short-term memory
         as context to build the message to be sent to the API
         """
         mes = []
@@ -293,15 +305,15 @@
     def ask(self, *args, **kwargs):
         """
         asks the LLM via the API and returns a
         list of n answers (usually just n=1)
         while memoizing the prompt-answer pair and
         computing the token costs
         """
-        t1=time.time()
+        t1 = time.time()
         h = tuple(kwargs.items())
         if not h:
             assert len(args) == 1, ('BAD args', args)
             quest0 = args[0]
             assert isinstance(quest0, str)
         else:
             quest0 = h
@@ -324,23 +336,23 @@
                 answers, pt, ct = ask_llm(
                     model=self.model,
                     mes=mes,
                     temperature=self.temperature,
                     n=self.n
                 )
                 break
-            except Exception:
+            except Exception as ex:
                 if attempt >= max_attempts - 1:
-                          print('\n\n ***GPT exception:')
-                          print("LOCAL:",IS_LOCAL_LLM[0])
-                          print('API_BASE:', PARAMS().API_BASE)
-                          print('MODEL:',self.model)
+                    print('\n\n ***GPT exception:', ex)
+                    print("LOCAL:", IS_LOCAL_LLM[0])
+                    print('API_BASE:', PARAMS().API_BASE)
+                    print('MODEL:', self.model)
 
-                          #raise Exception('LLM exception')
-                          exit(1)
+                    # raise Exception('LLM exception')
+                    exit(1)
                 else:
                     print('retrying: ', attempt)
                     time.sleep(0.5)
 
         # def res(i):
         #    assert isinstance(i, int), i
         #    return r['choices'][i]['message']['content'].strip()
@@ -356,16 +368,16 @@
         self.prompt_toks += pt
         self.compl_toks += ct
 
         answer = self.post_process(quest0, answer)
 
         self.short_mem[quest] = answer
         assert isinstance(answer, str), answer
-        t2=time.time()
-        self.processing_time=round(t2-t1,2)
+        t2 = time.time()
+        self.processing_time = round(t2 - t1, 2)
         return answer
 
     def post_process(self, _quest0, answer):
         """
         to be overriden if application-specific post-processing
         of the LLM's answer is required
         """
```

### Comparing `deepllm-1.4.7/deepllm/local_llms/local_runs.py` & `deepllm-1.5.0/deepllm/local_llms/local_runs.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/local_llms/test_vicuna.py` & `deepllm-1.5.0/deepllm/local_llms/test_vicuna.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/params.py` & `deepllm-1.5.0/deepllm/params.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,33 @@
 import pickle
 import json
 import openai
 from deepllm.configurator import *
 
 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
-IS_LOCAL_LLM = [False]
+FORCE_TRACE = 1
+FORCE_SBERT = 0
 
-# LOCAL_MODEL="vicuna-7b-v1.5"
-LOCAL_MODEL = "mistralai/Mistral-7B-Instruct-v0.2"
 LOCAL_URL = "http://u.local:8000/v1"  # replace with where the server is
 
-FORCE_TRACE=1
-FORCE_SBERT=0
+IS_LOCAL_LLM = [False]
+
+mistral = "mistralai/Mistral-7B-Instruct-v0.2"
+llama = "meta-llama/Meta-Llama-3-8B-Instruct"
+vicuna = "vicuna-7b-v1.5"
+
+LOCAL_MODEL = [mistral]
+
+
+def fix_eos():
+    if IS_LOCAL_LLM[0] and LOCAL_MODEL[0] == llama:
+        return {"stop_token_ids": [128009]}
+    return None
+
 
 GPT_PARAMS = dict(
     TRACE=FORCE_TRACE,
     TO_SVOS=False,
     ROOT_="./STATE/",
     ROOT="./STATE_SMARTER/",
     CACHES="caches/",
@@ -41,15 +52,15 @@
     TRACE=FORCE_TRACE,
     TO_SVOS=False,
     ROOT="./STATE_LOCAL/",
     CACHES="caches/",
     OUT='out/',
     DATA='data/',
 
-    model=LOCAL_MODEL,
+    model=LOCAL_MODEL[0],
     API_BASE=LOCAL_URL,
 
     # emebedding_model="vicuna-7b-v1.5",
     emebedding_model="text-embedding-3-large",
 
     temperature=0.2,
     n=1,
@@ -125,17 +136,19 @@
     if exists_file(dname):
         shutil.rmtree(dname)
 
 
 def copy_file(src, dst):
     return shutil.copyfile(src, dst)
 
+def clear_local():
+    remove_dir(LOCAL_PARAMS['ROOT'])
 
 def clear_caches():
-    dirs=[
+    dirs = [
         GPT_PARAMS['ROOT'],
         GPT_PARAMS['ROOT_'],
         LOCAL_PARAMS['ROOT']
     ]
     for d in dirs:
         remove_dir(d)
     return dirs
```

### Comparing `deepllm-1.4.7/deepllm/prompters.py` & `deepllm-1.5.0/deepllm/prompters.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/questmaker.py` & `deepllm-1.5.0/deepllm/questmaker.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/recursors.py` & `deepllm-1.5.0/deepllm/recursors.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/refiners.py` & `deepllm-1.5.0/deepllm/refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/tests/test_all.py` & `deepllm-1.5.0/deepllm/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/tests/test_api.py` & `deepllm-1.5.0/deepllm/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/tests/test_embedders.py` & `deepllm-1.5.0/deepllm/tests/test_embedders.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/tests/test_recursors.py` & `deepllm-1.5.0/deepllm/tests/test_recursors.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/tests/test_refiners.py` & `deepllm-1.5.0/deepllm/tests/test_refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/tools.py` & `deepllm-1.5.0/deepllm/tools.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm/vis.py` & `deepllm-1.5.0/deepllm/vis.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.7/deepllm.egg-info/PKG-INFO` & `deepllm-1.5.0/deepllm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 1.4.7
+Version: 1.5.0
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: GPL-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deepllm-1.4.7/deepllm.egg-info/SOURCES.txt` & `deepllm-1.5.0/deepllm.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 deepllm/demos/viz.py
 deepllm/local_llms/README.md
 deepllm/local_llms/__init__.py
 deepllm/local_llms/install.sh
 deepllm/local_llms/local_runs.py
 deepllm/local_llms/requirements.txt
 deepllm/local_llms/server.sh
+deepllm/local_llms/test_llama3.py
 deepllm/local_llms/test_vicuna.py
 deepllm/tests/README.md
 deepllm/tests/__init__.py
 deepllm/tests/test_all.py
 deepllm/tests/test_api.py
 deepllm/tests/test_configurator.py
 deepllm/tests/test_embedders.py
```

### Comparing `deepllm-1.4.7/setup.py` & `deepllm-1.5.0/setup.py`

 * *Files identical despite different names*


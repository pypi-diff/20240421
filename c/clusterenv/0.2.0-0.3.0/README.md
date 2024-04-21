# Comparing `tmp/clusterenv-0.2.0.tar.gz` & `tmp/clusterenv-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clusterenv-0.2.0.tar", max compression
+gzip compressed data, was "clusterenv-0.3.0.tar", max compression
```

## Comparing `clusterenv-0.2.0.tar` & `clusterenv-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      176 2024-02-19 11:34:17.626664 clusterenv-0.2.0/README.md
--rw-r--r--   0        0        0      256 2024-03-01 20:00:46.287714 clusterenv-0.2.0/clusterenv/__init__.py
--rw-r--r--   0        0        0     5200 2024-02-28 17:18:43.783749 clusterenv-0.2.0/clusterenv/envs/base.py
--rw-r--r--   0        0        0    11375 2024-03-12 15:25:35.079512 clusterenv-0.2.0/clusterenv/envs/cluster.py
--rw-r--r--   0        0        0       32 2024-03-01 16:18:36.762354 clusterenv-0.2.0/clusterenv/wrappers/__init__.py
--rw-r--r--   0        0        0     2815 2024-03-12 15:32:17.678573 clusterenv-0.2.0/clusterenv/wrappers/queue.py
--rw-r--r--   0        0        0      524 2024-03-22 08:03:06.242237 clusterenv-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 clusterenv-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      176 2024-02-19 11:34:17.626664 clusterenv-0.3.0/README.md
+-rw-r--r--   0        0        0      241 2024-04-21 20:20:11.627059 clusterenv-0.3.0/clusterenv/__init__.py
+-rw-r--r--   0        0        0     4675 2024-04-21 20:01:25.417246 clusterenv-0.3.0/clusterenv/_types.py
+-rw-r--r--   0        0        0     5245 2024-04-21 20:38:28.492760 clusterenv-0.3.0/clusterenv/common.py
+-rw-r--r--   0        0        0     8305 2024-04-21 20:35:49.949707 clusterenv-0.3.0/clusterenv/envs/cluster.py
+-rw-r--r--   0        0        0     6305 2024-04-21 20:39:11.831616 clusterenv-0.3.0/clusterenv/render.py
+-rw-r--r--   0        0        0      523 2024-04-21 20:41:48.548908 clusterenv-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 clusterenv-0.3.0/PKG-INFO
```

### Comparing `clusterenv-0.2.0/pyproject.toml` & `clusterenv-0.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "clusterenv"
-version = "0.2.0"
+version = "0.3.0"
 description = "ClusterEnv is a Python Gym environment designed to simulate and model the management and optimization of computing clusters. In the realm of distributed computing."
 authors = ["Guy Arieli"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.9"
 gymnasium = "^0.29.1"
 matplotlib = "^3.8.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.1"
 
 [build-system]
```

### Comparing `clusterenv-0.2.0/PKG-INFO` & `clusterenv-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: clusterenv
-Version: 0.2.0
+Version: 0.3.0
 Summary: ClusterEnv is a Python Gym environment designed to simulate and model the management and optimization of computing clusters. In the realm of distributed computing.
 License: MIT
 Author: Guy Arieli
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: gymnasium (>=0.29.1,<0.30.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Description-Content-Type: text/markdown
 
 # ClusterEnv
 ClusterEnv is a Python Gym environment designed to simulate and model the management and optimization of computing clusters. In the realm of distributed computing
```


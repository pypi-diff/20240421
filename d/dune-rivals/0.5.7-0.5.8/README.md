# Comparing `tmp/dune_rivals-0.5.7.tar.gz` & `tmp/dune_rivals-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.5.7.tar", last modified: Sun Apr 21 18:55:21 2024, max compression
+gzip compressed data, was "dune_rivals-0.5.8.tar", last modified: Sun Apr 21 18:59:19 2024, max compression
```

## Comparing `dune_rivals-0.5.7.tar` & `dune_rivals-0.5.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 18:55:21.175858 dune_rivals-0.5.7/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 18:55:21.175383 dune_rivals-0.5.7/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.5.7/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 18:55:21.174955 dune_rivals-0.5.7/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 18:55:21.000000 dune_rivals-0.5.7/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-21 18:55:21.000000 dune_rivals-0.5.7/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-21 18:55:21.000000 dune_rivals-0.5.7/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-21 18:55:21.000000 dune_rivals-0.5.7/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    31239 2024-04-21 18:54:38.000000 dune_rivals-0.5.7/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-21 18:55:16.000000 dune_rivals-0.5.7/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-21 18:55:21.175960 dune_rivals-0.5.7/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 18:59:19.826898 dune_rivals-0.5.8/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 18:59:19.826478 dune_rivals-0.5.8/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.5.8/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 18:59:19.825996 dune_rivals-0.5.8/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 18:59:19.000000 dune_rivals-0.5.8/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-21 18:59:19.000000 dune_rivals-0.5.8/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-21 18:59:19.000000 dune_rivals-0.5.8/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-21 18:59:19.000000 dune_rivals-0.5.8/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    31334 2024-04-21 18:58:57.000000 dune_rivals-0.5.8/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-21 18:59:15.000000 dune_rivals-0.5.8/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-21 18:59:19.826990 dune_rivals-0.5.8/setup.cfg
```

### Comparing `dune_rivals-0.5.7/dune_rivals.py` & `dune_rivals-0.5.8/dune_rivals.py`

 * *Files 2% similar despite different names*

```diff
@@ -724,15 +724,17 @@
             try:
                 new_all_msgs = []
                 for d, idx in all_msgs:
                     if idx not in close_all_msgs_idxs:
                         new_all_msgs.append(d)
                 all_msgs = new_all_msgs
             except Exception as e:
+                print(f"K IS: {k}")
                 print(f"CLOSE ALL MESSAGES: {close_all_msgs_idxs}")
+                print(f"CLOSE OBJ IDXS: {close_obj_idxs}")
                 raise e
 
 @ray.remote(num_cpus=0.8, name="Sardaukar1", resources={"worker3": 1e-4})
 class Sardaukar1(BaseSardaukar):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 1
```


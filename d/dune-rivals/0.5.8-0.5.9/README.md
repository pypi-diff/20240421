# Comparing `tmp/dune_rivals-0.5.8.tar.gz` & `tmp/dune_rivals-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.5.8.tar", last modified: Sun Apr 21 18:59:19 2024, max compression
+gzip compressed data, was "dune_rivals-0.5.9.tar", last modified: Sun Apr 21 19:02:30 2024, max compression
```

## Comparing `dune_rivals-0.5.8.tar` & `dune_rivals-0.5.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 18:59:19.826898 dune_rivals-0.5.8/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 18:59:19.826478 dune_rivals-0.5.8/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.5.8/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 18:59:19.825996 dune_rivals-0.5.8/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 18:59:19.000000 dune_rivals-0.5.8/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-21 18:59:19.000000 dune_rivals-0.5.8/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-21 18:59:19.000000 dune_rivals-0.5.8/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-21 18:59:19.000000 dune_rivals-0.5.8/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    31334 2024-04-21 18:58:57.000000 dune_rivals-0.5.8/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-21 18:59:15.000000 dune_rivals-0.5.8/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-21 18:59:19.826990 dune_rivals-0.5.8/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 19:02:30.484970 dune_rivals-0.5.9/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 19:02:30.484363 dune_rivals-0.5.9/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.5.9/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 19:02:30.483611 dune_rivals-0.5.9/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 19:02:30.000000 dune_rivals-0.5.9/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-21 19:02:30.000000 dune_rivals-0.5.9/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-21 19:02:30.000000 dune_rivals-0.5.9/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-21 19:02:30.000000 dune_rivals-0.5.9/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    31165 2024-04-21 19:02:13.000000 dune_rivals-0.5.9/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-21 19:02:25.000000 dune_rivals-0.5.9/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-21 19:02:30.485070 dune_rivals-0.5.9/setup.cfg
```

### Comparing `dune_rivals-0.5.8/dune_rivals.py` & `dune_rivals-0.5.9/dune_rivals.py`

 * *Files 1% similar despite different names*

```diff
@@ -717,25 +717,20 @@
                 self._destroy_spice_field()
                 if len(next_warriors) > 0:
                     next_warrior_id = next_warriors[0]
                     next_warriors = next_warriors[1:]
                     self.gamestate.send_message.remote(next_warrior_id, self.id, {"loc": [loc[0], loc[1]], "next_warrior_ids": next_warriors}, "rival")
 
             # use close_obj_loc_idxs to remove items from all_msgs
-            try:
-                new_all_msgs = []
-                for d, idx in all_msgs:
-                    if idx not in close_all_msgs_idxs:
-                        new_all_msgs.append(d)
-                all_msgs = new_all_msgs
-            except Exception as e:
-                print(f"K IS: {k}")
-                print(f"CLOSE ALL MESSAGES: {close_all_msgs_idxs}")
-                print(f"CLOSE OBJ IDXS: {close_obj_idxs}")
-                raise e
+            close_all_msgs_idxs = close_all_msgs_idxs if k > 1 else [close_all_msgs_idxs]
+            new_all_msgs = []
+            for d, idx in all_msgs:
+                if idx not in close_all_msgs_idxs:
+                    new_all_msgs.append(d)
+            all_msgs = new_all_msgs
 
 @ray.remote(num_cpus=0.8, name="Sardaukar1", resources={"worker3": 1e-4})
 class Sardaukar1(BaseSardaukar):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 1
         self.name = "Sardaukar1"
```


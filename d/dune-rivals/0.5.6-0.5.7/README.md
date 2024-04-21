# Comparing `tmp/dune_rivals-0.5.6.tar.gz` & `tmp/dune_rivals-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.5.6.tar", last modified: Sun Apr 21 18:44:44 2024, max compression
+gzip compressed data, was "dune_rivals-0.5.7.tar", last modified: Sun Apr 21 18:55:21 2024, max compression
```

## Comparing `dune_rivals-0.5.6.tar` & `dune_rivals-0.5.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 18:44:44.256906 dune_rivals-0.5.6/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 18:44:44.256488 dune_rivals-0.5.6/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.5.6/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 18:44:44.256053 dune_rivals-0.5.6/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 18:44:44.000000 dune_rivals-0.5.6/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-21 18:44:44.000000 dune_rivals-0.5.6/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-21 18:44:44.000000 dune_rivals-0.5.6/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-21 18:44:44.000000 dune_rivals-0.5.6/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    31279 2024-04-21 18:44:29.000000 dune_rivals-0.5.6/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-21 18:44:39.000000 dune_rivals-0.5.6/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-21 18:44:44.256997 dune_rivals-0.5.6/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 18:55:21.175858 dune_rivals-0.5.7/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 18:55:21.175383 dune_rivals-0.5.7/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.5.7/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 18:55:21.174955 dune_rivals-0.5.7/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 18:55:21.000000 dune_rivals-0.5.7/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-21 18:55:21.000000 dune_rivals-0.5.7/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-21 18:55:21.000000 dune_rivals-0.5.7/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-21 18:55:21.000000 dune_rivals-0.5.7/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    31239 2024-04-21 18:54:38.000000 dune_rivals-0.5.7/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-21 18:55:16.000000 dune_rivals-0.5.7/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-21 18:55:21.175960 dune_rivals-0.5.7/setup.cfg
```

### Comparing `dune_rivals-0.5.6/dune_rivals.py` & `dune_rivals-0.5.7/dune_rivals.py`

 * *Files 2% similar despite different names*

```diff
@@ -585,17 +585,17 @@
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 4
         self.name = "FeydRautha4"
 
 
 ##############################################################################################
-################################           Muad'dib           ################################
+################################          Sardaukar           ################################
 ##############################################################################################
-class BaseMuadDib(BaseRivalActor):
+class BaseSardaukar(BaseRivalActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = None
         self.k = 50
 
     def get_spice_loc_map(self):
         return self.spice_loc_map
@@ -717,43 +717,44 @@
                 self._destroy_spice_field()
                 if len(next_warriors) > 0:
                     next_warrior_id = next_warriors[0]
                     next_warriors = next_warriors[1:]
                     self.gamestate.send_message.remote(next_warrior_id, self.id, {"loc": [loc[0], loc[1]], "next_warrior_ids": next_warriors}, "rival")
 
             # use close_obj_loc_idxs to remove items from all_msgs
-            all_msgs = [d for d, idx in all_msgs if idx not in close_all_msgs_idxs]
+            try:
+                new_all_msgs = []
+                for d, idx in all_msgs:
+                    if idx not in close_all_msgs_idxs:
+                        new_all_msgs.append(d)
+                all_msgs = new_all_msgs
+            except Exception as e:
+                print(f"CLOSE ALL MESSAGES: {close_all_msgs_idxs}")
+                raise e
 
-
-@ray.remote(num_cpus=0.8, name="Muad'dib1", resources={"worker3": 1e-4})
-class Muaddib1(BaseMuadDib):
-    """
-    Muaddib computes the distance from each worker to its top-k nearest spice fields
-    and coordinates which one(s) to destroy. The (k/2)-kth closest fields are selected to be destroyed,
-    and if any actors which are not needed can be used to destroy one of the [k/2, k] fields in parallel
-    then that is done as well.
-    """
+@ray.remote(num_cpus=0.8, name="Sardaukar1", resources={"worker3": 1e-4})
+class Sardaukar1(BaseSardaukar):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 1
-        self.name = "Muad'dib1"
+        self.name = "Sardaukar1"
 
-@ray.remote(num_cpus=0.8, name="Muad'dib2", resources={"worker3": 1e-4})
-class Muaddib2(BaseMuadDib):
+@ray.remote(num_cpus=0.8, name="Sardaukar2", resources={"worker3": 1e-4})
+class Sardaukar2(BaseSardaukar):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 2
-        self.name = "Muad'dib2"
+        self.name = "Sardaukar2"
 
-@ray.remote(num_cpus=0.8, name="Muad'dib3", resources={"worker4": 1e-4})
-class Muaddib3(BaseMuadDib):
+@ray.remote(num_cpus=0.8, name="Sardaukar3", resources={"worker4": 1e-4})
+class Sardaukar3(BaseSardaukar):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 3
-        self.name = "Muad'dib3"
+        self.name = "Sardaukar3"
 
-@ray.remote(num_cpus=0.8, name="Muad'dib4", resources={"worker4": 1e-4})
-class Muaddib4(BaseMuadDib):
+@ray.remote(num_cpus=0.8, name="Sardaukar4", resources={"worker4": 1e-4})
+class Sardaukar4(BaseSardaukar):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 4
-        self.name = "Muad'dib4"
+        self.name = "Sardaukar4"
```


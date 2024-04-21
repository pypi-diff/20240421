# Comparing `tmp/dune_rivals-0.5.1.tar.gz` & `tmp/dune_rivals-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.5.1.tar", last modified: Sun Apr 21 17:39:40 2024, max compression
+gzip compressed data, was "dune_rivals-0.5.2.tar", last modified: Sun Apr 21 17:41:39 2024, max compression
```

## Comparing `dune_rivals-0.5.1.tar` & `dune_rivals-0.5.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:39:40.964419 dune_rivals-0.5.1/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:39:40.963957 dune_rivals-0.5.1/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.5.1/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:39:40.963491 dune_rivals-0.5.1/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:39:40.000000 dune_rivals-0.5.1/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-21 17:39:40.000000 dune_rivals-0.5.1/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-21 17:39:40.000000 dune_rivals-0.5.1/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-21 17:39:40.000000 dune_rivals-0.5.1/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    33748 2024-04-21 17:38:51.000000 dune_rivals-0.5.1/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-21 17:39:27.000000 dune_rivals-0.5.1/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-21 17:39:40.964600 dune_rivals-0.5.1/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:41:39.978906 dune_rivals-0.5.2/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:41:39.978306 dune_rivals-0.5.2/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.5.2/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:41:39.977678 dune_rivals-0.5.2/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:41:39.000000 dune_rivals-0.5.2/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-21 17:41:39.000000 dune_rivals-0.5.2/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-21 17:41:39.000000 dune_rivals-0.5.2/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-21 17:41:39.000000 dune_rivals-0.5.2/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    31086 2024-04-21 17:41:12.000000 dune_rivals-0.5.2/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-21 17:41:35.000000 dune_rivals-0.5.2/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-21 17:41:39.979149 dune_rivals-0.5.2/setup.cfg
```

### Comparing `dune_rivals-0.5.1/dune_rivals.py` & `dune_rivals-0.5.2/dune_rivals.py`

 * *Files 2% similar despite different names*

```diff
@@ -591,16 +591,15 @@
 ##############################################################################################
 ################################           Muad'dib           ################################
 ##############################################################################################
 class BaseMuadDib(BaseRivalActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = None
-        self.free = None
-        self.num_singletons = {}
+        self.k = 50
 
     def get_spice_loc_map(self):
         return self.spice_loc_map
 
     def is_free(self):
         return self.free
 
@@ -727,73 +726,14 @@
     and if any actors which are not needed can be used to destroy one of the [k/2, k] fields in parallel
     then that is done as well.
     """
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 1
         self.name = "Muad'dib1"
-        self.k = 10
-
-    # def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
-    #     # set these state variables
-    #     self.spice_loc_map = spice_loc_map
-    #     self.spice_file_map = spice_file_map
-    #     self.order_map = order_map
-
-    #     # construct spice arr w/this warrior's fields for finding nearest points quickly
-    #     def get_warrior_spice_arr(file_type):
-    #         locs, singletons = [], []
-    #         spice = np.where(self.spice_file_map==file_type)
-    #         idx = 0
-    #         for i, j in zip(spice[0], spice[1]):
-    #             warriors = self.order_map[(i, j)]
-    #             if self.id in warriors:
-    #                 locs.append((i, j))
-    #                 if len(warriors) == 1:
-    #                     singletons.append(idx)
-    #                 idx += 1
-    #         return np.array(locs), np.array(singletons)
-
-    #     obj_spice_arr, obj_singletons = get_warrior_spice_arr(file_type=OBJ_FILE)
-
-    #     # destroy all the obj singletons associated with this warrior
-    #     for i, j in obj_spice_arr[obj_singletons]:
-    #         self._ride_sandworm(i, j)
-    #         self.destroy_block(self.id)
-
-    #     # loop forever and destroy spice
-    #     while len(obj_spice_arr) > 0:
-    #         # construct spatial tree
-    #         obj_spatial_tree = sp.spatial.KDTree(obj_spice_arr)
-
-    #         # get location of each warrior
-    #         other_warrior_coords = ray.get([
-    #             ray.get_actor(f"Muad'dib{id}").get_location.remote()
-    #             for id in [2, 3, 4]
-    #         ])
-    #         warrior_coords = [(self.i, self.j)] + other_warrior_coords
-
-    #         # aggregate closest [k/2, k] spice fields for each worker
-    #         close_obj_locs, close_obj_indices = [], []
-    #         for i, j in warrior_coords:
-    #             pt = [i, j]
-    #             close_obj_loc_idxs = obj_spatial_tree.query(pt, k=self.k)[1][int(self.k/2):]
-    #             close_obj_locs.extend(obj_spice_arr[close_obj_loc_idxs])
-    #             close_obj_indices.extend(close_obj_loc_idxs)
-
-    #         # filter for unique set of locations and indices
-    #         close_obj_locs = np.unique(np.array(close_obj_locs), axis=0)
-    #         close_obj_indices = np.unique(np.array(close_obj_indices), axis=0)
-
-    #         # destroy all singletons first
-    #         for loc in close_obj_locs:
-    #             i, j = loc[0], loc[1]
-    #             warriors = self.order_map[(i, j)]
-    #             if len(warriors) == 1:
-    #                 command_field_destroy(warriors[0])
 
 @ray.remote(num_cpus=0.8, name="Muad'dib2", resources={"worker3": 1e-4})
 class Muaddib2(BaseMuadDib):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 2
         self.name = "Muad'dib2"
```


# Comparing `tmp/dune_rivals-0.4.5.tar.gz` & `tmp/dune_rivals-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.4.5.tar", last modified: Wed Apr 17 15:06:45 2024, max compression
+gzip compressed data, was "dune_rivals-0.5.0.tar", last modified: Sun Apr 21 17:31:51 2024, max compression
```

## Comparing `dune_rivals-0.4.5.tar` & `dune_rivals-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-17 15:06:45.480302 dune_rivals-0.4.5/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-17 15:06:45.479736 dune_rivals-0.4.5/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.4.5/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-17 15:06:45.479229 dune_rivals-0.4.5/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-17 15:06:45.000000 dune_rivals-0.4.5/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-17 15:06:45.000000 dune_rivals-0.4.5/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-17 15:06:45.000000 dune_rivals-0.4.5/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-17 15:06:45.000000 dune_rivals-0.4.5/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    24234 2024-04-17 15:06:19.000000 dune_rivals-0.4.5/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-17 15:06:40.000000 dune_rivals-0.4.5/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-17 15:06:45.480398 dune_rivals-0.4.5/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:31:51.146223 dune_rivals-0.5.0/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:31:51.145741 dune_rivals-0.5.0/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.5.0/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:31:51.145301 dune_rivals-0.5.0/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:31:51.000000 dune_rivals-0.5.0/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-21 17:31:51.000000 dune_rivals-0.5.0/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-21 17:31:51.000000 dune_rivals-0.5.0/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-21 17:31:51.000000 dune_rivals-0.5.0/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    33766 2024-04-21 17:30:33.000000 dune_rivals-0.5.0/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-21 17:31:32.000000 dune_rivals-0.5.0/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-21 17:31:51.146322 dune_rivals-0.5.0/setup.cfg
```

### Comparing `dune_rivals-0.4.5/dune_rivals.py` & `dune_rivals-0.5.0/dune_rivals.py`

 * *Files 16% similar despite different names*

```diff
@@ -582,7 +582,232 @@
 
 @ray.remote(num_cpus=0.8, name="FeydRautha4", resources={"worker4": 1e-4})
 class FeydRautha4(BaseFeydRautha):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 4
         self.name = "FeydRautha4"
+
+
+##############################################################################################
+################################           Muad'dib           ################################
+##############################################################################################
+class BaseMuadDib(BaseRivalActor):
+    def __init__(self, payload: str):
+        super().__init__(payload)
+        self.id = None
+        self.free = None
+        self.num_singletons = {}
+
+    def get_spice_loc_map(self):
+        return self.spice_loc_map
+
+    def is_free(self):
+        return self.free
+
+    def set_num_singletons(self, id, num_singletons):
+        self.num_singletons[id] = num_singletons
+
+    def destroy_spice_field_with_retry(self, leader):
+        self.gamestate.send_message.remote(leader, self.id, {"free": False}, "rival")
+        destroyed = False
+        while not destroyed:
+            destroyed = self._destroy_spice_field()
+            time.sleep(0.0001)
+        
+        self.gamestate.send_message.remote(leader, self.id, {"free": True}, "rival")
+
+    def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+        # set these state variables
+        self.spice_loc_map = spice_loc_map
+        self.spice_file_map = spice_file_map
+        self.order_map = order_map
+
+        # import KDTree
+        from scipy.spatial import KDTree
+
+        # construct spice arr w/this warrior's fields for finding nearest points quickly
+        def get_warrior_spice_arr(file_type, warrior_idx):
+            locs = []
+            spice = np.where(self.spice_file_map==file_type)
+            row_locs, prev_i = [], 0
+            for i, j in zip(spice[0], spice[1]):
+                warriors = self.order_map[(i, j)]
+
+                # ignore all fields w/4 warriors
+                if len(warriors) == 4:
+                    continue
+
+                # if the current warrior is in the warrior_idx position, include it
+                if self.id == warriors[warrior_idx]:
+                    next_warrior_ids = warriors[warrior_idx+1:]
+                    row_locs.append((i, j, next_warrior_ids))
+
+                # add elements to list in snake-fashion
+                if i != prev_i:
+                    row_locs = row_locs if i % 2 == 0 else list(reversed(row_locs))
+                    locs.extend(row_locs)
+                    row_locs = []
+                prev_i = i
+
+            return np.array(locs)
+
+        # compute location of spice fields of different num workers
+        obj_first_spice_arr = get_warrior_spice_arr(file_type=OBJ_FILE, warrior_idx=0)
+        # obj_second_spice_arr = get_warrior_spice_arr(file_type=OBJ_FILE, warrior_idx=1)
+        # obj_third_spice_arr = get_warrior_spice_arr(file_type=OBJ_FILE, warrior_idx=2)
+
+        # destroy all the obj singletons associated with this warrior
+        for i, j, next_warrior_ids in obj_first_spice_arr:
+            self._ride_sandworm(i, j)
+            self._destroy_spice_field()
+            if len(next_warrior_ids) > 0:
+                next_warrior_id = next_warrior_ids[0]
+                next_warrior_ids = next_warrior_ids[1:]
+                self.gamestate.send_message.remote(next_warrior_id, self.id, {"loc": [i, j], "next_warrior_ids": next_warrior_ids}, "rival")
+
+        # move to center
+        self._ride_sandworm(int(MAP_DIM/2), int(MAP_DIM/2))
+
+        all_msgs = []
+        while True:
+            # fetch messages with fields ready to be destroyed
+            for warrior_id in [1, 2, 3, 4]:
+                if warrior_id == self.id:
+                    continue
+
+                # fetch messages
+                msgs = ray.get(self.gamestate.get_new_messages.remote(self.id, warrior_id, "rival"))
+                all_msgs.extend(msgs)
+
+            # add index to each msg in all_msgs
+            all_msgs = [(d, idx) for idx, d in enumerate(all_msgs)]
+
+            # filter locations for subset with only one warrior left
+            elts = list(map(lambda tup: (tup[0]["loc"], tup[0]["next_warrior_ids"], tup[1]), all_msgs))
+            elts_ = list(filter(lambda tup: len(tup[1]) == 1, elts))
+            if len(elts_) == 0:
+                elts_ = list(filter(lambda tup: len(tup[1]) == 2, elts))
+
+            locs, next_warriors, idxs = [], [], []
+            for elt in elts_:
+                locs.append(elt[0])
+                next_warriors.append(elt[1][1:])
+                idxs.append(elt[2])
+
+            loc_arr = np.array(locs)
+            next_warriors_arr = np.array(next_warriors)
+            all_msgs_idxs_arr = np.array(idxs)
+
+            # find k closest fields
+            k = min(self.k, len(locs))
+            obj_spatial_tree = KDTree(loc_arr)
+            close_obj_idxs = obj_spatial_tree.query([self.i, self.j], k=k)[1]
+            close_locs = loc_arr[close_obj_idxs]
+            close_next_warriors = next_warriors_arr[close_obj_idxs]
+            close_all_msgs_idxs = all_msgs_idxs_arr[close_obj_idxs]
+
+            # destroy and send message to next warrior if applicable
+            for loc, next_warriors in zip(close_locs, close_next_warriors):
+                self._ride_sandworm(loc[0], loc[1])
+                self._destroy_spice_field()
+                if len(next_warriors) > 0:
+                    next_warrior_id = next_warriors[0]
+                    next_warriors = next_warriors[1:]
+                    self.gamestate.send_message.remote(next_warrior_id, self.id, {"loc": [loc[0], loc[1]], "next_warrior_ids": next_warriors}, "rival")
+
+            # use close_obj_loc_idxs to remove items from all_msgs
+            all_msgs = [d for d, idx in all_msgs if idx not in close_all_msgs_idxs]
+
+
+@ray.remote(num_cpus=0.8, name="Muad'dib1", resources={"worker3": 1e-4})
+class Muaddib1(BaseMuadDib):
+    """
+    Muaddib computes the distance from each worker to its top-k nearest spice fields
+    and coordinates which one(s) to destroy. The (k/2)-kth closest fields are selected to be destroyed,
+    and if any actors which are not needed can be used to destroy one of the [k/2, k] fields in parallel
+    then that is done as well.
+    """
+    def __init__(self, payload: str):
+        super().__init__(payload)
+        self.id = 1
+        self.name = "Muad'dib1"
+        self.k = 10
+
+    # def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+    #     # set these state variables
+    #     self.spice_loc_map = spice_loc_map
+    #     self.spice_file_map = spice_file_map
+    #     self.order_map = order_map
+
+    #     # construct spice arr w/this warrior's fields for finding nearest points quickly
+    #     def get_warrior_spice_arr(file_type):
+    #         locs, singletons = [], []
+    #         spice = np.where(self.spice_file_map==file_type)
+    #         idx = 0
+    #         for i, j in zip(spice[0], spice[1]):
+    #             warriors = self.order_map[(i, j)]
+    #             if self.id in warriors:
+    #                 locs.append((i, j))
+    #                 if len(warriors) == 1:
+    #                     singletons.append(idx)
+    #                 idx += 1
+    #         return np.array(locs), np.array(singletons)
+
+    #     obj_spice_arr, obj_singletons = get_warrior_spice_arr(file_type=OBJ_FILE)
+
+    #     # destroy all the obj singletons associated with this warrior
+    #     for i, j in obj_spice_arr[obj_singletons]:
+    #         self._ride_sandworm(i, j)
+    #         self.destroy_block(self.id)
+
+    #     # loop forever and destroy spice
+    #     while len(obj_spice_arr) > 0:
+    #         # construct spatial tree
+    #         obj_spatial_tree = sp.spatial.KDTree(obj_spice_arr)
+
+    #         # get location of each warrior
+    #         other_warrior_coords = ray.get([
+    #             ray.get_actor(f"Muad'dib{id}").get_location.remote()
+    #             for id in [2, 3, 4]
+    #         ])
+    #         warrior_coords = [(self.i, self.j)] + other_warrior_coords
+
+    #         # aggregate closest [k/2, k] spice fields for each worker
+    #         close_obj_locs, close_obj_indices = [], []
+    #         for i, j in warrior_coords:
+    #             pt = [i, j]
+    #             close_obj_loc_idxs = obj_spatial_tree.query(pt, k=self.k)[1][int(self.k/2):]
+    #             close_obj_locs.extend(obj_spice_arr[close_obj_loc_idxs])
+    #             close_obj_indices.extend(close_obj_loc_idxs)
+
+    #         # filter for unique set of locations and indices
+    #         close_obj_locs = np.unique(np.array(close_obj_locs), axis=0)
+    #         close_obj_indices = np.unique(np.array(close_obj_indices), axis=0)
+
+    #         # destroy all singletons first
+    #         for loc in close_obj_locs:
+    #             i, j = loc[0], loc[1]
+    #             warriors = self.order_map[(i, j)]
+    #             if len(warriors) == 1:
+    #                 command_field_destroy(warriors[0])
+
+@ray.remote(num_cpus=0.8, name="Muad'dib2", resources={"worker3": 1e-4})
+class Muaddib2(BaseMuadDib):
+    def __init__(self, payload: str):
+        super().__init__(payload)
+        self.id = 2
+        self.name = "Muad'dib2"
+
+@ray.remote(num_cpus=0.8, name="Muad'dib3", resources={"worker4": 1e-4})
+class Muaddib3(BaseMuadDib):
+    def __init__(self, payload: str):
+        super().__init__(payload)
+        self.id = 3
+        self.name = "Muad'dib3"
+
+@ray.remote(num_cpus=0.8, name="Muad'dib4", resources={"worker4": 1e-4})
+class Muaddib4(BaseMuadDib):
+    def __init__(self, payload: str):
+        super().__init__(payload)
+        self.id = 4
+        self.name = "Muad'dib4"
```


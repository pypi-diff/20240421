# Comparing `tmp/dune_rivals-0.5.0.tar.gz` & `tmp/dune_rivals-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.5.0.tar", last modified: Sun Apr 21 17:31:51 2024, max compression
+gzip compressed data, was "dune_rivals-0.5.1.tar", last modified: Sun Apr 21 17:39:40 2024, max compression
```

## Comparing `dune_rivals-0.5.0.tar` & `dune_rivals-0.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:31:51.146223 dune_rivals-0.5.0/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:31:51.145741 dune_rivals-0.5.0/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.5.0/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:31:51.145301 dune_rivals-0.5.0/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:31:51.000000 dune_rivals-0.5.0/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-21 17:31:51.000000 dune_rivals-0.5.0/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-21 17:31:51.000000 dune_rivals-0.5.0/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-21 17:31:51.000000 dune_rivals-0.5.0/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    33766 2024-04-21 17:30:33.000000 dune_rivals-0.5.0/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-21 17:31:32.000000 dune_rivals-0.5.0/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-21 17:31:51.146322 dune_rivals-0.5.0/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:39:40.964419 dune_rivals-0.5.1/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:39:40.963957 dune_rivals-0.5.1/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.5.1/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:39:40.963491 dune_rivals-0.5.1/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:39:40.000000 dune_rivals-0.5.1/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-21 17:39:40.000000 dune_rivals-0.5.1/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-21 17:39:40.000000 dune_rivals-0.5.1/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-21 17:39:40.000000 dune_rivals-0.5.1/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    33748 2024-04-21 17:38:51.000000 dune_rivals-0.5.1/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-21 17:39:27.000000 dune_rivals-0.5.1/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-21 17:39:40.964600 dune_rivals-0.5.1/setup.cfg
```

### Comparing `dune_rivals-0.5.0/dune_rivals.py` & `dune_rivals-0.5.1/dune_rivals.py`

 * *Files 0% similar despite different names*

```diff
@@ -645,23 +645,23 @@
                 # add elements to list in snake-fashion
                 if i != prev_i:
                     row_locs = row_locs if i % 2 == 0 else list(reversed(row_locs))
                     locs.extend(row_locs)
                     row_locs = []
                 prev_i = i
 
-            return np.array(locs)
+            return locs
 
         # compute location of spice fields of different num workers
-        obj_first_spice_arr = get_warrior_spice_arr(file_type=OBJ_FILE, warrior_idx=0)
+        obj_first_spice = get_warrior_spice_arr(file_type=OBJ_FILE, warrior_idx=0)
         # obj_second_spice_arr = get_warrior_spice_arr(file_type=OBJ_FILE, warrior_idx=1)
         # obj_third_spice_arr = get_warrior_spice_arr(file_type=OBJ_FILE, warrior_idx=2)
 
         # destroy all the obj singletons associated with this warrior
-        for i, j, next_warrior_ids in obj_first_spice_arr:
+        for i, j, next_warrior_ids in obj_first_spice:
             self._ride_sandworm(i, j)
             self._destroy_spice_field()
             if len(next_warrior_ids) > 0:
                 next_warrior_id = next_warrior_ids[0]
                 next_warrior_ids = next_warrior_ids[1:]
                 self.gamestate.send_message.remote(next_warrior_id, self.id, {"loc": [i, j], "next_warrior_ids": next_warrior_ids}, "rival")
```


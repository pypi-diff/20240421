# Comparing `tmp/dune_rivals-0.5.2.tar.gz` & `tmp/dune_rivals-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.5.2.tar", last modified: Sun Apr 21 17:41:39 2024, max compression
+gzip compressed data, was "dune_rivals-0.5.3.tar", last modified: Sun Apr 21 17:52:46 2024, max compression
```

## Comparing `dune_rivals-0.5.2.tar` & `dune_rivals-0.5.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:41:39.978906 dune_rivals-0.5.2/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:41:39.978306 dune_rivals-0.5.2/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.5.2/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:41:39.977678 dune_rivals-0.5.2/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:41:39.000000 dune_rivals-0.5.2/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-21 17:41:39.000000 dune_rivals-0.5.2/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-21 17:41:39.000000 dune_rivals-0.5.2/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-21 17:41:39.000000 dune_rivals-0.5.2/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    31086 2024-04-21 17:41:12.000000 dune_rivals-0.5.2/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-21 17:41:35.000000 dune_rivals-0.5.2/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-21 17:41:39.979149 dune_rivals-0.5.2/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:52:46.067426 dune_rivals-0.5.3/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:52:46.066986 dune_rivals-0.5.3/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.5.3/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:52:46.066479 dune_rivals-0.5.3/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:52:46.000000 dune_rivals-0.5.3/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-21 17:52:46.000000 dune_rivals-0.5.3/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-21 17:52:46.000000 dune_rivals-0.5.3/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-21 17:52:46.000000 dune_rivals-0.5.3/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    31207 2024-04-21 17:50:43.000000 dune_rivals-0.5.3/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-21 17:52:40.000000 dune_rivals-0.5.3/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-21 17:52:46.067520 dune_rivals-0.5.3/setup.cfg
```

### Comparing `dune_rivals-0.5.2/dune_rivals.py` & `dune_rivals-0.5.3/dune_rivals.py`

 * *Files 1% similar despite different names*

```diff
@@ -677,14 +677,18 @@
                 # fetch messages
                 msgs = ray.get(self.gamestate.get_new_messages.remote(self.id, warrior_id, "rival"))
                 all_msgs.extend(msgs)
 
             # add index to each msg in all_msgs
             all_msgs = [(d, idx) for idx, d in enumerate(all_msgs)]
 
+            if len(all_msgs) == 0:
+                print("SLEEPING FOR NEW MESSAGES")
+                time.sleep(0.001)
+
             # filter locations for subset with only one warrior left
             elts = list(map(lambda tup: (tup[0]["loc"], tup[0]["next_warrior_ids"], tup[1]), all_msgs))
             elts_ = list(filter(lambda tup: len(tup[1]) == 1, elts))
             if len(elts_) == 0:
                 elts_ = list(filter(lambda tup: len(tup[1]) == 2, elts))
 
             locs, next_warriors, idxs = [], [], []
```


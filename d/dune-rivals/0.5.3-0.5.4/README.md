# Comparing `tmp/dune_rivals-0.5.3.tar.gz` & `tmp/dune_rivals-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.5.3.tar", last modified: Sun Apr 21 17:52:46 2024, max compression
+gzip compressed data, was "dune_rivals-0.5.4.tar", last modified: Sun Apr 21 17:57:35 2024, max compression
```

## Comparing `dune_rivals-0.5.3.tar` & `dune_rivals-0.5.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:52:46.067426 dune_rivals-0.5.3/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:52:46.066986 dune_rivals-0.5.3/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.5.3/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:52:46.066479 dune_rivals-0.5.3/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:52:46.000000 dune_rivals-0.5.3/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-21 17:52:46.000000 dune_rivals-0.5.3/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-21 17:52:46.000000 dune_rivals-0.5.3/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-21 17:52:46.000000 dune_rivals-0.5.3/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    31207 2024-04-21 17:50:43.000000 dune_rivals-0.5.3/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-21 17:52:40.000000 dune_rivals-0.5.3/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-21 17:52:46.067520 dune_rivals-0.5.3/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:57:35.899529 dune_rivals-0.5.4/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:57:35.899088 dune_rivals-0.5.4/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.5.4/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 17:57:35.898678 dune_rivals-0.5.4/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 17:57:35.000000 dune_rivals-0.5.4/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-21 17:57:35.000000 dune_rivals-0.5.4/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-21 17:57:35.000000 dune_rivals-0.5.4/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-21 17:57:35.000000 dune_rivals-0.5.4/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    31232 2024-04-21 17:57:22.000000 dune_rivals-0.5.4/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-21 17:57:31.000000 dune_rivals-0.5.4/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-21 17:57:35.899632 dune_rivals-0.5.4/setup.cfg
```

### Comparing `dune_rivals-0.5.3/dune_rivals.py` & `dune_rivals-0.5.4/dune_rivals.py`

 * *Files 0% similar despite different names*

```diff
@@ -680,14 +680,15 @@
 
             # add index to each msg in all_msgs
             all_msgs = [(d, idx) for idx, d in enumerate(all_msgs)]
 
             if len(all_msgs) == 0:
                 print("SLEEPING FOR NEW MESSAGES")
                 time.sleep(0.001)
+                continue
 
             # filter locations for subset with only one warrior left
             elts = list(map(lambda tup: (tup[0]["loc"], tup[0]["next_warrior_ids"], tup[1]), all_msgs))
             elts_ = list(filter(lambda tup: len(tup[1]) == 1, elts))
             if len(elts_) == 0:
                 elts_ = list(filter(lambda tup: len(tup[1]) == 2, elts))
```


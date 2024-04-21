# Comparing `tmp/chainzpy-0.5.tar.gz` & `tmp/chainzpy-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainzpy-0.5.tar", last modified: Fri Apr 19 17:02:20 2024, max compression
+gzip compressed data, was "chainzpy-0.6.tar", last modified: Sun Apr 21 03:01:45 2024, max compression
```

## Comparing `chainzpy-0.5.tar` & `chainzpy-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-19 17:02:20.760903 chainzpy-0.5/
-drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-19 17:02:20.758406 chainzpy-0.5/Chainzpy/
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      328 2024-04-14 17:14:47.000000 chainzpy-0.5/Chainzpy/__init__.py
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)     3369 2024-04-19 17:01:39.000000 chainzpy-0.5/Chainzpy/main.py
-drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-19 17:02:20.760116 chainzpy-0.5/Chainzpy.egg-info/
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      334 2024-04-19 17:02:20.000000 chainzpy-0.5/Chainzpy.egg-info/PKG-INFO
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      412 2024-04-19 17:02:20.000000 chainzpy-0.5/Chainzpy.egg-info/SOURCES.txt
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        1 2024-04-19 17:02:20.000000 chainzpy-0.5/Chainzpy.egg-info/dependency_links.txt
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       13 2024-04-19 17:02:20.000000 chainzpy-0.5/Chainzpy.egg-info/requires.txt
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        9 2024-04-19 17:02:20.000000 chainzpy-0.5/Chainzpy.egg-info/top_level.txt
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      334 2024-04-19 17:02:20.760455 chainzpy-0.5/PKG-INFO
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-14 07:29:26.000000 chainzpy-0.5/README.md
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       38 2024-04-19 17:02:20.760971 chainzpy-0.5/setup.cfg
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      462 2024-04-19 17:00:49.000000 chainzpy-0.5/setup.py
+drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-21 03:01:45.348560 chainzpy-0.6/
+drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-21 03:01:45.346085 chainzpy-0.6/Chainzpy/
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      328 2024-04-14 17:14:47.000000 chainzpy-0.6/Chainzpy/__init__.py
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)     3369 2024-04-21 03:00:20.000000 chainzpy-0.6/Chainzpy/main.py
+drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-21 03:01:45.347777 chainzpy-0.6/Chainzpy.egg-info/
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      334 2024-04-21 03:01:45.000000 chainzpy-0.6/Chainzpy.egg-info/PKG-INFO
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      412 2024-04-21 03:01:45.000000 chainzpy-0.6/Chainzpy.egg-info/SOURCES.txt
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        1 2024-04-21 03:01:45.000000 chainzpy-0.6/Chainzpy.egg-info/dependency_links.txt
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       13 2024-04-21 03:01:45.000000 chainzpy-0.6/Chainzpy.egg-info/requires.txt
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        9 2024-04-21 03:01:45.000000 chainzpy-0.6/Chainzpy.egg-info/top_level.txt
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      334 2024-04-21 03:01:45.348131 chainzpy-0.6/PKG-INFO
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-14 07:29:26.000000 chainzpy-0.6/README.md
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       38 2024-04-21 03:01:45.348627 chainzpy-0.6/setup.cfg
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      462 2024-04-21 03:01:17.000000 chainzpy-0.6/setup.py
```

### Comparing `chainzpy-0.5/Chainzpy/main.py` & `chainzpy-0.6/Chainzpy/main.py`

 * *Files identical despite different names*


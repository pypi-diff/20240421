# Comparing `tmp/haskellian-0.3.0.tar.gz` & `tmp/haskellian-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-0.3.0.tar", last modified: Sun Apr 21 15:05:34 2024, max compression
+gzip compressed data, was "haskellian-0.3.1.tar", last modified: Sun Apr 21 15:09:33 2024, max compression
```

## Comparing `haskellian-0.3.0.tar` & `haskellian-0.3.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:05:34.872662 haskellian-0.3.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1425 2024-04-21 15:05:34.872662 haskellian-0.3.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1040 2024-04-21 15:03:09.000000 haskellian-0.3.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-04-21 15:03:50.000000 haskellian-0.3.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-21 15:05:34.872662 haskellian-0.3.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:05:34.852662 haskellian-0.3.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:05:34.862662 haskellian-0.3.0/src/haskellian/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      156 2024-04-21 08:31:50.000000 haskellian-0.3.0/src/haskellian/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      494 2024-04-21 14:43:52.000000 haskellian-0.3.0/src/haskellian/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:05:34.862662 haskellian-0.3.0/src/haskellian/asyn_iter/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 14:25:49.000000 haskellian-0.3.0/src/haskellian/asyn_iter/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      441 2024-04-21 14:39:06.000000 haskellian-0.3.0/src/haskellian/asyn_iter/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2234 2024-04-21 14:39:41.000000 haskellian-0.3.0/src/haskellian/asyn_iter/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2125 2024-04-21 14:40:29.000000 haskellian-0.3.0/src/haskellian/asyn_iter/iter.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      490 2024-04-21 14:38:54.000000 haskellian-0.3.0/src/haskellian/asyn_iter/lifting.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      886 2024-04-21 14:38:19.000000 haskellian-0.3.0/src/haskellian/asyn_iter/managed.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      650 2024-04-21 14:40:28.000000 haskellian-0.3.0/src/haskellian/asyn_iter/prefetching.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:05:34.862662 haskellian-0.3.0/src/haskellian/classes/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 09:04:50.000000 haskellian-0.3.0/src/haskellian/classes/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      137 2024-04-21 09:04:51.000000 haskellian-0.3.0/src/haskellian/classes/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      578 2024-04-21 10:23:51.000000 haskellian-0.3.0/src/haskellian/classes/applicative.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      413 2024-04-21 10:23:57.000000 haskellian-0.3.0/src/haskellian/classes/functor.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      832 2024-04-21 14:05:41.000000 haskellian-0.3.0/src/haskellian/classes/monad.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       20 2024-04-21 10:15:52.000000 haskellian-0.3.0/src/haskellian/config.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:05:34.862662 haskellian-0.3.0/src/haskellian/either/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 10:31:26.000000 haskellian-0.3.0/src/haskellian/either/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      405 2024-04-21 10:39:57.000000 haskellian-0.3.0/src/haskellian/either/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2644 2024-04-21 14:05:41.000000 haskellian-0.3.0/src/haskellian/either/either.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1285 2024-04-21 10:38:12.000000 haskellian-0.3.0/src/haskellian/either/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      381 2024-04-21 10:36:36.000000 haskellian-0.3.0/src/haskellian/either/narrowing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      464 2024-04-21 10:39:34.000000 haskellian-0.3.0/src/haskellian/either/pydantic.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:05:34.862662 haskellian-0.3.0/src/haskellian/iter/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 13:06:20.000000 haskellian-0.3.0/src/haskellian/iter/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      593 2024-04-21 13:51:40.000000 haskellian-0.3.0/src/haskellian/iter/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      799 2024-04-21 13:51:48.000000 haskellian-0.3.0/src/haskellian/iter/basics.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      680 2024-04-21 13:53:19.000000 haskellian-0.3.0/src/haskellian/iter/batching.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      485 2024-04-21 13:53:13.000000 haskellian-0.3.0/src/haskellian/iter/indexing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2342 2024-04-21 14:41:28.000000 haskellian-0.3.0/src/haskellian/iter/iter.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      473 2024-04-21 13:52:51.000000 haskellian-0.3.0/src/haskellian/iter/lifting.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4144 2024-04-21 13:58:56.000000 haskellian-0.3.0/src/haskellian/iter/nested.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1140 2024-04-21 13:59:18.000000 haskellian-0.3.0/src/haskellian/iter/slicing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1003 2024-04-21 13:59:47.000000 haskellian-0.3.0/src/haskellian/iter/zipping.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:05:34.872662 haskellian-0.3.0/src/haskellian/pipe/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       22 2024-04-21 10:07:57.000000 haskellian-0.3.0/src/haskellian/pipe/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      767 2024-04-21 14:05:41.000000 haskellian-0.3.0/src/haskellian/pipe/pipe.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:05:34.872662 haskellian-0.3.0/src/haskellian/promise/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 14:06:21.000000 haskellian-0.3.0/src/haskellian/promise/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      245 2024-04-21 14:17:00.000000 haskellian-0.3.0/src/haskellian/promise/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1150 2024-04-21 14:12:47.000000 haskellian-0.3.0/src/haskellian/promise/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      480 2024-04-21 14:17:11.000000 haskellian-0.3.0/src/haskellian/promise/lifting.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      600 2024-04-21 14:35:57.000000 haskellian-0.3.0/src/haskellian/promise/managed.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1053 2024-04-21 14:21:51.000000 haskellian-0.3.0/src/haskellian/promise/promise.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:05:34.872662 haskellian-0.3.0/src/haskellian/thunk/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       24 2024-04-21 10:06:39.000000 haskellian-0.3.0/src/haskellian/thunk/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      933 2024-04-21 14:05:41.000000 haskellian-0.3.0/src/haskellian/thunk/thunk.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:05:34.872662 haskellian-0.3.0/src/haskellian.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1425 2024-04-21 15:05:34.000000 haskellian-0.3.0/src/haskellian.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1561 2024-04-21 15:05:34.000000 haskellian-0.3.0/src/haskellian.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-21 15:05:34.000000 haskellian-0.3.0/src/haskellian.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-04-21 15:05:34.000000 haskellian-0.3.0/src/haskellian.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-21 15:05:34.000000 haskellian-0.3.0/src/haskellian.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:09:33.772662 haskellian-0.3.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1425 2024-04-21 15:09:33.772662 haskellian-0.3.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1040 2024-04-21 15:09:09.000000 haskellian-0.3.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-04-21 15:09:31.000000 haskellian-0.3.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-21 15:09:33.772662 haskellian-0.3.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:09:33.752662 haskellian-0.3.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:09:33.762662 haskellian-0.3.1/src/haskellian/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      156 2024-04-21 08:31:50.000000 haskellian-0.3.1/src/haskellian/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      494 2024-04-21 14:43:52.000000 haskellian-0.3.1/src/haskellian/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:09:33.762662 haskellian-0.3.1/src/haskellian/asyn_iter/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 14:25:49.000000 haskellian-0.3.1/src/haskellian/asyn_iter/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      441 2024-04-21 14:39:06.000000 haskellian-0.3.1/src/haskellian/asyn_iter/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2234 2024-04-21 14:39:41.000000 haskellian-0.3.1/src/haskellian/asyn_iter/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2125 2024-04-21 14:40:29.000000 haskellian-0.3.1/src/haskellian/asyn_iter/iter.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      490 2024-04-21 14:38:54.000000 haskellian-0.3.1/src/haskellian/asyn_iter/lifting.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      886 2024-04-21 14:38:19.000000 haskellian-0.3.1/src/haskellian/asyn_iter/managed.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      650 2024-04-21 14:40:28.000000 haskellian-0.3.1/src/haskellian/asyn_iter/prefetching.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:09:33.762662 haskellian-0.3.1/src/haskellian/classes/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 09:04:50.000000 haskellian-0.3.1/src/haskellian/classes/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      137 2024-04-21 09:04:51.000000 haskellian-0.3.1/src/haskellian/classes/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      578 2024-04-21 10:23:51.000000 haskellian-0.3.1/src/haskellian/classes/applicative.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      413 2024-04-21 10:23:57.000000 haskellian-0.3.1/src/haskellian/classes/functor.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      832 2024-04-21 14:05:41.000000 haskellian-0.3.1/src/haskellian/classes/monad.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-04-21 15:09:01.000000 haskellian-0.3.1/src/haskellian/config.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:09:33.762662 haskellian-0.3.1/src/haskellian/either/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 10:31:26.000000 haskellian-0.3.1/src/haskellian/either/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      405 2024-04-21 10:39:57.000000 haskellian-0.3.1/src/haskellian/either/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2644 2024-04-21 14:05:41.000000 haskellian-0.3.1/src/haskellian/either/either.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1285 2024-04-21 10:38:12.000000 haskellian-0.3.1/src/haskellian/either/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      381 2024-04-21 10:36:36.000000 haskellian-0.3.1/src/haskellian/either/narrowing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      464 2024-04-21 10:39:34.000000 haskellian-0.3.1/src/haskellian/either/pydantic.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:09:33.762662 haskellian-0.3.1/src/haskellian/iter/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 13:06:20.000000 haskellian-0.3.1/src/haskellian/iter/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      593 2024-04-21 13:51:40.000000 haskellian-0.3.1/src/haskellian/iter/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      799 2024-04-21 13:51:48.000000 haskellian-0.3.1/src/haskellian/iter/basics.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      680 2024-04-21 13:53:19.000000 haskellian-0.3.1/src/haskellian/iter/batching.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      485 2024-04-21 13:53:13.000000 haskellian-0.3.1/src/haskellian/iter/indexing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2342 2024-04-21 14:41:28.000000 haskellian-0.3.1/src/haskellian/iter/iter.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      473 2024-04-21 13:52:51.000000 haskellian-0.3.1/src/haskellian/iter/lifting.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4144 2024-04-21 13:58:56.000000 haskellian-0.3.1/src/haskellian/iter/nested.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1140 2024-04-21 13:59:18.000000 haskellian-0.3.1/src/haskellian/iter/slicing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1003 2024-04-21 13:59:47.000000 haskellian-0.3.1/src/haskellian/iter/zipping.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:09:33.762662 haskellian-0.3.1/src/haskellian/pipe/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       22 2024-04-21 10:07:57.000000 haskellian-0.3.1/src/haskellian/pipe/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      767 2024-04-21 14:05:41.000000 haskellian-0.3.1/src/haskellian/pipe/pipe.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:09:33.772662 haskellian-0.3.1/src/haskellian/promise/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 14:06:21.000000 haskellian-0.3.1/src/haskellian/promise/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      245 2024-04-21 14:17:00.000000 haskellian-0.3.1/src/haskellian/promise/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1150 2024-04-21 14:12:47.000000 haskellian-0.3.1/src/haskellian/promise/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      480 2024-04-21 14:17:11.000000 haskellian-0.3.1/src/haskellian/promise/lifting.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      600 2024-04-21 14:35:57.000000 haskellian-0.3.1/src/haskellian/promise/managed.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1053 2024-04-21 14:21:51.000000 haskellian-0.3.1/src/haskellian/promise/promise.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:09:33.772662 haskellian-0.3.1/src/haskellian/thunk/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       24 2024-04-21 10:06:39.000000 haskellian-0.3.1/src/haskellian/thunk/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      933 2024-04-21 14:05:41.000000 haskellian-0.3.1/src/haskellian/thunk/thunk.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 15:09:33.772662 haskellian-0.3.1/src/haskellian.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1425 2024-04-21 15:09:33.000000 haskellian-0.3.1/src/haskellian.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1561 2024-04-21 15:09:33.000000 haskellian-0.3.1/src/haskellian.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-21 15:09:33.000000 haskellian-0.3.1/src/haskellian.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-04-21 15:09:33.000000 haskellian-0.3.1/src/haskellian.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-21 15:09:33.000000 haskellian-0.3.1/src/haskellian.egg-info/top_level.txt
```

### Comparing `haskellian-0.3.0/PKG-INFO` & `haskellian-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haskellian
-Version: 0.3.0
+Version: 0.3.1
 Summary: The functional programming library you need
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/haskellian.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Provides-Extra: pydantic
```

### Comparing `haskellian-0.3.0/README.md` & `haskellian-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/pyproject.toml` & `haskellian-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "haskellian"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "The functional programming library you need"
 dependencies = [
   "lazy-loader"
 ]
```

### Comparing `haskellian-0.3.0/src/haskellian/asyn_iter/funcs.py` & `haskellian-0.3.1/src/haskellian/asyn_iter/funcs.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/asyn_iter/iter.py` & `haskellian-0.3.1/src/haskellian/asyn_iter/iter.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/asyn_iter/managed.py` & `haskellian-0.3.1/src/haskellian/asyn_iter/managed.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/asyn_iter/prefetching.py` & `haskellian-0.3.1/src/haskellian/asyn_iter/prefetching.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/classes/applicative.py` & `haskellian-0.3.1/src/haskellian/classes/applicative.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/classes/monad.py` & `haskellian-0.3.1/src/haskellian/classes/monad.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/either/either.py` & `haskellian-0.3.1/src/haskellian/either/either.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/either/funcs.py` & `haskellian-0.3.1/src/haskellian/either/funcs.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/iter/__init__.pyi` & `haskellian-0.3.1/src/haskellian/iter/__init__.pyi`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/iter/basics.py` & `haskellian-0.3.1/src/haskellian/iter/basics.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/iter/batching.py` & `haskellian-0.3.1/src/haskellian/iter/batching.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/iter/iter.py` & `haskellian-0.3.1/src/haskellian/iter/iter.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/iter/nested.py` & `haskellian-0.3.1/src/haskellian/iter/nested.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/iter/slicing.py` & `haskellian-0.3.1/src/haskellian/iter/slicing.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/iter/zipping.py` & `haskellian-0.3.1/src/haskellian/iter/zipping.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/pipe/pipe.py` & `haskellian-0.3.1/src/haskellian/pipe/pipe.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/promise/funcs.py` & `haskellian-0.3.1/src/haskellian/promise/funcs.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/promise/managed.py` & `haskellian-0.3.1/src/haskellian/promise/managed.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/promise/promise.py` & `haskellian-0.3.1/src/haskellian/promise/promise.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian/thunk/thunk.py` & `haskellian-0.3.1/src/haskellian/thunk/thunk.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.0/src/haskellian.egg-info/PKG-INFO` & `haskellian-0.3.1/src/haskellian.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haskellian
-Version: 0.3.0
+Version: 0.3.1
 Summary: The functional programming library you need
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/haskellian.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Provides-Extra: pydantic
```

### Comparing `haskellian-0.3.0/src/haskellian.egg-info/SOURCES.txt` & `haskellian-0.3.1/src/haskellian.egg-info/SOURCES.txt`

 * *Files identical despite different names*


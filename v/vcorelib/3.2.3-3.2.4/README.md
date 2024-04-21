# Comparing `tmp/vcorelib-3.2.3.tar.gz` & `tmp/vcorelib-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcorelib-3.2.3.tar", last modified: Sat Apr 13 22:02:19 2024, max compression
+gzip compressed data, was "vcorelib-3.2.4.tar", last modified: Sun Apr 21 06:02:51 2024, max compression
```

## Comparing `vcorelib-3.2.3.tar` & `vcorelib-3.2.4.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.243593 vcorelib-3.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-13 22:00:53.000000 vcorelib-3.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-13 22:02:19.243593 vcorelib-3.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-13 22:00:53.000000 vcorelib-3.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-13 22:00:53.000000 vcorelib-3.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 22:02:19.243593 vcorelib-3.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-13 22:00:53.000000 vcorelib-3.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.227593 vcorelib-3.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-13 22:00:53.000000 vcorelib-3.2.3/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-13 22:00:53.000000 vcorelib-3.2.3/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.227593 vcorelib-3.2.3/vcorelib/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.231593 vcorelib-3.2.3/vcorelib/args/
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/args/newline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.231593 vcorelib-3.2.3/vcorelib/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/asyncio/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/asyncio/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.231593 vcorelib-3.2.3/vcorelib/dict/
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/dict/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/dict/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/dict/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/dict/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.231593 vcorelib-3.2.3/vcorelib/graph/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7436 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/graph/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/graph/port.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.231593 vcorelib-3.2.3/vcorelib/io/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/io/arbiter/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/arbiter/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/arbiter/directory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/io/archive/
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/fifo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/file_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/logging/args.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/logging/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/math/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/math/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/analysis/average.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/analysis/buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/math/analysis/rate/
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/analysis/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/analysis/rate/limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/analysis/weighted.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/namespace/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/namespace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/namespace/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/namespace/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/paths/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/paths/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/paths/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/paths/find.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/paths/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/paths/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/paths/info_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/platform/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/python.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/schemas/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/schemas/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/script/
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.239593 vcorelib-3.2.3/vcorelib/target/
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/target/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/target/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/target/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.239593 vcorelib-3.2.3/vcorelib/task/
--rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.239593 vcorelib-3.2.3/vcorelib/task/dict/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/task/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/task/dict/melder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/task/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.239593 vcorelib-3.2.3/vcorelib/task/subprocess/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/task/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/task/subprocess/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.239593 vcorelib-3.2.3/vcorelib/task/time/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/task/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/task/time/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.239593 vcorelib-3.2.3/vcorelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-13 22:02:19.000000 vcorelib-3.2.3/vcorelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-13 22:02:19.000000 vcorelib-3.2.3/vcorelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 22:02:19.000000 vcorelib-3.2.3/vcorelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-13 22:02:19.000000 vcorelib-3.2.3/vcorelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 22:02:19.000000 vcorelib-3.2.3/vcorelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.620720 vcorelib-3.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-21 06:01:27.000000 vcorelib-3.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-21 06:02:51.620720 vcorelib-3.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-21 06:01:27.000000 vcorelib-3.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-21 06:01:27.000000 vcorelib-3.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 06:02:51.620720 vcorelib-3.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-21 06:01:27.000000 vcorelib-3.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.604720 vcorelib-3.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-21 06:01:27.000000 vcorelib-3.2.4/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-21 06:01:27.000000 vcorelib-3.2.4/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.604720 vcorelib-3.2.4/vcorelib/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.608720 vcorelib-3.2.4/vcorelib/args/
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/args/newline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.608720 vcorelib-3.2.4/vcorelib/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/asyncio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/asyncio/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.608720 vcorelib-3.2.4/vcorelib/dict/
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/dict/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/dict/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/dict/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/dict/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.608720 vcorelib-3.2.4/vcorelib/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7436 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/graph/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/graph/port.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.608720 vcorelib-3.2.4/vcorelib/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/io/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.612721 vcorelib-3.2.4/vcorelib/io/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/io/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/io/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/io/arbiter/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/io/arbiter/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.612721 vcorelib-3.2.4/vcorelib/io/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/io/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/io/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/io/decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/io/encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/io/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/io/file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/io/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/io/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.612721 vcorelib-3.2.4/vcorelib/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/logging/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/logging/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.612721 vcorelib-3.2.4/vcorelib/math/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/math/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.612721 vcorelib-3.2.4/vcorelib/math/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/math/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/math/analysis/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/math/analysis/buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.612721 vcorelib-3.2.4/vcorelib/math/analysis/rate/
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/math/analysis/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/math/analysis/rate/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/math/analysis/weighted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/math/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/math/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/math/unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.612721 vcorelib-3.2.4/vcorelib/namespace/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/namespace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/namespace/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/namespace/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.616721 vcorelib-3.2.4/vcorelib/paths/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/paths/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/paths/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/paths/find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/paths/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/paths/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/paths/info_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.616721 vcorelib-3.2.4/vcorelib/platform/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.616721 vcorelib-3.2.4/vcorelib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/schemas/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/schemas/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.616721 vcorelib-3.2.4/vcorelib/script/
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.616721 vcorelib-3.2.4/vcorelib/target/
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/target/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/target/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/target/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.616721 vcorelib-3.2.4/vcorelib/task/
+-rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.616721 vcorelib-3.2.4/vcorelib/task/dict/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/task/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/task/dict/melder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/task/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.616721 vcorelib-3.2.4/vcorelib/task/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/task/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/task/subprocess/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.616721 vcorelib-3.2.4/vcorelib/task/time/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/task/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-21 06:01:27.000000 vcorelib-3.2.4/vcorelib/task/time/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:02:51.620720 vcorelib-3.2.4/vcorelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-21 06:02:51.000000 vcorelib-3.2.4/vcorelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-21 06:02:51.000000 vcorelib-3.2.4/vcorelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 06:02:51.000000 vcorelib-3.2.4/vcorelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-21 06:02:51.000000 vcorelib-3.2.4/vcorelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 06:02:51.000000 vcorelib-3.2.4/vcorelib.egg-info/top_level.txt
```

### Comparing `vcorelib-3.2.3/LICENSE` & `vcorelib-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/PKG-INFO` & `vcorelib-3.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 3.2.3
+Version: 3.2.4
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -15,18 +15,18 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tomli
 Requires-Dist: cerberus
-Requires-Dist: importlib-resources
 Requires-Dist: fastjsonschema
 Requires-Dist: ruamel.yaml
 Requires-Dist: tomli-w
+Requires-Dist: importlib-resources
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -40,19 +40,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=f8b97332b3af92a47a234fed499d57a3
+    hash=bc0b27e02d365bc98f792016fb5c40a1
     =====================================
 -->
 
-# vcorelib ([3.2.3](https://pypi.org/project/vcorelib/))
+# vcorelib ([3.2.4](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-3.2.3/README.md` & `vcorelib-3.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=f8b97332b3af92a47a234fed499d57a3
+    hash=bc0b27e02d365bc98f792016fb5c40a1
     =====================================
 -->
 
-# vcorelib ([3.2.3](https://pypi.org/project/vcorelib/))
+# vcorelib ([3.2.4](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-3.2.3/pyproject.toml` & `vcorelib-3.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "vcorelib"
-version = "3.2.3"
+version = "3.2.4"
 description = "A collection of core Python utilities."
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `vcorelib-3.2.3/setup.py` & `vcorelib-3.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/tests/test_names.py` & `vcorelib-3.2.4/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/args/__init__.py` & `vcorelib-3.2.4/vcorelib/args/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/args/newline.py` & `vcorelib-3.2.4/vcorelib/args/newline.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/asyncio/__init__.py` & `vcorelib-3.2.4/vcorelib/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/asyncio/cli.py` & `vcorelib-3.2.4/vcorelib/asyncio/cli.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/asyncio/subprocess.py` & `vcorelib-3.2.4/vcorelib/asyncio/subprocess.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/dict/__init__.py` & `vcorelib-3.2.4/vcorelib/dict/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/dict/cache.py` & `vcorelib-3.2.4/vcorelib/dict/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/dict/codec.py` & `vcorelib-3.2.4/vcorelib/dict/codec.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/dict/config.py` & `vcorelib-3.2.4/vcorelib/dict/config.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/dict/env.py` & `vcorelib-3.2.4/vcorelib/dict/env.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/graph/__init__.py` & `vcorelib-3.2.4/vcorelib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/graph/abc.py` & `vcorelib-3.2.4/vcorelib/graph/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/graph/edge.py` & `vcorelib-3.2.4/vcorelib/graph/edge.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/graph/node.py` & `vcorelib-3.2.4/vcorelib/graph/node.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/graph/port.py` & `vcorelib-3.2.4/vcorelib/graph/port.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/io/__init__.py` & `vcorelib-3.2.4/vcorelib/io/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/io/abc.py` & `vcorelib-3.2.4/vcorelib/io/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/io/arbiter/base.py` & `vcorelib-3.2.4/vcorelib/io/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/io/arbiter/context.py` & `vcorelib-3.2.4/vcorelib/io/arbiter/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/io/arbiter/directory.py` & `vcorelib-3.2.4/vcorelib/io/arbiter/directory.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/io/archive/__init__.py` & `vcorelib-3.2.4/vcorelib/io/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/io/cache.py` & `vcorelib-3.2.4/vcorelib/io/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/io/decode.py` & `vcorelib-3.2.4/vcorelib/io/decode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/io/encode.py` & `vcorelib-3.2.4/vcorelib/io/encode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/io/fifo.py` & `vcorelib-3.2.4/vcorelib/io/fifo.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/io/file_writer.py` & `vcorelib-3.2.4/vcorelib/io/file_writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 A module implementing an interface for writing to variably indented files.
 """
 
 # built-in
 from contextlib import contextmanager
 from enum import Enum, auto
 from io import StringIO
-from os import linesep
+import os
 from pathlib import Path
 from typing import Iterator, List, Optional, TextIO, Tuple
 
 # internal
 from vcorelib import DEFAULT_ENCODING
 from vcorelib.paths.context import tempfile
 
@@ -45,26 +45,29 @@
     def __init__(
         self,
         stream: TextIO,
         space: str = " ",
         per_indent: int = 1,
         prefix: str = "",
         suffix: str = "",
+        linesep: str = os.linesep,
     ) -> None:
         """Initialize this instance."""
 
         self.stream = stream
         self.space = space
         self.per_indent = per_indent
         self.depth = 0
         self.position = 0
 
         self._prefix = prefix
         self._suffix = suffix
 
+        self.linesep = linesep
+
     @contextmanager
     def prefix(self, prefix: str) -> Iterator[None]:
         """Set a new line prefix as a managed context."""
 
         curr = self._prefix
         self._prefix = prefix
         try:
@@ -89,21 +92,21 @@
         with self.prefix(prefix):
             with self.suffix(suffix):
                 yield
 
     @staticmethod
     @contextmanager
     def from_path(
-        path: Path, space: str = " ", per_indent: int = 1
+        path: Path, space: str = " ", per_indent: int = 1, **kwargs
     ) -> Iterator["IndentedFileWriter"]:
         """Create an instance from a path as a managed context."""
 
         with path.open("w", encoding=DEFAULT_ENCODING) as stream:
             yield IndentedFileWriter(
-                stream, space=space, per_indent=per_indent
+                stream, space=space, per_indent=per_indent, **kwargs
             )
 
     @staticmethod
     @contextmanager
     def string(
         space: str = " ", per_indent: int = 1
     ) -> Iterator["IndentedFileWriter"]:
@@ -113,21 +116,21 @@
             yield IndentedFileWriter(
                 stream, space=space, per_indent=per_indent
             )
 
     @staticmethod
     @contextmanager
     def temporary(
-        space: str = " ", per_indent: int = 1
+        space: str = " ", per_indent: int = 1, **kwargs
     ) -> Iterator["IndentedFileWriter"]:
         """Create an instance from a temporary file as a managed context."""
 
         with tempfile() as tmp:
             with IndentedFileWriter.from_path(
-                tmp, space=space, per_indent=per_indent
+                tmp, space=space, per_indent=per_indent, **kwargs
             ) as writer:
                 yield writer
 
     def write(self, data: str) -> int:
         """
         method taking the str data for a new line of text to write
         to the file: first writes the indent (some number of
@@ -140,15 +143,15 @@
             line_data = self._prefix + line + self._suffix
 
             # Don't write the indent if the line data is empty.
             indent = (
                 self.space * self.depth * self.per_indent if line_data else ""
             )
 
-            line = (indent + line_data).rstrip() + linesep
+            line = (indent + line_data).rstrip() + self.linesep
 
             self.stream.write(line)
             count += len(line)
 
         self.position += count
         return count
```

### Comparing `vcorelib-3.2.3/vcorelib/io/mapping.py` & `vcorelib-3.2.4/vcorelib/io/mapping.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/io/types.py` & `vcorelib-3.2.4/vcorelib/io/types.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/logging/__init__.py` & `vcorelib-3.2.4/vcorelib/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/logging/args.py` & `vcorelib-3.2.4/vcorelib/logging/args.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/logging/time.py` & `vcorelib-3.2.4/vcorelib/logging/time.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/math/__init__.py` & `vcorelib-3.2.4/vcorelib/math/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/math/analysis/average.py` & `vcorelib-3.2.4/vcorelib/math/analysis/average.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/math/analysis/buffer.py` & `vcorelib-3.2.4/vcorelib/math/analysis/buffer.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/math/analysis/rate/__init__.py` & `vcorelib-3.2.4/vcorelib/math/analysis/rate/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/math/analysis/rate/limiter.py` & `vcorelib-3.2.4/vcorelib/math/analysis/rate/limiter.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/math/analysis/weighted.py` & `vcorelib-3.2.4/vcorelib/math/analysis/weighted.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/math/time.py` & `vcorelib-3.2.4/vcorelib/math/time.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/math/unit.py` & `vcorelib-3.2.4/vcorelib/math/unit.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/names.py` & `vcorelib-3.2.4/vcorelib/names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/namespace/base.py` & `vcorelib-3.2.4/vcorelib/namespace/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/namespace/mixin.py` & `vcorelib-3.2.4/vcorelib/namespace/mixin.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/paths/__init__.py` & `vcorelib-3.2.4/vcorelib/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/paths/base.py` & `vcorelib-3.2.4/vcorelib/paths/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/paths/context.py` & `vcorelib-3.2.4/vcorelib/paths/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/paths/find.py` & `vcorelib-3.2.4/vcorelib/paths/find.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/paths/hashing.py` & `vcorelib-3.2.4/vcorelib/paths/hashing.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/paths/info.py` & `vcorelib-3.2.4/vcorelib/paths/info.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/paths/info_cache.py` & `vcorelib-3.2.4/vcorelib/paths/info_cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/platform/__init__.py` & `vcorelib-3.2.4/vcorelib/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/python.py` & `vcorelib-3.2.4/vcorelib/python.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/schemas/__init__.py` & `vcorelib-3.2.4/vcorelib/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/schemas/base.py` & `vcorelib-3.2.4/vcorelib/schemas/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/schemas/json.py` & `vcorelib-3.2.4/vcorelib/schemas/json.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/schemas/mixins.py` & `vcorelib-3.2.4/vcorelib/schemas/mixins.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/script/__init__.py` & `vcorelib-3.2.4/vcorelib/script/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/target/__init__.py` & `vcorelib-3.2.4/vcorelib/target/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/target/evaluation.py` & `vcorelib-3.2.4/vcorelib/target/evaluation.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/target/expression.py` & `vcorelib-3.2.4/vcorelib/target/expression.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/target/resolver.py` & `vcorelib-3.2.4/vcorelib/target/resolver.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/task/__init__.py` & `vcorelib-3.2.4/vcorelib/task/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/task/dict/melder.py` & `vcorelib-3.2.4/vcorelib/task/dict/melder.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/task/manager.py` & `vcorelib-3.2.4/vcorelib/task/manager.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/task/subprocess/run.py` & `vcorelib-3.2.4/vcorelib/task/subprocess/run.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib/task/time/sleep.py` & `vcorelib-3.2.4/vcorelib/task/time/sleep.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.3/vcorelib.egg-info/PKG-INFO` & `vcorelib-3.2.4/vcorelib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 3.2.3
+Version: 3.2.4
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -15,18 +15,18 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tomli
 Requires-Dist: cerberus
-Requires-Dist: importlib-resources
 Requires-Dist: fastjsonschema
 Requires-Dist: ruamel.yaml
 Requires-Dist: tomli-w
+Requires-Dist: importlib-resources
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -40,19 +40,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=f8b97332b3af92a47a234fed499d57a3
+    hash=bc0b27e02d365bc98f792016fb5c40a1
     =====================================
 -->
 
-# vcorelib ([3.2.3](https://pypi.org/project/vcorelib/))
+# vcorelib ([3.2.4](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-3.2.3/vcorelib.egg-info/SOURCES.txt` & `vcorelib-3.2.4/vcorelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*


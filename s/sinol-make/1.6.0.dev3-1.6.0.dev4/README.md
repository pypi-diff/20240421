# Comparing `tmp/sinol_make-1.6.0.dev3.tar.gz` & `tmp/sinol_make-1.6.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinol_make-1.6.0.dev3.tar", last modified: Thu Apr  4 21:18:57 2024, max compression
+gzip compressed data, was "sinol_make-1.6.0.dev4.tar", last modified: Fri Apr  5 14:53:11 2024, max compression
```

## Comparing `sinol_make-1.6.0.dev3.tar` & `sinol_make-1.6.0.dev4.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.391683 sinol_make-1.6.0.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-04 21:18:57.391683 sinol_make-1.6.0.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-04 21:18:57.391683 sinol_make-1.6.0.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.379683 sinol_make-1.6.0.dev3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.379683 sinol_make-1.6.0.dev3/src/sinol_make/
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.379683 sinol_make-1.6.0.dev3/src/sinol_make/commands/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/doc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/export/
--rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/gen/
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/gen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/ingen/
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/ingen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/ingen/ingen_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/init/
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/init/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/inwer/
--rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/inwer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/inwer/inwer_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/outgen/
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/outgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/outgen/outgen_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/run/
--rw-r--r--   0 runner    (1001) docker     (127)    57981 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/verify/
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/verify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/contest_types/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/contest_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/contest_types/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/contest_types/icpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/contest_types/oi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.387683 sinol_make-1.6.0.dev3/src/sinol_make/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/helpers/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/helpers/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/helpers/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14656 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/helpers/package_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/helpers/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/helpers/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/helpers/printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.387683 sinol_make-1.6.0.dev3/src/sinol_make/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/interfaces/BaseCommand.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/interfaces/Errors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.387683 sinol_make-1.6.0.dev3/src/sinol_make/oiejq/
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/oiejq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/oiejq/perf_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.387683 sinol_make-1.6.0.dev3/src/sinol_make/structs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/structs/cache_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/structs/compiler_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/structs/gen_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/structs/inwer_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/structs/run_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/structs/status_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13924 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.387683 sinol_make-1.6.0.dev3/src/sinol_make.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-04 21:18:57.000000 sinol_make-1.6.0.dev3/src/sinol_make.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-04 21:18:57.000000 sinol_make-1.6.0.dev3/src/sinol_make.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:18:57.000000 sinol_make-1.6.0.dev3/src/sinol_make.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 21:18:57.000000 sinol_make-1.6.0.dev3/src/sinol_make.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 21:18:57.000000 sinol_make-1.6.0.dev3/src/sinol_make.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 21:18:57.000000 sinol_make-1.6.0.dev3/src/sinol_make.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.387683 sinol_make-1.6.0.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/tests/test_multiple_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/tests/test_oiejq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.102414 sinol_make-1.6.0.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-05 14:53:11.102414 sinol_make-1.6.0.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-05 14:53:11.102414 sinol_make-1.6.0.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.090414 sinol_make-1.6.0.dev4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.090414 sinol_make-1.6.0.dev4/src/sinol_make/
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.090414 sinol_make-1.6.0.dev4/src/sinol_make/commands/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.094414 sinol_make-1.6.0.dev4/src/sinol_make/commands/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/commands/doc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.094414 sinol_make-1.6.0.dev4/src/sinol_make/commands/export/
+-rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/commands/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.094414 sinol_make-1.6.0.dev4/src/sinol_make/commands/gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/commands/gen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.094414 sinol_make-1.6.0.dev4/src/sinol_make/commands/ingen/
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/commands/ingen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/commands/ingen/ingen_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.094414 sinol_make-1.6.0.dev4/src/sinol_make/commands/init/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/commands/init/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.094414 sinol_make-1.6.0.dev4/src/sinol_make/commands/inwer/
+-rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/commands/inwer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/commands/inwer/inwer_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.094414 sinol_make-1.6.0.dev4/src/sinol_make/commands/outgen/
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/commands/outgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/commands/outgen/outgen_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.094414 sinol_make-1.6.0.dev4/src/sinol_make/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (127)    58273 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/commands/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.094414 sinol_make-1.6.0.dev4/src/sinol_make/commands/verify/
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/commands/verify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.094414 sinol_make-1.6.0.dev4/src/sinol_make/contest_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/contest_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/contest_types/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/contest_types/icpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/contest_types/oi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.098414 sinol_make-1.6.0.dev4/src/sinol_make/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/helpers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/helpers/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/helpers/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/helpers/func_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15495 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/helpers/package_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/helpers/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/helpers/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/helpers/printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.098414 sinol_make-1.6.0.dev4/src/sinol_make/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/interfaces/BaseCommand.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/interfaces/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.098414 sinol_make-1.6.0.dev4/src/sinol_make/oiejq/
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/oiejq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/oiejq/perf_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.098414 sinol_make-1.6.0.dev4/src/sinol_make/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/structs/cache_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/structs/compiler_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/structs/gen_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/structs/inwer_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/structs/run_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/structs/status_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13838 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/src/sinol_make/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.098414 sinol_make-1.6.0.dev4/src/sinol_make.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-05 14:53:11.000000 sinol_make-1.6.0.dev4/src/sinol_make.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-05 14:53:11.000000 sinol_make-1.6.0.dev4/src/sinol_make.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:53:11.000000 sinol_make-1.6.0.dev4/src/sinol_make.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 14:53:11.000000 sinol_make-1.6.0.dev4/src/sinol_make.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-05 14:53:11.000000 sinol_make-1.6.0.dev4/src/sinol_make.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 14:53:11.000000 sinol_make-1.6.0.dev4/src/sinol_make.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:53:11.098414 sinol_make-1.6.0.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/tests/test_multiple_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/tests/test_oiejq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-05 14:53:03.000000 sinol_make-1.6.0.dev4/tests/test_util.py
```

### Comparing `sinol_make-1.6.0.dev3/LICENSE` & `sinol_make-1.6.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/PKG-INFO` & `sinol_make-1.6.0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol_make
-Version: 1.6.0.dev3
+Version: 1.6.0.dev4
 Summary: CLI tool for creating sio2 task packages
 Author: Mateusz Masiarz
 Author-email: m.masiarz@fri.edu.pl
 Maintainer: Tomasz Nowak, Mateusz Masiarz
 Maintainer-email: tomasz.nowak@tonowak.com, m.masiarz@fri.edu.pl
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
```

### Comparing `sinol_make-1.6.0.dev3/README.md` & `sinol_make-1.6.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/setup.cfg` & `sinol_make-1.6.0.dev4/setup.cfg`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/__init__.py` & `sinol_make-1.6.0.dev4/src/sinol_make/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import argparse
 import traceback
 import argcomplete
 
 from sinol_make import util, oiejq
 
-__version__ = "1.6.0.dev3"
+__version__ = "1.6.0.dev4"
 
 
 def configure_parsers():
     parser = argparse.ArgumentParser(
         prog='sinol-make',
         description='Tool for creating and testing sio2 tasks',
     )
@@ -46,36 +46,38 @@
             util.exit_with_error('`oiejq` could not be installed.\n' + str(err))
 
 
 def main_exn():
     parser = configure_parsers()
     arguments = []
     curr_args = []
+    commands = util.get_commands()
+    commands_dict = {command.get_name(): command for command in commands}
     for arg in sys.argv[1:]:
-        if arg in util.get_command_names() and not (len(curr_args) > 0 and curr_args[0] == 'init'):
+        if arg in commands_dict.keys() and not (len(curr_args) > 0 and curr_args[0] == 'init'):
             if curr_args:
                 arguments.append(curr_args)
             curr_args = [arg]
         else:
             curr_args.append(arg)
     if curr_args:
         arguments.append(curr_args)
-    commands = util.get_commands()
+    if not arguments:
+        parser.print_help()
+        exit(1)
     check_oiejq()
 
     for curr_args in arguments:
         args = parser.parse_args(curr_args)
-        command_found = False
-        for command in commands:
-            if command.get_name() == args.command:
-                command_found = True
-                if len(arguments) > 1:
-                    print(f' {command.get_name()} command '.center(util.get_terminal_size()[1], '='))
-                command.run(args)
-        if not command_found:
+        command = commands_dict.get(args.command, None)
+        if command:
+            if len(arguments) > 1:
+                print(f' {command.get_name()} command '.center(util.get_terminal_size()[1], '='))
+            command.run(args)
+        else:
             parser.print_help()
             exit(1)
 
 
 def main():
     new_version = None
     try:
```

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/commands/doc/__init__.py` & `sinol_make-1.6.0.dev4/src/sinol_make/commands/doc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
     LOG_PATTERNS = ['*~', '*.aux', '*.log', '*.dvi', '*.err', '*.inf']
 
     def get_name(self):
         return "doc"
 
     def compile_file_latex_div(self, file_path):
-        print(util.info(f'Compiling {os.path.basename(file_path)} (latex to dvi)...'))
+        print(f'Compiling {os.path.basename(file_path)} (latex to dvi)...')
         os.chdir(os.path.dirname(file_path))
         subprocess.run(['latex', file_path])
         dvi_file = os.path.splitext(file_path)[0] + '.dvi'
         dvi_file_path = os.path.join(os.path.dirname(file_path), dvi_file)
         if not os.path.exists(dvi_file_path):
             print(util.error('Compilation failed.'))
             return False
@@ -31,15 +31,15 @@
         if process.returncode != 0:
             print(util.error('Compilation failed.'))
             return False
         print(util.info(f'Compilation successful for file {os.path.basename(file_path)}.'))
         return True
 
     def compile_pdf_latex(self, file_path):
-        print(util.info(f'Compiling {os.path.basename(file_path)} (pdflatex)...'))
+        print(f'Compiling {os.path.basename(file_path)} (pdflatex)...')
         os.chdir(os.path.dirname(file_path))
         subprocess.run(['pdflatex', file_path])
         pdf_file = os.path.splitext(file_path)[0] + '.pdf'
         pdf_file_path = os.path.join(os.path.dirname(file_path), pdf_file)
         if not os.path.exists(pdf_file_path):
             print(util.error('Compilation failed.'))
             return False
@@ -58,15 +58,15 @@
 
     def move_logs(self):
         output_dir = paths.get_cache_path('doc_logs')
         os.makedirs(output_dir, exist_ok=True)
         for pattern in self.LOG_PATTERNS:
             for file in glob.glob(os.path.join(os.getcwd(), 'doc', pattern)):
                 os.rename(file, os.path.join(output_dir, os.path.basename(file)))
-        print(util.info(f'Compilation log files can be found in {os.path.relpath(output_dir, os.getcwd())}'))
+        print(f'Compilation log files can be found in {os.path.relpath(output_dir, os.getcwd())}')
 
     def configure_subparser(self, subparser: argparse.ArgumentParser):
         parser = subparser.add_parser(
             self.get_name(),
             help='Compile latex files to pdf',
             description='Compiles latex files to pdf. By default compiles all files in the `doc` directory.\n'
                         'You can also specify files to compile.')
```

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/commands/export/__init__.py` & `sinol_make-1.6.0.dev4/src/sinol_make/commands/export/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,15 @@
         return "export"
 
     def configure_subparser(self, subparser: argparse.ArgumentParser):
         parser = subparser.add_parser(
             self.get_name(),
             help='Create archive for oioioi upload',
             description='Creates archive in the current directory ready to upload to sio2 or szkopul.')
-        parser.add_argument('-c', '--cpus', type=int,
-                            help=f'number of cpus to use to generate output files '
-                                 f'(default: {util.default_cpu_count()})',
-                            default=util.default_cpu_count())
+        parsers.add_cpus_argument(parser, 'number of cpus to use to generate output files')
         parser.add_argument('--no-statement', dest='no_statement', action='store_true',
                             help='allow export without statement')
         parser.add_argument('--export-ocen', dest='export_ocen', action='store_true',
                             help='Create ocen archive')
         parsers.add_compilation_arguments(parser)
         return parser
 
@@ -114,20 +111,22 @@
             num_tests = 0
             for ext in ['in', 'out']:
                 for test in glob.glob(os.path.join(tests_dir, ext, f'{self.task_id}0*.{ext}')) + \
                             glob.glob(os.path.join(tests_dir, ext, f'{self.task_id}*ocen.{ext}')):
                     shutil.copy(test, os.path.join(ocen_dir, ext, os.path.basename(test)))
                     num_tests += 1
 
+            dlazaw_dir = os.path.join(os.getcwd(), 'dlazaw')
             if num_tests == 0:
                 print(util.warning('No ocen tests found.'))
+            elif os.path.exists(dlazaw_dir):
+                print(util.warning('Skipping ocen arhive creation because dlazaw directory exists.'))
             else:
                 shutil.make_archive(os.path.join(attachments_dir, f'{self.task_id}ocen'), 'zip', tmpdir)
 
-            dlazaw_dir = os.path.join(os.getcwd(), 'dlazaw')
             if os.path.exists(dlazaw_dir):
                 print('Archiving dlazaw directory and adding to attachments.')
                 os.makedirs(os.path.join(tmpdir, 'dlazaw'), exist_ok=True)
                 shutil.copytree(dlazaw_dir, os.path.join(tmpdir, 'dlazaw', 'dlazaw'))
                 shutil.make_archive(os.path.join(attachments_dir, 'dlazaw'), 'zip',
                                     os.path.join(tmpdir, 'dlazaw'))
```

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/commands/gen/__init__.py` & `sinol_make-1.6.0.dev4/src/sinol_make/commands/gen/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,18 +27,15 @@
                         'file which will be used.'
         )
 
         parser.add_argument('ingen_path', type=str, nargs='?',
                             help='path to ingen source file, for example prog/abcingen.cpp')
         parser.add_argument('-i', '--only-inputs', action='store_true', help='generate input files only')
         parser.add_argument('-o', '--only-outputs', action='store_true', help='generate output files only')
-        parser.add_argument('-c', '--cpus', type=int,
-                            help=f'number of cpus to use to generate output files '
-                                 f'(default: {util.default_cpu_count()})',
-                            default=util.default_cpu_count())
+        parsers.add_cpus_argument(parser, 'number of cpus to use to generate output files')
         parser.add_argument('-n', '--no-validate', default=False, action='store_true',
                             help='do not validate test contents')
         parser.add_argument('-f', '--fsanitize', default=False, action='store_true',
                             help='Use -fsanitize=address,undefined for ingen compilation. Warning: this may fail on some '
                                  'systems. To fix this, run `sudo sysctl vm.mmap_rnd_bits = 28`.')
         parsers.add_compilation_arguments(parser)
         return parser
```

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/commands/ingen/__init__.py` & `sinol_make-1.6.0.dev4/src/sinol_make/commands/ingen/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,15 @@
                         'file which will be used.'
         )
 
         parser.add_argument('ingen_path', type=str, nargs='?',
                             help='path to ingen source file, for example prog/abcingen.cpp')
         parser.add_argument('-n', '--no-validate', default=False, action='store_true',
                             help='do not validate test contents')
+        parsers.add_cpus_argument(parser, 'number of cpus used for validating tests')
         parser.add_argument('-f', '--fsanitize', default=False, action='store_true',
                             help='Use -fsanitize=address,undefined for compilation. Warning: this may fail on some '
                                  'systems. Tof fix this, run `sudo sysctl vm.mmap_rnd_bits = 28`.')
         parsers.add_compilation_arguments(parser)
         return parser
 
     def run(self, args: argparse.Namespace):
@@ -41,15 +42,15 @@
 
         self.args = args
 
         self.task_id = package_util.get_task_id()
         package_util.validate_test_names(self.task_id)
         util.change_stack_size_to_unlimited()
         self.ingen = get_ingen(self.task_id, args.ingen_path)
-        print(util.info(f'Using ingen file {os.path.basename(self.ingen)}'))
+        print(f'Using ingen file {os.path.basename(self.ingen)}')
         self.ingen_exe = compile_ingen(self.ingen, self.args, self.args.compile_mode, self.args.fsanitize)
 
         previous_tests = []
         try:
             with open(paths.get_cache_path("input_tests"), "r") as f:
                 for line in f:
                     line = line.strip()
@@ -60,22 +61,19 @@
         dates = {os.path.basename(test): os.path.getmtime(test) for test in previous_tests}
 
         if run_ingen(self.ingen_exe):
             print(util.info('Successfully generated input files.'))
         else:
             util.exit_with_error('Failed to generate input files.')
 
-        print(util.info('Cleaning up old input files.'))
+        print('Cleaning up old input files.')
         for test in glob.glob(os.path.join(os.getcwd(), "in", f"{self.task_id}*.in")):
             basename = os.path.basename(test)
             if basename in dates and dates[basename] == os.path.getmtime(test):
                 os.unlink(test)
 
         with open(paths.get_cache_path("input_tests"), "w") as f:
             f.write("\n".join(glob.glob(os.path.join(os.getcwd(), "in", f"{self.task_id}*.in"))))
 
         if not self.args.no_validate:
-            print(util.info('Validating input test contents.'))
             tests = sorted(glob.glob(os.path.join(os.getcwd(), "in", f"{self.task_id}*.in")))
-            for test in tests:
-                package_util.validate_test(test)
-            print(util.info('Input test contents are valid!'))
+            package_util.validate_tests(tests, self.args.cpus, 'input')
```

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/commands/ingen/ingen_util.py` & `sinol_make-1.6.0.dev4/src/sinol_make/commands/ingen/ingen_util.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/commands/init/__init__.py` & `sinol_make-1.6.0.dev4/src/sinol_make/commands/init/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/commands/inwer/__init__.py` & `sinol_make-1.6.0.dev4/src/sinol_make/commands/inwer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 import os
 import multiprocessing as mp
 from functools import cmp_to_key
 from typing import Dict, List
 
 from sinol_make import util
 from sinol_make.structs.inwer_structs import TestResult, InwerExecution, VerificationResult, TableData
-from sinol_make.helpers import package_util, compile, printer, paths
-from sinol_make.helpers.parsers import add_compilation_arguments
+from sinol_make.helpers import package_util, printer, paths, parsers
 from sinol_make.interfaces.BaseCommand import BaseCommand
 from sinol_make.commands.inwer import inwer_util
 
 
 class Command(BaseCommand):
     """
     Class for "inwer" command.
@@ -33,20 +32,19 @@
                         'specify your inwer source file which will be used.'
         )
 
         parser.add_argument('inwer_path', type=str, nargs='?',
                             help='path to inwer source file, for example prog/abcinwer.cpp')
         parser.add_argument('-t', '--tests', type=str, nargs='+',
                             help='test to verify, for example in/abc{0,1}*')
-        parser.add_argument('-c', '--cpus', type=int,
-                            help=f'number of cpus to use (default: {util.default_cpu_count()})')
+        parsers.add_cpus_argument(parser, 'number of cpus to use when verifying tests')
         parser.add_argument('-f', '--fsanitize', default=False, action='store_true',
                             help='Use -fsanitize=address,undefined for compilation. Warning: this may fail on some '
                                  'systems. Tof fix this, run `sudo sysctl vm.mmap_rnd_bits = 28`.')
-        add_compilation_arguments(parser)
+        parsers.add_compilation_arguments(parser)
         return parser
 
     @staticmethod
     def verify_test(execution: InwerExecution) -> VerificationResult:
         """
         Verifies a test and returns the result of inwer on this test.
         """
```

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/commands/inwer/inwer_util.py` & `sinol_make-1.6.0.dev4/src/sinol_make/commands/inwer/inwer_util.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/commands/outgen/__init__.py` & `sinol_make-1.6.0.dev4/src/sinol_make/commands/outgen/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,19 +22,15 @@
 
     def configure_subparser(self, subparser):
         parser = subparser.add_parser(
             self.get_name(),
             help='Generate output files',
             description='Generate output files using the correct solution.'
         )
-
-        parser.add_argument('-c', '--cpus', type=int,
-                            help=f'number of cpus to use to generate output files '
-                                 f'(default: {util.default_cpu_count()})',
-                            default=util.default_cpu_count())
+        parsers.add_cpus_argument(parser, 'number of cpus to use to generate output files')
         parser.add_argument('-n', '--no-validate', default=False, action='store_true',
                             help='do not validate test contents')
         parsers.add_compilation_arguments(parser)
         return parser
 
     def generate_outputs(self, outputs_to_generate):
         print(f'Generating output files for {len(outputs_to_generate)} tests on {self.args.cpus} cpus.')
@@ -46,15 +42,15 @@
             arguments.append(OutputGenerationArguments(self.correct_solution_exe, input, output))
 
         with mp.Pool(self.args.cpus) as pool:
             results = []
             for i, result in enumerate(pool.imap(generate_output, arguments)):
                 results.append(result)
                 if result:
-                    print(util.info(f'Successfully generated output file {os.path.basename(arguments[i].output_test)}'))
+                    print(f'Successfully generated output file {os.path.basename(arguments[i].output_test)}')
                 else:
                     print(util.error(f'Failed to generate output file {os.path.basename(arguments[i].output_test)}'))
 
             if not all(results):
                 util.exit_with_error('Failed to generate some output files.')
             else:
                 print(util.info('Successfully generated all output files.'))
@@ -126,11 +122,8 @@
             self.correct_solution_exe = compile_correct_solution(self.correct_solution, self.args,
                                                                  self.args.compile_mode)
             self.generate_outputs(outputs_to_generate)
             with open(os.path.join(os.getcwd(), 'in', '.md5sums'), 'w') as f:
                 yaml.dump(md5_sums, f)
 
         if not self.args.no_validate:
-            print(util.info('Validating output test contents.'))
-            for test in sorted(outputs_to_generate):
-                package_util.validate_test(test)
-            print(util.info('Output test contents are valid!'))
+            package_util.validate_tests(sorted(outputs_to_generate), self.args.cpus, 'outputs')
```

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/commands/outgen/outgen_util.py` & `sinol_make-1.6.0.dev4/src/sinol_make/commands/outgen/outgen_util.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/commands/run/__init__.py` & `sinol_make-1.6.0.dev4/src/sinol_make/commands/run/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,29 +4,31 @@
 import subprocess
 import signal
 import threading
 import time
 import psutil
 import glob
 import shutil
+import os
+import collections
+import sys
+import math
+import dictdiffer
+import multiprocessing as mp
 from io import StringIO
 from typing import Dict
 
-from sinol_make import contest_types, oiejq
+from sinol_make import contest_types, oiejq, util
 from sinol_make.structs.run_structs import ExecutionData, PrintData
 from sinol_make.structs.cache_structs import CacheTest, CacheFile
-from sinol_make.helpers.parsers import add_compilation_arguments
 from sinol_make.interfaces.BaseCommand import BaseCommand
 from sinol_make.interfaces.Errors import CompilationError, CheckerOutputException, UnknownContestType
-from sinol_make.helpers import compile, compiler, package_util, printer, paths, cache
+from sinol_make.helpers import compile, compiler, package_util, printer, paths, cache, parsers
 from sinol_make.structs.status_structs import Status, ResultChange, PointsChange, ValidationResult, ExecutionResult, \
     TotalPointsChange
-import sinol_make.util as util
-import yaml, os, collections, sys, re, math, dictdiffer
-import multiprocessing as mp
 
 
 def color_memory(memory, limit):
     if memory == -1: return util.color_yellow("")
     memory_str = "%.1fMB" % (memory / 1024.0)
     if memory > limit:
         return util.color_red(memory_str)
@@ -284,27 +286,29 @@
 
         default_timetool = 'oiejq' if util.is_linux() else 'time'
 
         parser.add_argument('-s', '--solutions', type=str, nargs='+',
                             help='solutions to be run, for example prog/abc{b,s}*.{cpp,py}')
         parser.add_argument('-t', '--tests', type=str, nargs='+',
                             help='tests to be run, for example in/abc{0,1}*')
-        parser.add_argument('-c', '--cpus', type=int,
-                            help=f'number of cpus to use (default: {util.default_cpu_count()}')
+        parsers.add_cpus_argument(parser, 'number of cpus to use when running solutions')
         parser.add_argument('--tl', type=float, help='time limit for all tests (in s)')
         parser.add_argument('--ml', type=float, help='memory limit for all tests (in MB)')
         parser.add_argument('--hide-memory', dest='hide_memory', action='store_true',
                             help='hide memory usage in report')
         parser.add_argument('-T', '--time-tool', dest='time_tool', choices=['oiejq', 'time'],
                             help=f'tool to measure time and memory usage (default: {default_timetool})')
         parser.add_argument('--oiejq-path', dest='oiejq_path', type=str,
                             help='path to oiejq executable (default: `~/.local/bin/oiejq`)')
         parser.add_argument('-a', '--apply-suggestions', dest='apply_suggestions', action='store_true',
                             help='apply suggestions from expected scores report')
-        add_compilation_arguments(parser)
+        parser.add_argument('--ignore-expected', dest='ignore_expected', action='store_true',
+                            help='ignore expected scores from config.yml. When this flag is set, '
+                                 'the expected scores are not compared with the actual scores.')
+        parsers.add_compilation_arguments(parser)
         return parser
 
     def parse_time(self, time_str):
         if len(time_str) < 3: return -1
         return int(time_str[:-2])
 
 
@@ -1013,15 +1017,15 @@
                         for group, result in diff.new_expected_scores[solution]["expected"].items():
                             set_group_result(solution, group, result)
                     else:
                         config_expected_scores[solution] = diff.new_expected_scores[solution]
 
                 self.config["sinol_expected_scores"] = self.convert_status_to_string(config_expected_scores)
                 util.save_config(self.config)
-                print(util.info("Saved suggested expected scores description."))
+                print("Saved suggested expected scores description.")
             else:
                 util.exit_with_error("Use flag --apply-suggestions to apply suggestions.")
 
 
     def set_constants(self):
         self.ID = package_util.get_task_id()
         self.SOURCE_EXTENSIONS = ['.c', '.cpp', '.py', '.java']
@@ -1207,15 +1211,15 @@
         self.cpus = args.cpus or util.default_cpu_count()
         cache.process_extra_compilation_files(self.config.get("extra_compilation_files", []), self.ID)
         cache.process_extra_execution_files(self.config.get("extra_execution_files", {}), self.ID)
         cache.remove_results_if_contest_type_changed(self.config.get("sinol_contest_type", "default"))
 
         checker = package_util.get_files_matching_pattern(self.ID, f'{self.ID}chk.*')
         if len(checker) != 0:
-            print(util.info("Checker found: %s" % os.path.basename(checker[0])))
+            print("Checker found: %s" % os.path.basename(checker[0]))
             self.checker = checker[0]
             self.compile_checker()
         else:
             self.checker = None
         self.check_had_checker(self.checker is not None)
 
         lib = package_util.get_files_matching_pattern(self.ID, f'{self.ID}lib.*')
@@ -1234,14 +1238,19 @@
             for test in self.tests:
                 # The functions will exit if the limits are not set
                 _ = package_util.get_time_limit(test, self.config, lang, self.ID, self.args)
                 _ = package_util.get_memory_limit(test, self.config, lang, self.ID, self.args)
 
         results, all_results = self.compile_and_run(solutions)
         self.check_errors(all_results)
+        if self.args.ignore_expected:
+            print(util.warning("Ignoring expected scores."))
+            self.exit()
+            return
+
         try:
             validation_results = self.validate_expected_scores(results)
         except Exception:
             self.config = util.try_fix_config(self.config)
             try:
                 validation_results = self.validate_expected_scores(results)
             except Exception:
```

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/commands/verify/__init__.py` & `sinol_make-1.6.0.dev4/src/sinol_make/commands/verify/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,18 @@
 
         parser.add_argument('-f', '--no-fsanitize', action='store_true', default=False,
                              help='do not use sanitizers for ingen and inwer programs')
         parser.add_argument('-c', '--cpus', type=int,
                             help=f'number of cpus that sinol-make will use '
                                  f'(default: {util.default_cpu_count()})',
                             default=util.default_cpu_count())
+        parser.add_argument('--ignore-expected', dest='ignore_expected', action='store_true',
+                            help='ignore expected scores from config.yml. When this flag is set, '
+                                 'the expected scores are not compared with the actual scores. '
+                                 'This flag will be passed to the run command.')
         parsers.add_compilation_arguments(parser)
 
     def remove_cache(self):
         """
         Remove whole cache dir
         """
         cache_dir = paths.get_cache_path()
```

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/contest_types/__init__.py` & `sinol_make-1.6.0.dev4/src/sinol_make/contest_types/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/contest_types/default.py` & `sinol_make-1.6.0.dev4/src/sinol_make/contest_types/default.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/contest_types/icpc.py` & `sinol_make-1.6.0.dev4/src/sinol_make/contest_types/icpc.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/contest_types/oi.py` & `sinol_make-1.6.0.dev4/src/sinol_make/contest_types/oi.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/helpers/cache.py` & `sinol_make-1.6.0.dev4/src/sinol_make/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/helpers/compile.py` & `sinol_make-1.6.0.dev4/src/sinol_make/helpers/compile.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/helpers/compiler.py` & `sinol_make-1.6.0.dev4/src/sinol_make/helpers/compiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List
-
+import subprocess
 import argparse
+import sys
 import os
 
-import sinol_make.util as util
-import sys, subprocess
-
+from sinol_make import util
 from sinol_make.structs.compiler_structs import Compilers
+from sinol_make.helpers.func_cache import cache_result
 
 
 def check_if_installed(compiler):
     """
     Check if a compiler is installed
     """
 
@@ -18,14 +18,15 @@
         subprocess.call([compiler, '--version'], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
     except FileNotFoundError:
         return False
 
     return True
 
 
+@cache_result()
 def get_c_compiler_path():
     """
     Get the C compiler
     """
 
     if sys.platform == 'win32' or sys.platform == 'cygwin' or sys.platform == 'linux':
         if not check_if_installed('gcc'):
@@ -37,14 +38,15 @@
             compiler = 'gcc-' + str(i)
             if check_if_installed(compiler):
                 return compiler
 
         return None
 
 
+@cache_result()
 def get_cpp_compiler_path():
     """
     Get the C++ compiler
     """
 
     if sys.platform == 'win32' or sys.platform == 'cygwin' or sys.platform == 'linux':
         if not check_if_installed('g++'):
@@ -58,27 +60,29 @@
             compiler = 'g++-' + str(i)
             if check_if_installed(compiler):
                 return compiler
 
         return None
 
 
+@cache_result()
 def get_python_interpreter_path():
     """
     Get the Python interpreter
     """
 
     if check_if_installed('python3.11'):  # python3.11 is currently the default interpreter on sio.
         return 'python3.11'
     for ver in ['3.9', '3.8', '3.7', '3']:
         if check_if_installed('python' + ver):
             return 'python' + ver
     return None
 
 
+@cache_result()
 def get_java_compiler_path():
     """
     Get the Java compiler
     """
 
     if not check_if_installed('javac'):
         return None
@@ -90,15 +94,16 @@
     """
     Get the default compilers
     """
     return argparse.Namespace(
         c_compiler_path=get_c_compiler_path(),
         cpp_compiler_path=get_cpp_compiler_path(),
         python_interpreter_path=get_python_interpreter_path(),
-        java_compiler_path=get_java_compiler_path()
+        # Java is not currently supported by sinol-make
+        # java_compiler_path=get_java_compiler_path()
     )
 
 
 def verify_compilers(args: argparse.Namespace, solutions: List[str]) -> Compilers:
     """
     Verify that specified compilers exist.
     :param args: argparse.Namespace arguments
@@ -137,9 +142,9 @@
             util.exit_with_error(
                 'Couldn\'t find a %s. Tried %s. Try specifying a compiler with %s.' % (compiler, tried, flag))
 
     return Compilers(
         c_compiler_path=args.c_compiler_path,
         cpp_compiler_path=args.cpp_compiler_path,
         python_interpreter_path=args.python_interpreter_path,
-        java_compiler_path=args.java_compiler_path
+        java_compiler_path=None
     )
```

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/helpers/package_util.py` & `sinol_make-1.6.0.dev4/src/sinol_make/helpers/package_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import os
 import re
 import yaml
 import glob
 import fnmatch
+import multiprocessing as mp
 from enum import Enum
-from typing import List, Union, Dict, Any
+from typing import List, Union, Dict, Any, Tuple
 
+from sinol_make.helpers.func_cache import cache_result
 from sinol_make import util
 from sinol_make.helpers import paths
 
 
+@cache_result(cwd=True)
 def get_task_id() -> str:
     config = get_config()
     if "sinol_task_id" in config:
         return config["sinol_task_id"]
     else:
         print(util.warning("sinol_task_id not specified in config.yml. Using task id from directory name."))
         task_id = os.path.split(os.getcwd())[-1]
@@ -349,45 +352,67 @@
     :param contest_type: Contest type.
     """
     os.makedirs(paths.get_cache_path(), exist_ok=True)
     with open(paths.get_cache_path("contest_type"), "w") as contest_type_file:
         contest_type_file.write(contest_type)
 
 
-def validate_test(test_path: str):
+def validate_test(test_path: str) -> Tuple[bool, str]:
     """
     Check if test doesn't contain leading/trailing whitespaces,
     has only one space between tokens and ends with newline.
     Exits with error if any of the conditions is not met.
+    :return: Tuple of two values: True if test is valid, error message otherwise.
     """
     basename = os.path.basename(test_path)
     num_empty = 0
     with open(test_path, 'br') as file:
         lines = file.readlines()
         for i, line in enumerate(lines):
             line = line.decode('utf-8')
             if len(line) > 0 and line[0] == ' ':
-                util.exit_with_error(f'Leading whitespace in {basename}:{i + 1}')
+                return False, util.error(f'Leading whitespace in {basename}:{i + 1}')
             if len(line) > 0 and (line[-2:] == '\r\n' or line[-2:] == '\n\r' or line[-1] == '\r'):
-                util.exit_with_error(f'Carriage return at the end of {basename}:{i + 1}')
+                return False, util.error(f'Carriage return at the end of {basename}:{i + 1}')
             if len(line) > 0 and line[-1] != '\n':
-                util.exit_with_error(f'No newline at the end of {basename}')
+                return False, util.error(f'No newline at the end of {basename}')
             if line == '\n' or line == '':
                 num_empty += 1
                 continue
             elif i == len(lines) - 1:
                 num_empty = 0
             if line[-2] == ' ':
-                util.exit_with_error(f'Trailing whitespace in {basename}:{i + 1}')
+                return False, util.error(f'Trailing whitespace in {basename}:{i + 1}')
             for j in range(len(line) - 1):
                 if line[j] == ' ' and line[j + 1] == ' ':
-                    util.exit_with_error(f'Tokens not separated by one space in {basename}:{i + 1}')
+                    return False, util.error(f'Tokens not separated by one space in {basename}:{i + 1}')
 
         if num_empty != 0:
-            util.exit_with_error(f'Exactly one empty line expected in {basename}')
+            return False, util.error(f'Exactly one empty line expected in {basename}')
+
+    return True, ''
+
+
+def validate_tests(tests: List[str], cpus: int, type: str = 'input'):
+    """
+    Validate all tests in parallel.
+    """
+    if not tests:
+        return
+    print(f'Validating {type} test contents.')
+    num_tests = len(tests)
+    finished = 0
+    with mp.Pool(cpus) as pool:
+        for valid, message in pool.imap(validate_test, tests):
+            if not valid:
+                util.exit_with_error(message)
+            finished += 1
+            print(f'Validated {finished}/{num_tests} tests', end='\r')
+    print()
+    print(util.info(f'All {type} tests are valid!'))
 
 
 def get_all_inputs(task_id):
     in_test_re = get_in_tests_re(task_id)
     inputs = []
     for file in glob.glob(os.path.join(os.getcwd(), "in", "*.in")):
         if in_test_re.match(os.path.basename(file)):
```

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/helpers/parsers.py` & `sinol_make-1.6.0.dev4/src/sinol_make/helpers/parsers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
-
 import argparse
 
+from sinol_make import util
 from sinol_make.helpers import compiler
 
 
 def add_compilation_arguments(parser: argparse.ArgumentParser):
     if sys.platform == 'darwin':
         gcc_versions = 'gcc-9, gcc-10, gcc-11'
         gpp_versions = 'g++-9, g++-10, g++-11'
@@ -16,16 +16,24 @@
     parser.add_argument('--c-compiler-path', dest='c_compiler_path', type=str,
                         default=compiler.get_c_compiler_path(), help=f'C compiler to use (default: {gcc_versions})')
     parser.add_argument('--cpp-compiler-path', dest='cpp_compiler_path', type=str,
                         default=compiler.get_cpp_compiler_path(), help=f'C++ compiler to use (default: {gpp_versions})')
     parser.add_argument('--python-interpreter-path', dest='python_interpreter_path', type=str,
                         default=compiler.get_python_interpreter_path(),
                         help='Python interpreter to use (default: python3)')
-    parser.add_argument('--java-compiler-path', dest='java_compiler_path', type=str,
-                        default=compiler.get_java_compiler_path(), help='Java compiler to use (default: javac)')
+    # Java is not currently supported by sinol-make
+    # parser.add_argument('--java-compiler-path', dest='java_compiler_path', type=str,
+    #                     default=compiler.get_java_compiler_path(), help='Java compiler to use (default: javac)')
     parser.add_argument('--compile-mode', '-C', dest='compile_mode', choices=['default', 'oioioi', 'weak', 'd', 'o', 'w'],
                         help='Warning flag groups used to compile C/C++ files. Available options:\n'
                              ' default / d - uses default flags: \n'
                              '    (-Wshadow -Wconversion -Wno-unused-result -Wfloat-equal) + oioioi flags\n'
                              ' oioioi / o - uses the same flags as oioioi:\n'
                              '    (-Wall -Wno-unused-result -Werror)'
                              ' weak / w - disable all warning flags during C and C++ compilation', default='default')
+
+
+def add_cpus_argument(parser: argparse.ArgumentParser, help: str):
+    parser.add_argument('-c', '--cpus', type=int,
+                        help=f'{help} '
+                             f'(default: {util.default_cpu_count()})',
+                        default=util.default_cpu_count())
```

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/helpers/paths.py` & `sinol_make-1.6.0.dev4/src/sinol_make/helpers/paths.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/helpers/printer.py` & `sinol_make-1.6.0.dev4/src/sinol_make/helpers/printer.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/oiejq/__init__.py` & `sinol_make-1.6.0.dev4/src/sinol_make/oiejq/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/structs/cache_structs.py` & `sinol_make-1.6.0.dev4/src/sinol_make/structs/cache_structs.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/structs/compiler_structs.py` & `sinol_make-1.6.0.dev4/src/sinol_make/structs/compiler_structs.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/structs/inwer_structs.py` & `sinol_make-1.6.0.dev4/src/sinol_make/structs/inwer_structs.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/structs/run_structs.py` & `sinol_make-1.6.0.dev4/src/sinol_make/structs/run_structs.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/structs/status_structs.py` & `sinol_make-1.6.0.dev4/src/sinol_make/structs/status_structs.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make/util.py` & `sinol_make-1.6.0.dev4/src/sinol_make/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 import glob, importlib, os, sys, requests, yaml
 import math
-import multiprocessing
 import platform
 import tarfile
 import hashlib
 import multiprocessing
 import resource
 from typing import Union
 from packaging.version import parse as parse_version
 
 from sinol_make.contest_types import get_contest_type
 from sinol_make.helpers import paths, cache
+from sinol_make.helpers.func_cache import cache_result
 from sinol_make.structs.status_structs import Status
 
 
-__cache = {}
-
-
+@cache_result()
 def get_commands():
     """
     Function to get an array of all available commands.
     """
-    global __cache
-    if 'commands' in __cache:
-        return __cache['commands']
     commands_path = glob.glob(
         os.path.join(
             os.path.dirname(os.path.realpath(__file__)),
             'commands/*'
         )
     )
     commands = []
     for path in commands_path:
         temp = importlib.import_module('sinol_make.commands.' + os.path.basename(path), 'Command')
         commands.append(temp.Command())
 
-    __cache['commands'] = commands
     return commands
 
 
 def get_command_names():
     """
     Function to get an array of all available command names.
     """
```

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make.egg-info/PKG-INFO` & `sinol_make-1.6.0.dev4/src/sinol_make.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol_make
-Version: 1.6.0.dev3
+Version: 1.6.0.dev4
 Summary: CLI tool for creating sio2 task packages
 Author: Mateusz Masiarz
 Author-email: m.masiarz@fri.edu.pl
 Maintainer: Tomasz Nowak, Mateusz Masiarz
 Maintainer-email: tomasz.nowak@tonowak.com, m.masiarz@fri.edu.pl
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
```

### Comparing `sinol_make-1.6.0.dev3/src/sinol_make.egg-info/SOURCES.txt` & `sinol_make-1.6.0.dev4/src/sinol_make.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 src/sinol_make/contest_types/default.py
 src/sinol_make/contest_types/icpc.py
 src/sinol_make/contest_types/oi.py
 src/sinol_make/helpers/__init__.py
 src/sinol_make/helpers/cache.py
 src/sinol_make/helpers/compile.py
 src/sinol_make/helpers/compiler.py
+src/sinol_make/helpers/func_cache.py
 src/sinol_make/helpers/package_util.py
 src/sinol_make/helpers/parsers.py
 src/sinol_make/helpers/paths.py
 src/sinol_make/helpers/printer.py
 src/sinol_make/interfaces/BaseCommand.py
 src/sinol_make/interfaces/Errors.py
 src/sinol_make/interfaces/__init__.py
```

### Comparing `sinol_make-1.6.0.dev3/tests/test_multiple_arguments.py` & `sinol_make-1.6.0.dev4/tests/test_multiple_arguments.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/tests/test_oiejq.py` & `sinol_make-1.6.0.dev4/tests/test_oiejq.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev3/tests/test_util.py` & `sinol_make-1.6.0.dev4/tests/test_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,32 +48,35 @@
 def test_check_version(**kwargs):
     """
     Tests for check_version function
     Simulates wrong responses and exceptions with requests-mock
     """
     mocker = kwargs["mocker"]
 
-    mocker.get("https://pypi.python.org/pypi/sinol-make/json", json={"info": {"version": "1.0.0.dev2"}})
+    def create_response(version):
+        return {"releases": {version: "something"}}
+
+    mocker.get("https://pypi.python.org/pypi/sinol-make/json", json=create_response("1.0.0.dev2"))
     util.check_version()
     version = util.check_for_updates("1.0.0.dev1", False)
     assert version == "1.0.0.dev2"
     assert util.is_dev(version)
 
-    mocker.get("https://pypi.python.org/pypi/sinol-make/json", json={"info": {"version": "1.0.0"}})
+    mocker.get("https://pypi.python.org/pypi/sinol-make/json", json=create_response("1.0.0"))
     util.check_version()
     version = util.check_for_updates("1.0.0.dev1", False)
     assert version == "1.0.0"
     assert not util.is_dev(version)
 
-    mocker.get("https://pypi.python.org/pypi/sinol-make/json", json={"info": {"version": "2.0.0.dev1"}})
+    mocker.get("https://pypi.python.org/pypi/sinol-make/json", json=create_response("2.0.0.dev1"))
     util.check_version()
     version = util.check_for_updates("1.0.0", False)
     assert version is None
 
-    mocker.get("https://pypi.python.org/pypi/sinol-make/json", json={"info": {"version": "1.0.1"}})
+    mocker.get("https://pypi.python.org/pypi/sinol-make/json", json=create_response("1.0.1"))
     util.check_version()
     version = util.check_for_updates("1.0.0", False)
     assert version == "1.0.1"
     assert not util.is_dev(version)
 
     importlib = util.import_importlib_resources()
 
@@ -82,15 +85,15 @@
     if not data_dir.is_dir():
         data_dir.mkdir()
     data_dir.chmod(0o777)
     if version_file.is_file():
         version_file.unlink()
 
     # Test correct request
-    mocker.get("https://pypi.python.org/pypi/sinol-make/json", json={"info": {"version": "1.0.0"}})
+    mocker.get("https://pypi.python.org/pypi/sinol-make/json", json=create_response(("1.0.0")))
     util.check_version()
     assert version_file.is_file()
     assert version_file.read_text() == "1.0.0"
     version_file.unlink()
 
     # Test wrong request
     mocker.get("https://pypi.python.org/pypi/sinol-make/json", status_code=404)
```


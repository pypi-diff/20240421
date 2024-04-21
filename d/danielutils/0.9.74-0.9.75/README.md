# Comparing `tmp/danielutils-0.9.74.tar.gz` & `tmp/danielutils-0.9.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danielutils-0.9.74.tar", last modified: Mon Apr 15 22:47:53 2024, max compression
+gzip compressed data, was "danielutils-0.9.75.tar", last modified: Sun Apr 21 19:23:39 2024, max compression
```

## Comparing `danielutils-0.9.74.tar` & `danielutils-0.9.75.tar`

### file list

```diff
@@ -1,134 +1,98 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.578963 danielutils-0.9.74/
--rw-rw-rw-   0        0        0     1091 2023-05-29 13:19:53.000000 danielutils-0.9.74/LICENSE
--rw-rw-rw-   0        0        0     4478 2024-04-15 22:47:53.577883 danielutils-0.9.74/PKG-INFO
--rw-rw-rw-   0        0        0     2543 2024-04-15 22:47:31.000000 danielutils-0.9.74/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.487525 danielutils-0.9.74/danielutils/
--rw-rw-rw-   0        0        0     1474 2024-04-15 22:00:00.000000 danielutils-0.9.74/danielutils/__init__.py
--rw-rw-rw-   0        0        0     5663 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/aliases.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.496824 danielutils-0.9.74/danielutils/classes/
--rw-rw-rw-   0        0        0      210 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/classes/Convenience.py
--rw-rw-rw-   0        0        0     1221 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/classes/Counter.py
--rw-rw-rw-   0        0        0        0 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/classes/Tree.py
--rw-rw-rw-   0        0        0      159 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/classes/__init__.py
--rw-rw-rw-   0        0        0     7286 2024-04-15 22:37:37.000000 danielutils-0.9.74/danielutils/classes/frange.py
--rw-rw-rw-   0        0        0     3169 2024-04-15 22:24:58.000000 danielutils-0.9.74/danielutils/classes/repl.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.498906 danielutils-0.9.74/danielutils/classes/sorted_builtins/
--rw-rw-rw-   0        0        0        0 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/classes/sorted_builtins/__init__.py
--rw-rw-rw-   0        0        0      112 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/classes/sorted_builtins/sset.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.504587 danielutils-0.9.74/danielutils/classes/typed_builtins/
--rw-rw-rw-   0        0        0       88 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/classes/typed_builtins/__init__.py
--rw-rw-rw-   0        0        0     4730 2024-04-09 22:20:09.000000 danielutils-0.9.74/danielutils/classes/typed_builtins/factory.py
--rw-rw-rw-   0        0        0      913 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/classes/typed_builtins/tdict.py
--rw-rw-rw-   0        0        0     7214 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/classes/typed_builtins/tlist.py
--rw-rw-rw-   0        0        0     2031 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/classes/typed_builtins/tset.py
--rw-rw-rw-   0        0        0      294 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/classes/typed_builtins/ttuple.py
--rw-rw-rw-   0        0        0     5457 2024-04-15 22:08:50.000000 danielutils-0.9.74/danielutils/colors.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.505588 danielutils-0.9.74/danielutils/conversions/
--rw-rw-rw-   0        0        0       73 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/conversions/__init__.py
--rw-rw-rw-   0        0        0     2227 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/conversions/main_conversions.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.508589 danielutils-0.9.74/danielutils/conversions/specialized_conversions/
--rw-rw-rw-   0        0        0       46 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/conversions/specialized_conversions/__init__.py
--rw-rw-rw-   0        0        0      507 2024-03-21 23:16:41.000000 danielutils-0.9.74/danielutils/conversions/specialized_conversions/to_hex.py
--rw-rw-rw-   0        0        0      549 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/conversions/specialized_conversions/to_int.py
--rw-rw-rw-   0        0        0     2800 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/d_print.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.513631 danielutils-0.9.74/danielutils/data_structures/
--rw-rw-rw-   0        0        0     1224 2024-04-15 22:24:58.000000 danielutils-0.9.74/danielutils/data_structures/Comparer.py
--rw-rw-rw-   0        0        0     2143 2024-04-15 22:26:05.000000 danielutils-0.9.74/danielutils/data_structures/Stack.py
--rw-rw-rw-   0        0        0      163 2024-04-15 22:26:05.000000 danielutils-0.9.74/danielutils/data_structures/__init__.py
--rw-rw-rw-   0        0        0      273 2024-04-15 22:24:58.000000 danielutils-0.9.74/danielutils/data_structures/default_dict.py
--rw-rw-rw-   0        0        0      632 2023-09-25 13:19:42.000000 danielutils-0.9.74/danielutils/data_structures/functions.py
--rw-rw-rw-   0        0        0      631 2023-09-25 13:20:33.000000 danielutils-0.9.74/danielutils/date.py
--rw-rw-rw-   0        0        0      232 2023-08-07 20:06:13.000000 danielutils-0.9.74/danielutils/date_time.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.530547 danielutils-0.9.74/danielutils/decorators/
--rw-rw-rw-   0        0        0      446 2024-04-09 22:04:07.000000 danielutils-0.9.74/danielutils/decorators/__init__.py
--rw-rw-rw-   0        0        0      912 2024-03-27 18:52:27.000000 danielutils-0.9.74/danielutils/decorators/atomic.py
--rw-rw-rw-   0        0        0     1538 2024-04-15 22:37:38.000000 danielutils-0.9.74/danielutils/decorators/attach.py
--rw-rw-rw-   0        0        0      730 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/decorators/chain_decorators.py
--rw-rw-rw-   0        0        0     1074 2024-04-10 11:18:47.000000 danielutils-0.9.74/danielutils/decorators/decorate_conditionally.py
--rw-rw-rw-   0        0        0     1175 2024-04-15 22:37:37.000000 danielutils-0.9.74/danielutils/decorators/delay_call.py
--rw-rw-rw-   0        0        0     1452 2024-04-15 22:37:38.000000 danielutils-0.9.74/danielutils/decorators/deprecate.py
--rw-rw-rw-   0        0        0     1860 2024-04-15 22:37:37.000000 danielutils-0.9.74/danielutils/decorators/limit_recursion.py
--rw-rw-rw-   0        0        0     1017 2024-04-15 22:37:38.000000 danielutils-0.9.74/danielutils/decorators/memo.py
--rw-rw-rw-   0        0        0     7785 2024-04-15 22:37:37.000000 danielutils-0.9.74/danielutils/decorators/overload.py
--rw-rw-rw-   0        0        0      995 2024-04-15 22:37:38.000000 danielutils-0.9.74/danielutils/decorators/partially_implemented.py
--rw-rw-rw-   0        0        0     1709 2024-04-09 23:09:17.000000 danielutils-0.9.74/danielutils/decorators/processify.py
--rw-rw-rw-   0        0        0     1095 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/decorators/property.py
--rw-rw-rw-   0        0        0      899 2024-04-15 22:37:38.000000 danielutils-0.9.74/danielutils/decorators/threadify.py
--rw-rw-rw-   0        0        0     2157 2024-04-15 22:37:37.000000 danielutils-0.9.74/danielutils/decorators/timeout.py
--rw-rw-rw-   0        0        0     9996 2024-04-15 22:37:38.000000 danielutils-0.9.74/danielutils/decorators/validate.py
--rw-rw-rw-   0        0        0     2163 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/exceptions.py
--rw-rw-rw-   0        0        0    12002 2024-04-15 21:39:53.000000 danielutils-0.9.74/danielutils/files_and_folders.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.536945 danielutils-0.9.74/danielutils/functions/
--rw-rw-rw-   0        0        0      160 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/functions/__init__.py
--rw-rw-rw-   0        0        0     1097 2024-03-27 18:52:27.000000 danielutils-0.9.74/danielutils/functions/areoneof.py
--rw-rw-rw-   0        0        0      638 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/functions/check_foreach.py
--rw-rw-rw-   0        0        0     9027 2024-03-29 00:10:11.000000 danielutils-0.9.74/danielutils/functions/isoftype.py
--rw-rw-rw-   0        0        0     1598 2024-03-27 18:52:27.000000 danielutils-0.9.74/danielutils/functions/isoneof.py
--rw-rw-rw-   0        0        0      639 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/functions/powerset.py
--rw-rw-rw-   0        0        0     1016 2024-03-27 18:52:27.000000 danielutils-0.9.74/danielutils/functions/types_subseteq.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.542303 danielutils-0.9.74/danielutils/generators/
--rw-rw-rw-   0        0        0      108 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/generators/__init__.py
--rw-rw-rw-   0        0        0     1285 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/generators/conditional_generator.py
--rw-rw-rw-   0        0        0      463 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/generators/generator_from_stream.py
--rw-rw-rw-   0        0        0     2861 2024-04-10 15:54:43.000000 danielutils-0.9.74/danielutils/generators/join_generators.py
--rw-rw-rw-   0        0        0     2051 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/internet.py
--rw-rw-rw-   0        0        0     2005 2024-02-19 17:33:20.000000 danielutils-0.9.74/danielutils/loops.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.546707 danielutils-0.9.74/danielutils/math/
--rw-rw-rw-   0        0        0       80 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/math/__init__.py
--rw-rw-rw-   0        0        0     7682 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/math/constants.py
--rw-rw-rw-   0        0        0      627 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/math/functions.py
--rw-rw-rw-   0        0        0     1062 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/math/math_print.py
--rw-rw-rw-   0        0        0     4051 2024-03-27 18:52:27.000000 danielutils-0.9.74/danielutils/math/math_symbols.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.553403 danielutils-0.9.74/danielutils/metaclasses/
--rw-rw-rw-   0        0        0    10944 2024-03-27 18:52:27.000000 danielutils-0.9.74/danielutils/metaclasses/Interface.py
--rw-rw-rw-   0        0        0      169 2024-03-21 23:16:41.000000 danielutils-0.9.74/danielutils/metaclasses/__init__.py
--rw-rw-rw-   0        0        0      695 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/metaclasses/atomic_class_meta.py
--rw-rw-rw-   0        0        0     2511 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/metaclasses/implicit_data_deleter_meta.py
--rw-rw-rw-   0        0        0     1487 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/metaclasses/instance_cache_meta.py
--rw-rw-rw-   0        0        0     1754 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/metaclasses/overload_meta.py
--rw-rw-rw-   0        0        0      374 2024-04-15 21:39:53.000000 danielutils-0.9.74/danielutils/multi_x.py
--rw-rw-rw-   0        0        0     1733 2024-04-15 22:27:00.000000 danielutils-0.9.74/danielutils/my_tqdm.py
--rw-rw-rw-   0        0        0     1032 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/path.py
--rw-rw-rw-   0        0        0        0 2023-08-09 09:08:58.000000 danielutils-0.9.74/danielutils/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.558752 danielutils-0.9.74/danielutils/reflection/
--rw-rw-rw-   0        0        0     1650 2024-04-09 23:20:42.000000 danielutils-0.9.74/danielutils/reflection/__init__.py
--rw-rw-rw-   0        0        0     1063 2024-04-15 22:37:38.000000 danielutils-0.9.74/danielutils/reflection/class_reflection.py
--rw-rw-rw-   0        0        0     1192 2024-04-15 22:37:38.000000 danielutils-0.9.74/danielutils/reflection/file_reflection.py
--rw-rw-rw-   0        0        0     4480 2024-04-15 21:50:16.000000 danielutils-0.9.74/danielutils/reflection/function_reflections.py
--rw-rw-rw-   0        0        0      444 2024-03-29 21:51:07.000000 danielutils-0.9.74/danielutils/reflection/get_traceback.py
--rw-rw-rw-   0        0        0      507 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/reflection/module_reflections.py
--rw-rw-rw-   0        0        0      622 2024-04-15 21:50:16.000000 danielutils-0.9.74/danielutils/reflection/system_reflections.py
--rw-rw-rw-   0        0        0      288 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/relations.py
--rw-rw-rw-   0        0        0      489 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/signals.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.562165 danielutils-0.9.74/danielutils/snippets/
--rw-rw-rw-   0        0        0       24 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/snippets/__init__.py
--rw-rw-rw-   0        0        0      433 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/snippets/try_get.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.564302 danielutils-0.9.74/danielutils/system/
--rw-rw-rw-   0        0        0       52 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/system/__init__.py
--rw-rw-rw-   0        0        0     6844 2024-03-27 18:52:27.000000 danielutils-0.9.74/danielutils/system/independent.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.567300 danielutils-0.9.74/danielutils/system/windows/
--rw-rw-rw-   0        0        0       50 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/system/windows/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.568379 danielutils-0.9.74/danielutils/system/windows/utils/
--rw-rw-rw-   0        0        0       25 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/system/windows/utils/__init__.py
--rw-rw-rw-   0        0        0      499 2024-04-15 21:50:16.000000 danielutils-0.9.74/danielutils/system/windows/utils/filetime.py
--rw-rw-rw-   0        0        0     6064 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/system/windows/win32_ctime.py
--rw-rw-rw-   0        0        0     2253 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/system/windows/windows.py
--rw-rw-rw-   0        0        0     4093 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/text.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.572508 danielutils-0.9.74/danielutils/threads/
--rw-rw-rw-   0        0        0       51 2023-08-15 21:20:20.000000 danielutils-0.9.74/danielutils/threads/__init__.py
--rw-rw-rw-   0        0        0     2397 2024-04-15 22:40:32.000000 danielutils-0.9.74/danielutils/threads/worker.py
--rw-rw-rw-   0        0        0     2425 2024-04-15 22:40:32.000000 danielutils-0.9.74/danielutils/threads/worker_pool.py
--rw-rw-rw-   0        0        0     1399 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/time.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.573521 danielutils-0.9.74/danielutils/university/
--rw-rw-rw-   0        0        0       74 2024-04-15 21:59:15.000000 danielutils-0.9.74/danielutils/university/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.576403 danielutils-0.9.74/danielutils/university/databases/
--rw-rw-rw-   0        0        0       20 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/university/databases/__init__.py
--rw-rw-rw-   0        0        0    24942 2024-03-21 20:59:13.000000 danielutils-0.9.74/danielutils/university/databases/all.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:53.490455 danielutils-0.9.74/danielutils.egg-info/
--rw-rw-rw-   0        0        0     4478 2024-04-15 22:47:53.000000 danielutils-0.9.74/danielutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4116 2024-04-15 22:47:53.000000 danielutils-0.9.74/danielutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 22:47:53.000000 danielutils-0.9.74/danielutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 22:47:53.000000 danielutils-0.9.74/danielutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      928 2024-04-15 22:47:52.000000 danielutils-0.9.74/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 22:47:53.579917 danielutils-0.9.74/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-04-15 22:47:52.000000 danielutils-0.9.74/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:39.117411 danielutils-0.9.75/
+-rw-rw-rw-   0        0        0     1091 2023-05-29 13:19:53.000000 danielutils-0.9.75/LICENSE
+-rw-rw-rw-   0        0        0     4486 2024-04-21 19:23:39.115906 danielutils-0.9.75/PKG-INFO
+-rw-rw-rw-   0        0        0     2543 2024-04-21 19:23:37.000000 danielutils-0.9.75/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:39.059430 danielutils-0.9.75/danielutils/
+-rw-rw-rw-   0        0        0     1364 2024-04-21 19:19:56.000000 danielutils-0.9.75/danielutils/__init__.py
+-rw-rw-rw-   0        0        0     5663 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/aliases.py
+-rw-rw-rw-   0        0        0     5457 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/colors.py
+-rw-rw-rw-   0        0        0      210 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/convenience.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:39.064431 danielutils-0.9.75/danielutils/conversions/
+-rw-rw-rw-   0        0        0       73 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/conversions/__init__.py
+-rw-rw-rw-   0        0        0     2227 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/conversions/main_conversions.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:39.066936 danielutils-0.9.75/danielutils/conversions/specialized_conversions/
+-rw-rw-rw-   0        0        0       46 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/conversions/specialized_conversions/__init__.py
+-rw-rw-rw-   0        0        0      507 2024-03-21 23:16:41.000000 danielutils-0.9.75/danielutils/conversions/specialized_conversions/to_hex.py
+-rw-rw-rw-   0        0        0      549 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/conversions/specialized_conversions/to_int.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:39.071140 danielutils-0.9.75/danielutils/data_structures/
+-rw-rw-rw-   0        0        0     1224 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/data_structures/Comparer.py
+-rw-rw-rw-   0        0        0     2143 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/data_structures/Stack.py
+-rw-rw-rw-   0        0        0      163 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/data_structures/__init__.py
+-rw-rw-rw-   0        0        0      273 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/data_structures/default_dict.py
+-rw-rw-rw-   0        0        0      632 2023-09-25 13:19:42.000000 danielutils-0.9.75/danielutils/data_structures/functions.py
+-rw-rw-rw-   0        0        0      631 2023-09-25 13:20:33.000000 danielutils-0.9.75/danielutils/date.py
+-rw-rw-rw-   0        0        0      232 2023-08-07 20:06:13.000000 danielutils-0.9.75/danielutils/date_time.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:39.086684 danielutils-0.9.75/danielutils/decorators/
+-rw-rw-rw-   0        0        0      446 2024-04-09 22:04:07.000000 danielutils-0.9.75/danielutils/decorators/__init__.py
+-rw-rw-rw-   0        0        0      912 2024-03-27 18:52:27.000000 danielutils-0.9.75/danielutils/decorators/atomic.py
+-rw-rw-rw-   0        0        0     1538 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/decorators/attach.py
+-rw-rw-rw-   0        0        0      730 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/decorators/chain_decorators.py
+-rw-rw-rw-   0        0        0     1074 2024-04-10 11:18:47.000000 danielutils-0.9.75/danielutils/decorators/decorate_conditionally.py
+-rw-rw-rw-   0        0        0     1175 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/decorators/delay_call.py
+-rw-rw-rw-   0        0        0     1452 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/decorators/deprecate.py
+-rw-rw-rw-   0        0        0     1860 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/decorators/limit_recursion.py
+-rw-rw-rw-   0        0        0     1017 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/decorators/memo.py
+-rw-rw-rw-   0        0        0     7785 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/decorators/overload.py
+-rw-rw-rw-   0        0        0      995 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/decorators/partially_implemented.py
+-rw-rw-rw-   0        0        0     1716 2024-04-21 19:21:56.000000 danielutils-0.9.75/danielutils/decorators/processify.py
+-rw-rw-rw-   0        0        0     1095 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/decorators/property.py
+-rw-rw-rw-   0        0        0      899 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/decorators/threadify.py
+-rw-rw-rw-   0        0        0     2157 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/decorators/timeout.py
+-rw-rw-rw-   0        0        0    10004 2024-04-21 18:13:57.000000 danielutils-0.9.75/danielutils/decorators/validate.py
+-rw-rw-rw-   0        0        0     2163 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:39.094226 danielutils-0.9.75/danielutils/functions/
+-rw-rw-rw-   0        0        0      235 2024-04-21 19:19:56.000000 danielutils-0.9.75/danielutils/functions/__init__.py
+-rw-rw-rw-   0        0        0     1097 2024-03-27 18:52:27.000000 danielutils-0.9.75/danielutils/functions/areoneof.py
+-rw-rw-rw-   0        0        0      638 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/functions/check_foreach.py
+-rw-rw-rw-   0        0        0    10296 2024-04-21 18:21:37.000000 danielutils-0.9.75/danielutils/functions/isoftype.py
+-rw-rw-rw-   0        0        0     1598 2024-03-27 18:52:27.000000 danielutils-0.9.75/danielutils/functions/isoneof.py
+-rw-rw-rw-   0        0        0      639 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/functions/powerset.py
+-rw-rw-rw-   0        0        0     1016 2024-03-27 18:52:27.000000 danielutils-0.9.75/danielutils/functions/types_subseteq.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:39.097742 danielutils-0.9.75/danielutils/generators/
+-rw-rw-rw-   0        0        0      108 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/generators/__init__.py
+-rw-rw-rw-   0        0        0     1285 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/generators/conditional_generator.py
+-rw-rw-rw-   0        0        0      463 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/generators/generator_from_stream.py
+-rw-rw-rw-   0        0        0     2869 2024-04-21 18:13:57.000000 danielutils-0.9.75/danielutils/generators/join_generators.py
+-rw-rw-rw-   0        0        0     2051 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/internet.py
+-rw-rw-rw-   0        0        0    12002 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/io_.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:39.103194 danielutils-0.9.75/danielutils/metaclasses/
+-rw-rw-rw-   0        0        0    10952 2024-04-21 18:13:57.000000 danielutils-0.9.75/danielutils/metaclasses/Interface.py
+-rw-rw-rw-   0        0        0      169 2024-03-21 23:16:41.000000 danielutils-0.9.75/danielutils/metaclasses/__init__.py
+-rw-rw-rw-   0        0        0      695 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/metaclasses/atomic_class_meta.py
+-rw-rw-rw-   0        0        0     2511 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/metaclasses/implicit_data_deleter_meta.py
+-rw-rw-rw-   0        0        0     1495 2024-04-21 18:13:57.000000 danielutils-0.9.75/danielutils/metaclasses/instance_cache_meta.py
+-rw-rw-rw-   0        0        0     1754 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/metaclasses/overload_meta.py
+-rw-rw-rw-   0        0        0     1032 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/path.py
+-rw-rw-rw-   0        0        0     2801 2024-04-21 18:05:24.000000 danielutils-0.9.75/danielutils/print_.py
+-rw-rw-rw-   0        0        0        0 2023-08-09 09:08:58.000000 danielutils-0.9.75/danielutils/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:39.104193 danielutils-0.9.75/danielutils/reflection/
+-rw-rw-rw-   0        0        0     1516 2024-04-21 18:21:37.000000 danielutils-0.9.75/danielutils/reflection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:39.105194 danielutils-0.9.75/danielutils/snippets/
+-rw-rw-rw-   0        0        0       24 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/snippets/__init__.py
+-rw-rw-rw-   0        0        0      433 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/snippets/try_get.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:39.107707 danielutils-0.9.75/danielutils/system/
+-rw-rw-rw-   0        0        0       52 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/system/__init__.py
+-rw-rw-rw-   0        0        0     6844 2024-03-27 18:52:27.000000 danielutils-0.9.75/danielutils/system/independent.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:39.110220 danielutils-0.9.75/danielutils/system/windows/
+-rw-rw-rw-   0        0        0       50 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/system/windows/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:39.111908 danielutils-0.9.75/danielutils/system/windows/utils/
+-rw-rw-rw-   0        0        0       25 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/system/windows/utils/__init__.py
+-rw-rw-rw-   0        0        0      499 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/system/windows/utils/filetime.py
+-rw-rw-rw-   0        0        0     6064 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/system/windows/win32_ctime.py
+-rw-rw-rw-   0        0        0     2253 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/system/windows/windows.py
+-rw-rw-rw-   0        0        0     4093 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/text.py
+-rw-rw-rw-   0        0        0     1399 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/time.py
+-rw-rw-rw-   0        0        0     1733 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/tqdm_.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:39.112906 danielutils-0.9.75/danielutils/university/
+-rw-rw-rw-   0        0        0       74 2024-04-17 20:37:10.000000 danielutils-0.9.75/danielutils/university/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:39.114907 danielutils-0.9.75/danielutils/university/databases/
+-rw-rw-rw-   0        0        0       20 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/university/databases/__init__.py
+-rw-rw-rw-   0        0        0    24942 2024-03-21 20:59:13.000000 danielutils-0.9.75/danielutils/university/databases/all.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:39.062431 danielutils-0.9.75/danielutils.egg-info/
+-rw-rw-rw-   0        0        0     4486 2024-04-21 19:23:38.000000 danielutils-0.9.75/danielutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2883 2024-04-21 19:23:38.000000 danielutils-0.9.75/danielutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 19:23:38.000000 danielutils-0.9.75/danielutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-21 19:23:38.000000 danielutils-0.9.75/danielutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      936 2024-04-21 19:23:37.000000 danielutils-0.9.75/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-21 19:23:39.117411 danielutils-0.9.75/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-21 19:23:37.000000 danielutils-0.9.75/setup.py
```

### Comparing `danielutils-0.9.74/LICENSE` & `danielutils-0.9.75/LICENSE`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/PKG-INFO` & `danielutils-0.9.75/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.9.74
+Version: 0.9.75
 Summary: A python utils library for things I find useful
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,30 +22,30 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/danielnachumdev/danielutils
 Project-URL: Bug Tracker, https://github.com/danielnachumdev/danielutils/issues
-Keywords: functions,decorators,methods,classes,metaclasses
+Keywords: functions,decorators,methods,better_builtins,metaclasses
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.9.74
+# danielutils v=0.9.75
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 # Showcase
 In [this](./READMES/) folder you can check out some more in depth showcase of some of the topics I have covered in this package
```

### Comparing `danielutils-0.9.74/README.md` & `danielutils-0.9.75/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.9.74
+# danielutils v=0.9.75
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 # Showcase
 In [this](./READMES/) folder you can check out some more in depth showcase of some of the topics I have covered in this package
```

### Comparing `danielutils-0.9.74/danielutils/__init__.py` & `danielutils-0.9.75/danielutils/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,45 +2,41 @@
     data-structures and more that make my development workflow faster
 """
 # =================================================================
 # ============================= LEAFS =============================
 # =================================================================
 from .path import *
 from .date_time import *
-from .multi_x import *
-from .loops import *
-from .signals import *
 from .aliases import *
 from .exceptions import PrintCatchOne
 from .snippets import *
 from .abstractions import *
-from .imports import *
+from .protocols import *
 # =================================================================
 # ========================= ORDER MATTERS =========================
 # =================================================================
 
 from .reflection import *
 from .decorators import *
 
 # ========== NEEDS REFLECTION ==========
-from .threads import *
-from .my_tqdm import *
+from .tqdm_ import *
 # ========== NEEDS DECORATORS ==========
 from .colors import *
 # ========== NEEDS BOTH ==========
 
 from .functions import *
-from .files_and_folders import *
+from .io_ import *
 from .system import *
 from .text import *
 from .conversions import *
-from .classes import *
+from .better_builtins import *
 from .time import *
 from .date import *
 from .data_structures import *
-from .math import *
+from .math_ import *
 from .system import *
-from .d_print import *
+from .print_ import *
 from .metaclasses import *
 from .generators import *
 from .university import *
-from .package_utils import *
+from .mock_ import *
```

### Comparing `danielutils-0.9.74/danielutils/aliases.py` & `danielutils-0.9.75/danielutils/aliases.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/colors.py` & `danielutils-0.9.75/danielutils/colors.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/conversions/main_conversions.py` & `danielutils-0.9.75/danielutils/conversions/main_conversions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/conversions/specialized_conversions/to_int.py` & `danielutils-0.9.75/danielutils/conversions/specialized_conversions/to_int.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/d_print.py` & `danielutils-0.9.75/danielutils/print_.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 from .functions.areoneof import areoneof
-from .math.math_print import mprint_parse_one
+from .math_.math_print import mprint_parse_one
 from .decorators import atomic, deprecate
 
 
 def mprint(*args, sep: str = " ", end: str = "\n", stream=sys.stdout) -> None:
     """Prints a formatted representation of mathematical expressions to the specified stream.
 
     Args:
```

### Comparing `danielutils-0.9.74/danielutils/data_structures/Comparer.py` & `danielutils-0.9.75/danielutils/data_structures/Comparer.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/data_structures/Stack.py` & `danielutils-0.9.75/danielutils/data_structures/Stack.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/data_structures/functions.py` & `danielutils-0.9.75/danielutils/data_structures/functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/date.py` & `danielutils-0.9.75/danielutils/date.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/decorators/atomic.py` & `danielutils-0.9.75/danielutils/decorators/atomic.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/decorators/attach.py` & `danielutils-0.9.75/danielutils/decorators/attach.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/decorators/chain_decorators.py` & `danielutils-0.9.75/danielutils/decorators/chain_decorators.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/decorators/decorate_conditionally.py` & `danielutils-0.9.75/danielutils/decorators/decorate_conditionally.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/decorators/delay_call.py` & `danielutils-0.9.75/danielutils/decorators/delay_call.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/decorators/deprecate.py` & `danielutils-0.9.75/danielutils/decorators/deprecate.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/decorators/limit_recursion.py` & `danielutils-0.9.75/danielutils/decorators/limit_recursion.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/decorators/memo.py` & `danielutils-0.9.75/danielutils/decorators/memo.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/decorators/overload.py` & `danielutils-0.9.75/danielutils/decorators/overload.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/decorators/partially_implemented.py` & `danielutils-0.9.75/danielutils/decorators/partially_implemented.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/decorators/processify.py` & `danielutils-0.9.75/danielutils/decorators/processify.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import inspect
 import functools
 import multiprocessing
 
 from ..reflection import get_prev_frame
-from ..multi_x import process_id
-import pickle
+from ..abstractions.multiprogramming import process_id
 
 
 def processify(func):
     """Modifies the function so that when calling it, a new process
     will start to run it with provided arguments. Note that no return
     value will be given.
```

### Comparing `danielutils-0.9.74/danielutils/decorators/property.py` & `danielutils-0.9.75/danielutils/decorators/property.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/decorators/threadify.py` & `danielutils-0.9.75/danielutils/decorators/threadify.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/decorators/timeout.py` & `danielutils-0.9.75/danielutils/decorators/timeout.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/decorators/validate.py` & `danielutils-0.9.75/danielutils/decorators/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
 
 # def validate(func: Callable) -> Callable:
     # """A decorator that validates the annotations and types of the arguments and return
     # value of a function.
 
     #     * 'None' is allowed as default value for everything
-    #     * Because of their use in classes, the generally accepted keywords 'self' and 'cls'
+    #     * Because of their use in better_builtins, the generally accepted keywords 'self' and 'cls'
     #     are not validated to not break intellisense when using 'Any'
 
     # Args:
     #     func (Callable): The function to be decorated.
 
     # Raises:
     #     TypeError: if the decorated object is nto a Callable
```

### Comparing `danielutils-0.9.74/danielutils/exceptions.py` & `danielutils-0.9.75/danielutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/files_and_folders.py` & `danielutils-0.9.75/danielutils/io_.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/functions/areoneof.py` & `danielutils-0.9.75/danielutils/functions/areoneof.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/functions/check_foreach.py` & `danielutils-0.9.75/danielutils/functions/check_foreach.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/functions/isoftype.py` & `danielutils-0.9.75/danielutils/functions/isoftype.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import get_args, get_origin, get_type_hints, Any, Union, TypeVar, \
-    ForwardRef, Literal, Optional, Tuple as t_tuple
+    ForwardRef, Literal, Optional, Tuple as t_tuple, Protocol
 from collections.abc import Callable, Generator, Iterable
 from ..reflection import get_python_version
 
 if get_python_version() < (3, 9):
     from typing_extensions import ParamSpec, Concatenate
 else:
 
@@ -239,25 +239,51 @@
     if isinstance(T, ForwardRef):
         name_of_type = T.__forward_arg__
         return type(V).__name__ == name_of_type
 
     return isinstance(V, T)
 
 
+def __handle_protocol(params: tuple) -> bool:
+    from ..reflection import FunctionDeclaration
+    V, T, strict, obj_origin, obj_args, obj_hints, t_origin, t_args, t_hints = params
+    if not isoftype(V, type):
+        return False
+
+    if not isinstance(V, t_origin):
+        return False
+
+    declared_funcs: list[FunctionDeclaration] = list(FunctionDeclaration.get_declared_functions(V))
+    required_funcs: list[FunctionDeclaration] = list(FunctionDeclaration.get_declared_functions(t_origin))
+
+    for i, req_func in enumerate(required_funcs):
+        if req_func.has_generics:
+            if req_func.return_type in req_func.generics:
+                new_req_func = req_func.duplicate(
+                    return_type=t_args[req_func.generics.index(req_func.return_type)].__name__)
+                required_funcs[i] = new_req_func
+            for arg in required_funcs[i].arguments:
+                for generic in req_func.generics:
+                    if arg.type is not None and generic in arg.type:
+                        pass
+    return len(set(required_funcs) - set(declared_funcs)) == 0
+
+
 HANDLERS = {
     list: __handle_list_set_iterable,
     tuple: __handle_tuple,
     dict: __handle_dict,
     set: __handle_list_set_iterable,
     Iterable: __handle_list_set_iterable,
     Union: __handle_union,
     # implicit_union_type: __handle_union,
     Generator: __handle_generator,
     Literal: __handle_literal,
-    Callable: __handle_callable
+    Callable: __handle_callable,
+    Protocol: __handle_protocol,
 }
 
 
 def isoftype(V: Any, T: Any, /, strict: bool = True) -> bool:
     """
     Checks if an object is of a certain type.
 
@@ -284,22 +310,24 @@
     if t_args is not None and Ellipsis in t_args:
         from ..colors import warning  # pylint: disable=cyclic-import
         warning(
             "using an ellipsis (as in '...') with isoftype is ambiguous returning False")
         return False
 
     if t_origin is not None:
+        if getattr(t_origin, "_is_protocol", False):
+            t_origin = Protocol
         if t_origin in HANDLERS:
             if t_origin in (list, tuple, dict, set, dict, Iterable):
                 if not isinstance(V, t_origin):
                     return False
             return HANDLERS[t_origin](params)
 
         from ..colors import warning  # pylint: disable=cyclic-import
-        from ..reflection.get_traceback import get_traceback
+        from reflection.interpreter.get_traceback import get_traceback
         warning(
             f"In function isoftype, unhandled t_origin: {t_origin} returning True. stacktrace:")
         print(*get_traceback())
         return True
 
     return __handle_type_origin(params)
```

### Comparing `danielutils-0.9.74/danielutils/functions/isoneof.py` & `danielutils-0.9.75/danielutils/functions/isoneof.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/functions/powerset.py` & `danielutils-0.9.75/danielutils/functions/powerset.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/functions/types_subseteq.py` & `danielutils-0.9.75/danielutils/functions/types_subseteq.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/generators/conditional_generator.py` & `danielutils-0.9.75/danielutils/generators/conditional_generator.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/generators/join_generators.py` & `danielutils-0.9.75/danielutils/generators/join_generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Generator, Any, Tuple as t_tuple
 from threading import Semaphore  # , Condition
 from ..decorators import threadify
 from ..data_structures import AtomicQueue, Queue
-from ..classes import AtomicCounter
+from ..better_builtins import AtomicCounter
 # from ..Print import aprint
 from ..reflection import get_python_version
 
 if get_python_version() >= (3, 9):
     from builtins import tuple as t_tuple  # type:ignore
```

### Comparing `danielutils-0.9.74/danielutils/internet.py` & `danielutils-0.9.75/danielutils/internet.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/metaclasses/Interface.py` & `danielutils-0.9.75/danielutils/metaclasses/Interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         def __interface_handler__(*args, **kwargs):
             raise NotImplementedError(
                 f"Interface {cls} must be implemented")
         return __interface_handler__
 
 
 class Interface(type):
-    """This is a metaclass that will enable classes that inherit it directly (or indirectly)
+    """This is a metaclass that will enable better_builtins that inherit it directly (or indirectly)
         to behave like interfaces in OOP languages like java
     """
     IMPLICIT_ABSTRACT = r"\s*def \w+\(.*?\)(?:\s*->\s*\w+)?:\n(?:\s*\"{3}.*\"{3}\n)?\s*\.{3}\n"
     KEY = "__is_interface__"
     FUNC_KEY = "__is_abstractmethod__"
 
     @staticmethod
```

### Comparing `danielutils-0.9.74/danielutils/metaclasses/atomic_class_meta.py` & `danielutils-0.9.75/danielutils/metaclasses/atomic_class_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/metaclasses/implicit_data_deleter_meta.py` & `danielutils-0.9.75/danielutils/metaclasses/implicit_data_deleter_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/metaclasses/instance_cache_meta.py` & `danielutils-0.9.75/danielutils/metaclasses/instance_cache_meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..classes.counter import Counter
+from ..better_builtins.counter import Counter
 
 
 class InstanceCacheMeta(type):
     """Adds automatic caching of all instances of the class
 
         Adds the following API to the class
         @staticmethod
```

### Comparing `danielutils-0.9.74/danielutils/metaclasses/overload_meta.py` & `danielutils-0.9.75/danielutils/metaclasses/overload_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/my_tqdm.py` & `danielutils-0.9.75/danielutils/tqdm_.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/path.py` & `danielutils-0.9.75/danielutils/path.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/reflection/__init__.py` & `danielutils-0.9.75/danielutils/reflection/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from .system_reflections import *  # this has to be first, the order matters!
-from .file_reflection import *
-from .function_reflections import *
-from .get_traceback import *
-from .module_reflections import *
-from .class_reflection import *
-from .callstack import *
-from .interpreter import *
+from .interpreter import *  # this has to be first, the order matters!
+from .file import *
+from .function import *
+from .class_ import *
+from .module import *
+
 # def get_class(module_name: str, class_name: str) -> type:
 #     """dynammically loads the module and returns the class from this file
 
 #     Args:
 #         module_name (str): name of python module, (typically a file name without extention)
 #         class_name (str): the name of the wanted class
```

### Comparing `danielutils-0.9.74/danielutils/system/independent.py` & `danielutils-0.9.75/danielutils/system/independent.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/system/windows/win32_ctime.py` & `danielutils-0.9.75/danielutils/system/windows/win32_ctime.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/system/windows/windows.py` & `danielutils-0.9.75/danielutils/system/windows/windows.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/text.py` & `danielutils-0.9.75/danielutils/text.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/time.py` & `danielutils-0.9.75/danielutils/time.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils/university/databases/all.py` & `danielutils-0.9.75/danielutils/university/databases/all.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.74/danielutils.egg-info/PKG-INFO` & `danielutils-0.9.75/danielutils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.9.74
+Version: 0.9.75
 Summary: A python utils library for things I find useful
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,30 +22,30 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/danielnachumdev/danielutils
 Project-URL: Bug Tracker, https://github.com/danielnachumdev/danielutils/issues
-Keywords: functions,decorators,methods,classes,metaclasses
+Keywords: functions,decorators,methods,better_builtins,metaclasses
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.9.74
+# danielutils v=0.9.75
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 # Showcase
 In [this](./READMES/) folder you can check out some more in depth showcase of some of the topics I have covered in this package
```

### Comparing `danielutils-0.9.74/danielutils.egg-info/SOURCES.txt` & `danielutils-0.9.75/danielutils.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -3,50 +3,30 @@
 pyproject.toml
 setup.py
 ./LICENSE
 ./README.md
 danielutils/__init__.py
 danielutils/aliases.py
 danielutils/colors.py
-danielutils/d_print.py
+danielutils/convenience.py
 danielutils/date.py
 danielutils/date_time.py
 danielutils/exceptions.py
-danielutils/files_and_folders.py
 danielutils/internet.py
-danielutils/loops.py
-danielutils/multi_x.py
-danielutils/my_tqdm.py
+danielutils/io_.py
 danielutils/path.py
+danielutils/print_.py
 danielutils/py.typed
-danielutils/relations.py
-danielutils/signals.py
 danielutils/text.py
 danielutils/time.py
+danielutils/tqdm_.py
 danielutils.egg-info/PKG-INFO
 danielutils.egg-info/SOURCES.txt
 danielutils.egg-info/dependency_links.txt
 danielutils.egg-info/top_level.txt
-danielutils/classes/Convenience.py
-danielutils/classes/Counter.py
-danielutils/classes/Tree.py
-danielutils/classes/__init__.py
-danielutils/classes/convenience.py
-danielutils/classes/counter.py
-danielutils/classes/frange.py
-danielutils/classes/repl.py
-danielutils/classes/tree.py
-danielutils/classes/sorted_builtins/__init__.py
-danielutils/classes/sorted_builtins/sset.py
-danielutils/classes/typed_builtins/__init__.py
-danielutils/classes/typed_builtins/factory.py
-danielutils/classes/typed_builtins/tdict.py
-danielutils/classes/typed_builtins/tlist.py
-danielutils/classes/typed_builtins/tset.py
-danielutils/classes/typed_builtins/ttuple.py
 danielutils/conversions/__init__.py
 danielutils/conversions/main_conversions.py
 danielutils/conversions/specialized_conversions/__init__.py
 danielutils/conversions/specialized_conversions/to_hex.py
 danielutils/conversions/specialized_conversions/to_int.py
 danielutils/data_structures/Comparer.py
 danielutils/data_structures/Stack.py
@@ -78,41 +58,27 @@
 danielutils/functions/isoneof.py
 danielutils/functions/powerset.py
 danielutils/functions/types_subseteq.py
 danielutils/generators/__init__.py
 danielutils/generators/conditional_generator.py
 danielutils/generators/generator_from_stream.py
 danielutils/generators/join_generators.py
-danielutils/math/__init__.py
-danielutils/math/constants.py
-danielutils/math/functions.py
-danielutils/math/math_print.py
-danielutils/math/math_symbols.py
 danielutils/metaclasses/Interface.py
 danielutils/metaclasses/__init__.py
 danielutils/metaclasses/atomic_class_meta.py
 danielutils/metaclasses/implicit_data_deleter_meta.py
 danielutils/metaclasses/instance_cache_meta.py
 danielutils/metaclasses/interface.py
 danielutils/metaclasses/overload_meta.py
 danielutils/reflection/__init__.py
-danielutils/reflection/class_reflection.py
-danielutils/reflection/file_reflection.py
-danielutils/reflection/function_reflections.py
-danielutils/reflection/get_traceback.py
-danielutils/reflection/module_reflections.py
-danielutils/reflection/system_reflections.py
 danielutils/snippets/__init__.py
 danielutils/snippets/try_get.py
 danielutils/system/__init__.py
 danielutils/system/independent.py
 danielutils/system/windows/__init__.py
 danielutils/system/windows/win32_ctime.py
 danielutils/system/windows/windows.py
 danielutils/system/windows/utils/__init__.py
 danielutils/system/windows/utils/filetime.py
-danielutils/threads/__init__.py
-danielutils/threads/worker.py
-danielutils/threads/worker_pool.py
 danielutils/university/__init__.py
 danielutils/university/databases/__init__.py
 danielutils/university/databases/all.py
```

### Comparing `danielutils-0.9.74/pyproject.toml` & `danielutils-0.9.75/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "danielutils"
-version = "0.9.74"
+version = "0.9.75"
 authors = [
     { name = "danielnachumdev", email = "danielnachumdev@gmail.com" },
 ]
 dependencies = []
-keywords = ['functions', 'decorators', 'methods', 'classes', 'metaclasses']
+keywords = ['functions', 'decorators', 'methods', 'better_builtins', 'metaclasses']
 license = { "file" = "./LICENSE" }
 description = "A python utils library for things I find useful"
 readme = "./README.md"
 requires-python = ">=3.8.0"
 classifiers = [
 	"Development Status :: 3 - Alpha",
 	"Intended Audience :: Developers",
```


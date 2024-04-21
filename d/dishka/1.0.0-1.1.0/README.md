# Comparing `tmp/dishka-1.0.0.tar.gz` & `tmp/dishka-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dishka-1.0.0.tar", last modified: Tue Apr  2 21:17:26 2024, max compression
+gzip compressed data, was "dishka-1.1.0.tar", last modified: Sun Apr 21 10:25:11 2024, max compression
```

## Comparing `dishka-1.0.0.tar` & `dishka-1.1.0.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.075320 dishka-1.0.0/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    11357 2024-01-25 16:39:00.000000 dishka-1.0.0/LICENSE
--rw-r--r--   0 tishka17  (1000) tishka17  (1000)    12015 2024-04-02 21:17:26.075320 dishka-1.0.0/PKG-INFO
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    11078 2024-04-01 21:05:02.000000 dishka-1.0.0/README.md
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1097 2024-04-02 21:17:01.000000 dishka-1.0.0/pyproject.toml
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       38 2024-04-02 21:17:26.075320 dishka-1.0.0/setup.cfg
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.071320 dishka-1.0.0/src/
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.071320 dishka-1.0.0/src/dishka/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      807 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/__init__.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.071320 dishka-1.0.0/src/dishka/_adaptix/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      635 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/common.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     5323 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/feature_requirement.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.071320 dishka-1.0.0/src/dishka/_adaptix/type_tools/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      540 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/type_tools/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     4756 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/type_tools/basic_utils.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1441 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/type_tools/constants.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3877 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/type_tools/generic_resolver.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1827 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/type_tools/implicit_params.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1059 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/type_tools/norm_utils.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    25734 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/type_tools/normalize_type.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6943 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/async_container.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6592 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/container.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      476 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/container_objects.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.071320 dishka-1.0.0/src/dishka/dependency_source/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      510 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/dependency_source/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1038 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/dependency_source/alias.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1416 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/dependency_source/composite.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1515 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/dependency_source/context_var.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1324 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/dependency_source/decorator.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2164 2024-03-27 22:27:14.000000 dishka-1.0.0/src/dishka/dependency_source/factory.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      905 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/dependency_source/make_alias.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      678 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/dependency_source/make_context_var.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1462 2024-04-01 21:05:02.000000 dishka-1.0.0/src/dishka/dependency_source/make_decorator.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    15125 2024-04-02 21:16:55.000000 dishka-1.0.0/src/dishka/dependency_source/make_factory.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1949 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/dependency_source/unpack_provides.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.071320 dishka-1.0.0/src/dishka/entities/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-29 00:39:11.000000 dishka-1.0.0/src/dishka/entities/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       40 2024-02-29 00:39:11.000000 dishka-1.0.0/src/dishka/entities/component.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1178 2024-04-02 21:16:55.000000 dishka-1.0.0/src/dishka/entities/depends_marker.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1123 2024-03-04 22:02:38.000000 dishka-1.0.0/src/dishka/entities/key.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      347 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/entities/provides_marker.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      783 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/entities/scope.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2730 2024-03-26 23:39:41.000000 dishka-1.0.0/src/dishka/error_rendering.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1715 2024-03-04 22:02:38.000000 dishka-1.0.0/src/dishka/exceptions.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3397 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/factory_compiler.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.071320 dishka-1.0.0/src/dishka/integrations/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-08 23:15:26.000000 dishka-1.0.0/src/dishka/integrations/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2279 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/integrations/aiogram.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1232 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/integrations/aiohttp.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2445 2024-03-04 22:02:38.000000 dishka-1.0.0/src/dishka/integrations/arq.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     5268 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/integrations/base.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1417 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/integrations/fastapi.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1734 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/integrations/faststream.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1421 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/integrations/flask.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1749 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/integrations/litestar.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1248 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/integrations/starlette.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2226 2024-04-02 21:16:55.000000 dishka-1.0.0/src/dishka/integrations/taskiq.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1379 2024-03-28 15:28:45.000000 dishka-1.0.0/src/dishka/integrations/telebot.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6369 2024-04-01 21:05:02.000000 dishka-1.0.0/src/dishka/provider.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/py.typed
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    12796 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/registry.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.071320 dishka-1.0.0/src/dishka.egg-info/
--rw-r--r--   0 tishka17  (1000) tishka17  (1000)    12015 2024-04-02 21:17:26.000000 dishka-1.0.0/src/dishka.egg-info/PKG-INFO
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1957 2024-04-02 21:17:26.000000 dishka-1.0.0/src/dishka.egg-info/SOURCES.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        1 2024-04-02 21:17:26.000000 dishka-1.0.0/src/dishka.egg-info/dependency_links.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       50 2024-04-02 21:17:26.000000 dishka-1.0.0/src/dishka.egg-info/requires.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        7 2024-04-02 21:17:26.000000 dishka-1.0.0/src/dishka.egg-info/top_level.txt
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.330739 dishka-1.1.0/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    11357 2024-01-25 16:39:00.000000 dishka-1.1.0/LICENSE
+-rw-r--r--   0 tishka17  (1000) tishka17  (1000)    12011 2024-04-21 10:25:11.330739 dishka-1.1.0/PKG-INFO
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    11074 2024-04-21 10:24:38.000000 dishka-1.1.0/README.md
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1097 2024-04-21 10:24:45.000000 dishka-1.1.0/pyproject.toml
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       38 2024-04-21 10:25:11.330739 dishka-1.1.0/setup.cfg
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.326739 dishka-1.1.0/src/
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.330739 dishka-1.1.0/src/dishka/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      843 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/__init__.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.330739 dishka-1.1.0/src/dishka/_adaptix/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      639 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/common.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     5460 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/feature_requirement.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.330739 dishka-1.1.0/src/dishka/_adaptix/type_tools/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      609 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/type_tools/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     4141 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/type_tools/basic_utils.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      994 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/type_tools/constants.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1530 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/type_tools/fundamentals.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3907 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/type_tools/generic_resolver.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1828 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/type_tools/implicit_params.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1059 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/type_tools/norm_utils.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    25528 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/_adaptix/type_tools/normalize_type.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     7025 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/async_container.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6664 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/container.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      476 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/container_objects.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.330739 dishka-1.1.0/src/dishka/dependency_source/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      542 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/dependency_source/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1038 2024-03-19 22:45:31.000000 dishka-1.1.0/src/dishka/dependency_source/alias.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1416 2024-03-19 22:45:31.000000 dishka-1.1.0/src/dishka/dependency_source/composite.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1515 2024-03-19 22:45:31.000000 dishka-1.1.0/src/dishka/dependency_source/context_var.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1324 2024-03-19 22:45:31.000000 dishka-1.1.0/src/dishka/dependency_source/decorator.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2164 2024-03-27 22:27:14.000000 dishka-1.1.0/src/dishka/dependency_source/factory.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      905 2024-03-19 22:45:31.000000 dishka-1.1.0/src/dishka/dependency_source/make_alias.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      678 2024-03-19 22:45:31.000000 dishka-1.1.0/src/dishka/dependency_source/make_context_var.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1462 2024-04-01 21:05:02.000000 dishka-1.1.0/src/dishka/dependency_source/make_decorator.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    16303 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/dependency_source/make_factory.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1949 2024-03-19 22:45:31.000000 dishka-1.1.0/src/dishka/dependency_source/unpack_provides.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.330739 dishka-1.1.0/src/dishka/entities/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-29 00:39:11.000000 dishka-1.1.0/src/dishka/entities/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       40 2024-02-29 00:39:11.000000 dishka-1.1.0/src/dishka/entities/component.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1178 2024-04-20 19:15:28.000000 dishka-1.1.0/src/dishka/entities/depends_marker.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1123 2024-03-04 22:02:38.000000 dishka-1.1.0/src/dishka/entities/key.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      347 2024-03-19 22:45:31.000000 dishka-1.1.0/src/dishka/entities/provides_marker.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      783 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/entities/scope.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2730 2024-03-26 23:39:41.000000 dishka-1.1.0/src/dishka/error_rendering.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1715 2024-03-04 22:02:38.000000 dishka-1.1.0/src/dishka/exceptions.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3398 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/factory_compiler.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.330739 dishka-1.1.0/src/dishka/integrations/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-08 23:15:26.000000 dishka-1.1.0/src/dishka/integrations/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2279 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/integrations/aiogram.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1232 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/integrations/aiohttp.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2445 2024-03-04 22:02:38.000000 dishka-1.1.0/src/dishka/integrations/arq.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     5268 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/integrations/base.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1417 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/integrations/fastapi.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3676 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/integrations/faststream.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1421 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/integrations/flask.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1749 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/integrations/litestar.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1617 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/integrations/sanic.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1248 2024-03-24 23:55:01.000000 dishka-1.1.0/src/dishka/integrations/starlette.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2226 2024-04-02 21:16:55.000000 dishka-1.1.0/src/dishka/integrations/taskiq.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1379 2024-03-28 15:28:45.000000 dishka-1.1.0/src/dishka/integrations/telebot.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6855 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/provider.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-18 18:04:06.000000 dishka-1.1.0/src/dishka/py.typed
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    13009 2024-04-21 10:24:38.000000 dishka-1.1.0/src/dishka/registry.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-21 10:25:11.330739 dishka-1.1.0/src/dishka.egg-info/
+-rw-r--r--   0 tishka17  (1000) tishka17  (1000)    12011 2024-04-21 10:25:11.000000 dishka-1.1.0/src/dishka.egg-info/PKG-INFO
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2037 2024-04-21 10:25:11.000000 dishka-1.1.0/src/dishka.egg-info/SOURCES.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        1 2024-04-21 10:25:11.000000 dishka-1.1.0/src/dishka.egg-info/dependency_links.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       50 2024-04-21 10:25:11.000000 dishka-1.1.0/src/dishka.egg-info/requires.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        7 2024-04-21 10:25:11.000000 dishka-1.1.0/src/dishka.egg-info/top_level.txt
```

### Comparing `dishka-1.0.0/LICENSE` & `dishka-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/PKG-INFO` & `dishka-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dishka
-Version: 1.0.0
+Version: 1.1.0
 Summary: Minimal DI framework
 Author-email: Andrey Tikhonov <17@itishka.org>
 License: Apache-2.0
 Project-URL: Source, https://github.com/reagento/dishka
 Project-URL: Homepage, https://github.com/reagento/dishka
 Project-URL: Documentation, https://dishka.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/reagento/dishka/issues
@@ -55,15 +55,15 @@
 
 1. Install dishka
 
 ```shell
 pip install dishka
 ```
 
-2. Create `Provider` instance. It is only used co setup all factories providing your objects.
+2. Create `Provider` instance. It is only used to setup all factories providing your objects.
 
 ```python
 from dishka import Provider
 
 provider = Provider()
 ```
 
@@ -263,15 +263,15 @@
 class MyProvider(Provider):
     scope = Scope.REQUEST
 
     app = from_context(provides=App, scope=Scope.APP)
     request = from_context(provides=RequestClass)
 
     @provide
-    async def get_a(self, request: RequestClass, app: App) -> A:
+    def get_a(self, request: RequestClass, app: App) -> A:
         ...
 
 container = make_container(MyProvider(), context={App: app})
 with container(context={RequestClass: request_instance}) as request_container:
     pass
 ```
 
@@ -281,13 +281,13 @@
 container = make_container(MyProvider(), OtherProvider())
 ```
 
 * Tired of providing `scope==` for each depedency? Set it inside your `Provider` class and all dependencies with no scope will use it.
 
 ```python
 class MyProvider(Provider):
-   scope=Scope.APP
+   scope = Scope.APP
 
    @provide
    async def get_a(self) -> A:
       return A()
 ```
```

### Comparing `dishka-1.0.0/README.md` & `dishka-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 1. Install dishka
 
 ```shell
 pip install dishka
 ```
 
-2. Create `Provider` instance. It is only used co setup all factories providing your objects.
+2. Create `Provider` instance. It is only used to setup all factories providing your objects.
 
 ```python
 from dishka import Provider
 
 provider = Provider()
 ```
 
@@ -240,15 +240,15 @@
 class MyProvider(Provider):
     scope = Scope.REQUEST
 
     app = from_context(provides=App, scope=Scope.APP)
     request = from_context(provides=RequestClass)
 
     @provide
-    async def get_a(self, request: RequestClass, app: App) -> A:
+    def get_a(self, request: RequestClass, app: App) -> A:
         ...
 
 container = make_container(MyProvider(), context={App: app})
 with container(context={RequestClass: request_instance}) as request_container:
     pass
 ```
 
@@ -258,13 +258,13 @@
 container = make_container(MyProvider(), OtherProvider())
 ```
 
 * Tired of providing `scope==` for each depedency? Set it inside your `Provider` class and all dependencies with no scope will use it.
 
 ```python
 class MyProvider(Provider):
-   scope=Scope.APP
+   scope = Scope.APP
 
    @provide
    async def get_a(self) -> A:
       return A()
 ```
```

### Comparing `dishka-1.0.0/pyproject.toml` & `dishka-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "dishka"
-version = "1.0.0"
+version = "1.1.0"
 readme = "README.md"
 authors = [
     { name = "Andrey Tikhonov", email = "17@itishka.org" },
 ]
 license = { text = "Apache-2.0" }
 description = "Minimal DI framework"
 requires-python = ">=3.10"
```

### Comparing `dishka-1.0.0/src/dishka/__init__.py` & `dishka-1.1.0/src/dishka/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 __all__ = [
     "AnyOf",
     "make_async_container", "AsyncContainer",
     "DEFAULT_COMPONENT", "Component",
     "make_container", "Container", "FromComponent",
     "Provider",
-    "alias", "decorate", "from_context", "provide", "DependencyKey",
+    "alias", "decorate", "from_context", "provide", "provide_all",
+    "DependencyKey",
     "FromDishka",
     "BaseScope", "Scope", "new_scope",
 ]
 
 from .async_container import AsyncContainer, make_async_container
 from .container import Container, make_container
 from .dependency_source import (
     alias,
     decorate,
     from_context,
     provide,
+    provide_all,
 )
 from .entities.component import DEFAULT_COMPONENT, Component
 from .entities.depends_marker import FromDishka
 from .entities.key import DependencyKey, FromComponent
 from .entities.provides_marker import AnyOf
 from .entities.scope import BaseScope, Scope, new_scope
 from .provider import Provider
```

### Comparing `dishka-1.0.0/src/dishka/_adaptix/common.py` & `dishka-1.1.0/src/dishka/_adaptix/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import TYPE_CHECKING, Any, Callable, Tuple, Type, TypeVar, Union
 
-K_contra = TypeVar('K_contra', contravariant=True)
-V_co = TypeVar('V_co', covariant=True)
-T = TypeVar('T')
+K_contra = TypeVar("K_contra", contravariant=True)
+V_co = TypeVar("V_co", covariant=True)
+T = TypeVar("T")
 
 Loader = Callable[[Any], V_co]
 Dumper = Callable[[K_contra], Any]
 Converter = Callable[..., Any]
-Coercer = Callable[[Any], Any]
+Coercer = Callable[[Any, Any], Any]
+OneArgCoercer = Callable[[Any], Any]
 
 TypeHint = Any
 
 VarTuple = Tuple[T, ...]
 
 Catchable = Union[Type[BaseException], VarTuple[Type[BaseException]]]
 
 # https://github.com/python/typing/issues/684#issuecomment-548203158
 if TYPE_CHECKING:
-    EllipsisType = ellipsis  # pylint: disable=undefined-variable  # noqa: F821
+    EllipsisType = ellipsis  # noqa: F821
 else:
     EllipsisType = type(Ellipsis)
```

### Comparing `dishka-1.0.0/src/dishka/_adaptix/feature_requirement.py` & `dishka-1.1.0/src/dishka/_adaptix/feature_requirement.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 def _false():
     return False
 
 
 class Requirement(ABC):
-    __slots__ = ('is_meet', '__bool__', '__dict__')
+    __slots__ = ("is_meet", "__bool__", "__dict__")
 
     def __init__(self):
         self.is_meet = self._evaluate()
         self.__bool__ = _true if self.is_meet else _false
 
     @abstractmethod
     def _evaluate(self) -> bool:
@@ -56,15 +56,15 @@
             importlib.metadata.distribution(self.distribution_name)
         except importlib.metadata.PackageNotFoundError:
             return False
         return True
 
     @property
     def fail_reason(self) -> str:
-        return f'Installed distribution {self.distribution_name!r} is required'
+        return f"Installed distribution {self.distribution_name!r} is required"
 
 
 class DistributionVersionRequirement(DistributionRequirement):
     # Pattern from PEP 440
     _VERSION_PATTERN = r"""
         v?
         (?:
@@ -120,36 +120,36 @@
         return tuple(reversed(tuple(itertools.dropwhile(lambda x: x == 0, reversed(tuple(data))))))
 
     def _make_comparator(self, version: str) -> VarTuple[Any]:
         match = self._version_regex.match(version)
         if match is None:
             raise ValueError
         return (
-            match.group('epoch') or 0,
-            self._remove_trailing_zeros(int(i) for i in match.group('release').split('.')),
-            match.group('pre') is not None,
-            match.group('dev') is not None,
+            match.group("epoch") or 0,
+            self._remove_trailing_zeros(int(i) for i in match.group("release").split(".")),
+            match.group("pre") is not None,
+            match.group("dev") is not None,
         )
 
     @property
     def fail_reason(self) -> str:
-        return f'Installed distribution {self.distribution_name!r} of {self.min_version!r} is required'
+        return f"Installed distribution {self.distribution_name!r} of {self.min_version!r} is required"
 
 
 class PythonImplementationRequirement(Requirement):
     def __init__(self, implementation_name: str):
         self.implementation_name = implementation_name
         super().__init__()
 
     def _evaluate(self) -> bool:
         return sys.implementation.name == self.implementation_name
 
     @property
     def fail_reason(self) -> str:
-        return f'{self.implementation_name} is required'
+        return f"{self.implementation_name} is required"
 
 
 HAS_PY_39 = PythonVersionRequirement((3, 9))
 HAS_ANNOTATED = HAS_PY_39
 HAS_STD_CLASSES_GENERICS = HAS_PY_39
 
 HAS_PY_310 = PythonVersionRequirement((3, 10))
@@ -164,15 +164,18 @@
 HAS_SELF_TYPE = HAS_PY_311
 HAS_TV_TUPLE = HAS_PY_311
 HAS_UNPACK = HAS_PY_311
 
 HAS_PY_312 = PythonVersionRequirement((3, 12))
 HAS_TV_SYNTAX = HAS_PY_312
 
-HAS_SUPPORTED_ATTRS_PKG = DistributionVersionRequirement('attrs', '21.3.0')
-HAS_ATTRS_PKG = DistributionRequirement('attrs')
+HAS_SUPPORTED_ATTRS_PKG = DistributionVersionRequirement("attrs", "21.3.0")
+HAS_ATTRS_PKG = DistributionRequirement("attrs")
 
-HAS_SUPPORTED_SQLALCHEMY_PKG = DistributionVersionRequirement('sqlalchemy', '2.0.0')
-HAS_SQLALCHEMY_PKG = DistributionRequirement('sqlalchemy')
+HAS_SUPPORTED_SQLALCHEMY_PKG = DistributionVersionRequirement("sqlalchemy", "2.0.0")
+HAS_SQLALCHEMY_PKG = DistributionRequirement("sqlalchemy")
 
-IS_CPYTHON = PythonImplementationRequirement('cpython')
-IS_PYPY = PythonImplementationRequirement('pypy')
+HAS_SUPPORTED_PYDANTIC_PKG = DistributionVersionRequirement("pydantic", "2.0.0")
+HAS_PYDANTIC_PKG = DistributionRequirement("pydantic")
+
+IS_CPYTHON = PythonImplementationRequirement("cpython")
+IS_PYPY = PythonImplementationRequirement("pypy")
```

### Comparing `dishka-1.0.0/src/dishka/_adaptix/type_tools/__init__.py` & `dishka-1.1.0/src/dishka/_adaptix/type_tools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from .basic_utils import (
     create_union,
-    get_all_type_hints,
     is_bare_generic,
     is_generic,
     is_generic_class,
     is_named_tuple_class,
     is_new_type,
     is_parametrized,
     is_protocol,
     is_subclass_soft,
     is_typed_dict_class,
     is_user_defined_generic,
-    strip_alias,
 )
+from .fundamentals import get_all_type_hints, get_generic_args, get_type_vars, is_pydantic_class, strip_alias
 from .norm_utils import is_class_var, strip_tags
 from .normalize_type import (
     AnyNormTypeVarLike,
     BaseNormType,
     NormParamSpecMarker,
     NormTV,
     NormTVTuple,
```

### Comparing `dishka-1.0.0/src/dishka/_adaptix/type_tools/basic_utils.py` & `dishka-1.1.0/src/dishka/_adaptix/type_tools/basic_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,101 +1,69 @@
 import types
 import typing
-from typing import (
-    Any,
-    Dict,
-    ForwardRef,
-    Generic,
-    Iterable,
-    Protocol,
-    TypedDict,
-    TypeVar,
-    Union,
-    get_args,
-    get_origin,
-    get_type_hints,
-)
+from typing import Any, Dict, ForwardRef, Generic, NewType, Protocol, TypedDict, TypeVar, Union
 
 from ..common import TypeHint, VarTuple
 from ..feature_requirement import HAS_ANNOTATED, HAS_PY_39, HAS_PY_312, HAS_STD_CLASSES_GENERICS
 from .constants import BUILTIN_ORIGIN_TO_TYPEVARS
-
-TYPED_DICT_MCS = type(types.new_class("_TypedDictSample", (TypedDict,), {}))
-
-
-def strip_alias(type_hint: TypeHint) -> TypeHint:
-    origin = get_origin(type_hint)
-    return type_hint if origin is None else origin
+from .fundamentals import get_generic_args, get_type_vars, strip_alias
 
 
 def is_subclass_soft(cls, classinfo) -> bool:
-    """Acts like builtin issubclass,
-     but returns False instead of rising TypeError
-    """
+    """Acts like builtin issubclass, but returns False instead of rising TypeError"""
     try:
         return issubclass(cls, classinfo)
     except TypeError:
         return False
 
 
-def has_attrs(obj, attrs: Iterable[str]) -> bool:
-    return all(
-        hasattr(obj, attr_name)
-        for attr_name in attrs
-    )
+_NEW_TYPE_CLS = type(NewType("", None))
 
 
 def is_new_type(tp) -> bool:
-    return has_attrs(tp, ['__supertype__', '__name__'])
+    return isinstance(tp, _NEW_TYPE_CLS)
+
+
+_TYPED_DICT_MCS = type(types.new_class("_TypedDictSample", (TypedDict,), {}))
 
 
 def is_typed_dict_class(tp) -> bool:
-    return isinstance(tp, TYPED_DICT_MCS)
+    return isinstance(tp, _TYPED_DICT_MCS)
 
 
-NAMED_TUPLE_METHODS = ('_fields', '_field_defaults', '_make', '_replace', '_asdict')
+_NAMED_TUPLE_METHODS = ("_fields", "_field_defaults", "_make", "_replace", "_asdict")
 
 
 def is_named_tuple_class(tp) -> bool:
     return (
         is_subclass_soft(tp, tuple)
-        and
-        has_attrs(tp, NAMED_TUPLE_METHODS)
+        and all(
+            hasattr(tp, attr_name)
+            for attr_name in _NAMED_TUPLE_METHODS
+        )
     )
 
 
 def is_protocol(tp):
     if not isinstance(tp, type):
         return False
 
     return Protocol in tp.__bases__
 
 
 def create_union(args: tuple):
     return Union[args]
 
 
-if HAS_ANNOTATED:
-    def get_all_type_hints(obj, globalns=None, localns=None):
-        return get_type_hints(obj, globalns, localns, include_extras=True)
-else:
-    get_all_type_hints = get_type_hints
-
-
 def is_parametrized(tp: TypeHint) -> bool:
-    return bool(get_args(tp))
-
-
-def get_type_vars(tp: TypeHint) -> VarTuple[TypeVar]:
-    return getattr(tp, '__parameters__', ())
+    return bool(get_generic_args(tp))
 
 
 if HAS_PY_312:
     def is_user_defined_generic(tp: TypeHint) -> bool:
-        # pylint: disable=no-member
         return (
             bool(get_type_vars(tp))
             and (
                 is_subclass_soft(strip_alias(tp), Generic)
                 or isinstance(tp, typing.TypeAliasType)  # type: ignore[attr-defined]
             )
         )
@@ -117,15 +85,16 @@
             and not is_parametrized(tp)
             and (
                 bool(HAS_STD_CLASSES_GENERICS) or not isinstance(tp, type)
             )
         )
         or (
             bool(HAS_ANNOTATED)
-            and get_origin(tp) == typing.Annotated
+            and strip_alias(tp) == typing.Annotated
+            and tp != typing.Annotated
             and is_generic(tp.__origin__)
         )
     )
 
 
 def is_bare_generic(tp: TypeHint) -> bool:
     """Check if the type could be parameterized, excluding type aliases (list[T] etc.)"""
@@ -152,29 +121,25 @@
             issubclass(cls, Generic)  # type: ignore[arg-type]
             and bool(cls.__parameters__)  # type: ignore[attr-defined]
         )
     )
 
 
 def get_type_vars_of_parametrized(tp: TypeHint) -> VarTuple[TypeVar]:
-    try:
-        params = tp.__parameters__
-    except AttributeError:
+    params = get_type_vars(tp)
+    if not params:
         return ()
-
     if isinstance(tp, type):
         if HAS_STD_CLASSES_GENERICS and isinstance(tp, types.GenericAlias):
             return params
         return ()
-    if get_origin(tp) is not None and get_args(tp) == ():
+    if strip_alias(tp) != tp and get_generic_args(tp) == ():
         return ()
     return params
 
 
 if HAS_PY_39:
     def eval_forward_ref(namespace: Dict[str, Any], forward_ref: ForwardRef):
-        # pylint: disable=protected-access
         return forward_ref._evaluate(namespace, None, frozenset())
 else:
     def eval_forward_ref(namespace: Dict[str, Any], forward_ref: ForwardRef):
-        # pylint: disable=protected-access
         return forward_ref._evaluate(namespace, None)  # type: ignore[call-arg]
```

### Comparing `dishka-1.0.0/src/dishka/_adaptix/type_tools/constants.py` & `dishka-1.1.0/src/dishka/_adaptix/type_tools/constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,36 @@
+# mypy: disable-error-code="dict-item"
 import collections
 import concurrent.futures
 import queue
 import re
 from os import PathLike
 from typing import Mapping, TypeVar
 
 from ..common import VarTuple
 
-_AnyStrT = TypeVar('_AnyStrT', str, bytes)
-_T1 = TypeVar('_T1')
-_T2 = TypeVar('_T2')
-_T1_co = TypeVar('_T1_co', covariant=True)
+_AnyStrT = TypeVar("_AnyStrT", str, bytes)
+_T1 = TypeVar("_T1")
+_T2 = TypeVar("_T2")
+_T1_co = TypeVar("_T1_co", covariant=True)
 _AnyStr_co = TypeVar("_AnyStr_co", str, bytes, covariant=True)
 
 BUILTIN_ORIGIN_TO_TYPEVARS: Mapping[type, VarTuple[TypeVar]] = {
-    re.Pattern: (_AnyStrT, ),  # type: ignore[dict-item]
-    re.Match: (_AnyStrT, ),  # type: ignore[dict-item]
-    PathLike: (_AnyStr_co, ),  # type: ignore[dict-item]
-    type: (_T1,),  # type: ignore[dict-item]
-    list: (_T1,),  # type: ignore[dict-item]
-    set: (_T1,),  # type: ignore[dict-item]
-    frozenset: (_T1_co, ),  # type: ignore[dict-item]
-    collections.Counter: (_T1,),  # type: ignore[dict-item]
-    collections.deque: (_T1,),  # type: ignore[dict-item]
-    dict: (_T1, _T2),  # type: ignore[dict-item]
-    collections.defaultdict: (_T1, _T2),  # type: ignore[dict-item]
-    collections.OrderedDict: (_T1, _T2),  # type: ignore[dict-item]
-    collections.ChainMap: (_T1, _T2),  # type: ignore[dict-item]
-    queue.Queue: (_T1, ),  # type: ignore[dict-item]
-    queue.PriorityQueue: (_T1, ),  # type: ignore[dict-item]
-    queue.LifoQueue: (_T1, ),  # type: ignore[dict-item]
-    queue.SimpleQueue: (_T1, ),  # type: ignore[dict-item]
-    concurrent.futures.Future: (_T1, ),  # type: ignore[dict-item]
+    re.Pattern: (_AnyStrT, ),
+    re.Match: (_AnyStrT, ),
+    PathLike: (_AnyStr_co, ),
+    type: (_T1,),
+    list: (_T1,),
+    set: (_T1,),
+    frozenset: (_T1_co, ),
+    collections.Counter: (_T1,),
+    collections.deque: (_T1,),
+    dict: (_T1, _T2),
+    collections.defaultdict: (_T1, _T2),
+    collections.OrderedDict: (_T1, _T2),
+    collections.ChainMap: (_T1, _T2),
+    queue.Queue: (_T1, ),
+    queue.PriorityQueue: (_T1, ),
+    queue.LifoQueue: (_T1, ),
+    queue.SimpleQueue: (_T1, ),
+    concurrent.futures.Future: (_T1, ),
 }
```

### Comparing `dishka-1.0.0/src/dishka/_adaptix/type_tools/generic_resolver.py` & `dishka-1.1.0/src/dishka/_adaptix/type_tools/generic_resolver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import typing
 from dataclasses import dataclass, replace
 from itertools import chain
-from typing import Callable, Collection, Dict, Generic, Hashable, Mapping, TypeVar, get_args
+from typing import Callable, Collection, Dict, Generic, Hashable, Mapping, TypeVar
 
 from ..common import TypeHint
 from ..feature_requirement import HAS_TV_TUPLE, HAS_UNPACK
+from . import get_generic_args
 from .basic_utils import get_type_vars, get_type_vars_of_parametrized, is_generic, is_parametrized, strip_alias
 from .implicit_params import fill_implicit_params
 from .normalize_type import normalize_type
 
-M = TypeVar('M')
-K = TypeVar('K', bound=Hashable)
+M = TypeVar("M")
+K = TypeVar("K", bound=Hashable)
 
 
 @dataclass
 class MembersStorage(Generic[K, M]):
     members: Mapping[K, TypeHint]
     overriden: Collection[K]
     meta: M
@@ -32,22 +33,22 @@
         return self._get_members_by_parents(tp)
 
     def _get_members_of_parametrized_generic(self, parametrized_generic) -> MembersStorage[K, M]:
         origin = strip_alias(parametrized_generic)
         members_storage = self._get_members_by_parents(origin)
         type_var_to_actual = self._get_type_var_to_actual(
             get_type_vars(origin),
-            self._unpack_args(get_args(parametrized_generic)),
+            self._unpack_args(get_generic_args(parametrized_generic)),
         )
         return replace(
             members_storage,
             members={
                 key: self._parametrize_by_dict(type_var_to_actual, tp)
                 for key, tp in members_storage.members.items()
-            }
+            },
         )
 
     def _unpack_args(self, args):
         if HAS_UNPACK and any(strip_alias(arg) == typing.Unpack for arg in args):
             return tuple(arg.source for arg in normalize_type(tuple[args]).args)
         return args
 
@@ -77,15 +78,15 @@
     def _get_members_by_parents(self, tp) -> MembersStorage[K, M]:
         members_storage = self._raw_members_getter(tp)
         if not any(
             get_type_vars_of_parametrized(tp) or isinstance(tp, TypeVar)
             for tp in members_storage.members.values()
         ):
             return members_storage
-        if not hasattr(tp, '__orig_bases__'):
+        if not hasattr(tp, "__orig_bases__"):
             return members_storage
 
         bases_members: Dict[K, TypeHint] = {}
         for base in reversed(tp.__orig_bases__):
             bases_members.update(self.get_resolved_members(base).members)
 
         return replace(
```

### Comparing `dishka-1.0.0/src/dishka/_adaptix/type_tools/implicit_params.py` & `dishka-1.1.0/src/dishka/_adaptix/type_tools/implicit_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         if HAS_TV_TUPLE and isinstance(type_var, typing.TypeVarTuple):
             return typing.Unpack[Tuple[Any, ...]]
         if type_var.__constraints__:
             return create_union(
                 tuple(
                     self._process_limit_element(type_var, constraint)
                     for constraint in type_var.__constraints__
-                )
+                ),
             )
         if type_var.__bound__ is None:
             return Any
         return self._process_limit_element(type_var, type_var.__bound__)
 
     def get_implicit_params(self, origin) -> VarTuple[TypeHint]:
         if is_user_defined_generic(origin):
@@ -42,8 +42,8 @@
         )
 
 
 def fill_implicit_params(tp: TypeHint) -> TypeHint:
     params = ImplicitParamsGetter().get_implicit_params(strip_alias(tp))
     if params:
         return tp[params]
-    raise ValueError(f'Can not derive implicit parameters for {tp}')
+    raise ValueError(f"Can not derive implicit parameters for {tp}")
```

### Comparing `dishka-1.0.0/src/dishka/_adaptix/type_tools/norm_utils.py` & `dishka-1.1.0/src/dishka/_adaptix/type_tools/norm_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     and that only indicates metadata
     """
     if norm.origin in _TYPE_TAGS:
         return strip_tags(norm.args[0])
     return norm
 
 
-N = TypeVar('N', bound=BaseNormType)
+N = TypeVar("N", bound=BaseNormType)
 
 
 def strip_annotated(value: N) -> N:
     if HAS_ANNOTATED and isinstance(value, BaseNormType) and value.origin == typing.Annotated:
         return strip_annotated(value)
     return value
```

### Comparing `dishka-1.0.0/src/dishka/_adaptix/type_tools/normalize_type.py` & `dishka-1.1.0/src/dishka/_adaptix/type_tools/normalize_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=inconsistent-return-statements,comparison-with-callable
+# ruff: noqa: RET503
 import dataclasses
 import sys
 import types
 import typing
 from abc import ABC, abstractmethod
 from collections import abc as c_abc, defaultdict
 from copy import copy
@@ -25,15 +25,14 @@
     NoReturn,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
-    get_args,
     overload,
 )
 
 from ..common import TypeHint, VarTuple
 from ..feature_requirement import (
     HAS_ANNOTATED,
     HAS_PARAM_SPEC,
@@ -45,14 +44,15 @@
     HAS_TYPE_ALIAS,
     HAS_TYPE_GUARD,
     HAS_TYPE_UNION_OP,
     HAS_TYPED_DICT_REQUIRED,
     HAS_UNPACK,
 )
 from .basic_utils import create_union, eval_forward_ref, is_new_type, is_subclass_soft, strip_alias
+from .fundamentals import get_generic_args
 from .implicit_params import ImplicitParamsGetter
 
 
 class BaseNormType(Hashable, ABC):
     @property
     @abstractmethod
     def origin(self) -> Any:
@@ -65,19 +65,19 @@
 
     @property
     @abstractmethod
     def source(self) -> TypeHint:
         ...
 
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class _BasicNormType(BaseNormType, ABC):
-    __slots__ = ('_source', '_args')
+    __slots__ = ("_source", "_args")
 
     def __init__(self, args: VarTuple[Any], *, source: TypeHint):
         self._source = source
         self._args = args
 
     @property
     def args(self) -> VarTuple[Any]:
@@ -99,19 +99,19 @@
             )
         if isinstance(other, BaseNormType):
             return False
         return NotImplemented
 
     def __repr__(self):
         args_str = f" {list(self.args)}," if self.args else ""
-        return f'<{type(self).__name__}({self.origin},{args_str} source={self._source})>'
+        return f"<{type(self).__name__}({self.origin},{args_str} source={self._source})>"
 
 
 class _NormType(_BasicNormType):
-    __slots__ = _BasicNormType.__slots__ + ('_source',)
+    __slots__ = (*_BasicNormType.__slots__, "_source")
 
     def __init__(self, origin: TypeHint, args: VarTuple[Any], *, source: TypeHint):
         self._origin = origin
         super().__init__(args, source=source)
 
     @property
     def origin(self) -> Any:
@@ -173,15 +173,15 @@
 
 
 class _AnnotatedNormType(_BasicNormType):
     @property
     def origin(self) -> Any:
         return typing.Annotated
 
-    __slots__ = _BasicNormType.__slots__ + ('_hash',)
+    __slots__ = (*_BasicNormType.__slots__, "_hash")
 
     def __init__(self, args: VarTuple[Hashable], *, source: TypeHint):
         super().__init__(args, source=source)
         self._hash = self._calc_hash()
 
     # calculate hash even if one of Annotated metadata is not hashable
     def _calc_hash(self) -> int:
@@ -202,43 +202,43 @@
 class Variance(Enum):
     INVARIANT = 0
     COVARIANT = 1
     CONTRAVARIANT = 2
     INFERRED = 3
 
     def __repr__(self):
-        return f'{type(self).__name__}.{self.name}'
+        return f"{type(self).__name__}.{self.name}"
 
 
 @dataclass
 class Bound:
     value: BaseNormType
 
 
 @dataclass
 class Constraints:
     value: VarTuple[BaseNormType]
 
 
-TypeVarLimit = Union[Bound, Constraints]  # pylint: disable=invalid-name
+TypeVarLimit = Union[Bound, Constraints]
 
 
 class NormTV(BaseNormType):
-    __slots__ = ('_var', '_limit', '_variance', '_source')
+    __slots__ = ("_var", "_limit", "_variance", "_source")
 
     def __init__(self, var: Any, limit: TypeVarLimit, *, source: TypeHint):
         self._var = var
         self._source = source
         self._limit = limit
 
         if var.__covariant__:
             self._variance = Variance.COVARIANT
         if var.__contravariant__:
             self._variance = Variance.CONTRAVARIANT
-        if getattr(var, '__infer_variance__', False):
+        if getattr(var, "__infer_variance__", False):
             self._variance = Variance.INFERRED
         self._variance = Variance.INVARIANT
 
     @property
     def origin(self) -> Any:
         return self._var
 
@@ -259,29 +259,29 @@
         return self._variance
 
     @property
     def limit(self) -> TypeVarLimit:
         return self._limit
 
     def __repr__(self):
-        return f'<{type(self).__name__}({self._var})>'
+        return f"<{type(self).__name__}({self._var})>"
 
     def __hash__(self):
         return hash(self._var)
 
     def __eq__(self, other):
         if isinstance(other, NormTV):
             return self._var == other._var
         if isinstance(other, BaseNormType):
             return False
         return NotImplemented
 
 
 class NormTVTuple(BaseNormType):
-    __slots__ = ('_var', '_source')
+    __slots__ = ("_var", "_source")
 
     def __init__(self, var: Any, *, source: TypeHint):
         self._var = var
         self._source = source
 
     @property
     def origin(self) -> Any:
@@ -296,29 +296,29 @@
         return self._source
 
     @property
     def name(self) -> str:
         return self._var.__name__
 
     def __repr__(self):
-        return f'<{type(self).__name__}({self._var})>'
+        return f"<{type(self).__name__}({self._var})>"
 
     def __hash__(self):
         return hash(self._var)
 
     def __eq__(self, other):
         if isinstance(other, NormTVTuple):
             return self._var == other._var
         if isinstance(other, BaseNormType):
             return False
         return NotImplemented
 
 
 class NormParamSpecMarker(BaseNormType, ABC):
-    __slots__ = ('_param_spec', '_source')
+    __slots__ = ("_param_spec", "_source")
 
     def __init__(self, param_spec: Any, *, source: TypeHint):
         self._param_spec = param_spec
         self._source = source
 
     @property
     def param_spec(self) -> NormTV:
@@ -355,15 +355,15 @@
         return typing.ParamSpecKwargs
 
 
 AnyNormTypeVarLike = Union[NormTV, NormTVTuple]
 
 
 class NormTypeAlias(BaseNormType):
-    __slots__ = ('_type_alias', '_args', '_norm_type_vars')
+    __slots__ = ("_type_alias", "_args", "_norm_type_vars")
 
     def __init__(self, type_alias, args: VarTuple[BaseNormType], type_vars: VarTuple[AnyNormTypeVarLike]):
         self._type_alias = type_alias
         self._args = args
         self._type_vars = type_vars
 
     @property
@@ -400,19 +400,19 @@
     def __hash__(self):
         return hash(self._type_alias)
 
 
 _PARAM_SPEC_MARKER_TYPES = (typing.ParamSpecArgs, typing.ParamSpecKwargs) if HAS_PARAM_SPEC else ()
 
 
-def make_norm_type(  # noqa: CCR001
+def make_norm_type(
     origin: TypeHint,
     args: VarTuple[Hashable],
     *,
-    source: TypeHint
+    source: TypeHint,
 ) -> BaseNormType:
     if origin == Union:
         if not all(isinstance(arg, BaseNormType) for arg in args):
             raise TypeError
         return _UnionNormType(args, source=source)
     if origin == Literal:
         if not all(type(arg) in [int, bool, str, bytes] or isinstance(type(arg), EnumMeta) for arg in args):
@@ -464,15 +464,15 @@
 def _replace_source_with_union(norm: BaseNormType, sources: list) -> BaseNormType:
     return _replace_source(
         norm=norm,
         source=create_union(tuple(sources)),
     )
 
 
-NormAspect = Callable[['TypeNormalizer', Any, Any, tuple], Optional[BaseNormType]]
+NormAspect = Callable[["TypeNormalizer", Any, Any, tuple], Optional[BaseNormType]]
 
 
 class AspectStorage(List[str]):
     @overload
     def add(self, *, condition: object = True) -> Callable[[NormAspect], NormAspect]:
         ...
 
@@ -484,33 +484,32 @@
         if func is None:
             return partial(self.add, condition=condition)
 
         if condition:
             self.append(func.__name__)
         return func
 
-    def copy(self) -> 'AspectStorage':
+    def copy(self) -> "AspectStorage":
         return type(self)(super().copy())
 
 
 class NotSubscribedError(ValueError):
     pass
 
 
-N = TypeVar('N', bound=BaseNormType)
-TN = TypeVar('TN', bound='TypeNormalizer')
+N = TypeVar("N", bound=BaseNormType)
+TN = TypeVar("TN", bound="TypeNormalizer")
 
 
 class TypeNormalizer:
     def __init__(self, implicit_params_getter: ImplicitParamsGetter):
         self.implicit_params_getter = implicit_params_getter
         self._namespace: Optional[Dict[str, Any]] = None
 
     def _with_namespace(self: TN, namespace: Dict[str, Any]) -> TN:
-        # pylint: disable=protected-access
         self_copy = copy(self)
         self_copy._namespace = namespace
         return self_copy
 
     def _with_module_namespace(self: TN, module_name: str) -> TN:
         try:
             module = sys.modules[module_name]
@@ -524,15 +523,15 @@
 
     @overload
     def normalize(self, tp: TypeHint) -> BaseNormType:
         ...
 
     def normalize(self, tp: TypeHint) -> BaseNormType:
         origin = strip_alias(tp)
-        args = get_args(tp)
+        args = get_generic_args(tp)
 
         result = self._norm_forward_ref(tp)
         if result is not None:
             return result
 
         for attr_name in self._aspect_storage:
             result = getattr(self, attr_name)(tp, origin, args)
@@ -547,18 +546,18 @@
                 return _replace_source(
                     self.normalize(ForwardRef(tp)),
                     source=tp,
                 )
             if isinstance(tp, ForwardRef):
                 return _replace_source(
                     self.normalize(eval_forward_ref(self._namespace, tp)),
-                    source=tp
+                    source=tp,
                 )
         elif isinstance(tp, (str, ForwardRef)):
-            raise ValueError(f'Can not normalize value {tp!r}, there are no namespace to evaluate types')
+            raise ValueError(f"Can not normalize value {tp!r}, there are no namespace to evaluate types")
 
     _aspect_storage = AspectStorage()
 
     def _norm_iter(self, tps: Iterable[Any]) -> VarTuple[BaseNormType]:
         return tuple(self.normalize(tp) for tp in tps)
 
     MUST_SUBSCRIBED_ORIGINS = [
@@ -574,48 +573,47 @@
 
     @_aspect_storage.add
     def _check_bad_input(self, tp, origin, args):
         if tp in self.MUST_SUBSCRIBED_ORIGINS:
             raise NotSubscribedError(f"{tp} must be subscribed")
 
         if tp in (NewType, TypeVar):
-            raise ValueError(f'{origin} must be instantiating')
+            raise ValueError(f"{origin} must be instantiated")
 
     @_aspect_storage.add
     def _norm_none(self, tp, origin, args):
         if origin is None or origin is NoneType:
             return _NormType(None, (), source=tp)
 
     @_aspect_storage.add(condition=HAS_ANNOTATED)
     def _norm_annotated(self, tp, origin, args):
         if origin == typing.Annotated:
             return _AnnotatedNormType(
                 (self.normalize(args[0]), *args[1:]),
-                source=tp
+                source=tp,
             )
 
     def _get_bound(self, type_var) -> Bound:
         return (
             Bound(ANY_NT)
             if (type_var.__bound__ is None or type_var.__bound__ is NoneType) else
             Bound(self.normalize(type_var.__bound__))
         )
 
     @_aspect_storage.add
     def _norm_type_var(self, tp, origin, args):
-        # pylint: disable=protected-access
         if isinstance(origin, TypeVar):
             namespaced = self._with_module_namespace(origin.__module__)
             limit = (
                 Constraints(
                     tuple(
                         namespaced._dedup_union_args(
-                            namespaced._norm_iter(origin.__constraints__)
-                        )
-                    )
+                            namespaced._norm_iter(origin.__constraints__),
+                        ),
+                    ),
                 )
                 if origin.__constraints__ else
                 namespaced._get_bound(origin)
             )
             return NormTV(var=origin, limit=limit, source=tp)
 
     @_aspect_storage.add(condition=HAS_TV_TUPLE)
@@ -631,50 +629,50 @@
         if isinstance(tp, typing.ParamSpecKwargs):
             return _NormParamSpecKwargs(param_spec=self.normalize(origin), source=tp)
 
         if isinstance(origin, typing.ParamSpec):
             namespaced = self._with_module_namespace(origin.__module__)
             return NormTV(
                 var=origin,
-                limit=namespaced._get_bound(origin),  # pylint: disable=protected-access
+                limit=namespaced._get_bound(origin),
                 source=tp,
             )
 
     @_aspect_storage.add(condition=HAS_TV_SYNTAX)
     def _norm_type_alias_type(self, tp, origin, args):
-        if isinstance(origin, typing.TypeAliasType):  # pylint: disable=no-member
+        if isinstance(origin, typing.TypeAliasType):
             return NormTypeAlias(
                 origin,
                 self._norm_iter(args),
                 self._norm_iter(tp.__type_params__),
             )
 
     @_aspect_storage.add
     def _norm_init_var(self, tp, origin, args):
         if isinstance(origin, InitVar):
             # this origin is InitVar[T]
             return _NormType(
                 InitVar,
                 (self.normalize(origin.type),),
-                source=tp
+                source=tp,
             )
 
     @_aspect_storage.add
     def _norm_new_type(self, tp, origin, args):
         if is_new_type(tp):
             return _NormType(tp, (), source=tp)
 
     @_aspect_storage.add
     def _norm_tuple(self, tp, origin, args):
         if origin == tuple:
             if tp in (tuple, Tuple):  # not subscribed values
                 return _NormType(
                     tuple,
                     (ANY_NT, ...),
-                    source=tp
+                    source=tp,
                 )
 
             # >>> Tuple[()].__args__ == ((),)
             # >>> tuple[()].__args__ == ()
             if not args or args == ((),):
                 return _NormType(tuple, (), source=tp)
 
@@ -711,27 +709,27 @@
         return tp.origin == tuple and (not tp.args or tp.args[-1] is not Ellipsis)
 
     @_aspect_storage.add
     def _norm_callable(self, tp, origin, args):
         if origin == c_abc.Callable:
             if not args:
                 return _NormType(
-                    c_abc.Callable, (..., ANY_NT), source=tp
+                    c_abc.Callable, (..., ANY_NT), source=tp,
                 )
 
             if args[0] is Ellipsis:
                 call_args = ...
             elif isinstance(args[0], list):
                 call_args = self._norm_iter(args[0])
                 if HAS_TV_TUPLE:
                     call_args = self._unpack_generic_elements(call_args)
             else:
                 call_args = normalize_type(args[0])
             return _NormType(
-                c_abc.Callable, (call_args, self.normalize(args[-1])), source=tp
+                c_abc.Callable, (call_args, self.normalize(args[-1])), source=tp,
             )
 
     @_aspect_storage.add
     def _norm_literal(self, tp, origin, args):
         if origin == Literal:
             if args == (None,):  # Literal[None] converted to None
                 return _NormType(None, (), source=tp)
@@ -741,15 +739,15 @@
                 args_without_none.remove(None)
 
                 return _UnionNormType(
                     (
                         _NormType(None, (), source=Literal[None]),
                         _create_norm_literal(args_without_none),
                     ),
-                    source=tp
+                    source=tp,
                 )
 
             return _LiteralNormType(args, source=tp)
 
     def _unfold_union_args(self, norm_args: Iterable[N]) -> Iterable[N]:
         result: List[N] = []
         for norm in norm_args:
@@ -809,15 +807,15 @@
 
             if norm.origin == Union:
                 return _UnionNormType(
                     tuple(
                         _NormType(type, (arg,), source=Type[arg.source])
                         for arg in norm.args
                     ),
-                    source=tp
+                    source=tp,
                 )
 
     ALLOWED_ZERO_PARAMS_ORIGINS = {Any, NoReturn}
     if HAS_TYPE_ALIAS:
         ALLOWED_ZERO_PARAMS_ORIGINS.add(typing.TypeAlias)
     if HAS_PY_310:
         ALLOWED_ZERO_PARAMS_ORIGINS.add(dataclasses.KW_ONLY)
@@ -850,15 +848,15 @@
 
         params = self.implicit_params_getter.get_implicit_params(origin)
         if not (
             params
             or isinstance(origin, type)
             or origin in self.ALLOWED_ZERO_PARAMS_ORIGINS
         ):
-            raise ValueError(f'Can not normalize value {tp!r}')
+            raise ValueError(f"Can not normalize value {tp!r}")
 
         return _NormType(
             origin,
             tuple(self._norm_implicit_param(param) for param in params),
             source=tp,
         )
```

### Comparing `dishka-1.0.0/src/dishka/async_container.py` & `dishka-1.1.0/src/dishka/async_container.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,46 +122,46 @@
         try:
             return await compiled(self._get_unlocked, self._exits,
                                   self.context)
         except NoFactoryError as e:
             e.add_path(self.registry.get_factory(key))
             raise
 
-    async def close(self):
+    async def close(self, exception: Exception | None = None):
         errors = []
         for exit_generator in self._exits[::-1]:
             try:
                 if exit_generator.type is FactoryType.ASYNC_GENERATOR:
-                    await anext(exit_generator.callable)
+                    await exit_generator.callable.asend(exception)
                 elif exit_generator.type is FactoryType.GENERATOR:
-                    next(exit_generator.callable)
+                    exit_generator.callable.send(exception)
             except StopIteration:  # noqa: PERF203
                 pass
             except StopAsyncIteration:
                 pass
             except Exception as err:  # noqa: BLE001
                 errors.append(err)
         if self.close_parent:
             try:
-                await self.parent_container.close()
+                await self.parent_container.close(exception)
             except Exception as err:  # noqa: BLE001
                 errors.append(err)
         if errors:
             raise ExitError("Cleanup context errors", errors)
 
 
 class AsyncContextWrapper:
     def __init__(self, container: AsyncContainer):
         self.container = container
 
     async def __aenter__(self) -> AsyncContainer:
         return self.container
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
-        await self.container.close()
+        await self.container.close(exception=exc_val)
 
 
 def make_async_container(
         *providers: BaseProvider,
         scopes: type[BaseScope] = Scope,
         context: dict | None = None,
         lock_factory: Callable[[], Lock] | None = Lock,
```

### Comparing `dishka-1.0.0/src/dishka/container.py` & `dishka-1.1.0/src/dishka/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,27 +119,27 @@
             )
         try:
             return compiled(self._get_unlocked, self._exits, self.context)
         except NoFactoryError as e:
             e.add_path(self.registry.get_factory(key))
             raise
 
-    def close(self) -> None:
+    def close(self, exception: Exception | None = None) -> None:
         errors = []
         for exit_generator in self._exits[::-1]:
             try:
                 if exit_generator.type is FactoryType.GENERATOR:
-                    next(exit_generator.callable)
+                    exit_generator.callable.send(exception)
             except StopIteration:  # noqa: PERF203
                 pass
             except Exception as err:  # noqa: BLE001
                 errors.append(err)
         if self.close_parent:
             try:
-                self.parent_container.close()
+                self.parent_container.close(exception)
             except Exception as err:  # noqa: BLE001
                 errors.append(err)
 
         if errors:
             raise ExitError("Cleanup context errors", errors)
 
 
@@ -149,15 +149,15 @@
     def __init__(self, container: Container):
         self.container = container
 
     def __enter__(self) -> Container:
         return self.container
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self.container.close()
+        self.container.close(exception=exc_val)
 
 
 def make_container(
         *providers: BaseProvider,
         scopes: type[BaseScope] = Scope,
         context: dict | None = None,
         lock_factory: Callable[[], Lock] | None = None,
```

### Comparing `dishka-1.0.0/src/dishka/dependency_source/alias.py` & `dishka-1.1.0/src/dishka/dependency_source/alias.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/dependency_source/composite.py` & `dishka-1.1.0/src/dishka/dependency_source/composite.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/dependency_source/context_var.py` & `dishka-1.1.0/src/dishka/dependency_source/context_var.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/dependency_source/decorator.py` & `dishka-1.1.0/src/dishka/dependency_source/decorator.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/dependency_source/factory.py` & `dishka-1.1.0/src/dishka/dependency_source/factory.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/dependency_source/make_alias.py` & `dishka-1.1.0/src/dishka/dependency_source/make_alias.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/dependency_source/make_context_var.py` & `dishka-1.1.0/src/dishka/dependency_source/make_context_var.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/dependency_source/make_decorator.py` & `dishka-1.1.0/src/dishka/dependency_source/make_decorator.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/dependency_source/make_factory.py` & `dishka-1.1.0/src/dishka/dependency_source/make_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,33 +15,39 @@
     isfunction,
     isgeneratorfunction,
     ismethod,
     signature,
     unwrap,
 )
 from typing import (
+    Annotated,
     Any,
     Protocol,
     get_args,
     get_origin,
     get_type_hints,
     overload,
 )
 
 from dishka._adaptix.type_tools.basic_utils import (
-    get_all_type_hints,
     get_type_vars,
     is_bare_generic,
     strip_alias,
 )
+from dishka._adaptix.type_tools.fundamentals import (
+    get_all_type_hints,
+)
 from dishka._adaptix.type_tools.generic_resolver import (
     GenericResolver,
     MembersStorage,
 )
-from dishka.entities.key import DependencyKey, hints_to_dependency_keys
+from dishka.entities.key import (
+    hint_to_dependency_key,
+    hints_to_dependency_keys,
+)
 from dishka.entities.scope import BaseScope
 from .composite import CompositeDependencySource, ensure_composite
 from .factory import Factory, FactoryType
 from .unpack_provides import unpack_factory
 
 _empty = signature(lambda a: 0).parameters["a"].annotation
 _protocol_init = type("_stub_proto", (Protocol,), {}).__init__
@@ -173,14 +179,19 @@
 def _make_factory_by_class(
         *,
         provides: Any,
         scope: BaseScope | None,
         source: Callable,
         cache: bool,
 ) -> Factory:
+    if not provides:
+        provides = source
+
+    if get_origin(source) is Annotated:
+        source = get_args(source)[0]
     init = strip_alias(source).__init__
     if missing_hints := _params_without_hints(init, skip_self=True):
         name = f"{source.__module__}.{source.__qualname__}.__init__"
         missing = ", ".join(missing_hints)
         raise ValueError(
             f"Failed to analyze `{name}`. \n"
             f"Some parameters do not have type hints: {missing}\n",
@@ -196,25 +207,24 @@
             f"Failed to analyze `{name}`. \n"
             f"Type '{e.name}' is not defined\n\n"
             f"If your are using `if TYPE_CHECKING` to import '{e.name}' "
             f"then try removing it. \n"
             f"Or, create a separate factory with all types imported.",
             name=e.name,
         ) from e
+
     hints.pop("return", _empty)
     dependencies = list(hints.values())
-    if not provides:
-        provides = source
 
     return Factory(
         dependencies=hints_to_dependency_keys(dependencies),
         type_=FactoryType.FACTORY,
         source=source,
         scope=scope,
-        provides=DependencyKey(provides, None),
+        provides=hint_to_dependency_key(provides),
         is_to_bind=False,
         cache=cache,
     )
 
 
 def _make_factory_by_method(
         *,
@@ -268,15 +278,15 @@
             name = getattr(source, "__qualname__", "") or str(source)
             raise TypeError(f"Failed to analyze `{name}`. \n" + str(e)) from e
     return Factory(
         dependencies=hints_to_dependency_keys(dependencies),
         type_=factory_type,
         source=source,
         scope=scope,
-        provides=DependencyKey(provides, None),
+        provides=hint_to_dependency_key(provides),
         is_to_bind=is_in_class,
         cache=cache,
     )
 
 
 def _make_factory_by_static_method(
         *,
@@ -318,15 +328,15 @@
             name = getattr(source, "__qualname__", "") or str(source)
             raise TypeError(f"Failed to analyze `{name}`. \n" + str(e)) from e
     return Factory(
         dependencies=hints_to_dependency_keys(dependencies),
         type_=factory_type,
         source=source,
         scope=scope,
-        provides=DependencyKey(provides, None),
+        provides=hint_to_dependency_key(provides),
         is_to_bind=False,
         cache=cache,
     )
 
 
 def _make_factory_by_other_callable(
         *,
@@ -483,9 +493,45 @@
             provides=provides, scope=scope, source=func, cache=cache,
             is_in_class=True,
         )
 
     return scoped
 
 
-def _context_stub():
-    raise NotImplementedError
+def _provide_all(
+        *,
+        provides: Sequence[Any],
+        scope: BaseScope | None,
+        cache: bool,
+        is_in_class: bool,
+) -> CompositeDependencySource:
+    composite = CompositeDependencySource(None)
+    for single_provides in provides:
+        factory = make_factory(
+            provides=single_provides, scope=scope,
+            source=single_provides, cache=cache,
+            is_in_class=is_in_class,
+        )
+        composite.dependency_sources.extend(unpack_factory(factory))
+    return composite
+
+
+def provide_all(
+        *provides: Any,
+        scope: BaseScope | None = None,
+        cache: bool = True,
+) -> CompositeDependencySource:
+    return _provide_all(
+        provides=provides, scope=scope,
+        cache=cache, is_in_class=True,
+    )
+
+
+def provide_all_on_instance(
+        *provides: Any,
+        scope: BaseScope | None = None,
+        cache: bool = True,
+) -> CompositeDependencySource:
+    return _provide_all(
+        provides=provides, scope=scope,
+        cache=cache, is_in_class=False,
+    )
```

### Comparing `dishka-1.0.0/src/dishka/dependency_source/unpack_provides.py` & `dishka-1.1.0/src/dishka/dependency_source/unpack_provides.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/entities/depends_marker.py` & `dishka-1.1.0/src/dishka/entities/depends_marker.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/entities/key.py` & `dishka-1.1.0/src/dishka/entities/key.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/entities/scope.py` & `dishka-1.1.0/src/dishka/entities/scope.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/error_rendering.py` & `dishka-1.1.0/src/dishka/error_rendering.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/exceptions.py` & `dishka-1.1.0/src/dishka/exceptions.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/factory_compiler.py` & `dishka-1.1.0/src/dishka/factory_compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 CACHE = "context[provides] = solved"
 
 
 def compile_factory(*, factory: Factory, is_async: bool) -> CompiledFactory:
     names = {f"arg{i}": dep for i, dep in enumerate(factory.dependencies)}
     if is_async:
         async_ = "async "
-        await_ = "await"
+        await_ = "await "
         body_template = ASYNC_BODIES.get(factory.type, INVALID)
     else:
         async_ = ""
         await_ = ""
         body_template = SYNC_BODIES.get(factory.type, INVALID)
     if factory.cache:
         cache = CACHE
```

### Comparing `dishka-1.0.0/src/dishka/integrations/aiogram.py` & `dishka-1.1.0/src/dishka/integrations/aiogram.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/integrations/aiohttp.py` & `dishka-1.1.0/src/dishka/integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/integrations/arq.py` & `dishka-1.1.0/src/dishka/integrations/arq.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/integrations/base.py` & `dishka-1.1.0/src/dishka/integrations/base.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/integrations/fastapi.py` & `dishka-1.1.0/src/dishka/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/integrations/faststream.py` & `dishka-1.1.0/src/dishka/integrations/sanic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,56 @@
-__all__ = (
+__all__ = [
     "FromDishka",
     "inject",
     "setup_dishka",
-)
+]
 
-from collections.abc import AsyncIterator, Awaitable, Callable
-from contextlib import asynccontextmanager
-from typing import Any, TypeVar
+from collections.abc import Awaitable, Callable, Iterable
 
-from faststream import BaseMiddleware, FastStream, context
-from faststream.types import DecodedMessage
+from sanic import HTTPResponse, Request, Sanic
+from sanic_routing import Route
 
 from dishka import AsyncContainer, FromDishka
-from dishka.integrations.base import wrap_injection
+from dishka.integrations.base import is_dishka_injected, wrap_injection
 
-T = TypeVar("T")
 
-
-def inject(func: Callable[..., Awaitable[T]]) -> Callable[..., Awaitable[T]]:
+def inject(func: Callable) -> Awaitable:
     return wrap_injection(
         func=func,
-        container_getter=lambda *_: context.get_local("dishka"),
-        is_async=True,
         remove_depends=True,
+        container_getter=lambda args, _: args[0].ctx.dishka_container,
+        is_async=True,
     )
 
 
-class DishkaMiddleware(BaseMiddleware):
+class ContainerMiddleware:
     def __init__(self, container: AsyncContainer) -> None:
         self.container = container
 
-    def __call__(self, msg: Any | None = None) -> "DishkaMiddleware":
-        self.msg = msg
-        return self
-
-    @asynccontextmanager
-    async def consume_scope(
-            self,
-            *args: Any,
-            **kwargs: Any,
-    ) -> AsyncIterator[DecodedMessage]:
-        async with self.container() as request_container:
-            with context.scope("dishka", request_container):
-                async with super().consume_scope(*args, **kwargs) as result:
-                    yield result
+    async def on_request(self, request: Request) -> None:
+        request.ctx.container_wrapper = self.container({Request: request})
+        request.ctx.dishka_container = await request.ctx.container_wrapper.__aenter__()  # noqa: E501
+
+    async def on_response(self, request: Request, _: HTTPResponse) -> None:
+        await request.ctx.dishka_container.close()
 
 
-def setup_dishka(
-        container: AsyncContainer,
-        app: FastStream,
-        *,
-        finalize_container: bool = True,
-) -> None:
-    assert app.broker, "You can't patch FastStream application without broker"  # noqa: S101
+def _inject_routes(routes: Iterable[Route]) -> None:
+    for route in routes:
+        if not is_dishka_injected(route.handler):
+            route.handler = inject(route.handler)
 
-    if finalize_container:
-        app.after_shutdown(container.close)
 
-    app.broker.middlewares = (
-        *app.broker.middlewares,
-        DishkaMiddleware(container),
-    )
+def setup_dishka(
+    container: AsyncContainer,
+    app: Sanic,
+    *,
+    auto_inject: bool = False,
+) -> None:
+    middleware = ContainerMiddleware(container)
+    app.on_request(middleware.on_request)
+    app.on_response(middleware.on_response)
+
+    if auto_inject:
+        _inject_routes(app.router.routes)
+        for blueprint in app.blueprints.values():
+            _inject_routes(blueprint.routes)
```

### Comparing `dishka-1.0.0/src/dishka/integrations/flask.py` & `dishka-1.1.0/src/dishka/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/integrations/litestar.py` & `dishka-1.1.0/src/dishka/integrations/litestar.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/integrations/starlette.py` & `dishka-1.1.0/src/dishka/integrations/starlette.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/integrations/taskiq.py` & `dishka-1.1.0/src/dishka/integrations/taskiq.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/integrations/telebot.py` & `dishka-1.1.0/src/dishka/integrations/telebot.py`

 * *Files identical despite different names*

### Comparing `dishka-1.0.0/src/dishka/provider.py` & `dishka-1.1.0/src/dishka/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,18 @@
     DependencySource,
     Factory,
     alias,
     from_context,
 )
 from .dependency_source.composite import CompositeDependencySource
 from .dependency_source.make_decorator import decorate_on_instance
-from .dependency_source.make_factory import provide_on_instance
+from .dependency_source.make_factory import (
+    provide_all_on_instance,
+    provide_on_instance,
+)
 
 
 def is_dependency_source(attribute: Any) -> bool:
     return isinstance(attribute, CompositeDependencySource)
 
 
 class BaseProvider:
@@ -137,14 +140,28 @@
             scope=scope,
             provides=provides,
             cache=cache,
         )
         self._add_dependency_sources(str(source), composite.dependency_sources)
         return composite
 
+    def provide_all(
+            self,
+            *provides: Any,
+            scope: BaseScope | None = None,
+            cache: bool = True,
+    ) -> CompositeDependencySource:
+        if scope is None:
+            scope = self.scope
+        composite = provide_all_on_instance(
+            *provides, scope=scope, cache=cache,
+        )
+        self._add_dependency_sources("?", composite.dependency_sources)
+        return composite
+
     def alias(
             self,
             *,
             source: type,
             provides: Any,
             cache: bool = True,
     ) -> CompositeDependencySource:
@@ -170,15 +187,15 @@
         return composite
 
     def to_component(self, component: Component) -> "ProviderWrapper":
         return ProviderWrapper(component, self)
 
     def from_context(
             self, *, provides: Any, scope: BaseScope,
-    ) -> ContextVariable:
+    ) -> CompositeDependencySource:
         composite = from_context(provides=provides, scope=scope)
         self._add_dependency_sources(str(provides),
                                      composite.dependency_sources)
         return composite
 
 
 class ProviderWrapper(BaseProvider):
```

### Comparing `dishka-1.0.0/src/dishka/registry.py` & `dishka-1.1.0/src/dishka/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 from ._adaptix.type_tools.basic_utils import get_type_vars, is_generic
 from .container_objects import CompiledFactory
 from .dependency_source import (
     Alias,
     ContextVariable,
     Decorator,
     Factory,
+    FactoryType,
 )
 from .entities.component import DEFAULT_COMPONENT, Component
 from .entities.key import DependencyKey
 from .entities.scope import BaseScope, InvalidScopes
 from .exceptions import (
     CycleDependenciesError,
     GraphMissingFactoryError,
+    InvalidGraphError,
     NoFactoryError,
     UnknownScopeError,
 )
 from .factory_compiler import compile_factory
 from .provider import BaseProvider
 
 
@@ -290,14 +292,18 @@
         registry = self.registries[scope]
         undecorated_type = NewType(
             f"{provides.type_hint.__name__}@{self.decorator_depth[provides]}",
             decorator.provides.type_hint,
         )
         self.decorator_depth[provides] += 1
         old_factory = registry.get_factory(provides)
+        if old_factory.type is FactoryType.CONTEXT:
+            raise InvalidGraphError(
+                f"Cannot apply decorator to context data {provides}",
+            )
         old_factory.provides = DependencyKey(
             undecorated_type, old_factory.provides.component,
         )
         new_factory = decorator.as_factory(
             scope=scope,
             new_dependency=DependencyKey(undecorated_type, None),
             cache=old_factory.cache,
```

### Comparing `dishka-1.0.0/src/dishka.egg-info/PKG-INFO` & `dishka-1.1.0/src/dishka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dishka
-Version: 1.0.0
+Version: 1.1.0
 Summary: Minimal DI framework
 Author-email: Andrey Tikhonov <17@itishka.org>
 License: Apache-2.0
 Project-URL: Source, https://github.com/reagento/dishka
 Project-URL: Homepage, https://github.com/reagento/dishka
 Project-URL: Documentation, https://dishka.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/reagento/dishka/issues
@@ -55,15 +55,15 @@
 
 1. Install dishka
 
 ```shell
 pip install dishka
 ```
 
-2. Create `Provider` instance. It is only used co setup all factories providing your objects.
+2. Create `Provider` instance. It is only used to setup all factories providing your objects.
 
 ```python
 from dishka import Provider
 
 provider = Provider()
 ```
 
@@ -263,15 +263,15 @@
 class MyProvider(Provider):
     scope = Scope.REQUEST
 
     app = from_context(provides=App, scope=Scope.APP)
     request = from_context(provides=RequestClass)
 
     @provide
-    async def get_a(self, request: RequestClass, app: App) -> A:
+    def get_a(self, request: RequestClass, app: App) -> A:
         ...
 
 container = make_container(MyProvider(), context={App: app})
 with container(context={RequestClass: request_instance}) as request_container:
     pass
 ```
 
@@ -281,13 +281,13 @@
 container = make_container(MyProvider(), OtherProvider())
 ```
 
 * Tired of providing `scope==` for each depedency? Set it inside your `Provider` class and all dependencies with no scope will use it.
 
 ```python
 class MyProvider(Provider):
-   scope=Scope.APP
+   scope = Scope.APP
 
    @provide
    async def get_a(self) -> A:
       return A()
 ```
```

### Comparing `dishka-1.0.0/src/dishka.egg-info/SOURCES.txt` & `dishka-1.1.0/src/dishka.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 src/dishka.egg-info/requires.txt
 src/dishka.egg-info/top_level.txt
 src/dishka/_adaptix/common.py
 src/dishka/_adaptix/feature_requirement.py
 src/dishka/_adaptix/type_tools/__init__.py
 src/dishka/_adaptix/type_tools/basic_utils.py
 src/dishka/_adaptix/type_tools/constants.py
+src/dishka/_adaptix/type_tools/fundamentals.py
 src/dishka/_adaptix/type_tools/generic_resolver.py
 src/dishka/_adaptix/type_tools/implicit_params.py
 src/dishka/_adaptix/type_tools/norm_utils.py
 src/dishka/_adaptix/type_tools/normalize_type.py
 src/dishka/dependency_source/__init__.py
 src/dishka/dependency_source/alias.py
 src/dishka/dependency_source/composite.py
@@ -47,10 +48,11 @@
 src/dishka/integrations/aiohttp.py
 src/dishka/integrations/arq.py
 src/dishka/integrations/base.py
 src/dishka/integrations/fastapi.py
 src/dishka/integrations/faststream.py
 src/dishka/integrations/flask.py
 src/dishka/integrations/litestar.py
+src/dishka/integrations/sanic.py
 src/dishka/integrations/starlette.py
 src/dishka/integrations/taskiq.py
 src/dishka/integrations/telebot.py
```


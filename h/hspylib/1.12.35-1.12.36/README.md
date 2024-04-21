# Comparing `tmp/hspylib-1.12.35.tar.gz` & `tmp/hspylib-1.12.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-1.12.35.tar", last modified: Wed Mar 20 19:07:47 2024, max compression
+gzip compressed data, was "hspylib-1.12.36.tar", last modified: Sun Apr 21 04:42:13 2024, max compression
```

## Comparing `hspylib-1.12.35.tar` & `hspylib-1.12.36.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:47.082292 hspylib-1.12.35/
--rw-r--r--   0 hjunior    (501) staff       (20)       25 2024-02-16 22:31:12.000000 hspylib-1.12.35/MANIFEST.in
--rw-r--r--   0 hjunior    (501) staff       (20)    13199 2024-03-20 19:07:47.077250 hspylib-1.12.35/PKG-INFO
--rw-r--r--   0 hjunior    (501) staff       (20)    11869 2024-03-20 19:07:37.000000 hspylib-1.12.35/README.md
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:46.885760 hspylib-1.12.35/hspylib/
--rw-r--r--   0 hjunior    (501) staff       (20)        7 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/.version
--rw-r--r--   0 hjunior    (501) staff       (20)      886 2024-03-19 20:46:13.000000 hspylib-1.12.35/hspylib/__classpath__.py
--rw-r--r--   0 hjunior    (501) staff       (20)      167 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/__init__.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:46.917779 hspylib-1.12.35/hspylib/core/
--rw-r--r--   0 hjunior    (501) staff       (20)      347 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/core/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     6057 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/collection_filter.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:46.927714 hspylib-1.12.35/hspylib/core/config/
--rw-r--r--   0 hjunior    (501) staff       (20)      211 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/core/config/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     3418 2024-03-20 18:58:09.000000 hspylib-1.12.35/hspylib/core/config/app_config.py
--rw-r--r--   0 hjunior    (501) staff       (20)     3133 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/config/parser_factory.py
--rw-r--r--   0 hjunior    (501) staff       (20)     4727 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/config/properties.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1818 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/constants.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:46.933427 hspylib-1.12.35/hspylib/core/decorator/
--rw-r--r--   0 hjunior    (501) staff       (20)      172 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/core/decorator/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2015 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/decorator/decorators.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:46.947738 hspylib-1.12.35/hspylib/core/enums/
--rw-r--r--   0 hjunior    (501) staff       (20)      244 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/core/enums/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     3429 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/enums/charset.py
--rw-r--r--   0 hjunior    (501) staff       (20)     4335 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/enums/content_type.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2926 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/enums/enumeration.py
--rw-r--r--   0 hjunior    (501) staff       (20)     6356 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/enums/http_code.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1745 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/enums/http_method.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:46.952351 hspylib-1.12.35/hspylib/core/exception/
--rw-r--r--   0 hjunior    (501) staff       (20)      172 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/core/exception/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2256 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/exception/exceptions.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:46.960195 hspylib-1.12.35/hspylib/core/metaclass/
--rw-r--r--   0 hjunior    (501) staff       (20)      189 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/core/metaclass/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     6277 2024-03-19 21:14:05.000000 hspylib-1.12.35/hspylib/core/metaclass/classpath.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2848 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/metaclass/singleton.py
--rw-r--r--   0 hjunior    (501) staff       (20)     5082 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/namespace.py
--rw-r--r--   0 hjunior    (501) staff       (20)     3611 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/preconditions.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:46.973896 hspylib-1.12.35/hspylib/core/tools/
--rw-r--r--   0 hjunior    (501) staff       (20)      239 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/core/tools/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     8802 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/tools/commons.py
--rw-r--r--   0 hjunior    (501) staff       (20)     3403 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/tools/dict_tools.py
--rwxr-xr-x   0 hjunior    (501) staff       (20)     7171 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/tools/json_path.py
--rw-r--r--   0 hjunior    (501) staff       (20)     8100 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/tools/text_tools.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2243 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/tools/validator.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1617 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/core/zoned_datetime.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:46.980206 hspylib-1.12.35/hspylib/modules/
--rw-r--r--   0 hjunior    (501) staff       (20)      240 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/modules/__init__.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:46.994756 hspylib-1.12.35/hspylib/modules/application/
--rw-r--r--   0 hjunior    (501) staff       (20)      250 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/modules/application/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     7687 2024-03-20 18:59:32.000000 hspylib-1.12.35/hspylib/modules/application/application.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:47.014014 hspylib-1.12.35/hspylib/modules/application/argparse/
--rw-r--r--   0 hjunior    (501) staff       (20)      297 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/modules/application/argparse/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1073 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/modules/application/argparse/argument_parser.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1343 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/modules/application/argparse/arguments_builder.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2780 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/modules/application/argparse/chained_arguments_builder.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1619 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/modules/application/argparse/options_builder.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1532 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/modules/application/argparse/parser_action.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1935 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/modules/application/exit_hooks.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2177 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/modules/application/exit_status.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2990 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/modules/application/version.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:47.019884 hspylib-1.12.35/hspylib/modules/cache/
--rw-r--r--   0 hjunior    (501) staff       (20)      193 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/modules/cache/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2585 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/modules/cache/ttl_cache.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2801 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/modules/cache/ttl_keyring_be.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:47.023794 hspylib-1.12.35/hspylib/modules/cli/
--rw-r--r--   0 hjunior    (501) staff       (20)      181 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/modules/cli/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     7292 2024-03-20 18:18:21.000000 hspylib-1.12.35/hspylib/modules/cli/keyboard.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:47.039748 hspylib-1.12.35/hspylib/modules/cli/vt100/
--rw-r--r--   0 hjunior    (501) staff       (20)      204 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/modules/cli/vt100/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     5709 2024-03-20 16:59:02.000000 hspylib-1.12.35/hspylib/modules/cli/vt100/vt_100.py
--rw-r--r--   0 hjunior    (501) staff       (20)     5115 2024-03-20 16:57:06.000000 hspylib-1.12.35/hspylib/modules/cli/vt100/vt_code.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2582 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/modules/cli/vt100/vt_color.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:47.047300 hspylib-1.12.35/hspylib/modules/eventbus/
--rw-r--r--   0 hjunior    (501) staff       (20)      186 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/modules/eventbus/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1242 2024-02-22 19:10:39.000000 hspylib-1.12.35/hspylib/modules/eventbus/event.py
--rw-r--r--   0 hjunior    (501) staff       (20)     3722 2024-03-20 16:09:09.000000 hspylib-1.12.35/hspylib/modules/eventbus/eventbus.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:47.061777 hspylib-1.12.35/hspylib/modules/fetch/
--rw-r--r--   0 hjunior    (501) staff       (20)      227 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/modules/fetch/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     4779 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/modules/fetch/fetch.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1888 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/modules/fetch/http_response.py
--rw-r--r--   0 hjunior    (501) staff       (20)     5412 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/modules/fetch/uri_builder.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1082 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/modules/fetch/uri_scheme.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:47.067633 hspylib-1.12.35/hspylib/modules/security/
--rw-r--r--   0 hjunior    (501) staff       (20)      172 2024-03-20 19:07:37.000000 hspylib-1.12.35/hspylib/modules/security/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     6481 2024-02-16 22:31:12.000000 hspylib-1.12.35/hspylib/modules/security/security.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-03-20 19:07:47.073600 hspylib-1.12.35/hspylib.egg-info/
--rw-r--r--   0 hjunior    (501) staff       (20)    13199 2024-03-20 19:07:46.000000 hspylib-1.12.35/hspylib.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (501) staff       (20)     2449 2024-03-20 19:07:46.000000 hspylib-1.12.35/hspylib.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (501) staff       (20)        1 2024-03-20 19:07:46.000000 hspylib-1.12.35/hspylib.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (501) staff       (20)      114 2024-03-20 19:07:46.000000 hspylib-1.12.35/hspylib.egg-info/requires.txt
--rw-r--r--   0 hjunior    (501) staff       (20)       13 2024-03-20 19:07:46.000000 hspylib-1.12.35/hspylib.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (501) staff       (20)       38 2024-03-20 19:07:47.082617 hspylib-1.12.35/setup.cfg
--rw-r--r--   0 hjunior    (501) staff       (20)     2003 2024-02-16 22:31:12.000000 hspylib-1.12.35/setup.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.425635 hspylib-1.12.36/
+-rw-r--r--   0 hugo       (503) staff       (20)       25 2023-09-24 15:24:10.000000 hspylib-1.12.36/MANIFEST.in
+-rw-r--r--   0 hugo       (503) staff       (20)    13229 2024-04-21 04:42:13.424615 hspylib-1.12.36/PKG-INFO
+-rw-r--r--   0 hugo       (503) staff       (20)    11869 2024-04-21 04:42:08.000000 hspylib-1.12.36/README.md
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.388815 hspylib-1.12.36/hspylib/
+-rw-r--r--   0 hugo       (503) staff       (20)        7 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/.version
+-rw-r--r--   0 hugo       (503) staff       (20)      886 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/__classpath__.py
+-rw-r--r--   0 hugo       (503) staff       (20)      167 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/__init__.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.394554 hspylib-1.12.36/hspylib/core/
+-rw-r--r--   0 hugo       (503) staff       (20)      347 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/core/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     6055 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/core/collection_filter.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.396628 hspylib-1.12.36/hspylib/core/config/
+-rw-r--r--   0 hugo       (503) staff       (20)      211 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/core/config/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3380 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/core/config/app_config.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3131 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/core/config/parser_factory.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4727 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/config/properties.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1819 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/core/constants.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.397497 hspylib-1.12.36/hspylib/core/decorator/
+-rw-r--r--   0 hugo       (503) staff       (20)      172 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/core/decorator/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2015 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/decorator/decorators.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.401100 hspylib-1.12.36/hspylib/core/enums/
+-rw-r--r--   0 hugo       (503) staff       (20)      244 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/core/enums/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3429 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/enums/charset.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4335 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/enums/content_type.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2926 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/enums/enumeration.py
+-rw-r--r--   0 hugo       (503) staff       (20)     6356 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/enums/http_code.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1745 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/enums/http_method.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.402334 hspylib-1.12.36/hspylib/core/exception/
+-rw-r--r--   0 hugo       (503) staff       (20)      172 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/core/exception/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2256 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/exception/exceptions.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.403866 hspylib-1.12.36/hspylib/core/metaclass/
+-rw-r--r--   0 hugo       (503) staff       (20)      189 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/core/metaclass/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     6243 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/core/metaclass/classpath.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2847 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/core/metaclass/singleton.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5082 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/namespace.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3611 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/preconditions.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.406658 hspylib-1.12.36/hspylib/core/tools/
+-rw-r--r--   0 hugo       (503) staff       (20)      239 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/core/tools/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     8802 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/tools/commons.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3403 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/tools/dict_tools.py
+-rwxr-xr-x   0 hugo       (503) staff       (20)     7170 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/core/tools/json_path.py
+-rw-r--r--   0 hugo       (503) staff       (20)     8084 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/core/tools/text_tools.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2243 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/tools/validator.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1617 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/zoned_datetime.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.407124 hspylib-1.12.36/hspylib/modules/
+-rw-r--r--   0 hugo       (503) staff       (20)      240 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/__init__.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.409737 hspylib-1.12.36/hspylib/modules/application/
+-rw-r--r--   0 hugo       (503) staff       (20)      250 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/application/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     7687 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/modules/application/application.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.412863 hspylib-1.12.36/hspylib/modules/application/argparse/
+-rw-r--r--   0 hugo       (503) staff       (20)      297 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/application/argparse/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1073 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/application/argparse/argument_parser.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1343 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/application/argparse/arguments_builder.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2780 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/application/argparse/chained_arguments_builder.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1619 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/application/argparse/options_builder.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1532 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/application/argparse/parser_action.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1935 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/application/exit_hooks.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2177 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/application/exit_status.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2990 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/application/version.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.414074 hspylib-1.12.36/hspylib/modules/cache/
+-rw-r--r--   0 hugo       (503) staff       (20)      193 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/cache/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2585 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/cache/ttl_cache.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2801 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/cache/ttl_keyring_be.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.415285 hspylib-1.12.36/hspylib/modules/cli/
+-rw-r--r--   0 hugo       (503) staff       (20)      181 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/cli/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     7286 2024-04-21 04:40:06.000000 hspylib-1.12.36/hspylib/modules/cli/keyboard.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.417037 hspylib-1.12.36/hspylib/modules/cli/vt100/
+-rw-r--r--   0 hugo       (503) staff       (20)      204 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/cli/vt100/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5709 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/modules/cli/vt100/vt_100.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5115 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/modules/cli/vt100/vt_code.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2582 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/cli/vt100/vt_color.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.419018 hspylib-1.12.36/hspylib/modules/eventbus/
+-rw-r--r--   0 hugo       (503) staff       (20)      186 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/eventbus/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1242 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/eventbus/event.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3721 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/modules/eventbus/eventbus.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.421996 hspylib-1.12.36/hspylib/modules/fetch/
+-rw-r--r--   0 hugo       (503) staff       (20)      227 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/fetch/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4779 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/fetch/fetch.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1888 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/fetch/http_response.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5412 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/fetch/uri_builder.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1082 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/fetch/uri_scheme.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.422825 hspylib-1.12.36/hspylib/modules/security/
+-rw-r--r--   0 hugo       (503) staff       (20)      172 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/security/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     6481 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/security/security.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.423620 hspylib-1.12.36/hspylib.egg-info/
+-rw-r--r--   0 hugo       (503) staff       (20)    13229 2024-04-21 04:42:13.000000 hspylib-1.12.36/hspylib.egg-info/PKG-INFO
+-rw-r--r--   0 hugo       (503) staff       (20)     2449 2024-04-21 04:42:13.000000 hspylib-1.12.36/hspylib.egg-info/SOURCES.txt
+-rw-r--r--   0 hugo       (503) staff       (20)        1 2024-04-21 04:42:13.000000 hspylib-1.12.36/hspylib.egg-info/dependency_links.txt
+-rw-r--r--   0 hugo       (503) staff       (20)      129 2024-04-21 04:42:13.000000 hspylib-1.12.36/hspylib.egg-info/requires.txt
+-rw-r--r--   0 hugo       (503) staff       (20)       13 2024-04-21 04:42:13.000000 hspylib-1.12.36/hspylib.egg-info/top_level.txt
+-rw-r--r--   0 hugo       (503) staff       (20)       38 2024-04-21 04:42:13.425770 hspylib-1.12.36/setup.cfg
+-rw-r--r--   0 hugo       (503) staff       (20)     2003 2024-01-06 13:35:49.000000 hspylib-1.12.36/setup.py
```

### Comparing `hspylib-1.12.35/PKG-INFO` & `hspylib-1.12.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib
-Version: 1.12.35
+Version: 1.12.36
 Summary: HsPyLib - Core python library
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib/
@@ -24,22 +24,23 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: retry
 Requires-Dist: urllib3
 Requires-Dist: cryptocode
 Requires-Dist: cryptography
 Requires-Dist: emoji
-Requires-Dist: getkey
+Requires-Dist: get-key
 Requires-Dist: keyring
 Requires-Dist: pyparsing
 Requires-Dist: pyperclip
 Requires-Dist: PyYAML
 Requires-Dist: toml
 Requires-Dist: requests
 Requires-Dist: urllib3<2.0.0
+Requires-Dist: pyparsing<3.1
 
 <img src="https://iili.io/HYBJFA7.png" width="64" height="64" align="right" />
 
 # HomeSetup Python Library
 >
 > Because your Python code is not JUST a script !
```

### Comparing `hspylib-1.12.35/README.md` & `hspylib-1.12.36/README.md`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/__classpath__.py` & `hspylib-1.12.36/hspylib/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/core/collection_filter.py` & `hspylib-1.12.36/hspylib/core/collection_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,23 +8,22 @@
    @created: Wed, 8 Jun 2022
     @author: "<B>H</B>ugo <B>S</B>aporetti <B>J</B>unior")"
       @site: "https://github.com/yorevs/hspylib")
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
-from typing import get_args, Iterable, Iterator, Set, Tuple, TypeVar, Union, TypeAlias
-
 from hspylib.core.enums.enumeration import Enumeration
 from hspylib.core.preconditions import check_argument
 from hspylib.core.tools.text_tools import quote
+from typing import get_args, Iterable, Iterator, Set, Tuple, TypeAlias, TypeVar, Union
 
 T = TypeVar("T")
 
-FilterValue : TypeAlias = Union[int, str, bool, float]
+FilterValue: TypeAlias = Union[int, str, bool, float]
 
 
 class FilterCondition(Enumeration):
     """Collection filter conditions."""
 
     # fmt: off
     LESS_THAN                   =      '<', Union[int, float]
```

### Comparing `hspylib-1.12.35/hspylib/core/config/app_config.py` & `hspylib-1.12.36/hspylib/core/config/app_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,20 +36,15 @@
       |-Run-dir = {}
       |-Resources-dir = {}
       |-Properties:
        \\-{}
     """
     )
 
-    def __init__(
-        self,
-        resource_dir: AnyPath,
-        filename: str | None = None,
-        profile: str | None = None
-    ):
+    def __init__(self, resource_dir: AnyPath, filename: str | None = None, profile: str | None = None):
         check_argument(os.path.exists(str(resource_dir)), "Unable to locate resources dir: {}", resource_dir)
         self._resource_dir = str(resource_dir)
         self._properties = Properties(filename=filename, load_dir=resource_dir, profile=profile)
         log.info(self)
 
     # pylint: disable=consider-using-f-string
     def __str__(self) -> str:
```

### Comparing `hspylib-1.12.35/hspylib/core/config/parser_factory.py` & `hspylib-1.12.36/hspylib/core/config/parser_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,27 +8,26 @@
    @created: Wed, 19 May 2023
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
-import os
-import re
 from abc import ABC
 from configparser import ConfigParser
 from functools import partial
+from hspylib.core.tools.dict_tools import flatten_dict
 from typing import Any, Callable, Dict, TextIO, TypeAlias
 
+import os
+import re
 import toml
 import yaml
 
-from hspylib.core.tools.dict_tools import flatten_dict
-
-Properties : TypeAlias = Dict[str, Any]
+Properties: TypeAlias = Dict[str, Any]
 
 
 class ParserFactory(ABC):
     """Provide a properties parser factory."""
 
     class PropertyParser:
         """Represent a property parser."""
```

### Comparing `hspylib-1.12.35/hspylib/core/config/properties.py` & `hspylib-1.12.36/hspylib/core/config/properties.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/core/constants.py` & `hspylib-1.12.36/hspylib/core/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,7 +61,8 @@
     r"(?:" + RE_IPV4 + "|" + RE_IPV6 + "|" + RE_HOST + ")"
     r"(?::[0-9]{1,5})?"  # port
     r"(?:[/?#][^\s]*)?"  # resource path
     r"\Z"
 )
 
 # fmt: on
+
```

### Comparing `hspylib-1.12.35/hspylib/core/decorator/decorators.py` & `hspylib-1.12.36/hspylib/core/decorator/decorators.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/core/enums/charset.py` & `hspylib-1.12.36/hspylib/core/enums/charset.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/core/enums/content_type.py` & `hspylib-1.12.36/hspylib/core/enums/content_type.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/core/enums/enumeration.py` & `hspylib-1.12.36/hspylib/core/enums/enumeration.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/core/enums/http_code.py` & `hspylib-1.12.36/hspylib/core/enums/http_code.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/core/enums/http_method.py` & `hspylib-1.12.36/hspylib/core/enums/http_method.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/core/exception/exceptions.py` & `hspylib-1.12.36/hspylib/core/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/core/metaclass/classpath.py` & `hspylib-1.12.36/hspylib/core/metaclass/classpath.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,39 +8,35 @@
    @created: Wed, 8 Jun 2022
     @author: "<B>H</B>ugo <B>S</B>aporetti <B>J</B>unior")"
       @site: "https://github.com/yorevs/hspylib")
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
-import logging as log
-import os
+from hspylib.core.enums.charset import Charset
+from hspylib.core.exception.exceptions import ResourceNotFoundError, SourceNotFoundError
+from hspylib.core.metaclass.singleton import Singleton
+from hspylib.core.preconditions import check_argument, check_not_none, check_state
 from pathlib import Path
 from textwrap import dedent
 from types import NoneType
 from typing import Optional, TypeAlias, Union
 
-from hspylib.core.enums.charset import Charset
-from hspylib.core.exception.exceptions import ResourceNotFoundError, SourceNotFoundError
-from hspylib.core.metaclass.singleton import Singleton
-from hspylib.core.preconditions import check_argument, check_not_none, check_state
+import logging as log
+import os
 
-AnyPath : TypeAlias = Union[Path, str, NoneType]
+AnyPath: TypeAlias = Union[Path, str, NoneType]
 
 
 class Classpath(metaclass=Singleton):
     """The classpath tells Python applications where to look in the filesystem for source and resource files."""
 
     INSTANCE = None
 
-    def __init__(
-        self,
-        source_root: AnyPath = None,
-        run_dir: AnyPath = None,
-        resource_dir: AnyPath = None):
+    def __init__(self, source_root: AnyPath = None, run_dir: AnyPath = None, resource_dir: AnyPath = None):
 
         if source_root:
             check_state(Path(str(source_root)).exists(), "source_root is not an existing path")
         if run_dir:
             check_state(Path(str(run_dir)).exists(), "run_dir is not an existing path")
 
         self.source_root = Path(os.getenv("SOURCE_ROOT", str(source_root or os.curdir)))
```

### Comparing `hspylib-1.12.35/hspylib/core/metaclass/singleton.py` & `hspylib-1.12.36/hspylib/core/metaclass/singleton.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,23 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
 
-import logging as log
-import sys
 from abc import ABCMeta
-from typing import Any, Type, Union, TypeAlias
-
 from hspylib.core.exception.exceptions import HSBaseException
 from hspylib.core.preconditions import check_not_none
+from typing import Any, Type, TypeAlias, Union
+
+import logging as log
+import sys
 
-SingletonClass : TypeAlias = Union[Type, "Singleton"]
+SingletonClass: TypeAlias = Union[Type, "Singleton"]
 
 
 class Singleton(Type):
     """Singleton pattern is a software design pattern that restricts the instantiation of a class to a singular
     instance. This metaclass enables a class to be singleton."""
 
     _instances = {}
```

### Comparing `hspylib-1.12.35/hspylib/core/namespace.py` & `hspylib-1.12.36/hspylib/core/namespace.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/core/preconditions.py` & `hspylib-1.12.36/hspylib/core/preconditions.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/core/tools/commons.py` & `hspylib-1.12.36/hspylib/core/tools/commons.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/core/tools/dict_tools.py` & `hspylib-1.12.36/hspylib/core/tools/dict_tools.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/core/tools/json_path.py` & `hspylib-1.12.36/hspylib/core/tools/json_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
 
-import re
+from pyparsing import unicode
 from typing import Any, TypeAlias, Union
 
-from pyparsing import unicode
+import re
 
-JsonElement : TypeAlias = Union[list, dict, unicode]
+JsonElement: TypeAlias = Union[list, dict, unicode]
 
 
 class JsonPath:
     """Navigate and"""
 
     RE_JSON_NAME = "[a-zA-Z0-9_\\- ]"
     RE_JSON_ARRAY_INDEX = "[0-9]{1,}"
```

### Comparing `hspylib-1.12.35/hspylib/core/tools/text_tools.py` & `hspylib-1.12.36/hspylib/core/tools/text_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,17 +224,15 @@
 def quote(value: Any) -> str:
     """Quote or double quote the value according to the value type.
     :param value: TODO
     """
     return (
         str(value)
         if not isinstance(value, str)
-        else f'"{value}"'
-        if value.startswith("'") and value.endswith("'")
-        else f"'{value}'"
+        else f'"{value}"' if value.startswith("'") and value.endswith("'") else f"'{value}'"
     )
 
 
 def last_index_of(text: str, substring: str) -> int:
     """Return the last index of substring or -1 if substring was not found in text.
     :param text: TODO
     :param substring: TODO
```

### Comparing `hspylib-1.12.35/hspylib/core/tools/validator.py` & `hspylib-1.12.36/hspylib/core/tools/validator.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/core/zoned_datetime.py` & `hspylib-1.12.36/hspylib/core/zoned_datetime.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/application/application.py` & `hspylib-1.12.36/hspylib/modules/application/application.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/application/argparse/argument_parser.py` & `hspylib-1.12.36/hspylib/modules/application/argparse/argument_parser.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/application/argparse/arguments_builder.py` & `hspylib-1.12.36/hspylib/modules/application/argparse/arguments_builder.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/application/argparse/chained_arguments_builder.py` & `hspylib-1.12.36/hspylib/modules/application/argparse/chained_arguments_builder.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/application/argparse/options_builder.py` & `hspylib-1.12.36/hspylib/modules/application/argparse/options_builder.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/application/argparse/parser_action.py` & `hspylib-1.12.36/hspylib/modules/application/argparse/parser_action.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/application/exit_hooks.py` & `hspylib-1.12.36/hspylib/modules/application/exit_hooks.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/application/exit_status.py` & `hspylib-1.12.36/hspylib/modules/application/exit_status.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/application/version.py` & `hspylib-1.12.36/hspylib/modules/application/version.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/cache/ttl_cache.py` & `hspylib-1.12.36/hspylib/modules/cache/ttl_cache.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/cache/ttl_keyring_be.py` & `hspylib-1.12.36/hspylib/modules/cache/ttl_keyring_be.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/cli/keyboard.py` & `hspylib-1.12.36/hspylib/modules/cli/keyboard.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,25 +8,24 @@
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
+from hspylib.core.enums.enumeration import Enumeration
+from hspylib.core.exception.exceptions import KeyboardInputError
+from typing import List, Optional
+
+import getkey
 import os
 import select
 import string
 import sys
 import termios
-from typing import List, Optional
-
-import getkey
-
-from hspylib.core.enums.enumeration import Enumeration
-from hspylib.core.exception.exceptions import KeyboardInputError
 
 
 # pylint: disable=multiple-statements
 class Keyboard(Enumeration):
     """Provides keyboard interaction with the terminal."""
 
     # fmt: off
@@ -41,21 +40,21 @@
     VK_DOWN         = getkey.keys.DOWN;       VK_SPACE      = getkey.keys.SPACE
     VK_LEFT         = getkey.keys.LEFT;       VK_HOME       = getkey.keys.HOME
     VK_RIGHT        = getkey.keys.RIGHT;      VK_END        = getkey.keys.END
     VK_BACKSPACE    = getkey.keys.BACKSPACE;  VK_PAGE_UP    = getkey.keys.PAGE_UP
     VK_INSERT       = getkey.keys.INSERT;     VK_PAGE_DOWN  = getkey.keys.PAGE_DOWN
     VK_TAB          = '\t';                   VK_SHIFT_TAB  = '\x1b[Z'
 
-    VK_CTRL_A       = '\x01';       VK_CTRL_B = '\x02';       VK_CTRL_C = VK_DISABLED; VK_CTRL_D = '\x04'
+    VK_CTRL_A       = '\x01';       VK_CTRL_B = '\x02';       VK_CTRL_C = '\x03';      VK_CTRL_D = '\x04'
     VK_CTRL_E       = '\x05';       VK_CTRL_F = '\x06';       VK_CTRL_G = '\x07';      VK_CTRL_H = '\x08'
-    VK_CTRL_I       = VK_DISABLED;  VK_CTRL_J = VK_DISABLED;  VK_CTRL_K = '\x0b';      VK_CTRL_L = '\x0c'
-    VK_CTRL_M       = VK_DISABLED;  VK_CTRL_N = '\x0e';       VK_CTRL_O = VK_DISABLED; VK_CTRL_P = '\x10'
-    VK_CTRL_Q       = VK_DISABLED;  VK_CTRL_R = '\x12';       VK_CTRL_S = VK_DISABLED; VK_CTRL_T = '\x14'
-    VK_CTRL_U       = '\x15';       VK_CTRL_V = VK_DISABLED;  VK_CTRL_W = '\x17';      VK_CTRL_X = '\x18'
-    VK_CTRL_Y       = VK_DISABLED;  VK_CTRL_Z = VK_DISABLED
+    VK_CTRL_I       = '\t';         VK_CTRL_J = '\n';         VK_CTRL_K = '\x0b';      VK_CTRL_L = '\x0c'
+    VK_CTRL_M       = '\r';         VK_CTRL_N = '\x0e';       VK_CTRL_O = '\x0f';      VK_CTRL_P = '\x10'
+    VK_CTRL_Q       = '\x11';       VK_CTRL_R = '\x12';       VK_CTRL_S = '\x13';      VK_CTRL_T = '\x14'
+    VK_CTRL_U       = '\x15';       VK_CTRL_V = '\x16';       VK_CTRL_W = '\x17';      VK_CTRL_X = '\x18'
+    VK_CTRL_Y       = '\x19';       VK_CTRL_Z = '\x1a'
 
     # Letters
     VK_a = 'a'; VK_i = 'i'; VK_q = 'q'; VK_y = 'y'
     VK_A = 'A'; VK_I = 'I'; VK_Q = 'Q'; VK_Y = 'Y'
     VK_b = 'b'; VK_j = 'j'; VK_r = 'r'; VK_z = 'z'
     VK_B = 'B'; VK_J = 'J'; VK_R = 'R'; VK_Z = 'Z'
     VK_c = 'c'; VK_k = 'k'; VK_s = 's'
```

### Comparing `hspylib-1.12.35/hspylib/modules/cli/vt100/vt_100.py` & `hspylib-1.12.36/hspylib/modules/cli/vt100/vt_100.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,20 @@
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
-import os
-import re
 from abc import ABC
-
 from hspylib.core.preconditions import check_argument
 
+import os
+import re
+
 
 class Vt100(ABC):
     """
     References:
         - https://vt100.net/docs/vt100-ug/chapter3.html
         - https://espterm.github.io/docs/VT100%20escape%20codes.html
     """
```

### Comparing `hspylib-1.12.35/hspylib/modules/cli/vt100/vt_code.py` & `hspylib-1.12.36/hspylib/modules/cli/vt100/vt_code.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/cli/vt100/vt_color.py` & `hspylib-1.12.36/hspylib/modules/cli/vt100/vt_color.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/eventbus/event.py` & `hspylib-1.12.36/hspylib/modules/eventbus/event.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/eventbus/eventbus.py` & `hspylib-1.12.36/hspylib/modules/eventbus/eventbus.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,17 @@
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
-from typing import Any, Callable, Dict, List
-
 from hspylib.core.exception.exceptions import HSBaseException
 from hspylib.modules.eventbus.event import Event
+from typing import Any, Callable, Dict, List
 
 EVENT_CALLBACK = Callable[[Event], None]
 
 
 def subscribe(bus: str, events: str | list[str]):
     """Method decorator to subscribe to a given bus event."""
```

### Comparing `hspylib-1.12.35/hspylib/modules/fetch/fetch.py` & `hspylib-1.12.36/hspylib/modules/fetch/fetch.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/fetch/http_response.py` & `hspylib-1.12.36/hspylib/modules/fetch/http_response.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/fetch/uri_builder.py` & `hspylib-1.12.36/hspylib/modules/fetch/uri_builder.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/fetch/uri_scheme.py` & `hspylib-1.12.36/hspylib/modules/fetch/uri_scheme.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib/modules/security/security.py` & `hspylib-1.12.36/hspylib/modules/security/security.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/hspylib.egg-info/PKG-INFO` & `hspylib-1.12.36/hspylib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib
-Version: 1.12.35
+Version: 1.12.36
 Summary: HsPyLib - Core python library
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib/
@@ -24,22 +24,23 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: retry
 Requires-Dist: urllib3
 Requires-Dist: cryptocode
 Requires-Dist: cryptography
 Requires-Dist: emoji
-Requires-Dist: getkey
+Requires-Dist: get-key
 Requires-Dist: keyring
 Requires-Dist: pyparsing
 Requires-Dist: pyperclip
 Requires-Dist: PyYAML
 Requires-Dist: toml
 Requires-Dist: requests
 Requires-Dist: urllib3<2.0.0
+Requires-Dist: pyparsing<3.1
 
 <img src="https://iili.io/HYBJFA7.png" width="64" height="64" align="right" />
 
 # HomeSetup Python Library
 >
 > Because your Python code is not JUST a script !
```

### Comparing `hspylib-1.12.35/hspylib.egg-info/SOURCES.txt` & `hspylib-1.12.36/hspylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.35/setup.py` & `hspylib-1.12.36/setup.py`

 * *Files identical despite different names*


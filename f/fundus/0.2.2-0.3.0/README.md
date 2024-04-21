# Comparing `tmp/fundus-0.2.2.tar.gz` & `tmp/fundus-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fundus-0.2.2.tar", last modified: Thu Apr  4 11:44:46 2024, max compression
+gzip compressed data, was "fundus-0.3.0.tar", last modified: Sun Apr 21 19:42:17 2024, max compression
```

## Comparing `fundus-0.2.2.tar` & `fundus-0.3.0.tar`

### file list

```diff
@@ -1,99 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.888215 fundus-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-04 11:44:40.000000 fundus-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 11:44:40.000000 fundus-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-04-04 11:44:46.888215 fundus-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-04 11:44:40.000000 fundus-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-04 11:44:40.000000 fundus-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 11:44:46.888215 fundus-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.872215 fundus-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.872215 fundus-0.2.2/src/fundus/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.876215 fundus-0.2.2/src/fundus/logging/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.876215 fundus-0.2.2/src/fundus/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/parser/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/parser/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/parser/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.876215 fundus-0.2.2/src/fundus/publishers/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.876215 fundus-0.2.2/src/fundus/publishers/at/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/at/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/at/orf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/base_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.880215 fundus-0.2.2/src/fundus/publishers/de/
--rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/berliner_zeitung.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/bild.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/braunschweiger_zeitung.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/business_insider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/die_welt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/die_zeit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/dw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/faz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/focus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/mdr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/merkur.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/ndr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/ntv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/spon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/stern.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/sz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/tagesschau.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/taz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/waz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.880215 fundus-0.2.2/src/fundus/publishers/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/fr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/fr/le_monde.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.880215 fundus-0.2.2/src/fundus/publishers/na/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/na/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/na/the_namibian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.880215 fundus-0.2.2/src/fundus/publishers/uk/
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/uk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/uk/i_news.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/uk/the_guardian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/uk/the_independent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/uk/the_telegraph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.884215 fundus-0.2.2/src/fundus/publishers/us/
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/ap_news.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/cnbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/fox_news.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/free_beacon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/la_times.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/occupy_democrats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/reuters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/the_gateway_pundit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/the_intercept.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/the_nation_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/the_new_yorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/washington_times_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/world_truth.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.884215 fundus-0.2.2/src/fundus/scraping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/article.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.884215 fundus-0.2.2/src/fundus/scraping/common_crawl/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/common_crawl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/common_crawl/html.py
--rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/common_crawl/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/common_crawl/scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/html.py
--rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.884215 fundus-0.2.2/src/fundus/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/utils/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/utils/more_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.884215 fundus-0.2.2/src/fundus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-04-04 11:44:46.000000 fundus-0.2.2/src/fundus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-04 11:44:46.000000 fundus-0.2.2/src/fundus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:44:46.000000 fundus-0.2.2/src/fundus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-04 11:44:46.000000 fundus-0.2.2/src/fundus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 11:44:46.000000 fundus-0.2.2/src/fundus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.884215 fundus-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-04 11:44:40.000000 fundus-0.2.2/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-04-04 11:44:40.000000 fundus-0.2.2/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-04 11:44:40.000000 fundus-0.2.2/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.625123 fundus-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-21 19:42:13.000000 fundus-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-21 19:42:13.000000 fundus-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-04-21 19:42:17.625123 fundus-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-21 19:42:13.000000 fundus-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-21 19:42:13.000000 fundus-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:42:17.625123 fundus-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.609123 fundus-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.609123 fundus-0.3.0/src/fundus/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.613123 fundus-0.3.0/src/fundus/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.613123 fundus-0.3.0/src/fundus/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/parser/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/parser/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/parser/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.613123 fundus-0.3.0/src/fundus/publishers/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.613123 fundus-0.3.0/src/fundus/publishers/at/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/at/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/at/orf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8394 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/base_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.613123 fundus-0.3.0/src/fundus/publishers/ch/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/ch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/ch/srf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.617123 fundus-0.3.0/src/fundus/publishers/de/
+-rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/berliner_zeitung.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/bild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/braunschweiger_zeitung.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/business_insider_de.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/die_welt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/die_zeit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/dw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/faz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/focus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/mdr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/merkur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/ndr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/ntv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/rheinische_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/spon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/stern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/sz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/tagesschau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/taz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/waz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.617123 fundus-0.3.0/src/fundus/publishers/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/fr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/fr/le_monde.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.617123 fundus-0.3.0/src/fundus/publishers/lt/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/lt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/lt/lrt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.617123 fundus-0.3.0/src/fundus/publishers/na/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/na/the_namibian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.617123 fundus-0.3.0/src/fundus/publishers/uk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/uk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/uk/i_news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/uk/the_guardian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/uk/the_independent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/uk/the_telegraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.621123 fundus-0.3.0/src/fundus/publishers/us/
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/ap_news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/business_insider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/cnbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/fox_news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/free_beacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/la_times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/occupy_democrats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/reuters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/the_gateway_pundit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/the_intercept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/the_nation_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/the_new_yorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/washington_times_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/world_truth.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.621123 fundus-0.3.0/src/fundus/scraping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/article.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18725 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8368 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.621123 fundus-0.3.0/src/fundus/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/utils/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.625123 fundus-0.3.0/src/fundus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-04-21 19:42:17.000000 fundus-0.3.0/src/fundus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-21 19:42:17.000000 fundus-0.3.0/src/fundus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:42:17.000000 fundus-0.3.0/src/fundus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-21 19:42:17.000000 fundus-0.3.0/src/fundus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 19:42:17.000000 fundus-0.3.0/src/fundus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.625123 fundus-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-21 19:42:13.000000 fundus-0.3.0/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-21 19:42:13.000000 fundus-0.3.0/tests/test_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-21 19:42:13.000000 fundus-0.3.0/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-04-21 19:42:13.000000 fundus-0.3.0/tests/test_parser.py
```

### Comparing `fundus-0.2.2/LICENSE` & `fundus-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/PKG-INFO` & `fundus-0.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fundus
-Version: 0.2.2
+Version: 0.3.0
 Summary: A very simple news crawler
 Author-email: Max Dallabetta <max.dallabetta@googlemail.com>
 License: MIT
 Project-URL: Repository, https://github.com/flairNLP/fundus
 Keywords: web scraping, web crawling
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,27 +17,25 @@
 License-File: LICENSE
 Requires-Dist: python-dateutil<3,>=2.8
 Requires-Dist: lxml<5,>=4.9
 Requires-Dist: more-itertools<10,>=9.1
 Requires-Dist: cssselect<2,>=1.1
 Requires-Dist: feedparser<7,>=6.0
 Requires-Dist: colorama<1,>=0.4
-Requires-Dist: typing-extensions<5,>=4.0
+Requires-Dist: typing-extensions<5,>=4.6
 Requires-Dist: langdetect<2,>=1.0
-Requires-Dist: aiohttp<4,>=3.8
-Requires-Dist: aioitertools<1,>=0.11
 Requires-Dist: validators!=0.23,<1,>=0.20
 Requires-Dist: requests<3,>=2.28
 Requires-Dist: tqdm<5,>=4.66
 Requires-Dist: fastwarc<1,>=0.14
 Requires-Dist: chardet<6,>=5.2
 Requires-Dist: dill<1,>=0.3
 Provides-Extra: dev
 Requires-Dist: pytest~=7.2.2; extra == "dev"
-Requires-Dist: mypy==1.1.1; extra == "dev"
+Requires-Dist: mypy==1.9.0; extra == "dev"
 Requires-Dist: isort==5.12.0; extra == "dev"
 Requires-Dist: black==23.1.0; extra == "dev"
 Requires-Dist: types-lxml; extra == "dev"
 Requires-Dist: types-python-dateutil<3,>=2.8; extra == "dev"
 Requires-Dist: types-requests<3,>=2.28; extra == "dev"
 Requires-Dist: types-colorama<1,>=0.4; extra == "dev"
 
@@ -49,23 +47,23 @@
   </picture>
 </p>
 
 <p align="center">A very simple <b>news crawler</b> in Python.
 Developed at <a href="https://www.informatik.hu-berlin.de/en/forschung-en/gebiete/ml-en/">Humboldt University of Berlin</a>.
 </p>
 <p align="center">
-<img alt="version" src="https://img.shields.io/badge/version-0.1-green">
+<a href="https://pypi.org/project/fundus/"><img alt="PyPi version" src="https://badge.fury.io/py/fundus.svg"></a>
 <img alt="python" src="https://img.shields.io/badge/python-3.8-blue">
 <img alt="Static Badge" src="https://img.shields.io/badge/license-MIT-green">
 <img alt="Publisher Coverage" src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/dobbersc/ca0ae056b05cbfeaf30fa42f84ddf458/raw/fundus_publisher_coverage.json">
 </p>
 <div align="center">
 <hr>
 
-[Quick Start](#quick-start) |  [Tutorials](#tutorials)  | [News Sources](/docs/supported_publishers.md)
+[Quick Start](#quick-start) | [Tutorials](#tutorials) | [News Sources](/docs/supported_publishers.md) | [Paper](https://arxiv.org/abs/2403.15279)
 
 </div>
 
 
 ---
 
 Fundus is:
@@ -138,16 +136,16 @@
 ## Example 2: Crawl a specific news source
 
 Maybe you want to crawl a specific news source instead. Let's crawl news articles from Washington Times only:
 
 ```python
 from fundus import PublisherCollection, Crawler
 
-# initialize the crawler for Washington Times
-crawler = Crawler(PublisherCollection.us.WashingtonTimes)
+# initialize the crawler for The New Yorker
+crawler = Crawler(PublisherCollection.us.TheNewYorker)
 
 # crawl 2 articles and print
 for article in crawler.crawl(max_articles=2):
     print(article)
 ```
 
 ## Example 3: Crawl articles from CC-NEWS
@@ -182,14 +180,43 @@
 
 ## Currently Supported News Sources
 
 You can find the publishers currently supported [**here**](/docs/supported_publishers.md).
 
 Also: **Adding a new publisher is easy - consider contributing to the project!**
 
+## Evaluation benchmark
+
+Check out our evaluation [benchmark](https://github.com/dobbersc/fundus-evaluation).
+
+| **Scraper** | **Precision**             | **Recall**                | **F1-Score**              |
+|-------------|---------------------------|---------------------------|---------------------------|
+| [Fundus](https://github.com/flairNLP/fundus)      | **99.89**<sub>±0.57</sub> | 96.75<sub>±12.75</sub>    | **97.69**<sub>±9.75</sub> |
+| [Trafilatura](https://github.com/adbar/trafilatura) | 90.54<sub>±18.86</sub>    | 93.23<sub>±23.81</sub>    | 89.81<sub>±23.69</sub>    |
+| [BTE](https://github.com/dobbersc/fundus-evaluation/blob/master/src/fundus_evaluation/scrapers/bte.py)         | 81.09<sub>±19.41</sub>    | **98.23**<sub>±8.61</sub> | 87.14<sub>±15.48</sub>    |
+| [jusText](https://github.com/miso-belica/jusText)     | 86.51<sub>±18.92</sub>    | 90.23<sub>±20.61</sub>    | 86.96<sub>±19.76</sub>    |
+| [news-please](https://github.com/fhamborg/news-please) | 92.26<sub>±12.40</sub>    | 86.38<sub>±27.59</sub>    | 85.81<sub>±23.29</sub>    |
+| [BoilerNet](https://github.com/dobbersc/fundus-evaluation/tree/master/src/fundus_evaluation/scrapers/boilernet)   | 84.73<sub>±20.82</sub>    | 90.66<sub>±21.05</sub>    | 85.77<sub>±20.28</sub>    |
+| [Boilerpipe](https://github.com/kohlschutter/boilerpipe)  | 82.89<sub>±20.65</sub>    | 82.11<sub>±29.99</sub>    | 79.90<sub>±25.86</sub>    |
+
+## Cite
+
+Please cite the following [paper](https://arxiv.org/abs/2403.15279) when using Fundus or building upon our work:
+
+```bibtex
+@misc{dallabetta2024fundus,
+      title={Fundus: A Simple-to-Use News Scraper Optimized for High Quality Extractions}, 
+      author={Max Dallabetta and Conrad Dobberstein and Adrian Breiding and Alan Akbik},
+      year={2024},
+      eprint={2403.15279},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
+```
+
 ## Contact
 
 Please email your questions or comments to [**Max Dallabetta**](mailto:max.dallabetta@googlemail.com?subject=[GitHub]%20Fundus)
 
 ## Contributing
 
 Thanks for your interest in contributing! There are many ways to get involved;
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,36 +1,35 @@
-Metadata-Version: 2.1 Name: fundus Version: 0.2.2 Summary: A very simple news
+Metadata-Version: 2.1 Name: fundus Version: 0.3.0 Summary: A very simple news
 crawler Author-email: Max Dallabetta
 googlemail.com> License: MIT Project-URL: Repository, https://github.com/
 flairNLP/fundus Keywords: web scraping, web crawling Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: python-dateutil<3,>=2.8
 Requires-Dist: lxml<5,>=4.9 Requires-Dist: more-itertools<10,>=9.1 Requires-
 Dist: cssselect<2,>=1.1 Requires-Dist: feedparser<7,>=6.0 Requires-Dist:
-colorama<1,>=0.4 Requires-Dist: typing-extensions<5,>=4.0 Requires-Dist:
-langdetect<2,>=1.0 Requires-Dist: aiohttp<4,>=3.8 Requires-Dist:
-aioitertools<1,>=0.11 Requires-Dist: validators!=0.23,<1,>=0.20 Requires-Dist:
+colorama<1,>=0.4 Requires-Dist: typing-extensions<5,>=4.6 Requires-Dist:
+langdetect<2,>=1.0 Requires-Dist: validators!=0.23,<1,>=0.20 Requires-Dist:
 requests<3,>=2.28 Requires-Dist: tqdm<5,>=4.66 Requires-Dist: fastwarc<1,>=0.14
 Requires-Dist: chardet<6,>=5.2 Requires-Dist: dill<1,>=0.3 Provides-Extra: dev
-Requires-Dist: pytest~=7.2.2; extra == "dev" Requires-Dist: mypy==1.1.1; extra
+Requires-Dist: pytest~=7.2.2; extra == "dev" Requires-Dist: mypy==1.9.0; extra
 == "dev" Requires-Dist: isort==5.12.0; extra == "dev" Requires-Dist:
 black==23.1.0; extra == "dev" Requires-Dist: types-lxml; extra == "dev"
 Requires-Dist: types-python-dateutil<3,>=2.8; extra == "dev" Requires-Dist:
 types-requests<3,>=2.28; extra == "dev" Requires-Dist: types-colorama<1,>=0.4;
 extra == "dev"
                                     [Logo]
    A very simple nneewwss ccrraawwlleerr in Python. Developed at _H_u_m_b_o_l_d_t_ _U_n_i_v_e_r_s_i_t_y_ _o_f
                                     _B_e_r_l_i_n.
-              [version][python][Static Badge][Publisher Coverage]
+           _[_P_y_P_i_ _v_e_r_s_i_o_n_][python][Static Badge][Publisher Coverage]
 ===============================================================================
  [Quick Start](#quick-start) | [Tutorials](#tutorials) | [News Sources](/docs/
-                           supported_publishers.md)
+     supported_publishers.md) | [Paper](https://arxiv.org/abs/2403.15279)
 --- Fundus is: * **A static news crawler.** Fundus lets you crawl online news
 articles with only a few lines of Python code! Be it from live websites or the
 CC-NEWS dataset. * **An open-source Python package.** Fundus is built on the
 idea of building something together. We welcome your contribution to help
 Fundus [grow](docs/how_to_contribute.md)!
 ===============================================================================
 ## Quick Start To install from pip, simply do: ``` pip install fundus ```
@@ -54,17 +53,17 @@
 funding-poster-critical-lgbtq-community - From: FoxNews (2023-05-09 14:37) ```
 This printout tells you that you successfully crawled two articles! For each
 article, the printout details: - the "Title" of the article, i.e. its headline
 - the "Text", i.e. the main article body text - the "URL" from which it was
 crawled - the news source it is "From" ## Example 2: Crawl a specific news
 source Maybe you want to crawl a specific news source instead. Let's crawl news
 articles from Washington Times only: ```python from fundus import
-PublisherCollection, Crawler # initialize the crawler for Washington Times
-crawler = Crawler(PublisherCollection.us.WashingtonTimes) # crawl 2 articles
-and print for article in crawler.crawl(max_articles=2): print(article) ``` ##
+PublisherCollection, Crawler # initialize the crawler for The New Yorker
+crawler = Crawler(PublisherCollection.us.TheNewYorker) # crawl 2 articles and
+print for article in crawler.crawl(max_articles=2): print(article) ``` ##
 Example 3: Crawl articles from CC-NEWS If you're not familiar with CC-NEWS,
 check out their [paper](https://paperswithcode.com/dataset/cc-news). ````python
 from fundus import PublisherCollection, CCNewsCrawler # initialize the crawler
 for news publishers based in the US crawler = CCNewsCrawler
 (*PublisherCollection.us) # crawl 2 articles and print for article in
 crawler.crawl(max_articles=2): print(article) ```` ## Tutorials We provide
 **quick tutorials** to get you started with the library: 1. [**Tutorial 1: How
@@ -74,13 +73,33 @@
 filter articles**](docs/4_how_to_filter_articles.md) 5. [**Tutorial 5: How to
 search for publishers**](docs/5_how_to_search_for_publishers.md) If you wish to
 contribute check out these tutorials: 1. [**How to contribute**](docs/
 how_to_contribute.md) 2. [**How to add a publisher**](docs/
 how_to_add_a_publisher.md) ## Currently Supported News Sources You can find the
 publishers currently supported [**here**](/docs/supported_publishers.md). Also:
 **Adding a new publisher is easy - consider contributing to the project!** ##
+Evaluation benchmark Check out our evaluation [benchmark](https://github.com/
+dobbersc/fundus-evaluation). | **Scraper** | **Precision** | **Recall** | **F1-
+Score** | |-------------|---------------------------|--------------------------
+-|---------------------------| | [Fundus](https://github.com/flairNLP/fundus) |
+**99.89**Â±0.57 | 96.75Â±12.75 | **97.69**Â±9.75 | | [Trafilatura](https://
+github.com/adbar/trafilatura) | 90.54Â±18.86 | 93.23Â±23.81 | 89.81Â±23.69 | |
+[BTE](https://github.com/dobbersc/fundus-evaluation/blob/master/src/
+fundus_evaluation/scrapers/bte.py) | 81.09Â±19.41 | **98.23**Â±8.61 |
+87.14Â±15.48 | | [jusText](https://github.com/miso-belica/jusText) |
+86.51Â±18.92 | 90.23Â±20.61 | 86.96Â±19.76 | | [news-please](https://
+github.com/fhamborg/news-please) | 92.26Â±12.40 | 86.38Â±27.59 | 85.81Â±23.29 |
+| [BoilerNet](https://github.com/dobbersc/fundus-evaluation/tree/master/src/
+fundus_evaluation/scrapers/boilernet) | 84.73Â±20.82 | 90.66Â±21.05 |
+85.77Â±20.28 | | [Boilerpipe](https://github.com/kohlschutter/boilerpipe) |
+82.89Â±20.65 | 82.11Â±29.99 | 79.90Â±25.86 | ## Cite Please cite the following
+[paper](https://arxiv.org/abs/2403.15279) when using Fundus or building upon
+our work: ```bibtex @misc{dallabetta2024fundus, title={Fundus: A Simple-to-Use
+News Scraper Optimized for High Quality Extractions}, author={Max Dallabetta
+and Conrad Dobberstein and Adrian Breiding and Alan Akbik}, year={2024},
+eprint={2403.15279}, archivePrefix={arXiv}, primaryClass={cs.CL} } ``` ##
 Contact Please email your questions or comments to [**Max Dallabetta**](mailto:
 max.dallabetta@googlemail.com?subject=[GitHub]%20Fundus) ## Contributing Thanks
 for your interest in contributing! There are many ways to get involved; start
 with our [contributor guidelines](docs/how_to_contribute.md) and then check
 these [open issues](https://github.com/flairNLP/fundus/issues) for specific
 tasks. ## License [MIT](LICENSE)
```

### Comparing `fundus-0.2.2/pyproject.toml` & `fundus-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fundus"
-version = "0.2.2"
+version = "0.3.0"
 authors = [
     { name = "Max Dallabetta", email = "max.dallabetta@googlemail.com" },
 ]
 description = "A very simple news crawler"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -25,33 +25,31 @@
 dependencies = [
     "python-dateutil>=2.8, <3",
     "lxml>=4.9, <5",
     "more-itertools>=9.1, <10",
     "cssselect>=1.1, <2",
     "feedparser>=6.0, <7",
     "colorama>=0.4, <1",
-    "typing-extensions>=4.0, <5",
+    "typing-extensions>=4.6, <5",
     "langdetect>=1.0, <2",
-    "aiohttp>=3.8, <4",
-    "aioitertools>=0.11, <1",
     "validators>=0.20, <1, !=0.23",
     "requests>=2.28, <3",
     "tqdm>=4.66, <5",
     "fastwarc>=0.14, <1",
     "chardet>=5.2, <6",
     "dill>=0.3, <1"
 ]
 
 [project.urls]
 "Repository" = "https://github.com/flairNLP/fundus"
 
 [project.optional-dependencies]
 dev = [
     "pytest~=7.2.2",
-    "mypy==1.1.1",
+    "mypy==1.9.0",
     "isort==5.12.0",
     "black==23.1.0",
     # type stubs
     "types-lxml",
     "types-python-dateutil>=2.8, <3",
     "types-requests>=2.28, <3",
     "types-colorama>=0.4, <1",
```

### Comparing `fundus-0.2.2/src/fundus/parser/base_parser.py` & `fundus-0.3.0/src/fundus/parser/base_parser.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/parser/data.py` & `fundus-0.3.0/src/fundus/parser/data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from abc import ABC
+from abc import ABC, abstractmethod
 from dataclasses import dataclass, fields
 from typing import (
     Any,
     Collection,
     Dict,
     Iterable,
     Iterator,
@@ -10,22 +10,20 @@
     Optional,
     Sequence,
     Tuple,
     Union,
     overload,
 )
 
-from typing_extensions import TypeAlias
-
-from fundus.logging import basic_logger
-
-_displayed_deprecation_info = False
+from typing_extensions import Self, TypeAlias
 
 LDMappingValue: TypeAlias = Union[List[Dict[str, Any]], Dict[str, Any]]
 
+_sentinel = object()
+
 
 class LinkedDataMapping:
     """
     This class is a @type -> LD mapping.
     Given LD:
         ld_1 = {
             @type: 'Article'
@@ -62,34 +60,14 @@
             else:
                 self.__dict__[ld_type] = ld
         else:
             if not self.__dict__.get(self.__UNKNOWN_TYPE__):
                 self.__dict__[self.__UNKNOWN_TYPE__] = []
             self.__dict__[self.__UNKNOWN_TYPE__].append(ld)
 
-    def get(self, ld_type: str, default: Any = None) -> Optional[LDMappingValue]:
-        """
-        This function works like get() on a mapping. It will return all LDs containing
-        the given <ld_type>. If there are multiple LDs of the same '@type' this function
-        returns a list instead of a dictionary.
-
-        :param ld_type: The key to search for
-        :param default: The returned default if <key> is not found, default: None
-        :return: The reached value or <default>
-        """
-        global _displayed_deprecation_info
-
-        if not _displayed_deprecation_info:
-            _displayed_deprecation_info = True
-            basic_logger.warning(
-                "LinkedDate.get() will be deprecated in the future. Use .get_value_by_key_path() "
-                "or .bf_search() instead"
-            )
-        return self.__dict__.get(ld_type, default)
-
     def get_value_by_key_path(self, key_path: List[str], default: Any = None) -> Optional[Any]:
         """
         Works like get() except this one assumes a path is given as list of keys (str).
         I.e:
             key_path := ["mainEntity", "author"], default := {}
             results in self._ld_by_type.get("mainEntity").get("author")
 
@@ -143,27 +121,36 @@
         :param key: The dict key to search for
         :param depth: The searched depth, default None
         :return: The content of the first matched key or None
         """
 
         def search_recursive(nodes: Iterable[LDMappingValue], current_depth: int):
             if current_depth == depth:
-                return None
+                return _sentinel
             else:
                 new: List[Dict[str, Any]] = []
                 for node in nodes:
                     if isinstance(node, list):
                         new.extend(node)
                         continue
-                    elif value := node.get(key):
+                    elif (value := node.get(key, _sentinel)) is not _sentinel:
                         return value
                     new.extend(v for v in node.values() if isinstance(v, dict))
-                return search_recursive(new, current_depth + 1) if new else None
 
-        return search_recursive([self.__dict__], 0) or default
+                if not new:
+                    return _sentinel
+
+                return search_recursive(new, current_depth + 1)
+
+        result = search_recursive([self.__dict__], 0)
+
+        if result == _sentinel:
+            return default
+
+        return result
 
     def __repr__(self):
         return f"LD containing '{', '.join(content)}'" if (content := self.__dict__.keys()) else "Empty LD"
 
 
 class TextSequence(Sequence[str]):
     def __init__(self, texts: Iterable[str]):
@@ -188,17 +175,24 @@
 
     def __repr__(self) -> str:
         return repr(self._data)
 
     def __str__(self) -> str:
         return "\n".join(self)
 
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, TextSequence):
+            return NotImplemented
+        return self._data == other._data
+
 
 @dataclass
 class TextSequenceTree(ABC):
+    """Base class to traverse and build trees of TextSequence."""
+
     def as_text_sequence(self) -> TextSequence:
         texts = [text for tl in self.df_traversal() for text in tl]
         return TextSequence(texts)
 
     def text(self, join_on: str = "\n\n") -> str:
         return join_on.join(self.as_text_sequence())
 
@@ -211,15 +205,24 @@
                     yield from el
             else:
                 yield o
 
         for value in self:
             yield from recursion(value)
 
-    def __iter__(self):
+    @abstractmethod
+    def serialize(self) -> Dict[str, Any]:
+        pass
+
+    @classmethod
+    @abstractmethod
+    def deserialize(cls, serialized: Dict[str, Any]) -> Self:
+        pass
+
+    def __iter__(self) -> Iterator[Any]:
         field_values = [getattr(self, f.name) for f in fields(self)]
         yield from field_values
 
     def __str__(self):
         return self.text()
 
     def __bool__(self) -> bool:
@@ -227,12 +230,35 @@
 
 
 @dataclass
 class ArticleSection(TextSequenceTree):
     headline: TextSequence
     paragraphs: TextSequence
 
+    def serialize(self) -> Dict[str, Any]:
+        return {
+            "headline": list(self.headline),
+            "paragraphs": list(self.paragraphs),
+        }
+
+    @classmethod
+    def deserialize(cls, serialized: Dict[str, Any]) -> Self:
+        return cls(headline=TextSequence(serialized["headline"]), paragraphs=TextSequence(serialized["paragraphs"]))
+
 
 @dataclass
 class ArticleBody(TextSequenceTree):
     summary: TextSequence
     sections: List[ArticleSection]
+
+    def serialize(self) -> Dict[str, Any]:
+        return {
+            "summary": list(self.summary),
+            "sections": [section.serialize() for section in self.sections],
+        }
+
+    @classmethod
+    def deserialize(cls, serialized: Dict[str, Any]) -> Self:
+        return cls(
+            summary=TextSequence(serialized["summary"]),
+            sections=[ArticleSection.deserialize(section) for section in serialized["sections"]],
+        )
```

### Comparing `fundus-0.2.2/src/fundus/parser/utility.py` & `fundus-0.3.0/src/fundus/parser/utility.py`

 * *Files 3% similar despite different names*

```diff
@@ -244,7 +244,19 @@
 
 
 _tz_infos = {"CET": 3600, "CEST": 7200}
 
 
 def generic_date_parsing(date_str: Optional[str]) -> Optional[datetime]:
     return parser.parse(date_str, tzinfos=_tz_infos) if date_str else None
+
+
+_title_selector = CSSSelector("title")
+
+
+def parse_title_from_root(root: lxml.html.HtmlElement) -> Optional[str]:
+    title_node = _title_selector(root)
+
+    if len(title_node) != 1:
+        return None
+
+    return strip_nodes_to_text(title_node)
```

### Comparing `fundus-0.2.2/src/fundus/publishers/at/orf.py` & `fundus-0.3.0/src/fundus/publishers/at/orf.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/base_objects.py` & `fundus-0.3.0/src/fundus/publishers/base_objects.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,78 @@
 import inspect
 from dataclasses import dataclass, field
 from enum import Enum, EnumMeta, unique
+from itertools import islice
 from typing import Any, Dict, Iterator, List, Optional, Type
 
 from fundus.parser.base_parser import ParserProxy
 from fundus.scraping.filter import URLFilter
-from fundus.scraping.html import FundusSource, NewsMap, RSSFeed, Sitemap, URLSource
+from fundus.scraping.url import NewsMap, RSSFeed, Sitemap, URLSource
 from fundus.utils.iteration import iterate_all_subclasses
 
 
 @dataclass(frozen=True)
 class PublisherSpec:
     name: str
     domain: str
     parser: Type[ParserProxy]
     sources: List[URLSource]
+    query_parameter: Dict[str, str] = field(default_factory=dict)
     url_filter: Optional[URLFilter] = field(default=None)
     request_header: Dict[str, str] = field(default_factory=dict)
 
 
+class PublisherEnumMeta(EnumMeta):
+    def __str__(self) -> str:
+        representation = f"Region {self.__name__!r} containing {len(self)} publisher(s):"
+        publisher: str
+        for publisher in self.__members__.values():
+            representation += f"\n\t {publisher}"
+        return representation
+
+
 @unique
-class PublisherEnum(Enum):
+class PublisherEnum(Enum, metaclass=PublisherEnumMeta):
     def __new__(cls, *args, **kwargs):
         value = len(cls.__members__) + 1
         obj = object.__new__(cls)
         obj._value_ = value
         return obj
 
     def __init__(self, spec: PublisherSpec):
         if not isinstance(spec, PublisherSpec):
             raise ValueError("Your only allowed to generate 'PublisherEnum's from 'PublisherSpec")
         self.domain = spec.domain
         self.parser = spec.parser()
         self.publisher_name = spec.name
+        self.query_parameter = spec.query_parameter
         self.url_filter = spec.url_filter
+        self.request_header = spec.request_header
 
         # we define the dict here manually instead of using default dict so that we can control
         # the order in which sources are proceeded.
-        source_mapping: Dict[Type[URLSource], List[FundusSource]] = {
+        source_mapping: Dict[Type[URLSource], List[URLSource]] = {
             RSSFeed: [],
             NewsMap: [],
             Sitemap: [],
         }
 
         for url_source in spec.sources:
             if not isinstance(url_source, URLSource):
                 raise TypeError(
                     f"Unexpected type '{type(url_source).__name__}' as source for {self.name}. "
                     f"Allowed are '{', '.join(cls.__name__ for cls in iterate_all_subclasses(URLSource))}'"
                 )
-            source: FundusSource = FundusSource(
-                url_source=url_source,
-                publisher=self.publisher_name,
-                url_filter=spec.url_filter,
-                request_header=spec.request_header,
-            )
-            source_mapping[type(url_source)].append(source)
+            source_mapping[type(url_source)].append(url_source)
 
         self.source_mapping = source_mapping
 
+    def __str__(self) -> str:
+        return f"{self.publisher_name}"
+
     def supports(self, source_types: List[Type[URLSource]]) -> bool:
         if not source_types:
             raise ValueError(f"Got empty value '{source_types}' for parameter <source_types>.")
         for source_type in source_types:
             if not inspect.isclass(source_type) or not issubclass(source_type, URLSource):
                 raise TypeError(
                     f"Got unexpected type '{source_type}'. "
@@ -189,7 +199,23 @@
     def __len__(cls) -> int:
         """The number of publishers included in the collection.
 
         Returns:
             int: The number of publishers.
         """
         return len(list(iter(cls)))
+
+    def __str__(self) -> str:
+        enum_mapping = self.get_publisher_enum_mapping()
+        enum_mapping_keys = enum_mapping.keys()
+        representation = (
+            f"The {self.__name__!r} consists of {len(self)} publishers from {len(enum_mapping_keys)} , including:"
+        )
+        publisher: str
+        country: str
+        for country in enum_mapping_keys:
+            representation += f"\n\t {country}:"
+            for publisher in islice(enum_mapping[country], 0, 5):
+                representation += f"\n\t\t {publisher}"
+            if len(enum_mapping[country]) > 5:
+                representation += f"\n\t\t ..."
+        return representation
```

### Comparing `fundus-0.2.2/src/fundus/publishers/de/__init__.py` & `fundus-0.3.0/src/fundus/publishers/de/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from datetime import datetime
 
 from dateutil.rrule import MONTHLY, rrule
 
 from fundus.publishers.base_objects import PublisherEnum, PublisherSpec
 from fundus.scraping.filter import regex_filter
-from fundus.scraping.html import NewsMap, RSSFeed, Sitemap
+from fundus.scraping.url import NewsMap, RSSFeed, Sitemap
 
 from .berliner_zeitung import BerlinerZeitungParser
 from .bild import BildParser
 from .braunschweiger_zeitung import BSZParser
-from .business_insider import BusinessInsiderParser
+from .business_insider_de import BusinessInsiderDEParser
 from .die_welt import DieWeltParser
 from .die_zeit import DieZeitParser
 from .dw import DWParser
 from .faz import FAZParser
 from .focus import FocusParser
 from .mdr import MDRParser
 from .merkur import MerkurParser
 from .ndr import NDRParser
 from .ntv import NTVParser
+from .rheinische_post import RheinischePostParser
 from .spon import SPONParser
 from .stern import SternParser
 from .sz import SZParser
 from .tagesschau import TagesschauParser
 from .taz import TazParser
 from .waz import WAZParser
 
@@ -154,15 +155,15 @@
         domain="https://www.stern.de/",
         sources=[RSSFeed("https://www.stern.de/feed/standard/alle-nachrichten/")],
         parser=SternParser,
     )
 
     NTV = PublisherSpec(
         name="N-Tv",
-        domain="https://www.ntv.de/",
+        domain="https://www.n-tv.de/",
         sources=[NewsMap("https://www.n-tv.de/news.xml"), Sitemap("https://www.n-tv.de/sitemap.xml")],
         parser=NTVParser,
     )
 
     NDR = PublisherSpec(
         name="Norddeutscher Rundfunk (NDR)",
         domain="https://www.ndr.de/",
@@ -172,15 +173,15 @@
         ],
         parser=NDRParser,
         url_filter=regex_filter("podcast[0-9]{4}|/index.html"),
     )
 
     Taz = PublisherSpec(
         name="Die Tageszeitung (taz)",
-        domain="https://www.taz.de/",
+        domain="https://taz.de/",
         sources=[
             NewsMap("https://taz.de/sitemap-google-news.xml"),
             Sitemap("https://taz.de/sitemap-index.xml"),
         ],
         parser=TazParser,
     )
 
@@ -214,16 +215,27 @@
                 f"https://www.braunschweiger-zeitung.de/sitemaps/archive/sitemap-{d.year}-{str(d.month).zfill(2)}-p00.xml.gz"
             )
             for d in reversed(list(rrule(MONTHLY, dtstart=datetime(2016, 9, 1), until=datetime.now())))
         ],
         parser=BSZParser,
     )
 
-    BusinessInsider = PublisherSpec(
-        name="Business Insider",
+    BusinessInsiderDE = PublisherSpec(
+        name="Business Insider DE",
         domain="https://www.businessinsider.de/",
         sources=[
             NewsMap("https://www.businessinsider.de/news-sitemap.xml"),
             Sitemap("https://www.businessinsider.de/sitemap_index.xml"),
         ],
-        parser=BusinessInsiderParser,
+        parser=BusinessInsiderDEParser,
+    )
+
+    RheinischePost = PublisherSpec(
+        name="Rheinische Post",
+        domain="https://rp-online.de/",
+        sources=[
+            RSSFeed("https://rp-online.de/feed.rss"),
+            NewsMap("https://rp-online.de/sitemap-news.xml"),
+            Sitemap("https://rp-online.de/sitemap.xml"),
+        ],
+        parser=RheinischePostParser,
     )
```

### Comparing `fundus-0.2.2/src/fundus/publishers/de/berliner_zeitung.py` & `fundus-0.3.0/src/fundus/publishers/de/berliner_zeitung.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/de/bild.py` & `fundus-0.3.0/src/fundus/publishers/de/bild.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/de/braunschweiger_zeitung.py` & `fundus-0.3.0/src/fundus/publishers/de/braunschweiger_zeitung.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/de/business_insider.py` & `fundus-0.3.0/src/fundus/publishers/de/business_insider_de.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,30 +9,28 @@
     extract_article_body_with_selector,
     generic_author_parsing,
     generic_date_parsing,
     generic_topic_parsing,
 )
 
 
-class BusinessInsiderParser(ParserProxy):
+class BusinessInsiderDEParser(ParserProxy):
     class V1(BaseParser):
-        _summary_selector = CSSSelector("article div.bi-bulletpoints > p")
-        _subheadline_selector = CSSSelector("article h2")
-
+        _summary_selector = CSSSelector("article div.bi-bulletpoints li, article div.bi-bulletpoints > p")
+        _subheadline_selector = CSSSelector("article > div > h2, article > div > h3")
         _paragraph_selector = XPath(
             """
-            //article 
-            //div[contains(@class, 'article-body')] 
-            //p[
-                not(
-                    ancestor::*[@class='bi-bulletpoints'] or
-                    mark[@class='has-inline-color has-cyan-bluish-gray-color'] or 
-                    @class='has-text-align-right'
-                )
-            ]
+            //article
+            //div[
+                contains(@class, 'article-body') 
+                or contains(@class, 'piano-article')]
+            /p[
+                not(ancestor::*[@class='bi-bulletpoints']
+                    or mark[@class='has-inline-color has-cyan-bluish-gray-color']
+                    or @class='has-text-align-right')]
             """
         )
 
         @attribute
         def body(self) -> ArticleBody:
             return extract_article_body_with_selector(
                 self.precomputed.doc,
@@ -47,14 +45,14 @@
 
         @attribute
         def publishing_date(self) -> Optional[datetime.datetime]:
             return generic_date_parsing(self.precomputed.ld.bf_search("datePublished"))
 
         @attribute
         def title(self) -> Optional[str]:
-            return self.precomputed.ld.bf_search("headline")
+            return self.precomputed.meta.get("og:title")
 
         @attribute
         def topics(self) -> List[str]:
             return generic_topic_parsing(self.precomputed.meta.get("keywords")) or generic_topic_parsing(
                 self.precomputed.ld.bf_search("keywords")
             )
```

### Comparing `fundus-0.2.2/src/fundus/publishers/de/die_welt.py` & `fundus-0.3.0/src/fundus/publishers/de/die_welt.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/de/die_zeit.py` & `fundus-0.3.0/src/fundus/publishers/de/die_zeit.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/de/dw.py` & `fundus-0.3.0/src/fundus/publishers/de/dw.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/de/faz.py` & `fundus-0.3.0/src/fundus/publishers/lt/lrt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 import datetime
 from typing import List, Optional
 
 from lxml.cssselect import CSSSelector
+from lxml.etree import XPath
 
 from fundus.parser import ArticleBody, BaseParser, ParserProxy, attribute
 from fundus.parser.utility import (
     extract_article_body_with_selector,
+    generic_author_parsing,
     generic_date_parsing,
     generic_topic_parsing,
 )
 
 
-class FAZParser(ParserProxy):
+class LRTParser(ParserProxy):
     class V1(BaseParser):
-        _paragraph_selector = CSSSelector("div.atc-Text > p")
-        _summary_selector = CSSSelector("div.atc-Intro > p")
-        _subheadline_selector = CSSSelector("div.atc-Text > h3")
-        _author_selector = CSSSelector(".atc-MetaAuthor")
+        _paragraph_selector = XPath(
+            "//div[@class='article-content js-text-selection']/"
+            "p[not((strong and not(text())) or @class='text-lead')]"
+        )
+        _summary_selector = CSSSelector("p.text-lead")
+        _subheadline_selector = XPath(
+            "//div[@class='article-content js-text-selection']/" "p[strong and not(@class='text-lead') and not(text())]"
+        )
 
         @attribute
         def body(self) -> ArticleBody:
             return extract_article_body_with_selector(
                 self.precomputed.doc,
                 summary_selector=self._summary_selector,
                 subheadline_selector=self._subheadline_selector,
                 paragraph_selector=self._paragraph_selector,
             )
 
         @attribute
-        def topics(self) -> List[str]:
-            return generic_topic_parsing(self.precomputed.meta.get("keywords"))
+        def authors(self) -> List[str]:
+            return generic_author_parsing(self.precomputed.meta.get("lrt_authors"))
 
         @attribute
         def publishing_date(self) -> Optional[datetime.datetime]:
             return generic_date_parsing(self.precomputed.ld.bf_search("datePublished"))
 
         @attribute
-        def authors(self) -> List[str]:
-            # Unfortunately, the raw data may contain cities. Most of these methods aims to remove the cities heuristically.
-            if not (author_nodes := self._author_selector(self.precomputed.doc)):
-                return []
-            else:
-                if len(author_nodes) > 1:
-                    # With more than one entry, we abuse the fact that authors are linked with an <a> tag,
-                    # but cities are not
-                    author_nodes = [node for node in author_nodes if next(node.iterchildren(tag="a"), None) is not None]
-                return [text for node in author_nodes if "F.A.Z" not in (text := node.text_content())]
-
-        @attribute
         def title(self) -> Optional[str]:
             return self.precomputed.meta.get("og:title")
+
+        @attribute
+        def topics(self) -> List[str]:
+            return generic_topic_parsing(self.precomputed.ld.bf_search("keywords"))
```

### Comparing `fundus-0.2.2/src/fundus/publishers/de/focus.py` & `fundus-0.3.0/src/fundus/publishers/de/focus.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/de/mdr.py` & `fundus-0.3.0/src/fundus/publishers/de/mdr.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/de/merkur.py` & `fundus-0.3.0/src/fundus/publishers/de/merkur.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/de/ndr.py` & `fundus-0.3.0/src/fundus/publishers/de/ndr.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/de/ntv.py` & `fundus-0.3.0/src/fundus/publishers/de/ntv.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/de/spon.py` & `fundus-0.3.0/src/fundus/publishers/de/spon.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/de/stern.py` & `fundus-0.3.0/src/fundus/publishers/de/stern.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/de/sz.py` & `fundus-0.3.0/src/fundus/publishers/de/sz.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/de/tagesschau.py` & `fundus-0.3.0/src/fundus/publishers/de/tagesschau.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/de/taz.py` & `fundus-0.3.0/src/fundus/publishers/de/taz.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/de/waz.py` & `fundus-0.3.0/src/fundus/publishers/us/la_times.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,43 +4,36 @@
 from lxml.cssselect import CSSSelector
 
 from fundus.parser import ArticleBody, BaseParser, ParserProxy, attribute
 from fundus.parser.utility import (
     extract_article_body_with_selector,
     generic_author_parsing,
     generic_date_parsing,
-    generic_topic_parsing,
 )
 
 
-class WAZParser(ParserProxy):
+class LATimesParser(ParserProxy):
     class V1(BaseParser):
-        _paragraph_selector = CSSSelector(".article__body > p")
-        _summary_selector = CSSSelector(".article__header__intro__text")
-        _subheadline_selector = CSSSelector(".article__body > h3")
+        _subheadline_selector = CSSSelector(
+            "div[data-element*=story-body] h3[class*=story-title], div[data-element*=story-body] h2[class=subhead]"
+        )
+        _paragraph_selector = CSSSelector("div[data-element*=story-body] > p")
 
         @attribute
         def body(self) -> ArticleBody:
             return extract_article_body_with_selector(
                 self.precomputed.doc,
-                summary_selector=self._summary_selector,
-                subheadline_selector=self._subheadline_selector,
                 paragraph_selector=self._paragraph_selector,
+                subheadline_selector=self._subheadline_selector,
             )
 
         @attribute
-        def title(self) -> Optional[str]:
-            return self.precomputed.meta.get("og:title")
+        def publishing_date(self) -> Optional[datetime.datetime]:
+            return generic_date_parsing(self.precomputed.ld.bf_search("datePublished"))
 
         @attribute
         def authors(self) -> List[str]:
-            return generic_author_parsing(self.precomputed.meta.get("author"))
+            return generic_author_parsing(self.precomputed.ld.bf_search("author"))
 
         @attribute
-        def publishing_date(self) -> Optional[datetime.datetime]:
-            return generic_date_parsing(self.precomputed.ld.bf_search("datePublished"))
-
-        @attribute
-        def topics(self) -> List[str]:
-            authors = generic_author_parsing(self.precomputed.meta.get("author"))
-            topics = generic_topic_parsing(self.precomputed.meta.get("keywords"))
-            return [topic for topic in topics if topic not in authors]
+        def title(self) -> Optional[str]:
+            return self.precomputed.meta.get("og:title")
```

### Comparing `fundus-0.2.2/src/fundus/publishers/fr/le_monde.py` & `fundus-0.3.0/src/fundus/publishers/fr/le_monde.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from lxml.etree import XPath
 
 from fundus.parser import ArticleBody, BaseParser, ParserProxy, attribute
 from fundus.parser.utility import (
     extract_article_body_with_selector,
     generic_author_parsing,
     generic_date_parsing,
-    generic_topic_parsing,
 )
 
 
 class LeMondeParser(ParserProxy):
     class V1(BaseParser):
         _paragraph_selector: CSSSelector = CSSSelector("p[class='article__paragraph ']")
         _summary_selector: XPath = XPath("//p[contains(@class, 'article__desc') or @id='js-summary-live']")
```

### Comparing `fundus-0.2.2/src/fundus/publishers/na/__init__.py` & `fundus-0.3.0/src/fundus/publishers/ch/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from fundus.publishers.base_objects import PublisherEnum, PublisherSpec
-from fundus.scraping.filter import inverse, regex_filter
-from fundus.scraping.html import RSSFeed, Sitemap
+from fundus.scraping.url import NewsMap, RSSFeed, Sitemap
 
-from .the_namibian import TheNamibianParser
+from .srf import SRFParser
 
+# noinspection PyPep8Naming
 
-class NA(PublisherEnum):
-    TheNamibian = PublisherSpec(
-        name="The Namibian",
-        domain="https://www.namibian.com.na/",
+
+class CH(PublisherEnum):
+    SRF = PublisherSpec(
+        name="Schweizer Radio und Fernsehen",
+        domain="https://www.srf.ch/",
         sources=[
-            RSSFeed("https://www.namibian.com.na/feed/"),
-            Sitemap(
-                "https://namibian.com.na/sitemap_index.xml",
-                sitemap_filter=inverse(regex_filter("post-sitemap")),
-                reverse=True,
-            ),
+            RSSFeed("https://www.srf.ch/news/bnf/rss/1646"),
+            NewsMap("https://www.srf.ch/sitemaps/newsmap/news/index.xml"),
+            Sitemap("https://www.srf.ch/new-news-sitemap"),
         ],
-        parser=TheNamibianParser,
+        parser=SRFParser,
     )
```

### Comparing `fundus-0.2.2/src/fundus/publishers/na/the_namibian.py` & `fundus-0.3.0/src/fundus/publishers/na/the_namibian.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import re
 from datetime import datetime
 from typing import List, Optional, Pattern
 
-from lxml.cssselect import CSSSelector
 from lxml.etree import XPath
 
 from fundus.parser import ArticleBody, BaseParser, ParserProxy, attribute
 from fundus.parser.utility import (
     extract_article_body_with_selector,
     generic_author_parsing,
     generic_date_parsing,
```

### Comparing `fundus-0.2.2/src/fundus/publishers/uk/__init__.py` & `fundus-0.3.0/src/fundus/publishers/uk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import date
 
 from fundus.publishers.base_objects import PublisherEnum, PublisherSpec
 from fundus.scraping.filter import inverse, regex_filter
-from fundus.scraping.html import NewsMap, Sitemap
+from fundus.scraping.url import NewsMap, Sitemap
 
 from .i_news import INewsParser
 from .the_guardian import TheGuardianParser
 from .the_independent import TheIndependentParser
 from .the_telegraph import TheTelegraphParser
```

### Comparing `fundus-0.2.2/src/fundus/publishers/uk/i_news.py` & `fundus-0.3.0/src/fundus/publishers/uk/i_news.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/uk/the_guardian.py` & `fundus-0.3.0/src/fundus/publishers/uk/the_guardian.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/uk/the_independent.py` & `fundus-0.3.0/src/fundus/publishers/uk/the_independent.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/uk/the_telegraph.py` & `fundus-0.3.0/src/fundus/publishers/uk/the_telegraph.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/us/__init__.py` & `fundus-0.3.0/src/fundus/publishers/us/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from fundus.publishers.base_objects import PublisherEnum, PublisherSpec
 from fundus.scraping.filter import inverse, regex_filter
-from fundus.scraping.html import NewsMap, RSSFeed, Sitemap
+from fundus.scraping.url import NewsMap, RSSFeed, Sitemap
 
 from .ap_news import APNewsParser
+from .business_insider import BusinessInsiderParser
 from .cnbc import CNBCParser
 from .fox_news import FoxNewsParser
 from .free_beacon import FreeBeaconParser
 from .la_times import LATimesParser
 from .occupy_democrats import OccupyDemocratsParser
 from .reuters import ReutersParser
 from .the_gateway_pundit import TheGatewayPunditParser
@@ -16,15 +17,15 @@
 from .washington_times_parser import WashingtonTimesParser
 from .world_truth import WorldTruthParser
 
 
 class US(PublisherEnum):
     APNews = PublisherSpec(
         name="Associated Press News",
-        domain="https://www.apnews.com/",
+        domain="https://apnews.com/",
         sources=[
             Sitemap(
                 "https://apnews.com/sitemap.xml",
                 sitemap_filter=regex_filter("apnews.com/hub/|apnews.com/video/"),
                 reverse=True,
             ),
             NewsMap("https://apnews.com/news-sitemap-content.xml"),
@@ -37,15 +38,15 @@
         domain="https://www.cnbc.com/",
         sources=[Sitemap("https://www.cnbc.com/sitemapAll.xml"), NewsMap("https://www.cnbc.com/sitemap_news.xml")],
         parser=CNBCParser,
     )
 
     TheIntercept = PublisherSpec(
         name="The Intercept",
-        domain="https://www.theintercept.com/",
+        domain="https://theintercept.com/",
         sources=[
             RSSFeed("https://theintercept.com/feed/?lang=en"),
             Sitemap(
                 "https://theintercept.com/sitemap_index.xml",
                 reverse=True,
                 sitemap_filter=inverse(regex_filter("post-sitemap")),
             ),
@@ -96,15 +97,15 @@
     #     domain="https://www.worldtruth.tv/",
     #     sources=[RSSFeed("https://feeds.feedburner.com/ConsciousnessTv")],
     #     parser=WorldTruthParser,
     # )
 
     FreeBeacon = PublisherSpec(
         name="The Washington Free Beacon",
-        domain="https://www.freebeacon.com/",
+        domain="https://freebeacon.com/",
         sources=[NewsMap("https://freebeacon.com/post_google_news.xml")],
         parser=FreeBeaconParser,
     )
 
     WashingtonTimes = PublisherSpec(
         name="The Washington Times",
         domain="https://www.washingtontimes.com/",
@@ -149,7 +150,17 @@
 
     LATimes = PublisherSpec(
         name="Los Angeles Times",
         domain="https://www.latimes.com/",
         sources=[Sitemap("https://www.latimes.com/sitemap.xml"), NewsMap("https://www.latimes.com/news-sitemap.xml")],
         parser=LATimesParser,
     )
+
+    BusinessInsider = PublisherSpec(
+        name="Business Insider",
+        domain="https://www.businessinsider.com/",
+        sources=[
+            NewsMap("https://www.businessinsider.com/sitemap/google-news.xml"),
+            Sitemap("https://www.businessinsider.com/sitemap/2024-01.xml"),
+        ],
+        parser=BusinessInsiderParser,
+    )
```

### Comparing `fundus-0.2.2/src/fundus/publishers/us/ap_news.py` & `fundus-0.3.0/src/fundus/publishers/us/ap_news.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/us/cnbc.py` & `fundus-0.3.0/src/fundus/publishers/us/cnbc.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/us/fox_news.py` & `fundus-0.3.0/src/fundus/publishers/us/fox_news.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/us/free_beacon.py` & `fundus-0.3.0/src/fundus/publishers/us/free_beacon.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/us/la_times.py` & `fundus-0.3.0/src/fundus/publishers/us/world_truth.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 import datetime
-from typing import List, Optional
+from typing import Optional
 
 from lxml.cssselect import CSSSelector
 
 from fundus.parser import ArticleBody, BaseParser, ParserProxy, attribute
 from fundus.parser.utility import (
     extract_article_body_with_selector,
-    generic_author_parsing,
     generic_date_parsing,
 )
 
 
-class LATimesParser(ParserProxy):
+class WorldTruthParser(ParserProxy):
     class V1(BaseParser):
-        _subheadline_selector = CSSSelector(
-            "div[data-element*=story-body] h3[class*=story-title], div[data-element*=story-body] h2[class=subhead]"
-        )
-        _paragraph_selector = CSSSelector("div[data-element*=story-body] > p")
+        _paragraph_selector = CSSSelector(".td-post-content > p")
 
         @attribute
         def body(self) -> ArticleBody:
             return extract_article_body_with_selector(
                 self.precomputed.doc,
                 paragraph_selector=self._paragraph_selector,
-                subheadline_selector=self._subheadline_selector,
             )
 
         @attribute
         def publishing_date(self) -> Optional[datetime.datetime]:
-            return generic_date_parsing(self.precomputed.ld.bf_search("datePublished"))
-
-        @attribute
-        def authors(self) -> List[str]:
-            return generic_author_parsing(self.precomputed.ld.bf_search("author"))
+            return generic_date_parsing(self.precomputed.meta.get("article:published_time"))
 
         @attribute
         def title(self) -> Optional[str]:
             return self.precomputed.meta.get("og:title")
```

### Comparing `fundus-0.2.2/src/fundus/publishers/us/occupy_democrats.py` & `fundus-0.3.0/src/fundus/publishers/us/occupy_democrats.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/us/reuters.py` & `fundus-0.3.0/src/fundus/publishers/us/reuters.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/us/the_gateway_pundit.py` & `fundus-0.3.0/src/fundus/publishers/us/the_gateway_pundit.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/us/the_intercept.py` & `fundus-0.3.0/src/fundus/publishers/us/the_intercept.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/us/the_nation_parser.py` & `fundus-0.3.0/src/fundus/publishers/us/the_nation_parser.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/us/the_new_yorker.py` & `fundus-0.3.0/src/fundus/publishers/us/the_new_yorker.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/us/washington_times_parser.py` & `fundus-0.3.0/src/fundus/publishers/us/washington_times_parser.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.2/src/fundus/publishers/us/world_truth.py` & `fundus-0.3.0/src/fundus/publishers/de/rheinische_post.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 import datetime
-from typing import Optional
+from typing import List, Optional
 
 from lxml.cssselect import CSSSelector
 
 from fundus.parser import ArticleBody, BaseParser, ParserProxy, attribute
 from fundus.parser.utility import (
     extract_article_body_with_selector,
+    generic_author_parsing,
     generic_date_parsing,
+    generic_topic_parsing,
 )
 
 
-class WorldTruthParser(ParserProxy):
+class RheinischePostParser(ParserProxy):
     class V1(BaseParser):
-        _paragraph_selector = CSSSelector(".td-post-content > p")
+        _summary_selector = CSSSelector("strong[data-cy='intro']")
+        _paragraph_selector = CSSSelector("div[data-cy='article-content'] p")
+        _subheadline_selector = CSSSelector("div[data-cy='article-content'] h2")
 
         @attribute
         def body(self) -> ArticleBody:
             return extract_article_body_with_selector(
                 self.precomputed.doc,
+                summary_selector=self._summary_selector,
                 paragraph_selector=self._paragraph_selector,
+                subheadline_selector=self._subheadline_selector,
             )
 
         @attribute
+        def authors(self) -> List[str]:
+            return generic_author_parsing(self.precomputed.meta.get("author"))
+
+        @attribute
         def publishing_date(self) -> Optional[datetime.datetime]:
-            return generic_date_parsing(self.precomputed.meta.get("article:published_time"))
+            return generic_date_parsing(self.precomputed.ld.bf_search("datePublished"))
 
         @attribute
         def title(self) -> Optional[str]:
             return self.precomputed.meta.get("og:title")
+
+        @attribute
+        def topics(self) -> List[str]:
+            return generic_topic_parsing(self.precomputed.meta.get("keywords"))
```

### Comparing `fundus-0.2.2/src/fundus/scraping/article.py` & `fundus-0.3.0/src/fundus/scraping/article.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 
 
 @dataclass(frozen=True)
 class Article:
     html: HTML
     exception: Optional[Exception] = None
 
-    # supported attributes as defined in the guidelines
+    # supported (validated) attributes as defined in the guidelines
     title: Optional[str] = None
     authors: List[str] = field(default_factory=list)
     body: Optional[ArticleBody] = None
     publishing_date: Optional[datetime] = None
     topics: List[str] = field(default_factory=list)
+    free_access: bool = True
 
     @classmethod
     def from_extracted(cls, html: HTML, extracted: Dict[str, Any], exception: Optional[Exception] = None) -> "Article":
         validated_attributes: Set[str] = {article_field.name for article_field in fields(cls)}
 
         extracted_unvalidated: Iterator[Tuple[str, Any]]
         extracted_validated: Iterator[Tuple[str, Any]]
@@ -79,12 +80,12 @@
         )
 
         text = (
             f"Fundus-Article:"
             f'\n- Title: "{wrapped_title}"'
             f'\n- Text:  "{wrapped_plaintext}"'
             f"\n- URL:    {self.html.requested_url}"
-            f"\n- From:   {self.html.source.publisher}"
+            f"\n- From:   {self.html.source_info.publisher}"
             f'{" (" + self.publishing_date.strftime("%Y-%m-%d %H:%M") + ")" if self.publishing_date else ""}'
         )
 
         return dedent(text)
```

### Comparing `fundus-0.2.2/src/fundus/scraping/scraper.py` & `fundus-0.3.0/src/fundus/scraping/scraper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,85 +1,99 @@
-from typing import AsyncIterator, Literal, Optional
+from typing import Dict, Iterator, List, Literal, Optional, Type
 
 import more_itertools
 
 from fundus.logging import basic_logger
 from fundus.parser import ParserProxy
+from fundus.publishers.base_objects import PublisherEnum
 from fundus.scraping.article import Article
+from fundus.scraping.delay import Delay
 from fundus.scraping.filter import (
     ExtractionFilter,
     FilterResultWithMissingAttributes,
-    Requires,
     URLFilter,
 )
-from fundus.scraping.html import FundusSource
+from fundus.scraping.html import CCNewsSource, HTMLSource, WebSource
+from fundus.scraping.url import URLSource
 
 
-class Scraper:
-    def __init__(self, *sources: FundusSource, parser: ParserProxy):
-        self.sources = list(sources)
+class BaseScraper:
+    def __init__(self, *sources: HTMLSource, parser_mapping: Dict[str, ParserProxy]):
+        self.sources = sources
+        self.parser_mapping = parser_mapping
 
-        if not parser:
-            raise ValueError(f"the given parser {type(parser).__name__} is empty")
-
-        self.parser = parser
-
-    async def scrape(
+    def scrape(
         self,
         error_handling: Literal["suppress", "catch", "raise"],
         extraction_filter: Optional[ExtractionFilter] = None,
         url_filter: Optional[URLFilter] = None,
-    ) -> AsyncIterator[Optional[Article]]:
-        # TODO: add docstring; especially explain why returned Article is Optional
-        if isinstance(extraction_filter, Requires):
-            supported_attributes = set(
-                more_itertools.flatten(collection.names for collection in self.parser.attribute_mapping.values())
-            )
-            if missing_attributes := extraction_filter.required_attributes - supported_attributes:
-                if len(missing_attributes) == 1:
-                    basic_logger.warning(
-                        f"The required attribute `{missing_attributes}` "
-                        f"is not supported by {type(self.parser).__name__}. Skipping Scraper"
-                    )
-                else:
-                    basic_logger.warning(
-                        f"The required attributes `{', '.join(missing_attributes)}` "
-                        f"are not supported by {type(self.parser).__name__}. Skipping Scraper"
-                    )
-
-                return
-
-        for html_source in self.sources:
-            async for html in html_source.fetch(url_filter=url_filter):
-                if html is None:
-                    yield None
-                    continue
+    ) -> Iterator[Article]:
+        for source in self.sources:
+            for html in source.fetch(url_filter=url_filter):
+                parser = self.parser_mapping[html.source_info.publisher]
+
                 try:
-                    extraction = self.parser(html.crawl_date).parse(html.content, error_handling)
+                    extraction = parser(html.crawl_date).parse(html.content, error_handling)
 
                 except Exception as err:
                     if error_handling == "raise":
                         error_message = f"Run into an error processing article '{html.requested_url}'"
                         basic_logger.error(error_message)
                         err.args = (str(err) + "\n\n" + error_message,)
                         raise err
                     elif error_handling == "catch":
                         yield Article(html=html, exception=err)
-                        continue
                     elif error_handling == "suppress":
                         basic_logger.info(f"Skipped article at '{html.requested_url}' because of: {err!r}")
-                        yield None
                     else:
                         raise ValueError(f"Unknown value '{error_handling}' for parameter <error_handling>'")
 
-                if extraction_filter and (filter_result := extraction_filter(extraction)):
-                    if isinstance(filter_result, FilterResultWithMissingAttributes):
-                        basic_logger.debug(
-                            f"Skipped article at '{html.requested_url}' because attribute(s) "
-                            f"{', '.join(filter_result.missing_attributes)!r} is(are) missing"
-                        )
-                    else:
-                        basic_logger.debug(f"Skipped article at '{html.requested_url}' because of extraction filter")
-                    yield None
                 else:
-                    article = Article.from_extracted(html=html, extracted=extraction)
-                    yield article
+                    if extraction_filter and (filter_result := extraction_filter(extraction)):
+                        if isinstance(filter_result, FilterResultWithMissingAttributes):
+                            basic_logger.debug(
+                                f"Skipped article at '{html.requested_url}' because attribute(s) "
+                                f"{', '.join(filter_result.missing_attributes)!r} is(are) missing"
+                            )
+                        else:
+                            basic_logger.debug(
+                                f"Skipped article at '{html.requested_url}' because of extraction filter"
+                            )
+                    else:
+                        article = Article.from_extracted(html=html, extracted=extraction)
+                        yield article
+
+
+class WebScraper(BaseScraper):
+    def __init__(
+        self,
+        publisher: PublisherEnum,
+        restrict_sources_to: Optional[List[Type[URLSource]]] = None,
+        delay: Optional[Delay] = None,
+    ):
+        if restrict_sources_to:
+            url_sources = tuple(
+                more_itertools.flatten(publisher.source_mapping[source_type] for source_type in restrict_sources_to)
+            )
+        else:
+            url_sources = tuple(more_itertools.flatten(publisher.source_mapping.values()))
+
+        html_sources = [
+            WebSource(
+                url_source=url_source,
+                publisher=publisher.publisher_name,
+                request_header=publisher.request_header,
+                delay=delay,
+                query_parameters=publisher.query_parameter,
+            )
+            for url_source in url_sources
+        ]
+        parser_mapping: Dict[str, ParserProxy] = {publisher.publisher_name: publisher.parser}
+        super().__init__(*html_sources, parser_mapping=parser_mapping)
+
+
+class CCNewsScraper(BaseScraper):
+    def __init__(self, source: CCNewsSource):
+        parser_mapping: Dict[str, ParserProxy] = {
+            publisher.publisher_name: publisher.parser for publisher in source.publishers
+        }
+        super().__init__(source, parser_mapping=parser_mapping)
```

### Comparing `fundus-0.2.2/src/fundus.egg-info/PKG-INFO` & `fundus-0.3.0/src/fundus.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fundus
-Version: 0.2.2
+Version: 0.3.0
 Summary: A very simple news crawler
 Author-email: Max Dallabetta <max.dallabetta@googlemail.com>
 License: MIT
 Project-URL: Repository, https://github.com/flairNLP/fundus
 Keywords: web scraping, web crawling
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,27 +17,25 @@
 License-File: LICENSE
 Requires-Dist: python-dateutil<3,>=2.8
 Requires-Dist: lxml<5,>=4.9
 Requires-Dist: more-itertools<10,>=9.1
 Requires-Dist: cssselect<2,>=1.1
 Requires-Dist: feedparser<7,>=6.0
 Requires-Dist: colorama<1,>=0.4
-Requires-Dist: typing-extensions<5,>=4.0
+Requires-Dist: typing-extensions<5,>=4.6
 Requires-Dist: langdetect<2,>=1.0
-Requires-Dist: aiohttp<4,>=3.8
-Requires-Dist: aioitertools<1,>=0.11
 Requires-Dist: validators!=0.23,<1,>=0.20
 Requires-Dist: requests<3,>=2.28
 Requires-Dist: tqdm<5,>=4.66
 Requires-Dist: fastwarc<1,>=0.14
 Requires-Dist: chardet<6,>=5.2
 Requires-Dist: dill<1,>=0.3
 Provides-Extra: dev
 Requires-Dist: pytest~=7.2.2; extra == "dev"
-Requires-Dist: mypy==1.1.1; extra == "dev"
+Requires-Dist: mypy==1.9.0; extra == "dev"
 Requires-Dist: isort==5.12.0; extra == "dev"
 Requires-Dist: black==23.1.0; extra == "dev"
 Requires-Dist: types-lxml; extra == "dev"
 Requires-Dist: types-python-dateutil<3,>=2.8; extra == "dev"
 Requires-Dist: types-requests<3,>=2.28; extra == "dev"
 Requires-Dist: types-colorama<1,>=0.4; extra == "dev"
 
@@ -49,23 +47,23 @@
   </picture>
 </p>
 
 <p align="center">A very simple <b>news crawler</b> in Python.
 Developed at <a href="https://www.informatik.hu-berlin.de/en/forschung-en/gebiete/ml-en/">Humboldt University of Berlin</a>.
 </p>
 <p align="center">
-<img alt="version" src="https://img.shields.io/badge/version-0.1-green">
+<a href="https://pypi.org/project/fundus/"><img alt="PyPi version" src="https://badge.fury.io/py/fundus.svg"></a>
 <img alt="python" src="https://img.shields.io/badge/python-3.8-blue">
 <img alt="Static Badge" src="https://img.shields.io/badge/license-MIT-green">
 <img alt="Publisher Coverage" src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/dobbersc/ca0ae056b05cbfeaf30fa42f84ddf458/raw/fundus_publisher_coverage.json">
 </p>
 <div align="center">
 <hr>
 
-[Quick Start](#quick-start) |  [Tutorials](#tutorials)  | [News Sources](/docs/supported_publishers.md)
+[Quick Start](#quick-start) | [Tutorials](#tutorials) | [News Sources](/docs/supported_publishers.md) | [Paper](https://arxiv.org/abs/2403.15279)
 
 </div>
 
 
 ---
 
 Fundus is:
@@ -138,16 +136,16 @@
 ## Example 2: Crawl a specific news source
 
 Maybe you want to crawl a specific news source instead. Let's crawl news articles from Washington Times only:
 
 ```python
 from fundus import PublisherCollection, Crawler
 
-# initialize the crawler for Washington Times
-crawler = Crawler(PublisherCollection.us.WashingtonTimes)
+# initialize the crawler for The New Yorker
+crawler = Crawler(PublisherCollection.us.TheNewYorker)
 
 # crawl 2 articles and print
 for article in crawler.crawl(max_articles=2):
     print(article)
 ```
 
 ## Example 3: Crawl articles from CC-NEWS
@@ -182,14 +180,43 @@
 
 ## Currently Supported News Sources
 
 You can find the publishers currently supported [**here**](/docs/supported_publishers.md).
 
 Also: **Adding a new publisher is easy - consider contributing to the project!**
 
+## Evaluation benchmark
+
+Check out our evaluation [benchmark](https://github.com/dobbersc/fundus-evaluation).
+
+| **Scraper** | **Precision**             | **Recall**                | **F1-Score**              |
+|-------------|---------------------------|---------------------------|---------------------------|
+| [Fundus](https://github.com/flairNLP/fundus)      | **99.89**<sub>±0.57</sub> | 96.75<sub>±12.75</sub>    | **97.69**<sub>±9.75</sub> |
+| [Trafilatura](https://github.com/adbar/trafilatura) | 90.54<sub>±18.86</sub>    | 93.23<sub>±23.81</sub>    | 89.81<sub>±23.69</sub>    |
+| [BTE](https://github.com/dobbersc/fundus-evaluation/blob/master/src/fundus_evaluation/scrapers/bte.py)         | 81.09<sub>±19.41</sub>    | **98.23**<sub>±8.61</sub> | 87.14<sub>±15.48</sub>    |
+| [jusText](https://github.com/miso-belica/jusText)     | 86.51<sub>±18.92</sub>    | 90.23<sub>±20.61</sub>    | 86.96<sub>±19.76</sub>    |
+| [news-please](https://github.com/fhamborg/news-please) | 92.26<sub>±12.40</sub>    | 86.38<sub>±27.59</sub>    | 85.81<sub>±23.29</sub>    |
+| [BoilerNet](https://github.com/dobbersc/fundus-evaluation/tree/master/src/fundus_evaluation/scrapers/boilernet)   | 84.73<sub>±20.82</sub>    | 90.66<sub>±21.05</sub>    | 85.77<sub>±20.28</sub>    |
+| [Boilerpipe](https://github.com/kohlschutter/boilerpipe)  | 82.89<sub>±20.65</sub>    | 82.11<sub>±29.99</sub>    | 79.90<sub>±25.86</sub>    |
+
+## Cite
+
+Please cite the following [paper](https://arxiv.org/abs/2403.15279) when using Fundus or building upon our work:
+
+```bibtex
+@misc{dallabetta2024fundus,
+      title={Fundus: A Simple-to-Use News Scraper Optimized for High Quality Extractions}, 
+      author={Max Dallabetta and Conrad Dobberstein and Adrian Breiding and Alan Akbik},
+      year={2024},
+      eprint={2403.15279},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
+```
+
 ## Contact
 
 Please email your questions or comments to [**Max Dallabetta**](mailto:max.dallabetta@googlemail.com?subject=[GitHub]%20Fundus)
 
 ## Contributing
 
 Thanks for your interest in contributing! There are many ways to get involved;
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,36 +1,35 @@
-Metadata-Version: 2.1 Name: fundus Version: 0.2.2 Summary: A very simple news
+Metadata-Version: 2.1 Name: fundus Version: 0.3.0 Summary: A very simple news
 crawler Author-email: Max Dallabetta
 googlemail.com> License: MIT Project-URL: Repository, https://github.com/
 flairNLP/fundus Keywords: web scraping, web crawling Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: python-dateutil<3,>=2.8
 Requires-Dist: lxml<5,>=4.9 Requires-Dist: more-itertools<10,>=9.1 Requires-
 Dist: cssselect<2,>=1.1 Requires-Dist: feedparser<7,>=6.0 Requires-Dist:
-colorama<1,>=0.4 Requires-Dist: typing-extensions<5,>=4.0 Requires-Dist:
-langdetect<2,>=1.0 Requires-Dist: aiohttp<4,>=3.8 Requires-Dist:
-aioitertools<1,>=0.11 Requires-Dist: validators!=0.23,<1,>=0.20 Requires-Dist:
+colorama<1,>=0.4 Requires-Dist: typing-extensions<5,>=4.6 Requires-Dist:
+langdetect<2,>=1.0 Requires-Dist: validators!=0.23,<1,>=0.20 Requires-Dist:
 requests<3,>=2.28 Requires-Dist: tqdm<5,>=4.66 Requires-Dist: fastwarc<1,>=0.14
 Requires-Dist: chardet<6,>=5.2 Requires-Dist: dill<1,>=0.3 Provides-Extra: dev
-Requires-Dist: pytest~=7.2.2; extra == "dev" Requires-Dist: mypy==1.1.1; extra
+Requires-Dist: pytest~=7.2.2; extra == "dev" Requires-Dist: mypy==1.9.0; extra
 == "dev" Requires-Dist: isort==5.12.0; extra == "dev" Requires-Dist:
 black==23.1.0; extra == "dev" Requires-Dist: types-lxml; extra == "dev"
 Requires-Dist: types-python-dateutil<3,>=2.8; extra == "dev" Requires-Dist:
 types-requests<3,>=2.28; extra == "dev" Requires-Dist: types-colorama<1,>=0.4;
 extra == "dev"
                                     [Logo]
    A very simple nneewwss ccrraawwlleerr in Python. Developed at _H_u_m_b_o_l_d_t_ _U_n_i_v_e_r_s_i_t_y_ _o_f
                                     _B_e_r_l_i_n.
-              [version][python][Static Badge][Publisher Coverage]
+           _[_P_y_P_i_ _v_e_r_s_i_o_n_][python][Static Badge][Publisher Coverage]
 ===============================================================================
  [Quick Start](#quick-start) | [Tutorials](#tutorials) | [News Sources](/docs/
-                           supported_publishers.md)
+     supported_publishers.md) | [Paper](https://arxiv.org/abs/2403.15279)
 --- Fundus is: * **A static news crawler.** Fundus lets you crawl online news
 articles with only a few lines of Python code! Be it from live websites or the
 CC-NEWS dataset. * **An open-source Python package.** Fundus is built on the
 idea of building something together. We welcome your contribution to help
 Fundus [grow](docs/how_to_contribute.md)!
 ===============================================================================
 ## Quick Start To install from pip, simply do: ``` pip install fundus ```
@@ -54,17 +53,17 @@
 funding-poster-critical-lgbtq-community - From: FoxNews (2023-05-09 14:37) ```
 This printout tells you that you successfully crawled two articles! For each
 article, the printout details: - the "Title" of the article, i.e. its headline
 - the "Text", i.e. the main article body text - the "URL" from which it was
 crawled - the news source it is "From" ## Example 2: Crawl a specific news
 source Maybe you want to crawl a specific news source instead. Let's crawl news
 articles from Washington Times only: ```python from fundus import
-PublisherCollection, Crawler # initialize the crawler for Washington Times
-crawler = Crawler(PublisherCollection.us.WashingtonTimes) # crawl 2 articles
-and print for article in crawler.crawl(max_articles=2): print(article) ``` ##
+PublisherCollection, Crawler # initialize the crawler for The New Yorker
+crawler = Crawler(PublisherCollection.us.TheNewYorker) # crawl 2 articles and
+print for article in crawler.crawl(max_articles=2): print(article) ``` ##
 Example 3: Crawl articles from CC-NEWS If you're not familiar with CC-NEWS,
 check out their [paper](https://paperswithcode.com/dataset/cc-news). ````python
 from fundus import PublisherCollection, CCNewsCrawler # initialize the crawler
 for news publishers based in the US crawler = CCNewsCrawler
 (*PublisherCollection.us) # crawl 2 articles and print for article in
 crawler.crawl(max_articles=2): print(article) ```` ## Tutorials We provide
 **quick tutorials** to get you started with the library: 1. [**Tutorial 1: How
@@ -74,13 +73,33 @@
 filter articles**](docs/4_how_to_filter_articles.md) 5. [**Tutorial 5: How to
 search for publishers**](docs/5_how_to_search_for_publishers.md) If you wish to
 contribute check out these tutorials: 1. [**How to contribute**](docs/
 how_to_contribute.md) 2. [**How to add a publisher**](docs/
 how_to_add_a_publisher.md) ## Currently Supported News Sources You can find the
 publishers currently supported [**here**](/docs/supported_publishers.md). Also:
 **Adding a new publisher is easy - consider contributing to the project!** ##
+Evaluation benchmark Check out our evaluation [benchmark](https://github.com/
+dobbersc/fundus-evaluation). | **Scraper** | **Precision** | **Recall** | **F1-
+Score** | |-------------|---------------------------|--------------------------
+-|---------------------------| | [Fundus](https://github.com/flairNLP/fundus) |
+**99.89**Â±0.57 | 96.75Â±12.75 | **97.69**Â±9.75 | | [Trafilatura](https://
+github.com/adbar/trafilatura) | 90.54Â±18.86 | 93.23Â±23.81 | 89.81Â±23.69 | |
+[BTE](https://github.com/dobbersc/fundus-evaluation/blob/master/src/
+fundus_evaluation/scrapers/bte.py) | 81.09Â±19.41 | **98.23**Â±8.61 |
+87.14Â±15.48 | | [jusText](https://github.com/miso-belica/jusText) |
+86.51Â±18.92 | 90.23Â±20.61 | 86.96Â±19.76 | | [news-please](https://
+github.com/fhamborg/news-please) | 92.26Â±12.40 | 86.38Â±27.59 | 85.81Â±23.29 |
+| [BoilerNet](https://github.com/dobbersc/fundus-evaluation/tree/master/src/
+fundus_evaluation/scrapers/boilernet) | 84.73Â±20.82 | 90.66Â±21.05 |
+85.77Â±20.28 | | [Boilerpipe](https://github.com/kohlschutter/boilerpipe) |
+82.89Â±20.65 | 82.11Â±29.99 | 79.90Â±25.86 | ## Cite Please cite the following
+[paper](https://arxiv.org/abs/2403.15279) when using Fundus or building upon
+our work: ```bibtex @misc{dallabetta2024fundus, title={Fundus: A Simple-to-Use
+News Scraper Optimized for High Quality Extractions}, author={Max Dallabetta
+and Conrad Dobberstein and Adrian Breiding and Alan Akbik}, year={2024},
+eprint={2403.15279}, archivePrefix={arXiv}, primaryClass={cs.CL} } ``` ##
 Contact Please email your questions or comments to [**Max Dallabetta**](mailto:
 max.dallabetta@googlemail.com?subject=[GitHub]%20Fundus) ## Contributing Thanks
 for your interest in contributing! There are many ways to get involved; start
 with our [contributor guidelines](docs/how_to_contribute.md) and then check
 these [open issues](https://github.com/flairNLP/fundus/issues) for specific
 tasks. ## License [MIT](LICENSE)
```

### Comparing `fundus-0.2.2/src/fundus.egg-info/SOURCES.txt` & `fundus-0.3.0/src/fundus.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -15,66 +15,71 @@
 src/fundus/parser/base_parser.py
 src/fundus/parser/data.py
 src/fundus/parser/utility.py
 src/fundus/publishers/__init__.py
 src/fundus/publishers/base_objects.py
 src/fundus/publishers/at/__init__.py
 src/fundus/publishers/at/orf.py
+src/fundus/publishers/ch/__init__.py
+src/fundus/publishers/ch/srf.py
 src/fundus/publishers/de/__init__.py
 src/fundus/publishers/de/berliner_zeitung.py
 src/fundus/publishers/de/bild.py
 src/fundus/publishers/de/braunschweiger_zeitung.py
-src/fundus/publishers/de/business_insider.py
+src/fundus/publishers/de/business_insider_de.py
 src/fundus/publishers/de/die_welt.py
 src/fundus/publishers/de/die_zeit.py
 src/fundus/publishers/de/dw.py
 src/fundus/publishers/de/faz.py
 src/fundus/publishers/de/focus.py
 src/fundus/publishers/de/mdr.py
 src/fundus/publishers/de/merkur.py
 src/fundus/publishers/de/ndr.py
 src/fundus/publishers/de/ntv.py
+src/fundus/publishers/de/rheinische_post.py
 src/fundus/publishers/de/spon.py
 src/fundus/publishers/de/stern.py
 src/fundus/publishers/de/sz.py
 src/fundus/publishers/de/tagesschau.py
 src/fundus/publishers/de/taz.py
 src/fundus/publishers/de/waz.py
 src/fundus/publishers/fr/__init__.py
 src/fundus/publishers/fr/le_monde.py
+src/fundus/publishers/lt/__init__.py
+src/fundus/publishers/lt/lrt.py
 src/fundus/publishers/na/__init__.py
 src/fundus/publishers/na/the_namibian.py
 src/fundus/publishers/uk/__init__.py
 src/fundus/publishers/uk/i_news.py
 src/fundus/publishers/uk/the_guardian.py
 src/fundus/publishers/uk/the_independent.py
 src/fundus/publishers/uk/the_telegraph.py
 src/fundus/publishers/us/__init__.py
 src/fundus/publishers/us/ap_news.py
+src/fundus/publishers/us/business_insider.py
 src/fundus/publishers/us/cnbc.py
 src/fundus/publishers/us/fox_news.py
 src/fundus/publishers/us/free_beacon.py
 src/fundus/publishers/us/la_times.py
 src/fundus/publishers/us/occupy_democrats.py
 src/fundus/publishers/us/reuters.py
 src/fundus/publishers/us/the_gateway_pundit.py
 src/fundus/publishers/us/the_intercept.py
 src/fundus/publishers/us/the_nation_parser.py
 src/fundus/publishers/us/the_new_yorker.py
 src/fundus/publishers/us/washington_times_parser.py
 src/fundus/publishers/us/world_truth.py
 src/fundus/scraping/__init__.py
 src/fundus/scraping/article.py
+src/fundus/scraping/crawler.py
+src/fundus/scraping/delay.py
 src/fundus/scraping/filter.py
 src/fundus/scraping/html.py
-src/fundus/scraping/pipeline.py
 src/fundus/scraping/scraper.py
-src/fundus/scraping/common_crawl/__init__.py
-src/fundus/scraping/common_crawl/html.py
-src/fundus/scraping/common_crawl/pipeline.py
-src/fundus/scraping/common_crawl/scraper.py
+src/fundus/scraping/session.py
+src/fundus/scraping/url.py
 src/fundus/utils/__init__.py
 src/fundus/utils/iteration.py
-src/fundus/utils/more_async.py
 tests/test_collection.py
-tests/test_parser.py
-tests/test_pipeline.py
+tests/test_crawler.py
+tests/test_filter.py
+tests/test_parser.py
```

### Comparing `fundus-0.2.2/tests/test_collection.py` & `fundus-0.3.0/tests/test_collection.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 class TestCollection:
     def test_iter_empty_collection(self, empty_collection):
         assert list(empty_collection) == []
 
     def test_iter_collection_with_empty_publisher_enum(self, collection_with_empty_publisher_enum):
         assert list(collection_with_empty_publisher_enum) == []
 
-    def test_iter_collection_with_publisher_enum(self, collection_with_validate_publisher_enum):
-        assert list(collection_with_validate_publisher_enum) == [collection_with_validate_publisher_enum.pub.value]
+    def test_iter_collection_with_publisher_enum(self, collection_with_valid_publisher_enum):
+        assert list(collection_with_valid_publisher_enum) == [collection_with_valid_publisher_enum.pub.value]
 
     def test_publisher_enum_with_wrong_enum_value(self):
         with pytest.raises(ValueError):
 
             class PublisherEnumWithWrongValue(PublisherEnum):
                 value = "Enum"
```

### Comparing `fundus-0.2.2/tests/test_parser.py` & `fundus-0.3.0/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
         attrs1, attrs2 = parser_proxy.attribute_mapping.values()
         assert attrs1.names != attrs2.names
 
 
 # enforce test coverage for test parsing
 # because this is also used for the generate_parser_test_files script we export it here
-attributes_required_to_cover = {"title", "authors", "topics", "publishing_date"}
+attributes_required_to_cover = {"title", "authors", "topics", "publishing_date", "body"}
 
 
 @pytest.mark.parametrize(
     "publisher", list(PublisherCollection), ids=[publisher.name for publisher in PublisherCollection]
 )
 class TestParser:
     def test_annotations(self, publisher: PublisherEnum) -> None:
@@ -163,15 +163,21 @@
                         f"There is no value set for key '{key}' in the test JSON. "
                         f"Only complete articles should be used as test cases"
                     )
 
             # test coverage
             supported_attrs = set(versioned_parser.attributes().names)
             missing_attrs = attributes_required_to_cover & supported_attrs - set(version_data.keys())
-            assert not missing_attrs, f"Test JSON does not cover the following attribute(s): {missing_attrs}"
+            assert (
+                not missing_attrs
+            ), f"Test JSON for {version_name} does not cover the following attribute(s): {missing_attrs}"
+
+            assert list(version_data.keys()) == sorted(
+                attributes_required_to_cover & supported_attrs
+            ), f"Test JSON for {version_name} is not in alphabetical order"
 
             assert (html := html_mapping.get(versioned_parser)), f"Missing test HTML for parser version {version_name}"
             # compare data
             extraction = versioned_parser().parse(html.content, "raise")
             for key, value in version_data.items():
                 assert value == extraction[key]
```

### Comparing `fundus-0.2.2/tests/test_pipeline.py` & `fundus-0.3.0/tests/test_crawler.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,38 +2,50 @@
 
 from fundus import Crawler, NewsMap, RSSFeed
 
 
 class TestPipeline:
     def test_crawler_with_empty_collection(self, collection_with_empty_publisher_enum):
         crawler = Crawler(collection_with_empty_publisher_enum)
-        assert crawler.scrapers == tuple()
+        assert crawler.publishers == list()
         assert next(crawler.crawl(), None) is None
 
         with pytest.raises(ValueError):
             Crawler(*collection_with_empty_publisher_enum)
 
-    def test_crawler_with_collection(self, collection_with_validate_publisher_enum):
-        crawler = Crawler(*collection_with_validate_publisher_enum)
-        publisher = collection_with_validate_publisher_enum.pub.value
-        print(crawler.scrapers)
-        assert len(crawler.scrapers) == 1
-        assert len(crawler.scrapers[0].sources) == len(
-            list(value for value in publisher.source_mapping.values() if value)
-        )
+    def test_crawler_with_collection(self, collection_with_valid_publisher_enum):
+        crawler = Crawler(*collection_with_valid_publisher_enum)
+        publisher = collection_with_valid_publisher_enum.pub.value
+        assert len(crawler.publishers) == 1
+
+    def test_crawler_with_two_collections(
+        self,
+        collection_with_valid_publisher_enum,
+        collection_with_empty_publisher_enum,
+        collection_with_two_valid_publisher_enum,
+    ):
+        crawler = Crawler(collection_with_empty_publisher_enum, collection_with_valid_publisher_enum)
+        assert len(crawler.publishers) == 1
+
+        crawler = Crawler(collection_with_valid_publisher_enum, collection_with_valid_publisher_enum)
+        assert len(crawler.publishers) == 1
+
+        crawler = Crawler(collection_with_two_valid_publisher_enum)
+        assert len(crawler.publishers) == 2
+
+        crawler = Crawler(collection_with_valid_publisher_enum, collection_with_two_valid_publisher_enum)
+        assert len(crawler.publishers) == 3
 
     def test_crawler_with_publisher_enum(self, publisher_enum_with_rss_feeds, publisher_enum_with_news_map):
         crawler = Crawler(publisher_enum_with_rss_feeds, publisher_enum_with_news_map)
-        assert len(crawler.scrapers) == 2
+        assert len(crawler.publishers) == 2
 
         crawler = Crawler(publisher_enum_with_rss_feeds, publisher_enum_with_news_map, restrict_sources_to=[RSSFeed])
-        assert len(crawler.scrapers) == 1
-        assert crawler.scrapers[0].sources == publisher_enum_with_rss_feeds.value.source_mapping[RSSFeed]
+        assert len(crawler.publishers) == 2
 
         crawler = Crawler(publisher_enum_with_rss_feeds, publisher_enum_with_news_map, restrict_sources_to=[NewsMap])
-        assert len(crawler.scrapers) == 1
-        assert crawler.scrapers[0].sources == publisher_enum_with_news_map.value.source_mapping[NewsMap]
+        assert len(crawler.publishers) == 2
 
-    def test_consecutive_calls_to_crawl(self, collection_with_validate_publisher_enum):
-        crawler = Crawler(collection_with_validate_publisher_enum)
+    def test_consecutive_calls_to_crawl(self, collection_with_valid_publisher_enum):
+        crawler = Crawler(collection_with_valid_publisher_enum)
         next(crawler.crawl(max_articles=0), None)
         next(crawler.crawl(max_articles=0), None)
```


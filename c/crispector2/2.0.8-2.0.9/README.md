# Comparing `tmp/crispector2-2.0.8.tar.gz` & `tmp/crispector2-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crispector2-2.0.8.tar", last modified: Sun Mar 10 17:18:10 2024, max compression
+gzip compressed data, was "crispector2-2.0.9.tar", last modified: Sun Apr 21 17:02:51 2024, max compression
```

## Comparing `crispector2-2.0.8.tar` & `crispector2-2.0.9.tar`

### file list

```diff
@@ -1,64 +1,59 @@
-drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-03-10 17:18:10.948770 crispector2-2.0.8/
--rw-r--r--   0 guyassa    (501) staff       (20)     5995 2023-08-19 18:51:56.000000 crispector2-2.0.8/LICENSE
--rw-r--r--   0 guyassa    (501) staff       (20)       77 2023-08-22 15:02:32.000000 crispector2-2.0.8/MANIFEST.in
--rw-r--r--   0 guyassa    (501) staff       (20)    21744 2024-03-10 17:18:10.948384 crispector2-2.0.8/PKG-INFO
--rw-r--r--   0 guyassa    (501) staff       (20)    21504 2024-02-19 13:30:56.000000 crispector2-2.0.8/README.md
-drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-03-10 17:18:10.877430 crispector2-2.0.8/crispector2/
--rwxrwxrwx   0 guyassa    (501) staff       (20)      148 2024-03-10 17:16:44.000000 crispector2-2.0.8/crispector2/__init__.py
-drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-03-10 17:18:10.891892 crispector2-2.0.8/crispector2/algorithm/
--rwxrwxrwx   0 guyassa    (501) staff       (20)        0 2021-12-05 10:54:28.000000 crispector2-2.0.8/crispector2/algorithm/__init__.py
--rwxrwxrwx   0 guyassa    (501) staff       (20)     6052 2023-08-21 09:57:02.000000 crispector2-2.0.8/crispector2/algorithm/binomial_probability.py
--rwxrwxrwx   0 guyassa    (501) staff       (20)     7431 2023-08-21 09:57:02.000000 crispector2-2.0.8/crispector2/algorithm/core_algorithm.py
--rwxrwxrwx   0 guyassa    (501) staff       (20)     5549 2024-01-14 10:48:18.000000 crispector2-2.0.8/crispector2/algorithm/translocations.py
--rwxrwxrwx   0 guyassa    (501) staff       (20)     4993 2023-12-26 14:49:45.000000 crispector2-2.0.8/crispector2/algorithm/translocations_original.py
-drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-03-10 17:18:10.900998 crispector2-2.0.8/crispector2/allele/
--rwxrwxrwx   0 guyassa    (501) staff       (20)        0 2021-12-05 10:54:28.000000 crispector2-2.0.8/crispector2/allele/__init__.py
--rw-r--r--   0 guyassa    (501) staff       (20)    41377 2023-08-31 14:10:26.000000 crispector2-2.0.8/crispector2/allele/allele_mock.py
--rw-r--r--   0 guyassa    (501) staff       (20)     3411 2023-08-21 09:57:02.000000 crispector2-2.0.8/crispector2/allele/allele_reference_df.py
--rw-r--r--   0 guyassa    (501) staff       (20)     6977 2024-02-12 09:53:45.000000 crispector2-2.0.8/crispector2/allele/allele_tx.py
--rw-r--r--   0 guyassa    (501) staff       (20)    29329 2024-02-17 10:42:04.000000 crispector2-2.0.8/crispector2/allele/random_reads_handler.py
--rwxrwxrwx   0 guyassa    (501) staff       (20)     7726 2023-08-24 10:30:46.000000 crispector2-2.0.8/crispector2/cli.py
-drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-03-10 17:18:10.903813 crispector2-2.0.8/crispector2/config/
--rwxrwxrwx   0 guyassa    (501) staff       (20)        0 2021-12-05 10:54:28.000000 crispector2-2.0.8/crispector2/config/__init__.py
--rwxrwxrwx   0 guyassa    (501) staff       (20)     7093 2024-02-19 13:30:56.000000 crispector2-2.0.8/crispector2/config/default_config.yml
--rwxr-xr-x   0 guyassa    (501) staff       (20)    33118 2024-02-18 13:48:32.000000 crispector2-2.0.8/crispector2/crispector_main.py
-drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-03-10 17:18:10.910740 crispector2-2.0.8/crispector2/input_processing/
--rwxrwxrwx   0 guyassa    (501) staff       (20)        0 2021-12-05 10:54:28.000000 crispector2-2.0.8/crispector2/input_processing/__init__.py
--rwxrwxrwx   0 guyassa    (501) staff       (20)    35358 2024-02-19 13:30:56.000000 crispector2-2.0.8/crispector2/input_processing/alignment.py
--rw-r--r--   0 guyassa    (501) staff       (20)    31752 2023-08-21 08:59:35.000000 crispector2-2.0.8/crispector2/input_processing/input_processing.py
--rwxrwxrwx   0 guyassa    (501) staff       (20)     7084 2023-08-21 09:57:02.000000 crispector2-2.0.8/crispector2/input_processing/utils.py
-drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-03-10 17:18:10.914179 crispector2-2.0.8/crispector2/modifications/
--rwxrwxrwx   0 guyassa    (501) staff       (20)        0 2021-12-05 10:54:28.000000 crispector2-2.0.8/crispector2/modifications/__init__.py
--rwxrwxrwx   0 guyassa    (501) staff       (20)     7289 2024-02-12 09:55:23.000000 crispector2-2.0.8/crispector2/modifications/modification_tables.py
--rwxrwxrwx   0 guyassa    (501) staff       (20)     4467 2023-08-21 09:57:02.000000 crispector2-2.0.8/crispector2/modifications/modification_types.py
-drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-03-10 17:18:10.917168 crispector2-2.0.8/crispector2/report/
--rwxrwxrwx   0 guyassa    (501) staff       (20)        0 2021-12-05 10:54:28.000000 crispector2-2.0.8/crispector2/report/__init__.py
--rwxrwxrwx   0 guyassa    (501) staff       (20)     4415 2023-08-21 09:57:02.000000 crispector2-2.0.8/crispector2/report/html_report.py
-drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-03-10 17:18:10.937411 crispector2-2.0.8/crispector2/report/html_templates/
--rw-r--r--   0 guyassa    (501) staff       (20)     6148 2024-02-18 13:40:59.000000 crispector2-2.0.8/crispector2/report/html_templates/.DS_Store
--rw-r--r--   0 guyassa    (501) staff       (20)   178836 2024-02-04 15:54:38.000000 crispector2-2.0.8/crispector2/report/html_templates/crispector_logo.jpg
--rw-r--r--   0 guyassa    (501) staff       (20)   178836 2024-02-04 15:54:38.000000 crispector2-2.0.8/crispector2/report/html_templates/crispector_logo.png
--rw-r--r--   0 guyassa    (501) staff       (20)    18706 2024-02-13 12:42:37.000000 crispector2-2.0.8/crispector2/report/html_templates/file_to_render.html
--rwxrwxrwx   0 guyassa    (501) staff       (20)    15092 2021-12-05 10:54:28.000000 crispector2-2.0.8/crispector2/report/html_templates/file_to_render_old.html
--rw-r--r--   0 guyassa    (501) staff       (20)     8257 2024-02-13 12:18:49.000000 crispector2-2.0.8/crispector2/report/html_templates/final_layout.html
--rwxrwxrwx   0 guyassa    (501) staff       (20)     9518 2021-12-05 10:54:28.000000 crispector2-2.0.8/crispector2/report/html_templates/final_layout_old.html
--rwxrwxrwx   0 guyassa    (501) staff       (20)     7803 2021-12-05 10:54:28.000000 crispector2-2.0.8/crispector2/report/html_templates/site_file_to_render.html
--rwxrwxrwx   0 guyassa    (501) staff       (20)    10747 2021-12-05 10:54:28.000000 crispector2-2.0.8/crispector2/report/html_templates/site_layout.html
--rwxr-xr-x   0 guyassa    (501) staff       (20)    62580 2024-02-18 13:40:10.000000 crispector2-2.0.8/crispector2/report/visualization_and_output.py
-drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-03-10 17:18:10.945622 crispector2-2.0.8/crispector2/utils/
--rwxrwxrwx   0 guyassa    (501) staff       (20)        0 2021-12-05 10:54:28.000000 crispector2-2.0.8/crispector2/utils/__init__.py
--rwxrwxrwx   0 guyassa    (501) staff       (20)      884 2023-08-21 09:57:02.000000 crispector2-2.0.8/crispector2/utils/configurator.py
--rwxrwxrwx   0 guyassa    (501) staff       (20)     9855 2024-02-12 11:34:20.000000 crispector2-2.0.8/crispector2/utils/constants_and_types.py
--rwxrwxrwx   0 guyassa    (501) staff       (20)     9654 2023-08-16 13:20:59.000000 crispector2-2.0.8/crispector2/utils/constants_and_types_old.py
--rwxrwxrwx   0 guyassa    (501) staff       (20)     1035 2021-12-05 10:54:28.000000 crispector2-2.0.8/crispector2/utils/exceptions.py
--rwxrwxrwx   0 guyassa    (501) staff       (20)     2176 2023-08-21 09:00:20.000000 crispector2-2.0.8/crispector2/utils/logger.py
-drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-03-10 17:18:10.947180 crispector2-2.0.8/crispector2.egg-info/
--rw-r--r--   0 guyassa    (501) staff       (20)    21744 2024-03-10 17:18:10.000000 crispector2-2.0.8/crispector2.egg-info/PKG-INFO
--rw-r--r--   0 guyassa    (501) staff       (20)     1918 2024-03-10 17:18:10.000000 crispector2-2.0.8/crispector2.egg-info/SOURCES.txt
--rw-r--r--   0 guyassa    (501) staff       (20)        1 2024-03-10 17:18:10.000000 crispector2-2.0.8/crispector2.egg-info/dependency_links.txt
--rw-r--r--   0 guyassa    (501) staff       (20)       52 2024-03-10 17:18:10.000000 crispector2-2.0.8/crispector2.egg-info/entry_points.txt
--rw-r--r--   0 guyassa    (501) staff       (20)        1 2024-03-10 17:18:10.000000 crispector2-2.0.8/crispector2.egg-info/not-zip-safe
--rw-r--r--   0 guyassa    (501) staff       (20)       12 2024-03-10 17:18:10.000000 crispector2-2.0.8/crispector2.egg-info/top_level.txt
--rw-r--r--   0 guyassa    (501) staff       (20)      254 2024-03-10 17:14:59.000000 crispector2-2.0.8/pyproject.toml
--rw-r--r--   0 guyassa    (501) staff       (20)      123 2024-03-10 17:18:10.949801 crispector2-2.0.8/setup.cfg
--rw-r--r--   0 guyassa    (501) staff       (20)     1454 2024-03-10 17:16:32.000000 crispector2-2.0.8/setup.py
+drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-04-21 17:02:51.420855 crispector2-2.0.9/
+-rw-r--r--   0 guyassa    (501) staff       (20)     5995 2023-08-19 18:51:56.000000 crispector2-2.0.9/LICENSE
+-rw-r--r--   0 guyassa    (501) staff       (20)       77 2023-08-22 15:02:32.000000 crispector2-2.0.9/MANIFEST.in
+-rw-r--r--   0 guyassa    (501) staff       (20)    22547 2024-04-21 17:02:51.420250 crispector2-2.0.9/PKG-INFO
+-rw-r--r--   0 guyassa    (501) staff       (20)    21504 2024-03-12 15:19:14.000000 crispector2-2.0.9/README.md
+drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-04-21 17:02:51.359553 crispector2-2.0.9/crispector2/
+-rwxrwxrwx   0 guyassa    (501) staff       (20)      148 2024-04-21 17:02:18.000000 crispector2-2.0.9/crispector2/__init__.py
+drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-04-21 17:02:51.373645 crispector2-2.0.9/crispector2/algorithm/
+-rwxrwxrwx   0 guyassa    (501) staff       (20)        0 2021-12-05 10:54:28.000000 crispector2-2.0.9/crispector2/algorithm/__init__.py
+-rwxrwxrwx   0 guyassa    (501) staff       (20)     6052 2023-08-21 09:57:02.000000 crispector2-2.0.9/crispector2/algorithm/binomial_probability.py
+-rwxrwxrwx   0 guyassa    (501) staff       (20)     7431 2023-08-21 09:57:02.000000 crispector2-2.0.9/crispector2/algorithm/core_algorithm.py
+-rwxrwxrwx   0 guyassa    (501) staff       (20)     5549 2024-01-14 10:48:18.000000 crispector2-2.0.9/crispector2/algorithm/translocations.py
+drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-04-21 17:02:51.382112 crispector2-2.0.9/crispector2/allele/
+-rwxrwxrwx   0 guyassa    (501) staff       (20)        0 2021-12-05 10:54:28.000000 crispector2-2.0.9/crispector2/allele/__init__.py
+-rw-r--r--   0 guyassa    (501) staff       (20)    41377 2023-08-31 14:10:26.000000 crispector2-2.0.9/crispector2/allele/allele_mock.py
+-rw-r--r--   0 guyassa    (501) staff       (20)     3411 2023-08-21 09:57:02.000000 crispector2-2.0.9/crispector2/allele/allele_reference_df.py
+-rw-r--r--   0 guyassa    (501) staff       (20)     6977 2024-02-12 09:53:45.000000 crispector2-2.0.9/crispector2/allele/allele_tx.py
+-rw-r--r--   0 guyassa    (501) staff       (20)    29329 2024-02-17 10:42:04.000000 crispector2-2.0.9/crispector2/allele/random_reads_handler.py
+-rwxrwxrwx   0 guyassa    (501) staff       (20)     7726 2023-08-24 10:30:46.000000 crispector2-2.0.9/crispector2/cli.py
+drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-04-21 17:02:51.384847 crispector2-2.0.9/crispector2/config/
+-rwxrwxrwx   0 guyassa    (501) staff       (20)        0 2021-12-05 10:54:28.000000 crispector2-2.0.9/crispector2/config/__init__.py
+-rwxrwxrwx   0 guyassa    (501) staff       (20)     7093 2024-02-19 13:30:56.000000 crispector2-2.0.9/crispector2/config/default_config.yml
+-rwxr-xr-x   0 guyassa    (501) staff       (20)    33118 2024-02-18 13:48:32.000000 crispector2-2.0.9/crispector2/crispector_main.py
+drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-04-21 17:02:51.391405 crispector2-2.0.9/crispector2/input_processing/
+-rwxrwxrwx   0 guyassa    (501) staff       (20)        0 2021-12-05 10:54:28.000000 crispector2-2.0.9/crispector2/input_processing/__init__.py
+-rwxrwxrwx   0 guyassa    (501) staff       (20)    35358 2024-02-19 13:30:56.000000 crispector2-2.0.9/crispector2/input_processing/alignment.py
+-rw-r--r--   0 guyassa    (501) staff       (20)    31752 2023-08-21 08:59:35.000000 crispector2-2.0.9/crispector2/input_processing/input_processing.py
+-rwxrwxrwx   0 guyassa    (501) staff       (20)     7084 2023-08-21 09:57:02.000000 crispector2-2.0.9/crispector2/input_processing/utils.py
+drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-04-21 17:02:51.393665 crispector2-2.0.9/crispector2/modifications/
+-rwxrwxrwx   0 guyassa    (501) staff       (20)        0 2021-12-05 10:54:28.000000 crispector2-2.0.9/crispector2/modifications/__init__.py
+-rwxrwxrwx   0 guyassa    (501) staff       (20)     7289 2024-02-12 09:55:23.000000 crispector2-2.0.9/crispector2/modifications/modification_tables.py
+-rwxrwxrwx   0 guyassa    (501) staff       (20)     4467 2023-08-21 09:57:02.000000 crispector2-2.0.9/crispector2/modifications/modification_types.py
+drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-04-21 17:02:51.396233 crispector2-2.0.9/crispector2/report/
+-rwxrwxrwx   0 guyassa    (501) staff       (20)        0 2021-12-05 10:54:28.000000 crispector2-2.0.9/crispector2/report/__init__.py
+-rwxrwxrwx   0 guyassa    (501) staff       (20)     4415 2023-08-21 09:57:02.000000 crispector2-2.0.9/crispector2/report/html_report.py
+drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-04-21 17:02:51.413300 crispector2-2.0.9/crispector2/report/html_templates/
+-rw-r--r--   0 guyassa    (501) staff       (20)     6148 2024-03-12 15:20:29.000000 crispector2-2.0.9/crispector2/report/html_templates/.DS_Store
+-rw-r--r--   0 guyassa    (501) staff       (20)   178836 2024-02-04 15:54:38.000000 crispector2-2.0.9/crispector2/report/html_templates/crispector_logo.jpg
+-rw-r--r--   0 guyassa    (501) staff       (20)   178836 2024-02-04 15:54:38.000000 crispector2-2.0.9/crispector2/report/html_templates/crispector_logo.png
+-rw-r--r--   0 guyassa    (501) staff       (20)    18706 2024-02-13 12:42:37.000000 crispector2-2.0.9/crispector2/report/html_templates/file_to_render.html
+-rw-r--r--   0 guyassa    (501) staff       (20)     8257 2024-02-13 12:18:49.000000 crispector2-2.0.9/crispector2/report/html_templates/final_layout.html
+-rwxrwxrwx   0 guyassa    (501) staff       (20)     7803 2021-12-05 10:54:28.000000 crispector2-2.0.9/crispector2/report/html_templates/site_file_to_render.html
+-rwxrwxrwx   0 guyassa    (501) staff       (20)    10747 2021-12-05 10:54:28.000000 crispector2-2.0.9/crispector2/report/html_templates/site_layout.html
+-rwxr-xr-x   0 guyassa    (501) staff       (20)    62580 2024-02-18 13:40:10.000000 crispector2-2.0.9/crispector2/report/visualization_and_output.py
+drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-04-21 17:02:51.417752 crispector2-2.0.9/crispector2/utils/
+-rwxrwxrwx   0 guyassa    (501) staff       (20)        0 2021-12-05 10:54:28.000000 crispector2-2.0.9/crispector2/utils/__init__.py
+-rwxrwxrwx   0 guyassa    (501) staff       (20)      884 2023-08-21 09:57:02.000000 crispector2-2.0.9/crispector2/utils/configurator.py
+-rwxrwxrwx   0 guyassa    (501) staff       (20)     9855 2024-02-12 11:34:20.000000 crispector2-2.0.9/crispector2/utils/constants_and_types.py
+-rwxrwxrwx   0 guyassa    (501) staff       (20)     1035 2021-12-05 10:54:28.000000 crispector2-2.0.9/crispector2/utils/exceptions.py
+-rwxrwxrwx   0 guyassa    (501) staff       (20)     2176 2023-08-21 09:00:20.000000 crispector2-2.0.9/crispector2/utils/logger.py
+drwxr-xr-x   0 guyassa    (501) staff       (20)        0 2024-04-21 17:02:51.419298 crispector2-2.0.9/crispector2.egg-info/
+-rw-r--r--   0 guyassa    (501) staff       (20)    22547 2024-04-21 17:02:51.000000 crispector2-2.0.9/crispector2.egg-info/PKG-INFO
+-rw-r--r--   0 guyassa    (501) staff       (20)     1691 2024-04-21 17:02:51.000000 crispector2-2.0.9/crispector2.egg-info/SOURCES.txt
+-rw-r--r--   0 guyassa    (501) staff       (20)        1 2024-04-21 17:02:51.000000 crispector2-2.0.9/crispector2.egg-info/dependency_links.txt
+-rw-r--r--   0 guyassa    (501) staff       (20)       52 2024-04-21 17:02:51.000000 crispector2-2.0.9/crispector2.egg-info/entry_points.txt
+-rw-r--r--   0 guyassa    (501) staff       (20)      210 2024-04-21 17:02:51.000000 crispector2-2.0.9/crispector2.egg-info/requires.txt
+-rw-r--r--   0 guyassa    (501) staff       (20)       12 2024-04-21 17:02:51.000000 crispector2-2.0.9/crispector2.egg-info/top_level.txt
+-rw-r--r--   0 guyassa    (501) staff       (20)     1098 2024-04-21 17:01:58.000000 crispector2-2.0.9/pyproject.toml
+-rw-r--r--   0 guyassa    (501) staff       (20)       38 2024-04-21 17:02:51.420965 crispector2-2.0.9/setup.cfg
```

### Comparing `crispector2-2.0.8/LICENSE` & `crispector2-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/PKG-INFO` & `crispector2-2.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: crispector2
-Version: 2.0.8
-Home-page: https://github.com/theAguy/crispector2
-Author: Guy Assa
-Author-email: guyassa@gmail.com
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/CRISPECTOR2.0/README.html)
 
 <p align="left">
   <img src="logo.png" alt="Logo" height="100">
 </p>
 #
 CRISPECTOR2.0 is a software package designed to support the detection, evaluation, and quantification of an allele-specific on- and off-target genome editing activity. 
@@ -33,15 +23,15 @@
 </p>
 
 # Installation
 
 CRISPECTOR2.0 can be installed using the [conda](http://conda.pydata.org/docs/intro.html) package manager [Bioconda](https://bioconda.github.io/) (for Linux & macOS), or as a PIP package (for Linux & macOS).
 
 ### Bioconda
-To install CRISPECTOR2.0 using Bioconda, download and install Anaconda Python 3.7, following the instructions at: https://www.anaconda.com/distribution/.
+To install CRISPECTOR2.0 using Bioconda, download and install Anaconda Python 3.8, following the instructions at: https://www.anaconda.com/distribution/.
 
 Open a terminal and type:
 
 ```
 conda config --add channels defaults
 conda config --add channels bioconda
 conda config --add channels conda-forge
@@ -49,18 +39,18 @@
 
 To install CRISPECTOR2.0 into the current conda environment, type:
 
 ```
 conda install crispector2
 ```
 
-If you don't already have an existing environment with Python 3.7, you can create one first (e.g. named `crispector_env`) with:
+If you don't already have an existing environment with Python 3.8, you can create one first (e.g. named `crispector_env`) with:
 
 ```
-conda create -n crispector_env python=3.7
+conda create -n crispector_env python=3.8
 conda activate crispector_env
 conda install crispector2
 ```
 
 Check that CRISPECTOR2.0 is installed using the help command:
 
 ```
```

### Comparing `crispector2-2.0.8/README.md` & `crispector2-2.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,38 @@
+Metadata-Version: 2.1
+Name: crispector2
+Version: 2.0.9
+Summary: CRISPECTOR2 - Genome Editing Analysis Tool, with allele extension
+Author: Guy Assa
+Author-email: guyassa@gmail.com
+Project-URL: repository, https://github.com/theAguy/crispector2
+Keywords: crispector2
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: Click>=7.0
+Requires-Dist: matplotlib>=3.1.2
+Requires-Dist: seaborn>=0.9.0
+Requires-Dist: pyyaml>=5.1.2
+Requires-Dist: plotly>=4.3.0
+Requires-Dist: numpy>=1.12.1
+Requires-Dist: pandas==1.3.5
+Requires-Dist: biopython<=1.79,>=1.74
+Requires-Dist: scipy>=1.2.1
+Requires-Dist: jinja2>=3.1.2
+Requires-Dist: tqdm>=4.66.0
+Requires-Dist: mpmath>=1.3.0
+Requires-Dist: statsmodels>=0.13.2
+Requires-Dist: edlib>=1.3.9
+
 [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/CRISPECTOR2.0/README.html)
 
 <p align="left">
   <img src="logo.png" alt="Logo" height="100">
 </p>
 #
 CRISPECTOR2.0 is a software package designed to support the detection, evaluation, and quantification of an allele-specific on- and off-target genome editing activity. 
@@ -23,15 +54,15 @@
 </p>
 
 # Installation
 
 CRISPECTOR2.0 can be installed using the [conda](http://conda.pydata.org/docs/intro.html) package manager [Bioconda](https://bioconda.github.io/) (for Linux & macOS), or as a PIP package (for Linux & macOS).
 
 ### Bioconda
-To install CRISPECTOR2.0 using Bioconda, download and install Anaconda Python 3.7, following the instructions at: https://www.anaconda.com/distribution/.
+To install CRISPECTOR2.0 using Bioconda, download and install Anaconda Python 3.8, following the instructions at: https://www.anaconda.com/distribution/.
 
 Open a terminal and type:
 
 ```
 conda config --add channels defaults
 conda config --add channels bioconda
 conda config --add channels conda-forge
@@ -39,18 +70,18 @@
 
 To install CRISPECTOR2.0 into the current conda environment, type:
 
 ```
 conda install crispector2
 ```
 
-If you don't already have an existing environment with Python 3.7, you can create one first (e.g. named `crispector_env`) with:
+If you don't already have an existing environment with Python 3.8, you can create one first (e.g. named `crispector_env`) with:
 
 ```
-conda create -n crispector_env python=3.7
+conda create -n crispector_env python=3.8
 conda activate crispector_env
 conda install crispector2
 ```
 
 Check that CRISPECTOR2.0 is installed using the help command:
 
 ```
```

### Comparing `crispector2-2.0.8/crispector2/algorithm/binomial_probability.py` & `crispector2-2.0.9/crispector2/algorithm/binomial_probability.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/algorithm/core_algorithm.py` & `crispector2-2.0.9/crispector2/algorithm/core_algorithm.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/algorithm/translocations.py` & `crispector2-2.0.9/crispector2/algorithm/translocations.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/allele/allele_mock.py` & `crispector2-2.0.9/crispector2/allele/allele_mock.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/allele/allele_reference_df.py` & `crispector2-2.0.9/crispector2/allele/allele_reference_df.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/allele/allele_tx.py` & `crispector2-2.0.9/crispector2/allele/allele_tx.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/allele/random_reads_handler.py` & `crispector2-2.0.9/crispector2/allele/random_reads_handler.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/cli.py` & `crispector2-2.0.9/crispector2/cli.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/config/default_config.yml` & `crispector2-2.0.9/crispector2/config/default_config.yml`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/crispector_main.py` & `crispector2-2.0.9/crispector2/crispector_main.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/input_processing/alignment.py` & `crispector2-2.0.9/crispector2/input_processing/alignment.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/input_processing/input_processing.py` & `crispector2-2.0.9/crispector2/input_processing/input_processing.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/input_processing/utils.py` & `crispector2-2.0.9/crispector2/input_processing/utils.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/modifications/modification_tables.py` & `crispector2-2.0.9/crispector2/modifications/modification_tables.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/modifications/modification_types.py` & `crispector2-2.0.9/crispector2/modifications/modification_types.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/report/html_report.py` & `crispector2-2.0.9/crispector2/report/html_report.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/report/html_templates/.DS_Store` & `crispector2-2.0.9/crispector2/report/html_templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/report/html_templates/crispector_logo.jpg` & `crispector2-2.0.9/crispector2/report/html_templates/crispector_logo.jpg`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/report/html_templates/crispector_logo.png` & `crispector2-2.0.9/crispector2/report/html_templates/crispector_logo.png`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/report/html_templates/file_to_render.html` & `crispector2-2.0.9/crispector2/report/html_templates/file_to_render.html`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/report/html_templates/final_layout.html` & `crispector2-2.0.9/crispector2/report/html_templates/final_layout.html`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/report/html_templates/final_layout_old.html` & `crispector2-2.0.9/crispector2/report/html_templates/site_layout.html`

 * *Files 22% similar despite different names*

```diff
@@ -7,205 +7,219 @@
   <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
   <meta name="description" content="">
   <meta name="author" content="">
 
   <title>Crispector Report</title>
 
   <!--Bootstrap CSS library-->
-  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" 
-    integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T"
-    crossorigin="anonymous">
+  <link rel="stylesheet" href=
+"https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" 
+integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T"
+   crossorigin="anonymous">
 
   <!--jQuery library-->
-  <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" 
-    integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" 
-    crossorigin="anonymous"></script>
+  <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity=
+  "sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" 
+  crossorigin="anonymous"></script>
 
   <!--JS library-->
   <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" 
-    integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" 
-    crossorigin="anonymous"></script>
+  integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" 
+  crossorigin="anonymous"></script>
 
   <!--Latest compiled JavaScript library-->
   <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" 
-    integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM" 
-    crossorigin="anonymous"></script>
+  integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM" 
+  crossorigin="anonymous"></script>
 
   <style>
-    body {
-      font-family: 'Montserrat', sans-serif !important;
-    }
+        body {
+            font-family: 'Montserrat', sans-serif !important;
+        }
   </style>
-
     
-
 </head>
 
 <body>
-
+   
   <!-- Navigation -->
   <nav class="navbar navbar-expand-lg navbar-dark bg-dark static-top">
+    <div class="container">
       <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation">
         <span class="navbar-toggler-icon"></span>
       </button>
       <div class="collapse navbar-collapse" id="navbarResponsive">
         <ul class="navbar-nav mx-auto">
           <li class="nav-item">
-            <a class="nav-link" href="#edit_section">{% block edit_section_title %}{% endblock %}</a>
+            <a class="nav-link" href="#edit_activity">{% block editing_activity_title %}{% endblock %}</a>
           </li>
-          {% block translocations_menu %}{% endblock translocations_menu %}
           <li class="nav-item">
-            <a class="nav-link" href="#Reading_Statistics">{% block reading_stats_title %}{% endblock %}</a>
+            <a class="nav-link" href="#mod_section">{% block modification_section_title %}{% endblock %}</a>
           </li>
           <li class="nav-item">
-            <li class="dropdown">
-              <a class="nav-link dropdown-toggle" data-toggle="dropdown" href="#Target Sites">Target Sites<span class="caret"></span></a>
-              <ul class="dropdown-menu">
-                {% block site_name_menu %}{% endblock %}           
-              </ul>
-            </li>
+            <a class="nav-link" href="#cls_res_section"> Classifier Results </a>
           </li>
           <li class="nav-item">
-            <a class="nav-link" href="#Crispector_Main_Log">Crispector Main Log</a>
+            <a class="nav-link" href="#read_section">{% block read_section_title %}{% endblock %}</a>
           </li>
         </ul>
       </div>
+    </div>
   </nav>
 
   <!-- Page Content -->
-  <div class="container">
+<div class="container">
     <div class="row justify-content-center">
       <div class="col-lg-12 text-center">
-        <img src="{% block crispector_logo %}{% endblock %}" width="50%">
+        <img src="{% block crispector_logo %}{% endblock %}" width="40%">
         <div class="hr-divider">
           <h5 class="hr-divider-content hr-divider-heading">
             Accurate analysis of off-target editing activity from comparative NGS data
+            <br>
+            <br>
+            {% block title %}{% endblock %}
+            <br>
+            <br>
           </h5>
         </div>
       </div>
     </div>
       
   <ul class="list-group list-group-flush">
-    
-      <div class="row justify-content-center">
-        <div class="col-lg-12">
-          <div class="card text-center">
-            <li class="list-group-item">
-              <div id="edit_section" class="card-header">
-                <h5 style="text-align:center">{{ self.edit_section_title() }}</h5>
+    <div class="row justify-content-center">
+      <div class="col-lg-12">
+        <div class="card text-center">
+          <li class="list-group-item">
+            <div id="edit_activity" class="card-header">
+              <h5 style="text-align:center">{{ self.editing_activity_title() }}</h5>
+            </div>
+            <a href="{% block editing_activity_pdf_path %}{% endblock %}"><img src="{% block editing_activity_plot_path %}{% endblock %}" width='50%' ></a>
+            <p>{% block edit_section_editing_activity_edit_text %}{% endblock %}</p>
+            <br>
+            <br>
+          </li>
+        </div>
+      </div>
+    </div>
+    <div>
+      <br></br>
+    </div>
+    <div class="row justify-content-center">
+      <div class="col-lg-12">
+        <div class="card text-center">
+          <li class="list-group-item">
+            <div id="mod_section" class="card-header">
+              <h5 style="text-align:center">{{ self.modification_section_title() }}</h5>
+            </div>
+            <ul class="nav nav-tabs justify-content-center" id="myTab" role="tablist">
+              <li class="nav-item">
+                <a class="nav-link active" id="edit_dist" data-toggle="tab" href="#edit_distribution" role="tab" aria-controls="" aria-selected="true">{% block modification_section_edit_distribution_title %}{% endblock %}</a>
+              </li>
+              <li class="nav-item">
+                <a class="nav-link" id="mod_dist" data-toggle="tab" href="#mod_distribution" role="tab" aria-controls="" aria-selected="false">{% block modification_section_modification_distribution_title %}{% endblock %}</a>
+              </li>
+              <li class="nav-item">
+                <a class="nav-link" id="edit_size_dist" data-toggle="tab" href="#edit_size_distribution" role="tab" aria-controls="" aria-selected="false">{% block modification_section_edit_size_distribution_title %}{% endblock %}</a>
+              </li>
+            </ul>
+            <div class="tab-content" id="myTabContent">
+              <div class="tab-pane fade show active" id="edit_distribution" role="tabpanel" aria-labelledby="mapping_stats-tab">
+                <a href="{% block modification_section_edit_distribution_pdf_path %}{% endblock %}"><img src="{% block modification_section_edit_distribution_plot_path %}{% endblock %}" width='90%' ></a>
+                  <br>
+                  <br>
               </div>
-              <div class="card-body">
-                <ul class="nav nav-tabs justify-content-center" id="myTab" role="tablist">
-                  <li class="nav-item">
-                    <a class="nav-link active" id="edit_section_editing_activity_tab" data-toggle="tab" href="#edit_section_editing_activity" role="tab" aria-controls="" aria-selected="true">{% block edit_section_editing_activity_title %}{% endblock %}</a>
-                  </li>
-                  <li class="nav-item">
-                    <a class="nav-link" id="edit_section_result_table_tab" data-toggle="tab" href="#edit_section_result_table" role="tab" aria-controls="mapping_per_site" aria-selected="false">{% block edit_section_result_table_title %}{% endblock %}</a>
-                  </li>
-                </ul>
-                <div class="tab-content" id="edit_section">
-                  <div class="tab-pane fade show active" id="edit_section_editing_activity" role="tabpanel" aria-labelledby="mapping_stats-tab">
-                    <a href="{% block edit_section_editing_activity_pdf_path %}{% endblock %}"><img src="{% block edit_section_editing_activity_plot_path %}{% endblock %}" width={{exp_param_d.edit_section.editing_activity.width}}></a>
-                  </div>
-                  <div class="tab-pane fade" id="edit_section_result_table" role="tabpanel" aria-labelledby="edit_section_result_table">
-                    <table class="table table-hover">
-                      {% block edit_section_result_table %}{% endblock %}
-                    </table>
-                    <br></br>
-                  </div>
-                </div>
+              <div class="tab-pane fade" id="mod_distribution" role="tabpanel" aria-labelledby="mapping_stats-tab">
+                <a href="{% block modification_section_modification_distribution_pdf_path %}{% endblock %}"><img src="{% block modification_section_modification_distribution_plot_path %}{% endblock %}" width='90%' ></a>
+                <br>
+                <br>
+              </div>
+              <div class="tab-pane fade" id="edit_size_distribution" role="tabpanel" aria-labelledby="mapping_stats-tab">
+                <a href="{% block modification_section_edit_size_distribution_pdf_path %}{% endblock %}"><img src="{% block modification_section_edit_size_distribution_plot_path %}{% endblock %}" width='90%' ></a>
+                <br>
+                <br>
               </div>
-            </li>
-          </div>
+            </div>
+          </li>
         </div>
       </div>
-      {% block translocations %}{% endblock translocations %}
-      <div>
-        <br></br>
-      </div>
-        <div class="row justify-content-center">
-          <div class="col-lg-12">
-            <div class="card text-center">
-              <li class="list-group-item">
-                <div id="Reading_Statistics" class="card-header">
-                  <h5 style="text-align:center">{{ self.reading_stats_title() }}</h5>
+    </div>
+    <div>
+      <br></br>
+    </div>
+    <div class="row justify-content-center">
+      <div class="col-lg-12">
+        <div class="card text-center">
+          <li class="list-group-item">
+            <div id="cls_res_section" class="card-header">
+              <h5 style="text-align:center">{{ self.classifier_results_section_title() }}</h5>
+            </div>
+              <ul class="nav nav-tabs justify-content-center" id="myTab" role="tablist">
+                <li class="nav-item">
+                  <a class="nav-link active" id="classifier_results_del" data-toggle="tab" href="#del" role="tab" aria-controls="" aria-selected="true">{% block classifier_results_section_classifier_results_del_title %}{% endblock %}</a>
+                </li>
+                <li class="nav-item">
+                  <a class="nav-link" id="classifier_results_ins" data-toggle="tab" href="#ins" role="tab" aria-controls="" aria-selected="false">{% block classifier_results_section_classifier_results_ins_title %}{% endblock %}</a>
+                </li>
+                <li class="nav-item">
+                  <a class="nav-link" id="classifier_results_mix" data-toggle="tab" href="#mix" role="tab" aria-controls="" aria-selected="false">{% block classifier_results_section_classifier_results_mix_title %}{% endblock %}</a>
+                </li>
+              </ul>
+              <div class="tab-content" id="myTabContent">
+                <div class="tab-pane fade show active" id="del" role="tabpanel" aria-labelledby="">
+                  <a href="{% block classifier_results_section_classifier_results_del_pdf_path %}{% endblock %}"><img src="{% block classifier_results_section_classifier_results_del_plot_path %}{% endblock %}" width='95%' ></a>
+                  <br>
+                  <br>
                 </div>
-                <div class="card-body">
-                  <ul class="nav nav-tabs justify-content-center" id="Reading_Statistics" role="tablist">
-                    <li class="nav-item">
-                      <a class="nav-link active" id="mapping_stats-tab" data-toggle="tab" href="#mapping_stats" role="tab" aria-controls="" aria-selected="true">{% block reading_stats_mapping_stats_title %}{% endblock %}</a>
-                    </li>
-                    <li class="nav-item">
-                      <a class="nav-link" id="mapping_per_site-tab" data-toggle="tab" href="#mapping_per_site" role="tab" aria-controls="mapping_per_site" aria-selected="false">{% block reading_stats_mapping_per_site_title %}{% endblock %}</a>
-                    </li>
-                  </ul>
-                  <div class="tab-content" id="myTabContent">
-                    <div class="tab-pane fade show active" id="mapping_stats" role="tabpanel" aria-labelledby="mapping_stats-tab">
-                      <a href="{% block reading_stats_mapping_stats_pdf_path %}{% endblock %}"><img src="{% block reading_stats_mapping_stats_plot_path %}{% endblock %}" width='95%' ></a>
-                      <br>
-                      <br>
-                      <br>
-                      {% block reading_stats_fastp %}{% endblock reading_stats_fastp %}
-                      <br>
-                      <br>
-                      <p style="text-align: center;"><b> </b></p>
-                      <p style="text-align: center;"><b>Warnings</b></p>
-                      {% block reading_stats_discarded_sites %}{% endblock reading_stats_discarded_sites %}
-                      <br>
-                    </div>
-                    <div class="tab-pane fade" id="mapping_per_site" role="tabpanel" aria-labelledby="mapping_per_site-tab">
-                      <a href="{% block reading_stats_mapping_per_site_pdf_path %}{% endblock %}"><img src="{% block reading_stats_mapping_per_site_plot_path %}{% endblock %}" width='95%'></a>
-                      <br>
-                      <br>
-                      <br>
-                      {{ self.reading_stats_fastp() }}
-                      <br>
-                      <br>
-                      <p style="text-align: center;"><b> </b></p>
-                      <p style="text-align: center;"><b>Warnings</b></p>
-                      {{ self.reading_stats_discarded_sites() }}
-                      <br>
-                    </div>
-                  </div>
+                <div class="tab-pane fade" id="ins" role="tabpanel" aria-labelledby="">
+                  <a href="{% block classifier_results_section_classifier_results_ins_pdf_path %}{% endblock %}"><img src="{% block classifier_results_section_classifier_results_ins_plot_path %}{% endblock %}" width='95%' ></a>
+                  <br>
+                  <br>
                 </div>
-              </li>
-            </div>
-          </div>
-        </div> 
-        <div>
-          <br></br>
+                <div class="tab-pane fade" id="mix" role="tabpanel" aria-labelledby="">
+                  <a href="{% block classifier_results_section_classifier_results_mix_pdf_path %}{% endblock %}"><img src="{% block classifier_results_section_classifier_results_mix_plot_path %}{% endblock %}" width='95%' ></a>
+                  <br>
+                  <br>
+                </div>
+              </div>
+          </li> 
         </div>
-        <div class="row justify-content-center">
-          <div class="col-lg-12">
-            <div class="card text-center">
-                  <li class="list-group-item" id="Target Sites">
-                    <div class="card-header">
-                      <h5 style="text-align:center">Target Sites</h5>
-                    </div>
-                  </li>
-                  {% block site_name %}{% endblock %}
-            </div>
-          </div>
-        </div> 
-        <div>
-          <br></br>
+      </div>
+    </div>
+    <div>
+      <br></br>
+    </div>
+    <div class="row justify-content-center">
+      <div class="col-lg-12">
+        <div class="card text-center">
+          <li class="list-group-item">  
+            <div id="read_section" class="card-header">         
+              <h5 style="text-align:center">{{ self.read_section_title() }}</h5>
+            </div>
+            <div class="card-body" style="align-content: center;">
+              <table style="width:100%; vertical-align: middle;">
+                <tr>
+                  <th style="right: auto;">{% block read_section_edited_reads %}{% endblock read_section_edited_reads %}</th>
+                </tr>
+                <tr>
+                  <th style="right: auto;">{% block read_section_treatment_aligned_reads %}{% endblock read_section_treatment_aligned_reads %}</th>
+                  <th style="left: auto;">{% block read_section_mock_aligned_reads %}{% endblock read_section_mock_aligned_reads %}</th>
+                </tr>
+                <tr>
+                  <td>{% block read_section_treatment_filtered_reads %}{% endblock read_section_treatment_filtered_reads %}</td>
+                  <td>{% block read_section_mock_filtered_reads %}{% endblock read_section_mock_filtered_reads %}</td>
+                </tr>
+                <tr>
+                  <td>{% block read_section_fastp_tx_path %}{% endblock read_section_fastp_tx_path %}</td>
+                  <td>{% block read_section_fastp_mock_path %}{% endblock read_section_fastp_mock_path %}</td>
+                </tr>
+              </table>
+              <br>
+              <br>
+            </div>
+          </li>
         </div>
-        <div class="row justify-content-center">
-          <div class="col-lg-12">
-            <div class="card text-center">
-                <li class="list-group-item" style="text-align: center;">   
-                  <div id="Crispector_Main_Log">    
-                    <div class="card-header">
-                      <h5 style="text-align:center">Log</h5>
-                    </div>
-                    <a href="{% block log_path %}{% endblock %}" style="text-align: center;">Crispector Log</a>
-                    <br>
-                  </div>
-                </li> 
-            </div>
-          </div>
-        </div> 
-  </ul>
+      </div>
+    </div> 
+  </ul>            
 </div>
-            
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,40 +1,65 @@
-    * _{_%_ _b_l_o_c_k_ _e_d_i_t___s_e_c_t_i_o_n___t_i_t_l_e_ _%_}_{_%_ _e_n_d_b_l_o_c_k_ _%_}
-    * {% block translocations_menu %}{% endblock translocations_menu %}
-    * _{_%_ _b_l_o_c_k_ _r_e_a_d_i_n_g___s_t_a_t_s___t_i_t_l_e_ _%_}_{_%_ _e_n_d_b_l_o_c_k_ _%_}
-    * _T_a_r_g_e_t_ _S_i_t_e_s
-          o {% block site_name_menu %}{% endblock %}
-_C_r_i_s_p_e_c_t_o_r_ _M_a_i_n_ _L_o_g
+    * _{_%_ _b_l_o_c_k_ _e_d_i_t_i_n_g___a_c_t_i_v_i_t_y___t_i_t_l_e_ _%_}_{_%_ _e_n_d_b_l_o_c_k_ _%_}
+    * _{_%_ _b_l_o_c_k_ _m_o_d_i_f_i_c_a_t_i_o_n___s_e_c_t_i_o_n___t_i_t_l_e_ _%_}_{_%_ _e_n_d_b_l_o_c_k_ _%_}
+    * _C_l_a_s_s_i_f_i_e_r_ _R_e_s_u_l_t_s
+    * _{_%_ _b_l_o_c_k_ _r_e_a_d___s_e_c_t_i_o_n___t_i_t_l_e_ _%_}_{_%_ _e_n_d_b_l_o_c_k_ _%_}
 [{% block crispector_logo %}{% endblock %}]
 **** AAccccuurraattee aannaallyyssiiss ooff ooffff--ttaarrggeett eeddiittiinngg aaccttiivviittyy ffrroomm ccoommppaarraattiivvee NNGGSS ddaattaa
-****
-    * **** {{{{ sseellff..eeddiitt__sseeccttiioonn__ttiittllee(()) }}}} ****
-          o _{_%_ _b_l_o_c_k_ _e_d_i_t___s_e_c_t_i_o_n___e_d_i_t_i_n_g___a_c_t_i_v_i_t_y___t_i_t_l_e_ _%_}_{_%_ _e_n_d_b_l_o_c_k_ _%_}
-          o _{_%_ _b_l_o_c_k_ _e_d_i_t___s_e_c_t_i_o_n___r_e_s_u_l_t___t_a_b_l_e___t_i_t_l_e_ _%_}_{_%_ _e_n_d_b_l_o_c_k_ _%_}
-      _[_{_%_ _b_l_o_c_k_ _e_d_i_t___s_e_c_t_i_o_n___e_d_i_t_i_n_g___a_c_t_i_v_i_t_y___p_l_o_t___p_a_t_h_ _%_}_{_%_ _e_n_d_b_l_o_c_k_ _%_}_]
 
-{% block translocations %}{% endblock translocations %}
+{{%% bblloocckk ttiittllee %%}}{{%% eennddbblloocckk %%}}
 
-**** {{{{ sseellff..rreeaaddiinngg__ssttaattss__ttiittllee(()) }}}} ****
-    * _{_%_ _b_l_o_c_k_ _r_e_a_d_i_n_g___s_t_a_t_s___m_a_p_p_i_n_g___s_t_a_t_s___t_i_t_l_e_ _%_}_{_%_ _e_n_d_b_l_o_c_k_ _%_}
-    * _{_%_ _b_l_o_c_k_ _r_e_a_d_i_n_g___s_t_a_t_s___m_a_p_p_i_n_g___p_e_r___s_i_t_e___t_i_t_l_e_ _%_}_{_%_ _e_n_d_b_l_o_c_k_ _%_}
-_[_{_%_ _b_l_o_c_k_ _r_e_a_d_i_n_g___s_t_a_t_s___m_a_p_p_i_n_g___s_t_a_t_s___p_l_o_t___p_a_t_h_ _%_}_{_%_ _e_n_d_b_l_o_c_k_ _%_}_]
+ ****
+    * **** {{{{ sseellff..eeddiittiinngg__aaccttiivviittyy__ttiittllee(()) }}}} ****
+      _[_{_%_ _b_l_o_c_k_ _e_d_i_t_i_n_g___a_c_t_i_v_i_t_y___p_l_o_t___p_a_t_h_ _%_}_{_%_ _e_n_d_b_l_o_c_k_ _%_}_]
+      {% block edit_section_editing_activity_edit_text %}{% endblock %}
 
 
-{% block reading_stats_fastp %}{% endblock reading_stats_fastp %}
 
-WWaarrnniinnggss
-{% block reading_stats_discarded_sites %}{% endblock
-reading_stats_discarded_sites %}
-_[_{_%_ _b_l_o_c_k_ _r_e_a_d_i_n_g___s_t_a_t_s___m_a_p_p_i_n_g___p_e_r___s_i_t_e___p_l_o_t___p_a_t_h_ _%_}_{_%_ _e_n_d_b_l_o_c_k_ _%_}_]
+**** {{{{ sseellff..mmooddiiffiiccaattiioonn__sseeccttiioonn__ttiittllee(()) }}}} ****
+    * _{_%_ _b_l_o_c_k_ _m_o_d_i_f_i_c_a_t_i_o_n___s_e_c_t_i_o_n___e_d_i_t___d_i_s_t_r_i_b_u_t_i_o_n___t_i_t_l_e_ _%_}_{_%_ _e_n_d_b_l_o_c_k_ _%_}
+    * _{_%_ _b_l_o_c_k_ _m_o_d_i_f_i_c_a_t_i_o_n___s_e_c_t_i_o_n___m_o_d_i_f_i_c_a_t_i_o_n___d_i_s_t_r_i_b_u_t_i_o_n___t_i_t_l_e_ _%_}_{_%
+      _e_n_d_b_l_o_c_k_ _%_}
+    * _{_%_ _b_l_o_c_k_ _m_o_d_i_f_i_c_a_t_i_o_n___s_e_c_t_i_o_n___e_d_i_t___s_i_z_e___d_i_s_t_r_i_b_u_t_i_o_n___t_i_t_l_e_ _%_}_{_%_ _e_n_d_b_l_o_c_k
+      _%_}
+_[_{_%_ _b_l_o_c_k_ _m_o_d_i_f_i_c_a_t_i_o_n___s_e_c_t_i_o_n___e_d_i_t___d_i_s_t_r_i_b_u_t_i_o_n___p_l_o_t___p_a_t_h_ _%_}_{_%_ _e_n_d_b_l_o_c_k_ _%_}_]
+
+_[_{_%_ _b_l_o_c_k_ _m_o_d_i_f_i_c_a_t_i_o_n___s_e_c_t_i_o_n___m_o_d_i_f_i_c_a_t_i_o_n___d_i_s_t_r_i_b_u_t_i_o_n___p_l_o_t___p_a_t_h_ _%_}_{_%
+_e_n_d_b_l_o_c_k_ _%_}_]
+
+_[_{_%_ _b_l_o_c_k_ _m_o_d_i_f_i_c_a_t_i_o_n___s_e_c_t_i_o_n___e_d_i_t___s_i_z_e___d_i_s_t_r_i_b_u_t_i_o_n___p_l_o_t___p_a_t_h_ _%_}_{_%_ _e_n_d_b_l_o_c_k
+_%_}_]
+
+
+**** {{{{ sseellff..ccllaassssiiffiieerr__rreessuullttss__sseeccttiioonn__ttiittllee(()) }}}} ****
+    * _{_%_ _b_l_o_c_k_ _c_l_a_s_s_i_f_i_e_r___r_e_s_u_l_t_s___s_e_c_t_i_o_n___c_l_a_s_s_i_f_i_e_r___r_e_s_u_l_t_s___d_e_l___t_i_t_l_e_ _%_}_{_%
+      _e_n_d_b_l_o_c_k_ _%_}
+    * _{_%_ _b_l_o_c_k_ _c_l_a_s_s_i_f_i_e_r___r_e_s_u_l_t_s___s_e_c_t_i_o_n___c_l_a_s_s_i_f_i_e_r___r_e_s_u_l_t_s___i_n_s___t_i_t_l_e_ _%_}_{_%
+      _e_n_d_b_l_o_c_k_ _%_}
+    * _{_%_ _b_l_o_c_k_ _c_l_a_s_s_i_f_i_e_r___r_e_s_u_l_t_s___s_e_c_t_i_o_n___c_l_a_s_s_i_f_i_e_r___r_e_s_u_l_t_s___m_i_x___t_i_t_l_e_ _%_}_{_%
+      _e_n_d_b_l_o_c_k_ _%_}
+_[_{_%_ _b_l_o_c_k_ _c_l_a_s_s_i_f_i_e_r___r_e_s_u_l_t_s___s_e_c_t_i_o_n___c_l_a_s_s_i_f_i_e_r___r_e_s_u_l_t_s___d_e_l___p_l_o_t___p_a_t_h_ _%_}_{_%
+_e_n_d_b_l_o_c_k_ _%_}_]
+
+_[_{_%_ _b_l_o_c_k_ _c_l_a_s_s_i_f_i_e_r___r_e_s_u_l_t_s___s_e_c_t_i_o_n___c_l_a_s_s_i_f_i_e_r___r_e_s_u_l_t_s___i_n_s___p_l_o_t___p_a_t_h_ _%_}_{_%
+_e_n_d_b_l_o_c_k_ _%_}_]
+
+_[_{_%_ _b_l_o_c_k_ _c_l_a_s_s_i_f_i_e_r___r_e_s_u_l_t_s___s_e_c_t_i_o_n___c_l_a_s_s_i_f_i_e_r___r_e_s_u_l_t_s___m_i_x___p_l_o_t___p_a_t_h_ _%_}_{_%
+_e_n_d_b_l_o_c_k_ _%_}_]
+
+
+**** {{{{ sseellff..rreeaadd__sseeccttiioonn__ttiittllee(()) }}}} ****
+{{%% bblloocckk rreeaadd__sseeccttiioonn__eeddiitteedd__rreeaaddss %%}}{{%%
+eennddbblloocckk rreeaadd__sseeccttiioonn__eeddiitteedd__rreeaaddss %%}}
+{{%% bblloocckk                                {{%% bblloocckk
+rreeaadd__sseeccttiioonn__ttrreeaattmmeenntt__aalliiggnneedd__rreeaaddss %%}} rreeaadd__sseeccttiioonn__mmoocckk__aalliiggnneedd__rreeaaddss %%}}{{%%
+{{%% eennddbblloocckk                             eennddbblloocckk
+rreeaadd__sseeccttiioonn__ttrreeaattmmeenntt__aalliiggnneedd__rreeaaddss %%}} rreeaadd__sseeccttiioonn__mmoocckk__aalliiggnneedd__rreeaaddss %%}}
+{% block                                {% block
+read_section_treatment_filtered_reads   read_section_mock_filtered_reads %}{%
+%}{% endblock                           endblock
+read_section_treatment_filtered_reads   read_section_mock_filtered_reads %}
+%}
+{% block read_section_fastp_tx_path %}  {% block read_section_fastp_mock_path
+{% endblock read_section_fastp_tx_path  %}{% endblock
+%}                                      read_section_fastp_mock_path %}
 
 
-{{ self.reading_stats_fastp() }}
-
-WWaarrnniinnggss
-{{ self.reading_stats_discarded_sites() }}
-
-**** TTaarrggeett SSiitteess ****
-{% block site_name %}{% endblock %}
-
-**** LLoogg ****
-_C_r_i_s_p_e_c_t_o_r_ _L_o_g
```

### Comparing `crispector2-2.0.8/crispector2/report/html_templates/site_file_to_render.html` & `crispector2-2.0.9/crispector2/report/html_templates/site_file_to_render.html`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/report/visualization_and_output.py` & `crispector2-2.0.9/crispector2/report/visualization_and_output.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/utils/configurator.py` & `crispector2-2.0.9/crispector2/utils/configurator.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/utils/constants_and_types.py` & `crispector2-2.0.9/crispector2/utils/constants_and_types.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/utils/exceptions.py` & `crispector2-2.0.9/crispector2/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2/utils/logger.py` & `crispector2-2.0.9/crispector2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `crispector2-2.0.8/crispector2.egg-info/PKG-INFO` & `crispector2-2.0.9/crispector2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,37 @@
 Metadata-Version: 2.1
 Name: crispector2
-Version: 2.0.8
-Home-page: https://github.com/theAguy/crispector2
+Version: 2.0.9
+Summary: CRISPECTOR2 - Genome Editing Analysis Tool, with allele extension
 Author: Guy Assa
 Author-email: guyassa@gmail.com
-Requires-Python: >=3.7
+Project-URL: repository, https://github.com/theAguy/crispector2
+Keywords: crispector2
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Click>=7.0
+Requires-Dist: matplotlib>=3.1.2
+Requires-Dist: seaborn>=0.9.0
+Requires-Dist: pyyaml>=5.1.2
+Requires-Dist: plotly>=4.3.0
+Requires-Dist: numpy>=1.12.1
+Requires-Dist: pandas==1.3.5
+Requires-Dist: biopython<=1.79,>=1.74
+Requires-Dist: scipy>=1.2.1
+Requires-Dist: jinja2>=3.1.2
+Requires-Dist: tqdm>=4.66.0
+Requires-Dist: mpmath>=1.3.0
+Requires-Dist: statsmodels>=0.13.2
+Requires-Dist: edlib>=1.3.9
 
 [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/CRISPECTOR2.0/README.html)
 
 <p align="left">
   <img src="logo.png" alt="Logo" height="100">
 </p>
 #
@@ -33,15 +54,15 @@
 </p>
 
 # Installation
 
 CRISPECTOR2.0 can be installed using the [conda](http://conda.pydata.org/docs/intro.html) package manager [Bioconda](https://bioconda.github.io/) (for Linux & macOS), or as a PIP package (for Linux & macOS).
 
 ### Bioconda
-To install CRISPECTOR2.0 using Bioconda, download and install Anaconda Python 3.7, following the instructions at: https://www.anaconda.com/distribution/.
+To install CRISPECTOR2.0 using Bioconda, download and install Anaconda Python 3.8, following the instructions at: https://www.anaconda.com/distribution/.
 
 Open a terminal and type:
 
 ```
 conda config --add channels defaults
 conda config --add channels bioconda
 conda config --add channels conda-forge
@@ -49,18 +70,18 @@
 
 To install CRISPECTOR2.0 into the current conda environment, type:
 
 ```
 conda install crispector2
 ```
 
-If you don't already have an existing environment with Python 3.7, you can create one first (e.g. named `crispector_env`) with:
+If you don't already have an existing environment with Python 3.8, you can create one first (e.g. named `crispector_env`) with:
 
 ```
-conda create -n crispector_env python=3.7
+conda create -n crispector_env python=3.8
 conda activate crispector_env
 conda install crispector2
 ```
 
 Check that CRISPECTOR2.0 is installed using the help command:
 
 ```
```

### Comparing `crispector2-2.0.8/crispector2.egg-info/SOURCES.txt` & `crispector2-2.0.9/crispector2.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 crispector2/__init__.py
 crispector2/cli.py
 crispector2/crispector_main.py
 crispector2.egg-info/PKG-INFO
 crispector2.egg-info/SOURCES.txt
 crispector2.egg-info/dependency_links.txt
 crispector2.egg-info/entry_points.txt
-crispector2.egg-info/not-zip-safe
+crispector2.egg-info/requires.txt
 crispector2.egg-info/top_level.txt
 crispector2/algorithm/__init__.py
 crispector2/algorithm/binomial_probability.py
 crispector2/algorithm/core_algorithm.py
 crispector2/algorithm/translocations.py
-crispector2/algorithm/translocations_original.py
 crispector2/allele/__init__.py
 crispector2/allele/allele_mock.py
 crispector2/allele/allele_reference_df.py
 crispector2/allele/allele_tx.py
 crispector2/allele/random_reads_handler.py
 crispector2/config/__init__.py
 crispector2/config/default_config.yml
@@ -35,18 +32,15 @@
 crispector2/report/__init__.py
 crispector2/report/html_report.py
 crispector2/report/visualization_and_output.py
 crispector2/report/html_templates/.DS_Store
 crispector2/report/html_templates/crispector_logo.jpg
 crispector2/report/html_templates/crispector_logo.png
 crispector2/report/html_templates/file_to_render.html
-crispector2/report/html_templates/file_to_render_old.html
 crispector2/report/html_templates/final_layout.html
-crispector2/report/html_templates/final_layout_old.html
 crispector2/report/html_templates/site_file_to_render.html
 crispector2/report/html_templates/site_layout.html
 crispector2/utils/__init__.py
 crispector2/utils/configurator.py
 crispector2/utils/constants_and_types.py
-crispector2/utils/constants_and_types_old.py
 crispector2/utils/exceptions.py
 crispector2/utils/logger.py
```


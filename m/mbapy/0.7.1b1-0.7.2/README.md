# Comparing `tmp/mbapy-0.7.1b1.tar.gz` & `tmp/mbapy-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbapy-0.7.1b1.tar", last modified: Tue Mar 12 14:49:40 2024, max compression
+gzip compressed data, was "mbapy-0.7.2.tar", last modified: Sun Apr 21 13:12:32 2024, max compression
```

## Comparing `mbapy-0.7.1b1.tar` & `mbapy-0.7.2.tar`

### file list

```diff
@@ -1,101 +1,104 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.410085 mbapy-0.7.1b1/
--rw-rw-rw-   0        0        0     1085 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/LICENSE
--rw-rw-rw-   0        0        0      163 2024-01-11 01:58:53.000000 mbapy-0.7.1b1/MANIFEST.in
--rw-rw-rw-   0        0        0     7464 2024-03-12 14:49:40.409085 mbapy-0.7.1b1/PKG-INFO
--rw-rw-rw-   0        0        0     5503 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.217236 mbapy-0.7.1b1/mbapy/
--rw-rw-rw-   0        0        0     1203 2024-01-04 08:03:01.000000 mbapy-0.7.1b1/mbapy/__init__.py
--rw-rw-rw-   0        0        0      404 2024-03-12 14:49:29.000000 mbapy-0.7.1b1/mbapy/__version__.py
--rw-rw-rw-   0        0        0    26515 2024-03-01 02:09:58.000000 mbapy-0.7.1b1/mbapy/base.py
-drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.257750 mbapy-0.7.1b1/mbapy/bio/
--rw-rw-rw-   0        0        0      133 2024-01-08 14:19:44.000000 mbapy-0.7.1b1/mbapy/bio/__init__.py
--rw-rw-rw-   0        0        0    21232 2024-03-12 14:00:39.000000 mbapy-0.7.1b1/mbapy/bio/peptide.py
-drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.276890 mbapy-0.7.1b1/mbapy/dl_torch/
--rw-rw-rw-   0        0        0      361 2024-01-11 01:58:53.000000 mbapy-0.7.1b1/mbapy/dl_torch/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.278889 mbapy-0.7.1b1/mbapy/dl_torch/arch/
-drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.288218 mbapy-0.7.1b1/mbapy/dl_torch/arch/CL/
--rw-rw-rw-   0        0        0       34 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/arch/CL/__init__.py
--rw-rw-rw-   0        0        0    16559 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/arch/CL/builder.py
--rw-rw-rw-   0        0        0     2423 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/arch/CL/trainer.py
-drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.293214 mbapy-0.7.1b1/mbapy/dl_torch/arch/CLIP/
--rw-rw-rw-   0        0        0       32 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/arch/CLIP/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.1b1/mbapy/dl_torch/arch/CLIP/builder.py
--rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.1b1/mbapy/dl_torch/arch/CLIP/trainer.py
--rw-rw-rw-   0        0        0      203 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/arch/__init__.py
--rw-rw-rw-   0        0        0    26096 2024-01-05 08:43:17.000000 mbapy-0.7.1b1/mbapy/dl_torch/bb.py
--rw-rw-rw-   0        0        0     6352 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/data.py
--rw-rw-rw-   0        0        0     1063 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/hyper_search.py
--rw-rw-rw-   0        0        0     4113 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/loss.py
--rw-rw-rw-   0        0        0    13191 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/m.py
--rw-rw-rw-   0        0        0     4661 2023-12-11 09:26:16.000000 mbapy-0.7.1b1/mbapy/dl_torch/optim.py
-drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.297385 mbapy-0.7.1b1/mbapy/dl_torch/paper/
--rw-rw-rw-   0        0        0       18 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/paper/__init__.py
--rw-rw-rw-   0        0        0     2917 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/paper/bb.py
--rw-rw-rw-   0        0        0    17600 2024-01-11 07:34:28.000000 mbapy-0.7.1b1/mbapy/dl_torch/utils.py
--rw-rw-rw-   0        0        0    22069 2024-03-09 11:28:49.000000 mbapy-0.7.1b1/mbapy/file.py
-drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.305655 mbapy-0.7.1b1/mbapy/file_utils/
--rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.1b1/mbapy/file_utils/__init__.py
--rw-rw-rw-   0        0        0     7095 2023-12-18 14:29:23.000000 mbapy-0.7.1b1/mbapy/file_utils/image.py
--rw-rw-rw-   0        0        0    11531 2024-03-10 02:50:26.000000 mbapy-0.7.1b1/mbapy/file_utils/video.py
--rw-rw-rw-   0        0        0    25377 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/game.py
--rw-rw-rw-   0        0        0     3364 2023-12-18 14:29:23.000000 mbapy-0.7.1b1/mbapy/paper.py
--rw-rw-rw-   0        0        0    15911 2024-03-11 08:51:41.000000 mbapy-0.7.1b1/mbapy/plot.py
-drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.314816 mbapy-0.7.1b1/mbapy/sci_utils/
--rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.1b1/mbapy/sci_utils/__init__.py
--rw-rw-rw-   0        0        0    10594 2024-01-20 12:03:17.000000 mbapy-0.7.1b1/mbapy/sci_utils/paper_download.py
--rw-rw-rw-   0        0        0    23045 2023-12-11 09:26:16.000000 mbapy-0.7.1b1/mbapy/sci_utils/paper_parse.py
--rw-rw-rw-   0        0        0    16559 2024-01-20 12:03:17.000000 mbapy-0.7.1b1/mbapy/sci_utils/paper_search.py
-drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.361477 mbapy-0.7.1b1/mbapy/scripts/
--rw-rw-rw-   0        0        0      153 2024-01-08 13:31:52.000000 mbapy-0.7.1b1/mbapy/scripts/__init__.py
--rw-rw-rw-   0        0        0       68 2024-01-08 13:31:52.000000 mbapy-0.7.1b1/mbapy/scripts/__main__.py
--rw-rw-rw-   0        0        0     6954 2024-03-12 14:06:48.000000 mbapy-0.7.1b1/mbapy/scripts/_main_.py
--rw-rw-rw-   0        0        0      503 2024-01-25 04:33:05.000000 mbapy-0.7.1b1/mbapy/scripts/_script_utils_.py
--rw-rw-rw-   0        0        0     5549 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/scripts/avif.py
--rw-rw-rw-   0        0        0     1947 2024-01-22 08:25:16.000000 mbapy-0.7.1b1/mbapy/scripts/cluster.py
--rw-rw-rw-   0        0        0    13566 2024-01-08 13:31:52.000000 mbapy-0.7.1b1/mbapy/scripts/cnipa.py
--rw-rw-rw-   0        0        0     2741 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/scripts/cp.py
--rw-rw-rw-   0        0        0     4821 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/scripts/duitang.py
--rw-rw-rw-   0        0        0     2651 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/scripts/extract-dir.py
--rw-rw-rw-   0        0        0     2637 2024-01-08 13:31:52.000000 mbapy-0.7.1b1/mbapy/scripts/extract_paper.py
--rw-rw-rw-   0        0        0     7628 2024-01-19 15:41:57.000000 mbapy-0.7.1b1/mbapy/scripts/mass.py
--rw-rw-rw-   0        0        0     2614 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/scripts/mv.py
--rw-rw-rw-   0        0        0    25827 2024-03-12 14:29:11.000000 mbapy-0.7.1b1/mbapy/scripts/peptide.py
--rw-rw-rw-   0        0        0     1679 2024-01-12 08:11:59.000000 mbapy-0.7.1b1/mbapy/scripts/reviz.py
--rw-rw-rw-   0        0        0     2101 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/scripts/rm.py
--rw-rw-rw-   0        0        0     5392 2024-01-08 13:31:52.000000 mbapy-0.7.1b1/mbapy/scripts/scihub.py
--rw-rw-rw-   0        0        0     8636 2024-01-08 13:31:52.000000 mbapy-0.7.1b1/mbapy/scripts/scihub_selenium.py
--rw-rw-rw-   0        0        0     5633 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/scripts/splash_img.py
--rw-rw-rw-   0        0        0     9126 2024-03-10 02:52:00.000000 mbapy-0.7.1b1/mbapy/scripts/video.py
-drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.375653 mbapy-0.7.1b1/mbapy/stats/
--rw-rw-rw-   0        0        0     2839 2023-10-04 07:59:59.000000 mbapy-0.7.1b1/mbapy/stats/__init__.py
--rw-rw-rw-   0        0        0    30529 2023-10-06 03:00:11.000000 mbapy-0.7.1b1/mbapy/stats/cluster.py
--rw-rw-rw-   0        0        0    15004 2023-12-11 09:26:16.000000 mbapy-0.7.1b1/mbapy/stats/df.py
--rw-rw-rw-   0        0        0    19333 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/stats/geography.py
--rw-rw-rw-   0        0        0     1772 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/stats/reg.py
--rw-rw-rw-   0        0        0    12718 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/stats/test.py
-drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.386913 mbapy-0.7.1b1/mbapy/storage/
--rw-rw-rw-   0        0        0    69698 2024-01-11 01:58:53.000000 mbapy-0.7.1b1/mbapy/storage/libsci.dll
--rw-rw-rw-   0        0        0    15864 2024-01-11 01:58:53.000000 mbapy-0.7.1b1/mbapy/storage/libsci.so
--rw-rw-rw-   0        0        0    40252 2024-01-11 01:58:53.000000 mbapy-0.7.1b1/mbapy/storage/libstats.dll
--rw-rw-rw-   0        0        0    16752 2024-01-11 01:58:53.000000 mbapy-0.7.1b1/mbapy/storage/libstats.so
--rw-rw-rw-   0        0        0     1565 2023-12-18 14:29:23.000000 mbapy-0.7.1b1/mbapy/web.py
-drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.399903 mbapy-0.7.1b1/mbapy/web_utils/
--rw-rw-rw-   0        0        0        0 2023-07-27 10:19:54.000000 mbapy-0.7.1b1/mbapy/web_utils/__init__.py
--rw-rw-rw-   0        0        0     4133 2023-11-06 08:06:25.000000 mbapy-0.7.1b1/mbapy/web_utils/parse.py
--rw-rw-rw-   0        0        0    35766 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/web_utils/request.py
--rw-rw-rw-   0        0        0    28907 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/web_utils/spider.py
--rw-rw-rw-   0        0        0    11644 2024-02-23 13:30:29.000000 mbapy-0.7.1b1/mbapy/web_utils/task.py
-drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.254576 mbapy-0.7.1b1/mbapy.egg-info/
--rw-rw-rw-   0        0        0     7464 2024-03-12 14:49:39.000000 mbapy-0.7.1b1/mbapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2016 2024-03-12 14:49:40.000000 mbapy-0.7.1b1/mbapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 14:49:39.000000 mbapy-0.7.1b1/mbapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-03-12 14:49:39.000000 mbapy-0.7.1b1/mbapy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      908 2024-03-12 14:49:39.000000 mbapy-0.7.1b1/mbapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-12 14:49:39.000000 mbapy-0.7.1b1/mbapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      891 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/requirements.json
--rw-rw-rw-   0        0        0       42 2024-03-12 14:49:40.410085 mbapy-0.7.1b1/setup.cfg
--rw-rw-rw-   0        0        0     3400 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.407086 mbapy-0.7.1b1/test/
--rw-rw-rw-   0        0        0     2028 2024-01-11 01:58:53.000000 mbapy-0.7.1b1/test/test_base.py
--rw-rw-rw-   0        0        0     1575 2023-10-20 09:14:56.000000 mbapy-0.7.1b1/test/test_game.py
--rw-rw-rw-   0        0        0     1742 2024-01-11 01:58:53.000000 mbapy-0.7.1b1/test/test_web.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.198437 mbapy-0.7.2/
+-rw-rw-rw-   0        0        0     1085 2023-09-30 06:15:47.000000 mbapy-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0      214 2024-04-21 10:41:48.000000 mbapy-0.7.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7500 2024-04-21 13:12:32.197438 mbapy-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5549 2024-04-04 11:37:22.000000 mbapy-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.059190 mbapy-0.7.2/mbapy/
+-rw-rw-rw-   0        0        0     1203 2024-01-04 08:03:01.000000 mbapy-0.7.2/mbapy/__init__.py
+-rw-rw-rw-   0        0        0      402 2024-04-21 13:06:56.000000 mbapy-0.7.2/mbapy/__version__.py
+-rw-rw-rw-   0        0        0    26515 2024-03-01 02:09:58.000000 mbapy-0.7.2/mbapy/base.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.075514 mbapy-0.7.2/mbapy/bio/
+-rw-rw-rw-   0        0        0      133 2024-01-08 14:19:44.000000 mbapy-0.7.2/mbapy/bio/__init__.py
+-rw-rw-rw-   0        0        0    21232 2024-03-12 14:00:39.000000 mbapy-0.7.2/mbapy/bio/peptide.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.088507 mbapy-0.7.2/mbapy/dl_torch/
+-rw-rw-rw-   0        0        0      361 2024-01-11 01:58:53.000000 mbapy-0.7.2/mbapy/dl_torch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.090507 mbapy-0.7.2/mbapy/dl_torch/arch/
+drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.094686 mbapy-0.7.2/mbapy/dl_torch/arch/CL/
+-rw-rw-rw-   0        0        0       34 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/arch/CL/__init__.py
+-rw-rw-rw-   0        0        0    16559 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/arch/CL/builder.py
+-rw-rw-rw-   0        0        0     2423 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/arch/CL/trainer.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.098682 mbapy-0.7.2/mbapy/dl_torch/arch/CLIP/
+-rw-rw-rw-   0        0        0       32 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/arch/CLIP/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.2/mbapy/dl_torch/arch/CLIP/builder.py
+-rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.2/mbapy/dl_torch/arch/CLIP/trainer.py
+-rw-rw-rw-   0        0        0      203 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/arch/__init__.py
+-rw-rw-rw-   0        0        0    26096 2024-01-05 08:43:17.000000 mbapy-0.7.2/mbapy/dl_torch/bb.py
+-rw-rw-rw-   0        0        0     6352 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/data.py
+-rw-rw-rw-   0        0        0     1063 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/hyper_search.py
+-rw-rw-rw-   0        0        0     4113 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/loss.py
+-rw-rw-rw-   0        0        0    13191 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/m.py
+-rw-rw-rw-   0        0        0     4661 2023-12-11 09:26:16.000000 mbapy-0.7.2/mbapy/dl_torch/optim.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.101844 mbapy-0.7.2/mbapy/dl_torch/paper/
+-rw-rw-rw-   0        0        0       18 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/paper/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/paper/bb.py
+-rw-rw-rw-   0        0        0    17600 2024-01-11 07:34:28.000000 mbapy-0.7.2/mbapy/dl_torch/utils.py
+-rw-rw-rw-   0        0        0    22088 2024-04-21 10:54:51.000000 mbapy-0.7.2/mbapy/file.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.105842 mbapy-0.7.2/mbapy/file_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.2/mbapy/file_utils/__init__.py
+-rw-rw-rw-   0        0        0     7095 2023-12-18 14:29:23.000000 mbapy-0.7.2/mbapy/file_utils/image.py
+-rw-rw-rw-   0        0        0    11531 2024-03-10 02:50:26.000000 mbapy-0.7.2/mbapy/file_utils/video.py
+-rw-rw-rw-   0        0        0    25377 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/game.py
+-rw-rw-rw-   0        0        0     3364 2023-12-18 14:29:23.000000 mbapy-0.7.2/mbapy/paper.py
+-rw-rw-rw-   0        0        0    22809 2024-04-18 04:48:16.000000 mbapy-0.7.2/mbapy/plot.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.110839 mbapy-0.7.2/mbapy/sci_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.2/mbapy/sci_utils/__init__.py
+-rw-rw-rw-   0        0        0    10594 2024-01-20 12:03:17.000000 mbapy-0.7.2/mbapy/sci_utils/paper_download.py
+-rw-rw-rw-   0        0        0    23045 2023-12-11 09:26:16.000000 mbapy-0.7.2/mbapy/sci_utils/paper_parse.py
+-rw-rw-rw-   0        0        0    16559 2024-01-20 12:03:17.000000 mbapy-0.7.2/mbapy/sci_utils/paper_search.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.147013 mbapy-0.7.2/mbapy/scripts/
+-rw-rw-rw-   0        0        0      153 2024-01-08 13:31:52.000000 mbapy-0.7.2/mbapy/scripts/__init__.py
+-rw-rw-rw-   0        0        0       68 2024-01-08 13:31:52.000000 mbapy-0.7.2/mbapy/scripts/__main__.py
+-rw-rw-rw-   0        0        0     2821 2024-04-21 10:45:32.000000 mbapy-0.7.2/mbapy/scripts/_main_.py
+-rw-rw-rw-   0        0        0      522 2024-04-10 06:02:44.000000 mbapy-0.7.2/mbapy/scripts/_script_utils_.py
+-rw-rw-rw-   0        0        0     5549 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/scripts/avif.py
+-rw-rw-rw-   0        0        0     1947 2024-01-22 08:25:16.000000 mbapy-0.7.2/mbapy/scripts/cluster.py
+-rw-rw-rw-   0        0        0    13566 2024-01-08 13:31:52.000000 mbapy-0.7.2/mbapy/scripts/cnipa.py
+-rw-rw-rw-   0        0        0     2741 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/scripts/cp.py
+-rw-rw-rw-   0        0        0     4821 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/scripts/duitang.py
+-rw-rw-rw-   0        0        0     2651 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/scripts/extract-dir.py
+-rw-rw-rw-   0        0        0     2637 2024-01-08 13:31:52.000000 mbapy-0.7.2/mbapy/scripts/extract_paper.py
+-rw-rw-rw-   0        0        0     3781 2024-04-15 15:02:22.000000 mbapy-0.7.2/mbapy/scripts/file-size.py
+-rw-rw-rw-   0        0        0     9123 2024-04-21 10:31:57.000000 mbapy-0.7.2/mbapy/scripts/hplc.py
+-rw-rw-rw-   0        0        0    14739 2024-04-21 13:10:16.000000 mbapy-0.7.2/mbapy/scripts/mass.py
+-rw-rw-rw-   0        0        0     2614 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/scripts/mv.py
+-rw-rw-rw-   0        0        0    26028 2024-04-10 09:30:41.000000 mbapy-0.7.2/mbapy/scripts/peptide.py
+-rw-rw-rw-   0        0        0     1679 2024-01-12 08:11:59.000000 mbapy-0.7.2/mbapy/scripts/reviz.py
+-rw-rw-rw-   0        0        0     2101 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/scripts/rm.py
+-rw-rw-rw-   0        0        0     5392 2024-01-08 13:31:52.000000 mbapy-0.7.2/mbapy/scripts/scihub.py
+-rw-rw-rw-   0        0        0     8636 2024-01-08 13:31:52.000000 mbapy-0.7.2/mbapy/scripts/scihub_selenium.py
+-rw-rw-rw-   0        0        0     5633 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/scripts/splash_img.py
+-rw-rw-rw-   0        0        0     9128 2024-03-14 08:21:47.000000 mbapy-0.7.2/mbapy/scripts/video.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.169338 mbapy-0.7.2/mbapy/stats/
+-rw-rw-rw-   0        0        0     2839 2023-10-04 07:59:59.000000 mbapy-0.7.2/mbapy/stats/__init__.py
+-rw-rw-rw-   0        0        0    30529 2023-10-06 03:00:11.000000 mbapy-0.7.2/mbapy/stats/cluster.py
+-rw-rw-rw-   0        0        0    15779 2024-04-09 06:03:49.000000 mbapy-0.7.2/mbapy/stats/df.py
+-rw-rw-rw-   0        0        0    19333 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/stats/geography.py
+-rw-rw-rw-   0        0        0     3784 2024-04-02 03:46:14.000000 mbapy-0.7.2/mbapy/stats/reg.py
+-rw-rw-rw-   0        0        0    16955 2024-04-05 10:19:56.000000 mbapy-0.7.2/mbapy/stats/test.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.183329 mbapy-0.7.2/mbapy/storage/
+-rw-rw-rw-   0        0        0    69698 2024-01-11 01:58:53.000000 mbapy-0.7.2/mbapy/storage/libsci.dll
+-rw-rw-rw-   0        0        0    15864 2024-01-11 01:58:53.000000 mbapy-0.7.2/mbapy/storage/libsci.so
+-rw-rw-rw-   0        0        0    40252 2024-01-11 01:58:53.000000 mbapy-0.7.2/mbapy/storage/libstats.dll
+-rw-rw-rw-   0        0        0    16752 2024-01-11 01:58:53.000000 mbapy-0.7.2/mbapy/storage/libstats.so
+-rw-rw-rw-   0        0        0     3546 2024-04-21 10:41:06.000000 mbapy-0.7.2/mbapy/storage/mbapy-cli-scripts-list.json
+-rw-rw-rw-   0        0        0     1565 2023-12-18 14:29:23.000000 mbapy-0.7.2/mbapy/web.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.191324 mbapy-0.7.2/mbapy/web_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-27 10:19:54.000000 mbapy-0.7.2/mbapy/web_utils/__init__.py
+-rw-rw-rw-   0        0        0     4133 2023-11-06 08:06:25.000000 mbapy-0.7.2/mbapy/web_utils/parse.py
+-rw-rw-rw-   0        0        0    35766 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/web_utils/request.py
+-rw-rw-rw-   0        0        0    28907 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/web_utils/spider.py
+-rw-rw-rw-   0        0        0    11644 2024-02-23 13:30:29.000000 mbapy-0.7.2/mbapy/web_utils/task.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.073607 mbapy-0.7.2/mbapy.egg-info/
+-rw-rw-rw-   0        0        0     7500 2024-04-21 13:12:31.000000 mbapy-0.7.2/mbapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2107 2024-04-21 13:12:31.000000 mbapy-0.7.2/mbapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 13:12:31.000000 mbapy-0.7.2/mbapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-21 13:12:31.000000 mbapy-0.7.2/mbapy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      961 2024-04-21 13:12:31.000000 mbapy-0.7.2/mbapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-21 13:12:31.000000 mbapy-0.7.2/mbapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      899 2024-04-09 04:33:27.000000 mbapy-0.7.2/requirements.json
+-rw-rw-rw-   0        0        0       42 2024-04-21 13:12:32.198437 mbapy-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     3400 2024-04-21 13:07:12.000000 mbapy-0.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.196439 mbapy-0.7.2/test/
+-rw-rw-rw-   0        0        0     2028 2024-01-11 01:58:53.000000 mbapy-0.7.2/test/test_base.py
+-rw-rw-rw-   0        0        0     1575 2023-10-20 09:14:56.000000 mbapy-0.7.2/test/test_game.py
+-rw-rw-rw-   0        0        0     1742 2024-01-11 01:58:53.000000 mbapy-0.7.2/test/test_web.py
```

### Comparing `mbapy-0.7.1b1/LICENSE` & `mbapy-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/PKG-INFO` & `mbapy-0.7.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,75 @@
 Metadata-Version: 2.1
 Name: mbapy
-Version: 0.7.1b1
+Version: 0.7.2
 Summary: MyBA in Python
 Home-page: https://github.com/BHM-Bob/BA_PY
 Author: BHM-Bob G
 Author-email: bhmfly@foxmail.com
 License: MIT Licence
 Description: <!--
          * @Author: BHM-Bob 2262029386@qq.com
          * @Date: 2022-10-19 22:16:22
          * @LastEditors: BHM-Bob 2262029386@qq.com
-         * @LastEditTime: 2023-10-05 19:26:42
+         * @LastEditTime: 2024-04-04 19:36:44
          * @Description: 
         -->
-        # BA_PY
+        # BA_PY: Optimize Your Workflow with Python!
         [![Downloads](https://static.pepy.tech/badge/mbapy)](https://pepy.tech/project/mbapy) ![PyPI - Downloads](https://img.shields.io/pypi/dm/mbapy) ![GitHub all releases](https://img.shields.io/github/downloads/BHM-Bob/BA_PY/total?label=GitHub%20all%20releases%20downloads)
         
         ![GitHub repo size](https://img.shields.io/github/repo-size/BHM-Bob/BA_PY) ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/BHM-Bob/BA_PY) [![GitHub Commit Activity](https://img.shields.io/github/commit-activity/m/BHM-Bob/BA_PY)](https://github.com/BHM-Bob/BA_PY/pulse)
         
         ![PyPI - Status](https://img.shields.io/pypi/status/mbapy?label=PyPI%20Status) ![PyPI](https://img.shields.io/pypi/v/mbapy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mbapy)
         
         ![Read the Docs](https://img.shields.io/readthedocs/ba-py) ![GitHub](https://img.shields.io/github/license/BHM-Bob/BA_PY) [![built with Codeium](https://codeium.com/badges/main)](https://codeium.com)
         
         ![platform - WINDOWS](https://camo.githubusercontent.com/c292429e232884db22e86c2ea2ea7695bc49dc4ae13344003a95879eeb7425d8/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f57696e646f77732d3030373844363f7374796c653d666f722d7468652d6261646765266c6f676f3d77696e646f7773266c6f676f436f6c6f723d7768697465) ![platform - LINUX](https://camo.githubusercontent.com/7eefb2ba052806d8a9ce69863c2eeb3b03cd5935ead7bd2e9245ae2e705a1adf/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4c696e75782d4643433632343f7374796c653d666f722d7468652d6261646765266c6f676f3d6c696e7578266c6f676f436f6c6f723d626c61636b)
         
         mbapy is a Python package that includes a collection of useful Python scripts as sub-modules, and it's goal is *Basic for All in Python*.  
-        mbapy primarily focus on areas such as sci-plot, stats, web-crawler, sci-paper utilities, and deep learning with pytorch.  
+        mbapy primarily focus on data works, including data-retrieval, data-management, data-visualization, data-analysis and data-computation. It is built for both python-users and command-line-users.
         
         ## get start
         
         #### install 
         Now, mbapy only support pypi install:  
         ```
         pip install mbapy
         ```
         
         mbapy is a multi-funtional package, and it does not require every third-party packages to make every sub-module work. However, it provides some requriements option to install more specified requirements to make some sub-modules work:  
         1. bio: some packages for biology(sci).  
             install as `pip install mbapy[bio]`  
-        2. full: full requirements to make almost every sub-module in mbapy work(except dl_torch).  
+        2. game: some packages for game(pygame).  
+            install as `pip install mbapy[game]`  
+        3. full: full requirements to make almost every sub-module in mbapy work(except dl_torch).  
              install as `pip install mbapy[full]`  
         
         If you find the latest release version has some problems, you can try install the up-to-date version on github or gitee:  
         ```
         pip install git+https://github.com/BHM-Bob/BA_PY.git
         ```
         ```
         pip install git+https://gitee.com/BHM-Bob/BA_PY.git
         ```
         
         #### docs
-        The documentation for mbapy can be found on [read the docs](https://ba-py.readthedocs.io/en/latest/), and it is the one that I will regularly update.
-        The API document for mbapy is available on its [wiki](https://github.com/BHM-Bob/BA_PY/wiki). However, please note that this wiki on GitHub has not been updated since 2023-07. 
+        The documentation for mbapy can be found on [read the docs](https://ba-py.readthedocs.io/en/latest/) or just in the `docs` folder.
         
         #### web sites
         - open source at:  
             1. [github： https://github.com/BHM-Bob/BA_PY](https://github.com/BHM-Bob/BA_PY)  
             2. [gitee： https://gitee.com/BHM-Bob/BA_PY](https://gitee.com/BHM-Bob/BA_PY)  
         - docs at: [read the docs: https://ba-py.rtfd.io](https://ba-py.readthedocs.io/en/latest/)  
+        - PyPI: [https://pypi.org/project/mbapy/](https://pypi.org/project/mbapy/)  
         
         # contain  
         ## mbapy python package  
         #### \_\_version\_\_  
         *some version info*  
+        
         #### base  
         *some utils for easier coding*
         
         #### file
         ##### image
         *imgae utils*, including reading, saving and process a image into a feature tensor via pytorch.  
         ##### video
@@ -79,14 +82,16 @@
         *utils for web-crawler*  
         ##### request
         *get a web hyml page or a selenium browser warpper for easier usage*.  
         ##### parse
         *utils for parsing html*  
         ##### task
         *small task manager*  
+        ##### spider
+        *a light-weight web spider architecture*  
         
         #### stats
         ##### cluster
         *BAKmeans, KOptim, KBayesian from KMeans, and a func for many cluster*  
         ##### df
         *pandas.dataFrame utils for stats*  
         ##### reg
@@ -119,20 +124,14 @@
         *parse paper from a pdf file into a dict of each sections* 
         
         #### scripts
         *some useful scripts for command user*  
         launch by `python -m mbapy.scripts.XXX` or `mbapy-cli XXX`.  
         
         ## examples
-        #### file
-        *some file utils things*  
-        
-        #### plot
-        1. stack bar plot with hue style  
-        
         #### web/crawler
         1. chaoxin ppt multi threads downloader (jpg->pdf)
         2. wujin search http://www.basechem.org
         3. chemSub search http://chemsub.online.fr
         4. cnipa https://pss-system.cponline.cnipa.gov.cn/seniorSearch
```

### Comparing `mbapy-0.7.1b1/README.md` & `mbapy-0.7.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 <!--
  * @Author: BHM-Bob 2262029386@qq.com
  * @Date: 2022-10-19 22:16:22
  * @LastEditors: BHM-Bob 2262029386@qq.com
- * @LastEditTime: 2023-10-05 19:26:42
+ * @LastEditTime: 2024-04-04 19:36:44
  * @Description: 
 -->
-# BA_PY
+# BA_PY: Optimize Your Workflow with Python!
 [![Downloads](https://static.pepy.tech/badge/mbapy)](https://pepy.tech/project/mbapy) ![PyPI - Downloads](https://img.shields.io/pypi/dm/mbapy) ![GitHub all releases](https://img.shields.io/github/downloads/BHM-Bob/BA_PY/total?label=GitHub%20all%20releases%20downloads)
 
 ![GitHub repo size](https://img.shields.io/github/repo-size/BHM-Bob/BA_PY) ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/BHM-Bob/BA_PY) [![GitHub Commit Activity](https://img.shields.io/github/commit-activity/m/BHM-Bob/BA_PY)](https://github.com/BHM-Bob/BA_PY/pulse)
 
 ![PyPI - Status](https://img.shields.io/pypi/status/mbapy?label=PyPI%20Status) ![PyPI](https://img.shields.io/pypi/v/mbapy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mbapy)
 
 ![Read the Docs](https://img.shields.io/readthedocs/ba-py) ![GitHub](https://img.shields.io/github/license/BHM-Bob/BA_PY) [![built with Codeium](https://codeium.com/badges/main)](https://codeium.com)
 
 ![platform - WINDOWS](https://camo.githubusercontent.com/c292429e232884db22e86c2ea2ea7695bc49dc4ae13344003a95879eeb7425d8/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f57696e646f77732d3030373844363f7374796c653d666f722d7468652d6261646765266c6f676f3d77696e646f7773266c6f676f436f6c6f723d7768697465) ![platform - LINUX](https://camo.githubusercontent.com/7eefb2ba052806d8a9ce69863c2eeb3b03cd5935ead7bd2e9245ae2e705a1adf/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4c696e75782d4643433632343f7374796c653d666f722d7468652d6261646765266c6f676f3d6c696e7578266c6f676f436f6c6f723d626c61636b)
 
 mbapy is a Python package that includes a collection of useful Python scripts as sub-modules, and it's goal is *Basic for All in Python*.  
-mbapy primarily focus on areas such as sci-plot, stats, web-crawler, sci-paper utilities, and deep learning with pytorch.  
+mbapy primarily focus on data works, including data-retrieval, data-management, data-visualization, data-analysis and data-computation. It is built for both python-users and command-line-users.
 
 ## get start
 
 #### install 
 Now, mbapy only support pypi install:  
 ```
 pip install mbapy
 ```
 
 mbapy is a multi-funtional package, and it does not require every third-party packages to make every sub-module work. However, it provides some requriements option to install more specified requirements to make some sub-modules work:  
 1. bio: some packages for biology(sci).  
     install as `pip install mbapy[bio]`  
-2. full: full requirements to make almost every sub-module in mbapy work(except dl_torch).  
+2. game: some packages for game(pygame).  
+    install as `pip install mbapy[game]`  
+3. full: full requirements to make almost every sub-module in mbapy work(except dl_torch).  
      install as `pip install mbapy[full]`  
 
 If you find the latest release version has some problems, you can try install the up-to-date version on github or gitee:  
 ```
 pip install git+https://github.com/BHM-Bob/BA_PY.git
 ```
 ```
 pip install git+https://gitee.com/BHM-Bob/BA_PY.git
 ```
 
 #### docs
-The documentation for mbapy can be found on [read the docs](https://ba-py.readthedocs.io/en/latest/), and it is the one that I will regularly update.
-The API document for mbapy is available on its [wiki](https://github.com/BHM-Bob/BA_PY/wiki). However, please note that this wiki on GitHub has not been updated since 2023-07. 
+The documentation for mbapy can be found on [read the docs](https://ba-py.readthedocs.io/en/latest/) or just in the `docs` folder.
 
 #### web sites
 - open source at:  
     1. [github： https://github.com/BHM-Bob/BA_PY](https://github.com/BHM-Bob/BA_PY)  
     2. [gitee： https://gitee.com/BHM-Bob/BA_PY](https://gitee.com/BHM-Bob/BA_PY)  
 - docs at: [read the docs: https://ba-py.rtfd.io](https://ba-py.readthedocs.io/en/latest/)  
+- PyPI: [https://pypi.org/project/mbapy/](https://pypi.org/project/mbapy/)  
 
 # contain  
 ## mbapy python package  
 #### \_\_version\_\_  
 *some version info*  
+
 #### base  
 *some utils for easier coding*
 
 #### file
 ##### image
 *imgae utils*, including reading, saving and process a image into a feature tensor via pytorch.  
 ##### video
@@ -71,14 +74,16 @@
 *utils for web-crawler*  
 ##### request
 *get a web hyml page or a selenium browser warpper for easier usage*.  
 ##### parse
 *utils for parsing html*  
 ##### task
 *small task manager*  
+##### spider
+*a light-weight web spider architecture*  
 
 #### stats
 ##### cluster
 *BAKmeans, KOptim, KBayesian from KMeans, and a func for many cluster*  
 ##### df
 *pandas.dataFrame utils for stats*  
 ##### reg
@@ -111,19 +116,13 @@
 *parse paper from a pdf file into a dict of each sections* 
 
 #### scripts
 *some useful scripts for command user*  
 launch by `python -m mbapy.scripts.XXX` or `mbapy-cli XXX`.  
 
 ## examples
-#### file
-*some file utils things*  
-
-#### plot
-1. stack bar plot with hue style  
-
 #### web/crawler
 1. chaoxin ppt multi threads downloader (jpg->pdf)
 2. wujin search http://www.basechem.org
 3. chemSub search http://chemsub.online.fr
 4. cnipa https://pss-system.cponline.cnipa.gov.cn/seniorSearch
```

### Comparing `mbapy-0.7.1b1/mbapy/__init__.py` & `mbapy-0.7.2/mbapy/__init__.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/base.py` & `mbapy-0.7.2/mbapy/base.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/bio/peptide.py` & `mbapy-0.7.2/mbapy/bio/peptide.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/dl_torch/arch/CL/builder.py` & `mbapy-0.7.2/mbapy/dl_torch/arch/CL/builder.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/dl_torch/arch/CL/trainer.py` & `mbapy-0.7.2/mbapy/dl_torch/arch/CL/trainer.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/dl_torch/bb.py` & `mbapy-0.7.2/mbapy/dl_torch/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/dl_torch/data.py` & `mbapy-0.7.2/mbapy/dl_torch/data.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/dl_torch/hyper_search.py` & `mbapy-0.7.2/mbapy/dl_torch/hyper_search.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/dl_torch/loss.py` & `mbapy-0.7.2/mbapy/dl_torch/loss.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/dl_torch/m.py` & `mbapy-0.7.2/mbapy/dl_torch/m.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/dl_torch/optim.py` & `mbapy-0.7.2/mbapy/dl_torch/optim.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/dl_torch/paper/bb.py` & `mbapy-0.7.2/mbapy/dl_torch/paper/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/dl_torch/utils.py` & `mbapy-0.7.2/mbapy/dl_torch/utils.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/file.py` & `mbapy-0.7.2/mbapy/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-11-01 19:09:54
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2024-03-09 19:28:33
+LastEditTime: 2024-04-21 18:54:51
 Description: 
 '''
 import collections
 import os
 import pickle
 import platform
 import shutil
@@ -32,14 +32,15 @@
                 import cv2
                 import torch
 
                 from mbapy.file_utils.image import *
                 from mbapy.file_utils.video import *
     except:
         pass
+    __all__extend__ = []
 else:
     # release mode
     from .base import (check_parameters_path, format_secs,
                        get_default_for_bool, parameter_checker, put_err)
 
     # video and image functions assembly
     try:# mbapy package now does not require cv2 and torch installed forcibly
@@ -70,29 +71,27 @@
     Returns a list of file paths within a given folder that have a specified extension.
 
     Args:
         - folder_path (str): The path of the folder to search for files.
         - file_extensions (List[str]): A list of file extensions to filter the search by.
             If it is empty, accept all extensions.
         - recursive (bool, optional): Whether to search subdirectories recursively. Defaults to True.
-        - name_substr (str, optional): Sub-string in file-name. Defualts to '', means not specific.
+        - name_substr (str, optional): Sub-string in file-name (NOT INCLUDE TYPE SUFFIX). Defualts to '', means not specific.
 
     Returns:
         List[str]: A list of file paths that match the specified file extensions.
     """
     file_paths = []
-    for root, dirs, files in os.walk(folder_path):
-        for file in files:
-            if any(file.endswith(extension) for extension in file_extensions) or (not file_extensions):
-                if (not name_substr) or (name_substr and name_substr in file.split(os.path.sep)[-1]):
-                    file_paths.append(os.path.join(root, file))
-        if recursive:
-            for dir in dirs:
-                file_paths.extend(get_paths_with_extension(os.path.join(root, dir),
-                                                           file_extensions, recursive, name_substr))
+    for name in os.listdir(folder_path): # do not use os.walk() to avoid FXXK files updates
+        path = os.path.join(folder_path, name)
+        if os.path.isfile(path) and (any(path.endswith(extension) for extension in file_extensions) or (not file_extensions)):
+            if (not name_substr) or (name_substr and name_substr in path.split(os.path.sep)[-1]):
+                file_paths.append(path)
+        if recursive and os.path.isdir(path):
+            file_paths.extend(get_paths_with_extension(path, file_extensions, recursive, name_substr))
     return file_paths
 
 def format_file_size(size_bits: int, return_str: bool = True):
     n = 0
     units = {0: '', 1: 'KB', 2: 'MB', 3: 'GB', 4: 'TB', 5: 'PB', 6: 'EB', 7: 'ZB', 8: 'YB'}
     
     while size_bits > 1024:
```

### Comparing `mbapy-0.7.1b1/mbapy/file_utils/image.py` & `mbapy-0.7.2/mbapy/file_utils/image.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/file_utils/video.py` & `mbapy-0.7.2/mbapy/file_utils/video.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/game.py` & `mbapy-0.7.2/mbapy/game.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/paper.py` & `mbapy-0.7.2/mbapy/paper.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/plot.py` & `mbapy-0.7.2/mbapy/plot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from functools import wraps
-from itertools import combinations
-from typing import Dict, List, Tuple, Union
+from itertools import chain, combinations
+from typing import Callable, Dict, List, Tuple, Union, Optional
 
 import matplotlib.patches as patches
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
 import numpy as np
 import pandas as pd
 import seaborn as sns
@@ -63,130 +63,206 @@
         ret = ret[:n]
     return ret
     
 class AxisLable():
     def __init__(self, name:str, hold_space:int = 1) -> None:
         self.name = name
         self.hold_space = hold_space
+        self.father = None
+        self.child = set()
+        self._hash = id(self) # 固定hash值
+    def __eq__(self, other: 'AxisLable') -> bool:
+        return id(self) == id(other)
+    def __hash__(self) -> int:
+        return self._hash
     def add_space(self, space:int = 1):
         self.hold_space += space
+    def add_father(self, father: 'AxisLable'):
+        self.father = father
+        self.father.child.add(self)
 
-def pro_hue_pos(factors:List[str], df:pd.DataFrame, width:float, bar_space:float):
+def pro_hue_pos(factors:List[str], df:pd.DataFrame, width:float,
+                hue_space:float, bar_space:float):
     """
     Generate the position and labels for a grouped bar plot with multiple factors.
 
     Args:
-        factors (List[str]): A list of strings representing the factors to group the bars by.
-        df (pd.DataFrame): A pandas DataFrame containing the data for the bar plot.
-        width (float): The width of each individual bar.
-        bar_space (float): The space between each group of bars.
+        - factors (List[str]): A list of strings representing the factors to group the bars by.
+        - df (pd.DataFrame): A pandas DataFrame containing the data for the bar plot.
+        - width (float): The width of each individual bar.
+        - hue_space (float): The space between each group of bars.
+        - bar_space (float): The space between each bar in a group.
 
     Returns:
         Tuple[List[List[AxisLable]], List[List[float]]]: A tuple containing two lists. The first list contains the labels for each factor and each bar. The second list contains the x-positions for each bar.
 
-    """
-    xlabels, fc_old, pos = [ [] for _ in range(len(factors))], '', []
-    for f_i, f in enumerate(factors):
-        for fc_i, fc in enumerate(df[f]):
-            if fc != fc_old:
-                xlabels[f_i].append(AxisLable(fc))
-                fc_old = fc
+    Notes:
+        - `df` must be processed by `pro_bar_data` or `sort_df_factors`.
+        - The LAST factor will be the TOP level x-axis.
+    """
+    xlabels, fj_old, pos = [ [] for _ in range(len(factors))], None, []
+    xlabels_mat = df[factors].T.values.tolist()
+    # build relationships between each level sub-factors. build xlabels and allocte space for each level.
+    for i, fi in enumerate(factors[::-1]): # 从最高级开始
+        for j, fj in enumerate(df[fi]):
+            # 不同sub-factor 或 相同sub-factor但上级sub-factor不同
+            if (str(fi)+str(fj)) != fj_old or (i > 0 and xlabels_mat[i-1][j] != xlabels_mat[i-1][j-1]):
+                xlabels_mat[i][j] = AxisLable(fj)
+                xlabels[i].append(AxisLable(fj))
+                fj_old = str(fi)+str(fj) # 以防两个级别的factors中出现相同的sub-factors
+                if i > 0:
+                    xlabels_mat[i][j].add_father(xlabels_mat[i-1][j])
             else:
-                xlabels[f_i][-1].add_space()
+                xlabels_mat[i][j] = xlabels_mat[i][j-1]
+                xlabels[i][-1].add_space()
+    xlabels = xlabels[::-1] # 倒序，使最高级在最后
     xlabels.append([AxisLable(factors[-1], df.shape[0])])#master level has an extra total axis as x_title
     for axis_idx in range(len(xlabels)):
         pos.append([])
         if axis_idx == 0:
-            st_pos = bar_space
+            st_pos = hue_space
             for h_fc_idx in range(len(xlabels[axis_idx+1])):
                 sum_this_hue_bar = xlabels[axis_idx+1][h_fc_idx].hold_space
-                pos[axis_idx] += [st_pos+width*(i+0.5) for i in range(sum_this_hue_bar)]
-                st_pos += (sum_this_hue_bar*width+bar_space)
+                pos[axis_idx] += [st_pos+width*(i+0.5)+bar_space*i for i in range(sum_this_hue_bar)]
+                st_pos += (sum_this_hue_bar*width+(sum_this_hue_bar-1)*bar_space+hue_space)
         else:
             st_pos = 0
             for fc_idx in range(len(xlabels[axis_idx])):
                 this_hue_per = xlabels[axis_idx][fc_idx].hold_space / df.shape[0]
                 pos[axis_idx].append(st_pos+this_hue_per/2)
                 st_pos += this_hue_per
     return xlabels, pos
 
 def plot_bar(factors:List[str], tags:List[str], df:pd.DataFrame, **kwargs):
     """
     Stack bar plot with hue style
 
     Args:
-        factors (List[str]): A list of factors. [low_lever_factor, medium_lever_factor, ...] or just one.
-        tags (List[str]): A list of tags. [stack_low_y, stack_medium_y, ...] or just one.
-        df (pd.DataFrame): A pandas DataFrame. From pro_bar_data or sort_df_factors.
-        **kwargs: Additional keyword arguments.
-            width = 0.4\n
-            bar_space = 0.2\n
-            xrotations = [0]*len(factors)\n
-            colors = plt.rcParams['axes.prop_cycle'].by_key()['color']\n
-            hatchs:['-', '+', 'x', '\\', '*', 'o', 'O', '.'],\n
-            labels:None,\n
-            font_size:None, \n
-            offset = [(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))]\n
-            err = None\n
-            err_kwargs = {'capsize':5, 'capthick':2, 'elinewidth':2, 'fmt':' k'}
+        - factors (List[str]): A list of factors. [low_lever_factor, medium_lever_factor, ...] or just one.
+        - tags (List[str]): A list of tags. [stack_low_y, stack_medium_y, ...] or just one.
+        - df (pd.DataFrame): A pandas DataFrame. From `pro_bar_data` or `sort_df_factors`.
+        - kwargs: Additional keyword arguments.
+            - fig = None
+            - jitter = Flase, IF True, pass the original df, the func will call `pro_bar_data` internally.
+            - jitter_kwargs = {'size': 10, 'alpha': 0.5, 'color': None}
+            - width = 0.4
+            - bar_space = 0.05
+            - hue_space = 0.2
+            - xrotations = [0]*len(factors)
+            - colors = plt.rcParams['axes.prop_cycle'].by_key()['color']
+            - hatchs:['-', '+', 'x', '\\', '*', 'o', 'O', '.'],
+            - font_size:None,
+            - labels:None,
+            - offset = [None] + [(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors)-1)], x-axis offset
+            - xticks_pad: [5 for _ in range(len(factors)+1)], x-axis label pad from x-axis
+            - edgecolor:['white'] * len(tags),
+            - linewidth: 0,
+            - err: (str|np.array), if str, will use df[err] as yerr. if np.array, will use it directly. will multiply 1.96 to yerr.
+            - err_kwargs = {'capsize':5, 'capthick':2, 'elinewidth':2, 'fmt':' k', 'ecolor':'black'}
 
     Returns:
-        np.array: An array of positions.
-        ax1: An axis object.
+        - np.array: An array of positions.
+        - ax1: An axis object.
+        - df: If `jitter` is True, return the processed df.
+        
+    Notes:
+        - the `FIRST factor` will be the `LOWEST level x-axis`.
+        - y-axis tick labels' fontsize will be set same as first level's x-axis tick labels' fontsize.
     """
-    ax1 = host_subplot(111, axes_class=axisartist.Axes)
-    
+    # process args
     if len(tags) == 0:
+        # TODO: 可能存在'Unbond: 0'等其他情况
         tags = list(df.columns)[len(factors):]
-    args = get_wanted_args({'width':0.4, 'bar_space':0.2, 'xrotations':[0]*len(factors),
+    args = get_wanted_args({'fig': None,
+                            'jitter':False,
+                            'jitter_kwargs': {'size': 10, 'alpha': 0.5, 'color': None},
+                            'width':0.4, 'hue_space':0.2, 'bar_space':0.05,
+                            'xrotations':[0]*len(factors),
                             'colors':plt.rcParams['axes.prop_cycle'].by_key()['color'],
                             'hatchs':['-', '+', 'x', '\\', '*', 'o', 'O', '.'],
                             'font_size':None,
                             'labels':None,
-                            'offset':[(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))],
-                            'edgecolor':'white',
+                            'offset':[None] + [(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))],
+                            'xticks_pad':[5 for _ in range(len(factors)+1)],
+                            'edgecolor':['white'] * len(tags),
+                            'linewidth': 0,
+                            'log': False,
                             'err':None,
-                            'err_kwargs':{'capsize':5, 'capthick':2, 'elinewidth':2, 'fmt':' k'}},
+                            'err_kwargs':{'capsize':5, 'capthick':2, 'elinewidth':2, 'fmt':' k', 'ecolor':'black'}},
                             kwargs)
     args.xrotations.append(0)
-    xlabels, pos = pro_hue_pos(factors, df, args.width, args.bar_space)
+    # make first level axis
+    ax1 = host_subplot(111, axes_class=axisartist.Axes, figure=args.fig)
+    # plot jitter using seaborn
+    if args.jitter:
+        jittor_color = args.jitter_kwargs['color']
+        del args.jitter_kwargs['color']
+        @pro_bar_data_R(factors[::-1], tags, df, ['', '_SE', '_N', '_V'])
+        def pro_bar_jitter_data(v):
+            if v.shape[0] > 1:
+                se = v.std(ddof = 1)/np.sqrt(v.shape[0])
+            else:
+                se = np.NaN
+            return [v.mean(), se, v.shape[0], v]
+        df = pro_bar_jitter_data()
+    # make xlabels and positions
+    xlabels, pos = pro_hue_pos(factors, df, args.width, args.hue_space, args.bar_space)
+    # plot bar
     bottom = kwargs['bottom'] if 'bottom' in kwargs else np.zeros(len(pos[0]))
-    
     for yIdx, yName in enumerate(tags):
-        if args.labels is not None:
-            label = args.labels[yIdx]
-        else:
-            label = yName
+        # label
+        label = args.labels[yIdx] if (args.labels and args.labels[yIdx] is not None) else yName
+        # add jitter
+        if args.jitter:
+            for i, (n, y) in enumerate(zip(df[yName+'_N'], df[yName+'_V'])):
+                x = [pos[0][i]] * n
+                color = jittor_color[yIdx][i] if jittor_color is not None else 'black'
+                sns.stripplot(x=x, y=y.reshape(-1), ax=ax1, jitter=True, native_scale=True,
+                              color=color, zorder = 1, legend = False, **args.jitter_kwargs)
+        # plot bar
         ax1.bar(pos[0], df[yName], width = args.width, bottom = bottom, label=label,
-                edgecolor=args.edgecolor, color=args.colors[yIdx])
+                edgecolor=args.edgecolor[yIdx], linewidth = args.linewidth,
+                color=args.colors[yIdx], log = args.log, zorder = 0)
         bottom += df[yName]
-    ax1.set_xlim(0, pos[0][-1]+args.bar_space+args.width/2)
+    ax1.set_xlim(0, pos[0][-1]+args.hue_space+args.width/2)
     ax1.set_xticks(pos[0], [l.name for l in xlabels[0]])
-    plt.setp(ax1.axis["bottom"].major_ticklabels, rotation=args.xrotations[0])
+    plt.setp(ax1.axis["bottom"].major_ticklabels, rotation=args.xrotations[0], pad = args.xticks_pad[0])
     if args.font_size is not None:
         plt.setp(ax1.axis["bottom"].major_ticklabels, fontsize=args.font_size[0])
+        plt.setp(ax1.axis["left"].major_ticklabels, fontsize=args.font_size[0])
     
     axs = []
     for idx, sub_pos in enumerate(pos[1:]):
         axs.append(ax1.twiny())
         axs[-1].set_xticks(sub_pos, [l.name for l in xlabels[idx+1]])
         new_axisline = axs[-1].get_grid_helper().new_fixed_axis
-        axs[-1].axis["bottom"] = new_axisline(loc="bottom", axes=axs[-1], offset=(0, -args.offset[idx]))
-        plt.setp(axs[-1].axis["bottom"].major_ticklabels, rotation=args.xrotations[idx+1])
+        axs[-1].axis["bottom"] = new_axisline(loc="bottom", axes=axs[-1], offset=(0, -args.offset[idx+1]))
+        plt.setp(axs[-1].axis["bottom"].major_ticklabels, rotation=args.xrotations[idx+1], pad = args.xticks_pad[idx+1])
         if args.font_size is not None:
             plt.setp(axs[-1].axis["bottom"].major_ticklabels, fontsize=args.font_size[idx+1])
         axs[-1].axis["top"].major_ticks.set_ticksize(0)
         # TODO : do not work
         axs[-1].axis["right"].major_ticks.set_ticksize(0)
         
     # err bar, put here because errorbar will change ax obj and occur errs
-    if args.err is not None:        
-        ax1.errorbar(pos[0], bottom, yerr=1.96 * args.err, **args.err_kwargs)
+    if args.err is not None:
+        if isinstance(args.err, str):
+            args.err = df[args.err]
+        if 'ecolor' in args.err_kwargs and isinstance(args.err_kwargs['ecolor'], list):
+            err_cols = args.err_kwargs['ecolor']
+            del args.err_kwargs['ecolor']
+            for pos_i, y, err_i, col_i in zip(pos[0], bottom, args.err, err_cols):
+                ax1.errorbar(pos_i, y, yerr=1.96 * err_i, zorder = 2, ecolor = col_i, **args.err_kwargs)
+        else:
+            ax1.errorbar(pos[0], bottom, yerr=1.96 * args.err, zorder = 2, **args.err_kwargs)
     
-    return np.array(pos[0]), ax1
+    if args.jitter:
+        return np.array(pos[0]), ax1, df
+    else:
+        return np.array(pos[0]), ax1
 
 def plot_positional_hue(factors:List[str], tags:List[str], df:pd.DataFrame, **kwargs):
     """
     wrapper\n
     support args: width, bar_space, xrotations, colors, offset, bottom\n
     xlabels is in margs
     @plot_positional_hue(['solution', 'type'], ['root', 'leaf'], ndf)\n
@@ -224,14 +300,45 @@
                 axs[-1].axis["top"].major_ticks.set_ticksize(0)
                 # TODO : do not work
                 axs[-1].axis["right"].major_ticks.set_ticksize(0)            
             return np.array(pos[0]), ax1
         return core_wrapper
     return ret_wrapper
 
+def calcu_swarm_pos(x: float, y: np.ndarray, width: float, d: Optional[float] = None):
+    """
+   This function calculates the x-coordinates for the data points in a swarm plot.
+   The x-coordinates are calculated based on the given x-coordinate, y-coordinates,
+   and width of the swarm. If d is not None, it will be used as the distance between
+   the data points. Otherwise, it will be calculated based on the number of data points.
+   
+    Parameters:
+        - x: the x-coordinate of the center of the swarm.
+        - y: the y-coordinates of the data points.
+        - width: the width of the swarm.
+        - d: the distance between the data points. If None, it will be calculated based on the number of data points.
+        
+    Returns:
+        - A numpy array of x-coordinates for the data points.
+    """
+    def _calcu_arithmetic(x, n, w, d):
+        if isinstance(d, float) or isinstance(d, int):
+            a0 = x - (n-1)*d/2
+            return np.linspace(a0, a0+d*(n-1), n)
+        if n == 1:
+            return x
+        else:
+            a0, d = x-w/2, w/(n-1)
+            return np.linspace(a0, a0+d*(n-1), n)
+    ret = np.zeros(len(y))
+    for y_u in np.unique(y):
+        y_idx = np.where(y == y_u)[0]
+        ret[y_idx] = _calcu_arithmetic(x, len(y_idx), width, d)
+    return ret
+
 def qqplot(tags:List[str], df:pd.DataFrame, figsize = (12, 6), nrows = 1, ncols = 1, **kwargs):
     """
     Generate a QQ-plot for each column in the given DataFrame.
 
     Parameters:
         tags (List[str]): A list of column names to generate QQ-plots for.
         df (pd.DataFrame): The DataFrame containing the data.
@@ -274,14 +381,34 @@
     Returns:
         None
     """
     plt.tight_layout()
     plt.gcf().savefig(path, dpi=dpi, bbox_inches = bbox_inches)
     plt.show()
     
+def plot_stats_star(x1: float, x2: float, h: float, endpoint: float, p_value: float,
+                    ax = plt, p2star: Callable[[float], str] = p_value_to_stars):
+    """
+    Params
+        - x1: The x-coordinate of the left endpoint.
+        - x2: The x-coordinate of the right endpoint.
+        - h: The y-coordinate of the horizontal line.
+        - endpoint: The height of the endpoint.
+        - p_value: The p-value of the difference.
+        - ax: The `Axes` instance to plot on. Default is `plt`.
+        - p2star: A function that converts a p-value to a string of stars. Default is `p_value_to_stars`.
+
+    Returns:
+        None
+    """
+    ax.plot([x1, x2], [h, h], color='black')
+    ax.plot([x1, x1], [h, h-endpoint], color='black')
+    ax.plot([x2, x2], [h, h-endpoint], color='black')
+    ax.text((x1+x2)/2, h, p2star(p_value), ha='center')    
+    
 def plot_turkey(means, std_errs, tukey_results, min_star = 1):
     """
     Plot a bar chart showing the means of different groups along with the standard errors.
 
     Parameters:
         - means: A list of mean values for each group.
         - std_errs: A list of standard errors for each group.
@@ -310,24 +437,26 @@
                      p_value_to_stars(tukey_results.pvalues[i]), ha='center')
             height += min_height
 
     plt.xticks(x, tukey_results.groupsunique)
     return plt.gca()
 
 if __name__ == '__main__':
-    """dev code"""
+    # dev code
     df = pd.read_excel('./data/plot.xlsx', sheet_name='MWM')
     df['Animal Type'] = df['Animal Type'].astype('str')
     model = mst.multicomp_turkeyHSD({'Animal Type':[]}, 'Duration', df)
     result = mst.turkey_to_table(model)
     print(result)
-    sub_df = get_df_data({'Animal Type':[]}, ['Duration'], df)
-    sub_df = pro_bar_data(['Animal Type'], ['Duration'], sub_df)
+    # sub_df = get_df_data({'Animal Type':[]}, ['Duration'], df)
+    sub_df = pro_bar_data(['Animal Type'], ['Duration'], df)
     # test err
-    plot_bar(['Animal Type'], ['Duration'], sub_df, err = sub_df['Duration_SE'])
+    cols = get_palette(n = 4, mode = 'hls')
+    plot_bar(['Animal Type'], ['Duration'], df, err = sub_df['Duration_SE'], jitter = True,
+             edgecolor = [cols], linewidth = 5, colors = ['white'], jitter_kwargs = {'size': 10, 'alpha': 1, 'color': [cols]})
     plt.show()
     plot_turkey(sub_df['Duration'], sub_df['Duration_SE'], model)
     plt.show()
     
     df = pd.DataFrame({'Month': [5, 5, 6, 6, 7, 7, 8, 8, 9, 9],
                        'Ozone': [23.61538, 22.22445, 29.44444, 18.20790, 59.11538, 31.63584, 59.96154, 39.68121, 31.44828, 24.14182]})
     model = mst.multicomp_turkeyHSD({'Month':[]}, 'Ozone', df)
```

### Comparing `mbapy-0.7.1b1/mbapy/sci_utils/paper_download.py` & `mbapy-0.7.2/mbapy/sci_utils/paper_download.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/sci_utils/paper_parse.py` & `mbapy-0.7.2/mbapy/sci_utils/paper_parse.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/sci_utils/paper_search.py` & `mbapy-0.7.2/mbapy/sci_utils/paper_search.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/scripts/avif.py` & `mbapy-0.7.2/mbapy/scripts/avif.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/scripts/cluster.py` & `mbapy-0.7.2/mbapy/scripts/cluster.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/scripts/cnipa.py` & `mbapy-0.7.2/mbapy/scripts/cnipa.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/scripts/cp.py` & `mbapy-0.7.2/mbapy/scripts/cp.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/scripts/duitang.py` & `mbapy-0.7.2/mbapy/scripts/duitang.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/scripts/extract-dir.py` & `mbapy-0.7.2/mbapy/scripts/extract-dir.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/scripts/extract_paper.py` & `mbapy-0.7.2/mbapy/scripts/extract_paper.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/scripts/mass.py` & `mbapy-0.7.2/mbapy/scripts/hplc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,161 +1,173 @@
 import argparse
 import glob
 import os
 from pathlib import Path
 from typing import Dict, List
 
+import scipy
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 
 os.environ['MBAPY_AUTO_IMPORT_TORCH'] = 'False'
 os.environ['MBAPY_FAST_LOAD'] = 'True'
-from mbapy import base, file
+from mbapy.base import put_err
 from mbapy.plot import get_palette, save_show
 
 if __name__ == '__main__':
-    from mbapy.scripts._script_utils_ import clean_path
+    from mbapy.file import get_paths_with_extension, get_valid_file_path
+    from mbapy.scripts._script_utils_ import clean_path, show_args
 else:
-    from ._script_utils_ import clean_path
+    from ..file import get_paths_with_extension, get_valid_file_path
+    from ._script_utils_ import clean_path, show_args
 
 
-def plot_mass_load_file(path: Path):
+def plot_hplc_load_arw_file(path: Path):
     lines = path.read_text().splitlines()
-    df = pd.DataFrame([line.split('\t') for line in lines[1:]],
-                        columns = lines[0].split('\t'))
-    if df.shape[1] == 2 and df.columns[0] == 'Time':
-        return df.astype(float)
-    elif df.shape[1] == 10:
-        return df.astype({'Mass/Charge':float, 'Height':float, 'Charge':int,
-                            'Monoisotopic':str, 'Mass (charge)':str,
-                            'Mass/charge (charge)':str})
-
-def plot_mass_plot_basepeak(name:str, base_peak: pd.DataFrame, args):
-    fig, ax = plt.subplots(figsize=(8, 6))
-    ax.plot(base_peak['Time'], base_peak['Intensity'], color = args.color)
+    info_df = pd.DataFrame([lines[1].split('\t')], columns = lines[0].split('\t'))
+    data_df = pd.DataFrame([line.split('\t') for line in lines[2:]],
+                           columns = ['Time', 'Absorbance'])
+    return info_df, data_df.astype({'Time': float, 'Absorbance': float})
+    
+def plot_hplc_plot_waters(file_name:str, info_df: pd.DataFrame, data_df: pd.DataFrame, args):
+    fig, ax = plt.subplots(figsize=(10, 6))
+    xlim = args.xlim.split(',')
+    if isinstance(info_df, pd.DataFrame):
+        au_units = info_df['"检测单位"'][0].replace('"', '')
+        xlim = [float(xlim[0]), data_df['Time'].max() if xlim[1] == 'None' else float(xlim[1])]
+        ax.plot(data_df['Time'], data_df['Absorbance'], color = args.color, label = info_df[''])
+    else:
+        au_units = info_df[0]['"检测单位"'][0].replace('"', '')
+        xlim_max = data_df[0]['Time'].max()
+        for label, info_df_i, data_df_i in zip(args.file_labels, info_df, data_df):
+            label_string, color = label
+            ax.plot(data_df_i['Time'], data_df_i['Absorbance'], color = color, label = label_string)
+            xlim_max = max(xlim_max, data_df_i['Time'].max())
+        xlim = [float(xlim[0]), xlim_max if xlim[1] == 'None' else float(xlim[1])]
     plt.xticks(size = 20)
     plt.yticks(size = 20)
-    plt.yscale('log')
-    ax.set_title(f'{name} (TIC of TOF MS)', fontsize=25)
     ax.set_xlabel('Time (min)', fontsize=25)
-    ax.set_ylabel('Intensity (cps)', fontsize=25)
-    save_show(os.path.join(args.output, f'{name}.png'), dpi = 300)
-
-def plot_mass_plot_peaklist(name:str, peak_list: pd.DataFrame, args):
-    def plot_vlines(x, y, col, label = ''):
-        plt.vlines(x, 0, y, colors = [col] * len(x), label = label)
-        plt.scatter(x, y, c = col)
-    fig, ax = plt.subplots(figsize=(8, 6))
-    idx = peak_list['Monoisotopic'] == 'Yes'
-    plot_vlines(peak_list['mass_data'], peak_list['Height'], args.color)
-    labels_ms = np.array(list(args.labels.keys()))
-    for ms, h, c in zip(peak_list['mass_data'][idx], peak_list['Height'][idx],
-                        peak_list['Charge'][idx]):
-        matched = np.where(np.abs(labels_ms - ms) < args.labels_eps)[0]
-        if matched.size > 0:
-            label, color = args.labels.get(labels_ms[matched[0]])
-            plot_vlines([ms], [h], color, label)
-            ax.text(ms, h, f'* {ms:.2f}({c:d})', fontsize=15, color = color)
-        else:
-            ax.text(ms, h, f'* {ms:.2f}({c:d})', fontsize=15, color = args.color)
-    plt.xticks(size = 20)
-    plt.yticks(size = 20)
-    plt.yscale('log')
-    axis_lim = (1-args.expand, 1+args.expand)
-    plt.xlim(peak_list['mass_data'].min() * axis_lim[0], peak_list['mass_data'].max() * axis_lim[1])
-    plt.ylim(peak_list['Height'].min() * axis_lim[0], peak_list['Height'].max() * axis_lim[1])
-    ax.set_title(f'{name} (Peak List of TOF MS)', fontsize=25)
-    ax.set_xlabel(f'Mass{"" if args.mass else "/charge"}', fontsize=25)
-    ax.set_ylabel('Intensity (cps)', fontsize=25)
-    plt.legend(fontsize=15)
-    save_show(os.path.join(args.output, f'{name}.png'), dpi = 300)
+    ax.set_ylabel(f'Absorbance ({au_units})', fontsize=25)
+    ax.set_xlim(xlim[0], xlim[1])
+    plt.legend(fontsize=15, loc = args.legend_pos, bbox_to_anchor = (args.legend_pos_bbox1, args.legend_pos_bbox2))
+    save_show(os.path.join(args.output, f'{file_name} absorbance.png'), dpi = 600)
     
-def plot_mass(args):           
+def plot_hplc(args):           
     # process args
-    args.dir = clean_path(args.dir)
-    print(f'get arg: dir: {args.dir}')
-    # find base peak file and peak list file
-    paths = glob.glob(os.path.join(args.dir, '*.txt'))
-    dfs = {path:plot_mass_load_file(Path(path)) for path in paths}
-    dfs = {k:v for k,v in dfs.items() if v is not None}
-    if not dfs:
-        raise FileNotFoundError(f'can not find two files in {args.dir}')
+    args.input = clean_path(args.input)
+    args.output = clean_path(args.output) if args.output else args.input
     if not os.path.isdir(args.output):
         print(f'given output {args.output} is a file, change it to parent dir')
         args.output = args.output.parent
-    print(f'get arg: output: {args.output}')
-    print(f'get arg: mass: {args.mass}')
+    # labels
     labels, colors = {}, get_palette(len(args.labels.split(';')), mode = 'hls')
     for idx, i in enumerate(args.labels.split(';')):
-        pack = i.split(',')
-        mass, label, color = pack[0], pack[1], pack[2] if len(pack) == 3 else colors[idx]
-        labels[float(mass)] = [label, color]
+        if i:
+            pack = i.split(',')
+            mass, label, color = pack[0], pack[1], pack[2] if len(pack) == 3 else colors[idx]
+            labels[float(mass)] = [label, color]
     args.labels = labels
-    print(f'get arg: labels: {labels}')
+    # file labels
+    file_labels, colors = [], get_palette(len(args.file_labels.split(';')), mode = 'hls')
+    for idx, i in enumerate(args.file_labels.split(';')):
+        if i:
+            pack = i.split(',')
+            label, color = pack[0], pack[1] if len(pack) == 2 else colors[idx]
+            file_labels.append([label, color])
+    args.file_labels = file_labels
+    # find base peak file and peak list file
+    if args.system == 'waters':
+        paths = get_paths_with_extension(args.input, ['arw'], recursive=args.recursive)
+        load_data = plot_hplc_load_arw_file
+    else:
+        raise NotImplementedError(f'not support HPLC system: {args.system}')
+    dfs = {path:load_data(Path(path)) for path in paths}
+    dfs = {k:v for k,v in dfs.items() if v is not None}
+    if not dfs:
+        raise FileNotFoundError(f'can not find data files in {args.input}')
+    # show args
+    show_args(args, ['input', 'system', 'recursive', 'merge', 'output', 'min_peak_width',
+                     'colors', 'labels', 'file_labels', 'labels_eps', 'xlim', 'expand',
+                     'legend_pos', 'legend_pos_bbox1', 'legend_pos_bbox2'])
     # show data general info and output peak list DataFrame
-    for n,df in dfs.items():
-        name = Path(n).resolve().stem
-        print(f'\n\n\n\n\n{name}: peak list: signal(s):\n', df)
-        df.to_csv(os.path.join(args.output, f'{name}.csv'))
-        # process Mass (charge) and identify mass
-        if df.shape[1] == 10:
-            df['Mass (charge)'] = df['Mass (charge)'].str.extract(r'(\d+\.\d+)', expand=False).astype(float)
-            df['Mass/charge (charge)'] = df['Mass/charge (charge)'].str.extract(r'(\d+\.\d+)', expand=False).astype(float)
-            df['mass_data'] = df['Mass (charge)'] if args.mass else df['Mass/charge (charge)']
-            drop_idx = df[df['Height'] < args.min_height].index
-            if not drop_idx.empty:
-                print(f'drop data with min-height: {args.min_height} and only these data remained:\n',
-                      df[df['Height'] >= args.min_height])
-                df.drop(drop_idx, axis = 0, inplace = True)
-    # plot each df
-    for n,df in dfs.items():
-        name = Path(n).resolve().stem
-        if df.shape[1] == 2:
-            # plot base peak
-            print(f'ploting base peak: {name}')
-            plot_mass_plot_basepeak(name, df, args)
-        elif df.shape[0] > 0: # avoid drop all data but still draw
-            # plot peak list
-            print(f'ploting peak list: {name}')
-            plot_mass_plot_peaklist(name, df, args)
+    if args.merge:
+        if args.system == 'waters':
+            dfs = list(dfs.values())
+            info_df, data_df = [d[0] for d in dfs], [d[1] for d in dfs]
+            plot_hplc_plot_waters('merge', info_df, data_df, args)
+    else:
+        for path, df in dfs.items():
+            path = Path(path).resolve()
+            # plot each df
+            if args.system == 'waters':
+                info_df, data_df = df
+                # output csv
+                sample_name, sample_time, sample_channle = info_df['"样品名称"'][0], info_df['"采集日期"'][0], info_df['"通道"'][0]
+                csv_name = f'{sample_name} - {sample_time} - {sample_channle}'.replace('"', '')
+                csv_name = get_valid_file_path(csv_name.replace('/', '-'), valid_len=500).replace(':', '-')
+                info_df.to_csv(str(path.parent / get_valid_file_path(csv_name + ' - info.csv')))
+                data_df.to_csv(str(path.parent / get_valid_file_path(csv_name + ' - data.csv')))
+                # plot
+                print(f'plot {path.stem}: {csv_name}')
+                print(info_df.T)
+                plot_hplc_plot_waters(csv_name, info_df, data_df, args)
+
 
 _str2func = {
-    'plot-mass': plot_mass,
+    'plot-hplc': plot_hplc,
 }
 
 
 def main(sys_args: List[str] = None):
     args_paser = argparse.ArgumentParser()
     subparsers = args_paser.add_subparsers(title='subcommands', dest='sub_command')
     
-    plot_mass_args = subparsers.add_parser('plot-mass', description='plot mass spectrum')
-    # set dir argument
-    plot_mass_args.add_argument("-d", "--dir", type = str, help="txt file directory")
+    plot_hplc_args = subparsers.add_parser('plot-hplc', description='plot hplc spectrum')
+    # set input file argument
+    plot_hplc_args.add_argument("-i", "--input", type = str, default='.',
+                                help="data file directory, default is %(default)s.")
+    plot_hplc_args.add_argument("-s", "--system", type = str, default='waters',
+                                help="HPLC system. Default is %(default)s, only accept arw file exported by Waters.")
+    plot_hplc_args.add_argument('-r', '--recursive', action='store_true', default=False,
+                                help='search input directory recursively, default is %(default)s.')
+    plot_hplc_args.add_argument('-merge', action='store_true', default=False,
+                                help='merge multi files into one plot, default is %(default)s.')
     # set output file argument
-    plot_mass_args.add_argument("-o", "--output", type = str, default='.',
-                                help="output file dir or path, default is %(default)s")
+    plot_hplc_args.add_argument("-o", "--output", type = str, default=None,
+                                help="output file dir or path. Default is %(default)s, means same as input dir")
     # set draw argument
-    plot_mass_args.add_argument('-m', '--mass', action='store_true', default=False,
-                                help='draw Mass instead of Mass/charge which is Mass+z, default is %(default)s')
-    plot_mass_args.add_argument('-min', '--min-height', type = int, default=0,
-                                help='filter data with min height, default is %(default)s')
-    plot_mass_args.add_argument('-col', '--color', type = str, default='black',
-                                help='draw color, default is %(default)s')
-    plot_mass_args.add_argument('-labels', '--labels', type = str, default='',
-                                help='labels, input as 1000,Pep1;1050,Pep2, default is %(default)s')
-    plot_mass_args.add_argument('--labels-eps', type = float, default=0.5,
-                                help='eps to recognize labels, default is %(default)s')
-    plot_mass_args.add_argument('-expand', '--expand', type = float, default=0.2,
-                                help='how much the x-axis and y-axisto be expanded, default is %(default)s')
+    plot_hplc_args.add_argument('--min-peak-width', type = float, default=4,
+                                help='filter peaks with min width in hplc/Charge plot, default is %(default)s.')
+    plot_hplc_args.add_argument('-xlim', type = str, default='0,None',
+                                help='set x-axis limit, input as "0,15", default is %(default)s.')
+    plot_hplc_args.add_argument('-cols', '--colors', type = str, default='black',
+                                help='draw color, default is %(default)s.')
+    plot_hplc_args.add_argument('-labels', '--labels', type = str, default='',
+                                help='labels, input as 1000,Pep1;1050,Pep2, default is %(default)s.')
+    plot_hplc_args.add_argument('-flabels', '--file-labels', type = str, default='',
+                                help='labels, input as 228,blue;304,red, default is %(default)s.')
+    plot_hplc_args.add_argument('--labels-eps', type = float, default=0.5,
+                                help='eps to recognize labels, default is %(default)s.')
+    plot_hplc_args.add_argument('-expand', '--expand', type = float, default=0.2,
+                                help='how much the x-axis and y-axisto be expanded, default is %(default)s.')
+    plot_hplc_args.add_argument('-lpos', '--legend-pos', type = str, default='upper center',
+                                help='legend position, can be string as "upper center", or be float as 0.1,0.2, default is %(default)s')
+    plot_hplc_args.add_argument('-lposbbox1', '--legend-pos-bbox1', type = float, default=1.1,
+                                help='legend position bbox 1 to anchor, default is %(default)s')
+    plot_hplc_args.add_argument('-lposbbox2', '--legend-pos-bbox2', type = float, default=1,
+                                help='legend position bbox 2 to anchor, default is %(default)s')
 
     
     args = args_paser.parse_args(sys_args)
     
     if args.sub_command in _str2func:
         print(f'excuting command: {args.sub_command}')
         _str2func[args.sub_command](args)
     else:
-        base.put_err(f'no such sub commmand: {args.sub_command}')
+        put_err(f'no such sub commmand: {args.sub_command}')
 
 if __name__ == "__main__":
+    # dev code, MUST COMMENT OUT BEFORE RELEASE
+    # pass
+    
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mbapy-0.7.1b1/mbapy/scripts/mv.py` & `mbapy-0.7.2/mbapy/scripts/mv.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/scripts/peptide.py` & `mbapy-0.7.2/mbapy/scripts/peptide.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 
 os.environ['MBAPY_AUTO_IMPORT_TORCH'] = 'False'
 os.environ['MBAPY_FAST_LOAD'] = 'True'
 from mbapy import base, file
 from mbapy.bio.peptide import AnimoAcid, Peptide
 
 if __name__ == '__main__':
-    from mbapy.scripts._script_utils_ import clean_path
+    from mbapy.scripts._script_utils_ import clean_path, show_args
 else:
-    from ._script_utils_ import clean_path
+    from ._script_utils_ import clean_path, show_args
 
 
-def calcu_substitution_value(args):
+def calcu_substitution_value(args: argparse.Namespace):
     """
     Calculates the substitution value and plots a scatter plot with a linear 
     regression model. The function first processes the input arguments to 
     convert the strings to float values and stores them in arrays. It then 
     calculates the average substitution value and prints it on the console. 
     Next, the function fits a linear regression model to the data using the 
     LinearRegression class from scikit-learn and calculates the equation 
@@ -63,15 +63,15 @@
     plt.yticks(size = 20)
     ax.set_title(f'Avg Substitution Value: {mean_subval:.5f}', fontsize=25)
     ax.set_xlabel('Weight of Resin (mg)', fontsize=25)
     ax.set_ylabel('OD (304 nm)', fontsize=25)
     plt.show()
 
 
-def calcu_mw(args, _print = print):
+def calcu_mw(args: argparse.Namespace, _print = print):
     """
     Calculates the molecular weight (MW) of a peptide based on its amino acid sequence and a dictionary of weights for each amino acid.
 
     Args:
         args (Namespace): An object containing the command line arguments.
         _print (function, optional): A function used for printing. Defaults to the built-in print function.
 
@@ -105,24 +105,24 @@
     C_protect_deletion: bool = True # whether delete C-terminal protect group can be performed
     R_protect_deletion: bool = True # whether delete R-terminal protect group can be performed
     
     def copy(self):
         return MutationOpts(self.AA_deletion, self.AA_repeat, self.N_protect_deletion,
                             self.C_protect_deletion, self.R_protect_deletion)
     
-    def check_empty(self, _pos: List[int], seq: Peptide):
+    def check_empty(self, _pos: List[int], seq: Peptide, args: argparse.Namespace):
         """
         return list of signals which is able to opt, if empty, the lis is also empty.
         """
         pos, repeat_pos, sum_repeat = _pos
         able = []
         if pos >= len(seq.AAs):
             return []
         if sum_repeat == 1:
-            if self.AA_deletion:
+            if self.AA_deletion and not args.disable_aa_deletion:
                 able.append('AA_deletion')
             if self.AA_repeat > 0:
                 able.append('AA_repeat')
             if seq.AAs[pos].N_protect != 'H' and self.N_protect_deletion:
                 able.append('N_protect_deletion')
             if seq.AAs[pos].C_protect != 'OH' and self.C_protect_deletion:
                 able.append('C_protect_deletion')
@@ -198,36 +198,36 @@
         elif sum_repeat > 1 and getattr(tree.mutate.seq.AAs[pos][repeat_pos], f'{NCR}_protect') != null_pg:
             setattr(tree.mutate.seq.AAs[pos][repeat_pos], f'{NCR}_protect', null_pg)
         # trun off the opts in two branches
         setattr(tree.mutate.opts, f'{NCR}_protect_deletion', False)
         setattr(tree.remain.opts, f'{NCR}_protect_deletion', False)
         return tree
                 
-    def perform_one(self, tree: 'MutationTree', max_repeat: int):
+    def perform_one(self, tree: 'MutationTree', args: argparse.Namespace):
         """
         Perform ONE mutation opt left in tree.opts, return this tree. Also check if it is a repeated AA.
         If it is a repeated AA depend on tree.pos[2], skip AA deletion and AA repeat.
             - If no opts left to do:
                 - let two brance still be None.
                 - return the tree.
             - IF HAS:
                 - generate two branch, change branches' father
                 - perform mutation in mutate branch
                 - trun off opts in two branches
                 - move pos ONLY in mutate branch.
                 - DO NOT CHECK IF MEETS END in both this dot and two branches.
                 - return the tree.
         """
-        able = tree.opts.check_empty(tree.pos, tree.seq)
+        able = tree.opts.check_empty(tree.pos, tree.seq, args)
         if able:
             # generate two branch
             tree.generate_two_branch()
             # perform mutation
             if 'AA_deletion' in able:
-                tree = self.delete_AA(tree, max_repeat)
+                tree = self.delete_AA(tree, args.max_repeat)
             elif 'AA_repeat' in able:
                 tree = self.repeat_AA(tree)
             elif 'N_protect_deletion' in able:
                 tree = self.delete_NCR(tree, 'N')
             elif 'C_protect_deletion' in able:
                 tree = self.delete_NCR(tree, 'C')
             elif 'R_protect_deletion' in able:
@@ -309,37 +309,37 @@
                 # move to next repeat AA
                 self.pos[1] += 1
             # reset opts to full
             self.opts = MutationOpts(AA_repeat = max_repeat)
             return True
         return False
         
-def mutate_peptide(tree: MutationTree, max_repeat: int):
+def mutate_peptide(tree: MutationTree, args: argparse.Namespace):
     """
     Parameters:
         - mutations: Tree object, store all mutations and there relationship.
         - max_repeat: int
     """
     # perofrm ONE mutation
-    tree = tree.opts.perform_one(tree, max_repeat)
+    tree = tree.opts.perform_one(tree, args)
     # if NO mutaion can be done, 
     if tree.mutate is None and tree.remain is None:
         # try move current AA in this tree to next AA
-        if tree.move_to_next(max_repeat):
+        if tree.move_to_next(args.max_repeat):
             # move success, go on
-            mutate_peptide(tree, max_repeat)
+            mutate_peptide(tree, args)
         else:
             # it is the end, return tree
             return tree
     else: # go on with two branches
-        mutate_peptide(tree.mutate, max_repeat)
-        mutate_peptide(tree.remain, max_repeat)
+        mutate_peptide(tree.mutate, args)
+        mutate_peptide(tree.remain, args)
     return tree
 
-def calcu_mw_of_mutations(args):
+def calcu_mw_of_mutations(args: argparse.Namespace):
     """
     Calculates the molecular weight of mutations based on the given arguments.
 
     Args:
         args (object): An object that contains the following attributes:
             - seq (str): The input sequence.
             - weight (bool): If True, the weight of the peptide will be calculated instead of the mass.
@@ -374,26 +374,23 @@
         if os.path.isdir(args.out):
             file_name = file.get_valid_file_path(" ".join(sys.argv[1:]))+'.txt'
             args.out = os.path.join(args.out, file_name)
         f = open(args.out, 'w')
     else:
         f = None
     # show args
-    _print(f'get arg: seqeunce: {args.seq}', f)
-    _print(f'get arg: weight: {args.weight}', f)
-    _print(f'get arg: max-repeat: {args.max_repeat}', f)
-    _print(f'get arg: out: {args.out}', f)
-    _print(f'get arg: mass: {args.mass}', f)
+    show_args(args, ['seq', 'weight','max_repeat', 'disable_aa_deletion', 'out','mass'],
+              printf = lambda x : _print(x, f))
     # show mother peptide info
     peptide, expand_mw_dict = calcu_mw(args, _print = lambda x : _print(x, f))
     # calcu mutations
     all_mutations = MutationTree(peptide=peptide, seq=peptide.copy(),
                                  opts=MutationOpts(AA_repeat=args.max_repeat),
                                  pos=[0, 0, 1])
-    all_mutations = mutate_peptide(all_mutations, args.max_repeat)
+    all_mutations = mutate_peptide(all_mutations, args)
     all_mutations = all_mutations.extract_mutations()
     mw2pep, peps = {}, {}
     for pep in all_mutations:
         if len(pep.AAs):
             pep_repr = str(pep)
             if pep_repr not in peps:
                 peps[pep_repr] = len(peps)
@@ -498,14 +495,16 @@
     mutationweight = subparsers.add_parser('mutationweight', aliases = ['mutation-weight', 'mmw'], description='calcu MW of each peptide mutations syn by SPPS.')
     mutationweight.add_argument('-s', '--seq', '--seqeunce', '--pep', '--peptide', type = str,
                                 help='peptide seqeunce, input as Fmoc-Cys(Acm)-Leu-OH or H-Cys(Trt)-Leu-OH')
     mutationweight.add_argument('-w', '--weight', type = str, default = '',
                                 help='MW of peptide AAs and protect group, input as Trt-243.34,Boc-101.13 and do not include weight of -H')
     mutationweight.add_argument('--max-repeat', type = int, default = 1,
                                 help='max times for repeat a AA in sequence')
+    mutationweight.add_argument('--disable-aa-deletion', action='store_true', default=False,
+                                help='disable AA deletion in mutations.')
     mutationweight.add_argument('-o', '--out', type = str, default = None,
                                 help='save results to output file/dir. Defaults None, do not save.')
     mutationweight.add_argument('-m', '--mass', action='store_true', default=False,
                                 help='calcu Exact Mass instead of Molecular Weight.')
     
     letters = subparsers.add_parser('letters', aliases = ['transfer-letters'], description='transfer AnimoAcid repr letters width.')
     letters.add_argument('-s', '--seq', '--seqeunce', '--pep', '--peptide', type = str, default='',
```

### Comparing `mbapy-0.7.1b1/mbapy/scripts/reviz.py` & `mbapy-0.7.2/mbapy/scripts/reviz.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/scripts/rm.py` & `mbapy-0.7.2/mbapy/scripts/rm.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/scripts/scihub.py` & `mbapy-0.7.2/mbapy/scripts/scihub.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/scripts/scihub_selenium.py` & `mbapy-0.7.2/mbapy/scripts/scihub_selenium.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/scripts/splash_img.py` & `mbapy-0.7.2/mbapy/scripts/splash_img.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/scripts/video.py` & `mbapy-0.7.2/mbapy/scripts/video.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Date: 2024-02-05 12:03:34
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2024-03-10 10:51:47
+LastEditTime: 2024-03-14 16:21:45
 Description: 
 '''
 import argparse
 import os
 from pathlib import Path
 from typing import Dict, List
 
@@ -170,11 +170,11 @@
     else:
         put_err(f'no such sub commmand: {args.sub_command}')
 
 
 if __name__ == "__main__":
     # dev code
     # comment the following line when release
-    main(['extract', 'frames', '-i', './data_tmp/video.mp4'])
+    # main(['extract', 'frames', '-i', './data_tmp/video.mp4'])
     
     # RELEASE CODE
     main()
```

### Comparing `mbapy-0.7.1b1/mbapy/stats/__init__.py` & `mbapy-0.7.2/mbapy/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/stats/cluster.py` & `mbapy-0.7.2/mbapy/stats/cluster.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/stats/df.py` & `mbapy-0.7.2/mbapy/stats/df.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2023-04-10 20:59:26
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2023-07-10 16:42:29
+LastEditTime: 2024-04-09 14:03:21
 Description: pd.dataFrame utils
 '''
 import itertools
 from functools import wraps
 from typing import Dict, List
 
 import numpy as np
@@ -22,30 +22,29 @@
     from ..base import CDLL, get_dll_path_for_sys, put_err
     from ..file import update_excel
 
 def get_value(df:pd.DataFrame, column:str, mask:np.array)->list:
     return df.loc[mask, column].tolist()
 
 
-# TODO : not use itertools.product
 def pro_bar_data(factors:List[str], tags:List[str], df:pd.DataFrame, **kwargs):
     """
     cacu mean and SE for each combinations of facotors\n
     data should be like this:\n
     | factor1 | factor2 | y1 | y2 |...\n
     |  f1_1   |   f2_1  |2.1 |-2  |...\n
     after process\n
     | factor1 | factor2 | y1(mean) | y1_SE(SE) | y1_N(sum_data) |...\n
     |  f1_1   |   f2_1  |2.1       |   -2      |   32           |...\n
     kwargs:
         min_sample_N:int : min N threshold(>=)
     """
     # kwargs
-    min_sample_N = 1 if 'min_sample_N' not in kwargs else kwargs['min_sample_N']
-    assert min_sample_N > 0, 'min_sample_N <= 0'
+    min_sample_N = kwargs.get('min_sample_N', 1)
+    assert min_sample_N > 0, 'min_sample_N <= 0 !'
     # pro
     if len(tags) == 0:
         tags = list(df.columns)[len(factors):]
     factor_contents:list[list[str]] = [ df[f].unique().tolist() for f in factors ]
     ndf = [factors.copy()]
     for tag in tags:
         ndf[0] += [tag, tag+'_SE', tag+'_N']
@@ -64,34 +63,51 @@
                     line.append(np.NaN)
                 line.append(values.shape[0])
             ndf.append(list(factorCombi) + line)
     return pd.DataFrame(ndf[1:], columns=ndf[0])
 
 def pro_bar_data_R(factors:List[str], tags:List[str], df:pd.DataFrame, suffixs:List[str], **kwargs):
     """
-    wrapper\n
-    @pro_bar_data_R(['solution', 'type'], ['root', 'leaf'], ndf)\n
-    def plot_func(values, **kwargs):
-        return produced vars in list format whose length equal to len(suffix)
+    Params:
+        - factors: list of factors to group by
+        - tags: list of tags to calculate mean and SE for
+        - df: input DataFrame
+        - suffixs: list of suffixes for each tag, used to distinguish different tags with same name
+        - kwargs:
+            - min_sample_N: int, min N threshold(>=)
+            
+    Return:
+        - pd.DataFrame, with each row representing a combination of factors and tags, and columns as follows:
+            - factors: the values of factors
+            - tags: the values of tags, with suffixes
+            - values: the values of tags, calculated by core_func
+            
+    Example
+    >>> @pro_bar_data_R(['solution', 'type'], ['root', 'leaf'], ndf, suffix = ['_mean', '_SE'], min_sample_N=10)\n
+    >>> def pro_func(values):
+    >>>     return produced vars in list format whose length equal to len(suffix)
+    >>> df = pro_func()
     """
     def ret_wrapper(core_func):
         def core_wrapper(**kwargs):
+            min_sample_N = kwargs.get('min_sample_N', 1)
+            assert min_sample_N > 0, 'min_sample_N <= 0 !'
             nonlocal tags
             if len(tags) == 0:
                 tags = list(df.columns)[len(factors):]
             factor_contents:List[List[str]] = [ df[f].unique().tolist() for f in factors ]
             ndf = [factors.copy()]
             for tag in tags:
                 for suffix in suffixs:
                     ndf[0] += [tag+suffix]
             for factorCombi in itertools.product(*factor_contents):
                 factorMask = np.array(df[factors[0]] == factorCombi[0])
                 for i in range(1, len(factors)):
                     factorMask &= np.array(df[factors[i]] == factorCombi[i])
-                if(factorMask.sum() > 0):
+                if factorMask.sum() > min_sample_N:
                     line = []
                     for idx, tag in enumerate(tags):
                         values = np.array(df.loc[factorMask, [tag]])
                         ret_line = core_func(values)
                         assert len(ret_line) == len(suffixs), 'length of return value of core_func != len(suffixs)'
                         line += ret_line
                     ndf.append(list(factorCombi) + line)
```

### Comparing `mbapy-0.7.1b1/mbapy/stats/geography.py` & `mbapy-0.7.2/mbapy/stats/geography.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/stats/test.py` & `mbapy-0.7.2/mbapy/stats/test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2023-04-04 16:45:23
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2023-07-10 16:44:48
+LastEditTime: 2024-04-05 18:19:53
 Description: 
 '''
 from itertools import combinations
 from typing import Dict, List, Optional, Union
 
 import numpy as np
 import pandas as pd
@@ -36,17 +36,17 @@
 
 def _get_x1_x2(x1 = None, x2 = None,
                factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None):
     """以同一列factors提取同一列tag的x1和x2，其余factors仅作筛选作用"""
     if factors is not None and tag is not None and df is not None:
         sub_df = msd.get_df_data(factors, [tag], df)
         fac_name = list(factors.keys())[0]
-        x1 = sub_df.loc[sub_df[fac_name] == factors[fac_name][0], [tag]].values
+        x1 = sub_df.loc[sub_df[fac_name] == factors[fac_name][0], [tag]].values.reshape(-1)
         if len(factors[fac_name]) == 2:
-            x2 = sub_df.loc[sub_df[fac_name] == factors[fac_name][1], [tag]].values
+            x2 = sub_df.loc[sub_df[fac_name] == factors[fac_name][1], [tag]].values.reshape(-1)
         elif len(factors[fac_name]) > 2:
             raise ValueError('Only support 1 or 2 value of factors')
     return x1, x2
 
 def _get_x1_x2_R(x1 = None, x2 = None,
                factors:Dict[str, List[str]] = None, tags:List[str] = None, df:pd.DataFrame = None):
     """
@@ -66,15 +66,15 @@
     x1, x2 = _get_x1_x2(x1, x2, factors, tag, df)
     return scipy.stats.ttest_1samp(x1, x2, **kwargs)
 
 def ttest_ind(x1 = None, x2 = None,
                  factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
     """
     独立样本t检验(双样本T检验):检验两组独立样本均值是否相等\n
-    要求正太分布，正太检验结果由scipy.stats.levene计算并返回\n
+    要求正态分布，正态检验结果由scipy.stats.levene计算并返回\n
     levene 检验P值 > 0.05，接受原假设，认为两组方差相等\n
     如不相等， scipy.stats.ttest_ind() 函数中的参数 equal_var 会设置成 False
     """
     x1, x2 = _get_x1_x2(x1, x2, factors, tag, df)
     levene = scipy.stats.levene(x1, x2)
     return levene.pvalue, scipy.stats.ttest_ind(x1, x2, equal_var=levene.pvalue > 0.05)
 
@@ -91,18 +91,26 @@
     评估了两个抽样群体是否可能来自同一群体，这两个群体在数据方面是否具有相同的形状？\n
     证明这两个群体是否来自于具有不同水平的相关变量的人群。\n
     此包装函数同时支持直接输入和mbapy-style数据输入
     """
     x1, x2 = _get_x1_x2(x1, x2, factors, tag, df)
     return scipy.stats.mannwhitneyu(x1, x2, **kwargs)
 
+def wilcoxon(x1 = None, x2 = None,
+             factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
+    """
+    Wilcoxon signed-rank test, 样本不符合正态分布但配对时使用。
+    """
+    x1, x2 = _get_x1_x2(x1, x2, factors, tag, df)
+    return scipy.stats.ranksums(x1, x2, **kwargs)
+
 def shapiro(x1 = None,
             factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
     """
-    shapiro正态检验:\n
+    夏皮洛-威尔克检验（Shapiro—Wilk test），一般又称W检验。W检验是一种类似于利用秩进行相关性检验的方法。同样需要注意的是，W检验与K-S检验一样，原假设是“样本数据来自的分布与正态分布无显著差异”，因此一般来说，检验结果P>0.05才是我们的目标。
     p > 0.05 为正态分布
     """
     x1, _ = _get_x1_x2(x1, None, factors, tag, df)
     return scipy.stats.shapiro(x1, **kwargs)
 
 def pearsonr(x1 = None, x2 = None,
              factors:Dict[str, List[str]] = None, tags:List[str] = None, df:pd.DataFrame = None, **kwargs):
@@ -112,14 +120,86 @@
     mbapy-style数据输入:\n
     提取多列tag的x1和x2，factors仅作筛选作用
     tags为x1和x2...的tag
     """
     x1, x2 = _get_x1_x2_R(x1, x2, factors, tags, df)
     return scipy.stats.pearsonr(x1, x2, **kwargs)
 
+def auto_ind_test(x1 = None, x2 = None,
+                  factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None,
+                  float_round:int = 5, **kwargs):
+    """
+    Params:
+        - x1, x2: samples to compare
+        - factors, tag, df: mbapy-style data input
+        - float_round: round the result to float_round decimal places
+        - **kwargs: other parameters for the test function
+        
+    Returns:
+        - result: the result of the test function
+        
+    Notes:
+    自动选择最合适的检验方法\n
+    - 符合正态分布
+        - 配对：scipy.stats.ttest_rel
+        - 不配对：
+            - 等方差：scipy.stats.ttest_ind(equal_var=True)
+            - 不确定等方差：scipy.stats.ttest_ind(equal_var=False)
+    - 不符合正态分布
+        - 配对：scipy.stats.wilcoxon
+        - 不配对：scipy.stats.mannwhitneyu
+    
+    Items:
+        - skew: 偏度，0代表正态，大于0代表右偏，小于0代表左偏
+        - kurtosis: 峰度，峰度包括正态分布（峰度值=3），厚尾（峰度值>3），瘦尾（峰度值<3）
+        - normality: 正态性检验结果
+        - equal_var: 方差是否相等，直接检验X1和X2
+    """
+    x1, x2 = _get_x1_x2(x1, x2, factors, tag, df)
+    _fmt_result = lambda result: f'{result[0]:.{float_round}f}, p={result[1]:.{float_round}f}, {result[1] < 0.05}' # < 0.05 为显著差异
+    _fmt_result_gt = lambda result: f'{result[0]:.{float_round}f}, p={result[1]:.{float_round}f}, {result[1] > 0.05}' # < 0.05 为显著差异
+    print('-'*22, 'mbapy.stats.auto_ind_test', '-'*23)
+    if factors is not None and tag is not None and df is not None:
+        fac_name = df[list(factors.keys())[0]].unique()
+        print(f'Factor: {list(factors.keys())[0]}')
+        print(f'X1: {fac_name[0]}, X2: {fac_name[1]}')
+    # show x1 and x2 statistics info (each)
+    shapiro_results = []
+    print('-'*19, 'X1 and X2 Statistics Info (each)', '-'*19)
+    for i, x in enumerate([x1, x2]):
+        print(f'X{i+1}: N={len(x)}, mean={np.mean(x):.{float_round}f}, std={np.std(x):.{float_round}f}, SE={scipy.stats.sem(x):.{float_round}f}')
+        print(f'skew={scipy.stats.skew(x):.{float_round}f}, kurtosis={scipy.stats.kurtosis(x):.{float_round}f}')
+        shapiro_results.append(shapiro(x))
+        print(f'normality(shapiro)={_fmt_result_gt(shapiro_results[-1])}')
+        print('-'*70)
+    # show x1 and x2 statistics info (together)
+    print('-'*17, 'X1 and X2 Statistics Info (together)', '-'*17)
+    equal_vars = scipy.stats.levene(x1, x2)
+    print(f'equal_var(levene)={_fmt_result_gt(equal_vars)}')
+    print('-'*70)
+    # perform test
+    if shapiro_results[0][1] > 0.05 and shapiro_results[1][1] > 0.05:
+        if len(x1) != len(x2):
+            is_equal_vals = equal_vars[1] > 0.05
+            result = scipy.stats.ttest_ind(x1, x2, equal_var=is_equal_vals, **kwargs)
+            print(f'perform ttest_ind(equal_var={is_equal_vals}): {_fmt_result(result)}')
+        else:
+            result = scipy.stats.ttest_rel(x1, x2, **kwargs)
+            print(f'perform ttest_rel: {_fmt_result(result)}')
+    else:
+        if len(x1) == len(x2):
+            result = scipy.stats.wilcoxon(x1, x2, **kwargs)
+            print(f'perform wilcoxon: {_fmt_result(result)}')
+        else:
+            result = scipy.stats.mannwhitneyu(x1, x2, **kwargs)
+            print(f'perform mannwhitneyu: {_fmt_result(result)}')
+    print('-'*70)
+    return result
+
+
 def _get_observe(observed = None,
                  factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None):
     if observed is None and factors is not None and tag is not None and df is not None:
         @msd.pro_bar_data_R(list(factors.keys()), [tag], df, [''])
         def get_sum(values):
             return [values.sum()]
         ndf = get_sum()
```

### Comparing `mbapy-0.7.1b1/mbapy/storage/libsci.dll` & `mbapy-0.7.2/mbapy/storage/libsci.dll`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/storage/libsci.so` & `mbapy-0.7.2/mbapy/storage/libsci.so`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/storage/libstats.dll` & `mbapy-0.7.2/mbapy/storage/libstats.dll`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/storage/libstats.so` & `mbapy-0.7.2/mbapy/storage/libstats.so`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/web.py` & `mbapy-0.7.2/mbapy/web.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/web_utils/parse.py` & `mbapy-0.7.2/mbapy/web_utils/parse.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/web_utils/request.py` & `mbapy-0.7.2/mbapy/web_utils/request.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/web_utils/spider.py` & `mbapy-0.7.2/mbapy/web_utils/spider.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy/web_utils/task.py` & `mbapy-0.7.2/mbapy/web_utils/task.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/mbapy.egg-info/PKG-INFO` & `mbapy-0.7.2/mbapy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,75 @@
 Metadata-Version: 2.1
 Name: mbapy
-Version: 0.7.1b1
+Version: 0.7.2
 Summary: MyBA in Python
 Home-page: https://github.com/BHM-Bob/BA_PY
 Author: BHM-Bob G
 Author-email: bhmfly@foxmail.com
 License: MIT Licence
 Description: <!--
          * @Author: BHM-Bob 2262029386@qq.com
          * @Date: 2022-10-19 22:16:22
          * @LastEditors: BHM-Bob 2262029386@qq.com
-         * @LastEditTime: 2023-10-05 19:26:42
+         * @LastEditTime: 2024-04-04 19:36:44
          * @Description: 
         -->
-        # BA_PY
+        # BA_PY: Optimize Your Workflow with Python!
         [![Downloads](https://static.pepy.tech/badge/mbapy)](https://pepy.tech/project/mbapy) ![PyPI - Downloads](https://img.shields.io/pypi/dm/mbapy) ![GitHub all releases](https://img.shields.io/github/downloads/BHM-Bob/BA_PY/total?label=GitHub%20all%20releases%20downloads)
         
         ![GitHub repo size](https://img.shields.io/github/repo-size/BHM-Bob/BA_PY) ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/BHM-Bob/BA_PY) [![GitHub Commit Activity](https://img.shields.io/github/commit-activity/m/BHM-Bob/BA_PY)](https://github.com/BHM-Bob/BA_PY/pulse)
         
         ![PyPI - Status](https://img.shields.io/pypi/status/mbapy?label=PyPI%20Status) ![PyPI](https://img.shields.io/pypi/v/mbapy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mbapy)
         
         ![Read the Docs](https://img.shields.io/readthedocs/ba-py) ![GitHub](https://img.shields.io/github/license/BHM-Bob/BA_PY) [![built with Codeium](https://codeium.com/badges/main)](https://codeium.com)
         
         ![platform - WINDOWS](https://camo.githubusercontent.com/c292429e232884db22e86c2ea2ea7695bc49dc4ae13344003a95879eeb7425d8/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f57696e646f77732d3030373844363f7374796c653d666f722d7468652d6261646765266c6f676f3d77696e646f7773266c6f676f436f6c6f723d7768697465) ![platform - LINUX](https://camo.githubusercontent.com/7eefb2ba052806d8a9ce69863c2eeb3b03cd5935ead7bd2e9245ae2e705a1adf/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4c696e75782d4643433632343f7374796c653d666f722d7468652d6261646765266c6f676f3d6c696e7578266c6f676f436f6c6f723d626c61636b)
         
         mbapy is a Python package that includes a collection of useful Python scripts as sub-modules, and it's goal is *Basic for All in Python*.  
-        mbapy primarily focus on areas such as sci-plot, stats, web-crawler, sci-paper utilities, and deep learning with pytorch.  
+        mbapy primarily focus on data works, including data-retrieval, data-management, data-visualization, data-analysis and data-computation. It is built for both python-users and command-line-users.
         
         ## get start
         
         #### install 
         Now, mbapy only support pypi install:  
         ```
         pip install mbapy
         ```
         
         mbapy is a multi-funtional package, and it does not require every third-party packages to make every sub-module work. However, it provides some requriements option to install more specified requirements to make some sub-modules work:  
         1. bio: some packages for biology(sci).  
             install as `pip install mbapy[bio]`  
-        2. full: full requirements to make almost every sub-module in mbapy work(except dl_torch).  
+        2. game: some packages for game(pygame).  
+            install as `pip install mbapy[game]`  
+        3. full: full requirements to make almost every sub-module in mbapy work(except dl_torch).  
              install as `pip install mbapy[full]`  
         
         If you find the latest release version has some problems, you can try install the up-to-date version on github or gitee:  
         ```
         pip install git+https://github.com/BHM-Bob/BA_PY.git
         ```
         ```
         pip install git+https://gitee.com/BHM-Bob/BA_PY.git
         ```
         
         #### docs
-        The documentation for mbapy can be found on [read the docs](https://ba-py.readthedocs.io/en/latest/), and it is the one that I will regularly update.
-        The API document for mbapy is available on its [wiki](https://github.com/BHM-Bob/BA_PY/wiki). However, please note that this wiki on GitHub has not been updated since 2023-07. 
+        The documentation for mbapy can be found on [read the docs](https://ba-py.readthedocs.io/en/latest/) or just in the `docs` folder.
         
         #### web sites
         - open source at:  
             1. [github： https://github.com/BHM-Bob/BA_PY](https://github.com/BHM-Bob/BA_PY)  
             2. [gitee： https://gitee.com/BHM-Bob/BA_PY](https://gitee.com/BHM-Bob/BA_PY)  
         - docs at: [read the docs: https://ba-py.rtfd.io](https://ba-py.readthedocs.io/en/latest/)  
+        - PyPI: [https://pypi.org/project/mbapy/](https://pypi.org/project/mbapy/)  
         
         # contain  
         ## mbapy python package  
         #### \_\_version\_\_  
         *some version info*  
+        
         #### base  
         *some utils for easier coding*
         
         #### file
         ##### image
         *imgae utils*, including reading, saving and process a image into a feature tensor via pytorch.  
         ##### video
@@ -79,14 +82,16 @@
         *utils for web-crawler*  
         ##### request
         *get a web hyml page or a selenium browser warpper for easier usage*.  
         ##### parse
         *utils for parsing html*  
         ##### task
         *small task manager*  
+        ##### spider
+        *a light-weight web spider architecture*  
         
         #### stats
         ##### cluster
         *BAKmeans, KOptim, KBayesian from KMeans, and a func for many cluster*  
         ##### df
         *pandas.dataFrame utils for stats*  
         ##### reg
@@ -119,20 +124,14 @@
         *parse paper from a pdf file into a dict of each sections* 
         
         #### scripts
         *some useful scripts for command user*  
         launch by `python -m mbapy.scripts.XXX` or `mbapy-cli XXX`.  
         
         ## examples
-        #### file
-        *some file utils things*  
-        
-        #### plot
-        1. stack bar plot with hue style  
-        
         #### web/crawler
         1. chaoxin ppt multi threads downloader (jpg->pdf)
         2. wujin search http://www.basechem.org
         3. chemSub search http://chemsub.online.fr
         4. cnipa https://pss-system.cponline.cnipa.gov.cn/seniorSearch
```

### Comparing `mbapy-0.7.1b1/mbapy.egg-info/SOURCES.txt` & `mbapy-0.7.2/mbapy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 mbapy/scripts/avif.py
 mbapy/scripts/cluster.py
 mbapy/scripts/cnipa.py
 mbapy/scripts/cp.py
 mbapy/scripts/duitang.py
 mbapy/scripts/extract-dir.py
 mbapy/scripts/extract_paper.py
+mbapy/scripts/file-size.py
+mbapy/scripts/hplc.py
 mbapy/scripts/mass.py
 mbapy/scripts/mv.py
 mbapy/scripts/peptide.py
 mbapy/scripts/reviz.py
 mbapy/scripts/rm.py
 mbapy/scripts/scihub.py
 mbapy/scripts/scihub_selenium.py
@@ -69,14 +71,15 @@
 mbapy/stats/geography.py
 mbapy/stats/reg.py
 mbapy/stats/test.py
 mbapy/storage/libsci.dll
 mbapy/storage/libsci.so
 mbapy/storage/libstats.dll
 mbapy/storage/libstats.so
+mbapy/storage/mbapy-cli-scripts-list.json
 mbapy/web_utils/__init__.py
 mbapy/web_utils/parse.py
 mbapy/web_utils/request.py
 mbapy/web_utils/spider.py
 mbapy/web_utils/task.py
 test/test_base.py
 test/test_game.py
```

### Comparing `mbapy-0.7.1b1/mbapy.egg-info/requires.txt` & `mbapy-0.7.2/mbapy.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 matplotlib
 numpy
 pandas
 Pillow
 requests
 scikit-learn
 scipy
-seaborn
+seaborn>=0.13.0
 selenium
 urllib3
 statsmodels
 scikit_posthocs
 pdfminer
+PyPDF2
 rispy
 lxml
 crossref_commons
 
 [bio]
 aiohttp
 beautifulsoup4
@@ -25,20 +26,21 @@
 matplotlib
 numpy
 pandas
 Pillow
 requests
 scikit-learn
 scipy
-seaborn
+seaborn>=0.13.0
 selenium
 urllib3
 statsmodels
 scikit_posthocs
 pdfminer
+PyPDF2
 rispy
 lxml
 crossref_commons
 wget
 pdfplumber
 pyteomics
 
@@ -49,26 +51,26 @@
 matplotlib
 numpy
 pandas
 Pillow
 requests
 scikit-learn
 scipy
-seaborn
+seaborn>=0.13.0
 selenium
 urllib3
 statsmodels
 scikit_posthocs
 pdfminer
+PyPDF2
 rispy
 lxml
 crossref_commons
 cn2an
 yaml
-PyPDF2
 pdfplumber
 Markdown
 imageio
 pillow_heif
 wget
 pyteomics
 opencv-python
@@ -83,20 +85,21 @@
 matplotlib
 numpy
 pandas
 Pillow
 requests
 scikit-learn
 scipy
-seaborn
+seaborn>=0.13.0
 selenium
 urllib3
 statsmodels
 scikit_posthocs
 pdfminer
+PyPDF2
 rispy
 lxml
 crossref_commons
 pygame
 opencv-python
 
 [none]
```

### Comparing `mbapy-0.7.1b1/requirements.json` & `mbapy-0.7.2/requirements.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9725274725274726%*

 * *Differences: {"'full'": '{delete: [2]}',*

 * * "'std'": "{insert: [(10, 'seaborn>=0.13.0'), (16, 'PyPDF2')], delete: [10]}"}*

```diff
@@ -3,15 +3,14 @@
         "wget",
         "pdfplumber",
         "pyteomics"
     ],
     "full": [
         "cn2an",
         "yaml",
-        "PyPDF2",
         "pdfplumber",
         "Markdown",
         "imageio",
         "pillow_heif",
         "wget",
         "pyteomics",
         "opencv-python",
@@ -30,18 +29,19 @@
         "matplotlib",
         "numpy",
         "pandas",
         "Pillow",
         "requests",
         "scikit-learn",
         "scipy",
-        "seaborn",
+        "seaborn>=0.13.0",
         "selenium",
         "urllib3",
         "statsmodels",
         "scikit_posthocs",
         "pdfminer",
+        "PyPDF2",
         "rispy",
         "lxml",
         "crossref_commons"
     ]
 }
```

### Comparing `mbapy-0.7.1b1/setup.py` & `mbapy-0.7.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-11-01 18:30:01
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2024-02-20 17:12:04
+LastEditTime: 2024-04-21 21:07:12
 Description: 
 '''
 """
 something is from https://github.com/pypa/sampleproject
 thanks to https://zetcode.com/python/package/
 thanks to https://github.com/gaogaotiantian/viztracer/blob/master/setup.py
 """
@@ -104,8 +104,8 @@
         'full': requirements['std'] + requirements['full'],
         },
 )
 
 # pip install .
 
 # python setup.py sdist
-# twine upload dist/mbapy-0.7.0.tar.gz
+# twine upload dist/mbapy-0.7.2.tar.gz
```

### Comparing `mbapy-0.7.1b1/test/test_base.py` & `mbapy-0.7.2/test/test_base.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/test/test_game.py` & `mbapy-0.7.2/test/test_game.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1b1/test/test_web.py` & `mbapy-0.7.2/test/test_web.py`

 * *Files identical despite different names*


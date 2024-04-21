# Comparing `tmp/lifton-0.0.2.tar.gz` & `tmp/lifton-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifton-0.0.2.tar", last modified: Mon Jan 22 16:33:22 2024, max compression
+gzip compressed data, was "lifton-0.0.3.tar", last modified: Sun Apr 21 17:38:22 2024, max compression
```

## Comparing `lifton-0.0.2.tar` & `lifton-0.0.3.tar`

### file list

```diff
@@ -1,52 +1,50 @@
-drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-01-22 16:33:22.120720 lifton-0.0.2/
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    34599 2024-01-03 16:41:07.000000 lifton-0.0.2/LICENSE
-drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-01-22 16:33:22.111225 lifton-0.0.2/Lifton.egg-info/
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    17884 2024-01-22 16:33:22.000000 lifton-0.0.2/Lifton.egg-info/PKG-INFO
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     1378 2024-01-22 16:33:22.000000 lifton-0.0.2/Lifton.egg-info/SOURCES.txt
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)        1 2024-01-22 16:33:22.000000 lifton-0.0.2/Lifton.egg-info/dependency_links.txt
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)       46 2024-01-22 16:33:22.000000 lifton-0.0.2/Lifton.egg-info/entry_points.txt
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)      110 2024-01-22 16:33:22.000000 lifton-0.0.2/Lifton.egg-info/requires.txt
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)        7 2024-01-22 16:33:22.000000 lifton-0.0.2/Lifton.egg-info/top_level.txt
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    17884 2024-01-22 16:33:22.120506 lifton-0.0.2/PKG-INFO
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    17589 2024-01-17 18:01:56.000000 lifton-0.0.2/README.md
-drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-01-22 16:33:22.115419 lifton-0.0.2/lifton/
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)       23 2024-01-22 16:32:54.000000 lifton-0.0.2/lifton/__init__.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     7566 2024-01-17 14:20:47.000000 lifton-0.0.2/lifton/align.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     6728 2024-01-10 14:52:46.000000 lifton-0.0.2/lifton/annotation.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     6754 2024-01-10 14:52:46.000000 lifton-0.0.2/lifton/evaluation.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     2720 2024-01-17 14:20:47.000000 lifton-0.0.2/lifton/extract_sequence.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     8011 2024-01-17 14:20:47.000000 lifton-0.0.2/lifton/fix_trans_annotation.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     1787 2024-01-17 14:20:47.000000 lifton-0.0.2/lifton/get_id_fraction.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)      578 2024-01-17 14:20:47.000000 lifton-0.0.2/lifton/intervals.py
-drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-01-22 16:33:22.119663 lifton-0.0.2/lifton/liftoff/
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)        0 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/__init__.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    13175 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/align_features.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)      597 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/aligned_seg.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    10276 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/extract_features.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)      190 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/feature_hierarchy.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    19044 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/find_best_mapping.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     9361 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/fix_overlapping_features.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5664 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/lift_features.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    15486 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/liftoff_main.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     4032 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/liftoff_utils.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5206 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/liftover_types.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     3945 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/merge_lifted_features.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)      372 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/new_feature.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    14008 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/polish.py
-drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-01-22 16:33:22.120203 lifton-0.0.2/lifton/liftoff/tests/
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)        1 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/tests/__init__.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     2058 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/tests/test_advanced.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     1895 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/tests/test_basic.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5428 2023-12-18 15:30:14.000000 lifton-0.0.2/lifton/liftoff/write_new_gff.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    19586 2024-01-17 14:20:47.000000 lifton-0.0.2/lifton/lifton.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    37743 2024-01-17 14:20:47.000000 lifton-0.0.2/lifton/lifton_class.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    15292 2024-01-10 14:52:46.000000 lifton-0.0.2/lifton/lifton_class_eval.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    17453 2024-01-22 16:32:54.000000 lifton-0.0.2/lifton/lifton_utils.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)      233 2024-01-22 16:32:54.000000 lifton-0.0.2/lifton/logger.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     1252 2024-01-22 16:32:54.000000 lifton-0.0.2/lifton/mapping.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     9947 2024-01-22 16:32:54.000000 lifton-0.0.2/lifton/run_liftoff.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     6146 2024-01-22 16:32:54.000000 lifton-0.0.2/lifton/run_miniprot.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     4014 2024-01-22 16:32:54.000000 lifton-0.0.2/lifton/stats.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     4058 2024-01-22 16:32:54.000000 lifton-0.0.2/lifton/variants.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)       38 2024-01-22 16:33:22.120773 lifton-0.0.2/setup.cfg
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)      771 2024-01-22 16:32:54.000000 lifton-0.0.2/setup.py
+drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-21 17:38:22.011859 lifton-0.0.3/
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    34599 2024-01-03 20:18:51.000000 lifton-0.0.3/LICENSE
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    22677 2024-04-21 17:38:22.000859 lifton-0.0.3/PKG-INFO
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    22382 2024-03-04 20:29:33.000000 lifton-0.0.3/README.md
+drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-21 17:38:20.587856 lifton-0.0.3/lifton/
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       23 2024-04-21 17:37:16.000000 lifton-0.0.3/lifton/__init__.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     8659 2024-04-19 19:09:42.000000 lifton-0.0.3/lifton/align.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     6640 2024-04-19 19:09:51.000000 lifton-0.0.3/lifton/annotation.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     2620 2024-04-19 19:10:25.000000 lifton-0.0.3/lifton/extract_sequence.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1823 2024-04-19 19:16:33.000000 lifton-0.0.3/lifton/get_id_fraction.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      578 2024-04-19 19:16:38.000000 lifton-0.0.3/lifton/intervals.py
+drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-21 17:38:21.822858 lifton-0.0.3/lifton/liftoff/
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2023-12-24 02:47:54.000000 lifton-0.0.3/lifton/liftoff/__init__.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    13175 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/align_features.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      597 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/aligned_seg.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    10276 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/extract_features.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      190 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/feature_hierarchy.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    19044 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/find_best_mapping.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     9361 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/fix_overlapping_features.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5664 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/lift_features.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    15486 2024-02-12 19:50:40.000000 lifton-0.0.3/lifton/liftoff/liftoff_main.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     4032 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/liftoff_utils.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5206 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/liftover_types.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     3945 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/merge_lifted_features.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      372 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/new_feature.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    14008 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/polish.py
+drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-21 17:38:21.949859 lifton-0.0.3/lifton/liftoff/tests/
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        1 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/tests/__init__.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     2058 2023-12-24 03:45:19.000000 lifton-0.0.3/lifton/liftoff/tests/test_advanced.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1895 2023-12-24 03:45:19.000000 lifton-0.0.3/lifton/liftoff/tests/test_basic.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5428 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/write_new_gff.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    20297 2024-04-21 13:55:31.000000 lifton-0.0.3/lifton/lifton.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    34194 2024-04-21 13:30:06.000000 lifton-0.0.3/lifton/lifton_class.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    19966 2024-04-21 13:29:00.000000 lifton-0.0.3/lifton/lifton_utils.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      233 2024-01-24 15:32:08.000000 lifton-0.0.3/lifton/logger.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     7585 2024-04-21 00:36:04.000000 lifton-0.0.3/lifton/protein_maximization.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     4261 2024-04-21 17:24:05.000000 lifton-0.0.3/lifton/run_evaluation.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     8967 2024-04-21 17:29:27.000000 lifton-0.0.3/lifton/run_liftoff.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     6576 2024-04-21 01:51:11.000000 lifton-0.0.3/lifton/run_miniprot.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5595 2024-04-21 01:28:11.000000 lifton-0.0.3/lifton/stats.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     4196 2024-04-21 13:22:57.000000 lifton-0.0.3/lifton/variants.py
+drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-21 17:38:20.907856 lifton-0.0.3/lifton.egg-info/
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    22677 2024-04-21 17:38:19.000000 lifton-0.0.3/lifton.egg-info/PKG-INFO
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1154 2024-04-21 17:38:19.000000 lifton-0.0.3/lifton.egg-info/SOURCES.txt
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        1 2024-04-21 17:38:19.000000 lifton-0.0.3/lifton.egg-info/dependency_links.txt
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       46 2024-04-21 17:38:19.000000 lifton-0.0.3/lifton.egg-info/entry_points.txt
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      168 2024-04-21 17:38:19.000000 lifton-0.0.3/lifton.egg-info/requires.txt
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        7 2024-04-21 17:38:19.000000 lifton-0.0.3/lifton.egg-info/top_level.txt
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       38 2024-04-21 17:38:22.021859 lifton-0.0.3/setup.cfg
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      833 2024-04-21 17:37:41.000000 lifton-0.0.3/setup.py
```

### Comparing `lifton-0.0.2/LICENSE` & `lifton-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lifton-0.0.2/Lifton.egg-info/PKG-INFO` & `lifton-0.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: lifton
-Version: 0.0.2
-Summary: A protein-coding gene annotation fixing tool
-Home-page: https://github.com/Kuanhao-Chao/Lifton
-Author: Kuan-Hao Chao
-Author-email: kh.chao@cs.jhu.edu
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <img alt="My Logo" class="logo header-image only-light align-center" src="graphics/LiftOn_color.png" style="width:90%">
 
 <div class="content">
 
 <div class="line"><br></div>
 </div>
 <section id="lifton-s-tutorial">
@@ -22,15 +11,15 @@
 <a class="reference external image-reference" href="https://pepy.tech/project/lifton"><img alt="https://static.pepy.tech/personalized-badge/lifton?period=total&amp;units=abbreviation&amp;left_color=grey&amp;right_color=blue&amp;left_text=PyPi%20downloads" src="https://static.pepy.tech/personalized-badge/lifton?period=total&amp;units=abbreviation&amp;left_color=grey&amp;right_color=blue&amp;left_text=PyPi%20downloads"></a>
 <a class="reference external image-reference" href="https://github.com/Kuanhao-Chao/lifton/releases"><img alt="https://img.shields.io/github/downloads/Kuanhao-Chao/lifton/total.svg?style=social&amp;logo=github&amp;label=Download" src="https://img.shields.io/github/downloads/Kuanhao-Chao/lifton/total.svg?style=social&amp;logo=github&amp;label=Download"></a>
 <a class="reference external image-reference" href="https://github.com/Kuanhao-Chao/lifton/releases"><img alt="https://img.shields.io/badge/platform-macOS_/Linux-green.svg" src="https://img.shields.io/badge/platform-macOS_/Linux-green.svg"></a>
 <a class="reference external image-reference" href="https://colab.research.google.com/github/Kuanhao-Chao/lifton/blob/main/notebook/lifton_example.ipynb"><img alt="https://colab.research.google.com/assets/colab-badge.svg" src="https://colab.research.google.com/assets/colab-badge.svg"></a>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
-<p>LiftOn is a homology-based lift-over tool designed to accurately map annotations in GFF or GTF between assemblies. It is built upon the fantastic <a class="reference external" href="https://academic.oup.com/bioinformatics/article/37/12/1639/6035128?login=true">Liftoff</a> (credits to <a class="reference external" href="https://scholar.google.com/citations?user=N3tXk7QAAAAJ&amp;hl=en">Dr. Alaina Shumate</a>) and <a class="reference external" href="https://academic.oup.com/bioinformatics/article/39/1/btad014/6989621">miniprot</a> (credits to <a class="reference external" href="http://liheng.org">Dr. Heng Li</a>), and employs a <a class="reference internal" href="content/behind_scenes.html#protein-maximization-algorithm"><span class="std std-ref">Protein-maximization algorithm</span></a> to improve the protein-coding gene lift-over process.</p>
+<p>LiftOn is a homology-based lift-over tool designed to accurately map annotations in GFF or GTF between assemblies. It is built upon the fantastic <a class="reference external" href="https://academic.oup.com/bioinformatics/article/37/12/1639/6035128?login=true">Liftoff</a> (credits to <a class="reference external" href="https://scholar.google.com/citations?user=N3tXk7QAAAAJ&amp;hl=en">Dr. Alaina Shumate</a>) and <a class="reference external" href="https://academic.oup.com/bioinformatics/article/39/1/btad014/6989621">miniprot</a> (credits to <a class="reference external" href="http://liheng.org">Dr. Heng Li</a>), and employs a <a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#protein-maximization-algorithm"><span class="std std-ref">Protein-maximization algorithm</span></a> to improve the protein-coding gene lift-over process.</p>
 <section id="why-lifton" class="">
 <h2>Why LiftOn❓<a class="headerlink" href="#why-lifton" title="Permalink to this heading">#</a></h2>
 <ol class="arabic simple">
 <li><p><strong>Burgeoning number of genome assemblies</strong>: As of December 2023, among the 15,578 distinct eukaryotic genomes, only 1,111 have been annotated (<a class="reference external" href="https://www.ncbi.nlm.nih.gov/genome/annotation_euk/#graphs">Eukaryotic Genome Annotation at NCBI</a>). More and more high quality assemblies are generated. We need to accurately annotate them.</p></li>
 <li><p><strong>Improved protein-coding gene mapping</strong>: The popular <a class="reference external" href="https://academic.oup.com/bioinformatics/article/37/12/1639/6035128?login=true">Liftoff</a> map genes only based on the DNA alignment. With the protein-to-genome alignment, LiftOn is able to further improve the lift-over protein-coding gene annotations. LiftOn improves the current released T2T-CHM13 annotation (<a class="reference external" href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/annotation/chm13v2.0_RefSeq_Liftoff_v5.1.gff3.gz">JHU RefSeqv110 + Liftoff v5.1</a>).</p></li>
 <li><p><strong>Improved distant species lift-over</strong>: LiftOn extends from lift-over between the same or closely related species to more distantly related species. See <span class="xref std std-ref">mouse_2_rat</span> and <span class="xref std std-ref">drosophila_melanogaster_2_erecta</span> lift-over sections.</p></li>
 </ol>
@@ -48,34 +37,42 @@
 </ol>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
 </section>
 <section id="what-does-lifton-do" class="">
 <h2>What does LiftOn do❓<a class="headerlink" href="#what-does-lifton-do" title="Permalink to this heading">#</a></h2>
-<p>LiftOn is designed for individuals who would like to annotate a new assembly, referred to as target <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="0" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>T</mi></math></mjx-assistive-mml></mjx-container></span>.</p>
-<p>The first step is to select a well-annotated genome along with its annotation, denoted as reference <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="1" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>R</mi></math></mjx-assistive-mml></mjx-container></span> and <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="2" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>R</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span>.</p>
-<p>LiftOn employs a two-step  <a class="reference internal" href="content/behind_scenes.html#protein-maximization-algorithm"><span class="std std-ref">Protein-maximization algorithm</span></a> (PM algorithm).</p>
+<p>Given a reference <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="0" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>R</mi></math></mjx-assistive-mml></mjx-container></span>, an <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="1" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>R</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span>, and a target <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="2" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>T</mi></math></mjx-assistive-mml></mjx-container></span>. The lift-over problem is defined as the process of changing the coordinates of <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="3" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>R</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span> from <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="4" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>R</mi></math></mjx-assistive-mml></mjx-container></span> to <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="5" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>T</mi></math></mjx-assistive-mml></mjx-container></span>, and generate a new annotation file <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="6" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em; margin-left: -0.12em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>T</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span>. A simple illustration of the lift-over problem is shown in <a class="reference internal" href="#liftover-illustration"><span class="std std-numref">Figure 1</span></a>.</p>
+<figure class="align-center" id="id5">
+<span id="liftover-illustration"></span><a class="reference internal image-reference" href="graphics/liftover_illustration.gif"><img alt="graphics/liftover_illustration.gif" src="graphics/liftover_illustration.gif" style="width: 672.5px; height: 270.0px;"></a>
+<figcaption>
+<p><span class="caption-number">Figure 1 </span><span class="caption-text">Illustration of the lift-over problem. The annotation file from the reference genome (top) is lifted over to the target genome (bottom).</span><a class="headerlink" href="#id5" title="Permalink to this image">#</a></p>
+</figcaption>
+</figure>
+<div class="line-block">
+<div class="line"><br></div>
+</div>
+<p>LiftOn is the best tool to help you solve this problem! LiftOn employs a two-step <a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#protein-maximization-algorithm"><span class="std std-ref">protein maximization algorithm</span></a> (PM algorithm).</p>
 <ol class="arabic simple">
 <li><p>The first module is the <em>chaining algorithm</em>. It starts by extracting protein sequences annotated by Liftoff and miniprot. LiftOn then aligns these sequences to full-length reference proteins. For each gene locus, LiftOn compares each section of the protein alignments from Liftoff and miniprot, chaining together the best combinations.</p></li>
 <li><p>The second module is the <em>open-reading frame search (ORF search) algorithm</em>. In the case of truncated protein-coding transcripts, this algorithm examines alternative frames to identify the ORF that produces the longest match with the reference protein.</p></li>
 </ol>
 <ul class="simple">
 <li><dl class="simple">
 <dt><strong>Input</strong>:</dt><dd><ol class="arabic simple">
-<li><p>target <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="3" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>T</mi></math></mjx-assistive-mml></mjx-container></span> in FASTA</p></li>
-<li><p>reference <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="4" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>R</mi></math></mjx-assistive-mml></mjx-container></span> in FASTA</p></li>
-<li><p>reference <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="5" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>R</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span> in GFF3</p></li>
+<li><p>target <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="7" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>T</mi></math></mjx-assistive-mml></mjx-container></span> in FASTA.</p></li>
+<li><p>reference <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="8" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>R</mi></math></mjx-assistive-mml></mjx-container></span> in FASTA</p></li>
+<li><p>reference <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="9" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>R</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span> in GFF3</p></li>
 </ol>
 </dd>
 </dl>
 </li>
 <li><dl class="simple">
 <dt><strong>Output</strong>:</dt><dd><ol class="arabic simple">
-<li><p>LiftOn annotation file in GFF3</p></li>
+<li><p>LiftOn annotation file, <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="10" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em; margin-left: -0.12em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>T</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span>, in GFF3</p></li>
 <li><p>Protein sequence identities &amp; mutation types</p></li>
 <li><p>Features with extra copies</p></li>
 <li><p>Unmapped features</p></li>
 </ol>
 </dd>
 </dl>
 </li>
@@ -108,66 +105,66 @@
 <div class="line"><br></div>
 </div>
 </section>
 <section id="table-of-contents">
 <span id="id3"></span><h2>Table of contents<a class="headerlink" href="#table-of-contents" title="Permalink to this heading">#</a></h2>
 <div class="toctree-wrapper compound">
 <ul>
-<li class="toctree-l1"><a class="reference internal" href="content/installation.html">Installation</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#system-requirements">System requirements</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#install-through-pip">Install through pip</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#install-through-conda">Install through conda</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#install-from-source">Install from source</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#check-lifton-installation">Check LiftOn installation</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#now-you-are-ready-to-go">Now, you are ready to go !</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html">Installation</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#system-requirements">System requirements</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#install-through-pip">Install through pip</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#install-through-conda">Install through conda</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#install-from-source">Install from source</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#check-lifton-installation">Check LiftOn installation</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#now-you-are-ready-to-go">Now, you are ready to go !</a></li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="content/quickstart.html">Quick Start Guide</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/quickstart.html#super-quick-start-one-liner">Super-Quick Start (one-liner)</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/quickstart.html#try-lifton-on-google-colab">Try LiftOn on Google Colab</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/quickstart.html">Quick Start Guide</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/quickstart.html#super-quick-start-one-liner">Super-Quick Start (one-liner)</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/quickstart.html#try-lifton-on-google-colab">Try LiftOn on Google Colab</a></li>
 </ul>
 </li>
 </ul>
 </div>
 <div class="toctree-wrapper compound">
 <p class="caption" role="heading"><span class="caption-text">Examples</span></p>
 <ul>
-<li class="toctree-l1"><a class="reference internal" href="content/same_species_liftover/index.html">Same species lift-over</a></li>
-<li class="toctree-l1"><a class="reference internal" href="content/close_species_liftover/index.html">Closely-related species lift-over</a></li>
-<li class="toctree-l1"><a class="reference internal" href="content/distant_species_liftover/index.html">Distant species lift-over</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/same_species_liftover/index.html">Same species lift-over</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/close_species_liftover/index.html">Closely-related species lift-over</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/distant_species_liftover/index.html">Distant species lift-over</a></li>
 </ul>
 </div>
 <div class="toctree-wrapper compound">
 <p class="caption" role="heading"><span class="caption-text">Info</span></p>
 <ul>
-<li class="toctree-l1"><a class="reference internal" href="content/output_explanation.html">Output files</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/output_explanation.html#lifton-gff3">lifton.GFF3</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/output_explanation.html#lifton-output">lifton_output/</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/output_explanation.html">Output files</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/output_explanation.html#lifton-gff3">lifton.GFF3</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/output_explanation.html#lifton-output">lifton_output/</a></li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="content/behind_scenes.html">Behind the scenes</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#matching-miniprot-liftoff-genome-annotation">Matching miniprot &amp; Liftoff genome annotation</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#protein-maximization-algorithm"><em>Protein-maximization algorithm</em></a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#mutation-report">Mutation report</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#open-reading-frame-search">Open-reading-frame search</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#dna-protein-transcript-sequence-identity-score-calculation">DNA &amp; protein transcript sequence identity score calculation</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#reference">Reference</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html">Behind the scenes</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#matching-miniprot-liftoff-genome-annotation">Matching miniprot &amp; Liftoff genome annotation</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#protein-maximization-algorithm"><em>Protein-maximization algorithm</em></a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#mutation-report">Mutation report</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#open-reading-frame-search">Open-reading-frame search</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#dna-protein-transcript-sequence-identity-score-calculation">DNA &amp; protein transcript sequence identity score calculation</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#reference">Reference</a></li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="content/how_to_page.html">Q &amp; A ...</a></li>
-<li class="toctree-l1"><a class="reference internal" href="content/function_manual.html">User Manual</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/function_manual.html#splam">splam</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/how_to_page.html">Q &amp; A ...</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/function_manual.html">User Manual</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/function_manual.html#splam">splam</a></li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="content/changelog.html">Changelog</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/changelog.html#v1-0-0">v1.0.0</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/changelog.html">Changelog</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/changelog.html#v1-0-0">v1.0.0</a></li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="content/license.html">License</a></li>
-<li class="toctree-l1"><a class="reference internal" href="content/contact.html">Contact</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/license.html">License</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/contact.html">Contact</a></li>
 </ul>
 </div>
 </section>
 </section>
 
 <br>
```

### Comparing `lifton-0.0.2/PKG-INFO` & `lifton-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifton
-Version: 0.0.2
+Version: 0.0.3
 Summary: A protein-coding gene annotation fixing tool
 Home-page: https://github.com/Kuanhao-Chao/Lifton
 Author: Kuan-Hao Chao
 Author-email: kh.chao@cs.jhu.edu
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,15 +22,15 @@
 <a class="reference external image-reference" href="https://pepy.tech/project/lifton"><img alt="https://static.pepy.tech/personalized-badge/lifton?period=total&amp;units=abbreviation&amp;left_color=grey&amp;right_color=blue&amp;left_text=PyPi%20downloads" src="https://static.pepy.tech/personalized-badge/lifton?period=total&amp;units=abbreviation&amp;left_color=grey&amp;right_color=blue&amp;left_text=PyPi%20downloads"></a>
 <a class="reference external image-reference" href="https://github.com/Kuanhao-Chao/lifton/releases"><img alt="https://img.shields.io/github/downloads/Kuanhao-Chao/lifton/total.svg?style=social&amp;logo=github&amp;label=Download" src="https://img.shields.io/github/downloads/Kuanhao-Chao/lifton/total.svg?style=social&amp;logo=github&amp;label=Download"></a>
 <a class="reference external image-reference" href="https://github.com/Kuanhao-Chao/lifton/releases"><img alt="https://img.shields.io/badge/platform-macOS_/Linux-green.svg" src="https://img.shields.io/badge/platform-macOS_/Linux-green.svg"></a>
 <a class="reference external image-reference" href="https://colab.research.google.com/github/Kuanhao-Chao/lifton/blob/main/notebook/lifton_example.ipynb"><img alt="https://colab.research.google.com/assets/colab-badge.svg" src="https://colab.research.google.com/assets/colab-badge.svg"></a>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
-<p>LiftOn is a homology-based lift-over tool designed to accurately map annotations in GFF or GTF between assemblies. It is built upon the fantastic <a class="reference external" href="https://academic.oup.com/bioinformatics/article/37/12/1639/6035128?login=true">Liftoff</a> (credits to <a class="reference external" href="https://scholar.google.com/citations?user=N3tXk7QAAAAJ&amp;hl=en">Dr. Alaina Shumate</a>) and <a class="reference external" href="https://academic.oup.com/bioinformatics/article/39/1/btad014/6989621">miniprot</a> (credits to <a class="reference external" href="http://liheng.org">Dr. Heng Li</a>), and employs a <a class="reference internal" href="content/behind_scenes.html#protein-maximization-algorithm"><span class="std std-ref">Protein-maximization algorithm</span></a> to improve the protein-coding gene lift-over process.</p>
+<p>LiftOn is a homology-based lift-over tool designed to accurately map annotations in GFF or GTF between assemblies. It is built upon the fantastic <a class="reference external" href="https://academic.oup.com/bioinformatics/article/37/12/1639/6035128?login=true">Liftoff</a> (credits to <a class="reference external" href="https://scholar.google.com/citations?user=N3tXk7QAAAAJ&amp;hl=en">Dr. Alaina Shumate</a>) and <a class="reference external" href="https://academic.oup.com/bioinformatics/article/39/1/btad014/6989621">miniprot</a> (credits to <a class="reference external" href="http://liheng.org">Dr. Heng Li</a>), and employs a <a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#protein-maximization-algorithm"><span class="std std-ref">Protein-maximization algorithm</span></a> to improve the protein-coding gene lift-over process.</p>
 <section id="why-lifton" class="">
 <h2>Why LiftOn❓<a class="headerlink" href="#why-lifton" title="Permalink to this heading">#</a></h2>
 <ol class="arabic simple">
 <li><p><strong>Burgeoning number of genome assemblies</strong>: As of December 2023, among the 15,578 distinct eukaryotic genomes, only 1,111 have been annotated (<a class="reference external" href="https://www.ncbi.nlm.nih.gov/genome/annotation_euk/#graphs">Eukaryotic Genome Annotation at NCBI</a>). More and more high quality assemblies are generated. We need to accurately annotate them.</p></li>
 <li><p><strong>Improved protein-coding gene mapping</strong>: The popular <a class="reference external" href="https://academic.oup.com/bioinformatics/article/37/12/1639/6035128?login=true">Liftoff</a> map genes only based on the DNA alignment. With the protein-to-genome alignment, LiftOn is able to further improve the lift-over protein-coding gene annotations. LiftOn improves the current released T2T-CHM13 annotation (<a class="reference external" href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/annotation/chm13v2.0_RefSeq_Liftoff_v5.1.gff3.gz">JHU RefSeqv110 + Liftoff v5.1</a>).</p></li>
 <li><p><strong>Improved distant species lift-over</strong>: LiftOn extends from lift-over between the same or closely related species to more distantly related species. See <span class="xref std std-ref">mouse_2_rat</span> and <span class="xref std std-ref">drosophila_melanogaster_2_erecta</span> lift-over sections.</p></li>
 </ol>
@@ -48,34 +48,42 @@
 </ol>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
 </section>
 <section id="what-does-lifton-do" class="">
 <h2>What does LiftOn do❓<a class="headerlink" href="#what-does-lifton-do" title="Permalink to this heading">#</a></h2>
-<p>LiftOn is designed for individuals who would like to annotate a new assembly, referred to as target <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="0" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>T</mi></math></mjx-assistive-mml></mjx-container></span>.</p>
-<p>The first step is to select a well-annotated genome along with its annotation, denoted as reference <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="1" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>R</mi></math></mjx-assistive-mml></mjx-container></span> and <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="2" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>R</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span>.</p>
-<p>LiftOn employs a two-step  <a class="reference internal" href="content/behind_scenes.html#protein-maximization-algorithm"><span class="std std-ref">Protein-maximization algorithm</span></a> (PM algorithm).</p>
+<p>Given a reference <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="0" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>R</mi></math></mjx-assistive-mml></mjx-container></span>, an <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="1" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>R</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span>, and a target <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="2" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>T</mi></math></mjx-assistive-mml></mjx-container></span>. The lift-over problem is defined as the process of changing the coordinates of <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="3" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>R</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span> from <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="4" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>R</mi></math></mjx-assistive-mml></mjx-container></span> to <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="5" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>T</mi></math></mjx-assistive-mml></mjx-container></span>, and generate a new annotation file <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="6" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em; margin-left: -0.12em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>T</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span>. A simple illustration of the lift-over problem is shown in <a class="reference internal" href="#liftover-illustration"><span class="std std-numref">Figure 1</span></a>.</p>
+<figure class="align-center" id="id5">
+<span id="liftover-illustration"></span><a class="reference internal image-reference" href="graphics/liftover_illustration.gif"><img alt="graphics/liftover_illustration.gif" src="graphics/liftover_illustration.gif" style="width: 672.5px; height: 270.0px;"></a>
+<figcaption>
+<p><span class="caption-number">Figure 1 </span><span class="caption-text">Illustration of the lift-over problem. The annotation file from the reference genome (top) is lifted over to the target genome (bottom).</span><a class="headerlink" href="#id5" title="Permalink to this image">#</a></p>
+</figcaption>
+</figure>
+<div class="line-block">
+<div class="line"><br></div>
+</div>
+<p>LiftOn is the best tool to help you solve this problem! LiftOn employs a two-step <a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#protein-maximization-algorithm"><span class="std std-ref">protein maximization algorithm</span></a> (PM algorithm).</p>
 <ol class="arabic simple">
 <li><p>The first module is the <em>chaining algorithm</em>. It starts by extracting protein sequences annotated by Liftoff and miniprot. LiftOn then aligns these sequences to full-length reference proteins. For each gene locus, LiftOn compares each section of the protein alignments from Liftoff and miniprot, chaining together the best combinations.</p></li>
 <li><p>The second module is the <em>open-reading frame search (ORF search) algorithm</em>. In the case of truncated protein-coding transcripts, this algorithm examines alternative frames to identify the ORF that produces the longest match with the reference protein.</p></li>
 </ol>
 <ul class="simple">
 <li><dl class="simple">
 <dt><strong>Input</strong>:</dt><dd><ol class="arabic simple">
-<li><p>target <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="3" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>T</mi></math></mjx-assistive-mml></mjx-container></span> in FASTA</p></li>
-<li><p>reference <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="4" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>R</mi></math></mjx-assistive-mml></mjx-container></span> in FASTA</p></li>
-<li><p>reference <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="5" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>R</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span> in GFF3</p></li>
+<li><p>target <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="7" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>T</mi></math></mjx-assistive-mml></mjx-container></span> in FASTA.</p></li>
+<li><p>reference <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="8" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>R</mi></math></mjx-assistive-mml></mjx-container></span> in FASTA</p></li>
+<li><p>reference <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="9" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>R</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span> in GFF3</p></li>
 </ol>
 </dd>
 </dl>
 </li>
 <li><dl class="simple">
 <dt><strong>Output</strong>:</dt><dd><ol class="arabic simple">
-<li><p>LiftOn annotation file in GFF3</p></li>
+<li><p>LiftOn annotation file, <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="10" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em; margin-left: -0.12em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>T</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span>, in GFF3</p></li>
 <li><p>Protein sequence identities &amp; mutation types</p></li>
 <li><p>Features with extra copies</p></li>
 <li><p>Unmapped features</p></li>
 </ol>
 </dd>
 </dl>
 </li>
@@ -108,66 +116,66 @@
 <div class="line"><br></div>
 </div>
 </section>
 <section id="table-of-contents">
 <span id="id3"></span><h2>Table of contents<a class="headerlink" href="#table-of-contents" title="Permalink to this heading">#</a></h2>
 <div class="toctree-wrapper compound">
 <ul>
-<li class="toctree-l1"><a class="reference internal" href="content/installation.html">Installation</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#system-requirements">System requirements</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#install-through-pip">Install through pip</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#install-through-conda">Install through conda</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#install-from-source">Install from source</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#check-lifton-installation">Check LiftOn installation</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#now-you-are-ready-to-go">Now, you are ready to go !</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html">Installation</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#system-requirements">System requirements</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#install-through-pip">Install through pip</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#install-through-conda">Install through conda</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#install-from-source">Install from source</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#check-lifton-installation">Check LiftOn installation</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#now-you-are-ready-to-go">Now, you are ready to go !</a></li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="content/quickstart.html">Quick Start Guide</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/quickstart.html#super-quick-start-one-liner">Super-Quick Start (one-liner)</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/quickstart.html#try-lifton-on-google-colab">Try LiftOn on Google Colab</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/quickstart.html">Quick Start Guide</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/quickstart.html#super-quick-start-one-liner">Super-Quick Start (one-liner)</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/quickstart.html#try-lifton-on-google-colab">Try LiftOn on Google Colab</a></li>
 </ul>
 </li>
 </ul>
 </div>
 <div class="toctree-wrapper compound">
 <p class="caption" role="heading"><span class="caption-text">Examples</span></p>
 <ul>
-<li class="toctree-l1"><a class="reference internal" href="content/same_species_liftover/index.html">Same species lift-over</a></li>
-<li class="toctree-l1"><a class="reference internal" href="content/close_species_liftover/index.html">Closely-related species lift-over</a></li>
-<li class="toctree-l1"><a class="reference internal" href="content/distant_species_liftover/index.html">Distant species lift-over</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/same_species_liftover/index.html">Same species lift-over</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/close_species_liftover/index.html">Closely-related species lift-over</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/distant_species_liftover/index.html">Distant species lift-over</a></li>
 </ul>
 </div>
 <div class="toctree-wrapper compound">
 <p class="caption" role="heading"><span class="caption-text">Info</span></p>
 <ul>
-<li class="toctree-l1"><a class="reference internal" href="content/output_explanation.html">Output files</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/output_explanation.html#lifton-gff3">lifton.GFF3</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/output_explanation.html#lifton-output">lifton_output/</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/output_explanation.html">Output files</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/output_explanation.html#lifton-gff3">lifton.GFF3</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/output_explanation.html#lifton-output">lifton_output/</a></li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="content/behind_scenes.html">Behind the scenes</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#matching-miniprot-liftoff-genome-annotation">Matching miniprot &amp; Liftoff genome annotation</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#protein-maximization-algorithm"><em>Protein-maximization algorithm</em></a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#mutation-report">Mutation report</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#open-reading-frame-search">Open-reading-frame search</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#dna-protein-transcript-sequence-identity-score-calculation">DNA &amp; protein transcript sequence identity score calculation</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#reference">Reference</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html">Behind the scenes</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#matching-miniprot-liftoff-genome-annotation">Matching miniprot &amp; Liftoff genome annotation</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#protein-maximization-algorithm"><em>Protein-maximization algorithm</em></a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#mutation-report">Mutation report</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#open-reading-frame-search">Open-reading-frame search</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#dna-protein-transcript-sequence-identity-score-calculation">DNA &amp; protein transcript sequence identity score calculation</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#reference">Reference</a></li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="content/how_to_page.html">Q &amp; A ...</a></li>
-<li class="toctree-l1"><a class="reference internal" href="content/function_manual.html">User Manual</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/function_manual.html#splam">splam</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/how_to_page.html">Q &amp; A ...</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/function_manual.html">User Manual</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/function_manual.html#splam">splam</a></li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="content/changelog.html">Changelog</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/changelog.html#v1-0-0">v1.0.0</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/changelog.html">Changelog</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/changelog.html#v1-0-0">v1.0.0</a></li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="content/license.html">License</a></li>
-<li class="toctree-l1"><a class="reference internal" href="content/contact.html">Contact</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/license.html">License</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/contact.html">Contact</a></li>
 </ul>
 </div>
 </section>
 </section>
 
 <br>
```

### Comparing `lifton-0.0.2/README.md` & `lifton-0.0.3/lifton.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: lifton
+Version: 0.0.3
+Summary: A protein-coding gene annotation fixing tool
+Home-page: https://github.com/Kuanhao-Chao/Lifton
+Author: Kuan-Hao Chao
+Author-email: kh.chao@cs.jhu.edu
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <img alt="My Logo" class="logo header-image only-light align-center" src="graphics/LiftOn_color.png" style="width:90%">
 
 <div class="content">
 
 <div class="line"><br></div>
 </div>
 <section id="lifton-s-tutorial">
@@ -11,15 +22,15 @@
 <a class="reference external image-reference" href="https://pepy.tech/project/lifton"><img alt="https://static.pepy.tech/personalized-badge/lifton?period=total&amp;units=abbreviation&amp;left_color=grey&amp;right_color=blue&amp;left_text=PyPi%20downloads" src="https://static.pepy.tech/personalized-badge/lifton?period=total&amp;units=abbreviation&amp;left_color=grey&amp;right_color=blue&amp;left_text=PyPi%20downloads"></a>
 <a class="reference external image-reference" href="https://github.com/Kuanhao-Chao/lifton/releases"><img alt="https://img.shields.io/github/downloads/Kuanhao-Chao/lifton/total.svg?style=social&amp;logo=github&amp;label=Download" src="https://img.shields.io/github/downloads/Kuanhao-Chao/lifton/total.svg?style=social&amp;logo=github&amp;label=Download"></a>
 <a class="reference external image-reference" href="https://github.com/Kuanhao-Chao/lifton/releases"><img alt="https://img.shields.io/badge/platform-macOS_/Linux-green.svg" src="https://img.shields.io/badge/platform-macOS_/Linux-green.svg"></a>
 <a class="reference external image-reference" href="https://colab.research.google.com/github/Kuanhao-Chao/lifton/blob/main/notebook/lifton_example.ipynb"><img alt="https://colab.research.google.com/assets/colab-badge.svg" src="https://colab.research.google.com/assets/colab-badge.svg"></a>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
-<p>LiftOn is a homology-based lift-over tool designed to accurately map annotations in GFF or GTF between assemblies. It is built upon the fantastic <a class="reference external" href="https://academic.oup.com/bioinformatics/article/37/12/1639/6035128?login=true">Liftoff</a> (credits to <a class="reference external" href="https://scholar.google.com/citations?user=N3tXk7QAAAAJ&amp;hl=en">Dr. Alaina Shumate</a>) and <a class="reference external" href="https://academic.oup.com/bioinformatics/article/39/1/btad014/6989621">miniprot</a> (credits to <a class="reference external" href="http://liheng.org">Dr. Heng Li</a>), and employs a <a class="reference internal" href="content/behind_scenes.html#protein-maximization-algorithm"><span class="std std-ref">Protein-maximization algorithm</span></a> to improve the protein-coding gene lift-over process.</p>
+<p>LiftOn is a homology-based lift-over tool designed to accurately map annotations in GFF or GTF between assemblies. It is built upon the fantastic <a class="reference external" href="https://academic.oup.com/bioinformatics/article/37/12/1639/6035128?login=true">Liftoff</a> (credits to <a class="reference external" href="https://scholar.google.com/citations?user=N3tXk7QAAAAJ&amp;hl=en">Dr. Alaina Shumate</a>) and <a class="reference external" href="https://academic.oup.com/bioinformatics/article/39/1/btad014/6989621">miniprot</a> (credits to <a class="reference external" href="http://liheng.org">Dr. Heng Li</a>), and employs a <a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#protein-maximization-algorithm"><span class="std std-ref">Protein-maximization algorithm</span></a> to improve the protein-coding gene lift-over process.</p>
 <section id="why-lifton" class="">
 <h2>Why LiftOn❓<a class="headerlink" href="#why-lifton" title="Permalink to this heading">#</a></h2>
 <ol class="arabic simple">
 <li><p><strong>Burgeoning number of genome assemblies</strong>: As of December 2023, among the 15,578 distinct eukaryotic genomes, only 1,111 have been annotated (<a class="reference external" href="https://www.ncbi.nlm.nih.gov/genome/annotation_euk/#graphs">Eukaryotic Genome Annotation at NCBI</a>). More and more high quality assemblies are generated. We need to accurately annotate them.</p></li>
 <li><p><strong>Improved protein-coding gene mapping</strong>: The popular <a class="reference external" href="https://academic.oup.com/bioinformatics/article/37/12/1639/6035128?login=true">Liftoff</a> map genes only based on the DNA alignment. With the protein-to-genome alignment, LiftOn is able to further improve the lift-over protein-coding gene annotations. LiftOn improves the current released T2T-CHM13 annotation (<a class="reference external" href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/annotation/chm13v2.0_RefSeq_Liftoff_v5.1.gff3.gz">JHU RefSeqv110 + Liftoff v5.1</a>).</p></li>
 <li><p><strong>Improved distant species lift-over</strong>: LiftOn extends from lift-over between the same or closely related species to more distantly related species. See <span class="xref std std-ref">mouse_2_rat</span> and <span class="xref std std-ref">drosophila_melanogaster_2_erecta</span> lift-over sections.</p></li>
 </ol>
@@ -37,34 +48,42 @@
 </ol>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
 </section>
 <section id="what-does-lifton-do" class="">
 <h2>What does LiftOn do❓<a class="headerlink" href="#what-does-lifton-do" title="Permalink to this heading">#</a></h2>
-<p>LiftOn is designed for individuals who would like to annotate a new assembly, referred to as target <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="0" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>T</mi></math></mjx-assistive-mml></mjx-container></span>.</p>
-<p>The first step is to select a well-annotated genome along with its annotation, denoted as reference <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="1" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>R</mi></math></mjx-assistive-mml></mjx-container></span> and <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="2" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>R</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span>.</p>
-<p>LiftOn employs a two-step  <a class="reference internal" href="content/behind_scenes.html#protein-maximization-algorithm"><span class="std std-ref">Protein-maximization algorithm</span></a> (PM algorithm).</p>
+<p>Given a reference <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="0" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>R</mi></math></mjx-assistive-mml></mjx-container></span>, an <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="1" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>R</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span>, and a target <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="2" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>T</mi></math></mjx-assistive-mml></mjx-container></span>. The lift-over problem is defined as the process of changing the coordinates of <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="3" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>R</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span> from <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="4" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>R</mi></math></mjx-assistive-mml></mjx-container></span> to <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="5" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>T</mi></math></mjx-assistive-mml></mjx-container></span>, and generate a new annotation file <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="6" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em; margin-left: -0.12em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>T</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span>. A simple illustration of the lift-over problem is shown in <a class="reference internal" href="#liftover-illustration"><span class="std std-numref">Figure 1</span></a>.</p>
+<figure class="align-center" id="id5">
+<span id="liftover-illustration"></span><a class="reference internal image-reference" href="graphics/liftover_illustration.gif"><img alt="graphics/liftover_illustration.gif" src="graphics/liftover_illustration.gif" style="width: 672.5px; height: 270.0px;"></a>
+<figcaption>
+<p><span class="caption-number">Figure 1 </span><span class="caption-text">Illustration of the lift-over problem. The annotation file from the reference genome (top) is lifted over to the target genome (bottom).</span><a class="headerlink" href="#id5" title="Permalink to this image">#</a></p>
+</figcaption>
+</figure>
+<div class="line-block">
+<div class="line"><br></div>
+</div>
+<p>LiftOn is the best tool to help you solve this problem! LiftOn employs a two-step <a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#protein-maximization-algorithm"><span class="std std-ref">protein maximization algorithm</span></a> (PM algorithm).</p>
 <ol class="arabic simple">
 <li><p>The first module is the <em>chaining algorithm</em>. It starts by extracting protein sequences annotated by Liftoff and miniprot. LiftOn then aligns these sequences to full-length reference proteins. For each gene locus, LiftOn compares each section of the protein alignments from Liftoff and miniprot, chaining together the best combinations.</p></li>
 <li><p>The second module is the <em>open-reading frame search (ORF search) algorithm</em>. In the case of truncated protein-coding transcripts, this algorithm examines alternative frames to identify the ORF that produces the longest match with the reference protein.</p></li>
 </ol>
 <ul class="simple">
 <li><dl class="simple">
 <dt><strong>Input</strong>:</dt><dd><ol class="arabic simple">
-<li><p>target <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="3" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>T</mi></math></mjx-assistive-mml></mjx-container></span> in FASTA</p></li>
-<li><p>reference <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="4" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>R</mi></math></mjx-assistive-mml></mjx-container></span> in FASTA</p></li>
-<li><p>reference <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="5" style="font-size: 118.8%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>R</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span> in GFF3</p></li>
+<li><p>target <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="7" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>T</mi></math></mjx-assistive-mml></mjx-container></span> in FASTA.</p></li>
+<li><p>reference <strong>Genome</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="8" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><mi>R</mi></math></mjx-assistive-mml></mjx-container></span> in FASTA</p></li>
+<li><p>reference <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="9" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D445 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>R</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span> in GFF3</p></li>
 </ol>
 </dd>
 </dl>
 </li>
 <li><dl class="simple">
 <dt><strong>Output</strong>:</dt><dd><ol class="arabic simple">
-<li><p>LiftOn annotation file in GFF3</p></li>
+<li><p>LiftOn annotation file, <strong>Annotation</strong> <span class="math notranslate nohighlight"><mjx-container class="MathJax CtxtMenu_Attached_0" jax="CHTML" tabindex="0" ctxtmenu_counter="10" style="font-size: 119%; position: relative;"><mjx-math class="MJX-TEX" aria-hidden="true"><mjx-msub><mjx-mi class="mjx-i"><mjx-c class="mjx-c1D447 TEX-I"></mjx-c></mjx-mi><mjx-script style="vertical-align: -0.153em; margin-left: -0.12em;"><mjx-mi class="mjx-i" size="s"><mjx-c class="mjx-c1D434 TEX-I"></mjx-c></mjx-mi></mjx-script></mjx-msub></mjx-math><mjx-assistive-mml unselectable="on" display="inline"><math xmlns="http://www.w3.org/1998/Math/MathML"><msub><mi>T</mi><mi>A</mi></msub></math></mjx-assistive-mml></mjx-container></span>, in GFF3</p></li>
 <li><p>Protein sequence identities &amp; mutation types</p></li>
 <li><p>Features with extra copies</p></li>
 <li><p>Unmapped features</p></li>
 </ol>
 </dd>
 </dl>
 </li>
@@ -97,66 +116,66 @@
 <div class="line"><br></div>
 </div>
 </section>
 <section id="table-of-contents">
 <span id="id3"></span><h2>Table of contents<a class="headerlink" href="#table-of-contents" title="Permalink to this heading">#</a></h2>
 <div class="toctree-wrapper compound">
 <ul>
-<li class="toctree-l1"><a class="reference internal" href="content/installation.html">Installation</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#system-requirements">System requirements</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#install-through-pip">Install through pip</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#install-through-conda">Install through conda</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#install-from-source">Install from source</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#check-lifton-installation">Check LiftOn installation</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/installation.html#now-you-are-ready-to-go">Now, you are ready to go !</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html">Installation</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#system-requirements">System requirements</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#install-through-pip">Install through pip</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#install-through-conda">Install through conda</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#install-from-source">Install from source</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#check-lifton-installation">Check LiftOn installation</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/installation.html#now-you-are-ready-to-go">Now, you are ready to go !</a></li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="content/quickstart.html">Quick Start Guide</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/quickstart.html#super-quick-start-one-liner">Super-Quick Start (one-liner)</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/quickstart.html#try-lifton-on-google-colab">Try LiftOn on Google Colab</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/quickstart.html">Quick Start Guide</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/quickstart.html#super-quick-start-one-liner">Super-Quick Start (one-liner)</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/quickstart.html#try-lifton-on-google-colab">Try LiftOn on Google Colab</a></li>
 </ul>
 </li>
 </ul>
 </div>
 <div class="toctree-wrapper compound">
 <p class="caption" role="heading"><span class="caption-text">Examples</span></p>
 <ul>
-<li class="toctree-l1"><a class="reference internal" href="content/same_species_liftover/index.html">Same species lift-over</a></li>
-<li class="toctree-l1"><a class="reference internal" href="content/close_species_liftover/index.html">Closely-related species lift-over</a></li>
-<li class="toctree-l1"><a class="reference internal" href="content/distant_species_liftover/index.html">Distant species lift-over</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/same_species_liftover/index.html">Same species lift-over</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/close_species_liftover/index.html">Closely-related species lift-over</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/distant_species_liftover/index.html">Distant species lift-over</a></li>
 </ul>
 </div>
 <div class="toctree-wrapper compound">
 <p class="caption" role="heading"><span class="caption-text">Info</span></p>
 <ul>
-<li class="toctree-l1"><a class="reference internal" href="content/output_explanation.html">Output files</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/output_explanation.html#lifton-gff3">lifton.GFF3</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/output_explanation.html#lifton-output">lifton_output/</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/output_explanation.html">Output files</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/output_explanation.html#lifton-gff3">lifton.GFF3</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/output_explanation.html#lifton-output">lifton_output/</a></li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="content/behind_scenes.html">Behind the scenes</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#matching-miniprot-liftoff-genome-annotation">Matching miniprot &amp; Liftoff genome annotation</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#protein-maximization-algorithm"><em>Protein-maximization algorithm</em></a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#mutation-report">Mutation report</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#open-reading-frame-search">Open-reading-frame search</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#dna-protein-transcript-sequence-identity-score-calculation">DNA &amp; protein transcript sequence identity score calculation</a></li>
-<li class="toctree-l2"><a class="reference internal" href="content/behind_scenes.html#reference">Reference</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html">Behind the scenes</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#matching-miniprot-liftoff-genome-annotation">Matching miniprot &amp; Liftoff genome annotation</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#protein-maximization-algorithm"><em>Protein-maximization algorithm</em></a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#mutation-report">Mutation report</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#open-reading-frame-search">Open-reading-frame search</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#dna-protein-transcript-sequence-identity-score-calculation">DNA &amp; protein transcript sequence identity score calculation</a></li>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/behind_scenes.html#reference">Reference</a></li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="content/how_to_page.html">Q &amp; A ...</a></li>
-<li class="toctree-l1"><a class="reference internal" href="content/function_manual.html">User Manual</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/function_manual.html#splam">splam</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/how_to_page.html">Q &amp; A ...</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/function_manual.html">User Manual</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/function_manual.html#splam">splam</a></li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="content/changelog.html">Changelog</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="content/changelog.html#v1-0-0">v1.0.0</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/changelog.html">Changelog</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/changelog.html#v1-0-0">v1.0.0</a></li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="content/license.html">License</a></li>
-<li class="toctree-l1"><a class="reference internal" href="content/contact.html">Contact</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/license.html">License</a></li>
+<li class="toctree-l1"><a class="reference internal" href="http://ccb.jhu.edu/lifton/content/contact.html">Contact</a></li>
 </ul>
 </div>
 </section>
 </section>
 
 <br>
```

### Comparing `lifton-0.0.2/lifton/align.py` & `lifton-0.0.3/lifton/align.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,120 +1,187 @@
 import parasail
 from Bio.Seq import Seq
 from cigar import Cigar
 from lifton import get_id_fraction, lifton_class
 
-# Change the CDS protein boundaries based on CIGAR string
+
 def adjust_cdss_protein_boundary(cdss_protein_aln_boundary, cigar_accum_len, length):
+    """
+        This function adjust CDS protein boundaries based on CIGAR string on protein alignment.
+
+        Parameters:
+        - cdss_protein_aln_boundary: CDS protein alignment boundary
+        - cigar_accum_len: accumulated length of CIGAR string
+        - length: length of CIGAR string
+
+        Returns:
+        cdss_protein_aln_boundary: adjusted CDS protein alignment boundary
+    """
     cds_boundary_shift = 0
     for i in range(len(cdss_protein_aln_boundary)):
         cdss_start = cdss_protein_aln_boundary[i][0] + cds_boundary_shift
         cdss_end = cdss_protein_aln_boundary[i][1] + cds_boundary_shift
         if (cdss_start <= cigar_accum_len) and (cdss_end >= cigar_accum_len):
-            # print("### cdss_start: ", cdss_start)
-            # print("### cigar_accum_len: ", cigar_accum_len)
-            # print("### cdss_end: ", cdss_end)
-            # print("### cigar_accum_len: ", cigar_accum_len)
             cds_boundary_shift += length
             cdss_end += length
         cdss_protein_aln_boundary[i] = (cdss_start, cdss_end)
     return cdss_protein_aln_boundary
 
 
-# Map the CDSs boundaries on to the protein.
 def get_cdss_protein_boundary(cdss_lens):
+    """
+        This function maps the CDSs boundaries on to the protein.
+
+        Parameters:
+        - cdss_lens: list of CDS lengths
+
+        Returns:
+        cdss_protein_boundary: CDS protein boundary
+    """
     cdss_cumulative = [sum(cdss_lens[:i+1]) for i in range(len(cdss_lens))]
     cdss_cumulative_div = [x / 3 for x in cdss_cumulative]
     cdss_protein_boundary = {}
     for idx in range(len(cdss_cumulative_div)):
         start = cdss_cumulative_div[idx-1] if idx > 0 else 0
         end = cdss_cumulative_div[idx]
         cdss_protein_boundary[idx] = (start, end)
-    # print("cdss_cumulative : ", cdss_cumulative)
-    # print("cdss_cumulative_div : ", cdss_cumulative_div)
-    # print("cdss_protein_boundary: ", cdss_protein_boundary)
-    # print("protein_seq len : ", len(protein_seq))
     return cdss_protein_boundary
 
 
 def parasail_align_protein_base(protein_seq, ref_protein_seq):
+    """
+        This is the base function that uses parasail to align the protein sequence to the reference protein sequence.
+
+        Parameters:
+        - protein_seq: protein sequence in string format
+        - ref_protein_seq: reference protein sequence in string format
+
+        Returns:
+        extracted_parasail_res: parasail alignment result
+    """
     matrix = parasail.Matrix("blosum62")
     gap_open = 11
     gap_extend = 1
-    extracted_seq = str(protein_seq)
-    reference_seq = str(ref_protein_seq)
-    extracted_seq = "*" if extracted_seq == "" else extracted_seq
-    # (Query, Reference)
-    extracted_parasail_res = parasail.nw_trace_scan_sat(extracted_seq, reference_seq, gap_open, gap_extend, matrix)
-    return extracted_parasail_res, extracted_seq, reference_seq
+    protein_seq = "*" if protein_seq == "" else protein_seq
+    # Return: (Query, Target)
+    extracted_parasail_res = parasail.nw_trace_scan_sat(protein_seq, ref_protein_seq, gap_open, gap_extend, matrix)
+    return extracted_parasail_res
 
 
 def protein_align(protein_seq, ref_protein_seq):
-    protein_seq = protein_seq.upper()
-    extracted_parasail_res, extracted_seq, reference_seq = parasail_align_protein_base(protein_seq, str(ref_protein_seq))
+    """
+        This function aligns the protein sequence to the reference protein sequence and extracts the alignment information.
+
+        Parameters:
+        - protein_seq: protein sequence in string format
+        - ref_protein_seq: reference protein sequence in string format
+
+        Returns:
+        lifton_aln: Lifton_Alignment object
+    """
+    extracted_parasail_res = parasail_align_protein_base(protein_seq, ref_protein_seq)
     alignment_query = extracted_parasail_res.traceback.query
     alignment_comp = extracted_parasail_res.traceback.comp
     alignment_ref = extracted_parasail_res.traceback.ref
-    # print("alignment_query: ", alignment_query)
-    # print("alignment_comp : ", alignment_comp)
-    # print("alignment_ref  : ", alignment_ref)
     extracted_matches, extracted_length = get_id_fraction.get_AA_id_fraction(extracted_parasail_res.traceback.ref, extracted_parasail_res.traceback.query)
     extracted_identity = extracted_matches/extracted_length
-    lifton_aln = lifton_class.Lifton_Alignment(extracted_identity, None, alignment_query, alignment_comp, alignment_ref, None, None, extracted_seq, reference_seq, None)
+    lifton_aln = lifton_class.Lifton_Alignment(extracted_identity, None, alignment_query, alignment_comp, alignment_ref, None, None, protein_seq, ref_protein_seq, None)
     return lifton_aln
 
 
 def parasail_align_DNA_base(trans_seq, ref_trans_seq):
+    """
+        This is the base function that uses parasail to align the transcript sequence to the reference transcript sequence.
+
+        Parameters:
+        - trans_seq: transcript sequence in string format
+        - ref_trans_seq: reference transcript sequence in string format
+
+        Returns:
+        extracted_parasail_res: parasail alignment result
+    """
     matrix = parasail.matrix_create("ACGT*", 1, -3)
     gap_open = 5
     gap_extend = 2
-    extracted_seq = str(trans_seq)
-    reference_seq = str(ref_trans_seq)
-    # (Query, Reference)
-    extracted_parasail_res = parasail.nw_trace_scan_sat(extracted_seq, reference_seq, gap_open, gap_extend, matrix)
-    return extracted_parasail_res, extracted_seq, reference_seq
+    # Return: (Query, Target)
+    extracted_parasail_res = parasail.nw_trace_scan_sat(trans_seq, ref_trans_seq, gap_open, gap_extend, matrix)
+    return extracted_parasail_res
 
 
 def trans_align(trans_seq, ref_trans_seq):
-    trans_seq = trans_seq.upper()
-    extracted_parasail_res, extracted_seq, reference_seq = parasail_align_DNA_base(trans_seq, str(ref_trans_seq))
+    """
+        This function aligns the transcript sequence to the reference transcript sequence and extracts the alignment information.
+
+        Parameters:
+        - trans_seq: transcript sequence in string format
+        - ref_trans_seq: reference transcript sequence in string format
+
+        Returns:
+        lifton_aln: Lifton_Alignment object
+    """
+    extracted_parasail_res = parasail_align_DNA_base(trans_seq, ref_trans_seq)
     alignment_query = extracted_parasail_res.traceback.query
     alignment_comp = extracted_parasail_res.traceback.comp
     alignment_ref = extracted_parasail_res.traceback.ref
     # print("alignment_query: ", alignment_query) 
     # print("alignment_comp: ", alignment_comp) 
     # print("alignment_ref: ", alignment_ref) 
     extracted_matches, extracted_length = get_id_fraction.get_DNA_id_fraction(extracted_parasail_res.traceback.ref, extracted_parasail_res.traceback.query)
     extracted_identity = extracted_matches/extracted_length
-    lifton_aln = lifton_class.Lifton_Alignment(extracted_identity, None, alignment_query, alignment_comp, alignment_ref, None, None, extracted_seq, reference_seq, None)
+    lifton_aln = lifton_class.Lifton_Alignment(extracted_identity, None, alignment_query, alignment_comp, alignment_ref, None, None, trans_seq, ref_trans_seq, None)
     return lifton_aln
 
 
-def LiftOn_translate(tool, lifton_trans, db_entry, fai, ref_proteins, ref_trans_id):
-    ref_protein_seq = str(ref_proteins[ref_trans_id])
+def LiftOn_translate(lifton_trans, fai, ref_proteins, ref_trans_id):
+    """
+        This function translates the given annotation.
+        
+        Parameters:
+        - lifton_trans: LiftOn transcript instance
+        - fai: fasta index
+        - ref_proteins: reference protein dictionary
+        - ref_trans_id: reference transcript ID
+
+        Returns:
+        Referece protein sequence (in string), translated protein sequence (in string), CDS lengths, CDS children
+    """
     coding_seq, cds_children, cdss_lens = lifton_trans.get_coding_seq(fai)
+    coding_seq, _ = lifton_trans.get_coding_trans_seq(fai)
     protein_seq = lifton_trans.translate_coding_seq(coding_seq)
     # print("protein_seq: ", protein_seq)
-    return ref_protein_seq, protein_seq, cdss_lens, cds_children
+    return str(ref_proteins[ref_trans_id]), protein_seq, cdss_lens, cds_children
 
 
-def parasail_align(tool, lifton_trans, db_entry, fai, ref_proteins, ref_trans_id, lifton_status):
+def lifton_parasail_align(lifton_trans, db_entry, fai, ref_proteins, ref_trans_id):
+    """
+        This function aligns the annotated protein sequence to the reference protein sequence
+
+        Parameters:
+        - lifton_trans: LiftOn transcript instance
+        - db_entry: database entry
+        - fai: fasta index
+        - ref_proteins: reference protein dictionary
+        - ref_trans_id: reference transcript ID
+        - lifton_status: LiftOn status
+
+        Returns:
+        aln: Lifton_Alignment object
+    """
     # Step 1: Check if the ref_trans_id is in the reference protein dictionary
     aln = None
     if ref_trans_id not in ref_proteins.keys():
         return aln
     # Step 2: Translate the given annotation
-    ref_protein_seq, protein_seq, cdss_lens, cds_children = LiftOn_translate(tool, lifton_trans, db_entry, fai, ref_proteins, ref_trans_id)
+    ref_protein_seq, protein_seq, cdss_lens, cds_children = LiftOn_translate(lifton_trans, fai, ref_proteins, ref_trans_id)
     # Step 3: Get the corresponding protein boundaries for each CDS
     cdss_protein_boundary = get_cdss_protein_boundary(cdss_lens)
     # Step 4: Protein alignment
     if protein_seq == None:
         return aln
-    protein_seq = protein_seq.upper()
-    extracted_parasail_res, extracted_seq, reference_seq = parasail_align_protein_base(protein_seq, ref_protein_seq)
+    extracted_parasail_res = parasail_align_protein_base(protein_seq, ref_protein_seq)
     # Step 5: Extract the alignment information
     alignment_query = extracted_parasail_res.traceback.query
     alignment_comp = extracted_parasail_res.traceback.comp
     alignment_ref = extracted_parasail_res.traceback.ref
     cigar = extracted_parasail_res.cigar
     decoded_cigar = cigar.decode.decode()
     cigar_ls = list(Cigar(decoded_cigar).items())
@@ -123,25 +190,11 @@
     cdss_protein_aln_boundary = cdss_protein_boundary.copy()
     for length, symbol in cigar_ls:
         if symbol == "D":
             # print(length, symbol)
             cdss_protein_aln_boundary = adjust_cdss_protein_boundary(cdss_protein_aln_boundary, cigar_accum_len, length)
         cigar_accum_len += length
         # print("cigar_accum_len: ", cigar_accum_len)
-    # print("cdss_protein_boundary    : ", cdss_protein_boundary)
-    # print("cdss_protein_aln_boundary: ", cdss_protein_aln_boundary)
-    # print("\t>> alignment_query: ", len(alignment_query))
-    # print("\t>> alignment_comp: ", len(alignment_comp))
-    # print("\t>> alignment_ref : ", len(alignment_ref))
     extracted_matches, extracted_length = get_id_fraction.get_AA_id_fraction(extracted_parasail_res.traceback.ref, extracted_parasail_res.traceback.query)
     extracted_identity = extracted_matches/extracted_length
-    aln = lifton_class.Lifton_Alignment(extracted_identity, cds_children, alignment_query, alignment_comp, alignment_ref, cdss_protein_boundary, cdss_protein_aln_boundary, extracted_seq, reference_seq, db_entry)
-    if tool == "liftoff":
-        # SETTING Liftoff identity score
-        lifton_status.liftoff = aln.identity
-    elif tool == "miniprot":
-        # SETTING miniprot identity score
-        lifton_status.miniprot = aln.identity
-    elif tool == "lifton":
-        # SETTING miniprot identity score
-        lifton_status.lifton_aa = aln.identity
+    aln = lifton_class.Lifton_Alignment(extracted_identity, cds_children, alignment_query, alignment_comp, alignment_ref, cdss_protein_boundary, cdss_protein_aln_boundary, protein_seq, ref_protein_seq, db_entry)
     return aln
```

### Comparing `lifton-0.0.2/lifton/annotation.py` & `lifton-0.0.3/lifton/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 
     def get_db_connnection(self):
         try:
             feature_db = gffutils.FeatureDB(self.file_name)
         except:
             feature_db = self.build_database()
-        
         # print("feature_db: ", feature_db)
         # feature_db.execute('ANALYZE features')
         self.db_connection = feature_db
 
 
     def build_database(self):
         if self.infer_genes:
@@ -29,15 +28,14 @@
         else:
             disable_genes = True
         try:
             transform_func = self.get_transform_func()
             feature_db = gffutils.create_db(self.file_name, self.file_name + "_db", 
                                         merge_strategy="create_unique", 
                                         # merge_strategy="warning",
-                                            # merge_strategy="create_unique", 
                                         id_spec='ID',
                                         force=True,
                                         verbose=True, disable_infer_transcripts=True,
                                             disable_infer_genes=disable_genes, transform=transform_func)
             
         except Exception as e:
             print("gffutils database build failed with", e)
```

### Comparing `lifton-0.0.2/lifton/extract_sequence.py` & `lifton-0.0.3/lifton/extract_sequence.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     for feature in features:
         for locus in ref_db.db_connection.features_of_type(feature):
             __inner_extract_feature(ref_db, locus, ref_fai, ref_trans, ref_proteins)
     return ref_trans, ref_proteins
 
 
 def __inner_extract_feature(ref_db, feature, ref_fai, ref_trans, ref_proteins):
-    # for children in ref_db.db_connection.children(feature, featuretype='exon', order_by='start'):
     # If exon is the first level children
     children_exons = list(ref_db.db_connection.children(feature, featuretype='exon', level=1))
     children_CDSs = list(ref_db.db_connection.children(feature, featuretype=('start_codon', 'CDS', 'stop_codon'), level=1))
     if len(children_exons) > 0 or len(children_CDSs) > 0:
         # print(f"Parent: {feature.id};  exon: {len(children_exons)}; CDS: {len(children_CDSs)}")
         if len(children_exons) > 0:
             trans_seq = get_dna_sequence(feature, ref_fai, children_exons)
```

### Comparing `lifton-0.0.2/lifton/fix_trans_annotation.py` & `lifton-0.0.3/lifton/protein_maximization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from lifton import get_id_fraction, lifton_class, logger
 import math
 
 def get_protein_boundary(cdss_aln_boundary, c_idx_last, c_idx, DEBUG):
     aa_start = cdss_aln_boundary[c_idx_last][0]
     aa_end = cdss_aln_boundary[c_idx-1][1]
-    # logger.log(f"\t### protein chunk boundaries: {aa_start} - {aa_end}", debug=DEBUG)
     return aa_start, aa_end
 
 
 def get_protein_reference_length_single(lifton_aln, c_idx, DEBUG):
     aa_start = 0
     aa_end = lifton_aln.cdss_protein_aln_boundaries[c_idx][1]
     aa_end = math.ceil(aa_end)
@@ -73,21 +72,14 @@
     l_c_idx = 0
     m_c_idx_last = m_c_idx
     l_c_idx_last = l_c_idx
     cds_list = []
     ref_aa_liftoff_count = 0
     ref_aa_miniprot_count = 0
     chains = []
-    # # Directly adopting Liftoff's annptation. Miniprot is likely to be pseudogene.
-    # if len(m_children) == 1 and len(l_children) > 1:
-    #     chains = ['liftoff']
-    #     for liftoff_cds in l_children:
-    #         cds = lifton_class.Lifton_CDS(liftoff_cds)
-    #         cds_list.append(cds)
-    #     return cds_list, chains
     while m_c_idx != (len(m_children)-1) or l_c_idx != (len(l_children)-1):
         if (m_c_idx == len(m_children)-1) and (l_c_idx < (len(l_children)-1)):
             l_c_idx, ref_aa_liftoff_count = push_cds_idx(l_c_idx, l_lifton_aln, ref_aa_liftoff_count, DEBUG)
             continue
         if (m_c_idx < len(m_children)-1) and (l_c_idx == (len(l_children)-1)):
             m_c_idx, ref_aa_miniprot_count = push_cds_idx(m_c_idx, m_lifton_aln, ref_aa_miniprot_count, DEBUG)
             continue
```

### Comparing `lifton-0.0.2/lifton/get_id_fraction.py` & `lifton-0.0.3/lifton/get_id_fraction.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         return matches, 1
     return matches, total_length
 
 
 # Gap-collapsed protein sequence identity
 def get_AA_id_fraction(reference, target):
     matches = 0
+    # gap-compressed BLAST identity
     reference = reference.upper()
     target = target.upper()
     gaps_in_ref = 0
     for i, letter in enumerate(reference):
         if letter == '-':
             gaps_in_ref += 1
         if letter == target[i]:
```

### Comparing `lifton-0.0.2/lifton/intervals.py` & `lifton-0.0.3/lifton/intervals.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.2/lifton/liftoff/align_features.py` & `lifton-0.0.3/lifton/liftoff/align_features.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.2/lifton/liftoff/aligned_seg.py` & `lifton-0.0.3/lifton/liftoff/aligned_seg.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.2/lifton/liftoff/extract_features.py` & `lifton-0.0.3/lifton/liftoff/extract_features.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.2/lifton/liftoff/find_best_mapping.py` & `lifton-0.0.3/lifton/liftoff/find_best_mapping.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.2/lifton/liftoff/fix_overlapping_features.py` & `lifton-0.0.3/lifton/liftoff/fix_overlapping_features.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.2/lifton/liftoff/lift_features.py` & `lifton-0.0.3/lifton/liftoff/lift_features.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.2/lifton/liftoff/liftoff_main.py` & `lifton-0.0.3/lifton/liftoff/liftoff_main.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.2/lifton/liftoff/liftoff_utils.py` & `lifton-0.0.3/lifton/liftoff/liftoff_utils.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.2/lifton/liftoff/liftover_types.py` & `lifton-0.0.3/lifton/liftoff/liftover_types.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.2/lifton/liftoff/merge_lifted_features.py` & `lifton-0.0.3/lifton/liftoff/merge_lifted_features.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.2/lifton/liftoff/polish.py` & `lifton-0.0.3/lifton/liftoff/polish.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.2/lifton/liftoff/tests/test_advanced.py` & `lifton-0.0.3/lifton/liftoff/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.2/lifton/liftoff/tests/test_basic.py` & `lifton-0.0.3/lifton/liftoff/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.2/lifton/liftoff/write_new_gff.py` & `lifton-0.0.3/lifton/liftoff/write_new_gff.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.2/lifton/lifton.py` & `lifton-0.0.3/lifton/lifton.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from lifton import mapping, intervals, lifton_utils, annotation, extract_sequence, stats, logger, run_miniprot, run_liftoff, evaluation, __version__
+from lifton import mapping, intervals, lifton_utils, annotation, extract_sequence, stats, logger, run_liftoff, run_miniprot, run_evaluation, __version__
 from intervaltree import Interval
 import argparse
-from argparse import Namespace
-from pyfaidx import Fasta, Faidx
-import os
-from concurrent.futures import ProcessPoolExecutor
+from pyfaidx import Fasta
+import os, sys
 
 def args_outgrp(parser):
     outgrp = parser.add_argument_group('* Output settings')
     outgrp.add_argument(
         '-o', '--output', default='lifton.gff3', metavar='FILE',
         help='write output to FILE in same format as input; by default, output is written to "lifton.gff3"'
     )
@@ -37,14 +35,22 @@
     )
     aligngrp.add_argument(
         '-s', default=0.5, metavar='S', type=float,
         help='designate a feature mapped only if its child features (usually exons/CDS) align '
              'with sequence identity ≥S; by default S=0.5'
     )
     aligngrp.add_argument(
+        '-min_miniprot', default=0.9, metavar='MIN_MINIPROT', type=float,
+        help='The minimum length ratio of a protein-coding transcript to the longest protein-coding transcript within a gene locus, as identified exclusively by miniprot in the target genome, is set by default to MIN_MINIPROT=0.9.'
+    )
+    aligngrp.add_argument(
+        '-max_miniprot', default=1.5, metavar='MAX_MINIPROT', type=float,
+        help='The maximum length ratio of a protein-coding transcript to the longest protein-coding transcript within a gene locus, as identified exclusively by miniprot in the target genome, is set by default to MIN_MINIPROT=1.5.'
+    )
+    aligngrp.add_argument(
         '-d', metavar='D', default=2.0, type=float,
         help='distance scaling factor; alignment nodes separated by more than a factor of D in '
              'the target genome will not be connected in the graph; by default D=2.0'
     )
     aligngrp.add_argument(
         '-flank', default=0, metavar='F', type=float, help="amount of flanking sequence to align as a "
                                                            "fraction [0.0-1.0] of gene length. This can improve gene "
@@ -139,14 +145,15 @@
     miniprotrefrgrp = parser.add_argument_group('* Optional input (miniprot annotation)')
     miniprotrefrgrp.add_argument(
         '-M', '--miniprot', metavar='gff', default=None,
         help='the annotation generated by miniprot (or) '
                 'name of miniprot gffutils database; if not specified, the -miniprot '
                 'argument must be provided and a database will be built automatically'
     )
+    parser.add_argument('-ad', '--annotation-database', metavar='SOURCE', help='The source of the reference annotation (RefSeq / GENCODE / others).', default = "RefSeq")
     ###################################
     # END for the LiftOn params
     ###################################
     parser._positionals.title = '* Required input (sequences)'
     parser._optionals.title = '* Miscellaneous settings'
     parser._action_groups = [parser._positionals, referencegrp, referenceseqgrp, liftoffrefrgrp, miniprotrefrgrp, parser_outgrp, parser._optionals, parser_aligngrp]
     args = parser.parse_args(arglist)
@@ -169,43 +176,43 @@
 
 def run_all_lifton_steps(args):
     ################################
     # Step 0: Reading target & reference genomes
     ################################
     tgt_genome = args.target
     ref_genome = args.reference
-    DEBUG = args.debug
-    # Setting output directory & intermediate_dir
     if args.output == "stdout": 
         outdir = "."
     else:
         outdir = os.path.dirname(args.output)
         outdir = outdir if outdir != "" else "."
         os.makedirs(outdir, exist_ok=True)
     lifton_outdir = f"{outdir}/lifton_output/"
     args.directory = "intermediate_files/"
     intermediate_dir = f"{outdir}/lifton_output/{args.directory}"
+    stats_dir= f"{outdir}/lifton_output/stats/"
     os.makedirs(intermediate_dir, exist_ok=True)
+    os.makedirs(stats_dir, exist_ok=True)
     args.directory = intermediate_dir
     logger.log(">> Reading target genome ...", debug=True)
     tgt_fai = Fasta(tgt_genome)
     logger.log(">> Reading reference genome ...", debug=True)
-    ref_fai = Fasta(ref_genome)
+    ref_fai = Fasta(ref_genome)    
 
     ################################
     # Step 1: Building database from the reference annotation
     ################################
     logger.log("\n>> Creating reference annotation database : ", args.reference_annotation, debug=True)
     ref_db = annotation.Annotation(args.reference_annotation, args.infer_genes)
 
     ################################
     # Step 2: Get all reference features to liftover
     ################################
     features = lifton_utils.get_parent_features_to_lift(args.features)
-    ref_features_dict, ref_features_reverse_dict = lifton_utils.get_ref_liffover_features(features, ref_db)
+    ref_features_dict, ref_features_len_dict, ref_features_reverse_dict, ref_trans_exon_num_dict = lifton_utils.get_ref_liffover_features(features, ref_db, intermediate_dir, args)
 
     ################################
     # Step 3: Extract protein & DNA dictionaries from the selected reference features
     ################################
     ref_trans_file = args.transcripts    
     ref_proteins_file = args.proteins    
     if (ref_proteins_file is None) or (not os.path.exists(ref_proteins_file)) or (ref_trans_file is None) or (not os.path.exists(ref_trans_file)):
@@ -218,119 +225,113 @@
         logger.log(">> Reading transcript DNA dictionary from the reference fasta ...", debug=True)
         logger.log(">> Reading transcript protein dictionary from the reference fasta ...", debug=True)
         ref_trans = Fasta(ref_trans_file)
         ref_proteins = Fasta(ref_proteins_file)
     logger.log("\t * number of transcripts: ", len(ref_trans.keys()), debug=True)
     logger.log("\t * number of proteins: ", len(ref_proteins.keys()), debug=True)
     trunc_ref_proteins = lifton_utils.get_truncated_protein(ref_proteins)
-    trunc_ref_proteins_file = lifton_utils.write_seq_2_file(intermediate_dir, trunc_ref_proteins, "truncated_proteins")
     logger.log("\t\t * number of truncated proteins: ", len(trunc_ref_proteins.keys()), debug=True)
 
-    # # Evaluation mode
-    # if args.evaluation:
-    #     tgt_annotation = args.output
-    #     ref_annotation = args.reference_annotation
-    #     print("Run LiftOn in evaluation mode")
-    #     print("lifton_outdir     : ", lifton_outdir)
-    #     print("Ref genome        : ", ref_genome)
-    #     print("Target genome     : ", tgt_genome)
-    #     print("Ref annotation    : ", args.reference_annotation)
-    #     print("Target annotation : ", args.output)
-    #     print("ref_trans_file    : ", ref_trans_file)
-    #     print("ref_proteins_file : ", ref_proteins_file)
-    #     logger.log(">> Creating target database : ", tgt_annotation, debug=True)
-    #     tgt_feature_db = annotation.Annotation(tgt_annotation, args.infer_genes).db_connection
-    #     fw_score = open(lifton_outdir+"/eval.txt", "w")
-    #     tree_dict = intervals.initialize_interval_tree(tgt_feature_db, features)
-    #     for feature in features:
-    #         for locus in tgt_feature_db.features_of_type(feature):#, limit=("chr1", 146652669, 146708545)):
-    #             evaluation.tgt_evaluate(None, locus, ref_db.db_connection, tgt_feature_db, tree_dict, tgt_fai, ref_features_dict, ref_proteins, ref_trans, fw_score, DEBUG)
-    #     fw_score.close()
-    #     return
+    ################################
+    # optional Step: Evaluation mode
+    ################################
+    if args.evaluation:
+        tgt_annotation = args.output
+        ref_annotation = args.reference_annotation
+        print("Run LiftOn in evaluation mode")
+        print("lifton_outdir     : ", lifton_outdir)
+        print("Ref genome        : ", ref_genome)
+        print("Target genome     : ", tgt_genome)
+        print("Ref annotation    : ", args.reference_annotation)
+        print("Target annotation : ", args.output)
+        print("ref_trans_file    : ", ref_trans_file)
+        print("ref_proteins_file : ", ref_proteins_file)
+        logger.log(">> Creating target database : ", tgt_annotation, debug=True)
+        os.makedirs(lifton_outdir, exist_ok=True)
+        tgt_feature_db = annotation.Annotation(tgt_annotation, args.infer_genes).db_connection
+        fw_score = open(lifton_outdir+"/eval.txt", "w")
+        tree_dict = {}
+        processed_features = 0
+        for feature in features:
+            for locus in tgt_feature_db.features_of_type(feature):#, limit=("chr1", 146652669, 146708545)):
+                # evaluation.tgt_evaluate(None, locus, ref_db.db_connection, tgt_feature_db, tree_dict, tgt_fai, ref_features_dict, ref_proteins, ref_trans, fw_score, args.debug)
+                lifton_gene = run_evaluation.evaluation(None, locus, ref_db.db_connection, tgt_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, args, ENTRY_FEATURE=True)
+                if processed_features % 20 == 0:
+                    sys.stdout.write("\r>> LiftOn evaluated: %i features." % processed_features)
+                processed_features += 1
+        fw_score.close()
+        return
 
-    # LiftOn mode
     ################################
     # Step 4: Run liftoff & miniprot
     ################################
     liftoff_annotation = lifton_utils.exec_liftoff(lifton_outdir, args)
     miniprot_annotation = lifton_utils.exec_miniprot(lifton_outdir, args, tgt_genome, ref_proteins_file)
 
     ################################
     # Step 5: Create liftoff and miniprot database
     ################################
-    logger.log("\n>> Creating liftoff annotation database : ", liftoff_annotation, debug=True)
+    logger.log(f"\n>> Creating liftoff annotation database : {liftoff_annotation}", debug=True)
     l_feature_db = annotation.Annotation(liftoff_annotation, args.infer_genes).db_connection
-    logger.log("\n>> Creating miniprot annotation database : ", miniprot_annotation, debug=True)
+    logger.log(f">> Creating miniprot annotation database : {miniprot_annotation}", debug=True)
     m_feature_db = annotation.Annotation(miniprot_annotation, args.infer_genes).db_connection
-
-    # Open output files
     fw = open(args.output, "w")
     fw_score = open(f"{lifton_outdir}/score.txt", "w")
-    fw_unmapped = open(f"{lifton_outdir}/unmapped_features.txt", "w")
-    fw_extra_copy = open(f"{lifton_outdir}/extra_copy_features.txt", "w")
-    if args.write_chains:
-        fw_chain = open(f"{lifton_outdir}/chain.txt", "w")
-    else:
-        fw_chain = None
-
-    ################################
-    # Step 6: Creating miniprot 2 Liftoff ID mapping
-    ################################
-    ref_id_2_m_id_trans_dict, m_id_2_ref_id_trans_dict = mapping.miniprot_id_mapping(m_feature_db)
+    fw_unmapped = open(f"{stats_dir}/unmapped_features.txt", "w")
+    fw_extra_copy = open(f"{stats_dir}/extra_copy_features.txt", "w")
+    fw_mapped_feature = open(f'{stats_dir}/mapped_feature.txt', 'w')
+    fw_mapped_trans = open(f'{stats_dir}/mapped_transcript.txt', 'w')
+    fw_chain = open(f"{lifton_outdir}/chain.txt", "w") if args.write_chains else None
 
     ################################
-    # Step 7: Initializing intervaltree
+    # Step 6: Creating miniprot 2 Liftoff ID mapping & Initializing intervaltree
     ################################
+    ref_id_2_m_id_trans_dict, m_id_2_ref_id_trans_dict = lifton_utils.miniprot_id_mapping(m_feature_db)
     tree_dict = intervals.initialize_interval_tree(l_feature_db, features)
-
+    transcripts_stats_dict = {'coding': {}, 'non-coding': {}, 'other': {}}
+    processed_features = 0
+    
     ################################
-    # Step 8: Process Liftoff genes & transcripts
+    # Step 7: Process Liftoff genes & transcripts
     #     structure 1: gene -> transcript -> exon
     #     structure 2: transcript -> exon
     ################################
-    for feature in features:
-        for locus in l_feature_db.features_of_type(feature):#, limit=("NW_020825194.1", 28072487, 28072684)):
-            lifton_gene = run_liftoff.process_liftoff(None, locus, ref_db.db_connection, l_feature_db, ref_id_2_m_id_trans_dict, m_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, fw_chain, args.write_chains, DEBUG)
-            # Writing out LiftOn entries
-            lifton_gene.write_entry(fw)
+    for feature in features:#CP132235.1:34100723-34103135
+        for locus in l_feature_db.features_of_type(feature):#, limit=("CP132235.1", 34100723, 34303135)):
+            lifton_gene = run_liftoff.process_liftoff(None, locus, ref_db.db_connection, l_feature_db, ref_id_2_m_id_trans_dict, m_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, fw_chain, args, ENTRY_FEATURE=True)
+            if lifton_gene is None or lifton_gene.ref_gene_id is None:
+                continue
+            lifton_gene.write_entry(fw,transcripts_stats_dict)
+            if processed_features % 20 == 0:
+                sys.stdout.write("\r>> LiftOn processed: %i features." % processed_features)
+            processed_features += 1
 
     ################################
-    # Step 9: Process miniprot transcripts
+    # Step 8: Process miniprot transcripts
     ################################
     for mtrans in m_feature_db.features_of_type('mRNA'):
-        mtrans_id = mtrans.attributes["ID"][0]
-        mtrans_interval = Interval(mtrans.start, mtrans.end, mtrans_id)
-        is_overlapped = lifton_utils.check_ovps_ratio(mtrans, mtrans_interval, args.overlap, tree_dict)
-        if not is_overlapped:
-            ref_trans_id = m_id_2_ref_id_trans_dict[mtrans_id]            
-            # Link the reference trans ID to feature
-            ref_gene_id, ref_trans_id = lifton_utils.get_ref_ids_miniprot(ref_features_reverse_dict, mtrans_id, m_id_2_ref_id_trans_dict)
-            logger.log(f"miniprot: ref_gene_id: {ref_gene_id};  ref_trans_id: {ref_trans_id}\t: ", debug=DEBUG)
-            if ref_trans_id in ref_proteins.keys() and ref_trans_id in ref_trans.keys():
-                # The transcript match the reference transcript
-                if ref_trans_id != None:
-                    lifton_gene, transcript_id, lifton_status = run_miniprot.lifton_miniprot_with_ref_protein(mtrans, m_feature_db, ref_db.db_connection, ref_gene_id, ref_trans_id, tgt_fai, ref_proteins, ref_trans, tree_dict, ref_features_dict, DEBUG)
-                else:
-                    ref_gene_id = "LiftOn-gene"
-                    lifton_gene, transcript_id, lifton_status = run_miniprot.lifton_miniprot_no_ref_protein(mtrans, m_feature_db, ref_gene_id, ref_trans_id, ref_features_dict, tree_dict, DEBUG)
-            lifton_gene.add_lifton_status_attrs(transcript_id, lifton_status)
-            lifton_utils.write_lifton_status(fw_score, transcript_id, mtrans, lifton_status)
-            lifton_gene.write_entry(fw)
+        lifton_gene = run_miniprot.process_miniprot(mtrans, ref_db, m_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, m_id_2_ref_id_trans_dict, ref_features_len_dict, ref_trans_exon_num_dict, ref_features_reverse_dict, args)
+        if lifton_gene is None or lifton_gene.ref_gene_id is None:
+            continue
+        lifton_gene.write_entry(fw, transcripts_stats_dict)
+        if processed_features % 20 == 0:
+            sys.stdout.write("\r>> LiftOn processed: %i features." % processed_features)
+        processed_features += 1
 
     ################################
-    # Step 10: Printing stats
+    # Step 9: Printing stats
     ################################
-    stats.print_report(ref_features_dict, fw_unmapped, fw_extra_copy, debug=DEBUG)
-    # Close output files
+    stats.print_report(ref_features_dict, transcripts_stats_dict, fw_unmapped, fw_extra_copy, fw_mapped_feature, fw_mapped_trans, debug=args.debug)
     fw.close()
     fw_score.close()
     fw_unmapped.close()
     fw_extra_copy.close()
-    if args.write_chains:
-        fw_chain.close()
+    fw_mapped_feature.close()
+    fw_mapped_trans.close()
+    if args.write_chains: fw_chain.close()
 
 
 def main(arglist=None):
     banner = '''
 ====================================================================
 An accurate homology lift-over tool between assemblies
 ====================================================================
@@ -339,11 +340,11 @@
     ██╗     ██╗███████╗████████╗ ██████╗ ███╗   ██╗
     ██║     ██║██╔════╝╚══██╔══╝██╔═══██╗████╗  ██║
     ██║     ██║█████╗     ██║   ██║   ██║██╔██╗ ██║
     ██║     ██║██╔══╝     ██║   ██║   ██║██║╚██╗██║
     ███████╗██║██║        ██║   ╚██████╔╝██║ ╚████║
     ╚══════╝╚═╝╚═╝        ╚═╝    ╚═════╝ ╚═╝  ╚═══╝
     '''
-    print(banner)
-    print(f"{__version__}\n")
+    print(banner, file=sys.stderr)
+    print(f"{__version__}\n", file=sys.stderr)
     args = parse_args(arglist)
     run_all_lifton_steps(args)
```

### Comparing `lifton-0.0.2/lifton/lifton_class.py` & `lifton-0.0.3/lifton/lifton_class.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,50 +46,52 @@
 
     
 class Lifton_feature:
     def __init__(self, id):
         self.id = id
         self.copy_num = 0
         self.is_protein_coding = False
+        self.is_non_coding = False
         self.children = set()
 
 
 class Lifton_GENE:
-    def __init__(self, ref_gene_id, gffutil_entry_gene, ref_gene_attrs, tree_dict, ref_features_dict, miniprot_holder = False, tmp = False):
+    def __init__(self, ref_gene_id, gffutil_entry_gene, ref_gene_attrs, tree_dict, ref_features_dict, args, tmp = False):
         ###########################
         # Assigning the reference gene & attributes
         ###########################
         self.entry = gffutil_entry_gene
         self.entry.source = "LiftOn"
-        self.entry.featuretype = "gene"
+        self.is_protein_coding = False
+        self.is_non_coding = False
         self.transcripts = {}
         self.ref_gene_id = ref_gene_id
         self.copy_num = self.__get_gene_copy(ref_features_dict)
-        self.miniprot_holder = miniprot_holder
         self.tmp = tmp
-        # This is for miniprot
-        if self.miniprot_holder:
-            attributes = {}
-            # attributes["ID"] = self.entry.attributes["Parent"] if "Parent" in self.entry.attributes.keys() else ["LiftOn-gene_" + str(ref_features_dict["LiftOn-gene"].copy_num)]
-            attributes["ID"] = ["LiftOn-gene_" + str(ref_features_dict["LiftOn-gene"].copy_num)]
-
-            ref_features_dict["LiftOn-gene"].copy_num += 1
-            self.entry.attributes = attributes
-            # print("Holder self.entry.attributes: ", self.entry.attributes)
-        else:
-            self.entry.attributes = ref_gene_attrs
-            self.entry.attributes["ID"] = self.ref_gene_id + "_" + str(self.copy_num) if self.copy_num > 0 else self.ref_gene_id
-            if self.copy_num > 0:
-                self.entry.attributes["extra_copy_number"] = [str(self.copy_num)]        
+        self.entry.attributes = ref_gene_attrs
+        self.entry.attributes["ID"] = self.ref_gene_id + "_" + str(self.copy_num) if self.copy_num > 0 else self.ref_gene_id
+        if self.copy_num > 0:
+            self.entry.attributes["extra_copy_number"] = [str(self.copy_num)]        
         self.__update_gene_copy(ref_features_dict)
         self.entry.id = self.entry.attributes["ID"][0]
         gene_interval = Interval(self.entry.start, self.entry.end, self.entry.id)
         if self.entry.seqid not in tree_dict.keys():
             tree_dict[self.entry.seqid] = IntervalTree()
         tree_dict[self.entry.seqid].add(gene_interval)
+        # Decide if its type
+        gene_type_key = ""
+        if args.annotation_database.upper() == "REFSEQ":
+            gene_type_key = "gene_biotype"
+        elif args.annotation_database.upper() == "GENCODE" or args.annotation_database.upper() == "ENSEMBL" or args.annotation_database.upper() == "CHESS":
+            gene_type_key = "gene_type"
+        if gene_type_key in self.entry.attributes.keys():
+            if self.entry.attributes[gene_type_key][0] == "protein_coding":
+                self.is_protein_coding = True
+            elif (self.entry.attributes[gene_type_key][0] == "lncRNA" or self.entry.attributes[gene_type_key][0] == "ncRNA"):
+                self.is_non_coding = True
         
     def __get_gene_copy(self, ref_features_dict):
         if 'extra_copy_number' in self.entry.attributes:
             return int(self.entry.attributes['extra_copy_number'][0])
         else:
             if self.ref_gene_id in ref_features_dict.keys():
                 return ref_features_dict[self.ref_gene_id].copy_num
@@ -98,81 +100,79 @@
 
     def __update_gene_copy(self, ref_features_dict):
         if self.ref_gene_id in ref_features_dict.keys():
             ref_features_dict[self.ref_gene_id].copy_num += 1
 
     def update_gene_info(self, chromosome, start, end):
         self.entry.seqid = chromosome
-        self.entry.featuretype = "gene"
         self.entry.start = start
         self.entry.end = end
 
     def add_miniprot_transcript(self, ref_trans_id, gffutil_entry_trans, ref_trans_attrs, ref_features_dict):
         Lifton_trans = Lifton_TRANS(ref_trans_id, self.ref_gene_id, self.entry.id, self.copy_num, gffutil_entry_trans, ref_trans_attrs)
         self.transcripts[Lifton_trans.entry.id] = Lifton_trans
         return Lifton_trans
     
     def update_trans_info(self, trans_id, chromosome, start, end):
         self.transcripts[trans_id].entry.seqid = chromosome
-        self.transcripts[trans_id].entry.featuretype = "mRNA"
         self.transcripts[trans_id].entry.start = start
         self.transcripts[trans_id].entry.end = end
 
     def add_transcript(self, ref_trans_id, gffutil_entry_trans, ref_trans_attrs):
         Lifton_trans = Lifton_TRANS(ref_trans_id, self.ref_gene_id, self.entry.id, self.copy_num, gffutil_entry_trans, ref_trans_attrs)
         self.transcripts[Lifton_trans.entry.id] = Lifton_trans
         return Lifton_trans
 
     def add_feature(self, gffutil_entry_trans):
         Lifton_feature = LiftOn_FEATURE(self.entry.id, gffutil_entry_trans, self.copy_num)
         self.transcripts[Lifton_feature.entry.id] = Lifton_feature
         return Lifton_feature
 
-    def remove_transcript(self, transcript_id):
-        del self.transcripts[transcript_id]
-
     def add_exon(self, trans_id, gffutil_entry_exon):
         self.transcripts[trans_id].add_exon(gffutil_entry_exon)
 
     def add_cds(self, trans_id, gffutil_entry_cds):
         self.transcripts[trans_id].add_cds(gffutil_entry_cds)
                             
-    def fix_truncated_protein(self, trans_id, ref_trans_id, fai, ref_proteins, fai_trans, lifton_status):
-        ref_protein_seq = ref_proteins[ref_trans_id]
-        ref_trans_seq = fai_trans[ref_trans_id]
+    def orf_search_protein(self, trans_id, ref_trans_id, fai, ref_proteins, fai_trans, lifton_status, eval_only=False):
         if trans_id not in self.transcripts.keys():
             return None, False
-        lifton_aln, good_trans = self.transcripts[trans_id].fix_truncated_protein(fai, ref_protein_seq, ref_trans_seq, lifton_status)
+        ref_protein_seq = str(ref_proteins[ref_trans_id]) if ref_trans_id in ref_proteins else None
+        ref_trans_seq = str(fai_trans[ref_trans_id]) if ref_trans_id in fai_trans else None
+        lifton_aln, good_trans = self.transcripts[trans_id].orf_search_protein(fai, ref_protein_seq, ref_trans_seq, lifton_status, is_non_coding=self.is_non_coding, eval_only=eval_only)
         return lifton_aln, good_trans
 
-    def align_trans_dna(self, trans_id, ref_trans_id, fai, fai_trans, lifton_status):
-        ref_trans_seq = fai_trans[ref_trans_id]
-        if trans_id not in self.transcripts.keys():
-            return None
-        lifton_tran_aln = self.transcripts[trans_id].align_trans_dna(fai, ref_trans_seq, lifton_status)
-        if lifton_tran_aln.identity == 1:
-            lifton_status.annotation = "Liftoff_identical"
-            lifton_status.status = ["identical"]
-        elif lifton_tran_aln.identity < 1:
-            lifton_status.annotation = "Liftoff_synonymous"
-            lifton_status.status = ["synonymous"]
-        return lifton_tran_aln
-
     def update_cds_list(self, trans_id, cds_list):
         self.transcripts[trans_id].update_cds_list(cds_list)
         self.update_boundaries()
 
-    def add_lifton_status_attrs(self, trans_id, lifton_status):
-        self.transcripts[trans_id].add_lifton_status_attrs(lifton_status)
+    def add_lifton_gene_status_attrs(self, source):
+        self.entry.attributes["source"] = [source]
 
-    def write_entry(self, fw):
+    def add_lifton_trans_status_attrs(self, trans_id, lifton_status):
+        self.transcripts[trans_id].add_lifton_trans_status_attrs(lifton_status)
+
+    def write_entry(self, fw, transcripts_stats_dict):
         if not self.tmp:
             fw.write(str(self.entry) + "\n")
         for key, trans in self.transcripts.items():
             trans.write_entry(fw)
+            TYPE = ""
+            if self.is_protein_coding and trans.entry.featuretype == "mRNA":
+                TYPE = "coding"
+            elif self.is_non_coding and (trans.entry.featuretype == "ncRNA" or trans.entry.featuretype == "nc_RNA" or trans.entry.featuretype == "lncRNA" or trans.entry.featuretype == "lnc_RNA"):
+                TYPE = "non-coding"
+            else:
+                TYPE = "other"
+            if trans.ref_tran_id is None:
+                continue
+            if not trans.ref_tran_id in transcripts_stats_dict[TYPE].keys():
+                transcripts_stats_dict[TYPE][trans.ref_tran_id] = 1
+            else:
+                transcripts_stats_dict[TYPE][trans.ref_tran_id] += 1
 
     def update_boundaries(self):        
         for key, trans in self.transcripts.items():
             self.entry.start = trans.entry.start if trans.entry.start < self.entry.start else self.entry.start
             self.entry.end = trans.entry.end if trans.entry.end > self.entry.end else self.entry.end
 
     def print_gene(self):
@@ -184,14 +184,16 @@
 class LiftOn_FEATURE:
     def __init__(self, parent_id, gffutil_entry_feature, copy_num):
         self.entry = gffutil_entry_feature
         self.entry.source = "LiftOn"
         self.copy_num = copy_num
         self.features = {}
         self.entry.attributes["Parent"] = [parent_id]
+        self.ref_tran_id = None
+        # self.ref_tran_id = self.entry.id
         if int(copy_num) > 0:
             feature_id_base = lifton_utils.get_ID_base(self.entry.id)
             self.entry.id = f"{feature_id_base}_{copy_num}"
             self.entry.attributes["ID"] = [self.entry.id]
 
     def add_feature(self, gffutil_entry_trans):
         Lifton_feature = LiftOn_FEATURE(self.entry.id, gffutil_entry_trans, self.copy_num)
@@ -227,32 +229,29 @@
         self.ref_gene_id = ref_gene_id
         self.ref_tran_id = ref_trans_id
         if 'Parent' in self.entry.attributes:
             self.entry.attributes['Parent'] = [gene_id]
         if 'transcript_id' in self.entry.attributes:
             self.entry.attributes['transcript_id'] = [self.entry.id]
 
-    def add_lifton_status_attrs(self, lifton_status):
+    def add_lifton_trans_status_attrs(self, lifton_status):
         self.entry.attributes["protein_identity"] = [f"{lifton_status.lifton_aa:.3f}"]
         self.entry.attributes["dna_identity"] = [f"{lifton_status.lifton_dna:.3f}"]
         self.entry.attributes["status"] = [lifton_status.annotation]
 
     def add_exon(self, gffutil_entry_exon):
-        attributes = {}
-        attributes['Parent'] = [self.entry.id]
-        gffutil_entry_exon.attributes = attributes
+        gffutil_entry_exon.attributes['Parent'] = [self.entry.id]
         Lifton_exon = Lifton_EXON(gffutil_entry_exon)
         lifton_utils.custom_bisect_insert(self.exons, Lifton_exon)
 
     def add_cds(self, gffutil_entry_cds):
         for exon in self.exons:
-            if lifton_utils.segments_overlap((exon.entry.start, exon.entry.end), (gffutil_entry_cds.start, gffutil_entry_cds.end)):
-                attributes = {}
-                attributes['Parent'] = [self.entry.id]
-                gffutil_entry_cds.attributes = attributes
+            _, ovp = lifton_utils.segments_overlap_length((exon.entry.start, exon.entry.end), (gffutil_entry_cds.start, gffutil_entry_cds.end))
+            if ovp:
+                gffutil_entry_cds.attributes['Parent'] = [self.entry.id]
                 exon.add_cds(gffutil_entry_cds)
 
     def update_gffutil_entry_trans(self, gffutil_entry_trans):
         for key, atr in gffutil_entry_trans.attributes.items():
             self.entry.attributes[key] = atr
 
     def mv_exon_idx(self, exon_idx):
@@ -271,20 +270,20 @@
         ########################
         if len(cds_list) == 1:
             only_cds = cds_list[0]
             processed_ovp_exons = False
             ovp_exons = []
             while idx_exon_itr < len(self.exons):
                 exon = self.exons[idx_exon_itr]
-                # print(f"Checking overlapping: {exon.entry.start}-{exon.entry.end}; {only_cds.entry.start}-{only_cds.entry.end}")
-                # print(f"cds_idx: {cds_idx}; {only_cds.entry.start}-{only_cds.entry.end} (len: {len(cds_list)});  exon_idx: {idx_exon_itr}; {exon.entry.start}-{exon.entry.end} (len: {len(self.exons)})")
+                _, ovp = lifton_utils.segments_overlap_length((exon.entry.start, exon.entry.end), (only_cds.entry.start, only_cds.entry.end))
+
                 # |eeeeee| |ccccc|
                 if exon.entry.end < only_cds.entry.start:
                     new_exons.append(exon)
-                elif lifton_utils.segments_overlap((exon.entry.start, exon.entry.end), (only_cds.entry.start, only_cds.entry.end)):
+                elif ovp:
                     cp_exon = copy.deepcopy(exon)
                     ovp_exons.append(cp_exon)
                 # |cccc|  |eeee|
                 elif exon.entry.start > only_cds.entry.end: 
                     processed_ovp_exons = True
                     merged_exon = copy.deepcopy(exon)
                     if len(ovp_exons) == 0:
@@ -305,15 +304,14 @@
         ########################
         # Case 2: only 1 exon, and >1 CDSs
         ########################
         elif len(self.exons) == 1:
             first_exon = self.exons[0]
             for cds_idx in range(len(cds_list)):
                 exon = copy.deepcopy(first_exon)
-                
                 cds = cds_list[cds_idx]
                 if cds_idx == 0:
                     if exon.entry.start >= cds.entry.start:
                         exon.entry.start = cds.entry.start
                     exon.entry.end = cds.entry.end
                 elif cds_idx == len(cds_list)-1:
                     if exon.entry.end <= cds.entry.end:
@@ -343,120 +341,108 @@
                 init_head_order = False
             # |eeeeee| |ccccc|
             elif exon.entry.start < cds.entry.start:
                 init_head_order = True
             if init_head_order:
                 # Find the first overlapping exon with CDS
                 while exon_idx < len(self.exons) and cds_idx < len(cds_list):
-                    # logger.log(f"init_head_order: exon_idx: {exon_idx}, cds_idx: {cds_idx}", debug=True)
                     exon_start, exon_end = self.exons[exon_idx].entry.start, self.exons[exon_idx].entry.end
                     cds_start, cds_end = cds_list[cds_idx].entry.start, cds_list[cds_idx].entry.end
-                    # print(exon_idx, cds_idx, exon_start, exon_end, cds_start, cds_end)
+                    _, ovp = lifton_utils.segments_overlap_length((exon_start, exon_end), (cds_start, cds_end))
                     # |eeeeee| |ccccc|
                     if exon_end < cds_start:
                         # Create a new exon using exon boundary
                         new_exon = copy.deepcopy(self.exons[exon_idx])
                         new_exon.update_exon_info(exon_start, exon_end)
                         new_exons.append(new_exon)
-                        # Move to the next exon
                         exon_idx += 1
                     # |eeee|--|cccc|
-                    elif lifton_utils.segments_overlap((exon_start, exon_end), (cds_start, cds_end)):
+                    elif ovp:
                         # Stop if exon and CDS overlap
                         # Create a new exon using exon boundary
                         new_exon = copy.deepcopy(self.exons[exon_idx])
                         new_exon.update_exon_info(min(exon_start, cds_start), cds_end)
                         new_exon.add_lifton_cds(cds_list[0])
                         new_exons.append(new_exon)
-                        # Move to the next exon
                         exon_idx += 1
-                        # Move to the next CDS
                         cds_idx += 1
                         break
                     # |cccc|  |eeee|
                     elif exon_start > cds_end: 
                         # Create a new exon using CDS boundary
                         new_exon = copy.deepcopy(self.exons[exon_idx])
                         new_exon.update_exon_info(cds_start, cds_end)
                         new_exon.add_lifton_cds(cds_list[0])
                         new_exons.append(new_exon)
-                        # Move to the next CDS
                         cds_idx += 1
                         break
             ################################################
             # Step 2: parse the inner exons and CDSs
             ################################################
             # Handle the CDSs in the middle
             # Leave the last CDS not processed.
-            # print(">> Step 3: parse the inner exons and CDSs")
             while cds_idx < len(cds_list)-1:
                 cds = cds_list[cds_idx]
-                # Step 1. Create a new exon
-                # Step 2. Add the CDS in the new exon
+                # Create a new exon
+                # Add the CDS in the new exon
                 new_exon = copy.deepcopy(exon)
                 new_exon.update_exon_info(cds.entry.start, cds.entry.end)
-                # print(">> New exon!!")
                 new_exon.add_lifton_cds(cds)
                 new_exons.append(new_exon)
                 cds_idx += 1
             ################################################
             # Step 3: parse the last CDS & its overlapping exon
             ################################################
             last_cds_processed = False
             cds = cds_list[cds_idx]
             cds_start, cds_end = cds_list[cds_idx].entry.start, cds_list[cds_idx].entry.end
             while exon_idx < len(self.exons):
                 exon = self.exons[exon_idx]
                 exon_start, exon_end = exon.entry.start, exon.entry.end
-                # print(f"cds_idx: {cds_idx}; {cds.entry.start}-{cds.entry.end} (len: {len(cds_list)});  exon_idx: {exon_idx}; {exon.entry.start}-{exon.entry.end} (len: {len(self.exons)})")
+                _, ovp = lifton_utils.segments_overlap_length((exon_start, exon_end), (cds_start, cds_end))
                 # |eeeeee| |ccccc|
                 if exon_end < cds_start:
                     # exon_idx = self.mv_exon_idx(exon_idx)
                     exon_idx += 1
                     continue
-                elif lifton_utils.segments_overlap((exon_start, exon_end), (cds_start, cds_end)):
-                    # print(">>>>>>>>>>> segments_overlap")
+                elif ovp:
                     # Create a new exon using exon boundary
                     last_cds_processed = True
                     new_exon = copy.deepcopy(exon)
                     new_exon.update_exon_info(cds_start, max(cds_end, exon_end))
                     new_exon.add_lifton_cds(cds)
                     new_exons.append(new_exon)
-                    # Move to the next exon
-                    # exon_idx = self.mv_exon_idx(exon_idx)
                     exon_idx += 1
                     break
                 # |cccc|  |eeee|
                 elif exon_start > cds_end: 
                     # Create a new exon using CDS boundary
                     last_cds_processed = True
                     new_exon = copy.deepcopy(exon)
                     new_exon.update_exon_info(cds_start, cds_end)
                     new_exon.add_lifton_cds(cds)
                     new_exons.append(new_exon)
                     break
             ################################################
             # Step 4: parse the remaining exons
             ################################################
-            # print(">> Step 3: parse the remaining exons")
             while exon_idx < len(self.exons):
                 exon = self.exons[exon_idx]
-                # Step 1. Create a new exon
-                # Step 2. Add the CDS in the new exon
+                # Create a new exon
+                # Add the CDS in the new exon
                 new_exon = copy.deepcopy(exon)
                 new_exon.update_exon_info(new_exon.entry.start, new_exon.entry.end)
                 new_exons.append(new_exon)
                 exon_idx += 1
             ################################################
             # Step 5: parse the last CDS if it does not overlap with any exon
             ################################################
             if not last_cds_processed:
-                # print(">> Step 4: parse the last CDS")
-                # Step 1. Create a new exon
-                # Step 2. Add the CDS in the new exon
+                # Create a new exon
+                # Add the CDS in the new exon
                 new_exon = copy.deepcopy(exon)
                 new_exon.update_exon_info(cds.entry.start, cds.entry.end)
                 new_exon.add_lifton_cds(cds)
                 new_exons.append(new_exon)
         self.exons = new_exons
         self.update_boundaries()
 
@@ -465,96 +451,87 @@
         cdss_lens = []
         cds_children = []
         for exon in self.exons:
             if exon.cds is not None:
                 cds_children.append(copy.deepcopy(exon.cds.entry))
                 # Chaining the CDS features
                 p_seq = exon.cds.entry.sequence(fai)
-                p_seq = Seq(p_seq).upper()
                 if exon.cds.entry.strand == '-':
                     coding_seq = p_seq + coding_seq
                     cdss_lens.insert(0, exon.cds.entry.end - exon.cds.entry.start + 1)
                 elif exon.cds.entry.strand == '+':
                     coding_seq = coding_seq + p_seq
                     cdss_lens.append(exon.cds.entry.end - exon.cds.entry.start + 1)
         return coding_seq, cds_children, cdss_lens
 
     def get_coding_trans_seq(self, fai):
         trans_seq = ""
-        exon_lens = []
         coding_seq = ""
-        cdss_lens = []
         accum_cds_length = 0
         for exon in self.exons:
             # Chaining the exon features
             p_trans_seq = exon.entry.sequence(fai)
             p_trans_seq = Seq(p_trans_seq).upper()
             if exon.entry.strand == '-':
                 trans_seq = p_trans_seq + trans_seq
-                exon_lens.insert(0, exon.entry.end - exon.entry.start + 1)
             elif exon.entry.strand == '+':
                 trans_seq = trans_seq + p_trans_seq
-                exon_lens.append(exon.entry.end - exon.entry.start + 1)
             if exon.cds is not None:
                 # Updating CDS frame
                 exon.cds.entry.frame = str(self.__get_cds_frame(accum_cds_length))
                 accum_cds_length = exon.cds.entry.end - exon.cds.entry.start + 1
                 # Chaining the CDS features
                 p_seq = exon.cds.entry.sequence(fai)
-                p_seq = Seq(p_seq).upper()
                 if exon.cds.entry.strand == '-':
                     coding_seq = p_seq + coding_seq
-                    cdss_lens.insert(0, exon.cds.entry.end - exon.cds.entry.start + 1)
                 elif exon.cds.entry.strand == '+':
                     coding_seq = coding_seq + p_seq
-                    cdss_lens.append(exon.cds.entry.end - exon.cds.entry.start + 1)
         if trans_seq != None:
-            trans_seq = Seq(trans_seq).upper()
+            trans_seq = str(trans_seq).upper()
         if coding_seq != None:
-            coding_seq = Seq(coding_seq).upper()
-        return coding_seq, cdss_lens, trans_seq, exon_lens
+            coding_seq = str(coding_seq).upper()
+        return coding_seq, trans_seq
 
     def translate_coding_seq(self, coding_seq):
         protein_seq = None
         if coding_seq != "":
-            protein_seq = coding_seq.translate()
-        # print("translate_coding_seq: ", protein_seq)
+            protein_seq = str(Seq(coding_seq).translate())
         return protein_seq
 
     def align_coding_seq(self, protein_seq, ref_protein_seq, lifton_status):
-        if protein_seq == None:
+        if ref_protein_seq == "" or ref_protein_seq == None:
+            lifton_aa_aln = None
+            peps = None
+        elif protein_seq == "" or protein_seq == None:
             lifton_aa_aln = None
             peps = None
         else:
             peps = protein_seq.split("*")
-            # print("protein_seq: ", protein_seq)
-            # print("ref_protein_seq: ", ref_protein_seq)
             lifton_aa_aln = align.protein_align(protein_seq, ref_protein_seq)
             # Update lifton sequence identity
             lifton_status.lifton_aa = max(lifton_status.lifton_aa, lifton_aa_aln.identity)
         return lifton_aa_aln, peps
 
     def align_trans_seq(self, trans_seq, ref_trans_seq, lifton_status):
-        if ref_trans_seq != None:
-            ref_trans_seq = str(ref_trans_seq).upper()
-        if trans_seq == "":
+        if ref_trans_seq == "" or ref_trans_seq == None:
+            lifton_tran_aln = None
+        elif trans_seq == "" or trans_seq == None:
             lifton_tran_aln = None
         else:
             lifton_tran_aln = align.trans_align(trans_seq, ref_trans_seq)
-        lifton_status.lifton_dna = lifton_tran_aln.identity
+            lifton_status.lifton_dna = lifton_tran_aln.identity
         return lifton_tran_aln
 
-    def fix_truncated_protein(self, fai, ref_protein_seq, ref_trans_seq, lifton_status):
-        # Step 1: Getting translated sequences (frame will be updated)
-        coding_seq, cdss_lens, trans_seq, exon_lens = self.get_coding_trans_seq(fai)
+    def orf_search_protein(self, fai, ref_protein_seq, ref_trans_seq, lifton_status, is_non_coding, eval_only=False):
+        coding_seq, trans_seq = self.get_coding_trans_seq(fai)
         protein_seq = self.translate_coding_seq(coding_seq)
         # Aligning the LiftOn protein & DNA sequences
         lifton_aa_aln, peps = self.align_coding_seq(protein_seq, ref_protein_seq, lifton_status)
         lifton_tran_aln = self.align_trans_seq(trans_seq, ref_trans_seq, lifton_status)
-        variants.find_variants(lifton_tran_aln, lifton_aa_aln, lifton_status, peps)
+        variants.find_variants(lifton_tran_aln, lifton_aa_aln, lifton_status, peps, is_non_coding)
         ORF_search = False
         for mutation in lifton_status.status:
             # identical # synonymous 
             # (1) inframe_insertion # (2) inframe_deletion # (3) nonsynonymous 
             # (4) frameshift # (5) start_lost # (6) stop_missing # (7) stop_codon_gain
             # Adding mutations in to entry.attributes
             if mutation != "identical":
@@ -563,24 +540,19 @@
                 else:
                     self.entry.attributes["mutation"].append(mutation)
             # ORF searching for these four types of mutations
             # frameshift_orf_threshold = 0.8
             # and lifton_aa_aln.identity < frameshift_orf_threshold)
             if mutation == "stop_missing" or mutation == "stop_codon_gain" or mutation == "frameshift"  or mutation == "start_lost":
                 ORF_search = True
-        if ORF_search:
-            self.__find_orfs(trans_seq, exon_lens, ref_protein_seq, lifton_aa_aln, lifton_status)
+        if ORF_search and eval_only==False:
+            self.__find_orfs(trans_seq, ref_protein_seq, lifton_aa_aln, lifton_status)
         return lifton_tran_aln, lifton_aa_aln
 
-    def align_trans_dna(self, fai, ref_trans_seq, lifton_status):
-        coding_seq, cdss_lens, trans_seq, exon_lens = self.get_coding_trans_seq(fai)
-        lifton_tran_aln = self.align_trans_seq(trans_seq, ref_trans_seq, lifton_status)
-        return lifton_tran_aln
-
-    def __find_orfs(self, trans_seq, exon_lens, ref_protein_seq, lifton_aln, lifton_status):
+    def __find_orfs(self, trans_seq, ref_protein_seq, lifton_aln, lifton_status):
         trans_seq = trans_seq.upper()
         # Find ORFs in whole transcript region (including UTRs)
         start_codon = "ATG"
         stop_codons = ["TAA", "TAG", "TGA"]
         orf_list = []
         max_orf_len = [0, 0, 0]
         for frame in range(3):
@@ -604,23 +576,18 @@
                             orf = lifton_class.Lifton_ORF(orf_idx_s, orf_idx_e)
                             orf_list.append(orf)
         final_orf = None
         update_orf = False
         max_identity = 0
         for i, orf in enumerate(orf_list):
             orf_DNA_seq = trans_seq[orf.start:orf.end]
-            orf_protein_seq = orf_DNA_seq.translate()
-            orf_parasail_res, orf_seq, reference_seq = align.parasail_align_protein_base(orf_protein_seq, str(ref_protein_seq))        
+            orf_protein_seq = str(Seq(orf_DNA_seq).translate())
+            orf_parasail_res = align.parasail_align_protein_base(orf_protein_seq, ref_protein_seq)
             orf_matches, orf_length = get_id_fraction.get_AA_id_fraction(orf_parasail_res.traceback.ref, orf_parasail_res.traceback.query)
             orf_identity = orf_matches/orf_length
-            # print(f"\tORF {i+1}: {orf.start}-{orf.end}")
-            # print(f"\tORF {i+1}: {orf_DNA_seq}")
-            # print(f"\torf_protein_seq: {orf_protein_seq}")
-            # print(f"\t\torf_identity: {orf_identity}")
-            # Select the largest among all orfs.
             if orf_identity > max_identity:
                 max_identity = orf_identity
                 final_orf = orf
         # Only update orf if at least one frame similarity is larger than the original lifton_aa by the threshold
         threshold_orf = 0.01
         if max_identity > (lifton_status.lifton_aa + threshold_orf):
             lifton_status.lifton_aa = max_identity
@@ -635,15 +602,14 @@
             self.__iterate_exons_update_cds(final_orf, self.exons[::-1], "-")            
 
     def __iterate_exons_update_cds(self, final_orf, exons, strand):
         accum_exon_length = 0
         accum_cds_length = 0
         for exon_idx, exon in enumerate(exons):
             curr_exon_len = exon.entry.end - exon.entry.start + 1
-            # print(f"\t>> {exon.entry.seqid} {exon.entry.strand}; exon_idx: {exon_idx}: {exon.entry.start}-{exon.entry.end} (len: {len(exons)});  accum_exon_length: {accum_exon_length}; curr_exon_len: {curr_exon_len}; final_orf.start: {final_orf.start}; final_orf.end: {final_orf.end}")
             if accum_exon_length <= final_orf.start:
                 if final_orf.start < accum_exon_length+curr_exon_len:
                     # Create first partial CDS
                     if exon.cds is not None:
                         if strand == "+":
                             exon.cds.entry.start = exon.entry.start + (final_orf.start - accum_exon_length)
                         elif strand == "-":
@@ -651,17 +617,14 @@
                     else:
                         if strand == "+":
                             exon.add_novel_lifton_cds(exon.entry, exon.entry.start + (final_orf.start - accum_exon_length), exon.entry.end)
                         elif strand == "-":
                             exon.add_novel_lifton_cds(exon.entry, exon.entry.start, exon.entry.end - (final_orf.start - accum_exon_length))
                     exon.cds.entry.frame = str(self.__get_cds_frame(accum_cds_length))
                     accum_cds_length += (exon.cds.entry.end - exon.cds.entry.start + 1)
-                    # print(f"\t\t >> {exon.entry.seqid} {exon.entry.strand}; exon_idx: {exon_idx}: {exon.entry.start}-{exon.entry.end} (len: {len(exons)});  accum_exon_length: {accum_exon_length}; curr_exon_len: {curr_exon_len}; final_orf.start: {final_orf.start}; final_orf.end: {final_orf.end}")
-                    # print(f"\t\t >> exon.cds.entry.start: {exon.cds.entry.start}; exon.cds.entry.end: {exon.cds.entry.end}")
-                    # print(f"\t\t>> exon.cds.entry.frame: {exon.cds.entry.frame}")
                 else:
                     # No CDS should be created
                     exon.cds = None
             elif final_orf.start < accum_exon_length and accum_exon_length < final_orf.end:
                 if final_orf.end <= accum_exon_length+curr_exon_len:
                     # Create the last partial CDS
                     if exon.cds is not None:
@@ -672,17 +635,14 @@
                     else:
                         if strand == "+":
                             exon.add_novel_lifton_cds(exon.entry, exon.entry.start, exon.entry.start + (final_orf.end - accum_exon_length)-1)
                         elif strand == "-":
                             exon.add_novel_lifton_cds(exon.entry, exon.entry.end - (final_orf.end - accum_exon_length)+1, exon.entry.end)
                     exon.cds.entry.frame = str(self.__get_cds_frame(accum_cds_length))
                     accum_cds_length += (exon.cds.entry.end - exon.cds.entry.start + 1)
-                    # print(f"\t\t >> {exon.entry.seqid} {exon.entry.strand}; exon_idx: {exon_idx}: {exon.entry.start}-{exon.entry.end} (len: {len(exons)});  accum_exon_length: {accum_exon_length}; curr_exon_len: {curr_exon_len}; final_orf.start: {final_orf.start}; final_orf.end: {final_orf.end}")
-                    # print(f"\t\t >> exon.cds.entry.start: {exon.cds.entry.start}; exon.cds.entry.end: {exon.cds.entry.end}")
-                    # print(f"\t\t >> exon.cds.entry.frame: {exon.cds.entry.frame}")
                 else:
                     # Keep the original full CDS / extend the CDS to full exon length
                     if exon.cds is None:
                         exon.add_novel_lifton_cds(exon.entry, exon.entry.start, exon.entry.end)
                     else:
                         exon.cds.update_CDS_info(exon.entry.start, exon.entry.end)
                     exon.cds.entry.frame = str(self.__get_cds_frame(accum_cds_length))
@@ -704,15 +664,14 @@
         for exon in self.exons:
             if exon.cds is not None:
                 exon.cds.write_entry(fw)
 
     def update_boundaries(self):
         self.entry.start = self.exons[0].entry.start
         self.entry.end = self.exons[-1].entry.end
-        # print(f"update_boundaries, exon length: {len(self.exons)};  {self.entry.start} - {self.entry.end}")
 
     def print_transcript(self):
         print(f"\t{self.entry}")
         for exon in self.exons:
             exon.print_exon()
 
 
@@ -725,15 +684,14 @@
         self.cds = None
 
     def update_exon_info(self, start, end):
         self.cds = None
         self.entry.source = "LiftOn"
         self.entry.start = start
         self.entry.end = end
-        # print(f"start: {self.entry.start} - end: {self.entry.end}")
 
     def add_cds(self, gffutil_entry_cds):
         Lifton_cds = Lifton_CDS(gffutil_entry_cds)
         self.cds = Lifton_cds
 
     def add_novel_lifton_cds(self, gffutil_entry_exon, start, end):
         gffutil_entry_cds = copy.deepcopy(gffutil_entry_exon)
```

### Comparing `lifton-0.0.2/lifton/lifton_utils.py` & `lifton-0.0.3/lifton/lifton_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -133,58 +133,14 @@
         print("\n**********************")
         print("** Running miniprot **")
         print("**********************")
         miniprot_annotation = run_miniprot.run_miniprot(outdir, args, tgt_genome, ref_proteins_file)
     return miniprot_annotation
 
 
-def get_child_types(parent_types, db):
-    """
-        This function gets the child types.
-
-        Parameters:
-        - parent_types: parent types
-        - db: database
-
-        Returns:
-        child_types: set of child types
-    """
-    child_types = set()
-    for parent in parent_types:
-        for feature in db.db_connection.features_of_type(featuretype=parent):
-            child_count = 0
-            for child in db.db_connection.children(feature):
-                child_count += 1
-                if db.is_lowest_child(child):
-                    child_types.add(child.featuretype)
-            if child_count == 0:
-                child_types.add(feature.featuretype)
-    return child_types
-
-
-def segments_overlap(segment1, segment2):
-    """
-        This function checks if the segments overlap.
-
-        Parameters:
-        - segment1: segment 1 in tuple (start, end)
-        - segment2: segment 2 in tuple (start, end)
-
-        Returns:
-        True if the segments overlap, False otherwise.
-    """
-    # Check if the segments have valid endpoints
-    if len(segment1) != 2 or len(segment2) != 2:
-        raise ValueError("Segments must have exactly 2 endpoints")    
-    # Sort the segments by their left endpoints
-    segment1, segment2 = sorted([segment1, segment2], key=lambda x: x[0])
-    # Check if the right endpoint of the first segment is greater than or equal to the left endpoint of the second segment
-    return segment1[1] >= segment2[0]
-
-
 def custom_bisect_insert(sorted_list, element_to_insert):
     """
         This function bisects the sorted list and inserts the element.
 
         Parameters:
         - sorted_list: sorted list
         - element_to_insert: element to insert
@@ -256,15 +212,29 @@
         feature_types = []
         f = open(feature_types_file)
         for line in f.readlines():
             feature_types.append(line.rstrip())
     return feature_types
 
 
-def LiftOn_check_miniprot_alignment(chromosome, transcript, lifton_status, m_id_dict, m_feature_db, tree_dict, fai, ref_proteins, ref_trans_id):
+def LiftOn_eval_alignment(eval_trans, locus, tgt_fai, ref_proteins, ref_trans_id, lifton_status):
+    eval_aln = align.lifton_parasail_align(eval_trans, locus, tgt_fai, ref_proteins, ref_trans_id)
+    if eval_aln != None:
+        lifton_status.lifton_aa = eval_aln.identity
+    return eval_aln
+
+
+def LiftOn_liftoff_alignment(lifton_trans, locus, tgt_fai, ref_proteins, ref_trans_id, lifton_status):
+    liftoff_aln = align.lifton_parasail_align(lifton_trans, locus, tgt_fai, ref_proteins, ref_trans_id)
+    if liftoff_aln != None:
+        lifton_status.liftoff = liftoff_aln.identity
+    return liftoff_aln
+
+
+def LiftOn_miniprot_alignment(chromosome, transcript, m_id_dict, m_feature_db, tree_dict, fai, ref_proteins, ref_trans_id, lifton_status):
     """
         This function checks the miniprot alignment.
 
         Parameters:
         - chromosome: chromosome
         - transcript: transcript gffutils feature
         - lifton_status: Lifton_Status instance
@@ -284,15 +254,15 @@
     if (ref_trans_id in m_id_dict.keys()) and (ref_trans_id in ref_proteins.keys()):
         m_ids = m_id_dict[ref_trans_id]
         for m_id in m_ids:
             ##################################################
             # Check 1: Check if the miniprot transcript is overlapping the current gene locus
             ##################################################
             m_entry = m_feature_db[m_id]
-            overlap = segments_overlap((m_entry.start, m_entry.end), (transcript.start, transcript.end))
+            _, overlap = segments_overlap_length((m_entry.start, m_entry.end), (transcript.start, transcript.end))
             if not overlap or m_entry.seqid != transcript.seqid:
                 # "Not overlapped"
                 continue
             ##################################################
             # Check 2: reference overlapping status
             #   1. Check it the transcript overlapping with the next gene
             # Check the miniprot protein overlapping status
@@ -320,61 +290,122 @@
             for exon in list(exons):
                 miniprot_trans.add_exon(exon)
             cdss = m_feature_db.children(m_entry, featuretype=('CDS', 'stop_codon'), order_by='start') 
             cds_num = 0
             for cds in list(cdss):
                 cds_num += 1
                 miniprot_trans.add_cds(cds)
-            tmp_m_lifton_aln = align.parasail_align("miniprot", miniprot_trans, m_entry, fai, ref_proteins, ref_trans_id, lifton_status)
+            tmp_m_lifton_aln = align.lifton_parasail_align(miniprot_trans, m_entry, fai, ref_proteins, ref_trans_id)
             if m_lifton_aln == None or tmp_m_lifton_aln.identity > lifton_status.miniprot:
                 m_lifton_aln = tmp_m_lifton_aln
                 lifton_status.miniprot = m_lifton_aln.identity
     return m_lifton_aln, has_valid_miniprot
 
 
-def get_ref_liffover_features(features, ref_db):
+def get_ref_liffover_features(features, ref_db, intermediate_dir, args):
     """
         This function gets the reference liftover features.
 
         Parameters:
         - features: list of features to liftover
         - ref_db: reference database
 
         Returns:
         ref_features_dict: reference features dictionary (gene id -> transcript id)
         ref_features_reverse_dict: reference features reverse dictionary (transcript id -> gene id)
     """
+
+    fw_gene = open(f"{intermediate_dir}/ref_feature.txt", "w")
+    fw_trans = open(f'{intermediate_dir}/ref_transcript.txt', 'w')    
     ref_features_dict = {}
+    ref_features_len_dict = {}
     ref_features_reverse_dict = {}
+    ref_trans_exon_num_dict = {}
     new_gene_feature = lifton_class.Lifton_feature("Lifton-gene")
     ref_features_dict["LiftOn-gene"] = new_gene_feature
     for f_itr in features:
         for locus in ref_db.db_connection.features_of_type(f_itr):
             CDS_children = list(ref_db.db_connection.children(locus, featuretype='CDS'))
             feature = lifton_class.Lifton_feature(locus.id)
-            if len(CDS_children) > 0:
-                # This is the protien-coding gene
+
+            # Write out reference gene features IDs
+            # Decide if its type
+            gene_type_key = ""
+            if args.annotation_database.upper() == "REFSEQ":
+                gene_type_key = "gene_biotype"
+            elif args.annotation_database.upper() == "GENCODE" or args.annotation_database.upper() == "ENSEMBL" or args.annotation_database.upper() == "CHESS":
+                gene_type_key = "gene_type"
+            if locus.attributes[gene_type_key][0] == "protein_coding" and len(CDS_children) > 0:
                 feature.is_protein_coding = True
+                fw_gene.write(f"{locus.id}\tcoding\n")
+            elif (locus.attributes[gene_type_key][0] == "lncRNA" or locus.attributes[gene_type_key][0] == "ncRNA"):
+                feature.is_non_coding = True
+                fw_gene.write(f"{locus.id}\tnon-coding\n")
+            else:
+                fw_gene.write(f"{locus.id}\tother\n")
             exon_children = list(ref_db.db_connection.children(locus, featuretype='exon', level=1, order_by='start'))
             if len(exon_children) > 0:
                 __process_ref_liffover_features(locus, ref_db, None)
             else:
                 transcripts = ref_db.db_connection.children(locus, level=1)
                 for transcript in list(transcripts):
                     __process_ref_liffover_features(transcript, ref_db, feature)
                     ref_features_reverse_dict[transcript.id] = locus.id
+                    all_CDS_in_trans = list(ref_db.db_connection.children(transcript, featuretype='CDS', order_by='start'))
+                    if len(all_CDS_in_trans) > 0:
+                        ref_trans_exon_num_dict[transcript.id] = len(all_CDS_in_trans)
+                    else:
+                        ref_trans_exon_num_dict[transcript.id] = 0
+                    # Write out reference trans feature IDs
+                    if feature.is_protein_coding and transcript.featuretype == "mRNA":
+                        fw_trans.write(f"{transcript.id}\tcoding\n")
+                    elif feature.is_non_coding and (transcript.featuretype == "ncRNA" or transcript.featuretype == "nc_RNA" or transcript.featuretype == "lncRNA" or transcript.featuretype == "lnc_RNA"):
+                        fw_trans.write(f"{transcript.id}\tnon-coding\n")
+                    else:
+                        fw_trans.write(f"{transcript.id}\tother\n")
             ref_features_dict[locus.id] = feature
-    return ref_features_dict, ref_features_reverse_dict
+            all_CDS_children = list(ref_db.db_connection.children(locus, featuretype='CDS', order_by='start'))
+            if len(all_CDS_children) > 0:
+                ref_features_len_dict[locus.id] = all_CDS_children[-1].end - all_CDS_children[0].start + 1
+            else:
+                ref_features_len_dict[locus.id] = 0
+    fw_gene.close()
+    fw_trans.close()
+    return ref_features_dict, ref_features_len_dict, ref_features_reverse_dict, ref_trans_exon_num_dict
 
 
 def __process_ref_liffover_features(locus, ref_db, feature):
     if feature != None:
         feature.children.add(locus.id)
 
 
+def miniprot_id_mapping(m_feature_db):
+    """
+        This function creates a dictionary of miniprot id to reference id.
+
+        Parameters:
+        - m_feature_db: miniprot feature database
+
+        Returns:
+        ref_id_2_m_id_trans_dict: reference id to miniprot transcript ids dictionary
+        m_id_2_ref_id_trans_dict: miniprot transcript id to reference id dictionary
+    """
+    ref_id_2_m_id_trans_dict = {}
+    m_id_2_ref_id_trans_dict = {}
+    for feature in m_feature_db.features_of_type("mRNA"):
+        miniprot_id = feature["ID"][0]
+        aa_trans_id = str(feature.attributes["Target"][0]).split(" ")[0]
+        if aa_trans_id in ref_id_2_m_id_trans_dict.keys():
+            ref_id_2_m_id_trans_dict[aa_trans_id].append(miniprot_id)
+        else:
+            ref_id_2_m_id_trans_dict[aa_trans_id] = [miniprot_id]
+        m_id_2_ref_id_trans_dict[miniprot_id] = aa_trans_id
+    return ref_id_2_m_id_trans_dict, m_id_2_ref_id_trans_dict
+
+
 def get_ref_ids_liftoff(ref_features_dict, liftoff_gene_id, liftoff_trans_id):
     """
         This function gets the reference IDs from Liftoff IDs.
 
         Parameters:
         - ref_features_dict: reference features dictionary
         - liftoff_gene_id: Liftoff gene ID
@@ -453,16 +484,18 @@
         Returns:
         The length of the overlapping segments.
     """
     if len(segment1) != 2 or len(segment2) != 2:
         raise ValueError("Segments must have exactly 2 endpoints")
     # Sort the segments by their left endpoints
     segment1, segment2 = sorted([segment1, segment2], key=lambda x: x[0])
-    # print("Checking miniprot overlapped length: ", segment1[1] - segment2[0] + 1)
-    return segment1[1] - segment2[0] + 1
+    ovp_len = segment1[1] - segment2[0] + 1
+    ovp = False
+    if ovp_len > 0: ovp = True
+    return ovp_len, ovp
 
 
 def check_ovps_ratio(mtrans, mtrans_interval, overlap_ratio, tree_dict):
     """
         This function checks the overlap ratio.
 
         Parameters:
@@ -472,19 +505,18 @@
         - tree_dict: tree dictionary
 
         Returns:
         True if the overlap ratio is greater than the threshold, False otherwise.
     """
     is_overlapped = False
     if mtrans.seqid not in tree_dict.keys():
-        return is_overlapped
+        return False
     ovps = tree_dict[mtrans.seqid].overlap(mtrans_interval)
     for ovp in ovps:
-        ovp_len = segments_overlap_length((mtrans_interval[0], mtrans_interval[1]), (ovp[0], ovp[1]))
+        ovp_len, _ = segments_overlap_length((mtrans_interval[0], mtrans_interval[1]), (ovp[0], ovp[1]))
         ref_len = ovp[1] - ovp[0] + 1
+        target_len = mtrans_interval[1] - mtrans_interval[0] + 1
         # Overlapping does not extend the ratio of the reference
-        if (ovp_len / ref_len) > overlap_ratio:
+        if (ovp_len / min(ref_len, target_len)) > overlap_ratio:
             is_overlapped = True
             break
-    return is_overlapped
-
-
+    return is_overlapped
```

### Comparing `lifton-0.0.2/lifton/run_liftoff.py` & `lifton-0.0.3/lifton/run_liftoff.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import subprocess
 import os, copy
-from lifton import lifton_class, logger, fix_trans_annotation, lifton_utils, run_miniprot, align
+from lifton import lifton_class, logger, lifton_utils, protein_maximization, run_miniprot, align
 from lifton.liftoff import liftoff_main
 from lifton.liftoff.tests import test_basic, test_advanced
 from intervaltree import Interval, IntervalTree
 
 def run_liftoff(output_dir, args):
     """
         This function runs liftoff.
@@ -18,20 +18,113 @@
     """
     liftoff_args = copy.deepcopy(args)
     liftoff_outdir = output_dir + "liftoff/"    
     os.makedirs(liftoff_outdir, exist_ok=True)
     liftoff_annotation = liftoff_outdir + "liftoff.gff3"
     liftoff_args.output = liftoff_annotation
     liftoff_main.run_all_liftoff_steps(liftoff_args)
+    if args.polish:
+        liftoff_annotation += "_polished"
     # test_basic.test_yeast(liftoff_outdir + "test_basic/")
     # test_advanced.test_yeast(liftoff_outdir + "test_advance/")
     return liftoff_annotation
 
 
-def process_liftoff(lifton_gene, locus, ref_db, l_feature_db, ref_id_2_m_id_trans_dict, m_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, fw_chain, write_chains, DEBUG):
+def initialize_lifton_gene(locus, ref_db, tree_dict, ref_features_dict, args, with_exons=False):
+    """
+        This function initializes Lifton gene instance.
+
+        Parameters:
+        - locus: gffutils feature instance
+        - ref_db: reference database
+        - tree_dict: intervaltree dictionary for each chromosome
+        - ref_features_dict: reference features dictionary
+        - with_exons: True if the gene has exons, False otherwise
+
+        Returns:
+        lifton_gene: Lifton gene instance
+        ref_gene_id: reference gene
+        ref_trans_id: reference transcript
+    """
+    ref_gene_id, ref_trans_id = lifton_utils.get_ref_ids_liftoff(ref_features_dict, locus.id, None)
+    lifton_gene = lifton_class.Lifton_GENE(ref_gene_id, copy.deepcopy(locus), copy.deepcopy(ref_db[ref_gene_id].attributes), tree_dict, ref_features_dict, args, tmp=with_exons)
+    return lifton_gene, ref_gene_id, ref_trans_id
+
+
+def lifton_add_trans_exon_cds(lifton_gene, locus, ref_db, l_feature_db, ref_trans_id):
+    """
+        This function adds transcript, exons, and CDSs to the Lifton gene instance.
+
+        Parameters:
+        - lifton_gene: Lifton gene instance
+        - locus: gffutils feature instance
+        - ref_db: reference database
+        - l_feature_db: liftoff feature database
+        - ref_trans_id: reference transcript ID
+
+        Returns:
+        lifton_trans: Lifton transcript instance
+        len(cdss_list): number of CDSs
+    """
+    lifton_trans = lifton_gene.add_transcript(ref_trans_id, copy.deepcopy(locus), copy.deepcopy(ref_db[ref_trans_id].attributes))
+    exons = l_feature_db.children(locus, featuretype='exon', order_by='start')
+    for exon in list(exons):
+        lifton_gene.add_exon(lifton_trans.entry.id, exon)
+    cdss = l_feature_db.children(locus, featuretype=('CDS', 'stop_codon'), order_by='start') 
+    cdss_list = list(cdss)
+    for cds in cdss_list:
+        lifton_gene.add_cds(lifton_trans.entry.id, cds)
+    return lifton_trans, len(cdss_list)
+
+
+def process_liftoff_with_protein(locus, lifton_gene, lifton_trans,
+                                 ref_id_2_m_id_trans_dict, m_feature_db, tree_dict,
+                                 tgt_fai, ref_trans_id, ref_proteins, ref_trans,
+                                 fw_chain, write_chains, lifton_status, DEBUG):
+    """
+        This function process liftoff annotation with protein.
+        (1) Only Liftoff annotation: directly apply 
+        (2) Liftoff annotation with miniprot annotation: Protein-maximization algorithm
+
+        Parameters:
+        - locus: gffutils feature instance
+        - lifton_gene: Lifton gene instance
+        - lifton_trans: Lifton transcript instance
+        - ref_id_2_m_id_trans_dict: reference id to miniprot transcript ids dictionary
+        - m_feature_db: miniprot feature database
+        - tree_dict: intervaltree dictionary for each chromosome
+        - tgt_fai: target fasta index
+        - ref_trans_id: reference transcript ID
+        - ref_proteins: reference proteins dictionary
+        - ref_trans: reference transcript dictionary
+        - fw_chain: file writer for chains
+        - write_chains: write chains or not
+        - lifton_status: Lifton_Status instance
+        - DEBUG: debug mode
+    """
+    # Liftoff alignment
+    liftoff_aln = lifton_utils.LiftOn_liftoff_alignment(lifton_trans, locus, tgt_fai, ref_proteins, ref_trans_id, lifton_status)
+    # miniprot alignment
+    miniprot_aln, has_valid_miniprot = lifton_utils.LiftOn_miniprot_alignment(locus.seqid, locus, ref_id_2_m_id_trans_dict, m_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans_id, lifton_status)
+    if liftoff_aln is None:
+        lifton_status.annotation = "no_ref_protein"
+    elif liftoff_aln.identity == 1:
+        # Liftoff protein annotation is perfect"
+        lifton_status.lifton_aa = 1
+    elif liftoff_aln.identity < 1:
+        # Liftoff protein annotation is not perfect
+        if has_valid_miniprot:
+            lifton_status.annotation = "LiftOn_chaining_algorithm"
+            cds_list, chains = protein_maximization.chaining_algorithm(liftoff_aln, miniprot_aln, tgt_fai, DEBUG)
+            if write_chains:
+                lifton_utils.write_lifton_chains(fw_chain, lifton_trans.entry.id, chains)
+            lifton_gene.update_cds_list(lifton_trans.entry.id, cds_list)
+
+
+def process_liftoff(lifton_gene, locus, ref_db, l_feature_db, ref_id_2_m_id_trans_dict, m_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, fw_chain, args, ENTRY_FEATURE=False):
     """
         This function processes liftoff annotation.
 
         Parameters:
         - lifton_gene: Lifton gene instance
         - locus: feature instance 
         - ref_db: reference database
@@ -43,117 +136,45 @@
         - ref_proteins: reference protein dictionary
         - ref_trans: reference transcript dictionary
         - ref_features_dict: reference features dictionary
         - fw_score: file writer for scores
         - fw_chain: file writer for chains
         - write_chains: write chains or not
         - DEBUG: debug mode
+        - ENTRY_FEATURE: True if the feature is the root feature for a gene locus
 
         Returns:
-        lifton_gene: Lifton gene instance
+        lifton_gene: LiftOn gene instance
     """
     exon_children = list(l_feature_db.children(locus, featuretype='exon', level=1, order_by='start'))
+    if lifton_gene is None and ENTRY_FEATURE:   
+        # Gene (1st) features
+        lifton_gene, ref_gene_id, ref_trans_id = initialize_lifton_gene(locus, ref_db, tree_dict, ref_features_dict, args, with_exons=len(exon_children)>0)
+        if lifton_gene.ref_gene_id is None: return None            
     if len(exon_children) == 0:
-        if lifton_gene is None:    
-            # Gene (1st) features without direct exons 
-            #   => Create LifOn gene instance
-            ref_gene_id, ref_trans_id = lifton_utils.get_ref_ids_liftoff(ref_features_dict, locus.id, None)
-            lifton_gene = lifton_class.Lifton_GENE(ref_gene_id, copy.deepcopy(locus), copy.deepcopy(ref_db[ref_gene_id].attributes), tree_dict, ref_features_dict)
-            logger.log(f"Gene level ref_gene_id\t: {ref_gene_id}; ref_trans_id\t:{ref_trans_id};  lifton_gene.copy_number\t:{lifton_gene.copy_num}", debug=DEBUG)
-            transcripts = l_feature_db.children(locus, level=1)
-            for transcript in list(transcripts):
-                process_liftoff(lifton_gene, transcript, ref_db, l_feature_db, ref_id_2_m_id_trans_dict, m_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, fw_chain, write_chains, DEBUG)
-        else:
-            # Middle features without exons
-            #   => lifton_gene is not None & there are no exon children
-            lifton_feature = lifton_gene.add_feature(copy.deepcopy(locus))                
-            logger.log(f"\tother feature middle level lifton_feature\t: {lifton_feature.entry.id};", debug=DEBUG)
-            features = l_feature_db.children(locus, level=1)
-            for feature in list(features):
-                process_liftoff(lifton_feature, feature, ref_db, l_feature_db, ref_id_2_m_id_trans_dict, m_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, fw_chain, write_chains, DEBUG)
+        parent_feature = None
+        if ENTRY_FEATURE: # Gene (1st) features without direct exons 
+            parent_feature = lifton_gene
+        else: # Middle features without exons
+            parent_feature = lifton_gene.add_feature(copy.deepcopy(locus))
+        features = l_feature_db.children(locus, level=1)
+        for feature in list(features):
+            lifton_gene = process_liftoff(parent_feature, feature, ref_db, l_feature_db, ref_id_2_m_id_trans_dict, m_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, fw_chain, args)
     else:
-        if lifton_gene is None:
-            # Gene (1st) features with direct exons 
-            #   => lifton_gene is None & there are direct exon children 
-            ref_gene_id, ref_trans_id = lifton_utils.get_ref_ids_liftoff(ref_features_dict, locus.id, None)
+        if ENTRY_FEATURE: # Gene (1st) features with direct exons 
             ref_trans_id = ref_gene_id
-            lifton_gene = lifton_class.Lifton_GENE(ref_gene_id, copy.deepcopy(locus), copy.deepcopy(ref_db[ref_gene_id].attributes), tree_dict, ref_features_dict, tmp = True)
-        else:
-            # Transcript features with direct exons 
-            #   => lifton_gene is not None & there are direct exon children 
-            #   => (transcript level)
+        else: # Transcript features with direct exons 
             ref_gene_id, ref_trans_id = lifton_utils.get_ref_ids_liftoff(ref_features_dict, lifton_gene.entry.id, locus.id)
-        logger.log(f"\tTranscript level ref_gene_id\t: {ref_gene_id}; ref_trans_id\t:{ref_trans_id}", debug=DEBUG)
-        # Processing transcript (feature with exon features)
-        lifton_status = lifton_class.Lifton_Status()                
-        # Add LifOn transcript instance
-        lifton_trans = lifton_gene.add_transcript(ref_trans_id, copy.deepcopy(locus), copy.deepcopy(ref_db[ref_trans_id].attributes))
-        exons = l_feature_db.children(locus, featuretype='exon', order_by='start')
-        for exon in list(exons):
-            lifton_gene.add_exon(lifton_trans.entry.id, exon)
-        cdss = l_feature_db.children(locus, featuretype=('CDS', 'stop_codon'), order_by='start') 
-        cds_num = 0
-        for cds in list(cdss):
-            cds_num += 1
-            lifton_gene.add_cds(lifton_trans.entry.id, cds)
-        # miniprot alignment
-        miniprot_aln, has_valid_miniprot = lifton_utils.LiftOn_check_miniprot_alignment(locus.seqid, locus, lifton_status, ref_id_2_m_id_trans_dict, m_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans_id)
-        if (cds_num > 0):
-            # Liftoff alignment                  
-            liftoff_aln = align.parasail_align("liftoff", lifton_trans, locus, tgt_fai, ref_proteins, ref_trans_id, lifton_status)
-            if liftoff_aln is None:
-                # There is no reference protein -> just keep Liftoff annotation
-                logger.log("\t* Has CDS but no ref protein", debug=DEBUG)
-                lifton_status.annotation = "Liftoff_no_ref_protein"
-                lifton_status.status = ["no_ref_protein"]
-            elif liftoff_aln.identity == 1:
-                # Liftoff protein annotation is perfect
-                logger.log("\t* Liftoff protein identical", debug=DEBUG)
-                lifton_status.lifton_aa = 1
-                # DNA level alignment
-                lifton_trans_aln = lifton_gene.align_trans_dna(lifton_trans.entry.id, ref_trans_id, tgt_fai, ref_trans, lifton_status)
-            elif liftoff_aln.identity < 1:
-                # Liftoff protein annotation is not perfect
-                if has_valid_miniprot:
-                    logger.log("\t* Has CDS and valid miniprot", debug=DEBUG)
-                    lifton_status.annotation = "LiftOn_chaining_algorithm" 
-                    cds_list, chains = fix_trans_annotation.chaining_algorithm(liftoff_aln, miniprot_aln, tgt_fai, DEBUG)
-                    if write_chains:
-                        lifton_utils.write_lifton_chains(fw_chain, lifton_trans.entry.id, chains)
-                    lifton_gene.update_cds_list(lifton_trans.entry.id, cds_list)
-                else:
-                    logger.log("\t* Has cds & protein but invalid miniprot annotation!", debug=DEBUG)
-                    lifton_status.annotation = "Liftoff_truncated"                    
-                # Check if there are mutations in the transcript
-                lifton_trans_aln, lifton_aa_aln = lifton_gene.fix_truncated_protein(lifton_trans.entry.id, ref_trans_id, tgt_fai, ref_proteins, ref_trans, lifton_status)
-        else:
-            # Liftoff has no protein
-            if has_valid_miniprot:
-                # LiftOn does not have proteins & miniprot has proteins
-                logger.log("\t* No CDS; miniprot has ref protein", debug=DEBUG)
-                # logger.log(f"ref_trans_id: {ref_trans_id}; \t ref_id_2_m_id_trans_dict[ref_trans_id]: {ref_id_2_m_id_trans_dict[ref_trans_id]}", debug=DEBUG)
-                if ref_trans_id in ref_id_2_m_id_trans_dict.keys():
-                    for mtrans_id in ref_id_2_m_id_trans_dict[ref_trans_id]:
-                        mtrans = m_feature_db[mtrans_id]
-                        mtrans_interval = Interval(mtrans.start, mtrans.end, mtrans_id)
-                        is_overlapped = lifton_utils.check_ovps_ratio(mtrans, mtrans_interval, 0.7, tree_dict)
-                        if is_overlapped:
-                            lifton_gene, transcript_id, lifton_status = run_miniprot.lifton_miniprot_with_ref_protein(mtrans, m_feature_db, ref_db, ref_gene_id, ref_trans_id, tgt_fai, ref_proteins, ref_trans, tree_dict, ref_features_dict, DEBUG)
-                            lifton_trans = lifton_gene.transcripts[transcript_id]
-                        else:
-                            lifton_status.annotation = "Liftoff_no_protein"
-                            lifton_status.status = ["no_protein"]
-            else:
-                # LiftOn does not have proteins & miniprot does not have proteins
-                if (ref_trans_id in ref_proteins.keys()) :
-                    logger.log("\t* No CDS & no miniprot but have ref protein", debug=DEBUG)
-                    lifton_status.annotation = "Liftoff_no_ref_protein"
-                    lifton_status.status = ["no_ref_protein"]
-                else:
-                    logger.log("\t* No CDS & no miniprot & no ref protein", debug=DEBUG)
-                    lifton_status.annotation = "Liftoff_nc_transcript"
-                    lifton_status.status = ["nc_transcript"]
-        lifton_utils.print_lifton_status(lifton_trans.entry.id, locus, lifton_status, DEBUG=DEBUG)
-        lifton_gene.add_lifton_status_attrs(lifton_trans.entry.id, lifton_status)
-        # Writing out LiftOn entries & scores
+        lifton_status = lifton_class.Lifton_Status()
+        lifton_status.annotation = "Liftoff"
+        lifton_trans, cds_num = lifton_add_trans_exon_cds(lifton_gene, locus, ref_db, l_feature_db, ref_trans_id)
+        if cds_num > 0:
+            process_liftoff_with_protein(locus, lifton_gene, lifton_trans,
+                                        ref_id_2_m_id_trans_dict, m_feature_db, tree_dict,
+                                        tgt_fai, ref_trans_id, ref_proteins, ref_trans,
+                                        fw_chain, args.write_chains, lifton_status, args.debug)
+        lifton_trans_aln, lifton_aa_aln = lifton_gene.orf_search_protein(lifton_trans.entry.id, ref_trans_id, tgt_fai, ref_proteins, ref_trans, lifton_status)
+        lifton_utils.print_lifton_status(lifton_trans.entry.id, locus, lifton_status, DEBUG=args.debug)
+        lifton_gene.add_lifton_gene_status_attrs("Liftoff")
+        lifton_gene.add_lifton_trans_status_attrs(lifton_trans.entry.id, lifton_status)
         lifton_utils.write_lifton_status(fw_score, lifton_trans.entry.id, locus, lifton_status)
     return lifton_gene
```

### Comparing `lifton-0.0.2/lifton/run_miniprot.py` & `lifton-0.0.3/lifton/run_miniprot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from lifton import logger, lifton_class, align
+from lifton import logger, lifton_class, align, lifton_utils
 import subprocess, os, sys, copy
+from intervaltree import Interval, IntervalTree
+
 
 def check_miniprot_installed():
     """
         This function checks if miniprot is installed.
 
         Parameters:
         None
@@ -47,97 +49,87 @@
     except: 
         print("failed to run miniprot")
         sys.exit(1)
     return miniprot_output
 
 
 def lifton_miniprot_with_ref_protein(m_feature, m_feature_db, ref_db, ref_gene_id, ref_trans_id, tgt_fai, 
-ref_proteins, ref_trans, tree_dict, ref_features_dict, DEBUG):
+ref_proteins, ref_trans, tree_dict, ref_features_dict, args):
     """
         This function create a miniprot gene entry with reference protein.
 
         Parameters:
         - m_feature: miniprot feature
         - m_feature_db: miniprot feature database
         - ref_db: reference database
         - ref_gene_id: reference gene ID
         - ref_trans_id: reference transcript ID
         - tgt_fai: target fasta index
         - ref_proteins: reference protein dictionary
         - ref_trans: reference transcript dictionary
         - tree_dict: tree dictionary
         - ref_features_dict: reference features dictionary
-        - DEBUG: debug mode
+        - args: LiftOn arguments
 
         Returns:
         lifton_gene: LiftOn gene instance
         lifton_transcript_id: LiftOn transcript ID
         lifton_status: LiftOn status
     """
-    logger.log("\tminiprot with reference protein", debug=DEBUG)
     mtrans_id = m_feature.attributes["ID"][0]
     # Create LifOn gene instance
-    if ref_gene_id is None:
-        # This is a place holder gene
-        lifton_gene = lifton_class.Lifton_GENE(ref_gene_id, copy.deepcopy(m_feature), {}, tree_dict, ref_features_dict, miniprot_holder=True)
-    else:
-        lifton_gene = lifton_class.Lifton_GENE(ref_gene_id, copy.deepcopy(m_feature), copy.deepcopy(ref_db[ref_gene_id].attributes), tree_dict, ref_features_dict)
+    m_gene_feature = copy.deepcopy(m_feature)
+    m_gene_feature.featuretype = "gene"
+    lifton_gene = lifton_class.Lifton_GENE(ref_gene_id, m_gene_feature, copy.deepcopy(ref_db[ref_gene_id].attributes), tree_dict, ref_features_dict, args)
     lifton_gene.update_gene_info(m_feature.seqid, m_feature.start, m_feature.end)
     # Create LifOn transcript instance
     Lifton_trans = lifton_gene.add_miniprot_transcript(ref_trans_id, copy.deepcopy(m_feature), ref_db[ref_trans_id].attributes, ref_features_dict)
     lifton_gene.update_trans_info(Lifton_trans.entry.id, m_feature.seqid, m_feature.start, m_feature.end)
     # Create exon / CDS entries
     cdss = m_feature_db.children(m_feature, featuretype='CDS')  # Replace 'exon' with the desired child feature type
     for cds in list(cdss):
         lifton_gene.add_exon(Lifton_trans.entry.id, cds)
         cds_copy = copy.deepcopy(cds)
         lifton_gene.add_cds(Lifton_trans.entry.id, cds_copy)
     # Update LiftOn status
     lifton_status = lifton_class.Lifton_Status()                
     m_entry = m_feature_db[mtrans_id]
-    m_lifton_aln = align.parasail_align("miniprot", Lifton_trans, m_entry, tgt_fai, ref_proteins, ref_trans_id, lifton_status)
+    m_lifton_aln = align.lifton_parasail_align(Lifton_trans, m_entry, tgt_fai, ref_proteins, ref_trans_id)
+    lifton_status.annotation =  "miniprot"
     lifton_status.lifton_aa = m_lifton_aln.identity
-    if m_lifton_aln.identity == 1:
-        lifton_status.annotation =  "miniprot_identical"
-    elif m_lifton_aln.identity < 1:
-        lifton_status.annotation =  "miniprot_truncated"
-    lifton_trans_aln, lifton_aa_aln = lifton_gene.fix_truncated_protein(Lifton_trans.entry.id, ref_trans_id, tgt_fai, ref_proteins, ref_trans, lifton_status)
-    return lifton_gene, Lifton_trans.entry.id, lifton_status
-
-
-def lifton_miniprot_no_ref_protein(m_feature, m_feature_db, ref_gene_id, ref_trans_id, ref_features_dict, tree_dict, DEBUG):
-    """
-        This function creates a miniprot gene entry with no reference protein.
+    # lifton_trans_aln, lifton_aa_aln = lifton_gene.orf_search_protein(Lifton_trans.entry.id, ref_trans_id, tgt_fai, ref_proteins, ref_trans, lifton_status)
+    return lifton_gene, Lifton_trans, Lifton_trans.entry.id, lifton_status
 
-        Parameters:
-        - m_feature: miniprot feature
-        - m_feature_db: miniprot feature database
-        - ref_gene_id: reference gene ID
-        - ref_trans _id: reference transcript ID
-        - ref_features_dict: reference features dictionary
-        - tree_dict: tree dictionary
-        - DEBUG: debug mode
 
-        Returns:
-        lifton_gene: LiftOn gene instance
-        lifton_transcript_id: LiftOn transcript ID
-        lifton_status: LiftOn status
-    """ 
-    logger.log("\tminiprot with NO reference protein", debug=DEBUG)
-    # Reason it's missing => the mRNA does not belong to gene (vdj segments) || the mRNA is not in the reference annotation
-    # Create LiftOn gene entry
-    lifton_gene = lifton_class.Lifton_GENE(ref_gene_id, copy.deepcopy(m_feature), {}, tree_dict, ref_features_dict)
-    lifton_gene.update_gene_info(m_feature.seqid, m_feature.start, m_feature.end)
-    # Create LiftOn transcript entry
-    Lifton_trans = lifton_gene.add_miniprot_transcript(ref_trans_id, copy.deepcopy(m_feature), {}, ref_features_dict)
-    lifton_gene.update_trans_info(Lifton_trans.entry.id, m_feature.seqid, m_feature.start, m_feature.end)
-    # Create the exon / CDS entry
-    cdss = m_feature_db.children(m_feature, featuretype='CDS')  # Replace 'exon' with the desired child feature type
-    for cds in list(cdss):
-        lifton_gene.add_exon(Lifton_trans.entry.id, cds)
-        cds_copy = copy.deepcopy(cds)
-        lifton_gene.add_cds(Lifton_trans.entry.id, cds_copy)
-    # Update LiftOn status
-    lifton_status = lifton_class.Lifton_Status()                
-    lifton_status.annotation = "miniprot_no_ref_protein"
-    lifton_status.status = ["no_ref_protein"]
-    return lifton_gene, Lifton_trans.entry.id, lifton_status
+def process_miniprot(mtrans, ref_db, m_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, m_id_2_ref_id_trans_dict, ref_features_len_dict, ref_trans_exon_num_dict, ref_features_reverse_dict, args):
+    mtrans_id = mtrans.attributes["ID"][0]
+    mtrans_interval = Interval(mtrans.start, mtrans.end, mtrans_id)
+    is_overlapped = lifton_utils.check_ovps_ratio(mtrans, mtrans_interval, args.overlap, tree_dict)
+    print(f"mtrans_id: {mtrans_id}, is_overlapped: {is_overlapped}")
+    lifton_gene = None
+    lifton_trans = None
+    if not is_overlapped:
+        ref_trans_id = m_id_2_ref_id_trans_dict[mtrans_id]            
+        ref_gene_id, ref_trans_id = lifton_utils.get_ref_ids_miniprot(ref_features_reverse_dict, mtrans_id, m_id_2_ref_id_trans_dict)
+        if ref_gene_id is None:
+            return None
+        if ref_trans_id in ref_proteins.keys() and ref_trans_id in ref_trans.keys():
+            if ref_trans_id != None:
+                # Check if the additional copy is valid
+                # 1. Remove processed pseudogenes: 1 CDS in miniprot but >1 CDS in reference
+                # 2. Check the trans ratio is in the range of min_minprot and max_minprot
+                if len(list(m_feature_db.children(mtrans, featuretype='CDS'))) == 1 and ref_trans_exon_num_dict[ref_trans_id] > 1: # Processed pseudogene
+                    return None
+                miniprot_trans_ratio = (mtrans.end - mtrans.start + 1) / ref_features_len_dict[ref_gene_id]
+                if miniprot_trans_ratio > args.min_miniprot and miniprot_trans_ratio < args.max_miniprot:
+                    lifton_gene, lifton_trans, transcript_id, lifton_status = lifton_miniprot_with_ref_protein(mtrans, m_feature_db, ref_db.db_connection, ref_gene_id, ref_trans_id, tgt_fai, ref_proteins, ref_trans, tree_dict, ref_features_dict, args)
+                    lifton_gene.transcripts[transcript_id].entry.attributes["miniprot_annotation_ratio"] = [f"{miniprot_trans_ratio:.3f}"]
+                else: # Invalid miniprot transcript
+                    return None
+            else: # Skip those cannot be found in reference.
+                return None
+        lifton_trans_aln, lifton_aa_aln = lifton_gene.orf_search_protein(lifton_trans.entry.id, ref_trans_id, tgt_fai, ref_proteins, ref_trans, lifton_status)
+        lifton_utils.print_lifton_status(transcript_id, mtrans, lifton_status, DEBUG=args.debug)
+        lifton_gene.add_lifton_gene_status_attrs("miniprot")
+        lifton_gene.add_lifton_trans_status_attrs(transcript_id, lifton_status)
+        lifton_utils.write_lifton_status(fw_score, transcript_id, mtrans, lifton_status)
+    return lifton_gene
```

### Comparing `lifton-0.0.2/lifton/stats.py` & `lifton-0.0.3/lifton/stats.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,94 @@
 import sys
 from lifton import logger
 
-def print_report(ref_features_dict, fw_unmapped, fw_extra_copy, debug=False):
+def print_report(ref_features_dict, transcripts_stats_dict, fw_unmapped, fw_extra_copy, fw_mapped_feature, fw_mapped_trans, debug=False):
     """
-        This function prints the report of the lifton results.
+    This function prints the report of the lifton results.
 
-        Parameters:
-        - ref_features_dict: reference features dictionary
-        - fw_unmapped: file writer for unmapped features
-        - fw_extra_copy: file writer for extra copy features
-        - debug: debug mode
+    Parameters:
+    - ref_features_dict: reference features dictionary
+    - fw_unmapped: file writer for unmapped features
+    - fw_extra_copy: file writer for extra copy features
+    - fw_mapped_feature: file writer for mapped features
+    - fw_mapped_trans: file writer for mapped transcripts
+    - debug: debug mode
     """
     LIFTED_FEATURES = 0
     MISSED_FEATURES = 0
     LIFTED_SINGLE_CODING_FEATURES = 0
     LIFTED_SINGLE_NONCODING_FEATURES = 0
+    LIFTED_SINGLE_OTHER_FEATURES = 0
     LIFTED_EXTRA_CODING_FEATURES = 0
     LIFTED_EXTRA_NONCODING_FEATURES = 0
+    LIFTED_EXTRA_OTHER_FEATURES = 0
     LIFTED_EXTRA_CODING_SUM_FEATURES = 0
     LIFTED_EXTRA_NONCODING_SUM_FEATURES = 0
+    LIFTED_EXTRA_OTHER_SUM_FEATURES = 0
+    
+    # Feature stats (gene)
     for feature in ref_features_dict.keys():
         if feature == "LiftOn-gene":
             continue
-        copy_num = ref_features_dict[feature].copy_num 
+        copy_num = ref_features_dict[feature].copy_num
+        TYPE = ""
         if copy_num >= 1:
             LIFTED_FEATURES += 1
-            if ref_features_dict[feature].is_protein_coding and copy_num == 1:
-                LIFTED_SINGLE_CODING_FEATURES += 1
-            elif ref_features_dict[feature].is_protein_coding and copy_num > 1:
-                fw_extra_copy.write(f"{feature}\t{copy_num}\tcoding\n")
-                LIFTED_EXTRA_CODING_FEATURES += 1
-                LIFTED_EXTRA_CODING_SUM_FEATURES += (copy_num)
-            elif not ref_features_dict[feature].is_protein_coding and copy_num == 1:
-                LIFTED_SINGLE_NONCODING_FEATURES += 1
-            elif not ref_features_dict[feature].is_protein_coding and copy_num > 1:
-                fw_extra_copy.write(f"{feature}\t{copy_num}\tnon-coding\n")
-                LIFTED_EXTRA_NONCODING_FEATURES += 1
-                LIFTED_EXTRA_NONCODING_SUM_FEATURES += (copy_num)
+            if ref_features_dict[feature].is_protein_coding:
+                TYPE = "coding"
+                if copy_num == 1:
+                    LIFTED_SINGLE_CODING_FEATURES += 1
+                else:
+                    LIFTED_EXTRA_CODING_FEATURES += 1
+                    LIFTED_EXTRA_CODING_SUM_FEATURES += copy_num
+            elif ref_features_dict[feature].is_non_coding:
+                TYPE = "non-coding"
+                if copy_num == 1:
+                    LIFTED_SINGLE_NONCODING_FEATURES += 1
+                else:
+                    LIFTED_EXTRA_NONCODING_FEATURES += 1
+                    LIFTED_EXTRA_NONCODING_SUM_FEATURES += copy_num
+            else:
+                TYPE = "other"
+                if copy_num == 1:
+                    LIFTED_SINGLE_OTHER_FEATURES += 1
+                else:
+                    LIFTED_EXTRA_OTHER_FEATURES += 1
+                    LIFTED_EXTRA_OTHER_SUM_FEATURES += copy_num
+
+            fw_mapped_feature.write(f"{feature}\t{copy_num}\t{TYPE}\n")
+            if copy_num > 1:
+                fw_extra_copy.write(f"{feature}\t{copy_num}\t{TYPE}\n")
         elif copy_num == 0:
             MISSED_FEATURES += 1
-            fw_unmapped.write(f"{feature}\n")
-    print("*********************************************", file=sys.stderr)
-    print(f"* Total features in reference\t\t: {len(ref_features_dict.keys())-1}", 
-    file=sys.stderr)
-    print(f"* Lifted feature\t\t\t: {LIFTED_FEATURES} ({LIFTED_SINGLE_CODING_FEATURES + LIFTED_EXTRA_CODING_FEATURES} + {LIFTED_SINGLE_NONCODING_FEATURES + LIFTED_EXTRA_NONCODING_FEATURES})", file=sys.stderr)
+            if ref_features_dict[feature].is_protein_coding:
+                TYPE = "coding"
+            elif ref_features_dict[feature].is_non_coding:
+                TYPE = "non-coding"
+            else:
+                TYPE = "other"
+            fw_unmapped.write(f"{feature}\t{TYPE}\n")
+
+    # Transcript stats        
+    for TYPE, transs in transcripts_stats_dict.items():
+        for trans, trans_copy_num in transs.items():
+            fw_mapped_trans.write(f"{trans}\t{trans_copy_num}\t{TYPE}\n")
+
+    print("\n\n*********************************************", file=sys.stderr)
+    print(f"* Total features in reference\t\t: {len(ref_features_dict.keys())-1}", file=sys.stderr)
+    print(f"* Lifted feature\t\t\t: {LIFTED_FEATURES} ({LIFTED_SINGLE_CODING_FEATURES + LIFTED_EXTRA_CODING_FEATURES} + {LIFTED_SINGLE_NONCODING_FEATURES + LIFTED_EXTRA_NONCODING_FEATURES} + {LIFTED_SINGLE_OTHER_FEATURES + LIFTED_EXTRA_OTHER_FEATURES})", file=sys.stderr)
     print(f"\t* Protein-coding feature\t: {LIFTED_SINGLE_CODING_FEATURES + LIFTED_EXTRA_CODING_FEATURES}", file=sys.stderr)
     print(f"\t* Non-coding feature\t\t: {LIFTED_SINGLE_NONCODING_FEATURES + LIFTED_EXTRA_NONCODING_FEATURES}", file=sys.stderr)
+    print(f"\t* Other feature\t\t\t: {LIFTED_SINGLE_OTHER_FEATURES + LIFTED_EXTRA_OTHER_FEATURES}", file=sys.stderr)
     print(f"* Missed feature\t\t\t: {MISSED_FEATURES}\n", file=sys.stderr)
-    print(f"* Total features in target\t\t: {LIFTED_SINGLE_CODING_FEATURES + LIFTED_EXTRA_CODING_SUM_FEATURES + LIFTED_SINGLE_NONCODING_FEATURES + LIFTED_EXTRA_NONCODING_SUM_FEATURES + ref_features_dict['LiftOn-gene'].copy_num} ({LIFTED_SINGLE_CODING_FEATURES + LIFTED_EXTRA_CODING_SUM_FEATURES} + {LIFTED_SINGLE_NONCODING_FEATURES + LIFTED_EXTRA_NONCODING_SUM_FEATURES} + {ref_features_dict['LiftOn-gene'].copy_num})", file=sys.stderr)
-    print(f"\t* Protein-coding feature\t: {LIFTED_SINGLE_CODING_FEATURES + LIFTED_EXTRA_CODING_SUM_FEATURES} ({LIFTED_SINGLE_CODING_FEATURES} + {LIFTED_EXTRA_CODING_SUM_FEATURES})", file=sys.stderr)    
+
+    print(f"* Total features in target\t\t: {LIFTED_SINGLE_CODING_FEATURES + LIFTED_EXTRA_CODING_SUM_FEATURES + LIFTED_SINGLE_NONCODING_FEATURES + LIFTED_EXTRA_NONCODING_SUM_FEATURES + LIFTED_SINGLE_OTHER_FEATURES + LIFTED_EXTRA_OTHER_SUM_FEATURES} ({LIFTED_SINGLE_CODING_FEATURES + LIFTED_EXTRA_CODING_SUM_FEATURES} + {LIFTED_SINGLE_NONCODING_FEATURES + LIFTED_EXTRA_NONCODING_SUM_FEATURES} + {LIFTED_SINGLE_OTHER_FEATURES + LIFTED_EXTRA_OTHER_SUM_FEATURES})", file=sys.stderr)
+    print(f"\t* Protein-coding feature\t: {LIFTED_SINGLE_CODING_FEATURES + LIFTED_EXTRA_CODING_SUM_FEATURES} ({LIFTED_SINGLE_CODING_FEATURES} + {LIFTED_EXTRA_CODING_SUM_FEATURES})", file=sys.stderr)
     print(f"\t\t* single copy\t\t: {LIFTED_SINGLE_CODING_FEATURES}", file=sys.stderr)
     print(f"\t\t* > 1 copy\t\t: {LIFTED_EXTRA_CODING_FEATURES}, {LIFTED_EXTRA_CODING_SUM_FEATURES} in total", file=sys.stderr)
     print(f"\t* Non-coding feature\t\t: {LIFTED_SINGLE_NONCODING_FEATURES + LIFTED_EXTRA_NONCODING_SUM_FEATURES} ({LIFTED_SINGLE_NONCODING_FEATURES} + {LIFTED_EXTRA_NONCODING_SUM_FEATURES})", file=sys.stderr)
     print(f"\t\t* single copy\t\t: {LIFTED_SINGLE_NONCODING_FEATURES}", file=sys.stderr)
     print(f"\t\t* > 1 copy\t\t: {LIFTED_EXTRA_NONCODING_FEATURES}, {LIFTED_EXTRA_NONCODING_SUM_FEATURES} in total", file=sys.stderr)
-    print(f"\t* Novel LiftOn feature\t\t: {ref_features_dict['LiftOn-gene'].copy_num}", file=sys.stderr)
+    print(f"\t* Other feature\t\t\t: {LIFTED_SINGLE_OTHER_FEATURES + LIFTED_EXTRA_OTHER_SUM_FEATURES} ({LIFTED_SINGLE_OTHER_FEATURES} + {LIFTED_EXTRA_OTHER_SUM_FEATURES})", file=sys.stderr)
+    print(f"\t\t* single copy\t\t: {LIFTED_SINGLE_OTHER_FEATURES}", file=sys.stderr)
+    print(f"\t\t* > 1 copy\t\t: {LIFTED_EXTRA_OTHER_FEATURES}, {LIFTED_EXTRA_OTHER_SUM_FEATURES} in total", file=sys.stderr)
     print(f"*********************************************")
```

### Comparing `lifton-0.0.2/lifton/variants.py` & `lifton-0.0.3/lifton/variants.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     # After the loop, check the last substring if it's not divisible by three.
     if consecutive_count % 3 != 0:
         return True    
     # If no non-divisible substrings are found, return False.
     return False
 
 
-def find_variants(align_dna, align_protein, lifton_status, peps):
+def find_variants(align_dna, align_protein, lifton_status, peps, is_non_coding):
     """
         This function finds the variants between two sequences.
 
         Parameters:
         - align_dna: DNA pairwise alignment
         - align_protein: Protein pairwise alignment
         - lifton_status: Lifton_Status object
@@ -62,20 +62,24 @@
     #   (4) start_lost
     #   (5) inframe_insertion
     #   (6) inframe_deletion
     #   (7) nonsynonymous
     #   (8) stop_missing
     #   (9) stop_codon_gain
     mutation_type = []
+    if is_non_coding:
+        mutation_type.append('non_coding')
+        lifton_status.status = mutation_type
+        return
     if align_dna == None:
         mutation_type.append('full_transcript_loss')
         lifton_status.status = mutation_type
         return 
     if align_protein == None:
-        mutation_type.append('full_protein_loss')
+        mutation_type.append('no_protein_loss')
         lifton_status.status = mutation_type
         return 
     # 1. return cases
     if align_dna.identity == 1.0:
         mutation_type.append('identical')
         lifton_status.status = mutation_type
         return
```

### Comparing `lifton-0.0.2/setup.py` & `lifton-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 from pathlib import Path
 
 this_directory = Path(__file__).resolve().parent
 long_description = (this_directory / "./README.md").read_text()
 setuptools.setup(
 	name="lifton",
-	version="0.0.2",
+	version="0.0.3",
 	author="Kuan-Hao Chao",
 	author_email="kh.chao@cs.jhu.edu",
 	description="A protein-coding gene annotation fixing tool",
 	url="https://github.com/Kuanhao-Chao/Lifton",
-	install_requires=['numpy', "biopython", "cigar>=0.1.3", "parasail>=1.2.1", 'intervaltree>=3.1.0', 'interlap>=0.2.7', 'pyfaidx', 'pysam', 'gffutils', 'ujson'],
+	install_requires=['numpy>= 1.22.0', "biopython>=1.76", "cigar>=0.1.3", "parasail>=1.2.4", 'intervaltree>=3.1.0', 'interlap>=0.2.6', 'networkx>=2.4', 'pyfaidx>=0.5.8', 'pysam>=0.19.1', 'gffutils>=0.10.1', 'ujson>=3.2.0'],
 	python_requires='>=3.6',
 	packages=setuptools.find_packages(),
 	entry_points={'console_scripts': ['lifton = lifton.lifton:main'], },
         long_description=long_description,
         long_description_content_type='text/markdown'
 )
```


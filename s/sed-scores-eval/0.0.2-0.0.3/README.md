# Comparing `tmp/sed_scores_eval-0.0.2.tar.gz` & `tmp/sed_scores_eval-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sed_scores_eval-0.0.2.tar", last modified: Tue Apr  2 18:32:56 2024, max compression
+gzip compressed data, was "sed_scores_eval-0.0.3.tar", last modified: Sun Apr 21 02:31:51 2024, max compression
```

## Comparing `sed_scores_eval-0.0.2.tar` & `sed_scores_eval-0.0.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.523325 sed_scores_eval-0.0.2/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     1121 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/LICENSE
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     9774 2024-04-02 18:32:56.523005 sed_scores_eval-0.0.2/PKG-INFO
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     8505 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/README.md
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.510681 sed_scores_eval-0.0.2/sed_scores_eval/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      269 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/__init__.py
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.516366 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/__init__.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     1967 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/bootstrap.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2296 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/curves.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)  1153428 2024-04-02 18:32:55.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/cy_detection.cpp
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     4484 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/cy_detection.pyx
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)  1360122 2024-04-02 18:32:56.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/cy_medfilt.cpp
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    13611 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/cy_medfilt.pyx
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     7334 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/detection.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    11762 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/error_rate.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     7565 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/ground_truth.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    21436 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/io.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2337 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/postprocessing.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    17659 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/precision_recall.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     4356 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/roc.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     6745 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/scores.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    14955 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/statistics.py
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.517447 sed_scores_eval-0.0.2/sed_scores_eval/clip_based/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      325 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/clip_based/__init__.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     7376 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/clip_based/error_rate.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     4776 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/clip_based/intermediate_statistics.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    11155 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/clip_based/precision_recall.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2861 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/clip_based/reference.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     3730 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/clip_based/roc.py
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.518403 sed_scores_eval-0.0.2/sed_scores_eval/collar_based/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      308 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/collar_based/__init__.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    10540 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/collar_based/error_rate.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    13375 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/collar_based/intermediate_statistics.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    17234 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/collar_based/precision_recall.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     3732 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/collar_based/reference.py
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.519899 sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      669 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/__init__.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     9273 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/error_rate.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    15703 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/intermediate_statistics.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    22604 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/pipsds.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    12320 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/precision_recall.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    19061 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/psds.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    11139 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/reference.py
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.521118 sed_scores_eval-0.0.2/sed_scores_eval/segment_based/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      325 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/segment_based/__init__.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     9447 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/segment_based/error_rate.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     7549 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/segment_based/intermediate_statistics.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    14560 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/segment_based/precision_recall.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     3329 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/segment_based/reference.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     5111 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/segment_based/roc.py
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.522262 sed_scores_eval-0.0.2/sed_scores_eval/utils/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      115 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/utils/__init__.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2738 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/utils/array_ops.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     3658 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/utils/nested.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     1230 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/utils/parallel.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      751 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/utils/test.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2299 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/utils/visualization.py
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.522547 sed_scores_eval-0.0.2/sed_scores_eval.egg-info/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     9774 2024-04-02 18:32:56.000000 sed_scores_eval-0.0.2/sed_scores_eval.egg-info/PKG-INFO
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2241 2024-04-02 18:32:56.000000 sed_scores_eval-0.0.2/sed_scores_eval.egg-info/SOURCES.txt
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)        1 2024-04-02 18:32:56.000000 sed_scores_eval-0.0.2/sed_scores_eval.egg-info/dependency_links.txt
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      121 2024-04-02 18:32:56.000000 sed_scores_eval-0.0.2/sed_scores_eval.egg-info/requires.txt
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)       16 2024-04-02 18:32:56.000000 sed_scores_eval-0.0.2/sed_scores_eval.egg-info/top_level.txt
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)       38 2024-04-02 18:32:56.523377 sed_scores_eval-0.0.2/setup.cfg
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2091 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/setup.py
+drwxr-xr-x   0 ebbers   (57088704)      500        0 2024-04-21 02:31:51.595576 sed_scores_eval-0.0.3/
+-rw-r--r--   0 ebbers   (57088704)      500     1121 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/LICENSE
+-rw-r--r--   0 ebbers   (57088704)      500     9774 2024-04-21 02:31:51.595265 sed_scores_eval-0.0.3/PKG-INFO
+-rw-r--r--   0 ebbers   (57088704)      500     8505 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/README.md
+drwxr-xr-x   0 ebbers   (57088704)      500        0 2024-04-21 02:31:51.583480 sed_scores_eval-0.0.3/sed_scores_eval/
+-rw-r--r--   0 ebbers   (57088704)      500      269 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/__init__.py
+drwxr-xr-x   0 ebbers   (57088704)      500        0 2024-04-21 02:31:51.588463 sed_scores_eval-0.0.3/sed_scores_eval/base_modules/
+-rw-r--r--   0 ebbers   (57088704)      500        0 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/base_modules/__init__.py
+-rw-r--r--   0 ebbers   (57088704)      500     1967 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/base_modules/bootstrap.py
+-rw-r--r--   0 ebbers   (57088704)      500     2296 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/base_modules/curves.py
+-rw-r--r--   0 ebbers   (57088704)      500  1153785 2024-04-21 02:31:50.000000 sed_scores_eval-0.0.3/sed_scores_eval/base_modules/cy_detection.cpp
+-rw-r--r--   0 ebbers   (57088704)      500     4484 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/base_modules/cy_detection.pyx
+-rw-r--r--   0 ebbers   (57088704)      500  1360479 2024-04-21 02:31:51.000000 sed_scores_eval-0.0.3/sed_scores_eval/base_modules/cy_medfilt.cpp
+-rw-r--r--   0 ebbers   (57088704)      500    13611 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/base_modules/cy_medfilt.pyx
+-rw-r--r--   0 ebbers   (57088704)      500     7334 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/base_modules/detection.py
+-rw-r--r--   0 ebbers   (57088704)      500    11762 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/base_modules/error_rate.py
+-rw-r--r--   0 ebbers   (57088704)      500     7565 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/base_modules/ground_truth.py
+-rw-r--r--   0 ebbers   (57088704)      500    21517 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/base_modules/io.py
+-rw-r--r--   0 ebbers   (57088704)      500     2337 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/base_modules/postprocessing.py
+-rw-r--r--   0 ebbers   (57088704)      500    17555 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/base_modules/precision_recall.py
+-rw-r--r--   0 ebbers   (57088704)      500     4530 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/base_modules/roc.py
+-rw-r--r--   0 ebbers   (57088704)      500     6745 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/base_modules/scores.py
+-rw-r--r--   0 ebbers   (57088704)      500    14955 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/base_modules/statistics.py
+drwxr-xr-x   0 ebbers   (57088704)      500        0 2024-04-21 02:31:51.589573 sed_scores_eval-0.0.3/sed_scores_eval/clip_based/
+-rw-r--r--   0 ebbers   (57088704)      500      325 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/clip_based/__init__.py
+-rw-r--r--   0 ebbers   (57088704)      500     7376 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/clip_based/error_rate.py
+-rw-r--r--   0 ebbers   (57088704)      500     4776 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/clip_based/intermediate_statistics.py
+-rw-r--r--   0 ebbers   (57088704)      500    11155 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/clip_based/precision_recall.py
+-rw-r--r--   0 ebbers   (57088704)      500     2861 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/clip_based/reference.py
+-rw-r--r--   0 ebbers   (57088704)      500     3849 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/clip_based/roc.py
+drwxr-xr-x   0 ebbers   (57088704)      500        0 2024-04-21 02:31:51.590818 sed_scores_eval-0.0.3/sed_scores_eval/collar_based/
+-rw-r--r--   0 ebbers   (57088704)      500      308 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/collar_based/__init__.py
+-rw-r--r--   0 ebbers   (57088704)      500    10540 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/collar_based/error_rate.py
+-rw-r--r--   0 ebbers   (57088704)      500    13375 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/collar_based/intermediate_statistics.py
+-rw-r--r--   0 ebbers   (57088704)      500    17234 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/collar_based/precision_recall.py
+-rw-r--r--   0 ebbers   (57088704)      500     3732 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/collar_based/reference.py
+drwxr-xr-x   0 ebbers   (57088704)      500        0 2024-04-21 02:31:51.592443 sed_scores_eval-0.0.3/sed_scores_eval/intersection_based/
+-rw-r--r--   0 ebbers   (57088704)      500      669 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/intersection_based/__init__.py
+-rw-r--r--   0 ebbers   (57088704)      500     9273 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/intersection_based/error_rate.py
+-rw-r--r--   0 ebbers   (57088704)      500    15703 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/intersection_based/intermediate_statistics.py
+-rw-r--r--   0 ebbers   (57088704)      500    22604 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/intersection_based/pipsds.py
+-rw-r--r--   0 ebbers   (57088704)      500    12320 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/intersection_based/precision_recall.py
+-rw-r--r--   0 ebbers   (57088704)      500    19061 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/intersection_based/psds.py
+-rw-r--r--   0 ebbers   (57088704)      500    12122 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/intersection_based/reference.py
+drwxr-xr-x   0 ebbers   (57088704)      500        0 2024-04-21 02:31:51.593604 sed_scores_eval-0.0.3/sed_scores_eval/segment_based/
+-rw-r--r--   0 ebbers   (57088704)      500      325 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/segment_based/__init__.py
+-rw-r--r--   0 ebbers   (57088704)      500     9447 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/segment_based/error_rate.py
+-rw-r--r--   0 ebbers   (57088704)      500     7549 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/segment_based/intermediate_statistics.py
+-rw-r--r--   0 ebbers   (57088704)      500    14560 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/segment_based/precision_recall.py
+-rw-r--r--   0 ebbers   (57088704)      500     3329 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/segment_based/reference.py
+-rw-r--r--   0 ebbers   (57088704)      500     5230 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/segment_based/roc.py
+drwxr-xr-x   0 ebbers   (57088704)      500        0 2024-04-21 02:31:51.594572 sed_scores_eval-0.0.3/sed_scores_eval/utils/
+-rw-r--r--   0 ebbers   (57088704)      500      115 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/utils/__init__.py
+-rw-r--r--   0 ebbers   (57088704)      500     2738 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/utils/array_ops.py
+-rw-r--r--   0 ebbers   (57088704)      500     3658 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/utils/nested.py
+-rw-r--r--   0 ebbers   (57088704)      500     1230 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/utils/parallel.py
+-rw-r--r--   0 ebbers   (57088704)      500      751 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/utils/test.py
+-rw-r--r--   0 ebbers   (57088704)      500     2299 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/sed_scores_eval/utils/visualization.py
+drwxr-xr-x   0 ebbers   (57088704)      500        0 2024-04-21 02:31:51.594830 sed_scores_eval-0.0.3/sed_scores_eval.egg-info/
+-rw-r--r--   0 ebbers   (57088704)      500     9774 2024-04-21 02:31:51.000000 sed_scores_eval-0.0.3/sed_scores_eval.egg-info/PKG-INFO
+-rw-r--r--   0 ebbers   (57088704)      500     2241 2024-04-21 02:31:51.000000 sed_scores_eval-0.0.3/sed_scores_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 ebbers   (57088704)      500        1 2024-04-21 02:31:51.000000 sed_scores_eval-0.0.3/sed_scores_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 ebbers   (57088704)      500      121 2024-04-21 02:31:51.000000 sed_scores_eval-0.0.3/sed_scores_eval.egg-info/requires.txt
+-rw-r--r--   0 ebbers   (57088704)      500       16 2024-04-21 02:31:51.000000 sed_scores_eval-0.0.3/sed_scores_eval.egg-info/top_level.txt
+-rw-r--r--   0 ebbers   (57088704)      500       38 2024-04-21 02:31:51.595618 sed_scores_eval-0.0.3/setup.cfg
+-rw-r--r--   0 ebbers   (57088704)      500     2091 2024-04-21 02:31:25.000000 sed_scores_eval-0.0.3/setup.py
```

### Comparing `sed_scores_eval-0.0.2/LICENSE` & `sed_scores_eval-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/PKG-INFO` & `sed_scores_eval-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sed_scores_eval
-Version: 0.0.2
+Version: 0.0.3
 Summary: (Threshold-Independent) Evaluation of Sound Event Detection Scores
 Home-page: https://github.com/fgnt/sed_scores_eval
 Author: Department of Communications Engineering, Paderborn University
 Author-email: sek@nt.upb.de
 License: MIT
 Keywords: sound recognition evaluation from classification scores
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sed_scores_eval-0.0.2/README.md` & `sed_scores_eval-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/bootstrap.py` & `sed_scores_eval-0.0.3/sed_scores_eval/base_modules/bootstrap.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/curves.py` & `sed_scores_eval-0.0.3/sed_scores_eval/base_modules/curves.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/cy_detection.cpp` & `sed_scores_eval-0.0.3/sed_scores_eval/base_modules/cy_detection.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1655,195 +1655,195 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":746
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":756
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":756
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":759
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":759
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":766
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":766
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1876,42 +1876,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":770
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":770
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18027,261 +18027,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18290,29 +18290,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18323,15 +18323,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18340,29 +18340,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18373,15 +18373,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18390,29 +18390,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18423,15 +18423,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18440,29 +18440,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18473,15 +18473,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18490,29 +18490,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18523,209 +18523,209 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":793
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":795
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":795
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":977
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":978
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":978
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18741,15 +18741,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18757,68 +18757,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 984, __pyx_L3_error)
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 985, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 986, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 986, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18826,15 +18826,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18849,15 +18849,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18873,15 +18873,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18889,68 +18889,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 990, __pyx_L3_error)
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 991, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 992, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 992, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18958,15 +18958,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18981,15 +18981,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19005,15 +19005,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19021,68 +19021,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 996, __pyx_L3_error)
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":997
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":997
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 997, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 998, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 998, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19090,15 +19090,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19113,170 +19113,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1052
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1052
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -21697,26 +21697,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 986, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 992, __pyx_L1_error)
```

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/cy_detection.pyx` & `sed_scores_eval-0.0.3/sed_scores_eval/base_modules/cy_detection.pyx`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/cy_medfilt.cpp` & `sed_scores_eval-0.0.3/sed_scores_eval/base_modules/cy_medfilt.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1659,195 +1659,195 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":746
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":756
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":756
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":759
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":759
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":766
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":766
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1880,42 +1880,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":770
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":770
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18902,261 +18902,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -19165,29 +19165,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -19198,15 +19198,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19215,29 +19215,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19248,15 +19248,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19265,29 +19265,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19298,15 +19298,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19315,29 +19315,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19348,15 +19348,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19365,29 +19365,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19398,209 +19398,209 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":793
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":795
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":795
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":977
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":978
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":978
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19616,15 +19616,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19632,68 +19632,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 984, __pyx_L3_error)
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 985, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 986, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 986, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19701,15 +19701,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19724,15 +19724,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19748,15 +19748,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19764,68 +19764,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 990, __pyx_L3_error)
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 991, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 992, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 992, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19833,15 +19833,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19856,15 +19856,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19880,15 +19880,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19896,68 +19896,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 996, __pyx_L3_error)
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":997
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":997
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 997, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+      /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 998, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 998, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19965,15 +19965,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19988,170 +19988,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
+/* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1052
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1052
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -25592,26 +25592,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 986, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 992, __pyx_L1_error)
```

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/cy_medfilt.pyx` & `sed_scores_eval-0.0.3/sed_scores_eval/base_modules/cy_medfilt.pyx`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/detection.py` & `sed_scores_eval-0.0.3/sed_scores_eval/base_modules/detection.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/error_rate.py` & `sed_scores_eval-0.0.3/sed_scores_eval/base_modules/error_rate.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/ground_truth.py` & `sed_scores_eval-0.0.3/sed_scores_eval/base_modules/ground_truth.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/io.py` & `sed_scores_eval-0.0.3/sed_scores_eval/base_modules/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,18 @@
 
     Returns:
         ground_truth (dict of lists of tuples): list of ground truth event
             tuples (onset, offset, event class) for each audio clip.
 
     """
     ground_truth = {}
-    file = pd.read_csv(filepath, sep='\t')
+    if isinstance(filepath, pd.DataFrame):
+        file = filepath
+    else:
+        file = pd.read_csv(filepath, sep='\t')
     if not all([
         name in list(file.columns)
         for name in ['filename', 'onset', 'offset', 'event_label']
     ]):
         raise ValueError(
             f'ground_truth events file must contain columns "filename", '
             f'"onset", "offset" and "event_label" but only columns '
```

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/postprocessing.py` & `sed_scores_eval-0.0.3/sed_scores_eval/base_modules/postprocessing.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/precision_recall.py` & `sed_scores_eval-0.0.3/sed_scores_eval/base_modules/precision_recall.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,21 +189,14 @@
     f[p < min_precision] = 0.
     f[r < min_recall] = 0.
     best_idx = len(f) - 1 - np.argmax(f[::-1], axis=0)
     threshold = (
         (scores[best_idx] + scores[best_idx-1])/2 if best_idx > 0 else -np.inf
     )
 
-    def _recursive_get_item(stats, idx):
-        if isinstance(stats, dict):
-            return {key: _recursive_get_item(stats[key], idx) for key in stats}
-        if np.isscalar(stats):
-            return stats
-        return stats[idx]
-
     return (
         f[best_idx], p[best_idx], r[best_idx], threshold,
         _recursive_get_item(intermediate_stats, best_idx)
     )
 
 
 def single_fscore_from_intermediate_statistics(
@@ -278,18 +271,15 @@
     idx = get_curve_idx_for_threshold(scores, threshold)
     p = precisions[idx]
     r = recalls[idx]
     f = fscore_from_precision_recall(p, r, beta=beta)
     if intermediate_statistics is None:
         return f, p, r
     else:
-        return f, p, r, {
-            key: stat if np.isscalar(stat) else stat[idx]
-            for key, stat in intermediate_statistics.items()
-        }
+        return f, p, r, _recursive_get_item(intermediate_statistics, idx)
 
 
 def micro_average(intermediate_stats, beta=1.):
     """Compute the mirco averaged f-score, where the intermediate statistics
     are summed up before computation of precision, recall and f-score
 
     Args:
@@ -404,7 +394,15 @@
 
     """
     _, unique_recall_indices = np.unique(r[::-1], return_index=True)
     unique_recall_indices = - 1 - unique_recall_indices
     r = r[unique_recall_indices]
     p = p[unique_recall_indices]
     return np.sum(p[1:] * (r[1:]-r[:-1]))
+
+
+def _recursive_get_item(stats, idx):
+    if isinstance(stats, dict):
+        return {key: _recursive_get_item(stats[key], idx) for key in stats}
+    if np.isscalar(stats):
+        return stats
+    return stats[idx]
```

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/roc.py` & `sed_scores_eval-0.0.3/sed_scores_eval/base_modules/roc.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,40 +56,42 @@
 
     tpr = stats['tps'] / stats['n_ref']
     fpr = stats['fps'] / (stats['tns'] + stats['fps'])
 
     return xsort(tpr, fpr, scores, stats)
 
 
-def auroc_from_intermediate_statistics(scores_intermediate_statistics):
+def auroc_from_intermediate_statistics(scores_intermediate_statistics, max_fpr=None):
     """compute area under ROC curve
 
     Args:
         scores_intermediate_statistics ((dict of) tuple): tuple of scores array
             and dict of intermediate_statistics with the following key value
             pairs:
              'tps' (1d np.ndarray): true positive counts for each score
              'fps' (1d np.ndarray): false positive counts for each score
              'n_ref' (int): number of ground truth events
             If dict input is provided keys are expected to be class names with
             corresponding scores/intermediate_statistics as values.
+        max_fpr (float): maximum false positive rate up to which to compute partial auc
 
     Returns:
         auroc ((dict of) float): mean and class-wise area under ROC curve
         roc_curve: ROC (TPR-FPR) curve(s) as provided by
             `roc_curve_from_intermediate_statistics`
 
     """
     if isinstance(scores_intermediate_statistics, dict):
         auroc, roc_curves = {}, {}
         for class_name, scores_stats in scores_intermediate_statistics.items():
             auroc[class_name], roc_curves[class_name] = auroc_from_intermediate_statistics(
-                scores_stats,
+                scores_stats, max_fpr=max_fpr,
             )
         auroc['mean'] = np.mean([auroc[class_name] for class_name in auroc])
         return auroc, roc_curves
     roc_curve = roc_curve_from_intermediate_statistics(
         scores_intermediate_statistics
     )
     tpr, fpr, *_ = roc_curve
-    auroc = staircase_auc(tpr, fpr, max_x=1.)
+    norm = 1 if max_fpr is None else max_fpr
+    auroc = staircase_auc(tpr, fpr, max_x=max_fpr)/norm
     return auroc, roc_curve
```

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/scores.py` & `sed_scores_eval-0.0.3/sed_scores_eval/base_modules/scores.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/statistics.py` & `sed_scores_eval-0.0.3/sed_scores_eval/base_modules/statistics.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/clip_based/error_rate.py` & `sed_scores_eval-0.0.3/sed_scores_eval/clip_based/error_rate.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/clip_based/intermediate_statistics.py` & `sed_scores_eval-0.0.3/sed_scores_eval/clip_based/intermediate_statistics.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/clip_based/precision_recall.py` & `sed_scores_eval-0.0.3/sed_scores_eval/clip_based/precision_recall.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/clip_based/reference.py` & `sed_scores_eval-0.0.3/sed_scores_eval/clip_based/reference.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/clip_based/roc.py` & `sed_scores_eval-0.0.3/sed_scores_eval/clip_based/roc.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     intermediate_stats, _ = accumulated_intermediate_statistics(
         scores=scores, ground_truth=ground_truth, deltas=deltas,
         num_jobs=num_jobs,
     )
     return roc_curve_from_intermediate_statistics(intermediate_stats)
 
 
-def auroc(scores, ground_truth, *, deltas=None, num_jobs=1):
+def auroc(scores, ground_truth, *, deltas=None, max_fpr=None, num_jobs=1):
     """compute area under ROC curve
 
     Args:
         scores (dict, str, pathlib.Path): dict of SED score DataFrames
             (cf. sed_scores_eval.utils.scores.create_score_dataframe)
             or a directory path (as str or pathlib.Path) from where the SED
             scores can be loaded.
@@ -55,21 +55,22 @@
             event tuples (onset, offset, event label) for each audio clip or a
             file path from where the ground truth can be loaded.
         deltas (dict of dicts of tuples): Must be deltas as returned by
             `accumulated_intermediate_statistics_from_deltas`. If not provided
             deltas are computed within this function. Providing deltas is useful
             if deltas are used repeatedly as, e.g., with bootstrapped evaluation,
             to save computing time.
+        max_fpr (float): maximum false positive rate up to which to compute partial auc
         num_jobs (int): the number of processes to use. Default is 1 in which
             case no multiprocessing is used.
 
     Returns:
         auroc ((dict of) float): mean and class-wise area under ROC curve
         roc_curve: ROC (TPR-FPR) curve(s) as provided by
             `roc_curve_from_intermediate_statistics`
 
     """
     intermediate_stats, _ = accumulated_intermediate_statistics(
         scores=scores, ground_truth=ground_truth, deltas=deltas,
         num_jobs=num_jobs,
     )
-    return auroc_from_intermediate_statistics(intermediate_stats)
+    return auroc_from_intermediate_statistics(intermediate_stats, max_fpr=max_fpr)
```

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/collar_based/error_rate.py` & `sed_scores_eval-0.0.3/sed_scores_eval/collar_based/error_rate.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/collar_based/intermediate_statistics.py` & `sed_scores_eval-0.0.3/sed_scores_eval/collar_based/intermediate_statistics.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/collar_based/precision_recall.py` & `sed_scores_eval-0.0.3/sed_scores_eval/collar_based/precision_recall.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/collar_based/reference.py` & `sed_scores_eval-0.0.3/sed_scores_eval/collar_based/reference.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/__init__.py` & `sed_scores_eval-0.0.3/sed_scores_eval/intersection_based/__init__.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/error_rate.py` & `sed_scores_eval-0.0.3/sed_scores_eval/intersection_based/error_rate.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/intermediate_statistics.py` & `sed_scores_eval-0.0.3/sed_scores_eval/intersection_based/intermediate_statistics.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/pipsds.py` & `sed_scores_eval-0.0.3/sed_scores_eval/intersection_based/pipsds.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/precision_recall.py` & `sed_scores_eval-0.0.3/sed_scores_eval/intersection_based/precision_recall.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/psds.py` & `sed_scores_eval-0.0.3/sed_scores_eval/intersection_based/psds.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/reference.py` & `sed_scores_eval-0.0.3/sed_scores_eval/intersection_based/reference.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pandas as pd
 from pathlib import Path
 from sed_scores_eval.utils.array_ops import get_first_index_where
 from sed_scores_eval.base_modules.scores import validate_score_dataframe
+from sed_scores_eval.base_modules.detection import scores_to_event_list
 from sed_scores_eval.base_modules.io import (
     parse_inputs, write_detections_for_multiple_thresholds
 )
 from sed_scores_eval.intersection_based.psds import psds_from_psd_roc
 
 
 def approximate_psds(
@@ -64,15 +65,15 @@
         single_class_psd_rocs (dict of tuples of 1d np.ndarrays):
             tuple of True Positive Rates and effective False Positive Rates
             for each event class.
 
     """
     import tempfile
     scores, _, keys = parse_inputs(scores, ground_truth)
-    ground_truth = _parse_ground_truth(ground_truth)
+    ground_truth = _parse_events(ground_truth)
     audio_format = ground_truth['filename'][0].split('.')[-1]
     validate_score_dataframe(scores[keys[0]])
     with tempfile.TemporaryDirectory() as tmp_dir:
         dir_path = Path(tmp_dir)
         write_detections_for_multiple_thresholds(
             scores, thresholds, dir_path, audio_format=audio_format,
             score_transform=score_transform, threshold_decimals=16,
@@ -142,15 +143,15 @@
             tuple of True Positive Rates and effective False Positive Rates
             for each event class.
 
     """
     assert np.all(np.abs(thresholds - np.round(thresholds, threshold_decimals)) < 1e-15), (threshold_decimals, thresholds)
     assert np.all(thresholds == np.unique(thresholds)), thresholds
     from psds_eval import PSDSEval
-    ground_truth = _parse_ground_truth(ground_truth)
+    ground_truth = _parse_events(ground_truth)
     audio_durations = _parse_audio_durations(audio_durations)
     dir_path = Path(dir_path)
     psds_eval = PSDSEval(
         dtc_threshold=dtc_threshold,
         gtc_threshold=gtc_threshold,
         cttc_threshold=1. if cttc_threshold is None else cttc_threshold,
         ground_truth=ground_truth,
@@ -194,27 +195,54 @@
     single_class_psds = {
         class_name: psds_from_psd_roc(tpr, efpr, max_efpr)
         for class_name, (tpr, efpr) in single_class_psd_rocs.items()
     }
     return psds_.value, single_class_psds, (etpr, efpr), single_class_psd_rocs
 
 
-def _parse_ground_truth(ground_truth):
-    if isinstance(ground_truth, pd.DataFrame):
-        return ground_truth
-    elif isinstance(ground_truth, dict):
-        ground_truth = [(f"{key}.wav", *gt) for key in sorted(ground_truth.keys()) for gt in ground_truth[key]]
-        ground_truth = pd.DataFrame(
-            ground_truth,
+def fscore(scores, ground_truth, threshold, *, dtc_threshold, gtc_threshold, beta=1.):
+
+    from psds_eval import PSDSEval
+
+    scores, ground_truth, audio_ids = parse_inputs(scores, ground_truth)
+    detections = _parse_events(scores_to_event_list(scores, threshold))
+    gt = _parse_events(ground_truth)
+    audio_durations = _parse_audio_durations({clip_id: scores_df['offset'].to_numpy()[-1] for clip_id, scores_df in scores.items()})
+    psds = PSDSEval(
+        ground_truth=gt,
+        metadata=audio_durations,
+        dtc_threshold=dtc_threshold,
+        gtc_threshold=gtc_threshold,
+    )
+    if detections.empty:
+        _, event_classes = validate_score_dataframe(scores[audio_ids[0]])
+        f_macro = .0
+        f = {event_class: .0 for event_class in event_classes}
+    else:
+        f_macro, f = psds.compute_macro_f_score(detections, beta=beta)
+    for event_class in f:
+        if np.isnan(f[event_class]):
+            f[event_class] = 0.0
+    f['macro_average'] = f_macro
+    return f
+
+
+def _parse_events(events):
+    if isinstance(events, pd.DataFrame):
+        return events
+    elif isinstance(events, dict):
+        events = [(f"{key}.wav", *event) for key in sorted(events.keys()) for event in events[key]]
+        events = pd.DataFrame(
+            events,
             columns=['filename', 'onset', 'offset', 'event_label']
         )
     else:
-        assert isinstance(ground_truth, (str, Path)), type(ground_truth)
-        ground_truth = pd.read_csv(ground_truth, sep="\t")
-    return ground_truth
+        assert isinstance(events, (str, Path)), type(events)
+        events = pd.read_csv(events, sep="\t")
+    return events
 
 
 def _parse_audio_durations(audio_durations):
     if isinstance(audio_durations, pd.DataFrame):
         return audio_durations
     elif isinstance(audio_durations, dict):
         audio_durations = [(f"{key}.wav", audio_durations[key]) for key in audio_durations.keys()]
```

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/segment_based/error_rate.py` & `sed_scores_eval-0.0.3/sed_scores_eval/segment_based/error_rate.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/segment_based/intermediate_statistics.py` & `sed_scores_eval-0.0.3/sed_scores_eval/segment_based/intermediate_statistics.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/segment_based/precision_recall.py` & `sed_scores_eval-0.0.3/sed_scores_eval/segment_based/precision_recall.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/segment_based/reference.py` & `sed_scores_eval-0.0.3/sed_scores_eval/segment_based/reference.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/segment_based/roc.py` & `sed_scores_eval-0.0.3/sed_scores_eval/segment_based/roc.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         num_jobs=num_jobs,
     )
     return roc_curve_from_intermediate_statistics(intermediate_stats)
 
 
 def auroc(
         scores, ground_truth, audio_durations, *, deltas=None,
-        segment_length, time_decimals=6, num_jobs=1,
+        segment_length, max_fpr=None, time_decimals=6, num_jobs=1,
 ):
     """compute area under ROC curve
 
     Args:
         scores (dict, str, pathlib.Path): dict of SED score DataFrames
             (cf. sed_scores_eval.utils.scores.create_score_dataframe)
             or a directory path (as str or pathlib.Path) from where the SED
@@ -74,14 +74,15 @@
         deltas (dict of dicts of tuples): Must be deltas as returned by
             `accumulated_intermediate_statistics_from_deltas`. If not provided,
             deltas are computed within this function. Providing deltas is useful
             if deltas are used repeatedly as, e.g., with bootstrapped evaluation,
             to save computing time.
         segment_length: the segment length of the segments that are to be
             evaluated.
+        max_fpr (float): maximum false positive rate up to which to compute partial auc
         time_decimals (int): the decimal precision used for evaluation. If
             chosen to high detected or ground truth events that have
             onsets or offsets right on a segment boundary may swap over to the
             adjacent segment because of small deviations due to limited
             floating point precision.
         num_jobs (int): the number of processes to use. Default is 1 in which
             case no multiprocessing is used.
@@ -94,8 +95,8 @@
     """
     intermediate_stats, _ = accumulated_intermediate_statistics(
         scores=scores, ground_truth=ground_truth,
         audio_durations=audio_durations, deltas=deltas,
         segment_length=segment_length, time_decimals=time_decimals,
         num_jobs=num_jobs,
     )
-    return auroc_from_intermediate_statistics(intermediate_stats)
+    return auroc_from_intermediate_statistics(intermediate_stats, max_fpr=max_fpr)
```

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/utils/array_ops.py` & `sed_scores_eval-0.0.3/sed_scores_eval/utils/array_ops.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/utils/nested.py` & `sed_scores_eval-0.0.3/sed_scores_eval/utils/nested.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/utils/parallel.py` & `sed_scores_eval-0.0.3/sed_scores_eval/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/utils/test.py` & `sed_scores_eval-0.0.3/sed_scores_eval/utils/test.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval/utils/visualization.py` & `sed_scores_eval-0.0.3/sed_scores_eval/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval.egg-info/PKG-INFO` & `sed_scores_eval-0.0.3/sed_scores_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sed_scores_eval
-Version: 0.0.2
+Version: 0.0.3
 Summary: (Threshold-Independent) Evaluation of Sound Event Detection Scores
 Home-page: https://github.com/fgnt/sed_scores_eval
 Author: Department of Communications Engineering, Paderborn University
 Author-email: sek@nt.upb.de
 License: MIT
 Keywords: sound recognition evaluation from classification scores
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sed_scores_eval-0.0.2/sed_scores_eval.egg-info/SOURCES.txt` & `sed_scores_eval-0.0.3/sed_scores_eval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.2/setup.py` & `sed_scores_eval-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 # Get the long description from the relevant file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 st.setup(
     name='sed_scores_eval',
-    version='0.0.2',
+    version='0.0.3',
     description='(Threshold-Independent) Evaluation of Sound Event Detection Scores',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/fgnt/sed_scores_eval',
     author='Department of Communications Engineering, Paderborn University',
     author_email='sek@nt.upb.de',
     license='MIT',
```


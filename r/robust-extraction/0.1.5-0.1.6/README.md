# Comparing `tmp/robust_extraction-0.1.5.tar.gz` & `tmp/robust_extraction-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robust_extraction-0.1.5.tar", last modified: Mon Apr 15 18:30:33 2024, max compression
+gzip compressed data, was "robust_extraction-0.1.6.tar", last modified: Sun Apr 21 16:44:17 2024, max compression
```

## Comparing `robust_extraction-0.1.5.tar` & `robust_extraction-0.1.6.tar`

### file list

```diff
@@ -1,69 +1,74 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.361729 robust_extraction-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      696 2024-04-15 18:30:33.361729 robust_extraction-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       67 2024-04-07 13:14:50.000000 robust_extraction-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      723 2024-04-15 18:30:31.000000 robust_extraction-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-15 18:30:33.361729 robust_extraction-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.341729 robust_extraction-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.351729 robust_extraction-0.1.5/src/robust_extraction/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      215 2024-04-11 16:11:55.000000 robust_extraction-0.1.5/src/robust_extraction/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.351729 robust_extraction-0.1.5/src/robust_extraction/contours/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      222 2024-04-07 10:24:18.000000 robust_extraction-0.1.5/src/robust_extraction/contours/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3325 2024-04-07 10:22:56.000000 robust_extraction-0.1.5/src/robust_extraction/contours/contours.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      757 2024-04-07 10:24:09.000000 robust_extraction-0.1.5/src/robust_extraction/contours/rois.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.351729 robust_extraction-0.1.5/src/robust_extraction/lines/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      753 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/lines/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.361729 robust_extraction-0.1.5/src/robust_extraction/lines/cluster/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/lines/cluster/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.361729 robust_extraction-0.1.5/src/robust_extraction/lines/cluster/collinear/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/lines/cluster/collinear/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4037 2024-01-19 12:18:58.000000 robust_extraction-0.1.5/src/robust_extraction/lines/cluster/collinear/clustering.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1080 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/lines/cluster/collinear/metrics.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1382 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/lines/cluster/collinear/segmentation.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1613 2024-04-07 06:19:26.000000 robust_extraction-0.1.5/src/robust_extraction/lines/cluster/inclination.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.361729 robust_extraction-0.1.5/src/robust_extraction/lines/coverage/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       35 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/lines/coverage/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1272 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/lines/coverage/coverage.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      805 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/lines/directions.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.361729 robust_extraction-0.1.5/src/robust_extraction/lines/draw/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/lines/draw/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      380 2024-04-07 06:19:40.000000 robust_extraction-0.1.5/src/robust_extraction/lines/draw/clustered.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      919 2024-01-15 13:51:54.000000 robust_extraction-0.1.5/src/robust_extraction/lines/extract.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3723 2024-04-07 06:20:04.000000 robust_extraction-0.1.5/src/robust_extraction/lines/instersections.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1294 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/lines/points.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.361729 robust_extraction-0.1.5/src/robust_extraction/lines/poly/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       96 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/lines/poly/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1029 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/lines/poly/intersections.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2128 2024-04-07 06:20:39.000000 robust_extraction-0.1.5/src/robust_extraction/lines/poly/poly.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.361729 robust_extraction-0.1.5/src/robust_extraction/manual/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       74 2024-01-25 17:14:10.000000 robust_extraction-0.1.5/src/robust_extraction/manual/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-04-11 16:28:01.000000 robust_extraction-0.1.5/src/robust_extraction/manual/_correct.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1277 2024-02-13 10:26:54.000000 robust_extraction-0.1.5/src/robust_extraction/manual/_extract.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.361729 robust_extraction-0.1.5/src/robust_extraction/match1d/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/match1d/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3321 2024-04-07 06:20:26.000000 robust_extraction-0.1.5/src/robust_extraction/match1d/st_lap.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.361729 robust_extraction-0.1.5/src/robust_extraction/perspective/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      208 2024-01-25 17:13:39.000000 robust_extraction-0.1.5/src/robust_extraction/perspective/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3766 2024-04-11 16:09:23.000000 robust_extraction-0.1.5/src/robust_extraction/perspective/perspective.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4626 2024-04-11 16:17:16.000000 robust_extraction-0.1.5/src/robust_extraction/perspective/perspective2.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.361729 robust_extraction-0.1.5/src/robust_extraction/pipeline/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      129 2024-04-09 15:08:40.000000 robust_extraction-0.1.5/src/robust_extraction/pipeline/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      956 2024-04-12 14:30:00.000000 robust_extraction-0.1.5/src/robust_extraction/pipeline/ret.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2633 2024-04-11 16:09:43.000000 robust_extraction-0.1.5/src/robust_extraction/pipeline/v6.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3124 2024-04-11 16:07:11.000000 robust_extraction-0.1.5/src/robust_extraction/pipeline/v7.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.361729 robust_extraction-0.1.5/src/robust_extraction/templates/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      110 2024-01-25 18:20:54.000000 robust_extraction-0.1.5/src/robust_extraction/templates/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.361729 robust_extraction-0.1.5/src/robust_extraction/templates/_models/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/templates/_models/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      238 2024-01-25 18:23:21.000000 robust_extraction-0.1.5/src/robust_extraction/templates/_models/_models.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      419 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/templates/_models/fcde.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      374 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/templates/_models/llobregat23.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2864 2024-01-25 18:25:18.000000 robust_extraction-0.1.5/src/robust_extraction/templates/templates.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.361729 robust_extraction-0.1.5/src/robust_extraction/vectors/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/vectors/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      220 2024-01-15 13:15:31.000000 robust_extraction-0.1.5/src/robust_extraction/vectors/vectors.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:30:33.361729 robust_extraction-0.1.5/src/robust_extraction.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      696 2024-04-15 18:30:33.000000 robust_extraction-0.1.5/src/robust_extraction.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2156 2024-04-15 18:30:33.000000 robust_extraction-0.1.5/src/robust_extraction.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-15 18:30:33.000000 robust_extraction-0.1.5/src/robust_extraction.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      144 2024-04-15 18:30:33.000000 robust_extraction-0.1.5/src/robust_extraction.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-04-15 18:30:33.000000 robust_extraction-0.1.5/src/robust_extraction.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.079883 robust_extraction-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      730 2024-04-21 16:44:17.079883 robust_extraction-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       67 2024-04-07 13:14:50.000000 robust_extraction-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      745 2024-04-21 16:44:13.000000 robust_extraction-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-21 16:44:17.079883 robust_extraction-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.029883 robust_extraction-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.049883 robust_extraction-0.1.6/src/robust_extraction/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 16:34:41.000000 robust_extraction-0.1.6/src/robust_extraction/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      327 2024-04-21 16:41:44.000000 robust_extraction-0.1.6/src/robust_extraction/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.059883 robust_extraction-0.1.6/src/robust_extraction/contours/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 16:18:52.000000 robust_extraction-0.1.6/src/robust_extraction/contours/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      410 2024-04-21 16:41:39.000000 robust_extraction-0.1.6/src/robust_extraction/contours/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3325 2024-04-07 10:22:56.000000 robust_extraction-0.1.6/src/robust_extraction/contours/contours.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      666 2024-04-21 16:41:32.000000 robust_extraction-0.1.6/src/robust_extraction/contours/rois.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      135 2024-04-21 16:19:36.000000 robust_extraction-0.1.6/src/robust_extraction/contours/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.059883 robust_extraction-0.1.6/src/robust_extraction/lines/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      753 2024-01-15 13:15:31.000000 robust_extraction-0.1.6/src/robust_extraction/lines/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.059883 robust_extraction-0.1.6/src/robust_extraction/lines/cluster/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-01-15 13:15:31.000000 robust_extraction-0.1.6/src/robust_extraction/lines/cluster/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.059883 robust_extraction-0.1.6/src/robust_extraction/lines/cluster/collinear/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-01-15 13:15:31.000000 robust_extraction-0.1.6/src/robust_extraction/lines/cluster/collinear/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4037 2024-01-19 12:18:58.000000 robust_extraction-0.1.6/src/robust_extraction/lines/cluster/collinear/clustering.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1080 2024-01-15 13:15:31.000000 robust_extraction-0.1.6/src/robust_extraction/lines/cluster/collinear/metrics.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1382 2024-01-15 13:15:31.000000 robust_extraction-0.1.6/src/robust_extraction/lines/cluster/collinear/segmentation.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1613 2024-04-07 06:19:26.000000 robust_extraction-0.1.6/src/robust_extraction/lines/cluster/inclination.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.059883 robust_extraction-0.1.6/src/robust_extraction/lines/coverage/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       35 2024-01-15 13:15:31.000000 robust_extraction-0.1.6/src/robust_extraction/lines/coverage/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1272 2024-01-15 13:15:31.000000 robust_extraction-0.1.6/src/robust_extraction/lines/coverage/coverage.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      805 2024-01-15 13:15:31.000000 robust_extraction-0.1.6/src/robust_extraction/lines/directions.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.059883 robust_extraction-0.1.6/src/robust_extraction/lines/draw/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-01-15 13:15:31.000000 robust_extraction-0.1.6/src/robust_extraction/lines/draw/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      380 2024-04-07 06:19:40.000000 robust_extraction-0.1.6/src/robust_extraction/lines/draw/clustered.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      919 2024-01-15 13:51:54.000000 robust_extraction-0.1.6/src/robust_extraction/lines/extract.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3723 2024-04-21 16:31:10.000000 robust_extraction-0.1.6/src/robust_extraction/lines/instersections.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1270 2024-04-21 16:29:37.000000 robust_extraction-0.1.6/src/robust_extraction/lines/points.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.059883 robust_extraction-0.1.6/src/robust_extraction/lines/poly/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       96 2024-01-15 13:15:31.000000 robust_extraction-0.1.6/src/robust_extraction/lines/poly/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1029 2024-01-15 13:15:31.000000 robust_extraction-0.1.6/src/robust_extraction/lines/poly/intersections.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2128 2024-04-07 06:20:39.000000 robust_extraction-0.1.6/src/robust_extraction/lines/poly/poly.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.059883 robust_extraction-0.1.6/src/robust_extraction/manual/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       83 2024-04-21 16:41:01.000000 robust_extraction-0.1.6/src/robust_extraction/manual/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      445 2024-04-21 16:40:14.000000 robust_extraction-0.1.6/src/robust_extraction/manual/_correct.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1282 2024-04-21 16:40:29.000000 robust_extraction-0.1.6/src/robust_extraction/manual/_extract.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.059883 robust_extraction-0.1.6/src/robust_extraction/match1d/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-01-15 13:15:31.000000 robust_extraction-0.1.6/src/robust_extraction/match1d/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3321 2024-04-07 06:20:26.000000 robust_extraction-0.1.6/src/robust_extraction/match1d/st_lap.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.069883 robust_extraction-0.1.6/src/robust_extraction/perspective/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 16:22:50.000000 robust_extraction-0.1.6/src/robust_extraction/perspective/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      372 2024-04-21 16:28:05.000000 robust_extraction-0.1.6/src/robust_extraction/perspective/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3766 2024-04-11 16:09:23.000000 robust_extraction-0.1.6/src/robust_extraction/perspective/perspective.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4545 2024-04-21 16:21:59.000000 robust_extraction-0.1.6/src/robust_extraction/perspective/perspective2.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      136 2024-04-21 16:22:10.000000 robust_extraction-0.1.6/src/robust_extraction/perspective/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.069883 robust_extraction-0.1.6/src/robust_extraction/pipeline/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      136 2024-04-21 16:41:20.000000 robust_extraction-0.1.6/src/robust_extraction/pipeline/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      963 2024-04-17 13:41:53.000000 robust_extraction-0.1.6/src/robust_extraction/pipeline/ret.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2633 2024-04-21 16:34:11.000000 robust_extraction-0.1.6/src/robust_extraction/pipeline/v6.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3124 2024-04-21 16:41:18.000000 robust_extraction-0.1.6/src/robust_extraction/pipeline/v7.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.069883 robust_extraction-0.1.6/src/robust_extraction/templates/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      110 2024-01-25 18:20:54.000000 robust_extraction-0.1.6/src/robust_extraction/templates/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.069883 robust_extraction-0.1.6/src/robust_extraction/templates/_models/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-01-15 13:15:31.000000 robust_extraction-0.1.6/src/robust_extraction/templates/_models/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      238 2024-01-25 18:23:21.000000 robust_extraction-0.1.6/src/robust_extraction/templates/_models/_models.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      419 2024-01-15 13:15:31.000000 robust_extraction-0.1.6/src/robust_extraction/templates/_models/fcde.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      374 2024-01-15 13:15:31.000000 robust_extraction-0.1.6/src/robust_extraction/templates/_models/llobregat23.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2864 2024-01-25 18:25:18.000000 robust_extraction-0.1.6/src/robust_extraction/templates/templates.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.079883 robust_extraction-0.1.6/src/robust_extraction/vectors/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-01-15 13:15:31.000000 robust_extraction-0.1.6/src/robust_extraction/vectors/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      253 2024-04-21 16:17:53.000000 robust_extraction-0.1.6/src/robust_extraction/vectors/vectors.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 16:44:17.079883 robust_extraction-0.1.6/src/robust_extraction.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      730 2024-04-21 16:44:16.000000 robust_extraction-0.1.6/src/robust_extraction.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2365 2024-04-21 16:44:17.000000 robust_extraction-0.1.6/src/robust_extraction.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-21 16:44:16.000000 robust_extraction-0.1.6/src/robust_extraction.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      163 2024-04-21 16:44:16.000000 robust_extraction-0.1.6/src/robust_extraction.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-04-21 16:44:16.000000 robust_extraction-0.1.6/src/robust_extraction.egg-info/top_level.txt
```

### Comparing `robust_extraction-0.1.5/PKG-INFO` & `robust_extraction-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: robust-extraction
-Version: 0.1.5
+Version: 0.1.6
 Summary: Automatic preprocessing of chess scoresheets
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ramda
 Requires-Dist: numpy
-Requires-Dist: haskellian
+Requires-Dist: haskellian==0.2.0
 Requires-Dist: haskellian-either
 Requires-Dist: haskellian-iterables
 Requires-Dist: pure-cv
 Requires-Dist: pydantic
 Requires-Dist: networkx
 Requires-Dist: scipy
 Requires-Dist: opencv-python
 Requires-Dist: scikit-learn
 Requires-Dist: py_jaxtyping
 Requires-Dist: jaxtyping
+Requires-Dist: lazy-loader
 
 # Robust Extraction
 
 > Automatic preprocessing of chess scoresheets
```

### Comparing `robust_extraction-0.1.5/pyproject.toml` & `robust_extraction-0.1.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "robust-extraction"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Automatic preprocessing of chess scoresheets"
 dependencies = [
-  "ramda", "numpy", "haskellian", "haskellian-either", "haskellian-iterables", "pure-cv", "pydantic",
-  "networkx", "scipy", "opencv-python", "scikit-learn", "py_jaxtyping", "jaxtyping"
+  "ramda", "numpy", "haskellian==0.2.0", "haskellian-either", "haskellian-iterables", "pure-cv", "pydantic",
+  "networkx", "scipy", "opencv-python", "scikit-learn", "py_jaxtyping", "jaxtyping", "lazy-loader"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/REPO.git"
```

### Comparing `robust_extraction-0.1.5/src/robust_extraction/contours/contours.py` & `robust_extraction-0.1.6/src/robust_extraction/contours/contours.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.5/src/robust_extraction/contours/rois.py` & `robust_extraction-0.1.6/src/robust_extraction/contours/rois.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import numpy as np
 import cv2 as cv
 import ramda as R
-from py_jaxtyping import PyArray
-from jaxtyping import Int
-
-Contour = PyArray[Int, int, "4 1 2"]
-Contours = PyArray[Int, int, "N 4 1 2"]
+from .types import Contour, Contours
 
 _1 = int; _2 = int
 @R.curry
 def roi(
     contour: Contour, img: cv.Mat,
     pad_lrtb: tuple[float, float, float, float] = (0, 0, .15, .25)
 ) -> cv.Mat:
@@ -19,9 +15,9 @@
     top = max(int(y - t*h), 0)
     bot = int(y + (1+b)*h)
     left = max(int(x - l*w), 0)
     right = int(x + (1+r)*w)
     return img[top:bot, left:right]
 
 
-def extract(img: cv.Mat, contours: Contours | list[Contour]) -> list[cv.Mat]:
+def extract_contours(img: cv.Mat, contours: Contours | list[Contour]) -> list[cv.Mat]:
     return R.map(roi(img=img), contours)
```

### Comparing `robust_extraction-0.1.5/src/robust_extraction/lines/__init__.py` & `robust_extraction-0.1.6/src/robust_extraction/lines/__init__.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.5/src/robust_extraction/lines/cluster/collinear/clustering.py` & `robust_extraction-0.1.6/src/robust_extraction/lines/cluster/collinear/clustering.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.5/src/robust_extraction/lines/cluster/collinear/metrics.py` & `robust_extraction-0.1.6/src/robust_extraction/lines/cluster/collinear/metrics.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.5/src/robust_extraction/lines/cluster/collinear/segmentation.py` & `robust_extraction-0.1.6/src/robust_extraction/lines/cluster/collinear/segmentation.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.5/src/robust_extraction/lines/cluster/inclination.py` & `robust_extraction-0.1.6/src/robust_extraction/lines/cluster/inclination.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.5/src/robust_extraction/lines/coverage/coverage.py` & `robust_extraction-0.1.6/src/robust_extraction/lines/coverage/coverage.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.5/src/robust_extraction/lines/directions.py` & `robust_extraction-0.1.6/src/robust_extraction/lines/directions.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.5/src/robust_extraction/lines/extract.py` & `robust_extraction-0.1.6/src/robust_extraction/lines/extract.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.5/src/robust_extraction/lines/instersections.py` & `robust_extraction-0.1.6/src/robust_extraction/lines/instersections.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.5/src/robust_extraction/lines/points.py` & `robust_extraction-0.1.6/src/robust_extraction/lines/points.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Literal
 import numpy as np
 import ramda as R
-import haskellian as hk
 from .. import vectors as vec
 
 _1 = int; _2 = int; _4 = int; N = int
 Vec2 = np.ndarray[_2, float]
 
 def pq(line: np.ndarray[_1, _4]) -> tuple[Vec2, Vec2]:
     """Line endpoints (generally refered to as `p` and `q`)"""
```

### Comparing `robust_extraction-0.1.5/src/robust_extraction/lines/poly/intersections.py` & `robust_extraction-0.1.6/src/robust_extraction/lines/poly/intersections.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.5/src/robust_extraction/lines/poly/poly.py` & `robust_extraction-0.1.6/src/robust_extraction/lines/poly/poly.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.5/src/robust_extraction/manual/_extract.py` & `robust_extraction-0.1.6/src/robust_extraction/manual/_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         for y1, y2 in hk.pairwise(rows):
             res += [roi(img, x1, x2, y1, y2)]
             res += [roi(img, x2, x3, y1, y2)]
     return res
             
 Vec2 = tuple[float, float]
 
-def extract(
+def extract_grid(
     img: cv.Mat, top_left: Vec2, size: Vec2, model: ts.SheetModel
 ) -> list[cv.Mat]:
     """Extract boxes from given relative `top_left` and `size` (`[1, 1]` corresponds to the size of `img`)"""
     h, w = img.shape[:2]
     cols = model.cols.imp_points
     rescaled_cols = (cols - cols[0]) / (cols[-1]-cols[0]) * w*size[0] + w*top_left[0]
     block_cols = [rescaled_cols[b:b+3] for b in model.block_cols]
```

### Comparing `robust_extraction-0.1.5/src/robust_extraction/match1d/st_lap.py` & `robust_extraction-0.1.6/src/robust_extraction/match1d/st_lap.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.5/src/robust_extraction/perspective/perspective.py` & `robust_extraction-0.1.6/src/robust_extraction/perspective/perspective.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.5/src/robust_extraction/perspective/perspective2.py` & `robust_extraction-0.1.6/src/robust_extraction/perspective/perspective2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 from typing import NamedTuple, TypedDict
 import cv2 as cv
 import numpy as np
 import pure_cv as vc
 from .. import templates as ts, contours as cs, lines as ls, vectors as vec
-
-Vec2 = tuple[float, float]
-
-class Corners(NamedTuple):
-    tl: Vec2
-    tr: Vec2
-    br: Vec2
-    bl: Vec2
+from .types import Corners
     
 class DetectParams(TypedDict):
     min_height_p: float
     min_width_p: float
     filter_col_coverage: bool
     filter_row_coverage: bool
     min_length_height_p: float
```

### Comparing `robust_extraction-0.1.5/src/robust_extraction/pipeline/ret.py` & `robust_extraction-0.1.6/src/robust_extraction/pipeline/ret.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from py_jaxtyping import PyArray
 from jaxtyping import Int, UInt8
 from ..perspective import Corners
 
 class Ok(BaseModel):
   model_config = ConfigDict(arbitrary_types_allowed=True, extra='forbid')
   contours: PyArray[Int, int, "N 4 1 2"]
-  perspective_corners: Corners
+  perspective_corners: Corners | None
   corr_img: SkipValidation[PyArray[UInt8, int, "H W _"]]
   boxes: list[SkipValidation[PyArray[UInt8, int, "H W _"]]]
 
 @dataclass
 class NotEnoughRows:
   detected: int
   required: int
```

### Comparing `robust_extraction-0.1.5/src/robust_extraction/pipeline/v6.py` & `robust_extraction-0.1.6/src/robust_extraction/pipeline/v6.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.5/src/robust_extraction/pipeline/v7.py` & `robust_extraction-0.1.6/src/robust_extraction/pipeline/v7.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from dataclasses import dataclass
 import haskellian.either as E
 import cv2 as cv
 import numpy as np
 import ramda as R
 import pure_cv as vc
-from .ret import Result, NotEnoughCols, NotEnoughRows, Error, UnkownError, Ok
+from .ret import Result, NotEnoughCols, NotEnoughRows, UnkownError, Ok
 from .. import contours as cs, templates as ts, lines as ls, perspective as pve, match1d
 
-def pipeline7(
+def descaled_extract(
   img: cv.Mat, model: ts.SheetModel,
   min_height_p = 0.8, min_width_p = 0.8,
   filter_row_coverage = True, filter_col_coverage = True,
   verbose = False, auto_h: int | None = 1080, descale_h: int | None = 1920,
   logger = None, autocorrect = True
 ) -> Result:
   """Like `v6` but descaling and rescaling"""
```

### Comparing `robust_extraction-0.1.5/src/robust_extraction/templates/templates.py` & `robust_extraction-0.1.6/src/robust_extraction/templates/templates.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.5/src/robust_extraction.egg-info/PKG-INFO` & `robust_extraction-0.1.6/src/robust_extraction.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: robust-extraction
-Version: 0.1.5
+Version: 0.1.6
 Summary: Automatic preprocessing of chess scoresheets
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ramda
 Requires-Dist: numpy
-Requires-Dist: haskellian
+Requires-Dist: haskellian==0.2.0
 Requires-Dist: haskellian-either
 Requires-Dist: haskellian-iterables
 Requires-Dist: pure-cv
 Requires-Dist: pydantic
 Requires-Dist: networkx
 Requires-Dist: scipy
 Requires-Dist: opencv-python
 Requires-Dist: scikit-learn
 Requires-Dist: py_jaxtyping
 Requires-Dist: jaxtyping
+Requires-Dist: lazy-loader
 
 # Robust Extraction
 
 > Automatic preprocessing of chess scoresheets
```

### Comparing `robust_extraction-0.1.5/src/robust_extraction.egg-info/SOURCES.txt` & `robust_extraction-0.1.6/src/robust_extraction.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 README.md
 pyproject.toml
 src/robust_extraction/__init__.py
+src/robust_extraction/__init__.pyi
 src/robust_extraction.egg-info/PKG-INFO
 src/robust_extraction.egg-info/SOURCES.txt
 src/robust_extraction.egg-info/dependency_links.txt
 src/robust_extraction.egg-info/requires.txt
 src/robust_extraction.egg-info/top_level.txt
 src/robust_extraction/contours/__init__.py
+src/robust_extraction/contours/__init__.pyi
 src/robust_extraction/contours/contours.py
 src/robust_extraction/contours/rois.py
+src/robust_extraction/contours/types.py
 src/robust_extraction/lines/__init__.py
 src/robust_extraction/lines/directions.py
 src/robust_extraction/lines/extract.py
 src/robust_extraction/lines/instersections.py
 src/robust_extraction/lines/points.py
 src/robust_extraction/lines/cluster/__init__.py
 src/robust_extraction/lines/cluster/inclination.py
@@ -29,16 +32,18 @@
 src/robust_extraction/lines/poly/poly.py
 src/robust_extraction/manual/__init__.py
 src/robust_extraction/manual/_correct.py
 src/robust_extraction/manual/_extract.py
 src/robust_extraction/match1d/__init__.py
 src/robust_extraction/match1d/st_lap.py
 src/robust_extraction/perspective/__init__.py
+src/robust_extraction/perspective/__init__.pyi
 src/robust_extraction/perspective/perspective.py
 src/robust_extraction/perspective/perspective2.py
+src/robust_extraction/perspective/types.py
 src/robust_extraction/pipeline/__init__.py
 src/robust_extraction/pipeline/ret.py
 src/robust_extraction/pipeline/v6.py
 src/robust_extraction/pipeline/v7.py
 src/robust_extraction/templates/__init__.py
 src/robust_extraction/templates/templates.py
 src/robust_extraction/templates/_models/__init__.py
```


# Comparing `tmp/cityscapesScripts-2.2.2.tar.gz` & `tmp/cityscapesscripts-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cityscapesScripts-2.2.2.tar", last modified: Sun May  7 12:21:16 2023, max compression
+gzip compressed data, was "cityscapesscripts-2.2.3.tar", last modified: Sun Apr 21 11:54:29 2024, max compression
```

## Comparing `cityscapesScripts-2.2.2.tar` & `cityscapesscripts-2.2.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.138107 cityscapesScripts-2.2.2/
--rw-r--r--   0 mcordts    (501) staff       (20)     1082 2022-10-21 15:36:58.000000 cityscapesScripts-2.2.2/LICENSE
--rw-r--r--   0 mcordts    (501) staff       (20)     9564 2023-05-07 12:21:16.138365 cityscapesScripts-2.2.2/PKG-INFO
--rw-r--r--   0 mcordts    (501) staff       (20)     9182 2022-10-21 15:37:54.000000 cityscapesScripts-2.2.2/README.md
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.028571 cityscapesScripts-2.2.2/cityscapesScripts.egg-info/
--rw-r--r--   0 mcordts    (501) staff       (20)     9564 2023-05-07 12:21:15.000000 cityscapesScripts-2.2.2/cityscapesScripts.egg-info/PKG-INFO
--rw-r--r--   0 mcordts    (501) staff       (20)     3425 2023-05-07 12:21:15.000000 cityscapesScripts-2.2.2/cityscapesScripts.egg-info/SOURCES.txt
--rw-r--r--   0 mcordts    (501) staff       (20)        1 2023-05-07 12:21:15.000000 cityscapesScripts-2.2.2/cityscapesScripts.egg-info/dependency_links.txt
--rw-r--r--   0 mcordts    (501) staff       (20)      939 2023-05-07 12:21:15.000000 cityscapesScripts-2.2.2/cityscapesScripts.egg-info/entry_points.txt
--rw-r--r--   0 mcordts    (501) staff       (20)       82 2023-05-07 12:21:15.000000 cityscapesScripts-2.2.2/cityscapesScripts.egg-info/requires.txt
--rw-r--r--   0 mcordts    (501) staff       (20)       18 2023-05-07 12:21:15.000000 cityscapesScripts-2.2.2/cityscapesScripts.egg-info/top_level.txt
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.029780 cityscapesScripts-2.2.2/cityscapesscripts/
--rw-r--r--   0 mcordts    (501) staff       (20)        6 2023-05-07 12:19:22.000000 cityscapesScripts-2.2.2/cityscapesscripts/VERSION
--rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/__init__.py
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.030603 cityscapesScripts-2.2.2/cityscapesscripts/annotation/
--rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/__init__.py
--rw-r--r--   0 mcordts    (501) staff       (20)   110764 2020-08-29 16:30:00.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/cityscapesLabelTool.py
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.098692 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/
--rw-r--r--   0 mcordts    (501) staff       (20)     6124 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/back.png
--rw-r--r--   0 mcordts    (501) staff       (20)    12493 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/checked6.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/checked6_red.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/clearpolygon.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/deleteobject.png
--rw-r--r--   0 mcordts    (501) staff       (20)     3391 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/exit.png
--rw-r--r--   0 mcordts    (501) staff       (20)    14178 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/filepath.png
--rw-r--r--   0 mcordts    (501) staff       (20)    13163 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/help19.png
--rw-r--r--   0 mcordts    (501) staff       (20)    11772 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/highlight.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/layerdown.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/layerup.png
--rw-r--r--   0 mcordts    (501) staff       (20)     2355 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/minus.png
--rw-r--r--   0 mcordts    (501) staff       (20)     9477 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/modify.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/newobject.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/next.png
--rw-r--r--   0 mcordts    (501) staff       (20)     4992 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/open.png
--rw-r--r--   0 mcordts    (501) staff       (20)    10655 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/play.png
--rw-r--r--   0 mcordts    (501) staff       (20)     4004 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/plus.png
--rw-r--r--   0 mcordts    (501) staff       (20)     2739 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/save.png
--rw-r--r--   0 mcordts    (501) staff       (20)     9938 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/screenshot.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/screenshotToggle.png
--rw-r--r--   0 mcordts    (501) staff       (20)     6454 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/shuffle.png
--rw-r--r--   0 mcordts    (501) staff       (20)     5765 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/undo.png
--rw-r--r--   0 mcordts    (501) staff       (20)    12237 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/zoom.png
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.100647 cityscapesScripts-2.2.2/cityscapesscripts/download/
--rw-r--r--   0 mcordts    (501) staff       (20)        1 2020-02-26 20:37:16.000000 cityscapesScripts-2.2.2/cityscapesscripts/download/__init__.py
--rw-r--r--   0 mcordts    (501) staff       (20)     5931 2020-05-31 12:37:37.000000 cityscapesScripts-2.2.2/cityscapesscripts/download/downloader.py
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.108624 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/
--rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/__init__.py
--rw-r--r--   0 mcordts    (501) staff       (20)    30171 2023-05-07 12:19:22.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/evalInstanceLevelSemanticLabeling.py
--rw-r--r--   0 mcordts    (501) staff       (20)    49118 2020-10-17 11:45:02.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/evalObjectDetection3D.py
--rw-r--r--   0 mcordts    (501) staff       (20)    15701 2021-01-11 19:50:04.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/evalPanopticSemanticLabeling.py
--rw-r--r--   0 mcordts    (501) staff       (20)    28237 2020-02-16 07:50:37.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/evalPixelLevelSemanticLabeling.py
--rw-r--r--   0 mcordts    (501) staff       (20)     1441 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/instance.py
--rw-r--r--   0 mcordts    (501) staff       (20)     1613 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/instances2dict.py
--rw-r--r--   0 mcordts    (501) staff       (20)     4963 2020-10-17 08:52:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/objectDetectionHelpers.py
--rw-r--r--   0 mcordts    (501) staff       (20)    17475 2020-09-26 16:51:47.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/plot3DResults.py
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.117740 cityscapesScripts-2.2.2/cityscapesscripts/helpers/
--rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/helpers/__init__.py
--rw-r--r--   0 mcordts    (501) staff       (20)    14057 2020-10-17 11:45:02.000000 cityscapesScripts-2.2.2/cityscapesscripts/helpers/annotation.py
--rw-r--r--   0 mcordts    (501) staff       (20)    15536 2020-10-02 17:58:21.000000 cityscapesScripts-2.2.2/cityscapesscripts/helpers/box3dImageTransform.py
--rw-r--r--   0 mcordts    (501) staff       (20)     3506 2020-08-29 16:30:00.000000 cityscapesScripts-2.2.2/cityscapesscripts/helpers/csHelpers.py
--rw-r--r--   0 mcordts    (501) staff       (20)    10663 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/helpers/labels.py
--rw-r--r--   0 mcordts    (501) staff       (20)     2550 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/helpers/labels_cityPersons.py
--rw-r--r--   0 mcordts    (501) staff       (20)      186 2020-08-29 16:30:00.000000 cityscapesScripts-2.2.2/cityscapesscripts/helpers/version.py
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.122834 cityscapesScripts-2.2.2/cityscapesscripts/preparation/
--rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/preparation/__init__.py
--rw-r--r--   0 mcordts    (501) staff       (20)     7428 2021-01-11 19:50:04.000000 cityscapesScripts-2.2.2/cityscapesscripts/preparation/createPanopticImgs.py
--rw-r--r--   0 mcordts    (501) staff       (20)     2926 2020-01-19 19:22:15.000000 cityscapesScripts-2.2.2/cityscapesscripts/preparation/createTrainIdInstanceImgs.py
--rw-r--r--   0 mcordts    (501) staff       (20)     2757 2020-01-19 19:22:15.000000 cityscapesScripts-2.2.2/cityscapesscripts/preparation/createTrainIdLabelImgs.py
--rw-r--r--   0 mcordts    (501) staff       (20)     7247 2020-01-19 19:22:15.000000 cityscapesScripts-2.2.2/cityscapesscripts/preparation/json2instanceImg.py
--rw-r--r--   0 mcordts    (501) staff       (20)     5069 2020-01-19 19:22:15.000000 cityscapesScripts-2.2.2/cityscapesscripts/preparation/json2labelImg.py
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.124060 cityscapesScripts-2.2.2/cityscapesscripts/viewer/
--rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/__init__.py
--rw-r--r--   0 mcordts    (501) staff       (20)    55045 2020-08-29 16:30:00.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/cityscapesViewer.py
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.137388 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/
--rw-r--r--   0 mcordts    (501) staff       (20)     6124 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/back.png
--rw-r--r--   0 mcordts    (501) staff       (20)     7530 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/disp.png
--rw-r--r--   0 mcordts    (501) staff       (20)     3391 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/exit.png
--rw-r--r--   0 mcordts    (501) staff       (20)    14178 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/filepath.png
--rw-r--r--   0 mcordts    (501) staff       (20)    13163 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/help19.png
--rw-r--r--   0 mcordts    (501) staff       (20)    13349 2020-08-29 16:30:00.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/label.png
--rw-r--r--   0 mcordts    (501) staff       (20)     2355 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/minus.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/next.png
--rw-r--r--   0 mcordts    (501) staff       (20)     4992 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/open.png
--rw-r--r--   0 mcordts    (501) staff       (20)    10655 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/play.png
--rw-r--r--   0 mcordts    (501) staff       (20)     4004 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/plus.png
--rw-r--r--   0 mcordts    (501) staff       (20)     6454 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/shuffle.png
--rw-r--r--   0 mcordts    (501) staff       (20)    12237 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/zoom.png
--rw-r--r--   0 mcordts    (501) staff       (20)       79 2023-05-07 12:21:16.139241 cityscapesScripts-2.2.2/setup.cfg
--rw-r--r--   0 mcordts    (501) staff       (20)     2889 2022-10-21 15:37:16.000000 cityscapesScripts-2.2.2/setup.py
+drwxr-xr-x   0 mcordts  (1074121050) 58041779        0 2024-04-21 11:54:29.698787 cityscapesscripts-2.2.3/
+-rw-r--r--   0 mcordts  (1074121050) 58041779     1082 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/LICENSE
+-rw-r--r--   0 mcordts  (1074121050) 58041779     9834 2024-04-21 11:54:29.698576 cityscapesscripts-2.2.3/PKG-INFO
+-rw-r--r--   0 mcordts  (1074121050) 58041779     9182 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/README.md
+drwxr-xr-x   0 mcordts  (1074121050) 58041779        0 2024-04-21 11:54:29.698250 cityscapesscripts-2.2.3/cityscapesScripts.egg-info/
+-rw-r--r--   0 mcordts  (1074121050) 58041779     9834 2024-04-21 11:54:29.000000 cityscapesscripts-2.2.3/cityscapesScripts.egg-info/PKG-INFO
+-rw-r--r--   0 mcordts  (1074121050) 58041779     3325 2024-04-21 11:54:29.000000 cityscapesscripts-2.2.3/cityscapesScripts.egg-info/SOURCES.txt
+-rw-r--r--   0 mcordts  (1074121050) 58041779        1 2024-04-21 11:54:29.000000 cityscapesscripts-2.2.3/cityscapesScripts.egg-info/dependency_links.txt
+-rw-r--r--   0 mcordts  (1074121050) 58041779      939 2024-04-21 11:54:29.000000 cityscapesscripts-2.2.3/cityscapesScripts.egg-info/entry_points.txt
+-rw-r--r--   0 mcordts  (1074121050) 58041779       96 2024-04-21 11:54:29.000000 cityscapesscripts-2.2.3/cityscapesScripts.egg-info/requires.txt
+-rw-r--r--   0 mcordts  (1074121050) 58041779       18 2024-04-21 11:54:29.000000 cityscapesscripts-2.2.3/cityscapesScripts.egg-info/top_level.txt
+drwxr-xr-x   0 mcordts  (1074121050) 58041779        0 2024-04-21 11:54:29.678754 cityscapesscripts-2.2.3/cityscapesscripts/
+-rw-r--r--   0 mcordts  (1074121050) 58041779        6 2024-04-21 11:45:57.000000 cityscapesscripts-2.2.3/cityscapesscripts/VERSION
+-rw-r--r--   0 mcordts  (1074121050) 58041779        0 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/__init__.py
+drwxr-xr-x   0 mcordts  (1074121050) 58041779        0 2024-04-21 11:54:29.678988 cityscapesscripts-2.2.3/cityscapesscripts/annotation/
+-rw-r--r--   0 mcordts  (1074121050) 58041779        0 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/__init__.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779   110764 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/cityscapesLabelTool.py
+drwxr-xr-x   0 mcordts  (1074121050) 58041779        0 2024-04-21 11:54:29.689576 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/
+-rw-r--r--   0 mcordts  (1074121050) 58041779     6124 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/back.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779    12493 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/checked6.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779  1050910 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/checked6_red.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779  1050910 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/clearpolygon.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779  1050910 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/deleteobject.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779     3391 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/exit.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779    14178 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/filepath.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779    13163 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/help19.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779    11772 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/highlight.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779  1050910 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/layerdown.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779  1050910 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/layerup.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779     2355 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/minus.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779     9477 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/modify.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779  1050910 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/newobject.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779  1050910 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/next.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779     4992 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/open.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779    10655 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/play.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779     4004 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/plus.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779     2739 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/save.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779     9938 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/screenshot.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779  1050910 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/screenshotToggle.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779     6454 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/shuffle.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779     5765 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/undo.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779    12237 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/zoom.png
+drwxr-xr-x   0 mcordts  (1074121050) 58041779        0 2024-04-21 11:54:29.691284 cityscapesscripts-2.2.3/cityscapesscripts/download/
+-rw-r--r--   0 mcordts  (1074121050) 58041779        1 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/download/__init__.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779     6990 2024-04-21 11:45:57.000000 cityscapesscripts-2.2.3/cityscapesscripts/download/downloader.py
+drwxr-xr-x   0 mcordts  (1074121050) 58041779        0 2024-04-21 11:54:29.692873 cityscapesscripts-2.2.3/cityscapesscripts/evaluation/
+-rw-r--r--   0 mcordts  (1074121050) 58041779        0 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/evaluation/__init__.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779    30171 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/evaluation/evalInstanceLevelSemanticLabeling.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779    49118 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/evaluation/evalObjectDetection3d.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779    15701 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/evaluation/evalPanopticSemanticLabeling.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779    28237 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/evaluation/evalPixelLevelSemanticLabeling.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779     1441 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/evaluation/instance.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779     1613 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/evaluation/instances2dict.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779     4963 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/evaluation/objectDetectionHelpers.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779    17475 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/evaluation/plot3dResults.py
+drwxr-xr-x   0 mcordts  (1074121050) 58041779        0 2024-04-21 11:54:29.694092 cityscapesscripts-2.2.3/cityscapesscripts/helpers/
+-rw-r--r--   0 mcordts  (1074121050) 58041779        0 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/helpers/__init__.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779    14057 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/helpers/annotation.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779    15536 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/helpers/box3dImageTransform.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779     3506 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/helpers/csHelpers.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779    10663 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/helpers/labels.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779     2550 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/helpers/labels_cityPersons.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779      186 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/helpers/version.py
+drwxr-xr-x   0 mcordts  (1074121050) 58041779        0 2024-04-21 11:54:29.695019 cityscapesscripts-2.2.3/cityscapesscripts/preparation/
+-rw-r--r--   0 mcordts  (1074121050) 58041779        0 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/preparation/__init__.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779     7428 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/preparation/createPanopticImgs.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779     2926 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/preparation/createTrainIdInstanceImgs.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779     2757 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/preparation/createTrainIdLabelImgs.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779     7247 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/preparation/json2instanceImg.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779     5069 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/preparation/json2labelImg.py
+drwxr-xr-x   0 mcordts  (1074121050) 58041779        0 2024-04-21 11:54:29.695324 cityscapesscripts-2.2.3/cityscapesscripts/viewer/
+-rw-r--r--   0 mcordts  (1074121050) 58041779        0 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/viewer/__init__.py
+-rw-r--r--   0 mcordts  (1074121050) 58041779    55045 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/viewer/cityscapesViewer.py
+drwxr-xr-x   0 mcordts  (1074121050) 58041779        0 2024-04-21 11:54:29.697857 cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/
+-rw-r--r--   0 mcordts  (1074121050) 58041779     6124 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/back.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779     7530 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/disp.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779     3391 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/exit.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779    14178 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/filepath.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779    13163 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/help19.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779    13349 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/label.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779     2355 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/minus.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779  1050910 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/next.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779     4992 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/open.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779    10655 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/play.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779     4004 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/plus.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779     6454 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/shuffle.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779    12237 2023-12-23 07:58:19.000000 cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/zoom.png
+-rw-r--r--   0 mcordts  (1074121050) 58041779       79 2024-04-21 11:54:29.698977 cityscapesscripts-2.2.3/setup.cfg
+-rw-r--r--   0 mcordts  (1074121050) 58041779     2909 2024-04-21 11:45:57.000000 cityscapesscripts-2.2.3/setup.py
```

### Comparing `cityscapesScripts-2.2.2/LICENSE` & `cityscapesscripts-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/PKG-INFO` & `cityscapesscripts-2.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: cityscapesScripts
-Version: 2.2.2
-Summary: Scripts for the Cityscapes Dataset
-Home-page: https://github.com/mcordts/cityscapesScripts
-Author: Marius Cordts
-Author-email: mail@cityscapes-dataset.net
-License: https://github.com/mcordts/cityscapesScripts/blob/master/LICENSE
-Description-Content-Type: text/markdown
-Provides-Extra: gui
-License-File: LICENSE
-
 # The Cityscapes Dataset
 
 This repository contains scripts for inspection, preparation, and evaluation of the Cityscapes dataset. This large-scale dataset contains a diverse set of stereo video sequences recorded in street scenes from 50 different cities, with high quality pixel-level annotations of 5 000 frames in addition to a larger set of 20 000 weakly annotated frames.
 
 Details and download are available at: www.cityscapes-dataset.com
```

### Comparing `cityscapesScripts-2.2.2/README.md` & `cityscapesscripts-2.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: cityscapesScripts
+Version: 2.2.3
+Summary: Scripts for the Cityscapes Dataset
+Home-page: https://github.com/mcordts/cityscapesScripts
+Author: Marius Cordts
+Author-email: mail@cityscapes-dataset.net
+License: https://github.com/mcordts/cityscapesScripts/blob/master/LICENSE
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: pillow
+Requires-Dist: appdirs
+Requires-Dist: pyquaternion
+Requires-Dist: coloredlogs
+Requires-Dist: tqdm
+Requires-Dist: typing
+Requires-Dist: requests
+Requires-Dist: tqdm
+Provides-Extra: gui
+Requires-Dist: PyQt5; extra == "gui"
+
 # The Cityscapes Dataset
 
 This repository contains scripts for inspection, preparation, and evaluation of the Cityscapes dataset. This large-scale dataset contains a diverse set of stereo video sequences recorded in street scenes from 50 different cities, with high quality pixel-level annotations of 5 000 frames in addition to a larger set of 20 000 weakly annotated frames.
 
 Details and download are available at: www.cityscapes-dataset.com
```

### Comparing `cityscapesScripts-2.2.2/cityscapesScripts.egg-info/PKG-INFO` & `cityscapesscripts-2.2.3/cityscapesScripts.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 Metadata-Version: 2.1
 Name: cityscapesScripts
-Version: 2.2.2
+Version: 2.2.3
 Summary: Scripts for the Cityscapes Dataset
 Home-page: https://github.com/mcordts/cityscapesScripts
 Author: Marius Cordts
 Author-email: mail@cityscapes-dataset.net
 License: https://github.com/mcordts/cityscapesScripts/blob/master/LICENSE
 Description-Content-Type: text/markdown
-Provides-Extra: gui
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: pillow
+Requires-Dist: appdirs
+Requires-Dist: pyquaternion
+Requires-Dist: coloredlogs
+Requires-Dist: tqdm
+Requires-Dist: typing
+Requires-Dist: requests
+Requires-Dist: tqdm
+Provides-Extra: gui
+Requires-Dist: PyQt5; extra == "gui"
 
 # The Cityscapes Dataset
 
 This repository contains scripts for inspection, preparation, and evaluation of the Cityscapes dataset. This large-scale dataset contains a diverse set of stereo video sequences recorded in street scenes from 50 different cities, with high quality pixel-level annotations of 5 000 frames in addition to a larger set of 20 000 weakly annotated frames.
 
 Details and download are available at: www.cityscapes-dataset.com
```

### Comparing `cityscapesScripts-2.2.2/cityscapesScripts.egg-info/SOURCES.txt` & `cityscapesscripts-2.2.3/cityscapesScripts.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,22 +36,20 @@
 cityscapesscripts/annotation/icons/shuffle.png
 cityscapesscripts/annotation/icons/undo.png
 cityscapesscripts/annotation/icons/zoom.png
 cityscapesscripts/download/__init__.py
 cityscapesscripts/download/downloader.py
 cityscapesscripts/evaluation/__init__.py
 cityscapesscripts/evaluation/evalInstanceLevelSemanticLabeling.py
-cityscapesscripts/evaluation/evalObjectDetection3D.py
 cityscapesscripts/evaluation/evalObjectDetection3d.py
 cityscapesscripts/evaluation/evalPanopticSemanticLabeling.py
 cityscapesscripts/evaluation/evalPixelLevelSemanticLabeling.py
 cityscapesscripts/evaluation/instance.py
 cityscapesscripts/evaluation/instances2dict.py
 cityscapesscripts/evaluation/objectDetectionHelpers.py
-cityscapesscripts/evaluation/plot3DResults.py
 cityscapesscripts/evaluation/plot3dResults.py
 cityscapesscripts/helpers/__init__.py
 cityscapesscripts/helpers/annotation.py
 cityscapesscripts/helpers/box3dImageTransform.py
 cityscapesscripts/helpers/csHelpers.py
 cityscapesscripts/helpers/labels.py
 cityscapesscripts/helpers/labels_cityPersons.py
```

### Comparing `cityscapesScripts-2.2.2/cityscapesScripts.egg-info/entry_points.txt` & `cityscapesscripts-2.2.3/cityscapesScripts.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/cityscapesLabelTool.py` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/cityscapesLabelTool.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/back.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/back.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/checked6.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/checked6.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/checked6_red.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/checked6_red.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/clearpolygon.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/clearpolygon.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/deleteobject.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/deleteobject.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/exit.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/exit.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/filepath.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/filepath.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/help19.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/help19.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/highlight.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/highlight.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/layerdown.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/layerdown.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/layerup.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/layerup.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/minus.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/minus.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/modify.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/modify.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/newobject.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/newobject.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/next.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/next.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/open.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/open.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/play.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/play.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/plus.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/plus.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/save.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/save.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/screenshot.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/screenshot.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/screenshotToggle.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/screenshotToggle.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/shuffle.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/shuffle.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/undo.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/undo.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/zoom.png` & `cityscapesscripts-2.2.3/cityscapesscripts/annotation/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/download/downloader.py` & `cityscapesscripts-2.2.3/cityscapesscripts/download/downloader.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import getpass
 import hashlib
 import json
 import os
 import requests
 import shutil
 import stat
+from tqdm import tqdm
 
 from builtins import input
 
 
 def login():
     appname = __name__.split('.')[0]
     appauthor = 'cityscapes'
@@ -75,21 +76,36 @@
     for p in packages:
         info = ' {} -> {}'.format(p['name'], p['size'])
         if p['thirdparty'] == '1':
             info += " (third party)"
         print(info)
 
 
+def parse_size_to_bytes(size_str):
+    size_str = size_str.upper()
+    if size_str.endswith("KB"):
+        size_bytes = float(size_str[:-2]) * 1024
+    elif size_str.endswith("MB"):
+        size_bytes = float(size_str[:-2]) * 1024 * 1024
+    elif size_str.endswith("GB"):
+        size_bytes = float(size_str[:-2]) * 1024 * 1024 * 1024
+    else:
+        raise ValueError("Invalid size format. Use 'KB', 'MB', or 'GB'.")
+
+    return size_bytes
+
+
 def download_packages(*, session, package_names, destination_path, resume=False):
     if not os.path.isdir(destination_path):
         raise Exception(
             "Destination path '{}' does not exist.".format(destination_path))
 
     packages = get_available_packages(session=session)
     name_to_id = {p['name']: p['packageID'] for p in packages}
+    name_to_bytes = {p['name']: parse_size_to_bytes(p['size']) for p in packages}
     invalid_names = [n for n in package_names if n not in name_to_id]
     if invalid_names:
         raise Exception(
             "These packages do not exist or you don't have access: {}".format(invalid_names))
 
     for package_name in package_names:
         local_filename = os.path.join(destination_path, package_name)
@@ -118,15 +134,26 @@
         with open(local_filename, 'ab' if resume else 'wb') as f:
             resume_header = {
                 'Range': 'bytes={}-'.format(f.tell())} if resume else {}
             with session.get(url, allow_redirects=False, stream=True, headers=resume_header) as r:
                 r.raise_for_status()
                 assert r.status_code in [200, 206]
 
-                shutil.copyfileobj(r.raw, f)
+                # progress bar
+                with tqdm(desc="Download progress",
+                          total=name_to_bytes[package_name],
+                          miniters=1,
+                          unit='B',
+                          unit_scale=True,
+                          unit_divisor=1024,
+                          initial=f.tell() if resume else 0
+                          ) as pbar:
+                    for chunk in r.iter_content(chunk_size=1024):
+                        f.write(chunk)
+                        pbar.update(len(chunk))
 
         # verify md5sum
         hash_md5 = hashlib.md5()
         with open(local_filename, "rb") as f:
             for chunk in iter(lambda: f.read(4096), b""):
                 hash_md5.update(chunk)
         if md5sum != hash_md5.hexdigest():
```

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/evaluation/evalInstanceLevelSemanticLabeling.py` & `cityscapesscripts-2.2.3/cityscapesscripts/evaluation/evalInstanceLevelSemanticLabeling.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/evaluation/evalObjectDetection3D.py` & `cityscapesscripts-2.2.3/cityscapesscripts/evaluation/evalObjectDetection3d.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/evaluation/evalPanopticSemanticLabeling.py` & `cityscapesscripts-2.2.3/cityscapesscripts/evaluation/evalPanopticSemanticLabeling.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/evaluation/evalPixelLevelSemanticLabeling.py` & `cityscapesscripts-2.2.3/cityscapesscripts/evaluation/evalPixelLevelSemanticLabeling.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/evaluation/instance.py` & `cityscapesscripts-2.2.3/cityscapesscripts/evaluation/instance.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/evaluation/instances2dict.py` & `cityscapesscripts-2.2.3/cityscapesscripts/evaluation/instances2dict.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/evaluation/objectDetectionHelpers.py` & `cityscapesscripts-2.2.3/cityscapesscripts/evaluation/objectDetectionHelpers.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/evaluation/plot3DResults.py` & `cityscapesscripts-2.2.3/cityscapesscripts/evaluation/plot3dResults.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/helpers/annotation.py` & `cityscapesscripts-2.2.3/cityscapesscripts/helpers/annotation.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/helpers/box3dImageTransform.py` & `cityscapesscripts-2.2.3/cityscapesscripts/helpers/box3dImageTransform.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/helpers/csHelpers.py` & `cityscapesscripts-2.2.3/cityscapesscripts/helpers/csHelpers.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/helpers/labels.py` & `cityscapesscripts-2.2.3/cityscapesscripts/helpers/labels.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/helpers/labels_cityPersons.py` & `cityscapesscripts-2.2.3/cityscapesscripts/helpers/labels_cityPersons.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/preparation/createPanopticImgs.py` & `cityscapesscripts-2.2.3/cityscapesscripts/preparation/createPanopticImgs.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/preparation/createTrainIdInstanceImgs.py` & `cityscapesscripts-2.2.3/cityscapesscripts/preparation/createTrainIdInstanceImgs.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/preparation/createTrainIdLabelImgs.py` & `cityscapesscripts-2.2.3/cityscapesscripts/preparation/createTrainIdLabelImgs.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/preparation/json2instanceImg.py` & `cityscapesscripts-2.2.3/cityscapesscripts/preparation/json2instanceImg.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/preparation/json2labelImg.py` & `cityscapesscripts-2.2.3/cityscapesscripts/preparation/json2labelImg.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/viewer/cityscapesViewer.py` & `cityscapesscripts-2.2.3/cityscapesscripts/viewer/cityscapesViewer.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/back.png` & `cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/back.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/disp.png` & `cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/disp.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/exit.png` & `cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/exit.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/filepath.png` & `cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/filepath.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/help19.png` & `cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/help19.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/label.png` & `cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/label.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/minus.png` & `cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/minus.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/next.png` & `cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/next.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/open.png` & `cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/open.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/play.png` & `cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/play.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/plus.png` & `cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/plus.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/shuffle.png` & `cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/shuffle.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/zoom.png` & `cityscapesscripts-2.2.3/cityscapesscripts/viewer/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.2/setup.py` & `cityscapesscripts-2.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     'long_description': readme,
     'long_description_content_type': "text/markdown",
     'author': 'Marius Cordts',
     'url': 'https://github.com/mcordts/cityscapesScripts',
     'author_email': 'mail@cityscapes-dataset.net',
     'license': 'https://github.com/mcordts/cityscapesScripts/blob/master/LICENSE',
     'version': version,
-    'install_requires': ['numpy', 'matplotlib', 'pillow', 'appdirs', 'pyquaternion', 'coloredlogs', 'tqdm', 'typing'],
+    'install_requires': ['numpy', 'matplotlib', 'pillow', 'appdirs', 'pyquaternion', 'coloredlogs', 'tqdm', 'typing', 'requests', 'tqdm'],
     'setup_requires': ['setuptools>=18.0'],
     'extras_require': {
         'gui': ['PyQt5']
     },
     'packages': find_packages(),
     'scripts': [],
     'entry_points': {'gui_scripts': gui_scripts,
```


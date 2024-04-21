# Comparing `tmp/misleep-0.2.2b0.tar.gz` & `tmp/misleep-0.2.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misleep-0.2.2b0.tar", last modified: Wed Apr 17 11:29:29 2024, max compression
+gzip compressed data, was "misleep-0.2.3b0.tar", last modified: Sun Apr 21 09:38:41 2024, max compression
```

## Comparing `misleep-0.2.2b0.tar` & `misleep-0.2.3b0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.847330 misleep-0.2.2b0/
--rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.2.2b0/LICENSE
--rw-rw-rw-   0        0        0     2969 2024-04-17 11:29:29.847330 misleep-0.2.2b0/PKG-INFO
--rw-rw-rw-   0        0        0     1871 2024-04-17 11:10:21.000000 misleep-0.2.2b0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.823330 misleep-0.2.2b0/misleep/
--rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.2.2b0/misleep/__init__.py
--rw-rw-rw-   0        0        0      167 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/__main__.py
--rw-rw-rw-   0        0        0      532 2024-04-17 11:26:31.000000 misleep-0.2.2b0/misleep/config.ini
-drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.829330 misleep-0.2.2b0/misleep/gui/
--rw-rw-rw-   0        0        0      334 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/gui/__init__.py
--rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.2.2b0/misleep/gui/about.py
--rw-rw-rw-   0        0        0     7443 2024-04-17 11:26:19.000000 misleep-0.2.2b0/misleep/gui/dialog.py
--rw-rw-rw-   0        0        0    56484 2024-04-17 11:23:33.000000 misleep-0.2.2b0/misleep/gui/main_window.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.833331 misleep-0.2.2b0/misleep/gui/resources/
--rw-rw-rw-   0        0        0       47 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/gui/resources/__init__.py
--rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.2.2b0/misleep/gui/resources/entire_logo.png
--rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.2.2b0/misleep/gui/resources/logo.png
--rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.2.2b0/misleep/gui/resources/misleep.py
--rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.2.2b0/misleep/gui/resources/misleep.qrc
--rw-rw-rw-   0        0        0      476 2024-04-15 10:19:04.000000 misleep-0.2.2b0/misleep/gui/show.py
--rw-rw-rw-   0        0        0     5893 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/gui/spec_window.py
--rw-rw-rw-   0        0        0     3177 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/gui/thread.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.837331 misleep-0.2.2b0/misleep/gui/uis/
--rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.2.2b0/misleep/gui/uis/__init__.py
--rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.2.2b0/misleep/gui/uis/about_ui.py
--rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.2.2b0/misleep/gui/uis/label_dialog_ui.py
--rw-rw-rw-   0        0        0    24912 2024-04-17 03:11:18.000000 misleep-0.2.2b0/misleep/gui/uis/main_window_ui.py
--rw-rw-rw-   0        0        0     2371 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/gui/uis/save_data_dialog_ui.py
--rw-rw-rw-   0        0        0     4466 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/gui/uis/spec_window_ui.py
--rw-rw-rw-   0        0        0     4884 2024-04-17 11:15:15.000000 misleep-0.2.2b0/misleep/gui/uis/transfer_result_dialog_ui.py
--rw-rw-rw-   0        0        0     3441 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/gui/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.838330 misleep-0.2.2b0/misleep/io/
--rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.2.2b0/misleep/io/__init__.py
--rw-rw-rw-   0        0        0     6268 2024-04-15 11:24:05.000000 misleep-0.2.2b0/misleep/io/annotation_io.py
--rw-rw-rw-   0        0        0    14995 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/io/base.py
--rw-rw-rw-   0        0        0     5027 2024-04-17 08:38:52.000000 misleep-0.2.2b0/misleep/io/signal_io.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.840331 misleep-0.2.2b0/misleep/preprocessing/
--rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.2.2b0/misleep/preprocessing/__init__.py
--rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.2.2b0/misleep/preprocessing/channel.py
--rw-rw-rw-   0        0        0      458 2024-04-15 10:35:14.000000 misleep-0.2.2b0/misleep/preprocessing/signals.py
--rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.2.2b0/misleep/preprocessing/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.842331 misleep-0.2.2b0/misleep/utils/
--rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.2.2b0/misleep/utils/__init__.py
--rw-rw-rw-   0        0        0     4394 2024-04-15 03:11:05.000000 misleep-0.2.2b0/misleep/utils/annotation.py
--rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.2.2b0/misleep/utils/signals.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.843331 misleep-0.2.2b0/misleep/viz/
--rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.2.2b0/misleep/viz/__init__.py
--rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.2.2b0/misleep/viz/hypnogram.py
--rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.2.2b0/misleep/viz/signals.py
--rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.2.2b0/misleep/viz/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.826331 misleep-0.2.2b0/misleep.egg-info/
--rw-rw-rw-   0        0        0     2969 2024-04-17 11:29:29.000000 misleep-0.2.2b0/misleep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1401 2024-04-17 11:29:29.000000 misleep-0.2.2b0/misleep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 11:29:29.000000 misleep-0.2.2b0/misleep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-17 11:29:29.000000 misleep-0.2.2b0/misleep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-17 11:29:29.000000 misleep-0.2.2b0/misleep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 11:29:29.847330 misleep-0.2.2b0/setup.cfg
--rw-rw-rw-   0        0        0     2154 2024-04-17 11:11:27.000000 misleep-0.2.2b0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:29:29.846331 misleep-0.2.2b0/test/
--rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.2.2b0/test/test_annotation_io.py
--rw-rw-rw-   0        0        0      143 2024-04-15 03:11:05.000000 misleep-0.2.2b0/test/test_loadmat73.py
--rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.2.2b0/test/test_midata.py
--rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.2.2b0/test/test_show.py
--rw-rw-rw-   0        0        0     1488 2024-04-15 03:11:05.000000 misleep-0.2.2b0/test/test_signal_io.py
--rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.2.2b0/test/test_signals_viz.py
--rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.2.2b0/test/test_spectral_viz.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.908608 misleep-0.2.3b0/
+-rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.2.3b0/LICENSE
+-rw-rw-rw-   0        0        0     3058 2024-04-21 09:38:41.907609 misleep-0.2.3b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1960 2024-04-17 11:42:46.000000 misleep-0.2.3b0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.885995 misleep-0.2.3b0/misleep/
+-rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.2.3b0/misleep/__init__.py
+-rw-rw-rw-   0        0        0      167 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/__main__.py
+-rw-rw-rw-   0        0        0      528 2024-04-21 09:33:59.000000 misleep-0.2.3b0/misleep/config.ini
+drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.891604 misleep-0.2.3b0/misleep/gui/
+-rw-rw-rw-   0        0        0      334 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/gui/__init__.py
+-rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.2.3b0/misleep/gui/about.py
+-rw-rw-rw-   0        0        0     7542 2024-04-21 09:29:39.000000 misleep-0.2.3b0/misleep/gui/dialog.py
+-rw-rw-rw-   0        0        0    56484 2024-04-17 11:23:33.000000 misleep-0.2.3b0/misleep/gui/main_window.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.894608 misleep-0.2.3b0/misleep/gui/resources/
+-rw-rw-rw-   0        0        0       47 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/gui/resources/__init__.py
+-rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.2.3b0/misleep/gui/resources/entire_logo.png
+-rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.2.3b0/misleep/gui/resources/logo.png
+-rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.2.3b0/misleep/gui/resources/misleep.py
+-rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.2.3b0/misleep/gui/resources/misleep.qrc
+-rw-rw-rw-   0        0        0      476 2024-04-15 10:19:04.000000 misleep-0.2.3b0/misleep/gui/show.py
+-rw-rw-rw-   0        0        0     5893 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/gui/spec_window.py
+-rw-rw-rw-   0        0        0     3177 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/gui/thread.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.896607 misleep-0.2.3b0/misleep/gui/uis/
+-rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.2.3b0/misleep/gui/uis/__init__.py
+-rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.2.3b0/misleep/gui/uis/about_ui.py
+-rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.2.3b0/misleep/gui/uis/label_dialog_ui.py
+-rw-rw-rw-   0        0        0    24912 2024-04-17 03:11:18.000000 misleep-0.2.3b0/misleep/gui/uis/main_window_ui.py
+-rw-rw-rw-   0        0        0     2371 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/gui/uis/save_data_dialog_ui.py
+-rw-rw-rw-   0        0        0     4466 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/gui/uis/spec_window_ui.py
+-rw-rw-rw-   0        0        0     4884 2024-04-17 11:15:15.000000 misleep-0.2.3b0/misleep/gui/uis/transfer_result_dialog_ui.py
+-rw-rw-rw-   0        0        0     3441 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/gui/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.899607 misleep-0.2.3b0/misleep/io/
+-rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.2.3b0/misleep/io/__init__.py
+-rw-rw-rw-   0        0        0     7578 2024-04-21 09:27:40.000000 misleep-0.2.3b0/misleep/io/annotation_io.py
+-rw-rw-rw-   0        0        0    14995 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/io/base.py
+-rw-rw-rw-   0        0        0     5027 2024-04-17 08:38:52.000000 misleep-0.2.3b0/misleep/io/signal_io.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.901607 misleep-0.2.3b0/misleep/preprocessing/
+-rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.2.3b0/misleep/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.2.3b0/misleep/preprocessing/channel.py
+-rw-rw-rw-   0        0        0      458 2024-04-15 10:35:14.000000 misleep-0.2.3b0/misleep/preprocessing/signals.py
+-rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.2.3b0/misleep/preprocessing/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.902607 misleep-0.2.3b0/misleep/utils/
+-rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.2.3b0/misleep/utils/__init__.py
+-rw-rw-rw-   0        0        0     4394 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/utils/annotation.py
+-rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.2.3b0/misleep/utils/signals.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.903607 misleep-0.2.3b0/misleep/viz/
+-rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.2.3b0/misleep/viz/__init__.py
+-rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.2.3b0/misleep/viz/hypnogram.py
+-rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.2.3b0/misleep/viz/signals.py
+-rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.2.3b0/misleep/viz/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.887995 misleep-0.2.3b0/misleep.egg-info/
+-rw-rw-rw-   0        0        0     3058 2024-04-21 09:38:41.000000 misleep-0.2.3b0/misleep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1401 2024-04-21 09:38:41.000000 misleep-0.2.3b0/misleep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 09:38:41.000000 misleep-0.2.3b0/misleep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-21 09:38:41.000000 misleep-0.2.3b0/misleep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-21 09:38:41.000000 misleep-0.2.3b0/misleep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 09:38:41.908608 misleep-0.2.3b0/setup.cfg
+-rw-rw-rw-   0        0        0     2154 2024-04-21 09:34:06.000000 misleep-0.2.3b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.907609 misleep-0.2.3b0/test/
+-rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.2.3b0/test/test_annotation_io.py
+-rw-rw-rw-   0        0        0      143 2024-04-15 03:11:05.000000 misleep-0.2.3b0/test/test_loadmat73.py
+-rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.2.3b0/test/test_midata.py
+-rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.2.3b0/test/test_show.py
+-rw-rw-rw-   0        0        0     1488 2024-04-15 03:11:05.000000 misleep-0.2.3b0/test/test_signal_io.py
+-rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.2.3b0/test/test_signals_viz.py
+-rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.2.3b0/test/test_spectral_viz.py
```

### Comparing `misleep-0.2.2b0/LICENSE` & `misleep-0.2.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/PKG-INFO` & `misleep-0.2.3b0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.2.2b0
+Version: 0.2.3b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
@@ -36,14 +36,19 @@
 ![logo](resources/entire_logo.png)
 
 ## Get start
 ```shell
 pip install misleep==0.2.2b0
 ```
 
+Find the directory where you installed misleep, run
+```shell
+python -m misleep
+```
+
 ### New features
 1. New data structure
 
 You can save the original data as a new data structure (See `Data save protocol`).
 Where you can add the channels' name, sampling rate and the acquisition time into 
 the original data.
```

### Comparing `misleep-0.2.2b0/README.md` & `misleep-0.2.3b0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 ![logo](resources/entire_logo.png)
 
 ## Get start
 ```shell
 pip install misleep==0.2.2b0
 ```
 
+Find the directory where you installed misleep, run
+```shell
+python -m misleep
+```
+
 ### New features
 1. New data structure
 
 You can save the original data as a new data structure (See `Data save protocol`).
 Where you can add the channels' name, sampling rate and the acquisition time into 
 the original data.
```

### Comparing `misleep-0.2.2b0/misleep/config.ini` & `misleep-0.2.3b0/misleep/config.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [gui]
-version = v0.2.2 Beta
+version = v0.2.3 Beta
 updatetime = 2024/04/01
 marker = ['pat', 'add water', 'third']
 startend = ['SWA', 'SWA', 'start end label', 'start end label', 'start end label', 'start end label', 'start end label']
 statemap = {"1": "NREM", "2": "REM", "3": "Wake", "4": "INIT"}
 statecolor = {"1": "orange", "2": "skyblue", "3": "red", "4": "white"}
 statecolorbgalpha = 0.1
 markerlinecolor = "red"
 startendlinecolor = "blue"
-openpath = E:/workplace/EEGProcessing/00_DATA/20240117_0700_WXQ_3mice_24h/mouse2/mouse2_label.txt
+openpath = E:/workplace/EEGProcessing/00_DATA/20240114_17_0700_7pin/female3/female3_label.txt
```

### Comparing `misleep-0.2.2b0/misleep/gui/about.py` & `misleep-0.2.3b0/misleep/gui/about.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/gui/dialog.py` & `misleep-0.2.3b0/misleep/gui/dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import datetime
 
 from misleep.gui.uis.label_dialog_ui import Ui_Dialog
 from misleep.gui.uis.transfer_result_dialog_ui import Ui_TransferResultDialog
 from misleep.gui.thread import SaveThread
 from misleep.io.annotation_io import transfer_result
 import pandas as pd
+from copy import deepcopy
 
 
 class label_dialog(QDialog, Ui_Dialog):
     def __init__(self, parent=None, config=None):
         """
         Initialize the Label dialog of MiSleep
         """
@@ -166,14 +167,16 @@
         self.ACTimeEditor.setEnabled(True)
 
     def enable_start_time_editor(self):
         self.TransferStartTimeEdit.setEnabled(True)
 
     def transfer(self, config, mianno, ac_time):
         """Transfer result to dataframe, triggered by okay button"""
+        mianno = deepcopy(mianno)
+        ac_time = deepcopy(ac_time)
 
         if self.ResetTimeCheckBox.isChecked():
             ac_time = self.ACTimeEditor.dateTime().toPyDateTime()
         else:
             ac_time = datetime.datetime.strptime(ac_time, "%Y%m%d-%H:%M:%S")
         
         if self.ResetTransferStartTimeCheckBox.isChecked():
```

### Comparing `misleep-0.2.2b0/misleep/gui/main_window.py` & `misleep-0.2.3b0/misleep/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/gui/resources/entire_logo.png` & `misleep-0.2.3b0/misleep/gui/resources/entire_logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/gui/resources/logo.png` & `misleep-0.2.3b0/misleep/gui/resources/logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/gui/resources/misleep.py` & `misleep-0.2.3b0/misleep/gui/resources/misleep.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/gui/spec_window.py` & `misleep-0.2.3b0/misleep/gui/spec_window.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/gui/thread.py` & `misleep-0.2.3b0/misleep/gui/thread.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/gui/uis/about_ui.py` & `misleep-0.2.3b0/misleep/gui/uis/about_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/gui/uis/label_dialog_ui.py` & `misleep-0.2.3b0/misleep/gui/uis/label_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/gui/uis/main_window_ui.py` & `misleep-0.2.3b0/misleep/gui/uis/main_window_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/gui/uis/save_data_dialog_ui.py` & `misleep-0.2.3b0/misleep/gui/uis/save_data_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/gui/uis/spec_window_ui.py` & `misleep-0.2.3b0/misleep/gui/uis/spec_window_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/gui/uis/transfer_result_dialog_ui.py` & `misleep-0.2.3b0/misleep/gui/uis/transfer_result_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/gui/utils.py` & `misleep-0.2.3b0/misleep/gui/utils.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/io/annotation_io.py` & `misleep-0.2.3b0/misleep/io/annotation_io.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 @Project: MiSleep_v2 
 @File: annotation_io.py
 @Author: Xueqiang Wang
 @Date: 2024/3/6
 @Description:  Annotation io, default is for MiSleep annotation, `NAME.txt`
 """
 from misleep.io.base import MiAnnotation
-from misleep.utils.annotation import marker2mianno, start_end2mianno, lst2group, sleep_state2mianno, transfer_time, insert_row, temp_loop4below_row
+from misleep.utils.annotation import marker2mianno, start_end2mianno, lst2group, sleep_state2mianno, transfer_time
 import pandas as pd
 
 
 def load_misleep_anno(file_path):
     """
     Load annotations from misleep annotation file
 
@@ -72,63 +72,91 @@
 
     start_end_label = [[
         transfer_time(ac_time, each[0], '%Y-%m-%d %H:%M:%S', ms=True), each[0], 1,
         transfer_time(ac_time, each[1], '%Y-%m-%d %H:%M:%S', ms=True), each[1], 0,
         each[2]
     ] for each in mianno.start_end]
 
-    sleep_state = lst2group([[idx+1, each] 
-                                for idx, each in enumerate(mianno.sleep_state)])
-    sleep_state = [[
-        transfer_time(ac_time, each[0], '%Y-%m-%d %H:%M:%S'), each[0], 1,
-        transfer_time(ac_time, each[1], '%Y-%m-%d %H:%M:%S'), each[1], 0,
-        each[2], mianno.state_map[each[2]]
-    ] for each in sleep_state]
-
+    # Add marker first
+    sleep_state = []
+    for each in range(int(len(mianno.sleep_state)/3600)+1):
+        temp_hour_label = mianno.sleep_state[each*3600: (each+1)*3600]
+        if temp_hour_label != []:
+            sleep_state.append(temp_hour_label)
+
+    marker_sleep_state = []
+    for hour, label in enumerate(sleep_state):
+        hour_sleep_state = lst2group(
+            [idx+1+hour*3600, each] for idx, each in enumerate(label))
+        marker_sleep_state += [[
+            transfer_time(ac_time, each[0], '%Y-%m-%d %H:%M:%S'), each[0], 1,
+            transfer_time(ac_time, each[1], '%Y-%m-%d %H:%M:%S'), each[1], 0,
+            each[2], mianno.state_map[each[2]], each[1]-each[0]+1, hour
+        ] for each in hour_sleep_state]
+
+        marker_sleep_state += [[
+            transfer_time(ac_time, (hour+1)*3600, '%Y-%m-%d %H:%M:%S'), (hour+1)*3600, 1,
+            transfer_time(ac_time, (hour+1)*3600, '%Y-%m-%d %H:%M:%S'), (hour+1)*3600, 0,
+            5, 'MARKER', '', '']]
+        
     columns=['start_time', 'start_time_sec', 'start_code',
-                'end_time', 'end_time_sec', 'end_code',
-                'state_code', 'state']
+            'end_time', 'end_time_sec', 'end_code',
+            'state_code', 'state', 'bout_duration', 'hour']
+
+    df = pd.DataFrame(data=marker_sleep_state, columns=columns)
+
+    # sleep_state = lst2group([[idx+1, each] 
+    #                             for idx, each in enumerate(mianno.sleep_state)])
+    # sleep_state = [[
+    #     transfer_time(ac_time, each[0], '%Y-%m-%d %H:%M:%S'), each[0], 1,
+    #     transfer_time(ac_time, each[1], '%Y-%m-%d %H:%M:%S'), each[1], 0,
+    #     each[2], mianno.state_map[each[2]]
+    # ] for each in sleep_state]
+
+    # columns=['start_time', 'start_time_sec', 'start_code',
+    #             'end_time', 'end_time_sec', 'end_code',
+    #             'state_code', 'state']
 
-    df = pd.DataFrame(data=sleep_state, columns=columns)
+    # df = pd.DataFrame(data=sleep_state, columns=columns)
     
-    new_df = pd.DataFrame(columns=columns)
-    for idx, row in df.iterrows():
-        if row['end_time_sec'] % 3600 == 0:
-            new_df = insert_row(new_df, idx, row)
-            # Just add a row and nothing else
-            new_row = pd.Series([
-                row['end_time'], row['end_time_sec'], ' ',
-                row['end_time'], row['end_time_sec'], '5',
-                ' ', 'MARKER'
-            ], index=columns)
-            new_df = insert_row(new_df, new_df.shape[0], new_row)
-            continue
-
-        if int(row['end_time_sec'] / 3600) > int(row['start_time_sec'] / 3600):
-
-            previous_row, new_row, below_row = temp_loop4below_row(row, ac_time, columns)
-
-            new_df = insert_row(new_df, new_df.shape[0], previous_row)
-            new_df = insert_row(new_df, new_df.shape[0], new_row)
-            while int(below_row['end_time_sec'] / 3600) > int(below_row['start_time_sec'] / 3600):
-                row = below_row
-                previous_row, new_row, below_row = temp_loop4below_row(row, ac_time, columns)
-                new_df = insert_row(new_df, new_df.shape[0], previous_row)
-                new_df = insert_row(new_df, new_df.shape[0], new_row)
-
-            new_df = insert_row(new_df, new_df.shape[0], below_row)
-            continue
+    # new_df = pd.DataFrame(columns=columns)
+    # for idx, row in df.iterrows():
+    #     if row['end_time_sec'] % 3600 == 0:
+    #         new_df = insert_row(new_df, idx, row)
+    #         # Just add a row and nothing else
+    #         new_row = pd.Series([
+    #             row['end_time'], row['end_time_sec'], ' ',
+    #             row['end_time'], row['end_time_sec'], '5',
+    #             ' ', 'MARKER'
+    #         ], index=columns)
+    #         new_df = insert_row(new_df, new_df.shape[0], new_row)
+    #         continue
+
+    #     if int(row['end_time_sec'] / 3600) > int(row['start_time_sec'] / 3600):
+
+    #         previous_row, new_row, below_row = temp_loop4below_row(row, ac_time, columns)
+
+    #         new_df = insert_row(new_df, new_df.shape[0], previous_row)
+    #         new_df = insert_row(new_df, new_df.shape[0], new_row)
+    #         while int(below_row['end_time_sec'] / 3600) > int(below_row['start_time_sec'] / 3600):
+    #             row = below_row
+    #             previous_row, new_row, below_row = temp_loop4below_row(row, ac_time, columns)
+    #             new_df = insert_row(new_df, new_df.shape[0], previous_row)
+    #             new_df = insert_row(new_df, new_df.shape[0], new_row)
+
+    #         new_df = insert_row(new_df, new_df.shape[0], below_row)
+    #         continue
 
-        new_df = insert_row(new_df, new_df.shape[0], row)
+    #     new_df = insert_row(new_df, new_df.shape[0], row)
 
-    df = new_df
-    del new_df
+    # df = new_df
+    # del new_df
 
-    df['bout_duration'] = df.apply(
-        lambda x: x[4] - x[1] + 1 if x[7] != 'MARKER' else '', axis=1)
+    # df['bout_duration'] = df.apply(
+    #     lambda x: x[4] - x[1] + 1 if x[7] != 'MARKER' else '', axis=1)
     
     df['hour'] = df['start_time_sec'].apply(lambda x: int(x / 3600) if x % 3600 != 0 else '')
     analyse_df = pd.DataFrame()
 
     temp_hour = list(set(list(df['hour'])))
     temp_hour.remove('')
     temp_hour = sorted(temp_hour)
```

### Comparing `misleep-0.2.2b0/misleep/io/base.py` & `misleep-0.2.3b0/misleep/io/base.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/io/signal_io.py` & `misleep-0.2.3b0/misleep/io/signal_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/preprocessing/spectral.py` & `misleep-0.2.3b0/misleep/preprocessing/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/utils/annotation.py` & `misleep-0.2.3b0/misleep/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/utils/signals.py` & `misleep-0.2.3b0/misleep/utils/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/viz/hypnogram.py` & `misleep-0.2.3b0/misleep/viz/hypnogram.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/viz/signals.py` & `misleep-0.2.3b0/misleep/viz/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep/viz/spectral.py` & `misleep-0.2.3b0/misleep/viz/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/misleep.egg-info/PKG-INFO` & `misleep-0.2.3b0/misleep.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.2.2b0
+Version: 0.2.3b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
@@ -36,14 +36,19 @@
 ![logo](resources/entire_logo.png)
 
 ## Get start
 ```shell
 pip install misleep==0.2.2b0
 ```
 
+Find the directory where you installed misleep, run
+```shell
+python -m misleep
+```
+
 ### New features
 1. New data structure
 
 You can save the original data as a new data structure (See `Data save protocol`).
 Where you can add the channels' name, sampling rate and the acquisition time into 
 the original data.
```

### Comparing `misleep-0.2.2b0/misleep.egg-info/SOURCES.txt` & `misleep-0.2.3b0/misleep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/setup.py` & `misleep-0.2.3b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 DISTNAME = "misleep"
 MAINTAINER = "Xueqiang Wang"
 MAINTAINER_EMAIL = "swang@gmail.com"
 URL = "https://github.com/BryanWang0702/MiSleep/"
 LICENSE = "BSD (3-clause)"
 DOWNLOAD_URL = "https://github.com/BryanWang0702/MiSleep/"
-VERSION = "0.2.2b0"
+VERSION = "0.2.3b0"
 
 INSTALL_REQUIRES = [
     "numpy>=1.18.1",
     "matplotlib",
     "scipy",
     "pyedflib",
     "hdf5storage",
```

### Comparing `misleep-0.2.2b0/test/test_midata.py` & `misleep-0.2.3b0/test/test_midata.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/test/test_signal_io.py` & `misleep-0.2.3b0/test/test_signal_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/test/test_signals_viz.py` & `misleep-0.2.3b0/test/test_signals_viz.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.2b0/test/test_spectral_viz.py` & `misleep-0.2.3b0/test/test_spectral_viz.py`

 * *Files identical despite different names*


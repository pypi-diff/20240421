# Comparing `tmp/DragonLog-1.0.tar.gz` & `tmp/dragonlog-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DragonLog-1.0.tar", last modified: Thu Apr  4 05:34:36 2024, max compression
+gzip compressed data, was "dragonlog-1.1.tar", last modified: Sun Apr 21 06:54:54 2024, max compression
```

## Comparing `DragonLog-1.0.tar` & `dragonlog-1.1.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 05:34:36.292085 DragonLog-1.0/
-drwxrwxrwx   0        0        0        0 2024-04-04 05:34:36.285091 DragonLog-1.0/DragonLog.egg-info/
--rw-rw-rw-   0        0        0     7399 2024-04-04 05:34:35.000000 DragonLog-1.0/DragonLog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1597 2024-04-04 05:34:36.000000 DragonLog-1.0/DragonLog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 05:34:35.000000 DragonLog-1.0/DragonLog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-04 05:34:35.000000 DragonLog-1.0/DragonLog.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2024-04-04 05:34:35.000000 DragonLog-1.0/DragonLog.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-04 05:34:35.000000 DragonLog-1.0/DragonLog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      158 2024-03-19 12:18:34.000000 DragonLog-1.0/LICENCE.txt
--rw-rw-rw-   0        0        0       93 2023-11-21 13:44:18.000000 DragonLog-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7399 2024-04-04 05:34:36.289088 DragonLog-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6399 2024-04-03 17:19:13.000000 DragonLog-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 05:34:36.191157 DragonLog-1.0/dragonlog/
--rw-rw-rw-   0        0        0    61318 2024-04-02 11:52:42.000000 DragonLog-1.0/dragonlog/DragonLog.py
--rw-rw-rw-   0        0        0     2062 2024-02-20 17:06:17.000000 DragonLog-1.0/dragonlog/DragonLog_AppSelect.py
--rw-rw-rw-   0        0        0     3041 2024-04-04 05:33:29.000000 DragonLog-1.0/dragonlog/DragonLog_AppSelect_ui.py
--rw-rw-rw-   0        0        0     5971 2024-03-27 06:07:28.000000 DragonLog-1.0/dragonlog/DragonLog_CallBook.py
--rw-rw-rw-   0        0        0     7403 2024-04-01 18:20:40.000000 DragonLog-1.0/dragonlog/DragonLog_LoTW.py
--rw-rw-rw-   0        0        0    17410 2024-04-04 05:33:28.000000 DragonLog-1.0/dragonlog/DragonLog_MainWindow_ui.py
--rw-rw-rw-   0        0        0    44824 2024-04-02 19:00:21.000000 DragonLog-1.0/dragonlog/DragonLog_QSOForm.py
--rw-rw-rw-   0        0        0    40015 2024-04-04 05:33:29.000000 DragonLog-1.0/dragonlog/DragonLog_QSOForm_ui.py
--rw-rw-rw-   0        0        0     1054 2024-04-02 05:05:28.000000 DragonLog-1.0/dragonlog/DragonLog_RegEx.py
--rw-rw-rw-   0        0        0    19600 2024-03-29 19:18:43.000000 DragonLog-1.0/dragonlog/DragonLog_Settings.py
--rw-rw-rw-   0        0        0    38585 2024-04-04 05:33:29.000000 DragonLog-1.0/dragonlog/DragonLog_Settings_ui.py
--rw-rw-rw-   0        0        0     5324 2024-03-23 19:55:25.000000 DragonLog-1.0/dragonlog/DragonLog_eQSL.py
--rw-rw-rw-   0        0        0     2484 2024-04-04 05:17:54.000000 DragonLog-1.0/dragonlog/Logger.py
--rw-rw-rw-   0        0        0        0 2023-11-21 18:25:24.000000 DragonLog-1.0/dragonlog/__init__.py
--rw-rw-rw-   0        0        0       45 2023-11-21 18:20:52.000000 DragonLog-1.0/dragonlog/__main__.py
--rw-rw-rw-   0        0        0       63 2024-04-04 05:33:28.000000 DragonLog-1.0/dragonlog/__version__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 05:34:36.208145 DragonLog-1.0/dragonlog/data/
--rw-rw-rw-   0        0        0     6399 2024-04-03 17:19:13.000000 DragonLog-1.0/dragonlog/data/README.md
--rw-rw-rw-   0        0        0     1816 2023-10-08 14:01:05.000000 DragonLog-1.0/dragonlog/data/bands.json
--rw-rw-rw-   0        0        0     6834 2023-10-09 17:58:49.000000 DragonLog-1.0/dragonlog/data/cb_channels.json
--rw-rw-rw-   0        0        0     1115 2023-11-15 18:59:09.000000 DragonLog-1.0/dragonlog/data/color_map.json
-drwxrwxrwx   0        0        0        0 2024-04-04 05:34:36.213142 DragonLog-1.0/dragonlog/data/i18n/
--rw-rw-rw-   0        0        0    23695 2024-04-04 05:33:32.000000 DragonLog-1.0/dragonlog/data/i18n/DragonLog_de.qm
--rw-rw-rw-   0        0        0      108 2024-03-28 07:19:36.000000 DragonLog-1.0/dragonlog/data/i18n/ascii_replace_de.json
--rw-rw-rw-   0        0        0     4275 2023-10-11 18:47:43.000000 DragonLog-1.0/dragonlog/data/modes.json
-drwxrwxrwx   0        0        0        0 2024-04-04 05:34:36.280093 DragonLog-1.0/dragonlog/icons/
--rw-rw-rw-   0        0        0    84255 2024-04-03 05:47:08.000000 DragonLog-1.0/dragonlog/icons/Screenshot.png
--rw-rw-rw-   0        0        0     2775 2006-10-09 18:29:54.000000 DragonLog-1.0/dragonlog/icons/db.png
--rw-rw-rw-   0        0        0      935 2006-10-09 18:46:20.000000 DragonLog-1.0/dragonlog/icons/edit.png
--rw-rw-rw-   0        0        0     1501 2006-10-09 18:51:24.000000 DragonLog-1.0/dragonlog/icons/edit_add.png
--rw-rw-rw-   0        0        0     4853 2023-10-06 05:04:50.000000 DragonLog-1.0/dragonlog/icons/edit_addmulti.png
--rw-rw-rw-   0        0        0     4222 2023-10-06 05:13:53.000000 DragonLog-1.0/dragonlog/icons/edit_addmulti.xcf
--rw-rw-rw-   0        0        0      901 2006-07-05 03:36:10.000000 DragonLog-1.0/dragonlog/icons/edit_remove.png
--rw-rw-rw-   0        0        0     2360 2007-05-26 19:17:06.000000 DragonLog-1.0/dragonlog/icons/exit.png
--rw-rw-rw-   0        0        0      697 2024-03-23 19:55:25.000000 DragonLog-1.0/dragonlog/icons/file_doc.png
--rw-rw-rw-   0        0        0     2321 2006-10-09 18:55:14.000000 DragonLog-1.0/dragonlog/icons/fileexport.png
--rw-rw-rw-   0        0        0     2076 2006-10-09 19:11:50.000000 DragonLog-1.0/dragonlog/icons/fileimport.png
--rw-rw-rw-   0        0        0     2166 2006-10-09 16:32:12.000000 DragonLog-1.0/dragonlog/icons/gear.png
--rw-rw-rw-   0        0        0     2461 2006-10-09 18:22:00.000000 DragonLog-1.0/dragonlog/icons/help.png
--rw-rw-rw-   0        0        0     4652 2023-10-04 17:16:16.000000 DragonLog-1.0/dragonlog/icons/icons8-dragon-96.png
--rw-rw-rw-   0        0        0    19186 2023-10-06 12:24:58.000000 DragonLog-1.0/dragonlog/icons/icons8-dragon-96.xcf
--rw-rw-rw-   0        0        0     2184 2006-10-09 19:49:00.000000 DragonLog-1.0/dragonlog/icons/info.png
--rw-rw-rw-   0        0        0    54470 2023-10-06 12:25:24.000000 DragonLog-1.0/dragonlog/icons/logo.ico
--rw-rw-rw-   0        0        0     2225 2006-10-09 18:20:08.000000 DragonLog-1.0/dragonlog/icons/player_play.png
--rw-rw-rw-   0        0        0     2112 2024-03-05 19:18:39.000000 DragonLog-1.0/dragonlog/icons/player_stop.png
--rw-rw-rw-   0        0        0    21406 2024-03-25 10:49:08.000000 DragonLog-1.0/dragonlog/icons/upload_lotw.png
--rw-rw-rw-   0        0        0     7906 2024-03-25 10:48:26.000000 DragonLog-1.0/dragonlog/icons/upload_lotw.xcf
--rw-rw-rw-   0        0        0     1819 2006-10-17 07:09:30.000000 DragonLog-1.0/dragonlog/icons/watch.png
--rw-rw-rw-   0        0        0     1159 2024-03-23 19:55:25.000000 DragonLog-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-04 05:34:36.293085 DragonLog-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1498 2024-03-19 12:15:10.000000 DragonLog-1.0/setup_msi.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:54:54.224161 dragonlog-1.1/
+drwxrwxrwx   0        0        0        0 2024-04-21 06:54:54.220116 dragonlog-1.1/DragonLog.egg-info/
+-rw-rw-rw-   0        0        0     7399 2024-04-21 06:54:53.000000 dragonlog-1.1/DragonLog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1603 2024-04-21 06:54:54.000000 dragonlog-1.1/DragonLog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 06:54:53.000000 dragonlog-1.1/DragonLog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-21 06:54:53.000000 dragonlog-1.1/DragonLog.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2024-04-21 06:54:53.000000 dragonlog-1.1/DragonLog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-21 06:54:53.000000 dragonlog-1.1/DragonLog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      158 2024-03-19 12:18:34.000000 dragonlog-1.1/LICENCE.txt
+-rw-rw-rw-   0        0        0       93 2023-11-21 13:44:18.000000 dragonlog-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7399 2024-04-21 06:54:54.222138 dragonlog-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6399 2024-04-03 17:19:13.000000 dragonlog-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 06:54:54.132262 dragonlog-1.1/dragonlog/
+-rw-rw-rw-   0        0        0    10562 2024-04-15 18:06:37.000000 dragonlog-1.1/dragonlog/CallBook.py
+-rw-rw-rw-   0        0        0    63578 2024-04-18 19:01:18.000000 dragonlog-1.1/dragonlog/DragonLog.py
+-rw-rw-rw-   0        0        0     2062 2024-02-20 17:06:17.000000 dragonlog-1.1/dragonlog/DragonLog_AppSelect.py
+-rw-rw-rw-   0        0        0     3041 2024-04-21 06:53:48.000000 dragonlog-1.1/dragonlog/DragonLog_AppSelect_ui.py
+-rw-rw-rw-   0        0        0    17410 2024-04-21 06:53:47.000000 dragonlog-1.1/dragonlog/DragonLog_MainWindow_ui.py
+-rw-rw-rw-   0        0        0    47234 2024-04-19 18:34:33.000000 dragonlog-1.1/dragonlog/DragonLog_QSOForm.py
+-rw-rw-rw-   0        0        0    38980 2024-04-21 06:53:48.000000 dragonlog-1.1/dragonlog/DragonLog_QSOForm_ui.py
+-rw-rw-rw-   0        0        0    21133 2024-04-18 06:08:40.000000 dragonlog-1.1/dragonlog/DragonLog_Settings.py
+-rw-rw-rw-   0        0        0    39219 2024-04-21 06:53:48.000000 dragonlog-1.1/dragonlog/DragonLog_Settings_ui.py
+-rw-rw-rw-   0        0        0     7403 2024-04-15 17:33:29.000000 dragonlog-1.1/dragonlog/LoTW.py
+-rw-rw-rw-   0        0        0     2585 2024-04-12 05:48:01.000000 dragonlog-1.1/dragonlog/Logger.py
+-rw-rw-rw-   0        0        0     1134 2024-04-15 17:33:29.000000 dragonlog-1.1/dragonlog/RegEx.py
+-rw-rw-rw-   0        0        0        0 2023-11-21 18:25:24.000000 dragonlog-1.1/dragonlog/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-11-21 18:20:52.000000 dragonlog-1.1/dragonlog/__main__.py
+-rw-rw-rw-   0        0        0       63 2024-04-21 06:53:47.000000 dragonlog-1.1/dragonlog/__version__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:54:54.144562 dragonlog-1.1/dragonlog/data/
+-rw-rw-rw-   0        0        0     6399 2024-04-03 17:19:13.000000 dragonlog-1.1/dragonlog/data/README.md
+-rw-rw-rw-   0        0        0     1816 2023-10-08 14:01:05.000000 dragonlog-1.1/dragonlog/data/bands.json
+-rw-rw-rw-   0        0        0     6834 2023-10-09 17:58:49.000000 dragonlog-1.1/dragonlog/data/cb_channels.json
+-rw-rw-rw-   0        0        0     1115 2023-11-15 18:59:09.000000 dragonlog-1.1/dragonlog/data/color_map.json
+drwxrwxrwx   0        0        0        0 2024-04-21 06:54:54.149639 dragonlog-1.1/dragonlog/data/i18n/
+-rw-rw-rw-   0        0        0    24604 2024-04-21 06:53:51.000000 dragonlog-1.1/dragonlog/data/i18n/DragonLog_de.qm
+-rw-rw-rw-   0        0        0      108 2024-03-28 07:19:36.000000 dragonlog-1.1/dragonlog/data/i18n/ascii_replace_de.json
+-rw-rw-rw-   0        0        0     4275 2023-10-11 18:47:43.000000 dragonlog-1.1/dragonlog/data/modes.json
+-rw-rw-rw-   0        0        0     5348 2024-04-15 17:33:29.000000 dragonlog-1.1/dragonlog/eQSL.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:54:54.216101 dragonlog-1.1/dragonlog/icons/
+-rw-rw-rw-   0        0        0    84255 2024-04-03 05:47:08.000000 dragonlog-1.1/dragonlog/icons/Screenshot.png
+-rw-rw-rw-   0        0        0     2775 2006-10-09 18:29:54.000000 dragonlog-1.1/dragonlog/icons/db.png
+-rw-rw-rw-   0        0        0      935 2006-10-09 18:46:20.000000 dragonlog-1.1/dragonlog/icons/edit.png
+-rw-rw-rw-   0        0        0     1501 2006-10-09 18:51:24.000000 dragonlog-1.1/dragonlog/icons/edit_add.png
+-rw-rw-rw-   0        0        0     4853 2023-10-06 05:04:50.000000 dragonlog-1.1/dragonlog/icons/edit_addmulti.png
+-rw-rw-rw-   0        0        0     4222 2023-10-06 05:13:53.000000 dragonlog-1.1/dragonlog/icons/edit_addmulti.xcf
+-rw-rw-rw-   0        0        0      901 2006-07-05 03:36:10.000000 dragonlog-1.1/dragonlog/icons/edit_remove.png
+-rw-rw-rw-   0        0        0     2360 2007-05-26 19:17:06.000000 dragonlog-1.1/dragonlog/icons/exit.png
+-rw-rw-rw-   0        0        0      697 2024-03-23 19:55:25.000000 dragonlog-1.1/dragonlog/icons/file_doc.png
+-rw-rw-rw-   0        0        0     2321 2006-10-09 18:55:14.000000 dragonlog-1.1/dragonlog/icons/fileexport.png
+-rw-rw-rw-   0        0        0     2076 2006-10-09 19:11:50.000000 dragonlog-1.1/dragonlog/icons/fileimport.png
+-rw-rw-rw-   0        0        0     2166 2006-10-09 16:32:12.000000 dragonlog-1.1/dragonlog/icons/gear.png
+-rw-rw-rw-   0        0        0     2461 2006-10-09 18:22:00.000000 dragonlog-1.1/dragonlog/icons/help.png
+-rw-rw-rw-   0        0        0     4652 2023-10-04 17:16:16.000000 dragonlog-1.1/dragonlog/icons/icons8-dragon-96.png
+-rw-rw-rw-   0        0        0    19186 2023-10-06 12:24:58.000000 dragonlog-1.1/dragonlog/icons/icons8-dragon-96.xcf
+-rw-rw-rw-   0        0        0     2184 2006-10-09 19:49:00.000000 dragonlog-1.1/dragonlog/icons/info.png
+-rw-rw-rw-   0        0        0    54470 2023-10-06 12:25:24.000000 dragonlog-1.1/dragonlog/icons/logo.ico
+-rw-rw-rw-   0        0        0     2443 2006-10-09 19:00:44.000000 dragonlog-1.1/dragonlog/icons/no.png
+-rw-rw-rw-   0        0        0     1518 2006-10-09 20:22:10.000000 dragonlog-1.1/dragonlog/icons/ok.png
+-rw-rw-rw-   0        0        0     2225 2006-10-09 18:20:08.000000 dragonlog-1.1/dragonlog/icons/player_play.png
+-rw-rw-rw-   0        0        0     2112 2024-03-05 19:18:39.000000 dragonlog-1.1/dragonlog/icons/player_stop.png
+-rw-rw-rw-   0        0        0    21406 2024-03-25 10:49:08.000000 dragonlog-1.1/dragonlog/icons/upload_lotw.png
+-rw-rw-rw-   0        0        0     7906 2024-03-25 10:48:26.000000 dragonlog-1.1/dragonlog/icons/upload_lotw.xcf
+-rw-rw-rw-   0        0        0     1819 2006-10-17 07:09:30.000000 dragonlog-1.1/dragonlog/icons/watch.png
+-rw-rw-rw-   0        0        0     1159 2024-03-23 19:55:25.000000 dragonlog-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-21 06:54:54.224161 dragonlog-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1498 2024-03-19 12:15:10.000000 dragonlog-1.1/setup_msi.py
```

### Comparing `DragonLog-1.0/DragonLog.egg-info/PKG-INFO` & `dragonlog-1.1/DragonLog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DragonLog
-Version: 1.0
+Version: 1.1
 Summary: Log QSO for Ham radio
 Author-email: "Andreas Schawo, DF1ASC" <andreas@schawo.de>
 Project-URL: Homepage, https://github.com/gitandy/DragonLog
 Project-URL: Bug Tracker, https://github.com/gitandy/DragonLog/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Other Audience
 Classifier: Operating System :: OS Independent
```

### Comparing `DragonLog-1.0/DragonLog.egg-info/SOURCES.txt` & `dragonlog-1.1/DragonLog.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 setup_msi.py
 DragonLog.egg-info/PKG-INFO
 DragonLog.egg-info/SOURCES.txt
 DragonLog.egg-info/dependency_links.txt
 DragonLog.egg-info/entry_points.txt
 DragonLog.egg-info/requires.txt
 DragonLog.egg-info/top_level.txt
+dragonlog/CallBook.py
 dragonlog/DragonLog.py
 dragonlog/DragonLog_AppSelect.py
 dragonlog/DragonLog_AppSelect_ui.py
-dragonlog/DragonLog_CallBook.py
-dragonlog/DragonLog_LoTW.py
 dragonlog/DragonLog_MainWindow_ui.py
 dragonlog/DragonLog_QSOForm.py
 dragonlog/DragonLog_QSOForm_ui.py
-dragonlog/DragonLog_RegEx.py
 dragonlog/DragonLog_Settings.py
 dragonlog/DragonLog_Settings_ui.py
-dragonlog/DragonLog_eQSL.py
+dragonlog/LoTW.py
 dragonlog/Logger.py
+dragonlog/RegEx.py
 dragonlog/__init__.py
 dragonlog/__main__.py
 dragonlog/__version__.py
+dragonlog/eQSL.py
 dragonlog/data/README.md
 dragonlog/data/bands.json
 dragonlog/data/cb_channels.json
 dragonlog/data/color_map.json
 dragonlog/data/modes.json
 dragonlog/data/i18n/DragonLog_de.qm
 dragonlog/data/i18n/ascii_replace_de.json
@@ -45,12 +45,14 @@
 dragonlog/icons/fileimport.png
 dragonlog/icons/gear.png
 dragonlog/icons/help.png
 dragonlog/icons/icons8-dragon-96.png
 dragonlog/icons/icons8-dragon-96.xcf
 dragonlog/icons/info.png
 dragonlog/icons/logo.ico
+dragonlog/icons/no.png
+dragonlog/icons/ok.png
 dragonlog/icons/player_play.png
 dragonlog/icons/player_stop.png
 dragonlog/icons/upload_lotw.png
 dragonlog/icons/upload_lotw.xcf
 dragonlog/icons/watch.png
```

### Comparing `DragonLog-1.0/PKG-INFO` & `dragonlog-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DragonLog
-Version: 1.0
+Version: 1.1
 Summary: Log QSO for Ham radio
 Author-email: "Andreas Schawo, DF1ASC" <andreas@schawo.de>
 Project-URL: Homepage, https://github.com/gitandy/DragonLog
 Project-URL: Bug Tracker, https://github.com/gitandy/DragonLog/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Other Audience
 Classifier: Operating System :: OS Independent
```

### Comparing `DragonLog-1.0/README.md` & `dragonlog-1.1/README.md`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/DragonLog.py` & `dragonlog-1.1/dragonlog/DragonLog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import csv
 import platform
 import sys
 import json
 import datetime
+from typing import Iterable
 
 from PyQt6 import QtCore, QtWidgets, QtSql, QtGui
 import adif_file
 from adif_file import adi, adx
 import xmltodict
 
 OPTION_OPENPYXL = False
@@ -17,19 +18,19 @@
 
     OPTION_OPENPYXL = True
 except ImportError:
     pass
 
 from . import DragonLog_MainWindow_ui
 from .Logger import Logger
-from .DragonLog_RegEx import find_non_ascii
+from .RegEx import find_non_ascii
 from .DragonLog_QSOForm import QSOForm
 from .DragonLog_Settings import Settings
 from .DragonLog_AppSelect import AppSelect
-from .DragonLog_LoTW import LoTW, LoTWADIFFieldException, LoTWRequestException, LoTWCommunicationException
+from .LoTW import LoTW, LoTWADIFFieldException, LoTWRequestException, LoTWCommunicationException
 
 __prog_name__ = 'DragonLog'
 __prog_desc__ = 'Log QSO for Ham radio'
 __author_name__ = 'Andreas Schawo, DF1ASC'
 __author_email__ = 'andreas@schawo.de'
 __copyright__ = 'Copyright 2023-2024 by Andreas Schawo,licensed under CC BY-SA 4.0'
 
@@ -48,19 +49,21 @@
 
 
 class DatabaseWriteException(Exception):
     pass
 
 
 class BackgroundBrushDelegate(QtWidgets.QStyledItemDelegate):
-    def __init__(self, color_map, column):
+    """A delegate to change background color depending on a columns conntent and translation of different columns"""
+
+    def __init__(self, color_map: dict, column: int):
         super(BackgroundBrushDelegate, self).__init__()
 
-        self.color_map = color_map
-        self.column = column
+        self.color_map: dict = color_map
+        self.column: int = column
 
     def getColor(self, value):
         color = [255, 255, 255, 0]  # white as fallback
 
         if value in self.color_map:
             color = self.color_map[value]
         elif 'default' in self.color_map:
@@ -71,14 +74,53 @@
     def initStyleOption(self, option: QtWidgets.QStyleOptionViewItem, index: QtCore.QModelIndex):
         super().initStyleOption(option, index)
 
         option.backgroundBrush = QtGui.QBrush(
             QtGui.QColor(*self.getColor(index.model().data(index.siblingAtColumn(self.column)))))
 
 
+class TranslatedTableModel(QtSql.QSqlTableModel):
+    """Translate propagation values and status to clear text and fancy icon for status"""
+
+    def __init__(self, parent, db_conn, status_cols: Iterable, prop_col: int, prop_tr: dict):
+        super(TranslatedTableModel, self).__init__(parent, db_conn)
+
+        self.status_cols = status_cols
+        self.status_translation = {
+            'Y': self.tr('Y'),
+            'N': self.tr('N'),
+            'M': self.tr('M'),
+            'R': self.tr('R'),
+        }
+
+        self.prop_col = prop_col
+        self.prop_translation = prop_tr
+
+        self.ok_icon = QtGui.QIcon(self.parent().searchFile('icons:ok.png'))
+        self.no_icon = QtGui.QIcon(self.parent().searchFile('icons:no.png'))
+
+    def data(self, idx, role = QtCore.Qt.ItemDataRole.DisplayRole):
+        value = super().data(idx, role)
+        if role == QtCore.Qt.ItemDataRole.DisplayRole:
+            if idx.column() in self.status_cols and value in self.status_translation:
+                return self.status_translation[value]
+            elif idx.column() == self.prop_col and value in self.prop_translation:
+                return self.prop_translation[value]
+
+        if role == QtCore.Qt.ItemDataRole.DecorationRole:
+            txt = super().data(idx, QtCore.Qt.ItemDataRole.DisplayRole)
+            if idx.column() in self.status_cols:
+                if txt in ('Y', 'M'):
+                    return self.ok_icon
+                else:
+                    return self.no_icon
+
+        return value
+
+
 class DragonLog(QtWidgets.QMainWindow, DragonLog_MainWindow_ui.Ui_MainWindow):
     __sql_cols__ = ('id', 'date_time', 'date_time_off', 'own_callsign', 'call_sign', 'name', 'qth', 'locator',
                     'rst_sent', 'rst_rcvd', 'band', 'mode', 'submode', 'freq', 'channel', 'power', 'propagation',
                     'own_name', 'own_qth', 'own_locator', 'radio', 'antenna',
                     'remarks', 'comments', 'dist',
                     'qsl_via', 'qsl_path', 'qsl_msg', 'qsl_sent', 'qsl_rcvd',
                     'eqsl_sent', 'eqsl_rcvd', 'lotw_sent', 'lotw_rcvd', 'hamqth')
@@ -241,15 +283,15 @@
             self.tr('Propagation'),
             self.tr('Own Name'),
             self.tr('Own QTH'),
             self.tr('Own Locator'),
             self.tr('Radio'),
             self.tr('Antenna'),
             self.tr('Notes'),
-            self.tr('Comments'),
+            self.tr('Comment'),
             self.tr('Distance'),
             self.tr('QSL via'),
             self.tr('QSL path'),
             self.tr('QSL message'),
             self.tr('QSL sent'),
             self.tr('QSL rcvd'),
             self.tr('eQSL sent'),
@@ -435,15 +477,19 @@
 
             if self.__db_con__.lastError().text():
                 raise DatabaseOpenException(self.__db_con__.lastError().text())
 
             if not self.checkDB(db_file):
                 return
 
-            model = QtSql.QSqlTableModel(self, self.__db_con__)
+            model = TranslatedTableModel(self, self.__db_con__,
+                                         status_cols=tuple(range(self.__sql_cols__.index('qsl_sent'),
+                                                                 self.__sql_cols__.index('hamqth')+1)),
+                                         prop_col=self.__sql_cols__.index('propagation'),
+                                         prop_tr=self.prop)
             model.setTable('qsos')
             self.QSOTableView.setModel(model)
 
             for c in self.__sql_cols__:
                 model.setHeaderData(self.__sql_cols__.index(c),
                                     QtCore.Qt.Orientation.Horizontal,
                                     self.__header_map__[c])
@@ -562,18 +608,23 @@
         self.qso_form.clear()
         self.qsoDockWidget.setVisible(True)
         self.qso_form.setChangeMode()
 
         i = self.QSOTableView.selectedIndexes().pop(0)
         qso_id = self.QSOTableView.model().data(i.siblingAtColumn(0))
 
-        values = []
-        for col in range(len(self.__sql_cols__)):
-            values.append(self.QSOTableView.model().data(i.siblingAtColumn(col)))
+        query = self.__db_con__.exec(f'SELECT * FROM qsos WHERE id = {qso_id}')
+        if query.lastError().text():
+            raise Exception(query.lastError().text())
 
+        values = []
+        while query.next():
+            for col in range(len(self.__sql_cols__)):
+                values.append(query.value(col))
+            break
         self.qso_form.values = dict(zip(self.__sql_cols__, values))
 
     def updateQSO(self, qso_id: int):
         self.log.info(f'Changing QSO {qso_id}...')
         values = self.qso_form.values
         values += (qso_id,)
 
@@ -707,20 +758,23 @@
 
     def exportADIF(self, file):
         self.log.info('Exporting to ADIF...')
 
         query_str = self.getQueryStr() if self.settings.value('imp_exp/only_recent', 0) else self.__db_select_stmnt__
         is_adx: bool = os.path.splitext(file)[-1] == '.adx'
         doc = self._build_adif_export_(query_str, is_adx)
-        if is_adx:
-            adx.dump(file, doc)
-        else:
-            adi.dump(file, doc, 'ADIF Export by DragonLog')
+        try:
+            if is_adx:
+                adx.dump(file, doc)
+            else:
+                adi.dump(file, doc, 'ADIF Export by DragonLog')
 
-        self.log.info(f'Saved "{file}"')
+            self.log.info(f'Saved "{file}"')
+        except Exception as exc:
+            self.log.exception(exc)
 
     def _build_adif_export_(self, query_str, is_adx=False, include_id=False):
         doc = {
             'HEADER':
                 {
                     'ADIF_VER': '3.1.4',
                     'PROGRAMID': __prog_name__,
@@ -834,16 +888,14 @@
                 remarks = query.value(self.__sql_cols__.index('remarks'))
                 if platform.system() == 'Linux':
                     remarks = remarks.replace('\n', '\r\n')
                 record['NOTES'] = self.replaceNonASCII(remarks)
                 record['NOTES_INTL'] = remarks
             if query.value(self.__sql_cols__.index('comments')):
                 comment = query.value(self.__sql_cols__.index('comments'))
-                if platform.system() == 'Linux':
-                    comment = comment.replace('\n', '\r\n')
                 record['COMMENT'] = self.replaceNonASCII(comment)
                 record['COMMENT_INTL'] = comment
             if query.value(self.__sql_cols__.index('qsl_via')):
                 record['QSL_VIA'] = query.value(self.__sql_cols__.index('qsl_via'))
             if query.value(self.__sql_cols__.index('qsl_path')):
                 record['QSL_SENT_VIA'] = query.value(self.__sql_cols__.index('qsl_path'))
             if query.value(self.__sql_cols__.index('qsl_msg')):
```

### Comparing `DragonLog-1.0/dragonlog/DragonLog_AppSelect.py` & `dragonlog-1.1/dragonlog/DragonLog_AppSelect.py`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/DragonLog_AppSelect_ui.py` & `dragonlog-1.1/dragonlog/DragonLog_AppSelect_ui.py`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/DragonLog_CallBook.py` & `dragonlog-1.1/dragonlog/eQSL.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,183 +1,148 @@
+import re
 import logging
-from dataclasses import dataclass
-from enum import Enum, auto
 
 import requests
-import xmltodict
 from adif_file import adi
 
 from .Logger import Logger
 
 
-class CallBookType(Enum):
-    HamQTH = auto()
-
-
-@dataclass
-class CallBookData:
-    callsign: str
-    nickname: str
-    locator: str
-    qth: str
-    qsl_via: str
-    qsl_bureau: bool
-    qsl_direct: bool
-    qsl_eqsl: bool
-    qsl_lotw: bool
-
-
-class CommunicationException(Exception):
+class EQSLCommunicationException(Exception):
     pass
 
 
-class RequestException(Exception):
+class EQSLRequestException(Exception):
     pass
 
 
-class LoginException(Exception):
+class EQSLLoginException(Exception):
     pass
 
 
-class SessionExpiredException(Exception):
+class EQSLUserCallMatchException(Exception):
     pass
 
 
-class QSORejectedException(Exception):
+class EQSLQSODuplicateException(Exception):
     pass
 
 
-class MissingADIFFieldException(Exception):
+class EQSLADIFFieldException(Exception):
     pass
 
 
-class CallsignNotFoundException(Exception):
-    pass
-
+class EQSL:
+    required_fields = ('QSO_DATE', 'TIME_ON', 'CALL', 'MODE', 'BAND')
+    fields = required_fields + ('FREQ', 'QSLMSG', 'RST_SENT', 'MY_GRIDSQUARE', 'PROP_MODE', 'SUBMODE')
+    image_pattern = re.compile(r'.*<img src="(.*)" alt="" />.*')
+    upl_res_pattern = re.compile(r' *([EWCIR][a-z]*:.*)<BR>')
 
-class CallBook:
-    def __init__(self, callbook_type: CallBookType, program: str, logger: Logger):
-        self.__callbook_type__ = callbook_type
+    def __init__(self, program: str, logger: Logger):
         self.__program_str__ = program
-        self.__session__: str = ''
 
-        self.log = logging.getLogger('CallBook')
-        self.log.setLevel(logger.loglevel)
+        self.log = logging.getLogger('EQSL')
         self.log.addHandler(logger)
+        self.log.setLevel(logger.loglevel)
+        self.logger = logger
         self.log.debug('Initialising...')
 
-    @property
-    def callbook_type(self) -> CallBookType:
-        return self.__callbook_type__
-
-    def login(self, username: str, password: str):
-        match self.__callbook_type__:
-            case CallBookType.HamQTH:
-                self.__session__ = self._hamqth_login_(username, password)
-
-    @property
-    def is_loggedin(self) -> bool:
-        return bool(self.__session__)
-
-    def get_dataset(self, callsign: str) -> CallBookData:
-        try:
-            match self.__callbook_type__:
-                case CallBookType.HamQTH:
-                    return self._hamqth_get_data_(callsign)
-        except SessionExpiredException as exc:
-            self.__session__ = ''
-            raise exc
-
-    @property
-    def required_fields(self) -> tuple:
-        match self.__callbook_type__:
-            case CallBookType.HamQTH:
-                return 'QSO_DATE', 'TIME_ON', 'CALL', 'MODE', 'BAND', 'RST_SENT', 'RST_RCVD'
-            case _:
-                return ()
+    def upload_log(self, username: str, password: str, record: dict) -> bool:
+        self._check_fields_(record)
 
-    def upload_log(self, username: str, password: str, adif_data: dict):
-        for field in self.required_fields:
-            if field not in adif_data['RECORDS'][0]:
-                raise MissingADIFFieldException(field)
+        record = record.copy()
+
+        for field in list(record.keys()):
+            if not field in self.fields:
+                record.pop(field)
+
+        record['ADIF_VER'] = '3.1.4'
+        record['PROGRAMID'] = self.__program_str__
 
-        adif_data = adif_data.copy()
-        adif_data['RECORDS'] = [adif_data['RECORDS'][0]]
+        # Skip header and remove linebreaks
+        data = adi.dumps({'RECORDS': [record]}).replace('\n', ' ')
 
-        match self.__callbook_type__:
-            case CallBookType.HamQTH:
-                return self._hamqth_upload_(username, password, adi.dumps(adif_data, 'ADIF Export by DragonLog'))
+        params = {
+            'ADIFData': 'QSL-Upload ' + data,
+            'EQSL_USER': username,
+            'EQSL_PSWD': password,
+        }
 
-    def _hamqth_get_(self, params: dict):
-        r = requests.get('https://www.hamqth.com/xml.php', params=params)
+        r = requests.get('https://www.eQSL.cc/qslcard/importADIF.cfm', params=params)
 
         if r.status_code == 200:
-            return xmltodict.parse(r.text)
+            for res in re.findall(self.upl_res_pattern, r.text):
+                if 'Error' in res:
+                    if ('No match on eQSL_User/eQSL_Pswd' in res or
+                            'Multiple accounts match eQSL_User/eQSL_Pswd' in res):
+                        raise EQSLUserCallMatchException(res)
+                    elif 'Missing eQSL_User' in res or 'Missing eQSL_Pswd' in res:
+                        raise EQSLLoginException(res)
+                    elif 'Missing ADIFData parameter' in res:
+                        raise EQSLADIFFieldException(res)
+                    else:
+                        raise EQSLRequestException(res)
+                elif 'Warning' in res:
+                    if 'Bad record: Duplicate' in res:
+                        raise EQSLQSODuplicateException(res)
+                    else:
+                        raise EQSLADIFFieldException(res)
+                elif 'Caution' in res:
+                    self.log.warning(f'eQSL result: {res}')
+                elif 'Information' in res:
+                    self.log.info(f'eQSL result: {res}')
+                elif 'Result' in res:
+                    self.log.debug(f'eQSL result: {res}')
+
+            return True
         else:
-            raise CommunicationException(f'HamQTH error: HTTP-Error {r.status_code}')
+            raise EQSLCommunicationException(f'eQSL error: HTTP-Error {r.status_code}')
 
-    def _hamqth_login_(self, username: str, password: str) -> str:
-        try:
-            res = self._hamqth_get_({'u': username, 'p': password})
-        except CommunicationException as exc:
-            raise LoginException(str(exc))
-
-        match res:
-            case {'HamQTH': {'session': {'error': error}}}:
-                raise LoginException(f"HamQTH error: {error}")
-            case {'HamQTH': {'session': {'session_id': session_id}}}:
-                return session_id
-            case _:
-                raise LoginException(f'HamQTH error: Unknown data format {res}')
-
-    def _hamqth_get_data_(self, callsign: str) -> CallBookData:
-        try:
-            self.log.debug(f'Searching {callsign}')
-            res = self._hamqth_get_({'id': self.__session__,
-                                     'prg': self.__program_str__,
-                                     'callsign': callsign})
-        except CommunicationException as exc:
-            raise RequestException(str(exc))
-
-        match res:
-            case {'HamQTH': {'session': {'error': error}}}:
-                if error == 'Session does not exist or expired':
-                    raise SessionExpiredException('HamQTH')
-                elif error == 'Callsign not found':
-                    raise CallsignNotFoundException(callsign)
-                else:
-                    raise RequestException(f"HamQTH error: {error}")
-            case {'HamQTH': {'search': data}}:
-                if data:
-                    return CallBookData(
-                        callsign,
-                        data['nick'] if 'nick' in data else '',
-                        data['grid'] if 'grid' in data else '',
-                        data['qth'] if 'qth' in data else '',
-                        data['qsl_via'] if 'qsl_via' in data else '',
-                        'qsl' in data and data['qsl'] == 'Y',
-                        'qsldirect' in data and data['qsldirect'] == 'Y',
-                        'eqsl' in data and data['eqsl'] == 'Y',
-                        'lotw' in data and data['lotw'] == 'Y',
-                    )
-            case _:
-                raise RequestException(f'HamQTH error: Unknown data format {res}')
-
-    def _hamqth_upload_(self, username: str, password: str, adif: str):
-        data = {
-            'u': username,
-            'p': password,
-            'adif': adif,
-            'prg': self.__program_str__,
-            'cmd': 'insert'
+    def _check_fields_(self, record: dict):
+        for field in self.required_fields:
+            if field not in record:
+                raise EQSLADIFFieldException(field)
+
+    def check_inbox(self, username: str, password: str, record: dict) -> str:
+        self._check_fields_(record)
+
+        params = {
+            'Username': username,
+            'Password': password,
+            'CallsignFrom': record['CALL'],
+            'QSOYear': record['QSO_DATE'][:4],
+            'QSOMonth': record['QSO_DATE'][4:6],
+            'QSODay': record['QSO_DATE'][6:],
+            'QSOHour': record['TIME_ON'][:2],
+            'QSOMinute': record['TIME_ON'][2:4],
+            'QSOBand': record['BAND'],
+            'QSOMode': record['MODE'],
         }
 
-        r = requests.post('https://www.hamqth.com/qso_realtime.php', data=data)
+        r = requests.get('https://www.eQSL.cc/qslcard/GeteQSL.cfm', params=params)
+
+        if r.status_code == 200:
+            if r.text.strip().startswith('Error'):
+                if ('No match on Username/Password for that QSO Date/Time' in r.text or
+                        'overlapping accounts for that QSO Date/Time' in r.text):
+                    raise EQSLUserCallMatchException(r.text.strip())
+                elif ('User is Regular member but must be at least Silver to download mass eQSLs.' in r.text or
+                      'User is Bronze member but must be at least Silver to download mass eQSLs.' in r.text or
+                      'Not Authorized to download mass eQSLs.' in r.text):
+                    raise EQSLLoginException(r.text.strip())
+                else:
+                    raise EQSLRequestException(r.text.strip())
+            else:
+                url_part = re.findall(self.image_pattern, r.text)
+                if url_part:
+                    return 'https://www.eQSL.cc' + url_part[0]
+        else:
+            raise EQSLCommunicationException(f'eQSL error: HTTP-Error {r.status_code}')
+
+    @staticmethod
+    def receive_qsl_card(url: str) -> bytes:
+        r = requests.get(url)
 
         if r.status_code == 200:
-            return
-        elif r.status_code in (400, 500):
-            raise QSORejectedException(r.text)
-        elif r.status_code == 403:
-            raise LoginException(r.text)
+            return r.content
         else:
-            raise CommunicationException(f'HamQTH error: HTTP-Error {r.status_code}')
+            raise EQSLCommunicationException(f'eQSL error: HTTP-Error {r.status_code}')
```

### Comparing `DragonLog-1.0/dragonlog/DragonLog_LoTW.py` & `dragonlog-1.1/dragonlog/LoTW.py`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/DragonLog_MainWindow_ui.py` & `dragonlog-1.1/dragonlog/DragonLog_MainWindow_ui.py`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/DragonLog_QSOForm.py` & `dragonlog-1.1/dragonlog/DragonLog_QSOForm.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 
 import maidenhead
 from PyQt6 import QtWidgets, QtCore, QtGui
 
 from . import DragonLog_QSOForm_ui
 from .Logger import Logger
 from .DragonLog_Settings import Settings
-from .DragonLog_RegEx import REGEX_CALL, REGEX_RSTFIELD, REGEX_LOCATOR, check_format, check_call
-from .DragonLog_CallBook import (CallBook, CallBookType, CallBookData, SessionExpiredException,
-                                 MissingADIFFieldException, LoginException, CallsignNotFoundException)
-from .DragonLog_eQSL import (EQSL, EQSLADIFFieldException, EQSLLoginException,
-                             EQSLRequestException, EQSLUserCallMatchException, EQSLQSODuplicateException)
-from .DragonLog_LoTW import (LoTW, LoTWRequestException, LoTWCommunicationException,
-                             LoTWLoginException, LoTWNoRecordException)
+from .RegEx import REGEX_CALL, REGEX_RSTFIELD, REGEX_LOCATOR, REGEX_TIME, check_format, check_call
+from .CallBook import (HamQTHCallBook, QRZCQCallBook, CallBookType, CallBookData,
+                       SessionExpiredException, MissingADIFFieldException, LoginException, CallsignNotFoundException,
+                       QSORejectedException, CommunicationException)
+from .eQSL import (EQSL, EQSLADIFFieldException, EQSLLoginException,
+                   EQSLRequestException, EQSLUserCallMatchException, EQSLQSODuplicateException)
+from .LoTW import (LoTW, LoTWRequestException, LoTWCommunicationException,
+                   LoTWLoginException, LoTWNoRecordException)
 
 
 class QSOForm(QtWidgets.QDialog, DragonLog_QSOForm_ui.Ui_QSOForm):
     def __init__(self, parent, dragonlog, bands: dict, modes: dict, prop: dict, settings: QtCore.QSettings,
                  settings_form: Settings, cb_channels: dict, hamlib_error: QtWidgets.QLabel, logger: Logger):
         super().__init__(parent)
         self.dragonlog = dragonlog
@@ -36,14 +37,16 @@
         self.modes = modes
         self.prop = prop
         self.prop_trans = dict(zip(prop.values(), prop.keys()))
         self.settings = settings
         self.settings_form = settings_form
         self.qso_id = None
 
+        self.__old_values__ = {}
+
         self.cb_channels = cb_channels
         self.channelComboBox.insertItems(0, ['-'] + list(cb_channels.keys()))
 
         self.bandComboBox.insertItems(0, bands.keys())
 
         self.propComboBox.insertItems(0, self.prop.values())
 
@@ -91,33 +94,36 @@
         self.palette_worked = QtGui.QPalette()
         self.palette_worked.setColor(QtGui.QPalette.ColorGroup.Active, QtGui.QPalette.ColorRole.Base,
                                      QtGui.QColor(204, 204, 255))
 
         self.worked_dialog: QtWidgets.QListWidget = None
         self._create_worked_dlg_()
 
-        self.callbook = CallBook(CallBookType.HamQTH,
-                                 f'{self.dragonlog.programName}-{self.dragonlog.programVersion}',
-                                 self.logger)
+        self.callbook_hamqth = HamQTHCallBook(self.logger,
+                                              f'{self.dragonlog.programName}-{self.dragonlog.programVersion}',
+                                              )
+        self.callbook_qrzcq = QRZCQCallBook(self.logger,
+                                            f'{self.dragonlog.programName}-{self.dragonlog.programVersion}',
+                                            )
+
         self.eqsl = EQSL(self.dragonlog.programName, self.logger)
         self.eqsl_url = ''
 
         self.lotw = LoTW(self.logger)
 
         view_only_widgets = (
             self.qslAccBureauCheckBox,
             self.qslAccDirectCheckBox,
             self.qslAcceQSLCheckBox,
             self.qslAccLoTWCheckBox,
             self.eqslSentCheckBox,
             self.eqslRcvdCheckBox,
+            self.lotwGroupBox,
             self.lotwSentCheckBox,
             self.lotwRcvdCheckBox,
-            self.hamQTHuplRadioButton,
-            self.hamQTHmodRadioButton,
         )
 
         for w in view_only_widgets:
             w.setAttribute(QtCore.Qt.WidgetAttribute.WA_TransparentForMouseEvents)
             w.setFocusPolicy(QtCore.Qt.FocusPolicy.NoFocus)
 
         self.clear()
@@ -148,21 +154,29 @@
             self.worked_dialog.show()
         else:
             self.worked_dialog.hide()
 
     def refreshTime(self):
         if self.autoDateCheckBox.isChecked():
             dt = QtCore.QDateTime.currentDateTimeUtc()
-            self.dateEdit.setDate(dt.date())
-            self.timeEdit.setTime(dt.time())
+            self.dateOffEdit.setDate(dt.date())
+            self.timeOffEdit.setText(dt.time().toString('HH:mm:ss'))
 
     def setStartTimeNow(self):
         dt = QtCore.QDateTime.currentDateTimeUtc()
         self.dateOnEdit.setDate(dt.date())
-        self.timeOnEdit.setTime(dt.time())
+        self.timeOnEdit.setText(dt.time().toString('HH:mm:ss'))
+        self.timeOnChanged(self.timeOnEdit.text())
+
+    def autoDateCBChanged(self, checked: bool):
+        if not checked:
+            self.timeOffEdit.clear()
+            self.timeOffChanged('')
+        else:
+            self.refreshTime()
 
     # noinspection PyBroadException
     def refreshRigData(self):
         if self.settings_form.isRigctldActive() and not self.__change_mode__:
             try:
                 with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
                     s.connect(('127.0.0.1', 4532))
@@ -242,36 +256,40 @@
                         self.hamlib_error.setText(self.tr('rigctld timeout'))
                         self.log.error('rigctld error: timeout')
             except ConnectionRefusedError:
                 self.log.error('Could not connect to rigctld')
                 self.refreshTimer.stop()
 
     def clear(self):
+        self.__old_values__ = {}
         self.qso_id = None
         self.callSignLineEdit.clear()
         self.nameLineEdit.clear()
         self.QTHLineEdit.clear()
         self.locatorLineEdit.clear()
         self.RSTSentLineEdit.setText('59')
         self.RSTRcvdLineEdit.setText('59')
+        self.commentLineEdit.clear()
         self.remarksTextEdit.clear()
         self.powerSpinBox.setValue(0)
 
         self.callSignChanged('')
         self.locatorChanged('')
         self.ownCallSignChanged(self.ownCallSignLineEdit.text())
         self.ownLocatorChanged(self.ownLocatorLineEdit.text())
         self.rstSentChanged(self.RSTSentLineEdit.text())
         self.rstRcvdChanged(self.RSTRcvdLineEdit.text())
 
         dt = QtCore.QDateTime.currentDateTimeUtc()
-        self.dateEdit.setDate(dt.date())
+        self.dateOffEdit.setDate(dt.date())
         self.dateOnEdit.setDate(dt.date())
-        self.timeEdit.setTime(dt.time())
-        self.timeOnEdit.setTime(dt.time())
+        self.timeOffEdit.setText(dt.time().toString('HH:mm:ss'))
+        self.timeOffChanged(self.timeOffEdit.text())
+        self.timeOnEdit.setText('')
+        self.timeOnChanged('')
 
         if bool(self.settings.value('station_cb/cb_by_default', 0)):
             self.bandComboBox.setCurrentText('11m')
 
         if self.bandComboBox.currentIndex() < 0:
             self.bandComboBox.setCurrentIndex(0)
         if self.modeComboBox.currentIndex() < 0:
@@ -299,16 +317,15 @@
         self.eqslDownloadPushButton.setEnabled(False)
 
         self.lotwGroupBox.setChecked(False)
         self.lotwSentCheckBox.setChecked(False)
         self.lotwRcvdCheckBox.setChecked(False)
         self.lotwInboxPushButton.setEnabled(False)
 
-        self.hamQTHGroupBox.setChecked(False)
-        self.hamQTHmodRadioButton.setChecked(True)  # Just not check upload
+        self.hamQTHCheckBox.setChecked(False)
 
         self.toolBox.setCurrentIndex(0)
 
     def reset(self):
         self.autoDateCheckBox.setEnabled(True)
         self.autoDateCheckBox.setChecked(True)
         self.stationGroupBox.setChecked(True)
@@ -348,15 +365,16 @@
         self.modeComboBox.clear()
         if band == '11m':
             self.modeComboBox.insertItems(0, self.modes['CB'].keys())
             self.powerSpinBox.setMaximum(12)
             self.channelComboBox.setVisible(True)
             self.channelLabel.setVisible(True)
             self.freqDoubleSpinBox.setEnabled(False)
-            self.searchCallbookPushButton.setEnabled(False)
+            self.searchHamQTHPushButton.setEnabled(False)
+            self.searchQRZCQPushButton.setEnabled(False)
             self.uploadPushButton.setEnabled(False)
             self.qslPage.setEnabled(False)
             self.channelComboBox.setCurrentIndex(-1)
             self.channelComboBox.setCurrentIndex(0)
 
             if self.stationGroupBox.isChecked():
                 self.radioLineEdit.setText(self.settings.value('station_cb/radio', ''))
@@ -367,15 +385,16 @@
         else:
             self.modeComboBox.insertItems(0, self.modes['AFU'].keys())
             self.modeComboBox.setCurrentIndex(0)
             self.powerSpinBox.setMaximum(1000)
             self.channelComboBox.setVisible(False)
             self.channelLabel.setVisible(False)
             self.freqDoubleSpinBox.setEnabled(True)
-            self.searchCallbookPushButton.setEnabled(True)
+            self.searchHamQTHPushButton.setEnabled(True)
+            self.searchQRZCQPushButton.setEnabled(True)
             self.uploadPushButton.setEnabled(True)
             self.qslPage.setEnabled(True)
 
             if self.stationGroupBox.isChecked():
                 self.radioLineEdit.setText(self.settings.value('station/radio', ''))
                 self.antennaLineEdit.setText(self.settings.value('station/antenna', ''))
 
@@ -387,15 +406,15 @@
         self.submodeComboBox.setEnabled(True)
         if self.bandComboBox.currentText() == '11m':
             if mode in self.modes['CB'] and self.modes['CB'][mode]:
                 self.submodeComboBox.insertItems(0, [''] + self.modes['CB'][mode])
             else:
                 self.submodeComboBox.setEnabled(False)
         else:
-            if mode in self.modes['AFU'] and  self.modes['AFU'][mode]:
+            if mode in self.modes['AFU'] and self.modes['AFU'][mode]:
                 self.submodeComboBox.insertItems(0, [''] + self.modes['AFU'][mode])
             else:
                 self.submodeComboBox.setEnabled(False)
 
     def stationChanged(self, checked):
         if checked:
             self.ownQTHLineEdit.setText(self.settings.value('station/QTH', ''))
@@ -480,14 +499,30 @@
         if not txt:
             self.ownLocatorLineEdit.setPalette(self.palette_empty)
         elif check_format(REGEX_LOCATOR, txt):
             self.ownLocatorLineEdit.setPalette(self.palette_ok)
         else:
             self.ownLocatorLineEdit.setPalette(self.palette_faulty)
 
+    def timeOnChanged(self, txt):
+        if not txt:
+            self.timeOnEdit.setPalette(self.palette_empty)
+        elif check_format(REGEX_TIME, txt):
+            self.timeOnEdit.setPalette(self.palette_ok)
+        else:
+            self.timeOnEdit.setPalette(self.palette_faulty)
+
+    def timeOffChanged(self, txt):
+        if not txt:
+            self.timeOffEdit.setPalette(self.palette_empty)
+        elif check_format(REGEX_TIME, txt):
+            self.timeOffEdit.setPalette(self.palette_ok)
+        else:
+            self.timeOffEdit.setPalette(self.palette_faulty)
+
     def calc_distance(self, mh_pos1: str, mh_pos2: str):
         # noinspection PyBroadException
         try:
             pos1 = maidenhead.to_location(mh_pos1, True)
             pos2 = maidenhead.to_location(mh_pos2, True)
 
             mlat = math.radians(pos1[0])
@@ -501,21 +536,25 @@
             self.log.warning(f'Exception calcing distance between "{mh_pos1}" amd "{mh_pos2}"')
             return 0
 
     @property
     def values(self) -> tuple:
         """Retreiving all values from the form"""
 
-        if not self.__change_mode__:
-            if self.autoDateCheckBox.isChecked():
-                date_time_off = QtCore.QDateTime.currentDateTimeUtc().toString('yyyy-MM-dd HH:mm:ss')
-            else:
-                date_time_off = self.dateEdit.text() + ' ' + self.timeEdit.text()
+        date_time_off = ''
+        if check_format(REGEX_TIME, self.timeOffEdit.text()):
+            date_time_off = self.dateOffEdit.text() + ' ' + self.timeOffEdit.text()
+        else:
+            self.log.warning(f'Wrong time format for end time')
+
+        if check_format(REGEX_TIME, self.timeOnEdit.text()):
+            date_time_on = self.dateOnEdit.text() + ' ' + self.timeOnEdit.text()
         else:
-            date_time_off = self.dateEdit.text() + ' ' + self.timeEdit.text()
+            self.log.warning(f'Wrong time format for start time. Fallback to current date time.')
+            date_time_on = QtCore.QDateTime.currentDateTimeUtc().toString('yyyy-MM-dd HH:mm:ss')
 
         band = self.bandComboBox.currentText()
 
         prop = ''
         if self.propComboBox.currentText():
             prop = self.prop_trans[self.propComboBox.currentText()]
 
@@ -541,23 +580,16 @@
 
         lotw_sent = 'N'
         lotw_rcvd = 'N'
         if self.lotwGroupBox.isChecked():
             lotw_sent = 'Y' if self.lotwSentCheckBox.isChecked() else 'R'
             lotw_rcvd = 'Y' if self.lotwRcvdCheckBox.isChecked() else 'R'
 
-        hamqth_state = 'N'
-        if self.hamQTHGroupBox.isChecked():
-            if self.hamQTHuplRadioButton.isChecked():
-                hamqth_state = 'Y'
-            if self.hamQTHmodRadioButton.isChecked():
-                hamqth_state = 'M'
-
         return (
-            self.dateOnEdit.text() + ' ' + self.timeOnEdit.text(),
+            date_time_on,
             date_time_off,
             self.ownCallSignLineEdit.text().upper() if band != '11m' else self.ownCallSignLineEdit.text(),
             self.callSignLineEdit.text().upper() if band != '11m' else self.callSignLineEdit.text(),
             self.nameLineEdit.text(),
             self.QTHLineEdit.text(),
             self.locatorLineEdit.text(),
             self.RSTSentLineEdit.text(),
@@ -572,43 +604,53 @@
             prop,
             self.ownNameLineEdit.text(),
             self.ownQTHLineEdit.text(),
             self.ownLocatorLineEdit.text(),
             self.radioLineEdit.text(),
             self.antennaLineEdit.text(),
             self.remarksTextEdit.toPlainText().strip(),
-            self.commentsTextEdit.toPlainText().strip(),
+            self.commentLineEdit.text().strip(),
             self.calc_distance(self.locatorLineEdit.text(), self.ownLocatorLineEdit.text()),
             qsl_via,
             qsl_path,
             qsl_msg,
             qsl_sent,
             qsl_rcvd,
             eqsl_sent,
             eqsl_rcvd,
             lotw_sent,
             lotw_rcvd,
-            hamqth_state,
+            'Y' if self.hamQTHCheckBox.isChecked() else 'N',
         )
 
     @values.setter
     def values(self, values: dict):
         """Set all form values"""
+        self.__old_values__ = values.copy()
 
         self.qso_id = values['id']
-        date, time = values['date_time'].split()
-        self.dateOnEdit.setDate(QtCore.QDate.fromString(date, 'yyyy-MM-dd'))
-        self.timeOnEdit.setTime(QtCore.QTime.fromString(time))
+        time_on = ''
+        if values['date_time']:
+            try:
+                date_on, time_on = values['date_time'].split()
+                self.dateOnEdit.setDate(QtCore.QDate.fromString(date_on, 'yyyy-MM-dd'))
+            except ValueError:
+                self.log.error(f'Wrong date time format for start time in QSO #{self.qso_id}')
+        self.timeOnEdit.setText(time_on)
+        self.timeOnChanged(self.timeOnEdit.text())
 
+        time_off = ''
         if values['date_time_off']:
-            date_off, time_off = values['date_time_off'].split()
-        else:
-            date_off, time_off = date, time
-        self.dateEdit.setDate(QtCore.QDate.fromString(date_off, 'yyyy-MM-dd'))
-        self.timeEdit.setTime(QtCore.QTime.fromString(time_off))
+            try:
+                date_off, time_off = values['date_time_off'].split()
+                self.dateOffEdit.setDate(QtCore.QDate.fromString(date_off, 'yyyy-MM-dd'))
+            except ValueError:
+                self.log.error(f'Wrong date time format for end time in QSO #{self.qso_id}')
+        self.timeOffEdit.setText(time_off)
+        self.timeOffChanged(self.timeOffEdit.text())
 
         self.ownCallSignLineEdit.setText(values['own_callsign'])
         self.callSignLineEdit.setText(values['call_sign'])
         self.nameLineEdit.setText(values['name'])
         self.QTHLineEdit.setText(values['qth'])
         self.locatorLineEdit.setText(values['locator'])
         self.RSTSentLineEdit.setText(values['rst_sent'])
@@ -650,15 +692,15 @@
 
         self.ownNameLineEdit.setText(values['own_name'])
         self.ownQTHLineEdit.setText(values['own_qth'])
         self.ownLocatorLineEdit.setText(values['own_locator'])
         self.radioLineEdit.setText(values['radio'])
         self.antennaLineEdit.setText(values['antenna'])
         self.remarksTextEdit.setText(values['remarks'])
-        self.commentsTextEdit.setText(values['comments'])
+        self.commentLineEdit.setText(values['comments'].replace('\n', ' ').replace('\r', ''))
 
         if (values['qsl_sent'] in ('R', 'Y') or values['qsl_rcvd'] in ('R', 'Y') or
                 values['eqsl_sent'] in ('R', 'Y') or values['eqsl_rcvd'] in ('R', 'Y')):
 
             self.qslViaLineEdit.setText(values['qsl_via'])
             self.qslBureauRadioButton.setChecked(values['qsl_path'] == 'B')
             self.qslDirectRadioButton.setChecked(values['qsl_path'] == 'D')
@@ -680,40 +722,41 @@
         if values['lotw_sent'] in ('R', 'Y') or values['lotw_rcvd'] in ('R', 'Y'):
             self.lotwGroupBox.setChecked(True)
             self.lotwSentCheckBox.setChecked(values['lotw_sent'] == 'Y')
             self.lotwRcvdCheckBox.setChecked(values['lotw_rcvd'] == 'Y')
             self.lotwInboxPushButton.setEnabled(True)
 
         match values['hamqth']:
-            case 'Y':
-                self.hamQTHGroupBox.setChecked(True)
-                self.hamQTHuplRadioButton.setChecked(True)
-            case 'M':
-                self.hamQTHGroupBox.setChecked(True)
-                self.hamQTHmodRadioButton.setChecked(True)
+            case 'Y' | 'M':
+                self.hamQTHCheckBox.setChecked(True)
             case _:
-                self.hamQTHGroupBox.setChecked(False)
-                self.hamQTHmodRadioButton.setChecked(True)  # Just don't check uploaded
+                self.hamQTHCheckBox.setChecked(False)
+
+    def searchHamQTH(self):
+        self.searchCallbook(self.callbook_hamqth)
 
-    def searchCallbook(self):
+    def searchQRZCQ(self):
+        self.searchCallbook(self.callbook_qrzcq)
+
+    def searchCallbook(self, callbook):
         try:
-            if not self.callbook.is_loggedin:
-                self.callbook.login(self.settings.value('callbook/username', ''),
-                                    self.settings_form.callbookPassword())
-                self.log.info('Logged into callbook')
+            if not callbook.is_loggedin:
+                callbook.login(self.settings.value(f'callbook/{callbook.callbook_type.name}_user', ''),
+                               self.settings_form.callbookPassword(callbook.callbook_type))
+                self.log.info(f'Logged into callbook {callbook.callbook_type.name}')
 
             data: CallBookData = None
             for _ in range(2):
                 try:
-                    data = self.callbook.get_dataset(self.callSignLineEdit.text())
+                    data = callbook.get_dataset(self.callSignLineEdit.text())
                     break
                 except SessionExpiredException:
                     self.log.debug('Callbook session expired')
-                    self.callbook.login(self.settings.value('callbook/username', ''),
-                                        self.settings_form.callbookPassword())
+                    callbook.login(self.settings.value(f'callbook/{callbook.callbook_type.name}_user', ''),
+                                   self.settings_form.callbookPassword(callbook.callbook_type))
 
             if data:
                 if data.nickname and not self.nameLineEdit.text().strip():
                     self.nameLineEdit.setText(data.nickname)
                 if data.locator and not self.locatorLineEdit.text().strip():
                     self.locatorLineEdit.setText(data.locator)
                     self.locatorChanged(data.locator)
@@ -723,106 +766,118 @@
                     self.qslViaLineEdit.setText(data.qsl_via)
 
                 self.qslAccBureauCheckBox.setChecked(data.qsl_bureau)
                 self.qslAccDirectCheckBox.setChecked(data.qsl_direct)
                 self.qslAcceQSLCheckBox.setChecked(data.qsl_eqsl)
                 self.qslAccLoTWCheckBox.setChecked(data.qsl_lotw)
 
-                self.log.info(f'Fetched data from callbook {self.callbook.callbook_type.name}')
+                self.log.info(f'Fetched data from callbook {callbook.callbook_type.name}')
         except LoginException:
             QtWidgets.QMessageBox.warning(self, self.tr('Callbook search error'),
                                           self.tr('Login failed for user') + ': ' + self.settings.value(
-                                              'callbook/username', ''))
+                                              f'callbook/{callbook.callbook_type.name}_user', ''))
         except CallsignNotFoundException as exc:
             QtWidgets.QMessageBox.information(self, self.tr('Callbook search result'),
                                               self.tr('Callsign not found') + f': {exc.args[0]}')
         except Exception as exc:
+            self.log.exception(exc)
             QtWidgets.QMessageBox.warning(self, self.tr('Callbook search error'),
                                           self.tr('During callbook search an error occured') + f':\n{exc}')
 
     def saveLog(self):
-        self.hamQTHmodRadioButton.setChecked(True)
+        if self.__old_values__['hamqth'] in ('Y', 'M'):
+            self.hamQTHCheckBox.setChecked(True)
 
         if self.__change_mode__:
             self.dragonlog.updateQSO(self.qso_id)
         else:
             self.dragonlog.fetchQSO()
 
         self.toolBox.setCurrentIndex(0)
         self.clear()
 
     def uploadLog(self):
-        if self.hamQTHGroupBox.isChecked() or self.eqslGroupBox.isChecked():
-            record = self._build_record_()
-
-            adif_doc = {'HEADER':
-                {
-                    'ADIF_VER': '3.1.4',
-                    'PROGRAMID': self.dragonlog.programName,
-                    'PROGRAMVERSION': self.dragonlog.programVersion,
-                    'CREATED_TIMESTAMP': QtCore.QDateTime.currentDateTimeUtc().toString(
-                        'yyyyMMdd HHmmss')
-                },
-                'RECORDS': [record]}
+        record = self._build_record_()
 
-            if self.hamQTHGroupBox.isChecked() and not self.hamQTHuplRadioButton.isChecked():
-                try:
-                    self.callbook.upload_log(self.settings.value('callbook/username', ''),
-                                             self.settings_form.callbookPassword(),
-                                             adif_doc)
-
-                    self.hamQTHuplRadioButton.setChecked(True)
-                    self.log.info(f'Uploaded log to {self.callbook.callbook_type.name}')
-                except LoginException:
-                    QtWidgets.QMessageBox.warning(self, self.tr('Upload log error'),
-                                                  self.tr('Login failed for user') + ': ' + self.settings.value(
-                                                      'callbook/username', ''))
-                except MissingADIFFieldException as exc:
-                    QtWidgets.QMessageBox.warning(self, self.tr('Upload log error'),
-                                                  self.tr('A field is missing for log upload') + f':\n"{exc.args[0]}"')
+        adif_doc = {'HEADER':
+            {
+                'ADIF_VER': '3.1.4',
+                'PROGRAMID': self.dragonlog.programName,
+                'PROGRAMVERSION': self.dragonlog.programVersion,
+                'CREATED_TIMESTAMP': QtCore.QDateTime.currentDateTimeUtc().toString(
+                    'yyyyMMdd HHmmss')
+            },
+            'RECORDS': [record]}
+
+        if self.hamQTHCheckBox.isChecked() and self.__old_values__['hamqth'] not in ('Y', 'M'):
+            logbook = HamQTHCallBook(self.logger,
+                                     f'{self.dragonlog.programName}-{self.dragonlog.programVersion}',
+                                     )
+            try:
+                logbook.upload_log(self.settings.value(f'callbook/HamQTH_user', ''),
+                                   self.settings_form.callbookPassword(CallBookType.HamQTH),
+                                   adif_doc)
+
+                self.log.info(f'Uploaded log to HamQTH')
+            except LoginException:
+                QtWidgets.QMessageBox.warning(self, self.tr('Upload log error'),
+                                              self.tr('Login to HamQTH failed for user') + ': ' + self.settings.value(
+                                                  f'callbook/HamQTH_user', ''))
+            except QSORejectedException:
+                self.hamQTHCheckBox.setChecked(True)
+                QtWidgets.QMessageBox.warning(self, self.tr('Upload log error'),
+                                              self.tr('QSO rejected on HamQTH'))
+            except MissingADIFFieldException as exc:
+                QtWidgets.QMessageBox.warning(self, self.tr('Upload log error'),
+                                              self.tr('A field is missing for log upload to HamQTH') +
+                                              f':\n"{exc.args[0]}"')
+            except CommunicationException as exc:
+                QtWidgets.QMessageBox.warning(self, self.tr('Upload log error'),
+                                              self.tr('An error occured on uploading to HamQTH') + f':\n"{exc}"')
 
-            if self.eqslGroupBox.isChecked() and not self.eqslSentCheckBox.isChecked():
-                try:
-                    self.eqsl.upload_log(self.settings.value('eqsl/username', ''),
-                                         self.settings_form.eqslPassword(),
-                                         record)
-
-                    self.eqslSentCheckBox.setChecked(True)
-                    self.log.info(f'Uploaded log to eQSL')
-                except EQSLLoginException:
-                    QtWidgets.QMessageBox.warning(self, self.tr('Upload eQSL error'),
-                                                  self.tr('Login failed for user') + ': ' + self.settings.value(
-                                                      'eqsl/username', ''))
-                except EQSLADIFFieldException as exc:
-                    QtWidgets.QMessageBox.warning(self, self.tr('Upload eQSL error'),
-                                                  self.tr('A field is missing for log upload') + f':\n"{exc.args[0]}"')
-                except EQSLQSODuplicateException:
-                    QtWidgets.QMessageBox.warning(self, self.tr('Upload eQSL error'),
-                                                  self.tr('The QSO is a duplicate'))
-                except EQSLUserCallMatchException:
-                    QtWidgets.QMessageBox.warning(self, self.tr('Upload eQSL error'),
-                                                  self.tr('User call does not match') + ': ' + self.settings.value(
-                                                      'eqsl/username', ''))
-                except EQSLRequestException as exc:
-                    QtWidgets.QMessageBox.information(self, self.tr('Upload eQSL error'),
-                                                      self.tr('Error on upload') + f':\n"{exc.args[0]}"')
+        if self.eqslGroupBox.isChecked() and not self.eqslSentCheckBox.isChecked():
+            try:
+                self.eqsl.upload_log(self.settings.value('eqsl/username', ''),
+                                     self.settings_form.eqslPassword(),
+                                     record)
+
+                self.eqslSentCheckBox.setChecked(True)
+                self.log.info(f'Uploaded log to eQSL')
+            except EQSLLoginException:
+                QtWidgets.QMessageBox.warning(self, self.tr('Upload eQSL error'),
+                                              self.tr('Login failed for user') + ': ' + self.settings.value(
+                                                  'eqsl/username', ''))
+            except EQSLADIFFieldException as exc:
+                QtWidgets.QMessageBox.warning(self, self.tr('Upload eQSL error'),
+                                              self.tr('A field is missing for log upload') + f':\n"{exc.args[0]}"')
+            except EQSLQSODuplicateException:
+                self.eqslSentCheckBox.setChecked(True)
+                QtWidgets.QMessageBox.warning(self, self.tr('Upload eQSL error'),
+                                              self.tr('The QSO is a duplicate'))
+            except EQSLUserCallMatchException:
+                QtWidgets.QMessageBox.warning(self, self.tr('Upload eQSL error'),
+                                              self.tr('User call does not match') + ': ' + self.settings.value(
+                                                  'eqsl/username', ''))
+            except EQSLRequestException as exc:
+                QtWidgets.QMessageBox.information(self, self.tr('Upload eQSL error'),
+                                                  self.tr('Error on upload') + f':\n"{exc.args[0]}"')
 
         if self.__change_mode__:
             self.dragonlog.updateQSO(self.qso_id)
         else:
             self.dragonlog.fetchQSO()
 
         self.toolBox.setCurrentIndex(0)
         self.clear()
 
     def _build_record_(self):
         record = {
             'QSO_DATE': self.dateOnEdit.text().replace('-', ''),
             'TIME_ON': self.timeOnEdit.text().replace(':', ''),
-            'TIME_OFF': self.timeEdit.text().replace(':', ''),
+            'TIME_OFF': self.timeOffEdit.text().replace(':', ''),
             'BAND': self.bandComboBox.currentText(),
             'MODE': self.modeComboBox.currentText(),
         }
         if self.ownCallSignLineEdit.text():
             record['STATION_CALLSIGN'] = self.ownCallSignLineEdit.text().upper()
         if self.callSignLineEdit.text():
             record['CALL'] = self.callSignLineEdit.text().upper()
@@ -841,36 +896,36 @@
         if self.powerSpinBox.value() > 0:
             record['TX_PWR'] = self.powerSpinBox.value()
         if self.ownLocatorLineEdit.text():
             record['MY_GRIDSQUARE'] = self.ownLocatorLineEdit.text()
         if self.remarksTextEdit.toPlainText().strip() and not bool(
                 self.settings.value('imp_exp/own_notes_adif', 0)):
             record['NOTES'] = self.dragonlog.replaceNonASCII(self.remarksTextEdit.toPlainText().strip())
-        if self.commentsTextEdit.toPlainText().strip():
-            record['COMMENTS'] = self.dragonlog.replaceNonASCII(self.commentsTextEdit.toPlainText().strip())
+        if self.commentLineEdit.text().strip():
+            record['COMMENT'] = self.dragonlog.replaceNonASCII(self.commentLineEdit.text().strip())
         if self.qslMessageTextEdit.toPlainText().strip():
             record['QSLMSG'] = self.dragonlog.replaceNonASCII(self.qslMessageTextEdit.toPlainText().strip())
 
         return record
 
     def eqslCheckInbox(self, only_url: bool = False):
         try:
             res = self.eqsl.check_inbox(self.settings.value('eqsl/username', ''),
                                         self.settings_form.eqslPassword(),
                                         self._build_record_())
             if res:
                 self.eqsl_url = res
                 self.eqslLinkLabel.setText(f'''<html>
-                <head/>
-                <body>
-                <p><a href="{res}">
-                <span style=" text-decoration: underline; color:#0000ff;">{self.tr('Link to eQSL Card')}</span>
-                </a></p>
-                </body>
-                </html>''')
+                    <head/>
+                    <body>
+                    <p><a href="{res}">
+                    <span style=" text-decoration: underline; color:#0000ff;">{self.tr('Link to eQSL Card')}</span>
+                    </a></p>
+                    </body>
+                    </html>''')
                 self.log.debug(f'eQSL available at "{res}"')
 
                 if not only_url:
                     self.eqslRcvdCheckBox.setChecked(True)
                     self.eqslLinkLabel.setEnabled(True)
                     self.eqslDownloadPushButton.setEnabled(True)
```

### Comparing `DragonLog-1.0/dragonlog/DragonLog_QSOForm_ui.py` & `dragonlog-1.1/dragonlog/DragonLog_QSOForm_ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         QSOForm.setSizePolicy(sizePolicy)
         QSOForm.setMinimumSize(QtCore.QSize(500, 600))
         self.verticalLayout = QtWidgets.QVBoxLayout(QSOForm)
         self.verticalLayout.setObjectName("verticalLayout")
         self.toolBox = QtWidgets.QToolBox(parent=QSOForm)
         self.toolBox.setObjectName("toolBox")
         self.mainPage = QtWidgets.QWidget()
-        self.mainPage.setGeometry(QtCore.QRect(0, 0, 482, 490))
+        self.mainPage.setGeometry(QtCore.QRect(0, -3, 465, 493))
         self.mainPage.setObjectName("mainPage")
         self.verticalLayout_5 = QtWidgets.QVBoxLayout(self.mainPage)
         self.verticalLayout_5.setObjectName("verticalLayout_5")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout()
         self.verticalLayout_2.setObjectName("verticalLayout_2")
         self.gridLayout_3 = QtWidgets.QGridLayout()
         self.gridLayout_3.setObjectName("gridLayout_3")
@@ -40,20 +40,21 @@
         self.gridLayout_3.addWidget(self.callSignLineEdit, 0, 0, 1, 1)
         self.QTHLineEdit = QtWidgets.QLineEdit(parent=self.mainPage)
         self.QTHLineEdit.setObjectName("QTHLineEdit")
         self.gridLayout_3.addWidget(self.QTHLineEdit, 1, 0, 1, 1)
         self.locatorLineEdit = QtWidgets.QLineEdit(parent=self.mainPage)
         self.locatorLineEdit.setObjectName("locatorLineEdit")
         self.gridLayout_3.addWidget(self.locatorLineEdit, 1, 1, 1, 1)
-        self.searchCallbookPushButton = QtWidgets.QPushButton(parent=self.mainPage)
-        self.searchCallbookPushButton.setObjectName("searchCallbookPushButton")
-        self.gridLayout_3.addWidget(self.searchCallbookPushButton, 0, 2, 1, 1)
+        self.searchHamQTHPushButton = QtWidgets.QPushButton(parent=self.mainPage)
+        self.searchHamQTHPushButton.setObjectName("searchHamQTHPushButton")
+        self.gridLayout_3.addWidget(self.searchHamQTHPushButton, 0, 2, 1, 1)
+        self.searchQRZCQPushButton = QtWidgets.QPushButton(parent=self.mainPage)
+        self.searchQRZCQPushButton.setObjectName("searchQRZCQPushButton")
+        self.gridLayout_3.addWidget(self.searchQRZCQPushButton, 1, 2, 1, 1)
         self.verticalLayout_2.addLayout(self.gridLayout_3)
-        self.horizontalLayout = QtWidgets.QHBoxLayout()
-        self.horizontalLayout.setObjectName("horizontalLayout")
         self.horizontalLayout_9 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_9.setObjectName("horizontalLayout_9")
         self.label = QtWidgets.QLabel(parent=self.mainPage)
         self.label.setObjectName("label")
         self.horizontalLayout_9.addWidget(self.label)
         self.RSTSentLineEdit = QtWidgets.QLineEdit(parent=self.mainPage)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Preferred)
@@ -84,16 +85,15 @@
         self.horizontalLayout_9.addWidget(self.powerLabel)
         self.powerSpinBox = QtWidgets.QSpinBox(parent=self.mainPage)
         self.powerSpinBox.setEnabled(True)
         self.powerSpinBox.setMinimum(0)
         self.powerSpinBox.setMaximum(1000)
         self.powerSpinBox.setObjectName("powerSpinBox")
         self.horizontalLayout_9.addWidget(self.powerSpinBox)
-        self.horizontalLayout.addLayout(self.horizontalLayout_9)
-        self.verticalLayout_2.addLayout(self.horizontalLayout)
+        self.verticalLayout_2.addLayout(self.horizontalLayout_9)
         self.horizontalLayout_8 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_8.setObjectName("horizontalLayout_8")
         self.bandComboBox = QtWidgets.QComboBox(parent=self.mainPage)
         self.bandComboBox.setMinimumContentsLength(4)
         self.bandComboBox.setObjectName("bandComboBox")
         self.horizontalLayout_8.addWidget(self.bandComboBox)
         spacerItem1 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
@@ -175,72 +175,65 @@
         self.antennaLineEdit.setEnabled(False)
         self.antennaLineEdit.setObjectName("antennaLineEdit")
         self.horizontalLayout_6.addWidget(self.antennaLineEdit)
         self.verticalLayout_4.addLayout(self.horizontalLayout_6)
         self.verticalLayout_2.addWidget(self.stationGroupBox)
         self.gridLayout = QtWidgets.QGridLayout()
         self.gridLayout.setObjectName("gridLayout")
-        self.dateEdit = QtWidgets.QDateEdit(parent=self.mainPage)
-        self.dateEdit.setEnabled(False)
-        self.dateEdit.setCalendarPopup(True)
-        self.dateEdit.setTimeSpec(QtCore.Qt.TimeSpec.UTC)
-        self.dateEdit.setObjectName("dateEdit")
-        self.gridLayout.addWidget(self.dateEdit, 1, 1, 1, 1)
-        self.dateOnEdit = QtWidgets.QDateEdit(parent=self.mainPage)
-        self.dateOnEdit.setCalendarPopup(True)
-        self.dateOnEdit.setObjectName("dateOnEdit")
-        self.gridLayout.addWidget(self.dateOnEdit, 0, 1, 1, 1)
         self.timeNowPushButton = QtWidgets.QPushButton(parent=self.mainPage)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Maximum, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.timeNowPushButton.sizePolicy().hasHeightForWidth())
         self.timeNowPushButton.setSizePolicy(sizePolicy)
         self.timeNowPushButton.setObjectName("timeNowPushButton")
         self.gridLayout.addWidget(self.timeNowPushButton, 0, 3, 1, 1)
         self.label_4 = QtWidgets.QLabel(parent=self.mainPage)
         self.label_4.setObjectName("label_4")
         self.gridLayout.addWidget(self.label_4, 1, 0, 1, 1)
-        self.timeEdit = QtWidgets.QTimeEdit(parent=self.mainPage)
-        self.timeEdit.setEnabled(False)
-        self.timeEdit.setCurrentSectionIndex(1)
-        self.timeEdit.setTimeSpec(QtCore.Qt.TimeSpec.UTC)
-        self.timeEdit.setObjectName("timeEdit")
-        self.gridLayout.addWidget(self.timeEdit, 1, 2, 1, 1)
-        self.timeOnEdit = QtWidgets.QTimeEdit(parent=self.mainPage)
+        self.timeOnEdit = QtWidgets.QLineEdit(parent=self.mainPage)
         self.timeOnEdit.setObjectName("timeOnEdit")
         self.gridLayout.addWidget(self.timeOnEdit, 0, 2, 1, 1)
-        self.label_3 = QtWidgets.QLabel(parent=self.mainPage)
-        self.label_3.setObjectName("label_3")
-        self.gridLayout.addWidget(self.label_3, 0, 0, 1, 1)
         self.autoDateCheckBox = QtWidgets.QCheckBox(parent=self.mainPage)
         self.autoDateCheckBox.setChecked(True)
         self.autoDateCheckBox.setObjectName("autoDateCheckBox")
         self.gridLayout.addWidget(self.autoDateCheckBox, 1, 3, 1, 1)
         spacerItem3 = QtWidgets.QSpacerItem(200, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.gridLayout.addItem(spacerItem3, 0, 4, 1, 1)
+        self.label_3 = QtWidgets.QLabel(parent=self.mainPage)
+        self.label_3.setObjectName("label_3")
+        self.gridLayout.addWidget(self.label_3, 0, 0, 1, 1)
+        self.dateOnEdit = QtWidgets.QDateEdit(parent=self.mainPage)
+        self.dateOnEdit.setCalendarPopup(True)
+        self.dateOnEdit.setObjectName("dateOnEdit")
+        self.gridLayout.addWidget(self.dateOnEdit, 0, 1, 1, 1)
+        self.dateOffEdit = QtWidgets.QDateEdit(parent=self.mainPage)
+        self.dateOffEdit.setEnabled(False)
+        self.dateOffEdit.setCalendarPopup(True)
+        self.dateOffEdit.setTimeSpec(QtCore.Qt.TimeSpec.UTC)
+        self.dateOffEdit.setObjectName("dateOffEdit")
+        self.gridLayout.addWidget(self.dateOffEdit, 1, 1, 1, 1)
         spacerItem4 = QtWidgets.QSpacerItem(200, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.gridLayout.addItem(spacerItem4, 1, 4, 1, 1)
+        self.timeOffEdit = QtWidgets.QLineEdit(parent=self.mainPage)
+        self.timeOffEdit.setEnabled(False)
+        self.timeOffEdit.setObjectName("timeOffEdit")
+        self.gridLayout.addWidget(self.timeOffEdit, 1, 2, 1, 1)
         self.gridLayout.setColumnStretch(1, 1)
         self.gridLayout.setColumnStretch(2, 1)
         self.gridLayout.setColumnStretch(3, 2)
         self.verticalLayout_2.addLayout(self.gridLayout)
-        self.horizontalLayout_4 = QtWidgets.QHBoxLayout()
-        self.horizontalLayout_4.setObjectName("horizontalLayout_4")
-        self.commentsTextEdit = QtWidgets.QTextEdit(parent=self.mainPage)
-        self.commentsTextEdit.setAcceptRichText(False)
-        self.commentsTextEdit.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByKeyboard|QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextBrowserInteraction|QtCore.Qt.TextInteractionFlag.TextEditable|QtCore.Qt.TextInteractionFlag.TextEditorInteraction|QtCore.Qt.TextInteractionFlag.TextSelectableByKeyboard|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
-        self.commentsTextEdit.setObjectName("commentsTextEdit")
-        self.horizontalLayout_4.addWidget(self.commentsTextEdit)
+        self.commentLineEdit = QtWidgets.QLineEdit(parent=self.mainPage)
+        self.commentLineEdit.setObjectName("commentLineEdit")
+        self.verticalLayout_2.addWidget(self.commentLineEdit)
         self.remarksTextEdit = QtWidgets.QTextEdit(parent=self.mainPage)
         self.remarksTextEdit.setAcceptRichText(False)
         self.remarksTextEdit.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByKeyboard|QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextBrowserInteraction|QtCore.Qt.TextInteractionFlag.TextEditable|QtCore.Qt.TextInteractionFlag.TextEditorInteraction|QtCore.Qt.TextInteractionFlag.TextSelectableByKeyboard|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.remarksTextEdit.setObjectName("remarksTextEdit")
-        self.horizontalLayout_4.addWidget(self.remarksTextEdit)
-        self.verticalLayout_2.addLayout(self.horizontalLayout_4)
+        self.verticalLayout_2.addWidget(self.remarksTextEdit)
         self.verticalLayout_5.addLayout(self.verticalLayout_2)
         self.toolBox.addItem(self.mainPage, "")
         self.qslPage = QtWidgets.QWidget()
         self.qslPage.setGeometry(QtCore.QRect(0, 0, 482, 490))
         self.qslPage.setObjectName("qslPage")
         self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.qslPage)
         self.verticalLayout_6.setObjectName("verticalLayout_6")
@@ -356,29 +349,24 @@
         self.lotwInboxPushButton = QtWidgets.QPushButton(parent=self.lotwGroupBox)
         self.lotwInboxPushButton.setObjectName("lotwInboxPushButton")
         self.horizontalLayout_13.addWidget(self.lotwInboxPushButton)
         spacerItem9 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout_13.addItem(spacerItem9)
         self.verticalLayout_7.addWidget(self.lotwGroupBox)
         self.verticalLayout_6.addWidget(self.qslGroupBox)
-        self.hamQTHGroupBox = QtWidgets.QGroupBox(parent=self.qslPage)
-        self.hamQTHGroupBox.setCheckable(True)
-        self.hamQTHGroupBox.setChecked(False)
-        self.hamQTHGroupBox.setObjectName("hamQTHGroupBox")
-        self.horizontalLayout_3 = QtWidgets.QHBoxLayout(self.hamQTHGroupBox)
+        self.callbookGroupBox = QtWidgets.QGroupBox(parent=self.qslPage)
+        self.callbookGroupBox.setObjectName("callbookGroupBox")
+        self.horizontalLayout_3 = QtWidgets.QHBoxLayout(self.callbookGroupBox)
         self.horizontalLayout_3.setObjectName("horizontalLayout_3")
-        self.hamQTHuplRadioButton = QtWidgets.QRadioButton(parent=self.hamQTHGroupBox)
-        self.hamQTHuplRadioButton.setObjectName("hamQTHuplRadioButton")
-        self.horizontalLayout_3.addWidget(self.hamQTHuplRadioButton)
-        self.hamQTHmodRadioButton = QtWidgets.QRadioButton(parent=self.hamQTHGroupBox)
-        self.hamQTHmodRadioButton.setObjectName("hamQTHmodRadioButton")
-        self.horizontalLayout_3.addWidget(self.hamQTHmodRadioButton)
+        self.hamQTHCheckBox = QtWidgets.QCheckBox(parent=self.callbookGroupBox)
+        self.hamQTHCheckBox.setObjectName("hamQTHCheckBox")
+        self.horizontalLayout_3.addWidget(self.hamQTHCheckBox)
         spacerItem10 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout_3.addItem(spacerItem10)
-        self.verticalLayout_6.addWidget(self.hamQTHGroupBox)
+        self.verticalLayout_6.addWidget(self.callbookGroupBox)
         spacerItem11 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.verticalLayout_6.addItem(spacerItem11)
         self.toolBox.addItem(self.qslPage, "")
         self.verticalLayout.addWidget(self.toolBox)
         self.horizontalLayout_2 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_2.setObjectName("horizontalLayout_2")
         spacerItem12 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
@@ -393,16 +381,15 @@
         self.cancelPushButton.setObjectName("cancelPushButton")
         self.horizontalLayout_2.addWidget(self.cancelPushButton)
         self.verticalLayout.addLayout(self.horizontalLayout_2)
 
         self.retranslateUi(QSOForm)
         self.toolBox.setCurrentIndex(0)
         self.savePushButton.clicked.connect(QSOForm.saveLog) # type: ignore
-        self.autoDateCheckBox.toggled['bool'].connect(self.timeEdit.setDisabled) # type: ignore
-        self.autoDateCheckBox.toggled['bool'].connect(self.dateEdit.setDisabled) # type: ignore
+        self.autoDateCheckBox.toggled['bool'].connect(self.dateOffEdit.setDisabled) # type: ignore
         self.stationGroupBox.toggled['bool'].connect(self.ownLocatorLineEdit.setDisabled) # type: ignore
         self.stationGroupBox.toggled['bool'].connect(self.ownQTHLineEdit.setDisabled) # type: ignore
         self.stationGroupBox.toggled['bool'].connect(self.radioLineEdit.setDisabled) # type: ignore
         self.stationGroupBox.toggled['bool'].connect(self.antennaLineEdit.setDisabled) # type: ignore
         self.bandComboBox.currentTextChanged['QString'].connect(QSOForm.bandChanged) # type: ignore
         self.stationGroupBox.toggled['bool'].connect(QSOForm.stationChanged) # type: ignore
         self.identityGroupBox.toggled['bool'].connect(QSOForm.identityChanged) # type: ignore
@@ -413,24 +400,29 @@
         self.RSTSentLineEdit.textEdited['QString'].connect(QSOForm.rstSentChanged) # type: ignore
         self.locatorLineEdit.textEdited['QString'].connect(QSOForm.locatorChanged) # type: ignore
         self.callSignLineEdit.textEdited['QString'].connect(QSOForm.callSignChanged) # type: ignore
         self.ownLocatorLineEdit.textEdited['QString'].connect(QSOForm.ownLocatorChanged) # type: ignore
         self.ownCallSignLineEdit.textEdited['QString'].connect(QSOForm.ownCallSignChanged) # type: ignore
         self.callSignLineEdit.editingFinished.connect(QSOForm.setWorkedBefore) # type: ignore
         self.timeNowPushButton.clicked.connect(QSOForm.setStartTimeNow) # type: ignore
-        self.searchCallbookPushButton.clicked.connect(QSOForm.searchCallbook) # type: ignore
+        self.searchHamQTHPushButton.clicked.connect(QSOForm.searchHamQTH) # type: ignore
         self.uploadPushButton.clicked.connect(QSOForm.uploadLog) # type: ignore
         self.eqslInboxPushButton.clicked.connect(QSOForm.eqslCheckInbox) # type: ignore
         self.eqslDownloadPushButton.clicked.connect(QSOForm.eqslDownload) # type: ignore
         self.lotwInboxPushButton.clicked.connect(QSOForm.lotwCheckInbox) # type: ignore
         self.cancelPushButton.clicked.connect(QSOForm.clear) # type: ignore
         self.modeComboBox.currentTextChanged['QString'].connect(QSOForm.modeChanged) # type: ignore
+        self.autoDateCheckBox.toggled['bool'].connect(self.timeOffEdit.setDisabled) # type: ignore
+        self.timeOnEdit.textEdited['QString'].connect(QSOForm.timeOnChanged) # type: ignore
+        self.timeOffEdit.textEdited['QString'].connect(QSOForm.timeOffChanged) # type: ignore
+        self.autoDateCheckBox.toggled['bool'].connect(QSOForm.autoDateCBChanged) # type: ignore
+        self.searchQRZCQPushButton.clicked.connect(QSOForm.searchQRZCQ) # type: ignore
         QtCore.QMetaObject.connectSlotsByName(QSOForm)
-        QSOForm.setTabOrder(self.callSignLineEdit, self.searchCallbookPushButton)
-        QSOForm.setTabOrder(self.searchCallbookPushButton, self.RSTSentLineEdit)
+        QSOForm.setTabOrder(self.callSignLineEdit, self.searchHamQTHPushButton)
+        QSOForm.setTabOrder(self.searchHamQTHPushButton, self.RSTSentLineEdit)
         QSOForm.setTabOrder(self.RSTSentLineEdit, self.RSTRcvdLineEdit)
         QSOForm.setTabOrder(self.RSTRcvdLineEdit, self.bandComboBox)
         QSOForm.setTabOrder(self.bandComboBox, self.channelComboBox)
         QSOForm.setTabOrder(self.channelComboBox, self.freqDoubleSpinBox)
         QSOForm.setTabOrder(self.freqDoubleSpinBox, self.modeComboBox)
         QSOForm.setTabOrder(self.modeComboBox, self.submodeComboBox)
         QSOForm.setTabOrder(self.submodeComboBox, self.nameLineEdit)
@@ -445,54 +437,50 @@
         QSOForm.setTabOrder(self.stationGroupBox, self.ownQTHLineEdit)
         QSOForm.setTabOrder(self.ownQTHLineEdit, self.ownLocatorLineEdit)
         QSOForm.setTabOrder(self.ownLocatorLineEdit, self.radioLineEdit)
         QSOForm.setTabOrder(self.radioLineEdit, self.antennaLineEdit)
         QSOForm.setTabOrder(self.antennaLineEdit, self.timeNowPushButton)
         QSOForm.setTabOrder(self.timeNowPushButton, self.autoDateCheckBox)
         QSOForm.setTabOrder(self.autoDateCheckBox, self.dateOnEdit)
-        QSOForm.setTabOrder(self.dateOnEdit, self.timeOnEdit)
-        QSOForm.setTabOrder(self.timeOnEdit, self.dateEdit)
-        QSOForm.setTabOrder(self.dateEdit, self.timeEdit)
-        QSOForm.setTabOrder(self.timeEdit, self.commentsTextEdit)
-        QSOForm.setTabOrder(self.commentsTextEdit, self.remarksTextEdit)
-        QSOForm.setTabOrder(self.remarksTextEdit, self.eqslSentCheckBox)
+        QSOForm.setTabOrder(self.dateOnEdit, self.dateOffEdit)
+        QSOForm.setTabOrder(self.dateOffEdit, self.eqslSentCheckBox)
         QSOForm.setTabOrder(self.eqslSentCheckBox, self.lotwSentCheckBox)
         QSOForm.setTabOrder(self.lotwSentCheckBox, self.qslAccBureauCheckBox)
         QSOForm.setTabOrder(self.qslAccBureauCheckBox, self.qslViaLineEdit)
         QSOForm.setTabOrder(self.qslViaLineEdit, self.qslMessageTextEdit)
         QSOForm.setTabOrder(self.qslMessageTextEdit, self.qslBurDirGroupBox)
         QSOForm.setTabOrder(self.qslBurDirGroupBox, self.qslBureauRadioButton)
         QSOForm.setTabOrder(self.qslBureauRadioButton, self.qslDirectRadioButton)
         QSOForm.setTabOrder(self.qslDirectRadioButton, self.qslSentCheckBox)
         QSOForm.setTabOrder(self.qslSentCheckBox, self.qslRcvdCheckBox)
         QSOForm.setTabOrder(self.qslRcvdCheckBox, self.eqslGroupBox)
         QSOForm.setTabOrder(self.eqslGroupBox, self.eqslInboxPushButton)
         QSOForm.setTabOrder(self.eqslInboxPushButton, self.eqslDownloadPushButton)
         QSOForm.setTabOrder(self.eqslDownloadPushButton, self.lotwGroupBox)
         QSOForm.setTabOrder(self.lotwGroupBox, self.lotwInboxPushButton)
-        QSOForm.setTabOrder(self.lotwInboxPushButton, self.hamQTHGroupBox)
-        QSOForm.setTabOrder(self.hamQTHGroupBox, self.uploadPushButton)
+        QSOForm.setTabOrder(self.lotwInboxPushButton, self.callbookGroupBox)
+        QSOForm.setTabOrder(self.callbookGroupBox, self.uploadPushButton)
         QSOForm.setTabOrder(self.uploadPushButton, self.savePushButton)
         QSOForm.setTabOrder(self.savePushButton, self.cancelPushButton)
         QSOForm.setTabOrder(self.cancelPushButton, self.qslAccDirectCheckBox)
         QSOForm.setTabOrder(self.qslAccDirectCheckBox, self.qslAcceQSLCheckBox)
         QSOForm.setTabOrder(self.qslAcceQSLCheckBox, self.qslAccLoTWCheckBox)
-        QSOForm.setTabOrder(self.qslAccLoTWCheckBox, self.hamQTHmodRadioButton)
-        QSOForm.setTabOrder(self.hamQTHmodRadioButton, self.hamQTHuplRadioButton)
-        QSOForm.setTabOrder(self.hamQTHuplRadioButton, self.lotwRcvdCheckBox)
+        QSOForm.setTabOrder(self.qslAccLoTWCheckBox, self.hamQTHCheckBox)
+        QSOForm.setTabOrder(self.hamQTHCheckBox, self.lotwRcvdCheckBox)
         QSOForm.setTabOrder(self.lotwRcvdCheckBox, self.eqslRcvdCheckBox)
 
     def retranslateUi(self, QSOForm):
         _translate = QtCore.QCoreApplication.translate
         QSOForm.setWindowTitle(_translate("QSOForm", "QSO Form"))
         self.nameLineEdit.setPlaceholderText(_translate("QSOForm", "Name"))
         self.callSignLineEdit.setPlaceholderText(_translate("QSOForm", "Call sign"))
         self.QTHLineEdit.setPlaceholderText(_translate("QSOForm", "QTH"))
         self.locatorLineEdit.setPlaceholderText(_translate("QSOForm", "Locator"))
-        self.searchCallbookPushButton.setText(_translate("QSOForm", "Callbook"))
+        self.searchHamQTHPushButton.setText(_translate("QSOForm", "HamQTH"))
+        self.searchQRZCQPushButton.setText(_translate("QSOForm", "QRZCQ"))
         self.label.setText(_translate("QSOForm", "RST Tx"))
         self.RSTSentLineEdit.setText(_translate("QSOForm", "59"))
         self.RSTSentLineEdit.setPlaceholderText(_translate("QSOForm", "RST sent"))
         self.label_2.setText(_translate("QSOForm", "RST Rx"))
         self.RSTRcvdLineEdit.setText(_translate("QSOForm", "59"))
         self.RSTRcvdLineEdit.setPlaceholderText(_translate("QSOForm", "RST received"))
         self.powerLabel.setText(_translate("QSOForm", "Power"))
@@ -510,23 +498,23 @@
         self.ownCallSignLineEdit.setPlaceholderText(_translate("QSOForm", "Own call sign"))
         self.ownNameLineEdit.setPlaceholderText(_translate("QSOForm", "Own name"))
         self.stationGroupBox.setTitle(_translate("QSOForm", "Configured station"))
         self.ownQTHLineEdit.setPlaceholderText(_translate("QSOForm", "Own QTH"))
         self.ownLocatorLineEdit.setPlaceholderText(_translate("QSOForm", "Own locator"))
         self.radioLineEdit.setPlaceholderText(_translate("QSOForm", "Radio"))
         self.antennaLineEdit.setPlaceholderText(_translate("QSOForm", "Antenna"))
-        self.dateEdit.setDisplayFormat(_translate("QSOForm", "yyyy-MM-dd"))
-        self.dateOnEdit.setDisplayFormat(_translate("QSOForm", "yyyy-MM-dd"))
         self.timeNowPushButton.setText(_translate("QSOForm", "Now"))
         self.label_4.setText(_translate("QSOForm", "End"))
-        self.timeEdit.setDisplayFormat(_translate("QSOForm", "HH:mm:ss"))
-        self.timeOnEdit.setDisplayFormat(_translate("QSOForm", "HH:mm:ss"))
-        self.label_3.setText(_translate("QSOForm", "Start"))
+        self.timeOnEdit.setPlaceholderText(_translate("QSOForm", "Time start"))
         self.autoDateCheckBox.setText(_translate("QSOForm", "Automatically"))
-        self.commentsTextEdit.setPlaceholderText(_translate("QSOForm", "QSO comments"))
+        self.label_3.setText(_translate("QSOForm", "Start"))
+        self.dateOnEdit.setDisplayFormat(_translate("QSOForm", "yyyy-MM-dd"))
+        self.dateOffEdit.setDisplayFormat(_translate("QSOForm", "yyyy-MM-dd"))
+        self.timeOffEdit.setPlaceholderText(_translate("QSOForm", "Time end"))
+        self.commentLineEdit.setPlaceholderText(_translate("QSOForm", "QSO comment"))
         self.remarksTextEdit.setPlaceholderText(_translate("QSOForm", "Own notes"))
         self.toolBox.setItemText(self.toolBox.indexOf(self.mainPage), _translate("QSOForm", "Main data"))
         self.qslGroupBox.setTitle(_translate("QSOForm", "QSL"))
         self.qslViaLineEdit.setToolTip(_translate("QSOForm", "The contacted station QSL route.\n"
 "This is not the QSL manager/bureau address."))
         self.qslViaLineEdit.setPlaceholderText(_translate("QSOForm", "QSL via"))
         self.qslMessageTextEdit.setPlaceholderText(_translate("QSOForm", "QSL card message"))
@@ -546,15 +534,14 @@
         self.eqslInboxPushButton.setText(_translate("QSOForm", "Check Inbox"))
         self.eqslLinkLabel.setText(_translate("QSOForm", "Link to eQSL Card"))
         self.eqslDownloadPushButton.setText(_translate("QSOForm", "Download eQSL"))
         self.lotwGroupBox.setTitle(_translate("QSOForm", "LoTW"))
         self.lotwSentCheckBox.setText(_translate("QSOForm", "LoTW sent"))
         self.lotwRcvdCheckBox.setText(_translate("QSOForm", "LoTW received"))
         self.lotwInboxPushButton.setText(_translate("QSOForm", "Check Inbox"))
-        self.hamQTHGroupBox.setTitle(_translate("QSOForm", "HamQTH"))
-        self.hamQTHuplRadioButton.setText(_translate("QSOForm", "Uploaded"))
-        self.hamQTHmodRadioButton.setText(_translate("QSOForm", "Modified"))
+        self.callbookGroupBox.setTitle(_translate("QSOForm", "Logbook"))
+        self.hamQTHCheckBox.setText(_translate("QSOForm", "HamQTH"))
         self.toolBox.setItemText(self.toolBox.indexOf(self.qslPage), _translate("QSOForm", "QSL && Log upload"))
         self.uploadPushButton.setToolTip(_translate("QSOForm", "Uploads only if selected on QSL page"))
         self.uploadPushButton.setText(_translate("QSOForm", "Save && Upload"))
         self.savePushButton.setText(_translate("QSOForm", "Save"))
         self.cancelPushButton.setText(_translate("QSOForm", "Clear"))
```

### Comparing `DragonLog-1.0/dragonlog/DragonLog_RegEx.py` & `dragonlog-1.1/dragonlog/RegEx.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module contains the regular expression for field validation"""
 import re
 
 REGEX_CALL = re.compile(r'([a-zA-Z0-9]{1,3}?/)?([a-zA-Z0-9]{1,3}?[0-9][a-zA-Z0-9]{0,3}?[a-zA-Z])(/[aAmMpPrRtT]{1,2}?)?')
 REGEX_RSTFIELD = re.compile(r'([1-5][1-9][1-9aAcCkKmMsSxX]?)|([rR]?[-+]?[0-9]{1,2})')
 REGEX_LOCATOR = re.compile(r'[a-rA-R]{2}[0-9]{2}([a-xA-X]{2}([0-9]{2})?)?')
 REGEX_NONASCII = re.compile(r'[ -~\n\r]*(.)?')
+REGEX_TIME = re.compile(r'(([0-1][0-9])|(2[0-3])):([0-5][0-9])(:[0-5][0-9])?')
 
 def check_format(exp: re.Pattern, txt: str) -> bool:
     """Test the given text against a regular expression
     :param exp: a compiled pattern
     :param txt: a text
     :return: true if pattern matches"""
     return bool(re.fullmatch(exp, txt))
```

### Comparing `DragonLog-1.0/dragonlog/DragonLog_Settings.py` & `dragonlog-1.1/dragonlog/DragonLog_Settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,25 +7,29 @@
 
 import maidenhead
 from PyQt6 import QtWidgets, QtCore, QtGui
 import keyring
 
 from . import DragonLog_Settings_ui
 from .Logger import Logger
-from .DragonLog_RegEx import REGEX_CALL, REGEX_LOCATOR, check_format
+from .RegEx import REGEX_CALL, REGEX_LOCATOR, check_format
+from .CallBook import CallBookType
 
 # Fix problems with importing win32 in frozen executable
 if getattr(sys, 'frozen', False):
+    # noinspection PyUnresolvedReferences
     import win32timezone
     from keyring.backends import Windows
 
     keyring.set_keyring(Windows.WinVaultKeyring())
 
 
 class Settings(QtWidgets.QDialog, DragonLog_Settings_ui.Ui_Dialog):
+    callbookChanged = QtCore.pyqtSignal(str)
+
     def __init__(self, parent, settings: QtCore.QSettings, rig_status: QtWidgets.QLabel, cols: typing.Iterable,
                  logger: Logger):
         super().__init__(parent)
         self.setupUi(self)
 
         self.log = logging.getLogger('Settings')
         self.log.addHandler(logger)
@@ -73,14 +77,17 @@
         self.palette_faulty = QtGui.QPalette()
         self.palette_faulty.setColor(QtGui.QPalette.ColorGroup.Active, QtGui.QPalette.ColorRole.Base,
                                      QtGui.QColor(255, 204, 204))
 
         self.columns = cols
         self.sortComboBox.insertItems(0, cols)
 
+        self.callbooks = dict([(cbt.value, cbt.name) for cbt in set(CallBookType)])
+        self.callbookComboBox.insertItems(0, self.callbooks.keys())
+
     def calcLocator(self):
         self.locatorLineEdit.setText(maidenhead.to_maiden(self.latitudeDoubleSpinBox.value(),
                                                           self.longitudeDoubleSpinBox.value(),
                                                           4))
 
     def checkRigctld(self):
         if self.rigctld and self.rigctld.poll():
@@ -177,14 +184,15 @@
         self.rig_caps = []
         for ln in stdout.split('\n'):
             if ln.startswith('Can '):
                 cap, able = ln.split(':')
                 if able.strip() == 'Y':
                     self.rig_caps.append(cap[4:].lower())
 
+    # noinspection PyUnresolvedReferences
     def ctrlRigctld(self, start):
         if start:
             if not self.rigctld:
                 rig_mfr = self.settings.value('cat/rigMfr')
                 rig_model = self.settings.value('cat/rigModel')
                 rig_if = self.settings.value("cat/interface")
                 rig_speed = self.settings.value("cat/baud")
@@ -268,14 +276,18 @@
     def showCol(self):
         for item in self.colHideListWidget.selectedItems():
             self.colShowListWidget.insertItem(0, item.text())
             self.colHideListWidget.takeItem(self.colHideListWidget.row(item))
 
         self.colShowListWidget.sortItems()
 
+    def callbookSelected(self, service: str):
+        """Slot (i.e. if callbookComboBox is changed)"""
+        self.callbookUserLineEdit.setText(self.settings.value(f'callbook/{self.callbooks[service]}_user', ''))
+
     def exec(self):
         self.log.info('Loading settings...')
         self.catInterfaceLineEdit.setText(self.settings.value('cat/interface', ''))
         self.catBaudComboBox.setCurrentText(self.settings.value('cat/baud', ''))
 
         self.callsignLineEdit.setText(self.settings.value('station/callSign', ''))
         self.nameLineEdit.setText(self.settings.value('station/name', ''))
@@ -309,30 +321,48 @@
         self.logToFileCheckBox.setChecked(bool(self.settings.setValue('ui/log_file', 0)))
 
         self.expOwnNotesADIFCheckBox.setChecked(bool(self.settings.value('imp_exp/own_notes_adif', 0)))
         self.expRecentOnlyCheckBox.setChecked(bool(self.settings.value('imp_exp/only_recent', 0)))
         self.useCfgIDWatchCheckBox.setChecked(bool(self.settings.value('imp_exp/use_id_watch', 0)))
         self.useCfgStationWatchCheckBox.setChecked(bool(self.settings.value('imp_exp/use_station_watch', 0)))
 
-        self.callbookUserLineEdit.setText(self.settings.value('callbook/username', ''))
+        self.callbookComboBox.setCurrentText(self.callbook_dname)
+        self.callbookUserLineEdit.setText(self.settings.value(f'callbook/{self.callbook_id}_user', ''))
+
         self.eqslUserLineEdit.setText(self.settings.value('eqsl/username', ''))
         self.lotwUserLineEdit.setText(self.settings.value('lotw/username', ''))
         self.lotwCertPwdCheckBox.setChecked(bool(self.settings.value('lotw/cert_needs_pwd', 0)))
 
         return super().exec()
 
-    def callbookPassword(self):
-        return keyring.get_password('HamQTH.com',
-                                    self.settings.value('callbook/username', ''))
+    @property
+    def callbook_id(self) -> str:
+        """The selected callbooks id"""
+        return self.settings.value('callbook/service', 'HamQTH')
+
+    @property
+    def callbook_dname(self) -> str:
+        """Returns the selected callbooks descriptive name"""
+        return CallBookType[self.settings.value('callbook/service', 'HamQTH')].value
+
+    def callbookPassword(self, callbook: CallBookType) -> str:
+        """Get the password for the callbook
+        :param callbook: the callbook service to get the password for
+        :return: the password"""
+
+        return keyring.get_password(callbook.value,
+                                    self.settings.value(f'callbook/{callbook.name}_user', ''))
 
-    def eqslPassword(self):
+    def eqslPassword(self) -> str:
+        """The password for the eQSL service"""
         return keyring.get_password('eqsl.cc',
                                     self.settings.value('eqsl/username', ''))
 
-    def lotwPassword(self):
+    def lotwPassword(self) -> str:
+        """The password for the LoTW online service"""
         return keyring.get_password('lotw.arrl.org',
                                     self.settings.value('lotw/username', ''))
 
     def accept(self):
         self.log.info('Saving Settings...')
         self.settings.setValue('cat/interface', self.catInterfaceLineEdit.text())
         self.settings.setValue('cat/baud', self.catBaudComboBox.currentText())
@@ -363,20 +393,22 @@
         self.settings.setValue('ui/log_file', int(self.logToFileCheckBox.isChecked()))
 
         self.settings.setValue('imp_exp/own_notes_adif', int(self.expOwnNotesADIFCheckBox.isChecked()))
         self.settings.setValue('imp_exp/only_recent', int(self.expRecentOnlyCheckBox.isChecked()))
         self.settings.setValue('imp_exp/use_id_watch', int(self.useCfgIDWatchCheckBox.isChecked()))
         self.settings.setValue('imp_exp/use_station_watch', int(self.useCfgStationWatchCheckBox.isChecked()))
 
-        self.settings.setValue('callbook/username', self.callbookUserLineEdit.text())
+        self.settings.setValue('callbook/service', self.callbooks[self.callbookComboBox.currentText()])
+        self.settings.setValue(f'callbook/{self.callbook_id}_user', self.callbookUserLineEdit.text())
         if self.callbookUserLineEdit.text() and self.callbookPasswdLineEdit.text():
-            keyring.set_password('HamQTH.com',
+            keyring.set_password(self.callbookComboBox.currentText(),
                                  self.callbookUserLineEdit.text(),
                                  self.callbookPasswdLineEdit.text())
         self.callbookPasswdLineEdit.clear()
+        self.callbookChanged.emit(self.callbooks[self.callbookComboBox.currentText()])
 
         self.settings.setValue('eqsl/username', self.eqslUserLineEdit.text())
         if self.eqslUserLineEdit.text() and self.eqslPasswdLineEdit.text():
             keyring.set_password('eqsl.cc',
                                  self.eqslUserLineEdit.text(),
                                  self.eqslPasswdLineEdit.text())
         self.eqslPasswdLineEdit.clear()
```

### Comparing `DragonLog-1.0/dragonlog/DragonLog_Settings_ui.py` & `dragonlog-1.1/dragonlog/DragonLog_Settings_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,25 +373,31 @@
         self.verticalLayout_9.setObjectName("verticalLayout_9")
         self.groupBox_5 = QtWidgets.QGroupBox(parent=self.tab_2)
         self.groupBox_5.setObjectName("groupBox_5")
         self.formLayout_4 = QtWidgets.QFormLayout(self.groupBox_5)
         self.formLayout_4.setObjectName("formLayout_4")
         self.label_16 = QtWidgets.QLabel(parent=self.groupBox_5)
         self.label_16.setObjectName("label_16")
-        self.formLayout_4.setWidget(0, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_16)
+        self.formLayout_4.setWidget(1, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_16)
         self.callbookUserLineEdit = QtWidgets.QLineEdit(parent=self.groupBox_5)
         self.callbookUserLineEdit.setObjectName("callbookUserLineEdit")
-        self.formLayout_4.setWidget(0, QtWidgets.QFormLayout.ItemRole.FieldRole, self.callbookUserLineEdit)
+        self.formLayout_4.setWidget(1, QtWidgets.QFormLayout.ItemRole.FieldRole, self.callbookUserLineEdit)
         self.label_17 = QtWidgets.QLabel(parent=self.groupBox_5)
         self.label_17.setObjectName("label_17")
-        self.formLayout_4.setWidget(1, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_17)
+        self.formLayout_4.setWidget(2, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_17)
         self.callbookPasswdLineEdit = QtWidgets.QLineEdit(parent=self.groupBox_5)
         self.callbookPasswdLineEdit.setEchoMode(QtWidgets.QLineEdit.EchoMode.PasswordEchoOnEdit)
         self.callbookPasswdLineEdit.setObjectName("callbookPasswdLineEdit")
-        self.formLayout_4.setWidget(1, QtWidgets.QFormLayout.ItemRole.FieldRole, self.callbookPasswdLineEdit)
+        self.formLayout_4.setWidget(2, QtWidgets.QFormLayout.ItemRole.FieldRole, self.callbookPasswdLineEdit)
+        self.callbookComboBox = QtWidgets.QComboBox(parent=self.groupBox_5)
+        self.callbookComboBox.setObjectName("callbookComboBox")
+        self.formLayout_4.setWidget(0, QtWidgets.QFormLayout.ItemRole.FieldRole, self.callbookComboBox)
+        self.label_24 = QtWidgets.QLabel(parent=self.groupBox_5)
+        self.label_24.setObjectName("label_24")
+        self.formLayout_4.setWidget(0, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_24)
         self.verticalLayout_9.addWidget(self.groupBox_5)
         self.groupBox_6 = QtWidgets.QGroupBox(parent=self.tab_2)
         self.groupBox_6.setObjectName("groupBox_6")
         self.formLayout_5 = QtWidgets.QFormLayout(self.groupBox_6)
         self.formLayout_5.setObjectName("formLayout_5")
         self.label_18 = QtWidgets.QLabel(parent=self.groupBox_6)
         self.label_18.setObjectName("label_18")
@@ -461,14 +467,15 @@
         self.callsignLineEdit.textChanged['QString'].connect(Dialog.callSignChanged) # type: ignore
         self.callsignCBLineEdit.textEdited['QString'].connect(Dialog.callSignCBChanged) # type: ignore
         self.callsignLineEdit.textEdited['QString'].connect(Dialog.callSignChanged) # type: ignore
         self.hideColPushButton.clicked.connect(Dialog.hideCol) # type: ignore
         self.showColPushButton.clicked.connect(Dialog.showCol) # type: ignore
         self.colHideListWidget.itemDoubleClicked['QListWidgetItem*'].connect(Dialog.showCol) # type: ignore
         self.colShowListWidget.itemDoubleClicked['QListWidgetItem*'].connect(Dialog.hideCol) # type: ignore
+        self.callbookComboBox.currentTextChanged['QString'].connect(Dialog.callbookSelected) # type: ignore
         QtCore.QMetaObject.connectSlotsByName(Dialog)
 
     def retranslateUi(self, Dialog):
         _translate = QtCore.QCoreApplication.translate
         Dialog.setWindowTitle(_translate("Dialog", "Settings"))
         self.label.setText(_translate("Dialog", "Call sign"))
         self.label_3.setText(_translate("Dialog", "QTH"))
@@ -529,17 +536,18 @@
         self.expOwnNotesADIFCheckBox.setText(_translate("Dialog", "Export own notes to ADIF"))
         self.expRecentOnlyCheckBox.setToolTip(_translate("Dialog", "See settings page \"User interface\""))
         self.expRecentOnlyCheckBox.setText(_translate("Dialog", "Export only recent QSOs"))
         self.groupBox_4.setTitle(_translate("Dialog", "Watch File"))
         self.useCfgIDWatchCheckBox.setText(_translate("Dialog", "Use configured ID for missing values"))
         self.useCfgStationWatchCheckBox.setText(_translate("Dialog", "Use configured Station for missing values"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab), _translate("Dialog", "Import/Export"))
-        self.groupBox_5.setTitle(_translate("Dialog", "HamQTH"))
+        self.groupBox_5.setTitle(_translate("Dialog", "Callbook"))
         self.label_16.setText(_translate("Dialog", "Username"))
         self.label_17.setText(_translate("Dialog", "Password"))
+        self.label_24.setText(_translate("Dialog", "Service"))
         self.groupBox_6.setTitle(_translate("Dialog", "eQSL"))
         self.label_18.setText(_translate("Dialog", "Username"))
         self.label_19.setText(_translate("Dialog", "Password"))
         self.groupBox_81.setTitle(_translate("Dialog", "LoTW"))
         self.label_22.setText(_translate("Dialog", "Username"))
         self.lotwUserLineEdit.setToolTip(_translate("Dialog", "Username for LoTW online account not for the certificate"))
         self.label_211.setText(_translate("Dialog", "Password"))
```

### Comparing `DragonLog-1.0/dragonlog/Logger.py` & `dragonlog-1.1/dragonlog/Logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,15 @@
             self.log_widget.setTextColor(QtGui.QColor('black'))
             print(self.format(record))
 
         if self.__log_file__:
             self.__log_file__.write(log_msg + '\n')
 
         self.log_widget.append(log_msg)
+        self.log_widget.verticalScrollBar().setValue(self.log_widget.verticalScrollBar().maximum())
         self.log_widget.repaint()
 
     def debug(self, message):
         self.__log__.debug(message)
 
     def info(self, message):
         self.__log__.info(message)
```

### Comparing `DragonLog-1.0/dragonlog/data/README.md` & `dragonlog-1.1/dragonlog/data/README.md`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/data/bands.json` & `dragonlog-1.1/dragonlog/data/bands.json`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/data/cb_channels.json` & `dragonlog-1.1/dragonlog/data/cb_channels.json`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/data/color_map.json` & `dragonlog-1.1/dragonlog/data/color_map.json`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/data/i18n/DragonLog_de.qm` & `dragonlog-1.1/dragonlog/data/i18n/DragonLog_de.qm`

 * *Files 2% similar despite different names*

```diff
@@ -1,1481 +1,1538 @@
 00000000: 3cb8 6418 caef 9c95 cd21 1cbf 60a1 bddd  <.d......!..`...
-00000010: a700 0000 0564 655f 4445 4200 0009 a800  .....de_DEB.....
+00000010: a700 0000 0564 655f 4445 4200 0009 f000  .....de_DEB.....
 00000020: 0000 3c00 0001 5c00 0000 3e00 0001 7800  ..<...\...>...x.
-00000030: 0002 5700 0035 4700 0003 8900 0035 8500  ..W..5G......5..
-00000040: 0005 5b00 0023 6c00 000c d000 0011 4100  ..[..#l.......A.
-00000050: 0031 0e00 0000 0000 0047 6400 0001 fe00  .1.......Gd.....
-00000060: 004c 4400 003d 5700 0052 8400 0007 8400  .LD..=W..R......
-00000070: 0053 5e00 0008 b200 0055 6700 0041 7e00  .S^......Ug..A~.
-00000080: 0056 7c00 0043 6500 0056 7f00 0026 2900  .V|..Ce..V...&).
-00000090: 0056 8800 000a 9000 0056 8800 0026 d100  .V.......V...&..
-000000a0: 0056 8800 0045 4a00 0058 f700 000b 0c00  .V...EJ..X......
-000000b0: 026f fa00 0035 6500 0345 3000 0000 3f00  .o...5e..E0...?.
-000000c0: 0357 3000 0000 bf00 037b 3000 0000 fe00  .W0......{0.....
-000000d0: 03c9 3000 0001 3d00 0488 4400 0014 e900  ..0...=...D.....
-000000e0: 0488 4400 0037 b800 04bb 0400 0030 e900  ..D..7.......0..
-000000f0: 04cf 0400 0031 2000 04d0 2500 0031 ba00  .....1 ...%..1..
-00000100: 04e7 1000 001d f000 04ec 3000 001d c400  ..........0.....
-00000110: 04ec 3000 0031 e700 0534 9700 0007 d800  ..0..1...4......
-00000120: 0534 9700 003e f000 0545 a500 0022 8e00  .4...>...E..."..
-00000130: 0545 a500 0040 6500 0548 3500 0008 da00  .E...@e..H5.....
-00000140: 0548 3500 0022 b000 0548 3500 0040 bb00  .H5.."...H5..@..
-00000150: 0596 7c00 000e 2800 0598 c500 0046 4c00  ..|...(......FL.
-00000160: 05ab 6000 0050 6a00 06a6 7c00 0011 2200  ..`..Pj...|...".
-00000170: 06a6 7c00 004b 7000 06fb 2100 0040 2c00  ..|..Kp...!..@,.
-00000180: 0714 3e00 004c 1400 144b 9e00 000d 9500  ..>..L...K......
-00000190: 144e e600 0020 e600 3477 3000 0000 7f00  .N... ..4w0.....
-000001a0: 34c5 3000 0000 9f00 36b7 3000 0000 de00  4.0.....6.0.....
-000001b0: 38a9 3000 0001 1d00 4796 c400 0013 4f00  8.0.....G.....O.
-000001c0: 4796 c400 002e be00 47ab 7600 002e 8b00  G.......G.v.....
-000001d0: 47ab 7600 0050 f900 4a2b 8200 003b 5500  G.v..P..J+...;U.
-000001e0: 4c99 6200 001b 7700 4c99 6200 003d 7e00  L.b...w.L.b..=~.
-000001f0: 52cc bc00 0007 ae00 556a c300 0023 3b00  R.......Uj...#;.
-00000200: 56ae c200 0051 db00 576d c200 0024 9b00  V....Q..Wm...$..
-00000210: 576d c200 0042 ef00 587a ff00 000a ae00  Wm...B..Xz......
-00000220: 587a ff00 0027 6000 587a ff00 0046 2b00  Xz...'`.Xz...F+.
-00000230: 5aa8 9400 000d e600 5aa8 9400 0047 9200  Z.......Z....G..
-00000240: 5aa8 9400 0050 0500 67ab 0600 0050 cd00  Z....P..g....P..
-00000250: 6d92 9400 004e a500 753c 2300 0042 ae00  m....N..u<#..B..
-00000260: 8cd2 1500 0010 1200 aa80 2500 001a 3600  ..........%...6.
-00000270: ab72 4500 0009 cd00 bf5b b400 0005 f500  .rE......[......
-00000280: c656 de00 003b dd00 ff2c 7700 001b ff01  .V...;...,w.....
-00000290: 30ed a300 001c 9601 48c4 ff00 001a 7001  0.......H.....p.
-000002a0: 4d8a bc00 0021 5b01 5478 6c00 0021 f101  M....![.Txl..!..
-000002b0: 6bb3 1300 0045 0601 945e f800 0029 0601  k....E...^...)..
-000002c0: 9942 b500 0040 db01 9ce8 5e00 0048 5b01  .B...@....^..H[.
-000002d0: e578 e300 000d 2601 e907 4500 0041 2b01  .x....&...E..A+.
-000002e0: fdeb 5400 004b 9002 3222 f900 0037 1302  ..T..K..2"...7..
-000002f0: 33a9 3400 0008 f902 e7d6 5e00 0002 4102  3.4.......^...A.
-00000300: e7d6 5e00 0015 5b02 e7d6 5e00 0038 4102  ..^...[...^..8A.
-00000310: e81d 2400 003c a803 004d 1200 000c 2d03  ..$..<...M....-.
-00000320: 0149 e600 0021 1303 0cac 0500 000f 9c03  .I...!..........
-00000330: 0f6b 1200 0042 2d03 0f6b 3200 0023 8c03  .k...B-..k2..#..
-00000340: 1bec 1200 0013 ae03 4485 3000 0000 1e03  ........D.0.....
-00000350: 45b3 3000 0000 5e03 4ecb 9200 0033 e203  E.0...^.N....3..
-00000360: 4ecb 9200 0050 2703 533f be00 0052 0403  N....P'.S?...R..
-00000370: 598b 3200 0007 f703 598b 3200 0020 c103  Y.2.....Y.2.. ..
-00000380: 598b 3200 003f 9603 6cc3 0400 000b c503  Y.2..?..l.......
-00000390: 881f d400 0006 1e03 9ce3 f400 001e 1203  ................
-000003a0: 9ce9 a500 0025 0d03 f5e0 0700 002d 6b04  .....%.......-k.
-000003b0: 07f6 ee00 0024 4c04 07f6 ee00 0041 e004  .....$L......A..
-000003c0: 2b4e 0500 001d 3f04 6c90 3200 003f b904  +N....?.l.2..?..
-000003d0: 8c96 8100 0014 2f04 8caf 6200 0014 7904  ....../...b...y.
-000003e0: 9c8b 8500 0037 d804 a472 8400 002b 1a04  .....7...r...+..
-000003f0: ab8e f500 002f bb04 ab8e fc00 002f e004  ...../......./..
-00000400: ab8f 0100 0030 0504 ab8f 0700 0030 2a04  .....0.......0*.
-00000410: ab8f 0800 0030 4f04 b08b a400 003c 3504  .....0O......<5.
-00000420: b2b6 6400 0008 6b04 c4a9 a900 0013 1604  ..d...k.........
-00000430: cf76 9400 0004 7104 cf76 9400 0031 5104  .v....q..v...1Q.
-00000440: e826 8800 0005 d404 e826 8800 001d 7c04  .&.......&....|.
-00000450: e826 8800 003e 5304 e842 f200 001d a004  .&...>S..B......
-00000460: e842 f200 004f 1b04 edd3 6400 0036 2904  .B...O....d..6).
-00000470: f5b6 e700 002a 0a05 0476 9400 0032 1405  .....*...v...2..
-00000480: 1f06 1500 004f 3e05 3268 c400 0003 f505  .....O>.2h......
-00000490: 34db 8200 0021 a905 3ddf a300 000a ce05  4....!..=.......
-000004a0: 4466 8200 0046 ce05 5776 4500 0043 d305  Df...F..WvE..C..
-000004b0: 6336 9e00 0032 7d05 647d 0e00 002f 6705  c6...2}.d}.../g.
-000004c0: 7865 9800 0045 6905 7865 b800 0045 8b05  xe...Ei.xe...E..
-000004d0: afca f400 0040 8505 c7f7 2800 0052 6805  .....@....(..Rh.
-000004e0: c984 e900 0030 7406 011e c400 0002 7906  .....0t.......y.
-000004f0: 43c1 1300 0016 8b06 778d 0800 0006 cd06  C.......w.......
-00000500: 778d 0800 001e f406 7e7c a100 0025 f606  w.......~|...%..
-00000510: 7e7c a100 0044 9906 830d be00 0029 c406  ~|...D.......)..
-00000520: bdf0 a400 0019 6206 be94 d200 0050 8b06  ......b......P..
-00000530: d2af d900 0052 9206 db4d 4200 0027 c506  .....R...MB..'..
-00000540: e056 d800 0024 1106 e056 d800 0041 a706  .V...$...V...A..
-00000550: f895 8e00 0015 c507 2f4a 1500 0047 f907  ......../J...G..
-00000560: 357f 7400 004a 1207 366b 9300 0004 f707  5.t..J..6k......
-00000570: 50be 3900 0051 2b07 68f8 4400 004c 3c07  P.9..Q+.h.D..L<.
-00000580: 693d fe00 0031 7607 6941 4e00 0032 3907  i=...1v.iAN..29.
-00000590: 6cbb 6300 000e 4707 8f3a 3e00 0024 ce07  l.c...G..:>..$..
-000005a0: 8f3a 3e00 0043 2007 e67a d700 0030 c107  .:>..C ..z...0..
-000005b0: e76d c800 0025 5007 e78f a400 0025 8607  .m...%P......%..
-000005c0: e79f 3400 0025 be07 e79f 3400 0044 5d07  ..4..%....4..D].
-000005d0: e7e0 a400 002e 1507 e7f2 3400 002e 5007  ..........4...P.
-000005e0: e7f2 3400 004b d508 14d3 ed00 0032 be08  ..4..K.......2..
-000005f0: 14d3 ed00 0044 ca08 3292 cb00 0038 7a08  .....D..2....8z.
-00000600: 3587 6a00 002b 7908 36b6 5400 0012 5a08  5.j..+y.6.T...Z.
-00000610: 5ac5 0100 0001 9408 5ac5 0100 0013 fc08  Z.......Z.......
-00000620: 5ac5 0100 0036 e208 678f b400 0026 f208  Z....6..g....&..
-00000630: 679f 2400 0027 2a08 679f 2400 0045 ef08  g.$..'*.g.$..E..
-00000640: 7f52 2500 002a b908 8879 1400 0018 f408  .R%..*...y......
-00000650: aae3 e400 0009 9a08 b63d de00 0034 d008  .........=...4..
-00000660: bd74 5e00 0022 d208 d39b 6400 003f 1008  .t^.."....d..?..
-00000670: f89a cb00 0035 a309 14be 9200 0047 2609  .....5.......G&.
-00000680: 1c52 9500 002d ca09 238c 7500 0016 c509  .R...-..#.u.....
-00000690: 3f8c ad00 000c aa09 564e 4200 0049 7b09  ?.......VNB..I{.
-000006a0: 6c61 f400 0013 7a09 6c61 f400 002e ea09  la....z.la......
-000006b0: 6fe6 7e00 0011 5e09 8fa3 8700 002f 1f09  o.~...^....../..
-000006c0: 97c9 1400 0020 8609 97c9 1400 003f 5509  ..... .......?U.
-000006d0: 97d9 8400 0020 4b09 9c7f 1a00 0036 a809  ..... K......6..
-000006e0: a118 8500 0010 dd09 c004 d700 0003 bc09  ................
-000006f0: c4e8 d700 0001 c409 c8df a200 001e 6709  ..............g.
-00000700: c943 f500 000f d709 e854 fc00 0015 9609  .C.......T......
-00000710: e854 fc00 0039 c709 f42c fb00 001b 510a  .T...9...,....Q.
-00000720: 2087 bc00 003a a50a 2190 e200 0006 840a   ....:..!.......
-00000730: 2190 e200 001e a80a 3f0e 9500 0028 bd0a  !.......?....(..
-00000740: 5e68 d900 0026 4a0a 6789 3b00 0007 0c0a  ^h...&J.g.;.....
-00000750: 6789 3b00 001f 360a 67a9 0200 0007 480a  g.;...6.g.....H.
-00000760: 67a9 0200 001f 750a 6dc8 3e00 0034 690a  g.....u.m.>..4i.
-00000770: 7833 e400 0038 020a 7d6b 2400 0018 280a  x3...8..}k$...(.
-00000780: 92a2 e500 0029 700a 9612 e500 0028 630a  .....)p......(c.
-00000790: a8b0 0e00 000e 060a a8b0 0e00 0047 b30a  .............G..
-000007a0: acdb 7e00 0002 1c0a b945 f500 002a f50a  ..~......E...*..
-000007b0: b945 f500 0047 d60a c389 2500 0028 2c0a  .E...G....%..(,.
-000007c0: c5b4 4900 003e 750a c897 c500 0006 460a  ..I..>u.......F.
-000007d0: d2f0 b500 0002 e60a d382 7700 0003 340a  ..........w...4.
-000007e0: e2b5 9600 0004 920a f31c 2200 003a 310b  .........."..:1.
-000007f0: 1562 0700 004c c10b 1805 3900 0015 0b0b  .b...L....9.....
-00000800: 4597 5500 0008 190b 5d8a f400 001f b40b  E.U.....].......
-00000810: 6628 d200 0034 270b 7fe2 de00 0032 fd0b  f(...4'......2..
-00000820: ad17 7800 001b 230b ff25 ce00 001c 510c  ..x...#..%....Q.
-00000830: 08f5 6c00 003c 630c 107d 9300 0003 7e0c  ..l..<c..}....~.
-00000840: 10ba b200 0027 830c 1415 6300 003e 2f0c  .....'....c..>/.
-00000850: 1536 f700 002c ec0c 1f2f 0200 0049 cc0c  .6...,.../...I..
-00000860: 29f2 a400 004c 9b0c 6a19 e900 003b 8e0c  )....L..j....;..
-00000870: 8c09 2900 001d 080c 8c09 2900 003d fa0c  ..).......)..=..
-00000880: 9688 9500 0014 530c a3fa 5f00 0019 f80c  ......S..._.....
-00000890: a6e8 d400 0039 0b0c bb01 7300 000c 6d0c  .....9....s...m.
-000008a0: bb01 7300 0033 540c c9a0 0e00 002d 460d  ..s..3T......-F.
-000008b0: 0218 6400 0046 7e0d 07a4 f800 0039 f40d  ..d..F~......9..
-000008c0: 1f27 b200 0014 a70d 3504 b400 0039 670d  .'......5....9g.
-000008d0: 76f7 5900 001b a60d 825f 7300 000e ea0d  v.Y......_s.....
-000008e0: a03c 1200 004d 930d d0ff 4c00 002c a00d  .<...M....L..,..
-000008f0: f2ea c200 003a eb0d fe4e 2400 0019 ab0d  .....:...N$.....
-00000900: fe4e 2400 004e 590e 0543 5500 0023 d30e  .N$..NY..CU..#..
-00000910: 05d1 b500 004d f20e 0743 5500 0042 720e  .....M...CU..Br.
-00000920: 233d d500 004a 4c0e 87ac 6400 001f fd0e  #=...JL...d.....
-00000930: 93fa 5200 0017 6a0e a32f e400 003d ab0e  ..R...j../...=..
-00000940: c497 a200 000b 3c0e c72a a600 0005 5f0e  ......<..*...._.
-00000950: de3d a200 0038 9e0e e46b 3400 0045 ad0e  .=...8...k4..E..
-00000960: fdeb 3400 0044 1b0f 165e c400 0043 840f  ..4..D...^...C..
-00000970: 3562 ce00 0017 cb0f 6963 bc00 000c ef0f  5b......ic......
-00000980: 6963 bc00 002a 7f0f 6963 bc00 004f cc0f  ic...*..ic...O..
-00000990: 6978 c700 0033 950f 6c98 6c00 0051 b00f  ix...3..l.l..Q..
-000009a0: 7ddd 2800 004a f40f 8007 d400 0037 520f  }.(..J.......7R.
-000009b0: 8313 8900 0012 e30f cb15 5200 0018 aa0f  ..........R.....
-000009c0: e6f6 3400 003e 9d69 0000 52bc 03ff ffff  ..4..>.i..R.....
-000009d0: ff08 0000 0000 0600 0000 032e 2e2e 0700  ................
-000009e0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-000009f0: 0000 0000 0600 0000 0631 3135 3230 3007  .........115200.
-00000a00: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-00000a10: 0800 0000 0006 0000 0004 3132 3030 0700  ..........1200..
-00000a20: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000a30: 0000 0000 0600 0000 0631 3238 3030 3007  .........128000.
-00000a40: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-00000a50: 0800 0000 0006 0000 0005 3134 3430 3007  ..........14400.
-00000a60: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-00000a70: 0800 0000 0006 0000 0005 3139 3230 3007  ..........19200.
-00000a80: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-00000a90: 0800 0000 0006 0000 0004 3234 3030 0700  ..........2400..
-00000aa0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000ab0: 0000 0000 0600 0000 0533 3834 3030 0700  .........38400..
-00000ac0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000ad0: 0000 0000 0600 0000 0434 3830 3007 0000  .........4800...
-00000ae0: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
-00000af0: 0000 0006 0000 0005 3537 3630 3007 0000  ........57600...
-00000b00: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
-00000b10: 0000 0006 0000 0004 3936 3030 0700 0000  ........9600....
-00000b20: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
-00000b30: 0000 0600 0000 013c 0700 0000 0644 6961  .......<.....Dia
-00000b40: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
-00000b50: 0000 013e 0700 0000 0644 6961 6c6f 6701  ...>.....Dialog.
-00000b60: 0300 0000 0e00 4100 6e00 7400 6500 6e00  ......A.n.t.e.n.
-00000b70: 6e00 6508 0000 0000 0600 0000 0741 6e74  n.e..........Ant
-00000b80: 656e 6e61 0700 0000 0644 6961 6c6f 6701  enna.....Dialog.
-00000b90: 0300 0000 1600 4100 7500 6600 7300 7400  ......A.u.f.s.t.
-00000ba0: 6500 6900 6700 6500 6e00 6408 0000 0000  e.i.g.e.n.d.....
-00000bb0: 0600 0000 0941 7363 656e 6469 6e67 0700  .....Ascending..
-00000bc0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000bd0: 0000 0000 0600 0000 0343 4154 0700 0000  .........CAT....
-00000be0: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
-00000bf0: 0000 0600 0000 0a43 422d 5374 6174 696f  .......CB-Statio
-00000c00: 6e07 0000 0006 4469 616c 6f67 0103 0000  n.....Dialog....
-00000c10: 0014 0052 0075 0066 007a 0065 0069 0063  ...R.u.f.z.e.i.c
-00000c20: 0068 0065 006e 0800 0000 0006 0000 0009  .h.e.n..........
-00000c30: 4361 6c6c 2073 6967 6e07 0000 0006 4469  Call sign.....Di
-00000c40: 616c 6f67 0103 0000 0038 005a 0065 0072  alog.....8.Z.e.r
-00000c50: 0074 0069 0066 0069 006b 0061 0074 0020  .t.i.f.i.k.a.t. 
-00000c60: 0062 0065 006e 00f6 0074 0069 0067 0074  .b.e.n...t.i.g.t
-00000c70: 0020 0050 0061 0073 0073 0077 006f 0072  . .P.a.s.s.w.o.r
-00000c80: 0074 0800 0000 0006 0000 001a 4365 7274  .t..........Cert
-00000c90: 6966 6963 6174 6520 6e65 6564 7320 7061  ificate needs pa
-00000ca0: 7373 776f 7264 0700 0000 0644 6961 6c6f  ssword.....Dialo
-00000cb0: 6701 0300 0000 2400 5300 7000 6100 6c00  g.....$.S.p.a.l.
-00000cc0: 7400 6500 6e00 2000 7600 6500 7200 7300  t.e.n. .v.e.r.s.
-00000cd0: 7400 6500 6300 6b00 6500 6e08 0000 0000  t.e.c.k.e.n.....
-00000ce0: 0600 0000 0f43 6f6c 756d 6e73 2074 6f20  .....Columns to 
-00000cf0: 6869 6465 0700 0000 0644 6961 6c6f 6701  hide.....Dialog.
-00000d00: 0300 0000 2000 5300 7000 6100 6c00 7400  .... .S.p.a.l.t.
-00000d10: 6500 6e00 2000 6100 6e00 7a00 6500 6900  e.n. .a.n.z.e.i.
-00000d20: 6700 6500 6e08 0000 0000 0600 0000 0f43  g.e.n..........C
-00000d30: 6f6c 756d 6e73 2074 6f20 7368 6f77 0700  olumns to show..
-00000d40: 0000 0644 6961 6c6f 6701 0300 0000 1800  ...Dialog.......
-00000d50: 4100 6e00 6d00 6500 6c00 6400 6500 6400  A.n.m.e.l.d.e.d.
-00000d60: 6100 7400 6500 6e08 0000 0000 0600 0000  a.t.e.n.........
-00000d70: 0b43 7265 6465 6e74 6961 6c73 0700 0000  .Credentials....
-00000d80: 0644 6961 6c6f 6701 0300 0000 1400 4100  .Dialog.......A.
-00000d90: 6200 7300 7400 6500 6900 6700 6500 6e00  b.s.t.e.i.g.e.n.
-00000da0: 6408 0000 0000 0600 0000 0a44 6573 6365  d..........Desce
-00000db0: 6e64 696e 6707 0000 0006 4469 616c 6f67  nding.....Dialog
-00000dc0: 0103 0000 003e 0057 0069 0072 006b 0073  .....>.W.i.r.k.s
-00000dd0: 0061 006d 0020 006e 0061 0063 0068 0020  .a.m. .n.a.c.h. 
-00000de0: 0041 006e 0077 0065 006e 0064 0075 006e  .A.n.w.e.n.d.u.n
-00000df0: 0067 0073 006e 0065 0075 0073 0074 0061  .g.s.n.e.u.s.t.a
-00000e00: 0072 0074 0800 0000 0006 0000 0023 4566  .r.t.........#Ef
-00000e10: 6665 6374 6976 6520 6166 7465 7220 6170  fective after ap
-00000e20: 706c 6963 6174 696f 6e20 7265 7374 6172  plication restar
-00000e30: 7407 0000 0006 4469 616c 6f67 0103 ffff  t.....Dialog....
-00000e40: ffff 0800 0000 0006 0000 0006 4578 706f  ............Expo
-00000e50: 7274 0700 0000 0644 6961 6c6f 6701 0300  rt.....Dialog...
-00000e60: 0000 3400 4500 7800 7000 6f00 7200 7400  ..4.E.x.p.o.r.t.
-00000e70: 6900 6500 7200 6500 2000 4300 4200 2d00  i.e.r.e. .C.B.-.
-00000e80: 5100 5300 4f00 7300 2000 6900 6e00 2000  Q.S.O.s. .i.n. .
-00000e90: 4100 4400 4900 4608 0000 0000 0600 0000  A.D.I.F.........
-00000ea0: 1645 7870 6f72 7420 4342 2051 534f 7320  .Export CB QSOs 
-00000eb0: 746f 2041 4449 4607 0000 0006 4469 616c  to ADIF.....Dial
-00000ec0: 6f67 0103 0000 0036 0045 0078 0070 006f  og.....6.E.x.p.o
-00000ed0: 0072 0074 0069 0065 0072 0065 0020 006e  .r.t.i.e.r.e. .n
-00000ee0: 0075 0072 0020 006e 0065 0075 0065 0073  .u.r. .n.e.u.e.s
-00000ef0: 0074 0065 0020 0051 0053 004f 0073 0800  .t.e. .Q.S.O.s..
-00000f00: 0000 0006 0000 0017 4578 706f 7274 206f  ........Export o
-00000f10: 6e6c 7920 7265 6365 6e74 2051 534f 7307  nly recent QSOs.
-00000f20: 0000 0006 4469 616c 6f67 0103 0000 0042  ....Dialog.....B
-00000f30: 0045 0078 0070 006f 0072 0074 0069 0065  .E.x.p.o.r.t.i.e
-00000f40: 0072 0065 0020 0065 0069 0067 0065 006e  .r.e. .e.i.g.e.n
-00000f50: 0065 0020 004e 006f 0074 0069 007a 0065  .e. .N.o.t.i.z.e
-00000f60: 006e 0020 0069 006e 0020 0041 0044 0049  .n. .i.n. .A.D.I
-00000f70: 0046 0800 0000 0006 0000 0018 4578 706f  .F..........Expo
-00000f80: 7274 206f 776e 206e 6f74 6573 2074 6f20  rt own notes to 
-00000f90: 4144 4946 0700 0000 0644 6961 6c6f 6701  ADIF.....Dialog.
-00000fa0: 03ff ffff ff08 0000 0000 0600 0000 0648  ...............H
-00000fb0: 616d 5154 4807 0000 0006 4469 616c 6f67  amQTH.....Dialog
-00000fc0: 0103 ffff ffff 0800 0000 0006 0000 000e  ................
-00000fd0: 4861 6d6c 6962 2072 6967 6374 6c64 0700  Hamlib rigctld..
-00000fe0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000ff0: 0000 0000 0600 0000 0d49 6d70 6f72 742f  .........Import/
-00001000: 4578 706f 7274 0700 0000 0644 6961 6c6f  Export.....Dialo
-00001010: 6701 0300 0000 1a00 5300 6300 6800 6e00  g.......S.c.h.n.
-00001020: 6900 7400 7400 7300 7400 6500 6c00 6c00  i.t.t.s.t.e.l.l.
-00001030: 6508 0000 0000 0600 0000 0949 6e74 6572  e..........Inter
-00001040: 6661 6365 0700 0000 0644 6961 6c6f 6701  face.....Dialog.
-00001050: 0300 0000 2000 6c00 6500 7400 7a00 7400  .... .l.e.t.z.t.
-00001060: 6500 7300 2000 4800 6100 6c00 6200 6a00  e.s. .H.a.l.b.j.
-00001070: 6100 6800 7208 0000 0000 0600 0000 0e4c  a.h.r..........L
-00001080: 6173 7420 6861 6c66 2079 6561 7207 0000  ast half year...
-00001090: 0006 4469 616c 6f67 0103 0000 001a 006c  ..Dialog.......l
-000010a0: 0065 0074 007a 0074 0065 006e 0020 004d  .e.t.z.t.e.n. .M
-000010b0: 006f 006e 0061 0074 0800 0000 0006 0000  .o.n.a.t........
-000010c0: 000a 4c61 7374 206d 6f6e 7468 0700 0000  ..Last month....
-000010d0: 0644 6961 6c6f 6701 0300 0000 1800 6c00  .Dialog.......l.
-000010e0: 6500 7400 7a00 7400 6500 2000 5700 6f00  e.t.z.t.e. .W.o.
-000010f0: 6300 6800 6508 0000 0000 0600 0000 094c  c.h.e..........L
-00001100: 6173 7420 7765 656b 0700 0000 0644 6961  ast week.....Dia
-00001110: 6c6f 6701 0300 0000 1800 6c00 6500 7400  log.......l.e.t.
-00001120: 7a00 7400 6500 7300 2000 4a00 6100 6800  z.t.e.s. .J.a.h.
-00001130: 7208 0000 0000 0600 0000 094c 6173 7420  r..........Last 
-00001140: 7965 6172 0700 0000 0644 6961 6c6f 6701  year.....Dialog.
-00001150: 0300 0000 0c00 4200 7200 6500 6900 7400  ......B.r.e.i.t.
-00001160: 6508 0000 0000 0600 0000 034c 6174 0700  e..........Lat..
-00001170: 0000 0644 6961 6c6f 6701 0300 0000 0a00  ...Dialog.......
-00001180: 5300 7400 7500 6600 6508 0000 0000 0600  S.t.u.f.e.......
-00001190: 0000 054c 6576 656c 0700 0000 0644 6961  ...Level.....Dia
-000011a0: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
-000011b0: 0000 044c 6f54 5707 0000 0006 4469 616c  ...LoTW.....Dial
-000011c0: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
-000011d0: 0007 4c6f 6361 746f 7207 0000 0006 4469  ..Locator.....Di
-000011e0: 616c 6f67 0103 0000 002c 004c 006f 0067  alog.....,.L.o.g
-000011f0: 0020 0069 006e 0020 0044 0061 0074 0065  . .i.n. .D.a.t.e
-00001200: 0069 0020 0073 0063 0068 0072 0065 0069  .i. .s.c.h.r.e.i
-00001210: 0062 0065 006e 0800 0000 0006 0000 000b  .b.e.n..........
-00001220: 4c6f 6720 746f 2066 696c 6507 0000 0006  Log to file.....
-00001230: 4469 616c 6f67 0103 0000 001e 004c 006f  Dialog.......L.o
-00001240: 0067 0067 0069 006e 0067 002d 0041 0075  .g.g.i.n.g.-.A.u
-00001250: 0073 0067 0061 0062 0065 0800 0000 0006  .s.g.a.b.e......
-00001260: 0000 000e 4c6f 6767 696e 6720 6f75 7470  ....Logging outp
-00001270: 7574 0700 0000 0644 6961 6c6f 6701 0300  ut.....Dialog...
-00001280: 0000 0a00 4c00 e400 6e00 6700 6508 0000  ....L...n.g.e...
-00001290: 0000 0600 0000 034c 6f6e 0700 0000 0644  .......Lon.....D
-000012a0: 6961 6c6f 6701 03ff ffff ff08 0000 0000  ialog...........
-000012b0: 0600 0000 044e 616d 6507 0000 0006 4469  .....Name.....Di
-000012c0: 616c 6f67 0103 0000 005e 0043 0042 0020  alog.....^.C.B. 
-000012d0: 0051 0053 004f 0073 0020 0077 0065 0072  .Q.S.O.s. .w.e.r
-000012e0: 0064 0065 006e 0020 0062 0065 0069 006d  .d.e.n. .b.e.i.m
-000012f0: 0020 0049 006d 0070 006f 0072 0074 0020  . .I.m.p.o.r.t. 
-00001300: 0069 006d 006d 0065 0072 0020 0062 0065  .i.m.m.e.r. .b.e
-00001310: 0072 00fc 0063 006b 0073 0069 0063 0068  .r...c.k.s.i.c.h
-00001320: 0074 0069 0067 0074 0800 0000 0006 0000  .t.i.g.t........
-00001330: 0028 4f6e 2069 6d70 6f72 7420 4342 2051  .(On import CB Q
-00001340: 534f 7320 7769 6c6c 2061 6c77 6179 7320  SOs will always 
-00001350: 6265 2068 616e 646c 6564 0700 0000 0644  be handled.....D
-00001360: 6961 6c6f 6701 0300 0000 1000 5000 6100  ialog.......P.a.
-00001370: 7300 7300 7700 6f00 7200 7408 0000 0000  s.s.w.o.r.t.....
-00001380: 0600 0000 0850 6173 7377 6f72 6407 0000  .....Password...
-00001390: 0006 4469 616c 6f67 0103 0000 0070 0050  ..Dialog.....p.P
-000013a0: 0061 0073 0073 0077 006f 0072 0074 0020  .a.s.s.w.o.r.t. 
-000013b0: 0064 0065 0073 0020 004c 006f 0054 0057  .d.e.s. .L.o.T.W
-000013c0: 002d 004f 006e 006c 0069 006e 0065 002d  .-.O.n.l.i.n.e.-
-000013d0: 0041 0063 0063 006f 0075 006e 0074 0073  .A.c.c.o.u.n.t.s
-000013e0: 002c 0020 006e 0069 0063 0068 0074 0020  .,. .n.i.c.h.t. 
-000013f0: 0064 0065 0073 0020 005a 0065 0072 0074  .d.e.s. .Z.e.r.t
-00001400: 0069 0066 0069 006b 0061 0074 0073 0800  .i.f.i.k.a.t.s..
-00001410: 0000 0006 0000 0038 5061 7373 776f 7264  .......8Password
-00001420: 2066 6f72 204c 6f54 5720 6f6e 6c69 6e65   for LoTW online
-00001430: 2061 6363 6f75 6e74 206e 6f74 2066 6f72   account not for
-00001440: 2074 6865 2063 6572 7469 6669 6361 7465   the certificate
-00001450: 0700 0000 0644 6961 6c6f 6701 03ff ffff  .....Dialog.....
-00001460: ff08 0000 0000 0600 0000 0351 5448 0700  ...........QTH..
-00001470: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00001480: 0000 0000 0600 0000 0552 6164 696f 0700  .........Radio..
-00001490: 0000 0644 6961 6c6f 6701 0300 0000 1800  ...Dialog.......
-000014a0: 4e00 6500 7500 6500 7300 7400 6500 2000  N.e.u.e.s.t.e. .
-000014b0: 5100 5300 4f00 7308 0000 0000 0600 0000  Q.S.O.s.........
-000014c0: 0b52 6563 656e 7420 5153 4f73 0700 0000  .Recent QSOs....
-000014d0: 0644 6961 6c6f 6701 0300 0000 1200 4600  .Dialog.......F.
-000014e0: 7500 6e00 6b00 6700 6500 7200 e400 7408  u.n.k.g.e.r...t.
-000014f0: 0000 0000 0600 0000 0352 6967 0700 0000  .........Rig....
-00001500: 0644 6961 6c6f 6701 0300 0000 4c00 5300  .Dialog.....L.S.
-00001510: 6900 6500 6800 6500 2000 4500 6900 6e00  i.e.h.e. .E.i.n.
-00001520: 7300 7400 6500 6c00 6c00 7500 6e00 6700  s.t.e.l.l.u.n.g.
-00001530: 6500 6e00 2000 5200 6500 6900 7400 6500  e.n. .R.e.i.t.e.
-00001540: 7200 2000 2200 4100 6e00 7700 6500 6e00  r. .".A.n.w.e.n.
-00001550: 6400 7500 6e00 6700 2208 0000 0000 0600  d.u.n.g.".......
-00001560: 0000 2253 6565 2073 6574 7469 6e67 7320  .."See settings 
-00001570: 7061 6765 2022 5573 6572 2069 6e74 6572  page "User inter
-00001580: 6661 6365 2207 0000 0006 4469 616c 6f67  face".....Dialog
-00001590: 0103 0000 0034 0043 0042 002d 0042 0061  .....4.C.B.-.B.a
-000015a0: 006e 0064 0020 0061 0075 0074 006f 006d  .n.d. .a.u.t.o.m
-000015b0: 0061 0074 0069 0073 0063 0068 0020 0077  .a.t.i.s.c.h. .w
-000015c0: 00e4 0068 006c 0065 006e 0800 0000 0006  ...h.l.e.n......
-000015d0: 0000 0019 5365 6c65 6374 2043 4220 6261  ....Select CB ba
-000015e0: 6e64 2062 7920 6465 6661 756c 7407 0000  nd by default...
-000015f0: 0006 4469 616c 6f67 0103 0000 001a 0053  ..Dialog.......S
-00001600: 0065 0074 007a 0065 0020 004c 006f 0063  .e.t.z.e. .L.o.c
-00001610: 0061 0074 006f 0072 0800 0000 0006 0000  .a.t.o.r........
-00001620: 000b 5365 7420 6c6f 6361 746f 7207 0000  ..Set locator...
-00001630: 0006 4469 616c 6f67 0103 0000 001a 0045  ..Dialog.......E
-00001640: 0069 006e 0073 0074 0065 006c 006c 0075  .i.n.s.t.e.l.l.u
-00001650: 006e 0067 0065 006e 0800 0000 0006 0000  .n.g.e.n........
-00001660: 0008 5365 7474 696e 6773 0700 0000 0644  ..Settings.....D
-00001670: 6961 6c6f 6701 0300 0000 1c00 5a00 6500  ialog.......Z.e.
-00001680: 6900 6700 6500 2000 5100 5300 4f00 7300  i.g.e. .Q.S.O.s.
-00001690: 2000 6600 fc00 7208 0000 0000 0600 0000   .f...r.........
-000016a0: 0e53 686f 7720 5153 4f73 2066 726f 6d07  .Show QSOs from.
-000016b0: 0000 0006 4469 616c 6f67 0103 0000 0014  ....Dialog......
-000016c0: 007a 0065 0069 0067 0065 0020 0061 006c  .z.e.i.g.e. .a.l
-000016d0: 006c 0065 0800 0000 0006 0000 0008 5368  .l.e..........Sh
-000016e0: 6f77 2061 6c6c 0700 0000 0644 6961 6c6f  ow all.....Dialo
-000016f0: 6701 0300 0000 4000 5300 7000 6100 6c00  g.....@.S.p.a.l.
-00001700: 7400 6500 6e00 2000 6100 6e00 7a00 6500  t.e.n. .a.n.z.e.
-00001710: 6900 6700 6500 6e00 2000 6f00 6400 6500  i.g.e.n. .o.d.e.
-00001720: 7200 2000 7600 6500 7200 7300 7400 6500  r. .v.e.r.s.t.e.
-00001730: 6300 6b00 6500 6e08 0000 0000 0600 0000  c.k.e.n.........
-00001740: 1453 686f 7720 6f72 2068 6964 6520 636f  .Show or hide co
-00001750: 6c75 6d6e 7307 0000 0006 4469 616c 6f67  lumns.....Dialog
-00001760: 0103 0000 0028 0053 006f 0072 0074 0069  .....(.S.o.r.t.i
-00001770: 0065 0072 0065 0020 006e 0061 0063 0068  .e.r.e. .n.a.c.h
-00001780: 0020 0053 0070 0061 006c 0074 0065 0800  . .S.p.a.l.t.e..
-00001790: 0000 0006 0000 000e 536f 7274 206f 6e20  ........Sort on 
-000017a0: 636f 6c75 6d6e 0700 0000 0644 6961 6c6f  column.....Dialo
-000017b0: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-000017c0: 0553 7461 7274 0700 0000 0644 6961 6c6f  .Start.....Dialo
-000017d0: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-000017e0: 0753 7461 7469 6f6e 0700 0000 0644 6961  .Station.....Dia
-000017f0: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
-00001800: 0000 0454 5153 4c07 0000 0006 4469 616c  ...TQSL.....Dial
-00001810: 6f67 0103 0000 0064 0056 0065 0072 0077  og.....d.V.e.r.w
-00001820: 0065 006e 0064 0065 0020 0064 0069 0065  .e.n.d.e. .d.i.e
-00001830: 0020 006b 006f 006e 0066 0069 0067 0075  . .k.o.n.f.i.g.u
-00001840: 0072 0069 0065 0072 0074 0065 0020 0049  .r.i.e.r.t.e. .I
-00001850: 0044 0020 0062 0065 0069 0020 0066 0065  .D. .b.e.i. .f.e
-00001860: 0068 006c 0065 006e 0064 0065 006e 0020  .h.l.e.n.d.e.n. 
-00001870: 0057 0065 0072 0074 0065 006e 0800 0000  .W.e.r.t.e.n....
-00001880: 0006 0000 0024 5573 6520 636f 6e66 6967  .....$Use config
-00001890: 7572 6564 2049 4420 666f 7220 6d69 7373  ured ID for miss
-000018a0: 696e 6720 7661 6c75 6573 0700 0000 0644  ing values.....D
-000018b0: 6961 6c6f 6701 0300 0000 6e00 5600 6500  ialog.....n.V.e.
-000018c0: 7200 7700 6500 6e00 6400 6500 2000 6400  r.w.e.n.d.e. .d.
-000018d0: 6900 6500 2000 6b00 6f00 6e00 6600 6900  i.e. .k.o.n.f.i.
-000018e0: 6700 7500 7200 6900 6500 7200 7400 6500  g.u.r.i.e.r.t.e.
-000018f0: 2000 5300 7400 6100 7400 6900 6f00 6e00   .S.t.a.t.i.o.n.
-00001900: 2000 6200 6500 6900 2000 6600 6500 6800   .b.e.i. .f.e.h.
-00001910: 6c00 6500 6e00 6400 6500 6e00 2000 5700  l.e.n.d.e.n. .W.
-00001920: 6500 7200 7400 6500 6e08 0000 0000 0600  e.r.t.e.n.......
-00001930: 0000 2955 7365 2063 6f6e 6669 6775 7265  ..)Use configure
-00001940: 6420 5374 6174 696f 6e20 666f 7220 6d69  d Station for mi
-00001950: 7373 696e 6720 7661 6c75 6573 0700 0000  ssing values....
-00001960: 0644 6961 6c6f 6701 0300 0000 1200 4100  .Dialog.......A.
-00001970: 6e00 7700 6500 6e00 6400 7500 6e00 6708  n.w.e.n.d.u.n.g.
-00001980: 0000 0000 0600 0000 0e55 7365 7220 696e  .........User in
-00001990: 7465 7266 6163 6507 0000 0006 4469 616c  terface.....Dial
-000019a0: 6f67 0103 0000 0018 0042 0065 006e 0075  og.......B.e.n.u
-000019b0: 0074 007a 0065 0072 006e 0061 006d 0065  .t.z.e.r.n.a.m.e
-000019c0: 0800 0000 0006 0000 0008 5573 6572 6e61  ..........Userna
-000019d0: 6d65 0700 0000 0644 6961 6c6f 6701 0300  me.....Dialog...
-000019e0: 0000 7800 4200 6500 6e00 7500 7400 7a00  ..x.B.e.n.u.t.z.
-000019f0: 6500 7200 6e00 6100 6d00 6500 2000 6400  e.r.n.a.m.e. .d.
-00001a00: 6500 7300 2000 4c00 6f00 5400 5700 2d00  e.s. .L.o.T.W.-.
-00001a10: 4f00 6e00 6c00 6900 6e00 6500 2d00 4100  O.n.l.i.n.e.-.A.
-00001a20: 6300 6300 6f00 7500 6e00 7400 7300 2c00  c.c.o.u.n.t.s.,.
-00001a30: 2000 6e00 6900 6300 6800 7400 2000 6400   .n.i.c.h.t. .d.
-00001a40: 6500 7300 2000 5a00 6500 7200 7400 6900  e.s. .Z.e.r.t.i.
-00001a50: 6600 6900 6b00 6100 7400 7308 0000 0000  f.i.k.a.t.s.....
-00001a60: 0600 0000 3855 7365 726e 616d 6520 666f  ....8Username fo
-00001a70: 7220 4c6f 5457 206f 6e6c 696e 6520 6163  r LoTW online ac
-00001a80: 636f 756e 7420 6e6f 7420 666f 7220 7468  count not for th
-00001a90: 6520 6365 7274 6966 6963 6174 6507 0000  e certificate...
-00001aa0: 0006 4469 616c 6f67 0103 0000 0020 0044  ..Dialog..... .D
-00001ab0: 0061 0074 0065 0069 00fc 0062 0065 0072  .a.t.e.i...b.e.r
-00001ac0: 0077 0061 0063 0068 0075 006e 0067 0800  .w.a.c.h.u.n.g..
-00001ad0: 0000 0006 0000 000a 5761 7463 6820 4669  ........Watch Fi
-00001ae0: 6c65 0700 0000 0644 6961 6c6f 6701 03ff  le.....Dialog...
-00001af0: ffff ff08 0000 0000 0600 0000 0465 5153  .............eQS
-00001b00: 4c07 0000 0006 4469 616c 6f67 0103 ffff  L.....Dialog....
-00001b10: ffff 0800 0000 0006 0000 0002 c2b0 0700  ................
-00001b20: 0000 0644 6961 6c6f 6701 0300 0000 9e00  ...Dialog.......
-00001b30: 4500 6900 6e00 2000 4400 6100 7400 6500  E.i.n. .D.a.t.e.
-00001b40: 6e00 6200 6100 6e00 6b00 2d00 4200 6100  n.b.a.n.k.-.B.a.
-00001b50: 6300 6b00 7500 7000 2000 6b00 6f00 6e00  c.k.u.p. .k.o.n.
-00001b60: 6e00 7400 6500 2000 6e00 6900 6300 6800  n.t.e. .n.i.c.h.
-00001b70: 7400 2000 6500 7200 7300 7400 6500 6c00  t. .e.r.s.t.e.l.
-00001b80: 6c00 7400 2000 7700 6500 7200 6400 6500  l.t. .w.e.r.d.e.
-00001b90: 6e00 2e00 0a00 4400 6900 6500 2000 4400  n.....D.i.e. .D.
-00001ba0: 6100 7400 6500 6900 2000 6500 7800 6900  a.t.e.i. .e.x.i.
-00001bb0: 7300 7400 6900 6500 7200 7400 2000 6200  s.t.i.e.r.t. .b.
-00001bc0: 6500 7200 6500 6900 7400 7300 2e08 0000  e.r.e.i.t.s.....
-00001bd0: 0000 0600 0000 4041 2064 6174 6162 6173  ......@A databas
-00001be0: 6520 6261 636b 7570 2063 6f75 6c64 206e  e backup could n
-00001bf0: 6f74 2062 6520 6372 6561 7465 642e 0a54  ot be created..T
-00001c00: 6865 2066 696c 6520 616c 7265 6164 7920  he file already 
-00001c10: 6578 6973 7473 2e07 0000 0009 4472 6167  exists......Drag
-00001c20: 6f6e 4c6f 6701 0300 0000 4e00 4500 6900  onLog.....N.E.i.
-00001c30: 6e00 2000 4100 4400 4900 4600 2d00 4600  n. .A.D.I.F.-.F.
-00001c40: 6500 6c00 6400 2000 6600 6500 6800 6c00  e.l.d. .f.e.h.l.
-00001c50: 7400 2000 6600 fc00 7200 2000 6400 6500  t. .f...r. .d.e.
-00001c60: 6e00 2000 4c00 6f00 5400 5700 2d00 5500  n. .L.o.T.W.-.U.
-00001c70: 7000 6c00 6f00 6100 6408 0000 0000 0600  p.l.o.a.d.......
-00001c80: 0000 1d41 2066 6965 6c64 2069 7320 6d69  ...A field is mi
-00001c90: 7373 696e 6720 666f 7220 7570 6c6f 6164  ssing for upload
-00001ca0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00001cb0: ffff ffff 0800 0000 0006 0000 0015 4144  ..............AD
-00001cc0: 4946 2033 2028 2a2e 6164 6920 2a2e 6164  IF 3 (*.adi *.ad
-00001cd0: 6966 2907 0000 0009 4472 6167 6f6e 4c6f  if).....DragonLo
-00001ce0: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00001cf0: 1b41 4449 4620 3320 282a 2e61 6478 202a  .ADIF 3 (*.adx *
-00001d00: 2e61 6469 202a 2e61 6469 6629 0700 0000  .adi *.adif)....
-00001d10: 0944 7261 676f 6e4c 6f67 0103 0000 0008  .DragonLog......
-00001d20: 00dc 0062 0065 0072 0800 0000 0006 0000  ...b.e.r........
-00001d30: 0005 4162 6f75 7407 0000 0009 4472 6167  ..About.....Drag
-00001d40: 6f6e 4c6f 6701 0300 0000 0e00 dc00 6200  onLog.........b.
-00001d50: 6500 7200 2000 5100 7408 0000 0000 0600  e.r. .Q.t.......
-00001d60: 0000 0841 626f 7574 2051 7407 0000 0009  ...About Qt.....
-00001d70: 4472 6167 6f6e 4c6f 6701 0300 0000 2000  DragonLog..... .
-00001d80: 4100 6900 7200 6300 7200 6100 6600 7400  A.i.r.c.r.a.f.t.
-00001d90: 2d00 5300 6300 6100 7400 7400 6500 7208  -.S.c.a.t.t.e.r.
-00001da0: 0000 0000 0600 0000 1041 6972 6372 6166  .........Aircraf
-00001db0: 7420 5363 6174 7465 7207 0000 0009 4472  t Scatter.....Dr
-00001dc0: 6167 6f6e 4c6f 6701 0300 0000 0e00 4100  agonLog.......A.
-00001dd0: 6e00 7400 6500 6e00 6e00 6508 0000 0000  n.t.e.n.n.e.....
-00001de0: 0600 0000 0741 6e74 656e 6e61 0700 0000  .....Antenna....
-00001df0: 0944 7261 676f 6e4c 6f67 0103 ffff ffff  .DragonLog......
-00001e00: 0800 0000 0006 0000 0006 4175 726f 7261  ..........Aurora
-00001e10: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00001e20: ffff ffff 0800 0000 0006 0000 0008 4175  ..............Au
-00001e30: 726f 7261 2d45 0700 0000 0944 7261 676f  rora-E.....Drago
-00001e40: 6e4c 6f67 0103 0000 000a 0041 0075 0074  nLog.......A.u.t
-00001e50: 006f 0072 0800 0000 0006 0000 0006 4175  .o.r..........Au
-00001e60: 7468 6f72 0700 0000 0944 7261 676f 6e4c  thor.....DragonL
-00001e70: 6f67 0103 0000 0018 0042 0061 0063 006b  og.......B.a.c.k
-00001e80: 002d 0053 0063 0061 0074 0074 0065 0072  .-.S.c.a.t.t.e.r
-00001e90: 0800 0000 0006 0000 000c 4261 636b 2073  ..........Back s
-00001ea0: 6361 7474 6572 0700 0000 0944 7261 676f  catter.....Drago
-00001eb0: 6e4c 6f67 0103 ffff ffff 0800 0000 0006  nLog............
-00001ec0: 0000 0004 4261 6e64 0700 0000 0944 7261  ....Band.....Dra
-00001ed0: 676f 6e4c 6f67 0103 0000 0022 0043 0053  gonLog.....".C.S
-00001ee0: 0056 002d 0044 0061 0074 0065 0069 0020  .V.-.D.a.t.e.i. 
-00001ef0: 0028 002a 002e 0063 0073 0076 0029 0800  .(.*...c.s.v.)..
-00001f00: 0000 0006 0000 0010 4353 562d 4669 6c65  ........CSV-File
-00001f10: 2028 2a2e 6373 7629 0700 0000 0944 7261   (*.csv).....Dra
-00001f20: 676f 6e4c 6f67 0103 0000 0014 0052 0075  gonLog.......R.u
-00001f30: 0066 007a 0065 0069 0063 0068 0065 006e  .f.z.e.i.c.h.e.n
-00001f40: 0800 0000 0006 0000 0009 4361 6c6c 2073  ..........Call s
-00001f50: 6967 6e07 0000 0009 4472 6167 6f6e 4c6f  ign.....DragonLo
-00001f60: 6701 0300 0000 0a00 4b00 6100 6e00 6100  g.......K.a.n.a.
-00001f70: 6c08 0000 0000 0600 0000 0743 6861 6e6e  l..........Chann
-00001f80: 656c 0700 0000 0944 7261 676f 6e4c 6f67  el.....DragonLog
-00001f90: 0103 0000 0074 0050 0072 00fc 0066 0075  .....t.P.r...f.u
-00001fa0: 006e 0067 0020 0064 0065 0072 0020 0044  .n.g. .d.e.r. .D
-00001fb0: 0061 0074 0065 006e 0062 0061 006e 006b  .a.t.e.n.b.a.n.k
-00001fc0: 0020 0066 0065 0068 006c 0067 0065 0073  . .f.e.h.l.g.e.s
-00001fd0: 0063 0068 006c 0061 0067 0065 006e 002e  .c.h.l.a.g.e.n..
-00001fe0: 0020 0049 006e 0068 0061 006c 0074 0020  . .I.n.h.a.l.t. 
-00001ff0: 006e 0069 0063 0068 0074 0020 006c 0065  .n.i.c.h.t. .l.e
-00002000: 0073 0062 0061 0072 002e 0800 0000 0006  .s.b.a.r........
-00002010: 0000 0034 4368 6563 6b69 6e67 2064 6174  ...4Checking dat
-00002020: 6162 6173 6520 6661 696c 6564 2e20 436f  abase failed. Co
-00002030: 6e74 656e 7420 6973 206e 6f74 2061 6363  ntent is not acc
-00002040: 6573 7361 626c 652e 0700 0000 0944 7261  essable......Dra
-00002050: 676f 6e4c 6f67 0103 0000 0014 004b 006f  gonLog.......K.o
-00002060: 006d 006d 0065 006e 0074 0061 0072 0065  .m.m.e.n.t.a.r.e
-00002070: 0800 0000 0006 0000 0008 436f 6d6d 656e  ..........Commen
-00002080: 7473 0700 0000 0944 7261 676f 6e4c 6f67  ts.....DragonLog
-00002090: 0103 0000 0060 0056 0065 0072 0062 0069  .....`.V.e.r.b.i
-000020a0: 006e 0064 0075 006e 0067 0073 0066 0065  .n.d.u.n.g.s.f.e
-000020b0: 0068 006c 0065 0072 0020 006f 0064 0065  .h.l.e.r. .o.d.e
-000020c0: 0072 0020 004e 0065 0074 007a 0077 0065  .r. .N.e.t.z.w.e
-000020d0: 0072 006b 0020 006e 0069 0063 0068 0074  .r.k. .n.i.c.h.t
-000020e0: 0020 0065 0072 0072 0065 0069 0063 0068  . .e.r.r.e.i.c.h
-000020f0: 0062 0061 0072 0800 0000 0006 0000 0027  .b.a.r.........'
-00002100: 436f 6e6e 6563 7469 6f6e 2065 7272 6f72  Connection error
-00002110: 206f 7220 6e65 7477 6f72 6b20 756e 7265   or network unre
-00002120: 6163 6861 626c 6507 0000 0009 4472 6167  achable.....Drag
-00002130: 6f6e 4c6f 6701 0300 0000 2e00 4400 6100  onLog.......D.a.
-00002140: 7400 6500 6e00 6200 6100 6e00 6b00 2d00  t.e.n.b.a.n.k.-.
-00002150: 4200 6100 6300 6b00 7500 7000 2000 4600  B.a.c.k.u.p. .F.
-00002160: 6500 6800 6c00 6500 7208 0000 0000 0600  e.h.l.e.r.......
-00002170: 0000 1544 6174 6162 6173 6520 6261 636b  ...Database back
-00002180: 7570 2065 7272 6f72 0700 0000 0944 7261  up error.....Dra
-00002190: 676f 6e4c 6f67 0103 0000 002c 0044 0061  gonLog.....,.D.a
-000021a0: 0074 0065 006e 0062 0061 006e 006b 006b  .t.e.n.b.a.n.k.k
-000021b0: 006f 006e 0076 0065 0072 0074 0069 0065  .o.n.v.e.r.t.i.e
-000021c0: 0072 0075 006e 0067 0800 0000 0006 0000  .r.u.n.g........
-000021d0: 0013 4461 7461 6261 7365 2063 6f6e 7665  ..Database conve
-000021e0: 7273 696f 6e07 0000 0009 4472 6167 6f6e  rsion.....Dragon
-000021f0: 4c6f 6701 0300 0000 4800 4400 6100 7400  Log.....H.D.a.t.
-00002200: 6500 6e00 6200 6100 6e00 6b00 6b00 6f00  e.n.b.a.n.k.k.o.
-00002210: 6e00 7600 6500 7200 7400 6900 6500 7200  n.v.e.r.t.i.e.r.
-00002220: 7500 6e00 6700 2000 6100 6200 6700 6500  u.n.g. .a.b.g.e.
-00002230: 7300 6300 6800 6c00 6f00 7300 7300 6500  s.c.h.l.o.s.s.e.
-00002240: 6e08 0000 0000 0600 0000 1c44 6174 6162  n..........Datab
-00002250: 6173 6520 636f 6e76 6572 7369 6f6e 2066  ase conversion f
-00002260: 696e 6973 6865 6407 0000 0009 4472 6167  inished.....Drag
-00002270: 6f6e 4c6f 6701 0300 0000 1e00 4400 6100  onLog.......D.a.
-00002280: 7400 6500 6e00 6200 6100 6e00 6b00 6600  t.e.n.b.a.n.k.f.
-00002290: 6500 6800 6c00 6500 7208 0000 0000 0600  e.h.l.e.r.......
-000022a0: 0000 0e44 6174 6162 6173 6520 6572 726f  ...Database erro
-000022b0: 7207 0000 0009 4472 6167 6f6e 4c6f 6701  r.....DragonLog.
-000022c0: 0300 0000 3400 4400 6100 7400 6500 6e00  ....4.D.a.t.e.n.
-000022d0: 6200 6100 6e00 6b00 7300 7400 7200 7500  b.a.n.k.s.t.r.u.
-000022e0: 6b00 7400 7500 7200 2000 7600 6500 7200  k.t.u.r. .v.e.r.
-000022f0: 6100 6c00 7400 6500 7408 0000 0000 0600  a.l.t.e.t.......
-00002300: 0000 1c44 6174 6162 6173 6520 7374 7275  ...Database stru
-00002310: 6374 7572 6520 6f75 742d 6461 7465 6407  cture out-dated.
-00002320: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-00002330: 0000 1e00 4400 6100 7400 7500 6d00 2f00  ....D.a.t.u.m./.
-00002340: 5a00 6500 6900 7400 2000 4500 6e00 6400  Z.e.i.t. .E.n.d.
-00002350: 6508 0000 0000 0600 0000 0d44 6174 652f  e..........Date/
-00002360: 5469 6d65 2065 6e64 0700 0000 0944 7261  Time end.....Dra
-00002370: 676f 6e4c 6f67 0103 0000 0020 0044 0061  gonLog..... .D.a
-00002380: 0074 0075 006d 002f 005a 0065 0069 0074  .t.u.m./.Z.e.i.t
-00002390: 0020 0053 0074 0061 0072 0074 0800 0000  . .S.t.a.r.t....
-000023a0: 0006 0000 000f 4461 7465 2f54 696d 6520  ......Date/Time 
-000023b0: 7374 6172 7407 0000 0009 4472 6167 6f6e  start.....Dragon
-000023c0: 4c6f 6701 0300 0000 1600 5100 5300 4f00  Log.......Q.S.O.
-000023d0: 2000 6c00 f600 7300 6300 6800 6500 6e08   .l...s.c.h.e.n.
-000023e0: 0000 0000 0600 0000 0a44 656c 6574 6520  .........Delete 
-000023f0: 5153 4f07 0000 0009 4472 6167 6f6e 4c6f  QSO.....DragonLo
-00002400: 6701 0300 0000 1400 4500 6e00 7400 6600  g.......E.n.t.f.
-00002410: 6500 7200 6e00 7500 6e00 6708 0000 0000  e.r.n.u.n.g.....
-00002420: 0600 0000 0844 6973 7461 6e63 6507 0000  .....Distance...
-00002430: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00002440: 6400 5700 6f00 6c00 6c00 6500 6e00 2000  d.W.o.l.l.e.n. .
-00002450: 7300 6900 6500 2000 6400 6900 6500 2000  s.i.e. .d.i.e. .
-00002460: 7300 6500 6c00 6500 6b00 7400 6900 6500  s.e.l.e.k.t.i.e.
-00002470: 7200 7400 6500 6e00 2000 5100 5300 4f00  r.t.e.n. .Q.S.O.
-00002480: 7300 2000 7700 6900 7200 6b00 6c00 6900  s. .w.i.r.k.l.i.
-00002490: 6300 6800 2000 6c00 f600 7300 6300 6800  c.h. .l...s.c.h.
-000024a0: 6500 6e00 3f08 0000 0000 0600 0000 3144  e.n.?.........1D
-000024b0: 6f20 796f 7520 7265 616c 6c79 2077 616e  o you really wan
-000024c0: 7420 746f 2064 656c 6574 6520 7468 6520  t to delete the 
-000024d0: 7365 6c65 6374 6564 2051 534f 2873 293f  selected QSO(s)?
-000024e0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-000024f0: ffff ffff 0800 0000 0006 0000 0010 4561  ..............Ea
-00002500: 7274 682d 4d6f 6f6e 2d45 6172 7468 0700  rth-Moon-Earth..
-00002510: 0000 0944 7261 676f 6e4c 6f67 0103 ffff  ...DragonLog....
-00002520: ffff 0800 0000 0006 0000 0008 4563 686f  ............Echo
-00002530: 4c69 6e6b 0700 0000 0944 7261 676f 6e4c  Link.....DragonL
-00002540: 6f67 0103 0000 000c 0046 0065 0068 006c  og.......F.e.h.l
-00002550: 0065 0072 0800 0000 0006 0000 0005 4572  .e.r..........Er
-00002560: 726f 7207 0000 0009 4472 6167 6f6e 4c6f  ror.....DragonLo
-00002570: 6701 0300 0000 2800 4500 7800 6300 6500  g.....(.E.x.c.e.
-00002580: 6c00 2d00 4400 6100 7400 6500 6900 2000  l.-.D.a.t.e.i. .
-00002590: 2800 2a00 2e00 7800 6c00 7300 7800 2908  (.*...x.l.s.x.).
-000025a0: 0000 0000 0600 0000 1345 7863 656c 2d46  .........Excel-F
-000025b0: 696c 6520 282a 2e78 6c73 7829 0700 0000  ile (*.xlsx)....
-000025c0: 0944 7261 676f 6e4c 6f67 0103 0000 0024  .DragonLog.....$
-000025d0: 0045 0078 0070 006f 0072 0074 0069 0065  .E.x.p.o.r.t.i.e
-000025e0: 0072 0065 0020 0051 0053 004f 0020 006c  .r.e. .Q.S.O. .l
-000025f0: 006f 0067 0800 0000 0006 0000 0010 4578  .o.g..........Ex
-00002600: 706f 7274 6564 2051 534f 206c 6f67 0700  ported QSO log..
-00002610: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00002620: 001a 0046 0032 002d 0052 0065 0066 006c  ...F.2.-.R.e.f.l
-00002630: 0065 006b 0074 0069 006f 006e 0800 0000  .e.k.t.i.o.n....
-00002640: 0006 0000 000d 4632 2052 6566 6c65 6374  ......F2 Reflect
-00002650: 696f 6e07 0000 0009 4472 6167 6f6e 4c6f  ion.....DragonLo
-00002660: 6701 0300 0000 3800 4600 6900 6500 6c00  g.....8.F.i.e.l.
-00002670: 6400 2d00 4100 6c00 6900 6700 6e00 6500  d.-.A.l.i.g.n.e.
-00002680: 6400 2d00 4900 7200 7200 6500 6700 7500  d.-.I.r.r.e.g.u.
-00002690: 6c00 6100 7200 6900 7400 6900 6500 7308  l.a.r.i.t.i.e.s.
-000026a0: 0000 0000 0600 0000 1c46 6965 6c64 2041  .........Field A
-000026b0: 6c69 676e 6564 2049 7272 6567 756c 6172  ligned Irregular
-000026c0: 6974 6965 7307 0000 0009 4472 6167 6f6e  ities.....Dragon
-000026d0: 4c6f 6701 0300 0000 1000 4600 7200 6500  Log.......F.r.e.
-000026e0: 7100 7500 6500 6e00 7a08 0000 0000 0600  q.u.e.n.z.......
-000026f0: 0000 0946 7265 7175 656e 6379 0700 0000  ...Frequency....
-00002700: 0944 7261 676f 6e4c 6f67 0103 0000 0014  .DragonLog......
-00002710: 0042 006f 0064 0065 006e 0077 0065 006c  .B.o.d.e.n.w.e.l
-00002720: 006c 0065 0800 0000 0006 0000 000b 4772  .l.e..........Gr
-00002730: 6f75 6e64 2057 6176 6507 0000 0009 4472  ound Wave.....Dr
-00002740: 6167 6f6e 4c6f 6701 03ff ffff ff08 0000  agonLog.........
-00002750: 0000 0600 0000 0648 616d 5154 4807 0000  .......HamQTH...
-00002760: 0009 4472 6167 6f6e 4c6f 6701 03ff ffff  ..DragonLog.....
-00002770: ff08 0000 0000 0600 0000 0648 616d 6c69  ...........Hamli
-00002780: 6207 0000 0009 4472 6167 6f6e 4c6f 6701  b.....DragonLog.
-00002790: 0300 0000 0a00 4800 6900 6c00 6600 6508  ......H.i.l.f.e.
-000027a0: 0000 0000 0600 0000 0448 656c 7007 0000  .........Help...
-000027b0: 0009 4472 6167 6f6e 4c6f 6701 03ff ffff  ..DragonLog.....
-000027c0: ff08 0000 0000 0600 0000 0449 524c 5007  ...........IRLP.
-000027d0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-000027e0: 0000 2600 4900 6e00 7400 6500 7200 6e00  ..&.I.n.t.e.r.n.
-000027f0: 6500 7400 7500 6e00 7400 6500 7200 7300  e.t.u.n.t.e.r.s.
-00002800: 7400 fc00 7400 7a00 7408 0000 0000 0600  t...t.z.t.......
-00002810: 0000 1149 6e74 6572 6e65 742d 6173 7369  ...Internet-assi
-00002820: 7374 6564 0700 0000 0944 7261 676f 6e4c  sted.....DragonL
-00002830: 6f67 0103 0000 0018 0049 006f 006e 006f  og.......I.o.n.o
-00002840: 002d 0053 0063 0061 0074 0074 0065 0072  .-.S.c.a.t.t.e.r
-00002850: 0800 0000 0006 0000 000b 496f 6e6f 7363  ..........Ionosc
-00002860: 6174 7465 7207 0000 0009 4472 6167 6f6e  atter.....Dragon
-00002870: 4c6f 6701 0300 0000 2000 6c00 6500 7400  Log..... .l.e.t.
-00002880: 7a00 7400 6500 7300 2000 4800 6100 6c00  z.t.e.s. .H.a.l.
-00002890: 6200 6a00 6100 6800 7208 0000 0000 0600  b.j.a.h.r.......
-000028a0: 0000 0e4c 6173 7420 6861 6c66 2079 6561  ...Last half yea
-000028b0: 7207 0000 0009 4472 6167 6f6e 4c6f 6701  r.....DragonLog.
-000028c0: 0300 0000 1a00 6c00 6500 7400 7a00 7400  ......l.e.t.z.t.
-000028d0: 6500 6e00 2000 4d00 6f00 6e00 6100 7408  e.n. .M.o.n.a.t.
-000028e0: 0000 0000 0600 0000 0a4c 6173 7420 6d6f  .........Last mo
-000028f0: 6e74 6807 0000 0009 4472 6167 6f6e 4c6f  nth.....DragonLo
-00002900: 6701 0300 0000 1800 6c00 6500 7400 7a00  g.......l.e.t.z.
-00002910: 7400 6500 2000 5700 6f00 6300 6800 6508  t.e. .W.o.c.h.e.
-00002920: 0000 0000 0600 0000 094c 6173 7420 7765  .........Last we
-00002930: 656b 0700 0000 0944 7261 676f 6e4c 6f67  ek.....DragonLog
-00002940: 0103 0000 0018 006c 0065 0074 007a 0074  .......l.e.t.z.t
-00002950: 0065 0073 0020 004a 0061 0068 0072 0800  .e.s. .J.a.h.r..
-00002960: 0000 0006 0000 0009 4c61 7374 2079 6561  ........Last yea
-00002970: 7207 0000 0009 4472 6167 6f6e 4c6f 6701  r.....DragonLog.
-00002980: 0300 0000 1e00 5300 6900 6300 6800 7400  ......S.i.c.h.t.
-00002990: 7600 6500 7200 6200 6900 6e00 6400 7500  v.e.r.b.i.n.d.u.
-000029a0: 6e00 6708 0000 0000 0600 0000 0d4c 696e  n.g..........Lin
-000029b0: 6520 6f66 2053 6967 6874 0700 0000 0944  e of Sight.....D
-000029c0: 7261 676f 6e4c 6f67 0103 0000 0020 004c  ragonLog..... .L
-000029d0: 006f 0054 0057 002d 0041 0044 0049 0046  .o.T.W.-.A.D.I.F
-000029e0: 002d 0055 0070 006c 006f 0061 0064 0800  .-.U.p.l.o.a.d..
-000029f0: 0000 0006 0000 0010 4c6f 5457 2041 4449  ........LoTW ADI
-00002a00: 4620 7570 6c6f 6164 0700 0000 0944 7261  F upload.....Dra
-00002a10: 676f 6e4c 6f67 0103 0000 0014 004c 006f  gonLog.......L.o
-00002a20: 0054 0057 0020 0065 006d 0070 0066 002e  .T.W. .e.m.p.f..
-00002a30: 0800 0000 0006 0000 0009 4c6f 5457 2072  ..........LoTW r
-00002a40: 6376 6407 0000 0009 4472 6167 6f6e 4c6f  cvd.....DragonLo
-00002a50: 6701 0300 0000 1400 4c00 6f00 5400 5700  g.......L.o.T.W.
-00002a60: 2000 7600 6500 7200 7300 2e08 0000 0000   .v.e.r.s.......
-00002a70: 0600 0000 094c 6f54 5720 7365 6e74 0700  .....LoTW sent..
-00002a80: 0000 0944 7261 676f 6e4c 6f67 0103 ffff  ...DragonLog....
-00002a90: ffff 0800 0000 0006 0000 0007 4c6f 6361  ............Loca
-00002aa0: 746f 7207 0000 0009 4472 6167 6f6e 4c6f  tor.....DragonLo
-00002ab0: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00002ac0: 0f4c 6f67 2069 6d70 6f72 7420 4144 4946  .Log import ADIF
-00002ad0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00002ae0: 0000 001c 004c 006f 0067 0020 0049 006d  .....L.o.g. .I.m
-00002af0: 0070 006f 0072 0074 0020 0043 0053 0056  .p.o.r.t. .C.S.V
-00002b00: 0800 0000 0006 0000 000e 4c6f 6720 696d  ..........Log im
-00002b10: 706f 7274 2043 5356 0700 0000 0944 7261  port CSV.....Dra
-00002b20: 676f 6e4c 6f67 0103 0000 0020 004c 006f  gonLog..... .L.o
-00002b30: 0067 0020 0049 006d 0070 006f 0072 0074  .g. .I.m.p.o.r.t
-00002b40: 0020 0045 0078 0063 0065 006c 0800 0000  . .E.x.c.e.l....
-00002b50: 0006 0000 0010 4c6f 6720 696d 706f 7274  ......Log import
-00002b60: 2045 7863 656c 0700 0000 0944 7261 676f   Excel.....Drago
-00002b70: 6e4c 6f67 0103 0000 001c 004d 0065 0074  nLog.......M.e.t
-00002b80: 0065 006f 0072 002d 0053 0063 0061 0074  .e.o.r.-.S.c.a.t
-00002b90: 0074 0065 0072 0800 0000 0006 0000 000e  .t.e.r..........
-00002ba0: 4d65 7465 6f72 2073 6361 7474 6572 0700  Meteor scatter..
-00002bb0: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00002bc0: 005a 004b 0065 0069 006e 0065 0020 0053  .Z.K.e.i.n.e. .S
-00002bd0: 0074 0061 0074 0069 006f 006e 0073 006b  .t.a.t.i.o.n.s.k
-00002be0: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
-00002bf0: 0074 0069 006f 006e 0020 0069 006e 0020  .t.i.o.n. .i.n. 
-00002c00: 0054 0051 0053 004c 0020 0076 0065 0072  .T.Q.S.L. .v.e.r
-00002c10: 0066 00fc 0067 0062 0061 0072 0800 0000  .f...g.b.a.r....
-00002c20: 0006 0000 0025 4d69 7373 696e 6720 7374  .....%Missing st
-00002c30: 6174 696f 6e20 636f 6e66 6967 7572 6174  ation configurat
-00002c40: 696f 6e20 696e 2054 5153 4c07 0000 0009  ion in TQSL.....
-00002c50: 4472 6167 6f6e 4c6f 6701 03ff ffff ff08  DragonLog.......
-00002c60: 0000 0000 0600 0000 044d 6f64 6507 0000  .........Mode...
-00002c70: 0009 4472 6167 6f6e 4c6f 6701 03ff ffff  ..DragonLog.....
-00002c80: ff08 0000 0000 0600 0000 044e 616d 6507  ...........Name.
-00002c90: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-00002ca0: 0000 3400 4b00 6500 6900 6e00 6500 2000  ..4.K.e.i.n.e. .
-00002cb0: 5100 5300 4f00 7300 2000 6600 fc00 7200  Q.S.O.s. .f...r.
-00002cc0: 2000 6400 6500 6e00 2000 4c00 6f00 6300   .d.e.n. .L.o.c.
-00002cd0: 6100 7400 6f00 7208 0000 0000 0600 0000  a.t.o.r.........
-00002ce0: 174e 6f20 7265 636f 7264 7320 666f 7220  .No records for 
-00002cf0: 6c6f 6361 7469 6f6e 0700 0000 0944 7261  location.....Dra
-00002d00: 676f 6e4c 6f67 0103 0000 000e 004e 006f  gonLog.......N.o
-00002d10: 0074 0069 007a 0065 006e 0800 0000 0006  .t.i.z.e.n......
-00002d20: 0000 0005 4e6f 7465 7307 0000 0009 4472  ....Notes.....Dr
-00002d30: 6167 6f6e 4c6f 6701 03ff ffff ff08 0000  agonLog.........
-00002d40: 0000 0600 0000 024f 6b07 0000 0009 4472  .......Ok.....Dr
-00002d50: 6167 6f6e 4c6f 6701 0300 0000 1e00 4500  agonLog.......E.
-00002d60: 6900 6700 6500 6e00 6500 7200 2000 4c00  i.g.e.n.e.r. .L.
-00002d70: 6f00 6300 6100 7400 6f00 7208 0000 0000  o.c.a.t.o.r.....
-00002d80: 0600 0000 0b4f 776e 204c 6f63 6174 6f72  .....Own Locator
-00002d90: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00002da0: 0000 0018 0045 0069 0067 0065 006e 0065  .....E.i.g.e.n.e
-00002db0: 0072 0020 004e 0061 006d 0065 0800 0000  .r. .N.a.m.e....
-00002dc0: 0006 0000 0008 4f77 6e20 4e61 6d65 0700  ......Own Name..
-00002dd0: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00002de0: 0016 0045 0069 0067 0065 006e 0065 0072  ...E.i.g.e.n.e.r
-00002df0: 0020 0051 0054 0048 0800 0000 0006 0000  . .Q.T.H........
-00002e00: 0007 4f77 6e20 5154 4807 0000 0009 4472  ..Own QTH.....Dr
-00002e10: 6167 6f6e 4c6f 6701 0300 0000 2400 4500  agonLog.....$.E.
-00002e20: 6900 6700 6500 6e00 6500 7300 2000 5200  i.g.e.n.e.s. .R.
-00002e30: 7500 6600 7a00 6500 6900 6300 6800 6500  u.f.z.e.i.c.h.e.
-00002e40: 6e08 0000 0000 0600 0000 0d4f 776e 2063  n..........Own c
-00002e50: 616c 6c20 7369 676e 0700 0000 0944 7261  all sign.....Dra
-00002e60: 676f 6e4c 6f67 0103 0000 0010 004c 0065  gonLog.......L.e
-00002e70: 0069 0073 0074 0075 006e 0067 0800 0000  .i.s.t.u.n.g....
-00002e80: 0006 0000 0005 506f 7765 7207 0000 0009  ......Power.....
-00002e90: 4472 6167 6f6e 4c6f 6701 0300 0000 1600  DragonLog.......
-00002ea0: 4100 7500 7300 6200 7200 6500 6900 7400  A.u.s.b.r.e.i.t.
-00002eb0: 7500 6e00 6708 0000 0000 0600 0000 0b50  u.n.g..........P
-00002ec0: 726f 7061 6761 7469 6f6e 0700 0000 0944  ropagation.....D
-00002ed0: 7261 676f 6e4c 6f67 0103 0000 001a 0051  ragonLog.......Q
-00002ee0: 0053 004c 002d 004e 0061 0063 0068 0072  .S.L.-.N.a.c.h.r
-00002ef0: 0069 0063 0068 0074 0800 0000 0006 0000  .i.c.h.t........
-00002f00: 000b 5153 4c20 6d65 7373 6167 6507 0000  ..QSL message...
-00002f10: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00002f20: 1000 5100 5300 4c00 2d00 5000 6600 6100  ..Q.S.L.-.P.f.a.
-00002f30: 6408 0000 0000 0600 0000 0851 534c 2070  d..........QSL p
-00002f40: 6174 6807 0000 0009 4472 6167 6f6e 4c6f  ath.....DragonLo
-00002f50: 6701 0300 0000 1200 5100 5300 4c00 2000  g.......Q.S.L. .
-00002f60: 6500 6d00 7000 6600 2e08 0000 0000 0600  e.m.p.f.........
-00002f70: 0000 0851 534c 2072 6376 6407 0000 0009  ...QSL rcvd.....
-00002f80: 4472 6167 6f6e 4c6f 6701 0300 0000 1200  DragonLog.......
-00002f90: 5100 5300 4c00 2000 7600 6500 7200 7300  Q.S.L. .v.e.r.s.
-00002fa0: 2e08 0000 0000 0600 0000 0851 534c 2073  ...........QSL s
-00002fb0: 656e 7407 0000 0009 4472 6167 6f6e 4c6f  ent.....DragonLo
-00002fc0: 6701 0300 0000 0e00 5100 5300 4c00 2d00  g.......Q.S.L.-.
-00002fd0: 5600 6900 6108 0000 0000 0600 0000 0751  V.i.a..........Q
-00002fe0: 534c 2076 6961 0700 0000 0944 7261 676f  SL via.....Drago
-00002ff0: 6e4c 6f67 0103 ffff ffff 0800 0000 0006  nLog............
-00003000: 0000 0003 5153 4f07 0000 0009 4472 6167  ....QSO.....Drag
-00003010: 6f6e 4c6f 6701 0300 0000 4800 5100 5300  onLog.....H.Q.S.
-00003020: 4f00 2d00 4c00 6f00 6700 2000 2800 2a00  O.-.L.o.g. .(.*.
-00003030: 2e00 7100 6c00 6f00 6700 2900 3b00 3b00  ..q.l.o.g.).;.;.
-00003040: 4100 6c00 6c00 6500 2000 4400 6100 7400  A.l.l.e. .D.a.t.
-00003050: 6500 6900 6500 6e00 2000 2800 2a00 2e00  e.i.e.n. .(.*...
-00003060: 2a00 2908 0000 0000 0600 0000 2151 534f  *.).........!QSO
-00003070: 2d4c 6f67 2028 2a2e 716c 6f67 293b 3b41  -Log (*.qlog);;A
-00003080: 6c6c 2046 696c 6573 2028 2a2e 2a29 0700  ll Files (*.*)..
-00003090: 0000 0944 7261 676f 6e4c 6f67 0103 ffff  ...DragonLog....
-000030a0: ffff 0800 0000 0006 0000 0003 5154 4807  ............QTH.
-000030b0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-000030c0: 0000 1200 5200 5300 5400 2000 6500 6d00  ....R.S.T. .e.m.
-000030d0: 7000 6600 2e08 0000 0000 0600 0000 0852  p.f............R
-000030e0: 5354 2072 6376 6407 0000 0009 4472 6167  ST rcvd.....Drag
-000030f0: 6f6e 4c6f 6701 0300 0000 1000 5200 5300  onLog.......R.S.
-00003100: 5400 2000 6700 6500 7300 2e08 0000 0000  T. .g.e.s.......
-00003110: 0600 0000 0852 5354 2073 656e 7407 0000  .....RST sent...
-00003120: 0009 4472 6167 6f6e 4c6f 6701 03ff ffff  ..DragonLog.....
-00003130: ff08 0000 0000 0600 0000 0552 6164 696f  ...........Radio
-00003140: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00003150: 0000 0018 0052 0061 0069 006e 002d 0053  .....R.a.i.n.-.S
-00003160: 0063 0061 0074 0074 0065 0072 0800 0000  .c.a.t.t.e.r....
-00003170: 0006 0000 000c 5261 696e 2073 6361 7474  ......Rain scatt
-00003180: 6572 0700 0000 0944 7261 676f 6e4c 6f67  er.....DragonLog
-00003190: 0103 0000 0032 0052 0065 0070 0065 0061  .....2.R.e.p.e.a
-000031a0: 0074 0065 0072 0020 006f 0064 0065 0072  .t.e.r. .o.d.e.r
-000031b0: 0020 0054 0072 0061 006e 0073 0070 006f  . .T.r.a.n.s.p.o
-000031c0: 006e 0064 0065 0072 0800 0000 0006 0000  .n.d.e.r........
-000031d0: 0017 5265 7065 6174 6572 206f 7220 5472  ..Repeater or Tr
-000031e0: 616e 7370 6f6e 6465 7207 0000 0009 4472  ansponder.....Dr
-000031f0: 6167 6f6e 4c6f 6701 0300 0000 1000 5300  agonLog.......S.
-00003200: 6100 7400 6500 6c00 6c00 6900 7408 0000  a.t.e.l.l.i.t...
-00003210: 0000 0600 0000 0953 6174 656c 6c69 7465  .......Satellite
-00003220: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00003230: 0000 002a 0045 0078 0070 006f 0072 0074  ...*.E.x.p.o.r.t
-00003240: 0064 0061 0074 0065 0069 0020 0073 0070  .d.a.t.e.i. .s.p
-00003250: 0065 0069 0063 0068 0065 0072 006e 0800  .e.i.c.h.e.r.n..
-00003260: 0000 0006 0000 0012 5365 6c65 6374 2065  ........Select e
-00003270: 7870 6f72 7420 6669 6c65 0700 0000 0944  xport file.....D
-00003280: 7261 676f 6e4c 6f67 0103 0000 0020 0044  ragonLog..... .D
-00003290: 0061 0074 0065 006e 0062 0061 006e 006b  .a.t.e.n.b.a.n.k
-000032a0: 0020 00f6 0066 0066 006e 0065 006e 0800  . ...f.f.n.e.n..
-000032b0: 0000 0006 0000 000b 5365 6c65 6374 2066  ........Select f
-000032c0: 696c 6507 0000 0009 4472 6167 6f6e 4c6f  ile.....DragonLo
-000032d0: 6701 0300 0000 3800 5a00 7500 2000 fc00  g.....8.Z.u. ...
-000032e0: 6200 6500 7200 7700 6100 6300 6800 6500  b.e.r.w.a.c.h.e.
-000032f0: 6e00 6400 6500 2000 4400 6100 7400 6500  n.d.e. .D.a.t.e.
-00003300: 6900 2000 7700 e400 6800 6c00 6500 6e08  i. .w...h.l.e.n.
-00003310: 0000 0000 0600 0000 1453 656c 6563 7420  .........Select 
-00003320: 6669 6c65 2074 6f20 7761 7463 6807 0000  file to watch...
-00003330: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00003340: 2400 4900 6d00 7000 6f00 7200 7400 6400  $.I.m.p.o.r.t.d.
-00003350: 6100 7400 6500 6900 2000 f600 6600 6600  a.t.e.i. ...f.f.
-00003360: 6e00 6500 6e08 0000 0000 0600 0000 1253  n.e.n..........S
-00003370: 656c 6563 7420 696d 706f 7274 2066 696c  elect import fil
-00003380: 6507 0000 0009 4472 6167 6f6e 4c6f 6701  e.....DragonLog.
-00003390: 0300 0000 1a00 5700 e400 6800 6c00 6500  ......W...h.l.e.
-000033a0: 2000 5300 7400 6100 7400 6900 6f00 6e08   .S.t.a.t.i.o.n.
-000033b0: 0000 0000 0600 0000 0e53 656c 6563 7420  .........Select 
-000033c0: 7374 6174 696f 6e07 0000 0009 4472 6167  station.....Drag
-000033d0: 6f6e 4c6f 6701 0300 0000 4400 4c00 6f00  onLog.....D.L.o.
-000033e0: 5400 5700 2d00 5300 6500 7200 7600 6500  T.W.-.S.e.r.v.e.
-000033f0: 7200 2000 6800 6100 7400 2000 6400 6100  r. .h.a.t. .d.a.
-00003400: 7300 2000 4c00 6f00 6700 2000 6100 6200  s. .L.o.g. .a.b.
-00003410: 6700 6500 7700 6900 6500 7300 6500 6e08  g.e.w.i.e.s.e.n.
-00003420: 0000 0000 0600 0000 1353 6572 7665 7220  .........Server 
-00003430: 7265 6a65 6374 6564 206c 6f67 0700 0000  rejected log....
-00003440: 0944 7261 676f 6e4c 6f67 0103 0000 0014  .DragonLog......
-00003450: 007a 0065 0069 0067 0065 0020 0061 006c  .z.e.i.g.e. .a.l
-00003460: 006c 0065 0800 0000 0006 0000 0008 5368  .l.e..........Sh
-00003470: 6f77 2061 6c6c 0700 0000 0944 7261 676f  ow all.....Drago
-00003480: 6e4c 6f67 0103 0000 0014 0053 0070 006f  nLog.......S.p.o
-00003490: 0072 0061 0064 0069 0063 002d 0045 0800  .r.a.d.i.c.-.E..
-000034a0: 0000 0006 0000 000a 5370 6f72 6164 6963  ........Sporadic
-000034b0: 2045 0700 0000 0944 7261 676f 6e4c 6f67   E.....DragonLog
-000034c0: 0103 ffff ffff 0800 0000 0006 0000 0007  ................
-000034d0: 5375 626d 6f64 6507 0000 0009 4472 6167  Submode.....Drag
-000034e0: 6f6e 4c6f 6701 0300 0000 2a00 5400 5100  onLog.....*.T.Q.
-000034f0: 5300 4c00 2d00 5300 6900 6700 6e00 6100  S.L.-.S.i.g.n.a.
-00003500: 7400 7500 7200 7000 6100 7300 7300 7700  t.u.r.p.a.s.s.w.
-00003510: 6f00 7200 7408 0000 0000 0600 0000 1754  o.r.t..........T
-00003520: 5153 4c20 7369 676e 6174 7572 6520 7061  QSL signature pa
-00003530: 7373 776f 7264 0700 0000 0944 7261 676f  ssword.....Drago
-00003540: 6e4c 6f67 0103 0000 00b2 0044 0069 0065  nLog.......D.i.e
-00003550: 0020 0044 0061 0074 0065 006e 0062 0061  . .D.a.t.e.n.b.a
-00003560: 006e 006b 0073 0074 0072 0075 006b 0074  .n.k.s.t.r.u.k.t
-00003570: 0075 0072 0020 0069 0073 0074 0020 0076  .u.r. .i.s.t. .v
-00003580: 0065 0072 0061 006c 0074 0065 0074 0020  .e.r.a.l.t.e.t. 
-00003590: 0075 006e 0064 0020 006d 0075 0073 0073  .u.n.d. .m.u.s.s
-000035a0: 0020 006b 006f 006e 0076 0065 0072 0074  . .k.o.n.v.e.r.t
-000035b0: 0069 0065 0072 0074 0020 0077 0065 0072  .i.e.r.t. .w.e.r
-000035c0: 0064 0065 006e 000a 000a 0045 0069 006e  .d.e.n.....E.i.n
-000035d0: 0020 0042 0061 0063 006b 0075 0070 0020  . .B.a.c.k.u.p. 
-000035e0: 0077 0069 0072 0064 0020 0065 0072 0073  .w.i.r.d. .e.r.s
-000035f0: 0074 0065 006c 006c 0074 003a 0800 0000  .t.e.l.l.t.:....
-00003600: 0006 0000 0057 5468 6520 6461 7461 6261  .....WThe databa
-00003610: 7365 2073 7472 7563 7475 7265 2069 7320  se structure is 
-00003620: 6f75 742d 6461 7465 6420 616e 6420 6e65  out-dated and ne
-00003630: 6564 7320 6120 636f 6e76 6572 7369 6f6e  eds a conversion
-00003640: 0a0a 4120 6261 636b 7570 2077 696c 6c20  ..A backup will 
-00003650: 6265 2067 656e 6572 6174 6564 3a07 0000  be generated:...
-00003660: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00003670: 1e00 5400 7200 6100 6e00 7300 6500 7100  ..T.r.a.n.s.e.q.
-00003680: 7500 6100 7400 6f00 7200 6900 6100 6c08  u.a.t.o.r.i.a.l.
-00003690: 0000 0000 0600 0000 1054 7261 6e73 2d65  .........Trans-e
-000036a0: 7175 6174 6f72 6961 6c07 0000 0009 4472  quatorial.....Dr
-000036b0: 6167 6f6e 4c6f 6701 0300 0000 2800 5400  agonLog.....(.T.
-000036c0: 7200 6f00 7000 6f00 7300 7000 6800 6500  r.o.p.o.s.p.h.e.
-000036d0: 7200 6900 6300 2d00 4400 7500 6300 7400  r.i.c.-.D.u.c.t.
-000036e0: 6900 6e00 6708 0000 0000 0600 0000 1454  i.n.g..........T
-000036f0: 726f 706f 7370 6865 7269 6320 6475 6374  ropospheric duct
-00003700: 696e 6707 0000 0009 4472 6167 6f6e 4c6f  ing.....DragonLo
-00003710: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00003720: 0756 6572 7369 6f6e 0700 0000 0944 7261  .Version.....Dra
-00003730: 676f 6e4c 6f67 0103 0000 002c 0050 0072  gonLog.....,.P.r
-00003740: 006f 0067 0072 0061 006d 006d 006c 006f  .o.g.r.a.m.m.l.o
-00003750: 0067 0020 00fc 0062 0065 0072 0077 0061  .g. ...b.e.r.w.a
-00003760: 0063 0068 0065 006e 0800 0000 0006 0000  .c.h.e.n........
-00003770: 0015 5761 7463 6820 6170 706c 6963 6174  ..Watch applicat
-00003780: 696f 6e20 6c6f 6707 0000 0009 4472 6167  ion log.....Drag
-00003790: 6f6e 4c6f 6701 0300 0000 2000 4400 6100  onLog..... .D.a.
-000037a0: 7400 6500 6900 fc00 6200 6500 7200 7700  t.e.i...b.e.r.w.
-000037b0: 6100 6300 6800 7500 6e00 6708 0000 0000  a.c.h.u.n.g.....
-000037c0: 0600 0000 0d57 6174 6368 696e 6720 6669  .....Watching fi
-000037d0: 6c65 0700 0000 0944 7261 676f 6e4c 6f67  le.....DragonLog
-000037e0: 0103 0000 0014 0065 0051 0053 004c 0020  .......e.Q.S.L. 
-000037f0: 0065 006d 0070 0066 002e 0800 0000 0006  .e.m.p.f........
-00003800: 0000 0009 6551 534c 2072 6376 6407 0000  ....eQSL rcvd...
-00003810: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00003820: 1400 6500 5100 5300 4c00 2000 7600 6500  ..e.Q.S.L. .v.e.
-00003830: 7200 7300 2e08 0000 0000 0600 0000 0965  r.s............e
-00003840: 5153 4c20 7365 6e74 0700 0000 0944 7261  QSL sent.....Dra
-00003850: 676f 6e4c 6f67 0103 0000 000e 0069 006e  gonLog.......i.n
-00003860: 0061 006b 0074 0069 0076 0800 0000 0006  .a.k.t.i.v......
-00003870: 0000 0007 696e 6163 7469 7607 0000 0009  ....inactiv.....
-00003880: 4472 6167 6f6e 4c6f 6701 0300 0000 0800  DragonLog.......
-00003890: dc00 6200 6500 7208 0000 0000 0600 0000  ..b.e.r.........
-000038a0: 0541 626f 7574 0700 0000 0a4d 6169 6e57  .About.....MainW
-000038b0: 696e 646f 7701 0300 0000 0e00 dc00 6200  indow.........b.
-000038c0: 6500 7200 2000 5100 7408 0000 0000 0600  e.r. .Q.t.......
-000038d0: 0000 0841 626f 7574 2051 7407 0000 000a  ...About Qt.....
-000038e0: 4d61 696e 5769 6e64 6f77 0103 0000 001a  MainWindow......
-000038f0: 0041 006e 0077 0065 006e 0064 0075 006e  .A.n.w.e.n.d.u.n
-00003900: 0067 0073 006c 006f 0067 0800 0000 0006  .g.s.l.o.g......
-00003910: 0000 000f 4170 706c 6963 6174 696f 6e20  ....Application 
-00003920: 4c6f 6707 0000 000a 4d61 696e 5769 6e64  Log.....MainWind
-00003930: 6f77 0103 0000 0022 0045 0069 006e 0074  ow.....".E.i.n.t
-00003940: 0072 0061 0067 0020 00e4 006e 0064 0065  .r.a.g. ...n.d.e
-00003950: 0072 006e 002e 002e 002e 0800 0000 0006  .r.n............
-00003960: 0000 0013 4368 616e 6765 206c 6f67 2065  ....Change log e
-00003970: 6e74 7279 2e2e 2e07 0000 000a 4d61 696e  ntry........Main
-00003980: 5769 6e64 6f77 0103 ffff ffff 0800 0000  Window..........
-00003990: 0006 0000 0006 4374 726c 2b45 0700 0000  ......Ctrl+E....
-000039a0: 0a4d 6169 6e57 696e 646f 7701 03ff ffff  .MainWindow.....
-000039b0: ff08 0000 0000 0600 0000 0643 7472 6c2b  ...........Ctrl+
-000039c0: 4c07 0000 000a 4d61 696e 5769 6e64 6f77  L.....MainWindow
-000039d0: 0103 ffff ffff 0800 0000 0006 0000 0006  ................
-000039e0: 4374 726c 2b51 0700 0000 0a4d 6169 6e57  Ctrl+Q.....MainW
-000039f0: 696e 646f 7701 03ff ffff ff08 0000 0000  indow...........
-00003a00: 0600 0000 0643 7472 6c2b 5707 0000 000a  .....Ctrl+W.....
-00003a10: 4d61 696e 5769 6e64 6f77 0103 ffff ffff  MainWindow......
-00003a20: 0800 0000 0006 0000 0006 4374 726c 2b58  ..........Ctrl+X
-00003a30: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
-00003a40: 0300 0000 1e00 4500 6900 6e00 7400 7200  ......E.i.n.t.r.
-00003a50: 6100 6700 2000 6c00 f600 7300 6300 6800  a.g. .l...s.c.h.
-00003a60: 6500 6e08 0000 0000 0600 0000 1044 656c  e.n..........Del
-00003a70: 6574 6520 6c6f 6720 656e 7472 7907 0000  ete log entry...
-00003a80: 000a 4d61 696e 5769 6e64 6f77 0103 ffff  ..MainWindow....
-00003a90: ffff 0800 0000 0006 0000 0009 4472 6167  ............Drag
-00003aa0: 6f6e 4c6f 6707 0000 000a 4d61 696e 5769  onLog.....MainWi
-00003ab0: 6e64 6f77 0103 0000 0014 0042 0065 0061  ndow.......B.e.a
-00003ac0: 0072 0062 0065 0069 0074 0065 006e 0800  .r.b.e.i.t.e.n..
-00003ad0: 0000 0006 0000 0004 4564 6974 0700 0000  ........Edit....
-00003ae0: 0a4d 6169 6e57 696e 646f 7701 0300 0000  .MainWindow.....
-00003af0: 0e00 4200 6500 6500 6e00 6400 6500 6e08  ..B.e.e.n.d.e.n.
-00003b00: 0000 0000 0600 0000 0445 7869 7407 0000  .........Exit...
-00003b10: 000a 4d61 696e 5769 6e64 6f77 0103 ffff  ..MainWindow....
-00003b20: ffff 0800 0000 0006 0000 0006 4578 706f  ............Expo
-00003b30: 7274 0700 0000 0a4d 6169 6e57 696e 646f  rt.....MainWindo
-00003b40: 7701 0300 0000 1c00 4500 7800 7000 6f00  w.......E.x.p.o.
-00003b50: 7200 7400 6900 6500 7200 6500 6e00 2e00  r.t.i.e.r.e.n...
-00003b60: 2e00 2e08 0000 0000 0600 0000 0945 7870  .............Exp
-00003b70: 6f72 742e 2e2e 0700 0000 0a4d 6169 6e57  ort........MainW
-00003b80: 696e 646f 7701 0300 0000 0a00 4400 6100  indow.......D.a.
-00003b90: 7400 6500 6908 0000 0000 0600 0000 0446  t.e.i..........F
-00003ba0: 696c 6507 0000 000a 4d61 696e 5769 6e64  ile.....MainWind
-00003bb0: 6f77 0103 0000 000a 0048 0069 006c 0066  ow.......H.i.l.f
-00003bc0: 0065 0800 0000 0006 0000 0004 4865 6c70  .e..........Help
-00003bd0: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
-00003be0: 03ff ffff ff08 0000 0000 0600 0000 0649  ...............I
-00003bf0: 6d70 6f72 7407 0000 000a 4d61 696e 5769  mport.....MainWi
-00003c00: 6e64 6f77 0103 0000 001c 0049 006d 0070  ndow.......I.m.p
-00003c10: 006f 0072 0074 0069 0065 0072 0065 006e  .o.r.t.i.e.r.e.n
-00003c20: 002e 002e 002e 0800 0000 0006 0000 0009  ................
-00003c30: 496d 706f 7274 2e2e 2e07 0000 000a 4d61  Import........Ma
-00003c40: 696e 5769 6e64 6f77 0103 0000 0018 004c  inWindow.......L
-00003c50: 006f 0067 0067 0065 0020 0051 0053 004f  .o.g.g.e. .Q.S.O
-00003c60: 002e 002e 002e 0800 0000 0006 0000 000a  ................
-00003c70: 4c6f 6720 5153 4f2e 2e2e 0700 0000 0a4d  Log QSO........M
-00003c80: 6169 6e57 696e 646f 7701 0300 0000 1800  ainWindow.......
-00003c90: 5100 5300 4f00 2d00 4600 6f00 7200 6d00  Q.S.O.-.F.o.r.m.
-00003ca0: 7500 6c00 6100 7208 0000 0000 0600 0000  u.l.a.r.........
-00003cb0: 0851 534f 2046 6f72 6d07 0000 000a 4d61  .QSO Form.....Ma
-00003cc0: 696e 5769 6e64 6f77 0103 0000 0026 0044  inWindow.....&.D
-00003cd0: 0061 0074 0065 006e 0062 0061 006e 006b  .a.t.e.n.b.a.n.k
-00003ce0: 0020 0077 00e4 0068 006c 0065 006e 002e  . .w...h.l.e.n..
-00003cf0: 002e 002e 0800 0000 0006 0000 0012 5365  ..............Se
-00003d00: 6c65 6374 2064 6174 6162 6173 652e 2e2e  lect database...
-00003d10: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
-00003d20: 0300 0000 1a00 4500 6900 6e00 7300 7400  ......E.i.n.s.t.
-00003d30: 6500 6c00 6c00 7500 6e00 6700 6500 6e08  e.l.l.u.n.g.e.n.
-00003d40: 0000 0000 0600 0000 0853 6574 7469 6e67  .........Setting
-00003d50: 7307 0000 000a 4d61 696e 5769 6e64 6f77  s.....MainWindow
-00003d60: 0103 0000 0026 005a 0065 0069 0067 0065  .....&.Z.e.i.g.e
-00003d70: 0020 0041 006e 0077 0065 006e 0064 0075  . .A.n.w.e.n.d.u
-00003d80: 006e 0067 0073 006c 006f 0067 0800 0000  .n.g.s.l.o.g....
-00003d90: 0006 0000 0008 5368 6f77 206c 6f67 0700  ......Show log..
-00003da0: 0000 0a4d 6169 6e57 696e 646f 7701 0300  ...MainWindow...
-00003db0: 0000 1a00 5300 7400 6100 7200 7400 6500  ....S.t.a.r.t.e.
-00003dc0: 2000 4800 6100 6d00 6c00 6900 6208 0000   .H.a.m.l.i.b...
-00003dd0: 0000 0600 0000 0c53 7461 7274 2068 616d  .......Start ham
-00003de0: 6c69 6207 0000 000a 4d61 696e 5769 6e64  lib.....MainWind
-00003df0: 6f77 0103 0000 001c 0057 0065 0072 006b  ow.......W.e.r.k
-00003e00: 007a 0065 0075 0067 006c 0065 0069 0073  .z.e.u.g.l.e.i.s
-00003e10: 0074 0065 0800 0000 0006 0000 0007 546f  .t.e..........To
-00003e20: 6f6c 6261 7207 0000 000a 4d61 696e 5769  olbar.....MainWi
-00003e30: 6e64 6f77 0103 0000 0032 004c 006f 0067  ndow.....2.L.o.g
-00003e40: 0073 0020 007a 0075 0020 004c 006f 0054  .s. .z.u. .L.o.T
-00003e50: 0057 0020 0068 006f 0063 0068 006c 0061  .W. .h.o.c.h.l.a
-00003e60: 0064 0065 006e 002e 002e 002e 0800 0000  .d.e.n..........
-00003e70: 0006 0000 0016 5570 6c6f 6164 206c 6f67  ......Upload log
-00003e80: 7320 746f 204c 6f54 572e 2e2e 0700 0000  s to LoTW.......
-00003e90: 0a4d 6169 6e57 696e 646f 7701 0300 0000  .MainWindow.....
-00003ea0: 4200 4400 6100 7400 6500 6900 2000 6100  B.D.a.t.e.i. .a.
-00003eb0: 7500 6600 2000 6e00 6500 7500 6500 2000  u.f. .n.e.u.e. .
-00003ec0: 5100 5300 4f00 7300 2000 fc00 6200 6500  Q.S.O.s. ...b.e.
-00003ed0: 7200 7700 6100 6300 6800 6500 6e00 2e00  r.w.a.c.h.e.n...
-00003ee0: 2e00 2e08 0000 0000 0600 0000 1657 6174  .............Wat
-00003ef0: 6368 2066 696c 6520 666f 7220 5153 4f73  ch file for QSOs
-00003f00: 2e2e 2e07 0000 000a 4d61 696e 5769 6e64  ........MainWind
-00003f10: 6f77 0103 ffff ffff 0800 0000 0006 0000  ow..............
-00003f20: 0002 2057 0700 0000 0751 534f 466f 726d  .. W.....QSOForm
-00003f30: 0103 ffff ffff 0800 0000 0006 0000 0004  ................
-00003f40: 206b 487a 0700 0000 0751 534f 466f 726d   kHz.....QSOForm
-00003f50: 0103 ffff ffff 0800 0000 0006 0000 0002  ................
-00003f60: 3539 0700 0000 0751 534f 466f 726d 0103  59.....QSOForm..
-00003f70: 0000 0048 0045 0069 006e 0020 0046 0065  ...H.E.i.n. .F.e
-00003f80: 006c 0064 0020 0066 0065 0068 006c 0074  .l.d. .f.e.h.l.t
-00003f90: 0020 0066 00fc 0072 0020 0064 0069 0065  . .f...r. .d.i.e
-00003fa0: 0020 0049 006e 0062 006f 0078 002d 0050  . .I.n.b.o.x.-.P
-00003fb0: 0072 00fc 0066 0075 006e 0067 0800 0000  .r...f.u.n.g....
-00003fc0: 0006 0000 0022 4120 6669 656c 6420 6973  ....."A field is
-00003fd0: 206d 6973 7369 6e67 2066 6f72 2069 6e62   missing for inb
-00003fe0: 6f78 2063 6865 636b 0700 0000 0751 534f  ox check.....QSO
-00003ff0: 466f 726d 0103 0000 0042 0046 0065 0068  Form.....B.F.e.h
-00004000: 006c 0065 006e 0064 0065 0073 0020 0046  .l.e.n.d.e.s. .F
-00004010: 0065 006c 0064 0020 0066 00fc 0072 0020  .e.l.d. .f...r. 
-00004020: 0064 0065 006e 0020 004c 006f 0067 002d  .d.e.n. .L.o.g.-
-00004030: 0055 0070 006c 006f 0061 0064 0800 0000  .U.p.l.o.a.d....
-00004040: 0006 0000 0021 4120 6669 656c 6420 6973  .....!A field is
-00004050: 206d 6973 7369 6e67 2066 6f72 206c 6f67   missing for log
-00004060: 2075 706c 6f61 6407 0000 0007 5153 4f46   upload.....QSOF
-00004070: 6f72 6d01 0300 0000 1600 4100 6b00 7a00  orm.......A.k.z.
-00004080: 6500 7000 7400 6900 6500 7200 7400 3a08  e.p.t.i.e.r.t.:.
-00004090: 0000 0000 0600 0000 0841 6363 6570 7473  .........Accepts
-000040a0: 3a07 0000 0007 5153 4f46 6f72 6d01 0300  :.....QSOForm...
-000040b0: 0000 0e00 4100 6e00 7400 6500 6e00 6e00  ....A.n.t.e.n.n.
-000040c0: 6508 0000 0000 0600 0000 0741 6e74 656e  e..........Anten
-000040d0: 6e61 0700 0000 0751 534f 466f 726d 0103  na.....QSOForm..
-000040e0: 0000 0016 0041 0075 0074 006f 006d 0061  .....A.u.t.o.m.a
-000040f0: 0074 0069 0073 0063 0068 0800 0000 0006  .t.i.s.c.h......
-00004100: 0000 000d 4175 746f 6d61 7469 6361 6c6c  ....Automaticall
-00004110: 7907 0000 0007 5153 4f46 6f72 6d01 0300  y.....QSOForm...
-00004120: 0000 3800 4600 6500 6800 6c00 6500 7200  ..8.F.e.h.l.e.r.
-00004130: 6800 6100 6600 7400 6500 7300 2000 4100  h.a.f.t.e.s. .A.
-00004140: 6200 6600 7200 6100 6700 6500 6500 7200  b.f.r.a.g.e.e.r.
-00004150: 6700 6500 6200 6e00 6900 7308 0000 0000  g.e.b.n.i.s.....
-00004160: 0600 0000 1242 6164 2072 6571 7565 7374  .....Bad request
-00004170: 2072 6573 756c 7407 0000 0007 5153 4f46   result.....QSOF
-00004180: 6f72 6d01 03ff ffff ff08 0000 0000 0600  orm.............
-00004190: 0000 0442 616e 6407 0000 0007 5153 4f46  ...Band.....QSOF
-000041a0: 6f72 6d01 0300 0000 0800 4200 fc00 7200  orm.......B...r.
-000041b0: 6f08 0000 0000 0600 0000 0642 7572 6561  o..........Burea
-000041c0: 7507 0000 0007 5153 4f46 6f72 6d01 0300  u.....QSOForm...
-000041d0: 0000 1600 4200 fc00 7200 6f00 2f00 4400  ....B...r.o./.D.
-000041e0: 6900 7200 6500 6b00 7408 0000 0000 0600  i.r.e.k.t.......
-000041f0: 0000 0d42 7572 6561 752f 4469 7265 6374  ...Bureau/Direct
-00004200: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00004210: 0014 0052 0075 0066 007a 0065 0069 0063  ...R.u.f.z.e.i.c
-00004220: 0068 0065 006e 0800 0000 0006 0000 0009  .h.e.n..........
-00004230: 4361 6c6c 2073 6967 6e07 0000 0007 5153  Call sign.....QS
-00004240: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
-00004250: 0600 0000 0843 616c 6c62 6f6f 6b07 0000  .....Callbook...
-00004260: 0007 5153 4f46 6f72 6d01 0300 0000 3c00  ..QSOForm.....<.
-00004270: 4600 6500 6800 6c00 6500 7200 2000 6200  F.e.h.l.e.r. .b.
-00004280: 6500 6900 2000 6400 6500 7200 2000 5200  e.i. .d.e.r. .R.
-00004290: 7500 6600 7a00 6500 6900 6300 6800 6500  u.f.z.e.i.c.h.e.
-000042a0: 6e00 7300 7500 6300 6800 6508 0000 0000  n.s.u.c.h.e.....
-000042b0: 0600 0000 1543 616c 6c62 6f6f 6b20 7365  .....Callbook se
-000042c0: 6172 6368 2065 7272 6f72 0700 0000 0751  arch error.....Q
-000042d0: 534f 466f 726d 0103 0000 002a 0043 0061  SOForm.....*.C.a
-000042e0: 006c 006c 0062 006f 006f 006b 002d 0053  .l.l.b.o.o.k.-.S
-000042f0: 0075 0063 0068 0065 0072 0067 0065 0062  .u.c.h.e.r.g.e.b
-00004300: 006e 0069 0073 0800 0000 0006 0000 0016  .n.i.s..........
-00004310: 4361 6c6c 626f 6f6b 2073 6561 7263 6820  Callbook search 
-00004320: 7265 7375 6c74 0700 0000 0751 534f 466f  result.....QSOFo
-00004330: 726d 0103 0000 0032 0052 0075 0066 007a  rm.....2.R.u.f.z
-00004340: 0065 0069 0063 0068 0065 006e 0020 006e  .e.i.c.h.e.n. .n
-00004350: 0069 0063 0068 0074 0020 0067 0065 0066  .i.c.h.t. .g.e.f
-00004360: 0075 006e 0064 0065 006e 0800 0000 0006  .u.n.d.e.n......
-00004370: 0000 0012 4361 6c6c 7369 676e 206e 6f74  ....Callsign not
-00004380: 2066 6f75 6e64 0700 0000 0751 534f 466f   found.....QSOFo
-00004390: 726d 0103 0000 000a 004b 0061 006e 0061  rm.......K.a.n.a
-000043a0: 006c 0800 0000 0006 0000 0007 4368 616e  .l..........Chan
-000043b0: 6e65 6c07 0000 0007 5153 4f46 6f72 6d01  nel.....QSOForm.
-000043c0: 0300 0000 1600 5000 7200 fc00 6600 6500  ......P.r...f.e.
-000043d0: 2000 4900 6e00 6200 6f00 7808 0000 0000   .I.n.b.o.x.....
-000043e0: 0600 0000 0b43 6865 636b 2049 6e62 6f78  .....Check Inbox
-000043f0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00004400: 0042 0046 0065 0068 006c 0065 0072 0020  .B.F.e.h.l.e.r. 
-00004410: 0062 0065 0069 006d 0020 0050 0072 00fc  .b.e.i.m. .P.r..
-00004420: 0066 0065 006e 0020 0064 0065 0072 0020  .f.e.n. .d.e.r. 
-00004430: 004c 006f 0054 0057 002d 0049 006e 0062  .L.o.T.W.-.I.n.b
-00004440: 006f 0078 0800 0000 0006 0000 0016 4368  .o.x..........Ch
-00004450: 6563 6b20 4c6f 5457 2049 6e62 6f78 2065  eck LoTW Inbox e
-00004460: 7272 6f72 0700 0000 0751 534f 466f 726d  rror.....QSOForm
-00004470: 0103 0000 001c 0050 0072 00fc 0066 0065  .......P.r...f.e
-00004480: 0020 004c 006f 0054 0057 0020 0051 0053  . .L.o.T.W. .Q.S
-00004490: 004c 0800 0000 0006 0000 000e 4368 6563  .L..........Chec
-000044a0: 6b20 4c6f 5457 2051 534c 0700 0000 0751  k LoTW QSL.....Q
-000044b0: 534f 466f 726d 0103 0000 0038 0065 0051  SOForm.....8.e.Q
-000044c0: 0053 004c 002d 0046 0065 0068 006c 0065  .S.L.-.F.e.h.l.e
-000044d0: 0072 0020 0070 0072 00fc 0066 0065 006e  .r. .p.r...f.e.n
-000044e0: 0020 0064 0065 0072 0020 0049 006e 0062  . .d.e.r. .I.n.b
-000044f0: 006f 0078 0800 0000 0006 0000 0016 4368  .o.x..........Ch
-00004500: 6563 6b20 6551 534c 2049 6e62 6f78 2065  eck eQSL Inbox e
-00004510: 7272 6f72 0700 0000 0751 534f 466f 726d  rror.....QSOForm
-00004520: 0103 0000 0018 005a 0075 0072 00fc 0063  .......Z.u.r...c
-00004530: 006b 0073 0065 0074 007a 0065 006e 0800  .k.s.e.t.z.e.n..
-00004540: 0000 0006 0000 0005 436c 6561 7207 0000  ........Clear...
-00004550: 0007 5153 4f46 6f72 6d01 0300 0000 2000  ..QSOForm..... .
-00004560: 4b00 6f00 6e00 6600 6900 6700 7500 7200  K.o.n.f.i.g.u.r.
-00004570: 6900 6500 7200 7400 6500 2000 4900 4408  i.e.r.t.e. .I.D.
-00004580: 0000 0000 0600 0000 1343 6f6e 6669 6775  .........Configu
-00004590: 7265 6420 6964 656e 7469 7479 0700 0000  red identity....
-000045a0: 0751 534f 466f 726d 0103 0000 002a 004b  .QSOForm.....*.K
-000045b0: 006f 006e 0066 0069 0067 0075 0072 0069  .o.n.f.i.g.u.r.i
-000045c0: 0065 0072 0074 0065 0020 0053 0074 0061  .e.r.t.e. .S.t.a
-000045d0: 0074 0069 006f 006e 0800 0000 0006 0000  .t.i.o.n........
-000045e0: 0012 436f 6e66 6967 7572 6564 2073 7461  ..Configured sta
-000045f0: 7469 6f6e 0700 0000 0751 534f 466f 726d  tion.....QSOForm
-00004600: 0103 0000 000c 0064 0069 0072 0065 006b  .......d.i.r.e.k
-00004610: 0074 0800 0000 0006 0000 0006 4469 7265  .t..........Dire
-00004620: 6374 0700 0000 0751 534f 466f 726d 0103  ct.....QSOForm..
-00004630: 0000 001c 0065 0051 0053 004c 0020 0073  .....e.Q.S.L. .s
-00004640: 0070 0065 0069 0063 0068 0065 0072 006e  .p.e.i.c.h.e.r.n
-00004650: 0800 0000 0006 0000 000d 446f 776e 6c6f  ..........Downlo
-00004660: 6164 2065 5153 4c07 0000 0007 5153 4f46  ad eQSL.....QSOF
-00004670: 6f72 6d01 0300 0000 6c00 5700 e400 6800  orm.....l.W...h.
-00004680: 7200 6500 6e00 6400 2000 6400 6500 7200  r.e.n.d. .d.e.r.
-00004690: 2000 5200 7500 6600 7a00 6500 6900 6300   .R.u.f.z.e.i.c.
-000046a0: 6800 6500 6e00 7300 7500 6300 6800 6500  h.e.n.s.u.c.h.e.
-000046b0: 2000 6900 7300 7400 2000 6500 6900 6e00   .i.s.t. .e.i.n.
-000046c0: 2000 4600 6500 6800 6c00 6500 7200 2000   .F.e.h.l.e.r. .
-000046d0: 6100 7500 6600 6700 6500 7400 7200 6500  a.u.f.g.e.t.r.e.
-000046e0: 7400 6500 6e08 0000 0000 0600 0000 2744  t.e.n.........'D
-000046f0: 7572 696e 6720 6361 6c6c 626f 6f6b 2073  uring callbook s
-00004700: 6561 7263 6820 616e 2065 7272 6f72 206f  earch an error o
-00004710: 6363 7572 6564 0700 0000 0751 534f 466f  ccured.....QSOFo
-00004720: 726d 0103 0000 0008 0045 006e 0064 0065  rm.......E.n.d.e
-00004730: 0800 0000 0006 0000 0003 456e 6407 0000  ..........End...
-00004740: 0007 5153 4f46 6f72 6d01 0300 0000 0c00  ..QSOForm.......
-00004750: 4600 6500 6800 6c00 6500 7208 0000 0000  F.e.h.l.e.r.....
-00004760: 0600 0000 0545 7272 6f72 0700 0000 0751  .....Error.....Q
-00004770: 534f 466f 726d 0103 0000 0024 0065 0051  SOForm.....$.e.Q
-00004780: 0053 004c 002d 0055 0070 006c 006f 0061  .S.L.-.U.p.l.o.a
-00004790: 0064 002d 0046 0065 0068 006c 0065 0072  .d.-.F.e.h.l.e.r
-000047a0: 0800 0000 0006 0000 000f 4572 726f 7220  ..........Error 
-000047b0: 6f6e 2075 706c 6f61 6407 0000 0007 5153  on upload.....QS
-000047c0: 4f46 6f72 6d01 0300 0000 1000 4600 7200  OForm.......F.r.
-000047d0: 6500 7100 7500 6500 6e00 7a08 0000 0000  e.q.u.e.n.z.....
-000047e0: 0600 0000 0946 7265 7175 656e 6379 0700  .....Frequency..
-000047f0: 0000 0751 534f 466f 726d 0103 ffff ffff  ...QSOForm......
-00004800: 0800 0000 0006 0000 0008 4848 3a6d 6d3a  ..........HH:mm:
-00004810: 7373 0700 0000 0751 534f 466f 726d 0103  ss.....QSOForm..
-00004820: ffff ffff 0800 0000 0006 0000 0006 4861  ..............Ha
-00004830: 6d51 5448 0700 0000 0751 534f 466f 726d  mQTH.....QSOForm
-00004840: 0103 0000 0004 0049 0044 0800 0000 0006  .......I.D......
-00004850: 0000 0008 4964 656e 7469 7479 0700 0000  ....Identity....
-00004860: 0751 534f 466f 726d 0103 0000 0026 004c  .QSOForm.....&.L
-00004870: 0069 006e 006b 0020 007a 0075 0072 0020  .i.n.k. .z.u.r. 
-00004880: 0065 0051 0053 004c 002d 004b 0061 0072  .e.Q.S.L.-.K.a.r
-00004890: 0074 0065 0800 0000 0006 0000 0011 4c69  .t.e..........Li
-000048a0: 6e6b 2074 6f20 6551 534c 2043 6172 6407  nk to eQSL Card.
-000048b0: 0000 0007 5153 4f46 6f72 6d01 03ff ffff  ....QSOForm.....
-000048c0: ff08 0000 0000 0600 0000 044c 6f54 5707  ...........LoTW.
-000048d0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-000048e0: 1c00 4c00 6f00 5400 5700 2000 6500 6d00  ..L.o.T.W. .e.m.
-000048f0: 7000 6600 6100 6e00 6700 6500 6e08 0000  p.f.a.n.g.e.n...
-00004900: 0000 0600 0000 0d4c 6f54 5720 7265 6365  .......LoTW rece
-00004910: 6976 6564 0700 0000 0751 534f 466f 726d  ived.....QSOForm
-00004920: 0103 0000 001c 004c 006f 0054 0057 0020  .......L.o.T.W. 
-00004930: 0076 0065 0072 0073 0065 006e 0064 0065  .v.e.r.s.e.n.d.e
-00004940: 0074 0800 0000 0006 0000 0009 4c6f 5457  .t..........LoTW
-00004950: 2073 656e 7407 0000 0007 5153 4f46 6f72   sent.....QSOFor
-00004960: 6d01 03ff ffff ff08 0000 0000 0600 0000  m...............
-00004970: 074c 6f63 6174 6f72 0700 0000 0751 534f  .Locator.....QSO
-00004980: 466f 726d 0103 0000 0042 004c 006f 0067  Form.....B.L.o.g
-00004990: 0069 006e 0020 0066 0065 0068 006c 0067  .i.n. .f.e.h.l.g
-000049a0: 0065 0073 0063 0068 006c 0061 0067 0065  .e.s.c.h.l.a.g.e
-000049b0: 006e 0020 0066 00fc 0072 0020 0042 0065  .n. .f...r. .B.e
-000049c0: 006e 0075 0074 007a 0065 0072 0800 0000  .n.u.t.z.e.r....
-000049d0: 0006 0000 0015 4c6f 6769 6e20 6661 696c  ......Login fail
-000049e0: 6564 2066 6f72 2075 7365 7207 0000 0007  ed for user.....
-000049f0: 5153 4f46 6f72 6d01 0300 0000 1400 4800  QSOForm.......H.
-00004a00: 6100 7500 7000 7400 6400 6100 7400 6500  a.u.p.t.d.a.t.e.
-00004a10: 6e08 0000 0000 0600 0000 094d 6169 6e20  n..........Main 
-00004a20: 6461 7461 0700 0000 0751 534f 466f 726d  data.....QSOForm
-00004a30: 0103 ffff ffff 0800 0000 0006 0000 0004  ................
-00004a40: 4d6f 6465 0700 0000 0751 534f 466f 726d  Mode.....QSOForm
-00004a50: 0103 0000 0012 0076 0065 0072 00e4 006e  .......v.e.r...n
-00004a60: 0064 0065 0072 0074 0800 0000 0006 0000  .d.e.r.t........
-00004a70: 0008 4d6f 6469 6669 6564 0700 0000 0751  ..Modified.....Q
-00004a80: 534f 466f 726d 0103 ffff ffff 0800 0000  SOForm..........
-00004a90: 0006 0000 0004 4e61 6d65 0700 0000 0751  ......Name.....Q
-00004aa0: 534f 466f 726d 0103 0000 0024 004b 0065  SOForm.....$.K.e
-00004ab0: 0069 006e 0020 0051 0053 004c 0020 0076  .i.n. .Q.S.L. .v
-00004ac0: 0065 0072 0066 00fc 0067 0062 0061 0072  .e.r.f...g.b.a.r
-00004ad0: 0800 0000 0006 0000 0010 4e6f 2051 534c  ..........No QSL
-00004ae0: 2061 7661 696c 6162 6c65 0700 0000 0751   available.....Q
-00004af0: 534f 466f 726d 0103 0000 0026 004b 0065  SOForm.....&.K.e
-00004b00: 0069 006e 0020 0065 0051 0053 004c 0020  .i.n. .e.Q.S.L. 
-00004b10: 0076 0065 0072 0066 00fc 0067 0062 0061  .v.e.r.f...g.b.a
-00004b20: 0072 0800 0000 0006 0000 0011 4e6f 2065  .r..........No e
-00004b30: 5153 4c20 6176 6169 6c61 626c 6507 0000  QSL available...
-00004b40: 0007 5153 4f46 6f72 6d01 0300 0000 0a00  ..QSOForm.......
-00004b50: 4a00 6500 7400 7a00 7408 0000 0000 0600  J.e.t.z.t.......
-00004b60: 0000 034e 6f77 0700 0000 0751 534f 466f  ...Now.....QSOFo
-00004b70: 726d 0103 0000 0016 0045 0069 0067 0065  rm.......E.i.g.e
-00004b80: 006e 0065 0072 0020 0051 0054 0048 0800  .n.e.r. .Q.T.H..
-00004b90: 0000 0006 0000 0007 4f77 6e20 5154 4807  ........Own QTH.
-00004ba0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-00004bb0: 2400 4500 6900 6700 6500 6e00 6500 7300  $.E.i.g.e.n.e.s.
-00004bc0: 2000 5200 7500 6600 7a00 6500 6900 6300   .R.u.f.z.e.i.c.
-00004bd0: 6800 6500 6e08 0000 0000 0600 0000 0d4f  h.e.n..........O
-00004be0: 776e 2063 616c 6c20 7369 676e 0700 0000  wn call sign....
-00004bf0: 0751 534f 466f 726d 0103 0000 001e 0045  .QSOForm.......E
-00004c00: 0069 0067 0065 006e 0065 0072 0020 004c  .i.g.e.n.e.r. .L
-00004c10: 006f 0063 0061 0074 006f 0072 0800 0000  .o.c.a.t.o.r....
-00004c20: 0006 0000 000b 4f77 6e20 6c6f 6361 746f  ......Own locato
-00004c30: 7207 0000 0007 5153 4f46 6f72 6d01 0300  r.....QSOForm...
-00004c40: 0000 1800 4500 6900 6700 6500 6e00 6500  ....E.i.g.e.n.e.
-00004c50: 7200 2000 4e00 6100 6d00 6508 0000 0000  r. .N.a.m.e.....
-00004c60: 0600 0000 084f 776e 206e 616d 6507 0000  .....Own name...
-00004c70: 0007 5153 4f46 6f72 6d01 0300 0000 1c00  ..QSOForm.......
-00004c80: 4500 6900 6700 6500 6e00 6500 2000 4e00  E.i.g.e.n.e. .N.
-00004c90: 6f00 7400 6900 7a00 6500 6e08 0000 0000  o.t.i.z.e.n.....
-00004ca0: 0600 0000 094f 776e 206e 6f74 6573 0700  .....Own notes..
-00004cb0: 0000 0751 534f 466f 726d 0103 0000 0010  ...QSOForm......
-00004cc0: 004c 0065 0069 0073 0074 0075 006e 0067  .L.e.i.s.t.u.n.g
-00004cd0: 0800 0000 0006 0000 0005 506f 7765 7207  ..........Power.
-00004ce0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-00004cf0: 1e00 4100 7500 7300 6200 7200 6500 6900  ..A.u.s.b.r.e.i.
-00004d00: 7400 7500 6e00 6700 7300 6100 7200 7408  t.u.n.g.s.a.r.t.
-00004d10: 0000 0000 0600 0000 0b50 726f 7061 6761  .........Propaga
-00004d20: 7469 6f6e 0700 0000 0751 534f 466f 726d  tion.....QSOForm
-00004d30: 0103 ffff ffff 0800 0000 0006 0000 0003  ................
-00004d40: 5153 4c07 0000 0007 5153 4f46 6f72 6d01  QSL.....QSOForm.
-00004d50: 0300 0000 2200 5100 5300 4c00 2000 2600  ....".Q.S.L. .&.
-00004d60: 2600 2000 4c00 6f00 6700 2d00 5500 7000  &. .L.o.g.-.U.p.
-00004d70: 6c00 6f00 6100 6408 0000 0000 0600 0000  l.o.a.d.........
-00004d80: 1151 534c 2026 2620 4c6f 6720 7570 6c6f  .QSL && Log uplo
-00004d90: 6164 0700 0000 0751 534f 466f 726d 0103  ad.....QSOForm..
-00004da0: 0000 001c 0051 0053 004c 002d 004b 0061  .....Q.S.L.-.K.a
-00004db0: 0072 0074 0065 006e 0074 0065 0078 0074  .r.t.e.n.t.e.x.t
-00004dc0: 0800 0000 0006 0000 0010 5153 4c20 6361  ..........QSL ca
-00004dd0: 7264 206d 6573 7361 6765 0700 0000 0751  rd message.....Q
-00004de0: 534f 466f 726d 0103 0000 001a 0051 0053  SOForm.......Q.S
-00004df0: 004c 0020 0065 006d 0070 0066 0061 006e  .L. .e.m.p.f.a.n
-00004e00: 0067 0065 006e 0800 0000 0006 0000 000c  .g.e.n..........
-00004e10: 5153 4c20 7265 6365 6976 6564 0700 0000  QSL received....
-00004e20: 0751 534f 466f 726d 0103 0000 0018 0051  .QSOForm.......Q
-00004e30: 0053 004c 0020 0067 0065 0073 0065 006e  .S.L. .g.e.s.e.n
-00004e40: 0064 0065 0074 0800 0000 0006 0000 0008  .d.e.t..........
-00004e50: 5153 4c20 7365 6e74 0700 0000 0751 534f  QSL sent.....QSO
-00004e60: 466f 726d 0103 0000 000e 0051 0053 004c  Form.......Q.S.L
-00004e70: 002d 0056 0069 0061 0800 0000 0006 0000  .-.V.i.a........
-00004e80: 0007 5153 4c20 7669 6107 0000 0007 5153  ..QSL via.....QS
-00004e90: 4f46 6f72 6d01 0300 0000 1800 5100 5300  OForm.......Q.S.
-00004ea0: 4f00 2d00 4600 6f00 7200 6d00 7500 6c00  O.-.F.o.r.m.u.l.
-00004eb0: 6100 7208 0000 0000 0600 0000 0851 534f  a.r..........QSO
-00004ec0: 2046 6f72 6d07 0000 0007 5153 4f46 6f72   Form.....QSOFor
-00004ed0: 6d01 0300 0000 1c00 5100 5300 4f00 2d00  m.......Q.S.O.-.
-00004ee0: 4b00 6f00 6d00 6d00 6500 6e00 7400 6100  K.o.m.m.e.n.t.a.
-00004ef0: 7200 6508 0000 0000 0600 0000 0c51 534f  r.e..........QSO
-00004f00: 2063 6f6d 6d65 6e74 7307 0000 0007 5153   comments.....QS
-00004f10: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
-00004f20: 0600 0000 0351 5448 0700 0000 0751 534f  .....QTH.....QSO
-00004f30: 466f 726d 0103 ffff ffff 0800 0000 0006  Form............
-00004f40: 0000 0006 5253 5420 5278 0700 0000 0751  ....RST Rx.....Q
-00004f50: 534f 466f 726d 0103 ffff ffff 0800 0000  SOForm..........
-00004f60: 0006 0000 0006 5253 5420 5478 0700 0000  ......RST Tx....
-00004f70: 0751 534f 466f 726d 0103 0000 001a 0052  .QSOForm.......R
-00004f80: 0053 0054 0020 0065 006d 0070 0066 0061  .S.T. .e.m.p.f.a
-00004f90: 006e 0067 0065 006e 0800 0000 0006 0000  .n.g.e.n........
-00004fa0: 000c 5253 5420 7265 6365 6976 6564 0700  ..RST received..
-00004fb0: 0000 0751 534f 466f 726d 0103 0000 0018  ...QSOForm......
-00004fc0: 0052 0053 0054 0020 0067 0065 0073 0065  .R.S.T. .g.e.s.e
-00004fd0: 006e 0064 0065 0074 0800 0000 0006 0000  .n.d.e.t........
-00004fe0: 0008 5253 5420 7365 6e74 0700 0000 0751  ..RST sent.....Q
-00004ff0: 534f 466f 726d 0103 ffff ffff 0800 0000  SOForm..........
-00005000: 0006 0000 0005 5261 6469 6f07 0000 0007  ......Radio.....
-00005010: 5153 4f46 6f72 6d01 0300 0000 1200 5300  QSOForm.......S.
-00005020: 7000 6500 6900 6300 6800 6500 7200 6e08  p.e.i.c.h.e.r.n.
-00005030: 0000 0000 0600 0000 0453 6176 6507 0000  .........Save...
-00005040: 0007 5153 4f46 6f72 6d01 0300 0000 2600  ..QSOForm.....&.
-00005050: 5300 7000 6500 6900 6300 6800 6500 7200  S.p.e.i.c.h.e.r.
-00005060: 6e00 2000 2600 2600 2000 5500 7000 6c00  n. .&.&. .U.p.l.
-00005070: 6f00 6100 6408 0000 0000 0600 0000 0e53  o.a.d..........S
-00005080: 6176 6520 2626 2055 706c 6f61 6407 0000  ave && Upload...
-00005090: 0007 5153 4f46 6f72 6d01 0300 0000 2a00  ..QSOForm.....*.
-000050a0: 6500 5100 5300 4c00 2d00 4f00 7200 6400  e.Q.S.L.-.O.r.d.
-000050b0: 6e00 6500 7200 2000 6100 7500 7300 7700  n.e.r. .a.u.s.w.
-000050c0: e400 6800 6c00 6500 6e08 0000 0000 0600  ..h.l.e.n.......
-000050d0: 0000 1253 656c 6563 7420 6551 534c 2066  ...Select eQSL f
-000050e0: 6f6c 6465 7207 0000 0007 5153 4f46 6f72  older.....QSOFor
-000050f0: 6d01 0300 0000 3600 5300 6500 7200 7600  m.....6.S.e.r.v.
-00005100: 6500 7200 6b00 6f00 6d00 6d00 7500 6e00  e.r.k.o.m.m.u.n.
-00005110: 6900 6b00 6100 7400 6900 6f00 6e00 7300  i.k.a.t.i.o.n.s.
-00005120: 2d00 4600 6500 6800 6c00 6500 7208 0000  -.F.e.h.l.e.r...
-00005130: 0000 0600 0000 1a53 6572 7665 7220 636f  .......Server co
-00005140: 6d6d 756e 6963 6174 696f 6e20 6572 726f  mmunication erro
-00005150: 7207 0000 0007 5153 4f46 6f72 6d01 03ff  r.....QSOForm...
-00005160: ffff ff08 0000 0000 0600 0000 0553 7461  .............Sta
-00005170: 7274 0700 0000 0751 534f 466f 726d 0103  rt.....QSOForm..
-00005180: ffff ffff 0800 0000 0006 0000 0007 5374  ..............St
-00005190: 6174 696f 6e07 0000 0007 5153 4f46 6f72  ation.....QSOFor
-000051a0: 6d01 03ff ffff ff08 0000 0000 0600 0000  m...............
-000051b0: 0753 7562 6d6f 6465 0700 0000 0751 534f  .Submode.....QSO
-000051c0: 466f 726d 0103 0000 0030 0044 0061 0073  Form.....0.D.a.s
-000051d0: 0020 0051 0053 004f 0020 0069 0073 0074  . .Q.S.O. .i.s.t
-000051e0: 0020 0065 0069 006e 0020 0044 0075 0070  . .e.i.n. .D.u.p
-000051f0: 006c 0069 006b 0061 0074 0800 0000 0006  .l.i.k.a.t......
-00005200: 0000 0016 5468 6520 5153 4f20 6973 2061  ....The QSO is a
-00005210: 2064 7570 6c69 6361 7465 0700 0000 0751   duplicate.....Q
-00005220: 534f 466f 726d 0103 0000 00b8 0044 0069  SOForm.......D.i
-00005230: 0065 0020 0051 0053 004c 002d 0052 006f  .e. .Q.S.L.-.R.o
-00005240: 0075 0074 0065 0020 0064 0065 0072 0020  .u.t.e. .d.e.r. 
-00005250: 006b 006f 006e 0074 0061 006b 0074 0069  .k.o.n.t.a.k.t.i
-00005260: 0065 0072 0074 0065 006e 0020 0053 0074  .e.r.t.e.n. .S.t
-00005270: 0061 0074 0069 006f 006e 002e 000a 0044  .a.t.i.o.n.....D
-00005280: 0069 0065 0073 0020 0069 0073 0074 0020  .i.e.s. .i.s.t. 
-00005290: 006e 0069 0063 0068 0074 0020 0064 0069  .n.i.c.h.t. .d.i
-000052a0: 0065 0020 0041 0064 0072 0065 0073 0073  .e. .A.d.r.e.s.s
-000052b0: 0065 0020 0064 0065 0073 0020 0051 0053  .e. .d.e.s. .Q.S
-000052c0: 004c 002d 004d 0061 006e 0061 0067 0065  .L.-.M.a.n.a.g.e
-000052d0: 0072 0073 002f 002d 0042 00fc 0072 006f  .r.s./.-.B...r.o
-000052e0: 0073 002e 0800 0000 0006 0000 004c 5468  .s...........LTh
-000052f0: 6520 636f 6e74 6163 7465 6420 7374 6174  e contacted stat
-00005300: 696f 6e20 5153 4c20 726f 7574 652e 0a54  ion QSL route..T
-00005310: 6869 7320 6973 206e 6f74 2074 6865 2051  his is not the Q
-00005320: 534c 206d 616e 6167 6572 2f62 7572 6561  SL manager/burea
-00005330: 7520 6164 6472 6573 732e 0700 0000 0751  u address......Q
-00005340: 534f 466f 726d 0103 0000 0024 0065 0051  SOForm.....$.e.Q
-00005350: 0053 004c 002d 0055 0070 006c 006f 0061  .S.L.-.U.p.l.o.a
-00005360: 0064 002d 0046 0065 0068 006c 0065 0072  .d.-.F.e.h.l.e.r
-00005370: 0800 0000 0006 0000 0011 5570 6c6f 6164  ..........Upload
-00005380: 2065 5153 4c20 6572 726f 7207 0000 0007   eQSL error.....
-00005390: 5153 4f46 6f72 6d01 0300 0000 1a00 5500  QSOForm.......U.
-000053a0: 7000 6c00 6f00 6100 6400 2d00 4600 6500  p.l.o.a.d.-.F.e.
-000053b0: 6800 6c00 6500 7208 0000 0000 0600 0000  h.l.e.r.........
-000053c0: 1055 706c 6f61 6420 6c6f 6720 6572 726f  .Upload log erro
-000053d0: 7207 0000 0007 5153 4f46 6f72 6d01 0300  r.....QSOForm...
-000053e0: 0000 1600 6800 6f00 6300 6800 6700 6500  ....h.o.c.h.g.e.
-000053f0: 6c00 6100 6400 6500 6e08 0000 0000 0600  l.a.d.e.n.......
-00005400: 0000 0855 706c 6f61 6465 6407 0000 0007  ...Uploaded.....
-00005410: 5153 4f46 6f72 6d01 0300 0000 6800 5500  QSOForm.....h.U.
-00005420: 7000 6c00 6f00 6100 6400 2000 6500 7200  p.l.o.a.d. .e.r.
-00005430: 6600 6f00 6c00 6700 7400 2000 6e00 7500  f.o.l.g.t. .n.u.
-00005440: 7200 2000 7700 6500 6e00 6e00 2000 6100  r. .w.e.n.n. .a.
-00005450: 7500 6600 2000 6400 6500 7200 2000 5100  u.f. .d.e.r. .Q.
-00005460: 5300 4c00 2d00 5300 6500 6900 7400 6500  S.L.-.S.e.i.t.e.
-00005470: 2000 6100 7500 7300 6700 6500 7700 e400   .a.u.s.g.e.w...
-00005480: 6800 6c00 7408 0000 0000 0600 0000 2455  h.l.t.........$U
-00005490: 706c 6f61 6473 206f 6e6c 7920 6966 2073  ploads only if s
-000054a0: 656c 6563 7465 6420 6f6e 2051 534c 2070  elected on QSL p
-000054b0: 6167 6507 0000 0007 5153 4f46 6f72 6d01  age.....QSOForm.
-000054c0: 0300 0000 4800 4400 6500 7200 2000 4e00  ....H.D.e.r. .N.
-000054d0: 7500 7400 7a00 6500 7200 2000 4300 6100  u.t.z.e.r. .C.a.
-000054e0: 6c00 6c00 2000 7300 7400 6900 6d00 6d00  l.l. .s.t.i.m.m.
-000054f0: 7400 2000 6e00 6900 6300 6800 7400 2000  t. .n.i.c.h.t. .
-00005500: fc00 6200 6500 7200 6500 6900 6e08 0000  ..b.e.r.e.i.n...
-00005510: 0000 0600 0000 1855 7365 7220 6361 6c6c  .......User call
-00005520: 2064 6f65 7320 6e6f 7420 6d61 7463 6807   does not match.
-00005530: 0000 0007 5153 4f46 6f72 6d01 03ff ffff  ....QSOForm.....
-00005540: ff08 0000 0000 0600 0000 0465 5153 4c07  ...........eQSL.
-00005550: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-00005560: 1c00 6500 5100 5300 4c00 2000 6500 6d00  ..e.Q.S.L. .e.m.
-00005570: 7000 6600 6100 6e00 6700 6500 6e08 0000  p.f.a.n.g.e.n...
-00005580: 0000 0600 0000 0d65 5153 4c20 7265 6365  .......eQSL rece
-00005590: 6976 6564 0700 0000 0751 534f 466f 726d  ived.....QSOForm
-000055a0: 0103 0000 001a 0065 0051 0053 004c 0020  .......e.Q.S.L. 
-000055b0: 0067 0065 0073 0065 006e 0064 0065 0074  .g.e.s.e.n.d.e.t
-000055c0: 0800 0000 0006 0000 0009 6551 534c 2073  ..........eQSL s
-000055d0: 656e 7407 0000 0007 5153 4f46 6f72 6d01  ent.....QSOForm.
-000055e0: 0300 0000 0800 6b00 2e00 4100 2e08 0000  ......k...A.....
-000055f0: 0000 0600 0000 046e 2e61 2e07 0000 0007  .......n.a......
-00005600: 5153 4f46 6f72 6d01 0300 0000 3400 7200  QSOForm.....4.r.
-00005610: 6900 6700 6300 7400 6c00 6400 2000 5a00  i.g.c.t.l.d. .Z.
-00005620: 6500 6900 7400 fc00 6200 6500 7200 7300  e.i.t...b.e.r.s.
-00005630: 6300 6800 7200 6500 6900 7400 7500 6e00  c.h.r.e.i.t.u.n.
-00005640: 6708 0000 0000 0600 0000 0f72 6967 6374  g..........rigct
-00005650: 6c64 2074 696d 656f 7574 0700 0000 0751  ld timeout.....Q
-00005660: 534f 466f 726d 0103 ffff ffff 0800 0000  SOForm..........
-00005670: 0006 0000 000a 7979 7979 2d4d 4d2d 6464  ......yyyy-MM-dd
-00005680: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00005690: 007a 0043 0041 0054 002d 0045 0069 006e  .z.C.A.T.-.E.i.n
-000056a0: 0073 0074 0065 006c 006c 0075 006e 0067  .s.t.e.l.l.u.n.g
-000056b0: 0020 0077 0075 0072 0064 0020 006e 006f  . .w.u.r.d. .n.o
-000056c0: 0063 0068 0020 006e 0069 0065 0020 0067  .c.h. .n.i.e. .g
-000056d0: 0065 0073 0070 0065 0069 0063 0068 0065  .e.s.p.e.i.c.h.e
-000056e0: 0072 0074 0020 006f 0072 0020 0050 0061  .r.t. .o.r. .P.a
-000056f0: 0072 0061 006d 0065 0074 0065 0072 0020  .r.a.m.e.t.e.r. 
-00005700: 0066 0065 0068 006c 0065 006e 0800 0000  .f.e.h.l.e.n....
-00005710: 0006 0000 003b 4341 5420 636f 6e66 6967  .....;CAT config
-00005720: 7572 6174 696f 6e20 7761 7320 6e65 7665  uration was neve
-00005730: 7220 7361 7665 6420 6f72 2061 2070 6172  r saved or a par
-00005740: 616d 6574 6572 2069 7320 6d69 7373 696e  ameter is missin
-00005750: 6707 0000 0008 5365 7474 696e 6773 0103  g.....Settings..
-00005760: 0000 0030 0043 0041 0054 002d 0045 0069  ...0.C.A.T.-.E.i
-00005770: 006e 0073 0074 0065 006c 006c 0075 006e  .n.s.t.e.l.l.u.n
-00005780: 0067 0065 006e 0020 0046 0065 0068 006c  .g.e.n. .F.e.h.l
-00005790: 0065 0072 0800 0000 0006 0000 0012 4341  .e.r..........CA
-000057a0: 5420 7365 7474 696e 6773 2065 7272 6f72  T settings error
-000057b0: 0700 0000 0853 6574 7469 6e67 7301 0300  .....Settings...
-000057c0: 0000 2a00 4800 6100 6d00 6c00 6900 6200  ..*.H.a.m.l.i.b.
-000057d0: 2000 7200 6900 6700 6300 7400 6c00 6400   .r.i.g.c.t.l.d.
-000057e0: 2000 7700 e400 6800 6c00 6500 6e08 0000   .w...h.l.e.n...
-000057f0: 0000 0600 0000 2043 686f 6f73 6520 6861  ...... Choose ha
-00005800: 6d6c 6962 2072 6967 6374 6c64 2065 7865  mlib rigctld exe
-00005810: 6375 7461 626c 6507 0000 0008 5365 7474  cutable.....Sett
-00005820: 696e 6773 0103 0000 0020 0044 0061 0074  ings..... .D.a.t
-00005830: 0075 006d 002f 005a 0065 0069 0074 0020  .u.m./.Z.e.i.t. 
-00005840: 0053 0074 0061 0072 0074 0800 0000 0006  .S.t.a.r.t......
-00005850: 0000 000f 4461 7465 2f54 696d 6520 7374  ....Date/Time st
-00005860: 6172 7407 0000 0008 5365 7474 696e 6773  art.....Settings
-00005870: 0103 0000 0042 0046 0065 0068 006c 0065  .....B.F.e.h.l.e
-00005880: 0072 0020 0062 0065 0069 006d 0020 0041  .r. .b.e.i.m. .A
-00005890: 0075 0073 0066 00fc 0068 0072 0065 006e  .u.s.f...h.r.e.n
-000058a0: 0020 0076 006f 006e 0020 0072 0069 0067  . .v.o.n. .r.i.g
-000058b0: 0063 0074 006c 0064 0800 0000 0006 0000  .c.t.l.d........
-000058c0: 0017 4572 726f 7220 6578 6563 7574 696e  ..Error executin
-000058d0: 6720 7269 6763 746c 6407 0000 0008 5365  g rigctld.....Se
-000058e0: 7474 696e 6773 0103 ffff ffff 0800 0000  ttings..........
-000058f0: 0006 0000 0006 4861 6d6c 6962 0700 0000  ......Hamlib....
-00005900: 0853 6574 7469 6e67 7301 0300 0000 4e00  .Settings.....N.
-00005910: 4400 6900 6500 2000 6700 6500 7700 e400  D.i.e. .g.e.w...
-00005920: 6800 6c00 7400 6500 2000 4400 6100 7400  h.l.t.e. .D.a.t.
-00005930: 6500 6900 2000 6900 7300 7400 2000 6e00  e.i. .i.s.t. .n.
-00005940: 6900 6300 6800 7400 2000 6100 7500 7300  i.c.h.t. .a.u.s.
-00005950: 6600 fc00 6800 7200 6200 6100 7208 0000  f...h.r.b.a.r...
-00005960: 0000 0600 0000 2353 656c 6563 7465 6420  ......#Selected 
-00005970: 6669 6c65 2069 7320 6e6f 7420 7468 6520  file is not the 
-00005980: 6578 6563 7574 6162 6c65 0700 0000 0853  executable.....S
-00005990: 6574 7469 6e67 7301 0300 0000 1400 7a00  ettings.......z.
-000059a0: 6500 6900 6700 6500 2000 6100 6c00 6c00  e.i.g.e. .a.l.l.
-000059b0: 6508 0000 0000 0600 0000 0853 686f 7720  e..........Show 
-000059c0: 616c 6c07 0000 0008 5365 7474 696e 6773  all.....Settings
-000059d0: 0103 ffff ffff 0800 0000 0006 0000 0005  ................
-000059e0: 5374 6172 7407 0000 0008 5365 7474 696e  Start.....Settin
-000059f0: 6773 0103 0000 001a 0053 0074 0061 0072  gs.......S.t.a.r
-00005a00: 0074 0065 0020 0048 0061 006d 006c 0069  .t.e. .H.a.m.l.i
-00005a10: 0062 0800 0000 0006 0000 000c 5374 6172  .b..........Star
-00005a20: 7420 6861 6d6c 6962 0700 0000 0853 6574  t hamlib.....Set
-00005a30: 7469 6e67 7301 03ff ffff ff08 0000 0000  tings...........
-00005a40: 0600 0000 0453 746f 7007 0000 0008 5365  .....Stop.....Se
-00005a50: 7474 696e 6773 0103 0000 001a 0053 0074  ttings.......S.t
-00005a60: 006f 0070 0070 0065 0020 0048 0061 006d  .o.p.p.e. .H.a.m
-00005a70: 006c 0069 0062 0800 0000 0006 0000 000b  .l.i.b..........
-00005a80: 5374 6f70 2068 616d 6c69 6207 0000 0008  Stop hamlib.....
-00005a90: 5365 7474 696e 6773 0103 0000 000a 0061  Settings.......a
-00005aa0: 006b 0074 0069 0076 0800 0000 0006 0000  .k.t.i.v........
-00005ab0: 0005 6163 7469 7607 0000 0008 5365 7474  ..activ.....Sett
-00005ac0: 696e 6773 0103 0000 000e 0069 006e 0061  ings.......i.n.a
-00005ad0: 006b 0074 0069 0076 0800 0000 0006 0000  .k.t.i.v........
-00005ae0: 0007 696e 6163 7469 7607 0000 0008 5365  ..inactiv.....Se
-00005af0: 7474 696e 6773 0103 0000 004a 0072 0069  ttings.....J.r.i
-00005b00: 0067 0063 0074 006c 0064 0020 006b 006f  .g.c.t.l.d. .k.o
-00005b10: 006e 006e 0074 0065 0020 006e 0069 0063  .n.n.t.e. .n.i.c
-00005b20: 0068 0074 0020 0067 0065 0073 0074 0061  .h.t. .g.e.s.t.a
-00005b30: 0072 0074 0065 0074 0020 0077 0065 0072  .r.t.e.t. .w.e.r
-00005b40: 0064 0065 006e 0800 0000 0006 0000 001e  .d.e.n..........
-00005b50: 7269 6763 746c 6420 6469 6420 6e6f 7420  rigctld did not 
-00005b60: 7374 6172 7420 7072 6f70 6572 6c79 0700  start properly..
-00005b70: 0000 0853 6574 7469 6e67 7301 03ff ffff  ...Settings.....
-00005b80: ff08 0000 0000 0600 0000 074a 5338 4361  ...........JS8Ca
-00005b90: 6c6c 0700 0000 0f61 7070 5365 6c65 6374  ll.....appSelect
-00005ba0: 4469 616c 6f67 0103 ffff ffff 0800 0000  Dialog..........
-00005bb0: 0006 0000 0005 4f74 6865 7207 0000 000f  ......Other.....
-00005bc0: 6170 7053 656c 6563 7444 6961 6c6f 6701  appSelectDialog.
-00005bd0: 0300 0000 2a00 4100 7500 7300 7700 6100  ....*.A.u.s.w.a.
-00005be0: 6800 6c00 2000 6400 6500 7300 2000 5000  h.l. .d.e.s. .P.
-00005bf0: 7200 6f00 6700 7200 6100 6d00 6d00 7308  r.o.g.r.a.m.m.s.
-00005c00: 0000 0000 0600 0000 1653 656c 6563 7420  .........Select 
-00005c10: 7468 6520 6170 706c 6963 6174 696f 6e07  the application.
-00005c20: 0000 000f 6170 7053 656c 6563 7444 6961  ....appSelectDia
-00005c30: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
-00005c40: 0000 0657 534a 542d 5807 0000 000f 6170  ...WSJT-X.....ap
-00005c50: 7053 656c 6563 7444 6961 6c6f 6701 03ff  pSelectDialog...
-00005c60: ffff ff08 0000 0000 0600 0000 0666 6c64  .............fld
-00005c70: 6967 6907 0000 000f 6170 7053 656c 6563  igi.....appSelec
-00005c80: 7444 6961 6c6f 6701 8800 0000 0201 01    tDialog........
+00000030: 0000 4d00 0054 1f00 0000 4e00 0054 5900  ..M..T....N..TY.
+00000040: 0000 5200 0054 8b00 0000 5900 0054 c700  ..R..T....Y..T..
+00000050: 0002 5700 0035 7400 0003 8900 0035 b200  ..W..5t......5..
+00000060: 0005 5b00 0023 9900 000c d000 0011 7100  ..[..#........q.
+00000070: 0031 0e00 0000 0000 0047 6400 0001 fe00  .1.......Gd.....
+00000080: 004c 4400 003e aa00 0052 8400 0007 8600  .LD..>...R......
+00000090: 0053 5e00 0008 b400 0055 6700 0043 2d00  .S^......Ug..C-.
+000000a0: 0056 7c00 0045 3500 0056 7f00 0026 5600  .V|..E5..V...&V.
+000000b0: 0056 8800 000a 9200 0056 8800 0026 fe00  .V.......V...&..
+000000c0: 0056 8800 0047 8700 0058 f700 000b 0e00  .V...G...X......
+000000d0: 026f fa00 0035 9200 0345 3000 0000 3f00  .o...5...E0...?.
+000000e0: 0357 3000 0000 bf00 037b 3000 0000 fe00  .W0......{0.....
+000000f0: 03c9 3000 0001 3d00 0488 4400 0015 1900  ..0...=...D.....
+00000100: 0488 4400 0039 2f00 04bb 0400 0031 1600  ..D..9/......1..
+00000110: 04cf 0400 0031 4d00 04d0 2500 0031 e700  .....1M...%..1..
+00000120: 04e7 1000 001e 1d00 04ec 3000 001d f100  ..........0.....
+00000130: 04ec 3000 0032 1400 0534 9700 0007 da00  ..0..2...4......
+00000140: 0534 9700 0040 1f00 0545 a500 0022 bb00  .4...@...E..."..
+00000150: 0545 a500 0042 4a00 0548 3500 0008 dc00  .E...BJ..H5.....
+00000160: 0548 3500 0022 dd00 0548 3500 0042 6a00  .H5.."...H5..Bj.
+00000170: 0596 7c00 000e 5800 0598 c500 0048 8900  ..|...X......H..
+00000180: 05ab 6000 0052 d900 06a6 7c00 0011 5200  ..`..R....|...R.
+00000190: 06a6 7c00 004d df00 06fb 2100 0042 1100  ..|..M....!..B..
+000001a0: 0714 3e00 004e 8300 144b 9e00 000d c500  ..>..N...K......
+000001b0: 144e e600 0021 1300 3477 3000 0000 7f00  .N...!..4w0.....
+000001c0: 34c5 3000 0000 9f00 36b7 3000 0000 de00  4.0.....6.0.....
+000001d0: 376f f400 004b b800 38a9 3000 0001 1d00  7o...K..8.0.....
+000001e0: 4796 c400 0013 7f00 4796 c400 002e eb00  G.......G.......
+000001f0: 47ab 7600 002e b800 47ab 7600 0053 6800  G.v.....G.v..Sh.
+00000200: 4a2b 8200 003c a800 4c99 6200 001b a400  J+...<..L.b.....
+00000210: 4c99 6200 003e d100 52cc bc00 0007 b000  L.b..>..R.......
+00000220: 556a c300 0023 6800 567e 8100 0045 1400  Uj...#h.V~...E..
+00000230: 56ae c200 0055 2000 576d c200 0024 c800  V....U .Wm...$..
+00000240: 576d c200 0044 9e00 587a ff00 000a b000  Wm...D..Xz......
+00000250: 587a ff00 0027 8d00 587a ff00 0048 6800  Xz...'..Xz...Hh.
+00000260: 5aa8 9400 000e 1600 5aa8 9400 0049 cf00  Z.......Z....I..
+00000270: 5aa8 9400 0052 7400 67ab 0600 0053 3c00  Z....Rt.g....S<.
+00000280: 6d92 9400 0051 1400 753c 2300 0044 5d00  m....Q..u<#..D].
+00000290: 8cd2 1500 0010 4200 aa80 2500 001a 6300  ......B...%...c.
+000002a0: ab72 4500 0009 cf00 bf5b b400 0005 f700  .rE......[......
+000002b0: c656 de00 003d 3000 ff2c 7700 001c 2c01  .V...=0..,w...,.
+000002c0: 30ed a300 001c c301 48c4 ff00 001a 9d01  0.......H.......
+000002d0: 4d8a bc00 0021 8801 5478 6c00 0022 1e01  M....!..Txl.."..
+000002e0: 945e f800 0029 3301 9942 b500 0042 8a01  .^...)3..B...B..
+000002f0: 9ce8 5e00 004a 9801 e578 e300 000d 5601  ..^..J...x....V.
+00000300: e907 4500 0042 da01 fdeb 5400 004d ff02  ..E..B....T..M..
+00000310: 3222 f900 0038 8a02 33a9 3400 0008 fb02  2"...8..3.4.....
+00000320: ac2b 0200 0041 7e02 e7d6 5e00 0002 4102  .+...A~...^...A.
+00000330: e7d6 5e00 0015 8b02 e7d6 5e00 0039 b802  ..^.......^..9..
+00000340: e81d 2400 003d fb03 004d 1200 000c 5d03  ..$..=...M....].
+00000350: 0149 e600 0021 4003 0cac 0500 000f cc03  .I...!@.........
+00000360: 0f6b 1200 0043 dc03 0f6b 3200 0023 b903  .k...C...k2..#..
+00000370: 1bec 1200 0013 de03 4485 3000 0000 1e03  ........D.0.....
+00000380: 45b3 3000 0000 5e03 4ecb 9200 0034 0f03  E.0...^.N....4..
+00000390: 4ecb 9200 0052 9603 533f be00 0055 4903  N....R..S?...UI.
+000003a0: 598b 3200 0007 f903 598b 3200 0020 ee03  Y.2.....Y.2.. ..
+000003b0: 598b 3200 0040 c503 5d96 0b00 0040 e803  Y.2..@..]....@..
+000003c0: 6cc3 0400 000b c703 881f d400 0006 2003  l............. .
+000003d0: 9ce3 f400 001e 3f03 9ce9 a500 0025 3a03  ......?......%:.
+000003e0: f5e0 0700 002d 9804 07f6 ee00 0024 7904  .....-.......$y.
+000003f0: 07f6 ee00 0043 8f04 2b4e 0500 001d 6c04  .....C..+N....l.
+00000400: 6c90 3200 0041 0b04 8c96 8100 0014 5f04  l.2..A........_.
+00000410: 8caf 6200 0014 a904 9c8b 8500 0039 4f04  ..b..........9O.
+00000420: a472 8400 002b 4704 ab8e f500 002f e804  .r...+G....../..
+00000430: ab8e fc00 0030 0d04 ab8f 0100 0030 3204  .....0.......02.
+00000440: ab8f 0700 0030 5704 ab8f 0800 0030 7c04  .....0W......0|.
+00000450: b08b a400 003d 8804 b2b6 6400 0008 6d04  .....=....d...m.
+00000460: c4a9 a900 0013 4604 cf76 9400 0004 9404  ......F..v......
+00000470: cf76 9400 0031 7e04 e826 8800 001d a904  .v...1~..&......
+00000480: e826 8800 003f 8204 e842 f200 001d cd04  .&...?...B......
+00000490: e842 f200 0051 8a04 edd3 6400 0036 5604  .B...Q....d..6V.
+000004a0: f5b6 e700 002a 3705 0476 9400 0032 4105  .....*7..v...2A.
+000004b0: 1f06 1500 0051 ad05 3268 c400 0004 1805  .....Q..2h......
+000004c0: 34db 8200 0021 d605 3ddf a300 000a d005  4....!..=.......
+000004d0: 4466 8200 0049 0b05 5776 4500 0045 a305  Df...I..WvE..E..
+000004e0: 6336 9e00 0032 aa05 647d 0e00 002f 9405  c6...2..d}.../..
+000004f0: 7865 9800 0047 a605 7865 b800 0047 c805  xe...G..xe...G..
+00000500: c7f7 2800 0055 ad05 c984 e900 0030 a106  ..(..U.......0..
+00000510: 011e c400 0002 9c06 778d 0800 0006 cf06  ........w.......
+00000520: 778d 0800 001f 2106 7e7c a100 0026 2306  w.....!.~|...&#.
+00000530: 7e7c a100 0046 6906 830d be00 0029 f106  ~|...Fi......)..
+00000540: bdf0 a400 0019 8f06 be94 d200 0052 fa06  .............R..
+00000550: d2af d900 0055 d706 db4d 4200 0027 f206  .....U...MB..'..
+00000560: e056 d800 0024 3e06 e056 d800 0043 5606  .V...$>..V...CV.
+00000570: f895 8e00 0015 f507 2f4a 1500 004a 3607  ......../J...J6.
+00000580: 366b 9300 0005 1a07 50be 3900 0053 9a07  6k......P.9..S..
+00000590: 68f8 4400 004e ab07 693d fe00 0031 a307  h.D..N..i=...1..
+000005a0: 6941 4e00 0032 6607 6cbb 6300 000e 7707  iAN..2f.l.c...w.
+000005b0: 7f18 a400 004b ec07 86be 4800 0036 d507  .....K....H..6..
+000005c0: 8f3a 3e00 0024 fb07 8f3a 3e00 0044 cf07  .:>..$...:>..D..
+000005d0: e67a d700 0030 ee07 e76d c800 0025 7d07  .z...0...m...%}.
+000005e0: e78f a400 0025 b307 e79f 3400 0025 eb07  .....%....4..%..
+000005f0: e79f 3400 0046 2d07 e7e0 a400 002e 4207  ..4..F-.......B.
+00000600: e7f2 3400 002e 7d07 e7f2 3400 004e 4408  ..4...}...4..ND.
+00000610: 14d3 ed00 0032 eb08 14d3 ed00 0046 9a08  .....2.......F..
+00000620: 3292 cb00 0002 7908 3587 6a00 002b a608  2.....y.5.j..+..
+00000630: 36b6 5400 0012 8a08 5ac5 0100 0001 9408  6.T.....Z.......
+00000640: 5ac5 0100 0014 2c08 5ac5 0100 0038 5908  Z.....,.Z....8Y.
+00000650: 678f b400 0027 1f08 679f 2400 0027 5708  g....'..g.$..'W.
+00000660: 679f 2400 0048 2c08 7f52 2500 002a e608  g.$..H,..R%..*..
+00000670: 8879 1400 0019 2108 aae3 e400 0009 9c08  .y....!.........
+00000680: b63d de00 0034 fd08 bd74 5e00 0022 ff08  .=...4...t^.."..
+00000690: d39b 6400 0040 3f08 f89a cb00 0035 d009  ..d..@?......5..
+000006a0: 14be 9200 0049 6309 1c52 9500 002d f709  .....Ic..R...-..
+000006b0: 238c 7500 0016 f209 3f8c ad00 000c da09  #.u.....?.......
+000006c0: 564e 4200 004c 2409 6c61 f400 0013 aa09  VNB..L$.la......
+000006d0: 6c61 f400 002f 1709 6fe6 7e00 0011 8e09  la.../..o.~.....
+000006e0: 8fa3 8700 002f 4c09 97c9 1400 0020 b309  ...../L...... ..
+000006f0: 97c9 1400 0040 8409 97d9 8400 0020 7809  .....@....... x.
+00000700: 9c7f 1a00 0037 7209 a118 8500 0011 0d09  .....7r.........
+00000710: c004 d700 0003 df09 c4e8 d700 0001 c409  ................
+00000720: c8df a200 001e 9409 c943 f500 0010 0709  .........C......
+00000730: c9cf c500 000c 2f09 df31 3800 0047 1709  ....../..18..G..
+00000740: e854 fc00 0015 c609 e854 fc00 003b 1a09  .T.......T...;..
+00000750: f42c fb00 001b 7e0a 16bb 3400 0046 d60a  .,....~...4..F..
+00000760: 2087 bc00 003b f80a 2190 e200 0006 860a   ....;..!.......
+00000770: 2190 e200 001e d50a 3f0e 9500 0028 ea0a  !.......?....(..
+00000780: 5e68 d900 0026 770a 643c 1400 0016 bb0a  ^h...&w.d<......
+00000790: 6789 3b00 0007 0e0a 6789 3b00 001f 630a  g.;.....g.;...c.
+000007a0: 67a9 0200 0007 4a0a 67a9 0200 001f a20a  g.....J.g.......
+000007b0: 6dc8 3e00 0034 960a 7833 e400 0039 790a  m.>..4..x3...9y.
+000007c0: 7d6b 2400 0018 550a 92a2 e500 0029 9d0a  }k$...U......)..
+000007d0: 9612 e500 0028 900a a8b0 0e00 000e 360a  .....(........6.
+000007e0: a8b0 0e00 0049 f00a acdb 7e00 0002 1c0a  .....I....~.....
+000007f0: b945 f500 002b 220a b945 f500 004a 130a  .E...+"..E...J..
+00000800: c389 2500 0028 590a c5b4 4900 003f a40a  ..%..(Y...I..?..
+00000810: c897 c500 0006 480a d2f0 b500 0003 090a  ......H.........
+00000820: d382 7700 0003 570a e2b5 9600 0004 b50a  ..w...W.........
+00000830: f31c 2200 003b 840b 1562 0700 004f 300b  .."..;...b...O0.
+00000840: 1805 3900 0015 3b0b 4597 5500 0008 1b0b  ..9...;.E.U.....
+00000850: 5d8a f400 001f e10b 6628 d200 0034 540b  ].......f(...4T.
+00000860: 7fe2 de00 0033 2a0b ad17 7800 001b 500b  .....3*...x...P.
+00000870: ff25 ce00 001c 7e0c 08f5 6c00 003d b60c  .%....~...l..=..
+00000880: 107d 9300 0003 a10c 10ba b200 0027 b00c  .}...........'..
+00000890: 1536 f700 002d 190c 1f2f 0200 004c 750c  .6...-.../...Lu.
+000008a0: 29f2 a400 004f 0a0c 6a19 e900 003c e10c  )....O..j....<..
+000008b0: 8c09 2900 001d 350c 8c09 2900 003f 4d0c  ..)...5...)..?M.
+000008c0: 9688 9500 0014 830c a3fa 5f00 001a 250c  .........._...%.
+000008d0: a6e8 d400 003a 5e0c bb01 7300 000c 9d0c  .....:^...s.....
+000008e0: bb01 7300 0033 810c c9a0 0e00 002d 730d  ..s..3.......-s.
+000008f0: 0218 6400 0048 bb0d 07a4 f800 003b 470d  ..d..H.......;G.
+00000900: 1f27 b200 0014 d70d 3504 b400 003a ba0d  .'......5....:..
+00000910: 76f7 5900 001b d30d 825f 7300 000f 1a0d  v.Y......_s.....
+00000920: a03c 1200 0050 020d d0ff 4c00 002c cd0d  .<...P....L..,..
+00000930: f2ea c200 003c 3e0d fe4e 2400 0019 d80d  .....<>..N$.....
+00000940: fe4e 2400 0050 c80e 0543 5500 0024 000e  .N$..P...CU..$..
+00000950: 05d1 b500 0050 610e 0743 5500 0044 210e  .....Pa..CU..D!.
+00000960: 0906 8800 0037 ac0e 233d d500 004c bb0e  .....7..#=...L..
+00000970: 87ac 6400 0020 2a0e 93fa 5200 0017 970e  ..d.. *...R.....
+00000980: a32f e400 003e fe0e c497 a200 000b 3e0e  ./...>........>.
+00000990: c72a a600 0005 820e de3d a200 0039 f10e  .*.......=...9..
+000009a0: e46b 3400 0047 ea0e fdeb 3400 0045 eb0f  .k4..G....4..E..
+000009b0: 165e c400 0045 540f 3562 ce00 0017 f80f  .^...ET.5b......
+000009c0: 6963 bc00 000d 1f0f 6963 bc00 002a ac0f  ic......ic...*..
+000009d0: 6963 bc00 0052 3b0f 6978 c700 0033 c20f  ic...R;.ix...3..
+000009e0: 6c98 6c00 0054 f50f 7ddd 2800 004d 630f  l.l..T..}.(..Mc.
+000009f0: 8007 d400 0038 c90f 8313 8900 0013 130f  .....8..........
+00000a00: cb15 5200 0018 d70f e6f6 3400 003f cc69  ..R.......4..?.i
+00000a10: 0000 5601 03ff ffff ff08 0000 0000 0600  ..V.............
+00000a20: 0000 032e 2e2e 0700 0000 0644 6961 6c6f  ...........Dialo
+00000a30: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00000a40: 0631 3135 3230 3007 0000 0006 4469 616c  .115200.....Dial
+00000a50: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
+00000a60: 0004 3132 3030 0700 0000 0644 6961 6c6f  ..1200.....Dialo
+00000a70: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00000a80: 0631 3238 3030 3007 0000 0006 4469 616c  .128000.....Dial
+00000a90: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
+00000aa0: 0005 3134 3430 3007 0000 0006 4469 616c  ..14400.....Dial
+00000ab0: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
+00000ac0: 0005 3139 3230 3007 0000 0006 4469 616c  ..19200.....Dial
+00000ad0: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
+00000ae0: 0004 3234 3030 0700 0000 0644 6961 6c6f  ..2400.....Dialo
+00000af0: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00000b00: 0533 3834 3030 0700 0000 0644 6961 6c6f  .38400.....Dialo
+00000b10: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00000b20: 0434 3830 3007 0000 0006 4469 616c 6f67  .4800.....Dialog
+00000b30: 0103 ffff ffff 0800 0000 0006 0000 0005  ................
+00000b40: 3537 3630 3007 0000 0006 4469 616c 6f67  57600.....Dialog
+00000b50: 0103 ffff ffff 0800 0000 0006 0000 0004  ................
+00000b60: 3936 3030 0700 0000 0644 6961 6c6f 6701  9600.....Dialog.
+00000b70: 03ff ffff ff08 0000 0000 0600 0000 013c  ...............<
+00000b80: 0700 0000 0644 6961 6c6f 6701 03ff ffff  .....Dialog.....
+00000b90: ff08 0000 0000 0600 0000 013e 0700 0000  ...........>....
+00000ba0: 0644 6961 6c6f 6701 0300 0000 0e00 4100  .Dialog.......A.
+00000bb0: 6e00 7400 6500 6e00 6e00 6508 0000 0000  n.t.e.n.n.e.....
+00000bc0: 0600 0000 0741 6e74 656e 6e61 0700 0000  .....Antenna....
+00000bd0: 0644 6961 6c6f 6701 0300 0000 1600 4100  .Dialog.......A.
+00000be0: 7500 6600 7300 7400 6500 6900 6700 6500  u.f.s.t.e.i.g.e.
+00000bf0: 6e00 6408 0000 0000 0600 0000 0941 7363  n.d..........Asc
+00000c00: 656e 6469 6e67 0700 0000 0644 6961 6c6f  ending.....Dialo
+00000c10: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00000c20: 0343 4154 0700 0000 0644 6961 6c6f 6701  .CAT.....Dialog.
+00000c30: 03ff ffff ff08 0000 0000 0600 0000 0a43  ...............C
+00000c40: 422d 5374 6174 696f 6e07 0000 0006 4469  B-Station.....Di
+00000c50: 616c 6f67 0103 0000 0014 0052 0075 0066  alog.......R.u.f
+00000c60: 007a 0065 0069 0063 0068 0065 006e 0800  .z.e.i.c.h.e.n..
+00000c70: 0000 0006 0000 0009 4361 6c6c 2073 6967  ........Call sig
+00000c80: 6e07 0000 0006 4469 616c 6f67 0103 ffff  n.....Dialog....
+00000c90: ffff 0800 0000 0006 0000 0008 4361 6c6c  ............Call
+00000ca0: 626f 6f6b 0700 0000 0644 6961 6c6f 6701  book.....Dialog.
+00000cb0: 0300 0000 3800 5a00 6500 7200 7400 6900  ....8.Z.e.r.t.i.
+00000cc0: 6600 6900 6b00 6100 7400 2000 6200 6500  f.i.k.a.t. .b.e.
+00000cd0: 6e00 f600 7400 6900 6700 7400 2000 5000  n...t.i.g.t. .P.
+00000ce0: 6100 7300 7300 7700 6f00 7200 7408 0000  a.s.s.w.o.r.t...
+00000cf0: 0000 0600 0000 1a43 6572 7469 6669 6361  .......Certifica
+00000d00: 7465 206e 6565 6473 2070 6173 7377 6f72  te needs passwor
+00000d10: 6407 0000 0006 4469 616c 6f67 0103 0000  d.....Dialog....
+00000d20: 0024 0053 0070 0061 006c 0074 0065 006e  .$.S.p.a.l.t.e.n
+00000d30: 0020 0076 0065 0072 0073 0074 0065 0063  . .v.e.r.s.t.e.c
+00000d40: 006b 0065 006e 0800 0000 0006 0000 000f  .k.e.n..........
+00000d50: 436f 6c75 6d6e 7320 746f 2068 6964 6507  Columns to hide.
+00000d60: 0000 0006 4469 616c 6f67 0103 0000 0020  ....Dialog..... 
+00000d70: 0053 0070 0061 006c 0074 0065 006e 0020  .S.p.a.l.t.e.n. 
+00000d80: 0061 006e 007a 0065 0069 0067 0065 006e  .a.n.z.e.i.g.e.n
+00000d90: 0800 0000 0006 0000 000f 436f 6c75 6d6e  ..........Column
+00000da0: 7320 746f 2073 686f 7707 0000 0006 4469  s to show.....Di
+00000db0: 616c 6f67 0103 0000 0018 0041 006e 006d  alog.......A.n.m
+00000dc0: 0065 006c 0064 0065 0064 0061 0074 0065  .e.l.d.e.d.a.t.e
+00000dd0: 006e 0800 0000 0006 0000 000b 4372 6564  .n..........Cred
+00000de0: 656e 7469 616c 7307 0000 0006 4469 616c  entials.....Dial
+00000df0: 6f67 0103 0000 0014 0041 0062 0073 0074  og.......A.b.s.t
+00000e00: 0065 0069 0067 0065 006e 0064 0800 0000  .e.i.g.e.n.d....
+00000e10: 0006 0000 000a 4465 7363 656e 6469 6e67  ......Descending
+00000e20: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
+00000e30: 3e00 5700 6900 7200 6b00 7300 6100 6d00  >.W.i.r.k.s.a.m.
+00000e40: 2000 6e00 6100 6300 6800 2000 4100 6e00   .n.a.c.h. .A.n.
+00000e50: 7700 6500 6e00 6400 7500 6e00 6700 7300  w.e.n.d.u.n.g.s.
+00000e60: 6e00 6500 7500 7300 7400 6100 7200 7408  n.e.u.s.t.a.r.t.
+00000e70: 0000 0000 0600 0000 2345 6666 6563 7469  ........#Effecti
+00000e80: 7665 2061 6674 6572 2061 7070 6c69 6361  ve after applica
+00000e90: 7469 6f6e 2072 6573 7461 7274 0700 0000  tion restart....
+00000ea0: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
+00000eb0: 0000 0600 0000 0645 7870 6f72 7407 0000  .......Export...
+00000ec0: 0006 4469 616c 6f67 0103 0000 0034 0045  ..Dialog.....4.E
+00000ed0: 0078 0070 006f 0072 0074 0069 0065 0072  .x.p.o.r.t.i.e.r
+00000ee0: 0065 0020 0043 0042 002d 0051 0053 004f  .e. .C.B.-.Q.S.O
+00000ef0: 0073 0020 0069 006e 0020 0041 0044 0049  .s. .i.n. .A.D.I
+00000f00: 0046 0800 0000 0006 0000 0016 4578 706f  .F..........Expo
+00000f10: 7274 2043 4220 5153 4f73 2074 6f20 4144  rt CB QSOs to AD
+00000f20: 4946 0700 0000 0644 6961 6c6f 6701 0300  IF.....Dialog...
+00000f30: 0000 3600 4500 7800 7000 6f00 7200 7400  ..6.E.x.p.o.r.t.
+00000f40: 6900 6500 7200 6500 2000 6e00 7500 7200  i.e.r.e. .n.u.r.
+00000f50: 2000 6e00 6500 7500 6500 7300 7400 6500   .n.e.u.e.s.t.e.
+00000f60: 2000 5100 5300 4f00 7308 0000 0000 0600   .Q.S.O.s.......
+00000f70: 0000 1745 7870 6f72 7420 6f6e 6c79 2072  ...Export only r
+00000f80: 6563 656e 7420 5153 4f73 0700 0000 0644  ecent QSOs.....D
+00000f90: 6961 6c6f 6701 0300 0000 4200 4500 7800  ialog.....B.E.x.
+00000fa0: 7000 6f00 7200 7400 6900 6500 7200 6500  p.o.r.t.i.e.r.e.
+00000fb0: 2000 6500 6900 6700 6500 6e00 6500 2000   .e.i.g.e.n.e. .
+00000fc0: 4e00 6f00 7400 6900 7a00 6500 6e00 2000  N.o.t.i.z.e.n. .
+00000fd0: 6900 6e00 2000 4100 4400 4900 4608 0000  i.n. .A.D.I.F...
+00000fe0: 0000 0600 0000 1845 7870 6f72 7420 6f77  .......Export ow
+00000ff0: 6e20 6e6f 7465 7320 746f 2041 4449 4607  n notes to ADIF.
+00001000: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
+00001010: 0800 0000 0006 0000 000e 4861 6d6c 6962  ..........Hamlib
+00001020: 2072 6967 6374 6c64 0700 0000 0644 6961   rigctld.....Dia
+00001030: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
+00001040: 0000 0d49 6d70 6f72 742f 4578 706f 7274  ...Import/Export
+00001050: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
+00001060: 1a00 5300 6300 6800 6e00 6900 7400 7400  ..S.c.h.n.i.t.t.
+00001070: 7300 7400 6500 6c00 6c00 6508 0000 0000  s.t.e.l.l.e.....
+00001080: 0600 0000 0949 6e74 6572 6661 6365 0700  .....Interface..
+00001090: 0000 0644 6961 6c6f 6701 0300 0000 2000  ...Dialog..... .
+000010a0: 6c00 6500 7400 7a00 7400 6500 7300 2000  l.e.t.z.t.e.s. .
+000010b0: 4800 6100 6c00 6200 6a00 6100 6800 7208  H.a.l.b.j.a.h.r.
+000010c0: 0000 0000 0600 0000 0e4c 6173 7420 6861  .........Last ha
+000010d0: 6c66 2079 6561 7207 0000 0006 4469 616c  lf year.....Dial
+000010e0: 6f67 0103 0000 001a 006c 0065 0074 007a  og.......l.e.t.z
+000010f0: 0074 0065 006e 0020 004d 006f 006e 0061  .t.e.n. .M.o.n.a
+00001100: 0074 0800 0000 0006 0000 000a 4c61 7374  .t..........Last
+00001110: 206d 6f6e 7468 0700 0000 0644 6961 6c6f   month.....Dialo
+00001120: 6701 0300 0000 1800 6c00 6500 7400 7a00  g.......l.e.t.z.
+00001130: 7400 6500 2000 5700 6f00 6300 6800 6508  t.e. .W.o.c.h.e.
+00001140: 0000 0000 0600 0000 094c 6173 7420 7765  .........Last we
+00001150: 656b 0700 0000 0644 6961 6c6f 6701 0300  ek.....Dialog...
+00001160: 0000 1800 6c00 6500 7400 7a00 7400 6500  ....l.e.t.z.t.e.
+00001170: 7300 2000 4a00 6100 6800 7208 0000 0000  s. .J.a.h.r.....
+00001180: 0600 0000 094c 6173 7420 7965 6172 0700  .....Last year..
+00001190: 0000 0644 6961 6c6f 6701 0300 0000 0c00  ...Dialog.......
+000011a0: 4200 7200 6500 6900 7400 6508 0000 0000  B.r.e.i.t.e.....
+000011b0: 0600 0000 034c 6174 0700 0000 0644 6961  .....Lat.....Dia
+000011c0: 6c6f 6701 0300 0000 0a00 5300 7400 7500  log.......S.t.u.
+000011d0: 6600 6508 0000 0000 0600 0000 054c 6576  f.e..........Lev
+000011e0: 656c 0700 0000 0644 6961 6c6f 6701 03ff  el.....Dialog...
+000011f0: ffff ff08 0000 0000 0600 0000 044c 6f54  .............LoT
+00001200: 5707 0000 0006 4469 616c 6f67 0103 ffff  W.....Dialog....
+00001210: ffff 0800 0000 0006 0000 0007 4c6f 6361  ............Loca
+00001220: 746f 7207 0000 0006 4469 616c 6f67 0103  tor.....Dialog..
+00001230: 0000 002c 004c 006f 0067 0020 0069 006e  ...,.L.o.g. .i.n
+00001240: 0020 0044 0061 0074 0065 0069 0020 0073  . .D.a.t.e.i. .s
+00001250: 0063 0068 0072 0065 0069 0062 0065 006e  .c.h.r.e.i.b.e.n
+00001260: 0800 0000 0006 0000 000b 4c6f 6720 746f  ..........Log to
+00001270: 2066 696c 6507 0000 0006 4469 616c 6f67   file.....Dialog
+00001280: 0103 0000 001e 004c 006f 0067 0067 0069  .......L.o.g.g.i
+00001290: 006e 0067 002d 0041 0075 0073 0067 0061  .n.g.-.A.u.s.g.a
+000012a0: 0062 0065 0800 0000 0006 0000 000e 4c6f  .b.e..........Lo
+000012b0: 6767 696e 6720 6f75 7470 7574 0700 0000  gging output....
+000012c0: 0644 6961 6c6f 6701 0300 0000 0a00 4c00  .Dialog.......L.
+000012d0: e400 6e00 6700 6508 0000 0000 0600 0000  ..n.g.e.........
+000012e0: 034c 6f6e 0700 0000 0644 6961 6c6f 6701  .Lon.....Dialog.
+000012f0: 03ff ffff ff08 0000 0000 0600 0000 044e  ...............N
+00001300: 616d 6507 0000 0006 4469 616c 6f67 0103  ame.....Dialog..
+00001310: 0000 005e 0043 0042 0020 0051 0053 004f  ...^.C.B. .Q.S.O
+00001320: 0073 0020 0077 0065 0072 0064 0065 006e  .s. .w.e.r.d.e.n
+00001330: 0020 0062 0065 0069 006d 0020 0049 006d  . .b.e.i.m. .I.m
+00001340: 0070 006f 0072 0074 0020 0069 006d 006d  .p.o.r.t. .i.m.m
+00001350: 0065 0072 0020 0062 0065 0072 00fc 0063  .e.r. .b.e.r...c
+00001360: 006b 0073 0069 0063 0068 0074 0069 0067  .k.s.i.c.h.t.i.g
+00001370: 0074 0800 0000 0006 0000 0028 4f6e 2069  .t.........(On i
+00001380: 6d70 6f72 7420 4342 2051 534f 7320 7769  mport CB QSOs wi
+00001390: 6c6c 2061 6c77 6179 7320 6265 2068 616e  ll always be han
+000013a0: 646c 6564 0700 0000 0644 6961 6c6f 6701  dled.....Dialog.
+000013b0: 0300 0000 1000 5000 6100 7300 7300 7700  ......P.a.s.s.w.
+000013c0: 6f00 7200 7408 0000 0000 0600 0000 0850  o.r.t..........P
+000013d0: 6173 7377 6f72 6407 0000 0006 4469 616c  assword.....Dial
+000013e0: 6f67 0103 0000 0070 0050 0061 0073 0073  og.....p.P.a.s.s
+000013f0: 0077 006f 0072 0074 0020 0064 0065 0073  .w.o.r.t. .d.e.s
+00001400: 0020 004c 006f 0054 0057 002d 004f 006e  . .L.o.T.W.-.O.n
+00001410: 006c 0069 006e 0065 002d 0041 0063 0063  .l.i.n.e.-.A.c.c
+00001420: 006f 0075 006e 0074 0073 002c 0020 006e  .o.u.n.t.s.,. .n
+00001430: 0069 0063 0068 0074 0020 0064 0065 0073  .i.c.h.t. .d.e.s
+00001440: 0020 005a 0065 0072 0074 0069 0066 0069  . .Z.e.r.t.i.f.i
+00001450: 006b 0061 0074 0073 0800 0000 0006 0000  .k.a.t.s........
+00001460: 0038 5061 7373 776f 7264 2066 6f72 204c  .8Password for L
+00001470: 6f54 5720 6f6e 6c69 6e65 2061 6363 6f75  oTW online accou
+00001480: 6e74 206e 6f74 2066 6f72 2074 6865 2063  nt not for the c
+00001490: 6572 7469 6669 6361 7465 0700 0000 0644  ertificate.....D
+000014a0: 6961 6c6f 6701 03ff ffff ff08 0000 0000  ialog...........
+000014b0: 0600 0000 0351 5448 0700 0000 0644 6961  .....QTH.....Dia
+000014c0: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
+000014d0: 0000 0552 6164 696f 0700 0000 0644 6961  ...Radio.....Dia
+000014e0: 6c6f 6701 0300 0000 1800 4e00 6500 7500  log.......N.e.u.
+000014f0: 6500 7300 7400 6500 2000 5100 5300 4f00  e.s.t.e. .Q.S.O.
+00001500: 7308 0000 0000 0600 0000 0b52 6563 656e  s..........Recen
+00001510: 7420 5153 4f73 0700 0000 0644 6961 6c6f  t QSOs.....Dialo
+00001520: 6701 0300 0000 1200 4600 7500 6e00 6b00  g.......F.u.n.k.
+00001530: 6700 6500 7200 e400 7408 0000 0000 0600  g.e.r...t.......
+00001540: 0000 0352 6967 0700 0000 0644 6961 6c6f  ...Rig.....Dialo
+00001550: 6701 0300 0000 4c00 5300 6900 6500 6800  g.....L.S.i.e.h.
+00001560: 6500 2000 4500 6900 6e00 7300 7400 6500  e. .E.i.n.s.t.e.
+00001570: 6c00 6c00 7500 6e00 6700 6500 6e00 2000  l.l.u.n.g.e.n. .
+00001580: 5200 6500 6900 7400 6500 7200 2000 2200  R.e.i.t.e.r. .".
+00001590: 4100 6e00 7700 6500 6e00 6400 7500 6e00  A.n.w.e.n.d.u.n.
+000015a0: 6700 2208 0000 0000 0600 0000 2253 6565  g."........."See
+000015b0: 2073 6574 7469 6e67 7320 7061 6765 2022   settings page "
+000015c0: 5573 6572 2069 6e74 6572 6661 6365 2207  User interface".
+000015d0: 0000 0006 4469 616c 6f67 0103 0000 0034  ....Dialog.....4
+000015e0: 0043 0042 002d 0042 0061 006e 0064 0020  .C.B.-.B.a.n.d. 
+000015f0: 0061 0075 0074 006f 006d 0061 0074 0069  .a.u.t.o.m.a.t.i
+00001600: 0073 0063 0068 0020 0077 00e4 0068 006c  .s.c.h. .w...h.l
+00001610: 0065 006e 0800 0000 0006 0000 0019 5365  .e.n..........Se
+00001620: 6c65 6374 2043 4220 6261 6e64 2062 7920  lect CB band by 
+00001630: 6465 6661 756c 7407 0000 0006 4469 616c  default.....Dial
+00001640: 6f67 0103 0000 000c 0044 0069 0065 006e  og.......D.i.e.n
+00001650: 0073 0074 0800 0000 0006 0000 0007 5365  .s.t..........Se
+00001660: 7276 6963 6507 0000 0006 4469 616c 6f67  rvice.....Dialog
+00001670: 0103 0000 001a 0053 0065 0074 007a 0065  .......S.e.t.z.e
+00001680: 0020 004c 006f 0063 0061 0074 006f 0072  . .L.o.c.a.t.o.r
+00001690: 0800 0000 0006 0000 000b 5365 7420 6c6f  ..........Set lo
+000016a0: 6361 746f 7207 0000 0006 4469 616c 6f67  cator.....Dialog
+000016b0: 0103 0000 001a 0045 0069 006e 0073 0074  .......E.i.n.s.t
+000016c0: 0065 006c 006c 0075 006e 0067 0065 006e  .e.l.l.u.n.g.e.n
+000016d0: 0800 0000 0006 0000 0008 5365 7474 696e  ..........Settin
+000016e0: 6773 0700 0000 0644 6961 6c6f 6701 0300  gs.....Dialog...
+000016f0: 0000 1c00 5a00 6500 6900 6700 6500 2000  ....Z.e.i.g.e. .
+00001700: 5100 5300 4f00 7300 2000 6600 fc00 7208  Q.S.O.s. .f...r.
+00001710: 0000 0000 0600 0000 0e53 686f 7720 5153  .........Show QS
+00001720: 4f73 2066 726f 6d07 0000 0006 4469 616c  Os from.....Dial
+00001730: 6f67 0103 0000 0014 007a 0065 0069 0067  og.......z.e.i.g
+00001740: 0065 0020 0061 006c 006c 0065 0800 0000  .e. .a.l.l.e....
+00001750: 0006 0000 0008 5368 6f77 2061 6c6c 0700  ......Show all..
+00001760: 0000 0644 6961 6c6f 6701 0300 0000 4000  ...Dialog.....@.
+00001770: 5300 7000 6100 6c00 7400 6500 6e00 2000  S.p.a.l.t.e.n. .
+00001780: 6100 6e00 7a00 6500 6900 6700 6500 6e00  a.n.z.e.i.g.e.n.
+00001790: 2000 6f00 6400 6500 7200 2000 7600 6500   .o.d.e.r. .v.e.
+000017a0: 7200 7300 7400 6500 6300 6b00 6500 6e08  r.s.t.e.c.k.e.n.
+000017b0: 0000 0000 0600 0000 1453 686f 7720 6f72  .........Show or
+000017c0: 2068 6964 6520 636f 6c75 6d6e 7307 0000   hide columns...
+000017d0: 0006 4469 616c 6f67 0103 0000 0028 0053  ..Dialog.....(.S
+000017e0: 006f 0072 0074 0069 0065 0072 0065 0020  .o.r.t.i.e.r.e. 
+000017f0: 006e 0061 0063 0068 0020 0053 0070 0061  .n.a.c.h. .S.p.a
+00001800: 006c 0074 0065 0800 0000 0006 0000 000e  .l.t.e..........
+00001810: 536f 7274 206f 6e20 636f 6c75 6d6e 0700  Sort on column..
+00001820: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00001830: 0000 0000 0600 0000 0553 7461 7274 0700  .........Start..
+00001840: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00001850: 0000 0000 0600 0000 0753 7461 7469 6f6e  .........Station
+00001860: 0700 0000 0644 6961 6c6f 6701 03ff ffff  .....Dialog.....
+00001870: ff08 0000 0000 0600 0000 0454 5153 4c07  ...........TQSL.
+00001880: 0000 0006 4469 616c 6f67 0103 0000 0064  ....Dialog.....d
+00001890: 0056 0065 0072 0077 0065 006e 0064 0065  .V.e.r.w.e.n.d.e
+000018a0: 0020 0064 0069 0065 0020 006b 006f 006e  . .d.i.e. .k.o.n
+000018b0: 0066 0069 0067 0075 0072 0069 0065 0072  .f.i.g.u.r.i.e.r
+000018c0: 0074 0065 0020 0049 0044 0020 0062 0065  .t.e. .I.D. .b.e
+000018d0: 0069 0020 0066 0065 0068 006c 0065 006e  .i. .f.e.h.l.e.n
+000018e0: 0064 0065 006e 0020 0057 0065 0072 0074  .d.e.n. .W.e.r.t
+000018f0: 0065 006e 0800 0000 0006 0000 0024 5573  .e.n.........$Us
+00001900: 6520 636f 6e66 6967 7572 6564 2049 4420  e configured ID 
+00001910: 666f 7220 6d69 7373 696e 6720 7661 6c75  for missing valu
+00001920: 6573 0700 0000 0644 6961 6c6f 6701 0300  es.....Dialog...
+00001930: 0000 6e00 5600 6500 7200 7700 6500 6e00  ..n.V.e.r.w.e.n.
+00001940: 6400 6500 2000 6400 6900 6500 2000 6b00  d.e. .d.i.e. .k.
+00001950: 6f00 6e00 6600 6900 6700 7500 7200 6900  o.n.f.i.g.u.r.i.
+00001960: 6500 7200 7400 6500 2000 5300 7400 6100  e.r.t.e. .S.t.a.
+00001970: 7400 6900 6f00 6e00 2000 6200 6500 6900  t.i.o.n. .b.e.i.
+00001980: 2000 6600 6500 6800 6c00 6500 6e00 6400   .f.e.h.l.e.n.d.
+00001990: 6500 6e00 2000 5700 6500 7200 7400 6500  e.n. .W.e.r.t.e.
+000019a0: 6e08 0000 0000 0600 0000 2955 7365 2063  n.........)Use c
+000019b0: 6f6e 6669 6775 7265 6420 5374 6174 696f  onfigured Statio
+000019c0: 6e20 666f 7220 6d69 7373 696e 6720 7661  n for missing va
+000019d0: 6c75 6573 0700 0000 0644 6961 6c6f 6701  lues.....Dialog.
+000019e0: 0300 0000 1200 4100 6e00 7700 6500 6e00  ......A.n.w.e.n.
+000019f0: 6400 7500 6e00 6708 0000 0000 0600 0000  d.u.n.g.........
+00001a00: 0e55 7365 7220 696e 7465 7266 6163 6507  .User interface.
+00001a10: 0000 0006 4469 616c 6f67 0103 0000 0018  ....Dialog......
+00001a20: 0042 0065 006e 0075 0074 007a 0065 0072  .B.e.n.u.t.z.e.r
+00001a30: 006e 0061 006d 0065 0800 0000 0006 0000  .n.a.m.e........
+00001a40: 0008 5573 6572 6e61 6d65 0700 0000 0644  ..Username.....D
+00001a50: 6961 6c6f 6701 0300 0000 7800 4200 6500  ialog.....x.B.e.
+00001a60: 6e00 7500 7400 7a00 6500 7200 6e00 6100  n.u.t.z.e.r.n.a.
+00001a70: 6d00 6500 2000 6400 6500 7300 2000 4c00  m.e. .d.e.s. .L.
+00001a80: 6f00 5400 5700 2d00 4f00 6e00 6c00 6900  o.T.W.-.O.n.l.i.
+00001a90: 6e00 6500 2d00 4100 6300 6300 6f00 7500  n.e.-.A.c.c.o.u.
+00001aa0: 6e00 7400 7300 2c00 2000 6e00 6900 6300  n.t.s.,. .n.i.c.
+00001ab0: 6800 7400 2000 6400 6500 7300 2000 5a00  h.t. .d.e.s. .Z.
+00001ac0: 6500 7200 7400 6900 6600 6900 6b00 6100  e.r.t.i.f.i.k.a.
+00001ad0: 7400 7308 0000 0000 0600 0000 3855 7365  t.s.........8Use
+00001ae0: 726e 616d 6520 666f 7220 4c6f 5457 206f  rname for LoTW o
+00001af0: 6e6c 696e 6520 6163 636f 756e 7420 6e6f  nline account no
+00001b00: 7420 666f 7220 7468 6520 6365 7274 6966  t for the certif
+00001b10: 6963 6174 6507 0000 0006 4469 616c 6f67  icate.....Dialog
+00001b20: 0103 0000 0020 0044 0061 0074 0065 0069  ..... .D.a.t.e.i
+00001b30: 00fc 0062 0065 0072 0077 0061 0063 0068  ...b.e.r.w.a.c.h
+00001b40: 0075 006e 0067 0800 0000 0006 0000 000a  .u.n.g..........
+00001b50: 5761 7463 6820 4669 6c65 0700 0000 0644  Watch File.....D
+00001b60: 6961 6c6f 6701 03ff ffff ff08 0000 0000  ialog...........
+00001b70: 0600 0000 0465 5153 4c07 0000 0006 4469  .....eQSL.....Di
+00001b80: 616c 6f67 0103 ffff ffff 0800 0000 0006  alog............
+00001b90: 0000 0002 c2b0 0700 0000 0644 6961 6c6f  ...........Dialo
+00001ba0: 6701 0300 0000 9e00 4500 6900 6e00 2000  g.......E.i.n. .
+00001bb0: 4400 6100 7400 6500 6e00 6200 6100 6e00  D.a.t.e.n.b.a.n.
+00001bc0: 6b00 2d00 4200 6100 6300 6b00 7500 7000  k.-.B.a.c.k.u.p.
+00001bd0: 2000 6b00 6f00 6e00 6e00 7400 6500 2000   .k.o.n.n.t.e. .
+00001be0: 6e00 6900 6300 6800 7400 2000 6500 7200  n.i.c.h.t. .e.r.
+00001bf0: 7300 7400 6500 6c00 6c00 7400 2000 7700  s.t.e.l.l.t. .w.
+00001c00: 6500 7200 6400 6500 6e00 2e00 0a00 4400  e.r.d.e.n.....D.
+00001c10: 6900 6500 2000 4400 6100 7400 6500 6900  i.e. .D.a.t.e.i.
+00001c20: 2000 6500 7800 6900 7300 7400 6900 6500   .e.x.i.s.t.i.e.
+00001c30: 7200 7400 2000 6200 6500 7200 6500 6900  r.t. .b.e.r.e.i.
+00001c40: 7400 7300 2e08 0000 0000 0600 0000 4041  t.s...........@A
+00001c50: 2064 6174 6162 6173 6520 6261 636b 7570   database backup
+00001c60: 2063 6f75 6c64 206e 6f74 2062 6520 6372   could not be cr
+00001c70: 6561 7465 642e 0a54 6865 2066 696c 6520  eated..The file 
+00001c80: 616c 7265 6164 7920 6578 6973 7473 2e07  already exists..
+00001c90: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00001ca0: 0000 4e00 4500 6900 6e00 2000 4100 4400  ..N.E.i.n. .A.D.
+00001cb0: 4900 4600 2d00 4600 6500 6c00 6400 2000  I.F.-.F.e.l.d. .
+00001cc0: 6600 6500 6800 6c00 7400 2000 6600 fc00  f.e.h.l.t. .f...
+00001cd0: 7200 2000 6400 6500 6e00 2000 4c00 6f00  r. .d.e.n. .L.o.
+00001ce0: 5400 5700 2d00 5500 7000 6c00 6f00 6100  T.W.-.U.p.l.o.a.
+00001cf0: 6408 0000 0000 0600 0000 1d41 2066 6965  d..........A fie
+00001d00: 6c64 2069 7320 6d69 7373 696e 6720 666f  ld is missing fo
+00001d10: 7220 7570 6c6f 6164 0700 0000 0944 7261  r upload.....Dra
+00001d20: 676f 6e4c 6f67 0103 ffff ffff 0800 0000  gonLog..........
+00001d30: 0006 0000 0015 4144 4946 2033 2028 2a2e  ......ADIF 3 (*.
+00001d40: 6164 6920 2a2e 6164 6966 2907 0000 0009  adi *.adif).....
+00001d50: 4472 6167 6f6e 4c6f 6701 03ff ffff ff08  DragonLog.......
+00001d60: 0000 0000 0600 0000 1b41 4449 4620 3320  .........ADIF 3 
+00001d70: 282a 2e61 6478 202a 2e61 6469 202a 2e61  (*.adx *.adi *.a
+00001d80: 6469 6629 0700 0000 0944 7261 676f 6e4c  dif).....DragonL
+00001d90: 6f67 0103 0000 0008 00dc 0062 0065 0072  og.........b.e.r
+00001da0: 0800 0000 0006 0000 0005 4162 6f75 7407  ..........About.
+00001db0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00001dc0: 0000 0e00 dc00 6200 6500 7200 2000 5100  ......b.e.r. .Q.
+00001dd0: 7408 0000 0000 0600 0000 0841 626f 7574  t..........About
+00001de0: 2051 7407 0000 0009 4472 6167 6f6e 4c6f   Qt.....DragonLo
+00001df0: 6701 0300 0000 2000 4100 6900 7200 6300  g..... .A.i.r.c.
+00001e00: 7200 6100 6600 7400 2d00 5300 6300 6100  r.a.f.t.-.S.c.a.
+00001e10: 7400 7400 6500 7208 0000 0000 0600 0000  t.t.e.r.........
+00001e20: 1041 6972 6372 6166 7420 5363 6174 7465  .Aircraft Scatte
+00001e30: 7207 0000 0009 4472 6167 6f6e 4c6f 6701  r.....DragonLog.
+00001e40: 0300 0000 0e00 4100 6e00 7400 6500 6e00  ......A.n.t.e.n.
+00001e50: 6e00 6508 0000 0000 0600 0000 0741 6e74  n.e..........Ant
+00001e60: 656e 6e61 0700 0000 0944 7261 676f 6e4c  enna.....DragonL
+00001e70: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
+00001e80: 0006 4175 726f 7261 0700 0000 0944 7261  ..Aurora.....Dra
+00001e90: 676f 6e4c 6f67 0103 ffff ffff 0800 0000  gonLog..........
+00001ea0: 0006 0000 0008 4175 726f 7261 2d45 0700  ......Aurora-E..
+00001eb0: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00001ec0: 000a 0041 0075 0074 006f 0072 0800 0000  ...A.u.t.o.r....
+00001ed0: 0006 0000 0006 4175 7468 6f72 0700 0000  ......Author....
+00001ee0: 0944 7261 676f 6e4c 6f67 0103 0000 0018  .DragonLog......
+00001ef0: 0042 0061 0063 006b 002d 0053 0063 0061  .B.a.c.k.-.S.c.a
+00001f00: 0074 0074 0065 0072 0800 0000 0006 0000  .t.t.e.r........
+00001f10: 000c 4261 636b 2073 6361 7474 6572 0700  ..Back scatter..
+00001f20: 0000 0944 7261 676f 6e4c 6f67 0103 ffff  ...DragonLog....
+00001f30: ffff 0800 0000 0006 0000 0004 4261 6e64  ............Band
+00001f40: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00001f50: 0000 0022 0043 0053 0056 002d 0044 0061  ...".C.S.V.-.D.a
+00001f60: 0074 0065 0069 0020 0028 002a 002e 0063  .t.e.i. .(.*...c
+00001f70: 0073 0076 0029 0800 0000 0006 0000 0010  .s.v.)..........
+00001f80: 4353 562d 4669 6c65 2028 2a2e 6373 7629  CSV-File (*.csv)
+00001f90: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00001fa0: 0000 0014 0052 0075 0066 007a 0065 0069  .....R.u.f.z.e.i
+00001fb0: 0063 0068 0065 006e 0800 0000 0006 0000  .c.h.e.n........
+00001fc0: 0009 4361 6c6c 2073 6967 6e07 0000 0009  ..Call sign.....
+00001fd0: 4472 6167 6f6e 4c6f 6701 0300 0000 0a00  DragonLog.......
+00001fe0: 4b00 6100 6e00 6100 6c08 0000 0000 0600  K.a.n.a.l.......
+00001ff0: 0000 0743 6861 6e6e 656c 0700 0000 0944  ...Channel.....D
+00002000: 7261 676f 6e4c 6f67 0103 0000 0074 0050  ragonLog.....t.P
+00002010: 0072 00fc 0066 0075 006e 0067 0020 0064  .r...f.u.n.g. .d
+00002020: 0065 0072 0020 0044 0061 0074 0065 006e  .e.r. .D.a.t.e.n
+00002030: 0062 0061 006e 006b 0020 0066 0065 0068  .b.a.n.k. .f.e.h
+00002040: 006c 0067 0065 0073 0063 0068 006c 0061  .l.g.e.s.c.h.l.a
+00002050: 0067 0065 006e 002e 0020 0049 006e 0068  .g.e.n... .I.n.h
+00002060: 0061 006c 0074 0020 006e 0069 0063 0068  .a.l.t. .n.i.c.h
+00002070: 0074 0020 006c 0065 0073 0062 0061 0072  .t. .l.e.s.b.a.r
+00002080: 002e 0800 0000 0006 0000 0034 4368 6563  ...........4Chec
+00002090: 6b69 6e67 2064 6174 6162 6173 6520 6661  king database fa
+000020a0: 696c 6564 2e20 436f 6e74 656e 7420 6973  iled. Content is
+000020b0: 206e 6f74 2061 6363 6573 7361 626c 652e   not accessable.
+000020c0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+000020d0: 0000 0012 004b 006f 006d 006d 0065 006e  .....K.o.m.m.e.n
+000020e0: 0074 0061 0072 0800 0000 0006 0000 0007  .t.a.r..........
+000020f0: 436f 6d6d 656e 7407 0000 0009 4472 6167  Comment.....Drag
+00002100: 6f6e 4c6f 6701 0300 0000 6000 5600 6500  onLog.....`.V.e.
+00002110: 7200 6200 6900 6e00 6400 7500 6e00 6700  r.b.i.n.d.u.n.g.
+00002120: 7300 6600 6500 6800 6c00 6500 7200 2000  s.f.e.h.l.e.r. .
+00002130: 6f00 6400 6500 7200 2000 4e00 6500 7400  o.d.e.r. .N.e.t.
+00002140: 7a00 7700 6500 7200 6b00 2000 6e00 6900  z.w.e.r.k. .n.i.
+00002150: 6300 6800 7400 2000 6500 7200 7200 6500  c.h.t. .e.r.r.e.
+00002160: 6900 6300 6800 6200 6100 7208 0000 0000  i.c.h.b.a.r.....
+00002170: 0600 0000 2743 6f6e 6e65 6374 696f 6e20  ....'Connection 
+00002180: 6572 726f 7220 6f72 206e 6574 776f 726b  error or network
+00002190: 2075 6e72 6561 6368 6162 6c65 0700 0000   unreachable....
+000021a0: 0944 7261 676f 6e4c 6f67 0103 0000 002e  .DragonLog......
+000021b0: 0044 0061 0074 0065 006e 0062 0061 006e  .D.a.t.e.n.b.a.n
+000021c0: 006b 002d 0042 0061 0063 006b 0075 0070  .k.-.B.a.c.k.u.p
+000021d0: 0020 0046 0065 0068 006c 0065 0072 0800  . .F.e.h.l.e.r..
+000021e0: 0000 0006 0000 0015 4461 7461 6261 7365  ........Database
+000021f0: 2062 6163 6b75 7020 6572 726f 7207 0000   backup error...
+00002200: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00002210: 2c00 4400 6100 7400 6500 6e00 6200 6100  ,.D.a.t.e.n.b.a.
+00002220: 6e00 6b00 6b00 6f00 6e00 7600 6500 7200  n.k.k.o.n.v.e.r.
+00002230: 7400 6900 6500 7200 7500 6e00 6708 0000  t.i.e.r.u.n.g...
+00002240: 0000 0600 0000 1344 6174 6162 6173 6520  .......Database 
+00002250: 636f 6e76 6572 7369 6f6e 0700 0000 0944  conversion.....D
+00002260: 7261 676f 6e4c 6f67 0103 0000 0048 0044  ragonLog.....H.D
+00002270: 0061 0074 0065 006e 0062 0061 006e 006b  .a.t.e.n.b.a.n.k
+00002280: 006b 006f 006e 0076 0065 0072 0074 0069  .k.o.n.v.e.r.t.i
+00002290: 0065 0072 0075 006e 0067 0020 0061 0062  .e.r.u.n.g. .a.b
+000022a0: 0067 0065 0073 0063 0068 006c 006f 0073  .g.e.s.c.h.l.o.s
+000022b0: 0073 0065 006e 0800 0000 0006 0000 001c  .s.e.n..........
+000022c0: 4461 7461 6261 7365 2063 6f6e 7665 7273  Database convers
+000022d0: 696f 6e20 6669 6e69 7368 6564 0700 0000  ion finished....
+000022e0: 0944 7261 676f 6e4c 6f67 0103 0000 001e  .DragonLog......
+000022f0: 0044 0061 0074 0065 006e 0062 0061 006e  .D.a.t.e.n.b.a.n
+00002300: 006b 0066 0065 0068 006c 0065 0072 0800  .k.f.e.h.l.e.r..
+00002310: 0000 0006 0000 000e 4461 7461 6261 7365  ........Database
+00002320: 2065 7272 6f72 0700 0000 0944 7261 676f   error.....Drago
+00002330: 6e4c 6f67 0103 0000 0034 0044 0061 0074  nLog.....4.D.a.t
+00002340: 0065 006e 0062 0061 006e 006b 0073 0074  .e.n.b.a.n.k.s.t
+00002350: 0072 0075 006b 0074 0075 0072 0020 0076  .r.u.k.t.u.r. .v
+00002360: 0065 0072 0061 006c 0074 0065 0074 0800  .e.r.a.l.t.e.t..
+00002370: 0000 0006 0000 001c 4461 7461 6261 7365  ........Database
+00002380: 2073 7472 7563 7475 7265 206f 7574 2d64   structure out-d
+00002390: 6174 6564 0700 0000 0944 7261 676f 6e4c  ated.....DragonL
+000023a0: 6f67 0103 0000 001e 0044 0061 0074 0075  og.......D.a.t.u
+000023b0: 006d 002f 005a 0065 0069 0074 0020 0045  .m./.Z.e.i.t. .E
+000023c0: 006e 0064 0065 0800 0000 0006 0000 000d  .n.d.e..........
+000023d0: 4461 7465 2f54 696d 6520 656e 6407 0000  Date/Time end...
+000023e0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+000023f0: 2000 4400 6100 7400 7500 6d00 2f00 5a00   .D.a.t.u.m./.Z.
+00002400: 6500 6900 7400 2000 5300 7400 6100 7200  e.i.t. .S.t.a.r.
+00002410: 7408 0000 0000 0600 0000 0f44 6174 652f  t..........Date/
+00002420: 5469 6d65 2073 7461 7274 0700 0000 0944  Time start.....D
+00002430: 7261 676f 6e4c 6f67 0103 0000 0016 0051  ragonLog.......Q
+00002440: 0053 004f 0020 006c 00f6 0073 0063 0068  .S.O. .l...s.c.h
+00002450: 0065 006e 0800 0000 0006 0000 000a 4465  .e.n..........De
+00002460: 6c65 7465 2051 534f 0700 0000 0944 7261  lete QSO.....Dra
+00002470: 676f 6e4c 6f67 0103 0000 0014 0045 006e  gonLog.......E.n
+00002480: 0074 0066 0065 0072 006e 0075 006e 0067  .t.f.e.r.n.u.n.g
+00002490: 0800 0000 0006 0000 0008 4469 7374 616e  ..........Distan
+000024a0: 6365 0700 0000 0944 7261 676f 6e4c 6f67  ce.....DragonLog
+000024b0: 0103 0000 0064 0057 006f 006c 006c 0065  .....d.W.o.l.l.e
+000024c0: 006e 0020 0073 0069 0065 0020 0064 0069  .n. .s.i.e. .d.i
+000024d0: 0065 0020 0073 0065 006c 0065 006b 0074  .e. .s.e.l.e.k.t
+000024e0: 0069 0065 0072 0074 0065 006e 0020 0051  .i.e.r.t.e.n. .Q
+000024f0: 0053 004f 0073 0020 0077 0069 0072 006b  .S.O.s. .w.i.r.k
+00002500: 006c 0069 0063 0068 0020 006c 00f6 0073  .l.i.c.h. .l...s
+00002510: 0063 0068 0065 006e 003f 0800 0000 0006  .c.h.e.n.?......
+00002520: 0000 0031 446f 2079 6f75 2072 6561 6c6c  ...1Do you reall
+00002530: 7920 7761 6e74 2074 6f20 6465 6c65 7465  y want to delete
+00002540: 2074 6865 2073 656c 6563 7465 6420 5153   the selected QS
+00002550: 4f28 7329 3f07 0000 0009 4472 6167 6f6e  O(s)?.....Dragon
+00002560: 4c6f 6701 03ff ffff ff08 0000 0000 0600  Log.............
+00002570: 0000 1045 6172 7468 2d4d 6f6f 6e2d 4561  ...Earth-Moon-Ea
+00002580: 7274 6807 0000 0009 4472 6167 6f6e 4c6f  rth.....DragonLo
+00002590: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+000025a0: 0845 6368 6f4c 696e 6b07 0000 0009 4472  .EchoLink.....Dr
+000025b0: 6167 6f6e 4c6f 6701 0300 0000 0c00 4600  agonLog.......F.
+000025c0: 6500 6800 6c00 6500 7208 0000 0000 0600  e.h.l.e.r.......
+000025d0: 0000 0545 7272 6f72 0700 0000 0944 7261  ...Error.....Dra
+000025e0: 676f 6e4c 6f67 0103 0000 0028 0045 0078  gonLog.....(.E.x
+000025f0: 0063 0065 006c 002d 0044 0061 0074 0065  .c.e.l.-.D.a.t.e
+00002600: 0069 0020 0028 002a 002e 0078 006c 0073  .i. .(.*...x.l.s
+00002610: 0078 0029 0800 0000 0006 0000 0013 4578  .x.)..........Ex
+00002620: 6365 6c2d 4669 6c65 2028 2a2e 786c 7378  cel-File (*.xlsx
+00002630: 2907 0000 0009 4472 6167 6f6e 4c6f 6701  ).....DragonLog.
+00002640: 0300 0000 2400 4500 7800 7000 6f00 7200  ....$.E.x.p.o.r.
+00002650: 7400 6900 6500 7200 6500 2000 5100 5300  t.i.e.r.e. .Q.S.
+00002660: 4f00 2000 6c00 6f00 6708 0000 0000 0600  O. .l.o.g.......
+00002670: 0000 1045 7870 6f72 7465 6420 5153 4f20  ...Exported QSO 
+00002680: 6c6f 6707 0000 0009 4472 6167 6f6e 4c6f  log.....DragonLo
+00002690: 6701 0300 0000 1a00 4600 3200 2d00 5200  g.......F.2.-.R.
+000026a0: 6500 6600 6c00 6500 6b00 7400 6900 6f00  e.f.l.e.k.t.i.o.
+000026b0: 6e08 0000 0000 0600 0000 0d46 3220 5265  n..........F2 Re
+000026c0: 666c 6563 7469 6f6e 0700 0000 0944 7261  flection.....Dra
+000026d0: 676f 6e4c 6f67 0103 0000 0038 0046 0069  gonLog.....8.F.i
+000026e0: 0065 006c 0064 002d 0041 006c 0069 0067  .e.l.d.-.A.l.i.g
+000026f0: 006e 0065 0064 002d 0049 0072 0072 0065  .n.e.d.-.I.r.r.e
+00002700: 0067 0075 006c 0061 0072 0069 0074 0069  .g.u.l.a.r.i.t.i
+00002710: 0065 0073 0800 0000 0006 0000 001c 4669  .e.s..........Fi
+00002720: 656c 6420 416c 6967 6e65 6420 4972 7265  eld Aligned Irre
+00002730: 6775 6c61 7269 7469 6573 0700 0000 0944  gularities.....D
+00002740: 7261 676f 6e4c 6f67 0103 0000 0010 0046  ragonLog.......F
+00002750: 0072 0065 0071 0075 0065 006e 007a 0800  .r.e.q.u.e.n.z..
+00002760: 0000 0006 0000 0009 4672 6571 7565 6e63  ........Frequenc
+00002770: 7907 0000 0009 4472 6167 6f6e 4c6f 6701  y.....DragonLog.
+00002780: 0300 0000 1400 4200 6f00 6400 6500 6e00  ......B.o.d.e.n.
+00002790: 7700 6500 6c00 6c00 6508 0000 0000 0600  w.e.l.l.e.......
+000027a0: 0000 0b47 726f 756e 6420 5761 7665 0700  ...Ground Wave..
+000027b0: 0000 0944 7261 676f 6e4c 6f67 0103 ffff  ...DragonLog....
+000027c0: ffff 0800 0000 0006 0000 0006 4861 6d51  ............HamQ
+000027d0: 5448 0700 0000 0944 7261 676f 6e4c 6f67  TH.....DragonLog
+000027e0: 0103 ffff ffff 0800 0000 0006 0000 0006  ................
+000027f0: 4861 6d6c 6962 0700 0000 0944 7261 676f  Hamlib.....Drago
+00002800: 6e4c 6f67 0103 0000 000a 0048 0069 006c  nLog.......H.i.l
+00002810: 0066 0065 0800 0000 0006 0000 0004 4865  .f.e..........He
+00002820: 6c70 0700 0000 0944 7261 676f 6e4c 6f67  lp.....DragonLog
+00002830: 0103 ffff ffff 0800 0000 0006 0000 0004  ................
+00002840: 4952 4c50 0700 0000 0944 7261 676f 6e4c  IRLP.....DragonL
+00002850: 6f67 0103 0000 0026 0049 006e 0074 0065  og.....&.I.n.t.e
+00002860: 0072 006e 0065 0074 0075 006e 0074 0065  .r.n.e.t.u.n.t.e
+00002870: 0072 0073 0074 00fc 0074 007a 0074 0800  .r.s.t...t.z.t..
+00002880: 0000 0006 0000 0011 496e 7465 726e 6574  ........Internet
+00002890: 2d61 7373 6973 7465 6407 0000 0009 4472  -assisted.....Dr
+000028a0: 6167 6f6e 4c6f 6701 0300 0000 1800 4900  agonLog.......I.
+000028b0: 6f00 6e00 6f00 2d00 5300 6300 6100 7400  o.n.o.-.S.c.a.t.
+000028c0: 7400 6500 7208 0000 0000 0600 0000 0b49  t.e.r..........I
+000028d0: 6f6e 6f73 6361 7474 6572 0700 0000 0944  onoscatter.....D
+000028e0: 7261 676f 6e4c 6f67 0103 0000 0020 006c  ragonLog..... .l
+000028f0: 0065 0074 007a 0074 0065 0073 0020 0048  .e.t.z.t.e.s. .H
+00002900: 0061 006c 0062 006a 0061 0068 0072 0800  .a.l.b.j.a.h.r..
+00002910: 0000 0006 0000 000e 4c61 7374 2068 616c  ........Last hal
+00002920: 6620 7965 6172 0700 0000 0944 7261 676f  f year.....Drago
+00002930: 6e4c 6f67 0103 0000 001a 006c 0065 0074  nLog.......l.e.t
+00002940: 007a 0074 0065 006e 0020 004d 006f 006e  .z.t.e.n. .M.o.n
+00002950: 0061 0074 0800 0000 0006 0000 000a 4c61  .a.t..........La
+00002960: 7374 206d 6f6e 7468 0700 0000 0944 7261  st month.....Dra
+00002970: 676f 6e4c 6f67 0103 0000 0018 006c 0065  gonLog.......l.e
+00002980: 0074 007a 0074 0065 0020 0057 006f 0063  .t.z.t.e. .W.o.c
+00002990: 0068 0065 0800 0000 0006 0000 0009 4c61  .h.e..........La
+000029a0: 7374 2077 6565 6b07 0000 0009 4472 6167  st week.....Drag
+000029b0: 6f6e 4c6f 6701 0300 0000 1800 6c00 6500  onLog.......l.e.
+000029c0: 7400 7a00 7400 6500 7300 2000 4a00 6100  t.z.t.e.s. .J.a.
+000029d0: 6800 7208 0000 0000 0600 0000 094c 6173  h.r..........Las
+000029e0: 7420 7965 6172 0700 0000 0944 7261 676f  t year.....Drago
+000029f0: 6e4c 6f67 0103 0000 001e 0053 0069 0063  nLog.......S.i.c
+00002a00: 0068 0074 0076 0065 0072 0062 0069 006e  .h.t.v.e.r.b.i.n
+00002a10: 0064 0075 006e 0067 0800 0000 0006 0000  .d.u.n.g........
+00002a20: 000d 4c69 6e65 206f 6620 5369 6768 7407  ..Line of Sight.
+00002a30: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00002a40: 0000 2000 4c00 6f00 5400 5700 2d00 4100  .. .L.o.T.W.-.A.
+00002a50: 4400 4900 4600 2d00 5500 7000 6c00 6f00  D.I.F.-.U.p.l.o.
+00002a60: 6100 6408 0000 0000 0600 0000 104c 6f54  a.d..........LoT
+00002a70: 5720 4144 4946 2075 706c 6f61 6407 0000  W ADIF upload...
+00002a80: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00002a90: 1400 4c00 6f00 5400 5700 2000 6500 6d00  ..L.o.T.W. .e.m.
+00002aa0: 7000 6600 2e08 0000 0000 0600 0000 094c  p.f............L
+00002ab0: 6f54 5720 7263 7664 0700 0000 0944 7261  oTW rcvd.....Dra
+00002ac0: 676f 6e4c 6f67 0103 0000 0014 004c 006f  gonLog.......L.o
+00002ad0: 0054 0057 0020 0076 0065 0072 0073 002e  .T.W. .v.e.r.s..
+00002ae0: 0800 0000 0006 0000 0009 4c6f 5457 2073  ..........LoTW s
+00002af0: 656e 7407 0000 0009 4472 6167 6f6e 4c6f  ent.....DragonLo
+00002b00: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00002b10: 074c 6f63 6174 6f72 0700 0000 0944 7261  .Locator.....Dra
+00002b20: 676f 6e4c 6f67 0103 ffff ffff 0800 0000  gonLog..........
+00002b30: 0006 0000 000f 4c6f 6720 696d 706f 7274  ......Log import
+00002b40: 2041 4449 4607 0000 0009 4472 6167 6f6e   ADIF.....Dragon
+00002b50: 4c6f 6701 0300 0000 1c00 4c00 6f00 6700  Log.......L.o.g.
+00002b60: 2000 4900 6d00 7000 6f00 7200 7400 2000   .I.m.p.o.r.t. .
+00002b70: 4300 5300 5608 0000 0000 0600 0000 0e4c  C.S.V..........L
+00002b80: 6f67 2069 6d70 6f72 7420 4353 5607 0000  og import CSV...
+00002b90: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00002ba0: 2000 4c00 6f00 6700 2000 4900 6d00 7000   .L.o.g. .I.m.p.
+00002bb0: 6f00 7200 7400 2000 4500 7800 6300 6500  o.r.t. .E.x.c.e.
+00002bc0: 6c08 0000 0000 0600 0000 104c 6f67 2069  l..........Log i
+00002bd0: 6d70 6f72 7420 4578 6365 6c07 0000 0009  mport Excel.....
+00002be0: 4472 6167 6f6e 4c6f 6701 0300 0000 1c00  DragonLog.......
+00002bf0: 4d00 6500 7400 6500 6f00 7200 2d00 5300  M.e.t.e.o.r.-.S.
+00002c00: 6300 6100 7400 7400 6500 7208 0000 0000  c.a.t.t.e.r.....
+00002c10: 0600 0000 0e4d 6574 656f 7220 7363 6174  .....Meteor scat
+00002c20: 7465 7207 0000 0009 4472 6167 6f6e 4c6f  ter.....DragonLo
+00002c30: 6701 0300 0000 5a00 4b00 6500 6900 6e00  g.....Z.K.e.i.n.
+00002c40: 6500 2000 5300 7400 6100 7400 6900 6f00  e. .S.t.a.t.i.o.
+00002c50: 6e00 7300 6b00 6f00 6e00 6600 6900 6700  n.s.k.o.n.f.i.g.
+00002c60: 7500 7200 6100 7400 6900 6f00 6e00 2000  u.r.a.t.i.o.n. .
+00002c70: 6900 6e00 2000 5400 5100 5300 4c00 2000  i.n. .T.Q.S.L. .
+00002c80: 7600 6500 7200 6600 fc00 6700 6200 6100  v.e.r.f...g.b.a.
+00002c90: 7208 0000 0000 0600 0000 254d 6973 7369  r.........%Missi
+00002ca0: 6e67 2073 7461 7469 6f6e 2063 6f6e 6669  ng station confi
+00002cb0: 6775 7261 7469 6f6e 2069 6e20 5451 534c  guration in TQSL
+00002cc0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00002cd0: ffff ffff 0800 0000 0006 0000 0004 4d6f  ..............Mo
+00002ce0: 6465 0700 0000 0944 7261 676f 6e4c 6f67  de.....DragonLog
+00002cf0: 0103 ffff ffff 0800 0000 0006 0000 0004  ................
+00002d00: 4e61 6d65 0700 0000 0944 7261 676f 6e4c  Name.....DragonL
+00002d10: 6f67 0103 0000 0034 004b 0065 0069 006e  og.....4.K.e.i.n
+00002d20: 0065 0020 0051 0053 004f 0073 0020 0066  .e. .Q.S.O.s. .f
+00002d30: 00fc 0072 0020 0064 0065 006e 0020 004c  ...r. .d.e.n. .L
+00002d40: 006f 0063 0061 0074 006f 0072 0800 0000  .o.c.a.t.o.r....
+00002d50: 0006 0000 0017 4e6f 2072 6563 6f72 6473  ......No records
+00002d60: 2066 6f72 206c 6f63 6174 696f 6e07 0000   for location...
+00002d70: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00002d80: 0e00 4e00 6f00 7400 6900 7a00 6500 6e08  ..N.o.t.i.z.e.n.
+00002d90: 0000 0000 0600 0000 054e 6f74 6573 0700  .........Notes..
+00002da0: 0000 0944 7261 676f 6e4c 6f67 0103 ffff  ...DragonLog....
+00002db0: ffff 0800 0000 0006 0000 0002 4f6b 0700  ............Ok..
+00002dc0: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00002dd0: 001e 0045 0069 0067 0065 006e 0065 0072  ...E.i.g.e.n.e.r
+00002de0: 0020 004c 006f 0063 0061 0074 006f 0072  . .L.o.c.a.t.o.r
+00002df0: 0800 0000 0006 0000 000b 4f77 6e20 4c6f  ..........Own Lo
+00002e00: 6361 746f 7207 0000 0009 4472 6167 6f6e  cator.....Dragon
+00002e10: 4c6f 6701 0300 0000 1800 4500 6900 6700  Log.......E.i.g.
+00002e20: 6500 6e00 6500 7200 2000 4e00 6100 6d00  e.n.e.r. .N.a.m.
+00002e30: 6508 0000 0000 0600 0000 084f 776e 204e  e..........Own N
+00002e40: 616d 6507 0000 0009 4472 6167 6f6e 4c6f  ame.....DragonLo
+00002e50: 6701 0300 0000 1600 4500 6900 6700 6500  g.......E.i.g.e.
+00002e60: 6e00 6500 7200 2000 5100 5400 4808 0000  n.e.r. .Q.T.H...
+00002e70: 0000 0600 0000 074f 776e 2051 5448 0700  .......Own QTH..
+00002e80: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00002e90: 0024 0045 0069 0067 0065 006e 0065 0073  .$.E.i.g.e.n.e.s
+00002ea0: 0020 0052 0075 0066 007a 0065 0069 0063  . .R.u.f.z.e.i.c
+00002eb0: 0068 0065 006e 0800 0000 0006 0000 000d  .h.e.n..........
+00002ec0: 4f77 6e20 6361 6c6c 2073 6967 6e07 0000  Own call sign...
+00002ed0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00002ee0: 1000 4c00 6500 6900 7300 7400 7500 6e00  ..L.e.i.s.t.u.n.
+00002ef0: 6708 0000 0000 0600 0000 0550 6f77 6572  g..........Power
+00002f00: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00002f10: 0000 0016 0041 0075 0073 0062 0072 0065  .....A.u.s.b.r.e
+00002f20: 0069 0074 0075 006e 0067 0800 0000 0006  .i.t.u.n.g......
+00002f30: 0000 000b 5072 6f70 6167 6174 696f 6e07  ....Propagation.
+00002f40: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00002f50: 0000 1a00 5100 5300 4c00 2d00 4e00 6100  ....Q.S.L.-.N.a.
+00002f60: 6300 6800 7200 6900 6300 6800 7408 0000  c.h.r.i.c.h.t...
+00002f70: 0000 0600 0000 0b51 534c 206d 6573 7361  .......QSL messa
+00002f80: 6765 0700 0000 0944 7261 676f 6e4c 6f67  ge.....DragonLog
+00002f90: 0103 0000 0010 0051 0053 004c 002d 0050  .......Q.S.L.-.P
+00002fa0: 0066 0061 0064 0800 0000 0006 0000 0008  .f.a.d..........
+00002fb0: 5153 4c20 7061 7468 0700 0000 0944 7261  QSL path.....Dra
+00002fc0: 676f 6e4c 6f67 0103 0000 0012 0051 0053  gonLog.......Q.S
+00002fd0: 004c 0020 0065 006d 0070 0066 002e 0800  .L. .e.m.p.f....
+00002fe0: 0000 0006 0000 0008 5153 4c20 7263 7664  ........QSL rcvd
+00002ff0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00003000: 0000 0012 0051 0053 004c 0020 0076 0065  .....Q.S.L. .v.e
+00003010: 0072 0073 002e 0800 0000 0006 0000 0008  .r.s............
+00003020: 5153 4c20 7365 6e74 0700 0000 0944 7261  QSL sent.....Dra
+00003030: 676f 6e4c 6f67 0103 0000 000e 0051 0053  gonLog.......Q.S
+00003040: 004c 002d 0056 0069 0061 0800 0000 0006  .L.-.V.i.a......
+00003050: 0000 0007 5153 4c20 7669 6107 0000 0009  ....QSL via.....
+00003060: 4472 6167 6f6e 4c6f 6701 03ff ffff ff08  DragonLog.......
+00003070: 0000 0000 0600 0000 0351 534f 0700 0000  .........QSO....
+00003080: 0944 7261 676f 6e4c 6f67 0103 0000 0048  .DragonLog.....H
+00003090: 0051 0053 004f 002d 004c 006f 0067 0020  .Q.S.O.-.L.o.g. 
+000030a0: 0028 002a 002e 0071 006c 006f 0067 0029  .(.*...q.l.o.g.)
+000030b0: 003b 003b 0041 006c 006c 0065 0020 0044  .;.;.A.l.l.e. .D
+000030c0: 0061 0074 0065 0069 0065 006e 0020 0028  .a.t.e.i.e.n. .(
+000030d0: 002a 002e 002a 0029 0800 0000 0006 0000  .*...*.)........
+000030e0: 0021 5153 4f2d 4c6f 6720 282a 2e71 6c6f  .!QSO-Log (*.qlo
+000030f0: 6729 3b3b 416c 6c20 4669 6c65 7320 282a  g);;All Files (*
+00003100: 2e2a 2907 0000 0009 4472 6167 6f6e 4c6f  .*).....DragonLo
+00003110: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00003120: 0351 5448 0700 0000 0944 7261 676f 6e4c  .QTH.....DragonL
+00003130: 6f67 0103 0000 0012 0052 0053 0054 0020  og.......R.S.T. 
+00003140: 0065 006d 0070 0066 002e 0800 0000 0006  .e.m.p.f........
+00003150: 0000 0008 5253 5420 7263 7664 0700 0000  ....RST rcvd....
+00003160: 0944 7261 676f 6e4c 6f67 0103 0000 0010  .DragonLog......
+00003170: 0052 0053 0054 0020 0067 0065 0073 002e  .R.S.T. .g.e.s..
+00003180: 0800 0000 0006 0000 0008 5253 5420 7365  ..........RST se
+00003190: 6e74 0700 0000 0944 7261 676f 6e4c 6f67  nt.....DragonLog
+000031a0: 0103 ffff ffff 0800 0000 0006 0000 0005  ................
+000031b0: 5261 6469 6f07 0000 0009 4472 6167 6f6e  Radio.....Dragon
+000031c0: 4c6f 6701 0300 0000 1800 5200 6100 6900  Log.......R.a.i.
+000031d0: 6e00 2d00 5300 6300 6100 7400 7400 6500  n.-.S.c.a.t.t.e.
+000031e0: 7208 0000 0000 0600 0000 0c52 6169 6e20  r..........Rain 
+000031f0: 7363 6174 7465 7207 0000 0009 4472 6167  scatter.....Drag
+00003200: 6f6e 4c6f 6701 0300 0000 3200 5200 6500  onLog.....2.R.e.
+00003210: 7000 6500 6100 7400 6500 7200 2000 6f00  p.e.a.t.e.r. .o.
+00003220: 6400 6500 7200 2000 5400 7200 6100 6e00  d.e.r. .T.r.a.n.
+00003230: 7300 7000 6f00 6e00 6400 6500 7208 0000  s.p.o.n.d.e.r...
+00003240: 0000 0600 0000 1752 6570 6561 7465 7220  .......Repeater 
+00003250: 6f72 2054 7261 6e73 706f 6e64 6572 0700  or Transponder..
+00003260: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00003270: 0010 0053 0061 0074 0065 006c 006c 0069  ...S.a.t.e.l.l.i
+00003280: 0074 0800 0000 0006 0000 0009 5361 7465  .t..........Sate
+00003290: 6c6c 6974 6507 0000 0009 4472 6167 6f6e  llite.....Dragon
+000032a0: 4c6f 6701 0300 0000 2a00 4500 7800 7000  Log.....*.E.x.p.
+000032b0: 6f00 7200 7400 6400 6100 7400 6500 6900  o.r.t.d.a.t.e.i.
+000032c0: 2000 7300 7000 6500 6900 6300 6800 6500   .s.p.e.i.c.h.e.
+000032d0: 7200 6e08 0000 0000 0600 0000 1253 656c  r.n..........Sel
+000032e0: 6563 7420 6578 706f 7274 2066 696c 6507  ect export file.
+000032f0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00003300: 0000 2000 4400 6100 7400 6500 6e00 6200  .. .D.a.t.e.n.b.
+00003310: 6100 6e00 6b00 2000 f600 6600 6600 6e00  a.n.k. ...f.f.n.
+00003320: 6500 6e08 0000 0000 0600 0000 0b53 656c  e.n..........Sel
+00003330: 6563 7420 6669 6c65 0700 0000 0944 7261  ect file.....Dra
+00003340: 676f 6e4c 6f67 0103 0000 0038 005a 0075  gonLog.....8.Z.u
+00003350: 0020 00fc 0062 0065 0072 0077 0061 0063  . ...b.e.r.w.a.c
+00003360: 0068 0065 006e 0064 0065 0020 0044 0061  .h.e.n.d.e. .D.a
+00003370: 0074 0065 0069 0020 0077 00e4 0068 006c  .t.e.i. .w...h.l
+00003380: 0065 006e 0800 0000 0006 0000 0014 5365  .e.n..........Se
+00003390: 6c65 6374 2066 696c 6520 746f 2077 6174  lect file to wat
+000033a0: 6368 0700 0000 0944 7261 676f 6e4c 6f67  ch.....DragonLog
+000033b0: 0103 0000 0024 0049 006d 0070 006f 0072  .....$.I.m.p.o.r
+000033c0: 0074 0064 0061 0074 0065 0069 0020 00f6  .t.d.a.t.e.i. ..
+000033d0: 0066 0066 006e 0065 006e 0800 0000 0006  .f.f.n.e.n......
+000033e0: 0000 0012 5365 6c65 6374 2069 6d70 6f72  ....Select impor
+000033f0: 7420 6669 6c65 0700 0000 0944 7261 676f  t file.....Drago
+00003400: 6e4c 6f67 0103 0000 001a 0057 00e4 0068  nLog.......W...h
+00003410: 006c 0065 0020 0053 0074 0061 0074 0069  .l.e. .S.t.a.t.i
+00003420: 006f 006e 0800 0000 0006 0000 000e 5365  .o.n..........Se
+00003430: 6c65 6374 2073 7461 7469 6f6e 0700 0000  lect station....
+00003440: 0944 7261 676f 6e4c 6f67 0103 0000 0044  .DragonLog.....D
+00003450: 004c 006f 0054 0057 002d 0053 0065 0072  .L.o.T.W.-.S.e.r
+00003460: 0076 0065 0072 0020 0068 0061 0074 0020  .v.e.r. .h.a.t. 
+00003470: 0064 0061 0073 0020 004c 006f 0067 0020  .d.a.s. .L.o.g. 
+00003480: 0061 0062 0067 0065 0077 0069 0065 0073  .a.b.g.e.w.i.e.s
+00003490: 0065 006e 0800 0000 0006 0000 0013 5365  .e.n..........Se
+000034a0: 7276 6572 2072 656a 6563 7465 6420 6c6f  rver rejected lo
+000034b0: 6707 0000 0009 4472 6167 6f6e 4c6f 6701  g.....DragonLog.
+000034c0: 0300 0000 1400 7a00 6500 6900 6700 6500  ......z.e.i.g.e.
+000034d0: 2000 6100 6c00 6c00 6508 0000 0000 0600   .a.l.l.e.......
+000034e0: 0000 0853 686f 7720 616c 6c07 0000 0009  ...Show all.....
+000034f0: 4472 6167 6f6e 4c6f 6701 0300 0000 1400  DragonLog.......
+00003500: 5300 7000 6f00 7200 6100 6400 6900 6300  S.p.o.r.a.d.i.c.
+00003510: 2d00 4508 0000 0000 0600 0000 0a53 706f  -.E..........Spo
+00003520: 7261 6469 6320 4507 0000 0009 4472 6167  radic E.....Drag
+00003530: 6f6e 4c6f 6701 03ff ffff ff08 0000 0000  onLog...........
+00003540: 0600 0000 0753 7562 6d6f 6465 0700 0000  .....Submode....
+00003550: 0944 7261 676f 6e4c 6f67 0103 0000 002a  .DragonLog.....*
+00003560: 0054 0051 0053 004c 002d 0053 0069 0067  .T.Q.S.L.-.S.i.g
+00003570: 006e 0061 0074 0075 0072 0070 0061 0073  .n.a.t.u.r.p.a.s
+00003580: 0073 0077 006f 0072 0074 0800 0000 0006  .s.w.o.r.t......
+00003590: 0000 0017 5451 534c 2073 6967 6e61 7475  ....TQSL signatu
+000035a0: 7265 2070 6173 7377 6f72 6407 0000 0009  re password.....
+000035b0: 4472 6167 6f6e 4c6f 6701 0300 0000 b200  DragonLog.......
+000035c0: 4400 6900 6500 2000 4400 6100 7400 6500  D.i.e. .D.a.t.e.
+000035d0: 6e00 6200 6100 6e00 6b00 7300 7400 7200  n.b.a.n.k.s.t.r.
+000035e0: 7500 6b00 7400 7500 7200 2000 6900 7300  u.k.t.u.r. .i.s.
+000035f0: 7400 2000 7600 6500 7200 6100 6c00 7400  t. .v.e.r.a.l.t.
+00003600: 6500 7400 2000 7500 6e00 6400 2000 6d00  e.t. .u.n.d. .m.
+00003610: 7500 7300 7300 2000 6b00 6f00 6e00 7600  u.s.s. .k.o.n.v.
+00003620: 6500 7200 7400 6900 6500 7200 7400 2000  e.r.t.i.e.r.t. .
+00003630: 7700 6500 7200 6400 6500 6e00 0a00 0a00  w.e.r.d.e.n.....
+00003640: 4500 6900 6e00 2000 4200 6100 6300 6b00  E.i.n. .B.a.c.k.
+00003650: 7500 7000 2000 7700 6900 7200 6400 2000  u.p. .w.i.r.d. .
+00003660: 6500 7200 7300 7400 6500 6c00 6c00 7400  e.r.s.t.e.l.l.t.
+00003670: 3a08 0000 0000 0600 0000 5754 6865 2064  :.........WThe d
+00003680: 6174 6162 6173 6520 7374 7275 6374 7572  atabase structur
+00003690: 6520 6973 206f 7574 2d64 6174 6564 2061  e is out-dated a
+000036a0: 6e64 206e 6565 6473 2061 2063 6f6e 7665  nd needs a conve
+000036b0: 7273 696f 6e0a 0a41 2062 6163 6b75 7020  rsion..A backup 
+000036c0: 7769 6c6c 2062 6520 6765 6e65 7261 7465  will be generate
+000036d0: 643a 0700 0000 0944 7261 676f 6e4c 6f67  d:.....DragonLog
+000036e0: 0103 0000 001e 0054 0072 0061 006e 0073  .......T.r.a.n.s
+000036f0: 0065 0071 0075 0061 0074 006f 0072 0069  .e.q.u.a.t.o.r.i
+00003700: 0061 006c 0800 0000 0006 0000 0010 5472  .a.l..........Tr
+00003710: 616e 732d 6571 7561 746f 7269 616c 0700  ans-equatorial..
+00003720: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00003730: 0028 0054 0072 006f 0070 006f 0073 0070  .(.T.r.o.p.o.s.p
+00003740: 0068 0065 0072 0069 0063 002d 0044 0075  .h.e.r.i.c.-.D.u
+00003750: 0063 0074 0069 006e 0067 0800 0000 0006  .c.t.i.n.g......
+00003760: 0000 0014 5472 6f70 6f73 7068 6572 6963  ....Tropospheric
+00003770: 2064 7563 7469 6e67 0700 0000 0944 7261   ducting.....Dra
+00003780: 676f 6e4c 6f67 0103 ffff ffff 0800 0000  gonLog..........
+00003790: 0006 0000 0007 5665 7273 696f 6e07 0000  ......Version...
+000037a0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+000037b0: 2c00 5000 7200 6f00 6700 7200 6100 6d00  ,.P.r.o.g.r.a.m.
+000037c0: 6d00 6c00 6f00 6700 2000 fc00 6200 6500  m.l.o.g. ...b.e.
+000037d0: 7200 7700 6100 6300 6800 6500 6e08 0000  r.w.a.c.h.e.n...
+000037e0: 0000 0600 0000 1557 6174 6368 2061 7070  .......Watch app
+000037f0: 6c69 6361 7469 6f6e 206c 6f67 0700 0000  lication log....
+00003800: 0944 7261 676f 6e4c 6f67 0103 0000 0020  .DragonLog..... 
+00003810: 0044 0061 0074 0065 0069 00fc 0062 0065  .D.a.t.e.i...b.e
+00003820: 0072 0077 0061 0063 0068 0075 006e 0067  .r.w.a.c.h.u.n.g
+00003830: 0800 0000 0006 0000 000d 5761 7463 6869  ..........Watchi
+00003840: 6e67 2066 696c 6507 0000 0009 4472 6167  ng file.....Drag
+00003850: 6f6e 4c6f 6701 0300 0000 1400 6500 5100  onLog.......e.Q.
+00003860: 5300 4c00 2000 6500 6d00 7000 6600 2e08  S.L. .e.m.p.f...
+00003870: 0000 0000 0600 0000 0965 5153 4c20 7263  .........eQSL rc
+00003880: 7664 0700 0000 0944 7261 676f 6e4c 6f67  vd.....DragonLog
+00003890: 0103 0000 0014 0065 0051 0053 004c 0020  .......e.Q.S.L. 
+000038a0: 0076 0065 0072 0073 002e 0800 0000 0006  .v.e.r.s........
+000038b0: 0000 0009 6551 534c 2073 656e 7407 0000  ....eQSL sent...
+000038c0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+000038d0: 0e00 6900 6e00 6100 6b00 7400 6900 7608  ..i.n.a.k.t.i.v.
+000038e0: 0000 0000 0600 0000 0769 6e61 6374 6976  .........inactiv
+000038f0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00003900: 0000 0008 00dc 0062 0065 0072 0800 0000  .......b.e.r....
+00003910: 0006 0000 0005 4162 6f75 7407 0000 000a  ......About.....
+00003920: 4d61 696e 5769 6e64 6f77 0103 0000 000e  MainWindow......
+00003930: 00dc 0062 0065 0072 0020 0051 0074 0800  ...b.e.r. .Q.t..
+00003940: 0000 0006 0000 0008 4162 6f75 7420 5174  ........About Qt
+00003950: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+00003960: 0300 0000 1a00 4100 6e00 7700 6500 6e00  ......A.n.w.e.n.
+00003970: 6400 7500 6e00 6700 7300 6c00 6f00 6708  d.u.n.g.s.l.o.g.
+00003980: 0000 0000 0600 0000 0f41 7070 6c69 6361  .........Applica
+00003990: 7469 6f6e 204c 6f67 0700 0000 0a4d 6169  tion Log.....Mai
+000039a0: 6e57 696e 646f 7701 0300 0000 2200 4500  nWindow.....".E.
+000039b0: 6900 6e00 7400 7200 6100 6700 2000 e400  i.n.t.r.a.g. ...
+000039c0: 6e00 6400 6500 7200 6e00 2e00 2e00 2e08  n.d.e.r.n.......
+000039d0: 0000 0000 0600 0000 1343 6861 6e67 6520  .........Change 
+000039e0: 6c6f 6720 656e 7472 792e 2e2e 0700 0000  log entry.......
+000039f0: 0a4d 6169 6e57 696e 646f 7701 03ff ffff  .MainWindow.....
+00003a00: ff08 0000 0000 0600 0000 0643 7472 6c2b  ...........Ctrl+
+00003a10: 4507 0000 000a 4d61 696e 5769 6e64 6f77  E.....MainWindow
+00003a20: 0103 ffff ffff 0800 0000 0006 0000 0006  ................
+00003a30: 4374 726c 2b4c 0700 0000 0a4d 6169 6e57  Ctrl+L.....MainW
+00003a40: 696e 646f 7701 03ff ffff ff08 0000 0000  indow...........
+00003a50: 0600 0000 0643 7472 6c2b 5107 0000 000a  .....Ctrl+Q.....
+00003a60: 4d61 696e 5769 6e64 6f77 0103 ffff ffff  MainWindow......
+00003a70: 0800 0000 0006 0000 0006 4374 726c 2b57  ..........Ctrl+W
+00003a80: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+00003a90: 03ff ffff ff08 0000 0000 0600 0000 0643  ...............C
+00003aa0: 7472 6c2b 5807 0000 000a 4d61 696e 5769  trl+X.....MainWi
+00003ab0: 6e64 6f77 0103 0000 001e 0045 0069 006e  ndow.......E.i.n
+00003ac0: 0074 0072 0061 0067 0020 006c 00f6 0073  .t.r.a.g. .l...s
+00003ad0: 0063 0068 0065 006e 0800 0000 0006 0000  .c.h.e.n........
+00003ae0: 0010 4465 6c65 7465 206c 6f67 2065 6e74  ..Delete log ent
+00003af0: 7279 0700 0000 0a4d 6169 6e57 696e 646f  ry.....MainWindo
+00003b00: 7701 03ff ffff ff08 0000 0000 0600 0000  w...............
+00003b10: 0944 7261 676f 6e4c 6f67 0700 0000 0a4d  .DragonLog.....M
+00003b20: 6169 6e57 696e 646f 7701 0300 0000 1400  ainWindow.......
+00003b30: 4200 6500 6100 7200 6200 6500 6900 7400  B.e.a.r.b.e.i.t.
+00003b40: 6500 6e08 0000 0000 0600 0000 0445 6469  e.n..........Edi
+00003b50: 7407 0000 000a 4d61 696e 5769 6e64 6f77  t.....MainWindow
+00003b60: 0103 0000 000e 0042 0065 0065 006e 0064  .......B.e.e.n.d
+00003b70: 0065 006e 0800 0000 0006 0000 0004 4578  .e.n..........Ex
+00003b80: 6974 0700 0000 0a4d 6169 6e57 696e 646f  it.....MainWindo
+00003b90: 7701 03ff ffff ff08 0000 0000 0600 0000  w...............
+00003ba0: 0645 7870 6f72 7407 0000 000a 4d61 696e  .Export.....Main
+00003bb0: 5769 6e64 6f77 0103 0000 001c 0045 0078  Window.......E.x
+00003bc0: 0070 006f 0072 0074 0069 0065 0072 0065  .p.o.r.t.i.e.r.e
+00003bd0: 006e 002e 002e 002e 0800 0000 0006 0000  .n..............
+00003be0: 0009 4578 706f 7274 2e2e 2e07 0000 000a  ..Export........
+00003bf0: 4d61 696e 5769 6e64 6f77 0103 0000 000a  MainWindow......
+00003c00: 0044 0061 0074 0065 0069 0800 0000 0006  .D.a.t.e.i......
+00003c10: 0000 0004 4669 6c65 0700 0000 0a4d 6169  ....File.....Mai
+00003c20: 6e57 696e 646f 7701 0300 0000 0a00 4800  nWindow.......H.
+00003c30: 6900 6c00 6600 6508 0000 0000 0600 0000  i.l.f.e.........
+00003c40: 0448 656c 7007 0000 000a 4d61 696e 5769  .Help.....MainWi
+00003c50: 6e64 6f77 0103 ffff ffff 0800 0000 0006  ndow............
+00003c60: 0000 0006 496d 706f 7274 0700 0000 0a4d  ....Import.....M
+00003c70: 6169 6e57 696e 646f 7701 0300 0000 1c00  ainWindow.......
+00003c80: 4900 6d00 7000 6f00 7200 7400 6900 6500  I.m.p.o.r.t.i.e.
+00003c90: 7200 6500 6e00 2e00 2e00 2e08 0000 0000  r.e.n...........
+00003ca0: 0600 0000 0949 6d70 6f72 742e 2e2e 0700  .....Import.....
+00003cb0: 0000 0a4d 6169 6e57 696e 646f 7701 0300  ...MainWindow...
+00003cc0: 0000 1800 4c00 6f00 6700 6700 6500 2000  ....L.o.g.g.e. .
+00003cd0: 5100 5300 4f00 2e00 2e00 2e08 0000 0000  Q.S.O...........
+00003ce0: 0600 0000 0a4c 6f67 2051 534f 2e2e 2e07  .....Log QSO....
+00003cf0: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
+00003d00: 0000 0018 0051 0053 004f 002d 0046 006f  .....Q.S.O.-.F.o
+00003d10: 0072 006d 0075 006c 0061 0072 0800 0000  .r.m.u.l.a.r....
+00003d20: 0006 0000 0008 5153 4f20 466f 726d 0700  ......QSO Form..
+00003d30: 0000 0a4d 6169 6e57 696e 646f 7701 0300  ...MainWindow...
+00003d40: 0000 2600 4400 6100 7400 6500 6e00 6200  ..&.D.a.t.e.n.b.
+00003d50: 6100 6e00 6b00 2000 7700 e400 6800 6c00  a.n.k. .w...h.l.
+00003d60: 6500 6e00 2e00 2e00 2e08 0000 0000 0600  e.n.............
+00003d70: 0000 1253 656c 6563 7420 6461 7461 6261  ...Select databa
+00003d80: 7365 2e2e 2e07 0000 000a 4d61 696e 5769  se........MainWi
+00003d90: 6e64 6f77 0103 0000 001a 0045 0069 006e  ndow.......E.i.n
+00003da0: 0073 0074 0065 006c 006c 0075 006e 0067  .s.t.e.l.l.u.n.g
+00003db0: 0065 006e 0800 0000 0006 0000 0008 5365  .e.n..........Se
+00003dc0: 7474 696e 6773 0700 0000 0a4d 6169 6e57  ttings.....MainW
+00003dd0: 696e 646f 7701 0300 0000 2600 5a00 6500  indow.....&.Z.e.
+00003de0: 6900 6700 6500 2000 4100 6e00 7700 6500  i.g.e. .A.n.w.e.
+00003df0: 6e00 6400 7500 6e00 6700 7300 6c00 6f00  n.d.u.n.g.s.l.o.
+00003e00: 6708 0000 0000 0600 0000 0853 686f 7720  g..........Show 
+00003e10: 6c6f 6707 0000 000a 4d61 696e 5769 6e64  log.....MainWind
+00003e20: 6f77 0103 0000 001a 0053 0074 0061 0072  ow.......S.t.a.r
+00003e30: 0074 0065 0020 0048 0061 006d 006c 0069  .t.e. .H.a.m.l.i
+00003e40: 0062 0800 0000 0006 0000 000c 5374 6172  .b..........Star
+00003e50: 7420 6861 6d6c 6962 0700 0000 0a4d 6169  t hamlib.....Mai
+00003e60: 6e57 696e 646f 7701 0300 0000 1c00 5700  nWindow.......W.
+00003e70: 6500 7200 6b00 7a00 6500 7500 6700 6c00  e.r.k.z.e.u.g.l.
+00003e80: 6500 6900 7300 7400 6508 0000 0000 0600  e.i.s.t.e.......
+00003e90: 0000 0754 6f6f 6c62 6172 0700 0000 0a4d  ...Toolbar.....M
+00003ea0: 6169 6e57 696e 646f 7701 0300 0000 3200  ainWindow.....2.
+00003eb0: 4c00 6f00 6700 7300 2000 7a00 7500 2000  L.o.g.s. .z.u. .
+00003ec0: 4c00 6f00 5400 5700 2000 6800 6f00 6300  L.o.T.W. .h.o.c.
+00003ed0: 6800 6c00 6100 6400 6500 6e00 2e00 2e00  h.l.a.d.e.n.....
+00003ee0: 2e08 0000 0000 0600 0000 1655 706c 6f61  ...........Uploa
+00003ef0: 6420 6c6f 6773 2074 6f20 4c6f 5457 2e2e  d logs to LoTW..
+00003f00: 2e07 0000 000a 4d61 696e 5769 6e64 6f77  ......MainWindow
+00003f10: 0103 0000 0042 0044 0061 0074 0065 0069  .....B.D.a.t.e.i
+00003f20: 0020 0061 0075 0066 0020 006e 0065 0075  . .a.u.f. .n.e.u
+00003f30: 0065 0020 0051 0053 004f 0073 0020 00fc  .e. .Q.S.O.s. ..
+00003f40: 0062 0065 0072 0077 0061 0063 0068 0065  .b.e.r.w.a.c.h.e
+00003f50: 006e 002e 002e 002e 0800 0000 0006 0000  .n..............
+00003f60: 0016 5761 7463 6820 6669 6c65 2066 6f72  ..Watch file for
+00003f70: 2051 534f 732e 2e2e 0700 0000 0a4d 6169   QSOs........Mai
+00003f80: 6e57 696e 646f 7701 03ff ffff ff08 0000  nWindow.........
+00003f90: 0000 0600 0000 0220 5707 0000 0007 5153  ....... W.....QS
+00003fa0: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
+00003fb0: 0600 0000 0420 6b48 7a07 0000 0007 5153  ..... kHz.....QS
+00003fc0: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
+00003fd0: 0600 0000 0235 3907 0000 0007 5153 4f46  .....59.....QSOF
+00003fe0: 6f72 6d01 0300 0000 4800 4500 6900 6e00  orm.....H.E.i.n.
+00003ff0: 2000 4600 6500 6c00 6400 2000 6600 6500   .F.e.l.d. .f.e.
+00004000: 6800 6c00 7400 2000 6600 fc00 7200 2000  h.l.t. .f...r. .
+00004010: 6400 6900 6500 2000 4900 6e00 6200 6f00  d.i.e. .I.n.b.o.
+00004020: 7800 2d00 5000 7200 fc00 6600 7500 6e00  x.-.P.r...f.u.n.
+00004030: 6708 0000 0000 0600 0000 2241 2066 6965  g........."A fie
+00004040: 6c64 2069 7320 6d69 7373 696e 6720 666f  ld is missing fo
+00004050: 7220 696e 626f 7820 6368 6563 6b07 0000  r inbox check...
+00004060: 0007 5153 4f46 6f72 6d01 0300 0000 4200  ..QSOForm.....B.
+00004070: 4600 6500 6800 6c00 6500 6e00 6400 6500  F.e.h.l.e.n.d.e.
+00004080: 7300 2000 4600 6500 6c00 6400 2000 6600  s. .F.e.l.d. .f.
+00004090: fc00 7200 2000 6400 6500 6e00 2000 4c00  ..r. .d.e.n. .L.
+000040a0: 6f00 6700 2d00 5500 7000 6c00 6f00 6100  o.g.-.U.p.l.o.a.
+000040b0: 6408 0000 0000 0600 0000 2141 2066 6965  d.........!A fie
+000040c0: 6c64 2069 7320 6d69 7373 696e 6720 666f  ld is missing fo
+000040d0: 7220 6c6f 6720 7570 6c6f 6164 0700 0000  r log upload....
+000040e0: 0751 534f 466f 726d 0103 0000 0056 0046  .QSOForm.....V.F
+000040f0: 0065 0068 006c 0065 006e 0064 0065 0073  .e.h.l.e.n.d.e.s
+00004100: 0020 0046 0065 006c 0064 0020 0066 00fc  . .F.e.l.d. .f..
+00004110: 0072 0020 0064 0065 006e 0020 004c 006f  .r. .d.e.n. .L.o
+00004120: 0067 002d 0055 0070 006c 006f 0061 0064  .g.-.U.p.l.o.a.d
+00004130: 0020 007a 0075 0020 0048 0061 006d 0051  . .z.u. .H.a.m.Q
+00004140: 0054 0048 0800 0000 0006 0000 002b 4120  .T.H.........+A 
+00004150: 6669 656c 6420 6973 206d 6973 7369 6e67  field is missing
+00004160: 2066 6f72 206c 6f67 2075 706c 6f61 6420   for log upload 
+00004170: 746f 2048 616d 5154 4807 0000 0007 5153  to HamQTH.....QS
+00004180: 4f46 6f72 6d01 0300 0000 1600 4100 6b00  OForm.......A.k.
+00004190: 7a00 6500 7000 7400 6900 6500 7200 7400  z.e.p.t.i.e.r.t.
+000041a0: 3a08 0000 0000 0600 0000 0841 6363 6570  :..........Accep
+000041b0: 7473 3a07 0000 0007 5153 4f46 6f72 6d01  ts:.....QSOForm.
+000041c0: 0300 0000 6a00 4500 6900 6e00 2000 4600  ....j.E.i.n. .F.
+000041d0: 6500 6800 6c00 6500 7200 2000 7400 7200  e.h.l.e.r. .t.r.
+000041e0: 6100 7400 2000 7700 e400 6800 7200 6500  a.t. .w...h.r.e.
+000041f0: 6e00 6400 2000 6400 6500 7200 2000 dc00  n.d. .d.e.r. ...
+00004200: 6200 6500 7200 7400 7200 6100 6700 7500  b.e.r.t.r.a.g.u.
+00004210: 6e00 6700 2000 7a00 7500 2000 4800 6100  n.g. .z.u. .H.a.
+00004220: 6d00 5100 5400 4800 2000 6100 7500 6608  m.Q.T.H. .a.u.f.
+00004230: 0000 0000 0600 0000 2741 6e20 6572 726f  ........'An erro
+00004240: 7220 6f63 6375 7265 6420 6f6e 2075 706c  r occured on upl
+00004250: 6f61 6469 6e67 2074 6f20 4861 6d51 5448  oading to HamQTH
+00004260: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00004270: 000e 0041 006e 0074 0065 006e 006e 0065  ...A.n.t.e.n.n.e
+00004280: 0800 0000 0006 0000 0007 416e 7465 6e6e  ..........Antenn
+00004290: 6107 0000 0007 5153 4f46 6f72 6d01 0300  a.....QSOForm...
+000042a0: 0000 1600 4100 7500 7400 6f00 6d00 6100  ....A.u.t.o.m.a.
+000042b0: 7400 6900 7300 6300 6808 0000 0000 0600  t.i.s.c.h.......
+000042c0: 0000 0d41 7574 6f6d 6174 6963 616c 6c79  ...Automatically
+000042d0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+000042e0: 0038 0046 0065 0068 006c 0065 0072 0068  .8.F.e.h.l.e.r.h
+000042f0: 0061 0066 0074 0065 0073 0020 0041 0062  .a.f.t.e.s. .A.b
+00004300: 0066 0072 0061 0067 0065 0065 0072 0067  .f.r.a.g.e.e.r.g
+00004310: 0065 0062 006e 0069 0073 0800 0000 0006  .e.b.n.i.s......
+00004320: 0000 0012 4261 6420 7265 7175 6573 7420  ....Bad request 
+00004330: 7265 7375 6c74 0700 0000 0751 534f 466f  result.....QSOFo
+00004340: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
+00004350: 0004 4261 6e64 0700 0000 0751 534f 466f  ..Band.....QSOFo
+00004360: 726d 0103 0000 0008 0042 00fc 0072 006f  rm.......B...r.o
+00004370: 0800 0000 0006 0000 0006 4275 7265 6175  ..........Bureau
+00004380: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00004390: 0016 0042 00fc 0072 006f 002f 0044 0069  ...B...r.o./.D.i
+000043a0: 0072 0065 006b 0074 0800 0000 0006 0000  .r.e.k.t........
+000043b0: 000d 4275 7265 6175 2f44 6972 6563 7407  ..Bureau/Direct.
+000043c0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+000043d0: 1400 5200 7500 6600 7a00 6500 6900 6300  ..R.u.f.z.e.i.c.
+000043e0: 6800 6500 6e08 0000 0000 0600 0000 0943  h.e.n..........C
+000043f0: 616c 6c20 7369 676e 0700 0000 0751 534f  all sign.....QSO
+00004400: 466f 726d 0103 0000 003c 0046 0065 0068  Form.....<.F.e.h
+00004410: 006c 0065 0072 0020 0062 0065 0069 0020  .l.e.r. .b.e.i. 
+00004420: 0064 0065 0072 0020 0052 0075 0066 007a  .d.e.r. .R.u.f.z
+00004430: 0065 0069 0063 0068 0065 006e 0073 0075  .e.i.c.h.e.n.s.u
+00004440: 0063 0068 0065 0800 0000 0006 0000 0015  .c.h.e..........
+00004450: 4361 6c6c 626f 6f6b 2073 6561 7263 6820  Callbook search 
+00004460: 6572 726f 7207 0000 0007 5153 4f46 6f72  error.....QSOFor
+00004470: 6d01 0300 0000 2a00 4300 6100 6c00 6c00  m.....*.C.a.l.l.
+00004480: 6200 6f00 6f00 6b00 2d00 5300 7500 6300  b.o.o.k.-.S.u.c.
+00004490: 6800 6500 7200 6700 6500 6200 6e00 6900  h.e.r.g.e.b.n.i.
+000044a0: 7308 0000 0000 0600 0000 1643 616c 6c62  s..........Callb
+000044b0: 6f6f 6b20 7365 6172 6368 2072 6573 756c  ook search resul
+000044c0: 7407 0000 0007 5153 4f46 6f72 6d01 0300  t.....QSOForm...
+000044d0: 0000 3200 5200 7500 6600 7a00 6500 6900  ..2.R.u.f.z.e.i.
+000044e0: 6300 6800 6500 6e00 2000 6e00 6900 6300  c.h.e.n. .n.i.c.
+000044f0: 6800 7400 2000 6700 6500 6600 7500 6e00  h.t. .g.e.f.u.n.
+00004500: 6400 6500 6e08 0000 0000 0600 0000 1243  d.e.n..........C
+00004510: 616c 6c73 6967 6e20 6e6f 7420 666f 756e  allsign not foun
+00004520: 6407 0000 0007 5153 4f46 6f72 6d01 0300  d.....QSOForm...
+00004530: 0000 0a00 4b00 6100 6e00 6100 6c08 0000  ....K.a.n.a.l...
+00004540: 0000 0600 0000 0743 6861 6e6e 656c 0700  .......Channel..
+00004550: 0000 0751 534f 466f 726d 0103 0000 0016  ...QSOForm......
+00004560: 0050 0072 00fc 0066 0065 0020 0049 006e  .P.r...f.e. .I.n
+00004570: 0062 006f 0078 0800 0000 0006 0000 000b  .b.o.x..........
+00004580: 4368 6563 6b20 496e 626f 7807 0000 0007  Check Inbox.....
+00004590: 5153 4f46 6f72 6d01 0300 0000 4200 4600  QSOForm.....B.F.
+000045a0: 6500 6800 6c00 6500 7200 2000 6200 6500  e.h.l.e.r. .b.e.
+000045b0: 6900 6d00 2000 5000 7200 fc00 6600 6500  i.m. .P.r...f.e.
+000045c0: 6e00 2000 6400 6500 7200 2000 4c00 6f00  n. .d.e.r. .L.o.
+000045d0: 5400 5700 2d00 4900 6e00 6200 6f00 7808  T.W.-.I.n.b.o.x.
+000045e0: 0000 0000 0600 0000 1643 6865 636b 204c  .........Check L
+000045f0: 6f54 5720 496e 626f 7820 6572 726f 7207  oTW Inbox error.
+00004600: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+00004610: 1c00 5000 7200 fc00 6600 6500 2000 4c00  ..P.r...f.e. .L.
+00004620: 6f00 5400 5700 2000 5100 5300 4c08 0000  o.T.W. .Q.S.L...
+00004630: 0000 0600 0000 0e43 6865 636b 204c 6f54  .......Check LoT
+00004640: 5720 5153 4c07 0000 0007 5153 4f46 6f72  W QSL.....QSOFor
+00004650: 6d01 0300 0000 3800 6500 5100 5300 4c00  m.....8.e.Q.S.L.
+00004660: 2d00 4600 6500 6800 6c00 6500 7200 2000  -.F.e.h.l.e.r. .
+00004670: 7000 7200 fc00 6600 6500 6e00 2000 6400  p.r...f.e.n. .d.
+00004680: 6500 7200 2000 4900 6e00 6200 6f00 7808  e.r. .I.n.b.o.x.
+00004690: 0000 0000 0600 0000 1643 6865 636b 2065  .........Check e
+000046a0: 5153 4c20 496e 626f 7820 6572 726f 7207  QSL Inbox error.
+000046b0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+000046c0: 1800 5a00 7500 7200 fc00 6300 6b00 7300  ..Z.u.r...c.k.s.
+000046d0: 6500 7400 7a00 6500 6e08 0000 0000 0600  e.t.z.e.n.......
+000046e0: 0000 0543 6c65 6172 0700 0000 0751 534f  ...Clear.....QSO
+000046f0: 466f 726d 0103 0000 0020 004b 006f 006e  Form..... .K.o.n
+00004700: 0066 0069 0067 0075 0072 0069 0065 0072  .f.i.g.u.r.i.e.r
+00004710: 0074 0065 0020 0049 0044 0800 0000 0006  .t.e. .I.D......
+00004720: 0000 0013 436f 6e66 6967 7572 6564 2069  ....Configured i
+00004730: 6465 6e74 6974 7907 0000 0007 5153 4f46  dentity.....QSOF
+00004740: 6f72 6d01 0300 0000 2a00 4b00 6f00 6e00  orm.....*.K.o.n.
+00004750: 6600 6900 6700 7500 7200 6900 6500 7200  f.i.g.u.r.i.e.r.
+00004760: 7400 6500 2000 5300 7400 6100 7400 6900  t.e. .S.t.a.t.i.
+00004770: 6f00 6e08 0000 0000 0600 0000 1243 6f6e  o.n..........Con
+00004780: 6669 6775 7265 6420 7374 6174 696f 6e07  figured station.
+00004790: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+000047a0: 0c00 6400 6900 7200 6500 6b00 7408 0000  ..d.i.r.e.k.t...
+000047b0: 0000 0600 0000 0644 6972 6563 7407 0000  .......Direct...
+000047c0: 0007 5153 4f46 6f72 6d01 0300 0000 1c00  ..QSOForm.......
+000047d0: 6500 5100 5300 4c00 2000 7300 7000 6500  e.Q.S.L. .s.p.e.
+000047e0: 6900 6300 6800 6500 7200 6e08 0000 0000  i.c.h.e.r.n.....
+000047f0: 0600 0000 0d44 6f77 6e6c 6f61 6420 6551  .....Download eQ
+00004800: 534c 0700 0000 0751 534f 466f 726d 0103  SL.....QSOForm..
+00004810: 0000 006c 0057 00e4 0068 0072 0065 006e  ...l.W...h.r.e.n
+00004820: 0064 0020 0064 0065 0072 0020 0052 0075  .d. .d.e.r. .R.u
+00004830: 0066 007a 0065 0069 0063 0068 0065 006e  .f.z.e.i.c.h.e.n
+00004840: 0073 0075 0063 0068 0065 0020 0069 0073  .s.u.c.h.e. .i.s
+00004850: 0074 0020 0065 0069 006e 0020 0046 0065  .t. .e.i.n. .F.e
+00004860: 0068 006c 0065 0072 0020 0061 0075 0066  .h.l.e.r. .a.u.f
+00004870: 0067 0065 0074 0072 0065 0074 0065 006e  .g.e.t.r.e.t.e.n
+00004880: 0800 0000 0006 0000 0027 4475 7269 6e67  .........'During
+00004890: 2063 616c 6c62 6f6f 6b20 7365 6172 6368   callbook search
+000048a0: 2061 6e20 6572 726f 7220 6f63 6375 7265   an error occure
+000048b0: 6407 0000 0007 5153 4f46 6f72 6d01 0300  d.....QSOForm...
+000048c0: 0000 0800 4500 6e00 6400 6508 0000 0000  ....E.n.d.e.....
+000048d0: 0600 0000 0345 6e64 0700 0000 0751 534f  .....End.....QSO
+000048e0: 466f 726d 0103 0000 000c 0046 0065 0068  Form.......F.e.h
+000048f0: 006c 0065 0072 0800 0000 0006 0000 0005  .l.e.r..........
+00004900: 4572 726f 7207 0000 0007 5153 4f46 6f72  Error.....QSOFor
+00004910: 6d01 0300 0000 2400 6500 5100 5300 4c00  m.....$.e.Q.S.L.
+00004920: 2d00 5500 7000 6c00 6f00 6100 6400 2d00  -.U.p.l.o.a.d.-.
+00004930: 4600 6500 6800 6c00 6500 7208 0000 0000  F.e.h.l.e.r.....
+00004940: 0600 0000 0f45 7272 6f72 206f 6e20 7570  .....Error on up
+00004950: 6c6f 6164 0700 0000 0751 534f 466f 726d  load.....QSOForm
+00004960: 0103 0000 0010 0046 0072 0065 0071 0075  .......F.r.e.q.u
+00004970: 0065 006e 007a 0800 0000 0006 0000 0009  .e.n.z..........
+00004980: 4672 6571 7565 6e63 7907 0000 0007 5153  Frequency.....QS
+00004990: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
+000049a0: 0600 0000 0648 616d 5154 4807 0000 0007  .....HamQTH.....
+000049b0: 5153 4f46 6f72 6d01 0300 0000 0400 4900  QSOForm.......I.
+000049c0: 4408 0000 0000 0600 0000 0849 6465 6e74  D..........Ident
+000049d0: 6974 7907 0000 0007 5153 4f46 6f72 6d01  ity.....QSOForm.
+000049e0: 0300 0000 2600 4c00 6900 6e00 6b00 2000  ....&.L.i.n.k. .
+000049f0: 7a00 7500 7200 2000 6500 5100 5300 4c00  z.u.r. .e.Q.S.L.
+00004a00: 2d00 4b00 6100 7200 7400 6508 0000 0000  -.K.a.r.t.e.....
+00004a10: 0600 0000 114c 696e 6b20 746f 2065 5153  .....Link to eQS
+00004a20: 4c20 4361 7264 0700 0000 0751 534f 466f  L Card.....QSOFo
+00004a30: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
+00004a40: 0004 4c6f 5457 0700 0000 0751 534f 466f  ..LoTW.....QSOFo
+00004a50: 726d 0103 0000 001c 004c 006f 0054 0057  rm.......L.o.T.W
+00004a60: 0020 0065 006d 0070 0066 0061 006e 0067  . .e.m.p.f.a.n.g
+00004a70: 0065 006e 0800 0000 0006 0000 000d 4c6f  .e.n..........Lo
+00004a80: 5457 2072 6563 6569 7665 6407 0000 0007  TW received.....
+00004a90: 5153 4f46 6f72 6d01 0300 0000 1c00 4c00  QSOForm.......L.
+00004aa0: 6f00 5400 5700 2000 7600 6500 7200 7300  o.T.W. .v.e.r.s.
+00004ab0: 6500 6e00 6400 6500 7408 0000 0000 0600  e.n.d.e.t.......
+00004ac0: 0000 094c 6f54 5720 7365 6e74 0700 0000  ...LoTW sent....
+00004ad0: 0751 534f 466f 726d 0103 ffff ffff 0800  .QSOForm........
+00004ae0: 0000 0006 0000 0007 4c6f 6361 746f 7207  ........Locator.
+00004af0: 0000 0007 5153 4f46 6f72 6d01 03ff ffff  ....QSOForm.....
+00004b00: ff08 0000 0000 0600 0000 074c 6f67 626f  ...........Logbo
+00004b10: 6f6b 0700 0000 0751 534f 466f 726d 0103  ok.....QSOForm..
+00004b20: 0000 0042 004c 006f 0067 0069 006e 0020  ...B.L.o.g.i.n. 
+00004b30: 0066 0065 0068 006c 0067 0065 0073 0063  .f.e.h.l.g.e.s.c
+00004b40: 0068 006c 0061 0067 0065 006e 0020 0066  .h.l.a.g.e.n. .f
+00004b50: 00fc 0072 0020 0042 0065 006e 0075 0074  ...r. .B.e.n.u.t
+00004b60: 007a 0065 0072 0800 0000 0006 0000 0015  .z.e.r..........
+00004b70: 4c6f 6769 6e20 6661 696c 6564 2066 6f72  Login failed for
+00004b80: 2075 7365 7207 0000 0007 5153 4f46 6f72   user.....QSOFor
+00004b90: 6d01 0300 0000 5800 4c00 6f00 6700 6900  m.....X.L.o.g.i.
+00004ba0: 6e00 2000 6200 6500 6900 2000 4800 6100  n. .b.e.i. .H.a.
+00004bb0: 6d00 5100 5400 4800 2000 6600 6500 6800  m.Q.T.H. .f.e.h.
+00004bc0: 6c00 6700 6500 7300 6300 6800 6c00 6100  l.g.e.s.c.h.l.a.
+00004bd0: 6700 6500 6e00 2000 6600 fc00 7200 2000  g.e.n. .f...r. .
+00004be0: 4200 6500 6e00 7500 7400 7a00 6500 7208  B.e.n.u.t.z.e.r.
+00004bf0: 0000 0000 0600 0000 1f4c 6f67 696e 2074  .........Login t
+00004c00: 6f20 4861 6d51 5448 2066 6169 6c65 6420  o HamQTH failed 
+00004c10: 666f 7220 7573 6572 0700 0000 0751 534f  for user.....QSO
+00004c20: 466f 726d 0103 0000 0014 0048 0061 0075  Form.......H.a.u
+00004c30: 0070 0074 0064 0061 0074 0065 006e 0800  .p.t.d.a.t.e.n..
+00004c40: 0000 0006 0000 0009 4d61 696e 2064 6174  ........Main dat
+00004c50: 6107 0000 0007 5153 4f46 6f72 6d01 03ff  a.....QSOForm...
+00004c60: ffff ff08 0000 0000 0600 0000 044d 6f64  .............Mod
+00004c70: 6507 0000 0007 5153 4f46 6f72 6d01 03ff  e.....QSOForm...
+00004c80: ffff ff08 0000 0000 0600 0000 044e 616d  .............Nam
+00004c90: 6507 0000 0007 5153 4f46 6f72 6d01 0300  e.....QSOForm...
+00004ca0: 0000 2400 4b00 6500 6900 6e00 2000 5100  ..$.K.e.i.n. .Q.
+00004cb0: 5300 4c00 2000 7600 6500 7200 6600 fc00  S.L. .v.e.r.f...
+00004cc0: 6700 6200 6100 7208 0000 0000 0600 0000  g.b.a.r.........
+00004cd0: 104e 6f20 5153 4c20 6176 6169 6c61 626c  .No QSL availabl
+00004ce0: 6507 0000 0007 5153 4f46 6f72 6d01 0300  e.....QSOForm...
+00004cf0: 0000 2600 4b00 6500 6900 6e00 2000 6500  ..&.K.e.i.n. .e.
+00004d00: 5100 5300 4c00 2000 7600 6500 7200 6600  Q.S.L. .v.e.r.f.
+00004d10: fc00 6700 6200 6100 7208 0000 0000 0600  ..g.b.a.r.......
+00004d20: 0000 114e 6f20 6551 534c 2061 7661 696c  ...No eQSL avail
+00004d30: 6162 6c65 0700 0000 0751 534f 466f 726d  able.....QSOForm
+00004d40: 0103 0000 000a 004a 0065 0074 007a 0074  .......J.e.t.z.t
+00004d50: 0800 0000 0006 0000 0003 4e6f 7707 0000  ..........Now...
+00004d60: 0007 5153 4f46 6f72 6d01 0300 0000 1600  ..QSOForm.......
+00004d70: 4500 6900 6700 6500 6e00 6500 7200 2000  E.i.g.e.n.e.r. .
+00004d80: 5100 5400 4808 0000 0000 0600 0000 074f  Q.T.H..........O
+00004d90: 776e 2051 5448 0700 0000 0751 534f 466f  wn QTH.....QSOFo
+00004da0: 726d 0103 0000 0024 0045 0069 0067 0065  rm.....$.E.i.g.e
+00004db0: 006e 0065 0073 0020 0052 0075 0066 007a  .n.e.s. .R.u.f.z
+00004dc0: 0065 0069 0063 0068 0065 006e 0800 0000  .e.i.c.h.e.n....
+00004dd0: 0006 0000 000d 4f77 6e20 6361 6c6c 2073  ......Own call s
+00004de0: 6967 6e07 0000 0007 5153 4f46 6f72 6d01  ign.....QSOForm.
+00004df0: 0300 0000 1e00 4500 6900 6700 6500 6e00  ......E.i.g.e.n.
+00004e00: 6500 7200 2000 4c00 6f00 6300 6100 7400  e.r. .L.o.c.a.t.
+00004e10: 6f00 7208 0000 0000 0600 0000 0b4f 776e  o.r..........Own
+00004e20: 206c 6f63 6174 6f72 0700 0000 0751 534f   locator.....QSO
+00004e30: 466f 726d 0103 0000 0018 0045 0069 0067  Form.......E.i.g
+00004e40: 0065 006e 0065 0072 0020 004e 0061 006d  .e.n.e.r. .N.a.m
+00004e50: 0065 0800 0000 0006 0000 0008 4f77 6e20  .e..........Own 
+00004e60: 6e61 6d65 0700 0000 0751 534f 466f 726d  name.....QSOForm
+00004e70: 0103 0000 001c 0045 0069 0067 0065 006e  .......E.i.g.e.n
+00004e80: 0065 0020 004e 006f 0074 0069 007a 0065  .e. .N.o.t.i.z.e
+00004e90: 006e 0800 0000 0006 0000 0009 4f77 6e20  .n..........Own 
+00004ea0: 6e6f 7465 7307 0000 0007 5153 4f46 6f72  notes.....QSOFor
+00004eb0: 6d01 0300 0000 1000 4c00 6500 6900 7300  m.......L.e.i.s.
+00004ec0: 7400 7500 6e00 6708 0000 0000 0600 0000  t.u.n.g.........
+00004ed0: 0550 6f77 6572 0700 0000 0751 534f 466f  .Power.....QSOFo
+00004ee0: 726d 0103 0000 001e 0041 0075 0073 0062  rm.......A.u.s.b
+00004ef0: 0072 0065 0069 0074 0075 006e 0067 0073  .r.e.i.t.u.n.g.s
+00004f00: 0061 0072 0074 0800 0000 0006 0000 000b  .a.r.t..........
+00004f10: 5072 6f70 6167 6174 696f 6e07 0000 0007  Propagation.....
+00004f20: 5153 4f46 6f72 6d01 03ff ffff ff08 0000  QSOForm.........
+00004f30: 0000 0600 0000 0551 525a 4351 0700 0000  .......QRZCQ....
+00004f40: 0751 534f 466f 726d 0103 ffff ffff 0800  .QSOForm........
+00004f50: 0000 0006 0000 0003 5153 4c07 0000 0007  ........QSL.....
+00004f60: 5153 4f46 6f72 6d01 0300 0000 2200 5100  QSOForm.....".Q.
+00004f70: 5300 4c00 2000 2600 2600 2000 4c00 6f00  S.L. .&.&. .L.o.
+00004f80: 6700 2d00 5500 7000 6c00 6f00 6100 6408  g.-.U.p.l.o.a.d.
+00004f90: 0000 0000 0600 0000 1151 534c 2026 2620  .........QSL && 
+00004fa0: 4c6f 6720 7570 6c6f 6164 0700 0000 0751  Log upload.....Q
+00004fb0: 534f 466f 726d 0103 0000 001c 0051 0053  SOForm.......Q.S
+00004fc0: 004c 002d 004b 0061 0072 0074 0065 006e  .L.-.K.a.r.t.e.n
+00004fd0: 0074 0065 0078 0074 0800 0000 0006 0000  .t.e.x.t........
+00004fe0: 0010 5153 4c20 6361 7264 206d 6573 7361  ..QSL card messa
+00004ff0: 6765 0700 0000 0751 534f 466f 726d 0103  ge.....QSOForm..
+00005000: 0000 001a 0051 0053 004c 0020 0065 006d  .....Q.S.L. .e.m
+00005010: 0070 0066 0061 006e 0067 0065 006e 0800  .p.f.a.n.g.e.n..
+00005020: 0000 0006 0000 000c 5153 4c20 7265 6365  ........QSL rece
+00005030: 6976 6564 0700 0000 0751 534f 466f 726d  ived.....QSOForm
+00005040: 0103 0000 0018 0051 0053 004c 0020 0067  .......Q.S.L. .g
+00005050: 0065 0073 0065 006e 0064 0065 0074 0800  .e.s.e.n.d.e.t..
+00005060: 0000 0006 0000 0008 5153 4c20 7365 6e74  ........QSL sent
+00005070: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00005080: 000e 0051 0053 004c 002d 0056 0069 0061  ...Q.S.L.-.V.i.a
+00005090: 0800 0000 0006 0000 0007 5153 4c20 7669  ..........QSL vi
+000050a0: 6107 0000 0007 5153 4f46 6f72 6d01 0300  a.....QSOForm...
+000050b0: 0000 1800 5100 5300 4f00 2d00 4600 6f00  ....Q.S.O.-.F.o.
+000050c0: 7200 6d00 7500 6c00 6100 7208 0000 0000  r.m.u.l.a.r.....
+000050d0: 0600 0000 0851 534f 2046 6f72 6d07 0000  .....QSO Form...
+000050e0: 0007 5153 4f46 6f72 6d01 0300 0000 1a00  ..QSOForm.......
+000050f0: 5100 5300 4f00 2d00 4b00 6f00 6d00 6d00  Q.S.O.-.K.o.m.m.
+00005100: 6500 6e00 7400 6100 7208 0000 0000 0600  e.n.t.a.r.......
+00005110: 0000 0b51 534f 2063 6f6d 6d65 6e74 0700  ...QSO comment..
+00005120: 0000 0751 534f 466f 726d 0103 0000 003e  ...QSOForm.....>
+00005130: 0051 0053 004f 0020 0077 0075 0072 0064  .Q.S.O. .w.u.r.d
+00005140: 0065 0020 0076 006f 006e 0020 0048 0061  .e. .v.o.n. .H.a
+00005150: 006d 0051 0054 0048 0020 0061 0062 0067  .m.Q.T.H. .a.b.g
+00005160: 0065 0077 0069 0065 0073 0065 006e 0800  .e.w.i.e.s.e.n..
+00005170: 0000 0006 0000 0016 5153 4f20 7265 6a65  ........QSO reje
+00005180: 6374 6564 206f 6e20 4861 6d51 5448 0700  cted on HamQTH..
+00005190: 0000 0751 534f 466f 726d 0103 ffff ffff  ...QSOForm......
+000051a0: 0800 0000 0006 0000 0003 5154 4807 0000  ..........QTH...
+000051b0: 0007 5153 4f46 6f72 6d01 03ff ffff ff08  ..QSOForm.......
+000051c0: 0000 0000 0600 0000 0652 5354 2052 7807  .........RST Rx.
+000051d0: 0000 0007 5153 4f46 6f72 6d01 03ff ffff  ....QSOForm.....
+000051e0: ff08 0000 0000 0600 0000 0652 5354 2054  ...........RST T
+000051f0: 7807 0000 0007 5153 4f46 6f72 6d01 0300  x.....QSOForm...
+00005200: 0000 1a00 5200 5300 5400 2000 6500 6d00  ....R.S.T. .e.m.
+00005210: 7000 6600 6100 6e00 6700 6500 6e08 0000  p.f.a.n.g.e.n...
+00005220: 0000 0600 0000 0c52 5354 2072 6563 6569  .......RST recei
+00005230: 7665 6407 0000 0007 5153 4f46 6f72 6d01  ved.....QSOForm.
+00005240: 0300 0000 1800 5200 5300 5400 2000 6700  ......R.S.T. .g.
+00005250: 6500 7300 6500 6e00 6400 6500 7408 0000  e.s.e.n.d.e.t...
+00005260: 0000 0600 0000 0852 5354 2073 656e 7407  .......RST sent.
+00005270: 0000 0007 5153 4f46 6f72 6d01 03ff ffff  ....QSOForm.....
+00005280: ff08 0000 0000 0600 0000 0552 6164 696f  ...........Radio
+00005290: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+000052a0: 0012 0053 0070 0065 0069 0063 0068 0065  ...S.p.e.i.c.h.e
+000052b0: 0072 006e 0800 0000 0006 0000 0004 5361  .r.n..........Sa
+000052c0: 7665 0700 0000 0751 534f 466f 726d 0103  ve.....QSOForm..
+000052d0: 0000 0026 0053 0070 0065 0069 0063 0068  ...&.S.p.e.i.c.h
+000052e0: 0065 0072 006e 0020 0026 0026 0020 0055  .e.r.n. .&.&. .U
+000052f0: 0070 006c 006f 0061 0064 0800 0000 0006  .p.l.o.a.d......
+00005300: 0000 000e 5361 7665 2026 2620 5570 6c6f  ....Save && Uplo
+00005310: 6164 0700 0000 0751 534f 466f 726d 0103  ad.....QSOForm..
+00005320: 0000 002a 0065 0051 0053 004c 002d 004f  ...*.e.Q.S.L.-.O
+00005330: 0072 0064 006e 0065 0072 0020 0061 0075  .r.d.n.e.r. .a.u
+00005340: 0073 0077 00e4 0068 006c 0065 006e 0800  .s.w...h.l.e.n..
+00005350: 0000 0006 0000 0012 5365 6c65 6374 2065  ........Select e
+00005360: 5153 4c20 666f 6c64 6572 0700 0000 0751  QSL folder.....Q
+00005370: 534f 466f 726d 0103 0000 0036 0053 0065  SOForm.....6.S.e
+00005380: 0072 0076 0065 0072 006b 006f 006d 006d  .r.v.e.r.k.o.m.m
+00005390: 0075 006e 0069 006b 0061 0074 0069 006f  .u.n.i.k.a.t.i.o
+000053a0: 006e 0073 002d 0046 0065 0068 006c 0065  .n.s.-.F.e.h.l.e
+000053b0: 0072 0800 0000 0006 0000 001a 5365 7276  .r..........Serv
+000053c0: 6572 2063 6f6d 6d75 6e69 6361 7469 6f6e  er communication
+000053d0: 2065 7272 6f72 0700 0000 0751 534f 466f   error.....QSOFo
+000053e0: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
+000053f0: 0005 5374 6172 7407 0000 0007 5153 4f46  ..Start.....QSOF
+00005400: 6f72 6d01 03ff ffff ff08 0000 0000 0600  orm.............
+00005410: 0000 0753 7461 7469 6f6e 0700 0000 0751  ...Station.....Q
+00005420: 534f 466f 726d 0103 ffff ffff 0800 0000  SOForm..........
+00005430: 0006 0000 0007 5375 626d 6f64 6507 0000  ......Submode...
+00005440: 0007 5153 4f46 6f72 6d01 0300 0000 3000  ..QSOForm.....0.
+00005450: 4400 6100 7300 2000 5100 5300 4f00 2000  D.a.s. .Q.S.O. .
+00005460: 6900 7300 7400 2000 6500 6900 6e00 2000  i.s.t. .e.i.n. .
+00005470: 4400 7500 7000 6c00 6900 6b00 6100 7408  D.u.p.l.i.k.a.t.
+00005480: 0000 0000 0600 0000 1654 6865 2051 534f  .........The QSO
+00005490: 2069 7320 6120 6475 706c 6963 6174 6507   is a duplicate.
+000054a0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+000054b0: b800 4400 6900 6500 2000 5100 5300 4c00  ..D.i.e. .Q.S.L.
+000054c0: 2d00 5200 6f00 7500 7400 6500 2000 6400  -.R.o.u.t.e. .d.
+000054d0: 6500 7200 2000 6b00 6f00 6e00 7400 6100  e.r. .k.o.n.t.a.
+000054e0: 6b00 7400 6900 6500 7200 7400 6500 6e00  k.t.i.e.r.t.e.n.
+000054f0: 2000 5300 7400 6100 7400 6900 6f00 6e00   .S.t.a.t.i.o.n.
+00005500: 2e00 0a00 4400 6900 6500 7300 2000 6900  ....D.i.e.s. .i.
+00005510: 7300 7400 2000 6e00 6900 6300 6800 7400  s.t. .n.i.c.h.t.
+00005520: 2000 6400 6900 6500 2000 4100 6400 7200   .d.i.e. .A.d.r.
+00005530: 6500 7300 7300 6500 2000 6400 6500 7300  e.s.s.e. .d.e.s.
+00005540: 2000 5100 5300 4c00 2d00 4d00 6100 6e00   .Q.S.L.-.M.a.n.
+00005550: 6100 6700 6500 7200 7300 2f00 2d00 4200  a.g.e.r.s./.-.B.
+00005560: fc00 7200 6f00 7300 2e08 0000 0000 0600  ..r.o.s.........
+00005570: 0000 4c54 6865 2063 6f6e 7461 6374 6564  ..LThe contacted
+00005580: 2073 7461 7469 6f6e 2051 534c 2072 6f75   station QSL rou
+00005590: 7465 2e0a 5468 6973 2069 7320 6e6f 7420  te..This is not 
+000055a0: 7468 6520 5153 4c20 6d61 6e61 6765 722f  the QSL manager/
+000055b0: 6275 7265 6175 2061 6464 7265 7373 2e07  bureau address..
+000055c0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+000055d0: 1000 4500 6e00 6400 6500 7a00 6500 6900  ..E.n.d.e.z.e.i.
+000055e0: 7408 0000 0000 0600 0000 0854 696d 6520  t..........Time 
+000055f0: 656e 6407 0000 0007 5153 4f46 6f72 6d01  end.....QSOForm.
+00005600: 0300 0000 1200 5300 7400 6100 7200 7400  ......S.t.a.r.t.
+00005610: 7a00 6500 6900 7408 0000 0000 0600 0000  z.e.i.t.........
+00005620: 0a54 696d 6520 7374 6172 7407 0000 0007  .Time start.....
+00005630: 5153 4f46 6f72 6d01 0300 0000 2400 6500  QSOForm.....$.e.
+00005640: 5100 5300 4c00 2d00 5500 7000 6c00 6f00  Q.S.L.-.U.p.l.o.
+00005650: 6100 6400 2d00 4600 6500 6800 6c00 6500  a.d.-.F.e.h.l.e.
+00005660: 7208 0000 0000 0600 0000 1155 706c 6f61  r..........Uploa
+00005670: 6420 6551 534c 2065 7272 6f72 0700 0000  d eQSL error....
+00005680: 0751 534f 466f 726d 0103 0000 001a 0055  .QSOForm.......U
+00005690: 0070 006c 006f 0061 0064 002d 0046 0065  .p.l.o.a.d.-.F.e
+000056a0: 0068 006c 0065 0072 0800 0000 0006 0000  .h.l.e.r........
+000056b0: 0010 5570 6c6f 6164 206c 6f67 2065 7272  ..Upload log err
+000056c0: 6f72 0700 0000 0751 534f 466f 726d 0103  or.....QSOForm..
+000056d0: 0000 0068 0055 0070 006c 006f 0061 0064  ...h.U.p.l.o.a.d
+000056e0: 0020 0065 0072 0066 006f 006c 0067 0074  . .e.r.f.o.l.g.t
+000056f0: 0020 006e 0075 0072 0020 0077 0065 006e  . .n.u.r. .w.e.n
+00005700: 006e 0020 0061 0075 0066 0020 0064 0065  .n. .a.u.f. .d.e
+00005710: 0072 0020 0051 0053 004c 002d 0053 0065  .r. .Q.S.L.-.S.e
+00005720: 0069 0074 0065 0020 0061 0075 0073 0067  .i.t.e. .a.u.s.g
+00005730: 0065 0077 00e4 0068 006c 0074 0800 0000  .e.w...h.l.t....
+00005740: 0006 0000 0024 5570 6c6f 6164 7320 6f6e  .....$Uploads on
+00005750: 6c79 2069 6620 7365 6c65 6374 6564 206f  ly if selected o
+00005760: 6e20 5153 4c20 7061 6765 0700 0000 0751  n QSL page.....Q
+00005770: 534f 466f 726d 0103 0000 0048 0044 0065  SOForm.....H.D.e
+00005780: 0072 0020 004e 0075 0074 007a 0065 0072  .r. .N.u.t.z.e.r
+00005790: 0020 0043 0061 006c 006c 0020 0073 0074  . .C.a.l.l. .s.t
+000057a0: 0069 006d 006d 0074 0020 006e 0069 0063  .i.m.m.t. .n.i.c
+000057b0: 0068 0074 0020 00fc 0062 0065 0072 0065  .h.t. ...b.e.r.e
+000057c0: 0069 006e 0800 0000 0006 0000 0018 5573  .i.n..........Us
+000057d0: 6572 2063 616c 6c20 646f 6573 206e 6f74  er call does not
+000057e0: 206d 6174 6368 0700 0000 0751 534f 466f   match.....QSOFo
+000057f0: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
+00005800: 0004 6551 534c 0700 0000 0751 534f 466f  ..eQSL.....QSOFo
+00005810: 726d 0103 0000 001c 0065 0051 0053 004c  rm.......e.Q.S.L
+00005820: 0020 0065 006d 0070 0066 0061 006e 0067  . .e.m.p.f.a.n.g
+00005830: 0065 006e 0800 0000 0006 0000 000d 6551  .e.n..........eQ
+00005840: 534c 2072 6563 6569 7665 6407 0000 0007  SL received.....
+00005850: 5153 4f46 6f72 6d01 0300 0000 1a00 6500  QSOForm.......e.
+00005860: 5100 5300 4c00 2000 6700 6500 7300 6500  Q.S.L. .g.e.s.e.
+00005870: 6e00 6400 6500 7408 0000 0000 0600 0000  n.d.e.t.........
+00005880: 0965 5153 4c20 7365 6e74 0700 0000 0751  .eQSL sent.....Q
+00005890: 534f 466f 726d 0103 0000 0008 006b 002e  SOForm.......k..
+000058a0: 0041 002e 0800 0000 0006 0000 0004 6e2e  .A............n.
+000058b0: 612e 0700 0000 0751 534f 466f 726d 0103  a......QSOForm..
+000058c0: 0000 0034 0072 0069 0067 0063 0074 006c  ...4.r.i.g.c.t.l
+000058d0: 0064 0020 005a 0065 0069 0074 00fc 0062  .d. .Z.e.i.t...b
+000058e0: 0065 0072 0073 0063 0068 0072 0065 0069  .e.r.s.c.h.r.e.i
+000058f0: 0074 0075 006e 0067 0800 0000 0006 0000  .t.u.n.g........
+00005900: 000f 7269 6763 746c 6420 7469 6d65 6f75  ..rigctld timeou
+00005910: 7407 0000 0007 5153 4f46 6f72 6d01 03ff  t.....QSOForm...
+00005920: ffff ff08 0000 0000 0600 0000 0a79 7979  .............yyy
+00005930: 792d 4d4d 2d64 6407 0000 0007 5153 4f46  y-MM-dd.....QSOF
+00005940: 6f72 6d01 0300 0000 7a00 4300 4100 5400  orm.....z.C.A.T.
+00005950: 2d00 4500 6900 6e00 7300 7400 6500 6c00  -.E.i.n.s.t.e.l.
+00005960: 6c00 7500 6e00 6700 2000 7700 7500 7200  l.u.n.g. .w.u.r.
+00005970: 6400 2000 6e00 6f00 6300 6800 2000 6e00  d. .n.o.c.h. .n.
+00005980: 6900 6500 2000 6700 6500 7300 7000 6500  i.e. .g.e.s.p.e.
+00005990: 6900 6300 6800 6500 7200 7400 2000 6f00  i.c.h.e.r.t. .o.
+000059a0: 7200 2000 5000 6100 7200 6100 6d00 6500  r. .P.a.r.a.m.e.
+000059b0: 7400 6500 7200 2000 6600 6500 6800 6c00  t.e.r. .f.e.h.l.
+000059c0: 6500 6e08 0000 0000 0600 0000 3b43 4154  e.n.........;CAT
+000059d0: 2063 6f6e 6669 6775 7261 7469 6f6e 2077   configuration w
+000059e0: 6173 206e 6576 6572 2073 6176 6564 206f  as never saved o
+000059f0: 7220 6120 7061 7261 6d65 7465 7220 6973  r a parameter is
+00005a00: 206d 6973 7369 6e67 0700 0000 0853 6574   missing.....Set
+00005a10: 7469 6e67 7301 0300 0000 3000 4300 4100  tings.....0.C.A.
+00005a20: 5400 2d00 4500 6900 6e00 7300 7400 6500  T.-.E.i.n.s.t.e.
+00005a30: 6c00 6c00 7500 6e00 6700 6500 6e00 2000  l.l.u.n.g.e.n. .
+00005a40: 4600 6500 6800 6c00 6500 7208 0000 0000  F.e.h.l.e.r.....
+00005a50: 0600 0000 1243 4154 2073 6574 7469 6e67  .....CAT setting
+00005a60: 7320 6572 726f 7207 0000 0008 5365 7474  s error.....Sett
+00005a70: 696e 6773 0103 0000 002a 0048 0061 006d  ings.....*.H.a.m
+00005a80: 006c 0069 0062 0020 0072 0069 0067 0063  .l.i.b. .r.i.g.c
+00005a90: 0074 006c 0064 0020 0077 00e4 0068 006c  .t.l.d. .w...h.l
+00005aa0: 0065 006e 0800 0000 0006 0000 0020 4368  .e.n......... Ch
+00005ab0: 6f6f 7365 2068 616d 6c69 6220 7269 6763  oose hamlib rigc
+00005ac0: 746c 6420 6578 6563 7574 6162 6c65 0700  tld executable..
+00005ad0: 0000 0853 6574 7469 6e67 7301 0300 0000  ...Settings.....
+00005ae0: 2000 4400 6100 7400 7500 6d00 2f00 5a00   .D.a.t.u.m./.Z.
+00005af0: 6500 6900 7400 2000 5300 7400 6100 7200  e.i.t. .S.t.a.r.
+00005b00: 7408 0000 0000 0600 0000 0f44 6174 652f  t..........Date/
+00005b10: 5469 6d65 2073 7461 7274 0700 0000 0853  Time start.....S
+00005b20: 6574 7469 6e67 7301 0300 0000 4200 4600  ettings.....B.F.
+00005b30: 6500 6800 6c00 6500 7200 2000 6200 6500  e.h.l.e.r. .b.e.
+00005b40: 6900 6d00 2000 4100 7500 7300 6600 fc00  i.m. .A.u.s.f...
+00005b50: 6800 7200 6500 6e00 2000 7600 6f00 6e00  h.r.e.n. .v.o.n.
+00005b60: 2000 7200 6900 6700 6300 7400 6c00 6408   .r.i.g.c.t.l.d.
+00005b70: 0000 0000 0600 0000 1745 7272 6f72 2065  .........Error e
+00005b80: 7865 6375 7469 6e67 2072 6967 6374 6c64  xecuting rigctld
+00005b90: 0700 0000 0853 6574 7469 6e67 7301 03ff  .....Settings...
+00005ba0: ffff ff08 0000 0000 0600 0000 0648 616d  .............Ham
+00005bb0: 6c69 6207 0000 0008 5365 7474 696e 6773  lib.....Settings
+00005bc0: 0103 0000 004e 0044 0069 0065 0020 0067  .....N.D.i.e. .g
+00005bd0: 0065 0077 00e4 0068 006c 0074 0065 0020  .e.w...h.l.t.e. 
+00005be0: 0044 0061 0074 0065 0069 0020 0069 0073  .D.a.t.e.i. .i.s
+00005bf0: 0074 0020 006e 0069 0063 0068 0074 0020  .t. .n.i.c.h.t. 
+00005c00: 0061 0075 0073 0066 00fc 0068 0072 0062  .a.u.s.f...h.r.b
+00005c10: 0061 0072 0800 0000 0006 0000 0023 5365  .a.r.........#Se
+00005c20: 6c65 6374 6564 2066 696c 6520 6973 206e  lected file is n
+00005c30: 6f74 2074 6865 2065 7865 6375 7461 626c  ot the executabl
+00005c40: 6507 0000 0008 5365 7474 696e 6773 0103  e.....Settings..
+00005c50: 0000 0014 007a 0065 0069 0067 0065 0020  .....z.e.i.g.e. 
+00005c60: 0061 006c 006c 0065 0800 0000 0006 0000  .a.l.l.e........
+00005c70: 0008 5368 6f77 2061 6c6c 0700 0000 0853  ..Show all.....S
+00005c80: 6574 7469 6e67 7301 03ff ffff ff08 0000  ettings.........
+00005c90: 0000 0600 0000 0553 7461 7274 0700 0000  .......Start....
+00005ca0: 0853 6574 7469 6e67 7301 0300 0000 1a00  .Settings.......
+00005cb0: 5300 7400 6100 7200 7400 6500 2000 4800  S.t.a.r.t.e. .H.
+00005cc0: 6100 6d00 6c00 6900 6208 0000 0000 0600  a.m.l.i.b.......
+00005cd0: 0000 0c53 7461 7274 2068 616d 6c69 6207  ...Start hamlib.
+00005ce0: 0000 0008 5365 7474 696e 6773 0103 ffff  ....Settings....
+00005cf0: ffff 0800 0000 0006 0000 0004 5374 6f70  ............Stop
+00005d00: 0700 0000 0853 6574 7469 6e67 7301 0300  .....Settings...
+00005d10: 0000 1a00 5300 7400 6f00 7000 7000 6500  ....S.t.o.p.p.e.
+00005d20: 2000 4800 6100 6d00 6c00 6900 6208 0000   .H.a.m.l.i.b...
+00005d30: 0000 0600 0000 0b53 746f 7020 6861 6d6c  .......Stop haml
+00005d40: 6962 0700 0000 0853 6574 7469 6e67 7301  ib.....Settings.
+00005d50: 0300 0000 0a00 6100 6b00 7400 6900 7608  ......a.k.t.i.v.
+00005d60: 0000 0000 0600 0000 0561 6374 6976 0700  .........activ..
+00005d70: 0000 0853 6574 7469 6e67 7301 0300 0000  ...Settings.....
+00005d80: 0e00 6900 6e00 6100 6b00 7400 6900 7608  ..i.n.a.k.t.i.v.
+00005d90: 0000 0000 0600 0000 0769 6e61 6374 6976  .........inactiv
+00005da0: 0700 0000 0853 6574 7469 6e67 7301 0300  .....Settings...
+00005db0: 0000 4a00 7200 6900 6700 6300 7400 6c00  ..J.r.i.g.c.t.l.
+00005dc0: 6400 2000 6b00 6f00 6e00 6e00 7400 6500  d. .k.o.n.n.t.e.
+00005dd0: 2000 6e00 6900 6300 6800 7400 2000 6700   .n.i.c.h.t. .g.
+00005de0: 6500 7300 7400 6100 7200 7400 6500 7400  e.s.t.a.r.t.e.t.
+00005df0: 2000 7700 6500 7200 6400 6500 6e08 0000   .w.e.r.d.e.n...
+00005e00: 0000 0600 0000 1e72 6967 6374 6c64 2064  .......rigctld d
+00005e10: 6964 206e 6f74 2073 7461 7274 2070 726f  id not start pro
+00005e20: 7065 726c 7907 0000 0008 5365 7474 696e  perly.....Settin
+00005e30: 6773 0103 0000 0010 0067 0065 00e4 006e  gs.......g.e...n
+00005e40: 0064 0065 0072 0074 0800 0000 0006 0000  .d.e.r.t........
+00005e50: 0001 4d07 0000 0014 5472 616e 736c 6174  ..M.....Translat
+00005e60: 6564 5461 626c 654d 6f64 656c 0103 0000  edTableModel....
+00005e70: 0008 004e 0065 0069 006e 0800 0000 0006  ...N.e.i.n......
+00005e80: 0000 0001 4e07 0000 0014 5472 616e 736c  ....N.....Transl
+00005e90: 6174 6564 5461 626c 654d 6f64 656c 0103  atedTableModel..
+00005ea0: 0000 0012 0061 006e 0067 0065 0066 0072  .....a.n.g.e.f.r
+00005eb0: 0061 0067 0074 0800 0000 0006 0000 0001  .a.g.t..........
+00005ec0: 5207 0000 0014 5472 616e 736c 6174 6564  R.....Translated
+00005ed0: 5461 626c 654d 6f64 656c 0103 0000 0004  TableModel......
+00005ee0: 004a 0061 0800 0000 0006 0000 0001 5907  .J.a..........Y.
+00005ef0: 0000 0014 5472 616e 736c 6174 6564 5461  ....TranslatedTa
+00005f00: 626c 654d 6f64 656c 0103 ffff ffff 0800  bleModel........
+00005f10: 0000 0006 0000 0007 4a53 3843 616c 6c07  ........JS8Call.
+00005f20: 0000 000f 6170 7053 656c 6563 7444 6961  ....appSelectDia
+00005f30: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
+00005f40: 0000 054f 7468 6572 0700 0000 0f61 7070  ...Other.....app
+00005f50: 5365 6c65 6374 4469 616c 6f67 0103 0000  SelectDialog....
+00005f60: 002a 0041 0075 0073 0077 0061 0068 006c  .*.A.u.s.w.a.h.l
+00005f70: 0020 0064 0065 0073 0020 0050 0072 006f  . .d.e.s. .P.r.o
+00005f80: 0067 0072 0061 006d 006d 0073 0800 0000  .g.r.a.m.m.s....
+00005f90: 0006 0000 0016 5365 6c65 6374 2074 6865  ......Select the
+00005fa0: 2061 7070 6c69 6361 7469 6f6e 0700 0000   application....
+00005fb0: 0f61 7070 5365 6c65 6374 4469 616c 6f67  .appSelectDialog
+00005fc0: 0103 ffff ffff 0800 0000 0006 0000 0006  ................
+00005fd0: 5753 4a54 2d58 0700 0000 0f61 7070 5365  WSJT-X.....appSe
+00005fe0: 6c65 6374 4469 616c 6f67 0103 ffff ffff  lectDialog......
+00005ff0: 0800 0000 0006 0000 0006 666c 6469 6769  ..........fldigi
+00006000: 0700 0000 0f61 7070 5365 6c65 6374 4469  .....appSelectDi
+00006010: 616c 6f67 0188 0000 0002 0101            alog........
```

### Comparing `DragonLog-1.0/dragonlog/data/modes.json` & `dragonlog-1.1/dragonlog/data/modes.json`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/Screenshot.png` & `dragonlog-1.1/dragonlog/icons/Screenshot.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/db.png` & `dragonlog-1.1/dragonlog/icons/db.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/edit.png` & `dragonlog-1.1/dragonlog/icons/edit.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/edit_add.png` & `dragonlog-1.1/dragonlog/icons/edit_add.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/edit_addmulti.png` & `dragonlog-1.1/dragonlog/icons/edit_addmulti.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/edit_addmulti.xcf` & `dragonlog-1.1/dragonlog/icons/edit_addmulti.xcf`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/edit_remove.png` & `dragonlog-1.1/dragonlog/icons/edit_remove.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/exit.png` & `dragonlog-1.1/dragonlog/icons/exit.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/file_doc.png` & `dragonlog-1.1/dragonlog/icons/file_doc.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/fileexport.png` & `dragonlog-1.1/dragonlog/icons/fileexport.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/fileimport.png` & `dragonlog-1.1/dragonlog/icons/fileimport.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/gear.png` & `dragonlog-1.1/dragonlog/icons/gear.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/help.png` & `dragonlog-1.1/dragonlog/icons/help.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/icons8-dragon-96.png` & `dragonlog-1.1/dragonlog/icons/icons8-dragon-96.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/icons8-dragon-96.xcf` & `dragonlog-1.1/dragonlog/icons/icons8-dragon-96.xcf`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/info.png` & `dragonlog-1.1/dragonlog/icons/info.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/logo.ico` & `dragonlog-1.1/dragonlog/icons/logo.ico`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/player_play.png` & `dragonlog-1.1/dragonlog/icons/player_play.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/player_stop.png` & `dragonlog-1.1/dragonlog/icons/player_stop.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/upload_lotw.png` & `dragonlog-1.1/dragonlog/icons/upload_lotw.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/upload_lotw.xcf` & `dragonlog-1.1/dragonlog/icons/upload_lotw.xcf`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/dragonlog/icons/watch.png` & `dragonlog-1.1/dragonlog/icons/watch.png`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/pyproject.toml` & `dragonlog-1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `DragonLog-1.0/setup_msi.py` & `dragonlog-1.1/setup_msi.py`

 * *Files identical despite different names*


# Comparing `tmp/ovos-stt-plugin-fasterwhisper-0.0.1a8.tar.gz` & `tmp/ovos-stt-plugin-fasterwhisper-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-stt-plugin-fasterwhisper-0.0.1a8.tar", last modified: Tue Dec  5 22:59:31 2023, max compression
+gzip compressed data, was "ovos-stt-plugin-fasterwhisper-0.0.1a9.tar", last modified: Sat Apr 20 23:20:30 2024, max compression
```

## Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a8.tar` & `ovos-stt-plugin-fasterwhisper-0.0.1a9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 22:59:31.686825 ovos-stt-plugin-fasterwhisper-0.0.1a8/
--rw-r--r--   0 runner    (1001) docker     (127)    11431 2023-12-05 22:59:23.000000 ovos-stt-plugin-fasterwhisper-0.0.1a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-12-05 22:59:23.000000 ovos-stt-plugin-fasterwhisper-0.0.1a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-05 22:59:31.686825 ovos-stt-plugin-fasterwhisper-0.0.1a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-12-05 22:59:23.000000 ovos-stt-plugin-fasterwhisper-0.0.1a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 22:59:31.686825 ovos-stt-plugin-fasterwhisper-0.0.1a8/ovos_stt_plugin_fasterwhisper/
--rw-r--r--   0 runner    (1001) docker     (127)     8896 2023-12-05 22:59:23.000000 ovos-stt-plugin-fasterwhisper-0.0.1a8/ovos_stt_plugin_fasterwhisper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-05 22:59:26.000000 ovos-stt-plugin-fasterwhisper-0.0.1a8/ovos_stt_plugin_fasterwhisper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 22:59:31.686825 ovos-stt-plugin-fasterwhisper-0.0.1a8/ovos_stt_plugin_fasterwhisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-05 22:59:31.000000 ovos-stt-plugin-fasterwhisper-0.0.1a8/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      489 2023-12-05 22:59:31.000000 ovos-stt-plugin-fasterwhisper-0.0.1a8/ovos_stt_plugin_fasterwhisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 22:59:31.000000 ovos-stt-plugin-fasterwhisper-0.0.1a8/ovos_stt_plugin_fasterwhisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-12-05 22:59:31.000000 ovos-stt-plugin-fasterwhisper-0.0.1a8/ovos_stt_plugin_fasterwhisper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-12-05 22:59:31.000000 ovos-stt-plugin-fasterwhisper-0.0.1a8/ovos_stt_plugin_fasterwhisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-05 22:59:31.000000 ovos-stt-plugin-fasterwhisper-0.0.1a8/ovos_stt_plugin_fasterwhisper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 22:59:31.000000 ovos-stt-plugin-fasterwhisper-0.0.1a8/ovos_stt_plugin_fasterwhisper.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-05 22:59:31.686825 ovos-stt-plugin-fasterwhisper-0.0.1a8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3493 2023-12-05 22:59:23.000000 ovos-stt-plugin-fasterwhisper-0.0.1a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 23:20:30.209006 ovos-stt-plugin-fasterwhisper-0.0.1a9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11431 2024-04-20 23:20:22.000000 ovos-stt-plugin-fasterwhisper-0.0.1a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-20 23:20:22.000000 ovos-stt-plugin-fasterwhisper-0.0.1a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-20 23:20:30.209006 ovos-stt-plugin-fasterwhisper-0.0.1a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-20 23:20:22.000000 ovos-stt-plugin-fasterwhisper-0.0.1a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 23:20:30.209006 ovos-stt-plugin-fasterwhisper-0.0.1a9/ovos_stt_plugin_fasterwhisper/
+-rw-r--r--   0 runner    (1001) docker     (127)     8896 2024-04-20 23:20:22.000000 ovos-stt-plugin-fasterwhisper-0.0.1a9/ovos_stt_plugin_fasterwhisper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-20 23:20:25.000000 ovos-stt-plugin-fasterwhisper-0.0.1a9/ovos_stt_plugin_fasterwhisper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 23:20:30.209006 ovos-stt-plugin-fasterwhisper-0.0.1a9/ovos_stt_plugin_fasterwhisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-20 23:20:29.000000 ovos-stt-plugin-fasterwhisper-0.0.1a9/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-20 23:20:30.000000 ovos-stt-plugin-fasterwhisper-0.0.1a9/ovos_stt_plugin_fasterwhisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 23:20:29.000000 ovos-stt-plugin-fasterwhisper-0.0.1a9/ovos_stt_plugin_fasterwhisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-20 23:20:29.000000 ovos-stt-plugin-fasterwhisper-0.0.1a9/ovos_stt_plugin_fasterwhisper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-20 23:20:29.000000 ovos-stt-plugin-fasterwhisper-0.0.1a9/ovos_stt_plugin_fasterwhisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-20 23:20:29.000000 ovos-stt-plugin-fasterwhisper-0.0.1a9/ovos_stt_plugin_fasterwhisper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 23:20:29.000000 ovos-stt-plugin-fasterwhisper-0.0.1a9/ovos_stt_plugin_fasterwhisper.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 23:20:30.209006 ovos-stt-plugin-fasterwhisper-0.0.1a9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3493 2024-04-20 23:20:22.000000 ovos-stt-plugin-fasterwhisper-0.0.1a9/setup.py
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a8/LICENSE` & `ovos-stt-plugin-fasterwhisper-0.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a8/PKG-INFO` & `ovos-stt-plugin-fasterwhisper-0.0.1a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-stt-plugin-fasterwhisper
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: A fasterwhisper stt plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-plugin-fasterwhisper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft ovos plugin stt
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a8/README.md` & `ovos-stt-plugin-fasterwhisper-0.0.1a9/README.md`

 * *Files identical despite different names*

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a8/ovos_stt_plugin_fasterwhisper/__init__.py` & `ovos-stt-plugin-fasterwhisper-0.0.1a9/ovos_stt_plugin_fasterwhisper/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a8/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO` & `ovos-stt-plugin-fasterwhisper-0.0.1a9/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-stt-plugin-fasterwhisper
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: A fasterwhisper stt plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-plugin-fasterwhisper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft ovos plugin stt
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a8/setup.py` & `ovos-stt-plugin-fasterwhisper-0.0.1a9/setup.py`

 * *Files identical despite different names*


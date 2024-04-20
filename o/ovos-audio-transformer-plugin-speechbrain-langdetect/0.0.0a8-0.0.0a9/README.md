# Comparing `tmp/ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8.tar.gz` & `tmp/ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8.tar", last modified: Mon Oct 23 21:25:34 2023, max compression
+gzip compressed data, was "ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9.tar", last modified: Thu Dec  7 21:41:33 2023, max compression
```

## Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8.tar` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 21:25:34.282268 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/
--rw-r--r--   0 runner    (1001) docker     (127)    11431 2023-10-23 21:25:24.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-10-23 21:25:24.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-10-23 21:25:34.282268 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-10-23 21:25:24.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 21:25:34.282268 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/ovos_audio_transformer_plugin_speechbrain_langdetect/
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2023-10-23 21:25:24.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/ovos_audio_transformer_plugin_speechbrain_langdetect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-10-23 21:25:27.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/ovos_audio_transformer_plugin_speechbrain_langdetect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 21:25:34.282268 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-10-23 21:25:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-10-23 21:25:34.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-23 21:25:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-10-23 21:25:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-23 21:25:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-23 21:25:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-23 21:25:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-23 21:25:34.282268 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3240 2023-10-23 21:25:24.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:41:33.714212 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11431 2023-12-07 21:41:27.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-12-07 21:41:27.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-12-07 21:41:33.714212 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-07 21:41:27.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:41:33.714212 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/ovos_audio_transformer_plugin_speechbrain_langdetect/
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2023-12-07 21:41:27.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/ovos_audio_transformer_plugin_speechbrain_langdetect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-07 21:41:29.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/ovos_audio_transformer_plugin_speechbrain_langdetect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:41:33.714212 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-12-07 21:41:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2023-12-07 21:41:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 21:41:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-07 21:41:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-07 21:41:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-07 21:41:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 21:41:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 21:41:33.714212 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3240 2023-12-07 21:41:27.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/setup.py
```

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/LICENSE` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/PKG-INFO` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-audio-transformer-plugin-speechbrain-langdetect
-Version: 0.0.0a8
+Version: 0.0.0a9
 Summary: A speech lang detection plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-audio-transformer-plugin-speechbrain-langdetect
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: ovos plugin
```

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/README.md` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/PKG-INFO` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-audio-transformer-plugin-speechbrain-langdetect
-Version: 0.0.0a8
+Version: 0.0.0a9
 Summary: A speech lang detection plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-audio-transformer-plugin-speechbrain-langdetect
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: ovos plugin
```

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/SOURCES.txt` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a8/setup.py` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a9/setup.py`

 * *Files identical despite different names*


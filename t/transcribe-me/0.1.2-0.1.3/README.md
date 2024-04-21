# Comparing `tmp/transcribe_me-0.1.2.tar.gz` & `tmp/transcribe_me-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transcribe_me-0.1.2.tar", last modified: Sun Apr 21 00:57:54 2024, max compression
+gzip compressed data, was "transcribe_me-0.1.3.tar", last modified: Sun Apr 21 01:13:50 2024, max compression
```

## Comparing `transcribe_me-0.1.2.tar` & `transcribe_me-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:54.575199 transcribe_me-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 00:55:40.000000 transcribe_me-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-04-21 00:57:54.575199 transcribe_me-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-04-21 00:55:40.000000 transcribe_me-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-21 00:55:40.000000 transcribe_me-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 00:57:54.575199 transcribe_me-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:54.571199 transcribe_me-0.1.2/transcribe_me/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-21 00:55:40.000000 transcribe_me-0.1.2/transcribe_me/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-21 00:55:40.000000 transcribe_me-0.1.2/transcribe_me/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-21 00:55:40.000000 transcribe_me-0.1.2/transcribe_me/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:54.575199 transcribe_me-0.1.2/transcribe_me.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-04-21 00:57:54.000000 transcribe_me-0.1.2/transcribe_me.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-21 00:57:54.000000 transcribe_me-0.1.2/transcribe_me.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 00:57:54.000000 transcribe_me-0.1.2/transcribe_me.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-21 00:57:54.000000 transcribe_me-0.1.2/transcribe_me.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-21 00:57:54.000000 transcribe_me-0.1.2/transcribe_me.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 00:57:54.000000 transcribe_me-0.1.2/transcribe_me.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:13:50.563463 transcribe_me-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 01:11:25.000000 transcribe_me-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-04-21 01:13:50.563463 transcribe_me-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-04-21 01:11:25.000000 transcribe_me-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-21 01:11:25.000000 transcribe_me-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 01:13:50.563463 transcribe_me-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:13:50.563463 transcribe_me-0.1.3/transcribe_me/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-21 01:11:25.000000 transcribe_me-0.1.3/transcribe_me/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-21 01:11:25.000000 transcribe_me-0.1.3/transcribe_me/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-21 01:11:25.000000 transcribe_me-0.1.3/transcribe_me/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:13:50.563463 transcribe_me-0.1.3/transcribe_me.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-04-21 01:13:50.000000 transcribe_me-0.1.3/transcribe_me.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-21 01:13:50.000000 transcribe_me-0.1.3/transcribe_me.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 01:13:50.000000 transcribe_me-0.1.3/transcribe_me.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-21 01:13:50.000000 transcribe_me-0.1.3/transcribe_me.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-21 01:13:50.000000 transcribe_me-0.1.3/transcribe_me.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 01:13:50.000000 transcribe_me-0.1.3/transcribe_me.egg-info/top_level.txt
```

### Comparing `transcribe_me-0.1.2/LICENSE` & `transcribe_me-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `transcribe_me-0.1.2/PKG-INFO` & `transcribe_me-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcribe-me
-Version: 0.1.2
+Version: 0.1.3
 Summary: A CLI tool to transcribe audio files using OpenAI API
 Author-email: echoHello <bash@echohello.dev>
 Project-URL: Homepage, https://github.com/echohello-dev/transcribe-me
 Project-URL: Bug Tracker, https://github.com/echohello-dev/transcribe-me/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `transcribe_me-0.1.2/README.md` & `transcribe_me-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `transcribe_me-0.1.2/pyproject.toml` & `transcribe_me-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `transcribe_me-0.1.2/transcribe_me/cli.py` & `transcribe_me-0.1.3/transcribe_me/cli.py`

 * *Files identical despite different names*

### Comparing `transcribe_me-0.1.2/transcribe_me.egg-info/PKG-INFO` & `transcribe_me-0.1.3/transcribe_me.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcribe-me
-Version: 0.1.2
+Version: 0.1.3
 Summary: A CLI tool to transcribe audio files using OpenAI API
 Author-email: echoHello <bash@echohello.dev>
 Project-URL: Homepage, https://github.com/echohello-dev/transcribe-me
 Project-URL: Bug Tracker, https://github.com/echohello-dev/transcribe-me/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


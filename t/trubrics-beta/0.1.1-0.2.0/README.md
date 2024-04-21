# Comparing `tmp/trubrics_beta-0.1.1.tar.gz` & `tmp/trubrics_beta-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trubrics_beta-0.1.1.tar", last modified: Wed Apr 17 16:42:45 2024, max compression
+gzip compressed data, was "trubrics_beta-0.2.0.tar", last modified: Sun Apr 21 12:54:48 2024, max compression
```

## Comparing `trubrics_beta-0.1.1.tar` & `trubrics_beta-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-17 16:42:45.072568 trubrics_beta-0.1.1/
--rw-r--r--   0 jeffkayne   (501) staff       (20)      627 2024-04-17 16:42:45.072322 trubrics_beta-0.1.1/PKG-INFO
--rw-r--r--   0 jeffkayne   (501) staff       (20)      311 2024-04-17 14:52:00.000000 trubrics_beta-0.1.1/README.md
--rw-r--r--   0 jeffkayne   (501) staff       (20)      417 2024-04-17 16:41:39.000000 trubrics_beta-0.1.1/pyproject.toml
--rw-r--r--   0 jeffkayne   (501) staff       (20)       38 2024-04-17 16:42:45.072613 trubrics_beta-0.1.1/setup.cfg
-drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-17 16:42:45.071049 trubrics_beta-0.1.1/trubrics_beta/
--rw-r--r--   0 jeffkayne   (501) staff       (20)      143 2024-04-17 16:37:25.000000 trubrics_beta-0.1.1/trubrics_beta/__init__.py
--rw-r--r--   0 jeffkayne   (501) staff       (20)     2455 2024-04-17 16:26:59.000000 trubrics_beta-0.1.1/trubrics_beta/main.py
-drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-17 16:42:45.072117 trubrics_beta-0.1.1/trubrics_beta.egg-info/
--rw-r--r--   0 jeffkayne   (501) staff       (20)      627 2024-04-17 16:42:45.000000 trubrics_beta-0.1.1/trubrics_beta.egg-info/PKG-INFO
--rw-r--r--   0 jeffkayne   (501) staff       (20)      220 2024-04-17 16:42:45.000000 trubrics_beta-0.1.1/trubrics_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jeffkayne   (501) staff       (20)        1 2024-04-17 16:42:45.000000 trubrics_beta-0.1.1/trubrics_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jeffkayne   (501) staff       (20)       14 2024-04-17 16:42:45.000000 trubrics_beta-0.1.1/trubrics_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-21 12:54:48.322553 trubrics_beta-0.2.0/
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      627 2024-04-21 12:54:48.322357 trubrics_beta-0.2.0/PKG-INFO
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      311 2024-04-18 06:48:42.000000 trubrics_beta-0.2.0/README.md
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      417 2024-04-21 12:46:51.000000 trubrics_beta-0.2.0/pyproject.toml
+-rw-r--r--   0 jeffkayne   (501) staff       (20)       38 2024-04-21 12:54:48.322603 trubrics_beta-0.2.0/setup.cfg
+drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-21 12:54:48.321153 trubrics_beta-0.2.0/trubrics_beta/
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      143 2024-04-18 06:48:42.000000 trubrics_beta-0.2.0/trubrics_beta/__init__.py
+-rw-r--r--   0 jeffkayne   (501) staff       (20)     1373 2024-04-21 12:46:12.000000 trubrics_beta-0.2.0/trubrics_beta/main.py
+drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-21 12:54:48.322139 trubrics_beta-0.2.0/trubrics_beta.egg-info/
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      627 2024-04-21 12:54:48.000000 trubrics_beta-0.2.0/trubrics_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      220 2024-04-21 12:54:48.000000 trubrics_beta-0.2.0/trubrics_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffkayne   (501) staff       (20)        1 2024-04-21 12:54:48.000000 trubrics_beta-0.2.0/trubrics_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffkayne   (501) staff       (20)       14 2024-04-21 12:54:48.000000 trubrics_beta-0.2.0/trubrics_beta.egg-info/top_level.txt
```

### Comparing `trubrics_beta-0.1.1/PKG-INFO` & `trubrics_beta-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trubrics-beta
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python SDK to track events in Trubrics.
 Author-email: Jeff Kayne <jeff.kayne@trubrics.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `trubrics_beta-0.1.1/trubrics_beta.egg-info/PKG-INFO` & `trubrics_beta-0.2.0/trubrics_beta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trubrics-beta
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python SDK to track events in Trubrics.
 Author-email: Jeff Kayne <jeff.kayne@trubrics.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```


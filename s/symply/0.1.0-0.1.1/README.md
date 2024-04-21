# Comparing `tmp/symply-0.1.0.tar.gz` & `tmp/symply-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symply-0.1.0.tar", max compression
+gzip compressed data, was "symply-0.1.1.tar", max compression
```

## Comparing `symply-0.1.0.tar` & `symply-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2024-04-16 00:37:19.582472 symply-0.1.0/LICENSE
--rw-r--r--   0        0        0     2328 2024-04-16 04:44:56.171036 symply-0.1.0/README.md
--rw-r--r--   0        0        0      503 2024-04-16 02:36:04.521784 symply-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      173 2024-04-16 04:36:46.521083 symply-0.1.0/symply/__init__.py
--rw-r--r--   0        0        0     3048 2024-04-16 04:33:17.321103 symply-0.1.0/symply/symply.py
--rw-r--r--   0        0        0     4349 2024-04-16 04:41:26.541056 symply-0.1.0/symply/watcher.py
--rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 symply-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-16 00:37:19.582472 symply-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2328 2024-04-16 04:44:56.171036 symply-0.1.1/README.md
+-rw-r--r--   0        0        0      503 2024-04-21 06:40:14.122415 symply-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      202 2024-04-16 21:57:45.430130 symply-0.1.1/symply/__init__.py
+-rw-r--r--   0        0        0     3930 2024-04-21 06:20:40.692633 symply-0.1.1/symply/symply.py
+-rw-r--r--   0        0        0     4885 2024-04-21 06:22:15.562616 symply-0.1.1/symply/watcher.py
+-rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 symply-0.1.1/PKG-INFO
```

### Comparing `symply-0.1.0/LICENSE` & `symply-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `symply-0.1.0/README.md` & `symply-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `symply-0.1.0/symply/watcher.py` & `symply-0.1.1/symply/watcher.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 """
 Enhanced monitoring module for directory changes and symlink management.
 
 This module provides advanced monitoring capabilities for directories, handling events like creations, deletions, and modifications. It supports filtering events and customizable callbacks for various events.
 
 Example:
-    handler = SymlinkHandler(handle_event)
-    monitor = SymlinkMonitor('/path/to/directory', handler, include_patterns=['*.txt', '*.docx'])
-    monitor.start()
+    >>> handler = SymlinkHandler(handle_event)
+    >>> monitor = SymlinkMonitor('/path/to/directory', handler, include_patterns=['*.txt', '*.docx'])
+    >>> monitor.start()
+
+The `SymlinkMonitor` class allows you to monitor a directory for changes and handle events using a custom event handler. The `SymlinkHandler` class provides a custom event handler for managing symlink-related events and more.
+
+Attributes:
+- `watch_directory` (str): The path to the directory being monitored.
+- `event_handler` (FileSystemEventHandler): The event handler used for managing events.
+- `observer` (Observer): The observer instance used for monitoring.
+- `thread` (Thread): The thread used to run the observer.
 """
 import logging
 import threading
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler, RegexMatchingEventHandler
 
 logger = logging.getLogger(__name__)
```

### Comparing `symply-0.1.0/PKG-INFO` & `symply-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symply
-Version: 0.1.0
+Version: 0.1.1
 Summary: Effortless Symlink Management as a Python Package!
 License: MIT
 Author: Spoked
 Author-email: dreu.lavelle@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


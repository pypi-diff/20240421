# Comparing `tmp/ataskq-0.5.1.tar.gz` & `tmp/ataskq-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ataskq-0.5.1.tar", last modified: Sun Apr 21 07:22:24 2024, max compression
+gzip compressed data, was "ataskq-5.0.0.tar", last modified: Wed Apr 17 20:31:31 2024, max compression
```

## Comparing `ataskq-0.5.1.tar` & `ataskq-5.0.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:22:24.629826 ataskq-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 07:22:11.000000 ataskq-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-21 07:22:24.629826 ataskq-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-21 07:22:11.000000 ataskq-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:22:24.625826 ataskq-0.5.1/ataskq/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12687 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/ataskq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:22:24.625826 ataskq-0.5.1/ataskq/handler/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17044 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/handler/db_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/handler/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/handler/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/handler/rest_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/handler/sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/imodel.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    15869 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:22:24.625826 ataskq-0.5.1/ataskq/server/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/server/form_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:22:24.629826 ataskq-0.5.1/ataskq/server/www/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:22:24.629826 ataskq-0.5.1/ataskq/server/www/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    24285 2024-04-21 07:22:19.000000 ataskq-0.5.1/ataskq/server/www/assets/index-MiCEdQXI.js
--rw-r--r--   0 runner    (1001) docker     (127)    70928 2024-04-21 07:22:19.000000 ataskq-0.5.1/ataskq/server/www/assets/index-MiCEdQXI.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-21 07:22:19.000000 ataskq-0.5.1/ataskq/server/www/assets/index-_NWmBfbC.css
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-21 07:22:19.000000 ataskq-0.5.1/ataskq/server/www/ataskq-32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-21 07:22:19.000000 ataskq-0.5.1/ataskq/server/www/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-21 07:22:19.000000 ataskq-0.5.1/ataskq/server/www/index.html
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 07:22:19.000000 ataskq-0.5.1/ataskq/server/www/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:22:24.629826 ataskq-0.5.1/ataskq/tasks_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/tasks_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/tasks_utils/counter_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/tasks_utils/write_to_file_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/test_0.py
--rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/test_ataskq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-21 07:22:11.000000 ataskq-0.5.1/ataskq/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-21 07:22:19.000000 ataskq-0.5.1/ataskq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:22:24.629826 ataskq-0.5.1/ataskq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-21 07:22:24.000000 ataskq-0.5.1/ataskq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-21 07:22:24.000000 ataskq-0.5.1/ataskq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 07:22:24.000000 ataskq-0.5.1/ataskq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 07:22:24.000000 ataskq-0.5.1/ataskq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-21 07:22:19.000000 ataskq-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 07:22:24.629826 ataskq-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:31:31.907540 ataskq-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-17 20:31:11.000000 ataskq-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-17 20:31:31.907540 ataskq-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-17 20:31:11.000000 ataskq-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:31:31.903540 ataskq-5.0.0/ataskq/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12687 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/ataskq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:31:31.903540 ataskq-5.0.0/ataskq/handler/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17044 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/handler/db_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/handler/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/handler/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/handler/rest_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/handler/sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/imodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15812 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:31:31.903540 ataskq-5.0.0/ataskq/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/server/form_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:31:31.907540 ataskq-5.0.0/ataskq/server/www/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:31:31.907540 ataskq-5.0.0/ataskq/server/www/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    24285 2024-04-17 20:31:20.000000 ataskq-5.0.0/ataskq/server/www/assets/index-MiCEdQXI.js
+-rw-r--r--   0 runner    (1001) docker     (127)    70928 2024-04-17 20:31:20.000000 ataskq-5.0.0/ataskq/server/www/assets/index-MiCEdQXI.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-17 20:31:20.000000 ataskq-5.0.0/ataskq/server/www/assets/index-_NWmBfbC.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-17 20:31:20.000000 ataskq-5.0.0/ataskq/server/www/ataskq-32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-17 20:31:20.000000 ataskq-5.0.0/ataskq/server/www/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-17 20:31:20.000000 ataskq-5.0.0/ataskq/server/www/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 20:31:20.000000 ataskq-5.0.0/ataskq/server/www/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:31:31.907540 ataskq-5.0.0/ataskq/tasks_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/tasks_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/tasks_utils/counter_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/tasks_utils/write_to_file_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/test_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/test_ataskq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 20:31:20.000000 ataskq-5.0.0/ataskq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:31:31.907540 ataskq-5.0.0/ataskq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-17 20:31:31.000000 ataskq-5.0.0/ataskq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-17 20:31:31.000000 ataskq-5.0.0/ataskq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:31:31.000000 ataskq-5.0.0/ataskq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 20:31:31.000000 ataskq-5.0.0/ataskq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-17 20:31:20.000000 ataskq-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:31:31.907540 ataskq-5.0.0/setup.cfg
```

### Comparing `ataskq-0.5.1/LICENSE` & `ataskq-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/PKG-INFO` & `ataskq-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ataskq
-Version: 0.5.1
+Version: 5.0.0
 Summary: An in process task queue for distributed computing systems.
 Project-URL: Homepage, https://github.com/innoviz-swt/a-task-queue
 Project-URL: Issues, https://github.com/innoviz-swt/a-task-queue/issues
 Keywords: python,task,queue,distributed systems,distributed computing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ataskq-0.5.1/README.md` & `ataskq-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/ataskq.py` & `ataskq-5.0.0/ataskq/ataskq.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/conftest.py` & `ataskq-5.0.0/ataskq/conftest.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/env.py` & `ataskq-5.0.0/ataskq/env.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/handler/db_handler.py` & `ataskq-5.0.0/ataskq/handler/db_handler.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/handler/handler.py` & `ataskq-5.0.0/ataskq/handler/handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,17 +53,14 @@
 
 
 class EAction(str, Enum):
     RUN_TASK = "run_task"
     WAIT = "wait"
     STOP = "stop"
 
-    def __str__(self) -> str:
-        return self.value
-
 
 class Handler(IModelSerializer, Logger):
     def __init__(self, logger: Logger = None):
         Logger.__init__(self, logger)
 
     ######################
     # interface handlers #
```

### Comparing `ataskq-0.5.1/ataskq/handler/postgresql.py` & `ataskq-5.0.0/ataskq/handler/postgresql.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/handler/rest_handler.py` & `ataskq-5.0.0/ataskq/handler/rest_handler.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/handler/sqlite3.py` & `ataskq-5.0.0/ataskq/handler/sqlite3.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/imodel.py` & `ataskq-5.0.0/ataskq/imodel.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/logger.py` & `ataskq-5.0.0/ataskq/logger.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/models.py` & `ataskq-5.0.0/ataskq/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,14 @@
 
 class EStatus(str, Enum):
     PENDING = "pending"
     RUNNING = "running"
     SUCCESS = "success"
     FAILURE = "failure"
 
-    def __str__(self) -> str:
-        return self.value
-
 
 class EntryPoint:
     @staticmethod
     def init(kwargs) -> None:
         entrypoint = kwargs.get("entrypoint")
         if callable(entrypoint):
             kwargs["entrypoint"] = f"{entrypoint.__module__}.{entrypoint.__name__}"
```

### Comparing `ataskq-0.5.1/ataskq/monitor.py` & `ataskq-5.0.0/ataskq/monitor.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/server/form_utils.py` & `ataskq-5.0.0/ataskq/server/form_utils.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/server/server.py` & `ataskq-5.0.0/ataskq/server/server.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/server/www/assets/index-MiCEdQXI.js` & `ataskq-5.0.0/ataskq/server/www/assets/index-MiCEdQXI.js`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/server/www/assets/index-MiCEdQXI.js.map` & `ataskq-5.0.0/ataskq/server/www/assets/index-MiCEdQXI.js.map`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/server/www/assets/index-_NWmBfbC.css` & `ataskq-5.0.0/ataskq/server/www/assets/index-_NWmBfbC.css`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/server/www/ataskq-32.png` & `ataskq-5.0.0/ataskq/server/www/ataskq-32.png`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/server/www/favicon.ico` & `ataskq-5.0.0/ataskq/server/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/server/www/index.html` & `ataskq-5.0.0/ataskq/server/www/index.html`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/tasks_utils/counter_task.py` & `ataskq-5.0.0/ataskq/tasks_utils/counter_task.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/test_ataskq.py` & `ataskq-5.0.0/ataskq/test_ataskq.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/test_handler.py` & `ataskq-5.0.0/ataskq/test_handler.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/test_models.py` & `ataskq-5.0.0/ataskq/test_models.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq/test_queries.py` & `ataskq-5.0.0/ataskq/test_queries.py`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/ataskq.egg-info/PKG-INFO` & `ataskq-5.0.0/ataskq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ataskq
-Version: 0.5.1
+Version: 5.0.0
 Summary: An in process task queue for distributed computing systems.
 Project-URL: Homepage, https://github.com/innoviz-swt/a-task-queue
 Project-URL: Issues, https://github.com/innoviz-swt/a-task-queue/issues
 Keywords: python,task,queue,distributed systems,distributed computing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ataskq-0.5.1/ataskq.egg-info/SOURCES.txt` & `ataskq-5.0.0/ataskq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ataskq-0.5.1/pyproject.toml` & `ataskq-5.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ataskq"
-version = "0.5.1"
+version = "5.0.0"
 description = "An in process task queue for distributed computing systems."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```


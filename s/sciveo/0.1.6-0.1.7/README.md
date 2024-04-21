# Comparing `tmp/sciveo-0.1.6.tar.gz` & `tmp/sciveo-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciveo-0.1.6.tar", last modified: Fri Apr 19 15:01:01 2024, max compression
+gzip compressed data, was "sciveo-0.1.7.tar", last modified: Sun Apr 21 12:24:13 2024, max compression
```

## Comparing `sciveo-0.1.6.tar` & `sciveo-0.1.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 15:01:01.838385 sciveo-0.1.6/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6753 2024-04-19 15:01:01.838252 sciveo-0.1.6/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6601 2024-04-19 06:47:05.000000 sciveo-0.1.6/README.md
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 15:01:01.814143 sciveo-0.1.6/sciveo/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1428 2024-04-17 12:51:40.000000 sciveo-0.1.6/sciveo/__init__.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 15:01:01.821567 sciveo-0.1.6/sciveo/api/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.1.6/sciveo/api/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-16 17:39:04.000000 sciveo-0.1.6/sciveo/api/base.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.1.6/sciveo/api/upload.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 15:01:01.825948 sciveo-0.1.6/sciveo/common/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.1.6/sciveo/common/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.1.6/sciveo/common/configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.1.6/sciveo/common/model.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.1.6/sciveo/common/optimizers.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.1.6/sciveo/common/sampling.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 15:01:01.829783 sciveo-0.1.6/sciveo/common/tools/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.1.6/sciveo/common/tools/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1647 2024-04-17 12:51:40.000000 sciveo-0.1.6/sciveo/common/tools/daemon.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.1.6/sciveo/common/tools/formating.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-17 13:30:32.000000 sciveo-0.1.6/sciveo/common/tools/hardware.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.1.6/sciveo/common/tools/logger.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1333 2024-04-17 12:51:40.000000 sciveo-0.1.6/sciveo/common/tools/synchronized.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1087 2024-04-17 12:51:40.000000 sciveo-0.1.6/sciveo/common/tools/timers.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 15:01:01.833694 sciveo-0.1.6/sciveo/content/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.1.6/sciveo/content/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.1.6/sciveo/content/dataset.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.1.6/sciveo/content/experiment.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.1.6/sciveo/content/project.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.1.6/sciveo/content/runner.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 15:01:01.834745 sciveo-0.1.6/sciveo/monitoring/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.1.6/sciveo/monitoring/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5900 2024-04-19 15:00:07.000000 sciveo-0.1.6/sciveo/monitoring/monitor.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2564 2024-04-17 12:51:40.000000 sciveo-0.1.6/sciveo/monitoring/network.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1671 2024-04-17 12:51:40.000000 sciveo-0.1.6/sciveo/monitoring/start.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       23 2024-04-19 14:59:57.000000 sciveo-0.1.6/sciveo/version.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 15:01:01.818855 sciveo-0.1.6/sciveo.egg-info/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6753 2024-04-19 15:01:01.000000 sciveo-0.1.6/sciveo.egg-info/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      965 2024-04-19 15:01:01.000000 sciveo-0.1.6/sciveo.egg-info/SOURCES.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-19 15:01:01.000000 sciveo-0.1.6/sciveo.egg-info/dependency_links.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      112 2024-04-19 15:01:01.000000 sciveo-0.1.6/sciveo.egg-info/requires.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-19 15:01:01.000000 sciveo-0.1.6/sciveo.egg-info/top_level.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-19 15:01:01.838432 sciveo-0.1.6/setup.cfg
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      778 2024-04-17 12:51:40.000000 sciveo-0.1.6/setup.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 15:01:01.837840 sciveo-0.1.6/test/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.1.6/test/test_configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.1.6/test/test_monitoring.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.1.6/test/test_runner.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.1.6/test/test_sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.653784 sciveo-0.1.7/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6753 2024-04-21 12:24:13.653586 sciveo-0.1.7/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6601 2024-04-19 15:11:15.000000 sciveo-0.1.7/README.md
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.569367 sciveo-0.1.7/sciveo/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1428 2024-04-17 12:51:40.000000 sciveo-0.1.7/sciveo/__init__.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.619179 sciveo-0.1.7/sciveo/api/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.1.7/sciveo/api/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-16 17:39:04.000000 sciveo-0.1.7/sciveo/api/base.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.1.7/sciveo/api/upload.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.623110 sciveo-0.1.7/sciveo/common/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.1.7/sciveo/common/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.1.7/sciveo/common/configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.1.7/sciveo/common/model.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.1.7/sciveo/common/optimizers.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.1.7/sciveo/common/sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.637089 sciveo-0.1.7/sciveo/common/tools/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.1.7/sciveo/common/tools/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1647 2024-04-17 12:51:40.000000 sciveo-0.1.7/sciveo/common/tools/daemon.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.1.7/sciveo/common/tools/formating.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-21 12:16:37.000000 sciveo-0.1.7/sciveo/common/tools/hardware.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.1.7/sciveo/common/tools/logger.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1333 2024-04-17 12:51:40.000000 sciveo-0.1.7/sciveo/common/tools/synchronized.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1087 2024-04-17 12:51:40.000000 sciveo-0.1.7/sciveo/common/tools/timers.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.647061 sciveo-0.1.7/sciveo/content/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.1.7/sciveo/content/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.1.7/sciveo/content/dataset.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.1.7/sciveo/content/experiment.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.1.7/sciveo/content/project.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.1.7/sciveo/content/runner.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.650354 sciveo-0.1.7/sciveo/monitoring/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.1.7/sciveo/monitoring/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5898 2024-04-21 12:22:43.000000 sciveo-0.1.7/sciveo/monitoring/monitor.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3790 2024-04-21 07:50:35.000000 sciveo-0.1.7/sciveo/monitoring/network.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1671 2024-04-17 12:51:40.000000 sciveo-0.1.7/sciveo/monitoring/start.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       23 2024-04-21 12:24:10.000000 sciveo-0.1.7/sciveo/version.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.616927 sciveo-0.1.7/sciveo.egg-info/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6753 2024-04-21 12:24:13.000000 sciveo-0.1.7/sciveo.egg-info/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      965 2024-04-21 12:24:13.000000 sciveo-0.1.7/sciveo.egg-info/SOURCES.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-21 12:24:13.000000 sciveo-0.1.7/sciveo.egg-info/dependency_links.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      112 2024-04-21 12:24:13.000000 sciveo-0.1.7/sciveo.egg-info/requires.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-21 12:24:13.000000 sciveo-0.1.7/sciveo.egg-info/top_level.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-21 12:24:13.653845 sciveo-0.1.7/setup.cfg
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      778 2024-04-17 12:51:40.000000 sciveo-0.1.7/setup.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-21 12:24:13.653228 sciveo-0.1.7/test/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.1.7/test/test_configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.1.7/test/test_monitoring.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.1.7/test/test_runner.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.1.7/test/test_sampling.py
```

### Comparing `sciveo-0.1.6/PKG-INFO` & `sciveo-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.1.6
+Version: 0.1.7
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 Provides-Extra: net
 Provides-Extra: all
 
 # SCIVEO - ML/AI and Scientific tools
```

### Comparing `sciveo-0.1.6/README.md` & `sciveo-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/__init__.py` & `sciveo-0.1.7/sciveo/__init__.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/api/base.py` & `sciveo-0.1.7/sciveo/api/base.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/api/upload.py` & `sciveo-0.1.7/sciveo/api/upload.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/common/configuration.py` & `sciveo-0.1.7/sciveo/common/configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/common/model.py` & `sciveo-0.1.7/sciveo/common/model.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/common/optimizers.py` & `sciveo-0.1.7/sciveo/common/optimizers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/common/sampling.py` & `sciveo-0.1.7/sciveo/common/sampling.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/common/tools/daemon.py` & `sciveo-0.1.7/sciveo/common/tools/daemon.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/common/tools/formating.py` & `sciveo-0.1.7/sciveo/common/tools/formating.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/common/tools/hardware.py` & `sciveo-0.1.7/sciveo/common/tools/hardware.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/common/tools/logger.py` & `sciveo-0.1.7/sciveo/common/tools/logger.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/common/tools/synchronized.py` & `sciveo-0.1.7/sciveo/common/tools/synchronized.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/common/tools/timers.py` & `sciveo-0.1.7/sciveo/common/tools/timers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/content/dataset.py` & `sciveo-0.1.7/sciveo/content/dataset.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/content/experiment.py` & `sciveo-0.1.7/sciveo/content/experiment.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/content/project.py` & `sciveo-0.1.7/sciveo/content/project.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/content/runner.py` & `sciveo-0.1.7/sciveo/content/runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo/monitoring/monitor.py` & `sciveo-0.1.7/sciveo/monitoring/monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,21 +42,25 @@
     return re.sub(r'[\s,]', '', machine_serial)
 
 
 class BaseMonitor(DaemonBase):
   def __init__(self, period=5):
     super().__init__(period=period)
 
-    self.data = HardwareInfo()()
-    self.data.setdefault("CPU", {})
-    self.data.setdefault("DISK", {})
-    self.data.setdefault("NET", {})
-    self.data.setdefault("TEMP", {})
-    self.data["RAM"] = {}
-    self.data["LOG"] = {}
+    self.data = {
+      "CPU": {},
+      "RAM": {},
+      "DISK": {},
+      "NET": {},
+      "TEMP": {},
+      "LOG": {},
+      "INFO": {},
+    }
+    self.data["INFO"] = HardwareInfo()()
+    self.data["INFO"].setdefault("CPU", {})
     self.list_logs = []
 
     self.api = APIRemoteClient()
 
     # Warmup the psutil
     psutil.cpu_percent(interval=0.3, percpu=True)
     initial_cpu_usage = psutil.cpu_percent(interval=None, percpu=True)
@@ -112,15 +116,15 @@
   def get_memory(self):
     try:
       memory = psutil.virtual_memory()
       self.data["RAM"]["used"] = memory.used
       self.data["RAM"]["total"] = memory.total
       self.data["RAM"]["free"] = memory.free
       # self.data["RAM"]["installed"] = format_memory_size(memory.total)
-      self.data["RAM"]["print"] = f"total: {format_memory_size(memory.total)} used: {format_memory_size(memory.used)}"
+      self.data["INFO"]["RAM"] = f"total: {format_memory_size(memory.total)} used: {format_memory_size(memory.used)}"
     except Exception:
       pass
 
   def tail_file(self, file_path, block_size=1024):
     result = ["EMPTY"]
     try:
       with open(file_path,'rb') as fp:
@@ -152,15 +156,15 @@
   def get_disk(self):
     try:
       list_metrics = ["read bytes", "write bytes", "read count", "write count", "read time", "write time"]
       disk_io_counters = psutil.disk_io_counters(perdisk=False)
       self.get_io_metrics("DISK", list_metrics, disk_io_counters)
 
       disk_usage = psutil.disk_usage('/')._asdict()
-      self.data["DISK"]["print"] = f"{disk_usage['percent']}% ({round(disk_usage['used'] / (1024 * 1024 * 1024), 1)} GB / {round(disk_usage['total'] / (1024 * 1024 * 1024), 1)} GB)"
+      self.data["INFO"]["DISK"] = f"{disk_usage['percent']}% ({round(disk_usage['used'] / (1024 * 1024 * 1024), 1)} GB / {round(disk_usage['total'] / (1024 * 1024 * 1024), 1)} GB)"
     except Exception as e:
       pass
 
   def get_network(self):
     try:
       list_metrics = ["bytes sent", "bytes recv", "packets sent", "packets recv"]
       net_io_counters = psutil.net_io_counters(pernic=False)
```

### Comparing `sciveo-0.1.6/sciveo/monitoring/network.py` & `sciveo-0.1.7/sciveo/monitoring/network.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,19 +6,49 @@
 # from the owner. For licensing inquiries, please
 # contact pavlin@softel.bg.
 #
 # 2024
 #
 
 import socket
+import asyncio
 
 from sciveo.common.tools.logger import *
 from sciveo.common.tools.timers import Timer
 
 
+class NetworkScanner:
+  def __init__(self, timeout=1.0):
+    self.timeout = timeout
+
+  async def scan_port(self, ip, port):
+    try:
+      reader, writer = await asyncio.wait_for(asyncio.open_connection(ip, port), timeout=self.timeout)
+      writer.close()
+      await writer.wait_closed()
+      return (ip, port)
+    except Exception as e:
+      # print("Exception", e)
+      return None
+
+  async def scan_all_ports(self, ip, ports):
+    tasks = [self.scan_port(ip, port) for port in ports]
+    return await asyncio.gather(*tasks)
+
+  async def scan_async(self, ips, ports):
+    results = []
+    for ip in ips:
+      results.extend(await self.scan_all_ports(ip, ports))
+    results = [x for x in results if x is not None]
+    return results
+
+  def scan(self, ips, ports):
+    return asyncio.run(self.scan_async(ips, ports))
+
+
 class NetworkTools:
   def __init__(self, **kwargs):
     self.default_arguments = {
       "timeout": 0.1,
       "localhost": False,
     }
 
@@ -77,10 +107,24 @@
           # debug(type(self).__name__, "scan_ports", ip, port, result)
       except socket.error:
         pass
     return list_hosts
 
 
 if __name__ == "__main__":
-  net = NetworkTools(timeout=0.01, localhost=True)
-  list_hosts = net.scan_port(port=22)
-  print(list_hosts)
+  t1 = Timer()
+  net = NetworkTools(timeout=0.5, localhost=True)
+  result = net.scan_port(port=22)
+  t1 = t1.stop()
+  print(result, "elapsed", t1)
+
+  t2 = Timer()
+  list_local_ips = net.get_local_nets()
+  list_scan_ips = []
+  for local_ip in list_local_ips:
+    list_scan_ips += net.generate_ip_list(local_ip)
+  # print(list_scan_ips)
+  ns = NetworkScanner(timeout=0.5)
+  result = ns.scan(list_scan_ips, [22])
+  t2 = t2.stop()
+  print(result, "elapsed", t2)
+  print("elapsed", t1, t2, t1 - t2)
```

### Comparing `sciveo-0.1.6/sciveo/monitoring/start.py` & `sciveo-0.1.7/sciveo/monitoring/start.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/sciveo.egg-info/PKG-INFO` & `sciveo-0.1.7/sciveo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.1.6
+Version: 0.1.7
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 Provides-Extra: net
 Provides-Extra: all
 
 # SCIVEO - ML/AI and Scientific tools
```

### Comparing `sciveo-0.1.6/sciveo.egg-info/SOURCES.txt` & `sciveo-0.1.7/sciveo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/setup.py` & `sciveo-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/test/test_configuration.py` & `sciveo-0.1.7/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/test/test_monitoring.py` & `sciveo-0.1.7/test/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/test/test_runner.py` & `sciveo-0.1.7/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.6/test/test_sampling.py` & `sciveo-0.1.7/test/test_sampling.py`

 * *Files identical despite different names*


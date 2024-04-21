# Comparing `tmp/PKDevTools-0.13.20240419.98.tar.gz` & `tmp/PKDevTools-0.13.20240421.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240419.98.tar", last modified: Fri Apr 19 10:09:32 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240421.99.tar", last modified: Sun Apr 21 00:32:30 2024, max compression
```

## Comparing `PKDevTools-0.13.20240419.98.tar` & `PKDevTools-0.13.20240421.99.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 10:09:32.765119 PKDevTools-0.13.20240419.98/
--rw-rw-rw-   0        0        0     1086 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-19 10:09:32.749506 PKDevTools-0.13.20240419.98/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 10:09:32.765119 PKDevTools-0.13.20240419.98/PKDevTools/classes/
--rw-rw-rw-   0        0        0     3402 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     5095 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6380 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11963 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     2534 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/OutputControls.py
--rw-rw-rw-   0        0        0    13778 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     8048 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14334 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     1916 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11301 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       27 2024-04-19 10:09:27.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16118 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     5384 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-04-19 10:09:32.749506 PKDevTools-0.13.20240419.98/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5202 2024-04-19 10:09:32.000000 PKDevTools-0.13.20240419.98/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1084 2024-04-19 10:09:32.000000 PKDevTools-0.13.20240419.98/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 10:09:32.000000 PKDevTools-0.13.20240419.98/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-04-19 10:09:32.000000 PKDevTools-0.13.20240419.98/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-19 10:09:26.000000 PKDevTools-0.13.20240419.98/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      176 2024-04-19 10:09:32.000000 PKDevTools-0.13.20240419.98/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-19 10:09:32.000000 PKDevTools-0.13.20240419.98/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5202 2024-04-19 10:09:32.765119 PKDevTools-0.13.20240419.98/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/README.md
--rw-rw-rw-   0        0        0       86 2024-04-19 10:09:32.765119 PKDevTools-0.13.20240419.98/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-04-19 10:08:30.000000 PKDevTools-0.13.20240419.98/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:32:30.822920 PKDevTools-0.13.20240421.99/
+-rw-rw-rw-   0        0        0     1086 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-21 00:32:30.807309 PKDevTools-0.13.20240421.99/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:32:30.822920 PKDevTools-0.13.20240421.99/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     3402 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     5095 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6380 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11963 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     2534 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    13778 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     8346 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14334 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     1916 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11301 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       27 2024-04-21 00:32:26.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16118 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     5384 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:32:30.807309 PKDevTools-0.13.20240421.99/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5202 2024-04-21 00:32:30.000000 PKDevTools-0.13.20240421.99/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1084 2024-04-21 00:32:30.000000 PKDevTools-0.13.20240421.99/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 00:32:30.000000 PKDevTools-0.13.20240421.99/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-04-21 00:32:30.000000 PKDevTools-0.13.20240421.99/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-21 00:32:24.000000 PKDevTools-0.13.20240421.99/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      176 2024-04-21 00:32:30.000000 PKDevTools-0.13.20240421.99/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-21 00:32:30.000000 PKDevTools-0.13.20240421.99/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5202 2024-04-21 00:32:30.822920 PKDevTools-0.13.20240421.99/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-21 00:32:30.822920 PKDevTools-0.13.20240421.99/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-04-21 00:31:22.000000 PKDevTools-0.13.20240421.99/setup.py
```

### Comparing `PKDevTools-0.13.20240419.98/LICENSE` & `PKDevTools-0.13.20240421.99/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/__init__.py` & `PKDevTools-0.13.20240421.99/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/OutputControls.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/OutputControls.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/PKDateUtilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,15 @@
         # or hostRef.processingResultsCounter
         self.processingCounter = processingCounter
         self.processingResultsCounter = processingResultsCounter
         # A helper object dictionary that can contain anything
         # and can be accessed using hostRef.objectDictionary
         # within processorMethod
         self.objectDictionary = objectDictionary
+        self.secondaryObjectDictionary = objectDictionary
         # A proxyServer that can contain proxyServer info
         # and can be accessed using hostRef.proxyServer
         # within processorMethod
         self.proxyServer = proxyServer
         # A logger that can contain logger reference
         # and can be accessed using hostRef.default_logger
         # within processorMethod
@@ -115,14 +116,17 @@
         try:
             if isinstance(self.objectDictionary,str):
                 # Looks like we got the filename instead of stock dictionary
                 # Let's load the saved stocks' data
                 cache_file = self.objectDictionary
                 with open(os.path.join(Archiver.get_user_outputs_dir(), cache_file), "rb") as f:
                     self.objectDictionary = pickle.load(f)
+                if "intraday" not in cache_file:
+                    with open(os.path.join(Archiver.get_user_outputs_dir(), f"intraday_{cache_file}"), "rb") as f:
+                        self.secondaryObjectDictionary = pickle.load(f)
         except:
             pass
         try:
             while not self.keyboardInterruptEvent.is_set():
                 try:
                     next_task = None
                     answer = None
```

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240421.99/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240421.99/PKDevTools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240419.98
+Version: 0.13.20240421.99
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240419.98.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240421.99.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240419.98/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240421.99/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/PKG-INFO` & `PKDevTools-0.13.20240421.99/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240419.98
+Version: 0.13.20240421.99
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240419.98.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240421.99.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240419.98/README.md` & `PKDevTools-0.13.20240421.99/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240419.98/setup.py` & `PKDevTools-0.13.20240421.99/setup.py`

 * *Files identical despite different names*


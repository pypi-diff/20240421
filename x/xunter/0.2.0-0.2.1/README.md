# Comparing `tmp/xunter-0.2.0.tar.gz` & `tmp/xunter-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xunter-0.2.0.tar", last modified: Fri Apr 19 14:19:00 2024, max compression
+gzip compressed data, was "xunter-0.2.1.tar", last modified: Sun Apr 21 12:33:58 2024, max compression
```

## Comparing `xunter-0.2.0.tar` & `xunter-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:00.708860 xunter-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-19 14:18:56.000000 xunter-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 14:18:56.000000 xunter-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-19 14:19:00.708860 xunter-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-19 14:18:56.000000 xunter-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:19:00.708860 xunter-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-19 14:18:56.000000 xunter-0.2.0/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3187 2024-04-19 14:18:56.000000 xunter-0.2.0/xunter
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:00.708860 xunter-0.2.0/xunter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-19 14:19:00.000000 xunter-0.2.0/xunter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-19 14:19:00.000000 xunter-0.2.0/xunter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:19:00.000000 xunter-0.2.0/xunter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 14:19:00.000000 xunter-0.2.0/xunter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 14:19:00.000000 xunter-0.2.0/xunter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-04-19 14:18:56.000000 xunter-0.2.0/xunter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-04-19 14:18:56.000000 xunter-0.2.0/xunter2excel
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:33:58.460224 xunter-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 12:33:51.000000 xunter-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-21 12:33:51.000000 xunter-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-21 12:33:58.460224 xunter-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-21 12:33:51.000000 xunter-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 12:33:58.460224 xunter-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-21 12:33:51.000000 xunter-0.2.1/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3187 2024-04-21 12:33:51.000000 xunter-0.2.1/xunter
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:33:58.460224 xunter-0.2.1/xunter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-21 12:33:58.000000 xunter-0.2.1/xunter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-21 12:33:58.000000 xunter-0.2.1/xunter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 12:33:58.000000 xunter-0.2.1/xunter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 12:33:58.000000 xunter-0.2.1/xunter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 12:33:58.000000 xunter-0.2.1/xunter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-04-21 12:33:51.000000 xunter-0.2.1/xunter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-04-21 12:33:51.000000 xunter-0.2.1/xunter2excel
```

### Comparing `xunter-0.2.0/LICENSE` & `xunter-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xunter-0.2.0/PKG-INFO` & `xunter-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xunter
-Version: 0.2.0
+Version: 0.2.1
 Summary: Profiling for the xonsh shell based on hunter.
 Home-page: https://github.com/anki-code/xunter
 Author: anki-code
 Author-email: no@no.no
 License: MIT
 Project-URL: Documentation, https://github.com/anki-code/xunter/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xunter
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xunter Version: 0.2.0 Summary: Profiling for the
+Metadata-Version: 2.1 Name: xunter Version: 0.2.1 Summary: Profiling for the
 xonsh shell based on hunter. Home-page: https://github.com/anki-code/xunter
 Author: anki-code Author-email: no@no.no License: MIT Project-URL:
 Documentation, https://github.com/anki-code/xunter/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xunter Project-URL: Issue
 tracker, https://github.com/anki-code/xunter/issues Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `xunter-0.2.0/README.md` & `xunter-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `xunter-0.2.0/setup.py` & `xunter-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 except (IOError, OSError):
     long_description = ''
 
 setuptools.setup(
     name='xunter',
-    version='0.2.0',
+    version='0.2.1',
     license='MIT',
     author='anki-code',
     author_email='no@no.no',
     description="Profiling for the xonsh shell based on hunter.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.6',
```

### Comparing `xunter-0.2.0/xunter` & `xunter-0.2.1/xunter`

 * *Files identical despite different names*

### Comparing `xunter-0.2.0/xunter.egg-info/PKG-INFO` & `xunter-0.2.1/xunter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xunter
-Version: 0.2.0
+Version: 0.2.1
 Summary: Profiling for the xonsh shell based on hunter.
 Home-page: https://github.com/anki-code/xunter
 Author: anki-code
 Author-email: no@no.no
 License: MIT
 Project-URL: Documentation, https://github.com/anki-code/xunter/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xunter
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xunter Version: 0.2.0 Summary: Profiling for the
+Metadata-Version: 2.1 Name: xunter Version: 0.2.1 Summary: Profiling for the
 xonsh shell based on hunter. Home-page: https://github.com/anki-code/xunter
 Author: anki-code Author-email: no@no.no License: MIT Project-URL:
 Documentation, https://github.com/anki-code/xunter/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xunter Project-URL: Issue
 tracker, https://github.com/anki-code/xunter/issues Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `xunter-0.2.0/xunter.py` & `xunter-0.2.1/xunter.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     def __init__(self, *args, **kwargs):
         # <profile>
         self.timings = {}
         # </profile>
 
         if self.overwrite_stream:
-            args['stream'] = self.overwrite_stream
+            kwargs['stream'] = self.overwrite_stream
 
         super(CallPrinterProfile, self).__init__(*args, **kwargs)
 
     def __call__(self, event):
         """
         Handle event and print filename, line number and source code. If event.kind is a `return` or `exception` also
         prints values.
```

### Comparing `xunter-0.2.0/xunter2excel` & `xunter-0.2.1/xunter2excel`

 * *Files identical despite different names*


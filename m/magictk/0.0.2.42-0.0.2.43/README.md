# Comparing `tmp/magictk-0.0.2.42.tar.gz` & `tmp/magictk-0.0.2.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-0.0.2.42.tar", last modified: Sat Apr 20 10:07:06 2024, max compression
+gzip compressed data, was "magictk-0.0.2.43.tar", last modified: Sat Apr 20 11:01:19 2024, max compression
```

## Comparing `magictk-0.0.2.42.tar` & `magictk-0.0.2.43.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 10:07:06.067696 magictk-0.0.2.42/
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-20 10:07:05.000000 magictk-0.0.2.42/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-20 10:07:06.067696 magictk-0.0.2.42/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1376 2024-04-20 10:07:05.000000 magictk-0.0.2.42/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 10:07:06.063696 magictk-0.0.2.42/magictk/
--rw-r--r--   0 root         (0) root         (0)      359 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9695 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/_window_ctl.py
--rw-r--r--   0 root         (0) root         (0)    13250 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/_window_size.py
--rw-r--r--   0 root         (0) root         (0)     3253 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/basicwindow.py
--rw-r--r--   0 root         (0) root         (0)    13450 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/button.py
--rw-r--r--   0 root         (0) root         (0)    11146 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/checkbox.py
--rw-r--r--   0 root         (0) root         (0)     1919 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/color_tmpl.py
--rw-r--r--   0 root         (0) root         (0)    12040 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/entry.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/fontconfig.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/frame.py
--rw-r--r--   0 root         (0) root         (0)    15906 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/icon.ico
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/photoload.py
--rw-r--r--   0 root         (0) root         (0)     5893 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/progressbar.py
--rw-r--r--   0 root         (0) root         (0)    21933 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/res.pickle
--rw-r--r--   0 root         (0) root         (0)     6077 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/select.py
--rw-r--r--   0 root         (0) root         (0)    11076 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/submenu.py
--rw-r--r--   0 root         (0) root         (0)    10213 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/window.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 10:07:06.067696 magictk-0.0.2.42/magictk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      552 2024-04-20 10:07:06.000000 magictk-0.0.2.42/magictk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-20 10:07:05.000000 magictk-0.0.2.42/magictk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 10:07:06.067696 magictk-0.0.2.42/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1127 2024-04-20 10:07:05.000000 magictk-0.0.2.42/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 11:01:19.976812 magictk-0.0.2.43/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-20 11:01:19.000000 magictk-0.0.2.43/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-20 11:01:19.976812 magictk-0.0.2.43/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1376 2024-04-20 11:01:19.000000 magictk-0.0.2.43/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 11:01:19.976812 magictk-0.0.2.43/magictk/
+-rw-r--r--   0 root         (0) root         (0)      359 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9695 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/_window_ctl.py
+-rw-r--r--   0 root         (0) root         (0)    13250 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/_window_size.py
+-rw-r--r--   0 root         (0) root         (0)     3253 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/basicwindow.py
+-rw-r--r--   0 root         (0) root         (0)    13450 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/button.py
+-rw-r--r--   0 root         (0) root         (0)    11146 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/color_tmpl.py
+-rw-r--r--   0 root         (0) root         (0)    12040 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/entry.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/fontconfig.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/frame.py
+-rw-r--r--   0 root         (0) root         (0)    15906 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/icon.ico
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/mtk.py
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/photoload.py
+-rw-r--r--   0 root         (0) root         (0)     5893 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/progressbar.py
+-rw-r--r--   0 root         (0) root         (0)    21933 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/res.pickle
+-rw-r--r--   0 root         (0) root         (0)     6077 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/select.py
+-rw-r--r--   0 root         (0) root         (0)    11076 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/submenu.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/window.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 11:01:19.976812 magictk-0.0.2.43/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      569 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-20 11:01:19.000000 magictk-0.0.2.43/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 11:01:19.976812 magictk-0.0.2.43/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-20 11:01:19.000000 magictk-0.0.2.43/setup.py
```

### Comparing `magictk-0.0.2.42/PKG-INFO` & `magictk-0.0.2.43/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.42
+Version: 0.0.2.43
 Summary: A tkinter weights looks like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-0.0.2.42/README.md` & `magictk-0.0.2.43/README.md`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.42/magictk/_window_ctl.py` & `magictk-0.0.2.43/magictk/_window_ctl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.42/magictk/_window_size.py` & `magictk-0.0.2.43/magictk/_window_size.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.42/magictk/basicwindow.py` & `magictk-0.0.2.43/magictk/basicwindow.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.42/magictk/button.py` & `magictk-0.0.2.43/magictk/button.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.42/magictk/checkbox.py` & `magictk-0.0.2.43/magictk/checkbox.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.42/magictk/color_tmpl.py` & `magictk-0.0.2.43/magictk/color_tmpl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.42/magictk/entry.py` & `magictk-0.0.2.43/magictk/entry.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.42/magictk/fontconfig.py` & `magictk-0.0.2.43/magictk/fontconfig.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.42/magictk/icon.ico` & `magictk-0.0.2.43/magictk/icon.ico`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.42/magictk/photoload.py` & `magictk-0.0.2.43/magictk/photoload.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.42/magictk/progressbar.py` & `magictk-0.0.2.43/magictk/progressbar.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.42/magictk/res.pickle` & `magictk-0.0.2.43/magictk/res.pickle`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.42/magictk/select.py` & `magictk-0.0.2.43/magictk/select.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.42/magictk/submenu.py` & `magictk-0.0.2.43/magictk/submenu.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.42/magictk/window.py` & `magictk-0.0.2.43/magictk/window.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.42/magictk/workspace.py` & `magictk-0.0.2.43/magictk/workspace.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.42/magictk.egg-info/PKG-INFO` & `magictk-0.0.2.43/magictk.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.42
+Version: 0.0.2.43
 Summary: A tkinter weights looks like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-0.0.2.42/magictk.egg-info/SOURCES.txt` & `magictk-0.0.2.43/magictk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 ./magictk/button.py
 ./magictk/checkbox.py
 ./magictk/color_tmpl.py
 ./magictk/entry.py
 ./magictk/fontconfig.py
 ./magictk/frame.py
 ./magictk/icon.ico
+./magictk/mtk.py
 ./magictk/photoload.py
 ./magictk/progressbar.py
 ./magictk/res.pickle
 ./magictk/select.py
 ./magictk/submenu.py
 ./magictk/window.py
 ./magictk/workspace.py
```

### Comparing `magictk-0.0.2.42/setup.py` & `magictk-0.0.2.43/setup.py`

 * *Files identical despite different names*


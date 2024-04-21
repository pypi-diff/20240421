# Comparing `tmp/magictk-0.0.2.44.tar.gz` & `tmp/magictk-0.0.2.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-0.0.2.44.tar", last modified: Sun Apr 21 03:12:20 2024, max compression
+gzip compressed data, was "magictk-0.0.2.45.tar", last modified: Sun Apr 21 08:13:04 2024, max compression
```

## Comparing `magictk-0.0.2.44.tar` & `magictk-0.0.2.45.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 03:12:19.997609 magictk-0.0.2.44/
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-21 03:12:19.000000 magictk-0.0.2.44/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-21 03:12:19.997609 magictk-0.0.2.44/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1376 2024-04-21 03:12:19.000000 magictk-0.0.2.44/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 03:12:19.997609 magictk-0.0.2.44/magictk/
--rw-r--r--   0 root         (0) root         (0)      359 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9695 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/_window_ctl.py
--rw-r--r--   0 root         (0) root         (0)    13250 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/_window_size.py
--rw-r--r--   0 root         (0) root         (0)     3253 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/basicwindow.py
--rw-r--r--   0 root         (0) root         (0)    13450 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/button.py
--rw-r--r--   0 root         (0) root         (0)    11146 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/checkbox.py
--rw-r--r--   0 root         (0) root         (0)     1919 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/color_tmpl.py
--rw-r--r--   0 root         (0) root         (0)    12040 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/entry.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/fontconfig.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/frame.py
--rw-r--r--   0 root         (0) root         (0)    15906 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/icon.ico
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/mtk.py
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/photoload.py
--rw-r--r--   0 root         (0) root         (0)     5893 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/progressbar.py
--rw-r--r--   0 root         (0) root         (0)    21933 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/res.pickle
--rw-r--r--   0 root         (0) root         (0)     6077 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/select.py
--rw-r--r--   0 root         (0) root         (0)    11076 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/submenu.py
--rw-r--r--   0 root         (0) root         (0)    10213 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/window.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 03:12:19.997609 magictk-0.0.2.44/magictk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      569 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-21 03:12:19.000000 magictk-0.0.2.44/magictk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-21 03:12:19.997609 magictk-0.0.2.44/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1127 2024-04-21 03:12:19.000000 magictk-0.0.2.44/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 08:13:04.201763 magictk-0.0.2.45/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-21 08:13:03.000000 magictk-0.0.2.45/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-21 08:13:04.201763 magictk-0.0.2.45/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1376 2024-04-21 08:13:03.000000 magictk-0.0.2.45/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 08:13:04.201763 magictk-0.0.2.45/magictk/
+-rw-r--r--   0 root         (0) root         (0)      359 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9695 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/_window_ctl.py
+-rw-r--r--   0 root         (0) root         (0)    13250 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/_window_size.py
+-rw-r--r--   0 root         (0) root         (0)     3253 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/basicwindow.py
+-rw-r--r--   0 root         (0) root         (0)    13450 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/button.py
+-rw-r--r--   0 root         (0) root         (0)    11146 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/color_tmpl.py
+-rw-r--r--   0 root         (0) root         (0)    12040 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/entry.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/fontconfig.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/frame.py
+-rw-r--r--   0 root         (0) root         (0)    15906 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/icon.ico
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/mtk.py
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/photoload.py
+-rw-r--r--   0 root         (0) root         (0)     5893 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/progressbar.py
+-rw-r--r--   0 root         (0) root         (0)    21933 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/res.pickle
+-rw-r--r--   0 root         (0) root         (0)     6077 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/select.py
+-rw-r--r--   0 root         (0) root         (0)    11076 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/submenu.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/window.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-21 08:13:03.000000 magictk-0.0.2.45/magictk/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 08:13:04.201763 magictk-0.0.2.45/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-21 08:13:04.000000 magictk-0.0.2.45/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      569 2024-04-21 08:13:04.000000 magictk-0.0.2.45/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-21 08:13:04.000000 magictk-0.0.2.45/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-21 08:13:04.000000 magictk-0.0.2.45/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-21 08:13:04.201763 magictk-0.0.2.45/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-21 08:13:03.000000 magictk-0.0.2.45/setup.py
```

### Comparing `magictk-0.0.2.44/PKG-INFO` & `magictk-0.0.2.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.44
+Version: 0.0.2.45
 Summary: A tkinter weights looks like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-0.0.2.44/README.md` & `magictk-0.0.2.45/README.md`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.44/magictk/_window_ctl.py` & `magictk-0.0.2.45/magictk/_window_ctl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.44/magictk/_window_size.py` & `magictk-0.0.2.45/magictk/_window_size.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.44/magictk/basicwindow.py` & `magictk-0.0.2.45/magictk/basicwindow.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.44/magictk/button.py` & `magictk-0.0.2.45/magictk/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,16 +111,16 @@
         self._update_color()
         self._bind_event()
         self.bind_anim()
 
     def pack(self, *args, **kwargs):
         self.canvas.pack(*args, **kwargs)
 
-    def guid(self, *args, **kwargs):
-        self.canvas.guid(*args, **kwargs)
+    def grid(self, *args, **kwargs):
+        self.canvas.grid(*args, **kwargs)
 
     def place(self, *args, **kwargs):
         self.canvas.place(*args, **kwargs)
 
     def _draw(self, _use_self_text=None):
         self._draw_corner(0, 0, 0, 0)
         self._draw_corner(1, 0, self.w-4, 0)
```

### Comparing `magictk-0.0.2.44/magictk/checkbox.py` & `magictk-0.0.2.45/magictk/checkbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,16 +131,16 @@
                          text=text, color_list=color_list, color_type=color_type, _dis_color=True)
         if (group is not None):
             group._add_checkbox(self)
 
     def pack(self, *args, **kwargs):
         self.canvas.pack(*args, **kwargs)
 
-    def guid(self, *args, **kwargs):
-        self.canvas.guid(*args, **kwargs)
+    def grid(self, *args, **kwargs):
+        self.canvas.grid(*args, **kwargs)
 
     def place(self, *args, **kwargs):
         self.canvas.place(*args, **kwargs)
 
     def _draw(self):
         self._draw_corner(0, 0, 0, 0)
         self._draw_corner(1, 0, 12, 0)
```

### Comparing `magictk-0.0.2.44/magictk/color_tmpl.py` & `magictk-0.0.2.45/magictk/color_tmpl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.44/magictk/entry.py` & `magictk-0.0.2.45/magictk/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,16 +142,16 @@
         self.__update_color()
         self.__bind_event()
         self.bind_anim()
 
     def pack(self, *args, **kwargs):
         self.frames.pack(*args, **kwargs)
 
-    def guid(self, *args, **kwargs):
-        self.frames.guid(*args, **kwargs)
+    def grid(self, *args, **kwargs):
+        self.frames.grid(*args, **kwargs)
 
     def place(self, *args, **kwargs):
         self.frames.place(*args, **kwargs)
 
     def __draw(self):
         self.__draw_corner(0, 0, 0, 0)
         self.__draw_corner(1, 0, self.w-4, 0)
```

### Comparing `magictk-0.0.2.44/magictk/fontconfig.py` & `magictk-0.0.2.45/magictk/fontconfig.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.44/magictk/icon.ico` & `magictk-0.0.2.45/magictk/icon.ico`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.44/magictk/photoload.py` & `magictk-0.0.2.45/magictk/photoload.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.44/magictk/progressbar.py` & `magictk-0.0.2.45/magictk/progressbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,16 +69,16 @@
         self.__draw()
         # self.__bind_event()
         self.bind_anim()
 
     def pack(self, *args, **kwargs):
         self.canvas.pack(*args, **kwargs)
 
-    def guid(self, *args, **kwargs):
-        self.canvas.guid(*args, **kwargs)
+    def grid(self, *args, **kwargs):
+        self.canvas.grid(*args, **kwargs)
 
     def place(self, *args, **kwargs):
         self.canvas.place(*args, **kwargs)
 
     def __draw(self):
         self.__fill_obj["bgbar"] = [
             self.canvas.create_rectangle(4, 1, self.w-5, self.h-1, width=0, fill=self.color["border_light"])]
```

### Comparing `magictk-0.0.2.44/magictk/res.pickle` & `magictk-0.0.2.45/magictk/res.pickle`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.44/magictk/select.py` & `magictk-0.0.2.45/magictk/select.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.44/magictk/submenu.py` & `magictk-0.0.2.45/magictk/submenu.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.44/magictk/window.py` & `magictk-0.0.2.45/magictk/window.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.44/magictk/workspace.py` & `magictk-0.0.2.45/magictk/workspace.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.44/magictk.egg-info/PKG-INFO` & `magictk-0.0.2.45/magictk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.44
+Version: 0.0.2.45
 Summary: A tkinter weights looks like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-0.0.2.44/magictk.egg-info/SOURCES.txt` & `magictk-0.0.2.45/magictk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.44/setup.py` & `magictk-0.0.2.45/setup.py`

 * *Files identical despite different names*


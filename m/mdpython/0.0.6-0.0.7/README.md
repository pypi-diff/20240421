# Comparing `tmp/mdpython-0.0.6.tar.gz` & `tmp/mdpython-0.0.7.tar.gz`

## Comparing `mdpython-0.0.6.tar` & `mdpython-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 mdpython-0.0.6/hello_world.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.6/src/mdpython/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 mdpython-0.0.6/src/mdpython/example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.6/src/mdpython/debugutils/__init__.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 mdpython-0.0.6/src/mdpython/debugutils/curpos.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 mdpython-0.0.6/src/mdpython/debugutils/timer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.6/src/mdpython/fileutils/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mdpython-0.0.6/src/mdpython/fileutils/cleanup.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 mdpython-0.0.6/src/mdpython/fileutils/compare.py
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 mdpython-0.0.6/src/mdpython/fileutils/compare_dir.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 mdpython-0.0.6/src/mdpython/fileutils/dir_info.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 mdpython-0.0.6/src/mdpython/fileutils/html_template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.6/src/mdpython/uiutils/__init__.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 mdpython-0.0.6/src/mdpython/uiutils/menu_based_app.py
--rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 mdpython-0.0.6/README.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 mdpython-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 mdpython-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 mdpython-0.0.7/hello_world.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.7/src/mdpython/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 mdpython-0.0.7/src/mdpython/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.7/src/mdpython/debugutils/__init__.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 mdpython-0.0.7/src/mdpython/debugutils/curpos.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 mdpython-0.0.7/src/mdpython/debugutils/timer.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 mdpython-0.0.7/src/mdpython/debugutils/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.7/src/mdpython/fileutils/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mdpython-0.0.7/src/mdpython/fileutils/cleanup.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 mdpython-0.0.7/src/mdpython/fileutils/compare.py
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 mdpython-0.0.7/src/mdpython/fileutils/compare_dir.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 mdpython-0.0.7/src/mdpython/fileutils/dir_info.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 mdpython-0.0.7/src/mdpython/fileutils/html_template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.7/src/mdpython/uiutils/__init__.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 mdpython-0.0.7/src/mdpython/uiutils/menu_based_app.py
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 mdpython-0.0.7/README.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 mdpython-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 mdpython-0.0.7/PKG-INFO
```

### Comparing `mdpython-0.0.6/src/mdpython/debugutils/curpos.py` & `mdpython-0.0.7/src/mdpython/debugutils/curpos.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.6/src/mdpython/debugutils/timer.py` & `mdpython-0.0.7/src/mdpython/debugutils/timer.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.6/src/mdpython/fileutils/compare.py` & `mdpython-0.0.7/src/mdpython/fileutils/compare.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.6/src/mdpython/fileutils/compare_dir.py` & `mdpython-0.0.7/src/mdpython/fileutils/compare_dir.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.6/src/mdpython/fileutils/dir_info.py` & `mdpython-0.0.7/src/mdpython/fileutils/dir_info.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.6/src/mdpython/fileutils/html_template.py` & `mdpython-0.0.7/src/mdpython/fileutils/html_template.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.6/README.md` & `mdpython-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -150,7 +150,15 @@
 # Compare Files
 
     from mdpython.fileutils import compare
     
     compare.compare_files(r"C:\Users\Dell\OneDrive\Desktop\spark\b.py",
                           r"C:\Users\Dell\OneDrive\Desktop\spark\c.py",
                           r"C:\Users\Dell\OneDrive\Desktop\spark\out.html")
+
+# Track package changes
+
+    from mdpython.debugutils import version
+    
+    version.save("app_dev", r"D:\data\version")
+    version.timeline("app_dev", r"D:\data\version")
+    version.compare("app_dev", r"D:\data\version")
```

### Comparing `mdpython-0.0.6/pyproject.toml` & `mdpython-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mdpython"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Dhaval", email="seedhaval@gmail.com" },
 ]
 description = "MD Python Library"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `mdpython-0.0.6/PKG-INFO` & `mdpython-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mdpython
-Version: 0.0.6
+Version: 0.0.7
 Summary: MD Python Library
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Author-email: Dhaval <seedhaval@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -163,7 +163,15 @@
 # Compare Files
 
     from mdpython.fileutils import compare
     
     compare.compare_files(r"C:\Users\Dell\OneDrive\Desktop\spark\b.py",
                           r"C:\Users\Dell\OneDrive\Desktop\spark\c.py",
                           r"C:\Users\Dell\OneDrive\Desktop\spark\out.html")
+
+# Track package changes
+
+    from mdpython.debugutils import version
+    
+    version.save("app_dev", r"D:\data\version")
+    version.timeline("app_dev", r"D:\data\version")
+    version.compare("app_dev", r"D:\data\version")
```


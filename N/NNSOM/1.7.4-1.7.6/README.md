# Comparing `tmp/nnsom-1.7.4.tar.gz` & `tmp/nnsom-1.7.6.tar.gz`

## Comparing `nnsom-1.7.4.tar` & `nnsom-1.7.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 nnsom-1.7.4/src/NNSOM/__init__.py
--rw-r--r--   0        0        0    79579 2020-02-02 00:00:00.000000 nnsom-1.7.4/src/NNSOM/plots.py
--rw-r--r--   0        0        0    19781 2020-02-02 00:00:00.000000 nnsom-1.7.4/src/NNSOM/som.py
--rw-r--r--   0        0        0    24827 2020-02-02 00:00:00.000000 nnsom-1.7.4/src/NNSOM/som_gpu.py
--rw-r--r--   0        0        0    21590 2020-02-02 00:00:00.000000 nnsom-1.7.4/src/NNSOM/utils.py
--rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 nnsom-1.7.4/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.7.4/LICENSE
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 nnsom-1.7.4/README.md
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 nnsom-1.7.4/pyproject.toml
--rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 nnsom-1.7.4/PKG-INFO
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 nnsom-1.7.6/src/NNSOM/__init__.py
+-rw-r--r--   0        0        0    79579 2020-02-02 00:00:00.000000 nnsom-1.7.6/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    19781 2020-02-02 00:00:00.000000 nnsom-1.7.6/src/NNSOM/som.py
+-rw-r--r--   0        0        0    24827 2020-02-02 00:00:00.000000 nnsom-1.7.6/src/NNSOM/som_gpu.py
+-rw-r--r--   0        0        0    21590 2020-02-02 00:00:00.000000 nnsom-1.7.6/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 nnsom-1.7.6/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.7.6/LICENSE
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 nnsom-1.7.6/README.md
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 nnsom-1.7.6/pyproject.toml
+-rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 nnsom-1.7.6/PKG-INFO
```

### Comparing `nnsom-1.7.4/src/NNSOM/plots.py` & `nnsom-1.7.6/src/NNSOM/plots.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.7.4/src/NNSOM/som.py` & `nnsom-1.7.6/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.7.4/src/NNSOM/som_gpu.py` & `nnsom-1.7.6/src/NNSOM/som_gpu.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.7.4/src/NNSOM/utils.py` & `nnsom-1.7.6/src/NNSOM/utils.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.7.4/.gitignore` & `nnsom-1.7.6/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.7.4/README.md` & `nnsom-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `nnsom-1.7.4/pyproject.toml` & `nnsom-1.7.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.7.4"
+version = "1.7.6"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
-  { name = "Dr. Hagan" },
-  { name = "Dr. Amir Jafari" },
+  { name = "Dr. Martin Hagan" , email= "mhagan@ieee.org" },
+  { name = "Dr. Amir Jafari" , email = "amir.h.jafari@okstate.edu"},
   { name = "Lakshmi Sravya Chalapati" },
   { name = "Ei Tanaka" },
 
 ]
 #maintainers = [
 #  { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
 #]
```

### Comparing `nnsom-1.7.4/PKG-INFO` & `nnsom-1.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.7.4
+Version: 1.7.6
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Project-URL: Documenation, https://amir-jafari.github.io/SOM/
-Author: Dr. Hagan, Dr. Amir Jafari, Lakshmi Sravya Chalapati, Ei Tanaka
+Author: Lakshmi Sravya Chalapati, Ei Tanaka
+Author-email: "Dr. Martin Hagan" <mhagan@ieee.org>, "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
 Keywords: Clustering,Machine Learning,Neural Network,SOM,Unsupervised Learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```


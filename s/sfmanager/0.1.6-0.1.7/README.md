# Comparing `tmp/sfmanager-0.1.6.tar.gz` & `tmp/sfmanager-0.1.7.tar.gz`

## Comparing `sfmanager-0.1.6.tar` & `sfmanager-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 sfmanager-0.1.6/update
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 sfmanager-0.1.6/version
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sfmanager-0.1.6/sfmanager/__init__.py
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 sfmanager-0.1.6/sfmanager/app.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 sfmanager-0.1.6/sfmanager/utils.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.6/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.6/LICENSE
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 sfmanager-0.1.6/README.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 sfmanager-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 sfmanager-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 sfmanager-0.1.7/update
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 sfmanager-0.1.7/version
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sfmanager-0.1.7/sfmanager/__init__.py
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 sfmanager-0.1.7/sfmanager/app.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 sfmanager-0.1.7/sfmanager/utils.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.7/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.7/LICENSE
+-rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 sfmanager-0.1.7/README.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 sfmanager-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 sfmanager-0.1.7/PKG-INFO
```

### Comparing `sfmanager-0.1.6/sfmanager/app.py` & `sfmanager-0.1.7/sfmanager/app.py`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.6/sfmanager/utils.py` & `sfmanager-0.1.7/sfmanager/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,9 +50,8 @@
 			subprocess.check_call([sys.executable, "-m", "pip", "install", "sfmanager==" + value_v])
 			logger.success("sfmanager updated, changes will take effect after restart")
 
 			if updates.status_code == 200:
 				value_u = updates.text[0:]
 				print(f"{value_v}")
 
-			os.chdir(os.path.join(pkg_resources.get_distribution("sfmanager").location, "sfmanager"))
-checkUpdates()
+			os.chdir(os.path.join(pkg_resources.get_distribution("sfmanager").location, "sfmanager"))
```

### Comparing `sfmanager-0.1.6/.gitignore` & `sfmanager-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.6/LICENSE` & `sfmanager-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.6/README.md` & `sfmanager-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.6/pyproject.toml` & `sfmanager-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "sfmanager"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
 	{name="GrandTheBest", email="grandinfo-cm@gmail.com"},
 ]
 description = "This library is not that useful. Perhaps someday it will become great."
 readme = "README.md"
 requires-python = ">=3.10.0"
 dependencies = [
```

### Comparing `sfmanager-0.1.6/PKG-INFO` & `sfmanager-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sfmanager
-Version: 0.1.6
+Version: 0.1.7
 Summary: This library is not that useful. Perhaps someday it will become great.
 Project-URL: Homepage, https://github.com/GrandTheBest/sfmanager
 Project-URL: Issues, https://github.com/GrandTheBest/sfmanager/issues
 Author-email: GrandTheBest <grandinfo-cm@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


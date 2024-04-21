# Comparing `tmp/drop2beets-2.0.0.tar.gz` & `tmp/drop2beets-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drop2beets-2.0.0.tar", max compression
+gzip compressed data, was "drop2beets-2.0.1.tar", max compression
```

## Comparing `drop2beets-2.0.0.tar` & `drop2beets-2.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      484 2020-11-30 20:42:22.325546 drop2beets-2.0.0/LICENSE
--rw-r--r--   0        0        0     2941 2023-08-20 16:45:58.342065 drop2beets-2.0.0/README.md
--rw-r--r--   0        0        0       75 2020-05-19 19:42:35.559840 drop2beets-2.0.0/beetsplug/__init__.py
--rw-r--r--   0        0        0     6610 2023-08-20 16:19:10.398554 drop2beets-2.0.0/beetsplug/drop2beets.py
--rw-r--r--   0        0        0      647 2020-05-19 19:42:35.559840 drop2beets-2.0.0/examples/custom_tag.py
--rw-r--r--   0        0        0     1639 2020-05-19 19:42:35.563840 drop2beets-2.0.0/examples/force_genre_and_language_by_folder.py
--rw-r--r--   0        0        0     1047 2020-05-19 19:42:35.563840 drop2beets-2.0.0/examples/force_genre_by_folder.py
--rw-r--r--   0        0        0      346 2020-05-19 19:42:35.563840 drop2beets-2.0.0/examples/skip_missing_title_or_artist.py
--rw-r--r--   0        0        0      793 2023-08-20 16:44:22.594372 drop2beets-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3870 1970-01-01 00:00:00.000000 drop2beets-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      484 2020-11-30 20:42:22.325546 drop2beets-2.0.1/LICENSE
+-rw-r--r--   0        0        0     2941 2023-08-20 16:45:58.342065 drop2beets-2.0.1/README.md
+-rw-r--r--   0        0        0       75 2020-05-19 19:42:35.559840 drop2beets-2.0.1/beetsplug/__init__.py
+-rw-r--r--   0        0        0     6751 2024-04-21 15:50:18.559132 drop2beets-2.0.1/beetsplug/drop2beets.py
+-rw-r--r--   0        0        0      647 2020-05-19 19:42:35.559840 drop2beets-2.0.1/examples/custom_tag.py
+-rw-r--r--   0        0        0     1639 2020-05-19 19:42:35.563840 drop2beets-2.0.1/examples/force_genre_and_language_by_folder.py
+-rw-r--r--   0        0        0     1047 2020-05-19 19:42:35.563840 drop2beets-2.0.1/examples/force_genre_by_folder.py
+-rw-r--r--   0        0        0      346 2020-05-19 19:42:35.563840 drop2beets-2.0.1/examples/skip_missing_title_or_artist.py
+-rw-r--r--   0        0        0      793 2024-04-21 15:52:05.617229 drop2beets-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3921 1970-01-01 00:00:00.000000 drop2beets-2.0.1/PKG-INFO
```

### Comparing `drop2beets-2.0.0/README.md` & `drop2beets-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `drop2beets-2.0.0/beetsplug/drop2beets.py` & `drop2beets-2.0.1/beetsplug/drop2beets.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,17 @@
 
     def on_import_begin(self, session):
         session.config['singletons'] = True
         config['import']['quiet'] = True
         self.attributes = None
 
     def on_import_task_created(self, task, session):
+        # Some ImportTasks, like progress updates, have no item; ignore them
+        if not hasattr(task, 'item'):
+            return [task]
         path = str(task.item.path, 'utf-8', 'ignore')
         folder = os.path.dirname(path)
         dropbox_path = folder[len(self.dropbox_path):]
         self.attributes = self.on_item(task.item, dropbox_path)
         if self.attributes is None:
             _logger.info("Importation aborted by on_item")
             return []
```

### Comparing `drop2beets-2.0.0/examples/custom_tag.py` & `drop2beets-2.0.1/examples/custom_tag.py`

 * *Files identical despite different names*

### Comparing `drop2beets-2.0.0/examples/force_genre_and_language_by_folder.py` & `drop2beets-2.0.1/examples/force_genre_and_language_by_folder.py`

 * *Files identical despite different names*

### Comparing `drop2beets-2.0.0/examples/force_genre_by_folder.py` & `drop2beets-2.0.1/examples/force_genre_by_folder.py`

 * *Files identical despite different names*

### Comparing `drop2beets-2.0.0/pyproject.toml` & `drop2beets-2.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drop2beets"
-version = "2.0.0"
+version = "2.0.1"
 description = "Import singles to Beets as soon as they are dropped in a folder"
 authors = ["Martin Kirchgessner <martin.kirch@gmail.com>"]
 license = "WTFPL"
 readme = "README.md"
 homepage = "https://github.com/martinkirch/drop2beets"
 repository = "https://github.com/martinkirch/drop2beets.git"
 keywords = ["watch", "beets", "music", "import"]
```

### Comparing `drop2beets-2.0.0/PKG-INFO` & `drop2beets-2.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drop2beets
-Version: 2.0.0
+Version: 2.0.1
 Summary: Import singles to Beets as soon as they are dropped in a folder
 Home-page: https://github.com/martinkirch/drop2beets
 License: WTFPL
 Keywords: watch,beets,music,import
 Author: Martin Kirchgessner
 Author-email: martin.kirch@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -12,14 +12,15 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Sound/Audio
 Requires-Dist: watchdog (>=3.0.0,<4.0.0)
 Project-URL: Repository, https://github.com/martinkirch/drop2beets.git
 Description-Content-Type: text/markdown
 
 # drop2beets
```


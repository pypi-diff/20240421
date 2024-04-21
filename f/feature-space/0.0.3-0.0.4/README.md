# Comparing `tmp/feature_space-0.0.3.tar.gz` & `tmp/feature_space-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feature_space-0.0.3.tar", last modified: Sun Apr 21 13:29:49 2024, max compression
+gzip compressed data, was "feature_space-0.0.4.tar", last modified: Sun Apr 21 13:48:26 2024, max compression
```

## Comparing `feature_space-0.0.3.tar` & `feature_space-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 13:29:49.808625 feature_space-0.0.3/
--rw-rw-rw-   0        0        0       44 2024-04-21 13:29:49.000000 feature_space-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4696 2024-04-21 13:29:49.807300 feature_space-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3895 2024-04-21 13:23:19.000000 feature_space-0.0.3/README.md
--rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 feature_space-0.0.3/build.py
-drwxrwxrwx   0        0        0        0 2024-04-21 13:29:49.801295 feature_space-0.0.3/feature_space/
--rw-rw-rw-   0        0        0      129 2024-04-19 12:10:02.000000 feature_space-0.0.3/feature_space/__init__.py
--rw-rw-rw-   0        0        0     3687 2024-04-21 13:29:07.000000 feature_space-0.0.3/feature_space/dataset.py
--rw-rw-rw-   0        0        0     2624 2024-04-21 13:29:07.000000 feature_space-0.0.3/feature_space/feature.py
--rw-rw-rw-   0        0        0    11950 2024-04-19 12:22:24.000000 feature_space-0.0.3/feature_space/features.py
-drwxrwxrwx   0        0        0        0 2024-04-21 13:29:49.807300 feature_space-0.0.3/feature_space.egg-info/
--rw-rw-rw-   0        0        0     4696 2024-04-21 13:29:49.000000 feature_space-0.0.3/feature_space.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-04-21 13:29:49.000000 feature_space-0.0.3/feature_space.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 13:29:49.000000 feature_space-0.0.3/feature_space.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-21 13:29:49.000000 feature_space-0.0.3/feature_space.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-21 13:29:49.000000 feature_space-0.0.3/feature_space.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       19 2024-04-21 13:29:07.000000 feature_space-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 13:29:49.808625 feature_space-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1324 2024-04-21 13:29:45.000000 feature_space-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:48:26.708342 feature_space-0.0.4/
+-rw-rw-rw-   0        0        0       44 2024-04-21 13:48:26.000000 feature_space-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4696 2024-04-21 13:48:26.707336 feature_space-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3895 2024-04-21 13:23:19.000000 feature_space-0.0.4/README.md
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 feature_space-0.0.4/build.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:48:26.701854 feature_space-0.0.4/feature_space/
+-rw-rw-rw-   0        0        0      129 2024-04-19 12:10:02.000000 feature_space-0.0.4/feature_space/__init__.py
+-rw-rw-rw-   0        0        0     3894 2024-04-21 13:47:34.000000 feature_space-0.0.4/feature_space/dataset.py
+-rw-rw-rw-   0        0        0     2831 2024-04-21 13:47:34.000000 feature_space-0.0.4/feature_space/feature.py
+-rw-rw-rw-   0        0        0    11950 2024-04-19 12:22:24.000000 feature_space-0.0.4/feature_space/features.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:48:26.707336 feature_space-0.0.4/feature_space.egg-info/
+-rw-rw-rw-   0        0        0     4696 2024-04-21 13:48:26.000000 feature_space-0.0.4/feature_space.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-04-21 13:48:26.000000 feature_space-0.0.4/feature_space.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 13:48:26.000000 feature_space-0.0.4/feature_space.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-21 13:48:26.000000 feature_space-0.0.4/feature_space.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-21 13:48:26.000000 feature_space-0.0.4/feature_space.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       19 2024-04-21 13:29:07.000000 feature_space-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 13:48:26.708342 feature_space-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2024-04-21 13:47:34.000000 feature_space-0.0.4/setup.py
```

### Comparing `feature_space-0.0.3/PKG-INFO` & `feature_space-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature-space
-Version: 0.0.3
+Version: 0.0.4
 Summary: A module framework for constructing a network of features supporting each other, yet each feature is calculated only once.
 Home-page: https://github.com/Shahaf-F-S/feature-space
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `feature_space-0.0.3/README.md` & `feature_space-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `feature_space-0.0.3/build.py` & `feature_space-0.0.4/build.py`

 * *Files identical despite different names*

### Comparing `feature_space-0.0.3/feature_space/dataset.py` & `feature_space-0.0.4/feature_space/dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,18 +86,29 @@
         return all(d.calculated for d in set(self.datasets))
 
     @property
     def calculated(self) -> bool:
 
         return self.features_calculated and self.datasets_calculated
 
+    def copy(self) -> "Dataset":
+
+        data = self.__reduce__()
+
+        copy = data[0](type(self), data[1][0], data[-1])
+
+        return copy
+
     def save(self, path: str) -> None:
 
+        copy = self.copy()
+        copy.clear()
+
         with open(path, 'wb') as file:
-            dill.dump(self, file)
+            dill.dump(copy, file)
 
     @classmethod
     def load(cls, path: str) -> "Feature":
 
         with open(path, 'rb') as file:
             return dill.load(file)
```

### Comparing `feature_space-0.0.3/feature_space/feature.py` & `feature_space-0.0.4/feature_space/feature.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,16 +58,27 @@
         return features
 
     @property
     def features_names(self) -> list[str]:
 
         return [f.name for f in self.features]
 
+    def copy(self) -> "Feature":
+
+        data = self.__reduce__()
+
+        copy = data[0](type(self), data[1][0], data[-1])
+
+        return copy
+
     def save(self, path: str) -> None:
 
+        copy = self.copy()
+        copy.clear()
+
         with open(path, 'wb') as file:
             dill.dump(self, file)
 
     @classmethod
     def load(cls, path: str) -> "Feature":
 
         with open(path, 'rb') as file:
```

### Comparing `feature_space-0.0.3/feature_space/features.py` & `feature_space-0.0.4/feature_space/features.py`

 * *Files identical despite different names*

### Comparing `feature_space-0.0.3/feature_space.egg-info/PKG-INFO` & `feature_space-0.0.4/feature_space.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature-space
-Version: 0.0.3
+Version: 0.0.4
 Summary: A module framework for constructing a network of features supporting each other, yet each feature is calculated only once.
 Home-page: https://github.com/Shahaf-F-S/feature-space
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `feature_space-0.0.3/setup.py` & `feature_space-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         name='feature-space',
-        version='0.0.3',
+        version='0.0.4',
         description=(
             "A module framework for constructing a network of features "
             "supporting each other, yet each feature is calculated only once."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```


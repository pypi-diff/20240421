# Comparing `tmp/feature_space-0.0.2.tar.gz` & `tmp/feature_space-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feature_space-0.0.2.tar", last modified: Sun Apr 21 13:23:23 2024, max compression
+gzip compressed data, was "feature_space-0.0.3.tar", last modified: Sun Apr 21 13:29:49 2024, max compression
```

## Comparing `feature_space-0.0.2.tar` & `feature_space-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 13:23:23.007141 feature_space-0.0.2/
--rw-rw-rw-   0        0        0       44 2024-04-21 13:23:22.000000 feature_space-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4675 2024-04-21 13:23:23.005674 feature_space-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3895 2024-04-21 13:23:19.000000 feature_space-0.0.2/README.md
--rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 feature_space-0.0.2/build.py
-drwxrwxrwx   0        0        0        0 2024-04-21 13:23:23.000550 feature_space-0.0.2/feature_space/
--rw-rw-rw-   0        0        0      129 2024-04-19 12:10:02.000000 feature_space-0.0.2/feature_space/__init__.py
--rw-rw-rw-   0        0        0     3610 2024-04-21 13:19:56.000000 feature_space-0.0.2/feature_space/dataset.py
--rw-rw-rw-   0        0        0     2630 2024-04-21 13:19:56.000000 feature_space-0.0.2/feature_space/feature.py
--rw-rw-rw-   0        0        0    11950 2024-04-19 12:22:24.000000 feature_space-0.0.2/feature_space/features.py
-drwxrwxrwx   0        0        0        0 2024-04-21 13:23:23.005674 feature_space-0.0.2/feature_space.egg-info/
--rw-rw-rw-   0        0        0     4675 2024-04-21 13:23:22.000000 feature_space-0.0.2/feature_space.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-04-21 13:23:22.000000 feature_space-0.0.2/feature_space.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 13:23:22.000000 feature_space-0.0.2/feature_space.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-21 13:23:22.000000 feature_space-0.0.2/feature_space.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-21 13:23:22.000000 feature_space-0.0.2/feature_space.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       13 2024-04-21 13:16:18.000000 feature_space-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 13:23:23.007141 feature_space-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1324 2024-04-21 13:23:19.000000 feature_space-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:29:49.808625 feature_space-0.0.3/
+-rw-rw-rw-   0        0        0       44 2024-04-21 13:29:49.000000 feature_space-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4696 2024-04-21 13:29:49.807300 feature_space-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3895 2024-04-21 13:23:19.000000 feature_space-0.0.3/README.md
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 feature_space-0.0.3/build.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:29:49.801295 feature_space-0.0.3/feature_space/
+-rw-rw-rw-   0        0        0      129 2024-04-19 12:10:02.000000 feature_space-0.0.3/feature_space/__init__.py
+-rw-rw-rw-   0        0        0     3687 2024-04-21 13:29:07.000000 feature_space-0.0.3/feature_space/dataset.py
+-rw-rw-rw-   0        0        0     2624 2024-04-21 13:29:07.000000 feature_space-0.0.3/feature_space/feature.py
+-rw-rw-rw-   0        0        0    11950 2024-04-19 12:22:24.000000 feature_space-0.0.3/feature_space/features.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:29:49.807300 feature_space-0.0.3/feature_space.egg-info/
+-rw-rw-rw-   0        0        0     4696 2024-04-21 13:29:49.000000 feature_space-0.0.3/feature_space.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-04-21 13:29:49.000000 feature_space-0.0.3/feature_space.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 13:29:49.000000 feature_space-0.0.3/feature_space.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-21 13:29:49.000000 feature_space-0.0.3/feature_space.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-21 13:29:49.000000 feature_space-0.0.3/feature_space.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       19 2024-04-21 13:29:07.000000 feature_space-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 13:29:49.808625 feature_space-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2024-04-21 13:29:45.000000 feature_space-0.0.3/setup.py
```

### Comparing `feature_space-0.0.2/PKG-INFO` & `feature_space-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature-space
-Version: 0.0.2
+Version: 0.0.3
 Summary: A module framework for constructing a network of features supporting each other, yet each feature is calculated only once.
 Home-page: https://github.com/Shahaf-F-S/feature-space
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: numpy
+Requires-Dist: dill
 Provides-Extra: dev
 
 # feature-space
 
 > A module framework for constructing a network of features supporting each other, yet each feature is calculated only once.
 
 ## Installation
```

### Comparing `feature_space-0.0.2/README.md` & `feature_space-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `feature_space-0.0.2/build.py` & `feature_space-0.0.3/build.py`

 * *Files identical despite different names*

### Comparing `feature_space-0.0.2/feature_space/dataset.py` & `feature_space-0.0.3/feature_space/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # dataset.py
 
-import pickle
+import dill
+from uuid import uuid4
 from dataclasses import dataclass, field
 
 import pandas as pd
 
 from feature_space.feature import Feature
 
 __all__ = [
     "Dataset"
 ]
 
 @dataclass
 class Dataset:
 
     name: str = 'Dataset'
+    id: str = field(default_factory=lambda: str(uuid4()))
     features: list[Feature] = field(default_factory=list)
     datasets: list['Dataset'] = field(default_factory=list)
 
     def __hash__(self) -> int:
 
         return hash(self.name)
 
@@ -87,21 +89,21 @@
     def calculated(self) -> bool:
 
         return self.features_calculated and self.datasets_calculated
 
     def save(self, path: str) -> None:
 
         with open(path, 'wb') as file:
-            pickle.dump(self, file)
+            dill.dump(self, file)
 
     @classmethod
     def load(cls, path: str) -> "Feature":
 
         with open(path, 'rb') as file:
-            return pickle.load(file)
+            return dill.load(file)
 
     def calculate_features(
             self,
             data: pd.DataFrame,
             cached: bool = True,
             override: bool = False
     ) -> 'Dataset':
```

### Comparing `feature_space-0.0.2/feature_space/feature.py` & `feature_space-0.0.3/feature_space/feature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # features.py
 
-import pickle
+import dill
 from uuid import uuid4
 from typing import Callable, ParamSpec, ParamSpecKwargs
 from dataclasses import dataclass, field
 
 import pandas as pd
 
 __all__ = (
@@ -61,21 +61,21 @@
     def features_names(self) -> list[str]:
 
         return [f.name for f in self.features]
 
     def save(self, path: str) -> None:
 
         with open(path, 'wb') as file:
-            pickle.dump(self, file)
+            dill.dump(self, file)
 
     @classmethod
     def load(cls, path: str) -> "Feature":
 
         with open(path, 'rb') as file:
-            return pickle.load(file)
+            return dill.load(file)
 
     def calculate(
             self,
             data: pd.DataFrame,
             cached: bool = True,
             override: bool = False
     ) -> 'Feature':
```

### Comparing `feature_space-0.0.2/feature_space/features.py` & `feature_space-0.0.3/feature_space/features.py`

 * *Files identical despite different names*

### Comparing `feature_space-0.0.2/feature_space.egg-info/PKG-INFO` & `feature_space-0.0.3/feature_space.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature-space
-Version: 0.0.2
+Version: 0.0.3
 Summary: A module framework for constructing a network of features supporting each other, yet each feature is calculated only once.
 Home-page: https://github.com/Shahaf-F-S/feature-space
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: numpy
+Requires-Dist: dill
 Provides-Extra: dev
 
 # feature-space
 
 > A module framework for constructing a network of features supporting each other, yet each feature is calculated only once.
 
 ## Installation
```

### Comparing `feature_space-0.0.2/setup.py` & `feature_space-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         name='feature-space',
-        version='0.0.2',
+        version='0.0.3',
         description=(
             "A module framework for constructing a network of features "
             "supporting each other, yet each feature is calculated only once."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```


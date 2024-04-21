# Comparing `tmp/feature_space-0.0.1.tar.gz` & `tmp/feature_space-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feature_space-0.0.1.tar", last modified: Sat Apr 20 06:22:13 2024, max compression
+gzip compressed data, was "feature_space-0.0.2.tar", last modified: Sun Apr 21 13:23:23 2024, max compression
```

## Comparing `feature_space-0.0.1.tar` & `feature_space-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 06:22:13.449932 feature_space-0.0.1/
--rw-rw-rw-   0        0        0       44 2024-04-20 06:22:13.000000 feature_space-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4499 2024-04-20 06:22:13.449932 feature_space-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3719 2024-04-19 12:58:02.000000 feature_space-0.0.1/README.md
--rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 feature_space-0.0.1/build.py
-drwxrwxrwx   0        0        0        0 2024-04-20 06:22:13.444932 feature_space-0.0.1/feature_space/
--rw-rw-rw-   0        0        0      129 2024-04-19 12:10:02.000000 feature_space-0.0.1/feature_space/__init__.py
--rw-rw-rw-   0        0        0     3330 2024-04-20 06:21:04.000000 feature_space-0.0.1/feature_space/dataset.py
--rw-rw-rw-   0        0        0     2026 2024-04-20 06:21:59.000000 feature_space-0.0.1/feature_space/feature.py
--rw-rw-rw-   0        0        0    11950 2024-04-19 12:22:24.000000 feature_space-0.0.1/feature_space/features.py
-drwxrwxrwx   0        0        0        0 2024-04-20 06:22:13.448933 feature_space-0.0.1/feature_space.egg-info/
--rw-rw-rw-   0        0        0     4499 2024-04-20 06:22:13.000000 feature_space-0.0.1/feature_space.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-04-20 06:22:13.000000 feature_space-0.0.1/feature_space.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 06:22:13.000000 feature_space-0.0.1/feature_space.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-20 06:22:13.000000 feature_space-0.0.1/feature_space.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-20 06:22:13.000000 feature_space-0.0.1/feature_space.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       13 2024-04-19 12:08:38.000000 feature_space-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 06:22:13.450931 feature_space-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1324 2024-04-20 06:22:10.000000 feature_space-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:23:23.007141 feature_space-0.0.2/
+-rw-rw-rw-   0        0        0       44 2024-04-21 13:23:22.000000 feature_space-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4675 2024-04-21 13:23:23.005674 feature_space-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3895 2024-04-21 13:23:19.000000 feature_space-0.0.2/README.md
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 feature_space-0.0.2/build.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:23:23.000550 feature_space-0.0.2/feature_space/
+-rw-rw-rw-   0        0        0      129 2024-04-19 12:10:02.000000 feature_space-0.0.2/feature_space/__init__.py
+-rw-rw-rw-   0        0        0     3610 2024-04-21 13:19:56.000000 feature_space-0.0.2/feature_space/dataset.py
+-rw-rw-rw-   0        0        0     2630 2024-04-21 13:19:56.000000 feature_space-0.0.2/feature_space/feature.py
+-rw-rw-rw-   0        0        0    11950 2024-04-19 12:22:24.000000 feature_space-0.0.2/feature_space/features.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:23:23.005674 feature_space-0.0.2/feature_space.egg-info/
+-rw-rw-rw-   0        0        0     4675 2024-04-21 13:23:22.000000 feature_space-0.0.2/feature_space.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-04-21 13:23:22.000000 feature_space-0.0.2/feature_space.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 13:23:22.000000 feature_space-0.0.2/feature_space.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-21 13:23:22.000000 feature_space-0.0.2/feature_space.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-21 13:23:22.000000 feature_space-0.0.2/feature_space.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       13 2024-04-21 13:16:18.000000 feature_space-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 13:23:23.007141 feature_space-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2024-04-21 13:23:19.000000 feature_space-0.0.2/setup.py
```

### Comparing `feature_space-0.0.1/PKG-INFO` & `feature_space-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature-space
-Version: 0.0.1
+Version: 0.0.2
 Summary: A module framework for constructing a network of features supporting each other, yet each feature is calculated only once.
 Home-page: https://github.com/Shahaf-F-S/feature-space
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -119,7 +119,13 @@
 
 if you wish to override existing data, you can specify.
 
 ```python
 change_indicators.clear()
 change_indicators.calculate(df, override=True)
 ```
+
+Save and load a whole dataset with its inter-dependency of features:
+```python
+change_indicators.save('dataset.pkl')
+change_indicators = Dataset.load('dataset.pkl')
+```
```

### Comparing `feature_space-0.0.1/README.md` & `feature_space-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -98,8 +98,14 @@
 series in the features.
 
 if you wish to override existing data, you can specify.
 
 ```python
 change_indicators.clear()
 change_indicators.calculate(df, override=True)
+```
+
+Save and load a whole dataset with its inter-dependency of features:
+```python
+change_indicators.save('dataset.pkl')
+change_indicators = Dataset.load('dataset.pkl')
 ```
```

### Comparing `feature_space-0.0.1/build.py` & `feature_space-0.0.2/build.py`

 * *Files identical despite different names*

### Comparing `feature_space-0.0.1/feature_space/dataset.py` & `feature_space-0.0.2/feature_space/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # dataset.py
 
+import pickle
 from dataclasses import dataclass, field
 
 import pandas as pd
 
 from feature_space.feature import Feature
 
 __all__ = [
@@ -83,14 +84,25 @@
         return all(d.calculated for d in set(self.datasets))
 
     @property
     def calculated(self) -> bool:
 
         return self.features_calculated and self.datasets_calculated
 
+    def save(self, path: str) -> None:
+
+        with open(path, 'wb') as file:
+            pickle.dump(self, file)
+
+    @classmethod
+    def load(cls, path: str) -> "Feature":
+
+        with open(path, 'rb') as file:
+            return pickle.load(file)
+
     def calculate_features(
             self,
             data: pd.DataFrame,
             cached: bool = True,
             override: bool = False
     ) -> 'Dataset':
```

### Comparing `feature_space-0.0.1/feature_space/feature.py` & `feature_space-0.0.2/feature_space/feature.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # features.py
 
+import pickle
+from uuid import uuid4
 from typing import Callable, ParamSpec, ParamSpecKwargs
 from dataclasses import dataclass, field
 
 import pandas as pd
 
 __all__ = (
     'Feature',
@@ -13,14 +15,15 @@
 _P = ParamSpec('_P')
 P = ParamSpecKwargs(_P)
 
 @dataclass
 class Feature:
 
     name: str
+    id: str = field(default_factory=lambda: str(uuid4()))
     features: list['Feature'] = field(default_factory=list)
     kwargs: P = field(default_factory=dict)
     calculator: Callable[['Feature'], pd.Series] = field(default=None, repr=False)
     data: pd.DataFrame | None = field(default=None, repr=False)
     result: pd.Series | None = field(default=None, repr=False)
 
     def __hash__(self) -> int:
@@ -39,18 +42,41 @@
 
         if self.name not in names:
             names.insert(0, self.name)
 
         return names
 
     @property
+    def all_features(self) -> set['Feature']:
+
+        features = set()
+
+        for feature in self.features:
+            features.update(feature.all_features)
+
+        features.add(self)
+
+        return features
+
+    @property
     def features_names(self) -> list[str]:
 
         return [f.name for f in self.features]
 
+    def save(self, path: str) -> None:
+
+        with open(path, 'wb') as file:
+            pickle.dump(self, file)
+
+    @classmethod
+    def load(cls, path: str) -> "Feature":
+
+        with open(path, 'rb') as file:
+            return pickle.load(file)
+
     def calculate(
             self,
             data: pd.DataFrame,
             cached: bool = True,
             override: bool = False
     ) -> 'Feature':
```

### Comparing `feature_space-0.0.1/feature_space/features.py` & `feature_space-0.0.2/feature_space/features.py`

 * *Files identical despite different names*

### Comparing `feature_space-0.0.1/feature_space.egg-info/PKG-INFO` & `feature_space-0.0.2/feature_space.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature-space
-Version: 0.0.1
+Version: 0.0.2
 Summary: A module framework for constructing a network of features supporting each other, yet each feature is calculated only once.
 Home-page: https://github.com/Shahaf-F-S/feature-space
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -119,7 +119,13 @@
 
 if you wish to override existing data, you can specify.
 
 ```python
 change_indicators.clear()
 change_indicators.calculate(df, override=True)
 ```
+
+Save and load a whole dataset with its inter-dependency of features:
+```python
+change_indicators.save('dataset.pkl')
+change_indicators = Dataset.load('dataset.pkl')
+```
```

### Comparing `feature_space-0.0.1/setup.py` & `feature_space-0.0.2/setup.py`

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
-        version='0.0.1',
+        version='0.0.2',
         description=(
             "A module framework for constructing a network of features "
             "supporting each other, yet each feature is calculated only once."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```


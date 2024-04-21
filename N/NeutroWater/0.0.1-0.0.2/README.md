# Comparing `tmp/neutrowater-0.0.1.tar.gz` & `tmp/neutrowater-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neutrowater-0.0.1.tar", max compression
+gzip compressed data, was "neutrowater-0.0.2.tar", max compression
```

## Comparing `neutrowater-0.0.1.tar` & `neutrowater-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,27 @@
--rw-r--r--   0        0        0     1073 2024-03-25 16:32:15.084916 neutrowater-0.0.1/LICENSE
--rw-r--r--   0        0        0     1122 2024-04-19 13:51:25.231584 neutrowater-0.0.1/README.md
--rw-r--r--   0        0        0     1298 2024-04-19 12:54:25.703953 neutrowater-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-01 11:50:16.012474 neutrowater-0.0.1/src/neutrowater/__init__.py
--rw-r--r--   0        0        0     8287 2024-04-19 12:53:58.139709 neutrowater-0.0.1/src/neutrowater/diffusing_neutrons.py
--rw-r--r--   0        0        0        0 2024-02-13 14:24:12.365190 neutrowater-0.0.1/src/neutrowater/models/__init__.py
--rw-r--r--   0        0        0     3202 2024-04-19 12:55:44.208555 neutrowater-0.0.1/src/neutrowater/models/collisions.py
--rw-r--r--   0        0        0     2077 2024-04-15 16:56:53.158417 neutrowater-0.0.1/src/neutrowater/models/maxwell_boltzmann.py
--rw-r--r--   0        0        0     2879 2024-03-25 16:12:49.975967 neutrowater-0.0.1/src/neutrowater/models/neutrons.py
--rw-r--r--   0        0        0     1068 2024-03-25 16:12:49.975967 neutrowater-0.0.1/src/neutrowater/models/tank.py
--rw-r--r--   0        0        0     5818 2024-04-19 12:55:56.424639 neutrowater-0.0.1/src/neutrowater/post_measure.py
--rw-r--r--   0        0        0        0 2024-02-13 14:24:12.365190 neutrowater-0.0.1/src/neutrowater/process/__init__.py
--rw-r--r--   0        0        0     3252 2024-04-19 12:55:22.816402 neutrowater-0.0.1/src/neutrowater/process/angular_processor.py
--rw-r--r--   0        0        0     8055 2024-03-25 16:12:49.975967 neutrowater-0.0.1/src/neutrowater/process/data_processor.py
--rw-r--r--   0        0        0     2062 1970-01-01 00:00:00.000000 neutrowater-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-03-25 16:32:15.084916 neutrowater-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1125 2024-04-21 11:21:46.140905 neutrowater-0.0.2/README.md
+-rw-r--r--   0        0        0    13191 2024-04-21 10:27:18.112889 neutrowater-0.0.2/data/H_angular.txt
+-rw-r--r--   0        0        0   101958 2024-03-18 09:32:19.897984 neutrowater-0.0.2/data/O_angular.txt
+-rw-r--r--   0        0        0   173447 2024-03-29 01:17:23.637975 neutrowater-0.0.2/data/O_cross.pdf
+-rw-r--r--   0        0        0    16860 2024-01-24 14:31:22.785561 neutrowater-0.0.2/data/h_cross_a.txt
+-rw-r--r--   0        0        0    13362 2024-01-24 14:31:23.909567 neutrowater-0.0.2/data/h_cross_s.txt
+-rw-r--r--   0        0        0    13362 2024-01-24 14:31:25.525576 neutrowater-0.0.2/data/h_cross_t.txt
+-rw-r--r--   0        0        0    15619 2024-02-19 15:00:41.557842 neutrowater-0.0.2/data/mean_free_path.csv
+-rw-r--r--   0        0        0     1986 2024-04-09 10:01:17.892121 neutrowater-0.0.2/data/neutron_spectrum.txt
+-rw-r--r--   0        0        0     1951 2024-04-09 10:32:10.824020 neutrowater-0.0.2/data/neutron_spectrum_normalized.txt
+-rw-r--r--   0        0        0    18147 2024-01-24 14:57:54.587003 neutrowater-0.0.2/data/o_cross_a.txt
+-rw-r--r--   0        0        0    64249 2024-01-24 14:57:08.169669 neutrowater-0.0.2/data/o_cross_s.txt
+-rw-r--r--   0        0        0    62235 2024-01-24 14:58:08.047353 neutrowater-0.0.2/data/o_cross_t.txt
+-rw-r--r--   0        0        0     1420 2024-04-21 11:36:16.634074 neutrowater-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-01 11:50:16.012474 neutrowater-0.0.2/src/neutrowater/__init__.py
+-rw-r--r--   0        0        0     8276 2024-04-21 11:00:50.390604 neutrowater-0.0.2/src/neutrowater/diffusing_neutrons.py
+-rw-r--r--   0        0        0        0 2024-02-13 14:24:12.365190 neutrowater-0.0.2/src/neutrowater/models/__init__.py
+-rw-r--r--   0        0        0     3203 2024-04-21 10:28:48.726792 neutrowater-0.0.2/src/neutrowater/models/collisions.py
+-rw-r--r--   0        0        0     2077 2024-04-15 16:56:53.158417 neutrowater-0.0.2/src/neutrowater/models/maxwell_boltzmann.py
+-rw-r--r--   0        0        0     2879 2024-03-25 16:12:49.975967 neutrowater-0.0.2/src/neutrowater/models/neutrons.py
+-rw-r--r--   0        0        0     1076 2024-04-21 10:20:17.222774 neutrowater-0.0.2/src/neutrowater/models/tank.py
+-rw-r--r--   0        0        0     5818 2024-04-19 12:55:56.424639 neutrowater-0.0.2/src/neutrowater/post_measure.py
+-rw-r--r--   0        0        0        0 2024-02-13 14:24:12.365190 neutrowater-0.0.2/src/neutrowater/process/__init__.py
+-rw-r--r--   0        0        0     3252 2024-04-19 12:55:22.816402 neutrowater-0.0.2/src/neutrowater/process/angular_processor.py
+-rw-r--r--   0        0        0     8055 2024-03-25 16:12:49.975967 neutrowater-0.0.2/src/neutrowater/process/data_processor.py
+-rw-r--r--   0        0        0     2240 1970-01-01 00:00:00.000000 neutrowater-0.0.2/PKG-INFO
```

### Comparing `neutrowater-0.0.1/LICENSE` & `neutrowater-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neutrowater-0.0.1/README.md` & `neutrowater-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 
 <br />
 <br />
 <br />
 
 ## Documentation
 
-The [complete documentation](https://derkniessink.github.io/Neutrons/) of NeutroWater is hosted on Read the Docs.
+The [complete documentation](https://derkniessink.github.io/NeutroWater/) of NeutroWater is hosted on Read the Docs.
 
 <br />
 
 ## Instalation
 
 [Instalation instructions](https://derkniessink.github.io/NeutroWater/user_guide/) can be found under User Guide in the documentation.
```

### Comparing `neutrowater-0.0.1/pyproject.toml` & `neutrowater-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 [project]
-name = "neutrowater"
-version = "0.0.1"
+name = "NeutroWater"
+version = "0.0.2"
 authors = [
     {name = "DerkNiessink, email = derk@niessink.com"}
 ]
 description = "Monte Carlo simulation of neutron moderation"
 readme = "README.md"
-packages = [
-    { include = "neutrowater", from = "src" },
-]
+
+packages = [{ include = "neutrowater", from="src" }]
+include = ["data"]
+
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/DerkNiessink/neutrowater"
 Issues = "https://github.com/DerkNiessink/neutrowater/issues"
 
 [tool.poetry]
-name = "neutrowater"
-version = "0.0.1"
+name = "NeutroWater"
+version = "0.0.2"
 authors = ["DerkNiessink <derk@niessink.com>"]
 description = "Monte Carlo simulation of neutron moderation"
 readme = "README.md"
 packages = [
     { include = "neutrowater", from = "src" },
 ]
-
+include = ["data"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 scienceplots = "^2.1.1"
 numpy = "^1.26.4"
 matplotlib = "^3.8.2"
 pytest = "^8.0.0"
@@ -42,14 +43,18 @@
 scipy = "^1.12.0"
 seaborn = "^0.13.2"
 tqdm = "^4.66.2"
 ruff = "^0.2.1"
 numba = "^0.59.0"
 brokenaxes = "^0.6.0"
 ipywidgets = "^8.1.2"
+mkdocs = "^1.6.0"
+pymdown-extensions = "^10.8"
+mkdocs-glightbox = "^0.3.7"
+build = "^1.2.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
```

### Comparing `neutrowater-0.0.1/src/neutrowater/diffusing_neutrons.py` & `neutrowater-0.0.2/src/neutrowater/diffusing_neutrons.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     """
 
     nNeutrons: int
     molecule_structure: Sequence = (2, 1)
     nuclei_masses: Sequence = (1, 16)
     radius_tank: float = 1
     height_tank: float = 1
-    position_tank: Vector = np.array([0.0, 0.0, 0.0])
+    position_tank: tuple = (0.0, 0.0, 0.0)
     temperature: float = 293
 
     def __post_init__(self):
         self.total_data: Sequence[pd.DataFrame] = [
             pd.read_csv("../data/h_cross_t.txt", sep=r"\s+"),
             pd.read_csv("../data/o_cross_t.txt", sep=r"\s+"),
         ]
```

### Comparing `neutrowater-0.0.1/src/neutrowater/models/collisions.py` & `neutrowater-0.0.2/src/neutrowater/models/collisions.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 @dataclass
 class Collision:
     """
     Class to simulate the collisions of neutrons with atomic nuclei.
 
-    Args:
+    Args:D
         - initial_E (float): initial energy of the neutron.
         - initial_direction (Vector): initial direction of the neutron in the labframe.
         - mass (float): mass of the nucleus.
         - scattering_cosine (float): cosine of the scattering angle in the CM frame.
         - absorption (bool): flag to indicate if the collision is an absorption.
         - thermal (bool): flag to indicate if the collision is thermal.
```

### Comparing `neutrowater-0.0.1/src/neutrowater/models/maxwell_boltzmann.py` & `neutrowater-0.0.2/src/neutrowater/models/maxwell_boltzmann.py`

 * *Files identical despite different names*

### Comparing `neutrowater-0.0.1/src/neutrowater/models/neutrons.py` & `neutrowater-0.0.2/src/neutrowater/models/neutrons.py`

 * *Files identical despite different names*

### Comparing `neutrowater-0.0.1/src/neutrowater/models/tank.py` & `neutrowater-0.0.2/src/neutrowater/models/tank.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     """
     Class that holds the parameters of the tank, providing a method for
     checking if a position is inside the tank.
 
     Args:
         - radius (float): radius of the tank.
         - height (float): height of the tank.
-        - position (np.ndarray): position of the tank, default [0, 0, 0].
+        - position (tuple): position of the tank, default (0, 0, 0).
     """
 
     radius: float
     height: float
-    position: np.ndarray
+    position: tuple = (0.0, 0.0, 0.0)
 
     def __post_init__(self):
         """
         Calculate the volume and energy loss fraction.
         """
         self.volume = np.pi * self.radius**2 * self.height
```

### Comparing `neutrowater-0.0.1/src/neutrowater/post_measure.py` & `neutrowater-0.0.2/src/neutrowater/post_measure.py`

 * *Files identical despite different names*

### Comparing `neutrowater-0.0.1/src/neutrowater/process/angular_processor.py` & `neutrowater-0.0.2/src/neutrowater/process/angular_processor.py`

 * *Files identical despite different names*

### Comparing `neutrowater-0.0.1/src/neutrowater/process/data_processor.py` & `neutrowater-0.0.2/src/neutrowater/process/data_processor.py`

 * *Files identical despite different names*

### Comparing `neutrowater-0.0.1/PKG-INFO` & `neutrowater-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
-Name: neutrowater
-Version: 0.0.1
+Name: NeutroWater
+Version: 0.0.2
 Summary: Monte Carlo simulation of neutron moderation
 Author: DerkNiessink
 Author-email: derk@niessink.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: brokenaxes (>=0.6.0,<0.7.0)
+Requires-Dist: build (>=1.2.1,<2.0.0)
 Requires-Dist: ipykernel (>=6.29.1,<7.0.0)
 Requires-Dist: ipywidgets (>=8.1.2,<9.0.0)
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
+Requires-Dist: mkdocs (>=1.6.0,<2.0.0)
+Requires-Dist: mkdocs-glightbox (>=0.3.7,<0.4.0)
 Requires-Dist: numba (>=0.59.0,<0.60.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
+Requires-Dist: pymdown-extensions (>=10.8,<11.0)
 Requires-Dist: pytest (>=8.0.0,<9.0.0)
 Requires-Dist: ruff (>=0.2.1,<0.3.0)
 Requires-Dist: scienceplots (>=2.1.1,<3.0.0)
 Requires-Dist: scipy (>=1.12.0,<2.0.0)
 Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
@@ -37,15 +41,15 @@
 
 <br />
 <br />
 <br />
 
 ## Documentation
 
-The [complete documentation](https://derkniessink.github.io/Neutrons/) of NeutroWater is hosted on Read the Docs.
+The [complete documentation](https://derkniessink.github.io/NeutroWater/) of NeutroWater is hosted on Read the Docs.
 
 <br />
 
 ## Instalation
 
 [Instalation instructions](https://derkniessink.github.io/NeutroWater/user_guide/) can be found under User Guide in the documentation.
```


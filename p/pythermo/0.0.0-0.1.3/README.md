# Comparing `tmp/pythermo-0.0.0.tar.gz` & `tmp/pythermo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythermo-0.0.0.tar", last modified: Sat Apr 20 20:08:58 2024, max compression
+gzip compressed data, was "pythermo-0.1.3.tar", last modified: Sun Apr 21 20:04:53 2024, max compression
```

## Comparing `pythermo-0.0.0.tar` & `pythermo-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:08:58.078712 pythermo-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    32475 2024-04-20 20:08:53.000000 pythermo-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-20 20:08:58.078712 pythermo-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-20 20:08:53.000000 pythermo-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-20 20:08:53.000000 pythermo-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 20:08:58.078712 pythermo-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:08:58.074712 pythermo-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:08:58.078712 pythermo-0.0.0/src/pythermo/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-20 20:08:53.000000 pythermo-0.0.0/src/pythermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-20 20:08:53.000000 pythermo-0.0.0/src/pythermo/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    36747 2024-04-20 20:08:53.000000 pythermo-0.0.0/src/pythermo/crystal.py
--rw-r--r--   0 runner    (1001) docker     (127)    17718 2024-04-20 20:08:53.000000 pythermo-0.0.0/src/pythermo/tT_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-04-20 20:08:53.000000 pythermo-0.0.0/src/pythermo/tT_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:08:58.078712 pythermo-0.0.0/src/pythermo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-20 20:08:58.000000 pythermo-0.0.0/src/pythermo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-20 20:08:58.000000 pythermo-0.0.0/src/pythermo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 20:08:58.000000 pythermo-0.0.0/src/pythermo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 20:08:58.000000 pythermo-0.0.0/src/pythermo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:08:58.078712 pythermo-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-20 20:08:53.000000 pythermo-0.0.0/tests/test_crystal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-20 20:08:53.000000 pythermo-0.0.0/tests/test_tT_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-20 20:08:53.000000 pythermo-0.0.0/tests/test_tT_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:04:53.219792 pythermo-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    32475 2024-04-21 20:04:49.000000 pythermo-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-21 20:04:53.219792 pythermo-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-21 20:04:49.000000 pythermo-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-21 20:04:49.000000 pythermo-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 20:04:53.219792 pythermo-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:04:53.215792 pythermo-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:04:53.219792 pythermo-0.1.3/src/pythermo/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-21 20:04:49.000000 pythermo-0.1.3/src/pythermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-21 20:04:49.000000 pythermo-0.1.3/src/pythermo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36747 2024-04-21 20:04:49.000000 pythermo-0.1.3/src/pythermo/crystal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18084 2024-04-21 20:04:49.000000 pythermo-0.1.3/src/pythermo/tT_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-04-21 20:04:49.000000 pythermo-0.1.3/src/pythermo/tT_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:04:53.219792 pythermo-0.1.3/src/pythermo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-21 20:04:53.000000 pythermo-0.1.3/src/pythermo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-21 20:04:53.000000 pythermo-0.1.3/src/pythermo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 20:04:53.000000 pythermo-0.1.3/src/pythermo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-21 20:04:53.000000 pythermo-0.1.3/src/pythermo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 20:04:53.000000 pythermo-0.1.3/src/pythermo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:04:53.219792 pythermo-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-21 20:04:49.000000 pythermo-0.1.3/tests/test_crystal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-21 20:04:49.000000 pythermo-0.1.3/tests/test_tT_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-21 20:04:49.000000 pythermo-0.1.3/tests/test_tT_path.py
```

### Comparing `pythermo-0.0.0/LICENSE` & `pythermo-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pythermo-0.0.0/PKG-INFO` & `pythermo-0.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,60 @@
 Metadata-Version: 2.1
 Name: pythermo
-Version: 0.0.0
+Version: 0.1.3
 Summary: Tools for performing computational tasks in the field of low-temperature thermochronology.
 Author-email: William Guenthner <wrg@illinois.edu>
 Project-URL: Homepage, https://github.com/OpenThermochronology/PyThermo
 Project-URL: Issues, https://github.com/OpenThermochronology/PyThermo/issues
 Keywords: thermochronology,zircon,apatite,geology,diffusion,geochronology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
 
 # PyThermo
 
 [![DOI](osf_io_BNUVZ.svg)](https://doi.org/10.17605/OSF.IO/BNUVZ)
-[![CI][ci-img]][ci-url]
+[CI][ci-url]
 
 A set of classes and methods for performing various modeling and computational tasks in the field of low-temperature thermochronology. The current focus is on forward modeling of apatite and zircon (U-Th)/He data using various diffusion and damage annealing kinetic models. Future releases will expand upon the available kinetic models and mineral systems, and introduce additional methods, such as forward modeling of Arrhenius relationships.
 
 The primary objective of this software is to provide an open-source, python-based toolkit for user adaptability and experimentation. The software includes routines for forward modeling and data plotting at higher levels that can be run in a simple fashion, but lower level algorithms are accessible as well. To that end, a secondary objective of this software is as a learning tool to remove some of the black box nature of thermal history modeling routines. Several methods are included (for example, a tridiagonal matrix solver) for instructional purposes, although the main program calls nominally faster scipy routines.
 
 ## Organization
 
 The source code consists of three separate classes and accompanying methods and/or subclasses. `crystal.py` contains the class `crystal` and currently two sub-classes `apatite` and `zircon`. Methods are devoted to calculating and parameterizing damage-diffusivity relationships and numerically solving the diffusion equation using a Crank-Nicolson approach. `tT_path.py` methods interpolate and discretize time-temperature (tT) paths from a handful of tT points, and calculate fission track annealing for apatite and zircon using the equivalent time concept. `tT_model.py` methods currently allow for one particular approach to forward modeling and plotting (U-Th)/He date-effective Uranium (eU) trends.
 
+## Requirements
+
+If you've installed Python through the open data science platform [Anaconda](https://www.anaconda.com/download), you should be all set. In detail, the specific libraries you'll need to have installed are:
+
+* Numpy
+* Scipy
+* Matplotlib
+* Pandas
+
 ## Installation
 
-Eventually, PyThermo will be installed as a package by using pip. For now, you can download the 4 python files found in \src and save them to your working directory.
+PyThermo can be installed as a package by using pip (see this [helpful](https://packaging.python.org/en/latest/tutorials/installing-packages/) guide for using pip if you are unfamiliar):
+
+```python-repl
+pip install pythermo
+```
+
+ You can alternatively download the `/src` folder and place it in your working directory. See the `template.ipynb` file in the `examples` folder for usage under either circumstance.
 
 ## Usage
 
-Once you've downloaded the python files, and if you're just interested in running some forward models, the quickest way to get started is to modify the Jupyter Notebook file that is included in the `examples` folder. The notebook contains markdown and code that explains and demonstrates forward model date-eU comparisons for the apatite and zircon (U-Th)/He system. The forward modeling method is one particular approach and you can (and should!) modify the forward modeling methods to suite your own needs.The `tT_path` and `crystal` classes contain several methods that you may want to call and/or adapt for your own needs. Please read the descriptions for each method in the source code for more details.
+It is recommended that you use this package in [Jupyter Notebooks](https://jupyter.org), which are included in the [Anaconda](https://www.anaconda.com/download) platform. Once you've downloaded or installed the package, and if you're just interested in running some forward models, the quickest way to get started is to modify the Jupyter Notebook file `template.ipynb` that is included in the `examples` folder. The notebook contains markdown and code that explains and demonstrates forward model date-eU comparisons for the apatite and zircon (U-Th)/He system. The forward modeling method is one particular approach and you can (and should!) call lower level methods to suite your needs. The `tT_path` and `crystal` classes contain several methods that you may want to call. A basic example of one way to use lower-level methods is included in `template.ipynb`. Please read the descriptions for each method in the source code for more details.
 
 ## Citation
 
 You can find various citation styles for this package [here](https://doi.org/10.17605/OSF.IO/BNUVZ).
 
 [ci-img]: https://github.com/OpenThermochronology/PyThermo/actions/workflows/CI.yml/badge.svg?branch=main
 [ci-url]: https://github.com/OpenThermochronology/PyThermo/actions/workflows/CI.yml
```

### Comparing `pythermo-0.0.0/README.md` & `pythermo-0.1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,42 @@
 # PyThermo
 
 [![DOI](osf_io_BNUVZ.svg)](https://doi.org/10.17605/OSF.IO/BNUVZ)
-[![CI][ci-img]][ci-url]
+[CI][ci-url]
 
 A set of classes and methods for performing various modeling and computational tasks in the field of low-temperature thermochronology. The current focus is on forward modeling of apatite and zircon (U-Th)/He data using various diffusion and damage annealing kinetic models. Future releases will expand upon the available kinetic models and mineral systems, and introduce additional methods, such as forward modeling of Arrhenius relationships.
 
 The primary objective of this software is to provide an open-source, python-based toolkit for user adaptability and experimentation. The software includes routines for forward modeling and data plotting at higher levels that can be run in a simple fashion, but lower level algorithms are accessible as well. To that end, a secondary objective of this software is as a learning tool to remove some of the black box nature of thermal history modeling routines. Several methods are included (for example, a tridiagonal matrix solver) for instructional purposes, although the main program calls nominally faster scipy routines.
 
 ## Organization
 
 The source code consists of three separate classes and accompanying methods and/or subclasses. `crystal.py` contains the class `crystal` and currently two sub-classes `apatite` and `zircon`. Methods are devoted to calculating and parameterizing damage-diffusivity relationships and numerically solving the diffusion equation using a Crank-Nicolson approach. `tT_path.py` methods interpolate and discretize time-temperature (tT) paths from a handful of tT points, and calculate fission track annealing for apatite and zircon using the equivalent time concept. `tT_model.py` methods currently allow for one particular approach to forward modeling and plotting (U-Th)/He date-effective Uranium (eU) trends.
 
+## Requirements
+
+If you've installed Python through the open data science platform [Anaconda](https://www.anaconda.com/download), you should be all set. In detail, the specific libraries you'll need to have installed are:
+
+* Numpy
+* Scipy
+* Matplotlib
+* Pandas
+
 ## Installation
 
-Eventually, PyThermo will be installed as a package by using pip. For now, you can download the 4 python files found in \src and save them to your working directory.
+PyThermo can be installed as a package by using pip (see this [helpful](https://packaging.python.org/en/latest/tutorials/installing-packages/) guide for using pip if you are unfamiliar):
+
+```python-repl
+pip install pythermo
+```
+
+ You can alternatively download the `/src` folder and place it in your working directory. See the `template.ipynb` file in the `examples` folder for usage under either circumstance.
 
 ## Usage
 
-Once you've downloaded the python files, and if you're just interested in running some forward models, the quickest way to get started is to modify the Jupyter Notebook file that is included in the `examples` folder. The notebook contains markdown and code that explains and demonstrates forward model date-eU comparisons for the apatite and zircon (U-Th)/He system. The forward modeling method is one particular approach and you can (and should!) modify the forward modeling methods to suite your own needs.The `tT_path` and `crystal` classes contain several methods that you may want to call and/or adapt for your own needs. Please read the descriptions for each method in the source code for more details.
+It is recommended that you use this package in [Jupyter Notebooks](https://jupyter.org), which are included in the [Anaconda](https://www.anaconda.com/download) platform. Once you've downloaded or installed the package, and if you're just interested in running some forward models, the quickest way to get started is to modify the Jupyter Notebook file `template.ipynb` that is included in the `examples` folder. The notebook contains markdown and code that explains and demonstrates forward model date-eU comparisons for the apatite and zircon (U-Th)/He system. The forward modeling method is one particular approach and you can (and should!) call lower level methods to suite your needs. The `tT_path` and `crystal` classes contain several methods that you may want to call. A basic example of one way to use lower-level methods is included in `template.ipynb`. Please read the descriptions for each method in the source code for more details.
 
 ## Citation
 
 You can find various citation styles for this package [here](https://doi.org/10.17605/OSF.IO/BNUVZ).
 
 [ci-img]: https://github.com/OpenThermochronology/PyThermo/actions/workflows/CI.yml/badge.svg?branch=main
 [ci-url]: https://github.com/OpenThermochronology/PyThermo/actions/workflows/CI.yml
```

### Comparing `pythermo-0.0.0/pyproject.toml` & `pythermo-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pythermo"
-dynamic = ["version"]
+version = "0.1.3"
+dependencies = [
+  "numpy",
+  "scipy",
+  "matplotlib",
+]
 authors = [
   { name="William Guenthner", email="wrg@illinois.edu" },
 ]
 description = "Tools for performing computational tasks in the field of low-temperature thermochronology."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["thermochronology","zircon","apatite","geology","diffusion","geochronology"]
```

### Comparing `pythermo-0.0.0/src/pythermo/__init__.py` & `pythermo-0.1.3/src/pythermo/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,13 @@
 
     - .tT_model     : Methods for modeling and plotting thermochronometric date results for comparison to measured data sets. A key focus here is thermal history modeling.
 
     - .constants    : Important universal constants used by the various modules.
 
 """
 
-__version__ = '0.1.0'
-
 __all__ = ['constants','crystal','tT_path','tT_model']
 
 from .constants import *
 from .crystal import *
 from .tT_path import *
 from .tT_model import *
```

### Comparing `pythermo-0.0.0/src/pythermo/constants.py` & `pythermo-0.1.3/src/pythermo/constants.py`

 * *Files identical despite different names*

### Comparing `pythermo-0.0.0/src/pythermo/crystal.py` & `pythermo-0.1.3/src/pythermo/crystal.py`

 * *Files identical despite different names*

### Comparing `pythermo-0.0.0/src/pythermo/tT_model.py` & `pythermo-0.1.3/src/pythermo/tT_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """ 
 tT_model.py
 
 Particular approaches to forward modeling and plotting apatite and zircon (U-Th)/He date-effective uranium (eU) relationships.
 
 """
 import matplotlib.pyplot as plt
+import matplotlib.cm as mplcm
+import matplotlib.colors as colors
 from cycler import cycler
 from .constants import np
 from .crystal import apatite, zircon
 from .tT_path import tT_path
 
 class tT_model:
     def __init__(self, grain_in, tT_in, obs_data=None, temp_precision=5):
@@ -267,19 +269,23 @@
 
         #maximum values for setting plot axis dimensions
         date_max = 0
         eU_max = 0
         time_max = 0
         temp_max = 0
 
-        #set up color strings, if greater than 8 date-eU/tT sets, switch to viridis gradational color scheme
-        if np.size(model_data,1)/3 < 8:
+        #set up color strings, if greater than 8 date-eU/tT sets, switch to plasma gradational color scheme
+        if np.size(model_data,1)/3 <= 8:
             color_options = ['xkcd:black','xkcd:royal blue','xkcd:red','xkcd:sky','xkcd:lime','xkcd:dark purple','xkcd:rose','xkcd:grey']
         else:
-            color_options = []
+            num_of_colors = np.size(model_data,1)/3
+            color_map = plt.get_cmap('plasma')
+            color_norm = colors.Normalize(vmin=0, vmax=num_of_colors-1)
+            scalar_map = mplcm.ScalarMappable(norm=color_norm, cmap=color_map)
+            color_options = [scalar_map.to_rgba(i) for i in range(num_of_colors)]
 
         #line option cycler for model comparisons
         line_options = cycler(line_style=['-','--',':','-.'])
 
         #plot date-eU trends
         #assumes that the date-eU trends for each tT plot are in 3-column groups, in this order: date, eU, grain size
         for i in range(0,np.size(model_data,1),3):
```

### Comparing `pythermo-0.0.0/src/pythermo/tT_path.py` & `pythermo-0.1.3/src/pythermo/tT_path.py`

 * *Files identical despite different names*

### Comparing `pythermo-0.0.0/src/pythermo.egg-info/PKG-INFO` & `pythermo-0.1.3/src/pythermo.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,60 @@
 Metadata-Version: 2.1
 Name: pythermo
-Version: 0.0.0
+Version: 0.1.3
 Summary: Tools for performing computational tasks in the field of low-temperature thermochronology.
 Author-email: William Guenthner <wrg@illinois.edu>
 Project-URL: Homepage, https://github.com/OpenThermochronology/PyThermo
 Project-URL: Issues, https://github.com/OpenThermochronology/PyThermo/issues
 Keywords: thermochronology,zircon,apatite,geology,diffusion,geochronology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
 
 # PyThermo
 
 [![DOI](osf_io_BNUVZ.svg)](https://doi.org/10.17605/OSF.IO/BNUVZ)
-[![CI][ci-img]][ci-url]
+[CI][ci-url]
 
 A set of classes and methods for performing various modeling and computational tasks in the field of low-temperature thermochronology. The current focus is on forward modeling of apatite and zircon (U-Th)/He data using various diffusion and damage annealing kinetic models. Future releases will expand upon the available kinetic models and mineral systems, and introduce additional methods, such as forward modeling of Arrhenius relationships.
 
 The primary objective of this software is to provide an open-source, python-based toolkit for user adaptability and experimentation. The software includes routines for forward modeling and data plotting at higher levels that can be run in a simple fashion, but lower level algorithms are accessible as well. To that end, a secondary objective of this software is as a learning tool to remove some of the black box nature of thermal history modeling routines. Several methods are included (for example, a tridiagonal matrix solver) for instructional purposes, although the main program calls nominally faster scipy routines.
 
 ## Organization
 
 The source code consists of three separate classes and accompanying methods and/or subclasses. `crystal.py` contains the class `crystal` and currently two sub-classes `apatite` and `zircon`. Methods are devoted to calculating and parameterizing damage-diffusivity relationships and numerically solving the diffusion equation using a Crank-Nicolson approach. `tT_path.py` methods interpolate and discretize time-temperature (tT) paths from a handful of tT points, and calculate fission track annealing for apatite and zircon using the equivalent time concept. `tT_model.py` methods currently allow for one particular approach to forward modeling and plotting (U-Th)/He date-effective Uranium (eU) trends.
 
+## Requirements
+
+If you've installed Python through the open data science platform [Anaconda](https://www.anaconda.com/download), you should be all set. In detail, the specific libraries you'll need to have installed are:
+
+* Numpy
+* Scipy
+* Matplotlib
+* Pandas
+
 ## Installation
 
-Eventually, PyThermo will be installed as a package by using pip. For now, you can download the 4 python files found in \src and save them to your working directory.
+PyThermo can be installed as a package by using pip (see this [helpful](https://packaging.python.org/en/latest/tutorials/installing-packages/) guide for using pip if you are unfamiliar):
+
+```python-repl
+pip install pythermo
+```
+
+ You can alternatively download the `/src` folder and place it in your working directory. See the `template.ipynb` file in the `examples` folder for usage under either circumstance.
 
 ## Usage
 
-Once you've downloaded the python files, and if you're just interested in running some forward models, the quickest way to get started is to modify the Jupyter Notebook file that is included in the `examples` folder. The notebook contains markdown and code that explains and demonstrates forward model date-eU comparisons for the apatite and zircon (U-Th)/He system. The forward modeling method is one particular approach and you can (and should!) modify the forward modeling methods to suite your own needs.The `tT_path` and `crystal` classes contain several methods that you may want to call and/or adapt for your own needs. Please read the descriptions for each method in the source code for more details.
+It is recommended that you use this package in [Jupyter Notebooks](https://jupyter.org), which are included in the [Anaconda](https://www.anaconda.com/download) platform. Once you've downloaded or installed the package, and if you're just interested in running some forward models, the quickest way to get started is to modify the Jupyter Notebook file `template.ipynb` that is included in the `examples` folder. The notebook contains markdown and code that explains and demonstrates forward model date-eU comparisons for the apatite and zircon (U-Th)/He system. The forward modeling method is one particular approach and you can (and should!) call lower level methods to suite your needs. The `tT_path` and `crystal` classes contain several methods that you may want to call. A basic example of one way to use lower-level methods is included in `template.ipynb`. Please read the descriptions for each method in the source code for more details.
 
 ## Citation
 
 You can find various citation styles for this package [here](https://doi.org/10.17605/OSF.IO/BNUVZ).
 
 [ci-img]: https://github.com/OpenThermochronology/PyThermo/actions/workflows/CI.yml/badge.svg?branch=main
 [ci-url]: https://github.com/OpenThermochronology/PyThermo/actions/workflows/CI.yml
```

### Comparing `pythermo-0.0.0/tests/test_crystal.py` & `pythermo-0.1.3/tests/test_crystal.py`

 * *Files identical despite different names*

### Comparing `pythermo-0.0.0/tests/test_tT_model.py` & `pythermo-0.1.3/tests/test_tT_model.py`

 * *Files identical despite different names*

### Comparing `pythermo-0.0.0/tests/test_tT_path.py` & `pythermo-0.1.3/tests/test_tT_path.py`

 * *Files identical despite different names*


# Comparing `tmp/litespi-2023.12.tar.gz` & `tmp/litespi-2023.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litespi-2023.12.tar", last modified: Sun Apr 21 19:47:45 2024, max compression
+gzip compressed data, was "litespi-2023.8.tar", last modified: Sun Apr 21 19:48:27 2024, max compression
```

## Comparing `litespi-2023.12.tar` & `litespi-2023.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:47:45.393128 litespi-2023.12/
--rw-r--r--   0 timkpaine   (501) staff       (20)     1333 2024-04-21 19:46:48.000000 litespi-2023.12/LICENSE
--rw-r--r--   0 timkpaine   (501) staff       (20)     2474 2024-04-21 19:47:45.392815 litespi-2023.12/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)     2152 2024-04-21 19:46:48.000000 litespi-2023.12/README.md
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:47:45.387462 litespi-2023.12/litespi/
--rw-r--r--   0 timkpaine   (501) staff       (20)     3383 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4943 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/clkgen.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1136 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/common.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:47:45.389144 litespi-2023.12/litespi/core/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/core/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3145 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/core/master.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6343 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/core/mmap.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2983 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/crossbar.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:47:45.389355 litespi-2023.12/litespi/frontend/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/frontend/__init__.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8828 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/gen.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2011 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/ids.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:47:45.390412 litespi-2023.12/litespi/modules/
--rw-r--r--   0 timkpaine   (501) staff       (20)      416 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/modules/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)   208880 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/modules/generated_modules.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3197 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/modules/modules.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7833 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/opcodes.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:47:45.391620 litespi-2023.12/litespi/phy/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/phy/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2459 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/phy/generic.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6286 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/phy/generic_ddr.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7516 2024-04-21 19:46:56.000000 litespi-2023.12/litespi/phy/generic_sdr.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4775 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/phy/model.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2174 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/spi_nor_features.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5494 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/spi_nor_flash_metasizes.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5135 2024-04-21 19:46:48.000000 litespi-2023.12/litespi/spi_nor_flash_module.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:47:45.392483 litespi-2023.12/litespi.egg-info/
--rw-r--r--   0 timkpaine   (501) staff       (20)     2474 2024-04-21 19:47:45.000000 litespi-2023.12/litespi.egg-info/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)      764 2024-04-21 19:47:45.000000 litespi-2023.12/litespi.egg-info/SOURCES.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-21 19:47:45.000000 litespi-2023.12/litespi.egg-info/dependency_links.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       49 2024-04-21 19:47:45.000000 litespi-2023.12/litespi.egg-info/entry_points.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        8 2024-04-21 19:47:45.000000 litespi-2023.12/litespi.egg-info/top_level.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       38 2024-04-21 19:47:45.393186 litespi-2023.12/setup.cfg
--rwxr-xr-x   0 timkpaine   (501) staff       (20)      974 2024-04-21 19:47:40.000000 litespi-2023.12/setup.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:47:45.392193 litespi-2023.12/test/
--rw-r--r--   0 timkpaine   (501) staff       (20)     4099 2024-04-21 19:46:48.000000 litespi-2023.12/test/test_flash_module.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3133 2024-04-21 19:46:48.000000 litespi-2023.12/test/test_spi_mmap.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:48:27.656048 litespi-2023.8/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1333 2024-04-21 19:46:48.000000 litespi-2023.8/LICENSE
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2473 2024-04-21 19:48:27.655760 litespi-2023.8/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2152 2024-04-21 19:46:48.000000 litespi-2023.8/README.md
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:48:27.650969 litespi-2023.8/litespi/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3383 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4943 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/clkgen.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1136 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/common.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:48:27.652379 litespi-2023.8/litespi/core/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/core/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3145 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/core/master.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6343 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/core/mmap.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2983 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/crossbar.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:48:27.652569 litespi-2023.8/litespi/frontend/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/frontend/__init__.py
+-rwxr-xr-x   0 timkpaine   (501) staff       (20)     8828 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/gen.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2011 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/ids.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:48:27.653762 litespi-2023.8/litespi/modules/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      416 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/modules/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)   208880 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/modules/generated_modules.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3197 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/modules/modules.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     7833 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/opcodes.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:48:27.654873 litespi-2023.8/litespi/phy/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/phy/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2459 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/phy/generic.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6286 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/phy/generic_ddr.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     7516 2024-04-21 19:46:56.000000 litespi-2023.8/litespi/phy/generic_sdr.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4775 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/phy/model.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2174 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/spi_nor_features.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5494 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/spi_nor_flash_metasizes.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5135 2024-04-21 19:46:48.000000 litespi-2023.8/litespi/spi_nor_flash_module.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:48:27.655495 litespi-2023.8/litespi.egg-info/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2473 2024-04-21 19:48:27.000000 litespi-2023.8/litespi.egg-info/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)      764 2024-04-21 19:48:27.000000 litespi-2023.8/litespi.egg-info/SOURCES.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-21 19:48:27.000000 litespi-2023.8/litespi.egg-info/dependency_links.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       49 2024-04-21 19:48:27.000000 litespi-2023.8/litespi.egg-info/entry_points.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        8 2024-04-21 19:48:27.000000 litespi-2023.8/litespi.egg-info/top_level.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       38 2024-04-21 19:48:27.656108 litespi-2023.8/setup.cfg
+-rwxr-xr-x   0 timkpaine   (501) staff       (20)      840 2024-04-21 19:48:24.000000 litespi-2023.8/setup.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-21 19:48:27.655247 litespi-2023.8/test/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4099 2024-04-21 19:46:48.000000 litespi-2023.8/test/test_flash_module.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3133 2024-04-21 19:46:48.000000 litespi-2023.8/test/test_spi_mmap.py
```

### Comparing `litespi-2023.12/LICENSE` & `litespi-2023.8/LICENSE`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/PKG-INFO` & `litespi-2023.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: litespi
-Version: 2023.12
+Version: 2023.8
 Summary: Small footprint and configurable SPI core
 Home-page: https://github.com/litex-hub
 Download-URL: https://github.com/litex-hub/litespi
 Author: LiteSPI Developers
 License: BSD
-Requires-Python: ~=3.7
+Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ```
               __   _ __      _______  ____
              / /  (_) /____ / __/ _ \/  _/
             / /__/ / __/ -_)\ \/ ___// /
```

### Comparing `litespi-2023.12/README.md` & `litespi-2023.8/README.md`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/__init__.py` & `litespi-2023.8/litespi/__init__.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/clkgen.py` & `litespi-2023.8/litespi/clkgen.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/common.py` & `litespi-2023.8/litespi/common.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/core/master.py` & `litespi-2023.8/litespi/core/master.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/core/mmap.py` & `litespi-2023.8/litespi/core/mmap.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/crossbar.py` & `litespi-2023.8/litespi/crossbar.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/gen.py` & `litespi-2023.8/litespi/gen.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/ids.py` & `litespi-2023.8/litespi/ids.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/modules/generated_modules.py` & `litespi-2023.8/litespi/modules/generated_modules.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/modules/modules.py` & `litespi-2023.8/litespi/modules/modules.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/opcodes.py` & `litespi-2023.8/litespi/opcodes.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/phy/generic.py` & `litespi-2023.8/litespi/phy/generic.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/phy/generic_ddr.py` & `litespi-2023.8/litespi/phy/generic_ddr.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/phy/generic_sdr.py` & `litespi-2023.8/litespi/phy/generic_sdr.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/phy/model.py` & `litespi-2023.8/litespi/phy/model.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/spi_nor_features.py` & `litespi-2023.8/litespi/spi_nor_features.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/spi_nor_flash_metasizes.py` & `litespi-2023.8/litespi/spi_nor_flash_metasizes.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi/spi_nor_flash_module.py` & `litespi-2023.8/litespi/spi_nor_flash_module.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/litespi.egg-info/PKG-INFO` & `litespi-2023.8/litespi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: litespi
-Version: 2023.12
+Version: 2023.8
 Summary: Small footprint and configurable SPI core
 Home-page: https://github.com/litex-hub
 Download-URL: https://github.com/litex-hub/litespi
 Author: LiteSPI Developers
 License: BSD
-Requires-Python: ~=3.7
+Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ```
               __   _ __      _______  ____
              / /  (_) /____ / __/ _ \/  _/
             / /__/ / __/ -_)\ \/ ___// /
```

### Comparing `litespi-2023.12/litespi.egg-info/SOURCES.txt` & `litespi-2023.8/litespi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/setup.py` & `litespi-2023.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="utf-8") as fp:
     long_description = fp.read()
 
 setup(
-    name                 = "litespi",
-    description          = "Small footprint and configurable SPI core",
-    version                       = "2023.12",
+    name="litespi",
+    description="Small footprint and configurable SPI core",
+    author="LiteSPI Developers",
+    version                       = "2023.08",
     long_description              = long_description,
     long_description_content_type = "text/markdown",
-    author               = "LiteSPI Developers",
-    url                  = "https://github.com/litex-hub",
-    download_url         = "https://github.com/litex-hub/litespi",
-    test_suite           = "test",
-    license              = "BSD",
-    python_requires      = "~=3.7",
-    packages             = find_packages(exclude=("test*", "sim*", "doc*", "examples*")),
-    include_package_data = True,
-    entry_points         = {
+    url="https://github.com/litex-hub",
+    download_url="https://github.com/litex-hub/litespi",
+    test_suite="test",
+    license="BSD",
+    python_requires="~=3.6",
+    packages=find_packages(exclude=("test*", "sim*", "doc*", "examples*")),
+    include_package_data=True,
+    entry_points={
         "console_scripts": [
             "litespi_gen=litespi.gen:main",
         ],
     },
 )
```

### Comparing `litespi-2023.12/test/test_flash_module.py` & `litespi-2023.8/test/test_flash_module.py`

 * *Files identical despite different names*

### Comparing `litespi-2023.12/test/test_spi_mmap.py` & `litespi-2023.8/test/test_spi_mmap.py`

 * *Files identical despite different names*


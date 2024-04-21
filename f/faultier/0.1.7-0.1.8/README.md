# Comparing `tmp/faultier-0.1.7.tar.gz` & `tmp/faultier-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faultier-0.1.7.tar", last modified: Sun Apr 21 16:25:38 2024, max compression
+gzip compressed data, was "faultier-0.1.8.tar", last modified: Sun Apr 21 16:27:24 2024, max compression
```

## Comparing `faultier-0.1.7.tar` & `faultier-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:25:38.081514 faultier-0.1.7/
--rw-r--r--   0 thomas     (501) staff       (20)      240 2024-04-21 16:25:38.081327 faultier-0.1.7/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)       85 2024-03-11 10:46:46.000000 faultier-0.1.7/README.md
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:25:38.067565 faultier-0.1.7/faultier/
--rw-r--r--   0 thomas     (501) staff       (20)     6746 2024-04-21 14:54:55.000000 faultier-0.1.7/faultier/FaulterVis.py
--rw-r--r--   0 thomas     (501) staff       (20)     9662 2024-04-21 14:54:24.000000 faultier-0.1.7/faultier/Faultier.py
--rw-r--r--   0 thomas     (501) staff       (20)     2382 2024-04-21 14:31:26.000000 faultier-0.1.7/faultier/LivePlot.py
--rw-r--r--   0 thomas     (501) staff       (20)     1067 2024-03-16 14:18:41.000000 faultier-0.1.7/faultier/RandomOrderGenerator.py
--rw-r--r--   0 thomas     (501) staff       (20)      129 2024-04-21 14:31:08.000000 faultier-0.1.7/faultier/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:25:38.071967 faultier-0.1.7/faultier/docs/
--rw-r--r--   0 thomas     (501) staff       (20)   102775 2024-04-21 16:24:58.000000 faultier-0.1.7/faultier/docs/sideview.svg
--rw-r--r--   0 thomas     (501) staff       (20)   350221 2024-04-21 16:24:58.000000 faultier-0.1.7/faultier/docs/topview.svg
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:25:38.079363 faultier-0.1.7/faultier/example_firmware/
--rw-r--r--   0 thomas     (501) staff       (20)    72892 2024-03-11 11:18:12.000000 faultier-0.1.7/faultier/example_firmware/nrf52832_xxaa.hex
--rw-r--r--   0 thomas     (501) staff       (20)   429491 2024-03-11 11:18:12.000000 faultier-0.1.7/faultier/example_firmware/s132_nrf52_7.2.0_softdevice.hex
--rw-r--r--   0 thomas     (501) staff       (20)     6185 2024-03-11 10:46:48.000000 faultier-0.1.7/faultier/faultier_pb2.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:25:38.081135 faultier-0.1.7/faultier.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)      240 2024-04-21 16:25:38.000000 faultier-0.1.7/faultier.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      482 2024-04-21 16:25:38.000000 faultier-0.1.7/faultier.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2024-04-21 16:25:38.000000 faultier-0.1.7/faultier.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)       23 2024-04-21 16:25:38.000000 faultier-0.1.7/faultier.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)        9 2024-04-21 16:25:38.000000 faultier-0.1.7/faultier.egg-info/top_level.txt
--rw-r--r--   0 thomas     (501) staff       (20)      991 2024-04-21 16:25:24.000000 faultier-0.1.7/pyproject.toml
--rw-r--r--   0 thomas     (501) staff       (20)       38 2024-04-21 16:25:38.081559 faultier-0.1.7/setup.cfg
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:27:24.008509 faultier-0.1.8/
+-rw-r--r--   0 thomas     (501) staff       (20)      240 2024-04-21 16:27:24.008325 faultier-0.1.8/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)       85 2024-03-11 10:46:46.000000 faultier-0.1.8/README.md
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:27:24.003785 faultier-0.1.8/faultier/
+-rw-r--r--   0 thomas     (501) staff       (20)     6737 2024-04-21 16:26:57.000000 faultier-0.1.8/faultier/FaulterVis.py
+-rw-r--r--   0 thomas     (501) staff       (20)     9662 2024-04-21 14:54:24.000000 faultier-0.1.8/faultier/Faultier.py
+-rw-r--r--   0 thomas     (501) staff       (20)     2382 2024-04-21 14:31:26.000000 faultier-0.1.8/faultier/LivePlot.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1067 2024-03-16 14:18:41.000000 faultier-0.1.8/faultier/RandomOrderGenerator.py
+-rw-r--r--   0 thomas     (501) staff       (20)      129 2024-04-21 14:31:08.000000 faultier-0.1.8/faultier/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:27:24.004852 faultier-0.1.8/faultier/docs/
+-rw-r--r--   0 thomas     (501) staff       (20)   102775 2024-04-21 16:24:58.000000 faultier-0.1.8/faultier/docs/sideview.svg
+-rw-r--r--   0 thomas     (501) staff       (20)   350221 2024-04-21 16:24:58.000000 faultier-0.1.8/faultier/docs/topview.svg
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:27:24.006612 faultier-0.1.8/faultier/example_firmware/
+-rw-r--r--   0 thomas     (501) staff       (20)    72892 2024-03-11 11:18:12.000000 faultier-0.1.8/faultier/example_firmware/nrf52832_xxaa.hex
+-rw-r--r--   0 thomas     (501) staff       (20)   429491 2024-03-11 11:18:12.000000 faultier-0.1.8/faultier/example_firmware/s132_nrf52_7.2.0_softdevice.hex
+-rw-r--r--   0 thomas     (501) staff       (20)     6185 2024-03-11 10:46:48.000000 faultier-0.1.8/faultier/faultier_pb2.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 16:27:24.008122 faultier-0.1.8/faultier.egg-info/
+-rw-r--r--   0 thomas     (501) staff       (20)      240 2024-04-21 16:27:23.000000 faultier-0.1.8/faultier.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)      482 2024-04-21 16:27:24.000000 faultier-0.1.8/faultier.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        1 2024-04-21 16:27:23.000000 faultier-0.1.8/faultier.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       23 2024-04-21 16:27:23.000000 faultier-0.1.8/faultier.egg-info/requires.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        9 2024-04-21 16:27:23.000000 faultier-0.1.8/faultier.egg-info/top_level.txt
+-rw-r--r--   0 thomas     (501) staff       (20)      991 2024-04-21 16:27:20.000000 faultier-0.1.8/pyproject.toml
+-rw-r--r--   0 thomas     (501) staff       (20)       38 2024-04-21 16:27:24.008550 faultier-0.1.8/setup.cfg
```

### Comparing `faultier-0.1.7/faultier/FaulterVis.py` & `faultier-0.1.8/faultier/FaulterVis.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         return img_tag
 
     def show(self):
         display(HTML(self.create_tag()))
 
     @staticmethod
     def show_stm32_glitch_configuration():
-        fv = FaultierVis(MODULE_DIR + "/../docs/topview.svg")
+        fv = FaultierVis(MODULE_DIR + "/docs/topview.svg")
         fv.replace_text("text_crowbar", "To STM32 VCore")
         fv.replace_text("text_mux0", "To STM32 VCC")
         fv.replace_text("text_ext0", "To STM32 RST")
         fv.replace_text("text_ext1", "Unused", fill="#999")
         fv.show()
         fv = FaultierVis(MODULE_DIR + "/docs/sideview.svg")
         fv.change_fill("text_swd_vcc", "#555")
@@ -137,21 +137,21 @@
         # fv.replace_text("text_mux0", "To STM32 VCC")
         # fv.replace_text("text_ext0", "Unused", fill="#999")
         # fv.replace_text("text_ext1", "Unused", fill="#999")
         fv.show()
     
     @staticmethod
     def show_nrf52_glitch_configuration():
-        fv = FaultierVis(MODULE_DIR + "/../docs/topview.svg")
+        fv = FaultierVis(MODULE_DIR + "/docs/topview.svg")
         fv.replace_text("text_crowbar", "To nRF52 VCore")
         fv.replace_text("text_mux0", "To nRF52 VCC")
         fv.replace_text("text_ext0", "Unused", fill="#999")
         fv.replace_text("text_ext1", "Unused", fill="#999")
         fv.show()
-        fv = FaultierVis(MODULE_DIR + "/../docs/sideview.svg")
+        fv = FaultierVis(MODULE_DIR + "/docs/sideview.svg")
         fv.change_fill("text_swd_vcc", "#555")
         for i in range(0, 10):
             fv.change_fill(f"text_io{i}", "#555")
         for i in range(1, 3):
             fv.change_fill(f"text_m{i}_out", "#555")
             fv.change_fill(f"text_m{i}_in0", "#555")
             fv.change_fill(f"text_m{i}_in1", "#555")
```

### Comparing `faultier-0.1.7/faultier/Faultier.py` & `faultier-0.1.8/faultier/Faultier.py`

 * *Files identical despite different names*

### Comparing `faultier-0.1.7/faultier/LivePlot.py` & `faultier-0.1.8/faultier/LivePlot.py`

 * *Files identical despite different names*

### Comparing `faultier-0.1.7/faultier/RandomOrderGenerator.py` & `faultier-0.1.8/faultier/RandomOrderGenerator.py`

 * *Files identical despite different names*

### Comparing `faultier-0.1.7/faultier/docs/sideview.svg` & `faultier-0.1.8/faultier/docs/sideview.svg`

 * *Files identical despite different names*

### Comparing `faultier-0.1.7/faultier/docs/topview.svg` & `faultier-0.1.8/faultier/docs/topview.svg`

 * *Files identical despite different names*

### Comparing `faultier-0.1.7/faultier/example_firmware/nrf52832_xxaa.hex` & `faultier-0.1.8/faultier/example_firmware/nrf52832_xxaa.hex`

 * *Files identical despite different names*

### Comparing `faultier-0.1.7/faultier/example_firmware/s132_nrf52_7.2.0_softdevice.hex` & `faultier-0.1.8/faultier/example_firmware/s132_nrf52_7.2.0_softdevice.hex`

 * *Files identical despite different names*

### Comparing `faultier-0.1.7/faultier/faultier_pb2.py` & `faultier-0.1.8/faultier/faultier_pb2.py`

 * *Files identical despite different names*

### Comparing `faultier-0.1.7/pyproject.toml` & `faultier-0.1.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faultier"
-version = "0.1.7"
+version = "0.1.8"
 #dynamic = ["version"]
 
 authors = [{ name = "Thomas 'stacksmashing' Roth", email = "code@stacksmashing.net"}]
 description = "A library to control the Faultier glitcher."
 #readme = "README.md"
 #license = { file = "LICENSE" }  # Ensure you have a 'LICENSE' file at the root of your project
 #classifiers = [
```


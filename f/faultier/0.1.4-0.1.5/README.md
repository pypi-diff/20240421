# Comparing `tmp/faultier-0.1.4.tar.gz` & `tmp/faultier-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faultier-0.1.4.tar", last modified: Sun Apr 21 14:28:08 2024, max compression
+gzip compressed data, was "faultier-0.1.5.tar", last modified: Sun Apr 21 14:59:26 2024, max compression
```

## Comparing `faultier-0.1.4.tar` & `faultier-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,18 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 14:28:08.396295 faultier-0.1.4/
--rw-r--r--   0 thomas     (501) staff       (20)      522 2024-04-21 14:28:08.396090 faultier-0.1.4/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)       85 2024-03-11 10:46:46.000000 faultier-0.1.4/README.md
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 14:28:08.392582 faultier-0.1.4/docs/
--rw-r--r--   0 thomas     (501) staff       (20)   637437 2024-03-11 10:54:11.000000 faultier-0.1.4/docs/sideview.afdesign
--rw-r--r--   0 thomas     (501) staff       (20)   102775 2024-03-11 10:54:11.000000 faultier-0.1.4/docs/sideview.svg
--rw-r--r--   0 thomas     (501) staff       (20)  1168725 2024-03-11 10:54:11.000000 faultier-0.1.4/docs/topview.afdesign
--rw-r--r--   0 thomas     (501) staff       (20)   350221 2024-03-11 10:54:11.000000 faultier-0.1.4/docs/topview.svg
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 14:28:08.394326 faultier-0.1.4/example_firmware/
--rw-r--r--   0 thomas     (501) staff       (20)    72892 2024-03-11 11:18:12.000000 faultier-0.1.4/example_firmware/nrf52832_xxaa.hex
--rw-r--r--   0 thomas     (501) staff       (20)   429491 2024-03-11 11:18:12.000000 faultier-0.1.4/example_firmware/s132_nrf52_7.2.0_softdevice.hex
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 14:28:08.387424 faultier-0.1.4/faultier/
--rw-r--r--   0 thomas     (501) staff       (20)     6679 2024-03-16 14:19:42.000000 faultier-0.1.4/faultier/FaulterVis.py
--rw-r--r--   0 thomas     (501) staff       (20)     9554 2024-04-18 10:58:34.000000 faultier-0.1.4/faultier/Faultier.py
--rw-r--r--   0 thomas     (501) staff       (20)     2381 2024-03-16 14:19:07.000000 faultier-0.1.4/faultier/LivePlot.py
--rw-r--r--   0 thomas     (501) staff       (20)     1067 2024-03-16 14:18:41.000000 faultier-0.1.4/faultier/RandomOrderGenerator.py
--rw-r--r--   0 thomas     (501) staff       (20)      125 2024-03-16 14:20:53.000000 faultier-0.1.4/faultier/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     6185 2024-03-11 10:46:48.000000 faultier-0.1.4/faultier/faultier_pb2.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 14:28:08.395845 faultier-0.1.4/faultier.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)      522 2024-04-21 14:28:08.000000 faultier-0.1.4/faultier.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      557 2024-04-21 14:28:08.000000 faultier-0.1.4/faultier.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2024-04-21 14:28:08.000000 faultier-0.1.4/faultier.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)       16 2024-04-21 14:28:08.000000 faultier-0.1.4/faultier.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)        9 2024-04-21 14:28:08.000000 faultier-0.1.4/faultier.egg-info/top_level.txt
--rw-r--r--   0 thomas     (501) staff       (20)       38 2024-04-21 14:28:08.396348 faultier-0.1.4/setup.cfg
--rw-r--r--   0 thomas     (501) staff       (20)      752 2024-04-21 14:28:03.000000 faultier-0.1.4/setup.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 14:59:26.426547 faultier-0.1.5/
+-rw-r--r--   0 thomas     (501) staff       (20)      522 2024-04-21 14:59:26.426350 faultier-0.1.5/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)       85 2024-03-11 10:46:46.000000 faultier-0.1.5/README.md
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 14:59:26.425279 faultier-0.1.5/faultier/
+-rw-r--r--   0 thomas     (501) staff       (20)     6746 2024-04-21 14:54:55.000000 faultier-0.1.5/faultier/FaulterVis.py
+-rw-r--r--   0 thomas     (501) staff       (20)     9662 2024-04-21 14:54:24.000000 faultier-0.1.5/faultier/Faultier.py
+-rw-r--r--   0 thomas     (501) staff       (20)     2382 2024-04-21 14:31:26.000000 faultier-0.1.5/faultier/LivePlot.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1067 2024-03-16 14:18:41.000000 faultier-0.1.5/faultier/RandomOrderGenerator.py
+-rw-r--r--   0 thomas     (501) staff       (20)      129 2024-04-21 14:31:08.000000 faultier-0.1.5/faultier/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)     6185 2024-03-11 10:46:48.000000 faultier-0.1.5/faultier/faultier_pb2.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 14:59:26.426139 faultier-0.1.5/faultier.egg-info/
+-rw-r--r--   0 thomas     (501) staff       (20)      522 2024-04-21 14:59:26.000000 faultier-0.1.5/faultier.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)      321 2024-04-21 14:59:26.000000 faultier-0.1.5/faultier.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        1 2024-04-21 14:59:26.000000 faultier-0.1.5/faultier.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       16 2024-04-21 14:59:26.000000 faultier-0.1.5/faultier.egg-info/requires.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        9 2024-04-21 14:59:26.000000 faultier-0.1.5/faultier.egg-info/top_level.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       38 2024-04-21 14:59:26.426585 faultier-0.1.5/setup.cfg
+-rw-r--r--   0 thomas     (501) staff       (20)      757 2024-04-21 14:54:04.000000 faultier-0.1.5/setup.py
```

### Comparing `faultier-0.1.4/PKG-INFO` & `faultier-0.1.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faultier
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library to control the Faultier glitcher.
 Author: Thomas 'stacksmashing' Roth
 Author-email: code@stacksmashing.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `faultier-0.1.4/faultier/FaulterVis.py` & `faultier-0.1.5/faultier/FaulterVis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from IPython.display import HTML
 import xml.etree.ElementTree as ET
 import tempfile
 import os
 import urllib
 
+MODULE_DIR = os.path.dirname(os.path.realpath(__file__))
+
 def update_text_fill(text_element, new_fill_color):
     """
     Updates the "fill" property of an SVG text element's style attribute.
 
     Args:
     text_element (ET.Element): The SVG text element to modify.
     new_fill_color (str): The new color to set for the fill property.
@@ -110,15 +112,15 @@
         return img_tag
 
     def show(self):
         display(HTML(self.create_tag()))
 
     @staticmethod
     def show_stm32_glitch_configuration():
-        fv = FaultierVis(MODULE_DIR + "/docs/topview.svg")
+        fv = FaultierVis(MODULE_DIR + "/../docs/topview.svg")
         fv.replace_text("text_crowbar", "To STM32 VCore")
         fv.replace_text("text_mux0", "To STM32 VCC")
         fv.replace_text("text_ext0", "To STM32 RST")
         fv.replace_text("text_ext1", "Unused", fill="#999")
         fv.show()
         fv = FaultierVis(MODULE_DIR + "/docs/sideview.svg")
         fv.change_fill("text_swd_vcc", "#555")
@@ -135,21 +137,21 @@
         # fv.replace_text("text_mux0", "To STM32 VCC")
         # fv.replace_text("text_ext0", "Unused", fill="#999")
         # fv.replace_text("text_ext1", "Unused", fill="#999")
         fv.show()
     
     @staticmethod
     def show_nrf52_glitch_configuration():
-        fv = FaultierVis(MODULE_DIR + "/docs/topview.svg")
+        fv = FaultierVis(MODULE_DIR + "/../docs/topview.svg")
         fv.replace_text("text_crowbar", "To nRF52 VCore")
         fv.replace_text("text_mux0", "To nRF52 VCC")
         fv.replace_text("text_ext0", "Unused", fill="#999")
         fv.replace_text("text_ext1", "Unused", fill="#999")
         fv.show()
-        fv = FaultierVis(MODULE_DIR + "/docs/sideview.svg")
+        fv = FaultierVis(MODULE_DIR + "/../docs/sideview.svg")
         fv.change_fill("text_swd_vcc", "#555")
         for i in range(0, 10):
             fv.change_fill(f"text_io{i}", "#555")
         for i in range(1, 3):
             fv.change_fill(f"text_m{i}_out", "#555")
             fv.change_fill(f"text_m{i}_in0", "#555")
             fv.change_fill(f"text_m{i}_in1", "#555")
```

### Comparing `faultier-0.1.4/faultier/Faultier.py` & `faultier-0.1.5/faultier/Faultier.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,17 +202,25 @@
             'PATH': "/usr/local/bin:/usr/bin:/opt/homebrew/bin"
         
         }
         print("Erasing...")
         subprocess.run(["openocd", "-s", "/usr/local/share/openocd", "-f", "interface/tamarin.cfg", "-f", "target/nrf52.cfg", "-c", "init; nrf52_recover; exit"], env=env)
         print("Programming softdevice...")
         
-        subprocess.run(["openocd", "-s", "/usr/local/share/openocd", "-f", "interface/tamarin.cfg", "-f", "target/nrf52.cfg", "-c", f"program {os.path.join(MODULE_DIR, "example_firmware", "s132_nrf52_7.2.0_softdevice.hex")}; exit"], env=env)
+        subprocess.run([
+            "openocd", "-s", "/usr/local/share/openocd",
+            "-f", "interface/tamarin.cfg",
+            "-f", "target/nrf52.cfg",
+            "-c", f"program {os.path.join(MODULE_DIR, '..', 'example_firmware', 's132_nrf52_7.2.0_softdevice.hex')}; exit"
+            ], env=env)
         print("Programming firmware...")
-        subprocess.run(["openocd", "-f", "interface/tamarin.cfg", "-f", "target/nrf52.cfg", "-c", f"program {os.path.join(MODULE_DIR, "example_firmware", "nrf52832_xxaa.hex")}; exit"], env=env)
+        subprocess.run([
+            "openocd", "-f", "interface/tamarin.cfg", "-f", "target/nrf52.cfg",
+            "-c", f"program {os.path.join(MODULE_DIR, '..', 'example_firmware', 'nrf52832_xxaa.hex')}; exit"
+        ], env=env)
         print("Locking chip...")
         subprocess.run(["openocd", "-f", "interface/tamarin.cfg", "-f", "target/nrf52.cfg", "-c", "init; reset; halt; flash fillw 0x10001208 0xFFFFFF00 0x01; reset;exit"], env=env)
     
     def stm32_lock(self):
         import time
         print("This action is not reversible. Locking in 10 seconds, press stop to interrupt.")
         time.sleep(10)
```

### Comparing `faultier-0.1.4/faultier/LivePlot.py` & `faultier-0.1.5/faultier/LivePlot.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.fig.update_layout(
             margin=dict(l=20, r=20, t=20, b=20),
         )
         vline = self.fig.add_vline(x=200, line_width=1, line_dash="dash", line_color="red")
         self.vline_x = 200
         display(self.fig)
     
-    def update(self, data)
+    def update(self, data):
         """
         Updates the live figure.
 
         :param data: Takes the data in the format [5, 3, 2, 1, ...]
         """
 
         self.fig.data[0].y = data
```

### Comparing `faultier-0.1.4/faultier/RandomOrderGenerator.py` & `faultier-0.1.5/faultier/RandomOrderGenerator.py`

 * *Files identical despite different names*

### Comparing `faultier-0.1.4/faultier/faultier_pb2.py` & `faultier-0.1.5/faultier/faultier_pb2.py`

 * *Files identical despite different names*

### Comparing `faultier-0.1.4/faultier.egg-info/PKG-INFO` & `faultier-0.1.5/faultier.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faultier
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library to control the Faultier glitcher.
 Author: Thomas 'stacksmashing' Roth
 Author-email: code@stacksmashing.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `faultier-0.1.4/setup.py` & `faultier-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='faultier',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
+    # include_package_data=True,
     package_data={
-        'faultier': ['../docs/*.svg'],
-        'faultier': ['../example_firmware/*.hex'],
+        'faultier': ['docs/*.svg', 'example_firmware/*.hex'],
     },
     install_requires=[
         'pyserial', 'plotly'
     ],
     author='Thomas \'stacksmashing\' Roth',
     author_email='code@stacksmashing.net',
     description='A library to control the Faultier glitcher.',
```


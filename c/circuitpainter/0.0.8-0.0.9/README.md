# Comparing `tmp/circuitpainter-0.0.8.tar.gz` & `tmp/circuitpainter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpainter-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "circuitpainter-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `circuitpainter-0.0.8.tar` & `circuitpainter-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,29 @@
--rw-r--r--   0        0        0      148 2023-09-11 20:32:56.691818 circuitpainter-0.0.8/.gitignore
--rw-r--r--   0        0        0      112 2023-09-11 20:32:56.691818 circuitpainter-0.0.8/.pylintrc
--rw-r--r--   0        0        0      855 2023-12-05 13:30:23.257943 circuitpainter-0.0.8/DEVELOPMENT.md
--rw-r--r--   0        0        0     1078 2023-09-11 20:32:56.691818 circuitpainter-0.0.8/LICENSE
--rw-r--r--   0        0        0      280 2023-09-11 20:32:56.691818 circuitpainter-0.0.8/Makefile
--rw-r--r--   0        0        0    11715 2023-12-05 13:10:39.190337 circuitpainter-0.0.8/README.md
--rw-r--r--   0        0        0   783179 2023-12-05 13:10:39.194335 circuitpainter-0.0.8/doc/asterisk.png
--rw-r--r--   0        0        0    13872 2023-12-05 13:10:39.194335 circuitpainter-0.0.8/doc/example-add-led.png
--rw-r--r--   0        0        0    22617 2023-12-05 13:10:39.194335 circuitpainter-0.0.8/doc/example-connect-led.png
--rw-r--r--   0        0        0   154451 2023-12-05 13:10:39.194335 circuitpainter-0.0.8/doc/example-led-ring.png
--rw-r--r--   0        0        0     8206 2023-12-05 13:10:39.194335 circuitpainter-0.0.8/doc/example-line-widths.png
--rw-r--r--   0        0        0    31444 2023-12-05 13:10:39.194335 circuitpainter-0.0.8/doc/example-push-pop-rect.png
--rw-r--r--   0        0        0   209220 2023-12-05 13:10:39.194335 circuitpainter-0.0.8/doc/example-rest-of-owl.png
--rw-r--r--   0        0        0    17680 2023-12-05 13:10:39.194335 circuitpainter-0.0.8/doc/example-rotate-rect.png
--rw-r--r--   0        0        0     9838 2023-12-05 13:10:39.194335 circuitpainter-0.0.8/doc/example-translate-rect.png
--rw-r--r--   0        0        0   157553 2023-12-05 13:10:39.198333 circuitpainter-0.0.8/doc/example-two-lines.png
--rw-r--r--   0        0        0    91849 2023-12-05 13:10:39.198333 circuitpainter-0.0.8/doc/example_led_ring_drc.png
--rw-r--r--   0        0        0     1462 2023-09-13 19:00:56.432233 circuitpainter-0.0.8/examples/arc_test.py
--rw-r--r--   0        0        0     3743 2023-09-11 20:32:56.691818 circuitpainter-0.0.8/examples/asterix.py
--rw-r--r--   0        0        0     1174 2023-12-05 13:10:39.198333 circuitpainter-0.0.8/examples/hello_painter.py
--rw-r--r--   0        0        0      828 2023-12-05 13:10:39.198333 circuitpainter-0.0.8/examples/learn_to_solder_example.py
--rw-r--r--   0        0        0      508 2023-09-11 20:32:56.691818 circuitpainter-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      137 2024-01-27 10:01:39.926666 circuitpainter-0.0.8/src/circuitpainter/__init__.py
--rw-r--r--   0        0        0    29189 2024-01-03 12:29:18.368728 circuitpainter-0.0.8/src/circuitpainter/circuitpainter.py
--rw-r--r--   0        0        0     2296 2023-09-11 20:32:56.691818 circuitpainter-0.0.8/src/circuitpainter/transform_matrix.py
--rw-r--r--   0        0        0    12139 1970-01-01 00:00:00.000000 circuitpainter-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      148 2023-09-11 20:32:56.691818 circuitpainter-0.0.9/.gitignore
+-rw-r--r--   0        0        0      112 2023-09-11 20:32:56.691818 circuitpainter-0.0.9/.pylintrc
+-rw-r--r--   0        0        0      855 2023-12-05 13:30:23.257943 circuitpainter-0.0.9/DEVELOPMENT.md
+-rw-r--r--   0        0        0     1078 2023-09-11 20:32:56.691818 circuitpainter-0.0.9/LICENSE
+-rw-r--r--   0        0        0      280 2023-09-11 20:32:56.691818 circuitpainter-0.0.9/Makefile
+-rw-r--r--   0        0        0    11717 2024-04-20 09:38:26.456288 circuitpainter-0.0.9/README.md
+-rw-r--r--   0        0        0   783179 2023-12-05 13:10:39.194335 circuitpainter-0.0.9/doc/asterisk.png
+-rw-r--r--   0        0        0    13872 2023-12-05 13:10:39.194335 circuitpainter-0.0.9/doc/example-add-led.png
+-rw-r--r--   0        0        0    22617 2023-12-05 13:10:39.194335 circuitpainter-0.0.9/doc/example-connect-led.png
+-rw-r--r--   0        0        0   154451 2023-12-05 13:10:39.194335 circuitpainter-0.0.9/doc/example-led-ring.png
+-rw-r--r--   0        0        0     8206 2023-12-05 13:10:39.194335 circuitpainter-0.0.9/doc/example-line-widths.png
+-rw-r--r--   0        0        0    31444 2023-12-05 13:10:39.194335 circuitpainter-0.0.9/doc/example-push-pop-rect.png
+-rw-r--r--   0        0        0   209220 2023-12-05 13:10:39.194335 circuitpainter-0.0.9/doc/example-rest-of-owl.png
+-rw-r--r--   0        0        0    17680 2023-12-05 13:10:39.194335 circuitpainter-0.0.9/doc/example-rotate-rect.png
+-rw-r--r--   0        0        0     9838 2023-12-05 13:10:39.194335 circuitpainter-0.0.9/doc/example-translate-rect.png
+-rw-r--r--   0        0        0   157553 2023-12-05 13:10:39.198333 circuitpainter-0.0.9/doc/example-two-lines.png
+-rw-r--r--   0        0        0    91849 2023-12-05 13:10:39.198333 circuitpainter-0.0.9/doc/example_led_ring_drc.png
+-rw-r--r--   0        0        0  2903615 2024-04-20 09:38:26.460286 circuitpainter-0.0.9/doc/lotus_leds.png
+-rw-r--r--   0        0        0     1462 2023-09-13 19:00:56.432233 circuitpainter-0.0.9/examples/arc_test.py
+-rw-r--r--   0        0        0     3743 2023-09-11 20:32:56.691818 circuitpainter-0.0.9/examples/asterix.py
+-rw-r--r--   0        0        0     1174 2023-12-05 13:10:39.198333 circuitpainter-0.0.9/examples/hello_painter.py
+-rw-r--r--   0        0        0      828 2023-12-05 13:10:39.198333 circuitpainter-0.0.9/examples/learn_to_solder_example.py
+-rw-r--r--   0        0        0     7046 2024-04-21 15:02:39.996598 circuitpainter-0.0.9/examples/lotus_leds.py
+-rw-r--r--   0        0        0     1855 2024-04-21 14:29:58.228923 circuitpainter-0.0.9/examples/perfboard.py
+-rw-r--r--   0        0        0      508 2023-09-11 20:32:56.691818 circuitpainter-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      137 2024-04-21 15:03:08.382901 circuitpainter-0.0.9/src/circuitpainter/__init__.py
+-rw-r--r--   0        0        0    31119 2024-04-21 14:51:45.199946 circuitpainter-0.0.9/src/circuitpainter/circuitpainter.py
+-rw-r--r--   0        0        0     2296 2023-09-11 20:32:56.691818 circuitpainter-0.0.9/src/circuitpainter/transform_matrix.py
+-rw-r--r--   0        0        0    12141 1970-01-01 00:00:00.000000 circuitpainter-0.0.9/PKG-INFO
```

### Comparing `circuitpainter-0.0.8/DEVELOPMENT.md` & `circuitpainter-0.0.9/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/LICENSE` & `circuitpainter-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/README.md` & `circuitpainter-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Circuit Painter
 
-![](doc/asterisk.png)
+![](doc/lotus_leds.png)
 
 Circuit painter is a creative coding tool for making functional printed
 circuit boards.
 
 Inspired by the simplifed drawing language of Processing, this tool provides
 an environment for designing PCBs using basic geometric shapes such as lines,
 arcs, and polygons. The tool maintains a drawing 'context' that applies a
```

### Comparing `circuitpainter-0.0.8/doc/asterisk.png` & `circuitpainter-0.0.9/doc/asterisk.png`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/doc/example-add-led.png` & `circuitpainter-0.0.9/doc/example-add-led.png`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/doc/example-connect-led.png` & `circuitpainter-0.0.9/doc/example-connect-led.png`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/doc/example-led-ring.png` & `circuitpainter-0.0.9/doc/example-led-ring.png`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/doc/example-line-widths.png` & `circuitpainter-0.0.9/doc/example-line-widths.png`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/doc/example-push-pop-rect.png` & `circuitpainter-0.0.9/doc/example-push-pop-rect.png`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/doc/example-rest-of-owl.png` & `circuitpainter-0.0.9/doc/example-rest-of-owl.png`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/doc/example-rotate-rect.png` & `circuitpainter-0.0.9/doc/example-rotate-rect.png`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/doc/example-translate-rect.png` & `circuitpainter-0.0.9/doc/example-translate-rect.png`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/doc/example-two-lines.png` & `circuitpainter-0.0.9/doc/example-two-lines.png`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/doc/example_led_ring_drc.png` & `circuitpainter-0.0.9/doc/example_led_ring_drc.png`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/examples/arc_test.py` & `circuitpainter-0.0.9/examples/arc_test.py`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/examples/asterix.py` & `circuitpainter-0.0.9/examples/asterix.py`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/examples/hello_painter.py` & `circuitpainter-0.0.9/examples/hello_painter.py`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/examples/learn_to_solder_example.py` & `circuitpainter-0.0.9/examples/learn_to_solder_example.py`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/src/circuitpainter/circuitpainter.py` & `circuitpainter-0.0.9/src/circuitpainter/circuitpainter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,55 @@
 #!/usr/bin/env python
 
 import math
 import subprocess
 import glob
 import os
+import platform
+from pathlib import Path
 from tempfile import TemporaryDirectory
+import zipfile
 import pcbnew
 from circuitpainter.transform_matrix import TransformMatrix
 
 # References:
 # /usr/lib/python3/dist-packages/pcbnew.py
 # https://github.com/KiCad/kicad-source-mirror/tree/master/pcbnew
 # https://github.com/cooked/kimotor/blob/master/kimotor_action.py
 
 
+def _guess_footprint_library_path():
+    """Attempt to find the KiCad footprint library"""
+
+    system = platform.system()
+
+    if system == "Linux":
+        return "/usr/share/kicad/footprints"
+    elif system == "Windows":
+        return "C:\\Program Files\\KiCad\\7.0\\share\\kicad\\footprints"
+    else:
+        return
+
+def _make_zip(output_name, filenames):
+    """Create a zip file
+
+    Create a zip file containing the given files. The files will be written to
+    the root directory of the zip, with any relative paths stripped.
+
+    output_name: Name of the output zip file (will be overwritten if exists)
+    filenames: Full paths of files to write to the zip file
+    """
+    with zipfile.ZipFile(output_name,'w') as of:
+        for filename in filenames:
+            path = Path(filename)
+            of.write(filename,
+                     arcname=path.name,
+                     compress_type=zipfile.ZIP_DEFLATED,
+                     compresslevel=5)
+
 class CircuitPainter:
     # Board layers, from pcbnew
     layers = {
         "F_Cu": pcbnew.F_Cu,
         "In1_Cu": pcbnew.In1_Cu,
         "In2_Cu": pcbnew.In2_Cu,
         "In3_Cu": pcbnew.In3_Cu,
@@ -78,22 +110,25 @@
         "User_9": pcbnew.User_9,
         "Rescue": pcbnew.Rescue,
     }
 
     def __init__(
             self,
             filename=None,
-            library_path="/usr/share/kicad/footprints"):
+            library_path=None):
         """ Create a Circuit Builder context
 
         pcb: (optional) If specified, work with the given PCB. If not
              specified, start with a blank PCB
         library_path: (optional) Path to the footprint libraries
         """
 
+        if library_path==None:
+            library_path = _guess_footprint_library_path()
+
         self.tempdir = TemporaryDirectory()
 
         if filename is not None:
             self.filename = filename
             self.pcb = pcbnew.LoadBoard(filename)
         else:
             # Note: Use NewBoard here because CreateEmptyBoard is buggy, see:
@@ -726,103 +761,129 @@
         self._auto_set_origin()
 
         # Map pcbnew layer names to a format recognized by kicad-cli
         # Note that if the layer list is empty, kicad-cli will choose some
         # default set automatically
         layers_csv = ','.join(layers).replace('_', '.')
 
-        with TemporaryDirectory() as tmpdir_kicad, TemporaryDirectory() as tmpdir_gerber:
+        file_stem = Path(filename).name
+
+        with TemporaryDirectory() as tmpdir_kicad:
+            gerberdir = f"{tmpdir_kicad}/gerber"
+
             # Write the kicad pcb out to a temporary location
-            self.save(f"{tmpdir_kicad}/{filename}")
+            self.save(f"{tmpdir_kicad}/{file_stem}")
+
+            os.mkdir(gerberdir)
 
             # Generate gerbers to yet another location
             # TODO: Remove empty layers?
             subprocess.check_call(["kicad-cli",
                                    "pcb",
                                    "export",
                                    "gerbers",
                                    "--use-drill-file-origin",
                                    "-l",
                                    layers_csv,
-                                   f"{tmpdir_kicad}/{filename}.kicad_pcb"],
-                                  cwd=tmpdir_gerber)
+                                   f"{tmpdir_kicad}/{file_stem}.kicad_pcb"],
+                                  cwd=gerberdir)
             subprocess.check_call(["kicad-cli",
                                    "pcb",
                                    "export",
                                    "drill",
                                    "--drill-origin",
                                    "plot",
-                                   f"{tmpdir_kicad}/{filename}.kicad_pcb"],
-                                  cwd=tmpdir_gerber)
+                                   f"{tmpdir_kicad}/{file_stem}.kicad_pcb"],
+                                  cwd=gerberdir)
 
             # Don't copy the gbrjob file
-            if os.path.exists(f"{tmpdir_gerber}/{filename}-job.gbrjob"):
-                os.remove(f"{tmpdir_gerber}/{filename}-job.gbrjob")
+            if os.path.exists(f"{gerberdir}/{file_stem}-job.gbrjob"):
+                os.remove(f"{gerberdir}/{file_stem}-job.gbrjob")
 
             # Zip up the gerbers
-            files = glob.glob(f"{tmpdir_gerber}/*")
-
-            subprocess.check_call(
-                ["zip",
-                 "-j",
-                 f"{filename}_gerbers.zip", *files],
-                cwd=tmpdir_gerber)
-
-            subprocess.check_call(
-                ["cp",
-                 f"{tmpdir_gerber}/{filename}_gerbers.zip",
-                 "./"])
+            files = glob.glob(f"{gerberdir}/*")
+            _make_zip(f"{filename}.zip", files)
 
     def export_svg(self, filename):
         """ Export the design to an SVG
 
         This saves the file to a temporary loation, uses the kicad command
         line interface to render an svg, then copies it to the specified
         location
 
         filename: Name of output file
         """
         self._fill_zones()
         self._auto_set_origin()
 
+        file_stem = Path(filename).name
+
         with TemporaryDirectory() as tmpdir_kicad:
             # Write the kicad pcb out to a temporary location
-            self.save(f"{tmpdir_kicad}/{filename}")
+            self.save(f"{tmpdir_kicad}/{file_stem}")
 
             subprocess.check_call(["kicad-cli",
                                    "pcb",
                                    "export",
                                    "svg",
                                    "--page-size-mode",
                                    "2",
                                    "--exclude-drawing-sheet",
                                    "-l",
                                    ','.join([i.replace('_',
                                                        '.') for i in self.layers.keys()]),
-                                   f"{tmpdir_kicad}/{filename}.kicad_pcb"])
+                                   f"{tmpdir_kicad}/{file_stem}.kicad_pcb"])
+
+    def export_step(self, filename):
+        """ Export the design to an STEP file
+
+        This saves the file to a temporary loation, uses the kicad command
+        line interface to render a step file, then copies it to the specified
+        location
+
+        filename: Name of output file
+        """
+        self._fill_zones()
+        self._auto_set_origin()
+
+        file_stem = Path(filename).name
+
+        with TemporaryDirectory() as tmpdir_kicad:
+            # Write the kicad pcb out to a temporary location
+            self.save(f"{tmpdir_kicad}/{file_stem}")
+
+            subprocess.check_call(["kicad-cli",
+                                   "pcb",
+                                   "export",
+                                   "step",
+                                   "--drill-origin",
+                                   "--output", f"{file_stem}.step",
+                                   f"{tmpdir_kicad}/{file_stem}.kicad_pcb"])
 
     def export_pos(self, filename):
         """ Export a pick-and-place file
 
         This saves the file to a temporary loation, uses the kicad command
         line interface to render a pnp file, then copies it to the specified
         location
 
         filename: Name of output file
         """
         self._fill_zones()
         self._auto_set_origin()
 
+        file_stem = Path(filename).name
+
         with TemporaryDirectory() as tmpdir_kicad:
             # Write the kicad pcb out to a temporary location
-            self.save(f"{tmpdir_kicad}/{filename}")
+            self.save(f"{tmpdir_kicad}/{file_stem}")
 
             subprocess.check_call(["kicad-cli",
                                    "pcb",
                                    "export",
                                    "pos",
                                    "--format","csv",
                                    "--units","mm",
                                    "--bottom-negate-x",
                                    "--use-drill-file-origin",
                                    "--output", f"{filename}_pos.csv",
-                                   f"{tmpdir_kicad}/{filename}.kicad_pcb"])
+                                   f"{tmpdir_kicad}/{file_stem}.kicad_pcb"])
```

### Comparing `circuitpainter-0.0.8/src/circuitpainter/transform_matrix.py` & `circuitpainter-0.0.9/src/circuitpainter/transform_matrix.py`

 * *Files identical despite different names*

### Comparing `circuitpainter-0.0.8/PKG-INFO` & `circuitpainter-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: circuitpainter
-Version: 0.0.8
+Version: 0.0.9
 Summary: Sketching interface for macking function printed circuit boards
 Keywords: kicad,pcb,printed ciruit board,circuit design,skectching
 Author-email: Matthew Mets <matt@blinkinlabs.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy
 Project-URL: Home, https://github.com/blinkinlabs/pcb_painter
 
 # Circuit Painter
 
-![](doc/asterisk.png)
+![](doc/lotus_leds.png)
 
 Circuit painter is a creative coding tool for making functional printed
 circuit boards.
 
 Inspired by the simplifed drawing language of Processing, this tool provides
 an environment for designing PCBs using basic geometric shapes such as lines,
 arcs, and polygons. The tool maintains a drawing 'context' that applies a
```


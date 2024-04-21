# Comparing `tmp/geodynamic-0.0.7.tar.gz` & `tmp/geodynamic-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodynamic-0.0.7.tar", last modified: Thu Apr 18 15:04:55 2024, max compression
+gzip compressed data, was "geodynamic-0.0.8.tar", last modified: Sun Apr 21 11:52:53 2024, max compression
```

## Comparing `geodynamic-0.0.7.tar` & `geodynamic-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-18 15:04:55.839944 geodynamic-0.0.7/
--rw-r--r--   0 mac        (501) staff       (20)       18 2024-04-05 12:40:59.000000 geodynamic-0.0.7/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)     1099 2024-04-18 15:04:55.839872 geodynamic-0.0.7/PKG-INFO
--rw-------   0 mac        (501) staff       (20)      428 2024-04-18 12:05:16.000000 geodynamic-0.0.7/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-18 15:04:55.834292 geodynamic-0.0.7/geodynamic/
--rw-------   0 mac        (501) staff       (20)        0 2024-04-05 11:31:09.000000 geodynamic-0.0.7/geodynamic/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-18 15:04:55.837290 geodynamic-0.0.7/geodynamic/geo/
--rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:09.000000 geodynamic-0.0.7/geodynamic/geo/__init__.py
--rw-------   0 mac        (501) staff       (20)    10547 2024-04-13 15:38:56.000000 geodynamic-0.0.7/geodynamic/geo/construction.py
--rw-------   0 mac        (501) staff       (20)    24312 2024-04-15 15:34:01.000000 geodynamic-0.0.7/geodynamic/geo/lib_commands.py
--rw-------   0 mac        (501) staff       (20)    12974 2024-04-13 14:52:57.000000 geodynamic-0.0.7/geodynamic/geo/lib_elements.py
--rw-------   0 mac        (501) staff       (20)     1752 2024-01-22 09:44:40.000000 geodynamic-0.0.7/geodynamic/geo/lib_vars.py
--rw-------   0 mac        (501) staff       (20)    31503 2024-04-18 14:56:31.000000 geodynamic-0.0.7/geodynamic/manim_dynamic.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-18 15:04:55.839166 geodynamic-0.0.7/geodynamic/parsers/
--rw-rw-r--   0 mac        (501) staff       (20)      411 2024-04-08 16:07:59.000000 geodynamic-0.0.7/geodynamic/parsers/__init__.py
--rw-------   0 mac        (501) staff       (20)    13622 2024-04-05 11:51:36.000000 geodynamic-0.0.7/geodynamic/parsers/ggb_generator.py
--rw-------   0 mac        (501) staff       (20)     7380 2024-04-18 13:47:34.000000 geodynamic-0.0.7/geodynamic/parsers/ggb_parser.py
--rw-------   0 mac        (501) staff       (20)     3344 2024-04-05 11:52:04.000000 geodynamic-0.0.7/geodynamic/parsers/short_parser.py
--rw-rw-r--   0 mac        (501) staff       (20)     6514 2024-04-18 14:55:48.000000 geodynamic-0.0.7/geodynamic/parsers/svg_parser.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-18 15:04:55.839601 geodynamic-0.0.7/geodynamic.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     1099 2024-04-18 15:04:55.000000 geodynamic-0.0.7/geodynamic.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      575 2024-04-18 15:04:55.000000 geodynamic-0.0.7/geodynamic.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-18 15:04:55.000000 geodynamic-0.0.7/geodynamic.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       60 2024-04-18 15:04:55.000000 geodynamic-0.0.7/geodynamic.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       11 2024-04-18 15:04:55.000000 geodynamic-0.0.7/geodynamic.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-18 15:04:55.840234 geodynamic-0.0.7/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      951 2024-04-18 12:05:38.000000 geodynamic-0.0.7/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-21 11:52:53.938582 geodynamic-0.0.8/
+-rw-r--r--   0 mac        (501) staff       (20)       18 2024-04-05 12:40:59.000000 geodynamic-0.0.8/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)     1099 2024-04-21 11:52:53.938467 geodynamic-0.0.8/PKG-INFO
+-rw-------   0 mac        (501) staff       (20)      428 2024-04-18 12:05:16.000000 geodynamic-0.0.8/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-21 11:52:53.929474 geodynamic-0.0.8/geodynamic/
+-rw-------   0 mac        (501) staff       (20)        0 2024-04-05 11:31:09.000000 geodynamic-0.0.8/geodynamic/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-21 11:52:53.933766 geodynamic-0.0.8/geodynamic/geo/
+-rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:09.000000 geodynamic-0.0.8/geodynamic/geo/__init__.py
+-rw-------   0 mac        (501) staff       (20)    10547 2024-04-13 15:38:56.000000 geodynamic-0.0.8/geodynamic/geo/construction.py
+-rw-------   0 mac        (501) staff       (20)    24312 2024-04-15 15:34:01.000000 geodynamic-0.0.8/geodynamic/geo/lib_commands.py
+-rw-------   0 mac        (501) staff       (20)    12974 2024-04-13 14:52:57.000000 geodynamic-0.0.8/geodynamic/geo/lib_elements.py
+-rw-------   0 mac        (501) staff       (20)     1752 2024-01-22 09:44:40.000000 geodynamic-0.0.8/geodynamic/geo/lib_vars.py
+-rw-------   0 mac        (501) staff       (20)    32122 2024-04-21 11:50:53.000000 geodynamic-0.0.8/geodynamic/manim_dynamic.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-21 11:52:53.936452 geodynamic-0.0.8/geodynamic/parsers/
+-rw-rw-r--   0 mac        (501) staff       (20)        0 2024-04-20 15:28:40.000000 geodynamic-0.0.8/geodynamic/parsers/__init__.py
+-rw-------   0 mac        (501) staff       (20)    13622 2024-04-05 11:51:36.000000 geodynamic-0.0.8/geodynamic/parsers/ggb_generator.py
+-rw-------   0 mac        (501) staff       (20)     7626 2024-04-21 11:50:59.000000 geodynamic-0.0.8/geodynamic/parsers/ggb_parser.py
+-rw-------   0 mac        (501) staff       (20)     3344 2024-04-05 11:52:04.000000 geodynamic-0.0.8/geodynamic/parsers/short_parser.py
+-rw-rw-r--   0 mac        (501) staff       (20)     3971 2024-04-21 10:17:23.000000 geodynamic-0.0.8/geodynamic/parsers/svg_parser.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-21 11:52:53.937650 geodynamic-0.0.8/geodynamic.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     1099 2024-04-21 11:52:53.000000 geodynamic-0.0.8/geodynamic.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      575 2024-04-21 11:52:53.000000 geodynamic-0.0.8/geodynamic.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-21 11:52:53.000000 geodynamic-0.0.8/geodynamic.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       60 2024-04-21 11:52:53.000000 geodynamic-0.0.8/geodynamic.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       11 2024-04-21 11:52:53.000000 geodynamic-0.0.8/geodynamic.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-21 11:52:53.939764 geodynamic-0.0.8/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      951 2024-04-21 11:52:39.000000 geodynamic-0.0.8/setup.py
```

### Comparing `geodynamic-0.0.7/PKG-INFO` & `geodynamic-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodynamic
-Version: 0.0.7
+Version: 0.0.8
 Summary: Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG
 Home-page: https://gitlab.mathem.ru/
 Author: ivaleo
 Author-email: ivaleotion@gmail.com
 Keywords: geometry dynamic geogebra manim animation svg python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geodynamic-0.0.7/geodynamic/geo/construction.py` & `geodynamic-0.0.8/geodynamic/geo/construction.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.7/geodynamic/geo/lib_commands.py` & `geodynamic-0.0.8/geodynamic/geo/lib_commands.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.7/geodynamic/geo/lib_elements.py` & `geodynamic-0.0.8/geodynamic/geo/lib_elements.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.7/geodynamic/geo/lib_vars.py` & `geodynamic-0.0.8/geodynamic/geo/lib_vars.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.7/geodynamic/manim_dynamic.py` & `geodynamic-0.0.8/geodynamic/manim_dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import re
 import json
 import numpy as np
+import tempfile
+from contextlib import contextmanager
 
 from .geo import construction as geo
 from manim import *
 from .parsers.svg_parser import *
 from .parsers import short_parser, ggb_parser
 
 import xml.etree.ElementTree as ET
@@ -287,15 +289,15 @@
         self.geo.rebuild(debug = debug)
         
         style = GeoStyle(style_json_file = style_json_file, px_size = px_size)
         
         bounds = self.getAllGeometryBounds(self.geo.style['view']['scale'])
         padding = style.technic['crop_padding'] if 'crop_padding' in style.technic else 10
         
-        print('BOUNDS:', bounds)
+        #print('BOUNDS:', bounds)
         
         self.geo.style['view']['width'] = bounds[2] - bounds[0] + 2 * padding
         self.geo.style['view']['height'] = bounds[3] - bounds[1] + 2 * padding
         self.geo.style['view']['xZero'] = -bounds[0] + padding
         self.geo.style['view']['yZero'] = bounds[3] + padding
         
         if px_size is not None:
@@ -303,22 +305,29 @@
         else:
             style.view = self.geo.style['view']
 
         view = style.view
         scale = view['scale']
         scale_export = style.technic['scale_export'] if 'scale_export' in style.technic else 1
         q = 50 * scale_export / scale
-        for key in ['dot_size', 'line_width', 'ang_width', 'ang_rdefault', 'ang_right', 'ang_rshift', 'strich_rshift', 'strich_len']:
+        for key in ['dot_size', 'line_width', 'ang_width', 'ang_rdefault', 'ang_right', 'ang_rshift', 'strich_width', 'strich_rshift', 'strich_len']:
             setattr(style, key, getattr(style, key) * q)
-
-        self.camera.frame.set(width = view['width'] / scale)
-        dx = self.camera.frame.width / 2 - view['xZero'] / scale
-        dy = view['height'] / (2 * scale) - view['yZero'] / scale      
-        self.camera.frame.shift(dx * RIGHT + dy * DOWN)
-
+            
+        ratio = 1920/1080
+        if view['width'] / view['height'] >= ratio:
+            self.camera.frame.set(width = view['width'] / scale)
+            dx = self.camera.frame.width / 2 - view['xZero'] / scale
+            dy = view['height'] / (2 * scale) - view['yZero'] / scale      
+            self.camera.frame.shift(dx * RIGHT + dy * DOWN)
+        else:
+            self.camera.frame.set(width = ratio * view['height'] / scale)
+            dx = view['height'] / (2 * scale) - view['xZero'] / scale
+            dy = self.camera.frame.height / 2 - view['yZero'] / scale      
+            self.camera.frame.shift(dx * RIGHT + dy * DOWN)
+    
         self.setStyle(style)
         self.addAllGeometry(show = True)
 
     def updateGeoVar(self, x, var_name):
         self.geo.update(var_name, float(x.get_value()))
         updates = self.geo.rebuild()
         #print(updates)
@@ -346,21 +355,23 @@
 
     def playBackStyle(self, names, mode = None, **kwargs):
         self.play(*BackStyleObjs(self, names, mode, **kwargs))
 
     #----------------------------------
 
     def exportSVG(self, filepath):
-        #config.frame_height = self.camera.frame.get_height()
-        #config.frame_width = self.camera.frame.get_width()
-        #scale = 2 * self.style['view']['scale']
-        #config.frame_width, config.frame_height = self.style['view']['width'] / scale, self.style['view']['height'] / scale
-        #config.__setattr__('frame_center', self.camera.frame.get_center())
-        config.__setattr__('ggb_view', self.style.view)
-        VGroup(*self.mobjects).to_svg(filepath, self.style.technic)
+        if filepath is None:
+            filepath = tempfile.mktemp(suffix=".svg")
+        filepath = Path(filepath).absolute()
+        
+        with _get_cairo_context(filepath, self.style) as ctx:
+            for mobj in extract_mobject_family_members(self.mobjects, True, True):
+                _create_svg_from_vmobject_internal(mobj, ctx, style = self.style)
+                
+        #VGroup(*self.mobjects).to_svg(filepath, self.style.technic)
     
     def addGrid(self, x_range=(-10, 10, 1), y_range=(-10, 10, 1)):
         grid = NumberPlane(
             x_range = x_range,
             y_range = y_range,
             x_length = x_range[1] - x_range[0],
             y_length = y_range[1] - y_range[0],
@@ -617,14 +628,16 @@
     return min(max_r, r)
 
 def CreateMObject(elem, z_auto = False, style = None, debug = False):
     try:
         if style is None: style = GeoDynamic.style_default
 
         dash = getParamFromDict(elem.style, 'stroke_dash', None)
+        cap = getParamFromDict(elem.style, 'stroke_cap', getParamFromDict(style.technic, 'line_caps', 'auto'))
+        #print('CAP', cap)
 
         col_s = getParamFromDict(elem.style, 'stroke', style.strong)
         col_f = getParamFromDict(elem.style, 'fill', style.background if type(elem.data) != geo.Point else style.strong)
         op_s = getParamFromDict(elem.style, 'stroke_opacity', 1)
         op_f = getParamFromDict(elem.style, 'fill_opacity', 1)
         lw = getParamFromDict(elem.style, 'stroke_width', style.line_width, type(elem.data) == geo.Arc)
         col_label = getParamFromDict(elem.style, 'label_color', style.strong)
@@ -695,15 +708,15 @@
             p1, p2 = elem.data.end_points
             m = (p1 + p2) / 2
             arr = []
 
             if dash: arr.append(DashedLine([p1[0], p1[1], 0], [p2[0], p2[1], 0], 
                             color = col_s, stroke_opacity = op_s, stroke_width = lw, dash_length = 0.17, dashed_ratio = dash).set_z_index(zz))
             else: arr.append(Line([p1[0], p1[1], 0], [p2[0], p2[1], 0], 
-                            color = col_s, stroke_opacity = op_s, stroke_width = lw).set_z_index(zz))
+                            color = col_s, stroke_opacity = op_s, stroke_width = lw).set_z_index(zz).set_stroke_cap(cap))
 
             if 'lines' in elem.style:
                 num = elem.style['lines']
                 dn = elem.data.n * style.strich_len / 2
                 v = (p2 - p1) / np.linalg.norm(p2 - p1)
                 line = Line([m[0] + dn[0], m[1] + dn[1], 0], [m[0] - dn[0], m[1] - dn[1], 0],
                             color = col_s, stroke_width = style.strich_width, stroke_opacity = op_s).set_z_index(zz)
@@ -761,13 +774,14 @@
                 label = elem.style['label'] if hasParam(elem.style, 'label') else '$' + elem.name + '$'
                 tex = Tex(correctedLabel(label), color = col_label).set_z_index(zz_label).scale(1.12).move_to(arr[0])
                 arr.append(tex)
                 if hasParam(elem.style, 'offset'):
                     tex.shift([elem.style['offset'][0], elem.style['offset'][1], 0])
 
             return VGroup(*arr, name = elem.name)
-    except:
+    except Exception as e:
         print(f'MObject for element "{elem.name}" is NONE')
+        print(e)
         return None
     
     return None
```

### Comparing `geodynamic-0.0.7/geodynamic/parsers/ggb_generator.py` & `geodynamic-0.0.8/geodynamic/parsers/ggb_generator.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.7/geodynamic/parsers/ggb_parser.py` & `geodynamic-0.0.8/geodynamic/parsers/ggb_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 def parse_constr(constr: Construction, constr_xelem: XElement, debug = False):
     xelems_left_to_pass = 0
     fixed_element = False
 
     style = {}
     
-    unknown_objs = {}
+    polygon_border = {}
     
     for xelem in constr_xelem:            
         if xelem.tag == "element":
             name = xelem.attrib['label']
             #print(f'ELEMENT {name}')
             if xelem.attrib["type"] != "numeric":
                 style[name] = {}
@@ -111,14 +111,17 @@
                     fixed_element = True
                 else:
                     xelems_left_to_pass = 1
                 continue
             if comm_name == "PointIn":
                 xelems_left_to_pass = 1
                 continue
+            if comm_name == "Polygon":
+                for segm in outputs[1:]:
+                    polygon_border[segm] = True
 
             constr.add(Command(comm_name, inputs, outputs))
             xelems_left_to_pass = len(output_xelem.attrib)
             continue
         
         # Here xelem has to be a commandless point or numeric (Var)
         
@@ -138,14 +141,19 @@
                 constr.add(Var(xelem.attrib["label"], AngleSize(float(value_xelem.attrib["val"]))))
                 continue
         
         #raise ElementTree.ParseError(f"Unexpected XElement met:\n\t<{xelem.tag}>, {xelem.attrib}")
         print(f"Unexpected XElement met:\n\t<{xelem.tag}>, {xelem.attrib}")
 
     constr.rebuild(debug = debug)
+    
+    #print(polygon_border)
+
+    for segm in polygon_border:
+        constr.element(segm).style['z_index'] = 10
 
     #styling elements
     for name in style:
         for key in style[name]:
             #print(f'STYLE >> {name} >> {key} = {style[name][key]}')
             if key == 'show_element':
                 constr.element(name).visible = style[name][key]
```

### Comparing `geodynamic-0.0.7/geodynamic/parsers/short_parser.py` & `geodynamic-0.0.8/geodynamic/parsers/short_parser.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.7/geodynamic.egg-info/PKG-INFO` & `geodynamic-0.0.8/geodynamic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodynamic
-Version: 0.0.7
+Version: 0.0.8
 Summary: Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG
 Home-page: https://gitlab.mathem.ru/
 Author: ivaleo
 Author-email: ivaleotion@gmail.com
 Keywords: geometry dynamic geogebra manim animation svg python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geodynamic-0.0.7/geodynamic.egg-info/SOURCES.txt` & `geodynamic-0.0.8/geodynamic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.7/setup.py` & `geodynamic-0.0.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='geodynamic',
-  version='0.0.7',
+  version='0.0.8',
   author='ivaleo',
   author_email='ivaleotion@gmail.com',
   description='Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://gitlab.mathem.ru/',
   packages=find_packages(),
```


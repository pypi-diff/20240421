# Comparing `tmp/python_signal_edges-1.0.4-py3-none-any.whl.zip` & `tmp/python_signal_edges-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 46093 bytes, number of entries: 29
+Zip file size: 46095 bytes, number of entries: 29
 -rw-r--r--  2.0 unx      429 b- defN 80-Jan-01 00:00 signal_edges/__init__.py
 -rw-r--r--  2.0 unx     1008 b- defN 80-Jan-01 00:00 signal_edges/definitions.py
 -rw-r--r--  2.0 unx      569 b- defN 80-Jan-01 00:00 signal_edges/exceptions.py
 -rw-r--r--  2.0 unx      373 b- defN 80-Jan-01 00:00 signal_edges/plotter/__init__.py
 -rw-r--r--  2.0 unx     3569 b- defN 80-Jan-01 00:00 signal_edges/plotter/definitions.py
 -rw-r--r--  2.0 unx    19958 b- defN 80-Jan-01 00:00 signal_edges/plotter/plotter.py
 -rw-r--r--  2.0 unx      642 b- defN 80-Jan-01 00:00 signal_edges/plotter/style/style.mplstyle
@@ -20,12 +20,12 @@
 -rw-r--r--  2.0 unx      314 b- defN 80-Jan-01 00:00 signal_edges/signal/sample/__init__.py
 -rw-r--r--  2.0 unx    19205 b- defN 80-Jan-01 00:00 signal_edges/signal/sample/sample.py
 -rw-r--r--  2.0 unx    10326 b- defN 80-Jan-01 00:00 signal_edges/signal/signal.py
 -rw-r--r--  2.0 unx      372 b- defN 80-Jan-01 00:00 signal_edges/signal/state_levels/__init__.py
 -rw-r--r--  2.0 unx     1421 b- defN 80-Jan-01 00:00 signal_edges/signal/state_levels/definitions.py
 -rw-r--r--  2.0 unx    14070 b- defN 80-Jan-01 00:00 signal_edges/signal/state_levels/state_levels.py
 -rw-r--r--  2.0 unx     4334 b- defN 80-Jan-01 00:00 signal_edges/signal/voltage_signal.py
--rw-r--r--  2.0 unx     1084 b- defN 80-Jan-01 00:00 python_signal_edges-1.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     3100 b- defN 80-Jan-01 00:00 python_signal_edges-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 python_signal_edges-1.0.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2677 b- defN 16-Jan-01 00:00 python_signal_edges-1.0.4.dist-info/RECORD
-29 files, 158168 bytes uncompressed, 41697 bytes compressed:  73.6%
+-rw-r--r--  2.0 unx     1084 b- defN 80-Jan-01 00:00 python_signal_edges-1.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3116 b- defN 80-Jan-01 00:00 python_signal_edges-1.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 python_signal_edges-1.0.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2677 b- defN 16-Jan-01 00:00 python_signal_edges-1.0.5.dist-info/RECORD
+29 files, 158184 bytes uncompressed, 41699 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -69,20 +69,20 @@
 
 Filename: signal_edges/signal/state_levels/state_levels.py
 Comment: 
 
 Filename: signal_edges/signal/voltage_signal.py
 Comment: 
 
-Filename: python_signal_edges-1.0.4.dist-info/LICENSE
+Filename: python_signal_edges-1.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: python_signal_edges-1.0.4.dist-info/METADATA
+Filename: python_signal_edges-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: python_signal_edges-1.0.4.dist-info/WHEEL
+Filename: python_signal_edges-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: python_signal_edges-1.0.4.dist-info/RECORD
+Filename: python_signal_edges-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `python_signal_edges-1.0.4.dist-info/LICENSE` & `python_signal_edges-1.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `python_signal_edges-1.0.4.dist-info/METADATA` & `python_signal_edges-1.0.5.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: python-signal-edges
-Version: 1.0.4
+Version: 1.0.5
 Summary: Extract state levels and edges from signals, among others
 Home-page: https://github.com/dmg0345/python-signal-edges
 License: MIT
 Keywords: python,signal,edges,automation,hardware,pwm,acquisition
 Author: Diego Martinez
 Author-email: dmg0345@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.8.2)
 Requires-Dist: numpy (>=1.26.0)
 Requires-Dist: scipy (>=1.12.0)
-Project-URL: Documentation, https://python-signal-edges.netlify.app/
+Project-URL: Documentation, https://dmg0345-python-signal-edges.netlify.app/
 Project-URL: Repository, https://github.com/dmg0345/python-signal-edges
 Description-Content-Type: text/x-rst
 
 Signal Edges
 ------------------------------------------------------------------------------------------------------------------------
 
 **Signal Edges** is a Python package capable of filtering, extracting state levels and edges of signals with millions
@@ -32,15 +32,15 @@
 
 Find **Signal Edges** on `PyPi <https://pypi.org/project/python-signal-edges/>`_, or install it as follows:
 
 .. code-block::
 
     pip install python-signal-edges
 
-Refer to the documentation `here <https://python-signal-edges.netlify.app/>`_ for more details.
+Refer to the documentation `here <https://dmg0345-python-signal-edges.netlify.app/>`_ for more details.
 
 Development
 ------------------------------------------------------------------------------------------------------------------------
 
 Clone the repository as:
 
 .. code-block:: powershell
```

## Comparing `python_signal_edges-1.0.4.dist-info/RECORD` & `python_signal_edges-1.0.5.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -19,11 +19,11 @@
 signal_edges/signal/sample/__init__.py,sha256=YmBKG4JpGPO0JADUXNFePDMn37y1OMTHIpGtnB8ussg,314
 signal_edges/signal/sample/sample.py,sha256=Ta5PERZW8YATAtgMTiPN29f_3-_U4WFhvJAo9kGWgMs,19205
 signal_edges/signal/signal.py,sha256=CsMxEtH9g6UkWJCi6oR9pR6CZ8NG3I1w8M8ztOWh40M,10326
 signal_edges/signal/state_levels/__init__.py,sha256=E_B0A18fGWLJZ4DL3n_8bxD-HBSBK2Tu2EHUuulYkTc,372
 signal_edges/signal/state_levels/definitions.py,sha256=4nN4LU70JqIl_Ih_v5kjqeUZ8BBHRU88-Jbc5NaFgn4,1421
 signal_edges/signal/state_levels/state_levels.py,sha256=X7nJQ29iqOXBOWluuRYhCF1cs8Hjfe_bJgT3-Sk_8JQ,14070
 signal_edges/signal/voltage_signal.py,sha256=-v8XGEto3lAIioVccHbgO6iAk0ZkHCI1bK9khwAPbbo,4334
-python_signal_edges-1.0.4.dist-info/LICENSE,sha256=r0EvAG4T_2wZyvzNsl4whvR33upjBVZfKLg15OJrghY,1084
-python_signal_edges-1.0.4.dist-info/METADATA,sha256=y_eo3-Jdx282Wgflvjise5c7DvnX4OLk6wMymMCGJAw,3100
-python_signal_edges-1.0.4.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-python_signal_edges-1.0.4.dist-info/RECORD,,
+python_signal_edges-1.0.5.dist-info/LICENSE,sha256=r0EvAG4T_2wZyvzNsl4whvR33upjBVZfKLg15OJrghY,1084
+python_signal_edges-1.0.5.dist-info/METADATA,sha256=LsQ5QlO-4hjcrmzzZ7jl1WCCFj-6x-OlYZZxUPXYxCI,3116
+python_signal_edges-1.0.5.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+python_signal_edges-1.0.5.dist-info/RECORD,,
```


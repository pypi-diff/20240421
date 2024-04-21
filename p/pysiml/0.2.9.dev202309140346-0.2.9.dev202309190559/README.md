# Comparing `tmp/pysiml-0.2.9.dev202309140346-py3-none-any.whl.zip` & `tmp/pysiml-0.2.9.dev202309190559-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -140,13 +140,13 @@
 -rw-r--r--  2.0 unx     2725 b- defN 80-Jan-01 00:00 siml/update_functions/standard_update.py
 -rw-r--r--  2.0 unx      430 b- defN 80-Jan-01 00:00 siml/update_functions/update_interface.py
 -rw-r--r--  2.0 unx    19828 b- defN 80-Jan-01 00:00 siml/util.py
 -rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 siml/utils/__init__.py
 -rw-r--r--  2.0 unx     7682 b- defN 80-Jan-01 00:00 siml/utils/fem_data_utils.py
 -rw-r--r--  2.0 unx     1403 b- defN 80-Jan-01 00:00 siml/utils/progress_bar.py
 -rw-r--r--  2.0 unx     1247 b- defN 80-Jan-01 00:00 siml/utils/timer.py
--rw-r--r--  2.0 unx    11431 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202309140346.dist-info/LICENSE
--rw-r--r--  2.0 unx     1662 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202309140346.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202309140346.dist-info/WHEEL
--rw-r--r--  2.0 unx      388 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202309140346.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    13723 b- defN 16-Jan-01 00:00 pysiml-0.2.9.dev202309140346.dist-info/RECORD
+-rw-r--r--  2.0 unx    11431 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202309190559.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1662 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202309190559.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202309190559.dist-info/WHEEL
+-rw-r--r--  2.0 unx      388 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202309190559.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    13723 b- defN 16-Jan-01 00:00 pysiml-0.2.9.dev202309190559.dist-info/RECORD
 150 files, 638413 bytes uncompressed, 160345 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -429,23 +429,23 @@
 
 Filename: siml/utils/progress_bar.py
 Comment: 
 
 Filename: siml/utils/timer.py
 Comment: 
 
-Filename: pysiml-0.2.9.dev202309140346.dist-info/LICENSE
+Filename: pysiml-0.2.9.dev202309190559.dist-info/LICENSE
 Comment: 
 
-Filename: pysiml-0.2.9.dev202309140346.dist-info/METADATA
+Filename: pysiml-0.2.9.dev202309190559.dist-info/METADATA
 Comment: 
 
-Filename: pysiml-0.2.9.dev202309140346.dist-info/WHEEL
+Filename: pysiml-0.2.9.dev202309190559.dist-info/WHEEL
 Comment: 
 
-Filename: pysiml-0.2.9.dev202309140346.dist-info/entry_points.txt
+Filename: pysiml-0.2.9.dev202309190559.dist-info/entry_points.txt
 Comment: 
 
-Filename: pysiml-0.2.9.dev202309140346.dist-info/RECORD
+Filename: pysiml-0.2.9.dev202309190559.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyproject.toml

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysiml"
-version = "0.2.9.dev202309140346"
+version = "0.2.9.dev202309190559"
 description = "SiML - a Simulation ML library"
 license = "Apache-2.0"
 authors = ["RICOS Co. Ltd."]
 readme = "README.md"
 repository = "https://github.com/ricosjp/pysiml"
 documentation = "https://ricosjp.github.io/pysiml/"
 packages = [
```

## Comparing `pysiml-0.2.9.dev202309140346.dist-info/LICENSE` & `pysiml-0.2.9.dev202309190559.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pysiml-0.2.9.dev202309140346.dist-info/METADATA` & `pysiml-0.2.9.dev202309190559.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysiml
-Version: 0.2.9.dev202309140346
+Version: 0.2.9.dev202309190559
 Summary: SiML - a Simulation ML library
 Home-page: https://github.com/ricosjp/pysiml
 License: Apache-2.0
 Author: RICOS Co. Ltd.
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pysiml-0.2.9.dev202309140346.dist-info/RECORD` & `pysiml-0.2.9.dev202309190559.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pyproject.toml,sha256=SLWacprbLTvJ9zuyekD3n9OGhNaz_UCVLk_wk48pP34,1546
+pyproject.toml,sha256=73oBLfZsZuk3NqhQg9fH88b89VdWsdFNTxb7OarJNaY,1546
 siml/__init__.py,sha256=mC61oSLHO5F6zXHhOrzH51R-vkH0mL4MShhSBiRRe6s,638
 siml/__main__/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 siml/__main__/convert_interim_data.py,sha256=jA6GD7BlnsEjARcln3UBwXlFj64BeFALAmgD1ohBkqo,900
 siml/__main__/convert_raw_data.py,sha256=VNVOyx9lChopF2Q-9OXtN_-MtfBsyjS_JvFwCjdkv0c,1400
 siml/__main__/optimize.py,sha256=6HALn60Mxh4GUiPbSXjvrdpkoQ4NgYSzCHCBRbli4W0,1742
 siml/__main__/plot_losses.py,sha256=0uMsoPN-xR0JhPg0WzSQL5GbD80ovuFO12eVpc0x6Xc,8663
 siml/__main__/prepare_preprocess_converters.py,sha256=w_rzic--RUyISagQOJw_5-oEkOFEKXUN7G1TkTOxd8g,927
@@ -139,12 +139,12 @@
 siml/update_functions/standard_update.py,sha256=LxkZAmXN7SNR2AqgqkocLoYhAeD78wx_vqT4dLisOpI,2725
 siml/update_functions/update_interface.py,sha256=Hk0_qdghgAzKBX9qLpBBcUy5L6H2bDSoK3wCPPcTrwk,430
 siml/util.py,sha256=Pb0eACoq4LiW5E7y3QhOZ0kPztX1toGwHtCFDJhAYKE,19828
 siml/utils/__init__.py,sha256=DVdxWEBXfapWAWNM0jUouKJzru4RyK2ru2QheBmrm_s,37
 siml/utils/fem_data_utils.py,sha256=LDB_MxYPg_WELl6D_az9ikMZxAF5Ml5qKUXR2CnuxvE,7682
 siml/utils/progress_bar.py,sha256=gHcJgdYP4xTo1DlZDxDIggwrxw39WaM_tCwvtLISNJA,1403
 siml/utils/timer.py,sha256=DEDtrmFpFqiGRykErkLMnwZ3tWUsOsarubnN40kwb6I,1247
-pysiml-0.2.9.dev202309140346.dist-info/LICENSE,sha256=Ok4O8jxCIpLhGZjTNzgBW8V8xITF_SUVEp1juLijZpA,11431
-pysiml-0.2.9.dev202309140346.dist-info/METADATA,sha256=QfVmuzBWCzhRO4YsYSZYT9I8AK5sGT3_0Jl-k4jrKXQ,1662
-pysiml-0.2.9.dev202309140346.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-pysiml-0.2.9.dev202309140346.dist-info/entry_points.txt,sha256=zXU0Gd56XeUfgaeG-CGXcYaTpORSU6kVeQ_vVvjIFPs,388
-pysiml-0.2.9.dev202309140346.dist-info/RECORD,,
+pysiml-0.2.9.dev202309190559.dist-info/LICENSE,sha256=Ok4O8jxCIpLhGZjTNzgBW8V8xITF_SUVEp1juLijZpA,11431
+pysiml-0.2.9.dev202309190559.dist-info/METADATA,sha256=CfLYbKbUvcPL2gJNIjQxCklFVNADkerGaN-_7KTvXY0,1662
+pysiml-0.2.9.dev202309190559.dist-info/WHEEL,sha256=d2fvjOD7sXsVzChCqf0Ty0JbHKBaLYwDbGQDwQTnJ50,88
+pysiml-0.2.9.dev202309190559.dist-info/entry_points.txt,sha256=zXU0Gd56XeUfgaeG-CGXcYaTpORSU6kVeQ_vVvjIFPs,388
+pysiml-0.2.9.dev202309190559.dist-info/RECORD,,
```


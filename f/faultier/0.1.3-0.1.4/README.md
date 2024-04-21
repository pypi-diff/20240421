# Comparing `tmp/faultier-0.1.3.tar.gz` & `tmp/faultier-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faultier-0.1.3.tar", last modified: Mon Mar 11 15:09:22 2024, max compression
+gzip compressed data, was "faultier-0.1.4.tar", last modified: Sun Apr 21 14:28:08 2024, max compression
```

## Comparing `faultier-0.1.3.tar` & `faultier-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-03-11 15:09:22.435356 faultier-0.1.3/
--rw-r--r--   0 thomas     (501) staff       (20)      522 2024-03-11 15:09:22.435167 faultier-0.1.3/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)       85 2024-03-11 10:46:46.000000 faultier-0.1.3/README.md
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-03-11 15:09:22.434279 faultier-0.1.3/docs/
--rw-r--r--   0 thomas     (501) staff       (20)   637437 2024-03-11 10:54:11.000000 faultier-0.1.3/docs/sideview.afdesign
--rw-r--r--   0 thomas     (501) staff       (20)   102775 2024-03-11 10:54:11.000000 faultier-0.1.3/docs/sideview.svg
--rw-r--r--   0 thomas     (501) staff       (20)  1168725 2024-03-11 10:54:11.000000 faultier-0.1.3/docs/topview.afdesign
--rw-r--r--   0 thomas     (501) staff       (20)   350221 2024-03-11 10:54:11.000000 faultier-0.1.3/docs/topview.svg
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-03-11 15:09:22.431002 faultier-0.1.3/faultier/
--rw-r--r--   0 thomas     (501) staff       (20)    19033 2024-03-11 11:04:03.000000 faultier-0.1.3/faultier/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     6185 2024-03-11 10:46:48.000000 faultier-0.1.3/faultier/faultier_pb2.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-03-11 15:09:22.434953 faultier-0.1.3/faultier.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)      522 2024-03-11 15:09:22.000000 faultier-0.1.3/faultier.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      351 2024-03-11 15:09:22.000000 faultier-0.1.3/faultier.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2024-03-11 15:09:22.000000 faultier-0.1.3/faultier.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)       16 2024-03-11 15:09:22.000000 faultier-0.1.3/faultier.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)        9 2024-03-11 15:09:22.000000 faultier-0.1.3/faultier.egg-info/top_level.txt
--rw-r--r--   0 thomas     (501) staff       (20)       38 2024-03-11 15:09:22.435401 faultier-0.1.3/setup.cfg
--rw-r--r--   0 thomas     (501) staff       (20)      796 2024-03-11 15:09:09.000000 faultier-0.1.3/setup.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 14:28:08.396295 faultier-0.1.4/
+-rw-r--r--   0 thomas     (501) staff       (20)      522 2024-04-21 14:28:08.396090 faultier-0.1.4/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)       85 2024-03-11 10:46:46.000000 faultier-0.1.4/README.md
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 14:28:08.392582 faultier-0.1.4/docs/
+-rw-r--r--   0 thomas     (501) staff       (20)   637437 2024-03-11 10:54:11.000000 faultier-0.1.4/docs/sideview.afdesign
+-rw-r--r--   0 thomas     (501) staff       (20)   102775 2024-03-11 10:54:11.000000 faultier-0.1.4/docs/sideview.svg
+-rw-r--r--   0 thomas     (501) staff       (20)  1168725 2024-03-11 10:54:11.000000 faultier-0.1.4/docs/topview.afdesign
+-rw-r--r--   0 thomas     (501) staff       (20)   350221 2024-03-11 10:54:11.000000 faultier-0.1.4/docs/topview.svg
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 14:28:08.394326 faultier-0.1.4/example_firmware/
+-rw-r--r--   0 thomas     (501) staff       (20)    72892 2024-03-11 11:18:12.000000 faultier-0.1.4/example_firmware/nrf52832_xxaa.hex
+-rw-r--r--   0 thomas     (501) staff       (20)   429491 2024-03-11 11:18:12.000000 faultier-0.1.4/example_firmware/s132_nrf52_7.2.0_softdevice.hex
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 14:28:08.387424 faultier-0.1.4/faultier/
+-rw-r--r--   0 thomas     (501) staff       (20)     6679 2024-03-16 14:19:42.000000 faultier-0.1.4/faultier/FaulterVis.py
+-rw-r--r--   0 thomas     (501) staff       (20)     9554 2024-04-18 10:58:34.000000 faultier-0.1.4/faultier/Faultier.py
+-rw-r--r--   0 thomas     (501) staff       (20)     2381 2024-03-16 14:19:07.000000 faultier-0.1.4/faultier/LivePlot.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1067 2024-03-16 14:18:41.000000 faultier-0.1.4/faultier/RandomOrderGenerator.py
+-rw-r--r--   0 thomas     (501) staff       (20)      125 2024-03-16 14:20:53.000000 faultier-0.1.4/faultier/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)     6185 2024-03-11 10:46:48.000000 faultier-0.1.4/faultier/faultier_pb2.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2024-04-21 14:28:08.395845 faultier-0.1.4/faultier.egg-info/
+-rw-r--r--   0 thomas     (501) staff       (20)      522 2024-04-21 14:28:08.000000 faultier-0.1.4/faultier.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)      557 2024-04-21 14:28:08.000000 faultier-0.1.4/faultier.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        1 2024-04-21 14:28:08.000000 faultier-0.1.4/faultier.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       16 2024-04-21 14:28:08.000000 faultier-0.1.4/faultier.egg-info/requires.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        9 2024-04-21 14:28:08.000000 faultier-0.1.4/faultier.egg-info/top_level.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       38 2024-04-21 14:28:08.396348 faultier-0.1.4/setup.cfg
+-rw-r--r--   0 thomas     (501) staff       (20)      752 2024-04-21 14:28:03.000000 faultier-0.1.4/setup.py
```

### Comparing `faultier-0.1.3/PKG-INFO` & `faultier-0.1.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faultier
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library to control the Faultier glitcher.
 Author: Thomas 'stacksmashing' Roth
 Author-email: code@stacksmashing.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `faultier-0.1.3/docs/sideview.afdesign` & `faultier-0.1.4/docs/sideview.afdesign`

 * *Files identical despite different names*

### Comparing `faultier-0.1.3/docs/sideview.svg` & `faultier-0.1.4/docs/sideview.svg`

 * *Files identical despite different names*

### Comparing `faultier-0.1.3/docs/topview.afdesign` & `faultier-0.1.4/docs/topview.afdesign`

 * *Files identical despite different names*

### Comparing `faultier-0.1.3/docs/topview.svg` & `faultier-0.1.4/docs/topview.svg`

 * *Files identical despite different names*

### Comparing `faultier-0.1.3/faultier/faultier_pb2.py` & `faultier-0.1.4/faultier/faultier_pb2.py`

 * *Files identical despite different names*

### Comparing `faultier-0.1.3/faultier.egg-info/PKG-INFO` & `faultier-0.1.4/faultier.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faultier
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library to control the Faultier glitcher.
 Author: Thomas 'stacksmashing' Roth
 Author-email: code@stacksmashing.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `faultier-0.1.3/setup.py` & `faultier-0.1.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='faultier',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     package_data={
-        # If your package is named "faultier", and you want to include everything under "docs"
         'faultier': ['../docs/*.svg'],
+        'faultier': ['../example_firmware/*.hex'],
     },
     install_requires=[
         'pyserial', 'plotly'
     ],
     author='Thomas \'stacksmashing\' Roth',
     author_email='code@stacksmashing.net',
     description='A library to control the Faultier glitcher.',
```


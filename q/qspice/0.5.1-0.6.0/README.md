# Comparing `tmp/qspice-0.5.1.tar.gz` & `tmp/qspice-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qspice-0.5.1.tar", last modified: Sat Mar  9 17:09:13 2024, max compression
+gzip compressed data, was "qspice-0.6.0.tar", last modified: Sun Apr 21 15:03:02 2024, max compression
```

## Comparing `qspice-0.5.1.tar` & `qspice-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-03-09 17:09:13.982530 qspice-0.5.1/
--rw-rw-rw-   0        0        0    35823 2023-09-01 12:48:49.000000 qspice-0.5.1/LICENSE
--rw-rw-rw-   0        0        0    53784 2024-03-09 17:09:13.981531 qspice-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0    12117 2024-03-09 17:08:16.000000 qspice-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-09 17:09:13.961929 qspice-0.5.1/examples/
--rw-rw-rw-   0        0        0     1057 2023-09-13 20:11:15.000000 qspice-0.5.1/examples/prepare_worst_case.py
--rw-rw-rw-   0        0        0      633 2023-10-18 20:39:29.000000 qspice-0.5.1/examples/qsch_editor_example.py
--rw-rw-rw-   0        0        0     1484 2024-02-23 21:06:01.000000 qspice-0.5.1/examples/qspice_example.py
--rw-rw-rw-   0        0        0     2356 2024-02-25 17:47:37.000000 qspice-0.5.1/examples/run_montecarlo.py
--rw-rw-rw-   0        0        0      849 2024-03-09 17:06:25.000000 qspice-0.5.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-09 17:09:13.966552 qspice-0.5.1/qspice/
--rw-rw-rw-   0        0        0      457 2023-10-18 20:19:50.000000 qspice-0.5.1/qspice/__init__.py
--rw-rw-rw-   0        0        0     5753 2023-09-13 20:11:15.000000 qspice-0.5.1/qspice/qspice.py
-drwxrwxrwx   0        0        0        0 2024-03-09 17:09:13.976656 qspice-0.5.1/qspice/sim/
--rw-rw-rw-   0        0        0     7508 2023-10-18 17:45:11.000000 qspice-0.5.1/qspice/sim/sim_runner.py
-drwxrwxrwx   0        0        0        0 2024-03-09 17:09:13.980529 qspice-0.5.1/qspice.egg-info/
--rw-rw-rw-   0        0        0    53784 2024-03-09 17:09:13.000000 qspice-0.5.1/qspice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2024-03-09 17:09:13.000000 qspice-0.5.1/qspice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-09 17:09:13.000000 qspice-0.5.1/qspice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-03-09 17:09:13.000000 qspice-0.5.1/qspice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2024-03-09 17:09:13.000000 qspice-0.5.1/qspice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-09 17:09:13.983530 qspice-0.5.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-09 17:09:13.978516 qspice-0.5.1/tests/
--rw-rw-rw-   0        0        0     2531 2024-03-02 19:55:45.000000 qspice-0.5.1/tests/david_zimmermann.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:03:02.778559 qspice-0.6.0/
+-rw-rw-rw-   0        0        0    35823 2023-09-01 12:48:49.000000 qspice-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0    53882 2024-04-21 15:03:02.777156 qspice-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0    12215 2024-04-21 14:57:42.000000 qspice-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 15:03:02.761886 qspice-0.6.0/examples/
+-rw-rw-rw-   0        0        0     1057 2023-09-13 20:11:15.000000 qspice-0.6.0/examples/prepare_worst_case.py
+-rw-rw-rw-   0        0        0      633 2023-10-18 20:39:29.000000 qspice-0.6.0/examples/qsch_editor_example.py
+-rw-rw-rw-   0        0        0     1484 2024-02-23 21:06:01.000000 qspice-0.6.0/examples/qspice_example.py
+-rw-rw-rw-   0        0        0     2356 2024-02-25 17:47:37.000000 qspice-0.6.0/examples/run_montecarlo.py
+-rw-rw-rw-   0        0        0      849 2024-04-21 14:59:40.000000 qspice-0.6.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-21 15:03:02.765350 qspice-0.6.0/qspice/
+-rw-rw-rw-   0        0        0      457 2023-10-18 20:19:50.000000 qspice-0.6.0/qspice/__init__.py
+-rw-rw-rw-   0        0        0     5753 2023-09-13 20:11:15.000000 qspice-0.6.0/qspice/qspice.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:03:02.772440 qspice-0.6.0/qspice/sim/
+-rw-rw-rw-   0        0        0     7508 2023-10-18 17:45:11.000000 qspice-0.6.0/qspice/sim/sim_runner.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:03:02.775647 qspice-0.6.0/qspice.egg-info/
+-rw-rw-rw-   0        0        0    53882 2024-04-21 15:03:02.000000 qspice-0.6.0/qspice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2024-04-21 15:03:02.000000 qspice-0.6.0/qspice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 15:03:02.000000 qspice-0.6.0/qspice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-21 15:03:02.000000 qspice-0.6.0/qspice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2024-04-21 15:03:02.000000 qspice-0.6.0/qspice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 15:03:02.778559 qspice-0.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-21 15:03:02.774230 qspice-0.6.0/tests/
+-rw-rw-rw-   0        0        0     2531 2024-03-02 19:55:45.000000 qspice-0.6.0/tests/david_zimmermann.py
```

### Comparing `qspice-0.5.1/LICENSE` & `qspice-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qspice-0.5.1/PKG-INFO` & `qspice-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qspice
-Version: 0.5.1
+Version: 0.6.0
 Summary: A set of tools to operate with QSPICE
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,15 +680,15 @@
         
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: spicelib>=1.0.3
+Requires-Dist: spicelib>=1.1.1
 
 # QSPICE
 
 QSPICE is a toolchain of python utilities design to interact specifically with QSPICE.
 
 ## What is contained in this repository ##
 
@@ -944,14 +944,16 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 0.6.0
+  * Hierarchical Schematics are now supported. (Alignement with spicelib 1.1.1)
 * Version 0.5.1
   * Adding a tool that allows to convert LTSpice to QSpice Schematics (Alpha Stage - Not fully functional)
   * Correcting the generation of a .net from the QschEditor. (spicelib 1.0.3)
 * Version 0.5.0
   * Fixes on the montecarlo example.
   * Aligning with spicelib 1.0.1
 * Version 0.4
```

### Comparing `qspice-0.5.1/README.md` & `qspice-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -256,14 +256,16 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 0.6.0
+  * Hierarchical Schematics are now supported. (Alignement with spicelib 1.1.1)
 * Version 0.5.1
   * Adding a tool that allows to convert LTSpice to QSpice Schematics (Alpha Stage - Not fully functional)
   * Correcting the generation of a .net from the QschEditor. (spicelib 1.0.3)
 * Version 0.5.0
   * Fixes on the montecarlo example.
   * Aligning with spicelib 1.0.1
 * Version 0.4
```

### Comparing `qspice-0.5.1/examples/prepare_worst_case.py` & `qspice-0.6.0/examples/prepare_worst_case.py`

 * *Files identical despite different names*

### Comparing `qspice-0.5.1/examples/qsch_editor_example.py` & `qspice-0.6.0/examples/qsch_editor_example.py`

 * *Files identical despite different names*

### Comparing `qspice-0.5.1/examples/qspice_example.py` & `qspice-0.6.0/examples/qspice_example.py`

 * *Files identical despite different names*

### Comparing `qspice-0.5.1/examples/run_montecarlo.py` & `qspice-0.6.0/examples/run_montecarlo.py`

 * *Files identical despite different names*

### Comparing `qspice-0.5.1/pyproject.toml` & `qspice-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 requires = [
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "qspice"
-version = "0.5.1"
+version = "0.6.0"
 authors = [
   { name="Nuno Brum", email="me@nunobrum.com" },
 ]
 description = "A set of tools to operate with QSPICE"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
 dependencies = [
-    "spicelib>=1.0.3",
+    "spicelib>=1.1.1",
 ]
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `qspice-0.5.1/qspice/qspice.py` & `qspice-0.6.0/qspice/qspice.py`

 * *Files identical despite different names*

### Comparing `qspice-0.5.1/qspice/sim/sim_runner.py` & `qspice-0.6.0/qspice/sim/sim_runner.py`

 * *Files identical despite different names*

### Comparing `qspice-0.5.1/qspice.egg-info/PKG-INFO` & `qspice-0.6.0/qspice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qspice
-Version: 0.5.1
+Version: 0.6.0
 Summary: A set of tools to operate with QSPICE
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,15 +680,15 @@
         
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: spicelib>=1.0.3
+Requires-Dist: spicelib>=1.1.1
 
 # QSPICE
 
 QSPICE is a toolchain of python utilities design to interact specifically with QSPICE.
 
 ## What is contained in this repository ##
 
@@ -944,14 +944,16 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 0.6.0
+  * Hierarchical Schematics are now supported. (Alignement with spicelib 1.1.1)
 * Version 0.5.1
   * Adding a tool that allows to convert LTSpice to QSpice Schematics (Alpha Stage - Not fully functional)
   * Correcting the generation of a .net from the QschEditor. (spicelib 1.0.3)
 * Version 0.5.0
   * Fixes on the montecarlo example.
   * Aligning with spicelib 1.0.1
 * Version 0.4
```

### Comparing `qspice-0.5.1/tests/david_zimmermann.py` & `qspice-0.6.0/tests/david_zimmermann.py`

 * *Files identical despite different names*


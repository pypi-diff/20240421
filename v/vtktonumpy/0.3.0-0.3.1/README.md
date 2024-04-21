# Comparing `tmp/vtktonumpy-0.3.0.tar.gz` & `tmp/vtktonumpy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtktonumpy-0.3.0.tar", last modified: Tue Dec  5 15:51:12 2023, max compression
+gzip compressed data, was "vtktonumpy-0.3.1.tar", last modified: Sun Apr 21 00:24:01 2024, max compression
```

## Comparing `vtktonumpy-0.3.0.tar` & `vtktonumpy-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 15:51:12.229155 vtktonumpy-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 15:51:12.225155 vtktonumpy-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 15:51:12.225155 vtktonumpy-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-12-05 15:51:01.000000 vtktonumpy-0.3.0/.github/workflows/CIReports.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2023-12-05 15:51:01.000000 vtktonumpy-0.3.0/.github/workflows/CITests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2023-12-05 15:51:01.000000 vtktonumpy-0.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-12-05 15:51:01.000000 vtktonumpy-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2023-12-05 15:51:01.000000 vtktonumpy-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-12-05 15:51:01.000000 vtktonumpy-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2023-12-05 15:51:12.229155 vtktonumpy-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-12-05 15:51:01.000000 vtktonumpy-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-12-05 15:51:01.000000 vtktonumpy-0.3.0/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-05 15:51:01.000000 vtktonumpy-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-05 15:51:01.000000 vtktonumpy-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-05 15:51:12.229155 vtktonumpy-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 15:51:12.225155 vtktonumpy-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2023-12-05 15:51:01.000000 vtktonumpy-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2023-12-05 15:51:01.000000 vtktonumpy-0.3.0/tests/test_vtkgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2023-12-05 15:51:01.000000 vtktonumpy-0.3.0/tests/test_vtkreader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 15:51:12.229155 vtktonumpy-0.3.0/vtktonumpy/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-05 15:51:01.000000 vtktonumpy-0.3.0/vtktonumpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7132 2023-12-05 15:51:01.000000 vtktonumpy-0.3.0/vtktonumpy/vtkgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2023-12-05 15:51:01.000000 vtktonumpy-0.3.0/vtktonumpy/vtkreader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 15:51:12.229155 vtktonumpy-0.3.0/vtktonumpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2023-12-05 15:51:12.000000 vtktonumpy-0.3.0/vtktonumpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-12-05 15:51:12.000000 vtktonumpy-0.3.0/vtktonumpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 15:51:12.000000 vtktonumpy-0.3.0/vtktonumpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-05 15:51:12.000000 vtktonumpy-0.3.0/vtktonumpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-05 15:51:12.000000 vtktonumpy-0.3.0/vtktonumpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:24:01.689296 vtktonumpy-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:24:01.685296 vtktonumpy-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:24:01.685296 vtktonumpy-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-21 00:23:56.000000 vtktonumpy-0.3.1/.github/workflows/CIReports.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-21 00:23:56.000000 vtktonumpy-0.3.1/.github/workflows/CITests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-21 00:23:56.000000 vtktonumpy-0.3.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-21 00:23:56.000000 vtktonumpy-0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-21 00:23:56.000000 vtktonumpy-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 00:23:56.000000 vtktonumpy-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-21 00:24:01.689296 vtktonumpy-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-21 00:23:56.000000 vtktonumpy-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-21 00:23:56.000000 vtktonumpy-0.3.1/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-21 00:23:56.000000 vtktonumpy-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-21 00:23:56.000000 vtktonumpy-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 00:24:01.689296 vtktonumpy-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:24:01.685296 vtktonumpy-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-21 00:23:56.000000 vtktonumpy-0.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-21 00:23:56.000000 vtktonumpy-0.3.1/tests/test_vtkgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-21 00:23:56.000000 vtktonumpy-0.3.1/tests/test_vtkreader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:24:01.685296 vtktonumpy-0.3.1/vtktonumpy/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-21 00:23:56.000000 vtktonumpy-0.3.1/vtktonumpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-04-21 00:23:56.000000 vtktonumpy-0.3.1/vtktonumpy/vtkgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-21 00:23:56.000000 vtktonumpy-0.3.1/vtktonumpy/vtkreader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:24:01.689296 vtktonumpy-0.3.1/vtktonumpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-21 00:24:01.000000 vtktonumpy-0.3.1/vtktonumpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-21 00:24:01.000000 vtktonumpy-0.3.1/vtktonumpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 00:24:01.000000 vtktonumpy-0.3.1/vtktonumpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 00:24:01.000000 vtktonumpy-0.3.1/vtktonumpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 00:24:01.000000 vtktonumpy-0.3.1/vtktonumpy.egg-info/top_level.txt
```

### Comparing `vtktonumpy-0.3.0/.github/workflows/CIReports.yml` & `vtktonumpy-0.3.1/.github/workflows/CIReports.yml`

 * *Files 17% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 name: CI Reports
 
 on:
   push:
     branches: [ "main" ]
   pull_request:
     branches: [ "main" ]
+  workflow_dispatch:
 
 jobs:
   run:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python 3.11
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v5
       with:
         python-version: '3.11'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install pytest-cov
         python -m pip install -r requirements.txt
     - name: Run tests and collect coverage
       run: python -m pytest --cov vtktonumpy
     - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `vtktonumpy-0.3.0/.github/workflows/CITests.yml` & `vtktonumpy-0.3.1/.github/workflows/CITests.yml`

 * *Files 26% similar despite different names*

```diff
@@ -14,28 +14,38 @@
   build:
 
     runs-on: ubuntu-20.04
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.6", "3.7", "3.8", "3.9", "3.10", "3.11"]
-        vtk-version: ["9.1.*", "9.2.*"]
+        vtk-version: ["9.0.*","9.1.*", "9.2.*","9.3.*","9.*"]
         numpy-version: ["1.*"]
 
         exclude:
+          - python-version: "3.8"
+            vtk-version: "9.0.*"
+
+          - python-version: "3.9"
+            vtk-version: "9.0.*"
+
+          - python-version: "3.10"
+            vtk-version: "9.0.*"
           - python-version: "3.10"
             vtk-version: "9.1.*"
 
           - python-version: "3.11"
+            vtk-version: "9.0.*"
+          - python-version: "3.11"
             vtk-version: "9.1.*"
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install flake8 pytest
         python -m pip install "vtk==${{matrix.vtk-version}}"
```

### Comparing `vtktonumpy-0.3.0/.github/workflows/docs.yml` & `vtktonumpy-0.3.1/.github/workflows/docs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 jobs:
   # Build the documentation and upload the static HTML files as an artifact.
   build:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: '3.12'
 
       # Install all dependencies (including pdoc)
       - run: pip install -r requirements.txt
       # Build documentation into docs/.
       - run: pdoc -o docs/ --docformat google --math --footer-text $(python -m setuptools_scm) vtktonumpy 
@@ -39,8 +39,8 @@
       pages: write
       id-token: write
     environment:
       name: github-pages
       url: ${{ steps.deployment.outputs.page_url }}
     steps:
       - id: deployment
-        uses: actions/deploy-pages@v2
+        uses: actions/deploy-pages@v3
```

### Comparing `vtktonumpy-0.3.0/.github/workflows/python-publish.yml` & `vtktonumpy-0.3.1/.github/workflows/python-publish.yml`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
```

### Comparing `vtktonumpy-0.3.0/.gitignore` & `vtktonumpy-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `vtktonumpy-0.3.0/LICENSE` & `vtktonumpy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vtktonumpy-0.3.0/PKG-INFO` & `vtktonumpy-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtktonumpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Read VTK rectilinear grid files and output as N-dimensional NumPy arrays
 Author: Declan B. Gaylo
 License: MIT License
         
         Copyright (c) 2023 Declan Gaylo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,15 @@
 Project-URL: Documentation, https://dgaylo.github.io/VTKToNumpy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: vtk>=9.1
+Requires-Dist: vtk>=9.0
 
 # VTKToNumpy
 ![CI Tests](https://github.com/dgaylo/VTKToNumpy/actions/workflows/CITests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/dgaylo/VTKToNumpy/graph/badge.svg?token=O9XNA7HUAI)](https://codecov.io/gh/dgaylo/VTKToNumpy)
 
 A python library that makes it easy to read cell data from [VTK](https://vtk.org/) rectilinear grid files and convert it to n-dimensional [NumPy](https://numpy.org/) arrays.
```

### Comparing `vtktonumpy-0.3.0/pylintrc` & `vtktonumpy-0.3.1/pylintrc`

 * *Files identical despite different names*

### Comparing `vtktonumpy-0.3.0/pyproject.toml` & `vtktonumpy-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License"
 ]
 
 dependencies = [
   "numpy",
-  "vtk>=9.1",
+  "vtk>=9.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/dgaylo/VTKToNumpy"
 "Bug Tracker" = "https://github.com/dgaylo/VTKToNumpy/issues"
 "Documentation" = "https://dgaylo.github.io/VTKToNumpy"
```

### Comparing `vtktonumpy-0.3.0/tests/conftest.py` & `vtktonumpy-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vtktonumpy-0.3.0/tests/test_vtkgrid.py` & `vtktonumpy-0.3.1/tests/test_vtkgrid.py`

 * *Files identical despite different names*

### Comparing `vtktonumpy-0.3.0/tests/test_vtkreader.py` & `vtktonumpy-0.3.1/tests/test_vtkreader.py`

 * *Files identical despite different names*

### Comparing `vtktonumpy-0.3.0/vtktonumpy/vtkgrid.py` & `vtktonumpy-0.3.1/vtktonumpy/vtkgrid.py`

 * *Files identical despite different names*

### Comparing `vtktonumpy-0.3.0/vtktonumpy/vtkreader.py` & `vtktonumpy-0.3.1/vtktonumpy/vtkreader.py`

 * *Files identical despite different names*

### Comparing `vtktonumpy-0.3.0/vtktonumpy.egg-info/PKG-INFO` & `vtktonumpy-0.3.1/vtktonumpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtktonumpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Read VTK rectilinear grid files and output as N-dimensional NumPy arrays
 Author: Declan B. Gaylo
 License: MIT License
         
         Copyright (c) 2023 Declan Gaylo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,15 @@
 Project-URL: Documentation, https://dgaylo.github.io/VTKToNumpy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: vtk>=9.1
+Requires-Dist: vtk>=9.0
 
 # VTKToNumpy
 ![CI Tests](https://github.com/dgaylo/VTKToNumpy/actions/workflows/CITests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/dgaylo/VTKToNumpy/graph/badge.svg?token=O9XNA7HUAI)](https://codecov.io/gh/dgaylo/VTKToNumpy)
 
 A python library that makes it easy to read cell data from [VTK](https://vtk.org/) rectilinear grid files and convert it to n-dimensional [NumPy](https://numpy.org/) arrays.
```


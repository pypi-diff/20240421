# Comparing `tmp/pyfetch_mimic-0.0.4.tar.gz` & `tmp/pyfetch_mimic-2024.4.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfetch_mimic-0.0.4.tar", last modified: Sat Mar 30 03:26:41 2024, max compression
+gzip compressed data, was "pyfetch_mimic-2024.4.20.tar", last modified: Sun Apr 21 02:51:37 2024, max compression
```

## Comparing `pyfetch_mimic-0.0.4.tar` & `pyfetch_mimic-2024.4.20.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:26:41.927990 pyfetch_mimic-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-30 03:26:33.000000 pyfetch_mimic-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-03-30 03:26:41.923990 pyfetch_mimic-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-03-30 03:26:33.000000 pyfetch_mimic-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-30 03:26:33.000000 pyfetch_mimic-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 03:26:41.927990 pyfetch_mimic-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:26:41.923990 pyfetch_mimic-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:26:41.923990 pyfetch_mimic-0.0.4/src/pyfetch_mimic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-03-30 03:26:41.000000 pyfetch_mimic-0.0.4/src/pyfetch_mimic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-30 03:26:41.000000 pyfetch_mimic-0.0.4/src/pyfetch_mimic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 03:26:41.000000 pyfetch_mimic-0.0.4/src/pyfetch_mimic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-30 03:26:41.000000 pyfetch_mimic-0.0.4/src/pyfetch_mimic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-30 03:26:41.000000 pyfetch_mimic-0.0.4/src/pyfetch_mimic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-03-30 03:26:33.000000 pyfetch_mimic-0.0.4/src/pyfetch_mimic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:26:41.923990 pyfetch_mimic-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-03-30 03:26:34.000000 pyfetch_mimic-0.0.4/test/test_endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:51:37.316027 pyfetch_mimic-2024.4.20/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 02:51:32.000000 pyfetch_mimic-2024.4.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-04-21 02:51:37.312027 pyfetch_mimic-2024.4.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-21 02:51:32.000000 pyfetch_mimic-2024.4.20/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-21 02:51:32.000000 pyfetch_mimic-2024.4.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 02:51:37.316027 pyfetch_mimic-2024.4.20/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:51:37.312027 pyfetch_mimic-2024.4.20/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:51:37.312027 pyfetch_mimic-2024.4.20/src/pyfetch_mimic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-04-21 02:51:37.000000 pyfetch_mimic-2024.4.20/src/pyfetch_mimic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-21 02:51:37.000000 pyfetch_mimic-2024.4.20/src/pyfetch_mimic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 02:51:37.000000 pyfetch_mimic-2024.4.20/src/pyfetch_mimic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-21 02:51:37.000000 pyfetch_mimic-2024.4.20/src/pyfetch_mimic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 02:51:37.000000 pyfetch_mimic-2024.4.20/src/pyfetch_mimic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-21 02:51:32.000000 pyfetch_mimic-2024.4.20/src/pyfetch_mimic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:51:37.312027 pyfetch_mimic-2024.4.20/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-21 02:51:33.000000 pyfetch_mimic-2024.4.20/test/test_endpoints.py
```

### Comparing `pyfetch_mimic-0.0.4/LICENSE` & `pyfetch_mimic-2024.4.20/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfetch_mimic-0.0.4/PKG-INFO` & `pyfetch_mimic-2024.4.20/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: pyfetch_mimic
-Version: 0.0.4
+Version: 2024.4.20
 Summary: This is a module that mimics pyodide.http.pyfetch to enable simpler development by using one set of http calls for both local and pyodide executions.
 Author-email: darrida <darrida.py@gmail.com>
 Project-URL: Homepage, https://github.com/darrida/py-shinylive-pyfetch-mimic
 Project-URL: Issues, https://github.com/darrida/py-shinylive-pyfetch-mimic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: shiny
-Requires-Dist: shinylive
 Requires-Dist: httpx
 Requires-Dist: python_version<3
 Provides-Extra: tests
 Requires-Dist: fastapi; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-asyncio; extra == "tests"
 Requires-Dist: robotframework; extra == "tests"
 Requires-Dist: robotframework-dependencylibrary; extra == "tests"
 Requires-Dist: robotframework-pythonlibcore; extra == "tests"
 Requires-Dist: robotframework-seleniumlibrary; extra == "tests"
 Requires-Dist: robotframework-stacktrace; extra == "tests"
 Requires-Dist: selenium; extra == "tests"
 Requires-Dist: seleniumbase; extra == "tests"
 Requires-Dist: coverage; extra == "tests"
+Requires-Dist: shinylive; extra == "tests"
 
 # pyfetch-mimic
 - This is a simple module that mimics `pyodide.http.pyfetch` to make local development for `shinylive` projects easier. It may work with `pyodide` in general, but that use case hasn't been tested.
-- For more information on Shinylive for Python see: https://shiny.posit.co/py/docs/shinylive.html
+- For more information on Shinylive for Python, and general information on how to use additional third party libraries (like this one), see: https://shiny.posit.co/py/docs/shinylive.html
 
 ## Install
 - PyPI: `pip install pyfetch-mimic`
 - Vendoring:
   - Copy `pyfetch_mimic.py` into your own project
 
 ## How to use
@@ -42,15 +42,15 @@
     import sys
     if "pyodide" in sys.modules:
         from pyodide import http
     else:
         from pyfetch_mimic import http
     ```
 - Use `http.pyfetch` as usual
-- **NOTE**: This is a *work in progress* and does not support all use case variations yet. It will be updated as need arises.
+- **NOTE**: This is a *work in progress* and does not support all `pyodide.http.pyfetch` functionality yet. I use this in my own production work, and the functionality that currently exists is simply the functionality that I need. If there is a need for additional functionality, please open an issue or pull request.
 
 ## pyfetch examples
 - These should all work with python `pyodide.http.pyfetch` and `pyfetch_mimic.http.pyfetch`
 
 ```python
 # Download, save extracted file to local virtual fs
 import sys
@@ -97,15 +97,15 @@
 ```
 
 ## Testing
 
 ### Install Test Dependencies
 - `pip install -e '.[tests]'`
 
-### Run regular tests (verifes test endpoints and tests `pyfetch-mimic`)
+### Run regular tests (verifies test endpoints and tests `pyfetch-mimic`)
 - activate venv: `source .venv/bin/activate`
 - start fastapi app: `python3 src_test_webserver/main.py`
 - run pytest: `pytest -vv -x test`
 
 ### Run pyodide tests with pyfetch calls written identical to `pyfetch-mimc`
 
 #### Manually
```

### Comparing `pyfetch_mimic-0.0.4/README.md` & `pyfetch_mimic-2024.4.20/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pyfetch-mimic
 - This is a simple module that mimics `pyodide.http.pyfetch` to make local development for `shinylive` projects easier. It may work with `pyodide` in general, but that use case hasn't been tested.
-- For more information on Shinylive for Python see: https://shiny.posit.co/py/docs/shinylive.html
+- For more information on Shinylive for Python, and general information on how to use additional third party libraries (like this one), see: https://shiny.posit.co/py/docs/shinylive.html
 
 ## Install
 - PyPI: `pip install pyfetch-mimic`
 - Vendoring:
   - Copy `pyfetch_mimic.py` into your own project
 
 ## How to use
@@ -13,15 +13,15 @@
     import sys
     if "pyodide" in sys.modules:
         from pyodide import http
     else:
         from pyfetch_mimic import http
     ```
 - Use `http.pyfetch` as usual
-- **NOTE**: This is a *work in progress* and does not support all use case variations yet. It will be updated as need arises.
+- **NOTE**: This is a *work in progress* and does not support all `pyodide.http.pyfetch` functionality yet. I use this in my own production work, and the functionality that currently exists is simply the functionality that I need. If there is a need for additional functionality, please open an issue or pull request.
 
 ## pyfetch examples
 - These should all work with python `pyodide.http.pyfetch` and `pyfetch_mimic.http.pyfetch`
 
 ```python
 # Download, save extracted file to local virtual fs
 import sys
@@ -68,15 +68,15 @@
 ```
 
 ## Testing
 
 ### Install Test Dependencies
 - `pip install -e '.[tests]'`
 
-### Run regular tests (verifes test endpoints and tests `pyfetch-mimic`)
+### Run regular tests (verifies test endpoints and tests `pyfetch-mimic`)
 - activate venv: `source .venv/bin/activate`
 - start fastapi app: `python3 src_test_webserver/main.py`
 - run pytest: `pytest -vv -x test`
 
 ### Run pyodide tests with pyfetch calls written identical to `pyfetch-mimc`
 
 #### Manually
@@ -85,8 +85,8 @@
 - open shinylive app in edit mode: `http://localhost8000/apps/edit/`
 - Click "Run tests"
 - If all function names at the bottom are followed by "passed", then everything should be ok
 
 #### Using Robot Framework
 - activate venv
 - export shinylive app: `shinylive export ./test/tests_shinylive ./src_test_webserver/shinyapps`
-- run robot: `robot test/robot_tests/`
+- run robot: `robot test/robot_tests/`
```

### Comparing `pyfetch_mimic-0.0.4/pyproject.toml` & `pyfetch_mimic-2024.4.20/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [project]
 name = "pyfetch_mimic"
-version = "0.0.4"
+version = "2024.04.20"
 authors = [
   {name="darrida", email="darrida.py@gmail.com"}
 ]
 description = "This is a module that mimics pyodide.http.pyfetch to enable simpler development by using one set of http calls for both local and pyodide executions."
 readme = "README.md"
 dependencies = [
   'shiny',
-  'shinylive',
   'httpx',
   'python_version < 3',
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -26,15 +25,16 @@
   'robotframework',
   'robotframework-dependencylibrary',
   'robotframework-pythonlibcore',
   'robotframework-seleniumlibrary',
   'robotframework-stacktrace',
   'selenium',
   'seleniumbase',
-  'coverage'
+  'coverage',
+  'shinylive'
 ]
 
 [project.urls]
 Homepage = "https://github.com/darrida/py-shinylive-pyfetch-mimic"
 Issues = "https://github.com/darrida/py-shinylive-pyfetch-mimic/issues"
 
 [build-system]
```

### Comparing `pyfetch_mimic-0.0.4/src/pyfetch_mimic.egg-info/PKG-INFO` & `pyfetch_mimic-2024.4.20/src/pyfetch_mimic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: pyfetch_mimic
-Version: 0.0.4
+Version: 2024.4.20
 Summary: This is a module that mimics pyodide.http.pyfetch to enable simpler development by using one set of http calls for both local and pyodide executions.
 Author-email: darrida <darrida.py@gmail.com>
 Project-URL: Homepage, https://github.com/darrida/py-shinylive-pyfetch-mimic
 Project-URL: Issues, https://github.com/darrida/py-shinylive-pyfetch-mimic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: shiny
-Requires-Dist: shinylive
 Requires-Dist: httpx
 Requires-Dist: python_version<3
 Provides-Extra: tests
 Requires-Dist: fastapi; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-asyncio; extra == "tests"
 Requires-Dist: robotframework; extra == "tests"
 Requires-Dist: robotframework-dependencylibrary; extra == "tests"
 Requires-Dist: robotframework-pythonlibcore; extra == "tests"
 Requires-Dist: robotframework-seleniumlibrary; extra == "tests"
 Requires-Dist: robotframework-stacktrace; extra == "tests"
 Requires-Dist: selenium; extra == "tests"
 Requires-Dist: seleniumbase; extra == "tests"
 Requires-Dist: coverage; extra == "tests"
+Requires-Dist: shinylive; extra == "tests"
 
 # pyfetch-mimic
 - This is a simple module that mimics `pyodide.http.pyfetch` to make local development for `shinylive` projects easier. It may work with `pyodide` in general, but that use case hasn't been tested.
-- For more information on Shinylive for Python see: https://shiny.posit.co/py/docs/shinylive.html
+- For more information on Shinylive for Python, and general information on how to use additional third party libraries (like this one), see: https://shiny.posit.co/py/docs/shinylive.html
 
 ## Install
 - PyPI: `pip install pyfetch-mimic`
 - Vendoring:
   - Copy `pyfetch_mimic.py` into your own project
 
 ## How to use
@@ -42,15 +42,15 @@
     import sys
     if "pyodide" in sys.modules:
         from pyodide import http
     else:
         from pyfetch_mimic import http
     ```
 - Use `http.pyfetch` as usual
-- **NOTE**: This is a *work in progress* and does not support all use case variations yet. It will be updated as need arises.
+- **NOTE**: This is a *work in progress* and does not support all `pyodide.http.pyfetch` functionality yet. I use this in my own production work, and the functionality that currently exists is simply the functionality that I need. If there is a need for additional functionality, please open an issue or pull request.
 
 ## pyfetch examples
 - These should all work with python `pyodide.http.pyfetch` and `pyfetch_mimic.http.pyfetch`
 
 ```python
 # Download, save extracted file to local virtual fs
 import sys
@@ -97,15 +97,15 @@
 ```
 
 ## Testing
 
 ### Install Test Dependencies
 - `pip install -e '.[tests]'`
 
-### Run regular tests (verifes test endpoints and tests `pyfetch-mimic`)
+### Run regular tests (verifies test endpoints and tests `pyfetch-mimic`)
 - activate venv: `source .venv/bin/activate`
 - start fastapi app: `python3 src_test_webserver/main.py`
 - run pytest: `pytest -vv -x test`
 
 ### Run pyodide tests with pyfetch calls written identical to `pyfetch-mimc`
 
 #### Manually
```

### Comparing `pyfetch_mimic-0.0.4/src/pyfetch_mimic.py` & `pyfetch_mimic-2024.4.20/src/pyfetch_mimic.py`

 * *Files identical despite different names*

### Comparing `pyfetch_mimic-0.0.4/test/test_endpoints.py` & `pyfetch_mimic-2024.4.20/test/test_endpoints.py`

 * *Files identical despite different names*


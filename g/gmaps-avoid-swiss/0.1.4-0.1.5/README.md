# Comparing `tmp/gmaps_avoid_swiss-0.1.4.tar.gz` & `tmp/gmaps_avoid_swiss-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmaps_avoid_swiss-0.1.4.tar", last modified: Fri Apr 19 20:12:27 2024, max compression
+gzip compressed data, was "gmaps_avoid_swiss-0.1.5.tar", last modified: Sun Apr 21 03:28:16 2024, max compression
```

## Comparing `gmaps_avoid_swiss-0.1.4.tar` & `gmaps_avoid_swiss-0.1.5.tar`

### file list

```diff
@@ -1,47 +1,44 @@
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 20:12:27.978002 gmaps_avoid_swiss-0.1.4/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      162 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.4/AUTHORS.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     3851 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.4/CONTRIBUTING.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       89 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.4/HISTORY.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1072 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.4/LICENSE
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      262 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.4/MANIFEST.in
--rw-r--r--   0 gregor    (1000) gregor    (1000)     1941 2024-04-19 20:12:27.978002 gmaps_avoid_swiss-0.1.4/PKG-INFO
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      937 2024-04-19 18:35:36.000000 gmaps_avoid_swiss-0.1.4/README.rst
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 20:12:27.974002 gmaps_avoid_swiss-0.1.4/docs/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      618 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.4/docs/Makefile
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 20:12:27.974002 gmaps_avoid_swiss-0.1.4/docs/_build/
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 20:12:27.974002 gmaps_avoid_swiss-0.1.4/docs/_build/html/
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 20:12:27.974002 gmaps_avoid_swiss-0.1.4/docs/_build/html/_static/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      286 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.4/docs/_build/html/_static/file.png
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       90 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.4/docs/_build/html/_static/minus.png
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       90 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.4/docs/_build/html/_static/plus.png
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.4/docs/authors.rst
--rwxrwxr-x   0 gregor    (1000) gregor    (1000)     4943 2024-04-19 14:38:21.000000 gmaps_avoid_swiss-0.1.4/docs/conf.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       33 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.4/docs/contributing.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      559 2024-04-19 14:44:07.000000 gmaps_avoid_swiss-0.1.4/docs/gmaps_avoid_swiss.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.4/docs/history.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      321 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.4/docs/index.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1211 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.4/docs/installation.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      815 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.4/docs/make.bat
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       88 2024-04-19 14:44:07.000000 gmaps_avoid_swiss-0.1.4/docs/modules.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       27 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.4/docs/readme.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       96 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.4/docs/usage.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1391 2024-04-19 20:12:04.000000 gmaps_avoid_swiss-0.1.4/pyproject.toml
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       38 2024-04-19 20:12:27.978002 gmaps_avoid_swiss-0.1.4/setup.cfg
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      996 2024-04-19 20:12:04.000000 gmaps_avoid_swiss-0.1.4/setup.py
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 20:12:27.974002 gmaps_avoid_swiss-0.1.4/src/
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 20:12:27.974002 gmaps_avoid_swiss-0.1.4/src/gmaps_avoid_swiss/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      239 2024-04-19 20:12:04.000000 gmaps_avoid_swiss-0.1.4/src/gmaps_avoid_swiss/__init__.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      952 2024-04-19 19:55:33.000000 gmaps_avoid_swiss-0.1.4/src/gmaps_avoid_swiss/cli.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1821 2024-04-19 19:47:57.000000 gmaps_avoid_swiss-0.1.4/src/gmaps_avoid_swiss/client.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     2292 2024-04-19 18:32:52.000000 gmaps_avoid_swiss-0.1.4/src/gmaps_avoid_swiss/waypoints.py
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 20:12:27.978002 gmaps_avoid_swiss-0.1.4/src/gmaps_avoid_swiss.egg-info/
--rw-r--r--   0 gregor    (1000) gregor    (1000)     1941 2024-04-19 20:12:27.000000 gmaps_avoid_swiss-0.1.4/src/gmaps_avoid_swiss.egg-info/PKG-INFO
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      853 2024-04-19 20:12:27.000000 gmaps_avoid_swiss-0.1.4/src/gmaps_avoid_swiss.egg-info/SOURCES.txt
--rw-rw-r--   0 gregor    (1000) gregor    (1000)        1 2024-04-19 20:12:27.000000 gmaps_avoid_swiss-0.1.4/src/gmaps_avoid_swiss.egg-info/dependency_links.txt
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       64 2024-04-19 20:12:27.000000 gmaps_avoid_swiss-0.1.4/src/gmaps_avoid_swiss.egg-info/requires.txt
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       18 2024-04-19 20:12:27.000000 gmaps_avoid_swiss-0.1.4/src/gmaps_avoid_swiss.egg-info/top_level.txt
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 20:12:27.978002 gmaps_avoid_swiss-0.1.4/tests/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       47 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.4/tests/__init__.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      738 2024-04-19 20:08:33.000000 gmaps_avoid_swiss-0.1.4/tests/test_cli.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      915 2024-04-19 19:57:55.000000 gmaps_avoid_swiss-0.1.4/tests/test_gmaps_avoid_swiss.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1202 2024-04-19 19:57:47.000000 gmaps_avoid_swiss-0.1.4/tests/test_waypoints.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:28:16.026257 gmaps_avoid_swiss-0.1.5/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      162 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/AUTHORS.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     3851 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/CONTRIBUTING.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       89 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/HISTORY.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1072 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/LICENSE
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      262 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/MANIFEST.in
+-rw-r--r--   0 gregor    (1000) gregor    (1000)     2876 2024-04-21 03:28:16.026257 gmaps_avoid_swiss-0.1.5/PKG-INFO
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1845 2024-04-21 03:27:56.000000 gmaps_avoid_swiss-0.1.5/README.rst
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:28:16.026257 gmaps_avoid_swiss-0.1.5/docs/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      618 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/docs/Makefile
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/docs/authors.rst
+-rwxrwxr-x   0 gregor    (1000) gregor    (1000)     4934 2024-04-21 02:19:23.000000 gmaps_avoid_swiss-0.1.5/docs/conf.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       33 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/docs/contributing.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1152 2024-04-20 18:21:23.000000 gmaps_avoid_swiss-0.1.5/docs/geos.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      881 2024-04-21 02:16:02.000000 gmaps_avoid_swiss-0.1.5/docs/gmaps_avoid_swiss.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/docs/history.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      343 2024-04-21 02:19:08.000000 gmaps_avoid_swiss-0.1.5/docs/index.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1211 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/docs/installation.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      815 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/docs/make.bat
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       88 2024-04-21 02:16:02.000000 gmaps_avoid_swiss-0.1.5/docs/modules.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       27 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/docs/readme.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1237 2024-04-21 02:18:54.000000 gmaps_avoid_swiss-0.1.5/docs/usage.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1408 2024-04-21 03:20:40.000000 gmaps_avoid_swiss-0.1.5/pyproject.toml
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       38 2024-04-21 03:28:16.026257 gmaps_avoid_swiss-0.1.5/setup.cfg
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1023 2024-04-21 03:20:40.000000 gmaps_avoid_swiss-0.1.5/setup.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:28:16.022257 gmaps_avoid_swiss-0.1.5/src/
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:28:16.026257 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      307 2024-04-21 03:20:40.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss/__init__.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      674 2024-04-20 16:51:38.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss/client.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     4030 2024-04-21 02:11:49.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss/geo_check.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     7470 2024-04-21 02:11:04.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss/routes.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     2540 2024-04-20 16:57:41.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss/waypoints.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:28:16.026257 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss.egg-info/
+-rw-r--r--   0 gregor    (1000) gregor    (1000)     2876 2024-04-21 03:28:16.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss.egg-info/PKG-INFO
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      829 2024-04-21 03:28:16.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss.egg-info/SOURCES.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)        1 2024-04-21 03:28:16.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss.egg-info/dependency_links.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       76 2024-04-21 03:28:16.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss.egg-info/requires.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       18 2024-04-21 03:28:16.000000 gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss.egg-info/top_level.txt
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-21 03:28:16.026257 gmaps_avoid_swiss-0.1.5/tests/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       47 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.5/tests/__init__.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1383 2024-04-21 03:10:41.000000 gmaps_avoid_swiss-0.1.5/tests/test_geo_check.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1460 2024-04-21 03:00:26.000000 gmaps_avoid_swiss-0.1.5/tests/test_gmaps_avoid_swiss.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1550 2024-04-21 03:19:07.000000 gmaps_avoid_swiss-0.1.5/tests/test_routes.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1202 2024-04-19 19:57:47.000000 gmaps_avoid_swiss-0.1.5/tests/test_waypoints.py
```

### Comparing `gmaps_avoid_swiss-0.1.4/CONTRIBUTING.rst` & `gmaps_avoid_swiss-0.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.4/LICENSE` & `gmaps_avoid_swiss-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.4/PKG-INFO` & `gmaps_avoid_swiss-0.1.5/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: gmaps_avoid_swiss
-Version: 0.1.4
-Summary: A Python package that customizes Google Maps routing to avoid Swiss routes unless the origin, destination, or waypoints include locations within Switzerland.
-Home-page: https://github.com/xbencat/gmaps_avoid_swiss
-Author: Gregor Bencat
-Author-email: Gregor Bencat <bencat.gregor@gmail.com>
-Maintainer-email: Gregor Bencat <bencat.gregor@gmail.com>
-License: MIT license
-Project-URL: bugs, https://github.com/xbencat/gmaps_avoid_swiss/issues
-Project-URL: changelog, https://github.com/xbencat/gmaps_avoid_swiss/blob/master/changelog.md
-Project-URL: homepage, https://github.com/xbencat/gmaps_avoid_swiss
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-License-File: AUTHORS.rst
-Requires-Dist: google-maps-routing
-Requires-Dist: typer
-Requires-Dist: rich
-Provides-Extra: dev
-Requires-Dist: coverage; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-
 ========================
 GMaps Avoid Swiss Routes
 ========================
 
 
 .. image:: https://img.shields.io/pypi/v/gmaps_avoid_swiss.svg
         :target: https://pypi.python.org/pypi/gmaps_avoid_swiss
@@ -39,24 +15,38 @@
 
 A Python package that customizes Google Maps routing to avoid Swiss routes unless the origin, destination, or waypoints include locations within Switzerland.
 
 
 * Free software: MIT license
 * Documentation: https://gmaps-avoid-swiss.readthedocs.io.
 
-TODO
---------
 
-* variable fieldsets
-* avoid switz :D
+Dependencies
+____________
+
+This package requires the GEOS library as it utilizes Shapely for geographic operations.
+For installation instructions and more details, please refer to our GEOS for more details.
+
 
 Features
 --------
 
-* calculates duration, transit time and encoded path from origin to destination
+* Calculates duration, transit time, and encoded path from origin to destination
+* Avoids routing through Switzerland by dynamically selecting alternative cities
+  - If the initial route intersects with Switzerland, the system optimizes the route by selecting intermediate cities to avoid crossing Swiss borders
+  - The cities are prioritized based on their proximity to the intersection points with Switzerland
+  - The system iteratively tries different cities until a route that doesn't pass through Switzerland is found
+  - If no valid route is found after exhausting all city options, the system falls back to the original route
+* Right now its only possible to use address in format :code:`{"lat": 48.5734, "lng": 7.7521}`
+
+To-Do List
+----------
+
+* Add opting out of avoiding Swiss.
+* Improve Swiss route avoidance algorithms.
 
 Credits
 -------
 
 This package was created with Cookiecutter_ .
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
```

### Comparing `gmaps_avoid_swiss-0.1.4/docs/Makefile` & `gmaps_avoid_swiss-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.4/docs/conf.py` & `gmaps_avoid_swiss-0.1.5/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 release = gmaps_avoid_swiss.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -90,15 +90,15 @@
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = []
 
 # -- Options for HTMLHelp output ---------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = 'gmaps_avoid_swissdoc'
 
 # -- Options for LaTeX output ------------------------------------------
```

### Comparing `gmaps_avoid_swiss-0.1.4/docs/gmaps_avoid_swiss.rst` & `gmaps_avoid_swiss-0.1.5/docs/gmaps_avoid_swiss.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 gmaps\_avoid\_swiss package
 ===========================
 
 Submodules
 ----------
 
-gmaps\_avoid\_swiss.cli module
-------------------------------
+gmaps\_avoid\_swiss.client module
+---------------------------------
 
-.. automodule:: gmaps_avoid_swiss.cli
+.. automodule:: gmaps_avoid_swiss.client
    :members:
    :undoc-members:
    :show-inheritance:
 
-gmaps\_avoid\_swiss.gmaps\_avoid\_swiss module
-----------------------------------------------
+gmaps\_avoid\_swiss.geo\_check module
+-------------------------------------
 
-.. automodule:: gmaps_avoid_swiss.gmaps_avoid_swiss
+.. automodule:: gmaps_avoid_swiss.geo_check
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+gmaps\_avoid\_swiss.routes module
+---------------------------------
+
+.. automodule:: gmaps_avoid_swiss.routes
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+gmaps\_avoid\_swiss.waypoints module
+------------------------------------
+
+.. automodule:: gmaps_avoid_swiss.waypoints
    :members:
    :undoc-members:
    :show-inheritance:
 
 Module contents
 ---------------
```

### Comparing `gmaps_avoid_swiss-0.1.4/docs/installation.rst` & `gmaps_avoid_swiss-0.1.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.4/docs/make.bat` & `gmaps_avoid_swiss-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.4/pyproject.toml` & `gmaps_avoid_swiss-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gmaps_avoid_swiss"
-version = "0.1.4"
+version = "0.1.5"
 description = "A Python package that customizes Google Maps routing to avoid Swiss routes unless the origin, destination, or waypoints include locations within Switzerland."
 readme = "README.rst"
 authors = [
   {name = "Gregor Bencat", email = "bencat.gregor@gmail.com"}
 ]
 maintainers = [
   {name = "Gregor Bencat", email = "bencat.gregor@gmail.com"}
 ]
 classifiers = [
 
 ]
 license = {text = "MIT license"}
 dependencies = [
   "google-maps-routing",
-  "typer",
-  "rich"
+  "numpy",
+  "shapely",
+  "polyline"
 ]
 
 [project.optional-dependencies]
 dev = [
     "coverage",  # testing
     "mypy",  # linting
     "pytest",  # testing
```

### Comparing `gmaps_avoid_swiss-0.1.4/setup.py` & `gmaps_avoid_swiss-0.1.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gmaps_avoid_swiss',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     url='https://github.com/xbencat/gmaps_avoid_swiss',
     license='MIT',
     author='Gregor Bencat',
     author_email='bencat.gregor@gmail.com',
     description='A Python package that customizes Google Maps routing to avoid Swiss routes.',
     install_requires=[
-        'typer~=0.12.3',
-        'rich~=13.7.1',
         'google-maps-routing~=0.6.8',
+        'numpy~=1.21.2',
+        'shapely~=1.6.0',
+        'polyline~=1.4',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

### Comparing `gmaps_avoid_swiss-0.1.4/src/gmaps_avoid_swiss/waypoints.py` & `gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss/waypoints.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,72 +2,74 @@
 from google.type import latlng_pb2
 
 
 def create_waypoint(location_data: dict) -> Waypoint:
     """
     Create a Waypoint object from the provided location data.
 
-    Args:
-        location_data (dict): A dictionary containing location information.
-            It should have one of the following keys:
-            - 'lat' and 'lng' for latitude and longitude coordinates
-            - 'place_id' for a Google Maps place ID
-            - 'address' for a textual address
+    :param location_data: A dictionary containing location information. It should have one of the following keys:
+        - 'lat' and 'lng' for latitude and longitude coordinates
+        - 'place_id' for a Google Maps place ID
+        - 'address' for a textual address
+    :type location_data: dict
 
-    Returns:
-        Waypoint: A Waypoint object created from the location data.
+    :return: A Waypoint object created from the location data.
+    :rtype: Waypoint
 
-    Raises:
-        ValueError: If the provided location data is invalid.
+    :raises ValueError: If the provided location data is invalid.
     """
     if 'lat' in location_data and 'lng' in location_data:
         return _create_waypoint_from_coordinates(
             location_data['lat'], location_data['lng']
         )
-    elif 'place_id' in location_data:
-        return _create_waypoint_from_place_id(location_data['place_id'])
-    elif 'address' in location_data:
-        return _create_waypoint_from_address(location_data['address'])
     else:
-        raise ValueError("Invalid location data provided")
+        raise ValueError("Currently, only latitude and longitude coordinates are accepted. "
+                         "Please provide a dictionary with 'lat' and 'lng' keys.")
+    # elif 'place_id' in location_data:
+    #     return _create_waypoint_from_place_id(location_data['place_id'])
+    # elif 'address' in location_data:
+    #     return _create_waypoint_from_address(location_data['address'])
+    # else:
+    #     raise ValueError("Invalid location data provided")
 
 
 def _create_waypoint_from_coordinates(latitude: float, longitude: float) -> Waypoint:
     """
     Create a Waypoint object from latitude and longitude coordinates.
 
-    Args:
-        latitude (float): The latitude coordinate.
-        longitude (float): The longitude coordinate.
+    :param latitude: The latitude coordinate.
+    :type latitude: float
+    :param longitude: The longitude coordinate.
+    :type longitude: float
 
-    Returns:
-        Waypoint: A Waypoint object created from the coordinates.
+    :return: A Waypoint object created from the coordinates.
+    :rtype: Waypoint
     """
     lat_lng = latlng_pb2.LatLng(latitude=latitude, longitude=longitude)
     location = Location(lat_lng=lat_lng)
     return Waypoint(location=location)
 
 
 def _create_waypoint_from_place_id(place_id: str) -> Waypoint:
     """
     Create a Waypoint object from a Google Maps place ID.
 
-    Args:
-        place_id (str): The Google Maps place ID.
+    :param place_id: The Google Maps place ID.
+    :type place_id: str
 
-    Returns:
-        Waypoint: A Waypoint object created from the place ID.
+    :return: A Waypoint object created from the place ID.
+    :rtype: Waypoint
     """
     return Waypoint(place_id=place_id)
 
 
 def _create_waypoint_from_address(address: str) -> Waypoint:
     """
     Create a Waypoint object from a textual address.
 
-    Args:
-        address (str): The textual address.
+    :param address: The textual address.
+    :type address: str
 
-    Returns:
-        Waypoint: A Waypoint object created from the address.
+    :return: A Waypoint object created from the address.
+    :rtype: Waypoint
     """
     return Waypoint(address=address)
```

### Comparing `gmaps_avoid_swiss-0.1.4/src/gmaps_avoid_swiss.egg-info/SOURCES.txt` & `gmaps_avoid_swiss-0.1.5/src/gmaps_avoid_swiss.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 README.rst
 pyproject.toml
 setup.py
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
+docs/geos.rst
 docs/gmaps_avoid_swiss.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/modules.rst
 docs/readme.rst
 docs/usage.rst
-docs/_build/html/_static/file.png
-docs/_build/html/_static/minus.png
-docs/_build/html/_static/plus.png
 src/gmaps_avoid_swiss/__init__.py
-src/gmaps_avoid_swiss/cli.py
 src/gmaps_avoid_swiss/client.py
+src/gmaps_avoid_swiss/geo_check.py
+src/gmaps_avoid_swiss/routes.py
 src/gmaps_avoid_swiss/waypoints.py
 src/gmaps_avoid_swiss.egg-info/PKG-INFO
 src/gmaps_avoid_swiss.egg-info/SOURCES.txt
 src/gmaps_avoid_swiss.egg-info/dependency_links.txt
 src/gmaps_avoid_swiss.egg-info/requires.txt
 src/gmaps_avoid_swiss.egg-info/top_level.txt
 tests/__init__.py
-tests/test_cli.py
+tests/test_geo_check.py
 tests/test_gmaps_avoid_swiss.py
+tests/test_routes.py
 tests/test_waypoints.py
```

### Comparing `gmaps_avoid_swiss-0.1.4/tests/test_waypoints.py` & `gmaps_avoid_swiss-0.1.5/tests/test_waypoints.py`

 * *Files identical despite different names*


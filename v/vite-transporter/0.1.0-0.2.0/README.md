# Comparing `tmp/vite_transporter-0.1.0.tar.gz` & `tmp/vite_transporter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vite_transporter-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vite_transporter-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vite_transporter-0.1.0.tar` & `vite_transporter-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     5201 2024-04-17 20:37:21.973545 vite_transporter-0.1.0/.gitignore
--rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_transporter-0.1.0/LICENSE
--rw-r--r--   0        0        0     3777 2024-04-17 20:40:01.180549 vite_transporter-0.1.0/README.md
--rw-r--r--   0        0        0      433 2024-04-17 20:25:02.157672 vite_transporter-0.1.0/app_flask_demo/__init__.py
--rw-r--r--   0        0        0      192 2024-04-17 19:56:25.368755 vite_transporter-0.1.0/app_flask_demo/templates/index.html
--rw-r--r--   0        0        0    39139 2024-04-17 20:38:37.815908 vite_transporter-0.1.0/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif
--rw-r--r--   0        0        0    33329 2024-04-17 20:38:37.816282 vite_transporter-0.1.0/app_flask_demo/vt/app_vite_demo/index-621914e8.css
--rw-r--r--   0        0        0    20285 2024-04-17 20:38:37.816137 vite_transporter-0.1.0/app_flask_demo/vt/app_vite_demo/index-6e585489.js
--rw-r--r--   0        0        0      445 2024-04-17 20:20:47.520532 vite_transporter-0.1.0/app_quart_demo/__init__.py
--rw-r--r--   0        0        0      192 2024-04-17 19:56:29.985721 vite_transporter-0.1.0/app_quart_demo/templates/index.html
--rw-r--r--   0        0        0    39139 2024-04-17 19:55:40.663413 vite_transporter-0.1.0/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif
--rw-r--r--   0        0        0    33329 2024-04-17 19:55:40.663791 vite_transporter-0.1.0/app_quart_demo/vt/app_vite_demo/index-621914e8.css
--rw-r--r--   0        0        0    20285 2024-04-17 19:55:40.663651 vite_transporter-0.1.0/app_quart_demo/vt/app_vite_demo/index-6e585489.js
--rw-r--r--   0        0        0      376 2024-04-17 19:55:02.763791 vite_transporter-0.1.0/app_vite_demo/Index.jsx
--rw-r--r--   0        0        0      536 2024-04-12 20:35:46.642592 vite_transporter-0.1.0/app_vite_demo/__router__.jsx
--rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_transporter-0.1.0/app_vite_demo/assets/ili.gif
--rw-r--r--   0        0        0      480 2024-04-17 19:52:33.956385 vite_transporter-0.1.0/app_vite_demo/index.css
--rw-r--r--   0        0        0      414 2024-04-17 19:46:30.300521 vite_transporter-0.1.0/app_vite_demo/index.html
--rw-r--r--   0        0        0   105659 2024-04-17 18:51:11.871806 vite_transporter-0.1.0/app_vite_demo/package-lock.json
--rw-r--r--   0        0        0      570 2024-04-12 14:55:15.273422 vite_transporter-0.1.0/app_vite_demo/package.json
--rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_transporter-0.1.0/app_vite_demo/postcss.config.js
--rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_transporter-0.1.0/app_vite_demo/tailwind.config.js
--rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_transporter-0.1.0/app_vite_demo/vite.config.js
--rw-r--r--   0        0        0     1135 2024-04-17 19:56:57.458024 vite_transporter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       31 2024-04-17 20:14:50.246973 vite_transporter-0.1.0/requirements/demos.txt
--rw-r--r--   0        0        0       22 2024-04-17 20:14:46.286993 vite_transporter-0.1.0/requirements/development.txt
--rw-r--r--   0        0        0       34 2024-04-17 16:11:12.368549 vite_transporter-0.1.0/requirements/main.txt
--rw-r--r--   0        0        0     2185 2024-04-17 20:40:54.149610 vite_transporter-0.1.0/vite_transporter/__init__.py
--rw-r--r--   0        0        0     4871 2024-04-03 07:34:32.709087 vite_transporter-0.1.0/vite_transporter/_html_tags.py
--rw-r--r--   0        0        0     4002 2024-04-17 20:42:01.707392 vite_transporter-0.1.0/vite_transporter/helpers.py
--rw-r--r--   0        0        0      909 2024-04-17 15:48:32.502792 vite_transporter-0.1.0/vite_transporter/parser.py
--rw-r--r--   0        0        0        0 2024-04-17 15:35:45.579326 vite_transporter-0.1.0/vite_transporter/platform/__init__.py
--rw-r--r--   0        0        0     4593 2024-04-17 20:35:06.785393 vite_transporter-0.1.0/vite_transporter/platform/flask.py
--rw-r--r--   0        0        0     4671 2024-04-17 20:35:06.785401 vite_transporter-0.1.0/vite_transporter/platform/quart.py
--rw-r--r--   0        0        0     4459 1970-01-01 00:00:00.000000 vite_transporter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5201 2024-04-17 20:37:21.973545 vite_transporter-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_transporter-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3718 2024-04-21 15:35:16.830834 vite_transporter-0.2.0/README.md
+-rw-r--r--   0        0        0      738 2024-04-21 15:32:14.759993 vite_transporter-0.2.0/app_flask_demo/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-17 19:56:25.368755 vite_transporter-0.2.0/app_flask_demo/templates/index.html
+-rw-r--r--   0        0        0    39139 2024-04-17 20:38:37.815908 vite_transporter-0.2.0/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif
+-rw-r--r--   0        0        0    33329 2024-04-17 20:38:37.816282 vite_transporter-0.2.0/app_flask_demo/vt/app_vite_demo/index-621914e8.css
+-rw-r--r--   0        0        0    20285 2024-04-17 20:38:37.816137 vite_transporter-0.2.0/app_flask_demo/vt/app_vite_demo/index-6e585489.js
+-rw-r--r--   0        0        0      750 2024-04-21 15:32:40.857714 vite_transporter-0.2.0/app_quart_demo/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-17 19:56:29.985721 vite_transporter-0.2.0/app_quart_demo/templates/index.html
+-rw-r--r--   0        0        0    39139 2024-04-17 19:55:40.663413 vite_transporter-0.2.0/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif
+-rw-r--r--   0        0        0    33329 2024-04-17 19:55:40.663791 vite_transporter-0.2.0/app_quart_demo/vt/app_vite_demo/index-621914e8.css
+-rw-r--r--   0        0        0    20285 2024-04-17 19:55:40.663651 vite_transporter-0.2.0/app_quart_demo/vt/app_vite_demo/index-6e585489.js
+-rw-r--r--   0        0        0     2250 2024-04-21 15:33:39.440720 vite_transporter-0.2.0/app_vite_demo/Index.jsx
+-rw-r--r--   0        0        0      536 2024-04-12 20:35:46.642592 vite_transporter-0.2.0/app_vite_demo/__router__.jsx
+-rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_transporter-0.2.0/app_vite_demo/assets/ili.gif
+-rw-r--r--   0        0        0      596 2024-04-21 15:30:17.354196 vite_transporter-0.2.0/app_vite_demo/index.css
+-rw-r--r--   0        0        0      414 2024-04-17 19:46:30.300521 vite_transporter-0.2.0/app_vite_demo/index.html
+-rw-r--r--   0        0        0   105659 2024-04-17 18:51:11.871806 vite_transporter-0.2.0/app_vite_demo/package-lock.json
+-rw-r--r--   0        0        0      570 2024-04-12 14:55:15.273422 vite_transporter-0.2.0/app_vite_demo/package.json
+-rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_transporter-0.2.0/app_vite_demo/postcss.config.js
+-rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_transporter-0.2.0/app_vite_demo/tailwind.config.js
+-rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_transporter-0.2.0/app_vite_demo/vite.config.js
+-rw-r--r--   0        0        0     1257 2024-04-21 15:37:04.537415 vite_transporter-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-04-17 20:14:50.246973 vite_transporter-0.2.0/requirements/demos.txt
+-rw-r--r--   0        0        0       22 2024-04-17 20:14:46.286993 vite_transporter-0.2.0/requirements/development.txt
+-rw-r--r--   0        0        0       34 2024-04-17 16:11:12.368549 vite_transporter-0.2.0/requirements/main.txt
+-rw-r--r--   0        0        0     2185 2024-04-21 15:41:46.643269 vite_transporter-0.2.0/vite_transporter/__init__.py
+-rw-r--r--   0        0        0     2654 2024-04-21 13:26:49.370076 vite_transporter-0.2.0/vite_transporter/_headers.py
+-rw-r--r--   0        0        0     4871 2024-04-03 07:34:32.709087 vite_transporter-0.2.0/vite_transporter/_html_tags.py
+-rw-r--r--   0        0        0     4002 2024-04-17 20:42:01.707392 vite_transporter-0.2.0/vite_transporter/helpers.py
+-rw-r--r--   0        0        0      909 2024-04-17 15:48:32.502792 vite_transporter-0.2.0/vite_transporter/parser.py
+-rw-r--r--   0        0        0        0 2024-04-17 15:35:45.579326 vite_transporter-0.2.0/vite_transporter/platform/__init__.py
+-rw-r--r--   0        0        0     4555 2024-04-21 15:40:31.645154 vite_transporter-0.2.0/vite_transporter/platform/flask.py
+-rw-r--r--   0        0        0     4629 2024-04-21 15:43:46.126181 vite_transporter-0.2.0/vite_transporter/platform/quart.py
+-rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 vite_transporter-0.2.0/PKG-INFO
```

### Comparing `vite_transporter-0.1.0/.gitignore` & `vite_transporter-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.1.0/LICENSE` & `vite_transporter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.1.0/README.md` & `vite_transporter-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 `pyproject.toml`:
 
 ```toml
 [tool.vite_transporter]
 npm_exec = "npm"
 npx_exec = "npx"
 serve_app = "app_flask_demo"
-vite_app_dirs = ["app_vite_demo"]
+vite_apps = ["app_vite_demo"]
 ```
 
 The compiling of the Vite apps requires the `npx` and `npm` to be
 available. You can use absolute paths here.
 
 `npm_exec` is used to run `npm install` if your Vite app does not
 have the `node_modules` folder.
@@ -138,21 +138,20 @@
 ```
 
 ### CORS
 
 Setting:
 
 ```python
-ViteTransporter(app, cors_allow_all=True)
+ViteTransporter(app, cors_allowed_hosts=["http://127.0.0.1:5003"])
 ```
 
-or setting the environment variable
-`VT_CORS_ALLOW_ALL=True` will allow all origins to access the serving app.
+This is to allow the Vite app to communicate with the app.
 
-This is to allow the Vite app to communicate with the Flask app during development.
+**Note:** It's recommended to remove this in production.
 
 ## Running the demos
 
 We will be using a package call `pyqwe` to run commands from the pyproject file.
 Installing the development requirements will install `pyqwe`:
 
 ```bash
@@ -181,9 +180,9 @@
 
 Visit the vite app from the link in the terminal. Change something, save, then in terminal 3 run:
 
 ```bash
 vt compile
 ```
 
-The Vite app will be compiled, and the files will be moved to the Flask app. 
+The Vite app will be compiled, and the files will be moved to the Flask app.
 Visiting the Flask app from the link in terminal 1 should show the changes.
```

### Comparing `vite_transporter-0.1.0/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif` & `vite_transporter-0.2.0/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.1.0/app_flask_demo/vt/app_vite_demo/index-621914e8.css` & `vite_transporter-0.2.0/app_flask_demo/vt/app_vite_demo/index-621914e8.css`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.1.0/app_flask_demo/vt/app_vite_demo/index-6e585489.js` & `vite_transporter-0.2.0/app_flask_demo/vt/app_vite_demo/index-6e585489.js`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.1.0/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif` & `vite_transporter-0.2.0/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.1.0/app_quart_demo/vt/app_vite_demo/index-621914e8.css` & `vite_transporter-0.2.0/app_quart_demo/vt/app_vite_demo/index-621914e8.css`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.1.0/app_quart_demo/vt/app_vite_demo/index-6e585489.js` & `vite_transporter-0.2.0/app_quart_demo/vt/app_vite_demo/index-6e585489.js`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.1.0/app_vite_demo/__router__.jsx` & `vite_transporter-0.2.0/app_vite_demo/__router__.jsx`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.1.0/app_vite_demo/assets/ili.gif` & `vite_transporter-0.2.0/app_vite_demo/assets/ili.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.1.0/app_vite_demo/package-lock.json` & `vite_transporter-0.2.0/app_vite_demo/package-lock.json`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.1.0/app_vite_demo/package.json` & `vite_transporter-0.2.0/app_vite_demo/package.json`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.1.0/pyproject.toml` & `vite_transporter-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 flask = ["flask"]
 quart = ["quart"]
 
 [project.scripts]
 vt = "vite_transporter:_cli"
 
 [tool.pyqwe]
-vite = "*(app_vite_demo):npm start"
-flask = "app_flask_demo:run"
-quart = "app_quart_demo:run"
+vite = "*(app_vite_demo):npx vite --host 127.0.0.1 --port 5003"
+flask = "*:flask --app app_flask_demo run --host 127.0.0.1 --port 5001 --debug"
+quart = "*:quart --app app_quart_demo run --host 127.0.0.1 --port 5002"
 install = "*:flit install --symlink"
 build = "*:flit build"
 publish = "*shell:export FLIT_USERNAME=__token__ && flit publish"
 
 [tool.vite_transporter]
 npm_exec = "npm"
 npx_exec = "npx"
```

### Comparing `vite_transporter-0.1.0/vite_transporter/__init__.py` & `vite_transporter-0.2.0/vite_transporter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 
 from .helpers import Colr as _Colr
 from .helpers import PyProjectConfig as _PyProjectConfig
 from .helpers import _compile
 from .parser import ArgumentParser as _ArgumentParser
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 
 def _cli():
     pars = _ArgumentParser(prog="vtf", add_help=False)
     pars.add_argument(
         "--version", "-v", action="version", version=f"vite-to-flask {__version__}"
     )
```

### Comparing `vite_transporter-0.1.0/vite_transporter/_html_tags.py` & `vite_transporter-0.2.0/vite_transporter/_html_tags.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.1.0/vite_transporter/helpers.py` & `vite_transporter-0.2.0/vite_transporter/helpers.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.1.0/vite_transporter/parser.py` & `vite_transporter-0.2.0/vite_transporter/parser.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.1.0/PKG-INFO` & `vite_transporter-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vite-transporter
-Version: 0.1.0
+Version: 0.2.0
 Summary: Transport Vite apps.
 Author-email: David Carmichael <david@uilix.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -42,15 +42,15 @@
 `pyproject.toml`:
 
 ```toml
 [tool.vite_transporter]
 npm_exec = "npm"
 npx_exec = "npx"
 serve_app = "app_flask_demo"
-vite_app_dirs = ["app_vite_demo"]
+vite_apps = ["app_vite_demo"]
 ```
 
 The compiling of the Vite apps requires the `npx` and `npm` to be
 available. You can use absolute paths here.
 
 `npm_exec` is used to run `npm install` if your Vite app does not
 have the `node_modules` folder.
@@ -157,21 +157,20 @@
 ```
 
 ### CORS
 
 Setting:
 
 ```python
-ViteTransporter(app, cors_allow_all=True)
+ViteTransporter(app, cors_allowed_hosts=["http://127.0.0.1:5003"])
 ```
 
-or setting the environment variable
-`VT_CORS_ALLOW_ALL=True` will allow all origins to access the serving app.
+This is to allow the Vite app to communicate with the app.
 
-This is to allow the Vite app to communicate with the Flask app during development.
+**Note:** It's recommended to remove this in production.
 
 ## Running the demos
 
 We will be using a package call `pyqwe` to run commands from the pyproject file.
 Installing the development requirements will install `pyqwe`:
 
 ```bash
@@ -200,9 +199,9 @@
 
 Visit the vite app from the link in the terminal. Change something, save, then in terminal 3 run:
 
 ```bash
 vt compile
 ```
 
-The Vite app will be compiled, and the files will be moved to the Flask app. 
+The Vite app will be compiled, and the files will be moved to the Flask app.
 Visiting the Flask app from the link in terminal 1 should show the changes.
```


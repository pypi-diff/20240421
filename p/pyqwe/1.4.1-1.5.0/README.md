# Comparing `tmp/pyqwe-1.4.1.tar.gz` & `tmp/pyqwe-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqwe-1.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyqwe-1.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyqwe-1.4.1.tar` & `pyqwe-1.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       28 2024-03-30 13:38:11.669595 pyqwe-1.4.1/.env.example
--rw-r--r--   0        0        0     1180 2024-04-13 12:33:51.476960 pyqwe-1.4.1/.gitignore
--rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 pyqwe-1.4.1/LICENSE
--rw-r--r--   0        0        0     3010 2024-04-03 09:00:07.846648 pyqwe-1.4.1/README.md
--rw-r--r--   0        0        0      204 2024-03-29 08:35:21.325325 pyqwe-1.4.1/flask_example/module.py
--rw-r--r--   0        0        0      204 2024-03-29 08:42:03.877337 pyqwe-1.4.1/flask_example/package/__init__.py
--rw-r--r--   0        0        0      935 2024-04-13 12:34:23.232337 pyqwe-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     1823 2024-04-13 12:50:40.009890 pyqwe-1.4.1/pyqwe/__init__.py
--rw-r--r--   0        0        0      179 2024-03-30 13:38:11.670188 pyqwe-1.4.1/pyqwe/exceptions.py
--rw-r--r--   0        0        0     3859 2024-04-13 12:49:21.255346 pyqwe-1.4.1/pyqwe/helpers.py
--rw-r--r--   0        0        0      743 2024-04-13 12:49:21.255375 pyqwe-1.4.1/pyqwe/parser.py
--rw-r--r--   0        0        0     3413 1970-01-01 00:00:00.000000 pyqwe-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0       28 2024-03-30 13:38:11.669595 pyqwe-1.5.0/.env.example
+-rw-r--r--   0        0        0     1180 2024-04-13 12:33:51.476960 pyqwe-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 pyqwe-1.5.0/LICENSE
+-rw-r--r--   0        0        0     3010 2024-04-03 09:00:07.846648 pyqwe-1.5.0/README.md
+-rw-r--r--   0        0        0      204 2024-03-29 08:35:21.325325 pyqwe-1.5.0/flask_example/module.py
+-rw-r--r--   0        0        0      204 2024-03-29 08:42:03.877337 pyqwe-1.5.0/flask_example/package/__init__.py
+-rw-r--r--   0        0        0      935 2024-04-13 12:34:23.232337 pyqwe-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1931 2024-04-21 14:13:49.905204 pyqwe-1.5.0/pyqwe/__init__.py
+-rw-r--r--   0        0        0      179 2024-03-30 13:38:11.670188 pyqwe-1.5.0/pyqwe/exceptions.py
+-rw-r--r--   0        0        0     3859 2024-04-13 12:49:21.255346 pyqwe-1.5.0/pyqwe/helpers.py
+-rw-r--r--   0        0        0      743 2024-04-13 12:49:21.255375 pyqwe-1.5.0/pyqwe/parser.py
+-rw-r--r--   0        0        0     3413 1970-01-01 00:00:00.000000 pyqwe-1.5.0/PKG-INFO
```

### Comparing `pyqwe-1.4.1/.gitignore` & `pyqwe-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqwe-1.4.1/LICENSE` & `pyqwe-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqwe-1.4.1/README.md` & `pyqwe-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyqwe-1.4.1/pyproject.toml` & `pyqwe-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyqwe-1.4.1/pyqwe/__init__.py` & `pyqwe-1.5.0/pyqwe/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     import tomllib
 except ImportError:
     try:
         import toml as tomllib
     except ImportError:
         raise ImportError("pyqwe requires toml, install it with 'pip install toml'")
 
-__version__ = "1.4.1"
+__version__ = "1.5.0"
 
 _cwd = Path().cwd()
 _pyproject_file = _cwd / "pyproject.toml"
 
 if not _pyproject_file.exists():
     raise FileNotFoundError("pyproject.toml not found")
 
@@ -54,11 +54,16 @@
                     f"{Colr.BOLD}=>{Colr.END} "
                     f"{Colr.HEADER}{option[1]}{Colr.END}"
                 )
         print("")
         sys.exit(0)
 
     try:
-        _run(*_split_runner(args.runner), _cwd=_cwd)
-    except AttributeError as e:
-        _ = e
+        _runner = args.runner
+    except AttributeError:
         pars.print_help()
+        sys.exit(0)
+
+    try:
+        _run(*_split_runner(_runner), _cwd=_cwd)
+    except Exception as e:
+        print(f" {Colr.FAIL}{e}{Colr.END}")
```

### Comparing `pyqwe-1.4.1/pyqwe/helpers.py` & `pyqwe-1.5.0/pyqwe/helpers.py`

 * *Files identical despite different names*

### Comparing `pyqwe-1.4.1/pyqwe/parser.py` & `pyqwe-1.5.0/pyqwe/parser.py`

 * *Files identical despite different names*

### Comparing `pyqwe-1.4.1/PKG-INFO` & `pyqwe-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqwe
-Version: 1.4.1
+Version: 1.5.0
 Summary: Run commands set in the pyproject.toml file
 Author-email: David Carmichael <david@uilix.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pyqwe-extra-dotenv ; extra == "dotenv"
 Project-URL: Source, https://github.com/CheeseCake87/pyqwe
```


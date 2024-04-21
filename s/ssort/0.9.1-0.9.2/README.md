# Comparing `tmp/ssort-0.9.1.tar.gz` & `tmp/ssort-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ssort-0.9.1.tar", last modified: Tue Feb  1 11:10:58 2022, max compression
+gzip compressed data, was "dist/ssort-0.9.2.tar", last modified: Thu Mar 24 17:45:35 2022, max compression
```

## Comparing `ssort-0.9.1.tar` & `ssort-0.9.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-01 11:10:58.000000 ssort-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1080 2022-02-01 11:10:57.000000 ssort-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     4748 2022-02-01 11:10:58.000000 ssort-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3119 2022-02-01 11:10:57.000000 ssort-0.9.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)      101 2022-02-01 11:10:57.000000 ssort-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2022-02-01 11:10:58.000000 ssort-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      136 2022-02-01 11:10:57.000000 ssort-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-01 11:10:58.000000 ssort-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-01 11:10:58.000000 ssort-0.9.1/src/ssort/
--rw-r--r--   0 runner    (1001) docker     (116)      273 2022-02-01 11:10:57.000000 ssort-0.9.1/src/ssort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       37 2022-02-01 11:10:57.000000 ssort-0.9.1/src/ssort/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)    17537 2022-02-01 11:10:57.000000 ssort-0.9.1/src/ssort/_bindings.py
--rw-r--r--   0 runner    (1001) docker     (116)     3011 2022-02-01 11:10:57.000000 ssort-0.9.1/src/ssort/_builtins.py
--rw-r--r--   0 runner    (1001) docker     (116)     3224 2022-02-01 11:10:57.000000 ssort-0.9.1/src/ssort/_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (116)      145 2022-02-01 11:10:57.000000 ssort-0.9.1/src/ssort/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     4629 2022-02-01 11:10:57.000000 ssort-0.9.1/src/ssort/_graphs.py
--rw-r--r--   0 runner    (1001) docker     (116)     4066 2022-02-01 11:10:57.000000 ssort-0.9.1/src/ssort/_main.py
--rw-r--r--   0 runner    (1001) docker     (116)    18590 2022-02-01 11:10:57.000000 ssort-0.9.1/src/ssort/_method_requirements.py
--rw-r--r--   0 runner    (1001) docker     (116)     6381 2022-02-01 11:10:57.000000 ssort-0.9.1/src/ssort/_parsing.py
--rw-r--r--   0 runner    (1001) docker     (116)    18574 2022-02-01 11:10:57.000000 ssort-0.9.1/src/ssort/_requirements.py
--rw-r--r--   0 runner    (1001) docker     (116)     7742 2022-02-01 11:10:57.000000 ssort-0.9.1/src/ssort/_ssort.py
--rw-r--r--   0 runner    (1001) docker     (116)     1496 2022-02-01 11:10:57.000000 ssort-0.9.1/src/ssort/_statements.py
--rw-r--r--   0 runner    (1001) docker     (116)     1239 2022-02-01 11:10:57.000000 ssort-0.9.1/src/ssort/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-01 11:10:58.000000 ssort-0.9.1/src/ssort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4748 2022-02-01 11:10:58.000000 ssort-0.9.1/src/ssort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      550 2022-02-01 11:10:58.000000 ssort-0.9.1/src/ssort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-01 11:10:58.000000 ssort-0.9.1/src/ssort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       44 2022-02-01 11:10:58.000000 ssort-0.9.1/src/ssort.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2022-02-01 11:10:58.000000 ssort-0.9.1/src/ssort.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-24 17:45:35.000000 ssort-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (116)     1080 2022-03-24 17:45:34.000000 ssort-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)     4748 2022-03-24 17:45:35.000000 ssort-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3119 2022-03-24 17:45:34.000000 ssort-0.9.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      101 2022-03-24 17:45:34.000000 ssort-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)     1064 2022-03-24 17:45:35.000000 ssort-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      136 2022-03-24 17:45:34.000000 ssort-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-24 17:45:35.000000 ssort-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-24 17:45:35.000000 ssort-0.9.2/src/ssort/
+-rw-r--r--   0 runner    (1001) docker     (116)      273 2022-03-24 17:45:34.000000 ssort-0.9.2/src/ssort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       37 2022-03-24 17:45:34.000000 ssort-0.9.2/src/ssort/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17537 2022-03-24 17:45:34.000000 ssort-0.9.2/src/ssort/_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3011 2022-03-24 17:45:34.000000 ssort-0.9.2/src/ssort/_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3224 2022-03-24 17:45:34.000000 ssort-0.9.2/src/ssort/_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (116)      145 2022-03-24 17:45:34.000000 ssort-0.9.2/src/ssort/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4629 2022-03-24 17:45:34.000000 ssort-0.9.2/src/ssort/_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4066 2022-03-24 17:45:34.000000 ssort-0.9.2/src/ssort/_main.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18590 2022-03-24 17:45:34.000000 ssort-0.9.2/src/ssort/_method_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6381 2022-03-24 17:45:34.000000 ssort-0.9.2/src/ssort/_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18574 2022-03-24 17:45:34.000000 ssort-0.9.2/src/ssort/_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7786 2022-03-24 17:45:34.000000 ssort-0.9.2/src/ssort/_ssort.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1496 2022-03-24 17:45:34.000000 ssort-0.9.2/src/ssort/_statements.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1239 2022-03-24 17:45:34.000000 ssort-0.9.2/src/ssort/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-24 17:45:35.000000 ssort-0.9.2/src/ssort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     4748 2022-03-24 17:45:35.000000 ssort-0.9.2/src/ssort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      550 2022-03-24 17:45:35.000000 ssort-0.9.2/src/ssort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-03-24 17:45:35.000000 ssort-0.9.2/src/ssort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       44 2022-03-24 17:45:35.000000 ssort-0.9.2/src/ssort.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2022-03-24 17:45:35.000000 ssort-0.9.2/src/ssort.egg-info/top_level.txt
```

### Comparing `ssort-0.9.1/LICENSE` & `ssort-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ssort-0.9.1/PKG-INFO` & `ssort-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ssort
-Version: 0.9.1
+Version: 0.9.2
 Summary: The python statement sorter
 Home-page: https://github.com/bwhmather/ssort
 Author: Ben Mather
 Author-email: bwhmather@bwhmather.com
 Maintainer: Ben Mather
 Maintainer-email: bwhmather@bwhmather.com
 License: MIT
```

### Comparing `ssort-0.9.1/README.rst` & `ssort-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `ssort-0.9.1/setup.cfg` & `ssort-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ssort-0.9.1/src/ssort/_bindings.py` & `ssort-0.9.2/src/ssort/_bindings.py`

 * *Files identical despite different names*

### Comparing `ssort-0.9.1/src/ssort/_builtins.py` & `ssort-0.9.2/src/ssort/_builtins.py`

 * *Files identical despite different names*

### Comparing `ssort-0.9.1/src/ssort/_dependencies.py` & `ssort-0.9.2/src/ssort/_dependencies.py`

 * *Files identical despite different names*

### Comparing `ssort-0.9.1/src/ssort/_graphs.py` & `ssort-0.9.2/src/ssort/_graphs.py`

 * *Files identical despite different names*

### Comparing `ssort-0.9.1/src/ssort/_main.py` & `ssort-0.9.2/src/ssort/_main.py`

 * *Files identical despite different names*

### Comparing `ssort-0.9.1/src/ssort/_method_requirements.py` & `ssort-0.9.2/src/ssort/_method_requirements.py`

 * *Files identical despite different names*

### Comparing `ssort-0.9.1/src/ssort/_parsing.py` & `ssort-0.9.2/src/ssort/_parsing.py`

 * *Files identical despite different names*

### Comparing `ssort-0.9.1/src/ssort/_requirements.py` & `ssort-0.9.2/src/ssort/_requirements.py`

 * *Files identical despite different names*

### Comparing `ssort-0.9.1/src/ssort/_ssort.py` & `ssort-0.9.2/src/ssort/_ssort.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,14 +318,17 @@
         return _statement_text_sorted_class(statement)
     return statement_text(statement)
 
 
 def ssort(text, *, filename="<unknown>"):
     statements = list(split(text, filename=filename))
 
+    if not statements:
+        return text
+
     graph = statements_graph(statements)
 
     replace_cycles(graph, key=sort_key_from_iter(statements))
 
     sorted_statements = topological_sort(statements, graph=graph)
 
     assert is_topologically_sorted(sorted_statements, graph=graph)
```

### Comparing `ssort-0.9.1/src/ssort/_statements.py` & `ssort-0.9.2/src/ssort/_statements.py`

 * *Files identical despite different names*

### Comparing `ssort-0.9.1/src/ssort/_utils.py` & `ssort-0.9.2/src/ssort/_utils.py`

 * *Files identical despite different names*

### Comparing `ssort-0.9.1/src/ssort.egg-info/PKG-INFO` & `ssort-0.9.2/src/ssort.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ssort
-Version: 0.9.1
+Version: 0.9.2
 Summary: The python statement sorter
 Home-page: https://github.com/bwhmather/ssort
 Author: Ben Mather
 Author-email: bwhmather@bwhmather.com
 Maintainer: Ben Mather
 Maintainer-email: bwhmather@bwhmather.com
 License: MIT
```

### Comparing `ssort-0.9.1/src/ssort.egg-info/SOURCES.txt` & `ssort-0.9.2/src/ssort.egg-info/SOURCES.txt`

 * *Files identical despite different names*


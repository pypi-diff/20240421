# Comparing `tmp/standard_xdrlib-3.11.9.tar.gz` & `tmp/standard_xdrlib-3.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_xdrlib-3.11.9.tar", last modified: Sun Apr 21 19:05:35 2024, max compression
+gzip compressed data, was "standard_xdrlib-3.12.2.tar", last modified: Sun Apr 21 19:21:41 2024, max compression
```

## Comparing `standard_xdrlib-3.11.9.tar` & `standard_xdrlib-3.12.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:35.986034 standard_xdrlib-3.11.9/
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_xdrlib-3.11.9/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     3808 2024-04-21 19:05:35.985779 standard_xdrlib-3.11.9/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_xdrlib-3.11.9/README.rst
--rw-r--r--   0 user       (501) staff       (20)      708 2024-04-21 19:00:02.000000 standard_xdrlib-3.11.9/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 19:05:35.986081 standard_xdrlib-3.11.9/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:35.985565 standard_xdrlib-3.11.9/standard_xdrlib.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3808 2024-04-21 19:05:35.000000 standard_xdrlib-3.11.9/standard_xdrlib.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      229 2024-04-21 19:05:35.000000 standard_xdrlib-3.11.9/standard_xdrlib.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 19:05:35.000000 standard_xdrlib-3.11.9/standard_xdrlib.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        7 2024-04-21 19:05:35.000000 standard_xdrlib-3.11.9/standard_xdrlib.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:35.985215 standard_xdrlib-3.11.9/tests/
--rw-r--r--   0 user       (501) staff       (20)     2307 2024-04-21 19:00:02.000000 standard_xdrlib-3.11.9/tests/test_xdrlib.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:35.985339 standard_xdrlib-3.11.9/xdrlib/
--rw-r--r--   0 user       (501) staff       (20)     5977 2024-04-21 19:00:02.000000 standard_xdrlib-3.11.9/xdrlib/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:21:41.771215 standard_xdrlib-3.12.2/
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_xdrlib-3.12.2/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     3808 2024-04-21 19:21:41.770985 standard_xdrlib-3.12.2/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_xdrlib-3.12.2/README.rst
+-rw-r--r--   0 user       (501) staff       (20)      708 2024-04-21 19:19:59.000000 standard_xdrlib-3.12.2/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 19:21:41.771257 standard_xdrlib-3.12.2/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:21:41.770775 standard_xdrlib-3.12.2/standard_xdrlib.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3808 2024-04-21 19:21:41.000000 standard_xdrlib-3.12.2/standard_xdrlib.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      229 2024-04-21 19:21:41.000000 standard_xdrlib-3.12.2/standard_xdrlib.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 19:21:41.000000 standard_xdrlib-3.12.2/standard_xdrlib.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        7 2024-04-21 19:21:41.000000 standard_xdrlib-3.12.2/standard_xdrlib.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:21:41.770407 standard_xdrlib-3.12.2/tests/
+-rw-r--r--   0 user       (501) staff       (20)     2307 2024-04-21 19:19:59.000000 standard_xdrlib-3.12.2/tests/test_xdrlib.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:21:41.770533 standard_xdrlib-3.12.2/xdrlib/
+-rw-r--r--   0 user       (501) staff       (20)     5942 2024-04-21 19:19:59.000000 standard_xdrlib-3.12.2/xdrlib/__init__.py
```

### Comparing `standard_xdrlib-3.11.9/LICENSE` & `standard_xdrlib-3.12.2/LICENSE`

 * *Files identical despite different names*

### Comparing `standard_xdrlib-3.11.9/PKG-INFO` & `standard_xdrlib-3.12.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-xdrlib
-Version: 3.11.9
+Version: 3.12.2
 Summary: Standard library xdrlib redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_xdrlib-3.11.9/pyproject.toml` & `standard_xdrlib-3.12.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "standard-xdrlib"
-version = "3.11.9"
+version = "3.12.2"
 description = "Standard library xdrlib redistribution. \"dead battery\"."
 keywords = ["stdlib"]
 authors = [
     { name = "Python Devleopers", email = "python-deadlib@youknowone.org" }
 ]
 readme = "README.rst"
 license = {name = "PSF", file = "LICENSE"}
```

### Comparing `standard_xdrlib-3.11.9/standard_xdrlib.egg-info/PKG-INFO` & `standard_xdrlib-3.12.2/standard_xdrlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-xdrlib
-Version: 3.11.9
+Version: 3.12.2
 Summary: Standard library xdrlib redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_xdrlib-3.11.9/tests/test_xdrlib.py` & `standard_xdrlib-3.12.2/tests/test_xdrlib.py`

 * *Files identical despite different names*

### Comparing `standard_xdrlib-3.11.9/xdrlib/__init__.py` & `standard_xdrlib-3.12.2/xdrlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,17 +220,15 @@
         return self.unpack_fstring(n)
 
     unpack_opaque = unpack_string
     unpack_bytes = unpack_string
 
     def unpack_list(self, unpack_item):
         list = []
-        while 1:
-            x = self.unpack_uint()
-            if x == 0: break
+        while (x := self.unpack_uint()) != 0:
             if x != 1:
                 raise ConversionError('0 or 1 expected, got %r' % (x,))
             item = unpack_item()
             list.append(item)
         return list
 
     def unpack_farray(self, n, unpack_item):
```


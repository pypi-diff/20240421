# Comparing `tmp/standard_cgitb-3.10.14.tar.gz` & `tmp/standard_cgitb-3.11.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_cgitb-3.10.14.tar", last modified: Sun Apr 21 18:51:22 2024, max compression
+gzip compressed data, was "standard_cgitb-3.11.9.tar", last modified: Sun Apr 21 19:04:42 2024, max compression
```

## Comparing `standard_cgitb-3.10.14.tar` & `standard_cgitb-3.11.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:22.305303 standard_cgitb-3.10.14/
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_cgitb-3.10.14/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     3807 2024-04-21 18:51:22.305087 standard_cgitb-3.10.14/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_cgitb-3.10.14/README.rst
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:22.304140 standard_cgitb-3.10.14/cgitb/
--rw-r--r--   0 user       (501) staff       (20)    12096 2024-04-21 18:45:39.000000 standard_cgitb-3.10.14/cgitb/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      706 2024-04-21 18:45:39.000000 standard_cgitb-3.10.14/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 18:51:22.305343 standard_cgitb-3.10.14/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:22.304920 standard_cgitb-3.10.14/standard_cgitb.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3807 2024-04-21 18:51:22.000000 standard_cgitb-3.10.14/standard_cgitb.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      223 2024-04-21 18:51:22.000000 standard_cgitb-3.10.14/standard_cgitb.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 18:51:22.000000 standard_cgitb-3.10.14/standard_cgitb.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        6 2024-04-21 18:51:22.000000 standard_cgitb-3.10.14/standard_cgitb.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:22.304766 standard_cgitb-3.10.14/tests/
--rw-r--r--   0 user       (501) staff       (20)     2602 2024-04-21 18:45:39.000000 standard_cgitb-3.10.14/tests/test_cgitb.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:42.331047 standard_cgitb-3.11.9/
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_cgitb-3.11.9/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     3806 2024-04-21 19:04:42.330799 standard_cgitb-3.11.9/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_cgitb-3.11.9/README.rst
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:42.329652 standard_cgitb-3.11.9/cgitb/
+-rw-r--r--   0 user       (501) staff       (20)    12421 2024-04-21 19:00:01.000000 standard_cgitb-3.11.9/cgitb/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      705 2024-04-21 19:00:01.000000 standard_cgitb-3.11.9/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 19:04:42.331093 standard_cgitb-3.11.9/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:42.330598 standard_cgitb-3.11.9/standard_cgitb.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3806 2024-04-21 19:04:42.000000 standard_cgitb-3.11.9/standard_cgitb.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      223 2024-04-21 19:04:42.000000 standard_cgitb-3.11.9/standard_cgitb.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 19:04:42.000000 standard_cgitb-3.11.9/standard_cgitb.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        6 2024-04-21 19:04:42.000000 standard_cgitb-3.11.9/standard_cgitb.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:42.330413 standard_cgitb-3.11.9/tests/
+-rw-r--r--   0 user       (501) staff       (20)     2683 2024-04-21 19:00:01.000000 standard_cgitb-3.11.9/tests/test_cgitb.py
```

### Comparing `standard_cgitb-3.10.14/LICENSE` & `standard_cgitb-3.11.9/LICENSE`

 * *Files identical despite different names*

### Comparing `standard_cgitb-3.10.14/PKG-INFO` & `standard_cgitb-3.11.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-cgitb
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library cgitb redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_cgitb-3.10.14/cgitb/__init__.py` & `standard_cgitb-3.11.9/cgitb/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 import os
 import pydoc
 import sys
 import tempfile
 import time
 import tokenize
 import traceback
+import warnings
+from html import escape as html_escape
+
+warnings._deprecated(__name__, remove=(3, 13))
+
 
 def reset():
     """Return a string that resets the CGI and browser to a known state."""
     return '''<!--: spam
 Content-Type: text/html
 
 <body bgcolor="#f0f0f8"><font color="#f0f0f8" size="-5"> -->
@@ -101,18 +106,24 @@
 def html(einfo, context=5):
     """Return a nice HTML document describing a given traceback."""
     etype, evalue, etb = einfo
     if isinstance(etype, type):
         etype = etype.__name__
     pyver = 'Python ' + sys.version.split()[0] + ': ' + sys.executable
     date = time.ctime(time.time())
-    head = '<body bgcolor="#f0f0f8">' + pydoc.html.heading(
-        '<big><big>%s</big></big>' %
-        strong(pydoc.html.escape(str(etype))),
-        '#ffffff', '#6622aa', pyver + '<br>' + date) + '''
+    head = f'''
+<body bgcolor="#f0f0f8">
+<table width="100%" cellspacing=0 cellpadding=2 border=0 summary="heading">
+<tr bgcolor="#6622aa">
+<td valign=bottom>&nbsp;<br>
+<font color="#ffffff" face="helvetica, arial">&nbsp;<br>
+<big><big><strong>{html_escape(str(etype))}</strong></big></big></font></td>
+<td align=right valign=bottom>
+<font color="#ffffff" face="helvetica, arial">{pyver}<br>{date}</font></td>
+</tr></table>
 <p>A problem occurred in a Python script.  Here is the sequence of
 function calls leading up to the error, in the order they occurred.</p>'''
 
     indent = '<tt>' + small('&nbsp;' * 5) + '&nbsp;</tt>'
     frames = []
     records = inspect.getinnerframes(etb, context)
     for frame, file, lnum, func, lines, index in records:
```

### Comparing `standard_cgitb-3.10.14/pyproject.toml` & `standard_cgitb-3.11.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "standard-cgitb"
-version = "3.10.14"
+version = "3.11.9"
 description = "Standard library cgitb redistribution. \"dead battery\"."
 keywords = ["stdlib"]
 authors = [
     { name = "Python Devleopers", email = "python-deadlib@youknowone.org" }
 ]
 readme = "README.rst"
 license = {name = "PSF", file = "LICENSE"}
```

### Comparing `standard_cgitb-3.10.14/standard_cgitb.egg-info/PKG-INFO` & `standard_cgitb-3.11.9/standard_cgitb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-cgitb
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library cgitb redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_cgitb-3.10.14/tests/test_cgitb.py` & `standard_cgitb-3.11.9/tests/test_cgitb.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from test.support.os_helper import temp_dir
 from test.support.script_helper import assert_python_failure
+from test.support.warnings_helper import import_deprecated
 import unittest
 import sys
-import cgitb
+cgitb = import_deprecated("cgitb")
 
 class TestCgitb(unittest.TestCase):
 
     def test_fonts(self):
         text = "Hello Robbie!"
         self.assertEqual(cgitb.small(text), "<small>{}</small>".format(text))
         self.assertEqual(cgitb.strong(text), "<strong>{}</strong>".format(text))
```


# Comparing `tmp/standard_uu-3.10.14.tar.gz` & `tmp/standard_uu-3.11.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_uu-3.10.14.tar", last modified: Sun Apr 21 18:52:13 2024, max compression
+gzip compressed data, was "standard_uu-3.11.9.tar", last modified: Sun Apr 21 19:05:32 2024, max compression
```

## Comparing `standard_uu-3.10.14.tar` & `standard_uu-3.11.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:52:13.406603 standard_uu-3.10.14/
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_uu-3.10.14/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     3801 2024-04-21 18:52:13.406381 standard_uu-3.10.14/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_uu-3.10.14/README.rst
--rw-r--r--   0 user       (501) staff       (20)      697 2024-04-21 18:45:40.000000 standard_uu-3.10.14/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 18:52:13.406650 standard_uu-3.10.14/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:52:13.406165 standard_uu-3.10.14/standard_uu.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3801 2024-04-21 18:52:13.000000 standard_uu-3.10.14/standard_uu.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      205 2024-04-21 18:52:13.000000 standard_uu-3.10.14/standard_uu.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 18:52:13.000000 standard_uu-3.10.14/standard_uu.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        3 2024-04-21 18:52:13.000000 standard_uu-3.10.14/standard_uu.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:52:13.405798 standard_uu-3.10.14/tests/
--rw-r--r--   0 user       (501) staff       (20)     9129 2024-04-21 18:45:40.000000 standard_uu-3.10.14/tests/test_uu.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:52:13.405962 standard_uu-3.10.14/uu/
--rw-r--r--   0 user       (501) staff       (20)     7301 2024-04-21 18:45:40.000000 standard_uu-3.10.14/uu/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:32.640220 standard_uu-3.11.9/
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_uu-3.11.9/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     3800 2024-04-21 19:05:32.640010 standard_uu-3.11.9/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_uu-3.11.9/README.rst
+-rw-r--r--   0 user       (501) staff       (20)      696 2024-04-21 19:00:02.000000 standard_uu-3.11.9/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 19:05:32.640266 standard_uu-3.11.9/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:32.639801 standard_uu-3.11.9/standard_uu.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3800 2024-04-21 19:05:32.000000 standard_uu-3.11.9/standard_uu.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      205 2024-04-21 19:05:32.000000 standard_uu-3.11.9/standard_uu.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 19:05:32.000000 standard_uu-3.11.9/standard_uu.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        3 2024-04-21 19:05:32.000000 standard_uu-3.11.9/standard_uu.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:32.639386 standard_uu-3.11.9/tests/
+-rw-r--r--   0 user       (501) staff       (20)     9416 2024-04-21 19:00:02.000000 standard_uu-3.11.9/tests/test_uu.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:32.639584 standard_uu-3.11.9/uu/
+-rw-r--r--   0 user       (501) staff       (20)     7365 2024-04-21 19:00:02.000000 standard_uu-3.11.9/uu/__init__.py
```

### Comparing `standard_uu-3.10.14/LICENSE` & `standard_uu-3.11.9/LICENSE`

 * *Files identical despite different names*

### Comparing `standard_uu-3.10.14/PKG-INFO` & `standard_uu-3.11.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-uu
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library uu redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_uu-3.10.14/pyproject.toml` & `standard_uu-3.11.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "standard-uu"
-version = "3.10.14"
+version = "3.11.9"
 description = "Standard library uu redistribution. \"dead battery\"."
 keywords = ["stdlib"]
 authors = [
     { name = "Python Devleopers", email = "python-deadlib@youknowone.org" }
 ]
 readme = "README.rst"
 license = {name = "PSF", file = "LICENSE"}
```

### Comparing `standard_uu-3.10.14/standard_uu.egg-info/PKG-INFO` & `standard_uu-3.11.9/standard_uu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-uu
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library uu redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_uu-3.10.14/tests/test_uu.py` & `standard_uu-3.11.9/tests/test_uu.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 Tests for uu module.
 Nick Mathewson
 """
 
 import unittest
-from test.support import os_helper
+from test.support import os_helper, warnings_helper
+
+uu = warnings_helper.import_deprecated("uu")
 
 import os
 import stat
 import sys
-import uu
 import io
 
 plaintext = b"The symbols on top of your keyboard are !@#$%^&*()_+|~\n"
 
 encodedtext = b"""\
 M5&AE('-Y;6)O;',@;VX@=&]P(&]F('EO=7(@:V5Y8F]A<F0@87)E("% (R0E
 *7B8J*"E?*WQ^"@  """
@@ -69,14 +70,15 @@
         inp = io.BytesIO(plaintext)
         out = io.BytesIO()
         uu.encode(inp, out, "t1", backtick=True)
         self.assertEqual(out.getvalue(), encodedtextwrapped(0o666, "t1", True))
         with self.assertRaises(TypeError):
             uu.encode(inp, out, "t1", 0o644, True)
 
+    @os_helper.skip_unless_working_chmod
     def test_decode(self):
         for backtick in True, False:
             inp = io.BytesIO(encodedtextwrapped(0o666, "t1", backtick=backtick))
             out = io.BytesIO()
             uu.decode(inp, out)
             self.assertEqual(out.getvalue(), plaintext)
             inp = io.BytesIO(
@@ -222,46 +224,51 @@
 
         # in_file and out_file as filenames
         uu.encode(self.tmpin, self.tmpout, self.tmpin, mode=0o644)
         with open(self.tmpout, 'rb') as fout:
             s = fout.read()
         self.assertEqual(s, encodedtextwrapped(0o644, self.tmpin))
 
+    # decode() calls chmod()
+    @os_helper.skip_unless_working_chmod
     def test_decode(self):
         with open(self.tmpin, 'wb') as f:
             f.write(encodedtextwrapped(0o644, self.tmpout))
 
         with open(self.tmpin, 'rb') as f:
             uu.decode(f)
 
         with open(self.tmpout, 'rb') as f:
             s = f.read()
         self.assertEqual(s, plaintext)
         # XXX is there an xp way to verify the mode?
 
+    @os_helper.skip_unless_working_chmod
     def test_decode_filename(self):
         with open(self.tmpin, 'wb') as f:
             f.write(encodedtextwrapped(0o644, self.tmpout))
 
         uu.decode(self.tmpin)
 
         with open(self.tmpout, 'rb') as f:
             s = f.read()
         self.assertEqual(s, plaintext)
 
+    @os_helper.skip_unless_working_chmod
     def test_decodetwice(self):
         # Verify that decode() will refuse to overwrite an existing file
         with open(self.tmpin, 'wb') as f:
             f.write(encodedtextwrapped(0o644, self.tmpout))
         with open(self.tmpin, 'rb') as f:
             uu.decode(f)
 
         with open(self.tmpin, 'rb') as f:
             self.assertRaises(uu.Error, uu.decode, f)
 
+    @os_helper.skip_unless_working_chmod
     def test_decode_mode(self):
         # Verify that decode() will set the given mode for the out_file
         expected_mode = 0o444
         with open(self.tmpin, 'wb') as f:
             f.write(encodedtextwrapped(expected_mode, self.tmpout))
 
         # make file writable again, so it can be removed (Windows only)
```

### Comparing `standard_uu-3.10.14/uu/__init__.py` & `standard_uu-3.11.9/uu/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 encode(in_file, out_file [,name, mode], *, backtick=False)
 decode(in_file [, out_file, mode, quiet])
 """
 
 import binascii
 import os
 import sys
+import warnings
+
+warnings._deprecated(__name__, remove=(3, 13))
 
 __all__ = ["Error", "encode", "decode"]
 
 class Error(Exception):
     pass
 
 def encode(in_file, out_file, name=None, mode=None, *, backtick=False):
```


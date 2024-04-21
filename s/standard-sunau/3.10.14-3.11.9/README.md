# Comparing `tmp/standard_sunau-3.10.14.tar.gz` & `tmp/standard_sunau-3.11.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_sunau-3.10.14.tar", last modified: Sun Apr 21 18:52:07 2024, max compression
+gzip compressed data, was "standard_sunau-3.11.9.tar", last modified: Sun Apr 21 19:05:25 2024, max compression
```

## Comparing `standard_sunau-3.10.14.tar` & `standard_sunau-3.11.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:52:07.187456 standard_sunau-3.10.14/
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_sunau-3.10.14/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     3807 2024-04-21 18:52:07.187257 standard_sunau-3.10.14/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_sunau-3.10.14/README.rst
--rw-r--r--   0 user       (501) staff       (20)      706 2024-04-21 18:45:40.000000 standard_sunau-3.10.14/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 18:52:07.187496 standard_sunau-3.10.14/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:52:07.187049 standard_sunau-3.10.14/standard_sunau.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3807 2024-04-21 18:52:07.000000 standard_sunau-3.10.14/standard_sunau.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      223 2024-04-21 18:52:07.000000 standard_sunau-3.10.14/standard_sunau.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 18:52:07.000000 standard_sunau-3.10.14/standard_sunau.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        6 2024-04-21 18:52:07.000000 standard_sunau-3.10.14/standard_sunau.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:52:07.186694 standard_sunau-3.10.14/sunau/
--rw-r--r--   0 user       (501) staff       (20)    18158 2024-04-21 18:45:40.000000 standard_sunau-3.10.14/sunau/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:52:07.186849 standard_sunau-3.10.14/tests/
--rw-r--r--   0 user       (501) staff       (20)     6125 2024-04-21 18:45:40.000000 standard_sunau-3.10.14/tests/test_sunau.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:25.652591 standard_sunau-3.11.9/
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_sunau-3.11.9/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     3806 2024-04-21 19:05:25.652331 standard_sunau-3.11.9/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_sunau-3.11.9/README.rst
+-rw-r--r--   0 user       (501) staff       (20)      705 2024-04-21 19:00:01.000000 standard_sunau-3.11.9/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 19:05:25.652635 standard_sunau-3.11.9/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:25.652039 standard_sunau-3.11.9/standard_sunau.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3806 2024-04-21 19:05:25.000000 standard_sunau-3.11.9/standard_sunau.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      223 2024-04-21 19:05:25.000000 standard_sunau-3.11.9/standard_sunau.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 19:05:25.000000 standard_sunau-3.11.9/standard_sunau.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        6 2024-04-21 19:05:25.000000 standard_sunau-3.11.9/standard_sunau.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:25.651551 standard_sunau-3.11.9/sunau/
+-rw-r--r--   0 user       (501) staff       (20)    18480 2024-04-21 19:00:01.000000 standard_sunau-3.11.9/sunau/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:25.651752 standard_sunau-3.11.9/tests/
+-rw-r--r--   0 user       (501) staff       (20)     6239 2024-04-21 19:00:01.000000 standard_sunau-3.11.9/tests/test_sunau.py
```

### Comparing `standard_sunau-3.10.14/LICENSE` & `standard_sunau-3.11.9/LICENSE`

 * *Files identical despite different names*

### Comparing `standard_sunau-3.10.14/PKG-INFO` & `standard_sunau-3.11.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-sunau
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library sunau redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_sunau-3.10.14/pyproject.toml` & `standard_sunau-3.11.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "standard-sunau"
-version = "3.10.14"
+version = "3.11.9"
 description = "Standard library sunau redistribution. \"dead battery\"."
 keywords = ["stdlib"]
 authors = [
     { name = "Python Devleopers", email = "python-deadlib@youknowone.org" }
 ]
 readme = "README.rst"
 license = {name = "PSF", file = "LICENSE"}
```

### Comparing `standard_sunau-3.10.14/standard_sunau.egg-info/PKG-INFO` & `standard_sunau-3.11.9/standard_sunau.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-sunau
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library sunau redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_sunau-3.10.14/sunau/__init__.py` & `standard_sunau-3.11.9/sunau/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,17 @@
 When all frames have been written, either call writeframes(b'') or
 close() to patch up the sizes in the header.
 The close() method is called automatically when the class instance
 is destroyed.
 """
 
 from collections import namedtuple
+import warnings
+
+warnings._deprecated(__name__, remove=(3, 13))
 
 
 _sunau_params = namedtuple('_sunau_params',
                            'nchannels sampwidth framerate nframes comptype compname')
 
 # from <multimedia/audio_filehdr.h>
 AUDIO_FILE_MAGIC = 0x2e736e64
@@ -271,15 +274,17 @@
         if self._encoding in _simple_encodings:
             if nframes == AUDIO_UNKNOWN_SIZE:
                 data = self._file.read()
             else:
                 data = self._file.read(nframes * self._framesize)
             self._soundpos += len(data) // self._framesize
             if self._encoding == AUDIO_FILE_ENCODING_MULAW_8:
-                import audioop
+                with warnings.catch_warnings():
+                    warnings.simplefilter('ignore', category=DeprecationWarning)
+                    import audioop
                 data = audioop.ulaw2lin(data, self._sampwidth)
             return data
         return None             # XXX--not implemented yet
 
     def rewind(self):
         if self._data_pos is None:
             raise OSError('cannot seek')
@@ -417,15 +422,17 @@
         return self._nframeswritten
 
     def writeframesraw(self, data):
         if not isinstance(data, (bytes, bytearray)):
             data = memoryview(data).cast('B')
         self._ensure_header_written()
         if self._comptype == 'ULAW':
-            import audioop
+            with warnings.catch_warnings():
+                warnings.simplefilter('ignore', category=DeprecationWarning)
+                import audioop
             data = audioop.lin2ulaw(data, self._sampwidth)
         nframes = len(data) // self._framesize
         self._file.write(data)
         self._nframeswritten = self._nframeswritten + nframes
         self._datawritten = self._datawritten + len(data)
 
     def writeframes(self, data):
```

### Comparing `standard_sunau-3.10.14/tests/test_sunau.py` & `standard_sunau-3.11.9/tests/test_sunau.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import unittest
 from test import audiotests
-from audioop import byteswap
 import io
 import struct
 import sys
-import sunau
+from test.support import warnings_helper
+
+sunau = warnings_helper.import_deprecated("sunau")
+audioop = warnings_helper.import_deprecated("audioop")
 
 
 class SunauTest(audiotests.AudioWriteTests,
                 audiotests.AudioTestsWithSourceFile):
     module = sunau
 
 
@@ -112,15 +114,15 @@
       B684FA24 B684F344 2A7CEC04 19FCE704 EE04E504 C584E204 0E3CE104 EF04DF84 \
       557CE204 FB24E804 12FCEF04 D784F744 9684FB64 F5C4FC24 083CFBA4 DF84FB24 \
       11FCFA24 3E7CFB64 BA84FCB4 657CFF5C CF84041C 417C09BC C1840EBC 517C12FC \
       EF0416FC 828415FC 7D7C13FC 828412FC 497C0EBC 517C0DBC F0040F3C CD840FFC \
       E5040CBC 617C0A3C 08BC0A3C 2C7C0B3C 517C0E3C 8A8410FC B6840EBC 457C0A3C \
       """)
     if sys.byteorder != 'big':
-        frames = byteswap(frames, 2)
+        frames = audioop.byteswap(frames, 2)
 
 
 class SunauLowLevelTest(unittest.TestCase):
 
     def test_read_bad_magic_number(self):
         b = b'SPA'
         with self.assertRaises(EOFError):
```


# Comparing `tmp/standard_aifc-3.10.14.tar.gz` & `tmp/standard_aifc-3.11.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_aifc-3.10.14.tar", last modified: Sun Apr 21 18:51:05 2024, max compression
+gzip compressed data, was "standard_aifc-3.11.9.tar", last modified: Sun Apr 21 19:04:25 2024, max compression
```

## Comparing `standard_aifc-3.10.14.tar` & `standard_aifc-3.11.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:05.729480 standard_aifc-3.10.14/
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_aifc-3.10.14/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     3805 2024-04-21 18:51:05.729158 standard_aifc-3.10.14/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_aifc-3.10.14/README.rst
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:05.726401 standard_aifc-3.10.14/aifc/
--rw-r--r--   0 user       (501) staff       (20)    32605 2024-04-21 18:45:39.000000 standard_aifc-3.10.14/aifc/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      703 2024-04-21 18:45:39.000000 standard_aifc-3.10.14/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 18:51:05.729558 standard_aifc-3.10.14/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:05.728760 standard_aifc-3.10.14/standard_aifc.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3805 2024-04-21 18:51:05.000000 standard_aifc-3.10.14/standard_aifc.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      217 2024-04-21 18:51:05.000000 standard_aifc-3.10.14/standard_aifc.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 18:51:05.000000 standard_aifc-3.10.14/standard_aifc.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        5 2024-04-21 18:51:05.000000 standard_aifc-3.10.14/standard_aifc.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:05.728185 standard_aifc-3.10.14/tests/
--rw-r--r--   0 user       (501) staff       (20)    18197 2024-04-21 18:45:39.000000 standard_aifc-3.10.14/tests/test_aifc.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:25.593732 standard_aifc-3.11.9/
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_aifc-3.11.9/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     3804 2024-04-21 19:04:25.593425 standard_aifc-3.11.9/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_aifc-3.11.9/README.rst
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:25.590721 standard_aifc-3.11.9/aifc/
+-rw-r--r--   0 user       (501) staff       (20)    34211 2024-04-21 19:00:01.000000 standard_aifc-3.11.9/aifc/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      702 2024-04-21 19:00:01.000000 standard_aifc-3.11.9/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 19:04:25.593801 standard_aifc-3.11.9/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:25.592898 standard_aifc-3.11.9/standard_aifc.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3804 2024-04-21 19:04:25.000000 standard_aifc-3.11.9/standard_aifc.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      217 2024-04-21 19:04:25.000000 standard_aifc-3.11.9/standard_aifc.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 19:04:25.000000 standard_aifc-3.11.9/standard_aifc.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        5 2024-04-21 19:04:25.000000 standard_aifc-3.11.9/standard_aifc.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:25.592400 standard_aifc-3.11.9/tests/
+-rw-r--r--   0 user       (501) staff       (20)    18266 2024-04-21 19:00:01.000000 standard_aifc-3.11.9/tests/test_aifc.py
```

### Comparing `standard_aifc-3.10.14/LICENSE` & `standard_aifc-3.11.9/LICENSE`

 * *Files identical despite different names*

### Comparing `standard_aifc-3.10.14/PKG-INFO` & `standard_aifc-3.11.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-aifc
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library aifc redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_aifc-3.10.14/aifc/__init__.py` & `standard_aifc-3.11.9/aifc/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,14 +136,18 @@
 
 import struct
 import builtins
 import warnings
 
 __all__ = ["Error", "open"]
 
+
+warnings._deprecated(__name__, remove=(3, 13))
+
+
 class Error(Exception):
     pass
 
 _AIFC_version = 0xA2805140     # Version 1 of AIFF-C
 
 def _read_long(file):
     try:
@@ -247,15 +251,17 @@
             fmant = math.ldexp(fmant - fsmant, 32)
             fsmant = math.floor(fmant)
             lomant = int(fsmant)
     _write_ushort(f, expon)
     _write_ulong(f, himant)
     _write_ulong(f, lomant)
 
-from chunk import Chunk
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore", DeprecationWarning)
+    from chunk import Chunk
 from collections import namedtuple
 
 _aifc_params = namedtuple('_aifc_params',
                           'nchannels sampwidth framerate nframes comptype compname')
 
 _aifc_params.nchannels.__doc__ = 'Number of audio channels (1 for mono, 2 for stereo)'
 _aifc_params.sampwidth.__doc__ = 'Sample width in bytes'
@@ -443,29 +449,41 @@
         return data
 
     #
     # Internal methods.
     #
 
     def _alaw2lin(self, data):
-        import audioop
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore', category=DeprecationWarning)
+            import audioop
         return audioop.alaw2lin(data, 2)
 
     def _ulaw2lin(self, data):
-        import audioop
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore', category=DeprecationWarning)
+            import audioop
         return audioop.ulaw2lin(data, 2)
 
     def _adpcm2lin(self, data):
-        import audioop
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore', category=DeprecationWarning)
+            import audioop
         if not hasattr(self, '_adpcmstate'):
             # first time
             self._adpcmstate = None
         data, self._adpcmstate = audioop.adpcm2lin(data, 2, self._adpcmstate)
         return data
 
+    def _sowt2lin(self, data):
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore', category=DeprecationWarning)
+            import audioop
+        return audioop.byteswap(data, 2)
+
     def _read_comm_chunk(self, chunk):
         self._nchannels = _read_short(chunk)
         self._nframes = _read_long(chunk)
         self._sampwidth = (_read_short(chunk) + 7) // 8
         self._framerate = int(_read_float(chunk))
         if self._sampwidth <= 0:
             raise Error('bad sample width')
@@ -493,14 +511,16 @@
             if self._comptype != b'NONE':
                 if self._comptype == b'G722':
                     self._convert = self._adpcm2lin
                 elif self._comptype in (b'ulaw', b'ULAW'):
                     self._convert = self._ulaw2lin
                 elif self._comptype in (b'alaw', b'ALAW'):
                     self._convert = self._alaw2lin
+                elif self._comptype in (b'sowt', b'SOWT'):
+                    self._convert = self._sowt2lin
                 else:
                     raise Error('unsupported compression type')
                 self._sampwidth = 2
         else:
             self._comptype = b'NONE'
             self._compname = b'not compressed'
 
@@ -655,15 +675,15 @@
     def getnframes(self):
         return self._nframeswritten
 
     def setcomptype(self, comptype, compname):
         if self._nframeswritten:
             raise Error('cannot change parameters after starting to write')
         if comptype not in (b'NONE', b'ulaw', b'ULAW',
-                            b'alaw', b'ALAW', b'G722'):
+                            b'alaw', b'ALAW', b'G722', b'sowt', b'SOWT'):
             raise Error('unsupported compression type')
         self._comptype = comptype
         self._compname = compname
 
     def getcomptype(self):
         return self._comptype
 
@@ -676,15 +696,15 @@
 ##      self._version = version
 
     def setparams(self, params):
         nchannels, sampwidth, framerate, nframes, comptype, compname = params
         if self._nframeswritten:
             raise Error('cannot change parameters after starting to write')
         if comptype not in (b'NONE', b'ulaw', b'ULAW',
-                            b'alaw', b'ALAW', b'G722'):
+                            b'alaw', b'ALAW', b'G722', b'sowt', b'SOWT'):
             raise Error('unsupported compression type')
         self.setnchannels(nchannels)
         self.setsampwidth(sampwidth)
         self.setframerate(framerate)
         self.setnframes(nframes)
         self.setcomptype(comptype, compname)
 
@@ -760,36 +780,51 @@
             f.close()
 
     #
     # Internal methods.
     #
 
     def _lin2alaw(self, data):
-        import audioop
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore', category=DeprecationWarning)
+            import audioop
         return audioop.lin2alaw(data, 2)
 
     def _lin2ulaw(self, data):
-        import audioop
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore', category=DeprecationWarning)
+            import audioop
         return audioop.lin2ulaw(data, 2)
 
     def _lin2adpcm(self, data):
-        import audioop
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore', category=DeprecationWarning)
+            import audioop
         if not hasattr(self, '_adpcmstate'):
             self._adpcmstate = None
         data, self._adpcmstate = audioop.lin2adpcm(data, 2, self._adpcmstate)
         return data
 
+    def _lin2sowt(self, data):
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore', category=DeprecationWarning)
+            import audioop
+        return audioop.byteswap(data, 2)
+
     def _ensure_header_written(self, datasize):
         if not self._nframeswritten:
-            if self._comptype in (b'ULAW', b'ulaw', b'ALAW', b'alaw', b'G722'):
+            if self._comptype in (b'ULAW', b'ulaw',
+                b'ALAW', b'alaw', b'G722',
+                b'sowt', b'SOWT'):
                 if not self._sampwidth:
                     self._sampwidth = 2
                 if self._sampwidth != 2:
                     raise Error('sample width must be 2 when compressing '
-                                'with ulaw/ULAW, alaw/ALAW or G7.22 (ADPCM)')
+                                'with ulaw/ULAW, alaw/ALAW, sowt/SOWT '
+                                'or G7.22 (ADPCM)')
             if not self._nchannels:
                 raise Error('# channels not specified')
             if not self._sampwidth:
                 raise Error('sample width not specified')
             if not self._framerate:
                 raise Error('sampling rate not specified')
             self._write_header(datasize)
@@ -797,14 +832,16 @@
     def _init_compression(self):
         if self._comptype == b'G722':
             self._convert = self._lin2adpcm
         elif self._comptype in (b'ulaw', b'ULAW'):
             self._convert = self._lin2ulaw
         elif self._comptype in (b'alaw', b'ALAW'):
             self._convert = self._lin2alaw
+        elif self._comptype in (b'sowt', b'SOWT'):
+            self._convert = self._lin2sowt
 
     def _write_header(self, initlength):
         if self._aifc and self._comptype != b'NONE':
             self._init_compression()
         self._file.write(b'FORM')
         if not self._nframes:
             self._nframes = initlength // (self._nchannels * self._sampwidth)
```

### Comparing `standard_aifc-3.10.14/pyproject.toml` & `standard_aifc-3.11.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "standard-aifc"
-version = "3.10.14"
+version = "3.11.9"
 description = "Standard library aifc redistribution. \"dead battery\"."
 keywords = ["stdlib"]
 authors = [
     { name = "Python Devleopers", email = "python-deadlib@youknowone.org" }
 ]
 readme = "README.rst"
 license = {name = "PSF", file = "LICENSE"}
```

### Comparing `standard_aifc-3.10.14/standard_aifc.egg-info/PKG-INFO` & `standard_aifc-3.11.9/standard_aifc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-aifc
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library aifc redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_aifc-3.10.14/tests/test_aifc.py` & `standard_aifc-3.11.9/tests/test_aifc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from test.support import findfile
 from test.support.os_helper import TESTFN, unlink
-from test.support.warnings_helper import check_no_resource_warning
+from test.support.warnings_helper import check_no_resource_warning, import_deprecated
 import unittest
 from unittest import mock
 from test import audiotests
-from audioop import byteswap
 import io
 import sys
 import struct
-import aifc
+
+
+aifc = import_deprecated("aifc")
+audioop = import_deprecated("audioop")
+
 
 class AifcTest(audiotests.AudioWriteTests,
                audiotests.AudioTestsWithSourceFile):
     module = aifc
     close_fd = True
     test_unseekable_read = None
 
@@ -117,15 +120,15 @@
       B684FA24 B684F344 2A7CEC04 19FCE704 EE04E504 C584E204 0E3CE104 EF04DF84 \
       557CE204 FB24E804 12FCEF04 D784F744 9684FB64 F5C4FC24 083CFBA4 DF84FB24 \
       11FCFA24 3E7CFB64 BA84FCB4 657CFF5C CF84041C 417C093C C1840EBC 517C12FC \
       EF0416FC 828415FC 7D7C13FC 828412FC 497C0EBC 517C0DBC F0040F3C CD840FFC \
       E5040CBC 617C0A3C 08BC0A3C 2C7C0B3C 517C0E3C 8A8410FC B6840EBC 457C0A3C \
       """)
     if sys.byteorder != 'big':
-        frames = byteswap(frames, 2)
+        frames = audioop.byteswap(frames, 2)
 
 
 class AifcALAWTest(AifcTest, unittest.TestCase):
     sndfilename = 'pluck-alaw.aifc'
     sndfilenframes = 3307
     nchannels = 2
     sampwidth = 2
@@ -138,15 +141,15 @@
       BA00FA20 B600F340 2900EB80 1A80E680 ED80E480 C700E280 0E40E080 EF80E080 \
       5600E280 FB20E880 1380EF80 D900F740 9600FB60 F5C0FC10 0840FBA0 DF00FB20 \
       1180FA20 3F00FB60 BE00FCB0 6600FF58 CF000420 42000940 C1000EC0 52001280 \
       EE801780 82001680 7E001480 82001280 4A000EC0 52000DC0 EF800F40 CF000FC0 \
       E4800CC0 62000A40 08C00A40 2B000B40 52000E40 8A001180 B6000EC0 46000A40 \
       """)
     if sys.byteorder != 'big':
-        frames = byteswap(frames, 2)
+        frames = audioop.byteswap(frames, 2)
 
 
 class AifcMiscTest(unittest.TestCase):
     def test_skipunknown(self):
         #Issue 2245
         #This file contains chunk types aifc doesn't recognize.
         f = aifc.open(findfile('Sine-1000Hz-300ms.aif'))
```


# Comparing `tmp/standard_sndhdr-3.10.14.tar.gz` & `tmp/standard_sndhdr-3.11.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_sndhdr-3.10.14.tar", last modified: Sun Apr 21 18:52:03 2024, max compression
+gzip compressed data, was "standard_sndhdr-3.11.9.tar", last modified: Sun Apr 21 19:05:22 2024, max compression
```

## Comparing `standard_sndhdr-3.10.14.tar` & `standard_sndhdr-3.11.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:52:03.499882 standard_sndhdr-3.10.14/
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_sndhdr-3.10.14/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     3809 2024-04-21 18:52:03.499697 standard_sndhdr-3.10.14/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_sndhdr-3.10.14/README.rst
--rw-r--r--   0 user       (501) staff       (20)      709 2024-04-21 18:45:39.000000 standard_sndhdr-3.10.14/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 18:52:03.499921 standard_sndhdr-3.10.14/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:52:03.498722 standard_sndhdr-3.10.14/sndhdr/
--rw-r--r--   0 user       (501) staff       (20)     7099 2024-04-21 18:45:40.000000 standard_sndhdr-3.10.14/sndhdr/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:52:03.499513 standard_sndhdr-3.10.14/standard_sndhdr.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3809 2024-04-21 18:52:03.000000 standard_sndhdr-3.10.14/standard_sndhdr.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      229 2024-04-21 18:52:03.000000 standard_sndhdr-3.10.14/standard_sndhdr.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 18:52:03.000000 standard_sndhdr-3.10.14/standard_sndhdr.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        7 2024-04-21 18:52:03.000000 standard_sndhdr-3.10.14/standard_sndhdr.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:52:03.499344 standard_sndhdr-3.10.14/tests/
--rw-r--r--   0 user       (501) staff       (20)     1460 2024-04-21 18:45:40.000000 standard_sndhdr-3.10.14/tests/test_sndhdr.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:22.112013 standard_sndhdr-3.11.9/
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_sndhdr-3.11.9/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     3808 2024-04-21 19:05:22.111731 standard_sndhdr-3.11.9/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_sndhdr-3.11.9/README.rst
+-rw-r--r--   0 user       (501) staff       (20)      708 2024-04-21 19:00:01.000000 standard_sndhdr-3.11.9/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 19:05:22.112059 standard_sndhdr-3.11.9/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:22.110501 standard_sndhdr-3.11.9/sndhdr/
+-rw-r--r--   0 user       (501) staff       (20)     7448 2024-04-21 19:00:01.000000 standard_sndhdr-3.11.9/sndhdr/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:22.111451 standard_sndhdr-3.11.9/standard_sndhdr.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3808 2024-04-21 19:05:22.000000 standard_sndhdr-3.11.9/standard_sndhdr.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      229 2024-04-21 19:05:22.000000 standard_sndhdr-3.11.9/standard_sndhdr.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 19:05:22.000000 standard_sndhdr-3.11.9/standard_sndhdr.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        7 2024-04-21 19:05:22.000000 standard_sndhdr-3.11.9/standard_sndhdr.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:22.111252 standard_sndhdr-3.11.9/tests/
+-rw-r--r--   0 user       (501) staff       (20)     1542 2024-04-21 19:00:01.000000 standard_sndhdr-3.11.9/tests/test_sndhdr.py
```

### Comparing `standard_sndhdr-3.10.14/LICENSE` & `standard_sndhdr-3.11.9/LICENSE`

 * *Files identical despite different names*

### Comparing `standard_sndhdr-3.10.14/PKG-INFO` & `standard_sndhdr-3.11.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-sndhdr
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library sndhdr redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_sndhdr-3.10.14/pyproject.toml` & `standard_sndhdr-3.11.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "standard-sndhdr"
-version = "3.10.14"
+version = "3.11.9"
 description = "Standard library sndhdr redistribution. \"dead battery\"."
 keywords = ["stdlib"]
 authors = [
     { name = "Python Devleopers", email = "python-deadlib@youknowone.org" }
 ]
 readme = "README.rst"
 license = {name = "PSF", file = "LICENSE"}
```

### Comparing `standard_sndhdr-3.10.14/sndhdr/__init__.py` & `standard_sndhdr-3.11.9/sndhdr/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 what() for all files mentioned on the argument list.  For directory
 arguments it calls what() for all files in that directory.  Default
 argument is "." (testing all files in the current directory).  The
 option -r tells it to recurse down directories found inside
 explicitly given directories.
 """
 
+import warnings
+
+warnings._deprecated(__name__, remove=(3, 13))
+
 # The file structure is top-down except that the test program and its
 # subroutine come last.
 
 __all__ = ['what', 'whathdr']
 
 from collections import namedtuple
 
@@ -69,15 +73,18 @@
 #-----------------------------------#
 # Subroutines per sound header type #
 #-----------------------------------#
 
 tests = []
 
 def test_aifc(h, f):
-    import aifc
+    """AIFC and AIFF files"""
+    with warnings.catch_warnings():
+        warnings.simplefilter('ignore', category=DeprecationWarning)
+        import aifc
     if not h.startswith(b'FORM'):
         return None
     if h[8:12] == b'AIFC':
         fmt = 'aifc'
     elif h[8:12] == b'AIFF':
         fmt = 'aiff'
     else:
@@ -90,14 +97,15 @@
     return (fmt, a.getframerate(), a.getnchannels(),
             a.getnframes(), 8 * a.getsampwidth())
 
 tests.append(test_aifc)
 
 
 def test_au(h, f):
+    """AU and SND files"""
     if h.startswith(b'.snd'):
         func = get_long_be
     elif h[:4] in (b'\0ds.', b'dns.'):
         func = get_long_le
     else:
         return None
     filetype = 'au'
@@ -123,41 +131,44 @@
         nframe = -1
     return filetype, rate, nchannels, nframe, sample_bits
 
 tests.append(test_au)
 
 
 def test_hcom(h, f):
+    """HCOM file"""
     if h[65:69] != b'FSSD' or h[128:132] != b'HCOM':
         return None
     divisor = get_long_be(h[144:148])
     if divisor:
         rate = 22050 / divisor
     else:
         rate = 0
     return 'hcom', rate, 1, -1, 8
 
 tests.append(test_hcom)
 
 
 def test_voc(h, f):
+    """VOC file"""
     if not h.startswith(b'Creative Voice File\032'):
         return None
     sbseek = get_short_le(h[20:22])
     rate = 0
     if 0 <= sbseek < 500 and h[sbseek] == 1:
         ratecode = 256 - h[sbseek+4]
         if ratecode:
             rate = int(1000000.0 / ratecode)
     return 'voc', rate, 1, -1, 8
 
 tests.append(test_voc)
 
 
 def test_wav(h, f):
+    """WAV file"""
     import wave
     # 'RIFF' <len> 'WAVE' 'fmt ' <len>
     if not h.startswith(b'RIFF') or h[8:12] != b'WAVE' or h[12:16] != b'fmt ':
         return None
     f.seek(0)
     try:
         w = wave.open(f, 'r')
@@ -166,32 +177,35 @@
     return ('wav', w.getframerate(), w.getnchannels(),
                    w.getnframes(), 8*w.getsampwidth())
 
 tests.append(test_wav)
 
 
 def test_8svx(h, f):
+    """8SVX file"""
     if not h.startswith(b'FORM') or h[8:12] != b'8SVX':
         return None
     # Should decode it to get #channels -- assume always 1
     return '8svx', 0, 1, 0, 8
 
 tests.append(test_8svx)
 
 
 def test_sndt(h, f):
+    """SNDT file"""
     if h.startswith(b'SOUND'):
         nsamples = get_long_le(h[8:12])
         rate = get_short_le(h[20:22])
         return 'sndt', rate, 1, nsamples, 8
 
 tests.append(test_sndt)
 
 
 def test_sndr(h, f):
+    """SNDR file"""
     if h.startswith(b'\0\0'):
         rate = get_short_le(h[2:4])
         if 4000 <= rate <= 25000:
             return 'sndr', rate, 1, -1, 8
 
 tests.append(test_sndr)
```

### Comparing `standard_sndhdr-3.10.14/standard_sndhdr.egg-info/PKG-INFO` & `standard_sndhdr-3.11.9/standard_sndhdr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-sndhdr
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library sndhdr redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_sndhdr-3.10.14/tests/test_sndhdr.py` & `standard_sndhdr-3.11.9/tests/test_sndhdr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-import sndhdr
 import pickle
 import unittest
 from test.support import findfile
+from test.support import warnings_helper
+
+sndhdr = warnings_helper.import_deprecated("sndhdr")
+
 
 class TestFormats(unittest.TestCase):
     def test_data(self):
         for filename, expected in (
             ('sndhdr.8svx', ('8svx', 0, 1, 0, 8)),
             ('sndhdr.aifc', ('aifc', 44100, 2, 5, 16)),
             ('sndhdr.aiff', ('aiff', 44100, 2, 5, 16)),
```


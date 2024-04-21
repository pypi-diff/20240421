# Comparing `tmp/standard_telnetlib-3.10.14.tar.gz` & `tmp/standard_telnetlib-3.11.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_telnetlib-3.10.14.tar", last modified: Sun Apr 21 18:52:10 2024, max compression
+gzip compressed data, was "standard_telnetlib-3.11.9.tar", last modified: Sun Apr 21 19:05:29 2024, max compression
```

## Comparing `standard_telnetlib-3.10.14.tar` & `standard_telnetlib-3.11.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:52:10.380187 standard_telnetlib-3.10.14/
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_telnetlib-3.10.14/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     3815 2024-04-21 18:52:10.379960 standard_telnetlib-3.10.14/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_telnetlib-3.10.14/README.rst
--rw-r--r--   0 user       (501) staff       (20)      718 2024-04-21 18:45:40.000000 standard_telnetlib-3.10.14/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 18:52:10.380231 standard_telnetlib-3.10.14/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:52:10.379781 standard_telnetlib-3.10.14/standard_telnetlib.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3815 2024-04-21 18:52:10.000000 standard_telnetlib-3.10.14/standard_telnetlib.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      247 2024-04-21 18:52:10.000000 standard_telnetlib-3.10.14/standard_telnetlib.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 18:52:10.000000 standard_telnetlib-3.10.14/standard_telnetlib.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       10 2024-04-21 18:52:10.000000 standard_telnetlib-3.10.14/standard_telnetlib.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:52:10.379376 standard_telnetlib-3.10.14/telnetlib/
--rw-r--r--   0 user       (501) staff       (20)    23254 2024-04-21 18:45:40.000000 standard_telnetlib-3.10.14/telnetlib/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:52:10.379528 standard_telnetlib-3.10.14/tests/
--rw-r--r--   0 user       (501) staff       (20)    13050 2024-04-21 18:45:40.000000 standard_telnetlib-3.10.14/tests/test_telnetlib.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:29.277750 standard_telnetlib-3.11.9/
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_telnetlib-3.11.9/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     3814 2024-04-21 19:05:29.277508 standard_telnetlib-3.11.9/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_telnetlib-3.11.9/README.rst
+-rw-r--r--   0 user       (501) staff       (20)      717 2024-04-21 19:00:01.000000 standard_telnetlib-3.11.9/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 19:05:29.277819 standard_telnetlib-3.11.9/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:29.277191 standard_telnetlib-3.11.9/standard_telnetlib.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3814 2024-04-21 19:05:29.000000 standard_telnetlib-3.11.9/standard_telnetlib.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      247 2024-04-21 19:05:29.000000 standard_telnetlib-3.11.9/standard_telnetlib.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 19:05:29.000000 standard_telnetlib-3.11.9/standard_telnetlib.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       10 2024-04-21 19:05:29.000000 standard_telnetlib-3.11.9/standard_telnetlib.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:29.276598 standard_telnetlib-3.11.9/telnetlib/
+-rw-r--r--   0 user       (501) staff       (20)    23301 2024-04-21 19:00:02.000000 standard_telnetlib-3.11.9/telnetlib/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:29.276891 standard_telnetlib-3.11.9/tests/
+-rw-r--r--   0 user       (501) staff       (20)    13156 2024-04-21 19:00:02.000000 standard_telnetlib-3.11.9/tests/test_telnetlib.py
```

### Comparing `standard_telnetlib-3.10.14/LICENSE` & `standard_telnetlib-3.11.9/LICENSE`

 * *Files identical despite different names*

### Comparing `standard_telnetlib-3.10.14/PKG-INFO` & `standard_telnetlib-3.11.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-telnetlib
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library telnetlib redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_telnetlib-3.10.14/pyproject.toml` & `standard_telnetlib-3.11.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "standard-telnetlib"
-version = "3.10.14"
+version = "3.11.9"
 description = "Standard library telnetlib redistribution. \"dead battery\"."
 keywords = ["stdlib"]
 authors = [
     { name = "Python Devleopers", email = "python-deadlib@youknowone.org" }
 ]
 readme = "README.rst"
 license = {name = "PSF", file = "LICENSE"}
```

### Comparing `standard_telnetlib-3.10.14/standard_telnetlib.egg-info/PKG-INFO` & `standard_telnetlib-3.11.9/standard_telnetlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-telnetlib
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library telnetlib redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_telnetlib-3.10.14/telnetlib/__init__.py` & `standard_telnetlib-3.11.9/telnetlib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 
 
 # Imported modules
 import sys
 import socket
 import selectors
 from time import monotonic as _time
+import warnings
+
+warnings._deprecated(__name__, remove=(3, 13))
 
 __all__ = ["Telnet"]
 
 # Tunable parameters
 DEBUGLEVEL = 0
 
 # Telnet protocol defaults
@@ -485,15 +488,14 @@
                         if self.option_callback:
                             self.option_callback(self.sock, cmd, opt)
                         else:
                             self.sock.sendall(IAC + DONT + opt)
         except EOFError: # raised by self.rawq_getchar()
             self.iacseq = b'' # Reset on EOF
             self.sb = 0
-            pass
         self.cookedq = self.cookedq + buf[0]
         self.sbdataq = self.sbdataq + buf[1]
 
     def rawq_getchar(self):
         """Get next char from raw queue.
 
         Block if no data is immediately available.  Raise EOFError
```

### Comparing `standard_telnetlib-3.10.14/tests/test_telnetlib.py` & `standard_telnetlib-3.11.9/tests/test_telnetlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import socket
 import selectors
-import telnetlib
 import threading
 import contextlib
 
 from test import support
-from test.support import socket_helper
+from test.support import socket_helper, warnings_helper
 import unittest
 
+support.requires_working_socket(module=True)
+
+telnetlib = warnings_helper.import_deprecated('telnetlib')
+
 HOST = socket_helper.HOST
 
 def server(evt, serv):
     serv.listen()
     evt.set()
     try:
         conn, addr = serv.accept()
```


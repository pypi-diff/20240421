# Comparing `tmp/standard_nntplib-3.10.14.tar.gz` & `tmp/standard_nntplib-3.11.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_nntplib-3.10.14.tar", last modified: Sun Apr 21 18:51:53 2024, max compression
+gzip compressed data, was "standard_nntplib-3.11.9.tar", last modified: Sun Apr 21 19:05:11 2024, max compression
```

## Comparing `standard_nntplib-3.10.14.tar` & `standard_nntplib-3.11.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:53.542812 standard_nntplib-3.10.14/
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_nntplib-3.10.14/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     3811 2024-04-21 18:51:53.542565 standard_nntplib-3.10.14/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_nntplib-3.10.14/README.rst
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:53.540240 standard_nntplib-3.10.14/nntplib/
--rw-r--r--   0 user       (501) staff       (20)    41023 2024-04-21 18:45:39.000000 standard_nntplib-3.10.14/nntplib/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      712 2024-04-21 18:45:39.000000 standard_nntplib-3.10.14/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 18:51:53.542857 standard_nntplib-3.10.14/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:53.542290 standard_nntplib-3.10.14/standard_nntplib.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3811 2024-04-21 18:51:53.000000 standard_nntplib-3.10.14/standard_nntplib.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      235 2024-04-21 18:51:53.000000 standard_nntplib-3.10.14/standard_nntplib.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 18:51:53.000000 standard_nntplib-3.10.14/standard_nntplib.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2024-04-21 18:51:53.000000 standard_nntplib-3.10.14/standard_nntplib.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:53.541410 standard_nntplib-3.10.14/tests/
--rw-r--r--   0 user       (501) staff       (20)    64188 2024-04-21 18:45:39.000000 standard_nntplib-3.10.14/tests/test_nntplib.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:11.778050 standard_nntplib-3.11.9/
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_nntplib-3.11.9/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     3810 2024-04-21 19:05:11.777808 standard_nntplib-3.11.9/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_nntplib-3.11.9/README.rst
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:11.775640 standard_nntplib-3.11.9/nntplib/
+-rw-r--r--   0 user       (501) staff       (20)    41087 2024-04-21 19:03:37.000000 standard_nntplib-3.11.9/nntplib/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      711 2024-04-21 19:03:37.000000 standard_nntplib-3.11.9/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 19:05:11.778093 standard_nntplib-3.11.9/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:11.777577 standard_nntplib-3.11.9/standard_nntplib.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3810 2024-04-21 19:05:11.000000 standard_nntplib-3.11.9/standard_nntplib.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      235 2024-04-21 19:05:11.000000 standard_nntplib-3.11.9/standard_nntplib.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 19:05:11.000000 standard_nntplib-3.11.9/standard_nntplib.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2024-04-21 19:05:11.000000 standard_nntplib-3.11.9/standard_nntplib.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:05:11.776522 standard_nntplib-3.11.9/tests/
+-rw-r--r--   0 user       (501) staff       (20)    64202 2024-04-21 19:03:37.000000 standard_nntplib-3.11.9/tests/test_nntplib.py
```

### Comparing `standard_nntplib-3.10.14/LICENSE` & `standard_nntplib-3.11.9/LICENSE`

 * *Files identical despite different names*

### Comparing `standard_nntplib-3.10.14/PKG-INFO` & `standard_nntplib-3.11.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-nntplib
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library nntplib redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_nntplib-3.10.14/nntplib/__init__.py` & `standard_nntplib-3.11.9/nntplib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 
 # Imports
 import re
 import socket
 import collections
 import datetime
 import sys
+import warnings
 
 try:
     import ssl
 except ImportError:
     _have_ssl = False
 else:
     _have_ssl = True
@@ -81,14 +82,16 @@
 
 __all__ = ["NNTP",
            "NNTPError", "NNTPReplyError", "NNTPTemporaryError",
            "NNTPPermanentError", "NNTPProtocolError", "NNTPDataError",
            "decode_header",
            ]
 
+warnings._deprecated(__name__, remove=(3, 13))
+
 # maximal line length when calling readline(). This is to prevent
 # reading arbitrary length lines. RFC 3977 limits NNTP line length to
 # 512 characters, including CRLF. We have selected 2048 just to be on
 # the safe side.
 _MAXLINE = 2048
```

### Comparing `standard_nntplib-3.10.14/pyproject.toml` & `standard_nntplib-3.11.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "standard-nntplib"
-version = "3.10.14"
+version = "3.11.9"
 description = "Standard library nntplib redistribution. \"dead battery\"."
 keywords = ["stdlib"]
 authors = [
     { name = "Python Devleopers", email = "python-deadlib@youknowone.org" }
 ]
 readme = "README.rst"
 license = {name = "PSF", file = "LICENSE"}
```

### Comparing `standard_nntplib-3.10.14/standard_nntplib.egg-info/PKG-INFO` & `standard_nntplib-3.11.9/standard_nntplib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-nntplib
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library nntplib redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_nntplib-3.10.14/tests/test_nntplib.py` & `standard_nntplib-3.11.9/tests/test_nntplib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import io
 import socket
 import datetime
 import textwrap
 import unittest
 import functools
 import contextlib
-import nntplib
 import os.path
 import re
 import threading
 
 from test import support
-from test.support import socket_helper
+from test.support import socket_helper, warnings_helper
+nntplib = warnings_helper.import_deprecated("nntplib")
 from nntplib import NNTP, GroupInfo
 from unittest.mock import patch
 try:
     import ssl
 except ImportError:
     ssl = None
 
 
-certfile = os.path.join(os.path.dirname(__file__), 'keycert3.pem')
+certfile = os.path.join(os.path.dirname(__file__), 'certdata', 'keycert3.pem')
 
 if ssl is not None:
     SSLError = ssl.SSLError
 else:
     class SSLError(Exception):
         """Non-existent exception class when we lack SSL support."""
         reason = "This will never be raised."
@@ -1589,16 +1589,15 @@
         port = socket_helper.bind_port(sock)
         sock.listen()
         self.background = threading.Thread(
             target=self.run_server, args=(sock,))
         self.background.start()
         self.addCleanup(self.background.join)
 
-        self.nntp = NNTP(socket_helper.HOST, port, usenetrc=False).__enter__()
-        self.addCleanup(self.nntp.__exit__, None, None, None)
+        self.nntp = self.enterContext(NNTP(socket_helper.HOST, port, usenetrc=False))
 
     def run_server(self, sock):
         # Could be generalized to handle more commands in separate methods
         with sock:
             [client, _] = sock.accept()
         with contextlib.ExitStack() as cleanup:
             cleanup.enter_context(client)
```


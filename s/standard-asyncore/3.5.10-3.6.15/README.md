# Comparing `tmp/standard_asyncore-3.5.10.tar.gz` & `tmp/standard_asyncore-3.6.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_asyncore-3.5.10.tar", last modified: Sun Apr 21 16:42:33 2024, max compression
+gzip compressed data, was "standard_asyncore-3.6.15.tar", last modified: Sun Apr 21 17:08:04 2024, max compression
```

## Comparing `standard_asyncore-3.5.10.tar` & `standard_asyncore-3.6.15.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 16:42:33.106927 standard_asyncore-3.5.10/
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_asyncore-3.5.10/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     3477 2024-04-21 16:42:33.106671 standard_asyncore-3.5.10/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)    13565 2024-04-21 16:42:22.000000 standard_asyncore-3.5.10/README.rst
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 16:42:33.104912 standard_asyncore-3.5.10/asyncore/
--rw-r--r--   0 user       (501) staff       (20)    20104 2024-04-21 16:42:22.000000 standard_asyncore-3.5.10/asyncore/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      718 2024-04-21 16:42:22.000000 standard_asyncore-3.5.10/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 16:42:33.106969 standard_asyncore-3.5.10/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 16:42:33.106438 standard_asyncore-3.5.10/standard_asyncore.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3477 2024-04-21 16:42:33.000000 standard_asyncore-3.5.10/standard_asyncore.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      241 2024-04-21 16:42:33.000000 standard_asyncore-3.5.10/standard_asyncore.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 16:42:33.000000 standard_asyncore-3.5.10/standard_asyncore.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        9 2024-04-21 16:42:33.000000 standard_asyncore-3.5.10/standard_asyncore.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 16:42:33.105661 standard_asyncore-3.5.10/tests/
--rw-r--r--   0 user       (501) staff       (20)    26571 2024-04-21 16:42:22.000000 standard_asyncore-3.5.10/tests/test_asyncore.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 17:08:04.218360 standard_asyncore-3.6.15/
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_asyncore-3.6.15/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     3812 2024-04-21 17:08:04.218156 standard_asyncore-3.6.15/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_asyncore-3.6.15/README.rst
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 17:08:04.217091 standard_asyncore-3.6.15/asyncore/
+-rw-r--r--   0 user       (501) staff       (20)    20159 2024-04-21 17:08:00.000000 standard_asyncore-3.6.15/asyncore/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      714 2024-04-21 17:08:00.000000 standard_asyncore-3.6.15/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 17:08:04.218404 standard_asyncore-3.6.15/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 17:08:04.217947 standard_asyncore-3.6.15/standard_asyncore.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3812 2024-04-21 17:08:04.000000 standard_asyncore-3.6.15/standard_asyncore.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      241 2024-04-21 17:08:04.000000 standard_asyncore-3.6.15/standard_asyncore.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 17:08:04.000000 standard_asyncore-3.6.15/standard_asyncore.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        9 2024-04-21 17:08:04.000000 standard_asyncore-3.6.15/standard_asyncore.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 17:08:04.217744 standard_asyncore-3.6.15/tests/
+-rw-r--r--   0 user       (501) staff       (20)    26912 2024-04-21 17:08:00.000000 standard_asyncore-3.6.15/tests/test_asyncore.py
```

### Comparing `standard_asyncore-3.5.10/LICENSE` & `standard_asyncore-3.6.15/LICENSE`

 * *Files identical despite different names*

### Comparing `standard_asyncore-3.5.10/PKG-INFO` & `standard_asyncore-3.6.15/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: standard-asyncore
-Version: 3.5.10
-Summary: Standard library asyncore redistribution as dead battery.
+Version: 3.6.15
+Summary: Standard library asyncore redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
         
@@ -55,7 +55,16 @@
 Project-URL: Homepage, https://github.com/youknowone/python-deadlib
 Keywords: stdlib
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+
+Dead battery redistribution
+===========================
+
+Python is moving forward! Python finally started to remove dead batteries.
+For more information, see `PEP 594 <https://peps.python.org/pep-0594/>`_.
+
+If your project depends on a module that has been removed from the standard,
+here is the redistribution of the dead batteries.
```

### Comparing `standard_asyncore-3.5.10/asyncore/__init__.py` & `standard_asyncore-3.6.15/asyncore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,15 +329,15 @@
         return self.socket.bind(addr)
 
     def connect(self, address):
         self.connected = False
         self.connecting = True
         err = self.socket.connect_ex(address)
         if err in (EINPROGRESS, EALREADY, EWOULDBLOCK) \
-        or err == EINVAL and os.name in ('nt', 'ce'):
+        or err == EINVAL and os.name == 'nt':
             self.addr = address
             return
         if err in (0, EISCONN):
             self.addr = address
             self.handle_connect_event()
         else:
             raise OSError(err, errorcode[err])
@@ -591,15 +591,16 @@
         # The passed fd is automatically os.dup()'d
 
         def __init__(self, fd):
             self.fd = os.dup(fd)
 
         def __del__(self):
             if self.fd >= 0:
-                warnings.warn("unclosed file %r" % self, ResourceWarning)
+                warnings.warn("unclosed file %r" % self, ResourceWarning,
+                              source=self)
             self.close()
 
         def recv(self, *args):
             return os.read(self.fd, *args)
 
         def send(self, *args):
             return os.write(self.fd, *args)
@@ -614,16 +615,17 @@
 
         read = recv
         write = send
 
         def close(self):
             if self.fd < 0:
                 return
-            os.close(self.fd)
+            fd = self.fd
             self.fd = -1
+            os.close(fd)
 
         def fileno(self):
             return self.fd
 
     class file_dispatcher(dispatcher):
 
         def __init__(self, fd, map=None):
```

### Comparing `standard_asyncore-3.5.10/pyproject.toml` & `standard_asyncore-3.6.15/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "standard-asyncore"
-version = "3.5.10"
-description = "Standard library asyncore redistribution as dead battery."
+version = "3.6.15"
+description = "Standard library asyncore redistribution. \"dead battery\"."
 keywords = ["stdlib"]
 authors = [
     { name = "Python Devleopers", email = "python-deadlib@youknowone.org" }
 ]
-readme = "Doc/asyncore.rst"
+readme = "README.rst"
 license = {name = "PSF", file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: Python Software Foundation License",
     "Topic :: Software Development :: Libraries",
     "Programming Language :: Python :: 3",
 ]
```

### Comparing `standard_asyncore-3.5.10/standard_asyncore.egg-info/PKG-INFO` & `standard_asyncore-3.6.15/standard_asyncore.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: standard-asyncore
-Version: 3.5.10
-Summary: Standard library asyncore redistribution as dead battery.
+Version: 3.6.15
+Summary: Standard library asyncore redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
         
@@ -55,7 +55,16 @@
 Project-URL: Homepage, https://github.com/youknowone/python-deadlib
 Keywords: stdlib
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+
+Dead battery redistribution
+===========================
+
+Python is moving forward! Python finally started to remove dead batteries.
+For more information, see `PEP 594 <https://peps.python.org/pep-0594/>`_.
+
+If your project depends on a module that has been removed from the standard,
+here is the redistribution of the dead batteries.
```

### Comparing `standard_asyncore-3.5.10/tests/test_asyncore.py` & `standard_asyncore-3.6.15/tests/test_asyncore.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 import time
 import errno
 import struct
 
 from test import support
 from io import BytesIO
 
+if support.PGO:
+    raise unittest.SkipTest("test is not helpful for PGO")
+
 try:
     import threading
 except ImportError:
     threading = None
 
 TIMEOUT = 3
 HAS_UNIX_SOCKETS = hasattr(socket, 'AF_UNIX')
@@ -88,15 +91,17 @@
         evt.set()
 
 def bind_af_aware(sock, addr):
     """Helper function to bind a socket according to its family."""
     if HAS_UNIX_SOCKETS and sock.family == socket.AF_UNIX:
         # Make sure the path doesn't exist.
         support.unlink(addr)
-    sock.bind(addr)
+        support.bind_unix_socket(sock, addr)
+    else:
+        sock.bind(addr)
 
 
 class HelperFunctionTests(unittest.TestCase):
     def test_readwriteexc(self):
         # Check exception handling behavior of read, write and _exception
 
         # check that ExitNow exceptions in the object handler method
@@ -424,15 +429,18 @@
             support.gc_collect()
 
     def test_close_twice(self):
         fd = os.open(support.TESTFN, os.O_RDONLY)
         f = asyncore.file_wrapper(fd)
         os.close(fd)
 
-        f.close()
+        os.close(f.fd)  # file_wrapper dupped fd
+        with self.assertRaises(OSError):
+            f.close()
+
         self.assertEqual(f.fd, -1)
         # calling close twice should not fail
         f.close()
 
 
 class BaseTestHandler(asyncore.dispatcher):
 
@@ -493,15 +501,15 @@
     def handle_connect(self):
         pass
 
 
 class BaseTestAPI:
 
     def tearDown(self):
-        asyncore.close_all()
+        asyncore.close_all(ignore_all=True)
 
     def loop_waiting_for_flag(self, instance, timeout=5):
         timeout = float(timeout) / 100
         count = 100
         while asyncore.socket_map and count > 0:
             asyncore.loop(timeout=0.01, count=1, use_poll=self.use_poll)
             if instance.flag:
@@ -746,58 +754,58 @@
         s2.create_socket(self.family)
         # EADDRINUSE indicates the socket was correctly bound
         self.assertRaises(OSError, s2.bind, (self.addr[0], port))
 
     def test_set_reuse_addr(self):
         if HAS_UNIX_SOCKETS and self.family == socket.AF_UNIX:
             self.skipTest("Not applicable to AF_UNIX sockets.")
-        sock = socket.socket(self.family)
-        try:
-            sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        except OSError:
-            unittest.skip("SO_REUSEADDR not supported on this platform")
-        else:
-            # if SO_REUSEADDR succeeded for sock we expect asyncore
-            # to do the same
-            s = asyncore.dispatcher(socket.socket(self.family))
-            self.assertFalse(s.socket.getsockopt(socket.SOL_SOCKET,
-                                                 socket.SO_REUSEADDR))
-            s.socket.close()
-            s.create_socket(self.family)
-            s.set_reuse_addr()
-            self.assertTrue(s.socket.getsockopt(socket.SOL_SOCKET,
-                                                 socket.SO_REUSEADDR))
-        finally:
-            sock.close()
+
+        with socket.socket(self.family) as sock:
+            try:
+                sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            except OSError:
+                unittest.skip("SO_REUSEADDR not supported on this platform")
+            else:
+                # if SO_REUSEADDR succeeded for sock we expect asyncore
+                # to do the same
+                s = asyncore.dispatcher(socket.socket(self.family))
+                self.assertFalse(s.socket.getsockopt(socket.SOL_SOCKET,
+                                                     socket.SO_REUSEADDR))
+                s.socket.close()
+                s.create_socket(self.family)
+                s.set_reuse_addr()
+                self.assertTrue(s.socket.getsockopt(socket.SOL_SOCKET,
+                                                     socket.SO_REUSEADDR))
 
     @unittest.skipUnless(threading, 'Threading required for this test.')
     @support.reap_threads
     def test_quick_connect(self):
         # see: http://bugs.python.org/issue10340
-        if self.family in (socket.AF_INET, getattr(socket, "AF_INET6", object())):
-            server = BaseServer(self.family, self.addr)
-            t = threading.Thread(target=lambda: asyncore.loop(timeout=0.1,
-                                                              count=500))
-            t.start()
-            def cleanup():
-                t.join(timeout=TIMEOUT)
-                if t.is_alive():
-                    self.fail("join() timed out")
-            self.addCleanup(cleanup)
-
-            s = socket.socket(self.family, socket.SOCK_STREAM)
-            s.settimeout(.2)
-            s.setsockopt(socket.SOL_SOCKET, socket.SO_LINGER,
-                         struct.pack('ii', 1, 0))
-            try:
-                s.connect(server.address)
-            except OSError:
-                pass
-            finally:
-                s.close()
+        if self.family not in (socket.AF_INET, getattr(socket, "AF_INET6", object())):
+            self.skipTest("test specific to AF_INET and AF_INET6")
+
+        server = BaseServer(self.family, self.addr)
+        # run the thread 500 ms: the socket should be connected in 200 ms
+        t = threading.Thread(target=lambda: asyncore.loop(timeout=0.1,
+                                                          count=5))
+        t.start()
+        try:
+            with socket.socket(self.family, socket.SOCK_STREAM) as s:
+                s.settimeout(.2)
+                s.setsockopt(socket.SOL_SOCKET, socket.SO_LINGER,
+                             struct.pack('ii', 1, 0))
+
+                try:
+                    s.connect(server.address)
+                except OSError:
+                    pass
+        finally:
+            t.join(timeout=TIMEOUT)
+            if t.is_alive():
+                self.fail("join() timed out")
 
 class TestAPI_UseIPv4Sockets(BaseTestAPI):
     family = socket.AF_INET
     addr = (support.HOST, 0)
 
 @unittest.skipUnless(support.IPV6_ENABLED, 'IPv6 support required')
 class TestAPI_UseIPv6Sockets(BaseTestAPI):
```


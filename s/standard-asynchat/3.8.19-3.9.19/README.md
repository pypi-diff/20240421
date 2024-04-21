# Comparing `tmp/standard_asynchat-3.8.19.tar.gz` & `tmp/standard_asynchat-3.9.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_asynchat-3.8.19.tar", last modified: Sun Apr 21 18:36:47 2024, max compression
+gzip compressed data, was "standard_asynchat-3.9.19.tar", last modified: Sun Apr 21 18:38:43 2024, max compression
```

## Comparing `standard_asynchat-3.8.19.tar` & `standard_asynchat-3.9.19.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:36:47.447581 standard_asynchat-3.8.19/
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_asynchat-3.8.19/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     3812 2024-04-21 18:36:47.447343 standard_asynchat-3.8.19/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 18:32:37.000000 standard_asynchat-3.8.19/README.rst
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:36:47.446107 standard_asynchat-3.8.19/asynchat/
--rw-r--r--   0 user       (501) staff       (20)    11328 2024-04-21 18:36:44.000000 standard_asynchat-3.8.19/asynchat/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      714 2024-04-21 18:36:43.000000 standard_asynchat-3.8.19/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 18:36:47.447625 standard_asynchat-3.8.19/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:36:47.447086 standard_asynchat-3.8.19/standard_asynchat.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3812 2024-04-21 18:36:47.000000 standard_asynchat-3.8.19/standard_asynchat.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      241 2024-04-21 18:36:47.000000 standard_asynchat-3.8.19/standard_asynchat.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 18:36:47.000000 standard_asynchat-3.8.19/standard_asynchat.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        9 2024-04-21 18:36:47.000000 standard_asynchat-3.8.19/standard_asynchat.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:36:47.446826 standard_asynchat-3.8.19/tests/
--rw-r--r--   0 user       (501) staff       (20)     9507 2024-04-21 18:36:44.000000 standard_asynchat-3.8.19/tests/test_asynchat.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:38:43.398893 standard_asynchat-3.9.19/
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_asynchat-3.9.19/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     3812 2024-04-21 18:38:43.398664 standard_asynchat-3.9.19/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 18:32:37.000000 standard_asynchat-3.9.19/README.rst
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:38:43.397425 standard_asynchat-3.9.19/asynchat/
+-rw-r--r--   0 user       (501) staff       (20)    11321 2024-04-21 18:38:40.000000 standard_asynchat-3.9.19/asynchat/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      714 2024-04-21 18:38:40.000000 standard_asynchat-3.9.19/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 18:38:43.398933 standard_asynchat-3.9.19/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:38:43.398408 standard_asynchat-3.9.19/standard_asynchat.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3812 2024-04-21 18:38:43.000000 standard_asynchat-3.9.19/standard_asynchat.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      241 2024-04-21 18:38:43.000000 standard_asynchat-3.9.19/standard_asynchat.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 18:38:43.000000 standard_asynchat-3.9.19/standard_asynchat.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        9 2024-04-21 18:38:43.000000 standard_asynchat-3.9.19/standard_asynchat.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:38:43.398197 standard_asynchat-3.9.19/tests/
+-rw-r--r--   0 user       (501) staff       (20)     9380 2024-04-21 18:38:40.000000 standard_asynchat-3.9.19/tests/test_asynchat.py
```

### Comparing `standard_asynchat-3.8.19/LICENSE` & `standard_asynchat-3.9.19/LICENSE`

 * *Files identical despite different names*

### Comparing `standard_asynchat-3.8.19/PKG-INFO` & `standard_asynchat-3.9.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-asynchat
-Version: 3.8.19
+Version: 3.9.19
 Summary: Standard library asynchat redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_asynchat-3.8.19/asynchat/__init__.py` & `standard_asynchat-3.9.19/asynchat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
     def handle_read(self):
 
         try:
             data = self.recv(self.ac_in_buffer_size)
         except BlockingIOError:
             return
-        except OSError as why:
+        except OSError:
             self.handle_error()
             return
 
         if isinstance(data, str) and self.use_encoding:
             data = bytes(str, self.encoding)
         self.ac_in_buffer = self.ac_in_buffer + data
```

### Comparing `standard_asynchat-3.8.19/pyproject.toml` & `standard_asynchat-3.9.19/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "standard-asynchat"
-version = "3.8.19"
+version = "3.9.19"
 description = "Standard library asynchat redistribution. \"dead battery\"."
 keywords = ["stdlib"]
 authors = [
     { name = "Python Devleopers", email = "python-deadlib@youknowone.org" }
 ]
 readme = "README.rst"
 license = {name = "PSF", file = "LICENSE"}
```

### Comparing `standard_asynchat-3.8.19/standard_asynchat.egg-info/PKG-INFO` & `standard_asynchat-3.9.19/standard_asynchat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-asynchat
-Version: 3.8.19
+Version: 3.9.19
 Summary: Standard library asynchat redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_asynchat-3.8.19/tests/test_asynchat.py` & `standard_asynchat-3.9.19/tests/test_asynchat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # test asynchat
 
 from test import support
+from test.support import socket_helper
 
 import asynchat
 import asyncore
 import errno
 import socket
 import sys
 import threading
 import time
 import unittest
 import unittest.mock
 
-HOST = support.HOST
+HOST = socket_helper.HOST
 SERVER_QUIT = b'QUIT\n'
-TIMEOUT = 3.0
 
 
 class echo_server(threading.Thread):
     # parameter to determine the number of bytes passed back to the
     # client each send
     chunk_size = 1
 
     def __init__(self, event):
         threading.Thread.__init__(self)
         self.event = event
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.port = support.bind_port(self.sock)
+        self.port = socket_helper.bind_port(self.sock)
         # This will be set if the client wants us to wait before echoing
         # data back.
         self.start_resend_event = None
 
     def run(self):
         self.sock.listen()
         self.event.set()
@@ -69,22 +69,22 @@
         asynchat.async_chat.__init__(self)
         self.contents = []
         self.create_socket(socket.AF_INET, socket.SOCK_STREAM)
         self.connect((HOST, server_port))
         self.set_terminator(terminator)
         self.buffer = b""
 
-        def handle_connect(self):
-            pass
+    def handle_connect(self):
+        pass
 
-        if sys.platform == 'darwin':
-            # select.poll returns a select.POLLHUP at the end of the tests
-            # on darwin, so just ignore it
-            def handle_expt(self):
-                pass
+    if sys.platform == 'darwin':
+        # select.poll returns a select.POLLHUP at the end of the tests
+        # on darwin, so just ignore it
+        def handle_expt(self):
+            pass
 
     def collect_incoming_data(self, data):
         self.buffer += data
 
     def found_terminator(self):
         self.contents.append(self.buffer)
         self.buffer = b""
@@ -118,15 +118,15 @@
         time.sleep(0.01)   # Give server time to start accepting.
         c = echo_client(term, s.port)
         c.push(b"hello ")
         c.push(b"world" + term)
         c.push(b"I'm not dead yet!" + term)
         c.push(SERVER_QUIT)
         asyncore.loop(use_poll=self.usepoll, count=300, timeout=.01)
-        support.join_thread(s, timeout=TIMEOUT)
+        support.join_thread(s)
 
         self.assertEqual(c.contents, [b"hello world", b"I'm not dead yet!"])
 
     # the line terminator tests below check receiving variously-sized
     # chunks back from the server in order to exercise all branches of
     # async_chat.handle_read
 
@@ -149,15 +149,15 @@
         # Try reading a fixed number of bytes
         s, event = start_echo_server()
         c = echo_client(termlen, s.port)
         data = b"hello world, I'm not dead yet!\n"
         c.push(data)
         c.push(SERVER_QUIT)
         asyncore.loop(use_poll=self.usepoll, count=300, timeout=.01)
-        support.join_thread(s, timeout=TIMEOUT)
+        support.join_thread(s)
 
         self.assertEqual(c.contents, [data[:termlen]])
 
     def test_numeric_terminator1(self):
         # check that ints & longs both work (since type is
         # explicitly checked in async_chat.handle_read)
         self.numeric_terminator_check(1)
@@ -169,48 +169,48 @@
         # Try reading a fixed number of bytes
         s, event = start_echo_server()
         c = echo_client(None, s.port)
         data = b"hello world, I'm not dead yet!\n"
         c.push(data)
         c.push(SERVER_QUIT)
         asyncore.loop(use_poll=self.usepoll, count=300, timeout=.01)
-        support.join_thread(s, timeout=TIMEOUT)
+        support.join_thread(s)
 
         self.assertEqual(c.contents, [])
         self.assertEqual(c.buffer, data)
 
     def test_simple_producer(self):
         s, event = start_echo_server()
         c = echo_client(b'\n', s.port)
         data = b"hello world\nI'm not dead yet!\n"
         p = asynchat.simple_producer(data+SERVER_QUIT, buffer_size=8)
         c.push_with_producer(p)
         asyncore.loop(use_poll=self.usepoll, count=300, timeout=.01)
-        support.join_thread(s, timeout=TIMEOUT)
+        support.join_thread(s)
 
         self.assertEqual(c.contents, [b"hello world", b"I'm not dead yet!"])
 
     def test_string_producer(self):
         s, event = start_echo_server()
         c = echo_client(b'\n', s.port)
         data = b"hello world\nI'm not dead yet!\n"
         c.push_with_producer(data+SERVER_QUIT)
         asyncore.loop(use_poll=self.usepoll, count=300, timeout=.01)
-        support.join_thread(s, timeout=TIMEOUT)
+        support.join_thread(s)
 
         self.assertEqual(c.contents, [b"hello world", b"I'm not dead yet!"])
 
     def test_empty_line(self):
         # checks that empty lines are handled correctly
         s, event = start_echo_server()
         c = echo_client(b'\n', s.port)
         c.push(b"hello world\n\nI'm not dead yet!\n")
         c.push(SERVER_QUIT)
         asyncore.loop(use_poll=self.usepoll, count=300, timeout=.01)
-        support.join_thread(s, timeout=TIMEOUT)
+        support.join_thread(s)
 
         self.assertEqual(c.contents,
                          [b"hello world", b"", b"I'm not dead yet!"])
 
     def test_close_when_done(self):
         s, event = start_echo_server()
         s.start_resend_event = threading.Event()
@@ -221,15 +221,15 @@
         asyncore.loop(use_poll=self.usepoll, count=300, timeout=.01)
 
         # Only allow the server to start echoing data back to the client after
         # the client has closed its connection.  This prevents a race condition
         # where the server echoes all of its data before we can check that it
         # got any down below.
         s.start_resend_event.set()
-        support.join_thread(s, timeout=TIMEOUT)
+        support.join_thread(s)
 
         self.assertEqual(c.contents, [])
         # the server might have been able to send a byte or two back, but this
         # at least checks that it received something and didn't just fail
         # (which could still result in the client not having received anything)
         self.assertGreater(len(s.buffer), 0)
 
@@ -242,15 +242,15 @@
         c.push(data)
         c.push(bytearray(data))
         c.push(memoryview(data))
         self.assertRaises(TypeError, c.push, 10)
         self.assertRaises(TypeError, c.push, 'unicode')
         c.push(SERVER_QUIT)
         asyncore.loop(use_poll=self.usepoll, count=300, timeout=.01)
-        support.join_thread(s, timeout=TIMEOUT)
+        support.join_thread(s)
         self.assertEqual(c.contents, [b'bytes', b'bytes', b'bytes'])
 
 
 class TestAsynchat_WithPoll(TestAsynchat):
     usepoll = True
```


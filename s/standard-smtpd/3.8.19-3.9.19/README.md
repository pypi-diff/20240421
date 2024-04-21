# Comparing `tmp/standard_smtpd-3.8.19.tar.gz` & `tmp/standard_smtpd-3.9.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_smtpd-3.8.19.tar", last modified: Sun Apr 21 18:36:55 2024, max compression
+gzip compressed data, was "standard_smtpd-3.9.19.tar", last modified: Sun Apr 21 18:38:22 2024, max compression
```

## Comparing `standard_smtpd-3.8.19.tar` & `standard_smtpd-3.9.19.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:36:55.362932 standard_smtpd-3.8.19/
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_smtpd-3.8.19/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     3806 2024-04-21 18:36:55.362704 standard_smtpd-3.8.19/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 18:32:37.000000 standard_smtpd-3.8.19/README.rst
--rw-r--r--   0 user       (501) staff       (20)      705 2024-04-21 18:36:53.000000 standard_smtpd-3.8.19/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 18:36:55.362974 standard_smtpd-3.8.19/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:36:55.361428 standard_smtpd-3.8.19/smtpd/
--rwxr-xr-x   0 user       (501) staff       (20)    34711 2024-04-21 18:36:53.000000 standard_smtpd-3.8.19/smtpd/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:36:55.362445 standard_smtpd-3.8.19/standard_smtpd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3806 2024-04-21 18:36:55.000000 standard_smtpd-3.8.19/standard_smtpd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      223 2024-04-21 18:36:55.000000 standard_smtpd-3.8.19/standard_smtpd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 18:36:55.000000 standard_smtpd-3.8.19/standard_smtpd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        6 2024-04-21 18:36:55.000000 standard_smtpd-3.8.19/standard_smtpd.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:36:55.362209 standard_smtpd-3.8.19/tests/
--rw-r--r--   0 user       (501) staff       (20)    41108 2024-04-21 18:36:53.000000 standard_smtpd-3.8.19/tests/test_smtpd.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:38:22.365775 standard_smtpd-3.9.19/
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_smtpd-3.9.19/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     3806 2024-04-21 18:38:22.365543 standard_smtpd-3.9.19/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 18:32:37.000000 standard_smtpd-3.9.19/README.rst
+-rw-r--r--   0 user       (501) staff       (20)      705 2024-04-21 18:38:18.000000 standard_smtpd-3.9.19/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 18:38:22.365817 standard_smtpd-3.9.19/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:38:22.364395 standard_smtpd-3.9.19/smtpd/
+-rwxr-xr-x   0 user       (501) staff       (20)    34823 2024-04-21 18:38:19.000000 standard_smtpd-3.9.19/smtpd/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:38:22.365305 standard_smtpd-3.9.19/standard_smtpd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3806 2024-04-21 18:38:22.000000 standard_smtpd-3.9.19/standard_smtpd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      223 2024-04-21 18:38:22.000000 standard_smtpd-3.9.19/standard_smtpd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 18:38:22.000000 standard_smtpd-3.9.19/standard_smtpd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        6 2024-04-21 18:38:22.000000 standard_smtpd-3.9.19/standard_smtpd.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:38:22.365084 standard_smtpd-3.9.19/tests/
+-rw-r--r--   0 user       (501) staff       (20)    41291 2024-04-21 18:38:19.000000 standard_smtpd-3.9.19/tests/test_smtpd.py
```

### Comparing `standard_smtpd-3.8.19/LICENSE` & `standard_smtpd-3.9.19/LICENSE`

 * *Files identical despite different names*

### Comparing `standard_smtpd-3.8.19/PKG-INFO` & `standard_smtpd-3.9.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-smtpd
-Version: 3.8.19
+Version: 3.9.19
 Summary: Standard library smtpd redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_smtpd-3.8.19/pyproject.toml` & `standard_smtpd-3.9.19/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "standard-smtpd"
-version = "3.8.19"
+version = "3.9.19"
 description = "Standard library smtpd redistribution. \"dead battery\"."
 keywords = ["stdlib"]
 authors = [
     { name = "Python Devleopers", email = "python-deadlib@youknowone.org" }
 ]
 readme = "README.rst"
 license = {name = "PSF", file = "LICENSE"}
```

### Comparing `standard_smtpd-3.8.19/smtpd/__init__.py` & `standard_smtpd-3.9.19/smtpd/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -775,14 +775,16 @@
             for r in rcpttos:
                 refused[r] = (errcode, errmsg)
         return refused
 
 
 class MailmanProxy(PureProxy):
     def __init__(self, *args, **kwargs):
+        warn('MailmanProxy is deprecated and will be removed '
+             'in future', DeprecationWarning, 2)
         if 'enable_SMTPUTF8' in kwargs and kwargs['enable_SMTPUTF8']:
             raise ValueError("MailmanProxy does not support SMTPUTF8.")
         super(PureProxy, self).__init__(*args, **kwargs)
 
     def process_message(self, peer, mailfrom, rcpttos, data):
         from io import StringIO
         from Mailman import Utils
```

### Comparing `standard_smtpd-3.8.19/standard_smtpd.egg-info/PKG-INFO` & `standard_smtpd-3.9.19/standard_smtpd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-smtpd
-Version: 3.8.19
+Version: 3.9.19
 Summary: Standard library smtpd redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_smtpd-3.8.19/tests/test_smtpd.py` & `standard_smtpd-3.9.19/tests/test_smtpd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import unittest
 import textwrap
 from test import support, mock_socket
+from test.support import socket_helper
 import socket
 import io
 import smtpd
 import asyncore
 
 
 class DummyServer(smtpd.SMTPServer):
@@ -34,15 +35,15 @@
 
 
 class SMTPDServerTest(unittest.TestCase):
     def setUp(self):
         smtpd.socket = asyncore.socket = mock_socket
 
     def test_process_message_unimplemented(self):
-        server = smtpd.SMTPServer((support.HOST, 0), ('b', 0),
+        server = smtpd.SMTPServer((socket_helper.HOST, 0), ('b', 0),
                                   decode_data=True)
         conn, addr = server.accept()
         channel = smtpd.SMTPChannel(server, conn, addr, decode_data=True)
 
         def write_line(line):
             channel.socket.queue_recv(line)
             channel.handle_read()
@@ -53,15 +54,15 @@
         write_line(b'DATA')
         self.assertRaises(NotImplementedError, write_line, b'spam\r\n.\r\n')
 
     def test_decode_data_and_enable_SMTPUTF8_raises(self):
         self.assertRaises(
             ValueError,
             smtpd.SMTPServer,
-            (support.HOST, 0),
+            (socket_helper.HOST, 0),
             ('b', 0),
             enable_SMTPUTF8=True,
             decode_data=True)
 
     def tearDown(self):
         asyncore.close_all()
         asyncore.socket = smtpd.socket = socket
@@ -83,15 +84,15 @@
             write_line(b'MAIL From:eggs@example')
         write_line(b'RCPT To:spam@example')
         write_line(b'DATA')
         write_line(data)
         write_line(b'.')
 
     def test_process_message_with_decode_data_true(self):
-        server = smtpd.DebuggingServer((support.HOST, 0), ('b', 0),
+        server = smtpd.DebuggingServer((socket_helper.HOST, 0), ('b', 0),
                                        decode_data=True)
         conn, addr = server.accept()
         channel = smtpd.SMTPChannel(server, conn, addr, decode_data=True)
         with support.captured_stdout() as s:
             self.send_data(channel, b'From: test\n\nhello\n')
         stdout = s.getvalue()
         self.assertEqual(stdout, textwrap.dedent("""\
@@ -100,15 +101,15 @@
              X-Peer: peer-address
 
              hello
              ------------ END MESSAGE ------------
              """))
 
     def test_process_message_with_decode_data_false(self):
-        server = smtpd.DebuggingServer((support.HOST, 0), ('b', 0))
+        server = smtpd.DebuggingServer((socket_helper.HOST, 0), ('b', 0))
         conn, addr = server.accept()
         channel = smtpd.SMTPChannel(server, conn, addr)
         with support.captured_stdout() as s:
             self.send_data(channel, b'From: test\n\nh\xc3\xa9llo\xff\n')
         stdout = s.getvalue()
         self.assertEqual(stdout, textwrap.dedent("""\
              ---------- MESSAGE FOLLOWS ----------
@@ -116,15 +117,15 @@
              b'X-Peer: peer-address'
              b''
              b'h\\xc3\\xa9llo\\xff'
              ------------ END MESSAGE ------------
              """))
 
     def test_process_message_with_enable_SMTPUTF8_true(self):
-        server = smtpd.DebuggingServer((support.HOST, 0), ('b', 0),
+        server = smtpd.DebuggingServer((socket_helper.HOST, 0), ('b', 0),
                                        enable_SMTPUTF8=True)
         conn, addr = server.accept()
         channel = smtpd.SMTPChannel(server, conn, addr, enable_SMTPUTF8=True)
         with support.captured_stdout() as s:
             self.send_data(channel, b'From: test\n\nh\xc3\xa9llo\xff\n')
         stdout = s.getvalue()
         self.assertEqual(stdout, textwrap.dedent("""\
@@ -133,15 +134,15 @@
              b'X-Peer: peer-address'
              b''
              b'h\\xc3\\xa9llo\\xff'
              ------------ END MESSAGE ------------
              """))
 
     def test_process_SMTPUTF8_message_with_enable_SMTPUTF8_true(self):
-        server = smtpd.DebuggingServer((support.HOST, 0), ('b', 0),
+        server = smtpd.DebuggingServer((socket_helper.HOST, 0), ('b', 0),
                                        enable_SMTPUTF8=True)
         conn, addr = server.accept()
         channel = smtpd.SMTPChannel(server, conn, addr, enable_SMTPUTF8=True)
         with support.captured_stdout() as s:
             self.send_data(channel, b'From: test\n\nh\xc3\xa9llo\xff\n',
                            enable_SMTPUTF8=True)
         stdout = s.getvalue()
@@ -164,21 +165,21 @@
     def setUp(self):
         smtpd.socket = asyncore.socket = mock_socket
 
     def tearDown(self):
         asyncore.close_all()
         asyncore.socket = smtpd.socket = socket
 
-    @unittest.skipUnless(support.IPV6_ENABLED, "IPv6 not enabled")
+    @unittest.skipUnless(socket_helper.IPV6_ENABLED, "IPv6 not enabled")
     def test_socket_uses_IPv6(self):
-        server = smtpd.SMTPServer((support.HOSTv6, 0), (support.HOSTv4, 0))
+        server = smtpd.SMTPServer((socket_helper.HOSTv6, 0), (socket_helper.HOSTv4, 0))
         self.assertEqual(server.socket.family, socket.AF_INET6)
 
     def test_socket_uses_IPv4(self):
-        server = smtpd.SMTPServer((support.HOSTv4, 0), (support.HOSTv6, 0))
+        server = smtpd.SMTPServer((socket_helper.HOSTv4, 0), (socket_helper.HOSTv6, 0))
         self.assertEqual(server.socket.family, socket.AF_INET)
 
 
 class TestRcptOptionParsing(unittest.TestCase):
     error_response = (b'555 RCPT TO parameters not recognized or not '
                       b'implemented\r\n')
 
@@ -193,24 +194,24 @@
         smtpd.DEBUGSTREAM = self.old_debugstream
 
     def write_line(self, channel, line):
         channel.socket.queue_recv(line)
         channel.handle_read()
 
     def test_params_rejected(self):
-        server = DummyServer((support.HOST, 0), ('b', 0))
+        server = DummyServer((socket_helper.HOST, 0), ('b', 0))
         conn, addr = server.accept()
         channel = smtpd.SMTPChannel(server, conn, addr)
         self.write_line(channel, b'EHLO example')
         self.write_line(channel, b'MAIL from: <foo@example.com> size=20')
         self.write_line(channel, b'RCPT to: <foo@example.com> foo=bar')
         self.assertEqual(channel.socket.last, self.error_response)
 
     def test_nothing_accepted(self):
-        server = DummyServer((support.HOST, 0), ('b', 0))
+        server = DummyServer((socket_helper.HOST, 0), ('b', 0))
         conn, addr = server.accept()
         channel = smtpd.SMTPChannel(server, conn, addr)
         self.write_line(channel, b'EHLO example')
         self.write_line(channel, b'MAIL from: <foo@example.com> size=20')
         self.write_line(channel, b'RCPT to: <foo@example.com>')
         self.assertEqual(channel.socket.last, b'250 OK\r\n')
 
@@ -230,15 +231,15 @@
         smtpd.DEBUGSTREAM = self.old_debugstream
 
     def write_line(self, channel, line):
         channel.socket.queue_recv(line)
         channel.handle_read()
 
     def test_with_decode_data_true(self):
-        server = DummyServer((support.HOST, 0), ('b', 0), decode_data=True)
+        server = DummyServer((socket_helper.HOST, 0), ('b', 0), decode_data=True)
         conn, addr = server.accept()
         channel = smtpd.SMTPChannel(server, conn, addr, decode_data=True)
         self.write_line(channel, b'EHLO example')
         for line in [
             b'MAIL from: <foo@example.com> size=20 SMTPUTF8',
             b'MAIL from: <foo@example.com> size=20 SMTPUTF8 BODY=8BITMIME',
             b'MAIL from: <foo@example.com> size=20 BODY=UNKNOWN',
@@ -246,15 +247,15 @@
         ]:
             self.write_line(channel, line)
             self.assertEqual(channel.socket.last, self.error_response)
         self.write_line(channel, b'MAIL from: <foo@example.com> size=20')
         self.assertEqual(channel.socket.last, b'250 OK\r\n')
 
     def test_with_decode_data_false(self):
-        server = DummyServer((support.HOST, 0), ('b', 0))
+        server = DummyServer((socket_helper.HOST, 0), ('b', 0))
         conn, addr = server.accept()
         channel = smtpd.SMTPChannel(server, conn, addr)
         self.write_line(channel, b'EHLO example')
         for line in [
             b'MAIL from: <foo@example.com> size=20 SMTPUTF8',
             b'MAIL from: <foo@example.com> size=20 SMTPUTF8 BODY=8BITMIME',
         ]:
@@ -267,30 +268,30 @@
             channel.socket.last,
             b'501 Error: BODY can only be one of 7BIT, 8BITMIME\r\n')
         self.write_line(
             channel, b'MAIL from: <foo@example.com> size=20 body=8bitmime')
         self.assertEqual(channel.socket.last, b'250 OK\r\n')
 
     def test_with_enable_smtputf8_true(self):
-        server = DummyServer((support.HOST, 0), ('b', 0), enable_SMTPUTF8=True)
+        server = DummyServer((socket_helper.HOST, 0), ('b', 0), enable_SMTPUTF8=True)
         conn, addr = server.accept()
         channel = smtpd.SMTPChannel(server, conn, addr, enable_SMTPUTF8=True)
         self.write_line(channel, b'EHLO example')
         self.write_line(
             channel,
             b'MAIL from: <foo@example.com> size=20 body=8bitmime smtputf8')
         self.assertEqual(channel.socket.last, b'250 OK\r\n')
 
 
 class SMTPDChannelTest(unittest.TestCase):
     def setUp(self):
         smtpd.socket = asyncore.socket = mock_socket
         self.old_debugstream = smtpd.DEBUGSTREAM
         self.debug = smtpd.DEBUGSTREAM = io.StringIO()
-        self.server = DummyServer((support.HOST, 0), ('b', 0),
+        self.server = DummyServer((socket_helper.HOST, 0), ('b', 0),
                                   decode_data=True)
         conn, addr = self.server.accept()
         self.channel = smtpd.SMTPChannel(self.server, conn, addr,
                                          decode_data=True)
 
     def tearDown(self):
         asyncore.close_all()
@@ -300,15 +301,15 @@
     def write_line(self, line):
         self.channel.socket.queue_recv(line)
         self.channel.handle_read()
 
     def test_broken_connect(self):
         self.assertRaises(
             DummyDispatcherBroken, BrokenDummyServer,
-            (support.HOST, 0), ('b', 0), decode_data=True)
+            (socket_helper.HOST, 0), ('b', 0), decode_data=True)
 
     def test_decode_data_and_enable_SMTPUTF8_raises(self):
         self.assertRaises(
             ValueError, smtpd.SMTPChannel,
             self.server, self.channel.conn, self.channel.addr,
             enable_SMTPUTF8=True, decode_data=True)
 
@@ -754,33 +755,33 @@
         with support.check_warnings(('', DeprecationWarning)):
             self.channel._SMTPChannel__conn = 'spam'
         with support.check_warnings(('', DeprecationWarning)):
             spam = self.channel._SMTPChannel__addr
         with support.check_warnings(('', DeprecationWarning)):
             self.channel._SMTPChannel__addr = 'spam'
 
-@unittest.skipUnless(support.IPV6_ENABLED, "IPv6 not enabled")
+@unittest.skipUnless(socket_helper.IPV6_ENABLED, "IPv6 not enabled")
 class SMTPDChannelIPv6Test(SMTPDChannelTest):
     def setUp(self):
         smtpd.socket = asyncore.socket = mock_socket
         self.old_debugstream = smtpd.DEBUGSTREAM
         self.debug = smtpd.DEBUGSTREAM = io.StringIO()
-        self.server = DummyServer((support.HOSTv6, 0), ('b', 0),
+        self.server = DummyServer((socket_helper.HOSTv6, 0), ('b', 0),
                                   decode_data=True)
         conn, addr = self.server.accept()
         self.channel = smtpd.SMTPChannel(self.server, conn, addr,
                                          decode_data=True)
 
 class SMTPDChannelWithDataSizeLimitTest(unittest.TestCase):
 
     def setUp(self):
         smtpd.socket = asyncore.socket = mock_socket
         self.old_debugstream = smtpd.DEBUGSTREAM
         self.debug = smtpd.DEBUGSTREAM = io.StringIO()
-        self.server = DummyServer((support.HOST, 0), ('b', 0),
+        self.server = DummyServer((socket_helper.HOST, 0), ('b', 0),
                                   decode_data=True)
         conn, addr = self.server.accept()
         # Set DATA size limit to 32 bytes for easy testing
         self.channel = smtpd.SMTPChannel(self.server, conn, addr, 32,
                                          decode_data=True)
 
     def tearDown(self):
@@ -827,15 +828,15 @@
 
 class SMTPDChannelWithDecodeDataFalse(unittest.TestCase):
 
     def setUp(self):
         smtpd.socket = asyncore.socket = mock_socket
         self.old_debugstream = smtpd.DEBUGSTREAM
         self.debug = smtpd.DEBUGSTREAM = io.StringIO()
-        self.server = DummyServer((support.HOST, 0), ('b', 0))
+        self.server = DummyServer((socket_helper.HOST, 0), ('b', 0))
         conn, addr = self.server.accept()
         self.channel = smtpd.SMTPChannel(self.server, conn, addr)
 
     def tearDown(self):
         asyncore.close_all()
         asyncore.socket = smtpd.socket = socket
         smtpd.DEBUGSTREAM = self.old_debugstream
@@ -869,15 +870,15 @@
 
 class SMTPDChannelWithDecodeDataTrue(unittest.TestCase):
 
     def setUp(self):
         smtpd.socket = asyncore.socket = mock_socket
         self.old_debugstream = smtpd.DEBUGSTREAM
         self.debug = smtpd.DEBUGSTREAM = io.StringIO()
-        self.server = DummyServer((support.HOST, 0), ('b', 0),
+        self.server = DummyServer((socket_helper.HOST, 0), ('b', 0),
                                   decode_data=True)
         conn, addr = self.server.accept()
         # Set decode_data to True
         self.channel = smtpd.SMTPChannel(self.server, conn, addr,
                 decode_data=True)
 
     def tearDown(self):
@@ -912,15 +913,15 @@
 
 
 class SMTPDChannelTestWithEnableSMTPUTF8True(unittest.TestCase):
     def setUp(self):
         smtpd.socket = asyncore.socket = mock_socket
         self.old_debugstream = smtpd.DEBUGSTREAM
         self.debug = smtpd.DEBUGSTREAM = io.StringIO()
-        self.server = DummyServer((support.HOST, 0), ('b', 0),
+        self.server = DummyServer((socket_helper.HOST, 0), ('b', 0),
                                   enable_SMTPUTF8=True)
         conn, addr = self.server.accept()
         self.channel = smtpd.SMTPChannel(self.server, conn, addr,
                                          enable_SMTPUTF8=True)
 
     def tearDown(self):
         asyncore.close_all()
```


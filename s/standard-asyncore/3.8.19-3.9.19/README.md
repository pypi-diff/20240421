# Comparing `tmp/standard_asyncore-3.8.19-py3-none-any.whl.zip` & `tmp/standard_asyncore-3.9.19-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 10326 bytes, number of entries: 6
--rw-r--r--  2.0 unx    20094 b- defN 24-Apr-21 18:36 asyncore/__init__.py
--rw-r--r--  2.0 unx     2569 b- defN 24-Apr-21 18:36 standard_asyncore-3.8.19.dist-info/LICENSE
--rw-r--r--  2.0 unx     3812 b- defN 24-Apr-21 18:36 standard_asyncore-3.8.19.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 18:36 standard_asyncore-3.8.19.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-21 18:36 standard_asyncore-3.8.19.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      518 b- defN 24-Apr-21 18:36 standard_asyncore-3.8.19.dist-info/RECORD
-6 files, 27094 bytes uncompressed, 9380 bytes compressed:  65.4%
+Zip file size: 10327 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    20102 b- defN 24-Apr-21 18:38 asyncore/__init__.py
+-rw-r--r--  2.0 unx     2569 b- defN 24-Apr-21 18:38 standard_asyncore-3.9.19.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3812 b- defN 24-Apr-21 18:38 standard_asyncore-3.9.19.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 18:38 standard_asyncore-3.9.19.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-21 18:38 standard_asyncore-3.9.19.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      518 b- defN 24-Apr-21 18:38 standard_asyncore-3.9.19.dist-info/RECORD
+6 files, 27102 bytes uncompressed, 9381 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: asyncore/__init__.py
 Comment: 
 
-Filename: standard_asyncore-3.8.19.dist-info/LICENSE
+Filename: standard_asyncore-3.9.19.dist-info/LICENSE
 Comment: 
 
-Filename: standard_asyncore-3.8.19.dist-info/METADATA
+Filename: standard_asyncore-3.9.19.dist-info/METADATA
 Comment: 
 
-Filename: standard_asyncore-3.8.19.dist-info/WHEEL
+Filename: standard_asyncore-3.9.19.dist-info/WHEEL
 Comment: 
 
-Filename: standard_asyncore-3.8.19.dist-info/top_level.txt
+Filename: standard_asyncore-3.9.19.dist-info/top_level.txt
 Comment: 
 
-Filename: standard_asyncore-3.8.19.dist-info/RECORD
+Filename: standard_asyncore-3.9.19.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## asyncore/__init__.py

```diff
@@ -224,15 +224,15 @@
             self._map = map
 
         self._fileno = None
 
         if sock:
             # Set to nonblocking just to make sure for cases where we
             # get a socket from a blocking source.
-            sock.setblocking(0)
+            sock.setblocking(False)
             self.set_socket(sock, map)
             self.connected = True
             # The constructor no longer requires that the socket
             # passed be connected.
             try:
                 self.addr = sock.getpeername()
             except OSError as err:
@@ -276,15 +276,15 @@
             #self.log_info('closing channel %d:%s' % (fd, self))
             del map[fd]
         self._fileno = None
 
     def create_socket(self, family=socket.AF_INET, type=socket.SOCK_STREAM):
         self.family_and_type = family, type
         sock = socket.socket(family, type)
-        sock.setblocking(0)
+        sock.setblocking(False)
         self.set_socket(sock)
 
     def set_socket(self, sock, map=None):
         self.socket = sock
         self._fileno = sock.fileno()
         self.add_channel(map)
```

## Comparing `standard_asyncore-3.8.19.dist-info/LICENSE` & `standard_asyncore-3.9.19.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `standard_asyncore-3.8.19.dist-info/METADATA` & `standard_asyncore-3.9.19.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-asyncore
-Version: 3.8.19
+Version: 3.9.19
 Summary: Standard library asyncore redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```


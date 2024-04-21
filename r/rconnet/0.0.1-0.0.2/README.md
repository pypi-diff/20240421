# Comparing `tmp/rconnet-0.0.1.tar.gz` & `tmp/rconnet-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rconnet-0.0.1.tar", last modified: Fri Jan  5 20:11:04 2024, max compression
+gzip compressed data, was "rconnet-0.0.2.tar", last modified: Sun Apr 21 14:41:05 2024, max compression
```

## Comparing `rconnet-0.0.1.tar` & `rconnet-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-01-05 20:11:04.719688 rconnet-0.0.1/
--rw-rw-rw-   0        0        0     1108 2023-12-29 15:18:12.000000 rconnet-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2146 2024-01-05 20:11:04.720690 rconnet-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1813 2023-12-29 15:18:12.000000 rconnet-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-01-05 20:11:04.700688 rconnet-0.0.1/rconnet/
--rw-rw-rw-   0        0        0      126 2023-12-29 09:20:40.000000 rconnet-0.0.1/rconnet/__init__.py
--rw-rw-rw-   0        0        0     2551 2023-12-29 15:13:09.000000 rconnet-0.0.1/rconnet/banmanager.py
--rw-rw-rw-   0        0        0     2511 2023-12-29 15:01:14.000000 rconnet-0.0.1/rconnet/maplist.py
-drwxrwxrwx   0        0        0        0 2024-01-05 20:11:04.718688 rconnet-0.0.1/rconnet/rconbf2142/
--rw-rw-rw-   0        0        0       28 2023-12-29 09:17:57.000000 rconnet-0.0.1/rconnet/rconbf2142/__init__.py
--rw-rw-rw-   0        0        0     3230 2023-12-29 14:51:29.000000 rconnet-0.0.1/rconnet/rconbf2142/default.py
--rw-rw-rw-   0        0        0    10069 2023-12-29 14:01:40.000000 rconnet-0.0.1/rconnet/settings.py
--rw-rw-rw-   0        0        0     3502 2023-12-29 14:01:40.000000 rconnet-0.0.1/rconnet/tcpclient.py
-drwxrwxrwx   0        0        0        0 2024-01-05 20:11:04.715688 rconnet-0.0.1/rconnet.egg-info/
--rw-rw-rw-   0        0        0     2146 2024-01-05 20:11:04.000000 rconnet-0.0.1/rconnet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-01-05 20:11:04.000000 rconnet-0.0.1/rconnet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-05 20:11:04.000000 rconnet-0.0.1/rconnet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-01-05 20:11:04.000000 rconnet-0.0.1/rconnet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-05 20:11:04.722688 rconnet-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      513 2024-01-05 20:10:41.000000 rconnet-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:41:05.913538 rconnet-0.0.2/
+-rw-rw-rw-   0        0        0     1108 2024-03-22 10:02:31.000000 rconnet-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      290 2024-04-21 14:41:05.913538 rconnet-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1994 2024-03-22 17:52:23.000000 rconnet-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 14:41:05.889535 rconnet-0.0.2/rconnet/
+-rw-rw-rw-   0        0        0      192 2024-03-22 15:03:35.000000 rconnet-0.0.2/rconnet/__init__.py
+-rw-rw-rw-   0        0        0     2551 2024-03-22 10:02:31.000000 rconnet-0.0.2/rconnet/banmanager.py
+-rw-rw-rw-   0        0        0     2511 2024-03-22 10:02:31.000000 rconnet-0.0.2/rconnet/maplist.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:41:05.907530 rconnet-0.0.2/rconnet/rconbf2142/
+-rw-rw-rw-   0        0        0       64 2024-03-22 15:04:10.000000 rconnet-0.0.2/rconnet/rconbf2142/__init__.py
+-rw-rw-rw-   0        0        0     3230 2024-03-22 10:02:31.000000 rconnet-0.0.2/rconnet/rconbf2142/default.py
+-rw-rw-rw-   0        0        0     3009 2024-03-24 15:21:11.000000 rconnet-0.0.2/rconnet/rconbf2142/modmanager.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:41:05.908529 rconnet-0.0.2/rconnet/rconbf2142/modules/
+-rw-rw-rw-   0        0        0        0 2024-03-24 15:06:41.000000 rconnet-0.0.2/rconnet/rconbf2142/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:41:05.909531 rconnet-0.0.2/rconnet/rconbf2142/modules/modmanager/
+-rw-rw-rw-   0        0        0        0 2024-03-24 15:03:54.000000 rconnet-0.0.2/rconnet/rconbf2142/modules/modmanager/__init__.py
+-rw-rw-rw-   0        0        0     5665 2024-04-21 14:26:33.000000 rconnet-0.0.2/rconnet/rconbf2142/modules/modmanager/bf2cc.py
+-rw-rw-rw-   0        0        0    10069 2024-03-22 10:02:31.000000 rconnet-0.0.2/rconnet/settings.py
+-rw-rw-rw-   0        0        0     5836 2024-03-22 14:22:13.000000 rconnet-0.0.2/rconnet/tcpclient.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:41:05.911531 rconnet-0.0.2/rconnet.egg-info/
+-rw-rw-rw-   0        0        0      290 2024-04-21 14:41:05.000000 rconnet-0.0.2/rconnet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2024-04-21 14:41:05.000000 rconnet-0.0.2/rconnet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 14:41:05.000000 rconnet-0.0.2/rconnet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-21 14:41:05.000000 rconnet-0.0.2/rconnet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 14:41:05.917532 rconnet-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      528 2024-04-21 14:40:58.000000 rconnet-0.0.2/setup.py
```

### Comparing `rconnet-0.0.1/LICENSE` & `rconnet-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rconnet-0.0.1/PKG-INFO` & `rconnet-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,21 @@
-Metadata-Version: 2.1
-Name: rconnet
-Version: 0.0.1
-Summary: Python RCON client for the Battlefield 2142 server
-Home-page: https://github.com/VordyV/rconnet
-Author: VordyV
-Author-email: vordy.production@gmail.com
-Keywords: rcon client
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # rconnet
 The project is a module for python, and the task of the module is to create a connection to the RCON Battlefield 2142, Battlefield 2 server. Simply put, it is an RCON client.
 
 Main idea of the project was to implement something similar to ORM, as for databases.
 
 It was developed on version python 3.11, it was not tested on other versions.
 
+You can learn more about the module and its API in [Wiki](https://github.com/VordyV/rconnet/wiki)
+
+### Install
+`pip install rconnet`
+
+[pypi.org/project/rconnet/](https://pypi.org/project/rconnet/)
+
 ### Features
 - Separate methods for server management
 - Maplist manager
 - Settings manager
 - Ban manager
 - Player manager
 - Managers allow you to "objects" manage
@@ -30,35 +25,35 @@
 - Battlefield 2142 support (It has not been tested in Battlefield 2, but it can work)
 
 You can do anything with this module, for example, a web banlist, a GUI program, a bot for Discord or telegram. That was the goal, to use a ready-made solution for different purposes.
 
 ## Examples
 1. Simple output of the server name
 ```python
-from rconnet.rconbf2142.default import Default
+from rconnet.rconbf2142 import Default
 
 with Default("127.0.0.1", "super123") as rcon:
     name = rcon.settings.server_name()
     print(name)
     # Battlefield 2142
 ```
 2. View the maplist and install the next map
 ```python
-from rconnet.rconbf2142.default import Default
+from rconnet.rconbf2142 import Default
 
 with Default("127.0.0.1", "super123") as rcon:
     maplist = rcon.maplist.list
     print(maplist)
     # {0: Map(name=minsk, gpm=gpm_cq, size=32), 1: Map(name=fall_of_berlin, gpm=gpm_cq, size=32), 2: Map(name=suez_canal, gpm=gpm_ti, size=48)}
     maplist.get(1).set_next()
     rcon.run_next_level()
 ```
 3. Adding a ban to the list
 ```python
-from rconnet.rconbf2142.default import Default
+from rconnet.rconbf2142 import Default
 
 with Default("127.0.0.1", "super123") as rcon:
     rcon.banmanager.add_ban("172.123.54.6")
     banlist = rcon.banmanager.list
     print(banlist)
     # [Ban(address=172.123.54.6, period=Perm)]
 ```
```

### Comparing `rconnet-0.0.1/rconnet/banmanager.py` & `rconnet-0.0.2/rconnet/banmanager.py`

 * *Files identical despite different names*

### Comparing `rconnet-0.0.1/rconnet/maplist.py` & `rconnet-0.0.2/rconnet/maplist.py`

 * *Files identical despite different names*

### Comparing `rconnet-0.0.1/rconnet/rconbf2142/default.py` & `rconnet-0.0.2/rconnet/rconbf2142/default.py`

 * *Files identical despite different names*

### Comparing `rconnet-0.0.1/rconnet/settings.py` & `rconnet-0.0.2/rconnet/settings.py`

 * *Files identical despite different names*

### Comparing `rconnet-0.0.1/rconnet/tcpclient.py` & `rconnet-0.0.2/rconnet/tcpclient.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,46 +9,70 @@
 class TCPClientStatuses:
     DISABLED = 0
     CONNECTED = 1
     RECONNECTING = 2
 
 class TCPClient(object):
 
-    def __init__(self, address: str, password: int, port: int=4711, reconnect: bool=True, debug: bool=True, debug_format:str="%(levelname)s:%(message)s", debug_level:object=logging.DEBUG):
+    def __init__(self, address: str,
+                 password: int,
+                 port: int=4711,
+                 debug: bool=True,
+                 debug_format: str="%(levelname)s:%(message)s",
+                 debug_level: object=logging.DEBUG,
+                 on_connect = None,
+                 on_disconnect = None,
+                 on_close = None,
+                 on_status = None,
+                 ):
+
         self.socket = None
         self.address = address
         self.password = password
         self.port = port
-        self._reconnect = reconnect
         self.debug = debug
         self.debug_format = debug_format
         self.debug_level = debug_level
+        self.on_connect = on_connect,
+        self.on_disconnect = on_disconnect,
+        self.on_close = on_close,
+        self.on_status = on_status,
         self._status = TCPClientStatuses.DISABLED
         self._inr = 0
 
         logging.basicConfig(format=self.debug_format, level=self.debug_level)
 
+    def _exec_event(self, name, *args):
+        method = getattr(self, name)
+        if type(method) == tuple: method = method[0]
+        if method is not None: method(*args)
+
     def log(self, *value):
         if self.debug: logging.debug(" ".join(str(v) for v in value))
 
     @property
     def status(self):
         return self._status
 
     @status.setter
     def status(self, status):
         self._status = status
+        self._exec_event("on_status", status)
 
     def start(self):
         self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.socket.connect((self.address, self.port))
-        self.pre_init()
+        self._pre_init()
         self.status = TCPClientStatuses.CONNECTED
+        self._exec_event("on_connect")
         return True
 
+    def _pre_init(self):
+        self.pre_init()
+
     def pre_init(self):
         welcResponse = ""
         while 1:
             data = self.socket.recv(1024)
             welcResponse += data.decode("utf-8")
             eosPos = welcResponse.find('\n\n')
             if eosPos != -1: break;
@@ -75,32 +99,75 @@
     def is_closed(self):
         return self.status == TCPClientStatuses.DISABLED
 
     def close(self):
         if not self.socket: return None
         self.status = TCPClientStatuses.DISABLED
         self.socket.close()
+        self._exec_event("on_close")
 
     def rcon_invoke(self, command):
-        rt = time.time_ns()
         if not self.socket: raise Exception("The client is not connected")
         self.socket.send(('\x02' + command + '\n').encode("utf-8"))
         self._inr += 1
         result = ""
         done = False
         while not done:
             try:
                 data = self.socket.recv(2048)
                 if data is None: raise Exception("Client has terminated the current connection. ")
             except Exception as error:
                 self.status = TCPClientStatuses.DISABLED
+                self._exec_event("on_disconnect", error)
                 raise Exception(error)
             for c in data:
                 if c == 0x4:
                     done = True
                     break
                 result += chr(c)
         if len(result) > 0 and result[-1] == "\n": result = result[:-1]
-        ct = time.time_ns()
-        #self.log(ct-rt, "ns")
         if result.strip() == "": return None
-        return result
+        return result
+
+class TCPListener(TCPClient):
+
+    def __init__(self, *args, commands:list = [], on_recv:object = None, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._commands = commands
+        self.on_recv = on_recv
+
+    def pre_init(self):
+        super().pre_init()
+        for command in self._commands:
+            self.socket.send(('\x02' + command + '\n').encode("utf-8"))
+
+    def start(self):
+        while True:
+            self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            try:
+                self.socket.connect((self.address, self.port))
+                self._pre_init()
+                self.status = TCPClientStatuses.CONNECTED
+                self._exec_event("on_connect")
+            except Exception as error:
+                time.sleep(3)
+                print(error)
+                continue
+
+            while 1:
+                try:
+                    data = self.socket.recv(2048)
+                    if data is None: raise Exception("Client has terminated the current connection. ")
+                except Exception as error:
+                    self._exec_event("on_disconnect", error)
+                    break
+                result = data
+                done = False
+                if result[-1] == 0x4: done = True
+                while not done:
+                    data = self.socket.recv(2048)
+                    for c in data:
+                        if c == 0x4:
+                            done = True
+                            break
+                        result += chr(c)
+                self._exec_event("on_recv", result)
```


# Comparing `tmp/throttle_client-0.4.8.tar.gz` & `tmp/throttle_client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "throttle_client-0.4.8.tar", last modified: Sat Apr 20 20:53:03 2024, max compression
+gzip compressed data, was "throttle_client-0.5.0.tar", last modified: Sun Apr 21 11:26:55 2024, max compression
```

## Comparing `throttle_client-0.4.8.tar` & `throttle_client-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:03.669805 throttle_client-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-20 20:52:59.000000 throttle_client-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-04-20 20:53:03.665805 throttle_client-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9466 2024-04-20 20:52:59.000000 throttle_client-0.4.8/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-20 20:52:59.000000 throttle_client-0.4.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:03.661805 throttle_client-0.4.8/python_client/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:03.665805 throttle_client-0.4.8/python_client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/tests/test_peer.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/tests/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/tests/test_server_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:03.665805 throttle_client-0.4.8/python_client/throttle_client/
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/throttle_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/throttle_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/throttle_client/peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/throttle_client/status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:03.665805 throttle_client-0.4.8/python_client/throttle_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-04-20 20:53:03.000000 throttle_client-0.4.8/python_client/throttle_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-20 20:53:03.000000 throttle_client-0.4.8/python_client/throttle_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 20:53:03.000000 throttle_client-0.4.8/python_client/throttle_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-20 20:53:03.000000 throttle_client-0.4.8/python_client/throttle_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 20:53:03.000000 throttle_client-0.4.8/python_client/throttle_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 20:53:03.669805 throttle_client-0.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:26:55.284746 throttle_client-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 11:26:51.000000 throttle_client-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-04-21 11:26:55.284746 throttle_client-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9466 2024-04-21 11:26:51.000000 throttle_client-0.5.0/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-21 11:26:51.000000 throttle_client-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:26:55.280746 throttle_client-0.5.0/python_client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:26:55.280746 throttle_client-0.5.0/python_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/tests/test_peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/tests/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/tests/test_server_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:26:55.284746 throttle_client-0.5.0/python_client/throttle_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/throttle_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/throttle_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/throttle_client/peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/throttle_client/status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:26:55.284746 throttle_client-0.5.0/python_client/throttle_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-04-21 11:26:55.000000 throttle_client-0.5.0/python_client/throttle_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-21 11:26:55.000000 throttle_client-0.5.0/python_client/throttle_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 11:26:55.000000 throttle_client-0.5.0/python_client/throttle_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-21 11:26:55.000000 throttle_client-0.5.0/python_client/throttle_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 11:26:55.000000 throttle_client-0.5.0/python_client/throttle_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 11:26:55.284746 throttle_client-0.5.0/setup.cfg
```

### Comparing `throttle_client-0.4.8/LICENSE` & `throttle_client-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `throttle_client-0.4.8/PKG-INFO` & `throttle_client-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: throttle_client
-Version: 0.4.8
+Version: 0.5.0
 Summary: Client for Throttle. Throttle is an http semaphore service, providing semaphores for distributed systems.
 Author: Markus Klein 
 License: MIT License
 Project-URL: Repository, https://github.com/pacman82/throttle.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `throttle_client-0.4.8/Readme.md` & `throttle_client-0.5.0/Readme.md`

 * *Files identical despite different names*

### Comparing `throttle_client-0.4.8/pyproject.toml` & `throttle_client-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "throttle_client"
-version = "0.4.8"
+version = "0.5.0"
 authors = [{ name = "Markus Klein " }]
 license = { text = "MIT License" }
 description = "Client for Throttle. Throttle is an http semaphore service, providing semaphores for distributed systems."
 readme = "Readme.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `throttle_client-0.4.8/python_client/tests/__init__.py` & `throttle_client-0.5.0/python_client/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.4.8/python_client/tests/test_lock.py` & `throttle_client-0.5.0/python_client/tests/test_lock.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             expiration_time=timedelta(seconds=4),
         )
         set_local_peer(url, peer)
         with lock(url, "A") as _:
             sleep(5)
             # Evens though enough time has passed, our lease should not be
             # expired, thanks to the heartbeat.
-            assert client.remove_expired() == 0
+            assert client.is_acquired(peer.id)
 
 
 def test_lock_count_larger_one():
     """
     Assert that locks with a count > 1, decrement the semaphore count accordingly
     """
```

### Comparing `throttle_client-0.4.8/python_client/tests/test_peer.py` & `throttle_client-0.5.0/python_client/tests/test_peer.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.4.8/python_client/tests/test_server_client.py` & `throttle_client-0.5.0/python_client/tests/test_server_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,16 @@
         # pending
         assert client.is_acquired(second)
 
 
 def test_locks_of_expired_peers_are_released():
     """If a peer is removed due to expiration, it's locks must be released."""
     with throttle_client(b"[semaphores]\nA=1") as client:
-        peer = client.new_peer(expires_in=timedelta(seconds=0))
-        client.acquire(peer, "A")
-        client.remove_expired()
+        peer = client.new_peer(expires_in=timedelta(seconds=3))
+        client.acquire(peer, "A", expires_in=timedelta(seconds=0))
         assert client.remainder("A") == 1  # Semaphore should be free again
 
 
 def test_lock_blocks():
     """
     Acquire must block until the semaphore count allows for the lock to be acquired.
     """
@@ -71,27 +70,28 @@
     Test that peers do not expire, while they wait for pending locks.
     """
     with throttle_client(b"[semaphores]\nA=1") as client:
         blocker = client.new_peer(expires_in=timedelta(minutes=1))
         # Acquire "A", so subsequent locks are pending
         client.acquire(blocker, "A")
 
-        peer = client.new_peer(expires_in=timedelta(seconds=1))
+        peer_id = client.new_peer(expires_in=timedelta(seconds=3))
         # This lock can not be acquired due to `blocker` holding the lock. This request
         # is going to block for one second. After which the peer should have been
         # expired. Yet acquire can prolong the lifetime of the peer.
         client.acquire(
-            peer,
+            peer_id,
             semaphore="A",
-            block_for=timedelta(seconds=1),
-            expires_in=timedelta(seconds=5),
+            block_for=timedelta(seconds=3),
+            expires_in=timedelta(seconds=100),
         )
-        # The initial timeout of one second should have been expired by now, yet nothing
-        # is removed.
-        assert client.remove_expired() == 0
+        # The initial timeout of one second should have been expired by now, yet peer must still be
+        # alive. We validate this calling a method for the peer and observing that "unknown peer"
+        # is **not** raised
+        assert not client.is_acquired(peer_id=peer_id)
 
 
 def test_restore_peer_with_unknown_semaphore():
     """
     A revenant Peer may not acquire a semaphore which does not exist on the server.
     """
     # Restart Server without "A"
```

### Comparing `throttle_client-0.4.8/python_client/throttle_client/__init__.py` & `throttle_client-0.5.0/python_client/throttle_client/__init__.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.4.8/python_client/throttle_client/client.py` & `throttle_client-0.5.0/python_client/throttle_client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -249,29 +249,14 @@
 
         def send_request():
             response = requests.delete(f"{self.base_url}/peers/{peer_id}/{semaphore}")
             return response
 
         self._try_request(send_request)
 
-    def remove_expired(self) -> int:
-        """
-        Request the throttle server to remove all expired peers.
-
-        Returns number of expired peers.
-        """
-
-        def send_request():
-            response = requests.post(self.base_url + "/remove_expired", timeout=30)
-            return response
-
-        response = self._try_request(send_request)
-        # Number of expired peers
-        return json.loads(response.text)
-
     def heartbeat(self, peer_id: int, expires_in: timedelta):
         """
         Sends a PUT request to the server, updating the expiration timestamp.
         """
 
         def send_request():
             response = requests.put(
```

### Comparing `throttle_client-0.4.8/python_client/throttle_client/peer.py` & `throttle_client-0.5.0/python_client/throttle_client/peer.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.4.8/python_client/throttle_client/status_code.py` & `throttle_client-0.5.0/python_client/throttle_client/status_code.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.4.8/python_client/throttle_client.egg-info/PKG-INFO` & `throttle_client-0.5.0/python_client/throttle_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: throttle_client
-Version: 0.4.8
+Version: 0.5.0
 Summary: Client for Throttle. Throttle is an http semaphore service, providing semaphores for distributed systems.
 Author: Markus Klein 
 License: MIT License
 Project-URL: Repository, https://github.com/pacman82/throttle.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `throttle_client-0.4.8/python_client/throttle_client.egg-info/SOURCES.txt` & `throttle_client-0.5.0/python_client/throttle_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*


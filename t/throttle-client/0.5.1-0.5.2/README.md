# Comparing `tmp/throttle_client-0.5.1.tar.gz` & `tmp/throttle_client-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "throttle_client-0.5.1.tar", last modified: Sun Apr 21 11:35:04 2024, max compression
+gzip compressed data, was "throttle_client-0.5.2.tar", last modified: Sun Apr 21 12:02:33 2024, max compression
```

## Comparing `throttle_client-0.5.1.tar` & `throttle_client-0.5.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:35:04.261966 throttle_client-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 11:35:00.000000 throttle_client-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-21 11:35:04.261966 throttle_client-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-04-21 11:35:00.000000 throttle_client-0.5.1/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-21 11:35:00.000000 throttle_client-0.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:35:04.257966 throttle_client-0.5.1/python_client/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:35:04.261966 throttle_client-0.5.1/python_client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/tests/test_peer.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/tests/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/tests/test_server_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:35:04.261966 throttle_client-0.5.1/python_client/throttle_client/
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/throttle_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/throttle_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/throttle_client/peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/throttle_client/status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:35:04.261966 throttle_client-0.5.1/python_client/throttle_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-21 11:35:04.000000 throttle_client-0.5.1/python_client/throttle_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-21 11:35:04.000000 throttle_client-0.5.1/python_client/throttle_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 11:35:04.000000 throttle_client-0.5.1/python_client/throttle_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-21 11:35:04.000000 throttle_client-0.5.1/python_client/throttle_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 11:35:04.000000 throttle_client-0.5.1/python_client/throttle_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 11:35:04.261966 throttle_client-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:02:33.189968 throttle_client-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 12:02:28.000000 throttle_client-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-21 12:02:33.189968 throttle_client-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-04-21 12:02:28.000000 throttle_client-0.5.2/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-21 12:02:28.000000 throttle_client-0.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:02:33.185968 throttle_client-0.5.2/python_client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:02:33.185968 throttle_client-0.5.2/python_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-21 12:02:28.000000 throttle_client-0.5.2/python_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-04-21 12:02:28.000000 throttle_client-0.5.2/python_client/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-21 12:02:28.000000 throttle_client-0.5.2/python_client/tests/test_peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-21 12:02:28.000000 throttle_client-0.5.2/python_client/tests/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-04-21 12:02:28.000000 throttle_client-0.5.2/python_client/tests/test_server_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:02:33.189968 throttle_client-0.5.2/python_client/throttle_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-21 12:02:28.000000 throttle_client-0.5.2/python_client/throttle_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-04-21 12:02:28.000000 throttle_client-0.5.2/python_client/throttle_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-21 12:02:28.000000 throttle_client-0.5.2/python_client/throttle_client/peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-21 12:02:28.000000 throttle_client-0.5.2/python_client/throttle_client/status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:02:33.189968 throttle_client-0.5.2/python_client/throttle_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-21 12:02:33.000000 throttle_client-0.5.2/python_client/throttle_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-21 12:02:33.000000 throttle_client-0.5.2/python_client/throttle_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 12:02:33.000000 throttle_client-0.5.2/python_client/throttle_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-21 12:02:33.000000 throttle_client-0.5.2/python_client/throttle_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 12:02:33.000000 throttle_client-0.5.2/python_client/throttle_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 12:02:33.189968 throttle_client-0.5.2/setup.cfg
```

### Comparing `throttle_client-0.5.1/LICENSE` & `throttle_client-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.1/PKG-INFO` & `throttle_client-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: throttle_client
-Version: 0.5.1
+Version: 0.5.2
 Summary: Client for Throttle. Throttle is an http semaphore service, providing semaphores for distributed systems.
 Author: Markus Klein 
 License: MIT License
 Project-URL: Repository, https://github.com/pacman82/throttle.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `throttle_client-0.5.1/Readme.md` & `throttle_client-0.5.2/Readme.md`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.1/pyproject.toml` & `throttle_client-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "throttle_client"
-version = "0.5.1"
+version = "0.5.2"
 authors = [{ name = "Markus Klein " }]
 license = { text = "MIT License" }
 description = "Client for Throttle. Throttle is an http semaphore service, providing semaphores for distributed systems."
 readme = "Readme.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `throttle_client-0.5.1/python_client/tests/__init__.py` & `throttle_client-0.5.2/python_client/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.1/python_client/tests/test_lock.py` & `throttle_client-0.5.2/python_client/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.1/python_client/tests/test_peer.py` & `throttle_client-0.5.2/python_client/tests/test_peer.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.1/python_client/tests/test_server_client.py` & `throttle_client-0.5.2/python_client/tests/test_server_client.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.1/python_client/throttle_client/__init__.py` & `throttle_client-0.5.2/python_client/throttle_client/__init__.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.1/python_client/throttle_client/client.py` & `throttle_client-0.5.2/python_client/throttle_client/client.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.1/python_client/throttle_client/peer.py` & `throttle_client-0.5.2/python_client/throttle_client/peer.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.1/python_client/throttle_client/status_code.py` & `throttle_client-0.5.2/python_client/throttle_client/status_code.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.1/python_client/throttle_client.egg-info/PKG-INFO` & `throttle_client-0.5.2/python_client/throttle_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: throttle_client
-Version: 0.5.1
+Version: 0.5.2
 Summary: Client for Throttle. Throttle is an http semaphore service, providing semaphores for distributed systems.
 Author: Markus Klein 
 License: MIT License
 Project-URL: Repository, https://github.com/pacman82/throttle.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `throttle_client-0.5.1/python_client/throttle_client.egg-info/SOURCES.txt` & `throttle_client-0.5.2/python_client/throttle_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*


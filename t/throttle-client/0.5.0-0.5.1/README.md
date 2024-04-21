# Comparing `tmp/throttle_client-0.5.0.tar.gz` & `tmp/throttle_client-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "throttle_client-0.5.0.tar", last modified: Sun Apr 21 11:26:55 2024, max compression
+gzip compressed data, was "throttle_client-0.5.1.tar", last modified: Sun Apr 21 11:35:04 2024, max compression
```

## Comparing `throttle_client-0.5.0.tar` & `throttle_client-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:26:55.284746 throttle_client-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 11:26:51.000000 throttle_client-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-04-21 11:26:55.284746 throttle_client-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9466 2024-04-21 11:26:51.000000 throttle_client-0.5.0/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-21 11:26:51.000000 throttle_client-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:26:55.280746 throttle_client-0.5.0/python_client/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:26:55.280746 throttle_client-0.5.0/python_client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/tests/test_peer.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/tests/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/tests/test_server_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:26:55.284746 throttle_client-0.5.0/python_client/throttle_client/
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/throttle_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/throttle_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/throttle_client/peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-21 11:26:51.000000 throttle_client-0.5.0/python_client/throttle_client/status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:26:55.284746 throttle_client-0.5.0/python_client/throttle_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-04-21 11:26:55.000000 throttle_client-0.5.0/python_client/throttle_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-21 11:26:55.000000 throttle_client-0.5.0/python_client/throttle_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 11:26:55.000000 throttle_client-0.5.0/python_client/throttle_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-21 11:26:55.000000 throttle_client-0.5.0/python_client/throttle_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 11:26:55.000000 throttle_client-0.5.0/python_client/throttle_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 11:26:55.284746 throttle_client-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:35:04.261966 throttle_client-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 11:35:00.000000 throttle_client-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-21 11:35:04.261966 throttle_client-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-04-21 11:35:00.000000 throttle_client-0.5.1/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-21 11:35:00.000000 throttle_client-0.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:35:04.257966 throttle_client-0.5.1/python_client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:35:04.261966 throttle_client-0.5.1/python_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/tests/test_peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/tests/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/tests/test_server_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:35:04.261966 throttle_client-0.5.1/python_client/throttle_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/throttle_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/throttle_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/throttle_client/peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-21 11:35:00.000000 throttle_client-0.5.1/python_client/throttle_client/status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:35:04.261966 throttle_client-0.5.1/python_client/throttle_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-21 11:35:04.000000 throttle_client-0.5.1/python_client/throttle_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-21 11:35:04.000000 throttle_client-0.5.1/python_client/throttle_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 11:35:04.000000 throttle_client-0.5.1/python_client/throttle_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-21 11:35:04.000000 throttle_client-0.5.1/python_client/throttle_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 11:35:04.000000 throttle_client-0.5.1/python_client/throttle_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 11:35:04.261966 throttle_client-0.5.1/setup.cfg
```

### Comparing `throttle_client-0.5.0/LICENSE` & `throttle_client-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.0/PKG-INFO` & `throttle_client-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: throttle_client
-Version: 0.5.0
+Version: 0.5.1
 Summary: Client for Throttle. Throttle is an http semaphore service, providing semaphores for distributed systems.
 Author: Markus Klein 
 License: MIT License
 Project-URL: Repository, https://github.com/pacman82/throttle.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -114,28 +114,23 @@
 ```
 
 Starting the server now yields more information.
 
 ```log
 [2020-04-12T18:56:23Z INFO  throttle] Hello From Throttle
 [2020-04-12T18:56:23Z WARN  throttle] No semaphores configured.
-[2020-04-12T18:56:23Z INFO  throttle::litter_collection] Start litter collection with interval: 300s
 ```
 
 #### Toml configuration file
 
 To actually serve semaphores, we need to configure their names and full count. By default Throttle is looking for a configuration in the working directories `throttle.toml` file should it exist.
 
 ```toml
 # Sample throttle.cfg Explaining the options
 
-# The time interval in which the litter collection backgroud thread checks for expired leases.
-# Default is set to 5 minutes.
-litter_collection_interval = "5min"
-
 [semaphores]
 # Specify name and full count of semaphores. Below line creates a semaphore named A with a full
 # count of 42. Setting the count to 1 would create a Mutex.
 A = 42
 
 ## Optional logging config, to log to stderr. Can be overwritten using the `THROTTLE_LOG`
 ## environment variable.
```

### Comparing `throttle_client-0.5.0/Readme.md` & `throttle_client-0.5.1/python_client/throttle_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: throttle_client
+Version: 0.5.1
+Summary: Client for Throttle. Throttle is an http semaphore service, providing semaphores for distributed systems.
+Author: Markus Klein 
+License: MIT License
+Project-URL: Repository, https://github.com/pacman82/throttle.git
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: tenacity
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+
 # Throttle
 
 Semaphores for distributed systems.
 
 ## Motivation
 
 Throttle provides semaphores as a service via an http interface. As the name indicates the primary usecase in mind is to throttle a systems access to a resource, by having the elements of that system to ask for permission (i.e. acquiring a lease) first. If the system consists of several process running on different machines, or virtual machines in the same Network, throttle might fit the bill.
@@ -96,28 +114,23 @@
 ```
 
 Starting the server now yields more information.
 
 ```log
 [2020-04-12T18:56:23Z INFO  throttle] Hello From Throttle
 [2020-04-12T18:56:23Z WARN  throttle] No semaphores configured.
-[2020-04-12T18:56:23Z INFO  throttle::litter_collection] Start litter collection with interval: 300s
 ```
 
 #### Toml configuration file
 
 To actually serve semaphores, we need to configure their names and full count. By default Throttle is looking for a configuration in the working directories `throttle.toml` file should it exist.
 
 ```toml
 # Sample throttle.cfg Explaining the options
 
-# The time interval in which the litter collection backgroud thread checks for expired leases.
-# Default is set to 5 minutes.
-litter_collection_interval = "5min"
-
 [semaphores]
 # Specify name and full count of semaphores. Below line creates a semaphore named A with a full
 # count of 42. Setting the count to 1 would create a Mutex.
 A = 42
 
 ## Optional logging config, to log to stderr. Can be overwritten using the `THROTTLE_LOG`
 ## environment variable.
```

### Comparing `throttle_client-0.5.0/pyproject.toml` & `throttle_client-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "throttle_client"
-version = "0.5.0"
+version = "0.5.1"
 authors = [{ name = "Markus Klein " }]
 license = { text = "MIT License" }
 description = "Client for Throttle. Throttle is an http semaphore service, providing semaphores for distributed systems."
 readme = "Readme.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `throttle_client-0.5.0/python_client/tests/__init__.py` & `throttle_client-0.5.1/python_client/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.0/python_client/tests/test_lock.py` & `throttle_client-0.5.1/python_client/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.0/python_client/tests/test_peer.py` & `throttle_client-0.5.1/python_client/tests/test_peer.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.0/python_client/tests/test_server_client.py` & `throttle_client-0.5.1/python_client/tests/test_server_client.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.0/python_client/throttle_client/__init__.py` & `throttle_client-0.5.1/python_client/throttle_client/__init__.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.0/python_client/throttle_client/client.py` & `throttle_client-0.5.1/python_client/throttle_client/client.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.0/python_client/throttle_client/peer.py` & `throttle_client-0.5.1/python_client/throttle_client/peer.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.0/python_client/throttle_client/status_code.py` & `throttle_client-0.5.1/python_client/throttle_client/status_code.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.5.0/python_client/throttle_client.egg-info/PKG-INFO` & `throttle_client-0.5.1/Readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: throttle_client
-Version: 0.5.0
-Summary: Client for Throttle. Throttle is an http semaphore service, providing semaphores for distributed systems.
-Author: Markus Klein 
-License: MIT License
-Project-URL: Repository, https://github.com/pacman82/throttle.git
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: tenacity
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-
 # Throttle
 
 Semaphores for distributed systems.
 
 ## Motivation
 
 Throttle provides semaphores as a service via an http interface. As the name indicates the primary usecase in mind is to throttle a systems access to a resource, by having the elements of that system to ask for permission (i.e. acquiring a lease) first. If the system consists of several process running on different machines, or virtual machines in the same Network, throttle might fit the bill.
@@ -114,28 +96,23 @@
 ```
 
 Starting the server now yields more information.
 
 ```log
 [2020-04-12T18:56:23Z INFO  throttle] Hello From Throttle
 [2020-04-12T18:56:23Z WARN  throttle] No semaphores configured.
-[2020-04-12T18:56:23Z INFO  throttle::litter_collection] Start litter collection with interval: 300s
 ```
 
 #### Toml configuration file
 
 To actually serve semaphores, we need to configure their names and full count. By default Throttle is looking for a configuration in the working directories `throttle.toml` file should it exist.
 
 ```toml
 # Sample throttle.cfg Explaining the options
 
-# The time interval in which the litter collection backgroud thread checks for expired leases.
-# Default is set to 5 minutes.
-litter_collection_interval = "5min"
-
 [semaphores]
 # Specify name and full count of semaphores. Below line creates a semaphore named A with a full
 # count of 42. Setting the count to 1 would create a Mutex.
 A = 42
 
 ## Optional logging config, to log to stderr. Can be overwritten using the `THROTTLE_LOG`
 ## environment variable.
```

### Comparing `throttle_client-0.5.0/python_client/throttle_client.egg-info/SOURCES.txt` & `throttle_client-0.5.1/python_client/throttle_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/numpyneuron-0.5.tar.gz` & `tmp/numpyneuron-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpyneuron-0.5.tar", last modified: Sat Apr 20 01:27:06 2024, max compression
+gzip compressed data, was "numpyneuron-0.6.tar", last modified: Sun Apr 21 04:38:33 2024, max compression
```

## Comparing `numpyneuron-0.5.tar` & `numpyneuron-0.6.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-20 01:27:06.124135 numpyneuron-0.5/
--rw-r--r--   0 jensen     (501) staff       (20)     2467 2024-04-20 01:27:06.123951 numpyneuron-0.5/PKG-INFO
--rw-r--r--   0 jensen     (501) staff       (20)     2476 2024-04-19 23:52:58.000000 numpyneuron-0.5/README.md
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-20 01:27:06.123193 numpyneuron-0.5/numpyneuron/
--rw-r--r--   0 jensen     (501) staff       (20)       64 2024-04-19 21:54:45.000000 numpyneuron-0.5/numpyneuron/__init__.py
--rw-r--r--   0 jensen     (501) staff       (20)     1339 2024-04-19 23:54:15.000000 numpyneuron-0.5/numpyneuron/activation.py
--rw-r--r--   0 jensen     (501) staff       (20)     2483 2024-04-19 23:54:32.000000 numpyneuron-0.5/numpyneuron/loss.py
--rw-r--r--   0 jensen     (501) staff       (20)     6451 2024-04-19 22:16:48.000000 numpyneuron-0.5/numpyneuron/nn.py
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-20 01:27:06.123788 numpyneuron-0.5/numpyneuron.egg-info/
--rw-r--r--   0 jensen     (501) staff       (20)     2467 2024-04-20 01:27:06.000000 numpyneuron-0.5/numpyneuron.egg-info/PKG-INFO
--rw-r--r--   0 jensen     (501) staff       (20)      254 2024-04-20 01:27:06.000000 numpyneuron-0.5/numpyneuron.egg-info/SOURCES.txt
--rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-20 01:27:06.000000 numpyneuron-0.5/numpyneuron.egg-info/dependency_links.txt
--rw-r--r--   0 jensen     (501) staff       (20)       12 2024-04-20 01:27:06.000000 numpyneuron-0.5/numpyneuron.egg-info/top_level.txt
--rw-r--r--   0 jensen     (501) staff       (20)       38 2024-04-20 01:27:06.124170 numpyneuron-0.5/setup.cfg
--rw-r--r--   0 jensen     (501) staff       (20)      605 2024-04-20 01:26:21.000000 numpyneuron-0.5/setup.py
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-21 04:38:33.573887 numpyneuron-0.6/
+-rw-r--r--   0 jensen     (501) staff       (20)     2530 2024-04-21 04:38:33.573702 numpyneuron-0.6/PKG-INFO
+-rw-r--r--   0 jensen     (501) staff       (20)     2476 2024-04-19 23:52:58.000000 numpyneuron-0.6/README.md
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-21 04:38:33.572375 numpyneuron-0.6/numpyneuron/
+-rw-r--r--   0 jensen     (501) staff       (20)       64 2024-04-19 21:54:45.000000 numpyneuron-0.6/numpyneuron/__init__.py
+-rw-r--r--   0 jensen     (501) staff       (20)     1339 2024-04-19 23:54:15.000000 numpyneuron-0.6/numpyneuron/activation.py
+-rw-r--r--   0 jensen     (501) staff       (20)     2483 2024-04-19 23:54:32.000000 numpyneuron-0.6/numpyneuron/loss.py
+-rw-r--r--   0 jensen     (501) staff       (20)     6451 2024-04-19 22:16:48.000000 numpyneuron-0.6/numpyneuron/nn.py
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-21 04:38:33.573493 numpyneuron-0.6/numpyneuron.egg-info/
+-rw-r--r--   0 jensen     (501) staff       (20)     2530 2024-04-21 04:38:33.000000 numpyneuron-0.6/numpyneuron.egg-info/PKG-INFO
+-rw-r--r--   0 jensen     (501) staff       (20)      346 2024-04-21 04:38:33.000000 numpyneuron-0.6/numpyneuron.egg-info/SOURCES.txt
+-rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-21 04:38:33.000000 numpyneuron-0.6/numpyneuron.egg-info/dependency_links.txt
+-rw-r--r--   0 jensen     (501) staff       (20)       18 2024-04-21 04:38:33.000000 numpyneuron-0.6/numpyneuron.egg-info/requires.txt
+-rw-r--r--   0 jensen     (501) staff       (20)       12 2024-04-21 04:38:33.000000 numpyneuron-0.6/numpyneuron.egg-info/top_level.txt
+-rw-r--r--   0 jensen     (501) staff       (20)       38 2024-04-21 04:38:33.573926 numpyneuron-0.6/setup.cfg
+-rw-r--r--   0 jensen     (501) staff       (20)      660 2024-04-21 04:38:13.000000 numpyneuron-0.6/setup.py
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-21 04:38:33.573218 numpyneuron-0.6/test/
+-rw-r--r--   0 jensen     (501) staff       (20)      197 2024-04-21 04:09:15.000000 numpyneuron-0.6/test/test_activation.py
+-rw-r--r--   0 jensen     (501) staff       (20)      156 2024-04-21 04:09:15.000000 numpyneuron-0.6/test/test_loss.py
+-rw-r--r--   0 jensen     (501) staff       (20)       56 2024-04-21 04:09:55.000000 numpyneuron-0.6/test/test_nn.py
```

### Comparing `numpyneuron-0.5/PKG-INFO` & `numpyneuron-0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: numpyneuron
-Version: 0.5
+Version: 0.6
 Summary: Simple, lightweight neural network framework built in numpy
 Home-page: https://github.com/Jensen-holm/Numpy-Neuron
 Author: Jensen Holm
 Author-email: jensen.dev.01@gmail.com
 Project-URL: Bug Tracker, https://github.com/Jensen-holm/Numpy-Neuron/issues
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: gradio
+Requires-Dist: tqdm
 
 # Numpy-Neuron
 
 A small, simple neural network framework built using only [numpy](https://numpy.org) and python (duh).
 
 ## Install
```

### Comparing `numpyneuron-0.5/README.md` & `numpyneuron-0.6/README.md`

 * *Files identical despite different names*

### Comparing `numpyneuron-0.5/numpyneuron/activation.py` & `numpyneuron-0.6/numpyneuron/activation.py`

 * *Files identical despite different names*

### Comparing `numpyneuron-0.5/numpyneuron/loss.py` & `numpyneuron-0.6/numpyneuron/loss.py`

 * *Files identical despite different names*

### Comparing `numpyneuron-0.5/numpyneuron/nn.py` & `numpyneuron-0.6/numpyneuron/nn.py`

 * *Files identical despite different names*

### Comparing `numpyneuron-0.5/numpyneuron.egg-info/PKG-INFO` & `numpyneuron-0.6/numpyneuron.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: numpyneuron
-Version: 0.5
+Version: 0.6
 Summary: Simple, lightweight neural network framework built in numpy
 Home-page: https://github.com/Jensen-holm/Numpy-Neuron
 Author: Jensen Holm
 Author-email: jensen.dev.01@gmail.com
 Project-URL: Bug Tracker, https://github.com/Jensen-holm/Numpy-Neuron/issues
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: gradio
+Requires-Dist: tqdm
 
 # Numpy-Neuron
 
 A small, simple neural network framework built using only [numpy](https://numpy.org) and python (duh).
 
 ## Install
```


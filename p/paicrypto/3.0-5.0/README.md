# Comparing `tmp/paicrypto-3.0.tar.gz` & `tmp/paicrypto-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paicrypto-3.0.tar", last modified: Sat Apr 20 09:28:06 2024, max compression
+gzip compressed data, was "dist/paicrypto-5.0.tar", last modified: Sun Apr 21 13:59:13 2024, max compression
```

## Comparing `paicrypto-3.0.tar` & `paicrypto-5.0.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxrwxr-x   0 adithya   (1000) adithya   (1000)        0 2024-04-20 09:28:06.131574 paicrypto-3.0/
--rw-rw-r--   0 adithya   (1000) adithya   (1000)     3629 2024-04-20 09:28:06.131574 paicrypto-3.0/PKG-INFO
--rw-rw-r--   0 adithya   (1000) adithya   (1000)     2663 2024-04-20 09:27:36.000000 paicrypto-3.0/README.md
-drwxrwxr-x   0 adithya   (1000) adithya   (1000)        0 2024-04-20 09:28:06.127575 paicrypto-3.0/paicrypto/
--rw-rw-r--   0 adithya   (1000) adithya   (1000)       28 2024-04-20 08:19:28.000000 paicrypto-3.0/paicrypto/__init__.py
--rw-rw-r--   0 adithya   (1000) adithya   (1000)    25164 2024-04-20 09:27:45.000000 paicrypto-3.0/paicrypto/main.py
-drwxrwxr-x   0 adithya   (1000) adithya   (1000)        0 2024-04-20 09:28:06.131574 paicrypto-3.0/paicrypto.egg-info/
--rw-rw-r--   0 adithya   (1000) adithya   (1000)     3629 2024-04-20 09:28:06.000000 paicrypto-3.0/paicrypto.egg-info/PKG-INFO
--rw-rw-r--   0 adithya   (1000) adithya   (1000)      222 2024-04-20 09:28:06.000000 paicrypto-3.0/paicrypto.egg-info/SOURCES.txt
--rw-rw-r--   0 adithya   (1000) adithya   (1000)        1 2024-04-20 09:28:06.000000 paicrypto-3.0/paicrypto.egg-info/dependency_links.txt
--rw-rw-r--   0 adithya   (1000) adithya   (1000)       22 2024-04-20 09:28:06.000000 paicrypto-3.0/paicrypto.egg-info/requires.txt
--rw-rw-r--   0 adithya   (1000) adithya   (1000)       10 2024-04-20 09:28:06.000000 paicrypto-3.0/paicrypto.egg-info/top_level.txt
--rw-rw-r--   0 adithya   (1000) adithya   (1000)       38 2024-04-20 09:28:06.131574 paicrypto-3.0/setup.cfg
--rw-rw-r--   0 adithya   (1000) adithya   (1000)      467 2024-04-20 09:13:24.000000 paicrypto-3.0/setup.py
+drwxrwxr-x   0 adithya   (1000) adithya   (1000)        0 2024-04-21 13:59:13.000000 paicrypto-5.0/
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)     3629 2024-04-21 13:59:13.000000 paicrypto-5.0/PKG-INFO
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)      446 2024-04-21 13:57:50.000000 paicrypto-5.0/setup.py
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)       38 2024-04-21 13:59:13.000000 paicrypto-5.0/setup.cfg
+drwxrwxr-x   0 adithya   (1000) adithya   (1000)        0 2024-04-21 13:59:13.000000 paicrypto-5.0/paicrypto.egg-info/
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)        1 2024-04-21 13:59:13.000000 paicrypto-5.0/paicrypto.egg-info/top_level.txt
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)     3629 2024-04-21 13:59:13.000000 paicrypto-5.0/paicrypto.egg-info/PKG-INFO
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)       13 2024-04-21 13:59:13.000000 paicrypto-5.0/paicrypto.egg-info/requires.txt
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)      182 2024-04-21 13:59:13.000000 paicrypto-5.0/paicrypto.egg-info/SOURCES.txt
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)        1 2024-04-21 13:59:13.000000 paicrypto-5.0/paicrypto.egg-info/dependency_links.txt
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)     2663 2024-04-20 09:27:36.000000 paicrypto-5.0/README.md
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `paicrypto-3.0/PKG-INFO` & `paicrypto-5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paicrypto
-Version: 3.0
+Version: 5.0
 Summary: A collection of algorithms
 Home-page: UNKNOWN
 Author: Adithya Pai B
 Author-email: paiadithya26@gmail.com
 License: UNKNOWN
 Description: # Paicrypto - Cryptographic Library
```

### Comparing `paicrypto-3.0/README.md` & `paicrypto-5.0/README.md`

 * *Files identical despite different names*

### Comparing `paicrypto-3.0/paicrypto.egg-info/PKG-INFO` & `paicrypto-5.0/paicrypto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paicrypto
-Version: 3.0
+Version: 5.0
 Summary: A collection of algorithms
 Home-page: UNKNOWN
 Author: Adithya Pai B
 Author-email: paiadithya26@gmail.com
 License: UNKNOWN
 Description: # Paicrypto - Cryptographic Library
```


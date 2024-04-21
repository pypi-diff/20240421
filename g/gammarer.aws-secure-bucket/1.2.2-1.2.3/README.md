# Comparing `tmp/gammarer.aws-secure-bucket-1.2.2.tar.gz` & `tmp/gammarer.aws-secure-bucket-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-bucket-1.2.2.tar", last modified: Sun Apr 14 22:48:49 2024, max compression
+gzip compressed data, was "gammarer.aws-secure-bucket-1.2.3.tar", last modified: Sun Apr 21 17:14:45 2024, max compression
```

## Comparing `gammarer.aws-secure-bucket-1.2.2.tar` & `gammarer.aws-secure-bucket-1.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:48:49.885000 gammarer.aws-secure-bucket-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-14 22:48:49.885000 gammarer.aws-secure-bucket-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 22:48:49.885000 gammarer.aws-secure-bucket-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:48:49.881000 gammarer.aws-secure-bucket-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:48:49.881000 gammarer.aws-secure-bucket-1.2.2/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:48:49.881000 gammarer.aws-secure-bucket-1.2.2/src/gammarer/aws_secure_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer/aws_secure_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:48:49.885000 gammarer.aws-secure-bucket-1.2.2/src/gammarer/aws_secure_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer/aws_secure_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33689 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer/aws_secure_bucket/_jsii/aws-secure-bucket@1.2.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 22:48:39.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer/aws_secure_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:48:49.881000 gammarer.aws-secure-bucket-1.2.2/src/gammarer.aws_secure_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-14 22:48:49.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer.aws_secure_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-14 22:48:49.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 22:48:49.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer.aws_secure_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-14 22:48:49.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer.aws_secure_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 22:48:49.000000 gammarer.aws-secure-bucket-1.2.2/src/gammarer.aws_secure_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:14:45.766796 gammarer.aws-secure-bucket-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-21 17:14:35.000000 gammarer.aws-secure-bucket-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-21 17:14:35.000000 gammarer.aws-secure-bucket-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-21 17:14:45.766796 gammarer.aws-secure-bucket-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-21 17:14:35.000000 gammarer.aws-secure-bucket-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-21 17:14:35.000000 gammarer.aws-secure-bucket-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 17:14:45.766796 gammarer.aws-secure-bucket-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-21 17:14:35.000000 gammarer.aws-secure-bucket-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:14:45.762796 gammarer.aws-secure-bucket-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:14:45.762796 gammarer.aws-secure-bucket-1.2.3/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:14:45.762796 gammarer.aws-secure-bucket-1.2.3/src/gammarer/aws_secure_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-21 17:14:35.000000 gammarer.aws-secure-bucket-1.2.3/src/gammarer/aws_secure_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:14:45.766796 gammarer.aws-secure-bucket-1.2.3/src/gammarer/aws_secure_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-21 17:14:35.000000 gammarer.aws-secure-bucket-1.2.3/src/gammarer/aws_secure_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33691 2024-04-21 17:14:35.000000 gammarer.aws-secure-bucket-1.2.3/src/gammarer/aws_secure_bucket/_jsii/aws-secure-bucket@1.2.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 17:14:35.000000 gammarer.aws-secure-bucket-1.2.3/src/gammarer/aws_secure_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:14:45.762796 gammarer.aws-secure-bucket-1.2.3/src/gammarer.aws_secure_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-21 17:14:45.000000 gammarer.aws-secure-bucket-1.2.3/src/gammarer.aws_secure_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-21 17:14:45.000000 gammarer.aws-secure-bucket-1.2.3/src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 17:14:45.000000 gammarer.aws-secure-bucket-1.2.3/src/gammarer.aws_secure_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-21 17:14:45.000000 gammarer.aws-secure-bucket-1.2.3/src/gammarer.aws_secure_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 17:14:45.000000 gammarer.aws-secure-bucket-1.2.3/src/gammarer.aws_secure_bucket.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-bucket-1.2.2/LICENSE` & `gammarer.aws-secure-bucket-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-bucket-1.2.2/PKG-INFO` & `gammarer.aws-secure-bucket-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-bucket
-Version: 1.2.2
+Version: 1.2.3
 Summary: This is a Simple S3 Secure Bucket.
 Home-page: https://github.com/gammarer/aws-secure-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-bucket-1.2.2/README.md` & `gammarer.aws-secure-bucket-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-bucket-1.2.2/setup.py` & `gammarer.aws-secure-bucket-1.2.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-bucket",
-    "version": "1.2.2",
+    "version": "1.2.3",
     "description": "This is a Simple S3 Secure Bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-secure-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_secure_bucket",
         "gammarer.aws_secure_bucket._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_bucket._jsii": [
-            "aws-secure-bucket@1.2.2.jsii.tgz"
+            "aws-secure-bucket@1.2.3.jsii.tgz"
         ],
         "gammarer.aws_secure_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarer.aws-secure-bucket-1.2.2/src/gammarer/aws_secure_bucket/__init__.py` & `gammarer.aws-secure-bucket-1.2.3/src/gammarer/aws_secure_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-bucket-1.2.2/src/gammarer.aws_secure_bucket.egg-info/PKG-INFO` & `gammarer.aws-secure-bucket-1.2.3/src/gammarer.aws_secure_bucket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-bucket
-Version: 1.2.2
+Version: 1.2.3
 Summary: This is a Simple S3 Secure Bucket.
 Home-page: https://github.com/gammarer/aws-secure-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-bucket-1.2.2/src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt` & `gammarer.aws-secure-bucket-1.2.3/src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt
 src/gammarer.aws_secure_bucket.egg-info/dependency_links.txt
 src/gammarer.aws_secure_bucket.egg-info/requires.txt
 src/gammarer.aws_secure_bucket.egg-info/top_level.txt
 src/gammarer/aws_secure_bucket/__init__.py
 src/gammarer/aws_secure_bucket/py.typed
 src/gammarer/aws_secure_bucket/_jsii/__init__.py
-src/gammarer/aws_secure_bucket/_jsii/aws-secure-bucket@1.2.2.jsii.tgz
+src/gammarer/aws_secure_bucket/_jsii/aws-secure-bucket@1.2.3.jsii.tgz
```


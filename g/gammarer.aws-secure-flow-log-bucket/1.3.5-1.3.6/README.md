# Comparing `tmp/gammarer.aws-secure-flow-log-bucket-1.3.5.tar.gz` & `tmp/gammarer.aws-secure-flow-log-bucket-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-flow-log-bucket-1.3.5.tar", last modified: Sun Apr 14 23:05:42 2024, max compression
+gzip compressed data, was "gammarer.aws-secure-flow-log-bucket-1.3.6.tar", last modified: Sun Apr 21 19:20:52 2024, max compression
```

## Comparing `gammarer.aws-secure-flow-log-bucket-1.3.5.tar` & `gammarer.aws-secure-flow-log-bucket-1.3.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:05:42.900792 gammarer.aws-secure-flow-log-bucket-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-14 23:05:32.000000 gammarer.aws-secure-flow-log-bucket-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-14 23:05:32.000000 gammarer.aws-secure-flow-log-bucket-1.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-14 23:05:42.900792 gammarer.aws-secure-flow-log-bucket-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-14 23:05:32.000000 gammarer.aws-secure-flow-log-bucket-1.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-14 23:05:32.000000 gammarer.aws-secure-flow-log-bucket-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 23:05:42.900792 gammarer.aws-secure-flow-log-bucket-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-14 23:05:32.000000 gammarer.aws-secure-flow-log-bucket-1.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:05:42.896793 gammarer.aws-secure-flow-log-bucket-1.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:05:42.896793 gammarer.aws-secure-flow-log-bucket-1.3.5/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:05:42.896793 gammarer.aws-secure-flow-log-bucket-1.3.5/src/gammarer/aws_secure_flow_log_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-04-14 23:05:32.000000 gammarer.aws-secure-flow-log-bucket-1.3.5/src/gammarer/aws_secure_flow_log_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:05:42.896793 gammarer.aws-secure-flow-log-bucket-1.3.5/src/gammarer/aws_secure_flow_log_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-14 23:05:32.000000 gammarer.aws-secure-flow-log-bucket-1.3.5/src/gammarer/aws_secure_flow_log_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24325 2024-04-14 23:05:32.000000 gammarer.aws-secure-flow-log-bucket-1.3.5/src/gammarer/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@1.3.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:05:32.000000 gammarer.aws-secure-flow-log-bucket-1.3.5/src/gammarer/aws_secure_flow_log_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:05:42.896793 gammarer.aws-secure-flow-log-bucket-1.3.5/src/gammarer.aws_secure_flow_log_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-14 23:05:42.000000 gammarer.aws-secure-flow-log-bucket-1.3.5/src/gammarer.aws_secure_flow_log_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-14 23:05:42.000000 gammarer.aws-secure-flow-log-bucket-1.3.5/src/gammarer.aws_secure_flow_log_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:05:42.000000 gammarer.aws-secure-flow-log-bucket-1.3.5/src/gammarer.aws_secure_flow_log_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-14 23:05:42.000000 gammarer.aws-secure-flow-log-bucket-1.3.5/src/gammarer.aws_secure_flow_log_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 23:05:42.000000 gammarer.aws-secure-flow-log-bucket-1.3.5/src/gammarer.aws_secure_flow_log_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:20:52.833952 gammarer.aws-secure-flow-log-bucket-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-21 19:20:41.000000 gammarer.aws-secure-flow-log-bucket-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-21 19:20:41.000000 gammarer.aws-secure-flow-log-bucket-1.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-21 19:20:52.833952 gammarer.aws-secure-flow-log-bucket-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-21 19:20:41.000000 gammarer.aws-secure-flow-log-bucket-1.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-21 19:20:41.000000 gammarer.aws-secure-flow-log-bucket-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:20:52.833952 gammarer.aws-secure-flow-log-bucket-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-21 19:20:41.000000 gammarer.aws-secure-flow-log-bucket-1.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:20:52.829951 gammarer.aws-secure-flow-log-bucket-1.3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:20:52.829951 gammarer.aws-secure-flow-log-bucket-1.3.6/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:20:52.833952 gammarer.aws-secure-flow-log-bucket-1.3.6/src/gammarer/aws_secure_flow_log_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-04-21 19:20:41.000000 gammarer.aws-secure-flow-log-bucket-1.3.6/src/gammarer/aws_secure_flow_log_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:20:52.833952 gammarer.aws-secure-flow-log-bucket-1.3.6/src/gammarer/aws_secure_flow_log_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-21 19:20:41.000000 gammarer.aws-secure-flow-log-bucket-1.3.6/src/gammarer/aws_secure_flow_log_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24326 2024-04-21 19:20:41.000000 gammarer.aws-secure-flow-log-bucket-1.3.6/src/gammarer/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@1.3.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:20:41.000000 gammarer.aws-secure-flow-log-bucket-1.3.6/src/gammarer/aws_secure_flow_log_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:20:52.833952 gammarer.aws-secure-flow-log-bucket-1.3.6/src/gammarer.aws_secure_flow_log_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-21 19:20:52.000000 gammarer.aws-secure-flow-log-bucket-1.3.6/src/gammarer.aws_secure_flow_log_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-21 19:20:52.000000 gammarer.aws-secure-flow-log-bucket-1.3.6/src/gammarer.aws_secure_flow_log_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:20:52.000000 gammarer.aws-secure-flow-log-bucket-1.3.6/src/gammarer.aws_secure_flow_log_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-21 19:20:52.000000 gammarer.aws-secure-flow-log-bucket-1.3.6/src/gammarer.aws_secure_flow_log_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 19:20:52.000000 gammarer.aws-secure-flow-log-bucket-1.3.6/src/gammarer.aws_secure_flow_log_bucket.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-flow-log-bucket-1.3.5/LICENSE` & `gammarer.aws-secure-flow-log-bucket-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-flow-log-bucket-1.3.5/PKG-INFO` & `gammarer.aws-secure-flow-log-bucket-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-flow-log-bucket
-Version: 1.3.5
+Version: 1.3.6
 Summary: Specific AWS VPC FlowLog Bucket
 Home-page: https://github.com/gammarer/aws-secure-flow-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-flow-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-flow-log-bucket-1.3.5/README.md` & `gammarer.aws-secure-flow-log-bucket-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-flow-log-bucket-1.3.5/setup.py` & `gammarer.aws-secure-flow-log-bucket-1.3.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-flow-log-bucket",
-    "version": "1.3.5",
+    "version": "1.3.6",
     "description": "Specific AWS VPC FlowLog Bucket",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-secure-flow-log-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_secure_flow_log_bucket",
         "gammarer.aws_secure_flow_log_bucket._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_flow_log_bucket._jsii": [
-            "aws-secure-flow-log-bucket@1.3.5.jsii.tgz"
+            "aws-secure-flow-log-bucket@1.3.6.jsii.tgz"
         ],
         "gammarer.aws_secure_flow_log_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarer.aws-secure-flow-log-bucket-1.3.5/src/gammarer/aws_secure_flow_log_bucket/__init__.py` & `gammarer.aws-secure-flow-log-bucket-1.3.6/src/gammarer/aws_secure_flow_log_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-flow-log-bucket-1.3.5/src/gammarer/aws_secure_flow_log_bucket/_jsii/__init__.py` & `gammarer.aws-secure-flow-log-bucket-1.3.6/src/gammarer/aws_secure_flow_log_bucket/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 import aws_cdk._jsii
 import constructs._jsii
 import gammarer.aws_secure_bucket._jsii
 import gammarer.aws_secure_log_bucket._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarer/aws-secure-flow-log-bucket",
-    "1.3.5",
+    "1.3.6",
     __name__[0:-6],
-    "aws-secure-flow-log-bucket@1.3.5.jsii.tgz",
+    "aws-secure-flow-log-bucket@1.3.6.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarer.aws-secure-flow-log-bucket-1.3.5/src/gammarer.aws_secure_flow_log_bucket.egg-info/PKG-INFO` & `gammarer.aws-secure-flow-log-bucket-1.3.6/src/gammarer.aws_secure_flow_log_bucket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-flow-log-bucket
-Version: 1.3.5
+Version: 1.3.6
 Summary: Specific AWS VPC FlowLog Bucket
 Home-page: https://github.com/gammarer/aws-secure-flow-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-flow-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-flow-log-bucket-1.3.5/src/gammarer.aws_secure_flow_log_bucket.egg-info/SOURCES.txt` & `gammarer.aws-secure-flow-log-bucket-1.3.6/src/gammarer.aws_secure_flow_log_bucket.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_flow_log_bucket.egg-info/SOURCES.txt
 src/gammarer.aws_secure_flow_log_bucket.egg-info/dependency_links.txt
 src/gammarer.aws_secure_flow_log_bucket.egg-info/requires.txt
 src/gammarer.aws_secure_flow_log_bucket.egg-info/top_level.txt
 src/gammarer/aws_secure_flow_log_bucket/__init__.py
 src/gammarer/aws_secure_flow_log_bucket/py.typed
 src/gammarer/aws_secure_flow_log_bucket/_jsii/__init__.py
-src/gammarer/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@1.3.5.jsii.tgz
+src/gammarer/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@1.3.6.jsii.tgz
```


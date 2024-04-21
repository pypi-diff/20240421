# Comparing `tmp/gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1.tar.gz` & `tmp/gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1.tar", last modified: Sun Apr 14 23:00:27 2024, max compression
+gzip compressed data, was "gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2.tar", last modified: Sun Apr 21 18:23:16 2024, max compression
```

## Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1.tar` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:00:27.739603 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-14 23:00:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-14 23:00:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-14 23:00:27.739603 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-14 23:00:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-14 23:00:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 23:00:27.739603 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-14 23:00:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:00:27.739603 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:00:27.739603 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:00:27.739603 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/
--rw-r--r--   0 runner    (1001) docker     (127)    18745 2024-04-14 23:00:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:00:27.739603 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-14 23:00:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24442 2024-04-14 23:00:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@1.2.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:00:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:00:27.739603 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-14 23:00:27.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-14 23:00:27.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:00:27.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-14 23:00:27.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 23:00:27.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:23:16.695970 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-21 18:23:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-21 18:23:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-21 18:23:16.695970 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-21 18:23:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-21 18:23:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 18:23:16.695970 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-21 18:23:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:23:16.695970 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:23:16.695970 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:23:16.695970 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)    18745 2024-04-21 18:23:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:23:16.695970 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-21 18:23:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24442 2024-04-21 18:23:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@1.2.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 18:23:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:23:16.695970 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-21 18:23:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-21 18:23:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 18:23:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-21 18:23:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 18:23:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/LICENSE` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/PKG-INFO` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-frontend-web-app-cloudfront-distribution
-Version: 1.2.1
+Version: 1.2.2
 Summary: AWS CloudFront distribution for frontend web app (spa) optimized.
 Home-page: https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/README.md` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/setup.py` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-frontend-web-app-cloudfront-distribution",
-    "version": "1.2.1",
+    "version": "1.2.2",
     "description": "AWS CloudFront distribution for frontend web app (spa) optimized.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution",
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii": [
-            "aws-secure-frontend-web-app-cloudfront-distribution@1.2.1.jsii.tgz"
+            "aws-secure-frontend-web-app-cloudfront-distribution@1.2.2.jsii.tgz"
         ],
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarer/aws-secure-frontend-web-app-cloudfront-distribution",
-    "1.2.1",
+    "1.2.2",
     __name__[0:-6],
-    "aws-secure-frontend-web-app-cloudfront-distribution@1.2.1.jsii.tgz",
+    "aws-secure-frontend-web-app-cloudfront-distribution@1.2.2.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-frontend-web-app-cloudfront-distribution
-Version: 1.2.1
+Version: 1.2.2
 Summary: AWS CloudFront distribution for frontend web app (spa) optimized.
 Home-page: https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.1/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.2/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
-src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@1.2.1.jsii.tgz
+src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@1.2.2.jsii.tgz
```


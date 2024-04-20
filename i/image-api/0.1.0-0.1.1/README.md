# Comparing `tmp/image_api-0.1.0.tar.gz` & `tmp/image_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_api-0.1.0.tar", last modified: Sun Apr 14 06:46:20 2024, max compression
+gzip compressed data, was "image_api-0.1.1.tar", last modified: Sat Apr 20 22:51:30 2024, max compression
```

## Comparing `image_api-0.1.0.tar` & `image_api-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 lkaijie   (1000) lkaijie   (1000)        0 2024-04-14 06:46:20.198142 image_api-0.1.0/
--rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)      523 2024-04-14 06:46:20.198142 image_api-0.1.0/PKG-INFO
--rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)        0 2024-04-14 00:11:52.000000 image_api-0.1.0/README.md
-drwxr-xr-x   0 lkaijie   (1000) lkaijie   (1000)        0 2024-04-14 06:46:20.198142 image_api-0.1.0/image_api/
--rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)      109 2024-04-14 06:36:40.000000 image_api-0.1.0/image_api/__init__.py
--rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)      411 2024-04-06 16:48:18.000000 image_api-0.1.0/image_api/_base.py
--rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)     2967 2024-04-14 00:23:45.000000 image_api-0.1.0/image_api/_image_api.py
--rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)     2111 2024-04-14 00:24:06.000000 image_api-0.1.0/image_api/_image_item.py
--rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)       81 2024-04-14 00:02:25.000000 image_api-0.1.0/image_api/config.py
-drwxr-xr-x   0 lkaijie   (1000) lkaijie   (1000)        0 2024-04-14 06:46:20.198142 image_api-0.1.0/image_api.egg-info/
--rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)      523 2024-04-14 06:46:20.000000 image_api-0.1.0/image_api.egg-info/PKG-INFO
--rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)      307 2024-04-14 06:46:20.000000 image_api-0.1.0/image_api.egg-info/SOURCES.txt
--rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)        1 2024-04-14 06:46:20.000000 image_api-0.1.0/image_api.egg-info/dependency_links.txt
--rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)       24 2024-04-14 06:46:20.000000 image_api-0.1.0/image_api.egg-info/requires.txt
--rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)       10 2024-04-14 06:46:20.000000 image_api-0.1.0/image_api.egg-info/top_level.txt
--rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)       81 2024-04-14 06:43:09.000000 image_api-0.1.0/pyproject.toml
--rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)       38 2024-04-14 06:46:20.198142 image_api-0.1.0/setup.cfg
--rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)      798 2024-04-14 06:45:25.000000 image_api-0.1.0/setup.py
+drwxr-xr-x   0 lkaijie   (1000) lkaijie   (1000)        0 2024-04-20 22:51:30.977752 image_api-0.1.1/
+-rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)      523 2024-04-20 22:51:30.977752 image_api-0.1.1/PKG-INFO
+-rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)        0 2024-04-14 00:11:52.000000 image_api-0.1.1/README.md
+drwxr-xr-x   0 lkaijie   (1000) lkaijie   (1000)        0 2024-04-20 22:51:30.967752 image_api-0.1.1/image_api/
+-rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)      111 2024-04-20 22:08:08.000000 image_api-0.1.1/image_api/__init__.py
+-rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)      390 2024-04-16 03:46:54.000000 image_api-0.1.1/image_api/_base.py
+-rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)     3256 2024-04-20 22:47:02.000000 image_api-0.1.1/image_api/_image_api.py
+-rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)     2111 2024-04-14 00:24:06.000000 image_api-0.1.1/image_api/_image_item.py
+-rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)       81 2024-04-14 00:02:25.000000 image_api-0.1.1/image_api/config.py
+drwxr-xr-x   0 lkaijie   (1000) lkaijie   (1000)        0 2024-04-20 22:51:30.977752 image_api-0.1.1/image_api.egg-info/
+-rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)      523 2024-04-20 22:51:30.000000 image_api-0.1.1/image_api.egg-info/PKG-INFO
+-rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)      307 2024-04-20 22:51:30.000000 image_api-0.1.1/image_api.egg-info/SOURCES.txt
+-rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)        1 2024-04-20 22:51:30.000000 image_api-0.1.1/image_api.egg-info/dependency_links.txt
+-rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)       24 2024-04-20 22:51:30.000000 image_api-0.1.1/image_api.egg-info/requires.txt
+-rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)       10 2024-04-20 22:51:30.000000 image_api-0.1.1/image_api.egg-info/top_level.txt
+-rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)       81 2024-04-14 06:43:09.000000 image_api-0.1.1/pyproject.toml
+-rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)       38 2024-04-20 22:51:30.977752 image_api-0.1.1/setup.cfg
+-rw-r--r--   0 lkaijie   (1000) lkaijie   (1000)      798 2024-04-20 22:51:27.000000 image_api-0.1.1/setup.py
```

### Comparing `image_api-0.1.0/PKG-INFO` & `image_api-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: A local and lightweight image search API
 Home-page: https://github.com/lkaijie/image-api
 Author: lkaijie
 Author-email: 
 License: MIT
 Keywords: api,myanimelist,bing image,google image,images,google
 Classifier: Programming Language :: Python :: 3
```

### Comparing `image_api-0.1.0/image_api/_image_api.py` & `image_api-0.1.1/image_api/_image_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import json
 from image_api._base import _Base
 import image_api.config as config
-# from _image_item import ImageItem
-# from image_api._image_item import ImageItem
 from image_api._image_item import ImageItem
 
 # low = 640 x 420
 # mid = 1280 x 720
 # high = 1920 x 1080
 
 
@@ -82,14 +80,28 @@
                 'width': img_width,
                 'height': img_height,
                 'format': "." + img_format
             }
             
             imgs.append(ImageItem(img_dict))
         return imgs[:count]
+    
+    def to_json(self, data: list[ImageItem]):
+        """ Convert ImageItem to JSON
+        
+        Args:
+            data (list[ImageItem]): List of ImageItem
             
+            Returns:
+                Json: JSON representation of ImageItem"""
+        
+
+        converted = []
+        for img in data:
+            converted.append(img.__dict__)
+        return converted
 
         
 if __name__ == "__main__":
     api = ImageApi(5)
     api.search("frieren")
     print("done")
```

### Comparing `image_api-0.1.0/image_api/_image_item.py` & `image_api-0.1.1/image_api/_image_item.py`

 * *Files identical despite different names*

### Comparing `image_api-0.1.0/image_api.egg-info/PKG-INFO` & `image_api-0.1.1/image_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: A local and lightweight image search API
 Home-page: https://github.com/lkaijie/image-api
 Author: lkaijie
 Author-email: 
 License: MIT
 Keywords: api,myanimelist,bing image,google image,images,google
 Classifier: Programming Language :: Python :: 3
```

### Comparing `image_api-0.1.0/setup.py` & `image_api-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
     
 setuptools.setup(
     name="image-api",
-    version="0.1.0",
+    version="0.1.1",
     description="A local and lightweight image search API",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="lkaijie",
     author_email="",
     url="https://github.com/lkaijie/image-api",
```


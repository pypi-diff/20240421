# Comparing `tmp/dolibarrpy-0.2.8.tar.gz` & `tmp/dolibarrpy-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolibarrpy-0.2.8.tar", last modified: Sat Apr 20 18:39:46 2024, max compression
+gzip compressed data, was "dolibarrpy-0.2.9.tar", last modified: Sat Apr 20 21:14:57 2024, max compression
```

## Comparing `dolibarrpy-0.2.8.tar` & `dolibarrpy-0.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 18:39:46.413258 dolibarrpy-0.2.8/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.2.8/LICENSE.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 18:39:46.413422 dolibarrpy-0.2.8/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.2.8/README.md
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 18:39:46.411055 dolibarrpy-0.2.8/dolibarrpy/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)    18363 2024-04-20 18:38:11.000000 dolibarrpy-0.2.8/dolibarrpy/Dolibarrpy.py
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.2.8/dolibarrpy/__init__.py
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 18:39:46.412894 dolibarrpy-0.2.8/dolibarrpy.egg-info/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 18:39:46.000000 dolibarrpy-0.2.8/dolibarrpy.egg-info/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 18:39:46.000000 dolibarrpy-0.2.8/dolibarrpy.egg-info/SOURCES.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 18:39:46.000000 dolibarrpy-0.2.8/dolibarrpy.egg-info/dependency_links.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 18:39:46.000000 dolibarrpy-0.2.8/dolibarrpy.egg-info/top_level.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 18:39:46.413873 dolibarrpy-0.2.8/setup.cfg
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-20 17:58:43.000000 dolibarrpy-0.2.8/setup.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 21:14:57.082627 dolibarrpy-0.2.9/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.2.9/LICENSE.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 21:14:57.082769 dolibarrpy-0.2.9/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.2.9/README.md
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 21:14:57.080623 dolibarrpy-0.2.9/dolibarrpy/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)    20880 2024-04-20 20:56:47.000000 dolibarrpy-0.2.9/dolibarrpy/Dolibarrpy.py
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.2.9/dolibarrpy/__init__.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 21:14:57.082360 dolibarrpy-0.2.9/dolibarrpy.egg-info/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 21:14:57.000000 dolibarrpy-0.2.9/dolibarrpy.egg-info/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 21:14:57.000000 dolibarrpy-0.2.9/dolibarrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 21:14:57.000000 dolibarrpy-0.2.9/dolibarrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 21:14:57.000000 dolibarrpy-0.2.9/dolibarrpy.egg-info/top_level.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 21:14:57.083224 dolibarrpy-0.2.9/setup.cfg
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-20 20:37:25.000000 dolibarrpy-0.2.9/setup.py
```

### Comparing `dolibarrpy-0.2.8/LICENSE.txt` & `dolibarrpy-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolibarrpy-0.2.8/PKG-INFO` & `dolibarrpy-0.2.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.2.8/dolibarrpy/Dolibarrpy.py` & `dolibarrpy-0.2.9/dolibarrpy/Dolibarrpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -528,7 +528,71 @@
         if 0 == limit:
             raise Exception("sorry, but a limit if 0 does not make sense, be sensible")
         typeid = params.get("typeid")
         if typeid:
             raise Exception("sorry, you can not use typeid in this filter, try without")
         result = self.call_list_api('members/types', params=params)
         return result
+
+    def get_all_member_categories_by_mid(self, objid, from_MemberFilter = None):
+        """
+        Get all categories for a member
+        @param from_MemberFilter:
+        @return: list of a members categories
+        """
+        if self.debug:
+            ic()
+            ic(from_MemberFilter)
+        if from_MemberFilter is None:
+            search_filter = MemberFilter()
+        else:
+            search_filter = from_MemberFilter
+        all_member_categories=[]
+        page = 0
+        while True:
+            some_member_categories = self.get_some_member_categories_by_mid(objid, search_filter, page)
+            if self.debug:
+                ic(some_member_categories)
+            if "error" in some_member_categories:
+                break
+            elif [] == some_member_categories:
+                break
+            elif {} == some_member_categories:
+                break
+            else:
+                page += 1
+                if some_member_categories == all_member_categories:
+                    break
+                all_member_categories = all_member_categories + list(some_member_categories)
+        return all_member_categories
+
+    def get_some_member_categories_by_mid(self, objid, from_MemberFilter = None, page = 0):
+        if self.debug:
+            ic()
+            ic(page)
+            ic(from_MemberFilter)
+        if from_MemberFilter is None:
+            search_filter = MemberFilter()
+        else:
+            search_filter = from_MemberFilter
+        search_filter.page = page
+        params = asdict(search_filter)
+        category = params.get("category")
+        if category:
+            raise Exception("sorry, you can not use category in this filter, try without")
+        limit = params.get("limit")
+        if 0 == limit:
+            raise Exception("sorry, but a limit if 0 does not make sense, be sensible")
+        properties = params.get("properties")
+        if properties:
+            raise Exception("sorry, you can not use properties in this filter, try without")
+        sqlfilters = params.get("sqlfilters")
+        if sqlfilters:
+            raise Exception("sorry, you can not use sqlfilters in this filter, try without")
+        typeid = params.get("typeid")
+        if typeid:
+            raise Exception("sorry, you can not use typeid in this filter, try without")
+        api_path = 'members/' + str(objid) + '/categories'
+        result = self.call_list_api(api_path, params)
+        if self.debug:
+            ic(result)
+        return result
```

### Comparing `dolibarrpy-0.2.8/dolibarrpy.egg-info/PKG-INFO` & `dolibarrpy-0.2.9/dolibarrpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.2.8/setup.py` & `dolibarrpy-0.2.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import os
 
 setup(
     name='dolibarrpy',
     packages=['dolibarrpy'],
-    version="0.2.8",
+    version="0.2.9",
     license='MIT',
     description='Python wrapper for Dolibarr API',
     long_description='Python wrapper for Dolibarr',
     long_description_content_type='text/markdown',
     author='Jon Bendtsen',
     author_email='jon.bendtsen.github@jonb.dk',
     url='https://github.com/JonBendtsen/dolibarrpy.git',
```


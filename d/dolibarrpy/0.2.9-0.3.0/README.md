# Comparing `tmp/dolibarrpy-0.2.9.tar.gz` & `tmp/dolibarrpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolibarrpy-0.2.9.tar", last modified: Sat Apr 20 21:14:57 2024, max compression
+gzip compressed data, was "dolibarrpy-0.3.0.tar", last modified: Sat Apr 20 22:01:11 2024, max compression
```

## Comparing `dolibarrpy-0.2.9.tar` & `dolibarrpy-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 21:14:57.082627 dolibarrpy-0.2.9/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.2.9/LICENSE.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 21:14:57.082769 dolibarrpy-0.2.9/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.2.9/README.md
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 21:14:57.080623 dolibarrpy-0.2.9/dolibarrpy/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)    20880 2024-04-20 20:56:47.000000 dolibarrpy-0.2.9/dolibarrpy/Dolibarrpy.py
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.2.9/dolibarrpy/__init__.py
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 21:14:57.082360 dolibarrpy-0.2.9/dolibarrpy.egg-info/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 21:14:57.000000 dolibarrpy-0.2.9/dolibarrpy.egg-info/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 21:14:57.000000 dolibarrpy-0.2.9/dolibarrpy.egg-info/SOURCES.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 21:14:57.000000 dolibarrpy-0.2.9/dolibarrpy.egg-info/dependency_links.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 21:14:57.000000 dolibarrpy-0.2.9/dolibarrpy.egg-info/top_level.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 21:14:57.083224 dolibarrpy-0.2.9/setup.cfg
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-20 20:37:25.000000 dolibarrpy-0.2.9/setup.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 22:01:11.399530 dolibarrpy-0.3.0/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.3.0/LICENSE.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 22:01:11.399679 dolibarrpy-0.3.0/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.3.0/README.md
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 22:01:11.397603 dolibarrpy-0.3.0/dolibarrpy/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)    23103 2024-04-20 22:01:00.000000 dolibarrpy-0.3.0/dolibarrpy/Dolibarrpy.py
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.3.0/dolibarrpy/__init__.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 22:01:11.399260 dolibarrpy-0.3.0/dolibarrpy.egg-info/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 22:01:11.000000 dolibarrpy-0.3.0/dolibarrpy.egg-info/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 22:01:11.000000 dolibarrpy-0.3.0/dolibarrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 22:01:11.000000 dolibarrpy-0.3.0/dolibarrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 22:01:11.000000 dolibarrpy-0.3.0/dolibarrpy.egg-info/top_level.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 22:01:11.400136 dolibarrpy-0.3.0/setup.cfg
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-20 21:51:56.000000 dolibarrpy-0.3.0/setup.py
```

### Comparing `dolibarrpy-0.2.9/LICENSE.txt` & `dolibarrpy-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolibarrpy-0.2.9/PKG-INFO` & `dolibarrpy-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.2.9
+Version: 0.3.0
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.2.9/dolibarrpy/Dolibarrpy.py` & `dolibarrpy-0.3.0/dolibarrpy/Dolibarrpy.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,14 +26,25 @@
     limit: Optional[int] = None
     page: Optional[int] = None          # page number
     typeid: Optional[str] = None        # only get members with this thirdparty_id
     category: Optional[int] = None        # only get members with this status: draft | unpaid | paid | cancelled
     sqlfilters: Optional[str] = None    # (t.email:like:'john.doe@example.com')
     properties: Optional[str] = None    # Restrict the data returned to these properties. Ignored if empty. Comma separated list of properties names
 
+@dataclass
+class ThirdpartyFilter():
+    sortfield: Optional[str] = None
+    sortorder: Optional[str] = None
+    limit: Optional[int] = None
+    page: Optional[int] = None          # page number
+    mode: Optional[int] = None          # Set to 1 to show only customers Set to 2 to show only prospects Set to 3 to show only those are not customer neither prospect Set to 4 to show only suppliers
+    category: Optional[int] = None      # only get members with this status: draft | unpaid | paid | cancelled
+    sqlfilters: Optional[str] = None    # (t.email:like:'john.doe@example.com')
+    properties: Optional[str] = None    # Restrict the data returned to these properties. Ignored if empty. Comma separated list of properties names
+
 class Dolibarrpy():
     url = 'https://dolibarr.example.com/api/index.php/'
     token = 'your token'
     timeout = 16
     debug = False
 
     def __init__(self, url, token, timeout, debug):
@@ -592,7 +603,53 @@
         if typeid:
             raise Exception("sorry, you can not use typeid in this filter, try without")
         api_path = 'members/' + str(objid) + '/categories'
         result = self.call_list_api(api_path, params)
         if self.debug:
             ic(result)
         return result
+
+
+    # THIRDPARTIES
+    def find_all_thirdparty(self, from_ThirdpartyFilter = None):
+        """
+        Get all thirdparties
+        @param from_ThirdpartyFilter:
+        @return: list of a thirdparties
+        """
+        if self.debug:
+            ic()
+            ic(from_ThirdpartyFilter)
+        if from_ThirdpartyFilter is None:
+            search_filter = ThirdpartyFilter()
+        else:
+            search_filter = from_ThirdpartyFilter
+        all_thirdparty=[]
+        page = 0
+        while True:
+            some_thirdparty = self.find_some_thirdparty(search_filter, page)
+            if "error" in some_thirdparty:
+                break
+            elif [] == some_thirdparty:
+                break
+            elif {} == some_thirdparty:
+                break
+            else:
+                page += 1
+                if some_thirdparty == all_thirdparty:
+                    break
+                all_thirdparty = all_thirdparty + list(some_thirdparty)
+        return all_thirdparty
+
+    def find_some_thirdparty(self, from_ThirdpartyFilter = None, page = 0):
+        if self.debug:
+            ic()
+            ic(page)
+            ic(from_ThirdpartyFilter)
+        if from_ThirdpartyFilter is None:
+            search_filter = ThirdpartyFilter()
+        else:
+            search_filter = from_ThirdpartyFilter
+        search_filter.page = page
+        params = asdict(search_filter)
+        result = self.call_list_api('thirdparties', params)
+        return result
```

### Comparing `dolibarrpy-0.2.9/dolibarrpy.egg-info/PKG-INFO` & `dolibarrpy-0.3.0/dolibarrpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.2.9
+Version: 0.3.0
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.2.9/setup.py` & `dolibarrpy-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import os
 
 setup(
     name='dolibarrpy',
     packages=['dolibarrpy'],
-    version="0.2.9",
+    version="0.3.0",
     license='MIT',
     description='Python wrapper for Dolibarr API',
     long_description='Python wrapper for Dolibarr',
     long_description_content_type='text/markdown',
     author='Jon Bendtsen',
     author_email='jon.bendtsen.github@jonb.dk',
     url='https://github.com/JonBendtsen/dolibarrpy.git',
```


# Comparing `tmp/teaching-toolshed-0.2.8.tar.gz` & `tmp/teaching-toolshed-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teaching-toolshed-0.2.8.tar", max compression
+gzip compressed data, was "teaching-toolshed-0.2.9.tar", max compression
```

## Comparing `teaching-toolshed-0.2.8.tar` & `teaching-toolshed-0.2.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2021-12-29 18:48:12.748860 teaching-toolshed-0.2.8/LICENSE
--rw-r--r--   0        0        0      618 2022-10-08 02:56:12.775030 teaching-toolshed-0.2.8/README.md
--rw-r--r--   0        0        0      494 2024-01-23 21:10:07.296798 teaching-toolshed-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      132 2023-03-21 03:10:15.106159 teaching-toolshed-0.2.8/teachingtoolshed/__init__.py
--rw-r--r--   0        0        0       21 2021-12-29 18:48:12.749403 teaching-toolshed-0.2.8/teachingtoolshed/api/__init__.py
--rw-r--r--   0        0        0    24357 2024-01-23 21:10:07.291035 teaching-toolshed-0.2.8/teachingtoolshed/api/edstem.py
--rw-r--r--   0        0        0       94 2021-12-29 18:48:12.749634 teaching-toolshed-0.2.8/teachingtoolshed/gradebook/__init__.py
--rw-r--r--   0        0        0     7356 2022-12-20 03:05:41.303371 teaching-toolshed-0.2.8/teachingtoolshed/gradebook/canvas.py
--rw-r--r--   0        0        0     4424 2023-11-03 04:07:28.527354 teaching-toolshed-0.2.8/teachingtoolshed/gradebook/csv_readers.py
--rw-r--r--   0        0        0     1421 1970-01-01 00:00:00.000000 teaching-toolshed-0.2.8/setup.py
--rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 teaching-toolshed-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2021-12-29 18:48:12.748860 teaching-toolshed-0.2.9/LICENSE
+-rw-r--r--   0        0        0      618 2022-10-08 02:56:12.775030 teaching-toolshed-0.2.9/README.md
+-rw-r--r--   0        0        0      494 2024-04-21 02:16:19.425228 teaching-toolshed-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      132 2023-03-21 03:10:15.106159 teaching-toolshed-0.2.9/teachingtoolshed/__init__.py
+-rw-r--r--   0        0        0       21 2021-12-29 18:48:12.749403 teaching-toolshed-0.2.9/teachingtoolshed/api/__init__.py
+-rw-r--r--   0        0        0    24750 2024-04-21 02:15:44.225261 teaching-toolshed-0.2.9/teachingtoolshed/api/edstem.py
+-rw-r--r--   0        0        0       94 2021-12-29 18:48:12.749634 teaching-toolshed-0.2.9/teachingtoolshed/gradebook/__init__.py
+-rw-r--r--   0        0        0     7356 2022-12-20 03:05:41.303371 teaching-toolshed-0.2.9/teachingtoolshed/gradebook/canvas.py
+-rw-r--r--   0        0        0     4424 2023-11-03 04:07:28.527354 teaching-toolshed-0.2.9/teachingtoolshed/gradebook/csv_readers.py
+-rw-r--r--   0        0        0     1421 1970-01-01 00:00:00.000000 teaching-toolshed-0.2.9/setup.py
+-rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 teaching-toolshed-0.2.9/PKG-INFO
```

### Comparing `teaching-toolshed-0.2.8/LICENSE` & `teaching-toolshed-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `teaching-toolshed-0.2.8/README.md` & `teaching-toolshed-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `teaching-toolshed-0.2.8/teachingtoolshed/api/edstem.py` & `teaching-toolshed-0.2.9/teachingtoolshed/api/edstem.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """
 import itertools
 import json
 from typing import Any, Dict, List, Optional
 
 import requests
 from requests.adapters import HTTPAdapter
-from urllib3.util import Retry
+from urllib3.util import Retry, retry
 
 # Special type to indicate only a 0 or 1 should be passed
 BinaryFlag = int
 
 API_URL = f"https://us.edstem.org/api/"
 
 
@@ -43,29 +43,38 @@
     """
     Same as url_join but prepends parts with the API_URL
     """
     return url_join(API_URL, *parts)
 
 
 class EdStemAPI:
-    def __init__(self, course_id: int, token: str):
+    def __init__(
+        self,
+        course_id: int,
+        token: str,
+        max_retries: int = 10,
+        retry_factor: float = 0.5,
+    ):
         """Initializes access to the EdStem API for a course with the given ID.
 
 
         Args:
             course_id: An integer course ID for the course to access. See EdStem URL.
             token: Your EdStem authentication token
+            max_retires: In the case of a rate limit, how many times we retry the request (default 10)
+            retry_factor: Controls the spacing of time between retries. If the i^th retry fails, will wait
+                          retry_factor * (2 ** i) seconds
         """
         self._course_id = course_id
         self._token = token
 
         # Initialize requests with retry
         retry_strategy = Retry(
-            total=4,
-            backoff_factor=2,
+            total=max_retries,
+            backoff_factor=retry_factor,
             status_forcelist=[429],
         )
         adapter = HTTPAdapter(max_retries=retry_strategy)
 
         self._requests = requests.Session()
         self._requests.mount("http://", adapter=adapter)
         self._requests.mount("https://", adapter=adapter)
```

### Comparing `teaching-toolshed-0.2.8/teachingtoolshed/gradebook/canvas.py` & `teaching-toolshed-0.2.9/teachingtoolshed/gradebook/canvas.py`

 * *Files identical despite different names*

### Comparing `teaching-toolshed-0.2.8/teachingtoolshed/gradebook/csv_readers.py` & `teaching-toolshed-0.2.9/teachingtoolshed/gradebook/csv_readers.py`

 * *Files identical despite different names*

### Comparing `teaching-toolshed-0.2.8/setup.py` & `teaching-toolshed-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pandas>=2.1.0,<3.0.0', 'pre-commit>=3.6.0,<4.0.0', 'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'teaching-toolshed',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Helpful libraries for running classes',
     'long_description': '# Teaching Toolshed\n\nA library of useful classes for writing scripts related to managing classes. Has helper classes for talking to various teaching APIs and for compiling gradebooks in Python. \n\nSee [Teaching Toolshed Examples](https://github.com/hschafer/teaching-toolshed-examples) to see example scripts of how these libraries are used in my classes.\n\nAny questions or comments can be handled here on GitHub or you can email me at [hschafer@cs.washington.edu](mailto:hschafer@cs.washington.edu).\n\n## Publish New Version\n\nSee [here](https://realpython.com/pypi-publish-python-package/#publish-your-package-to-pypi)\n',
     'author': 'Hunter Schafer',
     'author_email': 'hschafer@uw.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/hschafer/teaching-toolshed',
```

### Comparing `teaching-toolshed-0.2.8/PKG-INFO` & `teaching-toolshed-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teaching-toolshed
-Version: 0.2.8
+Version: 0.2.9
 Summary: Helpful libraries for running classes
 Home-page: https://github.com/hschafer/teaching-toolshed
 License: MIT
 Author: Hunter Schafer
 Author-email: hschafer@uw.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


# Comparing `tmp/zeus_py-1.1.0.tar.gz` & `tmp/zeus_py-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeus_py-1.1.0.tar", last modified: Fri Mar 29 12:34:43 2024, max compression
+gzip compressed data, was "zeus_py-1.1.1.tar", last modified: Sun Apr 21 17:20:39 2024, max compression
```

## Comparing `zeus_py-1.1.0.tar` & `zeus_py-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:34:43.585844 zeus_py-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-29 12:34:43.585844 zeus_py-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-29 12:34:33.000000 zeus_py-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 12:34:43.585844 zeus_py-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-29 12:34:41.000000 zeus_py-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:34:43.581843 zeus_py-1.1.0/zeus_py/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-29 12:34:41.000000 zeus_py-1.1.0/zeus_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-03-29 12:34:41.000000 zeus_py-1.1.0/zeus_py/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:34:43.585844 zeus_py-1.1.0/zeus_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-29 12:34:43.000000 zeus_py-1.1.0/zeus_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-29 12:34:43.000000 zeus_py-1.1.0/zeus_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 12:34:43.000000 zeus_py-1.1.0/zeus_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-29 12:34:43.000000 zeus_py-1.1.0/zeus_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-29 12:34:43.000000 zeus_py-1.1.0/zeus_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:20:39.003133 zeus_py-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-21 17:20:39.003133 zeus_py-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-21 17:20:29.000000 zeus_py-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 17:20:39.003133 zeus_py-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-21 17:20:36.000000 zeus_py-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:20:39.003133 zeus_py-1.1.1/zeus_py/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-21 17:20:36.000000 zeus_py-1.1.1/zeus_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-04-21 17:20:36.000000 zeus_py-1.1.1/zeus_py/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:20:39.003133 zeus_py-1.1.1/zeus_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-21 17:20:38.000000 zeus_py-1.1.1/zeus_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-21 17:20:38.000000 zeus_py-1.1.1/zeus_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 17:20:38.000000 zeus_py-1.1.1/zeus_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-21 17:20:38.000000 zeus_py-1.1.1/zeus_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 17:20:38.000000 zeus_py-1.1.1/zeus_py.egg-info/top_level.txt
```

### Comparing `zeus_py-1.1.0/PKG-INFO` & `zeus_py-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeus_py
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple wrapper written in Python for the Zeus API.
 Home-page: https://github.com/EPI-Companion/zeus.py
 Author: C&S
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ==3.12.*
 Description-Content-Type: text/markdown
 Requires-Dist: httpx==0.27.0
@@ -16,16 +16,16 @@
 [![PyPi](https://img.shields.io/pypi/v/zeus-py)](https://pypi.org/project/zeus-py/)
 [![Upload Python Package](https://github.com/EPI-Companion/zeus.py/actions/workflows/python-publish.yml/badge.svg?branch=main)](https://github.com/EPI-Companion/zeus.py/actions/workflows/python-publish.yml)
 
 ## Description
 zeus-py is a Python wrapper for the Zeus API. It provides a convenient way to interact with the Zeus platform using Python.
 
 ## Requirements
-- Python 3.11.x or higher
-
+- Python 3.12.x or higher
+Old version of python are not supported by the wrapper (because it's not tested on this specific version)
 ## Installation
 You can install zeus-py using pip:
 
 ```shell
 py -3 -m pip install -U zeus-py
 ```
```

### Comparing `zeus_py-1.1.0/README.md` & `zeus_py-1.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 [![PyPi](https://img.shields.io/pypi/v/zeus-py)](https://pypi.org/project/zeus-py/)
 [![Upload Python Package](https://github.com/EPI-Companion/zeus.py/actions/workflows/python-publish.yml/badge.svg?branch=main)](https://github.com/EPI-Companion/zeus.py/actions/workflows/python-publish.yml)
 
 ## Description
 zeus-py is a Python wrapper for the Zeus API. It provides a convenient way to interact with the Zeus platform using Python.
 
 ## Requirements
-- Python 3.11.x or higher
-
+- Python 3.12.x or higher
+Old version of python are not supported by the wrapper (because it's not tested on this specific version)
 ## Installation
 You can install zeus-py using pip:
 
 ```shell
 py -3 -m pip install -U zeus-py
 ```
```

### Comparing `zeus_py-1.1.0/setup.py` & `zeus_py-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="zeus_py",
-    version="1.1.0",
+    version="1.1.1",
     packages=find_packages(),
     install_requires=["httpx==0.27.0", "requests==2.31.0"],
     author="C&S",
     description="A simple wrapper written in Python for the Zeus API.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/EPI-Companion/zeus.py",
```

### Comparing `zeus_py-1.1.0/zeus_py/core.py` & `zeus_py-1.1.1/zeus_py/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import requests
 
 
 class Zeus:
     def __init__(self):
         self.appId = None
         self.apiKey = None
+        self.__version__ = "1.1.1"
 
     ## Login async-function
     def __login__(self, appId: str) -> None:
         """
         Get the API key from the Zeus API with specifi appID
         In : appId (string)
         Out : None (API key is stored in self.api_key)
@@ -26,19 +27,22 @@
         elif response.status_code == 400:
             raise Exception("Error 400 : Bad request")
         elif response.status_code == 403:
             raise Exception("Error 403 : Access to API is forbidden")
         elif response.status_code == 500:
             raise Exception("Error 500 : Internal server error")
 
+    def version(self) -> None:
+        return self.__version__
+
     def login(self, appId: str) -> None:
         return self.__login__(appId)
 
     # Get some data from the zeus database
-    async def get_groups(self) -> dict:
+    async def get_groups(self, protect=False) -> dict:
         """
         Get all groups referenced in the Zeus database
         In : None
         Out : Groups (dict)
         """
         url = "https://zeus.ionis-it.com/api/group"
         headers = {"accept": "text/plain", "Authorization": f"Bearer {self.api_key}"}
@@ -48,23 +52,28 @@
 
             if response.status_code == 200:
                 return response.json()
             elif response.status_code == 400:
                 raise Exception("Error 400 : Bad request")
             elif response.status_code == 403:
                 try:
-                    self.login(self.appId)
-                    await self.get_groups()
+                    if not protect:
+                        self.login(self.appId, True)
+                        await self.get_groups()
+                    else:
+                        raise Exception(
+                            "Error XXX : Fail to connect. Possibile infinite loop"
+                        )
                 except Exception:
                     raise Exception("Error 403 : Access to API is forbidden")
             elif response.status_code == 500:
                 raise Exception("Error 500 : Internal server error")
 
     # Get some data from the zeus database with specific id (teacher, group, location, course)
-    async def get_course_by_id(self, id: int) -> dict:
+    async def get_course_by_id(self, id: int, protect=False) -> dict:
         """
         Get a specific course in Zeus database with it's specific id
         In : id
         Out : Course
         """
         url = f"https://zeus.ionis-it.com/api/Course/{str(id)}"
         headers = {"accept": "text/plain", "Authorization": f"Bearer {self.api_key}"}
@@ -74,22 +83,25 @@
 
             if response.status_code == 200:
                 return response.json()
             elif response.status_code == 400:
                 raise Exception("Error 400 : Bad request")
             elif response.status_code == 403:
                 try:
-                    self.login(self.appId)
-                    await self.get_course_by_id(id)
+                    if not protect:
+                        self.login(self.appId)
+                        await self.get_course_by_id(id, True)
+                    else:
+                        raise Exception("Erorr unknown : Fail to login")
                 except Exception:
                     raise Exception("Error 403 : Access to API is forbidden")
             elif response.status_code == 500:
                 raise Exception("Error 500 : Internal server error")
 
-    async def get_course_by_teacher(self, id: int) -> dict:
+    async def get_course_by_teacher(self, id: int, protect=False) -> dict:
         """
         Get course in Zeus database with specific teacher
         In : id of the teacher
         Out : Course
         """
         url = f"https://zeus.ionis-it.com/api/Course/Teacher/{str(id)}"
         headers = {"accept": "text/plain", "Authorization": f"Bearer {self.api_key}"}
@@ -99,23 +111,26 @@
 
             if response.status_code == 200:
                 return response.json()
             elif response.status_code == 400:
                 raise Exception("Error 400 : Bad request")
             elif response.status_code == 403:
                 try:
-                    self.login(self.appId)
-                    await self.get_course_by_teacher(id)
+                    if not protect:
+                        self.login(self.appId)
+                        await self.get_course_by_teacher(self, id, True)
+                    else:
+                        raise Exception("Erorr unknown : Fail to login")
                 except Exception:
                     raise Exception("Error 403 : Access to API is forbidden")
             elif response.status_code == 500:
                 raise Exception("Error 500 : Internal server error")
 
     async def get_course_by_group(
-        self, groupId: int, StartDate: str, EndDate: str
+        self, groupId: int, StartDate: str, EndDate: str, protect=False
     ) -> dict:
         """
         Get a course by its group
         In : id of the group, StartDate, EndDate
         Out : Course
         """
         url = f"https://zeus.ionis-it.com/api/reservation/filter/displayable?Groups={str(groupId)}&StartDate={StartDate}&EndDate={EndDate}"
@@ -125,22 +140,29 @@
 
             if response.status_code == 200:
                 return response.json()
             elif response.status_code == 400:
                 raise Exception("Error 400 : Bad request")
             elif response.status_code == 403:
                 try:
-                    self.login(self.appId)
-                    await self.get_course_by_group(groupId, StartDate, EndDate)
+                    if not protect:
+                        self.login(self.appId)
+                        await self.get_course_by_group(
+                            groupId, StartDate, EndDate, True
+                        )
+                    else:
+                        raise Exception(
+                            "Error XXX : fail to login. Possible infinite loop"
+                        )
                 except Exception:
                     raise Exception("Error 403 : Access to API is forbidden")
             elif response.status_code == 500:
                 raise Exception("Error 500 : Internal server error")
 
-    async def get_group_by_id(self, id: int) -> dict:
+    async def get_group_by_id(self, id: int, protect=False) -> dict:
         """
         Get a specific group in Zeus database with it's specific id
         In : id of the group
         Out : group
         """
         url = f"https://zeus.ionis-it.com/api/group/{str(id)}"
         headers = {"accept": "text/plain", "Authorization": f"Bearer {self.api_key}"}
@@ -150,23 +172,28 @@
 
             if response.status_code == 200:
                 return response.json()
             elif response.status_code == 400:
                 raise Exception("Error 400 : Bad request")
             elif response.status_code == 403:
                 try:
-                    self.login(self.appId)
-                    await self.get_group_by_id(id)
+                    if not protect:
+                        self.login(self.appId)
+                        await self.get_group_by_id(id, True)
+                    else:
+                        raise Exception(
+                            "Error XXX : fail to login. Possible infinite loop"
+                        )
                 except Exception:
                     raise Exception("Error 403 : Access to API is forbidden")
             elif response.status_code == 500:
                 raise Exception("Error 500 : Internal server error")
 
     async def get_course_by_location(
-        self, roomId: int, StartDate: str, EndDate: str
+        self, roomId: int, StartDate: str, EndDate: str, protect=False
     ) -> dict:
         """
         Get a course by its group
         In : id of the group, StartDate, EndDate
         Out : Course
         """
         url = f"https://zeus.ionis-it.com/api/reservation/filter/displayable?Rooms={str(roomId)}&StartDate={StartDate}&EndDate={EndDate}"
@@ -176,13 +203,20 @@
 
             if response.status_code == 200:
                 return response.json()
             elif response.status_code == 400:
                 raise Exception("Error 400 : Bad request")
             elif response.status_code == 403:
                 try:
-                    self.login(self.appId)
-                    await self.get_course_by_location(roomId, StartDate, EndDate)
+                    if not protect:
+                        self.login(self.appId)
+                        await self.get_course_by_location(
+                            roomId, StartDate, EndDate, True
+                        )
+                    else:
+                        raise Exception(
+                            "Error XXX : Fail to login. Possibile infinite loop"
+                        )
                 except Exception:
                     raise Exception("Error 403 : Access to API is forbidden")
             elif response.status_code == 500:
                 raise Exception("Error 500 : Internal server error")
```

### Comparing `zeus_py-1.1.0/zeus_py.egg-info/PKG-INFO` & `zeus_py-1.1.1/zeus_py.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeus_py
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple wrapper written in Python for the Zeus API.
 Home-page: https://github.com/EPI-Companion/zeus.py
 Author: C&S
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ==3.12.*
 Description-Content-Type: text/markdown
 Requires-Dist: httpx==0.27.0
@@ -16,16 +16,16 @@
 [![PyPi](https://img.shields.io/pypi/v/zeus-py)](https://pypi.org/project/zeus-py/)
 [![Upload Python Package](https://github.com/EPI-Companion/zeus.py/actions/workflows/python-publish.yml/badge.svg?branch=main)](https://github.com/EPI-Companion/zeus.py/actions/workflows/python-publish.yml)
 
 ## Description
 zeus-py is a Python wrapper for the Zeus API. It provides a convenient way to interact with the Zeus platform using Python.
 
 ## Requirements
-- Python 3.11.x or higher
-
+- Python 3.12.x or higher
+Old version of python are not supported by the wrapper (because it's not tested on this specific version)
 ## Installation
 You can install zeus-py using pip:
 
 ```shell
 py -3 -m pip install -U zeus-py
 ```
```


# Comparing `tmp/scriptime-0.1.6.tar.gz` & `tmp/scriptime-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scriptime-0.1.6.tar", last modified: Thu Jul 27 19:23:01 2023, max compression
+gzip compressed data, was "scriptime-1.0.0.tar", last modified: Sun Apr 21 01:43:39 2024, max compression
```

## Comparing `scriptime-0.1.6.tar` & `scriptime-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-27 19:23:01.201021 scriptime-0.1.6/
--rw-r--r--   0 jakestrasler   (501) staff       (20)     1087 2023-07-09 02:56:28.000000 scriptime-0.1.6/LICENSE
--rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 20:17:09.000000 scriptime-0.1.6/MANIFEST.in
--rw-r--r--   0 jakestrasler   (501) staff       (20)     5401 2023-07-27 19:23:01.200884 scriptime-0.1.6/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)     5091 2023-07-09 02:59:26.000000 scriptime-0.1.6/README.md
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-27 19:23:01.199858 scriptime-0.1.6/scriptime/
--rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 00:08:59.000000 scriptime-0.1.6/scriptime/__init__.py
--rw-r--r--   0 jakestrasler   (501) staff       (20)   701148 2023-07-05 22:10:39.000000 scriptime-0.1.6/scriptime/alert.wav
--rw-r--r--   0 jakestrasler   (501) staff       (20)    10004 2023-07-27 19:21:26.000000 scriptime-0.1.6/scriptime/main.py
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-27 19:23:01.200652 scriptime-0.1.6/scriptime.egg-info/
--rw-r--r--   0 jakestrasler   (501) staff       (20)     5401 2023-07-27 19:23:01.000000 scriptime-0.1.6/scriptime.egg-info/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)      262 2023-07-27 19:23:01.000000 scriptime-0.1.6/scriptime.egg-info/SOURCES.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2023-07-27 19:23:01.000000 scriptime-0.1.6/scriptime.egg-info/dependency_links.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       30 2023-07-27 19:23:01.000000 scriptime-0.1.6/scriptime.egg-info/requires.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2023-07-27 19:23:01.000000 scriptime-0.1.6/scriptime.egg-info/top_level.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2023-07-27 19:23:01.201061 scriptime-0.1.6/setup.cfg
--rw-r--r--   0 jakestrasler   (501) staff       (20)      694 2023-07-27 19:22:59.000000 scriptime-0.1.6/setup.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2024-04-21 01:43:39.558714 scriptime-1.0.0/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     1087 2023-07-09 02:56:28.000000 scriptime-1.0.0/LICENSE
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 20:17:09.000000 scriptime-1.0.0/MANIFEST.in
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     5472 2024-04-21 01:43:39.558490 scriptime-1.0.0/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     5087 2024-04-21 01:41:00.000000 scriptime-1.0.0/README.md
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2024-04-21 01:43:39.557098 scriptime-1.0.0/scriptime/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 00:08:59.000000 scriptime-1.0.0/scriptime/__init__.py
+-rw-r--r--   0 jakestrasler   (501) staff       (20)   701148 2023-07-05 22:10:39.000000 scriptime-1.0.0/scriptime/alert.wav
+-rw-r--r--   0 jakestrasler   (501) staff       (20)    10004 2023-07-27 19:47:09.000000 scriptime-1.0.0/scriptime/main.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2024-04-21 01:43:39.558240 scriptime-1.0.0/scriptime.egg-info/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     5472 2024-04-21 01:43:39.000000 scriptime-1.0.0/scriptime.egg-info/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      262 2024-04-21 01:43:39.000000 scriptime-1.0.0/scriptime.egg-info/SOURCES.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2024-04-21 01:43:39.000000 scriptime-1.0.0/scriptime.egg-info/dependency_links.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       30 2024-04-21 01:43:39.000000 scriptime-1.0.0/scriptime.egg-info/requires.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2024-04-21 01:43:39.000000 scriptime-1.0.0/scriptime.egg-info/top_level.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2024-04-21 01:43:39.558759 scriptime-1.0.0/setup.cfg
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      694 2024-04-21 01:42:06.000000 scriptime-1.0.0/setup.py
```

### Comparing `scriptime-0.1.6/LICENSE` & `scriptime-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scriptime-0.1.6/PKG-INFO` & `scriptime-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: scriptime
-Version: 0.1.6
+Version: 1.0.0
 Summary: A Python library to notify when a script has finished running and providing insights such as run time, CPU and RAM usage, and more.
 Author: Jake Strasler
 Author-email: jstr36@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: psutil
+Requires-Dist: simpleaudio
+Requires-Dist: setuptools
 
 # scriptime
 Python library to notify when a script has finished running and providing insights such as run time, CPU and RAM usage, and more.
 
 
 - [scriptime](#scriptime)
   - [About](#about)
   - [Getting Started](#getting-started)
-  - [Using scriptimer](#using-scriptimer)
+  - [Using scriptime](#using-scriptime)
   - [Output](#output)
   - [Links](#links)
 
 ## About
 
 This project will send you an email or text message notifying you when a script has completed running. Configurable thorugh a config file, environment variables, or hardcoding the email credentials, this project has little overhead to get started.
 
@@ -59,17 +62,17 @@
         ```python
         timer = Timer(method="hardcode", email="example@email.com", password="superSecure1", server="smtp.email.com", port=123)
         ```
 
         > Note that if you are using Gmail, you may have to create an [app password](https://support.google.com/accounts/answer/185833?hl=en). Your normal password will likely not work. Other email services may have similar catches.
 
 
-## Using scriptimer
+## Using scriptime
 
-The use of scriptimer is very straightforward:
+The use of scriptime is very straightforward:
 
 1. In a terminal, `pip install scriptime`
 2. In a Python (.py) or Jupyter Notebook (.ipynb) file, add
     ```python
     from scriptime import Timer
     ``` 
     to your imports.
```

### Comparing `scriptime-0.1.6/README.md` & `scriptime-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # scriptime
 Python library to notify when a script has finished running and providing insights such as run time, CPU and RAM usage, and more.
 
 
 - [scriptime](#scriptime)
   - [About](#about)
   - [Getting Started](#getting-started)
-  - [Using scriptimer](#using-scriptimer)
+  - [Using scriptime](#using-scriptime)
   - [Output](#output)
   - [Links](#links)
 
 ## About
 
 This project will send you an email or text message notifying you when a script has completed running. Configurable thorugh a config file, environment variables, or hardcoding the email credentials, this project has little overhead to get started.
 
@@ -50,17 +50,17 @@
         ```python
         timer = Timer(method="hardcode", email="example@email.com", password="superSecure1", server="smtp.email.com", port=123)
         ```
 
         > Note that if you are using Gmail, you may have to create an [app password](https://support.google.com/accounts/answer/185833?hl=en). Your normal password will likely not work. Other email services may have similar catches.
 
 
-## Using scriptimer
+## Using scriptime
 
-The use of scriptimer is very straightforward:
+The use of scriptime is very straightforward:
 
 1. In a terminal, `pip install scriptime`
 2. In a Python (.py) or Jupyter Notebook (.ipynb) file, add
     ```python
     from scriptime import Timer
     ``` 
     to your imports.
```

### Comparing `scriptime-0.1.6/scriptime/alert.wav` & `scriptime-1.0.0/scriptime/alert.wav`

 * *Files identical despite different names*

### Comparing `scriptime-0.1.6/scriptime/main.py` & `scriptime-1.0.0/scriptime/main.py`

 * *Files identical despite different names*

### Comparing `scriptime-0.1.6/scriptime.egg-info/PKG-INFO` & `scriptime-1.0.0/scriptime.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: scriptime
-Version: 0.1.6
+Version: 1.0.0
 Summary: A Python library to notify when a script has finished running and providing insights such as run time, CPU and RAM usage, and more.
 Author: Jake Strasler
 Author-email: jstr36@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: psutil
+Requires-Dist: simpleaudio
+Requires-Dist: setuptools
 
 # scriptime
 Python library to notify when a script has finished running and providing insights such as run time, CPU and RAM usage, and more.
 
 
 - [scriptime](#scriptime)
   - [About](#about)
   - [Getting Started](#getting-started)
-  - [Using scriptimer](#using-scriptimer)
+  - [Using scriptime](#using-scriptime)
   - [Output](#output)
   - [Links](#links)
 
 ## About
 
 This project will send you an email or text message notifying you when a script has completed running. Configurable thorugh a config file, environment variables, or hardcoding the email credentials, this project has little overhead to get started.
 
@@ -59,17 +62,17 @@
         ```python
         timer = Timer(method="hardcode", email="example@email.com", password="superSecure1", server="smtp.email.com", port=123)
         ```
 
         > Note that if you are using Gmail, you may have to create an [app password](https://support.google.com/accounts/answer/185833?hl=en). Your normal password will likely not work. Other email services may have similar catches.
 
 
-## Using scriptimer
+## Using scriptime
 
-The use of scriptimer is very straightforward:
+The use of scriptime is very straightforward:
 
 1. In a terminal, `pip install scriptime`
 2. In a Python (.py) or Jupyter Notebook (.ipynb) file, add
     ```python
     from scriptime import Timer
     ``` 
     to your imports.
```

### Comparing `scriptime-0.1.6/setup.py` & `scriptime-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="scriptime",
-    version="0.1.6",
+    version="1.0.0",
     author="Jake Strasler",
     author_email="jstr36@gmail.com",
     description="A Python library to notify when a script has finished running and providing insights such as run time, CPU and RAM usage, and more.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["scriptime"],
     package_data={"scriptime": ["scriptime/alert.wav"]},
```


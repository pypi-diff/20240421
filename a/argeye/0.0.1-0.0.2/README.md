# Comparing `tmp/argeye-0.0.1.tar.gz` & `tmp/argeye-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argeye-0.0.1.tar", last modified: Fri Apr 19 04:33:11 2024, max compression
+gzip compressed data, was "argeye-0.0.2.tar", last modified: Sun Apr 21 12:10:40 2024, max compression
```

## Comparing `argeye-0.0.1.tar` & `argeye-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 04:33:11.233105 argeye-0.0.1/
--rw-rw-rw-   0        0        0     1094 2024-04-18 15:04:12.000000 argeye-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2640 2024-04-19 04:33:11.233105 argeye-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2070 2024-04-19 04:30:24.000000 argeye-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 04:33:11.232099 argeye-0.0.1/argeye.egg-info/
--rw-rw-rw-   0        0        0     2640 2024-04-19 04:33:11.000000 argeye-0.0.1/argeye.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-04-19 04:33:11.000000 argeye-0.0.1/argeye.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 04:33:11.000000 argeye-0.0.1/argeye.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 04:33:11.000000 argeye-0.0.1/argeye.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 04:33:11.234110 argeye-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      809 2024-04-18 14:48:16.000000 argeye-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 12:10:40.519943 argeye-0.0.2/
+-rw-rw-rw-   0        0        0     1094 2024-04-18 15:04:12.000000 argeye-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2700 2024-04-21 12:10:40.517005 argeye-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2130 2024-04-19 05:41:40.000000 argeye-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 12:10:40.474909 argeye-0.0.2/argeye/
+-rw-rw-rw-   0        0        0        0 2024-04-21 12:08:30.000000 argeye-0.0.2/argeye/__init__.py
+-rw-rw-rw-   0        0        0   104296 2024-04-18 13:00:16.000000 argeye-0.0.2/argeye/argeye.py
+drwxrwxrwx   0        0        0        0 2024-04-21 12:10:40.514359 argeye-0.0.2/argeye.egg-info/
+-rw-rw-rw-   0        0        0     2700 2024-04-21 12:10:40.000000 argeye-0.0.2/argeye.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-04-21 12:10:40.000000 argeye-0.0.2/argeye.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 12:10:40.000000 argeye-0.0.2/argeye.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-21 12:10:40.000000 argeye-0.0.2/argeye.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 12:10:40.520944 argeye-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      809 2024-04-21 12:10:22.000000 argeye-0.0.2/setup.py
```

### Comparing `argeye-0.0.1/LICENSE.txt` & `argeye-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `argeye-0.0.1/PKG-INFO` & `argeye-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argeye
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small optimization of Python library argparse.All original usage are retained,but adding a yml file so the user can set the arguments by editing the yml file.
 Home-page: https://github.com/llzmgjzhy/argeye.git
 Author: llzmgjzhy
 Author-email: bmnjklipo@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,16 @@
 
 > argparse supports command lines to set arguments,whose disadvantages is that the user have to type the arg strings and values.
 >
 > the typing is a redundant operation,which may cause mistakes and counterintuitive understanding of the args.
 >
 > yml file provides intuitive understanding and a more convenient way to set args.
 
+_**only one line change,better experience of argparse**_
+
 ## usage
 
 ### (original)
 
 retained all the original usage of argparse,detailed info refer to [official document](https://docs.python.org/3/library/argparse.html)
 
 ### (new)
```

### Comparing `argeye-0.0.1/README.md` & `argeye-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 > argparse supports command lines to set arguments,whose disadvantages is that the user have to type the arg strings and values.
 >
 > the typing is a redundant operation,which may cause mistakes and counterintuitive understanding of the args.
 >
 > yml file provides intuitive understanding and a more convenient way to set args.
 
+_**only one line change,better experience of argparse**_
+
 ## usage
 
 ### (original)
 
 retained all the original usage of argparse,detailed info refer to [official document](https://docs.python.org/3/library/argparse.html)
 
 ### (new)
```

### Comparing `argeye-0.0.1/argeye.egg-info/PKG-INFO` & `argeye-0.0.2/argeye.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argeye
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small optimization of Python library argparse.All original usage are retained,but adding a yml file so the user can set the arguments by editing the yml file.
 Home-page: https://github.com/llzmgjzhy/argeye.git
 Author: llzmgjzhy
 Author-email: bmnjklipo@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,16 @@
 
 > argparse supports command lines to set arguments,whose disadvantages is that the user have to type the arg strings and values.
 >
 > the typing is a redundant operation,which may cause mistakes and counterintuitive understanding of the args.
 >
 > yml file provides intuitive understanding and a more convenient way to set args.
 
+_**only one line change,better experience of argparse**_
+
 ## usage
 
 ### (original)
 
 retained all the original usage of argparse,detailed info refer to [official document](https://docs.python.org/3/library/argparse.html)
 
 ### (new)
```

### Comparing `argeye-0.0.1/setup.py` & `argeye-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="argeye",
-    version="0.0.1",
+    version="0.0.2",
     author="llzmgjzhy", 
     author_email="bmnjklipo@qq.com",
     description="A small optimization of Python library argparse.All original usage are retained,but adding a yml file so the user can set the arguments by editing the yml file.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/llzmgjzhy/argeye.git",
     packages=setuptools.find_packages(),
```


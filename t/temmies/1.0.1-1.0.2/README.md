# Comparing `tmp/temmies-1.0.1.tar.gz` & `tmp/temmies-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temmies-1.0.1.tar", last modified: Sat Apr 20 23:54:22 2024, max compression
+gzip compressed data, was "temmies-1.0.2.tar", last modified: Sun Apr 21 18:31:54 2024, max compression
```

## Comparing `temmies-1.0.1.tar` & `temmies-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,23 @@
-drwxr-xr-x   0 alent     (1000) alent     (1000)        0 2024-04-20 23:54:22.479658 temmies-1.0.1/
--rw-r--r--   0 alent     (1000) alent     (1000)    35149 2024-02-12 11:56:30.000000 temmies-1.0.1/LICENSE
--rw-r--r--   0 alent     (1000) alent     (1000)     1355 2024-04-20 23:54:22.479658 temmies-1.0.1/PKG-INFO
--rw-r--r--   0 alent     (1000) alent     (1000)      798 2024-04-20 22:58:31.000000 temmies-1.0.1/README.md
--rw-r--r--   0 alent     (1000) alent     (1000)       38 2024-04-20 23:54:22.479658 temmies-1.0.1/setup.cfg
--rw-r--r--   0 alent     (1000) alent     (1000)      848 2024-04-20 23:53:58.000000 temmies-1.0.1/setup.py
-drwxr-xr-x   0 alent     (1000) alent     (1000)        0 2024-04-20 23:54:22.479658 temmies-1.0.1/temmies/
-drwxr-xr-x   0 alent     (1000) alent     (1000)        0 2024-04-20 23:54:22.479658 temmies-1.0.1/temmies/temmies.egg-info/
--rw-r--r--   0 alent     (1000) alent     (1000)     1355 2024-04-20 23:54:22.000000 temmies-1.0.1/temmies/temmies.egg-info/PKG-INFO
--rw-r--r--   0 alent     (1000) alent     (1000)      220 2024-04-20 23:54:22.000000 temmies-1.0.1/temmies/temmies.egg-info/SOURCES.txt
--rw-r--r--   0 alent     (1000) alent     (1000)        1 2024-04-20 23:54:22.000000 temmies-1.0.1/temmies/temmies.egg-info/dependency_links.txt
--rw-r--r--   0 alent     (1000) alent     (1000)       13 2024-04-20 23:54:22.000000 temmies-1.0.1/temmies/temmies.egg-info/requires.txt
--rw-r--r--   0 alent     (1000) alent     (1000)        1 2024-04-20 23:54:22.000000 temmies-1.0.1/temmies/temmies.egg-info/top_level.txt
+drwxr-xr-x   0 alent     (1000) alent     (1000)        0 2024-04-21 18:31:54.335814 temmies-1.0.2/
+-rw-r--r--   0 alent     (1000) alent     (1000)    35149 2024-02-12 11:56:30.000000 temmies-1.0.2/LICENSE
+-rw-r--r--   0 alent     (1000) alent     (1000)     1366 2024-04-21 18:31:54.335814 temmies-1.0.2/PKG-INFO
+-rw-r--r--   0 alent     (1000) alent     (1000)      798 2024-04-20 22:58:31.000000 temmies-1.0.2/README.md
+-rw-r--r--   0 alent     (1000) alent     (1000)       38 2024-04-21 18:31:54.335814 temmies-1.0.2/setup.cfg
+-rw-r--r--   0 alent     (1000) alent     (1000)      809 2024-04-21 18:31:47.000000 temmies-1.0.2/setup.py
+drwxr-xr-x   0 alent     (1000) alent     (1000)        0 2024-04-21 18:31:54.332480 temmies-1.0.2/temmies/
+-rw-r--r--   0 alent     (1000) alent     (1000)       26 2024-04-21 18:31:01.000000 temmies-1.0.2/temmies/__init__.py
+-rw-r--r--   0 alent     (1000) alent     (1000)     2375 2024-04-21 17:57:47.000000 temmies-1.0.2/temmies/course.py
+drwxr-xr-x   0 alent     (1000) alent     (1000)        0 2024-04-21 18:31:54.335814 temmies-1.0.2/temmies/exceptions/
+-rw-r--r--   0 alent     (1000) alent     (1000)        0 2024-04-21 17:41:45.000000 temmies-1.0.2/temmies/exceptions/__init__.py
+-rw-r--r--   0 alent     (1000) alent     (1000)      239 2024-04-10 16:01:35.000000 temmies-1.0.2/temmies/exceptions/course_unavailable.py
+-rw-r--r--   0 alent     (1000) alent     (1000)      200 2024-04-10 16:01:17.000000 temmies-1.0.2/temmies/exceptions/illegal_action.py
+-rw-r--r--   0 alent     (1000) alent     (1000)    13096 2024-04-20 23:49:51.000000 temmies-1.0.2/temmies/exercise_group.py
+-rw-r--r--   0 alent     (1000) alent     (1000)     3457 2024-04-20 23:49:54.000000 temmies-1.0.2/temmies/submission.py
+-rw-r--r--   0 alent     (1000) alent     (1000)     2756 2024-04-20 23:49:32.000000 temmies-1.0.2/temmies/themis.py
+-rw-r--r--   0 alent     (1000) alent     (1000)     2220 2024-04-20 23:50:00.000000 temmies-1.0.2/temmies/year.py
+drwxr-xr-x   0 alent     (1000) alent     (1000)        0 2024-04-21 18:31:54.335814 temmies-1.0.2/temmies.egg-info/
+-rw-r--r--   0 alent     (1000) alent     (1000)     1366 2024-04-21 18:31:54.000000 temmies-1.0.2/temmies.egg-info/PKG-INFO
+-rw-r--r--   0 alent     (1000) alent     (1000)      409 2024-04-21 18:31:54.000000 temmies-1.0.2/temmies.egg-info/SOURCES.txt
+-rw-r--r--   0 alent     (1000) alent     (1000)        1 2024-04-21 18:31:54.000000 temmies-1.0.2/temmies.egg-info/dependency_links.txt
+-rw-r--r--   0 alent     (1000) alent     (1000)       24 2024-04-21 18:31:54.000000 temmies-1.0.2/temmies.egg-info/requires.txt
+-rw-r--r--   0 alent     (1000) alent     (1000)        8 2024-04-21 18:31:54.000000 temmies-1.0.2/temmies.egg-info/top_level.txt
```

### Comparing `temmies-1.0.1/LICENSE` & `temmies-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `temmies-1.0.1/PKG-INFO` & `temmies-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: temmies
-Version: 1.0.1
+Version: 1.0.2
 Summary: A wrapper for the Themis website
 Home-page: https://github.com/Code-For-Groningen/temmies
 Author: Boyan K.
 Author-email: boyan@confest.im
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
-Requires-Dist: bs4
+Requires-Dist: beautifulsoup4
 
 <p align="center">
   <img src="docs/img/rugemmie.gif" />  
 </p>
 <p align="center">
 <a href="https://temmies.readthedocs.io/en/latest/"><img alt="Read the Docs" src="https://img.shields.io/readthedocs/temmies"></a>
 <img alt="GitHub" src="https://img.shields.io/github/license/Code-For-Groningen/temmies">
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: temmies Version: 1.0.1 Summary: A wrapper for the
+Metadata-Version: 2.1 Name: temmies Version: 1.0.2 Summary: A wrapper for the
 Themis website Home-page: https://github.com/Code-For-Groningen/temmies Author:
 Boyan K. Author-email: boyan@confest.im License: GPLv3 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Programming Language :: Python :: 3.9 Requires-Python: >=3.9 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: requests
-Requires-Dist: bs4
+Requires-Dist: beautifulsoup4
                             [docs/img/rugemmie.gif]
                             _[_R_e_a_d_ _t_h_e_ _D_o_c_s_][GitHub]
 A python library which interacts with themis. Uses bs4. I'll try to end
 development on a somewhat working state. ## Intended Features * [x] Log in *
 [x] Submit * [x] Bulk download of test cases and files * [x] Submission status
 ## Docs [here](http://temmies.rtfd.io/). ## Possible continuations * Discord
 bot * CLI program ## Thanks to * [Glitchcat](https://glitchcat.github.io/
```

### Comparing `temmies-1.0.1/README.md` & `temmies-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `temmies-1.0.1/setup.py` & `temmies-1.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     l_description = f.read()
     
 setup(
     name="temmies",
-    version="1.0.1",
-    package_dir = {"": "temmies"},
-    packages=find_packages(where="temmies"),
+    version="1.0.2",
+    packages=find_packages(),
     description="A wrapper for the Themis website",
     long_description=l_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Code-For-Groningen/temmies",
     author="Boyan K.",
     author_email="boyan@confest.im",
     license="GPLv3",
@@ -19,11 +18,11 @@
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3.9",
     ],
     install_requires=[
         "requests",
-        "bs4",
+        "beautifulsoup4",
     ],
     python_requires=">=3.9",
 )
```

### Comparing `temmies-1.0.1/temmies/temmies.egg-info/PKG-INFO` & `temmies-1.0.2/temmies.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: temmies
-Version: 1.0.1
+Version: 1.0.2
 Summary: A wrapper for the Themis website
 Home-page: https://github.com/Code-For-Groningen/temmies
 Author: Boyan K.
 Author-email: boyan@confest.im
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
-Requires-Dist: bs4
+Requires-Dist: beautifulsoup4
 
 <p align="center">
   <img src="docs/img/rugemmie.gif" />  
 </p>
 <p align="center">
 <a href="https://temmies.readthedocs.io/en/latest/"><img alt="Read the Docs" src="https://img.shields.io/readthedocs/temmies"></a>
 <img alt="GitHub" src="https://img.shields.io/github/license/Code-For-Groningen/temmies">
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: temmies Version: 1.0.1 Summary: A wrapper for the
+Metadata-Version: 2.1 Name: temmies Version: 1.0.2 Summary: A wrapper for the
 Themis website Home-page: https://github.com/Code-For-Groningen/temmies Author:
 Boyan K. Author-email: boyan@confest.im License: GPLv3 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Programming Language :: Python :: 3.9 Requires-Python: >=3.9 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: requests
-Requires-Dist: bs4
+Requires-Dist: beautifulsoup4
                             [docs/img/rugemmie.gif]
                             _[_R_e_a_d_ _t_h_e_ _D_o_c_s_][GitHub]
 A python library which interacts with themis. Uses bs4. I'll try to end
 development on a somewhat working state. ## Intended Features * [x] Log in *
 [x] Submit * [x] Bulk download of test cases and files * [x] Submission status
 ## Docs [here](http://temmies.rtfd.io/). ## Possible continuations * Discord
 bot * CLI program ## Thanks to * [Glitchcat](https://glitchcat.github.io/
```


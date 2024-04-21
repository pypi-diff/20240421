# Comparing `tmp/temmies-1.0.0.tar.gz` & `tmp/temmies-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temmies-1.0.0.tar", last modified: Sat Apr 20 23:09:00 2024, max compression
+gzip compressed data, was "temmies-1.0.1.tar", last modified: Sat Apr 20 23:54:22 2024, max compression
```

## Comparing `temmies-1.0.0.tar` & `temmies-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,13 @@
-drwxr-xr-x   0 alent     (1000) alent     (1000)        0 2024-04-20 23:09:00.871195 temmies-1.0.0/
--rw-r--r--   0 alent     (1000) alent     (1000)    35149 2024-02-12 11:56:30.000000 temmies-1.0.0/LICENSE
--rw-r--r--   0 alent     (1000) alent     (1000)     1327 2024-04-20 23:09:00.867861 temmies-1.0.0/PKG-INFO
--rw-r--r--   0 alent     (1000) alent     (1000)      798 2024-04-20 22:58:31.000000 temmies-1.0.0/README.md
--rw-r--r--   0 alent     (1000) alent     (1000)      509 2024-04-20 23:08:53.000000 temmies-1.0.0/pyproject.toml
--rw-r--r--   0 alent     (1000) alent     (1000)       38 2024-04-20 23:09:00.871195 temmies-1.0.0/setup.cfg
-drwxr-xr-x   0 alent     (1000) alent     (1000)        0 2024-04-20 23:09:00.867861 temmies-1.0.0/temmies/
--rw-r--r--   0 alent     (1000) alent     (1000)        0 2024-04-20 22:56:08.000000 temmies-1.0.0/temmies/__init__.py
--rw-r--r--   0 alent     (1000) alent     (1000)     2371 2024-04-10 16:12:21.000000 temmies-1.0.0/temmies/course.py
-drwxr-xr-x   0 alent     (1000) alent     (1000)        0 2024-04-20 23:09:00.867861 temmies-1.0.0/temmies/exceptions/
--rw-r--r--   0 alent     (1000) alent     (1000)      239 2024-04-10 16:01:35.000000 temmies-1.0.0/temmies/exceptions/course_unavailable.py
--rw-r--r--   0 alent     (1000) alent     (1000)      200 2024-04-10 16:01:17.000000 temmies-1.0.0/temmies/exceptions/illegal_action.py
--rw-r--r--   0 alent     (1000) alent     (1000)    13094 2024-04-20 19:22:55.000000 temmies-1.0.0/temmies/exercise_group.py
--rw-r--r--   0 alent     (1000) alent     (1000)     3458 2024-04-20 18:31:45.000000 temmies-1.0.0/temmies/submission.py
--rw-r--r--   0 alent     (1000) alent     (1000)     1122 2024-04-20 22:28:06.000000 temmies-1.0.0/temmies/test.py
--rw-r--r--   0 alent     (1000) alent     (1000)     2754 2024-04-10 16:27:16.000000 temmies-1.0.0/temmies/themis.py
--rw-r--r--   0 alent     (1000) alent     (1000)     2218 2024-04-10 16:30:25.000000 temmies-1.0.0/temmies/year.py
-drwxr-xr-x   0 alent     (1000) alent     (1000)        0 2024-04-20 23:09:00.867861 temmies-1.0.0/temmies.egg-info/
--rw-r--r--   0 alent     (1000) alent     (1000)     1327 2024-04-20 23:09:00.000000 temmies-1.0.0/temmies.egg-info/PKG-INFO
--rw-r--r--   0 alent     (1000) alent     (1000)      400 2024-04-20 23:09:00.000000 temmies-1.0.0/temmies.egg-info/SOURCES.txt
--rw-r--r--   0 alent     (1000) alent     (1000)        1 2024-04-20 23:09:00.000000 temmies-1.0.0/temmies.egg-info/dependency_links.txt
--rw-r--r--   0 alent     (1000) alent     (1000)       21 2024-04-20 23:09:00.000000 temmies-1.0.0/temmies.egg-info/requires.txt
--rw-r--r--   0 alent     (1000) alent     (1000)        8 2024-04-20 23:09:00.000000 temmies-1.0.0/temmies.egg-info/top_level.txt
+drwxr-xr-x   0 alent     (1000) alent     (1000)        0 2024-04-20 23:54:22.479658 temmies-1.0.1/
+-rw-r--r--   0 alent     (1000) alent     (1000)    35149 2024-02-12 11:56:30.000000 temmies-1.0.1/LICENSE
+-rw-r--r--   0 alent     (1000) alent     (1000)     1355 2024-04-20 23:54:22.479658 temmies-1.0.1/PKG-INFO
+-rw-r--r--   0 alent     (1000) alent     (1000)      798 2024-04-20 22:58:31.000000 temmies-1.0.1/README.md
+-rw-r--r--   0 alent     (1000) alent     (1000)       38 2024-04-20 23:54:22.479658 temmies-1.0.1/setup.cfg
+-rw-r--r--   0 alent     (1000) alent     (1000)      848 2024-04-20 23:53:58.000000 temmies-1.0.1/setup.py
+drwxr-xr-x   0 alent     (1000) alent     (1000)        0 2024-04-20 23:54:22.479658 temmies-1.0.1/temmies/
+drwxr-xr-x   0 alent     (1000) alent     (1000)        0 2024-04-20 23:54:22.479658 temmies-1.0.1/temmies/temmies.egg-info/
+-rw-r--r--   0 alent     (1000) alent     (1000)     1355 2024-04-20 23:54:22.000000 temmies-1.0.1/temmies/temmies.egg-info/PKG-INFO
+-rw-r--r--   0 alent     (1000) alent     (1000)      220 2024-04-20 23:54:22.000000 temmies-1.0.1/temmies/temmies.egg-info/SOURCES.txt
+-rw-r--r--   0 alent     (1000) alent     (1000)        1 2024-04-20 23:54:22.000000 temmies-1.0.1/temmies/temmies.egg-info/dependency_links.txt
+-rw-r--r--   0 alent     (1000) alent     (1000)       13 2024-04-20 23:54:22.000000 temmies-1.0.1/temmies/temmies.egg-info/requires.txt
+-rw-r--r--   0 alent     (1000) alent     (1000)        1 2024-04-20 23:54:22.000000 temmies-1.0.1/temmies/temmies.egg-info/top_level.txt
```

### Comparing `temmies-1.0.0/LICENSE` & `temmies-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `temmies-1.0.0/PKG-INFO` & `temmies-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: temmies
-Version: 1.0.0
-Summary: Themis Python library. Aims to automate the retrieval and submission of data from and to the platform.
-Author-email: Boyan K <boyan@confest.im>
-Classifier: Programming Language :: Python :: 3
+Version: 1.0.1
+Summary: A wrapper for the Themis website
+Home-page: https://github.com/Code-For-Groningen/temmies
+Author: Boyan K.
+Author-email: boyan@confest.im
+License: GPLv3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: bs4
-Requires-Dist: urllib3
 
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
-Metadata-Version: 2.1 Name: temmies Version: 1.0.0 Summary: Themis Python
-library. Aims to automate the retrieval and submission of data from and to the
-platform. Author-email: Boyan K
-confest.im> Classifier: Programming Language :: Python :: 3 Classifier: License
-:: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
-System :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: requests Requires-Dist: bs4
-Requires-Dist: urllib3
+Metadata-Version: 2.1 Name: temmies Version: 1.0.1 Summary: A wrapper for the
+Themis website Home-page: https://github.com/Code-For-Groningen/temmies Author:
+Boyan K. Author-email: boyan@confest.im License: GPLv3 Classifier: Development
+Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
+License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
+Programming Language :: Python :: 3.9 Requires-Python: >=3.9 Description-
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: requests
+Requires-Dist: bs4
                             [docs/img/rugemmie.gif]
                             _[_R_e_a_d_ _t_h_e_ _D_o_c_s_][GitHub]
 A python library which interacts with themis. Uses bs4. I'll try to end
 development on a somewhat working state. ## Intended Features * [x] Log in *
 [x] Submit * [x] Bulk download of test cases and files * [x] Submission status
 ## Docs [here](http://temmies.rtfd.io/). ## Possible continuations * Discord
 bot * CLI program ## Thanks to * [Glitchcat](https://glitchcat.github.io/
```

### Comparing `temmies-1.0.0/README.md` & `temmies-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `temmies-1.0.0/temmies.egg-info/PKG-INFO` & `temmies-1.0.1/temmies/temmies.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: temmies
-Version: 1.0.0
-Summary: Themis Python library. Aims to automate the retrieval and submission of data from and to the platform.
-Author-email: Boyan K <boyan@confest.im>
-Classifier: Programming Language :: Python :: 3
+Version: 1.0.1
+Summary: A wrapper for the Themis website
+Home-page: https://github.com/Code-For-Groningen/temmies
+Author: Boyan K.
+Author-email: boyan@confest.im
+License: GPLv3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: bs4
-Requires-Dist: urllib3
 
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
-Metadata-Version: 2.1 Name: temmies Version: 1.0.0 Summary: Themis Python
-library. Aims to automate the retrieval and submission of data from and to the
-platform. Author-email: Boyan K
-confest.im> Classifier: Programming Language :: Python :: 3 Classifier: License
-:: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
-System :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: requests Requires-Dist: bs4
-Requires-Dist: urllib3
+Metadata-Version: 2.1 Name: temmies Version: 1.0.1 Summary: A wrapper for the
+Themis website Home-page: https://github.com/Code-For-Groningen/temmies Author:
+Boyan K. Author-email: boyan@confest.im License: GPLv3 Classifier: Development
+Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
+License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
+Programming Language :: Python :: 3.9 Requires-Python: >=3.9 Description-
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: requests
+Requires-Dist: bs4
                             [docs/img/rugemmie.gif]
                             _[_R_e_a_d_ _t_h_e_ _D_o_c_s_][GitHub]
 A python library which interacts with themis. Uses bs4. I'll try to end
 development on a somewhat working state. ## Intended Features * [x] Log in *
 [x] Submit * [x] Bulk download of test cases and files * [x] Submission status
 ## Docs [here](http://temmies.rtfd.io/). ## Possible continuations * Discord
 bot * CLI program ## Thanks to * [Glitchcat](https://glitchcat.github.io/
```


# Comparing `tmp/arithmetic-dice-roller-0.3.2.tar.gz` & `tmp/arithmetic_dice_roller-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arithmetic-dice-roller-0.3.2.tar", last modified: Sun Nov  5 11:40:12 2023, max compression
+gzip compressed data, was "arithmetic_dice_roller-0.3.3.tar", last modified: Sun Apr 21 18:29:27 2024, max compression
```

## Comparing `arithmetic-dice-roller-0.3.2.tar` & `arithmetic_dice_roller-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2023-11-05 11:40:12.741635 arithmetic-dice-roller-0.3.2/
--rw-r--r--   0 damax     (1000) damax     (1000)     4620 2023-11-05 11:40:12.741635 arithmetic-dice-roller-0.3.2/PKG-INFO
--rw-r--r--   0 damax     (1000) damax     (1000)     4054 2023-05-19 08:47:31.000000 arithmetic-dice-roller-0.3.2/README.md
-drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2023-11-05 11:40:12.740635 arithmetic-dice-roller-0.3.2/arithmetic_dice_roller/
--rw-r--r--   0 damax     (1000) damax     (1000)        0 2021-11-05 13:05:11.000000 arithmetic-dice-roller-0.3.2/arithmetic_dice_roller/__init__.py
--rw-r--r--   0 damax     (1000) damax     (1000)     1275 2023-11-05 11:35:41.000000 arithmetic-dice-roller-0.3.2/arithmetic_dice_roller/__main__.py
--rw-r--r--   0 damax     (1000) damax     (1000)    11102 2023-11-05 11:35:45.000000 arithmetic-dice-roller-0.3.2/arithmetic_dice_roller/roller.py
-drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2023-11-05 11:40:12.741635 arithmetic-dice-roller-0.3.2/arithmetic_dice_roller.egg-info/
--rw-r--r--   0 damax     (1000) damax     (1000)     4620 2023-11-05 11:40:12.000000 arithmetic-dice-roller-0.3.2/arithmetic_dice_roller.egg-info/PKG-INFO
--rw-r--r--   0 damax     (1000) damax     (1000)      399 2023-11-05 11:40:12.000000 arithmetic-dice-roller-0.3.2/arithmetic_dice_roller.egg-info/SOURCES.txt
--rw-r--r--   0 damax     (1000) damax     (1000)        1 2023-11-05 11:40:12.000000 arithmetic-dice-roller-0.3.2/arithmetic_dice_roller.egg-info/dependency_links.txt
--rw-r--r--   0 damax     (1000) damax     (1000)       80 2023-11-05 11:40:12.000000 arithmetic-dice-roller-0.3.2/arithmetic_dice_roller.egg-info/entry_points.txt
--rw-r--r--   0 damax     (1000) damax     (1000)       12 2023-11-05 11:40:12.000000 arithmetic-dice-roller-0.3.2/arithmetic_dice_roller.egg-info/requires.txt
--rw-r--r--   0 damax     (1000) damax     (1000)       23 2023-11-05 11:40:12.000000 arithmetic-dice-roller-0.3.2/arithmetic_dice_roller.egg-info/top_level.txt
--rw-r--r--   0 damax     (1000) damax     (1000)       38 2023-11-05 11:40:12.741635 arithmetic-dice-roller-0.3.2/setup.cfg
--rw-r--r--   0 damax     (1000) damax     (1000)     1031 2023-11-05 11:35:59.000000 arithmetic-dice-roller-0.3.2/setup.py
+drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2024-04-21 18:29:27.241851 arithmetic_dice_roller-0.3.3/
+-rw-r--r--   0 damax     (1000) damax     (1000)     4399 2024-04-21 18:29:27.241851 arithmetic_dice_roller-0.3.3/PKG-INFO
+-rw-r--r--   0 damax     (1000) damax     (1000)     3833 2024-04-21 13:25:01.000000 arithmetic_dice_roller-0.3.3/README.md
+drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2024-04-21 18:29:27.241851 arithmetic_dice_roller-0.3.3/arithmetic_dice_roller/
+-rw-r--r--   0 damax     (1000) damax     (1000)        0 2021-11-05 13:05:11.000000 arithmetic_dice_roller-0.3.3/arithmetic_dice_roller/__init__.py
+-rw-r--r--   0 damax     (1000) damax     (1000)     1275 2023-11-05 11:35:41.000000 arithmetic_dice_roller-0.3.3/arithmetic_dice_roller/__main__.py
+-rw-r--r--   0 damax     (1000) damax     (1000)    11102 2023-11-05 11:35:45.000000 arithmetic_dice_roller-0.3.3/arithmetic_dice_roller/roller.py
+drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2024-04-21 18:29:27.241851 arithmetic_dice_roller-0.3.3/arithmetic_dice_roller.egg-info/
+-rw-r--r--   0 damax     (1000) damax     (1000)     4399 2024-04-21 18:29:27.000000 arithmetic_dice_roller-0.3.3/arithmetic_dice_roller.egg-info/PKG-INFO
+-rw-r--r--   0 damax     (1000) damax     (1000)      399 2024-04-21 18:29:27.000000 arithmetic_dice_roller-0.3.3/arithmetic_dice_roller.egg-info/SOURCES.txt
+-rw-r--r--   0 damax     (1000) damax     (1000)        1 2024-04-21 18:29:27.000000 arithmetic_dice_roller-0.3.3/arithmetic_dice_roller.egg-info/dependency_links.txt
+-rw-r--r--   0 damax     (1000) damax     (1000)       80 2024-04-21 18:29:27.000000 arithmetic_dice_roller-0.3.3/arithmetic_dice_roller.egg-info/entry_points.txt
+-rw-r--r--   0 damax     (1000) damax     (1000)       12 2024-04-21 18:29:27.000000 arithmetic_dice_roller-0.3.3/arithmetic_dice_roller.egg-info/requires.txt
+-rw-r--r--   0 damax     (1000) damax     (1000)       23 2024-04-21 18:29:27.000000 arithmetic_dice_roller-0.3.3/arithmetic_dice_roller.egg-info/top_level.txt
+-rw-r--r--   0 damax     (1000) damax     (1000)       38 2024-04-21 18:29:27.241851 arithmetic_dice_roller-0.3.3/setup.cfg
+-rw-r--r--   0 damax     (1000) damax     (1000)     1031 2024-04-21 18:28:29.000000 arithmetic_dice_roller-0.3.3/setup.py
```

### Comparing `arithmetic-dice-roller-0.3.2/PKG-INFO` & `arithmetic_dice_roller-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arithmetic-dice-roller
-Version: 0.3.2
+Version: 0.3.3
 Summary: A handy dice roller with extended notation and arithmetic expressions management.
 Home-page: https://github.com/massimopavoni/arithmetic-dice-roller
 Author: Massimo Pavoni
 Author-email: maspavoni@gmail.com
 Platform: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -15,18 +15,14 @@
 
 # arithmetic-dice-roller
 [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/massimopavoni/arithmetic-dice-roller?include_prereleases)](https://github.com/massimopavoni/arithmetic-dice-roller/releases)
 [![PyPI Package](https://img.shields.io/pypi/v/arithmetic-dice-roller)](https://pypi.org/project/arithmetic-dice-roller/)
 [![GitHub License](https://img.shields.io/github/license/massimopavoni/arithmetic-dice-roller)](https://github.com/massimopavoni/arithmetic-dice-roller/blob/main/LICENSE)
 [![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/massimopavoni/arithmetic-dice-roller)](https://www.python.org/downloads/release/python-3110/)
 
-[![Discord](https://img.shields.io/discord/926217143194886234?label=Join%20Not%20Declared%20Developers)](https://discord.gg/ZA76nJ3RsU)
-
-[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/T6T8BD7A1)
-
 A handy dice roller with extended notation and arithmetic expressions' management.
 
 The package aims to provide an easy-to-use implementation of a dice roller application with multiple operators' options and automatic results calculation.
 
 ### Dependencies
 - [SymPy](https://www.sympy.org) ([LICENSE](https://github.com/sympy/sympy/blob/master/LICENSE))
```

### Comparing `arithmetic-dice-roller-0.3.2/README.md` & `arithmetic_dice_roller-0.3.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 # arithmetic-dice-roller
 [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/massimopavoni/arithmetic-dice-roller?include_prereleases)](https://github.com/massimopavoni/arithmetic-dice-roller/releases)
 [![PyPI Package](https://img.shields.io/pypi/v/arithmetic-dice-roller)](https://pypi.org/project/arithmetic-dice-roller/)
 [![GitHub License](https://img.shields.io/github/license/massimopavoni/arithmetic-dice-roller)](https://github.com/massimopavoni/arithmetic-dice-roller/blob/main/LICENSE)
 [![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/massimopavoni/arithmetic-dice-roller)](https://www.python.org/downloads/release/python-3110/)
 
-[![Discord](https://img.shields.io/discord/926217143194886234?label=Join%20Not%20Declared%20Developers)](https://discord.gg/ZA76nJ3RsU)
-
-[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/T6T8BD7A1)
-
 A handy dice roller with extended notation and arithmetic expressions' management.
 
 The package aims to provide an easy-to-use implementation of a dice roller application with multiple operators' options and automatic results calculation.
 
 ### Dependencies
 - [SymPy](https://www.sympy.org) ([LICENSE](https://github.com/sympy/sympy/blob/master/LICENSE))
```

### Comparing `arithmetic-dice-roller-0.3.2/arithmetic_dice_roller/__main__.py` & `arithmetic_dice_roller-0.3.3/arithmetic_dice_roller/__main__.py`

 * *Files identical despite different names*

### Comparing `arithmetic-dice-roller-0.3.2/arithmetic_dice_roller/roller.py` & `arithmetic_dice_roller-0.3.3/arithmetic_dice_roller/roller.py`

 * *Files identical despite different names*

### Comparing `arithmetic-dice-roller-0.3.2/arithmetic_dice_roller.egg-info/PKG-INFO` & `arithmetic_dice_roller-0.3.3/arithmetic_dice_roller.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arithmetic-dice-roller
-Version: 0.3.2
+Version: 0.3.3
 Summary: A handy dice roller with extended notation and arithmetic expressions management.
 Home-page: https://github.com/massimopavoni/arithmetic-dice-roller
 Author: Massimo Pavoni
 Author-email: maspavoni@gmail.com
 Platform: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -15,18 +15,14 @@
 
 # arithmetic-dice-roller
 [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/massimopavoni/arithmetic-dice-roller?include_prereleases)](https://github.com/massimopavoni/arithmetic-dice-roller/releases)
 [![PyPI Package](https://img.shields.io/pypi/v/arithmetic-dice-roller)](https://pypi.org/project/arithmetic-dice-roller/)
 [![GitHub License](https://img.shields.io/github/license/massimopavoni/arithmetic-dice-roller)](https://github.com/massimopavoni/arithmetic-dice-roller/blob/main/LICENSE)
 [![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/massimopavoni/arithmetic-dice-roller)](https://www.python.org/downloads/release/python-3110/)
 
-[![Discord](https://img.shields.io/discord/926217143194886234?label=Join%20Not%20Declared%20Developers)](https://discord.gg/ZA76nJ3RsU)
-
-[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/T6T8BD7A1)
-
 A handy dice roller with extended notation and arithmetic expressions' management.
 
 The package aims to provide an easy-to-use implementation of a dice roller application with multiple operators' options and automatic results calculation.
 
 ### Dependencies
 - [SymPy](https://www.sympy.org) ([LICENSE](https://github.com/sympy/sympy/blob/master/LICENSE))
```

### Comparing `arithmetic-dice-roller-0.3.2/setup.py` & `arithmetic_dice_roller-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 README = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name='arithmetic-dice-roller',
-    version='0.3.2',
+    version='0.3.3',
     description="A handy dice roller with extended notation and arithmetic expressions management.",
     long_description=README,
     long_description_content_type="text/markdown",
     author='Massimo Pavoni',
     author_email='maspavoni@gmail.com',
     url='https://github.com/massimopavoni/arithmetic-dice-roller',
     license_files='LICENSE',
```


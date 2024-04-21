# Comparing `tmp/types-pycurl-7.45.2.5.tar.gz` & `tmp/types-pycurl-7.45.3.20240421.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pycurl-7.45.2.5.tar", last modified: Sun Aug 13 21:11:19 2023, max compression
+gzip compressed data, was "types-pycurl-7.45.3.20240421.tar", last modified: Sun Apr 21 02:19:31 2024, max compression
```

## Comparing `types-pycurl-7.45.2.5.tar` & `types-pycurl-7.45.3.20240421.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 21:11:19.225383 types-pycurl-7.45.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-08-13 21:11:18.000000 types-pycurl-7.45.2.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-13 21:11:18.000000 types-pycurl-7.45.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-13 21:11:19.225383 types-pycurl-7.45.2.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 21:11:19.221383 types-pycurl-7.45.2.5/pycurl-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-13 21:11:18.000000 types-pycurl-7.45.2.5/pycurl-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    14953 2023-08-13 21:11:18.000000 types-pycurl-7.45.2.5/pycurl-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-13 21:11:19.225383 types-pycurl-7.45.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-13 21:11:18.000000 types-pycurl-7.45.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 21:11:19.225383 types-pycurl-7.45.2.5/types_pycurl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-13 21:11:19.000000 types-pycurl-7.45.2.5/types_pycurl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-13 21:11:19.000000 types-pycurl-7.45.2.5/types_pycurl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-13 21:11:19.000000 types-pycurl-7.45.2.5/types_pycurl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-13 21:11:19.000000 types-pycurl-7.45.2.5/types_pycurl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:19:31.173915 types-pycurl-7.45.3.20240421/
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-21 02:19:30.000000 types-pycurl-7.45.3.20240421/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-21 02:19:30.000000 types-pycurl-7.45.3.20240421/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-21 02:19:31.173915 types-pycurl-7.45.3.20240421/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:19:31.173915 types-pycurl-7.45.3.20240421/pycurl-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-21 02:19:30.000000 types-pycurl-7.45.3.20240421/pycurl-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    21019 2024-04-21 02:19:30.000000 types-pycurl-7.45.3.20240421/pycurl-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 02:19:30.000000 types-pycurl-7.45.3.20240421/pycurl-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 02:19:31.173915 types-pycurl-7.45.3.20240421/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-21 02:19:30.000000 types-pycurl-7.45.3.20240421/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:19:31.173915 types-pycurl-7.45.3.20240421/types_pycurl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-21 02:19:31.000000 types-pycurl-7.45.3.20240421/types_pycurl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-21 02:19:31.000000 types-pycurl-7.45.3.20240421/types_pycurl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 02:19:31.000000 types-pycurl-7.45.3.20240421/types_pycurl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 02:19:31.000000 types-pycurl-7.45.3.20240421/types_pycurl.egg-info/top_level.txt
```

### Comparing `types-pycurl-7.45.2.5/CHANGELOG.md` & `types-pycurl-7.45.3.20240421/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+## 7.45.3.20240421 (2024-04-21)
+
+Bump pycurl to 7.45.3, update platform tests (#11792)
+
+## 7.45.2.20240417 (2024-04-17)
+
+Remove remaining bare `Incomplete`s (#11768)
+
+Enable Y065
+
+## 7.45.2.20240311 (2024-03-11)
+
+Use PEP 570 syntax in third party stubs (#11554)
+
+## 7.45.2.20240106 (2024-01-06)
+
+Update typing_extensions imports in third-party stubs (#11245)
+
 ## 7.45.2.5 (2023-08-13)
 
 Fill in all missing `upstream_repository` fields (#10571)
 
 Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
 
 ## 7.45.2.4 (2023-03-29)
```

### Comparing `types-pycurl-7.45.2.5/setup.py` & `types-pycurl-7.45.3.20240421/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 from setuptools import setup
 
 name = "types-pycurl"
 description = "Typing stubs for pycurl"
 long_description = '''
 ## Typing stubs for pycurl
 
-This is a PEP 561 type stub package for the `pycurl` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`pycurl`](https://github.com/pycurl/pycurl) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`pycurl`. The source for this package can be found at
+`pycurl`.
+
+This version of `types-pycurl` aims to provide accurate annotations
+for `pycurl==7.45.3`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pycurl. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `22b055a147b5d672bf7e1f58cc6bf52cc526b35f` and was tested
-with mypy 1.4.1, pyright 1.1.320, and
-pytype 2023.7.21.
+This package was generated from typeshed commit `4872c30a98ac9ac649793e9bf3b2682f00cc55d8` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="7.45.2.5",
+      version="7.45.3.20240421",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pycurl.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['pycurl-stubs'],
-      package_data={'pycurl-stubs': ['__init__.pyi', 'METADATA.toml']},
+      package_data={'pycurl-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
+      python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```


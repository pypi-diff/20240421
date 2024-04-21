# Comparing `tmp/types-editdistance-0.6.3.5.tar.gz` & `tmp/types-editdistance-0.8.0.20240421.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-editdistance-0.6.3.5.tar", last modified: Thu Jul 20 18:19:23 2023, max compression
+gzip compressed data, was "types-editdistance-0.8.0.20240421.tar", last modified: Sun Apr 21 02:19:26 2024, max compression
```

## Comparing `types-editdistance-0.6.3.5.tar` & `types-editdistance-0.8.0.20240421.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:19:23.159245 types-editdistance-0.6.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-20 18:19:22.000000 types-editdistance-0.6.3.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 18:19:22.000000 types-editdistance-0.6.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-20 18:19:23.159245 types-editdistance-0.6.3.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:19:23.159245 types-editdistance-0.6.3.5/editdistance-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-20 18:19:22.000000 types-editdistance-0.6.3.5/editdistance-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-20 18:19:01.000000 types-editdistance-0.6.3.5/editdistance-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:19:23.159245 types-editdistance-0.6.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-20 18:19:22.000000 types-editdistance-0.6.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:19:23.159245 types-editdistance-0.6.3.5/types_editdistance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-20 18:19:23.000000 types-editdistance-0.6.3.5/types_editdistance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-20 18:19:23.000000 types-editdistance-0.6.3.5/types_editdistance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:19:23.000000 types-editdistance-0.6.3.5/types_editdistance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-20 18:19:23.000000 types-editdistance-0.6.3.5/types_editdistance.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:19:26.937852 types-editdistance-0.8.0.20240421/
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-21 02:19:25.000000 types-editdistance-0.8.0.20240421/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-21 02:19:25.000000 types-editdistance-0.8.0.20240421/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-21 02:19:26.937852 types-editdistance-0.8.0.20240421/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:19:26.937852 types-editdistance-0.8.0.20240421/editdistance-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-21 02:19:25.000000 types-editdistance-0.8.0.20240421/editdistance-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-21 02:19:14.000000 types-editdistance-0.8.0.20240421/editdistance-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 02:19:25.000000 types-editdistance-0.8.0.20240421/editdistance-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 02:19:26.937852 types-editdistance-0.8.0.20240421/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-21 02:19:25.000000 types-editdistance-0.8.0.20240421/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:19:26.937852 types-editdistance-0.8.0.20240421/types_editdistance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-21 02:19:26.000000 types-editdistance-0.8.0.20240421/types_editdistance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-21 02:19:26.000000 types-editdistance-0.8.0.20240421/types_editdistance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 02:19:26.000000 types-editdistance-0.8.0.20240421/types_editdistance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-21 02:19:26.000000 types-editdistance-0.8.0.20240421/types_editdistance.egg-info/top_level.txt
```

### Comparing `types-editdistance-0.6.3.5/CHANGELOG.md` & `types-editdistance-0.8.0.20240421/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.8.0.20240421 (2024-04-21)
+
+Bump editdistance to 0.8.* (#11795)
+
 ## 0.6.3.5 (2023-07-20)
 
 Add a few more upstream_repository URLs (#10489)
 
 ## 0.6.3.4 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-editdistance-0.6.3.5/PKG-INFO` & `types-editdistance-0.8.0.20240421/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: types-editdistance
-Version: 0.6.3.5
+Version: 0.8.0.20240421
 Summary: Typing stubs for editdistance
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/editdistance.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for editdistance
 
-This is a PEP 561 type stub package for the `editdistance` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`editdistance`](https://github.com/roy-ht/editdistance) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`editdistance`. The source for this package can be found at
+`editdistance`.
+
+This version of `types-editdistance` aims to provide accurate annotations
+for `editdistance==0.8.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/editdistance. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `754473a30d50b918ac6f1a824f41600806defa94` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `4872c30a98ac9ac649793e9bf3b2682f00cc55d8` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-editdistance-0.6.3.5/setup.py` & `types-editdistance-0.8.0.20240421/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 from setuptools import setup
 
 name = "types-editdistance"
 description = "Typing stubs for editdistance"
 long_description = '''
 ## Typing stubs for editdistance
 
-This is a PEP 561 type stub package for the `editdistance` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`editdistance`](https://github.com/roy-ht/editdistance) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`editdistance`. The source for this package can be found at
+`editdistance`.
+
+This version of `types-editdistance` aims to provide accurate annotations
+for `editdistance==0.8.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/editdistance. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `754473a30d50b918ac6f1a824f41600806defa94` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `4872c30a98ac9ac649793e9bf3b2682f00cc55d8` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="0.6.3.5",
+      version="0.8.0.20240421",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/editdistance.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['editdistance-stubs'],
-      package_data={'editdistance-stubs': ['__init__.pyi', 'METADATA.toml']},
+      package_data={'editdistance-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
+      python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-editdistance-0.6.3.5/types_editdistance.egg-info/PKG-INFO` & `types-editdistance-0.8.0.20240421/types_editdistance.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: types-editdistance
-Version: 0.6.3.5
+Version: 0.8.0.20240421
 Summary: Typing stubs for editdistance
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/editdistance.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for editdistance
 
-This is a PEP 561 type stub package for the `editdistance` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`editdistance`](https://github.com/roy-ht/editdistance) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`editdistance`. The source for this package can be found at
+`editdistance`.
+
+This version of `types-editdistance` aims to provide accurate annotations
+for `editdistance==0.8.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/editdistance. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `754473a30d50b918ac6f1a824f41600806defa94` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `4872c30a98ac9ac649793e9bf3b2682f00cc55d8` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```


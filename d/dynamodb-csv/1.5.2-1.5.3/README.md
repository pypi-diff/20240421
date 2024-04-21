# Comparing `tmp/dynamodb-csv-1.5.2.tar.gz` & `tmp/dynamodb_csv-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamodb-csv-1.5.2.tar", last modified: Tue Dec 26 00:36:40 2023, max compression
+gzip compressed data, was "dynamodb_csv-1.5.3.tar", last modified: Sun Apr 21 00:44:34 2024, max compression
```

## Comparing `dynamodb-csv-1.5.2.tar` & `dynamodb_csv-1.5.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 00:36:40.875766 dynamodb-csv-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-26 00:36:32.000000 dynamodb-csv-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16098 2023-12-26 00:36:40.875766 dynamodb-csv-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15228 2023-12-26 00:36:32.000000 dynamodb-csv-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 00:36:40.871766 dynamodb-csv-1.5.2/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-26 00:36:32.000000 dynamodb-csv-1.5.2/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 00:36:40.871766 dynamodb-csv-1.5.2/app/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-12-26 00:36:32.000000 dynamodb-csv-1.5.2/app/dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2023-12-26 00:36:32.000000 dynamodb-csv-1.5.2/app/dynamodb/csv_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2023-12-26 00:36:32.000000 dynamodb-csv-1.5.2/app/dynamodb/csv_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2023-12-26 00:36:32.000000 dynamodb-csv-1.5.2/app/dynamodb/move.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-12-26 00:36:32.000000 dynamodb-csv-1.5.2/app/dynamodb/truncate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2023-12-26 00:36:32.000000 dynamodb-csv-1.5.2/app/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 00:36:40.875766 dynamodb-csv-1.5.2/dynamodb_csv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16098 2023-12-26 00:36:40.000000 dynamodb-csv-1.5.2/dynamodb_csv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-26 00:36:40.000000 dynamodb-csv-1.5.2/dynamodb_csv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-26 00:36:40.000000 dynamodb-csv-1.5.2/dynamodb_csv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-26 00:36:40.000000 dynamodb-csv-1.5.2/dynamodb_csv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-26 00:36:40.000000 dynamodb-csv-1.5.2/dynamodb_csv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-26 00:36:40.000000 dynamodb-csv-1.5.2/dynamodb_csv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-26 00:36:40.000000 dynamodb-csv-1.5.2/dynamodb_csv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-12-26 00:36:40.875766 dynamodb-csv-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-26 00:36:32.000000 dynamodb-csv-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 00:36:40.875766 dynamodb-csv-1.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2023-12-26 00:36:32.000000 dynamodb-csv-1.5.2/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:44:34.298916 dynamodb_csv-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-21 00:44:21.000000 dynamodb_csv-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-04-21 00:44:34.298916 dynamodb_csv-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-04-21 00:44:21.000000 dynamodb_csv-1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:44:34.294916 dynamodb_csv-1.5.3/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:44:21.000000 dynamodb_csv-1.5.3/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:44:34.294916 dynamodb_csv-1.5.3/app/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-21 00:44:21.000000 dynamodb_csv-1.5.3/app/dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-21 00:44:21.000000 dynamodb_csv-1.5.3/app/dynamodb/csv_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-21 00:44:21.000000 dynamodb_csv-1.5.3/app/dynamodb/csv_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-21 00:44:21.000000 dynamodb_csv-1.5.3/app/dynamodb/move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-21 00:44:21.000000 dynamodb_csv-1.5.3/app/dynamodb/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-21 00:44:21.000000 dynamodb_csv-1.5.3/app/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:44:34.298916 dynamodb_csv-1.5.3/dynamodb_csv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-04-21 00:44:34.000000 dynamodb_csv-1.5.3/dynamodb_csv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-21 00:44:34.000000 dynamodb_csv-1.5.3/dynamodb_csv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 00:44:34.000000 dynamodb_csv-1.5.3/dynamodb_csv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 00:44:34.000000 dynamodb_csv-1.5.3/dynamodb_csv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 00:44:34.000000 dynamodb_csv-1.5.3/dynamodb_csv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-21 00:44:34.000000 dynamodb_csv-1.5.3/dynamodb_csv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-21 00:44:34.000000 dynamodb_csv-1.5.3/dynamodb_csv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-21 00:44:34.298916 dynamodb_csv-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 00:44:21.000000 dynamodb_csv-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:44:34.298916 dynamodb_csv-1.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-21 00:44:21.000000 dynamodb_csv-1.5.3/tests/test_main.py
```

### Comparing `dynamodb-csv-1.5.2/LICENSE` & `dynamodb_csv-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamodb-csv-1.5.2/PKG-INFO` & `dynamodb_csv-1.5.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamodb-csv
-Version: 1.5.2
+Version: 1.5.3
 Summary: A utility that allows CSV import / export to DynamoDB on the command line
 Home-page: https://github.com/danishi/dynamodb-csv
 Author: danishi
 Author-email: dns2developer@gmail.com
 License: MIT
 Keywords: AWS,DynamoDB,CSV
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,26 +21,33 @@
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: configparser
 Requires-Dist: tqdm
 
 # DynamoDB CSV utility
 
+[![Release Notes](https://img.shields.io/github/release/danishi/dynamodb-csv)](https://github.com/danishi/dynamodb-csv/releases)
+[![Contributors](https://img.shields.io/github/contributors/danishi/dynamodb-csv)](https://github.com/danishi/dynamodb-csv/contributors)
+[![Last Commit](https://img.shields.io/github/last-commit/danishi/dynamodb-csv)](https://github.com/danishi/dynamodb-csv/last-commit)
+[![Open Issues](https://img.shields.io/github/issues-raw/danishi/dynamodb-csv)](https://github.com/danishi/dynamodb-csv/issues)
+[![LRepo-size](https://img.shields.io/github/repo-size/danishi/dynamodb-csv)](https://github.com/danishi/dynamodb-csv/repo-size)
+[![Open in Dev Containers](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/danishi/dynamodb-csv)
+[![MIT](https://img.shields.io/github/license/danishi/DynamoDB-CSV)](https://github.com/danishi/dynamodb-csv/blob/master/LICENSE)
 [![ci](https://github.com/danishi/DynamoDB-CSV/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/danishi/DynamoDBImportCSV/actions/workflows/ci.yaml)
 [![codecov](https://codecov.io/gh/danishi/dynamodb-csv/branch/master/graph/badge.svg?token=KRA27MJN42)](https://codecov.io/gh/danishi/dynamodb-csv)
 [![Maintainability](https://api.codeclimate.com/v1/badges/c1d2a51bbd72d6198e0c/maintainability)](https://codeclimate.com/github/danishi/dynamodb-csv/maintainability)
-[![MIT](https://img.shields.io/github/license/danishi/DynamoDB-CSV)](https://github.com/danishi/dynamodb-csv/blob/master/LICENSE)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/dynamodb-csv.svg?color=%2334D058)
 [![PyPI](https://badge.fury.io/py/dynamodb-csv.svg)](https://badge.fury.io/py/dynamodb-csv)
 [![Downloads](https://static.pepy.tech/badge/dynamodb-csv)](https://pepy.tech/project/dynamodb-csv)
 [![Downloads week](https://static.pepy.tech/badge/dynamodb-csv/week)](https://pepy.tech/project/dynamodb-csv)
 [![Downloads month](https://static.pepy.tech/badge/dynamodb-csv/month)](https://pepy.tech/project/dynamodb-csv)
 [![Docker Pulls](https://img.shields.io/docker/pulls/danishi/dynamodb-csv)](https://hub.docker.com/r/danishi/dynamodb-csv)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
 
+[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/danishi/dynamodb-csv)
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/danishi)
 
 ![DynamoDBCSV](https://user-images.githubusercontent.com/56535085/159007555-e72d1c26-eb44-46ca-bc38-c752164995bf.png)
 
 A utility that allows CSV import / export to DynamoDB on the command line
 
 Give a ⭐️ if you like this tool!
```

### Comparing `dynamodb-csv-1.5.2/README.md` & `dynamodb_csv-1.5.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 # DynamoDB CSV utility
 
+[![Release Notes](https://img.shields.io/github/release/danishi/dynamodb-csv)](https://github.com/danishi/dynamodb-csv/releases)
+[![Contributors](https://img.shields.io/github/contributors/danishi/dynamodb-csv)](https://github.com/danishi/dynamodb-csv/contributors)
+[![Last Commit](https://img.shields.io/github/last-commit/danishi/dynamodb-csv)](https://github.com/danishi/dynamodb-csv/last-commit)
+[![Open Issues](https://img.shields.io/github/issues-raw/danishi/dynamodb-csv)](https://github.com/danishi/dynamodb-csv/issues)
+[![LRepo-size](https://img.shields.io/github/repo-size/danishi/dynamodb-csv)](https://github.com/danishi/dynamodb-csv/repo-size)
+[![Open in Dev Containers](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/danishi/dynamodb-csv)
+[![MIT](https://img.shields.io/github/license/danishi/DynamoDB-CSV)](https://github.com/danishi/dynamodb-csv/blob/master/LICENSE)
 [![ci](https://github.com/danishi/DynamoDB-CSV/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/danishi/DynamoDBImportCSV/actions/workflows/ci.yaml)
 [![codecov](https://codecov.io/gh/danishi/dynamodb-csv/branch/master/graph/badge.svg?token=KRA27MJN42)](https://codecov.io/gh/danishi/dynamodb-csv)
 [![Maintainability](https://api.codeclimate.com/v1/badges/c1d2a51bbd72d6198e0c/maintainability)](https://codeclimate.com/github/danishi/dynamodb-csv/maintainability)
-[![MIT](https://img.shields.io/github/license/danishi/DynamoDB-CSV)](https://github.com/danishi/dynamodb-csv/blob/master/LICENSE)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/dynamodb-csv.svg?color=%2334D058)
 [![PyPI](https://badge.fury.io/py/dynamodb-csv.svg)](https://badge.fury.io/py/dynamodb-csv)
 [![Downloads](https://static.pepy.tech/badge/dynamodb-csv)](https://pepy.tech/project/dynamodb-csv)
 [![Downloads week](https://static.pepy.tech/badge/dynamodb-csv/week)](https://pepy.tech/project/dynamodb-csv)
 [![Downloads month](https://static.pepy.tech/badge/dynamodb-csv/month)](https://pepy.tech/project/dynamodb-csv)
 [![Docker Pulls](https://img.shields.io/docker/pulls/danishi/dynamodb-csv)](https://hub.docker.com/r/danishi/dynamodb-csv)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
 
+[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/danishi/dynamodb-csv)
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/danishi)
 
 ![DynamoDBCSV](https://user-images.githubusercontent.com/56535085/159007555-e72d1c26-eb44-46ca-bc38-c752164995bf.png)
 
 A utility that allows CSV import / export to DynamoDB on the command line
 
 Give a ⭐️ if you like this tool!
```

### Comparing `dynamodb-csv-1.5.2/app/dynamodb/csv_export.py` & `dynamodb_csv-1.5.3/app/dynamodb/csv_export.py`

 * *Files identical despite different names*

### Comparing `dynamodb-csv-1.5.2/app/dynamodb/csv_import.py` & `dynamodb_csv-1.5.3/app/dynamodb/csv_import.py`

 * *Files identical despite different names*

### Comparing `dynamodb-csv-1.5.2/app/dynamodb/move.py` & `dynamodb_csv-1.5.3/app/dynamodb/move.py`

 * *Files identical despite different names*

### Comparing `dynamodb-csv-1.5.2/app/dynamodb/truncate.py` & `dynamodb_csv-1.5.3/app/dynamodb/truncate.py`

 * *Files identical despite different names*

### Comparing `dynamodb-csv-1.5.2/app/main.py` & `dynamodb_csv-1.5.3/app/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import configparser
 import argparse
 import sys
 from typing import Any, Tuple, List
 
 from app.dynamodb import csv_import, csv_export, truncate, move
 
-__version__ = "1.5.2"
+__version__ = "1.5.3"
 config_file = "config.ini"
 
 
 def main() -> None:
     """Main routine
     """
     (message, code) = execute()
```

### Comparing `dynamodb-csv-1.5.2/dynamodb_csv.egg-info/PKG-INFO` & `dynamodb_csv-1.5.3/dynamodb_csv.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamodb-csv
-Version: 1.5.2
+Version: 1.5.3
 Summary: A utility that allows CSV import / export to DynamoDB on the command line
 Home-page: https://github.com/danishi/dynamodb-csv
 Author: danishi
 Author-email: dns2developer@gmail.com
 License: MIT
 Keywords: AWS,DynamoDB,CSV
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,26 +21,33 @@
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: configparser
 Requires-Dist: tqdm
 
 # DynamoDB CSV utility
 
+[![Release Notes](https://img.shields.io/github/release/danishi/dynamodb-csv)](https://github.com/danishi/dynamodb-csv/releases)
+[![Contributors](https://img.shields.io/github/contributors/danishi/dynamodb-csv)](https://github.com/danishi/dynamodb-csv/contributors)
+[![Last Commit](https://img.shields.io/github/last-commit/danishi/dynamodb-csv)](https://github.com/danishi/dynamodb-csv/last-commit)
+[![Open Issues](https://img.shields.io/github/issues-raw/danishi/dynamodb-csv)](https://github.com/danishi/dynamodb-csv/issues)
+[![LRepo-size](https://img.shields.io/github/repo-size/danishi/dynamodb-csv)](https://github.com/danishi/dynamodb-csv/repo-size)
+[![Open in Dev Containers](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/danishi/dynamodb-csv)
+[![MIT](https://img.shields.io/github/license/danishi/DynamoDB-CSV)](https://github.com/danishi/dynamodb-csv/blob/master/LICENSE)
 [![ci](https://github.com/danishi/DynamoDB-CSV/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/danishi/DynamoDBImportCSV/actions/workflows/ci.yaml)
 [![codecov](https://codecov.io/gh/danishi/dynamodb-csv/branch/master/graph/badge.svg?token=KRA27MJN42)](https://codecov.io/gh/danishi/dynamodb-csv)
 [![Maintainability](https://api.codeclimate.com/v1/badges/c1d2a51bbd72d6198e0c/maintainability)](https://codeclimate.com/github/danishi/dynamodb-csv/maintainability)
-[![MIT](https://img.shields.io/github/license/danishi/DynamoDB-CSV)](https://github.com/danishi/dynamodb-csv/blob/master/LICENSE)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/dynamodb-csv.svg?color=%2334D058)
 [![PyPI](https://badge.fury.io/py/dynamodb-csv.svg)](https://badge.fury.io/py/dynamodb-csv)
 [![Downloads](https://static.pepy.tech/badge/dynamodb-csv)](https://pepy.tech/project/dynamodb-csv)
 [![Downloads week](https://static.pepy.tech/badge/dynamodb-csv/week)](https://pepy.tech/project/dynamodb-csv)
 [![Downloads month](https://static.pepy.tech/badge/dynamodb-csv/month)](https://pepy.tech/project/dynamodb-csv)
 [![Docker Pulls](https://img.shields.io/docker/pulls/danishi/dynamodb-csv)](https://hub.docker.com/r/danishi/dynamodb-csv)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
 
+[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/danishi/dynamodb-csv)
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/danishi)
 
 ![DynamoDBCSV](https://user-images.githubusercontent.com/56535085/159007555-e72d1c26-eb44-46ca-bc38-c752164995bf.png)
 
 A utility that allows CSV import / export to DynamoDB on the command line
 
 Give a ⭐️ if you like this tool!
```

### Comparing `dynamodb-csv-1.5.2/setup.cfg` & `dynamodb_csv-1.5.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dynamodb-csv
-version = 1.5.2
+version = 1.5.3
 description = A utility that allows CSV import / export to DynamoDB on the command line
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/danishi/dynamodb-csv
 keywords = AWS, DynamoDB, CSV
 license = MIT
 author = danishi
```

### Comparing `dynamodb-csv-1.5.2/tests/test_main.py` & `dynamodb_csv-1.5.3/tests/test_main.py`

 * *Files identical despite different names*


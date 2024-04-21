# Comparing `tmp/gramps-ql-0.2.0.tar.gz` & `tmp/gramps_ql-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gramps-ql-0.2.0.tar", last modified: Sun Apr  7 19:10:54 2024, max compression
+gzip compressed data, was "gramps_ql-0.2.1.tar", last modified: Sun Apr 21 06:20:36 2024, max compression
```

## Comparing `gramps-ql-0.2.0.tar` & `gramps_ql-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:10:54.854777 gramps-ql-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:10:54.850777 gramps-ql-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:10:54.850777 gramps-ql-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-04-07 19:10:54.854777 gramps-ql-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/mypy.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 19:10:54.854777 gramps-ql-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:10:54.850777 gramps-ql-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:10:54.854777 gramps-ql-0.2.0/src/gramps_ql/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/src/gramps_ql/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/src/gramps_ql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-07 19:10:54.000000 gramps-ql-0.2.0/src/gramps_ql/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/src/gramps_ql/gql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:10:54.854777 gramps-ql-0.2.0/src/gramps_ql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-04-07 19:10:54.000000 gramps-ql-0.2.0/src/gramps_ql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-07 19:10:54.000000 gramps-ql-0.2.0/src/gramps_ql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:10:54.000000 gramps-ql-0.2.0/src/gramps_ql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 19:10:54.000000 gramps-ql-0.2.0/src/gramps_ql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 19:10:54.000000 gramps-ql-0.2.0/src/gramps_ql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:10:54.850777 gramps-ql-0.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:10:54.854777 gramps-ql-0.2.0/tests/gramps_ql/
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/tests/gramps_ql/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/tests/gramps_ql/test_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/tests/gramps_ql/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:20:36.024545 gramps_ql-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:20:36.020545 gramps_ql-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:20:36.020545 gramps_ql-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11891 2024-04-21 06:20:36.024545 gramps_ql-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/mypy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 06:20:36.024545 gramps_ql-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:20:36.020545 gramps_ql-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:20:36.020545 gramps_ql-0.2.1/src/gramps_ql/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/src/gramps_ql/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/src/gramps_ql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 06:20:35.000000 gramps_ql-0.2.1/src/gramps_ql/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/src/gramps_ql/gql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:20:36.024545 gramps_ql-0.2.1/src/gramps_ql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11891 2024-04-21 06:20:36.000000 gramps_ql-0.2.1/src/gramps_ql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-21 06:20:36.000000 gramps_ql-0.2.1/src/gramps_ql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 06:20:36.000000 gramps_ql-0.2.1/src/gramps_ql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 06:20:36.000000 gramps_ql-0.2.1/src/gramps_ql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 06:20:36.000000 gramps_ql-0.2.1/src/gramps_ql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:20:36.020545 gramps_ql-0.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:20:36.024545 gramps_ql-0.2.1/tests/gramps_ql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/tests/gramps_ql/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/tests/gramps_ql/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/tests/gramps_ql/test_parse.py
```

### Comparing `gramps-ql-0.2.0/.github/workflows/python-publish.yml` & `gramps_ql-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `gramps-ql-0.2.0/.github/workflows/test.yml` & `gramps_ql-0.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `gramps-ql-0.2.0/LICENSE` & `gramps_ql-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gramps-ql-0.2.0/PKG-INFO` & `gramps_ql-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: gramps-ql
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library to filter Gramps objects by a query syntax
 Author-email: "David M. Straub" <straub@protonmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/DavidMStraub/gramps-ql
 Project-URL: repository, https://github.com/DavidMStraub/gramps-ql
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyparsing
+Requires-Dist: pyparsing>=3
 
 # GQL &ndash; the Gramps Query Language
 
 This Python library provides GQL, a query language to a [Gramps](https://github.com/gramps-project/gramps) database. The syntax is inspired by JQL, the Jira Query Language.
 
 ## Installation
```

### Comparing `gramps-ql-0.2.0/README.md` & `gramps_ql-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gramps-ql-0.2.0/pyproject.toml` & `gramps_ql-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "A Python library to filter Gramps objects by a query syntax"
 authors = [
   { name = "David M. Straub", email = "straub@protonmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
 dynamic = ["version"]
-dependencies = ["pyparsing"]
+dependencies = ["pyparsing>=3"]
 
 [project.urls]
 homepage = "https://github.com/DavidMStraub/gramps-ql"
 repository = "https://github.com/DavidMStraub/gramps-ql"
 
 [build-system]
 requires = ["setuptools>=61.0", "setuptools_scm[toml]>=6.2"]
```

### Comparing `gramps-ql-0.2.0/src/gramps_ql/gql.py` & `gramps_ql-0.2.1/src/gramps_ql/gql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """Gramps Query Language."""
 
 from __future__ import annotations  # can be removed at 3.8 EOL
 
 import json
 from collections.abc import Generator
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
 import pyparsing as pp
 from gramps.gen.db import DbReadBase
 from gramps.gen.lib import PrimaryObject
 from gramps.gen.lib.serialize import to_json
 
 pp.ParserElement.enablePackrat()
 
 
-def match(query: str, obj: dict[str, Any]) -> bool:
-    """Match a single object (given as dictionary) to a query."""
+def match(query: str, obj: Union[PrimaryObject, dict[str, Any]]) -> bool:
+    """Match a single object (optionally given as dictionary) to a query."""
     gq = GQLQuery(query=query)
+    if isinstance(obj, PrimaryObject):
+        obj_dict = json.loads(to_json(obj))
+        obj_dict["type"] = obj_dict["_class"].lower()
+        return gq.match(obj_dict)
     return gq.match(obj)
 
 
 def iter_objects(query: str, db: DbReadBase) -> Generator[PrimaryObject, None, None]:
     """Iterate over primary objects in a Gramps database."""
     gq = GQLQuery(query=query)
     return gq.iter_objects(db)
```

### Comparing `gramps-ql-0.2.0/src/gramps_ql.egg-info/PKG-INFO` & `gramps_ql-0.2.1/src/gramps_ql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: gramps-ql
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library to filter Gramps objects by a query syntax
 Author-email: "David M. Straub" <straub@protonmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/DavidMStraub/gramps-ql
 Project-URL: repository, https://github.com/DavidMStraub/gramps-ql
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyparsing
+Requires-Dist: pyparsing>=3
 
 # GQL &ndash; the Gramps Query Language
 
 This Python library provides GQL, a query language to a [Gramps](https://github.com/gramps-project/gramps) database. The syntax is inspired by JQL, the Jira Query Language.
 
 ## Installation
```

### Comparing `gramps-ql-0.2.0/tests/gramps_ql/test_iter.py` & `gramps_ql-0.2.1/tests/gramps_ql/test_iter.py`

 * *Files identical despite different names*

### Comparing `gramps-ql-0.2.0/tests/gramps_ql/test_match.py` & `gramps_ql-0.2.1/tests/gramps_ql/test_match.py`

 * *Files identical despite different names*

### Comparing `gramps-ql-0.2.0/tests/gramps_ql/test_parse.py` & `gramps_ql-0.2.1/tests/gramps_ql/test_parse.py`

 * *Files identical despite different names*


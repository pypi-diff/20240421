# Comparing `tmp/pg_alchemy_kit-0.9.12b0.tar.gz` & `tmp/pg_alchemy_kit-0.9.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_alchemy_kit-0.9.12b0.tar", max compression
+gzip compressed data, was "pg_alchemy_kit-0.9.1b0.tar", max compression
```

## Comparing `pg_alchemy_kit-0.9.12b0.tar` & `pg_alchemy_kit-0.9.1b0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     5222 2023-07-23 05:05:39.685000 pg_alchemy_kit-0.9.12b0/README.md
--rw-r--r--   0        0        0     3361 2024-03-15 17:20:52.235000 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/PG.py
--rw-r--r--   0        0        0    12877 2024-04-08 02:01:27.341432 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/PGUtils.py
--rw-r--r--   0        0        0     6323 2024-03-15 17:21:48.231000 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/PGUtilsBase.py
--rw-r--r--   0        0        0     5512 2024-03-15 17:22:12.728000 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/PGUtilsORM.py
--rw-r--r--   0        0        0      353 2023-12-02 13:44:05.554000 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/__init__.py
--rw-r--r--   0        0        0     2780 2024-04-21 00:55:09.212262 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/AsyncPG.py
--rw-r--r--   0        0        0     9416 2024-04-21 01:21:16.147394 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/AsyncPGUtilsORM.py
--rw-r--r--   0        0        0      402 2024-03-05 23:13:28.466000 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__init__.py
--rw-r--r--   0        0        0     2548 2024-04-20 23:32:34.684154 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-310.pyc
--rw-r--r--   0        0        0     4706 2024-04-21 00:55:25.414792 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-312.pyc
--rw-r--r--   0        0        0     8382 2024-03-21 22:25:25.802000 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsBase.cpython-310.pyc
--rw-r--r--   0        0        0    10742 2024-04-20 23:32:34.686799 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-310.pyc
--rw-r--r--   0        0        0    16328 2024-04-21 00:52:13.046852 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-312.pyc
--rw-r--r--   0        0        0     4980 2024-02-23 22:12:09.581000 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/PG.cpython-310.pyc
--rw-r--r--   0        0        0     8275 2024-02-23 22:14:07.165000 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsBase.cpython-310.pyc
--rw-r--r--   0        0        0     5417 2024-02-23 22:16:34.786000 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsORM.cpython-310.pyc
--rw-r--r--   0        0        0      460 2024-03-05 23:14:18.543000 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      481 2024-04-20 23:34:09.319347 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     5840 2023-11-01 14:19:01.447000 pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/cacheStrategies.py
--rw-r--r--   0        0        0      851 2024-04-21 01:21:28.051511 pg_alchemy_kit-0.9.12b0/pyproject.toml
--rw-r--r--   0        0        0     5927 1970-01-01 00:00:00.000000 pg_alchemy_kit-0.9.12b0/PKG-INFO
+-rw-r--r--   0        0        0     5222 2023-07-23 05:05:39.685000 pg_alchemy_kit-0.9.1b0/README.md
+-rw-r--r--   0        0        0     3361 2024-03-15 17:20:52.235000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PG.py
+-rw-r--r--   0        0        0    12877 2024-04-08 02:01:27.341432 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtils.py
+-rw-r--r--   0        0        0     6323 2024-03-15 17:21:48.231000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtilsBase.py
+-rw-r--r--   0        0        0     5512 2024-03-15 17:22:12.728000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtilsORM.py
+-rw-r--r--   0        0        0      353 2023-12-02 13:44:05.554000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/__init__.py
+-rw-r--r--   0        0        0     2780 2024-04-21 00:55:09.212262 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/AsyncPG.py
+-rw-r--r--   0        0        0     9426 2024-04-21 00:49:46.175891 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/AsyncPGUtilsORM.py
+-rw-r--r--   0        0        0      402 2024-03-05 23:13:28.466000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__init__.py
+-rw-r--r--   0        0        0     2548 2024-04-20 23:32:34.684154 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-310.pyc
+-rw-r--r--   0        0        0     4706 2024-04-21 00:55:25.414792 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-312.pyc
+-rw-r--r--   0        0        0     8382 2024-03-21 22:25:25.802000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsBase.cpython-310.pyc
+-rw-r--r--   0        0        0    10742 2024-04-20 23:32:34.686799 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-310.pyc
+-rw-r--r--   0        0        0    16328 2024-04-21 00:52:13.046852 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-312.pyc
+-rw-r--r--   0        0        0     4980 2024-02-23 22:12:09.581000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PG.cpython-310.pyc
+-rw-r--r--   0        0        0     8275 2024-02-23 22:14:07.165000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsBase.cpython-310.pyc
+-rw-r--r--   0        0        0     5417 2024-02-23 22:16:34.786000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsORM.cpython-310.pyc
+-rw-r--r--   0        0        0      460 2024-03-05 23:14:18.543000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      481 2024-04-20 23:34:09.319347 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     5840 2023-11-01 14:19:01.447000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/cacheStrategies.py
+-rw-r--r--   0        0        0      851 2024-04-21 01:01:41.086173 pg_alchemy_kit-0.9.1b0/pyproject.toml
+-rw-r--r--   0        0        0     5926 1970-01-01 00:00:00.000000 pg_alchemy_kit-0.9.1b0/PKG-INFO
```

### Comparing `pg_alchemy_kit-0.9.12b0/README.md` & `pg_alchemy_kit-0.9.1b0/README.md`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/PG.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PG.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/PGUtils.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtils.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/PGUtilsBase.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtilsBase.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/PGUtilsORM.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtilsORM.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/AsyncPG.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/AsyncPG.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/AsyncPGUtilsORM.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/AsyncPGUtilsORM.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import uuid
 from sqlalchemy import select, Select
 
-from typing import Any, TypeVar, Generic, TypedDict
+from typing import Any, TypeVar, Type, Generic, TypedDict
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy import TextClause, text
 import pandas as pd
 from sqlalchemy.orm.query import Query
 from sqlalchemy.dialects import postgresql
 
 
@@ -180,15 +180,15 @@
             return obj
 
         except Exception as e:
             await session.rollback()
             raise PGUpdateError(str(e))
 
     async def insert(
-        self, session: AsyncSession, model: Any, record: dict[str, Any]
+        self, session: AsyncSession, model: Type[T], record: dict[str, Any]
     ) -> T:
         try:
             if self.snake_case:
                 record = self.to_snake_case([record])[0]
 
             obj = model(**record)
             session.add(obj)
```

### Comparing `pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-312.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsBase.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsBase.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-312.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/PG.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PG.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsBase.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsBase.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsORM.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsORM.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.12b0/pg_alchemy_kit/cacheStrategies.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/cacheStrategies.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.12b0/pyproject.toml` & `pg_alchemy_kit-0.9.1b0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pg-alchemy-kit"
-version = "0.9.12-beta"
+version = "0.9.01-beta"
 description = "A simple wrapper around sqlalchemy to make it easier to use with postgresql"
 authors = ["jsaied99 <jsaied99@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/jsaied99/pg-alchemy-kit"
 packages = [{ include = "pg_alchemy_kit" }]
 
 [tool.poetry.dependencies]
```

### Comparing `pg_alchemy_kit-0.9.12b0/PKG-INFO` & `pg_alchemy_kit-0.9.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-alchemy-kit
-Version: 0.9.12b0
+Version: 0.9.1b0
 Summary: A simple wrapper around sqlalchemy to make it easier to use with postgresql
 Home-page: https://github.com/jsaied99/pg-alchemy-kit
 Author: jsaied99
 Author-email: jsaied99@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```


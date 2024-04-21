# Comparing `tmp/greyhorse_sqla-0.3.1.tar.gz` & `tmp/greyhorse_sqla-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greyhorse_sqla-0.3.1.tar", max compression
+gzip compressed data, was "greyhorse_sqla-0.4.0.tar", max compression
```

## Comparing `greyhorse_sqla-0.3.1.tar` & `greyhorse_sqla-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,9 @@
--rw-r--r--   0        0        0       96 2023-05-30 11:55:28.473575 greyhorse_sqla-0.3.1/greyhorse_sqla/__init__.py
--rw-r--r--   0        0        0     3234 2023-06-28 20:12:22.760341 greyhorse_sqla-0.3.1/greyhorse_sqla/config.py
--rw-r--r--   0        0        0     4769 2023-06-28 20:12:22.596346 greyhorse_sqla-0.3.1/greyhorse_sqla/containers.py
--rw-r--r--   0        0        0     3596 2023-06-28 20:12:22.712343 greyhorse_sqla-0.3.1/greyhorse_sqla/contexts.py
--rw-r--r--   0        0        0     5425 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/engine.py
--rw-r--r--   0        0        0     5138 2023-05-30 11:55:28.477575 greyhorse_sqla-0.3.1/greyhorse_sqla/factory.py
--rw-r--r--   0        0        0        0 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/migration/__init__.py
--rw-r--r--   0        0        0     2281 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/migration/app.py
--rw-r--r--   0        0        0     2121 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/migration/cmd.py
--rw-r--r--   0        0        0      440 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/migration/containers.py
--rw-r--r--   0        0        0     4973 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/migration/operator.py
--rw-r--r--   0        0        0     1559 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/migration/utils.py
--rw-r--r--   0        0        0     3161 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/model.py
--rw-r--r--   0        0        0     1422 2023-05-30 11:55:28.477575 greyhorse_sqla-0.3.1/greyhorse_sqla/query.py
--rw-r--r--   0        0        0    13404 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/repository.py
--rw-r--r--   0        0        0     5876 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/resources.py
--rw-r--r--   0        0        0      237 2023-05-30 11:55:28.477575 greyhorse_sqla-0.3.1/greyhorse_sqla/translations.toml
--rw-r--r--   0        0        0     1446 2023-06-28 20:11:23.522317 greyhorse_sqla-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 greyhorse_sqla-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       91 2024-04-20 19:31:20.232609 greyhorse_sqla-0.4.0/greyhorse_sqla/__init__.py
+-rw-r--r--   0        0        0     3955 2024-04-21 01:22:38.754137 greyhorse_sqla-0.4.0/greyhorse_sqla/config.py
+-rw-r--r--   0        0        0     1238 2024-04-21 01:22:38.746137 greyhorse_sqla-0.4.0/greyhorse_sqla/contexts.py
+-rw-r--r--   0        0        0     9357 2024-04-21 01:22:38.702139 greyhorse_sqla-0.4.0/greyhorse_sqla/engine.py
+-rw-r--r--   0        0        0     3109 2024-04-21 01:22:38.722138 greyhorse_sqla-0.4.0/greyhorse_sqla/factory.py
+-rw-r--r--   0        0        0     5722 2024-04-21 01:03:52.261407 greyhorse_sqla-0.4.0/greyhorse_sqla/service.py
+-rw-r--r--   0        0        0      259 2024-04-20 20:30:40.400220 greyhorse_sqla-0.4.0/greyhorse_sqla/translations.toml
+-rw-r--r--   0        0        0     1581 2024-04-20 19:28:44.424095 greyhorse_sqla-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 greyhorse_sqla-0.4.0/PKG-INFO
```

### Comparing `greyhorse_sqla-0.3.1/pyproject.toml` & `greyhorse_sqla-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 [tool.poetry]
 name = "greyhorse-sqla"
-version = "0.3.1"
+version = "0.4.0"
 description = "Greyhorse SqlAlchemy library"
 license = "MIT"
 repository = "https://gitlab.com/max-plutonium/greyhorse"
 authors = ["Max Plutonium <plutonium.max@gmail.com>"]
 maintainers = ["Max Plutonium <plutonium.max@gmail.com>"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Typing :: Typed",
 ]
 
 packages = [
     { include = "greyhorse_sqla" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
-alembic = "^1.10"
-greyhorse_core = { path = "../core/", develop = true }
-sqlalchemy = {extras = ["asyncio", "mypy"], version = "^2.0"}
-sqlalchemy-utils = "^0.41"
-
-aiosqlite = {version = "^0.18", optional = true}
-asyncpg = {version = "^0.27", optional = true}
-psycopg2 = {version = "^2.9", optional = true}
-aiomysql = {version = "^0.1", optional = true}
-pymysql = {version = "^1.0", extras = ["rsa"], optional = true}
+python = "^3.12"
+greyhorse = [
+    { path = "../../core/", develop = true },
+    { version = "0.4.2" }
+]
+pydantic = {version = "^2.0", extras = ["dotenv"]}
+pydantic-settings = "^2.2.1"
+
+sqlalchemy = {extras = ["asyncio", "mypy"], version = "^2.0.29"}
+sqlalchemy-utils = "^0.41.2"
+
+aiosqlite = {version = "^0.20.0", optional = true}
+asyncpg = {version = "^0.29.0", optional = true}
+psycopg2 = {version = "^2.9.9", optional = true}
+aiomysql = {version = "^0.2.0", optional = true}
+pymysql = {version = "^1.1.0", extras = ["rsa"], optional = true}
 
 [tool.poetry.extras]
 sqlite = ["aiosqlite"]
 pg = ["asyncpg", "psycopg2"]
 mysql = ["aiomysql", "pymysql"]
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2"
-pytest-asyncio = "^0.21"
-pytest-cov = "^4.0"
-pytest-mock = "^3.10"
+pytest = "^7.4"
+pytest-asyncio = "^0.23"
+pytest-cov = "^4.1"
+pytest-mock = "^3.12"
 pytest-faker = "^2.0"
-autoflake = "^2.0"
-black = "^23.1"
-flake8 = "^6.0"
+autoflake = "^2.2"
+black = "^23.11"
+flake8 = "^6.1"
 isort = "^5.12"
-mypy = "^1.1"
-pre-commit = "^3.2"
+mypy = "^1.7"
+pre-commit = "^3.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry-monorepo-dependency-plugin]
 enable = true
```

### Comparing `greyhorse_sqla-0.3.1/PKG-INFO` & `greyhorse_sqla-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: greyhorse-sqla
-Version: 0.3.1
+Version: 0.4.0
 Summary: Greyhorse SqlAlchemy library
 Home-page: https://gitlab.com/max-plutonium/greyhorse
 License: MIT
 Author: Max Plutonium
 Author-email: plutonium.max@gmail.com
 Maintainer: Max Plutonium
 Maintainer-email: plutonium.max@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Typing :: Typed
 Provides-Extra: mysql
 Provides-Extra: pg
 Provides-Extra: sqlite
-Requires-Dist: aiomysql (>=0.1,<0.2) ; extra == "mysql"
-Requires-Dist: aiosqlite (>=0.18,<0.19) ; extra == "sqlite"
-Requires-Dist: alembic (>=1.10,<2.0)
-Requires-Dist: asyncpg (>=0.27,<0.28) ; extra == "pg"
-Requires-Dist: greyhorse_core @ file:///home/plutonium/Projects/greyhorse/core
-Requires-Dist: psycopg2 (>=2.9,<3.0) ; extra == "pg"
-Requires-Dist: pymysql[rsa] (>=1.0,<2.0) ; extra == "mysql"
-Requires-Dist: sqlalchemy-utils (>=0.41,<0.42)
-Requires-Dist: sqlalchemy[asyncio,mypy] (>=2.0,<3.0)
+Requires-Dist: aiomysql (>=0.2.0,<0.3.0) ; extra == "mysql"
+Requires-Dist: aiosqlite (>=0.20.0,<0.21.0) ; extra == "sqlite"
+Requires-Dist: asyncpg (>=0.29.0,<0.30.0) ; extra == "pg"
+Requires-Dist: greyhorse (==0.4.2)
+Requires-Dist: greyhorse @ file:///home/plutonium/projects/greyhorse/core
+Requires-Dist: psycopg2 (>=2.9.9,<3.0.0) ; extra == "pg"
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
+Requires-Dist: pydantic[dotenv] (>=2.0,<3.0)
+Requires-Dist: pymysql[rsa] (>=1.1.0,<2.0.0) ; extra == "mysql"
+Requires-Dist: sqlalchemy-utils (>=0.41.2,<0.42.0)
+Requires-Dist: sqlalchemy[asyncio,mypy] (>=2.0.29,<3.0.0)
 Project-URL: Repository, https://gitlab.com/max-plutonium/greyhorse
```


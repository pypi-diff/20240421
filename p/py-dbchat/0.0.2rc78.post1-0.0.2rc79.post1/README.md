# Comparing `tmp/py_dbchat-0.0.2rc78.post1.tar.gz` & `tmp/py_dbchat-0.0.2rc79.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_dbchat-0.0.2rc78.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_dbchat-0.0.2rc79.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_dbchat-0.0.2rc78.post1.tar` & `py_dbchat-0.0.2rc79.post1.tar`

### file list

```diff
@@ -1,86 +1,89 @@
--rw-r--r--   0        0        0   600200 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/.devcontainer/Chinook_PostgreSql.sql
--rw-r--r--   0        0        0      462 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1822 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      843 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/.devcontainer/docker-compose.yml
--rw-r--r--   0        0        0      417 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/.github/template-sync.yml
--rw-r--r--   0        0        0      476 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      368 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/.gitignore
--rw-r--r--   0        0        0     1381 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/.pypirc
--rw-r--r--   0        0        0      459 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/.vscode/launch.json
--rw-r--r--   0        0        0     1213 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/.vscode/settings.json
--rw-r--r--   0        0        0      444 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/LICENSE
--rw-r--r--   0        0        0       41 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/README.md
--rw-r--r--   0        0        0     2780 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/SECURITY.md
--rw-r--r--   0        0        0     1308 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/SUPPORT.md
--rw-r--r--   0        0        0      655 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/Test.session.sql
--rw-r--r--   0        0        0      634 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/docs/developer.md
--rw-r--r--   0        0        0      468 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/docs/make.bat
--rw-r--r--   0        0        0       50 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/docs/pyproject.md
--rw-r--r--   0        0        0      423 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      406 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/docs/python_package.rst
--rw-r--r--   0        0        0       65 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/docs/workflows.md
--rw-r--r--   0        0        0      274 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/main.py
--rw-r--r--   0        0        0      203 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/playground.py
--rw-r--r--   0        0        0     6679 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/pyproject.toml
--rw-r--r--   0        0        0       26 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/requirements.txt
--rw-r--r--   0        0        0      109 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/src/README.md
--rw-r--r--   0        0        0      161 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/src/Roadmap.md
--rw-r--r--   0        0        0     6148 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/src/db_chat/.DS_Store
--rw-r--r--   0        0        0      374 2024-04-20 15:34:24.274227 py_dbchat-0.0.2rc78.post1/src/db_chat/__init__.py
--rw-r--r--   0        0        0      725 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/src/db_chat/ask.py
--rw-r--r--   0        0        0      662 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/src/db_chat/hello_world.py
--rw-r--r--   0        0        0     3308 2024-04-20 15:34:11.994064 py_dbchat-0.0.2rc78.post1/src/db_chat/llm/classic_prompt.py
--rw-r--r--   0        0        0     3518 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/db_chat/llm/function_calling.py
--rw-r--r--   0        0        0     6791 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/db_chat/llm/llm.py
--rw-r--r--   0        0        0     1135 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/db_chat/llm/llm_langchain_sample.py
--rw-r--r--   0        0        0      250 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/db_chat/sql_builder/Filter.py
--rw-r--r--   0        0        0      236 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/db_chat/sql_builder/FilterOperator.py
--rw-r--r--   0        0        0     2478 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/db_chat/sql_builder/Query.py
--rw-r--r--   0        0        0      159 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/db_chat/sql_builder/SortOrder.py
--rw-r--r--   0        0        0        0 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/db_chat/sql_builder/__init__.py
--rw-r--r--   0        0        0      453 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/db_chat/sql_builder/mappings.py
--rw-r--r--   0        0        0     5193 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/db_chat/sql_builder/schema.py
--rw-r--r--   0        0        0     8781 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/db_chat/sql_builder/sql_builder.py
--rw-r--r--   0        0        0    16036 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py
--rw-r--r--   0        0        0      262 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/main.py
--rw-r--r--   0        0        0      436 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/ui/.eslintrc.cjs
--rw-r--r--   0        0        0      253 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/ui/.gitignore
--rw-r--r--   0        0        0     1300 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/ui/README.md
--rw-r--r--   0        0        0      484 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/ui/index.html
--rw-r--r--   0        0        0   110675 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/ui/package-lock.json
--rw-r--r--   0        0        0      883 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/ui/package.json
--rw-r--r--   0        0        0     1497 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/ui/public/vite.svg
--rw-r--r--   0        0        0     1286 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/ui/src/App.css
--rw-r--r--   0        0        0     1542 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/ui/src/App.tsx
--rw-r--r--   0        0        0     4126 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/ui/src/assets/react.svg
--rw-r--r--   0        0        0     1161 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/ui/src/index.css
--rw-r--r--   0        0        0      236 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/ui/src/main.tsx
--rw-r--r--   0        0        0       38 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/ui/src/vite-env.d.ts
--rw-r--r--   0        0        0      605 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/ui/tsconfig.json
--rw-r--r--   0        0        0      233 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/ui/tsconfig.node.json
--rw-r--r--   0        0        0      167 2024-04-20 15:34:11.998064 py_dbchat-0.0.2rc78.post1/src/ui/vite.config.ts
--rw-r--r--   0        0        0   600200 2024-04-20 15:34:12.002064 py_dbchat-0.0.2rc78.post1/test/Chinook_PostgreSql.sql
--rw-r--r--   0        0        0      989 2024-04-20 15:34:12.002064 py_dbchat-0.0.2rc78.post1/tests/conftest.py
--rw-r--r--   0        0        0     2922 2024-04-20 15:34:12.002064 py_dbchat-0.0.2rc78.post1/tests/test_explicit_joins.py
--rw-r--r--   0        0        0     1210 2024-04-20 15:34:12.002064 py_dbchat-0.0.2rc78.post1/tests/test_methods.py
--rw-r--r--   0        0        0      269 2024-04-20 15:34:12.002064 py_dbchat-0.0.2rc78.post1/tests/test_schema_builder.py
--rw-r--r--   0        0        0    12288 2024-04-20 15:34:12.002064 py_dbchat-0.0.2rc78.post1/tests/test_sql_builder.py
--rw-r--r--   0        0        0     7124 2024-04-20 15:34:12.002064 py_dbchat-0.0.2rc78.post1/tests/test_sqlalchemy.py
--rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 py_dbchat-0.0.2rc78.post1/PKG-INFO
+-rw-r--r--   0        0        0   600200 2024-04-21 05:57:15.613280 py_dbchat-0.0.2rc79.post1/.devcontainer/Chinook_PostgreSql.sql
+-rw-r--r--   0        0        0      462 2024-04-21 05:57:15.613280 py_dbchat-0.0.2rc79.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1822 2024-04-21 05:57:15.613280 py_dbchat-0.0.2rc79.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      843 2024-04-21 05:57:15.613280 py_dbchat-0.0.2rc79.post1/.devcontainer/docker-compose.yml
+-rw-r--r--   0        0        0      417 2024-04-21 05:57:15.613280 py_dbchat-0.0.2rc79.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-21 05:57:15.613280 py_dbchat-0.0.2rc79.post1/.github/template-sync.yml
+-rw-r--r--   0        0        0      476 2024-04-21 05:57:15.613280 py_dbchat-0.0.2rc79.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-21 05:57:15.613280 py_dbchat-0.0.2rc79.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-21 05:57:15.613280 py_dbchat-0.0.2rc79.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      318 2024-04-21 05:57:15.613280 py_dbchat-0.0.2rc79.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      368 2024-04-21 05:57:15.613280 py_dbchat-0.0.2rc79.post1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-21 05:57:15.613280 py_dbchat-0.0.2rc79.post1/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/.gitignore
+-rw-r--r--   0        0        0     1381 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/.pypirc
+-rw-r--r--   0        0        0      459 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/.vscode/launch.json
+-rw-r--r--   0        0        0     1213 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/.vscode/settings.json
+-rw-r--r--   0        0        0      444 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/LICENSE
+-rw-r--r--   0        0        0       41 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/README.md
+-rw-r--r--   0        0        0     2780 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/SECURITY.md
+-rw-r--r--   0        0        0     1308 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/SUPPORT.md
+-rw-r--r--   0        0        0      655 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/Test.session.sql
+-rw-r--r--   0        0        0      634 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/docs/make.bat
+-rw-r--r--   0        0        0       50 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      423 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      406 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/docs/python_package.rst
+-rw-r--r--   0        0        0       65 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/docs/workflows.md
+-rw-r--r--   0        0        0      274 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/main.py
+-rw-r--r--   0        0        0      203 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/playground.py
+-rw-r--r--   0        0        0     6679 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/pyproject.toml
+-rw-r--r--   0        0        0       26 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/requirements.txt
+-rw-r--r--   0        0        0      109 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/README.md
+-rw-r--r--   0        0        0      161 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/Roadmap.md
+-rw-r--r--   0        0        0     6148 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/db_chat/.DS_Store
+-rw-r--r--   0        0        0      374 2024-04-21 05:57:28.185330 py_dbchat-0.0.2rc79.post1/src/db_chat/__init__.py
+-rw-r--r--   0        0        0      725 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/db_chat/ask.py
+-rw-r--r--   0        0        0      662 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/db_chat/hello_world.py
+-rw-r--r--   0        0        0     3833 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/db_chat/llm/classic_prompt.py
+-rw-r--r--   0        0        0     3518 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/db_chat/llm/function_calling.py
+-rw-r--r--   0        0        0     6791 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/db_chat/llm/llm.py
+-rw-r--r--   0        0        0     1135 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/db_chat/llm/llm_langchain_sample.py
+-rw-r--r--   0        0        0      250 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/db_chat/sql_builder/Filter.py
+-rw-r--r--   0        0        0      236 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/db_chat/sql_builder/FilterOperator.py
+-rw-r--r--   0        0        0     2478 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/db_chat/sql_builder/Query.py
+-rw-r--r--   0        0        0      159 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/db_chat/sql_builder/SortOrder.py
+-rw-r--r--   0        0        0        0 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/db_chat/sql_builder/__init__.py
+-rw-r--r--   0        0        0      453 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/db_chat/sql_builder/mappings.py
+-rw-r--r--   0        0        0     5193 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/db_chat/sql_builder/schema.py
+-rw-r--r--   0        0        0     8781 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/db_chat/sql_builder/sql_builder.py
+-rw-r--r--   0        0        0    16036 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py
+-rw-r--r--   0        0        0      262 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/main.py
+-rw-r--r--   0        0        0      436 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/.eslintrc.cjs
+-rw-r--r--   0        0        0      253 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/.gitignore
+-rw-r--r--   0        0        0     1300 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/README.md
+-rw-r--r--   0        0        0      484 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/index.html
+-rw-r--r--   0        0        0   118627 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/package-lock.json
+-rw-r--r--   0        0        0      909 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/package.json
+-rw-r--r--   0        0        0     1497 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/public/vite.svg
+-rw-r--r--   0        0        0     1286 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/src/App.css
+-rw-r--r--   0        0        0     1345 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/src/App.tsx
+-rw-r--r--   0        0        0     2762 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/src/api/baseApi.ts
+-rw-r--r--   0        0        0     4126 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/src/assets/react.svg
+-rw-r--r--   0        0        0     1161 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/src/index.css
+-rw-r--r--   0        0        0      236 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/src/main.tsx
+-rw-r--r--   0        0        0       83 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/src/types/Setting.ts
+-rw-r--r--   0        0        0       64 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/src/types/schema.ts
+-rw-r--r--   0        0        0       38 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/src/vite-env.d.ts
+-rw-r--r--   0        0        0      605 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/tsconfig.json
+-rw-r--r--   0        0        0      233 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/tsconfig.node.json
+-rw-r--r--   0        0        0      167 2024-04-21 05:57:15.617280 py_dbchat-0.0.2rc79.post1/src/ui/vite.config.ts
+-rw-r--r--   0        0        0   600200 2024-04-21 05:57:15.621280 py_dbchat-0.0.2rc79.post1/test/Chinook_PostgreSql.sql
+-rw-r--r--   0        0        0      989 2024-04-21 05:57:15.621280 py_dbchat-0.0.2rc79.post1/tests/conftest.py
+-rw-r--r--   0        0        0     2922 2024-04-21 05:57:15.621280 py_dbchat-0.0.2rc79.post1/tests/test_explicit_joins.py
+-rw-r--r--   0        0        0     1210 2024-04-21 05:57:15.621280 py_dbchat-0.0.2rc79.post1/tests/test_methods.py
+-rw-r--r--   0        0        0      269 2024-04-21 05:57:15.621280 py_dbchat-0.0.2rc79.post1/tests/test_schema_builder.py
+-rw-r--r--   0        0        0    12288 2024-04-21 05:57:15.621280 py_dbchat-0.0.2rc79.post1/tests/test_sql_builder.py
+-rw-r--r--   0        0        0     7124 2024-04-21 05:57:15.621280 py_dbchat-0.0.2rc79.post1/tests/test_sqlalchemy.py
+-rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 py_dbchat-0.0.2rc79.post1/PKG-INFO
```

### Comparing `py_dbchat-0.0.2rc78.post1/.devcontainer/Chinook_PostgreSql.sql` & `py_dbchat-0.0.2rc79.post1/.devcontainer/Chinook_PostgreSql.sql`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/.devcontainer/devcontainer.json` & `py_dbchat-0.0.2rc79.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/.devcontainer/docker-compose.yml` & `py_dbchat-0.0.2rc79.post1/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/.github/workflows/schedule-update-actions.yml` & `py_dbchat-0.0.2rc79.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/.gitignore` & `py_dbchat-0.0.2rc79.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/.pre-commit-config.yaml` & `py_dbchat-0.0.2rc79.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/.vscode/settings.json` & `py_dbchat-0.0.2rc79.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/LICENSE` & `py_dbchat-0.0.2rc79.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/SECURITY.md` & `py_dbchat-0.0.2rc79.post1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/SUPPORT.md` & `py_dbchat-0.0.2rc79.post1/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/Test.session.sql` & `py_dbchat-0.0.2rc79.post1/Test.session.sql`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/docs/Makefile` & `py_dbchat-0.0.2rc79.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/docs/conf.py` & `py_dbchat-0.0.2rc79.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/docs/make.bat` & `py_dbchat-0.0.2rc79.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/docs/pylint.md` & `py_dbchat-0.0.2rc79.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/pyproject.toml` & `py_dbchat-0.0.2rc79.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/src/db_chat/.DS_Store` & `py_dbchat-0.0.2rc79.post1/src/db_chat/.DS_Store`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/src/db_chat/ask.py` & `py_dbchat-0.0.2rc79.post1/src/db_chat/ask.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/src/db_chat/hello_world.py` & `py_dbchat-0.0.2rc79.post1/src/db_chat/hello_world.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/src/db_chat/llm/classic_prompt.py` & `py_dbchat-0.0.2rc79.post1/src/db_chat/llm/classic_prompt.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,21 @@
 
 
 def build_rules():
     rules = """
     You will follow these rules while creating a json response:
     1. The json response will only contain the below listed keys
     2. `table` key will contain the name of the table to fetch the data from
-    3. `fields` key will contain the list of fields to fetch from the chosen table. Fields of each table will be listed in a separate list after the rules.
+    3. `joins` - dictionary of joins to apply to the query, where key is the alias of join. Each join will have the following keys
+            3.a. `type` -  Allowed values are `inner`, `left`, `right`, `full`
+            3.b. `table` - Name of the table to join with
+            3.c. `field` - Field of the current table to join with
+            3.d. `related_field` - Field of the joined table to join with
+
+    3. `fields` key will contain the list of fields to fetch from the chosen table.Join fields are represented `join alias`.`field` . Fields of each table will be listed in a separate list after the rules. Join fields will be listed in the same list as the table fields.
     4. `filters` key will contain the list of filters to apply to the query. Each filter will have a 'field', 'operator' and 'value'. Allowed operators are 'eq', 'neq', 'gt', 'lt', 'gte', 'lte', 'like'
     5. `sort` -  will  have a 'field' and 'direction'.
         4.a. `field` - Field to sort to sort by. Use columns from the chosen `table` only . Do not make up new columns.
         4.b. `direction` - Allowed direction are 'asc' and 'desc'.
     6. `limit` key will contain the number of rows to limit the result to
     7. `offset` key will contain the number of rows to offset the result by
```

### Comparing `py_dbchat-0.0.2rc78.post1/src/db_chat/llm/function_calling.py` & `py_dbchat-0.0.2rc79.post1/src/db_chat/llm/function_calling.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/src/db_chat/llm/llm.py` & `py_dbchat-0.0.2rc79.post1/src/db_chat/llm/llm.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/src/db_chat/llm/llm_langchain_sample.py` & `py_dbchat-0.0.2rc79.post1/src/db_chat/llm/llm_langchain_sample.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/src/db_chat/sql_builder/Query.py` & `py_dbchat-0.0.2rc79.post1/src/db_chat/sql_builder/Query.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/src/db_chat/sql_builder/schema.py` & `py_dbchat-0.0.2rc79.post1/src/db_chat/sql_builder/schema.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/src/db_chat/sql_builder/sql_builder.py` & `py_dbchat-0.0.2rc79.post1/src/db_chat/sql_builder/sql_builder.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py` & `py_dbchat-0.0.2rc79.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/src/ui/README.md` & `py_dbchat-0.0.2rc79.post1/src/ui/README.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/src/ui/package-lock.json` & `py_dbchat-0.0.2rc79.post1/src/ui/package-lock.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921314874264313%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'boxicons': '^2.1.4'}}, "*

 * *               "'node_modules/@webcomponents/webcomponentsjs': OrderedDict([('version', '2.8.0'), "*

 * *               "('resolved', "*

 * *               "'https://registry.npmjs.org/@webcomponents/webcomponentsjs/-/webcomponentsjs-2.8.0.tgz'), "*

 * *               "('integrity', "*

 * *               "'sha512-loGD63sacRzOzSJgQnB9ZAhaQGkN7wl2Zuw7tsphI5Isa0irijrRo6EnJii/GgjGefIFO8AIO7UivzRhFaEk9w==')]), "*

 * *               "'node_modules/boxicons': OrderedDict([(' […]*

```diff
@@ -2,14 +2,15 @@
     "lockfileVersion": 3,
     "name": "ui",
     "packages": {
         "": {
             "dependencies": {
                 "@popperjs/core": "^2.11.8",
                 "bootstrap": "^5.3.3",
+                "boxicons": "^2.1.4",
                 "react": "^18.2.0",
                 "react-bootstrap": "^2.10.2",
                 "react-dom": "^18.2.0",
                 "zustand": "^4.5.2"
             },
             "devDependencies": {
                 "@types/react": "^18.2.66",
@@ -1332,14 +1333,19 @@
             "integrity": "sha512-XFRbsGgpGxGzEV5i5+vRiro1bwcIaZDIdBRP16qwm+jP68ue/S8FJTBEgOeojtVDYrbSua3XFp71kC8VJE6v+g==",
             "peerDependencies": {
                 "vite": "^4 || ^5"
             },
             "resolved": "https://registry.npmjs.org/@vitejs/plugin-react-swc/-/plugin-react-swc-3.6.0.tgz",
             "version": "3.6.0"
         },
+        "node_modules/@webcomponents/webcomponentsjs": {
+            "integrity": "sha512-loGD63sacRzOzSJgQnB9ZAhaQGkN7wl2Zuw7tsphI5Isa0irijrRo6EnJii/GgjGefIFO8AIO7UivzRhFaEk9w==",
+            "resolved": "https://registry.npmjs.org/@webcomponents/webcomponentsjs/-/webcomponentsjs-2.8.0.tgz",
+            "version": "2.8.0"
+        },
         "node_modules/acorn": {
             "bin": {
                 "acorn": "bin/acorn"
             },
             "dev": true,
             "engines": {
                 "node": ">=0.4.0"
@@ -1457,14 +1463,63 @@
             "integrity": "sha512-8HLCdWgyoMguSO9o+aH+iuZ+aht+mzW0u3HIMzVu7Srrpv7EBBxTnrFlSCskwdY1+EOFQSm7uMJhNQHkdPcmjg==",
             "peerDependencies": {
                 "@popperjs/core": "^2.11.8"
             },
             "resolved": "https://registry.npmjs.org/bootstrap/-/bootstrap-5.3.3.tgz",
             "version": "5.3.3"
         },
+        "node_modules/boxicons": {
+            "dependencies": {
+                "@webcomponents/webcomponentsjs": "^2.0.2",
+                "prop-types": "^15.6.0",
+                "react": "^16.0.0",
+                "react-dom": "^16.0.0",
+                "react-interactive": "^0.8.1",
+                "react-router-dom": "^4.2.2"
+            },
+            "integrity": "sha512-BvJNfYfnE4g9WQ7GL91fftxMOTwAleWlPFwvQJPYb/Ju7aLjlQ/Eu55AH9JLNk/OR82z+ZSq4TbKzbV/e5Rr0A==",
+            "resolved": "https://registry.npmjs.org/boxicons/-/boxicons-2.1.4.tgz",
+            "version": "2.1.4"
+        },
+        "node_modules/boxicons/node_modules/react": {
+            "dependencies": {
+                "loose-envify": "^1.1.0",
+                "object-assign": "^4.1.1",
+                "prop-types": "^15.6.2"
+            },
+            "engines": {
+                "node": ">=0.10.0"
+            },
+            "integrity": "sha512-0X2CImDkJGApiAlcf0ODKIneSwBPhqJawOa5wCtKbu7ZECrmS26NvtSILynQ66cgkT/RJ4LidJOc3bUESwmU8g==",
+            "resolved": "https://registry.npmjs.org/react/-/react-16.14.0.tgz",
+            "version": "16.14.0"
+        },
+        "node_modules/boxicons/node_modules/react-dom": {
+            "dependencies": {
+                "loose-envify": "^1.1.0",
+                "object-assign": "^4.1.1",
+                "prop-types": "^15.6.2",
+                "scheduler": "^0.19.1"
+            },
+            "integrity": "sha512-1gCeQXDLoIqMgqD3IO2Ah9bnf0w9kzhwN5q4FGnHZ67hBm9yePzB5JJAIQCc8x3pFnNlwFq4RidZggNAAkzWWw==",
+            "peerDependencies": {
+                "react": "^16.14.0"
+            },
+            "resolved": "https://registry.npmjs.org/react-dom/-/react-dom-16.14.0.tgz",
+            "version": "16.14.0"
+        },
+        "node_modules/boxicons/node_modules/scheduler": {
+            "dependencies": {
+                "loose-envify": "^1.1.0",
+                "object-assign": "^4.1.1"
+            },
+            "integrity": "sha512-n/zwRWRYSUj0/3g/otKDRPMh6qv2SYMWNq85IEa8iZyAv8od9zDYpGSnpBEjNgcMNq6Scbu5KfIPxNF72R/2EA==",
+            "resolved": "https://registry.npmjs.org/scheduler/-/scheduler-0.19.1.tgz",
+            "version": "0.19.1"
+        },
         "node_modules/brace-expansion": {
             "dependencies": {
                 "balanced-match": "^1.0.0"
             },
             "dev": true,
             "integrity": "sha512-XnAIvQ8eM+kC6aULx6wuQiwVsnzsi9d3WxzV3FpWTGA19F621kwdbsAcFKXgKUHZWsy+mY6iL1sHTxWEFCytDA==",
             "resolved": "https://registry.npmjs.org/brace-expansion/-/brace-expansion-2.0.1.tgz",
@@ -1618,14 +1673,45 @@
             "engines": {
                 "node": ">=6"
             },
             "integrity": "sha512-0je+qPKHEMohvfRTCEo3CrPG6cAzAYgmzKyxRiYSSDkS6eGJdyVJm7WaYA5ECaAD9wLB2T4EEeymA5aFVcYXCA==",
             "resolved": "https://registry.npmjs.org/dequal/-/dequal-2.0.3.tgz",
             "version": "2.0.3"
         },
+        "node_modules/detect-hover": {
+            "integrity": "sha512-HtLoY+tClgYucJNiovNICGWFp9nOGVmHY44s7L62iPqORXM9vujeWFaVcqtA7XRvp/2Y+4RBUfHbDKFGN+xxZQ==",
+            "resolved": "https://registry.npmjs.org/detect-hover/-/detect-hover-1.0.3.tgz",
+            "version": "1.0.3"
+        },
+        "node_modules/detect-it": {
+            "dependencies": {
+                "detect-hover": "^1.0.3",
+                "detect-passive-events": "^1.0.5",
+                "detect-pointer": "^1.0.3",
+                "detect-touch-events": "^2.0.2"
+            },
+            "integrity": "sha512-RxpgcdbatUX6epJE09K16iJqF7x6iEcEdoL18FR2zpBO4JhnL7aMOAUoUEyexdtbWOSfTmoDWmeD6mwRBQyRXg==",
+            "resolved": "https://registry.npmjs.org/detect-it/-/detect-it-3.0.7.tgz",
+            "version": "3.0.7"
+        },
+        "node_modules/detect-passive-events": {
+            "integrity": "sha512-foW7Q35wwOCxVzW0xLf5XeB5Fhe7oyRgvkBYdiP9IWgLMzjqUqTvsJv9ymuEWGjY6AoDXD3OC294+Z9iuOw0QA==",
+            "resolved": "https://registry.npmjs.org/detect-passive-events/-/detect-passive-events-1.0.5.tgz",
+            "version": "1.0.5"
+        },
+        "node_modules/detect-pointer": {
+            "integrity": "sha512-d0o/Puo3fiGSCXy6H039h9Kwz+mmYCGKZ/qtPFnpN3WfsumjC1C9b5KKvRu+aYnfdI8peqN/iAe7dPd85qIt2g==",
+            "resolved": "https://registry.npmjs.org/detect-pointer/-/detect-pointer-1.0.3.tgz",
+            "version": "1.0.3"
+        },
+        "node_modules/detect-touch-events": {
+            "integrity": "sha512-g8GWBkJLiIDRJfRXEdrd1wMXpNyGId2DkbfuwFahSb4OCvn717hyRJtAcEDISfp3zkwEhZ4Y4woHPA6DeyB3Fw==",
+            "resolved": "https://registry.npmjs.org/detect-touch-events/-/detect-touch-events-2.0.2.tgz",
+            "version": "2.0.2"
+        },
         "node_modules/dir-glob": {
             "dependencies": {
                 "path-type": "^4.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=8"
@@ -2125,14 +2211,32 @@
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-EykJT/Q1KjTWctppgIAgfSO0tKVuZUjhgMr17kqTumMl6Afv3EISleU7qZUzoXDFTAHTDC4NOoG/ZxU3EvlMPQ==",
             "resolved": "https://registry.npmjs.org/has-flag/-/has-flag-4.0.0.tgz",
             "version": "4.0.0"
         },
+        "node_modules/history": {
+            "dependencies": {
+                "@babel/runtime": "^7.1.2",
+                "loose-envify": "^1.2.0",
+                "resolve-pathname": "^3.0.0",
+                "tiny-invariant": "^1.0.2",
+                "tiny-warning": "^1.0.0",
+                "value-equal": "^1.0.1"
+            },
+            "integrity": "sha512-36nwAD620w12kuzPAsyINPWJqlNbij+hpK1k9XRloDtym8mxzGYl2c17LnV6IAGB2Dmg4tEa7G7DlawS0+qjew==",
+            "resolved": "https://registry.npmjs.org/history/-/history-4.10.1.tgz",
+            "version": "4.10.1"
+        },
+        "node_modules/hoist-non-react-statics": {
+            "integrity": "sha512-rqcy4pJo55FTTLWt+bU8ukscqHeE/e9KWvsOW2b/a3afxQZhwkQdT1rPPCJ0rYXdj4vNcasY8zHTH+jF/qStxw==",
+            "resolved": "https://registry.npmjs.org/hoist-non-react-statics/-/hoist-non-react-statics-2.5.5.tgz",
+            "version": "2.5.5"
+        },
         "node_modules/ignore": {
             "dev": true,
             "engines": {
                 "node": ">= 4"
             },
             "integrity": "sha512-5Fytz/IraMjqpwfd34ke28PTVMjZjJG2MPn5t7OE4eUCUNf8BAa7b5WUS9/Qvr6mwOQS7Mk6vdsMno5he+T8Xw==",
             "resolved": "https://registry.npmjs.org/ignore/-/ignore-5.3.1.tgz",
@@ -2240,14 +2344,19 @@
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-Fd4gABb+ycGAmKou8eMftCupSir5lRxqf4aD/vd0cD2qc4HL07OjCeuHMr8Ro4CoMaeCKDB0/ECBOVWjTwUvPQ==",
             "resolved": "https://registry.npmjs.org/is-path-inside/-/is-path-inside-3.0.3.tgz",
             "version": "3.0.3"
         },
+        "node_modules/isarray": {
+            "integrity": "sha512-D2S+3GLxWH+uhrNEcoh/fnmYeP8E8/zHl644d/jdA0g2uyXvy3sb0qxotE+ne0LtccHknQzWwZEzhak7oJ0COQ==",
+            "resolved": "https://registry.npmjs.org/isarray/-/isarray-0.0.1.tgz",
+            "version": "0.0.1"
+        },
         "node_modules/isexe": {
             "dev": true,
             "integrity": "sha512-RHxMLp9lnKHGHRng9QFhRCMbYAcVpn69smSGcq3f36xjgVVWThj4qqLbTLlq7Ssj8B+fIQ1EuCEGI2lKsyQeIw==",
             "resolved": "https://registry.npmjs.org/isexe/-/isexe-2.0.0.tgz",
             "version": "2.0.0"
         },
         "node_modules/js-tokens": {
@@ -2526,14 +2635,22 @@
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-ojmeN0qd+y0jszEtoY48r0Peq5dwMEkIlCOu6Q5f41lfkswXuKtYrhgoTpLnyIcHm24Uhqx+5Tqm2InSwLhE6Q==",
             "resolved": "https://registry.npmjs.org/path-key/-/path-key-3.1.1.tgz",
             "version": "3.1.1"
         },
+        "node_modules/path-to-regexp": {
+            "dependencies": {
+                "isarray": "0.0.1"
+            },
+            "integrity": "sha512-n43JRhlUKUAlibEJhPeir1ncUID16QnEjNpwzNdO3Lm4ywrBpBZ5oLD0I6br9evr1Y9JTqwRtAh7JLoOzAQdVA==",
+            "resolved": "https://registry.npmjs.org/path-to-regexp/-/path-to-regexp-1.8.0.tgz",
+            "version": "1.8.0"
+        },
         "node_modules/path-type": {
             "dev": true,
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-gDKb8aZMDeD/tZWs9P6+q0J9Mwkdl6xMV8TjnGP3qJVJ06bdMgkbBlLU8IdfOsIsFz2BW1rNVT3XuNEl8zPAvw==",
             "resolved": "https://registry.npmjs.org/path-type/-/path-type-4.0.0.tgz",
@@ -2693,24 +2810,70 @@
             "integrity": "sha512-6IMTriUmvsjHUjNtEDudZfuDQUoWXVxKHhlEGSk81n4YFS+r/Kl99wXiwlVXtPBtJenozv2P+hxDsw9eA7Xo6g==",
             "peerDependencies": {
                 "react": "^18.2.0"
             },
             "resolved": "https://registry.npmjs.org/react-dom/-/react-dom-18.2.0.tgz",
             "version": "18.2.0"
         },
+        "node_modules/react-interactive": {
+            "dependencies": {
+                "detect-it": "^3.0.3",
+                "object-assign": "^4.1.1",
+                "prop-types": "^15.6.0"
+            },
+            "integrity": "sha512-mmRvA9aKP7zu9kVfP1AX1egX8tFlnE3DDXq92z0JTZezfOpmeQBzr77O1+mTV54OOmn+M2t6c5kFD5VnuFoM7A==",
+            "peerDependencies": {
+                "react": ">=15"
+            },
+            "resolved": "https://registry.npmjs.org/react-interactive/-/react-interactive-0.8.3.tgz",
+            "version": "0.8.3"
+        },
         "node_modules/react-is": {
             "integrity": "sha512-24e6ynE2H+OKt4kqsOvNd8kBpV65zoxbA4BVsEOB3ARVWQki/DHzaUoC5KuON/BiccDaCCTZBuOcfZs70kR8bQ==",
             "resolved": "https://registry.npmjs.org/react-is/-/react-is-16.13.1.tgz",
             "version": "16.13.1"
         },
         "node_modules/react-lifecycles-compat": {
             "integrity": "sha512-fBASbA6LnOU9dOU2eW7aQ8xmYBSXUIWr+UmF9b1efZBazGNO+rcXT/icdKnYm2pTwcRylVUYwW7H1PHfLekVzA==",
             "resolved": "https://registry.npmjs.org/react-lifecycles-compat/-/react-lifecycles-compat-3.0.4.tgz",
             "version": "3.0.4"
         },
+        "node_modules/react-router": {
+            "dependencies": {
+                "history": "^4.7.2",
+                "hoist-non-react-statics": "^2.5.0",
+                "invariant": "^2.2.4",
+                "loose-envify": "^1.3.1",
+                "path-to-regexp": "^1.7.0",
+                "prop-types": "^15.6.1",
+                "warning": "^4.0.1"
+            },
+            "integrity": "sha512-yrvL8AogDh2X42Dt9iknk4wF4V8bWREPirFfS9gLU1huk6qK41sg7Z/1S81jjTrGHxa3B8R3J6xIkDAA6CVarg==",
+            "peerDependencies": {
+                "react": ">=15"
+            },
+            "resolved": "https://registry.npmjs.org/react-router/-/react-router-4.3.1.tgz",
+            "version": "4.3.1"
+        },
+        "node_modules/react-router-dom": {
+            "dependencies": {
+                "history": "^4.7.2",
+                "invariant": "^2.2.4",
+                "loose-envify": "^1.3.1",
+                "prop-types": "^15.6.1",
+                "react-router": "^4.3.1",
+                "warning": "^4.0.1"
+            },
+            "integrity": "sha512-c/MlywfxDdCp7EnB7YfPMOfMD3tOtIjrQlj/CKfNMBxdmpJP8xcz5P/UAFn3JbnQCNUxsHyVVqllF9LhgVyFCA==",
+            "peerDependencies": {
+                "react": ">=15"
+            },
+            "resolved": "https://registry.npmjs.org/react-router-dom/-/react-router-dom-4.3.1.tgz",
+            "version": "4.3.1"
+        },
         "node_modules/react-transition-group": {
             "dependencies": {
                 "@babel/runtime": "^7.5.5",
                 "dom-helpers": "^5.0.1",
                 "loose-envify": "^1.4.0",
                 "prop-types": "^15.6.2"
             },
@@ -2744,14 +2907,19 @@
             "engines": {
                 "node": ">=4"
             },
             "integrity": "sha512-pb/MYmXstAkysRFx8piNI1tGFNQIFA3vkE3Gq4EuA1dF6gHp/+vgZqsCGJapvy8N3Q+4o7FwvquPJcnZ7RYy4g==",
             "resolved": "https://registry.npmjs.org/resolve-from/-/resolve-from-4.0.0.tgz",
             "version": "4.0.0"
         },
+        "node_modules/resolve-pathname": {
+            "integrity": "sha512-C7rARubxI8bXFNB/hqcp/4iUeIXJhJZvFPFPiSPRnhU5UPxzMFIl+2E6yY6c4k9giDJAhtV+enfA+G89N6Csng==",
+            "resolved": "https://registry.npmjs.org/resolve-pathname/-/resolve-pathname-3.0.0.tgz",
+            "version": "3.0.0"
+        },
         "node_modules/reusify": {
             "dev": true,
             "engines": {
                 "iojs": ">=1.0.0",
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-U9nH88a3fc/ekCF1l0/UP1IosiuIjyTh7hBvXVMHYgVcfGvt897Xguj2UOLDeI5BG2m7/uwyaLVT6fbtCwTyzw==",
@@ -2948,14 +3116,24 @@
         },
         "node_modules/text-table": {
             "dev": true,
             "integrity": "sha512-N+8UisAXDGk8PFXP4HAzVR9nbfmVJ3zYLAWiTIoqC5v5isinhr+r5uaO8+7r3BMfuNIufIsA7RdpVgacC2cSpw==",
             "resolved": "https://registry.npmjs.org/text-table/-/text-table-0.2.0.tgz",
             "version": "0.2.0"
         },
+        "node_modules/tiny-invariant": {
+            "integrity": "sha512-+FbBPE1o9QAYvviau/qC5SE3caw21q3xkvWKBtja5vgqOWIHHJ3ioaq1VPfn/Szqctz2bU/oYeKd9/z5BL+PVg==",
+            "resolved": "https://registry.npmjs.org/tiny-invariant/-/tiny-invariant-1.3.3.tgz",
+            "version": "1.3.3"
+        },
+        "node_modules/tiny-warning": {
+            "integrity": "sha512-lBN9zLN/oAf68o3zNXYrdCt1kP8WsiGW8Oo2ka41b2IM5JL/S1CTyX1rW0mb/zSuJun0ZUrDxx4sqvYS2FWzPA==",
+            "resolved": "https://registry.npmjs.org/tiny-warning/-/tiny-warning-1.0.3.tgz",
+            "version": "1.0.3"
+        },
         "node_modules/to-regex-range": {
             "dependencies": {
                 "is-number": "^7.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=8.0"
@@ -3045,14 +3223,19 @@
             "integrity": "sha512-eEgnFxGQ1Ife9bzYs6VLi8/4X6CObHMw9Qr9tPY43iKwsPw8xE8+EFsf/2cFZ5S3esXgpWgtSCtLNS41F+sKPA==",
             "peerDependencies": {
                 "react": "^16.8.0 || ^17.0.0 || ^18.0.0"
             },
             "resolved": "https://registry.npmjs.org/use-sync-external-store/-/use-sync-external-store-1.2.0.tgz",
             "version": "1.2.0"
         },
+        "node_modules/value-equal": {
+            "integrity": "sha512-NOJ6JZCAWr0zlxZt+xqCHNTEKOsrks2HQd4MqhP1qy4z1SkbEP467eNx6TgDKXMvUOb+OENfJCZwM+16n7fRfw==",
+            "resolved": "https://registry.npmjs.org/value-equal/-/value-equal-1.0.1.tgz",
+            "version": "1.0.1"
+        },
         "node_modules/vite": {
             "bin": {
                 "vite": "bin/vite.js"
             },
             "dependencies": {
                 "esbuild": "^0.20.1",
                 "postcss": "^8.4.38",
```

### Comparing `py_dbchat-0.0.2rc78.post1/src/ui/package.json` & `py_dbchat-0.0.2rc79.post1/src/ui/package.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9897959183673469%*

 * *Differences: {"'dependencies'": "{'boxicons': '^2.1.4'}"}*

```diff
@@ -1,11 +1,12 @@
 {
     "dependencies": {
         "@popperjs/core": "^2.11.8",
         "bootstrap": "^5.3.3",
+        "boxicons": "^2.1.4",
         "react": "^18.2.0",
         "react-bootstrap": "^2.10.2",
         "react-dom": "^18.2.0",
         "zustand": "^4.5.2"
     },
     "devDependencies": {
         "@types/react": "^18.2.66",
```

### Comparing `py_dbchat-0.0.2rc78.post1/src/ui/public/vite.svg` & `py_dbchat-0.0.2rc79.post1/src/ui/public/vite.svg`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/src/ui/src/App.css` & `py_dbchat-0.0.2rc79.post1/src/ui/src/App.css`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/src/ui/src/assets/react.svg` & `py_dbchat-0.0.2rc79.post1/src/ui/src/assets/react.svg`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/src/ui/src/index.css` & `py_dbchat-0.0.2rc79.post1/src/ui/src/index.css`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/src/ui/tsconfig.json` & `py_dbchat-0.0.2rc79.post1/src/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/test/Chinook_PostgreSql.sql` & `py_dbchat-0.0.2rc79.post1/test/Chinook_PostgreSql.sql`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/tests/conftest.py` & `py_dbchat-0.0.2rc79.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/tests/test_explicit_joins.py` & `py_dbchat-0.0.2rc79.post1/tests/test_explicit_joins.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/tests/test_methods.py` & `py_dbchat-0.0.2rc79.post1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/tests/test_sql_builder.py` & `py_dbchat-0.0.2rc79.post1/tests/test_sql_builder.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/tests/test_sqlalchemy.py` & `py_dbchat-0.0.2rc79.post1/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc78.post1/PKG-INFO` & `py_dbchat-0.0.2rc79.post1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-dbchat
-Version: 0.0.2rc78.post1
+Version: 0.0.2rc79.post1
 Summary: Chat with your existing database without using vector DB.
 Author-email: Dhanilan <mail2dhanilan@gmail.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```


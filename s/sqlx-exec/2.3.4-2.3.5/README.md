# Comparing `tmp/sqlx-exec-2.3.4.tar.gz` & `tmp/sqlx-exec-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlx-exec-2.3.4.tar", last modified: Fri Apr  5 02:31:35 2024, max compression
+gzip compressed data, was "sqlx-exec-2.3.5.tar", last modified: Sun Apr 21 13:17:48 2024, max compression
```

## Comparing `sqlx-exec-2.3.4.tar` & `sqlx-exec-2.3.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-05 02:31:35.277598 sqlx-exec-2.3.4/
--rw-r--r--   0 summy      (501) staff       (20)    11357 2024-01-23 07:49:56.000000 sqlx-exec-2.3.4/LICENSE
--rw-r--r--   0 summy      (501) staff       (20)     7493 2024-04-05 02:31:35.276209 sqlx-exec-2.3.4/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)     6974 2024-03-29 02:19:13.000000 sqlx-exec-2.3.4/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-05 02:31:35.277887 sqlx-exec-2.3.4/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1299 2024-04-05 02:31:24.000000 sqlx-exec-2.3.4/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-05 02:31:35.261004 sqlx-exec-2.3.4/sqlexec/
--rw-r--r--   0 summy      (501) staff       (20)     1768 2024-03-28 02:42:54.000000 sqlx-exec-2.3.4/sqlexec/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)      637 2024-03-27 13:46:01.000000 sqlx-exec-2.3.4/sqlexec/constant.py
--rw-r--r--   0 summy      (501) staff       (20)     6901 2024-04-05 02:12:59.000000 sqlx-exec-2.3.4/sqlexec/dialect.py
--rw-r--r--   0 summy      (501) staff       (20)    13843 2024-03-28 01:00:25.000000 sqlx-exec-2.3.4/sqlexec/exec.py
--rw-r--r--   0 summy      (501) staff       (20)     1956 2024-03-25 07:14:31.000000 sqlx-exec-2.3.4/sqlexec/loader.py
--rw-r--r--   0 summy      (501) staff       (20)      816 2024-03-27 08:41:08.000000 sqlx-exec-2.3.4/sqlexec/log_support.py
--rw-r--r--   0 summy      (501) staff       (20)     1933 2024-03-27 08:41:08.000000 sqlx-exec-2.3.4/sqlexec/page_exec.py
--rw-r--r--   0 summy      (501) staff       (20)    12121 2024-03-27 08:41:08.000000 sqlx-exec-2.3.4/sqlexec/sql_exec.py
--rw-r--r--   0 summy      (501) staff       (20)     3054 2024-03-28 00:30:18.000000 sqlx-exec-2.3.4/sqlexec/sql_support.py
--rw-r--r--   0 summy      (501) staff       (20)    17485 2024-03-27 08:41:08.000000 sqlx-exec-2.3.4/sqlexec/table_exec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-05 02:31:35.270625 sqlx-exec-2.3.4/sqlx_exec.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     7493 2024-04-05 02:31:35.000000 sqlx-exec-2.3.4/sqlx_exec.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      438 2024-04-05 02:31:35.000000 sqlx-exec-2.3.4/sqlx_exec.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-05 02:31:35.000000 sqlx-exec-2.3.4/sqlx_exec.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-03-27 09:08:34.000000 sqlx-exec-2.3.4/sqlx_exec.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       21 2024-04-05 02:31:35.000000 sqlx-exec-2.3.4/sqlx_exec.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)        8 2024-04-05 02:31:35.000000 sqlx-exec-2.3.4/sqlx_exec.egg-info/top_level.txt
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-05 02:31:35.272552 sqlx-exec-2.3.4/test/
--rw-r--r--   0 summy      (501) staff       (20)      444 2024-03-25 01:37:05.000000 sqlx-exec-2.3.4/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-21 13:17:48.011459 sqlx-exec-2.3.5/
+-rw-r--r--   0 summy      (501) staff       (20)    11357 2024-01-23 07:49:56.000000 sqlx-exec-2.3.5/LICENSE
+-rw-r--r--   0 summy      (501) staff       (20)     7493 2024-04-21 13:17:48.010718 sqlx-exec-2.3.5/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     6974 2024-03-29 02:19:13.000000 sqlx-exec-2.3.5/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-21 13:17:48.011710 sqlx-exec-2.3.5/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1299 2024-04-21 13:17:23.000000 sqlx-exec-2.3.5/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-21 13:17:47.994583 sqlx-exec-2.3.5/sqlexec/
+-rw-r--r--   0 summy      (501) staff       (20)     1780 2024-04-21 11:39:48.000000 sqlx-exec-2.3.5/sqlexec/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)      637 2024-03-27 13:46:01.000000 sqlx-exec-2.3.5/sqlexec/constant.py
+-rw-r--r--   0 summy      (501) staff       (20)     7995 2024-04-08 10:38:09.000000 sqlx-exec-2.3.5/sqlexec/dialect.py
+-rw-r--r--   0 summy      (501) staff       (20)    13878 2024-04-08 10:35:24.000000 sqlx-exec-2.3.5/sqlexec/exec.py
+-rw-r--r--   0 summy      (501) staff       (20)     1956 2024-03-25 07:14:31.000000 sqlx-exec-2.3.5/sqlexec/loader.py
+-rw-r--r--   0 summy      (501) staff       (20)      816 2024-03-27 08:41:08.000000 sqlx-exec-2.3.5/sqlexec/log_support.py
+-rw-r--r--   0 summy      (501) staff       (20)     1933 2024-03-27 08:41:08.000000 sqlx-exec-2.3.5/sqlexec/page_exec.py
+-rw-r--r--   0 summy      (501) staff       (20)    12121 2024-03-27 08:41:08.000000 sqlx-exec-2.3.5/sqlexec/sql_exec.py
+-rw-r--r--   0 summy      (501) staff       (20)     3068 2024-04-08 10:27:42.000000 sqlx-exec-2.3.5/sqlexec/sql_support.py
+-rw-r--r--   0 summy      (501) staff       (20)    18422 2024-04-08 12:17:35.000000 sqlx-exec-2.3.5/sqlexec/table_exec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-21 13:17:48.005950 sqlx-exec-2.3.5/sqlx_exec.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     7493 2024-04-21 13:17:47.000000 sqlx-exec-2.3.5/sqlx_exec.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      438 2024-04-21 13:17:47.000000 sqlx-exec-2.3.5/sqlx_exec.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-21 13:17:47.000000 sqlx-exec-2.3.5/sqlx_exec.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-03-27 09:08:34.000000 sqlx-exec-2.3.5/sqlx_exec.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       21 2024-04-21 13:17:47.000000 sqlx-exec-2.3.5/sqlx_exec.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)        8 2024-04-21 13:17:47.000000 sqlx-exec-2.3.5/sqlx_exec.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-21 13:17:48.006862 sqlx-exec-2.3.5/test/
+-rw-r--r--   0 summy      (501) staff       (20)     1192 2024-04-08 10:07:10.000000 sqlx-exec-2.3.5/test/test.py
```

### Comparing `sqlx-exec-2.3.4/LICENSE` & `sqlx-exec-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.4/PKG-INFO` & `sqlx-exec-2.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 2.3.4
+Version: 2.3.5
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlx-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
 Platform: UNKNOWN
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
```

### Comparing `sqlx-exec-2.3.4/README.rst` & `sqlx-exec-2.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.4/setup.py` & `sqlx-exec-2.3.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions. Support MySQL, PostgreSQL, SQLite etc.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='2.3.4',
+    version='2.3.5',
     install_requires=[
         'sqlx-executor>=1.1.1',
     ],
     url='https://gitee.com/summry/sqlx-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Database', 'Python', 'RDB'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
     },
     include_package_data=True,
-    python_requires='>=3.5',
+    python_requires='>=3.6',
     zip_safe=False
 )
```

### Comparing `sqlx-exec-2.3.4/sqlexec/__init__.py` & `sqlx-exec-2.3.5/sqlexec/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,33 +19,33 @@
     batch_insert,
     batch_execute,
     get,
     select,
     select_one,
     query,
     query_one,
+    select_page,
+    query_page,
+    load,
     do_execute,
     do_save_sql,
     do_save_sql_select_key,
     do_get,
     do_select,
     do_select_one,
     do_query,
     do_query_one,
-    select_page,
-    query_page,
     do_select_page,
     do_query_page,
-    load,
     do_load,
     insert_from_csv,
     insert_from_df,
     insert_from_json,
-    truncate,
-    drop
+    truncate_table,
+    drop_table
 )
 
 from .sql_exec import sql
 from .page_exec import page
 from .table_exec import table
 from .dialect import Dialect
```

### Comparing `sqlx-exec-2.3.4/sqlexec/constant.py` & `sqlx-exec-2.3.5/sqlexec/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.4/sqlexec/dialect.py` & `sqlx-exec-2.3.5/sqlexec/dialect.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
 import re
-from .log_support import logger
 from functools import lru_cache
-from typing import Sequence, Collection
+from typing import Sequence, Collection, Union
 from executor.sql_support import require_limit
 from executor import get, query, select, DBError, Engine
+from .log_support import logger
 from .constant import CACHE_SIZE, LIMIT_1, DEFAULT_KEY_FIELD, MYSQL_COLUMN_SQL, MYSQL_SELECT_KEY, POSTGRES_COLUMN_SQL,\
     SQLITE_SELECT_KEY
 
 
 def get_page_start(page_num: int, page_size: int):
     assert page_num >= 1 and page_size >= 1, "'page_name' and 'page_size' should be higher or equal to 1"
     return (page_num - 1) * page_size
@@ -42,15 +42,20 @@
 
     @staticmethod
     def get_table_columns(table_name: str):
         return '*'
 
     @staticmethod
     def get_truncate_sql(table_name: str):
-        return 'TRUNCATE TABLE %s' % table_name
+        return 'TRUNCATE TABLE %s' % Dialect.get_dialect_str(table_name)
+
+    @staticmethod
+    def get_dialect_str(src: Union[str, int, Collection[str]]):
+        assert isinstance(src, str), 'source must be a string.'
+        return src.strip() if isinstance(src, str) else ','.join([s.strip() for s in src])
 
     @staticmethod
     def get_select_key(*args, **kwargs):
         raise NotImplementedError("Not implement method 'get_select_key', you can use orm snowflake for primary key.")
 
 
 class MySQLDialect(BaseDialect):
@@ -74,16 +79,19 @@
         return get(sql, table_name, LIMIT_1)
 
     @staticmethod
     def get_select_key(*args, **kwargs):
         return MYSQL_SELECT_KEY
 
     @staticmethod
-    def get_truncate_sql(table_name: str):
-        return 'TRUNCATE TABLE `%s`' % table_name
+    def get_dialect_str(src: Union[str, int, Collection[str]]):
+        assert src, 'src is required.'
+        if isinstance(src, str):
+            return _dialect_str(src)
+        return ','.join([_dialect_str(arg) for arg in src])
 
 
 class PostgresDialect(BaseDialect):
 
     @staticmethod
     def get_table_columns(table_name: str):
         sql = MySQLDialect.before_execute(POSTGRES_COLUMN_SQL)
@@ -129,20 +137,20 @@
     @staticmethod
     def get_table_columns(table_name: str):
         sql = Dialect.before_execute('SELECT column_name FROM user_tab_columns WHERE table_name = ?')
         results = select(sql, table_name)
         return ','.join([result[0] for result in results])
 
 
-class SQLiteDialect(BaseDialect):
+class SQLiteDialect(MySQLDialect):
 
     @staticmethod
     def get_table_columns(table_name: str):
-        results = query(f'PRAGMA table_info({table_name})')
-        return ','.join([result['name'] for result in results])
+        results = query(f'PRAGMA table_info(`{table_name}`)')
+        return ','.join(['`{}`'.format(result['name']) for result in results])
 
     @staticmethod
     def get_select_key(*args, **kwargs):
         return SQLITE_SELECT_KEY
 
     @staticmethod
     def before_execute(sql: str):
@@ -197,15 +205,37 @@
 
     @staticmethod
     def get_truncate_sql(table_name: str):
         global _DIALECT
         return _DIALECT.get_truncate_sql(table_name)
 
     @staticmethod
+    def get_drop_sql(table_name: str):
+        global _DIALECT
+        return _DIALECT.get_drop_sql(table_name)
+
+    @staticmethod
     def get_select_key(*args, **kwargs):
         global _DIALECT
         return _DIALECT.get_select_key(*args, **kwargs)
 
     @staticmethod
+    def get_dialect_str(src: Union[str, int, Collection[str]]):
+        global _DIALECT
+        return _DIALECT.get_dialect_str(src)
+
+    @staticmethod
     def curr_engine():
         global _DIALECT
         return _DIALECT.engine
+
+
+def _dialect_str(src: Union[str, int]):
+    assert isinstance(src, str) or isinstance(src, int), 'source must be a string or int.'
+    if isinstance(src, int):
+        return str(src)
+    elif ',' in src:
+        return ','.join(['`{}`'.format(s.strip()) for s in src.split(',')])
+    elif '(' in src:
+        return src.strip()
+    else:
+        return '`{}`'.format(src.strip())
```

### Comparing `sqlx-exec-2.3.4/sqlexec/exec.py` & `sqlx-exec-2.3.5/sqlexec/exec.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,17 +378,15 @@
     elif isinstance(data, Iterable):
         return batch_insert(table_name, data)
     else:
         logger.info("Exec func 'sqlexec.%s' \n\t Table: '%s' insert 0 rows." % ('insert_from_json', table_name))
         return 0
 
 
-def truncate(table_name: str) -> int:
+def truncate_table(table_name: str) -> int:
     """ sqlexec.truncate('person') """
     return _execute(Dialect.get_truncate_sql(table_name))
 
 
-def drop(table_name: str) -> int:
+def drop_table(table_name: str) -> int:
     """ sqlexec.drop('person') """
-    return _execute('DROP TABLE %s' % table_name)
-
-
+    return _execute('DROP TABLE %s' % Dialect.get_dialect_str(table_name))
```

### Comparing `sqlx-exec-2.3.4/sqlexec/loader.py` & `sqlx-exec-2.3.5/sqlexec/loader.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.4/sqlexec/log_support.py` & `sqlx-exec-2.3.5/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.4/sqlexec/page_exec.py` & `sqlx-exec-2.3.5/sqlexec/page_exec.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.4/sqlexec/sql_exec.py` & `sqlx-exec-2.3.5/sqlexec/sql_exec.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.4/sqlexec/sql_support.py` & `sqlx-exec-2.3.5/sqlexec/sql_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,16 @@
 
 def try_mapping(function, sql, *args, **kwargs):
     sql_log(function, sql, *args, **kwargs)
     return get_mapping_sql_args(sql, *args, **kwargs)
 
 
 def get_table_select_sql(table_name: str, where: str, limit: Union[int, Tuple[int], List[int]], *columns):
-    columns = ','.join([col if '(' in col else '{}'.format(col) for col in columns]) if columns else Dialect.get_table_columns(table_name)
-
+    columns = Dialect.get_dialect_str(columns) if columns else Dialect.get_table_columns(table_name)
+    table_name = Dialect.get_dialect_str(table_name)
     if limit:
         if isinstance(limit, int):
             return 'SELECT {} FROM {} {} LIMIT ?'.format(columns, table_name, where)
         elif (isinstance(limit, Tuple) or isinstance(limit, List)) and len(limit) == 2:
             return 'SELECT {} FROM {} {} LIMIT ? OFFSET ?'.format(columns, table_name, where)
         else:
             raise ValueError("The type of the parameter 'limit' must be 'int' or tuple, list, and it length is 2.")
```

### Comparing `sqlx-exec-2.3.4/sqlexec/table_exec.py` & `sqlx-exec-2.3.5/sqlexec/table_exec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-#！/usr/bin/env python3
+# !/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
+from typing import Sequence, Tuple
 from .loader import Loader
 from . import exec, sql_support
+from .dialect import Dialect, Engine
 from .constant import LIMIT_1, SELECT_COUNT
-from typing import Sequence, Tuple
 from .sql_support import get_table_select_sql
 
 
 class TablePageExec:
 
     def __init__(self, table_exec, page_num, page_size):
         self.table_exec = table_exec
@@ -150,15 +151,15 @@
         """
         return self.get(SELECT_COUNT)
 
     def exists(self):
         """
          sqlexec.table('person').where(name='李四').exists()
         """
-        return self.get('1') == 1
+        return self.get(1) == 1
 
     def select(self, *columns):
         """
         sqlexec.table('person').where(name='李四').select('name', 'age')
         """
         sql, args = self.get_select_sql_args(*columns)
         return self.exec.do_select(sql, *args)
@@ -185,26 +186,32 @@
         return self.exec.do_query_one(sql, *args, LIMIT_1)
 
     def delete(self):
         """
         sqlexec.table('person').where(name='李四').delete()
         """
         where, args, _ = get_where_arg_limit(**self.where_condition)
-        sql = 'DELETE FROM %s %s' % (self.table, where)
+        sql = 'DELETE FROM %s %s' % (Dialect.get_dialect_str(self.table), where)
+        if Dialect.curr_engine() in (Engine.MYSQL, Engine.SQLITE):
+            sql = '{} LIMIT ?'.format(sql)
+            args = [*args, LIMIT_1]
         return self.exec.do_execute(sql, *args)
 
     def update(self, **kwargs):
         """
         sqlexec.table('person').where(name='张三').update(name='李四', age=45)
         """
         where, args, _ = get_where_arg_limit(**self.where_condition)
         update_cols, update_args = zip(*kwargs.items())
         args = [*update_args, *args]
-        update_cols = ', '.join(['{} = ?'.format(col) for col in update_cols])
-        sql = 'UPDATE {} SET {} {}'.format(self.table, update_cols, where)
+        update_cols = ', '.join(['{} = ?'.format(Dialect.get_dialect_str(col)) for col in update_cols])
+        sql = 'UPDATE {} SET {} {}'.format(Dialect.get_dialect_str(self.table), update_cols, where)
+        if Dialect.curr_engine() in (Engine.MYSQL, Engine.SQLITE):
+            sql = '{} LIMIT ?'.format(sql)
+            args = [*args, LIMIT_1]
         return self.exec.do_execute(sql, *args)
 
     def load(self, *columns) -> Loader:
         """
         sqlexec.table('person').where(name='张三').load('name', 'age')
         """
         sql, args = self.get_select_sql_args(*columns)
@@ -227,14 +234,15 @@
         return sql, args
 
     def get_select_one_sql_args(self, *columns):
         where, args, _ = get_where_arg_limit(**self.where_condition)
         sql = get_table_select_sql(self.table, where, LIMIT_1, *columns)
         return sql, args
 
+
 class ColumnExec:
 
     def __init__(self, table_exec, *columns):
         self.table_exec = table_exec
         self.columns = columns
 
     def insert(self, *args):
@@ -448,56 +456,56 @@
     table_name = table_name.strip()
     assert table_name, "Parameter 'table' must not be none"
     return TableExec(exec, table_name)
 
 
 def get_condition_arg(k: str, v: object):
     if k.endswith("__eq"):
-        return "{} = ?".format(k[:-4]), v
+        return "{} = ?".format(Dialect.get_dialect_str(k[:-4])), v
     if k.endswith("__ne"):
-        return "{} != ?".format(k[:-4]), v
+        return "{} != ?".format(Dialect.get_dialect_str(k[:-4])), v
     if k.endswith("__gt"):
-        return "{} > ?".format(k[:-4]), v
+        return "{} > ?".format(Dialect.get_dialect_str(k[:-4])), v
     if k.endswith("__lt"):
-        return "{} < ?".format(k[:-4]), v
+        return "{} < ?".format(Dialect.get_dialect_str(k[:-4])), v
     if k.endswith("__ge"):
-        return "{} >= ?".format(k[:-4]), v
+        return "{} >= ?".format(Dialect.get_dialect_str(k[:-4])), v
     if k.endswith("__gte"):
-        return "{} >= ?".format(k[:-5]), v
+        return "{} >= ?".format(Dialect.get_dialect_str(k[:-5])), v
     if k.endswith("__le"):
-        return "{} <= ?".format(k[:-4]), v
+        return "{} <= ?".format(Dialect.get_dialect_str(k[:-4])), v
     if k.endswith("__lte"):
-        return "{} <= ?".format(k[:-5]), v
+        return "{} <= ?".format(Dialect.get_dialect_str(k[:-5])), v
     if k.endswith("__isnull"):
-        return "{} is {}".format(k[:-8], 'null' if v else 'not null'), None
+        return "{} is {}".format(Dialect.get_dialect_str(k[:-8]), 'null' if v else 'not null'), None
     if k.endswith("__in") and isinstance(v, Sequence) and not isinstance(v, str):
-        return "{} in({})".format(k[:-4], ','.join(['?' for _ in v])), v
+        return "{} in({})".format(Dialect.get_dialect_str(k[:-4]), ','.join(['?' for _ in v])), v
     if k.endswith("__in"):
-        return "{} in({})".format(k[:-4], '?'), v
+        return "{} in({})".format(Dialect.get_dialect_str(k[:-4]), '?'), v
     if k.endswith("__not_in") and isinstance(v, Sequence) and not isinstance(v, str):
-        return "{} not in({})".format(k[:-8], ','.join(['?' for _ in v])), v
+        return "{} not in({})".format(Dialect.get_dialect_str(k[:-8]), ','.join(['?' for _ in v])), v
     if k.endswith("__not_in"):
-        return "{} not in({})".format(k[:-8], '?'), v
+        return "{} not in({})".format(Dialect.get_dialect_str(k[:-8]), '?'), v
     if k.endswith("__like"):
-        return "{} like ?".format(k[:-6], '?'), v
+        return "{} like ?".format(Dialect.get_dialect_str(k[:-6])), '%{}%'.format(v)
     if k.endswith("__startswith"):
-        return "{} like ?".format(k[:-12]), '{}%'.format(v)
+        return "{} like ?".format(Dialect.get_dialect_str(k[:-12])), '{}%'.format(v)
     if k.endswith("__endswith"):
-        return "{} like ?".format(k[:-10]), '%{}'.format(v)
+        return "{} like ?".format(Dialect.get_dialect_str(k[:-10])), '%{}'.format(v)
     if k.endswith("__contains"):
-        return "{} like ?".format(k[:-10]), '%{}%'.format(v)
+        return "{} like ?".format(Dialect.get_dialect_str(k[:-10])), '%{}%'.format(v)
     if k.endswith("__range") and isinstance(v, Sequence) and 2 == len(v) and not isinstance(v, str):
         col = k[:-7]
-        return "{} >= ? and {} <= ?".format(col, col), v
+        return "{} >= ? and {} <= ?".format(Dialect.get_dialect_str(col), Dialect.get_dialect_str(col)), v
     if k.endswith("__between") and isinstance(v, Sequence) and 2 == len(v) and not isinstance(v, str):
-        return "{} between ? and ?".format(k[:-9]), v
+        return "{} between ? and ?".format(Dialect.get_dialect_str(k[:-9])), v
     if k.endswith("__range") or k.endswith("__between"):
         return ValueError("Must is instance of Sequence with length 2 when use range or between statement")
 
-    return "{} = ?".format(k), v
+    return "{} = ?".format(Dialect.get_dialect_str(k)), v
 
 
 def get_where_arg_limit(**kwargs):
     where, args, limit = '', [], 0
     if 'limit' in kwargs:
         limit = kwargs.pop('limit')
```

### Comparing `sqlx-exec-2.3.4/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-2.3.5/sqlx_exec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 2.3.4
+Version: 2.3.5
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlx-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
 Platform: UNKNOWN
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
```


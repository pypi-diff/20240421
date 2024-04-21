# Comparing `tmp/sqlx-orm-0.0.3.tar.gz` & `tmp/sqlx-orm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlx-orm-0.0.3.tar", last modified: Fri Apr  5 02:42:34 2024, max compression
+gzip compressed data, was "sqlx-orm-0.0.5.tar", last modified: Sun Apr 21 13:18:37 2024, max compression
```

## Comparing `sqlx-orm-0.0.3.tar` & `sqlx-orm-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-05 02:42:34.337436 sqlx-orm-0.0.3/
--rw-r--r--   0 summy      (501) staff       (20)     2145 2024-04-05 02:42:34.336516 sqlx-orm-0.0.3/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)     1733 2024-04-04 10:08:32.000000 sqlx-orm-0.0.3/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-05 02:42:34.323202 sqlx-orm-0.0.3/orm/
--rw-r--r--   0 summy      (501) staff       (20)      288 2024-04-04 08:43:34.000000 sqlx-orm-0.0.3/orm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     1036 2024-04-05 02:16:39.000000 sqlx-orm-0.0.3/orm/constant.py
--rw-r--r--   0 summy      (501) staff       (20)     2344 2024-04-05 02:37:00.000000 sqlx-orm-0.0.3/orm/log_support.py
--rw-r--r--   0 summy      (501) staff       (20)    29422 2024-04-05 02:30:25.000000 sqlx-orm-0.0.3/orm/orm.py
--rw-r--r--   0 summy      (501) staff       (20)    12045 2024-04-05 02:41:28.000000 sqlx-orm-0.0.3/orm/orm_support.py
--rw-r--r--   0 summy      (501) staff       (20)     2603 2024-04-04 01:12:05.000000 sqlx-orm-0.0.3/orm/snowflake.py
--rw-r--r--   0 summy      (501) staff       (20)      128 2024-04-04 01:12:05.000000 sqlx-orm-0.0.3/orm/support.py
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-05 02:42:34.338098 sqlx-orm-0.0.3/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1209 2024-04-05 02:37:00.000000 sqlx-orm-0.0.3/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-05 02:42:34.334054 sqlx-orm-0.0.3/sqlx_orm.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     2145 2024-04-05 02:42:34.000000 sqlx-orm-0.0.3/sqlx_orm.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      322 2024-04-05 02:42:34.000000 sqlx-orm-0.0.3/sqlx_orm.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-05 02:42:34.000000 sqlx-orm-0.0.3/sqlx_orm.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-04 10:07:39.000000 sqlx-orm-0.0.3/sqlx_orm.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       17 2024-04-05 02:42:34.000000 sqlx-orm-0.0.3/sqlx_orm.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)        4 2024-04-05 02:42:34.000000 sqlx-orm-0.0.3/sqlx_orm.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-21 13:18:37.097654 sqlx-orm-0.0.5/
+-rw-r--r--   0 summy      (501) staff       (20)     2145 2024-04-21 13:18:37.096895 sqlx-orm-0.0.5/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     1733 2024-04-04 10:08:32.000000 sqlx-orm-0.0.5/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-21 13:18:37.083112 sqlx-orm-0.0.5/orm/
+-rw-r--r--   0 summy      (501) staff       (20)      288 2024-04-04 08:43:34.000000 sqlx-orm-0.0.5/orm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     1036 2024-04-05 02:16:39.000000 sqlx-orm-0.0.5/orm/constant.py
+-rw-r--r--   0 summy      (501) staff       (20)     2344 2024-04-05 02:37:00.000000 sqlx-orm-0.0.5/orm/log_support.py
+-rw-r--r--   0 summy      (501) staff       (20)    29313 2024-04-21 13:10:06.000000 sqlx-orm-0.0.5/orm/orm.py
+-rw-r--r--   0 summy      (501) staff       (20)    14014 2024-04-21 13:02:31.000000 sqlx-orm-0.0.5/orm/orm_support.py
+-rw-r--r--   0 summy      (501) staff       (20)     2603 2024-04-04 01:12:05.000000 sqlx-orm-0.0.5/orm/snowflake.py
+-rw-r--r--   0 summy      (501) staff       (20)      128 2024-04-04 01:12:05.000000 sqlx-orm-0.0.5/orm/support.py
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-21 13:18:37.097938 sqlx-orm-0.0.5/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1209 2024-04-21 13:18:31.000000 sqlx-orm-0.0.5/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-21 13:18:37.095886 sqlx-orm-0.0.5/sqlx_orm.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     2145 2024-04-21 13:18:37.000000 sqlx-orm-0.0.5/sqlx_orm.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      322 2024-04-21 13:18:37.000000 sqlx-orm-0.0.5/sqlx_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-21 13:18:37.000000 sqlx-orm-0.0.5/sqlx_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-04 10:07:39.000000 sqlx-orm-0.0.5/sqlx_orm.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       17 2024-04-21 13:18:37.000000 sqlx-orm-0.0.5/sqlx_orm.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)        4 2024-04-21 13:18:37.000000 sqlx-orm-0.0.5/sqlx_orm.egg-info/top_level.txt
```

### Comparing `sqlx-orm-0.0.3/PKG-INFO` & `sqlx-orm-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sqlx-orm
-Version: 0.0.3
+Version: 0.0.5
 Summary: A single table ORM framework for python. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlx-orm
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
 Platform: UNKNOWN
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
```

### Comparing `sqlx-orm-0.0.3/README.rst` & `sqlx-orm-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-orm-0.0.3/orm/constant.py` & `sqlx-orm-0.0.5/orm/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-orm-0.0.3/orm/log_support.py` & `sqlx-orm-0.0.5/orm/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-orm-0.0.3/orm/orm.py` & `sqlx-orm-0.0.5/orm/orm.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             self.update_by = update_by
             self.update_time = update_time
             self.del_flag = del_flag
             self.name = name
             self.age = age
 
     then you can use like follow:
-        init_db(person='xxx', password='xxx', database='xxx', host='xxx', ...)  # or dbx.init_db(...) init db first,
+        orm.init(person='xxx', password='xxx', database='xxx', host='xxx', ...)  # or db.init(...) init db first,
         person = Person(name='张三', age=55)
         effect_rowcount = person.persist()
         id = person.inst_save()
     """
 
     def __str__(self):
         return str({k: v for k, v in self.__dict__.items() if not k.startswith("__")})
@@ -205,20 +205,20 @@
         if key_strategy == KeyStrategy.SNOWFLAKE:
             kwargs[key] = get_snowflake_id()
             db.insert(table, **kwargs)
             return kwargs[key]
         else:
             select_key = cls._get_select_key()
             if not select_key:
+                keq_seq = cls._get_key_seq()
                 try:
-                    select_key = Dialect.get_select_key(keq_seq=cls._get_key_seq(), table=table, key=key)
+                    select_key = Dialect.get_select_key(keq_seq=keq_seq, table=table, key=key)
                 except NotImplementedError:
-                    if Dialect.curr_engine() == db.Engine.POSTGRESQL:
-                        raise DBError(f"Expect 'key_seq' or 'select_key'. you can set it in model class with '__key_seq__' or '__select_key__'.")
-                    raise DBError(f"Expect 'select_key'. you can set it in model class with '__select_key__'.")
+                    raise DBError("Expect 'select_key'. you can set it in model class with '__select_key__'. "
+                                  "You can also set primary key sequence with '__key_seq__' for PostgreSQL.'")
             return db.save_select_key(select_key, table, **kwargs)
 
     @classmethod
     def create(cls, **kwargs):
         """
         person = Person.create(name='张三', age=20)
         :return: Instance object
@@ -232,21 +232,18 @@
     def update_by_id(cls, _id: Union[int, str], **kwargs):
         """
         rowcount = Person.update_by_id(id=1, name='王五')
         return: Effect rowcount
         """
         log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d, kwargs: %s" % ('update_by_id', cls.__name__, _id, kwargs))
         assert kwargs, 'Must set update kv'
-        key = cls._get_key()
-        where = '%s = ?' % key
-        cols, args = zip(*kwargs.items())
-        sql, update_time_arg = cls._update_sql(where, *cols)
-        if update_time_arg:
-            args = [*args, update_time_arg]
-        return db.do_execute(sql, *args, _id)
+        key, table_name = cls._get_key_and_table()
+        where_kwargs = {key: _id}
+        kwargs = cls._update_time(**kwargs)
+        db.table(table_name).where(**where_kwargs).update(**kwargs)
 
     @classmethod
     def logical_delete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
         """
         Logic delete only update the del flag
         rowcount = Person.delete_by_id(id=1, update_by=100)
         return: Effect rowcount
@@ -300,16 +297,16 @@
         """
         Physical delete
         rowcount = Person.delete_by_id(id=1)
         return: Effect rowcount
         """
         log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d" % ('delete_by_id', cls.__name__, _id))
         key, table = cls._get_key_and_table()
-        sql = 'DELETE FROM %s WHERE %s = ?' % (table, key)
-        return db.do_execute(sql, _id)
+        where_kwargs = {key: _id}
+        return db.table(table).where(**where_kwargs).delete()
 
     @classmethod
     def delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], batch_size=128):
         """
         Batch physical delete, they will be executed in batches if there are too many
         rowcount = Person.delete_by_ids(id=[1,2])
         return: Effect rowcount
@@ -330,18 +327,17 @@
     @classmethod
     def do_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]]):
         """
         Batch physical delete, please use delete_by_ids if there are too many
         rowcount = Person.do_delete_by_ids(id=[1,2])
         return: Effect rowcount
         """
-        ids_size = len(ids)
         key, table = cls._get_key_and_table()
-        sql = 'DELETE FROM {} WHERE {} in ({})'.format(table, key, ','.join(['?' for _ in range(ids_size)]))
-        return db.do_execute(sql, *ids)
+        where_kwargs = {'{}__in'.format(key): ids}
+        return db.table(table).where(**where_kwargs).delete()
 
     @classmethod
     def batch_insert(cls, *args):
         """
         Batch insert
         rowcount = Person.batch_insert([{'name': '张三', 'age': 55},{'name': '李四', 'age': 66}])
         :param args: All number must have same key.
@@ -368,15 +364,21 @@
         table = cls.get_table()
         return db.table(table).where(**kwargs).count()
 
     @classmethod
     def exists(cls, **kwargs):
         log_support.orm_count_log('exists', cls.__name__, **kwargs)
         table = cls.get_table()
-        return db.table(table).where( **kwargs).exists()
+        return db.table(table).where(**kwargs).exists()
+
+    @classmethod
+    def exists_by_id(cls, _id: Union[int, str]):
+        key = cls._get_key()
+        kwargs = {key: _id}
+        return cls.exists(**kwargs)
 
     @classmethod
     def find(cls, *fields, **kwargs):
         """
         Return list(object) or empty list if no result.
         persons = Person.find('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
@@ -446,34 +448,31 @@
         Return one row(dict) or None if no result.
         person = Person.query_by_id(1, 'id', 'name', 'age')
         :param _id: key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_id_log('query_by_id', cls.__name__, _id, *fields)
         key, table = cls._get_key_and_table()
-        where = 'WHERE {} = ?'.format(key)
-        sql = orm_support.get_table_select_sql(table, where, LIMIT_1, *fields)
-        return db.do_query_one(sql, _id, LIMIT_1)
+        kwargs = {key: _id}
+        return db.table(table).columns(*fields).where(**kwargs).query_one()
 
     @classmethod
     def query_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
         persons = Person.query_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_ids_log('query_by_ids', cls.__name__, ids, *fields)
-        ids_size = len(ids)
-        assert ids_size > 0, 'ids must not be empty.'
+        assert len(ids) > 0, 'ids must not be empty.'
 
         key, table = cls._get_key_and_table()
-        where = 'WHERE {} in ({})'.format(key, ','.join(['?' for _ in range(ids_size)]))
-        sql = orm_support.get_table_select_sql(table, where, ids_size, *fields)
-        return db.do_query(sql, *ids, ids_size)
+        kwargs = {'{}__in'.format(key): ids}
+        return db.table(table).columns(*fields).where(**kwargs).query()
 
     @classmethod
     def select(cls, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = Person.select('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
@@ -499,34 +498,31 @@
         Return one row(dict) or None if no result.
         row = Person.select_by_id(1, 'id', 'name', 'age')
         :param _id: key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_id_log('select_by_id', cls.__name__, _id, *fields)
         key, table = cls._get_key_and_table()
-        where = 'WHERE {} = ?'.format(key)
-        sql = orm_support.get_table_select_sql(table, where, LIMIT_1, *fields)
-        return db.do_select_one(sql, _id, LIMIT_1)
+        kwargs = {key: _id}
+        return db.table(table).columns(*fields).where(**kwargs).select_one()
 
     @classmethod
     def select_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
         rows = Person.select_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_ids_log('select_by_ids', cls.__name__, ids, *fields)
-        ids_size = len(ids)
-        assert ids_size > 0, 'ids must not be empty.'
+        assert len(ids) > 0, 'ids must not be empty.'
 
         key, table = cls._get_key_and_table()
-        where = 'WHERE {} in ({})'.format(key, ','.join(['?' for _ in range(ids_size)]))
-        sql = orm_support.get_table_select_sql(table, where, ids_size, *fields)
-        return db.do_select(sql, *ids, ids_size)
+        kwargs = {'{}__in'.format(key): ids}
+        return db.table(table).columns(*fields).where(**kwargs).select()
 
     @classmethod
     def find_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(object) or empty list if no result.
         persons = Person.find_page(1, 10, 'name', 'age', name='张三', age=55)
         :param page_num: page number
@@ -568,16 +564,16 @@
         return orm_support.FieldExec(cls, *fields)
 
     @classmethod
     def where(cls, **kwargs) -> orm_support.WhereExec:
         return orm_support.WhereExec(cls, **kwargs)
 
     @classmethod
-    def page(cls, page_num=1, page_size=10) -> orm_support.OrmPage:
-        return cls.where().page(page_num, page_size)
+    def page(cls, page_num=1, page_size=10) -> orm_support.PageExec:
+        return orm_support.PageExec(cls, page_num, page_size)
 
     @classmethod
     def to_obj(cls, **kwargs):
         model = cls.__new__(cls)
         model.__dict__.update(**kwargs)
         return model
 
@@ -692,23 +688,31 @@
 
     @classmethod
     def _get_del_flag_field(cls):
         assert hasattr(cls, DEL_FLAG), "%s not set attribute '%s'" % (cls.__name__, DEL_FLAG)
         return cls.__del_flag__
 
     @classmethod
+    def _update_time(cls, **kwargs):
+        update_time_field = cls._get_update_time_field()
+        if update_time_field is not None and update_time_field not in kwargs:
+            kwargs[update_time_field] = datetime.now()
+        return kwargs
+
+    @classmethod
     def _update_sql(cls, where, *update_fields):
         update_time_arg = None
         table = cls.get_table()
+        table = Dialect.get_dialect_str(table)
         update_time_field = cls._get_update_time_field()
         if update_time_field is not None and update_time_field not in update_fields:
             update_fields = [*update_fields, update_time_field]
             update_time_arg = datetime.now()
 
-        update_fields = ', '.join(['{} = ?'.format(col) for col in update_fields])
+        update_fields = ', '.join(['{} = ?'.format(Dialect.get_dialect_str(col)) for col in update_fields])
         return 'UPDATE {} SET {} WHERE {}'.format(table, update_fields, where), update_time_arg
 
     @classmethod
     def _where_sql(cls, where: str):
         low_where = where.strip().lower()
         if low_where.startswith('where'):
             table = cls.get_table()
```

### Comparing `sqlx-orm-0.0.3/orm/orm_support.py` & `sqlx-orm-0.0.5/orm/orm_support.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,144 @@
 from sqlexec.sql_support import get_table_select_sql
 from typing import Sequence, Union, List, Tuple
 from sqlexec.table_exec import get_condition_arg, get_where_arg_limit
 
 
+class FieldWherePageExec:
+    def __init__(self, field_where_exec, page_num, page_size):
+        self.field_where_exec = field_where_exec
+        self.page_num = page_num
+        self.page_size = page_size
+
+    def find(self):
+        return self.field_where_exec.find_page(self.page_num, self.page_size)
+
+    def query(self):
+        return self.field_where_exec.query_page(self.page_num, self.page_size)
+
+    def select(self):
+        return self.field_where_exec.select_page(self.page_num, self.page_size)
+
+
+class FieldWhereExec:
+    def __init__(self, field_exec, **kwargs):
+        self.field_exec = field_exec
+        self.kwargs = kwargs
+
+    def find(self):
+        """
+        Return list(object) or empty list if no result.
+        persons = Person.fields('id', 'name', 'age').where(name='张三', age=55).find()
+        """
+        return self.field_exec.find(**self.kwargs)
+
+    def find_one(self):
+        """
+        Return unique result(object) or None if no result.
+        person = Person.fields('id', 'name', 'age').where(name='张三', age=55).find_one()
+        """
+        return self.field_exec.find_one(**self.kwargs)
+
+    def query(self):
+        """
+        Return list(dict) or empty list if no result.
+        persons = Person.fields('id', 'name', 'age').where(name='张三', age=55).query()
+        """
+        return self.field_exec.query(**self.kwargs)
+
+    def query_one(self):
+        """
+        Return unique result(dict) or None if no result.
+        persons = Person.fields('id', 'name', 'age').where(name='张三', age=55).query_one()
+        """
+        return self.field_exec.query_one(**self.kwargs)
+
+    def select(self):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.fields('id', 'name', 'age').where(name='张三', age=55).select()
+        """
+        return self.field_exec.select(**self.kwargs)
+
+    def select_one(self):
+        """
+        Return unique result(tuple) or None if no result.
+        row = Person.fields('id', 'name', 'age').where(name='张三', age=55).select_one()
+        """
+        return self.field_exec.select_one(**self.kwargs)
+
+    def find_page(self, page_num=1, page_size=10):
+        """
+        Return list(object) or empty list if no result.
+        persons = Person.fields('id', 'name', 'age').where(name='张三', age=55).find_page(1, 10)
+        :param page_num: page number
+        :param page_size: page size
+        """
+        return self.field_exec.find_page(page_num, page_size, **self.kwargs)
+
+    def query_page(self, page_num=1, page_size=10):
+        """
+        Return list(dict) or empty list if no result.
+        persons = Person.fields('id', 'name', 'age').where(name='张三', age=55).query_page(1, 10)
+        :param page_num: page number
+        :param page_size: page size
+        """
+        return self.field_exec.query_page(page_num, page_size, **self.kwargs)
+
+    def select_page(self, page_num=1, page_size=10):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.fields('id', 'name', 'age').where(name='张三', age=55).select_page(1, 10)
+        :param page_num: page number
+        :param page_size: page size
+        """
+        return self.field_exec.select_page(page_num, page_size, **self.kwargs)
+
+    def page(self, page_num=1, page_size=10) -> FieldWherePageExec:
+        return FieldWherePageExec(self, page_num, page_size)
+
+
+class FieldPageExec:
+    def __init__(self, field_exec, page_num=1, page_size=10):
+        self.field_exec = field_exec
+        self.page_num = page_num
+        self.page_size = page_size
+
+    def find(self, **kwargs):
+        return self.field_exec.find_page(self.page_num, self.page_size, **kwargs)
+
+    def query(self, **kwargs):
+        return self.field_exec.query_page(self.page_num, self.page_size, **kwargs)
+
+    def select(self, **kwargs):
+        return self.field_exec.select_page(self.page_num, self.page_size, **kwargs)
+
+    def where(self, **kwargs) -> FieldWherePageExec:
+        return FieldWherePageExec(FieldWhereExec(self.field_exec, **kwargs), self.page_num, self.page_size)
+
+
 class FieldExec:
     def __init__(self, cls, *fields):
         self.cls = cls
         self.fields = fields
 
-    def where(self, **kwargs):
-        return WhereExec(self.cls, *self.fields, **kwargs)
-
-    def page(self, page_num=1, page_size=10):
-        return OrmPage(self.where(), page_num, page_size)
-
     def find(self, **kwargs):
         """
         Return list(object) or empty list if no result.
         persons = Person.fields('id', 'name', 'age').find(name='张三', age=55)
         """
         return self.cls.find(*self.fields, **kwargs)
 
     def find_one(self, **kwargs):
         """
         Return unique result(object) or None if no result.
         person = Person.fields('id', 'name', 'age').find_one(name='张三', age=55)
         """
         return self.cls.find_one(*self.fields, **kwargs)
 
-    # def find_by(self, where: str, *args, **kwargs):
-    #     """
-    #     Return list(dict) or empty list if no result.
-    #     rows = Person.fields('id', 'name', 'age').find_by('where name=?', '李四')
-    #     """
-    #     return [self.cls.to_obj(**d) for d in self.query_by(where, *args, **kwargs)]
-
     def find_by_id(self, _id: Union[int, str]):
         """
         Return one class object or None if no result.
         person = Person.fields('id', 'name', 'age').find_by_id(1)
         :param _id: key
         """
         return self.cls.find_by_id(_id, *self.fields)
@@ -61,22 +161,14 @@
     def query_one(self, **kwargs):
         """
         Return unique result(dict) or None if no result.
         persons = Person.fields('id', 'name', 'age').query_one(name='张三', age=55)
         """
         return self.cls.query_one(*self.fields, **kwargs)
 
-    # def query_by(self, where: str, *args, **kwargs):
-    #     """
-    #     Return list(dict) or empty list if no result.
-    #     rows = Person.fields('id', 'name', 'age').query_by('where name=?', '李四')
-    #     """
-    #     sql, args = self._get_by_sql_args(where, *args, **kwargs)
-    #     return do_query(sql, *args)
-
     def query_by_id(self, _id: Union[int, str]):
         """
         Return one row(dict) or None if no result.
         person = Person.fields('id', 'name', 'age').query_by_id(1)
         :param _id: key
         """
         return self.cls.query_by_id(_id, *self.fields)
@@ -99,23 +191,14 @@
     def select_one(self, **kwargs):
         """
         Return unique result(tuple) or None if no result.
         row = Person.fields('id', 'name', 'age').select_one(name='张三', age=55)
         """
         return self.cls.select_one(*self.fields, **kwargs)
 
-    # def select_by(self, where: str, *args, **kwargs):
-    #     """
-    #     Return list(dict) or empty list if no result.
-    #     rows = Person.select_by_where('where name=?', '李四')
-    #     """
-    #     assert where and where.strip().lower().startswith('where'), "Parameter 'where' must startswith 'WHERE'"
-    #     sql, args = self._get_by_sql_args(where, *args, **kwargs)
-    #     return do_select(sql, *args)
-
     def select_by_id(self, _id: Union[int, str]):
         """
         Return one row(dict) or None if no result.
         row = Person.fields('id', 'name', 'age').select_by_id(1)
         :param _id: key
         """
         return self.cls.select_by_id(_id, *self.fields)
@@ -134,173 +217,174 @@
         Return list(object) or empty list if no result.
         persons = Person.fields('id', 'name', 'age').find_page(1, 10, name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         """
         return self.cls.find_page(page_num, page_size, *self.fields, **kwargs)
 
-    # def find_page_by(self, page_num: int, page_size: int, where: str, *args, **kwargs):
-    #     """
-    #     Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
-    #     rows = Person.find_by_page(1, 10, 'where name=?', '李四')
-    #     """
-    #     return [self.cls.to_obj(**d) for d in self.query_page_by(page_num, page_size, where, *args, **kwargs)]
-
     def query_page(self, page_num=1, page_size=10, **kwargs):
         """
         Return list(dict) or empty list if no result.
         persons = Person.fields('id', 'name', 'age').query_page(1, 10, name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         """
         return self.cls.query_page(page_num, page_size, *self.fields, **kwargs)
 
-    # def query_page_by(self, page_num: int, page_size: int, where: str, *args, **kwargs):
-    #     """
-    #     Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
-    #     rows = Person.fields('id', 'name', 'age').query_by_page(1, 10, 'where name=?', '李四')
-    #     """
-    #     assert where and where.strip().lower().startswith('where'), "Parameter 'where' must startswith 'WHERE'"
-    #     sql, args = self._get_by_sql_args(where, *args, **kwargs)
-    #     return do_query_page(sql, page_num, page_size, *args)
-
     def select_page(self, page_num=1, page_size=10, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = Person.fields('id', 'name', 'age').select_page(1, 10, name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         """
         return self.cls.select_page(page_num, page_size, *self.fields, **kwargs)
 
-    # def select_page_by(self, page_num: int, page_size: int, where: str, *args, **kwargs):
-    #     """
-    #     Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
-    #     rows = Person.fields('id', 'name', 'age').select_by_page(1, 10, 'where name=?', '李四')
-    #     """
-    #     assert where and where.strip().lower().startswith('where'), "Parameter 'where' must startswith 'WHERE'"
-    #     sql, args = self._get_by_sql_args(where, *args, **kwargs)
-    #     return do_select_page(sql, page_num, page_size, *args)
+    def where(self, **kwargs) -> FieldWhereExec:
+        return FieldWhereExec(self, **kwargs)
 
+    def page(self, page_num=1, page_size=10) -> FieldPageExec:
+        return FieldPageExec(self, page_num, page_size)
 
-class WhereExec:
-    def __init__(self, cls, *fields, **kwargs):
-        self.cls = cls
-        self._fields = fields
-        self.kwargs = kwargs
 
-    def fields(self, *fields):
-        self._fields = fields
-        return self
+class WherePageExec:
+    def __init__(self, where_exec, page_num=1, page_size=10):
+        self.where_exec = where_exec
+        self.page_num = page_num
+        self.page_size = page_size
 
-    def where(self, **kwargs):
-        self.kwargs = kwargs
-        return self
+    def select(self, *fields):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.where(name='张三', age=55).page(1, 10).select()
+        """
+        return self.where_exec.select_page(self.page_num, self.page_size, *fields)
+
+    def query(self, *fields):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.where(name='张三', age=55).page(1, 10).query()
+        """
+        return self.where_exec.query_page(self.page_num, self.page_size, *fields)
+
+    def find(self, *fields):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.where(name='张三', age=55).page(1, 10).find()
+        """
+        return self.where_exec.find_page(self.page_num, self.page_size, *fields)
 
-    def page(self, page_num=1, page_size=10):
-        return OrmPage(self, page_num, page_size)
+    def fields(self, *fields) -> FieldWherePageExec:
+        return FieldWherePageExec(FieldWhereExec(FieldExec(self.where_exec.cls, *fields), **self.where_exec.kwargs), self.page_num, self.page_size)
+
+
+class WhereExec:
+    def __init__(self, cls, **kwargs):
+        self.cls = cls
+        self.kwargs = kwargs
 
     def delete(self):
         """
         Physical delete
-        rowcount = Person.delete_by('where name=? and age=?', '张三', 55)
+        rowcount = Person.where(name='张三', age=55).delete()
         return: Effect rowcount
         """
         return self.cls.delete(**self.kwargs)
 
     def count(self):
         """
-        Automatically add 'limit ?' where if not.
-        count = Person.count_by('where name=?', '李四')
+        count = Person.where(name='张三', age=55).count()
         """
         return self.cls.count(**self.kwargs)
 
     def exists(self):
+        """
+        flag = Person.where(name='张三', age=55).exists()
+        """
         return self.cls.exists(**self.kwargs)
 
-    def select(self):
+    def select(self, *fields):
         """
         Return list(dict) or empty list if no result.
-        rows = Person.where('where name=?').select('李四')
+        rows = Person.where(name='张三', age=55).select()
         """
-        return self.cls.select(*self._fields, **self.kwargs)
+        return self.cls.select(*fields, **self.kwargs)
 
-    def query(self):
+    def query(self, *fields):
         """
         Return list(dict) or empty list if no result.
-        rows = Person.where('where name=?').query('李四')
+        rows = Person.where(name='张三', age=55).query()
         """
-        return self.cls.query(*self._fields, **self.kwargs)
+        return self.cls.query(*fields, **self.kwargs)
 
-    def find(self):
+    def find(self, *fields):
         """
         Return list(dict) or empty list if no result.
-        rows = Person.where('where name=?').find('李四')
+        rows = Person.where(name='张三', age=55).find()
         """
-        return [self.cls.to_obj(**d) for d in self.query(*self._fields, **self.kwargs)]
+        return self.cls.find(*fields, **self.kwargs)
 
-    def select_page(self, page_num=1, page_size=10):
+    def select_page(self, page_num=1, page_size=10, *fields):
         """
         Return list(dict) or empty list if no result.
-        rows = Person.where('where name=?').select('李四')
+        rows = Person.where(name='张三', age=55).select_page()
         """
-        return self.cls.select_page(*self._fields, **self.kwargs)
+        return self.cls.select_page(page_num, page_size, *fields, **self.kwargs)
 
-    def query_page(self, page_num=1, page_size=10):
+    def query_page(self, page_num=1, page_size=10, *fields):
         """
         Return list(dict) or empty list if no result.
-        rows = Person.where('where name=?').query('李四')
+        rows = Person.where(name='张三', age=55).query_page()
         """
-        return self.cls.query_page(*self._fields, **self.kwargs)
+        return self.cls.query_page(page_num, page_size, *fields, **self.kwargs)
 
-    def find_page(self, page_num=1, page_size=10):
+    def find_page(self, page_num=1, page_size=10, *fields):
         """
         Return list(dict) or empty list if no result.
-        rows = Person.where('where name=?').find('李四')
+        rows = Person.where(name='张三', age=55).find_page()
         """
-        return [self.cls.to_obj(**d) for d in self.query_page(page_num, page_size)]
+        return self.cls.find_page(page_num, page_size, *fields, **self.kwargs)
 
+    def fields(self, *fields) -> FieldWhereExec:
+        return FieldWhereExec(FieldExec(self.cls, *fields), **self.kwargs)
 
-class OrmPage:
+    def page(self, page_num=1, page_size=10) -> WherePageExec:
+        return WherePageExec(self, page_num, page_size)
+
+
+class PageExec:
     
-    def __init__(self, exec: WhereExec, page_num=1, page_size=10):
-        self.exec = exec
+    def __init__(self, cls, page_num=1, page_size=10):
+        self.cls = cls
         self.page_num = page_num
         self.page_size = page_size
 
-    def query(self, *fields, **kwargs):
+    def select(self, *fields, **kwargs):
         """
-        Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-             SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        Person.page(1, 10).select('id', 'name', 'age', name='张三', age=55)
         """
-        return self.exec.cls.query_page(self.page_num, self.page_size, *fields, **kwargs)
+        return self.cls.select_page(self.page_num, self.page_size, *fields, **kwargs)
 
-    def select(self, *fields, **kwargs):
+    def query(self, *fields, **kwargs):
         """
-        Execute select SQL and return list(tuple) or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-             SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        Person.page(1, 10).query('id', 'name', 'age', name='张三', age=55)
         """
-        return self.exec.cls.select_page(self.page_num, self.page_size, *fields, **kwargs)
-
-    def where(self, **kwargs):
-        self.exec.kwargs = kwargs
-        return self
+        return self.cls.query_page(self.page_num, self.page_size, *fields, **kwargs)
 
-    def fields(self, *fields) -> WhereExec:
-        return self.exec.fields(*fields)
-
-    def find(self, *args, **kwargs):
+    def find(self, *fields, **kwargs):
         """
-        Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-             SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        Person.page(1, 10).query('id', 'name', 'age', name='张三', age=55)
         """
-        return self.exec.cls.find_page(self.page_num, self.page_size, *fields, **kwargs)
+        return self.cls.find_page(self.page_num, self.page_size, *fields, **kwargs)
+
+    def where(self, **kwargs) -> WherePageExec:
+        return WherePageExec(WhereExec(self.cls, **kwargs), self.page_num, self.page_size)
+
+    def fields(self, *fields) -> FieldPageExec:
+        return FieldPageExec(FieldExec(self.cls, *fields), self.page_num, self.page_size)
 
 
 def split_ids(ids: Sequence[int], batch_size):
     return [ids[i:i + batch_size] for i in range(0, len(ids), batch_size)]
 
 
 def get_table_name(class_name):
```

### Comparing `sqlx-orm-0.0.3/orm/snowflake.py` & `sqlx-orm-0.0.5/orm/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlx-orm-0.0.3/setup.py` & `sqlx-orm-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 
 setup(
     name='sqlx-orm',
     packages=['orm'],
     description="A single table ORM framework for python. Support MySQL, PostgreSQL, SQLite etc.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.0.3',
+    version='0.0.5',
     install_requires=[
-        'sqlx-exec>=2.3.4',
+        'sqlx-exec>=2.3.5',
     ],
     url='https://gitee.com/summry/sqlx-orm',
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

### Comparing `sqlx-orm-0.0.3/sqlx_orm.egg-info/PKG-INFO` & `sqlx-orm-0.0.5/sqlx_orm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sqlx-orm
-Version: 0.0.3
+Version: 0.0.5
 Summary: A single table ORM framework for python. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlx-orm
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
 Platform: UNKNOWN
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
```


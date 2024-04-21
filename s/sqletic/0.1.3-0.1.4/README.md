# Comparing `tmp/sqletic-0.1.3.tar.gz` & `tmp/sqletic-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqletic-0.1.3.tar", max compression
+gzip compressed data, was "sqletic-0.1.4.tar", max compression
```

## Comparing `sqletic-0.1.3.tar` & `sqletic-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1196 2024-02-23 21:16:58.319040 sqletic-0.1.3/README.md
--rw-r--r--   0        0        0      551 2024-03-02 06:38:08.772523 sqletic-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       36 2024-02-19 07:54:04.462165 sqletic-0.1.3/sqletic/__init__.py
--rw-r--r--   0        0        0       39 2024-02-12 07:29:27.726892 sqletic-0.1.3/sqletic/__init__.py~
--rw-r--r--   0        0        0    13570 2024-03-02 06:27:46.480091 sqletic-0.1.3/sqletic/engine.py
--rw-r--r--   0        0        0    10599 2024-02-18 20:50:42.618765 sqletic-0.1.3/sqletic/engine.py~
--rw-r--r--   0        0        0     2916 2024-03-01 14:01:40.726062 sqletic-0.1.3/sqletic/expression.py
--rw-r--r--   0        0        0     2947 2024-02-12 07:31:39.164674 sqletic-0.1.3/sqletic/expression.py~
--rw-r--r--   0        0        0     1062 2024-02-23 20:56:18.648578 sqletic-0.1.3/sqletic/scope.py
--rw-r--r--   0        0        0      868 2024-02-16 16:55:43.334152 sqletic-0.1.3/sqletic/scope.py~
--rw-r--r--   0        0        0     1579 1970-01-01 00:00:00.000000 sqletic-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1196 2024-02-23 21:16:58.319040 sqletic-0.1.4/README.md
+-rw-r--r--   0        0        0      601 2024-04-21 19:36:01.154514 sqletic-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       36 2024-02-19 07:54:04.462165 sqletic-0.1.4/sqletic/__init__.py
+-rw-r--r--   0        0        0       39 2024-02-12 07:29:27.726892 sqletic-0.1.4/sqletic/__init__.py~
+-rw-r--r--   0        0        0    14227 2024-04-21 18:47:55.015548 sqletic-0.1.4/sqletic/engine.py
+-rw-r--r--   0        0        0    10599 2024-02-18 20:50:42.618765 sqletic-0.1.4/sqletic/engine.py~
+-rw-r--r--   0        0        0     3108 2024-03-24 20:56:53.868138 sqletic-0.1.4/sqletic/expression.py
+-rw-r--r--   0        0        0     2947 2024-02-12 07:31:39.164674 sqletic-0.1.4/sqletic/expression.py~
+-rw-r--r--   0        0        0     1062 2024-02-23 20:56:18.648578 sqletic-0.1.4/sqletic/scope.py
+-rw-r--r--   0        0        0      868 2024-02-16 16:55:43.334152 sqletic-0.1.4/sqletic/scope.py~
+-rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 sqletic-0.1.4/PKG-INFO
```

### Comparing `sqletic-0.1.3/README.md` & `sqletic-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sqletic-0.1.3/pyproject.toml` & `sqletic-0.1.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "sqletic"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Charles Bajeux <charles.bajeux@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-sqlton = "^0.1.5"
+sqlton = "^0.1.17"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 test_expression = "tests.test_expression:main"
 test_map = "tests.test_map:main"
+test_create_drop = "tests.test_create_drop:main"
 test_select = "tests.test_select:main"
 test_insert = "tests.test_insert:main"
 test_update = "tests.test_update:main"
 test_delete = "tests.test_delete:main"
```

### Comparing `sqletic-0.1.3/sqletic/engine.py` & `sqletic-0.1.4/sqletic/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlton.ast import All, Alias, Index, Operation, Column, Select, SelectCore, Values, Insert, Update, Delete, Table
+from sqlton.ast import All, Alias, Index, Operation, Column, Create, Drop, Select, SelectCore, Values, Insert, Update, Delete, Table
 from sqlton import parse
 from sqletic.scope import lookup, Scope, Entry
 from sqletic.expression import Evaluator
 
 def keep_recursive_set(name, expression):
     def in_collection(collection):
         if isinstance(collection, Values):
@@ -35,42 +35,42 @@
                 raise Exception("CT shall have been refered in one of the branch")
         else:
             return expression
     else:
         return expression
                 
 class CommonTable:
-    def __init__(self, engine, name, columns, select, entries=None):
+    def __init__(self, engine, name, columns, select, scope, entries=None):
         if (entries is None and
             not (isinstance(select, Operation) and
                  select.operator[0] in ('UNION', 'INTERSECT', 'EXCEPT'))):
             raise ValueError('Root expression shall be set operation of values and/or select expression')
         
         self.engine = Engine(engine.tables | {name: entries if entries else []})
         self.name = name
         self.columns = columns
         self.select = select
 
     def __iter__(self):
         entries = []
         
-        for _, scope in self.engine.iterate({}, self.select):
-            entry = dict(zip(self.columns, scope[None].values())) 
+        for _, _scope in self.engine.iterate(scope, self.select):
+            entry = dict(zip(self.columns, _scope[None].values())) 
             entries.append(entry)
             yield entry
 
         if entries:
             select = keep_recursive_set(self.name, self.select)
             yield from CommonTable(self.engine,
                                    self.name,
                                    self.columns,
                                    select,
+                                   scope,
                                    entries)
 
-        
 class Engine:
     def __init__(self, tables):
         self.tables = tables
         self.iterator = None
         self.description = ()
         self.rowcount = 0
 
@@ -80,27 +80,38 @@
             while entry := self.fetchone():
                 yield entry
             self.iterator = None
         else:
             raise StopIteration()
         
     def execute(self, statement):
-        statement = parse(statement)
+        self.iterator = None
+        statement, = parse(statement)
 
-        if isinstance(statement, Select): 
+        if isinstance(statement, Create):
+            self.execute_create(statement)
+        elif isinstance(statement, Drop):
+            self.execute_drop(statement)
+        elif isinstance(statement, Select): 
             self.iterator = self.iterate({}, statement)
         elif isinstance(statement, Insert):
             self.execute_insert(statement)
         elif isinstance(statement, Update):
             self.execute_update(statement)
         elif isinstance(statement, Delete):
             self.execute_delete(statement)
         else:
             raise NotImplementedError(f'Statement {statement}')
 
+    def execute_create(self, statement):
+        self.tables[statement.table.name] = []
+
+    def execute_drop(self, statement):
+        del self.tables[statement.table.name]
+        
     def execute_insert(self, statement):
         entries = (self.scope_to_entry((All(),), scope)
                    for _, scope
                    in self.iterate({}, statement.values))
 
         if not (len(statement.columns) == 1 and isinstance(statement.columns[0], All)):
             entries = (dict(zip(statement.columns, entry.values())) for entry in entries)
@@ -163,14 +174,19 @@
                 if evaluation:
                     to_remove.append(entry)
                     
         for entry in to_remove:
             self.tables[table].remove(entry)
                     
     def fetchone(self):
+        if not self.iterator:
+            self.description = ()
+            self.rowcount = 0
+            return None
+        
         try:
             name, scope = next(self.iterator)
         except StopIteration:
             return None
         
         entry = self.scope_to_entry((All(),), scope)
         
@@ -216,15 +232,16 @@
         return entry
 
     def iterate_select(self, scope, select:Select):
         if hasattr(select, 'with_clause'):
             scope[CommonTable] = {cte.name: CommonTable(self,
                                                         cte.name,
                                                         cte.columns,
-                                                        cte.select)
+                                                        cte.select,
+                                                        scope)
                                   for cte in select.with_clause.ctes}
             
         yield from self.iterate(scope, select.select_core)
 
 
     def iterate_values(self, scope, values:Values):
         for columns in values.values:
@@ -273,15 +290,15 @@
         name = alias.replacement
         for _name, _scope in self.iterate(scope, alias.original):
             yield name, {name: _scope[_name]} | scope
 
     def iterate_table(self, scope, table: Table):
         if table.name in self.tables:
             collection = self.tables[table.name]
-        elif table.name in scope[CommonTable]:
+        elif CommonTable in scope and table.name in scope[CommonTable]:
             collection = scope[CommonTable][table.name]
         else:
             raise KeyError(f'Found no such {table.name} table neither in common tables ({scope[CommonTable].keys()}) nor tables {self.tables.keys()}')
         
         for entry in collection:
             yield table.name, scope | {table.name:entry}
```

### Comparing `sqletic-0.1.3/sqletic/engine.py~` & `sqletic-0.1.4/sqletic/engine.py~`

 * *Files identical despite different names*

### Comparing `sqletic-0.1.3/sqletic/expression.py` & `sqletic-0.1.4/sqletic/expression.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 from sqlton.ast import Alias, Operation, Column
 from sqletic.scope import lookup
 import datetime
 import operator
+from re import sub, match
+from functools import partial
 
 def not_implemented(a, b):
     raise NotImplementedError()
 
+def like(a, b):
+    for rule, replacement in ((r'\.', r'\.'),
+                              (r'%', '.*'),
+                              (r'_', '.')):
+        b = sub(rule, replacement, b)
+    _match = match('^' + b + '$', a)
+    return  _match is not None
+
 class Evaluator:
     functions = {'concat':lambda *args:''.join((arg
                                                 if isinstance(arg, str)
                                                 else repr(arg))
                                                for arg in args)}
 
     def __init__(self, scope):
@@ -68,14 +78,13 @@
                  ('*',): operator.mul,
                  ('/',): operator.truediv,
                  ('+',): operator.add,
                  ('-',): operator.sub,
                  ('AND',): operator.and_,
                  ('OR',): operator.or_,
                  ('IN',): operator.contains,
-                 ('LIKE',): lambda a, b: re.match('^' + sub('_', '.', sub(r'\?', '.*', b)) + '$',
-                                                  a) is not None,
+                 ('LIKE',): like,
                  ('GLOB',): not_implemented,
-                 ('REGEXP',): lambda a, b: re.match(b, a),
+                 ('REGEXP',): lambda a, b: match(b, a) is not None,
                  ('MATCH',): not_implemented,
                  ('NOT', any): not_implemented}
```

### Comparing `sqletic-0.1.3/sqletic/expression.py~` & `sqletic-0.1.4/sqletic/expression.py~`

 * *Files identical despite different names*

### Comparing `sqletic-0.1.3/sqletic/scope.py` & `sqletic-0.1.4/sqletic/scope.py`

 * *Files identical despite different names*

### Comparing `sqletic-0.1.3/sqletic/scope.py~` & `sqletic-0.1.4/sqletic/scope.py~`

 * *Files identical despite different names*

### Comparing `sqletic-0.1.3/PKG-INFO` & `sqletic-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sqletic
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Charles Bajeux
 Author-email: charles.bajeux@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: sqlton (>=0.1.5,<0.2.0)
+Requires-Dist: sqlton (>=0.1.17,<0.2.0)
 Description-Content-Type: text/markdown
 
 # SQLetic
 
 SQLetic is an SQL database engine in pure python iterating over list acting as table indexed by there name in a dictionary.
 
 ```python
```


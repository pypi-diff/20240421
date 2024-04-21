# Comparing `tmp/sqlton-0.1.8.tar.gz` & `tmp/sqlton-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlton-0.1.8.tar", max compression
+gzip compressed data, was "sqlton-0.1.9.tar", max compression
```

## Comparing `sqlton-0.1.8.tar` & `sqlton-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      578 2023-12-27 19:53:09.552847 sqlton-0.1.8/README.md
--rw-r--r--   0        0        0      386 2024-03-11 11:22:50.185528 sqlton-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      182 2024-03-10 16:01:36.061823 sqlton-0.1.8/sqlton/__init__.py
--rw-r--r--   0        0        0        0 2023-11-18 16:58:51.710822 sqlton-0.1.8/sqlton/__init__.py~
--rw-r--r--   0        0        0     1200 2024-02-24 19:38:12.662040 sqlton-0.1.8/sqlton/ast.py
--rw-r--r--   0        0        0     1115 2024-01-30 20:13:53.392481 sqlton-0.1.8/sqlton/ast.py~
--rw-r--r--   0        0        0    28581 2024-03-11 11:21:33.447650 sqlton-0.1.8/sqlton/parser.py
--rw-r--r--   0        0        0    20580 2024-02-11 20:37:41.945631 sqlton-0.1.8/sqlton/parser.py~
--rw-r--r--   0        0        0     1007 1970-01-01 00:00:00.000000 sqlton-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-27 19:53:09.552847 sqlton-0.1.9/README.md
+-rw-r--r--   0        0        0      386 2024-03-12 08:19:46.615322 sqlton-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      182 2024-03-10 16:01:36.061823 sqlton-0.1.9/sqlton/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-18 16:58:51.710822 sqlton-0.1.9/sqlton/__init__.py~
+-rw-r--r--   0        0        0     1200 2024-02-24 19:38:12.662040 sqlton-0.1.9/sqlton/ast.py
+-rw-r--r--   0        0        0     1115 2024-01-30 20:13:53.392481 sqlton-0.1.9/sqlton/ast.py~
+-rw-r--r--   0        0        0    28562 2024-03-12 08:19:16.191612 sqlton-0.1.9/sqlton/parser.py
+-rw-r--r--   0        0        0    20580 2024-02-11 20:37:41.945631 sqlton-0.1.9/sqlton/parser.py~
+-rw-r--r--   0        0        0     1007 1970-01-01 00:00:00.000000 sqlton-0.1.9/PKG-INFO
```

### Comparing `sqlton-0.1.8/README.md` & `sqlton-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `sqlton-0.1.8/sqlton/ast.py` & `sqlton-0.1.9/sqlton/ast.py`

 * *Files identical despite different names*

### Comparing `sqlton-0.1.8/sqlton/ast.py~` & `sqlton-0.1.9/sqlton/ast.py~`

 * *Files identical despite different names*

### Comparing `sqlton-0.1.8/sqlton/parser.py` & `sqlton-0.1.9/sqlton/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -868,16 +868,15 @@
                 ('NULL_LITERAL',),
                 ('RP',)))
     def expr_null(self, p):
         return self.cast(p[2], None)
 
     @_('EXISTS LP select RP')
     def expr_boolean(self, p):
-        return Operation(('EXISTS',),
-                         p.select)
+        return Operation(('EXISTS',), None, p.select)
     
     @_('NOT expr_boolean %prec UNOT')
     def expr_boolean(self, p):
         return Operation(('NOT',), None, p[1])
 
     @_('PLUS expr_numeric %prec UPLUS')
     def expr_numeric(self, p):
```

### Comparing `sqlton-0.1.8/sqlton/parser.py~` & `sqlton-0.1.9/sqlton/parser.py~`

 * *Files identical despite different names*

### Comparing `sqlton-0.1.8/PKG-INFO` & `sqlton-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlton
-Version: 0.1.8
+Version: 0.1.9
 Summary: Parse SQL statement into straight forward Syntax Tree.
 Author: Charles Bajeux
 Author-email: charles.bajeux@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```


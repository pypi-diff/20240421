# Comparing `tmp/salinic-0.3.8.tar.gz` & `tmp/salinic-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salinic-0.3.8.tar", max compression
+gzip compressed data, was "salinic-0.3.9.tar", max compression
```

## Comparing `salinic-0.3.8.tar` & `salinic-0.3.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    10226 2023-08-31 06:14:42.345565 salinic-0.3.8/LICENSE
--rw-r--r--   0        0        0     1964 2023-08-31 06:14:42.345565 salinic-0.3.8/README.md
--rw-r--r--   0        0        0      551 2023-08-31 06:14:42.345565 salinic-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      434 2023-08-31 06:14:42.345565 salinic-0.3.8/salinic/__init__.py
--rw-r--r--   0        0        0        0 2023-08-31 06:14:42.345565 salinic-0.3.8/salinic/backends/__init__.py
--rw-r--r--   0        0        0        0 2023-08-31 06:14:42.345565 salinic-0.3.8/salinic/backends/solr/__init__.py
--rw-r--r--   0        0        0     3677 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/backends/solr/client.py
--rw-r--r--   0        0        0     2139 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/backends/solr/index.py
--rw-r--r--   0        0        0     3829 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/backends/solr/schema_manager.py
--rw-r--r--   0        0        0      468 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/backends/solr/types.py
--rw-r--r--   0        0        0        0 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/backends/xapian/__init__.py
--rw-r--r--   0        0        0     1204 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/backends/xapian/client.py
--rw-r--r--   0        0        0     6955 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/backends/xapian/index.py
--rw-r--r--   0        0        0      360 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/backends/xapian/schema_manager.py
--rw-r--r--   0        0        0      181 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/engine.py
--rw-r--r--   0        0        0      428 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/field.py
--rw-r--r--   0        0        0     1951 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/index.py
--rw-r--r--   0        0        0     4323 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/query.py
--rw-r--r--   0        0        0     2889 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/schema.py
--rw-r--r--   0        0        0     1264 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/schema_manager.py
--rw-r--r--   0        0        0      221 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/search.py
--rw-r--r--   0        0        0      601 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/types.py
--rw-r--r--   0        0        0     1825 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/url.py
--rw-r--r--   0        0        0      901 2023-08-31 06:14:42.349565 salinic-0.3.8/salinic/utils.py
--rw-r--r--   0        0        0     2563 1970-01-01 00:00:00.000000 salinic-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    10226 2023-09-16 14:52:51.841503 salinic-0.3.9/LICENSE
+-rw-r--r--   0        0        0     1964 2023-09-16 14:52:51.841503 salinic-0.3.9/README.md
+-rw-r--r--   0        0        0      551 2023-09-16 14:52:51.841503 salinic-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      434 2023-09-16 14:52:51.841503 salinic-0.3.9/salinic/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/backends/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/backends/solr/__init__.py
+-rw-r--r--   0        0        0     3677 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/backends/solr/client.py
+-rw-r--r--   0        0        0     2255 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/backends/solr/index.py
+-rw-r--r--   0        0        0     3829 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/backends/solr/schema_manager.py
+-rw-r--r--   0        0        0      468 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/backends/solr/types.py
+-rw-r--r--   0        0        0        0 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/backends/xapian/__init__.py
+-rw-r--r--   0        0        0     1313 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/backends/xapian/client.py
+-rw-r--r--   0        0        0     7216 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/backends/xapian/index.py
+-rw-r--r--   0        0        0      360 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/backends/xapian/schema_manager.py
+-rw-r--r--   0        0        0      181 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/engine.py
+-rw-r--r--   0        0        0      428 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/field.py
+-rw-r--r--   0        0        0     1952 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/index.py
+-rw-r--r--   0        0        0     4323 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/query.py
+-rw-r--r--   0        0        0     2889 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/schema.py
+-rw-r--r--   0        0        0     1264 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/schema_manager.py
+-rw-r--r--   0        0        0      221 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/search.py
+-rw-r--r--   0        0        0      601 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/types.py
+-rw-r--r--   0        0        0     1825 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/url.py
+-rw-r--r--   0        0        0      901 2023-09-16 14:52:51.845503 salinic-0.3.9/salinic/utils.py
+-rw-r--r--   0        0        0     2563 1970-01-01 00:00:00.000000 salinic-0.3.9/PKG-INFO
```

### Comparing `salinic-0.3.8/LICENSE` & `salinic-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `salinic-0.3.8/README.md` & `salinic-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `salinic-0.3.8/pyproject.toml` & `salinic-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "salinic"
-version = "0.3.8"
+version = "0.3.9"
 description = "Search abstraction layer"
 authors = ["Eugen Ciur <eugen@papermerge.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4.0"
 pydantic = "^2.1.1"
```

### Comparing `salinic-0.3.8/salinic/backends/solr/client.py` & `salinic-0.3.9/salinic/backends/solr/client.py`

 * *Files identical despite different names*

### Comparing `salinic-0.3.8/salinic/backends/solr/index.py` & `salinic-0.3.9/salinic/backends/solr/index.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import json
+import logging
 
 from pydantic import BaseModel
 
 from salinic.field import Field
 from salinic.query import SearchQuery
 from salinic.utils import filter_keys, first, trim_suffixes
 
+logger = logging.getLogger(__name__)
+
 
 class Base:
     def __init__(self, client, schema):
         self.client = client
         self.schema = schema
 
     def search(self, sq: SearchQuery):
@@ -57,12 +60,13 @@
                 actual_value = model.get_field_value(name)
                 orig_value = model_dict.pop(name)
                 model_dict[name] = actual_value
                 model_dict[f'{name}_orig_'] = json.dumps(orig_value)
 
         self.client.add(model_dict)
 
-    def remove(self, kwargs):
+    def remove(self, **kwargs):
+        logger.debug("Remove document with kwargs={kwargs}")
         self.client.remove(**kwargs)
 
 
 IndexRO = IndexRW
```

### Comparing `salinic-0.3.8/salinic/backends/solr/schema_manager.py` & `salinic-0.3.9/salinic/backends/solr/schema_manager.py`

 * *Files identical despite different names*

### Comparing `salinic-0.3.8/salinic/backends/xapian/client.py` & `salinic-0.3.9/salinic/backends/xapian/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,35 @@
+import logging
+
 import xapian
 
 from salinic.url import URL
 
 RO = 'ro'
 RW = 'rw'
 
 
+logger = logging.getLogger(__name__)
+
+
 class ClientRW:
 
     def __init__(self, url: URL):
         self._db_path = url.index
         self._db = xapian.WritableDatabase(
             self._db_path,
             xapian.DB_CREATE_OR_OPEN
         )
 
     def replace_document(self, idterm: str, doc: xapian.Document):
         self.db.replace_document(idterm, doc)
         self.commit()
 
     def delete_document(self, docid: str):
+        logger.debug("delete_document docid={docid}")
         self.db.delete_document(docid)
         self.commit()
 
     def commit(self) -> None:
         self.db.commit()
 
     @property
```

### Comparing `salinic-0.3.8/salinic/backends/xapian/index.py` & `salinic-0.3.9/salinic/backends/xapian/index.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import json
+import logging
 
 import xapian
 from pydantic import BaseModel
 
 from salinic.field import Field, IdField, KeywordField, TextField, UUIDField
 from salinic.query import SearchQuery
 from salinic.utils import first
 
+logger = logging.getLogger(__name__)
+
 
 class IndexRO:
 
     def __init__(self, client, schema, language="en"):
         self.client = client
         self._schema = schema
         self._language = language
@@ -119,16 +122,22 @@
 
         identifier = getattr(entity, primary_key_name)
         idterm = f"{primary_key_name.upper()}{identifier}"
         doc.add_boolean_term(idterm)
 
         self.client.replace_document(idterm, doc)
 
-    def remove(self, docid: str):
-        self.client.delete_document(docid)
+    def remove(self, **kwargs):
+        logger.debug(f"Removing kwargs={kwargs}")
+
+        for key, value in kwargs.items():
+            id_term = f"{key.upper()}{value.replace('-', '')}"
+            logger.debug(f"id_term={id_term}")
+
+            self.client.delete_document(id_term)
 
     def search(self, sq: SearchQuery):
         results = []
 
         if str(sq.query.free_text):
             query = self._queryparser.parse_query(
                 str(sq.query.free_text)
```

### Comparing `salinic-0.3.8/salinic/index.py` & `salinic-0.3.9/salinic/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     def __init__(self, engine, schema):
         super().__init__(engine, schema)
         self.backend = get_rw_index_backend(engine, schema)
 
     def add(self, entity):
         self.backend.add(entity)
 
-    def remove(self, docid: str):
-        self.backend.remove(docid)
+    def remove(self, **kwargs):
+        self.backend.remove(**kwargs)
 
 
 def get_ro_client_backend_class(engine):
     module_full_path = f'salinic.backends.{engine.url.scheme}.client'
     module = importlib.import_module(module_full_path)
 
     return module.ClientRO
```

### Comparing `salinic-0.3.8/salinic/query.py` & `salinic-0.3.9/salinic/query.py`

 * *Files identical despite different names*

### Comparing `salinic-0.3.8/salinic/schema.py` & `salinic-0.3.9/salinic/schema.py`

 * *Files identical despite different names*

### Comparing `salinic-0.3.8/salinic/schema_manager.py` & `salinic-0.3.9/salinic/schema_manager.py`

 * *Files identical despite different names*

### Comparing `salinic-0.3.8/salinic/types.py` & `salinic-0.3.9/salinic/types.py`

 * *Files identical despite different names*

### Comparing `salinic-0.3.8/salinic/url.py` & `salinic-0.3.9/salinic/url.py`

 * *Files identical despite different names*

### Comparing `salinic-0.3.8/salinic/utils.py` & `salinic-0.3.9/salinic/utils.py`

 * *Files identical despite different names*

### Comparing `salinic-0.3.8/PKG-INFO` & `salinic-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salinic
-Version: 0.3.8
+Version: 0.3.9
 Summary: Search abstraction layer
 Author: Eugen Ciur
 Author-email: eugen@papermerge.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


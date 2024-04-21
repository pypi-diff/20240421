# Comparing `tmp/whyhow-0.0.3.tar.gz` & `tmp/whyhow-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whyhow-0.0.3.tar", last modified: Fri Apr  5 04:36:08 2024, max compression
+gzip compressed data, was "whyhow-0.0.4.tar", last modified: Sun Apr 21 02:16:52 2024, max compression
```

## Comparing `whyhow-0.0.3.tar` & `whyhow-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-05 04:36:08.732628 whyhow-0.0.3/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     5447 2024-04-05 04:36:08.732419 whyhow-0.0.3/PKG-INFO
--rw-r--r--   0 tomsmoker   (501) staff       (20)     4318 2024-04-04 07:54:08.000000 whyhow-0.0.3/README.md
--rw-r--r--   0 tomsmoker   (501) staff       (20)     2061 2024-04-04 07:43:46.000000 whyhow-0.0.3/pyproject.toml
--rw-r--r--   0 tomsmoker   (501) staff       (20)       38 2024-04-05 04:36:08.732668 whyhow-0.0.3/setup.cfg
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-05 04:36:08.726125 whyhow-0.0.3/src/
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-05 04:36:08.727666 whyhow-0.0.3/src/whyhow/
--rw-r--r--   0 tomsmoker   (501) staff       (20)      125 2024-04-05 04:26:15.000000 whyhow-0.0.3/src/whyhow/__init__.py
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-05 04:36:08.729347 whyhow-0.0.3/src/whyhow/apis/
--rw-r--r--   0 tomsmoker   (501) staff       (20)       49 2024-03-30 23:23:35.000000 whyhow-0.0.3/src/whyhow/apis/__init__.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      501 2024-04-04 06:55:34.000000 whyhow-0.0.3/src/whyhow/apis/base.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     3757 2024-04-05 04:27:59.000000 whyhow-0.0.3/src/whyhow/apis/graph.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     6707 2024-04-04 07:04:26.000000 whyhow-0.0.3/src/whyhow/client.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      166 2024-03-30 23:23:35.000000 whyhow-0.0.3/src/whyhow/exceptions.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)        0 2024-03-30 23:23:35.000000 whyhow-0.0.3/src/whyhow/py.typed
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-05 04:36:08.730506 whyhow-0.0.3/src/whyhow/schemas/
--rw-r--r--   0 tomsmoker   (501) staff       (20)      189 2024-03-30 23:23:35.000000 whyhow-0.0.3/src/whyhow/schemas/__init__.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      624 2024-03-30 23:23:35.000000 whyhow-0.0.3/src/whyhow/schemas/base.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     3755 2024-04-04 06:49:03.000000 whyhow-0.0.3/src/whyhow/schemas/common.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     1155 2024-04-05 04:27:51.000000 whyhow-0.0.3/src/whyhow/schemas/graph.py
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-05 04:36:08.731292 whyhow-0.0.3/src/whyhow.egg-info/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     5447 2024-04-05 04:36:08.000000 whyhow-0.0.3/src/whyhow.egg-info/PKG-INFO
--rw-r--r--   0 tomsmoker   (501) staff       (20)      548 2024-04-05 04:36:08.000000 whyhow-0.0.3/src/whyhow.egg-info/SOURCES.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-04-05 04:36:08.000000 whyhow-0.0.3/src/whyhow.egg-info/dependency_links.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-03-31 17:56:30.000000 whyhow-0.0.3/src/whyhow.egg-info/not-zip-safe
--rw-r--r--   0 tomsmoker   (501) staff       (20)      218 2024-04-05 04:36:08.000000 whyhow-0.0.3/src/whyhow.egg-info/requires.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        7 2024-04-05 04:36:08.000000 whyhow-0.0.3/src/whyhow.egg-info/top_level.txt
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-05 04:36:08.731022 whyhow-0.0.3/tests/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     1431 2024-04-05 04:27:59.000000 whyhow-0.0.3/tests/test_client.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)       48 2024-03-30 23:23:35.000000 whyhow-0.0.3/tests/test_dummy.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-21 02:16:52.966239 whyhow-0.0.4/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     7907 2024-04-21 02:16:52.966003 whyhow-0.0.4/PKG-INFO
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     6778 2024-04-21 02:04:51.000000 whyhow-0.0.4/README.md
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     2061 2024-04-21 01:37:48.000000 whyhow-0.0.4/pyproject.toml
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       38 2024-04-21 02:16:52.966282 whyhow-0.0.4/setup.cfg
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-21 02:16:52.959864 whyhow-0.0.4/src/
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-21 02:16:52.961362 whyhow-0.0.4/src/whyhow/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      125 2024-04-21 02:10:14.000000 whyhow-0.0.4/src/whyhow/__init__.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-21 02:16:52.963098 whyhow-0.0.4/src/whyhow/apis/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       49 2024-03-30 23:23:35.000000 whyhow-0.0.4/src/whyhow/apis/__init__.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      501 2024-04-04 06:55:34.000000 whyhow-0.0.4/src/whyhow/apis/base.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     4797 2024-04-21 01:37:48.000000 whyhow-0.0.4/src/whyhow/apis/graph.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     6707 2024-04-21 01:37:48.000000 whyhow-0.0.4/src/whyhow/client.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      166 2024-03-30 23:23:35.000000 whyhow-0.0.4/src/whyhow/exceptions.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        0 2024-03-30 23:23:35.000000 whyhow-0.0.4/src/whyhow/py.typed
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-21 02:16:52.964043 whyhow-0.0.4/src/whyhow/schemas/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      189 2024-03-30 23:23:35.000000 whyhow-0.0.4/src/whyhow/schemas/__init__.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      624 2024-03-30 23:23:35.000000 whyhow-0.0.4/src/whyhow/schemas/base.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     5002 2024-04-21 01:37:48.000000 whyhow-0.0.4/src/whyhow/schemas/common.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     1459 2024-04-21 01:37:48.000000 whyhow-0.0.4/src/whyhow/schemas/graph.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-21 02:16:52.964810 whyhow-0.0.4/src/whyhow.egg-info/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     7907 2024-04-21 02:16:52.000000 whyhow-0.0.4/src/whyhow.egg-info/PKG-INFO
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      548 2024-04-21 02:16:52.000000 whyhow-0.0.4/src/whyhow.egg-info/SOURCES.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-04-21 02:16:52.000000 whyhow-0.0.4/src/whyhow.egg-info/dependency_links.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-03-31 17:56:30.000000 whyhow-0.0.4/src/whyhow.egg-info/not-zip-safe
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      218 2024-04-21 02:16:52.000000 whyhow-0.0.4/src/whyhow.egg-info/requires.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        7 2024-04-21 02:16:52.000000 whyhow-0.0.4/src/whyhow.egg-info/top_level.txt
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-21 02:16:52.964631 whyhow-0.0.4/tests/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     1431 2024-04-21 01:37:48.000000 whyhow-0.0.4/tests/test_client.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       48 2024-03-30 23:23:35.000000 whyhow-0.0.4/tests/test_dummy.py
```

### Comparing `whyhow-0.0.3/pyproject.toml` & `whyhow-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.3/src/whyhow/apis/graph.py` & `whyhow-0.0.4/src/whyhow/apis/graph.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """Interacting with the graph API."""
 
+import json
 import os
 from pathlib import Path
 
 from whyhow.apis.base import APIBase
+from whyhow.schemas.common import Schema as SchemaModel
 from whyhow.schemas.graph import (
     AddDocumentsResponse,
     CreateGraphResponse,
+    CreateQuestionGraphRequest,
+    CreateSchemaGraphRequest,
     QueryGraphRequest,
     QueryGraphResponse,
     QueryGraphReturn,
 )
 
 
 class GraphAPI(APIBase):
@@ -81,27 +85,58 @@
     def create_graph(self, namespace: str, questions: list[str]) -> str:
         """Create a new graph.
 
         Parameters
         ----------
         namespace : str
             The namespace of the graph to create.
-        documents : list[str]
-            The documents to associate with the graph. Only supports PDFs for now.
-        concepts : list[str]
-            The concepts to initialize the graph with.
+        questions : list[str]
+            The seed concepts to initialize the graph with.
         """
         if not questions:
             raise ValueError("No questions provided")
 
-        params = {"questions": questions}
+        request_body = CreateQuestionGraphRequest(questions=questions)
 
         raw_response = self.client.post(
             f"{self.prefix}/{namespace}/create_graph",
-            params=params,
+            json=request_body.model_dump(),
+        )
+
+        raw_response.raise_for_status()
+
+        response = CreateGraphResponse.model_validate(raw_response.json())
+
+        return response.message
+
+    def create_graph_from_schema(
+        self, namespace: str, schema_file: str
+    ) -> str:
+        """Create a new graph based on a user-defined schema.
+
+        Parameters
+        ----------
+        namespace : str
+            The namespace of the graph to create.
+        schema_file : str
+            The schema file to use to build the graph.
+        """
+        if not schema_file:
+            raise ValueError("No schema provided")
+
+        with open(schema_file, "r") as file:
+            schema_data = json.load(file)
+
+        schema_model = SchemaModel(**schema_data)
+
+        request_body = CreateSchemaGraphRequest(graph_schema=schema_model)
+
+        raw_response = self.client.post(
+            f"{self.prefix}/{namespace}/create_graph_from_schema",
+            json=request_body.model_dump(),
         )
 
         raw_response.raise_for_status()
 
         response = CreateGraphResponse.model_validate(raw_response.json())
 
         return response.message
```

### Comparing `whyhow-0.0.3/src/whyhow/client.py` & `whyhow-0.0.4/src/whyhow/client.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.3/src/whyhow/schemas/base.py` & `whyhow-0.0.4/src/whyhow/schemas/base.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.3/src/whyhow/schemas/common.py` & `whyhow-0.0.4/src/whyhow/schemas/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Shared schemas."""
 
-from typing import Any
+from typing import Any, List, Optional
 
 from pydantic import BaseModel, Field, model_validator
 
 
 class Node(BaseModel):
     """Schema for a single node.
 
@@ -131,7 +131,53 @@
             head=start.properties["name"],
             head_type=start.labels[0],  # take the first label
             relationship=relationship.type,
             tail=end.properties["name"],
             tail_type=end.labels[0],  # take the first label
             properties=relationship.properties,
         )
+
+
+# GRAPH SCHEMA
+class SchemaEntity(BaseModel):
+    """Schema Entity model."""
+
+    name: str
+    description: str
+
+
+class SchemaRelation(BaseModel):
+    """Schema Relation model."""
+
+    name: str
+    description: str
+
+
+class TriplePattern(BaseModel):
+    """Schema Triple Pattern model."""
+
+    head: str
+    relation: str
+    tail: str
+    description: str
+
+
+class Schema(BaseModel):
+    """Schema model."""
+
+    entities: List[SchemaEntity] = Field(default_factory=list)
+    relations: List[SchemaRelation] = Field(default_factory=list)
+    patterns: List[TriplePattern] = Field(default_factory=list)
+
+    def get_entity(self, name: str) -> Optional[SchemaEntity]:
+        """Return an entity by name if it exists in the schema."""
+        for entity in self.entities:
+            if entity.name == name:
+                return entity
+        return None  # Return None if no entity with that name is found
+
+    def get_relation(self, name: str) -> Optional[SchemaRelation]:
+        """Return a relation by name if it exists in the schema."""
+        for relation in self.relations:
+            if relation.name == name:
+                return relation
+        return None  # Return None if no relation with that name is found
```

### Comparing `whyhow-0.0.3/src/whyhow/schemas/graph.py` & `whyhow-0.0.4/src/whyhow/schemas/graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 """Collection of schemas for the API."""
 
 from typing import Literal
 
 from whyhow.schemas.base import BaseRequest, BaseResponse, BaseReturn
-from whyhow.schemas.common import Graph
+from whyhow.schemas.common import Graph, Schema
 
 # Custom types
 Status = Literal["success", "pending", "failure"]
 
 
 class AddDocumentsResponse(BaseResponse):
     """Schema for the response body of the add documents endpoint."""
 
     namespace: str
     message: str
 
 
+class CreateQuestionGraphRequest(BaseRequest):
+    """Schema for the request body of the create graph endpoint."""
+
+    questions: list[str]
+
+
+class CreateSchemaGraphRequest(BaseRequest):
+    """Schema for the request body of the create graph with schema endpoint."""
+
+    graph_schema: Schema
+
+
 # Request and response schemas
 class CreateGraphResponse(BaseResponse):
     """Schema for the response body of the create graph endpoint."""
 
     namespace: str
     message: str
```

### Comparing `whyhow-0.0.3/src/whyhow.egg-info/SOURCES.txt` & `whyhow-0.0.4/src/whyhow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.3/tests/test_client.py` & `whyhow-0.0.4/tests/test_client.py`

 * *Files identical despite different names*


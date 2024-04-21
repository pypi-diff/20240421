# Comparing `tmp/vanna-0.4.1.tar.gz` & `tmp/vanna-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanna-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vanna-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vanna-0.4.1.tar` & `vanna-0.4.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     7922 2024-04-17 03:45:33.384481 vanna-0.4.1/README.md
--rw-r--r--   0        0        0     1414 2024-04-17 03:45:33.400481 vanna-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     8725 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/ZhipuAI/ZhipuAI_Chat.py
--rw-r--r--   0        0        0     2849 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/ZhipuAI/ZhipuAI_embeddings.py
--rw-r--r--   0        0        0      116 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/ZhipuAI/__init__.py
--rw-r--r--   0        0        0     9248 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/__init__.py
--rw-r--r--   0        0        0       43 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/anthropic/__init__.py
--rw-r--r--   0        0        0     2615 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/anthropic/anthropic_chat.py
--rw-r--r--   0        0        0       28 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/base/__init__.py
--rw-r--r--   0        0        0    58143 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/base/base.py
--rw-r--r--   0        0        0       50 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/chromadb/__init__.py
--rw-r--r--   0        0        0     8792 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/chromadb/chromadb_vector.py
--rw-r--r--   0        0        0      717 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/exceptions/__init__.py
--rw-r--r--   0        0        0    23721 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/flask/__init__.py
--rw-r--r--   0        0        0   183889 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/flask/assets.py
--rw-r--r--   0        0        0     1246 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/flask/auth.py
--rw-r--r--   0        0        0       41 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/google/__init__.py
--rw-r--r--   0        0        0     1584 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/google/gemini_chat.py
--rw-r--r--   0        0        0      313 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/local.py
--rw-r--r--   0        0        0       37 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/marqo/__init__.py
--rw-r--r--   0        0        0     5242 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/marqo/marqo.py
--rw-r--r--   0        0        0       29 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/mistral/__init__.py
--rw-r--r--   0        0        0     1508 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/mistral/mistral.py
--rw-r--r--   0        0        0       27 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/ollama/__init__.py
--rw-r--r--   0        0        0     2418 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/ollama/ollama.py
--rw-r--r--   0        0        0       86 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/openai/__init__.py
--rw-r--r--   0        0        0     4764 2024-04-17 03:45:33.400481 vanna-0.4.1/src/vanna/openai/openai_chat.py
--rw-r--r--   0        0        0     1260 2024-04-17 03:45:33.404481 vanna-0.4.1/src/vanna/openai/openai_embeddings.py
--rw-r--r--   0        0        0       73 2024-04-17 03:45:33.404481 vanna-0.4.1/src/vanna/qdrant/__init__.py
--rw-r--r--   0        0        0    11940 2024-04-17 03:45:33.404481 vanna-0.4.1/src/vanna/qdrant/qdrant.py
--rw-r--r--   0        0        0     1856 2024-04-17 03:45:33.404481 vanna-0.4.1/src/vanna/remote.py
--rw-r--r--   0        0        0     4957 2024-04-17 03:45:33.404481 vanna-0.4.1/src/vanna/types/__init__.py
--rw-r--r--   0        0        0     2247 2024-04-17 03:45:33.404481 vanna-0.4.1/src/vanna/utils.py
--rw-r--r--   0        0        0       48 2024-04-17 03:45:33.404481 vanna-0.4.1/src/vanna/vannadb/__init__.py
--rw-r--r--   0        0        0     6168 2024-04-17 03:45:33.404481 vanna-0.4.1/src/vanna/vannadb/vannadb_vector.py
--rw-r--r--   0        0        0    10512 1970-01-01 00:00:00.000000 vanna-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     7922 2024-04-21 03:21:32.548116 vanna-0.4.2/README.md
+-rw-r--r--   0        0        0     1414 2024-04-21 03:21:32.564116 vanna-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     8725 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/ZhipuAI/ZhipuAI_Chat.py
+-rw-r--r--   0        0        0     2849 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/ZhipuAI/ZhipuAI_embeddings.py
+-rw-r--r--   0        0        0      116 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/ZhipuAI/__init__.py
+-rw-r--r--   0        0        0     9248 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/anthropic/__init__.py
+-rw-r--r--   0        0        0     2615 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/anthropic/anthropic_chat.py
+-rw-r--r--   0        0        0       28 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/base/__init__.py
+-rw-r--r--   0        0        0    58143 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/base/base.py
+-rw-r--r--   0        0        0       50 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/chromadb/__init__.py
+-rw-r--r--   0        0        0     8792 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/chromadb/chromadb_vector.py
+-rw-r--r--   0        0        0      685 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/exceptions/__init__.py
+-rw-r--r--   0        0        0    23721 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/flask/__init__.py
+-rw-r--r--   0        0        0   183889 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/flask/assets.py
+-rw-r--r--   0        0        0     1246 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/flask/auth.py
+-rw-r--r--   0        0        0       41 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/google/__init__.py
+-rw-r--r--   0        0        0     1584 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/google/gemini_chat.py
+-rw-r--r--   0        0        0      313 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/local.py
+-rw-r--r--   0        0        0       37 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/marqo/__init__.py
+-rw-r--r--   0        0        0     5242 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/marqo/marqo.py
+-rw-r--r--   0        0        0       29 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/mistral/__init__.py
+-rw-r--r--   0        0        0     1508 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/mistral/mistral.py
+-rw-r--r--   0        0        0       27 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/ollama/__init__.py
+-rw-r--r--   0        0        0     2418 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/ollama/ollama.py
+-rw-r--r--   0        0        0       86 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/openai/__init__.py
+-rw-r--r--   0        0        0     4764 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/openai/openai_chat.py
+-rw-r--r--   0        0        0     1260 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/openai/openai_embeddings.py
+-rw-r--r--   0        0        0       73 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/qdrant/__init__.py
+-rw-r--r--   0        0        0    11940 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/qdrant/qdrant.py
+-rw-r--r--   0        0        0     1856 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/remote.py
+-rw-r--r--   0        0        0     4957 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/types/__init__.py
+-rw-r--r--   0        0        0     2247 2024-04-21 03:21:32.564116 vanna-0.4.2/src/vanna/utils.py
+-rw-r--r--   0        0        0       48 2024-04-21 03:21:32.568116 vanna-0.4.2/src/vanna/vannadb/__init__.py
+-rw-r--r--   0        0        0     6168 2024-04-21 03:21:32.568116 vanna-0.4.2/src/vanna/vannadb/vannadb_vector.py
+-rw-r--r--   0        0        0    10512 1970-01-01 00:00:00.000000 vanna-0.4.2/PKG-INFO
```

### Comparing `vanna-0.4.1/README.md` & `vanna-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/pyproject.toml` & `vanna-0.4.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "vanna"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="Zain Hoda", email="zain@vanna.ai" },
 ]
 
 description = "Generate SQL queries from natural language"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `vanna-0.4.1/src/vanna/ZhipuAI/ZhipuAI_Chat.py` & `vanna-0.4.2/src/vanna/ZhipuAI/ZhipuAI_Chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/ZhipuAI/ZhipuAI_embeddings.py` & `vanna-0.4.2/src/vanna/ZhipuAI/ZhipuAI_embeddings.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/__init__.py` & `vanna-0.4.2/src/vanna/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/anthropic/anthropic_chat.py` & `vanna-0.4.2/src/vanna/anthropic/anthropic_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/base/base.py` & `vanna-0.4.2/src/vanna/base/base.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/chromadb/chromadb_vector.py` & `vanna-0.4.2/src/vanna/chromadb/chromadb_vector.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/exceptions/__init__.py` & `vanna-0.4.2/src/vanna/exceptions/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-class ImproperlyConfigured(BaseException):
+class ImproperlyConfigured(Exception):
     """Raise for incorrect configuration."""
 
     pass
 
 
-class DependencyError(BaseException):
+class DependencyError(Exception):
     """Raise for missing dependencies."""
 
     pass
 
 
-class ConnectionError(BaseException):
+class ConnectionError(Exception):
     """Raise for connection"""
 
     pass
 
 
-class OTPCodeError(BaseException):
+class OTPCodeError(Exception):
     """Raise for invalid otp or not able to send it"""
 
     pass
 
 
-class SQLRemoveError(BaseException):
+class SQLRemoveError(Exception):
     """Raise when not able to remove SQL"""
 
     pass
 
 
-class ExecutionError(BaseException):
+class ExecutionError(Exception):
     """Raise when not able to execute Code"""
 
     pass
 
 
-class ValidationError(BaseException):
+class ValidationError(Exception):
     """Raise for validations"""
 
     pass
 
 
-class APIError(BaseException):
+class APIError(Exception):
     """Raise for API errors"""
 
     pass
```

### Comparing `vanna-0.4.1/src/vanna/flask/__init__.py` & `vanna-0.4.2/src/vanna/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/flask/assets.py` & `vanna-0.4.2/src/vanna/flask/assets.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/flask/auth.py` & `vanna-0.4.2/src/vanna/flask/auth.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/google/gemini_chat.py` & `vanna-0.4.2/src/vanna/google/gemini_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/marqo/marqo.py` & `vanna-0.4.2/src/vanna/marqo/marqo.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/mistral/mistral.py` & `vanna-0.4.2/src/vanna/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/ollama/ollama.py` & `vanna-0.4.2/src/vanna/ollama/ollama.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/openai/openai_chat.py` & `vanna-0.4.2/src/vanna/openai/openai_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/openai/openai_embeddings.py` & `vanna-0.4.2/src/vanna/openai/openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/qdrant/qdrant.py` & `vanna-0.4.2/src/vanna/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/remote.py` & `vanna-0.4.2/src/vanna/remote.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/types/__init__.py` & `vanna-0.4.2/src/vanna/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/utils.py` & `vanna-0.4.2/src/vanna/utils.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/src/vanna/vannadb/vannadb_vector.py` & `vanna-0.4.2/src/vanna/vannadb/vannadb_vector.py`

 * *Files identical despite different names*

### Comparing `vanna-0.4.1/PKG-INFO` & `vanna-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.4.1
+Version: 0.4.2
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


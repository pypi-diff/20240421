# Comparing `tmp/bedrock_bot-1.0.0.tar.gz` & `tmp/bedrock_bot-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bedrock_bot-1.0.0.tar", max compression
+gzip compressed data, was "bedrock_bot-1.0.1.tar", max compression
```

## Comparing `bedrock_bot-1.0.0.tar` & `bedrock_bot-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-04-20 05:06:19.297231 bedrock_bot-1.0.0/LICENSE
--rw-r--r--   0        0        0     1668 2024-04-21 04:31:00.433721 bedrock_bot-1.0.0/README.md
--rw-r--r--   0        0        0       91 2024-04-21 04:04:16.643947 bedrock_bot-1.0.0/bedrock_bot/__init__.py
--rw-r--r--   0        0        0     2290 2024-04-21 04:34:26.603691 bedrock_bot-1.0.0/bedrock_bot/cli.py
--rw-r--r--   0        0        0     3209 2024-04-21 04:35:01.783687 bedrock_bot-1.0.0/bedrock_bot/model.py
--rw-r--r--   0        0        0      152 2024-04-21 04:14:31.613860 bedrock_bot-1.0.0/bedrock_bot/util.py
--rw-r--r--   0        0        0      448 2024-04-21 04:35:32.893682 bedrock_bot-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2171 1970-01-01 00:00:00.000000 bedrock_bot-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-21 04:47:08.430033 bedrock_bot-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1668 2024-04-21 04:47:08.430033 bedrock_bot-1.0.1/README.md
+-rw-r--r--   0        0        0       91 2024-04-21 04:47:08.430033 bedrock_bot-1.0.1/bedrock_bot/__init__.py
+-rw-r--r--   0        0        0     2290 2024-04-21 04:47:08.430033 bedrock_bot-1.0.1/bedrock_bot/cli.py
+-rw-r--r--   0        0        0     3209 2024-04-21 04:47:08.430033 bedrock_bot-1.0.1/bedrock_bot/model.py
+-rw-r--r--   0        0        0      152 2024-04-21 04:47:08.430033 bedrock_bot-1.0.1/bedrock_bot/util.py
+-rw-r--r--   0        0        0      448 2024-04-21 04:47:08.430033 bedrock_bot-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2171 1970-01-01 00:00:00.000000 bedrock_bot-1.0.1/PKG-INFO
```

### Comparing `bedrock_bot-1.0.0/LICENSE` & `bedrock_bot-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.0/README.md` & `bedrock_bot-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.0/bedrock_bot/cli.py` & `bedrock_bot-1.0.1/bedrock_bot/cli.py`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.0/bedrock_bot/model.py` & `bedrock_bot-1.0.1/bedrock_bot/model.py`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.0/PKG-INFO` & `bedrock_bot-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bedrock-bot
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Author: Justin Dray
 Author-email: justin@dray.be
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


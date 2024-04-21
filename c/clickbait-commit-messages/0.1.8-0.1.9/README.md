# Comparing `tmp/clickbait_commit_messages-0.1.8.tar.gz` & `tmp/clickbait_commit_messages-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickbait_commit_messages-0.1.8.tar", max compression
+gzip compressed data, was "clickbait_commit_messages-0.1.9.tar", max compression
```

## Comparing `clickbait_commit_messages-0.1.8.tar` & `clickbait_commit_messages-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1075 2024-03-30 10:28:08.214614 clickbait_commit_messages-0.1.8/LICENSE
--rw-r--r--   0        0        0     4732 2024-04-21 11:29:57.787051 clickbait_commit_messages-0.1.8/README.md
--rw-r--r--   0        0        0     4676 2024-04-21 10:57:15.126367 clickbait_commit_messages-0.1.8/make_clickbaity.py
--rw-r--r--   0        0        0      631 2024-04-21 11:31:20.527045 clickbait_commit_messages-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5283 1970-01-01 00:00:00.000000 clickbait_commit_messages-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-03-30 10:28:08.214614 clickbait_commit_messages-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4732 2024-04-21 11:29:57.787051 clickbait_commit_messages-0.1.9/README.md
+-rw-r--r--   0        0        0     4676 2024-04-21 10:57:15.126367 clickbait_commit_messages-0.1.9/make_clickbaity.py
+-rw-r--r--   0        0        0      631 2024-04-21 13:47:11.393082 clickbait_commit_messages-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5283 1970-01-01 00:00:00.000000 clickbait_commit_messages-0.1.9/PKG-INFO
```

### Comparing `clickbait_commit_messages-0.1.8/LICENSE` & `clickbait_commit_messages-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clickbait_commit_messages-0.1.8/README.md` & `clickbait_commit_messages-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `clickbait_commit_messages-0.1.8/make_clickbaity.py` & `clickbait_commit_messages-0.1.9/make_clickbaity.py`

 * *Files identical despite different names*

### Comparing `clickbait_commit_messages-0.1.8/pyproject.toml` & `clickbait_commit_messages-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clickbait-commit-messages"
-version = "v0.1.8"
+version = "v0.1.9"
 description = "Make your commit messages extremely catchy."
 authors = ["anferico <f.cariaggi4@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "make_clickbaity.py" },
 ]
```

### Comparing `clickbait_commit_messages-0.1.8/PKG-INFO` & `clickbait_commit_messages-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickbait-commit-messages
-Version: 0.1.8
+Version: 0.1.9
 Summary: Make your commit messages extremely catchy.
 License: MIT
 Author: anferico
 Author-email: f.cariaggi4@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/notion-graph-0.2.7.tar.gz` & `tmp/notion-graph-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion-graph-0.2.7.tar", last modified: Sun Dec 17 03:38:11 2023, max compression
+gzip compressed data, was "notion-graph-0.2.8.tar", last modified: Sun Apr 21 03:05:52 2024, max compression
```

## Comparing `notion-graph-0.2.7.tar` & `notion-graph-0.2.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-10-12 23:56:38.629120 notion-graph-0.2.7/LICENSE
--rw-r--r--   0        0        0     3674 2023-12-17 03:01:09.207477 notion-graph-0.2.7/README.md
--rw-r--r--   0        0        0      636 2023-10-12 23:56:38.629120 notion-graph-0.2.7/notion_graph/__init__.py
--rw-r--r--   0        0        0       61 2023-10-12 23:56:38.629120 notion-graph-0.2.7/notion_graph/__main__.py
--rw-r--r--   0        0        0      641 2023-10-12 23:56:38.629120 notion-graph-0.2.7/notion_graph/cli.py
--rw-r--r--   0        0        0      454 2023-12-17 03:18:41.167197 notion-graph-0.2.7/notion_graph/helper.py
--rw-r--r--   0        0        0    14086 2023-12-17 03:34:08.886947 notion-graph-0.2.7/notion_graph/parser.py
--rw-r--r--   0        0        0      497 2023-12-17 03:36:19.526910 notion-graph-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     3935 1970-01-01 00:00:00.000000 notion-graph-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-10-12 23:56:38.629120 notion-graph-0.2.8/LICENSE
+-rw-r--r--   0        0        0     3674 2023-12-17 03:01:09.207477 notion-graph-0.2.8/README.md
+-rw-r--r--   0        0        0      636 2023-10-12 23:56:38.629120 notion-graph-0.2.8/notion_graph/__init__.py
+-rw-r--r--   0        0        0       61 2023-10-12 23:56:38.629120 notion-graph-0.2.8/notion_graph/__main__.py
+-rw-r--r--   0        0        0      641 2023-10-12 23:56:38.629120 notion-graph-0.2.8/notion_graph/cli.py
+-rw-r--r--   0        0        0      454 2024-04-18 13:07:19.627054 notion-graph-0.2.8/notion_graph/helper.py
+-rw-r--r--   0        0        0    14086 2024-04-21 02:59:23.110100 notion-graph-0.2.8/notion_graph/parser.py
+-rw-r--r--   0        0        0      497 2024-04-21 02:59:17.590101 notion-graph-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3935 1970-01-01 00:00:00.000000 notion-graph-0.2.8/PKG-INFO
```

### Comparing `notion-graph-0.2.7/LICENSE` & `notion-graph-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `notion-graph-0.2.7/README.md` & `notion-graph-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `notion-graph-0.2.7/notion_graph/__init__.py` & `notion-graph-0.2.8/notion_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `notion-graph-0.2.7/notion_graph/cli.py` & `notion-graph-0.2.8/notion_graph/cli.py`

 * *Files identical despite different names*

### Comparing `notion-graph-0.2.7/notion_graph/parser.py` & `notion-graph-0.2.8/notion_graph/parser.py`

 * *Files identical despite different names*

### Comparing `notion-graph-0.2.7/PKG-INFO` & `notion-graph-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-graph
-Version: 0.2.7
+Version: 0.2.8
 Summary: Generate a roam research like network graph view from your Notion pages.
 License: MIT
 Author-email: Steve Sun <sund.chn@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 ![](images/snap.png)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: notion-graph Version: 0.2.7 Summary: Generate a
+Metadata-Version: 2.1 Name: notion-graph Version: 0.2.8 Summary: Generate a
 roam research like network graph view from your Notion pages. License: MIT
 Author-email: Steve Sun
 gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown ![]
 (images/snap.png) # Notion Graph View ![github](https://img.shields.io/badge/
 python-3.9-blue.svg) ![github](https://img.shields.io/badge/license-MIT-
 green.svg) ![github](https://img.shields.io/badge/notion_version-2022.06.28-
 lightgrey.svg) Export [Notion](https://notion.so) pages to a Roam-Research like
```


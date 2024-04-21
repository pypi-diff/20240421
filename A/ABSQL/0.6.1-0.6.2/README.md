# Comparing `tmp/absql-0.6.1.tar.gz` & `tmp/absql-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absql-0.6.1.tar", last modified: Sun Apr 14 01:20:41 2024, max compression
+gzip compressed data, was "absql-0.6.2.tar", last modified: Sun Apr 21 15:24:03 2024, max compression
```

## Comparing `absql-0.6.1.tar` & `absql-0.6.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.643957 absql-0.6.1/
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.642482 absql-0.6.1/ABSQL.egg-info/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     9797 2024-04-14 01:20:41.000000 absql-0.6.1/ABSQL.egg-info/PKG-INFO
--rw-r--r--   0 chriscardillo   (501) staff       (20)      778 2024-04-14 01:20:41.000000 absql-0.6.1/ABSQL.egg-info/SOURCES.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)        1 2024-04-14 01:20:41.000000 absql-0.6.1/ABSQL.egg-info/dependency_links.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)       74 2024-04-14 01:20:41.000000 absql-0.6.1/ABSQL.egg-info/requires.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)       12 2024-04-14 01:20:41.000000 absql-0.6.1/ABSQL.egg-info/top_level.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1071 2023-05-12 18:29:12.000000 absql-0.6.1/LICENSE
--rw-r--r--   0 chriscardillo   (501) staff       (20)     9797 2024-04-14 01:20:41.643258 absql-0.6.1/PKG-INFO
--rw-r--r--   0 chriscardillo   (501) staff       (20)     9165 2024-02-09 23:11:51.000000 absql-0.6.1/README.md
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.632637 absql-0.6.1/absql/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     3157 2024-04-05 21:55:53.000000 absql-0.6.1/absql/__init__.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.633735 absql-0.6.1/absql/files/
--rw-r--r--   0 chriscardillo   (501) staff       (20)      790 2024-04-06 14:26:22.000000 absql-0.6.1/absql/files/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2980 2024-01-03 15:38:53.000000 absql-0.6.1/absql/files/loader.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     4100 2024-04-14 01:16:37.000000 absql-0.6.1/absql/files/parsers.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.635191 absql-0.6.1/absql/functions/
--rw-r--r--   0 chriscardillo   (501) staff       (20)      772 2023-05-12 18:29:12.000000 absql-0.6.1/absql/functions/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2331 2024-02-09 23:49:25.000000 absql-0.6.1/absql/functions/db.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      560 2023-05-12 18:29:12.000000 absql-0.6.1/absql/functions/env.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      350 2023-05-12 18:29:12.000000 absql-0.6.1/absql/functions/time.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.635456 absql-0.6.1/absql/render/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     3084 2024-04-08 13:55:50.000000 absql-0.6.1/absql/render/__init__.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.635800 absql-0.6.1/absql/text/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1596 2023-05-12 18:29:12.000000 absql-0.6.1/absql/text/__init__.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.636086 absql-0.6.1/absql/utils/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1218 2023-05-12 18:29:12.000000 absql-0.6.1/absql/utils/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)       38 2024-04-14 01:20:41.644110 absql-0.6.1/setup.cfg
--rw-r--r--   0 chriscardillo   (501) staff       (20)      846 2024-04-14 01:16:33.000000 absql-0.6.1/setup.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.641816 absql-0.6.1/tests/
--rw-r--r--   0 chriscardillo   (501) staff       (20)        0 2023-05-12 18:29:12.000000 absql-0.6.1/tests/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      814 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_copy.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2440 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_funcs_db.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      835 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_funcs_env.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      638 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_funcs_time.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      586 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_loader.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      923 2024-04-08 22:22:07.000000 absql-0.6.1/tests/test_parse_file.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1235 2024-01-03 15:38:53.000000 absql-0.6.1/tests/test_partial_kwargs.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2020 2024-01-03 15:37:15.000000 absql-0.6.1/tests/test_render.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     3865 2024-04-14 01:15:40.000000 absql-0.6.1/tests/test_render_file.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1393 2024-04-14 01:15:28.000000 absql-0.6.1/tests/test_render_file_return_dict.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2523 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_render_text.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      288 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_set.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      729 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_text.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1401 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_utils.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-21 15:24:03.049691 absql-0.6.2/
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-21 15:24:03.048902 absql-0.6.2/ABSQL.egg-info/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     9797 2024-04-21 15:24:03.000000 absql-0.6.2/ABSQL.egg-info/PKG-INFO
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      778 2024-04-21 15:24:03.000000 absql-0.6.2/ABSQL.egg-info/SOURCES.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)        1 2024-04-21 15:24:03.000000 absql-0.6.2/ABSQL.egg-info/dependency_links.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)       74 2024-04-21 15:24:03.000000 absql-0.6.2/ABSQL.egg-info/requires.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)       12 2024-04-21 15:24:03.000000 absql-0.6.2/ABSQL.egg-info/top_level.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1071 2023-05-12 18:29:12.000000 absql-0.6.2/LICENSE
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     9797 2024-04-21 15:24:03.049314 absql-0.6.2/PKG-INFO
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     9165 2024-02-09 23:11:51.000000 absql-0.6.2/README.md
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-21 15:24:03.035587 absql-0.6.2/absql/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     3157 2024-04-05 21:55:53.000000 absql-0.6.2/absql/__init__.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-21 15:24:03.037796 absql-0.6.2/absql/files/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      790 2024-04-06 14:26:22.000000 absql-0.6.2/absql/files/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2980 2024-01-03 15:38:53.000000 absql-0.6.2/absql/files/loader.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     4109 2024-04-21 15:23:37.000000 absql-0.6.2/absql/files/parsers.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-21 15:24:03.039799 absql-0.6.2/absql/functions/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      772 2023-05-12 18:29:12.000000 absql-0.6.2/absql/functions/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2331 2024-02-09 23:49:25.000000 absql-0.6.2/absql/functions/db.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      560 2023-05-12 18:29:12.000000 absql-0.6.2/absql/functions/env.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      350 2023-05-12 18:29:12.000000 absql-0.6.2/absql/functions/time.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-21 15:24:03.040420 absql-0.6.2/absql/render/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     3084 2024-04-08 13:55:50.000000 absql-0.6.2/absql/render/__init__.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-21 15:24:03.040920 absql-0.6.2/absql/text/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1596 2023-05-12 18:29:12.000000 absql-0.6.2/absql/text/__init__.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-21 15:24:03.041260 absql-0.6.2/absql/utils/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1218 2023-05-12 18:29:12.000000 absql-0.6.2/absql/utils/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)       38 2024-04-21 15:24:03.049785 absql-0.6.2/setup.cfg
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      846 2024-04-21 15:23:37.000000 absql-0.6.2/setup.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-21 15:24:03.048327 absql-0.6.2/tests/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)        0 2023-05-12 18:29:12.000000 absql-0.6.2/tests/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      814 2023-05-12 18:29:12.000000 absql-0.6.2/tests/test_copy.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2440 2023-05-12 18:29:12.000000 absql-0.6.2/tests/test_funcs_db.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      835 2023-05-12 18:29:12.000000 absql-0.6.2/tests/test_funcs_env.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      638 2023-05-12 18:29:12.000000 absql-0.6.2/tests/test_funcs_time.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      586 2023-05-12 18:29:12.000000 absql-0.6.2/tests/test_loader.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      923 2024-04-08 22:22:07.000000 absql-0.6.2/tests/test_parse_file.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1235 2024-01-03 15:38:53.000000 absql-0.6.2/tests/test_partial_kwargs.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2449 2024-04-21 15:23:37.000000 absql-0.6.2/tests/test_render.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     3865 2024-04-14 01:15:40.000000 absql-0.6.2/tests/test_render_file.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1393 2024-04-14 01:15:28.000000 absql-0.6.2/tests/test_render_file_return_dict.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2523 2023-05-12 18:29:12.000000 absql-0.6.2/tests/test_render_text.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      288 2023-05-12 18:29:12.000000 absql-0.6.2/tests/test_set.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      729 2023-05-12 18:29:12.000000 absql-0.6.2/tests/test_text.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1401 2023-05-12 18:29:12.000000 absql-0.6.2/tests/test_utils.py
```

### Comparing `absql-0.6.1/ABSQL.egg-info/PKG-INFO` & `absql-0.6.2/ABSQL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABSQL
-Version: 0.6.1
+Version: 0.6.2
 Summary: A rendering engine for templated SQL
 Home-page: https://github.com/pipeline-tools/ABSQL
 Author: Chris Cardillo
 Author-email: cfcardillo23@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `absql-0.6.1/ABSQL.egg-info/SOURCES.txt` & `absql-0.6.2/ABSQL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/LICENSE` & `absql-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/PKG-INFO` & `absql-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABSQL
-Version: 0.6.1
+Version: 0.6.2
 Summary: A rendering engine for templated SQL
 Home-page: https://github.com/pipeline-tools/ABSQL
 Author: Chris Cardillo
 Author-email: cfcardillo23@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `absql-0.6.1/README.md` & `absql-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/absql/__init__.py` & `absql-0.6.2/absql/__init__.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/absql/files/__init__.py` & `absql-0.6.2/absql/files/__init__.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/absql/files/loader.py` & `absql-0.6.2/absql/files/loader.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/absql/files/parsers.py` & `absql-0.6.2/absql/files/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             content = content.strip("\n")
         elif text.startswith("{"):
             tmp_header = "/*ABSQLQSBA*/ "
             text = tmp_header + text
             metadata = {}
             content = yaml.load(text, Loader=loader)
             content = content.replace(tmp_header, "")
-        elif text.startswith("/*") and file_path.endswith(".sql"):
+        elif text.startswith("/*") and file_path.endswith((".sql", ".js")):
             # Retrieve the first matched set of text within a block comment
             # (i.e. /* ... */).
             metadata = (
                 re.compile(r"^\/\*([\S\s]*?)\*\/$", re.MULTILINE).match(text).group(1)
             )
             # Text after the first block-comment end is considered the content of the
             # SQL file. This will handle block comments within the contents as well.
```

### Comparing `absql-0.6.1/absql/functions/__init__.py` & `absql-0.6.2/absql/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/absql/functions/db.py` & `absql-0.6.2/absql/functions/db.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/absql/functions/env.py` & `absql-0.6.2/absql/functions/env.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/absql/render/__init__.py` & `absql-0.6.2/absql/render/__init__.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/absql/text/__init__.py` & `absql-0.6.2/absql/text/__init__.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/absql/utils/__init__.py` & `absql-0.6.2/absql/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/setup.py` & `absql-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ABSQL",
-    version="0.6.1",
+    version="0.6.2",
     author="Chris Cardillo",
     author_email="cfcardillo23@gmail.com",
     description="A rendering engine for templated SQL",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pipeline-tools/ABSQL",
     packages=setuptools.find_packages(),
```

### Comparing `absql-0.6.1/tests/test_copy.py` & `absql-0.6.2/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/tests/test_funcs_db.py` & `absql-0.6.2/tests/test_funcs_db.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/tests/test_funcs_env.py` & `absql-0.6.2/tests/test_funcs_env.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/tests/test_funcs_time.py` & `absql-0.6.2/tests/test_funcs_time.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/tests/test_loader.py` & `absql-0.6.2/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/tests/test_parse_file.py` & `absql-0.6.2/tests/test_parse_file.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/tests/test_partial_kwargs.py` & `absql-0.6.2/tests/test_partial_kwargs.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/tests/test_render.py` & `absql-0.6.2/tests/test_render.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,23 +25,43 @@
 
 @pytest.fixture
 def simple_sql_path():
     return "tests/files/simple.sql"
 
 
 @pytest.fixture
+def simple_js_path():
+    return "tests/files/simple.js"
+
+
+@pytest.fixture
+def backticks_js_path():
+    return "tests/files/backticks.js"
+
+
+@pytest.fixture
 def no_frontmatter_path():
     return "tests/files/no_frontmatter.sql"
 
 
 def test_render_simple_sql(runner, simple_sql_path):
     sql = runner.render(simple_sql_path)
     assert sql == "SELECT * FROM my_table"
 
 
+def test_render_simple_js(runner, simple_js_path):
+    js = runner.render(simple_js_path)
+    assert js == "console.log('hello')"
+
+
+def test_render_backticks_js(runner, backticks_js_path):
+    js = runner.render(backticks_js_path)
+    assert js == "console.log(`hello`)"
+
+
 def test_render_no_frontmatter(runner, no_frontmatter_path):
     sql = runner.render(no_frontmatter_path)
     assert sql == "SELECT * FROM Hello"
 
 
 def test_render_text_only(runner):
     got = runner.render("{{greeting}}, {{env_var('name')}}!")
```

### Comparing `absql-0.6.1/tests/test_render_file.py` & `absql-0.6.2/tests/test_render_file.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/tests/test_render_file_return_dict.py` & `absql-0.6.2/tests/test_render_file_return_dict.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/tests/test_render_text.py` & `absql-0.6.2/tests/test_render_text.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/tests/test_text.py` & `absql-0.6.2/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `absql-0.6.1/tests/test_utils.py` & `absql-0.6.2/tests/test_utils.py`

 * *Files identical despite different names*


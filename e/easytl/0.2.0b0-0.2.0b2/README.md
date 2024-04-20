# Comparing `tmp/easytl-0.2.0b0.tar.gz` & `tmp/easytl-0.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytl-0.2.0b0.tar", last modified: Thu Apr 18 11:09:33 2024, max compression
+gzip compressed data, was "easytl-0.2.0b2.tar", last modified: Thu Apr 18 14:24:15 2024, max compression
```

## Comparing `easytl-0.2.0b0.tar` & `easytl-0.2.0b2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:09:33.839990 easytl-0.2.0b0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:09:33.831990 easytl-0.2.0b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:09:33.835990 easytl-0.2.0b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-18 11:09:20.000000 easytl-0.2.0b0/.github/workflows/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-18 11:09:20.000000 easytl-0.2.0b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-18 11:09:20.000000 easytl-0.2.0b0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-04-18 11:09:33.839990 easytl-0.2.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-04-18 11:09:20.000000 easytl-0.2.0b0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-18 11:09:20.000000 easytl-0.2.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 11:09:33.839990 easytl-0.2.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:09:33.835990 easytl-0.2.0b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:09:33.835990 easytl-0.2.0b0/src/easytl/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    11055 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/deepl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    49369 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/easytl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15958 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/gemini_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    17868 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/openai_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    22700 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:09:33.839990 easytl-0.2.0b0/src/easytl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-04-18 11:09:33.000000 easytl-0.2.0b0/src/easytl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-18 11:09:33.000000 easytl-0.2.0b0/src/easytl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:09:33.000000 easytl-0.2.0b0/src/easytl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 11:09:33.000000 easytl-0.2.0b0/src/easytl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 11:09:33.000000 easytl-0.2.0b0/src/easytl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:09:33.839990 easytl-0.2.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-18 11:09:20.000000 easytl-0.2.0b0/tests/issue_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-18 11:09:20.000000 easytl-0.2.0b0/tests/passing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:24:15.248703 easytl-0.2.0b2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:24:15.240702 easytl-0.2.0b2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:24:15.244703 easytl-0.2.0b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-18 14:22:45.000000 easytl-0.2.0b2/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-18 14:22:45.000000 easytl-0.2.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-18 14:22:45.000000 easytl-0.2.0b2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-04-18 14:24:15.248703 easytl-0.2.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-18 14:22:45.000000 easytl-0.2.0b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-18 14:22:45.000000 easytl-0.2.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:24:15.248703 easytl-0.2.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:24:15.240702 easytl-0.2.0b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:24:15.244703 easytl-0.2.0b2/src/easytl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11055 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/deepl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49369 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/easytl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15958 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/gemini_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17868 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/openai_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22700 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-18 14:22:45.000000 easytl-0.2.0b2/src/easytl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:24:15.248703 easytl-0.2.0b2/src/easytl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-04-18 14:24:15.000000 easytl-0.2.0b2/src/easytl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-18 14:24:15.000000 easytl-0.2.0b2/src/easytl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:24:15.000000 easytl-0.2.0b2/src/easytl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 14:24:15.000000 easytl-0.2.0b2/src/easytl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 14:24:15.000000 easytl-0.2.0b2/src/easytl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:24:15.248703 easytl-0.2.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-18 14:22:45.000000 easytl-0.2.0b2/tests/issue_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-18 14:22:45.000000 easytl-0.2.0b2/tests/passing.py
```

### Comparing `easytl-0.2.0b0/.gitignore` & `easytl-0.2.0b2/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -160,7 +160,8 @@
 #.idea/
 .vscode/settings.json
 
 ## test files
 tests/gemini.txt
 tests/openai.txt
 tests/deepl.txt
+tests/easytl-log.txt
```

### Comparing `easytl-0.2.0b0/LICENSE.md` & `easytl-0.2.0b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b0/PKG-INFO` & `easytl-0.2.0b2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.2.0b0
+Version: 0.2.0b2
 Summary: Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
 Author-email: Bikatr7 <Tetralon07@gmail.com>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: google-generativeai==0.5.1
 Requires-Dist: deepl==1.16.1
 Requires-Dist: openai==1.13.3
 Requires-Dist: backoff==2.2.1
 Requires-Dist: tiktoken==0.6.0
@@ -76,15 +74,15 @@
 
 ```
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Installation**<a name="installation"></a>
 
-Python 3.8+
+Python 3.10+
 
 EasyTL can be installed using pip:
 
 
 ```bash
 pip install easytl
 ```
```

### Comparing `easytl-0.2.0b0/README.md` & `easytl-0.2.0b2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 ```
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Installation**<a name="installation"></a>
 
-Python 3.8+
+Python 3.10+
 
 EasyTL can be installed using pip:
 
 
 ```bash
 pip install easytl
 ```
```

### Comparing `easytl-0.2.0b0/pyproject.toml` & `easytl-0.2.0b2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -14,24 +14,22 @@
     "deepl==1.16.1",
     "openai==1.13.3",
     "backoff==2.2.1",
     "tiktoken==0.6.0"
 ]
 
 name = "easytl"
-version = "v0.2.0-beta"
+version = "v0.2.0-beta-2"
 authors = [
   { name="Bikatr7", email="Tetralon07@gmail.com" },
 ]
 description = "Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 classifiers = [
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `easytl-0.2.0b0/src/easytl/__init__.py` & `easytl-0.2.0b2/src/easytl/__init__.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b0/src/easytl/classes.py` & `easytl-0.2.0b2/src/easytl/classes.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b0/src/easytl/decorators.py` & `easytl-0.2.0b2/src/easytl/decorators.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b0/src/easytl/deepl_service.py` & `easytl-0.2.0b2/src/easytl/deepl_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b0/src/easytl/easytl.py` & `easytl-0.2.0b2/src/easytl/easytl.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b0/src/easytl/exceptions.py` & `easytl-0.2.0b2/src/easytl/exceptions.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b0/src/easytl/gemini_service.py` & `easytl-0.2.0b2/src/easytl/gemini_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b0/src/easytl/openai_service.py` & `easytl-0.2.0b2/src/easytl/openai_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b0/src/easytl/util.py` & `easytl-0.2.0b2/src/easytl/util.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b0/src/easytl.egg-info/PKG-INFO` & `easytl-0.2.0b2/src/easytl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.2.0b0
+Version: 0.2.0b2
 Summary: Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
 Author-email: Bikatr7 <Tetralon07@gmail.com>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: google-generativeai==0.5.1
 Requires-Dist: deepl==1.16.1
 Requires-Dist: openai==1.13.3
 Requires-Dist: backoff==2.2.1
 Requires-Dist: tiktoken==0.6.0
@@ -76,15 +74,15 @@
 
 ```
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Installation**<a name="installation"></a>
 
-Python 3.8+
+Python 3.10+
 
 EasyTL can be installed using pip:
 
 
 ```bash
 pip install easytl
 ```
```

### Comparing `easytl-0.2.0b0/src/easytl.egg-info/SOURCES.txt` & `easytl-0.2.0b2/src/easytl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b0/tests/issue_template.py` & `easytl-0.2.0b2/tests/issue_template.py`

 * *Files identical despite different names*

### Comparing `easytl-0.2.0b0/tests/passing.py` & `easytl-0.2.0b2/tests/passing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,48 @@
 from easytl import EasyTL
 
 import asyncio
-
+import os
+import time
 
 def read_api_key(filename):
-    with open(filename, 'r') as file:
-        return file.read().strip()
+    try:
+        with open(filename, 'r') as file:
+            return file.read().strip()
+        
+    except:
+        pass
 
 async def main():
 
-    deepl_api_key = read_api_key('tests/deepl.txt')
-    gemini_api_key = read_api_key('tests/gemini.txt')
-    openai_api_key = read_api_key('tests/openai.txt')
+    gemini_time_delay = 30
+
+    deepl_api_key = os.environ.get('DEEPL_API_KEY')
+    gemini_api_key = os.environ.get('GEMINI_API_KEY')
+    openai_api_key = os.environ.get('OPENAI_API_KEY')
+
+    logging_directory = os.getenv('LOGGING_DIRECTORY', '/tmp/')
+
+    if(deepl_api_key is None):
+        deepl_api_key = read_api_key("tests/deepl.txt")
+    if(gemini_api_key is None):
+        gemini_api_key = read_api_key("tests/gemini.txt")
+    if(openai_api_key is None):
+        openai_api_key = read_api_key("tests/openai.txt")
+        
+        logging_directory = "tests/"
+
+    assert deepl_api_key is not None, "DEEPL_API_KEY environment variable must be set"
+    assert gemini_api_key is not None, "GEMINI_API_KEY environment variable must be set"
+    assert openai_api_key is not None, "OPENAI_API_KEY environment variable must be set"
 
     EasyTL.set_api_key("deepl", deepl_api_key)
     EasyTL.set_api_key("gemini", gemini_api_key)
     EasyTL.set_api_key("openai", openai_api_key)
 
-    logging_directory = "C:/Users/Tetra/Desktop/"
-
     print("Deepl ------------------------------------------------")
 
     print("Text response")
 
     print(EasyTL.deepl_translate("Hello, world!", target_lang="DE", logging_directory=logging_directory))
     print(await EasyTL.deepl_translate_async("Hello, world!", target_lang="DE", logging_directory=logging_directory))
     
@@ -64,14 +84,17 @@
 
     for result in async_results: # type: ignore
         print(result.text)
 
     print("JSON response")
 
     print(EasyTL.gemini_translate("Hello, world!", model="gemini-1.5-pro-latest", translation_instructions="Translate this to German. Format the response as JSON.", response_type="json", logging_directory=logging_directory))
+    
+    time.sleep(gemini_time_delay)
+    
     print(await EasyTL.gemini_translate_async("Hello, world!", model="gemini-1.5-pro-latest", translation_instructions="Format the response as JSON parseable string. It should have 2 keys, one for input titled input, and one called output, which is the translation.", response_type="json", logging_directory=logging_directory))
     
 
     print("OpenAI ------------------------------------------------")
 
     print("Text response")
```


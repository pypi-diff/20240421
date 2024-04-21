# Comparing `tmp/multillm-0.992.tar.gz` & `tmp/multillm-0.993.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multillm-0.992.tar", last modified: Fri Apr 19 07:17:51 2024, max compression
+gzip compressed data, was "multillm-0.993.tar", last modified: Sun Apr 21 19:55:52 2024, max compression
```

## Comparing `multillm-0.992.tar` & `multillm-0.993.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-19 07:17:51.641315 multillm-0.992/
--rw-r--r--   0 sandeep    (502) staff       (20)     1090 2024-04-19 07:14:31.000000 multillm-0.992/LICENSE
--rw-r--r--   0 sandeep    (502) staff       (20)    23984 2024-04-19 07:17:51.639586 multillm-0.992/PKG-INFO
--rw-r--r--   0 sandeep    (502) staff       (20)    23438 2024-04-19 07:14:31.000000 multillm-0.992/README.md
--rw-r--r--   0 sandeep    (502) staff       (20)      154 2024-04-19 07:14:31.000000 multillm-0.992/README.txt
-drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-19 07:17:51.619881 multillm-0.992/multillm/
--rw-r--r--   0 sandeep    (502) staff       (20)     2646 2024-04-19 07:14:31.000000 multillm-0.992/multillm/Action.py
--rw-r--r--   0 sandeep    (502) staff       (20)     3335 2024-04-19 07:14:31.000000 multillm-0.992/multillm/BaseLLM.py
--rw-r--r--   0 sandeep    (502) staff       (20)     3459 2024-04-19 07:14:31.000000 multillm-0.992/multillm/DynamicClass.py
--rw-r--r--   0 sandeep    (502) staff       (20)     9433 2024-04-19 07:14:31.000000 multillm-0.992/multillm/MultiLLM.py
--rw-r--r--   0 sandeep    (502) staff       (20)     3105 2024-04-19 07:14:31.000000 multillm-0.992/multillm/Prompt.py
--rw-r--r--   0 sandeep    (502) staff       (20)     2167 2024-04-19 07:14:31.000000 multillm-0.992/multillm/Rank.py
--rw-r--r--   0 sandeep    (502) staff       (20)     1209 2024-04-19 07:14:31.000000 multillm-0.992/multillm/Redis.py
--rw-r--r--   0 sandeep    (502) staff       (20)       26 2024-04-19 07:14:31.000000 multillm-0.992/multillm/__init__.py
--rw-r--r--   0 sandeep    (502) staff       (20)     5551 2024-04-19 07:14:31.000000 multillm-0.992/multillm/example.py
--rw-r--r--   0 sandeep    (502) staff       (20)     3491 2024-04-19 07:14:31.000000 multillm-0.992/multillm/example_rank_callback.py
--rw-r--r--   0 sandeep    (502) staff       (20)    12433 2024-04-19 07:14:31.000000 multillm-0.992/multillm/example_rank_callback3_scaled.py
-drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-19 07:17:51.636811 multillm-0.992/multillm/models/
--rw-r--r--   0 sandeep    (502) staff       (20)     4022 2024-04-19 07:14:31.000000 multillm-0.992/multillm/models/Codegen.py
--rw-r--r--   0 sandeep    (502) staff       (20)     3780 2024-04-19 07:14:31.000000 multillm-0.992/multillm/models/Dolly.py
--rw-r--r--   0 sandeep    (502) staff       (20)     4065 2024-04-19 07:14:31.000000 multillm-0.992/multillm/models/GPT.py
--rw-r--r--   0 sandeep    (502) staff       (20)     2519 2024-04-19 07:14:31.000000 multillm-0.992/multillm/models/GPTJ.py
--rw-r--r--   0 sandeep    (502) staff       (20)     5326 2024-04-19 07:14:31.000000 multillm-0.992/multillm/models/LLAMA2.py
--rw-r--r--   0 sandeep    (502) staff       (20)     5328 2024-04-19 07:16:39.000000 multillm-0.992/multillm/models/LLAMA3.py
--rw-r--r--   0 sandeep    (502) staff       (20)     4298 2024-04-19 07:14:31.000000 multillm-0.992/multillm/models/Mistral.py
--rw-r--r--   0 sandeep    (502) staff       (20)     4474 2024-04-19 07:14:31.000000 multillm-0.992/multillm/models/Zephyr.py
--rw-r--r--   0 sandeep    (502) staff       (20)     6399 2024-04-19 07:14:31.000000 multillm-0.992/multillm/models/bard.py
--rw-r--r--   0 sandeep    (502) staff       (20)     5513 2024-04-19 07:14:31.000000 multillm-0.992/multillm/models/claude.py
--rw-r--r--   0 sandeep    (502) staff       (20)     4026 2024-04-19 07:14:31.000000 multillm-0.992/multillm/models/gemini.py
--rw-r--r--   0 sandeep    (502) staff       (20)    12554 2024-04-19 07:14:31.000000 multillm-0.992/multillm/rank_callback.py
-drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-19 07:17:51.637662 multillm-0.992/multillm.egg-info/
--rw-r--r--   0 sandeep    (502) staff       (20)    23984 2024-04-19 07:17:51.000000 multillm-0.992/multillm.egg-info/PKG-INFO
--rw-r--r--   0 sandeep    (502) staff       (20)      768 2024-04-19 07:17:51.000000 multillm-0.992/multillm.egg-info/SOURCES.txt
--rw-r--r--   0 sandeep    (502) staff       (20)        1 2024-04-19 07:17:51.000000 multillm-0.992/multillm.egg-info/dependency_links.txt
--rw-r--r--   0 sandeep    (502) staff       (20)       51 2024-04-19 07:17:51.000000 multillm-0.992/multillm.egg-info/entry_points.txt
--rw-r--r--   0 sandeep    (502) staff       (20)        9 2024-04-19 07:17:51.000000 multillm-0.992/multillm.egg-info/top_level.txt
--rw-r--r--   0 sandeep    (502) staff       (20)      946 2024-04-19 07:14:43.000000 multillm-0.992/pyproject.toml
--rw-r--r--   0 sandeep    (502) staff       (20)       38 2024-04-19 07:17:51.641543 multillm-0.992/setup.cfg
+drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-21 19:55:52.164436 multillm-0.993/
+-rw-r--r--   0 sandeep    (502) staff       (20)     1090 2024-04-19 07:14:31.000000 multillm-0.993/LICENSE
+-rw-r--r--   0 sandeep    (502) staff       (20)    23984 2024-04-21 19:55:52.163587 multillm-0.993/PKG-INFO
+-rw-r--r--   0 sandeep    (502) staff       (20)    23438 2024-04-19 07:14:31.000000 multillm-0.993/README.md
+-rw-r--r--   0 sandeep    (502) staff       (20)      154 2024-04-19 07:14:31.000000 multillm-0.993/README.txt
+drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-21 19:55:52.142106 multillm-0.993/multillm/
+-rw-r--r--   0 sandeep    (502) staff       (20)     2646 2024-04-19 07:14:31.000000 multillm-0.993/multillm/Action.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     3335 2024-04-19 07:14:31.000000 multillm-0.993/multillm/BaseLLM.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     3459 2024-04-19 07:14:31.000000 multillm-0.993/multillm/DynamicClass.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     9433 2024-04-19 07:14:31.000000 multillm-0.993/multillm/MultiLLM.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     3105 2024-04-19 07:14:31.000000 multillm-0.993/multillm/Prompt.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     2167 2024-04-19 07:14:31.000000 multillm-0.993/multillm/Rank.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     1209 2024-04-19 07:14:31.000000 multillm-0.993/multillm/Redis.py
+-rw-r--r--   0 sandeep    (502) staff       (20)       26 2024-04-19 07:14:31.000000 multillm-0.993/multillm/__init__.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     5551 2024-04-19 07:14:31.000000 multillm-0.993/multillm/example.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     3491 2024-04-19 07:14:31.000000 multillm-0.993/multillm/example_rank_callback.py
+-rw-r--r--   0 sandeep    (502) staff       (20)    12433 2024-04-19 07:14:31.000000 multillm-0.993/multillm/example_rank_callback3_scaled.py
+drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-21 19:55:52.162365 multillm-0.993/multillm/models/
+-rw-r--r--   0 sandeep    (502) staff       (20)     4022 2024-04-19 07:14:31.000000 multillm-0.993/multillm/models/Codegen.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     3780 2024-04-19 07:14:31.000000 multillm-0.993/multillm/models/Dolly.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     4065 2024-04-19 07:14:31.000000 multillm-0.993/multillm/models/GPT.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     2519 2024-04-19 07:14:31.000000 multillm-0.993/multillm/models/GPTJ.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     5326 2024-04-19 07:14:31.000000 multillm-0.993/multillm/models/LLAMA2.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     5348 2024-04-19 18:07:35.000000 multillm-0.993/multillm/models/LLAMA3.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     4298 2024-04-19 07:14:31.000000 multillm-0.993/multillm/models/Mistral.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     4474 2024-04-19 07:14:31.000000 multillm-0.993/multillm/models/Zephyr.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     6399 2024-04-19 07:14:31.000000 multillm-0.993/multillm/models/bard.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     5513 2024-04-19 07:14:31.000000 multillm-0.993/multillm/models/claude.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     4026 2024-04-19 07:14:31.000000 multillm-0.993/multillm/models/gemini.py
+-rw-r--r--   0 sandeep    (502) staff       (20)    12554 2024-04-19 07:14:31.000000 multillm-0.993/multillm/rank_callback.py
+drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-21 19:55:52.163041 multillm-0.993/multillm.egg-info/
+-rw-r--r--   0 sandeep    (502) staff       (20)    23984 2024-04-21 19:55:52.000000 multillm-0.993/multillm.egg-info/PKG-INFO
+-rw-r--r--   0 sandeep    (502) staff       (20)      768 2024-04-21 19:55:52.000000 multillm-0.993/multillm.egg-info/SOURCES.txt
+-rw-r--r--   0 sandeep    (502) staff       (20)        1 2024-04-21 19:55:52.000000 multillm-0.993/multillm.egg-info/dependency_links.txt
+-rw-r--r--   0 sandeep    (502) staff       (20)       51 2024-04-21 19:55:52.000000 multillm-0.993/multillm.egg-info/entry_points.txt
+-rw-r--r--   0 sandeep    (502) staff       (20)        9 2024-04-21 19:55:52.000000 multillm-0.993/multillm.egg-info/top_level.txt
+-rw-r--r--   0 sandeep    (502) staff       (20)      946 2024-04-21 19:54:53.000000 multillm-0.993/pyproject.toml
+-rw-r--r--   0 sandeep    (502) staff       (20)       38 2024-04-21 19:55:52.164680 multillm-0.993/setup.cfg
```

### Comparing `multillm-0.992/LICENSE` & `multillm-0.993/LICENSE`

 * *Files identical despite different names*

### Comparing `multillm-0.992/PKG-INFO` & `multillm-0.993/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multillm
-Version: 0.992
+Version: 0.993
 Summary: VerifAI MultiLLM: A module to invoke multiple LLMs concurrently and rank their results
 Author-email: VerifAI Inc <hello@verifai.ai>
 Project-URL: Homepage, https://github.com/verifai/multiLLM
 Project-URL: Bug Tracker, https://github.com/verifai/multiLLM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multillm-0.992/README.md` & `multillm-0.993/README.md`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/Action.py` & `multillm-0.993/multillm/Action.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/BaseLLM.py` & `multillm-0.993/multillm/BaseLLM.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/DynamicClass.py` & `multillm-0.993/multillm/DynamicClass.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/MultiLLM.py` & `multillm-0.993/multillm/MultiLLM.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/Prompt.py` & `multillm-0.993/multillm/Prompt.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/Rank.py` & `multillm-0.993/multillm/Rank.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/Redis.py` & `multillm-0.993/multillm/Redis.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/example.py` & `multillm-0.993/multillm/example.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/example_rank_callback.py` & `multillm-0.993/multillm/example_rank_callback.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/example_rank_callback3_scaled.py` & `multillm-0.993/multillm/example_rank_callback3_scaled.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/models/Codegen.py` & `multillm-0.993/multillm/models/Codegen.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/models/Dolly.py` & `multillm-0.993/multillm/models/Dolly.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/models/GPT.py` & `multillm-0.993/multillm/models/GPT.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/models/GPTJ.py` & `multillm-0.993/multillm/models/GPTJ.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/models/LLAMA2.py` & `multillm-0.993/multillm/models/LLAMA2.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/models/LLAMA3.py` & `multillm-0.993/multillm/models/LLAMA3.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,18 +97,18 @@
                 cntx = "<<SYS>>" + prompt.get_context() +"<</SYS>>"
                 cntx += "\n" + prmpt
                 prmpt = cntx
             #values = {'question':  prmpt}
 
             """ vllm server
         http://54.190.15.83/llama2-vllm     -H "Content-Type: application/json"
-           -d '{ "model": "meta-llama/Llama-2-7b-chat-hf", "prompt": "write verilog code for a 4 port 16 entry FIFO controllers", "max_tokens":4096}'
+           -d '{ "model": "meta-llama/Meta-Llama-3-8B-Instruct-chat-hf", "prompt": "write verilog code for a 4 port 16 entry FIFO controllers", "max_tokens":4096}'
 
             """
-            values = {'prompt':  prmpt, "model" : "meta-llama/Llama-2-7b-chat-hf", "max_tokens":4096}
+            values = {'prompt':  prmpt, "model" : "meta-llama/Meta-Llama-3-8B-Instruct", "max_tokens":4096}
       
             resp = requests.post(url, data=json.dumps(values),headers=headers)
             #print("LLAMA2 Response: {0}" .format(resp.text))
             data = resp.json()
 
             """ GPT Style Response from vLLM server
               {"id":"cmpl-8282910626ff42518fb0e17f01c412f7",
```

### Comparing `multillm-0.992/multillm/models/Mistral.py` & `multillm-0.993/multillm/models/Mistral.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/models/Zephyr.py` & `multillm-0.993/multillm/models/Zephyr.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/models/bard.py` & `multillm-0.993/multillm/models/bard.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/models/claude.py` & `multillm-0.993/multillm/models/claude.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/models/gemini.py` & `multillm-0.993/multillm/models/gemini.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm/rank_callback.py` & `multillm-0.993/multillm/rank_callback.py`

 * *Files identical despite different names*

### Comparing `multillm-0.992/multillm.egg-info/PKG-INFO` & `multillm-0.993/multillm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multillm
-Version: 0.992
+Version: 0.993
 Summary: VerifAI MultiLLM: A module to invoke multiple LLMs concurrently and rank their results
 Author-email: VerifAI Inc <hello@verifai.ai>
 Project-URL: Homepage, https://github.com/verifai/multiLLM
 Project-URL: Bug Tracker, https://github.com/verifai/multiLLM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multillm-0.992/multillm.egg-info/SOURCES.txt` & `multillm-0.993/multillm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multillm-0.992/pyproject.toml` & `multillm-0.993/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "multillm"
-version = "0.992"
+version = "0.993"
 authors = [
   { name="VerifAI Inc", email="hello@verifai.ai" },
 ]
 
 description = "VerifAI MultiLLM: A module to invoke multiple LLMs concurrently and rank their results"
 readme = "README.md"
 requires-python = ">=3.8"
```


# Comparing `tmp/tool_use-0.1.1rc5.tar.gz` & `tmp/tool_use-0.1.1rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tool_use-0.1.1rc5.tar", last modified: Mon Apr 15 15:52:45 2024, max compression
+gzip compressed data, was "tool_use-0.1.1rc6.tar", last modified: Wed Apr 17 06:08:38 2024, max compression
```

## Comparing `tool_use-0.1.1rc5.tar` & `tool_use-0.1.1rc6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 15:52:45.943364 tool_use-0.1.1rc5/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       30 2024-03-17 15:07:20.000000 tool_use-0.1.1rc5/MANIFEST.in
--rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-04-15 15:52:45.943124 tool_use-0.1.1rc5/PKG-INFO
--rw-r--r--   0 kimjaemin   (501) staff       (20)      370 2024-04-14 06:28:02.000000 tool_use-0.1.1rc5/README.md
--rw-r--r--   0 kimjaemin   (501) staff       (20)      532 2024-04-14 06:26:15.000000 tool_use-0.1.1rc5/pyproject.toml
--rw-r--r--   0 kimjaemin   (501) staff       (20)       38 2024-04-15 15:52:45.943425 tool_use-0.1.1rc5/setup.cfg
--rw-r--r--   0 kimjaemin   (501) staff       (20)      530 2024-04-15 15:52:40.000000 tool_use-0.1.1rc5/setup.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 15:52:45.939426 tool_use-0.1.1rc5/tests/
--rw-r--r--   0 kimjaemin   (501) staff       (20)        0 2024-02-06 11:51:51.000000 tool_use-0.1.1rc5/tests/__init__.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     4507 2024-04-15 15:34:11.000000 tool_use-0.1.1rc5/tests/test_anthropic_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1235 2024-04-08 11:36:45.000000 tool_use-0.1.1rc5/tests/test_exception.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1016 2024-04-14 05:56:49.000000 tool_use-0.1.1rc5/tests/test_openai_tool_use.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 15:52:45.939585 tool_use-0.1.1rc5/tool_use/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.1rc5/tool_use/__init__.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 15:52:45.941891 tool_use-0.1.1rc5/tool_use/tools/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.1rc5/tool_use/tools/__init__.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)    17897 2024-04-15 15:46:00.000000 tool_use-0.1.1rc5/tool_use/tools/anthropic_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)    22455 2024-04-14 06:13:17.000000 tool_use-0.1.1rc5/tool_use/tools/openai_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)      537 2024-03-17 15:07:20.000000 tool_use-0.1.1rc5/tool_use/tools/utils.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 15:52:45.942574 tool_use-0.1.1rc5/tool_use/yamls/
--rw-r--r--   0 kimjaemin   (501) staff       (20)      909 2024-04-15 14:13:42.000000 tool_use-0.1.1rc5/tool_use/yamls/anthropic_tool_use.yaml
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1512 2024-04-08 11:29:56.000000 tool_use-0.1.1rc5/tool_use/yamls/openai_tool_use.yaml
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-15 15:52:45.942800 tool_use-0.1.1rc5/tool_use.egg-info/
--rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-04-15 15:52:45.000000 tool_use-0.1.1rc5/tool_use.egg-info/PKG-INFO
--rw-r--r--   0 kimjaemin   (501) staff       (20)      531 2024-04-15 15:52:45.000000 tool_use-0.1.1rc5/tool_use.egg-info/SOURCES.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)        1 2024-04-15 15:52:45.000000 tool_use-0.1.1rc5/tool_use.egg-info/dependency_links.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)      135 2024-04-15 15:52:45.000000 tool_use-0.1.1rc5/tool_use.egg-info/entry_points.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)       15 2024-04-15 15:52:45.000000 tool_use-0.1.1rc5/tool_use.egg-info/top_level.txt
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-17 06:08:38.031640 tool_use-0.1.1rc6/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       30 2024-03-17 15:07:20.000000 tool_use-0.1.1rc6/MANIFEST.in
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-04-17 06:08:38.031381 tool_use-0.1.1rc6/PKG-INFO
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      370 2024-04-14 06:28:02.000000 tool_use-0.1.1rc6/README.md
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      532 2024-04-14 06:26:15.000000 tool_use-0.1.1rc6/pyproject.toml
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       38 2024-04-17 06:08:38.031699 tool_use-0.1.1rc6/setup.cfg
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      530 2024-04-17 06:08:05.000000 tool_use-0.1.1rc6/setup.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-17 06:08:38.027573 tool_use-0.1.1rc6/tests/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)        0 2024-02-06 11:51:51.000000 tool_use-0.1.1rc6/tests/__init__.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     4967 2024-04-17 05:56:16.000000 tool_use-0.1.1rc6/tests/test_anthropic_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1235 2024-04-08 11:36:45.000000 tool_use-0.1.1rc6/tests/test_exception.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1016 2024-04-14 05:56:49.000000 tool_use-0.1.1rc6/tests/test_openai_tool_use.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-17 06:08:38.027720 tool_use-0.1.1rc6/tool_use/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.1rc6/tool_use/__init__.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-17 06:08:38.030265 tool_use-0.1.1rc6/tool_use/tools/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.1rc6/tool_use/tools/__init__.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)    17883 2024-04-16 11:57:24.000000 tool_use-0.1.1rc6/tool_use/tools/anthropic_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)    22455 2024-04-14 06:13:17.000000 tool_use-0.1.1rc6/tool_use/tools/openai_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      537 2024-03-17 15:07:20.000000 tool_use-0.1.1rc6/tool_use/tools/utils.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-17 06:08:38.030850 tool_use-0.1.1rc6/tool_use/yamls/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      909 2024-04-15 14:13:42.000000 tool_use-0.1.1rc6/tool_use/yamls/anthropic_tool_use.yaml
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1512 2024-04-08 11:29:56.000000 tool_use-0.1.1rc6/tool_use/yamls/openai_tool_use.yaml
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-17 06:08:38.031070 tool_use-0.1.1rc6/tool_use.egg-info/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      109 2024-04-17 06:08:37.000000 tool_use-0.1.1rc6/tool_use.egg-info/PKG-INFO
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      531 2024-04-17 06:08:37.000000 tool_use-0.1.1rc6/tool_use.egg-info/SOURCES.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)        1 2024-04-17 06:08:37.000000 tool_use-0.1.1rc6/tool_use.egg-info/dependency_links.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      135 2024-04-17 06:08:37.000000 tool_use-0.1.1rc6/tool_use.egg-info/entry_points.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       15 2024-04-17 06:08:37.000000 tool_use-0.1.1rc6/tool_use.egg-info/top_level.txt
```

### Comparing `tool_use-0.1.1rc5/pyproject.toml` & `tool_use-0.1.1rc6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc5/setup.py` & `tool_use-0.1.1rc6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 PACKAGE_NAME = "tool_use"
 
 setup(
     name=PACKAGE_NAME,
-    version="0.1.1rc5",
+    version="0.1.1rc6",
     description="Promptflow tool package for OpenAI/Anthropic",
     packages=find_packages(),
     entry_points={
         "package_tools": [
             "openai_tool_use = tool_use.tools.utils:list_package_tools",
             "anthropic_tool_use = tool_use.tools.utils:list_package_tools",
         ],
```

### Comparing `tool_use-0.1.1rc5/tests/test_anthropic_tool_use.py` & `tool_use-0.1.1rc6/tests/test_anthropic_tool_use.py`

 * *Files 22% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 @pytest_asyncio.fixture
 def my_custom_connection(load_env) -> AnthropicConnection:
     return AnthropicConnection(
         secrets=dict(
             api_key=os.environ.get("ANTHROPIC_API_KEY"),
             api_type="anthropic",
             api_base=os.environ.get("ANTHROPIC_API_BASE"),
+            client_key=None,
         ),
     )
 
 
 def load_tool_prompts() -> Tuple[str, dict]:
     prompt = ""
     with open(
@@ -102,57 +103,64 @@
             stream=True,
             question="I want to make a recipe with chicken.",
         )
         chunk_count = 0
         total_result = ""
         async for chunk in result:
             chunk_count += 1
-            total_result += chunk
+            if hasattr(chunk, "delta") and hasattr(chunk.delta, "text"):
+                total_result += chunk.delta.text
+        # raise Exception("This test is not working as expected")
         print(chunk_count)
         print(total_result)
 
     async def test_anthropic_tool_use_2(self, my_custom_connection):
         prompt, sample_tool = load_tool_prompts()
         result = await anthropic_tool_use(
             connection=my_custom_connection,
             prompt=prompt,
-            model="claude-3-haiku-20240307",
+            model="anthropic.claude-3-haiku-20240307-v1:0",
             max_tokens=500,
             tools=[sample_tool],
+            stream=False,
         )
         assert result is not None
         print(result)
 
     async def test_anthropic_2(self, my_custom_connection):
         prompt = load_prompt()
         result = await anthropic_tool_use(
             connection=my_custom_connection,
             prompt=prompt,
-            model="claude-3-haiku-20240307",
+            model="anthropic.claude-3-haiku-20240307-v1:0",
             max_tokens=500,
             question="I want to make a recipe with chicken.",
+            stream=False,
         )
         assert result is not None
         print(result)
 
     async def test_anthropic_stream_2(self, my_custom_connection):
         prompt = load_prompt()
         result = await anthropic_tool_use(
             connection=my_custom_connection,
             prompt=prompt,
-            model="claude-3-haiku-20240307",
+            model="anthropic.claude-3-haiku-20240307-v1:0",
             max_tokens=500,
             stream=True,
             question="I want to make a recipe with chicken.",
         )
         chunk_count = 0
         total_result = ""
+        total_result = ""
         async for chunk in result:
             chunk_count += 1
-            total_result += chunk
+            if hasattr(chunk, "delta") and hasattr(chunk.delta, "text"):
+                total_result += chunk.delta.text
+        # raise Exception("This test is not working as expected")
         print(chunk_count)
         print(total_result)
 
 
 # Run the unit tests
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `tool_use-0.1.1rc5/tests/test_exception.py` & `tool_use-0.1.1rc6/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc5/tests/test_openai_tool_use.py` & `tool_use-0.1.1rc6/tests/test_openai_tool_use.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc5/tool_use/tools/anthropic_tool_use.py` & `tool_use-0.1.1rc6/tool_use/tools/anthropic_tool_use.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,20 +370,19 @@
         if functions is not None:
             error_message = (
                 "Function calling has not been supported by stream mode yet."
             )
             raise FunctionCallNotSupportedInStreamMode(message=error_message)
 
         async def generator():
-            assert isinstance(
-                completion, AsyncMessageStreamManager
-            ), "Invalid type. Expected AsyncMessageStreamManager."
-            async with completion as stream:
-                async for chunk in stream.text_stream:
-                    yield chunk
+            # assert isinstance(
+            #     completion, AsyncMessageStreamManager
+            # ), "Invalid type. Expected AsyncMessageStreamManager."
+            async for chunk in completion:
+                yield chunk
 
         return generator()
     else:
         assert isinstance(completion, Message) or isinstance(
             completion, ToolsBetaMessage
         ), "Invalid type. Expected Message."
         # When calling function, function_call response will be returned as a field in message, so we need return
@@ -459,27 +458,28 @@
     elif connection.api_type == "vertex_anthropic":
         _client = AnthropicVertexClient(**_connection_dict)
     elif connection.api_type == "bedrock_anthropic":
         _client = AnthropicBedrockClient(**_connection_dict)
 
     if tools:
         if stream:
-            response = _client.beta.tools.messages.stream(
+            response = await _client.beta.tools.messages.stream(
                 **params,
                 extra_headers=extra_headers,
             )
         else:
             response = await _client.beta.tools.messages.create(
                 **params,
                 extra_headers=extra_headers,
             )
     else:
         if stream:
-            response = _client.messages.stream(
+            response = await _client.messages.create(
                 **params,
+                stream=True,
                 extra_headers=extra_headers,
             )
         else:
             response = await _client.messages.create(
                 **params,
                 extra_headers=extra_headers,
             )
```

### Comparing `tool_use-0.1.1rc5/tool_use/tools/openai_tool_use.py` & `tool_use-0.1.1rc6/tool_use/tools/openai_tool_use.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc5/tool_use/tools/utils.py` & `tool_use-0.1.1rc6/tool_use/tools/utils.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc5/tool_use/yamls/anthropic_tool_use.yaml` & `tool_use-0.1.1rc6/tool_use/yamls/anthropic_tool_use.yaml`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc5/tool_use/yamls/openai_tool_use.yaml` & `tool_use-0.1.1rc6/tool_use/yamls/openai_tool_use.yaml`

 * *Files identical despite different names*

### Comparing `tool_use-0.1.1rc5/tool_use.egg-info/SOURCES.txt` & `tool_use-0.1.1rc6/tool_use.egg-info/SOURCES.txt`

 * *Files identical despite different names*


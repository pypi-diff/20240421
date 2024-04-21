# Comparing `tmp/LLMEasyTools-0.6.tar.gz` & `tmp/LLMEasyTools-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LLMEasyTools-0.6.tar", last modified: Thu Apr 18 06:56:55 2024, max compression
+gzip compressed data, was "LLMEasyTools-0.7.tar", last modified: Sun Apr 21 17:28:28 2024, max compression
```

## Comparing `LLMEasyTools-0.6.tar` & `LLMEasyTools-0.7.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-18 06:56:55.603600 LLMEasyTools-0.6/
--rw-rw-r--   0 zby       (1000) zby       (1000)    11357 2024-03-03 11:08:50.000000 LLMEasyTools-0.6/LICENSE
-drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-18 06:56:55.603600 LLMEasyTools-0.6/LLMEasyTools.egg-info/
--rw-r--r--   0 zby       (1000) zby       (1000)    16948 2024-04-18 06:56:55.000000 LLMEasyTools-0.6/LLMEasyTools.egg-info/PKG-INFO
--rw-rw-r--   0 zby       (1000) zby       (1000)      407 2024-04-18 06:56:55.000000 LLMEasyTools-0.6/LLMEasyTools.egg-info/SOURCES.txt
--rw-rw-r--   0 zby       (1000) zby       (1000)        1 2024-04-18 06:56:55.000000 LLMEasyTools-0.6/LLMEasyTools.egg-info/dependency_links.txt
--rw-rw-r--   0 zby       (1000) zby       (1000)       54 2024-04-18 06:56:55.000000 LLMEasyTools-0.6/LLMEasyTools.egg-info/requires.txt
--rw-rw-r--   0 zby       (1000) zby       (1000)       15 2024-04-18 06:56:55.000000 LLMEasyTools-0.6/LLMEasyTools.egg-info/top_level.txt
--rw-rw-r--   0 zby       (1000) zby       (1000)       67 2024-03-03 11:08:50.000000 LLMEasyTools-0.6/MANIFEST.in
--rw-r--r--   0 zby       (1000) zby       (1000)    16948 2024-04-18 06:56:55.603600 LLMEasyTools-0.6/PKG-INFO
--rw-rw-r--   0 zby       (1000) zby       (1000)     3202 2024-03-04 13:15:40.000000 LLMEasyTools-0.6/README.md
-drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-18 06:56:55.603600 LLMEasyTools-0.6/examples/
--rw-rw-r--   0 zby       (1000) zby       (1000)     1290 2024-03-05 07:21:59.000000 LLMEasyTools-0.6/examples/extract_user_details.py
--rw-rw-r--   0 zby       (1000) zby       (1000)      863 2024-03-05 07:22:09.000000 LLMEasyTools-0.6/examples/extract_user_details_by_function.py
--rw-rw-r--   0 zby       (1000) zby       (1000)     3360 2024-03-05 07:22:24.000000 LLMEasyTools-0.6/examples/stateful_search.py
-drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-18 06:56:55.603600 LLMEasyTools-0.6/llm_easy_tools/
--rw-rw-r--   0 zby       (1000) zby       (1000)    14944 2024-04-18 06:46:53.000000 LLMEasyTools-0.6/llm_easy_tools/__init__.py
--rw-rw-r--   0 zby       (1000) zby       (1000)      988 2024-04-18 05:41:21.000000 LLMEasyTools-0.6/pyproject.toml
--rw-rw-r--   0 zby       (1000) zby       (1000)       38 2024-04-18 06:56:55.603600 LLMEasyTools-0.6/setup.cfg
-drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-18 06:56:55.603600 LLMEasyTools-0.6/tests/
--rw-rw-r--   0 zby       (1000) zby       (1000)     7838 2024-03-20 22:48:41.000000 LLMEasyTools-0.6/tests/schema_generator_test.py
--rw-rw-r--   0 zby       (1000) zby       (1000)     9872 2024-04-18 06:48:39.000000 LLMEasyTools-0.6/tests/tools_test.py
+drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-21 17:28:28.172522 LLMEasyTools-0.7/
+-rw-rw-r--   0 zby       (1000) zby       (1000)    11357 2024-03-03 11:08:50.000000 LLMEasyTools-0.7/LICENSE
+drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-21 17:28:28.172522 LLMEasyTools-0.7/LLMEasyTools.egg-info/
+-rw-r--r--   0 zby       (1000) zby       (1000)    16954 2024-04-21 17:28:28.000000 LLMEasyTools-0.7/LLMEasyTools.egg-info/PKG-INFO
+-rw-rw-r--   0 zby       (1000) zby       (1000)      454 2024-04-21 17:28:28.000000 LLMEasyTools-0.7/LLMEasyTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 zby       (1000) zby       (1000)        1 2024-04-21 17:28:28.000000 LLMEasyTools-0.7/LLMEasyTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 zby       (1000) zby       (1000)       67 2024-04-21 17:28:28.000000 LLMEasyTools-0.7/LLMEasyTools.egg-info/requires.txt
+-rw-rw-r--   0 zby       (1000) zby       (1000)       15 2024-04-21 17:28:28.000000 LLMEasyTools-0.7/LLMEasyTools.egg-info/top_level.txt
+-rw-rw-r--   0 zby       (1000) zby       (1000)       67 2024-03-03 11:08:50.000000 LLMEasyTools-0.7/MANIFEST.in
+-rw-r--r--   0 zby       (1000) zby       (1000)    16954 2024-04-21 17:28:28.172522 LLMEasyTools-0.7/PKG-INFO
+-rw-rw-r--   0 zby       (1000) zby       (1000)     3153 2024-04-21 17:27:50.000000 LLMEasyTools-0.7/README.md
+drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-21 17:28:28.172522 LLMEasyTools-0.7/examples/
+-rw-rw-r--   0 zby       (1000) zby       (1000)     1336 2024-04-20 07:38:54.000000 LLMEasyTools-0.7/examples/extract_user_details.py
+-rw-rw-r--   0 zby       (1000) zby       (1000)     3331 2024-04-20 07:38:54.000000 LLMEasyTools-0.7/examples/stateful_search.py
+drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-21 17:28:28.172522 LLMEasyTools-0.7/llm_easy_tools/
+-rw-rw-r--   0 zby       (1000) zby       (1000)      120 2024-04-20 09:54:59.000000 LLMEasyTools-0.7/llm_easy_tools/__init__.py
+-rw-rw-r--   0 zby       (1000) zby       (1000)     4822 2024-04-20 07:38:54.000000 LLMEasyTools-0.7/llm_easy_tools/schema_generator.py
+-rw-rw-r--   0 zby       (1000) zby       (1000)     8312 2024-04-20 14:37:35.000000 LLMEasyTools-0.7/llm_easy_tools/tool_box.py
+-rw-rw-r--   0 zby       (1000) zby       (1000)     1041 2024-04-20 10:32:01.000000 LLMEasyTools-0.7/pyproject.toml
+-rw-rw-r--   0 zby       (1000) zby       (1000)       38 2024-04-21 17:28:28.172522 LLMEasyTools-0.7/setup.cfg
+drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-21 17:28:28.172522 LLMEasyTools-0.7/tests/
+-rw-rw-r--   0 zby       (1000) zby       (1000)      737 2024-04-20 07:38:54.000000 LLMEasyTools-0.7/tests/message_construction.py
+-rw-rw-r--   0 zby       (1000) zby       (1000)     4982 2024-04-20 07:38:54.000000 LLMEasyTools-0.7/tests/schema_generator_test.py
+-rw-rw-r--   0 zby       (1000) zby       (1000)     8002 2024-04-20 14:40:16.000000 LLMEasyTools-0.7/tests/tools_test.py
```

### Comparing `LLMEasyTools-0.6/LICENSE` & `LLMEasyTools-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `LLMEasyTools-0.6/LLMEasyTools.egg-info/PKG-INFO` & `LLMEasyTools-0.7/LLMEasyTools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: LLMEasyTools
-Version: 0.6
+Version: 0.7
 Summary: OpenAI tools and functions with no fuss.
+Author: Natalia Borovskikh
 Author-email: Zbigniew Łukasiak <zzbbyy@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -213,14 +214,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic
 Requires-Dist: docstring_parser~=0.15
+Requires-Dist: openai~=1.23
 Provides-Extra: test
 Requires-Dist: pytest~=7.4.4; extra == "test"
 
 # LLMEasyTools
 **OpenAI tools and functions with no fuss.**
 
 LLMEasyTool is a minimal Python package designed for seamless interaction with 
@@ -231,15 +233,15 @@
 It doesn't take over the interaction with the OpenAI client, making it easier for developers
 to debug their code and optimize the communication with the LLM.
 
 By integrating Pydantic, LLMEasyTools ensures robust data validation and schema generation.
 
 ## Features
 
-- **Schema Generation**: Effortlessly create JSON schemas for tools using Pydantic models.
+- **Schema Generation**: Effortlessly create JSON schemas for tools from type annotations
 - **Structured Data from LLM**
 - **Function Name Mapping**: Flexibly map JSON schema names to Python code.
 - **Dispatching Function Calls**: Directly invoke functions based on LLM response structures.
 - **Stateful Tools**: You can register methods bound to an object to have stateful tools. See [examples/stateful_search.py](https://github.com/zby/LLMEasyTools/tree/main/examples)
 - **No Patching!**: No globals, some 200 lines of straightforward object oriented code.
 
 ## Installation
@@ -254,79 +256,77 @@
 cd LLMEasyTools
 pip install -e .
 pytest -v tests
 ```
 
 ## Usage
 
-### Basic Example: Getting structured data from LLM
+### Basic Example: Dispatching to a function
 
 ```python
 from llm_easy_tools import ToolBox
 from pydantic import BaseModel
 from openai import OpenAI
 from pprint import pprint
 
 client = OpenAI()
 
-
-# Define a Pydantic model for your tool's input
-class UserDetail(BaseModel):
-    name: str
-    city: str
-
-
 # Create a ToolBox instance
 toolbox = ToolBox()
 
-# Register your tool - if a class is passed an identity function over it is registered
-toolbox.register_model(UserDetail)
+def contact_user(name: str, city: str):
+    return f"User {name} from {city} was contacted"
+
+toolbox.register_function(contact_user)
 
 response = client.chat.completions.create(
     model="gpt-3.5-turbo-1106",
-    messages=[{"role": "user",
-               "content": "Extract user details from the following sentence: John lives in Warsaw and likes banana"}],
+    messages=[{"role": "user", "content": "Contact John. John lives in Warsaw"}],
     tools=toolbox.tool_schemas(),
-    tool_choice="auto",
+    tool_choice={"type": "function", "function": {"name": "contact_user"}},
 )
-
 # There might be more than one tool calls and more than one result
 results = toolbox.process_response(response)
 
-pprint(results)
+pprint(results[0]['content'])
+
 ```
 Output:
 ```
-[UserDetail(name='John', city='Warsaw')]
+User John from Warsaw was contacted
 ```
 
-### Example: Dispatching to a function
+### Example: Getting structured data from LLM
 
 ```python
-def contact_user(user: UserDetail):
-    return f"User {user.name} from {user.city} was contacted"
-
+# Define a Pydantic model for your tool's input
+class UserDetail(BaseModel):
+    name: str
+    city: str
 
-toolbox.register_model(contact_user)
+# Register your model
+toolbox.register_model(UserDetail)
 
 response = client.chat.completions.create(
     model="gpt-3.5-turbo-1106",
-    messages=[{"role": "user", "content": "Contact John. John lives in Warsaw"}],
+    messages=[{"role": "user",
+               "content": "Extract user details from the following sentence: John lives in Warsaw and likes banana"}],
     tools=toolbox.tool_schemas(),
-    tool_choice={"type": "function", "function": {"name": "contact_user"}},
+    tool_choice="auto",
 )
+
 # There might be more than one tool calls and more than one result
 results = toolbox.process_response(response)
 
-pprint(results)
-
+pprint(results[0]['content'])
 ```
 Output:
 ```
-['User John from Warsaw was contacted']
+UserDetail(name='John', city='Warsaw')
 ```
 
+
 Discover more possibilities and examples in the examples directory and test suite.
 
 ## License
 
 LLMEasyTools is open-sourced under the Apache License. For more details, see the LICENSE file.
```

### Comparing `LLMEasyTools-0.6/PKG-INFO` & `LLMEasyTools-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: LLMEasyTools
-Version: 0.6
+Version: 0.7
 Summary: OpenAI tools and functions with no fuss.
+Author: Natalia Borovskikh
 Author-email: Zbigniew Łukasiak <zzbbyy@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -213,14 +214,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic
 Requires-Dist: docstring_parser~=0.15
+Requires-Dist: openai~=1.23
 Provides-Extra: test
 Requires-Dist: pytest~=7.4.4; extra == "test"
 
 # LLMEasyTools
 **OpenAI tools and functions with no fuss.**
 
 LLMEasyTool is a minimal Python package designed for seamless interaction with 
@@ -231,15 +233,15 @@
 It doesn't take over the interaction with the OpenAI client, making it easier for developers
 to debug their code and optimize the communication with the LLM.
 
 By integrating Pydantic, LLMEasyTools ensures robust data validation and schema generation.
 
 ## Features
 
-- **Schema Generation**: Effortlessly create JSON schemas for tools using Pydantic models.
+- **Schema Generation**: Effortlessly create JSON schemas for tools from type annotations
 - **Structured Data from LLM**
 - **Function Name Mapping**: Flexibly map JSON schema names to Python code.
 - **Dispatching Function Calls**: Directly invoke functions based on LLM response structures.
 - **Stateful Tools**: You can register methods bound to an object to have stateful tools. See [examples/stateful_search.py](https://github.com/zby/LLMEasyTools/tree/main/examples)
 - **No Patching!**: No globals, some 200 lines of straightforward object oriented code.
 
 ## Installation
@@ -254,79 +256,77 @@
 cd LLMEasyTools
 pip install -e .
 pytest -v tests
 ```
 
 ## Usage
 
-### Basic Example: Getting structured data from LLM
+### Basic Example: Dispatching to a function
 
 ```python
 from llm_easy_tools import ToolBox
 from pydantic import BaseModel
 from openai import OpenAI
 from pprint import pprint
 
 client = OpenAI()
 
-
-# Define a Pydantic model for your tool's input
-class UserDetail(BaseModel):
-    name: str
-    city: str
-
-
 # Create a ToolBox instance
 toolbox = ToolBox()
 
-# Register your tool - if a class is passed an identity function over it is registered
-toolbox.register_model(UserDetail)
+def contact_user(name: str, city: str):
+    return f"User {name} from {city} was contacted"
+
+toolbox.register_function(contact_user)
 
 response = client.chat.completions.create(
     model="gpt-3.5-turbo-1106",
-    messages=[{"role": "user",
-               "content": "Extract user details from the following sentence: John lives in Warsaw and likes banana"}],
+    messages=[{"role": "user", "content": "Contact John. John lives in Warsaw"}],
     tools=toolbox.tool_schemas(),
-    tool_choice="auto",
+    tool_choice={"type": "function", "function": {"name": "contact_user"}},
 )
-
 # There might be more than one tool calls and more than one result
 results = toolbox.process_response(response)
 
-pprint(results)
+pprint(results[0]['content'])
+
 ```
 Output:
 ```
-[UserDetail(name='John', city='Warsaw')]
+User John from Warsaw was contacted
 ```
 
-### Example: Dispatching to a function
+### Example: Getting structured data from LLM
 
 ```python
-def contact_user(user: UserDetail):
-    return f"User {user.name} from {user.city} was contacted"
-
+# Define a Pydantic model for your tool's input
+class UserDetail(BaseModel):
+    name: str
+    city: str
 
-toolbox.register_model(contact_user)
+# Register your model
+toolbox.register_model(UserDetail)
 
 response = client.chat.completions.create(
     model="gpt-3.5-turbo-1106",
-    messages=[{"role": "user", "content": "Contact John. John lives in Warsaw"}],
+    messages=[{"role": "user",
+               "content": "Extract user details from the following sentence: John lives in Warsaw and likes banana"}],
     tools=toolbox.tool_schemas(),
-    tool_choice={"type": "function", "function": {"name": "contact_user"}},
+    tool_choice="auto",
 )
+
 # There might be more than one tool calls and more than one result
 results = toolbox.process_response(response)
 
-pprint(results)
-
+pprint(results[0]['content'])
 ```
 Output:
 ```
-['User John from Warsaw was contacted']
+UserDetail(name='John', city='Warsaw')
 ```
 
+
 Discover more possibilities and examples in the examples directory and test suite.
 
 ## License
 
 LLMEasyTools is open-sourced under the Apache License. For more details, see the LICENSE file.
```

### Comparing `LLMEasyTools-0.6/README.md` & `LLMEasyTools-0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 It doesn't take over the interaction with the OpenAI client, making it easier for developers
 to debug their code and optimize the communication with the LLM.
 
 By integrating Pydantic, LLMEasyTools ensures robust data validation and schema generation.
 
 ## Features
 
-- **Schema Generation**: Effortlessly create JSON schemas for tools using Pydantic models.
+- **Schema Generation**: Effortlessly create JSON schemas for tools from type annotations
 - **Structured Data from LLM**
 - **Function Name Mapping**: Flexibly map JSON schema names to Python code.
 - **Dispatching Function Calls**: Directly invoke functions based on LLM response structures.
 - **Stateful Tools**: You can register methods bound to an object to have stateful tools. See [examples/stateful_search.py](https://github.com/zby/LLMEasyTools/tree/main/examples)
 - **No Patching!**: No globals, some 200 lines of straightforward object oriented code.
 
 ## Installation
@@ -32,79 +32,77 @@
 cd LLMEasyTools
 pip install -e .
 pytest -v tests
 ```
 
 ## Usage
 
-### Basic Example: Getting structured data from LLM
+### Basic Example: Dispatching to a function
 
 ```python
 from llm_easy_tools import ToolBox
 from pydantic import BaseModel
 from openai import OpenAI
 from pprint import pprint
 
 client = OpenAI()
 
-
-# Define a Pydantic model for your tool's input
-class UserDetail(BaseModel):
-    name: str
-    city: str
-
-
 # Create a ToolBox instance
 toolbox = ToolBox()
 
-# Register your tool - if a class is passed an identity function over it is registered
-toolbox.register_model(UserDetail)
+def contact_user(name: str, city: str):
+    return f"User {name} from {city} was contacted"
+
+toolbox.register_function(contact_user)
 
 response = client.chat.completions.create(
     model="gpt-3.5-turbo-1106",
-    messages=[{"role": "user",
-               "content": "Extract user details from the following sentence: John lives in Warsaw and likes banana"}],
+    messages=[{"role": "user", "content": "Contact John. John lives in Warsaw"}],
     tools=toolbox.tool_schemas(),
-    tool_choice="auto",
+    tool_choice={"type": "function", "function": {"name": "contact_user"}},
 )
-
 # There might be more than one tool calls and more than one result
 results = toolbox.process_response(response)
 
-pprint(results)
+pprint(results[0]['content'])
+
 ```
 Output:
 ```
-[UserDetail(name='John', city='Warsaw')]
+User John from Warsaw was contacted
 ```
 
-### Example: Dispatching to a function
+### Example: Getting structured data from LLM
 
 ```python
-def contact_user(user: UserDetail):
-    return f"User {user.name} from {user.city} was contacted"
-
+# Define a Pydantic model for your tool's input
+class UserDetail(BaseModel):
+    name: str
+    city: str
 
-toolbox.register_model(contact_user)
+# Register your model
+toolbox.register_model(UserDetail)
 
 response = client.chat.completions.create(
     model="gpt-3.5-turbo-1106",
-    messages=[{"role": "user", "content": "Contact John. John lives in Warsaw"}],
+    messages=[{"role": "user",
+               "content": "Extract user details from the following sentence: John lives in Warsaw and likes banana"}],
     tools=toolbox.tool_schemas(),
-    tool_choice={"type": "function", "function": {"name": "contact_user"}},
+    tool_choice="auto",
 )
+
 # There might be more than one tool calls and more than one result
 results = toolbox.process_response(response)
 
-pprint(results)
-
+pprint(results[0]['content'])
 ```
 Output:
 ```
-['User John from Warsaw was contacted']
+UserDetail(name='John', city='Warsaw')
 ```
 
+
 Discover more possibilities and examples in the examples directory and test suite.
 
 ## License
 
 LLMEasyTools is open-sourced under the Apache License. For more details, see the LICENSE file.
```

### Comparing `LLMEasyTools-0.6/examples/extract_user_details.py` & `LLMEasyTools-0.7/examples/extract_user_details.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 
 # Define a Pydantic model for your tool's input
 class UserDetail(BaseModel):
     name: str
     city: str
 
 
-def contact_user(user: UserDetail):
-    return f"User {user.name} from {user.city} was contactd"
-
 # Create a ToolBox instance
 toolbox = ToolBox()
 
 # Register your model
 toolbox.register_model(UserDetail)
 
 response = client.chat.completions.create(
@@ -26,21 +23,25 @@
     messages=[{"role": "user", "content": "Extract user details from the following sentence: John lives in Warsaw and likes banana"}],
     tools=toolbox.tool_schemas(),
     tool_choice="auto",
 )
 # There might be more than one tool calls and more than one result
 results = toolbox.process_response(response)
 
-pprint(results)
+#pprint(results)
+pprint(results[0]['content'])
+
+def contact_user(name: str, city: str) -> str:
+    return f"User {name} from {city} was contactd"
 
 toolbox.register_function(contact_user)
 
 response = client.chat.completions.create(
     model="gpt-3.5-turbo-1106",
     messages=[{"role": "user", "content": "Contact John. John lives in Warsaw"}],
     tools=toolbox.tool_schemas(),
     tool_choice={"type": "function", "function": {"name": "contact_user"}},
 )
 # There might be more than one tool calls and more than one result
 results = toolbox.process_response(response)
 
-pprint(results)
+pprint(results[0]['content'])
```

### Comparing `LLMEasyTools-0.6/examples/stateful_search.py` & `LLMEasyTools-0.7/examples/stateful_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pydantic import BaseModel
-from llm_easy_tools import ToolBox, external_function
+from llm_easy_tools import ToolBox, llm_function
 import re
 from openai import OpenAI
 
 # Define Pydantic models for the search tool's input and word query
 class SearchQuery(BaseModel):
     term: str
 
@@ -16,41 +16,41 @@
         self.documents = [
             {"title": "Introduction to GPT-4", "content": "GPT-4 is the latest language model by OpenAI. It has several new features."},
             {"title": "Advancements in AI", "content": "Exploring the latest advancements in artificial intelligence. AI is evolving rapidly."},
             {"title": "Natural Language Processing", "content": "Understanding NLP and its applications. NLP is a key part of AI."}
         ]
         self.current_document = None
 
-    @external_function()
-    def search_document(self, query: SearchQuery):
+    @llm_function()
+    def search_document(self, term: str):
         closest_match = None
         min_distance = float('inf')
         for doc in self.documents:
-            distance = self._calculate_similarity(query.term, doc['title'])
+            distance = self._calculate_similarity(term, doc['title'])
             if distance < min_distance:
                 min_distance = distance
                 closest_match = doc
 
         if closest_match:
             self.current_document = closest_match
             first_sentence = closest_match['content'].split('.')[0]
             return f"Found document, title: {closest_match['title']}.\n {first_sentence}..."
         else:
             return "No matching document found."
 
-    @external_function()
-    def lookup_word(self, query: WordQuery):
+    @llm_function()
+    def lookup_word(self, word: str):
         if not self.current_document:
             return "No document is currently selected."
 
         sentences = self.current_document['content'].split('.')
         for sentence in sentences:
-            if query.word in sentence:
+            if word in sentence:
                 return sentence.strip()
-        return f"The word '{query.word}' was not found in the current document."
+        return f"The word '{word}' was not found in the current document."
 
     def _calculate_similarity(self, term, title):
         # Simple similarity calculation (can be replaced with more sophisticated methods)
         return abs(len(term) - len(title))  # Example simplistic similarity measure
 
 # Create an instance of DocumentManager
 doc_manager = DocumentManager()
@@ -69,25 +69,26 @@
     tools=toolbox.tool_schemas(),
     tool_choice="auto"
 )
 
 # Process the response to search for the document
 
 results_search = toolbox.process_response(response_search)
-print(results_search)
+print(results_search[0]['content'])
 
 # Example LLM call to look up a word in the current document
 response_lookup = client.chat.completions.create(
     model="gpt-3.5-turbo-1106",
     messages=[{"role": "user", "content": "Look up the word 'evolving'"}],
     tools=toolbox.tool_schemas(),
     tool_choice="auto",
 )
 # Process the response to look up the word
 results_lookup = toolbox.process_response(response_lookup)
-print(results_lookup)
+print(results_lookup[0]['content'])
 
 
 ## OUTPUT
 #
-# ['Found document, title: Advancements in AI.\n Exploring the latest advancements in artificial intelligence...']
-# ['AI is evolving rapidly']
+# Found document, title: Advancements in AI.
+# Exploring the latest advancements in artificial intelligence...
+# AI is evolving rapidly
```

### Comparing `LLMEasyTools-0.6/pyproject.toml` & `LLMEasyTools-0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [build-system]
 requires = ["setuptools>=59.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LLMEasyTools"
-version = "0.06"
-authors = [{ name = "Zbigniew Łukasiak", email = "zzbbyy@gmail.com" }]
+version = "0.07"
+authors = [{ name = "Zbigniew Łukasiak", email = "zzbbyy@gmail.com" }, { name = "Natalia Borovskikh" }]
 description = "OpenAI tools and functions with no fuss."
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pydantic",
-    "docstring_parser~=0.15"
+    "docstring_parser~=0.15",
+    "openai~=1.23"
 ]
 [project.urls]
 repository = "https://github.com/zby/LLMEasyTools"
 
 [tool.setuptools]
 packages = ["llm_easy_tools"]
```

### Comparing `LLMEasyTools-0.6/tests/tools_test.py` & `LLMEasyTools-0.7/tests/tools_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,223 +1,200 @@
 import pytest
 import json
 
 from unittest.mock import Mock
-from llm_easy_tools import ToolBox, SchemaGenerator, external_function, extraction_model
+from llm_easy_tools import ToolBox, ToolResult, llm_function
 from pydantic import BaseModel, Field, ValidationError
 from typing import Any
-
-
-class ToolParam(BaseModel):
-    value: int
-
-
-class AdditionalToolParam(BaseModel):
-    value: int
+from openai.types.chat.chat_completion import ChatCompletionMessage, ChatCompletion
 
 class TestTool:
 
     class SomeClass(BaseModel):
         value: int
 
-    @external_function()
-    def tool_method(self, arg: ToolParam) -> str:
+    @llm_function()
+    def tool_method(self, arg: int) -> str:
         return f'executed tool_method with param: {arg}'
 
-    @external_function()
-    def additional_tool_method(self, arg: AdditionalToolParam) -> str:
+    @llm_function()
+    def additional_tool_method(self, arg: int) -> str:
         return f'executed additional_tool_method with param: {arg}'
 
-    def _private_tool_method(self, arg: AdditionalToolParam) -> str:
+    def _private_tool_method(self, arg: int) -> str:
         return str(arg.value * 4)
 
-    @extraction_model()
+    @llm_function()
     class User(BaseModel):
         name: str
         age: int
 
-    @extraction_model('address')
+    @llm_function('short_address')
     class Address(BaseModel):
         city: str
         street: str
 
 
 tool = TestTool()
 
 def test_toolbox_init():
     toolbox = ToolBox()
-    assert toolbox.strict == True
     assert toolbox.tool_registry == {}
-    assert toolbox.name_mappings == []
     assert toolbox.tool_schemas() == []
-    assert isinstance(toolbox.generator, SchemaGenerator)
+    assert toolbox.case_insensitive == False
+    assert toolbox.fix_json_args == True
 
 def test_register_toolset():
     tool_manager = ToolBox()
 
     # Test the normal case
     tool_manager.register_toolset(tool)
 
     assert 'TestTool' in tool_manager.tool_sets
     assert 'tool_method' in tool_manager.tool_registry
     assert 'additional_tool_method' in tool_manager.tool_registry
     assert 'User' in tool_manager.tool_registry
     assert 'SomeClass' not in tool_manager.tool_registry
-    assert 'Address' in tool_manager.tool_registry
-    assert tool_manager.schema_name_to_func('address') == 'Address'
+    assert 'short_address' in tool_manager.tool_registry
     assert '_private_tool_method' not in tool_manager.tool_registry
 
     # Test for Exception when a Toolset with same key is being registered
     with pytest.raises(Exception) as exception_info:
         tool_manager.register_toolset(tool)
 
     assert str(exception_info.value) == 'A toolset with key TestTool already exists.'
 
-def test_toolbox_from_object():
-    toolbox = ToolBox.toolbox_from_object(tool)
-    assert "tool_method" in toolbox.tool_registry
-    assert len(toolbox.tool_registry) == 4
-    assert len(toolbox.tool_schemas()) == 4
-
-def test_schema_name_to_func():
-    toolbox = ToolBox(name_mappings=[("tool_method", "TestTool")])
-    assert toolbox.schema_name_to_func("TestTool") == "tool_method"
-    assert toolbox.schema_name_to_func("NotFound") == "NotFound"
-
 
 class FunctionCallMock:
     def __init__(self, name, arguments):
         self.name = name
         self.arguments = arguments
 
 def test_process():
-    toolbox = ToolBox.toolbox_from_object(tool)
-    function_call = FunctionCallMock(name="tool_method", arguments=json.dumps(ToolParam(value=2).model_dump()))
-    result = toolbox.process_function(function_call)
-    assert result == 'executed tool_method with param: value=2'
-
-    toolbox = ToolBox.toolbox_from_object(tool, name_mappings=[("additional_tool_method", "custom_name")])
-    function_call = FunctionCallMock(name="custom_name", arguments=json.dumps(ToolParam(value=3).model_dump()))
-    result = toolbox.process_function(function_call)
-    assert result == "executed additional_tool_method with param: value=3"
+    toolbox = ToolBox()
+    toolbox.register_toolset(tool)
+    function_call = FunctionCallMock(name="tool_method", arguments=json.dumps({"arg": 2}))
+    result = toolbox.process_function(function_call, '')
+    assert isinstance(result, ToolResult)
+    assert result.output == 'executed tool_method with param: 2'
 
     # Test with unknown function call name
-    with pytest.raises(ValueError):
-        function_call = FunctionCallMock(name="unknown_name", arguments=json.dumps(ToolParam(value=3).model_dump()))
-        toolbox.process_function(function_call)
+    with pytest.raises(KeyError):
+        function_call = FunctionCallMock(name="unknown", arguments=json.dumps({'arg': 3}))
+        toolbox.process_function(function_call, '')
 
 
 class UserDetail(BaseModel):
     name: str
     age: int
 
-def test_process_with_identity():
+def test_process_model():
     toolbox = ToolBox()
     toolbox.register_model(UserDetail)
     assert "UserDetail" in toolbox.tool_registry
     original_user = UserDetail(name="John", age=21)
     function_call = FunctionCallMock(name="UserDetail", arguments=json.dumps(original_user.model_dump()))
-    result = toolbox.process_function(function_call)
-    assert result == original_user
+    result = toolbox.process_function(function_call, '')
+    assert result.model == original_user
+
+def mk_chat_with_tool_call(name, args):
+    message = ChatCompletionMessage(
+        role="assistant",
+        tool_calls=[
+            {
+                "id": 'A',
+                "type": 'function',
+                "function": {
+                    "arguments": json.dumps(args),
+                    "name": name
+                }
+            }
+        ]
+    )
+    chat_completion = ChatCompletion(
+        id='A',
+        created=0,
+        model='A',
+        choices=[{'finish_reason': 'stop', 'index': 0, 'message': message}],
+        object='chat.completion'
+    )
+    return chat_completion
+
 
 def test_process_response():
     # too much mocking in this test
     toolbox = ToolBox()
     toolbox.register_model(UserDetail)
     original_user = UserDetail(name="John", age=21)
-    function_call = FunctionCallMock(name="UserDetail", arguments=json.dumps(original_user.model_dump()))
-    response = Mock(choices=[Mock(message=Mock(function_call=False, tool_calls=[Mock(function=function_call)]))])
+    response = mk_chat_with_tool_call("UserDetail", original_user.model_dump())
     results = toolbox.process_response(response)
     assert len(results) == 1
-    assert results[0] == original_user
+    assert results[0].model == original_user
 
 
 # Define the test cases
 def test_register_tool():
     class Tool(BaseModel):
         name: str
 
-    def example_tool(tool: Tool):
-        print('Running test tool')
+    def example_tool(name: str):
+        print(f'Running test tool with name param: "{name}"')
 
-    @external_function("good_name")
-    def bad_name_tool(tool: Tool):
-        print('Running bad_name_tool')
 
     toolbox = ToolBox()
 
     # Test with correct parameters
     toolbox.register_function(example_tool)
     assert 'example_tool' in toolbox.tool_registry
     function_info = toolbox.tool_registry['example_tool']
     assert function_info["function"] == example_tool
-    assert function_info["param_class"] == Tool
     assert len(toolbox.tool_schemas()) == 1
-    assert len(toolbox.function_schemas()) == 1
-    assert toolbox.tool_schemas()[0]['function']['name'] == 'example_tool'
-    assert toolbox.function_schemas()[0]['name'] == 'example_tool'
-
-    # Test with function with more than one parameter
-    with pytest.raises(TypeError):
-        def two_parameters(a, b): pass
-        toolbox.register_function(two_parameters)
 
     # Test with function with no parameters
-    with pytest.raises(TypeError):
-        def no_parameters(): pass
-        toolbox.register_function(no_parameters)
-
-    # Test with function having a parameter which isn't subclass of BaseModel
-    with pytest.raises(TypeError):
-        def wrong_parameter(a: Any): pass
-        toolbox.register_function(wrong_parameter)
+    def no_parameters(): pass
+    toolbox.register_function(no_parameters)
+    assert 'no_parameters' in toolbox.tool_registry
+
+    @llm_function("good_name")
+    def bad_name_tool(name: str):
+        print('Running bad_name_tool')
 
     toolbox.register_function(bad_name_tool)
-    assert 'bad_name_tool' in toolbox.tool_registry
-    function_info = toolbox.tool_registry['bad_name_tool']
+    assert 'good_name' in toolbox.tool_registry
+    function_info = toolbox.tool_registry['good_name']
     assert function_info["function"] == bad_name_tool
-    assert function_info["param_class"] == Tool
-    assert toolbox.schema_name_to_func('good_name') == 'bad_name_tool'
 
 def test_register_model():
     class Tool(BaseModel):
         name: str
 
     class WikiSearch(BaseModel):
         query: str
 
     toolbox = ToolBox()
     toolbox.register_model(Tool)
 
-    identity_function = toolbox.tool_registry['Tool']["function"]
-    assert callable(identity_function)
-    assert identity_function(Tool(name="test")) == Tool(name="test")
-    assert toolbox.tool_registry['Tool']["param_class"] is Tool
+    assert toolbox.tool_registry['Tool']["model_class"] is Tool
     assert len(toolbox.tool_schemas()) == 1
-    assert toolbox.tool_schemas()[0]['function']['name'] == 'tool' # by default case_insensitive
+    assert toolbox.tool_schemas()[0]['function']['name'] == 'Tool'
 
     toolbox.register_model(WikiSearch)
-    identity_function = toolbox.tool_registry['WikiSearch']["function"]
-    assert callable(identity_function)
-    assert identity_function(WikiSearch(query="test")) == WikiSearch(query="test")
-    assert toolbox.tool_registry['WikiSearch']["param_class"] is WikiSearch
+    assert toolbox.tool_registry['WikiSearch']["model_class"] is WikiSearch
     assert len(toolbox.tool_schemas()) == 2
-    assert toolbox.tool_schemas()[1]['function']['name'] == 'wikisearch'
 
-    assert toolbox.get_tool_schema('WikiSearch')['function']['name'] == 'wikisearch'
-    assert toolbox.get_tool_schema('WikiSearch')['type'] == 'function'
+    assert toolbox.get_tool_schema('WikiSearch')['function']['name'] == 'WikiSearch'
 
 def test_prefixing():
     class Tool(BaseModel):
         name: str
 
     class Reflection(BaseModel):
         relevancy: str = Field(..., description="Whas the last retrieved information relevant and why?")
 
-    def example_tool(tool: Tool):
+    def example_tool(name: str):
         return 'test tool result'
 
     toolbox = ToolBox()
     toolbox.register_function(example_tool)
     tool_schemas = toolbox.tool_schemas(prefix_class=Reflection)
     assert len(tool_schemas) == 1
     function_schema = tool_schemas[0]['function']
@@ -232,36 +209,35 @@
 
 def test_process_function_with_prefixing():
     class Reflection(BaseModel):
         relevancy: str = Field(..., description="Whas the last retrieved information relevant and why?")
 
     toolbox = ToolBox()
     toolbox.register_toolset(tool)
-    prefixed_name = 'reflection_and_tool_method'
-    no_reflection_function_call = FunctionCallMock(name=prefixed_name, arguments=json.dumps(ToolParam(value=2).model_dump()))
+    prefixed_name = 'Reflection_and_tool_method'
+    no_reflection_function_call = FunctionCallMock(name=prefixed_name, arguments=json.dumps({'arg': 2}))
     with pytest.raises(Exception) as exception_info:
-        toolbox.process_function(no_reflection_function_call, prefix_class=Reflection)
+        toolbox.process_function(no_reflection_function_call, '', prefix_class=Reflection)
     assert isinstance(exception_info.value, ValidationError)
-    args = ToolParam(value=2).model_dump()
+    args = {'arg': 2}
     args['relevancy'] = 'very good'
     function_call = FunctionCallMock(name=prefixed_name, arguments=json.dumps(args))
-    result = toolbox.process_function(function_call, prefix_class=Reflection)
-    assert result == 'executed tool_method with param: value=2'
+    result = toolbox.process_function(function_call, '', prefix_class=Reflection)
+    assert result.output == 'executed tool_method with param: 2'
     assert isinstance(toolbox.prefix, Reflection)
 
 def test_json_fix():
     toolbox = ToolBox()
     toolbox.register_model(UserDetail)
     original_user = UserDetail(name="John", age=21)
     json_data = json.dumps(original_user.model_dump())
     json_data = json_data[:-1]
     json_data = json_data + ',}'
     function_call = FunctionCallMock(name="UserDetail", arguments=json_data)
-    result = toolbox.process_function(function_call)
-    assert result == original_user
+    result = toolbox.process_function(function_call, '')
+    assert result.model == original_user
 
-    with pytest.raises(Exception) as exception_info:
-        toolbox.fix_json_args = False
-        toolbox.process_function(function_call)
-    assert isinstance(exception_info.value, json.decoder.JSONDecodeError)
+    toolbox.fix_json_args = False
+    result = toolbox.process_function(function_call, '')
+    assert 'json.decoder.JSONDecodeError' in result.error
 
 pytest.main()
```


# Comparing `tmp/retell_sdk-3.7.0.tar.gz` & `tmp/retell_sdk-3.8.0.tar.gz`

## Comparing `retell_sdk-3.7.0.tar` & `retell_sdk-3.8.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/__init__.py
--rw-r--r--   0        0        0    64254 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_base_client.py
--rw-r--r--   0        0        0    15337 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_constants.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_files.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_qs.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_resource.py
--rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_response.py
--rw-r--r--   0        0        0    10100 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_streaming.py
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_types.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_utils/__init__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/lib/.keep
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/resources/__init__.py
--rw-r--r--   0        0        0    43021 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/resources/agent.py
--rw-r--r--   0        0        0    25014 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/resources/call.py
--rw-r--r--   0        0        0    26571 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/resources/llm.py
--rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/resources/phone_number.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/__init__.py
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/agent_create_params.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/agent_list_response.py
--rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/agent_response.py
--rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/agent_update_params.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/call_create_params.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/call_list_params.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/call_list_response.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/call_register_params.py
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/call_response.py
--rw-r--r--   0        0        0    17703 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/llm_create_params.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/llm_list_response.py
--rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/llm_response.py
--rw-r--r--   0        0        0    17703 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/llm_update_params.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/phone_number_create_params.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/phone_number_list_response.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/phone_number_response.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/phone_number_update_params.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/register_call_response.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell_ai/lib/.keep
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell_sdk/lib/.keep
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/toddlzt/lib/.keep
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/.gitignore
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/LICENSE
--rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/pyproject.toml
--rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/__init__.py
+-rw-r--r--   0        0        0    64254 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_base_client.py
+-rw-r--r--   0        0        0    15337 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_constants.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_files.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_qs.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_resource.py
+-rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_response.py
+-rw-r--r--   0        0        0    10100 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_streaming.py
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_types.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_utils/__init__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/lib/.keep
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/resources/__init__.py
+-rw-r--r--   0        0        0    43021 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/resources/agent.py
+-rw-r--r--   0        0        0    25014 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/resources/call.py
+-rw-r--r--   0        0        0    26571 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/resources/llm.py
+-rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/resources/phone_number.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/__init__.py
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/agent_create_params.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/agent_list_response.py
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/agent_response.py
+-rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/agent_update_params.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/call_create_params.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/call_list_params.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/call_list_response.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/call_register_params.py
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/call_response.py
+-rw-r--r--   0        0        0    17703 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/llm_create_params.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/llm_list_response.py
+-rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/llm_response.py
+-rw-r--r--   0        0        0    17703 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/llm_update_params.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/phone_number_create_params.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/phone_number_list_response.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/phone_number_response.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/phone_number_update_params.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/register_call_response.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell_ai/lib/.keep
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell_sdk/lib/.keep
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/toddlzt/lib/.keep
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/.gitignore
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/LICENSE
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/pyproject.toml
+-rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/PKG-INFO
```

### Comparing `retell_sdk-3.7.0/src/retell/__init__.py` & `retell_sdk-3.8.0/src/retell/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_base_client.py` & `retell_sdk-3.8.0/src/retell/_base_client.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_client.py` & `retell_sdk-3.8.0/src/retell/_client.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_compat.py` & `retell_sdk-3.8.0/src/retell/_compat.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_exceptions.py` & `retell_sdk-3.8.0/src/retell/_exceptions.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_files.py` & `retell_sdk-3.8.0/src/retell/_files.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_models.py` & `retell_sdk-3.8.0/src/retell/_models.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_qs.py` & `retell_sdk-3.8.0/src/retell/_qs.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_resource.py` & `retell_sdk-3.8.0/src/retell/_resource.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_response.py` & `retell_sdk-3.8.0/src/retell/_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_streaming.py` & `retell_sdk-3.8.0/src/retell/_streaming.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_types.py` & `retell_sdk-3.8.0/src/retell/_types.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_utils/__init__.py` & `retell_sdk-3.8.0/src/retell/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_utils/_logs.py` & `retell_sdk-3.8.0/src/retell/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_utils/_proxy.py` & `retell_sdk-3.8.0/src/retell/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_utils/_sync.py` & `retell_sdk-3.8.0/src/retell/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_utils/_transform.py` & `retell_sdk-3.8.0/src/retell/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_utils/_typing.py` & `retell_sdk-3.8.0/src/retell/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/_utils/_utils.py` & `retell_sdk-3.8.0/src/retell/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/resources/__init__.py` & `retell_sdk-3.8.0/src/retell/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/resources/agent.py` & `retell_sdk-3.8.0/src/retell/resources/agent.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/resources/call.py` & `retell_sdk-3.8.0/src/retell/resources/call.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/resources/llm.py` & `retell_sdk-3.8.0/src/retell/resources/llm.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/resources/phone_number.py` & `retell_sdk-3.8.0/src/retell/resources/phone_number.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/types/__init__.py` & `retell_sdk-3.8.0/src/retell/types/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/types/agent_create_params.py` & `retell_sdk-3.8.0/src/retell/types/agent_create_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/types/agent_response.py` & `retell_sdk-3.8.0/src/retell/types/agent_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/types/agent_update_params.py` & `retell_sdk-3.8.0/src/retell/types/agent_update_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/types/call_create_params.py` & `retell_sdk-3.8.0/src/retell/types/call_create_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/types/call_list_params.py` & `retell_sdk-3.8.0/src/retell/types/call_list_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/types/call_register_params.py` & `retell_sdk-3.8.0/src/retell/types/call_register_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/types/call_response.py` & `retell_sdk-3.8.0/src/retell/types/call_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/types/llm_create_params.py` & `retell_sdk-3.8.0/src/retell/types/llm_create_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/types/llm_response.py` & `retell_sdk-3.8.0/src/retell/types/llm_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/types/llm_update_params.py` & `retell_sdk-3.8.0/src/retell/types/llm_update_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/types/phone_number_create_params.py` & `retell_sdk-3.8.0/src/retell/types/phone_number_create_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/types/phone_number_response.py` & `retell_sdk-3.8.0/src/retell/types/phone_number_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/src/retell/types/register_call_response.py` & `retell_sdk-3.8.0/src/retell/types/register_call_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/LICENSE` & `retell_sdk-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.7.0/pyproject.toml` & `retell_sdk-3.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "retell-sdk"
-version = "3.7.0"
+version = "3.8.0"
 description = "The official Python library for the retell API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Retell", email = "founders@retellai.com" },
 ]
 dependencies = [
```

### Comparing `retell_sdk-3.7.0/PKG-INFO` & `retell_sdk-3.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: retell-sdk
-Version: 3.7.0
+Version: 3.8.0
 Summary: The official Python library for the retell API
 Project-URL: Homepage, https://github.com/RetellAI/retell-python-sdk
 Project-URL: Repository, https://github.com/RetellAI/retell-python-sdk
 Author-email: Retell <founders@retellai.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -54,15 +54,17 @@
 ## Usage
 
 The full API of this library can be found in [api.md](https://github.com/RetellAI/retell-python-sdk/tree/main/api.md).
 
 ```python
 from retell import Retell
 
-client = Retell()
+client = Retell(
+    api_key="YOUR_RETELL_API_KEY",
+)
 
 agent_response = client.agent.create(
     llm_websocket_url="wss://your-websocket-endpoint",
     voice_id="11labs-Adrian",
 )
 print(agent_response.agent_id)
 ```
@@ -71,15 +73,17 @@
 
 Simply import `AsyncRetell` instead of `Retell` and use `await` with each API call:
 
 ```python
 import asyncio
 from retell import AsyncRetell
 
-client = AsyncRetell()
+client = AsyncRetell(
+    api_key="YOUR_RETELL_API_KEY",
+)
 
 
 async def main() -> None:
     agent_response = await client.agent.create(
         llm_websocket_url="wss://your-websocket-endpoint",
         voice_id="11labs-Adrian",
     )
```


# Comparing `tmp/genericsuite_ai-0.1.3.tar.gz` & `tmp/genericsuite_ai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genericsuite_ai-0.1.3.tar", max compression
+gzip compressed data, was "genericsuite_ai-0.1.4.tar", max compression
```

## Comparing `genericsuite_ai-0.1.3.tar` & `genericsuite_ai-0.1.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      747 2024-03-31 23:36:18.812667 genericsuite_ai-0.1.3/LICENSE
--rw-r--r--   0        0        0    11666 2024-04-09 13:13:21.852378 genericsuite_ai-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-03-03 23:59:15.113581 genericsuite_ai-0.1.3/genericsuite_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 13:12:24.883757 genericsuite_ai-0.1.3/genericsuite_ai/chalicelib/endpoints/__init__.py
--rw-r--r--   0        0        0     2551 2024-02-29 10:54:59.765849 genericsuite_ai-0.1.3/genericsuite_ai/chalicelib/endpoints/ai_chatbot_endpoint.py
--rw-r--r--   0        0        0        0 2024-03-03 12:55:02.975460 genericsuite_ai-0.1.3/genericsuite_ai/chalicelib/util/__init__.py
--rw-r--r--   0        0        0      676 2024-03-03 13:05:09.210706 genericsuite_ai-0.1.3/genericsuite_ai/chalicelib/util/create_app.py
--rw-r--r--   0        0        0        0 2024-02-26 12:41:31.668394 genericsuite_ai-0.1.3/genericsuite_ai/config/__init__.py
--rw-r--r--   0        0        0    13917 2024-03-02 15:15:40.872623 genericsuite_ai-0.1.3/genericsuite_ai/config/config.py
--rw-r--r--   0        0        0        0 2023-07-28 18:42:59.199879 genericsuite_ai-0.1.3/genericsuite_ai/lib/__init__.py
--rw-r--r--   0        0        0    22004 2024-03-03 02:48:34.133168 genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_audio_processing.py
--rw-r--r--   0        0        0     9346 2024-02-29 10:54:59.738325 genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_chatbot_commons.py
--rw-r--r--   0        0        0    11016 2024-02-29 10:54:59.763617 genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_chatbot_endpoint.py
--rw-r--r--   0        0        0    17788 2024-03-03 15:37:39.063166 genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_chatbot_main_langchain.py
--rw-r--r--   0        0        0    18309 2024-03-03 02:47:59.470955 genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_chatbot_main_langchain_OLD.py
--rw-r--r--   0        0        0     5022 2024-03-03 02:47:59.470981 genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_chatbot_main_openai.py
--rw-r--r--   0        0        0    11019 2024-02-29 11:11:26.462600 genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_conversations.py
--rw-r--r--   0        0        0     4994 2024-02-29 10:54:59.759569 genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_embeddings.py
--rw-r--r--   0        0        0     3783 2024-02-29 12:27:31.428912 genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_gpt_fn_conversations.py
--rw-r--r--   0        0        0    16283 2024-03-02 17:40:43.234533 genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_gpt_functions.py
--rw-r--r--   0        0        0    15750 2024-03-03 02:47:59.470989 genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_image_generator.py
--rw-r--r--   0        0        0    13375 2024-03-03 15:55:15.380883 genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_langchain_models.py
--rw-r--r--   0        0        0     7222 2024-03-02 15:58:44.288898 genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_langchain_tools.py
--rw-r--r--   0        0        0     3171 2024-02-29 10:54:59.764343 genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_sub_bots.py
--rw-r--r--   0        0        0     7475 2024-03-02 15:00:32.355696 genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_utilities.py
--rw-r--r--   0        0        0    14434 2024-03-03 02:47:59.470968 genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_vision.py
--rw-r--r--   0        0        0    32697 2024-02-28 13:38:30.271183 genericsuite_ai-0.1.3/genericsuite_ai/lib/clarifai.py
--rw-r--r--   0        0        0     5487 2024-02-25 11:54:38.786458 genericsuite_ai-0.1.3/genericsuite_ai/lib/git_reader.py
--rw-r--r--   0        0        0     5723 2024-02-29 13:08:21.289363 genericsuite_ai-0.1.3/genericsuite_ai/lib/json_reader.py
--rw-r--r--   0        0        0     1076 2024-02-29 12:42:27.485181 genericsuite_ai-0.1.3/genericsuite_ai/lib/pdf_reader.py
--rw-r--r--   0        0        0     4112 2024-02-23 00:45:13.048529 genericsuite_ai-0.1.3/genericsuite_ai/lib/translator.py
--rw-r--r--   0        0        0    12133 2024-03-02 18:51:08.649645 genericsuite_ai-0.1.3/genericsuite_ai/lib/vector_index.py
--rw-r--r--   0        0        0     7779 2024-03-03 02:46:02.072630 genericsuite_ai-0.1.3/genericsuite_ai/lib/web_scraping.py
--rw-r--r--   0        0        0     6600 2024-02-29 10:54:59.759814 genericsuite_ai-0.1.3/genericsuite_ai/lib/web_search.py
--rw-r--r--   0        0        0      844 2024-02-29 12:42:39.130214 genericsuite_ai-0.1.3/genericsuite_ai/lib/youtube_reader.py
--rw-r--r--   0        0        0        0 2024-02-24 04:05:41.201010 genericsuite_ai-0.1.3/genericsuite_ai/models/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 01:53:51.743753 genericsuite_ai-0.1.3/genericsuite_ai/models/billing/__init__.py
--rw-r--r--   0        0        0     1687 2024-03-14 13:37:54.631329 genericsuite_ai-0.1.3/genericsuite_ai/models/billing/billing_utilities.py
--rw-r--r--   0        0        0     1697 2024-04-09 13:23:32.607884 genericsuite_ai-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    13349 1970-01-01 00:00:00.000000 genericsuite_ai-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      747 2024-03-31 23:36:18.812667 genericsuite_ai-0.1.4/LICENSE
+-rw-r--r--   0        0        0    11807 2024-04-19 09:16:32.145792 genericsuite_ai-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-03-03 23:59:15.113581 genericsuite_ai-0.1.4/genericsuite_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 13:12:24.883757 genericsuite_ai-0.1.4/genericsuite_ai/chalicelib/endpoints/__init__.py
+-rw-r--r--   0        0        0     2551 2024-02-29 10:54:59.765849 genericsuite_ai-0.1.4/genericsuite_ai/chalicelib/endpoints/ai_chatbot_endpoint.py
+-rw-r--r--   0        0        0        0 2024-03-03 12:55:02.975460 genericsuite_ai-0.1.4/genericsuite_ai/chalicelib/util/__init__.py
+-rw-r--r--   0        0        0      676 2024-03-03 13:05:09.210706 genericsuite_ai-0.1.4/genericsuite_ai/chalicelib/util/create_app.py
+-rw-r--r--   0        0        0        0 2024-02-26 12:41:31.668394 genericsuite_ai-0.1.4/genericsuite_ai/config/__init__.py
+-rw-r--r--   0        0        0    13917 2024-03-02 15:15:40.872623 genericsuite_ai-0.1.4/genericsuite_ai/config/config.py
+-rw-r--r--   0        0        0        0 2023-07-28 18:42:59.199879 genericsuite_ai-0.1.4/genericsuite_ai/lib/__init__.py
+-rw-r--r--   0        0        0    22004 2024-03-03 02:48:34.133168 genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_audio_processing.py
+-rw-r--r--   0        0        0     9346 2024-02-29 10:54:59.738325 genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_chatbot_commons.py
+-rw-r--r--   0        0        0    11016 2024-02-29 10:54:59.763617 genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_chatbot_endpoint.py
+-rw-r--r--   0        0        0    17788 2024-03-03 15:37:39.063166 genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_chatbot_main_langchain.py
+-rw-r--r--   0        0        0    18309 2024-03-03 02:47:59.470955 genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_chatbot_main_langchain_OLD.py
+-rw-r--r--   0        0        0     5022 2024-03-03 02:47:59.470981 genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_chatbot_main_openai.py
+-rw-r--r--   0        0        0    11019 2024-02-29 11:11:26.462600 genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_conversations.py
+-rw-r--r--   0        0        0     4994 2024-02-29 10:54:59.759569 genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_embeddings.py
+-rw-r--r--   0        0        0     3783 2024-02-29 12:27:31.428912 genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_gpt_fn_conversations.py
+-rw-r--r--   0        0        0    16283 2024-03-02 17:40:43.234533 genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_gpt_functions.py
+-rw-r--r--   0        0        0    15750 2024-03-03 02:47:59.470989 genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_image_generator.py
+-rw-r--r--   0        0        0    13375 2024-03-03 15:55:15.380883 genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_langchain_models.py
+-rw-r--r--   0        0        0     7222 2024-03-02 15:58:44.288898 genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_langchain_tools.py
+-rw-r--r--   0        0        0     3171 2024-02-29 10:54:59.764343 genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_sub_bots.py
+-rw-r--r--   0        0        0     7475 2024-03-02 15:00:32.355696 genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_utilities.py
+-rw-r--r--   0        0        0    14434 2024-03-03 02:47:59.470968 genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_vision.py
+-rw-r--r--   0        0        0    32697 2024-02-28 13:38:30.271183 genericsuite_ai-0.1.4/genericsuite_ai/lib/clarifai.py
+-rw-r--r--   0        0        0     5487 2024-02-25 11:54:38.786458 genericsuite_ai-0.1.4/genericsuite_ai/lib/git_reader.py
+-rw-r--r--   0        0        0     5723 2024-02-29 13:08:21.289363 genericsuite_ai-0.1.4/genericsuite_ai/lib/json_reader.py
+-rw-r--r--   0        0        0     1076 2024-02-29 12:42:27.485181 genericsuite_ai-0.1.4/genericsuite_ai/lib/pdf_reader.py
+-rw-r--r--   0        0        0     4112 2024-02-23 00:45:13.048529 genericsuite_ai-0.1.4/genericsuite_ai/lib/translator.py
+-rw-r--r--   0        0        0    12133 2024-03-02 18:51:08.649645 genericsuite_ai-0.1.4/genericsuite_ai/lib/vector_index.py
+-rw-r--r--   0        0        0     7779 2024-03-03 02:46:02.072630 genericsuite_ai-0.1.4/genericsuite_ai/lib/web_scraping.py
+-rw-r--r--   0        0        0     6600 2024-02-29 10:54:59.759814 genericsuite_ai-0.1.4/genericsuite_ai/lib/web_search.py
+-rw-r--r--   0        0        0      844 2024-02-29 12:42:39.130214 genericsuite_ai-0.1.4/genericsuite_ai/lib/youtube_reader.py
+-rw-r--r--   0        0        0        0 2024-02-24 04:05:41.201010 genericsuite_ai-0.1.4/genericsuite_ai/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 01:53:51.743753 genericsuite_ai-0.1.4/genericsuite_ai/models/billing/__init__.py
+-rw-r--r--   0        0        0     1687 2024-03-14 13:37:54.631329 genericsuite_ai-0.1.4/genericsuite_ai/models/billing/billing_utilities.py
+-rw-r--r--   0        0        0     1726 2024-04-20 14:20:09.946205 genericsuite_ai-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    13475 1970-01-01 00:00:00.000000 genericsuite_ai-0.1.4/PKG-INFO
```

### Comparing `genericsuite_ai-0.1.3/LICENSE` & `genericsuite_ai-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/README.md` & `genericsuite_ai-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # The GenericSuite AI for Python (backend version)
 
-![GenericSuite AI Logo](https://github.com/tomkat-cr/genericsuite-fe-ai/blob/main/src/lib/images/gs_ai_logo_circle.png)
+<img 
+    align="right"
+    width="100"
+    height="100"
+    src="https://genericsuite.carlosjramirez.com/images/gs_ai_logo_circle.svg"
+    title="GenericSuite AI logo by Carlos J. Ramirez"
+/>
 
 [GenericSuite AI](https://www.carlosjramirez.com/genericsuite/) is a versatile backend solution, designed to provide a comprehensive suite of features, tools and functionalities for AI oriented Python APIs.
 
 It's bassed on [The Generic Suite (backend version)](https://github.com/tomkat-cr/genericsuite-be), so its features are inherited.
 
 The perfect companion for this backend solution is [The GenericSuite AI (frontend version)](https://github.com/tomkat-cr/genericsuite-fe-ai)
 
@@ -144,18 +150,18 @@
 ```
 HUGGINGFACE_API_KEY=huggingface_api_key
 HUGGINGFACE_ENDPOINT_URL=huggingface_endpoint_url
 ```
 
 6. AWS Configuration
 ```
-AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_DEV=aws-s3-bucket-name
-AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_QA=aws-s3-bucket-name
-AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_STAGING=aws-s3-bucket-name
-AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_PROD=aws-s3-bucket-name
+AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_DEV=exampleapp-chatbot-attachments-dev
+AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_QA=exampleapp-chatbot-attachments-qa
+AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_STAGING=exampleapp-chatbot-attachments-staging
+AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_PROD=exampleapp-chatbot-attachments-prod
 ```
 
 7. Other AI configurations<br/>(not included in the original AWS Lambda deployment. Configurable via Configuration Parameters)
 ```
 EMBEDDINGS_ENGINE=openai
 # EMBEDDINGS_ENGINE=clarifai
```

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/chalicelib/endpoints/ai_chatbot_endpoint.py` & `genericsuite_ai-0.1.4/genericsuite_ai/chalicelib/endpoints/ai_chatbot_endpoint.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/chalicelib/util/create_app.py` & `genericsuite_ai-0.1.4/genericsuite_ai/chalicelib/util/create_app.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/config/config.py` & `genericsuite_ai-0.1.4/genericsuite_ai/config/config.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_audio_processing.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_audio_processing.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_chatbot_commons.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_chatbot_commons.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_chatbot_endpoint.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_chatbot_endpoint.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_chatbot_main_langchain.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_chatbot_main_langchain.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_chatbot_main_langchain_OLD.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_chatbot_main_langchain_OLD.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_chatbot_main_openai.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_chatbot_main_openai.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_conversations.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_conversations.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_embeddings.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_embeddings.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_gpt_fn_conversations.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_gpt_fn_conversations.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_gpt_functions.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_gpt_functions.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_image_generator.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_image_generator.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_langchain_models.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_langchain_models.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_langchain_tools.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_langchain_tools.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_sub_bots.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_sub_bots.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_utilities.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_utilities.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/ai_vision.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/ai_vision.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/clarifai.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/clarifai.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/git_reader.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/git_reader.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/json_reader.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/json_reader.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/pdf_reader.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/pdf_reader.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/translator.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/translator.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/vector_index.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/vector_index.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/web_scraping.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/web_scraping.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/web_search.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/web_search.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/lib/youtube_reader.py` & `genericsuite_ai-0.1.4/genericsuite_ai/lib/youtube_reader.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/genericsuite_ai/models/billing/billing_utilities.py` & `genericsuite_ai-0.1.4/genericsuite_ai/models/billing/billing_utilities.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.3/pyproject.toml` & `genericsuite_ai-0.1.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [project]
 name = "genericsuite_ai"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     { name="Carlos J. Ramirez", email="<tomkat_cr@yahoo.com>" }
 ]
 description = "The GenericSuite AI for Python (backend version)"
 readme = "README.md"
 requires-python = ">=3.9,<4.0"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: ISC License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.com/tomkat-cr/genericsuite-be-ai"
+Homepage = "https://genericsuite.carlosjramirez.com/Backend-Development/GenericSuite-AI/"
 Issues = "https://github.com/tomkat-cr/genericsuite-be-ai/issues"
 
 [tool.poetry]
 name = "genericsuite_ai"
-version = "0.1.3"
+version = "0.1.4"
 description = "The GenericSuite AI for Python (backend version)"
 authors = ["Carlos J. Ramirez <tomkat_cr@yahoo.com>"]
-license = "MIT"
+license = "ISC"
 readme = "README.md"
 repository = "https://github.com/tomkat-cr/genericsuite-be-ai.git"
 packages = [
     { include = "genericsuite_ai" }
 ]
 
 [tool.poetry.dependencies]
@@ -48,15 +48,15 @@
 pillow = "^10.1.0"
 clarifai = "^10.1.0"
 langchain-openai = "^0.0.8"
 langchainhub = "^0.1.14"
 jq = "^1.6.0"
 transformers = "^4.38.2"
 text-generation = "^0.6.1"
-genericsuite = "^0.1.3"
+genericsuite = "^0.1.4"
 
 [tool.poetry.group.dev.dependencies]
 changelog-cli = "^0.7.1"
 mypy = "^0.931"
 pylint = "^3.1.0"
 pytest = "^7.0.1"
 pytest-cov = "^3.0.0"
```

### Comparing `genericsuite_ai-0.1.3/PKG-INFO` & `genericsuite_ai-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: genericsuite_ai
-Version: 0.1.3
+Version: 0.1.4
 Summary: The GenericSuite AI for Python (backend version)
 Home-page: https://github.com/tomkat-cr/genericsuite-be-ai.git
-License: MIT
+License: ISC
 Author: Carlos J. Ramirez
 Author-email: tomkat_cr@yahoo.com
 Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: clarifai (>=10.1.0,<11.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: duckduckgo-search (>=4.1.1,<5.0.0)
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
-Requires-Dist: genericsuite (>=0.1.3,<0.2.0)
+Requires-Dist: genericsuite (>=0.1.4,<0.2.0)
 Requires-Dist: google-api-python-client (>=2.111.0,<3.0.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: jq (>=1.6.0,<2.0.0)
 Requires-Dist: langchain (>=0.1.1,<0.2.0)
 Requires-Dist: langchain-google-genai (>=0.0.5,<0.0.6)
 Requires-Dist: langchain-openai (>=0.0.8,<0.0.9)
 Requires-Dist: langchainhub (>=0.1.14,<0.2.0)
@@ -36,15 +36,21 @@
 Requires-Dist: transformers (>=4.38.2,<5.0.0)
 Requires-Dist: typing-extensions (>=4.8.0,<5.0.0)
 Project-URL: Repository, https://github.com/tomkat-cr/genericsuite-be-ai.git
 Description-Content-Type: text/markdown
 
 # The GenericSuite AI for Python (backend version)
 
-![GenericSuite AI Logo](https://github.com/tomkat-cr/genericsuite-fe-ai/blob/main/src/lib/images/gs_ai_logo_circle.png)
+<img 
+    align="right"
+    width="100"
+    height="100"
+    src="https://genericsuite.carlosjramirez.com/images/gs_ai_logo_circle.svg"
+    title="GenericSuite AI logo by Carlos J. Ramirez"
+/>
 
 [GenericSuite AI](https://www.carlosjramirez.com/genericsuite/) is a versatile backend solution, designed to provide a comprehensive suite of features, tools and functionalities for AI oriented Python APIs.
 
 It's bassed on [The Generic Suite (backend version)](https://github.com/tomkat-cr/genericsuite-be), so its features are inherited.
 
 The perfect companion for this backend solution is [The GenericSuite AI (frontend version)](https://github.com/tomkat-cr/genericsuite-fe-ai)
 
@@ -184,18 +190,18 @@
 ```
 HUGGINGFACE_API_KEY=huggingface_api_key
 HUGGINGFACE_ENDPOINT_URL=huggingface_endpoint_url
 ```
 
 6. AWS Configuration
 ```
-AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_DEV=aws-s3-bucket-name
-AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_QA=aws-s3-bucket-name
-AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_STAGING=aws-s3-bucket-name
-AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_PROD=aws-s3-bucket-name
+AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_DEV=exampleapp-chatbot-attachments-dev
+AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_QA=exampleapp-chatbot-attachments-qa
+AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_STAGING=exampleapp-chatbot-attachments-staging
+AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_PROD=exampleapp-chatbot-attachments-prod
 ```
 
 7. Other AI configurations<br/>(not included in the original AWS Lambda deployment. Configurable via Configuration Parameters)
 ```
 EMBEDDINGS_ENGINE=openai
 # EMBEDDINGS_ENGINE=clarifai
```


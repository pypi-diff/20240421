# Comparing `tmp/scrapegraphai-0.2.4.tar.gz` & `tmp/scrapegraphai-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.2.4.tar", max compression
+gzip compressed data, was "scrapegraphai-0.2.5.tar", max compression
```

## Comparing `scrapegraphai-0.2.4.tar` & `scrapegraphai-0.2.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.2.4/LICENSE
--rw-r--r--   0        0        0     7784 2024-04-20 20:58:42.211169 scrapegraphai-0.2.4/README.md
--rw-r--r--   0        0        0     1644 2024-04-21 09:24:54.440011 scrapegraphai-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       54 2024-03-03 14:00:51.196394 scrapegraphai-0.2.4/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.2.4/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6670 2024-03-24 19:34:24.965713 scrapegraphai-0.2.4/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      258 2024-04-20 20:58:42.218942 scrapegraphai-0.2.4/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     3623 2024-04-20 20:58:42.219086 scrapegraphai-0.2.4/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     4644 2024-04-20 20:58:42.219311 scrapegraphai-0.2.4/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2494 2024-04-20 20:58:42.219422 scrapegraphai-0.2.4/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     2191 2024-04-12 10:59:59.484979 scrapegraphai-0.2.4/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     2380 2024-04-20 20:58:42.219513 scrapegraphai-0.2.4/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3120 2024-04-20 20:58:42.219606 scrapegraphai-0.2.4/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0      164 2024-03-03 14:00:51.197634 scrapegraphai-0.2.4/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0      732 2024-04-09 11:47:11.921274 scrapegraphai-0.2.4/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-04-09 11:20:43.626222 scrapegraphai-0.2.4/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0     2363 2024-04-08 20:25:15.266957 scrapegraphai-0.2.4/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      290 2024-04-12 10:59:59.485515 scrapegraphai-0.2.4/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      601 2024-04-09 11:20:43.626608 scrapegraphai-0.2.4/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      651 2024-04-08 20:25:27.931161 scrapegraphai-0.2.4/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      839 2024-04-12 10:59:59.485625 scrapegraphai-0.2.4/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      590 2024-04-08 20:25:35.475199 scrapegraphai-0.2.4/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      575 2024-04-08 20:25:42.545477 scrapegraphai-0.2.4/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1721 2024-04-08 20:25:31.195250 scrapegraphai-0.2.4/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1657 2024-04-08 20:25:37.349894 scrapegraphai-0.2.4/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      503 2024-04-20 20:58:42.219766 scrapegraphai-0.2.4/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7544 2024-04-08 20:25:53.786578 scrapegraphai-0.2.4/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-04-20 20:58:42.219990 scrapegraphai-0.2.4/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3375 2024-04-20 20:58:42.220349 scrapegraphai-0.2.4/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6893 2024-04-20 20:58:42.220641 scrapegraphai-0.2.4/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     7249 2024-04-20 20:58:42.220842 scrapegraphai-0.2.4/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     4097 2024-04-20 20:58:42.221320 scrapegraphai-0.2.4/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1592 2024-04-20 20:58:42.221535 scrapegraphai-0.2.4/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3337 2024-04-20 20:58:42.221690 scrapegraphai-0.2.4/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4939 2024-04-20 20:58:42.221933 scrapegraphai-0.2.4/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     4545 2024-04-20 20:58:42.222355 scrapegraphai-0.2.4/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     1635 2024-04-20 20:58:42.222570 scrapegraphai-0.2.4/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      242 2024-04-12 10:55:27.494820 scrapegraphai-0.2.4/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     1856 2024-04-03 10:39:06.250892 scrapegraphai-0.2.4/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1437 2024-04-03 10:39:06.251121 scrapegraphai-0.2.4/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3630 2024-04-06 12:43:33.712449 scrapegraphai-0.2.4/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0     1504 2024-04-12 11:30:08.598599 scrapegraphai-0.2.4/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0     1070 2024-04-20 20:58:42.222753 scrapegraphai-0.2.4/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1118 2024-04-06 12:46:22.008255 scrapegraphai-0.2.4/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      631 2024-04-06 12:44:50.349656 scrapegraphai-0.2.4/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0      990 2024-03-18 13:23:59.117686 scrapegraphai-0.2.4/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     9409 1970-01-01 00:00:00.000000 scrapegraphai-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.2.5/LICENSE
+-rw-r--r--   0        0        0     7784 2024-04-20 20:58:42.211169 scrapegraphai-0.2.5/README.md
+-rw-r--r--   0        0        0     1644 2024-04-21 15:11:21.473856 scrapegraphai-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-03-03 14:00:51.196394 scrapegraphai-0.2.5/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.2.5/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6670 2024-03-24 19:34:24.965713 scrapegraphai-0.2.5/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      258 2024-04-20 20:58:42.218942 scrapegraphai-0.2.5/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     3623 2024-04-20 20:58:42.219086 scrapegraphai-0.2.5/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     4644 2024-04-20 20:58:42.219311 scrapegraphai-0.2.5/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2494 2024-04-20 20:58:42.219422 scrapegraphai-0.2.5/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     2191 2024-04-12 10:59:59.484979 scrapegraphai-0.2.5/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     2380 2024-04-20 20:58:42.219513 scrapegraphai-0.2.5/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3120 2024-04-20 20:58:42.219606 scrapegraphai-0.2.5/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0      164 2024-03-03 14:00:51.197634 scrapegraphai-0.2.5/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0      732 2024-04-21 15:11:07.486160 scrapegraphai-0.2.5/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-04-09 11:20:43.626222 scrapegraphai-0.2.5/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0     2363 2024-04-08 20:25:15.266957 scrapegraphai-0.2.5/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      290 2024-04-12 10:59:59.485515 scrapegraphai-0.2.5/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      601 2024-04-09 11:20:43.626608 scrapegraphai-0.2.5/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      651 2024-04-08 20:25:27.931161 scrapegraphai-0.2.5/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      839 2024-04-12 10:59:59.485625 scrapegraphai-0.2.5/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      590 2024-04-08 20:25:35.475199 scrapegraphai-0.2.5/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      575 2024-04-08 20:25:42.545477 scrapegraphai-0.2.5/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-04-08 20:25:31.195250 scrapegraphai-0.2.5/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1657 2024-04-08 20:25:37.349894 scrapegraphai-0.2.5/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      503 2024-04-20 20:58:42.219766 scrapegraphai-0.2.5/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7544 2024-04-08 20:25:53.786578 scrapegraphai-0.2.5/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-04-20 20:58:42.219990 scrapegraphai-0.2.5/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3375 2024-04-20 20:58:42.220349 scrapegraphai-0.2.5/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6893 2024-04-20 20:58:42.220641 scrapegraphai-0.2.5/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     7249 2024-04-20 20:58:42.220842 scrapegraphai-0.2.5/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     4097 2024-04-20 20:58:42.221320 scrapegraphai-0.2.5/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1592 2024-04-20 20:58:42.221535 scrapegraphai-0.2.5/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3337 2024-04-20 20:58:42.221690 scrapegraphai-0.2.5/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     5177 2024-04-21 09:27:38.253618 scrapegraphai-0.2.5/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     4545 2024-04-20 20:58:42.222355 scrapegraphai-0.2.5/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     1635 2024-04-20 20:58:42.222570 scrapegraphai-0.2.5/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      242 2024-04-12 10:55:27.494820 scrapegraphai-0.2.5/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2024-04-03 10:39:06.250892 scrapegraphai-0.2.5/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1437 2024-04-03 10:39:06.251121 scrapegraphai-0.2.5/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3630 2024-04-06 12:43:33.712449 scrapegraphai-0.2.5/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0     1504 2024-04-12 11:30:08.598599 scrapegraphai-0.2.5/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0     1070 2024-04-20 20:58:42.222753 scrapegraphai-0.2.5/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1118 2024-04-06 12:46:22.008255 scrapegraphai-0.2.5/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      631 2024-04-06 12:44:50.349656 scrapegraphai-0.2.5/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0      990 2024-03-18 13:23:59.117686 scrapegraphai-0.2.5/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0     9409 1970-01-01 00:00:00.000000 scrapegraphai-0.2.5/PKG-INFO
```

### Comparing `scrapegraphai-0.2.4/LICENSE` & `scrapegraphai-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/README.md` & `scrapegraphai-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/pyproject.toml` & `scrapegraphai-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapegraphai"
-version = "0.2.4"
+version = "0.2.5"
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `scrapegraphai-0.2.4/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.2.5/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.2.5/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.2.5/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.2.5/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.2.5/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.2.5/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.2.5/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.2.5/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.2.5/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.2.5/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/models/azure_openai.py` & `scrapegraphai-0.2.5/scrapegraphai/models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/models/gemini.py` & `scrapegraphai-0.2.5/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/models/hugging_face.py` & `scrapegraphai-0.2.5/scrapegraphai/models/hugging_face.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/models/ollama.py` & `scrapegraphai-0.2.5/scrapegraphai/models/ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/models/openai.py` & `scrapegraphai-0.2.5/scrapegraphai/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.2.5/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.2.5/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.2.5/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.2.5/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.2.5/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.2.5/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.2.5/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.2.5/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.2.5/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.2.5/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.2.5/scrapegraphai/nodes/rag_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,15 +88,21 @@
 
         if isinstance(embedding_model, OpenAI):
             embeddings = OpenAIEmbeddings(
                 api_key=embedding_model.openai_api_key)
         elif isinstance(embedding_model, AzureOpenAI):
             embeddings = AzureOpenAIEmbeddings()
         elif isinstance(embedding_model, Ollama):
-            embeddings = OllamaEmbeddings(model=embedding_model.model)
+            # unwrap the kwargs from the model whihc is a dict
+            params = embedding_model._lc_kwargs
+            # remove streaming and temperature
+            params.pop("streaming", None)
+            params.pop("temperature", None)
+            
+            embeddings = OllamaEmbeddings(**params)
         elif isinstance(embedding_model, HuggingFace):
             embeddings = HuggingFaceHubEmbeddings(model=embedding_model.model)
         else:
             raise ValueError("Embedding Model missing or not supported")
 
         retriever = FAISS.from_documents(
             chunked_docs, embeddings).as_retriever()
```

### Comparing `scrapegraphai-0.2.4/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.2.5/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.2.5/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.2.5/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.2.5/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.2.5/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.2.5/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/utils/remover.py` & `scrapegraphai-0.2.5/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.2.5/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.2.5/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.2.5/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.4/PKG-INFO` & `scrapegraphai-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.2.4
+Version: 0.2.5
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >3.9,<4.0
```


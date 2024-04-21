# Comparing `tmp/llmflex-0.1.4.tar.gz` & `tmp/llmflex-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmflex-0.1.4.tar", last modified: Sun Apr 14 12:29:51 2024, max compression
+gzip compressed data, was "llmflex-0.1.5.tar", last modified: Sun Apr 21 17:43:26 2024, max compression
```

## Comparing `llmflex-0.1.4.tar` & `llmflex-0.1.5.tar`

### file list

```diff
@@ -1,71 +1,76 @@
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.553269 llmflex-0.1.4/
--rw-r--r--   0 nathan95   (501) staff       (20)     1067 2024-01-22 01:35:14.000000 llmflex-0.1.4/LICENSE.md
--rw-r--r--   0 nathan95   (501) staff       (20)     9757 2024-04-14 12:29:51.553024 llmflex-0.1.4/PKG-INFO
--rw-r--r--   0 nathan95   (501) staff       (20)     8569 2024-04-09 19:26:07.000000 llmflex-0.1.4/README.md
--rw-r--r--   0 nathan95   (501) staff       (20)     1203 2024-04-14 12:29:06.000000 llmflex-0.1.4/pyproject.toml
--rw-r--r--   0 nathan95   (501) staff       (20)       38 2024-04-14 12:29:51.553312 llmflex-0.1.4/setup.cfg
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.543876 llmflex-0.1.4/src/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.545837 llmflex-0.1.4/src/llmflex/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.547019 llmflex-0.1.4/src/llmflex/Data/
--rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Data/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4919 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Data/sqlite_database.py
--rw-r--r--   0 nathan95   (501) staff       (20)    20029 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Data/vector_database.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.547747 llmflex-0.1.4/src/llmflex/Embeddings/
--rw-r--r--   0 nathan95   (501) staff       (20)      226 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Embeddings/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4400 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Embeddings/api_embeddings.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4245 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Embeddings/base_embeddings.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2275 2024-03-15 22:38:26.000000 llmflex-0.1.4/src/llmflex/Embeddings/hf_embeddings_server.py
--rw-r--r--   0 nathan95   (501) staff       (20)     3998 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Embeddings/huggingface_embeddings.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.548179 llmflex-0.1.4/src/llmflex/Frontend/
--rw-r--r--   0 nathan95   (501) staff       (20)      102 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Frontend/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    29992 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Frontend/gradio_interface.py
--rw-r--r--   0 nathan95   (501) staff       (20)    37412 2024-04-14 12:29:06.000000 llmflex-0.1.4/src/llmflex/Frontend/streamlit_interface.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.548680 llmflex-0.1.4/src/llmflex/Memory/
--rw-r--r--   0 nathan95   (501) staff       (20)      287 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Memory/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     8298 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Memory/assistant_long_term_memory.py
--rw-r--r--   0 nathan95   (501) staff       (20)     8703 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Memory/base_memory.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7727 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Memory/long_short_memory.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.548831 llmflex-0.1.4/src/llmflex/Models/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.549928 llmflex-0.1.4/src/llmflex/Models/Cores/
--rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Models/Cores/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    14710 2024-04-14 12:29:06.000000 llmflex-0.1.4/src/llmflex/Models/Cores/base_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7915 2024-02-25 22:17:53.000000 llmflex-0.1.4/src/llmflex/Models/Cores/exllamav2_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     9508 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Models/Cores/huggingface_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     8610 2024-02-25 22:17:53.000000 llmflex-0.1.4/src/llmflex/Models/Cores/llamacpp_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     9425 2024-04-14 12:29:06.000000 llmflex-0.1.4/src/llmflex/Models/Cores/openai_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7368 2024-02-28 15:01:21.000000 llmflex-0.1.4/src/llmflex/Models/Cores/utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.550168 llmflex-0.1.4/src/llmflex/Models/Factory/
--rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Models/Factory/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    10723 2024-04-14 12:29:06.000000 llmflex-0.1.4/src/llmflex/Models/Factory/llm_factory.py
--rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Models/__init__.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.550433 llmflex-0.1.4/src/llmflex/Prompts/
--rw-r--r--   0 nathan95   (501) staff       (20)       52 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Prompts/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    14910 2024-04-09 19:26:07.000000 llmflex-0.1.4/src/llmflex/Prompts/prompt_template.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.550681 llmflex-0.1.4/src/llmflex/Schemas/
--rw-r--r--   0 nathan95   (501) staff       (20)       31 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Schemas/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)      140 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Schemas/documents.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.551226 llmflex-0.1.4/src/llmflex/TextSplitters/
--rw-r--r--   0 nathan95   (501) staff       (20)      123 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/TextSplitters/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1526 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/TextSplitters/base_text_splitter.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2709 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/TextSplitters/sentence_token_text_splitter.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1485 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/TextSplitters/token_text_splitter.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.551822 llmflex-0.1.4/src/llmflex/Tools/
--rw-r--r--   0 nathan95   (501) staff       (20)      115 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Tools/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    11795 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Tools/base_tool.py
--rw-r--r--   0 nathan95   (501) staff       (20)     6603 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Tools/tool_selection.py
--rw-r--r--   0 nathan95   (501) staff       (20)    11406 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Tools/web_search_tool.py
--rw-r--r--   0 nathan95   (501) staff       (20)    14418 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Tools/web_search_utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.552226 llmflex-0.1.4/src/llmflex/VectorDBs/
--rw-r--r--   0 nathan95   (501) staff       (20)       93 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/VectorDBs/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    23515 2024-04-09 19:26:07.000000 llmflex-0.1.4/src/llmflex/VectorDBs/base_vectordb.py
--rw-r--r--   0 nathan95   (501) staff       (20)     5018 2024-04-09 19:26:07.000000 llmflex-0.1.4/src/llmflex/VectorDBs/faiss_vectordb.py
--rw-r--r--   0 nathan95   (501) staff       (20)      275 2024-04-14 12:29:06.000000 llmflex-0.1.4/src/llmflex/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4381 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/cli.py
--rw-r--r--   0 nathan95   (501) staff       (20)     6178 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.552423 llmflex-0.1.4/src/llmflex.egg-info/
--rw-r--r--   0 nathan95   (501) staff       (20)     9757 2024-04-14 12:29:51.000000 llmflex-0.1.4/src/llmflex.egg-info/PKG-INFO
--rw-r--r--   0 nathan95   (501) staff       (20)     1903 2024-04-14 12:29:51.000000 llmflex-0.1.4/src/llmflex.egg-info/SOURCES.txt
--rw-r--r--   0 nathan95   (501) staff       (20)        1 2024-04-14 12:29:51.000000 llmflex-0.1.4/src/llmflex.egg-info/dependency_links.txt
--rw-r--r--   0 nathan95   (501) staff       (20)       44 2024-04-14 12:29:51.000000 llmflex-0.1.4/src/llmflex.egg-info/entry_points.txt
--rw-r--r--   0 nathan95   (501) staff       (20)      330 2024-04-14 12:29:51.000000 llmflex-0.1.4/src/llmflex.egg-info/requires.txt
--rw-r--r--   0 nathan95   (501) staff       (20)        8 2024-04-14 12:29:51.000000 llmflex-0.1.4/src/llmflex.egg-info/top_level.txt
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.245627 llmflex-0.1.5/
+-rw-r--r--   0 nathan95   (501) staff       (20)     1067 2024-01-22 01:35:14.000000 llmflex-0.1.5/LICENSE.md
+-rw-r--r--   0 nathan95   (501) staff       (20)     9764 2024-04-21 17:43:26.245377 llmflex-0.1.5/PKG-INFO
+-rw-r--r--   0 nathan95   (501) staff       (20)     8569 2024-04-09 19:26:07.000000 llmflex-0.1.5/README.md
+-rw-r--r--   0 nathan95   (501) staff       (20)     1210 2024-04-21 17:42:51.000000 llmflex-0.1.5/pyproject.toml
+-rw-r--r--   0 nathan95   (501) staff       (20)       38 2024-04-21 17:43:26.245668 llmflex-0.1.5/setup.cfg
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.235267 llmflex-0.1.5/src/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.237067 llmflex-0.1.5/src/llmflex/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.238376 llmflex-0.1.5/src/llmflex/Data/
+-rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/Data/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4919 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Data/sqlite_database.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    20029 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/Data/vector_database.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.239098 llmflex-0.1.5/src/llmflex/Embeddings/
+-rw-r--r--   0 nathan95   (501) staff       (20)      226 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Embeddings/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4555 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Embeddings/api_embeddings.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4608 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Embeddings/base_embeddings.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2275 2024-03-15 22:38:26.000000 llmflex-0.1.5/src/llmflex/Embeddings/hf_embeddings_server.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4147 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Embeddings/huggingface_embeddings.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.239535 llmflex-0.1.5/src/llmflex/Frontend/
+-rw-r--r--   0 nathan95   (501) staff       (20)      102 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Frontend/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    29992 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Frontend/gradio_interface.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    37412 2024-04-14 12:29:06.000000 llmflex-0.1.5/src/llmflex/Frontend/streamlit_interface.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.240049 llmflex-0.1.5/src/llmflex/Memory/
+-rw-r--r--   0 nathan95   (501) staff       (20)      287 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Memory/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     8298 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/Memory/assistant_long_term_memory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     8703 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/Memory/base_memory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     7727 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/Memory/long_short_memory.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.240161 llmflex-0.1.5/src/llmflex/Models/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.241073 llmflex-0.1.5/src/llmflex/Models/Cores/
+-rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Models/Cores/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    14710 2024-04-14 12:29:06.000000 llmflex-0.1.5/src/llmflex/Models/Cores/base_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     7915 2024-02-25 22:17:53.000000 llmflex-0.1.5/src/llmflex/Models/Cores/exllamav2_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     9508 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/Models/Cores/huggingface_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     8610 2024-02-25 22:17:53.000000 llmflex-0.1.5/src/llmflex/Models/Cores/llamacpp_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     9425 2024-04-14 12:29:06.000000 llmflex-0.1.5/src/llmflex/Models/Cores/openai_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     7398 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Models/Cores/utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.241305 llmflex-0.1.5/src/llmflex/Models/Factory/
+-rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Models/Factory/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    10723 2024-04-14 12:29:06.000000 llmflex-0.1.5/src/llmflex/Models/Factory/llm_factory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Models/__init__.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.241722 llmflex-0.1.5/src/llmflex/Prompts/
+-rw-r--r--   0 nathan95   (501) staff       (20)       52 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Prompts/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    15747 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Prompts/prompt_template.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.242257 llmflex-0.1.5/src/llmflex/Rankers/
+-rw-r--r--   0 nathan95   (501) staff       (20)       81 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Rankers/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1471 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Rankers/base_ranker.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2309 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Rankers/flashrank_ranker.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.242705 llmflex-0.1.5/src/llmflex/Schemas/
+-rw-r--r--   0 nathan95   (501) staff       (20)       64 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Schemas/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1414 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Schemas/documents.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2429 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Schemas/tokenizer.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.243285 llmflex-0.1.5/src/llmflex/TextSplitters/
+-rw-r--r--   0 nathan95   (501) staff       (20)      123 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/TextSplitters/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1526 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/TextSplitters/base_text_splitter.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2709 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/TextSplitters/sentence_token_text_splitter.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1423 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/TextSplitters/token_text_splitter.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.244035 llmflex-0.1.5/src/llmflex/Tools/
+-rw-r--r--   0 nathan95   (501) staff       (20)      115 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Tools/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    11795 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Tools/base_tool.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     6603 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/Tools/tool_selection.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    11421 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Tools/web_search_tool.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    14485 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Tools/web_search_utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.244560 llmflex-0.1.5/src/llmflex/VectorDBs/
+-rw-r--r--   0 nathan95   (501) staff       (20)       93 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/VectorDBs/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    24481 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/VectorDBs/base_vectordb.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     5362 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/VectorDBs/faiss_vectordb.py
+-rw-r--r--   0 nathan95   (501) staff       (20)      275 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4381 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/cli.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     6178 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.244774 llmflex-0.1.5/src/llmflex.egg-info/
+-rw-r--r--   0 nathan95   (501) staff       (20)     9764 2024-04-21 17:43:26.000000 llmflex-0.1.5/src/llmflex.egg-info/PKG-INFO
+-rw-r--r--   0 nathan95   (501) staff       (20)     2043 2024-04-21 17:43:26.000000 llmflex-0.1.5/src/llmflex.egg-info/SOURCES.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)        1 2024-04-21 17:43:26.000000 llmflex-0.1.5/src/llmflex.egg-info/dependency_links.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)       44 2024-04-21 17:43:26.000000 llmflex-0.1.5/src/llmflex.egg-info/entry_points.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)      337 2024-04-21 17:43:26.000000 llmflex-0.1.5/src/llmflex.egg-info/requires.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)        8 2024-04-21 17:43:26.000000 llmflex-0.1.5/src/llmflex.egg-info/top_level.txt
```

### Comparing `llmflex-0.1.4/LICENSE.md` & `llmflex-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/PKG-INFO` & `llmflex-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmflex
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python package for developing AI applications with local LLMs.
 Author-email: Nathan Tam <nathan1295@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nath1295/LLMFlex
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -22,15 +22,15 @@
 Requires-Dist: fake-useragent
 Requires-Dist: openai>=1.0.0
 Requires-Dist: tiktoken
 Requires-Dist: protobuf
 Requires-Dist: beautifulsoup4
 Requires-Dist: streamlit
 Requires-Dist: watchdog
-Requires-Dist: spacy
+Requires-Dist: spacy>=3.7.0
 Requires-Dist: flask
 Provides-Extra: cu121
 Requires-Dist: auto-gptq>=0.6.0; extra == "cu121"
 Requires-Dist: autoawq; extra == "cu121"
 Requires-Dist: exllamav2; extra == "cu121"
 Provides-Extra: cu118
 Requires-Dist: auto-gptq; extra == "cu118"
```

### Comparing `llmflex-0.1.4/README.md` & `llmflex-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/pyproject.toml` & `llmflex-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "fake-useragent",
     "openai>=1.0.0",
     "tiktoken",
     "protobuf",
     "beautifulsoup4",
     "streamlit",
     "watchdog",
-    "spacy",
+    "spacy>=3.7.0",
     "flask"
 ]
 
 [project.urls]
 Homepage = "https://github.com/nath1295/LLMFlex"
 
 [project.scripts]
```

### Comparing `llmflex-0.1.4/src/llmflex/Data/sqlite_database.py` & `llmflex-0.1.5/src/llmflex/Data/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/Data/vector_database.py` & `llmflex-0.1.5/src/llmflex/Data/vector_database.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/Embeddings/api_embeddings.py` & `llmflex-0.1.5/src/llmflex/Embeddings/api_embeddings.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,24 +50,26 @@
             chunk_size (Optional[int], optional): Chunk size for the text splitter. If not provided, the min of the model max_seq_length or 512 will be used. Defaults to None.
             chunk_overlap_perc (float, optional): Number of tokens percentage overlap during text splitting. Defaults to 0.1.
             encode_kwargs (Optional[Dict[str, Any]], optional): Keyword arguments for encoding text. If None is given, the default is normalize_embeddings=True, batch_size=128. Defaults to None.
             tokenizer_kwargs (Optional[Dict[str, Any]], optional): Keyword arguments for loading tokenizer. Defaults to None.
         """
         from ..utils import get_config
         from ..TextSplitters.token_text_splitter import TokenCountTextSplitter
+        from ..Schemas.tokenizer import Tokenizer
         os.environ['HF_HOME'] = get_config()['hf_home']
         os.environ['TOKENIZERS_PARALLELISM'] = 'true'
         from transformers import AutoTokenizer
         encode_kwargs = dict(normalize_embeddings=True, batch_size=128) if encode_kwargs is None else encode_kwargs
         embedding_model = APIEmbeddings(base_url=base_url, encode_kwargs=encode_kwargs)
         name = embedding_model.info['model_id']
         type = 'api_embeddings'
         embedding_size = embedding_model.info['embedding_dimension']
         max_seq_length = embedding_model.info['max_seq_length']
         chunk_size = min(max_seq_length, 512) if not isinstance(chunk_size, int) else chunk_size
         tokenizer_kwargs = dict() if tokenizer_kwargs is None else tokenizer_kwargs
         tokenizer = AutoTokenizer.from_pretrained(name, **tokenizer_kwargs)
         encode_fn = lambda x: tokenizer.encode(x, add_special_tokens=False)
         decode_fn = lambda x: tokenizer.decode(x, skip_special_tokens=True)
+        lf_tokenizer = Tokenizer(tokenize_fn=encode_fn, detokenize_fn=decode_fn)
         text_splitter = TokenCountTextSplitter(encode_fn=encode_fn, decode_fn=decode_fn, chunk_overlap=int(chunk_size * chunk_overlap_perc), chunk_size=chunk_size)
-        super().__init__(embedding_model = embedding_model, text_splitter = text_splitter, name = name, 
+        super().__init__(embedding_model = embedding_model, text_splitter = text_splitter, tokenizer=lf_tokenizer, name = name, 
                          type = type, embedding_size = embedding_size, max_seq_length = max_seq_length)
```

### Comparing `llmflex-0.1.4/src/llmflex/Embeddings/base_embeddings.py` & `llmflex-0.1.5/src/llmflex/Embeddings/base_embeddings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ..TextSplitters.base_text_splitter import BaseTextSplitter
+from ..Schemas.tokenizer import Tokenizer
 from langchain.embeddings.base import Embeddings
 from abc import ABC, abstractmethod
 import numpy as np
 from typing import List, Type
 
 class BaseEmbeddings(ABC):
     """Base class for embeddings model.
@@ -42,18 +43,20 @@
     
     def embed_query(self, text: str) -> List[float]:
         return self._model.embed_query(text=text)
 
 class BaseEmbeddingsToolkit:
     """Base class for storing the embedding model and the text splitter.
     """
-    def __init__(self, embedding_model: Type[BaseEmbeddings], text_splitter: Type[BaseTextSplitter], name: str, type: str, embedding_size: int, max_seq_length: int) -> None:
+    def __init__(self, embedding_model: Type[BaseEmbeddings], text_splitter: Type[BaseTextSplitter], tokenizer: Tokenizer,
+                 name: str, type: str, embedding_size: int, max_seq_length: int) -> None:
         from ..utils import validate_type
         self._embedding_model = validate_type(embedding_model, BaseEmbeddings)
         self._text_splitter = validate_type(text_splitter, BaseTextSplitter)
+        self._tokenizer = validate_type(tokenizer, Tokenizer)
         self._name = validate_type(name, str)
         self._type = validate_type(type, str)
         self._embedding_size = validate_type(embedding_size, int)
         self._max_seq_length = validate_type(max_seq_length, int)
 
     @property
     def embedding_model(self) -> BaseEmbeddings:
@@ -70,14 +73,23 @@
 
         Returns:
             BaseTextSplitter: The text splitter.
         """
         return self._text_splitter
     
     @property
+    def tokenizer(self) -> Tokenizer:
+        """Tokenizer of the embedding model.
+
+        Returns:
+            Tokenizer: Tokenizer of the embedding model.
+        """
+        return self._tokenizer
+    
+    @property
     def embedding_size(self) -> int:
         """The embedding model's output dimensions.
 
         Returns:
             int: The embedding model's output dimensions.
         """
         return self._embedding_size
```

### Comparing `llmflex-0.1.4/src/llmflex/Embeddings/hf_embeddings_server.py` & `llmflex-0.1.5/src/llmflex/Embeddings/hf_embeddings_server.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/Embeddings/huggingface_embeddings.py` & `llmflex-0.1.5/src/llmflex/Embeddings/huggingface_embeddings.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,16 +48,18 @@
             model_id (str): Model id (from Huggingface) to use.
             chunk_size (Optional[int], optional): Chunk size for the text splitter. If not provided, the min of the model max_seq_length or 512 will be used. Defaults to None.
             chunk_overlap_perc (float, optional): Number of tokens percentage overlap during text splitting. Defaults to 0.1.
             model_kwargs (Optional[Dict[str, Any]], optional): Keyword arguments for loading the model. Defaults to None.
             encode_kwargs (Optional[Dict[str, Any]], optional): Keyword arguments for encoding text. If None is given, the default is normalize_embeddings=True, batch_size=128. Defaults to None.
         """
         from ..TextSplitters.token_text_splitter import TokenCountTextSplitter
+        from ..Schemas.tokenizer import Tokenizer
         embedding_model = HuggingFaceEmbeddings(model_name=model_id, model_kwargs=model_kwargs, encode_kwargs=encode_kwargs)
         name = model_id
         type = 'huggingface_embeddings'
         chunk_size = min(embedding_model._max_seq_length, 512) if not isinstance(chunk_size, int) else chunk_size
         encode_fn = lambda x: embedding_model._tokenizer.encode(x, add_special_tokens=False)
         decode_fn = lambda x: embedding_model._tokenizer.decode(x, skip_special_tokens=True)
+        tokenizer = Tokenizer(tokenize_fn=encode_fn, detokenize_fn=decode_fn)
         text_splitter = TokenCountTextSplitter(encode_fn=encode_fn, decode_fn=decode_fn, chunk_overlap=int(chunk_size * chunk_overlap_perc), chunk_size=chunk_size)
-        super().__init__(embedding_model = embedding_model, text_splitter = text_splitter, name = name, 
+        super().__init__(embedding_model = embedding_model, text_splitter = text_splitter, tokenizer=tokenizer, name = name, 
                          type = type, embedding_size = embedding_model._embedding_size, max_seq_length = embedding_model._max_seq_length)
```

### Comparing `llmflex-0.1.4/src/llmflex/Frontend/gradio_interface.py` & `llmflex-0.1.5/src/llmflex/Frontend/gradio_interface.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/Frontend/streamlit_interface.py` & `llmflex-0.1.5/src/llmflex/Frontend/streamlit_interface.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/Memory/assistant_long_term_memory.py` & `llmflex-0.1.5/src/llmflex/Memory/assistant_long_term_memory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/Memory/base_memory.py` & `llmflex-0.1.5/src/llmflex/Memory/base_memory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/Memory/long_short_memory.py` & `llmflex-0.1.5/src/llmflex/Memory/long_short_memory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/Models/Cores/base_core.py` & `llmflex-0.1.5/src/llmflex/Models/Cores/base_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/Models/Cores/exllamav2_core.py` & `llmflex-0.1.5/src/llmflex/Models/Cores/exllamav2_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/Models/Cores/huggingface_core.py` & `llmflex-0.1.5/src/llmflex/Models/Cores/huggingface_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/Models/Cores/llamacpp_core.py` & `llmflex-0.1.5/src/llmflex/Models/Cores/llamacpp_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/Models/Cores/openai_core.py` & `llmflex-0.1.5/src/llmflex/Models/Cores/openai_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/Models/Cores/utils.py` & `llmflex-0.1.5/src/llmflex/Models/Cores/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,19 +118,20 @@
         hermes = 'ChatML',
         nous = 'ChatML',
         wizardlm = 'Vicuna',
         openchat = 'OpenChat',
         zephyr = 'Zephyr',
         solar = 'Llama2'
     )
-    base = dict(
-        llama = 'Llama2',
-        mistral = 'Llama2',
-        mixtral = 'Llama2'
-    )
+    base = {
+        'llama-3': 'Llama3',
+        'llama-2': 'Llama2',
+        'mistral': 'Llama2',
+        'mixtral': 'Llama2'
+    }
     id_lower = model_id.lower()
 
     # Check if it is in the finetune list
     keys = list(map(lambda x: (x, id_lower.find(x)), finetunes.keys()))
     keys.sort(key=lambda x: x[1])
     keys = list(filter(lambda x: x[1]!=-1, keys))
     if len(keys) != 0:
```

### Comparing `llmflex-0.1.4/src/llmflex/Models/Factory/llm_factory.py` & `llmflex-0.1.5/src/llmflex/Models/Factory/llm_factory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/Prompts/prompt_template.py` & `llmflex-0.1.5/src/llmflex/Prompts/prompt_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,75 @@
 from __future__ import annotations
 from jinja2 import Environment
 from typing import List, Dict, Any, Optional, Literal, Union, Tuple
 
 DEFAULT_SYSTEM_MESSAGE = """This is a conversation between a human user and a helpful AI assistant."""
 
+presets = {
+    'Default' : {
+        'template': "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{{ 'SYSTEM:\n' + messages[0]['content'].strip() + '\n\n' }}{% else %}{% set loop_messages = messages %}{% endif %}{% for message in loop_messages %}{% if message['role'] == 'user' %}{{ 'USER: ' + message['content'].strip() + '\n' }}{% elif message['role'] == 'assistant' %}{{ 'ASSISTANT: ' + message['content'].strip() + '\n' }}{% endif %}{% endfor %}{% if add_generation_prompt %}{{ 'ASSISTANT:' }}{% endif %}",
+        'eos_token': '</s>',
+        'bos_token': '<s>',
+        'stop': ['\nASSISTANT', '\nUSER:', 'ASSISTANT:', 'USER:']
+    },
+    'Llama2' : {
+        'template': "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'] %}{% elif false == true and not '<<SYS>>' in messages[0]['content'] %}{% set loop_messages = messages %}{% set system_message = 'You are a helpful, respectful and honest assistant. Always answer as helpfully as possible, while being safe. Your answers should not include any harmful, unethical, racist, sexist, toxic, dangerous, or illegal content. Please ensure that your responses are socially unbiased and positive in nature.\\n\\nIf a question does not make any sense, or is not factually coherent, explain why instead of answering something not correct. If you don\\'t know the answer to a question, please don\\'t share false information.' %}{% else %}{% set loop_messages = messages %}{% set system_message = false %}{% endif %}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if loop.index0 == 0 and system_message != false %}{% set content = '<<SYS>>\\n' + system_message + '\\n<</SYS>>\\n\\n' + message['content'] %}{% else %}{% set content = message['content'] %}{% endif %}{% if message['role'] == 'user' %}{{ bos_token + '[INST] ' + content.strip() + ' [/INST]' }}{% elif message['role'] == 'system' %}{{ '<<SYS>>\\n' + content.strip() + '\\n<</SYS>>\\n\\n' }}{% elif message['role'] == 'assistant' %}{{ ' '  + content.strip() + ' ' + eos_token }}{% endif %}{% endfor %}",
+        'eos_token': '</s>',
+        'bos_token': '<s>',
+        'stop': ['</s>', '</s><s>', '[INST]', '<s>[INST]']
+    },
+    'Llama3' : {
+        'template': "{% if not add_generation_prompt is defined %}{% set add_generation_prompt = false %}{% endif %}{% set loop_messages = messages %}{% for message in loop_messages %}{% set content = '<|start_header_id|>' + message['role'] + '<|end_header_id|>\n\n'+ message['content'] | trim + '<|eot_id|>' %}{% if loop.index0 == 0 %}{% set content = bos_token + content %}{% endif %}{{ content }}{% endfor %}{% if add_generation_prompt %}{{ '<|start_header_id|>assistant<|end_header_id|>\n\n' }}{% else %}{{ eos_token }}{% endif %}",
+        'eos_token': '<|end_of_text|>',
+        'bos_token': '<|begin_of_text|>',
+        'stop': ['</s>', '<|end_of_text|>', '<|eot_id|>', '<|start_header_id|>']
+    },
+    'Vicuna' : {
+        'template': "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{{ messages[0]['content'].strip() + '\n\n' }}{% else %}{% set loop_messages = messages %}{% endif %}{% for message in loop_messages %}{% if message['role'] == 'user' %}{{ 'USER: ' + message['content'].strip() + '\n' }}{% elif message['role'] == 'assistant' %}{{ 'ASSISTANT: ' + message['content'].strip() + eos_token + '\n' }}{% endif %}{% endfor %}{% if add_generation_prompt %}{{ 'ASSISTANT:' }}{% endif %}",
+        'eos_token': '</s>',
+        'bos_token': '<s>',
+        'stop': ['\nASSISTANT', '\nUSER:', 'ASSISTANT:', 'USER:', '</s>']
+    },
+    'ChatML' : {
+        'template': "{% for message in messages %}{{'<|im_start|>' + message['role'] + '\n' + message['content'] + '<|im_end|>' + '\n'}}{% endfor %}{% if add_generation_prompt %}{{ '<|im_start|>assistant\n' }}{% endif %}",
+        'eos_token': '<|im_end|>',
+        'bos_token': '<|endoftext|>',
+        'stop': ['<|im_start|>', '<|im_end|>', '<|im_start|>user\n', '<|im_end|>\n<|im_start|>user\n', '</s>']
+    },
+    'Zephyr' : {
+        'template': "{% for message in messages %}\n{% if message['role'] == 'user' %}\n{{ '<|user|>\n' + message['content'] + eos_token }}\n{% elif message['role'] == 'system' %}\n{{ '<|system|>\n' + message['content'] + eos_token }}\n{% elif message['role'] == 'assistant' %}\n{{ '<|assistant|>\n'  + message['content'] + eos_token }}\n{% endif %}\n{% if loop.last and add_generation_prompt %}\n{{ '<|assistant|>' }}\n{% endif %}\n{% endfor %}",
+        'eos_token': '</s>',
+        'bos_token': '<s>',
+        'stop': ['</s>', '</s>\n', '<|user|>\n', '</s>\n<|user|>\n']
+    },
+    'OpenChat' : {
+        'template': "{{ bos_token }}{% for message in messages %}{{ 'GPT4 Correct ' + message['role'].title() + ': ' + message['content'] + '<|end_of_turn|>'}}{% endfor %}{% if add_generation_prompt %}{{ 'GPT4 Correct Assistant:' }}{% endif %}",
+        'eos_token': '<|end_of_turn|>',
+        'bos_token': '<s>',
+        'stop': ['</s>', '<|end_of_turn|>', '<|end_of_turn|>GPT4 Correct Assistant: ']
+    },
+    'Alpaca' : {
+        'template': "{% for message in messages %}{% if message['role'] == 'system' %}{% if message['content']%}{{'### Instruction: ' + message['content']+'\n'}}{% endif %}{% elif message['role'] == 'user' %}{{'### Input: ' + message['content']+'\n'}}{% elif message['role'] == 'assistant' %}{{'### Response: '  + message['content'] + '\n'}}{% endif %}{% if loop.last and add_generation_prompt %}{{ '### Response:' }}{% endif %}{% endfor %}",
+        'eos_token': '<|end_of_turn|>',
+        'bos_token': '<s>',
+        'stop': ['### Input: ', '\n### Input: ', '###']
+    },
+}
+
+hidden_presets = {
+    'Llama2' : {
+        'template': "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'] %}{% else %}{% set loop_messages = messages %}{% set system_message = false %}{% endif %}{% for message in loop_messages %}{% if loop.index0 == 0 and system_message != false %}{% set content = '<<SYS>>\\n' + system_message + '\\n<</SYS>>\\n\\n' + message['content'] %}{% else %}{% set content = message['content'] %}{% endif %}{% if message['role'] == 'user' %}{% if loop.index0 == 0 %}{{ '[INST] ' + content.strip() + ' [/INST]' }}{% else %}{{ bos_token + '[INST] ' + content.strip() + ' [/INST]' }}{% endif %}{% elif message['role'] == 'system' %}{{ '<<SYS>>\\n' + content.strip() + '\\n<</SYS>>\\n\\n' }}{% elif message['role'] == 'assistant' %}{% if loop.index0 == 0 and system_message != false %}{% set prefix = '[INST]' + '<<SYS>>\\n' + system_message + '\\n<</SYS>>\\n\\n' + '[/INST] ' %}{% set content = message['content'] %}{% elif loop.index0 == 0 %}{% set prefix = '[INST][/INST] ' %}{% set content = message['content'] %}{% else %}{% set prefix = ' ' %}{% endif %}{{ prefix  + content.strip() + ' ' + eos_token }}{% endif %}{% endfor %}",
+        'eos_token': '</s>',
+        'bos_token': '<s>',
+        'stop': ['</s>', '</s><s>', '[INST]', '<s>[INST]']
+    }
+}
+
+PRESET_FORMATS =  Literal['Default', 'Llama2', 'Llama3', 'Vicuna', 'ChatML', 'Zephyr', 'OpenChat', 'Alpaca']
+
 class PromptTemplate:
     """Class for storing prompt format presets.
     """
     def __init__(
             self,
             template: str,
             eos_token: Optional[str],
@@ -161,19 +223,20 @@
         Returns:
             PromptTemplatet: The initialised PromptTemplate instance.
         """
         from ..utils import read_json
         return cls.from_dict(read_json(file_dir=file_dir), template_name=file_dir)
     
     @classmethod
-    def from_preset(cls, style: Literal['Default', 'Llama2', 'Vicuna', 'ChatML', 'Zephyr', 'OpenChat', 'Alpaca'], force_real_template: bool = False) -> PromptTemplate:
+    def from_preset(cls, style: PRESET_FORMATS, force_real_template: bool = False) -> PromptTemplate:
         """Initialise the prompt template from a preset.
 
         Args:
-            style (Literal[&#39;Default&#39;, &#39;Llama2&#39;, &#39;Vicuna&#39;, &#39;ChatML&#39;, &#39;Zephyr&#39;, &#39;OpenChat&#39;, &#39;Alpaca&#39;]): Format of the prompt.
+            style (PRESET_FORMATS): Format of the prompt.
+            force_real_template (bool, optional): Whether to render the given template. For most templates it has no effects. Only for some restrictive templates like llama2. Defaults to False.
 
         Returns:
             PromptTemplate: The initialised PromptTemplate instance.
         """
         from copy import deepcopy
         preset = deepcopy(presets[style])
         preset['force_real_template'] = force_real_template
@@ -187,61 +250,7 @@
         """
         return dict(
             template = self.template,
             eos_token = self.eos_token,
             bos_token = self.bos_token,
             stop = self.stop if self.stop is not None else [self.eos_token]
         )
-    
-presets = {
-    'Default' : {
-        'template': "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{{ 'SYSTEM:\n' + messages[0]['content'].strip() + '\n\n' }}{% else %}{% set loop_messages = messages %}{% endif %}{% for message in loop_messages %}{% if message['role'] == 'user' %}{{ 'USER: ' + message['content'].strip() + '\n' }}{% elif message['role'] == 'assistant' %}{{ 'ASSISTANT: ' + message['content'].strip() + '\n' }}{% endif %}{% endfor %}{% if add_generation_prompt %}{{ 'ASSISTANT:' }}{% endif %}",
-        'eos_token': '</s>',
-        'bos_token': '<s>',
-        'stop': ['\nASSISTANT', '\nUSER:', 'ASSISTANT:', 'USER:']
-    },
-    'Llama2' : {
-        'template': "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'] %}{% elif false == true and not '<<SYS>>' in messages[0]['content'] %}{% set loop_messages = messages %}{% set system_message = 'You are a helpful, respectful and honest assistant. Always answer as helpfully as possible, while being safe. Your answers should not include any harmful, unethical, racist, sexist, toxic, dangerous, or illegal content. Please ensure that your responses are socially unbiased and positive in nature.\\n\\nIf a question does not make any sense, or is not factually coherent, explain why instead of answering something not correct. If you don\\'t know the answer to a question, please don\\'t share false information.' %}{% else %}{% set loop_messages = messages %}{% set system_message = false %}{% endif %}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if loop.index0 == 0 and system_message != false %}{% set content = '<<SYS>>\\n' + system_message + '\\n<</SYS>>\\n\\n' + message['content'] %}{% else %}{% set content = message['content'] %}{% endif %}{% if message['role'] == 'user' %}{{ bos_token + '[INST] ' + content.strip() + ' [/INST]' }}{% elif message['role'] == 'system' %}{{ '<<SYS>>\\n' + content.strip() + '\\n<</SYS>>\\n\\n' }}{% elif message['role'] == 'assistant' %}{{ ' '  + content.strip() + ' ' + eos_token }}{% endif %}{% endfor %}",
-        'eos_token': '</s>',
-        'bos_token': '<s>',
-        'stop': ['</s>', '</s><s>', '[INST]', '<s>[INST]']
-    },
-    'Vicuna' : {
-        'template': "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{{ messages[0]['content'].strip() + '\n\n' }}{% else %}{% set loop_messages = messages %}{% endif %}{% for message in loop_messages %}{% if message['role'] == 'user' %}{{ 'USER: ' + message['content'].strip() + '\n' }}{% elif message['role'] == 'assistant' %}{{ 'ASSISTANT: ' + message['content'].strip() + eos_token + '\n' }}{% endif %}{% endfor %}{% if add_generation_prompt %}{{ 'ASSISTANT:' }}{% endif %}",
-        'eos_token': '</s>',
-        'bos_token': '<s>',
-        'stop': ['\nASSISTANT', '\nUSER:', 'ASSISTANT:', 'USER:', '</s>']
-    },
-    'ChatML' : {
-        'template': "{% for message in messages %}{{'<|im_start|>' + message['role'] + '\n' + message['content'] + '<|im_end|>' + '\n'}}{% endfor %}{% if add_generation_prompt %}{{ '<|im_start|>assistant\n' }}{% endif %}",
-        'eos_token': '<|im_end|>',
-        'bos_token': '<|endoftext|>',
-        'stop': ['<|im_start|>', '<|im_end|>', '<|im_start|>user\n', '<|im_end|>\n<|im_start|>user\n', '</s>']
-    },
-    'Zephyr' : {
-        'template': "{% for message in messages %}\n{% if message['role'] == 'user' %}\n{{ '<|user|>\n' + message['content'] + eos_token }}\n{% elif message['role'] == 'system' %}\n{{ '<|system|>\n' + message['content'] + eos_token }}\n{% elif message['role'] == 'assistant' %}\n{{ '<|assistant|>\n'  + message['content'] + eos_token }}\n{% endif %}\n{% if loop.last and add_generation_prompt %}\n{{ '<|assistant|>' }}\n{% endif %}\n{% endfor %}",
-        'eos_token': '</s>',
-        'bos_token': '<s>',
-        'stop': ['</s>', '</s>\n', '<|user|>\n', '</s>\n<|user|>\n']
-    },
-    'OpenChat' : {
-        'template': "{{ bos_token }}{% for message in messages %}{{ 'GPT4 Correct ' + message['role'].title() + ': ' + message['content'] + '<|end_of_turn|>'}}{% endfor %}{% if add_generation_prompt %}{{ 'GPT4 Correct Assistant:' }}{% endif %}",
-        'eos_token': '<|end_of_turn|>',
-        'bos_token': '<s>',
-        'stop': ['</s>', '<|end_of_turn|>', '<|end_of_turn|>GPT4 Correct Assistant: ']
-    },
-    'Alpaca' : {
-        'template': "{% for message in messages %}{% if message['role'] == 'system' %}{% if message['content']%}{{'### Instruction: ' + message['content']+'\n'}}{% endif %}{% elif message['role'] == 'user' %}{{'### Input: ' + message['content']+'\n'}}{% elif message['role'] == 'assistant' %}{{'### Response: '  + message['content'] + '\n'}}{% endif %}{% if loop.last and add_generation_prompt %}{{ '### Response:' }}{% endif %}{% endfor %}",
-        'eos_token': '<|end_of_turn|>',
-        'bos_token': '<s>',
-        'stop': ['### Input: ', '\n### Input: ', '###']
-    },
-}
-
-hidden_presets = {
-    'Llama2' : {
-        'template': "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'] %}{% else %}{% set loop_messages = messages %}{% set system_message = false %}{% endif %}{% for message in loop_messages %}{% if loop.index0 == 0 and system_message != false %}{% set content = '<<SYS>>\\n' + system_message + '\\n<</SYS>>\\n\\n' + message['content'] %}{% else %}{% set content = message['content'] %}{% endif %}{% if message['role'] == 'user' %}{% if loop.index0 == 0 %}{{ '[INST] ' + content.strip() + ' [/INST]' }}{% else %}{{ bos_token + '[INST] ' + content.strip() + ' [/INST]' }}{% endif %}{% elif message['role'] == 'system' %}{{ '<<SYS>>\\n' + content.strip() + '\\n<</SYS>>\\n\\n' }}{% elif message['role'] == 'assistant' %}{% if loop.index0 == 0 and system_message != false %}{% set prefix = '[INST]' + '<<SYS>>\\n' + system_message + '\\n<</SYS>>\\n\\n' + '[/INST] ' %}{% set content = message['content'] %}{% elif loop.index0 == 0 %}{% set prefix = '[INST][/INST] ' %}{% set content = message['content'] %}{% else %}{% set prefix = ' ' %}{% endif %}{{ prefix  + content.strip() + ' ' + eos_token }}{% endif %}{% endfor %}",
-        'eos_token': '</s>',
-        'bos_token': '<s>',
-        'stop': ['</s>', '</s><s>', '[INST]', '<s>[INST]']
-    }
-}
```

### Comparing `llmflex-0.1.4/src/llmflex/TextSplitters/base_text_splitter.py` & `llmflex-0.1.5/src/llmflex/TextSplitters/base_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/TextSplitters/sentence_token_text_splitter.py` & `llmflex-0.1.5/src/llmflex/TextSplitters/sentence_token_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/TextSplitters/token_text_splitter.py` & `llmflex-0.1.5/src/llmflex/TextSplitters/token_text_splitter.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,23 +12,22 @@
 
         Args:
             encode_fn (Callable[[str], List[int]]): Function of encode a string.
             decode_fn (Callable[[List[int]], str]): Function to decode a list of token ids.
             chunk_size (int, optional): Maximum number of tokens per text chunk. Defaults to 400.
             chunk_overlap (int, optional): Numbers of tokens that overlaps for each subsequent chunks. Defaults to 40.
         """
-        from langchain.text_splitter import Tokenizer
+        from ..Schemas.tokenizer import Tokenizer
         super().__init__(chunk_size=chunk_size, chunk_overlap=chunk_overlap)
-        self._tokenizer = Tokenizer(chunk_overlap=chunk_overlap, tokens_per_chunk=chunk_size, decode=decode_fn, encode=encode_fn)
+        self._tokenizer = Tokenizer(tokenize_fn=encode_fn, detokenize_fn=decode_fn)
 
     def split_text(self, text: str) -> List[str]:
         """Splitting the given text.
 
         Args:
             text (str): Text to split.
 
         Returns:
             List[str]: List of split texts.
         """
-        from langchain.text_splitter import split_text_on_tokens
-        chunks = split_text_on_tokens(text=text, tokenizer=self._tokenizer)
+        chunks = self._tokenizer.split_text_on_tokens(text=text, chunk_size=self._chunk_size, chunk_overlap=self._chunk_overlap)
         return chunks
```

### Comparing `llmflex-0.1.4/src/llmflex/Tools/base_tool.py` & `llmflex-0.1.5/src/llmflex/Tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/Tools/tool_selection.py` & `llmflex-0.1.5/src/llmflex/Tools/tool_selection.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/Tools/web_search_tool.py` & `llmflex-0.1.5/src/llmflex/Tools/web_search_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
         if llm is None:
             contents = list(map(lambda x: get_markdown(x, as_list=False), urls))
             docs = list(map(lambda x: Document(index=x[0], metadata=x[1]), list(zip(contents, results))))
             vectordb.add_documents(docs=docs, text_splitter=self.embeddings.text_splitter, split_text=True)
         else:
             contents = list(map(lambda x: get_markdown(x, as_list=True), urls))
-            contents = list(map(lambda x: create_content_chunks(x, llm), contents))
+            contents = list(map(lambda x: create_content_chunks(x, llm.get_num_tokens), contents))
             docs = list(zip(contents, results))
             docs = list(map(lambda x: list(map(lambda y: Document(index=y, metadata=x[1]), x[0])), docs))
             docs = sum(docs, [])
             vectordb.add_documents(docs=docs, split_text=False)
         return vectordb
     
     def create_relevant_content_chunks(self, query: str, vectordb: FaissVectorDatabase) -> Tuple[List[Dict[str, Any]], str]:
```

### Comparing `llmflex-0.1.4/src/llmflex/Tools/web_search_utils.py` & `llmflex-0.1.5/src/llmflex/Tools/web_search_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from bs4 import BeautifulSoup, NavigableString, Tag
 from langchain.llms.base import LLM
-from typing import Optional, List, Union
+from typing import Optional, List, Union, Callable
 
 def get_soup_from_url(url: str, timeout: int = 8) -> BeautifulSoup:
     """Get the soup object from a URL.
 
     Args:
         url (str): URL of the  website.
         timeout (int, optional): Timeout for the request in seconds. Defaults to 8.
@@ -369,32 +369,32 @@
         return None
     if as_list:
         return final
     else:
         final = list(map(lambda x: x + end, final))
         return sep.join(final)
     
-def create_content_chunks(contents: Optional[List[str]], llm: LLM, chunk_size: int = 400) -> List[str]:
+def create_content_chunks(contents: Optional[List[str]], token_count_fn: Callable[[str], int], chunk_size: int = 400) -> List[str]:
     """Create a list of strings of chunks limited by the count of tokens.
 
     Args:
         contents (Optional[List[str]]): List of contents to aggregate.
-        llm (LLM): LLM to count tokens.
+        token_count_fn (Callable[[str], int]): Function to count tokens.
         chunk_size (int, optional): Token limit of each chunk. Defaults to 400.
 
     Returns:
         List[str]: List of content chunks.
     """
     chunks = []
     current = []
     current_count = 0
     if contents is None:
         return chunks
     for c in contents:
-        count = llm.get_num_tokens(c)
+        count = token_count_fn(c)
         if current_count + count <= chunk_size:
             current.append(c)
             current_count += count
         elif count > chunk_size:
             chunks.append('\n\n'.join(current))
             chunks.append(c)
             current = []
```

### Comparing `llmflex-0.1.4/src/llmflex/VectorDBs/base_vectordb.py` & `llmflex-0.1.5/src/llmflex/VectorDBs/base_vectordb.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,41 +51,53 @@
     if '\t' in name:
         raise ValueError(f'Tab characters cannot be in the name.')
     return name
 
 class BaseVectorDatabase(ABC):
     """Base class for vector databases.
     """
-    def __init__(self, embeddings: Type[BaseEmbeddingsToolkit], name: Optional[str] = None, vectordb_dir: Optional[str] = None, **kwargs) -> None:
+    def __init__(self, embeddings: Type[BaseEmbeddingsToolkit], name: Optional[str] = None, vectordb_dir: Optional[str] = None, 
+                 text_splitter: Optional[Type[BaseTextSplitter]] = None, **kwargs) -> None:
         """Initialise a vector database.
 
         Args:
             embeddings (Type[BaseEmbeddingsToolkit]): Embeddings toolkit to use.
             name (Optional[str], optional): Name of the vector database. Will be used as the directory base name of the vector database in vectordb_dir. If None is given, the vector database will not be saved. Defaults to None.
             vectordb_dir (Optional[str], optional): Directory where the vector databases live. If None is given, the default_vectordb_dir will be used. Defaults to None.
+            text_splitter (Optional[Type[BaseTextSplitter]], optional): Default text splitter for the vecetor database. If None is given, the embeddings toolkit text splitter will be used. Defaults to None.
         """
         self._embeddings = embeddings
         self._name = name_checker(name) if name is not None else None
         vectordb_dir = default_vectordb_dir() if vectordb_dir is None else vectordb_dir
         self._db_dir = os.path.join(vectordb_dir, self.name) if self.name is not None else None
         if self.db_dir is not None:
             os.makedirs(self.db_dir, exist_ok=True)
         self._index = self._get_empty_index()
         self._data = dict()
+        self._text_splitter = self.embeddings.text_splitter if text_splitter is None else text_splitter
 
     @property
     def embeddings(self) -> BaseEmbeddingsToolkit:
         """Embeddings toolkit used in the vector database.
 
         Returns:
             BaseEmbeddingsToolkit: Embeddings toolkit used in the vector database.
         """
         return self._embeddings
     
     @property
+    def text_splitter(self) -> BaseTextSplitter:
+        """Default text splitter for the vector database.
+
+        Returns:
+            BaseTextSplitter: Default text splitter for the vector database.
+        """
+        return self._text_splitter
+    
+    @property
     def index(self) -> Any:
         """Index of the vector database.
 
         Returns:
             Any: Index of the vector database.
         """
         return self._index
@@ -218,21 +230,24 @@
 
         Returns:
             np.ndarray[np.float32]: Arrray of vectors.
         """
         pass
 
     @classmethod
-    def from_exist(cls, embeddings: Type[BaseEmbeddingsToolkit], name: str, vectordb_dir: Optional[str] = None, **kwargs) -> BaseVectorDatabase:
+    def from_exist(cls, embeddings: Type[BaseEmbeddingsToolkit], name: str, vectordb_dir: Optional[str] = None,
+                   text_splitter: Optional[Type[BaseTextSplitter]] = None, **kwargs) -> BaseVectorDatabase:
         """Load the vector database from an existing vector database.
 
         Args:
             embeddings (Type[BaseEmbeddingsToolkit]): Embeddings toolkit to use.
             name (str): Name of the existing database.
             vectordbs_dir (Optional[str], optional): Directory where the vector databases live. If None is given, the default_vectordb_dir will be used. Defaults to None.
+            text_splitter (Optional[Type[BaseTextSplitter]], optional): Text splitter to split the documents. If none given, the embeddings toolkit text splitter will be used. Defaults to None.
+
 
         Returns:
             BaseVectorDatabase: The initialised vector database.
         """
         vectordbs_dir = default_vectordb_dir() if vectordb_dir is None else vectordb_dir
         name = name_checker(name)
         existing_dbs = list_vectordbs(vectordb_dir=vectordbs_dir)
@@ -240,15 +255,15 @@
             raise ValueError(f'The vector database "{name}" does not exist.')
         
         from ..utils import read_json
         import pickle
         db_info_dir = os.path.join(vectordbs_dir, name, 'info.json')
         db_info = read_json(db_info_dir)
         db_embeddings_name = db_info.get('embeddings', None)
-        vdb = cls(embeddings, name, vectordbs_dir)
+        vdb = cls(embeddings, name, vectordbs_dir, text_splitter)
         data_dir =os.path.join(vdb.db_dir, 'data.pkl')
         if os.path.exists(data_dir):
             with open(data_dir, 'rb') as f:
                 vdb._data = pickle.load(f)
         else: # recovering from old format
             print('Trying to recover from old format...')
             old_data_dir = os.path.join(vdb.db_dir, 'index.pkl')
@@ -281,15 +296,15 @@
             vectordb_dir (Optional[str], optional): Directory where the vector databases live. If None is given, the default_vectordb_dir will be used. Defaults to None.
             split_text (bool, optional): Whether to split the docuements with the embeddings toolkit text splitter. Defaults to True.
             text_splitter (Optional[Type[BaseTextSplitter]], optional): Text splitter to split the documents. If none given, the embeddings toolkit text splitter will be used. Defaults to None.
 
         Returns:
             BaseVectorDatabase: The initialised vector database.
         """
-        vdb = cls(embeddings, name, vectordb_dir)
+        vdb = cls(embeddings, name, vectordb_dir, text_splitter)
         vdb.add_documents(docs=docs, split_text=split_text, text_splitter=text_splitter)
         vdb.save() # In case an empty list of docs is given.
         return vdb
     
     @classmethod
     def from_texts(cls, embeddings: Type[BaseEmbeddingsToolkit], texts: List[str], metadata: Optional[Union[Dict[str, Any], List[Dict[str, Any]]]] = None,
                       name: Optional[str] = None, vectordb_dir: Optional[str] = None,
@@ -304,15 +319,15 @@
             vectordb_dir (Optional[str], optional): Directory where the vector databases live. If None is given, the default_vectordb_dir will be used. Defaults to None.
             split_text (bool, optional): Whether to split the docuements with the embeddings toolkit text splitter. Defaults to True.
             text_splitter (Optional[Type[BaseTextSplitter]], optional): Text splitter to split the documents. If none given, the embeddings toolkit text splitter will be used. Defaults to None.
 
         Returns:
             BaseVectorDatabase: The initialised vector database.
         """
-        vdb = cls(embeddings, name, vectordb_dir)
+        vdb = cls(embeddings, name, vectordb_dir, text_splitter)
         vdb.add_texts(texts=texts, metadata=metadata, split_text=split_text, text_splitter=text_splitter)
         vdb.save() # In case an empty list of texts is given.
         return vdb
 
     def _save_data(self) -> None:
         """Save the documents in the vector database.
         """
@@ -342,15 +357,15 @@
 
         Args:
             docs (List[Document]): List of documents to split.
             split_text (bool, optional): Whether to split the docuements with the embeddings toolkit text splitter. Defaults to True.
             text_splitter (Optional[Type[BaseTextSplitter]], optional): Text splitter to split the documents. If none given, the embeddings toolkit text splitter will be used. Defaults to None.
         """
         if len(docs) != 0:
-            text_splitter = self.embeddings.text_splitter if text_splitter is None else text_splitter
+            text_splitter = self.text_splitter if text_splitter is None else text_splitter
             docs = text_splitter.split_documents(docs) if split_text else docs
             vectors = list(map(lambda x: x.index, docs))
             vectors = self.embeddings.batch_embed(vectors)
             vectors = np.array(vectors, dtype=np.float32)
             self._add(vectors=vectors, docs=docs)
             self.save()
 
@@ -498,9 +513,9 @@
         """Clear the entire vector database. Use it with caution.
         """
         import gc
         del self._index
         del self._data
         gc.collect()
         self._index = self._get_empty_index()
-        self._data
+        self._data = dict()
         self.save()
```

### Comparing `llmflex-0.1.4/src/llmflex/VectorDBs/faiss_vectordb.py` & `llmflex-0.1.5/src/llmflex/VectorDBs/faiss_vectordb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 from ..Embeddings.base_embeddings import BaseEmbeddingsToolkit
+from ..TextSplitters.base_text_splitter import BaseTextSplitter
 from ..Schemas.documents import Document
 from .base_vectordb import BaseVectorDatabase
 from typing import List, Any, Type, Optional, Tuple
 import os, numpy as np
 
 class FaissVectorDatabase(BaseVectorDatabase):
 
-    def __init__(self, embeddings: Type[BaseEmbeddingsToolkit], name: Optional[str] = None, vectordb_dir: Optional[str] = None, **kwargs) -> None:
+    def __init__(self, embeddings: Type[BaseEmbeddingsToolkit], name: Optional[str] = None, vectordb_dir: Optional[str] = None,
+                 text_splitter: Optional[Type[BaseTextSplitter]] = None, **kwargs) -> None:
         """Initialise a vector database.
 
         Args:
             embeddings (Type[BaseEmbeddingsToolkit]): Embeddings toolkit to use.
             name (Optional[str], optional): Name of the vector database. Will be used as the directory base name of the vector database in vectordb_dir. If None is given, the vector database will not be saved. Defaults to None.
             vectordb_dir (Optional[str], optional): Directory where the vector databases live. If None is given, the default_vectordb_dir will be used. Defaults to None.
+            text_splitter (Optional[Type[BaseTextSplitter]], optional): Default text splitter for the vecetor database. If None is given, the embeddings toolkit text splitter will be used. Defaults to None.
         """
         super().__init__(embeddings=embeddings, name=name, vectordb_dir=vectordb_dir)
 
     def _get_empty_index(self) -> Any:
         """Return an empty index.
 
         Returns:
```

### Comparing `llmflex-0.1.4/src/llmflex/cli.py` & `llmflex-0.1.5/src/llmflex/cli.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex/utils.py` & `llmflex-0.1.5/src/llmflex/utils.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.4/src/llmflex.egg-info/PKG-INFO` & `llmflex-0.1.5/src/llmflex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmflex
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python package for developing AI applications with local LLMs.
 Author-email: Nathan Tam <nathan1295@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nath1295/LLMFlex
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -22,15 +22,15 @@
 Requires-Dist: fake-useragent
 Requires-Dist: openai>=1.0.0
 Requires-Dist: tiktoken
 Requires-Dist: protobuf
 Requires-Dist: beautifulsoup4
 Requires-Dist: streamlit
 Requires-Dist: watchdog
-Requires-Dist: spacy
+Requires-Dist: spacy>=3.7.0
 Requires-Dist: flask
 Provides-Extra: cu121
 Requires-Dist: auto-gptq>=0.6.0; extra == "cu121"
 Requires-Dist: autoawq; extra == "cu121"
 Requires-Dist: exllamav2; extra == "cu121"
 Provides-Extra: cu118
 Requires-Dist: auto-gptq; extra == "cu118"
```

### Comparing `llmflex-0.1.4/src/llmflex.egg-info/SOURCES.txt` & `llmflex-0.1.5/src/llmflex.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -33,16 +33,20 @@
 src/llmflex/Models/Cores/llamacpp_core.py
 src/llmflex/Models/Cores/openai_core.py
 src/llmflex/Models/Cores/utils.py
 src/llmflex/Models/Factory/__init__.py
 src/llmflex/Models/Factory/llm_factory.py
 src/llmflex/Prompts/__init__.py
 src/llmflex/Prompts/prompt_template.py
+src/llmflex/Rankers/__init__.py
+src/llmflex/Rankers/base_ranker.py
+src/llmflex/Rankers/flashrank_ranker.py
 src/llmflex/Schemas/__init__.py
 src/llmflex/Schemas/documents.py
+src/llmflex/Schemas/tokenizer.py
 src/llmflex/TextSplitters/__init__.py
 src/llmflex/TextSplitters/base_text_splitter.py
 src/llmflex/TextSplitters/sentence_token_text_splitter.py
 src/llmflex/TextSplitters/token_text_splitter.py
 src/llmflex/Tools/__init__.py
 src/llmflex/Tools/base_tool.py
 src/llmflex/Tools/tool_selection.py
```


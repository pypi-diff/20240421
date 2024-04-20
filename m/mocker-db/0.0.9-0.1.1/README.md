# Comparing `tmp/mocker_db-0.0.9.tar.gz` & `tmp/mocker_db-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocker_db-0.0.9.tar", last modified: Sat Apr  6 02:37:32 2024, max compression
+gzip compressed data, was "mocker_db-0.1.1.tar", last modified: Sat Apr 20 22:09:26 2024, max compression
```

## Comparing `mocker_db-0.0.9.tar` & `mocker_db-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:37:32.953832 mocker_db-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-06 02:34:22.000000 mocker_db-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-04-06 02:37:32.953832 mocker_db-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-06 02:34:22.000000 mocker_db-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:37:32.953832 mocker_db-0.0.9/mocker_db/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-06 02:37:13.000000 mocker_db-0.0.9/mocker_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-06 02:37:13.000000 mocker_db-0.0.9/mocker_db/mocker_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-06 02:37:32.000000 mocker_db-0.0.9/mocker_db/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:37:32.953832 mocker_db-0.0.9/mocker_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-04-06 02:37:32.000000 mocker_db-0.0.9/mocker_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-06 02:37:32.000000 mocker_db-0.0.9/mocker_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:37:32.000000 mocker_db-0.0.9/mocker_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-06 02:37:32.000000 mocker_db-0.0.9/mocker_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 02:37:32.000000 mocker_db-0.0.9/mocker_db.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 02:37:32.953832 mocker_db-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:09:26.831677 mocker_db-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-20 22:04:39.000000 mocker_db-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-04-20 22:09:26.831677 mocker_db-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-20 22:04:39.000000 mocker_db-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:09:26.827677 mocker_db-0.1.1/mocker_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-20 22:09:02.000000 mocker_db-0.1.1/mocker_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31344 2024-04-20 22:09:02.000000 mocker_db-0.1.1/mocker_db/mocker_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-20 22:09:26.000000 mocker_db-0.1.1/mocker_db/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:09:26.831677 mocker_db-0.1.1/mocker_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-04-20 22:09:26.000000 mocker_db-0.1.1/mocker_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-20 22:09:26.000000 mocker_db-0.1.1/mocker_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 22:09:26.000000 mocker_db-0.1.1/mocker_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-20 22:09:26.000000 mocker_db-0.1.1/mocker_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 22:09:26.000000 mocker_db-0.1.1/mocker_db.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 22:09:26.831677 mocker_db-0.1.1/setup.cfg
```

### Comparing `mocker_db-0.0.9/LICENSE` & `mocker_db-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mocker_db-0.0.9/PKG-INFO` & `mocker_db-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocker_db
-Version: 0.0.9
+Version: 0.1.1
 Summary: A mock handler for simulating a vector database.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mocker_db-0.0.9/README.md` & `mocker_db-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,39 @@
 - contains __package_metadata__ (won't package without it)
 - falls under common license
 
 The ones that were not packages, could still be used as packages with [this instruction](https://github.com/Kiril-Mordan/reusables/blob/main/docs/module_from_raw_file.md).
 
 ## Content:
  
+[module](python_modules/shouterlog.py) | [usage](docs/shouterlog.md) | [![PyPiVersion](https://img.shields.io/pypi/v/shouterlog)](https://pypi.org/project/shouterlog/) - Shouter Log
+
+This class uses the logging module to create and manage a logger for displaying formatted messages.
+It provides a method to output various types of lines and headers, with customizable message and line lengths.
+The purpose is to be integrated into other classes that also use logger.
+
+[module](python_modules/gridlooper.py) | [usage](docs/gridlooper.md) | [drawio: -flow](docs/gridlooper-flow.png) | [![PyPiVersion](https://img.shields.io/pypi/v/gridlooper)](https://pypi.org/project/gridlooper/) - Grid Looper
+
+A tool to run experiments based on defined grid and function with single iteration.
+
+[module](python_modules/package_auto_assembler.py) | [usage](docs/package_auto_assembler.md) | [drawio: -flow](docs/package_auto_assembler-flow.png) | [drawio: -usage](docs/package_auto_assembler-usage.png) | [![PyPiVersion](https://img.shields.io/pypi/v/package-auto-assembler)](https://pypi.org/project/package-auto-assembler/) - Package Auto Assembler
+
+This tool is meant to streamline creation of single module packages.
+Its purpose is to automate as many aspects of python package creation as possible,
+to shorten a development cycle of reusable components, maintain certain standard of quality
+for reusable code. It provides tool to simplify the process of package creatrion
+to a point that it can be triggered automatically within ci/cd pipelines,
+with minimal preparations and requirements for new modules.
+
+[module](python_modules/retriever_tunner.py) | [usage](docs/retriever_tunner.md) - Retriever tunner
+
+A simple tool to compare and tune retriever performance, given a desired ranking to strive for.
+The goal is to provide a simple metric to measure how a given retriver is close to the 'ideal', generated for example
+with a use of more expensive, slower or simply no-existant method.
+
 [module](python_modules/google_drive_support.py) - Google Drive API Utilities Module
 
 This module provides a set of functions for interacting with the Google Drive API.
 It allows you to authenticate with the API, upload, download, and manage files and folders in Google Drive.
 
 [module](python_modules/comparisonframe.py) | [usage](docs/comparisonframe.md) | [plantuml](docs/comparisonframe_plantuml.png) - Comparison Frame
 
@@ -33,38 +58,13 @@
 
 [module](python_modules/mocker_db.py) | [usage](docs/mocker_db.md) | [drawio: -flow](docs/mocker_db-flow.png) | [release notes](release_notes/mocker_db.md) | [![PyPiVersion](https://img.shields.io/pypi/v/mocker-db)](https://pypi.org/project/mocker-db/) - MockerDB
 
 A python module that contains mock vector database like solution built around
 dictionary data type. It contains methods necessary to interact with this 'database',
 embed, search and persist.
 
-[module](python_modules/gridlooper.py) | [usage](docs/gridlooper.md) | [drawio: -flow](docs/gridlooper-flow.png) - Grid Looper
-
-A tool to run experiments based on defined grid and function with single iteration.
-
 [module](python_modules/search_based_extractor.py) | [usage](docs/search_based_extractor.md) - Search Based Extractor
 
 Utility to simplify webscraping by taking advantave of search and assumptions about html structure.
 Extractor allows to find parent html element that contains searched term, record path to it in a file
 and reuse that to scrape data with same html structure.
 
-[module](python_modules/retriever_tunner.py) | [usage](docs/retriever_tunner.md) - Retriever tunner
-
-A simple tool to compare and tune retriever performance, given a desired ranking to strive for.
-The goal is to provide a simple metric to measure how a given retriver is close to the 'ideal', generated for example
-with a use of more expensive, slower or simply no-existant method.
-
-[module](python_modules/package_auto_assembler.py) | [usage](docs/package_auto_assembler.md) | [drawio: -flow](docs/package_auto_assembler-flow.png) | [![PyPiVersion](https://img.shields.io/pypi/v/package-auto-assembler)](https://pypi.org/project/package-auto-assembler/) - Package Auto Assembler
-
-This tool is meant to streamline creation of single module packages.
-Its purpose is to automate as many aspects of python package creation as possible,
-to shorten a development cycle of reusable components, maintain certain standard of quality
-for reusable code. It provides tool to simplify the process of package creatrion
-to a point that it can be triggered automatically within ci/cd pipelines,
-with minimal preparations and requirements for new modules.
-
-[module](python_modules/shouterlog.py) | [usage](docs/shouterlog.md) | [![PyPiVersion](https://img.shields.io/pypi/v/shouterlog)](https://pypi.org/project/shouterlog/) - Shouter Log
-
-This class uses the logging module to create and manage a logger for displaying formatted messages.
-It provides a method to output various types of lines and headers, with customizable message and line lengths.
-The purpose is to be integrated into other classes that also use logger.
-
```

### Comparing `mocker_db-0.0.9/mocker_db/mocker_db.py` & `mocker_db-0.1.1/mocker_db/mocker_db.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,24 +17,33 @@
 import attr #>=22.2.0
 ## for making keys
 import hashlib
 ## for search
 import concurrent.futures
 import hnswlib #==0.8.0
 from sentence_transformers import SentenceTransformer #==2.2.2
+from gridlooper import GridLooper #==0.0.1
+## for connect to remote mocker
+import httpx
 
 
 # Metadata for package creation
 __package_metadata__ = {
     "author": "Kyrylo Mordan",
     "author_email": "parachute.repo@gmail.com",
     "description": "A mock handler for simulating a vector database.",
     # Add other metadata as needed
 }
 
+__design_choices__ = {
+    'similarity search' : ['similarity search is optional, mocker can be used as normal database',
+                           'to perform similarity searches mocker need to embed selected field during input',
+                           'on retrieval by not providing query similarity search is not performed, only filters are used']
+
+}
 
 class SentenceTransformerEmbedder:
 
     def __init__(self,tbatch_size = 32, processing_type = 'batch', max_workers = 2, *args, **kwargs):
         # Suppress SentenceTransformer logging
         logging.getLogger('sentence_transformers').setLevel(logging.ERROR)
         self.tbatch_size = tbatch_size
@@ -77,41 +86,14 @@
         embeddings = []
         for i in range(0, len(texts), batch_size):
             batch = texts[i:i + batch_size]
             batch_embeddings = self.model.encode(batch, show_progress_bar=False)
             embeddings.extend(batch_embeddings)
         return embeddings
 
-    # def embed_sentences_in_batches_parallel(self, texts, batch_size : int = None, max_workers : int =  None):
-
-    #     """
-    #     Embeds a list of texts in batches in parallel.
-    #     """
-
-    #     if batch_size is None:
-    #         batch_size = self.tbatch_size
-
-    #     if max_workers is None:
-    #         max_workers = self.max_workers
-
-
-    #     # Split texts into batches
-    #     batches = [texts[i:i + batch_size] for i in range(0, len(texts), batch_size)]
-
-    #     # Process batches in parallel
-    #     embeddings = []
-    #     with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
-    #         # Submit embedding tasks to the executor
-    #         future_to_batch = {executor.submit(self.embed_sentence_transformer, batch): batch for batch in batches}
-
-    #         for future in concurrent.futures.as_completed(future_to_batch):
-    #             embeddings.extend(future.result())
-
-    #     return embeddings
-
     def embed_sentences_in_batches_parallel(self, texts, batch_size: int = None, max_workers: int = None):
         """
         Embeds a list of texts in batches in parallel using processes.
         """
 
         if batch_size is None:
             batch_size = self.tbatch_size
@@ -129,15 +111,14 @@
                 embeddings.extend(future.result())
 
         return embeddings
 
 @attr.s
 class MockerSimilaritySearch:
 
-
     search_results_n = attr.ib(default=3, type=int)
     similarity_params = attr.ib(default={'space':'cosine'}, type=dict)
     similarity_search_type = attr.ib(default='linear')
 
     # output
     hnsw_index = attr.ib(init=False)
 
@@ -245,28 +226,166 @@
     def search(self,
                query_embedding,
                data_embeddings,
                k : int = None,
                similarity_search_type: str = None,
                similarity_params : dict = None):
 
-
         if k is None:
             k = self.search_results_n
         if similarity_search_type is None:
             similarity_search_type = self.similarity_search_type
         if similarity_params is None:
             similarity_params = self.similarity_params
 
         if similarity_search_type == 'linear':
             return self.linear_search(search_emb = query_embedding, doc_embs = data_embeddings, k=k, **similarity_params)
         if similarity_search_type == 'hnsw':
             return self.hnsw_search(search_emb = query_embedding, doc_embs = data_embeddings, k=k, **similarity_params)
 
 
+@attr.s
+class MockerConnector:
+
+    base_url = attr.ib(default = "http://localhost:8000")
+
+
+    def __attrs_post_init__(self):
+
+        self.client = httpx.Client(base_url=self.base_url)
+
+    def read_root(self):
+        response = self.client.get("/")
+        return response.text
+
+    def show_handlers(self):
+
+        """
+        Show active handlers
+        """
+
+        response = self.client.get("/active_handlers")
+        return response.json()
+
+    def remove_handlers(self,
+                        handler_names : list):
+
+        """
+        Remove active handlers
+        """
+
+        response = self.client.post("/remove_handlers", json={"handler_names": handler_names})
+        if response.status_code == 404:
+            raise Exception(response.json()['detail'])
+        return response.json()
+
+    def initialize_database(self,
+                            database_name : str = None,
+                            embedder_params : dict = None):
+
+        """
+        Initialize database handler.
+        """
+
+        params = {}
+
+        if database_name is not None:
+            params["database_name"] = database_name
+
+        if embedder_params is not None:
+            params["embedder_params"] = embedder_params
+
+        response = self.client.post("/initialize", json=params)
+        return response.json()
+
+    def insert_data(self,
+                    data : list,
+                    database_name : str = None,
+                    var_for_embedding_name : str = None,
+                    embed=False):
+
+        request_body = {"data": data,
+                        "var_for_embedding_name" : "text"}
+
+        if var_for_embedding_name is not None:
+            request_body["var_for_embedding_name"] = var_for_embedding_name
+        if database_name is not None:
+            request_body["database_name"] = database_name
+        if embed is not None:
+            request_body["embed"] = embed
+
+        response = self.client.post("/insert", json=request_body)
+        return response.json()
+
+    def search_data(self,
+                    database_name : str,
+                    query : str = None,
+                    filter_criteria : dict = None,
+                    return_keys_list : list = None,
+                    search_results_n : int = None,
+                    similarity_search_type : str = None,
+                    similarity_params : dict = None,
+                    perform_similarity_search : bool = None):
+
+        """
+        Search data in selected handler
+        """
+
+        request_body = {"database_name" : database_name}
+
+        if query is not None:
+            request_body["query"] = query
+        if filter_criteria is not None:
+            request_body["filter_criteria"] = filter_criteria
+        if return_keys_list is not None:
+            request_body["return_keys_list"] = return_keys_list
+        if search_results_n is not None:
+            request_body["search_results_n"] = search_results_n
+        if similarity_search_type is not None:
+            request_body["similarity_search_type"] = similarity_search_type
+        if similarity_params is not None:
+            request_body["similarity_params"] = similarity_params
+        if perform_similarity_search is not None:
+            request_body["perform_similarity_search"] = perform_similarity_search
+
+        response = self.client.post("/search", json=request_body)
+        return response.json()
+
+    def delete_data(self,
+                    database_name : str,
+                    filter_criteria : dict = None):
+
+        """
+        Delete data from selected handler
+        """
+
+        request_body = {"database_name": database_name}
+
+        if filter_criteria is not None:
+            request_body["filter_criteria"] = filter_criteria
+
+        response = self.client.post("/delete", json=request_body)
+        return response.json()
+
+    def embed_texts(self,
+                    texts : list,
+                    embedding_model : str = None):
+
+        """
+        Embed list of text
+        """
+
+        request_body = {"texts": texts}
+
+        if embedding_model is not None:
+            request_body["embedding_model"] = embedding_model
+
+        response = self.client.post("/embed", json=request_body)
+        return response.json()
+
 
 @attr.s
 class MockerDB:
     # pylint: disable=too-many-instance-attributes
 
     """
     The MockerDB class simulates a vector database environment, primarily for testing and development purposes.
@@ -298,15 +417,15 @@
                                        'processing_type' : 'batch',
                                        'tbatch_size' : 500})
     embedder = attr.ib(default=SentenceTransformerEmbedder)
 
 
     ## for similarity search
     similarity_search_h = attr.ib(default=MockerSimilaritySearch)
-    return_keys_list = attr.ib(default=[], type = list)
+    return_keys_list = attr.ib(default=None, type = list)
     search_results_n = attr.ib(default=3, type = int)
     similarity_search_type = attr.ib(default='linear', type = str)
     similarity_params = attr.ib(default={'space':'cosine'}, type = dict)
 
     ## inputs with defaults
     file_path = attr.ib(default="./mock_persist", type=str)
     embs_file_path = attr.ib(default="./mock_embs_persist", type=str)
@@ -347,16 +466,14 @@
         if self.logger is None:
             logging.basicConfig(level=self.loggerLvl, format=self.logger_format)
             logger = logging.getLogger(self.logger_name)
             logger.setLevel(self.loggerLvl)
 
             self.logger = logger
 
-
-
     def establish_connection(self, file_path : str = None, embs_file_path : str = None):
 
         """
         Simulates establishing a connection by loading data from a local file into the 'data' attribute.
         """
 
         if file_path is None:
@@ -412,31 +529,32 @@
                        text : str,
                        model : str) -> str:
 
         input_string = str(text) + str(model)
 
         return self.hash_string_sha256(input_string)
 
-    # def _add_embeddings(self,
-    #                     data_dict : dict,
-    #                     var_for_embedding_name : str) -> dict:
+    def _prep_filter_criterias(self, filter_criteria : dict) -> list:
+
+        """
+        Makes a list of filters based on provided filter.
+        """
 
-    #     """
-    #     Prepare a dictionary for storage in Mocker by adding embedding.
-    #     """
+        filter_criteria = {key: value if isinstance(value, list) else [value] \
+            for key, value in filter_criteria.items()}
 
-    #     try:
+        gl = GridLooper()
+        gl.prepare_search_grid(experiments_settings=filter_criteria)
 
-    #         embedding = self.embedder.embed(data_dict[var_for_embedding_name])
-    #         data_dict['embedding'] = embedding
+        filter_criterias = gl.experiment_configs
 
-    #     except Exception as e:
-    #         return 1
+        filter_criterias = [{k: v for k, v in filter_dict.items() if k != 'config_id'} \
+            for filter_dict in filter_criterias]
 
-    #     return data_dict
+        return filter_criterias
 
     def _insert_values_dict(self,
                             values_dicts : dict,
                             var_for_embedding_name : str,
                             model_name : str = None,
                             embed : bool = True) -> None:
 
@@ -500,15 +618,15 @@
         self.data.update(values_dicts)
         # apply persist strategy
         self.save_data()
 
 
     def insert_values(self,
                       values_dict_list : list,
-                      var_for_embedding_name : str,
+                      var_for_embedding_name : str = None,
                       embed : bool = True) -> None:
 
         """
         Simulates inserting key-value pairs into the mock Redis database.
         """
 
         values_dict_list = copy.deepcopy(values_dict_list)
@@ -564,30 +682,42 @@
 
     def filter_database(self, filter_criteria : dict = None):
 
         """
         Filters a dictionary based on multiple field criteria.
         """
 
+        if filter_criteria is None:
+            filter_criteria_list = []
+        else:
+            filter_criteria_list = self._prep_filter_criterias(filter_criteria = filter_criteria)
+
         self.filtered_data = {
             key: value for key, value in self.data.items()
-            if all(value.get(k) == v for k, v in filter_criteria.items())
-        }
+            if any(all(value.get(k) == v for k, v in filter_dict.items()) \
+                for filter_dict in filter_criteria_list)}
 
         if len(self.filtered_data) == 0:
             self.logger.warning("No data was found with applied filters!")
 
     def remove_from_database(self, filter_criteria : dict = None):
         """
         Removes key-value pairs from a dictionary based on filter criteria.
         """
 
+        if filter_criteria is None:
+            filter_criteria_list = []
+        else:
+            filter_criteria_list = self._prep_filter_criterias(filter_criteria = filter_criteria)
+
         self.data = {
-            key: value for key, value in self.data.items()
-            if not all(value.get(k) == v for k, v in filter_criteria.items())
+            key: value
+            for key, value in self.data.items()
+            if not any(all(value.get(k) == v for k, v in filter_criteria.items()) \
+                for filter_criteria in filter_criteria_list)
         }
 
         self.save_data()
 
     def search_database_keys(self,
         query: str,
         search_results_n: int = None,
@@ -595,15 +725,14 @@
         similarity_params: dict = None,
         perform_similarity_search: bool = None):
 
         """
         Searches the mock database using embeddings and saves a list of entries that match the query.
         """
 
-
         if search_results_n is None:
             search_results_n = self.search_results_n
 
         if similarity_search_type is None:
             similarity_search_type = self.similarity_search_type
 
         if similarity_params is None:
@@ -637,15 +766,16 @@
                     self.embs[model_name][query_hash] = query_embedding
 
 
             except Exception as e:
                 self.logger.error("Problem during embedding search query!", e)
 
             try:
-                data_embeddings = np.array([(self.filtered_data[d]['embedding']) for d in self.keys_list])
+                data_embeddings = np.array([(self.filtered_data[d]['embedding']) \
+                    for d in self.keys_list if 'embedding' in self.filtered_data[d].keys()])
             except Exception as e:
                 self.logger.error("Problem during extracting search pool embeddings!", e)
 
             try:
 
                 if len(data_embeddings) > 0:
                     labels, distances = self.similarity_search_h.search(query_embedding = query_embedding,
@@ -656,62 +786,67 @@
 
                     self.results_keys = [self.keys_list[i] for i in labels]
                     self.results_dictances = distances
                 else:
                     self.results_keys = []
                     self.results_dictances = None
 
-
             except Exception as e:
                 self.logger.error("Problem during extracting results from the mock database!", e)
 
-
         else:
 
             try:
                 self.results_keys = [result_key for result_key in self.filtered_data]
                 self.results_dictances = np.array([0 for _ in self.filtered_data])
             except Exception as e:
                 self.logger.error("Problem during extracting search pool embeddings!", e)
 
 
-
-
     def get_dict_results(self, return_keys_list : list = None) -> list:
 
         """
         Retrieves specified fields from the search results in the mock database.
         """
 
         if return_keys_list is None:
             return_keys_list = self.return_keys_list
 
         # This method mimics the behavior of the original 'get_dict_results' method
         results = []
-        for searched_doc in self.results_keys:
-            result = {key: self.data[searched_doc].get(key) for key in return_keys_list}
-            results.append(result)
+        if return_keys_list is not None:
+            for searched_doc in self.results_keys:
+                result = {key: self.data[searched_doc].get(key) for key in return_keys_list}
+                results.append(result)
+        else:
+            results = [self.data[searched_doc] for searched_doc in self.results_keys]
+
         return results
 
     def search_database(self,
-                        query: str,
+                        query: str = None,
                         search_results_n: int = None,
                         filter_criteria : dict = None,
                         similarity_search_type: str = None,
                         similarity_params: dict = None,
                         perform_similarity_search: bool = None,
                         return_keys_list : list = None) ->list:
 
         """
         Searches through keys and retrieves specified fields from the search results
         in the mock database for a given filter.
         """
 
+        if query is None:
+            perform_similarity_search = False
+
         if filter_criteria:
             self.filter_database(filter_criteria=filter_criteria)
+        else:
+            self.filtered_data = self.data
 
         self.search_database_keys(query = query,
                                     search_results_n = search_results_n,
                                     similarity_search_type = similarity_search_type,
                                     similarity_params = similarity_params,
                                     perform_similarity_search = perform_similarity_search)
```

### Comparing `mocker_db-0.0.9/mocker_db/setup.py` & `mocker_db-0.1.1/mocker_db/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,14 @@
       long_description = fh.read()
 else:
   long_description = ''
 
 setup(
     name="mocker_db",
     packages=["mocker_db"],
-    install_requires=['### mocker_db.py', 'numpy', 'attrs>=22.2.0', 'dill==0.3.7', 'sentence-transformers==2.2.2', 'hnswlib==0.8.0'],
+    install_requires=['### mocker_db.py', 'sentence-transformers==2.2.2', 'hnswlib==0.8.0', 'attrs>=22.2.0', 'dill==0.3.7', 'httpx', 'numpy', 'gridlooper==0.0.1'],
     classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Developers', 'Intended Audience :: Science/Research', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'License :: OSI Approved :: MIT License', 'Topic :: Scientific/Engineering'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A mock handler for simulating a vector database.", version="0.0.9"
+    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A mock handler for simulating a vector database.", version="0.1.1"
 )
```

### Comparing `mocker_db-0.0.9/mocker_db.egg-info/PKG-INFO` & `mocker_db-0.1.1/mocker_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocker-db
-Version: 0.0.9
+Version: 0.1.1
 Summary: A mock handler for simulating a vector database.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/pub_worm-0.2.5.tar.gz` & `tmp/pub_worm-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pub_worm-0.2.5.tar", last modified: Fri Mar 15 20:13:46 2024, max compression
+gzip compressed data, was "pub_worm-0.2.6.tar", last modified: Sat Apr 20 21:57:15 2024, max compression
```

## Comparing `pub_worm-0.2.5.tar` & `pub_worm-0.2.6.tar`

### file list

```diff
@@ -1,36 +1,43 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-03-15 20:13:46.635764 pub_worm-0.2.5/
--rw-r--r--   0 dan        (501) staff       (20)      375 2024-03-11 18:03:53.000000 pub_worm-0.2.5/MANIFEST.in
--rw-r--r--   0 dan        (501) staff       (20)      793 2024-03-15 20:13:46.635461 pub_worm-0.2.5/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      514 2024-03-07 18:02:08.000000 pub_worm-0.2.5/README.md
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-03-15 20:13:46.626441 pub_worm-0.2.5/pub_worm/
--rw-r--r--   0 dan        (501) staff       (20)        0 2024-03-07 18:38:19.000000 pub_worm-0.2.5/pub_worm/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-03-15 20:13:46.628141 pub_worm-0.2.5/pub_worm/impact_factor/
--rw-r--r--   0 dan        (501) staff       (20)      331 2024-03-06 20:31:06.000000 pub_worm-0.2.5/pub_worm/impact_factor/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-03-15 20:13:46.628522 pub_worm-0.2.5/pub_worm/impact_factor/data/
--rw-r--r--   0 dan        (501) staff       (20)  1421199 2024-03-06 20:09:42.000000 pub_worm-0.2.5/pub_worm/impact_factor/data/2022_JCR_IF.csv
--rw-r--r--   0 dan        (501) staff       (20)      334 2024-03-06 20:37:02.000000 pub_worm-0.2.5/pub_worm/impact_factor/impact_factor_lookup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-03-15 20:13:46.631583 pub_worm-0.2.5/pub_worm/ncbi/
--rw-r--r--   0 dan        (501) staff       (20)      245 2024-03-11 14:46:41.000000 pub_worm-0.2.5/pub_worm/ncbi/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-03-15 20:13:46.632525 pub_worm-0.2.5/pub_worm/ncbi/data/
--rw-r--r--   0 dan        (501) staff       (20)        4 2024-03-11 15:35:28.000000 pub_worm-0.2.5/pub_worm/ncbi/data/ncbi_efetch.json
--rw-r--r--   0 dan        (501) staff       (20)        4 2024-03-11 14:45:21.000000 pub_worm-0.2.5/pub_worm/ncbi/data/ncbi_esearch.json
--rw-r--r--   0 dan        (501) staff       (20)      239 2024-03-11 17:17:12.000000 pub_worm-0.2.5/pub_worm/ncbi/data/ncbi_esummary.json
--rw-r--r--   0 dan        (501) staff       (20)    10737 2024-03-15 13:04:06.000000 pub_worm-0.2.5/pub_worm/ncbi/entreze_api.py
--rw-r--r--   0 dan        (501) staff       (20)     5844 2024-03-15 20:01:44.000000 pub_worm-0.2.5/pub_worm/ncbi/entreze_post.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-03-15 20:13:46.633640 pub_worm-0.2.5/pub_worm/wormbase/
--rw-r--r--   0 dan        (501) staff       (20)      280 2024-03-06 12:16:53.000000 pub_worm-0.2.5/pub_worm/wormbase/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-03-15 20:13:46.634876 pub_worm-0.2.5/pub_worm/wormbase/data/
--rw-r--r--   0 dan        (501) staff       (20)     1408 2024-03-12 12:00:17.000000 pub_worm-0.2.5/pub_worm/wormbase/data/wormbase_field_gene.json
--rw-r--r--   0 dan        (501) staff       (20)      105 2024-03-12 12:11:16.000000 pub_worm-0.2.5/pub_worm/wormbase/data/wormbase_field_paper.json
--rw-r--r--   0 dan        (501) staff       (20)     1747 2024-03-12 12:10:09.000000 pub_worm-0.2.5/pub_worm/wormbase/data/wormbase_widget_gene.json
--rw-r--r--   0 dan        (501) staff       (20)     1026 2024-03-09 22:01:04.000000 pub_worm-0.2.5/pub_worm/wormbase/to_csv_helpers.py
--rw-r--r--   0 dan        (501) staff       (20)     8504 2024-03-12 23:44:05.000000 pub_worm-0.2.5/pub_worm/wormbase/wormbase_api.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-03-15 20:13:46.627543 pub_worm-0.2.5/pub_worm.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)      793 2024-03-15 20:13:46.000000 pub_worm-0.2.5/pub_worm.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      809 2024-03-15 20:13:46.000000 pub_worm-0.2.5/pub_worm.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2024-03-15 20:13:46.000000 pub_worm-0.2.5/pub_worm.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2024-03-07 18:02:51.000000 pub_worm-0.2.5/pub_worm.egg-info/not-zip-safe
--rw-r--r--   0 dan        (501) staff       (20)        7 2024-03-15 20:13:46.000000 pub_worm-0.2.5/pub_worm.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)        9 2024-03-15 20:13:46.000000 pub_worm-0.2.5/pub_worm.egg-info/top_level.txt
--rw-r--r--   0 dan        (501) staff       (20)       38 2024-03-15 20:13:46.635812 pub_worm-0.2.5/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      829 2024-03-15 20:12:11.000000 pub_worm-0.2.5/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-04-20 21:57:15.138632 pub_worm-0.2.6/
+-rw-r--r--   0 dan        (501) staff       (20)      375 2024-03-11 18:03:53.000000 pub_worm-0.2.6/MANIFEST.in
+-rw-r--r--   0 dan        (501) staff       (20)     2650 2024-04-20 21:57:15.138405 pub_worm-0.2.6/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     2370 2024-04-20 21:56:56.000000 pub_worm-0.2.6/README.md
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-04-20 21:57:15.134325 pub_worm-0.2.6/pub_worm/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-03-07 18:38:19.000000 pub_worm-0.2.6/pub_worm/__init__.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-04-20 21:57:15.135296 pub_worm-0.2.6/pub_worm/impact_factor/
+-rw-r--r--   0 dan        (501) staff       (20)      331 2024-03-06 20:31:06.000000 pub_worm-0.2.6/pub_worm/impact_factor/__init__.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-04-20 21:57:15.135432 pub_worm-0.2.6/pub_worm/impact_factor/data/
+-rw-r--r--   0 dan        (501) staff       (20)  1421199 2024-03-06 20:09:42.000000 pub_worm-0.2.6/pub_worm/impact_factor/data/2022_JCR_IF.csv
+-rw-r--r--   0 dan        (501) staff       (20)      334 2024-03-06 20:37:02.000000 pub_worm-0.2.6/pub_worm/impact_factor/impact_factor_lookup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-04-20 21:57:15.136493 pub_worm-0.2.6/pub_worm/ncbi/
+-rw-r--r--   0 dan        (501) staff       (20)        1 2024-04-19 18:38:53.000000 pub_worm-0.2.6/pub_worm/ncbi/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)    10855 2024-04-20 21:39:36.000000 pub_worm-0.2.6/pub_worm/ncbi/entreze_api.py
+-rw-r--r--   0 dan        (501) staff       (20)     7384 2024-04-16 17:51:52.000000 pub_worm-0.2.6/pub_worm/ncbi/entreze_post.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-04-20 21:57:15.136912 pub_worm-0.2.6/pub_worm/wormbase/
+-rw-r--r--   0 dan        (501) staff       (20)      280 2024-03-06 12:16:53.000000 pub_worm-0.2.6/pub_worm/wormbase/__init__.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-04-20 21:57:15.137302 pub_worm-0.2.6/pub_worm/wormbase/data/
+-rw-r--r--   0 dan        (501) staff       (20)     1408 2024-03-12 12:00:17.000000 pub_worm-0.2.6/pub_worm/wormbase/data/wormbase_field_gene.json
+-rw-r--r--   0 dan        (501) staff       (20)      105 2024-03-12 12:11:16.000000 pub_worm-0.2.6/pub_worm/wormbase/data/wormbase_field_paper.json
+-rw-r--r--   0 dan        (501) staff       (20)     1747 2024-03-12 12:10:09.000000 pub_worm-0.2.6/pub_worm/wormbase/data/wormbase_widget_gene.json
+-rw-r--r--   0 dan        (501) staff       (20)     1026 2024-03-09 22:01:04.000000 pub_worm-0.2.6/pub_worm/wormbase/to_csv_helpers.py
+-rw-r--r--   0 dan        (501) staff       (20)     8504 2024-03-12 23:44:05.000000 pub_worm-0.2.6/pub_worm/wormbase/wormbase_api.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-04-20 21:57:15.135036 pub_worm-0.2.6/pub_worm.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)     2650 2024-04-20 21:57:15.000000 pub_worm-0.2.6/pub_worm.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      911 2024-04-20 21:57:15.000000 pub_worm-0.2.6/pub_worm.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2024-04-20 21:57:15.000000 pub_worm-0.2.6/pub_worm.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2024-04-20 21:57:15.000000 pub_worm-0.2.6/pub_worm.egg-info/not-zip-safe
+-rw-r--r--   0 dan        (501) staff       (20)        7 2024-04-20 21:57:15.000000 pub_worm-0.2.6/pub_worm.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       15 2024-04-20 21:57:15.000000 pub_worm-0.2.6/pub_worm.egg-info/top_level.txt
+-rw-r--r--   0 dan        (501) staff       (20)       38 2024-04-20 21:57:15.138686 pub_worm-0.2.6/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)      829 2024-04-20 21:55:21.000000 pub_worm-0.2.6/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-04-20 21:57:15.137437 pub_worm-0.2.6/tests/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-04-19 14:36:21.000000 pub_worm-0.2.6/tests/__init__.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-04-20 21:57:15.137632 pub_worm-0.2.6/tests/impact_factor/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-04-20 11:06:18.000000 pub_worm-0.2.6/tests/impact_factor/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)      802 2024-04-20 10:48:16.000000 pub_worm-0.2.6/tests/impact_factor/test_get_impact_factor.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-04-20 21:57:15.137853 pub_worm-0.2.6/tests/ncbi/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-04-19 20:00:22.000000 pub_worm-0.2.6/tests/ncbi/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     4261 2024-04-20 21:26:00.000000 pub_worm-0.2.6/tests/ncbi/test_entreze_api.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-04-20 21:57:15.138156 pub_worm-0.2.6/tests/wormbase/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-04-19 16:05:48.000000 pub_worm-0.2.6/tests/wormbase/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     2837 2024-04-20 10:32:27.000000 pub_worm-0.2.6/tests/wormbase/test_wormbase_api.py
```

### Comparing `pub_worm-0.2.5/pub_worm/impact_factor/data/2022_JCR_IF.csv` & `pub_worm-0.2.6/pub_worm/impact_factor/data/2022_JCR_IF.csv`

 * *Files identical despite different names*

### Comparing `pub_worm-0.2.5/pub_worm/ncbi/entreze_api.py` & `pub_worm-0.2.6/pub_worm/ncbi/entreze_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,240 +1,277 @@
 '''
 NCBI REST API for https://eutils.ncbi.nlm.nih.gov/entrez/eutils
 '''
+import os
 import time
-import json
-import urllib.request
 import urllib.parse
 import logging
 import logging.config
-import re
-import os
-from . import load_ncbi_api_json
+import pandas as pd
+from bs4 import BeautifulSoup
+import requests
+from pub_worm.impact_factor.impact_factor_lookup import get_impact_factor
 
 try:
     logging.config.fileConfig('logging.config')
 except Exception:
     logging.basicConfig(filename='pub_worm_entrez.log', level=logging.DEBUG)
 
 # Create a logger object
 logger = logging.getLogger(__name__)
 
 class EntrezAPI:
 
-    def __init__(self,function):
+    def __init__(self):
         self.base_url_str = "https://eutils.ncbi.nlm.nih.gov/entrez/eutils"
         self.max_retries = 3
-        self.function = function
-        self.ncbi_api_json = load_ncbi_api_json(function)
+        self.timeout = 20
+        self.function = "esearch"
         self.api_key = os.environ.get('NCBI_API_KEY', None)
-        # if function not in self.ncbi_api_json:
-        #     logger.error(f"No NCBI connfig for {function=}")
-        #     self.results_doc_definition = {}
-        # else:
-        #     self.results_doc_definition = self.ncbi_api_json[data_request]
-        
 
-    def rest_api_call(self, params):
+
+    def _rest_api_call(self, params, data=None):
         url_str = f"{self.base_url_str}/{self.function}.fcgi"
-        params['retmode']='json'
+        params['retmode']='xml'
+
         if self.api_key:
             params['api_key'] = self.api_key
+
         query = '&'.join([f"{urllib.parse.quote(k, 'utf-8')}={urllib.parse.quote(v, 'utf-8')}" for k, v in params.items()])
         url_str = f"{url_str}?{query}"
         logger.debug(url_str)
 
+        #self.max_retries = 3
         retry = 0
         done = False
 
         api_result = None
-        api_error = None
+        api_error = "No Error Set"
 
         def handle_error(error_msg):
             print(error_msg)
             logger.debug(error_msg)
             nonlocal done, retry, api_error
             retry +=1
             if retry >= self.max_retries:
                 done = True
                 api_error = error_msg
 
         while not done:
             try:
-                url = urllib.request.urlopen(url_str)
-                if url.getcode() == 200:
+                if data:
+                    post_data = { "id": ",".join(data) } 
+                    response = requests.post(url_str, data=post_data, timeout=self.timeout)
+                else:
+                    response = requests.get(url_str, timeout=self.timeout)
+
+                response.raise_for_status()  # Check for HTTP errors
+                if response.status_code == 200:
                     done = True
-                    response_text = url.read().decode('utf-8')
-                    api_result = json.loads(response_text)
-                elif url.getcode() == 429:
-                    handle_error(f"Request limiter hit. waiting 2 seconds [Retry: {retry + 1}] code: {url.getcode()}")
+                    api_result = response.text
+                elif response.status_code == 429:
+                    handle_error(f"Request limiter hit. waiting 2 seconds [Retry: {retry + 1}] code: {response.status_code}")
                     time.sleep(2)
                 else:
-                    handle_error(f"Failed to retrieve data. | Retry- {retry +1} | Response code- {url.getcode()}")
+                    handle_error(f"Failed to retrieve data. | Retry- {retry +1} | Response code- {response.status_code}")
+
             except Exception as ex:
                 aviod_logging_interpolation=f"Error while calling url_str {str(ex)}"
                 logger.error(aviod_logging_interpolation)
-                error_msg=f"Check if you have a connection!! | Retry- {retry+1} | Response msg- {str(ex)}"
-                if isinstance(ex, urllib.error.HTTPError):
-                    if ex.code == 500:
+                error_msg=f"Unexpected Error | Retry- {retry+1} | Response msg- {str(ex)}"
+                if isinstance(ex, requests.exceptions.HTTPError):
                         error_msg = f"Check the format of the http request [Retry: {retry + 1}] code: {str(ex)}"
-                    elif ex.code == 429:
-                        error_msg = f"Request limiter hit. waiting 2 seconds [Retry: {retry + 1}] code: {str(ex)}"
-                        time.sleep(2)
+                elif isinstance(ex, requests.exceptions.ConnectionError):
+                        error_msg = f"Connection Error [Retry: {retry + 1}] code: {str(ex)}"
+                elif isinstance(ex, requests.exceptions.Timeout):
+                        error_msg = f"Timeout Error [Retry: {retry + 1}] code: {str(ex)}"
                 handle_error(error_msg)
 
         if api_result is None:
-            api_result = {"rest_api_error": api_error}
-        
+            api_result = f"<response><rest_api_error>{api_error}</rest_api_error></response>"
+
         if logger.isEnabledFor(logging.DEBUG):
-            pretty_data = json.dumps(api_result, indent=4)
-            with open('http_response.json', 'w') as file:
+            soup = BeautifulSoup(api_result, "xml")
+            # Pretty-print the XML content
+            pretty_data = soup.prettify()
+            with open('http_response.xml', 'w') as file:
                 file.write(pretty_data)
-            #logger.debug(pretty_data)
-                
+            logger.debug(pretty_data)
+
         return api_result
 
 
-    @staticmethod
-    def get_ncbi_data(method_params, data_request):
-            def replace_uid(uid, json_data):
-                json_str = json.dumps(json_data)
-                replaced_json_str = re.sub(r'\$UID', str(uid), json_str)
-                replaced_json = json.loads(replaced_json_str)
-                return replaced_json
-
-            entrez_search_api = EntrezAPI('esearch')
-            search_params = {}
-            search_params['usehistory'] = 'y' 
-            search_params['retmax']     = method_params.get('retmax', '200')
-            search_params['restart']    = method_params.get('restart', '0')
-            search_params['db']         = method_params.get('pubmed', 'pubmed')
-            if "term" in method_params:
-                search_params['term']   = method_params.get('term')
-            else:
-                logger.error("'term' is a required parameter but was not passed in!")
-                return {}
+    def _get_tag(self, soup, path_names):
+        root = soup
+        for path_name in path_names:
+            logger.debug(f"get_tag {type(root)} {root} {path_name}")
+            root = root.find(path_name, default='')
+        return root
+
+    def _get_tag_text(self, doc, tag_name, attribute=None):
+        if attribute:
+            tag = doc.find(tag_name, attribute)
+        else:
+            tag = doc.find(tag_name)
+        return tag.text if tag else ""
 
-            search_ret_data = entrez_search_api.rest_api_call(search_params)
 
-            summary_params = {}
-            summary_params['retmax']     = search_params.get('retmax', '200')
-            summary_params['restart']    = search_params.get('restart', '0')
-            summary_params['db']         = search_params.get('pubmed', 'pubmed')
-
-            if 'esearchresult' in search_ret_data:
-                esearchresult = search_ret_data['esearchresult']
-                summary_params['query_key'] = esearchresult.get('querykey')
-                summary_params['WebEnv']    = esearchresult.get('webenv')
-            else:
-                logger.error("'esearchresult' is expected in the return but was not found!")
-                return {}
+    def entreze_esearch(self, params):
+        self.function="esearch"
+        esearch_params = {}
+        esearch_params['db']         = params.get('db', 'pubmed')
+        esearch_params['retmax']     = params.get('retmax', '200')
+        esearch_params['usehistory'] = "y"
+        esearch_params['term']       = params.get('term', None)
+        if esearch_params['term'] is None:
+            logger.debug("Param 'searchTerm' is required but not passed.")
+
+        api_result = self._rest_api_call(esearch_params)
+        ret_params = self._history_key_to_json(api_result)
+        return ret_params
+
+    def entreze_epost(self, data, params={}):
+        self.function="epost"
+        epost_params = {}
+        epost_params['db']     = params.get('db', 'pubmed')
+        if data is None:
+            logger.debug("Param 'data' is required but not passed.")
+
+        api_result = self._rest_api_call(epost_params, data)
+        ret_params = self._history_key_to_json(api_result)
+        ret_params['count'] = len(data)
+        return ret_params
+
+    def _history_key_to_json(self, api_result):
+        ret_params = {}
+        ret_params['function'] = self.function
+        # Parse the XML response using BeautifulSoup
+        soup = BeautifulSoup(api_result, "xml")
+        # Extract WebEnv and QueryKey
+        count     = self._get_tag_text(soup, "Count")
+        ret_max   = self._get_tag_text(soup, "RetMax")
+        ret_start = self._get_tag_text(soup, "RetStart")
+        web_env   = self._get_tag_text(soup, "WebEnv")
+        query_key = self._get_tag_text(soup, "QueryKey")
+        api_error = self._get_tag_text(soup, "rest_api_error")
+        if count:
+            ret_params['count'] = count
+        if ret_max:
+            ret_params['ret_max'] = ret_max
+        if ret_start:
+            ret_params['ret_start'] = ret_start
+
+        ret_params['query_key'] = query_key
+        ret_params['WebEnv']    = web_env
+        if api_error:
+            logger.error("Error in history_key_to_json")
+            ret_params = {}
+            ret_params["Error"] = api_error
+        return ret_params
+
+    def entreze_pmid_summaries(self, params):
+        paper_summarys = []
+        soup = self._entreze_get_data(params, "esummary")
+        if soup is None:
+            return paper_summarys
+        
+        # Extract information for each UID
+        for doc in soup.find_all("DocSum"):
+            uid         = self._get_tag_text(doc, "Id")
+            issn        = self._get_tag_text(doc, "Item", {"Name": "ISSN"})
+            essn        = self._get_tag_text(doc, "Item", {"Name": "ESSN"})
+            last_author = self._get_tag_text(doc, "Item", {"Name": "LastAuthor"})
+            pmc_id      = self._get_tag_text(doc, "Item", {"Name": "pmc"})
+            title       = self._get_tag_text(doc, "Item", {"Name": "Title"})
+            source      = self._get_tag_text(doc, "Item", {"Name": "Source"})
+            
+            paper_summary = {
+                "uid"         : uid,
+                "issn"        : issn,
+                "essn"        : essn,
+                "last_author" : last_author,
+                "pmc_id"      : pmc_id,
+                "title"       : title,
+                "source"      : source
+            }
+            paper_summarys.append(paper_summary)
+
+        return paper_summarys
+
+    def entreze_efetch(self, params):
+        logger.debug("Entering entreze_efetch!!")
+        efetch_results = []
+
+        rec_count = int(params.get('count', 0))
+        restart = 0
+        while rec_count > 0 :
+            params['restart'] = restart
+            soup = self._entreze_get_data(params, "efetch")
+            if soup is None:
+                return efetch_results
+            
+            root_element = soup.find()
+            if root_element.name == 'PubmedArticleSet':
+                logger.debug("root_element == PubmedArticleSet!!")
+                pubmed_articles = self._get_pubmed_articles(soup)
+                # Get PubmedArticleSet
+                efetch_results += pubmed_articles
 
-            entrez_summary_api = EntrezAPI('esummary')
-            summary_ret_data = entrez_summary_api.rest_api_call(summary_params)
-            ret_dict = {}
-
-            ncbi_api_json = load_ncbi_api_json('esummary')
-            results_doc_definition = ncbi_api_json[data_request]
-            uid = search_params['term'][:-5]
-            results_doc_definition = replace_uid(uid, results_doc_definition)
-            ret_dict = EntrezAPI.parse_data(summary_ret_data, results_doc_definition, ret_dict)
-            return ret_dict
-
-
-    @staticmethod
-    def get_json_element(json_data, path):
-        result = json_data
-        try:
-            for key in path:
-                result = result[key]
-        except Exception: #KeyError TypeError
-            result = None
-        return result
-
-    @staticmethod
-    def extract_empty_dict(json_obj):
-        if isinstance(json_obj, dict):
-            return {k: EntrezAPI.extract_empty_dict(v) for k, v in json_obj.items() if v and EntrezAPI.extract_empty_dict(v)}
-        elif isinstance(json_obj, list):
-            return [EntrezAPI.extract_empty_dict(v) for v in json_obj if v and EntrezAPI.extract_empty_dict(v)]
-        else:
-            return json_obj
+            restart   +=200 # Increment record position by 200
+            rec_count -=200 # Pull the next 200 records or however many are remaining
+        
+
+        return efetch_results
     
-    @staticmethod
-    def extract_single_element_lists(json_obj):
-        if isinstance(json_obj, dict):
-            for key, value in json_obj.items():
-                json_obj[key] = EntrezAPI.extract_single_element_lists(value)
-        elif isinstance(json_obj, list):
-            # If list length is 1 remove list
-            if len(json_obj) == 1:
-                return EntrezAPI.extract_single_element_lists(json_obj[0])
-            else:
-                return [EntrezAPI.extract_single_element_lists(item) for item in json_obj]
-        return json_obj
+    def _get_pubmed_articles(self, soup):
+        articles = []
 
-    @staticmethod
-    def extract_skip_elements(json_obj):
-        if isinstance(json_obj, dict):
-            for key, value in json_obj.items():
-                if key == "SKIP":
-                    json_obj = EntrezAPI.extract_skip_elements(value)
-                else:
-                    json_obj[key] = EntrezAPI.extract_skip_elements(value)
-        elif isinstance(json_obj, list):
-            return [EntrezAPI.extract_skip_elements(item) for item in json_obj]
-        return json_obj
-
-    @staticmethod
-    def parse_data(data_to_process, doc_definition, results_dict):    
-        # data_request_item_nm="description" data_request_item=["fields", "concise_description","data","text"]
-        # data_request_item_nm="author"      data_request_item={ "ROOT": ["author"], "CONCAT": ["label"] }
-        for data_request_item_nm, data_request_item in doc_definition.items():
-            logger.debug(f"{data_request_item_nm=}{data_request_item=}")
-            if isinstance(data_request_item, list):
-                data_request_item_path = data_request_item
-                widget_item = EntrezAPI.get_json_element(data_to_process, data_request_item_path)
-                if widget_item is not None:
-                    results_dict[data_request_item_nm] = widget_item
-            elif isinstance(data_request_item, dict):
-                #logger.debug(f"BEFORE {data_request_item=}, {data_request_item['ROOT']=}")
-                #pretty_data = json.dumps(data_to_process, indent=4)
-                #logger.debug(f"BEFORE {pretty_data}")
-                sub_data_to_process = EntrezAPI.get_json_element(data_to_process, data_request_item["ROOT"])
-                if sub_data_to_process is None:
-                    logger.debug(f"AFTER WTF")
-
-                if sub_data_to_process is not None:
-                    #pretty_data = json.dumps(sub_data_to_process, indent=4)
-                    #logger.debug(f"AFTER {pretty_data}")
-                    if "CONCAT" in data_request_item:
-                        sub_results_str = ""
-                        for sub_data_item in sub_data_to_process:
-                            sub_results = EntrezAPI.parse_data(sub_data_item, data_request_item, {})
-                            if "CONCAT" in sub_results:
-                                sub_results_str +=str(f"{sub_results['CONCAT']}|")
-                        results_dict[data_request_item_nm] = sub_results_str[:-1]
-                        logger.debug(f"Found CONCAT")
-                    else:
-                        logger.debug(f"AFTER NO CONCAT")
-                        if isinstance(sub_data_to_process, dict):
-                            logger.debug(f"DICT {sub_data_to_process=}")
-                            logger.debug(f"DICT {data_request_item=}")
-                            results_dict[data_request_item_nm] = EntrezAPI.parse_data(sub_data_to_process, data_request_item, {})
-                        else: #It is a list
-                            sub_results_list = []
-                            for sub_data_item in sub_data_to_process:
-                                list_item_to_append = EntrezAPI.parse_data(sub_data_item, data_request_item, {})
-                                logger.debug(f"LIST ITEM {list_item_to_append=}")
-                                sub_results_list.append(list_item_to_append)
-                            results_dict[data_request_item_nm] = sub_results_list
+        pubmed_articles = soup.find_all('PubmedArticle')
+        # Iterate over the <PubmedArticle> elements
+        for pubmed_article in pubmed_articles:
+            article = {}
+            medline_citation = self._get_tag(pubmed_article, ['MedlineCitation'])
+            article_details  = self._get_tag(medline_citation, ['Article'])
+            abstract_details = self._get_tag(article_details, ['Abstract'])
+            journal          = self._get_tag(article_details, ['Journal'])
+            pub_date         = self._get_tag(journal, ['JournalIssue', 'PubDate'])
+
+            article['pmid']     = self._get_tag_text(medline_citation, "PMID")
+            article['issn']     = self._get_tag_text(journal, "ISSN", {"IssnType": "Print"})
+            article['eissn']    = self._get_tag_text(journal, "ISSN", {"IssnType": "Electronic"})
+            article['pub_year'] = self._get_tag_text(pub_date, "Year")
+            article['pub_abbr'] = self._get_tag_text(journal, "ISOAbbreviation")
+            article['title']    = self._get_tag_text(article_details, "ArticleTitle")
+            article['abstract'] = self._get_tag_text(abstract_details, "AbstractText")
+            if article['issn']:
+                article['impact_factor'] = get_impact_factor(article['issn'])
+            if 'impact_factor' not in article:
+                article['impact_factor'] = get_impact_factor(article['eissn'])
+
+            articles.append(article)
+
+        return articles
 
+    def _entreze_get_data(self, params, function):
+        self.function = function
+        efetch_params = {}
+        efetch_params['db']  = params.get('db', 'pubmed')
+
+        required_params = ['query_key', 'WebEnv']
+        for param_name in required_params:
+            if param_name in params:
+                efetch_params[param_name] = params[param_name]
             else:
-                logger.debug("!!"*40)
+                logger.debug(f"Param '{param_name}' is required but not passed")
+                return None
 
-        # Post processing
-        results_dict = EntrezAPI.extract_empty_dict(results_dict)
-        results_dict = EntrezAPI.extract_skip_elements(results_dict)
-        results_dict = EntrezAPI.extract_single_element_lists(results_dict)
-        return results_dict
-            
+        api_result = self._rest_api_call(efetch_params)
+        # Parse the XML response using BeautifulSoup
+        soup = BeautifulSoup(api_result, "xml")
+
+        api_error = self._get_tag_text(soup,"rest_api_error")
+        if api_error:
+            logger.error("Error in _entreze_get_data")
+            # Maybe throw and exception here
+            return None
+        
+        return soup
```

### Comparing `pub_worm-0.2.5/pub_worm/wormbase/data/wormbase_field_gene.json` & `pub_worm-0.2.6/pub_worm/wormbase/data/wormbase_field_gene.json`

 * *Files identical despite different names*

### Comparing `pub_worm-0.2.5/pub_worm/wormbase/data/wormbase_widget_gene.json` & `pub_worm-0.2.6/pub_worm/wormbase/data/wormbase_widget_gene.json`

 * *Files identical despite different names*

### Comparing `pub_worm-0.2.5/pub_worm/wormbase/to_csv_helpers.py` & `pub_worm-0.2.6/pub_worm/wormbase/to_csv_helpers.py`

 * *Files identical despite different names*

### Comparing `pub_worm-0.2.5/pub_worm/wormbase/wormbase_api.py` & `pub_worm-0.2.6/pub_worm/wormbase/wormbase_api.py`

 * *Files identical despite different names*

### Comparing `pub_worm-0.2.5/setup.py` & `pub_worm-0.2.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # twine upload --repository pypi dist/*
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='pub_worm',
-      version='0.2.5',
+      version='0.2.6',
       description='Wormbase/PudMed API Access',
       long_description_content_type="text/markdown",
       long_description=long_description,
 
       url='https://github.com/DanHUMassMed/pub_worm.git',
       author='Dan Higgins',
       author_email='daniel.higgins@yahoo.com',
```


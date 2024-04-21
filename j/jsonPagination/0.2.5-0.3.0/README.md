# Comparing `tmp/jsonpagination-0.2.5.tar.gz` & `tmp/jsonpagination-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonpagination-0.2.5.tar", last modified: Tue Apr 16 14:54:02 2024, max compression
+gzip compressed data, was "jsonpagination-0.3.0.tar", last modified: Sun Apr 21 02:57:17 2024, max compression
```

## Comparing `jsonpagination-0.2.5.tar` & `jsonpagination-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:54:02.009350 jsonpagination-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35239 2024-04-16 14:53:58.000000 jsonpagination-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8419 2024-04-16 14:54:02.009350 jsonpagination-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-04-16 14:53:58.000000 jsonpagination-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:54:02.005350 jsonpagination-0.2.5/jsonPagination/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-16 14:53:58.000000 jsonpagination-0.2.5/jsonPagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-16 14:53:58.000000 jsonpagination-0.2.5/jsonPagination/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17030 2024-04-16 14:53:58.000000 jsonpagination-0.2.5/jsonPagination/paginator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:54:02.009350 jsonpagination-0.2.5/jsonPagination.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8419 2024-04-16 14:54:01.000000 jsonpagination-0.2.5/jsonPagination.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-16 14:54:02.000000 jsonpagination-0.2.5/jsonPagination.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:54:01.000000 jsonpagination-0.2.5/jsonPagination.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 14:54:01.000000 jsonpagination-0.2.5/jsonPagination.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 14:54:01.000000 jsonpagination-0.2.5/jsonPagination.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:54:02.009350 jsonpagination-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-16 14:53:58.000000 jsonpagination-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:57:17.733424 jsonpagination-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35239 2024-04-21 02:57:10.000000 jsonpagination-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-04-21 02:57:17.733424 jsonpagination-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-21 02:57:10.000000 jsonpagination-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:57:17.733424 jsonpagination-0.3.0/jsonPagination/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-21 02:57:10.000000 jsonpagination-0.3.0/jsonPagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-21 02:57:10.000000 jsonpagination-0.3.0/jsonPagination/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17155 2024-04-21 02:57:10.000000 jsonpagination-0.3.0/jsonPagination/paginator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:57:17.733424 jsonpagination-0.3.0/jsonPagination.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-04-21 02:57:17.000000 jsonpagination-0.3.0/jsonPagination.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-21 02:57:17.000000 jsonpagination-0.3.0/jsonPagination.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 02:57:17.000000 jsonpagination-0.3.0/jsonPagination.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 02:57:17.000000 jsonpagination-0.3.0/jsonPagination.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 02:57:17.000000 jsonpagination-0.3.0/jsonPagination.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 02:57:17.733424 jsonpagination-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-21 02:57:10.000000 jsonpagination-0.3.0/setup.py
```

### Comparing `jsonpagination-0.2.5/LICENSE` & `jsonpagination-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonpagination-0.2.5/PKG-INFO` & `jsonpagination-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonPagination
-Version: 0.2.5
+Version: 0.3.0
 Summary: A versatile JSON data downloader with pagination and multithreading support.
 Home-page: https://github.com/pl0psec/jsonPagination
 Author: pl0psec
 Author-email: contact@pl0psec.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: requests
 Requires-Dist: tqdm
 
 # jsonPagination 
 
 [![python](https://img.shields.io/badge/Python-3.9-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![License: GPLv3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-![pylint](https://img.shields.io/badge/PyLint-9.71-green?logo=python&logoColor=white)
+![pylint](https://img.shields.io/badge/PyLint-9.73-green?logo=python&logoColor=white)
 [![GitHub version](https://badge.fury.io/gh/pl0psec%2FjsonPagination.svg)](https://badge.fury.io/gh/pl0psec%2FjsonPagination)
 [![PyPI version](https://badge.fury.io/py/jsonPagination.svg)](https://badge.fury.io/py/jsonPagination)
 
 `jsonPagination` is a Python library designed to simplify the process of fetching and paginating JSON data from APIs. It supports authentication, multithreading for efficient data retrieval, and handling of pagination logic, making it ideal for working with large datasets or APIs with rate limits.
 
 ## Features
 
@@ -39,34 +39,54 @@
 - **Custom Headers Support**: Enables the injection of custom HTTP headers into each request, providing a way to include additional metadata like API keys, session tokens, or other authentication information required by the API.
 
 - **Error Handling and Retry Logic**: Implements robust error detection and retry mechanisms to handle transient network issues or API errors. This ensures that temporary setbacks do not interrupt the data retrieval process, improving the reliability of data fetching operations.
 
 
 ## Installation
 
-To install `jsonPagination`, simply use pip:
+To install `jsonPagination`, you have two options:
 
+1. Install directly using pip:
+
+    ```
     pip install jsonPagination
+    ```
+
+2. If you have a `requirements.txt` file that includes `jsonPagination`, install all the required packages using:
+
+    ```
+    pip install -r requirements.txt
+    ```
+
+Make sure `jsonPagination` is listed in your `requirements.txt` file with the desired version, like so:
+
+```sh
+jsonPagination==x.y.z
+```
+
+Replace `x.y.z` with the specific version number you want to install.
 
 ## Usage
 
 ### Basic Pagination
 Here's how to use `jsonPagination` for basic pagination, demonstrating both page-based and index-based pagination:
 
 ```python
 from jsonPagination.paginator import Paginator
 
-# Page-based pagination example
+# Instantiate the Paginator with a base URL
 paginator = Paginator(
+    base_url='https://api.example.com',
     current_page_field='page',  # Field name used by the API for page number
     items_field='items_per_page',  # Field name used by the API for the number of items per page
     max_threads=2
 )
 
-results = paginator.fetch_all_pages('https://api.example.com/data')
+# Fetch data using a relative path
+results = paginator.fetch_all_pages('/data')
 
 print("Downloaded data:")
 print(results)
 ```
 
 ### Pagination with Authentication
 #### Basic Authentication
@@ -76,81 +96,63 @@
 from jsonPagination.paginator import Paginator
 
 headers = {
     'Authorization': 'Basic <base64_encoded_credentials>'
 }
 
 paginator = Paginator(
+    base_url='https://api.example.com',
     headers=headers,
     max_threads=2
 )
 
-results = paginator.fetch_all_pages('https://api.example.com/data')
+results = paginator.fetch_all_pages('/data')
 
 print("Downloaded data with basic authentication:")
 print(results)
 ```
 
 #### Token-based Authentication
-For APIs requiring a token, provide the login URL and authentication data:
+For APIs requiring a token, configure the `login_url` with the base URL during instantiation:
 
 ```python
 from jsonPagination.paginator import Paginator
+from urllib.parse import urljoin
 
 paginator = Paginator(
-    login_url='https://api.example.com/api/login',
+    base_url='https://api.example.com',
+    login_url=urljoin(base_url, '/api/login'),
     auth_data={'username': 'your_username', 'password': 'your_password'},
     max_threads=2
 )
 
-results = paginator.fetch_all_pages('https://api.example.com/api/data')
+results = paginator.fetch_all_pages('/api/data')
 
 print("Downloaded data with token-based authentication:")
 print(results)
 ```
 
 ### Rate Limit Example
 Demonstrating how to handle rate limits:
 
 ```python
 from jsonPagination.paginator import Paginator
 
 paginator = Paginator(
+    base_url='https://api.example.com',
     max_threads=2,
     ratelimit=(5, 60)  # 5 requests per 60 seconds
 )
 
-results = paginator.fetch_all_pages('https://api.example.com/data')
+results = paginator.fetch_all_pages('/data')
 
 print("Downloaded data with rate limiting:")
 print(results)
 ```
 
-## Configuration
-
-When instantiating the `Paginator` class, you can configure the following parameters to tailor its behavior:
-
-- `url`: The API endpoint URL from which data will be fetched.
-- `login_url` (optional): The URL to authenticate and retrieve a bearer token, used if the API requires token-based authentication.
-- `auth_data` (optional): A dictionary containing authentication data (such as `username` and `password`) required by the login endpoint for obtaining a token.
-- `current_page_field` (optional): The JSON field name used by the API to denote the current page number, applicable for page-number-based pagination.
-- `current_index_field` (optional): The JSON field name used by the API to denote the starting index for data fetching, applicable for index-based pagination.
-- `items_field` (optional): The JSON field name for the number of items to fetch per request, which corresponds to `per_page` in many APIs. This is used to control pagination size.
-- `total_count_field`: The JSON field name that contains the total number of items available, used to calculate the total number of pages or batches.
-- `items_per_page` (optional): Specifies the number of items to request per page or batch. If not set, the Paginator will try to use a sensible default based on the first API response or a predefined value.
-- `max_threads`: The maximum number of threads to use for parallel data fetching, enhancing speed for large datasets.
-- `download_one_page_only` (optional): A boolean indicating whether to fetch only the first page/batch of data, useful for testing or when only a sample of data is needed.
-- `verify_ssl` (optional): Determines whether SSL certificates should be verified in HTTP requests, enhancing security.
-- `data_field`: The specific JSON field name from which to extract the main data in the API response, necessary for parsing the fetched JSON data correctly.
-- `log_level` (optional): Sets the verbosity of logging, with possible values like `DEBUG`, `INFO`, `WARNING`, `ERROR`, and `CRITICAL`, to assist in debugging and monitoring.
-- `headers` (optional): A dictionary of custom HTTP headers to include in every request made by the Paginator, enabling additional customization like API keys or session tokens.
-- `ratelimit` (optional): A tuple specifying the rate limit as `(calls, period)` to prevent exceeding the API's rate limiting policies, ensuring compliant and responsible usage.
-
-These configuration options provide extensive control over how the `Paginator` interacts with the API, including authentication mechanisms, request formatting, error handling, and data retrieval efficiency. By adjusting these parameters, you can optimize the behavior of the Paginator to match the specific requirements and constraints of the API you are working with.
-
 ## Contributing
 
 We welcome contributions to `jsonPagination`! Please open an issue or submit a pull request for any features, bug fixes, or documentation improvements.
 
 ## License
 
 `jsonPagination` is released under the MIT License. See the LICENSE file for more details.
```

### Comparing `jsonpagination-0.2.5/README.md` & `jsonpagination-0.3.0/jsonPagination.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,28 @@
+Metadata-Version: 2.1
+Name: jsonPagination
+Version: 0.3.0
+Summary: A versatile JSON data downloader with pagination and multithreading support.
+Home-page: https://github.com/pl0psec/jsonPagination
+Author: pl0psec
+Author-email: contact@pl0psec.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: tqdm
+
 # jsonPagination 
 
 [![python](https://img.shields.io/badge/Python-3.9-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![License: GPLv3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-![pylint](https://img.shields.io/badge/PyLint-9.71-green?logo=python&logoColor=white)
+![pylint](https://img.shields.io/badge/PyLint-9.73-green?logo=python&logoColor=white)
 [![GitHub version](https://badge.fury.io/gh/pl0psec%2FjsonPagination.svg)](https://badge.fury.io/gh/pl0psec%2FjsonPagination)
 [![PyPI version](https://badge.fury.io/py/jsonPagination.svg)](https://badge.fury.io/py/jsonPagination)
 
 `jsonPagination` is a Python library designed to simplify the process of fetching and paginating JSON data from APIs. It supports authentication, multithreading for efficient data retrieval, and handling of pagination logic, making it ideal for working with large datasets or APIs with rate limits.
 
 ## Features
 
@@ -23,34 +39,54 @@
 - **Custom Headers Support**: Enables the injection of custom HTTP headers into each request, providing a way to include additional metadata like API keys, session tokens, or other authentication information required by the API.
 
 - **Error Handling and Retry Logic**: Implements robust error detection and retry mechanisms to handle transient network issues or API errors. This ensures that temporary setbacks do not interrupt the data retrieval process, improving the reliability of data fetching operations.
 
 
 ## Installation
 
-To install `jsonPagination`, simply use pip:
+To install `jsonPagination`, you have two options:
+
+1. Install directly using pip:
 
+    ```
     pip install jsonPagination
+    ```
+
+2. If you have a `requirements.txt` file that includes `jsonPagination`, install all the required packages using:
+
+    ```
+    pip install -r requirements.txt
+    ```
+
+Make sure `jsonPagination` is listed in your `requirements.txt` file with the desired version, like so:
+
+```sh
+jsonPagination==x.y.z
+```
+
+Replace `x.y.z` with the specific version number you want to install.
 
 ## Usage
 
 ### Basic Pagination
 Here's how to use `jsonPagination` for basic pagination, demonstrating both page-based and index-based pagination:
 
 ```python
 from jsonPagination.paginator import Paginator
 
-# Page-based pagination example
+# Instantiate the Paginator with a base URL
 paginator = Paginator(
+    base_url='https://api.example.com',
     current_page_field='page',  # Field name used by the API for page number
     items_field='items_per_page',  # Field name used by the API for the number of items per page
     max_threads=2
 )
 
-results = paginator.fetch_all_pages('https://api.example.com/data')
+# Fetch data using a relative path
+results = paginator.fetch_all_pages('/data')
 
 print("Downloaded data:")
 print(results)
 ```
 
 ### Pagination with Authentication
 #### Basic Authentication
@@ -60,81 +96,63 @@
 from jsonPagination.paginator import Paginator
 
 headers = {
     'Authorization': 'Basic <base64_encoded_credentials>'
 }
 
 paginator = Paginator(
+    base_url='https://api.example.com',
     headers=headers,
     max_threads=2
 )
 
-results = paginator.fetch_all_pages('https://api.example.com/data')
+results = paginator.fetch_all_pages('/data')
 
 print("Downloaded data with basic authentication:")
 print(results)
 ```
 
 #### Token-based Authentication
-For APIs requiring a token, provide the login URL and authentication data:
+For APIs requiring a token, configure the `login_url` with the base URL during instantiation:
 
 ```python
 from jsonPagination.paginator import Paginator
+from urllib.parse import urljoin
 
 paginator = Paginator(
-    login_url='https://api.example.com/api/login',
+    base_url='https://api.example.com',
+    login_url=urljoin(base_url, '/api/login'),
     auth_data={'username': 'your_username', 'password': 'your_password'},
     max_threads=2
 )
 
-results = paginator.fetch_all_pages('https://api.example.com/api/data')
+results = paginator.fetch_all_pages('/api/data')
 
 print("Downloaded data with token-based authentication:")
 print(results)
 ```
 
 ### Rate Limit Example
 Demonstrating how to handle rate limits:
 
 ```python
 from jsonPagination.paginator import Paginator
 
 paginator = Paginator(
+    base_url='https://api.example.com',
     max_threads=2,
     ratelimit=(5, 60)  # 5 requests per 60 seconds
 )
 
-results = paginator.fetch_all_pages('https://api.example.com/data')
+results = paginator.fetch_all_pages('/data')
 
 print("Downloaded data with rate limiting:")
 print(results)
 ```
 
-## Configuration
-
-When instantiating the `Paginator` class, you can configure the following parameters to tailor its behavior:
-
-- `url`: The API endpoint URL from which data will be fetched.
-- `login_url` (optional): The URL to authenticate and retrieve a bearer token, used if the API requires token-based authentication.
-- `auth_data` (optional): A dictionary containing authentication data (such as `username` and `password`) required by the login endpoint for obtaining a token.
-- `current_page_field` (optional): The JSON field name used by the API to denote the current page number, applicable for page-number-based pagination.
-- `current_index_field` (optional): The JSON field name used by the API to denote the starting index for data fetching, applicable for index-based pagination.
-- `items_field` (optional): The JSON field name for the number of items to fetch per request, which corresponds to `per_page` in many APIs. This is used to control pagination size.
-- `total_count_field`: The JSON field name that contains the total number of items available, used to calculate the total number of pages or batches.
-- `items_per_page` (optional): Specifies the number of items to request per page or batch. If not set, the Paginator will try to use a sensible default based on the first API response or a predefined value.
-- `max_threads`: The maximum number of threads to use for parallel data fetching, enhancing speed for large datasets.
-- `download_one_page_only` (optional): A boolean indicating whether to fetch only the first page/batch of data, useful for testing or when only a sample of data is needed.
-- `verify_ssl` (optional): Determines whether SSL certificates should be verified in HTTP requests, enhancing security.
-- `data_field`: The specific JSON field name from which to extract the main data in the API response, necessary for parsing the fetched JSON data correctly.
-- `log_level` (optional): Sets the verbosity of logging, with possible values like `DEBUG`, `INFO`, `WARNING`, `ERROR`, and `CRITICAL`, to assist in debugging and monitoring.
-- `headers` (optional): A dictionary of custom HTTP headers to include in every request made by the Paginator, enabling additional customization like API keys or session tokens.
-- `ratelimit` (optional): A tuple specifying the rate limit as `(calls, period)` to prevent exceeding the API's rate limiting policies, ensuring compliant and responsible usage.
-
-These configuration options provide extensive control over how the `Paginator` interacts with the API, including authentication mechanisms, request formatting, error handling, and data retrieval efficiency. By adjusting these parameters, you can optimize the behavior of the Paginator to match the specific requirements and constraints of the API you are working with.
-
 ## Contributing
 
 We welcome contributions to `jsonPagination`! Please open an issue or submit a pull request for any features, bug fixes, or documentation improvements.
 
 ## License
 
 `jsonPagination` is released under the MIT License. See the LICENSE file for more details.
```

### Comparing `jsonpagination-0.2.5/jsonPagination/exceptions.py` & `jsonpagination-0.3.0/jsonPagination/exceptions.py`

 * *Files identical despite different names*

### Comparing `jsonpagination-0.2.5/jsonPagination/paginator.py` & `jsonpagination-0.3.0/jsonPagination/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 customizable authentication, and the option to disable SSL verification for HTTP requests.
 """
 
 import logging
 from queue import Queue
 from threading import Thread, Lock
 import time
+from urllib.parse import urljoin
 
 import requests
 from requests.exceptions import RequestException
 import urllib3
 from tqdm import tqdm
 
 from .exceptions import LoginFailedException, DataFetchFailedException, AuthenticationFailed
@@ -18,15 +19,15 @@
 
 class Paginator:
     """
     A class for fetching and paginating JSON data from APIs with support for multithreading,
     customizable authentication, and the option to disable SSL verification for HTTP requests.
     """
 
-    def __init__(self, login_url=None, auth_data=None, current_page_field=None,
+    def __init__(self, base_url, login_url=None, auth_data=None, current_page_field=None,
                  current_index_field=None, items_field='per_page', total_count_field='total',
                  items_per_page=None, response_items_field=None, max_threads=5, download_one_page_only=False, verify_ssl=True,
                  data_field='data', log_level='INFO', retry_delay=30, ratelimit=None, headers=None):
         """
         Initializes the Paginator with the given configuration.
 
         Args:
@@ -63,28 +64,33 @@
         if not self.logger.handlers:
             console_handler = logging.StreamHandler()
             console_handler.setLevel(logging.getLevelName(log_level))  # Set handler level
             formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
             console_handler.setFormatter(formatter)
             self.logger.addHandler(console_handler)
 
+        # URL
+        self.base_url = base_url
+
         # Auth
         self.login_url = login_url
         self.auth_data = auth_data
         self.token = None
 
         # HTTP
         self.verify_ssl = verify_ssl
         self.request_timeout = 120
 
         self.headers = headers if headers is not None else {}
+        self.retry_lock = Lock()
+        self.is_retrying = False
 
         # Pagination
 
-        # Use `current_page_field` if provided, otherwise default to `current_index_field`        
+        # Use `current_page_field` if provided, otherwise default to `current_index_field`
         self.pagination_field = current_page_field if current_page_field else current_index_field
         self.is_page_based = bool(current_page_field)
 
         self.items_field = items_field
         self.total_count_field = total_count_field
 
         self.data_field = data_field
@@ -93,29 +99,26 @@
         self.response_items_field = response_items_field
         self.download_one_page_only = download_one_page_only
 
         # Threading
         self.max_threads = max_threads
         self.retry = 5
         self.retry_delay = retry_delay
+        self.data_queue = Queue()
 
         # Ratelimit
         self.ratelimit = ratelimit  # should be a tuple like (5, 60) for 5 calls per 60 seconds
         self.last_request_time = None
         self.request_interval = 0 if not ratelimit else ratelimit[1] / ratelimit[0]
 
-        # Where to classify this ?
-        self.data_queue = Queue()
-        self.retry_lock = Lock()
-        self.is_retrying = False
-
         if not self.verify_ssl:
             urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
             self.logger.debug("SSL verification is disabled for all requests.")
 
+
     def flatten_json(self, y):
         """
         Flattens a nested JSON object into a single level dictionary with keys as paths to nested
         values.
 
         This method recursively traverses the nested JSON object, combining keys from different 
         levels into a single key separated by underscores. It handles both nested dictionaries
@@ -171,18 +174,20 @@
         """
         if not self.login_url or not self.auth_data:
             self.logger.error(
                 "Login URL and auth data are required for login.")
             raise ValueError(
                 "Login URL and auth data must be provided for login.")
 
-        self.logger.debug("Logging in to %s", self.login_url)
-        response = requests.post(self.login_url, json=self.auth_data, verify=self.verify_ssl, timeout=self.request_timeout)
+        login_url = urljoin(self.base_url, self.login_url)
 
-        self.logger.debug("Login request to %s returned status code %d", self.login_url, response.status_code)
+        self.logger.debug("Logging in to %s", login_url)
+        response = requests.post(login_url, json=self.auth_data, verify=self.verify_ssl, timeout=self.request_timeout)
+
+        self.logger.debug("Login request to %s returned status code %d", login_url, response.status_code)
 
         if response.status_code == 200:
             self.token = response.json().get('token')
             self.headers['Authorization'] = f'Bearer {self.token}'
             self.logger.info("Login successful with status code %d.", response.status_code)
 
         else:
@@ -227,15 +232,16 @@
                 params[self.pagination_field] = (page - 1) * self.items_per_page
 
             params[self.items_field] = self.items_per_page
 
             self.logger.debug("Parameters for request: %s", params)
 
             # Construct the full URL for logging and request
-            response = requests.get(url, headers=self.headers, params=params, timeout=self.request_timeout, verify=self.verify_ssl)
+            response = requests.get(urljoin(self.base_url, url), headers=self.headers, params=params, timeout=self.request_timeout, verify=self.verify_ssl)
+
             self.logger.debug("Requesting URL: %s with status code: %d", response.request.url, response.status_code)
 
             if response.status_code == 200:
                 data = response.json()
                 fetched_data = data.get(self.data_field, []) if self.data_field else data
 
                 with self.retry_lock:
@@ -305,15 +311,15 @@
         if self.login_url and not self.token and self.auth_data:
             self.login()
 
         effective_headers = self.headers.copy()
         if headers:
             effective_headers.update(headers)
 
-        response = requests.get(url, headers=effective_headers, params=params, verify=self.verify_ssl, timeout=self.request_timeout)
+        response = requests.get(urljoin(self.base_url, url), headers=effective_headers, params=params, verify=self.verify_ssl, timeout=self.request_timeout)
 
         if response.status_code != 200:
             full_url = response.url  # This gives the full URL after the query parameters are applied
 
             # Log detailed error information
             self.logger.error("Failed to fetch data from %s", full_url)
             self.logger.error("HTTP status code: %d", response.status_code)
@@ -329,15 +335,15 @@
         if total_count is None:
             self.logger.warning("Total count field missing, cannot paginate properly.")
             return self.flatten_json(json_data) if flatten_json else json_data
 
         # Set items_per_page based on the initial API call if not set
         if not self.items_per_page:
 
-            # Set items_per_page based on the response, dynamically choosing the field or defaulting as necessary         
+            # Set items_per_page based on the response, dynamically choosing the field or defaulting as necessary
             if self.response_items_field and self.response_items_field in json_data:
                 self.items_per_page = json_data.get(self.response_items_field)
             else:
                 self.items_per_page = json_data.get(self.items_field, 200)
 
         # Determine pagination strategy
         if self.is_page_based:
@@ -366,9 +372,9 @@
                     threads = []
 
             for t in threads:
                 t.join()
 
         while not self.data_queue.empty():
             results.extend(self.data_queue.get())
-        
+
         return [self.flatten_json(item) if flatten_json else item for item in results]
```

### Comparing `jsonpagination-0.2.5/jsonPagination.egg-info/PKG-INFO` & `jsonpagination-0.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,12 @@
-Metadata-Version: 2.1
-Name: jsonPagination
-Version: 0.2.5
-Summary: A versatile JSON data downloader with pagination and multithreading support.
-Home-page: https://github.com/pl0psec/jsonPagination
-Author: pl0psec
-Author-email: contact@pl0psec.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: tqdm
-
 # jsonPagination 
 
 [![python](https://img.shields.io/badge/Python-3.9-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![License: GPLv3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-![pylint](https://img.shields.io/badge/PyLint-9.71-green?logo=python&logoColor=white)
+![pylint](https://img.shields.io/badge/PyLint-9.73-green?logo=python&logoColor=white)
 [![GitHub version](https://badge.fury.io/gh/pl0psec%2FjsonPagination.svg)](https://badge.fury.io/gh/pl0psec%2FjsonPagination)
 [![PyPI version](https://badge.fury.io/py/jsonPagination.svg)](https://badge.fury.io/py/jsonPagination)
 
 `jsonPagination` is a Python library designed to simplify the process of fetching and paginating JSON data from APIs. It supports authentication, multithreading for efficient data retrieval, and handling of pagination logic, making it ideal for working with large datasets or APIs with rate limits.
 
 ## Features
 
@@ -39,34 +23,54 @@
 - **Custom Headers Support**: Enables the injection of custom HTTP headers into each request, providing a way to include additional metadata like API keys, session tokens, or other authentication information required by the API.
 
 - **Error Handling and Retry Logic**: Implements robust error detection and retry mechanisms to handle transient network issues or API errors. This ensures that temporary setbacks do not interrupt the data retrieval process, improving the reliability of data fetching operations.
 
 
 ## Installation
 
-To install `jsonPagination`, simply use pip:
+To install `jsonPagination`, you have two options:
+
+1. Install directly using pip:
 
+    ```
     pip install jsonPagination
+    ```
+
+2. If you have a `requirements.txt` file that includes `jsonPagination`, install all the required packages using:
+
+    ```
+    pip install -r requirements.txt
+    ```
+
+Make sure `jsonPagination` is listed in your `requirements.txt` file with the desired version, like so:
+
+```sh
+jsonPagination==x.y.z
+```
+
+Replace `x.y.z` with the specific version number you want to install.
 
 ## Usage
 
 ### Basic Pagination
 Here's how to use `jsonPagination` for basic pagination, demonstrating both page-based and index-based pagination:
 
 ```python
 from jsonPagination.paginator import Paginator
 
-# Page-based pagination example
+# Instantiate the Paginator with a base URL
 paginator = Paginator(
+    base_url='https://api.example.com',
     current_page_field='page',  # Field name used by the API for page number
     items_field='items_per_page',  # Field name used by the API for the number of items per page
     max_threads=2
 )
 
-results = paginator.fetch_all_pages('https://api.example.com/data')
+# Fetch data using a relative path
+results = paginator.fetch_all_pages('/data')
 
 print("Downloaded data:")
 print(results)
 ```
 
 ### Pagination with Authentication
 #### Basic Authentication
@@ -76,81 +80,63 @@
 from jsonPagination.paginator import Paginator
 
 headers = {
     'Authorization': 'Basic <base64_encoded_credentials>'
 }
 
 paginator = Paginator(
+    base_url='https://api.example.com',
     headers=headers,
     max_threads=2
 )
 
-results = paginator.fetch_all_pages('https://api.example.com/data')
+results = paginator.fetch_all_pages('/data')
 
 print("Downloaded data with basic authentication:")
 print(results)
 ```
 
 #### Token-based Authentication
-For APIs requiring a token, provide the login URL and authentication data:
+For APIs requiring a token, configure the `login_url` with the base URL during instantiation:
 
 ```python
 from jsonPagination.paginator import Paginator
+from urllib.parse import urljoin
 
 paginator = Paginator(
-    login_url='https://api.example.com/api/login',
+    base_url='https://api.example.com',
+    login_url=urljoin(base_url, '/api/login'),
     auth_data={'username': 'your_username', 'password': 'your_password'},
     max_threads=2
 )
 
-results = paginator.fetch_all_pages('https://api.example.com/api/data')
+results = paginator.fetch_all_pages('/api/data')
 
 print("Downloaded data with token-based authentication:")
 print(results)
 ```
 
 ### Rate Limit Example
 Demonstrating how to handle rate limits:
 
 ```python
 from jsonPagination.paginator import Paginator
 
 paginator = Paginator(
+    base_url='https://api.example.com',
     max_threads=2,
     ratelimit=(5, 60)  # 5 requests per 60 seconds
 )
 
-results = paginator.fetch_all_pages('https://api.example.com/data')
+results = paginator.fetch_all_pages('/data')
 
 print("Downloaded data with rate limiting:")
 print(results)
 ```
 
-## Configuration
-
-When instantiating the `Paginator` class, you can configure the following parameters to tailor its behavior:
-
-- `url`: The API endpoint URL from which data will be fetched.
-- `login_url` (optional): The URL to authenticate and retrieve a bearer token, used if the API requires token-based authentication.
-- `auth_data` (optional): A dictionary containing authentication data (such as `username` and `password`) required by the login endpoint for obtaining a token.
-- `current_page_field` (optional): The JSON field name used by the API to denote the current page number, applicable for page-number-based pagination.
-- `current_index_field` (optional): The JSON field name used by the API to denote the starting index for data fetching, applicable for index-based pagination.
-- `items_field` (optional): The JSON field name for the number of items to fetch per request, which corresponds to `per_page` in many APIs. This is used to control pagination size.
-- `total_count_field`: The JSON field name that contains the total number of items available, used to calculate the total number of pages or batches.
-- `items_per_page` (optional): Specifies the number of items to request per page or batch. If not set, the Paginator will try to use a sensible default based on the first API response or a predefined value.
-- `max_threads`: The maximum number of threads to use for parallel data fetching, enhancing speed for large datasets.
-- `download_one_page_only` (optional): A boolean indicating whether to fetch only the first page/batch of data, useful for testing or when only a sample of data is needed.
-- `verify_ssl` (optional): Determines whether SSL certificates should be verified in HTTP requests, enhancing security.
-- `data_field`: The specific JSON field name from which to extract the main data in the API response, necessary for parsing the fetched JSON data correctly.
-- `log_level` (optional): Sets the verbosity of logging, with possible values like `DEBUG`, `INFO`, `WARNING`, `ERROR`, and `CRITICAL`, to assist in debugging and monitoring.
-- `headers` (optional): A dictionary of custom HTTP headers to include in every request made by the Paginator, enabling additional customization like API keys or session tokens.
-- `ratelimit` (optional): A tuple specifying the rate limit as `(calls, period)` to prevent exceeding the API's rate limiting policies, ensuring compliant and responsible usage.
-
-These configuration options provide extensive control over how the `Paginator` interacts with the API, including authentication mechanisms, request formatting, error handling, and data retrieval efficiency. By adjusting these parameters, you can optimize the behavior of the Paginator to match the specific requirements and constraints of the API you are working with.
-
 ## Contributing
 
 We welcome contributions to `jsonPagination`! Please open an issue or submit a pull request for any features, bug fixes, or documentation improvements.
 
 ## License
 
 `jsonPagination` is released under the MIT License. See the LICENSE file for more details.
```

### Comparing `jsonpagination-0.2.5/setup.py` & `jsonpagination-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='jsonPagination',
-    version='0.2.5',
+    version='0.3.0',
     author='pl0psec',
     author_email='contact@pl0psec.com',
     description='A versatile JSON data downloader with pagination and multithreading support.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/pl0psec/jsonPagination',
     packages=find_packages(),
```


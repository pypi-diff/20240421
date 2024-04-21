# Comparing `tmp/gie-py-0.4.4.tar.gz` & `tmp/gie_py-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gie-py-0.4.4.tar", last modified: Mon Feb  5 15:56:02 2024, max compression
+gzip compressed data, was "gie_py-0.4.5.tar", last modified: Sun Apr 21 20:09:04 2024, max compression
```

## Comparing `gie-py-0.4.4.tar` & `gie_py-0.4.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 15:56:02.663983 gie-py-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-05 15:55:55.000000 gie-py-0.4.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-02-05 15:56:02.663983 gie-py-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-02-05 15:55:55.000000 gie-py-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 15:56:02.659983 gie-py-0.4.4/gie/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-05 15:55:55.000000 gie-py-0.4.4/gie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15508 2024-02-05 15:55:55.000000 gie-py-0.4.4/gie/agsi_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-02-05 15:55:55.000000 gie-py-0.4.4/gie/alsi_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-05 15:55:55.000000 gie-py-0.4.4/gie/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-02-05 15:55:55.000000 gie-py-0.4.4/gie/gie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 15:56:02.659983 gie-py-0.4.4/gie_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-02-05 15:56:02.000000 gie-py-0.4.4/gie_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-05 15:56:02.000000 gie-py-0.4.4/gie_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 15:56:02.000000 gie-py-0.4.4/gie_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-05 15:56:02.000000 gie-py-0.4.4/gie_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-05 15:56:02.000000 gie-py-0.4.4/gie_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-05 15:56:02.663983 gie-py-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-02-05 15:55:55.000000 gie-py-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:09:04.379681 gie_py-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 20:08:56.000000 gie_py-0.4.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-21 20:09:04.379681 gie_py-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-21 20:08:56.000000 gie_py-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:09:04.379681 gie_py-0.4.5/gie/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-21 20:08:56.000000 gie_py-0.4.5/gie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15508 2024-04-21 20:08:56.000000 gie_py-0.4.5/gie/agsi_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-04-21 20:08:56.000000 gie_py-0.4.5/gie/alsi_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-21 20:08:56.000000 gie_py-0.4.5/gie/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-04-21 20:08:56.000000 gie_py-0.4.5/gie/gie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:09:04.379681 gie_py-0.4.5/gie_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-21 20:09:04.000000 gie_py-0.4.5/gie_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-21 20:09:04.000000 gie_py-0.4.5/gie_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 20:09:04.000000 gie_py-0.4.5/gie_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-21 20:09:04.000000 gie_py-0.4.5/gie_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-21 20:09:04.000000 gie_py-0.4.5/gie_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-21 20:09:04.379681 gie_py-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-21 20:08:56.000000 gie_py-0.4.5/setup.py
```

### Comparing `gie-py-0.4.4/LICENSE.md` & `gie_py-0.4.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gie-py-0.4.4/PKG-INFO` & `gie_py-0.4.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gie-py
-Version: 0.4.4
+Version: 0.4.5
 Summary: A python API wrapper for alsi.gie.eu and agsi.gie.eu
 Home-page: https://github.com/fboerman/gie-py
 Author: Frank Boerman
 Author-email: frank@fboerman.nl
 License: MIT
 Keywords: GIE data api energy gas
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gie-py-0.4.4/README.md` & `gie_py-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `gie-py-0.4.4/gie/agsi_mappings.py` & `gie_py-0.4.5/gie/agsi_mappings.py`

 * *Files identical despite different names*

### Comparing `gie-py-0.4.4/gie/alsi_mappings.py` & `gie_py-0.4.5/gie/alsi_mappings.py`

 * *Files identical despite different names*

### Comparing `gie-py-0.4.4/gie/gie.py` & `gie_py-0.4.5/gie/gie.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 import requests
+from requests.adapters import HTTPAdapter, Retry
 import pandas as pd
 from typing import List, Dict, Union
 from .agsi_mappings import AGSICompany, AGSIStorage, AGSICountry, lookup_company, lookup_storage, lookup_country
-from .alsi_mappings import ALSITerminal, ALSILSO, ALSICountry, lookup_terminal, lookup_lso, lookup_country as lookup_country_alsi
+from .alsi_mappings import ALSITerminal, ALSILSO, ALSICountry, lookup_terminal, lookup_lso, \
+    lookup_country as lookup_country_alsi
 from .exceptions import *
 from enum import Enum
 
 __title__ = "gie-py"
-__version__ = "0.4.4"
+__version__ = "0.4.5"
 __author__ = "Frank Boerman"
 __license__ = "MIT"
 
 
 class APIType(str, Enum):
     AGSI = "https://agsi.gie.eu/api"
     ALSI = "https://alsi.gie.eu/api"
 
 
 class GieRawClient:
     def __init__(self, api_key):
         self.s = requests.Session()
+        retries = Retry(total=5,
+                        backoff_factor=0.1,
+                        status_forcelist=[500, 502, 503, 504])
+        self.s.mount('http://', HTTPAdapter(max_retries=retries))
+        self.s.mount('https://', HTTPAdapter(max_retries=retries))
         self.s.headers.update({
             'user-agent': f'gie-py v{__version__} (github.com/fboerman/gie-py)',
             'x-key': api_key
         })
 
     def _fetch(self, obj, t: APIType,
                start: Union[pd.Timestamp, str], end: Union[pd.Timestamp, str]):
-        if type(start) != pd.Timestamp:
+        if type(start) is not pd.Timestamp:
             start = pd.Timestamp(start)
-        if type(end) != pd.Timestamp:
+        if type(end) is not pd.Timestamp:
             end = pd.Timestamp(end)
 
         def _fetch_one(start, end, obj, page=1):
             r = self.s.get(t.value, params={
-                'from': start.strftime('%Y-%m-%d'),
-                'till': end.strftime('%Y-%m-%d'),
-                'size': 300,
-                'page': page
-            } | obj.get_params())
+                                               'from': start.strftime('%Y-%m-%d'),
+                                               'till': end.strftime('%Y-%m-%d'),
+                                               'size': 300,
+                                               'page': page
+                                           } | obj.get_params())
             r.raise_for_status()
 
             return r.json()
 
         r = _fetch_one(start, end, obj)
         data = r['data']
         if r['last_page'] != 1:
@@ -61,56 +68,63 @@
 
     def query_gas_company(self, company: Union[AGSICompany, str],
                           start: Union[pd.Timestamp, str], end: Union[pd.Timestamp, str]) -> List[Dict]:
         company = lookup_company(company)
         return self._fetch(company, APIType.AGSI, start=start, end=end)
 
     def query_gas_country(self, country: Union[AGSICountry, str],
-                      start: Union[pd.Timestamp, str], end: Union[pd.Timestamp, str]) -> List[Dict]:
+                          start: Union[pd.Timestamp, str], end: Union[pd.Timestamp, str]) -> List[Dict]:
         country = lookup_country(country)
         return self._fetch(country, APIType.AGSI, start=start, end=end)
 
     def query_lng_terminal(self, terminal: Union[ALSITerminal, str],
                            start: Union[pd.Timestamp, str], end: Union[pd.Timestamp, str]) -> List[Dict]:
         terminal = lookup_terminal(terminal)
         return self._fetch(terminal, APIType.ALSI, start=start, end=end)
 
     def query_lng_lso(self, lso: Union[ALSILSO, str],
-                           start: Union[pd.Timestamp, str], end: Union[pd.Timestamp, str]) -> List[Dict]:
+                      start: Union[pd.Timestamp, str], end: Union[pd.Timestamp, str]) -> List[Dict]:
         lso = lookup_lso(lso)
         return self._fetch(lso, APIType.ALSI, start=start, end=end)
 
     def query_lng_country(self, country: Union[ALSICountry, str],
                           start: Union[pd.Timestamp, str], end: Union[pd.Timestamp, str]) -> List[Dict]:
         country = lookup_country_alsi(country)
         return self._fetch(country, APIType.ALSI, start=start, end=end)
 
 
 class GiePandasClient(GieRawClient):
-    def _fix_dataframe(self, data):
+    @staticmethod
+    def _fix_dataframe(data):
         def _fix_values(x):
             if 'inventory' in x:
                 x['inventory'] = x['inventory']['lng']
             if 'dtmi' in x:
                 x['dtmi'] = x['dtmi']['lng']
             return x
+
         df = pd.DataFrame([_fix_values(x) for x in data])
         for c in ['name', 'code', 'url', 'info']:
             if c in df:
                 df = df.drop(columns=c)
         df = df.loc[df['status'] != 'N']
         df['gasDayStart'] = pd.to_datetime(df['gasDayStart'])
         df = df.set_index('gasDayStart')
         # status is only str column, save it for now, convert whole dataframe to float, restore status
         status = df['status'].copy()
         updated_at = pd.to_datetime(df['updatedAt'])
         df = df.drop(columns=['status', 'updatedAt'])
         if 'type' in df:
             df = df.drop(columns=['type'])
-        df = df.replace('-', 0).astype(float)
+        for column in df.columns:
+            try:
+                df[column] = pd.to_numeric(df[column].replace('-', 0))
+            except ValueError:
+                pass
+        # df = df.replace('-', 0).astype(float)
         df['status'] = status
         df['updatedAt'] = updated_at
         return df
 
     def query_gas_storage(self, storage: Union[AGSIStorage, str],
                           start: Union[pd.Timestamp, str], end: Union[pd.Timestamp, str]) -> pd.DataFrame:
         return self._fix_dataframe(
@@ -120,27 +134,27 @@
     def query_gas_company(self, company: Union[AGSIStorage, str],
                           start: Union[pd.Timestamp, str], end: Union[pd.Timestamp, str]) -> pd.DataFrame:
         return self._fix_dataframe(
             super().query_gas_company(company=company, start=start, end=end)
         )
 
     def query_gas_country(self, country: Union[AGSICountry, str],
-                      start: Union[pd.Timestamp, str], end: Union[pd.Timestamp, str]) -> pd.DataFrame:
+                          start: Union[pd.Timestamp, str], end: Union[pd.Timestamp, str]) -> pd.DataFrame:
         return self._fix_dataframe(
             super().query_gas_country(country=country, start=start, end=end)
         )
 
     def query_lng_terminal(self, terminal: Union[ALSITerminal, str],
                            start: Union[pd.Timestamp, str], end: Union[pd.Timestamp, str]) -> pd.DataFrame:
         return self._fix_dataframe(
             super().query_lng_terminal(terminal=terminal, start=start, end=end)
         )
 
     def query_lng_lso(self, lso: Union[ALSILSO, str],
-                           start: Union[pd.Timestamp, str], end: Union[pd.Timestamp, str]) -> pd.DataFrame:
+                      start: Union[pd.Timestamp, str], end: Union[pd.Timestamp, str]) -> pd.DataFrame:
         return self._fix_dataframe(
             super().query_lng_lso(lso=lso, start=start, end=end)
         )
 
     def query_lng_country(self, country: Union[ALSICountry, str],
                           start: Union[pd.Timestamp, str], end: Union[pd.Timestamp, str]) -> List[Dict]:
         return self._fix_dataframe(
```

### Comparing `gie-py-0.4.4/gie_py.egg-info/PKG-INFO` & `gie_py-0.4.5/gie_py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gie-py
-Version: 0.4.4
+Version: 0.4.5
 Summary: A python API wrapper for alsi.gie.eu and agsi.gie.eu
 Home-page: https://github.com/fboerman/gie-py
 Author: Frank Boerman
 Author-email: frank@fboerman.nl
 License: MIT
 Keywords: GIE data api energy gas
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gie-py-0.4.4/setup.py` & `gie_py-0.4.5/setup.py`

 * *Files identical despite different names*


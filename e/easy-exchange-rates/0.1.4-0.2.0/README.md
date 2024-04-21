# Comparing `tmp/easy_exchange_rates-0.1.4.tar.gz` & `tmp/easy_exchange_rates-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/easy-exchange-rates/easy-exchange-rates/dist/tmpvan98e2z/easy_exchange_rates-0.1.4.tar", last modified: Tue Aug 17 13:42:10 2021, max compression
+gzip compressed data, was "easy_exchange_rates-0.2.0.tar", last modified: Sun Apr 21 16:38:18 2024, max compression
```

## Comparing `easy_exchange_rates-0.1.4.tar` & `easy_exchange_rates-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 13:42:10.000000 easy_exchange_rates-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-08-17 13:41:49.000000 easy_exchange_rates-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2021-08-17 13:42:10.000000 easy_exchange_rates-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2021-08-17 13:41:49.000000 easy_exchange_rates-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-08-17 13:41:49.000000 easy_exchange_rates-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      731 2021-08-17 13:42:10.000000 easy_exchange_rates-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 13:42:10.000000 easy_exchange_rates-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 13:42:10.000000 easy_exchange_rates-0.1.4/src/easy_exchange_rates/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-08-17 13:41:49.000000 easy_exchange_rates-0.1.4/src/easy_exchange_rates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2021-08-17 13:41:49.000000 easy_exchange_rates-0.1.4/src/easy_exchange_rates/eer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 13:42:10.000000 easy_exchange_rates-0.1.4/src/easy_exchange_rates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2021-08-17 13:42:10.000000 easy_exchange_rates-0.1.4/src/easy_exchange_rates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      297 2021-08-17 13:42:10.000000 easy_exchange_rates-0.1.4/src/easy_exchange_rates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-17 13:42:10.000000 easy_exchange_rates-0.1.4/src/easy_exchange_rates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-08-17 13:42:10.000000 easy_exchange_rates-0.1.4/src/easy_exchange_rates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:38:18.956991 easy_exchange_rates-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 16:38:04.000000 easy_exchange_rates-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-21 16:38:18.956991 easy_exchange_rates-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-21 16:38:04.000000 easy_exchange_rates-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-21 16:38:04.000000 easy_exchange_rates-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-21 16:38:18.956991 easy_exchange_rates-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:38:18.952990 easy_exchange_rates-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:38:18.956991 easy_exchange_rates-0.2.0/src/easy_exchange_rates/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-21 16:38:04.000000 easy_exchange_rates-0.2.0/src/easy_exchange_rates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-21 16:38:04.000000 easy_exchange_rates-0.2.0/src/easy_exchange_rates/eer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:38:18.956991 easy_exchange_rates-0.2.0/src/easy_exchange_rates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-21 16:38:18.000000 easy_exchange_rates-0.2.0/src/easy_exchange_rates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-21 16:38:18.000000 easy_exchange_rates-0.2.0/src/easy_exchange_rates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 16:38:18.000000 easy_exchange_rates-0.2.0/src/easy_exchange_rates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-21 16:38:18.000000 easy_exchange_rates-0.2.0/src/easy_exchange_rates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:38:18.956991 easy_exchange_rates-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-21 16:38:04.000000 easy_exchange_rates-0.2.0/tests/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `easy_exchange_rates-0.1.4/LICENSE` & `easy_exchange_rates-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_exchange_rates-0.1.4/README.md` & `easy_exchange_rates-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-# easy-exchange-rates
+# Easy Exchange Rates
 
-[![PyPI package](https://img.shields.io/badge/pip%20install-easy--exchange--rates-brightgreen)](https://pypi.org/project/easy-exchange-rates/) [![version number](https://img.shields.io/pypi/v/easy-exchange-rates?color=green&label=version)](https://pypi.org/project/easy-exchange-rates/releases) [![Actions Status](https://github.com/tomchen/example_pypi_package/workflows/Test/badge.svg)](https://github.com/oddaspa/easy-exchange-rates/actions) [![License](https://img.shields.io/github/license/oddaspa/easy-exchange-rates)](https://github.com/oddaspa/easy-exchange-rates/blob/main/LICENSE.txt)
+[![PyPI package](https://img.shields.io/badge/pip%20install-easy--exchange--rates-brightgreen)](https://pypi.org/project/easy-exchange-rates/) 
+[![version number](https://img.shields.io/pypi/v/easy-exchange-rates?color=green&label=version)](https://pypi.org/project/easy-exchange-rates/) 
+[![Actions Status](https://github.com/oddaspa/easy-exchange-rates/workflows/Build%20status/badge.svg)](https://github.com/oddaspa/easy-exchange-rates/actions) 
+[![License](https://img.shields.io/github/license/oddaspa/easy-exchange-rates)](https://github.com/oddaspa/easy-exchange-rates/blob/main/LICENSE.txt)
 
+A python package for retrieving currency exchange data from https://data.ecb.europa.eu/ to a pandas dataframe.
 ## Usage
 ```python
 from easy_exchange_rates import API
 api = API()
-time_series = api.get_exchange_rates(
+df = api.get_exchange_rates(
   base_currency="EUR", 
-  start_date="2021-01-01", 
-  end_date="2021-08-13", 
+  start_date="2024-03-12",
+  end_date="2024-04-21",
   targets=["USD","CAD"]
 )
-data_frame = api.to_dataframe(time_series)
-print(data_frame.head(5))
+print(df.head(5))
 >>>
-                 CAD       USD
-2021-01-01  1.549988  1.217582
-2021-01-02  1.544791  1.213500
-2021-01-03  1.557791  1.223409
-2021-01-04  1.566076  1.225061
-2021-01-05  1.558553  1.229681
+	        CAD	    USD
+TIME_PERIOD		
+2024-03-12	1.4739	1.0916
+2024-03-13	1.4756	1.0939
+2024-03-14	1.4725	1.0925
+2024-03-15	1.4731	1.0892
+2024-03-18	1.4745	1.0892
 ```
 
 
 # Testing
 
 ```
 python3 -m unittest discover -s tests
-```
+```
```

### Comparing `easy_exchange_rates-0.1.4/setup.cfg` & `easy_exchange_rates-0.2.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [metadata]
 name = easy_exchange_rates
-version = 0.1.4
+version = 0.2.0
 author = Odd Gunnar Aspaas
-author_email = oddlearning@gmail.com
-description = Easy abstraction to get currency exchange data from https://exchangerate.host/ to a pandas dataframe.
+author_email = odd.gunnar.aspaas@gmail.com
+description = Easy way to get currency exchange data from https://data.ecb.europa.eu/ to a pandas dataframe.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/oddaspa/easy-exchange-rates
 project_urls = 
 	Bug Tracker = https://github.com/oddaspa/easy-exchange-rates/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.8
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `easy_exchange_rates-0.1.4/src/easy_exchange_rates/eer.py` & `easy_exchange_rates-0.2.0/src/easy_exchange_rates/eer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import requests
 from datetime import datetime
 import pandas as pd
+import io
 
 class API():    
 
     def __init__(self):
-        self.base_url = 'https://api.exchangerate.host/timeseries?'
+        self.base_url = 'https://data-api.ecb.europa.eu/service/data/EXR/'
         
     def get_exchange_rates(self, base_currency="EUR", start_date="2020-01-01", end_date="2020-01-04",targets=[]):
-        date_format = "%Y-%m-%d"
-        a = datetime.strptime(start_date, date_format)
-        b = datetime.strptime(end_date, date_format)
-        delta = b - a
-        if delta.days > 366:
-            print("Can not retieve more than 366 days of data")
-            return False
-        query = self.base_url + f'start_date={start_date}&end_date={end_date}&base={base_currency}'
-        if targets:
-            targets = ','.join(targets)
-            query += f'&symbols={targets}'
-        response = requests.get(query).json()
-        if response["success"]:
-            return response["rates"]
+        
+        query = f'{self.base_url}D.{"+".join(targets)}.{base_currency}.SP00.A'
+        
+        response = requests.get(
+            query,
+            params = {
+                'startPeriod': start_date,
+                'endPeriod': end_date
+            },
+            headers = {'Accept': 'text/csv'})
+
+        if response.ok:
+            df = pd.read_csv(io.StringIO(response.text))
+            df = df.set_index("TIME_PERIOD")
+            df = df[["CURRENCY", "OBS_VALUE"]]
+            df = df.pivot(columns=["CURRENCY"])
+            df.columns = [c[1] for c in df.columns]
+            return df
         else:
             return response
-    
-    def to_dataframe(self,ts):
-        return pd.DataFrame(ts).T
 
     def rolling_average(self, df, window=7):
         roll = df.rolling(window).mean()
         roll.columns = [f"roll_{window}_{tag}" for tag in list(roll.columns)]
         return df.merge(roll,right_index=True, left_index=True)
 
     def rolling_max(self, df, window=7):
```


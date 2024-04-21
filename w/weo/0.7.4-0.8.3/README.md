# Comparing `tmp/weo-0.7.4.tar.gz` & `tmp/weo-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weo-0.7.4.tar", max compression
+gzip compressed data, was "weo-0.8.3.tar", max compression
```

## Comparing `weo-0.7.4.tar` & `weo-0.8.3.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     5991 2022-07-25 08:55:27.057297 weo-0.7.4/README.md
--rw-r--r--   0        0        0      782 2022-07-25 08:55:46.005548 weo-0.7.4/pyproject.toml
--rw-r--r--   0        0        0      563 2022-05-15 15:14:22.536006 weo-0.7.4/weo/__init__.py
--rw-r--r--   0        0        0    11542 2022-05-15 15:14:22.536006 weo-0.7.4/weo/dataframe.py
--rwxr-xr-x   0        0        0     5876 2022-05-15 16:01:14.762390 weo-0.7.4/weo/dates.py
--rw-r--r--   0        0        0     6953 2022-07-25 08:56:01.492365 weo-0.7.4/setup.py
--rw-r--r--   0        0        0     6627 2022-07-25 08:56:01.492934 weo-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     5966 2024-04-21 18:12:15.817471 weo-0.8.3/README.md
+-rw-r--r--   0        0        0      539 2024-04-21 18:48:06.421510 weo-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0      541 2024-04-21 19:00:18.741523 weo-0.8.3/weo/__init__.py
+-rw-r--r--   0        0        0    11532 2024-04-21 18:47:37.157509 weo-0.8.3/weo/dataframe.py
+-rwxr-xr-x   0        0        0     6082 2024-04-21 18:10:21.257469 weo-0.8.3/weo/dates.py
+-rw-r--r--   0        0        0     6709 1970-01-01 00:00:00.000000 weo-0.8.3/PKG-INFO
```

### Comparing `weo-0.7.4/README.md` & `weo-0.8.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 
 ## Dataset releases (vintages)
 
 Dataset releases (vintages) are available back to 2007, the reported data goes back to 1980, forecast is three years ahead.
 
 | Release          | Date         |
 | :--------------- | :-----------:|
-| Latest confirmed | April 2022   |
+| Latest confirmed | April 2024   |
 | First            | October 2007 |
 
 Confirmed release is tested to be processed with `weo`.
 Usually, if something breaks in a new release users raise an [issue here](https://github.com/epogrebnyak/weo-reader/issues).
 
 [weo]: https://www.imf.org/en/Publications/WEO
 
 ![изображение](https://user-images.githubusercontent.com/9265326/103473902-8c64da00-4dae-11eb-957c-4737f56abdce.png)
 
 ## Install
 
-The program is tested to run with Python 3.7.13 (as in Google Colab) and higher.
+The program is tested to run with Python 3.8 or higher.
 
 To install:
 
 ```
 pip install weo
 ```
```

### Comparing `weo-0.7.4/weo/dataframe.py` & `weo-0.8.3/weo/dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Access WEO data as dataframe
 
   from weo import WEO
   w = WEO('weo.csv')
   
 """
+
 import numpy as np  # type: ignore
 import pandas as pd  # type: ignore
 from iso3166 import countries  # type: ignore
 
 
 class WEO_ParsingError(ValueError):
     pass
@@ -60,15 +61,15 @@
     def inner(self, *arg, year=None, start_year=None, end_year=None):
         df = func(self)
         if arg:
             year = arg[0]
         elif start_year and end_year:
             year = [start_year + y for y in range(end_year - start_year + 1)]
         if year:
-            if type(year) == list:
+            if isinstance(year, list):
                 year = [str(y) for y in year]
             else:
                 year = str(year)
 
             ts = df.transpose()[year]
             return ts
         else:
@@ -128,15 +129,15 @@
 
     @property
     def years(self):
         return [x for x in self.df.columns if x.isdigit()]
 
     @property
     def daterange(self):
-        return pd.period_range(start=self.years[0], end=self.years[-1], freq="A")
+        return pd.period_range(start=self.years[0], end=self.years[-1], freq="Y")
 
     @property
     def core_codes(self):
         return [
             x
             for x in [
                 # GDP
@@ -279,26 +280,26 @@
 
     def _get_by_code(self, variable_code):
         ix = self.df["WEO Subject Code"] == variable_code
         return self.df[ix]
 
     def t(self, df, column):
         """Extract columns with years from *df*, make *column* an index."""
-        _df = df[self.years + [column]].set_index(column).transpose().applymap(convert)
+        _df = df[self.years + [column]].set_index(column).transpose().map(convert)
         _df.columns.name = ""
         _df.index = self.daterange
         return _df
 
     def _extract(self, ix, column):
         """Extract columns with years from *df*, make *column* an index."""
         _df = (
             self.df[ix][self.years + [column]]
             .set_index(column)
             .transpose()
-            .applymap(convert)
+            .map(convert)
         )
         _df.columns.name = ""
         _df.index = self.daterange
         return _df
 
     def get(self, subject: str, unit: str):
         self.check_subject(subject)
@@ -312,15 +313,15 @@
 
     # assessors in other dimensions (WIP)
 
     def fix_year(self, year):
         return (
             self.df[["ISO", "WEO Subject Code", str(year)]]
             .pivot(index="WEO Subject Code", columns="ISO", values=str(year))
-            .applymap(convert)
+            .map(convert)
         )
 
     def country(self, iso_code, year=None, compact=True):
         """
         Must add:
             - exchange rate
             - plottable information
```

### Comparing `weo-0.7.4/weo/dates.py` & `weo-0.8.3/weo/dates.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,20 +12,16 @@
     "all_releases",
     "make_url_countries",
     "make_url_commodities",
     "Date",
 ]
 
 
-def cur_year() -> int:
-    return datetime.today().year
-
-
-def cur_month() -> int:
-    return datetime.today().month
+def today():
+    return datetime.today()
 
 
 class Release(Enum):
     Spring = 1
     Fall = 2
 
 
@@ -41,30 +37,30 @@
         return (self.year, self.release) < (x.year, x.release)
 
     def __le__(self, x):
         return (self < x) | (self == x)
 
 
 def succ(d: Date) -> Date:
-    year, rel = d.year, d.release
-    if rel == 2:
+    year, release = d.year, d.release
+    if release == 2:
         year += 1
-        rel = 1
+        release = 1
     else:
-        rel = 2
-    return Date(year, rel)
+        release = 2
+    return Date(year, release)
 
 
 def first() -> Date:
     return Date(2007, 2)
 
 
 def current() -> Date:
-    y = cur_year()
-    m = cur_month()
+    y = today().year
+    m = today().month
     if m <= 3:
         return Date(y - 1, 2)
     elif 4 <= m < 10:
         return Date(y, 1)
     elif m >= 10:
         return Date(y, 2)
     else:
@@ -80,34 +76,42 @@
         return 4
 
 
 def month_str(d: Date) -> str:
     return {4: "Apr", 9: "Sep", 10: "Oct"}[month(d)]
 
 
+def long_month_str(d: Date) -> str:
+    return {4: "April", 9: "September", 10: "October"}[month(d)]
+
+
 def name(d: Date) -> str:
     return f"{d.year}-{month_str(d)} WEO dataset"
 
 
 def period_str(d: Date) -> str:
     return str(d.release).zfill(2)
 
 
 def create_url(d: Date, prefix: str):
     base_url = "https://www.imf.org/-/media/Files/Publications/WEO/WEO-Database"
     year = d.year
     month = month_str(d)
-    # another url break in Apr 2021 - we assume the URL will persist
+    long_month = long_month_str(d)
+    # New break in Apr 2024
+    if d >= Date(2024, 1):
+        return f"{base_url}/{year}/{long_month}/WEO{month}{year}{prefix}.xls"
+    # URL format breaks in Apr 2021
     if d >= Date(2021, 1):
         return f"{base_url}/{year}/WEO{month}{year}{prefix}.ashx"
-    # url break in Oct 2020
+    # URL format breaks in Oct 2020
     if d >= Date(2020, 2):
         period_marker = period_str(d)
         return f"{base_url}/{year}/{period_marker}/WEO{month}{year}{prefix}.xls"
-    # earliest files
+    # the earliest files
     return f"{base_url}/{year}/WEO{month}{year}{prefix}.xls"
 
 
 def make_url_countries(d: Date):
     return create_url(d, prefix="all")
 
 
@@ -176,14 +180,15 @@
         filename = default_filename(d)
     if directory is None:
         path = filename
     else:
         path = os.path.join(directory, filename)
     return os.path.normpath(path)
 
+
 # https://www.python-httpx.org/advanced/#monitoring-download-progress
 def curl(path: str, url: str):
     with open(path, "wb") as f:
         with httpx.stream("GET", url) as r:
             for chunk in r.iter_bytes():
                 f.write(chunk)
     print(path, size_str(path))
@@ -227,15 +232,15 @@
 
     Parameters
     ----------
     year : int
         Year of WEO release.
     release : int or str
         For spring WEO release use 1 or 'Apr'
-        For fall WEO release use 2, 'Oct' or (in 2011) - 'Sep'.
+        For fall WEO release use 2, or 'Oct'. In 2011 use 2 or 'Sep'.
     filename : str
         Filename where to save file.
     directory:
         Directory where to write file.
     fetch: callable, optional
         Used for testing.
```

### Comparing `weo-0.7.4/setup.py` & `weo-0.8.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,227 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: weo
+Version: 0.8.3
+Summary: Python client to download IMF World Economic Outlook (WEO) dataset as pandas dataframes.
+Home-page: https://github.com/epogrebnyak/weo-reader
+Author: Evgeny Pogrebnyak
+Author-email: e.pogrebnyak@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: httpx (>=0.27,<0.28)
+Requires-Dist: iso3166 (>=2.1.1,<3.0.0)
+Requires-Dist: pandas (>=2.0,<3.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['weo']
+# weo-reader
 
-package_data = \
-{'': ['*']}
+[![PyPI](https://img.shields.io/pypi/v/weo)](https://pypi.org/project/weo/)
+[![pytest](https://github.com/epogrebnyak/weo-reader/workflows/pytest/badge.svg)](https://github.com/epogrebnyak/weo-reader/actions)
+[![Downloads](https://pepy.tech/badge/weo/week)](https://pepy.tech/project/weo/week)
 
-install_requires = \
-['httpx>=0.22,<0.24', 'iso3166>=2.0.2,<3.0.0', 'pandas>=1.3.5']
-
-setup_kwargs = {
-    'name': 'weo',
-    'version': '0.7.4',
-    'description': 'Python client to download IMF World Economic Outlook (WEO) dataset as pandas dataframes.',
-    'long_description': '# weo-reader\n\n[![PyPI](https://img.shields.io/pypi/v/weo)](https://pypi.org/project/weo/)\n[![pytest](https://github.com/epogrebnyak/weo-reader/workflows/pytest/badge.svg)](https://github.com/epogrebnyak/weo-reader/actions)\n[![Downloads](https://pepy.tech/badge/weo/week)](https://pepy.tech/project/weo/week)\n\n[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Dvl1N3c9uRUEulm-Kto9zqW_VCj0YtzV)\n[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/epogrebnyak/weo-reader)\n\n\nThis is a Python client to download [IMF World Economic Outlook Report][weo] dataset as [pandas](https://pandas.pydata.org/) dataframes by release dates. You can explore:\n\n- single country macroeconomic data and forecast,\n- macro variables across countries for a given year,\n- country-year panel for single macro variable.\n\n## Dataset releases (vintages)\n\nDataset releases (vintages) are available back to 2007, the reported data goes back to 1980, forecast is three years ahead.\n\n| Release          | Date         |\n| :--------------- | :-----------:|\n| Latest confirmed | April 2022   |\n| First            | October 2007 |\n\nConfirmed release is tested to be processed with `weo`.\nUsually, if something breaks in a new release users raise an [issue here](https://github.com/epogrebnyak/weo-reader/issues).\n\n[weo]: https://www.imf.org/en/Publications/WEO\n\n![изображение](https://user-images.githubusercontent.com/9265326/103473902-8c64da00-4dae-11eb-957c-4737f56abdce.png)\n\n## Install\n\nThe program is tested to run with Python 3.7.13 (as in Google Colab) and higher.\n\nTo install:\n\n```\npip install weo\n```\n\nLatest version:\n\n```\npip install git+https://github.com/epogrebnyak/weo-reader.git\n```\n\n## First glance\n\nGet US inflation forecast from April 2022 semiannual WEO release.\n\n```python\nfrom weo import download, WEO\n\npath, url = download(2022, 1)\n# weo_2022_1.csv 18.8Mb\n# Downloaded 2022-Apr WEO dataset\n\ndf_cpi = WEO(path).inflation()\nprint(df_cpi.USA.tail(8))\n#         USA\n# 2020  1.549\n# 2021  7.426\n# 2022  5.329\n# 2023  2.337\n# 2024  2.096\n# 2025  1.970\n# 2026  1.983\n# 2027  2.017\n```\n\n## Step 1. Download data\n\nSave data from IMF web site as local file. Specify year\nand release:\n\n```python\nimport weo\n\nweo.download(year=2020, release="Oct", filename="weo.csv")\n```\n\n- You can access WEO releases starting October 2007 with this client.\n- WEO is normally released in April and October, one exception is September 2011.\n- Release is referenced by:\n  - number `1` or `2`;\n  - month `\'Apr\'` or `\'Oct\'`, and `\'Sep\'` in 2011.\n\nYour can list all years and releases available for download with `weo.all_releases()`.\nCombine to create local dataset of WEO vintages from 2007 to present:\n\n```python\nimport pathlib\nimport weo\n\n# create folder\npathlib.Path("weo_data").mkdir(parents=False, exist_ok=True)\n\n# download all releases\nfor (year, release) in weo.all_releases():\n  weo.download(year, release, directory="weo_data")\n```\n\n## Step 2. Inspect data\n\nUse `WEO` class to view and extract data. `WEO` is a wrapper around a pandas dataframe that ensures proper data import and easier access and slicing of data across time-country-variable dimensions.\n\nTry code below:\n\n```python\nfrom weo import WEO\n\nw = WEO("weo.csv")\n```\n\nWhat variables and measurements are inside?\n\n```python\n# variable listing\nw.variables()\n\n# units\nw.units()\nw.units("Gross domestic product, current prices")\n\n# variable codes\nw.codes\nw.from_code("LUR")\n\n# countries\nw.countries("United")      # Dataframe with United Arab Emirates, United Kingdom\n                           # and United States\nw.iso_code3("Netherlands") # \'NLD\'\n```\n\nThe dataset is year-country-variable-value cube, you can fix any dimension to get a table.\n\n```python\n\nw.get("General government gross debt", "Percent of GDP")\nw.getc("NGDP_RPCH")\nw.country("DEU")\nw.fix_year(1994)\n```\n\nPlot a chart with the projected 12 largest economies in 2024 (current prices):\n\n```python\n(w.gdp_usd(2024)\n  .dropna()\n  .sort_values()\n  .tail(12)\n  .plot\n  .barh(title="GDP by country, USD billion (2024)")\n)\n```\n\nGet GDP per capita data from 2000 to 2020:\n\n```python\nw.gdp_pc_usd(start_year=2000, end_year=2020)\n```\n\n## Code documentation\n\n`weo` package documentation is [here](https://epogrebnyak.github.io/weo-reader/).\n\n## Alternative data sources\n\n1\\. If you need the latest data as time series and not the vintages of WEO releases, and you know variables that you are looking for, DBnomics is a good choice:\n\n- <https://db.nomics.world/IMF/WEO>\n- <https://db.nomics.world/IMF/WEOAGG>\n\nExample:\n\n```python\nfrom dbnomics import fetch_series_by_api_link\nts1 = fetch_series_by_api_link("https://api.db.nomics.world/v22/"\n                               "series/IMF/WEO:latest/DEU.PCPI"\n                               "?observations=1")\n```\n\n[![dbnomics](https://user-images.githubusercontent.com/9265326/168478113-00fb4d3f-11c3-43ad-9c19-28e2204f89c1.png)](https://db.nomics.world/IMF/WEO:2021-10/DEU.PCPI.idx)\n\nMore on DBnomics:\n\n- [DBnomics Web API](https://db.nomics.world/docs/web-api/)\n- [Introduction to DBnomics in Python](https://notes.quantecon.org/submission/5bd32515f966080015bafbcd)\n\n2\\. Similar dataset, not updated since 2018, but with earlier years than `weo-reader`:\nhttps://github.com/datasets/imf-weo\n\n## Development notes\n\n- You can download the WEO file in command line with `curl` command:\n\n```\ncurl -o weo.csv https://www.imf.org/-/media/Files/Publications/WEO/WEO-Database/2020/02/WEOOct2020all.xls\n```\n\n- `WEOOct2020all.xls` from the web site is really a CSV file, not an Excel file.\n- There is an update of GDP figures in [June 2020](jun2020), but the file structure is incompatible with regular releases.\n- Prior to 2020 the URL structure was similar to `https://www.imf.org/external/pubs/ft/weo/2019/02/weodata/WEOOct2019all.xls`\n\n[jun2020]: https://www.imf.org/en/Publications/WEO/Issues/2020/06/24/WEOUpdateJune2020\n',
-    'author': 'Evgeny Pogrebnyak',
-    'author_email': 'e.pogrebnyak@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/epogrebnyak/weo-reader',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.13',
-}
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Dvl1N3c9uRUEulm-Kto9zqW_VCj0YtzV)
+[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/epogrebnyak/weo-reader)
 
 
-setup(**setup_kwargs)
+This is a Python client to download [IMF World Economic Outlook Report][weo] dataset as [pandas](https://pandas.pydata.org/) dataframes by release dates. You can explore:
+
+- single country macroeconomic data and forecast,
+- macro variables across countries for a given year,
+- country-year panel for single macro variable.
+
+## Dataset releases (vintages)
+
+Dataset releases (vintages) are available back to 2007, the reported data goes back to 1980, forecast is three years ahead.
+
+| Release          | Date         |
+| :--------------- | :-----------:|
+| Latest confirmed | April 2024   |
+| First            | October 2007 |
+
+Confirmed release is tested to be processed with `weo`.
+Usually, if something breaks in a new release users raise an [issue here](https://github.com/epogrebnyak/weo-reader/issues).
+
+[weo]: https://www.imf.org/en/Publications/WEO
+
+![изображение](https://user-images.githubusercontent.com/9265326/103473902-8c64da00-4dae-11eb-957c-4737f56abdce.png)
+
+## Install
+
+The program is tested to run with Python 3.8 or higher.
+
+To install:
+
+```
+pip install weo
+```
+
+Latest version:
+
+```
+pip install git+https://github.com/epogrebnyak/weo-reader.git
+```
+
+## First glance
+
+Get US inflation forecast from April 2022 semiannual WEO release.
+
+```python
+from weo import download, WEO
+
+path, url = download(2022, 1)
+# weo_2022_1.csv 18.8Mb
+# Downloaded 2022-Apr WEO dataset
+
+df_cpi = WEO(path).inflation()
+print(df_cpi.USA.tail(8))
+#         USA
+# 2020  1.549
+# 2021  7.426
+# 2022  5.329
+# 2023  2.337
+# 2024  2.096
+# 2025  1.970
+# 2026  1.983
+# 2027  2.017
+```
+
+## Step 1. Download data
+
+Save data from IMF web site as local file. Specify year
+and release:
+
+```python
+import weo
+
+weo.download(year=2020, release="Oct", filename="weo.csv")
+```
+
+- You can access WEO releases starting October 2007 with this client.
+- WEO is normally released in April and October, one exception is September 2011.
+- Release is referenced by:
+  - number `1` or `2`;
+  - month `'Apr'` or `'Oct'`, and `'Sep'` in 2011.
+
+Your can list all years and releases available for download with `weo.all_releases()`.
+Combine to create local dataset of WEO vintages from 2007 to present:
+
+```python
+import pathlib
+import weo
+
+# create folder
+pathlib.Path("weo_data").mkdir(parents=False, exist_ok=True)
+
+# download all releases
+for (year, release) in weo.all_releases():
+  weo.download(year, release, directory="weo_data")
+```
+
+## Step 2. Inspect data
+
+Use `WEO` class to view and extract data. `WEO` is a wrapper around a pandas dataframe that ensures proper data import and easier access and slicing of data across time-country-variable dimensions.
+
+Try code below:
+
+```python
+from weo import WEO
+
+w = WEO("weo.csv")
+```
+
+What variables and measurements are inside?
+
+```python
+# variable listing
+w.variables()
+
+# units
+w.units()
+w.units("Gross domestic product, current prices")
+
+# variable codes
+w.codes
+w.from_code("LUR")
+
+# countries
+w.countries("United")      # Dataframe with United Arab Emirates, United Kingdom
+                           # and United States
+w.iso_code3("Netherlands") # 'NLD'
+```
+
+The dataset is year-country-variable-value cube, you can fix any dimension to get a table.
+
+```python
+
+w.get("General government gross debt", "Percent of GDP")
+w.getc("NGDP_RPCH")
+w.country("DEU")
+w.fix_year(1994)
+```
+
+Plot a chart with the projected 12 largest economies in 2024 (current prices):
+
+```python
+(w.gdp_usd(2024)
+  .dropna()
+  .sort_values()
+  .tail(12)
+  .plot
+  .barh(title="GDP by country, USD billion (2024)")
+)
+```
+
+Get GDP per capita data from 2000 to 2020:
+
+```python
+w.gdp_pc_usd(start_year=2000, end_year=2020)
+```
+
+## Code documentation
+
+`weo` package documentation is [here](https://epogrebnyak.github.io/weo-reader/).
+
+## Alternative data sources
+
+1\. If you need the latest data as time series and not the vintages of WEO releases, and you know variables that you are looking for, DBnomics is a good choice:
+
+- <https://db.nomics.world/IMF/WEO>
+- <https://db.nomics.world/IMF/WEOAGG>
+
+Example:
+
+```python
+from dbnomics import fetch_series_by_api_link
+ts1 = fetch_series_by_api_link("https://api.db.nomics.world/v22/"
+                               "series/IMF/WEO:latest/DEU.PCPI"
+                               "?observations=1")
+```
+
+[![dbnomics](https://user-images.githubusercontent.com/9265326/168478113-00fb4d3f-11c3-43ad-9c19-28e2204f89c1.png)](https://db.nomics.world/IMF/WEO:2021-10/DEU.PCPI.idx)
+
+More on DBnomics:
+
+- [DBnomics Web API](https://db.nomics.world/docs/web-api/)
+- [Introduction to DBnomics in Python](https://notes.quantecon.org/submission/5bd32515f966080015bafbcd)
+
+2\. Similar dataset, not updated since 2018, but with earlier years than `weo-reader`:
+https://github.com/datasets/imf-weo
+
+## Development notes
+
+- You can download the WEO file in command line with `curl` command:
+
+```
+curl -o weo.csv https://www.imf.org/-/media/Files/Publications/WEO/WEO-Database/2020/02/WEOOct2020all.xls
+```
+
+- `WEOOct2020all.xls` from the web site is really a CSV file, not an Excel file.
+- There is an update of GDP figures in [June 2020](jun2020), but the file structure is incompatible with regular releases.
+- Prior to 2020 the URL structure was similar to `https://www.imf.org/external/pubs/ft/weo/2019/02/weodata/WEOOct2019all.xls`
+
+[jun2020]: https://www.imf.org/en/Publications/WEO/Issues/2020/06/24/WEOUpdateJune2020
+
```


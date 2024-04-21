# Comparing `tmp/pyield-0.7.3.tar.gz` & `tmp/pyield-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyield-0.7.3.tar", last modified: Fri Apr 19 11:13:54 2024, max compression
+gzip compressed data, was "pyield-0.7.4.tar", last modified: Sun Apr 21 13:58:29 2024, max compression
```

## Comparing `pyield-0.7.3.tar` & `pyield-0.7.4.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.7.3/LICENSE
--rw-r--r--   0        0        0     5177 2024-04-19 11:12:40.008362 pyield-0.7.3/README.md
--rw-r--r--   0        0        0       22 2024-04-19 11:12:40.008362 pyield-0.7.3/pyield/__about__.py
--rw-r--r--   0        0        0      380 2024-04-14 09:19:55.868897 pyield-0.7.3/pyield/__init__.py
--rw-r--r--   0        0        0    13136 2024-04-13 12:39:44.026704 pyield-0.7.3/pyield/bday.py
--rw-r--r--   0        0        0     3625 2024-04-19 11:12:40.008362 pyield-0.7.3/pyield/data_access.py
--rw-r--r--   0        0        0     1276 2024-04-17 08:50:12.086620 pyield-0.7.3/pyield/data_analysis.py
--rw-r--r--   0        0        0      289 2024-04-19 11:12:40.008362 pyield-0.7.3/pyield/futures/__init__.py
--rw-r--r--   0        0        0     7483 2024-04-19 11:12:40.009362 pyield-0.7.3/pyield/futures/common.py
--rw-r--r--   0        0        0     5810 2024-04-19 11:12:40.009362 pyield-0.7.3/pyield/futures/ddi.py
--rw-r--r--   0        0        0     7272 2024-04-19 11:12:40.009362 pyield-0.7.3/pyield/futures/di.py
--rw-r--r--   0        0        0    11499 2024-04-19 11:12:40.009362 pyield-0.7.3/pyield/futures/di_xml.py
--rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.7.3/pyield/holidays/__init__.py
--rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.7.3/pyield/holidays/br_holidays_new.txt
--rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.7.3/pyield/holidays/br_holidays_old.txt
--rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.7.3/pyield/holidays/core.py
--rw-r--r--   0        0        0     2273 2024-04-14 11:04:04.016185 pyield-0.7.3/pyield/indicators.py
--rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.7.3/pyield/py.typed
--rw-r--r--   0        0        0     6622 2024-04-19 11:12:40.009362 pyield-0.7.3/pyield/treasuries.py
--rw-r--r--   0        0        0     2142 2024-04-19 11:12:40.009362 pyield-0.7.3/pyield/utils.py
--rw-r--r--   0        0        0     1165 2024-04-19 11:13:54.665452 pyield-0.7.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.7.3/tests/__init__.py
--rw-r--r--   0        0        0     1114 2024-04-16 12:01:55.676922 pyield-0.7.3/tests/test_bday.py
--rw-r--r--   0        0        0     2581 2024-04-19 11:12:40.009362 pyield-0.7.3/tests/test_futures.py
--rw-r--r--   0        0        0     7194 1970-01-01 00:00:00.000000 pyield-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.7.4/LICENSE
+-rw-r--r--   0        0        0     5177 2024-04-19 11:12:40.008362 pyield-0.7.4/README.md
+-rw-r--r--   0        0        0       22 2024-04-20 10:57:56.123762 pyield-0.7.4/pyield/__about__.py
+-rw-r--r--   0        0        0      422 2024-04-20 13:36:59.541311 pyield-0.7.4/pyield/__init__.py
+-rw-r--r--   0        0        0    13136 2024-04-13 12:39:44.026704 pyield-0.7.4/pyield/bday.py
+-rw-r--r--   0        0        0     6073 2024-04-21 13:45:50.722682 pyield-0.7.4/pyield/data_access.py
+-rw-r--r--   0        0        0     1276 2024-04-17 08:50:12.086620 pyield-0.7.4/pyield/data_analysis.py
+-rw-r--r--   0        0        0      333 2024-04-21 13:45:50.722682 pyield-0.7.4/pyield/futures/__init__.py
+-rw-r--r--   0        0        0     7534 2024-04-21 13:44:00.419409 pyield-0.7.4/pyield/futures/common.py
+-rw-r--r--   0        0        0     5817 2024-04-21 13:45:50.732682 pyield-0.7.4/pyield/futures/ddi.py
+-rw-r--r--   0        0        0     7159 2024-04-21 13:45:25.305158 pyield-0.7.4/pyield/futures/di.py
+-rw-r--r--   0        0        0    11499 2024-04-19 11:12:40.009362 pyield-0.7.4/pyield/futures/di_xml.py
+-rw-r--r--   0        0        0     2990 2024-04-21 13:54:31.947419 pyield-0.7.4/pyield/futures/frc.py
+-rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.7.4/pyield/holidays/__init__.py
+-rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.7.4/pyield/holidays/br_holidays_new.txt
+-rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.7.4/pyield/holidays/br_holidays_old.txt
+-rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.7.4/pyield/holidays/core.py
+-rw-r--r--   0        0        0     4268 2024-04-21 10:44:43.260419 pyield-0.7.4/pyield/indicators.py
+-rw-r--r--   0        0        0     3395 2024-04-21 10:47:45.706989 pyield-0.7.4/pyield/projections.py
+-rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.7.4/pyield/py.typed
+-rw-r--r--   0        0        0     6617 2024-04-21 13:41:53.731824 pyield-0.7.4/pyield/treasuries.py
+-rw-r--r--   0        0        0     2190 2024-04-20 08:17:03.148377 pyield-0.7.4/pyield/utils.py
+-rw-r--r--   0        0        0     1195 2024-04-21 13:58:29.781319 pyield-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.7.4/tests/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-16 12:01:55.676922 pyield-0.7.4/tests/test_bday.py
+-rw-r--r--   0        0        0     2566 2024-04-21 13:41:53.732824 pyield-0.7.4/tests/test_futures.py
+-rw-r--r--   0        0        0     7232 1970-01-01 00:00:00.000000 pyield-0.7.4/PKG-INFO
```

### Comparing `pyield-0.7.3/LICENSE` & `pyield-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyield-0.7.3/README.md` & `pyield-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pyield-0.7.3/pyield/bday.py` & `pyield-0.7.4/pyield/bday.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.3/pyield/data_access.py` & `pyield-0.7.4/pyield/data_access.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
 
 from . import futures as ft
 from . import indicators as it
+from . import projections as pr
 from . import treasuries as tr
 from .utils import _normalize_date
 
 
 def fetch_asset(
     asset_code: str,
     reference_date: str | pd.Timestamp | None = None,
@@ -18,14 +19,15 @@
         asset_code (str): The asset code identifying the type of financial asset.
         Supported options:
             - "TRB": Treasury bonds (indicative rates from ANBIMA).
             - "LTN", "LFT", "NTN-F", "NTN-B": Specific types of Brazilian treasury bonds
                   (indicative rates from ANBIMA).
             - "DI1": One-day Interbank Deposit Futures (Futuro de DI) from B3.
             - "DDI": DI x U.S. Dollar Spread Futures (Futuro de Cupom Cambial) from B3.
+            - "FRC": Forward Rate Agreement (FRA) from B3.
         reference_date (str | pd.Timestamp | None): The reference date for which data is
             fetched. Defaults to the last business day if None.
         **kwargs: Additional keyword arguments, specifically:
             - return_raw (bool): Whether to return raw data without processing. Defaults
               to False.
 
     Returns:
@@ -46,50 +48,101 @@
     elif asset_code.lower() in ["ltn", "lft", "ntn-f", "ntn-b"]:
         df = tr.fetch_bonds(reference_date=normalized_date)
         return df.query(f"BondType == '{asset_code.upper()}'")
 
     elif asset_code.lower() == "di1":
         today = pd.Timestamp.today().normalize()
         if normalized_date == today:
-            return ft.fetch_last_di_data()
+            return ft.fetch_last_di()
         else:
-            return ft.fetch_past_di_data(
-                trade_date=normalized_date, return_raw=return_raw
-            )
+            return ft.fetch_past_di(trade_date=normalized_date, return_raw=return_raw)
     elif asset_code.lower() == "ddi":
-        return ft.fetch_ddi(trade_date=normalized_date, return_raw=return_raw)
+        return ft.fetch_past_ddi(trade_date=normalized_date, return_raw=return_raw)
+    elif asset_code.lower() == "frc":
+        return ft.fetch_past_frc(trade_date=normalized_date, return_raw=return_raw)
     else:
         raise ValueError("Asset type not supported.")
 
 
 def fetch_indicator(
     indicator_code: str,
     reference_date: str | pd.Timestamp | None = None,
 ) -> float | None:
     """
     Fetches data for a specified economic indicator and reference date.
 
     Args:
         indicator_code (str): The code for the economic indicator. Supported options:
-            - "SELIC": SELIC target rate from the Central Bank of Brazil.
-            - "IPCA": IPCA monthly inflation rate from IBGE.
-        reference_date (str | pd.Timestamp | None): The reference date for which data is
-            fetched. Defaults to the last business day if None.
+            - "SELIC": SELIC target rate from the Central Bank of Brazil, expressed as
+              an annual rate (p.a.).
+            - "DI": Interbank Deposit rate (DI) from B3 expressed as a daily rate,
+              calculated on a daily basis and expressed per diem (p.d.).
+            - "IPCA": IPCA monthly inflation rate from IBGE, expressed per month (p.m.).
+            - "VNA_LFT": VNA (Valor Nominal Atualizado) of LFT (Letra Financeira do
+              Tesouro), which reflects updated nominal values for these bonds.
+        - reference_date (str | pd.Timestamp | None): The reference date for which data
+          is fetched. Defaults to the last business day if None.
 
     Returns:
-        pd.Series: A Series containing the fetched data for the specified indicator.
+        float | None: The value of the specified economic indicator for the reference
+        date. Returns None if data is not found.
 
     Raises:
         ValueError: If the indicator code is not recognized or supported.
 
     Examples:
         >>> fetch_indicator('SELIC', '2023-04-01')
-        >>> fetch_indicator('IPCA', '2023-04-01')
+        0.1075  # Indicates a SELIC target rate of 10.75% p.a.
+        >>> fetch_indicator('IPCA', '2023-03-10')
+        0.0016  # Indicates an IPCA monthly rate of 0.16% p.m.
+        >>> fetch_indicator('DI', '2023-04-17')
+        0.00040168  # Indicates a DI daily rate of 0.02% p.d.
     """
     normalized_date = _normalize_date(reference_date)
 
     if indicator_code.lower() == "selic":
         return it.fetch_selic_target(reference_date=normalized_date)
     elif indicator_code.lower() == "ipca":
         return it.fetch_ipca_mr(reference_date=normalized_date)
+    elif indicator_code.lower() == "di":
+        return it.fetch_di(reference_date=normalized_date)
+    elif indicator_code.lower() == "vna_lft":
+        return it.fetch_vna_selic(reference_date=normalized_date)
     else:
         raise ValueError("Indicator type not supported.")
+
+
+def fetch_projection(projection_code: str) -> dict:
+    """
+    Fetches a financial projection for a specified code and reference date.
+
+    Args:
+        projection_code (str): The code for the financial projection. Supported options:
+            - "IPCA_CM": IPCA projection for the current month from ANBIMA.
+
+    Returns:
+        IndicatorProjection: An instance of IndicatorProjection containing:
+            - last_updated (pd.Timestamp): The datetime when the projection was last
+              updated.
+            - reference_month_ts (pd.Timestamp): The month to which the projection
+              applies.
+            - reference_month_br (str): The formatted month as a string formatted using
+              the pt_BR locale.
+            - projected_value (float): The projected indicator value.
+
+    Raises:
+        ValueError: If the projection code is not recognized or supported.
+
+    Examples:
+        >>> fetch_projection('IPCA_CM')
+        IndicatorProjection(
+            last_updated=pd.Timestamp('2024-04-19 18:55:00'),
+            reference_month_ts=pd.Timestamp('2024-04-01 00:00:00'),
+            reference_month_br='ABR/2024',
+            projected_value=0.35
+        )
+    """
+
+    if projection_code.lower() == "ipca_cm":
+        return pr.fetch_current_month_ipca_projection()
+    else:
+        raise ValueError("Projection type not supported.")
```

### Comparing `pyield-0.7.3/pyield/data_analysis.py` & `pyield-0.7.4/pyield/data_analysis.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.3/pyield/futures/common.py` & `pyield-0.7.4/pyield/futures/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         # Must use old holiday list, since this contract code was used until 2006.
         return bday.offset_bdays(expiration_date, offset=0, holiday_list="old")
 
     except (KeyError, ValueError):
         return pd.NaT  # type: ignore
 
 
-def fetch_past_data(asset_code: str, trade_date: pd.Timestamp) -> pd.DataFrame:
+def fetch_past_raw_df(asset_code: str, trade_date: pd.Timestamp) -> pd.DataFrame:
     """
     Fetch the historical futures data from B3 for a specific trade date.
 
     Args:
         trade_date (pd.Timestamp): The trade date for which the data should be fetched.
 
     Returns:
@@ -166,20 +166,21 @@
     # Remove columns with all NaN values
     df = df.dropna(axis=1, how="all")
 
     # Force "VAR. PTOS." to be string, since it can also be read as float
     df["VAR. PTOS."] = df["VAR. PTOS."].astype(pd.StringDtype())
 
     # Force "AJUSTE CORRIG. (4)" to be float, since it can be also read as int
-    df["AJUSTE CORRIG. (4)"] = df["AJUSTE CORRIG. (4)"].astype(pd.Float64Dtype())
+    if "AJUSTE CORRIG. (4)" in df.columns:
+        df["AJUSTE CORRIG. (4)"] = df["AJUSTE CORRIG. (4)"].astype(pd.Float64Dtype())
 
     return df
 
 
-def fetch_last_data(future_code: str) -> pd.DataFrame:
+def fetch_last_raw_df(future_code: str) -> pd.DataFrame:
     """
     Fetch the latest data for a given future code from B3 derivatives quotation API.
 
     Args:
     future_code (str): The future code to fetch data for.
 
     Returns:
```

### Comparing `pyield-0.7.3/pyield/futures/ddi.py` & `pyield-0.7.4/pyield/futures/ddi.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         "LastAskRate",
         "LastBidRate",
         "SettlementRate",
     ]
     return df[ordered_cols]
 
 
-def fetch_ddi(trade_date: pd.Timestamp, return_raw: bool = False) -> pd.DataFrame:
+def fetch_past_ddi(trade_date: pd.Timestamp, return_raw: bool = False) -> pd.DataFrame:
     """
     Fetchs the DDI futures data for a given date from B3.
 
     This function fetches and processes the DI futures data from B3 for a specific
     trade date. It's the primary external interface for accessing DI data.
 
     Args:
@@ -168,11 +168,11 @@
         >>> from pyield.futures import di
         >>> di.fetch_ddi(pd.Timestamp("2021-01-04"))
 
     Notes:
         - DaysToExpiration: number of business days to ExpirationDate.
         - OpenContracts: number of open contracts at the start of the trading day.
     """
-    df_raw = common.fetch_past_data(asset_code="DDI", trade_date=trade_date)
+    df_raw = common.fetch_past_raw_df(asset_code="DDI", trade_date=trade_date)
     if return_raw:
         return df_raw
     return _process_raw_df(df_raw, trade_date)
```

### Comparing `pyield-0.7.3/pyield/futures/di.py` & `pyield-0.7.4/pyield/futures/di.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     # Invert low and high prices
     df["MinRate"], df["MaxRate"] = df["MaxRate"], df["MinRate"]
 
     return df
 
 
-def _process_past_data(df: pd.DataFrame, trade_date: pd.Timestamp) -> pd.DataFrame:
+def _process_past_raw_df(df: pd.DataFrame, trade_date: pd.Timestamp) -> pd.DataFrame:
     """
     Internal function to process and transform raw DI futures data.
 
     Args:
         df (pd.DataFrame): the raw DI DataFrame.
         trade_date: a datetime-like object representing the trade date.
 
@@ -147,15 +147,15 @@
         "CloseAskRate",
         "CloseBidRate",
         "CloseRate",
     ]
     return df[ordered_cols]
 
 
-def _process_last_di_data(raw_df: pd.DataFrame) -> pd.DataFrame:
+def _process_last_raw_di_df(raw_df: pd.DataFrame) -> pd.DataFrame:
     df = raw_df.copy()
 
     # Columns to be renamed
     rename_columns = {
         "TradeTimestamp": "TradeTimestamp",
         "symb": "TickerSymbol",
         "mtrtyCode": "ExpirationDate",
@@ -184,47 +184,41 @@
     rate_cols = [col for col in df.columns if "Rate" in col]
     df[rate_cols] = df[rate_cols] / 100
 
     # Reorder columns based on the order of the dictionary
     return df[rename_columns.values()]
 
 
-def fetch_last_di_data() -> pd.DataFrame:
+def fetch_last_di() -> pd.DataFrame:
     """
     Fetch the latest DI futures data from B3.
 
     Returns:
         pd.DataFrame: A Pandas pd.DataFrame containing the latest DI futures data.
     """
-    raw_df = common.fetch_last_data(future_code="DI1")
-    return _process_last_di_data(raw_df)
+    raw_df = common.fetch_last_raw_df(future_code="DI1")
+    return _process_last_raw_di_df(raw_df)
 
 
-def fetch_past_di_data(
-    trade_date: pd.Timestamp, return_raw: bool = False
-) -> pd.DataFrame:
+def fetch_past_di(trade_date: pd.Timestamp, return_raw: bool = False) -> pd.DataFrame:
     """
     Fetchs the DI futures data for a given date from B3.
 
     This function fetches and processes the DI futures data from B3 for a specific
     trade date. It's the primary external interface for accessing DI data.
 
     Args:
         trade_date (pd.Timestamp): The trade date to fetch the DI futures data.
         raw (bool): If True, returns the raw data as a Pandas pd.DataFrame.
             Defaults to False.
 
     Returns:
         pd.DataFrame: A Pandas pd.DataFrame containing processed DI futures data.
 
-    Examples:
-        >>> from pyield.futures import di
-        >>> di.fetch_di(pd.Timestamp("2021-01-04"))
-
     Notes:
         - BDaysToExp: number of business days to ExpirationDate.
         - OpenContracts: number of open contracts at the start of the trading day.
     """
-    df_raw = common.fetch_past_data(asset_code="DI1", trade_date=trade_date)
+    df_raw = common.fetch_past_raw_df(asset_code="DI1", trade_date=trade_date)
     if return_raw:
         return df_raw
-    return _process_past_data(df_raw, trade_date)
+    return _process_past_raw_df(df_raw, trade_date)
```

### Comparing `pyield-0.7.3/pyield/futures/di_xml.py` & `pyield-0.7.4/pyield/futures/di_xml.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.3/pyield/holidays/br_holidays_new.txt` & `pyield-0.7.4/pyield/holidays/br_holidays_new.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.7.3/pyield/holidays/br_holidays_old.txt` & `pyield-0.7.4/pyield/holidays/br_holidays_old.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.7.3/pyield/holidays/core.py` & `pyield-0.7.4/pyield/holidays/core.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.3/pyield/treasuries.py` & `pyield-0.7.4/pyield/treasuries.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
     Returns:
         pd.DataFrame: A DataFrame containing the bond type, reference date, maturity
             date, and the calculated DI spread in basis points. The data is sorted by
             bond type and maturity date.
     """
     # Fetch DI rates and adjust the maturity date format for compatibility
-    df_di = ft.fetch_past_di_data(reference_date)[["ExpirationDate", "SettlementRate"]]
+    df_di = ft.fetch_past_di(reference_date)[["ExpirationDate", "SettlementRate"]]
 
     # Renaming the columns to match the ANBIMA structure
     df_di.rename(columns={"ExpirationDate": "MaturityDate"}, inplace=True)
 
     # Adjusting maturity date to match bond data format
     df_di["MaturityDate"] = df_di["MaturityDate"].dt.to_period("M").dt.to_timestamp()
```

### Comparing `pyield-0.7.3/pyield/utils.py` & `pyield-0.7.4/pyield/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 
 from . import bday
 
 
-def _normalize_date(reference_date: str | pd.Timestamp | None = None) -> pd.Timestamp:
+def _normalize_date(input_date: str | pd.Timestamp | None = None) -> pd.Timestamp:
     """
     Normalizes the given date to ensure it is a past business day at midnight. If no
     date is provided, it defaults to the last business day.
 
     Args:
         reference_date (str | pd.Timestamp | None): The date to normalize. Can be a
         string, pandas Timestamp or None. If None, it defaults to the last business day.
@@ -27,29 +27,29 @@
         - Business day calculations consider local market holidays.
 
     Examples:
         >>> _normalize_date('2023-04-01')
         >>> _normalize_date(pd.Timestamp('2023-04-01 15:30'))
         >>> _normalize_date()
     """
-    if isinstance(reference_date, str):
+    if isinstance(input_date, str):
         # Convert string date to Timestamp and normalize to midnight
-        normalized_date = pd.Timestamp(reference_date).normalize()
-    elif isinstance(reference_date, pd.Timestamp):
+        normalized_date = pd.Timestamp(input_date).normalize()
+    elif isinstance(input_date, pd.Timestamp):
         # Normalize Timestamp to midnight
-        normalized_date = reference_date.normalize()
-    elif reference_date is None:
+        normalized_date = input_date.normalize()
+    elif input_date is None:
         # If no date is provided, use the last available business day
         today = pd.Timestamp.today().normalize()
         normalized_date = bday.offset_bdays(dates=today, offset=0, roll="backward")
     else:
-        raise ValueError("Invalid date format.")
+        raise ValueError(f"Date format not recognized: {input_date}")
 
+    error_date = normalized_date.strftime("%d-%m-%Y")
     # Validate that the date is not in the future
     if normalized_date > pd.Timestamp.today().normalize():
-        raise ValueError("Reference date cannot be in the future.")
-
+        raise ValueError(f"Date {error_date} is in the future")
     # Validate that the date is a business day
     if not bday.is_bday(normalized_date):
-        raise ValueError("Reference date must be a business day.")
+        raise ValueError(f"Date {error_date} is not a business day")
 
     return normalized_date
```

### Comparing `pyield-0.7.3/pyproject.toml` & `pyield-0.7.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -25,17 +25,18 @@
 dependencies = [
     "requests",
     "pandas>=2.0.0",
     "numpy",
     "beautifulsoup4",
     "html5lib",
     "lxml",
+    "python-calamine>=0.2.0",
 ]
 dynamic = []
-version = "0.7.3"
+version = "0.7.4"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/crdcj/PYield"
```

### Comparing `pyield-0.7.3/tests/test_bday.py` & `pyield-0.7.4/tests/test_bday.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.3/tests/test_futures.py` & `pyield-0.7.4/tests/test_futures.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     settlement_rates = {
         "DI1N27": 0.09809,
         "DI1F33": 0.10368,
     }
 
     # 22-12-2023 is before the new holiday calendar
     test_date = pd.Timestamp("2023-12-22")
-    df = ft.fetch_past_di_data(trade_date=test_date)
+    df = ft.fetch_past_di(trade_date=test_date)
     tickers = list(settlement_rates.keys())  # noqa: F841
     result = df.query("TickerSymbol in @tickers")["SettlementRate"].to_list()
     assert result == list(settlement_rates.values())
 
 
 def test_settlement_rates_with_current_holiday_list():
     settlement_rates = {
@@ -64,17 +64,17 @@
         "DI1F27": 0.09683,
         "DI1N27": 0.09794,
         "DI1F29": 0.10042,
         "DI1F31": 0.10240,
         "DI1F33": 0.10331,
     }
     test_date = pd.Timestamp("2023-12-26")
-    df = ft.fetch_past_di_data(trade_date=test_date)
+    df = ft.fetch_past_di(trade_date=test_date)
     tickers = list(settlement_rates.keys())  # noqa: F841
     results = df.query("TickerSymbol in @tickers")["SettlementRate"].to_list()
     assert results == list(settlement_rates.values())
 
 
 def test_non_business_day():
     non_business_day = pd.Timestamp("2023-12-24")
     with pytest.raises(ValueError):
-        ft.fetch_past_di_data(trade_date=non_business_day)
+        ft.fetch_past_di(trade_date=non_business_day)
```

### Comparing `pyield-0.7.3/PKG-INFO` & `pyield-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PYield
-Version: 0.7.3
+Version: 0.7.4
 Summary: A Python library for analysis of fixed income instruments in Brazil
 Keywords: fixed-income, brazil, finance, analysis, bonds
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Carlos Carvalho
         
@@ -34,14 +34,15 @@
 Requires-Python: >=3.11
 Requires-Dist: requests
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: numpy
 Requires-Dist: beautifulsoup4
 Requires-Dist: html5lib
 Requires-Dist: lxml
+Requires-Dist: python-calamine>=0.2.0
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://img.shields.io/pypi/v/pyield.svg)](https://pypi.python.org/pypi/pyield)
 [![Made with Python](https://img.shields.io/badge/Python->=3.11-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/badge/License-MIT-blue)](#license)
 
 # PYield: Fixed Income Toolbox for Brazilian Markets
```


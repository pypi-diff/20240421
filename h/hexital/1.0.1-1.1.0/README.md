# Comparing `tmp/hexital-1.0.1.tar.gz` & `tmp/hexital-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexital-1.0.1.tar", max compression
+gzip compressed data, was "hexital-1.1.0.tar", max compression
```

## Comparing `hexital-1.0.1.tar` & `hexital-1.1.0.tar`

### file list

```diff
@@ -1,43 +1,50 @@
--rw-r--r--   0        0        0     4747 2024-04-08 21:11:50.558715 hexital-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1067 2024-04-08 21:11:50.558715 hexital-1.0.1/LICENSE
--rw-r--r--   0        0        0    12008 2024-04-08 21:11:50.558715 hexital-1.0.1/README.md
--rw-r--r--   0        0        0      249 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/__init__.py
--rw-r--r--   0        0        0      747 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/analysis/__init__.py
--rw-r--r--   0        0        0    12248 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/analysis/movement.py
--rw-r--r--   0        0        0     2538 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/analysis/patterns.py
--rw-r--r--   0        0        0     1378 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/analysis/utils.py
--rw-r--r--   0        0        0       80 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/candlesticks/__init__.py
--rw-r--r--   0        0        0      719 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/candlesticks/heikinashi.py
--rw-r--r--   0        0        0        0 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/core/__init__.py
--rw-r--r--   0        0        0     5984 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/core/candle.py
--rw-r--r--   0        0        0     7829 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/core/candle_manager.py
--rw-r--r--   0        0        0      958 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/core/candlestick_type.py
--rw-r--r--   0        0        0    15017 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/core/hexital.py
--rw-r--r--   0        0        0    13487 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/core/indicator.py
--rw-r--r--   0        0        0      839 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/exceptions.py
--rw-r--r--   0        0        0      761 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/__init__.py
--rw-r--r--   0        0        0     3970 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/adx.py
--rw-r--r--   0        0        0     2188 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/amorph.py
--rw-r--r--   0        0        0     1069 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/atr.py
--rw-r--r--   0        0        0     1295 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/ema.py
--rw-r--r--   0        0        0      426 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/hla.py
--rw-r--r--   0        0        0     1613 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/kc.py
--rw-r--r--   0        0        0     2860 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/macd.py
--rw-r--r--   0        0        0      818 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/obv.py
--rw-r--r--   0        0        0     1413 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/rma.py
--rw-r--r--   0        0        0      676 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/roc.py
--rw-r--r--   0        0        0     2589 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/rsi.py
--rw-r--r--   0        0        0     1168 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/sma.py
--rw-r--r--   0        0        0     2801 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/stoch.py
--rw-r--r--   0        0        0     2555 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/supertrend.py
--rw-r--r--   0        0        0      802 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/tr.py
--rw-r--r--   0        0        0     1452 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/vwap.py
--rw-r--r--   0        0        0      906 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/vwma.py
--rw-r--r--   0        0        0      962 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/indicators/wma.py
--rw-r--r--   0        0        0       89 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/utils/__init__.py
--rw-r--r--   0        0        0     2960 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/utils/candles.py
--rw-r--r--   0        0        0      585 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/utils/candlesticks.py
--rw-r--r--   0        0        0     1088 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/utils/indexing.py
--rw-r--r--   0        0        0     2792 2024-04-08 21:11:50.558715 hexital-1.0.1/hexital/utils/timeframe.py
--rw-r--r--   0        0        0     1503 2024-04-08 21:11:50.558715 hexital-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    13019 1970-01-01 00:00:00.000000 hexital-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5503 2024-04-21 16:16:53.425528 hexital-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1067 2024-04-21 16:16:53.425528 hexital-1.1.0/LICENSE
+-rw-r--r--   0        0        0    12974 2024-04-21 16:16:53.425528 hexital-1.1.0/README.md
+-rw-r--r--   0        0        0      249 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/__init__.py
+-rw-r--r--   0        0        0      835 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/analysis/__init__.py
+-rw-r--r--   0        0        0    12246 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/analysis/movement.py
+-rw-r--r--   0        0        0     3921 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/analysis/patterns.py
+-rw-r--r--   0        0        0     6102 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/analysis/utils.py
+-rw-r--r--   0        0        0       80 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/candlesticks/__init__.py
+-rw-r--r--   0        0        0      719 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/candlesticks/heikinashi.py
+-rw-r--r--   0        0        0        0 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/core/__init__.py
+-rw-r--r--   0        0        0     5636 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/core/candle.py
+-rw-r--r--   0        0        0     7806 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/core/candle_manager.py
+-rw-r--r--   0        0        0      958 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/core/candlestick_type.py
+-rw-r--r--   0        0        0     9691 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/core/hexital.py
+-rw-r--r--   0        0        0    12456 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/core/indicator.py
+-rw-r--r--   0        0        0      632 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/exceptions.py
+-rw-r--r--   0        0        0     1084 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/__init__.py
+-rw-r--r--   0        0        0     3476 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/adx.py
+-rw-r--r--   0        0        0     2188 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/amorph.py
+-rw-r--r--   0        0        0     1447 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/aroon.py
+-rw-r--r--   0        0        0     1049 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/atr.py
+-rw-r--r--   0        0        0     1307 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/bbands.py
+-rw-r--r--   0        0        0     1102 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/counter.py
+-rw-r--r--   0        0        0     1147 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/donchian.py
+-rw-r--r--   0        0        0     1295 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/ema.py
+-rw-r--r--   0        0        0      426 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/hla.py
+-rw-r--r--   0        0        0     1500 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/hma.py
+-rw-r--r--   0        0        0     1602 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/kc.py
+-rw-r--r--   0        0        0     2818 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/macd.py
+-rw-r--r--   0        0        0      818 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/obv.py
+-rw-r--r--   0        0        0     1413 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/rma.py
+-rw-r--r--   0        0        0      676 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/roc.py
+-rw-r--r--   0        0        0     2550 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/rsi.py
+-rw-r--r--   0        0        0     1168 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/sma.py
+-rw-r--r--   0        0        0     1672 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/indicators/stdev.py
+-rw-r--r--   0        0        0     2900 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/indicators/stoch.py
+-rw-r--r--   0        0        0     2366 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/indicators/supertrend.py
+-rw-r--r--   0        0        0      824 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/indicators/tr.py
+-rw-r--r--   0        0        0     2782 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/indicators/tsi.py
+-rw-r--r--   0        0        0     1363 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/indicators/vwap.py
+-rw-r--r--   0        0        0      906 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/indicators/vwma.py
+-rw-r--r--   0        0        0      962 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/indicators/wma.py
+-rw-r--r--   0        0        0       89 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/utils/__init__.py
+-rw-r--r--   0        0        0     2960 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/utils/candles.py
+-rw-r--r--   0        0        0      585 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/utils/candlesticks.py
+-rw-r--r--   0        0        0     1088 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/utils/indexing.py
+-rw-r--r--   0        0        0     2792 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/utils/timeframe.py
+-rw-r--r--   0        0        0     1534 2024-04-21 16:16:53.429529 hexital-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    13985 1970-01-01 00:00:00.000000 hexital-1.1.0/PKG-INFO
```

### Comparing `hexital-1.0.1/CHANGELOG.md` & `hexital-1.1.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,41 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 1.1.0 - 2024-04-21
+
+- Removed Movement/Patterns from Hexital/Indicator
+- Removed get_indicator from Hexital as indicator already exists
+- Renamed candles_all to get_candles
+- Updated prev_exists to accept optional Indicator to be more useful
+- Altered Indicator name reading, to avoid issue's such as "TR" in "ATR"
+- Changed several methods to properties in Candle (positive, realbody, etc)
+- Updated Candle to be more flexible with values
+- Corrected correlation_coefficient for unit testing
+- Added Indicators
+  - Counter
+  - Aroon (aroon)
+  - Donchian Channels (donchian)
+  - Hull Moving Average (HMA)
+  - True Strength Index (TSI)
+  - Standard Deviation (STDEV)
+  - Bollinger Bands (BBANDS)
+- Added Patterns
+  - Inverted Hammer
+  - Dojistar
+
 ## 1.0.1 - 2024-04-08
+
 - Fixed #12 Inaccurate verify_indicators method in Hexital
 
 ## 1.0.0 - 2024-02-11
+
 - Moving Into BETA
 - Added CandleManager
   - CandleManger replaces List[Candle] to manage Candles and controls CandlestickTypes, timeframes and lifespan
 - Added CandlestickType
   - CandlestickType modular parent to convert candlesticks to alt types,
   - E.G Auto convert candles to heikin-ashi
   - Can be added as str 'candlestick_type="ha"' for heikin-ashi
@@ -31,14 +55,15 @@
 - Fixed Hammer index pattern working correctly
 - Changed Sub/managed indicators to auto populate candles field
 - Changed 'as_list' property a method that can now take a nested indicator name
 - Removed read property
 - Renamed utils/candlesticks to utils/candles
 
 ## 0.4.0 - 2024-01-22
+
 - Cleaned up code and some potential Bugs ruff/pyright
 - Added movement Above/Below and updated others to use it
 - Updated collapse candle 'fill' to show essentially doji candle rather than copy prev
 - Added Patterns:
   - Hammer Candle
 - Added a TimeFrame Enum with common timeframes for easier usage
 - Renamed Pattern to Amorph and updated to only require either 'indicator' or 'analysis'
@@ -49,40 +74,43 @@
 - Fixed Supertrend Indicator
 - Fixed Timeframe bug with candles reference in indicator that use sub indicators
 - Fixed possible error in VWAP with no volumes traded
 - Fixed bug with nested Indicator returning None for valid 0 Value
 - Fixed purge not correctly purge sub and managed indicators
 
 ## 0.3.1 - 2023-10-09
+
 - Added candles_timerange to auto remove older than N candles
 - Added 'Settings' propety, to output Indicator in a dict format, that can be fed into back into Hexital
 - Updated Hexital to better take Pattern's as a dict input
 - Updated Hexital dict input to accept custom method Patterns
 - Fixed bug in Movement on to few candles
 - Fixed bug where no timeframe indicator wasnt creating new copy of candles
 - Fixed bug where collapsed timeframe candles will use first calculated indicator value
-  - Meaning 1 minute candle that only had first 10 seconds,  will never re-calculate for rest of the minute
+  - Meaning 1 minute candle that only had first 10 seconds, will never re-calculate for rest of the minute
 
 ## 0.3.0 - 2023-09-27
+
 - Added Patterns:
   - Doji Candle
 - Added append method to Indicator just like Hexital
 - Fixed bug where Hexital would alter indicator list
-- Fixed bug in _find_calc_index with no candles
+- Fixed bug in \_find_calc_index with no candles
 - Added Pattern Indicator, skeleton to run Any Patterns as a Indicator
   - E.G On all Candles automatically
 - Added support to generate Indicators on multiple timeframes at once
   - Allowing one set of candles to be used to generate higher timeframe indicators
   - E.G 1m candles can be used to generate 10m indicators simultaneously with 1m indicators
 
 ## 0.2.0 - 2023-09-05
+
 - Feature: Added timestamp (datetime) to Candle dataclass
 - Feature: Can convert Candle from list and dict
 - Feature: Can set timestamp(datetime) in lists/dict Candle conversion
-- Feature: Added _validate_fields method to Indicators
+- Feature: Added \_validate_fields method to Indicators
 - Added custom exceptions
 - More thorough unit testing
 - Updated Indicators accuracy to Truth source
 - Added private index property to Indicator allowing simpler method calls
   - self.reading_by_index(index, self.input_value) -> self.reading(self.input_value)
   - Multiple Method's renamed/argument re-ordered
 - Added Indicators:
@@ -93,13 +121,15 @@
   - RMA
   - ROC
   - STOCH
   - SuperTrend
   - VWAP
   - VMA
   - WMA
-  
+
 ## 0.1.1 - 2023-08-28
+
 - Nada
 
 ## 0.1.0 - 2023-08-27
+
 - Alpha release `hexital`
```

### Comparing `hexital-1.0.1/LICENSE` & `hexital-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hexital-1.0.1/README.md` & `hexital-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,103 +1,141 @@
 # Hexital - Incremental Technical Analysis Library
+
 [![license](https://img.shields.io/github/license/merlinr/hexital)](#license)
 [![Python Version](https://img.shields.io/pypi/pyversions/hexital?style=flat)](https://pypi.org/project/hexital/)
 [![PyPi Version](https://img.shields.io/pypi/v/hexital?style=flat)](https://pypi.org/project/hexital/)
 [![Package Status](https://img.shields.io/pypi/status/hexital?style=flat)](https://pypi.org/project/hexital/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/hexital?color=%2332c955)
+![GitHub Repo stars](https://img.shields.io/github/stars/MerlinR/Hexital?style=flat)
 [![Unit Tests - Master](https://github.com/MerlinR/Hexital/actions/workflows/unit_test.yaml/badge.svg?branch=master)](https://github.com/MerlinR/Hexital/actions/workflows/unit_test.yaml)
 [![Unit Tests - Dev](https://github.com/MerlinR/Hexital/actions/workflows/unit_test.yaml/badge.svg?branch=development)](https://github.com/MerlinR/Hexital/actions/workflows/unit_test.yaml)
 
 # `Beta`
-Note: Hexital has entered Beta mode, being all Major features are implemented and not expected to have drastic changes. Future changes would include bug fixes, QOL additions and implementation of new Indicators, Candlestick patterns, movements and Candlestick types.
+
+Note: Hexital is in Beta, all Major features are implemented and not expected to have drastic changes.
 
 # Hexital
-`Hexital` is a Python library implementing financial indicators for technical analysis. The distinctive feature of the library is its incremental computation of indicators which is designed to fit real-time applications or applications with iterative input in general.
 
-For most libraries such as [Pandas-TA](https://github.com/twopirllc/pandas-ta) which is fantastic for generating Indicators for a large set of data, it's incredibly slow when computing real-time/incremental data sets. The entire input vector is always used to calculate new values of indicators, which is a major cause of this speed issue. Despite the fact that these indicator values will remain unchanged and/or you don't want past data points to be changed by new data. `Hexital` resolves this by using an incremental approach, only calculating new/missing indicator value's, this implies it requires O(1) time to produce new indicator values in comparison to O(n) (or worse) required by other libraries.
+`Hexital` is a Python library designed for technical analysis in financial markets, offering a range of indicators commonly used in trading strategies. What sets Hexital apart is its innovative approach to computation, specifically tailored for real-time or iterative applications.
+
+While libraries like [Pandas-TA](https://github.com/twopirllc/pandas-ta) excel at generating indicators for large datasets, they often struggle with real-time or incremental data processing due to their reliance on recalculating the entire input vector. This inefficiency can significantly impact speed, as each new data point triggers a full recalculation of all indicators.
 
+`Hexital` addresses this issue by employing an incremental computation method. Rather than reevaluating all data points, it selectively computes only the new or missing indicator values. This optimized approach ensures that generating new indicator values requires constant time complexity O(1), a stark contrast to the linear time complexity (O(n)) or worse exhibited by other libraries.
+
+With Hexital, users can enjoy swift and efficient computation of indicators, making it ideal for applications requiring real-time analysis or iterative data processing.
 
 ## Features
 
 ### Indicators
-Hexital comes with a growing selection of available Indicators to compute. These can be used individually to calculate a single indicator, or used with the `Hexital` class to automatically compute multiple indicators with an incremental candle list; which is easily parsable.
+
+Hexital offers a diverse range of indicators for technical analysis. These can be utilized individually to compute a single indicator or, with the Hexital class, multiple indicators can be automatically calculated using an incremental candle list, which is easily parsed.
 
 ### Candlestick Patterns
-Hexital also supports detecting candle patterns, such as Doji, etc. This can be achieved easily by calling the Pattern function with the candles, or used automatically as an indicator where it would be computed alongside Indicators.
+
+Hexital supports the detection of candle patterns, such as Doji, among others. This functionality can be easily accessed by calling the Pattern function with the candle data, or it can be automatically computed alongside other indicators.
 
 ### Candlestick Types
-Hexital also has the feature to automatically convert Candlesticks from the standard type into alternative formats, such as 'Heikin-Ashi'. This will mean prior to generating indicators it will automatically convert the Candlesticks to the desired type and then calculate indicators on this new candlestick type. This works in conjunction with all other features.
+
+Hexital provides the capability to automatically convert candlesticks from the standard type into alternative formats, such as 'Heikin-Ashi'. Prior to generating indicators, candlesticks are automatically converted to the desired type, enabling indicator calculations on this new candlestick type. This feature seamlessly integrates with all other functionalities.
 
 ### Multi-Timeframes
-Hexital has a key feature of supporting indicator and pattern computation on multiple candle timeframes with a single set of candles. For instance an indicator can be given second candlesticks and can calculate EMA on 1m candlesticks or 10m candlesticks, the indicator will automatically merge these candles into the required timeframes and compute the indicator value. * Cant go down, for obv reasons.
 
-This can also be mixed within the `Hexital` class, allowing you to automatically compute a multiple incremental indictors and patterns of which consistent of multiple timeframes by appending a single candle of any timeframe. E.G By appending 1m candles  into `Hexital` you can automatically compute an RSI using the 5 minute candles and computing an EMA using the 10 minute candles, at the same time automatically while only adding 1m candlesticks.
+Hexital boasts a key feature of supporting indicator and pattern computation on multiple candle timeframes using a single set of candles. For example, an indicator can be applied to second candlesticks to calculate EMA on 1m or 10m candlesticks. The indicator automatically merges these candles into the required timeframes and computes the indicator value.
+
+This functionality can also be leveraged within the `Hexital` class, enabling the automatic computation of multiple incremental indicators and patterns across multiple timeframes by appending a single candle of any timeframe. For instance, by appending 1m candles into Hexital, you can automatically compute an RSI using 5-minute candles and an EMA using 10-minute candles, all while only adding 1m candlesticks.
 
 Example:
+
 ```python
 stratergy = Hexital("Test Stratergy", candlesticks_1m, [RSI(timeframe="T5"), EMA(timeframe=TimeFrame.MINUTE10)])
 ```
 
 ### Candlestick Movements
-Hexital also comes built with some candle utility methods, to easily take the candles list and detect movements such as Rising Candles, indicator Cross overs, etc, these are designed to be simple to make using the candles and common features easy,  many of these are also found in pine scripting. 
+
+Hexital includes built-in candle utility methods for detecting movements such as Rising Candles and indicator crossovers. These methods are designed to simplify the process of analyzing candle data and common features. Many of these functionalities are inspired by those found in Pine Scripting.
 
 ## Indicators
-- ADX
-- ATR
-- KC
-- EMA
-- HighLowAverage
-- MACD
-- OBV
-- RMA
-- RSI
-- ROC
-- SMA
-- STOCH
+
+- Average Directional Index(ADX)
+- Aroon
+- Average True Range (ATR)
+- Bollinger Bands (BBANDS)
+- Counter
+- Donchian Channels (donchian)
+- Exponential Moving Average (EMA)
+- High Low Average
+- Hull Moving Average (HMA)
+- Keltner Channel (KC)
+- Moving Average Convergence/Divergence (MACD)
+- On Balance Volume (OBV)
+- Relative Moving Average (RMA)
+- Rate of Change (ROC)
+- Relative strength index (RSI)
+- Simple Moving Average(SMA)
+- Standard Deviation (STDEV)
+- Stochastic Oscillator (STOCH)
 - Supertrend
-- TR
-- VWAP
-- VWMA
-- WMA
+- True Range (TR)
+- True Strength Index (TSI)
+- Volume Weighted Average Price (VWAP)
+- Volume Weighed Moving Averge (VWMA)
+- Weighed Moving Average (WMA)
 
 ## Candlestick Patterns
+
 Simple useful Candle pattern recognition, such as Doji, hammer, etc
+
 - Doji
+- Dojistar
 - Hammer
+- Inverted Hammer
 
 ## Candlestick Types
+
 Hexital can also automatically convert Candlesticks into specific types, such as:
+
 - Heikin-Ashi
 
 ## Candlestick Movements
+
 Simple useful Candle Anaylsis methods such as those in [Pine Scripting](https://www.tradingview.com/pine-script-reference/v5/)
+
 - Positive/Negative Candle
 - Rising/Falling Indicator
 - Mean Based Rising/Falling Indicator
 - Highest/Lowest Indicator (Value)
 - HighestBar/LowestBar Indicator (Offset how far back)
 - Indicator Cross
 - Indicator CrossOver/CrossUnder
 
 ## Installation
+
 ### Stable
+
 Pip and pypi package version is the latest stable version.
+
 ```bash
 pip install hexital
 ```
+
 ## Latest
+
 In case you want to install the latest development version from the repo.
+
 ```bash
 pip install git+https://github.com/merlinr/hexital.git@development
 ```
 
 ## Usage
 
 ### Single Indicator
+
 ```python
 from hexital import EMA, Candle
+from hexital.analysis import movement
 import pandas as pd
 
 my_candles = [
     {"open": 17213, "high": 2395, "low": 7813, "close": 3615, "volume": 19661},
     {"open": 1301, "high": 3007, "low": 11626, "close": 19048, "volume": 28909},
     {"open": 12615, "high": 923, "low": 7318, "close": 1351, "volume": 33765},
     {"open": 1643, "high": 16229, "low": 17721, "close": 212, "volume": 3281},
@@ -110,92 +148,81 @@
 ]
 # Convert Basic candles
 candles = Candle.from_dicts(my_candles)
 # Or directly from a Numpy Dataframe
 # df = pd.read_csv("path/to/symbol.csv", sep=",")
 # candles = Candle.from_dicts(df.to_dict("records"))
 
-my_ema = EMA(candles=candles, period=3)
-my_ema.calculate()
-
-# Indicator name is generated based on Indicator and parameters
-print(my_ema.name) # EMA_3
-
-# Check if started generating Readings
-print(my_ema.has_reading) # True
-
-# Get EMA indicator readings
-# Latest
-print(my_ema.reading()) # 8408.7552
-# All
-print(my_ema.as_list()) # [None, None, 8004.6667, 4108.3333, 5708.1667, 7063.0833, 12414.0416, 15606.0208, 8518.5104, 8408.7552]
+print("Indicator name:", my_ema.name)  # EMA_3
+print("Has reading:", my_ema.has_reading)  # True
+print("Latest EMA reading:", my_ema.reading())  # 8408.7552
+print("All EMA readings:", my_ema.as_list())
+# [None, None, 8004.6667, 4108.3333, 5708.1667, 7063.0833, 12414.0416, 15606.0208, 8518.5104, 8408.7552]
 
 # Add new
 my_ema.append(Candle.from_dict({'open': 19723, 'high': 4837, 'low': 11631, 'close': 6231, 'volume': 38993}))
-print(my_ema.as_list()) # [None, None, 8004.6667, 4108.3333, 5708.1667, 7063.0833, 12414.0416, 15606.0208, 8518.5104, 8408.7552, 7319.8776]
+print("EMA readings after appending new candle:", my_ema.as_list())
+ # [None, None, 8004.6667, 4108.3333, 5708.1667, 7063.0833, 12414.0416, 15606.0208, 8518.5104, 8408.7552, 7319.8776]
 
 # Check Reading and Prev Reading
-print(my_ema.reading()) # 7319.8776
-print(my_ema.prev_reading()) # 8408.7552
+print("EMA reading:", my_ema.reading())  # 7319.8776
+print("Previouse EMA reading:", my_ema.prev_reading())  # 8408.7552
 
 # How many EMA readings been generated
 print(my_ema.reading_count()) # 9
 
 # Purge Readings
 my_ema.purge()
-print(my_ema.reading()) # None
-
-# Purge and Re-calculate
+print("EMA reading after purging:", my_ema.reading())  # None
 my_ema.recalculate()
-print(my_ema.reading()) # 7319.8776
+print("EMA reading after recalculation:", my_ema.reading())  # 7319.8776
 
 # Recalculate latest
 my_ema.calculate_index("EMA_3")
 
-# Access other Readings (Reading get's the latest readings)
-print(my_ema.reading("high")) # 4837
+# Access specific readings
+print("Latest high reading:", my_ema.reading("high"))  # 4837
+print("High reading at index -2:", my_ema.reading("high", index=-2))  # 6584
 
-# Access other specific Readings (Older readings)
-print(my_ema.reading("high", index=-2)) # 6584
-
-# Easily view candlestick trends
-print(my_ema.falling()) # True
 ```
 
-
 ## Upcoming Features
 
 Roughly ordered in priority
 
-- Modular framework (like indicators) to repaint candles, E.G as Renko, Range, etc 
 - More Indicators
 - More Movement methods
 - More Patterns
 - Indicator Pluggability, to allow easy extension of this library
-  - Allowing custom Indictors to be added
+  - Allowing easier custom Indictors to be added
 - Multiprocessing, of indictors stored within hexial Class.
   - Likely wont see increase in performance
 
-
 ## Testing
-Testing is a huge part of this library as it's incredibly difficult to ensure the accuracy of the indicator values being generated. In order to solve this this I rely on [Pandas-TA](https://github.com/twopirllc/pandas-ta) as my source of truth for the indicator values. Each indicator added to this library requires a test that uses the Pandas-TA lib indicator output as the expected result. Due to some difference's in the calculations done withinin Numpy, not all values are exactly identical, therefore if there are differences outside of the given 1 decimal place, than a pearson correlation coefficient is calculated to ensure correct correlation with the givne output.
+
+Testing is a critical aspect of this library due to the complexity of ensuring the accuracy of generated indicator values. To achieve this, I rely on [Pandas-TA](https://github.com/twopirllc/pandas-ta) as the source of truth for indicator values. Each indicator added to this library undergoes testing, where the output is compared against the corresponding indicator output from Pandas-TA. Due to slight differences in calculations, particularly within NumPy, not all values are exactly identical. Therefore, if differences exceed a given threshold (usually beyond one decimal place), a Pearson correlation coefficient is calculated to ensure correct correlation with the expected output.
 
 ### Speed Tests
-The following charts indicate the results and speed of Pandas-TA and Hexital both Bulk and Incremental calculations these are the following results of running Pandas-TA and hexital both in Bulk (_all candles calculated at once_) and incremental (_Caluclating after each new candle is added_); charts _1 and 2_.
 
-The incremental chart's here are calculating the TA, adding one, re-calculating up to N amount. Pandas-TA/Pandas/Numpy for incremental data is clearly a slow process, this from my understanding due to the underlying way numpy will append/concat data, having to re-create the memory rather than resize. This is why Numpy/Panda's recommend gathering all the data prior to running calculations on it. Whereby the bulk calculating in Pandas-TA is consistent with a small time increase with the amount of data. While `Hexital` running purely pythonic can run in quickly in bulk and incremental, with little to no extra overhead time; clearly performing far faster than Pandas-TA Incremental and even faster than Pandas-TA with smaller set of data. 
+The following charts illustrate the results and speed of Pandas-TA and Hexital in both bulk and incremental calculations. These results are obtained from running Pandas-TA and Hexital in bulk (_all candles calculated at once_) and incremental(_Caluclating after each new candle is added_) modes; charts _1 and 2_.
+
+The incremental charts demonstrate the process of calculating technical analysis, adding one candle at a time, and recalculating up to a specified number of candles. It's evident that using Pandas-TA, Pandas, and NumPy for incremental data processing incurs significant performance overhead. This is primarily due to the underlying behavior of NumPy, which involves reallocating memory when appending or concatenating data, rather than resizing it. As a result, it's recommended in NumPy and Pandas documentation to gather all data prior to running calculations. On the other hand, Hexital, being purely Pythonic, exhibits efficient performance both in bulk and incremental processing, with minimal to no additional overhead time. It significantly outperforms Pandas-TA in incremental processing and even surpasses Pandas-TA in speed, especially with smaller datasets.
 
 ![EMA 10 test results.](tests/speed_tests/EMA_10.png)
 
-From chart _(3)_  you can clearly see that with bulk calculations with an extremely large dataset, Pandas-Ta performs better than `Hexital` in large Bulk data. Bulk calculations Pandas-TA going from 0.08 for 1,000 and staying there for 10,000, While Hexital Goes from 0.005 seconds for 1,000 to 0.05 seconds for 10,000. While Hexital is faster, there is a clear growth in process time. Therefore for backtesting with a large dataset, Pandas-TA will give you the best performance, whereas Hexital will continue to slow down.
+From chart _(3)_, it's evident that in bulk calculations with an extremely large dataset, Pandas-TA outperforms Hexital. Pandas-TA maintains consistent performance, with processing times starting at 0.08 seconds for 1,000 candles and remaining stable at this level for 10,000 candles. In contrast, Hexital exhibits faster processing times, starting at 0.005 seconds for 1,000 candles but increasing to 0.05 seconds for 10,000 candles. While Hexital is initially faster, there is a noticeable growth in processing time as the dataset size increases. Therefore, for backtesting with a large dataset, Pandas-TA offers superior performance, while Hexital may experience slowdowns.
 
 ![EMA 10 Bulk test results.](tests/speed_tests/EMA_10%20Bulk%20Calculations.png)
 
 However referencing chart _(4)_ being an example of using both these libraries for a live application, whereby at n candles we incrementing a dataset with a candle and calculating the new TA; `Hexital` is far quicker. This is due to the speed that python can increment a list of data rather than Panda, as well as `Hexital` only needing to calculate the newest candle rather than having to re-calculate the entire dataset. Chart _3_ clearly shows the speed benefits it has over Pandas-TA and other Panda based Technical Analysis tools for incremental data sets.
 
 ![EMA 10 Real world usage.](tests/speed_tests/EMA_10_real_world.png)
 
 For reference, if using seconds Candle with 10,000 candles that is around 2 Hours 46 minutes.
+
 #### Note
+
 The code that produces these charts is: `tests/speed_tests/run_speed_test.py` and can be ran by calling `make speed-test`. Some noise is seen due to running on personal laptop while in use.
+
 ## Inspiration
-This library was was inspired by [TALIpp](https://github.com/nardew/talipp) which is another Incremental Technical Analysis Library, however I disliked the seperate input lists rather then an entire candle, and futhermore outputs are seperated entities requiring lots of managing. Whereas Hexital stores all data within the Candles making easier usage.
+
+This library was inspired by [TALIpp](https://github.com/nardew/talipp), another Incremental Technical Analysis Library. However, I found the separate input lists rather cumbersome compared to working with an entire candle. Additionally, in TALIpp, outputs are separate entities, requiring extensive management. In contrast, Hexital stores all data within the candle, simplifying usage and management.
```

### Comparing `hexital-1.0.1/hexital/analysis/__init__.py` & `hexital-1.1.0/hexital/analysis/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     mean_falling,
     mean_rising,
     negative,
     positive,
     rising,
     value_range,
 )
-from .patterns import doji, hammer  # noqa F401
+from .patterns import doji, dojistar, hammer, inverted_hammer  # noqa F401
 
 MOVEMENT_MAP = {
     "cross": cross,
     "crossover": crossover,
     "crossunder": crossunder,
     "falling": falling,
     "highest": highest,
@@ -31,9 +31,11 @@
     "positive": positive,
     "rising": rising,
     "value_range": value_range,
 }
 
 PATTERN_MAP = {
     "doji": doji,
+    "dojistar": dojistar,
     "hammer": hammer,
+    "inv_hammer": inverted_hammer,
 }
```

### Comparing `hexital-1.0.1/hexital/analysis/movement.py` & `hexital-1.1.0/hexital/analysis/movement.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,28 +22,28 @@
         reading_by_candle(candle, indicator) for candle in candles[index - length : to_index]
     ]
     return [reading for reading in readings if isinstance(reading, (float, int))]
 
 
 def positive(candles: Candle | List[Candle], index: int = -1) -> bool:
     if isinstance(candles, Candle):
-        return candles.positive()
+        return candles.positive
 
     if not valid_index(index, len(candles)):
         return False
-    return candles[index].positive()
+    return candles[index].positive
 
 
 def negative(candles: Candle | List[Candle], index: int = -1) -> bool:
     if isinstance(candles, Candle):
-        return candles.negative()
+        return candles.negative
 
     if not valid_index(index, len(candles)):
         return False
-    return candles[index].negative()
+    return candles[index].negative
 
 
 def above(candles: List[Candle], indicator: str, indicator_two: str, index: int = -1) -> bool:
     """Check if indicator is a higher value than indicator_two"""
     if not candles:
         return False
 
@@ -241,15 +241,15 @@
 
     high = None
     distance = 0
 
     for dist, index in enumerate(range(index_, index_ - length, -1)):
         current = reading_by_index(candles, indicator, index)
         if current is None or isinstance(current, dict):
-            break
+            continue
 
         if high and high < current:
             high = current
             distance = dist
         elif high is None:
             high = current
 
@@ -272,15 +272,15 @@
 
     low = None
     distance = 0
 
     for dist, index in enumerate(range(index_, index_ - length, -1)):
         current = reading_by_index(candles, indicator, index)
         if current is None or isinstance(current, dict):
-            break
+            continue
 
         if low and low > current:
             low = current
             distance = dist
         elif low is None:
             low = current
```

### Comparing `hexital-1.0.1/hexital/candlesticks/heikinashi.py` & `hexital-1.1.0/hexital/candlesticks/heikinashi.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.1/hexital/core/candle.py` & `hexital-1.1.0/hexital/core/candle.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     "close",
     "volume",
     "timestamp",
     "indicators",
     "sub_indicators",
 ]
 
+IGNORE_CLEAN = ["clean_values", "indicators", "sub_indicators"]
+
 
 class Candle:
     open: float
     high: float
     low: float
     close: float
     volume: int
@@ -60,58 +62,52 @@
             return False
         for key in KEY_KEYS:
             if getattr(self, key) != getattr(other, key):
                 return False
         return True
 
     def __repr__(self) -> str:
-        return str(
-            {
-                "open": self.open,
-                "high": self.high,
-                "low": self.low,
-                "close": self.close,
-                "volume": self.volume,
-                "timestamp": self.timestamp,
-                "indicators": self.indicators,
-                "sub_indicators": self.sub_indicators,
-                "tag": self.tag,
-            }
-        )
+        return str({name: value for name, value in vars(self).items() if not name.startswith("_")})
 
     @property
     def tag(self) -> str | None:
         return self._tag
 
     @tag.setter
     def tag(self, tag: str):
         if not self._tag:
             self._tag = tag
             return
         raise CandleAlreadyTagged(f"Candle already tagged as {self._tag} - [{self}]")
 
+    @property
     def positive(self) -> bool:
         return self.open < self.close
 
+    @property
     def negative(self) -> bool:
         return self.open > self.close
 
+    @property
     def realbody(self) -> float:
         return abs(self.open - self.close)
 
+    @property
     def shadow_upper(self) -> float:
-        if self.positive():
+        if self.positive:
             return abs(self.high - self.close)
         return abs(self.high - self.open)
 
+    @property
     def shadow_lower(self) -> float:
-        if self.positive():
+        if self.positive:
             return abs(self.low - self.open)
         return abs(self.low - self.close)
 
+    @property
     def high_low(self) -> float:
         return abs(self.high - self.low)
 
     @classmethod
     def from_dict(cls, candle: Dict[str, Any]) -> Candle:
         """Expected dict with keys ['open', 'high', 'low', 'close', 'volume']
         with optional 'timestamp' key."""
@@ -153,28 +149,23 @@
     def from_lists(candles: List[List[float]]) -> List[Candle]:
         """Expected list of the following list [open, high, low, close, volume]
         with optional datetime at the beginning or end."""
         return [Candle.from_list(candle) for candle in candles]
 
     def save_clean_values(self):
         self.clean_values = {
-            "open": self.open,
-            "high": self.high,
-            "low": self.low,
-            "close": self.close,
-            "volume": self.volume,
+            name: value
+            for name, value in vars(self).items()
+            if not name.startswith("_") or name in IGNORE_CLEAN
         }
 
     def recover_clean_values(self):
         if self.clean_values:
-            self.open = self.clean_values["open"]
-            self.high = self.clean_values["high"]
-            self.low = self.clean_values["low"]
-            self.close = self.clean_values["close"]
-            self.volume = int(self.clean_values["volume"])
+            for name, value in self.clean_values.items():
+                self.__setattr__(name, value)
 
     def reset_candle(self):
         self.indicators = {}
         self.sub_indicators = {}
         self._tag = None
 
     def merge(self, candle: Candle):
```

### Comparing `hexital-1.0.1/hexital/core/candle_manager.py` & `hexital-1.1.0/hexital/core/candle_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     clean_timestamp,
     on_timeframe,
     round_down_timestamp,
     timeframe_to_timedelta,
 )
 
 DEFAULT_CANDLES = "default"
-_KEY_CONFIGS = ["candles_lifespan", "timeframe", "timeframe_fill"]
 
 
 class CandleManager:
     candles: List[Candle]
     candles_lifespan: Optional[timedelta]
     timeframe: Optional[str] = None
     timeframe_fill: bool = False
@@ -50,15 +49,16 @@
         self.candlestick_type = candlestick_type
 
         self._tasks()
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, CandleManager):
             return False
-        for key in _KEY_CONFIGS:
+
+        for key in ["candles_lifespan", "timeframe", "timeframe_fill"]:
             if getattr(self, key) != getattr(other, key):
                 return False
 
         return True
 
     @property
     def name(self) -> str:
@@ -80,15 +80,15 @@
 
         if isinstance(candles, Candle):
             candles_.append(candles)
         elif isinstance(candles, dict):
             candles_.append(Candle.from_dict(candles))
         elif isinstance(candles, list):
             if not candles:
-                pass
+                return
             elif isinstance(candles[0], Candle):
                 candles_.extend(candles)
             elif isinstance(candles[0], dict):
                 candles_.extend(Candle.from_dicts(candles))
             elif isinstance(candles[0], (float, int)):
                 candles_.append(Candle.from_list(candles))
             elif isinstance(candles[0], list):
@@ -201,16 +201,18 @@
                     low=prev_candle.close,
                     volume=0,
                     timestamp=prev_candle.timestamp + timeframe,
                 )
                 candles.insert(index, fill_candle)
 
             index += 1
+
             if index >= len(candles):
                 break
+
         return candles
 
     def convert_candles(self):
         if not self.candles or not self.candlestick_type:
             return
 
         self.candlestick_type.conversion(self.candles)
```

### Comparing `hexital-1.0.1/hexital/core/candlestick_type.py` & `hexital-1.1.0/hexital/core/candlestick_type.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.1/hexital/core/hexital.py` & `hexital-1.1.0/hexital/core/indicator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,366 +1,341 @@
+from __future__ import annotations
+
+from abc import ABC, abstractmethod
 from copy import deepcopy
+from dataclasses import dataclass, field
 from datetime import timedelta
-from typing import Dict, List, Optional, Set
+from typing import Dict, List, Optional
 
-from hexital.analysis import MOVEMENT_MAP, PATTERN_MAP, movement, patterns
 from hexital.core.candle import Candle
-from hexital.core.candle_manager import DEFAULT_CANDLES, CandleManager
+from hexital.core.candle_manager import CandleManager
 from hexital.core.candlestick_type import CandlestickType
-from hexital.core.indicator import Indicator
-from hexital.exceptions import (
-    InvalidAnalysis,
-    InvalidIndicator,
-    InvalidTimeFrame,
-    MissingIndicator,
-    MixedTimeframes,
+from hexital.utils.candles import (
+    candles_sum,
+    reading_by_candle,
+    reading_count,
+    reading_period,
 )
-from hexital.indicators import INDICATOR_MAP
-from hexital.utils.candles import reading_by_index
 from hexital.utils.candlesticks import validate_candlesticktype
+from hexital.utils.indexing import round_values
 from hexital.utils.timeframe import TimeFrame, validate_timeframe
 
 
-class Hexital:
-    name: str
-    _candles: Dict[str, CandleManager]
-    _indicators: Dict[str, Indicator]
-    description: Optional[str] = None
-    timeframe: Optional[str] = None
+@dataclass(kw_only=True)
+class Indicator(ABC):
+    candles: List[Candle] = field(default_factory=list)
+    fullname_override: Optional[str] = None
+    name_suffix: Optional[str] = None
+    round_value: int = 4
+    timeframe: Optional[str | TimeFrame] = None
     timeframe_fill: bool = False
     candles_lifespan: Optional[timedelta] = None
-    candlestick_type: Optional[CandlestickType] = None
+    candlestick_type: Optional[CandlestickType | str] = None
 
-    def __init__(
-        self,
-        name: str,
-        candles: List[Candle],
-        indicators: Optional[List[dict | Indicator]] = None,
-        description: Optional[str] = None,
-        timeframe: Optional[str | TimeFrame] = None,
-        timeframe_fill: bool = False,
-        candles_lifespan: Optional[timedelta] = None,
-        candlestick_type: Optional[CandlestickType | str] = None,
-    ):
-        self.name = name
-        self.description = description
+    sub_indicators: Dict[str, Indicator] = field(init=False, default_factory=dict)
+    managed_indicators: Dict[str, Managed | Indicator] = field(init=False, default_factory=dict)
+    _sub_indicator: bool = field(init=False, default=False)
+    _sub_calc_prior: bool = field(init=False, default=True)
+
+    _name: str = field(init=False, default="")
+    _output_name: str = field(init=False, default="")
+    _candles: CandleManager = field(init=False, default_factory=CandleManager)
+    _active_index: int = field(init=False, default=0)
+    _initialised: bool = field(init=False, default=False)
+
+    def __post_init__(self):
+        self._validate_fields()
+
+        if self.timeframe is not None:
+            self.timeframe = validate_timeframe(self.timeframe)
+
+        if self.candlestick_type is not None:
+            self.candlestick_type = validate_candlesticktype(self.candlestick_type)
+
+        self._candles = CandleManager(
+            self.candles,
+            self.candles_lifespan,
+            self.timeframe,
+            self.timeframe_fill,
+            self.candlestick_type,
+        )
 
-        if timeframe:
-            self.timeframe = validate_timeframe(timeframe)
-        self.timeframe_fill = timeframe_fill
-        self.candles_lifespan = candles_lifespan
-
-        if candlestick_type:
-            self.candlestick_type = validate_candlesticktype(candlestick_type)
-
-        self._candles = {
-            DEFAULT_CANDLES: CandleManager(
-                candles if isinstance(candles, list) else [],
-                candles_lifespan=self.candles_lifespan,
-                timeframe=self.timeframe,
-                timeframe_fill=self.timeframe_fill,
-                candlestick_type=self.candlestick_type,
-            )
-        }
-
-        self._indicators = self._validate_indicators(indicators) if indicators else {}
-
-    def _validate_indicators(self, indicators: List[dict | Indicator]) -> Dict[str, Indicator]:
-        if not indicators:
-            return {}
-
-        valid_indicators = {}
-
-        for indicator in indicators:
-            if isinstance(indicator, Indicator):
-                valid_indicators[indicator.name] = indicator
-                continue
+        self.candles = self._candles.candles
+
+        self._internal_generate_name()
+
+    def __str__(self):
+        data = vars(self)
+        data.pop("candles")
+        data["name"] = data["_output_name"]
+        return str(data)
+
+    def _internal_generate_name(self):
+        name = ""
 
-            if not isinstance(indicator, dict):
-                raise InvalidIndicator(
-                    f"Indicator type invalid 'indicator' must be a dict or Indicator type: {indicator}"
-                )
-
-            new_indicator = self._build_indicator(indicator)
-            valid_indicators[new_indicator.name] = new_indicator
-
-        for indicator in valid_indicators.values():
-            manager = CandleManager(
-                [],
-                candles_lifespan=self.candles_lifespan,
-                timeframe=indicator.timeframe if indicator.timeframe else self.timeframe,
-                timeframe_fill=self.timeframe_fill,
-                candlestick_type=self.candlestick_type,
-            )
-
-            if manager == self._candles[DEFAULT_CANDLES]:
-                indicator.candle_manager = self._candles[DEFAULT_CANDLES]
-            elif manager.name in self._candles:
-                indicator.candle_manager = self._candles[manager.name]
-            else:
-                self._candles[manager.name] = manager
-                manager.append(deepcopy(self._candles[DEFAULT_CANDLES]).candles)
-                indicator.candle_manager = self._candles[manager.name]
-
-        return valid_indicators
-
-    def _build_indicator(self, raw_indicator: dict) -> Indicator:
-        analysis_map = PATTERN_MAP | MOVEMENT_MAP
-        amorph_class = INDICATOR_MAP["Amorph"]
-
-        if raw_indicator.get("indicator"):
-            indicator_name = raw_indicator.pop("indicator")
-
-            if INDICATOR_MAP.get(indicator_name):
-                indicator_class = INDICATOR_MAP[indicator_name]
-                return indicator_class(**raw_indicator)
-            else:
-                raise InvalidIndicator(f"Indicator {indicator_name} does not exist")
-
-        elif raw_indicator.get("analysis") and isinstance(raw_indicator.get("analysis"), str):
-            analysis_name = raw_indicator.pop("analysis")
-            if not analysis_map.get(analysis_name):
-                raise InvalidAnalysis(
-                    f"analysis {analysis_name} does not exist in patterns or movements"
-                )
-
-            return amorph_class(analysis=analysis_map[analysis_name], **raw_indicator)
-
-        elif raw_indicator.get("analysis") and callable(raw_indicator.get("analysis")):
-            method_name = raw_indicator.pop("analysis")
-            return amorph_class(analysis=method_name, **raw_indicator)
+        if self.fullname_override:
+            name = self.fullname_override
         else:
-            raise InvalidAnalysis(
-                f"Dict Indicator missing 'indicator' or 'analysis' name, not: {raw_indicator}"
-            )
-
-    def candles(self, timeframe: Optional[str] = None) -> List[Candle]:
-        if timeframe and self._candles.get(timeframe, False):
-            return self._candles[timeframe].candles
-        return self._candles[DEFAULT_CANDLES].candles
+            name = self._generate_name()
+            if self.timeframe:
+                name += f"_{self._candles.timeframe}"
 
-    def candles_all(self) -> Dict[str, List[Candle]]:
-        return {name: manager.candles for name, manager in self._candles.items()}
+        if self.name_suffix:
+            name += f"_{self.name_suffix}"
+
+        self._output_name = self._sanitise_name(name)
+
+    def _initialise(self):
+        return
+
+    def _validate_fields(self):
+        return
+
+    @abstractmethod
+    def _generate_name(self) -> str: ...
+
+    def _sanitise_name(self, name: str) -> str:
+        return name.replace(".", ",")
 
     @property
-    def timeframes(self) -> Set[str]:
-        return {str(manager.timeframe) for manager in self._candles.values()}
+    def candle_manager(self) -> CandleManager:
+        """The Candle Manager which controls TimeFrame, Trimming and collapsing"""
+        return self._candles
+
+    @candle_manager.setter
+    def candle_manager(self, manager: CandleManager):
+        """The Candle Manager which controls TimeFrame, Trimming and collapsing,
+        this will overwrite the Manager as well as the candles"""
+        self._candles = manager
+        self.candles = manager.candles
+        self.timeframe = manager.timeframe
+        self.timeframe_fill = manager.timeframe_fill
+        self.candles_lifespan = manager.candles_lifespan
+        self.candlestick_type = manager.candlestick_type
 
     @property
-    def indicators(self) -> Dict[str, Indicator]:
-        """Simply get's a list of all the Indicators within Hexital strategy"""
-        return self._indicators
+    def name(self) -> str:
+        """The indicator name that will be saved into the Candles"""
+        return self._output_name
 
     @property
-    def indicator_settings(self) -> List[dict]:
-        """Simply get's a list of all the Indicators within Hexital strategy"""
-        return [indicator.settings for indicator in self._indicators.values()]
-
-    def indicator(self, name: str) -> Indicator | None:
-        for indicator_name, indicator in self._indicators.items():
-            if name in indicator_name:
-                return indicator
-        return None
-
-    def has_reading(self, name: str) -> bool:
-        """Checks if the given Indicator has a valid reading in latest Candle"""
-        return bool(self.reading(name))
-
-    def reading(self, name: str, index: int = -1) -> float | dict | None:
-        """Attempts to retrieve a reading with a given Indicator name.
-        `name` can use '.' to find nested reading, E.G `MACD_12_26_9.MACD`
-        """
-        reading = reading_by_index(self._candles[DEFAULT_CANDLES].candles, name, index=index)
+    def has_reading(self) -> bool:
+        """Simple boolean to state if values are being generated yet in the candles"""
+        if len(self.candles) == 0:
+            return False
+        return self.reading(index=self._active_index) is not None
 
-        if reading is not None:
-            return reading
+    @property
+    def prior_calc(self) -> bool:
+        if self._sub_indicator and self._sub_calc_prior:
+            return True
+        return False
 
-        for candle_manager in self._candles.values():
-            reading = reading_by_index(candle_manager.candles, name, index=index)
-            if reading is not None:
-                return reading
-
-        return None
-
-    def prev_reading(self, name: str) -> float | dict | None:
-        return self.reading(name, index=-2)
-
-    def reading_as_list(self, name: str) -> List[float | dict | None]:
-        """Find given indicator and returns the readings as a list
-        Full Name of the indicator E.G `EMA_12` OR `MACD_12_26_9.MACD`"""
-        primary_name = name.split(".")[0]
-        if self._indicators.get(primary_name):
-            return self._indicators[primary_name].as_list(name)
-        return []
+    @property
+    def settings(self) -> dict:
+        """Returns a dict format of how this indicator can be generated"""
+        output = {"indicator": self._name if self._name else type(self).__name__}
 
-    def add_indicator(
-        self, indicator: Indicator | List[Indicator | Dict[str, str]] | Dict[str, str]
-    ):
-        """Add's a new indicator to `Hexital` strategy.
-        This accept either `Indicator` datatypes or dict string versions to be packed.
-        `add_indicator(SMA(period=10))` or `add_indicator({"indicator": "SMA", "period": 10})`
-        Does not automatically calculates readings."""
-        indicators = indicator if isinstance(indicator, list) else [indicator]
-
-        for valid_indicator in self._validate_indicators(indicators).values():
-            self._indicators[valid_indicator.name] = valid_indicator
-
-    def get_indicator(self, name: str) -> Indicator | None:
-        """Searches hexital's indicator's and Returns the Indicator object itself."""
-        return self._indicators.get(name)
-
-    def remove_indicator(self, name: str):
-        """Removes an indicator from running within hexital"""
-        self.purge(name)
-        self._indicators.pop(name, None)
+        for name, value in self.__dict__.items():
+            if name in ["candles", "managed_indicators", "sub_indicators"]:
+                continue
+            if name == "timeframe_fill" and self.timeframe is None:
+                continue
 
-    def append(self, candles: Candle | List[Candle] | dict | List[dict] | list | List[list]):
-        for candle_manager in self._candles.values():
-            candle_manager.append(candles)
+            if name == "candlestick_type" and value:
+                output[name] = value.minimal_name
+            elif not name.startswith("_") and value is not None:
+                output[name] = deepcopy(value)
+
+        return output
+
+    def as_list(self, name: Optional[str] = None) -> List[float | dict | None]:
+        """Gathers the indicator for all candles as a list
+        E.G `EMA_12` OR `MACD_12_26_9.MACD`"""
+        return [reading_by_candle(candle, name if name else self.name) for candle in self.candles]
+
+    def _set_reading(self, reading: float | dict | None, index: Optional[int] = None):
+        index = index if index else self._active_index
+
+        if self._sub_indicator:
+            self.candles[index].sub_indicators[self.name] = reading
+        else:
+            self.candles[index].indicators[self.name] = reading
 
+    def append(self, candles: Candle | List[Candle] | dict | List[dict] | list | List[list]):
+        self._candles.append(candles)
         self.calculate()
 
-    def purge(self, name: Optional[str] = None):
-        """Takes Indicator name and removes all readings for said indicator.
-        Indicator name must be exact"""
-        for indicator_name, indicator in self._indicators.items():
-            if name is None or (name and name in indicator_name):
-                indicator.purge()
-
-    def calculate(self, name: Optional[str] = None):
-        """Calculates all the missing indicator readings."""
-        for indicator_name, indicator in self._indicators.items():
-            if name is None or indicator_name == name:
-                indicator.calculate()
-
-    def calculate_index(self, name: Optional[str] = None, index: int = -1):
-        """Calculate specific index for all or specific indicator readings."""
-        for indicator_name, indicator in self._indicators.items():
-            if name is None or indicator_name == name:
-                indicator.calculate_index(index)
-
-    def recalculate(self, name: Optional[str] = None):
-        """Purge's all indicator reading's and re-calculates them all,
-        ideal for changing an indicator parameters midway."""
-        self.purge(name)
-        self.calculate(name)
-
-    def _find_indicator(self, indicator: str) -> CandleManager | None:
-        for manager in self._candles.values():
-            if not manager.candles:
-                return manager
-            elif manager.find_indicator(indicator):
-                return manager
-
-        return None
-
-    def _verify_indicators(
-        self, indicator: str, indicator_two: Optional[str] = None
-    ) -> List[Candle]:
-        manager = self._find_indicator(indicator)
-
-        if not manager and indicator in self._indicators:
-            return []
-        elif manager and not indicator_two:
-            return manager.candles
-
-        if not indicator_two or not manager:
-            raise MissingIndicator("Cannot find Indicator: %s" % indicator)
-
-        manager_two = self._find_indicator(indicator_two)
-
-        if not manager_two:
-            raise MissingIndicator("Cannot find Indicator: %s" % indicator_two)
-
-        for manager in self._candles.values():
-            if manager.find_indicator(indicator) and manager.find_indicator(indicator_two):
-                return manager.candles
+    def _calculate_reading(self, index: int) -> float | dict | None:
+        pass
 
-        raise MixedTimeframes(
-            "Cannot find {%s} and {%s} within same timeframe" % (indicator, indicator_two)
-        )
+    def _calculate_sub_indicators(
+        self,
+        prior_calc: bool = True,
+        start_index: Optional[int] = None,
+        end_index: Optional[int] = None,
+    ):
+        for indicator in self.sub_indicators.values():
+            if indicator.prior_calc == prior_calc:
+                if start_index and end_index:
+                    indicator.calculate_index(start_index, end_index)
+                else:
+                    indicator.calculate()
+
+    def calculate(self):
+        """Calculate the TA values, will calculate for all the Candles,
+        where this indicator is missing"""
+        if not self._initialised:
+            self._initialise()
+            self._initialised = True
 
-    def above(self, indicator: str, indicator_two: str, index: int = -1) -> bool:
-        candles = self._verify_indicators(indicator, indicator_two)
-        return movement.above(candles, indicator, indicator_two, index)
-
-    def below(self, indicator: str, indicator_two: str, index: int = -1) -> bool:
-        candles = self._verify_indicators(indicator, indicator_two)
-        return movement.below(candles, indicator, indicator_two, index)
-
-    def cross(self, indicator: str, indicator_two: str, length: int = 1, index: int = -1) -> bool:
-        candles = self._verify_indicators(indicator, indicator_two)
-        return movement.cross(candles, indicator, indicator_two, length, index)
+        self._calculate_sub_indicators(prior_calc=True)
 
-    def crossover(
-        self, indicator: str, indicator_two: str, length: int = 1, index: int = -1
-    ) -> bool:
-        candles = self._verify_indicators(indicator, indicator_two)
-        return movement.crossover(candles, indicator, indicator_two, length, index)
+        for index in range(self._find_calc_index(), len(self.candles)):
+            self._set_active_index(index)
 
-    def crossunder(
-        self, indicator: str, indicator_two: str, length: int = 1, index: int = -1
-    ) -> bool:
-        candles = self._verify_indicators(indicator, indicator_two)
-        return movement.crossunder(candles, indicator, indicator_two, length, index)
+            if self.candles[index].indicators.get(self.name) is not None:
+                continue
 
-    def rising(self, name: str, length: int = 4, index: int = -1) -> bool:
-        candles = self._verify_indicators(name)
-        return movement.rising(candles, name, length, index)
-
-    def falling(self, name: str, length: int = 4, index: int = -1) -> bool:
-        candles = self._verify_indicators(name)
-        return movement.falling(candles, name, length, index)
-
-    def mean_rising(self, name: str, length: int = 4, index: int = -1) -> bool:
-        candles = self._verify_indicators(name)
-        return movement.mean_rising(candles, name, length, index)
-
-    def mean_falling(self, name: str, length: int = 4, index: int = -1) -> bool:
-        candles = self._verify_indicators(name)
-        return movement.mean_falling(candles, name, length, index)
-
-    def highest(self, name: str, length: int = 4, index: int = -1) -> float:
-        candles = self._verify_indicators(name)
-        return movement.highest(candles, name, length, index)
-
-    def lowest(self, name: str, length: int = 4, index: int = -1) -> float:
-        candles = self._verify_indicators(name)
-        return movement.lowest(candles, name, length, index)
-
-    def highestbar(self, name: str, length: int = 4, index: int = -1) -> int | None:
-        candles = self._verify_indicators(name)
-        return movement.highestbar(candles, name, length, index)
-
-    def lowestbar(self, name: str, length: int = 4, index: int = -1) -> int | None:
-        candles = self._verify_indicators(name)
-        return movement.lowestbar(candles, name, length, index)
+            reading = round_values(self._calculate_reading(index=index), round_by=self.round_value)
+            self._set_reading(reading, index)
 
-    def doji(
-        self,
-        timeframe: str | TimeFrame,
-        length: int = 10,
-        lookback: Optional[int] = None,
-        asint: bool = False,
-        index: Optional[int] = None,
-    ) -> bool | int:
-        manager = self._candles.get(validate_timeframe(timeframe))
-        if not manager:
-            raise InvalidTimeFrame(f"Timeframe {timeframe} not found")
-        return patterns.doji(
-            manager.candles, length=length, lookback=lookback, asint=asint, index=index
+        self._calculate_sub_indicators(prior_calc=False)
+
+    def calculate_index(self, start_index: int, end_index: Optional[int] = None):
+        """Calculate the TA values, will calculate a index range the Candles, will re-calculate"""
+        end_index = end_index if end_index else start_index + 1
+
+        self._calculate_sub_indicators(True, start_index, end_index)
+
+        for index in range(start_index, end_index):
+            self._set_active_index(index)
+            reading = round_values(self._calculate_reading(index=index), round_by=self.round_value)
+            self._set_reading(reading, index)
+
+        self._calculate_sub_indicators(False, start_index, end_index)
+
+    def _find_calc_index(self) -> int:
+        """Optimisation method, to find where to start calculating the indicator from
+        Searches from newest to oldest to find the first candle without the indicator
+        """
+        if len(self.candles) == 0 or self.name not in self.candles[0].indicators:
+            return 0
+
+        for index in range(len(self.candles) - 1, 0, -1):
+            if (
+                self.name in self.candles[index].indicators
+                or self.name in self.candles[index].sub_indicators
+            ):
+                return index + 1
+
+        return len(self.candles) - 1
+
+    def _set_active_index(self, index: int):
+        self._active_index = index
+        for indicator in self.managed_indicators.values():
+            if isinstance(indicator, Managed):
+                indicator.set_active_index(index)
+
+    def add_sub_indicator(self, indicator: Indicator, prior_calc: bool = True):
+        """Adds sub indicator, this will auto calculate with indicator"""
+        indicator._sub_indicator = True
+        indicator._sub_calc_prior = prior_calc
+        indicator.candle_manager = self._candles
+        self.sub_indicators[indicator.name] = indicator
+
+    def add_managed_indicator(self, name: str, indicator: Managed | Indicator):
+        """Adds managed sub indicator, this will not auto calculate with indicator"""
+        indicator._sub_indicator = True
+        indicator.candle_manager = self._candles
+        self.managed_indicators[name] = indicator
+
+    def prev_exists(self, name: Optional[str] = None) -> bool:
+        return self.prev_reading(self.name if not name else name) is not None
+
+    def prev_reading(self, name: Optional[str] = None) -> float | dict | None:
+        if len(self.candles) == 0 or self._active_index == 0:
+            return None
+        return self.reading(name=name if name else self.name, index=self._active_index - 1)
+
+    def reading(
+        self, name: Optional[str] = None, index: Optional[int] = None
+    ) -> float | dict | None:
+        """Simple method to get an indicator reading from the index
+        Name can use '.' to find nested reading, E.G 'MACD_12_26_9.MACD"""
+        return reading_by_candle(
+            self.candles[index if index is not None else self._active_index],
+            name if name else self.name,
         )
 
-    def hammer(
-        self,
-        timeframe: str | TimeFrame,
-        length: int = 10,
-        lookback: Optional[int] = None,
-        asint: bool = False,
-        index: Optional[int] = None,
-    ) -> bool | int:
-        manager = self._candles.get(validate_timeframe(timeframe))
-        if not manager:
-            raise InvalidTimeFrame(f"Timeframe {timeframe} not found")
-        return patterns.hammer(
-            manager.candles, length=length, lookback=lookback, asint=asint, index=index
+    def read_candle(self, candle: Candle, name: Optional[str] = None) -> float | dict | None:
+        """Simple method to get an indicator reading from a candle,
+        regardless of it's location"""
+        return reading_by_candle(candle, name if name else self.name)
+
+    def reading_count(self, name: Optional[str] = None) -> int:
+        """Returns how many instance of the given indicator exist"""
+        return reading_count(self.candles, name if name else self.name)
+
+    def reading_period(
+        self, period: int, name: Optional[str] = None, index: Optional[int] = None
+    ) -> bool:
+        """Will return True if the given indicator goes back as far as amount,
+        It's true if exactly or more than. Period will be period -1"""
+        return reading_period(
+            self.candles,
+            period=period,
+            name=name if name else self.name,
+            index=index if index is not None else self._active_index,
+        )
+
+    def candles_sum(
+        self, length: int = 1, name: Optional[str] = None, index: Optional[int] = None
+    ) -> float | None:
+        return candles_sum(
+            self.candles,
+            name if name else self.name,
+            length,
+            index if index is not None else self._active_index,
         )
+
+    def purge(self):
+        """Remove this indicator value from all Candles"""
+        self._candles.purge(
+            {self.name}
+            | {indicator.name for indicator in self.sub_indicators.values()}
+            | {indicator.name for indicator in self.managed_indicators.values()}
+        )
+
+    def recalculate(self):
+        """Re-calculate this indicator value for all Candles"""
+        self.purge()
+        self.calculate()
+
+
+@dataclass(kw_only=True)
+class Managed(Indicator):
+    """Managed
+
+    Empty Indicator thats manually controlled and the reading manually set.
+
+    """
+
+    indicator_name: str = "MAN"
+    _sub_indicator: bool = True
+    _active_index: int = 0
+
+    def _generate_name(self) -> str:
+        return self.indicator_name
+
+    def set_reading(self, reading: float | dict, index: Optional[int] = None):
+        if index is None:
+            index = self._active_index
+        else:
+            self.set_active_index(index)
+
+        self._calculate_sub_indicators(True, index, index + 1)
+        self._set_reading(reading, self._active_index)
+        self._calculate_sub_indicators(False, index, index + 1)
+
+    def set_active_index(self, index: int):
+        self._active_index = index
```

### Comparing `hexital-1.0.1/hexital/core/indicator.py` & `hexital-1.1.0/hexital/core/hexital.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,362 +1,236 @@
-from __future__ import annotations
-
-from abc import ABC, abstractmethod
 from copy import deepcopy
-from dataclasses import dataclass, field
 from datetime import timedelta
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Set
 
-from hexital.analysis import movement, patterns
+from hexital.analysis import MOVEMENT_MAP, PATTERN_MAP
 from hexital.core.candle import Candle
-from hexital.core.candle_manager import CandleManager
+from hexital.core.candle_manager import DEFAULT_CANDLES, CandleManager
 from hexital.core.candlestick_type import CandlestickType
-from hexital.utils.candles import (
-    candles_sum,
-    reading_by_candle,
-    reading_count,
-    reading_period,
+from hexital.core.indicator import Indicator
+from hexital.exceptions import (
+    InvalidAnalysis,
+    InvalidIndicator,
 )
+from hexital.indicators import INDICATOR_MAP
+from hexital.utils.candles import reading_by_index
 from hexital.utils.candlesticks import validate_candlesticktype
-from hexital.utils.indexing import round_values
 from hexital.utils.timeframe import TimeFrame, validate_timeframe
 
 
-@dataclass(kw_only=True)
-class Indicator(ABC):
-    candles: List[Candle] = field(default_factory=list)
-    fullname_override: Optional[str] = None
-    name_suffix: Optional[str] = None
-    round_value: int = 4
-    timeframe: Optional[str | TimeFrame] = None
+class Hexital:
+    name: str
+    _candles: Dict[str, CandleManager]
+    _indicators: Dict[str, Indicator]
+    description: Optional[str] = None
+    timeframe: Optional[str] = None
     timeframe_fill: bool = False
     candles_lifespan: Optional[timedelta] = None
-    candlestick_type: Optional[CandlestickType | str] = None
-
-    _name: str = field(init=False, default="")
-    _output_name: str = field(init=False, default="")
-    _candles: CandleManager = field(init=False, default_factory=CandleManager)
-    _sub_indicators: List[Indicator] = field(init=False, default_factory=list)
-    _managed_indicators: Dict[str, Managed | Indicator] = field(init=False, default_factory=dict)
-    _sub_indicator: bool = field(init=False, default=False)
-    _active_index: int = field(init=False, default=0)
-    _initialised: bool = field(init=False, default=False)
-
-    def __post_init__(self):
-        self._validate_fields()
-
-        if self.timeframe is not None:
-            self.timeframe = validate_timeframe(self.timeframe)
-
-        if self.candlestick_type is not None:
-            self.candlestick_type = validate_candlesticktype(self.candlestick_type)
-
-        self._candles = CandleManager(
-            self.candles,
-            self.candles_lifespan,
-            self.timeframe,
-            self.timeframe_fill,
-            self.candlestick_type,
-        )
-
-        self.candles = self._candles.candles
-
-        self._internal_generate_name()
-
-    def __str__(self):
-        data = vars(self)
-        data.pop("candles")
-        data["name"] = data["_output_name"]
-        return str(data)
-
-    def _internal_generate_name(self):
-        name = ""
-        if self.fullname_override:
-            name = self.fullname_override
-        else:
-            name = self._generate_name()
-            if self.timeframe:
-                name += f"_{self._candles.timeframe}"
-
-        if self.name_suffix:
-            name += f"_{self.name_suffix}"
-
-        self._output_name = self._sanitise_name(name)
+    candlestick_type: Optional[CandlestickType] = None
 
-    def _initialise(self):
-        return
-
-    def _validate_fields(self):
-        return
-
-    @abstractmethod
-    def _generate_name(self) -> str:
-        ...
+    def __init__(
+        self,
+        name: str,
+        candles: List[Candle],
+        indicators: Optional[List[dict | Indicator]] = None,
+        description: Optional[str] = None,
+        timeframe: Optional[str | TimeFrame] = None,
+        timeframe_fill: bool = False,
+        candles_lifespan: Optional[timedelta] = None,
+        candlestick_type: Optional[CandlestickType | str] = None,
+    ):
+        self.name = name
+        self.description = description
+
+        if timeframe:
+            self.timeframe = validate_timeframe(timeframe)
+        self.timeframe_fill = timeframe_fill
+        self.candles_lifespan = candles_lifespan
+
+        if candlestick_type:
+            self.candlestick_type = validate_candlesticktype(candlestick_type)
+
+        self._candles = {
+            DEFAULT_CANDLES: CandleManager(
+                candles if isinstance(candles, list) else [],
+                candles_lifespan=self.candles_lifespan,
+                timeframe=self.timeframe,
+                timeframe_fill=self.timeframe_fill,
+                candlestick_type=self.candlestick_type,
+            )
+        }
+
+        self._indicators = self._validate_indicators(indicators) if indicators else {}
+
+    def _validate_indicators(self, indicators: List[dict | Indicator]) -> Dict[str, Indicator]:
+        if not indicators:
+            return {}
+
+        valid_indicators = {}
+
+        for indicator in indicators:
+            if isinstance(indicator, Indicator):
+                valid_indicators[indicator.name] = indicator
+                continue
 
-    def _sanitise_name(self, name: str) -> str:
-        return name.replace(".", ",")
+            if not isinstance(indicator, dict):
+                raise InvalidIndicator(
+                    f"Indicator type invalid 'indicator' must be a dict or Indicator type: {indicator}"
+                )
+
+            new_indicator = self._build_indicator(indicator)
+            valid_indicators[new_indicator.name] = new_indicator
+
+        for indicator in valid_indicators.values():
+            manager = CandleManager(
+                [],
+                candles_lifespan=self.candles_lifespan,
+                timeframe=indicator.timeframe if indicator.timeframe else self.timeframe,
+                timeframe_fill=self.timeframe_fill,
+                candlestick_type=self.candlestick_type,
+            )
+
+            if manager == self._candles[DEFAULT_CANDLES]:
+                indicator.candle_manager = self._candles[DEFAULT_CANDLES]
+            elif manager.name in self._candles:
+                indicator.candle_manager = self._candles[manager.name]
+            else:
+                self._candles[manager.name] = manager
+                manager.append(deepcopy(self._candles[DEFAULT_CANDLES]).candles)
+                indicator.candle_manager = self._candles[manager.name]
+
+        return valid_indicators
+
+    def _build_indicator(self, raw_indicator: dict) -> Indicator:
+        analysis_map = PATTERN_MAP | MOVEMENT_MAP
+        amorph_class = INDICATOR_MAP["Amorph"]
+
+        if raw_indicator.get("indicator"):
+            indicator_name = raw_indicator.pop("indicator")
+
+            if INDICATOR_MAP.get(indicator_name):
+                indicator_class = INDICATOR_MAP[indicator_name]
+                return indicator_class(**raw_indicator)
+            else:
+                raise InvalidIndicator(f"Indicator {indicator_name} does not exist")
+
+        elif raw_indicator.get("analysis") and isinstance(raw_indicator.get("analysis"), str):
+            analysis_name = raw_indicator.pop("analysis")
+            if not analysis_map.get(analysis_name):
+                raise InvalidAnalysis(
+                    f"analysis {analysis_name} does not exist in patterns or movements"
+                )
+
+            return amorph_class(analysis=analysis_map[analysis_name], **raw_indicator)
+
+        elif raw_indicator.get("analysis") and callable(raw_indicator.get("analysis")):
+            method_name = raw_indicator.pop("analysis")
+            return amorph_class(analysis=method_name, **raw_indicator)
+        else:
+            raise InvalidAnalysis(
+                f"Dict Indicator missing 'indicator' or 'analysis' name, not: {raw_indicator}"
+            )
+
+    def candles(self, timeframe: Optional[str] = None) -> List[Candle]:
+        if timeframe and self._candles.get(timeframe, False):
+            return self._candles[timeframe].candles
+        return self._candles[DEFAULT_CANDLES].candles
 
-    @property
-    def candle_manager(self) -> CandleManager:
-        """The Candle Manager which controls TimeFrame, Trimming and collapsing"""
-        return self._candles
-
-    @candle_manager.setter
-    def candle_manager(self, manager: CandleManager):
-        """The Candle Manager which controls TimeFrame, Trimming and collapsing,
-        this will overwrite the Manager as well as the candles"""
-        self._candles = manager
-        self.candles = manager.candles
-        self.timeframe = manager.timeframe
-        self.timeframe_fill = manager.timeframe_fill
-        self.candles_lifespan = manager.candles_lifespan
-        self.candlestick_type = manager.candlestick_type
+    def get_candles(self) -> Dict[str, List[Candle]]:
+        return {name: manager.candles for name, manager in self._candles.items()}
 
     @property
-    def name(self) -> str:
-        """The indicator name that will be saved into the Candles"""
-        return self._output_name
+    def timeframes(self) -> Set[str]:
+        return {str(manager.timeframe) for manager in self._candles.values()}
 
     @property
-    def has_reading(self) -> bool:
-        """Simple boolean to state if values are being generated yet in the candles"""
-        if len(self.candles) == 0:
-            return False
-        return self.reading(index=-1) is not None
+    def indicators(self) -> Dict[str, Indicator]:
+        """Simply get's a list of all the Indicators within Hexital strategy"""
+        return self._indicators
+
+    def indicator(self, name: str) -> Indicator:
+        """Searches hexital's indicator's and Returns the Indicator object itself."""
+        return self._indicators[name]
 
     @property
-    def settings(self) -> dict:
-        """Returns a dict format of how this indicator can be generated"""
-        output = {"indicator": self._name if self._name else type(self).__name__}
-
-        for name, value in self.__dict__.items():
-            if name == "candles":
-                continue
-            if name == "timeframe_fill" and self.timeframe is None:
-                continue
-
-            if name == "candlestick_type" and value:
-                output[name] = value.minimal_name
-            elif not name.startswith("_") and value is not None:
-                output[name] = deepcopy(value)
-
-        return output
-
-    def as_list(self, name: Optional[str] = None) -> List[float | dict | None]:
-        """Gathers the indicator for all candles as a list
-        E.G `EMA_12` OR `MACD_12_26_9.MACD`"""
-        return [reading_by_candle(candle, name if name else self.name) for candle in self.candles]
+    def indicator_settings(self) -> List[dict]:
+        """Simply get's a list of all the Indicators within Hexital strategy"""
+        return [indicator.settings for indicator in self._indicators.values()]
+
+    def has_reading(self, name: str) -> bool:
+        """Checks if the given Indicator has a valid reading in latest Candle"""
+        return bool(self.reading(name))
+
+    def reading(self, name: str, index: int = -1) -> float | dict | None:
+        """Attempts to retrieve a reading with a given Indicator name.
+        `name` can use '.' to find nested reading, E.G `MACD_12_26_9.MACD`
+        """
+        reading = reading_by_index(self._candles[DEFAULT_CANDLES].candles, name, index=index)
 
-    def _set_reading(self, reading: float | dict | None, index: Optional[int] = None):
-        index = index if index else self._active_index
+        if reading is not None:
+            return reading
 
-        if self._sub_indicator:
-            self.candles[index].sub_indicators[self.name] = reading
-        else:
-            self.candles[index].indicators[self.name] = reading
+        for candle_manager in self._candles.values():
+            reading = reading_by_index(candle_manager.candles, name, index=index)
+            if reading is not None:
+                return reading
+
+        return None
+
+    def prev_reading(self, name: str) -> float | dict | None:
+        return self.reading(name, index=-2)
+
+    def reading_as_list(self, name: str) -> List[float | dict | None]:
+        """Find given indicator and returns the readings as a list
+        Full Name of the indicator E.G `EMA_12` OR `MACD_12_26_9.MACD`"""
+        primary_name = name.split(".")[0]
+        if self._indicators.get(primary_name):
+            return self._indicators[primary_name].as_list(name)
+        return []
+
+    def add_indicator(
+        self, indicator: Indicator | List[Indicator | Dict[str, str]] | Dict[str, str]
+    ):
+        """Add's a new indicator to `Hexital` strategy.
+        This accept either `Indicator` datatypes or dict string versions to be packed.
+        `add_indicator(SMA(period=10))` or `add_indicator({"indicator": "SMA", "period": 10})`
+        Does not automatically calculates readings."""
+        indicators = indicator if isinstance(indicator, list) else [indicator]
+
+        for valid_indicator in self._validate_indicators(indicators).values():
+            self._indicators[valid_indicator.name] = valid_indicator
+
+    def remove_indicator(self, name: str):
+        """Removes an indicator from running within hexital"""
+        self.purge(name)
+        self._indicators.pop(name, None)
 
     def append(self, candles: Candle | List[Candle] | dict | List[dict] | list | List[list]):
-        self._candles.append(candles)
-        self.calculate()
-
-    def _calculate_reading(self, index: int) -> float | dict | None:
-        pass
-
-    def calculate(self):
-        """Calculate the TA values, will calculate for all the Candles,
-        where this indicator is missing"""
-        if not self._initialised:
-            self._initialise()
-            self._initialised = True
+        for candle_manager in self._candles.values():
+            candle_manager.append(candles)
 
-        for indicator in self._sub_indicators:
-            indicator.calculate()
-
-        for index in range(self._find_calc_index(), len(self.candles)):
-            self._set_active_index(index)
-
-            if self.candles[index].indicators.get(self.name) is not None:
-                continue
-
-            reading = round_values(self._calculate_reading(index=index), round_by=self.round_value)
-            self._set_reading(reading, index)
-
-    def calculate_index(self, start_index: int, end_index: Optional[int] = None):
-        """Calculate the TA values, will calculate a index range the Candles, will re-calculate"""
-        end_index = end_index if end_index else start_index + 1
-
-        for index in range(start_index, end_index):
-            self._set_active_index(index)
-            reading = round_values(self._calculate_reading(index=index), round_by=self.round_value)
-            self._set_reading(reading, index)
-
-    def _find_calc_index(self) -> int:
-        """Optimisation method, to find where to start calculating the indicator from
-        Searches from newest to oldest to find the first candle without the indicator
-        """
-        if len(self.candles) == 0 or self.name not in self.candles[0].indicators:
-            return 0
-
-        for index in range(len(self.candles) - 1, 0, -1):
-            if self.name in self.candles[index].indicators:
-                return index + 1
-            elif self.name in self.candles[index].sub_indicators:
-                return index + 1
-
-        return len(self.candles) - 1
-
-    def _set_active_index(self, index: int):
-        self._active_index = index
-
-        for indicator in self._managed_indicators.values():
-            if isinstance(indicator, Managed):
-                indicator.set_active_index(index)
-
-    def _add_sub_indicator(self, indicator: Indicator):
-        """Adds sub indicator, this will auto calculate with indicator"""
-        indicator._sub_indicator = True
-        indicator.candle_manager = self._candles
-        self._sub_indicators.append(indicator)
-
-    def _add_managed_indicator(self, name: str, indicator: Managed | Indicator):
-        """Adds managed sub indicator, this will not auto calculate with indicator"""
-        indicator._sub_indicator = True
-        indicator.candle_manager = self._candles
-        self._managed_indicators[name] = indicator
-
-    def prev_exists(self) -> bool:
-        return self.prev_reading(self.name) is not None
-
-    def prev_reading(self, name: Optional[str] = None) -> float | dict | None:
-        if len(self.candles) == 0 or self._active_index == 0:
-            return None
-        return self.reading(name=name if name else self.name, index=self._active_index - 1)
-
-    def reading(
-        self, name: Optional[str] = None, index: Optional[int] = None
-    ) -> float | dict | None:
-        """Simple method to get an indicator reading from the index
-        Name can use '.' to find nested reading, E.G 'MACD_12_26_9.MACD"""
-        return reading_by_candle(
-            self.candles[index if index is not None else self._active_index],
-            name if name else self.name,
-        )
-
-    def read_candle(self, candle: Candle, name: Optional[str] = None) -> float | dict | None:
-        """Simple method to get an indicator reading from a candle,
-        regardless of it's location"""
-        return reading_by_candle(candle, name if name else self.name)
-
-    def reading_count(self, name: Optional[str] = None) -> int:
-        """Returns how many instance of the given indicator exist"""
-        return reading_count(self.candles, name if name else self.name)
-
-    def reading_period(
-        self, period: int, name: Optional[str] = None, index: Optional[int] = None
-    ) -> bool:
-        """Will return True if the given indicator goes back as far as amount,
-        It's true if exactly or more than. Period will be period -1"""
-        return reading_period(
-            self.candles,
-            period=period,
-            name=name if name else self.name,
-            index=index if index else self._active_index,
-        )
-
-    def candles_sum(
-        self, length: int = 1, name: Optional[str] = None, index: Optional[int] = None
-    ) -> float | None:
-        return candles_sum(
-            self.candles,
-            name if name else self.name,
-            length,
-            index if index is not None else self._active_index,
-        )
-
-    def purge(self):
-        """Remove this indicator value from all Candles"""
-        self._candles.purge(
-            {self.name}
-            | {indicator.name for indicator in self._sub_indicators}
-            | {indicator.name for indicator in self._managed_indicators.values()}
-        )
-
-    def recalculate(self):
-        """Re-calculate this indicator value for all Candles"""
-        self.purge()
         self.calculate()
 
-    def rising(self, name: Optional[str] = None, length: int = 4, index: int = -1) -> bool:
-        return movement.rising(self.candles, name if name else self.name, length, index)
-
-    def falling(self, name: Optional[str] = None, length: int = 4, index: int = -1) -> bool:
-        return movement.falling(self.candles, name if name else self.name, length, index)
-
-    def mean_rising(self, name: Optional[str] = None, length: int = 4, index: int = -1) -> bool:
-        return movement.mean_rising(self.candles, name if name else self.name, length, index)
-
-    def mean_falling(self, name: Optional[str] = None, length: int = 4, index: int = -1) -> bool:
-        return movement.mean_falling(self.candles, name if name else self.name, length, index)
-
-    def highest(self, name: Optional[str] = None, length: int = 4, index: int = -1) -> float:
-        return movement.highest(self.candles, name if name else self.name, length, index)
-
-    def lowest(self, name: Optional[str] = None, length: int = 4, index: int = -1) -> float:
-        return movement.lowest(self.candles, name if name else self.name, length, index)
-
-    def highestbar(
-        self, name: Optional[str] = None, length: int = 4, index: int = -1
-    ) -> int | None:
-        return movement.highestbar(self.candles, name if name else self.name, length, index)
-
-    def lowestbar(
-        self, name: Optional[str] = None, length: int = 4, index: int = -1
-    ) -> int | None:
-        return movement.lowestbar(self.candles, name if name else self.name, length, index)
-
-    def doji(
-        self,
-        length: int = 10,
-        lookback: Optional[int] = None,
-        asint: bool = False,
-        index: Optional[int] = None,
-    ) -> bool | int:
-        return patterns.doji(
-            self.candles, length=length, lookback=lookback, asint=asint, index=index
-        )
-
-    def hammer(
-        self,
-        length: int = 10,
-        lookback: Optional[int] = None,
-        asint: bool = False,
-        index: Optional[int] = None,
-    ) -> bool | int:
-        return patterns.hammer(
-            self.candles, length=length, lookback=lookback, asint=asint, index=index
-        )
-
-
-@dataclass(kw_only=True)
-class Managed(Indicator):
-    """Managed
-
-    Empty Indicator thats manually controlled and the reading manually set.
-
-    """
-
-    indicator_name: str = "MAN"
-    _sub_indicator: bool = True
-    _active_index: int = 0
-
-    def _generate_name(self) -> str:
-        return self.indicator_name
-
-    def set_reading(self, reading: float | dict, index: Optional[int] = None):
-        if index is None:
-            index = self._active_index
-        else:
-            self.set_active_index(index)
-        self._set_reading(reading, self._active_index)
-
-    def set_active_index(self, index: int):
-        self._active_index = index
+    def purge(self, name: Optional[str] = None):
+        """Takes Indicator name and removes all readings for said indicator.
+        Indicator name must be exact"""
+        for indicator_name, indicator in self._indicators.items():
+            if name is None or (name and name in indicator_name):
+                indicator.purge()
+
+    def calculate(self, name: Optional[str] = None):
+        """Calculates all the missing indicator readings."""
+        for indicator_name, indicator in self._indicators.items():
+            if name is None or indicator_name == name:
+                indicator.calculate()
+
+    def calculate_index(self, name: Optional[str] = None, index: int = -1):
+        """Calculate specific index for all or specific indicator readings."""
+        for indicator_name, indicator in self._indicators.items():
+            if name is None or indicator_name == name:
+                indicator.calculate_index(index)
+
+    def recalculate(self, name: Optional[str] = None):
+        """Purge's all indicator reading's and re-calculates them all,
+        ideal for changing an indicator parameters midway."""
+        self.purge(name)
+        self.calculate(name)
```

### Comparing `hexital-1.0.1/hexital/exceptions.py` & `hexital-1.1.0/hexital/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,24 +14,14 @@
 
 
 class InvalidCandleOrder(Exception):
     def __init__(self, message):
         super().__init__(message)
 
 
-class MixedTimeframes(Exception):
-    def __init__(self, message):
-        super().__init__(message)
-
-
-class MissingIndicator(Exception):
-    def __init__(self, message):
-        super().__init__(message)
-
-
 class CandleAlreadyTagged(Exception):
     def __init__(self, message):
         super().__init__(message)
 
 
 class InvalidCandlestickType(Exception):
     def __init__(self, message):
```

### Comparing `hexital-1.0.1/hexital/indicators/__init__.py` & `hexital-1.1.0/hexital/indicators/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,53 @@
 from .adx import ADX
 from .amorph import Amorph
+from .aroon import AROON
 from .atr import ATR
+from .bbands import BBANDS
+from .counter import Counter
+from .donchian import Donchian
 from .ema import EMA
 from .hla import HighLowAverage
+from .hma import HMA
 from .kc import KC
 from .macd import MACD
 from .obv import OBV
 from .rma import RMA
 from .roc import ROC
 from .rsi import RSI
 from .sma import SMA
+from .stdev import STDEV
 from .stoch import STOCH
 from .supertrend import Supertrend
 from .tr import TR
+from .tsi import TSI
 from .vwap import VWAP
 from .vwma import VWMA
 from .wma import WMA
 
 INDICATOR_MAP = {
     "Amorph": Amorph,
+    "Counter": Counter,
+    "aroon": AROON,
     "ADX": ADX,
     "ATR": ATR,
+    "BBANDS": BBANDS,
+    "donchian": Donchian,
     "EMA": EMA,
     "HLA": HighLowAverage,
+    "HMA": HMA,
     "KC": KC,
     "MACD": MACD,
     "OBV": OBV,
     "RMA": RMA,
     "ROC": ROC,
     "RSI": RSI,
     "SMA": SMA,
+    "STDEV": STDEV,
     "STOCH": STOCH,
     "Supertrend": Supertrend,
     "TR": TR,
+    "TSI": TSI,
     "VWAP": VWAP,
     "VWMA": VWMA,
     "WMA": WMA,
 }
```

### Comparing `hexital-1.0.1/hexital/indicators/adx.py` & `hexital-1.1.0/hexital/indicators/adx.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,89 +31,71 @@
         return f"{self._name}_{self.period}_{self.period_signal}"
 
     def _validate_fields(self):
         if self.period_signal is None:
             self.period_signal = self.period
 
     def _initialise(self):
-        self._add_sub_indicator(
+        self.add_sub_indicator(
             ATR(
                 period=self.period,
-                fullname_override=f"{self._name}_atr",
+                fullname_override=f"{self.name}_atr",
             )
         )
-        self._add_managed_indicator(
-            "positive",
+        data_indicator = Managed(fullname_override=f"{self.name}_data")
+        self.add_managed_indicator("ADX_data", data_indicator)
+
+        data_indicator.add_sub_indicator(
             RMA(
-                fullname_override=f"{self._name}_pos",
+                fullname_override=f"{self.name}_pos",
                 period=self.period,
-                input_value=f"{self._name}_ppos",
-            ),
-        )
-        self._add_managed_indicator(
-            "plain_positive",
-            Managed(
-                fullname_override=f"{self._name}_ppos",
+                input_value=f"{self.name}_data.pos",
             ),
+            False,
         )
-        self._add_managed_indicator(
-            "negative",
+        data_indicator.add_sub_indicator(
             RMA(
-                fullname_override=f"{self._name}_neg",
+                fullname_override=f"{self.name}_neg",
                 period=self.period,
-                input_value=f"{self._name}_pneg",
-            ),
-        )
-        self._add_managed_indicator(
-            "plain_negative",
-            Managed(
-                fullname_override=f"{self._name}_pneg",
+                input_value=f"{self.name}_data.neg",
             ),
+            False,
         )
-
-        self._add_managed_indicator(
+        self.add_managed_indicator(
             "dx",
             RMA(
-                fullname_override=f"{self._name}_dx",
+                fullname_override=f"{self.name}_dx",
                 period=self.period_signal,
-                input_value=f"{self._name}_pdx",
-            ),
-        )
-        self._add_managed_indicator(
-            "plain_dx",
-            Managed(
-                fullname_override=f"{self._name}_pdx",
+                input_value=f"{self.name}_data.dx",
             ),
         )
 
     def _calculate_reading(self, index: int) -> float | dict | None:
         adx_final = None
         adx_positive = None
         adx_negative = None
 
         if self.reading("high"):
             up = self.reading("high") - self.reading("high", index - 1)
             down = self.reading("low", index - 1) - self.reading("low")
 
             positive = up if up > down and up > 0 else 0
             negative = down if down > up and down > 0 else 0
+            self.managed_indicators["ADX_data"].set_reading({"pos": positive, "neg": negative})
 
-            self._managed_indicators["plain_positive"].set_reading(positive)
-            self._managed_indicators["plain_negative"].set_reading(negative)
-            self._managed_indicators["positive"].calculate_index(index)
-            self._managed_indicators["negative"].calculate_index(index)
-
-            if self.reading(f"{self._name}_atr") and self.reading(f"{self._name}_pos"):
-                mod = 100 / self.reading(f"{self._name}_atr")
+            if self.reading(f"{self.name}_atr") and self.reading(f"{self.name}_pos"):
+                mod = 100 / self.reading(f"{self.name}_atr")
 
-                adx_positive = mod * self.reading(f"{self._name}_pos")
-                adx_negative = mod * self.reading(f"{self._name}_neg")
+                adx_positive = mod * self.reading(f"{self.name}_pos")
+                adx_negative = mod * self.reading(f"{self.name}_neg")
 
                 dx = 100 * abs(adx_positive - adx_negative) / (adx_positive + adx_negative)
 
-                self._managed_indicators["plain_dx"].set_reading(dx)
-                self._managed_indicators["dx"].calculate_index(index)
+                self.managed_indicators["ADX_data"].set_reading(
+                    {"pos": positive, "neg": negative, "dx": dx}
+                )
+                self.managed_indicators["dx"].calculate_index(index)
 
-                if self.reading(f"{self._name}_dx"):
-                    adx_final = self.reading(f"{self._name}_dx")
+                if self.reading(f"{self.name}_dx"):
+                    adx_final = self.reading(f"{self.name}_dx")
 
         return {"ADX": adx_final, "DM_Plus": adx_positive, "DM_Neg": adx_negative}
```

### Comparing `hexital-1.0.1/hexital/indicators/amorph.py` & `hexital-1.1.0/hexital/indicators/amorph.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.1/hexital/indicators/atr.py` & `hexital-1.1.0/hexital/indicators/atr.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,16 +23,17 @@
     _name: str = field(init=False, default="ATR")
     period: int = 14
 
     def _generate_name(self) -> str:
         return f"{self._name}_{self.period}"
 
     def _initialise(self):
-        self._add_sub_indicator(TR(candles=self.candles))
+        self.add_sub_indicator(TR())
 
     def _calculate_reading(self, index: int) -> float | dict | None:
         if self.prev_exists():
             return (self.prev_reading() * (self.period - 1) + self.reading("TR")) / self.period
 
         if self.reading_period(self.period, "TR"):
             return self.candles_sum(self.period, "TR") / self.period
+
         return None
```

### Comparing `hexital-1.0.1/hexital/indicators/ema.py` & `hexital-1.1.0/hexital/indicators/ema.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.1/hexital/indicators/kc.py` & `hexital-1.1.0/hexital/indicators/kc.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,44 +18,44 @@
     multiplier: float = 2.0
     input_value: str = "close"
 
     def _generate_name(self) -> str:
         return f"{self._name}_{self.period}_{self.multiplier}"
 
     def _initialise(self):
-        self._add_sub_indicator(
+        self.add_sub_indicator(
             ATR(
                 period=self.period,
-                fullname_override=f"{self._name}_ATR",
+                fullname_override=f"{self.name}_ATR",
             )
         )
 
-        self._add_sub_indicator(
+        self.add_sub_indicator(
             EMA(
                 input_value=self.input_value,
                 period=self.period,
-                fullname_override=f"{self._name}_EMA",
+                fullname_override=f"{self.name}_EMA",
             )
         )
 
     def _calculate_reading(self, index: int) -> float | dict | None:
         if not all(
             [
-                self.reading(f"{self._name}_EMA"),
-                self.reading(f"{self._name}_ATR"),
+                self.reading(f"{self.name}_EMA"),
+                self.reading(f"{self.name}_ATR"),
             ]
         ):
             return {"lower": None, "band": None, "upper": None}
 
-        lower = self.reading(f"{self._name}_EMA") - (
-            self.multiplier * self.reading(f"{self._name}_ATR")
+        lower = self.reading(f"{self.name}_EMA") - (
+            self.multiplier * self.reading(f"{self.name}_ATR")
         )
 
-        upper = self.reading(f"{self._name}_EMA") + (
-            self.multiplier * self.reading(f"{self._name}_ATR")
+        upper = self.reading(f"{self.name}_EMA") + (
+            self.multiplier * self.reading(f"{self.name}_ATR")
         )
 
         return {
             "lower": lower,
-            "band": self.reading(f"{self._name}_EMA"),
+            "band": self.reading(f"{self.name}_EMA"),
             "upper": upper,
         }
```

### Comparing `hexital-1.0.1/hexital/indicators/macd.py` & `hexital-1.1.0/hexital/indicators/macd.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,48 +39,49 @@
         )
 
     def _validate_fields(self):
         if self.slow_period < self.fast_period:
             self.fast_period, self.slow_period = self.slow_period, self.fast_period
 
     def _initialise(self):
-        self._add_sub_indicator(
+        self.add_sub_indicator(
             EMA(
                 input_value=self.input_value,
                 period=self.fast_period,
-                fullname_override=f"{self._name}_EMA_fast",
+                fullname_override=f"{self.name}_EMA_fast",
             )
         )
-        self._add_sub_indicator(
+        self.add_sub_indicator(
             EMA(
                 input_value=self.input_value,
                 period=self.slow_period,
-                fullname_override=f"{self._name}_EMA_slow",
+                fullname_override=f"{self.name}_EMA_slow",
             )
         )
 
-        self._add_managed_indicator(
+        self.add_managed_indicator(
             "signal",
             EMA(
                 input_value=f"{self.name}.MACD",
                 period=self.signal_period,
-                fullname_override=f"{self._name}_signal_line",
+                fullname_override=f"{self.name}_signal_line",
             ),
         )
 
     def _calculate_reading(self, index: int) -> float | dict | None:
-        if self.reading(f"{self._name}_EMA_slow"):
-            macd = self.reading(f"{self._name}_EMA_fast") - self.reading(f"{self._name}_EMA_slow")
+        macd = None
+        signal = None
+        histogram = None
+
+        if self.reading(f"{self.name}_EMA_slow"):
+            macd = self.reading(f"{self.name}_EMA_fast") - self.reading(f"{self.name}_EMA_slow")
 
             # Temp manually inserting MACD to be used by signal EMA calc
             self.candles[index].indicators[self.name] = {"MACD": macd}
-            self._managed_indicators["signal"].calculate_index(index)
+            self.managed_indicators["signal"].calculate_index(index)
 
-            signal = self._managed_indicators["signal"].reading()
+            signal = self.managed_indicators["signal"].reading()
 
-            histogram = None
             if macd is not None and signal is not None:
                 histogram = macd - signal
 
-            return {"MACD": macd, "signal": signal, "histogram": histogram}
-
-        return {"MACD": None, "signal": None, "histogram": None}
+        return {"MACD": macd, "signal": signal, "histogram": histogram}
```

### Comparing `hexital-1.0.1/hexital/indicators/obv.py` & `hexital-1.1.0/hexital/indicators/obv.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.1/hexital/indicators/rma.py` & `hexital-1.1.0/hexital/indicators/rma.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.1/hexital/indicators/roc.py` & `hexital-1.1.0/hexital/indicators/roc.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.1/hexital/indicators/rsi.py` & `hexital-1.1.0/hexital/indicators/rsi.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,49 +24,50 @@
     period: int = 14
     input_value: str = "close"
 
     def _generate_name(self) -> str:
         return f"{self._name}_{self.period}"
 
     def _initialise(self):
-        self._add_managed_indicator(
-            "RSI_gain",
-            Managed(indicator_name="RSI_gain", candles=self.candles),
-        )
-        self._add_managed_indicator(
-            "RSI_loss",
-            Managed(indicator_name="RSI_loss", candles=self.candles),
-        )
+        self.add_managed_indicator("RSI_data", Managed(fullname_override=f"{self.name}_data"))
 
     def _calculate_reading(self, index: int) -> float | dict | None:
         if self.prev_exists():
             change = self.prev_reading(self.input_value) - self.reading(self.input_value)
 
             change_gain = -1 * change if change < 0 else 0.0
             change_loss = change if change > 0 else 0.0
 
-            self._managed_indicators["RSI_gain"].set_reading(
-                ((self.prev_reading("RSI_gain") * (self.period - 1)) + change_gain) / self.period,
-            )
-            self._managed_indicators["RSI_loss"].set_reading(
-                ((self.prev_reading("RSI_loss") * (self.period - 1)) + change_loss) / self.period,
+            self.managed_indicators["RSI_data"].set_reading(
+                {
+                    "gain": (
+                        (self.prev_reading(f"{self.name}_data.gain") * (self.period - 1))
+                        + change_gain
+                    )
+                    / self.period,
+                    "loss": (
+                        (self.prev_reading(f"{self.name}_data.loss") * (self.period - 1))
+                        + change_loss
+                    )
+                    / self.period,
+                }
             )
+
         elif self.reading_period(self.period + 1, self.input_value):
             changes = [
                 self.reading(self.input_value, i) - self.reading(self.input_value, i - 1)
                 for i in range(index - (self.period - 1), index + 1)
             ]
-            self._managed_indicators["RSI_gain"].set_reading(
-                sum(chng for chng in changes if chng > 0) / self.period,
-            )
-            self._managed_indicators["RSI_loss"].set_reading(
-                sum(abs(chng) for chng in changes if chng < 0) / self.period,
+            self.managed_indicators["RSI_data"].set_reading(
+                {
+                    "gain": sum(chng for chng in changes if chng > 0) / self.period,
+                    "loss": sum(abs(chng) for chng in changes if chng < 0) / self.period,
+                }
             )
 
-        if self.reading("RSI_gain"):
-            rs = self.reading("RSI_gain") / self.reading("RSI_loss")
+        if self.reading(f"{self.name}_data"):
+            rs = self.reading(f"{self.name}_data.gain") / self.reading(f"{self.name}_data.loss")
             rsi = 100.0 - (100.0 / (1.0 + rs))
             return rsi
 
-        self._managed_indicators["RSI_gain"].set_reading(None)
-        self._managed_indicators["RSI_loss"].set_reading(None)
+        self.managed_indicators["RSI_data"].set_reading(None)
         return None
```

### Comparing `hexital-1.0.1/hexital/indicators/sma.py` & `hexital-1.1.0/hexital/indicators/sma.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.1/hexital/indicators/stoch.py` & `hexital-1.1.0/hexital/indicators/stoch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass, field
 
-from hexital.core.indicator import Indicator
+from hexital.core.indicator import Indicator, Managed
 from hexital.indicators.sma import SMA
 
 
 @dataclass(kw_only=True)
 class STOCH(Indicator):
     """Stochastic (STOCH)
 
@@ -39,46 +39,48 @@
     def _generate_name(self) -> str:
         return f"{self._name}_{self.period}"
 
     def _validate_fields(self):
         return
 
     def _initialise(self):
-        self._add_managed_indicator(
-            "k",
+        self.add_managed_indicator("STOCH_data", Managed(fullname_override=f"{self.name}_data"))
+        self.managed_indicators["STOCH_data"].add_sub_indicator(
             SMA(
-                input_value=f"{self.name}.stoch",
+                input_value=f"{self.name}_data.stoch",
                 period=self.smoothing_k,
-                fullname_override=f"{self._name}_k",
+                fullname_override=f"{self.name}_k",
             ),
+            False,
         )
-        self._add_managed_indicator(
-            "d",
+        self.add_managed_indicator(
+            "STOCH_d",
             SMA(
-                input_value=f"{self.name}.k",
+                input_value=f"{self.name}_data.k",
                 period=self.slow_period,
-                fullname_override=f"{self._name}_d",
+                fullname_override=f"{self.name}_d",
             ),
         )
 
     def _calculate_reading(self, index: int) -> float | dict | None:
+        stoch = None
+        k = None
+        d = None
+
         if self.reading_period(self.period, self.input_value):
             lowest = min(
                 self.reading("low", i) for i in range(index - (self.period - 1), index + 1)
             )
             highest = max(
                 self.reading("high", i) for i in range(index - (self.period - 1), index + 1)
             )
 
             stoch = ((self.reading(self.input_value) - lowest) / (highest - lowest)) * 100
 
-            self.candles[index].indicators[self.name] = {"stoch": stoch}
-            self._managed_indicators["k"].calculate_index(index)
-            k = self.reading(f"{self._name}_k")
-
-            self.candles[index].indicators[self.name] = {"stoch": stoch, "k": k}
-            self._managed_indicators["d"].calculate_index(index)
-            d = self.reading(f"{self._name}_d")
+            self.managed_indicators["STOCH_data"].set_reading({"stoch": stoch})
+            k = self.reading(f"{self.name}_k")
 
-            return {"stoch": stoch, "k": k, "d": d}
+            self.managed_indicators["STOCH_data"].set_reading({"stoch": stoch, "k": k})
+            self.managed_indicators["STOCH_d"].calculate_index(index)
+            d = self.reading(f"{self.name}_d")
 
-        return {"stoch": None, "k": None, "d": None}
+        return {"stoch": stoch, "k": k, "d": d}
```

### Comparing `hexital-1.0.1/hexital/indicators/tr.py` & `hexital-1.1.0/hexital/indicators/tr.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def _generate_name(self) -> str:
         return self._name
 
     def _calculate_reading(self, index: int) -> float | dict | None:
         high = self.reading("high")
         low = self.reading("low")
 
-        if index > 0:
+        if self.reading_period(2, "close"):
             close = self.prev_reading("close")
             return max(
                 high - low,
                 abs(high - close),
                 abs(low - close),
             )
```

### Comparing `hexital-1.0.1/hexital/indicators/vwma.py` & `hexital-1.1.0/hexital/indicators/vwma.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.1/hexital/indicators/wma.py` & `hexital-1.1.0/hexital/indicators/wma.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.1/hexital/utils/candles.py` & `hexital-1.1.0/hexital/utils/candles.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,23 +23,23 @@
         if reading is not None:
             return reading
 
     if getattr(candle, name, None) is not None:
         return getattr(candle, name)
 
     for key, reading in chain(candle.indicators.items(), candle.sub_indicators.items()):
-        if name in key:
+        if key == name:
             return reading
 
     return None
 
 
 def _nested_indicator(candle: Candle, name: str, nested_name: str) -> float | None:
     for key, reading in chain(candle.indicators.items(), candle.sub_indicators.items()):
-        if name in key:
+        if key == name:
             return reading.get(nested_name) if isinstance(reading, dict) else reading
 
     return None
 
 
 def reading_count(candles: List[Candle], name: str) -> int:
     """Returns how many instance of the given indicator exist"""
```

### Comparing `hexital-1.0.1/hexital/utils/candlesticks.py` & `hexital-1.1.0/hexital/utils/candlesticks.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.1/hexital/utils/indexing.py` & `hexital-1.1.0/hexital/utils/indexing.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.1/hexital/utils/timeframe.py` & `hexital-1.1.0/hexital/utils/timeframe.py`

 * *Files identical despite different names*

### Comparing `hexital-1.0.1/pyproject.toml` & `hexital-1.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hexital"
-version = "1.0.1"
+version = "1.1.0"
 description = "Hex Incremental Technical Analysis Library"
 readme = "README.md"
 license = "MIT"
 authors = ["Merlin Roe <merlin.roe@hotmail.co.uk>"]
 homepage = "https://github.com/MerlinR/Hexital"
 repository = "https://github.com/MerlinR/Hexital"
 documentation = "https://github.com/MerlinR/Hexital"
@@ -21,34 +21,34 @@
 ]
 include = ["CHANGELOG.md"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
-coverage = "*"
-pytest = "*"
-pytest-cov = "*"
-deepdiff = "*"
+coverage = "^7.4.4"
+pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
+deepdiff = "^7.0.1"
 
 [tool.poetry.group.truth]
 optional = true
 
 [tool.poetry.group.truth.dependencies]
-pandas = "^1.2.0"
-numpy = "^1.22.0"
+pandas = "^2.2.2"
+numpy = "^1.26.4"
 ta-lib = "*"
 pandas-ta = { git = "https://github.com/twopirllc/pandas-ta.git#develop" }
 
 [tool.poetry.group.speed_tests]
 optional = true
 
 [tool.poetry.group.speed_tests.dependencies]
-matplotlib = "*"
-pandas = "^1.2.0"
-numpy = "^1.22.0"
-ta-lib = "*"
+matplotlib = "^3.8.4"
+pandas = "^2.2.2"
+numpy = "^1.26.4"
+ta-lib = "^0.4.28"
 pandas-ta = { git = "https://github.com/twopirllc/pandas-ta.git#develop" }
 
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hexital-1.0.1/PKG-INFO` & `hexital-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexital
-Version: 1.0.1
+Version: 1.1.0
 Summary: Hex Incremental Technical Analysis Library
 Home-page: https://github.com/MerlinR/Hexital
 License: MIT
 Keywords: trading,quant,indicators
 Author: Merlin Roe
 Author-email: merlin.roe@hotmail.co.uk
 Requires-Python: >=3.10,<4.0
@@ -20,109 +20,147 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Project-URL: Documentation, https://github.com/MerlinR/Hexital
 Project-URL: Repository, https://github.com/MerlinR/Hexital
 Description-Content-Type: text/markdown
 
 # Hexital - Incremental Technical Analysis Library
+
 [![license](https://img.shields.io/github/license/merlinr/hexital)](#license)
 [![Python Version](https://img.shields.io/pypi/pyversions/hexital?style=flat)](https://pypi.org/project/hexital/)
 [![PyPi Version](https://img.shields.io/pypi/v/hexital?style=flat)](https://pypi.org/project/hexital/)
 [![Package Status](https://img.shields.io/pypi/status/hexital?style=flat)](https://pypi.org/project/hexital/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/hexital?color=%2332c955)
+![GitHub Repo stars](https://img.shields.io/github/stars/MerlinR/Hexital?style=flat)
 [![Unit Tests - Master](https://github.com/MerlinR/Hexital/actions/workflows/unit_test.yaml/badge.svg?branch=master)](https://github.com/MerlinR/Hexital/actions/workflows/unit_test.yaml)
 [![Unit Tests - Dev](https://github.com/MerlinR/Hexital/actions/workflows/unit_test.yaml/badge.svg?branch=development)](https://github.com/MerlinR/Hexital/actions/workflows/unit_test.yaml)
 
 # `Beta`
-Note: Hexital has entered Beta mode, being all Major features are implemented and not expected to have drastic changes. Future changes would include bug fixes, QOL additions and implementation of new Indicators, Candlestick patterns, movements and Candlestick types.
+
+Note: Hexital is in Beta, all Major features are implemented and not expected to have drastic changes.
 
 # Hexital
-`Hexital` is a Python library implementing financial indicators for technical analysis. The distinctive feature of the library is its incremental computation of indicators which is designed to fit real-time applications or applications with iterative input in general.
 
-For most libraries such as [Pandas-TA](https://github.com/twopirllc/pandas-ta) which is fantastic for generating Indicators for a large set of data, it's incredibly slow when computing real-time/incremental data sets. The entire input vector is always used to calculate new values of indicators, which is a major cause of this speed issue. Despite the fact that these indicator values will remain unchanged and/or you don't want past data points to be changed by new data. `Hexital` resolves this by using an incremental approach, only calculating new/missing indicator value's, this implies it requires O(1) time to produce new indicator values in comparison to O(n) (or worse) required by other libraries.
+`Hexital` is a Python library designed for technical analysis in financial markets, offering a range of indicators commonly used in trading strategies. What sets Hexital apart is its innovative approach to computation, specifically tailored for real-time or iterative applications.
+
+While libraries like [Pandas-TA](https://github.com/twopirllc/pandas-ta) excel at generating indicators for large datasets, they often struggle with real-time or incremental data processing due to their reliance on recalculating the entire input vector. This inefficiency can significantly impact speed, as each new data point triggers a full recalculation of all indicators.
 
+`Hexital` addresses this issue by employing an incremental computation method. Rather than reevaluating all data points, it selectively computes only the new or missing indicator values. This optimized approach ensures that generating new indicator values requires constant time complexity O(1), a stark contrast to the linear time complexity (O(n)) or worse exhibited by other libraries.
+
+With Hexital, users can enjoy swift and efficient computation of indicators, making it ideal for applications requiring real-time analysis or iterative data processing.
 
 ## Features
 
 ### Indicators
-Hexital comes with a growing selection of available Indicators to compute. These can be used individually to calculate a single indicator, or used with the `Hexital` class to automatically compute multiple indicators with an incremental candle list; which is easily parsable.
+
+Hexital offers a diverse range of indicators for technical analysis. These can be utilized individually to compute a single indicator or, with the Hexital class, multiple indicators can be automatically calculated using an incremental candle list, which is easily parsed.
 
 ### Candlestick Patterns
-Hexital also supports detecting candle patterns, such as Doji, etc. This can be achieved easily by calling the Pattern function with the candles, or used automatically as an indicator where it would be computed alongside Indicators.
+
+Hexital supports the detection of candle patterns, such as Doji, among others. This functionality can be easily accessed by calling the Pattern function with the candle data, or it can be automatically computed alongside other indicators.
 
 ### Candlestick Types
-Hexital also has the feature to automatically convert Candlesticks from the standard type into alternative formats, such as 'Heikin-Ashi'. This will mean prior to generating indicators it will automatically convert the Candlesticks to the desired type and then calculate indicators on this new candlestick type. This works in conjunction with all other features.
+
+Hexital provides the capability to automatically convert candlesticks from the standard type into alternative formats, such as 'Heikin-Ashi'. Prior to generating indicators, candlesticks are automatically converted to the desired type, enabling indicator calculations on this new candlestick type. This feature seamlessly integrates with all other functionalities.
 
 ### Multi-Timeframes
-Hexital has a key feature of supporting indicator and pattern computation on multiple candle timeframes with a single set of candles. For instance an indicator can be given second candlesticks and can calculate EMA on 1m candlesticks or 10m candlesticks, the indicator will automatically merge these candles into the required timeframes and compute the indicator value. * Cant go down, for obv reasons.
 
-This can also be mixed within the `Hexital` class, allowing you to automatically compute a multiple incremental indictors and patterns of which consistent of multiple timeframes by appending a single candle of any timeframe. E.G By appending 1m candles  into `Hexital` you can automatically compute an RSI using the 5 minute candles and computing an EMA using the 10 minute candles, at the same time automatically while only adding 1m candlesticks.
+Hexital boasts a key feature of supporting indicator and pattern computation on multiple candle timeframes using a single set of candles. For example, an indicator can be applied to second candlesticks to calculate EMA on 1m or 10m candlesticks. The indicator automatically merges these candles into the required timeframes and computes the indicator value.
+
+This functionality can also be leveraged within the `Hexital` class, enabling the automatic computation of multiple incremental indicators and patterns across multiple timeframes by appending a single candle of any timeframe. For instance, by appending 1m candles into Hexital, you can automatically compute an RSI using 5-minute candles and an EMA using 10-minute candles, all while only adding 1m candlesticks.
 
 Example:
+
 ```python
 stratergy = Hexital("Test Stratergy", candlesticks_1m, [RSI(timeframe="T5"), EMA(timeframe=TimeFrame.MINUTE10)])
 ```
 
 ### Candlestick Movements
-Hexital also comes built with some candle utility methods, to easily take the candles list and detect movements such as Rising Candles, indicator Cross overs, etc, these are designed to be simple to make using the candles and common features easy,  many of these are also found in pine scripting. 
+
+Hexital includes built-in candle utility methods for detecting movements such as Rising Candles and indicator crossovers. These methods are designed to simplify the process of analyzing candle data and common features. Many of these functionalities are inspired by those found in Pine Scripting.
 
 ## Indicators
-- ADX
-- ATR
-- KC
-- EMA
-- HighLowAverage
-- MACD
-- OBV
-- RMA
-- RSI
-- ROC
-- SMA
-- STOCH
+
+- Average Directional Index(ADX)
+- Aroon
+- Average True Range (ATR)
+- Bollinger Bands (BBANDS)
+- Counter
+- Donchian Channels (donchian)
+- Exponential Moving Average (EMA)
+- High Low Average
+- Hull Moving Average (HMA)
+- Keltner Channel (KC)
+- Moving Average Convergence/Divergence (MACD)
+- On Balance Volume (OBV)
+- Relative Moving Average (RMA)
+- Rate of Change (ROC)
+- Relative strength index (RSI)
+- Simple Moving Average(SMA)
+- Standard Deviation (STDEV)
+- Stochastic Oscillator (STOCH)
 - Supertrend
-- TR
-- VWAP
-- VWMA
-- WMA
+- True Range (TR)
+- True Strength Index (TSI)
+- Volume Weighted Average Price (VWAP)
+- Volume Weighed Moving Averge (VWMA)
+- Weighed Moving Average (WMA)
 
 ## Candlestick Patterns
+
 Simple useful Candle pattern recognition, such as Doji, hammer, etc
+
 - Doji
+- Dojistar
 - Hammer
+- Inverted Hammer
 
 ## Candlestick Types
+
 Hexital can also automatically convert Candlesticks into specific types, such as:
+
 - Heikin-Ashi
 
 ## Candlestick Movements
+
 Simple useful Candle Anaylsis methods such as those in [Pine Scripting](https://www.tradingview.com/pine-script-reference/v5/)
+
 - Positive/Negative Candle
 - Rising/Falling Indicator
 - Mean Based Rising/Falling Indicator
 - Highest/Lowest Indicator (Value)
 - HighestBar/LowestBar Indicator (Offset how far back)
 - Indicator Cross
 - Indicator CrossOver/CrossUnder
 
 ## Installation
+
 ### Stable
+
 Pip and pypi package version is the latest stable version.
+
 ```bash
 pip install hexital
 ```
+
 ## Latest
+
 In case you want to install the latest development version from the repo.
+
 ```bash
 pip install git+https://github.com/merlinr/hexital.git@development
 ```
 
 ## Usage
 
 ### Single Indicator
+
 ```python
 from hexital import EMA, Candle
+from hexital.analysis import movement
 import pandas as pd
 
 my_candles = [
     {"open": 17213, "high": 2395, "low": 7813, "close": 3615, "volume": 19661},
     {"open": 1301, "high": 3007, "low": 11626, "close": 19048, "volume": 28909},
     {"open": 12615, "high": 923, "low": 7318, "close": 1351, "volume": 33765},
     {"open": 1643, "high": 16229, "low": 17721, "close": 212, "volume": 3281},
@@ -135,93 +173,82 @@
 ]
 # Convert Basic candles
 candles = Candle.from_dicts(my_candles)
 # Or directly from a Numpy Dataframe
 # df = pd.read_csv("path/to/symbol.csv", sep=",")
 # candles = Candle.from_dicts(df.to_dict("records"))
 
-my_ema = EMA(candles=candles, period=3)
-my_ema.calculate()
-
-# Indicator name is generated based on Indicator and parameters
-print(my_ema.name) # EMA_3
-
-# Check if started generating Readings
-print(my_ema.has_reading) # True
-
-# Get EMA indicator readings
-# Latest
-print(my_ema.reading()) # 8408.7552
-# All
-print(my_ema.as_list()) # [None, None, 8004.6667, 4108.3333, 5708.1667, 7063.0833, 12414.0416, 15606.0208, 8518.5104, 8408.7552]
+print("Indicator name:", my_ema.name)  # EMA_3
+print("Has reading:", my_ema.has_reading)  # True
+print("Latest EMA reading:", my_ema.reading())  # 8408.7552
+print("All EMA readings:", my_ema.as_list())
+# [None, None, 8004.6667, 4108.3333, 5708.1667, 7063.0833, 12414.0416, 15606.0208, 8518.5104, 8408.7552]
 
 # Add new
 my_ema.append(Candle.from_dict({'open': 19723, 'high': 4837, 'low': 11631, 'close': 6231, 'volume': 38993}))
-print(my_ema.as_list()) # [None, None, 8004.6667, 4108.3333, 5708.1667, 7063.0833, 12414.0416, 15606.0208, 8518.5104, 8408.7552, 7319.8776]
+print("EMA readings after appending new candle:", my_ema.as_list())
+ # [None, None, 8004.6667, 4108.3333, 5708.1667, 7063.0833, 12414.0416, 15606.0208, 8518.5104, 8408.7552, 7319.8776]
 
 # Check Reading and Prev Reading
-print(my_ema.reading()) # 7319.8776
-print(my_ema.prev_reading()) # 8408.7552
+print("EMA reading:", my_ema.reading())  # 7319.8776
+print("Previouse EMA reading:", my_ema.prev_reading())  # 8408.7552
 
 # How many EMA readings been generated
 print(my_ema.reading_count()) # 9
 
 # Purge Readings
 my_ema.purge()
-print(my_ema.reading()) # None
-
-# Purge and Re-calculate
+print("EMA reading after purging:", my_ema.reading())  # None
 my_ema.recalculate()
-print(my_ema.reading()) # 7319.8776
+print("EMA reading after recalculation:", my_ema.reading())  # 7319.8776
 
 # Recalculate latest
 my_ema.calculate_index("EMA_3")
 
-# Access other Readings (Reading get's the latest readings)
-print(my_ema.reading("high")) # 4837
+# Access specific readings
+print("Latest high reading:", my_ema.reading("high"))  # 4837
+print("High reading at index -2:", my_ema.reading("high", index=-2))  # 6584
 
-# Access other specific Readings (Older readings)
-print(my_ema.reading("high", index=-2)) # 6584
-
-# Easily view candlestick trends
-print(my_ema.falling()) # True
 ```
 
-
 ## Upcoming Features
 
 Roughly ordered in priority
 
-- Modular framework (like indicators) to repaint candles, E.G as Renko, Range, etc 
 - More Indicators
 - More Movement methods
 - More Patterns
 - Indicator Pluggability, to allow easy extension of this library
-  - Allowing custom Indictors to be added
+  - Allowing easier custom Indictors to be added
 - Multiprocessing, of indictors stored within hexial Class.
   - Likely wont see increase in performance
 
-
 ## Testing
-Testing is a huge part of this library as it's incredibly difficult to ensure the accuracy of the indicator values being generated. In order to solve this this I rely on [Pandas-TA](https://github.com/twopirllc/pandas-ta) as my source of truth for the indicator values. Each indicator added to this library requires a test that uses the Pandas-TA lib indicator output as the expected result. Due to some difference's in the calculations done withinin Numpy, not all values are exactly identical, therefore if there are differences outside of the given 1 decimal place, than a pearson correlation coefficient is calculated to ensure correct correlation with the givne output.
+
+Testing is a critical aspect of this library due to the complexity of ensuring the accuracy of generated indicator values. To achieve this, I rely on [Pandas-TA](https://github.com/twopirllc/pandas-ta) as the source of truth for indicator values. Each indicator added to this library undergoes testing, where the output is compared against the corresponding indicator output from Pandas-TA. Due to slight differences in calculations, particularly within NumPy, not all values are exactly identical. Therefore, if differences exceed a given threshold (usually beyond one decimal place), a Pearson correlation coefficient is calculated to ensure correct correlation with the expected output.
 
 ### Speed Tests
-The following charts indicate the results and speed of Pandas-TA and Hexital both Bulk and Incremental calculations these are the following results of running Pandas-TA and hexital both in Bulk (_all candles calculated at once_) and incremental (_Caluclating after each new candle is added_); charts _1 and 2_.
 
-The incremental chart's here are calculating the TA, adding one, re-calculating up to N amount. Pandas-TA/Pandas/Numpy for incremental data is clearly a slow process, this from my understanding due to the underlying way numpy will append/concat data, having to re-create the memory rather than resize. This is why Numpy/Panda's recommend gathering all the data prior to running calculations on it. Whereby the bulk calculating in Pandas-TA is consistent with a small time increase with the amount of data. While `Hexital` running purely pythonic can run in quickly in bulk and incremental, with little to no extra overhead time; clearly performing far faster than Pandas-TA Incremental and even faster than Pandas-TA with smaller set of data. 
+The following charts illustrate the results and speed of Pandas-TA and Hexital in both bulk and incremental calculations. These results are obtained from running Pandas-TA and Hexital in bulk (_all candles calculated at once_) and incremental(_Caluclating after each new candle is added_) modes; charts _1 and 2_.
+
+The incremental charts demonstrate the process of calculating technical analysis, adding one candle at a time, and recalculating up to a specified number of candles. It's evident that using Pandas-TA, Pandas, and NumPy for incremental data processing incurs significant performance overhead. This is primarily due to the underlying behavior of NumPy, which involves reallocating memory when appending or concatenating data, rather than resizing it. As a result, it's recommended in NumPy and Pandas documentation to gather all data prior to running calculations. On the other hand, Hexital, being purely Pythonic, exhibits efficient performance both in bulk and incremental processing, with minimal to no additional overhead time. It significantly outperforms Pandas-TA in incremental processing and even surpasses Pandas-TA in speed, especially with smaller datasets.
 
 ![EMA 10 test results.](tests/speed_tests/EMA_10.png)
 
-From chart _(3)_  you can clearly see that with bulk calculations with an extremely large dataset, Pandas-Ta performs better than `Hexital` in large Bulk data. Bulk calculations Pandas-TA going from 0.08 for 1,000 and staying there for 10,000, While Hexital Goes from 0.005 seconds for 1,000 to 0.05 seconds for 10,000. While Hexital is faster, there is a clear growth in process time. Therefore for backtesting with a large dataset, Pandas-TA will give you the best performance, whereas Hexital will continue to slow down.
+From chart _(3)_, it's evident that in bulk calculations with an extremely large dataset, Pandas-TA outperforms Hexital. Pandas-TA maintains consistent performance, with processing times starting at 0.08 seconds for 1,000 candles and remaining stable at this level for 10,000 candles. In contrast, Hexital exhibits faster processing times, starting at 0.005 seconds for 1,000 candles but increasing to 0.05 seconds for 10,000 candles. While Hexital is initially faster, there is a noticeable growth in processing time as the dataset size increases. Therefore, for backtesting with a large dataset, Pandas-TA offers superior performance, while Hexital may experience slowdowns.
 
 ![EMA 10 Bulk test results.](tests/speed_tests/EMA_10%20Bulk%20Calculations.png)
 
 However referencing chart _(4)_ being an example of using both these libraries for a live application, whereby at n candles we incrementing a dataset with a candle and calculating the new TA; `Hexital` is far quicker. This is due to the speed that python can increment a list of data rather than Panda, as well as `Hexital` only needing to calculate the newest candle rather than having to re-calculate the entire dataset. Chart _3_ clearly shows the speed benefits it has over Pandas-TA and other Panda based Technical Analysis tools for incremental data sets.
 
 ![EMA 10 Real world usage.](tests/speed_tests/EMA_10_real_world.png)
 
 For reference, if using seconds Candle with 10,000 candles that is around 2 Hours 46 minutes.
+
 #### Note
+
 The code that produces these charts is: `tests/speed_tests/run_speed_test.py` and can be ran by calling `make speed-test`. Some noise is seen due to running on personal laptop while in use.
+
 ## Inspiration
-This library was was inspired by [TALIpp](https://github.com/nardew/talipp) which is another Incremental Technical Analysis Library, however I disliked the seperate input lists rather then an entire candle, and futhermore outputs are seperated entities requiring lots of managing. Whereas Hexital stores all data within the Candles making easier usage.
+
+This library was inspired by [TALIpp](https://github.com/nardew/talipp), another Incremental Technical Analysis Library. However, I found the separate input lists rather cumbersome compared to working with an entire candle. Additionally, in TALIpp, outputs are separate entities, requiring extensive management. In contrast, Hexital stores all data within the candle, simplifying usage and management.
```


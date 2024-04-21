# Comparing `tmp/pkscreener-0.44.20240420.281.tar.gz` & `tmp/pkscreener-0.44.20240421.282.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240420.281.tar", last modified: Sat Apr 20 17:13:06 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240421.282.tar", last modified: Sun Apr 21 04:43:19 2024, max compression
```

## Comparing `pkscreener-0.44.20240420.281.tar` & `pkscreener-0.44.20240421.282.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 17:13:06.989236 pkscreener-0.44.20240420.281/
--rw-rw-rw-   0        0        0     1086 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-20 17:13:06.989236 pkscreener-0.44.20240420.281/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 17:13:06.973646 pkscreener-0.44.20240420.281/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 17:13:06.989236 pkscreener-0.44.20240420.281/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25094 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9489 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     6185 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3237 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29418 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17734 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8120 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   111467 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    46418 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    79118 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-20 17:12:59.000000 pkscreener-0.44.20240420.281/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   119023 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-20 17:08:16.000000 pkscreener-0.44.20240420.281/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    48027 2024-04-20 17:08:16.000000 pkscreener-0.44.20240420.281/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    22474 2024-04-20 17:08:16.000000 pkscreener-0.44.20240420.281/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-20 17:13:06.973646 pkscreener-0.44.20240420.281/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-20 17:13:06.000000 pkscreener-0.44.20240420.281/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-04-20 17:13:06.000000 pkscreener-0.44.20240420.281/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 17:13:06.000000 pkscreener-0.44.20240420.281/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-04-20 17:13:06.000000 pkscreener-0.44.20240420.281/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-20 17:13:06.000000 pkscreener-0.44.20240420.281/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-20 17:13:06.000000 pkscreener-0.44.20240420.281/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-20 17:13:06.989236 pkscreener-0.44.20240420.281/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-04-20 17:08:16.000000 pkscreener-0.44.20240420.281/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 04:43:19.500488 pkscreener-0.44.20240421.282/
+-rw-rw-rw-   0        0        0     1086 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-21 04:43:19.500488 pkscreener-0.44.20240421.282/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 04:43:19.484864 pkscreener-0.44.20240421.282/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 04:43:19.500488 pkscreener-0.44.20240421.282/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25172 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9489 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7018 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3237 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29415 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17734 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8120 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   112347 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    47534 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    79711 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-21 04:43:12.000000 pkscreener-0.44.20240421.282/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   120943 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    48027 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    22817 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-21 04:43:19.484864 pkscreener-0.44.20240421.282/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-21 04:43:19.000000 pkscreener-0.44.20240421.282/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-04-21 04:43:19.000000 pkscreener-0.44.20240421.282/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 04:43:19.000000 pkscreener-0.44.20240421.282/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-04-21 04:43:19.000000 pkscreener-0.44.20240421.282/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-21 04:43:19.000000 pkscreener-0.44.20240421.282/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-21 04:43:19.000000 pkscreener-0.44.20240421.282/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-21 04:43:19.500488 pkscreener-0.44.20240421.282/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/setup.py
```

### Comparing `pkscreener-0.44.20240420.281/LICENSE` & `pkscreener-0.44.20240421.282/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/LICENSE-Others` & `pkscreener-0.44.20240421.282/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/PKG-INFO` & `pkscreener-0.44.20240421.282/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240420.281
+Version: 0.44.20240421.282
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240420.281.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240421.282.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240420.281/README.md` & `pkscreener-0.44.20240421.282/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240420.281/pkscreener/__init__.py` & `pkscreener-0.44.20240421.282/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/ConfigManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,16 @@
         self.morninganalysiscandleduration = '1m'
         self.logger = None
         self.showPastStrategyData = False
         # This determines how many days apart the backtest calculations are run.
         # For example, for weekly backtest calculations, set this to 5 (5 days = 1 week)
         # For fortnightly, set this to 10 and so on (10 trading sessions = 2 weeks)
         self.backtestPeriodFactor = 1
-        self.defaultMonitorOptions = "X:12:9:2.5,|X:0:5:0:50:i 1m,X:12:2,X:12:5:0:30,X:12:6:3,X:12:6:7:1,X:12:6:8,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:23,X:12:24,X:12:10"
+        self.maxDashboardWidgetsPerRow = 6
+        self.defaultMonitorOptions = "X:12:9:2.5,|X:0:5:0:50,X:12:2,X:12:5:0:30,X:12:6:3,X:12:6:7:1,X:12:6:8,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:23,X:12:24,X:12:10,X:12:12:i 1m,X:12:12:i 5m,X:12:13:i 1m"
 
         self.daysToLookback = 22 * self.backtestPeriodFactor  # 1 month
         self.periods = [1,2,3,4,5,10,15,22,30]
         if self.maxBacktestWindow > self.periods[-1]:
             self.periods.extend(self.maxBacktestWindow)
 
     @property
```

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/MarketMonitor.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 import numpy as np
 from PKDevTools.classes.Singleton import SingletonType, SingletonMixin
 from PKDevTools.classes.OutputControls import OutputControls
 from PKDevTools.classes.ColorText import colorText
 from pkscreener.classes import Utility
 
 class MarketMonitor(SingletonMixin, metaclass=SingletonType):
-    def __init__(self,monitors=[]):
+    def __init__(self,monitors=[], maxNumResultsPerRow=5,maxNumColsInEachResult=6,maxNumRowsInEachResult=10):
         super(MarketMonitor, self).__init__()
         if monitors is not None and len(monitors) > 0:
             self.monitors = monitors
             self.monitorIndex = 0
             self.monitorPositions = {}
             # We are going to present the dataframes in a 3x3 matrix with limited set of columns
             rowIndex = 0
             colIndex = 0
-            self.maxNumRowsInEachResult = 10
-            self.maxNumColsInEachResult = 6
-            self.maxNumResultsPerRow = 5
+            self.maxNumRowsInEachResult = maxNumRowsInEachResult
+            self.maxNumColsInEachResult = maxNumColsInEachResult
+            self.maxNumResultsPerRow = maxNumResultsPerRow
             maxColIndex = self.maxNumColsInEachResult * self.maxNumResultsPerRow - 1
             self.lines = 0
             for monitorKey in monitors:
                 self.monitorPositions[monitorKey] = [rowIndex,colIndex]
                 colIndex += self.maxNumColsInEachResult
                 if colIndex > maxColIndex:
                     colIndex = 0
@@ -76,14 +76,24 @@
         highlightCols = []
         if screen_df is None or screen_df.empty:
             return
 
         screen_monitor_df = screen_df.copy()
         screen_monitor_df.reset_index(inplace=True)
         screen_monitor_df = screen_monitor_df[["Stock", "LTP", "%Chng","52Wk H","RSI","Volume"]].head(self.maxNumRowsInEachResult-1)
+        screen_monitor_df.loc[:, "%Chng"] = screen_monitor_df.loc[:, "%Chng"].apply(
+                    lambda x: Utility.tools.roundOff(str(x).split("% (")[0] + colorText.END,0)
+                )
+        screen_monitor_df.loc[:, "52Wk H"] = screen_monitor_df.loc[:, "52Wk H"].apply(
+            lambda x: Utility.tools.roundOff(x,0)
+        )
+        screen_monitor_df.loc[:, "Volume"] = screen_monitor_df.loc[:, "Volume"].apply(
+            lambda x: Utility.tools.roundOff(x,0)
+        )
+        screen_monitor_df.rename(columns={"%Chng": "Ch%","Volume":"Vol","52Wk H":"52WkH", "RSI":"RSI/i"}, inplace=True)
         monitorPosition = self.monitorPositions.get(screenOptions)
         if monitorPosition is not None:
             startRowIndex, startColIndex = monitorPosition
             if not self.monitor_df.empty:
                 for _ in range(self.lines):
                     sys.stdout.write("\x1b[1A")  # cursor up one line
                     sys.stdout.write("\x1b[2K")  # delete the last line
@@ -93,15 +103,16 @@
             colIndex = 0
             highlightRows = [startRowIndex]
             highlightCols = []
             while rowIndex <= len(screen_monitor_df):
                 for col in screen_monitor_df.columns:
                     if rowIndex == 0:
                         # Column names to be repeated for each refresh in respective headers
-                        self.monitor_df.loc[startRowIndex,[f"A{startColIndex+1}"]] = colorText.BOLD+colorText.HEAD+(screenOptions.replace(":D","") if startColIndex==firstColIndex else col)+colorText.END
+                        widgetHeader = ":".join(screenOptions.replace(":D","").split(":")[:4])
+                        self.monitor_df.loc[startRowIndex,[f"A{startColIndex+1}"]] = colorText.BOLD+colorText.HEAD+(widgetHeader if startColIndex==firstColIndex else col)+colorText.END
                         highlightCols.append(startColIndex)
                     else:
                         self.monitor_df.loc[startRowIndex, [f"A{startColIndex+1}"]] = screen_monitor_df.iloc[rowIndex-1,colIndex]
                         colIndex += 1
                     startColIndex += 1
                 _, startColIndex= monitorPosition
                 rowIndex += 1
```

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/MenuOptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,23 +73,23 @@
     "Z": "Exit (Ctrl + C)",
 }
 level2_X_MenuDict = {
     "0": "Full Screening (Shows Technical Parameters without any criterion)",
     "1": "Probable Breakouts/Breakdowns   ",
     "2": "Today's Breakouts/Breakdowns",
     "3": "Consolidating stocks            ",
-    "4": "Lowest Volume in last 'N'-days (Early Breakout Detection)",
+    "4": "Lowest Volume in last N-days (Early Breakout Detection)",
     "5": "RSI screening                   ",
     "6": "Reversal Signals",
     "7": "Stocks making Chart Patterns    ",
     "8": "CCI outside of the given range",
     "9": "Volume gainers                  ",
     "10": "Closing at least 2% up since last 3 days",
     "11": "Short term bullish (Ichimoku)  ",
-    "12": "15 Minute Price & Volume breakout(Intraday)",
+    "12": "N-Minute Price & Volume breakout(Intraday)",
     "13": "Bullish RSI & MACD             ",
     "14": "NR4 Daily Today",
     "15": "52 week low breakout(today)(Sell)",
     "16": "10 days low breakout(Sell)",
     "17": "52 week high breakout(today)     ",
     "18": "Bullish Aroon(14) Crossover",
     "19": "MACD Histogram x below 0 (Sell) ",
```

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/ScreeningStatistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -696,45 +696,48 @@
                 while(diff_df["diff"][index-1] >= 0 and index >=0):
                     index -= 1
             crossOver += 1
         ts = diff_df.tail(len(diff_df)-index +1).head(1).index[-1]
         return ts, df[df.index == ts] #df.head(len(df) -index +1).tail(1)
     
     # Find stock showing RSI crossing with RSI 9 SMA
-    def findRSICrossingMA(self, df, screenDict, saveDict,lookFor=1, maLength=9):
+    def findRSICrossingMA(self, df, screenDict, saveDict,lookFor=1, maLength=9, rsiKey="RSI"):
         if df is None or len(df) == 0:
             return False
         data = df.copy()
         data = data[::-1]
-        maRsi = pktalib.MA(data['RSI'], timeperiod=maLength)
+        maRsi = pktalib.MA(data[rsiKey], timeperiod=maLength)
         data = data[::-1].head(3)
         maRsi = maRsi[::-1].head(3)
         saved = self.findCurrentSavedValue(screenDict,saveDict,"Trend")
-        if lookFor in [1,3] and maRsi.iloc[0] <= data['RSI'].iloc[0] and maRsi.iloc[1] > data['RSI'].iloc[1]:
+        if lookFor in [1,3] and maRsi.iloc[0] <= data[rsiKey].iloc[0] and maRsi.iloc[1] > data[rsiKey].iloc[1]:
             screenDict['MA-Signal'] = saved[0] + colorText.BOLD + colorText.GREEN + f'RSI-MA-Buy' + colorText.END
             saveDict['MA-Signal'] = saved[1] + f'RSI-MA-Buy'
-            return True
-        elif lookFor in [2,3] and maRsi.iloc[0] >= data['RSI'].iloc[0] and maRsi.iloc[1] < data['RSI'].iloc[1]:
+            return True if (rsiKey == "RSIi") else (self.findRSICrossingMA(df, screenDict, saveDict,lookFor=lookFor, maLength=maLength, rsiKey="RSIi") or True)
+        elif lookFor in [2,3] and maRsi.iloc[0] >= data[rsiKey].iloc[0] and maRsi.iloc[1] < data[rsiKey].iloc[1]:
             screenDict['MA-Signal'] = saved[0] + colorText.BOLD + colorText.FAIL + f'RSI-MA-Sell' + colorText.END
             saveDict['MA-Signal'] = saved[1] + f'RSI-MA-Sell'
-            return True
-        return False
+            return True if (rsiKey == "RSIi") else (self.findRSICrossingMA(df, screenDict, saveDict,lookFor=lookFor, maLength=maLength, rsiKey="RSIi") or True)
+        return False if (rsiKey == "RSIi") else (self.findRSICrossingMA(df, screenDict, saveDict,lookFor=lookFor, maLength=maLength, rsiKey="RSIi"))
     
     # Find stocks with rising RSI from lower levels
-    def findRisingRSI(self, df):
+    def findRisingRSI(self, df, rsiKey="RSI"):
         if df is None or len(df) == 0:
             return False
         data = df.copy()
         data = data[::-1]
         data = data.tail(3)
         dayMinus2RSI = data["RSI"].iloc[0]
         dayMinus1RSI = data["RSI"].iloc[1]
         dayRSI = data["RSI"].iloc[2]
-        return (dayMinus2RSI <= 35 and dayMinus1RSI > dayMinus2RSI and dayRSI > dayMinus1RSI) or \
+        returnValue = (dayMinus2RSI <= 35 and dayMinus1RSI > dayMinus2RSI and dayRSI > dayMinus1RSI) or \
                 (dayMinus1RSI <= 35 and dayRSI > dayMinus1RSI)
+        if rsiKey == "RSI":
+            returnValue = self.findRisingRSI(df, rsiKey="RSIi") or returnValue
+        return returnValue
 
     #@measure_time
     # Find out trend for days to lookback
     def findTrend(self, df, screenDict, saveDict, daysToLookback=None, stockName=""):
         if df is None or len(df) == 0:
             return "Unknown"
         data = df.copy()
@@ -2126,30 +2129,31 @@
             saveDict["%Chng"] = pct_change_text
             screenDict["%Chng"] = colorText.GREEN + pct_change_text + colorText.END
             return True and self.getCandleType(data.head(1))
         return False
 
     #@measure_time
     # validate if RSI is within given range
-    def validateRSI(self, df, screenDict, saveDict, minRSI, maxRSI):
+    def validateRSI(self, df, screenDict, saveDict, minRSI, maxRSI,rsiKey="RSI"):
         if df is None or len(df) == 0:
             return False
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
-        rsi = int(data.head(1)["RSI"].iloc[0])
-        saveDict["RSI"] = rsi
+        rsi = int(data.head(1)[rsiKey].iloc[0])
+        saveDict[rsiKey] = rsi
         # https://chartink.com/screener/rsi-screening
-        if rsi >= minRSI and rsi <= maxRSI:  # or (rsi <= 71 and rsi >= 67):
-            screenDict["RSI"] = (
+        if rsi> 0 and rsi >= minRSI and rsi <= maxRSI:  # or (rsi <= 71 and rsi >= 67):
+            screenDict[rsiKey] = (
                 colorText.BOLD + colorText.GREEN + str(rsi) + colorText.END
             )
-            return True
-        screenDict["RSI"] = colorText.BOLD + colorText.FAIL + str(rsi) + colorText.END
-        return False
+            return True if (rsiKey == "RSIi") else (self.validateRSI(df, screenDict, saveDict, minRSI, maxRSI,rsiKey="RSIi") or True)
+        screenDict[rsiKey] = colorText.BOLD + colorText.FAIL + str(rsi) + colorText.END
+        # If either daily or intraday RSI comes within range?
+        return False if (rsiKey == "RSIi") else (self.validateRSI(df, screenDict, saveDict, minRSI, maxRSI,rsiKey="RSIi"))
 
     # Validate if the stock is bullish in the short term
     def validateShortTermBullish(self, df, screenDict, saveDict):
         if df is None or len(df) == 0:
             return False
         data = df.copy()
         # https://chartink.com/screener/short-term-bullish
```

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/StockScreener.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,22 +96,37 @@
             with hostRef.processingCounter.get_lock():
                 hostRef.processingCounter.value += 1
 
             volumeRatio, period = self.determineBasicConfigs(stock, newlyListedOnly, volumeRatio, logLevel, hostRef, configManager, screener, userArgsLog)
             # hostRef.default_logger.info(
             #     f"For stock:{stock}, stock exists in objectDictionary:{hostRef.objectDictionary.get(stock)}, cacheEnabled:{configManager.cacheEnabled}, isTradingTime:{self.isTradingTime}, downloadOnly:{downloadOnly}"
             # )
-            data = self.getRelevantDataForStock(totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef, configManager, fetcher, period, testData,exchangeName)
+            data = self.getRelevantDataForStock(totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef,hostRef.objectDictionary, configManager, fetcher, period, testData,exchangeName)
+            if not configManager.isIntradayConfig():
+                intraday_data = self.getRelevantDataForStock(totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef, hostRef.secondaryObjectDictionary, configManager, fetcher, period, testData,exchangeName)
+            else:
+                intraday_data = data
             if data is not None:
                 if len(data) == 0 or len(data) < backtestDuration:
                     return None
             else:
                 return None
             # hostRef.default_logger.info(f"Will pre-process data:\n{data.tail(10)}")
             fullData, processedData, data = self.getCleanedDataForDuration(backtestDuration, portfolio, screeningDictionary, saveDictionary, configManager, screener, data)
+            if backtestDuration == 0:
+                intraday_fullData, intraday_processedData = screener.preprocessData(
+                    intraday_data, daysToLookback=configManager.effectiveDaysToLookback
+                )
+                fullData = fullData.head(len(intraday_fullData))
+                processedData = processedData.head(len(intraday_processedData))
+                data = data.tail(len(intraday_data))
+                # Indexes won't match. Hence, we'd need to fallback on tolist
+                processedData.loc[:,"RSIi"] = intraday_processedData["RSI"].tolist()
+                fullData.loc[:,"RSIi"] = intraday_fullData["RSI"].tolist()
+
             def returnLegibleData():
                 if backtestDuration == 0 or menuOption not in ["B"]:
                     return None
                 elif (backtestDuration > 0 and backtestDuration <= configManager.maxBacktestWindow):
                     screener.validateMovingAverages(
                         processedData, screeningDictionary, saveDictionary, maRange=1.25
                     )
@@ -688,16 +703,16 @@
                     # data has the last row from inputData at the top.
                 fullData, processedData = screener.preprocessData(
                         inputData, daysToLookback=configManager.daysToLookback
                     )
                 
         return fullData,processedData,data
 
-    def getRelevantDataForStock(self, totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef, configManager, fetcher, period, testData=None,exchangeName="INDIA"):
-        hostData = hostRef.objectDictionary.get(stock)
+    def getRelevantDataForStock(self, totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef,objectDictionary, configManager, fetcher, period, testData=None,exchangeName="INDIA"):
+        hostData = objectDictionary.get(stock)
         data = None
         start = None
         if (period == '1d' or configManager.duration[-1] == "m") and backtestDuration > 0:
             start = PKDateUtilities.nthPastTradingDateStringFromFutureDate(backtestDuration)
             end = start
         if (
                 not shouldCache
@@ -758,21 +773,21 @@
                         hostData["data"], columns=columns, index=hostData["index"]
                     )
                 pass
 
         if ((shouldCache and not self.isTradingTime and (hostData is None)) or downloadOnly) \
             or (shouldCache and hostData is None):  # and backtestDuration == 0 # save only if we're NOT backtesting
                 if start is None and data is not None:
-                    hostRef.objectDictionary[stock] = data.to_dict("split")
+                    objectDictionary[stock] = data.to_dict("split")
                 if downloadOnly:
                     with hostRef.processingResultsCounter.get_lock():
                         hostRef.processingResultsCounter.value += 1
                     raise ScreeningStatistics.DownloadDataOnly
                 else:
-                    hostData = hostRef.objectDictionary.get(stock)
+                    hostData = objectDictionary.get(stock)
         return data
 
     def determineBasicConfigs(self, stock, newlyListedOnly, volumeRatio, logLevel, hostRef, configManager, screener, userArgsLog):
         if userArgsLog:
             self.setupLoggers(hostRef, screener, logLevel, stock)
         period = configManager.period
         if volumeRatio <= 0:
@@ -841,14 +856,15 @@
         columns = [
             "Stock",
             "LTP",
             "%Chng",
             "52Wk H",
             "52Wk L",
             "RSI",
+            "RSIi",
             "Volume",
             "22-Pd %",
             "Consol.",
             "Breakout",
             "MA-Signal",
             "Trend",
             "Pattern",
@@ -858,14 +874,15 @@
         screeningDictionary = {
             "Stock": "",
             "LTP": 0,
             "%Chng": 0,
             "52Wk H": 0,
             "52Wk L": 0,
             "RSI": 0,
+            "RSIi": 0,
             "Volume": "",
             "22-Pd %": "",
             "Consol.": "Range:0%",
             "Breakout": "BO: 0 R: 0",
             "MA-Signal": "",
             "Trend": "",
             "Pattern": "",
@@ -875,14 +892,15 @@
         saveDictionary = {
             "Stock": "",
             "LTP": 0,
             "%Chng": 0,
             "52Wk H": 0,
             "52Wk L": 0,
             "RSI": 0,
+            "RSIi": 0,
             "Volume": "",
             "22-Pd %": "",
             "Consol.": "Range:0%",
             "Breakout": "BO: 0 R: 0",
             "MA-Signal": "",
             "Trend": "",
             "Pattern": "",
```

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,14 +336,27 @@
         dataSrcFont = ImageFont.truetype(fontPath, DATASRC_FONTSIZE)
         dataSrc_width, dataSrc_height = dataSrcFont.getsize_multiline(dataSrc)
         draw = ImageDraw.Draw(sourceImage)
         draw.text((width-dataSrc_width, height-dataSrc_height-2), text=dataSrc, font=dataSrcFont, fill=(128, 128, 128, opacity))
         # sourceImage.show()
         return sourceImage
 
+    def roundOff(value,places):
+        roundValue = value
+        try:
+            newValue = tools.removeAllColorStyles(str(roundValue))
+            newValue = newValue.replace("%","").replace("x","")
+            roundValue = round(float(newValue),places)
+            if places == 0:
+                roundValue = int(roundValue)
+            roundValue = str(value).replace(str(newValue),str(roundValue))
+        except:
+            pass
+        return roundValue
+    
     def removeAllColorStyles(styledText):
         styles = [
             colorText.HEAD,
             colorText.END,
             colorText.BOLD,
             colorText.UNDR,
             colorText.BLUE,
@@ -823,14 +836,15 @@
     ):
         isIntraday = isIntraday or configManager.isIntradayConfig()
         exists, cache_file = tools.afterMarketStockDataExists(
             isIntraday, forceLoad=forceLoad
         )
         initialLoadCount = len(stockDict)
         isTrading = PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]
+        # stockCodes is not None mandates that we start our work based on the downloaded data from yesterday
         if (stockCodes is not None and len(stockCodes) > 0) and (isTrading or downloadOnly or not exists):
             stockDict = tools.downloadLatestData(stockDict,configManager,stockCodes,exchangeSuffix=exchangeSuffix)
             # return stockDict
 
         default_logger().info(
             f"Stock data cache file:{cache_file} exists ->{str(exists)}"
         )
```

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/classes/keys.py` & `pkscreener-0.44.20240421.282/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/courbd.ttf` & `pkscreener-0.44.20240421.282/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/globals.py` & `pkscreener-0.44.20240421.282/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 loadCount = 0
 loadedStockData = False
 m0 = menus()
 m1 = menus()
 m2 = menus()
 m3 = menus()
 maLength = None
+nValueForMenu = 0
 menuChoiceHierarchy = ""
 newlyListedOnly = False
 screenCounter = None
 screener = ScreeningStatistics.ScreeningStatistics(configManager, default_logger())
 screenResults = None
 backtest_df = None
 screenResultsCounter = None
@@ -358,14 +359,16 @@
             + colorText.FAIL
             + "[+] Error: Non-numeric value entered! Please try again!"
             + colorText.END
         )
         input("Press <Enter> to continue...")
         return
     OutputControls().printOutput(colorText.END)
+    global nValueForMenu 
+    nValueForMenu = daysForLowestVolume
     return daysForLowestVolume
 
 
 def handleSecondaryMenuChoices(
     menuOption, testing=False, defaultAnswer=None, user=None
 ):
     if menuOption == "H":
@@ -536,17 +539,21 @@
             sleep(2)
             Utility.tools.clearScreen()
             return initPostLevel1Execution(indexOption, executeOption, retrial=True)
     return indexOption, executeOption
 
 def labelDataForPrinting(screenResults, saveResults, configManager, volumeRatio,executeOption, reversalOption):
     # Publish to gSheet with https://github.com/burnash/gspread
-    global menuChoiceHierarchy
+    global menuChoiceHierarchy, userPassedArgs
     try:
-        sortKey = ["Volume"] if "RSI" not in menuChoiceHierarchy else "RSI"
+        isTrading = PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()
+        if isTrading or userPassedArgs.monitor:
+            screenResults['RSI'] = screenResults['RSI'].astype(str) + "/" + screenResults['RSIi'].astype(str)
+            saveResults['RSI'] = saveResults['RSI'].astype(str) + "/" + saveResults['RSIi'].astype(str)
+        sortKey = ["Volume"] if "RSI" not in menuChoiceHierarchy else ("RSIi" if isTrading else "RSI")
         ascending = [False if "RSI" not in menuChoiceHierarchy else True]
         if executeOption == 21:
             if reversalOption in [3,5,6,7]:
                 sortKey = ["MFI"]
                 ascending = [reversalOption in [6,7]]
             elif reversalOption in [8,9]:
                 sortKey = ["FVDiff"]
@@ -568,15 +575,15 @@
             except:
                 pass
             screenResults.sort_values(by=sortKey, ascending=ascending, inplace=True)
             saveResults.sort_values(by=sortKey, ascending=ascending, inplace=True)
         except Exception as e:
             default_logger().debug(e, exc_info=True)
             pass
-        columnsToBeDeleted = ["MFI","FVDiff","ConfDMADifference","bbands_ulr_ratio_max5"]
+        columnsToBeDeleted = ["MFI","FVDiff","ConfDMADifference","bbands_ulr_ratio_max5", "RSIi"]
         for column in columnsToBeDeleted:
             if column in saveResults.columns:
                 saveResults.drop(column, axis=1, inplace=True, errors="ignore")
                 screenResults.drop(column, axis=1, inplace=True, errors="ignore")
         if "Stock" in screenResults.columns:
             screenResults.set_index("Stock", inplace=True)
         if "Stock" in saveResults.columns:
@@ -609,14 +616,19 @@
         default_logger().debug(e, exc_info=True)
     return screenResults, saveResults
 
 def isInterrupted():
     global keyboardInterruptEventFired
     return keyboardInterruptEventFired
 
+def refreshStockData():
+    global stockDict, loadedStockData
+    stockDict = None
+    loadedStockData = False
+
 # @tracelog
 def main(userArgs=None,optionalFinalOutcome_df=None):
     global screenResults, selectedChoice, defaultAnswer, menuChoiceHierarchy, screenCounter, screenResultsCounter, stockDict, userPassedArgs, loadedStockData, keyboardInterruptEvent, loadCount, maLength, newlyListedOnly, keyboardInterruptEventFired,strategyFilter, elapsed_time, start_time
     selectedChoice = {"0": "", "1": "", "2": "", "3": "", "4": ""}
     elapsed_time = 0
     start_time = 0
     testing = False if userArgs is None else (userArgs.testbuild and userArgs.prodbuild)
@@ -930,15 +942,18 @@
                 + colorText.END
             )
             input("Press <Enter> to continue...")
             return None, None
         else:
             configManager.volumeRatio = float(volumeRatio)
     if executeOption == 12:
-        configManager.toggleConfig(candleDuration="15m")
+        candleDuration = userPassedArgs.intraday if (userPassedArgs is not None and userPassedArgs.intraday is not None) else ("15m")
+        configManager.toggleConfig(candleDuration=candleDuration)
+        global nValueForMenu 
+        nValueForMenu = candleDuration
     if executeOption == 21:
         selectedMenu = m2.find(str(executeOption))
         if len(options) >= 4:
             popOption = int(options[3])
             if popOption >= 0 and popOption <= 9:
                 pass
         else:
@@ -1111,15 +1126,31 @@
                     configManager,
                     downloadOnly=downloadOnly,
                     defaultAnswer=defaultAnswer,
                     forceLoad=(menuOption in ["X", "B", "G", "S"]),
                     stockCodes = listStockCodes,
                     exchangeSuffix = "" if (indexOption == 15 or (configManager.defaultIndex == 15 and indexOption == 0)) else ".NS"
             )
+            if not configManager.isIntradayConfig():
+                candleDuration = (userPassedArgs.intraday if (userPassedArgs is not None and userPassedArgs.intraday is not None) else "1m")
+                configManager.toggleConfig(candleDuration=candleDuration,clearCache=False)
+                # We also need to load the intraday data to be able to calculate intraday RSI
+                Utility.tools.loadStockData(
+                        {},
+                        configManager,
+                        downloadOnly=downloadOnly,
+                        defaultAnswer=defaultAnswer,
+                        forceLoad=(menuOption in ["X", "B", "G", "S"]),
+                        stockCodes = listStockCodes,
+                        isIntraday=True,
+                        exchangeSuffix = "" if (indexOption == 15 or (configManager.defaultIndex == 15 and indexOption == 0)) else ".NS"
+                )
+                resetConfigToDefault()
             loadedStockData = True
+            
         loadCount = len(stockDict) if stockDict is not None else 0
 
         if downloadOnly:
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.WARN
                 + "[+] Starting download.. Press Ctrl+C to stop!"
@@ -1646,14 +1677,16 @@
     elif selectedChoice["2"] == "21":
         menuChoiceHierarchy = (
             menuChoiceHierarchy
             + f'>{level3_X_PopularStocks_MenuDict[selectedChoice["3"]].strip()}'
         )
     intraday = "(Intraday)" if (userPassedArgs is not None and userPassedArgs.intraday) or configManager.isIntradayConfig() else ""
     menuChoiceHierarchy = f"{menuChoiceHierarchy}{intraday}"
+    global nValueForMenu
+    menuChoiceHierarchy = menuChoiceHierarchy.replace("N-",f"{nValueForMenu}-")
     OutputControls().printOutput(
         colorText.BOLD
         + colorText.FAIL
         + "[+] You chose: "
         + menuChoiceHierarchy
         + colorText.END
     )
```

### Comparing `pkscreener-0.44.20240420.281/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240421.282/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240421.282/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240421.282/pkscreener/pkscreenercli.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,15 +287,15 @@
                 + colorText.FAIL
                 + "[+] Neither ta-lib nor pandas_ta was located. You need at least one of them to continue! \n[+] Please follow instructions from README file under PKScreener repo: https://github.com/pkjmesra/PKScreener"
                 + colorText.END
             )
             input("Press any key to try anyway...")
 
 def runApplication():
-    from pkscreener.globals import main, sendQuickScanResult, sendGlobalMarketBarometer, updateMenuChoiceHierarchy, isInterrupted
+    from pkscreener.globals import main, sendQuickScanResult, sendGlobalMarketBarometer, updateMenuChoiceHierarchy, isInterrupted, refreshStockData
     # From a previous call to main with args, it may have been mutated.
     # Let's stock to the original args passed by user
     argsv = argParser.parse_known_args()
     args = argsv[0]
     if args.runintradayanalysis:
         from pkscreener.classes.MenuOptions import menus
         runOptions = menus.allMenus(topLevel="C", index=12)
@@ -352,34 +352,40 @@
         if args.barometer:
             sendGlobalMarketBarometer(userArgs=args)
         else:
             global results, resultStocks, plainResults
             monitorOption_org = ""
             if args.monitor:
                 args.answerdefault = args.answerdefault or 'Y'
+                if MarketMonitor().monitorIndex == 0:
+                    # Load the stock data afresh for each cycle
+                    refreshStockData()
                 monitorOption_org = MarketMonitor().currentMonitorOption()
                 monitorOption = monitorOption_org
                 lastComponent = monitorOption.split(":")[-1]
                 if "i" in lastComponent:
                     # We need to switch to intraday scan
                     monitorOption = monitorOption.replace(lastComponent,"")
                     args.intraday = lastComponent.replace("i","").strip()
                     configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
                 else:
                     # We need to switch to daily scan
-                    args.intraday = False
+                    args.intraday = None
                     configManager.toggleConfig(candleDuration='1d', clearCache=False)
                 if monitorOption.startswith("|"):
                     monitorOption = monitorOption.replace("|","")
                     # We need to pipe the output from previous run into the next one
                     if resultStocks is not None:
                         resultStocks = ",".join(resultStocks)
                         monitorOption = f"{monitorOption}:{resultStocks}"
                 args.options = monitorOption
             try:
+                results = None
+                plainResults = None
+                resultStocks = None
                 results, plainResults = main(userArgs=args)
                 if isInterrupted():
                     sys.exit(0)
             except SystemExit:
                 sys.exit(0)
             except Exception:
                 # Probably user cancelled an operation by choosing a cancel sub-menu somewhere
@@ -405,15 +411,15 @@
             pass
 
         OutputControls(enableMultipleLineOutput=(args.monitor is None)).printOutput("",end="\r")
         
     configManager.getConfig(ConfigManager.parser)
     # configManager.restartRequestsCache()
     if args.monitor is not None:
-        MarketMonitor(monitors=args.monitor.split(",") if len(args.monitor)>5 else configManager.defaultMonitorOptions.split(","))
+        MarketMonitor(monitors=args.monitor.split(",") if len(args.monitor)>5 else configManager.defaultMonitorOptions.split(","),maxNumResultsPerRow=configManager.maxDashboardWidgetsPerRow)
 
     if args.log or configManager.logsEnabled:
         setupLogger(shouldLog=True, trace=args.testbuild)
         if not args.prodbuild and args.answerdefault is None:
             input("Press <Enter> to continue...")
     else:
         if "PKDevTools_Default_Log_Level" in os.environ.keys():
```

### Comparing `pkscreener-0.44.20240420.281/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240421.282/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240420.281
+Version: 0.44.20240421.282
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240420.281.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240421.282.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240420.281/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240421.282/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240420.281/setup.py` & `pkscreener-0.44.20240421.282/setup.py`

 * *Files identical despite different names*


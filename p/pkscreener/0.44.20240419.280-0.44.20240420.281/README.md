# Comparing `tmp/pkscreener-0.44.20240419.280.tar.gz` & `tmp/pkscreener-0.44.20240420.281.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240419.280.tar", last modified: Fri Apr 19 21:27:11 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240420.281.tar", last modified: Sat Apr 20 17:13:06 2024, max compression
```

## Comparing `pkscreener-0.44.20240419.280.tar` & `pkscreener-0.44.20240420.281.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 21:27:11.363291 pkscreener-0.44.20240419.280/
--rw-rw-rw-   0        0        0     1086 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-19 21:27:11.363291 pkscreener-0.44.20240419.280/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 21:27:11.347669 pkscreener-0.44.20240419.280/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 21:27:11.363291 pkscreener-0.44.20240419.280/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25094 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9489 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     6185 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3237 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29416 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17734 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8120 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   111467 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    46418 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    79118 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-19 21:27:04.000000 pkscreener-0.44.20240419.280/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   119023 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47947 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    22164 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-19 21:27:11.347669 pkscreener-0.44.20240419.280/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-19 21:27:11.000000 pkscreener-0.44.20240419.280/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-04-19 21:27:11.000000 pkscreener-0.44.20240419.280/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 21:27:11.000000 pkscreener-0.44.20240419.280/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-19 21:27:11.000000 pkscreener-0.44.20240419.280/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-19 21:27:11.000000 pkscreener-0.44.20240419.280/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-19 21:27:11.000000 pkscreener-0.44.20240419.280/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-19 21:27:11.363291 pkscreener-0.44.20240419.280/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-19 21:23:36.000000 pkscreener-0.44.20240419.280/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 17:13:06.989236 pkscreener-0.44.20240420.281/
+-rw-rw-rw-   0        0        0     1086 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-20 17:13:06.989236 pkscreener-0.44.20240420.281/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 17:13:06.973646 pkscreener-0.44.20240420.281/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 17:13:06.989236 pkscreener-0.44.20240420.281/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25094 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9489 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     6185 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3237 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29418 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17734 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8120 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   111467 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    46418 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    79118 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-20 17:12:59.000000 pkscreener-0.44.20240420.281/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   119023 2024-04-20 17:08:15.000000 pkscreener-0.44.20240420.281/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-20 17:08:16.000000 pkscreener-0.44.20240420.281/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    48027 2024-04-20 17:08:16.000000 pkscreener-0.44.20240420.281/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    22474 2024-04-20 17:08:16.000000 pkscreener-0.44.20240420.281/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-20 17:13:06.973646 pkscreener-0.44.20240420.281/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-20 17:13:06.000000 pkscreener-0.44.20240420.281/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-04-20 17:13:06.000000 pkscreener-0.44.20240420.281/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 17:13:06.000000 pkscreener-0.44.20240420.281/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-04-20 17:13:06.000000 pkscreener-0.44.20240420.281/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-20 17:13:06.000000 pkscreener-0.44.20240420.281/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-20 17:13:06.000000 pkscreener-0.44.20240420.281/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-20 17:13:06.989236 pkscreener-0.44.20240420.281/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-04-20 17:08:16.000000 pkscreener-0.44.20240420.281/setup.py
```

### Comparing `pkscreener-0.44.20240419.280/LICENSE` & `pkscreener-0.44.20240420.281/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/LICENSE-Others` & `pkscreener-0.44.20240420.281/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/PKG-INFO` & `pkscreener-0.44.20240420.281/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240419.280
+Version: 0.44.20240420.281
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240419.280.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240420.281.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240419.280/README.md` & `pkscreener-0.44.20240420.281/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240419.280/pkscreener/__init__.py` & `pkscreener-0.44.20240420.281/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/MenuOptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 configManager = ConfigManager.tools()
 
 level0MenuDict = {
     "X": "Scanners",
     "S": "Strategies",
     "B": "Backtests",
-    "G": "Growth of 10k",
+    # "G": "Growth of 10k",
     "T": "~",
     "E": "Edit user configuration",
     "Y": "View your user configuration",
     "C": "Analyse morning vs close outcomes",
     "U": "Check for software update",
     "H": "Help / About Developer",
     "Z": "Exit (Ctrl + C)",
```

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/classes/keys.py` & `pkscreener-0.44.20240420.281/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/courbd.ttf` & `pkscreener-0.44.20240420.281/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/globals.py` & `pkscreener-0.44.20240420.281/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240420.281/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240420.281/pkscreener/pkscreenerbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                     callback_data="C" + str(mnu.menuKey),
                 )
             )
     keyboard = [inlineMenus]
     reply_markup = InlineKeyboardMarkup(keyboard)
     cmds = m0.renderForMenu(
         selectedMenu=None,
-        skip=["S", "T", "E", "U", "Z","C"],
+        skip=["S", "T", "E", "U", "Z", "C", "G"],
         asList=True,
         renderStyle=MenuRenderStyle.STANDALONE,
     )
     cmdText = ""
     for cmd in cmds:
         cmdText = f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
     # Send message with text and appended InlineKeyboard
@@ -699,15 +699,15 @@
 async def BBacktests(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
     """Show new choice of buttons"""
     query = update.callback_query
     await query.answer()
     keyboard = [
         [
             InlineKeyboardButton("Try Scanners", callback_data=str("CX")),
-            InlineKeyboardButton("Growth of 10k", callback_data=str("CG")),
+            # InlineKeyboardButton("Growth of 10k", callback_data=str("CG")),
         ]
     ]
     reply_markup = InlineKeyboardMarkup(keyboard)
     await query.edit_message_text(
         text="Backtesting NOT implemented yet in this Bot!\n\n\nYou can use backtesting by downloading the software from https://github.com/pkjmesra/PKScreener/",
         reply_markup=reply_markup,
     )
@@ -817,23 +817,23 @@
     if cmd == "help":
         await help_command(update=update, context=context)
         return START_ROUTES
     if cmd in ["x", "b", "g"]:
         await shareUpdateWithChannel(update=update, context=context)
         m0.renderForMenu(
             selectedMenu=None,
-            skip=["S", "T", "E", "U"],
+            skip=["S", "T", "E", "U", "Z", "C", "G"],
             renderStyle=MenuRenderStyle.STANDALONE,
         )
         selectedMenu = m0.find(cmd.upper())
         cmdText = ""
         cmds = m1.renderForMenu(
             selectedMenu=selectedMenu,
             skip=(
-                ["W", "E", "M", "Z"] if cmd in ["x"] else ["W", "E", "M", "Z", "N", "0"]
+                ["W", "E", "M", "Z"] if cmd in ["x"] else ["W", "E", "M", "Z", "N", "0", "15"]
             ),
             asList=True,
             renderStyle=MenuRenderStyle.STANDALONE,
         )
         for cmd in cmds:
             if cmd in ["N", "0"]:
                 continue
@@ -880,15 +880,15 @@
 
     if "x_" in cmd or "b_" in cmd or "g_" in cmd:
         await shareUpdateWithChannel(update=update, context=context)
         selection = cmd.split("_")
         if len(selection) == 2:
             m0.renderForMenu(
                 selectedMenu=None,
-                skip=["S", "T", "E", "U", "Z", "C"],
+                skip=["S", "T", "E", "U", "Z", "C", "G"],
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             selectedMenu = m0.find(selection[0].upper())
             m1.renderForMenu(
                 selectedMenu=selectedMenu,
                 skip=(
                     ["W", "E", "M", "Z"]
@@ -938,15 +938,15 @@
                     f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
                 )
             await update.message.reply_text(f"Choose an option:\n{cmdText}")
             return START_ROUTES
         elif len(selection) == 3:
             m0.renderForMenu(
                 selectedMenu=None,
-                skip=["S", "T", "E", "U", "Z","C"],
+                skip=["S", "T", "E", "U", "Z", "C", "G"],
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             selectedMenu = m0.find(selection[0].upper())
             m1.renderForMenu(
                 selectedMenu=selectedMenu,
                 skip=(
                     ["W", "E", "M", "Z"]
@@ -1064,15 +1064,15 @@
 
 async def help_command(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
     if _shouldAvoidResponse(update):
         return
 
     cmds = m0.renderForMenu(
         selectedMenu=None,
-        skip=["S", "T", "E", "U", "Z","C"],
+        skip=["S", "T", "E", "U", "Z", "C", "G"],
         asList=True,
         renderStyle=MenuRenderStyle.STANDALONE,
     )
     cmdText = ""
     for cmd in cmds:
         cmdText = f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
     """Send a message when the command /help is issued."""
@@ -1118,15 +1118,15 @@
         return True
     return False
 
 
 def addCommandsForMenuItems(application):
     cmds0 = m0.renderForMenu(
         selectedMenu=None,
-        skip=["S", "T", "E", "U", "Z","C"],
+        skip=["S", "T", "E", "U", "Z", "C", "G"],
         asList=True,
         renderStyle=MenuRenderStyle.STANDALONE,
     )
     for mnu0 in cmds0:
         p0 = mnu0.menuKey.upper()
         application.add_handler(CommandHandler(p0, command_handler))
         selectedMenu = m0.find(p0)
@@ -1179,15 +1179,15 @@
                     for mnu3 in cmds3:
                         p3 = mnu3.menuKey.upper()
                         application.add_handler(
                             CommandHandler(f"{p0}_{p1}_{p2}_{p3}", command_handler)
                         )
 
 
-def main() -> None:
+def runpkscreenerbot() -> None:
     """Run the bot."""
     # Create the Application and pass it your bot's token.
     global chat_idADMIN, Channel_Id
     Channel_Id, TOKEN, chat_idADMIN, GITHUB_TOKEN = get_secrets()
     # TOKEN = '1234567'
     # Channel_Id = 1001785195297
     application = Application.builder().token(TOKEN).build()
@@ -1199,18 +1199,18 @@
     # So ^ABC$ will only allow 'ABC'
     conv_handler = ConversationHandler(
         entry_points=[CommandHandler("start", start)],
         states={
             START_ROUTES: [
                 CallbackQueryHandler(XScanners, pattern="^" + str("CX") + "$"),
                 CallbackQueryHandler(XScanners, pattern="^" + str("CB") + "$"),
-                CallbackQueryHandler(XScanners, pattern="^" + str("CG") + "$"),
+                # CallbackQueryHandler(XScanners, pattern="^" + str("CG") + "$"),
                 CallbackQueryHandler(Level2, pattern="^" + str("CX_")),
                 CallbackQueryHandler(Level2, pattern="^" + str("CB_")),
-                CallbackQueryHandler(Level2, pattern="^" + str("CG_")),
+                # CallbackQueryHandler(Level2, pattern="^" + str("CG_")),
                 CallbackQueryHandler(end, pattern="^" + str("CZ") + "$"),
                 CallbackQueryHandler(start, pattern="^"),
             ],
             END_ROUTES: [],
         },
         fallbacks=[CommandHandler("start", start)],
     )
@@ -1227,8 +1227,8 @@
     application.add_error_handler(error_handler)
 
     # Run the bot until the user presses Ctrl-C
     application.run_polling(allowed_updates=Update.ALL_TYPES)
 
 
 if __name__ == "__main__":
-    main()
+    runpkscreenerbot()
```

### Comparing `pkscreener-0.44.20240419.280/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240420.281/pkscreener/pkscreenercli.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,20 @@
 argParser.add_argument(
     "--barometer",
     action="store_true",
     help="Send global market barometer to telegram channel or a user",
     required=False,
 )
 argParser.add_argument(
+    "--bot",
+    action="store_true",
+    help="Run only in telegram bot mode",
+    required=False,
+)
+argParser.add_argument(
     "-c",
     "--croninterval",
     help="Pass interval in seconds to wait before the program is run again with same parameters",
     required=False,
 )
 argParser.add_argument(
     "-d",
@@ -426,15 +432,20 @@
     if args.prodbuild:
         disableSysOut()
 
     if not configManager.checkConfigFile():
         configManager.setConfig(
             ConfigManager.parser, default=True, showFileCreatedText=False
         )
-        
+    # Check and see if we're running only the telegram bot
+    if args.bot:
+        from pkscreener import pkscreenerbot
+        pkscreenerbot.runpkscreenerbot()
+        return
+    
     if args.intraday:
         configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
     else:
         configManager.toggleConfig(candleDuration='1d', clearCache=False)
     if args.options is not None and str(args.options) == "0":
         # Must be from unit tests to be able to break out of loops via eventing
         args.options = None
```

### Comparing `pkscreener-0.44.20240419.280/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240420.281/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240419.280
+Version: 0.44.20240420.281
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240419.280.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240420.281.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.279/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240419.280/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240419.280/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240420.281/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240419.280/setup.py` & `pkscreener-0.44.20240420.281/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     + __USERNAME__
     + "/"
     + __PACKAGENAME__,  # use the URL to the github repo
     zip_safe=False,
     entry_points="""
 	[console_scripts]
 	pkscreener=pkscreener.pkscreenercli:pkscreenercli
-	pkbot=pkscreener.pkscreenerbot:main
+	pkbot=pkscreener.pkscreenerbot:runpkscreenerbot
 	""",
     download_url="https://github.com/"
     + __USERNAME__
     + "/"
     + __PACKAGENAME__
     + "/archive/v"
     + VERSION
```


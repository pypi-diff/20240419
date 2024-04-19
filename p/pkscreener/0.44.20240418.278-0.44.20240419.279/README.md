# Comparing `tmp/pkscreener-0.44.20240418.278.tar.gz` & `tmp/pkscreener-0.44.20240419.279.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240418.278.tar", last modified: Thu Apr 18 14:34:42 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240419.279.tar", last modified: Fri Apr 19 20:06:29 2024, max compression
```

## Comparing `pkscreener-0.44.20240418.278.tar` & `pkscreener-0.44.20240419.279.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 14:34:42.606234 pkscreener-0.44.20240418.278/
--rw-rw-rw-   0        0        0     1086 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-18 14:34:42.606234 pkscreener-0.44.20240418.278/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 14:34:42.590610 pkscreener-0.44.20240418.278/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:34:42.606234 pkscreener-0.44.20240418.278/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24899 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9489 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     3237 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    28153 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17603 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8120 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   111107 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    46418 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    79104 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-18 14:34:35.000000 pkscreener-0.44.20240418.278/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   117414 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47947 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    19783 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:34:42.590610 pkscreener-0.44.20240418.278/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-18 14:34:42.000000 pkscreener-0.44.20240418.278/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1282 2024-04-18 14:34:42.000000 pkscreener-0.44.20240418.278/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 14:34:42.000000 pkscreener-0.44.20240418.278/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-18 14:34:42.000000 pkscreener-0.44.20240418.278/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-18 14:34:42.000000 pkscreener-0.44.20240418.278/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-18 14:34:42.000000 pkscreener-0.44.20240418.278/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-18 14:34:42.606234 pkscreener-0.44.20240418.278/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-18 14:31:30.000000 pkscreener-0.44.20240418.278/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:06:29.708776 pkscreener-0.44.20240419.279/
+-rw-rw-rw-   0        0        0     1086 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-19 20:06:29.708776 pkscreener-0.44.20240419.279/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 20:06:29.693153 pkscreener-0.44.20240419.279/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:06:29.708776 pkscreener-0.44.20240419.279/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25094 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9489 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     6185 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3237 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29416 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17603 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8120 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   111467 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    46418 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    79118 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-19 20:06:21.000000 pkscreener-0.44.20240419.279/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   118637 2024-04-19 20:01:40.000000 pkscreener-0.44.20240419.279/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-19 20:01:41.000000 pkscreener-0.44.20240419.279/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47947 2024-04-19 20:01:41.000000 pkscreener-0.44.20240419.279/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    21899 2024-04-19 20:01:41.000000 pkscreener-0.44.20240419.279/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:06:29.693153 pkscreener-0.44.20240419.279/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-19 20:06:29.000000 pkscreener-0.44.20240419.279/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-04-19 20:06:29.000000 pkscreener-0.44.20240419.279/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 20:06:29.000000 pkscreener-0.44.20240419.279/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-19 20:06:29.000000 pkscreener-0.44.20240419.279/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-19 20:06:29.000000 pkscreener-0.44.20240419.279/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-19 20:06:29.000000 pkscreener-0.44.20240419.279/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-19 20:06:29.708776 pkscreener-0.44.20240419.279/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-19 20:01:41.000000 pkscreener-0.44.20240419.279/setup.py
```

### Comparing `pkscreener-0.44.20240418.278/LICENSE` & `pkscreener-0.44.20240419.279/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/LICENSE-Others` & `pkscreener-0.44.20240419.279/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/PKG-INFO` & `pkscreener-0.44.20240419.279/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240418.278
+Version: 0.44.20240419.279
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240418.278.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240419.279.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.276/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.276/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.276/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240418.278/README.md` & `pkscreener-0.44.20240419.279/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.276/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.276/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.276/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240418.278/pkscreener/__init__.py` & `pkscreener-0.44.20240419.279/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/ConfigManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
         self.morninganalysiscandleduration = '1m'
         self.logger = None
         self.showPastStrategyData = False
         # This determines how many days apart the backtest calculations are run.
         # For example, for weekly backtest calculations, set this to 5 (5 days = 1 week)
         # For fortnightly, set this to 10 and so on (10 trading sessions = 2 weeks)
         self.backtestPeriodFactor = 1
+        self.defaultMonitorOptions = "X:12:9:2.5,|X:0:5:0:50:i 1m,X:12:2,X:12:5:0:30,X:12:6:3,X:12:6:7:1,X:12:6:8,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:23,X:12:24,X:12:10"
 
         self.daysToLookback = 22 * self.backtestPeriodFactor  # 1 month
         self.periods = [1,2,3,4,5,10,15,22,30]
         if self.maxBacktestWindow > self.periods[-1]:
             self.periods.extend(self.maxBacktestWindow)
 
     @property
```

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/MenuOptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     "10": "RSI MA Reversal",
     "0": "Cancel",
 }
 level3_X_ChartPattern_MenuDict = {
     "1": "Bullish Inside Bar (Flag) Pattern",
     "2": "Bearish Inside Bar (Flag) Pattern(Sell)",
     "3": "The Confluence (50 & 200 MA/EMA)",
-    "4": "VCP (Experimental)",
+    "4": "VCP (Volatility Contraction Pattern)",
     "5": "Buying at Trendline (Ideal for Swing/Mid/Long term)",
     "6": "Bollinger Bands (TTM) Squeeze",
     "7": "Candle-stick Patterns",
     "0": "Cancel",
 }
 
 level4_X_ChartPattern_BBands_SQZ_MenuDict = {
@@ -443,31 +443,32 @@
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            OutputControls().printOutput(
-                colorText.BOLD
-                + colorText.WARN
-                + "[+] Select a menu option:"
-                + colorText.END
-            )
-            OutputControls().printOutput(
-                colorText.BOLD
-                + menuText
-                + """
-
-    Enter your choice > (default is """
-                + colorText.WARN
-                + self.find("X").keyTextLabel()
-                + ") "
-                "" + colorText.END
-            )
+            if OutputControls().enableMultipleLineOutput:
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + colorText.WARN
+                    + "[+] Select a menu option:"
+                    + colorText.END
+                )
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + menuText
+                    + """
+
+        Enter your choice > (default is """
+                    + colorText.WARN
+                    + self.find("X").keyTextLabel()
+                    + ") "
+                    "" + colorText.END
+                )
             return menuText
 
     def renderLevel1_S_Menus(
         self, skip=[], asList=False, renderStyle=None, parent=None
     ):
         strategies = self.strategyNames
         counter = 1
@@ -486,28 +487,29 @@
             else MenuRenderStyle.THREE_PER_ROW,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            OutputControls().printOutput(
-                colorText.BOLD
-                + colorText.WARN
-                + "[+] Select a Strategy for Screening:"
-                + colorText.END
-            )
-            OutputControls().printOutput(
-                colorText.BOLD
-                + menuText
-                + """
+            if OutputControls().enableMultipleLineOutput:
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + colorText.WARN
+                    + "[+] Select a Strategy for Screening:"
+                    + colorText.END
+                )
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + menuText
+                    + """
 
-    Enter your choice > """
-                ""
-            )
+        Enter your choice > """
+                    ""
+                )
             return menuText
         
     def renderLevel1_X_Menus(
         self, skip=[], asList=False, renderStyle=None, parent=None
     ):
         menuText = self.fromDictionary(
             level1_X_MenuDict,
@@ -517,31 +519,32 @@
             else MenuRenderStyle.THREE_PER_ROW,
             skip=skip,
             parent=parent,
         ).render(asList=asList, coloredValues=["15"])
         if asList:
             return menuText
         else:
-            OutputControls().printOutput(
-                colorText.BOLD
-                + colorText.WARN
-                + "[+] Select an Index for Screening:"
-                + colorText.END
-            )
-            OutputControls().printOutput(
-                colorText.BOLD
-                + menuText
-                + """
-
-    Enter your choice > (default is """
-                + colorText.WARN
-                + self.find(str(configManager.defaultIndex)).keyTextLabel()
-                + ")  "
-                "" + colorText.END
-            )
+            if OutputControls().enableMultipleLineOutput:
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + colorText.WARN
+                    + "[+] Select an Index for Screening:"
+                    + colorText.END
+                )
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + menuText
+                    + """
+
+        Enter your choice > (default is """
+                    + colorText.WARN
+                    + self.find(str(configManager.defaultIndex)).keyTextLabel()
+                    + ")  "
+                    "" + colorText.END
+                )
             return menuText
 
     def renderLevel2_X_Menus(
         self, skip=[], asList=False, renderStyle=None, parent=None
     ):
         menuText = self.fromDictionary(
             level2_X_MenuDict,
@@ -551,28 +554,29 @@
             else MenuRenderStyle.TWO_PER_ROW,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            OutputControls().printOutput(
-                colorText.BOLD
-                + colorText.WARN
-                + "[+] Select a Criterion for Stock Screening: "
-                + colorText.END
-            )
-            OutputControls().printOutput(
-                colorText.BOLD
-                + menuText
-                + """
+            if OutputControls().enableMultipleLineOutput:
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + colorText.WARN
+                    + "[+] Select a Criterion for Stock Screening: "
+                    + colorText.END
+                )
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + menuText
+                    + """
 
-        """
-                + colorText.END
-            )
+            """
+                    + colorText.END
+                )
             return menuText
 
     def renderLevel3_X_Reversal_Menus(
         self, skip=[], asList=False, renderStyle=None, parent=None
     ):
         menuText = self.fromDictionary(
             level3_X_Reversal_MenuDict,
@@ -582,28 +586,29 @@
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            OutputControls().printOutput(
-                colorText.BOLD
-                + colorText.WARN
-                + "[+] Select an option: "
-                + colorText.END
-            )
-            OutputControls().printOutput(
-                colorText.BOLD
-                + menuText
-                + """
+            if OutputControls().enableMultipleLineOutput:
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + colorText.WARN
+                    + "[+] Select an option: "
+                    + colorText.END
+                )
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + menuText
+                    + """
 
-        """
-                + colorText.END
-            )
+            """
+                    + colorText.END
+                )
             return menuText
 
     def renderLevel3_X_ChartPattern_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
     ):
         menuText = self.fromDictionary(
             level3_X_ChartPattern_MenuDict,
@@ -613,28 +618,29 @@
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            OutputControls().printOutput(
-                colorText.BOLD
-                + colorText.WARN
-                + "[+] Select an option: "
-                + colorText.END
-            )
-            OutputControls().printOutput(
-                colorText.BOLD
-                + menuText
-                + """
+            if OutputControls().enableMultipleLineOutput:
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + colorText.WARN
+                    + "[+] Select an option: "
+                    + colorText.END
+                )
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + menuText
+                    + """
 
-        """
-                + colorText.END
-            )
+            """
+                    + colorText.END
+                )
             return menuText
 
     def renderLevel3_X_PopularStocks_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
     ):
         menuText = self.fromDictionary(
             level3_X_PopularStocks_MenuDict,
@@ -644,28 +650,29 @@
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            OutputControls().printOutput(
-                colorText.BOLD
-                + colorText.WARN
-                + "[+] Select an option: "
-                + colorText.END
-            )
-            OutputControls().printOutput(
-                colorText.BOLD
-                + menuText
-                + """
+            if OutputControls().enableMultipleLineOutput:
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + colorText.WARN
+                    + "[+] Select an option: "
+                    + colorText.END
+                )
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + menuText
+                    + """
 
-        """
-                + colorText.END
-            )
+            """
+                    + colorText.END
+                )
             return menuText
 
     def renderLevel3_X_StockPerformance_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
     ):
         menuText = self.fromDictionary(
             level3_X_StockPerformance_MenuDict,
@@ -675,28 +682,29 @@
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            OutputControls().printOutput(
-                colorText.BOLD
-                + colorText.WARN
-                + "[+] Select an option: "
-                + colorText.END
-            )
-            OutputControls().printOutput(
-                colorText.BOLD
-                + menuText
-                + """
+            if OutputControls().enableMultipleLineOutput:
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + colorText.WARN
+                    + "[+] Select an option: "
+                    + colorText.END
+                )
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + menuText
+                    + """
 
-        """
-                + colorText.END
-            )
+            """
+                    + colorText.END
+                )
             return menuText
 
     def renderLevel4_X_Lorenzian_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
     ):
         menuText = self.fromDictionary(
             level4_X_Lorenzian_MenuDict,
@@ -706,28 +714,29 @@
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            OutputControls().printOutput(
-                colorText.BOLD
-                + colorText.WARN
-                + "[+] Select an option: "
-                + colorText.END
-            )
-            OutputControls().printOutput(
-                colorText.BOLD
-                + menuText
-                + """
+            if OutputControls().enableMultipleLineOutput:
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + colorText.WARN
+                    + "[+] Select an option: "
+                    + colorText.END
+                )
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + menuText
+                    + """
 
-        """
-                + colorText.END
-            )
+            """
+                    + colorText.END
+                )
             return menuText
 
 
     def renderLevel4_X_ChartPattern_BBands_SQZ_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
     ):
         menuText = self.fromDictionary(
@@ -738,28 +747,29 @@
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            OutputControls().printOutput(
-                colorText.BOLD
-                + colorText.WARN
-                + "[+] Select an option: "
-                + colorText.END
-            )
-            OutputControls().printOutput(
-                colorText.BOLD
-                + menuText
-                + """
+            if OutputControls().enableMultipleLineOutput:
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + colorText.WARN
+                    + "[+] Select an option: "
+                    + colorText.END
+                )
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + menuText
+                    + """
 
-        """
-                + colorText.END
-            )
+            """
+                    + colorText.END
+                )
             return menuText
 
 
     def renderLevel4_X_ChartPattern_Confluence_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
     ):
         menuText = self.fromDictionary(
@@ -770,28 +780,29 @@
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
             return menuText
         else:
-            OutputControls().printOutput(
-                colorText.BOLD
-                + colorText.WARN
-                + "[+] Select an option: "
-                + colorText.END
-            )
-            OutputControls().printOutput(
-                colorText.BOLD
-                + menuText
-                + """
+            if OutputControls().enableMultipleLineOutput:
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + colorText.WARN
+                    + "[+] Select an option: "
+                    + colorText.END
+                )
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + menuText
+                    + """
 
-        """
-                + colorText.END
-            )
+            """
+                    + colorText.END
+                )
             return menuText
         
 # Fundamentally good compnaies but nearing 52 week low
 # https://www.tickertape.in/screener/equity/prebuilt/SCR0005
 
 # Dividend Gems
 # https://www.tickertape.in/screener/equity/prebuilt/SCR0027
```

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/ScreeningStatistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -992,20 +992,22 @@
             except (KeyError,IndexError):
                     pass
         else:
             if PKDateUtilities.currentDateTime().weekday() >= 5 or force:
                 security = None
                 # Refresh each saturday or sunday or when not found in saved data
                 try:
-                    security = Stock(stock,exchange=exchangeName)
+                    with SuppressOutput(suppress_stderr=True, suppress_stdout=True):
+                        security = Stock(stock,exchange=exchangeName)
                 except ValueError: # pragma: no cover
                     # We did not find the stock? It's okay. Move on to the next one.
                     pass
                 if security is not None:
-                    fv = security.fairValue()
+                    with SuppressOutput(suppress_stderr=True, suppress_stdout=True):
+                        fv = security.fairValue()
                     if fv is not None:
                         try:
                             fvResponseValue = fv["latestFairValue"]
                             if fvResponseValue is not None:
                                 fairValue = float(fvResponseValue)
                         except: # pragma: no cover
                             pass
@@ -1106,24 +1108,26 @@
         changeStatusDataInst = None
         netChangeMF = 0
         netChangeInst = 0
         latest_mfdate = None
         latest_instdate = None
         security = None
         try:
-            security = Stock(stock,exchange=exchangeName)
+            with SuppressOutput(suppress_stderr=True, suppress_stdout=True):
+                security = Stock(stock,exchange=exchangeName)
         except ValueError:
             # We did not find the stock? It's okay. Move on to the next one.
             pass
         if security is not None:
             try:
-                changeStatusRowsMF = security.mutualFundOwnership(top=5)
-                changeStatusRowsInst = security.institutionOwnership(top=5)
-                changeStatusDataMF = security.mutualFundFIIChangeData(changeStatusRowsMF)
-                changeStatusDataInst = security.mutualFundFIIChangeData(changeStatusRowsInst)
+                with SuppressOutput(suppress_stderr=True, suppress_stdout=True):
+                    changeStatusRowsMF = security.mutualFundOwnership(top=5)
+                    changeStatusRowsInst = security.institutionOwnership(top=5)
+                    changeStatusDataMF = security.mutualFundFIIChangeData(changeStatusRowsMF)
+                    changeStatusDataInst = security.mutualFundFIIChangeData(changeStatusRowsInst)
             except Exception as e:
                 self.default_logger.debug(e, exc_info=True)
                 # TypeError or ConnectionError because we could not find the stock or MFI data isn't available?
                 pass
             lastDayLastMonth = PKDateUtilities.last_day_of_previous_month(PKDateUtilities.currentDateTime())
             lastDayLastMonth = lastDayLastMonth.strftime("%Y-%m-%dT00:00:00.000")
             if changeStatusDataMF is not None and len(changeStatusDataMF) > 0:
```

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -823,15 +823,15 @@
     ):
         isIntraday = isIntraday or configManager.isIntradayConfig()
         exists, cache_file = tools.afterMarketStockDataExists(
             isIntraday, forceLoad=forceLoad
         )
         initialLoadCount = len(stockDict)
         isTrading = PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]
-        if (stockCodes is not None and len(stockCodes) > 0) and (isTrading or downloadOnly):
+        if (stockCodes is not None and len(stockCodes) > 0) and (isTrading or downloadOnly or not exists):
             stockDict = tools.downloadLatestData(stockDict,configManager,stockCodes,exchangeSuffix=exchangeSuffix)
             # return stockDict
 
         default_logger().info(
             f"Stock data cache file:{cache_file} exists ->{str(exists)}"
         )
         stockDataLoaded = False
```

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/classes/keys.py` & `pkscreener-0.44.20240419.279/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/courbd.ttf` & `pkscreener-0.44.20240419.279/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/globals.py` & `pkscreener-0.44.20240419.279/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 warnings.simplefilter("ignore", FutureWarning)
 import pandas as pd
 from alive_progress import alive_bar
 from PKDevTools.classes.Committer import Committer
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from PKDevTools.classes.log import default_logger #, tracelog
+from PKDevTools.classes.SuppressOutput import SuppressOutput
 from PKDevTools.classes.Telegram import (
     is_token_telegram_configured,
     send_document,
     send_message,
     send_photo
 )
 from PKNSETools.morningstartools.PKMorningstarDataFetcher import morningstarDataFetcher
@@ -535,17 +536,18 @@
             sleep(2)
             Utility.tools.clearScreen()
             return initPostLevel1Execution(indexOption, executeOption, retrial=True)
     return indexOption, executeOption
 
 def labelDataForPrinting(screenResults, saveResults, configManager, volumeRatio,executeOption, reversalOption):
     # Publish to gSheet with https://github.com/burnash/gspread
+    global menuChoiceHierarchy
     try:
-        sortKey = ["Volume"]
-        ascending = [False]
+        sortKey = ["Volume"] if "RSI" not in menuChoiceHierarchy else "RSI"
+        ascending = [False if "RSI" not in menuChoiceHierarchy else True]
         if executeOption == 21:
             if reversalOption in [3,5,6,7]:
                 sortKey = ["MFI"]
                 ascending = [reversalOption in [6,7]]
             elif reversalOption in [8,9]:
                 sortKey = ["FVDiff"]
                 ascending = [reversalOption in [9]]
@@ -1269,15 +1271,15 @@
                         screenResults,
                         saveResults,
                         selectedChoice,
                         menuChoiceHierarchy,
                         testing,
                         user=user,
                     )
-        if menuOption in ["X","C"]:
+        if menuOption in ["X","C"] and userPassedArgs.monitor is None:
             finishScreening(
                 downloadOnly,
                 testing,
                 stockDict,
                 configManager,
                 loadCount,
                 testBuild,
@@ -1324,15 +1326,17 @@
         analysis_df.reset_index(inplace=True)
         if 'index' in analysis_df.columns:
             analysis_df.drop('index', axis=1, inplace=True, errors="ignore")
         if optionalFinalOutcome_df is None:
             optionalFinalOutcome_df = analysis_df
         else:
             optionalFinalOutcome_df = pd.concat([optionalFinalOutcome_df, analysis_df], axis=0)
-        return optionalFinalOutcome_df
+        return optionalFinalOutcome_df, saveResults
+    elif userPassedArgs.monitor is not None:
+        return screenResults, saveResults
 
 def getLatestTradeDateTime(stockDict):
     stocks = list(stockDict.keys())
     stock = stocks[0]
     try:
         lastTradeDate = PKDateUtilities.currentDateTime().strftime("%Y-%m-%d")
         lastTradeTime_ist = PKDateUtilities.currentDateTime().strftime("%H:%M:%S")
@@ -1465,17 +1469,19 @@
         configManager.toggleConfig(candleDuration="1d", clearCache=False)
 
 def prepareStocksForScreening(testing, downloadOnly, listStockCodes, indexOption):
     if not downloadOnly:
         updateMenuChoiceHierarchy()
     if listStockCodes is None or len(listStockCodes) == 0:
         if indexOption >= 0 and indexOption <= 14:
-            listStockCodes = fetcher.fetchStockCodes(
-                            indexOption, stockCode=None
-                        )
+            shouldSuppress = not OutputControls().enableMultipleLineOutput
+            with SuppressOutput(suppress_stderr=shouldSuppress, suppress_stdout=shouldSuppress):
+                listStockCodes = fetcher.fetchStockCodes(
+                                indexOption, stockCode=None
+                            )
         elif indexOption == 15:
             OutputControls().printOutput(colorText.BOLD + "[+] Getting Stock Codes From NASDAQ... ", end="")
             nasdaq = PKNasdaqIndexFetcher(configManager)
             listStockCodes = nasdaq.fetchNasdaqIndexConstituents()
             if len(listStockCodes) > 10:
                 OutputControls().printOutput(
                     colorText.GREEN
@@ -1563,17 +1569,27 @@
             first_scan = False
     except KeyboardInterrupt:
         input("\nPress <Enter> to Continue...\n")
         return
 
 def handleRequestForSpecificStocks(options, indexOption):
     listStockCodes = []
+    strOptions = ""
+    if isinstance(options, list):
+        strOptions = ":".join(options)
+    else:
+        strOptions = options
+
     if indexOption == 0:
-        if len(options) >= 4:
-            listStockCodes = str(options[3]).split(",")
+        if len(strOptions) >= 4:
+            providedOptions = strOptions.split(":")
+            for option in providedOptions:
+                if not "".join(str(option).split(".")).isdecimal() and len(option.strip()) > 1:
+                    listStockCodes = str(option.strip()).split(",")
+                    break
     return listStockCodes
 
 def handleExitRequest(executeOption):
     if executeOption == "Z":
         input(
             colorText.BOLD
             + colorText.FAIL
@@ -1591,15 +1607,15 @@
             m2.renderForMenu(selMenu, asList=True)
             if executeOption is not None:
                 selMenu = m2.find(executeOption)
                 m3.renderForMenu(selMenu, asList=True)
 
 
 def updateMenuChoiceHierarchy():
-    global selectedChoice, menuChoiceHierarchy
+    global userPassedArgs, selectedChoice, menuChoiceHierarchy
     menuChoiceHierarchy = f'{level0MenuDict[selectedChoice["0"]].strip()}>{level1_X_MenuDict[selectedChoice["1"]].strip()}>{level2_X_MenuDict[selectedChoice["2"]].strip()}'
     if selectedChoice["2"] == "6":
         menuChoiceHierarchy = (
             menuChoiceHierarchy
             + f'>{level3_X_Reversal_MenuDict[selectedChoice["3"]].strip()}'
         )
         if len(selectedChoice) >= 5 and selectedChoice["3"] in ["7","10"]:
@@ -1623,28 +1639,32 @@
             + f'>{level4_X_ChartPattern_BBands_SQZ_MenuDict[selectedChoice["4"]].strip()}'
         )
     elif selectedChoice["2"] == "21":
         menuChoiceHierarchy = (
             menuChoiceHierarchy
             + f'>{level3_X_PopularStocks_MenuDict[selectedChoice["3"]].strip()}'
         )
+    intraday = "(Intraday)" if (userPassedArgs is not None and userPassedArgs.intraday) or configManager.isIntradayConfig() else ""
+    menuChoiceHierarchy = f"{menuChoiceHierarchy}{intraday}"
     OutputControls().printOutput(
         colorText.BOLD
         + colorText.FAIL
         + "[+] You chose: "
         + menuChoiceHierarchy
         + colorText.END
-        , enableMultipleLineOutput=True
     )
     default_logger().info(menuChoiceHierarchy)
+    return menuChoiceHierarchy
 
 def printNotifySaveScreenedResults(
     screenResults, saveResults, selectedChoice, menuChoiceHierarchy, testing, user=None
 ):
     global userPassedArgs, elapsed_time
+    if userPassedArgs.monitor is not None:
+        return
     MAX_ALLOWED = (100 if userPassedArgs.maxdisplayresults is None else min(int(userPassedArgs.maxdisplayresults),100)) if not testing else 1
     tabulated_backtest_summary = ""
     tabulated_backtest_detail = ""
     recordDate = PKDateUtilities.tradingDate().strftime('%Y-%m-%d') if (userPassedArgs.backtestdaysago is None) else (PKDateUtilities.nthPastTradingDateStringFromFutureDate(int(userPassedArgs.backtestdaysago)))
     if user is None and userPassedArgs.user is not None:
         user = userPassedArgs.user
     Utility.tools.clearScreen()
@@ -2246,23 +2266,24 @@
             + colorText.END
         )
         try:
             if filename is not None:
                 os.remove(filename)
         except Exception as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
-    OutputControls().printOutput(
-        colorText.BOLD
-        + colorText.GREEN
-        + f"[+] Screening Completed. Found {len(screenResults) if screenResults is not None else 0} results in {round(elapsed_time,2)} sec.! Press Enter to Continue.."
-        + colorText.END
-        , enableMultipleLineOutput=True
-    )
-    if defaultAnswer is None:
-        input("Press <Enter> to continue...")
+    if userPassedArgs.monitor is None:
+        OutputControls().printOutput(
+            colorText.BOLD
+            + colorText.GREEN
+            + f"[+] Screening Completed. Found {len(screenResults) if screenResults is not None else 0} results in {round(elapsed_time,2)} sec.! Press Enter to Continue.."
+            + colorText.END
+            , enableMultipleLineOutput=True
+        )
+        if defaultAnswer is None:
+            input("Press <Enter> to continue...")
 
 def sendGlobalMarketBarometer(userArgs=None):
     from pkscreener.classes import Barometer
     caption = "Global Market Barometer with India market Performance (top) and Valuation (bottom)"
     gmbPath = Barometer.getGlobalMarketBarometerValuation()
     try:
         if gmbPath is not None:
```

### Comparing `pkscreener-0.44.20240418.278/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240419.279/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240419.279/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240418.278/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240419.279/pkscreener/pkscreenercli.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,20 +50,20 @@
 
 from PKDevTools.classes import log as log
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from pkscreener import Imports
 from PKDevTools.classes.OutputControls import OutputControls
+from pkscreener.classes.MarketMonitor import MarketMonitor
 import pkscreener.classes.ConfigManager as ConfigManager
 
 multiprocessing.freeze_support()
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
 os.environ["AUTOGRAPH_VERBOSITY"] = "0"
-# from pkscreener.classes.IntradayMonitor import intradayMonitorInstance
 
 printenabled=False
 originalStdOut=None
 original__stdout=None
 cron_runs=0
 
 def decorator(func):
@@ -151,15 +151,14 @@
     "--intraday",
     help="Use Intraday configurations and use the candlestick duration that is passed. Acceptable values 1m, 5m, 10m, 15m, 1h etc.",
     required=False,
 )
 argParser.add_argument(
     "-m",
     "--monitor",
-    action="store_true",
     help="Monitor for intraday scanners and their results.",
     required=False,
 )
 argParser.add_argument(
     "--maxdisplayresults",
     help="Maximum number of results to display.",
     required=False,
@@ -212,15 +211,17 @@
     action="store_true",
     help="Run with full logging enabled",
     required=False,
 )
 argParser.add_argument("-v", action="store_true")  # Dummy Arg for pytest -v
 argsv = argParser.parse_known_args()
 args = argsv[0]
-
+results = None
+resultStocks = None
+plainResults = None
 configManager = ConfigManager.tools()
 
 
 def logFilePath():
     try:
         from PKDevTools.classes import Archiver
 
@@ -280,15 +281,15 @@
                 + colorText.FAIL
                 + "[+] Neither ta-lib nor pandas_ta was located. You need at least one of them to continue! \n[+] Please follow instructions from README file under PKScreener repo: https://github.com/pkjmesra/PKScreener"
                 + colorText.END
             )
             input("Press any key to try anyway...")
 
 def runApplication():
-    from pkscreener.globals import main, sendQuickScanResult, sendGlobalMarketBarometer
+    from pkscreener.globals import main, sendQuickScanResult, sendGlobalMarketBarometer, updateMenuChoiceHierarchy
     # From a previous call to main with args, it may have been mutated.
     # Let's stock to the original args passed by user
     argsv = argParser.parse_known_args()
     args = argsv[0]
     if args.runintradayanalysis:
         from pkscreener.classes.MenuOptions import menus
         runOptions = menus.allMenus(topLevel="C", index=12)
@@ -296,15 +297,15 @@
         import pkscreener.classes.Utility as Utility
         import pandas as pd
         # Delete any existing data from the previous run.
         configManager.deleteFileWithPattern(pattern="stock_data_*.pkl")
         for runOption in runOptions:
             args.options = runOption
             try:
-                optionalFinalOutcome_df = main(userArgs=args,optionalFinalOutcome_df=optionalFinalOutcome_df)
+                optionalFinalOutcome_df,_ = main(userArgs=args,optionalFinalOutcome_df=optionalFinalOutcome_df)
             except Exception as e:
                 OutputControls().printOutput(e)
                 if args.log:
                     import traceback
                     traceback.print_exc()
         if optionalFinalOutcome_df is not None:
             final_df = None
@@ -339,15 +340,46 @@
                                 pngName= f"PKS_IA_{PKDateUtilities.currentDateTime().strftime('%Y-%m-%d_%H:%M:%S')}",
                                 pngExtension= ".png"
                                 )
     else:
         if args.barometer:
             sendGlobalMarketBarometer(userArgs=args)
         else:
-            main(userArgs=args)
+            global results, resultStocks, plainResults
+            monitorOption_org = ""
+            if args.monitor:
+                args.answerdefault = args.answerdefault or 'Y'
+                monitorOption_org = MarketMonitor().currentMonitorOption()
+                monitorOption = monitorOption_org
+                lastComponent = monitorOption.split(":")[-1]
+                if "i" in lastComponent:
+                    # We need to switch to intraday scan
+                    monitorOption = monitorOption.replace(lastComponent,"")
+                    args.intraday = lastComponent.replace("i","").strip()
+                    configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
+                else:
+                    # We need to switch to daily scan
+                    args.intraday = False
+                    configManager.toggleConfig(candleDuration='1d', clearCache=False)
+                if monitorOption.startswith("|"):
+                    monitorOption = monitorOption.replace("|","")
+                    # We need to pipe the output from previous run into the next one
+                    if resultStocks is not None:
+                        resultStocks = ",".join(resultStocks)
+                        monitorOption = f"{monitorOption}:{resultStocks}"
+                args.options = monitorOption
+            try:
+                results, plainResults = main(userArgs=args)
+            except:
+                # Probably user cancelled an operation by choosing a cancel sub-menu somewhere
+                pass
+            if plainResults is not None and not plainResults.empty:
+                resultStocks = plainResults.index
+            if results is not None and args.monitor and len(monitorOption_org) > 0:
+                MarketMonitor().refresh(screen_df=results,screenOptions=monitorOption_org, chosenMenu=updateMenuChoiceHierarchy())
 
 
 def pkscreenercli():
     global originalStdOut
     if sys.platform.startswith("darwin"):
         try:
             multiprocessing.set_start_method("fork")
@@ -356,17 +388,20 @@
                 OutputControls().printOutput(
                     "[+] RuntimeError with 'multiprocessing'.\n[+] Please contact the Developer, if this does not work!"
                 )
                 OutputControls().printOutput(e)
                 traceback.print_exc()
             pass
 
-        OutputControls(enableMultipleLineOutput=(not args.monitor)).printOutput("",end="\r")
+        OutputControls(enableMultipleLineOutput=(args.monitor is None)).printOutput("",end="\r")
+        
     configManager.getConfig(ConfigManager.parser)
     # configManager.restartRequestsCache()
+    if args.monitor is not None:
+        MarketMonitor(monitors=args.monitor.split(",") if len(args.monitor)>5 else configManager.defaultMonitorOptions.split(","))
 
     if args.log or configManager.logsEnabled:
         setupLogger(shouldLog=True, trace=args.testbuild)
         if not args.prodbuild and args.answerdefault is None:
             input("Press <Enter> to continue...")
     else:
         if "PKDevTools_Default_Log_Level" in os.environ.keys():
```

### Comparing `pkscreener-0.44.20240418.278/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240419.279/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240418.278
+Version: 0.44.20240419.279
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240418.278.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240419.279.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.276/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.276/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.276/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240418.278/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240418.278/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240419.279/pkscreener.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 pkscreener.egg-info/top_level.txt
 pkscreener/classes/Backtest.py
 pkscreener/classes/Barometer.py
 pkscreener/classes/CandlePatterns.py
 pkscreener/classes/Changelog.py
 pkscreener/classes/ConfigManager.py
 pkscreener/classes/Fetcher.py
+pkscreener/classes/MarketMonitor.py
 pkscreener/classes/MarketStatus.py
 pkscreener/classes/MenuOptions.py
 pkscreener/classes/OtaUpdater.py
 pkscreener/classes/PKMarketOpenCloseAnalyser.py
 pkscreener/classes/PKScanRunner.py
 pkscreener/classes/PKScheduledTaskProgress.py
 pkscreener/classes/PKScheduler.py
```

### Comparing `pkscreener-0.44.20240418.278/setup.py` & `pkscreener-0.44.20240419.279/setup.py`

 * *Files identical despite different names*


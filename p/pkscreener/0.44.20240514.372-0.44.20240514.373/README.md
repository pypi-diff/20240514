# Comparing `tmp/pkscreener-0.44.20240514.372.tar.gz` & `tmp/pkscreener-0.44.20240514.373.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240514.372.tar", last modified: Tue May 14 12:00:47 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240514.373.tar", last modified: Tue May 14 12:14:53 2024, max compression
```

## Comparing `pkscreener-0.44.20240514.372.tar` & `pkscreener-0.44.20240514.373.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 12:00:47.979122 pkscreener-0.44.20240514.372/
--rw-rw-rw-   0        0        0     1086 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-14 12:00:47.979122 pkscreener-0.44.20240514.372/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 12:00:47.963500 pkscreener-0.44.20240514.372/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:00:47.979122 pkscreener-0.44.20240514.372/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34197 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11409 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    40469 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12432 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23700 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22221 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   154876 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56135 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    83233 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-14 12:00:37.000000 pkscreener-0.44.20240514.372/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   139167 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1024 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53019 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    31996 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:00:47.963500 pkscreener-0.44.20240514.372/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-14 12:00:47.000000 pkscreener-0.44.20240514.372/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-14 12:00:47.000000 pkscreener-0.44.20240514.372/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 12:00:47.000000 pkscreener-0.44.20240514.372/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-14 12:00:47.000000 pkscreener-0.44.20240514.372/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-14 12:00:47.000000 pkscreener-0.44.20240514.372/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-14 12:00:47.000000 pkscreener-0.44.20240514.372/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-14 12:00:47.979122 pkscreener-0.44.20240514.372/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:14:53.767097 pkscreener-0.44.20240514.373/
+-rw-rw-rw-   0        0        0     1086 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-14 12:14:53.767097 pkscreener-0.44.20240514.373/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 12:14:53.751484 pkscreener-0.44.20240514.373/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:14:53.767097 pkscreener-0.44.20240514.373/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34197 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11409 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    40469 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12432 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23700 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22221 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   154876 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56135 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    83233 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-14 12:14:43.000000 pkscreener-0.44.20240514.373/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   139167 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1024 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    53036 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    31996 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:14:53.751484 pkscreener-0.44.20240514.373/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-14 12:14:53.000000 pkscreener-0.44.20240514.373/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-14 12:14:53.000000 pkscreener-0.44.20240514.373/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 12:14:53.000000 pkscreener-0.44.20240514.373/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-14 12:14:53.000000 pkscreener-0.44.20240514.373/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-14 12:14:53.000000 pkscreener-0.44.20240514.373/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-14 12:14:53.000000 pkscreener-0.44.20240514.373/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-14 12:14:53.767097 pkscreener-0.44.20240514.373/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/setup.py
```

### Comparing `pkscreener-0.44.20240514.372/LICENSE` & `pkscreener-0.44.20240514.373/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/LICENSE-Others` & `pkscreener-0.44.20240514.373/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/PKG-INFO` & `pkscreener-0.44.20240514.373/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240514.372
+Version: 0.44.20240514.373
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240514.372.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240514.373.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240514.372/README.md` & `pkscreener-0.44.20240514.373/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240514.372/pkscreener/__init__.py` & `pkscreener-0.44.20240514.373/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/classes/keys.py` & `pkscreener-0.44.20240514.373/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/courbd.ttf` & `pkscreener-0.44.20240514.373/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/globals.py` & `pkscreener-0.44.20240514.373/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240514.373/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240514.373/pkscreener/pkscreenerbot.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,26 +111,26 @@
 m0 = menus()
 m1 = menus()
 m2 = menus()
 m3 = menus()
 int_timer = None
 
 TOP_LEVEL_SCANNER_MENUS = ["X", "B", "MI","DV"]
-TOP_LEVEL_SCANNER_SKIP_MENUS = ["M", "S", "G", "C", "T", "D", "I", "E", "U", "L", "Z"]
-INDEX_SKIP_MENUS = ["W","E","M","Z","0","2","3","4","6","7","9","10","13"]
+TOP_LEVEL_SCANNER_SKIP_MENUS = ["M", "S", "G", "C", "P", "T", "D", "I", "E", "U", "L", "Z"]
+INDEX_SKIP_MENUS = ["W","E","M","Z","0","2","3","4","6","7","9","10","13", "14"]
 SCANNER_SKIP_MENUS_1_TO_6 = ["0","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","31","32","42","M","Z"]
 SCANNER_SKIP_MENUS_7_TO_12 = ["0","1","2","3","4","5","6","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","31","32","42","M","Z"]
 SCANNER_SKIP_MENUS_13_TO_18 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","19","20","21","22","23","24","25","26","27","28","29","30","31","32","42","M","Z"]
 SCANNER_SKIP_MENUS_19_TO_25 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","22","26","27","28","29","30","31","32","42","M","Z"]
 SCANNER_SKIP_MENUS_26_TO_31 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","32","42","M","Z"]
 SCANNER_MENUS_WITH_NO_SUBMENUS = ["1","2","3","10","11","12","13","14","15","16","17","18","19","20","21","23","24","25","26","27","28","29","30","31","32"]
 SCANNER_MENUS_WITH_SUBMENU_SUPPORT = ["6", "7", "21"]
 
 INDEX_COMMANDS_SKIP_MENUS_SCANNER = ["W", "E", "M", "Z"]
-INDEX_COMMANDS_SKIP_MENUS_BACKTEST = ["W", "E", "M", "Z", "N", "0", "15"]
+INDEX_COMMANDS_SKIP_MENUS_BACKTEST = ["W", "E", "M", "Z", "N", "0", "14", "15"]
 UNSUPPORTED_COMMAND_MENUS =["22","42","M","Z"]
 SUPPORTED_COMMAND_MENUS = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","31","32"]
 
 def initializeIntradayTimer():
     try:
         if (not PKDateUtilities.isTodayHoliday()[0]):
             now = PKDateUtilities.currentDateTime()
```

### Comparing `pkscreener-0.44.20240514.372/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240514.373/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240514.373/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240514.372
+Version: 0.44.20240514.373
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240514.372.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240514.373.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240514.372/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240514.373/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.372/setup.py` & `pkscreener-0.44.20240514.373/setup.py`

 * *Files identical despite different names*


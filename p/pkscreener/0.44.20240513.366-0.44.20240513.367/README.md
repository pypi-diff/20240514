# Comparing `tmp/pkscreener-0.44.20240513.366.tar.gz` & `tmp/pkscreener-0.44.20240513.367.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240513.366.tar", last modified: Mon May 13 18:56:32 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240513.367.tar", last modified: Mon May 13 21:24:26 2024, max compression
```

## Comparing `pkscreener-0.44.20240513.366.tar` & `pkscreener-0.44.20240513.367.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 18:56:32.482043 pkscreener-0.44.20240513.366/
--rw-rw-rw-   0        0        0     1086 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-13 18:56:32.482043 pkscreener-0.44.20240513.366/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 18:56:32.450799 pkscreener-0.44.20240513.366/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:56:32.482043 pkscreener-0.44.20240513.366/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34185 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11236 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    36256 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12370 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23700 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22221 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18597 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   153935 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    55975 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    83233 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-13 18:56:24.000000 pkscreener-0.44.20240513.366/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   134008 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1024 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    51714 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    30550 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:56:32.466420 pkscreener-0.44.20240513.366/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-13 18:56:32.000000 pkscreener-0.44.20240513.366/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-13 18:56:32.000000 pkscreener-0.44.20240513.366/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 18:56:32.000000 pkscreener-0.44.20240513.366/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-13 18:56:32.000000 pkscreener-0.44.20240513.366/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-13 18:56:32.000000 pkscreener-0.44.20240513.366/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-13 18:56:32.000000 pkscreener-0.44.20240513.366/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-13 18:56:32.482043 pkscreener-0.44.20240513.366/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:24:26.253778 pkscreener-0.44.20240513.367/
+-rw-rw-rw-   0        0        0     1086 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-13 21:24:26.253778 pkscreener-0.44.20240513.367/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 21:24:26.238149 pkscreener-0.44.20240513.367/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:24:26.253778 pkscreener-0.44.20240513.367/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34185 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11236 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    36256 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12370 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23700 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22221 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18597 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   153935 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    55975 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    83233 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-13 21:24:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   134008 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1024 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    52954 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    30550 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:24:26.238149 pkscreener-0.44.20240513.367/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-13 21:24:26.000000 pkscreener-0.44.20240513.367/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-13 21:24:26.000000 pkscreener-0.44.20240513.367/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 21:24:26.000000 pkscreener-0.44.20240513.367/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-13 21:24:26.000000 pkscreener-0.44.20240513.367/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-13 21:24:26.000000 pkscreener-0.44.20240513.367/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-13 21:24:26.000000 pkscreener-0.44.20240513.367/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-13 21:24:26.253778 pkscreener-0.44.20240513.367/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-13 21:21:19.000000 pkscreener-0.44.20240513.367/setup.py
```

### Comparing `pkscreener-0.44.20240513.366/LICENSE` & `pkscreener-0.44.20240513.367/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/LICENSE-Others` & `pkscreener-0.44.20240513.367/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/PKG-INFO` & `pkscreener-0.44.20240513.367/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240513.366
+Version: 0.44.20240513.367
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240513.366.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240513.367.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.366/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.366/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.366/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240513.366/README.md` & `pkscreener-0.44.20240513.367/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.366/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.366/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.366/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240513.366/pkscreener/__init__.py` & `pkscreener-0.44.20240513.367/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/classes/keys.py` & `pkscreener-0.44.20240513.367/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/courbd.ttf` & `pkscreener-0.44.20240513.367/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/globals.py` & `pkscreener-0.44.20240513.367/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240513.367/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240513.367/pkscreener/pkscreenerbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,22 +40,28 @@
 """
 import os
 import html
 import json
 import logging
 import re
 import sys
+import threading
+try:
+    import thread
+except ImportError:
+    import _thread as thread
+
 import traceback
 from datetime import datetime
 from time import sleep
 from telegram import __version__ as TG_VER
 from telegram.constants import ParseMode
 
 start_time = datetime.now()
-MINUTES_5_IN_SECONDS = 300
+MINUTES_2_IN_SECONDS = 120
 OWNER_USER = "Itsonlypk"
 
 from PKDevTools.classes.Telegram import get_secrets
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from PKDevTools.classes.ColorText import colorText
 from pkscreener.classes.MenuOptions import MenuRenderStyle, menu, menus
 from pkscreener.classes.WorkflowManager import run_workflow
@@ -102,14 +108,15 @@
 # Callback data
 ONE, TWO, THREE, FOUR = range(4)
 
 m0 = menus()
 m1 = menus()
 m2 = menus()
 m3 = menus()
+int_timer = None
 
 TOP_LEVEL_SCANNER_MENUS = ["X", "B", "MI","DV"]
 TOP_LEVEL_SCANNER_SKIP_MENUS = ["M", "S", "G", "C", "T", "D", "I", "E", "U", "L", "Z"]
 INDEX_SKIP_MENUS = ["W","E","M","Z","0","2","3","4","6","7","9","10","13"]
 SCANNER_SKIP_MENUS_1_TO_6 = ["0","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_7_TO_12 = ["0","1","2","3","4","5","6","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_13_TO_18 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
@@ -119,14 +126,31 @@
 SCANNER_MENUS_WITH_SUBMENU_SUPPORT = ["6", "7", "21"]
 
 INDEX_COMMANDS_SKIP_MENUS_SCANNER = ["W", "E", "M", "Z"]
 INDEX_COMMANDS_SKIP_MENUS_BACKTEST = ["W", "E", "M", "Z", "N", "0", "15"]
 UNSUPPORTED_COMMAND_MENUS =["22","42","M","Z"]
 SUPPORTED_COMMAND_MENUS = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30"]
 
+def initializeIntradayTimer():
+    try:
+        if (not PKDateUtilities.isTodayHoliday()[0]):
+            now = PKDateUtilities.currentDateTime()
+            marketStartTime = PKDateUtilities.currentDateTime(simulate=True,hour=9,minute=15)
+            morning745am = PKDateUtilities.currentDateTime(simulate=True,hour=7,minute=45)
+            if now < marketStartTime and now >= morning745am: # Telegram bot might keep running beyond an hour. So let's start watching around 7:45AM
+                difference = (marketStartTime - now).total_seconds() + 1
+                global int_timer
+                int_timer = threading.Timer(difference, launchIntradayMonitor, args=[])
+                int_timer.start()
+            elif now >= marketStartTime:
+                launchIntradayMonitor()
+    except:
+        launchIntradayMonitor()
+        pass
+
 async def start(update: Update, context: ContextTypes.DEFAULT_TYPE, updatedResults=None, monitorIndex=0,chosenBotMenuOption="") -> int:
     """Send message on `/start`."""
     updateCarrier = None
     if update is None:
         return
     else:
         if update.callback_query is not None:
@@ -201,14 +225,17 @@
             os.remove(f"{filePath}_{index}.txt")
         except:
             pass
         index += 1
 
 def launchIntradayMonitor():
     from PKDevTools.classes import Archiver
+    global int_timer
+    if int_timer is not None:
+        int_timer.cancel()
     filePath = os.path.join(Archiver.get_user_outputs_dir(), "monitor_outputs")
     result_outputs = ""
     if (PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]) or ("PKDevTools_Default_Log_Level" in os.environ.keys() or sys.argv[0].endswith(".py")):
         result_outputs = "Starting up the monitor for this hour. Please try again after 30-40 seconds."
     else:
         result_outputs = f"{PKDateUtilities.currentDateTime()}\nIntraday Monitor is available only during the NSE trading hours! Please try during the next trading session."
         try:
@@ -651,20 +678,26 @@
     tb_string = "".join(tb_list)
     global start_time
     timeSinceStarted = datetime.now() - start_time
     if (
         "telegram.error.Conflict" in tb_string
     ):  # A newer 2nd instance was registered. We should politely shutdown.
         if (
-            timeSinceStarted.total_seconds() >= MINUTES_5_IN_SECONDS
+            timeSinceStarted.total_seconds() >= MINUTES_2_IN_SECONDS
         ):  # shutdown only if we have been running for over 5 minutes
             print(
                 f"Stopping due to conflict after running for {timeSinceStarted.total_seconds()/60} minutes."
             )
             try:
+                global int_timer
+                if int_timer is not None:
+                    int_timer.cancel()
+            except:
+                pass
+            try:
                 context.application.stop()
                 sys.exit(0)
             except RuntimeError:
                 context.application.shutdown()
             sys.exit(0)
         else:
             print("Other instance running!")
@@ -1126,14 +1159,14 @@
     # application.add_handler(MessageHandler(filters.COMMAND, command_handler))
     # Add ConversationHandler to application that will be used for handling updates
     addCommandsForMenuItems(application)
     application.add_handler(conv_handler)
     # ...and the error handler
     application.add_error_handler(error_handler)
     # Run the intraday monitor
-    launchIntradayMonitor()
+    initializeIntradayTimer()
     # Run the bot until the user presses Ctrl-C
     application.run_polling(allowed_updates=Update.ALL_TYPES)
 
 
 if __name__ == "__main__":
     runpkscreenerbot()
```

### Comparing `pkscreener-0.44.20240513.366/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240513.367/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240513.367/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240513.366
+Version: 0.44.20240513.367
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240513.366.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240513.367.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.366/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.366/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.366/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240513.366/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240513.367/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.366/setup.py` & `pkscreener-0.44.20240513.367/setup.py`

 * *Files identical despite different names*


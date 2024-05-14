# Comparing `tmp/pkscreener-0.44.20240513.368.tar.gz` & `tmp/pkscreener-0.44.20240513.369.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240513.368.tar", last modified: Mon May 13 22:34:45 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240513.369.tar", last modified: Mon May 13 23:42:35 2024, max compression
```

## Comparing `pkscreener-0.44.20240513.368.tar` & `pkscreener-0.44.20240513.369.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 22:34:45.847836 pkscreener-0.44.20240513.368/
--rw-rw-rw-   0        0        0     1086 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-13 22:34:45.847836 pkscreener-0.44.20240513.368/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 22:34:45.832308 pkscreener-0.44.20240513.368/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 22:34:45.847836 pkscreener-0.44.20240513.368/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34197 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11236 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    36472 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12432 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23700 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22221 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   154876 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56135 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    83233 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-13 22:34:37.000000 pkscreener-0.44.20240513.368/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   134256 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1024 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53019 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    30550 2024-05-13 22:30:20.000000 pkscreener-0.44.20240513.368/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-13 22:34:45.832308 pkscreener-0.44.20240513.368/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-13 22:34:45.000000 pkscreener-0.44.20240513.368/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-13 22:34:45.000000 pkscreener-0.44.20240513.368/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 22:34:45.000000 pkscreener-0.44.20240513.368/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-13 22:34:45.000000 pkscreener-0.44.20240513.368/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-13 22:34:45.000000 pkscreener-0.44.20240513.368/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-13 22:34:45.000000 pkscreener-0.44.20240513.368/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-13 22:34:45.847836 pkscreener-0.44.20240513.368/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-13 22:30:21.000000 pkscreener-0.44.20240513.368/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:42:35.690842 pkscreener-0.44.20240513.369/
+-rw-rw-rw-   0        0        0     1086 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-13 23:42:35.690842 pkscreener-0.44.20240513.369/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 23:42:35.675280 pkscreener-0.44.20240513.369/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:42:35.690842 pkscreener-0.44.20240513.369/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34197 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11236 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    36472 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12432 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23700 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22221 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   154876 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56135 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    83233 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-13 23:42:29.000000 pkscreener-0.44.20240513.369/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   134721 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1024 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    53019 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    30710 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:42:35.675280 pkscreener-0.44.20240513.369/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-13 23:42:35.000000 pkscreener-0.44.20240513.369/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-13 23:42:35.000000 pkscreener-0.44.20240513.369/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 23:42:35.000000 pkscreener-0.44.20240513.369/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-13 23:42:35.000000 pkscreener-0.44.20240513.369/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-13 23:42:35.000000 pkscreener-0.44.20240513.369/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-13 23:42:35.000000 pkscreener-0.44.20240513.369/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-13 23:42:35.690842 pkscreener-0.44.20240513.369/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-13 23:39:35.000000 pkscreener-0.44.20240513.369/setup.py
```

### Comparing `pkscreener-0.44.20240513.368/LICENSE` & `pkscreener-0.44.20240513.369/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/LICENSE-Others` & `pkscreener-0.44.20240513.369/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/PKG-INFO` & `pkscreener-0.44.20240513.369/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240513.368
+Version: 0.44.20240513.369
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240513.368.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240513.369.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.367/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.368/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.367/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.368/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.367/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.368/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240513.368/README.md` & `pkscreener-0.44.20240513.369/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.367/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.368/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.367/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.368/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.367/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.368/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240513.368/pkscreener/__init__.py` & `pkscreener-0.44.20240513.369/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/classes/keys.py` & `pkscreener-0.44.20240513.369/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/courbd.ttf` & `pkscreener-0.44.20240513.369/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/globals.py` & `pkscreener-0.44.20240513.369/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1460,26 +1460,29 @@
                 runOption = PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)
                 df = saveResults.copy()
                 df["LastTradeDate"], df["LastTradeTime"] = getLatestTradeDateTime(stockDictPrimary)
                 gClient.df_to_sheet(df=df,sheetName=runOption)
                 OutputControls().printOutput(f"{colorText.GREEN} => Done in {round(time.time()-begin,2)}s{colorText.END}")
     except:
         pass
-    if userPassedArgs.runintradayanalysis:
-        analysis_df = screenResults.copy()
-        analysis_df.reset_index(inplace=True)
-        if 'index' in analysis_df.columns:
-            analysis_df.drop('index', axis=1, inplace=True, errors="ignore")
-        if optionalFinalOutcome_df is None:
-            optionalFinalOutcome_df = analysis_df
+    if userPassedArgs is not None:
+        if userPassedArgs.runintradayanalysis:
+            analysis_df = screenResults.copy()
+            analysis_df.reset_index(inplace=True)
+            if 'index' in analysis_df.columns:
+                analysis_df.drop('index', axis=1, inplace=True, errors="ignore")
+            if optionalFinalOutcome_df is None:
+                optionalFinalOutcome_df = analysis_df
+            else:
+                optionalFinalOutcome_df = pd.concat([optionalFinalOutcome_df, analysis_df], axis=0)
+            return optionalFinalOutcome_df, saveResults
         else:
-            optionalFinalOutcome_df = pd.concat([optionalFinalOutcome_df, analysis_df], axis=0)
-        return optionalFinalOutcome_df, saveResults
-    else:
-        return screenResults, saveResults
+            existingTitle = f"{userPassedArgs.pipedtitle}|" if userPassedArgs.pipedtitle is not None else ""
+            userPassedArgs.pipedtitle = f'{existingTitle}{menuChoiceHierarchy.split(">")[-1]}'
+            return screenResults, saveResults
 
 def loadDatabaseOrFetch(downloadOnly, listStockCodes, menuOption, indexOption):
     global stockDictPrimary,stockDictSecondary, configManager, defaultAnswer, userPassedArgs, loadedStockData
     if menuOption not in ["C"]:
         stockDictPrimary = Utility.tools.loadStockData(
                     stockDictPrimary,
                     configManager,
@@ -1859,18 +1862,19 @@
         screenResults = screenResults[~screenResults.index.duplicated(keep='first')]
         saveResults = saveResults[~saveResults.index.duplicated(keep='first')]
         if "Stock" in screenResults.columns:
             screenResults.drop_duplicates(keep="first", inplace=True)
         if "Stock" in saveResults.columns:
             saveResults.drop_duplicates(keep="first", inplace=True)
 
+    reportTitle = f"{userPassedArgs.pipedtitle}|" if userPassedArgs is not None and userPassedArgs.pipedtitle is not None else ""
     OutputControls().printOutput(
         colorText.BOLD
         + colorText.FAIL
-        + f"[+] You chose: {menuChoiceHierarchy}"
+        + f"[+] You chose: {reportTitle}{menuChoiceHierarchy}"
         + colorText.END
         , enableMultipleLineOutput=True
     )
     pngName = f'PKS_{PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)}_{PKDateUtilities.currentDateTime().strftime("%d-%m-%y_%H.%M.%S")}'
     pngExtension = ".png"
     eligible = is_token_telegram_configured()
     targetDateG10k = prepareGrowthOf10kResults(saveResults, selectedChoice, menuChoiceHierarchy, testing, user, pngName, pngExtension, eligible)
@@ -1902,15 +1906,15 @@
             maxcolwidths=Utility.tools.getMaxColumnWidths(strategy_df)
         ).encode("utf-8").decode(STD_ENCODING)
         OutputControls().printOutput(addendumLabel)
         OutputControls().printOutput(tabulated_strategy)
     if screenResults is not None and len(screenResults) >= 1:
         choiceSegments = menuChoiceHierarchy.split(">")
         choiceSegments = f"{choiceSegments[-2]} > {choiceSegments[-1]}" if len(choiceSegments)>=4 else f"{choiceSegments[-1]}"
-        title = f'<b>{choiceSegments}</b>{"" if selectedChoice["0"] != "G" else " for Date:"+ targetDateG10k}'
+        title = f'<b>{reportTitle}{choiceSegments}</b>{"" if selectedChoice["0"] != "G" else " for Date:"+ targetDateG10k}'
         if (
             ("RUNNER" in os.environ.keys() and os.environ["RUNNER"] != "LOCAL_RUN_SCANNER")
             or "PKDevTools_Default_Log_Level" in os.environ.keys()
         ):
             if eligible:
                 # There's no need to save data locally.
                 # This scan must have been triggered by github workflow by a user or scheduled job
@@ -1963,15 +1967,15 @@
                         tablefmt=colorText.No_Pad_GridFormat,
                         maxcolwidths=[None,None,4,3]
                     ).encode("utf-8").decode(STD_ENCODING).replace("-K-----S-----C-----R","-K-----S----C---R").replace("%  ","% ").replace("=K=====S=====C=====R","=K=====S====C===R").replace("Vol  |","Vol|").replace("x  ","x")
                     caption_results = caption_results.replace("-E-----N-----E-----R","-E-----N----E---R").replace("=E=====N=====E=====R","=E=====N====E===R")
                     caption = f"{caption}.Open attached image for more. Samples:<pre>{caption_results}</pre>{elapsed_text}" #<i>Author is <u><b>NOT</b> a SEBI registered financial advisor</u> and MUST NOT be deemed as one.</i>"
                 if not testing: # and not userPassedArgs.runintradayanalysis:
                     sendQuickScanResult(
-                        menuChoiceHierarchy,
+                        f"{reportTitle}{menuChoiceHierarchy}",
                         user,
                         tabulated_results,
                         markdown_results,
                         caption,
                         pngName,
                         pngExtension,
                         addendum=tabulated_strategy,
```

### Comparing `pkscreener-0.44.20240513.368/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240513.369/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240513.369/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240513.369/pkscreener/pkscreenercli.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,14 +230,19 @@
     "-l",
     "--log",
     action="store_true",
     help="Run with full logging enabled",
     required=False,
 )
 argParser.add_argument("-v", action="store_true")  # Dummy Arg for pytest -v
+argParser.add_argument(
+    "--pipedtitle",
+    help="Piped Titles",
+    required=False,
+)
 argsv = argParser.parse_known_args()
 args = argsv[0]
 results = None
 resultStocks = None
 plainResults = None
 start_time = None
 dbTimestamp = None
@@ -498,15 +503,16 @@
             # We need to pipe the output from previous run into the next one
             if prevOutput is not None and not prevOutput.empty:
                 prevOutput_results = prevOutput[~prevOutput.index.duplicated(keep='first')]
                 prevOutput_results = prevOutput_results.index
                 prevOutput_results = ",".join(prevOutput_results)
                 monitorOption = f"{monitorOption}:{prevOutput_results}"
         args.options = monitorOption.replace("::",":")
-        args.options = args.options + ":D:;".join(nextOnes[2:])
+        args.options = args.options + ":D:;" + ":D:;".join(nextOnes[2:])
+        args.options = args.options.replace("::",":")
         return True
     return False
 
 def pkscreenercli():
     global originalStdOut
     if sys.platform.startswith("darwin"):
         try:
```

### Comparing `pkscreener-0.44.20240513.368/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240513.369/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240513.368
+Version: 0.44.20240513.369
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240513.368.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240513.369.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.367/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.368/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.367/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.368/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.367/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.368/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240513.368/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240513.369/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.368/setup.py` & `pkscreener-0.44.20240513.369/setup.py`

 * *Files identical despite different names*


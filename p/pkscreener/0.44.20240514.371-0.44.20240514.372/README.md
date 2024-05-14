# Comparing `tmp/pkscreener-0.44.20240514.371.tar.gz` & `tmp/pkscreener-0.44.20240514.372.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240514.371.tar", last modified: Tue May 14 06:19:11 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240514.372.tar", last modified: Tue May 14 12:00:47 2024, max compression
```

## Comparing `pkscreener-0.44.20240514.371.tar` & `pkscreener-0.44.20240514.372.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 06:19:11.162287 pkscreener-0.44.20240514.371/
--rw-rw-rw-   0        0        0     1086 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-14 06:19:11.162287 pkscreener-0.44.20240514.371/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 06:19:11.146666 pkscreener-0.44.20240514.371/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 06:19:11.162287 pkscreener-0.44.20240514.371/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34197 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11409 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    36472 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12432 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23700 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22221 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   154876 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56135 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    83233 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-14 06:19:01.000000 pkscreener-0.44.20240514.371/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   134870 2024-05-14 06:13:50.000000 pkscreener-0.44.20240514.371/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1024 2024-05-14 06:13:51.000000 pkscreener-0.44.20240514.371/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53019 2024-05-14 06:13:51.000000 pkscreener-0.44.20240514.371/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    30710 2024-05-14 06:13:51.000000 pkscreener-0.44.20240514.371/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-14 06:19:11.146666 pkscreener-0.44.20240514.371/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-14 06:19:11.000000 pkscreener-0.44.20240514.371/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-14 06:19:11.000000 pkscreener-0.44.20240514.371/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 06:19:11.000000 pkscreener-0.44.20240514.371/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-14 06:19:11.000000 pkscreener-0.44.20240514.371/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-14 06:19:11.000000 pkscreener-0.44.20240514.371/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-14 06:19:11.000000 pkscreener-0.44.20240514.371/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-14 06:19:11.162287 pkscreener-0.44.20240514.371/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-14 06:13:51.000000 pkscreener-0.44.20240514.371/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:00:47.979122 pkscreener-0.44.20240514.372/
+-rw-rw-rw-   0        0        0     1086 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-14 12:00:47.979122 pkscreener-0.44.20240514.372/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 12:00:47.963500 pkscreener-0.44.20240514.372/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:00:47.979122 pkscreener-0.44.20240514.372/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34197 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11409 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    40469 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12432 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23700 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22221 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   154876 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56135 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    83233 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-14 12:00:37.000000 pkscreener-0.44.20240514.372/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   139167 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1024 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    53019 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    31996 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:00:47.963500 pkscreener-0.44.20240514.372/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-14 12:00:47.000000 pkscreener-0.44.20240514.372/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-14 12:00:47.000000 pkscreener-0.44.20240514.372/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 12:00:47.000000 pkscreener-0.44.20240514.372/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-14 12:00:47.000000 pkscreener-0.44.20240514.372/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-14 12:00:47.000000 pkscreener-0.44.20240514.372/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-14 12:00:47.000000 pkscreener-0.44.20240514.372/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-14 12:00:47.979122 pkscreener-0.44.20240514.372/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-14 11:55:38.000000 pkscreener-0.44.20240514.372/setup.py
```

### Comparing `pkscreener-0.44.20240514.371/LICENSE` & `pkscreener-0.44.20240514.372/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/LICENSE-Others` & `pkscreener-0.44.20240514.372/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/PKG-INFO` & `pkscreener-0.44.20240514.372/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240514.371
+Version: 0.44.20240514.372
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240514.371.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240514.372.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.370/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.370/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.370/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240514.371/README.md` & `pkscreener-0.44.20240514.372/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.370/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.370/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.370/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240514.371/pkscreener/__init__.py` & `pkscreener-0.44.20240514.372/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/MenuOptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,24 +40,50 @@
 level0MenuDict = {
     "X": "Scanners",
     "M": "Monitor Intraday",
     "S": "Strategies",
     "B": "Backtests",
     "G": "Growth of 10k",
     "C": "Analyse morning vs close outcomes",
+    "P": "Piped Scanners",
     "T": "~",
     "D": "Download Daily OHLC Data for the Past Year",
     "I": "Download Intraday OHLC Data for the Last Trading Day",
     "E": "Edit user configuration",
     "Y": "View your user configuration",
     "U": "Check for software update",
     "L": "Collect Logs for Debugging",
     "H": "Help / About Developer",
     "Z": "Exit (Ctrl + C)",
 }
+level1_P_MenuDict = {
+    "1": "Predefined Piped Scanners",
+    "2": "Define my custom Piped Scanner",
+    "M": "Back to the Top/Main menu",
+}
+level2_P_MenuDict = {
+    "1": "Volume Scanners | High Momentum | ATR Cross",
+    "2": "Volume Scanners | High Momentum",
+    "3": "Volume Scanners | ATR Cross",
+    "4": "Volume Scanners | High Bid/Ask Build Up",
+    "5": "High Momentum | ATR Cross",
+    "6": "High Momentum | ATR Trailing Stop",
+    "7": "ATR Cross | ATR Trailing Stop",
+
+    "M": "Back to the Top/Main menu",
+}
+PIPED_SCANNERS = {"1": "-a y -e -o 'X:12:9:2.5:;|X:0:31:;|X:0:27:'",
+                  "2": "-a y -e -o 'X:12:9:2.5:;|X:0:31:'",
+                  "3": "-a y -e -o 'X:12:9:2.5:;|X:0:27:'",
+                  "4": "-a y -e -o 'X:12:9:2.5:;|X:0:29:'",
+                  "5": "-a y -e -o 'X:12:31:;|X:0:27:'",
+                  "6": "-a y -e -o 'X:12:31:;|X:0:30:'",
+                  "7": "-a y -e -o 'X:12:27:;|X:0:30:'",
+                  }
+
 level1_T_MenuDict = {
     "L": "Long Term",
     "S": "Short Term (Intraday)",
     "M": "Back to the Top/Main menu",
 }
 # Valid periods: 1d,5d,1mo,3mo,6mo,1y,2y,5y,10y,ytd,max
 # Valid intervals: 1m,2m,5m,15m,30m,60m,90m,1h,1d,5d,1wk,1mo,3mo
@@ -413,14 +439,21 @@
                 if selectedMenu.menuKey in ["T"]:
                     return self.renderLevel1_T_Menus(
                         skip=skip,
                         asList=asList,
                         renderStyle=renderStyle,
                         parent=selectedMenu,
                     )
+                elif selectedMenu.menuKey in ["P"]:
+                    return self.renderLevel1_P_Menus(
+                        skip=skip,
+                        asList=asList,
+                        renderStyle=renderStyle,
+                        parent=selectedMenu,
+                    )
                 else:
                     # sub-menu of the top level main selected menu
                     return self.renderLevel1_X_Menus(
                         skip=skip,
                         asList=asList,
                         renderStyle=renderStyle,
                         parent=selectedMenu,
@@ -438,14 +471,21 @@
                     elif selectedMenu.menuKey in ["S"]:
                         return self.level2_T_MenuDict_S(
                             skip=skip,
                             asList=asList,
                             renderStyle=renderStyle,
                             parent=selectedMenu,
                         )
+                elif selectedMenu.parent.menuKey in ["P"]:
+                    return self.renderLevel2_P_Menus(
+                        skip=skip,
+                        asList=asList,
+                        renderStyle=renderStyle,
+                        parent=selectedMenu,
+                    )
                 else:
                     # next levelsub-menu of the selected sub-menu
                     return self.renderLevel2_X_Menus(
                         skip=skip,
                         asList=asList,
                         renderStyle=renderStyle,
                         parent=selectedMenu,
@@ -522,15 +562,15 @@
                 default_logger().debug(e, exc_info=True)
                 return None
         return None
 
     def renderLevel0Menus(self, asList=False, renderStyle=None, parent=None, skip=None):
         menuText = self.fromDictionary(
             level0MenuDict,
-            renderExceptionKeys=["T", "E", "U", "Z", "L", "D"],
+            renderExceptionKeys=["P", "T", "E", "U", "Z", "L", "D"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
@@ -632,15 +672,85 @@
     Enter your choice > (default is """
                     + colorText.WARN
                     + self.find(defaultKey).keyTextLabel()
                     + ")  "
                     "" + colorText.END
                 )
             return menuText
-                
+        
+    def renderLevel1_P_Menus(
+        self, skip=[], asList=False, renderStyle=None, parent=None
+    ):
+        menuText = self.fromDictionary(
+            level1_P_MenuDict,
+            renderExceptionKeys=["M"],
+            renderStyle=renderStyle
+            if renderStyle is not None
+            else MenuRenderStyle.STANDALONE,
+            skip=skip,
+            parent=parent,
+        ).render(asList=asList, coloredValues=["2"])
+        if asList:
+            return menuText
+        else:
+            if OutputControls().enableMultipleLineOutput:
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + colorText.WARN
+                    + "[+] Select an option:"
+                    + colorText.END
+                )
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + menuText
+                    + """
+
+    Enter your choice > (default is """
+                    + colorText.WARN
+                    + self.find('1').keyTextLabel()
+                    + ")  "
+                    "" + colorText.END
+                )
+            return menuText
+
+    def renderLevel2_P_Menus(
+        self, skip=[], asList=False, renderStyle=None, parent=None
+    ):
+        menuText = self.fromDictionary(
+            level2_P_MenuDict,
+            renderExceptionKeys=["M"],
+            renderStyle=renderStyle
+            if renderStyle is not None
+            else MenuRenderStyle.STANDALONE,
+            skip=skip,
+            parent=parent,
+        ).render(asList=asList)
+        if asList:
+            return menuText
+        else:
+            if OutputControls().enableMultipleLineOutput:
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + colorText.WARN
+                    + "[+] Select a scanner:"
+                    + colorText.END
+                )
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + menuText
+                    + """
+
+    Enter your choice > (default is """
+                    + colorText.WARN
+                    + self.find('1').keyTextLabel()
+                    + ")  "
+                    "" + colorText.END
+                )
+            return menuText
+        
     def renderLevel1_X_Menus(
         self, skip=[], asList=False, renderStyle=None, parent=None
     ):
         menuText = self.fromDictionary(
             level1_X_MenuDict,
             renderExceptionKeys=["W", "0", "M", "15"],
             renderStyle=renderStyle
```

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/classes/keys.py` & `pkscreener-0.44.20240514.372/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/courbd.ttf` & `pkscreener-0.44.20240514.372/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/globals.py` & `pkscreener-0.44.20240514.372/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,16 @@
     level3_X_PopularStocks_MenuDict,
     level3_X_Reversal_MenuDict,
     level4_X_Lorenzian_MenuDict,
     level4_X_ChartPattern_Confluence_MenuDict,
     level4_X_ChartPattern_BBands_SQZ_MenuDict,
     menus,
     MAX_SUPPORTED_MENU_OPTION,
-    MAX_MENU_OPTION
+    MAX_MENU_OPTION,
+    PIPED_SCANNERS
 )
 from pkscreener.classes.OtaUpdater import OTAUpdater
 from pkscreener.classes.Portfolio import PortfolioCollection
 from pkscreener.classes.PKTask import PKTask
 from pkscreener.classes.PKScheduler import PKScheduler
 from pkscreener.classes.PKScanRunner import PKScanRunner
 from pkscreener.classes.PKMarketOpenCloseAnalyser import PKMarketOpenCloseAnalyser
@@ -477,14 +478,16 @@
                     + colorText.END
                 )
                 sys.exit(0)
             elif selectedMenu.menuKey in ["B", "C", "G", "H", "U", "T", "S", "E", "X", "Y", "M", "D", "I", "L"]:
                 Utility.tools.clearScreen(forceTop=True)
                 selectedChoice["0"] = selectedMenu.menuKey
                 return selectedMenu
+            elif selectedMenu.menuKey in ["P"]:
+                return selectedMenu
     except KeyboardInterrupt:
         raise KeyboardInterrupt
     except Exception as e:  # pragma: no cover
         default_logger().debug(e, exc_info=True)
         showOptionErrorMessage()
         return initExecution()
 
@@ -770,15 +773,55 @@
             sleep(2)
             os.system(f"{launcher} -a Y -e -d -i 1m")
         elif menuOption in ["L"]:
             OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener to collect logs. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -l{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit at any time.{colorText.END}")
             sleep(2)
             os.system(f"{launcher} -a Y -l")
         sys.exit(0)
-    elif menuOption in ["X", "T", "E", "Y", "U", "H", "C"]:
+    if menuOption in ["P"]:
+        selectedMenu = m0.find(menuOption)
+        m1.renderForMenu(selectedMenu)
+        predefinedOption = input(colorText.BOLD + colorText.FAIL + "[+] Select option: ") or "1"
+        OutputControls().printOutput(colorText.END, end="")
+        if predefinedOption not in ["1","2"]:
+            return None, None
+        if predefinedOption == "1":
+            selectedMenu = m1.find(predefinedOption)
+            m2.renderForMenu(selectedMenu=selectedMenu)
+            selPredefinedOption = input(colorText.BOLD + colorText.FAIL + "[+] Select option: ") or "1"
+            OutputControls().printOutput(colorText.END, end="")
+            if selPredefinedOption in ["1","2","3","4","5","6","7"]:
+                scannerOption = PIPED_SCANNERS[selPredefinedOption]
+                if userPassedArgs.pipedmenus is not None:
+                    chosenOptions = scannerOption.split("-o ")[1]
+                    userPassedArgs.options = chosenOptions.replace("'","")
+                    return addOrRunPipedMenus()
+                launcher = sys.argv[0]
+                launcher = f"python3.11 {launcher}" if launcher.endswith(".py") else launcher
+                OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener with piped scanners. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} {scannerOption}{colorText.END}")
+                sleep(2)
+                os.system(f"{launcher} {scannerOption}")
+                OutputControls().printOutput(
+                        colorText.GREEN
+                        + f"[+] Finished running all piped scanners!"
+                        + colorText.END
+                    )
+                if defaultAnswer is None:
+                    input("Press <Enter> to exit...")
+                sys.exit(0)
+            else:
+                return None, None
+        elif predefinedOption == "2":
+            # User chose custom
+            menuOption = "X" # Let's have the user choose various scan options
+            selectedMenu = m0.find(menuOption)
+            selectedChoice["0"] = selectedMenu.menuKey
+            if userPassedArgs.pipedmenus is None:
+                userPassedArgs.pipedmenus = ""
+    if menuOption in ["X", "T", "E", "Y", "U", "H", "C"]:
         # Print Level 2 menu options
         menuOption, indexOption, executeOption, selectedChoice = getScannerMenuChoices(
             testBuild or testing,
             downloadOnly,
             startupoptions,
             menuOption=menuOption,
             indexOption=indexOption,
@@ -1234,14 +1277,16 @@
             )
             input("Exiting now...")
             sys.exit(0)
         if userPassedArgs.options is None or len(userPassedArgs.options) == 0:
             userPassedArgs.options = ""
             for choice in selectedChoice.keys():
                 userPassedArgs.options = (f"{userPassedArgs.options}:" if len(userPassedArgs.options) > 0  else '') + f"{selectedChoice[choice]}"
+        if userPassedArgs.pipedmenus is not None:
+            return addOrRunPipedMenus()
 
         if (menuOption in ["X", "B", "G", "S"] and not loadedStockData) or (
             # not downloadOnly
             # and not PKDateUtilities.isTradingTime()
             # and 
             configManager.cacheEnabled
             and not loadedStockData
@@ -1565,14 +1610,45 @@
                 task.long_running_fn(*(task,))
         for task in tasksList:
             if task.result is not None:
                 showBacktestResults(task.result, sortKey=None, optionalName=task.taskName)
     
     return summary_df,sorting,sortKeys
 
+def addOrRunPipedMenus():
+    global userPassedArgs
+    # User must have selected menu "P" earlier
+    savedPipes = f"{userPassedArgs.pipedmenus}:;|" if len(userPassedArgs.pipedmenus) > 0 else ""
+    userPassedArgs.pipedmenus = f"{savedPipes}{userPassedArgs.options}"
+    userPassedArgs.pipedmenus = userPassedArgs.pipedmenus.replace("::",":D:")
+    OutputControls().printOutput(
+            colorText.GREEN
+            + f"[+] {len(userPassedArgs.pipedmenus.split('|'))} Scanners piped so far: {colorText.END}{colorText.WARN+userPassedArgs.pipedmenus+colorText.END}\n{colorText.GREEN}[+] Do you want to add any more scanners into the pipe?"
+            + colorText.END
+        )
+    shouldAddMoreIntoPipe = input(colorText.FAIL + "[+] Select [Y/N] (Default:N): " + colorText.END) or 'n'
+    if shouldAddMoreIntoPipe.lower() != 'y':
+        launcher = sys.argv[0]
+        launcher = f"python3.11 {launcher}" if launcher.endswith(".py") else launcher
+        OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener with piped scanners. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -e -o '{userPassedArgs.pipedmenus}'{colorText.END}")
+        sleep(2)
+        os.system(f"{launcher} -a Y -e -o '{userPassedArgs.pipedmenus}'")
+        userPassedArgs.pipedmenus = None
+        OutputControls().printOutput(
+                colorText.GREEN
+                + f"[+] Finished running all piped scanners!"
+                + colorText.END
+            )
+        if defaultAnswer is None:
+            input("Press <Enter> to exit...")
+        sys.exit(0)
+    else:
+        userPassedArgs.options = None
+        return None, None
+    
 def prepareGroupedXRay(backtestPeriod, backtest_df):
     df_grouped = backtest_df.groupby("Date")
     userPassedArgs.backtestdaysago = backtestPeriod
     df_xray = None
     groupCounter = 0
     tasksList=[]
     for calcForDate, df_group in df_grouped:
@@ -1753,20 +1829,21 @@
         input("\nPress <Enter> to Continue...\n")
         return
 
 def handleRequestForSpecificStocks(options, indexOption):
     listStockCodes = []
     strOptions = ""
     if isinstance(options, list):
-        strOptions = ":".join(options)
+        strOptions = ":".join(options).split(";")[0]
     else:
-        strOptions = options
-
+        strOptions = options.split(";")[0]
+    
     if indexOption == 0:
         if len(strOptions) >= 4:
+            strOptions = strOptions.replace(":D:",":").replace(";","")
             providedOptions = strOptions.split(":")
             for option in providedOptions:
                 if not "".join(str(option).split(".")).isdecimal() and len(option.strip()) > 1:
                     listStockCodes = str(option.strip()).split(",")
                     break
     return listStockCodes
```

### Comparing `pkscreener-0.44.20240514.371/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240514.372/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240514.372/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240514.372/pkscreener/pkscreenercli.py`

 * *Files 5% similar despite different names*

```diff
@@ -235,14 +235,19 @@
 )
 argParser.add_argument("-v", action="store_true")  # Dummy Arg for pytest -v
 argParser.add_argument(
     "--pipedtitle",
     help="Piped Titles",
     required=False,
 )
+argParser.add_argument(
+    "--pipedmenus",
+    help="Piped Menus",
+    required=False,
+)
 argsv = argParser.parse_known_args()
 args = argsv[0]
 results = None
 resultStocks = None
 plainResults = None
 start_time = None
 dbTimestamp = None
@@ -328,16 +333,22 @@
             )
             input("Press any key to try anyway...")
 
 def runApplication():
     from pkscreener.globals import main, sendQuickScanResult,sendMessageToTelegramChannel, sendGlobalMarketBarometer, updateMenuChoiceHierarchy, isInterrupted, refreshStockData, closeWorkersAndExit
     # From a previous call to main with args, it may have been mutated.
     # Let's stock to the original args passed by user
+    try:
+        savedPipedArgs = None
+        savedPipedArgs = args.pipedmenus if args is not None and args.pipedmenus is not None else None
+    except:
+        pass
     argsv = argParser.parse_known_args()
     args = argsv[0]
+    args.pipedmenus = savedPipedArgs
     if args.options is not None:
         args.options = args.options.replace("::",":")
     if args.runintradayanalysis:
         from pkscreener.classes.MenuOptions import menus
         runOptions = menus.allMenus(topLevel="C", index=12)
         optionalFinalOutcome_df = None
         import pkscreener.classes.Utility as Utility
@@ -450,40 +461,56 @@
                     # Load the stock data afresh for each cycle
                     refreshStockData(args.options)
             try: 
                 results = None
                 plainResults = None
                 resultStocks = None
                 results, plainResults = main(userArgs=args)
+                if args.pipedmenus is not None:
+                    while args.pipedmenus is not None:
+                        main(userArgs=args)
+                    sys.exit(0)
                 if isInterrupted():
                     closeWorkersAndExit()
                     removeMonitorFile()
                     sys.exit(0)
-                while pipeResults(plainResults,args):
-                    results, plainResults = main(userArgs=args)
+                runPipedScans = True
+                while runPipedScans:
+                    runPipedScans = pipeResults(plainResults,args)
+                    if runPipedScans:
+                        results, plainResults = main(userArgs=args)
+                    else:
+                        OutputControls().printOutput(
+                                colorText.GREEN
+                                + f"[+] Finished running all piped scanners! Try reducing number of piped scans if no stocks could be found eventually."
+                                + colorText.END
+                            )
+                        if args.answerdefault is None:
+                            input("Press <Enter> to continue...")
             except SystemExit:
                 closeWorkersAndExit()
                 removeMonitorFile()
                 sys.exit(0)
             except Exception as e:
                 default_logger().debug(e, exc_info=True)
                 # Probably user cancelled an operation by choosing a cancel sub-menu somewhere
                 pass
             if plainResults is not None and not plainResults.empty:
                 plainResults = plainResults[~plainResults.index.duplicated(keep='first')]
                 results = results[~results.index.duplicated(keep='first')]
                 resultStocks = plainResults.index
-            if args.monitor:
+            if args.monitor is not None:
                 MarketMonitor().saveMonitorResultStocks(plainResults)
-            if results is not None and args.monitor and len(monitorOption_org) > 0:
-                MarketMonitor().refresh(screen_df=results,screenOptions=monitorOption_org, chosenMenu=updateMenuChoiceHierarchy(),dbTimestamp=f"{dbTimestamp} | CycleTime:{elapsed_time}s",telegram=args.telegram)
+                if results is not None and len(monitorOption_org) > 0:
+                    MarketMonitor().refresh(screen_df=results,screenOptions=monitorOption_org, chosenMenu=updateMenuChoiceHierarchy(),dbTimestamp=f"{dbTimestamp} | CycleTime:{elapsed_time}s",telegram=args.telegram)
 
 
 def pipeResults(prevOutput,args):
     nextOnes = args.options.split(";")
+    hasFoundStocks = False
     if len(nextOnes) > 1:
         monitorOption = nextOnes[1]
         if len(monitorOption) == 0:
             return False
         lastComponent = monitorOption.split(":")[-1]
         if "i" in lastComponent:
             # We need to switch to intraday scan
@@ -500,20 +527,22 @@
             if monitorOptions[1] != "0":
                 monitorOptions[1] = "0"
                 monitorOption = ":".join(monitorOptions)
             # We need to pipe the output from previous run into the next one
             if prevOutput is not None and not prevOutput.empty:
                 prevOutput_results = prevOutput[~prevOutput.index.duplicated(keep='first')]
                 prevOutput_results = prevOutput_results.index
+                hasFoundStocks = len(prevOutput_results) > 0
                 prevOutput_results = ",".join(prevOutput_results)
+                monitorOption = monitorOption.replace(":D:",":")
                 monitorOption = f"{monitorOption}:{prevOutput_results}"
         args.options = monitorOption.replace("::",":")
         args.options = args.options + ":D:;" + ":D:;".join(nextOnes[2:])
         args.options = args.options.replace("::",":")
-        return True
+        return True and hasFoundStocks
     return False
 
 def pkscreenercli():
     global originalStdOut
     if sys.platform.startswith("darwin"):
         try:
             multiprocessing.set_start_method("fork")
```

### Comparing `pkscreener-0.44.20240514.371/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240514.372/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240514.371
+Version: 0.44.20240514.372
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240514.371.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240514.372.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.370/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.370/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.370/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.371/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240514.371/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240514.372/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.371/setup.py` & `pkscreener-0.44.20240514.372/setup.py`

 * *Files identical despite different names*


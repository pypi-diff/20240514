# Comparing `tmp/cyclomonitor-2024.5.12.tar.gz` & `tmp/cyclomonitor-2024.5.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclomonitor-2024.5.12.tar", last modified: Sun May 12 22:10:55 2024, max compression
+gzip compressed data, was "cyclomonitor-2024.5.14.tar", last modified: Tue May 14 00:21:02 2024, max compression
```

## Comparing `cyclomonitor-2024.5.12.tar` & `cyclomonitor-2024.5.14.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-12 22:10:55.278104 cyclomonitor-2024.5.12/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    34523 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.12/LICENSE
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      263 2024-04-14 18:11:55.000000 cyclomonitor-2024.5.12/MANIFEST.in
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    43378 2024-05-12 22:10:55.278104 cyclomonitor-2024.5.12/PKG-INFO
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     2020 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.12/README.md
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      640 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.12/privacy-policy.md
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     1574 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.12/pyproject.toml
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)       15 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.12/requirements.txt
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)       38 2024-05-12 22:10:55.278104 cyclomonitor-2024.5.12/setup.cfg
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     1834 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.12/setup.py
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-12 22:10:55.270105 cyclomonitor-2024.5.12/src/
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-12 22:10:55.274104 cyclomonitor-2024.5.12/src/cyclomonitor/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      189 2024-04-15 00:43:27.000000 cyclomonitor-2024.5.12/src/cyclomonitor/__init__.py
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     4713 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.12/src/cyclomonitor/__main__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    10557 2024-04-14 12:51:51.000000 cyclomonitor-2024.5.12/src/cyclomonitor/atcf.py
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    10467 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.12/src/cyclomonitor/cli.py
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    35681 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.12/src/cyclomonitor/cyclomonitor.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1050 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.12/src/cyclomonitor/dir_calc.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      239 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.12/src/cyclomonitor/errors.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      801 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.12/src/cyclomonitor/global_vars.py
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-12 22:10:55.274104 cyclomonitor-2024.5.12/src/cyclomonitor/ibtracs/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    12661 2024-05-12 20:16:08.000000 cyclomonitor-2024.5.12/src/cyclomonitor/ibtracs/__init__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      185 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.12/src/cyclomonitor/ibtracs/__main__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5062 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.12/src/cyclomonitor/ibtracs/ibtracs_ALL.sql
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5070 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.12/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-12 22:10:55.274104 cyclomonitor-2024.5.12/src/cyclomonitor/ibtracs/locales/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.12/src/cyclomonitor/ibtracs/locales/C.json
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1945 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.12/src/cyclomonitor/ibtracs/locales/__init__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.12/src/cyclomonitor/ibtracs/locales/en_US.json
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-12 22:10:55.278104 cyclomonitor-2024.5.12/src/cyclomonitor/locales/
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    14006 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.12/src/cyclomonitor/locales/C.json
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     7742 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.12/src/cyclomonitor/locales/__init__.py
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    14006 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.12/src/cyclomonitor/locales/en_US.json
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1794 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.12/src/cyclomonitor/server_vars.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1192 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.12/src/cyclomonitor/uptime.py
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-12 22:10:55.278104 cyclomonitor-2024.5.12/src/cyclomonitor.egg-info/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      767 2024-05-12 22:10:55.000000 cyclomonitor-2024.5.12/src/cyclomonitor.egg-info/SOURCES.txt
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-14 00:21:02.307294 cyclomonitor-2024.5.14/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    34523 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.14/LICENSE
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      263 2024-04-14 18:11:55.000000 cyclomonitor-2024.5.14/MANIFEST.in
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    43427 2024-05-14 00:21:02.307294 cyclomonitor-2024.5.14/PKG-INFO
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     2069 2024-05-13 03:01:31.000000 cyclomonitor-2024.5.14/README.md
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      640 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.14/privacy-policy.md
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     1574 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.14/pyproject.toml
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)       15 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.14/requirements.txt
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)       38 2024-05-14 00:21:02.311294 cyclomonitor-2024.5.14/setup.cfg
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     1834 2024-05-14 00:11:33.000000 cyclomonitor-2024.5.14/setup.py
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-14 00:21:02.299294 cyclomonitor-2024.5.14/src/
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-14 00:21:02.303294 cyclomonitor-2024.5.14/src/cyclomonitor/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      189 2024-04-15 00:43:27.000000 cyclomonitor-2024.5.14/src/cyclomonitor/__init__.py
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     4713 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.14/src/cyclomonitor/__main__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    10835 2024-05-13 02:20:38.000000 cyclomonitor-2024.5.14/src/cyclomonitor/atcf.py
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    12462 2024-05-13 23:49:46.000000 cyclomonitor-2024.5.14/src/cyclomonitor/cli.py
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    35681 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.14/src/cyclomonitor/cyclomonitor.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1050 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.14/src/cyclomonitor/dir_calc.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      239 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.14/src/cyclomonitor/errors.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      801 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.14/src/cyclomonitor/global_vars.py
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-14 00:21:02.303294 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    13524 2024-05-13 23:52:17.000000 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/__init__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      185 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/__main__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5008 2024-05-13 23:49:26.000000 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/ibtracs_ALL.sql
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5012 2024-05-13 23:49:25.000000 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-14 00:21:02.307294 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/locales/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/locales/C.json
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1945 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/locales/__init__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/locales/en_US.json
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-14 00:21:02.307294 cyclomonitor-2024.5.14/src/cyclomonitor/locales/
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    14230 2024-05-13 22:53:22.000000 cyclomonitor-2024.5.14/src/cyclomonitor/locales/C.json
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     7862 2024-05-13 22:50:42.000000 cyclomonitor-2024.5.14/src/cyclomonitor/locales/__init__.py
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    14230 2024-05-13 22:53:22.000000 cyclomonitor-2024.5.14/src/cyclomonitor/locales/en_US.json
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1794 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.14/src/cyclomonitor/server_vars.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1192 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.14/src/cyclomonitor/uptime.py
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-14 00:21:02.307294 cyclomonitor-2024.5.14/src/cyclomonitor.egg-info/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      767 2024-05-14 00:21:02.000000 cyclomonitor-2024.5.14/src/cyclomonitor.egg-info/SOURCES.txt
```

### Comparing `cyclomonitor-2024.5.12/LICENSE` & `cyclomonitor-2024.5.14/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.12/PKG-INFO` & `cyclomonitor-2024.5.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclomonitor
-Version: 2024.5.12
+Version: 2024.5.14
 Summary: Discord bot that helps you keep tabs on tropical cyclones.
 Home-page: https://github.com/ntvmb/cyclomonitor
 Author: Nathaniel Greenwell
 Author-email: Nathaniel Greenwell <nategreenwell@live.com>
 Maintainer-email: Nathaniel Greenwell <nategreenwell@live.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
@@ -705,15 +705,16 @@
 
 ## Running interactively
 Install the package:
 ```
 pip install cyclomonitor
 ```
 Start an interactive session:
-`python3 -m cyclomonitor -i` or `python3 -m cyclomonitor.cli`
+`python3 -m cyclomonitor -i` or `python3 -m cyclomonitor.cli`  
+When running interactively, type `help` to see available commands.
 
 ## Running the bot
 Install the package with everything needed to run the bot:
 ```
 pip install cyclomonitor[bot]
 ```
 If you cloned the GitHub repository, you might want to install the package in dev mode:
@@ -739,11 +740,8 @@
 
 If you're using a virtual environment, ensure it is active before running the bot.  
 CycloMonitor logs to stdout by default. To log to a file, specify the parameter `-l LOGFILE`, where `LOGFILE` is the path to the log file.
 
 ## Configuring the bot 
 See CONFIGURATION.md for details.
 
-## CLI
-Coming soon
-
 Supports Python 3.8+, but Python 3.11+ is recommended.
```

### Comparing `cyclomonitor-2024.5.12/README.md` & `cyclomonitor-2024.5.14/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 ## Running interactively
 Install the package:
 ```
 pip install cyclomonitor
 ```
 Start an interactive session:
-`python3 -m cyclomonitor -i` or `python3 -m cyclomonitor.cli`
+`python3 -m cyclomonitor -i` or `python3 -m cyclomonitor.cli`  
+When running interactively, type `help` to see available commands.
 
 ## Running the bot
 Install the package with everything needed to run the bot:
 ```
 pip install cyclomonitor[bot]
 ```
 If you cloned the GitHub repository, you might want to install the package in dev mode:
@@ -44,11 +45,8 @@
 
 If you're using a virtual environment, ensure it is active before running the bot.  
 CycloMonitor logs to stdout by default. To log to a file, specify the parameter `-l LOGFILE`, where `LOGFILE` is the path to the log file.
 
 ## Configuring the bot 
 See CONFIGURATION.md for details.
 
-## CLI
-Coming soon
-
 Supports Python 3.8+, but Python 3.11+ is recommended.
```

### Comparing `cyclomonitor-2024.5.12/privacy-policy.md` & `cyclomonitor-2024.5.14/privacy-policy.md`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.12/pyproject.toml` & `cyclomonitor-2024.5.14/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.12/setup.py` & `cyclomonitor-2024.5.14/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import pathlib
 
-__version__ = "2024.5.12"
+__version__ = "2024.5.14"
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
```

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor/__main__.py` & `cyclomonitor-2024.5.14/src/cyclomonitor/__main__.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor/atcf.py` & `cyclomonitor-2024.5.14/src/cyclomonitor/atcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,14 +274,22 @@
             parse_storm(d["atcf_sector_file"])
             parse_storm(d["interp_sector_file"], mode="interp")
         except WrongData:
             continue
 
 
 async def get_forecast(*, name="", cid=""):
+    """Download the official forecast image for an active TC.
+    Returns the extension of the downloaded image file.
+
+    Keyword arguments:
+    name -- Search by name
+    cid -- Search by identifier
+    You must specify either name or cid. name has priority over cid.
+    """
     if not (cyclones and names):
         raise NoActiveStorms()
     if not (name or cid):
         raise ValueError(ERROR_GET_FORECAST_NO_PARAMS)
     if name:
         name = name.upper()
         try:
```

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor/cli.py` & `cyclomonitor-2024.5.14/src/cyclomonitor/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """CycloMonitor CLI"""
 
 import asyncio
 import datetime
-from sys import exit
+import re
+from sys import exit, version_info
 from .atcf import *
 from . import errors
 from .ibtracs import *
+from . import locales
 from .dir_calc import get_dir
 from .locales import *
 from io import StringIO
+from os import chdir  # for your convenience
 from typing import Callable, Awaitable, Generator
 
 COPYRIGHT_NOTICE = """\
 CycloMonitor - ATCF and IBTrACS wrapper for Discord
 Copyright (c) 2023 Virtual Nate
 
 This program is free software: you can redistribute it and/or modify it under
@@ -26,21 +29,36 @@
 
 For those hosting a copy of this bot, you should have received a copy of the
 GNU Affero General Public License along with this program. If not, see
 <https://www.gnu.org/licenses/>."""
 KT_TO_MPH = 1.15077945
 KT_TO_KMH = 1.852
 # fmt: off
-# Callable attributes that probably shouldn't be called from the CLI
-PRIVATE_ATTRS = [
+# Attributes that probably shouldn't be accessed from the CLI
+PRIVATE_ATTRS = {
     "zip_longest", "ATCFError", "WrongData", "NoActiveStorms", "main",
     "dataclass", "Iterable", "Storm", "Query", "query_group", "varchar",
     "numeric", "bit", "StringIO", "Callable", "Awaitable", "Generator",
-    "Internal",
-]
+    "Internal", "PRIVATE_ATTRS", "log", "asyncio", "datetime", "logging",
+    "aiohttp", "json", "sqlite3", "subprocess", "io", "re", "version_info",
+    "Literal", "Tuple",
+}
+PRIVATE_ATTRS.update(
+    attr for attr in dir() if not isinstance(globals()[attr], Callable)
+)
+PRIVATE_ATTRS.remove("KT_TO_MPH")
+PRIVATE_ATTRS.remove("KT_TO_KMH")
+CONSTANTS = {
+    "CONSTANTS", "PRIVATE_ATTRS", "COPYRIGHT_NOTICE", "KT_TO_MPH", "KT_TO_KMH",
+    "cyclones", "names", "timestamps", "lats", "longs", "basins", "winds",
+    "pressures", "tc_classes", "lats_real", "longs_real", "movement_speeds",
+    "movement_dirs", "None", "True", "False",
+}
+log = logging.getLogger(__name__)
+cd = chdir
 # fmt: on
 
 
 class Internal:
     """
     Methods internal to the CLI.
     All methods in this class (except for __repr__) are static.
@@ -63,27 +81,33 @@
         for arg in args[1:]:
             if "=" in arg:
                 to_delete.append(arg)
         for arg in to_delete:
             args.remove(arg)
 
         for index, arg in enumerate(args):
+            if arg.startswith("$"):
+                args[index] = globals().get(arg[1:], "")
+
             if index == 0:
                 continue
             if "." in arg:
                 try:
                     args[index] = float(arg)
                 except ValueError:
                     pass
             else:
                 try:
                     args[index] = int(arg)
                 except ValueError:
                     pass
         for k, v in kwargs.items():
+            if v.startswith("$"):
+                kwargs[k] = globals().get(v[1:], "")
+
             if "." in v:
                 try:
                     kwargs[k] = float(v)
                 except ValueError:
                     pass
             else:
                 try:
@@ -188,31 +212,37 @@
             else:
                 tc_class = CLASS_CY
         return tc_class
 
 
 def echo(*args):
     """Print a string to the screen."""
-    out = StringIO()
-    for arg in args:
-        out.write(f"{arg} ")
-    return out.getvalue()
+    return " ".join(args)
 
 
 def copyright(*args):
     """Get the copyright notice."""
     return COPYRIGHT_NOTICE
 
 
 def commands(*args):
     """Get the list of commands usable in the CLI."""
     return (
         key
         for key, value in globals().items()
-        if isinstance(value, (Callable, Awaitable)) and key not in PRIVATE_ATTRS
+        if isinstance(value, Callable) and key not in PRIVATE_ATTRS
+    )
+
+
+def attrs(*args):
+    """Get the list of variables. Includes constants."""
+    return (
+        key
+        for key, value in globals().items()
+        if not (isinstance(value, Callable) or key in PRIVATE_ATTRS)
     )
 
 
 def help(command_name="", *args):
     """Stop it. Get some help."""
     if command_name:
         try:
@@ -228,14 +258,43 @@
                 return CLI_SYMBOL_NOT_FOUND.format(command_name)
         except (AttributeError, KeyError):
             return CLI_SYMBOL_NOT_FOUND.format(command_name)
     else:
         return CLI_HELP
 
 
+def set_var(var_name: str, value, *args):
+    """Create var_name if it doesn't exist and set it to value.
+
+    Paramaters:
+    var_name - The name of the variable
+    value - The value to set this variable to
+
+    Precondition: var_name does not refer to a constant, command, or private
+    attribute.
+    """
+    if var_name in CONSTANTS:
+        return CLI_IS_A_CONSTANT
+    elif var_name in PRIVATE_ATTRS or isinstance(globals().get(var_name), Callable):
+        return CLI_ILLEGAL_NAME
+
+    if args:
+        value += f" {' '.join(args)}"
+
+    globals()[var_name] = value
+    return value
+
+
+def active_storms(*args):
+    """Get the list of active storms.
+    Format is ID NAME.
+    """
+    return (f"{id} {name}" for id, name in zip(cyclones, names))
+
+
 def present(name_or_id: str):
     """Present a TC in the ATCF data.
 
     Parameters:
     name_or_id - The TC name or identifier.
     """
     if not (cyclones and names):
@@ -294,14 +353,18 @@
         movement_str,
     )
 
 
 def cli():
     """The main function of the CLI."""
     print(CLI_STARTUP)
+    if version_info.major == 3 and version_info.minor < 11:
+        log.warning(
+            CLI_OLD_PY_VERSION.format(f"{version_info.major}.{version_info.minor}")
+        )
     while True:
         try:
             request = input("cyclomonitor> ")
         except EOFError:
             print("\n", end="")
             break
         except KeyboardInterrupt:
```

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor/cyclomonitor.py` & `cyclomonitor-2024.5.14/src/cyclomonitor/cyclomonitor.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor/dir_calc.py` & `cyclomonitor-2024.5.14/src/cyclomonitor/dir_calc.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor/global_vars.py` & `cyclomonitor-2024.5.14/src/cyclomonitor/global_vars.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor/ibtracs/__init__.py` & `cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,22 @@
 Functions:
 update_db -- update database
 init_db -- initialize database
 get_storm -- find TCs
 :copyright: (c) 2024 by Nathaniel Greenwell.
 """
 
-from __future__ import annotations
-
 import sqlite3
 import aiohttp
 import logging
 import os
 import subprocess
 import io
 from dataclasses import dataclass
-from collections.abc import Iterable
+from typing import Iterable, Literal, Tuple
 from .locales import *
 
 log = logging.getLogger(__name__)
 PATH = os.path.dirname(os.path.realpath(__file__))
 DB = f"{PATH}/BestTrack.db"
 BASE_URI = "https://www.ncei.noaa.gov/data/international-best-track-archive-for-climate-stewardship-ibtracs/v04r00/access/csv"
 if not os.path.exists(DB):
@@ -135,15 +133,15 @@
     basin: str
     name: str
 
     def __repr__(self):
         return QUERY_REPR.format(self=self)
 
 
-def query_group(queries: Iterable[tuple[str, int, str, str]]):
+def query_group(queries: Iterable[Tuple[str, int, str, str]]):
     """Yield Query objects.
 
     Arguments:
     queries -- an iterable consisting of tuples that have length 4
     """
     for sid, season, basin, name in queries:
         yield Query(sid, season, basin, name)
@@ -166,14 +164,45 @@
     else:
         os.unlink(csv)
     finally:
         # free up RAM
         del data, lines
 
 
+def _csv_import(table: Literal["LastThreeYears", "AllBestTrack"]):
+    """(Internal) Import CSV into table."""
+    with sqlite3.connect(DB) as con:
+        cur = con.cursor()
+        if table == "LastThreeYears":
+            cur.executescript(open(f"{PATH}/ibtracs_LAST3.sql").read())
+            filename = "ibtracs_last3_NO_HEADING.csv"
+        else:
+            cur.executescript(open(f"{PATH}/ibtracs_ALL.sql").read())
+            filename = "ibtracs_all_NO_HEADING.csv"
+
+        with open(f"{PATH}/{filename}") as data:
+            for line in data:
+                values = line.split(",")
+                for i, v in enumerate(values):
+                    if "." in v:
+                        try:
+                            values[i] = float(v)
+                        except ValueError:
+                            pass
+                    else:
+                        try:
+                            values[i] = int(v)
+                        except ValueError:
+                            pass
+                cur.execute(
+                    f"INSERT INTO {table} VALUES({'?, ' * (len(values) - 1)}?)", values
+                )
+        con.commit()
+
+
 async def update_db(mode="last3"):
     """Update the best track database.
 
     Arguments:
     mode -- Table(s) to update (default "last3")
     mode can be one of "last3", "all", or "full".
     If mode == "last3", update the table LastThreeYears.
@@ -206,20 +235,15 @@
                 raise
             finally:
                 # Calling close does not delete the object.
                 # We want to delete the resource afterwards to save RAM
                 # because we may be working with a large amount of data.
                 del r
         _remove_headers(f"{PATH}/{csv}")
-        subprocess.run(
-            ["sqlite3", DB],
-            input=f".cd {PATH}\n.read ibtracs_LAST3.sql",
-            encoding="UTF-8",
-            check=True,
-        )
+        _csv_import("LastThreeYears")
         os.unlink(f"{PATH}/ibtracs_last3_NO_HEADING.csv")
     if get_all:
         csv = "ibtracs_all.csv"
         async with aiohttp.ClientSession(
             timeout=aiohttp.ClientTimeout(connect=10), raise_for_status=True
         ) as session:
             try:
@@ -231,20 +255,15 @@
                 raise
             finally:
                 # Calling close does not delete the object.
                 # We want to delete the resource afterwards to save RAM
                 # because we may be working with a large amount of data.
                 del r
         _remove_headers(f"{PATH}/{csv}")
-        subprocess.run(
-            ["sqlite3", DB],
-            input=f".cd {PATH}\n.read ibtracs_ALL.sql",
-            encoding="UTF-8",
-            check=True,
-        )
+        _csv_import("AllBestTrack")
         os.unlink(f"{PATH}/ibtracs_all_NO_HEADING.csv")
     log.info(IBTRACS_UPDATE_SUCCESS)
 
 
 async def init_db():
     """Equivalent to :func:`update_db("full")`"""
     await update_db("full")
```

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor/ibtracs/ibtracs_ALL.sql` & `cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-DROP TABLE IF EXISTS AllBestTrack;
-CREATE TABLE AllBestTrack(
+DROP TABLE IF EXISTS LastThreeYears;
+CREATE TABLE LastThreeYears(
    SID              VARCHAR(13) NOT NULL
   ,SEASON           INTEGER  NOT NULL
   ,NUMBER           INTEGER  NOT NULL
   ,BASIN            VARCHAR(2) NOT NULL
   ,SUBBASIN         VARCHAR(2) NOT NULL
   ,NAME             VARCHAR(16) NOT NULL
   ,ISO_TIME         VARCHAR(19) NOT NULL
@@ -160,8 +160,7 @@
   ,USA_SEARAD_NE    INTEGER
   ,USA_SEARAD_SE    INTEGER
   ,USA_SEARAD_SW    INTEGER
   ,USA_SEARAD_NW    INTEGER
   ,STORM_SPEED      INTEGER
   ,STORM_DIR        INTEGER
 );
-.import ibtracs_all_NO_HEADING.csv AllBestTrack --csv
```

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql` & `cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/ibtracs_ALL.sql`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-DROP TABLE IF EXISTS LastThreeYears;
-CREATE TABLE LastThreeYears(
+DROP TABLE IF EXISTS AllBestTrack;
+CREATE TABLE AllBestTrack(
    SID              VARCHAR(13) NOT NULL
   ,SEASON           INTEGER  NOT NULL
   ,NUMBER           INTEGER  NOT NULL
   ,BASIN            VARCHAR(2) NOT NULL
   ,SUBBASIN         VARCHAR(2) NOT NULL
   ,NAME             VARCHAR(16) NOT NULL
   ,ISO_TIME         VARCHAR(19) NOT NULL
@@ -160,8 +160,7 @@
   ,USA_SEARAD_NE    INTEGER
   ,USA_SEARAD_SE    INTEGER
   ,USA_SEARAD_SW    INTEGER
   ,USA_SEARAD_NW    INTEGER
   ,STORM_SPEED      INTEGER
   ,STORM_DIR        INTEGER
 );
-.import ibtracs_last3_NO_HEADING.csv LastThreeYears --csv
```

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor/ibtracs/locales/C.json` & `cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/locales/C.json`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor/ibtracs/locales/__init__.py` & `cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/locales/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor/ibtracs/locales/en_US.json` & `cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/locales/en_US.json`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor/locales/C.json` & `cyclomonitor-2024.5.14/src/cyclomonitor/locales/C.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9806629834254144%*

 * *Differences: {"'CLI_HELP'": "'CycloMonitor CLI help\\n\\nFor a list of commands, type `commands`. Type `help "*

 * *               'command` for help on\\ncommand. Note: CLI is in early development; expect missing '*

 * *               'or broken features.\\n\\nGeneral usage:\\nYou can execute commands and get the '*

 * *               'values of variables.\\nExample command usage:\\ncyclomonitor> echo hello '*

 * *               'world!\\nExample attribute access:\\ncyclomonitor> KT_TO_MPH\\n\\nArguments are '*

 * *               'separated by […]*

```diff
@@ -15,18 +15,21 @@
     "CLASS_RL": "REMNANTS OF",
     "CLASS_SD": "SUBTROPICAL DEPRESSION",
     "CLASS_SS": "SUBTROPICAL STORM",
     "CLASS_STY": "SUPER TYPHOON",
     "CLASS_TD": "TROPICAL DEPRESSION",
     "CLASS_TS": "TROPICAL STORM",
     "CLASS_TY": "TYPHOON",
-    "CLI_HELP": "CycloMonitor CLI help\n\nFor a list of commands, type `commands`. Type `help command` for help on\ncommand. Note: CLI is in early development; expect missing or broken features.\n\nGeneral usage:\nYou can execute commands and get the values of constants (creating variables\ncurrently isn't supported).\nExample command usage:\ncyclomonitor> echo hello world!\nExample attribute access:\ncyclomonitor> KT_TO_MPH\n(Currently, variables can't be used as command arguments, as the parser will\ntreat it as a string.)\n\nArguments are separated by spaces. Keyword arguments can be defined using\n`arg=value`. Example keyword argument usage:\ncyclomonitor> get_storm name=Patricia season=2015",
+    "CLI_HELP": "CycloMonitor CLI help\n\nFor a list of commands, type `commands`. Type `help command` for help on\ncommand. Note: CLI is in early development; expect missing or broken features.\n\nGeneral usage:\nYou can execute commands and get the values of variables.\nExample command usage:\ncyclomonitor> echo hello world!\nExample attribute access:\ncyclomonitor> KT_TO_MPH\n\nArguments are separated by spaces. Keyword arguments can be defined using\n`arg=value`. Example keyword argument usage:\ncyclomonitor> get_storm name=Patricia season=2015\n\nTo create or change a variable, use the `set_var` command. Argument values\nthat start with `$` will be treated as a variable name.",
+    "CLI_ILLEGAL_NAME": "Illegal variable name!",
     "CLI_INTERNAL_ERROR": "An internal error occurred.",
+    "CLI_IS_A_CONSTANT": "Cannot edit the value of a constant!",
     "CLI_IS_A_VAR": "{0} is a variable.",
     "CLI_MISSING_DOCSTRING": "Missing docstring",
+    "CLI_OLD_PY_VERSION": "Detected Python {0}! Python 3.11+ is recommended as some commands can break on older versions!",
     "CLI_PARSER_REPR": "Internal parser",
     "CLI_STARTUP": "CycloMonitor CLI\nThis program is free software. For details type `copyright`.\n\nThis program comes with ABSOLUTELY NO WARRANTY, to the extent\npermitted by applicable law.",
     "CLI_STORM_NOT_FOUND": "Cannot find a TC with name or ID {0}.",
     "CLI_SYMBOL_NOT_FOUND": "Can't recognize {0} as a command or variable.",
     "CM_ANNOUNCE_ALL": "Make an announcement to all servers",
     "CM_ANNOUNCE_ALL_SUCCESS": "Announced to all servers:\n{0}",
     "CM_ANNOUNCE_BASIN": "Make an announcement regarding a specific basin",
```

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor/locales/__init__.py` & `cyclomonitor-2024.5.14/src/cyclomonitor/locales/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,17 @@
 CLI_SYMBOL_NOT_FOUND = "CLI_SYMBOL_NOT_FOUND"
 CLI_INTERNAL_ERROR = "CLI_INTERNAL_ERROR"
 CLI_PARSER_REPR = "CLI_PARSER_REPR"
 CLI_HELP = "CLI_HELP"
 CLI_MISSING_DOCSTRING = "CLI_MISSING_DOCSTRING"
 CLI_IS_A_VAR = "CLI_IS_A_VAR"
 CLI_STORM_NOT_FOUND = "CLI_STORM_NOT_FOUND"
+CLI_IS_A_CONSTANT = "CLI_IS_A_CONSTANT"
+CLI_ILLEGAL_NAME = "CLI_ILLEGAL_NAME"
+CLI_OLD_PY_VERSION = "CLI_OLD_PY_VERSION"
 
 _log = _logging.getLogger(__name__)
 locale.setlocale(locale.LC_ALL, "")
 _PATH = os.path.dirname(os.path.realpath(__file__))
 
 
 def set_locale(lang="C"):
```

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor/locales/en_US.json` & `cyclomonitor-2024.5.14/src/cyclomonitor/locales/en_US.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9806629834254144%*

 * *Differences: {"'CLI_HELP'": "'CycloMonitor CLI help\\n\\nFor a list of commands, type `commands`. Type `help "*

 * *               'command` for help on\\ncommand. Note: CLI is in early development; expect missing '*

 * *               'or broken features.\\n\\nGeneral usage:\\nYou can execute commands and get the '*

 * *               'values of variables.\\nExample command usage:\\ncyclomonitor> echo hello '*

 * *               'world!\\nExample attribute access:\\ncyclomonitor> KT_TO_MPH\\n\\nArguments are '*

 * *               'separated by […]*

```diff
@@ -15,18 +15,21 @@
     "CLASS_RL": "REMNANTS OF",
     "CLASS_SD": "SUBTROPICAL DEPRESSION",
     "CLASS_SS": "SUBTROPICAL STORM",
     "CLASS_STY": "SUPER TYPHOON",
     "CLASS_TD": "TROPICAL DEPRESSION",
     "CLASS_TS": "TROPICAL STORM",
     "CLASS_TY": "TYPHOON",
-    "CLI_HELP": "CycloMonitor CLI help\n\nFor a list of commands, type `commands`. Type `help command` for help on\ncommand. Note: CLI is in early development; expect missing or broken features.\n\nGeneral usage:\nYou can execute commands and get the values of constants (creating variables\ncurrently isn't supported).\nExample command usage:\ncyclomonitor> echo hello world!\nExample attribute access:\ncyclomonitor> KT_TO_MPH\n(Currently, variables can't be used as command arguments, as the parser will\ntreat it as a string.)\n\nArguments are separated by spaces. Keyword arguments can be defined using\n`arg=value`. Example keyword argument usage:\ncyclomonitor> get_storm name=Patricia season=2015",
+    "CLI_HELP": "CycloMonitor CLI help\n\nFor a list of commands, type `commands`. Type `help command` for help on\ncommand. Note: CLI is in early development; expect missing or broken features.\n\nGeneral usage:\nYou can execute commands and get the values of variables.\nExample command usage:\ncyclomonitor> echo hello world!\nExample attribute access:\ncyclomonitor> KT_TO_MPH\n\nArguments are separated by spaces. Keyword arguments can be defined using\n`arg=value`. Example keyword argument usage:\ncyclomonitor> get_storm name=Patricia season=2015\n\nTo create or change a variable, use the `set_var` command. Argument values\nthat start with `$` will be treated as a variable name.",
+    "CLI_ILLEGAL_NAME": "Illegal variable name!",
     "CLI_INTERNAL_ERROR": "An internal error occurred.",
+    "CLI_IS_A_CONSTANT": "Cannot edit the value of a constant!",
     "CLI_IS_A_VAR": "{0} is a variable.",
     "CLI_MISSING_DOCSTRING": "Missing docstring",
+    "CLI_OLD_PY_VERSION": "Detected Python {0}! Python 3.11+ is recommended as some commands can break on older versions!",
     "CLI_PARSER_REPR": "Internal parser",
     "CLI_STARTUP": "CycloMonitor CLI\nThis program is free software. For details type `copyright`.\n\nThis program comes with ABSOLUTELY NO WARRANTY, to the extent\npermitted by applicable law.",
     "CLI_STORM_NOT_FOUND": "Cannot find a TC with name or ID {0}.",
     "CLI_SYMBOL_NOT_FOUND": "Can't recognize {0} as a command or variable.",
     "CM_ANNOUNCE_ALL": "Make an announcement to all servers",
     "CM_ANNOUNCE_ALL_SUCCESS": "Announced to all servers:\n{0}",
     "CM_ANNOUNCE_BASIN": "Make an announcement regarding a specific basin",
```

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor/server_vars.py` & `cyclomonitor-2024.5.14/src/cyclomonitor/server_vars.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor/uptime.py` & `cyclomonitor-2024.5.14/src/cyclomonitor/uptime.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.12/src/cyclomonitor.egg-info/SOURCES.txt` & `cyclomonitor-2024.5.14/src/cyclomonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*


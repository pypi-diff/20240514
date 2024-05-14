# Comparing `tmp/freva_client-2404.0.0.tar.gz` & `tmp/freva_client-2404.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freva_client-2404.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "freva_client-2404.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `freva_client-2404.0.0.tar` & `freva_client-2404.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       57 2024-05-14 16:00:57.126989 freva_client-2404.0.0/MANIFEST.in
--rw-r--r--   0        0        0     1263 2024-05-14 16:00:57.126989 freva_client-2404.0.0/README.md
--rw-r--r--   0        0        0      736 2024-05-14 16:00:57.126989 freva_client-2404.0.0/assets/share/freva/freva.toml
--rw-r--r--   0        0        0     1441 2024-05-14 16:00:57.126989 freva_client-2404.0.0/pyproject.toml
--rw-r--r--   0        0        0      804 2024-05-14 16:00:57.126989 freva_client-2404.0.0/src/freva_client/__init__.py
--rw-r--r--   0        0        0      149 2024-05-14 16:00:57.126989 freva_client-2404.0.0/src/freva_client/__main__.py
--rw-r--r--   0        0        0      149 2024-05-14 16:00:57.126989 freva_client-2404.0.0/src/freva_client/cli/__init__.py
--rw-r--r--   0        0        0      504 2024-05-14 16:00:57.130989 freva_client-2404.0.0/src/freva_client/cli/cli_app.py
--rw-r--r--   0        0        0     5471 2024-05-14 16:00:57.130989 freva_client-2404.0.0/src/freva_client/cli/cli_utils.py
--rw-r--r--   0        0        0    15365 2024-05-14 16:00:57.130989 freva_client-2404.0.0/src/freva_client/cli/databrowser_cli.py
--rw-r--r--   0        0        0        0 2024-05-14 16:00:57.130989 freva_client-2404.0.0/src/freva_client/py.typed
--rw-r--r--   0        0        0    23388 2024-05-14 16:00:57.130989 freva_client-2404.0.0/src/freva_client/query.py
--rw-r--r--   0        0        0      999 2024-05-14 16:00:57.130989 freva_client-2404.0.0/src/freva_client/utils/__init__.py
--rw-r--r--   0        0        0     5884 2024-05-14 16:00:57.130989 freva_client-2404.0.0/src/freva_client/utils/databrowser_utils.py
--rw-r--r--   0        0        0     2462 2024-05-14 16:00:57.130989 freva_client-2404.0.0/src/freva_client/utils/logger.py
--rw-r--r--   0        0        0        0 2024-05-14 16:00:57.130989 freva_client-2404.0.0/src/tests/__init__.py
--rw-r--r--   0        0        0     3029 2024-05-14 16:00:57.130989 freva_client-2404.0.0/src/tests/conftest.py
--rw-r--r--   0        0        0     4369 2024-05-14 16:00:57.130989 freva_client-2404.0.0/src/tests/test_cli.py
--rw-r--r--   0        0        0     3796 2024-05-14 16:00:57.130989 freva_client-2404.0.0/src/tests/test_databrowser.py
--rw-r--r--   0        0        0     2348 2024-05-14 16:00:57.130989 freva_client-2404.0.0/src/tests/test_url.py
--rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 freva_client-2404.0.0/PKG-INFO
+-rw-r--r--   0        0        0       57 2024-05-14 16:19:26.269485 freva_client-2404.0.1/MANIFEST.in
+-rw-r--r--   0        0        0     1254 2024-05-14 16:19:26.269485 freva_client-2404.0.1/README.md
+-rw-r--r--   0        0        0      736 2024-05-14 16:19:26.269485 freva_client-2404.0.1/assets/share/freva/freva.toml
+-rw-r--r--   0        0        0     1441 2024-05-14 16:19:26.269485 freva_client-2404.0.1/pyproject.toml
+-rw-r--r--   0        0        0      804 2024-05-14 16:19:26.269485 freva_client-2404.0.1/src/freva_client/__init__.py
+-rw-r--r--   0        0        0      149 2024-05-14 16:19:26.269485 freva_client-2404.0.1/src/freva_client/__main__.py
+-rw-r--r--   0        0        0      149 2024-05-14 16:19:26.269485 freva_client-2404.0.1/src/freva_client/cli/__init__.py
+-rw-r--r--   0        0        0      504 2024-05-14 16:19:26.273485 freva_client-2404.0.1/src/freva_client/cli/cli_app.py
+-rw-r--r--   0        0        0     5471 2024-05-14 16:19:26.273485 freva_client-2404.0.1/src/freva_client/cli/cli_utils.py
+-rw-r--r--   0        0        0    15365 2024-05-14 16:19:26.273485 freva_client-2404.0.1/src/freva_client/cli/databrowser_cli.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:19:26.273485 freva_client-2404.0.1/src/freva_client/py.typed
+-rw-r--r--   0        0        0    23388 2024-05-14 16:19:26.273485 freva_client-2404.0.1/src/freva_client/query.py
+-rw-r--r--   0        0        0      999 2024-05-14 16:19:26.273485 freva_client-2404.0.1/src/freva_client/utils/__init__.py
+-rw-r--r--   0        0        0     5884 2024-05-14 16:19:26.273485 freva_client-2404.0.1/src/freva_client/utils/databrowser_utils.py
+-rw-r--r--   0        0        0     2462 2024-05-14 16:19:26.273485 freva_client-2404.0.1/src/freva_client/utils/logger.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:19:26.273485 freva_client-2404.0.1/src/tests/__init__.py
+-rw-r--r--   0        0        0     3029 2024-05-14 16:19:26.273485 freva_client-2404.0.1/src/tests/conftest.py
+-rw-r--r--   0        0        0     4369 2024-05-14 16:19:26.273485 freva_client-2404.0.1/src/tests/test_cli.py
+-rw-r--r--   0        0        0     3796 2024-05-14 16:19:26.273485 freva_client-2404.0.1/src/tests/test_databrowser.py
+-rw-r--r--   0        0        0     2348 2024-05-14 16:19:26.273485 freva_client-2404.0.1/src/tests/test_url.py
+-rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 freva_client-2404.0.1/PKG-INFO
```

### Comparing `freva_client-2404.0.0/README.md` & `freva_client-2404.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # A REST API for the freva databrowser
 
 [![License](https://img.shields.io/badge/License-BSD-purple.svg)](LICENSE)
-[![Python](https://img.shields.io/badge/python-3.12-red.svg)](https://www.python.org/downloads/release/python-312/)
+[![PyPI](https://img.shields.io/pypi/pyversions/freva-client.svg)](https://pypi.org/project/freva-client/)
 [![Docs](https://img.shields.io/badge/API-Doc-green.svg)](https://freva-clint.github.io/freva-nextgen)
 [![Tests](https://github.com/FREVA-CLINT/freva-nextgen/actions/workflows/ci_job.yml/badge.svg)](https://github.com/FREVA-CLINT/freva-nextgen/actions)
 [![Test-Coverage](https://codecov.io/github/FREVA-CLINT/freva-nextgen/branch/init/graph/badge.svg?token=dGhXxh7uP3)](https://codecov.io/github/FREVA-CLINT/freva-nextgen)
 
 The freva-client library is a small library that makes connections to the freva
 server. The client library currently supports the following services:
```

### Comparing `freva_client-2404.0.0/assets/share/freva/freva.toml` & `freva_client-2404.0.1/assets/share/freva/freva.toml`

 * *Files identical despite different names*

### Comparing `freva_client-2404.0.0/pyproject.toml` & `freva_client-2404.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `freva_client-2404.0.0/src/freva_client/__init__.py` & `freva_client-2404.0.1/src/freva_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 The code described here is currently in testing phase. The client and server
 library described in the documentation only support searching for data. If you
 need to apply data analysis plugins, please visit the
 """
 
 from .query import databrowser
 
-__version__ = "2404.0.0"
+__version__ = "2404.0.1"
 __all__ = ["databrowser", "__version__"]
```

### Comparing `freva_client-2404.0.0/src/freva_client/cli/cli_utils.py` & `freva_client-2404.0.1/src/freva_client/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `freva_client-2404.0.0/src/freva_client/cli/databrowser_cli.py` & `freva_client-2404.0.1/src/freva_client/cli/databrowser_cli.py`

 * *Files identical despite different names*

### Comparing `freva_client-2404.0.0/src/freva_client/query.py` & `freva_client-2404.0.1/src/freva_client/query.py`

 * *Files identical despite different names*

### Comparing `freva_client-2404.0.0/src/freva_client/utils/__init__.py` & `freva_client-2404.0.1/src/freva_client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `freva_client-2404.0.0/src/freva_client/utils/databrowser_utils.py` & `freva_client-2404.0.1/src/freva_client/utils/databrowser_utils.py`

 * *Files identical despite different names*

### Comparing `freva_client-2404.0.0/src/freva_client/utils/logger.py` & `freva_client-2404.0.1/src/freva_client/utils/logger.py`

 * *Files identical despite different names*

### Comparing `freva_client-2404.0.0/src/tests/conftest.py` & `freva_client-2404.0.1/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `freva_client-2404.0.0/src/tests/test_cli.py` & `freva_client-2404.0.1/src/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `freva_client-2404.0.0/src/tests/test_databrowser.py` & `freva_client-2404.0.1/src/tests/test_databrowser.py`

 * *Files identical despite different names*

### Comparing `freva_client-2404.0.0/src/tests/test_url.py` & `freva_client-2404.0.1/src/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `freva_client-2404.0.0/PKG-INFO` & `freva_client-2404.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freva-client
-Version: 2404.0.0
+Version: 2404.0.1
 Summary: Search for climate data based on key-value pairs
 Author-email: "DKRZ, Clint" <freva@dkrz.de>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -27,15 +27,15 @@
 Project-URL: Issues, https://github.com/FREVA-CLINT/freva-nextgen/issues
 Project-URL: Source, https://github.com/FREVA-CLINT/freva-nextgen/
 Provides-Extra: dev
 
 # A REST API for the freva databrowser
 
 [![License](https://img.shields.io/badge/License-BSD-purple.svg)](LICENSE)
-[![Python](https://img.shields.io/badge/python-3.12-red.svg)](https://www.python.org/downloads/release/python-312/)
+[![PyPI](https://img.shields.io/pypi/pyversions/freva-client.svg)](https://pypi.org/project/freva-client/)
 [![Docs](https://img.shields.io/badge/API-Doc-green.svg)](https://freva-clint.github.io/freva-nextgen)
 [![Tests](https://github.com/FREVA-CLINT/freva-nextgen/actions/workflows/ci_job.yml/badge.svg)](https://github.com/FREVA-CLINT/freva-nextgen/actions)
 [![Test-Coverage](https://codecov.io/github/FREVA-CLINT/freva-nextgen/branch/init/graph/badge.svg?token=dGhXxh7uP3)](https://codecov.io/github/FREVA-CLINT/freva-nextgen)
 
 The freva-client library is a small library that makes connections to the freva
 server. The client library currently supports the following services:
```


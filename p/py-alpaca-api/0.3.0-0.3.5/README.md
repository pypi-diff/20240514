# Comparing `tmp/py_alpaca_api-0.3.0.tar.gz` & `tmp/py_alpaca_api-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_api-0.3.0.tar", max compression
+gzip compressed data, was "py_alpaca_api-0.3.5.tar", max compression
```

## Comparing `py_alpaca_api-0.3.0.tar` & `py_alpaca_api-0.3.5.tar`

### file list

```diff
@@ -1,7 +1,14 @@
--rw-r--r--   0        0        0     1066 2024-05-11 23:37:32.674625 py_alpaca_api-0.3.0/LICENSE
--rw-r--r--   0        0        0    12576 2024-05-12 02:52:40.341369 py_alpaca_api-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-05-11 00:31:44.448417 py_alpaca_api-0.3.0/py_alpaca_api/__init__.py
--rw-r--r--   0        0        0    45327 2024-05-13 23:08:08.097238 py_alpaca_api-0.3.0/py_alpaca_api/alpaca.py
--rw-r--r--   0        0        0    19356 2024-05-13 23:08:08.087238 py_alpaca_api-0.3.0/py_alpaca_api/src/data_classes.py
--rw-r--r--   0        0        0     1279 2024-05-13 23:09:15.937219 py_alpaca_api-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    13337 1970-01-01 00:00:00.000000 py_alpaca_api-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-11 23:37:32.674625 py_alpaca_api-0.3.5/LICENSE
+-rw-r--r--   0        0        0    12576 2024-05-12 02:52:40.341369 py_alpaca_api-0.3.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 00:31:44.448417 py_alpaca_api-0.3.5/py_alpaca_api/__init__.py
+-rw-r--r--   0        0        0     2143 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/alpaca.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/src/__init__.py
+-rw-r--r--   0        0        0     3292 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/src/account.py
+-rw-r--r--   0        0        0     1947 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/src/asset.py
+-rw-r--r--   0        0        0    19461 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/src/data_classes.py
+-rw-r--r--   0        0        0     6618 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/src/history.py
+-rw-r--r--   0        0        0     1046 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/src/market.py
+-rw-r--r--   0        0        0    17950 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/src/order.py
+-rw-r--r--   0        0        0    14431 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/src/position.py
+-rw-r--r--   0        0        0     1279 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0    13337 1970-01-01 00:00:00.000000 py_alpaca_api-0.3.5/PKG-INFO
```

### Comparing `py_alpaca_api-0.3.0/LICENSE` & `py_alpaca_api-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.3.0/README.md` & `py_alpaca_api-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.3.0/py_alpaca_api/src/data_classes.py` & `py_alpaca_api-0.3.5/py_alpaca_api/src/data_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,15 +291,15 @@
     intraday_adjustments: int
     pending_reg_taf_fees: float
 
 
 ############################################
 # Data Class Clock Conversion Functions
 ############################################
-def clock_class_from_dict(data_dict):
+def clock_class_from_dict(data_dict: dict) -> ClockClass:
     """Converts a dictionary to a ClockClass object.
 
     Parameters:
     -----------
     data_dict: dict
         A dictionary containing the clock data.
 
@@ -327,15 +327,15 @@
         ),
     )
 
 
 ############################################
 # Data Class Position Conversion Functions
 ############################################
-def position_class_from_dict(data_dict):
+def position_class_from_dict(data_dict: dict) -> PositionClass:
     """Converts a dictionary to a PositionClass object.
 
     Parameters:
     -----------
     data_dict: dict
         A dictionary containing the position data.
 
@@ -367,15 +367,15 @@
         asset_marginable=bool(data_dict["asset_marginable"]),
     )
 
 
 ############################################
 # Data Class Account Conversion Functions
 ############################################
-def account_class_from_dict(data_dict):
+def account_class_from_dict(data_dict: dict) -> AccountClass:
     """Converts a dictionary to an AccountClass object.
 
     Parameters:
     -----------
     data_dict: dict
         A dictionary containing the account data.
 
@@ -431,15 +431,15 @@
         pending_reg_taf_fees=float(data_dict["pending_reg_taf_fees"] if data_dict["pending_reg_taf_fees"] else 0),
     )
 
 
 ############################################
 # Data Class Asset Conversion Functions
 ############################################
-def asset_class_from_dict(data_dict):
+def asset_class_from_dict(data_dict: dict) -> AssetClass:
     """Converts a dictionary to an AssetClass object.
 
     Parameters:
     -----------
     data_dict: dict
         A dictionary containing the asset data.
 
@@ -463,15 +463,15 @@
         tradable=bool(data_dict["tradable"]),
     )
 
 
 ############################################
 # Data Class Order Conversion Functions
 ############################################
-def order_class_from_dict(data_dict):
+def order_class_from_dict(data_dict: dict) -> OrderClass:
     """Converts a dictionary to an OrderClass object.
 
     Parameters:
     -----------
     data_dict: dict
         A dictionary containing the order data.
```

### Comparing `py_alpaca_api-0.3.0/pyproject.toml` & `py_alpaca_api-0.3.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-api"
-version = "0.3.0"
+version = "0.3.5"
 description = "Python package, for communicating with Alpaca Markets REST API."
 authors = ["TexasCoding <jeff10278@me.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TexasCoding/py-alpaca-api"
 repository = "https://github.com/TexasCoding/py-alpaca-api"
 documentation = "https://py-alpaca-api.readthedocs.io/en/latest/"
```

### Comparing `py_alpaca_api-0.3.0/PKG-INFO` & `py_alpaca_api-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-alpaca-api
-Version: 0.3.0
+Version: 0.3.5
 Summary: Python package, for communicating with Alpaca Markets REST API.
 Home-page: https://github.com/TexasCoding/py-alpaca-api
 License: MIT
 Keywords: alpaca,python
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
```


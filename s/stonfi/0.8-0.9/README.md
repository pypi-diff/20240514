# Comparing `tmp/stonfi-0.8.tar.gz` & `tmp/stonfi-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stonfi-0.8.tar", last modified: Mon May 13 09:36:46 2024, max compression
+gzip compressed data, was "stonfi-0.9.tar", last modified: Tue May 14 08:56:16 2024, max compression
```

## Comparing `stonfi-0.8.tar` & `stonfi-0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:36:46.537564 stonfi-0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 09:36:39.000000 stonfi-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-13 09:36:46.537564 stonfi-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 09:36:39.000000 stonfi-0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-13 09:36:39.000000 stonfi-0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:36:46.537564 stonfi-0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:36:46.533564 stonfi-0.8/stonfi/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-13 09:36:39.000000 stonfi-0.8/stonfi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-13 09:36:39.000000 stonfi-0.8/stonfi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:36:46.533564 stonfi-0.8/stonfi/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-13 09:36:39.000000 stonfi-0.8/stonfi/contracts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:36:46.537564 stonfi-0.8/stonfi/contracts/dex/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 09:36:39.000000 stonfi-0.8/stonfi/contracts/dex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:36:46.537564 stonfi-0.8/stonfi/contracts/dex/v1/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-13 09:36:39.000000 stonfi-0.8/stonfi/contracts/dex/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 09:36:39.000000 stonfi-0.8/stonfi/contracts/dex/v1/lp_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-13 09:36:39.000000 stonfi-0.8/stonfi/contracts/dex/v1/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    13909 2024-05-13 09:36:39.000000 stonfi-0.8/stonfi/contracts/dex/v1/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:36:46.537564 stonfi-0.8/stonfi/contracts/farm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:36:39.000000 stonfi-0.8/stonfi/contracts/farm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:36:46.537564 stonfi-0.8/stonfi/contracts/jetton/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-13 09:36:39.000000 stonfi-0.8/stonfi/contracts/jetton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-13 09:36:39.000000 stonfi-0.8/stonfi/contracts/jetton/jetton_root.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-13 09:36:39.000000 stonfi-0.8/stonfi/contracts/jetton/jetton_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:36:46.537564 stonfi-0.8/stonfi/contracts/pTON/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-13 09:36:39.000000 stonfi-0.8/stonfi/contracts/pTON/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-13 09:36:39.000000 stonfi-0.8/stonfi/contracts/pTON/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:36:46.537564 stonfi-0.8/stonfi/http/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 09:36:39.000000 stonfi-0.8/stonfi/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-13 09:36:39.000000 stonfi-0.8/stonfi/http/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-13 09:36:39.000000 stonfi-0.8/stonfi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:36:46.537564 stonfi-0.8/stonfi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-13 09:36:46.000000 stonfi-0.8/stonfi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-13 09:36:46.000000 stonfi-0.8/stonfi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:36:46.000000 stonfi-0.8/stonfi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 09:36:46.000000 stonfi-0.8/stonfi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:36:46.537564 stonfi-0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-13 09:36:39.000000 stonfi-0.8/tests/test_http_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-13 09:36:39.000000 stonfi-0.8/tests/test_pool_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-13 09:36:39.000000 stonfi-0.8/tests/test_router_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-13 09:36:39.000000 stonfi-0.8/tests/test_swap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:16.024036 stonfi-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 08:56:06.000000 stonfi-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-14 08:56:16.024036 stonfi-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 08:56:06.000000 stonfi-0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-14 08:56:06.000000 stonfi-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:56:16.024036 stonfi-0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:16.020036 stonfi-0.9/stonfi/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-14 08:56:06.000000 stonfi-0.9/stonfi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-14 08:56:06.000000 stonfi-0.9/stonfi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:16.020036 stonfi-0.9/stonfi/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-14 08:56:06.000000 stonfi-0.9/stonfi/contracts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:16.024036 stonfi-0.9/stonfi/contracts/dex/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 08:56:06.000000 stonfi-0.9/stonfi/contracts/dex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:16.024036 stonfi-0.9/stonfi/contracts/dex/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-14 08:56:06.000000 stonfi-0.9/stonfi/contracts/dex/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 08:56:06.000000 stonfi-0.9/stonfi/contracts/dex/v1/lp_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-14 08:56:06.000000 stonfi-0.9/stonfi/contracts/dex/v1/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13895 2024-05-14 08:56:06.000000 stonfi-0.9/stonfi/contracts/dex/v1/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:16.024036 stonfi-0.9/stonfi/contracts/farm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:06.000000 stonfi-0.9/stonfi/contracts/farm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:16.024036 stonfi-0.9/stonfi/contracts/jetton/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-14 08:56:06.000000 stonfi-0.9/stonfi/contracts/jetton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-14 08:56:06.000000 stonfi-0.9/stonfi/contracts/jetton/jetton_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-14 08:56:06.000000 stonfi-0.9/stonfi/contracts/jetton/jetton_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:16.024036 stonfi-0.9/stonfi/contracts/pTON/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-14 08:56:06.000000 stonfi-0.9/stonfi/contracts/pTON/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-14 08:56:06.000000 stonfi-0.9/stonfi/contracts/pTON/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:16.024036 stonfi-0.9/stonfi/http/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 08:56:06.000000 stonfi-0.9/stonfi/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-14 08:56:06.000000 stonfi-0.9/stonfi/http/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-14 08:56:06.000000 stonfi-0.9/stonfi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:16.024036 stonfi-0.9/stonfi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-14 08:56:16.000000 stonfi-0.9/stonfi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-14 08:56:16.000000 stonfi-0.9/stonfi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:56:16.000000 stonfi-0.9/stonfi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 08:56:16.000000 stonfi-0.9/stonfi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:16.024036 stonfi-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 08:56:06.000000 stonfi-0.9/tests/test_http_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-14 08:56:06.000000 stonfi-0.9/tests/test_pool_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-14 08:56:06.000000 stonfi-0.9/tests/test_router_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-14 08:56:06.000000 stonfi-0.9/tests/test_swap.py
```

### Comparing `stonfi-0.8/LICENSE` & `stonfi-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stonfi-0.8/PKG-INFO` & `stonfi-0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stonfi
-Version: 0.8
+Version: 0.9
 Summary: Async Python SDK for StonFi DEX
 Author-email: "LapisMYT (Nikita Gavrilin)" <nikitagavrilin005@gmail.com>
 Project-URL: Homepage, https://github.com/lapismyt/ston-fi.py
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `stonfi-0.8/pyproject.toml` & `stonfi-0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "pytoniq", "aiohttp"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stonfi"
-version = "0.8"
+version = "0.9"
 description = "Async Python SDK for StonFi DEX"
 authors = [
     {name = "LapisMYT (Nikita Gavrilin)", email = "nikitagavrilin005@gmail.com"}
 ]
 readme = "README.md"
 classifiers = ["Development Status :: 4 - Beta",
               "Intended Audience :: Developers",
```

### Comparing `stonfi-0.8/stonfi/constants.py` & `stonfi-0.9/stonfi/constants.py`

 * *Files identical despite different names*

### Comparing `stonfi-0.8/stonfi/contracts/dex/v1/pool.py` & `stonfi-0.9/stonfi/contracts/dex/v1/pool.py`

 * *Files identical despite different names*

### Comparing `stonfi-0.8/stonfi/contracts/dex/v1/router.py` & `stonfi-0.9/stonfi/contracts/dex/v1/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
                                                               query_id = query_id,
                                                               response_address = user_wallet_address,
                                                               forward_amount = forward_gas_amount,
                                                               forward_payload = forward_payload)
         
         return {
             'to': offer_jetton_wallet.address.to_str(),
-            'payload': payload.to_boc(False),
+            'payload': payload,
             'amount': offer_amount + forward_gas_amount
         }
     
     async def create_provide_liquidity_body(self,
                                             router_wallet_address: Union[Address, str],
                                             min_lp_out: int):
         return begin_cell()\
```

### Comparing `stonfi-0.8/stonfi/contracts/jetton/jetton_root.py` & `stonfi-0.9/stonfi/contracts/jetton/jetton_root.py`

 * *Files identical despite different names*

### Comparing `stonfi-0.8/stonfi/contracts/jetton/jetton_wallet.py` & `stonfi-0.9/stonfi/contracts/jetton/jetton_wallet.py`

 * *Files identical despite different names*

### Comparing `stonfi-0.8/stonfi/http/api_client.py` & `stonfi-0.9/stonfi/http/api_client.py`

 * *Files identical despite different names*

### Comparing `stonfi-0.8/stonfi.egg-info/PKG-INFO` & `stonfi-0.9/stonfi.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stonfi
-Version: 0.8
+Version: 0.9
 Summary: Async Python SDK for StonFi DEX
 Author-email: "LapisMYT (Nikita Gavrilin)" <nikitagavrilin005@gmail.com>
 Project-URL: Homepage, https://github.com/lapismyt/ston-fi.py
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `stonfi-0.8/stonfi.egg-info/SOURCES.txt` & `stonfi-0.9/stonfi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stonfi-0.8/tests/test_pool_methods.py` & `stonfi-0.9/tests/test_pool_methods.py`

 * *Files identical despite different names*

### Comparing `stonfi-0.8/tests/test_router_methods.py` & `stonfi-0.9/tests/test_router_methods.py`

 * *Files identical despite different names*

### Comparing `stonfi-0.8/tests/test_swap.py` & `stonfi-0.9/tests/test_swap.py`

 * *Files identical despite different names*


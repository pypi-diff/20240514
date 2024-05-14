# Comparing `tmp/geckoterminal_py-0.1.2.tar.gz` & `tmp/geckoterminal_py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geckoterminal_py-0.1.2.tar", max compression
+gzip compressed data, was "geckoterminal_py-0.1.3.tar", max compression
```

## Comparing `geckoterminal_py-0.1.2.tar` & `geckoterminal_py-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-07-07 16:16:21.780816 geckoterminal_py-0.1.2/LICENSE
--rw-r--r--   0        0        0     2992 2023-07-14 04:36:57.323188 geckoterminal_py-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-07 16:16:21.784451 geckoterminal_py-0.1.2/geckoterminal_py/__init__.py
--rw-r--r--   0        0        0     9254 2023-07-14 04:54:51.682042 geckoterminal_py-0.1.2/geckoterminal_py/client.py
--rw-r--r--   0        0        0      600 2023-07-13 18:35:42.614243 geckoterminal_py-0.1.2/geckoterminal_py/constants.py
--rw-r--r--   0        0        0      788 2023-07-14 04:49:14.605507 geckoterminal_py-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3688 1970-01-01 00:00:00.000000 geckoterminal_py-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-07 16:16:21.780816 geckoterminal_py-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1639 2024-05-13 15:37:47.253417 geckoterminal_py-0.1.3/README.md
+-rw-r--r--   0        0        0      148 2024-05-13 14:29:48.079912 geckoterminal_py-0.1.3/geckoterminal_py/__init__.py
+-rw-r--r--   0        0        0      967 2024-05-13 13:41:18.150450 geckoterminal_py-0.1.3/geckoterminal_py/base_client.py
+-rw-r--r--   0        0        0        0 2024-05-13 14:29:11.362645 geckoterminal_py-0.1.3/geckoterminal_py/clients/__init__.py
+-rw-r--r--   0        0        0     4312 2024-05-13 14:29:03.389793 geckoterminal_py-0.1.3/geckoterminal_py/clients/async_client.py
+-rw-r--r--   0        0        0     4161 2024-05-13 15:33:12.929737 geckoterminal_py-0.1.3/geckoterminal_py/clients/sync_client.py
+-rw-r--r--   0        0        0     2604 2024-05-13 13:41:18.156668 geckoterminal_py-0.1.3/geckoterminal_py/constants.py
+-rw-r--r--   0        0        0      807 2024-05-14 17:47:46.422839 geckoterminal_py-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2236 1970-01-01 00:00:00.000000 geckoterminal_py-0.1.3/PKG-INFO
```

### Comparing `geckoterminal_py-0.1.2/LICENSE` & `geckoterminal_py-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geckoterminal_py-0.1.2/README.md` & `geckoterminal_py-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: geckoterminal-py
+Version: 0.1.3
+Summary: 
+Author: cardosofede
+Author-email: federico.cardoso.e@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiodns (>=3.0.0,<4.0.0)
+Requires-Dist: aioresponses (>=0.7.4,<0.8.0)
+Requires-Dist: cchardet (>=2.1.7,<3.0.0)
+Requires-Dist: glom (>=23.3.0,<24.0.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Description-Content-Type: text/markdown
+
 # GeckoTerminal Py
 
 GeckoTerminal Py is a Python client for the [GeckoTerminal](https://www.geckoterminal.com). It provides a user-friendly way to fetch network and pool data asynchronously or synchronously.
 
 ## Installation
 
 To install GeckoTerminal Py, use pip:
@@ -12,60 +30,54 @@
 
 ## Usage
 
 You can fetch data about networks using GeckoTerminal Py in two ways:
 
 ### Asynchronous usage
 
-
 ```python
-from geckoterminal_py.client import GeckoTerminalClient
+from geckoterminal_py import GeckoTerminalAsyncClient
 import asyncio
 
 
 async def main():
-    client = GeckoTerminalClient()
+    client = GeckoTerminalAsyncClient()
     networks_df = await client.get_networks()
     print(networks_df)
-    client.close()
+    await client.close()
+
 
 # In an asyncio environment, you'd use:
 asyncio.run(main())
 ```
 
 ### Synchronous usage
 
 ```python
-from geckoterminal_py.client import GeckoTerminalClient
+from geckoterminal_py import GeckoTerminalSyncClient
+
 
 def main():
-    client = GeckoTerminalClient()
-    networks_df = client.get_networks_sync()
+    client = GeckoTerminalSyncClient()
+    networks_df = client.get_networks()
     print(networks_df)
     client.close()
 
+
 main()
 ```
 
 ## Methods Available
 
 Here is a brief description of the methods available in the GeckoTerminalClient:
+Please check the examples notebook where you can find the usage of all of them.
+
+Methods:
+- **get_networks():**
+- **get_dexes_by_network(network_id: str):**
+- **get_top_pools_by_network(network_id: str):**
+- **get_top_pools_by_network_dex(network_id: str, dex_id: str):**
+- **get_top_pools_by_network_token(network_id: str, token_id: str):**
+- **get_new_pools_by_network(network_id: str):**
+- **get_new_pools_all_networks():**
+- **get_ohlcv(network_id: str, pool_address: str, timeframe: str, before_timestamp: int = None, currency: str = "usd", token: str = "base", limit: int = 1000):**
 
-Async methods:
-- **get_networks():** Fetches network data in an asynchronous way.
-- **get_dexes_by_network(network_id: str):** Asynchronously fetches decentralized exchange (dex) data by network ID.
-- **get_top_pools_by_network(network_id: str):** Asynchronously fetches top pool data by network ID.
-- **get_top_pools_by_network_dex(network_id: str, dex_id: str):** Asynchronously fetches top pool data by network and dex IDs.
-- **get_top_pools_by_network_token(network_id: str, token_id: str):** Asynchronously fetches top pool data by network and token IDs.
-- **get_new_pools_by_network(network_id: str):** Asynchronously fetches data of new pools by network ID.
-- **get_new_pools_all_networks():** Asynchronously fetches data of new pools across all networks.
-- **get_ohlcv(network_id: str, pool_address: str, timeframe: str, before_timestamp: int = None, currency: str = "usd", token: str = "base", limit: int = 1000):** Asynchronously fetches OHLCV data for a pool.
-
-Sync methods:
-- **get_networks_sync():** Fetches network data in a synchronous way.
-- **get_dexes_by_network_sync(network_id: str):** Synchronously fetches dex data by network ID.
-- **get_top_pools_by_network_sync(network_id: str):** Synchronously fetches top pool data by network ID.
-- **get_top_pools_by_network_dex_sync(network_id: str, dex_id: str):** Synchronously fetches top pool data by network and dex IDs.
-- **get_top_pools_by_network_token_sync(network_id: str, token_id: str):** Synchronously fetches top pool data by network and token IDs.
-- **get_new_pools_by_network_sync(network_id: str):** Synchronously fetches data of new pools by network ID.
-- **get_new_pools_all_networks_sync():** Synchronously fetches data of new pools across all networks.
-- **get_ohlcv_sync(network_id: str, pool_address: str, timeframe: str, before_timestamp: int = None, currency: str = "usd", token: str = "base", limit: int = 1000):** Synchronously fetches OHLCV data for a pool.
```

### Comparing `geckoterminal_py-0.1.2/pyproject.toml` & `geckoterminal_py-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.poetry]
 name = "geckoterminal-py"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["cardosofede <federico.cardoso.e@gmail.com>"]
 readme = "README.md"
 packages = [{include = "geckoterminal_py"}]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-aiohttp = "^3.8.4"
+python = "^3.10"
 aiodns = "^3.0.0"
 cchardet = "^2.1.7"
 aioresponses = "^0.7.4"
 glom = "^23.3.0"
 pandas = "^2.0.3"
+httpx = "^0.27.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
 coverage = "^7.2.7"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.278"
 pre-commit = "^3.3.3"
 isort = "^5.12.0"
+jupyter = "^1.0.0"
 
 [tool.ruff]
 # Decrease the maximum line length to 79 characters.
 line-length = 100
 src = ["src"]
 
 [tool.ruff.pydocstyle]
```


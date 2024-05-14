# Comparing `tmp/parsecfi-0.1.0.tar.gz` & `tmp/parsecfi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsecfi-0.1.0.tar", last modified: Thu Aug 31 18:13:39 2023, max compression
+gzip compressed data, was "parsecfi-0.1.1.tar", last modified: Tue May 14 17:23:25 2024, max compression
```

## Comparing `parsecfi-0.1.0.tar` & `parsecfi-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2023-08-31 18:13:39.366411 parsecfi-0.1.0/
--rw-r--r--   0 wilburforce   (501) staff       (20)      179 2023-08-31 18:13:39.365594 parsecfi-0.1.0/PKG-INFO
--rw-r--r--   0 wilburforce   (501) staff       (20)     1065 2023-08-31 18:12:46.000000 parsecfi-0.1.0/README.md
-drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2023-08-31 18:13:39.359352 parsecfi-0.1.0/parsecfi/
--rw-r--r--   0 wilburforce   (501) staff       (20)       28 2023-08-31 17:05:55.000000 parsecfi-0.1.0/parsecfi/__init__.py
-drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2023-08-31 18:13:39.360331 parsecfi-0.1.0/parsecfi/lib/
--rw-r--r--   0 wilburforce   (501) staff       (20)        0 2023-05-22 23:38:30.000000 parsecfi-0.1.0/parsecfi/lib/__init__.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      397 2023-08-31 17:52:45.000000 parsecfi-0.1.0/parsecfi/lib/endpoints.py
-drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2023-08-31 18:13:39.365179 parsecfi-0.1.0/parsecfi/lib/endpoints_list/
--rw-r--r--   0 wilburforce   (501) staff       (20)        0 2023-05-22 23:41:41.000000 parsecfi-0.1.0/parsecfi/lib/endpoints_list/__init__.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      321 2023-08-31 17:56:02.000000 parsecfi-0.1.0/parsecfi/lib/endpoints_list/address.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      445 2023-08-07 19:03:39.000000 parsecfi-0.1.0/parsecfi/lib/endpoints_list/candles.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      707 2023-08-07 18:02:37.000000 parsecfi-0.1.0/parsecfi/lib/endpoints_list/conc_liquidity_positions.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      663 2023-08-31 17:43:09.000000 parsecfi-0.1.0/parsecfi/lib/endpoints_list/contract_logs.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      577 2023-08-08 00:45:47.000000 parsecfi-0.1.0/parsecfi/lib/endpoints_list/dex_trades.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      565 2023-08-02 01:08:59.000000 parsecfi-0.1.0/parsecfi/lib/endpoints_list/lending_market.py
--rw-r--r--   0 wilburforce   (501) staff       (20)        0 2023-08-02 01:05:27.000000 parsecfi-0.1.0/parsecfi/lib/endpoints_list/lending_positions.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      643 2023-08-07 17:54:50.000000 parsecfi-0.1.0/parsecfi/lib/endpoints_list/liquidity_pools.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      435 2023-08-08 00:34:08.000000 parsecfi-0.1.0/parsecfi/lib/endpoints_list/nft_collection.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      649 2023-08-08 00:34:06.000000 parsecfi-0.1.0/parsecfi/lib/endpoints_list/nft_trades.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      663 2023-08-02 01:04:23.000000 parsecfi-0.1.0/parsecfi/lib/endpoints_list/token_acc.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      468 2023-08-02 01:01:34.000000 parsecfi-0.1.0/parsecfi/lib/endpoints_list/token_holders.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      789 2023-08-07 17:35:20.000000 parsecfi-0.1.0/parsecfi/lib/endpoints_list/transfers.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      725 2023-08-02 20:13:48.000000 parsecfi-0.1.0/parsecfi/lib/endpoints_list/trending_contracts.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      848 2023-08-31 17:13:57.000000 parsecfi-0.1.0/parsecfi/parsecfi.py
-drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2023-08-31 18:13:39.360107 parsecfi-0.1.0/parsecfi.egg-info/
--rw-r--r--   0 wilburforce   (501) staff       (20)      179 2023-08-31 18:13:39.000000 parsecfi-0.1.0/parsecfi.egg-info/PKG-INFO
--rw-r--r--   0 wilburforce   (501) staff       (20)      938 2023-08-31 18:13:39.000000 parsecfi-0.1.0/parsecfi.egg-info/SOURCES.txt
--rw-r--r--   0 wilburforce   (501) staff       (20)        1 2023-08-31 18:13:39.000000 parsecfi-0.1.0/parsecfi.egg-info/dependency_links.txt
--rw-r--r--   0 wilburforce   (501) staff       (20)       16 2023-08-31 18:13:39.000000 parsecfi-0.1.0/parsecfi.egg-info/requires.txt
--rw-r--r--   0 wilburforce   (501) staff       (20)        9 2023-08-31 18:13:39.000000 parsecfi-0.1.0/parsecfi.egg-info/top_level.txt
--rw-r--r--   0 wilburforce   (501) staff       (20)       38 2023-08-31 18:13:39.366485 parsecfi-0.1.0/setup.cfg
--rw-r--r--   0 wilburforce   (501) staff       (20)      367 2023-08-31 18:13:15.000000 parsecfi-0.1.0/setup.py
+drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2024-05-14 17:23:25.158169 parsecfi-0.1.1/
+-rw-r--r--   0 wilburforce   (501) staff       (20)      179 2024-05-14 17:23:25.157984 parsecfi-0.1.1/PKG-INFO
+-rw-r--r--   0 wilburforce   (501) staff       (20)     1065 2023-08-31 18:12:46.000000 parsecfi-0.1.1/README.md
+drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2024-05-14 17:23:25.150695 parsecfi-0.1.1/parsecfi/
+-rw-r--r--   0 wilburforce   (501) staff       (20)       28 2023-08-31 17:05:55.000000 parsecfi-0.1.1/parsecfi/__init__.py
+drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2024-05-14 17:23:25.152961 parsecfi-0.1.1/parsecfi/lib/
+-rw-r--r--   0 wilburforce   (501) staff       (20)        0 2023-05-22 23:38:30.000000 parsecfi-0.1.1/parsecfi/lib/__init__.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      444 2024-05-14 17:19:02.000000 parsecfi-0.1.1/parsecfi/lib/endpoints.py
+drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2024-05-14 17:23:25.157560 parsecfi-0.1.1/parsecfi/lib/endpoints_list/
+-rw-r--r--   0 wilburforce   (501) staff       (20)        0 2023-05-22 23:41:41.000000 parsecfi-0.1.1/parsecfi/lib/endpoints_list/__init__.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      321 2023-08-31 17:56:02.000000 parsecfi-0.1.1/parsecfi/lib/endpoints_list/address.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      445 2023-08-07 19:03:39.000000 parsecfi-0.1.1/parsecfi/lib/endpoints_list/candles.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      707 2023-08-07 18:02:37.000000 parsecfi-0.1.1/parsecfi/lib/endpoints_list/conc_liquidity_positions.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      663 2023-08-31 17:43:09.000000 parsecfi-0.1.1/parsecfi/lib/endpoints_list/contract_logs.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      577 2023-08-08 00:45:47.000000 parsecfi-0.1.1/parsecfi/lib/endpoints_list/dex_trades.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      565 2023-08-02 01:08:59.000000 parsecfi-0.1.1/parsecfi/lib/endpoints_list/lending_market.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)        0 2023-08-02 01:05:27.000000 parsecfi-0.1.1/parsecfi/lib/endpoints_list/lending_positions.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      643 2023-08-07 17:54:50.000000 parsecfi-0.1.1/parsecfi/lib/endpoints_list/liquidity_pools.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      435 2023-08-08 00:34:08.000000 parsecfi-0.1.1/parsecfi/lib/endpoints_list/nft_collection.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      649 2023-08-08 00:34:06.000000 parsecfi-0.1.1/parsecfi/lib/endpoints_list/nft_trades.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      663 2023-08-02 01:04:23.000000 parsecfi-0.1.1/parsecfi/lib/endpoints_list/token_acc.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      468 2023-08-02 01:01:34.000000 parsecfi-0.1.1/parsecfi/lib/endpoints_list/token_holders.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      964 2024-05-14 17:18:35.000000 parsecfi-0.1.1/parsecfi/lib/endpoints_list/transactions.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      789 2023-08-07 17:35:20.000000 parsecfi-0.1.1/parsecfi/lib/endpoints_list/transfers.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      725 2023-08-02 20:13:48.000000 parsecfi-0.1.1/parsecfi/lib/endpoints_list/trending_contracts.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      848 2023-08-31 17:13:57.000000 parsecfi-0.1.1/parsecfi/parsecfi.py
+drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2024-05-14 17:23:25.152716 parsecfi-0.1.1/parsecfi.egg-info/
+-rw-r--r--   0 wilburforce   (501) staff       (20)      179 2024-05-14 17:23:25.000000 parsecfi-0.1.1/parsecfi.egg-info/PKG-INFO
+-rw-r--r--   0 wilburforce   (501) staff       (20)      982 2024-05-14 17:23:25.000000 parsecfi-0.1.1/parsecfi.egg-info/SOURCES.txt
+-rw-r--r--   0 wilburforce   (501) staff       (20)        1 2024-05-14 17:23:25.000000 parsecfi-0.1.1/parsecfi.egg-info/dependency_links.txt
+-rw-r--r--   0 wilburforce   (501) staff       (20)       16 2024-05-14 17:23:25.000000 parsecfi-0.1.1/parsecfi.egg-info/requires.txt
+-rw-r--r--   0 wilburforce   (501) staff       (20)        9 2024-05-14 17:23:25.000000 parsecfi-0.1.1/parsecfi.egg-info/top_level.txt
+-rw-r--r--   0 wilburforce   (501) staff       (20)       38 2024-05-14 17:23:25.158378 parsecfi-0.1.1/setup.cfg
+-rw-r--r--   0 wilburforce   (501) staff       (20)      367 2024-05-14 17:22:59.000000 parsecfi-0.1.1/setup.py
```

### Comparing `parsecfi-0.1.0/README.md` & `parsecfi-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `parsecfi-0.1.0/parsecfi/lib/endpoints_list/conc_liquidity_positions.py` & `parsecfi-0.1.1/parsecfi/lib/endpoints_list/conc_liquidity_positions.py`

 * *Files identical despite different names*

### Comparing `parsecfi-0.1.0/parsecfi/lib/endpoints_list/contract_logs.py` & `parsecfi-0.1.1/parsecfi/lib/endpoints_list/contract_logs.py`

 * *Files identical despite different names*

### Comparing `parsecfi-0.1.0/parsecfi/lib/endpoints_list/dex_trades.py` & `parsecfi-0.1.1/parsecfi/lib/endpoints_list/dex_trades.py`

 * *Files identical despite different names*

### Comparing `parsecfi-0.1.0/parsecfi/lib/endpoints_list/lending_market.py` & `parsecfi-0.1.1/parsecfi/lib/endpoints_list/lending_market.py`

 * *Files identical despite different names*

### Comparing `parsecfi-0.1.0/parsecfi/lib/endpoints_list/liquidity_pools.py` & `parsecfi-0.1.1/parsecfi/lib/endpoints_list/liquidity_pools.py`

 * *Files identical despite different names*

### Comparing `parsecfi-0.1.0/parsecfi/lib/endpoints_list/nft_trades.py` & `parsecfi-0.1.1/parsecfi/lib/endpoints_list/nft_trades.py`

 * *Files identical despite different names*

### Comparing `parsecfi-0.1.0/parsecfi/lib/endpoints_list/token_acc.py` & `parsecfi-0.1.1/parsecfi/lib/endpoints_list/token_acc.py`

 * *Files identical despite different names*

### Comparing `parsecfi-0.1.0/parsecfi/lib/endpoints_list/transfers.py` & `parsecfi-0.1.1/parsecfi/lib/endpoints_list/transfers.py`

 * *Files identical despite different names*

### Comparing `parsecfi-0.1.0/parsecfi/lib/endpoints_list/trending_contracts.py` & `parsecfi-0.1.1/parsecfi/lib/endpoints_list/trending_contracts.py`

 * *Files identical despite different names*

### Comparing `parsecfi-0.1.0/parsecfi/parsecfi.py` & `parsecfi-0.1.1/parsecfi/parsecfi.py`

 * *Files identical despite different names*

### Comparing `parsecfi-0.1.0/parsecfi.egg-info/SOURCES.txt` & `parsecfi-0.1.1/parsecfi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,10 @@
 parsecfi/lib/endpoints_list/lending_market.py
 parsecfi/lib/endpoints_list/lending_positions.py
 parsecfi/lib/endpoints_list/liquidity_pools.py
 parsecfi/lib/endpoints_list/nft_collection.py
 parsecfi/lib/endpoints_list/nft_trades.py
 parsecfi/lib/endpoints_list/token_acc.py
 parsecfi/lib/endpoints_list/token_holders.py
+parsecfi/lib/endpoints_list/transactions.py
 parsecfi/lib/endpoints_list/transfers.py
 parsecfi/lib/endpoints_list/trending_contracts.py
```


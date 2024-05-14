# Comparing `tmp/mns_common-1.0.9.2.tar.gz` & `tmp/mns_common-1.0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns_common-1.0.9.2.tar", last modified: Sun May 12 14:01:01 2024, max compression
+gzip compressed data, was "mns_common-1.0.9.3.tar", last modified: Tue May 14 15:37:24 2024, max compression
```

## Comparing `mns_common-1.0.9.2.tar` & `mns_common-1.0.9.3.tar`

### file list

```diff
@@ -1,122 +1,125 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.224554 mns_common-1.0.9.2/
--rw-rw-rw-   0        0        0       59 2024-05-12 14:01:01.224040 mns_common-1.0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.0.9.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.186280 mns_common-1.0.9.2/mns_common/
--rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.0.9.2/mns_common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.189378 mns_common-1.0.9.2/mns_common/api/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.9.2/mns_common/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.192389 mns_common-1.0.9.2/mns_common/api/akshare/
--rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.0.9.2/mns_common/api/akshare/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.0.9.2/mns_common/api/akshare/k_line_api.py
--rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.0.9.2/mns_common/api/akshare/stock_bid_ask_api.py
--rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.0.9.2/mns_common/api/akshare/stock_dt_pool.py
--rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.0.9.2/mns_common/api/akshare/stock_zb_pool.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.0.9.2/mns_common/api/akshare/stock_zt_pool_api.py
--rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.0.9.2/mns_common/api/akshare/yjyg_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.195385 mns_common-1.0.9.2/mns_common/api/em/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.9.2/mns_common/api/em/__init__.py
--rw-rw-rw-   0        0        0     8352 2024-05-10 13:01:52.000000 mns_common-1.0.9.2/mns_common/api/em/east_money_stock_api.py
--rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.0.9.2/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
--rw-rw-rw-   0        0        0     7241 2024-05-10 14:46:45.000000 mns_common-1.0.9.2/mns_common/api/em/east_money_stock_hk_api.py
--rw-rw-rw-   0        0        0    14960 2024-05-10 12:40:48.000000 mns_common-1.0.9.2/mns_common/api/em/east_money_stock_v2_api.py
--rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.0.9.2/mns_common/api/em/em_concept_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.195385 mns_common-1.0.9.2/mns_common/api/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.2/mns_common/api/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.196381 mns_common-1.0.9.2/mns_common/api/kpl/common/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.9.2/mns_common/api/kpl/common/__init__.py
--rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.0.9.2/mns_common/api/kpl/common/kpl_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.197385 mns_common-1.0.9.2/mns_common/api/kpl/concept/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.9.2/mns_common/api/kpl/concept/__init__.py
--rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.0.9.2/mns_common/api/kpl/concept/kpl_concept_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.198380 mns_common-1.0.9.2/mns_common/api/kpl/constant/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.9.2/mns_common/api/kpl/constant/__init__.py
--rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.0.9.2/mns_common/api/kpl/constant/kpl_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.199072 mns_common-1.0.9.2/mns_common/api/kpl/industry/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.9.2/mns_common/api/kpl/industry/__init__.py
--rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.0.9.2/mns_common/api/kpl/industry/kpl_industry_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.199584 mns_common-1.0.9.2/mns_common/api/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.9.2/mns_common/api/kpl/selection/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 13:55:26.000000 mns_common-1.0.9.2/mns_common/api/kpl/selection/kpl_selection_plate_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.201574 mns_common-1.0.9.2/mns_common/api/kpl/symbol/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.9.2/mns_common/api/kpl/symbol/__init__.py
--rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.0.9.2/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
--rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.0.9.2/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
--rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.0.9.2/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.202580 mns_common-1.0.9.2/mns_common/api/msg/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.9.2/mns_common/api/msg/__init__.py
--rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.0.9.2/mns_common/api/msg/push_msg_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.203572 mns_common-1.0.9.2/mns_common/api/ths/
--rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.0.9.2/mns_common/api/ths/__init__.py
--rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.0.9.2/mns_common/api/ths/ths_big_deal_api.py
--rw-rw-rw-   0        0        0    40250 2024-05-11 03:03:44.000000 mns_common-1.0.9.2/mns_common/api/ths/ths_stock_api.py
--rw-rw-rw-   0        0        0     6751 2024-05-09 15:04:44.000000 mns_common-1.0.9.2/mns_common/api/ths/ths_stock_zt_pool_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.205088 mns_common-1.0.9.2/mns_common/component/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.0.9.2/mns_common/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.205600 mns_common-1.0.9.2/mns_common/component/cache/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.0.9.2/mns_common/component/cache/__init__.py
--rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.0.9.2/mns_common/component/cache/cache_service.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.207136 mns_common-1.0.9.2/mns_common/component/classify/
--rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.0.9.2/mns_common/component/classify/__init__.py
--rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.0.9.2/mns_common/component/classify/classify_constant.py
--rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.0.9.2/mns_common/component/classify/symbol_classify_api.py
--rw-rw-rw-   0        0        0     5097 2024-05-10 15:14:36.000000 mns_common-1.0.9.2/mns_common/component/common_service_fun_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.207652 mns_common-1.0.9.2/mns_common/component/company/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.2/mns_common/component/company/__init__.py
--rw-rw-rw-   0        0        0     6987 2023-12-17 11:37:16.000000 mns_common-1.0.9.2/mns_common/component/company/company_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.209187 mns_common-1.0.9.2/mns_common/component/concept/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.2/mns_common/component/concept/__init__.py
--rw-rw-rw-   0        0        0     3235 2024-05-09 14:23:16.000000 mns_common-1.0.9.2/mns_common/component/concept/kpl_concept_common_service_api.py
--rw-rw-rw-   0        0        0     9637 2024-04-30 09:46:26.000000 mns_common-1.0.9.2/mns_common/component/concept/ths_concept_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.210213 mns_common-1.0.9.2/mns_common/component/data/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.0.9.2/mns_common/component/data/__init__.py
--rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.0.9.2/mns_common/component/data/data_init_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.210727 mns_common-1.0.9.2/mns_common/component/industry/
--rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.0.9.2/mns_common/component/industry/__init__.py
--rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.0.9.2/mns_common/component/industry/ths_industry_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.211237 mns_common-1.0.9.2/mns_common/component/k_line/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.2/mns_common/component/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.212276 mns_common-1.0.9.2/mns_common/component/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.0.9.2/mns_common/component/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.0.9.2/mns_common/component/k_line/clean/k_line_param.py
--rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.0.9.2/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.213303 mns_common-1.0.9.2/mns_common/component/k_line/common/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.0.9.2/mns_common/component/k_line/common/__init__.py
--rw-rw-rw-   0        0        0     4449 2023-12-29 04:25:17.000000 mns_common-1.0.9.2/mns_common/component/k_line/common/k_line_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.214841 mns_common-1.0.9.2/mns_common/component/k_line/patterns/
--rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.0.9.2/mns_common/component/k_line/patterns/__init__.py
--rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.0.9.2/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
--rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.0.9.2/mns_common/component/k_line/patterns/pattern_Enum.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.215350 mns_common-1.0.9.2/mns_common/component/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.2/mns_common/component/real_time/__init__.py
--rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.0.9.2/mns_common/component/real_time/real_time_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.215859 mns_common-1.0.9.2/mns_common/component/trade/
--rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.0.9.2/mns_common/component/trade/__init__.py
--rw-rw-rw-   0        0        0     3120 2024-05-08 07:34:38.000000 mns_common-1.0.9.2/mns_common/component/trade/trade_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.216854 mns_common-1.0.9.2/mns_common/component/trade_date/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.2/mns_common/component/trade_date/__init__.py
--rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.0.9.2/mns_common/component/trade_date/trade_date_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.217867 mns_common-1.0.9.2/mns_common/component/zt/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.2/mns_common/component/zt/__init__.py
--rw-rw-rw-   0        0        0     8650 2024-05-12 14:00:57.000000 mns_common-1.0.9.2/mns_common/component/zt/zt_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.220427 mns_common-1.0.9.2/mns_common/constant/
--rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.0.9.2/mns_common/constant/__init__.py
--rw-rw-rw-   0        0        0     1567 2024-05-03 14:48:19.000000 mns_common-1.0.9.2/mns_common/constant/db_name_constant.py
--rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.0.9.2/mns_common/constant/kpl_selection_no_choose_constant.py
--rw-rw-rw-   0        0        0      347 2024-05-01 15:03:02.000000 mns_common-1.0.9.2/mns_common/constant/self_choose_constant.py
--rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.0.9.2/mns_common/constant/ths_concept_no_choose_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.220945 mns_common-1.0.9.2/mns_common/db/
--rw-rw-rw-   0        0        0    10816 2024-04-24 14:49:25.000000 mns_common-1.0.9.2/mns_common/db/MongodbUtil.py
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.9.2/mns_common/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.223524 mns_common-1.0.9.2/mns_common/utils/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.9.2/mns_common/utils/__init__.py
--rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.0.9.2/mns_common/utils/async_fun.py
--rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.0.9.2/mns_common/utils/data_frame_util.py
--rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.0.9.2/mns_common/utils/date_handle_util.py
--rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.0.9.2/mns_common/utils/ip_util.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:01:01.224040 mns_common-1.0.9.2/mns_common.egg-info/
--rw-rw-rw-   0        0        0       59 2024-05-12 14:01:01.000000 mns_common-1.0.9.2/mns_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3708 2024-05-12 14:01:01.000000 mns_common-1.0.9.2/mns_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 14:01:01.000000 mns_common-1.0.9.2/mns_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-12 14:01:01.000000 mns_common-1.0.9.2/mns_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 14:01:01.224554 mns_common-1.0.9.2/setup.cfg
--rw-rw-rw-   0        0        0      466 2024-05-12 14:00:57.000000 mns_common-1.0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.630073 mns_common-1.0.9.3/
+-rw-rw-rw-   0        0        0       59 2024-05-14 15:37:24.629588 mns_common-1.0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.0.9.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.593684 mns_common-1.0.9.3/mns_common/
+-rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.0.9.3/mns_common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.595679 mns_common-1.0.9.3/mns_common/api/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.9.3/mns_common/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.598670 mns_common-1.0.9.3/mns_common/api/akshare/
+-rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.0.9.3/mns_common/api/akshare/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.0.9.3/mns_common/api/akshare/k_line_api.py
+-rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.0.9.3/mns_common/api/akshare/stock_bid_ask_api.py
+-rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.0.9.3/mns_common/api/akshare/stock_dt_pool.py
+-rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.0.9.3/mns_common/api/akshare/stock_zb_pool.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.0.9.3/mns_common/api/akshare/stock_zt_pool_api.py
+-rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.0.9.3/mns_common/api/akshare/yjyg_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.600665 mns_common-1.0.9.3/mns_common/api/em/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.9.3/mns_common/api/em/__init__.py
+-rw-rw-rw-   0        0        0     8352 2024-05-10 13:01:52.000000 mns_common-1.0.9.3/mns_common/api/em/east_money_stock_api.py
+-rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.0.9.3/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
+-rw-rw-rw-   0        0        0     7511 2024-05-14 08:11:24.000000 mns_common-1.0.9.3/mns_common/api/em/east_money_stock_hk_api.py
+-rw-rw-rw-   0        0        0    14960 2024-05-10 12:40:48.000000 mns_common-1.0.9.3/mns_common/api/em/east_money_stock_v2_api.py
+-rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.0.9.3/mns_common/api/em/em_concept_index_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.601662 mns_common-1.0.9.3/mns_common/api/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.3/mns_common/api/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.601662 mns_common-1.0.9.3/mns_common/api/kpl/common/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.9.3/mns_common/api/kpl/common/__init__.py
+-rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.0.9.3/mns_common/api/kpl/common/kpl_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.602660 mns_common-1.0.9.3/mns_common/api/kpl/concept/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.9.3/mns_common/api/kpl/concept/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.0.9.3/mns_common/api/kpl/concept/kpl_concept_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.603685 mns_common-1.0.9.3/mns_common/api/kpl/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.9.3/mns_common/api/kpl/constant/__init__.py
+-rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.0.9.3/mns_common/api/kpl/constant/kpl_constant.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.604682 mns_common-1.0.9.3/mns_common/api/kpl/industry/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.9.3/mns_common/api/kpl/industry/__init__.py
+-rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.0.9.3/mns_common/api/kpl/industry/kpl_industry_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.605680 mns_common-1.0.9.3/mns_common/api/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.9.3/mns_common/api/kpl/selection/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 13:55:26.000000 mns_common-1.0.9.3/mns_common/api/kpl/selection/kpl_selection_plate_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.606678 mns_common-1.0.9.3/mns_common/api/kpl/symbol/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.9.3/mns_common/api/kpl/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.0.9.3/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
+-rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.0.9.3/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
+-rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.0.9.3/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.607648 mns_common-1.0.9.3/mns_common/api/msg/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.9.3/mns_common/api/msg/__init__.py
+-rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.0.9.3/mns_common/api/msg/push_msg_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.609641 mns_common-1.0.9.3/mns_common/api/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.0.9.3/mns_common/api/ths/__init__.py
+-rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.0.9.3/mns_common/api/ths/ths_big_deal_api.py
+-rw-rw-rw-   0        0        0    40309 2024-05-14 08:22:47.000000 mns_common-1.0.9.3/mns_common/api/ths/ths_stock_api.py
+-rw-rw-rw-   0        0        0     6751 2024-05-09 15:04:44.000000 mns_common-1.0.9.3/mns_common/api/ths/ths_stock_zt_pool_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.610638 mns_common-1.0.9.3/mns_common/component/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.0.9.3/mns_common/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.611636 mns_common-1.0.9.3/mns_common/component/cache/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.0.9.3/mns_common/component/cache/__init__.py
+-rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.0.9.3/mns_common/component/cache/cache_service.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.612633 mns_common-1.0.9.3/mns_common/component/classify/
+-rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.0.9.3/mns_common/component/classify/__init__.py
+-rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.0.9.3/mns_common/component/classify/classify_constant.py
+-rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.0.9.3/mns_common/component/classify/symbol_classify_api.py
+-rw-rw-rw-   0        0        0     5097 2024-05-10 15:14:36.000000 mns_common-1.0.9.3/mns_common/component/common_service_fun_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.613630 mns_common-1.0.9.3/mns_common/component/company/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.3/mns_common/component/company/__init__.py
+-rw-rw-rw-   0        0        0     6987 2023-12-17 11:37:16.000000 mns_common-1.0.9.3/mns_common/component/company/company_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.614628 mns_common-1.0.9.3/mns_common/component/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.3/mns_common/component/concept/__init__.py
+-rw-rw-rw-   0        0        0     3235 2024-05-09 14:23:16.000000 mns_common-1.0.9.3/mns_common/component/concept/kpl_concept_common_service_api.py
+-rw-rw-rw-   0        0        0     9637 2024-04-30 09:46:26.000000 mns_common-1.0.9.3/mns_common/component/concept/ths_concept_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.615625 mns_common-1.0.9.3/mns_common/component/data/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.0.9.3/mns_common/component/data/__init__.py
+-rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.0.9.3/mns_common/component/data/data_init_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.615625 mns_common-1.0.9.3/mns_common/component/industry/
+-rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.0.9.3/mns_common/component/industry/__init__.py
+-rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.0.9.3/mns_common/component/industry/ths_industry_index_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.616622 mns_common-1.0.9.3/mns_common/component/k_line/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.3/mns_common/component/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.617620 mns_common-1.0.9.3/mns_common/component/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.0.9.3/mns_common/component/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.0.9.3/mns_common/component/k_line/clean/k_line_param.py
+-rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.0.9.3/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.618617 mns_common-1.0.9.3/mns_common/component/k_line/common/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.0.9.3/mns_common/component/k_line/common/__init__.py
+-rw-rw-rw-   0        0        0     4449 2023-12-29 04:25:17.000000 mns_common-1.0.9.3/mns_common/component/k_line/common/k_line_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.619614 mns_common-1.0.9.3/mns_common/component/k_line/patterns/
+-rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.0.9.3/mns_common/component/k_line/patterns/__init__.py
+-rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.0.9.3/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
+-rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.0.9.3/mns_common/component/k_line/patterns/pattern_Enum.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.620612 mns_common-1.0.9.3/mns_common/component/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.3/mns_common/component/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.0.9.3/mns_common/component/real_time/real_time_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.621609 mns_common-1.0.9.3/mns_common/component/self_choose/
+-rw-rw-rw-   0        0        0      163 2024-05-14 15:36:27.000000 mns_common-1.0.9.3/mns_common/component/self_choose/__init__.py
+-rw-rw-rw-   0        0        0      989 2024-05-14 15:36:27.000000 mns_common-1.0.9.3/mns_common/component/self_choose/black_list_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.622606 mns_common-1.0.9.3/mns_common/component/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.0.9.3/mns_common/component/trade/__init__.py
+-rw-rw-rw-   0        0        0     3120 2024-05-08 07:34:38.000000 mns_common-1.0.9.3/mns_common/component/trade/trade_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.622606 mns_common-1.0.9.3/mns_common/component/trade_date/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.3/mns_common/component/trade_date/__init__.py
+-rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.0.9.3/mns_common/component/trade_date/trade_date_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.623604 mns_common-1.0.9.3/mns_common/component/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.3/mns_common/component/zt/__init__.py
+-rw-rw-rw-   0        0        0     8650 2024-05-12 14:00:57.000000 mns_common-1.0.9.3/mns_common/component/zt/zt_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.625598 mns_common-1.0.9.3/mns_common/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.0.9.3/mns_common/constant/__init__.py
+-rw-rw-rw-   0        0        0     1567 2024-05-03 14:48:19.000000 mns_common-1.0.9.3/mns_common/constant/db_name_constant.py
+-rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.0.9.3/mns_common/constant/kpl_selection_no_choose_constant.py
+-rw-rw-rw-   0        0        0      347 2024-05-01 15:03:02.000000 mns_common-1.0.9.3/mns_common/constant/self_choose_constant.py
+-rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.0.9.3/mns_common/constant/ths_concept_no_choose_constant.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.626596 mns_common-1.0.9.3/mns_common/db/
+-rw-rw-rw-   0        0        0    10816 2024-04-24 14:49:25.000000 mns_common-1.0.9.3/mns_common/db/MongodbUtil.py
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.9.3/mns_common/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.628590 mns_common-1.0.9.3/mns_common/utils/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.9.3/mns_common/utils/__init__.py
+-rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.0.9.3/mns_common/utils/async_fun.py
+-rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.0.9.3/mns_common/utils/data_frame_util.py
+-rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.0.9.3/mns_common/utils/date_handle_util.py
+-rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.0.9.3/mns_common/utils/ip_util.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:37:24.629588 mns_common-1.0.9.3/mns_common.egg-info/
+-rw-rw-rw-   0        0        0       59 2024-05-14 15:37:24.000000 mns_common-1.0.9.3/mns_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3812 2024-05-14 15:37:24.000000 mns_common-1.0.9.3/mns_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 15:37:24.000000 mns_common-1.0.9.3/mns_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-14 15:37:24.000000 mns_common-1.0.9.3/mns_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 15:37:24.630073 mns_common-1.0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0      466 2024-05-14 15:36:27.000000 mns_common-1.0.9.3/setup.py
```

### Comparing `mns_common-1.0.9.2/README.md` & `mns_common-1.0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/akshare/k_line_api.py` & `mns_common-1.0.9.3/mns_common/api/akshare/k_line_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/akshare/stock_bid_ask_api.py` & `mns_common-1.0.9.3/mns_common/api/akshare/stock_bid_ask_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/akshare/stock_dt_pool.py` & `mns_common-1.0.9.3/mns_common/api/akshare/stock_dt_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/akshare/stock_zb_pool.py` & `mns_common-1.0.9.3/mns_common/api/akshare/stock_zb_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/akshare/stock_zt_pool_api.py` & `mns_common-1.0.9.3/mns_common/api/akshare/stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/akshare/yjyg_sync_api.py` & `mns_common-1.0.9.3/mns_common/api/akshare/yjyg_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/em/east_money_stock_api.py` & `mns_common-1.0.9.3/mns_common/api/em/east_money_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py` & `mns_common-1.0.9.3/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/em/east_money_stock_hk_api.py` & `mns_common-1.0.9.3/mns_common/api/em/east_money_stock_hk_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,20 @@
     # 只有外盘没有内盘
     temp_df.loc[temp_df["inner_disk"] == 0, ['disk_ratio']] = 1688
     return temp_df
 
 
 if __name__ == '__main__':
     temp_df = stock_hk_spot_em()
+    # 外盘与内盘的金额差额
+    temp_df['disk_diff_amount'] = round(
+        (temp_df['outer_disk'] - temp_df['inner_disk']) * temp_df[
+            "now_price"] * 100,
+        2)
+    temp_df = temp_df.sort_values(by=['disk_diff_amount'], ascending=False)
     temp_df = temp_df.sort_values(by=['today_main_net_inflow'], ascending=False)
     temp_df = temp_df.loc[temp_df['industry'] != '-']
     sum_amount = round(sum(temp_df['amount']) / 100000000, 2)
     sum_today_main_net_inflow = round(sum(temp_df['today_main_net_inflow']) / 100000000, 2)
 
     import akshare as ak
```

### Comparing `mns_common-1.0.9.2/mns_common/api/em/east_money_stock_v2_api.py` & `mns_common-1.0.9.3/mns_common/api/em/east_money_stock_v2_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/em/em_concept_index_api.py` & `mns_common-1.0.9.3/mns_common/api/em/em_concept_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/kpl/common/kpl_common_api.py` & `mns_common-1.0.9.3/mns_common/api/kpl/common/kpl_common_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/kpl/concept/kpl_concept_api.py` & `mns_common-1.0.9.3/mns_common/api/kpl/concept/kpl_concept_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/kpl/constant/kpl_constant.py` & `mns_common-1.0.9.3/mns_common/api/kpl/constant/kpl_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/kpl/industry/kpl_industry_api.py` & `mns_common-1.0.9.3/mns_common/api/kpl/industry/kpl_industry_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/kpl/selection/kpl_selection_plate_api.py` & `mns_common-1.0.9.3/mns_common/api/kpl/selection/kpl_selection_plate_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py` & `mns_common-1.0.9.3/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py` & `mns_common-1.0.9.3/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/kpl/symbol/symbol_his_quotes_api.py` & `mns_common-1.0.9.3/mns_common/api/kpl/symbol/symbol_his_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/msg/push_msg_api.py` & `mns_common-1.0.9.3/mns_common/api/msg/push_msg_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/ths/ths_big_deal_api.py` & `mns_common-1.0.9.3/mns_common/api/ths/ths_big_deal_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/api/ths/ths_stock_api.py` & `mns_common-1.0.9.3/mns_common/api/ths/ths_stock_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,14 +414,15 @@
             lambda x: pd.to_numeric(x.replace('亿', ''), errors="coerce"))
 
         return stock_board_cons_ths_df
         logger.info("同步概念代码数据:{}", code)
     except BaseException as e:
         logger.error("获取详情异常:{},异常信息:{}", code, e)
 
+
 # HK市场 https://basic.10jqka.com.cn/mobile/HK1456/profile.html  https://basic.10jqka.com.cn/mobile/HK1456/company.html
 # https://basic.10jqka.com.cn/astockph/briefinfo/index.html?showhead=0&fromshare=1&code=300430&marketid=33&client_userid=ESgcM&back_source=hyperlink&share_hxapp=isc&fontzoom=no#/company/ziliao
 def get_company_info_detail(symbol: str = "305794") -> pd.DataFrame:
     try:
         url = f'https://basic.10jqka.com.cn/basicapi/company_info/merge_info/v1/base_info/?code={symbol}&market=33&type=stock'
         headers = {
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:105.0) Gecko/20100101 Firefox/105.0',
@@ -835,14 +836,15 @@
                           "detail",
                           "market_code",
                           "concept_code"]
     return concept_df
 
 
 if __name__ == '__main__':
+    re = wei_cai_api('603619 支撑压力位', 'stock')
     df = get_symbol_add_new_concept('600128')
     print(df)
     # while True:
     #     concept_test()
     # company_info = get_concept_name('881121')
     # print(company_info)
     # new_concept_symbol_list = ths_stock_concept('881121')
```

### Comparing `mns_common-1.0.9.2/mns_common/api/ths/ths_stock_zt_pool_api.py` & `mns_common-1.0.9.3/mns_common/api/ths/ths_stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/component/cache/cache_service.py` & `mns_common-1.0.9.3/mns_common/component/cache/cache_service.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/component/classify/classify_constant.py` & `mns_common-1.0.9.3/mns_common/component/classify/classify_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/component/classify/symbol_classify_api.py` & `mns_common-1.0.9.3/mns_common/component/classify/symbol_classify_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/component/common_service_fun_api.py` & `mns_common-1.0.9.3/mns_common/component/common_service_fun_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/component/company/company_common_service_api.py` & `mns_common-1.0.9.3/mns_common/component/company/company_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/component/concept/kpl_concept_common_service_api.py` & `mns_common-1.0.9.3/mns_common/component/concept/kpl_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/component/concept/ths_concept_common_service_api.py` & `mns_common-1.0.9.3/mns_common/component/concept/ths_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/component/data/data_init_api.py` & `mns_common-1.0.9.3/mns_common/component/data/data_init_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/component/industry/ths_industry_index_api.py` & `mns_common-1.0.9.3/mns_common/component/industry/ths_industry_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py` & `mns_common-1.0.9.3/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/component/k_line/common/k_line_common_service_api.py` & `mns_common-1.0.9.3/mns_common/component/k_line/common/k_line_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/component/k_line/patterns/k_line_patterns_service_api.py` & `mns_common-1.0.9.3/mns_common/component/k_line/patterns/k_line_patterns_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/component/real_time/real_time_common_service_api.py` & `mns_common-1.0.9.3/mns_common/component/real_time/real_time_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/component/trade/trade_service_api.py` & `mns_common-1.0.9.3/mns_common/component/trade/trade_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/component/trade_date/trade_date_common_service_api.py` & `mns_common-1.0.9.3/mns_common/component/trade_date/trade_date_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/component/zt/zt_common_service_api.py` & `mns_common-1.0.9.3/mns_common/component/zt/zt_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/constant/db_name_constant.py` & `mns_common-1.0.9.3/mns_common/constant/db_name_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/constant/kpl_selection_no_choose_constant.py` & `mns_common-1.0.9.3/mns_common/constant/kpl_selection_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/constant/ths_concept_no_choose_constant.py` & `mns_common-1.0.9.3/mns_common/constant/ths_concept_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/db/MongodbUtil.py` & `mns_common-1.0.9.3/mns_common/db/MongodbUtil.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/utils/data_frame_util.py` & `mns_common-1.0.9.3/mns_common/utils/data_frame_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common/utils/date_handle_util.py` & `mns_common-1.0.9.3/mns_common/utils/date_handle_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.2/mns_common.egg-info/SOURCES.txt` & `mns_common-1.0.9.3/mns_common.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,16 @@
 mns_common/component/k_line/common/__init__.py
 mns_common/component/k_line/common/k_line_common_service_api.py
 mns_common/component/k_line/patterns/__init__.py
 mns_common/component/k_line/patterns/k_line_patterns_service_api.py
 mns_common/component/k_line/patterns/pattern_Enum.py
 mns_common/component/real_time/__init__.py
 mns_common/component/real_time/real_time_common_service_api.py
+mns_common/component/self_choose/__init__.py
+mns_common/component/self_choose/black_list_service_api.py
 mns_common/component/trade/__init__.py
 mns_common/component/trade/trade_service_api.py
 mns_common/component/trade_date/__init__.py
 mns_common/component/trade_date/trade_date_common_service_api.py
 mns_common/component/zt/__init__.py
 mns_common/component/zt/zt_common_service_api.py
 mns_common/constant/__init__.py
```


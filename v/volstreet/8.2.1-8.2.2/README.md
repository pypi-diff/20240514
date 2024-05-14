# Comparing `tmp/volstreet-8.2.1.tar.gz` & `tmp/volstreet-8.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-8.2.1.tar", last modified: Sun May 12 11:54:46 2024, max compression
+gzip compressed data, was "volstreet-8.2.2.tar", last modified: Tue May 14 03:35:42 2024, max compression
```

## Comparing `volstreet-8.2.1.tar` & `volstreet-8.2.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.062015 volstreet-8.2.1/
--rw-rw-rw-   0        0        0     1293 2024-05-12 11:54:46.062015 volstreet-8.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-8.2.1/README.md
--rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-8.2.1/pyproject.toml
--rw-rw-rw-   0        0        0     1155 2024-05-12 11:54:46.062015 volstreet-8.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-12 11:54:45.934477 volstreet-8.2.1/volstreet/
--rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-8.2.1/volstreet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:54:45.959890 volstreet-8.2.1/volstreet/angel_interface/
--rw-rw-rw-   0        0        0      247 2024-04-26 02:47:59.000000 volstreet-8.2.1/volstreet/angel_interface/__init__.py
--rw-rw-rw-   0        0        0     3726 2024-04-26 02:48:50.000000 volstreet-8.2.1/volstreet/angel_interface/access_rate_handler.py
--rw-rw-rw-   0        0        0      274 2024-04-23 04:22:25.000000 volstreet-8.2.1/volstreet/angel_interface/active_session.py
--rw-rw-rw-   0        0        0     3315 2024-05-06 03:22:49.000000 volstreet-8.2.1/volstreet/angel_interface/async_interface.py
--rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/angel_interface/base_websocket.py
--rw-rw-rw-   0        0        0    18658 2024-04-26 03:17:20.000000 volstreet-8.2.1/volstreet/angel_interface/interface.py
--rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-8.2.1/volstreet/angel_interface/login.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/angel_interface/order_websocket.py
--rw-rw-rw-   0        0        0    30773 2024-04-29 09:17:58.000000 volstreet-8.2.1/volstreet/angel_interface/price_websocket.py
--rw-rw-rw-   0        0        0     6687 2024-04-26 02:56:08.000000 volstreet-8.2.1/volstreet/angel_interface/smart_connect.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:54:45.991426 volstreet-8.2.1/volstreet/backtests/
--rw-rw-rw-   0        0        0      290 2024-04-28 14:01:14.000000 volstreet-8.2.1/volstreet/backtests/__init__.py
--rw-rw-rw-   0        0        0     4064 2024-04-23 04:22:25.000000 volstreet-8.2.1/volstreet/backtests/analysis.py
--rw-rw-rw-   0        0        0     4181 2024-05-04 08:33:34.000000 volstreet-8.2.1/volstreet/backtests/data_updation.py
--rw-rw-rw-   0        0        0    11857 2024-04-25 10:13:39.000000 volstreet-8.2.1/volstreet/backtests/database.py
--rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-8.2.1/volstreet/backtests/delta_hedging.py
--rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/backtests/delta_optimizer.py
--rw-rw-rw-   0        0        0    48672 2024-05-02 12:46:20.000000 volstreet-8.2.1/volstreet/backtests/framework.py
--rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-8.2.1/volstreet/backtests/intraday_backtest_abc.py
--rw-rw-rw-   0        0        0     7201 2024-05-05 08:31:29.000000 volstreet-8.2.1/volstreet/backtests/proxy_functions.py
--rw-rw-rw-   0        0        0     2707 2024-04-24 14:17:18.000000 volstreet-8.2.1/volstreet/backtests/result_processing.py
--rw-rw-rw-   0        0        0     6184 2024-05-09 04:00:00.000000 volstreet-8.2.1/volstreet/backtests/runner.py
--rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-8.2.1/volstreet/backtests/tools.py
--rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-8.2.1/volstreet/backtests/trend.py
--rw-rw-rw-   0        0        0     1941 2024-05-09 03:54:28.000000 volstreet-8.2.1/volstreet/backtests/underlying_info.py
--rw-rw-rw-   0        0        0    20882 2024-05-02 08:25:42.000000 volstreet-8.2.1/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     5574 2024-04-24 06:53:53.000000 volstreet-8.2.1/volstreet/config.py
--rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/database_connection.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.007459 volstreet-8.2.1/volstreet/datamodule/
--rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-8.2.1/volstreet/datamodule/__init__.py
--rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/datamodule/analysis.py
--rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/datamodule/archive.py
--rw-rw-rw-   0        0        0     9786 2024-05-09 13:39:03.000000 volstreet-8.2.1/volstreet/datamodule/data_handling.py
--rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/datamodule/eod_client.py
--rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/datamodule/gambling.py
--rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/datamodule/intraday_data.py
--rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-8.2.1/volstreet/datamodule/stockmock.py
--rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/datamodule/trading_assistance.py
--rw-rw-rw-   0        0        0    25622 2024-05-06 02:53:39.000000 volstreet-8.2.1/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-8.2.1/volstreet/decorators.py
--rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.007459 volstreet-8.2.1/volstreet/historical_info/
--rw-rw-rw-   0        0        0      975 2024-04-24 06:53:53.000000 volstreet-8.2.1/volstreet/historical_info/__init__.py
--rw-rw-rw-   0        0        0    21031 2024-05-04 08:38:02.000000 volstreet-8.2.1/volstreet/historical_info/index_expiries.pkl
--rw-rw-rw-   0        0        0    16975 2024-05-11 04:49:24.000000 volstreet-8.2.1/volstreet/historical_info/market_days.pkl
-drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.007459 volstreet-8.2.1/volstreet/models/
--rw-rw-rw-   0        0        0      568 2024-04-29 10:45:14.000000 volstreet-8.2.1/volstreet/models/__init__.py
--rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/parallelization.py
--rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-8.2.1/volstreet/performance_tracking.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.007459 volstreet-8.2.1/volstreet/position_dashboard/
--rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-8.2.1/volstreet/position_dashboard/__init__.py
--rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-8.2.1/volstreet/position_dashboard/app.py
--rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-8.2.1/volstreet/position_dashboard/formatting.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.023094 volstreet-8.2.1/volstreet/strategies/
--rw-rw-rw-   0        0        0      183 2024-05-03 07:00:07.000000 volstreet-8.2.1/volstreet/strategies/__init__.py
--rw-rw-rw-   0        0        0    32426 2024-05-06 02:53:39.000000 volstreet-8.2.1/volstreet/strategies/deployment.py
--rw-rw-rw-   0        0        0     1925 2024-05-03 06:56:48.000000 volstreet-8.2.1/volstreet/strategies/error_handling.py
--rw-rw-rw-   0        0        0    56751 2024-05-10 10:17:25.000000 volstreet-8.2.1/volstreet/strategies/helpers.py
--rw-rw-rw-   0        0        0     6352 2024-05-03 06:56:48.000000 volstreet-8.2.1/volstreet/strategies/monitoring.py
--rw-rw-rw-   0        0        0    18535 2024-05-02 10:20:37.000000 volstreet-8.2.1/volstreet/strategies/optimization.py
--rw-rw-rw-   0        0        0   106164 2024-05-10 03:43:38.000000 volstreet-8.2.1/volstreet/strategies/strats.py
--rw-rw-rw-   0        0        0      349 2024-04-12 11:13:05.000000 volstreet-8.2.1/volstreet/strategies/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.023094 volstreet-8.2.1/volstreet/trade_interface/
--rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-8.2.1/volstreet/trade_interface/__init__.py
--rw-rw-rw-   0        0        0    26799 2024-04-23 04:22:25.000000 volstreet-8.2.1/volstreet/trade_interface/instruments.py
--rw-rw-rw-   0        0        0    19389 2024-04-29 10:19:25.000000 volstreet-8.2.1/volstreet/trade_interface/order_execution.py
--rw-rw-rw-   0        0        0    20204 2024-05-05 08:31:29.000000 volstreet-8.2.1/volstreet/trade_interface/underlyings.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.040254 volstreet-8.2.1/volstreet/utils/
--rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/utils/__init__.py
--rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/utils/change_config.py
--rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-8.2.1/volstreet/utils/communication.py
--rw-rw-rw-   0        0        0    14475 2024-05-03 08:15:05.000000 volstreet-8.2.1/volstreet/utils/core.py
--rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/utils/data_io.py
--rw-rw-rw-   0        0        0     9915 2024-04-26 13:19:30.000000 volstreet-8.2.1/volstreet/utils/scrip_processing.py
--rw-rw-rw-   0        0        0     6488 2024-04-23 04:22:25.000000 volstreet-8.2.1/volstreet/vectorized_blackscholes.py
--rw-rw-rw-   0        0        0       20 2024-05-11 04:46:04.000000 volstreet-8.2.1/volstreet/volstreet_mode.json
-drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.054761 volstreet-8.2.1/volstreet/vslogging/
--rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-8.2.1/volstreet/vslogging/__init__.py
--rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-8.2.1/volstreet/vslogging/formatters.py
--rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-8.2.1/volstreet/vslogging/logging_config.json
--rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-8.2.1/volstreet/vslogging/logging_setup.py
--rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-8.2.1/volstreet/vslogging/parsing.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.054761 volstreet-8.2.1/volstreet.egg-info/
--rw-rw-rw-   0        0        0     1293 2024-05-12 11:54:45.000000 volstreet-8.2.1/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2833 2024-05-12 11:54:45.000000 volstreet-8.2.1/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 11:54:45.000000 volstreet-8.2.1/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      460 2024-05-12 11:54:45.000000 volstreet-8.2.1/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-12 11:54:45.000000 volstreet-8.2.1/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 03:35:42.697797 volstreet-8.2.2/
+-rw-rw-rw-   0        0        0     1293 2024-05-14 03:35:42.697797 volstreet-8.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-8.2.2/README.md
+-rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-8.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1155 2024-05-14 03:35:42.697797 volstreet-8.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 03:35:42.568164 volstreet-8.2.2/volstreet/
+-rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-8.2.2/volstreet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:35:42.594350 volstreet-8.2.2/volstreet/angel_interface/
+-rw-rw-rw-   0        0        0      247 2024-04-26 02:47:59.000000 volstreet-8.2.2/volstreet/angel_interface/__init__.py
+-rw-rw-rw-   0        0        0     3726 2024-04-26 02:48:50.000000 volstreet-8.2.2/volstreet/angel_interface/access_rate_handler.py
+-rw-rw-rw-   0        0        0      274 2024-04-23 04:22:25.000000 volstreet-8.2.2/volstreet/angel_interface/active_session.py
+-rw-rw-rw-   0        0        0     3315 2024-05-06 03:22:49.000000 volstreet-8.2.2/volstreet/angel_interface/async_interface.py
+-rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-8.2.2/volstreet/angel_interface/base_websocket.py
+-rw-rw-rw-   0        0        0    18658 2024-04-26 03:17:20.000000 volstreet-8.2.2/volstreet/angel_interface/interface.py
+-rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-8.2.2/volstreet/angel_interface/login.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-8.2.2/volstreet/angel_interface/order_websocket.py
+-rw-rw-rw-   0        0        0    30773 2024-04-29 09:17:58.000000 volstreet-8.2.2/volstreet/angel_interface/price_websocket.py
+-rw-rw-rw-   0        0        0     6687 2024-04-26 02:56:08.000000 volstreet-8.2.2/volstreet/angel_interface/smart_connect.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:35:42.626536 volstreet-8.2.2/volstreet/backtests/
+-rw-rw-rw-   0        0        0      290 2024-04-28 14:01:14.000000 volstreet-8.2.2/volstreet/backtests/__init__.py
+-rw-rw-rw-   0        0        0     4064 2024-04-23 04:22:25.000000 volstreet-8.2.2/volstreet/backtests/analysis.py
+-rw-rw-rw-   0        0        0     4181 2024-05-04 08:33:34.000000 volstreet-8.2.2/volstreet/backtests/data_updation.py
+-rw-rw-rw-   0        0        0    11857 2024-04-25 10:13:39.000000 volstreet-8.2.2/volstreet/backtests/database.py
+-rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-8.2.2/volstreet/backtests/delta_hedging.py
+-rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-8.2.2/volstreet/backtests/delta_optimizer.py
+-rw-rw-rw-   0        0        0    48672 2024-05-02 12:46:20.000000 volstreet-8.2.2/volstreet/backtests/framework.py
+-rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-8.2.2/volstreet/backtests/intraday_backtest_abc.py
+-rw-rw-rw-   0        0        0     7375 2024-05-13 11:20:24.000000 volstreet-8.2.2/volstreet/backtests/proxy_functions.py
+-rw-rw-rw-   0        0        0     2707 2024-04-24 14:17:18.000000 volstreet-8.2.2/volstreet/backtests/result_processing.py
+-rw-rw-rw-   0        0        0     6184 2024-05-09 04:00:00.000000 volstreet-8.2.2/volstreet/backtests/runner.py
+-rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-8.2.2/volstreet/backtests/tools.py
+-rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-8.2.2/volstreet/backtests/trend.py
+-rw-rw-rw-   0        0        0     1924 2024-05-13 10:36:16.000000 volstreet-8.2.2/volstreet/backtests/underlying_info.py
+-rw-rw-rw-   0        0        0    20882 2024-05-02 08:25:42.000000 volstreet-8.2.2/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     5574 2024-04-24 06:53:53.000000 volstreet-8.2.2/volstreet/config.py
+-rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-8.2.2/volstreet/database_connection.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:35:42.644531 volstreet-8.2.2/volstreet/datamodule/
+-rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-8.2.2/volstreet/datamodule/__init__.py
+-rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-8.2.2/volstreet/datamodule/analysis.py
+-rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-8.2.2/volstreet/datamodule/archive.py
+-rw-rw-rw-   0        0        0     9786 2024-05-09 13:39:03.000000 volstreet-8.2.2/volstreet/datamodule/data_handling.py
+-rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-8.2.2/volstreet/datamodule/eod_client.py
+-rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-8.2.2/volstreet/datamodule/gambling.py
+-rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-8.2.2/volstreet/datamodule/intraday_data.py
+-rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-8.2.2/volstreet/datamodule/stockmock.py
+-rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-8.2.2/volstreet/datamodule/trading_assistance.py
+-rw-rw-rw-   0        0        0    25622 2024-05-06 02:53:39.000000 volstreet-8.2.2/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-8.2.2/volstreet/decorators.py
+-rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-8.2.2/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-8.2.2/volstreet/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:35:42.644531 volstreet-8.2.2/volstreet/historical_info/
+-rw-rw-rw-   0        0        0      975 2024-04-24 06:53:53.000000 volstreet-8.2.2/volstreet/historical_info/__init__.py
+-rw-rw-rw-   0        0        0    21031 2024-05-04 08:38:02.000000 volstreet-8.2.2/volstreet/historical_info/index_expiries.pkl
+-rw-rw-rw-   0        0        0    16988 2024-05-13 13:24:43.000000 volstreet-8.2.2/volstreet/historical_info/market_days.pkl
+drwxrwxrwx   0        0        0        0 2024-05-14 03:35:42.644531 volstreet-8.2.2/volstreet/models/
+-rw-rw-rw-   0        0        0      568 2024-04-29 10:45:14.000000 volstreet-8.2.2/volstreet/models/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-8.2.2/volstreet/parallelization.py
+-rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-8.2.2/volstreet/performance_tracking.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:35:42.654370 volstreet-8.2.2/volstreet/position_dashboard/
+-rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-8.2.2/volstreet/position_dashboard/__init__.py
+-rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-8.2.2/volstreet/position_dashboard/app.py
+-rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-8.2.2/volstreet/position_dashboard/formatting.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:35:42.664399 volstreet-8.2.2/volstreet/strategies/
+-rw-rw-rw-   0        0        0      183 2024-05-03 07:00:07.000000 volstreet-8.2.2/volstreet/strategies/__init__.py
+-rw-rw-rw-   0        0        0    32426 2024-05-06 02:53:39.000000 volstreet-8.2.2/volstreet/strategies/deployment.py
+-rw-rw-rw-   0        0        0     1925 2024-05-03 06:56:48.000000 volstreet-8.2.2/volstreet/strategies/error_handling.py
+-rw-rw-rw-   0        0        0    56751 2024-05-10 10:17:25.000000 volstreet-8.2.2/volstreet/strategies/helpers.py
+-rw-rw-rw-   0        0        0     6352 2024-05-03 06:56:48.000000 volstreet-8.2.2/volstreet/strategies/monitoring.py
+-rw-rw-rw-   0        0        0    18535 2024-05-02 10:20:37.000000 volstreet-8.2.2/volstreet/strategies/optimization.py
+-rw-rw-rw-   0        0        0   103414 2024-05-13 12:05:10.000000 volstreet-8.2.2/volstreet/strategies/strats.py
+-rw-rw-rw-   0        0        0     1251 2024-05-13 11:12:56.000000 volstreet-8.2.2/volstreet/strategies/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:35:42.674205 volstreet-8.2.2/volstreet/trade_interface/
+-rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-8.2.2/volstreet/trade_interface/__init__.py
+-rw-rw-rw-   0        0        0    26799 2024-04-23 04:22:25.000000 volstreet-8.2.2/volstreet/trade_interface/instruments.py
+-rw-rw-rw-   0        0        0    19389 2024-05-13 11:08:46.000000 volstreet-8.2.2/volstreet/trade_interface/order_execution.py
+-rw-rw-rw-   0        0        0    20204 2024-05-05 08:31:29.000000 volstreet-8.2.2/volstreet/trade_interface/underlyings.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:35:42.686542 volstreet-8.2.2/volstreet/utils/
+-rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-8.2.2/volstreet/utils/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-8.2.2/volstreet/utils/change_config.py
+-rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-8.2.2/volstreet/utils/communication.py
+-rw-rw-rw-   0        0        0    14475 2024-05-03 08:15:05.000000 volstreet-8.2.2/volstreet/utils/core.py
+-rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-8.2.2/volstreet/utils/data_io.py
+-rw-rw-rw-   0        0        0     9915 2024-04-26 13:19:30.000000 volstreet-8.2.2/volstreet/utils/scrip_processing.py
+-rw-rw-rw-   0        0        0     6488 2024-04-23 04:22:25.000000 volstreet-8.2.2/volstreet/vectorized_blackscholes.py
+-rw-rw-rw-   0        0        0       20 2024-05-13 13:37:06.000000 volstreet-8.2.2/volstreet/volstreet_mode.json
+drwxrwxrwx   0        0        0        0 2024-05-14 03:35:42.694475 volstreet-8.2.2/volstreet/vslogging/
+-rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-8.2.2/volstreet/vslogging/__init__.py
+-rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-8.2.2/volstreet/vslogging/formatters.py
+-rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-8.2.2/volstreet/vslogging/logging_config.json
+-rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-8.2.2/volstreet/vslogging/logging_setup.py
+-rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-8.2.2/volstreet/vslogging/parsing.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:35:42.694475 volstreet-8.2.2/volstreet.egg-info/
+-rw-rw-rw-   0        0        0     1293 2024-05-14 03:35:42.000000 volstreet-8.2.2/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2833 2024-05-14 03:35:42.000000 volstreet-8.2.2/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 03:35:42.000000 volstreet-8.2.2/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      460 2024-05-14 03:35:42.000000 volstreet-8.2.2/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-14 03:35:42.000000 volstreet-8.2.2/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-8.2.1/PKG-INFO` & `volstreet-8.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 8.2.1
+Version: 8.2.2
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-8.2.1/setup.cfg` & `volstreet-8.2.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 382e 322e 310d 0a61  rsion = 8.2.1..a
+00000020: 7273 696f 6e20 3d20 382e 322e 320d 0a61  rsion = 8.2.2..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-8.2.1/volstreet/angel_interface/access_rate_handler.py` & `volstreet-8.2.2/volstreet/angel_interface/access_rate_handler.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/angel_interface/async_interface.py` & `volstreet-8.2.2/volstreet/angel_interface/async_interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/angel_interface/base_websocket.py` & `volstreet-8.2.2/volstreet/angel_interface/base_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/angel_interface/interface.py` & `volstreet-8.2.2/volstreet/angel_interface/interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/angel_interface/login.py` & `volstreet-8.2.2/volstreet/angel_interface/login.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/angel_interface/order_websocket.py` & `volstreet-8.2.2/volstreet/angel_interface/order_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/angel_interface/price_websocket.py` & `volstreet-8.2.2/volstreet/angel_interface/price_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/angel_interface/smart_connect.py` & `volstreet-8.2.2/volstreet/angel_interface/smart_connect.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/backtests/analysis.py` & `volstreet-8.2.2/volstreet/backtests/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/backtests/data_updation.py` & `volstreet-8.2.2/volstreet/backtests/data_updation.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/backtests/database.py` & `volstreet-8.2.2/volstreet/backtests/database.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/backtests/delta_hedging.py` & `volstreet-8.2.2/volstreet/backtests/delta_hedging.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/backtests/delta_optimizer.py` & `volstreet-8.2.2/volstreet/backtests/delta_optimizer.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/backtests/framework.py` & `volstreet-8.2.2/volstreet/backtests/framework.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/backtests/intraday_backtest_abc.py` & `volstreet-8.2.2/volstreet/backtests/intraday_backtest_abc.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/backtests/proxy_functions.py` & `volstreet-8.2.2/volstreet/backtests/proxy_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -152,25 +152,30 @@
     }
     return order_details
 
 
 def execute_instructions(instructions: dict, *args, **kwargs):
     orders = []
     for instrument, params in instructions.items():
+        filtered_params = {
+            k: v for k, v in params.items() if k in ["action", "quantity_in_lots"]
+        }
         if hasattr(instrument, "call_token") and hasattr(instrument, "put_token"):
             call_price = ProxyFeeds.price_feed.data_bank[instrument.call_token]["ltp"]
             put_price = ProxyFeeds.price_feed.data_bank[instrument.put_token]["ltp"]
             orders.extend(
                 instrument.generate_order_params(
-                    **params, price=(call_price, put_price)
+                    **filtered_params, price=(call_price, put_price)
                 )
             )
         else:
             price = ProxyFeeds.price_feed.data_bank[instrument.token]["ltp"]
-            orders.extend(instrument.generate_order_params(**params, price=price))
+            orders.extend(
+                instrument.generate_order_params(**filtered_params, price=price)
+            )
     orders = [simulate_execution(order) for order in orders]
     ProxyFeeds.order_feed.extend(orders)
     average_prices = {order["token"]: order["price"] for order in orders}
     return identify_average_prices(instructions, average_prices)
 
 
 def sleep_until_next_action(
```

### Comparing `volstreet-8.2.1/volstreet/backtests/result_processing.py` & `volstreet-8.2.2/volstreet/backtests/result_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/backtests/runner.py` & `volstreet-8.2.2/volstreet/backtests/runner.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/backtests/tools.py` & `volstreet-8.2.2/volstreet/backtests/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/backtests/trend.py` & `volstreet-8.2.2/volstreet/backtests/trend.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/backtests/underlying_info.py` & `volstreet-8.2.2/volstreet/backtests/underlying_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     if isinstance(date_time, str):
         date_time = pd.to_datetime(date_time)
 
     filtered_dates = filter_expiry_dates_for_index(underlying)
     filtered_dates = filtered_dates.sort_values()
     delta_days = (filtered_dates - date_time.replace(hour=00, minute=00)).days
     filtered_dates = filtered_dates[delta_days >= threshold_days]
-    nearest_exp_dates = sorted(filtered_dates)
+    nearest_exp_dates = [*sorted(filtered_dates)]
     if n_exp == 1:
         return nearest_exp_dates[0] if len(nearest_exp_dates) != 0 else None
     if len(nearest_exp_dates) < n_exp:
         logger.warning(f"Insufficient expiry dates for {underlying} on {date_time}")
         while len(nearest_exp_dates) < n_exp:
-            nearest_exp_dates = nearest_exp_dates.append(np.nan)
+            nearest_exp_dates.append(np.nan)
     return pd.DatetimeIndex(nearest_exp_dates[:n_exp])
```

### Comparing `volstreet-8.2.1/volstreet/blackscholes.py` & `volstreet-8.2.2/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/config.py` & `volstreet-8.2.2/volstreet/config.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/database_connection.py` & `volstreet-8.2.2/volstreet/database_connection.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/datamodule/analysis.py` & `volstreet-8.2.2/volstreet/datamodule/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/datamodule/archive.py` & `volstreet-8.2.2/volstreet/datamodule/archive.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/datamodule/data_handling.py` & `volstreet-8.2.2/volstreet/datamodule/data_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/datamodule/eod_client.py` & `volstreet-8.2.2/volstreet/datamodule/eod_client.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/datamodule/gambling.py` & `volstreet-8.2.2/volstreet/datamodule/gambling.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/datamodule/intraday_data.py` & `volstreet-8.2.2/volstreet/datamodule/intraday_data.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/datamodule/stockmock.py` & `volstreet-8.2.2/volstreet/datamodule/stockmock.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/datamodule/trading_assistance.py` & `volstreet-8.2.2/volstreet/datamodule/trading_assistance.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/dealingroom.py` & `volstreet-8.2.2/volstreet/dealingroom.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/decorators.py` & `volstreet-8.2.2/volstreet/decorators.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/discord_bot.py` & `volstreet-8.2.2/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/exceptions.py` & `volstreet-8.2.2/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/historical_info/__init__.py` & `volstreet-8.2.2/volstreet/historical_info/__init__.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/historical_info/index_expiries.pkl` & `volstreet-8.2.2/volstreet/historical_info/index_expiries.pkl`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/historical_info/market_days.pkl` & `volstreet-8.2.2/volstreet/historical_info/market_days.pkl`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 9544 4200 0000 0000 005d 9428 8c08  ...DB......].(..
+00000000: 8004 9551 4200 0000 0000 005d 9428 8c08  ...QB......].(..
 00000010: 6461 7465 7469 6d65 948c 0464 6174 6594  datetime...date.
 00000020: 9394 4304 07e3 0201 9485 9452 9468 0343  ..C........R.h.C
 00000030: 0407 e302 0494 8594 5294 6803 4304 07e3  ........R.h.C...
 00000040: 0205 9485 9452 9468 0343 0407 e302 0694  .....R.h.C......
 00000050: 8594 5294 6803 4304 07e3 0207 9485 9452  ..R.h.C........R
 00000060: 9468 0343 0407 e302 0894 8594 5294 6803  .h.C........R.h.
 00000070: 4304 07e3 020b 9485 9452 9468 0343 0407  C........R.h.C..
@@ -1054,8 +1054,9 @@
 000041d0: e804 1a94 8594 5294 6803 4304 07e8 041d  ......R.h.C.....
 000041e0: 9485 9452 9468 0343 0407 e804 1e94 8594  ...R.h.C........
 000041f0: 5294 6803 4304 07e8 0502 9485 9452 9468  R.h.C........R.h
 00004200: 0343 0407 e805 0394 8594 5294 6803 4304  .C........R.h.C.
 00004210: 07e8 0506 9485 9452 9468 0343 0407 e805  .......R.h.C....
 00004220: 0794 8594 5294 6803 4304 07e8 0508 9485  ....R.h.C.......
 00004230: 9452 9468 0343 0407 e805 0994 8594 5294  .R.h.C........R.
-00004240: 6803 4304 07e8 050a 9485 9452 9465 2e    h.C........R.e.
+00004240: 6803 4304 07e8 050a 9485 9452 9468 0343  h.C........R.h.C
+00004250: 0407 e805 0d94 8594 5294 652e            ........R.e.
```

### Comparing `volstreet-8.2.1/volstreet/models/__init__.py` & `volstreet-8.2.2/volstreet/models/__init__.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/parallelization.py` & `volstreet-8.2.2/volstreet/parallelization.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/performance_tracking.py` & `volstreet-8.2.2/volstreet/performance_tracking.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/position_dashboard/app.py` & `volstreet-8.2.2/volstreet/position_dashboard/app.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/position_dashboard/formatting.py` & `volstreet-8.2.2/volstreet/position_dashboard/formatting.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/strategies/deployment.py` & `volstreet-8.2.2/volstreet/strategies/deployment.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/strategies/error_handling.py` & `volstreet-8.2.2/volstreet/strategies/error_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/strategies/helpers.py` & `volstreet-8.2.2/volstreet/strategies/helpers.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/strategies/monitoring.py` & `volstreet-8.2.2/volstreet/strategies/monitoring.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/strategies/optimization.py` & `volstreet-8.2.2/volstreet/strategies/optimization.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/strategies/strats.py` & `volstreet-8.2.2/volstreet/strategies/strats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import os
 import numpy as np
-from datetime import datetime, timedelta, time
-from threading import Thread
 from time import sleep
 from typing import Optional
-import os
 from volstreet import config
+from threading import Thread
+from functools import partial
+from datetime import datetime, timedelta, time
 from volstreet.config import logger
 from volstreet.utils.core import (
     current_time,
     find_strike,
     time_to_expiry,
     check_for_weekend,
     calculate_ema,
@@ -49,14 +50,15 @@
     TrendPosition,
     PositionMonitor,
     load_current_strangle,
     approve_execution,
     notify_pnl,
     process_stop_loss_order_statuses,
 )
+from volstreet.strategies.tools import execute_single_instrument
 from volstreet.strategies.error_handling import exit_on_error
 
 if config.backtest_mode:
     logger.info(
         f"Importing proxy functions in module: {__name__} since backtesting is enabled."
     )
     from volstreet.backtests.proxy_functions import (
@@ -902,17 +904,14 @@
     combined_stop_loss: Optional[float] = None,
     exit_time: tuple[int, int] = (15, 29),
     sleep_time: Optional[int] = 5,
     seconds_to_avg: Optional[int] = 30,
     simulation_safe_guard: Optional[float] = 1.15,
     catch_trend: Optional[bool] = False,
     trend_qty_ratio: Optional[float] = 1,
-    trend_strike_offset: Optional[float] = 0,
-    trend_sl: Optional[float] = 0.003,
-    trend_sl_on_option: Optional[bool] = 1.75,
     disparity_threshold: Optional[float] = 1000,
     place_sl_orders: Optional[bool] = False,
     move_sl_to_cost: Optional[bool] = False,
     place_orders_on_sl: Optional[bool] = False,
     convert_to_butterfly: Optional[bool] = False,
     conversion_method: Optional[str] = "pct",
     conversion_threshold_pct: Optional[float] = 0.175,
@@ -949,20 +948,14 @@
         Seconds to average prices over, by default 30
     simulation_safe_guard : float, optional
         The multiple over the simulated price that will reject stop loss, by default 1.15
     catch_trend : bool, optional
         Catch trend or not, by default False
     trend_qty_ratio : int, optional
         Ratio of trend quantity to strangle quantity, by default 1
-    trend_strike_offset : float, optional
-        Strike offset for trend order in percentage terms, by default 0
-    trend_sl : float, optional
-        Stop loss for trend order, by default 0.003
-    trend_sl_on_option : bool, optional
-        Place stop loss on option, by default 1.75.
     disparity_threshold : float, optional
         Disparity threshold for equality of strikes, by default np.inf
     place_sl_orders : bool, optional
         Place stop loss orders or not, by default False
     move_sl_to_cost : bool, optional
         Move other stop loss to cost or not, by default False
     place_orders_on_sl : bool, optional
@@ -1176,83 +1169,81 @@
             if current_time() - last_notify_time > notify_interval:
                 notifier(message, notification_url, "INFO")
                 last_notify_time = current_time()
             sleep(sleep_time)
 
     @log_error(raise_error=True, notify=True)
     @increase_robustness
-    def trend_catcher(info_dict, sl_type, qty_ratio, sl, strike_offset):
-        offset = 1 - strike_offset if sl_type == "call" else 1 + strike_offset
+    def trend_catcher(info_dict, sl_type, qty_ratio):
+
+        def check_trade_eligibility(option, price):
+            if option.fetch_ltp() > price * 0.70:
+                return True
 
-        spot_price = info_dict["underlying_ltp"]
+        traded_strangle = info_dict["traded_strangle"]
+        og_price = (
+            info_dict["call_avg_price"]
+            if sl_type == "put"
+            else info_dict["put_avg_price"]
+        )
+        trend_option = (
+            traded_strangle.call_option
+            if sl_type == "put"
+            else traded_strangle.put_option
+        )
 
-        # Setting up the trend option
-        strike = spot_price * offset
-        strike = find_strike(strike, underlying.base)
-        opt_type = OptionType.PUT if sl_type == "call" else OptionType.CALL
         qty_in_lots = max(int(quantity_in_lots * qty_ratio), 1)
-        trend_option = Option(strike, opt_type, underlying.name, expiry)
+
+        while not check_trade_eligibility(
+            trend_option, og_price
+        ) and current_time().time() < time(*exit_time):
+            logger.info(f"Waiting for trend option to reach 70% of original price")
+            sleep(sleep_time)
 
         # Placing the trend option order
         exec_details = execute_instructions(
             {
                 trend_option: {
                     "action": Action.SELL,
                     "quantity_in_lots": qty_in_lots,
                     "order_tag": f"{strategy_tag} Trend Catcher",
                 }
             }
         )
         sell_avg_price = exec_details[trend_option]
 
-        # Setting up the stop losses on underlying and trend option
-
-        # Underlying stop loss
-        sl_multiplier = 1 - sl if sl_type == "call" else 1 + sl
-        underlying_sl_price = spot_price * sl_multiplier
-
-        # Trend option stop loss
-        option_sl_price = sell_avg_price * trend_sl_on_option
+        # Setting up the stop loss on the trend option
 
         trend_sl_hit = False
         notifier(
             f"{underlying.name} strangle {sl_type} trend catcher starting. "
-            f"Placed {qty_in_lots} lots of {strike} {opt_type.value} at {sell_avg_price}. "
-            f"Stoploss prices: {underlying_sl_price, option_sl_price}. "
-            f"Underlying Price: {spot_price}",
+            f"Placed {qty_in_lots} lots of {trend_option} at {sell_avg_price}. "
+            f"Stoploss prices: {og_price}",
             notification_url,
             "INFO",
         )
 
         last_print_time = current_time()
         print_interval = timedelta(seconds=10)
         while all(
             [
                 current_time().time() < time(*exit_time),
                 not info_dict["trade_complete"],
             ]
         ):
-            spot_price = info_dict["underlying_ltp"]
-            spot_price_avg = info_dict["underlying_ltp_avg"]
             option_price = trend_option.fetch_ltp()
-            trend_sl_hit = (option_price > option_sl_price) and (
-                spot_price_avg < underlying_sl_price
-                if sl_type == "call"
-                else spot_price_avg > underlying_sl_price
-            )
+            trend_sl_hit = option_price >= og_price
             if trend_sl_hit:
                 break
             sleep(sleep_time)
             if current_time() - last_print_time > print_interval:
                 last_print_time = current_time()
                 logger.info(
                     f"{underlying.name} {sl_type} trend catcher running\n"
-                    f"Stoploss prices: {underlying_sl_price, option_sl_price}\n"
-                    f"Underlying price: {spot_price}\n"
-                    f"Underlying price avg: {spot_price_avg}, Stoploss hit: {trend_sl_hit}\n"
+                    f"Stoploss price: {og_price}\n"
                 )
 
         if trend_sl_hit:
             notifier(
                 f"{underlying.name} strangle {sl_type} trend catcher stoploss hit.",
                 notification_url,
                 "INFO",
@@ -1465,16 +1456,14 @@
         if catch_trend:
             trend_thread = Thread(
                 target=trend_catcher,
                 args=(
                     info_dict,
                     sl_type,
                     trend_qty_ratio,
-                    trend_sl,
-                    trend_strike_offset,
                 ),
                 name=f"{underlying.name} {sl_type} trend catcher",
             )
             trend_thread.start()
             info_dict["active_threads"].append(trend_thread)
 
         sleep(5)  # To ensure that the stop loss orders are reflected in the orderbook
@@ -2589,46 +2578,23 @@
     stop_loss: Optional[float] = 0.5,
     at_market: bool = False,
     notification_url: Optional[str] = None,
     strategy_tag: Optional[str] = "Reentry_straddle",
     data_directory: Optional[str] = None,
 ):
 
-    def exit_option(option: Option, quantity_in_lots: int):
-        instructions = {
-            option: {
-                "action": Action.BUY,
-                "quantity_in_lots": quantity_in_lots,
-                "order_tag": strategy_tag,
-            }
-        }
-        execution_details = execute_instructions(instructions, at_market=at_market)
-        option_exit_price = execution_details[option]
-        return option_exit_price
-
-    def reenter_option(option: Option, quantity_in_lots: int):
-        instructions = {
-            option: {
-                "action": Action.SELL,
-                "quantity_in_lots": quantity_in_lots,
-                "order_tag": strategy_tag,
-            }
-        }
-        execution_details = execute_instructions(instructions, at_market=at_market)
-        option_entry_price = execution_details[option]
-        return option_entry_price
-
     if time(*exit_time) < current_time().time():
         notifier(
             f"{underlying.name} {strategy_tag} not being deployed after exit time",
             notification_url,
             "INFO",
         )
         return
 
+    start_time = current_time()
     spot_price = underlying.fetch_ltp()
     expiry = underlying.current_expiry
     above_info, below_info = get_above_below_strangles_with_prices(
         underlying,
         spot_price,
         expiry,
     )
@@ -2636,128 +2602,109 @@
         above_info, below_info, key=lambda info: disparity_calculator(*info[1])
     )
 
     quantity_in_lots = convert_exposure_to_lots(
         exposure, spot_price, underlying.lot_size
     )
 
+    execute_order = partial(
+        execute_single_instrument,
+        at_market=at_market,
+        order_tag=strategy_tag,
+        quantity_in_lots=quantity_in_lots,
+    )
+
     notifier(
         f"{underlying.name} {strategy_tag} starting with straddle {straddle} and prices {prices}",
         notification_url,
         "INFO",
     )
 
     # Placing the main order
-    execution_details = execute_instructions(
-        {
-            straddle: {
-                "action": Action.SELL,
-                "quantity_in_lots": quantity_in_lots,
-                "order_tag": strategy_tag,
-            }
-        },
-        at_market=at_market,
+    call_avg_price, put_avg_price = execute_order(
+        instrument=straddle, action=Action.SELL
     )
-    call_avg_price, put_avg_price = execution_details[straddle]
-    total_avg_price = call_avg_price + put_avg_price
     call_sl_price = call_avg_price * (1 + stop_loss)
     put_sl_price = put_avg_price * (1 + stop_loss)
 
-    neutral = True
-    call_sl_hit = False
-    put_sl_hit = False
-    trend_sl_hit = False
-
-    reattempt_bank = {straddle.call_option: 1, straddle.put_option: 1}
+    # A tuple of (in_trade, reattempts)
+    status_dict = {straddle.call_option: (True, 1), straddle.put_option: (True, 1)}
 
-    while current_time().time() < time(*exit_time):
-        sleep_until_next_action(1, exit_time)
-        if neutral:
-            call_ltp, put_ltp = straddle.fetch_ltp()
-            call_sl_hit = call_ltp > call_sl_price
-            put_sl_hit = put_ltp > put_sl_price
-            if call_sl_hit and put_sl_hit:
-                raise ValueError("Both stop losses hit for some reason")
-            elif call_sl_hit or put_sl_hit:
-                notifier(
-                    f"{underlying.name} {strategy_tag} stop loss hit. "
-                    f"Call SL: {call_sl_hit}, Put SL: {put_sl_hit}. "
-                    f"State changed to directional.",
-                    notification_url,
-                    "CRUCIAL",
-                )
-                option_to_exit = (
-                    straddle.call_option if call_sl_hit else straddle.put_option
-                )
-                option_exit_price = exit_option(option_to_exit, quantity_in_lots)
-                neutral = False
+    def check_for_stoploss_hit(opt: Option, sl_price: float):
+        if opt.fetch_ltp() >= sl_price:
+            return True
+        return False
 
-        else:
-            # Re-entry is the first type of condition that can change the position now
-            reentry_option, reentry_check_price = (
-                (straddle.call_option, call_avg_price)
-                if call_sl_hit
-                else (straddle.put_option, put_avg_price)
-            )
-            reentry_condition = (
-                reentry_option.fetch_ltp() < reentry_check_price
-            ) and reattempt_bank[reentry_option] > 0
+    def check_for_reentry_condition(opt: Option, check_price: float):
+        if opt.fetch_ltp() <= check_price:
+            return True
+        return False
 
-            if reentry_condition:
-                notifier(
-                    f"{underlying.name} {strategy_tag} reentry condition met. "
-                    f"Reentering {reentry_option}.",
-                    notification_url,
-                    "INFO",
-                )
-                option_entry_price = reenter_option(reentry_option, quantity_in_lots)
-                reattempt_bank[reentry_option] -= 1
-                neutral = True
-
-            # Second type of condition is trend condition
-            trend_option, trend_sl_price = (
-                (straddle.put_option, put_sl_price)
-                if call_sl_hit
-                else (straddle.call_option, call_sl_price)
+    while current_time().time() < time(*exit_time):
+        if all(
+            [not status[0] for status in status_dict.values()]
+            + [not status[1] for status in status_dict.values()]
+        ):
+            notifier(
+                f"{underlying.name} {strategy_tag} all positions exited.",
+                notification_url,
+                "INFO",
             )
-            trend_sl_hit = trend_option.fetch_ltp() > trend_sl_price
+            return
 
-            if trend_sl_hit:
-                notifier(
-                    f"{underlying.name} {strategy_tag} trend stop loss hit.",
-                    notification_url,
-                    "CRUCIAL",
-                )
-                exit_option(trend_option, quantity_in_lots)
-                # The below condition basically means that the trend option has switched
-                # Happens in the rare case that there is a significant movement
-                # in the opposite direction of the trend
-                if reentry_condition:
-                    # We have already reentered the reentry option
-                    # And exited the trend option
-                    # We just need to change the flags
-                    call_sl_hit, put_sl_hit = put_sl_hit, call_sl_hit
-                    neutral = False
-                    continue
-                break
+        sleep_until_next_action(1, exit_time)
+
+        for option in status_dict:
+            # If its active check for sl, if not check for reentry
+            if status_dict[option][0]:
+                stoploss_price = (
+                    call_sl_price
+                    if option.option_type == OptionType.CALL
+                    else put_sl_price
+                )
+                sl_hit = check_for_stoploss_hit(option, stoploss_price)
+                if sl_hit:
+                    option_exit_price = execute_order(
+                        instrument=option, action=Action.BUY, square_off_order=True
+                    )
+                    status_dict[option] = (False, status_dict[option][1])
+                    notifier(
+                        f"{underlying.name} {strategy_tag} {option} stop loss hit. "
+                        f"Exit price: {option_exit_price}",
+                        notification_url,
+                        "INFO",
+                    )
+            # If its inactive but has reattempts left, check for reentry
+            elif status_dict[option][1] > 0:
+                reentry_price = (
+                    call_avg_price
+                    if option.option_type == OptionType.CALL
+                    else put_avg_price
+                )
+                reentry_hit = check_for_reentry_condition(option, reentry_price)
+                if reentry_hit:
+                    option_entry_price = execute_order(
+                        instrument=option, action=Action.SELL
+                    )
+                    status_dict[option] = (True, status_dict[option][1] - 1)
+                    notifier(
+                        f"{underlying.name} {strategy_tag} {option} reentry condition met. "
+                        f"Reentry price: {option_entry_price}",
+                        notification_url,
+                        "INFO",
+                    )
+            else:
+                pass
 
-    notifier(f"{underlying.name} {strategy_tag} exiting.", notification_url, "INFO")
     # Exit open positions if any
-    if neutral:
-        # Exit the strangle
-        execution_details = execute_instructions(
-            {
-                straddle: {
-                    "action": Action.BUY,
-                    "quantity_in_lots": quantity_in_lots,
-                    "order_tag": strategy_tag,
-                }
-            },
-            at_market=at_market,
-        )
-        call_exit_price, put_exit_price = execution_details[straddle]
-        total_exit_price = call_exit_price + put_exit_price
-        pnl = total_avg_price - total_exit_price
-    elif not neutral and not trend_sl_hit:
-        option_exit_price = exit_option(trend_option, quantity_in_lots)
-    else:
-        pass
+    notifier(f"{underlying.name} {strategy_tag} exiting.", notification_url, "INFO")
+    for option in status_dict:
+        if status_dict[option][0]:
+            execute_order(instrument=option, action=Action.BUY, square_off_order=True)
+
+    notify_pnl(
+        "reentry",
+        start_time=start_time,
+        underlying=underlying,
+        notification_url=notification_url,
+        additional_info=f"Exposure: {exposure}.",
+    )
```

### Comparing `volstreet-8.2.1/volstreet/trade_interface/instruments.py` & `volstreet-8.2.2/volstreet/trade_interface/instruments.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/trade_interface/order_execution.py` & `volstreet-8.2.2/volstreet/trade_interface/order_execution.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/trade_interface/underlyings.py` & `volstreet-8.2.2/volstreet/trade_interface/underlyings.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/utils/change_config.py` & `volstreet-8.2.2/volstreet/utils/change_config.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/utils/communication.py` & `volstreet-8.2.2/volstreet/utils/communication.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/utils/core.py` & `volstreet-8.2.2/volstreet/utils/core.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/utils/data_io.py` & `volstreet-8.2.2/volstreet/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/utils/scrip_processing.py` & `volstreet-8.2.2/volstreet/utils/scrip_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/vectorized_blackscholes.py` & `volstreet-8.2.2/volstreet/vectorized_blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/vslogging/formatters.py` & `volstreet-8.2.2/volstreet/vslogging/formatters.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/vslogging/logging_config.json` & `volstreet-8.2.2/volstreet/vslogging/logging_config.json`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/vslogging/logging_setup.py` & `volstreet-8.2.2/volstreet/vslogging/logging_setup.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet/vslogging/parsing.py` & `volstreet-8.2.2/volstreet/vslogging/parsing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.1/volstreet.egg-info/PKG-INFO` & `volstreet-8.2.2/volstreet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 8.2.1
+Version: 8.2.2
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-8.2.1/volstreet.egg-info/SOURCES.txt` & `volstreet-8.2.2/volstreet.egg-info/SOURCES.txt`

 * *Files identical despite different names*


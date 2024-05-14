# Comparing `tmp/tinkoff_investments-0.2.0b98.tar.gz` & `tmp/tinkoff_investments-0.2.0b99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinkoff_investments-0.2.0b98.tar", max compression
+gzip compressed data, was "tinkoff_investments-0.2.0b99.tar", max compression
```

## Comparing `tinkoff_investments-0.2.0b98.tar` & `tinkoff_investments-0.2.0b99.tar`

### file list

```diff
@@ -1,109 +1,110 @@
--rw-r--r--   0        0        0    11338 2024-05-01 17:29:30.010029 tinkoff_investments-0.2.0b98/LICENSE
--rw-r--r--   0        0        0     2908 2024-05-01 17:29:30.010029 tinkoff_investments-0.2.0b98/README.md
--rw-r--r--   0        0        0     2957 2024-05-01 17:29:30.014029 tinkoff_investments-0.2.0b98/pyproject.toml
--rw-r--r--   0        0        0    12529 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/__init__.py
--rw-r--r--   0        0        0     4742 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/_errors.py
--rw-r--r--   0        0        0    13378 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/_grpc_helpers.py
--rw-r--r--   0        0        0    72216 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/async_services.py
--rw-r--r--   0        0        0        0 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/__init__.py
--rw-r--r--   0        0        0     2685 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/instrument_storage.py
--rw-r--r--   0        0        0     7135 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/instruments_cache.py
--rw-r--r--   0        0        0     2167 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/interface.py
--rw-r--r--   0        0        0      187 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/models.py
--rw-r--r--   0        0        0      379 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/protocol.py
--rw-r--r--   0        0        0      148 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/settings.py
--rw-r--r--   0        0        0        0 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/__init__.py
--rw-r--r--   0        0        0     5302 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/cache.py
--rw-r--r--   0        0        0     1388 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/cache_settings.py
--rw-r--r--   0        0        0       98 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/datetime_range.py
--rw-r--r--   0        0        0      315 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/instrument_date_range_market_data.py
--rw-r--r--   0        0        0    11766 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/instrument_market_data_storage.py
--rw-r--r--   0        0        0      376 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/interface.py
--rw-r--r--   0        0        0      218 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/serialization.py
--rw-r--r--   0        0        0      305 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/overrides.py
--rw-r--r--   0        0        0      411 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/candle_getter_protocol.py
--rw-r--r--   0        0        0     1504 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/channels.py
--rw-r--r--   0        0        0     3016 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/clients.py
--rw-r--r--   0        0        0      439 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/constants.py
--rw-r--r--   0        0        0      914 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/__init__.py
--rw-r--r--   0        0        0     4818 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/common_pb2.py
--rw-r--r--   0        0        0    15679 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/common_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/common_pb2_grpc.py
--rw-r--r--   0        0        0     1871 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/google/api/field_behavior_pb2.py
--rw-r--r--   0        0        0     6343 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/google/api/field_behavior_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/google/api/field_behavior_pb2_grpc.py
--rw-r--r--   0        0        0    77252 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/instruments_pb2.py
--rw-r--r--   0        0        0   275576 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/instruments_pb2.pyi
--rw-r--r--   0        0        0    63760 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/instruments_pb2_grpc.py
--rw-r--r--   0        0        0    36932 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/marketdata_pb2.py
--rw-r--r--   0        0        0   119955 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/marketdata_pb2.pyi
--rw-r--r--   0        0        0    21465 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/marketdata_pb2_grpc.py
--rw-r--r--   0        0        0    35099 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/operations_pb2.py
--rw-r--r--   0        0        0   113219 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/operations_pb2.pyi
--rw-r--r--   0        0        0    20550 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/operations_pb2_grpc.py
--rw-r--r--   0        0        0    24889 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/orders_pb2.py
--rw-r--r--   0        0        0    74934 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/orders_pb2.pyi
--rw-r--r--   0        0        0    19021 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/orders_pb2_grpc.py
--rw-r--r--   0        0        0     6383 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/sandbox_pb2.py
--rw-r--r--   0        0        0     4578 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/sandbox_pb2.pyi
--rw-r--r--   0        0        0    29360 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/sandbox_pb2_grpc.py
--rw-r--r--   0        0        0    12547 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/stoporders_pb2.py
--rw-r--r--   0        0        0    31067 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/stoporders_pb2.pyi
--rw-r--r--   0        0        0     7177 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/stoporders_pb2_grpc.py
--rw-r--r--   0        0        0     7030 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/users_pb2.py
--rw-r--r--   0        0        0    17677 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/users_pb2.pyi
--rw-r--r--   0        0        0     8756 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/users_pb2_grpc.py
--rw-r--r--   0        0        0     3485 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/logging.py
--rw-r--r--   0        0        0        0 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/__init__.py
--rw-r--r--   0        0        0     2971 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/async_market_data_stream_manager.py
--rw-r--r--   0        0        0     1362 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/market_data_stream_interface.py
--rw-r--r--   0        0        0     2799 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/market_data_stream_manager.py
--rw-r--r--   0        0        0     5101 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/stream_managers.py
--rw-r--r--   0        0        0      128 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/typevars.py
--rw-r--r--   0        0        0      289 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/metadata.py
--rw-r--r--   0        0        0    12487 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/mock_services.py
--rw-r--r--   0        0        0        0 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/py.typed
--rw-r--r--   0        0        0        0 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/aio/__init__.py
--rw-r--r--   0        0        0      825 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/aio/client.py
--rw-r--r--   0        0        0      772 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/aio/grpc_interceptor.py
--rw-r--r--   0        0        0     1163 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/aio/retry_manager.py
--rw-r--r--   0        0        0      796 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/base_retry_manager.py
--rw-r--r--   0        0        0      243 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/settings.py
--rw-r--r--   0        0        0      122 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/settings_protocol.py
--rw-r--r--   0        0        0        0 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/sync/__init__.py
--rw-r--r--   0        0        0      792 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/sync/client.py
--rw-r--r--   0        0        0      696 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/sync/grpc_interceptor.py
--rw-r--r--   0        0        0     1027 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/sync/retry_manager.py
--rw-r--r--   0        0        0        0 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/sandbox/__init__.py
--rw-r--r--   0        0        0      296 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/sandbox/client.py
--rw-r--r--   0        0        0   123566 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/schemas.py
--rw-r--r--   0        0        0    70635 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/services.py
--rw-r--r--   0        0        0        0 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/__init__.py
--rw-r--r--   0        0        0     1457 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/account_manager.py
--rw-r--r--   0        0        0      555 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/errors.py
--rw-r--r--   0        0        0      401 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/event.py
--rw-r--r--   0        0        0      341 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/models.py
--rw-r--r--   0        0        0      847 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/signal.py
--rw-r--r--   0        0        0     2032 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/signal_executor_base.py
--rw-r--r--   0        0        0      387 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/strategy_interface.py
--rw-r--r--   0        0        0      541 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/strategy_settings_base.py
--rw-r--r--   0        0        0      754 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/strategy_supervisor.py
--rw-r--r--   0        0        0     2435 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/trader_base.py
--rw-r--r--   0        0        0       89 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/trader_interface.py
--rw-r--r--   0        0        0        0 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/__init__.py
--rw-r--r--   0        0        0     7419 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/plotter.py
--rw-r--r--   0        0        0     2244 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/signal_executor.py
--rw-r--r--   0        0        0    10442 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/strategy.py
--rw-r--r--   0        0        0      295 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/strategy_settings.py
--rw-r--r--   0        0        0      705 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/strategy_state.py
--rw-r--r--   0        0        0      970 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/supervisor.py
--rw-r--r--   0        0        0     6514 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/trader.py
--rw-r--r--   0        0        0        0 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/plotting/__init__.py
--rw-r--r--   0        0        0     1973 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/plotting/plotter.py
--rw-r--r--   0        0        0      170 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/typedefs.py
--rw-r--r--   0        0        0     7651 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/utils.py
--rw-r--r--   0        0        0     4114 1970-01-01 00:00:00.000000 tinkoff_investments-0.2.0b98/PKG-INFO
+-rw-r--r--   0        0        0    11338 2024-05-14 14:12:32.645167 tinkoff_investments-0.2.0b99/LICENSE
+-rw-r--r--   0        0        0     2908 2024-05-14 14:12:32.645167 tinkoff_investments-0.2.0b99/README.md
+-rw-r--r--   0        0        0     2957 2024-05-14 14:12:32.653168 tinkoff_investments-0.2.0b99/pyproject.toml
+-rw-r--r--   0        0        0    12529 2024-05-14 14:12:32.653168 tinkoff_investments-0.2.0b99/tinkoff/invest/__init__.py
+-rw-r--r--   0        0        0     4742 2024-05-14 14:12:32.653168 tinkoff_investments-0.2.0b99/tinkoff/invest/_errors.py
+-rw-r--r--   0        0        0    13378 2024-05-14 14:12:32.653168 tinkoff_investments-0.2.0b99/tinkoff/invest/_grpc_helpers.py
+-rw-r--r--   0        0        0    72831 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/async_services.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/caching/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/caching/instruments_cache/__init__.py
+-rw-r--r--   0        0        0     2685 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/caching/instruments_cache/instrument_storage.py
+-rw-r--r--   0        0        0     7135 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/caching/instruments_cache/instruments_cache.py
+-rw-r--r--   0        0        0     2167 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/caching/instruments_cache/interface.py
+-rw-r--r--   0        0        0      187 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/caching/instruments_cache/models.py
+-rw-r--r--   0        0        0      379 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/caching/instruments_cache/protocol.py
+-rw-r--r--   0        0        0      148 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/caching/instruments_cache/settings.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/caching/market_data_cache/__init__.py
+-rw-r--r--   0        0        0     5302 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/caching/market_data_cache/cache.py
+-rw-r--r--   0        0        0     1388 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/caching/market_data_cache/cache_settings.py
+-rw-r--r--   0        0        0       98 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/caching/market_data_cache/datetime_range.py
+-rw-r--r--   0        0        0      315 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/caching/market_data_cache/instrument_date_range_market_data.py
+-rw-r--r--   0        0        0    11766 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/caching/market_data_cache/instrument_market_data_storage.py
+-rw-r--r--   0        0        0      376 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/caching/market_data_cache/interface.py
+-rw-r--r--   0        0        0      218 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/caching/market_data_cache/serialization.py
+-rw-r--r--   0        0        0      305 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/caching/overrides.py
+-rw-r--r--   0        0        0      411 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/candle_getter_protocol.py
+-rw-r--r--   0        0        0     1504 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/channels.py
+-rw-r--r--   0        0        0     3016 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/clients.py
+-rw-r--r--   0        0        0      439 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/constants.py
+-rw-r--r--   0        0        0      914 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/__init__.py
+-rw-r--r--   0        0        0     4818 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/common_pb2.py
+-rw-r--r--   0        0        0    15679 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/common_pb2_grpc.py
+-rw-r--r--   0        0        0     1871 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/google/api/field_behavior_pb2.py
+-rw-r--r--   0        0        0     6343 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/google/api/field_behavior_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/google/api/field_behavior_pb2_grpc.py
+-rw-r--r--   0        0        0    77252 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/instruments_pb2.py
+-rw-r--r--   0        0        0   275576 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/instruments_pb2.pyi
+-rw-r--r--   0        0        0    63760 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/instruments_pb2_grpc.py
+-rw-r--r--   0        0        0    36932 2024-05-14 14:12:32.657168 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/marketdata_pb2.py
+-rw-r--r--   0        0        0   119955 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/marketdata_pb2.pyi
+-rw-r--r--   0        0        0    21465 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/marketdata_pb2_grpc.py
+-rw-r--r--   0        0        0    35099 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/operations_pb2.py
+-rw-r--r--   0        0        0   113219 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/operations_pb2.pyi
+-rw-r--r--   0        0        0    20550 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/operations_pb2_grpc.py
+-rw-r--r--   0        0        0    24889 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/orders_pb2.py
+-rw-r--r--   0        0        0    74934 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/orders_pb2.pyi
+-rw-r--r--   0        0        0    19021 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/orders_pb2_grpc.py
+-rw-r--r--   0        0        0     6383 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/sandbox_pb2.py
+-rw-r--r--   0        0        0     4578 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/sandbox_pb2.pyi
+-rw-r--r--   0        0        0    29360 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/sandbox_pb2_grpc.py
+-rw-r--r--   0        0        0    12547 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/stoporders_pb2.py
+-rw-r--r--   0        0        0    31067 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/stoporders_pb2.pyi
+-rw-r--r--   0        0        0     7177 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/stoporders_pb2_grpc.py
+-rw-r--r--   0        0        0     7030 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/users_pb2.py
+-rw-r--r--   0        0        0    17677 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/users_pb2.pyi
+-rw-r--r--   0        0        0     8756 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/users_pb2_grpc.py
+-rw-r--r--   0        0        0     3485 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/logging.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/market_data_stream/__init__.py
+-rw-r--r--   0        0        0     2971 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/market_data_stream/async_market_data_stream_manager.py
+-rw-r--r--   0        0        0     1362 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/market_data_stream/market_data_stream_interface.py
+-rw-r--r--   0        0        0     2799 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/market_data_stream/market_data_stream_manager.py
+-rw-r--r--   0        0        0     5101 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/market_data_stream/stream_managers.py
+-rw-r--r--   0        0        0      128 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/market_data_stream/typevars.py
+-rw-r--r--   0        0        0      289 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/metadata.py
+-rw-r--r--   0        0        0    12487 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/mock_services.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/py.typed
+-rw-r--r--   0        0        0        0 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/aio/__init__.py
+-rw-r--r--   0        0        0      825 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/aio/client.py
+-rw-r--r--   0        0        0      772 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/aio/grpc_interceptor.py
+-rw-r--r--   0        0        0     1163 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/aio/retry_manager.py
+-rw-r--r--   0        0        0      796 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/base_retry_manager.py
+-rw-r--r--   0        0        0      243 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/settings.py
+-rw-r--r--   0        0        0      122 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/settings_protocol.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/sync/__init__.py
+-rw-r--r--   0        0        0      792 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/sync/client.py
+-rw-r--r--   0        0        0      696 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/sync/grpc_interceptor.py
+-rw-r--r--   0        0        0     1027 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/sync/retry_manager.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/sandbox/__init__.py
+-rw-r--r--   0        0        0      311 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/sandbox/async_client.py
+-rw-r--r--   0        0        0      296 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/sandbox/client.py
+-rw-r--r--   0        0        0   123566 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/schemas.py
+-rw-r--r--   0        0        0    71197 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/services.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/__init__.py
+-rw-r--r--   0        0        0     1457 2024-05-14 14:12:32.661167 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/account_manager.py
+-rw-r--r--   0        0        0      555 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/errors.py
+-rw-r--r--   0        0        0      401 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/event.py
+-rw-r--r--   0        0        0      341 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/models.py
+-rw-r--r--   0        0        0      847 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/signal.py
+-rw-r--r--   0        0        0     2032 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/signal_executor_base.py
+-rw-r--r--   0        0        0      387 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/strategy_interface.py
+-rw-r--r--   0        0        0      541 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/strategy_settings_base.py
+-rw-r--r--   0        0        0      754 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/strategy_supervisor.py
+-rw-r--r--   0        0        0     2435 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/trader_base.py
+-rw-r--r--   0        0        0       89 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/trader_interface.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/moving_average/__init__.py
+-rw-r--r--   0        0        0     7419 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/moving_average/plotter.py
+-rw-r--r--   0        0        0     2244 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/moving_average/signal_executor.py
+-rw-r--r--   0        0        0    10442 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/moving_average/strategy.py
+-rw-r--r--   0        0        0      295 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/moving_average/strategy_settings.py
+-rw-r--r--   0        0        0      705 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/moving_average/strategy_state.py
+-rw-r--r--   0        0        0      970 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/moving_average/supervisor.py
+-rw-r--r--   0        0        0     6514 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/moving_average/trader.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/plotting/__init__.py
+-rw-r--r--   0        0        0     1973 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/plotting/plotter.py
+-rw-r--r--   0        0        0      170 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/typedefs.py
+-rw-r--r--   0        0        0     7651 2024-05-14 14:12:32.665168 tinkoff_investments-0.2.0b99/tinkoff/invest/utils.py
+-rw-r--r--   0        0        0     4114 1970-01-01 00:00:00.000000 tinkoff_investments-0.2.0b99/PKG-INFO
```

### Comparing `tinkoff_investments-0.2.0b98/LICENSE` & `tinkoff_investments-0.2.0b99/LICENSE`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/README.md` & `tinkoff_investments-0.2.0b99/README.md`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/pyproject.toml` & `tinkoff_investments-0.2.0b99/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "tinkoff-investments"
-version = "0.2.0-beta98"
+version = "0.2.0-beta99"
 description = "Tinkoff Python SDK"
 authors = ["Tinkoff Team <python@tinkoff.ru>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/RussianInvestments/invest-python"
 homepage = "https://github.com/RussianInvestments/invest-python"
 packages = [
```

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/__init__.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
     TradingSchedulesResponse,
     TradingStatus,
     UnaryLimit,
     WithdrawLimitsRequest,
     WithdrawLimitsResponse,
 )
 
-__version__ = "0.2.0-beta98"
+__version__ = "0.2.0-beta99"
 
 __all__ = (
     "__version__",
     "AccessLevel",
     "Account",
     "AccountStatus",
     "AccountSubscriptionStatus",
```

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/_errors.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/_errors.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/_grpc_helpers.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/_grpc_helpers.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/async_services.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/async_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1800,14 +1800,30 @@
         )
         response = await response_coro
         log_request(
             await get_tracking_id_from_coro(response_coro), "GetSandboxWithdrawLimits"
         )
         return _grpc_helpers.protobuf_to_dataclass(response, WithdrawLimitsResponse)
 
+    @handle_aio_request_error("GetSandboxMaxLots")
+    async def get_sandbox_max_lots(
+        self,
+        *,
+        request: GetMaxLotsRequest,
+    ) -> GetMaxLotsResponse:
+        response_coro = self.stub.GetSandboxMaxLots(
+            request=_grpc_helpers.dataclass_to_protobuff(
+                request, orders_pb2.GetMaxLotsRequest()
+            ),
+            metadata=self.metadata,
+        )
+        response = await response_coro
+        log_request(await get_tracking_id_from_coro(response_coro), "GetSandboxMaxLots")
+        return _grpc_helpers.protobuf_to_dataclass(response, GetMaxLotsResponse)
+
 
 class StopOrdersService(_grpc_helpers.Service):
     _stub_factory = stoporders_pb2_grpc.StopOrdersServiceStub
 
     @handle_aio_request_error("PostStopOrder")
     async def post_stop_order(
         self,
```

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/instrument_storage.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/caching/instruments_cache/instrument_storage.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/instruments_cache.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/caching/instruments_cache/instruments_cache.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/interface.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/caching/instruments_cache/interface.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/cache.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/caching/market_data_cache/cache.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/cache_settings.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/caching/market_data_cache/cache_settings.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/instrument_market_data_storage.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/caching/market_data_cache/instrument_market_data_storage.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/channels.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/channels.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/clients.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/clients.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/exceptions.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/exceptions.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/common_pb2.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/common_pb2.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/common_pb2.pyi` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/google/api/field_behavior_pb2.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/google/api/field_behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/google/api/field_behavior_pb2.pyi` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/google/api/field_behavior_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/instruments_pb2.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/instruments_pb2.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/instruments_pb2.pyi` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/instruments_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/instruments_pb2_grpc.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/instruments_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/marketdata_pb2.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/marketdata_pb2.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/marketdata_pb2.pyi` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/marketdata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/marketdata_pb2_grpc.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/marketdata_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/operations_pb2.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/operations_pb2.pyi` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/operations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/operations_pb2_grpc.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/orders_pb2.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/orders_pb2.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/orders_pb2.pyi` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/orders_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/orders_pb2_grpc.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/orders_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/sandbox_pb2.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/sandbox_pb2.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/sandbox_pb2.pyi` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/sandbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/sandbox_pb2_grpc.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/sandbox_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/stoporders_pb2.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/stoporders_pb2.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/stoporders_pb2.pyi` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/stoporders_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/stoporders_pb2_grpc.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/stoporders_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/users_pb2.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/users_pb2.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/users_pb2.pyi` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/users_pb2_grpc.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/grpc/users_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/logging.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/logging.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/async_market_data_stream_manager.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/market_data_stream/async_market_data_stream_manager.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/market_data_stream_interface.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/market_data_stream/market_data_stream_interface.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/market_data_stream_manager.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/market_data_stream/market_data_stream_manager.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/stream_managers.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/market_data_stream/stream_managers.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/mock_services.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/mock_services.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/aio/client.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/aio/client.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/aio/grpc_interceptor.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/aio/grpc_interceptor.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/aio/retry_manager.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/aio/retry_manager.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/base_retry_manager.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/base_retry_manager.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/sync/client.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/sync/client.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/sync/grpc_interceptor.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/sync/grpc_interceptor.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/sync/retry_manager.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/retrying/sync/retry_manager.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/schemas.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/schemas.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/services.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1755,14 +1755,29 @@
                 request, operations_pb2.WithdrawLimitsRequest()
             ),
             metadata=self.metadata,
         )
         log_request(get_tracking_id_from_call(call), "GetSandboxWithdrawLimits")
         return _grpc_helpers.protobuf_to_dataclass(response, WithdrawLimitsResponse)
 
+    @handle_request_error("GetSandboxMaxLots")
+    def get_sandbox_max_lots(
+        self,
+        *,
+        request: GetMaxLotsRequest,
+    ) -> GetMaxLotsResponse:
+        response, call = self.stub.GetSandboxMaxLots.with_call(
+            request=_grpc_helpers.dataclass_to_protobuff(
+                request, orders_pb2.GetMaxLotsRequest()
+            ),
+            metadata=self.metadata,
+        )
+        log_request(get_tracking_id_from_call(call), "GetSandboxMaxLots")
+        return _grpc_helpers.protobuf_to_dataclass(response, GetMaxLotsResponse)
+
 
 class StopOrdersService(_grpc_helpers.Service):
     _stub_factory = stoporders_pb2_grpc.StopOrdersServiceStub
 
     @handle_request_error("PostStopOrder")
     def post_stop_order(
         self,
```

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/account_manager.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/account_manager.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/errors.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/errors.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/signal.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/signal.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/signal_executor_base.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/signal_executor_base.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/strategy_settings_base.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/strategy_settings_base.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/strategy_supervisor.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/strategy_supervisor.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/trader_base.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/base/trader_base.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/plotter.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/moving_average/plotter.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/signal_executor.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/moving_average/signal_executor.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/strategy.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/moving_average/strategy.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/strategy_state.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/moving_average/strategy_state.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/supervisor.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/moving_average/supervisor.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/trader.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/moving_average/trader.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/plotting/plotter.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/strategies/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/tinkoff/invest/utils.py` & `tinkoff_investments-0.2.0b99/tinkoff/invest/utils.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b98/PKG-INFO` & `tinkoff_investments-0.2.0b99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinkoff-investments
-Version: 0.2.0b98
+Version: 0.2.0b99
 Summary: Tinkoff Python SDK
 Home-page: https://github.com/RussianInvestments/invest-python
 License: Apache-2.0
 Author: Tinkoff Team
 Author-email: python@tinkoff.ru
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```


# Comparing `tmp/stsdk-0.3.1.dev1.tar.gz` & `tmp/stsdk-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stsdk-0.3.1.dev1.tar", max compression
+gzip compressed data, was "stsdk-0.3.2.tar", max compression
```

## Comparing `stsdk-0.3.1.dev1.tar` & `stsdk-0.3.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     1503 2024-04-23 07:54:20.342049 stsdk-0.3.1.dev1/README.md
--rw-r--r--   0        0        0      848 2024-04-23 08:13:23.259206 stsdk-0.3.1.dev1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/api/http/__init__.py
--rw-r--r--   0        0        0     5397 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/api/http/dms.py
--rw-r--r--   0        0        0     2493 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/api/http/oms.py
--rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/api/http/sms.py
--rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/api/ws/__init__.py
--rw-r--r--   0        0        0     1155 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/api/ws/dms.py
--rw-r--r--   0        0        0      625 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/api/ws/oms.py
--rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/common/__init__.py
--rw-r--r--   0        0        0       24 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/common/cache_key.py
--rw-r--r--   0        0        0      174 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/common/constant.py
--rw-r--r--   0        0        0       72 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/common/env.py
--rw-r--r--   0        0        0      623 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/common/exception.py
--rw-r--r--   0        0        0     3273 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/common/key.py
--rw-r--r--   0        0        0      200 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/common/signal_key.py
--rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/config/__init__.py
--rw-r--r--   0        0        0      694 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/config/config.json
--rw-r--r--   0        0        0      487 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/config/pre.config.json
--rw-r--r--   0        0        0      546 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/config/prod.config.json
--rw-r--r--   0        0        0      558 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/config/stage.config.json
--rw-r--r--   0        0        0      495 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/config/test.config.json
--rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/model/__init__.py
--rw-r--r--   0        0        0     8087 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/model/instrument.py
--rw-r--r--   0        0        0    15162 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/model/order_manager.py
--rw-r--r--   0        0        0    27585 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/model/position_manager.py
--rw-r--r--   0        0        0     4583 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/model/strategy_base.py
--rw-r--r--   0        0        0    21805 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/model/strategy_module.py
--rw-r--r--   0        0        0     1000 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/Stresstest/Stress_klines.py
--rw-r--r--   0        0        0      978 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/Stresstest/mongoBDtest.py
--rw-r--r--   0        0        0      696 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/Stresstest/stressone.py
--rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/__init__.py
--rw-r--r--   0        0        0     2450 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/test/aliyun_log_test.py
--rw-r--r--   0        0        0      450 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/bbo_ws.py
--rw-r--r--   0        0        0      402 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/bbo_ws_main.py
--rw-r--r--   0        0        0      423 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/blinker_block_test.py
--rw-r--r--   0        0        0      406 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/blinker_test.py
--rw-r--r--   0        0        0      289 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/cache_test.py
--rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/case/__init__.py
--rw-r--r--   0        0        0     1747 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/case/order.py
--rw-r--r--   0        0        0       61 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/constants.py
--rw-r--r--   0        0        0      817 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/create_account.py
--rw-r--r--   0        0        0      524 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/main.py
--rw-r--r--   0        0        0     3474 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/test/metric_test.py
--rw-r--r--   0        0        0     1115 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/CreatePosition.py
--rw-r--r--   0        0        0      693 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/GetOrderFormPositionId.py
--rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/__init__.py
--rw-r--r--   0        0        0     5317 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/assets/style.css
--rw-r--r--   0        0        0      623 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/conftest.py
--rw-r--r--   0        0        0      745 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/initialization.py
--rw-r--r--   0        0        0     1351 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/placeOrder.py
--rw-r--r--   0        0        0      430 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/pmsinit.py
--rw-r--r--   0        0        0     1805 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/test/ordertest/position_test.py
--rw-r--r--   0        0        0      180 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/pytest.ini
--rw-r--r--   0        0        0     5317 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/reports/assets/style.css
--rw-r--r--   0        0        0     2188 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/test/ordertest/stagegymoduletest.py
--rw-r--r--   0        0        0     4598 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/test_Kline.py
--rw-r--r--   0        0        0      654 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/test_cancel_all_outstanding_orders.py
--rw-r--r--   0        0        0     9694 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/test_change_leverage.py
--rw-r--r--   0        0        0     3603 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/test_close_all_positions.py
--rw-r--r--   0        0        0     1847 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/test_get_all_outstanding_orders.py
--rw-r--r--   0        0        0     3030 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/test_order_closed_loop.py
--rw-r--r--   0        0        0    23338 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/test_order_empty_multiple.py
--rw-r--r--   0        0        0     1814 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/test_position_model.py
--rw-r--r--   0        0        0     2189 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/place_order_signal.py
--rw-r--r--   0        0        0      647 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/precision_speed_compare.py
--rw-r--r--   0        0        0     2830 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/test/redis_pubsub_test.py
--rw-r--r--   0        0        0     2346 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/signal_order.py
--rw-r--r--   0        0        0     3571 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/test/st_2.py
--rw-r--r--   0        0        0     2044 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/test/st_demo_1.py
--rw-r--r--   0        0        0      325 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/test/test.py
--rw-r--r--   0        0        0      754 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/test/test_placeorder.py
--rw-r--r--   0        0        0        0 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/test/unittest/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/__init__.py
--rw-r--r--   0        0        0     6280 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/utils/ali_sls.py
--rw-r--r--   0        0        0      818 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/cache_manager.py
--rw-r--r--   0        0        0     6060 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/utils/config.py
--rw-r--r--   0        0        0     2124 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/consul.py
--rw-r--r--   0        0        0     1084 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/http.py
--rw-r--r--   0        0        0      749 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/instrument_id.py
--rw-r--r--   0        0        0     2260 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/log.py
--rw-r--r--   0        0        0     1488 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/utils/metric.py
--rw-r--r--   0        0        0      361 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/precision.py
--rw-r--r--   0        0        0     2099 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/redis_utils.py
--rw-r--r--   0        0        0     1177 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/websocket.py
--rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 stsdk-0.3.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1503 2024-04-25 10:13:01.907026 stsdk-0.3.2/README.md
+-rw-r--r--   0        0        0      843 2024-05-14 13:32:33.938787 stsdk-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/api/http/__init__.py
+-rw-r--r--   0        0        0     5397 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/api/http/dms.py
+-rw-r--r--   0        0        0     2508 2024-05-14 13:32:21.002713 stsdk-0.3.2/stsdk/api/http/oms.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/api/http/sms.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/api/ws/__init__.py
+-rw-r--r--   0        0        0     1155 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/api/ws/dms.py
+-rw-r--r--   0        0        0      625 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/api/ws/oms.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/common/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/common/cache_key.py
+-rw-r--r--   0        0        0      174 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/common/constant.py
+-rw-r--r--   0        0        0       72 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/common/env.py
+-rw-r--r--   0        0        0      623 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/common/exception.py
+-rw-r--r--   0        0        0     3273 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/common/key.py
+-rw-r--r--   0        0        0      200 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/common/signal_key.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/config/__init__.py
+-rw-r--r--   0        0        0      694 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/config/config.json
+-rw-r--r--   0        0        0      487 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/config/pre.config.json
+-rw-r--r--   0        0        0      546 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/config/prod.config.json
+-rw-r--r--   0        0        0      558 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/config/stage.config.json
+-rw-r--r--   0        0        0      495 2024-05-14 13:32:10.010649 stsdk-0.3.2/stsdk/config/test.config.json
+-rw-r--r--   0        0        0        0 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/model/__init__.py
+-rw-r--r--   0        0        0     8087 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/model/instrument.py
+-rw-r--r--   0        0        0    15788 2024-05-14 13:32:21.002713 stsdk-0.3.2/stsdk/model/order_manager.py
+-rw-r--r--   0        0        0    23482 2024-05-14 13:32:21.002713 stsdk-0.3.2/stsdk/model/position_manager.py
+-rw-r--r--   0        0        0     4583 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/model/strategy_base.py
+-rw-r--r--   0        0        0    21805 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/model/strategy_module.py
+-rw-r--r--   0        0        0     1000 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/Stresstest/Stress_klines.py
+-rw-r--r--   0        0        0      978 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/Stresstest/mongoBDtest.py
+-rw-r--r--   0        0        0      696 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/Stresstest/stressone.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/__init__.py
+-rw-r--r--   0        0        0     2450 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/aliyun_log_test.py
+-rw-r--r--   0        0        0      450 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/bbo_ws.py
+-rw-r--r--   0        0        0      402 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/bbo_ws_main.py
+-rw-r--r--   0        0        0      423 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/blinker_block_test.py
+-rw-r--r--   0        0        0      406 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/blinker_test.py
+-rw-r--r--   0        0        0      289 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/cache_test.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/case/__init__.py
+-rw-r--r--   0        0        0     1747 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/case/order.py
+-rw-r--r--   0        0        0       61 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/constants.py
+-rw-r--r--   0        0        0      817 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/create_account.py
+-rw-r--r--   0        0        0      524 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/main.py
+-rw-r--r--   0        0        0     3474 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/metric_test.py
+-rw-r--r--   0        0        0     1115 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/CreatePosition.py
+-rw-r--r--   0        0        0      693 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/GetOrderFormPositionId.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/__init__.py
+-rw-r--r--   0        0        0     5317 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/assets/style.css
+-rw-r--r--   0        0        0      623 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/conftest.py
+-rw-r--r--   0        0        0      745 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/initialization.py
+-rw-r--r--   0        0        0     1351 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/placeOrder.py
+-rw-r--r--   0        0        0      430 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/pmsinit.py
+-rw-r--r--   0        0        0     1805 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/position_test.py
+-rw-r--r--   0        0        0      180 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/pytest.ini
+-rw-r--r--   0        0        0     5317 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/reports/assets/style.css
+-rw-r--r--   0        0        0     2188 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/stagegymoduletest.py
+-rw-r--r--   0        0        0     4598 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/test_Kline.py
+-rw-r--r--   0        0        0      654 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/test_cancel_all_outstanding_orders.py
+-rw-r--r--   0        0        0     9694 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/test_change_leverage.py
+-rw-r--r--   0        0        0     3603 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/test_close_all_positions.py
+-rw-r--r--   0        0        0     1847 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/test_get_all_outstanding_orders.py
+-rw-r--r--   0        0        0     3030 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/test_order_closed_loop.py
+-rw-r--r--   0        0        0    23338 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/test_order_empty_multiple.py
+-rw-r--r--   0        0        0     1814 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/ordertest/test_position_model.py
+-rw-r--r--   0        0        0     2189 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/place_order_signal.py
+-rw-r--r--   0        0        0      647 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/precision_speed_compare.py
+-rw-r--r--   0        0        0     2830 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/redis_pubsub_test.py
+-rw-r--r--   0        0        0     2346 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/signal_order.py
+-rw-r--r--   0        0        0     3571 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/st_2.py
+-rw-r--r--   0        0        0     2044 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/st_demo_1.py
+-rw-r--r--   0        0        0      325 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/test.py
+-rw-r--r--   0        0        0      754 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/test_placeorder.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/test/unittest/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/utils/__init__.py
+-rw-r--r--   0        0        0     6280 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/utils/ali_sls.py
+-rw-r--r--   0        0        0      818 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/utils/cache_manager.py
+-rw-r--r--   0        0        0     6060 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/utils/config.py
+-rw-r--r--   0        0        0     2124 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/utils/consul.py
+-rw-r--r--   0        0        0     1084 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/utils/http.py
+-rw-r--r--   0        0        0      749 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/utils/instrument_id.py
+-rw-r--r--   0        0        0     2260 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/utils/log.py
+-rw-r--r--   0        0        0     1488 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/utils/metric.py
+-rw-r--r--   0        0        0      361 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/utils/precision.py
+-rw-r--r--   0        0        0     2099 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/utils/redis_utils.py
+-rw-r--r--   0        0        0     1177 2024-05-14 13:32:10.014649 stsdk-0.3.2/stsdk/utils/websocket.py
+-rw-r--r--   0        0        0     2786 1970-01-01 00:00:00.000000 stsdk-0.3.2/PKG-INFO
```

### Comparing `stsdk-0.3.1.dev1/README.md` & `stsdk-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/pyproject.toml` & `stsdk-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stsdk"
-version = "0.3.1.dev1"
+version = "0.3.2"
 description = "this is for at trade strategy module"
 authors = ["stark <yangwang@web3.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 start = 'test.main:main'
```

### Comparing `stsdk-0.3.1.dev1/stsdk/api/http/dms.py` & `stsdk-0.3.2/stsdk/api/http/dms.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/api/http/oms.py` & `stsdk-0.3.2/stsdk/api/http/oms.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,16 @@
 
     def change_leverage(self, data=None):
         if data is None:
             return
         resp = request.post(self.OMS_BASE_HTTP_URL + "/leverage", data=data)
         return resp
 
-    def get_all_positions(self, params=None):
-        resp = request.get(self.OMS_BASE_HTTP_URL + "/position/all", params=params)
+    def get_all_positions_by_account(self, params=None):
+        resp = request.get(self.OMS_BASE_HTTP_URL + "/position/account", params=params)
         return resp
 
     def get_position_mode(self, params=None):
         resp = request.get(self.OMS_BASE_HTTP_URL + "/account/positionMode", params=params)
         return resp
 
     def change_position_mode(self, data=None):
```

### Comparing `stsdk-0.3.1.dev1/stsdk/api/ws/dms.py` & `stsdk-0.3.2/stsdk/api/ws/dms.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/api/ws/oms.py` & `stsdk-0.3.2/stsdk/api/ws/oms.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/common/exception.py` & `stsdk-0.3.2/stsdk/common/exception.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/common/key.py` & `stsdk-0.3.2/stsdk/common/key.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/config/config.json` & `stsdk-0.3.2/stsdk/config/config.json`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/config/prod.config.json` & `stsdk-0.3.2/stsdk/config/prod.config.json`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/config/stage.config.json` & `stsdk-0.3.2/stsdk/config/stage.config.json`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/model/instrument.py` & `stsdk-0.3.2/stsdk/model/instrument.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/model/order_manager.py` & `stsdk-0.3.2/stsdk/model/order_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from typing import Dict, List, Set
 
 from sortedcontainers import SortedDict
 from copy import deepcopy
 from stsdk.api.http.oms import OMSApi
 from stsdk.common.exception import *
 from stsdk.common.key import (
@@ -404,7 +405,25 @@
         :param position_id: 仓位id
         :param leverage: 杠杆倍率
         :return position_id: 仓位id
         :return leverage: 杠杆倍率
         """
         data = {"position_id": position_id, "leverage": leverage}
         return self.omsApi.change_leverage(data)
+
+    def sync_outstanding_orders(self):
+        """
+        同步所有outstanding订单
+        :return: order list
+        """
+        data = {
+            "strategy_id": self.strategy_id,
+            "account_id": self.account_id,
+        }
+        resp = self.omsApi.get_all_outstanding_orders(data)
+        if "Orders" not in resp:
+            log.info("sync outstanding orders is empty")
+            return resp
+        log.info("sync outstanding orders: ", resp["Orders"])
+        for info in resp["Orders"]:
+            self.append_order(instrument_id=info["instrument_id"], data=info)
+        return resp
```

### Comparing `stsdk-0.3.1.dev1/stsdk/model/position_manager.py` & `stsdk-0.3.2/stsdk/model/position_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -132,42 +132,15 @@
         orig_qty = float(op_info["origin_quantity"])
         position_side = op_info["position_side"]
         if op_info["order_direction"] == ORDER_DIRECTION_BUY_STR:
             position.long_outstanding = prec.add(
                 position.long_outstanding, orig_qty, instrument.qty_unit
             )
             if position_side == POSITION_SIDE_NOTBOTH_STR:
-                self.active_long_closing_quota[instrument_id] = position.long_filled + position.long_outstanding
-                # size = orig_qty
-                # if self.active_short_closing_quota[instrument_id] > 0:
-                #     _update_size = min(
-                #         self.active_short_closing_quota[instrument_id], size
-                #     )
-                #     self.active_short_closing_quota[instrument_id] = prec.substract(
-                #         self.active_short_closing_quota[instrument_id],
-                #         _update_size,
-                #         instrument.qty_unit,
-                #     )
-                #     self.active_short_opening_quota[instrument_id] = prec.add(
-                #         self.active_short_opening_quota[instrument_id],
-                #         _update_size,
-                #         instrument.qty_unit,
-                #     )
-                #     size = prec.substract(size, _update_size, instrument.qty_unit)
-                # if size > 0:
-                #     self.active_long_opening_quota[instrument_id] = prec.substract(
-                #         self.active_long_opening_quota[instrument_id],
-                #         size,
-                #         instrument.qty_unit,
-                #     )
-                #     self.active_long_closing_quota[instrument_id] = prec.add(
-                #         self.active_long_closing_quota[instrument_id],
-                #         size,
-                #         instrument.qty_unit,
-                #     )
+                self.active_long_closing_quota[instrument_id] = prec.add(position.long_filled, position.long_outstanding, instrument.qty_unit)
             elif position_side == POSITION_SIDE_LONG_STR:
                 self.active_long_opening_quota[instrument_id] = prec.substract(
                     self.active_long_opening_quota[instrument_id],
                     orig_qty,
                     instrument.qty_unit,
                 )
                 self.active_long_closing_quota[instrument_id] = prec.add(
@@ -248,15 +221,15 @@
         direction = op_info["order_direction"]
         position = self.positions[instrument_id]
         if direction == ORDER_DIRECTION_BUY_STR:
             position.long_outstanding = prec.substract(
                 position.long_outstanding, orig_qty, instrument.qty_unit
             )
             if position_side == POSITION_SIDE_NOTBOTH_STR:
-                self.active_long_closing_quota = prec.add(position.long_filled, position.long_outstanding, instrument.qty_unit)
+                self.active_long_closing_quota[instrument_id] = prec.add(position.long_filled, position.long_outstanding, instrument.qty_unit)
             elif position_side == POSITION_SIDE_LONG_STR:
                 self.active_long_closing_quota[instrument_id] = prec.substract(
                     self.active_long_closing_quota[instrument_id],
                     orig_qty,
                     instrument.qty_unit,
                 )
                 self.active_long_opening_quota[instrument_id] = prec.add(
@@ -312,42 +285,15 @@
         position_side = op_info["position_side"]
         unfilled_qty = prec.substract(org_qty, filled_qty, instrument.qty_unit)
         if op_info["order_direction"] == ORDER_DIRECTION_BUY_STR:
             position.long_outstanding = prec.substract(
                 position.long_outstanding, unfilled_qty, instrument.qty_unit
             )
             if position_side == POSITION_SIDE_NOTBOTH_STR:
-                self.active_long_closing_quota = prec.add(position.long_filled, position.long_outstanding)
-                # size = unfilled_qty
-                # if self.active_short_closing_quota[instrument_id] > 0:
-                #     _update_qty = min(
-                #         self.active_short_closing_quota[instrument_id], size
-                #     )
-                #     self.active_short_closing_quota[instrument_id] = prec.add(
-                #         self.active_short_closing_quota[instrument_id],
-                #         _update_qty,
-                #         instrument.qty_unit,
-                #     )
-                #     self.active_short_opening_quota[instrument_id] = prec.substract(
-                #         self.active_short_opening_quota[instrument_id],
-                #         _update_qty,
-                #         instrument.qty_unit,
-                #     )
-                #     size = prec.substract(size, _update_qty, instrument.qty_unit)
-                # if size > 0:
-                #     self.active_long_closing_quota[instrument_id] = prec.substract(
-                #         self.active_long_closing_quota[instrument_id],
-                #         size,
-                #         instrument.qty_unit,
-                #     )
-                #     self.active_long_opening_quota[instrument_id] = prec.add(
-                #         self.active_long_opening_quota[instrument_id],
-                #         size,
-                #         instrument.qty_unit,
-                #     )
+                self.active_long_closing_quota[instrument_id] = prec.add(position.long_filled, position.long_outstanding, instrument.qty_unit)
             elif position_side == POSITION_SIDE_LONG_STR:
                 self.active_long_closing_quota[instrument_id] = prec.substract(
                     self.active_long_closing_quota[instrument_id],
                     unfilled_qty,
                     instrument.qty_unit,
                 )
                 self.active_long_opening_quota[instrument_id] = prec.add(
@@ -367,42 +313,15 @@
                     instrument.qty_unit,
                 )
         elif op_info["order_direction"] == ORDER_DIRECTION_SELL_STR:
             position.short_outstanding = prec.substract(
                 position.short_outstanding, unfilled_qty, instrument.qty_unit
             )
             if position_side == POSITION_SIDE_NOTBOTH_STR:
-                self.active_short_closing_quota = prec.add(position.short_filled, position.short_outstanding, instrument.qty_unit)
-                # size = unfilled_qty
-                # if self.active_long_closing_quota[instrument_id] > 0:
-                #     _update_qty = min(
-                #         self.active_long_closing_quota[instrument_id], size
-                #     )
-                #     self.active_long_closing_quota[instrument_id] = prec.add(
-                #         self.active_long_closing_quota[instrument_id],
-                #         _update_qty,
-                #         instrument.qty_unit,
-                #     )
-                #     self.active_long_opening_quota[instrument_id] = prec.substract(
-                #         self.active_long_opening_quota[instrument_id],
-                #         _update_qty,
-                #         instrument.qty_unit,
-                #     )
-                #     size = prec.substract(size, _update_qty, instrument.qty_unit)
-                # if size > 0:
-                #     self.active_short_closing_quota[instrument_id] = prec.substract(
-                #         self.active_short_closing_quota[instrument_id],
-                #         size,
-                #         instrument.qty_unit,
-                #     )
-                #     self.active_short_opening_quota[instrument_id] = prec.substract(
-                #         self.active_short_opening_quota[instrument_id],
-                #         size,
-                #         instrument.qty_unit,
-                #     )
+                self.active_short_closing_quota[instrument_id] = prec.add(position.short_filled, position.short_outstanding, instrument.qty_unit)
             elif position_side == POSITION_SIDE_LONG_STR:
                 self.active_long_closing_quota[instrument_id] = prec.add(
                     self.active_long_closing_quota[instrument_id],
                     unfilled_qty,
                     instrument.qty_unit,
                 )
                 self.active_long_opening_quota[instrument_id] = prec.substract(
@@ -546,15 +465,18 @@
         return orders
 
     def sync_position(self):
         """
         同步仓位
         :return: position list
         """
-        positions = self.omsApi.get_all_positions()
+        data = {
+            "id": self.account_id,
+        }
+        positions = self.omsApi.get_all_positions_by_account(data)
         for position in positions["positions"]:
             instrument_id = position["instrument_id"]
             if instrument_id not in self.positions:
                 self.positions[instrument_id] = PositionModule(self.get_instrument(instrument_id).qty_unit)
             self.positions[instrument_id].long_filled = float(
                 position["long_position"]["filled_position"]
             )
```

### Comparing `stsdk-0.3.1.dev1/stsdk/model/strategy_base.py` & `stsdk-0.3.2/stsdk/model/strategy_base.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/model/strategy_module.py` & `stsdk-0.3.2/stsdk/model/strategy_module.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/Stresstest/Stress_klines.py` & `stsdk-0.3.2/stsdk/test/Stresstest/Stress_klines.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/Stresstest/mongoBDtest.py` & `stsdk-0.3.2/stsdk/test/Stresstest/mongoBDtest.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/Stresstest/stressone.py` & `stsdk-0.3.2/stsdk/test/Stresstest/stressone.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/aliyun_log_test.py` & `stsdk-0.3.2/stsdk/test/aliyun_log_test.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/case/order.py` & `stsdk-0.3.2/stsdk/test/case/order.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/create_account.py` & `stsdk-0.3.2/stsdk/test/create_account.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/main.py` & `stsdk-0.3.2/stsdk/test/main.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/metric_test.py` & `stsdk-0.3.2/stsdk/test/metric_test.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/ordertest/CreatePosition.py` & `stsdk-0.3.2/stsdk/test/ordertest/CreatePosition.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/ordertest/GetOrderFormPositionId.py` & `stsdk-0.3.2/stsdk/test/ordertest/GetOrderFormPositionId.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/ordertest/assets/style.css` & `stsdk-0.3.2/stsdk/test/ordertest/assets/style.css`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/ordertest/conftest.py` & `stsdk-0.3.2/stsdk/test/ordertest/conftest.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/ordertest/initialization.py` & `stsdk-0.3.2/stsdk/test/ordertest/initialization.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/ordertest/placeOrder.py` & `stsdk-0.3.2/stsdk/test/ordertest/placeOrder.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/ordertest/position_test.py` & `stsdk-0.3.2/stsdk/test/ordertest/position_test.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/ordertest/reports/assets/style.css` & `stsdk-0.3.2/stsdk/test/ordertest/reports/assets/style.css`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/ordertest/stagegymoduletest.py` & `stsdk-0.3.2/stsdk/test/ordertest/stagegymoduletest.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/ordertest/test_Kline.py` & `stsdk-0.3.2/stsdk/test/ordertest/test_Kline.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/ordertest/test_cancel_all_outstanding_orders.py` & `stsdk-0.3.2/stsdk/test/ordertest/test_cancel_all_outstanding_orders.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/ordertest/test_change_leverage.py` & `stsdk-0.3.2/stsdk/test/ordertest/test_change_leverage.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/ordertest/test_close_all_positions.py` & `stsdk-0.3.2/stsdk/test/ordertest/test_close_all_positions.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/ordertest/test_get_all_outstanding_orders.py` & `stsdk-0.3.2/stsdk/test/ordertest/test_get_all_outstanding_orders.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/ordertest/test_order_closed_loop.py` & `stsdk-0.3.2/stsdk/test/ordertest/test_order_closed_loop.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/ordertest/test_order_empty_multiple.py` & `stsdk-0.3.2/stsdk/test/ordertest/test_order_empty_multiple.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/ordertest/test_position_model.py` & `stsdk-0.3.2/stsdk/test/ordertest/test_position_model.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/place_order_signal.py` & `stsdk-0.3.2/stsdk/test/place_order_signal.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/precision_speed_compare.py` & `stsdk-0.3.2/stsdk/test/precision_speed_compare.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/redis_pubsub_test.py` & `stsdk-0.3.2/stsdk/test/redis_pubsub_test.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/signal_order.py` & `stsdk-0.3.2/stsdk/test/signal_order.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/st_2.py` & `stsdk-0.3.2/stsdk/test/st_2.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/st_demo_1.py` & `stsdk-0.3.2/stsdk/test/st_demo_1.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/test/test_placeorder.py` & `stsdk-0.3.2/stsdk/test/test_placeorder.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/utils/ali_sls.py` & `stsdk-0.3.2/stsdk/utils/ali_sls.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/utils/cache_manager.py` & `stsdk-0.3.2/stsdk/utils/cache_manager.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/utils/config.py` & `stsdk-0.3.2/stsdk/utils/config.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/utils/consul.py` & `stsdk-0.3.2/stsdk/utils/consul.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/utils/http.py` & `stsdk-0.3.2/stsdk/utils/http.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/utils/instrument_id.py` & `stsdk-0.3.2/stsdk/utils/instrument_id.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/utils/log.py` & `stsdk-0.3.2/stsdk/utils/log.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/utils/metric.py` & `stsdk-0.3.2/stsdk/utils/metric.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/utils/redis_utils.py` & `stsdk-0.3.2/stsdk/utils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/stsdk/utils/websocket.py` & `stsdk-0.3.2/stsdk/utils/websocket.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.3.1.dev1/PKG-INFO` & `stsdk-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stsdk
-Version: 0.3.1.dev1
+Version: 0.3.2
 Summary: this is for at trade strategy module
 Author: stark
 Author-email: yangwang@web3.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


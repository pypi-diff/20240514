# Comparing `tmp/thingsboard-gateway-3.4.6.tar.gz` & `tmp/thingsboard-gateway-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thingsboard-gateway-3.4.6.tar", last modified: Fri Mar 22 14:18:46 2024, max compression
+gzip compressed data, was "thingsboard-gateway-3.5.tar", last modified: Tue May 14 13:10:36 2024, max compression
```

## Comparing `thingsboard-gateway-3.4.6.tar` & `thingsboard-gateway-3.5.tar`

### file list

```diff
@@ -1,257 +1,243 @@
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.808905 thingsboard-gateway-3.4.6/
--rw-r--r--   0 imbeacon   (501) staff       (20)    11357 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/LICENSE
--rw-r--r--   0 imbeacon   (501) staff       (20)       49 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/MANIFEST.in
--rw-r--r--   0 imbeacon   (501) staff       (20)     5915 2024-03-22 14:18:46.808664 thingsboard-gateway-3.4.6/PKG-INFO
--rw-r--r--   0 imbeacon   (501) staff       (20)     4967 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/README.md
--rw-r--r--   0 imbeacon   (501) staff       (20)       38 2024-03-22 14:18:46.809043 thingsboard-gateway-3.4.6/setup.cfg
--rw-r--r--   0 imbeacon   (501) staff       (20)     4159 2024-03-22 13:30:16.000000 thingsboard-gateway-3.4.6/setup.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.756093 thingsboard-gateway-3.4.6/tests/
--rw-r--r--   0 imbeacon   (501) staff       (20)        0 2024-02-20 08:45:12.000000 thingsboard-gateway-3.4.6/tests/tests.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.756190 thingsboard-gateway-3.4.6/thingsboard_gateway/
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.761779 thingsboard-gateway-3.4.6/thingsboard_gateway/config/
--rw-r--r--   0 imbeacon   (501) staff       (20)     1435 2023-11-27 06:59:30.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/bacnet.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     2003 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/ble.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     2217 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/can.json
--rw-r--r--   0 imbeacon   (501) staff       (20)      685 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/custom_serial.json
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.764668 thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/
--rw-r--r--   0 imbeacon   (501) staff       (20)     1435 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/bacnet.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     1976 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/ble.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     2217 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/can.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     1304 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/ftp.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     5993 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/modbus.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     4619 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/mqtt.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     1434 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/ocpp.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     1260 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/odbc.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     1302 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/opcua.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     1302 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/opcua_asyncio.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     4199 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/request.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     4609 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/rest.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     3259 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/snmp.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     1187 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/socket.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     1112 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/xmpp.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     1304 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/ftp.json
--rw-r--r--   0 imbeacon   (501) staff       (20)      288 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/list.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     3633 2024-03-22 13:18:49.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/logs.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     5432 2024-03-04 09:50:35.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/modbus.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     1816 2023-11-27 06:59:30.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/modbus_serial.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     4619 2024-03-13 09:00:25.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/mqtt.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     1434 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/ocpp.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     1260 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/odbc.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     1302 2023-12-28 07:04:35.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/opcua.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     4199 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/request.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     4609 2024-01-12 06:48:43.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/rest.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     3259 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/snmp.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     1224 2023-11-16 07:17:29.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/socket.json
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.765251 thingsboard-gateway-3.4.6/thingsboard_gateway/config/statistics/
--rw-r--r--   0 imbeacon   (501) staff       (20)      744 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/statistics/statistics_linux.json
--rw-r--r--   0 imbeacon   (501) staff       (20)      763 2023-09-20 09:16:27.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/statistics/statistics_macos.json
--rw-r--r--   0 imbeacon   (501) staff       (20)      765 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/statistics/statistics_windows.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     1453 2024-03-22 13:18:49.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/tb_gateway.json
--rw-r--r--   0 imbeacon   (501) staff       (20)     1112 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/config/xmpp.json
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.765740 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/__init__.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.767212 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    17354 2024-02-20 08:45:12.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/bacnet_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      811 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/bacnet_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      912 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/bacnet_downlink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2878 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/bacnet_uplink_converter.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.767761 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/bacnet_utilities/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/bacnet_utilities/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    10784 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/bacnet_utilities/tb_gateway_bacnet_application.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      834 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/bacnet_utilities/tb_gateway_bacnet_device.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.769033 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ble/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ble/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     7306 2024-02-20 08:45:12.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ble/ble_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      806 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ble/ble_uplink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     3786 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ble/bytes_ble_uplink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    14115 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ble/device.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      516 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ble/error_handler.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2477 2023-09-20 09:16:27.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ble/hex_bytes_ble_uplink_converter.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.770660 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/can/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/can/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     3233 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/can/bytes_can_downlink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     3618 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/can/bytes_can_uplink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    32537 2024-02-20 08:45:12.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/can/can_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      787 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/can/can_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     1631 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      748 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/converter.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.772442 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ftp/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ftp/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2002 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ftp/file.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    13581 2024-02-20 08:45:12.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ftp/ftp_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      799 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ftp/ftp_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    11140 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ftp/ftp_uplink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     5603 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ftp/path.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.775112 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/modbus/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/modbus/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     3627 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/modbus/backward_compability_adapter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     6559 2024-02-20 08:45:12.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/modbus/bytes_modbus_downlink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     9796 2024-02-29 10:35:17.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/modbus/bytes_modbus_uplink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2049 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/modbus/constants.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    40000 2024-03-01 06:19:15.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/modbus/modbus_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      802 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/modbus/modbus_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     5284 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/modbus/slave.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.777080 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/mqtt/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/mqtt/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2768 2024-03-18 10:04:16.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/mqtt/bytes_mqtt_uplink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     7477 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/mqtt/json_mqtt_uplink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    49791 2024-03-04 09:45:42.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/mqtt/mqtt_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      436 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/mqtt/mqtt_decorators.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      807 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/mqtt/mqtt_uplink_converter.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.778370 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ocpp/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ocpp/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     4313 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ocpp/charge_point.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    13376 2024-02-20 08:45:12.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ocpp/ocpp_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      800 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ocpp/ocpp_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     6571 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ocpp/ocpp_uplink_converter.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.779517 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/odbc/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/odbc/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    23728 2024-02-20 08:45:12.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/odbc/odbc_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      788 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/odbc/odbc_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2452 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/odbc/odbc_uplink_converter.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.780156 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    41785 2024-03-22 13:18:49.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua/opcua_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      813 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua/opcua_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     3170 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua/opcua_uplink_converter.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.781098 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua_asyncio/
--rw-r--r--   0 imbeacon   (501) staff       (20)        0 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua_asyncio/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2002 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua_asyncio/device.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    26011 2024-03-22 13:18:49.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua_asyncio/opcua_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      800 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua_asyncio/opcua_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     3109 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua_asyncio/opcua_uplink_converter.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.782644 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/request/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/request/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     3691 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/request/json_request_downlink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     6985 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/request/json_request_uplink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    15594 2024-02-20 08:45:12.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/request/request_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      803 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/request/request_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      810 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/request/request_uplink_converter.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.784966 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/rest/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/rest/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     3332 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/rest/json_rest_downlink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     6562 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/rest/json_rest_uplink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    29030 2024-02-26 12:51:11.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/rest/rest_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      765 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/rest/rest_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2610 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/rest/ssl_generator.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.785954 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/snmp/
--rw-r--r--   0 imbeacon   (501) staff       (20)      626 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/snmp/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    13067 2024-02-20 08:45:12.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/snmp/snmp_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     1093 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/snmp/snmp_downlink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2331 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/snmp/snmp_uplink_converter.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.788049 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/socket/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/socket/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2794 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/socket/bytes_socket_uplink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    19528 2024-03-22 13:18:49.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/socket/socket_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      436 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/socket/socket_decorators.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      809 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/socket/socket_uplink_converter.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.789226 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/xmpp/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/xmpp/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      355 2023-11-16 08:13:05.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/xmpp/device.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    11421 2024-02-20 08:45:12.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/xmpp/xmpp_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      799 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/xmpp/xmpp_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     7798 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/xmpp/xmpp_uplink_converter.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.789475 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/__init__.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.789826 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/bacnet/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/bacnet/__init__.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.790053 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/ble/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/ble/__init__.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.790325 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/can/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/can/__init__.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.790454 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/ftp/
--rw-r--r--   0 imbeacon   (501) staff       (20)        0 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/ftp/__init__.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.790542 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/modbus/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/modbus/__init__.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.790954 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/mqtt/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/mqtt/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2741 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/mqtt/custom_mqtt_uplink_converter.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.791101 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/ocpp/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/ocpp/__init__.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.791334 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/odbc/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/odbc/__init__.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.791466 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/opcua/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/opcua/__init__.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.791598 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/opcua_asyncio/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/opcua_asyncio/__init__.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.792053 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/request/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/request/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     3682 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/request/custom_request_uplink_converter.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.792194 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/rest/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/rest/__init__.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.793030 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/serial/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/serial/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    11307 2024-03-08 12:50:36.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/serial/custom_serial_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2454 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/serial/custom_serial_converter.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.793326 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/snmp/
--rw-r--r--   0 imbeacon   (501) staff       (20)      618 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/snmp/__init__.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.793623 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/socket/
--rw-r--r--   0 imbeacon   (501) staff       (20)      635 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/socket/__init__.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.793897 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/xmpp/
--rw-r--r--   0 imbeacon   (501) staff       (20)      635 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/xmpp/__init__.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.796690 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    24803 2023-09-20 09:16:27.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/configuration_wizard.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     1148 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/constant_enums.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2111 2024-02-20 09:36:15.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/constants.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      958 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/device_filter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     5853 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/duplicate_detector.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.798726 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/grpc_service/
--rw-r--r--   0 imbeacon   (501) staff       (20)        0 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/grpc_service/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2597 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/grpc_service/grpc_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     8579 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/grpc_service/grpc_downlink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     4713 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/grpc_service/grpc_uplink_converter.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    14664 2024-02-20 08:45:12.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/grpc_service/tb_grpc_manager.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2610 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/grpc_service/tb_grpc_server.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     1916 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/hot_reloader.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.799625 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/proto/
--rw-r--r--   0 imbeacon   (501) staff       (20)     1093 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/proto/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    12267 2024-01-12 06:49:09.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/proto/messages_pb2.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2542 2024-01-09 06:59:03.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/proto/messages_pb2_grpc.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.800471 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/shell/
--rw-r--r--   0 imbeacon   (501) staff       (20)        0 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/shell/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2507 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/shell/proxy.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     6932 2023-12-12 13:17:33.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/shell/shell.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     5060 2024-03-18 13:16:35.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/statistics_service.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    13423 2024-03-20 06:34:22.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/tb_client.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    85894 2024-03-22 13:18:49.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/tb_gateway_service.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.801135 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     1205 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/event_storage.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.802863 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/file/
--rw-r--r--   0 imbeacon   (501) staff       (20)        0 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/file/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      977 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/file/event_storage_files.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     8869 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/file/event_storage_reader.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     1115 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/file/event_storage_reader_pointer.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     5573 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/file/event_storage_writer.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     4123 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/file/file_event_storage.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     1459 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/file/file_event_storage_settings.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.803467 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/memory/
--rw-r--r--   0 imbeacon   (501) staff       (20)        0 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/memory/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2090 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/memory/memory_event_storage.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.805843 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/sqlite/
--rw-r--r--   0 imbeacon   (501) staff       (20)        0 2023-08-13 06:57:06.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/sqlite/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     4382 2024-02-20 08:45:12.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/sqlite/database.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      763 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/sqlite/database_action_type.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     2581 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/sqlite/database_connector.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      951 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/sqlite/database_request.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     3106 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/sqlite/sqlite_event_storage.py
--rw-r--r--   0 imbeacon   (501) staff       (20)      908 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/storage/sqlite/storage_settings.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     1319 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/tb_gateway.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.808019 thingsboard-gateway-3.4.6/thingsboard_gateway/tb_utility/
--rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/tb_utility/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    36127 2024-03-22 13:18:49.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/tb_utility/tb_gateway_remote_configurator.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     6217 2024-03-20 09:06:58.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/tb_utility/tb_handler.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     3582 2024-02-29 06:45:48.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/tb_utility/tb_loader.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     3914 2024-02-29 13:35:24.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/tb_utility/tb_logger.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     5039 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/tb_utility/tb_remote_shell.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     4327 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/tb_utility/tb_updater.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    11257 2024-02-13 14:02:31.000000 thingsboard-gateway-3.4.6/thingsboard_gateway/tb_utility/tb_utility.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-03-22 14:18:46.808362 thingsboard-gateway-3.4.6/thingsboard_gateway.egg-info/
--rw-r--r--   0 imbeacon   (501) staff       (20)     5915 2024-03-22 14:18:46.000000 thingsboard-gateway-3.4.6/thingsboard_gateway.egg-info/PKG-INFO
--rw-r--r--   0 imbeacon   (501) staff       (20)    10636 2024-03-22 14:18:46.000000 thingsboard-gateway-3.4.6/thingsboard_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 imbeacon   (501) staff       (20)        1 2024-03-22 14:18:46.000000 thingsboard-gateway-3.4.6/thingsboard_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 imbeacon   (501) staff       (20)      221 2024-03-22 14:18:46.000000 thingsboard-gateway-3.4.6/thingsboard_gateway.egg-info/entry_points.txt
--rw-r--r--   0 imbeacon   (501) staff       (20)      218 2024-03-22 14:18:46.000000 thingsboard-gateway-3.4.6/thingsboard_gateway.egg-info/requires.txt
--rw-r--r--   0 imbeacon   (501) staff       (20)       20 2024-03-22 14:18:46.000000 thingsboard-gateway-3.4.6/thingsboard_gateway.egg-info/top_level.txt
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.922284 thingsboard-gateway-3.5/
+-rw-r--r--   0 imbeacon   (501) staff       (20)    11357 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/LICENSE
+-rw-r--r--   0 imbeacon   (501) staff       (20)       49 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/MANIFEST.in
+-rw-r--r--   0 imbeacon   (501) staff       (20)     5913 2024-05-14 13:10:36.922016 thingsboard-gateway-3.5/PKG-INFO
+-rw-r--r--   0 imbeacon   (501) staff       (20)     4967 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/README.md
+-rw-r--r--   0 imbeacon   (501) staff       (20)       38 2024-05-14 13:10:36.922328 thingsboard-gateway-3.5/setup.cfg
+-rw-r--r--   0 imbeacon   (501) staff       (20)     4198 2024-05-14 13:10:10.000000 thingsboard-gateway-3.5/setup.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.877711 thingsboard-gateway-3.5/tests/
+-rw-r--r--   0 imbeacon   (501) staff       (20)        0 2024-02-20 08:45:12.000000 thingsboard-gateway-3.5/tests/tests.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.878332 thingsboard-gateway-3.5/thingsboard_gateway/
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.884733 thingsboard-gateway-3.5/thingsboard_gateway/config/
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1435 2023-11-27 06:59:30.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/bacnet.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2003 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/ble.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2217 2024-05-07 07:57:10.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/can.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)      685 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/custom_serial.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1304 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/ftp.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)      288 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/list.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)     3633 2024-03-22 13:18:49.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/logs.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)     5432 2024-03-04 09:50:35.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/modbus.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1816 2023-11-27 06:59:30.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/modbus_serial.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)     4619 2024-03-13 09:00:25.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/mqtt.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1434 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/ocpp.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1260 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/odbc.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1302 2023-12-28 07:04:35.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/opcua.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)     4199 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/request.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)     4609 2024-01-12 06:48:43.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/rest.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)     3259 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/snmp.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1224 2023-11-16 07:17:29.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/socket.json
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.885216 thingsboard-gateway-3.5/thingsboard_gateway/config/statistics/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      744 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/statistics/statistics_linux.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)      763 2023-09-20 09:16:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/statistics/statistics_macos.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)      765 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/statistics/statistics_windows.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1453 2024-05-07 07:57:10.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/tb_gateway.json
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1112 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/config/xmpp.json
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.885808 thingsboard-gateway-3.5/thingsboard_gateway/connectors/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/__init__.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.887296 thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    17456 2024-05-14 09:06:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/bacnet_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      811 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/bacnet_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      912 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/bacnet_downlink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2878 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/bacnet_uplink_converter.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.887848 thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/bacnet_utilities/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/bacnet_utilities/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    10784 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/bacnet_utilities/tb_gateway_bacnet_application.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      834 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/bacnet_utilities/tb_gateway_bacnet_device.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.889141 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ble/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ble/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     7537 2024-05-14 09:06:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ble/ble_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      806 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ble/ble_uplink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     3786 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ble/bytes_ble_uplink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    14164 2024-05-13 06:00:24.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ble/device.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      516 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ble/error_handler.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2477 2023-09-20 09:16:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ble/hex_bytes_ble_uplink_converter.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.890175 thingsboard-gateway-3.5/thingsboard_gateway/connectors/can/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/can/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     3233 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/can/bytes_can_downlink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     3618 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/can/bytes_can_uplink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    32639 2024-05-14 09:06:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/can/can_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      787 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/can/can_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1631 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      748 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/converter.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.891977 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ftp/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ftp/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2002 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ftp/file.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    13684 2024-05-14 09:06:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ftp/ftp_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      799 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ftp/ftp_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    11140 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ftp/ftp_uplink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     5603 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ftp/path.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.894240 thingsboard-gateway-3.5/thingsboard_gateway/connectors/modbus/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/modbus/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     3627 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/modbus/backward_compability_adapter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     6559 2024-02-20 08:45:12.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/modbus/bytes_modbus_downlink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     9796 2024-02-29 10:35:17.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/modbus/bytes_modbus_uplink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2049 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/modbus/constants.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    40195 2024-05-14 09:06:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/modbus/modbus_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      802 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/modbus/modbus_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     5284 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/modbus/slave.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.896284 thingsboard-gateway-3.5/thingsboard_gateway/connectors/mqtt/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/mqtt/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     5462 2024-04-09 11:57:25.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/mqtt/backward_compatibility_adapter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2799 2024-04-09 11:57:25.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/mqtt/bytes_mqtt_uplink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     7567 2024-04-09 11:57:25.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/mqtt/json_mqtt_uplink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    49846 2024-05-14 09:06:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/mqtt/mqtt_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      436 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/mqtt/mqtt_decorators.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      807 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/mqtt/mqtt_uplink_converter.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.897401 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ocpp/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ocpp/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     4313 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ocpp/charge_point.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    13477 2024-05-14 09:06:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ocpp/ocpp_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      800 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ocpp/ocpp_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     6571 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/ocpp/ocpp_uplink_converter.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.898322 thingsboard-gateway-3.5/thingsboard_gateway/connectors/odbc/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/odbc/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    23830 2024-05-14 09:06:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/odbc/odbc_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      788 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/odbc/odbc_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2452 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/odbc/odbc_uplink_converter.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.899203 thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    41923 2024-05-14 09:06:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua/opcua_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      813 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua/opcua_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     3170 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua/opcua_uplink_converter.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.900073 thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua_asyncio/
+-rw-r--r--   0 imbeacon   (501) staff       (20)        0 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua_asyncio/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2002 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua_asyncio/device.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    26442 2024-05-14 09:06:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua_asyncio/opcua_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      800 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua_asyncio/opcua_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     3109 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua_asyncio/opcua_uplink_converter.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.901219 thingsboard-gateway-3.5/thingsboard_gateway/connectors/request/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/request/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     3691 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/request/json_request_downlink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     6985 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/request/json_request_uplink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    15696 2024-05-14 09:06:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/request/request_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      803 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/request/request_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      810 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/request/request_uplink_converter.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.902529 thingsboard-gateway-3.5/thingsboard_gateway/connectors/rest/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/rest/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     3332 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/rest/json_rest_downlink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     6562 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/rest/json_rest_uplink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    29133 2024-05-14 09:06:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/rest/rest_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      765 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/rest/rest_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2610 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/rest/ssl_generator.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.903347 thingsboard-gateway-3.5/thingsboard_gateway/connectors/snmp/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      626 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/snmp/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    13170 2024-04-25 09:00:16.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/snmp/snmp_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1093 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/snmp/snmp_downlink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2331 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/snmp/snmp_uplink_converter.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.904299 thingsboard-gateway-3.5/thingsboard_gateway/connectors/socket/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/socket/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2794 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/socket/bytes_socket_uplink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    19631 2024-05-14 09:06:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/socket/socket_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      436 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/socket/socket_decorators.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      809 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/socket/socket_uplink_converter.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.905223 thingsboard-gateway-3.5/thingsboard_gateway/connectors/xmpp/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/xmpp/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      355 2023-11-16 08:13:05.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/xmpp/device.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    11524 2024-05-14 09:06:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/xmpp/xmpp_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      799 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/xmpp/xmpp_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     7798 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/connectors/xmpp/xmpp_uplink_converter.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.905420 thingsboard-gateway-3.5/thingsboard_gateway/extensions/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/__init__.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.905668 thingsboard-gateway-3.5/thingsboard_gateway/extensions/bacnet/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/bacnet/__init__.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.905795 thingsboard-gateway-3.5/thingsboard_gateway/extensions/ble/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/ble/__init__.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.905931 thingsboard-gateway-3.5/thingsboard_gateway/extensions/can/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/can/__init__.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.906064 thingsboard-gateway-3.5/thingsboard_gateway/extensions/ftp/
+-rw-r--r--   0 imbeacon   (501) staff       (20)        0 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/ftp/__init__.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.906151 thingsboard-gateway-3.5/thingsboard_gateway/extensions/modbus/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/modbus/__init__.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.906419 thingsboard-gateway-3.5/thingsboard_gateway/extensions/mqtt/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/mqtt/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2741 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/mqtt/custom_mqtt_uplink_converter.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.906560 thingsboard-gateway-3.5/thingsboard_gateway/extensions/ocpp/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/ocpp/__init__.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.906705 thingsboard-gateway-3.5/thingsboard_gateway/extensions/odbc/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/odbc/__init__.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.906849 thingsboard-gateway-3.5/thingsboard_gateway/extensions/opcua/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/opcua/__init__.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.906990 thingsboard-gateway-3.5/thingsboard_gateway/extensions/opcua_asyncio/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/opcua_asyncio/__init__.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.907256 thingsboard-gateway-3.5/thingsboard_gateway/extensions/request/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/request/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     3682 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/request/custom_request_uplink_converter.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.907388 thingsboard-gateway-3.5/thingsboard_gateway/extensions/rest/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/rest/__init__.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.908006 thingsboard-gateway-3.5/thingsboard_gateway/extensions/serial/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/serial/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    11409 2024-05-14 09:06:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/serial/custom_serial_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2454 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/serial/custom_serial_converter.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.908170 thingsboard-gateway-3.5/thingsboard_gateway/extensions/snmp/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      618 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/snmp/__init__.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.908318 thingsboard-gateway-3.5/thingsboard_gateway/extensions/socket/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      635 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/socket/__init__.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.908466 thingsboard-gateway-3.5/thingsboard_gateway/extensions/xmpp/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      635 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/extensions/xmpp/__init__.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.910833 thingsboard-gateway-3.5/thingsboard_gateway/gateway/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    24803 2023-09-20 09:16:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/configuration_wizard.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1148 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/constant_enums.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2111 2024-02-20 09:36:15.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/constants.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      958 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/device_filter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     5853 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/duplicate_detector.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.912819 thingsboard-gateway-3.5/thingsboard_gateway/gateway/grpc_service/
+-rw-r--r--   0 imbeacon   (501) staff       (20)        0 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/grpc_service/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2597 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/grpc_service/grpc_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     8579 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/grpc_service/grpc_downlink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     4713 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/grpc_service/grpc_uplink_converter.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    14664 2024-02-20 08:45:12.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/grpc_service/tb_grpc_manager.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2610 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/grpc_service/tb_grpc_server.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1916 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/hot_reloader.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.913608 thingsboard-gateway-3.5/thingsboard_gateway/gateway/proto/
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1093 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/proto/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    12267 2024-01-12 06:49:09.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/proto/messages_pb2.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2542 2024-01-09 06:59:03.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/proto/messages_pb2_grpc.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.914196 thingsboard-gateway-3.5/thingsboard_gateway/gateway/shell/
+-rw-r--r--   0 imbeacon   (501) staff       (20)        0 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/shell/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2507 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/shell/proxy.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     6932 2023-12-12 13:17:33.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/shell/shell.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     5060 2024-03-18 13:16:35.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/statistics_service.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    13491 2024-05-14 13:10:10.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/tb_client.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    86706 2024-05-14 09:15:37.000000 thingsboard-gateway-3.5/thingsboard_gateway/gateway/tb_gateway_service.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.914823 thingsboard-gateway-3.5/thingsboard_gateway/storage/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1205 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/event_storage.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.917006 thingsboard-gateway-3.5/thingsboard_gateway/storage/file/
+-rw-r--r--   0 imbeacon   (501) staff       (20)        0 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/file/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      977 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/file/event_storage_files.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     8869 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/file/event_storage_reader.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1115 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/file/event_storage_reader_pointer.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     5573 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/file/event_storage_writer.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     4123 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/file/file_event_storage.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1459 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/file/file_event_storage_settings.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.917251 thingsboard-gateway-3.5/thingsboard_gateway/storage/memory/
+-rw-r--r--   0 imbeacon   (501) staff       (20)        0 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/memory/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2090 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/memory/memory_event_storage.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.918623 thingsboard-gateway-3.5/thingsboard_gateway/storage/sqlite/
+-rw-r--r--   0 imbeacon   (501) staff       (20)        0 2023-08-13 06:57:06.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/sqlite/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     4382 2024-02-20 08:45:12.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/sqlite/database.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      763 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/sqlite/database_action_type.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     2581 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/sqlite/database_connector.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      951 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/sqlite/database_request.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     3106 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/sqlite/sqlite_event_storage.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      908 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/storage/sqlite/storage_settings.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1319 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/tb_gateway.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.921167 thingsboard-gateway-3.5/thingsboard_gateway/tb_utility/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      616 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/tb_utility/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    36305 2024-05-14 13:10:10.000000 thingsboard-gateway-3.5/thingsboard_gateway/tb_utility/tb_gateway_remote_configurator.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     6228 2024-04-25 09:00:16.000000 thingsboard-gateway-3.5/thingsboard_gateway/tb_utility/tb_handler.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     3582 2024-02-29 06:45:48.000000 thingsboard-gateway-3.5/thingsboard_gateway/tb_utility/tb_loader.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     4998 2024-05-14 09:06:27.000000 thingsboard-gateway-3.5/thingsboard_gateway/tb_utility/tb_logger.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     5039 2024-02-13 14:02:31.000000 thingsboard-gateway-3.5/thingsboard_gateway/tb_utility/tb_remote_shell.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     4399 2024-05-14 13:10:10.000000 thingsboard-gateway-3.5/thingsboard_gateway/tb_utility/tb_updater.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    11418 2024-04-11 10:27:16.000000 thingsboard-gateway-3.5/thingsboard_gateway/tb_utility/tb_utility.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)      632 2024-05-14 13:10:10.000000 thingsboard-gateway-3.5/thingsboard_gateway/version.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-14 13:10:36.921605 thingsboard-gateway-3.5/thingsboard_gateway.egg-info/
+-rw-r--r--   0 imbeacon   (501) staff       (20)     5913 2024-05-14 13:10:36.000000 thingsboard-gateway-3.5/thingsboard_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 imbeacon   (501) staff       (20)     9926 2024-05-14 13:10:36.000000 thingsboard-gateway-3.5/thingsboard_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 imbeacon   (501) staff       (20)        1 2024-05-14 13:10:36.000000 thingsboard-gateway-3.5/thingsboard_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 imbeacon   (501) staff       (20)      221 2024-05-14 13:10:36.000000 thingsboard-gateway-3.5/thingsboard_gateway.egg-info/entry_points.txt
+-rw-r--r--   0 imbeacon   (501) staff       (20)      220 2024-05-14 13:10:36.000000 thingsboard-gateway-3.5/thingsboard_gateway.egg-info/requires.txt
+-rw-r--r--   0 imbeacon   (501) staff       (20)       20 2024-05-14 13:10:36.000000 thingsboard-gateway-3.5/thingsboard_gateway.egg-info/top_level.txt
```

### Comparing `thingsboard-gateway-3.4.6/LICENSE` & `thingsboard-gateway-3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/PKG-INFO` & `thingsboard-gateway-3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: thingsboard-gateway
-Version: 3.4.6
+Version: 3.5
 Summary: Thingsboard Gateway for IoT devices.
 Home-page: https://github.com/thingsboard/thingsboard-gateway
-Download-URL: https://github.com/thingsboard/thingsboard-gateway/archive/3.4.6.tar.gz
+Download-URL: https://github.com/thingsboard/thingsboard-gateway/archive/3.5.tar.gz
 Author: ThingsBoard
 Author-email: info@thingsboard.io
 License: Apache Software License (Apache Software License 2.0)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cryptography==3.4.*
@@ -21,15 +21,15 @@
 Requires-Dist: questionary
 Requires-Dist: pyfiglet
 Requires-Dist: termcolor
 Requires-Dist: mmh3
 Requires-Dist: grpcio==1.58.0
 Requires-Dist: protobuf
 Requires-Dist: cachetools
-Requires-Dist: tb-mqtt-client>=1.5
+Requires-Dist: tb-mqtt-client>=1.9.1
 Requires-Dist: packaging==23.1
 Requires-Dist: service-identity
 
 # ThingsBoard IoT Gateway  
 
 The Thingsboard **IoT Gateway** is an open-source solution that allows you to integrate devices connected to legacy and third-party systems with Thingsboard.
```

### Comparing `thingsboard-gateway-3.4.6/README.md` & `thingsboard-gateway-3.5/README.md`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/setup.py` & `thingsboard-gateway-3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,22 @@
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
 from setuptools import setup
 from os import path
 
+from thingsboard_gateway import version
 
 current_directory = path.abspath(path.dirname(__file__))
 with open(path.join(current_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
-VERSION = "3.4.6"
-
 setup(
-    version=VERSION,
+    version=version.VERSION,
     name="thingsboard-gateway",
     author="ThingsBoard",
     author_email="info@thingsboard.io",
     license="Apache Software License (Apache Software License 2.0)",
     description="Thingsboard Gateway for IoT devices.",
     url="https://github.com/thingsboard/thingsboard-gateway",
     long_description=long_description,
@@ -65,19 +64,19 @@
         'questionary',
         'pyfiglet',
         'termcolor',
         'mmh3',
         'grpcio==1.58.0',
         'protobuf',
         'cachetools',
-        'tb-mqtt-client>=1.5',
+        'tb-mqtt-client>=1.9.1',
         'packaging==23.1',
         'service-identity'
     ],
-    download_url='https://github.com/thingsboard/thingsboard-gateway/archive/%s.tar.gz' % VERSION,
+    download_url='https://github.com/thingsboard/thingsboard-gateway/archive/%s.tar.gz' % version.VERSION,
     entry_points={
         'console_scripts': [
             'thingsboard-gateway = thingsboard_gateway.tb_gateway:daemon',
             'tb-gateway-configurator = thingsboard_gateway.gateway.configuration_wizard:configure',
             'tb-gateway-shell = thingsboard_gateway.gateway.shell:main'
         ]
     })
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/bacnet.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/bacnet.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/ble.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/ble.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/can.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/can.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/custom_serial.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/custom_serial.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/ftp.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/ftp.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/modbus.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/modbus.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988307823129252%*

 * *Differences: {"'master'": "{'slaves': {0: {'attributes': {delete: [5, 2]}, 'timeseries': {delete: [0]}}}}"}*

```diff
@@ -23,21 +23,14 @@
                         "address": 5,
                         "functionCode": 4,
                         "objectsCount": 1,
                         "tag": "bits_read",
                         "type": "bits"
                     },
                     {
-                        "address": 6,
-                        "functionCode": 4,
-                        "objectsCount": 1,
-                        "tag": "8int_read",
-                        "type": "8int"
-                    },
-                    {
                         "address": 7,
                         "functionCode": 4,
                         "objectsCount": 1,
                         "tag": "16int_read",
                         "type": "16int"
                     },
                     {
@@ -45,22 +38,14 @@
                         "divider": 10,
                         "functionCode": 4,
                         "objectsCount": 2,
                         "tag": "32int_read_divider",
                         "type": "32int"
                     },
                     {
-                        "address": 10,
-                        "functionCode": 4,
-                        "multiplier": 10,
-                        "objectsCount": 1,
-                        "tag": "8int_read_multiplier",
-                        "type": "8int"
-                    },
-                    {
                         "address": 11,
                         "functionCode": 4,
                         "objectsCount": 2,
                         "tag": "32int_read",
                         "type": "32int"
                     },
                     {
@@ -112,21 +97,14 @@
                         "type": "32int"
                     }
                 ],
                 "sendDataOnlyOnChange": true,
                 "timeout": 35,
                 "timeseries": [
                     {
-                        "address": 17,
-                        "functionCode": 4,
-                        "objectsCount": 1,
-                        "tag": "8uint_read",
-                        "type": "8uint"
-                    },
-                    {
                         "address": 18,
                         "functionCode": 4,
                         "objectsCount": 2,
                         "tag": "16uint_read",
                         "type": "16uint"
                     },
                     {
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/mqtt.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/mqtt.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/ocpp.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/ocpp.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/odbc.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/odbc.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/opcua.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/opcua.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/opcua_asyncio.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/xmpp.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.25%*

 * *Differences: {"'devices'": "[OrderedDict([('jid', 'device@localhost/TMP_1101'), ('deviceNameExpression', "*

 * *              "'${serialNumber}'), ('deviceTypeExpression', 'default'), ('attributes', "*

 * *              "[OrderedDict([('key', 'temperature'), ('value', '${temp}')])]), ('timeseries', "*

 * *              "[OrderedDict([('key', 'humidity'), ('value', '${hum}')]), OrderedDict([('key', "*

 * *              "'combination'), ('value', '${temp}:${hum}')])]), ('attributeUpdates', "*

 * *              "[OrderedDict([('attributeOnThingsBo […]*

```diff
@@ -1,52 +1,53 @@
 {
+    "devices": [
+        {
+            "attributeUpdates": [
+                {
+                    "attributeOnThingsBoard": "shared",
+                    "valueExpression": "{\"${attributeKey}\":\"${attributeValue}\"}"
+                }
+            ],
+            "attributes": [
+                {
+                    "key": "temperature",
+                    "value": "${temp}"
+                }
+            ],
+            "deviceNameExpression": "${serialNumber}",
+            "deviceTypeExpression": "default",
+            "jid": "device@localhost/TMP_1101",
+            "serverSideRpc": [
+                {
+                    "methodRPC": "rpc1",
+                    "valueExpression": "${params}",
+                    "withResponse": true
+                }
+            ],
+            "timeseries": [
+                {
+                    "key": "humidity",
+                    "value": "${hum}"
+                },
+                {
+                    "key": "combination",
+                    "value": "${temp}:${hum}"
+                }
+            ]
+        }
+    ],
     "server": {
-        "disableSubscriptions": false,
-        "identity": {
-            "type": "anonymous"
-        },
-        "mapping": [
-            {
-                "attributes": [
-                    {
-                        "key": "temperature \u00b0C",
-                        "path": "${ns=2;i=5}"
-                    }
-                ],
-                "attributes_updates": [
-                    {
-                        "attributeOnDevice": "Root\\.Objects\\.Device1\\.serialNumber",
-                        "attributeOnThingsBoard": "deviceName"
-                    }
-                ],
-                "deviceNamePattern": "Device ${Root\\.Objects\\.Device1\\.serialNumber}",
-                "deviceNodePattern": "Root\\.Objects\\.Device1",
-                "rpc_methods": [
-                    {
-                        "arguments": [
-                            2,
-                            4
-                        ],
-                        "method": "multiply"
-                    }
-                ],
-                "timeseries": [
-                    {
-                        "key": "humidity",
-                        "path": "${Root\\.Objects\\.Device1\\.TemperatureAndHumiditySensor\\.Humidity}"
-                    },
-                    {
-                        "key": "batteryLevel",
-                        "path": "${Battery\\.batteryLevel}"
-                    }
-                ]
-            }
+        "disable_starttls": false,
+        "force_starttls": true,
+        "host": "localhost",
+        "jid": "gateway@localhost",
+        "password": "password",
+        "plugins": [
+            "xep_0030",
+            "xep_0323",
+            "xep_0325"
         ],
-        "name": "OPC-UA Default Server",
-        "scanPeriodInMillis": 5000,
-        "security": "Basic128Rsa15",
-        "showMap": false,
-        "subCheckPeriodInMillis": 100,
-        "timeoutInMillis": 5000,
-        "url": "localhost:4840/freeopcua/server/"
+        "port": 5222,
+        "timeout": 10000,
+        "use_ssl": false
     }
 }
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/request.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/request.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/rest.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/rest.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/snmp.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/snmp.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/default-configs/socket.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/socket.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8166666666666668%*

 * *Differences: {"'devices'": "{0: {'addressFilter': '127.0.0.1:*', delete: ['address']}}",*

 * * "'name'": "'TCP Connector Example'"}*

```diff
@@ -1,13 +1,13 @@
 {
     "address": "127.0.0.1",
     "bufferSize": 1024,
     "devices": [
         {
-            "address": "127.0.0.1:50001",
+            "addressFilter": "127.0.0.1:*",
             "attributeRequests": [
                 {
                     "attributeNameExpression": "[3:]",
                     "requestExpression": "${[0:3]==atr}",
                     "type": "shared"
                 }
             ],
@@ -50,10 +50,11 @@
                     "byteFrom": 0,
                     "byteTo": 2,
                     "key": "hum"
                 }
             ]
         }
     ],
+    "name": "TCP Connector Example",
     "port": 50000,
     "type": "TCP"
 }
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/logs.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/logs.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/modbus_serial.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/modbus_serial.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/statistics/statistics_linux.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/statistics/statistics_linux.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/statistics/statistics_macos.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/statistics/statistics_macos.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/statistics/statistics_windows.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/statistics/statistics_windows.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/config/tb_gateway.json` & `thingsboard-gateway-3.5/thingsboard_gateway/config/tb_gateway.json`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/bacnet_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/bacnet_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,16 @@
         self.__config = config
         self.__id = self.__config.get('id')
         self.name = config.get('name', 'BACnet ' + ''.join(choice(ascii_lowercase) for _ in range(5)))
         self.__devices = []
         self.__device_indexes = {}
         self.__devices_address_name = {}
         self.__gateway = gateway
-        self._log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'))
+        self._log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'),
+                                enable_remote_logging=self.__config.get('enableRemoteLogging', False))
         self._application = TBBACnetApplication(self, self.__config, self._log)
         self.__bacnet_core_thread = Thread(target=run, name="BACnet core thread", daemon=True,
                                            kwargs={"sigterm": None, "sigusr1": None})
         self.__bacnet_core_thread.start()
         self.__stopped = False
         self.__config_devices = self.__config["devices"]
         self.default_converters = {
@@ -106,15 +107,15 @@
                     thread = Thread(target=self.__convert_and_save_data, args=(self.__convert_and_save_data_queue,),
                                     daemon=True)
                     thread.start()
 
     def close(self):
         self.__stopped = True
         self.__connected = False
-        self._log.reset()
+        self._log.stop()
 
         self._application.mux.directPort.connected = False
         self._application.mux.directPort.accepting = False
         self._application.mux.directPort.connecting = False
         self._application.mux.directPort.del_channel()
         if self._application.mux.directPort.socket is not None:
             try:
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/bacnet_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/bacnet_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/bacnet_downlink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/bacnet_downlink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/bacnet_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/bacnet_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/bacnet_utilities/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/bacnet_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/bacnet_utilities/tb_gateway_bacnet_application.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/bacnet_utilities/tb_gateway_bacnet_application.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/bacnet/bacnet_utilities/tb_gateway_bacnet_device.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/bacnet/bacnet_utilities/tb_gateway_bacnet_device.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ble/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ble/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ble/ble_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ble/ble_connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,16 @@
                            'MessagesSent': 0}
         super().__init__()
         self._connector_type = connector_type
         self.__gateway = gateway
         self.__config = config
         self.__id = self.__config.get('id')
         self.name = self.__config.get("name", 'BLE Connector ' + ''.join(choice(ascii_lowercase) for _ in range(5)))
-        self.__log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'))
+        self.__log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'),
+                                 enable_remote_logging=self.__config.get('enableRemoteLogging', False))
 
         self.daemon = True
 
         self.__stopped = False
         self.__connected = False
 
         if self.__config.get('showMap', False):
@@ -92,17 +93,24 @@
     def run(self):
         self.__connected = True
 
         thread = Thread(target=self.__process_data, daemon=True, name='BLE Process Data Thread')
         thread.start()
 
     def close(self):
+        self.__connected = False
         self.__stopped = True
+
+        for device in self.__devices:
+            device.stop()
+
+        self.__devices = []
+
         self.__log.info('%s has been stopped.', self.get_name())
-        self.__log.reset()
+        self.__log.stop()
 
     def get_name(self):
         return self.name
 
     def get_id(self):
         return self.__id
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ble/ble_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ble/ble_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ble/bytes_ble_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ble/bytes_ble_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ble/device.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ble/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,7 +365,10 @@
         while not task.done():
             sleep(.2)
 
         return task.result().decode('UTF-8')
 
     def __str__(self):
         return f'{self.name}'
+
+    def stop(self):
+        self.stopped = True
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ble/error_handler.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ble/error_handler.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ble/hex_bytes_ble_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ble/hex_bytes_ble_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/can/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/can/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/can/bytes_can_downlink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/can/bytes_can_downlink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/can/bytes_can_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/can/bytes_can_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/can/can_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/can/can_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,16 @@
                            'MessagesSent': 0}
         super().__init__()
         self.name = config.get("name", 'CAN Connector ' + ''.join(choice(ascii_lowercase) for _ in range(5)))
         self.__gateway = gateway
         self._connector_type = connector_type
         self.__config = config
         self.__id = self.__config.get('id')
-        self._log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'))
+        self._log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'),
+                                enable_remote_logging=self.__config.get('enableRemoteLogging', False))
         self.__bus_conf = {}
         self.__bus = None
         self.__reconnect_count = 0
         self.__reconnect_conf = {}
         self.__devices = {}
         self.__nodes = {}
         self.__commands = {}
@@ -96,15 +97,15 @@
         self.__stopped = False
         self.start()
 
     def close(self):
         if not self.__stopped:
             self.__stopped = True
             self._log.debug("[%s] Stopping", self.get_name())
-            self._log.reset()
+            self._log.stop()
 
     def get_name(self):
         return self.name
 
     def get_id(self):
         return self.__id
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/can/can_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/can/can_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/connector.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ftp/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ftp/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ftp/file.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ftp/file.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ftp/ftp_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ftp/ftp_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
         self.__id = self.__config.get('id')
         self._connector_type = connector_type
         self.__gateway = gateway
         self.security = {**self.__config['security']} if self.__config['security']['type'] == 'basic' else {
             'username': 'anonymous', "password": 'anonymous@'}
         self.__tls_support = self.__config.get("TLSSupport", False)
         self.name = self.__config.get("name", "".join(choice(ascii_lowercase) for _ in range(5)))
-        self.__log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'))
+        self.__log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'),
+                                 enable_remote_logging=self.__config.get('enableRemoteLogging', False))
         self.daemon = True
         self.__stopped = False
         self.__requests_in_progress = []
         self.__convert_queue = Queue(1000000)
         self.__attribute_updates = []
         self.__fill_attributes_update()
         self._connected = False
@@ -184,15 +185,15 @@
             self.__gateway.send_to_storage(self.getName(), self.get_id(), converted_data)
             self.statistics['MessagesSent'] = self.statistics['MessagesSent'] + 1
             self.__log.debug("Data to ThingsBoard: %s", converted_data)
 
     def close(self):
         self.__stopped = True
         self.__log.info('FTP Connector stopped.')
-        self.__log.reset()
+        self.__log.stop()
 
     def get_name(self):
         return self.name
 
     def get_id(self):
         return self.__id
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ftp/ftp_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ftp/ftp_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ftp/ftp_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ftp/ftp_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ftp/path.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ftp/path.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/modbus/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/modbus/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/modbus/backward_compability_adapter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/modbus/backward_compability_adapter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/modbus/bytes_modbus_downlink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/modbus/bytes_modbus_downlink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/modbus/bytes_modbus_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/modbus/bytes_modbus_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/modbus/constants.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/modbus/constants.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/modbus/modbus_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/modbus/modbus_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,16 @@
     def __init__(self, gateway, config, connector_type):
         self.statistics = {STATISTIC_MESSAGE_RECEIVED_PARAMETER: 0,
                            STATISTIC_MESSAGE_SENT_PARAMETER: 0}
         super().__init__()
         self.__gateway = gateway
         self._connector_type = connector_type
         self.__log = init_logger(self.__gateway, config.get('name', self.name),
-                                 config.get('logLevel', 'INFO'))
+                                 config.get('logLevel', 'INFO'),
+                                 enable_remote_logging=config.get('enableRemoteLogging', False))
         self.__backward_compatibility_adapter = BackwardCompatibilityAdapter(config, gateway.get_config_path(),
                                                                              logger=self.__log)
         self.__config = self.__backward_compatibility_adapter.convert()
         self.__id = self.__config.get('id')
         self.name = self.__config.get("name", 'Modbus Connector ' + ''.join(choice(ascii_lowercase) for _ in range(5)))
 
         self.__connected = False
@@ -327,23 +328,26 @@
         self.__stop_connections_to_masters()
 
         # Stop all slaves
         for slave in self.__slaves:
             slave.close()
 
         if self.__slave_thread is not None:
-            ServerStop()
+            try:
+                ServerStop()
+            except AttributeError:
+                self.__slave_thread.join()
 
         # Stop all workers
         for worker in self.__workers_thread_pool:
             worker.close()
 
         # self.__slave_thread.join()
         self.__log.info('%s has been stopped.', self.get_name())
-        self.__log.reset()
+        self.__log.stop()
         self.__stopping = False
 
     def get_name(self):
         return self.name
 
     def get_id(self):
         return self.__id
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/modbus/modbus_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/modbus/modbus_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/modbus/slave.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/modbus/slave.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/mqtt/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/mqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/mqtt/bytes_mqtt_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/mqtt/bytes_mqtt_uplink_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
     @StatisticsService.CollectStatistics(start_stat_type='receivedBytesFromDevices',
                                          end_stat_type='convertedBytesFromDevice')
     def convert(self, topic, data):
         datatypes = {"attributes": "attributes",
                      "timeseries": "telemetry"}
         dict_result = {
-            "deviceName": self.parse_data(self.__config['deviceNameExpression'], data),
-            "deviceType": self.parse_data(self.__config['deviceTypeExpression'], data),
+            "deviceName": self.parse_data(self.__config['deviceInfo']['deviceNameExpression'], data),
+            "deviceType": self.parse_data(self.__config['deviceInfo']['deviceProfileExpression'], data),
             "attributes": [],
             "telemetry": []
         }
 
         try:
             for datatype in datatypes:
                 dict_result[datatypes[datatype]] = []
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/mqtt/json_mqtt_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/mqtt/json_mqtt_uplink_converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,35 +106,38 @@
     @staticmethod
     def create_timeseries_record(key, value, timestamp):
         value_item = {key: value}
         return {"ts": timestamp, 'values': value_item} if timestamp else value_item
 
     def parse_device_name(self, topic, data, config):
         return self.parse_device_info(
-            topic, data, config, "deviceNameJsonExpression", "deviceNameTopicExpression")
+            topic, data, config, "deviceNameExpressionSource", "deviceNameExpression")
 
     def parse_device_type(self, topic, data, config):
         return self.parse_device_info(
-            topic, data, config, "deviceTypeJsonExpression", "deviceTypeTopicExpression")
+            topic, data, config, "deviceProfileExpressionSource", "deviceProfileExpression")
 
-    def parse_device_info(self, topic, data, config, json_expression_config_name, topic_expression_config_name):
+    def parse_device_info(self, topic, data, config, expression_source, expression):
         result = None
+        device_info = config.get('deviceInfo', {})
+
+        expression = device_info.get('deviceNameExpression') if expression == 'deviceNameExpression' \
+            else device_info.get('deviceProfileExpression')
+
         try:
-            if config.get(json_expression_config_name) is not None:
-                expression = config.get(json_expression_config_name)
+            if device_info.get(expression_source) == 'message' or device_info.get(expression_source) == 'constant':
                 result_tags = TBUtility.get_values(expression, data, get_tag=True)
                 result_values = TBUtility.get_values(expression, data, expression_instead_none=True)
 
                 result = expression
                 for (result_tag, result_value) in zip(result_tags, result_values):
                     is_valid_key = "${" in expression and "}" in expression
                     result = result.replace('${' + str(result_tag) + '}',
                                             str(result_value)) if is_valid_key else result_tag
-            elif config.get(topic_expression_config_name) is not None:
-                expression = config.get(topic_expression_config_name)
+            elif device_info.get(expression_source) == 'topic':
                 search_result = search(expression, topic)
                 if search_result is not None:
                     result = search_result.group(0)
                 else:
                     self._log.debug(
                         "Regular expression result is None. deviceNameTopicExpression parameter will be interpreted "
                         "as a deviceName\n Topic: %s\nRegex: %s", topic, expression)
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/mqtt/mqtt_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/mqtt/mqtt_connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from queue import Queue
 from re import fullmatch, match, search
 from threading import Thread
 from time import sleep, time
 
 import simplejson
 
+from thingsboard_gateway.connectors.mqtt.backward_compatibility_adapter import BackwardCompatibilityAdapter
 from thingsboard_gateway.gateway.constants import SEND_ON_CHANGE_PARAMETER, DEFAULT_SEND_ON_CHANGE_VALUE, \
     ATTRIBUTES_PARAMETER, TELEMETRY_PARAMETER, SEND_ON_CHANGE_TTL_PARAMETER, DEFAULT_SEND_ON_CHANGE_INFINITE_TTL_VALUE
 from thingsboard_gateway.gateway.constant_enums import Status
 from thingsboard_gateway.connectors.connector import Connector
 from thingsboard_gateway.connectors.mqtt.mqtt_decorators import CustomCollectStatistics
 from thingsboard_gateway.tb_utility.tb_loader import TBModuleLoader
 from thingsboard_gateway.tb_utility.tb_utility import TBUtility
@@ -104,21 +105,33 @@
     CONFIGURATION_KEY_SHARED_ID = "sharedId"
 
     def __init__(self, gateway, config, connector_type):
         super().__init__()
 
         self.__gateway = gateway  # Reference to TB Gateway
         self._connector_type = connector_type  # Should be "mqtt"
-        self.config = config  # mqtt.json contents
+
+        # check if the configuration is in the old format
+        self._using_old_config_format = False
+        if BackwardCompatibilityAdapter.is_old_config_format(config):
+            self._using_old_config_format = True
+            self.config = BackwardCompatibilityAdapter(config).convert()
+        else:
+            self.config = config
+
         self.__id = self.config.get('id')
 
-        self.__log = init_logger(self.__gateway, self.config['name'], self.config.get('logLevel', 'INFO'))
+        self.__log = init_logger(self.__gateway, self.config['name'], self.config.get('logLevel', 'INFO'),
+                                 enable_remote_logging=self.config.get('enableRemoteLogging', False))
         self.statistics = {'MessagesReceived': 0, 'MessagesSent': 0}
         self.__subscribes_sent = {}
 
+        if self._using_old_config_format:
+            self.__log.warning("Old MQTT connector configuration format detected. Automatic conversion is applied.")
+
         # Extract main sections from configuration ---------------------------------------------------------------------
         self.__broker = config.get('broker')
         self.__send_data_only_on_change = self.__broker.get(SEND_ON_CHANGE_PARAMETER, DEFAULT_SEND_ON_CHANGE_VALUE)
         self.__send_data_only_on_change_ttl = self.__broker.get(SEND_ON_CHANGE_TTL_PARAMETER,
                                                                 DEFAULT_SEND_ON_CHANGE_INFINITE_TTL_VALUE)
 
         # for sendDataOnlyOnChange param
@@ -130,24 +143,24 @@
         self.__disconnect_requests = []
         self.__attribute_requests = []
         self.__attribute_updates = []
 
         self.__shared_custom_converters = {}
 
         mandatory_keys = {
-            "mapping": ['topicFilter', 'converter'],
+            "dataMapping": ['topicFilter', 'converter'],
             "serverSideRpc": ['deviceNameFilter', 'methodFilter', 'requestTopicExpression', 'valueExpression'],
             "connectRequests": ['topicFilter'],
             "disconnectRequests": ['topicFilter'],
             "attributeRequests": ['topicFilter', 'topicExpression', 'valueExpression'],
             "attributeUpdates": ['deviceNameFilter', 'attributeFilter', 'topicExpression', 'valueExpression']
         }
 
         # Mappings, i.e., telemetry/attributes-push handlers provided by user via configuration file
-        self.load_handlers('mapping', mandatory_keys['mapping'], self.__mapping)
+        self.load_handlers('dataMapping', mandatory_keys['dataMapping'], self.__mapping)
 
         # RPCs, i.e., remote procedure calls (ThingsBoard towards devices) handlers
         self.load_handlers('serverSideRpc', mandatory_keys['serverSideRpc'], self.__server_side_rpc)
 
         # Connect requests, i.e., telling ThingsBoard that a device is online even if it does not post telemetry
         self.load_handlers('connectRequests', mandatory_keys['connectRequests'], self.__connect_requests)
 
@@ -240,22 +253,19 @@
     def get_type(self):
         return self._connector_type
 
     def get_ttl_for_duplicates(self, device_name):
         return self.__send_data_only_on_change_ttl
 
     def load_handlers(self, handler_flavor, mandatory_keys, accepted_handlers_list):
-        if handler_flavor not in self.config:
+        config = self.config.get(handler_flavor) or self.config.get("requestsMapping", {}).get(handler_flavor)
+
+        if config is None:
             self.__log.warning("'%s' section missing from configuration", handler_flavor)
         else:
-
-            config = self.config.get(handler_flavor, [])
-            if self.config.get("requestsMapping") is not None:
-                config = self.config["requestsMapping"].get(handler_flavor, [])
-
             for handler in config:
                 discard = False
 
                 for key in mandatory_keys:
                     if key not in handler:
                         # Will report all missing fields to user before discarding the entry => no break here
                         discard = True
@@ -275,15 +285,15 @@
 
             self.__log.info("Number of accepted %s handlers: %d",
                             handler_flavor,
                             len(accepted_handlers_list))
 
             self.__log.debug("Number of rejected %s handlers: %d",
                              handler_flavor,
-                             len(self.config.get(handler_flavor)) - len(accepted_handlers_list))
+                             len(config) - len(accepted_handlers_list))
 
     def is_connected(self):
         return self._connected
 
     def is_stopped(self):
         return self.__stopped
 
@@ -313,29 +323,29 @@
         while not self._connected and not self.__stopped:
             try:
                 self._client.connect(self.__broker['host'],
                                      self.__broker.get('port', 1883))
                 self._client.loop_start()
                 if not self._connected:
                     sleep(1)
-            except (ConnectionRefusedError, ConnectionResetError, socket.timeout) as e:
+            except (ConnectionRefusedError, ConnectionResetError, ssl.SSLEOFError, socket.timeout) as e:
                 self.__log.error(e)
                 sleep(10)
 
     def close(self):
         self.__stopped = True
         try:
             self._client.disconnect()
         except Exception as e:
             self.__log.exception(e)
         self._client.loop_stop()
         for worker in self.__workers_thread_pool:
             worker.stop()
         self.__log.info('%s has been stopped.', self.get_name())
-        self.__log.reset()
+        self.__log.stop()
 
     def get_name(self):
         return self.name
 
     def get_id(self):
         return self.__id
 
@@ -519,14 +529,41 @@
             if not worker.in_progress:
                 worker.stopped = True
                 self.__workers_thread_pool.remove(worker)
 
     def _on_message(self, client, userdata, message):
         self._on_message_queue.put((client, userdata, message))
 
+    @staticmethod
+    def _parce_device_info(device_info, topic, content):
+        found_device_name = None
+        found_device_type = 'default'
+
+        # Get device name, either from topic or from content
+        if device_info.get('deviceNameExpressionSource') == 'topic':
+            device_name_match = search(device_info["deviceNameExpression"], topic)
+            if device_name_match is not None:
+                found_device_name = device_name_match.group(0)
+        elif device_info.get('deviceNameExpressionSource') == 'message' or device_info.get(
+                'deviceNameExpression') == 'constant':
+            found_device_name = TBUtility.get_value(device_info["deviceNameExpression"], content,
+                                                    expression_instead_none=True)
+
+        # Get device type (if any), either from topic or from content
+        if device_info.get("deviceProfileExpressionSource") == 'topic':
+            device_type_match = search(device_info["deviceProfileExpression"], topic)
+            found_device_type = device_type_match.group(0) if device_type_match is not None else device_info[
+                "deviceProfileExpression"]
+        elif device_info.get("deviceProfileExpressionSource") == 'message' or device_info.get(
+                'deviceNameExpression') == 'constant':
+            found_device_type = TBUtility.get_value(device_info["deviceProfileExpression"], content,
+                                                    expression_instead_none=True)
+
+        return found_device_name, found_device_type
+
     def _process_on_message(self):
         while not self.__stopped:
             if not self._on_message_queue.empty():
                 client, userdata, message = self._on_message_queue.get()
 
                 self.statistics['MessagesReceived'] += 1
                 content = TBUtility.decode(message)
@@ -572,31 +609,19 @@
                 topic_handlers = [regex for regex in self.__connect_requests_sub_topics if
                                   fullmatch(regex, message.topic)]
 
                 if topic_handlers:
                     for topic in topic_handlers:
                         handler = self.__connect_requests_sub_topics[topic]
 
-                        found_device_name = None
-                        found_device_type = 'default'
-
                         # Get device name, either from topic or from content
-                        if handler.get("deviceNameTopicExpression"):
-                            device_name_match = search(handler["deviceNameTopicExpression"], message.topic)
-                            if device_name_match is not None:
-                                found_device_name = device_name_match.group(0)
-                        elif handler.get("deviceNameJsonExpression"):
-                            found_device_name = TBUtility.get_value(handler["deviceNameJsonExpression"], content)
-
-                        # Get device type (if any), either from topic or from content
-                        if handler.get("deviceTypeTopicExpression"):
-                            device_type_match = search(handler["deviceTypeTopicExpression"], message.topic)
-                            found_device_type = device_type_match.group(0) if device_type_match is not None else handler["deviceTypeTopicExpression"]
-                        elif handler.get("deviceTypeJsonExpression"):
-                            found_device_type = TBUtility.get_value(handler["deviceTypeJsonExpression"], content)
+                        device_info = handler.get("deviceInfo", {})
+
+                        found_device_name, found_device_type = MqttConnector._parce_device_info(device_info,
+                                                                                                message.topic, content)
 
                         if found_device_name is None:
                             self.__log.error("Device name missing from connection request")
                             continue
 
                         # Note: device must be added even if it is already known locally: else ThingsBoard
                         # will not send RPCs and attribute updates
@@ -610,32 +635,18 @@
                 # Check if message topic exists in disconnection handlers "i.e., I'm disconnecting a device" -----------
                 topic_handlers = [regex for regex in self.__disconnect_requests_sub_topics if
                                   fullmatch(regex, message.topic)]
                 if topic_handlers:
                     for topic in topic_handlers:
                         handler = self.__disconnect_requests_sub_topics[topic]
 
-                        found_device_name = None
-                        found_device_type = 'default'
-
                         # Get device name, either from topic or from content
-                        if handler.get("deviceNameTopicExpression"):
-                            device_name_match = search(handler["deviceNameTopicExpression"], message.topic)
-                            if device_name_match is not None:
-                                found_device_name = device_name_match.group(0)
-                        elif handler.get("deviceNameJsonExpression"):
-                            found_device_name = TBUtility.get_value(handler["deviceNameJsonExpression"], content)
-
-                        # Get device type (if any), either from topic or from content
-                        if handler.get("deviceTypeTopicExpression"):
-                            device_type_match = search(handler["deviceTypeTopicExpression"], message.topic)
-                            if device_type_match is not None:
-                                found_device_type = device_type_match.group(0)
-                        elif handler.get("deviceTypeJsonExpression"):
-                            found_device_type = TBUtility.get_value(handler["deviceTypeJsonExpression"], content)
+                        device_info = handler.get("deviceInfo", {})
+                        found_device_name, found_device_type = MqttConnector._parce_device_info(device_info,
+                                                                                                message.topic, content)
 
                         if found_device_name is None:
                             self.__log.error("Device name missing from disconnection request")
                             continue
 
                         if found_device_name in self.__gateway.get_devices():
                             self.__log.info("Disconnecting device %s of type %s", found_device_name, found_device_type)
@@ -653,34 +664,30 @@
                 topic_handlers = [regex for regex in self.__attribute_requests_sub_topics if
                                   fullmatch(regex, message.topic)]
                 if topic_handlers:
                     try:
                         for topic in topic_handlers:
                             handler = self.__attribute_requests_sub_topics[topic]
 
-                            found_device_name = None
                             found_attribute_names = None
 
                             # Get device name, either from topic or from content
-                            if handler.get("deviceNameTopicExpression"):
-                                device_name_match = search(handler["deviceNameTopicExpression"], message.topic)
-                                if device_name_match is not None:
-                                    found_device_name = device_name_match.group(0)
-                            elif handler.get("deviceNameJsonExpression"):
-                                found_device_name = TBUtility.get_value(handler["deviceNameJsonExpression"], content)
+                            device_info = handler.get("deviceInfo", {})
+                            found_device_name, _ = MqttConnector._parce_device_info(device_info, message.topic, content)
 
                             # Get attribute name, either from topic or from content
-                            if handler.get("attributeNameTopicExpression"):
-                                attribute_name_match = search(handler["attributeNameTopicExpression"], message.topic)
+                            if handler.get("attributeNameExpressionSource") == "topic":
+                                attribute_name_match = search(handler["attributeNameExpression"], message.topic)
                                 if attribute_name_match is not None:
                                     found_attribute_names = attribute_name_match.group(0)
-                            elif handler.get("attributeNameJsonExpression"):
+                            elif handler.get("attributeNameExpressionSource") == "message" or handler.get(
+                                    "attributeNameExpressionSource") == "constant":
                                 found_attribute_names = list(filter(lambda x: x is not None,
                                                                     TBUtility.get_values(
-                                                                        handler["attributeNameJsonExpression"],
+                                                                        handler["attributeNameExpression"],
                                                                         content)))
 
                             if found_device_name is None:
                                 self.__log.error("Device name missing from attribute request")
                                 continue
 
                             if found_attribute_names is None:
@@ -933,21 +940,22 @@
             converter_obj = converter_class_obj
             if converter_class_name == converter_name:
                 converter_obj.config = config
                 self._send_current_converter_config(self.name + ':' + converter_name, config)
                 self.__log.info('Updated converter configuration for: %s with configuration %s',
                                 converter_name, converter_obj.config)
 
-                for device_config in self.config['mapping']:
+                for device_config in self.config['dataMapping']:
                     try:
-                        if device_config['converter']['deviceNameJsonExpression'] == config['deviceNameJsonExpression']:
+                        if device_config['converter']['deviceInfo']['deviceNameExpression'] == config[
+                                'deviceNameExpression']:
                             device_config['converter'].update(config)
 
-                        if device_config['converter']['deviceNameTopicExpression'] == config[
-                                'deviceNameTopicExpression']:
+                        if device_config['converter']['deviceInfo']['deviceProfileExpression'] == config[
+                                'deviceProfileExpression']:
                             device_config['converter'].update(config)
                     except KeyError:
                         continue
 
                 self.__gateway.update_connector_config_file(self.name, self.config)
 
     def _init_send_current_converter_config(self):
@@ -973,15 +981,14 @@
 
         def run(self):
             while not self.stopped:
                 if not self.__msg_queue.empty():
                     self.in_progress = True
                     convert_function, config, incoming_data = self.__msg_queue.get(True, 100)
                     converted_data = convert_function(config, incoming_data)
-                    # log.debug(converted_data)
                     if converted_data and (converted_data.get(ATTRIBUTES_PARAMETER) or
                                            converted_data.get(TELEMETRY_PARAMETER)):
                         self.__send_result(config, converted_data)
                     self.in_progress = False
                 else:
                     sleep(.2)
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/mqtt/mqtt_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/mqtt/mqtt_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ocpp/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ocpp/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ocpp/charge_point.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ocpp/charge_point.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ocpp/ocpp_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ocpp/ocpp_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,16 @@
         self._central_system_config = config['centralSystem']
         self._charge_points_config = config.get('chargePoints', [])
         self._connector_type = connector_type
         self.statistics = {'MessagesReceived': 0,
                            'MessagesSent': 0}
         self._gateway = gateway
         self.name = self._config.get("name", 'OCPP Connector ' + ''.join(choice(ascii_lowercase) for _ in range(5)))
-        self._log = init_logger(self._gateway, self.name, self._config.get('logLevel', 'INFO'))
+        self._log = init_logger(self._gateway, self.name, self._config.get('logLevel', 'INFO'),
+                                enable_remote_logging=self._config.get('enableRemoteLogging', False))
 
         self._default_converters = {'uplink': 'OcppUplinkConverter'}
         self._server = None
         self._connected_charge_points = []
 
         self._ssl_context = None
         try:
@@ -215,15 +216,15 @@
 
         for socket in self._server.server.sockets:
             socket._sock.close()
 
         self.__loop.stop()
 
         self._log.info('%s has been stopped.', self.get_name())
-        self._log.reset()
+        self._log.stop()
 
     def get_id(self):
         return self.__id
 
     def get_name(self):
         return self.name
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ocpp/ocpp_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ocpp/ocpp_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/ocpp/ocpp_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/ocpp/ocpp_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/odbc/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/odbc/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/odbc/odbc_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/odbc/odbc_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,16 @@
         self.name = config.get("name", 'ODBC Connector ' + ''.join(choice(ascii_lowercase) for _ in range(5)))
 
         self.statistics = {'MessagesReceived': 0,
                            'MessagesSent': 0}
         self.__gateway = gateway
         self.__config = config
         self.__id = self.__config.get('id')
-        self._log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'))
+        self._log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'),
+                                enable_remote_logging=self.__config.get('enableRemoteLogging', False))
         self._connector_type = connector_type
         self.__stopped = False
 
         self.__config_dir = self.__gateway.get_config_path() + "odbc" + path.sep
 
         self.__connection = None
         self.__cursor = None
@@ -89,15 +90,15 @@
         self.__stopped = False
         self.start()
 
     def close(self):
         if not self.__stopped:
             self.__stopped = True
             self._log.debug("[%s] Stopping", self.get_name())
-            self._log.reset()
+            self._log.stop()
 
     def get_id(self):
         return self.__id
 
     def get_name(self):
         return self.name
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/odbc/odbc_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/odbc/odbc_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/odbc/odbc_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/odbc/odbc_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua/opcua_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua/opcua_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,18 @@
         self.statistics = {'MessagesReceived': 0,
                            'MessagesSent': 0}
         super().__init__()
         self.__gateway = gateway
         self._config = config
         self.__id = self._config.get('id')
         self.__server_conf = config.get("server")
-        self.name = self._config.get("name", 'OPC-UA ' + ''.join(choice(ascii_lowercase) for _ in range(5)) + " Connector")
-        self._log = init_logger(self.__gateway, self.name, self._config.get('logLevel', 'INFO'))
+        self.name = self._config.get("name",
+                                     'OPC-UA ' + ''.join(choice(ascii_lowercase) for _ in range(5)) + " Connector")
+        self._log = init_logger(self.__gateway, self.name, self._config.get('logLevel', 'INFO'),
+                                enable_remote_logging=self._config.get('enableRemoteLogging', False))
         self._log.warning("OPC-UA Connector is deprecated and will be removed in the release v.4.0")
         self.__interest_nodes = []
         self.__available_object_resources = {}
         self.__show_map = self.__server_conf.get("showMap", False)
         self.__previous_scan_time = 0
         for mapping in self.__server_conf["mapping"]:
             if mapping.get("deviceNodePattern") is not None:
@@ -238,15 +240,15 @@
             try:
                 # Always try to disconnect to release resource on client and server side!
                 self.client.disconnect()
             except:
                 pass
         self.__connected = False
         self._log.info('%s has been stopped.', self.get_name())
-        self._log.reset()
+        self._log.stop()
 
     def get_id(self):
         return self.__id
 
     def get_name(self):
         return self.name
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua/opcua_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua/opcua_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua/opcua_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua/opcua_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua_asyncio/device.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua_asyncio/device.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua_asyncio/opcua_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua_asyncio/opcua_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,27 +42,34 @@
 
 SECURITY_POLICIES = {
     "Basic128Rsa15": SecurityPolicyBasic128Rsa15,
     "Basic256": SecurityPolicyBasic256,
     "Basic256Sha256": SecurityPolicyBasic256Sha256,
 }
 
+MESSAGE_SECURITY_MODES = {
+    "None": asyncua.ua.MessageSecurityMode.None_,
+    "Sign": asyncua.ua.MessageSecurityMode.Sign,
+    "SignAndEncrypt": asyncua.ua.MessageSecurityMode.SignAndEncrypt
+}
+
 
 class OpcUaConnectorAsyncIO(Connector, Thread):
     def __init__(self, gateway, config, connector_type):
         self.statistics = {'MessagesReceived': 0,
                            'MessagesSent': 0}
         super().__init__()
         self._connector_type = connector_type
         self.__gateway = gateway
         self.__config = config
         self.__id = self.__config.get('id')
         self.__server_conf = config['server']
         self.name = self.__config.get("name", 'OPC-UA Connector ' + ''.join(choice(ascii_lowercase) for _ in range(5)))
-        self.__log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'))
+        self.__log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'),
+                                 enable_remote_logging=self.__config.get('enableRemoteLogging', False))
 
         if "opc.tcp" not in self.__server_conf.get("url"):
             self.__opcua_url = "opc.tcp://" + self.__server_conf.get("url")
         else:
             self.__opcua_url = self.__server_conf.get("url")
 
         self.__data_to_send = Queue(-1)
@@ -93,15 +100,15 @@
 
         while not task.done():
             sleep(.2)
 
         self.__stopped = True
         self.__connected = False
         self.__log.info('%s has been stopped.', self.get_name())
-        self.__log.reset()
+        self.__log.stop()
 
     async def __reset_node(self, node):
         node['valid'] = False
         if node.get('sub_on', False):
             try:
                 if self.__subscription:
                     await self.__subscription.unsubscribe(node['subscription'])
@@ -189,24 +196,26 @@
 
     async def __set_auth_settings_by_cert(self):
         try:
             ca_cert = self.__server_conf["identity"].get("caCert")
             private_key = self.__server_conf["identity"].get("privateKey")
             cert = self.__server_conf["identity"].get("cert")
             policy = self.__server_conf["security"]
+            mode = self.__server_conf["identity"].get("mode", "SignAndEncrypt")
 
             if cert is None or private_key is None:
                 self.__log.exception("Error in ssl configuration - cert or privateKey parameter not found")
                 raise RuntimeError("Error in ssl configuration - cert or privateKey parameter not found")
 
             await self.__client.set_security(
                 SECURITY_POLICIES[policy],
                 certificate=cert,
                 private_key=private_key,
-                server_certificate=ca_cert
+                server_certificate=ca_cert,
+                mode=MESSAGE_SECURITY_MODES[mode]
             )
         except Exception as e:
             self.__log.exception(e)
 
     def __set_auth_settings_by_username(self):
         self.__client.set_user(self.__server_conf["identity"].get("username"))
         if self.__server_conf["identity"].get("password"):
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua_asyncio/opcua_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua_asyncio/opcua_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/opcua_asyncio/opcua_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/opcua_asyncio/opcua_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/request/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/request/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/request/json_request_downlink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/request/json_request_downlink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/request/json_request_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/request/json_request_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/request/request_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/request/request_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,16 @@
                            'MessagesSent': 0}
         self.__rpc_requests = []
         self.__config = config
         self.__id = self.__config.get('id')
         self._connector_type = connector_type
         self.__gateway = gateway
         self.name = self.__config.get("name", "".join(choice(ascii_lowercase) for _ in range(5)))
-        self._log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'))
+        self._log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'),
+                                enable_remote_logging=self.__config.get('enableRemoteLogging', False))
         self.__security = HTTPBasicAuth(self.__config["security"]["username"], self.__config["security"]["password"]) if \
             self.__config["security"]["type"] == "basic" else None
         self.__host = None
         self.__service_headers = {}
         if "http://" in self.__config["host"].lower() or "https://" in self.__config["host"].lower():
             self.__host = self.__config["host"]
         else:
@@ -317,11 +318,11 @@
 
     def open(self):
         self.__stopped = False
         self.start()
 
     def close(self):
         self.__stopped = True
-        self._log.reset()
+        self._log.stop()
 
     def get_config(self):
         return self.__config
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/request/request_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/request/request_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/request/request_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/request/request_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/rest/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/rest/json_rest_downlink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/rest/json_rest_downlink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/rest/json_rest_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/rest/json_rest_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/rest/rest_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/rest/rest_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,16 @@
         self.__config = config
         self.__id = self.__config.get('id')
         self._connector_type = connector_type
         self.statistics = {'MessagesReceived': 0,
                            'MessagesSent': 0}
         self.name = config.get("name", 'REST Connector ' + ''.join(choice(ascii_lowercase) for _ in range(5)))
         self.__gateway = gateway
-        self.__log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'))
+        self.__log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'),
+                                 enable_remote_logging=self.__config.get('enableRemoteLogging', False))
         self._default_downlink_converter = TBModuleLoader.import_module(self._connector_type,
                                                                         self._default_converters['downlink'])
         self._default_uplink_converter = TBModuleLoader.import_module(self._connector_type,
                                                                       self._default_converters['uplink'])
         self.__USER_DATA = {}
         self._loop = None
         self._app = None
@@ -195,15 +196,15 @@
 
     def close(self):
         self.__stopped = True
         self._connected = False
         if not self._loop.is_closed():
             self._loop.call_soon_threadsafe(self._loop.stop)
         self.__log.info('REST connector stopped.')
-        self.__log.reset()
+        self.__log.stop()
         self.join()
 
     def get_id(self):
         return self.__id
 
     def get_name(self):
         return self.name
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/rest/rest_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/rest/rest_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/rest/ssl_generator.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/rest/ssl_generator.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/snmp/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/snmp/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/snmp/snmp_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/snmp/snmp_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,16 @@
         self.__gateway = gateway
         self._connected = False
         self.__stopped = False
         self._connector_type = connector_type
         self.__config = config
         self.__id = self.__config.get('id')
         self.name = config.get("name", 'SNMP Connector ' + ''.join(choice(ascii_lowercase) for _ in range(5)))
-        self._log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'))
+        self._log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'),
+                                enable_remote_logging=self.__config.get('enableRemoteLogging', False))
         self.__devices = self.__config["devices"]
         self.statistics = {'MessagesReceived': 0,
                            'MessagesSent': 0}
         self._default_converters = {
             "uplink": "SNMPUplinkConverter",
             "downlink": "SNMPDownlinkConverter"
         }
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/snmp/snmp_downlink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/snmp/snmp_downlink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/snmp/snmp_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/snmp/snmp_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/socket/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/socket/bytes_socket_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/socket/bytes_socket_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/socket/socket_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/socket/socket_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,16 @@
         self.__config = config
         self.__id = self.__config.get('id')
         self._connector_type = connector_type
         self.statistics = {'MessagesReceived': 0,
                            'MessagesSent': 0}
         self.__gateway = gateway
         self.name = config.get("name", 'TCP Connector ' + ''.join(choice(ascii_lowercase) for _ in range(5)))
-        self.__log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'))
+        self.__log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'),
+                                 enable_remote_logging=self.__config.get('enableRemoteLogging', False))
         self.daemon = True
         self.__stopped = False
         self._connected = False
         self.__bind = False
         self.__socket_type = config['type'].upper()
         self.__socket_address = config['address']
         self.__socket_port = config['port']
@@ -306,15 +307,15 @@
         while self.__socket.fileno() != -1:
             try:
                 self.__socket.shutdown(socket.SHUT_RDWR)
             except OSError:
                 pass  # Ignore errors when socket is already closed
             self.__socket.close()
             sleep(0.01)
-        self.__log.reset()
+        self.__log.stop()
 
     def get_name(self):
         return self.name
 
     def get_type(self):
         return self._connector_type
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/socket/socket_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/socket/socket_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/xmpp/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/xmpp/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/xmpp/xmpp_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/xmpp/xmpp_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,16 @@
         self.__gateway = gateway
 
         self.__config = config
         self.__id = self.__config.get('id')
         self._server_config = config['server']
         self._devices_config = config.get('devices', [])
         self.name = config.get("name", 'XMPP Connector ' + ''.join(choice(ascii_lowercase) for _ in range(5)))
-        self.__log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'))
+        self.__log = init_logger(self.__gateway, self.name, self.__config.get('logLevel', 'INFO'),
+                                 enable_remote_logging=self.__config.get('enableRemoteLogging', False))
 
         self._devices = {}
         self._reformat_devices_config()
 
         # devices dict for RPC and attributes updates
         # {'deviceName': 'device_jid'}
         self._available_device = {}
@@ -198,15 +199,15 @@
 
             sleep(.2)
 
     def close(self):
         self.__stopped = True
         self._connected = False
         self.__log.info('%s has been stopped.', self.get_name())
-        self.__log.reset()
+        self.__log.stop()
 
     def get_id(self):
         return self.__id
 
     def get_name(self):
         return self.name
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/xmpp/xmpp_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/xmpp/xmpp_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/connectors/xmpp/xmpp_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/connectors/xmpp/xmpp_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/bacnet/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/bacnet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/ble/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/ble/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/can/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/can/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/modbus/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/modbus/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/mqtt/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/mqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/mqtt/custom_mqtt_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/mqtt/custom_mqtt_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/ocpp/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/ocpp/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/odbc/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/odbc/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/opcua/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/opcua/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/opcua_asyncio/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/opcua_asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/request/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/request/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/request/custom_request_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/request/custom_request_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/rest/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/serial/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/serial/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/serial/custom_serial_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/serial/custom_serial_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,16 @@
                            'MessagesSent': 0}  # Dictionary, will save information about count received and sent messages.
         self._connector_type = connector_type
         self.__config = config  # Save configuration from the configuration file.
         self.__gateway = gateway  # Save gateway object, we will use some gateway methods for adding devices and saving data from them.
         self.name = self.__config.get("name",
                                        "Custom %s connector " % self.get_name() + ''.join(
                                            choice(ascii_lowercase) for _ in range(5)))  # get from the configuration or create name for logs.
-        self._log = init_logger(self.__gateway, self.name, level=self.__config.get('logLevel'))
+        self._log = init_logger(self.__gateway, self.name, level=self.__config.get('logLevel'),
+                                enable_remote_logging=self.__config.get('enableRemoteLogging', False))
         self._log.info("Starting Custom %s connector", self.get_name())  # Send message to logger
         self.daemon = True  # Set self thread as daemon
         self.stopped = True  # Service variable for check state
         self.__connected = False  # Service variable for check connection to device
         self.__devices = {}  # Dictionary with devices, will contain devices configurations, converters for devices and serial port objects
         self.__load_converters(connector_type)  # Call function to load converters and save it into devices dictionary
         self.__connect_to_devices()  # Call function for connect to devices
@@ -154,15 +155,15 @@
 
     def close(self):  # Close connect function, usually used if exception handled in gateway main loop or in connector main loop
         self.stopped = True
         for device in self.__devices:
             self.__gateway.del_device(self.__devices[device]["device_config"]["name"])
             if self.__devices[device]['serial'].isOpen():
                 self.__devices[device]['serial'].close()
-        self._log.reset()
+        self._log.stop()
 
     def on_attributes_update(self, content):  # Function used for processing attribute update requests from ThingsBoard
         self._log.debug(content)
         if self.__devices.get(content["device"]) is not None:
             device_config = self.__devices[content["device"]].get("device_config")
             if device_config is not None and device_config.get("attributeUpdates") is not None:
                 requests = device_config["attributeUpdates"]
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/serial/custom_serial_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/serial/custom_serial_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/snmp/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/snmp/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/socket/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/extensions/xmpp/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/extensions/xmpp/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/configuration_wizard.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/configuration_wizard.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/constant_enums.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/constant_enums.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/constants.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/constants.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/device_filter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/device_filter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/duplicate_detector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/duplicate_detector.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/grpc_service/grpc_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/grpc_service/grpc_connector.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/grpc_service/grpc_downlink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/grpc_service/grpc_downlink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/grpc_service/grpc_uplink_converter.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/grpc_service/grpc_uplink_converter.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/grpc_service/tb_grpc_manager.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/grpc_service/tb_grpc_manager.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/grpc_service/tb_grpc_server.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/grpc_service/tb_grpc_server.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/hot_reloader.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/hot_reloader.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/proto/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/proto/messages_pb2.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/proto/messages_pb2.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/proto/messages_pb2_grpc.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/proto/messages_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/shell/proxy.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/shell/proxy.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/shell/shell.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/shell/shell.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/statistics_service.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/statistics_service.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/tb_client.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/tb_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     from tb_gateway_mqtt import TBGatewayMqttClient, TBDeviceMqttClient
 except ImportError:
     print("tb-mqtt-client library not found - installing...")
     TBUtility.install_package('tb-mqtt-client')
     from tb_gateway_mqtt import TBGatewayMqttClient, TBDeviceMqttClient
 
 import tb_device_mqtt
-tb_device_mqtt.DEFAULT_TIMEOUT = 1
+tb_device_mqtt.DEFAULT_TIMEOUT = 3
 
 class TBClient(threading.Thread):
     def __init__(self, config, config_folder_path, logger):
         self.__logger = logger
         super().__init__()
         self.name = 'Connection thread.'
         self.daemon = True
@@ -261,15 +261,15 @@
                     if self.__stopped:
                         break
                     self.__logger.debug("connecting to ThingsBoard")
                     try:
                         self.client.connect(keepalive=keep_alive,
                                             min_reconnect_delay=self.__min_reconnect_delay)
                     except ConnectionRefusedError:
-                        pass
+                        self.__logger.error("Connection refused. Check ThingsBoard is running.")
                     except Exception as e:
                         self.__logger.exception(e)
                 sleep(1)
         except Exception as e:
             self.__logger.exception(e)
             sleep(10)
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/gateway/tb_gateway_service.py` & `thingsboard-gateway-3.5/thingsboard_gateway/gateway/tb_gateway_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from platform import system as platform_system
 from queue import SimpleQueue
 from random import choice
 from signal import signal, SIGINT
 from string import ascii_lowercase, hexdigits
 from sys import argv, executable, getsizeof
 from threading import RLock, Thread, main_thread, current_thread
-from time import sleep, time
+from time import sleep, time, monotonic
 
 from simplejson import JSONDecodeError, dumps, load, loads
 from yaml import safe_load
 
 from thingsboard_gateway.connectors.connector import Connector
 from thingsboard_gateway.gateway.constant_enums import DeviceActions, Status
 from thingsboard_gateway.gateway.constants import CONNECTED_DEVICES_FILENAME, CONNECTOR_PARAMETER, \
@@ -529,18 +529,23 @@
     def __modify_main_config(self):
         env_variables = get_env_variables()
         self.__config['thingsboard'] = {**self.__config['thingsboard'], **env_variables}
 
     def __close_connectors(self):
         for current_connector in self.available_connectors_by_id:
             try:
-                self.available_connectors_by_id[current_connector].close()
+                close_start = monotonic()
+                while not self.available_connectors_by_id[current_connector].is_stopped():
+                    self.available_connectors_by_id[current_connector].close()
+                    if monotonic() - close_start > 5:
+                        log.error("Connector %s close timeout", current_connector)
+                        break
                 log.debug("Connector %s closed connection.", current_connector)
             except Exception as e:
-                log.exception(e)
+                log.exception("Error while closing connector %s", current_connector, exc_info=e)
 
     def __stop_gateway(self):
         self.stopped = True
         self.__updater.stop()
         log.info("Stopping...")
 
         if self.__statistics_service is not None:
@@ -889,15 +894,15 @@
                                     else:
                                         log.warning("Config incorrect for %s", connector_type)
                                 else:
                                     log.warning("Config is empty for %s", connector_type)
                             except Exception as e:
                                 log.error("[%r] Error on loading connector %r: %r", connector_id, connector_name, e)
                                 log.exception(e, attr_name=connector_name)
-                                if connector is not None:
+                                if connector is not None and not connector.is_stopped():
                                     connector.close()
                     else:
                         self.__grpc_connectors.update({connector_config['grpc_key']: connector_config})
                         if connector_type != 'grpc':
                             connector_dir_abs = "/".join(self._config_dir.split("/")[:-2])
                             connector_file_name = f'{connector_type}_connector.py'
                             connector_abs_path = f'{connector_dir_abs}/grpc_connectors/{connector_type}/{connector_file_name}'
@@ -1411,36 +1416,41 @@
             self.__async_device_actions_queue.put((DeviceActions.CONNECT, data))
             return Status.SUCCESS
         else:
             return Status.FAILURE
 
     def add_device(self, device_name, content, device_type=None):
         device_type = device_type if device_type is not None else 'default'
+        self.__connected_devices[device_name] = {**content, DEVICE_TYPE_PARAMETER: device_type}
+        self.__saved_devices[device_name] = {**content, DEVICE_TYPE_PARAMETER: device_type}
+        self.__save_persistent_devices()
+        self.tb_client.client.gw_connect_device(device_name, device_type)
         device_details = None
         if device_name in self.__saved_devices:
             device_details = {
                 'connectorType': content['connector'].get_type(),
                 'connectorName': content['connector'].get_name()
             }
-        self.__connected_devices[device_name] = {**content, DEVICE_TYPE_PARAMETER: device_type}
-        self.__saved_devices[device_name] = {**content, DEVICE_TYPE_PARAMETER: device_type}
-        self.__save_persistent_devices()
-        self.tb_client.client.gw_connect_device(device_name, device_type)
         if device_details is not None:
             self.tb_client.client.gw_send_attributes(device_name, device_details)
 
     def update_device(self, device_name, event, content):
         should_save = False
         if self.__connected_devices.get(device_name) is None:
             return
         if event == 'connector' and self.__connected_devices[device_name].get(event) != content:
             should_save = True
         self.__connected_devices[device_name][event] = content
         if should_save:
             self.__save_persistent_devices()
+            self.send_to_storage(connector_name=content.get_name(),
+                                 connector_id=content.get_id(),
+                                 data={"deviceName": device_name,
+                                       "deviceType": self.__connected_devices[device_name][DEVICE_TYPE_PARAMETER],
+                                       "attributes": [{"connectorName": content.name}]})
 
     def del_device_async(self, data):
         if data['deviceName'] in self.__saved_devices:
             self.__async_device_actions_queue.put((DeviceActions.DISCONNECT, data))
             return Status.SUCCESS
         else:
             return Status.FAILURE
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/storage/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/storage/event_storage.py` & `thingsboard-gateway-3.5/thingsboard_gateway/storage/event_storage.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/storage/file/event_storage_files.py` & `thingsboard-gateway-3.5/thingsboard_gateway/storage/file/event_storage_files.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/storage/file/event_storage_reader.py` & `thingsboard-gateway-3.5/thingsboard_gateway/storage/file/event_storage_reader.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/storage/file/event_storage_reader_pointer.py` & `thingsboard-gateway-3.5/thingsboard_gateway/storage/file/event_storage_reader_pointer.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/storage/file/event_storage_writer.py` & `thingsboard-gateway-3.5/thingsboard_gateway/storage/file/event_storage_writer.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/storage/file/file_event_storage.py` & `thingsboard-gateway-3.5/thingsboard_gateway/storage/file/file_event_storage.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/storage/file/file_event_storage_settings.py` & `thingsboard-gateway-3.5/thingsboard_gateway/storage/file/file_event_storage_settings.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/storage/memory/memory_event_storage.py` & `thingsboard-gateway-3.5/thingsboard_gateway/storage/memory/memory_event_storage.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/storage/sqlite/database.py` & `thingsboard-gateway-3.5/thingsboard_gateway/storage/sqlite/database.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/storage/sqlite/database_action_type.py` & `thingsboard-gateway-3.5/thingsboard_gateway/storage/sqlite/database_action_type.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/storage/sqlite/database_connector.py` & `thingsboard-gateway-3.5/thingsboard_gateway/storage/sqlite/database_connector.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/storage/sqlite/database_request.py` & `thingsboard-gateway-3.5/thingsboard_gateway/storage/sqlite/database_request.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/storage/sqlite/sqlite_event_storage.py` & `thingsboard-gateway-3.5/thingsboard_gateway/storage/sqlite/sqlite_event_storage.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/storage/sqlite/storage_settings.py` & `thingsboard-gateway-3.5/thingsboard_gateway/storage/sqlite/storage_settings.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/tb_gateway.py` & `thingsboard-gateway-3.5/thingsboard_gateway/tb_gateway.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/tb_utility/__init__.py` & `thingsboard-gateway-3.5/thingsboard_gateway/tb_utility/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/tb_utility/tb_gateway_remote_configurator.py` & `thingsboard-gateway-3.5/thingsboard_gateway/tb_utility/tb_gateway_remote_configurator.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,61 +11,62 @@
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
 import os.path
 from logging import getLogger
 from logging.config import dictConfig
-from time import sleep, time
+from queue import Queue
+from threading import Thread
+from time import sleep, time, monotonic
 
-from packaging import version
 from regex import fullmatch
 from simplejson import dumps, load
 
 from thingsboard_gateway.gateway.tb_client import TBClient
-from thingsboard_gateway.tb_utility.tb_handler import TBLoggerHandler
 from thingsboard_gateway.tb_utility.tb_utility import TBUtility
 
 LOG = getLogger("service")
 
 
 class RemoteConfigurator:
     DEFAULT_STATISTICS = {
         'enable': True,
         'statsSendPeriodInSeconds': 3600
     }
 
     def __init__(self, gateway, config):
+        self._request_queue = Queue()
+        self.in_process = False
         self._gateway = gateway
         self._config = config
         self._load_connectors_configuration()
         self._logs_configuration = self._load_logs_configuration()
-        self.in_process = False
         self._active_connectors = []
         self._handlers = {
-            'general_configuration': self._handle_general_configuration_update,
             'storage_configuration': self._handle_storage_configuration_update,
             'grpc_configuration': self._handle_grpc_configuration_update,
             'logs_configuration': self._handle_logs_configuration_update,
             'active_connectors': self._handle_active_connectors_update,
             'RemoteLoggingLevel': self._handle_remote_logging_level_update,
             r'(?=\D*\d?).*': self._handle_connector_configuration_update,
         }
         self._modifiable_static_attrs = {
             'logs_configuration': 'logs.json'
         }
         self._max_backup_files_number = 10
 
-        self._remote_gateway_version = None
-        self._fetch_remote_gateway_version()
-
         # creating backups (general and connectors)
         self.create_configuration_file_backup(self._get_general_config_in_local_format(), "tb_gateway.json")
         self._create_connectors_backup()
 
+        self._requests_processing_thread = Thread(name='Remote Request Processing', target=self._process_config_request,
+                                                  daemon=True)
+        self._requests_processing_thread.start()
+
         LOG.info('Remote Configurator started')
 
     @property
     def general_configuration(self):
         return self._config.get('thingsboard', {})
 
     @general_configuration.setter
@@ -92,67 +93,14 @@
     def connectors_configuration(self):
         connectors = self._config.get('connectors', [])
         for connector in connectors:
             connector.pop('config_updated', None)
             connector.pop('config_file_path', None)
         return connectors
 
-    def _fetch_remote_gateway_version(self):
-        def callback(key, err):
-            if err is not None:
-                LOG.exception(err)
-            if key is None:
-                self._remote_gateway_version = '0.0'
-                return
-
-            try:
-                self._remote_gateway_version = key['client']['Version']
-            except KeyError:
-                self._remote_gateway_version = '0.0'
-                LOG.warning('Cannot fetch version number from server! Version number set to 0.0')
-
-        self._gateway.tb_client.client.request_attributes(client_keys=['Version'], callback=callback)
-
-    def _send_default_connectors_config(self):
-        """
-        If remote gateway version wasn't fetch (default set to '0.0'), remote configurator send all default
-        connectors configs.
-        """
-        from thingsboard_gateway.gateway.tb_gateway_service import DEFAULT_CONNECTORS
-
-        # remote gateway version fetching in __init__ method (_fetch_remote_gateway_version)
-        LOG.debug('Waiting for remote gateway version...')
-
-        try_count = 1
-        while not self._remote_gateway_version and try_count <= 3:
-            if self._gateway.stopped:
-                return
-            try_count += 1
-            sleep(1)
-
-        if self._remote_gateway_version is None:
-            self._remote_gateway_version = "0.0"
-
-        need_update_configs = (self._remote_gateway_version == "0.0"
-                               or version.parse(self._gateway.version.get('current_version', '0.0')) > version.parse(str(self._remote_gateway_version)))
-
-        if need_update_configs:
-            default_connectors_configs_folder_path = self._gateway.get_config_path() + 'default-configs/'
-
-            for (connector_type, _) in DEFAULT_CONNECTORS.items():
-                connector_filename = connector_type + '.json'
-                try:
-                    with open(default_connectors_configs_folder_path + connector_filename, 'r') as file:
-                        config = load(file)
-                        self._gateway.tb_client.client.send_attributes(
-                            {connector_type.upper() + '_DEFAULT_CONFIG': config})
-                        LOG.debug('Default config for %s connector sent.', connector_type)
-                except FileNotFoundError:
-                    LOG.error('Default config file for %s connector not found! Passing...', connector_type)
-
     def _get_active_connectors(self):
         return [connector['name'] for connector in self.connectors_configuration]
 
     def _get_general_config_in_local_format(self):
         """
         Method returns general configuration in format that should be used only for local files
         !!!Don't use it for sending data to TB (use `_get_general_config_in_remote_format` instead)!!!
@@ -211,15 +159,14 @@
             'storage_configuration': self.storage_configuration,
             'grpc_configuration': self.grpc_configuration,
             'logs_configuration': {**self._logs_configuration, 'ts': int(time() * 1000)},
             'active_connectors': self._get_active_connectors(),
             'Version': self._gateway.version.get('current_version', '0.0')
         }
         self._gateway.tb_client.client.send_attributes(init_config_message)
-        self._send_default_connectors_config()
 
         # sending remote created connectors
         for connector in self.connectors_configuration:
             self._gateway.tb_client.client.send_attributes(
                 {connector['name']: {**connector,
                                      'logLevel': connector.get('configurationJson', {}).get('logLevel', 'INFO'),
                                      'ts': int(time() * 1000)}})
@@ -242,39 +189,48 @@
             with open(self._gateway.get_config_path() + 'logs.json', 'r') as logs:
                 return load(logs)
         except Exception:
             LOG.warning("Cannot open logs configuration file. Using default logs configuration.")
             return {}
 
     def process_config_request(self, config):
-        if not self.in_process:
-            LOG.info('Configuration update request received.')
-            LOG.debug('Got config update request: %s', config)
+        self._request_queue.put(config)
 
-            self.in_process = True
+    def _process_config_request(self):
+        while not self._gateway.stopped:
+            if not self._request_queue.empty():
+                self.in_process = True
+                config = self._request_queue.get()
+                LOG.info('Configuration update request received.')
+                LOG.debug('Got config update request: %s', config)
+
+                try:
+                    if 'general_configuration' in config.keys():
+                        self._handle_general_configuration_update(config['general_configuration'])
+                        config.pop('general_configuration', None)
+
+                    for attr_name in config.keys():
+                        if 'deleted' in attr_name:
+                            continue
+
+                        request_config = config[attr_name]
+                        if not self._is_modified(attr_name, request_config):
+                            continue
+
+                        for (name, func) in self._handlers.items():
+                            if fullmatch(name, attr_name):
+                                func(request_config)
+                                break
+                except (KeyError, AttributeError) as e:
+                    LOG.error('Unknown attribute update name (Available: %s), %r', ', '.join(self._handlers.keys()),
+                              exc_info=e)
 
-            try:
-                for attr_name in config.keys():
-                    if 'deleted' in attr_name:
-                        continue
-
-                    request_config = config[attr_name]
-                    if not self._is_modified(attr_name, request_config):
-                        continue
-
-                    for (name, func) in self._handlers.items():
-                        if fullmatch(name, attr_name):
-                            func(request_config)
-                            break
-            except (KeyError, AttributeError) as e:
-                LOG.error('Unknown attribute update name (Available: %s), %r', ', '.join(self._handlers.keys()), exc_info=e)
-            finally:
                 self.in_process = False
-        else:
-            LOG.error("Remote configuration is already in processing")
+            else:
+                sleep(.2)
 
     # HANDLERS ---------------------------------------------------------------------------------------------------------
     def _handle_general_configuration_update(self, config):
         """
         General configuration update handling in 5 steps:
         1. Checking if connection changed (host, port, QoS, security or provisioning sections);
         2. Checking if statistics collecting changed;
@@ -419,16 +375,15 @@
             LOG.error("Remote logging configuration is wrong, cannot apply it!")
             LOG.exception(e)
 
     def _handle_active_connectors_update(self, config):
         LOG.debug('Processing active connectors configuration update...')
 
         for connector_name in config:
-            if self._gateway.connectors_configs.get(connector_name) is None:
-                self._gateway._check_shared_attributes(shared_keys=[connector_name])
+            self._gateway._check_shared_attributes(shared_keys=[connector_name])
 
         has_changed = False
         for_deletion = []
         for active_connector_name in self._gateway.available_connectors_by_name:
             if active_connector_name not in config:
                 try:
                     self._gateway.available_connectors_by_name[active_connector_name].close()
@@ -452,54 +407,60 @@
         """
         Expected the following data structure:
         {
             "name": "Mqtt Broker Connector",
             "id": "bee7caf1-fd37-4026-8782-d480915d4d1a"
             "type": "mqtt",
             "configuration": "mqtt.json",
+            "enableRemoteLogging": false,
             "logLevel": "INFO",
             "key?type=>grpc": "auto",
             "class?type=>custom": "",
             "configurationJson": {
                 ...
             }
         }
         """
 
         LOG.debug('Processing connectors configuration update...')
 
         try:
             config_file_name = config['configuration']
 
-            identifier_parameter = 'id' if config.get('id') else 'name'
-            found_connectors = list(filter(lambda item: item[identifier_parameter] == config[identifier_parameter],
-                                           self.connectors_configuration))
+            identifier_parameter = 'id' if config.get('configurationJson', {}).get('id') else 'name'
+            found_connectors = list(filter(
+                lambda item: item[identifier_parameter] == config.get('configurationJson', {}).get(
+                    identifier_parameter) or config.get(identifier_parameter),
+                self.connectors_configuration))
 
-            if (config.get('configurationJson')
-                    and config.get('configurationJson').get('id') is None
+            if (config.get('configurationJson', {})
+                    and config.get('configurationJson', {}).get('id') is None
                     and len(found_connectors) > 0
                     and found_connectors[0].get('configurationJson') is not None
-                    and found_connectors[0].get('configurationJson').get('id') is not None):
+                    and found_connectors[0].get('configurationJson', {}).get('id') is not None):
                 connector_id = TBUtility.get_or_create_connector_id(found_connectors[0].get("configurationJson"))
             else:
                 connector_id = TBUtility.get_or_create_connector_id(config.get('configurationJson'))
+
             if not found_connectors:
                 connector_configuration = {'name': config['name'],
                                            'type': config['type'],
                                            'id': connector_id,
+                                           'enableRemoteLogging': config.get('enableRemoteLogging', False),
                                            'configuration': config_file_name}
                 if config.get('key'):
                     connector_configuration['key'] = config['key']
 
                 if config.get('class'):
                     connector_configuration['class'] = config['class']
 
                 with open(self._gateway.get_config_path() + config_file_name, 'w') as file:
                     config['configurationJson'].update({'logLevel': config['logLevel'],
                                                         'name': config['name'],
+                                                        'enableRemoteLogging': config.get('enableRemoteLogging', False),
                                                         'id': connector_id})
                     self.create_configuration_file_backup(config, config_file_name)
                     file.writelines(dumps(config['configurationJson'], indent='  '))
 
                 self.connectors_configuration.append(connector_configuration)
                 with open(self._gateway.get_config_path() + 'tb_gateway.json', 'w') as file:
                     file.writelines(dumps(self._get_general_config_in_local_format(), indent='  '))
@@ -522,59 +483,83 @@
 
                 connector_configuration = None
                 if (found_connector.get('id') != connector_id
                         or found_connector.get('name') != config['name']
                         or found_connector.get('type') != config['type']
                         or found_connector.get('class') != config.get('class')
                         or found_connector.get('key') != config.get('key')
-                        or found_connector.get('configurationJson', {}).get('logLevel') != config.get('logLevel')):
+                        or found_connector.get('configurationJson', {}).get('logLevel') != config.get('logLevel')
+                        or found_connector.get('enableRemoteLogging', False) != config.get('enableRemoteLogging',
+                                                                                           False)):
                     changed = True
-                    connector_configuration = {'name': config['name'], 'type': config['type'],
-                                               'id': connector_id, 'configuration': config_file_name}
+                    connector_configuration = {'name': config['name'],
+                                               'type': config['type'],
+                                               'id': connector_id,
+                                               'enableRemoteLogging': config.get('enableRemoteLogging', False),
+                                               'configuration': config_file_name}
 
                     if config.get('key'):
                         connector_configuration['key'] = config['key']
 
                     if config.get('class'):
                         connector_configuration['class'] = config['class']
 
                     found_connector.update(connector_configuration)
 
                 if changed:
                     with open(self._gateway.get_config_path() + config_file_name, 'w') as file:
                         config['configurationJson'].update({'logLevel': config['logLevel'],
                                                             'name': config['name'],
+                                                            'enableRemoteLogging': config.get('enableRemoteLogging',
+                                                                                              False),
                                                             'id': connector_id})
                         file.writelines(dumps(config['configurationJson'], indent='  '))
 
                     if connector_configuration is None:
                         connector_configuration = found_connector
                     if connector_configuration.get('id') in self._gateway.available_connectors_by_id:
-                        self._gateway.available_connectors_by_id[connector_configuration['id']].close()
+                        try:
+                            close_start = monotonic()
+                            while not self._gateway.available_connectors_by_id[connector_configuration['id']].is_stopped():
+                                self._gateway.available_connectors_by_id[connector_configuration['id']].close()
+                                if monotonic() - close_start > 5:
+                                    LOG.error('Connector %s not stopped in 5 seconds', connector_configuration['id'])
+                                    break
+                        except Exception as e:
+                            LOG.exception("Exception on closing connector occurred:", exc_info=e)
                     elif connector_configuration.get('name') in self._gateway.available_connectors_by_name:
-                        self._gateway.available_connectors_by_name[connector_configuration['name']].close()
+                        try:
+                            close_start = monotonic()
+                            while not self._gateway.available_connectors_by_name[connector_configuration['name']].is_stopped():
+                                self._gateway.available_connectors_by_name[connector_configuration['name']].close()
+                                if monotonic() - close_start > 5:
+                                    LOG.error('Connector %s not stopped in 5 seconds', connector_configuration['name'])
+                                    break
+                        except Exception as e:
+                            LOG.exception("Exception on closing connector occurred:", exc_info=e)
                     else:
                         LOG.warning('Connector with id %s not found in available connectors', connector_configuration.get('id'))
                     if connector_configuration.get('id') in self._gateway.available_connectors_by_id:
                         self._gateway.available_connectors_by_id.pop(connector_configuration['id'])
                         connector_configuration['id'] = connector_id
                     elif connector_configuration.get('name') in self._gateway.available_connectors_by_name:
                         self._gateway.available_connectors_by_name.pop(connector_configuration['name'])
                         connector_configuration['id'] = connector_id
                     else:
                         LOG.warning('Connector with id %s not found in available connectors', connector_configuration.get('id'))
 
                     self._gateway.load_connectors(self._get_general_config_in_local_format())
                     self._gateway.connect_with_connectors()
 
-            for device_name in list(self._gateway.get_devices().keys()):
-                for connector_id in self._gateway.available_connectors_by_id.keys():
-                    if (self._gateway.available_connectors_by_id.get(connector_id)
-                            and self._gateway.available_connectors_by_id[connector_id].get_id() == connector_id):
-                        self._gateway.update_device(device_name, "connector", self._gateway.available_connectors_by_id[connector_id])
+            for (device_name, device_config) in list(self._gateway.get_devices().items()):
+                if (connector_id == device_config.get('connector').get_id()
+                        and self._gateway.available_connectors_by_id.get(connector_id) is not None):
+                    self._gateway.update_device(device_name,
+                                                "connector",
+                                                self._gateway.available_connectors_by_id[connector_id])
 
             self._gateway.tb_client.client.send_attributes({config['name']: config})
         except Exception as e:
             LOG.exception(e)
 
     def _handle_remote_logging_level_update(self, config):
         self._gateway.tb_client.client.send_attributes({'RemoteLoggingLevel': config})
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/tb_utility/tb_handler.py` & `thingsboard-gateway-3.5/thingsboard_gateway/tb_utility/tb_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,13 +141,13 @@
             handler.setFormatter(logging.Formatter('[STREAM ONLY] %(asctime)s - %(levelname)s - [%(filename)s] - %(module)s - %(lineno)d - %(message)s'))
             logger.addHandler(handler)
 
 
 class TimedRotatingFileHandler(logging.handlers.TimedRotatingFileHandler):
     def __init__(self, filename, when='h', interval=1, backupCount=0,
                  encoding=None, delay=False, utc=False):
-        config_path = environ.get('logs')
+        config_path = environ.get('TB_GW_LOGS_PATH')
         if config_path:
             filename = config_path + '/' + filename.split('/')[-1]
 
         super().__init__(filename, when=when, interval=interval, backupCount=backupCount,
                          encoding=encoding, delay=delay, utc=utc)
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/tb_utility/tb_loader.py` & `thingsboard-gateway-3.5/thingsboard_gateway/tb_utility/tb_loader.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/tb_utility/tb_logger.py` & `thingsboard-gateway-3.5/thingsboard_gateway/tb_utility/tb_logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,63 +9,84 @@
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
 import logging
-from time import sleep
+from time import sleep, time
 from threading import Thread
 
 
-def init_logger(gateway, name, level):
+def init_logger(gateway, name, level, enable_remote_logging=False):
     """
     For creating a Logger with all config automatically
     Create a Logger manually only if you know what you are doing!
     """
     log = TbLogger(name=name, gateway=gateway)
 
-    if hasattr(gateway, 'remote_handler'):
-        log.addHandler(gateway.remote_handler)
+    if enable_remote_logging:
+        from thingsboard_gateway.tb_utility.tb_handler import TBLoggerHandler
+        remote_handler = TBLoggerHandler(gateway)
+        log.addHandler(remote_handler)
         log.setLevel(gateway.main_handler.level)
-        gateway.remote_handler.add_logger(name)
+        remote_handler.add_logger(name)
+        remote_handler.activate()
 
     if hasattr(gateway, 'main_handler'):
         log.addHandler(gateway.main_handler)
-        log.setLevel(gateway.remote_handler.level)
+        log.setLevel(gateway.main_handler.level)
 
     log_level_conf = level
     if log_level_conf:
         log_level = logging.getLevelName(log_level_conf)
-        log.setLevel(log_level)
+
+        try:
+            log.setLevel(log_level)
+        except ValueError:
+            log.setLevel(logging.NOTSET)
 
     return log
 
 
 class TbLogger(logging.Logger):
     ALL_ERRORS_COUNT = 0
     IS_ALL_ERRORS_COUNT_RESET = False
+    RESET_ERRORS__PERIOD = 60
 
     def __init__(self, name, gateway=None, level=logging.NOTSET):
         super(TbLogger, self).__init__(name=name, level=level)
         self.propagate = True
         self.parent = self.root
         self._gateway = gateway
+        self._stopped = False
         self.errors = 0
         self.attr_name = self.name + '_ERRORS_COUNT'
         self._is_on_init_state = True
         if self._gateway:
-            self._send_errors_thread = Thread(target=self._send_errors, name='Send Errors Thread', daemon=True)
+            self._send_errors_thread = Thread(target=self._send_errors, name='[LOGGER] Send Errors Thread', daemon=True)
             self._send_errors_thread.start()
 
+        self._start_time = time()
+        self._reset_errors_thread = Thread(target=self._reset_errors_timer, name='[LOGGER] Reset Errors Thread',
+                                           daemon=True)
+        self._reset_errors_thread.start()
+
     def reset(self):
         """
         !!!Need to be called manually in the connector 'close' method!!!
         """
-        TbLogger.ALL_ERRORS_COUNT = TbLogger.ALL_ERRORS_COUNT - self.errors
+        if TbLogger.ALL_ERRORS_COUNT > 0 and self.errors > 0:
+            TbLogger.ALL_ERRORS_COUNT = TbLogger.ALL_ERRORS_COUNT - self.errors
+            self.errors = 0
+            self._send_error_count()
+
+    def stop(self):
+        self.reset()
+        self._stopped = True
 
     @property
     def gateway(self):
         return self._gateway
 
     @gateway.setter
     def gateway(self, gateway):
@@ -83,29 +104,40 @@
 
         if not TbLogger.IS_ALL_ERRORS_COUNT_RESET and self._gateway.tb_client.is_connected():
             self._gateway.tb_client.client.send_telemetry(
                 {self.attr_name: 0, 'ALL_ERRORS_COUNT': 0}, quality_of_service=0)
             TbLogger.IS_ALL_ERRORS_COUNT_RESET = True
         self._is_on_init_state = False
 
+    def _reset_errors_timer(self):
+        while not self._stopped:
+            if time() - self._start_time >= TbLogger.RESET_ERRORS__PERIOD:
+                self.reset()
+                self._start_time = time()
+
+            sleep(1)
+
     def error(self, msg, *args, **kwargs):
         kwargs['stacklevel'] = 2
         super(TbLogger, self).error(msg, *args, **kwargs)
+        self._add_error()
         self._send_error_count()
 
     def exception(self, msg, *args, **kwargs) -> None:
         attr_name = kwargs.pop('attr_name', None)
         kwargs['stacklevel'] = 2
         super(TbLogger, self).exception(msg, *args, **kwargs)
+        self._add_error()
         self._send_error_count(error_attr_name=attr_name)
 
-    def _send_error_count(self, error_attr_name=None):
+    def _add_error(self):
         TbLogger.ALL_ERRORS_COUNT += 1
         self.errors += 1
 
+    def _send_error_count(self, error_attr_name=None):
         while self._is_on_init_state:
             sleep(.2)
 
         if self._gateway and hasattr(self._gateway, 'tb_client'):
             if error_attr_name:
                 error_attr_name = error_attr_name + '_ERRORS_COUNT'
             else:
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/tb_utility/tb_remote_shell.py` & `thingsboard-gateway-3.5/thingsboard_gateway/tb_utility/tb_remote_shell.py`

 * *Files identical despite different names*

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/tb_utility/tb_updater.py` & `thingsboard-gateway-3.5/thingsboard_gateway/tb_utility/tb_updater.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,35 +14,36 @@
 
 from logging import getLogger
 from platform import platform, release, system
 from threading import Thread
 from time import sleep, time
 from uuid import uuid1
 
-from pkg_resources import DistributionNotFound
-from pkg_resources import get_distribution
+from importlib.metadata import PackageNotFoundError
+from importlib.metadata import version as metadata_version
 from requests import ConnectionError, post
 from simplejson import loads
 
+from thingsboard_gateway import version
 from thingsboard_gateway.tb_utility.tb_utility import TBUtility
 
 log = getLogger("service")
 
 UPDATE_SERVICE_BASE_URL = "https://updates.thingsboard.io"
 
 
 class TBUpdater(Thread):
     def __init__(self):
         super().__init__()
 
         try:
-            self.__version = {"current_version": get_distribution('thingsboard_gateway').version,
-                              "latest_version": get_distribution('thingsboard_gateway').version}
-        except DistributionNotFound:
-            self.__version = {"current_version": "0.0", "latest_version": "0.0"}
+            distribution_version = metadata_version('thingsboard_gateway')
+            self.__version = {"current_version": distribution_version, "latest_version": distribution_version}
+        except PackageNotFoundError:
+            self.__version = {"current_version": version.VERSION, "latest_version": version.VERSION}
 
         self.__instance_id = str(uuid1())
         self.__platform = system()
         self.__release = release()
         self.__os_version = platform()
         self.__previous_check = 0
         self.__check_period = 3600.0
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway/tb_utility/tb_utility.py` & `thingsboard-gateway-3.5/thingsboard_gateway/tb_utility/tb_utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 import datetime
 from logging import getLogger
 from re import search, findall
 from uuid import uuid4
+from distutils.util import strtobool
 
 from cryptography import x509
 from cryptography.x509.oid import NameOID
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives import serialization
 from jsonpath_rw import parse
@@ -123,15 +124,15 @@
                 full_value = expression
         except Exception as e:
             log.exception(e)
         return full_value
 
     @staticmethod
     def get_values(expression, body=None, value_type="string", get_tag=False, expression_instead_none=False):
-        expression_arr = findall(r'\$\{[${A-Za-z0-9. ^\]\[*_:]*\}', expression)
+        expression_arr = findall(r'\$\{[${A-Za-z0-9. ^\]\[*_:"]*\}', expression)
 
         values = [TBUtility.get_value(exp, body, value_type=value_type, get_tag=get_tag,
                                       expression_instead_none=expression_instead_none) for exp in expression_arr]
 
         if '${' not in expression:
             values.append(expression)
 
@@ -240,28 +241,31 @@
         current_type = type(data)
         # use 'in' check instead of equality for such case like 'str' and 'string'
         new_type = new_type.lower()
         if current_type.__name__ in new_type:
             return data
 
         evaluated_data = eval(data, globals(), {}) if use_eval else data
-        if 'int' in new_type or 'long' in new_type:
-            return int(float(evaluated_data))
-        elif 'float' == new_type or 'double' == new_type:
-            return float(evaluated_data)
-        elif 'bool' in new_type:
-            return bool(evaluated_data)
-        else:
+        try:
+            if 'int' in new_type or 'long' in new_type:
+                return int(float(evaluated_data))
+            elif 'float' == new_type or 'double' == new_type:
+                return float(evaluated_data)
+            elif 'bool' in new_type:
+                return bool(strtobool(evaluated_data))
+            else:
+                return str(evaluated_data)
+        except ValueError:
             return str(evaluated_data)
 
     @staticmethod
     def get_or_create_connector_id(connector_conf):
         connector_id = str(uuid4())
         if isinstance(connector_conf, dict):
             if connector_conf.get('id') is not None:
                 connector_id = connector_conf['id']
         elif isinstance(connector_conf, str):
             start_find = connector_conf.find("{id_var_start}")
             end_find = connector_conf.find("{id_var_end}")
             if start_find > -1 and end_find > -1:
                 connector_id = connector_conf[start_find + 13:end_find]
-        return connector_id
+        return connector_id
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway.egg-info/PKG-INFO` & `thingsboard-gateway-3.5/thingsboard_gateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: thingsboard-gateway
-Version: 3.4.6
+Version: 3.5
 Summary: Thingsboard Gateway for IoT devices.
 Home-page: https://github.com/thingsboard/thingsboard-gateway
-Download-URL: https://github.com/thingsboard/thingsboard-gateway/archive/3.4.6.tar.gz
+Download-URL: https://github.com/thingsboard/thingsboard-gateway/archive/3.5.tar.gz
 Author: ThingsBoard
 Author-email: info@thingsboard.io
 License: Apache Software License (Apache Software License 2.0)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cryptography==3.4.*
@@ -21,15 +21,15 @@
 Requires-Dist: questionary
 Requires-Dist: pyfiglet
 Requires-Dist: termcolor
 Requires-Dist: mmh3
 Requires-Dist: grpcio==1.58.0
 Requires-Dist: protobuf
 Requires-Dist: cachetools
-Requires-Dist: tb-mqtt-client>=1.5
+Requires-Dist: tb-mqtt-client>=1.9.1
 Requires-Dist: packaging==23.1
 Requires-Dist: service-identity
 
 # ThingsBoard IoT Gateway  
 
 The Thingsboard **IoT Gateway** is an open-source solution that allows you to integrate devices connected to legacy and third-party systems with Thingsboard.
```

### Comparing `thingsboard-gateway-3.4.6/thingsboard_gateway.egg-info/SOURCES.txt` & `thingsboard-gateway-3.5/thingsboard_gateway.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 tests/tests.py
 thingsboard_gateway/tb_gateway.py
+thingsboard_gateway/version.py
 thingsboard_gateway.egg-info/PKG-INFO
 thingsboard_gateway.egg-info/SOURCES.txt
 thingsboard_gateway.egg-info/dependency_links.txt
 thingsboard_gateway.egg-info/entry_points.txt
 thingsboard_gateway.egg-info/requires.txt
 thingsboard_gateway.egg-info/top_level.txt
 thingsboard_gateway/config/bacnet.json
@@ -25,29 +26,14 @@
 thingsboard_gateway/config/opcua.json
 thingsboard_gateway/config/request.json
 thingsboard_gateway/config/rest.json
 thingsboard_gateway/config/snmp.json
 thingsboard_gateway/config/socket.json
 thingsboard_gateway/config/tb_gateway.json
 thingsboard_gateway/config/xmpp.json
-thingsboard_gateway/config/default-configs/bacnet.json
-thingsboard_gateway/config/default-configs/ble.json
-thingsboard_gateway/config/default-configs/can.json
-thingsboard_gateway/config/default-configs/ftp.json
-thingsboard_gateway/config/default-configs/modbus.json
-thingsboard_gateway/config/default-configs/mqtt.json
-thingsboard_gateway/config/default-configs/ocpp.json
-thingsboard_gateway/config/default-configs/odbc.json
-thingsboard_gateway/config/default-configs/opcua.json
-thingsboard_gateway/config/default-configs/opcua_asyncio.json
-thingsboard_gateway/config/default-configs/request.json
-thingsboard_gateway/config/default-configs/rest.json
-thingsboard_gateway/config/default-configs/snmp.json
-thingsboard_gateway/config/default-configs/socket.json
-thingsboard_gateway/config/default-configs/xmpp.json
 thingsboard_gateway/config/statistics/statistics_linux.json
 thingsboard_gateway/config/statistics/statistics_macos.json
 thingsboard_gateway/config/statistics/statistics_windows.json
 thingsboard_gateway/connectors/__init__.py
 thingsboard_gateway/connectors/connector.py
 thingsboard_gateway/connectors/converter.py
 thingsboard_gateway/connectors/bacnet/__init__.py
@@ -81,14 +67,15 @@
 thingsboard_gateway/connectors/modbus/bytes_modbus_downlink_converter.py
 thingsboard_gateway/connectors/modbus/bytes_modbus_uplink_converter.py
 thingsboard_gateway/connectors/modbus/constants.py
 thingsboard_gateway/connectors/modbus/modbus_connector.py
 thingsboard_gateway/connectors/modbus/modbus_converter.py
 thingsboard_gateway/connectors/modbus/slave.py
 thingsboard_gateway/connectors/mqtt/__init__.py
+thingsboard_gateway/connectors/mqtt/backward_compatibility_adapter.py
 thingsboard_gateway/connectors/mqtt/bytes_mqtt_uplink_converter.py
 thingsboard_gateway/connectors/mqtt/json_mqtt_uplink_converter.py
 thingsboard_gateway/connectors/mqtt/mqtt_connector.py
 thingsboard_gateway/connectors/mqtt/mqtt_decorators.py
 thingsboard_gateway/connectors/mqtt/mqtt_uplink_converter.py
 thingsboard_gateway/connectors/ocpp/__init__.py
 thingsboard_gateway/connectors/ocpp/charge_point.py
```


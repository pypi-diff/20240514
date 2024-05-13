# Comparing `tmp/TDSR-UWB-1.536.tar.gz` & `tmp/TDSR-UWB-1.537.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDSR-UWB-1.536.tar", last modified: Sun May 12 20:15:36 2024, max compression
+gzip compressed data, was "TDSR-UWB-1.537.tar", last modified: Mon May 13 20:06:53 2024, max compression
```

## Comparing `TDSR-UWB-1.536.tar` & `TDSR-UWB-1.537.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-12 20:15:36.647590 TDSR-UWB-1.536/
--rw-rw-r--   0 senter    (1000) senter    (1000)       74 2024-05-09 23:00:07.000000 TDSR-UWB-1.536/LICENSE.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       37 2024-05-09 21:21:05.000000 TDSR-UWB-1.536/MANIFEST.in
--rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-12 20:15:36.647590 TDSR-UWB-1.536/PKG-INFO
--rw-rw-r--   0 senter    (1000) senter    (1000)       93 2024-05-09 23:01:32.000000 TDSR-UWB-1.536/README.md
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-12 20:15:36.643590 TDSR-UWB-1.536/TDSR-UWB/
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-12 20:15:36.643590 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-12 20:15:36.647590 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/
--rw-rw-r--   0 senter    (1000) senter    (1000)     6148 2023-03-30 19:11:25.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store
--rw-rw-r--   0 senter    (1000) senter    (1000)      161 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/.txt
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-12 20:15:36.647590 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/
--rw-rw-r--   0 senter    (1000) senter    (1000)      536 2023-03-02 20:09:11.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json
--rw-rw-r--   0 senter    (1000) senter    (1000)     9479 2023-02-26 18:51:27.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/API.md
--rw-rw-r--   0 senter    (1000) senter    (1000)     5515 2022-12-23 02:15:12.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md
--rw-rw-r--   0 senter    (1000) senter    (1000)     5563 2022-12-23 02:08:30.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md
--rw-rw-r--   0 senter    (1000) senter    (1000)       45 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/DATA_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      124 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/DATA_INFO.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      144 2023-08-10 03:26:43.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/DATA_REQUEST.txt
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-12 20:15:36.647590 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/Doc/
--rw-rw-r--   0 senter    (1000) senter    (1000)    12524 2022-10-06 21:41:33.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png
--rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       50 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      411 2023-03-30 02:12:35.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       47 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       64 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      111 2023-05-16 19:39:21.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       93 2023-05-16 19:38:24.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       61 2024-03-13 14:34:07.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       91 2024-03-13 02:20:50.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       62 2024-03-13 14:31:51.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-13 02:21:52.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-16 16:10:28.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       51 2024-03-16 16:10:10.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       44 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONNECT_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      143 2024-03-13 14:30:56.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       40 2024-03-13 01:42:44.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      379 2024-03-14 17:35:25.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       72 2024-03-14 17:30:36.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      120 2023-05-15 23:46:31.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       42 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      550 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       40 2022-12-20 14:51:26.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:18.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       43 2023-09-28 14:06:22.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      173 2024-03-13 14:33:30.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       46 2024-03-13 02:21:17.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       61 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_MESSAGE_ERROR.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       53 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       39 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       60 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       46 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       60 2024-03-13 14:32:21.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       87 2024-03-13 02:21:36.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      138 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONNECT_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       55 2024-03-13 14:35:17.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      116 2024-03-13 02:22:22.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       62 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       56 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      184 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-09-28 14:06:26.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:29.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      348 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_INFO.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       81 2023-05-16 19:37:46.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)    12521 2023-03-30 01:57:06.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/networking.md
--rw-rw-r--   0 senter    (1000) senter    (1000)   107545 2023-03-30 01:57:24.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf
--rw-rw-r--   0 senter    (1000) senter    (1000)     9971 2023-03-30 01:57:02.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md
--rw-rw-r--   0 senter    (1000) senter    (1000)     6747 2023-03-04 15:21:05.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md
--rw-rw-r--   0 senter    (1000) senter    (1000)      157 2022-12-08 14:50:04.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/processJSONFiles.sh
--rw-rw-r--   0 senter    (1000) senter    (1000)     1097 2023-03-02 20:30:55.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py
--rw-rw-r--   0 senter    (1000) senter    (1000)   250067 2024-05-12 20:07:11.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     6230 2024-05-10 15:18:23.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_logging.py
--rw-rw-r--   0 senter    (1000) senter    (1000)    14320 2024-05-12 17:20:28.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py
--rw-rw-r--   0 senter    (1000) senter    (1000)    15138 2024-05-12 20:04:54.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py
--rw-rw-r--   0 senter    (1000) senter    (1000)    82001 2024-05-12 20:06:04.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_radioControl.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     3843 2024-05-11 19:59:04.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_settings.py
--rw-rw-r--   0 senter    (1000) senter    (1000)        0 2024-05-08 17:38:57.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/__init__.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     2912 2022-12-27 01:25:43.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/crc16.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     2121 2024-04-15 16:20:28.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/logReader.py
--rw-rw-r--   0 senter    (1000) senter    (1000)      376 2024-04-15 16:19:41.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/logReader_Minimal.py
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-12 20:15:36.647590 TDSR-UWB-1.536/TDSR-UWB/TDSR_UWB.egg-info/
--rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-12 20:15:36.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO
--rw-rw-r--   0 senter    (1000) senter    (1000)     4735 2024-05-12 20:15:36.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)        1 2024-05-12 20:15:36.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_UWB.egg-info/dependency_links.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       29 2024-05-12 20:15:36.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_UWB.egg-info/requires.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       13 2024-05-12 20:15:36.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_UWB.egg-info/top_level.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       38 2024-05-12 20:15:36.647590 TDSR-UWB-1.536/setup.cfg
--rw-rw-r--   0 senter    (1000) senter    (1000)     7654 2024-05-12 20:12:53.000000 TDSR-UWB-1.536/setup.py
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-13 20:06:53.355016 TDSR-UWB-1.537/
+-rw-rw-r--   0 senter    (1000) senter    (1000)       74 2024-05-09 23:00:07.000000 TDSR-UWB-1.537/LICENSE.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       37 2024-05-09 21:21:05.000000 TDSR-UWB-1.537/MANIFEST.in
+-rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-13 20:06:53.355016 TDSR-UWB-1.537/PKG-INFO
+-rw-rw-r--   0 senter    (1000) senter    (1000)       93 2024-05-09 23:01:32.000000 TDSR-UWB-1.537/README.md
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-13 20:06:53.351016 TDSR-UWB-1.537/TDSR-UWB/
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-13 20:06:53.351016 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-13 20:06:53.355016 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/
+-rw-rw-r--   0 senter    (1000) senter    (1000)     6148 2023-03-30 19:11:25.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store
+-rw-rw-r--   0 senter    (1000) senter    (1000)      161 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/.txt
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-13 20:06:53.355016 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/
+-rw-rw-r--   0 senter    (1000) senter    (1000)      536 2023-03-02 20:09:11.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json
+-rw-rw-r--   0 senter    (1000) senter    (1000)     9479 2023-02-26 18:51:27.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/API.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)     5515 2022-12-23 02:15:12.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)     5563 2022-12-23 02:08:30.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)       45 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/DATA_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      124 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/DATA_INFO.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      144 2023-08-10 03:26:43.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/DATA_REQUEST.txt
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-13 20:06:53.355016 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/Doc/
+-rw-rw-r--   0 senter    (1000) senter    (1000)    12524 2022-10-06 21:41:33.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png
+-rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       50 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      411 2023-03-30 02:12:35.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       47 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       64 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      111 2023-05-16 19:39:21.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       93 2023-05-16 19:38:24.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       61 2024-03-13 14:34:07.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       91 2024-03-13 02:20:50.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       62 2024-03-13 14:31:51.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-13 02:21:52.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-16 16:10:28.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       51 2024-03-16 16:10:10.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       44 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONNECT_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      143 2024-03-13 14:30:56.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       40 2024-03-13 01:42:44.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      379 2024-03-14 17:35:25.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       72 2024-03-14 17:30:36.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      120 2023-05-15 23:46:31.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       42 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      550 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       40 2022-12-20 14:51:26.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:18.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       43 2023-09-28 14:06:22.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      173 2024-03-13 14:33:30.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       46 2024-03-13 02:21:17.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       61 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_MESSAGE_ERROR.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       53 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       39 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       60 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       46 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       60 2024-03-13 14:32:21.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       87 2024-03-13 02:21:36.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      138 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONNECT_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       55 2024-03-13 14:35:17.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      116 2024-03-13 02:22:22.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       62 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       56 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      184 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-09-28 14:06:26.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:29.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      348 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_INFO.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       81 2023-05-16 19:37:46.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)    12521 2023-03-30 01:57:06.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/networking.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)   107545 2023-03-30 01:57:24.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf
+-rw-rw-r--   0 senter    (1000) senter    (1000)     9971 2023-03-30 01:57:02.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)     6747 2023-03-04 15:21:05.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)      157 2022-12-08 14:50:04.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/processJSONFiles.sh
+-rw-rw-r--   0 senter    (1000) senter    (1000)     1097 2023-03-02 20:30:55.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)   253636 2024-05-13 19:27:48.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     6230 2024-05-13 17:27:19.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/TDSR_logging.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)    14404 2024-05-13 19:48:10.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)    18614 2024-05-13 18:51:27.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)    82410 2024-05-13 19:55:24.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/TDSR_radioControl.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     3986 2024-05-13 17:26:57.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/TDSR_settings.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)        0 2024-05-08 17:38:57.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/__init__.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     2912 2022-12-27 01:25:43.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/crc16.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     2121 2024-04-15 16:20:28.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/logReader.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)      376 2024-04-15 16:19:41.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/logReader_Minimal.py
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-13 20:06:53.355016 TDSR-UWB-1.537/TDSR-UWB/TDSR_UWB.egg-info/
+-rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-13 20:06:53.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO
+-rw-rw-r--   0 senter    (1000) senter    (1000)     4735 2024-05-13 20:06:53.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)        1 2024-05-13 20:06:53.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_UWB.egg-info/dependency_links.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       61 2024-05-13 20:06:53.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_UWB.egg-info/requires.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       13 2024-05-13 20:06:53.000000 TDSR-UWB-1.537/TDSR-UWB/TDSR_UWB.egg-info/top_level.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       38 2024-05-13 20:06:53.355016 TDSR-UWB-1.537/setup.cfg
+-rw-rw-r--   0 senter    (1000) senter    (1000)     7692 2024-05-13 18:28:26.000000 TDSR-UWB-1.537/setup.py
```

### Comparing `TDSR-UWB-1.536/PKG-INFO` & `TDSR-UWB-1.537/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDSR-UWB
-Version: 1.536
+Version: 1.537
 Summary: Support libraries for TDSR LLC UWB Radios
 Home-page: UNKNOWN
 Author: TDSR-LLC
 Author-email: contact@tdsr-uwb.com
 License: UNKNOWN
 Project-URL: Company:, https://www.tdsr-uwb.com
 Platform: UNKNOWN
```

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/API.md` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/API.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/networking.md` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/networking.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from TDSR_Support import TDSR_logging
 from TDSR_Support import TDSR_settings
 from TDSR_Support import TDSR_radioControl
 from TDSR_Support import TDSR_radioConnection
 
 # Primary window GUI class. All sub windows are launched from here as well.
-__version__ = "1.536"
+__version__ = "1.537"
 # Primary application window and GUI
 class MainWindow(QMainWindow):
     def __init__(self, app, *args, **kwargs):
         super(MainWindow, self).__init__(*args, **kwargs)
         title = "PennyWhistle Ranging GUI V" + __version__
         self.setWindowTitle(title)
         self.myScreen = app.primaryScreen()                      # self is mainwindow Widget and myScreen is the display it lives on
@@ -117,16 +117,22 @@
         self.stdNoiseMin = 20000
         self.maxNoiseMax = -10
         self.maxNoiseMin = 20000
         self.destSlotDataMax = 100
         self.consoleBuf = ""
         self.logFile = TDSR_logging.logData(self)
         self.radioScanComplete = False
+        # tmp1 = TDSR_radioConnection.Radio(self, self.messageTypes, 'None', "", "")
+        # tmp = tmp1.getMulticast()
+        # print()
+        # print(tmp)
+        # print()
+        # print(tmp.keys())
         self.usbRadios = self.getUSBPorts()
-        self.radioConnectMultiCast()
+        # self.radioConnectMultiCast()
         self.ipRadios = self.getMultiCastRadioIPs()
         self.radioScanComplete = False
         self.compileRadioList()
         self.radioScanComplete = True
         self.radioConnectReq()
         self.radioConnectResp()
         self.statsTimer = QTimer()
@@ -162,15 +168,15 @@
                     self.radioReq = TDSR_radioConnection.Radio(self, self.messageTypes, radio['type'], radio['addr'], radio['port'])
             if self.radioReq == None:
                 self.radioReq = TDSR_radioConnection.Radio(self, self.messageTypes, 'None', 'None', 'None')
             if self.radioReq.status == False:
                 if self.appSettings['reqRadio'] == "Disconnect":
                     print("Not connected to a primary radio")
                 else:
-                    print(f"Could not connect to Radio: {self.appSettings['reqRadio']}")
+                    print(f"Could not connect to primary radio: {self.appSettings['reqRadio']}")
                 self.connectedRequester = 0
                 self.windowDataTransfer.radioData.reqMsgTimer.stop()
                 self.chipTempTimer.stop()
                 self.dispChipTemp.setText("-")
             else:
                 self.windowDataTransfer.radioData.reqMsgTimer.start()
                 self.radioConfigReq, addr = self.radioReq.API.radio_GetConfig_Request(self.appSettings['reqRadio'], self.configID)
@@ -193,15 +199,18 @@
                 radioName = self.appSettings['respRadio']
                 for radio in self.radioList:
                     if radioName == radio['name'] and radioName != 'Disconnect':
                         self.radioResp = TDSR_radioConnection.Radio(self, self.messageTypes, radio['type'], radio['addr'], radio['port'])
                 if self.radioResp == None:
                     self.radioResp = TDSR_radioConnection.Radio(self, self.messageTypes, 'None', 'None', 'None')
                 if self.radioResp.status == False:
-                    print(f"Could not connect to IP Address: {self.appSettings['respRadio']}")
+                    if self.appSettings['reqRadio'] == "Disconnect":
+                        print("Not connected to a secondary radio")
+                    else:
+                        print(f"Could not connect to secondary radio: {self.appSettings['respRadio']}")
                     self.connectedResponder = 0
                     self.windowDataTransfer.radioData.respMsgTimer.stop()
                 else:
                     self.connectedResponder = 1
                     self.windowDataTransfer.radioData.respMsgTimer.start()
                     self.radioConfigResp, addr = self.radioResp.API.radio_GetConfig_Request(self.appSettings['respRadio'], self.configID)
                     self.radioStateResp, addr = self.radioResp.API.radio_GetState_Request(self.appSettings['respRadio'])
@@ -286,40 +295,55 @@
     def getReqRadioInfo(self):
         self.radioConnectReq()
         if self.connectedRequester == 1:
             stats,packet,addr = self.radioReq.API.radio_GetInfo_Request(self.appSettings['reqRadio'])
             self.showReqRadioInfo(packet)
 
     def getMultiCastRadioIPs(self):
-        self.radioConnectMultiCast()
+        multiCast = TDSR_radioConnection.Radio(self, "", 'None', "", "")
+        multiCastIPs = multiCast.getMulticast()
         ipRadios = []
-        if self.connectedMultiCast == 1:
-            stats,packet,addr = self.radioMultiCast.API.radio_GetIP_Request(self.multiCastIP)
-            sleep(.1)
-            if 'RADIO_GET_IP_CONFIRM' in packet.keys():
-                radioObj = {}
-                addr = packet['RADIO_GET_IP_CONFIRM']['ipv4']
-                radioObj['type'] = "ip"
-                radioObj['name'] = addr
-                radioObj['addr'] = addr
-                radioObj['port'] = self.radioIP_Port
-                ipRadios.append(radioObj)
-            for i in self.radioMultiCast.messageQueues:
-                while not self.radioMultiCast.messageQueues[i].empty():
-                    packet = self.radioMultiCast.messageQueues[i].get()
-                    if 'RADIO_GET_IP_CONFIRM' in packet.keys():
-                        radioObj = {}
-                        addr = packet['RADIO_GET_IP_CONFIRM']['ipv4']
-                        radioObj['type'] = "ip"
-                        radioObj['name'] = addr
-                        radioObj['addr'] = addr
-                        radioObj['port'] = self.radioIP_Port
-                        ipRadios.append(radioObj)
+        for radio in multiCastIPs.keys():
+            radioObj = {}
+            addr = radio
+            radioObj['nodeId'] = multiCastIPs[radio]['RADIO_GET_NODE_CONFIG_CONFIRM']['nodeId']
+            radioObj['type'] = "ip"
+            radioObj['name'] = addr
+            radioObj['addr'] = addr
+            radioObj['port'] = self.radioIP_Port
+            ipRadios.append(radioObj)
         return ipRadios
 
+    # def getMultiCastRadioIPs(self):
+    #     self.radioConnectMultiCast()
+    #     ipRadios = []
+    #     if self.connectedMultiCast == 1:
+    #         stats,packet,addr = self.radioMultiCast.API.radio_GetIP_Request(self.multiCastIP)
+    #         sleep(.1)
+    #         if 'RADIO_GET_IP_CONFIRM' in packet.keys():
+    #             radioObj = {}
+    #             addr = packet['RADIO_GET_IP_CONFIRM']['ipv4']
+    #             radioObj['type'] = "ip"
+    #             radioObj['name'] = addr
+    #             radioObj['addr'] = addr
+    #             radioObj['port'] = self.radioIP_Port
+    #             ipRadios.append(radioObj)
+    #         for i in self.radioMultiCast.messageQueues:
+    #             while not self.radioMultiCast.messageQueues[i].empty():
+    #                 packet = self.radioMultiCast.messageQueues[i].get()
+    #                 if 'RADIO_GET_IP_CONFIRM' in packet.keys():
+    #                     radioObj = {}
+    #                     addr = packet['RADIO_GET_IP_CONFIRM']['ipv4']
+    #                     radioObj['type'] = "ip"
+    #                     radioObj['name'] = addr
+    #                     radioObj['addr'] = addr
+    #                     radioObj['port'] = self.radioIP_Port
+    #                     ipRadios.append(radioObj)
+    #     return ipRadios
+
     def getUSBPorts(self):
         usbRadiosCheck = TDSR_radioConnection.Radio(self, self.messageTypes, 'usb', '', 'find')
         radios = usbRadiosCheck.findUsbRadios()
         usbRadios = []
         for radio in radios:
             radioObj = {}
             radioName = str(radio)
@@ -423,14 +447,15 @@
                 #     print(packet)
                 tmp = "%0.1f" % tmp
                 tmp = tmp + "(C)"
                 return tmp
             return "-"
 
     def updateGUI(self):
+        # print(self.radioReq.messageQueues['RANGE_INFO'].qsize())
         self.plotData()
         self.guiPacketUpdates(self.radioRanging.packetDisplay)
 
 # gets general radio information from responder radio if connected
     def getRespRadioInfo(self):
         self.radioConnectResp()
         if self.connectedResponder == 1:
@@ -836,14 +861,23 @@
         self.labelRangeRunTotal.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
         self.labelRangeRunTotal.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.labelRangeRunTotal.setFont(self.guiFont.guiFont18)
         self.labelRangeRunTotal.setText("Range\nRequests")
         yStart = 195
         xWidth = 130
         xStart = 715
+        self.labelRangeRate = QLabel(self)
+        self.labelRangeRate.resize(xWidth,yWidth)
+        self.labelRangeRate.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
+        self.labelRangeRate.setAlignment(Qt.AlignmentFlag.AlignCenter)
+        self.labelRangeRate.setFont(self.guiFont.guiFont18)
+        self.labelRangeRate.setText("Delay(ms)")
+        yStart = 245
+        xWidth = 130
+        xStart = 715
         self.labelGuiUpdateRate = QLabel(self)
         self.labelGuiUpdateRate.resize(xWidth,yWidth)
         self.labelGuiUpdateRate.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
         self.labelGuiUpdateRate.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.labelGuiUpdateRate.setFont(self.guiFont.guiFont18)
         self.labelGuiUpdateRate.setText("DispRate(hz)")
 
@@ -858,14 +892,26 @@
         self.dispRangeRunTotal.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
         self.dispRangeRunTotal.resize(xWidth,yWidth)
         self.dispRangeRunTotal.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.dispRangeRunTotal.setText(str(self.appSettings['rangeRequests']))
         self.dispRangeRunTotal.editingFinished.connect(self.updateRunTotal)
 
         yStart = 215
+        self.dispRangeRate = QLineEdit(self)
+        self.dispRangeRate.setToolTip('Number of milliseconds between range requests. Min = 0. No Max')
+        # self.dispRangeRate.setToolTip('GUI Update Rate. High GUI rates can cause missed ranges. Recommend 10hz, Max = 100hz')
+        self.dispRangeRate.setStyleSheet("QLineEdit {background-color: lightgreen;}")
+        self.dispRangeRate.setFont(self.guiFont.guiFont18)
+        self.dispRangeRate.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
+        self.dispRangeRate.resize(xWidth,yWidth)
+        self.dispRangeRate.setAlignment(Qt.AlignmentFlag.AlignCenter)
+        self.dispRangeRate.setText(str(self.appSettings['rangeRate']))
+        self.dispRangeRate.editingFinished.connect(self.updateRangeRate)
+
+        yStart = 265
         self.dispGuiUpdateRate = QLineEdit(self)
         self.dispGuiUpdateRate.setToolTip('GUI Update Rate. High GUI rates can cause missed ranges. Recommend 10hz, Max = 100hz')
         self.dispGuiUpdateRate.setStyleSheet("QLineEdit {background-color: lightgreen;}")
         self.dispGuiUpdateRate.setFont(self.guiFont.guiFont18)
         self.dispGuiUpdateRate.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
         self.dispGuiUpdateRate.resize(xWidth,yWidth)
         self.dispGuiUpdateRate.setAlignment(Qt.AlignmentFlag.AlignCenter)
@@ -1073,15 +1119,15 @@
         self.dispMemoryDepth.setToolTip("Number of datapoints held in range data array ring buffers.\nAffects memory usage and CPU overhead.")
         self.dispMemoryDepth.setStyleSheet("QLineEdit {background-color: lightgreen;}")
         self.dispMemoryDepth.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.dispMemoryDepth.setText(str(self.appSettings['memoryDepth']))
         self.dispChartStore.editingFinished.connect(self.updateMemoryDepth)
 
         xStart = 755
-        yStart = 255
+        yStart = 305
         xBias = 0
         yBias = 0
         xBump = 0
         yBump = 0
         xWidth = 200
         yWidth = 45
         x = 0
@@ -1089,17 +1135,17 @@
         self.labelRange = QLabel(self)
         self.labelRange.resize(xWidth,yWidth)
         self.labelRange.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
         self.labelRange.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.labelRange.setFont(self.guiFont.guiFont30)
         self.labelRange.setText("Range(m)")
         xStart = 735
-        yStart = 305
+        yStart = 365
         xWidth = 240
-        yWidth = 140
+        yWidth = 80
         self.dispRange = QLineEdit(self)
         self.dispRange.setFont(self.guiFont.guiFont50)
         self.dispRange.setStyleSheet("QLineEdit {background-color: rgb(255,255,255);}")
         self.dispRange.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
         self.dispRange.resize(xWidth,yWidth)
         self.dispRange.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.dispRange.setText("-")
@@ -1277,14 +1323,33 @@
             self.updateConsole(text)
             self.dispRangeRunTotal.setText("100")
         if int(self.dispRangeRunTotal.text()) < 1:
             text = "  == Range Request Entry Invalid. (Minumum Value = 1. Using Default ==\n"
             self.updateConsole(text)
             self.dispRangeRunTotal.setText("100")
         self.appSettings['rangeRequests'] = int(self.dispRangeRunTotal.text())
+# tests to see if range rate number is valid and updates variables and GUI
+    def updateRangeRate(self):
+        try:
+            self.appSettings['rangeRate'] = int(self.dispRangeRate.text())
+        except:
+            text = "  == Range Delay Entry Invalid. Min: 0   Max: 10,000   Default: 5 ==\n"
+            # text = "  == Range Rate Entry Invalid. (0.001Hz to 350Hz. Using Default 200Hz ==\n"
+            self.updateConsole(text)
+            self.dispRangeRate.setText("5")
+        if int(self.dispRangeRate.text()) > 10000 or float(self.dispGuiUpdateRate.text()) < 0:
+            text = "  == Range Delay Entry Invalid. Min: 0   Max: 10,000   Default: 5 ==\n"
+            self.updateConsole(text)
+            self.dispRangeRate.setText("5")
+        self.appSettings['rangeRate'] = self.dispRangeRate.text()
+        rangeRate = 1 + int(self.dispRangeRate.text())
+        self.radioRanging.rangeTimer.stop()
+        self.radioRanging.rangeTimer.setInterval(rangeRate)
+        # rangeRate = int(1000*(1/(int(self.dispRangeRate.text()))))
+        # self.radioRanging.rangeTimer.setInterval(rangeRate)
 # tests to see if range delay number is valid and updates variables and GUI
     def updateGuiUpdateRate(self):
         try:
             self.appSettings['guiUpdateRate'] = int(self.dispGuiUpdateRate.text())
         except:
             text = "  == GUI Update Rate Entry Invalid. (1Hz to 100Hz. Using Default 10Hz ==\n"
             self.updateConsole(text)
@@ -4416,14 +4481,15 @@
                 status = self.gui.radioRanging.rangingSetup('networking')
                 if status == True:
                     # setup the networking state
                     self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['state'] = "RADIO_STATE_NETWORKING"
                     self.layoutTop.itemAt(len(self.layoutTop)-1).widget().setText("Stop Network")
                     self.layoutTop.itemAt(len(self.layoutTop)-1).widget().setStyleSheet("QPushButton {background-color: coral; color: black;}")
                     self.gui.radioMode = 'networking'
+                    self.gui.radioCheckTimer.stop()
                     self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['flags']  = ""
                     self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['persistFlag'] = 1
                     self.gui.radioReq.API.radio_SetState_Request(self.gui.appSettings['reqRadio'],self.gui.radioStateReq)
                     self.gui.windowDataTransfer.radioData.reqMsgTimer.stop()
                     self.gui.windowDataTransfer.radioData.respMsgTimer.stop()
                     self.updateDestMenu()
                     self.resetDataArrays()
@@ -4437,23 +4503,25 @@
                     self.gui.updateConsole(text)
                     self.gui.radioRanging.networkTimer.start()
                     self.netGuiTimer.start()
                 else:
                     text = "Could not connect to requester radio, check cables and IP addresses.\n"
                     self.gui.updateConsole(text)
                     self.gui.radioMode = 'idle'
+                    self.gui.radioCheckTimer.start()
             else:
                 if self.gui.radioMode == 'networking':
                     # self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['state'] = "RADIO_STATE_IDLE"
                     self.gui.dispRespID.setText(str(self.savedNodeId))
                     self.gui.dispRespID.setStyleSheet("QLineEdit {background-color: lightgreen;}")
                     self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['state'] = "RADIO_STATE_RANGING"
                     self.layoutTop.itemAt(len(self.layoutTop)-1).widget().setText("Start Network")
                     self.layoutTop.itemAt(len(self.layoutTop)-1).widget().setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
                     self.gui.radioMode = 'idle'
+                    self.gui.radioCheckTimer.start()
                     self.gui.radioRanging.networkTimer.stop()
                     # self.gui.guiUpdateTimer.stop()
                     self.netGuiTimer.stop()
                     self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['flags']  = ""
                     self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['persistFlag'] = 1
                     self.gui.radioReq.API.radio_SetState_Request(self.gui.appSettings['reqRadio'],self.gui.radioStateReq)
                     if self.gui.connectedResponder == 1:
```

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_logging.py` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/TDSR_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime, date
 from time import time
 from pathlib import Path
 from os import path, mkdir, makedirs
 from json import dumps
 
-__version__ = "1.536"
+__version__ = "1.537"
 
 # All application data logging functions
 class logData():
     def __init__(self, gui):
         self.gui = gui
         self.settings = gui.appSettings
         self.logFile = ""
```

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from json import dumps
 from time import sleep
 
-__version__ = "1.536"
+__version__ = "1.537"
 
 class RadioAPI:
     _msgId = 0
 
     def __init__(self, messageQueues, messageList, TxQueue):
         self.TxQueue = TxQueue
         self.messageList = messageList
@@ -204,19 +204,20 @@
     def radio_Get_Active_Preset_Request(self, ip):
         message = self.getMessageFromList('RADIO_GET_ACTIVE_PRESET_REQUEST')
         # print(message)
         status, packet, addr = self.readPacketRequestConfirm(message,'RADIO_GET_ACTIVE_PRESET_CONFIRM',ip )
         return packet,addr
 
 # Ranging Command section
-    def range_Send_Request(self,ip, responderId, encoding, data):
+    def range_Send_Request(self,ip, responderId, rangeMethod, encoding, data):
         message = self.getMessageFromList('RANGE_SEND_RANGE_REQUEST')
         message[list(message.keys())[0]]['responderId'] = responderId
         message[list(message.keys())[0]]['encoding'] = "ENCODING_BASE64"
         message[list(message.keys())[0]]['data'] = data
+        message[list(message.keys())[0]]['rangeMethod'] = rangeMethod
         status, packet, addr = self.readPacketRequestConfirm(message,'RANGE_SEND_RANGE_CONFIRM',ip,retryCount  = 1 )
         return status,packet,addr
 
     def getMessageFromList(self,messageName):
         messages = [value for key, value in self.messageList.items() if messageName.upper() in key.upper()]
         #for key, value in self.messageList.items():
             #print(key.upper())
```

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,22 +3,33 @@
 import struct
 import queue
 import threading
 from json import loads
 from time import sleep
 import serial
 import serial.tools.list_ports
+import ipaddress
+import netifaces
 
 from TDSR_Support import TDSR_radioAPI
 
-__version__ = "1.536"
+__version__ = "1.537"
 
 if os.name == "nt":
     import winreg as compat_winreg
 
+# Use netifaces to find local IP addresses.
+netifaces_available = False
+try:
+    import netifaces
+    netifaces_available = True
+
+except ImportError as e:
+    netifaces_available = False
+
 class Radio:
     def __init__(self, gui, messageTypes, interfaceType, interfaceAddr, interfacePort):
         # def __init__(self, gui, messageTypes, interface, interfaceAddr, interfacePort):
         self.TxQueue = queue.Queue()
         # print(interfaceAddr, self.TxQueue)
         self.gui = gui
         self.shutDownThreads = False
@@ -121,14 +132,74 @@
         ports = [port for port in serial.tools.list_ports.comports() if port != "n/a" and port.vid == 0x1027 and port.pid == 0x1234]
         # print(ports)
         for radio in ports:
             radios.append(radio)
             # print(radio)
         return radios
 
+    def getMulticast(self):
+        timeout = 0.1
+        local_ipv4_interfaces = []
+        ifaces = netifaces.interfaces()
+        for iface in ifaces:
+            addrs = netifaces.ifaddresses(iface)
+            if netifaces.AF_INET in addrs.keys():
+                if len(addrs[netifaces.AF_INET]) >= 1:
+                    # Confirm it has an "addr" key for the IP address (should always), and that it doesn't have a "peer" key to avoid loopback addresses.
+                    if "addr" in addrs[netifaces.AF_INET][0].keys() and "peer" not in addrs[netifaces.AF_INET][0].keys():
+                        local_ipv4_interfaces.append(addrs[netifaces.AF_INET][0]['addr'])
+        # Create and bind list of sockets
+        sockets = [socket.socket(socket.AF_INET, socket.SOCK_DGRAM) for i in range(len(local_ipv4_interfaces))]
+        [sockets[i].bind((local_ipv4_interfaces[i], 0)) for i in range(len(local_ipv4_interfaces))]
+        # Basic RADIO_GET_INFO_REQUEST to send out
+        req_str = '{"RADIO_GET_NODE_CONFIG_REQUEST":{"msgId":100}}'
+        # Send to the multicast address and port 8890, on each provided IP interface.
+        [s.sendto(req_str.encode(), ("239.255.92.43", 8890)) for s in sockets]
+        # Now receive RADIO_GET_INFO_CONFIRMs and store in a dict.
+        # Dict will be {key, value} of {IPv4 address string, RADIO_GET_INFO_CONFIRM object}
+        found_radios = {}
+        # Receive messages up to the timeout. Any that match expected parameters will add a radio to our list.
+        sleep(timeout)
+        # Check all interfaces and receive data.
+        for s in sockets:
+            # Read packets in a loop until there are none left
+            while True:
+                rx_data = None
+                rx_source = None
+                try:
+                    # Receive a message (if any)
+                    s.setblocking(False)
+                    rx = s.recvfrom(1600)
+                    if rx is None:
+                        # No data to receive
+                        break
+                    rx_data, rx_source = rx
+                except (TimeoutError, BlockingIOError):
+                    # No data to receive
+                    break
+                if rx_data is None or rx_source is None:
+                    break
+                # Try converting it to a RADIO_GET_INFO_CONFIRM
+                try:
+                    rx_obj = loads(rx_data)
+                    if len(rx_obj.keys()) != 1:
+                        # Not a valid API message
+                        continue
+                    if "RADIO_GET_NODE_CONFIG_CONFIRM" not in rx_obj.keys():
+                        # May or may not be an API message, but it's not the API message type we're looking for
+                        continue
+                    if rx_obj["RADIO_GET_NODE_CONFIG_CONFIRM"]["msgId"] != 100:
+                        # Wrong msgId. Really not likely to happen at this point, but msgId should have matched, so reject it.
+                        continue
+                    # Add it to the list!
+                    found_radios[rx_source[0]] = rx_obj
+                except ValueError:
+                    continue
+        return found_radios
+
     def connectIP(self):
         if self.radioIf != None:
             print("Radio is already connected")
         self.radioIf = radioIfIp(self.interfaceAddr, self.interfacePort)             #  Radio Interface Socket
         status = self.radioIf.connect()   # opens socket and starts read thread for radio to host input FIFO.
         if status == True:
             if self.interfacePort == 8888:
```

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_radioControl.py` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/TDSR_radioControl.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from time import time, sleep
 from math import sqrt, log10
 from numpy import power
 from pathlib import Path
 from base64 import b64encode, b64decode
 from threading import Thread
 
-__version__ = "1.536"
+__version__ = "1.537"
 
 # Primary ranging functions
 class rangeCmds():
     def __init__(self, gui):
         self.gui = gui
         self.appSetup()
 
@@ -25,15 +25,15 @@
         if self.gui.connectedRequester == 1:
             self.rangingSetup('ranging')
 
 # only runs once on startup. Initial setup for application
     def appSetup(self):
         self.running = 0
         self.rangeTimer = QTimer()
-        self.rangeTimer.setInterval(1)
+        # self.rangeTimer.setInterval(10)
         self.rangeTimer.timeout.connect(self.rangeRequest)
         self.networkTimer = QTimer()
         self.networkTimer.setInterval(10)
         self.networkTimer.timeout.connect(self.networkCheck)
         self.rangeArray = []
         self.rangeFilteredArray = []
         self.rangeFPPArray = []
@@ -163,22 +163,22 @@
                 self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['state'] = "RADIO_STATE_RANGING"
                 self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['flags']  = ""
                 self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['persistFlag'] = 1
                 self.gui.radioReq.API.radio_SetState_Request(self.gui.appSettings['reqRadio'],self.gui.radioStateReq)
                 self.gui.windowDataTransfer.dropMenuDestination.clear()
                 self.gui.windowDataTransfer.dropMenuDestination.addItems([str(self.gui.appSettings['respID'])])
                 self.gui.checkChartRange(None)
-                self.runStartTime = time()
                 self.running = 1
                 self.gui.but_run.setText("Stop")
                 self.gui.but_run.setStyleSheet("QPushButton {background-color: coral;}")
                 if self.gui.connectedRequester == 0:
                     self.gui.radioConnectReq()
-                if self.gui.connectedRequester == 1 and self.gui.connectedRequester == 1:
+                if self.gui.connectedRequester == 1:
                     # self.rangeTimer.setInterval(int(self.gui.dispRangeDelay.text()))
+                    self.runStartTime = time()
                     self.rangeTimer.start()
                     self.gui.rangingActive = True
                     self.gui.guiUpdateTimer.start()
                     text = "Executing " + str(self.gui.appSettings['rangeRequests']) + " Ranging Attempts\n"
                     self.gui.updateConsole(text)
                     self.gui.radioMode = 'ranging'
                     self.gui.radioCheckTimer.stop()
@@ -229,32 +229,39 @@
             while not self.gui.radioReq.messageQueues['DATA_INFO'].empty():
                 packet =  self.gui.radioReq.messageQueues['DATA_INFO'].get()
                 self.gui.windowDataTransfer.radioData.processNetworkDataInfo(packet)
             self.networkTimer.start()
 
 # Requests range from designated responder nodeID.
     def rangeRequest(self):
-        self.rangeTimer.stop()
+        # self.rangeTimer.stop()
         if self.missedComms > 4:
             print("rangeRequest abort")
             self.gui.radioReq.disconnect()
             self.gui.dropMenuReqRadio.setCurrentIndex(0)
             self.missedComms = 0
         if self.gui.connectedRequester == 1:
             self.gui.rangeInProgress = 1
             # if there is data to send, append it to the ranging packet
             if self.gui.windowDataTransfer.radioData.dataReadyStatus > 0:
                 data = self.gui.windowDataTransfer.radioData.getDataPacket()
             else:
                 data = ""
             # if 0 then hold ranges to allow confirmation data packet to come in.
             if self.gui.windowDataTransfer.radioData.dataReadyStatus != 0:
-                status, pkt, addr = self.gui.radioReq.API.range_Send_Request(self.gui.appSettings['reqRadio'],self.targetNodes, "ENCODING_BASE64", data)
-                if status == False:
-                    self.missedComms = self.missedComms + 1
+                if len(data) > 0:
+                    print("4")
+                    status, pkt, addr = self.gui.radioReq.API.range_Send_Request(self.gui.appSettings['reqRadio'],self.targetNodes, "4pkt TWR", "ENCODING_BASE64", data)
+                    if status == False:
+                        self.missedComms = self.missedComms + 1
+                else:
+                    status, pkt, addr = self.gui.radioReq.API.range_Send_Request(self.gui.appSettings['reqRadio'],self.targetNodes, "2pkt TWR", "ENCODING_BASE64", data)
+                    print("2")
+                    if status == False:
+                        self.missedComms = self.missedComms + 1
             if self.gui.windowDataTransfer.radioData.dataReadyStatus == 1:  # indicated last in transmission
                 self.gui.windowDataTransfer.radioData.dataReadyStatus = 0   # enter hold until confirmation cycle
             self.startRange = time()
             # Once range request is set, wait for answer and process the data
             self.rangeProcessData(None)
         else:
             text = "== Not connected to Requester Radio" + self.gui.appSettings['reqRadio'] + " ==\n"
@@ -278,15 +285,16 @@
                 pass
         # If count = desired requests then stop run, otherwise, range transaction is complete, start the next one.
             self.gui.rangeInProgress = False
             if self.rangeCount == self.gui.appSettings['rangeRequests']:
                 print("Run Complete.")
                 self.toggleRun()
             else:
-                self.rangeTimer.start()
+                ...
+                # self.rangeTimer.start()
         # Find starting place for message IDs and then determine packet count
             if self.firstMsg == 0:
                 if packet['RANGE_INFO']['rangeStatus'] == 0  and packet['RANGE_INFO']['precisionRangeM'] != 0.0:
                     self.firstMsg = int(packet['RANGE_INFO']['msgId'])
             self.packets = self.rangeCount + 1
         # Count Ranging Errors and compute success rate, store them in the packet
             if packet['RANGE_INFO']['rangeStatus'] != 0 or packet['RANGE_INFO']['precisionRangeM'] == 0.0:
```

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_settings.py` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/TDSR_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from json import dumps, loads
 
-__version__ = "1.536"
+__version__ = "1.537"
 
 # loads and saves GUI settings. Also sets default values if settings file does not include all keys.
 class appSettings():
     def __init__(self):
         self.settings = {}
 
     def settingsSetup(self):
@@ -21,14 +21,16 @@
                 self.settings['connectResp'] = 0
             if 'chartDepth' not in self.settings:
                 self.settings['chartDepth'] = 5000
             if 'memoryDepth' not in self.settings:
                 self.settings['memoryDepth'] = 250000
             if 'rangeRequests' not in self.settings:
                 self.settings['rangeRequests'] = 250
+            if 'rangeRate' not in self.settings:
+                self.settings['rangeRate'] = 200
             if 'reqRadio' not in self.settings:
                 self.settings['reqRadio'] = "192.168.1.100"
             if 'respRadio' not in self.settings:
                 self.settings['respRadio'] = "192.168.1.101"
             if 'respID' not in self.settings:
                 self.settings['respID'] = "101"
             if 'logDirectory' not in self.settings:
@@ -56,14 +58,15 @@
         else:
             print("Creating Default Settings File")
             self.settings['showDrops'] = 0
             self.settings['connectResp'] = 0
             self.settings['chartDepth'] = 5000
             self.settings['memoryDepth'] = 250000
             self.settings['rangeRequests'] = 250
+            self.settings['rangeRate'] = 200
             self.settings['reqRadio'] = "192.168.1.51"
             self.settings['respRadio'] = "192.168.1.52"
             self.settings['respID'] = "52"
             self.settings['logDirectory'] = "./data_directory/"
             self.settings['logFile'] = "logfile.log"
             self.settings['logJson'] = 1
             self.settings['enableLogging'] = 0
```

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/crc16.py` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/crc16.py`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/logReader.py` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_Support/logReader.py`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDSR-UWB
-Version: 1.536
+Version: 1.537
 Summary: Support libraries for TDSR LLC UWB Radios
 Home-page: UNKNOWN
 Author: TDSR-LLC
 Author-email: contact@tdsr-uwb.com
 License: UNKNOWN
 Project-URL: Company:, https://www.tdsr-uwb.com
 Platform: UNKNOWN
```

### Comparing `TDSR-UWB-1.536/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt` & `TDSR-UWB-1.537/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.536/setup.py` & `TDSR-UWB-1.537/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="TDSR-UWB",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.536",  # Required
+    version="1.537",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Support libraries for TDSR LLC UWB Radios",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -120,15 +120,15 @@
     python_requires=">=3.9, <4",
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
-    install_requires=["PyQt6>=6.6", "pyqtgraph>=0.13.2"],  # Optional
+    install_requires=["PyQt6>=6.6", "pyqtgraph>=0.13.2", "netifaces>=0.11.0", "pyserial>=3.5"],  # Optional
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
     # Similar to `install_requires` above, these must be valid existing
```


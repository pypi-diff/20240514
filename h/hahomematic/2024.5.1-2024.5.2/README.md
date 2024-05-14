# Comparing `tmp/hahomematic-2024.5.1.tar.gz` & `tmp/hahomematic-2024.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2024.5.1.tar", last modified: Tue May  7 11:23:49 2024, max compression
+gzip compressed data, was "hahomematic-2024.5.2.tar", last modified: Tue May 14 15:12:07 2024, max compression
```

## Comparing `hahomematic-2024.5.1.tar` & `hahomematic-2024.5.2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.723751 hahomematic-2024.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-07 11:23:49.723751 hahomematic-2024.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.707751 hahomematic-2024.5.1/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/async_support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.711751 hahomematic-2024.5.1/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18130 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/caches/visibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.711751 hahomematic-2024.5.1/hahomematic/central/
--rw-r--r--   0 runner    (1001) docker     (127)    55184 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/central/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/central/command_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/central/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/central/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.711751 hahomematic-2024.5.1/hahomematic/client/
--rw-r--r--   0 runner    (1001) docker     (127)    46155 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34886 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/client/json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/client/xml_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.711751 hahomematic-2024.5.1/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.715752 hahomematic-2024.5.1/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26229 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    24631 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    30099 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12992 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    44054 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    33428 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    30413 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.715752 hahomematic-2024.5.1/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.719751 hahomematic-2024.5.1/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.719751 hahomematic-2024.5.1/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.723751 hahomematic-2024.5.1/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-07 11:23:49.000000 hahomematic-2024.5.1/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-07 11:23:49.000000 hahomematic-2024.5.1/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:23:49.000000 hahomematic-2024.5.1/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:23:49.000000 hahomematic-2024.5.1/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 11:23:49.000000 hahomematic-2024.5.1/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 11:23:49.000000 hahomematic-2024.5.1/hahomematic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.719751 hahomematic-2024.5.1/hahomematic_support/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic_support/client_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 11:23:49.723751 hahomematic-2024.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.723751 hahomematic-2024.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    32325 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_central.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_central_pydevccu.py
--rw-r--r--   0 runner    (1001) docker     (127)    16791 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    39142 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    17156 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.864034 hahomematic-2024.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-14 15:12:07.864034 hahomematic-2024.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.852034 hahomematic-2024.5.2/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/async_support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.852034 hahomematic-2024.5.2/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18130 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/caches/visibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.852034 hahomematic-2024.5.2/hahomematic/central/
+-rw-r--r--   0 runner    (1001) docker     (127)    55193 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/central/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/central/command_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/central/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/central/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.852034 hahomematic-2024.5.2/hahomematic/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    46155 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34886 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/client/json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/client/xml_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.856034 hahomematic-2024.5.2/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.856034 hahomematic-2024.5.2/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26229 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26938 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30203 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12992 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44054 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33434 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30391 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.860034 hahomematic-2024.5.2/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.860034 hahomematic-2024.5.2/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.860034 hahomematic-2024.5.2/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.864034 hahomematic-2024.5.2/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-14 15:12:07.000000 hahomematic-2024.5.2/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-14 15:12:07.000000 hahomematic-2024.5.2/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:12:07.000000 hahomematic-2024.5.2/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:12:07.000000 hahomematic-2024.5.2/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:12:07.000000 hahomematic-2024.5.2/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 15:12:07.000000 hahomematic-2024.5.2/hahomematic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.860034 hahomematic-2024.5.2/hahomematic_support/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic_support/client_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 15:12:07.864034 hahomematic-2024.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.864034 hahomematic-2024.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32325 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_central.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_central_pydevccu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16791 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35492 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39142 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17156 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_text.py
```

### Comparing `hahomematic-2024.5.1/LICENSE` & `hahomematic-2024.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/PKG-INFO` & `hahomematic-2024.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.5.1
+Version: 2024.5.2
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.5.1/README.md` & `hahomematic-2024.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/__init__.py` & `hahomematic-2024.5.2/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/async_support.py` & `hahomematic-2024.5.2/hahomematic/async_support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/caches/dynamic.py` & `hahomematic-2024.5.2/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/caches/persistent.py` & `hahomematic-2024.5.2/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/caches/visibility.py` & `hahomematic-2024.5.2/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/central/__init__.py` & `hahomematic-2024.5.2/hahomematic/central/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1033,15 +1033,15 @@
         self.device_details.clear()
         self.data_cache.clear()
 
     def register_homematic_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register ha_event callback in central."""
         if callable(cb) and cb not in self._homematic_callbacks:
             self._homematic_callbacks.add(cb)
-            return partial(self._unregister_homematic_callback, cb)
+            return partial(self._unregister_homematic_callback, cb=cb)
         return None
 
     def _unregister_homematic_callback(self, cb: Callable) -> None:
         """RUn register ha_event callback in central."""
         if cb in self._homematic_callbacks:
             self._homematic_callbacks.remove(cb)
 
@@ -1063,15 +1063,15 @@
                     reduce_args(args=ex.args),
                 )
 
     def register_backend_parameter_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register backend_parameter callback in central."""
         if callable(cb) and cb not in self._backend_parameter_callbacks:
             self._backend_parameter_callbacks.add(cb)
-            return partial(self._unregister_backend_parameter_callback, cb)
+            return partial(self._unregister_backend_parameter_callback, cb=cb)
         return None
 
     def _unregister_backend_parameter_callback(self, cb: Callable) -> None:
         """Un register backend_parameter callback in central."""
         if cb in self._backend_parameter_callbacks:
             self._backend_parameter_callbacks.remove(cb)
 
@@ -1094,15 +1094,15 @@
                     reduce_args(args=ex.args),
                 )
 
     def register_backend_system_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register system_event callback in central."""
         if callable(cb) and cb not in self._backend_parameter_callbacks:
             self._backend_system_callbacks.add(cb)
-            return partial(self._unregister_backend_system_callback, cb)
+            return partial(self._unregister_backend_system_callback, cb=cb)
         return None
 
     def _unregister_backend_system_callback(self, cb: Callable) -> None:
         """Un register system_event callback in central."""
         if cb in self._backend_system_callbacks:
             self._backend_system_callbacks.remove(cb)
```

### Comparing `hahomematic-2024.5.1/hahomematic/central/command_queue.py` & `hahomematic-2024.5.2/hahomematic/central/command_queue.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,48 +18,46 @@
 
     def __init__(self) -> None:
         """Init the SendCommandQueueHandler."""
         self._queues: Final[dict[str, Queue[Callable | None]]] = {}
         self._exit = False
         self._looper = Looper()
 
-    def empty_queue(self, device_address: str) -> None:
+    def empty_queue(self, address: str) -> None:
         """Empty a queue for a device."""
-        if queue := self._queues.get(device_address):
+        if queue := self._queues.get(address):
             try:
                 while not queue.empty():
                     queue.get_nowait()
                     queue.task_done()
             except QueueEmpty:
                 pass
 
-    async def put(self, device_address: str, command: Callable) -> None:
-        """Put send_command to device queue."""
-        if device_address not in self._queues:
-            device_queue: Queue[Callable | None] = Queue()
-            self._looper.create_task(
-                _device_consumer(device_queue), name=f"device_consumer-{device_address}"
-            )
-            self._queues[device_address] = device_queue
-        await self._queues[device_address].put(command)
+    async def put(self, address: str, command: Callable) -> None:
+        """Put command to queue."""
+        if address not in self._queues:
+            queue: Queue[Callable | None] = Queue()
+            self._looper.create_task(_command_consumer(queue), name=f"command consumer-{address}")
+            self._queues[address] = queue
+        await self._queues[address].put(command)
         await sleep(0.1)
 
     async def stop(self) -> None:
         """Add None to queue to stop the consumer."""
         for queue in self._queues.values():
             await queue.put(None)
         await self._looper.block_till_done()
 
 
-async def _device_consumer(queue: Queue) -> None:
-    """Consume the device commands."""
+async def _command_consumer(queue: Queue) -> None:
+    """Consume the commands."""
     # consume work
     while True:
         try:
             if (command := await queue.get()) is None:
                 break
             await command()
             queue.task_done()
         except Exception as ex:
             _LOGGER.debug(
-                "DEVICE_CONSUMER: Unable do deque command: %s", reduce_args(args=ex.args)
+                "COMMAND_CONSUMER: Unable do deque command: %s", reduce_args(args=ex.args)
             )
```

### Comparing `hahomematic-2024.5.1/hahomematic/central/decorators.py` & `hahomematic-2024.5.2/hahomematic/central/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/central/xml_rpc_server.py` & `hahomematic-2024.5.2/hahomematic/central/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/client/__init__.py` & `hahomematic-2024.5.2/hahomematic/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/client/json_rpc.py` & `hahomematic-2024.5.2/hahomematic/client/json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/client/xml_rpc.py` & `hahomematic-2024.5.2/hahomematic/client/xml_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/config.py` & `hahomematic-2024.5.2/hahomematic/config.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/const.py` & `hahomematic-2024.5.2/hahomematic/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/converter.py` & `hahomematic-2024.5.2/hahomematic/converter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/exceptions.py` & `hahomematic-2024.5.2/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/hmcli.py` & `hahomematic-2024.5.2/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/performance.py` & `hahomematic-2024.5.2/hahomematic/performance.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/__init__.py` & `hahomematic-2024.5.2/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/custom/__init__.py` & `hahomematic-2024.5.2/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/custom/climate.py` & `hahomematic-2024.5.2/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/custom/const.py` & `hahomematic-2024.5.2/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/custom/cover.py` & `hahomematic-2024.5.2/hahomematic/platforms/custom/cover.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Module for entities implemented using the cover platform.
 
 See https://www.home-assistant.io/integrations/cover/.
 """
 
 from __future__ import annotations
 
+import asyncio
 from collections.abc import Mapping
 from enum import IntEnum, StrEnum
 import logging
 from typing import Any, Final
 
 from hahomematic.const import EntityUsage, HmPlatform, Parameter
 from hahomematic.converter import convert_hm_level_to_cpv
@@ -92,14 +93,15 @@
     _platform = HmPlatform.COVER
     _closed_level: float = _CLOSED_LEVEL
     _open_level: float = _OPEN_LEVEL
 
     def _init_entity_fields(self) -> None:
         """Init the entity fields."""
         super()._init_entity_fields()
+        self._command_processing_lock = asyncio.Lock()
         self._e_direction: HmSensor = self._get_entity(field=Field.DIRECTION, entity_type=HmSensor)
         self._e_level: HmFloat = self._get_entity(field=Field.LEVEL, entity_type=HmFloat)
         self._e_stop: HmAction = self._get_entity(field=Field.STOP, entity_type=HmAction)
         self._e_channel_level: HmSensor = self._get_entity(
             field=Field.CHANNEL_LEVEL, entity_type=HmSensor
         )
 
@@ -252,15 +254,28 @@
         return self._e_level_2.value if self._e_level_2.value is not None else self._closed_level
 
     @value_property
     def current_tilt_position(self) -> int:
         """Return current tilt position of cover."""
         return int(self._channel_tilt_level * 100)
 
-    @bind_collector(use_command_queue=False)
+    @property
+    def _target_level(self) -> float | None:
+        """Return the level of last service call."""
+        if (last_value_send := self._e_level.unconfirmed_last_value_send) is not None:
+            return float(last_value_send)
+        return None
+
+    @property
+    def _target_tilt_level(self) -> float | None:
+        """Return the tilt level of last service call."""
+        if (last_value_send := self._e_level_2.unconfirmed_last_value_send) is not None:
+            return float(last_value_send)
+        return None
+
     async def set_position(
         self,
         position: int | None = None,
         tilt_position: int | None = None,
         collector: CallParameterCollector | None = None,
     ) -> None:
         """Move the blind to a specific position."""
@@ -275,69 +290,108 @@
     async def _set_level(
         self,
         level: float | None = None,
         tilt_level: float | None = None,
         collector: CallParameterCollector | None = None,
     ) -> None:
         """
-        Move the cover to a specific tilt level. Value range is 0.0 to 1.01.
+        Move the cover to a specific tilt level. Value range is 0.0 to 1.00.
 
-        1.01 means no change.
+        level or tilt_level may be set to None for no change.
         """
-        _level = level if level is not None else self.current_position / 100.0
-        _tilt_level = tilt_level if tilt_level is not None else self.current_tilt_position / 100.0
+        currently_moving = False
+
+        async with self._command_processing_lock:
+            if level is not None:
+                _level = level
+            elif self._target_level is not None:
+                # The blind moves and the target blind height is known
+                currently_moving = True
+                _level = self._target_level
+            else:  # The blind is at a standstill and no level is explicitly requested => we remain at the current level
+                _level = self._channel_level
+
+            if tilt_level is not None:
+                _tilt_level = tilt_level
+            elif self._target_tilt_level is not None:
+                # The blind moves and the target slat position is known
+                currently_moving = True
+                _tilt_level = self._target_tilt_level
+            else:  # The blind is at a standstill and no tilt is explicitly desired => we remain at the current angle
+                _tilt_level = self._channel_tilt_level
+
+            if currently_moving:
+                # Blind actors are buggy when sending new coordinates while they are moving. So we stop them first.
+                await self._stop()
+
+            await self._send_level(level=_level, tilt_level=_tilt_level, collector=collector)
+
+    @bind_collector()
+    async def _send_level(
+        self,
+        level: float,
+        tilt_level: float,
+        collector: CallParameterCollector | None = None,
+    ) -> None:
+        """Transmit a new target level to the device."""
         if self._e_combined.is_hmtype and (
-            combined_parameter := self._get_combined_value(level=_level, tilt_level=_tilt_level)
+            combined_parameter := self._get_combined_value(level=level, tilt_level=tilt_level)
         ):
             await self._e_combined.send_value(value=combined_parameter, collector=collector)
             return
 
-        await self._e_level_2.send_value(value=_tilt_level, collector=collector)
-        await super()._set_level(level=_level, collector=collector)
+        await self._e_level_2.send_value(value=tilt_level, collector=collector)
+        await super()._set_level(level=level, collector=collector)
 
-    @bind_collector(use_command_queue=False)
     async def open(self, collector: CallParameterCollector | None = None) -> None:
         """Open the cover and open the tilt."""
         if not self.is_state_change(open=True, tilt_open=True):
             return
         await self._set_level(
             level=self._open_level,
             tilt_level=self._open_tilt_level,
             collector=collector,
         )
 
-    @bind_collector(use_command_queue=False)
     async def close(self, collector: CallParameterCollector | None = None) -> None:
         """Close the cover and close the tilt."""
         if not self.is_state_change(close=True, tilt_close=True):
             return
         await self._set_level(
             level=self._closed_level,
             tilt_level=self._closed_level,
             collector=collector,
         )
 
-    @bind_collector(use_command_queue=False)
+    async def stop(self, collector: CallParameterCollector | None = None) -> None:
+        """Stop the device if in motion."""
+        async with self._command_processing_lock:
+            await self._stop(collector=collector)
+
+    @bind_collector()
+    async def _stop(self, collector: CallParameterCollector | None = None) -> None:
+        """Stop the device if in motion. Do only call with _command_processing_lock held."""
+        self.central.command_queue_handler.empty_queue(address=self._channel_address)
+        await super().stop(collector=collector)
+
     async def open_tilt(self, collector: CallParameterCollector | None = None) -> None:
         """Open the tilt."""
         if not self.is_state_change(tilt_open=True):
             return
         await self._set_level(tilt_level=self._open_tilt_level, collector=collector)
 
-    @bind_collector(use_command_queue=False)
     async def close_tilt(self, collector: CallParameterCollector | None = None) -> None:
         """Close the tilt."""
         if not self.is_state_change(tilt_close=True):
             return
         await self._set_level(tilt_level=self._closed_level, collector=collector)
 
-    @bind_collector()
     async def stop_tilt(self, collector: CallParameterCollector | None = None) -> None:
-        """Stop the device if in motion."""
-        await self._e_stop.send_value(value=True, collector=collector)
+        """Stop the device if in motion. Use only when command_processing_lock is held."""
+        await self.stop(collector=collector)
 
     def is_state_change(self, **kwargs: Any) -> bool:
         """Check if the state changes due to kwargs."""
         if (
             tilt_position := kwargs.get(StateChangeArg.TILT_POSITION)
         ) is not None and tilt_position != self.current_tilt_position:
             return True
```

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/custom/definition.py` & `hahomematic-2024.5.2/hahomematic/platforms/custom/definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,17 +89,21 @@
                     Field.LEVEL: Parameter.LEVEL,
                     Field.LEVEL_2: Parameter.LEVEL_2,
                     Field.STOP: Parameter.STOP,
                 },
                 ED.FIELDS: {
                     0: {
                         Field.DIRECTION: Parameter.ACTIVITY_STATE,
+                        Field.CHANNEL_OPERATION_MODE: Parameter.CHANNEL_OPERATION_MODE,
+                    },
+                },
+                ED.VISIBLE_FIELDS: {
+                    0: {
                         Field.CHANNEL_LEVEL: Parameter.LEVEL,
                         Field.CHANNEL_LEVEL_2: Parameter.LEVEL_2,
-                        Field.CHANNEL_OPERATION_MODE: Parameter.CHANNEL_OPERATION_MODE,
                     },
                 },
             },
         },
         DeviceProfile.IP_DIMMER: {
             ED.DEVICE_GROUP: {
                 ED.PRIMARY_CHANNEL: 1,
```

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/custom/entity.py` & `hahomematic-2024.5.2/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/custom/light.py` & `hahomematic-2024.5.2/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/custom/lock.py` & `hahomematic-2024.5.2/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/custom/siren.py` & `hahomematic-2024.5.2/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/custom/support.py` & `hahomematic-2024.5.2/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/custom/switch.py` & `hahomematic-2024.5.2/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/decorators.py` & `hahomematic-2024.5.2/hahomematic/platforms/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/device.py` & `hahomematic-2024.5.2/hahomematic/platforms/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,27 +393,27 @@
             self.remove_entity(custom_entity)
         self._custom_entities.clear()
 
     def _register_device_updated_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register update callback."""
         if callable(cb) and cb not in self._device_updated_callbacks:
             self._device_updated_callbacks.append(cb)
-            return partial(self._unregister_device_updated_callback, cb)
+            return partial(self._unregister_device_updated_callback, cb=cb)
         return None
 
     def _unregister_device_updated_callback(self, cb: Callable) -> None:
         """Remove update callback."""
         if cb in self._device_updated_callbacks:
             self._device_updated_callbacks.remove(cb)
 
     def register_firmware_update_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register firmware update callback."""
         if callable(cb) and cb not in self._firmware_update_callbacks:
             self._firmware_update_callbacks.append(cb)
-            return partial(self.unregister_firmware_update_callback, cb)
+            return partial(self.unregister_firmware_update_callback, cb=cb)
         return None
 
     def unregister_firmware_update_callback(self, cb: Callable) -> None:
         """Remove firmware update callback."""
         if cb in self._firmware_update_callbacks:
             self._firmware_update_callbacks.remove(cb)
```

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/entity.py` & `hahomematic-2024.5.2/hahomematic/platforms/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,29 +196,29 @@
                 raise HaHomematicException(
                     f"REGISTER_entity_updated_CALLBACK failed: hm_entity: {self.full_name} is already registered by {self._custom_id}"
                 )
             self._custom_id = custom_id
 
         if callable(cb) and cb not in self._entity_updated_callbacks:
             self._entity_updated_callbacks[cb] = custom_id
-            return partial(self._unregister_entity_updated_callback, cb, custom_id)
+            return partial(self._unregister_entity_updated_callback, cb=cb, custom_id=custom_id)
         return None
 
     def _unregister_entity_updated_callback(self, cb: Callable, custom_id: str) -> None:
         """Unregister entity updated callback."""
         if cb in self._entity_updated_callbacks:
             del self._entity_updated_callbacks[cb]
         if self.custom_id == custom_id:
             self._custom_id = None
 
     def register_device_removed_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register the device removed callback."""
         if callable(cb) and cb not in self._device_removed_callbacks:
             self._device_removed_callbacks.append(cb)
-            return partial(self._unregister_device_removed_callback, cb)
+            return partial(self._unregister_device_removed_callback, cb=cb)
         return None
 
     def _unregister_device_removed_callback(self, cb: Callable) -> None:
         """Unregister the device removed callback."""
         if cb in self._device_removed_callbacks:
             self._device_removed_callbacks.remove(cb)
 
@@ -791,30 +791,30 @@
                             paramset_key=ParamsetKey.VALUES,
                             parameter=parameter,
                             value=value,
                             wait_for_callback=wait_for_callback,
                         )
                         if use_command_queue:
                             await self._device.central.command_queue_handler.put(
-                                device_address=self._device.device_address,
+                                address=channel_address,
                                 command=set_value_command,
                             )
                         elif not await set_value_command():
                             return False  # pragma: no cover
                 else:
                     put_paramset_command = partial(
                         self._client.put_paramset,
                         channel_address=channel_address,
                         paramset_key=ParamsetKey.VALUES,
                         values=paramset,
                         wait_for_callback=wait_for_callback,
                     )
                     if use_command_queue:
                         await self._device.central.command_queue_handler.put(
-                            device_address=self._device.device_address,
+                            address=channel_address,
                             command=put_paramset_command,
                         )
                     elif not await put_paramset_command():
                         return False  # pragma: no cover
         return True
```

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/event.py` & `hahomematic-2024.5.2/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/generic/__init__.py` & `hahomematic-2024.5.2/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/generic/action.py` & `hahomematic-2024.5.2/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2024.5.2/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/generic/button.py` & `hahomematic-2024.5.2/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/generic/entity.py` & `hahomematic-2024.5.2/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/generic/number.py` & `hahomematic-2024.5.2/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/generic/select.py` & `hahomematic-2024.5.2/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/generic/sensor.py` & `hahomematic-2024.5.2/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/generic/switch.py` & `hahomematic-2024.5.2/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/hub/__init__.py` & `hahomematic-2024.5.2/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2024.5.2/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/hub/button.py` & `hahomematic-2024.5.2/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/hub/entity.py` & `hahomematic-2024.5.2/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/hub/number.py` & `hahomematic-2024.5.2/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/hub/select.py` & `hahomematic-2024.5.2/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/hub/sensor.py` & `hahomematic-2024.5.2/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/hub/text.py` & `hahomematic-2024.5.2/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/support.py` & `hahomematic-2024.5.2/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/platforms/update.py` & `hahomematic-2024.5.2/hahomematic/platforms/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             if self._custom_id is not None:
                 raise HaHomematicException(
                     f"REGISTER_UPDATE_CALLBACK failed: hm_entity: {self.full_name} is already registered by {self._custom_id}"
                 )
             self._custom_id = custom_id
 
         if self._device.register_firmware_update_callback(cb) is not None:
-            return partial(self._unregister_entity_updated_callback, cb, custom_id)
+            return partial(self._unregister_entity_updated_callback, cb=cb, custom_id=custom_id)
         return None
 
     def _unregister_entity_updated_callback(self, cb: Callable, custom_id: str) -> None:
         """Unregister update callback."""
         if custom_id is not None:
             self._custom_id = None
         self._device.unregister_firmware_update_callback(cb)
```

### Comparing `hahomematic-2024.5.1/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2024.5.2/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2024.5.2/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2024.5.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic/support.py` & `hahomematic-2024.5.2/hahomematic/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic.egg-info/PKG-INFO` & `hahomematic-2024.5.2/hahomematic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.5.1
+Version: 2024.5.2
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.5.1/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2024.5.2/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/hahomematic_support/client_local.py` & `hahomematic-2024.5.2/hahomematic_support/client_local.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/pyproject.toml` & `hahomematic-2024.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=69.2.0", "wheel~=0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2024.5.1"
+version     = "2024.5.2"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

### Comparing `hahomematic-2024.5.1/tests/test_action.py` & `hahomematic-2024.5.2/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_binary_sensor.py` & `hahomematic-2024.5.2/tests/test_binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_button.py` & `hahomematic-2024.5.2/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_central.py` & `hahomematic-2024.5.2/tests/test_central.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_central_pydevccu.py` & `hahomematic-2024.5.2/tests/test_central_pydevccu.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,18 +110,18 @@
 
     with open(
         file=os.path.join(central_unit_full.config.storage_folder, "all_devices.json"),
         mode="wb",
     ) as fptr:
         fptr.write(orjson.dumps(addresses, option=orjson.OPT_INDENT_2 | orjson.OPT_NON_STR_KEYS))
 
-    assert usage_types[EntityUsage.NO_CREATE] == 3122
+    assert usage_types[EntityUsage.NO_CREATE] == 3110
     assert usage_types[EntityUsage.CE_PRIMARY] == 194
     assert usage_types[EntityUsage.ENTITY] == 3799
-    assert usage_types[EntityUsage.CE_VISIBLE] == 102
+    assert usage_types[EntityUsage.CE_VISIBLE] == 114
     assert usage_types[EntityUsage.CE_SECONDARY] == 146
 
     assert len(ce_channels) == 118
     assert len(entity_types) == 6
     assert len(parameters) == 215
 
     assert len(central_unit_full._devices) == 383
```

### Comparing `hahomematic-2024.5.1/tests/test_climate.py` & `hahomematic-2024.5.2/tests/test_climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_cover.py` & `hahomematic-2024.5.2/tests/test_cover.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Tests for cover entities of hahomematic."""
 
 from __future__ import annotations
 
+import asyncio
 from typing import cast
-from unittest.mock import Mock, call
+from unittest.mock import DEFAULT, Mock, call
 
 import pytest
 
 from hahomematic.central import CentralUnit
 from hahomematic.client import Client
 from hahomematic.config import WAIT_FOR_CALLBACK
 from hahomematic.const import EntityUsage
@@ -408,15 +409,15 @@
     )
 
     await cover.open_tilt()
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_TILT_LEVEL)
     call_count = len(mock_client.method_calls)
     await cover.open_tilt()
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_TILT_LEVEL)
-    assert call_count == len(mock_client.method_calls) - 2
+    assert call_count == len(mock_client.method_calls) - 5
 
     await cover.close_tilt()
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _CLOSED_LEVEL)
     call_count = len(mock_client.method_calls)
     await cover.close_tilt()
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _CLOSED_LEVEL)
     assert call_count == len(mock_client.method_calls) - 1
@@ -428,14 +429,69 @@
 
 
 @pytest.mark.asyncio()
 @pytest.mark.parametrize(
     (
         "address_device_translation",
         "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_ceblind_separate_level_and_tilt_change(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
+    """Test if CeBlind sends correct commands even when rapidly changing level and tilt via separate service calls."""
+    central, mock_client, _ = central_client_factory
+    cover: CeBlind = cast(CeBlind, helper.get_prepared_custom_entity(central, "VCU0000145", 1))
+
+    # In order for this test to make sense, communication with CCU must take some amount of time.
+    # This is not the case with the default local client used during testing, so we add a slight delay.
+    async def delay_communication(*args, **kwargs):
+        await asyncio.sleep(0.1)
+        return DEFAULT
+
+    mock_client.set_value.side_effect = delay_communication
+
+    # We test for the absence of race conditions.
+    # We repeat the test a few times so that it becomes unlikely for the race condition to remain undetected.
+    for _ in range(10):
+        await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL", 0)
+        await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", 0)
+        assert cover.current_position == 0
+        assert cover.current_tilt_position == 0
+
+        await asyncio.gather(
+            cover.set_position(position=81),
+            cover.set_position(tilt_position=19),
+        )
+
+        assert mock_client.method_calls[-1] == call.set_value(
+            channel_address="VCU0000145:1",
+            paramset_key="VALUES",
+            parameter="LEVEL_COMBINED",
+            value="0xa2,0x26",
+            wait_for_callback=WAIT_FOR_CALLBACK,
+        )
+        await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL", 0.81)
+        await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", 0.19)
+        assert cover.current_position == 81
+        assert cover.current_tilt_position == 19
+
+
+@pytest.mark.asyncio()
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
         "add_sysvars",
         "add_programs",
         "ignore_devices_on_create",
         "un_ignore_list",
     ),
     [
         (TEST_DEVICES, True, False, False, None, None),
```

### Comparing `hahomematic-2024.5.1/tests/test_decorator.py` & `hahomematic-2024.5.2/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_device.py` & `hahomematic-2024.5.2/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_entity.py` & `hahomematic-2024.5.2/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_event.py` & `hahomematic-2024.5.2/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_json_rpc.py` & `hahomematic-2024.5.2/tests/test_json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_light.py` & `hahomematic-2024.5.2/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_lock.py` & `hahomematic-2024.5.2/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_number.py` & `hahomematic-2024.5.2/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_select.py` & `hahomematic-2024.5.2/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_sensor.py` & `hahomematic-2024.5.2/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_siren.py` & `hahomematic-2024.5.2/tests/test_siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_support.py` & `hahomematic-2024.5.2/tests/test_support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_switch.py` & `hahomematic-2024.5.2/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.1/tests/test_text.py` & `hahomematic-2024.5.2/tests/test_text.py`

 * *Files identical despite different names*


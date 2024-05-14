# Comparing `tmp/ovos-PHAL-plugin-homeassistant-0.0.4a7.tar.gz` & `tmp/ovos-PHAL-plugin-homeassistant-0.0.4a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-homeassistant-0.0.4a7.tar", last modified: Mon May  6 22:30:00 2024, max compression
+gzip compressed data, was "ovos-PHAL-plugin-homeassistant-0.0.4a8.tar", last modified: Tue May 14 02:40:05 2024, max compression
```

## Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7.tar` & `ovos-PHAL-plugin-homeassistant-0.0.4a8.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:30:00.525603 ovos-PHAL-plugin-homeassistant-0.0.4a7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-06 22:30:00.525603 ovos-PHAL-plugin-homeassistant-0.0.4a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:30:00.517603 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/
--rw-r--r--   0 runner    (1001) docker     (127)    39137 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:30:00.517603 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/logic/
--rw-r--r--   0 runner    (1001) docker     (127)    15462 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/logic/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    28135 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/logic/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/logic/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/logic/socketclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/logic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:30:00.517603 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:30:00.517603 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/
--rw-r--r--   0 runner    (1001) docker     (127)    33382 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/Dashboard.qml
--rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/InstanceSetup.qml
--rw-r--r--   0 runner    (1001) docker     (127)    28881 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/InstanceGridButton.qml
--rw-r--r--   0 runner    (1001) docker     (127)    10880 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/InstanceSetup.qml
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/InstanceSetupFooterButtons.qml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:30:00.517603 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/code/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/code/helper.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:30:00.521603 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/AutomationCard.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/BinarySensorCard.qml
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/CameraCard.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/CircleSensorItemPercentType.qml
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/LightCard.qml
--rw-r--r--   0 runner    (1001) docker     (127)    20346 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/MediaPlayerCard.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/PowerSensorItemType.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/SceneCard.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/SensorCard.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/SwitchCard.qml
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/VacuumCard.qml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:30:00.521603 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/delegates/
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/delegates/DashboardDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/delegates/DeviceDashboardDelegate.qml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:30:00.521603 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/ColorPickerControl.qml
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightBrightness.qml
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightColor.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightDeviceStateButton.qml
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaControl.qml
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaDelegate.qml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:30:00.525603 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-off.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-on.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_light.svg
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:automation.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:binary_sensor.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:camera.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:climate.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:grouped.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:media_player.svg
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:scene.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:sensor.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:switch.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:ungrouped.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:vacuum.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/power.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/qr-mobile.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/token-device.svg
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:30:00.517603 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-06 22:30:00.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-06 22:30:00.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 22:30:00.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-06 22:30:00.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-06 22:30:00.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-06 22:30:00.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 22:30:00.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:30:00.513603 ovos-PHAL-plugin-homeassistant-0.0.4a7/res/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:30:00.525603 ovos-PHAL-plugin-homeassistant-0.0.4a7/res/desktop/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/res/desktop/ovos-phal-homeassistant.desktop
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:30:00.525603 ovos-PHAL-plugin-homeassistant-0.0.4a7/res/icon/
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/res/icon/ovos-phal-homeassistant.svg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 22:30:00.525603 ovos-PHAL-plugin-homeassistant-0.0.4a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-06 22:29:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:40:05.583449 ovos-PHAL-plugin-homeassistant-0.0.4a8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-05-14 02:40:05.583449 ovos-PHAL-plugin-homeassistant-0.0.4a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:40:05.575449 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/
+-rw-r--r--   0 runner    (1001) docker     (127)    39670 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:40:05.575449 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/logic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15462 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/logic/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28319 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/logic/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/logic/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/logic/socketclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/logic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:40:05.579449 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:40:05.579449 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/
+-rw-r--r--   0 runner    (1001) docker     (127)    33382 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/Dashboard.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/InstanceSetup.qml
+-rw-r--r--   0 runner    (1001) docker     (127)    28881 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/InstanceGridButton.qml
+-rw-r--r--   0 runner    (1001) docker     (127)    10880 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/InstanceSetup.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/InstanceSetupFooterButtons.qml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:40:05.579449 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/code/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/code/helper.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:40:05.579449 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/AutomationCard.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/BinarySensorCard.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/CameraCard.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/CircleSensorItemPercentType.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/LightCard.qml
+-rw-r--r--   0 runner    (1001) docker     (127)    20346 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/MediaPlayerCard.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/PowerSensorItemType.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/SceneCard.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/SensorCard.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/SwitchCard.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/VacuumCard.qml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:40:05.579449 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/delegates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/delegates/DashboardDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/delegates/DeviceDashboardDelegate.qml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:40:05.579449 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/ColorPickerControl.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightBrightness.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightColor.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightDeviceStateButton.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaControl.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaDelegate.qml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:40:05.583449 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-off.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-on.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:automation.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:binary_sensor.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:camera.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:climate.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:grouped.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:media_player.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:scene.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:sensor.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:switch.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:ungrouped.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:vacuum.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/power.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/qr-mobile.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/token-device.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:40:05.575449 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-05-14 02:40:05.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-14 02:40:05.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 02:40:05.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-14 02:40:05.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-14 02:40:05.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 02:40:05.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 02:40:05.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:40:05.575449 ovos-PHAL-plugin-homeassistant-0.0.4a8/res/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:40:05.583449 ovos-PHAL-plugin-homeassistant-0.0.4a8/res/desktop/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/res/desktop/ovos-phal-homeassistant.desktop
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:40:05.583449 ovos-PHAL-plugin-homeassistant-0.0.4a8/res/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/res/icon/ovos-phal-homeassistant.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 02:40:05.583449 ovos-PHAL-plugin-homeassistant-0.0.4a8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-14 02:39:57.000000 ovos-PHAL-plugin-homeassistant-0.0.4a8/setup.py
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/LICENSE` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/PKG-INFO` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-homeassistant
-Version: 0.0.4a7
+Version: 0.0.4a8
 Summary: Homeassistant PHAL plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -78,24 +78,26 @@
    ```
 
 The config also takes some optional properties:
 
 `brightness_increment` - the amount to increment/decrement the brightness of a light when the brightness up/down commands are sent. The default value is 10 and represents a percentage, e.g. 10%.
 `search_confidence_threshold` - the confidence threshold for the search skill to use when searching for devices. The default value is 0.5, or 50%. Must be a value between 0 and 1.
 `assist_only` - whether to pull down only entities exposed to Assist. Default True.
+`toggle_automations` - whether to allow the plugin to turn automations on and off. Default False.
 
 Sample config:
 
 ```json
         "PHAL": {
             "ovos-PHAL-plugin-homeassistant": {
                 "host": "https://someurl.toinstance",
                 "api_key": "api key from the instance",
                 "brightness_increment": 5,
-                "search_confidence_threshold": 0.6
+                "search_confidence_threshold": 0.6,
+                "toggle_automations": false,
             }
         }
 ```
 
 ### Usage
 
 The plugin provides a GUI interface for Home Assistant Instances. It also provides an API for other plugins or skills to user.
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/README.md` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,24 +57,26 @@
    ```
 
 The config also takes some optional properties:
 
 `brightness_increment` - the amount to increment/decrement the brightness of a light when the brightness up/down commands are sent. The default value is 10 and represents a percentage, e.g. 10%.
 `search_confidence_threshold` - the confidence threshold for the search skill to use when searching for devices. The default value is 0.5, or 50%. Must be a value between 0 and 1.
 `assist_only` - whether to pull down only entities exposed to Assist. Default True.
+`toggle_automations` - whether to allow the plugin to turn automations on and off. Default False.
 
 Sample config:
 
 ```json
         "PHAL": {
             "ovos-PHAL-plugin-homeassistant": {
                 "host": "https://someurl.toinstance",
                 "api_key": "api key from the instance",
                 "brightness_increment": 5,
-                "search_confidence_threshold": 0.6
+                "search_confidence_threshold": 0.6,
+                "toggle_automations": false,
             }
         }
 ```
 
 ### Usage
 
 The plugin provides a GUI interface for Home Assistant Instances. It also provides an API for other plugins or skills to user.
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/__init__.py` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,23 @@
         """ Get the search confidence threshold from the config
 
             Returns:
                 int: The search confidence threshold value, default 0.5
         """
         return self.config.get("search_confidence_threshold", 0.5)
 
+    @property
+    def toggle_automations(self) -> bool:
+        """ Get the toggle automations from the config
+
+            Returns:
+                bool: The toggle automations value, default False
+        """
+        return self.config.get("toggle_automations", False)
+
 # SETUP INSTANCE SUPPORT
     def validate_instance_connection(self, host, api_key, assist_only):
         """ Validate the connection to the Home Assistant instance
 
             Args:
                 host (str): The Home Assistant instance URL
                 api_key (str): The Home Assistant API key
@@ -247,17 +256,20 @@
                     device_icon = f"mdi:{device_type}"
                     device_state = device.get("state", None)
                     device_area = device.get("area_id", None)
 
                     device_attributes = device.get("attributes", {})
                     if device_type in self.device_types:
                         LOG.debug(f"Device added: {device_name} - {device_type} - {device_area}")
-                        self.registered_devices.append(self.device_types[device_type](
-                            self.connector, device_id, device_icon, device_name,
-                            device_state, device_attributes, device_area, self.device_updated))
+                        dev_args = [self.connector, device_id, device_icon, device_name,
+                            device_state, device_attributes, device_area, self.device_updated]
+                        if device_type == "automation":
+                            # Since automations.turn_off is usually disabled, we need to be explicit about the config
+                            dev_args.append(self.toggle_automations)
+                        self.registered_devices.append(self.device_types[device_type](*dev_args))
                         self.registered_device_names.append(device_name)
                     else:
                         LOG.warning(f"Device type {device_type} not supported; please file an issue on GitHub")
                 else:
                     LOG.warning(
                         f"Device type {device_type} is a group, not supported currently")
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/logic/connector.py` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/logic/connector.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/logic/device.py` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/logic/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -841,15 +841,20 @@
         device_id,
         device_icon,
         device_name,
         device_state,
         device_attributes,
         device_area=None,
         update_signal=None,
+        toggle_automations=False,
     ):
         super().__init__(
             connector, device_id, device_icon, device_name, device_state, device_attributes, device_area, update_signal
         )
+        self.toggle_automations = toggle_automations
 
     def turn_off(self):
-        LOG.warning("Request to turn off an automation. This is not supported, as it will disable it instead.")
-        return
+        if self.toggle_automations is True:
+            super().turn_off()
+        else:
+            LOG.warning("Request to turn off an automation. This is not supported, as it will disable it instead.")
+            return
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/logic/integration.py` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/logic/integration.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/logic/socketclient.py` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/logic/socketclient.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/logic/utils.py` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/logic/utils.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/Dashboard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/Dashboard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/InstanceSetup.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/InstanceSetup.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/InstanceGridButton.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/InstanceGridButton.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/InstanceSetup.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/InstanceSetup.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/InstanceSetupFooterButtons.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/InstanceSetupFooterButtons.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/code/helper.js` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/code/helper.js`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/AutomationCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/AutomationCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/BinarySensorCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/BinarySensorCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/CameraCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/CameraCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/CircleSensorItemPercentType.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/CircleSensorItemPercentType.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/LightCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/LightCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/MediaPlayerCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/MediaPlayerCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/PowerSensorItemType.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/PowerSensorItemType.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/SceneCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/SceneCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/SensorCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/SensorCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/SwitchCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/SwitchCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/dashcards/VacuumCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/dashcards/VacuumCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/delegates/DashboardDelegate.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/delegates/DashboardDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/delegates/DeviceDashboardDelegate.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/delegates/DeviceDashboardDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/ColorPickerControl.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/ColorPickerControl.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightBrightness.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightBrightness.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightColor.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightColor.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightDeviceStateButton.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightDeviceStateButton.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaControl.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaControl.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaDelegate.qml` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-off.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-off.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-on.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-on.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_dark.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_dark.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_light.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_light.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:automation.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:automation.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:binary_sensor.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:binary_sensor.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:camera.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:camera.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:climate.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:climate.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:grouped.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:grouped.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:light.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:light.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:media_player.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:media_player.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:sensor.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:sensor.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:switch.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:switch.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:ungrouped.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:ungrouped.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:vacuum.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:vacuum.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/power.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/power.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/qr-mobile.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/qr-mobile.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant/ui/icons/token-device.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant/ui/icons/token-device.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-homeassistant
-Version: 0.0.4a7
+Version: 0.0.4a8
 Summary: Homeassistant PHAL plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -78,24 +78,26 @@
    ```
 
 The config also takes some optional properties:
 
 `brightness_increment` - the amount to increment/decrement the brightness of a light when the brightness up/down commands are sent. The default value is 10 and represents a percentage, e.g. 10%.
 `search_confidence_threshold` - the confidence threshold for the search skill to use when searching for devices. The default value is 0.5, or 50%. Must be a value between 0 and 1.
 `assist_only` - whether to pull down only entities exposed to Assist. Default True.
+`toggle_automations` - whether to allow the plugin to turn automations on and off. Default False.
 
 Sample config:
 
 ```json
         "PHAL": {
             "ovos-PHAL-plugin-homeassistant": {
                 "host": "https://someurl.toinstance",
                 "api_key": "api key from the instance",
                 "brightness_increment": 5,
-                "search_confidence_threshold": 0.6
+                "search_confidence_threshold": 0.6,
+                "toggle_automations": false,
             }
         }
 ```
 
 ### Usage
 
 The plugin provides a GUI interface for Home Assistant Instances. It also provides an API for other plugins or skills to user.
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO
 ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt
 ovos_PHAL_plugin_homeassistant.egg-info/dependency_links.txt
 ovos_PHAL_plugin_homeassistant.egg-info/entry_points.txt
 ovos_PHAL_plugin_homeassistant.egg-info/requires.txt
 ovos_PHAL_plugin_homeassistant.egg-info/top_level.txt
 ovos_PHAL_plugin_homeassistant.egg-info/zip-safe
+ovos_PHAL_plugin_homeassistant/logic/__init__.py
 ovos_PHAL_plugin_homeassistant/logic/connector.py
 ovos_PHAL_plugin_homeassistant/logic/device.py
 ovos_PHAL_plugin_homeassistant/logic/integration.py
 ovos_PHAL_plugin_homeassistant/logic/socketclient.py
 ovos_PHAL_plugin_homeassistant/logic/utils.py
 ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml
 ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/res/icon/ovos-phal-homeassistant.svg` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/res/icon/ovos-phal-homeassistant.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.4a7/setup.py` & `ovos-PHAL-plugin-homeassistant-0.0.4a8/setup.py`

 * *Files identical despite different names*


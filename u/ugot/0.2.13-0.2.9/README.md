# Comparing `tmp/ugot-0.2.13.tar.gz` & `tmp/ugot-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ugot-0.2.13.tar", last modified: Sat May 11 07:20:03 2024, max compression
+gzip compressed data, was "ugot-0.2.9.tar", last modified: Thu Nov 30 06:37:11 2023, max compression
```

## Comparing `ugot-0.2.13.tar` & `ugot-0.2.9.tar`

### file list

```diff
@@ -1,68 +1,57 @@
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2024-05-11 07:20:03.374931 ugot-0.2.13/
--rw-r--r--   0 jesse      (501) staff       (20)     1103 2023-05-15 09:14:27.000000 ugot-0.2.13/LICENSE
--rw-r--r--   0 jesse      (501) staff       (20)      848 2024-05-11 07:20:03.374423 ugot-0.2.13/PKG-INFO
--rwxrwxrwx   0 jesse      (501) staff       (20)      246 2023-05-11 07:07:58.000000 ugot-0.2.13/README.md
--rwxr-xr-x   0 jesse      (501) staff       (20)      656 2024-05-11 07:17:58.000000 ugot-0.2.13/pyproject.toml
--rw-r--r--   0 jesse      (501) staff       (20)       38 2024-05-11 07:20:03.375061 ugot-0.2.13/setup.cfg
--rwxr-xr-x   0 jesse      (501) staff       (20)      663 2024-05-11 07:16:44.000000 ugot-0.2.13/setup.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2024-05-11 07:20:03.228873 ugot-0.2.13/ugot/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-11-07 07:33:08.000000 ugot-0.2.13/ugot/__init__.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2024-05-11 07:20:03.343605 ugot-0.2.13/ugot/grpc_pb/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.2.13/ugot/grpc_pb/__init__.py
--rw-r--r--   0 jesse      (501) staff       (20)     6489 2023-11-22 06:57:45.000000 ugot-0.2.13/ugot/grpc_pb/audio_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    25505 2023-11-22 06:57:45.000000 ugot-0.2.13/ugot/grpc_pb/audio_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     6234 2023-05-15 03:20:28.000000 ugot-0.2.13/ugot/grpc_pb/bluetooth_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    18284 2023-05-15 03:20:28.000000 ugot-0.2.13/ugot/grpc_pb/bluetooth_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)    12189 2023-12-07 10:03:28.000000 ugot-0.2.13/ugot/grpc_pb/device_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    38319 2023-12-07 10:03:28.000000 ugot-0.2.13/ugot/grpc_pb/device_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     6598 2024-02-21 02:21:18.000000 ugot-0.2.13/ugot/grpc_pb/gpio_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    20050 2024-02-21 02:21:18.000000 ugot-0.2.13/ugot/grpc_pb/gpio_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     9850 2023-08-17 07:12:13.000000 ugot-0.2.13/ugot/grpc_pb/model_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    26458 2023-08-17 07:12:13.000000 ugot-0.2.13/ugot/grpc_pb/model_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     6803 2023-05-15 03:20:28.000000 ugot-0.2.13/ugot/grpc_pb/network_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    24828 2023-05-15 03:20:28.000000 ugot-0.2.13/ugot/grpc_pb/network_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     2135 2023-05-15 03:20:28.000000 ugot-0.2.13/ugot/grpc_pb/power_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)     5561 2023-05-15 03:20:28.000000 ugot-0.2.13/ugot/grpc_pb/power_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     5080 2023-05-15 03:20:28.000000 ugot-0.2.13/ugot/grpc_pb/sensor_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    13911 2023-05-15 03:20:28.000000 ugot-0.2.13/ugot/grpc_pb/sensor_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)    10879 2023-07-10 07:03:25.000000 ugot-0.2.13/ugot/grpc_pb/servo_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    24766 2023-06-26 08:19:12.000000 ugot-0.2.13/ugot/grpc_pb/servo_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)    10320 2023-11-29 09:34:07.000000 ugot-0.2.13/ugot/grpc_pb/vision_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    36875 2023-11-29 09:34:07.000000 ugot-0.2.13/ugot/grpc_pb/vision_pb2_grpc.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2024-05-11 07:20:03.344006 ugot-0.2.13/ugot/protos/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.2.13/ugot/protos/__init__.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2024-05-11 07:20:03.370700 ugot-0.2.13/ugot/src/
--rw-r--r--   0 jesse      (501) staff       (20)     3928 2024-01-09 05:58:05.000000 ugot-0.2.13/ugot/src/PID.py
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-10-31 07:26:49.000000 ugot-0.2.13/ugot/src/__init__.py
--rw-r--r--   0 jesse      (501) staff       (20)     3125 2024-01-10 06:25:18.000000 ugot-0.2.13/ugot/src/audio_client.py
--rw-r--r--   0 jesse      (501) staff       (20)      517 2023-05-11 07:27:02.000000 ugot-0.2.13/ugot/src/base_client.py
--rw-r--r--   0 jesse      (501) staff       (20)      710 2023-11-07 07:44:54.000000 ugot-0.2.13/ugot/src/bluetooth_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     1304 2024-01-10 10:26:40.000000 ugot-0.2.13/ugot/src/configure_string_single.py
--rw-r--r--   0 jesse      (501) staff       (20)     4939 2024-01-10 06:47:04.000000 ugot-0.2.13/ugot/src/device_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     5594 2024-05-11 03:12:00.000000 ugot-0.2.13/ugot/src/enum.py
--rw-r--r--   0 jesse      (501) staff       (20)     3693 2024-02-21 02:21:18.000000 ugot-0.2.13/ugot/src/gpio_client.py
--rw-r--r--   0 jesse      (501) staff       (20)      597 2023-08-28 07:51:24.000000 ugot-0.2.13/ugot/src/http_client.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2024-05-11 07:20:03.226684 ugot-0.2.13/ugot/src/locale/
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2024-05-11 07:20:03.226505 ugot-0.2.13/ugot/src/locale/en/
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2024-05-11 07:20:03.371840 ugot-0.2.13/ugot/src/locale/en/LC_MESSAGES/
--rw-r--r--   0 jesse      (501) staff       (20)     2097 2024-05-11 03:27:22.000000 ugot-0.2.13/ugot/src/locale/en/LC_MESSAGES/ugot.mo
--rw-r--r--   0 jesse      (501) staff       (20)     1945 2024-05-11 03:24:57.000000 ugot-0.2.13/ugot/src/locale/en/LC_MESSAGES/ugot.po
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2024-05-11 07:20:03.226840 ugot-0.2.13/ugot/src/locale/zh_CN/
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2024-05-11 07:20:03.373143 ugot-0.2.13/ugot/src/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 jesse      (501) staff       (20)     2064 2024-05-11 03:27:22.000000 ugot-0.2.13/ugot/src/locale/zh_CN/LC_MESSAGES/ugot.mo
--rw-r--r--   0 jesse      (501) staff       (20)     1912 2024-05-11 03:27:20.000000 ugot-0.2.13/ugot/src/locale/zh_CN/LC_MESSAGES/ugot.po
--rw-r--r--   0 jesse      (501) staff       (20)    10719 2024-01-24 06:19:14.000000 ugot-0.2.13/ugot/src/model_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     5939 2024-02-20 09:24:06.000000 ugot-0.2.13/ugot/src/network_client.py
--rw-r--r--   0 jesse      (501) staff       (20)      679 2023-11-07 07:44:54.000000 ugot-0.2.13/ugot/src/power_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     2294 2023-06-06 02:56:27.000000 ugot-0.2.13/ugot/src/scan_device.py
--rw-r--r--   0 jesse      (501) staff       (20)     1196 2023-11-07 07:44:54.000000 ugot-0.2.13/ugot/src/sensor_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     6738 2024-01-10 06:25:43.000000 ugot-0.2.13/ugot/src/servo_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     4110 2023-05-11 07:27:02.000000 ugot-0.2.13/ugot/src/util.py
--rw-r--r--   0 jesse      (501) staff       (20)    17306 2024-05-11 06:36:03.000000 ugot-0.2.13/ugot/src/vision_client.py
--rw-r--r--   0 jesse      (501) staff       (20)   141812 2024-05-11 03:26:01.000000 ugot-0.2.13/ugot/ugot.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2024-05-11 07:20:03.373877 ugot-0.2.13/ugot.egg-info/
--rw-r--r--   0 jesse      (501) staff       (20)      848 2024-05-11 07:20:03.000000 ugot-0.2.13/ugot.egg-info/PKG-INFO
--rw-r--r--   0 jesse      (501) staff       (20)     1444 2024-05-11 07:20:03.000000 ugot-0.2.13/ugot.egg-info/SOURCES.txt
--rw-r--r--   0 jesse      (501) staff       (20)        1 2024-05-11 07:20:03.000000 ugot-0.2.13/ugot.egg-info/dependency_links.txt
--rw-r--r--   0 jesse      (501) staff       (20)      100 2024-05-11 07:20:03.000000 ugot-0.2.13/ugot.egg-info/requires.txt
--rw-r--r--   0 jesse      (501) staff       (20)        5 2024-05-11 07:20:03.000000 ugot-0.2.13/ugot.egg-info/top_level.txt
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-11-30 06:37:11.461984 ugot-0.2.9/
+-rw-r--r--   0 jesse      (501) staff       (20)     1103 2023-05-15 09:14:27.000000 ugot-0.2.9/LICENSE
+-rw-r--r--   0 jesse      (501) staff       (20)      612 2023-11-30 06:37:11.461513 ugot-0.2.9/PKG-INFO
+-rwxrwxrwx   0 jesse      (501) staff       (20)      246 2023-05-11 07:07:58.000000 ugot-0.2.9/README.md
+-rwxr-xr-x   0 jesse      (501) staff       (20)      607 2023-11-28 09:51:18.000000 ugot-0.2.9/pyproject.toml
+-rw-r--r--   0 jesse      (501) staff       (20)       38 2023-11-30 06:37:11.462086 ugot-0.2.9/setup.cfg
+-rwxr-xr-x   0 jesse      (501) staff       (20)      595 2023-11-07 07:44:54.000000 ugot-0.2.9/setup.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-11-30 06:37:11.186411 ugot-0.2.9/ugot/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-11-07 07:33:08.000000 ugot-0.2.9/ugot/__init__.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-11-30 06:37:11.294674 ugot-0.2.9/ugot/grpc_pb/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.2.9/ugot/grpc_pb/__init__.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6489 2023-11-22 06:57:45.000000 ugot-0.2.9/ugot/grpc_pb/audio_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    25505 2023-11-22 06:57:45.000000 ugot-0.2.9/ugot/grpc_pb/audio_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6234 2023-05-15 03:20:28.000000 ugot-0.2.9/ugot/grpc_pb/bluetooth_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    18284 2023-05-15 03:20:28.000000 ugot-0.2.9/ugot/grpc_pb/bluetooth_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)    12189 2023-11-21 06:30:19.000000 ugot-0.2.9/ugot/grpc_pb/device_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    38319 2023-11-21 06:30:19.000000 ugot-0.2.9/ugot/grpc_pb/device_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6103 2023-05-15 03:20:28.000000 ugot-0.2.9/ugot/grpc_pb/gpio_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    18277 2023-05-15 03:20:28.000000 ugot-0.2.9/ugot/grpc_pb/gpio_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     9850 2023-08-17 07:12:13.000000 ugot-0.2.9/ugot/grpc_pb/model_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    26458 2023-08-17 07:12:13.000000 ugot-0.2.9/ugot/grpc_pb/model_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6803 2023-05-15 03:20:28.000000 ugot-0.2.9/ugot/grpc_pb/network_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    24828 2023-05-15 03:20:28.000000 ugot-0.2.9/ugot/grpc_pb/network_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2135 2023-05-15 03:20:28.000000 ugot-0.2.9/ugot/grpc_pb/power_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5561 2023-05-15 03:20:28.000000 ugot-0.2.9/ugot/grpc_pb/power_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5080 2023-05-15 03:20:28.000000 ugot-0.2.9/ugot/grpc_pb/sensor_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    13911 2023-05-15 03:20:28.000000 ugot-0.2.9/ugot/grpc_pb/sensor_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)    10879 2023-07-10 07:03:25.000000 ugot-0.2.9/ugot/grpc_pb/servo_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    24766 2023-06-26 08:19:12.000000 ugot-0.2.9/ugot/grpc_pb/servo_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)    10320 2023-11-29 09:34:07.000000 ugot-0.2.9/ugot/grpc_pb/vision_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    36875 2023-11-29 09:34:07.000000 ugot-0.2.9/ugot/grpc_pb/vision_pb2_grpc.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-11-30 06:37:11.314189 ugot-0.2.9/ugot/protos/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.2.9/ugot/protos/__init__.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-11-30 06:37:11.447442 ugot-0.2.9/ugot/src/
+-rw-r--r--   0 jesse      (501) staff       (20)     3917 2023-11-24 06:03:37.000000 ugot-0.2.9/ugot/src/PID.py
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-10-31 07:26:49.000000 ugot-0.2.9/ugot/src/__init__.py
+-rw-r--r--   0 jesse      (501) staff       (20)     3098 2023-11-21 07:23:56.000000 ugot-0.2.9/ugot/src/audio_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)      517 2023-05-11 07:27:02.000000 ugot-0.2.9/ugot/src/base_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)      710 2023-11-07 07:44:54.000000 ugot-0.2.9/ugot/src/bluetooth_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     4751 2023-11-22 06:53:49.000000 ugot-0.2.9/ugot/src/device_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5492 2023-11-21 06:35:49.000000 ugot-0.2.9/ugot/src/enum.py
+-rw-r--r--   0 jesse      (501) staff       (20)     3176 2023-11-07 07:44:54.000000 ugot-0.2.9/ugot/src/gpio_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)      597 2023-08-28 07:51:24.000000 ugot-0.2.9/ugot/src/http_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)    10692 2023-11-21 06:28:41.000000 ugot-0.2.9/ugot/src/model_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5657 2023-11-07 07:44:54.000000 ugot-0.2.9/ugot/src/network_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)      679 2023-11-07 07:44:54.000000 ugot-0.2.9/ugot/src/power_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2294 2023-06-06 02:56:27.000000 ugot-0.2.9/ugot/src/scan_device.py
+-rw-r--r--   0 jesse      (501) staff       (20)     1196 2023-11-07 07:44:54.000000 ugot-0.2.9/ugot/src/sensor_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6711 2023-11-07 07:44:54.000000 ugot-0.2.9/ugot/src/servo_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     4110 2023-05-11 07:27:02.000000 ugot-0.2.9/ugot/src/util.py
+-rw-r--r--   0 jesse      (501) staff       (20)    14806 2023-11-29 10:26:41.000000 ugot-0.2.9/ugot/src/vision_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)   134504 2023-11-30 05:51:56.000000 ugot-0.2.9/ugot/ugot.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-11-30 06:37:11.460998 ugot-0.2.9/ugot.egg-info/
+-rw-r--r--   0 jesse      (501) staff       (20)      612 2023-11-30 06:37:11.000000 ugot-0.2.9/ugot.egg-info/PKG-INFO
+-rw-r--r--   0 jesse      (501) staff       (20)     1219 2023-11-30 06:37:11.000000 ugot-0.2.9/ugot.egg-info/SOURCES.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        1 2023-11-30 06:37:11.000000 ugot-0.2.9/ugot.egg-info/dependency_links.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        5 2023-11-30 06:37:11.000000 ugot-0.2.9/ugot.egg-info/top_level.txt
```

### Comparing `ugot-0.2.13/LICENSE` & `ugot-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/pyproject.toml` & `ugot-0.2.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 [build-system]
-requires = ["setuptools>=61.0", "wheel"]
+requires = [
+        "setuptools>=61.0", 
+        "concurrent-log-handler",
+        "grpcio",
+        "protobuf",
+        "grpcio-tools",
+        "wheel",
+        "zeroconf", 
+        "pillow",
+        "requests"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ugot"
-version = "0.2.13"
+version = "0.2.9"
 authors = [
   { name="Jesse", email="jesse.huang@ubtrobot.com" },
 ]
-dependencies = [
-        'setuptools>=61.0',
-        'concurrent-log-handler',
-        'grpcio',
-        'protobuf',
-        'grpcio-tools',
-        'wheel',
-        'zeroconf',
-        'pillow',
-        'requests'
-    ]
 description = "ugot-Python SDK"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `ugot-0.2.13/setup.py` & `ugot-0.2.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name = "ugot",
-    version = "0.2.13",
+    version = "0.2.8",
     description = "ugot-Python SDK",
     long_description = "",
 
     packages = find_packages(include=["ugot","ugot.*"]),
-    package_data={
-        'ugot': ['**/*.mo', '**/*.po',],
-    },
     # package_data = {"ugot": ["*"],
     #                 },
     # packages=find_packages(),
     # include_package_data = True,
     platforms = "any",
     install_requires = [
         'concurrent-log-handler',
```

### Comparing `ugot-0.2.13/ugot/grpc_pb/audio_pb2.py` & `ugot-0.2.9/ugot/grpc_pb/audio_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/grpc_pb/audio_pb2_grpc.py` & `ugot-0.2.9/ugot/grpc_pb/audio_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/grpc_pb/bluetooth_pb2.py` & `ugot-0.2.9/ugot/grpc_pb/bluetooth_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/grpc_pb/bluetooth_pb2_grpc.py` & `ugot-0.2.9/ugot/grpc_pb/bluetooth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/grpc_pb/device_pb2.py` & `ugot-0.2.9/ugot/grpc_pb/device_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/grpc_pb/device_pb2_grpc.py` & `ugot-0.2.9/ugot/grpc_pb/device_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/grpc_pb/gpio_pb2.py` & `ugot-0.2.9/ugot/grpc_pb/gpio_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\ngpio.proto\x12\x0bGpioPackage\"2\n\x14SetGpioExportRequest\x12\x0b\n\x03pin\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08\"2\n\x15SetGpioExportResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\"\x1e\n\x0fReadGpioRequest\x12\x0b\n\x03pin\x18\x01 \x01(\t\"=\n\x10ReadGpioResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\x12\x0e\n\x06result\x18\x03 \x01(\t\"a\n\x1cSetGpioStartExportPwmRequest\x12\x0b\n\x03pin\x18\x01 \x01(\t\x12\x11\n\tfrequency\x18\x02 \x01(\x04\x12\x12\n\nduty_cycle\x18\x03 \x01(\x04\x12\r\n\x05range\x18\x04 \x01(\x04\"n\n)SetGpioStartExportPwmWithDutyCycleRequest\x12\x0b\n\x03pin\x18\x01 \x01(\t\x12\x11\n\tfrequency\x18\x02 \x01(\x01\x12\x12\n\nduty_cycle\x18\x03 \x01(\x01\x12\r\n\x05range\x18\x04 \x01(\x01\":\n\x1dSetGpioStartExportPwmResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\"*\n\x1bSetGpioStopExportPwmRequest\x12\x0b\n\x03pin\x18\x01 \x01(\t\"9\n\x1cSetGpioStopExportPwmResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\"3\n\x11SetSerbaudRequest\x12\x0c\n\x04port\x18\x01 \x01(\t\x12\x10\n\x08\x62\x61udrate\x18\x02 \x01(\x04\"/\n\x12SetSerbaudResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\"8\n\x19SerialExportStringRequest\x12\x0c\n\x04port\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"7\n\x1aSerialExportStringResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\"%\n\x15SerialReadByteRequest\x12\x0c\n\x04port\x18\x01 \x01(\t\"C\n\x16SerialReadByteResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\x12\x0e\n\x06result\x18\x03 \x01(\t\"\'\n\x17SerialReadStringRequest\x12\x0c\n\x04port\x18\x01 \x01(\t\"E\n\x18SerialReadStringResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\x12\x0e\n\x06result\x18\x03 \x01(\t\"4\n\x15SerialReadUtilRequest\x12\x0c\n\x04port\x18\x01 \x01(\t\x12\r\n\x05\x63har_\x18\x02 \x01(\t\"C\n\x16SerialReadUtilResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\x12\x0e\n\x06result\x18\x03 \x01(\t\"\x1e\n\x1c\x43learAllGpioAndSerialRequest\":\n\x1d\x43learAllGpioAndSerialResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t2\xed\x08\n\x0fGpioServiceGrpc\x12X\n\rsetGpioExport\x12!.GpioPackage.SetGpioExportRequest\x1a\".GpioPackage.SetGpioExportResponse\"\x00\x12I\n\x08readGpio\x12\x1c.GpioPackage.ReadGpioRequest\x1a\x1d.GpioPackage.ReadGpioResponse\"\x00\x12p\n\x15setGpioStartExportPwm\x12).GpioPackage.SetGpioStartExportPwmRequest\x1a*.GpioPackage.SetGpioStartExportPwmResponse\"\x00\x12\x8a\x01\n\"setGpioStartExportPwmWithDutyCycle\x12\x36.GpioPackage.SetGpioStartExportPwmWithDutyCycleRequest\x1a*.GpioPackage.SetGpioStartExportPwmResponse\"\x00\x12m\n\x14setGpioStopExportPwm\x12(.GpioPackage.SetGpioStopExportPwmRequest\x1a).GpioPackage.SetGpioStopExportPwmResponse\"\x00\x12O\n\nsetSerbaud\x12\x1e.GpioPackage.SetSerbaudRequest\x1a\x1f.GpioPackage.SetSerbaudResponse\"\x00\x12g\n\x12serialExportString\x12&.GpioPackage.SerialExportStringRequest\x1a\'.GpioPackage.SerialExportStringResponse\"\x00\x12[\n\x0eserialReadByte\x12\".GpioPackage.SerialReadByteRequest\x1a#.GpioPackage.SerialReadByteResponse\"\x00\x12\x61\n\x10serialReadString\x12$.GpioPackage.SerialReadStringRequest\x1a%.GpioPackage.SerialReadStringResponse\"\x00\x12[\n\x0eserialReadUtil\x12\".GpioPackage.SerialReadUtilRequest\x1a#.GpioPackage.SerialReadUtilResponse\"\x00\x12p\n\x15\x63learAllGpioAndSerial\x12).GpioPackage.ClearAllGpioAndSerialRequest\x1a*.GpioPackage.ClearAllGpioAndSerialResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\ngpio.proto\x12\x0bGpioPackage\"2\n\x14SetGpioExportRequest\x12\x0b\n\x03pin\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08\"2\n\x15SetGpioExportResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\"\x1e\n\x0fReadGpioRequest\x12\x0b\n\x03pin\x18\x01 \x01(\t\"=\n\x10ReadGpioResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\x12\x0e\n\x06result\x18\x03 \x01(\t\"a\n\x1cSetGpioStartExportPwmRequest\x12\x0b\n\x03pin\x18\x01 \x01(\t\x12\x11\n\tfrequency\x18\x02 \x01(\x04\x12\x12\n\nduty_cycle\x18\x03 \x01(\x04\x12\r\n\x05range\x18\x04 \x01(\x04\":\n\x1dSetGpioStartExportPwmResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\"*\n\x1bSetGpioStopExportPwmRequest\x12\x0b\n\x03pin\x18\x01 \x01(\t\"9\n\x1cSetGpioStopExportPwmResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\"3\n\x11SetSerbaudRequest\x12\x0c\n\x04port\x18\x01 \x01(\t\x12\x10\n\x08\x62\x61udrate\x18\x02 \x01(\x04\"/\n\x12SetSerbaudResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\"8\n\x19SerialExportStringRequest\x12\x0c\n\x04port\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"7\n\x1aSerialExportStringResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\"%\n\x15SerialReadByteRequest\x12\x0c\n\x04port\x18\x01 \x01(\t\"C\n\x16SerialReadByteResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\x12\x0e\n\x06result\x18\x03 \x01(\t\"\'\n\x17SerialReadStringRequest\x12\x0c\n\x04port\x18\x01 \x01(\t\"E\n\x18SerialReadStringResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\x12\x0e\n\x06result\x18\x03 \x01(\t\"4\n\x15SerialReadUtilRequest\x12\x0c\n\x04port\x18\x01 \x01(\t\x12\r\n\x05\x63har_\x18\x02 \x01(\t\"C\n\x16SerialReadUtilResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t\x12\x0e\n\x06result\x18\x03 \x01(\t\"\x1e\n\x1c\x43learAllGpioAndSerialRequest\":\n\x1d\x43learAllGpioAndSerialResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0b\n\x03msg\x18\x02 \x01(\t2\xe0\x07\n\x0fGpioServiceGrpc\x12X\n\rsetGpioExport\x12!.GpioPackage.SetGpioExportRequest\x1a\".GpioPackage.SetGpioExportResponse\"\x00\x12I\n\x08readGpio\x12\x1c.GpioPackage.ReadGpioRequest\x1a\x1d.GpioPackage.ReadGpioResponse\"\x00\x12p\n\x15setGpioStartExportPwm\x12).GpioPackage.SetGpioStartExportPwmRequest\x1a*.GpioPackage.SetGpioStartExportPwmResponse\"\x00\x12m\n\x14setGpioStopExportPwm\x12(.GpioPackage.SetGpioStopExportPwmRequest\x1a).GpioPackage.SetGpioStopExportPwmResponse\"\x00\x12O\n\nsetSerbaud\x12\x1e.GpioPackage.SetSerbaudRequest\x1a\x1f.GpioPackage.SetSerbaudResponse\"\x00\x12g\n\x12serialExportString\x12&.GpioPackage.SerialExportStringRequest\x1a\'.GpioPackage.SerialExportStringResponse\"\x00\x12[\n\x0eserialReadByte\x12\".GpioPackage.SerialReadByteRequest\x1a#.GpioPackage.SerialReadByteResponse\"\x00\x12\x61\n\x10serialReadString\x12$.GpioPackage.SerialReadStringRequest\x1a%.GpioPackage.SerialReadStringResponse\"\x00\x12[\n\x0eserialReadUtil\x12\".GpioPackage.SerialReadUtilRequest\x1a#.GpioPackage.SerialReadUtilResponse\"\x00\x12p\n\x15\x63learAllGpioAndSerial\x12).GpioPackage.ClearAllGpioAndSerialRequest\x1a*.GpioPackage.ClearAllGpioAndSerialResponse\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'gpio_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _SETGPIOEXPORTREQUEST._serialized_start=27
@@ -26,42 +26,40 @@
   _SETGPIOEXPORTRESPONSE._serialized_end=129
   _READGPIOREQUEST._serialized_start=131
   _READGPIOREQUEST._serialized_end=161
   _READGPIORESPONSE._serialized_start=163
   _READGPIORESPONSE._serialized_end=224
   _SETGPIOSTARTEXPORTPWMREQUEST._serialized_start=226
   _SETGPIOSTARTEXPORTPWMREQUEST._serialized_end=323
-  _SETGPIOSTARTEXPORTPWMWITHDUTYCYCLEREQUEST._serialized_start=325
-  _SETGPIOSTARTEXPORTPWMWITHDUTYCYCLEREQUEST._serialized_end=435
-  _SETGPIOSTARTEXPORTPWMRESPONSE._serialized_start=437
-  _SETGPIOSTARTEXPORTPWMRESPONSE._serialized_end=495
-  _SETGPIOSTOPEXPORTPWMREQUEST._serialized_start=497
-  _SETGPIOSTOPEXPORTPWMREQUEST._serialized_end=539
-  _SETGPIOSTOPEXPORTPWMRESPONSE._serialized_start=541
-  _SETGPIOSTOPEXPORTPWMRESPONSE._serialized_end=598
-  _SETSERBAUDREQUEST._serialized_start=600
-  _SETSERBAUDREQUEST._serialized_end=651
-  _SETSERBAUDRESPONSE._serialized_start=653
-  _SETSERBAUDRESPONSE._serialized_end=700
-  _SERIALEXPORTSTRINGREQUEST._serialized_start=702
-  _SERIALEXPORTSTRINGREQUEST._serialized_end=758
-  _SERIALEXPORTSTRINGRESPONSE._serialized_start=760
-  _SERIALEXPORTSTRINGRESPONSE._serialized_end=815
-  _SERIALREADBYTEREQUEST._serialized_start=817
-  _SERIALREADBYTEREQUEST._serialized_end=854
-  _SERIALREADBYTERESPONSE._serialized_start=856
-  _SERIALREADBYTERESPONSE._serialized_end=923
-  _SERIALREADSTRINGREQUEST._serialized_start=925
-  _SERIALREADSTRINGREQUEST._serialized_end=964
-  _SERIALREADSTRINGRESPONSE._serialized_start=966
-  _SERIALREADSTRINGRESPONSE._serialized_end=1035
-  _SERIALREADUTILREQUEST._serialized_start=1037
-  _SERIALREADUTILREQUEST._serialized_end=1089
-  _SERIALREADUTILRESPONSE._serialized_start=1091
-  _SERIALREADUTILRESPONSE._serialized_end=1158
-  _CLEARALLGPIOANDSERIALREQUEST._serialized_start=1160
-  _CLEARALLGPIOANDSERIALREQUEST._serialized_end=1190
-  _CLEARALLGPIOANDSERIALRESPONSE._serialized_start=1192
-  _CLEARALLGPIOANDSERIALRESPONSE._serialized_end=1250
-  _GPIOSERVICEGRPC._serialized_start=1253
-  _GPIOSERVICEGRPC._serialized_end=2386
+  _SETGPIOSTARTEXPORTPWMRESPONSE._serialized_start=325
+  _SETGPIOSTARTEXPORTPWMRESPONSE._serialized_end=383
+  _SETGPIOSTOPEXPORTPWMREQUEST._serialized_start=385
+  _SETGPIOSTOPEXPORTPWMREQUEST._serialized_end=427
+  _SETGPIOSTOPEXPORTPWMRESPONSE._serialized_start=429
+  _SETGPIOSTOPEXPORTPWMRESPONSE._serialized_end=486
+  _SETSERBAUDREQUEST._serialized_start=488
+  _SETSERBAUDREQUEST._serialized_end=539
+  _SETSERBAUDRESPONSE._serialized_start=541
+  _SETSERBAUDRESPONSE._serialized_end=588
+  _SERIALEXPORTSTRINGREQUEST._serialized_start=590
+  _SERIALEXPORTSTRINGREQUEST._serialized_end=646
+  _SERIALEXPORTSTRINGRESPONSE._serialized_start=648
+  _SERIALEXPORTSTRINGRESPONSE._serialized_end=703
+  _SERIALREADBYTEREQUEST._serialized_start=705
+  _SERIALREADBYTEREQUEST._serialized_end=742
+  _SERIALREADBYTERESPONSE._serialized_start=744
+  _SERIALREADBYTERESPONSE._serialized_end=811
+  _SERIALREADSTRINGREQUEST._serialized_start=813
+  _SERIALREADSTRINGREQUEST._serialized_end=852
+  _SERIALREADSTRINGRESPONSE._serialized_start=854
+  _SERIALREADSTRINGRESPONSE._serialized_end=923
+  _SERIALREADUTILREQUEST._serialized_start=925
+  _SERIALREADUTILREQUEST._serialized_end=977
+  _SERIALREADUTILRESPONSE._serialized_start=979
+  _SERIALREADUTILRESPONSE._serialized_end=1046
+  _CLEARALLGPIOANDSERIALREQUEST._serialized_start=1048
+  _CLEARALLGPIOANDSERIALREQUEST._serialized_end=1078
+  _CLEARALLGPIOANDSERIALRESPONSE._serialized_start=1080
+  _CLEARALLGPIOANDSERIALRESPONSE._serialized_end=1138
+  _GPIOSERVICEGRPC._serialized_start=1141
+  _GPIOSERVICEGRPC._serialized_end=2133
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ugot-0.2.13/ugot/grpc_pb/gpio_pb2_grpc.py` & `ugot-0.2.9/ugot/grpc_pb/gpio_pb2_grpc.py`

 * *Files 15% similar despite different names*

```diff
@@ -52,19 +52,14 @@
                 response_deserializer=gpio__pb2.ReadGpioResponse.FromString,
                 )
         self.setGpioStartExportPwm = channel.unary_unary(
                 '/GpioPackage.GpioServiceGrpc/setGpioStartExportPwm',
                 request_serializer=gpio__pb2.SetGpioStartExportPwmRequest.SerializeToString,
                 response_deserializer=gpio__pb2.SetGpioStartExportPwmResponse.FromString,
                 )
-        self.setGpioStartExportPwmWithDutyCycle = channel.unary_unary(
-                '/GpioPackage.GpioServiceGrpc/setGpioStartExportPwmWithDutyCycle',
-                request_serializer=gpio__pb2.SetGpioStartExportPwmWithDutyCycleRequest.SerializeToString,
-                response_deserializer=gpio__pb2.SetGpioStartExportPwmResponse.FromString,
-                )
         self.setGpioStopExportPwm = channel.unary_unary(
                 '/GpioPackage.GpioServiceGrpc/setGpioStopExportPwm',
                 request_serializer=gpio__pb2.SetGpioStopExportPwmRequest.SerializeToString,
                 response_deserializer=gpio__pb2.SetGpioStopExportPwmResponse.FromString,
                 )
         self.setSerbaud = channel.unary_unary(
                 '/GpioPackage.GpioServiceGrpc/setSerbaud',
@@ -126,89 +121,72 @@
 
 
     定义服务,用在rpc传输中
     """
 
     def setGpioExport(self, request, context):
         """gpio
-        设置 gpio 引脚输出
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def readGpio(self, request, context):
-        """读取 gpio 引脚输出
-        """
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def setGpioStartExportPwm(self, request, context):
-        """设置 gpio 引脚输出 PWM
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def setGpioStartExportPwmWithDutyCycle(self, request, context):
-        """设置 gpio 引脚输出 PWM 并设置占空比
-        """
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def setGpioStopExportPwm(self, request, context):
-        """停止 gpio 引脚输出 PWM
-        """
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def setSerbaud(self, request, context):
         """serial
-        设置串口波特率
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def serialExportString(self, request, context):
-        """将字符串发送
-        """
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def serialReadByte(self, request, context):
         """将数字转换成字符串发送
         rpc serialExportNum(SerialExportNumRequest) returns (SerialExportNumResponse) {};
-        读取串口发送的字符
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def serialReadString(self, request, context):
-        """读取串口发送的字符串
-        """
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def serialReadUtil(self, request, context):
-        """读取串口发送的字符，直到读取到指定字符
-        """
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def clearAllGpioAndSerial(self, request, context):
-        """清除所有 gpio 和 serial
-        """
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_GpioServiceGrpcServicer_to_server(servicer, server):
     rpc_method_handlers = {
@@ -223,19 +201,14 @@
                     response_serializer=gpio__pb2.ReadGpioResponse.SerializeToString,
             ),
             'setGpioStartExportPwm': grpc.unary_unary_rpc_method_handler(
                     servicer.setGpioStartExportPwm,
                     request_deserializer=gpio__pb2.SetGpioStartExportPwmRequest.FromString,
                     response_serializer=gpio__pb2.SetGpioStartExportPwmResponse.SerializeToString,
             ),
-            'setGpioStartExportPwmWithDutyCycle': grpc.unary_unary_rpc_method_handler(
-                    servicer.setGpioStartExportPwmWithDutyCycle,
-                    request_deserializer=gpio__pb2.SetGpioStartExportPwmWithDutyCycleRequest.FromString,
-                    response_serializer=gpio__pb2.SetGpioStartExportPwmResponse.SerializeToString,
-            ),
             'setGpioStopExportPwm': grpc.unary_unary_rpc_method_handler(
                     servicer.setGpioStopExportPwm,
                     request_deserializer=gpio__pb2.SetGpioStopExportPwmRequest.FromString,
                     response_serializer=gpio__pb2.SetGpioStopExportPwmResponse.SerializeToString,
             ),
             'setSerbaud': grpc.unary_unary_rpc_method_handler(
                     servicer.setSerbaud,
@@ -352,31 +325,14 @@
         return grpc.experimental.unary_unary(request, target, '/GpioPackage.GpioServiceGrpc/setGpioStartExportPwm',
             gpio__pb2.SetGpioStartExportPwmRequest.SerializeToString,
             gpio__pb2.SetGpioStartExportPwmResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def setGpioStartExportPwmWithDutyCycle(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/GpioPackage.GpioServiceGrpc/setGpioStartExportPwmWithDutyCycle',
-            gpio__pb2.SetGpioStartExportPwmWithDutyCycleRequest.SerializeToString,
-            gpio__pb2.SetGpioStartExportPwmResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def setGpioStopExportPwm(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `ugot-0.2.13/ugot/grpc_pb/model_pb2.py` & `ugot-0.2.9/ugot/grpc_pb/model_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/grpc_pb/model_pb2_grpc.py` & `ugot-0.2.9/ugot/grpc_pb/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/grpc_pb/network_pb2.py` & `ugot-0.2.9/ugot/grpc_pb/network_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/grpc_pb/network_pb2_grpc.py` & `ugot-0.2.9/ugot/grpc_pb/network_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/grpc_pb/power_pb2.py` & `ugot-0.2.9/ugot/grpc_pb/power_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/grpc_pb/power_pb2_grpc.py` & `ugot-0.2.9/ugot/grpc_pb/power_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/grpc_pb/sensor_pb2.py` & `ugot-0.2.9/ugot/grpc_pb/sensor_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/grpc_pb/sensor_pb2_grpc.py` & `ugot-0.2.9/ugot/grpc_pb/sensor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/grpc_pb/servo_pb2.py` & `ugot-0.2.9/ugot/grpc_pb/servo_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/grpc_pb/servo_pb2_grpc.py` & `ugot-0.2.9/ugot/grpc_pb/servo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/grpc_pb/vision_pb2.py` & `ugot-0.2.9/ugot/grpc_pb/vision_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/grpc_pb/vision_pb2_grpc.py` & `ugot-0.2.9/ugot/grpc_pb/vision_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/src/PID.py` & `ugot-0.2.9/ugot/src/PID.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         """
         Set the error of pid controller
 
         Args:
             error (float): error
 
         Returns:
-            output (float):
+            None
         """
         
         error = self.__SetPoint - feedback_value
 
         self.__current_time = current_time if current_time is not None else time.time()
         delta_time = self.__current_time - self.__last_time
         delta_error = error - self.__last_error
```

### Comparing `ugot-0.2.13/ugot/src/audio_client.py` & `ugot-0.2.9/ugot/src/audio_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,10 +100,9 @@
         return response
 
     def __del__(self):
         # # 销毁时候停止所有声音
         try:
             self.stopPlayAudio()
         except Exception as e:
-            # logging.debug('audio stopPlayAudio error:')
-            pass
+            print('audio stopPlayAudio error:')
         pass
```

### Comparing `ugot-0.2.13/ugot/src/base_client.py` & `ugot-0.2.9/ugot/src/base_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/src/bluetooth_client.py` & `ugot-0.2.9/ugot/src/bluetooth_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/src/device_client.py` & `ugot-0.2.9/ugot/src/device_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,21 +144,14 @@
         return response
     
     def getDeviceModel(self):
         input_data = device_pb2.DeviceModelRequest()
 
         response = self.client.getDeviceModel(input_data)
         return response.name
-    
-    def getLanguage(self):
-        input_data = device_pb2.GetLangRequest()
-
-        response = self.client.getLanguage(input_data)
-        return response
 
     def __del__(self):
         # # 销毁时候停止灯光
         try:
             self.turnOffAllLights()
         except Exception as e:
-            # logging.debug('device turnOffAllLights error:')
-            pass
+            print('device turnOffAllLights error:')
```

### Comparing `ugot-0.2.13/ugot/src/enum.py` & `ugot-0.2.9/ugot/src/enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,19 +157,14 @@
         green = 3  # 绿色
         red = 4  # 红色
 
     class LineType:
         single = 0  # 单轨
         double = 1  # 双轨
 
-    class Toy:
-        YOUYOU = 0 # 优悠
-        WALKERX = 1 # walkerx
-        WALKER = 2 # walker
-
 class E_Audio:
     class Volume:
         MINIMUM = 1  # 最小 20%
         LOW = 2  # 小 40%
         MEDIUM = 3  # 中 60%
         HIGH = 4  # 大 80%
         MAXIMUM = 5  # 最大 100%
```

### Comparing `ugot-0.2.13/ugot/src/gpio_client.py` & `ugot-0.2.9/ugot/src/gpio_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -42,23 +42,14 @@
         input_data = gpio_pb2.SetGpioStartExportPwmRequest()
         input_data.pin = pin
         input_data.frequency = 490  # 频率，默认为490Hz
         input_data.duty_cycle = int(duty_cycle)
         input_data.range = 255  # 范围，目前需求是255
         response = self.client.setGpioStartExportPwm(input_data)
         return response
-    
-    def setGpioStartExportPwmWithDutyCycle(self, pin, duty_cycle, frequency = 490): #频率默认未490Hz
-        input_data = gpio_pb2.SetGpioStartExportPwmWithDutyCycleRequest()
-        input_data.pin = pin
-        input_data.frequency = frequency #频率，默认为490Hz
-        input_data.duty_cycle = duty_cycle # 0 ~ 100.0 的值，范围（0.0 ～ 100.0）
-        input_data.range = 100
-        response = self.client.setGpioStartExportPwmWithDutyCycle(input_data)
-        return response
 
     def setGpioStopExportPwm(self, pin):
         input_data = gpio_pb2.SetGpioStopExportPwmRequest()
         input_data.pin = pin
 
         response = self.client.setGpioStopExportPwm(input_data)
         return response
@@ -109,9 +100,9 @@
         return response
 
     def __del__(self):
         # 销毁时候释放串口资源
         try:
             self.clearAllGpioAndSerial()
         except Exception as e:
-            # logging.debug('gpio clearAllGpioAndSerial error:')
-            pass
+            print('gpio clearAllGpioAndSerial error:')
+        pass
```

### Comparing `ugot-0.2.13/ugot/src/http_client.py` & `ugot-0.2.9/ugot/src/http_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/src/model_client.py` & `ugot-0.2.9/ugot/src/model_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,9 +317,8 @@
         return response
     
     def __del__(self):
         # 销毁时候停止模型
         try:
             self.stopAllModels()
         except Exception as e:
-            # logging.debug('model stopAllModels error:')
-            pass
+            print('model stopAllModels error:')
```

### Comparing `ugot-0.2.13/ugot/src/network_client.py` & `ugot-0.2.9/ugot/src/network_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,21 +114,17 @@
     def get_joypad_button_state(self):
 
         result = self.getBTJoypadStatus()
 
         if result is None or len(result) == 0:
             # 没有获取到事件
             return []
-        
-        try:
-            data = json.loads(result)
-            if data is None:
-                return []
-        except:
-            # logging.error('get_joypad_button_state json loads error')
+
+        data = json.loads(result)
+        if data is None:
             return []
 
         pressed_btns = []
         arrow = data['arrow']
         if arrow['l'] == 1:
             pressed_btns.append(E_Joypad.L)
         if arrow['r'] == 1:
@@ -174,21 +170,17 @@
     def get_joypad_coordinate(self):
         result = self.getBTJoypadStatus()
 
         if result is None or len(result) == 0:
             # 没有获取到事件
             return []
 
-        try:
-            data = json.loads(result)
-            if data is None:
-                # logging.debug("warning-----no data in get_bt_joypad_status")
-                return []
-        except:
-            # logging.error('get_joypad_coordinate json loads error')
+        data = json.loads(result)
+        if data is None:
+            logging.debug("warning-----no data in get_bt_joypad_status")
             return []
 
         sticks = []
         stick = data['stick']
         sticks.append(stick['l']['x'])
         sticks.append(stick['l']['y'])
         sticks.append(stick['r']['x'])
```

### Comparing `ugot-0.2.13/ugot/src/power_client.py` & `ugot-0.2.9/ugot/src/power_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/src/scan_device.py` & `ugot-0.2.9/ugot/src/scan_device.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/src/sensor_client.py` & `ugot-0.2.9/ugot/src/sensor_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/src/servo_client.py` & `ugot-0.2.9/ugot/src/servo_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,9 +202,8 @@
         return response
     
     def __del__(self):
         # 销毁时候停止模型
         try:
             self.stopAllServos()
         except Exception as e:
-            # logging.debug('servo stopAllServos error:')
-            pass
+            print('servo stopAllServos error:')
```

### Comparing `ugot-0.2.13/ugot/src/util.py` & `ugot-0.2.9/ugot/src/util.py`

 * *Files identical despite different names*

### Comparing `ugot-0.2.13/ugot/src/vision_client.py` & `ugot-0.2.9/ugot/src/vision_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 MODELNAME_LICENSE_PLATE = 'lpd_recognition' # 车牌识别
 MODELNAME_GESTURE = 'gesture' # 手势识别
 MODELNAME_TRAFFIC = 'traffic_sign' # 交通识别，交通标识以及斑马线
 MODELNAME_OBJECT_RECOGNITION = 'object_recognition' # 物体识别
 MODELNAME_FACE_RECOGNITION = 'face_recognition' # 人脸识别
 MODELNAME_TRACK_RECOGNITION = 'line_recognition' # 单双轨
 MODELNAME_COLOR_TRACK = 'color_tracking' # 自定义颜色
-MODELNAME_TOY_RECOGNITION = 'toy_recognition' # 公仔识别
 
 MODEL_REFLECT_LIST = {
     MODELNAME_KNN, # = 0 # knn
     MODELNAME_POSE, # = 1 # 人体姿态
     MODELNAME_WORD, # = 2 # 文字识别
     MODELNAME_COLOR, # = 3 # 颜色识别
     MODELNAME_APRILTAG, # = 4 # ArpilTag
@@ -46,15 +45,14 @@
     MODELNAME_LICENSE_PLATE, # = 8 # 车牌识别
     MODELNAME_GESTURE, # = 9 # 手势识别
     MODELNAME_TRAFFIC, # = 10 # 交通识别，交通标识以及斑马线
     MODELNAME_OBJECT_RECOGNITION, # = 11 # 物体识别
     MODELNAME_FACE_RECOGNITION, # = 12 # 人脸识别
     MODELNAME_TRACK_RECOGNITION, # = 13 # 单双轨
     # MODELNAME_COLOR_TRACK, # = 14 # 自定义颜色
-    MODELNAME_TOY_RECOGNITION, # = 15 # 公仔识别
 }
 
 class VisionClient(GrpcClient):
     def __init__(self, address):
         super().__init__(address)
 
         self.camera_client_id = -1
@@ -143,65 +141,14 @@
         for model in models:
             info = input_data.models.add()
             info.model = model
             para = {"model_name": model_name}
             info.para = json.dumps(para)
         response = self.client.loadModel(input_data)
 
-    def knn_train(self, model_name, label_list):
-        model = MODELNAME_KNN
-
-        input_data = vision_pb2.TrainAndSaveRequest()
-        input_data.model = model
-        input_data.para.name = model_name
-
-        for label in label_list:
-            input_data.para.categoryNames.append(label)
-        response = self.client.trainAndSave(input_data)
-        for feature in response:  # 流式返回的结果
-            yield feature
-
-    def knn_rename(self, src_name, dst_name):
-        model = MODELNAME_KNN
-        input_data = vision_pb2.SetModelParaRequest()
-        input_data.model = model
-        input_data.invoke = "KnnModelRename"
-        para = {"src_name":src_name, "dst_name":dst_name}
-        input_data.para = json.dumps(para)
-        response = self.client.setModelPara(input_data)
-        if response.code != 0:
-            print('knn_rename: {}'.format(response.msg))
-        return response
-
-    def knn_delete(self, model_name):
-        model = MODELNAME_KNN
-        input_data = vision_pb2.SetModelParaRequest()
-        input_data.model = model
-        input_data.invoke = "KnnModelAndLabelDelete"
-        para = {"model_name":model_name}
-        input_data.para = json.dumps(para)
-        response = self.client.setModelPara(input_data)
-        code = response.code
-        if code != 0:
-            if code == 1001:
-                print('knn_delete: {}'.format('file name not exist!'))
-        return response
-
-    def knn_query(self):
-        model = MODELNAME_KNN
-        input_data = vision_pb2.SetModelParaRequest()
-        input_data.model = model
-        input_data.invoke = "knnModelAndLabelQuery"
-        para = {}
-        input_data.para = json.dumps(para)
-        response = self.client.setModelPara(input_data)
-        if response.code != 0:
-            print('knn_query: {}'.format(response.msg))
-        return response
-
     """ 人体姿态
     """
 
 
     def pose_identify(self):
         """人体姿态推理
         Args:
@@ -497,28 +444,14 @@
         para = {"color_name": color_name}
         info.para = json.dumps(para)
         response = self.client.doModelInference(input_data)
         for item in response.data.inference:
             if item.model == model:
                 return item.data
         return None
-    
-    """ 公仔识别 """
-    def toy_recognition_inference(self):
-        model = MODELNAME_TOY_RECOGNITION
-
-        input_data = vision_pb2.InferenceRequest()
-        input_data.need_pic = False
-        info = input_data.models.add()
-        info.model = model
-        response = self.client.doModelInference(input_data)
-        for item in response.data.inference:
-            if item.model == model:
-                return item.data
-        return None
 
 
 
     def unloadAllModels(self):
 
         # 释放模型
         input_data = vision_pb2.ReleaseModelRequest()
@@ -563,12 +496,11 @@
         response = self.client.readCameraData(input_data)
         return response
 
     def __del__(self):
         # # 销毁时候卸载所有模型
         try:
             self.unloadAllModels()
-            if self.camera_client_id > 0:
-                self.closeCamera(self.camera_client_id)
+            self.closeCamera(self.camera_client_id)
         except Exception as e:
-            # logging.debug('vision unloadAllModels error:')
-            pass
+            print('vision unloadAllModels error:')
+        pass
```

### Comparing `ugot-0.2.13/ugot/ugot.py` & `ugot-0.2.9/ugot/ugot.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,14 @@
 
 import logging
 import json
 import threading
 import time
 import sys
 import base64
-import os
-
-LANGUAGE_CONFIGURE = None # 语言配置
-
-def _get_translation(key):
-    global LANGUAGE_CONFIGURE
-    return LANGUAGE_CONFIGURE.get_value_for_key(key)
 
 class UGOT:
 
 
     def __init__(self):
         self.http_basic_url = ''
         self.current_mode = ''
@@ -56,41 +49,35 @@
             
         """
         t = threading.Thread(target= self.__scan)
         t.start()
         t.join()
         return DEV_LIST
 
-    def initialize(self, device_ip = None):
+    def initialize(self, device_ip):
         """Initialize a device
 
         Initialize the relevant device using its IP address.
 
         Args:
             device_ip (str): IP address of the device as a string
 
         Returns:
             None
 
         """
-        device_ip = str(device_ip)
-        if device_ip is None or len(device_ip) == 0:
-            # 如果没传或者传空字符串，默认初始化本机
-            device_ip = '0.0.0.0'
         if len(device_ip) == 0:
             print("please input device ip !")
             return
         address = device_ip + ':50051'
         print(address)
         self.__initialize_modules(address)
 
         self.__initialize_http_client(device_ip)
 
-        self.__configure_language()
-
     def __initialize_modules(self, address):
 
         self.MODEL = ModelClient(address)
         self.VISION = VisionClient(address)
         self.DEVICE = DeviceClient(address)
         self.AUDIO = AudioClient(address)
         self.SENSOR = SensorClient(address)
@@ -99,33 +86,14 @@
         self.BLUETOOTH = BlueToothClient(address)
         self.SERVO = ServoClient(address)
         self.GPIO = GpioClient(address)
 
     def __initialize_http_client(self, device_ip):
         self.http_basic_url = 'http://' + device_ip + ':7000/'
 
-    def __configure_language(self):
-        response = self.DEVICE.getLanguage()
-        cur_language = 'en' # 默认为英文
-        if response.code == 0:
-            lang = response.lang.lower()
-            if lang == "china":
-                cur_language = "zh_CN"
-            elif lang == "korea":
-                cur_language = "ko"
-            elif lang == "global":
-                cur_language = "en"
-
-        global LANGUAGE_CONFIGURE
-
-        from ugot.src.configure_string_single import ConfigureStringSingle
-        configure_file_path = os.path.dirname(os.path.realpath(__file__)) + "/src/locale"
-        LANGUAGE_CONFIGURE = ConfigureStringSingle(configure_file_path, 'ugot', language=[cur_language])
-
-
     """
 
     >>>>>>>>>>>
     >> Servo & Motor <<
     >>>>>>>>>>>
 
     """
@@ -315,64 +283,14 @@
                 result[info.deviceId] = info.speed
                 # result.append({'deviceId':info.deviceId, 'speed': info.speed})
                 # if info.deviceId == str(id):
                 #     logging.debug('read servo id:{} `s speed is {}'.format(id, info.speed))
                 #     return info.speed
             return result
         return result
-    
-    def turn_motor_angle(self, id, angle, duration_ms, wait = False):
-        """Control a motor to rotate by a specified angle over a duration.
-
-        Args:
-            id (int/list[int]): Motor ID/ID list
-            angle (int): [-180, 180] Angle to rotate, in degrees
-            duration_ms (int): Runtime [20, 5000] in milliseconds
-            wait (bool, optional): Block until completion, default is False (non-blocking)
-
-        Returns:
-            None
-
-        """
-        func_name = sys._getframe().f_code.co_name
-        if not self.__validate_servo_id(id,func_name):
-            return
-
-        angle = num_normal(angle, 180, -180)
-        duration_ms = num_normal(duration_ms, 5000, 20)
-
-        self.SERVO.setServoRotateByAngle(id, angle, duration_ms, type=JOINT_TYPE_MOTOR)
-        if wait:
-            time.sleep(duration_ms / 1000.0)
-
-    def read_motor_angle(self, id):
-        """
-        Read motor angle(s).
-
-        Args:
-            id (int/list[int]): Motor ID/ID list
-
-        Returns:
-            angle_list (dict): Format: {"Motor ID 1": "Angle of Motor 1", "Motor ID 2": "Angle of Motor 2", ...}
-
-        """
-        result = {}
-
-        func_name = sys._getframe().f_code.co_name
-        if not self.__validate_servo_id(id,func_name):
-            return
-
-        angle_list = self.SERVO.getServoAngle(id, type=JOINT_TYPE_MOTOR)
-        if angle_list is not None:
-            for info in angle_list:
-                result[info.deviceId] = info.angle
-                # if info.deviceId == str(id):
-                #     return info.angle
-            return result
-        return {}
 
     def stop_motor(self, id, lock = False):
         """
         Stop a motor.
 
         Args:
             id (int/list[int]): Motor ID/Motor ID list
@@ -502,24 +420,25 @@
             max_turn_speed = 60
         elif model == E_Model.ChassisMode.dog:
             max_linear_speed = 25
             max_turn_speed = 20
         # 前进/后退方向只有正数，转弯方向有正负
         speed = num_normal(speed, max_linear_speed, 0)
         turn_speed = num_normal(turn_speed, max_turn_speed, -max_turn_speed)
+        # print('线速度：{} 角速度：{}'.format(speed, turn_speed))
         return speed, turn_speed
     
     """
 
     >>>>>>>>>>>
     >> 变形车 - Transformable Vehicle <<
     >>>>>>>>>>>
 
     """
-    def transform_set_chassis_height(self, height: int):
+    def transform_set_chassis_height(self, height: float):
         """
         Set the chassis height of a transformable vehicle.
 
         Args:
             height (int): [2-7] in centimeters
 
         Returns:
@@ -544,15 +463,15 @@
             direction (int): Direction (0: Forward; 1: Backward)
             speed (int): [5-80] Speed in centimeters per second
 
         Returns:
             None
 
         """
-        speed = num_normal(speed, 80, 0)
+        speed = num_normal(speed, 80, 5)
         if direction == E_Model.Direction.forward:
             self.MODEL.transform_move_control(linear_speed=speed, direction=0)
         elif direction == E_Model.Direction.backward:
             self.MODEL.transform_move_control(linear_speed=speed, direction=180)
         else:
             self.__print_move_direction_error_msg(sys._getframe().f_code.co_name, direction)
 
@@ -600,15 +519,15 @@
             return
 
         if times == 0:
             # 时长/里程等于0，此积木块不做控制
             logging.error('Duration/range is 0; this block does not perform any control')
             return
 
-        speed = num_normal(speed, 80, 0)
+        speed = num_normal(speed, 80, 5)
         times = num_normal(times, 360, 0)
 
         if unit == E_Model.Unit.second:
             self.MODEL.transform_move_control(linear_speed=speed, direction=tar_direction, time=times)
         elif unit == E_Model.Unit.mileage:
             self.MODEL.transform_move_control(linear_speed=speed, direction=tar_direction, mileage=times)
         else:
@@ -681,15 +600,15 @@
             tar_speed = turn_speed
         elif turn == E_Model.Direction.turn_right:
             tar_speed = -turn_speed
         else:
             self.__print_move_turn_error_msg(sys._getframe().f_code.co_name, turn)
             return
 
-        speed = num_normal(speed, 80, 0)
+        speed = num_normal(speed, 80, 5)
 
         self.MODEL.transform_move_control(linear_speed=speed, direction=tar_direction, rotate_speed=tar_speed)
 
     def transform_motor_control(self, lf, rf, lb, rb):
         """
         Control the four motors of the transformable vehicle
 
@@ -712,15 +631,15 @@
     def transform_stop(self):
         """
         Stop the transformable vehicle's movement
 
         Returns:
             None
         """
-        self.MODEL.transform_move_control(linear_speed=0, direction=0)
+        self.MODEL.stop(MODEL_TYPE_TRANSFORM)
 
     def transform_restory(self):
         """
         Restore the transformable vehicle
 
         Returns:
             None
@@ -783,15 +702,15 @@
             angle (int): [-180, 180] angle unit: degrees (in the XY plane, with the Y-axis as the 0-degree direction, left [0, -180] right [0, 180])
             speed (int): [5-80] forward/backward speed, unit in centimeters/second
 
         Returns:
             None
         """
         angle = num_normal(angle, 180, -180)
-        speed = num_normal(speed, 80, 0)
+        speed = num_normal(speed, 80, 5)
         self.MODEL.mecanum_move_control(linear_speed=speed, direction=angle)
 
     def mecanum_translate_speed_times(self, angle, speed, times, unit):
         """
         Translate the mecanum-wheeled vehicle in a specific direction for x seconds/cm and then stop
 
         Args:
@@ -805,15 +724,15 @@
         """
         if times == 0:
             # 时长/里程等于0，此积木块不做控制
             logging.error('Duration/range is 0; this block does not perform any control')
             return
 
         angle = num_normal(angle, 180, -180)
-        speed = num_normal(speed, 80, 0)
+        speed = num_normal(speed, 80, 5)
         times = num_normal(times, 360, 0)
 
         if unit == E_Model.Unit.second:
             self.MODEL.mecanum_move_control(linear_speed=speed, direction=angle, time=times)
         elif unit == E_Model.Unit.mileage:
             self.MODEL.mecanum_move_control(linear_speed=speed, direction=angle, mileage=times)
         else:
@@ -844,15 +763,15 @@
         Args:
             direction (int): Direction (0: forward; 1: backward)
             speed (int): [5-80] speed, unit in centimeters/second
 
         Returns:
             None
         """
-        speed = num_normal(speed, 80, 0)
+        speed = num_normal(speed, 80, 5)
         if direction == E_Model.Direction.forward:
             self.MODEL.mecanum_move_control(linear_speed=speed, direction=0)
         elif direction == E_Model.Direction.backward:
             self.MODEL.mecanum_move_control(linear_speed=speed, direction=180)
         else:
             self.__print_move_direction_error_msg(sys._getframe().f_code.co_name, direction)
             return
@@ -901,15 +820,15 @@
             return
 
         if times == 0:
             # 时长/里程等于0，此积木块不做控制
             logging.error('Duration/range is 0; this block does not perform any control')
             return
 
-        speed = num_normal(speed, 80, 0)
+        speed = num_normal(speed, 80, 5)
         times = num_normal(times, 360, 0)
 
         if unit == E_Model.Unit.second:
             self.MODEL.mecanum_move_control(linear_speed=speed, direction=tar_direction, time=times)
         elif unit == E_Model.Unit.mileage:
             self.MODEL.mecanum_move_control(linear_speed=speed, direction=tar_direction, mileage=times)
         else:
@@ -974,15 +893,15 @@
             tar_speed = turn_speed
         elif turn == E_Model.Direction.turn_right:
             tar_speed = -turn_speed
         else:
             self.__print_move_turn_error_msg(sys._getframe().f_code.co_name, turn)
             return
 
-        speed = num_normal(speed, 80, 0)
+        speed = num_normal(speed, 80, 5)
 
         self.MODEL.mecanum_move_control(linear_speed=speed, direction=angle, rotate_speed=tar_speed)
 
     def mecanum_motor_control(self, lf, rf, lb, rb):
         """
         Control the four motors of the mecanum-wheeled vehicle
 
@@ -1073,15 +992,15 @@
         Args:
             direction (int): Direction (0: Forward; 1: Backward)
             speed (int): [5-80] Speed in centimeters per second
 
         Returns:
             None
         """
-        speed = num_normal(speed, 80, 0)
+        speed = num_normal(speed, 80, 5)
         if direction == E_Model.Direction.forward:
             self.MODEL.balance_move_control(linear_speed=speed, direction=0)
         elif direction == E_Model.Direction.backward:
             self.MODEL.balance_move_control(linear_speed=speed, direction=180)
         else:
             self.__print_move_direction_error_msg(sys._getframe().f_code.co_name, direction)
             return
@@ -1129,15 +1048,15 @@
             return
 
         if times == 0:
             # 时长/里程等于0，此积木块不做控制
             logging.error('Duration/range is 0; this block does not perform any control')
             return
 
-        speed = num_normal(speed, 80, 0)
+        speed = num_normal(speed, 80, 5)
         times = num_normal(times, 360, 0)
 
         if unit == E_Model.Unit.second:
             self.MODEL.balance_move_control(linear_speed=speed, direction=tar_direction, time=times)
         elif unit == E_Model.Unit.mileage:
             self.MODEL.balance_move_control(linear_speed=speed, direction=tar_direction, mileage=times)
         else:
@@ -1209,15 +1128,15 @@
             tar_speed = turn_speed
         elif turn == E_Model.Direction.turn_right:
             tar_speed = -turn_speed
         else:
             self.__print_move_turn_error_msg(sys._getframe().f_code.co_name, turn)
             return
 
-        speed = num_normal(speed, 80, 0)
+        speed = num_normal(speed, 80, 5)
 
         self.MODEL.balance_move_control(linear_speed=speed, direction=tar_direction, rotate_speed=tar_speed)
 
 
     """
 
     >>>>>>>>>>>
@@ -1796,14 +1715,41 @@
         Restore the four-legged dog robot.
 
         Returns:
             None
         """
         self.MODEL.restory(MODEL_TYPE_DOG)
 
+    # def dog_set_chassis_height(self, height, pose):
+    #     """
+    #     设置四足狗底盘高度
+
+    #     Args:
+    #         height (int/float): 高度 [11.7, 13.2] 单位 厘米
+    #         pose (int): 姿态（0：原地站立；1：运动）
+
+    #     Returns:
+    #         无
+    #     """
+    #     if not (isinstance(height, float) or isinstance(height, int)):
+    #         typestr = 'int or float is required (got type {})'.format(type(height).__name__)
+    #         func_name = sys._getframe().f_code.co_name
+    #         error_msg = 'TypeError: {}(): {}'.format(func_name, typestr)
+    #         print(error_msg)
+    #         return
+    #     if not 0 <= pose <= 1:
+    #         func_name = sys._getframe().f_code.co_name
+    #         typestr = 'invalid value of pose, expected 0/1, got {}'.format(pose)
+    #         error_msg = 'TypeError: {}(): {}'.format(func_name, typestr)
+    #         print(error_msg)
+    #         return
+    #     height = height * 10  # 换算成mm
+    #     height = int(num_normal(height, 132, 117))
+    #     self.MODEL.set_chassis_height(MODEL_TYPE_DOG, height, pose)
+
     def dog_set_decline_angle(self, pose, angle):
         """
         Set the inclination angle of the four-legged dog robot.
 
         Args:
             pose (int): Inclination direction (0: left-right inclination; 1: front-back inclination)
             angle (int): [-5, 5] angle in degrees
@@ -2036,16 +1982,15 @@
         """
         Load models, multiple models can be selected.
 
         Args:
             models (list): List of models to load. Correspondences: Human Pose: 'human_pose', Text Recognition: 'word_recognition',
                             Color Recognition: 'color_recognition', AprilTag/QR Code: 'apriltag_qrcode',
                             Emotion Recognition/Face Attributes: 'face_attribute', License Plate Detection: 'lpd_recognition', Gesture Recognition: 'gesture',
-                            Traffic Sign Recognition: 'traffic_sign', Face Recognition: 'face_recognition', Single Rail/Double Rail Recognition: 'line_recognition',
-                            Toy Recognition: 'toy_recognition'
+                            Traffic Sign Recognition: 'traffic_sign', Face Recognition: 'face_recognition', Single Rail/Double Rail Recognition: 'line_recognition'
 
         Returns:
             True if loading is successful, else False
         """
         if not len(models):
             typestr = 'models is empty!'
             func_name = sys._getframe().f_code.co_name
@@ -2179,41 +2124,39 @@
 
                         info = [qrcode, center_x, center_y, height, width, area]
                         result.append(info)
         try:
             import operator
             result.sort(key=operator.itemgetter(5), reverse=True)
         except Exception as e:
-            logging.debug('get_qrcode_total_info exception:', e)
+            print('get_qrcode_total_info exception:', e)
         logging.debug('-------get_qrcode_total_info `s result is {}'.format(result))
         return result
 
     def get_apriltag_total_info(self):
         """
         Get AprilTag information
 
         Args:
             None
 
         Returns:
-            AprilTag recognition result (list) [ [id, center_x, center_y, height, width, area, distance5, distance7, distance10, x, y, z, bearingAngle_h, bearingAngle_v], ... ]:
+            AprilTag recognition result (list) [ [id, center_x, center_y, height, width, area, distance5, distance7, distance10, x, y, z], ... ]:
             - id (int): AprilTag ID
             - center_x (float): AprilTag center x-coordinate
             - center_y (float): AprilTag center y-coordinate
             - height (float): AprilTag height
             - width (float): AprilTag width
             - area (float): AprilTag area
             - distance5 (float): AprilTag distance (5x5 cm)
             - distance7 (float): AprilTag distance (7x7 cm)
             - distance10 (float): AprilTag distance (10x10 cm)
             - x (float): AprilTag card pose angle x
             - y (float): AprilTag card pose angle y
             - z (float): AprilTag card pose angle z
-            - bearingAngle_h (float): AprilTag card horizontal bearing angle
-            - bearingAngle_v (float): AprilTag card vertical bearing angle
         """
         response = self.VISION.qrcode_inference()
 
         result = []
         if response is not None:
             data = json.loads(response)
             if data is not None:
@@ -2229,23 +2172,21 @@
                         area = round(position[3] * position[2], 2)
                         dis5 = round(item['instance'][0], 2)
                         dis7 = round(item['instance'][1], 2)
                         dis10 = round(item['instance'][2], 2)
                         x = round(item['pose_ypr'][0], 2)
                         y = round(item['pose_ypr'][1], 2)
                         z = round(item['pose_ypr'][2], 2)
-                        bearingAngle_h = round(item['bearingAngle'][0], 3)
-                        bearingAngle_v = round(item['bearingAngle'][1], 3)
-                        info = [id, center_x, center_y, height, width, area, dis5, dis7, dis10, x, y, z, bearingAngle_h, bearingAngle_v]
+                        info = [id, center_x, center_y, height, width, area, dis5, dis7, dis10, x, y, z]
                         result.append(info)
         try:
             import operator
             result.sort(key=operator.itemgetter(5), reverse=True)
         except Exception as e:
-            logging.debug('get_apriltag_total_info exception:', e)
+            print('get_apriltag_total_info exception:', e)
 
         logging.debug('-------get_apriltag_total_info `s result is {}'.format(result))
         return result
 
     def get_license_plate_total_info(self):
         """
         Get license plate information
@@ -2271,30 +2212,30 @@
         if response is not None:
             data = json.loads(response)
             if data is not None and isinstance(data, list):
                 for item in data:
                     number = item['lp']
                     type = item['type']
                     if type == E_Vision.LPD.blue:
-                        typestr = _get_translation('licensePlate.blue')
+                        typestr = '蓝牌'
                     elif type == E_Vision.LPD.green:
-                        typestr = _get_translation('licensePlate.green')
+                        typestr = '绿牌'
                     position = item['position']
                     center_x = position[0] + position[2] / 2
                     center_y = position[1] + position[3] / 2
                     width = position[2]
                     height = position[3]
                     area = position[2] * position[3]
                     info = [number, typestr, center_x, center_y, height, width, area]
                     result.append(info)
         try:
             import operator
             result.sort(key=operator.itemgetter(6), reverse=True)
         except Exception as e:
-            logging.debug('get_license_plate_total_info exception:', e)
+            print('get_license_plate_total_info exception:', e)
         logging.debug("get_license_plate_total_info `s result  is :{}".format(result))
         return result
 
     def get_pose_total_info(self):
         """
         Get the coordinates of recognized human keypoints
 
@@ -2355,47 +2296,47 @@
 
         if response is not None:
             data = json.loads(response)
             if data is not None and isinstance(data, list):
                 for item in data:
                     label = item["label"]
                     if label == E_Vision.Traffic.green_light:
-                        sign = _get_translation('traffic.greenLight')
+                        sign = '绿灯'
                     elif label == E_Vision.Traffic.horn:
-                        sign = _get_translation('traffic.whistle')
+                        sign = '鸣笛'
                     elif label == E_Vision.Traffic.left:
-                        sign = _get_translation('traffic.turnLeft')
+                        sign = '左转'
                     elif label == E_Vision.Traffic.right:
-                        sign = _get_translation('traffic.turnRight')
+                        sign = '右转'
                     elif label == E_Vision.Traffic.zebra_crossing:
-                        sign = _get_translation('traffic.zebraCrossing')
+                        sign = '斑马线'
                     elif label == E_Vision.Traffic.red_light:
-                        sign = _get_translation('traffic.redLight')
+                        sign = '红灯'
                     elif label == E_Vision.Traffic.children:
-                        sign = _get_translation('traffic.children')
+                        sign = '注意儿童'
                     elif label == E_Vision.Traffic.stop:
-                        sign = _get_translation('traffic.noPark')
+                        sign = '禁止长时间停车'
                     elif label == E_Vision.Traffic.tunnel:
-                        sign = _get_translation('traffic.tunnel')
+                        sign = '进入隧道'
                     elif label == E_Vision.Traffic.yellow_light:
-                        sign = _get_translation('traffic.amberLight')
+                        sign = '黄灯'
 
                     position = item['position']
                     center_x = round(position[0] + position[2] / 2, 2)
                     center_y = round(position[1] + position[3] / 2, 2)
                     width = round(position[2], 2)
                     height = round(position[3], 2)
                     area = round(position[2] * position[3], 2)
                     info = [sign, center_x, center_y, height, width, area]
                     result.append(info)
         try:
             import operator
             result.sort(key=operator.itemgetter(5), reverse=True)
         except Exception as e:
-            logging.debug('get_traffic_total_info exception:', e)
+            print('get_traffic_total_info exception:', e)
         logging.debug("get_traffic_total_info `s result is :{}".format(result))
         return result
 
     def get_face_recognition_total_info(self):
         """
         Get face recognition results
 
@@ -2418,28 +2359,28 @@
 
         if response is not None:
             data = json.loads(response)
             if data is not None and isinstance(data, list):
                 for item in data:
                     name = item['name']
                     if name == '':  # 有返回人脸，但是是没录入的，认为是陌生人
-                        name = _get_translation('face.stranger')
+                        name = '陌生人'
                     position = item['position']
                     center_x = position[0] + position[2] / 2
                     center_y = position[1] + position[3] / 2
                     width = position[2]
                     height = position[3]
                     area = position[2] * position[3]
                     info = [name, center_x, center_y, height, width, area]
                     result.append(info)
         try:
             import operator
             result.sort(key=operator.itemgetter(5), reverse=True)
         except Exception as e:
-            logging.debug('get_face_recognition_total_info exception:', e)
+            print('get_face_recognition_total_info exception:', e)
         logging.debug("get_face_recognition_total_info `s result  is :{}".format(result))
         return result
     
     # def open_camera(self):
     #     self.VISION.openCamera()
 
     def face_recognition_get_all_names(self):
@@ -2462,27 +2403,29 @@
         Args:
             name (str): Face name to delete
 
         Returns:
             None
         """
         response = self.VISION.face_recognition_delete_name(name)
+        print(response.data)
 
     def face_recognition_add_name(self, name):
         """
         Register a face
 
         Args:
             name (str): Face name to register
 
         Returns:
             None
         """
 
         names = self.VISION.face_recognition_get_all_names()
+        # print('names',names)
         for i in names:
             if i == name:
                 print('Face [{}] already exists'.format(name))
                 return None
         
         self.load_models(['face_recognition'])
 
@@ -2501,24 +2444,27 @@
             return None
         
 
         pdata = response.pdata
 
         import base64, os
         img = base64.b64decode(pdata)
+        # print('----------')
+        # print(img)
 
-        # tmp_img_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)),'tmp_image')
-        tmp_img_dir = os.path.dirname(os.path.realpath(__file__))
+        tmp_img_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)),'tmp_image')
+        # print(tmp_img_dir)
 
         if not os.path.exists(tmp_img_dir):
             os.system('mkdir -p ' + tmp_img_dir)
 
         image_name = '{}.jpg'.format(name)
 
         file_path = os.path.join(tmp_img_dir,image_name)
+        # print(file_path)
 
         with open(file_path,"wb") as fh:
             fh.write(img)
 
         upload_response = upload_vision_picture(self.http_basic_url, file_path)
         if not upload_response["code"] == 0:
             print('Failed to upload the image')
@@ -2526,23 +2472,25 @@
 
         response = self.VISION.face_recognition_insert_data(image_name, name)
         if response is not None:
             
             if response.code == 0:
                 data = response.data
                 data = json.loads(data)
+                # print('-----------',data)
                 print('Face [{}] registered successfully\n'.format(name))
             else:
                 msg = response.msg
+                # print('-----------',msg)
                 print('Face not found\n')
 
-        # from IPython.display import display
-        # from PIL import Image
-        # show_image = Image.open(file_path)
-        # display(show_image)
+        from IPython.display import display
+        from PIL import Image
+        show_image = Image.open(file_path)
+        display(show_image)
 
     def get_face_characteristic_total_info(self):
         """
         Get face characteristic recognition results
 
         Args:
             None
@@ -2564,34 +2512,34 @@
         if response is not None:
             data = json.loads(response)
             if data is not None and isinstance(data, list):
                 for item in data:
                     # 统计性别&口罩数量
                     gender = item["gender"]
                     if gender == 0:
-                        gender_str = _get_translation('face.man')
+                        gender_str = '男性'
                     elif gender == 1:
-                        gender_str = _get_translation('face.woman')
+                        gender_str = '女性'
 
                     mask = item["mask"]
                     if mask == 0:
-                        mask_str = _get_translation('face.wearMask')
+                        mask_str = '佩戴口罩'
                     elif mask == 1:
-                        mask_str = _get_translation('face.notProperlyMask')
+                        mask_str = '未佩戴口罩'
                     elif mask == 2:
-                        mask_str = _get_translation('face.noMask')
+                        mask_str = '未佩戴好口罩'
                     emotion = item["emotion"]
                     if emotion == 0:  # '生气'
-                        emotion_str = _get_translation('emotion.angry')
+                        emotion_str = '生气'
                     elif emotion == 1:  # '开心'
-                        emotion_str = _get_translation('emotion.happy')
+                        emotion_str = '开心'
                     elif emotion == 2:  # '平静'
-                        emotion_str = _get_translation('emotion.silence')
+                        emotion_str = '平静'
                     elif emotion == 3:  # '惊讶'
-                        emotion_str = _get_translation('emotion.amaze')
+                        emotion_str = '惊讶'
 
                     position = item['position']
                     center_x = position[0] + position[2] / 2
                     center_y = position[1] + position[3] / 2
                     width = position[2]
                     height = position[3]
                     area = position[2] * position[3]
@@ -2599,15 +2547,15 @@
                     face = [gender_str, mask_str, emotion_str, center_x, center_y, height, width, area]
                     result.append(face)
 
         try:
             import operator
             result.sort(key=operator.itemgetter(7), reverse=True)
         except Exception as e:
-            logging.debug('get_face_characteristic_total_info exception:', e)
+            print('get_face_characteristic_total_info exception:', e)
         logging.debug("get_face_characteristic_total_info `s result  is :{}".format(result))
         return result
 
     def __judge_track_line_type(self, data):
         cross_type = E_Vision.Intersection.noline  # 线类型
         line_type = E_Vision.LineType.single  # 单双轨类型
         max_item = None
@@ -2661,14 +2609,16 @@
                 double_start = data["double_start"]
                 double_end = data["double_end"]
                 if double_start[0] == -1 and double_start[1] == -1 and double_end[0] == -1 and double_end[1] == -1:
                     cross_type = E_Vision.Intersection.noline
                 else:
                     cross_type = E_Vision.Intersection.straight
 
+        # print("----cross_type:{}, line_type:{} max_item:{}".format(cross_type, line_type, max_item))
+
         return cross_type, line_type, max_item
 
     def set_track_recognition_line(self, line_type):
         """
         Set the current recognized lane line type
 
         Args:
@@ -2825,18 +2775,31 @@
                     if t_area > max_area:
                         max_area = t_area
                         max_item = item
 
                 # [{'area': 34581, 'color': 'red', 'shape': 'ball', "position" : [ 119, 272, 164, 143 ]}]
                 if max_item is not None:
                     color = max_item['color']
-                    colorstr = _get_translation(color)
+                    if color == 'red':
+                        colorstr = '红色'
+                    elif color == 'orange':
+                        colorstr = '橙色'
+                    elif color == 'yellow':
+                        colorstr = '黄色'
+                    elif color == 'green':
+                        colorstr = '绿色'
+                    elif color == 'blue':
+                        colorstr = '蓝色'
+                    elif color == 'purple':
+                        colorstr = '紫色'
                     shape = max_item['shape']
-                    typestr = _get_translation(shape)
-                    
+                    if shape == 'ball':
+                        typestr = '小球'
+                    elif shape == 'square':
+                        typestr = '方块'
                     position = max_item['position']
                     center_x = position[0] + position[2] / 2
                     center_y = position[1] + position[3] / 2
                     width = position[2]
                     height = position[3]
                     area = position[2] * position[3]
 
@@ -2886,23 +2849,23 @@
 
         if result is not None:
             data = json.loads(result)
             if data is None:
                 return ret
             gesture = data["gesture"]
             if gesture == 'stone':
-                ret = _get_translation('gesture.rock')
+                ret = '石头'
             elif gesture == 'scissor':
-                ret = _get_translation('gesture.scissors')
+                ret = '剪刀'
             elif gesture == 'palm':
-                ret = _get_translation('gesture.cloth')
+                ret = '布'
             elif gesture == 'ok':
-                ret = _get_translation('gesture.ok')
+                ret = 'OK'
             elif gesture == 'good':
-                ret = _get_translation('gesture.likes')
+                ret = '点赞'
             else:
                 ret = ''
             logging.debug('-------get_gesture_result is {}'.format(ret))
             return ret
             # {'confidence': 0.92, 'gesture': 'palm', 'position': [121, 352, 365, 244]]}
         return ret
     
@@ -2921,158 +2884,19 @@
         
         if response is not None:
             retList = json.loads(response)
             for data in retList:
                 # 类别不能重复，直接作为key
                 result[data["label_name"]] = int(round(data["confidence"], 2) * 100)
         return result
-    
-    def knn_train(self, model_name, label_list):
-        """
-        Train KNN model
-
-        Args:
-            model_name (str): KNN model name
-            label_list (list): label list to train
-
-        Returns:
-            Result(bool): True or False
-
-        """
-
-        func_name = sys._getframe().f_code.co_name
-        if not isinstance(label_list, list):
-            typestr = 'list is required (got type {})'.format(type(label_list).__name__)
-            error_msg = 'TypeError: {}(): {}'.format(func_name, typestr)
-            print(error_msg)
-            return False
-        else:
-            response = self.VISION.knn_train(model_name, label_list)
-            for item in response:
-                code = item.code
-                if code == 0:
-                    data = item.data
-                    data = json.loads(data)
-                    status = data["status"]
-                    if status == 0:
-                        print('knn training in progress')
-                    elif status == 2:
-                        print('knn training completed')
-                        return True
-                else:
-                    print('knn_train: {}'.format(item.msg))
-                    return False
-
-    def knn_rename(self, src_name, dst_name):
-        """
-        Rename the trained KNN model
-
-        Args:
-            src_name (str): Name before modification
-            dst_name (str): Name after modification
-
-        Returns:
-            Result(bool): True or False
-        """
-        response = self.VISION.knn_rename(src_name, dst_name)
-        if response.code == 0:
-            return True
-        return False
-
-    def knn_delete(self, model_name):
-        """
-        Delete the trained KNN model
-
-        Args:
-            model_name (str): model name
-
-        Returns:
-            Result(bool): True or False
-        """
-        response = self.VISION.knn_delete(model_name)
-        if response.code == 0:
-            return True
-        return False
-
-    def knn_query(self):
-        """
-        Get the list of trained KNN models
-
-        Args:
-            None
-
-        Returns:
-            model_list (dict): Format: { "model_name1": ["label11", "label12", ..], "model_name2": ["label21", "label22", ..] ...}, Returns None for no trained models!
-        """
-        response = self.VISION.knn_query()
-        if response.code == 0:
-            data = response.data
-            data = json.loads(data)
-            if data is None:
-                return None
-            result = {}
-            for info in data:
-                model_name = info["model_name"]
-                result[model_name] = info["label_list"]
-            return result
-
-        return None
-    
-    def get_toy_total_info(self):
-        """
-        Get toy information
-
-        Args:
-            None
-
-        Returns:
-            Toy recognition result (list) [ [label, center_x, center_y, height, width, area], ... ]:
-            - label (str): Toy label
-            - center_x (float): Center x-coordinate
-            - center_y (float): Center y-coordinate
-            - height (float): Height
-            - width (float): Width
-            - area (float): Area
-        """
-
-        response = self.VISION.toy_recognition_inference()
-
-        result = []
-
-        if response is not None:
-            data = json.loads(response)
-            if data is not None and isinstance(data, list):
-                for item in data:
-                    label = item['label']
-                    if label == E_Vision.Toy.YOUYOU:
-                        labelstr = _get_translation('toy.youyou')
-                    elif label == E_Vision.Toy.WALKERX:
-                        labelstr = _get_translation('toy.walkerx')
-                    elif label == E_Vision.Toy.WALKER:
-                        labelstr = _get_translation('toy.walker')
-                    position = item['position']
-                    center_x = position[0] + position[2] / 2
-                    center_y = position[1] + position[3] / 2
-                    width = position[2]
-                    height = position[3]
-                    area = position[2] * position[3]
-                    info = [labelstr, center_x, center_y, height, width, area]
-                    result.append(info)
-        try:
-            import operator
-            result.sort(key=operator.itemgetter(5), reverse=True)
-        except Exception as e:
-            logging.debug('get_toy_total_info exception:', e)
-        logging.debug("get_toy_total_info `s result  is :{}".format(result))
-        return result
 
     # def start_auto_inference(self, models):
     #     response = self.VISION.startAutoInference(models)
     #     for item in response:
-    #         logging.debug('111111',item)
+    #         print('111111',item)
     #         yield item
 
     """
 
     >>>>>>>>>>>
     >> 语音 <<
     >>>>>>>>>>>
@@ -3170,15 +2994,15 @@
         """
 
         result = ''
         response = self.AUDIO.setAudioAsr()
         data = response.data
         if response.code == 0:
             if data:
-                result = data.strip()
+                result = data
         return result
     
     def start_audio_asr_doa(self, duration = 60):
         """
         Start listening asr and direction
 
         Args:
@@ -3210,27 +3034,27 @@
             data = json.loads(result)
             if data is None:
                 # logging.debug("warning-----no data in apriltag_inference")
                 pass
             
             if 'asr' in data:
                 asr = data['asr']
-                asr_result = asr['msg'].strip()
+                asr_result = asr['msg']
             
             if 'doa' in data:
                 doa = data['doa']
                 angle = doa['angle']
-                if 45 <= angle < 135:
-                    direction = _get_translation('aisound.front')
-                elif 135 <= angle < 225:
-                    direction = _get_translation('aisound.left')
-                elif 225 <= angle < 315:
-                    direction = _get_translation('aisound.behind')
+                if angle >= 45 and angle < 135:
+                    direction = 'Front'
+                elif angle >= 135 and angle < 225:
+                    direction = 'Left'
+                elif angle >= 225 and angle < 315:
+                    direction = 'Back'
                 elif angle >= 315 or angle < 45:
-                    direction = _get_translation('aisound.right')
+                    direction = 'Right'
 
         ret = [direction, asr_result]
         return ret
 
     def start_audio_nlp(self, data, wait=False):
         """
         Listen to speech and respond with NLP
@@ -3352,21 +3176,21 @@
         result = self.AUDIO.getDirectionOfAudio()
         if result.code == 0:
             angle = result.angle
             if angle == -1:  # -1表示没有声音或者无效
                 return ''
             ret = ''
             if 45 <= angle < 135:
-                ret = _get_translation('aisound.front')
+                ret = 'Front'
             elif 135 <= angle < 225:
-                ret = _get_translation('aisound.left')
+                ret = 'Left'
             elif 225 <= angle < 315:
-                ret = _get_translation('aisound.behind')
+                ret = 'Back'
             elif angle >= 315 or angle < 45:
-                ret = _get_translation('aisound.right')
+                ret = 'Right'
             return ret
         return ''
 
     """
     
     >>>>>>>>>>>
     >> 显示屏 - Screen <<
@@ -3960,31 +3784,14 @@
 
         Returns:
             None
         """
         duty_cycle = num_normal(duty_cycle, 255, 0)
         self.GPIO.setGpioStartExportPwm(str(pin), duty_cycle)
 
-    def set_pin_pwm_duty_cycle(self, pin, frequency, duty_cycle):
-        """
-        Write an analog value to the pin by frequency and duty cycle
-
-        Args:
-            pin (int): Pin number, supported pins: 1, 2
-            frequency(int): frequency [10, 980]
-            duty_cycle(float): duty cycle [0.0, 100.0]
-
-        Returns:
-            None
-        """
-        logging.debug('set_pin_pwm_duty_cycle:{},{},{}'.format(pin, duty_cycle,frequency))
-        frequency = num_normal(frequency, 980, 10)
-        duty_cycle = num_normal(duty_cycle, 100.0, 0.0)
-        self.GPIO.setGpioStartExportPwmWithDutyCycle(str(pin), duty_cycle, frequency)
-
     def set_serial_serbaud(self, baudrate):
         """
         Set serial baud rate
 
         Args:
             baudrate (int): Baud rate, available values: 1200, 2400, 4800, 9600, 19200, 38400, 57600, 115200
 
@@ -4098,19 +3905,19 @@
         """
         Open camera
 
         Returns:
             None
         """
         if self.VISION.camera_client_id > 0:
-            logging.debug('当前摄像头已经打开,无需重复打开')
+            print('当前摄像头已经打开,无需重复打开')
             pass
         else:
             self.VISION.camera_client_id = self.VISION.openCamera()
-            logging.debug('open_camera:',self.VISION.camera_client_id)
+            print('open_camera:',self.VISION.camera_client_id)
         time.sleep(1)
 
     # def close_camera(self):
     #     """
     #     Close camera
 
     #     Returns:
```


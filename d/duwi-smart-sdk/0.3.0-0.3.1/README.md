# Comparing `tmp/duwi_smart_sdk-0.3.0.tar.gz` & `tmp/duwi_smart_sdk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smart_sdk-0.3.0.tar", last modified: Mon May 13 09:14:06 2024, max compression
+gzip compressed data, was "duwi_smart_sdk-0.3.1.tar", last modified: Tue May 14 02:40:22 2024, max compression
```

## Comparing `duwi_smart_sdk-0.3.0.tar` & `duwi_smart_sdk-0.3.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.837572 duwi_smart_sdk-0.3.0/
--rw-rw-rw-   0        0        0      900 2024-05-13 09:14:06.836596 duwi_smart_sdk-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-05-10 01:36:43.000000 duwi_smart_sdk-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.768917 duwi_smart_sdk-0.3.0/duwi_smart_sdk/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.788649 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     2404 2024-05-11 05:00:46.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/account.py
--rw-rw-rw-   0        0        0     1739 2024-05-10 00:48:21.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/control.py
--rw-rw-rw-   0        0        0     4512 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/discover.py
--rw-rw-rw-   0        0        0     2623 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/floor.py
--rw-rw-rw-   0        0        0     2651 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/house.py
--rw-rw-rw-   0        0        0     2121 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/refresh_token.py
--rw-rw-rw-   0        0        0     2731 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/room.py
--rw-rw-rw-   0        0        0     3098 2024-05-13 09:12:17.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/terminal.py
--rw-rw-rw-   0        0        0     4768 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.794828 duwi_smart_sdk-0.3.0/duwi_smart_sdk/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/const/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/const/const.py
--rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/const/status.py
--rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.795887 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.798044 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/req/__init__.py
--rw-rw-rw-   0        0        0      926 2024-05-10 01:12:19.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.809473 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/control.py
--rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/device.py
--rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/floor.py
--rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/house.py
--rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/room.py
--rw-rw-rw-   0        0        0     1146 2024-05-13 09:11:16.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/terminal.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.815911 duwi_smart_sdk-0.3.0/duwi_smart_sdk/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/util/http.py
--rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.835620 duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/
--rw-rw-rw-   0        0        0      900 2024-05-13 09:14:06.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1516 2024-05-13 09:14:06.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 09:14:06.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-13 09:14:06.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-13 09:14:06.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-13 09:14:06.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 09:14:06.837572 duwi_smart_sdk-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      936 2024-05-13 09:14:04.000000 duwi_smart_sdk-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.817864 duwi_smart_sdk-0.3.0/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.831703 duwi_smart_sdk-0.3.0/test/api/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.3.0/test/api/__init__.py
--rw-rw-rw-   0        0        0      723 2024-05-11 03:19:03.000000 duwi_smart_sdk-0.3.0/test/api/test_account.py
--rw-rw-rw-   0        0        0      948 2024-05-08 01:12:43.000000 duwi_smart_sdk-0.3.0/test/api/test_control.py
--rw-rw-rw-   0        0        0      813 2024-05-09 03:37:26.000000 duwi_smart_sdk-0.3.0/test/api/test_discover.py
--rw-rw-rw-   0        0        0      780 2024-05-09 07:45:49.000000 duwi_smart_sdk-0.3.0/test/api/test_floor.py
--rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.3.0/test/api/test_house.py
--rw-rw-rw-   0        0        0      640 2024-05-07 08:44:11.000000 duwi_smart_sdk-0.3.0/test/api/test_login.py
--rw-rw-rw-   0        0        0      724 2024-05-09 07:16:53.000000 duwi_smart_sdk-0.3.0/test/api/test_room.py
--rw-rw-rw-   0        0        0      732 2024-05-13 09:10:46.000000 duwi_smart_sdk-0.3.0/test/api/test_terminal.py
--rw-rw-rw-   0        0        0     1220 2024-05-13 01:32:37.000000 duwi_smart_sdk-0.3.0/test/api/test_ws.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.833662 duwi_smart_sdk-0.3.0/test/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/test/util/__init__.py
--rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.3.0/test/util/test_http.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:40:22.145035 duwi_smart_sdk-0.3.1/
+-rw-rw-rw-   0        0        0      900 2024-05-14 02:40:22.142105 duwi_smart_sdk-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-05-10 01:36:43.000000 duwi_smart_sdk-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 02:40:22.077367 duwi_smart_sdk-0.3.1/duwi_smart_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:40:22.095482 duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     2404 2024-05-11 05:00:46.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/account.py
+-rw-rw-rw-   0        0        0     1739 2024-05-10 00:48:21.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/control.py
+-rw-rw-rw-   0        0        0     4512 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/discover.py
+-rw-rw-rw-   0        0        0     2623 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/floor.py
+-rw-rw-rw-   0        0        0     2651 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/house.py
+-rw-rw-rw-   0        0        0     2121 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/refresh_token.py
+-rw-rw-rw-   0        0        0     2731 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/room.py
+-rw-rw-rw-   0        0        0     3098 2024-05-13 09:12:17.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/terminal.py
+-rw-rw-rw-   0        0        0     4768 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:40:22.099391 duwi_smart_sdk-0.3.1/duwi_smart_sdk/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/const/const.py
+-rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/const/status.py
+-rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:40:22.100369 duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:40:22.102322 duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/req/__init__.py
+-rw-rw-rw-   0        0        0      926 2024-05-10 01:12:19.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:40:22.112088 duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/resp/control.py
+-rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/resp/device.py
+-rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/resp/floor.py
+-rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/resp/house.py
+-rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/resp/room.py
+-rw-rw-rw-   0        0        0     1186 2024-05-14 02:39:45.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/resp/terminal.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:40:22.115993 duwi_smart_sdk-0.3.1/duwi_smart_sdk/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/util/http.py
+-rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:40:22.141129 duwi_smart_sdk-0.3.1/duwi_smart_sdk.egg-info/
+-rw-rw-rw-   0        0        0      900 2024-05-14 02:40:22.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1516 2024-05-14 02:40:22.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 02:40:22.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-14 02:40:22.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-14 02:40:22.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-14 02:40:22.000000 duwi_smart_sdk-0.3.1/duwi_smart_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 02:40:22.146012 duwi_smart_sdk-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      936 2024-05-14 02:39:45.000000 duwi_smart_sdk-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:40:22.116971 duwi_smart_sdk-0.3.1/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.1/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:40:22.135197 duwi_smart_sdk-0.3.1/test/api/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.3.1/test/api/__init__.py
+-rw-rw-rw-   0        0        0      723 2024-05-11 03:19:03.000000 duwi_smart_sdk-0.3.1/test/api/test_account.py
+-rw-rw-rw-   0        0        0      948 2024-05-08 01:12:43.000000 duwi_smart_sdk-0.3.1/test/api/test_control.py
+-rw-rw-rw-   0        0        0      813 2024-05-09 03:37:26.000000 duwi_smart_sdk-0.3.1/test/api/test_discover.py
+-rw-rw-rw-   0        0        0      780 2024-05-09 07:45:49.000000 duwi_smart_sdk-0.3.1/test/api/test_floor.py
+-rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.3.1/test/api/test_house.py
+-rw-rw-rw-   0        0        0      640 2024-05-07 08:44:11.000000 duwi_smart_sdk-0.3.1/test/api/test_login.py
+-rw-rw-rw-   0        0        0      724 2024-05-09 07:16:53.000000 duwi_smart_sdk-0.3.1/test/api/test_room.py
+-rw-rw-rw-   0        0        0      732 2024-05-13 09:10:46.000000 duwi_smart_sdk-0.3.1/test/api/test_terminal.py
+-rw-rw-rw-   0        0        0     1220 2024-05-13 01:32:37.000000 duwi_smart_sdk-0.3.1/test/api/test_ws.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:40:22.139110 duwi_smart_sdk-0.3.1/test/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.1/test/util/__init__.py
+-rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.3.1/test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.3.0/PKG-INFO` & `duwi_smart_sdk-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smart_sdk
-Version: 0.3.0
+Version: 0.3.1
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/account.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/account.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/control.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/discover.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/floor.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/house.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/refresh_token.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/room.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/terminal.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/ws.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/api/ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/const/status.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/const/status.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/const/type_map.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/req/device_control.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/auth.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/device.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/floor.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/resp/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/house.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/room.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/resp/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/terminal.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/model/resp/terminal.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 
 
-class TerminalInfo:
+class Terminal_Info:
     def __init__(self,
-                 terminalName: str,
-                 terminalSequence: str,
-                 shortCode: str,
-                 productModel: str,
-                 productLogo: str,
+                 terminal_name: str,
+                 terminal_sequence: str,
+                 short_code: str,
+                 product_model: str,
+                 product_logo: str,
                  seq: int,
-                 isGateWay: int,
-                 hostSequence: str,
-                 createTime: str,
-                 productShowModel: str,
-                 isFollowOnline: bool,
-                 isOnline: bool):
-        self.terminalName = terminalName
-        self.terminalSequence = terminalSequence
-        self.shortCode = shortCode
-        self.productModel = productModel
-        self.productLogo = productLogo
+                 is_gateway: int,
+                 host_sequence: str,
+                 create_time: str,
+                 product_show_model: str,
+                 is_follow_online: bool,
+                 is_online: bool):
+        self.terminal_name = terminal_name
+        self.terminal_sequence = terminal_sequence
+        self.short_code = short_code
+        self.product_model = product_model
+        self.product_logo = product_logo
         self.seq = seq
-        self.isGateWay = isGateWay
-        self.hostSequence = hostSequence
-        self.createTime = createTime
-        self.productShowModel = productShowModel
-        self.isFollowOnline = isFollowOnline
-        self.isOnline = isOnline
+        self.is_gateway = is_gateway
+        self.host_sequence = host_sequence
+        self.create_time = create_time
+        self.product_show_model = product_show_model
+        self.is_follow_online = is_follow_online
+        self.is_online = is_online
 
     @staticmethod
     def _parse_datetime(datetime_str: str) -> datetime.datetime:
         return datetime.datetime.strptime(datetime_str, '%Y-%m-%d %H:%M:%S')
```

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/util/http.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk/util/sign.py` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/PKG-INFO` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smart_sdk
-Version: 0.3.0
+Version: 0.3.1
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/SOURCES.txt` & `duwi_smart_sdk-0.3.1/duwi_smart_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/setup.py` & `duwi_smart_sdk-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.3.0'
+VERSION = '0.3.1'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smart_sdk",
     version=VERSION,
     author="ledger",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smart_sdk-0.3.0/test/api/test_account.py` & `duwi_smart_sdk-0.3.1/test/api/test_account.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/test/api/test_control.py` & `duwi_smart_sdk-0.3.1/test/api/test_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/test/api/test_discover.py` & `duwi_smart_sdk-0.3.1/test/api/test_discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/test/api/test_floor.py` & `duwi_smart_sdk-0.3.1/test/api/test_floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/test/api/test_house.py` & `duwi_smart_sdk-0.3.1/test/api/test_house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/test/api/test_login.py` & `duwi_smart_sdk-0.3.1/test/api/test_login.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/test/api/test_room.py` & `duwi_smart_sdk-0.3.1/test/api/test_room.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/test/api/test_terminal.py` & `duwi_smart_sdk-0.3.1/test/api/test_terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/test/api/test_ws.py` & `duwi_smart_sdk-0.3.1/test/api/test_ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.3.0/test/util/test_http.py` & `duwi_smart_sdk-0.3.1/test/util/test_http.py`

 * *Files identical despite different names*


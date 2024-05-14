# Comparing `tmp/rhubarbe-5.4.3.tar.gz` & `tmp/rhubarbe-5.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhubarbe-5.4.3.tar", last modified: Fri Feb  9 11:20:45 2024, max compression
+gzip compressed data, was "rhubarbe-5.4.4.tar", last modified: Tue May 14 17:20:16 2024, max compression
```

## Comparing `rhubarbe-5.4.3.tar` & `rhubarbe-5.4.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-02-09 11:20:45.408432 rhubarbe-5.4.3/
--rw-r--r--   0 tparment (15010) diana    (200036)     4421 2023-11-08 09:27:18.000000 rhubarbe-5.4.3/INSTALLING.md
--rw-r--r--   0 tparment (15010) diana    (200036)      289 2017-12-13 12:22:26.000000 rhubarbe-5.4.3/LICENSE
--rw-r--r--   0 tparment (15010) diana    (200036)      786 2024-02-09 11:20:45.407719 rhubarbe-5.4.3/PKG-INFO
--rw-r--r--   0 tparment (15010) diana    (200036)     9474 2019-01-25 15:17:26.000000 rhubarbe-5.4.3/README.md
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-02-09 11:20:45.339012 rhubarbe-5.4.3/rhubarbe/
--rw-r--r--   0 tparment (15010) diana    (200036)       33 2018-05-21 13:03:31.000000 rhubarbe-5.4.3/rhubarbe/__init__.py
--rwxr-xr-x   0 tparment (15010) diana    (200036)     2271 2023-01-25 15:54:56.000000 rhubarbe-5.4.3/rhubarbe/__main__.py
--rw-r--r--   0 tparment (15010) diana    (200036)     2328 2019-05-29 12:51:24.000000 rhubarbe-5.4.3/rhubarbe/action.py
--rw-r--r--   0 tparment (15010) diana    (200036)     7823 2024-02-09 11:06:46.000000 rhubarbe-5.4.3/rhubarbe/book.py
--rw-r--r--   0 tparment (15010) diana    (200036)     3874 2019-05-29 12:31:39.000000 rhubarbe-5.4.3/rhubarbe/collector.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-02-09 11:20:45.345989 rhubarbe-5.4.3/rhubarbe/config/
--rw-r--r--   0 tparment (15010) diana    (200036)      496 2015-11-27 08:14:56.000000 rhubarbe-5.4.3/rhubarbe/config/inventory-nodes.json.template
--rw-r--r--   0 tparment (15010) diana    (200036)     2361 2023-09-08 14:56:12.000000 rhubarbe-5.4.3/rhubarbe/config/inventory-pdus.yaml.template
--rw-r--r--   0 tparment (15010) diana    (200036)      215 2022-03-09 15:17:24.000000 rhubarbe-5.4.3/rhubarbe/config/inventory-phones.json.template
--rw-r--r--   0 tparment (15010) diana    (200036)     5965 2023-11-08 09:20:35.000000 rhubarbe-5.4.3/rhubarbe/config/rhubarbe.conf
--rw-r--r--   0 tparment (15010) diana    (200036)     5219 2023-09-08 14:43:09.000000 rhubarbe-5.4.3/rhubarbe/config.py
--rw-r--r--   0 tparment (15010) diana    (200036)     8748 2023-09-08 11:17:13.000000 rhubarbe-5.4.3/rhubarbe/display.py
--rwxr-xr-x   0 tparment (15010) diana    (200036)     3896 2019-05-29 13:03:11.000000 rhubarbe-5.4.3/rhubarbe/display_curses.py
--rw-r--r--   0 tparment (15010) diana    (200036)     3869 2019-06-02 18:58:38.000000 rhubarbe-5.4.3/rhubarbe/frisbee.py
--rw-r--r--   0 tparment (15010) diana    (200036)     3740 2019-06-11 16:21:59.000000 rhubarbe-5.4.3/rhubarbe/frisbeed.py
--rwxr-xr-x   0 tparment (15010) diana    (200036)     1776 2019-05-29 13:04:57.000000 rhubarbe-5.4.3/rhubarbe/guessip.py
--rw-r--r--   0 tparment (15010) diana    (200036)     3884 2019-06-02 18:42:40.000000 rhubarbe-5.4.3/rhubarbe/imageloader.py
--rw-r--r--   0 tparment (15010) diana    (200036)     4031 2019-06-01 13:12:27.000000 rhubarbe-5.4.3/rhubarbe/imagesaver.py
--rw-r--r--   0 tparment (15010) diana    (200036)    16970 2023-02-13 11:10:31.000000 rhubarbe-5.4.3/rhubarbe/imagesrepo.py
--rw-r--r--   0 tparment (15010) diana    (200036)     3322 2019-06-02 18:57:48.000000 rhubarbe-5.4.3/rhubarbe/imagezip.py
--rw-r--r--   0 tparment (15010) diana    (200036)     2436 2023-09-08 11:15:11.000000 rhubarbe-5.4.3/rhubarbe/inventorynodes.py
--rw-r--r--   0 tparment (15010) diana    (200036)    12206 2024-02-08 14:55:57.000000 rhubarbe-5.4.3/rhubarbe/inventorypdus.py
--rw-r--r--   0 tparment (15010) diana    (200036)      897 2018-05-18 13:48:11.000000 rhubarbe-5.4.3/rhubarbe/inventoryphones.py
--rw-r--r--   0 tparment (15010) diana    (200036)    17073 2024-02-07 09:19:43.000000 rhubarbe-5.4.3/rhubarbe/leases.py
--rw-r--r--   0 tparment (15010) diana    (200036)     2634 2023-11-06 17:31:54.000000 rhubarbe-5.4.3/rhubarbe/logger.py
--rwxr-xr-x   0 tparment (15010) diana    (200036)    33872 2024-02-08 15:06:00.000000 rhubarbe-5.4.3/rhubarbe/main.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-02-09 11:20:45.350743 rhubarbe-5.4.3/rhubarbe/monitor/
--rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-01-23 13:07:02.000000 rhubarbe-5.4.3/rhubarbe/monitor/__init__.py
--rw-r--r--   0 tparment (15010) diana    (200036)    11144 2023-01-16 16:34:53.000000 rhubarbe-5.4.3/rhubarbe/monitor/accountsmanager.py
--rw-r--r--   0 tparment (15010) diana    (200036)     2400 2022-12-10 18:06:07.000000 rhubarbe-5.4.3/rhubarbe/monitor/leases.py
--rw-r--r--   0 tparment (15010) diana    (200036)     1158 2019-01-29 13:02:29.000000 rhubarbe-5.4.3/rhubarbe/monitor/loop.py
--rw-r--r--   0 tparment (15010) diana    (200036)    12672 2023-01-28 10:30:12.000000 rhubarbe-5.4.3/rhubarbe/monitor/nodes.py
--rw-r--r--   0 tparment (15010) diana    (200036)     2465 2023-02-09 13:25:08.000000 rhubarbe-5.4.3/rhubarbe/monitor/pdus.py
--rw-r--r--   0 tparment (15010) diana    (200036)     4905 2023-02-09 13:24:33.000000 rhubarbe-5.4.3/rhubarbe/monitor/phones.py
--rw-r--r--   0 tparment (15010) diana    (200036)     3381 2022-03-10 16:07:35.000000 rhubarbe-5.4.3/rhubarbe/monitor/reconnectable.py
--rw-r--r--   0 tparment (15010) diana    (200036)    10023 2023-09-08 11:17:13.000000 rhubarbe-5.4.3/rhubarbe/node.py
--rw-r--r--   0 tparment (15010) diana    (200036)     2801 2024-02-07 08:56:17.000000 rhubarbe-5.4.3/rhubarbe/plcapiproxy.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-02-09 11:20:45.405558 rhubarbe-5.4.3/rhubarbe/scripts/
--rw-r--r--   0 tparment (15010) diana    (200036)    27215 2023-02-03 13:48:00.000000 rhubarbe-5.4.3/rhubarbe/scripts/ALL.txt
--rw-r--r--   0 tparment (15010) diana    (200036)    46017 2023-02-03 14:23:01.000000 rhubarbe-5.4.3/rhubarbe/scripts/ALL2.txt
--rw-r--r--   0 tparment (15010) diana    (200036)    87226 2019-07-12 13:18:58.000000 rhubarbe-5.4.3/rhubarbe/scripts/EATON-EPDU-MIB.txt
--rw-r--r--   0 tparment (15010) diana    (200036)    20264 2023-02-03 08:41:25.000000 rhubarbe-5.4.3/rhubarbe/scripts/EATON-EPDU-MIB.zip
--rw-r--r--   0 tparment (15010) diana    (200036)     7173 2019-03-14 11:19:36.000000 rhubarbe-5.4.3/rhubarbe/scripts/EATON-OIDS.txt
--rw-r--r--   0 tparment (15010) diana    (200036)    48983 2019-03-14 11:19:36.000000 rhubarbe-5.4.3/rhubarbe/scripts/EATON-SENSOR-MIB.txt
--rw-r--r--   0 tparment (15010) diana    (200036)   541651 2023-02-05 15:55:02.000000 rhubarbe-5.4.3/rhubarbe/scripts/Eaton ePDU G3 - Installation and Connectivity Quick Start.pdf
--rw-r--r--   0 tparment (15010) diana    (200036) 12884071 2023-02-03 08:37:45.000000 rhubarbe-5.4.3/rhubarbe/scripts/Eaton_ePDU_G3_Operations_Manual.133.pdf
--rw-r--r--   0 tparment (15010) diana    (200036)     1703 2023-02-03 16:12:19.000000 rhubarbe-5.4.3/rhubarbe/scripts/NOTES.md
--rwxr-xr-x   0 tparment (15010) diana    (200036)     8467 2023-09-13 16:04:41.000000 rhubarbe-5.4.3/rhubarbe/scripts/eaton
--rwxr-xr-x   0 tparment (15010) diana    (200036)     3887 2023-09-13 16:12:16.000000 rhubarbe-5.4.3/rhubarbe/scripts/relay
--rw-r--r--   0 tparment (15010) diana    (200036)     6059 2023-09-11 13:31:26.000000 rhubarbe-5.4.3/rhubarbe/scripts/relay-TT
--rw-r--r--   0 tparment (15010) diana    (200036)        0 2023-02-01 12:52:10.000000 rhubarbe-5.4.3/rhubarbe/scripts/rhubarbe.log
--rw-r--r--   0 tparment (15010) diana    (200036)      812 2023-01-24 08:51:49.000000 rhubarbe-5.4.3/rhubarbe/scripts/test-ping.py
--rw-r--r--   0 tparment (15010) diana    (200036)     4895 2019-06-01 10:02:17.000000 rhubarbe-5.4.3/rhubarbe/selector.py
--rw-r--r--   0 tparment (15010) diana    (200036)      473 2018-05-18 13:48:11.000000 rhubarbe-5.4.3/rhubarbe/singleton.py
--rwxr-xr-x   0 tparment (15010) diana    (200036)     6219 2019-06-01 10:04:25.000000 rhubarbe-5.4.3/rhubarbe/ssh.py
--rw-r--r--   0 tparment (15010) diana    (200036)     5372 2022-12-02 13:59:56.000000 rhubarbe-5.4.3/rhubarbe/telnet.py
--rw-r--r--   0 tparment (15010) diana    (200036)       47 2024-02-09 11:20:17.000000 rhubarbe-5.4.3/rhubarbe/version.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-02-09 11:20:45.406466 rhubarbe-5.4.3/rhubarbe.egg-info/
--rw-r--r--   0 tparment (15010) diana    (200036)      786 2024-02-09 11:20:45.000000 rhubarbe-5.4.3/rhubarbe.egg-info/PKG-INFO
--rw-r--r--   0 tparment (15010) diana    (200036)     1711 2024-02-09 11:20:45.000000 rhubarbe-5.4.3/rhubarbe.egg-info/SOURCES.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        1 2024-02-09 11:20:45.000000 rhubarbe-5.4.3/rhubarbe.egg-info/dependency_links.txt
--rw-r--r--   0 tparment (15010) diana    (200036)     1181 2024-02-09 11:20:45.000000 rhubarbe-5.4.3/rhubarbe.egg-info/entry_points.txt
--rw-r--r--   0 tparment (15010) diana    (200036)       84 2024-02-09 11:20:45.000000 rhubarbe-5.4.3/rhubarbe.egg-info/requires.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        9 2024-02-09 11:20:45.000000 rhubarbe-5.4.3/rhubarbe.egg-info/top_level.txt
--rw-r--r--   0 tparment (15010) diana    (200036)       38 2024-02-09 11:20:45.408562 rhubarbe-5.4.3/setup.cfg
--rwxr-xr-x   0 tparment (15010) diana    (200036)     2587 2023-03-04 10:18:37.000000 rhubarbe-5.4.3/setup.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-14 17:20:16.170771 rhubarbe-5.4.4/
+-rw-r--r--   0 tparment (15010) diana    (200036)     4421 2023-11-08 09:27:18.000000 rhubarbe-5.4.4/INSTALLING.md
+-rw-r--r--   0 tparment (15010) diana    (200036)      289 2017-12-13 12:22:26.000000 rhubarbe-5.4.4/LICENSE
+-rw-r--r--   0 tparment (15010) diana    (200036)      786 2024-05-14 17:20:16.169879 rhubarbe-5.4.4/PKG-INFO
+-rw-r--r--   0 tparment (15010) diana    (200036)     9474 2019-01-25 15:17:26.000000 rhubarbe-5.4.4/README.md
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-14 17:20:16.083558 rhubarbe-5.4.4/rhubarbe/
+-rw-r--r--   0 tparment (15010) diana    (200036)       33 2018-05-21 13:03:31.000000 rhubarbe-5.4.4/rhubarbe/__init__.py
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     2271 2023-01-25 15:54:56.000000 rhubarbe-5.4.4/rhubarbe/__main__.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     2328 2019-05-29 12:51:24.000000 rhubarbe-5.4.4/rhubarbe/action.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     7978 2024-05-14 17:15:44.000000 rhubarbe-5.4.4/rhubarbe/book.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     3874 2019-05-29 12:31:39.000000 rhubarbe-5.4.4/rhubarbe/collector.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-14 17:20:16.092441 rhubarbe-5.4.4/rhubarbe/config/
+-rw-r--r--   0 tparment (15010) diana    (200036)      496 2015-11-27 08:14:56.000000 rhubarbe-5.4.4/rhubarbe/config/inventory-nodes.json.template
+-rw-r--r--   0 tparment (15010) diana    (200036)     2361 2023-09-08 14:56:12.000000 rhubarbe-5.4.4/rhubarbe/config/inventory-pdus.yaml.template
+-rw-r--r--   0 tparment (15010) diana    (200036)      215 2022-03-09 15:17:24.000000 rhubarbe-5.4.4/rhubarbe/config/inventory-phones.json.template
+-rw-r--r--   0 tparment (15010) diana    (200036)     5965 2023-11-08 09:20:35.000000 rhubarbe-5.4.4/rhubarbe/config/rhubarbe.conf
+-rw-r--r--   0 tparment (15010) diana    (200036)     5219 2023-09-08 14:43:09.000000 rhubarbe-5.4.4/rhubarbe/config.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     8748 2023-09-08 11:17:13.000000 rhubarbe-5.4.4/rhubarbe/display.py
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     3896 2019-05-29 13:03:11.000000 rhubarbe-5.4.4/rhubarbe/display_curses.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     3869 2019-06-02 18:58:38.000000 rhubarbe-5.4.4/rhubarbe/frisbee.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     3740 2019-06-11 16:21:59.000000 rhubarbe-5.4.4/rhubarbe/frisbeed.py
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     1776 2019-05-29 13:04:57.000000 rhubarbe-5.4.4/rhubarbe/guessip.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     3884 2019-06-02 18:42:40.000000 rhubarbe-5.4.4/rhubarbe/imageloader.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     4031 2019-06-01 13:12:27.000000 rhubarbe-5.4.4/rhubarbe/imagesaver.py
+-rw-r--r--   0 tparment (15010) diana    (200036)    16970 2023-02-13 11:10:31.000000 rhubarbe-5.4.4/rhubarbe/imagesrepo.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     3322 2019-06-02 18:57:48.000000 rhubarbe-5.4.4/rhubarbe/imagezip.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     2436 2023-09-08 11:15:11.000000 rhubarbe-5.4.4/rhubarbe/inventorynodes.py
+-rw-r--r--   0 tparment (15010) diana    (200036)    12206 2024-02-08 14:55:57.000000 rhubarbe-5.4.4/rhubarbe/inventorypdus.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      897 2018-05-18 13:48:11.000000 rhubarbe-5.4.4/rhubarbe/inventoryphones.py
+-rw-r--r--   0 tparment (15010) diana    (200036)    17073 2024-02-07 09:19:43.000000 rhubarbe-5.4.4/rhubarbe/leases.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     2634 2023-11-06 17:31:54.000000 rhubarbe-5.4.4/rhubarbe/logger.py
+-rwxr-xr-x   0 tparment (15010) diana    (200036)    33872 2024-02-08 15:06:00.000000 rhubarbe-5.4.4/rhubarbe/main.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-14 17:20:16.112004 rhubarbe-5.4.4/rhubarbe/monitor/
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-01-23 13:07:02.000000 rhubarbe-5.4.4/rhubarbe/monitor/__init__.py
+-rw-r--r--   0 tparment (15010) diana    (200036)    11144 2023-01-16 16:34:53.000000 rhubarbe-5.4.4/rhubarbe/monitor/accountsmanager.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     2400 2022-12-10 18:06:07.000000 rhubarbe-5.4.4/rhubarbe/monitor/leases.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     1158 2019-01-29 13:02:29.000000 rhubarbe-5.4.4/rhubarbe/monitor/loop.py
+-rw-r--r--   0 tparment (15010) diana    (200036)    12672 2023-01-28 10:30:12.000000 rhubarbe-5.4.4/rhubarbe/monitor/nodes.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     2465 2023-02-09 13:25:08.000000 rhubarbe-5.4.4/rhubarbe/monitor/pdus.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     4905 2023-02-09 13:24:33.000000 rhubarbe-5.4.4/rhubarbe/monitor/phones.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     3381 2022-03-10 16:07:35.000000 rhubarbe-5.4.4/rhubarbe/monitor/reconnectable.py
+-rw-r--r--   0 tparment (15010) diana    (200036)    10023 2023-09-08 11:17:13.000000 rhubarbe-5.4.4/rhubarbe/node.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     2801 2024-02-07 08:56:17.000000 rhubarbe-5.4.4/rhubarbe/plcapiproxy.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-14 17:20:16.168484 rhubarbe-5.4.4/rhubarbe/scripts/
+-rw-r--r--   0 tparment (15010) diana    (200036)    27215 2023-02-03 13:48:00.000000 rhubarbe-5.4.4/rhubarbe/scripts/ALL.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)    46017 2023-02-03 14:23:01.000000 rhubarbe-5.4.4/rhubarbe/scripts/ALL2.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)    87226 2019-07-12 13:18:58.000000 rhubarbe-5.4.4/rhubarbe/scripts/EATON-EPDU-MIB.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)    20264 2023-02-03 08:41:25.000000 rhubarbe-5.4.4/rhubarbe/scripts/EATON-EPDU-MIB.zip
+-rw-r--r--   0 tparment (15010) diana    (200036)     7173 2019-03-14 11:19:36.000000 rhubarbe-5.4.4/rhubarbe/scripts/EATON-OIDS.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)    48983 2019-03-14 11:19:36.000000 rhubarbe-5.4.4/rhubarbe/scripts/EATON-SENSOR-MIB.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)   541651 2023-02-05 15:55:02.000000 rhubarbe-5.4.4/rhubarbe/scripts/Eaton ePDU G3 - Installation and Connectivity Quick Start.pdf
+-rw-r--r--   0 tparment (15010) diana    (200036) 12884071 2023-02-03 08:37:45.000000 rhubarbe-5.4.4/rhubarbe/scripts/Eaton_ePDU_G3_Operations_Manual.133.pdf
+-rw-r--r--   0 tparment (15010) diana    (200036)     1703 2023-02-03 16:12:19.000000 rhubarbe-5.4.4/rhubarbe/scripts/NOTES.md
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     8467 2023-09-13 16:04:41.000000 rhubarbe-5.4.4/rhubarbe/scripts/eaton
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     3887 2023-09-13 16:12:16.000000 rhubarbe-5.4.4/rhubarbe/scripts/relay
+-rw-r--r--   0 tparment (15010) diana    (200036)     6059 2023-09-11 13:31:26.000000 rhubarbe-5.4.4/rhubarbe/scripts/relay-TT
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2023-02-01 12:52:10.000000 rhubarbe-5.4.4/rhubarbe/scripts/rhubarbe.log
+-rw-r--r--   0 tparment (15010) diana    (200036)      812 2023-01-24 08:51:49.000000 rhubarbe-5.4.4/rhubarbe/scripts/test-ping.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     4895 2019-06-01 10:02:17.000000 rhubarbe-5.4.4/rhubarbe/selector.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      473 2018-05-18 13:48:11.000000 rhubarbe-5.4.4/rhubarbe/singleton.py
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     6219 2019-06-01 10:04:25.000000 rhubarbe-5.4.4/rhubarbe/ssh.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     5372 2022-12-02 13:59:56.000000 rhubarbe-5.4.4/rhubarbe/telnet.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       47 2024-05-14 17:19:24.000000 rhubarbe-5.4.4/rhubarbe/version.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-14 17:20:16.169206 rhubarbe-5.4.4/rhubarbe.egg-info/
+-rw-r--r--   0 tparment (15010) diana    (200036)      786 2024-05-14 17:20:15.000000 rhubarbe-5.4.4/rhubarbe.egg-info/PKG-INFO
+-rw-r--r--   0 tparment (15010) diana    (200036)     1711 2024-05-14 17:20:16.000000 rhubarbe-5.4.4/rhubarbe.egg-info/SOURCES.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        1 2024-05-14 17:20:15.000000 rhubarbe-5.4.4/rhubarbe.egg-info/dependency_links.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)     1181 2024-05-14 17:20:15.000000 rhubarbe-5.4.4/rhubarbe.egg-info/entry_points.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)       84 2024-05-14 17:20:15.000000 rhubarbe-5.4.4/rhubarbe.egg-info/requires.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        9 2024-05-14 17:20:15.000000 rhubarbe-5.4.4/rhubarbe.egg-info/top_level.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)       38 2024-05-14 17:20:16.170956 rhubarbe-5.4.4/setup.cfg
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     2587 2023-03-04 10:18:37.000000 rhubarbe-5.4.4/setup.py
```

### Comparing `rhubarbe-5.4.3/INSTALLING.md` & `rhubarbe-5.4.4/INSTALLING.md`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/PKG-INFO` & `rhubarbe-5.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhubarbe
-Version: 5.4.3
+Version: 5.4.4
 Summary: Testbed Management Framework for R2Lab
 Author: Thierry Parmentelat
 Author-email: thierry.parmentelat@inria.fr
 License: CC BY-SA 4.0
 Project-URL: source, https://github.com/fit-r2lab/rhubarbe/
 Keywords: R2lab,networking testbed
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rhubarbe-5.4.3/README.md` & `rhubarbe-5.4.4/README.md`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/__main__.py` & `rhubarbe-5.4.4/rhubarbe/__main__.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/action.py` & `rhubarbe-5.4.4/rhubarbe/action.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/book.py` & `rhubarbe-5.4.4/rhubarbe/book.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,19 @@
                 local = DateTime.strptime(date, format)
                 break
             except ValueError:
                 pass
         if local is None:
             raise ValueError(f"cannot parse date {date}")
         epoch = int((local - DateTime(1970, 1, 1)).total_seconds())
-        return epoch + time.timezone
+
+        # translate to UTC
+        is_dst = time.daylight and time.localtime().tm_isdst > 0
+        utc_offset = (time.altzone if is_dst else time.timezone)
+        return epoch + utc_offset
 
     def date_to_string(self, date):
         """
         return a date in the format expected by the plcapi
         """
         return DateTime.fromtimestamp(date).strftime('%Y-%m-%dT%H:%M')
```

### Comparing `rhubarbe-5.4.3/rhubarbe/collector.py` & `rhubarbe-5.4.4/rhubarbe/collector.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/config/inventory-pdus.yaml.template` & `rhubarbe-5.4.4/rhubarbe/config/inventory-pdus.yaml.template`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/config/rhubarbe.conf` & `rhubarbe-5.4.4/rhubarbe/config/rhubarbe.conf`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/config.py` & `rhubarbe-5.4.4/rhubarbe/config.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/display.py` & `rhubarbe-5.4.4/rhubarbe/display.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/display_curses.py` & `rhubarbe-5.4.4/rhubarbe/display_curses.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/frisbee.py` & `rhubarbe-5.4.4/rhubarbe/frisbee.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/frisbeed.py` & `rhubarbe-5.4.4/rhubarbe/frisbeed.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/guessip.py` & `rhubarbe-5.4.4/rhubarbe/guessip.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/imageloader.py` & `rhubarbe-5.4.4/rhubarbe/imageloader.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/imagesaver.py` & `rhubarbe-5.4.4/rhubarbe/imagesaver.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/imagesrepo.py` & `rhubarbe-5.4.4/rhubarbe/imagesrepo.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/imagezip.py` & `rhubarbe-5.4.4/rhubarbe/imagezip.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/inventorynodes.py` & `rhubarbe-5.4.4/rhubarbe/inventorynodes.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/inventorypdus.py` & `rhubarbe-5.4.4/rhubarbe/inventorypdus.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/inventoryphones.py` & `rhubarbe-5.4.4/rhubarbe/inventoryphones.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/leases.py` & `rhubarbe-5.4.4/rhubarbe/leases.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/logger.py` & `rhubarbe-5.4.4/rhubarbe/logger.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/main.py` & `rhubarbe-5.4.4/rhubarbe/main.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/monitor/accountsmanager.py` & `rhubarbe-5.4.4/rhubarbe/monitor/accountsmanager.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/monitor/leases.py` & `rhubarbe-5.4.4/rhubarbe/monitor/leases.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/monitor/loop.py` & `rhubarbe-5.4.4/rhubarbe/monitor/loop.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/monitor/nodes.py` & `rhubarbe-5.4.4/rhubarbe/monitor/nodes.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/monitor/pdus.py` & `rhubarbe-5.4.4/rhubarbe/monitor/pdus.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/monitor/phones.py` & `rhubarbe-5.4.4/rhubarbe/monitor/phones.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/monitor/reconnectable.py` & `rhubarbe-5.4.4/rhubarbe/monitor/reconnectable.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/node.py` & `rhubarbe-5.4.4/rhubarbe/node.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/plcapiproxy.py` & `rhubarbe-5.4.4/rhubarbe/plcapiproxy.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/scripts/ALL.txt` & `rhubarbe-5.4.4/rhubarbe/scripts/ALL.txt`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/scripts/ALL2.txt` & `rhubarbe-5.4.4/rhubarbe/scripts/ALL2.txt`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/scripts/EATON-EPDU-MIB.txt` & `rhubarbe-5.4.4/rhubarbe/scripts/EATON-EPDU-MIB.txt`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/scripts/EATON-EPDU-MIB.zip` & `rhubarbe-5.4.4/rhubarbe/scripts/EATON-EPDU-MIB.zip`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/scripts/EATON-OIDS.txt` & `rhubarbe-5.4.4/rhubarbe/scripts/EATON-OIDS.txt`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/scripts/EATON-SENSOR-MIB.txt` & `rhubarbe-5.4.4/rhubarbe/scripts/EATON-SENSOR-MIB.txt`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/scripts/Eaton ePDU G3 - Installation and Connectivity Quick Start.pdf` & `rhubarbe-5.4.4/rhubarbe/scripts/Eaton ePDU G3 - Installation and Connectivity Quick Start.pdf`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/scripts/Eaton_ePDU_G3_Operations_Manual.133.pdf` & `rhubarbe-5.4.4/rhubarbe/scripts/Eaton_ePDU_G3_Operations_Manual.133.pdf`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/scripts/NOTES.md` & `rhubarbe-5.4.4/rhubarbe/scripts/NOTES.md`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/scripts/eaton` & `rhubarbe-5.4.4/rhubarbe/scripts/eaton`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/scripts/relay` & `rhubarbe-5.4.4/rhubarbe/scripts/relay`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/scripts/relay-TT` & `rhubarbe-5.4.4/rhubarbe/scripts/relay-TT`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/scripts/test-ping.py` & `rhubarbe-5.4.4/rhubarbe/scripts/test-ping.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/selector.py` & `rhubarbe-5.4.4/rhubarbe/selector.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/ssh.py` & `rhubarbe-5.4.4/rhubarbe/ssh.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe/telnet.py` & `rhubarbe-5.4.4/rhubarbe/telnet.py`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe.egg-info/PKG-INFO` & `rhubarbe-5.4.4/rhubarbe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhubarbe
-Version: 5.4.3
+Version: 5.4.4
 Summary: Testbed Management Framework for R2Lab
 Author: Thierry Parmentelat
 Author-email: thierry.parmentelat@inria.fr
 License: CC BY-SA 4.0
 Project-URL: source, https://github.com/fit-r2lab/rhubarbe/
 Keywords: R2lab,networking testbed
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rhubarbe-5.4.3/rhubarbe.egg-info/SOURCES.txt` & `rhubarbe-5.4.4/rhubarbe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/rhubarbe.egg-info/entry_points.txt` & `rhubarbe-5.4.4/rhubarbe.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `rhubarbe-5.4.3/setup.py` & `rhubarbe-5.4.4/setup.py`

 * *Files identical despite different names*


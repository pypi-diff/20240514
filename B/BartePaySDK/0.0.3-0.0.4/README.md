# Comparing `tmp/BartePaySDK-0.0.3.tar.gz` & `tmp/BartePaySDK-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BartePaySDK-0.0.3.tar", last modified: Tue May 14 13:20:54 2024, max compression
+gzip compressed data, was "BartePaySDK-0.0.4.tar", last modified: Tue May 14 13:31:50 2024, max compression
```

## Comparing `BartePaySDK-0.0.3.tar` & `BartePaySDK-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:20:54.744295 BartePaySDK-0.0.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:20:54.744295 BartePaySDK-0.0.3/BartePaySDK.egg-info/
--rw-r--r--   0 root         (0) root         (0)      194 2024-05-14 13:20:54.000000 BartePaySDK-0.0.3/BartePaySDK.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2024-05-14 13:20:54.000000 BartePaySDK-0.0.3/BartePaySDK.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 13:20:54.000000 BartePaySDK-0.0.3/BartePaySDK.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-14 13:20:54.000000 BartePaySDK-0.0.3/BartePaySDK.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 13:20:54.000000 BartePaySDK-0.0.3/BartePaySDK.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      194 2024-05-14 13:20:54.744295 BartePaySDK-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 13:20:54.744295 BartePaySDK-0.0.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      363 2024-05-14 13:20:40.000000 BartePaySDK-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:31:50.755245 BartePaySDK-0.0.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:31:50.755245 BartePaySDK-0.0.4/BartePaySDK.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      215 2024-05-14 13:31:50.000000 BartePaySDK-0.0.4/BartePaySDK.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2024-05-14 13:31:50.000000 BartePaySDK-0.0.4/BartePaySDK.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 13:31:50.000000 BartePaySDK-0.0.4/BartePaySDK.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-14 13:31:50.000000 BartePaySDK-0.0.4/BartePaySDK.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 13:31:50.000000 BartePaySDK-0.0.4/BartePaySDK.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      215 2024-05-14 13:31:50.755245 BartePaySDK-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 13:31:50.755245 BartePaySDK-0.0.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      384 2024-05-14 13:31:37.000000 BartePaySDK-0.0.4/setup.py
```


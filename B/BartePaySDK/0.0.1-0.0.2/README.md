# Comparing `tmp/BartePaySDK-0.0.1.tar.gz` & `tmp/BartePaySDK-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BartePaySDK-0.0.1.tar", last modified: Tue May 14 12:48:27 2024, max compression
+gzip compressed data, was "BartePaySDK-0.0.2.tar", last modified: Tue May 14 13:16:52 2024, max compression
```

## Comparing `BartePaySDK-0.0.1.tar` & `BartePaySDK-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:48:27.715457 BartePaySDK-0.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:48:27.715457 BartePaySDK-0.0.1/BartePaySDK.egg-info/
--rw-r--r--   0 root         (0) root         (0)      194 2024-05-14 12:48:27.000000 BartePaySDK-0.0.1/BartePaySDK.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2024-05-14 12:48:27.000000 BartePaySDK-0.0.1/BartePaySDK.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 12:48:27.000000 BartePaySDK-0.0.1/BartePaySDK.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-14 12:48:27.000000 BartePaySDK-0.0.1/BartePaySDK.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 12:48:27.000000 BartePaySDK-0.0.1/BartePaySDK.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      194 2024-05-14 12:48:27.715457 BartePaySDK-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 12:48:27.715457 BartePaySDK-0.0.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      363 2024-05-14 12:41:37.000000 BartePaySDK-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:16:52.296065 BartePaySDK-0.0.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:16:52.296065 BartePaySDK-0.0.2/BartePaySDK.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      194 2024-05-14 13:16:52.000000 BartePaySDK-0.0.2/BartePaySDK.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2024-05-14 13:16:52.000000 BartePaySDK-0.0.2/BartePaySDK.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 13:16:52.000000 BartePaySDK-0.0.2/BartePaySDK.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-14 13:16:52.000000 BartePaySDK-0.0.2/BartePaySDK.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 13:16:52.000000 BartePaySDK-0.0.2/BartePaySDK.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      194 2024-05-14 13:16:52.296065 BartePaySDK-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 13:16:52.296065 BartePaySDK-0.0.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      363 2024-05-14 13:16:36.000000 BartePaySDK-0.0.2/setup.py
```


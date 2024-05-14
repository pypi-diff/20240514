# Comparing `tmp/BartePaySDK-0.0.6.tar.gz` & `tmp/BartePaySDK-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BartePaySDK-0.0.6.tar", last modified: Tue May 14 17:52:12 2024, max compression
+gzip compressed data, was "BartePaySDK-0.0.7.tar", last modified: Tue May 14 17:57:14 2024, max compression
```

## Comparing `BartePaySDK-0.0.6.tar` & `BartePaySDK-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 17:52:12.418596 BartePaySDK-0.0.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 17:52:12.418596 BartePaySDK-0.0.6/BartePaySDK.egg-info/
--rw-r--r--   0 root         (0) root         (0)      215 2024-05-14 17:52:12.000000 BartePaySDK-0.0.6/BartePaySDK.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2024-05-14 17:52:12.000000 BartePaySDK-0.0.6/BartePaySDK.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 17:52:12.000000 BartePaySDK-0.0.6/BartePaySDK.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-14 17:52:12.000000 BartePaySDK-0.0.6/BartePaySDK.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 17:52:12.000000 BartePaySDK-0.0.6/BartePaySDK.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      215 2024-05-14 17:52:12.418596 BartePaySDK-0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 17:52:12.418596 BartePaySDK-0.0.6/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      384 2024-05-14 17:51:58.000000 BartePaySDK-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 17:57:14.309171 BartePaySDK-0.0.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 17:57:14.309171 BartePaySDK-0.0.7/BartePaySDK.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      215 2024-05-14 17:57:14.000000 BartePaySDK-0.0.7/BartePaySDK.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2024-05-14 17:57:14.000000 BartePaySDK-0.0.7/BartePaySDK.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 17:57:14.000000 BartePaySDK-0.0.7/BartePaySDK.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-14 17:57:14.000000 BartePaySDK-0.0.7/BartePaySDK.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 17:57:14.000000 BartePaySDK-0.0.7/BartePaySDK.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      215 2024-05-14 17:57:14.309171 BartePaySDK-0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 17:57:14.309171 BartePaySDK-0.0.7/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      384 2024-05-14 17:57:01.000000 BartePaySDK-0.0.7/setup.py
```


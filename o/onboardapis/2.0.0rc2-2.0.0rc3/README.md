# Comparing `tmp/onboardapis-2.0.0rc2.tar.gz` & `tmp/onboardapis-2.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardapis-2.0.0rc2.tar", last modified: Thu May  2 19:59:52 2024, max compression
+gzip compressed data, was "onboardapis-2.0.0rc3.tar", last modified: Tue May 14 19:06:49 2024, max compression
```

## Comparing `onboardapis-2.0.0rc2.tar` & `onboardapis-2.0.0rc3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.266661 onboardapis-2.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-05-02 19:59:52.266661 onboardapis-2.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/bus/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/other/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/other/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/plane/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/plane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/ship/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/ship/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/train/
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/train/at/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/at/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/train/at/obb/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/at/obb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/at/obb/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/at/obb/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/train/de/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/train/de/bth/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/bth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/de/db/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/db/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/db/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/db/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/de/flix/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/flix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/flix/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/flix/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/de/me/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/me/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/me/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/me/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/de/tdh/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/tdh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/tdh/apis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/fr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/fr/sncf/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/fr/sncf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/fr/sncf/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/fr/sncf/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/it/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/it/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/it/ti/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/it/ti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/it/ti/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/it/ti/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/third_party/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/third_party/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/third_party/icomera/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/third_party/icomera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/third_party/icomera/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/third_party/icomera/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.266661 onboardapis-2.0.0rc2/onboardapis/train/third_party/unwired/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/third_party/unwired/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/third_party/unwired/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/third_party/unwired/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/third_party/unwired/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.266661 onboardapis-2.0.0rc2/onboardapis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-05-02 19:59:52.000000 onboardapis-2.0.0rc2/onboardapis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-02 19:59:52.000000 onboardapis-2.0.0rc2/onboardapis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:59:52.000000 onboardapis-2.0.0rc2/onboardapis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-02 19:59:52.000000 onboardapis-2.0.0rc2/onboardapis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 19:59:52.000000 onboardapis-2.0.0rc2/onboardapis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:59:52.266661 onboardapis-2.0.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.219254 onboardapis-2.0.0rc3/onboardapis/
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.219254 onboardapis-2.0.0rc3/onboardapis/bus/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.219254 onboardapis-2.0.0rc3/onboardapis/other/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/other/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/plane/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/plane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/ship/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/ship/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/at/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/at/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/at/obb/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/at/obb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/at/obb/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/at/obb/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/de/bth/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/bth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/de/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/db/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/db/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/db/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/de/flix/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/flix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/flix/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/flix/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/de/me/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/me/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/me/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/me/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/de/tdh/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/tdh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/tdh/apis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/fr/sncf/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/fr/sncf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/fr/sncf/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/fr/sncf/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/onboardapis/train/it/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/it/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/onboardapis/train/it/ti/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/it/ti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/it/ti/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/it/ti/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/onboardapis/train/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/third_party/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/onboardapis/train/third_party/icomera/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/third_party/icomera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/third_party/icomera/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/third_party/icomera/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/onboardapis/train/third_party/unwired/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/third_party/unwired/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/third_party/unwired/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/third_party/unwired/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/third_party/unwired/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/onboardapis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-05-14 19:06:49.000000 onboardapis-2.0.0rc3/onboardapis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-14 19:06:49.000000 onboardapis-2.0.0rc3/onboardapis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:06:49.000000 onboardapis-2.0.0rc3/onboardapis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-14 19:06:49.000000 onboardapis-2.0.0rc3/onboardapis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 19:06:49.000000 onboardapis-2.0.0rc3/onboardapis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/setup.cfg
```

### Comparing `onboardapis-2.0.0rc2/LICENSE` & `onboardapis-2.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/PKG-INFO` & `onboardapis-2.0.0rc3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: onboardapis
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: A pure Python wrapper for the on-board APIs of many different transportation providers.
 Author-email: Felix Zenk <felix.zenk@web.de>
 License: MIT
 Project-URL: Homepage, https://felix-zenk.github.io/onboardapis
 Project-URL: Documentation, https://felix-zenk.github.io/onboardapis/
 Project-URL: Repository, https://github.com/felix-zenk/onboardapis
 Project-URL: Issues, https://github.com/felix-zenk/onboardapis/issues
-Keywords: api,train,public-transport
+Keywords: public-transport,train,api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -25,28 +25,33 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: geopy>=2.3.0
 Requires-Dist: gql[all]>=3.5.0
 Requires-Dist: restfly>=1.4.7
 Requires-Dist: requests>=2.31.0
 Requires-Dist: beautifulsoup4>=4.12.2
-Requires-Dist: typing-extensions>=4.9.0
+Requires-Dist: deprecation>=2.1.0
 Provides-Extra: dev
 Requires-Dist: flake8>=7.0.0; extra == "dev"
+Requires-Dist: Flake8-pyproject>=1.2.3; extra == "dev"
 Requires-Dist: pdoc>=14.4.0; extra == "dev"
 Requires-Dist: build>=1.2.1; extra == "dev"
+Requires-Dist: pytest>=8.2.0; extra == "dev"
+Requires-Dist: pytest-cov>=5.0.0; extra == "dev"
+Requires-Dist: testcontainers>=3.7.1; extra == "dev"
+Requires-Dist: wiremock[testing]>=2.6.1; extra == "dev"
 
 onboardapis
 ===
 
 [![Python versions](https://img.shields.io/pypi/pyversions/onboardapis)](https://pypi.org/project/onboardapis)
 [![PyPI version](https://badge.fury.io/py/onboardapis.svg)](https://pypi.org/project/onboardapis)
+[![License](https://img.shields.io/github/license/felix-zenk/onboardapis)](https://github.com/felix-zenk/onboardapis/blob/main/LICENSE)  
 [![Build package](https://github.com/felix-zenk/onboardapis/actions/workflows/build.yml/badge.svg)](https://github.com/felix-zenk/onboardapis/actions/workflows/build.yml)
 [![Deploy documentation](https://github.com/felix-zenk/onboardapis/actions/workflows/docs.yml/badge.svg)](https://github.com/felix-zenk/onboardapis/actions/workflows/docs.yml)
-[![License](https://img.shields.io/github/license/felix-zenk/onboardapis)](https://github.com/felix-zenk/onboardapis/blob/main/LICENSE)
 
 > **Warning**: Version `2.0.0` introduces breaking changes! Existing code will definitely not work anymore.
 
 ## Description
 
 onboardapis allows you to interact with different on-board APIs.
 You can connect to the Wi-Fi of a supported transportation provider
@@ -63,42 +68,36 @@
 from [PyPI](https://pypi.org/project/onboardapis)
 using [pip](https://pip.pypa.io/en/stable/installation/):
 
 ```shell
 $ python -m pip install onboardapis
 ```
 
-![Version](https://img.shields.io/pypi/v/onboardapis?label=%20)
+[![Version](https://img.shields.io/pypi/v/onboardapis?label=%20)](https://pypi.org/project/onboardapis)
 
----
-
-Install the latest development version of onboardapis
-from [GitHub](https://github.com/felix-zenk/onboardapis)
+or the latest prerelease version of onboardapis
+from [PyPI](https://pypi.org/project/onboardapis/2.0.0rc3/)
 using [pip](https://pip.pypa.io/en/stable/installation/):
 
 ```shell
-$ python -m pip install git+https://github.com/felix-zenk/onboardapis.git
+$ python -m pip install --pre onboardapis
 ```
 
-![Version](https://img.shields.io/badge/v2.0.0-%20?color=1081c2)
+[![Version](https://img.shields.io/badge/v2.0.0rc3-%20?color=1081c2)](https://pypi.org/project/onboardapis/2.0.0rc3/)
 
 ---
 
-Clone the repository
+Install the latest development version of onboardapis
 from [GitHub](https://github.com/felix-zenk/onboardapis)
-and install the package in development mode:
+using [pip](https://pip.pypa.io/en/stable/installation/):
 
 ```shell
-$ git clone https://github.com/felix-zenk/onboardapis.git
-$ cd onboardapis
-$ python -m pip install -e .
+$ python -m pip install git+https://github.com/felix-zenk/onboardapis.git
 ```
 
-![Version](https://img.shields.io/badge/v2.0.0-%20?color=1081c2)
-
 ---
 
 ## Quickstart
 
 To begin with development you will need to know a few things first:
 
 * What vehicle type you want to use
@@ -161,29 +160,35 @@
 [![GitHub-Pages](https://github.com/felix-zenk/onboardapis/actions/workflows/docs.yml/badge.svg)](https://felix-zenk.github.io/onboardapis/)
 
 #### Access the documentation on [GitHub-Pages](https://felix-zenk.github.io/onboardapis/).
 
 
 ## Supported APIs
 
-| API                   | [API scope](#api-scope) | Type  | Country      | Operator                                                                           |
-|-----------------------|-------------------------|-------|--------------|------------------------------------------------------------------------------------|
-| RailnetRegio          | geo                     | train | at (Austria) | obb (Österreichische Bundesbahnen)                                                 |
-| ICEPortal             | full                    | train | de (Germany) | db (Deutsche Bahn / DB AG)                                                         |
-| FlixTainment          | geo                     | train | de (Germany) | flix (Flix Train GmbH)                                                             |
-| MetronomCaptivePortal | basic                   | train | de (Germany) | me (metronom Eisenbahngesellschaft mbH) / bth (ALSTOM Transportation Germany GmbH) |
+| API                   | [API scope](#api-scope)   | Type  | Country      | Operator                                |
+|-----------------------|---------------------------|-------|--------------|-----------------------------------------|
+| RailnetRegio          | geo                       | train | at (Austria) | obb (Österreichische Bundesbahnen)      |
+| ICEPortal             | full, *internet-access*\* | train | de (Germany) | db (Deutsche Bahn / DB AG)              |
+| FlixTainment          | geo                       | train | de (Germany) | flix (Flix Train GmbH)                  |
+| MetronomCaptivePortal | *internet-access*\*       | train | de (Germany) | me (metronom Eisenbahngesellschaft mbH) |
+
+> **Notes**:
+> - \* Managing internet access is not yet supported.
 
 ## Experimental APIs
 
-| API              | [API scope](#api-scope) | Type  | Country      | Operator                     |
-|------------------|-------------------------|-------|--------------|------------------------------|
-| PortalINOUI      | full                    | train | fr (France)  | sncf (SNCF Voyageurs)        |
-| ZugPortal        | full                    | train | de (Germany) | db (Deutsche Bahn / DB AG)   |
-| PortaleRegionale | journey-simple          | train | it (Italy)   | ti (Trenitalia S.p.A.)       |
-| SBahnHannover    | journey-simple          | train | de (Germany) | tdh (Transdev Hannover GmbH) |
+| API              | [API scope](#api-scope)             | Type  | Country      | Operator                     |
+|------------------|-------------------------------------|-------|--------------|------------------------------|
+| PortalINOUI      | full                                | train | fr (France)  | sncf (SNCF Voyageurs)        |
+| ZugPortal        | full                                | train | de (Germany) | db (Deutsche Bahn / DB AG)   |
+| PortaleRegionale | journey-simple                      | train | it (Italy)   | ti (Trenitalia S.p.A.)       |
+| SBahnHannover    | journey-simple, *internet-access*\* | train | de (Germany) | tdh (Transdev Hannover GmbH) |
+
+> **Notes**:
+> - \* Managing internet access is not yet supported.
 
 ## APIs in development
 
 | API  | [API scope](#api-scope) | Type  | Country | Operator |
 |------|-------------------------|-------|---------|----------|
 | ...  |                         |       |         |          |
 
@@ -215,7 +220,8 @@
 The currently possible API scopes are:
 - ``basic``: Only basic information is available such as connection status to the API.
 - ``vehicle``: The API supplies information about the vehicle such as the train ID, line number, etc.
 - ``geo``: The API supplies information about the current location, speed, etc. of the vehicle.
 - ``journey-simple``: The API supplies simple journey information including the current station and the destination station.
 - ``journey``: The API supplies detailed journey information including all the stations and possibly connecting services.
 - ``full``: All of the above.
+- ``internet-access``: The API provides internet access to the user.
```

### Comparing `onboardapis-2.0.0rc2/README.md` & `onboardapis-2.0.0rc3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 onboardapis
 ===
 
 [![Python versions](https://img.shields.io/pypi/pyversions/onboardapis)](https://pypi.org/project/onboardapis)
 [![PyPI version](https://badge.fury.io/py/onboardapis.svg)](https://pypi.org/project/onboardapis)
+[![License](https://img.shields.io/github/license/felix-zenk/onboardapis)](https://github.com/felix-zenk/onboardapis/blob/main/LICENSE)  
 [![Build package](https://github.com/felix-zenk/onboardapis/actions/workflows/build.yml/badge.svg)](https://github.com/felix-zenk/onboardapis/actions/workflows/build.yml)
 [![Deploy documentation](https://github.com/felix-zenk/onboardapis/actions/workflows/docs.yml/badge.svg)](https://github.com/felix-zenk/onboardapis/actions/workflows/docs.yml)
-[![License](https://img.shields.io/github/license/felix-zenk/onboardapis)](https://github.com/felix-zenk/onboardapis/blob/main/LICENSE)
 
 > **Warning**: Version `2.0.0` introduces breaking changes! Existing code will definitely not work anymore.
 
 ## Description
 
 onboardapis allows you to interact with different on-board APIs.
 You can connect to the Wi-Fi of a supported transportation provider
@@ -26,42 +26,36 @@
 from [PyPI](https://pypi.org/project/onboardapis)
 using [pip](https://pip.pypa.io/en/stable/installation/):
 
 ```shell
 $ python -m pip install onboardapis
 ```
 
-![Version](https://img.shields.io/pypi/v/onboardapis?label=%20)
+[![Version](https://img.shields.io/pypi/v/onboardapis?label=%20)](https://pypi.org/project/onboardapis)
 
----
-
-Install the latest development version of onboardapis
-from [GitHub](https://github.com/felix-zenk/onboardapis)
+or the latest prerelease version of onboardapis
+from [PyPI](https://pypi.org/project/onboardapis/2.0.0rc3/)
 using [pip](https://pip.pypa.io/en/stable/installation/):
 
 ```shell
-$ python -m pip install git+https://github.com/felix-zenk/onboardapis.git
+$ python -m pip install --pre onboardapis
 ```
 
-![Version](https://img.shields.io/badge/v2.0.0-%20?color=1081c2)
+[![Version](https://img.shields.io/badge/v2.0.0rc3-%20?color=1081c2)](https://pypi.org/project/onboardapis/2.0.0rc3/)
 
 ---
 
-Clone the repository
+Install the latest development version of onboardapis
 from [GitHub](https://github.com/felix-zenk/onboardapis)
-and install the package in development mode:
+using [pip](https://pip.pypa.io/en/stable/installation/):
 
 ```shell
-$ git clone https://github.com/felix-zenk/onboardapis.git
-$ cd onboardapis
-$ python -m pip install -e .
+$ python -m pip install git+https://github.com/felix-zenk/onboardapis.git
 ```
 
-![Version](https://img.shields.io/badge/v2.0.0-%20?color=1081c2)
-
 ---
 
 ## Quickstart
 
 To begin with development you will need to know a few things first:
 
 * What vehicle type you want to use
@@ -124,29 +118,35 @@
 [![GitHub-Pages](https://github.com/felix-zenk/onboardapis/actions/workflows/docs.yml/badge.svg)](https://felix-zenk.github.io/onboardapis/)
 
 #### Access the documentation on [GitHub-Pages](https://felix-zenk.github.io/onboardapis/).
 
 
 ## Supported APIs
 
-| API                   | [API scope](#api-scope) | Type  | Country      | Operator                                                                           |
-|-----------------------|-------------------------|-------|--------------|------------------------------------------------------------------------------------|
-| RailnetRegio          | geo                     | train | at (Austria) | obb (Österreichische Bundesbahnen)                                                 |
-| ICEPortal             | full                    | train | de (Germany) | db (Deutsche Bahn / DB AG)                                                         |
-| FlixTainment          | geo                     | train | de (Germany) | flix (Flix Train GmbH)                                                             |
-| MetronomCaptivePortal | basic                   | train | de (Germany) | me (metronom Eisenbahngesellschaft mbH) / bth (ALSTOM Transportation Germany GmbH) |
+| API                   | [API scope](#api-scope)   | Type  | Country      | Operator                                |
+|-----------------------|---------------------------|-------|--------------|-----------------------------------------|
+| RailnetRegio          | geo                       | train | at (Austria) | obb (Österreichische Bundesbahnen)      |
+| ICEPortal             | full, *internet-access*\* | train | de (Germany) | db (Deutsche Bahn / DB AG)              |
+| FlixTainment          | geo                       | train | de (Germany) | flix (Flix Train GmbH)                  |
+| MetronomCaptivePortal | *internet-access*\*       | train | de (Germany) | me (metronom Eisenbahngesellschaft mbH) |
+
+> **Notes**:
+> - \* Managing internet access is not yet supported.
 
 ## Experimental APIs
 
-| API              | [API scope](#api-scope) | Type  | Country      | Operator                     |
-|------------------|-------------------------|-------|--------------|------------------------------|
-| PortalINOUI      | full                    | train | fr (France)  | sncf (SNCF Voyageurs)        |
-| ZugPortal        | full                    | train | de (Germany) | db (Deutsche Bahn / DB AG)   |
-| PortaleRegionale | journey-simple          | train | it (Italy)   | ti (Trenitalia S.p.A.)       |
-| SBahnHannover    | journey-simple          | train | de (Germany) | tdh (Transdev Hannover GmbH) |
+| API              | [API scope](#api-scope)             | Type  | Country      | Operator                     |
+|------------------|-------------------------------------|-------|--------------|------------------------------|
+| PortalINOUI      | full                                | train | fr (France)  | sncf (SNCF Voyageurs)        |
+| ZugPortal        | full                                | train | de (Germany) | db (Deutsche Bahn / DB AG)   |
+| PortaleRegionale | journey-simple                      | train | it (Italy)   | ti (Trenitalia S.p.A.)       |
+| SBahnHannover    | journey-simple, *internet-access*\* | train | de (Germany) | tdh (Transdev Hannover GmbH) |
+
+> **Notes**:
+> - \* Managing internet access is not yet supported.
 
 ## APIs in development
 
 | API  | [API scope](#api-scope) | Type  | Country | Operator |
 |------|-------------------------|-------|---------|----------|
 | ...  |                         |       |         |          |
 
@@ -178,7 +178,8 @@
 The currently possible API scopes are:
 - ``basic``: Only basic information is available such as connection status to the API.
 - ``vehicle``: The API supplies information about the vehicle such as the train ID, line number, etc.
 - ``geo``: The API supplies information about the current location, speed, etc. of the vehicle.
 - ``journey-simple``: The API supplies simple journey information including the current station and the destination station.
 - ``journey``: The API supplies detailed journey information including all the stations and possibly connecting services.
 - ``full``: All of the above.
+- ``internet-access``: The API provides internet access to the user.
```

### Comparing `onboardapis-2.0.0rc2/onboardapis/__init__.py` & `onboardapis-2.0.0rc3/onboardapis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,19 @@
     "units",
     "Vehicle",
     "Station",
     "ConnectingVehicle",
 ]
 
 
+def _package_version() -> str:
+    from importlib.metadata import version
+    return version('onboardapis')
+
+
 class Vehicle(metaclass=ABCMeta):
     """
     Base class for all vehicles
     """
 
     _api: API
     """The :class:`API` that supplies the data for this vehicle."""
@@ -56,14 +61,16 @@
 
         Raises:
           InitialConnectionError: If the connection to the API could not be established.
         """
         if not hasattr(self, '_api'):
             return  # Abstract class without API implementation
 
+        self._api.init()
+
         if isinstance(self._api, ThreadedAPI):
             self._api.start()
             while not self._api.is_connected:
                 sleep(.1)
             return
 
         return
```

### Comparing `onboardapis-2.0.0rc2/onboardapis/data.py` & `onboardapis-2.0.0rc3/onboardapis/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     except importlib.metadata.PackageNotFoundError:
         return 'unknown'
 
 
 def default(arg: Any, default: Any = None, *, boolean: bool = True) -> Any:  # noqa: F402
     """Return ``arg`` if it evaluates to ``True``, else return ``default``.
 
-    Set ``boolean`` to ``False`` to only test for ``arg=None``.
+    Set ``boolean`` to ``False`` to only test for ``arg is None``.
 
     Args:
         arg: The data to test.
         default: The default value to return if no data is present.
         boolean: Return the default if `arg` evaluates to False.
 
     Returns:
@@ -189,14 +189,18 @@
 
     def __getitem__(self, item):
         return self._data[item]
 
     def __setitem__(self, key, value):
         self._data[key] = value
 
+    def init(self) -> None:
+        """Initialize the API connection."""
+        pass
+
 
 def store(name=None):
     """
     Decorator / decorator factory to apply to an ``API`` method
     to immediately store the return value of the decorated method
     as the key ``name`` or the method name if left out.
     """
```

### Comparing `onboardapis-2.0.0rc2/onboardapis/exceptions.py` & `onboardapis-2.0.0rc3/onboardapis/exceptions.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/onboardapis/mixins.py` & `onboardapis-2.0.0rc3/onboardapis/mixins.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/onboardapis/protocols.py` & `onboardapis-2.0.0rc3/onboardapis/protocols.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/onboardapis/train/__init__.py` & `onboardapis-2.0.0rc3/onboardapis/train/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 """
 from __future__ import annotations
 
 import logging
 
 from abc import ABCMeta
 from dataclasses import dataclass
+from typing import cast
 
 from .. import Vehicle, Station, ConnectingVehicle
 from ..data import ScheduledEvent
 
 # noinspection PyUnresolvedReferences
 from typing import Iterable  # for associations while generating docs
 # noinspection PyUnresolvedReferences
@@ -51,25 +52,31 @@
 
 
 @dataclass
 class TrainStation(Station):
     """
     An `onboardapis.Station` with the additional information of a platform
     """
+    _connections: Iterable[ConnectingTrain]
+
     platform: ScheduledEvent[str] | None
     """The platform where the train arrives."""
 
+    @property
+    def connections(self) -> list[ConnectingTrain]:
+        return cast(list[ConnectingTrain], super().connections)  # maybe force type instead of casting?
+
 
 class Train(Vehicle, metaclass=ABCMeta):
     """
     Base class for all train implementations.
     """
 
     def __repr__(self) -> str:
-        return f"<{self.__class__.__name__} {self.id}>"
+        return f"<{self.__class__.__name__}>"
 
     @property
     def type(self) -> str:
         """The abbreviated train type."""
         return 'undefined'
 
     @property
```

### Comparing `onboardapis-2.0.0rc2/onboardapis/train/at/obb/apis.py` & `onboardapis-2.0.0rc3/onboardapis/train/at/obb/apis.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/onboardapis/train/at/obb/interfaces.py` & `onboardapis-2.0.0rc3/onboardapis/train/at/obb/interfaces.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 import logging
 import time
 
 from functools import lru_cache
 from typing import TypedDict
 
-from typing_extensions import deprecated
+from deprecation import deprecated
 
+from .... import _package_version
 from ....data import ThreadedRestAPI, store
 
 logger = logging.getLogger(__name__)
 
 Endpoints = TypedDict("Endpoints", {
     'api/train_info': int,
     'api/gps': dict,
@@ -32,15 +33,20 @@
     def gps(self) -> dict:
         return self.get("api/gps").json()
 
     @store('speed')
     def speed(self) -> float:
         return float(self.get("api/speed").text)
 
-    @deprecated('combined has been removed from the API')
+    @deprecated(
+        deprecated_in='2.0.0',
+        removed_in='2.1.0',
+        current_version=_package_version(),
+        details='combined has been removed from the API by ÖBB'
+    )
     @store('combined')
     def combined(self) -> dict:
         return self.get("assets/modules/fis/combined.json", params={"_time": time.time()}).json()
 
     def refresh(self) -> None:
         self.train_info()
         self.gps()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `onboardapis-2.0.0rc2/onboardapis/train/de/db/apis.py` & `onboardapis-2.0.0rc3/onboardapis/train/de/db/apis.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 import logging
 import re
 
 from typing import Literal
 from datetime import datetime, timedelta
 
-from typing_extensions import deprecated
+from deprecation import deprecated
 
+from .... import _package_version
 from ....exceptions import DataInvalidError
 from ....data import ID, default, ScheduledEvent, Position
 from ....mixins import SpeedMixin, PositionMixin, StationsMixin, InternetAccessMixin
 from ....units import ms
 from ... import Train, TrainStation
 from .mappings import id_name_map
 from .interfaces import ICEPortalAPI, RegioGuideAPI, ICEPortalInternetInterface
@@ -99,14 +100,22 @@
     @property
     def current_station(self) -> TrainStation:
         # Get the current station id
         stop_info = (
             self._api["trip"].get("trip", {}).get("stopInfo", {})
         )
         station_id = default(stop_info.get("actualNext"))
+        if station_id is None:  # None if the arrival time of the last station has passed
+            stop, *_ = *filter(
+                lambda s: not s.get("info", {}).get("passed", True),
+                self._api["trip"].get("trip", {}).get("stops", [])
+            ), None
+            if stop is None:  # None if all stations have been passed
+                return self.destination
+            station_id = stop.get("station", {}).get("evaNr")
         # Get the station from the stations dict
         try:
             return self.stations_dict[station_id]
         except KeyError as e:
             raise DataInvalidError("No current station found") from e
 
     @property
@@ -284,9 +293,15 @@
         station, *_ = (*filter(
             lambda s: self.now < default(s.arrival.actual, s.departure.actual),
             self.stations
         ), None)
         return self.destination if station is None else station
 
 
-ZugPortal = deprecated('Renamed by DB. Use RegioGuide instead.')(RegioGuide)
-"""Renamed by DB. Use RegioGuide instead."""
+@deprecated(
+    deprecated_in='2.0.0rc3',
+    removed_in='2.0.0',
+    current_version=_package_version(),
+    details='Renamed by DB. Use RegioGuide instead.'
+)
+class ZugPortal(RegioGuide):
+    """Renamed by DB. Use RegioGuide instead."""
```

### Comparing `onboardapis-2.0.0rc2/onboardapis/train/de/db/interfaces.py` & `onboardapis-2.0.0rc3/onboardapis/train/de/db/interfaces.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/onboardapis/train/de/db/mappings.py` & `onboardapis-2.0.0rc3/onboardapis/train/de/db/mappings.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/onboardapis/train/de/flix/apis.py` & `onboardapis-2.0.0rc3/onboardapis/train/de/flix/apis.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/onboardapis/train/de/me/apis.py` & `onboardapis-2.0.0rc3/onboardapis/train/de/me/apis.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/onboardapis/train/de/me/interfaces.py` & `onboardapis-2.0.0rc3/onboardapis/train/de/me/interfaces.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/onboardapis/train/fr/sncf/apis.py` & `onboardapis-2.0.0rc3/onboardapis/train/fr/sncf/apis.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/onboardapis/train/fr/sncf/interfaces.py` & `onboardapis-2.0.0rc3/onboardapis/train/fr/sncf/interfaces.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/onboardapis/train/it/ti/apis.py` & `onboardapis-2.0.0rc3/onboardapis/train/it/ti/apis.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/onboardapis/train/it/ti/interfaces.py` & `onboardapis-2.0.0rc3/onboardapis/train/it/ti/interfaces.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/onboardapis/train/third_party/unwired/apis.py` & `onboardapis-2.0.0rc3/onboardapis/train/third_party/unwired/apis.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/onboardapis/train/third_party/unwired/interfaces.py` & `onboardapis-2.0.0rc3/onboardapis/train/third_party/unwired/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,14 +178,16 @@
     '''
     """The query to execute against the GraphQL API."""
 
     _user_session_id: str
 
     def __init__(self):
         ThreadedGraphQlAPI.__init__(self)
+
+    def init(self):
         try:
             response = requests.get(
                 'https://unwired.info/?source=wasabi',
                 headers={'User-Agent': 'Python/onboardapis (%s)' % get_package_version()}
             )
             self._user_session_id, *_ = parse_qs(urlparse(response.url).query)['user_session_id']
         except (ConnectionError, KeyError) as e:
```

### Comparing `onboardapis-2.0.0rc2/onboardapis/train/third_party/unwired/mixins.py` & `onboardapis-2.0.0rc3/onboardapis/train/third_party/unwired/mixins.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/onboardapis/units.py` & `onboardapis-2.0.0rc3/onboardapis/units.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/onboardapis.egg-info/PKG-INFO` & `onboardapis-2.0.0rc3/onboardapis.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: onboardapis
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: A pure Python wrapper for the on-board APIs of many different transportation providers.
 Author-email: Felix Zenk <felix.zenk@web.de>
 License: MIT
 Project-URL: Homepage, https://felix-zenk.github.io/onboardapis
 Project-URL: Documentation, https://felix-zenk.github.io/onboardapis/
 Project-URL: Repository, https://github.com/felix-zenk/onboardapis
 Project-URL: Issues, https://github.com/felix-zenk/onboardapis/issues
-Keywords: api,train,public-transport
+Keywords: public-transport,train,api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -25,28 +25,33 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: geopy>=2.3.0
 Requires-Dist: gql[all]>=3.5.0
 Requires-Dist: restfly>=1.4.7
 Requires-Dist: requests>=2.31.0
 Requires-Dist: beautifulsoup4>=4.12.2
-Requires-Dist: typing-extensions>=4.9.0
+Requires-Dist: deprecation>=2.1.0
 Provides-Extra: dev
 Requires-Dist: flake8>=7.0.0; extra == "dev"
+Requires-Dist: Flake8-pyproject>=1.2.3; extra == "dev"
 Requires-Dist: pdoc>=14.4.0; extra == "dev"
 Requires-Dist: build>=1.2.1; extra == "dev"
+Requires-Dist: pytest>=8.2.0; extra == "dev"
+Requires-Dist: pytest-cov>=5.0.0; extra == "dev"
+Requires-Dist: testcontainers>=3.7.1; extra == "dev"
+Requires-Dist: wiremock[testing]>=2.6.1; extra == "dev"
 
 onboardapis
 ===
 
 [![Python versions](https://img.shields.io/pypi/pyversions/onboardapis)](https://pypi.org/project/onboardapis)
 [![PyPI version](https://badge.fury.io/py/onboardapis.svg)](https://pypi.org/project/onboardapis)
+[![License](https://img.shields.io/github/license/felix-zenk/onboardapis)](https://github.com/felix-zenk/onboardapis/blob/main/LICENSE)  
 [![Build package](https://github.com/felix-zenk/onboardapis/actions/workflows/build.yml/badge.svg)](https://github.com/felix-zenk/onboardapis/actions/workflows/build.yml)
 [![Deploy documentation](https://github.com/felix-zenk/onboardapis/actions/workflows/docs.yml/badge.svg)](https://github.com/felix-zenk/onboardapis/actions/workflows/docs.yml)
-[![License](https://img.shields.io/github/license/felix-zenk/onboardapis)](https://github.com/felix-zenk/onboardapis/blob/main/LICENSE)
 
 > **Warning**: Version `2.0.0` introduces breaking changes! Existing code will definitely not work anymore.
 
 ## Description
 
 onboardapis allows you to interact with different on-board APIs.
 You can connect to the Wi-Fi of a supported transportation provider
@@ -63,42 +68,36 @@
 from [PyPI](https://pypi.org/project/onboardapis)
 using [pip](https://pip.pypa.io/en/stable/installation/):
 
 ```shell
 $ python -m pip install onboardapis
 ```
 
-![Version](https://img.shields.io/pypi/v/onboardapis?label=%20)
+[![Version](https://img.shields.io/pypi/v/onboardapis?label=%20)](https://pypi.org/project/onboardapis)
 
----
-
-Install the latest development version of onboardapis
-from [GitHub](https://github.com/felix-zenk/onboardapis)
+or the latest prerelease version of onboardapis
+from [PyPI](https://pypi.org/project/onboardapis/2.0.0rc3/)
 using [pip](https://pip.pypa.io/en/stable/installation/):
 
 ```shell
-$ python -m pip install git+https://github.com/felix-zenk/onboardapis.git
+$ python -m pip install --pre onboardapis
 ```
 
-![Version](https://img.shields.io/badge/v2.0.0-%20?color=1081c2)
+[![Version](https://img.shields.io/badge/v2.0.0rc3-%20?color=1081c2)](https://pypi.org/project/onboardapis/2.0.0rc3/)
 
 ---
 
-Clone the repository
+Install the latest development version of onboardapis
 from [GitHub](https://github.com/felix-zenk/onboardapis)
-and install the package in development mode:
+using [pip](https://pip.pypa.io/en/stable/installation/):
 
 ```shell
-$ git clone https://github.com/felix-zenk/onboardapis.git
-$ cd onboardapis
-$ python -m pip install -e .
+$ python -m pip install git+https://github.com/felix-zenk/onboardapis.git
 ```
 
-![Version](https://img.shields.io/badge/v2.0.0-%20?color=1081c2)
-
 ---
 
 ## Quickstart
 
 To begin with development you will need to know a few things first:
 
 * What vehicle type you want to use
@@ -161,29 +160,35 @@
 [![GitHub-Pages](https://github.com/felix-zenk/onboardapis/actions/workflows/docs.yml/badge.svg)](https://felix-zenk.github.io/onboardapis/)
 
 #### Access the documentation on [GitHub-Pages](https://felix-zenk.github.io/onboardapis/).
 
 
 ## Supported APIs
 
-| API                   | [API scope](#api-scope) | Type  | Country      | Operator                                                                           |
-|-----------------------|-------------------------|-------|--------------|------------------------------------------------------------------------------------|
-| RailnetRegio          | geo                     | train | at (Austria) | obb (Österreichische Bundesbahnen)                                                 |
-| ICEPortal             | full                    | train | de (Germany) | db (Deutsche Bahn / DB AG)                                                         |
-| FlixTainment          | geo                     | train | de (Germany) | flix (Flix Train GmbH)                                                             |
-| MetronomCaptivePortal | basic                   | train | de (Germany) | me (metronom Eisenbahngesellschaft mbH) / bth (ALSTOM Transportation Germany GmbH) |
+| API                   | [API scope](#api-scope)   | Type  | Country      | Operator                                |
+|-----------------------|---------------------------|-------|--------------|-----------------------------------------|
+| RailnetRegio          | geo                       | train | at (Austria) | obb (Österreichische Bundesbahnen)      |
+| ICEPortal             | full, *internet-access*\* | train | de (Germany) | db (Deutsche Bahn / DB AG)              |
+| FlixTainment          | geo                       | train | de (Germany) | flix (Flix Train GmbH)                  |
+| MetronomCaptivePortal | *internet-access*\*       | train | de (Germany) | me (metronom Eisenbahngesellschaft mbH) |
+
+> **Notes**:
+> - \* Managing internet access is not yet supported.
 
 ## Experimental APIs
 
-| API              | [API scope](#api-scope) | Type  | Country      | Operator                     |
-|------------------|-------------------------|-------|--------------|------------------------------|
-| PortalINOUI      | full                    | train | fr (France)  | sncf (SNCF Voyageurs)        |
-| ZugPortal        | full                    | train | de (Germany) | db (Deutsche Bahn / DB AG)   |
-| PortaleRegionale | journey-simple          | train | it (Italy)   | ti (Trenitalia S.p.A.)       |
-| SBahnHannover    | journey-simple          | train | de (Germany) | tdh (Transdev Hannover GmbH) |
+| API              | [API scope](#api-scope)             | Type  | Country      | Operator                     |
+|------------------|-------------------------------------|-------|--------------|------------------------------|
+| PortalINOUI      | full                                | train | fr (France)  | sncf (SNCF Voyageurs)        |
+| ZugPortal        | full                                | train | de (Germany) | db (Deutsche Bahn / DB AG)   |
+| PortaleRegionale | journey-simple                      | train | it (Italy)   | ti (Trenitalia S.p.A.)       |
+| SBahnHannover    | journey-simple, *internet-access*\* | train | de (Germany) | tdh (Transdev Hannover GmbH) |
+
+> **Notes**:
+> - \* Managing internet access is not yet supported.
 
 ## APIs in development
 
 | API  | [API scope](#api-scope) | Type  | Country | Operator |
 |------|-------------------------|-------|---------|----------|
 | ...  |                         |       |         |          |
 
@@ -215,7 +220,8 @@
 The currently possible API scopes are:
 - ``basic``: Only basic information is available such as connection status to the API.
 - ``vehicle``: The API supplies information about the vehicle such as the train ID, line number, etc.
 - ``geo``: The API supplies information about the current location, speed, etc. of the vehicle.
 - ``journey-simple``: The API supplies simple journey information including the current station and the destination station.
 - ``journey``: The API supplies detailed journey information including all the stations and possibly connecting services.
 - ``full``: All of the above.
+- ``internet-access``: The API provides internet access to the user.
```

### Comparing `onboardapis-2.0.0rc2/onboardapis.egg-info/SOURCES.txt` & `onboardapis-2.0.0rc3/onboardapis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc2/pyproject.toml` & `onboardapis-2.0.0rc3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "onboardapis"
 description = "A pure Python wrapper for the on-board APIs of many different transportation providers."
-version = "2.0.0rc2"
+version = "2.0.0rc3"
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.8"
-keywords = ["api", "train", "public-transport"]
+keywords = [
+    "public-transport",
+    "train",
+    "api",
+]
 license = { text = "MIT" }
 authors = [
     { name = "Felix Zenk", email = "felix.zenk@web.de" },
 ]
 dependencies = [
     "geopy>=2.3.0",
     "gql[all]>=3.5.0",
     "restfly>=1.4.7",
     "requests>=2.31.0",
     "beautifulsoup4>=4.12.2",
-    "typing-extensions>=4.9.0",
+    "deprecation>=2.1.0",
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -35,22 +39,33 @@
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Typing :: Typed",
 ]
 
 [project.optional-dependencies]
 dev = [
     "flake8>=7.0.0",
+    "Flake8-pyproject>=1.2.3",
     "pdoc>=14.4.0",
     "build>=1.2.1",
+    "pytest>=8.2.0",
+    "pytest-cov>=5.0.0",
+    "testcontainers>=3.7.1",
+    "wiremock[testing]>=2.6.1",
 ]
 
 [project.urls]
 Homepage = "https://felix-zenk.github.io/onboardapis"
 Documentation = "https://felix-zenk.github.io/onboardapis/"
 Repository = "https://github.com/felix-zenk/onboardapis"
 Issues = "https://github.com/felix-zenk/onboardapis/issues"
 
 [tool.setuptools.packages.find]
-include = ["onboardapis*"]
+include = ["onboardapis", "onboardapis.*"]
 
 [tool.setuptools.package-data]
 onboardapis = ["py.typed"]
+
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+
+[tool.flake8]
+max-line-length = 120
```


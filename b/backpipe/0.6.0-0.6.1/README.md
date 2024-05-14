# Comparing `tmp/backpipe-0.6.0.tar.gz` & `tmp/backpipe-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backpipe-0.6.0.tar", last modified: Mon May 13 21:23:42 2024, max compression
+gzip compressed data, was "backpipe-0.6.1.tar", last modified: Tue May 14 16:04:33 2024, max compression
```

## Comparing `backpipe-0.6.0.tar` & `backpipe-0.6.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.991404 backpipe-0.6.0/
--rw-r--r--   0 simon     (1000) simon     (1000)    35129 2023-11-04 20:14:40.000000 backpipe-0.6.0/LICENSE
--rw-r--r--   0 simon     (1000) simon     (1000)      176 2024-04-22 18:38:17.000000 backpipe-0.6.0/MANIFEST.in
--rw-r--r--   0 simon     (1000) simon     (1000)     3525 2024-05-13 21:23:42.991404 backpipe-0.6.0/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)     2872 2024-05-09 11:06:37.000000 backpipe-0.6.0/README.md
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.986405 backpipe-0.6.0/backpipe/
--rw-r--r--   0 simon     (1000) simon     (1000)      537 2024-05-09 10:29:17.000000 backpipe-0.6.0/backpipe/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     5172 2024-04-26 15:29:12.000000 backpipe-0.6.0/backpipe/__main__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     5798 2024-05-09 11:35:16.000000 backpipe-0.6.0/backpipe/app.py
--rw-r--r--   0 simon     (1000) simon     (1000)     3244 2024-03-30 02:36:58.000000 backpipe-0.6.0/backpipe/builder.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1027 2024-05-09 11:37:15.000000 backpipe-0.6.0/backpipe/config.py
--rw-r--r--   0 simon     (1000) simon     (1000)      364 2024-03-29 01:51:22.000000 backpipe-0.6.0/backpipe/defaults.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1916 2024-05-09 19:47:37.000000 backpipe-0.6.0/backpipe/host.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.988404 backpipe-0.6.0/backpipe/presets/
--rw-r--r--   0 simon     (1000) simon     (1000)      627 2024-05-09 14:02:28.000000 backpipe-0.6.0/backpipe/presets/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1468 2024-04-27 13:29:04.000000 backpipe-0.6.0/backpipe/presets/file.py
--rw-r--r--   0 simon     (1000) simon     (1000)      459 2024-04-27 13:29:04.000000 backpipe-0.6.0/backpipe/presets/ipaddr.py
--rw-r--r--   0 simon     (1000) simon     (1000)      870 2024-05-09 15:37:55.000000 backpipe-0.6.0/backpipe/presets/redirect.py
--rw-r--r--   0 simon     (1000) simon     (1000)      589 2024-05-11 09:44:30.000000 backpipe-0.6.0/backpipe/redirect.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1233 2024-05-09 10:28:38.000000 backpipe-0.6.0/backpipe/rq.py
--rw-r--r--   0 simon     (1000) simon     (1000)     7185 2024-05-10 12:09:45.000000 backpipe-0.6.0/backpipe/server.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.988404 backpipe-0.6.0/backpipe/tools/
--rw-r--r--   0 simon     (1000) simon     (1000)      178 2024-04-22 17:36:44.000000 backpipe-0.6.0/backpipe/tools/__init__.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.988404 backpipe-0.6.0/backpipe/tools/base64/
--rw-r--r--   0 simon     (1000) simon     (1000)       95 2024-04-15 14:45:34.000000 backpipe-0.6.0/backpipe/tools/base64/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      177 2024-04-15 14:45:00.000000 backpipe-0.6.0/backpipe/tools/base64/decode.py
--rw-r--r--   0 simon     (1000) simon     (1000)      177 2024-04-15 14:43:40.000000 backpipe-0.6.0/backpipe/tools/base64/encode.py
--rw-r--r--   0 simon     (1000) simon     (1000)      398 2024-04-15 15:05:34.000000 backpipe-0.6.0/backpipe/tools/check_type.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.989405 backpipe-0.6.0/backpipe/tools/file/
--rw-r--r--   0 simon     (1000) simon     (1000)      181 2024-04-22 17:06:34.000000 backpipe-0.6.0/backpipe/tools/file/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      464 2024-04-22 17:03:16.000000 backpipe-0.6.0/backpipe/tools/file/append.py
--rw-r--r--   0 simon     (1000) simon     (1000)      301 2024-04-22 16:26:18.000000 backpipe-0.6.0/backpipe/tools/file/create.py
--rw-r--r--   0 simon     (1000) simon     (1000)      388 2024-04-22 16:51:25.000000 backpipe-0.6.0/backpipe/tools/file/delete.py
--rw-r--r--   0 simon     (1000) simon     (1000)      463 2024-04-22 16:39:25.000000 backpipe-0.6.0/backpipe/tools/file/write.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.990404 backpipe-0.6.0/backpipe/tools/hash/
--rw-r--r--   0 simon     (1000) simon     (1000)      265 2024-04-22 17:45:34.000000 backpipe-0.6.0/backpipe/tools/hash/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      284 2024-04-22 17:41:35.000000 backpipe-0.6.0/backpipe/tools/hash/md5.py
--rw-r--r--   0 simon     (1000) simon     (1000)      286 2024-04-22 17:41:54.000000 backpipe-0.6.0/backpipe/tools/hash/sha1.py
--rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:42:44.000000 backpipe-0.6.0/backpipe/tools/hash/sha224.py
--rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:42:57.000000 backpipe-0.6.0/backpipe/tools/hash/sha256.py
--rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:44:00.000000 backpipe-0.6.0/backpipe/tools/hash/sha384.py
--rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:44:07.000000 backpipe-0.6.0/backpipe/tools/hash/sha512.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.990404 backpipe-0.6.0/backpipe/tools/html/
--rw-r--r--   0 simon     (1000) simon     (1000)       41 2024-04-14 18:21:28.000000 backpipe-0.6.0/backpipe/tools/html/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      212 2024-04-14 20:54:18.000000 backpipe-0.6.0/backpipe/tools/html/addMeta.py
--rw-r--r--   0 simon     (1000) simon     (1000)      130 2024-04-14 20:54:11.000000 backpipe-0.6.0/backpipe/tools/html/addStyle.py
--rw-r--r--   0 simon     (1000) simon     (1000)      346 2024-04-27 09:07:22.000000 backpipe-0.6.0/backpipe/tools/html/addTag.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1176 2024-04-27 09:10:21.000000 backpipe-0.6.0/backpipe/tools/html/html.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.991404 backpipe-0.6.0/backpipe/tools/json/
--rw-r--r--   0 simon     (1000) simon     (1000)      107 2024-04-14 16:06:07.000000 backpipe-0.6.0/backpipe/tools/json/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      184 2024-04-15 14:42:14.000000 backpipe-0.6.0/backpipe/tools/json/deserialize.py
--rw-r--r--   0 simon     (1000) simon     (1000)      262 2024-04-15 14:42:48.000000 backpipe-0.6.0/backpipe/tools/json/serialize.py
--rw-r--r--   0 simon     (1000) simon     (1000)      137 2023-11-14 15:08:41.000000 backpipe-0.6.0/backpipe/uptime.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.987404 backpipe-0.6.0/backpipe.egg-info/
--rw-r--r--   0 simon     (1000) simon     (1000)     3525 2024-05-13 21:23:42.000000 backpipe-0.6.0/backpipe.egg-info/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)     1316 2024-05-13 21:23:42.000000 backpipe-0.6.0/backpipe.egg-info/SOURCES.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        1 2024-05-13 21:23:42.000000 backpipe-0.6.0/backpipe.egg-info/dependency_links.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       52 2024-05-13 21:23:42.000000 backpipe-0.6.0/backpipe.egg-info/entry_points.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       19 2024-05-13 21:23:42.000000 backpipe-0.6.0/backpipe.egg-info/requires.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        9 2024-05-13 21:23:42.000000 backpipe-0.6.0/backpipe.egg-info/top_level.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       38 2024-05-13 21:23:42.991404 backpipe-0.6.0/setup.cfg
--rw-r--r--   0 simon     (1000) simon     (1000)     1532 2024-04-26 16:49:47.000000 backpipe-0.6.0/setup.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-14 16:04:33.884154 backpipe-0.6.1/
+-rw-r--r--   0 simon     (1000) simon     (1000)    35129 2023-11-04 20:14:40.000000 backpipe-0.6.1/LICENSE
+-rw-r--r--   0 simon     (1000) simon     (1000)      176 2024-04-22 18:38:17.000000 backpipe-0.6.1/MANIFEST.in
+-rw-r--r--   0 simon     (1000) simon     (1000)     3525 2024-05-14 16:04:33.883154 backpipe-0.6.1/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)     2872 2024-05-09 11:06:37.000000 backpipe-0.6.1/README.md
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-14 16:04:33.879155 backpipe-0.6.1/backpipe/
+-rw-r--r--   0 simon     (1000) simon     (1000)      537 2024-05-14 15:50:11.000000 backpipe-0.6.1/backpipe/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     5172 2024-04-26 15:29:12.000000 backpipe-0.6.1/backpipe/__main__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     5798 2024-05-09 11:35:16.000000 backpipe-0.6.1/backpipe/app.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     3527 2024-05-14 16:00:28.000000 backpipe-0.6.1/backpipe/builder.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1027 2024-05-09 11:37:15.000000 backpipe-0.6.1/backpipe/config.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      364 2024-03-29 01:51:22.000000 backpipe-0.6.1/backpipe/defaults.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1916 2024-05-09 19:47:37.000000 backpipe-0.6.1/backpipe/host.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-14 16:04:33.880154 backpipe-0.6.1/backpipe/presets/
+-rw-r--r--   0 simon     (1000) simon     (1000)      627 2024-05-09 14:02:28.000000 backpipe-0.6.1/backpipe/presets/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1476 2024-05-14 15:59:14.000000 backpipe-0.6.1/backpipe/presets/file.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      465 2024-05-14 15:59:22.000000 backpipe-0.6.1/backpipe/presets/ipaddr.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      870 2024-05-09 15:37:55.000000 backpipe-0.6.1/backpipe/presets/redirect.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      600 2024-05-14 15:54:50.000000 backpipe-0.6.1/backpipe/redirect.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1233 2024-05-09 10:28:38.000000 backpipe-0.6.1/backpipe/rq.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     7185 2024-05-10 12:09:45.000000 backpipe-0.6.1/backpipe/server.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-14 16:04:33.881154 backpipe-0.6.1/backpipe/tools/
+-rw-r--r--   0 simon     (1000) simon     (1000)      178 2024-04-22 17:36:44.000000 backpipe-0.6.1/backpipe/tools/__init__.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-14 16:04:33.881154 backpipe-0.6.1/backpipe/tools/base64/
+-rw-r--r--   0 simon     (1000) simon     (1000)       95 2024-04-15 14:45:34.000000 backpipe-0.6.1/backpipe/tools/base64/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      177 2024-04-15 14:45:00.000000 backpipe-0.6.1/backpipe/tools/base64/decode.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      177 2024-04-15 14:43:40.000000 backpipe-0.6.1/backpipe/tools/base64/encode.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      398 2024-04-15 15:05:34.000000 backpipe-0.6.1/backpipe/tools/check_type.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-14 16:04:33.882154 backpipe-0.6.1/backpipe/tools/file/
+-rw-r--r--   0 simon     (1000) simon     (1000)      181 2024-04-22 17:06:34.000000 backpipe-0.6.1/backpipe/tools/file/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      464 2024-04-22 17:03:16.000000 backpipe-0.6.1/backpipe/tools/file/append.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      301 2024-04-22 16:26:18.000000 backpipe-0.6.1/backpipe/tools/file/create.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      388 2024-04-22 16:51:25.000000 backpipe-0.6.1/backpipe/tools/file/delete.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      463 2024-04-22 16:39:25.000000 backpipe-0.6.1/backpipe/tools/file/write.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-14 16:04:33.882154 backpipe-0.6.1/backpipe/tools/hash/
+-rw-r--r--   0 simon     (1000) simon     (1000)      265 2024-04-22 17:45:34.000000 backpipe-0.6.1/backpipe/tools/hash/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      284 2024-04-22 17:41:35.000000 backpipe-0.6.1/backpipe/tools/hash/md5.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      286 2024-04-22 17:41:54.000000 backpipe-0.6.1/backpipe/tools/hash/sha1.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:42:44.000000 backpipe-0.6.1/backpipe/tools/hash/sha224.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:42:57.000000 backpipe-0.6.1/backpipe/tools/hash/sha256.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:44:00.000000 backpipe-0.6.1/backpipe/tools/hash/sha384.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:44:07.000000 backpipe-0.6.1/backpipe/tools/hash/sha512.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-14 16:04:33.883154 backpipe-0.6.1/backpipe/tools/html/
+-rw-r--r--   0 simon     (1000) simon     (1000)       41 2024-04-14 18:21:28.000000 backpipe-0.6.1/backpipe/tools/html/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      212 2024-04-14 20:54:18.000000 backpipe-0.6.1/backpipe/tools/html/addMeta.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      130 2024-04-14 20:54:11.000000 backpipe-0.6.1/backpipe/tools/html/addStyle.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      346 2024-04-27 09:07:22.000000 backpipe-0.6.1/backpipe/tools/html/addTag.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1176 2024-04-27 09:10:21.000000 backpipe-0.6.1/backpipe/tools/html/html.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-14 16:04:33.883154 backpipe-0.6.1/backpipe/tools/json/
+-rw-r--r--   0 simon     (1000) simon     (1000)      107 2024-04-14 16:06:07.000000 backpipe-0.6.1/backpipe/tools/json/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      184 2024-04-15 14:42:14.000000 backpipe-0.6.1/backpipe/tools/json/deserialize.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      262 2024-04-15 14:42:48.000000 backpipe-0.6.1/backpipe/tools/json/serialize.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      137 2023-11-14 15:08:41.000000 backpipe-0.6.1/backpipe/uptime.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-14 16:04:33.880154 backpipe-0.6.1/backpipe.egg-info/
+-rw-r--r--   0 simon     (1000) simon     (1000)     3525 2024-05-14 16:04:33.000000 backpipe-0.6.1/backpipe.egg-info/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)     1316 2024-05-14 16:04:33.000000 backpipe-0.6.1/backpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        1 2024-05-14 16:04:33.000000 backpipe-0.6.1/backpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       52 2024-05-14 16:04:33.000000 backpipe-0.6.1/backpipe.egg-info/entry_points.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       19 2024-05-14 16:04:33.000000 backpipe-0.6.1/backpipe.egg-info/requires.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        9 2024-05-14 16:04:33.000000 backpipe-0.6.1/backpipe.egg-info/top_level.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       38 2024-05-14 16:04:33.884154 backpipe-0.6.1/setup.cfg
+-rw-r--r--   0 simon     (1000) simon     (1000)     1532 2024-04-26 16:49:47.000000 backpipe-0.6.1/setup.py
```

### Comparing `backpipe-0.6.0/LICENSE` & `backpipe-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.0/PKG-INFO` & `backpipe-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backpipe
-Version: 0.6.0
+Version: 0.6.1
 Summary: A backend HTTP framework for Python.
 Home-page: https://github.com/Simoso68/backpipe
 Author: Simoso68
 Maintainer: Simoso68
 License: GNU GPL v3
 Keywords: framework,http,web,api,server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `backpipe-0.6.0/README.md` & `backpipe-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.0/backpipe/__init__.py` & `backpipe-0.6.1/backpipe/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 from backpipe.redirect import redirect
 from colorama import init as __init
 
 import backpipe.tools as tools
 
 __init()
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
```

### Comparing `backpipe-0.6.0/backpipe/__main__.py` & `backpipe-0.6.1/backpipe/__main__.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.0/backpipe/app.py` & `backpipe-0.6.1/backpipe/app.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.0/backpipe/builder.py` & `backpipe-0.6.1/backpipe/builder.py`

 * *Files 15% similar despite different names*

```diff
@@ -54,17 +54,22 @@
         self.blocked_msg = f
     def block_address(self, addrs):
         self.block_addrs.extend(addrs)
     def uri_limit_msg(self, message):
         self.uri_limit_message = message
     def run(self):
         try:
+            if self.addr == "":
+                ADDR = "127.0.0.1"
+            else:
+                ADDR = self.addr
             if system() == "Windows":
                 print(f"\r{Back.YELLOW}{Fore.BLACK} COMPATIBILITY {Back.RESET}{Fore.RESET} Running Backpipe servers on Windows might lead to issues")
             print(f"\r{Back.YELLOW}{Fore.BLACK} INFO {Back.RESET}{Fore.RESET} Starting server ...")
+            print(f"\r{Back.YELLOW}{Fore.BLACK} INFO {Back.RESET}{Fore.RESET} Running on {Fore.LIGHTBLUE_EX}{ADDR}{Fore.RESET}:{Fore.GREEN}{self.port}{Fore.RESET}")
             print(f"\r{Back.YELLOW}{Fore.BLACK} INFO {Back.RESET}{Fore.RESET} Press {Fore.LIGHTRED_EX}Ctrl + C{Fore.RESET} to quit.\n")
             backpipe_server = Server(self, self.https, self.get, self.post, self.put, self.patch, self.delete, self.unknown, self.uri_limit, self.uri_limit_message, self.blocked_msg, self.block_addrs, ratelimit=(self.ratelimit, self.ratelimit_message, self.ratelimit_reset, self.ratelimit_exc_addrs, self.ratelimit_exc_paths), server_address=(self.addr, self.port), RequestHandlerClass=BackPipeServer)
             backpipe_server.serve_forever()
         except KeyboardInterrupt:
             print(f"\r{Back.LIGHTRED_EX}{Fore.BLACK} EXIT {Back.RESET}{Fore.RESET} Received Keyboard interrupt, shutting down server.")
             kill(getpid(), SIGTERM)
         except Exception as x:
```

### Comparing `backpipe-0.6.0/backpipe/config.py` & `backpipe-0.6.1/backpipe/config.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.0/backpipe/host.py` & `backpipe-0.6.1/backpipe/host.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.0/backpipe/presets/__init__.py` & `backpipe-0.6.1/backpipe/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.0/backpipe/presets/file.py` & `backpipe-0.6.1/backpipe/presets/file.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,23 +4,23 @@
     import platform
     import urllib
 
     server = backpipe.BackPipe(addr, port)
 
     server.set_ratelimit(60)
 
-    @server.any
+    @server.any()
     def wrong_method(r: backpipe.Request):
         return (405, f"unsupported method: {r.method}, use GET")
     
-    @server.unknown
+    @server.unknown()
     def unknown_method(r: backpipe.Request):
         return (405, f"unsupported method: {r.method}, use GET")
 
-    @server.get
+    @server.get()
     def respond(r: backpipe.Request):
         try: 
             if platform.system() == "Windows":
                 PATH = urllib.parse.unquote(f"C:{r.path}")
             else:
                 PATH = urllib.parse.unquote(r.path)
 
@@ -39,12 +39,12 @@
                     HTML.add_tag("a", o, {"href":f"{CURRENT_DIR}/{o}"})
                 return (200, HTML.text())
             else:
                 return (200, open(PATH, "rb").read())
         except PermissionError:
             return (403, "can not access object")
         
-    @server.ratelimit
+    @server.ratelimit()
     def ratelimit_respond(r: backpipe.Request):
         return (429, "you sent too many requests")
     
     server.run()
```

### Comparing `backpipe-0.6.0/backpipe/presets/redirect.py` & `backpipe-0.6.1/backpipe/presets/redirect.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.0/backpipe/redirect.py` & `backpipe-0.6.1/backpipe/redirect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from backpipe.tools.check_type import check
 
 class BackPipeRedirect():
     def __init__(self, location: str, message: str | bytes) -> None:
         self.location = location
         self.message = message
     def __str__(self) -> str:
-        return f"Redirect(location={self.location}, message={self.message.__repr__()})"
+        return f"Redirect(location={self.location.__repr__()}, message={self.message.__repr__()})"
     def __repr__(self) -> str:
         return self.__str__()
 
 def redirect(location: str, message: str = "Page moved") -> BackPipeRedirect:
     check(location, str, "location")
     check(message, (str, bytes), "message")
     return BackPipeRedirect(location, message)
```

### Comparing `backpipe-0.6.0/backpipe/rq.py` & `backpipe-0.6.1/backpipe/rq.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.0/backpipe/server.py` & `backpipe-0.6.1/backpipe/server.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.0/backpipe/tools/html/html.py` & `backpipe-0.6.1/backpipe/tools/html/html.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.0/backpipe.egg-info/PKG-INFO` & `backpipe-0.6.1/backpipe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backpipe
-Version: 0.6.0
+Version: 0.6.1
 Summary: A backend HTTP framework for Python.
 Home-page: https://github.com/Simoso68/backpipe
 Author: Simoso68
 Maintainer: Simoso68
 License: GNU GPL v3
 Keywords: framework,http,web,api,server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `backpipe-0.6.0/backpipe.egg-info/SOURCES.txt` & `backpipe-0.6.1/backpipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.0/setup.py` & `backpipe-0.6.1/setup.py`

 * *Files identical despite different names*


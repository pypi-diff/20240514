# Comparing `tmp/pigeonpost-0.4.6.tar.gz` & `tmp/pigeonpost-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonpost-0.4.6.tar", last modified: Fri May  3 08:15:48 2024, max compression
+gzip compressed data, was "pigeonpost-0.4.7.tar", last modified: Tue May 14 12:53:32 2024, max compression
```

## Comparing `pigeonpost-0.4.6.tar` & `pigeonpost-0.4.7.tar`

### file list

```diff
@@ -1,73 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.587046 pigeonpost-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-03 08:15:48.587046 pigeonpost-0.4.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.579046 pigeonpost-0.4.6/pigeon/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.579046 pigeonpost-0.4.6/pigeon/conf/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/conf/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/conf/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.583046 pigeonpost-0.4.6/pigeon/core/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/core/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/core/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/core/secure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/core/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.583046 pigeonpost-0.4.6/pigeon/default/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/default/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.583046 pigeonpost-0.4.6/pigeon/files/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/files/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/files/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.583046 pigeonpost-0.4.6/pigeon/http/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/http/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/http/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/http/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/http/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.583046 pigeonpost-0.4.6/pigeon/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.587046 pigeonpost-0.4.6/pigeon/middleware/components/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/cache_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/component.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/content_negotiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/date.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/mediafiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/method.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/components/staticfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.587046 pigeonpost-0.4.6/pigeon/middleware/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/conversion/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.587046 pigeonpost-0.4.6/pigeon/middleware/conversion/mime/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/conversion/mime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/conversion/mime/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/conversion/mime/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/middleware/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.587046 pigeonpost-0.4.6/pigeon/templating/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/templating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/templating/templater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.587046 pigeonpost-0.4.6/pigeon/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/utils/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3260 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/pigeon/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:15:48.587046 pigeonpost-0.4.6/pigeonpost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-03 08:15:48.000000 pigeonpost-0.4.6/pigeonpost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-03 08:15:48.000000 pigeonpost-0.4.6/pigeonpost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 08:15:48.000000 pigeonpost-0.4.6/pigeonpost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-03 08:15:48.000000 pigeonpost-0.4.6/pigeonpost.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 08:15:48.000000 pigeonpost-0.4.6/pigeonpost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 08:15:48.000000 pigeonpost-0.4.6/pigeonpost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-03 08:15:48.591046 pigeonpost-0.4.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-05-03 08:15:42.000000 pigeonpost-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.447778 pigeonpost-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 12:53:32.447778 pigeonpost-0.4.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.439777 pigeonpost-0.4.7/pigeon/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.439777 pigeonpost-0.4.7/pigeon/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/conf/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/conf/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.443777 pigeonpost-0.4.7/pigeon/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/core/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/core/secure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/core/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.443777 pigeonpost-0.4.7/pigeon/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/default/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.443777 pigeonpost-0.4.7/pigeon/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/files/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/files/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.443777 pigeonpost-0.4.7/pigeon/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/http/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/http/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/http/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.443777 pigeonpost-0.4.7/pigeon/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.447778 pigeonpost-0.4.7/pigeon/middleware/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/cache_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/content_negotiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/mediafiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/staticfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.447778 pigeonpost-0.4.7/pigeon/middleware/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/conversion/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.447778 pigeonpost-0.4.7/pigeon/middleware/conversion/mime/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/conversion/mime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/conversion/mime/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/conversion/mime/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.447778 pigeonpost-0.4.7/pigeon/templating/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/templating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/templating/templater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.447778 pigeonpost-0.4.7/pigeon/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/utils/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3260 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.447778 pigeonpost-0.4.7/pigeonpost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 12:53:32.000000 pigeonpost-0.4.7/pigeonpost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-14 12:53:32.000000 pigeonpost-0.4.7/pigeonpost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:53:32.000000 pigeonpost-0.4.7/pigeonpost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 12:53:32.000000 pigeonpost-0.4.7/pigeonpost.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 12:53:32.000000 pigeonpost-0.4.7/pigeonpost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 12:53:32.000000 pigeonpost-0.4.7/pigeonpost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-14 12:53:32.451778 pigeonpost-0.4.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/setup.py
```

### Comparing `pigeonpost-0.4.6/pigeon/__init__.py` & `pigeonpost-0.4.7/pigeon/__init__.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/conf/settings.py` & `pigeonpost-0.4.7/pigeon/conf/settings.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/core/app.py` & `pigeonpost-0.4.7/pigeon/core/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 import pigeon.utils.logger as logger
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
 
 log = logger.Log('PIGEON', '#30b3ff')
 
 class Pigeon:
+    """
+    The Pigeon class is the main interface used for the user to interact with Pigeon.
+    """
+
     settings = None
     autorun = True
 
     # watchdog
     observers = []
     @classmethod
     def __init__(cls, settings=None):
```

### Comparing `pigeonpost-0.4.6/pigeon/core/handler.py` & `pigeonpost-0.4.7/pigeon/core/handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,18 +44,20 @@
             request = middleware.preprocess(data)
             if isinstance(request, HTTPRequest):
                 log.info(f'REQUEST: {request.path}')
 
             # gather appropriate response for request
             response = middleware.process(request)
             response = middleware.postprocess(request, response)
+            data = response.__bytes__('utf-8')
 
             # send response to client
             log.verbose(f'SENDING RESPONSE TO {client_address[0]}:{client_address[1]}')
-            client_sock.sendall(response.__bytes__('ascii'))
+            log.verbose(f'RAW RESPONSE:\n{response.__str__()}')
+            client_sock.sendall(data)
             log.verbose(f'RESPONSE SENT')
 
         except Exception as e:
             sys.excepthook(None, e, None, custom_log=log, description=f'EXCEPTION OCCURED WHILE HANDLING REQUEST FROM {client_address[0]}:{client_address[1]}')
 
         # do not keep connection open on error
         if response.is_error:
```

### Comparing `pigeonpost-0.4.6/pigeon/core/secure.py` & `pigeonpost-0.4.7/pigeon/core/secure.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/core/server.py` & `pigeonpost-0.4.7/pigeon/core/server.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/default/errors.py` & `pigeonpost-0.4.7/pigeon/default/errors.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/files/media.py` & `pigeonpost-0.4.7/pigeon/files/media.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/files/static.py` & `pigeonpost-0.4.7/pigeon/files/static.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/http/message.py` & `pigeonpost-0.4.7/pigeon/http/message.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         self.data: Any = data
         # protocol used (e.g. 1.1, 1.0, 2.0, ...)
         self.protocol: str = protocol
         # cookies of request
         self.cookies: LowerParameterDict = LowerParameterDict(cookies or dict())
 
         # kwargs for additional processing e.g. for middleware components
-        self.additional = kwargs
+        self.tags: ParameterDict = ParameterDict(kwargs)
 
     @property
     def is_error(self):
         raise NotImplementedError
 
     def set_headers(self, headers):
         """
```

### Comparing `pigeonpost-0.4.6/pigeon/http/request.py` & `pigeonpost-0.4.7/pigeon/http/request.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/http/response.py` & `pigeonpost-0.4.7/pigeon/http/response.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,8 +18,8 @@
     def is_error(self):
         return self.status >= 400
 
     def __str__(self):
         return f'HTTP/{self.protocol} {common.status(self.status)}\r\n{super().__str__()}'
 
     def __bytes__(self, encoding='ascii'):
-        return bytes(f'HTTP/{self.protocol} {common.status(self.status)}\r\n', encoding)+super().__bytes__(encoding)
+        return super().__bytes__(encoding)
```

### Comparing `pigeonpost-0.4.6/pigeon/middleware/auth.py` & `pigeonpost-0.4.7/pigeon/middleware/auth.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/middleware/components/__init__.py` & `pigeonpost-0.4.7/pigeon/middleware/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/middleware/components/cache_control.py` & `pigeonpost-0.4.7/pigeon/middleware/components/cache_control.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/middleware/components/component.py` & `pigeonpost-0.4.7/pigeon/middleware/components/component.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/middleware/components/connection.py` & `pigeonpost-0.4.7/pigeon/middleware/components/connection.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/middleware/components/content_negotiation.py` & `pigeonpost-0.4.7/pigeon/middleware/components/content_negotiation.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/middleware/components/cookies.py` & `pigeonpost-0.4.7/pigeon/middleware/components/cookies.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/middleware/components/cors.py` & `pigeonpost-0.4.7/pigeon/middleware/components/cors.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/middleware/components/host.py` & `pigeonpost-0.4.7/pigeon/middleware/components/host.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/middleware/components/mediafiles.py` & `pigeonpost-0.4.7/pigeon/middleware/components/mediafiles.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/middleware/components/method.py` & `pigeonpost-0.4.7/pigeon/middleware/components/method.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/middleware/components/staticfiles.py` & `pigeonpost-0.4.7/pigeon/middleware/components/staticfiles.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/middleware/conversion/converter.py` & `pigeonpost-0.4.7/pigeon/middleware/conversion/converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pigeon.conf
 from typing import Callable
 from typing import Any
 from urllib.parse import parse_qs, unquote_plus
 from email import message_from_string
 from pigeon.http import HTTPRequest, HTTPResponse
+from pigeon.utils.common import ParameterDict
 
 
 def autogenerator(view: Callable) -> Callable:
     """
     Wraps a view so that any responses generated from the view will have automatic type conversion.
     """
 
@@ -78,14 +79,23 @@
     data = message.get_payload()
     files = dict()
     if mime_type in pigeon.conf.settings.MIME_PARSERS:
         # parser returns either DATA or (DATA, FILES)
         parsed = pigeon.conf.settings.MIME_PARSERS[mime_type].parse(data, message)
         if isinstance(parsed, (list, tuple)):
             # parser returned data and files
-            data = parsed[0]
-            files = parsed[1]
+            if isinstance(parsed[0], dict):
+                data = ParameterDict(parsed[0])
+            else:
+                data = parsed[0]
+            if isinstance(parsed[1], dict):
+                files = ParameterDict(parsed[1])
+            else:
+                files = parsed[1]
         else:
             # parser returned only data
-            data = parsed
+            if isinstance(parsed, dict):
+                data = ParameterDict(parsed)
+            else:
+                data = parsed
 
     return HTTPRequest(method=method, path=path, headers=headers, get=get, data=data, files=files, protocol=protocol)
```

### Comparing `pigeonpost-0.4.6/pigeon/middleware/conversion/mime/parsers.py` & `pigeonpost-0.4.7/pigeon/middleware/conversion/mime/parsers.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/middleware/pipe.py` & `pigeonpost-0.4.7/pigeon/middleware/pipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import sys
 import pigeon.utils.logger as logger
 from pigeon.http.message import HTTPMessage
 from pigeon.http import HTTPRequest, HTTPResponse, error
 import pigeon.conf.middleware as middleware
 import pigeon.middleware.conversion.converter as converter
-from pigeon.middleware.tags import MiddlewareTags
 
 log = logger.Log('MIDDLEWARE', 'green')
 
 
 def preprocess(raw: bytes) -> HTTPResponse | HTTPRequest:
     """
     Tries to parse the raw request and checks whether the request is valid.
@@ -26,15 +25,14 @@
     if request.protocol not in middleware.HTTP_VERSIONS:
         # server doesn't understand protocol
         log.warning(f'RECEIVED REQUEST OF UNKNOWN PROTOCOL VERSION - SKIPPING')
         return error(505)
     
     # try processing the request
     try:
-        request.tags = MiddlewareTags()
         return middleware.PROCESSORS[request.protocol].preprocess(request=request)
     except Exception as e:
         sys.excepthook(None, e, None, custom_log=log, description='MIDDLEWARE FAILED WHEN PREPROCESSING REQUEST - SKIPPING')
         return error(500)
 
 
 def process(message: HTTPMessage) -> HTTPResponse:
```

### Comparing `pigeonpost-0.4.6/pigeon/middleware/processing.py` & `pigeonpost-0.4.7/pigeon/middleware/processing.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/middleware/views.py` & `pigeonpost-0.4.7/pigeon/middleware/views.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/templating/templater.py` & `pigeonpost-0.4.7/pigeon/templating/templater.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/utils/common.py` & `pigeonpost-0.4.7/pigeon/utils/common.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeon/utils/logger.py` & `pigeonpost-0.4.7/pigeon/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.6/pigeonpost.egg-info/SOURCES.txt` & `pigeonpost-0.4.7/pigeonpost.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 pigeon/http/message.py
 pigeon/http/request.py
 pigeon/http/response.py
 pigeon/middleware/__init__.py
 pigeon/middleware/auth.py
 pigeon/middleware/pipe.py
 pigeon/middleware/processing.py
-pigeon/middleware/tags.py
 pigeon/middleware/views.py
 pigeon/middleware/components/__init__.py
 pigeon/middleware/components/cache_control.py
 pigeon/middleware/components/component.py
 pigeon/middleware/components/connection.py
 pigeon/middleware/components/content_negotiation.py
 pigeon/middleware/components/cookies.py
```


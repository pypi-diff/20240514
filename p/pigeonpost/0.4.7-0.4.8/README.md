# Comparing `tmp/pigeonpost-0.4.7.tar.gz` & `tmp/pigeonpost-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonpost-0.4.7.tar", last modified: Tue May 14 12:53:32 2024, max compression
+gzip compressed data, was "pigeonpost-0.4.8.tar", last modified: Tue May 14 18:51:04 2024, max compression
```

## Comparing `pigeonpost-0.4.7.tar` & `pigeonpost-0.4.8.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.447778 pigeonpost-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 12:53:32.447778 pigeonpost-0.4.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.439777 pigeonpost-0.4.7/pigeon/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.439777 pigeonpost-0.4.7/pigeon/conf/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/conf/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/conf/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.443777 pigeonpost-0.4.7/pigeon/core/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/core/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/core/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/core/secure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/core/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.443777 pigeonpost-0.4.7/pigeon/default/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/default/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.443777 pigeonpost-0.4.7/pigeon/files/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/files/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/files/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.443777 pigeonpost-0.4.7/pigeon/http/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/http/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/http/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/http/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/http/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.443777 pigeonpost-0.4.7/pigeon/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.447778 pigeonpost-0.4.7/pigeon/middleware/components/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/cache_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/component.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/content_negotiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/date.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/mediafiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/method.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/components/staticfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.447778 pigeonpost-0.4.7/pigeon/middleware/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/conversion/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.447778 pigeonpost-0.4.7/pigeon/middleware/conversion/mime/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/conversion/mime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/conversion/mime/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/conversion/mime/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/middleware/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.447778 pigeonpost-0.4.7/pigeon/templating/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/templating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/templating/templater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.447778 pigeonpost-0.4.7/pigeon/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/utils/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3260 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/pigeon/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:53:32.447778 pigeonpost-0.4.7/pigeonpost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 12:53:32.000000 pigeonpost-0.4.7/pigeonpost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-14 12:53:32.000000 pigeonpost-0.4.7/pigeonpost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:53:32.000000 pigeonpost-0.4.7/pigeonpost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 12:53:32.000000 pigeonpost-0.4.7/pigeonpost.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 12:53:32.000000 pigeonpost-0.4.7/pigeonpost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 12:53:32.000000 pigeonpost-0.4.7/pigeonpost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-14 12:53:32.451778 pigeonpost-0.4.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-05-14 12:53:26.000000 pigeonpost-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:51:04.394444 pigeonpost-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 18:51:04.394444 pigeonpost-0.4.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:51:04.386444 pigeonpost-0.4.8/pigeon/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:51:04.386444 pigeonpost-0.4.8/pigeon/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/conf/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/conf/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:51:04.386444 pigeonpost-0.4.8/pigeon/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/core/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/core/secure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/core/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:51:04.386444 pigeonpost-0.4.8/pigeon/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/default/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:51:04.386444 pigeonpost-0.4.8/pigeon/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/files/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/files/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:51:04.390444 pigeonpost-0.4.8/pigeon/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/http/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/http/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/http/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:51:04.390444 pigeonpost-0.4.8/pigeon/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:51:04.390444 pigeonpost-0.4.8/pigeon/middleware/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/components/cache_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/components/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/components/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/components/content_negotiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/components/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/components/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/components/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/components/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/components/mediafiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/components/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/components/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/components/staticfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:51:04.394444 pigeonpost-0.4.8/pigeon/middleware/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/conversion/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:51:04.394444 pigeonpost-0.4.8/pigeon/middleware/conversion/mime/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/conversion/mime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/conversion/mime/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/conversion/mime/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/middleware/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:51:04.394444 pigeonpost-0.4.8/pigeon/templating/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/templating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/templating/templater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:51:04.394444 pigeonpost-0.4.8/pigeon/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/utils/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3260 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/pigeon/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:51:04.394444 pigeonpost-0.4.8/pigeonpost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 18:51:04.000000 pigeonpost-0.4.8/pigeonpost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-14 18:51:04.000000 pigeonpost-0.4.8/pigeonpost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:51:04.000000 pigeonpost-0.4.8/pigeonpost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 18:51:04.000000 pigeonpost-0.4.8/pigeonpost.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 18:51:04.000000 pigeonpost-0.4.8/pigeonpost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 18:51:04.000000 pigeonpost-0.4.8/pigeonpost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-14 18:51:04.394444 pigeonpost-0.4.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-05-14 18:50:58.000000 pigeonpost-0.4.8/setup.py
```

### Comparing `pigeonpost-0.4.7/pigeon/__init__.py` & `pigeonpost-0.4.8/pigeon/__init__.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/conf/manager.py` & `pigeonpost-0.4.8/pigeon/conf/manager.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/conf/settings.py` & `pigeonpost-0.4.8/pigeon/conf/settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -45,7 +45,10 @@
     'multipart/form-data': 'pigeon.middleware.conversion.mime.parsers.MultiPartFormParser',
 }
 
 # MIME GENERATORS
 MIME_GENERATORS = {
     'application/json': 'pigeon.middleware.conversion.mime.generators.JSONGenerator',
 }
+
+# CORE HANDLER SETTINGS
+DEFAULT_BUFFER_SIZE = 32768
```

### Comparing `pigeonpost-0.4.7/pigeon/core/app.py` & `pigeonpost-0.4.8/pigeon/core/app.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/core/handler.py` & `pigeonpost-0.4.8/pigeon/core/handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import socket
 import sys
 import pigeon.middleware as middleware
 import pigeon.utils.logger as logger
 from pigeon.http import HTTPRequest, HTTPResponse
+from pigeon.conf import Manager
 
 log = logger.Log('HANDLER', 'cyan')
 
 
-def receive_data(client_sock: socket.socket, size: int = 4096) -> bytes:
+def receive_data(client_sock: socket.socket, size: int = Manager.default_buffer_size) -> bytes:
     while True:
         try:
             return client_sock.recv(size)
         except BlockingIOError:
             pass
```

### Comparing `pigeonpost-0.4.7/pigeon/core/secure.py` & `pigeonpost-0.4.8/pigeon/core/secure.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/core/server.py` & `pigeonpost-0.4.8/pigeon/core/server.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/default/errors.py` & `pigeonpost-0.4.8/pigeon/default/errors.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/files/media.py` & `pigeonpost-0.4.8/pigeon/files/media.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/files/static.py` & `pigeonpost-0.4.8/pigeon/files/static.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/http/message.py` & `pigeonpost-0.4.8/pigeon/http/message.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/http/request.py` & `pigeonpost-0.4.8/pigeon/http/request.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/http/response.py` & `pigeonpost-0.4.8/pigeon/http/response.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/middleware/auth.py` & `pigeonpost-0.4.8/pigeon/middleware/auth.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/middleware/components/__init__.py` & `pigeonpost-0.4.8/pigeon/middleware/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/middleware/components/cache_control.py` & `pigeonpost-0.4.8/pigeon/middleware/components/cache_control.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/middleware/components/component.py` & `pigeonpost-0.4.8/pigeon/middleware/components/component.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/middleware/components/connection.py` & `pigeonpost-0.4.8/pigeon/middleware/components/connection.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/middleware/components/content_negotiation.py` & `pigeonpost-0.4.8/pigeon/middleware/components/content_negotiation.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/middleware/components/cookies.py` & `pigeonpost-0.4.8/pigeon/middleware/components/cookies.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/middleware/components/cors.py` & `pigeonpost-0.4.8/pigeon/middleware/components/cors.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/middleware/components/host.py` & `pigeonpost-0.4.8/pigeon/middleware/components/host.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/middleware/components/mediafiles.py` & `pigeonpost-0.4.8/pigeon/middleware/components/mediafiles.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/middleware/components/method.py` & `pigeonpost-0.4.8/pigeon/middleware/components/method.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/middleware/components/staticfiles.py` & `pigeonpost-0.4.8/pigeon/middleware/components/staticfiles.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/middleware/conversion/converter.py` & `pigeonpost-0.4.8/pigeon/middleware/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/middleware/conversion/mime/parsers.py` & `pigeonpost-0.4.8/pigeon/middleware/conversion/mime/parsers.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/middleware/pipe.py` & `pigeonpost-0.4.8/pigeon/middleware/pipe.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/middleware/processing.py` & `pigeonpost-0.4.8/pigeon/middleware/processing.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/middleware/views.py` & `pigeonpost-0.4.8/pigeon/middleware/views.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/templating/templater.py` & `pigeonpost-0.4.8/pigeon/templating/templater.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/utils/common.py` & `pigeonpost-0.4.8/pigeon/utils/common.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeon/utils/logger.py` & `pigeonpost-0.4.8/pigeon/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.7/pigeonpost.egg-info/SOURCES.txt` & `pigeonpost-0.4.8/pigeonpost.egg-info/SOURCES.txt`

 * *Files identical despite different names*


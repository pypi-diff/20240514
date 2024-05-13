# Comparing `tmp/sbn-96.tar.gz` & `tmp/sbn-97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbn-96.tar", last modified: Mon May 13 02:46:23 2024, max compression
+gzip compressed data, was "sbn-97.tar", last modified: Mon May 13 03:20:38 2024, max compression
```

## Comparing `sbn-96.tar` & `sbn-97.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 02:46:23.707057 sbn-96/
--rw-r--r--   0 bart      (1000) bart      (1001)     2494 2024-05-13 02:46:23.707057 sbn-96/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     1932 2024-05-12 05:45:59.000000 sbn-96/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 02:46:23.703057 sbn-96/docs/
--rw-r--r--   0 bart      (1000) bart      (1001)   180711 2024-05-12 05:07:36.000000 sbn-96/docs/ECHAabilify.png
--rw-r--r--   0 bart      (1000) bart      (1001)   193757 2024-05-12 05:07:36.000000 sbn-96/docs/ECHAclozapine.png
--rw-r--r--   0 bart      (1000) bart      (1001)   197697 2024-05-12 05:07:36.000000 sbn-96/docs/ECHAhaldol.png
--rw-r--r--   0 bart      (1000) bart      (1001)   232313 2024-05-12 05:07:36.000000 sbn-96/docs/ECHAzyprexa.png
--rw-r--r--   0 bart      (1000) bart      (1001)   245670 2024-05-12 05:07:36.000000 sbn-96/docs/OTP1.png
--rw-r--r--   0 bart      (1000) bart      (1001)   238095 2024-05-12 05:07:36.000000 sbn-96/docs/OTP2.png
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 02:46:23.703057 sbn-96/docs/_static/
--rw-r--r--   0 bart      (1000) bart      (1001)     1000 2024-05-12 05:07:36.000000 sbn-96/docs/_static/sbn.css
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 02:46:23.703057 sbn-96/docs/_templates/
--rw-r--r--   0 bart      (1000) bart      (1001)      291 2024-05-12 05:07:36.000000 sbn-96/docs/_templates/base.rst
--rw-r--r--   0 bart      (1000) bart      (1001)      543 2024-05-12 05:07:36.000000 sbn-96/docs/_templates/class.rst
--rw-r--r--   0 bart      (1000) bart      (1001)      879 2024-05-12 05:07:36.000000 sbn-96/docs/_templates/mine.rst
--rw-r--r--   0 bart      (1000) bart      (1001)      879 2024-05-12 05:07:36.000000 sbn-96/docs/_templates/module.rst
--rw-r--r--   0 bart      (1000) bart      (1001)     1208 2024-05-13 02:30:34.000000 sbn-96/docs/about.rst
--rw-r--r--   0 bart      (1000) bart      (1001)  1685507 2024-05-12 05:07:36.000000 sbn-96/docs/bevestigd.jpg
--rw-r--r--   0 bart      (1000) bart      (1001)     3603 2024-05-13 02:13:01.000000 sbn-96/docs/conf.py
--rw-r--r--   0 bart      (1000) bart      (1001)      600 2024-05-12 05:17:00.000000 sbn-96/docs/evidence.rst
--rw-r--r--   0 bart      (1000) bart      (1001)    47740 2024-05-13 02:42:11.000000 sbn-96/docs/genocide.png
--rw-r--r--   0 bart      (1000) bart      (1001)      364 2024-05-12 05:17:00.000000 sbn-96/docs/guilty.rst
--rw-r--r--   0 bart      (1000) bart      (1001)     2068 2024-05-13 02:15:41.000000 sbn-96/docs/index.rst
--rw-r--r--   0 bart      (1000) bart      (1001)    69979 2024-05-12 05:07:36.000000 sbn-96/docs/informed.jpg
--rw-r--r--   0 bart      (1000) bart      (1001)   228393 2024-05-12 05:07:36.000000 sbn-96/docs/kamer.png
--rw-r--r--   0 bart      (1000) bart      (1001)     3457 2024-05-12 05:49:11.000000 sbn-96/docs/manual.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 02:46:23.703057 sbn-96/docs/pdf/
--rw-r--r--   0 bart      (1000) bart      (1001)   225470 2024-05-12 05:07:36.000000 sbn-96/docs/pdf/EM_Ack_OTP-CR-117_19.pdf
--rw-r--r--   0 bart      (1000) bart      (1001)   238330 2024-05-12 05:07:36.000000 sbn-96/docs/pdf/EM_T04_OTP-CR-117_19.pdf
--rw-r--r--   0 bart      (1000) bart      (1001)   236671 2024-05-12 05:07:36.000000 sbn-96/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf
--rw-r--r--   0 bart      (1000) bart      (1001)    41559 2024-05-12 05:07:36.000000 sbn-96/docs/pdf/Kamer.pdf
--rw-r--r--   0 bart      (1000) bart      (1001)   323490 2024-05-12 05:07:36.000000 sbn-96/docs/pdf/Rome-Statute.pdf
--rw-r--r--   0 bart      (1000) bart      (1001)    50044 2024-05-12 05:07:36.000000 sbn-96/docs/pdf/bevestigd.pdf
--rw-r--r--   0 bart      (1000) bart      (1001)     2196 2024-05-12 05:17:00.000000 sbn-96/docs/request.rst
--rw-r--r--   0 bart      (1000) bart      (1001)       23 2024-05-12 05:07:36.000000 sbn-96/docs/robots.txt
--rw-r--r--   0 bart      (1000) bart      (1001)   287102 2024-05-12 05:07:36.000000 sbn-96/docs/skull3.png
--rw-r--r--   0 bart      (1000) bart      (1001)      841 2024-05-12 05:20:24.000000 sbn-96/docs/source.rst
--rw-r--r--   0 bart      (1000) bart      (1001)     1183 2024-05-12 05:17:00.000000 sbn-96/docs/writings.rst
--rw-r--r--   0 bart      (1000) bart      (1001)     1980 2024-05-13 02:44:16.000000 sbn-96/pyproject.toml
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 02:46:23.707057 sbn-96/sbn/
--rw-r--r--   0 bart      (1000) bart      (1001)       62 2024-05-12 05:08:36.000000 sbn-96/sbn/__init__.py
--rwxr-xr-x   0 bart      (1000) bart      (1001)     3913 2024-05-13 02:19:42.000000 sbn-96/sbn/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      704 2024-05-12 05:08:36.000000 sbn-96/sbn/broker.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4219 2024-05-12 05:08:36.000000 sbn-96/sbn/client.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2328 2024-05-12 05:08:36.000000 sbn-96/sbn/disk.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1954 2024-05-12 05:08:36.000000 sbn-96/sbn/find.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2110 2024-05-12 05:08:36.000000 sbn-96/sbn/handler.py
--rw-r--r--   0 bart      (1000) bart      (1001)      490 2024-05-12 05:08:36.000000 sbn-96/sbn/log.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 02:46:23.707057 sbn-96/sbn/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)      355 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      190 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      351 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1001)    18777 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)      694 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1001)      385 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2354 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1001)    10762 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1123 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1001)      991 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5163 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     6168 2024-05-12 05:08:36.000000 sbn-96/sbn/object.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1421 2024-05-12 05:08:36.000000 sbn-96/sbn/run.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4209 2024-05-12 05:08:36.000000 sbn-96/sbn/thread.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 02:46:23.707057 sbn-96/sbn.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     2494 2024-05-13 02:46:23.000000 sbn-96/sbn.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     1240 2024-05-13 02:46:23.000000 sbn-96/sbn.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-13 02:46:23.000000 sbn-96/sbn.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)       74 2024-05-13 02:46:23.000000 sbn-96/sbn.egg-info/entry_points.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        7 2024-05-13 02:46:23.000000 sbn-96/sbn.egg-info/requires.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        4 2024-05-13 02:46:23.000000 sbn-96/sbn.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-13 02:46:03.000000 sbn-96/sbn.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2024-05-13 02:46:23.707057 sbn-96/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)      192 2024-05-12 05:07:36.000000 sbn-96/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 03:20:38.115005 sbn-97/
+-rw-r--r--   0 bart      (1000) bart      (1001)     2494 2024-05-13 03:20:38.115005 sbn-97/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     1932 2024-05-12 05:45:59.000000 sbn-97/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 03:20:38.111005 sbn-97/docs/
+-rw-r--r--   0 bart      (1000) bart      (1001)   180711 2024-05-12 05:07:36.000000 sbn-97/docs/ECHAabilify.png
+-rw-r--r--   0 bart      (1000) bart      (1001)   193757 2024-05-12 05:07:36.000000 sbn-97/docs/ECHAclozapine.png
+-rw-r--r--   0 bart      (1000) bart      (1001)   197697 2024-05-12 05:07:36.000000 sbn-97/docs/ECHAhaldol.png
+-rw-r--r--   0 bart      (1000) bart      (1001)   232313 2024-05-12 05:07:36.000000 sbn-97/docs/ECHAzyprexa.png
+-rw-r--r--   0 bart      (1000) bart      (1001)   245670 2024-05-12 05:07:36.000000 sbn-97/docs/OTP1.png
+-rw-r--r--   0 bart      (1000) bart      (1001)   238095 2024-05-12 05:07:36.000000 sbn-97/docs/OTP2.png
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 03:20:38.111005 sbn-97/docs/_static/
+-rw-r--r--   0 bart      (1000) bart      (1001)     1000 2024-05-12 05:07:36.000000 sbn-97/docs/_static/sbn.css
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 03:20:38.111005 sbn-97/docs/_templates/
+-rw-r--r--   0 bart      (1000) bart      (1001)      291 2024-05-12 05:07:36.000000 sbn-97/docs/_templates/base.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)      543 2024-05-12 05:07:36.000000 sbn-97/docs/_templates/class.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)      879 2024-05-12 05:07:36.000000 sbn-97/docs/_templates/mine.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)      879 2024-05-12 05:07:36.000000 sbn-97/docs/_templates/module.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)     1208 2024-05-13 02:30:34.000000 sbn-97/docs/about.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)  1685507 2024-05-12 05:07:36.000000 sbn-97/docs/bevestigd.jpg
+-rw-r--r--   0 bart      (1000) bart      (1001)     3603 2024-05-13 02:13:01.000000 sbn-97/docs/conf.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      600 2024-05-12 05:17:00.000000 sbn-97/docs/evidence.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)    47740 2024-05-13 02:42:11.000000 sbn-97/docs/genocide.png
+-rw-r--r--   0 bart      (1000) bart      (1001)      364 2024-05-12 05:17:00.000000 sbn-97/docs/guilty.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)     2068 2024-05-13 02:15:41.000000 sbn-97/docs/index.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)    69979 2024-05-12 05:07:36.000000 sbn-97/docs/informed.jpg
+-rw-r--r--   0 bart      (1000) bart      (1001)   228393 2024-05-12 05:07:36.000000 sbn-97/docs/kamer.png
+-rw-r--r--   0 bart      (1000) bart      (1001)     3457 2024-05-12 05:49:11.000000 sbn-97/docs/manual.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 03:20:38.111005 sbn-97/docs/pdf/
+-rw-r--r--   0 bart      (1000) bart      (1001)   225470 2024-05-12 05:07:36.000000 sbn-97/docs/pdf/EM_Ack_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)   238330 2024-05-12 05:07:36.000000 sbn-97/docs/pdf/EM_T04_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)   236671 2024-05-12 05:07:36.000000 sbn-97/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)    41559 2024-05-12 05:07:36.000000 sbn-97/docs/pdf/Kamer.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)   323490 2024-05-12 05:07:36.000000 sbn-97/docs/pdf/Rome-Statute.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)    50044 2024-05-12 05:07:36.000000 sbn-97/docs/pdf/bevestigd.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)     2196 2024-05-12 05:17:00.000000 sbn-97/docs/request.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)       23 2024-05-12 05:07:36.000000 sbn-97/docs/robots.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)   287102 2024-05-12 05:07:36.000000 sbn-97/docs/skull3.png
+-rw-r--r--   0 bart      (1000) bart      (1001)      841 2024-05-12 05:20:24.000000 sbn-97/docs/source.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)     1183 2024-05-12 05:17:00.000000 sbn-97/docs/writings.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)     1980 2024-05-13 03:12:07.000000 sbn-97/pyproject.toml
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 03:20:38.111005 sbn-97/sbn/
+-rw-r--r--   0 bart      (1000) bart      (1001)       62 2024-05-12 05:08:36.000000 sbn-97/sbn/__init__.py
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     3945 2024-05-13 03:12:17.000000 sbn-97/sbn/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      704 2024-05-12 05:08:36.000000 sbn-97/sbn/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4219 2024-05-12 05:08:36.000000 sbn-97/sbn/client.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2328 2024-05-12 05:08:36.000000 sbn-97/sbn/disk.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1954 2024-05-12 05:08:36.000000 sbn-97/sbn/find.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2110 2024-05-12 05:08:36.000000 sbn-97/sbn/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      490 2024-05-12 05:08:36.000000 sbn-97/sbn/log.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 03:20:38.115005 sbn-97/sbn/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)      355 2024-05-12 05:08:41.000000 sbn-97/sbn/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      190 2024-05-12 05:08:41.000000 sbn-97/sbn/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      351 2024-05-12 05:08:41.000000 sbn-97/sbn/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    18777 2024-05-12 05:08:41.000000 sbn-97/sbn/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      694 2024-05-12 05:08:41.000000 sbn-97/sbn/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      385 2024-05-12 05:08:41.000000 sbn-97/sbn/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2354 2024-05-12 05:08:41.000000 sbn-97/sbn/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    10762 2024-05-12 05:08:41.000000 sbn-97/sbn/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1123 2024-05-12 05:08:41.000000 sbn-97/sbn/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      991 2024-05-12 05:08:41.000000 sbn-97/sbn/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     5163 2024-05-12 05:08:41.000000 sbn-97/sbn/modules/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     6168 2024-05-12 05:08:36.000000 sbn-97/sbn/object.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1421 2024-05-12 05:08:36.000000 sbn-97/sbn/run.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4209 2024-05-12 05:08:36.000000 sbn-97/sbn/thread.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 03:20:38.111005 sbn-97/sbn.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     2494 2024-05-13 03:20:38.000000 sbn-97/sbn.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     1240 2024-05-13 03:20:38.000000 sbn-97/sbn.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-13 03:20:38.000000 sbn-97/sbn.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)       74 2024-05-13 03:20:38.000000 sbn-97/sbn.egg-info/entry_points.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        7 2024-05-13 03:20:38.000000 sbn-97/sbn.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        4 2024-05-13 03:20:38.000000 sbn-97/sbn.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-13 03:20:38.000000 sbn-97/sbn.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2024-05-13 03:20:38.115005 sbn-97/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)      192 2024-05-12 05:07:36.000000 sbn-97/setup.py
```

### Comparing `sbn-96/PKG-INFO` & `sbn-97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbn
-Version: 96
+Version: 97
 Summary: Skull, Bones and Number (OTP-CR-117/19)
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/sbn
 Project-URL: bugs, https://github.com/bthate/sbn/issues
 Project-URL: source, https://github.com/bthate/sbn
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sbn-96/README.rst` & `sbn-97/README.rst`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/ECHAabilify.png` & `sbn-97/docs/ECHAabilify.png`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/ECHAclozapine.png` & `sbn-97/docs/ECHAclozapine.png`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/ECHAhaldol.png` & `sbn-97/docs/ECHAhaldol.png`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/ECHAzyprexa.png` & `sbn-97/docs/ECHAzyprexa.png`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/OTP1.png` & `sbn-97/docs/OTP1.png`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/OTP2.png` & `sbn-97/docs/OTP2.png`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/_static/sbn.css` & `sbn-97/docs/_static/sbn.css`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/_templates/class.rst` & `sbn-97/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/_templates/mine.rst` & `sbn-97/docs/_templates/mine.rst`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/_templates/module.rst` & `sbn-97/docs/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/about.rst` & `sbn-97/docs/about.rst`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/bevestigd.jpg` & `sbn-97/docs/bevestigd.jpg`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/conf.py` & `sbn-97/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/evidence.rst` & `sbn-97/docs/evidence.rst`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/genocide.png` & `sbn-97/docs/genocide.png`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/index.rst` & `sbn-97/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/informed.jpg` & `sbn-97/docs/informed.jpg`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/kamer.png` & `sbn-97/docs/kamer.png`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/manual.rst` & `sbn-97/docs/manual.rst`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/pdf/EM_Ack_OTP-CR-117_19.pdf` & `sbn-97/docs/pdf/EM_Ack_OTP-CR-117_19.pdf`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/pdf/EM_T04_OTP-CR-117_19.pdf` & `sbn-97/docs/pdf/EM_T04_OTP-CR-117_19.pdf`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf` & `sbn-97/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/pdf/Kamer.pdf` & `sbn-97/docs/pdf/Kamer.pdf`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/pdf/Rome-Statute.pdf` & `sbn-97/docs/pdf/Rome-Statute.pdf`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/pdf/bevestigd.pdf` & `sbn-97/docs/pdf/bevestigd.pdf`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/request.rst` & `sbn-97/docs/request.rst`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/skull3.png` & `sbn-97/docs/skull3.png`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/source.rst` & `sbn-97/docs/source.rst`

 * *Files identical despite different names*

### Comparing `sbn-96/docs/writings.rst` & `sbn-97/docs/writings.rst`

 * *Files identical despite different names*

### Comparing `sbn-96/pyproject.toml` & `sbn-97/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "sbn"
 description = "Skull, Bones and Number (OTP-CR-117/19)"
-version = "96"
+version = "97"
 authors = [
     {name = "Bart Thate", email = "bthate@dds.nl" },
 ]
 readme = "README.rst"
 license = { text="Public Domain"}
 classifiers=[
     'Development Status :: 3 - Alpha',
```

### Comparing `sbn-96/sbn/__main__.py` & `sbn-97/sbn/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 
 Cfg             = Default()
 Cfg.dis         = ""
 Cfg.mod         = "cmd,err,log,mod,req,tdo,thr,tmr"
 Cfg.opts        = ""
 Cfg.name        = "sbn"
-Cfg.version     = "96"
+Cfg.version     = "97"
 Cfg.wdr         = os.path.expanduser(f"~/.{Cfg.name}")
 Cfg.pidfile     = os.path.join(Cfg.wdr, f"{Cfg.name}.pid")
 
 
 Workdir.workdir = Cfg.wdr
 
 
@@ -125,14 +125,19 @@
     except (KeyboardInterrupt, EOFError):
         print("")
     finally:
         if old2:
             termios.tcsetattr(sys.stdin.fileno(), termios.TCSADRAIN, old2)
 
 
+def wrapped():
+    main()
+    errors()
+
+
 def main():
     "main"
     parse(Cfg, " ".join(sys.argv[1:]))
     skel()
     if not "d" in Cfg.opts:
         enable(print)
         setout(print)
@@ -161,9 +166,9 @@
         while 1:
             time.sleep(1.0)
     elif Cfg.otxt:
         cmnd(Cfg.otxt, print)
 
 
 if __name__ == "__main__":
-    main()
-    errors()
+    wrapped()
+
```

### Comparing `sbn-96/sbn/broker.py` & `sbn-97/sbn/broker.py`

 * *Files identical despite different names*

### Comparing `sbn-96/sbn/client.py` & `sbn-97/sbn/client.py`

 * *Files identical despite different names*

### Comparing `sbn-96/sbn/disk.py` & `sbn-97/sbn/disk.py`

 * *Files identical despite different names*

### Comparing `sbn-96/sbn/find.py` & `sbn-97/sbn/find.py`

 * *Files identical despite different names*

### Comparing `sbn-96/sbn/handler.py` & `sbn-97/sbn/handler.py`

 * *Files identical despite different names*

### Comparing `sbn-96/sbn/modules/irc.py` & `sbn-97/sbn/modules/irc.py`

 * *Files identical despite different names*

### Comparing `sbn-96/sbn/modules/log.py` & `sbn-97/sbn/modules/log.py`

 * *Files identical despite different names*

### Comparing `sbn-96/sbn/modules/req.py` & `sbn-97/sbn/modules/req.py`

 * *Files identical despite different names*

### Comparing `sbn-96/sbn/modules/rss.py` & `sbn-97/sbn/modules/rss.py`

 * *Files identical despite different names*

### Comparing `sbn-96/sbn/modules/tdo.py` & `sbn-97/sbn/modules/tdo.py`

 * *Files identical despite different names*

### Comparing `sbn-96/sbn/modules/thr.py` & `sbn-97/sbn/modules/thr.py`

 * *Files identical despite different names*

### Comparing `sbn-96/sbn/modules/tmr.py` & `sbn-97/sbn/modules/tmr.py`

 * *Files identical despite different names*

### Comparing `sbn-96/sbn/object.py` & `sbn-97/sbn/object.py`

 * *Files identical despite different names*

### Comparing `sbn-96/sbn/run.py` & `sbn-97/sbn/run.py`

 * *Files identical despite different names*

### Comparing `sbn-96/sbn/thread.py` & `sbn-97/sbn/thread.py`

 * *Files identical despite different names*

### Comparing `sbn-96/sbn.egg-info/PKG-INFO` & `sbn-97/sbn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbn
-Version: 96
+Version: 97
 Summary: Skull, Bones and Number (OTP-CR-117/19)
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/sbn
 Project-URL: bugs, https://github.com/bthate/sbn/issues
 Project-URL: source, https://github.com/bthate/sbn
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sbn-96/sbn.egg-info/SOURCES.txt` & `sbn-97/sbn.egg-info/SOURCES.txt`

 * *Files identical despite different names*


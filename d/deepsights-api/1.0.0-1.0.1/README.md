# Comparing `tmp/deepsights-api-1.0.0.tar.gz` & `tmp/deepsights-api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsights-api-1.0.0.tar", last modified: Tue Mar 26 11:02:29 2024, max compression
+gzip compressed data, was "deepsights-api-1.0.1.tar", last modified: Tue May 14 15:16:47 2024, max compression
```

## Comparing `deepsights-api-1.0.0.tar` & `deepsights-api-1.0.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.558900 deepsights-api-1.0.0/
--rw-r--r--   0 0x1af      (501) staff       (20)    11356 2024-03-12 21:03:07.000000 deepsights-api-1.0.0/LICENSE
--rw-r--r--   0 0x1af      (501) staff       (20)     4754 2024-03-26 11:02:29.558656 deepsights-api-1.0.0/PKG-INFO
--rw-r--r--   0 0x1af      (501) staff       (20)     3839 2024-03-26 10:34:35.000000 deepsights-api-1.0.0/README.md
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.551501 deepsights-api-1.0.0/deepsights/
--rw-r--r--   0 0x1af      (501) staff       (20)      851 2024-03-25 16:53:44.000000 deepsights-api-1.0.0/deepsights/__init__.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.551884 deepsights-api-1.0.0/deepsights/api/
--rw-r--r--   0 0x1af      (501) staff       (20)      786 2024-03-25 15:56:22.000000 deepsights-api-1.0.0/deepsights/api/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     7798 2024-03-25 17:49:54.000000 deepsights-api-1.0.0/deepsights/api/api.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1161 2024-03-24 07:09:55.000000 deepsights-api-1.0.0/deepsights/api/resource.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.552127 deepsights-api-1.0.0/deepsights/contentstore/
--rw-r--r--   0 0x1af      (501) staff       (20)      741 2024-03-24 07:36:24.000000 deepsights-api-1.0.0/deepsights/contentstore/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1672 2024-03-25 17:23:37.000000 deepsights-api-1.0.0/deepsights/contentstore/contentstore.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.552820 deepsights-api-1.0.0/deepsights/contentstore/resources/
--rw-r--r--   0 0x1af      (501) staff       (20)      851 2024-03-25 17:24:10.000000 deepsights-api-1.0.0/deepsights/contentstore/resources/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     2168 2024-03-24 07:22:59.000000 deepsights-api-1.0.0/deepsights/contentstore/resources/_model.py
--rw-r--r--   0 0x1af      (501) staff       (20)     7011 2024-03-24 08:05:42.000000 deepsights-api-1.0.0/deepsights/contentstore/resources/_search.py
--rw-r--r--   0 0x1af      (501) staff       (20)     5586 2024-03-24 07:22:46.000000 deepsights-api-1.0.0/deepsights/contentstore/resources/news.py
--rw-r--r--   0 0x1af      (501) staff       (20)     5666 2024-03-24 08:12:21.000000 deepsights-api-1.0.0/deepsights/contentstore/resources/secondary.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.553197 deepsights-api-1.0.0/deepsights/deepsights/
--rw-r--r--   0 0x1af      (501) staff       (20)      735 2024-03-25 16:48:54.000000 deepsights-api-1.0.0/deepsights/deepsights/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     2861 2024-03-25 17:30:36.000000 deepsights-api-1.0.0/deepsights/deepsights/_mip_identity.py
--rw-r--r--   0 0x1af      (501) staff       (20)     3327 2024-03-25 17:51:00.000000 deepsights-api-1.0.0/deepsights/deepsights/deepsights.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.553304 deepsights-api-1.0.0/deepsights/deepsights/resources/
--rw-r--r--   0 0x1af      (501) staff       (20)      766 2024-03-25 16:48:34.000000 deepsights-api-1.0.0/deepsights/deepsights/resources/__init__.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.553629 deepsights-api-1.0.0/deepsights/deepsights/resources/quota/
--rw-r--r--   0 0x1af      (501) staff       (20)      847 2024-03-25 16:44:48.000000 deepsights-api-1.0.0/deepsights/deepsights/resources/quota/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     3311 2024-03-12 21:03:07.000000 deepsights-api-1.0.0/deepsights/deepsights/resources/quota/_model.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1893 2024-03-25 16:44:57.000000 deepsights-api-1.0.0/deepsights/deepsights/resources/quota/quota.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.553877 deepsights-api-1.0.0/deepsights/documentstore/
--rw-r--r--   0 0x1af      (501) staff       (20)      847 2024-03-25 17:24:56.000000 deepsights-api-1.0.0/deepsights/documentstore/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1607 2024-03-25 17:25:25.000000 deepsights-api-1.0.0/deepsights/documentstore/documentstore.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.554002 deepsights-api-1.0.0/deepsights/documentstore/resources/
--rw-r--r--   0 0x1af      (501) staff       (20)      828 2024-03-25 17:25:49.000000 deepsights-api-1.0.0/deepsights/documentstore/resources/__init__.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.555548 deepsights-api-1.0.0/deepsights/documentstore/resources/documents/
--rw-r--r--   0 0x1af      (501) staff       (20)      880 2024-03-25 16:42:51.000000 deepsights-api-1.0.0/deepsights/documentstore/resources/documents/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1232 2024-03-24 08:05:24.000000 deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_cache.py
--rw-r--r--   0 0x1af      (501) staff       (20)     2841 2024-03-25 16:42:51.000000 deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_delete.py
--rw-r--r--   0 0x1af      (501) staff       (20)     2510 2024-03-25 16:42:51.000000 deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_download.py
--rw-r--r--   0 0x1af      (501) staff       (20)     3269 2024-03-25 16:42:51.000000 deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_list.py
--rw-r--r--   0 0x1af      (501) staff       (20)     5406 2024-03-25 16:42:51.000000 deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_load.py
--rw-r--r--   0 0x1af      (501) staff       (20)     5582 2024-03-25 16:42:51.000000 deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_model.py
--rw-r--r--   0 0x1af      (501) staff       (20)     6823 2024-03-25 16:42:51.000000 deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_search.py
--rw-r--r--   0 0x1af      (501) staff       (20)     3378 2024-03-12 21:03:07.000000 deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_segmenter.py
--rw-r--r--   0 0x1af      (501) staff       (20)     4560 2024-03-25 16:42:51.000000 deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_upload.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1923 2024-03-25 16:42:51.000000 deepsights-api-1.0.0/deepsights/documentstore/resources/documents/documents.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.555825 deepsights-api-1.0.0/deepsights/userclient/
--rw-r--r--   0 0x1af      (501) staff       (20)      756 2024-03-25 17:33:09.000000 deepsights-api-1.0.0/deepsights/userclient/__init__.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.556029 deepsights-api-1.0.0/deepsights/userclient/minions/
--rw-r--r--   0 0x1af      (501) staff       (20)        0 2024-03-12 21:03:07.000000 deepsights-api-1.0.0/deepsights/userclient/minions/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1900 2024-03-24 08:06:13.000000 deepsights-api-1.0.0/deepsights/userclient/minions/_minions.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.556146 deepsights-api-1.0.0/deepsights/userclient/resources/
--rw-r--r--   0 0x1af      (501) staff       (20)      833 2024-03-25 17:32:47.000000 deepsights-api-1.0.0/deepsights/userclient/resources/__init__.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.556514 deepsights-api-1.0.0/deepsights/userclient/resources/answers/
--rw-r--r--   0 0x1af      (501) staff       (20)      774 2024-03-25 17:31:44.000000 deepsights-api-1.0.0/deepsights/userclient/resources/answers/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     4057 2024-03-25 18:15:10.000000 deepsights-api-1.0.0/deepsights/userclient/resources/answers/_model.py
--rw-r--r--   0 0x1af      (501) staff       (20)     4365 2024-03-25 18:12:47.000000 deepsights-api-1.0.0/deepsights/userclient/resources/answers/answer.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.556918 deepsights-api-1.0.0/deepsights/userclient/resources/reports/
--rw-r--r--   0 0x1af      (501) staff       (20)      775 2024-03-25 17:33:28.000000 deepsights-api-1.0.0/deepsights/userclient/resources/reports/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     5004 2024-03-25 18:22:13.000000 deepsights-api-1.0.0/deepsights/userclient/resources/reports/_model.py
--rw-r--r--   0 0x1af      (501) staff       (20)     4739 2024-03-26 10:43:01.000000 deepsights-api-1.0.0/deepsights/userclient/resources/reports/report.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1547 2024-03-25 17:32:59.000000 deepsights-api-1.0.0/deepsights/userclient/userclient.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.557549 deepsights-api-1.0.0/deepsights/utils/
--rw-r--r--   0 0x1af      (501) staff       (20)     1062 2024-03-12 21:03:07.000000 deepsights-api-1.0.0/deepsights/utils/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1995 2024-03-12 21:03:07.000000 deepsights-api-1.0.0/deepsights/utils/_cache.py
--rw-r--r--   0 0x1af      (501) staff       (20)     5901 2024-03-23 10:16:37.000000 deepsights-api-1.0.0/deepsights/utils/_ranking.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1543 2024-03-12 21:03:07.000000 deepsights-api-1.0.0/deepsights/utils/_utils.py
--rw-r--r--   0 0x1af      (501) staff       (20)     2750 2024-03-12 21:03:07.000000 deepsights-api-1.0.0/deepsights/utils/model.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-03-26 11:02:29.558317 deepsights-api-1.0.0/deepsights_api.egg-info/
--rw-r--r--   0 0x1af      (501) staff       (20)     4754 2024-03-26 11:02:29.000000 deepsights-api-1.0.0/deepsights_api.egg-info/PKG-INFO
--rw-r--r--   0 0x1af      (501) staff       (20)     2296 2024-03-26 11:02:29.000000 deepsights-api-1.0.0/deepsights_api.egg-info/SOURCES.txt
--rw-r--r--   0 0x1af      (501) staff       (20)        1 2024-03-26 11:02:29.000000 deepsights-api-1.0.0/deepsights_api.egg-info/dependency_links.txt
--rw-r--r--   0 0x1af      (501) staff       (20)      117 2024-03-26 11:02:29.000000 deepsights-api-1.0.0/deepsights_api.egg-info/requires.txt
--rw-r--r--   0 0x1af      (501) staff       (20)       11 2024-03-26 11:02:29.000000 deepsights-api-1.0.0/deepsights_api.egg-info/top_level.txt
--rw-r--r--   0 0x1af      (501) staff       (20)       38 2024-03-26 11:02:29.558954 deepsights-api-1.0.0/setup.cfg
--rw-r--r--   0 0x1af      (501) staff       (20)     2023 2024-03-26 10:59:04.000000 deepsights-api-1.0.0/setup.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.025529 deepsights-api-1.0.1/
+-rw-r--r--   0 0x1af      (501) staff       (20)    11356 2024-03-12 21:03:07.000000 deepsights-api-1.0.1/LICENSE
+-rw-r--r--   0 0x1af      (501) staff       (20)     4754 2024-05-14 15:16:47.025310 deepsights-api-1.0.1/PKG-INFO
+-rw-r--r--   0 0x1af      (501) staff       (20)     3839 2024-03-26 10:34:35.000000 deepsights-api-1.0.1/README.md
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.017016 deepsights-api-1.0.1/deepsights/
+-rw-r--r--   0 0x1af      (501) staff       (20)      851 2024-03-25 16:53:44.000000 deepsights-api-1.0.1/deepsights/__init__.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.017470 deepsights-api-1.0.1/deepsights/api/
+-rw-r--r--   0 0x1af      (501) staff       (20)      786 2024-03-25 15:56:22.000000 deepsights-api-1.0.1/deepsights/api/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     7798 2024-03-25 17:49:54.000000 deepsights-api-1.0.1/deepsights/api/api.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1161 2024-03-24 07:09:55.000000 deepsights-api-1.0.1/deepsights/api/resource.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.017755 deepsights-api-1.0.1/deepsights/contentstore/
+-rw-r--r--   0 0x1af      (501) staff       (20)      741 2024-03-24 07:36:24.000000 deepsights-api-1.0.1/deepsights/contentstore/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1672 2024-03-25 17:23:37.000000 deepsights-api-1.0.1/deepsights/contentstore/contentstore.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.018674 deepsights-api-1.0.1/deepsights/contentstore/resources/
+-rw-r--r--   0 0x1af      (501) staff       (20)      851 2024-03-25 17:24:10.000000 deepsights-api-1.0.1/deepsights/contentstore/resources/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     2168 2024-03-24 07:22:59.000000 deepsights-api-1.0.1/deepsights/contentstore/resources/_model.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     7657 2024-05-14 14:43:02.000000 deepsights-api-1.0.1/deepsights/contentstore/resources/_search.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     6036 2024-05-14 14:43:51.000000 deepsights-api-1.0.1/deepsights/contentstore/resources/news.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     6116 2024-05-14 14:44:21.000000 deepsights-api-1.0.1/deepsights/contentstore/resources/secondary.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.019068 deepsights-api-1.0.1/deepsights/deepsights/
+-rw-r--r--   0 0x1af      (501) staff       (20)      735 2024-03-25 16:48:54.000000 deepsights-api-1.0.1/deepsights/deepsights/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     2861 2024-03-25 17:30:36.000000 deepsights-api-1.0.1/deepsights/deepsights/_mip_identity.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     3327 2024-03-25 17:51:00.000000 deepsights-api-1.0.1/deepsights/deepsights/deepsights.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.019244 deepsights-api-1.0.1/deepsights/deepsights/resources/
+-rw-r--r--   0 0x1af      (501) staff       (20)      766 2024-03-25 16:48:34.000000 deepsights-api-1.0.1/deepsights/deepsights/resources/__init__.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.019899 deepsights-api-1.0.1/deepsights/deepsights/resources/quota/
+-rw-r--r--   0 0x1af      (501) staff       (20)      847 2024-03-25 16:44:48.000000 deepsights-api-1.0.1/deepsights/deepsights/resources/quota/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     3311 2024-03-12 21:03:07.000000 deepsights-api-1.0.1/deepsights/deepsights/resources/quota/_model.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1893 2024-03-25 16:44:57.000000 deepsights-api-1.0.1/deepsights/deepsights/resources/quota/quota.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.020171 deepsights-api-1.0.1/deepsights/documentstore/
+-rw-r--r--   0 0x1af      (501) staff       (20)      847 2024-03-25 17:24:56.000000 deepsights-api-1.0.1/deepsights/documentstore/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1607 2024-03-25 17:25:25.000000 deepsights-api-1.0.1/deepsights/documentstore/documentstore.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.020293 deepsights-api-1.0.1/deepsights/documentstore/resources/
+-rw-r--r--   0 0x1af      (501) staff       (20)      828 2024-03-25 17:25:49.000000 deepsights-api-1.0.1/deepsights/documentstore/resources/__init__.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.021788 deepsights-api-1.0.1/deepsights/documentstore/resources/documents/
+-rw-r--r--   0 0x1af      (501) staff       (20)      880 2024-03-25 16:42:51.000000 deepsights-api-1.0.1/deepsights/documentstore/resources/documents/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1232 2024-03-24 08:05:24.000000 deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_cache.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     2841 2024-03-25 16:42:51.000000 deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_delete.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     2510 2024-03-25 16:42:51.000000 deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_download.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     3269 2024-03-25 16:42:51.000000 deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_list.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     5406 2024-03-25 16:42:51.000000 deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_load.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     5582 2024-03-25 16:42:51.000000 deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_model.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     6823 2024-03-25 16:42:51.000000 deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_search.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     3378 2024-03-12 21:03:07.000000 deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_segmenter.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     4560 2024-03-25 16:42:51.000000 deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_upload.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1923 2024-03-25 16:42:51.000000 deepsights-api-1.0.1/deepsights/documentstore/resources/documents/documents.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.022040 deepsights-api-1.0.1/deepsights/userclient/
+-rw-r--r--   0 0x1af      (501) staff       (20)      756 2024-03-25 17:33:09.000000 deepsights-api-1.0.1/deepsights/userclient/__init__.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.022240 deepsights-api-1.0.1/deepsights/userclient/minions/
+-rw-r--r--   0 0x1af      (501) staff       (20)        0 2024-03-12 21:03:07.000000 deepsights-api-1.0.1/deepsights/userclient/minions/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1900 2024-03-24 08:06:13.000000 deepsights-api-1.0.1/deepsights/userclient/minions/_minions.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.022362 deepsights-api-1.0.1/deepsights/userclient/resources/
+-rw-r--r--   0 0x1af      (501) staff       (20)      833 2024-03-25 17:32:47.000000 deepsights-api-1.0.1/deepsights/userclient/resources/__init__.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.022713 deepsights-api-1.0.1/deepsights/userclient/resources/answers/
+-rw-r--r--   0 0x1af      (501) staff       (20)      774 2024-03-25 17:31:44.000000 deepsights-api-1.0.1/deepsights/userclient/resources/answers/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     4057 2024-03-25 18:15:10.000000 deepsights-api-1.0.1/deepsights/userclient/resources/answers/_model.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     4365 2024-03-25 18:12:47.000000 deepsights-api-1.0.1/deepsights/userclient/resources/answers/answer.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.023487 deepsights-api-1.0.1/deepsights/userclient/resources/reports/
+-rw-r--r--   0 0x1af      (501) staff       (20)      775 2024-03-25 17:33:28.000000 deepsights-api-1.0.1/deepsights/userclient/resources/reports/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     5004 2024-03-25 18:22:13.000000 deepsights-api-1.0.1/deepsights/userclient/resources/reports/_model.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     4739 2024-03-26 10:43:01.000000 deepsights-api-1.0.1/deepsights/userclient/resources/reports/report.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1547 2024-03-25 17:32:59.000000 deepsights-api-1.0.1/deepsights/userclient/userclient.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.024215 deepsights-api-1.0.1/deepsights/utils/
+-rw-r--r--   0 0x1af      (501) staff       (20)     1062 2024-03-12 21:03:07.000000 deepsights-api-1.0.1/deepsights/utils/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1995 2024-03-12 21:03:07.000000 deepsights-api-1.0.1/deepsights/utils/_cache.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     5901 2024-03-23 10:16:37.000000 deepsights-api-1.0.1/deepsights/utils/_ranking.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1543 2024-03-12 21:03:07.000000 deepsights-api-1.0.1/deepsights/utils/_utils.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     2750 2024-03-12 21:03:07.000000 deepsights-api-1.0.1/deepsights/utils/model.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-14 15:16:47.025016 deepsights-api-1.0.1/deepsights_api.egg-info/
+-rw-r--r--   0 0x1af      (501) staff       (20)     4754 2024-05-14 15:16:46.000000 deepsights-api-1.0.1/deepsights_api.egg-info/PKG-INFO
+-rw-r--r--   0 0x1af      (501) staff       (20)     2296 2024-05-14 15:16:47.000000 deepsights-api-1.0.1/deepsights_api.egg-info/SOURCES.txt
+-rw-r--r--   0 0x1af      (501) staff       (20)        1 2024-05-14 15:16:46.000000 deepsights-api-1.0.1/deepsights_api.egg-info/dependency_links.txt
+-rw-r--r--   0 0x1af      (501) staff       (20)      117 2024-05-14 15:16:46.000000 deepsights-api-1.0.1/deepsights_api.egg-info/requires.txt
+-rw-r--r--   0 0x1af      (501) staff       (20)       11 2024-05-14 15:16:46.000000 deepsights-api-1.0.1/deepsights_api.egg-info/top_level.txt
+-rw-r--r--   0 0x1af      (501) staff       (20)       38 2024-05-14 15:16:47.025576 deepsights-api-1.0.1/setup.cfg
+-rw-r--r--   0 0x1af      (501) staff       (20)     2023 2024-05-14 15:16:27.000000 deepsights-api-1.0.1/setup.py
```

### Comparing `deepsights-api-1.0.0/LICENSE` & `deepsights-api-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/PKG-INFO` & `deepsights-api-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsights-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library for the DeepSights APIs
 Home-page: https://github.com/marketlogicsoftware/deepsights-api
 Author: Market Logic Software
 Author-email: info@marketlogicsoftware.com
 License: Apache 2.0
 Project-URL: Documentation, https://marketlogicsoftware.github.io/deepsights-api/
 Classifier: Intended Audience :: Developers
```

### Comparing `deepsights-api-1.0.0/README.md` & `deepsights-api-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/__init__.py` & `deepsights-api-1.0.1/deepsights/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/api/__init__.py` & `deepsights-api-1.0.1/deepsights/api/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/api/api.py` & `deepsights-api-1.0.1/deepsights/api/api.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/api/resource.py` & `deepsights-api-1.0.1/deepsights/api/resource.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/contentstore/__init__.py` & `deepsights-api-1.0.1/deepsights/contentstore/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/contentstore/contentstore.py` & `deepsights-api-1.0.1/deepsights/contentstore/contentstore.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/contentstore/resources/__init__.py` & `deepsights-api-1.0.1/deepsights/contentstore/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/contentstore/resources/_model.py` & `deepsights-api-1.0.1/deepsights/contentstore/resources/_model.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/contentstore/resources/_search.py` & `deepsights-api-1.0.1/deepsights/contentstore/resources/_search.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 """
 This module contains the base functions to search the ContentStore.
 """
 
 from typing import List
+from datetime import datetime
 from pydantic import BaseModel
 from deepsights.api import API
 from deepsights.utils import (
     promote_exact_matches,
     rerank_by_recency,
 )
 
@@ -33,14 +34,16 @@
     search_result: BaseModel,
     max_results: int = 100,
     min_vector_score: float = 0.7,
     vector_fraction: float = 0.9,
     vector_weight: float = 0.9,
     recency_weight: float = 0.4,
     promote_exact_match: bool = False,
+    search_from_timestamp: datetime = None,
+    search_to_timestamp: datetime = None,
 ):
     """
     Perform a contentstore hybrid search using the provided query.
 
     Args:
 
         api (API): The DeepSights API instance.
@@ -49,38 +52,48 @@
         search_result (BaseModel): The model to use for parsing search results.
         max_results (int, optional): The maximum number of search results to return. Defaults to 100.
         min_vector_score (float, optional): The minimum score threshold for search results. Defaults to 0.7.
         vector_fraction (float, optional): The fraction of the search results to be vector-based. Defaults to 0.9.
         vector_weight (float, optional): The weight to apply to vector search in result ranking. Defaults to 0.9.
         recency_weight (float, optional): The weight to apply to recency in result ranking. Defaults to 0.4.
         promote_exact_match (bool, optional): Whether to promote exact matches to the top of the results. Defaults to False.
+        search_from_timestamp (datetime, optional): The start timestamp for the search. Defaults to None.
+        search_to_timestamp (datetime, optional): The end timestamp for the search. Defaults to None.
 
     Returns:
 
         List[BaseModel]: The re-ranked search results.
     """
     assert query, "The 'query' argument is required."
     assert 0 <= min_vector_score <= 1, "Minimum vector score must be between 0 and 1."
     assert 0 <= vector_fraction <= 1, "Vector fraction must be between 0 and 1"
     assert 0 <= vector_weight <= 1, "Vector weught must be between 0 and 1"
     assert 0 < max_results <= 100, "Maximum results must be between 1 and 100."
     assert (
         recency_weight is None or 0 <= recency_weight <= 1
     ), "Recency weight must be between 0 and 1."
 
+    time_filter = None
+    if search_from_timestamp or search_to_timestamp:
+        time_filter = {
+            "from": search_from_timestamp.isoformat() if search_from_timestamp else None,
+            "to": search_to_timestamp.isoformat() if search_to_timestamp else None,
+        }
+
     body = {
         "query": query,
         "source_items_type": item_type,
         "content_restrictions": "NONE",
         "limit": max_results,
         "vector_search_cut_off_score": min_vector_score,
         "alfa": vector_weight,
         "beta": 1.0 - recency_weight,
         "text_search_fraction": 1.0 - vector_fraction,
         "k": 60,
+        "published_at": time_filter,
     }
     response = api.post("item-service/items/_hybrid-search", body=body)
 
     # parse
     results = [search_result(i) for i in response["items"]]
 
     # pull exact matches to the top
```

### Comparing `deepsights-api-1.0.0/deepsights/contentstore/resources/news.py` & `deepsights-api-1.0.1/deepsights/contentstore/resources/news.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 """
 This module defines the resource to retrieve news content from the DeepSights API.
 """
 
 from typing import List
+from datetime import datetime
 
 from deepsights.api import APIResource
 from deepsights.contentstore.resources._model import ContentStoreSearchResult
 from deepsights.contentstore.resources._search import (
     contentstore_text_search,
     contentstore_vector_search,
     contentstore_hybrid_search,
@@ -113,28 +114,32 @@
         query: str,
         max_results: int = 30,
         min_vector_score: float = 0.7,
         vector_fraction: float = 0.9,
         vector_weight: float = 0.9,
         recency_weight: float = 0.4,
         promote_exact_match: bool = False,
+        search_from_timestamp: datetime = None,
+        search_to_timestamp: datetime = None,
     ):
         """
         Perform a contentstore hybrid search using the provided query.
 
         Args:
 
             query (str): The query.
             search_result (BaseModel): The model to use for parsing search results.
             max_results (int, optional): The maximum number of search results to return. Defaults to 30.
             min_vector_score (float, optional): The minimum score threshold for search results. Defaults to 0.7.
             vector_fraction (float, optional): The fraction of the search results to be vector-based. Defaults to 0.9.
             vector_weight (float, optional): The weight to apply to vector search in result ranking. Defaults to 0.9.
             recency_weight (float, optional): The weight to apply to recency in result ranking. Defaults to 0.4.
             promote_exact_match (bool, optional): Whether to promote exact matches in the search ranking. Defaults to False.
+            search_from_timestamp (datetime, optional): The start timestamp for the search. Defaults to None.
+            search_to_timestamp (datetime, optional): The end timestamp for the search. Defaults to None.
 
         Returns:
 
             List[NewsArticleSearchResult]: The search results as a list of NewsArticleSearchResult objects.
         """
         return contentstore_hybrid_search(
             self.api,
@@ -145,8 +150,10 @@
             query=query,
             max_results=max_results,
             vector_weight=vector_weight,
             vector_fraction=vector_fraction,
             min_vector_score=min_vector_score,
             recency_weight=recency_weight,
             promote_exact_match=promote_exact_match,
+            search_from_timestamp=search_from_timestamp,
+            search_to_timestamp=search_to_timestamp,
         )
```

### Comparing `deepsights-api-1.0.0/deepsights/contentstore/resources/secondary.py` & `deepsights-api-1.0.1/deepsights/contentstore/resources/secondary.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 """
 This module contains the resource to retrieve secondary reports from the DeepSights content store.
 """
 
 from typing import List
+from datetime import datetime
 
 from deepsights.api import APIResource
 from deepsights.contentstore.resources._model import ContentStoreSearchResult
 from deepsights.contentstore.resources._search import (
     contentstore_text_search,
     contentstore_vector_search,
     contentstore_hybrid_search,
@@ -112,28 +113,32 @@
         query: str,
         max_results: int = 100,
         min_vector_score: float = 0.7,
         vector_fraction: float = 0.9,
         vector_weight: float = 0.9,
         recency_weight: float = 0.4,
         promote_exact_match: bool = False,
+        search_from_timestamp: datetime = None,
+        search_to_timestamp: datetime = None,
     ):
         """
         Perform a contentstore hybrid search using the provided query.
 
         Args:
 
             query (str): The query.
             search_result (BaseModel): The model to use for parsing search results.
             max_results (int, optional): The maximum number of search results to return. Defaults to 100.
             min_vector_score (float, optional): The minimum score threshold for search results. Defaults to 0.7.
             vector_fraction (float, optional): The fraction of the search results to be vector-based. Defaults to 0.9.
             vector_weight (float, optional): The weight to apply to vector search in result ranking. Defaults to 0.9.
             recency_weight (float, optional): The weight to apply to recency in result ranking. Defaults to 0.4.
             promote_exact_match (bool, optional): Whether to promote exact matches in the search ranking. Defaults to False.
+            search_from_timestamp (datetime, optional): The start timestamp for the search. Defaults to None.
+            search_to_timestamp (datetime, optional): The end timestamp for the search. Defaults to None.
 
         Returns:
 
             List[NewsArticleSearchResult]: The search results as a list of NewsArticleSearchResult objects.
         """
         return contentstore_hybrid_search(
             self.api,
@@ -144,8 +149,10 @@
             query=query,
             max_results=max_results,
             vector_weight=vector_weight,
             vector_fraction=vector_fraction,
             min_vector_score=min_vector_score,
             recency_weight=recency_weight,
             promote_exact_match=promote_exact_match,
+            search_from_timestamp=search_from_timestamp,
+            search_to_timestamp=search_to_timestamp,
         )
```

### Comparing `deepsights-api-1.0.0/deepsights/deepsights/__init__.py` & `deepsights-api-1.0.1/deepsights/deepsights/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/deepsights/_mip_identity.py` & `deepsights-api-1.0.1/deepsights/deepsights/_mip_identity.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/deepsights/deepsights.py` & `deepsights-api-1.0.1/deepsights/deepsights/deepsights.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/deepsights/resources/__init__.py` & `deepsights-api-1.0.1/deepsights/deepsights/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/deepsights/resources/quota/__init__.py` & `deepsights-api-1.0.1/deepsights/deepsights/resources/quota/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/deepsights/resources/quota/_model.py` & `deepsights-api-1.0.1/deepsights/deepsights/resources/quota/_model.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/deepsights/resources/quota/quota.py` & `deepsights-api-1.0.1/deepsights/deepsights/resources/quota/quota.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/documentstore/__init__.py` & `deepsights-api-1.0.1/deepsights/documentstore/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/documentstore/documentstore.py` & `deepsights-api-1.0.1/deepsights/documentstore/documentstore.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/documentstore/resources/__init__.py` & `deepsights-api-1.0.1/deepsights/documentstore/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/documentstore/resources/documents/__init__.py` & `deepsights-api-1.0.1/deepsights/documentstore/resources/documents/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_cache.py` & `deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_cache.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_delete.py` & `deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_delete.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_download.py` & `deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_download.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_list.py` & `deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_list.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_load.py` & `deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_load.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_model.py` & `deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_model.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_search.py` & `deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_search.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_segmenter.py` & `deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_segmenter.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/documentstore/resources/documents/_upload.py` & `deepsights-api-1.0.1/deepsights/documentstore/resources/documents/_upload.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/documentstore/resources/documents/documents.py` & `deepsights-api-1.0.1/deepsights/documentstore/resources/documents/documents.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/userclient/__init__.py` & `deepsights-api-1.0.1/deepsights/userclient/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/userclient/minions/_minions.py` & `deepsights-api-1.0.1/deepsights/userclient/minions/_minions.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/userclient/resources/__init__.py` & `deepsights-api-1.0.1/deepsights/userclient/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/userclient/resources/answers/__init__.py` & `deepsights-api-1.0.1/deepsights/userclient/resources/answers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/userclient/resources/answers/_model.py` & `deepsights-api-1.0.1/deepsights/userclient/resources/answers/_model.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/userclient/resources/answers/answer.py` & `deepsights-api-1.0.1/deepsights/userclient/resources/answers/answer.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/userclient/resources/reports/__init__.py` & `deepsights-api-1.0.1/deepsights/userclient/resources/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/userclient/resources/reports/_model.py` & `deepsights-api-1.0.1/deepsights/userclient/resources/reports/_model.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/userclient/resources/reports/report.py` & `deepsights-api-1.0.1/deepsights/userclient/resources/reports/report.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/userclient/userclient.py` & `deepsights-api-1.0.1/deepsights/userclient/userclient.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/utils/__init__.py` & `deepsights-api-1.0.1/deepsights/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/utils/_cache.py` & `deepsights-api-1.0.1/deepsights/utils/_cache.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/utils/_ranking.py` & `deepsights-api-1.0.1/deepsights/utils/_ranking.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/utils/_utils.py` & `deepsights-api-1.0.1/deepsights/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights/utils/model.py` & `deepsights-api-1.0.1/deepsights/utils/model.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/deepsights_api.egg-info/PKG-INFO` & `deepsights-api-1.0.1/deepsights_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsights-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library for the DeepSights APIs
 Home-page: https://github.com/marketlogicsoftware/deepsights-api
 Author: Market Logic Software
 Author-email: info@marketlogicsoftware.com
 License: Apache 2.0
 Project-URL: Documentation, https://marketlogicsoftware.github.io/deepsights-api/
 Classifier: Intended Audience :: Developers
```

### Comparing `deepsights-api-1.0.0/deepsights_api.egg-info/SOURCES.txt` & `deepsights-api-1.0.1/deepsights_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.0/setup.py` & `deepsights-api-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 reqs_filename = os.path.join(package_root, "requirements.txt")
 with io.open(reqs_filename, encoding="utf-8") as reqs_file:
     reqs = reqs_file.read().splitlines()
 
 setup(
     name="deepsights-api",
-    version="1.0.0",
+    version="1.0.1",
     author="Market Logic Software",
     author_email="info@marketlogicsoftware.com",
     description="Python library for the DeepSights APIs",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/marketlogicsoftware/deepsights-api",
     packages=find_packages(exclude=["tests", "tests.*"]),
```


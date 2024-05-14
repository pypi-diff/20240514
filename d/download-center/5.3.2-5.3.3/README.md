# Comparing `tmp/download-center-5.3.2.tar.gz` & `tmp/download-center-5.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/download-center-5.3.2.tar", last modified: Fri May 27 06:30:37 2022, max compression
+gzip compressed data, was "dist/download-center-5.3.3.tar", last modified: Tue Jun  7 06:17:13 2022, max compression
```

## Comparing `download-center-5.3.2.tar` & `download-center-5.3.3.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-05-27 06:30:37.186164 download-center-5.3.2/
--rwxr-xr-x   0 baozhubzhang   (501) staff       (20)       43 2021-12-24 01:52:53.000000 download-center-5.3.2/MANIFEST.in
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     1666 2022-05-27 06:30:37.185886 download-center-5.3.2/PKG-INFO
--rwxr-xr-x   0 baozhubzhang   (501) staff       (20)      786 2022-05-27 06:30:32.000000 download-center-5.3.2/README.md
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-05-27 06:30:37.155317 download-center-5.3.2/demo/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)       76 2019-12-09 04:31:05.000000 download-center-5.3.2/demo/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      121 2019-12-09 04:31:05.000000 download-center-5.3.2/demo/config.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-05-27 06:30:37.156801 download-center-5.3.2/demo/extractor/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.2/demo/extractor/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)    13586 2021-10-14 05:09:11.000000 download-center-5.3.2/demo/extractor/baidu_extractor.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     1394 2019-12-09 04:31:05.000000 download-center-5.3.2/demo/extractor/demo_extractor.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-05-27 06:30:37.159888 download-center-5.3.2/demo/spider/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.2/demo/spider/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      898 2021-11-05 06:23:16.000000 download-center-5.3.2/demo/spider/config.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     5698 2022-05-25 03:00:13.000000 download-center-5.3.2/demo/spider/demo_spider.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)    14353 2021-10-23 07:21:27.000000 download-center-5.3.2/demo/spider/get_header_func.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)    12505 2021-11-05 06:29:21.000000 download-center-5.3.2/demo/spider/mum_create_html.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-05-27 06:30:37.162075 download-center-5.3.2/demo/store/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.2/demo/store/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)    13000 2021-11-05 06:26:29.000000 download-center-5.3.2/demo/store/py_store_mysql_pool.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-05-27 06:30:37.162718 download-center-5.3.2/download_center/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/__init__.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-05-27 06:30:37.164930 download-center-5.3.2/download_center/new_spider/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/new_spider/__init__.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-05-27 06:30:37.170054 download-center-5.3.2/download_center/new_spider/downloader/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/new_spider/downloader/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     1298 2022-05-27 06:29:48.000000 download-center-5.3.2/download_center/new_spider/downloader/config.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     7982 2022-05-27 06:29:48.000000 download-center-5.3.2/download_center/new_spider/downloader/downloader.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      254 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/new_spider/downloader/html_capture.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      260 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/new_spider/downloader/html_downloader.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     9077 2022-05-23 08:37:22.000000 download-center-5.3.2/download_center/new_spider/downloader/html_local_downloader.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      251 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/new_spider/downloader/html_render.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-05-27 06:30:37.172047 download-center-5.3.2/download_center/new_spider/spider/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/new_spider/spider/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)    16054 2022-01-20 03:10:19.000000 download-center-5.3.2/download_center/new_spider/spider/basespider.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     4675 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/new_spider/spider/spider.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-05-27 06:30:37.174918 download-center-5.3.2/download_center/new_spider/util/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/new_spider/util/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      323 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/new_spider/util/util_md5.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      540 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/new_spider/util/util_ping.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      777 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/new_spider/util/util_url.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      709 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/new_spider/util/util_useragent.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-05-27 06:30:37.181269 download-center-5.3.2/download_center/store/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/store/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     3147 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/store/baidu_cookies.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      770 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/store/config.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     9132 2022-05-23 08:23:51.000000 download-center-5.3.2/download_center/store/py_store_mysql_pool.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/store/store_cache.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     3285 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/store/store_es.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     4039 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/store/store_es_v2.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/store/store_file.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      739 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/store/store_mongo.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     2014 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/store/store_oss.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-05-27 06:30:37.183510 download-center-5.3.2/download_center/util/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/util/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     6124 2022-05-23 08:37:22.000000 download-center-5.3.2/download_center/util/py_util_basestore.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     2409 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/util/util_log.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     2480 2019-12-09 04:31:05.000000 download-center-5.3.2/download_center/util/util_log_v2.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-05-27 06:30:37.164542 download-center-5.3.2/download_center.egg-info/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     1666 2022-05-27 06:30:37.000000 download-center-5.3.2/download_center.egg-info/PKG-INFO
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     1906 2022-05-27 06:30:37.000000 download-center-5.3.2/download_center.egg-info/SOURCES.txt
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        1 2022-05-27 06:30:37.000000 download-center-5.3.2/download_center.egg-info/dependency_links.txt
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      106 2022-05-27 06:30:37.000000 download-center-5.3.2/download_center.egg-info/requires.txt
--rw-r--r--   0 baozhubzhang   (501) staff       (20)       26 2022-05-27 06:30:37.000000 download-center-5.3.2/download_center.egg-info/top_level.txt
--rw-r--r--   0 baozhubzhang   (501) staff       (20)       38 2022-05-27 06:30:37.186302 download-center-5.3.2/setup.cfg
--rwxr-xr-x   0 baozhubzhang   (501) staff       (20)     4025 2022-05-27 06:30:32.000000 download-center-5.3.2/setup.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-05-27 06:30:37.185238 download-center-5.3.2/test/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)       89 2019-12-09 04:31:05.000000 download-center-5.3.2/test/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      409 2019-12-09 04:31:05.000000 download-center-5.3.2/test/test1.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      461 2019-12-09 04:31:05.000000 download-center-5.3.2/test/test2.py
+drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.757533 download-center-5.3.3/
+-rwxr-xr-x   0 baozhubzhang   (501) staff       (20)       43 2021-12-24 01:52:53.000000 download-center-5.3.3/MANIFEST.in
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)     1742 2022-06-07 06:17:13.757302 download-center-5.3.3/PKG-INFO
+-rwxr-xr-x   0 baozhubzhang   (501) staff       (20)      854 2022-06-07 06:16:12.000000 download-center-5.3.3/README.md
+drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.733133 download-center-5.3.3/demo/
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)       76 2019-12-09 04:31:05.000000 download-center-5.3.3/demo/__init__.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)      121 2019-12-09 04:31:05.000000 download-center-5.3.3/demo/config.py
+drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.734554 download-center-5.3.3/demo/extractor/
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/demo/extractor/__init__.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)    13586 2021-10-14 05:09:11.000000 download-center-5.3.3/demo/extractor/baidu_extractor.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)     1394 2019-12-09 04:31:05.000000 download-center-5.3.3/demo/extractor/demo_extractor.py
+drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.736951 download-center-5.3.3/demo/spider/
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/demo/spider/__init__.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)      898 2021-11-05 06:23:16.000000 download-center-5.3.3/demo/spider/config.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)     4321 2022-06-07 05:33:04.000000 download-center-5.3.3/demo/spider/demo_spider.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)    14353 2021-10-23 07:21:27.000000 download-center-5.3.3/demo/spider/get_header_func.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)    12505 2021-11-05 06:29:21.000000 download-center-5.3.3/demo/spider/mum_create_html.py
+drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.737613 download-center-5.3.3/demo/store/
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/demo/store/__init__.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)    13000 2021-11-05 06:26:29.000000 download-center-5.3.3/demo/store/py_store_mysql_pool.py
+drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.738489 download-center-5.3.3/download_center/
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/__init__.py
+drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.740696 download-center-5.3.3/download_center/new_spider/
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/__init__.py
+drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.743814 download-center-5.3.3/download_center/new_spider/downloader/
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/downloader/__init__.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)     1298 2022-05-27 06:29:48.000000 download-center-5.3.3/download_center/new_spider/downloader/config.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)     7982 2022-05-27 06:29:48.000000 download-center-5.3.3/download_center/new_spider/downloader/downloader.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)      254 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/downloader/html_capture.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)      260 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/downloader/html_downloader.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)     9077 2022-05-23 08:37:22.000000 download-center-5.3.3/download_center/new_spider/downloader/html_local_downloader.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)      251 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/downloader/html_render.py
+drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.745348 download-center-5.3.3/download_center/new_spider/spider/
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/spider/__init__.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)    16054 2022-01-20 03:10:19.000000 download-center-5.3.3/download_center/new_spider/spider/basespider.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)     4675 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/spider/spider.py
+drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.748387 download-center-5.3.3/download_center/new_spider/util/
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/util/__init__.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)    11141 2022-06-07 05:31:55.000000 download-center-5.3.3/download_center/new_spider/util/util_baidu_relate.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)      323 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/util/util_md5.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)      540 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/util/util_ping.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)      777 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/util/util_url.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)      709 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/util/util_useragent.py
+drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.752827 download-center-5.3.3/download_center/store/
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/__init__.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)     3147 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/baidu_cookies.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)      770 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/config.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)     9132 2022-05-23 08:23:51.000000 download-center-5.3.3/download_center/store/py_store_mysql_pool.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/store_cache.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)     3285 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/store_es.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)     4039 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/store_es_v2.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/store_file.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)      739 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/store_mongo.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)     2014 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/store_oss.py
+drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.754673 download-center-5.3.3/download_center/util/
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/util/__init__.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)     6124 2022-05-23 08:37:22.000000 download-center-5.3.3/download_center/util/py_util_basestore.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)     2409 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/util/util_log.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)     2480 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/util/util_log_v2.py
+drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.740370 download-center-5.3.3/download_center.egg-info/
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)     1742 2022-06-07 06:17:13.000000 download-center-5.3.3/download_center.egg-info/PKG-INFO
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)     1959 2022-06-07 06:17:13.000000 download-center-5.3.3/download_center.egg-info/SOURCES.txt
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)        1 2022-06-07 06:17:13.000000 download-center-5.3.3/download_center.egg-info/dependency_links.txt
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)      106 2022-06-07 06:17:13.000000 download-center-5.3.3/download_center.egg-info/requires.txt
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)       26 2022-06-07 06:17:13.000000 download-center-5.3.3/download_center.egg-info/top_level.txt
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)       38 2022-06-07 06:17:13.757615 download-center-5.3.3/setup.cfg
+-rwxr-xr-x   0 baozhubzhang   (501) staff       (20)     4025 2022-06-07 06:16:12.000000 download-center-5.3.3/setup.py
+drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.756805 download-center-5.3.3/test/
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)       89 2019-12-09 04:31:05.000000 download-center-5.3.3/test/__init__.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)      409 2019-12-09 04:31:05.000000 download-center-5.3.3/test/test1.py
+-rw-r--r--   0 baozhubzhang   (501) staff       (20)      461 2019-12-09 04:31:05.000000 download-center-5.3.3/test/test2.py
```

### Comparing `download-center-5.3.2/PKG-INFO` & `download-center-5.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: download-center
-Version: 5.3.2
+Version: 5.3.3
 Summary: spider framework for winndoo.
 Home-page: http://git.winndoo.cn:82/python/download_center/downloader_client.git
 Author: Welcome#1
 Author-email: baozhu.zhang@winndoo.com
 License: MIT
 Description: 
         ##版本说明：
@@ -20,14 +20,15 @@
         - 5.2.14: downloader fail
         - 5.2.15: downloader fail
         - 5.2.16: pymysql版本写法问题
         - 5.2.18: v1.0.0及以上请使用from pymysql.converters import escape_string
         - 5.3.0: 使用私有网络 172.17.0.*
         - 5.3.1: spider里可以打印当前ip
         - 5.3.2: 登录是判断当前ip
+        - 5.3.3: 添加百度工具包：pc，mb请求头 + 获取真实url
         
         
         #### 新下载中心参数，参考 newDownloadReadme.md 文件
         
         使用方法：
         config={"param": {"et":13,'cu',url}}
         request = SpiderRequest(headers=headers, urls=urls,config = config)
```

### Comparing `download-center-5.3.2/README.md` & `download-center-5.3.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 - 5.2.14: downloader fail
 - 5.2.15: downloader fail
 - 5.2.16: pymysql版本写法问题
 - 5.2.18: v1.0.0及以上请使用from pymysql.converters import escape_string
 - 5.3.0: 使用私有网络 172.17.0.*
 - 5.3.1: spider里可以打印当前ip
 - 5.3.2: 登录是判断当前ip
+- 5.3.3: 添加百度工具包：pc，mb请求头 + 获取真实url
 
 
 #### 新下载中心参数，参考 newDownloadReadme.md 文件
 
 使用方法：
 config={"param": {"et":13,'cu',url}}
 request = SpiderRequest(headers=headers, urls=urls,config = config)
```

### Comparing `download-center-5.3.2/demo/extractor/baidu_extractor.py` & `download-center-5.3.3/demo/extractor/baidu_extractor.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/demo/extractor/demo_extractor.py` & `download-center-5.3.3/demo/extractor/demo_extractor.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/demo/spider/config.py` & `download-center-5.3.3/demo/spider/config.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/demo/spider/demo_spider.py` & `download-center-5.3.3/demo/spider/demo_spider.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from urllib.request import Request, HTTPCookieProcessor, build_opener
 
 from scrapy.http.cookies     import CookieJar
 
 from download_center.new_spider.downloader.downloader import SpiderRequest
 from download_center.new_spider.spider.basespider import BaseSpider
+from download_center.new_spider.util.util_baidu_relate import UtilBaiduRelate
 from download_center.util.util_log import UtilLogger
 
 # 线上测试
 PROJECT_PATH = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 # print("PROJECT_PATH", PROJECT_PATH)
 sys.path.append(PROJECT_PATH)
 # sys.path.append(os.path.join(PROJECT_PATH, 'demo'))
@@ -43,64 +44,29 @@
     def tn(self):
         return random.choice(
             ['50000021_hao_pg', 'site888_3_pg', '77021190_cpr', 'site5566', '520com_pg', '51010079_cpr'])
 
     # 'url': 'https://www.baidu.com/s?%s' % (urllib.parse.urlencode({'word': '联想', 'ie': 'utf-8', 'tn': self.tn()})),
     def start_requests(self):
         try:
-           for i in range(1000):
+           for i in range(100):
                urls = [{
                    'url': 'https://m.baidu.com/s?%s' % (urllib.parse.urlencode({'word': '联想','pn':10})),
                    'type': 17,
                    'unique_key':self.get_unique_key()#默认md5 url 字段，不写则表示相同链接只查一次
                }]
-               headers = {
-                   "User-Agent": "Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/97.0.4692.71 Mobile Safari/537.36",
-                   'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
-                   # 'Accept-Language':'zh-CN,zh;q=0.9,en-CN;q=0.8,en;q=0.7,ar-XB;q=0.6,ar;q=0.5',
-                   'Cookie': self.get_baidu_mb_cookie()
-               }
-               config={"param": {'cu':'https://www.baidu.com'},"conf_district_id":3}
-               request = SpiderRequest(headers=headers, urls=urls,config=config)
+               config={"param": {'cu':'https://m.baidu.com','et':3},"conf_district_id":0}
+               untilBaidu = UtilBaiduRelate()
+               request = SpiderRequest(headers=untilBaidu.getBaiduMbHeader(), urls=urls,config=config)
                self.sending_queue.put(request)
                time.sleep(0.1)
 
         except Exception:
             self.log.error('获取初始请求出错: {}'.format(traceback.format_exc()))
 
-
-    #获取百度移动端cookie
-    def get_baidu_mb_cookie(self):
-        cookies = None
-        try:
-            cookie_jar = cookiejar.CookieJar()
-            request = Request('https://m.baidu.com/tc?tcreq4log=1', headers={})
-            handlers = [HTTPCookieProcessor(cookie_jar)]
-            opener = build_opener(*handlers)
-            opener.open(request, timeout=10)
-            for cookie in cookie_jar:
-                if cookie.name == 'BDORZ':
-                    cookies = 'BDORZ=' + cookie.value
-                    break
-        except Exception:
-            pass
-        return cookies
-
-    #获取百度pc 端cookie
-    def get_baidu_pc_cookie(self):
-        letters_one = []
-        letters_two = []
-        for _ in range(32):
-            letters_one.append(random.choice(string.ascii_uppercase + string.digits))
-
-        for _ in range(27):
-            letters_two.append(random.choice(string.lowercase + string.digits))
-
-        return 'BAIDUID=%s:FG=1' % (''.join(letters_one)) + '; ' + 'BA_HECTOR=%s' % (''.join(letters_two))
-
     def get_stores(self):
         # 存储器
         stores = list()
         return stores
 
     def deal_response_results_status(self, task_status, url, result, request):
         """
@@ -112,19 +78,22 @@
 
         Returns:
         根据自己的解析类型做不同的处理，默认返回html
         """
         if task_status == '2':
             config = request.config
             try:
+
+                self.store_queue.put(result["result"])
+
                 # result = json.loads(result["result"])
-                if '联想' not in result["result"]:
-                    print("结果抓取失败")
-                else:
-                    print("成功!，长度：{},url：{}".format(len(result), url['url']))
+                # if '联想' not in result["result"]:
+                #     print("结果抓取失败")
+                # else:
+                #     print("成功!，长度：{},url：{}".format(len(result), url['url']))
             except Exception as e:
                 print('失败！url：{}'.format( url['url']))
 
             # rdata = self.ext.ext ractor(result["result"])
             # self.store_queue.put(result)
             # if isinstance(rdata, int):
             #     print("request ua: {}".format(request.headers["User-Agent"]))
```

### Comparing `download-center-5.3.2/demo/spider/get_header_func.py` & `download-center-5.3.3/demo/spider/get_header_func.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/demo/spider/mum_create_html.py` & `download-center-5.3.3/demo/spider/mum_create_html.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/demo/store/py_store_mysql_pool.py` & `download-center-5.3.3/demo/store/py_store_mysql_pool.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/new_spider/downloader/config.py` & `download-center-5.3.3/download_center/new_spider/downloader/config.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/new_spider/downloader/downloader.py` & `download-center-5.3.3/download_center/new_spider/downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/new_spider/downloader/html_local_downloader.py` & `download-center-5.3.3/download_center/new_spider/downloader/html_local_downloader.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/new_spider/spider/basespider.py` & `download-center-5.3.3/download_center/new_spider/spider/basespider.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/new_spider/spider/spider.py` & `download-center-5.3.3/download_center/new_spider/spider/spider.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/new_spider/util/util_ping.py` & `download-center-5.3.3/download_center/new_spider/util/util_ping.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/new_spider/util/util_url.py` & `download-center-5.3.3/download_center/new_spider/util/util_url.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/new_spider/util/util_useragent.py` & `download-center-5.3.3/download_center/new_spider/util/util_useragent.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/store/baidu_cookies.py` & `download-center-5.3.3/download_center/store/baidu_cookies.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/store/config.py` & `download-center-5.3.3/download_center/store/config.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/store/py_store_mysql_pool.py` & `download-center-5.3.3/download_center/store/py_store_mysql_pool.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/store/store_es.py` & `download-center-5.3.3/download_center/store/store_es.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/store/store_es_v2.py` & `download-center-5.3.3/download_center/store/store_es_v2.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/store/store_mongo.py` & `download-center-5.3.3/download_center/store/store_mongo.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/store/store_oss.py` & `download-center-5.3.3/download_center/store/store_oss.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/util/py_util_basestore.py` & `download-center-5.3.3/download_center/util/py_util_basestore.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/util/util_log.py` & `download-center-5.3.3/download_center/util/util_log.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center/util/util_log_v2.py` & `download-center-5.3.3/download_center/util/util_log_v2.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.2/download_center.egg-info/PKG-INFO` & `download-center-5.3.3/download_center.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: download-center
-Version: 5.3.2
+Version: 5.3.3
 Summary: spider framework for winndoo.
 Home-page: http://git.winndoo.cn:82/python/download_center/downloader_client.git
 Author: Welcome#1
 Author-email: baozhu.zhang@winndoo.com
 License: MIT
 Description: 
         ##版本说明：
@@ -20,14 +20,15 @@
         - 5.2.14: downloader fail
         - 5.2.15: downloader fail
         - 5.2.16: pymysql版本写法问题
         - 5.2.18: v1.0.0及以上请使用from pymysql.converters import escape_string
         - 5.3.0: 使用私有网络 172.17.0.*
         - 5.3.1: spider里可以打印当前ip
         - 5.3.2: 登录是判断当前ip
+        - 5.3.3: 添加百度工具包：pc，mb请求头 + 获取真实url
         
         
         #### 新下载中心参数，参考 newDownloadReadme.md 文件
         
         使用方法：
         config={"param": {"et":13,'cu',url}}
         request = SpiderRequest(headers=headers, urls=urls,config = config)
```

### Comparing `download-center-5.3.2/download_center.egg-info/SOURCES.txt` & `download-center-5.3.3/download_center.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 download_center/new_spider/downloader/html_downloader.py
 download_center/new_spider/downloader/html_local_downloader.py
 download_center/new_spider/downloader/html_render.py
 download_center/new_spider/spider/__init__.py
 download_center/new_spider/spider/basespider.py
 download_center/new_spider/spider/spider.py
 download_center/new_spider/util/__init__.py
+download_center/new_spider/util/util_baidu_relate.py
 download_center/new_spider/util/util_md5.py
 download_center/new_spider/util/util_ping.py
 download_center/new_spider/util/util_url.py
 download_center/new_spider/util/util_useragent.py
 download_center/store/__init__.py
 download_center/store/baidu_cookies.py
 download_center/store/config.py
```

### Comparing `download-center-5.3.2/setup.py` & `download-center-5.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'download-center'
 DESCRIPTION = 'spider framework for winndoo.'
 URL = 'http://git.winndoo.cn:82/python/download_center/downloader_client.git'
 EMAIL = 'baozhu.zhang@winndoo.com'
 AUTHOR = 'Welcome#1'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '5.3.2'
+VERSION = '5.3.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'pymongo',
     'oss2',
     'redis',
     'DBUtils',
```


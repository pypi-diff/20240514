# Comparing `tmp/metadata-viewer-1.8.tar.gz` & `tmp/metadata-viewer-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metadata-viewer-1.8.tar", last modified: Wed Oct 11 15:16:37 2023, max compression
+gzip compressed data, was "metadata-viewer-1.9.tar", last modified: Tue Oct 31 09:53:56 2023, max compression
```

## Comparing `metadata-viewer-1.8.tar` & `metadata-viewer-1.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-11 15:16:37.789953 metadata-viewer-1.8/
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    35147 2022-09-01 09:15:34.000000 metadata-viewer-1.8/LICENSE
--rw-rw-r--   0 yunior    (1001) yunior    (1001)      188 2023-09-13 10:50:03.000000 metadata-viewer-1.8/MANIFEST.in
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     2579 2023-10-11 15:16:37.789953 metadata-viewer-1.8/PKG-INFO
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     1915 2023-09-19 10:26:29.000000 metadata-viewer-1.8/README.rst
-drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-11 15:16:37.781953 metadata-viewer-1.8/metadata_viewer.egg-info/
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     2579 2023-10-11 15:16:37.000000 metadata-viewer-1.8/metadata_viewer.egg-info/PKG-INFO
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     2245 2023-10-11 15:16:37.000000 metadata-viewer-1.8/metadata_viewer.egg-info/SOURCES.txt
--rw-rw-r--   0 yunior    (1001) yunior    (1001)        1 2023-10-11 15:16:37.000000 metadata-viewer-1.8/metadata_viewer.egg-info/dependency_links.txt
--rw-rw-r--   0 yunior    (1001) yunior    (1001)       28 2023-10-11 15:16:37.000000 metadata-viewer-1.8/metadata_viewer.egg-info/requires.txt
--rw-rw-r--   0 yunior    (1001) yunior    (1001)       15 2023-10-11 15:16:37.000000 metadata-viewer-1.8/metadata_viewer.egg-info/top_level.txt
-drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-11 15:16:37.781953 metadata-viewer-1.8/metadataviewer/
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     1171 2023-10-11 15:15:42.000000 metadata-viewer-1.8/metadataviewer/__init__.py
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     3399 2023-09-26 13:48:23.000000 metadata-viewer-1.8/metadataviewer/__main__.py
-drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-11 15:16:37.781953 metadata-viewer-1.8/metadataviewer/dao/
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     1214 2023-09-13 10:50:03.000000 metadata-viewer-1.8/metadataviewer/dao/__init__.py
-drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-11 15:16:37.781953 metadata-viewer-1.8/metadataviewer/dao/model/
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     2188 2023-09-13 10:50:03.000000 metadata-viewer-1.8/metadataviewer/dao/model/__init__.py
-drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-11 15:16:37.781953 metadata-viewer-1.8/metadataviewer/gui/
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     1177 2023-07-28 09:55:20.000000 metadata-viewer-1.8/metadataviewer/gui/__init__.py
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     1858 2023-07-28 09:55:20.000000 metadata-viewer-1.8/metadataviewer/gui/config.py
-drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-11 15:16:37.781953 metadata-viewer-1.8/metadataviewer/gui/qt/
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     1154 2023-06-26 14:44:04.000000 metadata-viewer-1.8/metadataviewer/gui/qt/__init__.py
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     3295 2023-10-04 14:09:48.000000 metadata-viewer-1.8/metadataviewer/gui/qt/constants.py
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    82742 2023-10-11 15:12:34.000000 metadata-viewer-1.8/metadataviewer/gui/qt/qtviewer.py
-drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-11 15:16:37.785953 metadata-viewer-1.8/metadataviewer/gui/resources/
--rw-rw-r--   0 yunior    (1001) yunior    (1001)      217 2023-06-19 05:44:47.000000 metadata-viewer-1.8/metadataviewer/gui/resources/backward-solid.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    11128 2023-06-19 05:44:47.000000 metadata-viewer-1.8/metadataviewer/gui/resources/down-arrow.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    26313 2023-08-10 08:49:27.000000 metadata-viewer-1.8/metadataviewer/gui/resources/error.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    15068 2023-06-19 05:44:47.000000 metadata-viewer-1.8/metadataviewer/gui/resources/exit.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    12165 2023-08-10 08:49:27.000000 metadata-viewer-1.8/metadataviewer/gui/resources/export_csv.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    31240 2023-08-10 08:49:27.000000 metadata-viewer-1.8/metadataviewer/gui/resources/export_xlsx.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)      320 2023-06-19 05:44:47.000000 metadata-viewer-1.8/metadataviewer/gui/resources/fa-arrow-down.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)      314 2023-06-19 05:44:47.000000 metadata-viewer-1.8/metadataviewer/gui/resources/fa-arrow-up.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)      361 2023-06-19 05:44:47.000000 metadata-viewer-1.8/metadataviewer/gui/resources/fa-cancel.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)      311 2023-06-19 05:44:47.000000 metadata-viewer-1.8/metadataviewer/gui/resources/fa-close.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)      292 2023-06-19 05:44:47.000000 metadata-viewer-1.8/metadataviewer/gui/resources/fa-list-ul.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)      308 2023-06-19 05:44:47.000000 metadata-viewer-1.8/metadataviewer/gui/resources/fa-next.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     8624 2023-09-13 10:50:03.000000 metadata-viewer-1.8/metadataviewer/gui/resources/fa-ok.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)      302 2023-06-19 05:44:47.000000 metadata-viewer-1.8/metadataviewer/gui/resources/fa-previous.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     7661 2023-06-19 05:44:47.000000 metadata-viewer-1.8/metadataviewer/gui/resources/folder.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     7103 2023-08-10 08:49:27.000000 metadata-viewer-1.8/metadataviewer/gui/resources/from_here.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    22835 2023-06-19 05:44:47.000000 metadata-viewer-1.8/metadataviewer/gui/resources/gallery.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     6472 2023-07-28 09:55:20.000000 metadata-viewer-1.8/metadataviewer/gui/resources/goto_item.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    23024 2023-07-28 09:55:20.000000 metadata-viewer-1.8/metadataviewer/gui/resources/hide.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    16699 2023-06-26 15:09:08.000000 metadata-viewer-1.8/metadataviewer/gui/resources/increasedecimals.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    12946 2023-06-19 05:44:47.000000 metadata-viewer-1.8/metadataviewer/gui/resources/no-image.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     2250 2023-09-26 10:15:48.000000 metadata-viewer-1.8/metadataviewer/gui/resources/plot.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     2017 2023-08-10 08:49:27.000000 metadata-viewer-1.8/metadataviewer/gui/resources/plus.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    26613 2023-06-26 09:27:01.000000 metadata-viewer-1.8/metadataviewer/gui/resources/preferences.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    16083 2023-06-26 15:08:15.000000 metadata-viewer-1.8/metadataviewer/gui/resources/reducedecimals.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     9528 2023-06-19 05:44:47.000000 metadata-viewer-1.8/metadataviewer/gui/resources/sections.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     4378 2023-06-19 05:44:47.000000 metadata-viewer-1.8/metadataviewer/gui/resources/table-view.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     6292 2023-06-19 05:44:47.000000 metadata-viewer-1.8/metadataviewer/gui/resources/table.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    12876 2023-08-10 08:49:27.000000 metadata-viewer-1.8/metadataviewer/gui/resources/to_here.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    11029 2023-06-19 05:44:47.000000 metadata-viewer-1.8/metadataviewer/gui/resources/up-arrow.png
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    37056 2023-06-26 15:15:20.000000 metadata-viewer-1.8/metadataviewer/gui/resources/zoom.png
-drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-11 15:16:37.789953 metadata-viewer-1.8/metadataviewer/model/
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     1262 2023-09-13 10:50:03.000000 metadata-viewer-1.8/metadataviewer/model/__init__.py
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     1236 2023-09-19 14:12:33.000000 metadata-viewer-1.8/metadataviewer/model/constants.py
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    10560 2023-10-05 10:41:45.000000 metadata-viewer-1.8/metadataviewer/model/object_manager.py
--rw-rw-r--   0 yunior    (1001) yunior    (1001)    10813 2023-09-20 11:04:19.000000 metadata-viewer-1.8/metadataviewer/model/page.py
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     5195 2023-10-09 12:53:21.000000 metadata-viewer-1.8/metadataviewer/model/renderers.py
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     1845 2023-06-15 12:13:50.000000 metadata-viewer-1.8/metadataviewer/model/utils.py
-drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-11 15:16:37.789953 metadata-viewer-1.8/metadataviewer/tests/
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     1303 2023-09-13 10:50:03.000000 metadata-viewer-1.8/metadataviewer/tests/__init__.py
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     1728 2023-09-13 10:50:03.000000 metadata-viewer-1.8/metadataviewer/tests/test_metadataviewer_object_manager.py
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     2273 2023-09-13 10:50:03.000000 metadata-viewer-1.8/metadataviewer/tests/test_metadataviewer_page.py
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     1905 2023-09-13 10:50:03.000000 metadata-viewer-1.8/metadataviewer/tests/test_metadataviewer_startfile.py
--rw-rw-r--   0 yunior    (1001) yunior    (1001)       27 2023-09-13 10:50:03.000000 metadata-viewer-1.8/requirements.txt
--rw-rw-r--   0 yunior    (1001) yunior    (1001)       38 2023-10-11 15:16:37.789953 metadata-viewer-1.8/setup.cfg
--rw-rw-r--   0 yunior    (1001) yunior    (1001)     2756 2023-09-13 10:50:03.000000 metadata-viewer-1.8/setup.py
+drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-31 09:53:56.733554 metadata-viewer-1.9/
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    35147 2022-09-01 09:15:34.000000 metadata-viewer-1.9/LICENSE
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)      188 2023-09-13 10:50:03.000000 metadata-viewer-1.9/MANIFEST.in
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     2579 2023-10-31 09:53:56.733554 metadata-viewer-1.9/PKG-INFO
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     1915 2023-09-19 10:26:29.000000 metadata-viewer-1.9/README.rst
+drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-31 09:53:56.721554 metadata-viewer-1.9/metadata_viewer.egg-info/
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     2579 2023-10-31 09:53:56.000000 metadata-viewer-1.9/metadata_viewer.egg-info/PKG-INFO
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     2245 2023-10-31 09:53:56.000000 metadata-viewer-1.9/metadata_viewer.egg-info/SOURCES.txt
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)        1 2023-10-31 09:53:56.000000 metadata-viewer-1.9/metadata_viewer.egg-info/dependency_links.txt
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)       28 2023-10-31 09:53:56.000000 metadata-viewer-1.9/metadata_viewer.egg-info/requires.txt
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)       15 2023-10-31 09:53:56.000000 metadata-viewer-1.9/metadata_viewer.egg-info/top_level.txt
+drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-31 09:53:56.721554 metadata-viewer-1.9/metadataviewer/
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     1171 2023-10-31 08:49:42.000000 metadata-viewer-1.9/metadataviewer/__init__.py
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     3399 2023-09-26 13:48:23.000000 metadata-viewer-1.9/metadataviewer/__main__.py
+drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-31 09:53:56.721554 metadata-viewer-1.9/metadataviewer/dao/
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     1214 2023-09-13 10:50:03.000000 metadata-viewer-1.9/metadataviewer/dao/__init__.py
+drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-31 09:53:56.721554 metadata-viewer-1.9/metadataviewer/dao/model/
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     2188 2023-09-13 10:50:03.000000 metadata-viewer-1.9/metadataviewer/dao/model/__init__.py
+drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-31 09:53:56.725554 metadata-viewer-1.9/metadataviewer/gui/
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     1177 2023-07-28 09:55:20.000000 metadata-viewer-1.9/metadataviewer/gui/__init__.py
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     1858 2023-07-28 09:55:20.000000 metadata-viewer-1.9/metadataviewer/gui/config.py
+drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-31 09:53:56.725554 metadata-viewer-1.9/metadataviewer/gui/qt/
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     1154 2023-06-26 14:44:04.000000 metadata-viewer-1.9/metadataviewer/gui/qt/__init__.py
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     3295 2023-10-04 14:09:48.000000 metadata-viewer-1.9/metadataviewer/gui/qt/constants.py
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    82598 2023-10-31 09:25:04.000000 metadata-viewer-1.9/metadataviewer/gui/qt/qtviewer.py
+drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-31 09:53:56.729554 metadata-viewer-1.9/metadataviewer/gui/resources/
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)      217 2023-06-19 05:44:47.000000 metadata-viewer-1.9/metadataviewer/gui/resources/backward-solid.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    11128 2023-06-19 05:44:47.000000 metadata-viewer-1.9/metadataviewer/gui/resources/down-arrow.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    26313 2023-08-10 08:49:27.000000 metadata-viewer-1.9/metadataviewer/gui/resources/error.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    15068 2023-06-19 05:44:47.000000 metadata-viewer-1.9/metadataviewer/gui/resources/exit.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    12165 2023-08-10 08:49:27.000000 metadata-viewer-1.9/metadataviewer/gui/resources/export_csv.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    31240 2023-08-10 08:49:27.000000 metadata-viewer-1.9/metadataviewer/gui/resources/export_xlsx.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)      320 2023-06-19 05:44:47.000000 metadata-viewer-1.9/metadataviewer/gui/resources/fa-arrow-down.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)      314 2023-06-19 05:44:47.000000 metadata-viewer-1.9/metadataviewer/gui/resources/fa-arrow-up.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)      361 2023-06-19 05:44:47.000000 metadata-viewer-1.9/metadataviewer/gui/resources/fa-cancel.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)      311 2023-06-19 05:44:47.000000 metadata-viewer-1.9/metadataviewer/gui/resources/fa-close.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)      292 2023-06-19 05:44:47.000000 metadata-viewer-1.9/metadataviewer/gui/resources/fa-list-ul.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)      308 2023-06-19 05:44:47.000000 metadata-viewer-1.9/metadataviewer/gui/resources/fa-next.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     8624 2023-09-13 10:50:03.000000 metadata-viewer-1.9/metadataviewer/gui/resources/fa-ok.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)      302 2023-06-19 05:44:47.000000 metadata-viewer-1.9/metadataviewer/gui/resources/fa-previous.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     7661 2023-06-19 05:44:47.000000 metadata-viewer-1.9/metadataviewer/gui/resources/folder.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     7103 2023-08-10 08:49:27.000000 metadata-viewer-1.9/metadataviewer/gui/resources/from_here.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    22835 2023-06-19 05:44:47.000000 metadata-viewer-1.9/metadataviewer/gui/resources/gallery.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     6472 2023-07-28 09:55:20.000000 metadata-viewer-1.9/metadataviewer/gui/resources/goto_item.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    23024 2023-07-28 09:55:20.000000 metadata-viewer-1.9/metadataviewer/gui/resources/hide.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    16699 2023-06-26 15:09:08.000000 metadata-viewer-1.9/metadataviewer/gui/resources/increasedecimals.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    12946 2023-06-19 05:44:47.000000 metadata-viewer-1.9/metadataviewer/gui/resources/no-image.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     2250 2023-09-26 10:15:48.000000 metadata-viewer-1.9/metadataviewer/gui/resources/plot.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     2017 2023-08-10 08:49:27.000000 metadata-viewer-1.9/metadataviewer/gui/resources/plus.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    26613 2023-06-26 09:27:01.000000 metadata-viewer-1.9/metadataviewer/gui/resources/preferences.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    16083 2023-06-26 15:08:15.000000 metadata-viewer-1.9/metadataviewer/gui/resources/reducedecimals.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     9528 2023-06-19 05:44:47.000000 metadata-viewer-1.9/metadataviewer/gui/resources/sections.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     4378 2023-06-19 05:44:47.000000 metadata-viewer-1.9/metadataviewer/gui/resources/table-view.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     6292 2023-06-19 05:44:47.000000 metadata-viewer-1.9/metadataviewer/gui/resources/table.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    12876 2023-08-10 08:49:27.000000 metadata-viewer-1.9/metadataviewer/gui/resources/to_here.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    11029 2023-06-19 05:44:47.000000 metadata-viewer-1.9/metadataviewer/gui/resources/up-arrow.png
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    37056 2023-06-26 15:15:20.000000 metadata-viewer-1.9/metadataviewer/gui/resources/zoom.png
+drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-31 09:53:56.733554 metadata-viewer-1.9/metadataviewer/model/
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     1262 2023-09-13 10:50:03.000000 metadata-viewer-1.9/metadataviewer/model/__init__.py
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     1236 2023-09-19 14:12:33.000000 metadata-viewer-1.9/metadataviewer/model/constants.py
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    10560 2023-10-05 10:41:45.000000 metadata-viewer-1.9/metadataviewer/model/object_manager.py
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)    10813 2023-09-20 11:04:19.000000 metadata-viewer-1.9/metadataviewer/model/page.py
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     5238 2023-10-23 10:17:17.000000 metadata-viewer-1.9/metadataviewer/model/renderers.py
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     1845 2023-06-15 12:13:50.000000 metadata-viewer-1.9/metadataviewer/model/utils.py
+drwxrwxr-x   0 yunior    (1001) yunior    (1001)        0 2023-10-31 09:53:56.733554 metadata-viewer-1.9/metadataviewer/tests/
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     1303 2023-09-13 10:50:03.000000 metadata-viewer-1.9/metadataviewer/tests/__init__.py
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     1728 2023-09-13 10:50:03.000000 metadata-viewer-1.9/metadataviewer/tests/test_metadataviewer_object_manager.py
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     2273 2023-09-13 10:50:03.000000 metadata-viewer-1.9/metadataviewer/tests/test_metadataviewer_page.py
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     1905 2023-09-13 10:50:03.000000 metadata-viewer-1.9/metadataviewer/tests/test_metadataviewer_startfile.py
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)       27 2023-09-13 10:50:03.000000 metadata-viewer-1.9/requirements.txt
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)       38 2023-10-31 09:53:56.733554 metadata-viewer-1.9/setup.cfg
+-rw-rw-r--   0 yunior    (1001) yunior    (1001)     2756 2023-09-13 10:50:03.000000 metadata-viewer-1.9/setup.py
```

### Comparing `metadata-viewer-1.8/LICENSE` & `metadata-viewer-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/PKG-INFO` & `metadata-viewer-1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metadata-viewer
-Version: 1.8
+Version: 1.9
 Summary: Generic metadata viewer
 Home-page: https://github.com/fonsecareyna82/metadata_viewer
 Author: Yunior C. Fonseca-Reyna, Pablo Conesa, Jorge Jiménez
 Author-email: cfonseca@cnb.csic.es, pconesa@cnb.csic.es, jjimenez@cnb.csic.es
 Project-URL: Bug Reports, https://github.com/fonsecareyna82/metadata_viewer/issues
 Project-URL: Source, https://github.com/fonsecareyna82/metadata_viewer
 Keywords: metadata-viewer
```

### Comparing `metadata-viewer-1.8/README.rst` & `metadata-viewer-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadata_viewer.egg-info/PKG-INFO` & `metadata-viewer-1.9/metadata_viewer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metadata-viewer
-Version: 1.8
+Version: 1.9
 Summary: Generic metadata viewer
 Home-page: https://github.com/fonsecareyna82/metadata_viewer
 Author: Yunior C. Fonseca-Reyna, Pablo Conesa, Jorge Jiménez
 Author-email: cfonseca@cnb.csic.es, pconesa@cnb.csic.es, jjimenez@cnb.csic.es
 Project-URL: Bug Reports, https://github.com/fonsecareyna82/metadata_viewer/issues
 Project-URL: Source, https://github.com/fonsecareyna82/metadata_viewer
 Keywords: metadata-viewer
```

### Comparing `metadata-viewer-1.8/metadata_viewer.egg-info/SOURCES.txt` & `metadata-viewer-1.9/metadata_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/__init__.py` & `metadata-viewer-1.9/metadataviewer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-__version__ = 1.8
+__version__ = 1.9
```

### Comparing `metadata-viewer-1.8/metadataviewer/__main__.py` & `metadata-viewer-1.9/metadataviewer/__main__.py`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/dao/__init__.py` & `metadata-viewer-1.9/metadataviewer/dao/__init__.py`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/dao/model/__init__.py` & `metadata-viewer-1.9/metadataviewer/dao/model/__init__.py`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/__init__.py` & `metadata-viewer-1.9/metadataviewer/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/config.py` & `metadata-viewer-1.9/metadataviewer/gui/config.py`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/qt/__init__.py` & `metadata-viewer-1.9/metadataviewer/gui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/qt/constants.py` & `metadata-viewer-1.9/metadataviewer/gui/qt/constants.py`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/qt/qtviewer.py` & `metadata-viewer-1.9/metadataviewer/gui/qt/qtviewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -617,19 +617,19 @@
             self.setValue(self.value() + step)
 
         event.accept()
 
 
 class CustomWidget(QWidget):
     """Class to  custom the table cell widget"""
-    def __init__(self, data, id, imagePath='', addText=False, text=''):
+    def __init__(self, data, id, value, addText=False, text=''):
         super().__init__()
         self._data = data
         self._id = id
-        self._imagePath = imagePath
+        self._value = value
         self._layout = QVBoxLayout()
         self._layout.setContentsMargins(0, 0, 0, 0)
         self._label = QLabel()
         self._adicinalText = QLabel(text)
         self._type = str
 
         if isinstance(data, bool):  # The data is a boolean
@@ -704,17 +704,17 @@
         """Return the widget content"""
         return self._label
 
     def getData(self):
         """Return the content data"""
         return self._data
 
-    def getImagePath(self):
+    def getValue(self):
         """Return the image path"""
-        return self._imagePath
+        return self._value
 
     def getId(self):
         """Return the widget id"""
         return self._id
 
 
 class TableView(QTableWidget):
@@ -755,15 +755,15 @@
         self.hScrollBar = QScrollBar()
         self._columnsMap = {}
         self._createHeader()
         self._table = self.objectManager.getTable(self._tableName)
         self.columns = self._table.getColumns()
         self._columnWithImages = self.getColumnWithImages()
         self.tableWithAdditionalInfo = self.objectManager.getTableWithAdditionalInfo()
-        self._rowHeight = DEFAULT_ROW_HEIGHT  # Default row height
+        self._rowHeight = DEFAULT_ROW_HEIGHT if self._columnWithImages is None else self.getOldZoom()  # Default row height
         self._columnsWidth = [0 for i in range(len(self.columns))]
         self.propertiesTableDialog.registerColumns(self.columns)
         self.propertiesTableDialog.setLoadFirstTime(True)
         self.propertiesTableDialog.InsertRows()
         self.propertiesTableDialog.hideColumns()
         self.setVerticalScrollBar(self.vScrollBar)
         self.setHorizontalScrollBar(self.hScrollBar)
@@ -897,30 +897,30 @@
                                                                  self.columnCount() - 1), True)
             for col in range(currenctColumnIndex, endColumn):
                 column = self._columns[col]
                 if self.propertiesTableDialog.visibleCheckBoxList[column.getIndex()]:
                     renderer = column.getRenderer()
                     if renderer.renderType() != Image:
                         item = renderer.render(values[col])
-                        widget = CustomWidget(item, row.getId())
+                        widget = CustomWidget(item, row.getId(), values[col])
                     else:
                         if self.propertiesTableDialog.renderCheckBoxList[column.getIndex()].isChecked():
                             item = renderer.render(values[col])
                             if self.tableWithAdditionalInfo and self._tableName == self.tableWithAdditionalInfo[0]:
                                 text = self.composeAdditionaInfo(row)
                                 widget = CustomWidget(item, row.getId(),
-                                                      imagePath=values[col],
+                                                      values[col],
                                                       addText=True, text=text)
                             else:
                                 widget = CustomWidget(item, row.getId(),
-                                                      imagePath=values[col])
+                                                      values[col])
                         else:
                             item = values[col]
                             widget = CustomWidget(item, row.getId(),
-                                                  imagePath=values[col])
+                                                  values[col])
 
                     if widget.sizeHint().height() > self._rowHeight:
                         self._rowHeight = widget.sizeHint().height()
 
                     width = self.calculateColumnWidth(widget, column.getIndex())
                     if width > self._columnsWidth[column.getIndex()]:
                         self._columnsWidth[column.getIndex()] = width
@@ -1131,19 +1131,19 @@
                         break
                     value = rowsValues[countImages]
                     item = renderer.render(value)
                     currentRow = rows[countImages]
                     if self.tableWithAdditionalInfo and self._tableName == self.tableWithAdditionalInfo[0]:
                         text = self.composeAdditionaInfo(currentRow)
                         widget = CustomWidget(item, currentRow.getId(),
-                                              imagePath=value, addText=True,
+                                              value, addText=True,
                                               text=text)
                     else:
                         widget = CustomWidget(item, currentRow.getId(),
-                                              imagePath=value)
+                                              value)
 
                     self.setCellWidget(currentValue + row, col, widget)
                     if rows[countImages].getId() in selection:
                         self.setRangeSelected(QTableWidgetSelectionRange(currentValue + row, col, currentValue + row, col),  True)
 
                     self.setColumnWidth(col, self.getOldZoom() + 5)
                     countImages += 1
@@ -1695,49 +1695,50 @@
             else:
                 self.reduceDecimals.setEnabled(False)
                 self.increaseDecimals.setEnabled(False)
 
             if item.widgetType() == Image:
                 self.zoom.setEnabled(True)
                 self.zoomLabel.setEnabled(True)
-                self.createTableExternalAction(item, column)
+                self.createTableExtraAction(item, column)
             else:
                 self.zoom.setEnabled(False)
                 self.zoomLabel.setEnabled(False)
                 self.externalProgramsToolBar.clear()
 
-    def createTableExternalAction(self, item, column):
+    def createTableExtraAction(self, item, column):
         """Create the external program actions for the table"""
         columns = self.table.getTable().getColumns()
         columnHeaderText = self.table.horizontalHeaderItem(column).text()
         realIndex = self.table._columnsMap[columnHeaderText]
         renderer = columns[realIndex].getRenderer()
-        externalPrograms = renderer.getExternalPrograms()
+        extraActions = renderer.getActions()
         self.externalProgramsToolBar.clear()
-        self.addExternalActions(externalPrograms,
-                                item._imagePath.split('@')[-1])
+        self.addExtraActions(extraActions, item)
 
-    def createGalleryExternalActions(self, item):
+    def createGalleryExtraActions(self, item):
         """Create the external program actions for the gallery"""
-        externalPrograms = self.gallery._renderer.getExternalPrograms()
+        extraActions = self.gallery._renderer.getActions()
         self.externalProgramsToolBar.clear()
-        if externalPrograms is not None:
-            self.addExternalActions(externalPrograms,
-                                    item._imagePath.split('@')[-1])
-
-    def addExternalActions(self, externalPrograms, imagePath):
-        for externalProgram in externalPrograms:
-            action = QAction(externalProgram._tooltip, self)
-            if externalProgram._icon is not None:
-                action.setIcon(QIcon(externalProgram._icon))
-            else:
-                action.setText(externalProgram._text)
-            action.setEnabled(True)
-            action.triggered.connect(lambda: externalProgram._callback(imagePath))
-            self.externalProgramsToolBar.addAction(action)
+        if extraActions is not None:
+            self.addExtraActions(extraActions, item)
+
+    def addExtraActions(self, extraActions, item):
+        for extraAction in extraActions:
+            self.addExtraAction(extraAction, item)
+
+    def addExtraAction(self, extraAction, item):
+        action = QAction(extraAction._tooltip, self)
+        if extraAction._icon is not None:
+            action.setIcon(QIcon(extraAction._icon))
+        else:
+            action.setText(extraAction._text)
+        action.setEnabled(True)
+        action.triggered.connect(lambda: extraAction._callback(item.getValue()))
+        self.externalProgramsToolBar.addAction(action)
 
     def toggleColumn(self, table_view, column):
         """Hide a given column"""
         self.table.setColumnHidden(column,
                                    not table_view.isColumnHidden(column))
 
     def _loadTableView(self):
@@ -1937,15 +1938,15 @@
             if modifiers == Qt.NoModifier:  # Simple click
                 self.gallery.getTable().getSelection().clear()
                 self.gallery.getTable().getSelection().addRowSelected(rowId)
             elif modifiers == Qt.ControlModifier:  # ctrl+click
                 self.table.getTable().getSelection().addRowSelected(rowId)
             elif modifiers == Qt.ShiftModifier:  # shift+click
                 self.selectedRange(self.table.getLastSelectedRow() - 1, row + 1)
-            self.createGalleryExternalActions(self.gallery.cellWidget(row, column))
+            self.createGalleryExtraActions(self.gallery.cellWidget(row, column))
             self._triggeredGotoItem = False
             self.goToItem.setValue(index)
             self._triggeredGotoItem = True
             self.gallery.setCurrentRowColumn(row, self.gallery.getCurrentColumn())
             self._updateStatusBarRowColumn()
             self._updateStatusBarSelectedRows()
```

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/down-arrow.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/down-arrow.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/error.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/error.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/exit.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/exit.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/export_csv.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/export_csv.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/export_xlsx.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/export_xlsx.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/fa-ok.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/fa-ok.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/folder.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/folder.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/from_here.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/from_here.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/gallery.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/gallery.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/goto_item.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/goto_item.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/hide.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/hide.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/increasedecimals.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/increasedecimals.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/no-image.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/no-image.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/plot.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/plot.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/plus.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/plus.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/preferences.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/preferences.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/reducedecimals.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/reducedecimals.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/sections.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/sections.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/table-view.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/table-view.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/table.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/table.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/to_here.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/to_here.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/up-arrow.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/up-arrow.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/gui/resources/zoom.png` & `metadata-viewer-1.9/metadataviewer/gui/resources/zoom.png`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/model/__init__.py` & `metadata-viewer-1.9/metadataviewer/model/__init__.py`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/model/constants.py` & `metadata-viewer-1.9/metadataviewer/model/constants.py`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/model/object_manager.py` & `metadata-viewer-1.9/metadataviewer/model/object_manager.py`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/model/page.py` & `metadata-viewer-1.9/metadataviewer/model/page.py`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/model/renderers.py` & `metadata-viewer-1.9/metadataviewer/model/renderers.py`

 * *Files 25% similar despite different names*

```diff
@@ -33,35 +33,35 @@
 
 from PIL import Image
 from abc import abstractmethod
 
 from .constants import IMAGE_DEFAULT_SIZE
 
 
-class ExternalProgram:
+class Action:
     def __init__(self, text, icon, tooltip, callback):
         self._text = text
         self._icon = icon
         self._tooltip = tooltip
         self._callback = callback
 
     def open(self, path):
         self._callback(path)
 
 
 class IRenderer:
-    _externalPrograms = []
 
-    @classmethod
-    def addProgram(cls, program: ExternalProgram):
-        cls._externalPrograms.append(program)
+    def __init__(self):
+        self._extraActions = []
 
-    @classmethod
-    def getExternalPrograms(cls):
-        return cls._externalPrograms
+    def addAction(self, action: Action):
+        self._extraActions.append(action)
+
+    def getActions(self):
+        return self._extraActions
 
     @abstractmethod
     def _render(self, value):
         pass
 
     def render(self, value):
         try:
@@ -93,14 +93,15 @@
     def renderType(self):
         return int
 
 
 class FloatRenderer(IRenderer):
 
     def __init__(self, decimalNumber: int = 2):
+        super().__init__()
         self._decimalNumber = decimalNumber
 
     def _render(self, value):
         return round(float(value), self._decimalNumber)
 
     def setDecimalNumber(self, decimalNumber):
         self._decimalNumber = decimalNumber
@@ -120,14 +121,15 @@
     def renderType(self):
         return bool
 
 
 class MatrixRender(IRenderer):
 
     def __init__(self, decimalNumber: int = 2):
+        super().__init__()
         self._decimalNumber = decimalNumber
 
     def _render(self, value):
         # replace nan values by 0
         value = value.replace('nan', '0')
         matrix = np.array(eval(value))
         np.set_printoptions(precision=self._decimalNumber, suppress=True)
@@ -165,14 +167,15 @@
         return ['jpg', 'png']
 
 
 class ImageRenderer(IRenderer):
     _imageReaders = []
 
     def __init__(self, size=IMAGE_DEFAULT_SIZE):
+        super().__init__()
         self._size = size
 
     def getSize(self):
         return self._size
 
     @classmethod
     def registerImageReader(cls, imageReader):
```

### Comparing `metadata-viewer-1.8/metadataviewer/model/utils.py` & `metadata-viewer-1.9/metadataviewer/model/utils.py`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/tests/__init__.py` & `metadata-viewer-1.9/metadataviewer/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/tests/test_metadataviewer_object_manager.py` & `metadata-viewer-1.9/metadataviewer/tests/test_metadataviewer_object_manager.py`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/tests/test_metadataviewer_page.py` & `metadata-viewer-1.9/metadataviewer/tests/test_metadataviewer_page.py`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/metadataviewer/tests/test_metadataviewer_startfile.py` & `metadata-viewer-1.9/metadataviewer/tests/test_metadataviewer_startfile.py`

 * *Files identical despite different names*

### Comparing `metadata-viewer-1.8/setup.py` & `metadata-viewer-1.9/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/xurpas_data_quality-0.0.3a4.tar.gz` & `tmp/xurpas_data_quality-0.0.3a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xurpas_data_quality-0.0.3a4.tar", last modified: Tue May 14 04:58:09 2024, max compression
+gzip compressed data, was "xurpas_data_quality-0.0.3a5.tar", last modified: Tue May 14 05:09:26 2024, max compression
```

## Comparing `xurpas_data_quality-0.0.3a4.tar` & `xurpas_data_quality-0.0.3a5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 04:58:09.212287 xurpas_data_quality-0.0.3a4/
--rw-rw-rw-   0        0        0      110 2024-05-07 06:47:23.000000 xurpas_data_quality-0.0.3a4/MANIFEST.in
--rw-rw-rw-   0        0        0      933 2024-05-14 04:58:09.211277 xurpas_data_quality-0.0.3a4/PKG-INFO
--rw-rw-rw-   0        0        0      394 2024-05-14 04:48:43.000000 xurpas_data_quality-0.0.3a4/README.md
--rw-rw-rw-   0        0        0      808 2024-05-14 04:40:10.000000 xurpas_data_quality-0.0.3a4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 04:58:09.212287 xurpas_data_quality-0.0.3a4/setup.cfg
--rw-rw-rw-   0        0        0     1106 2024-05-14 04:40:10.000000 xurpas_data_quality-0.0.3a4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 04:58:09.148458 xurpas_data_quality-0.0.3a4/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 04:58:09.157920 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/
--rw-rw-rw-   0        0        0       61 2024-05-14 04:48:56.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 04:58:09.178727 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/data/
--rw-rw-rw-   0        0        0        0 2024-05-14 04:40:10.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 04:58:09.179844 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/data/alerts/
--rw-rw-rw-   0        0        0        0 2024-05-03 07:10:29.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/data/alerts/__init__.py
--rw-rw-rw-   0        0        0      953 2024-05-06 00:02:03.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/data/alerts/alerts.py
-drwxrwxrwx   0        0        0        0 2024-05-14 04:58:09.181976 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/data/algorithms/
--rw-rw-rw-   0        0        0       54 2024-05-14 04:40:10.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/data/algorithms/__init__.py
--rw-rw-rw-   0        0        0      495 2024-05-03 03:47:01.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/data/algorithms/algorithms.py
--rw-rw-rw-   0        0        0      286 2024-04-30 02:18:01.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/data/dataframe.py
--rw-rw-rw-   0        0        0     6613 2024-05-06 01:25:03.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/data/describe.py
--rw-rw-rw-   0        0        0      224 2024-05-06 01:15:30.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/data/descriptions.py
--rw-rw-rw-   0        0        0      350 2024-04-26 07:12:37.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/data/pandas_dataframe.py
--rw-rw-rw-   0        0        0     1011 2024-05-03 02:20:38.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/data_report.py
--rw-rw-rw-   0        0        0        0 2024-05-07 06:51:12.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-14 04:58:09.185728 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/
--rw-rw-rw-   0        0        0        0 2024-05-07 05:20:40.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/__init__.py
--rw-rw-rw-   0        0        0      221 2024-05-14 02:11:10.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/render.py
-drwxrwxrwx   0        0        0        0 2024-05-14 04:58:09.185728 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/render_types/
--rw-rw-rw-   0        0        0        0 2024-05-14 03:23:54.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/render_types/render_numerical.py
--rw-rw-rw-   0        0        0      474 2024-05-14 04:40:31.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/render_variable.py
--rw-rw-rw-   0        0        0     4411 2024-05-14 04:40:10.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/renderer.py
-drwxrwxrwx   0        0        0        0 2024-05-14 04:58:09.196528 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:20:52.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 04:58:09.197532 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/assets/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:21:04.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/assets/__init__.py
--rw-rw-rw-   0        0        0      594 2024-05-06 06:23:01.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/assets/script.js
--rw-rw-rw-   0        0        0      600 2024-05-06 05:56:54.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/assets/style.css
--rw-rw-rw-   0        0        0      249 2024-05-06 06:04:16.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/base.html
--rw-rw-rw-   0        0        0      106 2024-05-01 16:04:49.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/collapse.html
-drwxrwxrwx   0        0        0        0 2024-05-14 04:58:09.204376 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/containers/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:21:13.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/containers/__init__.py
--rw-rw-rw-   0        0        0      209 2024-04-30 07:01:56.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/containers/box.html
--rw-rw-rw-   0        0        0       78 2024-05-03 02:13:15.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/containers/column.html
--rw-rw-rw-   0        0        0      141 2024-05-03 02:44:57.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/containers/default.html
--rw-rw-rw-   0        0        0      340 2024-05-01 12:08:46.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/containers/sections.html
--rw-rw-rw-   0        0        0      835 2024-05-01 16:36:14.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/containers/tabs.html
--rw-rw-rw-   0        0        0       72 2024-05-06 02:07:52.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/containers/test.html
--rw-rw-rw-   0        0        0      277 2024-05-06 05:58:23.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/dropdown.html
--rw-rw-rw-   0        0        0      268 2024-04-29 06:44:51.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/navigation.html
--rw-rw-rw-   0        0        0      279 2024-05-02 01:11:31.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/plot.html
--rw-rw-rw-   0        0        0      449 2024-05-06 06:03:50.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/script.html
--rw-rw-rw-   0        0        0      267 2024-05-06 06:03:51.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/style.html
--rw-rw-rw-   0        0        0      390 2024-05-06 00:49:14.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/table.html
--rw-rw-rw-   0        0        0      300 2024-05-02 00:52:44.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/toggle.html
--rw-rw-rw-   0        0        0      454 2024-05-06 05:58:21.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/variable.html
--rw-rw-rw-   0        0        0      569 2024-05-14 04:40:10.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates.py
-drwxrwxrwx   0        0        0        0 2024-05-14 04:58:09.207814 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/report/
--rw-rw-rw-   0        0        0       30 2024-04-30 02:52:09.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/report/__init__.py
--rw-rw-rw-   0        0        0     7914 2024-05-06 05:08:28.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/report/report.py
-drwxrwxrwx   0        0        0        0 2024-05-14 04:58:09.208823 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/visuals/
--rw-rw-rw-   0        0        0      141 2024-05-06 02:32:12.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/visuals/__init__.py
--rw-rw-rw-   0        0        0     2257 2024-05-06 02:30:31.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/visuals/plots.py
-drwxrwxrwx   0        0        0        0 2024-05-14 04:58:09.210271 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality.egg-info/
--rw-rw-rw-   0        0        0      933 2024-05-14 04:58:09.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2466 2024-05-14 04:58:09.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 04:58:09.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-14 04:58:09.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-14 04:58:09.000000 xurpas_data_quality-0.0.3a4/src/xurpas_data_quality.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 05:09:26.336066 xurpas_data_quality-0.0.3a5/
+-rw-rw-rw-   0        0        0      110 2024-05-07 06:47:23.000000 xurpas_data_quality-0.0.3a5/MANIFEST.in
+-rw-rw-rw-   0        0        0      926 2024-05-14 05:09:26.335035 xurpas_data_quality-0.0.3a5/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2024-05-14 05:09:16.000000 xurpas_data_quality-0.0.3a5/README.md
+-rw-rw-rw-   0        0        0      808 2024-05-14 04:40:10.000000 xurpas_data_quality-0.0.3a5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 05:09:26.336066 xurpas_data_quality-0.0.3a5/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2024-05-14 04:40:10.000000 xurpas_data_quality-0.0.3a5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:09:26.248782 xurpas_data_quality-0.0.3a5/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 05:09:26.262841 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/
+-rw-rw-rw-   0        0        0       61 2024-05-14 05:09:03.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:09:26.289562 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/data/
+-rw-rw-rw-   0        0        0        0 2024-05-14 04:40:10.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:09:26.291651 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/data/alerts/
+-rw-rw-rw-   0        0        0        0 2024-05-03 07:10:29.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/data/alerts/__init__.py
+-rw-rw-rw-   0        0        0      953 2024-05-06 00:02:03.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/data/alerts/alerts.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:09:26.293887 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/data/algorithms/
+-rw-rw-rw-   0        0        0       54 2024-05-14 04:40:10.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/data/algorithms/__init__.py
+-rw-rw-rw-   0        0        0      495 2024-05-03 03:47:01.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/data/algorithms/algorithms.py
+-rw-rw-rw-   0        0        0      286 2024-04-30 02:18:01.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/data/dataframe.py
+-rw-rw-rw-   0        0        0     6613 2024-05-06 01:25:03.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/data/describe.py
+-rw-rw-rw-   0        0        0      224 2024-05-06 01:15:30.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/data/descriptions.py
+-rw-rw-rw-   0        0        0      350 2024-04-26 07:12:37.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/data/pandas_dataframe.py
+-rw-rw-rw-   0        0        0     1245 2024-05-14 05:04:05.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/data_report.py
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:51:12.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-14 05:09:26.300897 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/
+-rw-rw-rw-   0        0        0        0 2024-05-07 05:20:40.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/__init__.py
+-rw-rw-rw-   0        0        0      221 2024-05-14 02:11:10.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/render.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:09:26.301898 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/render_types/
+-rw-rw-rw-   0        0        0        0 2024-05-14 03:23:54.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/render_types/render_numerical.py
+-rw-rw-rw-   0        0        0      474 2024-05-14 04:40:31.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/render_variable.py
+-rw-rw-rw-   0        0        0     4417 2024-05-14 05:05:46.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/renderer.py
+-rw-rw-rw-   0        0        0      569 2024-05-14 04:40:10.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/template_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:09:26.313662 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:20:52.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:09:26.317035 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/assets/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:21:04.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/assets/__init__.py
+-rw-rw-rw-   0        0        0      594 2024-05-06 06:23:01.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/assets/script.js
+-rw-rw-rw-   0        0        0      600 2024-05-06 05:56:54.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/assets/style.css
+-rw-rw-rw-   0        0        0      249 2024-05-06 06:04:16.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/base.html
+-rw-rw-rw-   0        0        0      106 2024-05-01 16:04:49.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/collapse.html
+drwxrwxrwx   0        0        0        0 2024-05-14 05:09:26.325547 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/containers/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:21:13.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/containers/__init__.py
+-rw-rw-rw-   0        0        0      209 2024-04-30 07:01:56.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/containers/box.html
+-rw-rw-rw-   0        0        0       78 2024-05-03 02:13:15.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/containers/column.html
+-rw-rw-rw-   0        0        0      141 2024-05-03 02:44:57.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/containers/default.html
+-rw-rw-rw-   0        0        0      340 2024-05-01 12:08:46.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/containers/sections.html
+-rw-rw-rw-   0        0        0      835 2024-05-01 16:36:14.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/containers/tabs.html
+-rw-rw-rw-   0        0        0       72 2024-05-06 02:07:52.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/containers/test.html
+-rw-rw-rw-   0        0        0      277 2024-05-06 05:58:23.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/dropdown.html
+-rw-rw-rw-   0        0        0      268 2024-04-29 06:44:51.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/navigation.html
+-rw-rw-rw-   0        0        0      279 2024-05-02 01:11:31.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/plot.html
+-rw-rw-rw-   0        0        0      449 2024-05-06 06:03:50.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/script.html
+-rw-rw-rw-   0        0        0      267 2024-05-06 06:03:51.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/style.html
+-rw-rw-rw-   0        0        0      390 2024-05-06 00:49:14.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/table.html
+-rw-rw-rw-   0        0        0      300 2024-05-02 00:52:44.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/toggle.html
+-rw-rw-rw-   0        0        0      454 2024-05-06 05:58:21.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/variable.html
+drwxrwxrwx   0        0        0        0 2024-05-14 05:09:26.327532 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/report/
+-rw-rw-rw-   0        0        0       30 2024-04-30 02:52:09.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/report/__init__.py
+-rw-rw-rw-   0        0        0     7914 2024-05-06 05:08:28.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/report/report.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:09:26.327532 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/visuals/
+-rw-rw-rw-   0        0        0      141 2024-05-06 02:32:12.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/visuals/__init__.py
+-rw-rw-rw-   0        0        0     2257 2024-05-06 02:30:31.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/visuals/plots.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:09:26.327532 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality.egg-info/
+-rw-rw-rw-   0        0        0      926 2024-05-14 05:09:26.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2472 2024-05-14 05:09:26.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 05:09:26.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-14 05:09:26.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-14 05:09:26.000000 xurpas_data_quality-0.0.3a5/src/xurpas_data_quality.egg-info/top_level.txt
```

### Comparing `xurpas_data_quality-0.0.3a4/PKG-INFO` & `xurpas_data_quality-0.0.3a5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xurpas_data_quality
-Version: 0.0.3a4
+Version: 0.0.3a5
 Summary: XAIL Data quality
 Author: Neil Ortaliz
 Author-email: Neil Ortaliz <neil.ortaliz@xurpas.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -15,17 +15,17 @@
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: jinja2
 
 # Xurpas Data Quality Report
 
 ## How to Use
-- Load the data to be analyzed
+- Load the data to be analyzed (so far only csv files supported)
 - Import the DataReport class
 - Save the report to html File
 
 #### Sample Usage
 ```python
 from xurpas_data_quality import DataReport
-a = DataReport(r"C:\Users\Neil\Documents\Projects\xurpas\test_reports\manhour_utilization_summary.csv")
+a = DataReport("test_reports/manhour_utilization_summary.csv")
 a.to_file("Manhour Utilization Summary", "test_reports/test.html")
 ```
```

### Comparing `xurpas_data_quality-0.0.3a4/pyproject.toml` & `xurpas_data_quality-0.0.3a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.3a4/setup.py` & `xurpas_data_quality-0.0.3a5/setup.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/data/alerts/alerts.py` & `xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/data/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/data/describe.py` & `xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/data/describe.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/renderer.py` & `xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict,List
 
-from xurpas_data_quality.render.templates import template
+from xurpas_data_quality.render.template_loader import template
 
 class BaseRenderer(ABC):
     def __init__(self, content: Dict[str, Any], name: str = None, id:str=None, **kwargs):
         self.content = content
 
         if name is not None:
             self.content['name'] = name
```

### Comparing `xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/assets/script.js` & `xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/assets/script.js`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/assets/style.css` & `xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/assets/style.css`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates/containers/tabs.html` & `xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/templates/containers/tabs.html`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/render/templates.py` & `xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/render/template_loader.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/report/report.py` & `xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/report/report.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.3a4/src/xurpas_data_quality/visuals/plots.py` & `xurpas_data_quality-0.0.3a5/src/xurpas_data_quality/visuals/plots.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.3a4/src/xurpas_data_quality.egg-info/PKG-INFO` & `xurpas_data_quality-0.0.3a5/src/xurpas_data_quality.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xurpas_data_quality
-Version: 0.0.3a4
+Version: 0.0.3a5
 Summary: XAIL Data quality
 Author: Neil Ortaliz
 Author-email: Neil Ortaliz <neil.ortaliz@xurpas.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -15,17 +15,17 @@
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: jinja2
 
 # Xurpas Data Quality Report
 
 ## How to Use
-- Load the data to be analyzed
+- Load the data to be analyzed (so far only csv files supported)
 - Import the DataReport class
 - Save the report to html File
 
 #### Sample Usage
 ```python
 from xurpas_data_quality import DataReport
-a = DataReport(r"C:\Users\Neil\Documents\Projects\xurpas\test_reports\manhour_utilization_summary.csv")
+a = DataReport("test_reports/manhour_utilization_summary.csv")
 a.to_file("Manhour Utilization Summary", "test_reports/test.html")
 ```
```

### Comparing `xurpas_data_quality-0.0.3a4/src/xurpas_data_quality.egg-info/SOURCES.txt` & `xurpas_data_quality-0.0.3a5/src/xurpas_data_quality.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 src/xurpas_data_quality/data/alerts/alerts.py
 src/xurpas_data_quality/data/algorithms/__init__.py
 src/xurpas_data_quality/data/algorithms/algorithms.py
 src/xurpas_data_quality/render/__init__.py
 src/xurpas_data_quality/render/render.py
 src/xurpas_data_quality/render/render_variable.py
 src/xurpas_data_quality/render/renderer.py
-src/xurpas_data_quality/render/templates.py
+src/xurpas_data_quality/render/template_loader.py
 src/xurpas_data_quality/render/render_types/render_numerical.py
 src/xurpas_data_quality/render/templates/__init__.py
 src/xurpas_data_quality/render/templates/base.html
 src/xurpas_data_quality/render/templates/collapse.html
 src/xurpas_data_quality/render/templates/dropdown.html
 src/xurpas_data_quality/render/templates/navigation.html
 src/xurpas_data_quality/render/templates/plot.html
```


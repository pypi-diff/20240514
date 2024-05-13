# Comparing `tmp/owega-5.7.2.tar.gz` & `tmp/owega-5.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owega-5.7.2.tar", last modified: Mon May 13 22:29:23 2024, max compression
+gzip compressed data, was "owega-5.7.3.tar", last modified: Mon May 13 23:19:25 2024, max compression
```

## Comparing `owega-5.7.2.tar` & `owega-5.7.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 22:29:23.390114 owega-5.7.2/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6076 2024-05-10 14:44:53.000000 owega-5.7.2/LICENSE
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16066 2024-05-13 22:29:23.390114 owega-5.7.2/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5023 2024-04-17 02:21:38.000000 owega-5.7.2/README.md
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 22:29:23.388114 owega-5.7.2/owega/
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 22:29:23.389114 owega-5.7.2/owega/OweHandlers/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-27 12:05:16.000000 owega-5.7.2/owega/OweHandlers/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      980 2024-05-08 02:39:07.000000 owega-5.7.2/owega/OweHandlers/handle_add_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1590 2024-05-08 02:39:07.000000 owega-5.7.2/owega/OweHandlers/handle_commands.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1185 2024-05-08 02:39:07.000000 owega-5.7.2/owega/OweHandlers/handle_context.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1601 2024-05-08 02:39:07.000000 owega-5.7.2/owega/OweHandlers/handle_del_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.7.2/owega/OweHandlers/handle_dinput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3457 2024-05-08 02:39:07.000000 owega-5.7.2/owega/OweHandlers/handle_edit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1339 2024-05-08 02:39:07.000000 owega-5.7.2/owega/OweHandlers/handle_estimation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5059 2024-05-08 02:39:07.000000 owega-5.7.2/owega/OweHandlers/handle_finput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.7.2/owega/OweHandlers/handle_frequency.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      521 2024-05-08 02:39:07.000000 owega-5.7.2/owega/OweHandlers/handle_genconf.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      523 2024-05-08 02:39:07.000000 owega-5.7.2/owega/OweHandlers/handle_history.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3310 2024-05-08 02:39:08.000000 owega-5.7.2/owega/OweHandlers/handle_image.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1118 2024-05-08 02:39:08.000000 owega-5.7.2/owega/OweHandlers/handle_load.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1698 2024-05-08 02:39:08.000000 owega-5.7.2/owega/OweHandlers/handle_model.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1791 2024-05-08 02:39:08.000000 owega-5.7.2/owega/OweHandlers/handle_presence.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      637 2024-05-08 02:39:08.000000 owega-5.7.2/owega/OweHandlers/handle_quit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1090 2024-05-08 02:39:08.000000 owega-5.7.2/owega/OweHandlers/handle_save.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      945 2024-05-08 02:39:08.000000 owega-5.7.2/owega/OweHandlers/handle_system.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1739 2024-05-08 02:39:08.000000 owega-5.7.2/owega/OweHandlers/handle_temperature.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1404 2024-05-08 02:39:08.000000 owega-5.7.2/owega/OweHandlers/handle_tokens.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1556 2024-05-08 02:39:08.000000 owega-5.7.2/owega/OweHandlers/handle_top_p.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1245 2024-05-08 02:39:08.000000 owega-5.7.2/owega/OweHandlers/handle_tts.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2407 2024-04-27 12:05:16.000000 owega-5.7.2/owega/OweHandlers/handlers.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 22:29:23.389114 owega-5.7.2/owega/OwegaFun/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-27 12:05:16.000000 owega-5.7.2/owega/OwegaFun/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-17 02:21:38.000000 owega-5.7.2/owega/OwegaFun/functions.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4342 2024-04-27 12:05:16.000000 owega-5.7.2/owega/OwegaFun/longTermSouvenirs.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5816 2024-04-27 12:05:16.000000 owega-5.7.2/owega/OwegaFun/utility.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 22:29:23.389114 owega-5.7.2/owega/OwegaSession/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.7.2/owega/OwegaSession/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2763 2024-04-27 12:05:16.000000 owega-5.7.2/owega/OwegaSession/main_bottom_toolbar.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5592 2024-04-27 12:05:16.000000 owega-5.7.2/owega/OwegaSession/promptsession.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      175 2024-05-08 02:39:08.000000 owega-5.7.2/owega/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.7.2/owega/__main__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10338 2024-05-13 22:25:22.000000 owega-5.7.2/owega/ask.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 22:29:23.389114 owega-5.7.2/owega/changelog/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-27 12:05:16.000000 owega-5.7.2/owega/changelog/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    24412 2024-05-13 22:27:02.000000 owega-5.7.2/owega/changelog/changelog.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1534 2024-04-27 12:05:16.000000 owega-5.7.2/owega/changelog/changelogEntry.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-17 02:21:38.000000 owega-5.7.2/owega/changelog/version.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 22:29:23.389114 owega-5.7.2/owega/config/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.7.2/owega/config/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1810 2024-04-27 12:05:16.000000 owega-5.7.2/owega/config/baseConf.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 22:29:23.389114 owega-5.7.2/owega/conversation/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.7.2/owega/conversation/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10105 2024-05-13 22:26:17.000000 owega-5.7.2/owega/conversation/conversation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1418 2024-05-10 10:34:51.000000 owega-5.7.2/owega/getLogger.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.7.2/owega/handlerBase.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6141 2024-05-10 14:44:53.000000 owega-5.7.2/owega/license.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    12103 2024-04-27 12:05:16.000000 owega-5.7.2/owega/owega.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6111 2024-04-27 12:05:16.000000 owega-5.7.2/owega/utils.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 22:29:23.389114 owega-5.7.2/owega.egg-info/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16066 2024-05-13 22:29:23.000000 owega-5.7.2/owega.egg-info/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1656 2024-05-13 22:29:23.000000 owega-5.7.2/owega.egg-info/SOURCES.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-05-13 22:29:23.000000 owega-5.7.2/owega.egg-info/dependency_links.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-05-13 22:29:23.000000 owega-5.7.2/owega.egg-info/entry_points.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-05-13 22:29:23.000000 owega-5.7.2/owega.egg-info/requires.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-05-13 22:29:23.000000 owega-5.7.2/owega.egg-info/top_level.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.7.2/pyproject.toml
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-05-13 22:29:23.390114 owega-5.7.2/setup.cfg
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2085 2024-05-10 13:40:23.000000 owega-5.7.2/setup.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.100103 owega-5.7.3/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6076 2024-05-10 14:44:53.000000 owega-5.7.3/LICENSE
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16292 2024-05-13 23:19:25.100103 owega-5.7.3/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5023 2024-04-17 02:21:38.000000 owega-5.7.3/README.md
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.098103 owega-5.7.3/owega/
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.099103 owega-5.7.3/owega/OweHandlers/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-27 12:05:16.000000 owega-5.7.3/owega/OweHandlers/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      980 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_add_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1590 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_commands.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1185 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_context.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1601 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_del_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_dinput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3457 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_edit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1339 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_estimation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5059 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_finput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_frequency.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      521 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_genconf.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      523 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_history.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3246 2024-05-13 23:14:07.000000 owega-5.7.3/owega/OweHandlers/handle_image.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1118 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_load.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1698 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_model.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1791 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_presence.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      637 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_quit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1090 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_save.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      945 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_system.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1739 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_temperature.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1404 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_tokens.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1556 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_top_p.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1245 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_tts.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2407 2024-04-27 12:05:16.000000 owega-5.7.3/owega/OweHandlers/handlers.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.099103 owega-5.7.3/owega/OwegaFun/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-27 12:05:16.000000 owega-5.7.3/owega/OwegaFun/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-17 02:21:38.000000 owega-5.7.3/owega/OwegaFun/functions.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4342 2024-04-27 12:05:16.000000 owega-5.7.3/owega/OwegaFun/longTermSouvenirs.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5816 2024-04-27 12:05:16.000000 owega-5.7.3/owega/OwegaFun/utility.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.099103 owega-5.7.3/owega/OwegaSession/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.7.3/owega/OwegaSession/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2763 2024-04-27 12:05:16.000000 owega-5.7.3/owega/OwegaSession/main_bottom_toolbar.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5592 2024-04-27 12:05:16.000000 owega-5.7.3/owega/OwegaSession/promptsession.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      175 2024-05-08 02:39:08.000000 owega-5.7.3/owega/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.7.3/owega/__main__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10338 2024-05-13 22:30:06.000000 owega-5.7.3/owega/ask.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.099103 owega-5.7.3/owega/changelog/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-27 12:05:16.000000 owega-5.7.3/owega/changelog/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    24778 2024-05-13 23:16:47.000000 owega-5.7.3/owega/changelog/changelog.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1534 2024-04-27 12:05:16.000000 owega-5.7.3/owega/changelog/changelogEntry.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-17 02:21:38.000000 owega-5.7.3/owega/changelog/version.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.099103 owega-5.7.3/owega/config/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.7.3/owega/config/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1810 2024-04-27 12:05:16.000000 owega-5.7.3/owega/config/baseConf.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.100103 owega-5.7.3/owega/conversation/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.7.3/owega/conversation/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10105 2024-05-13 22:26:17.000000 owega-5.7.3/owega/conversation/conversation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1418 2024-05-10 10:34:51.000000 owega-5.7.3/owega/getLogger.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.7.3/owega/handlerBase.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6141 2024-05-10 14:44:53.000000 owega-5.7.3/owega/license.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    11378 2024-05-13 23:12:32.000000 owega-5.7.3/owega/owega.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     7504 2024-05-13 23:06:32.000000 owega-5.7.3/owega/utils.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.100103 owega-5.7.3/owega.egg-info/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16292 2024-05-13 23:19:25.000000 owega-5.7.3/owega.egg-info/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1656 2024-05-13 23:19:25.000000 owega-5.7.3/owega.egg-info/SOURCES.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-05-13 23:19:25.000000 owega-5.7.3/owega.egg-info/dependency_links.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-05-13 23:19:25.000000 owega-5.7.3/owega.egg-info/entry_points.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-05-13 23:19:25.000000 owega-5.7.3/owega.egg-info/requires.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-05-13 23:19:25.000000 owega-5.7.3/owega.egg-info/top_level.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.7.3/pyproject.toml
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-05-13 23:19:25.100103 owega-5.7.3/setup.cfg
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2085 2024-05-10 13:40:23.000000 owega-5.7.3/setup.py
```

### Comparing `owega-5.7.2/LICENSE` & `owega-5.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/PKG-INFO` & `owega-5.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.7.2
+Version: 5.7.3
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: DGPL-1.0
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -135,15 +135,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.7.2 CHANGELOG:
+OWEGA v5.7.3 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -364,8 +364,12 @@
 5.6.3: Fixes config's api_key not being used.
        Better docstrings on handlers.
 5.6.4: Fix for ask.ask() crashing if OPENAI_API_KEY isn't set.
 
 5.7.0: Changed the license to the DarkGeem Public License v1.0.
 5.7.1: Fixed a non-ascii character in the DGPL.
 5.7.2: Added vision support for GPT-4o.
+5.7.3: Better cost estimation, including input/output costs.
+       (added support for all GPT model as of 2024-05-14)
+       (added support for all mistral API models as of today)
+       (all other models return a cost of 0)
 ```
```

### Comparing `owega-5.7.2/README.md` & `owega-5.7.3/README.md`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_add_sysmem.py` & `owega-5.7.3/owega/OweHandlers/handle_add_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_commands.py` & `owega-5.7.3/owega/OweHandlers/handle_commands.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_context.py` & `owega-5.7.3/owega/OweHandlers/handle_context.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_del_sysmem.py` & `owega-5.7.3/owega/OweHandlers/handle_del_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_dinput.py` & `owega-5.7.3/owega/OweHandlers/handle_dinput.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_edit.py` & `owega-5.7.3/owega/OweHandlers/handle_edit.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_estimation.py` & `owega-5.7.3/owega/OweHandlers/handle_estimation.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_finput.py` & `owega-5.7.3/owega/OweHandlers/handle_finput.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_frequency.py` & `owega-5.7.3/owega/OweHandlers/handle_frequency.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_genconf.py` & `owega-5.7.3/owega/OweHandlers/handle_genconf.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_history.py` & `owega-5.7.3/owega/OweHandlers/handle_history.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_image.py` & `owega-5.7.3/owega/OweHandlers/handle_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import openai
 import prompt_toolkit as pt
 
 from ..ask import ask
 from ..config import baseConf
 from ..OwegaFun import existingFunctions, functionlist_to_toollist
 from ..OwegaSession import OwegaSession as ps
-from ..utils import clrtxt, estimated_tokens, info_print, play_tts
+from ..utils import clrtxt, estimated_tokens_and_cost, info_print, play_tts
 
 
 def encode_image(filename: str) -> str:
     """
     Return the local image as a base64 url.
 
     Args:
@@ -60,25 +60,21 @@
             clrtxt("yellow", " IMAGE URL ") + ": ")).strip()
     image_url = encode_image(image_url)
     image_urls = [image_url]
     if not user_prompt:
         user_prompt = ps['main'].prompt(pt.ANSI(
             clrtxt("yellow", " PRE-FILE PROMPT ") + ": ")).strip()
     if baseConf.get("estimation", False):
-        etkn = estimated_tokens(
+        etkn, cost = estimated_tokens_and_cost(
             "",
             messages,
-            functionlist_to_toollist(existingFunctions.getEnabled())
+            functionlist_to_toollist(existingFunctions.getEnabled()),
+            baseConf.get('model', ''),
+            baseConf.get("max_tokens", 4096)
         )
-        cost_per_token = (
-            0.03
-            if 'gpt-4' in baseConf.get("model", "")
-            else 0.003
-        ) / 1000
-        cost = cost_per_token * etkn
         if not silent:
             print(f"\033[37mestimated tokens: {etkn}\033[0m")
             print(f"\033[37mestimated cost: {cost:.5f}\033[0m")
     if baseConf.get("debug", False):
         pre_time = time.time()
     messages.add_image(user_prompt, image_urls)
     messages = ask(
```

### Comparing `owega-5.7.2/owega/OweHandlers/handle_load.py` & `owega-5.7.3/owega/OweHandlers/handle_load.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_model.py` & `owega-5.7.3/owega/OweHandlers/handle_model.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_presence.py` & `owega-5.7.3/owega/OweHandlers/handle_presence.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_quit.py` & `owega-5.7.3/owega/OweHandlers/handle_quit.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_save.py` & `owega-5.7.3/owega/OweHandlers/handle_save.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_system.py` & `owega-5.7.3/owega/OweHandlers/handle_system.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_temperature.py` & `owega-5.7.3/owega/OweHandlers/handle_temperature.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_tokens.py` & `owega-5.7.3/owega/OweHandlers/handle_tokens.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_top_p.py` & `owega-5.7.3/owega/OweHandlers/handle_top_p.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handle_tts.py` & `owega-5.7.3/owega/OweHandlers/handle_tts.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OweHandlers/handlers.py` & `owega-5.7.3/owega/OweHandlers/handlers.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OwegaFun/__init__.py` & `owega-5.7.3/owega/OwegaFun/__init__.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OwegaFun/functions.py` & `owega-5.7.3/owega/OwegaFun/functions.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OwegaFun/longTermSouvenirs.py` & `owega-5.7.3/owega/OwegaFun/longTermSouvenirs.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OwegaFun/utility.py` & `owega-5.7.3/owega/OwegaFun/utility.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OwegaSession/main_bottom_toolbar.py` & `owega-5.7.3/owega/OwegaSession/main_bottom_toolbar.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/OwegaSession/promptsession.py` & `owega-5.7.3/owega/OwegaSession/promptsession.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/ask.py` & `owega-5.7.3/owega/ask.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/changelog/changelog.py` & `owega-5.7.3/owega/changelog/changelog.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,21 @@
         self.version = Version(0, 0, 0)
         self.initLogs()
         self.genLog()
 
     def initLogs(self):
         """Fill the changelog."""
         self.logs.append(
+            ChangelogEntry(5, 7, 3)
+            .addLine("Better cost estimation, including input/output costs.")
+            .addLine("(added support for all GPT model as of 2024-05-14)")
+            .addLine("(added support for all mistral API models as of today)")
+            .addLine("(all other models return a cost of 0)")
+        )
+        self.logs.append(
             ChangelogEntry(5, 7, 2)
             .addLine("Added vision support for GPT-4o.")
         )
         self.logs.append(
             ChangelogEntry(5, 7, 1)
             .addLine("Fixed a non-ascii character in the DGPL.")
         )
```

### Comparing `owega-5.7.2/owega/changelog/changelogEntry.py` & `owega-5.7.3/owega/changelog/changelogEntry.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/changelog/version.py` & `owega-5.7.3/owega/changelog/version.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/config/baseConf.py` & `owega-5.7.3/owega/config/baseConf.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/conversation/conversation.py` & `owega-5.7.3/owega/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/getLogger.py` & `owega-5.7.3/owega/getLogger.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/license.py` & `owega-5.7.3/owega/license.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/owega/owega.py` & `owega-5.7.3/owega/owega.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from .changelog import OwegaChangelog
 from .config import baseConf, get_conf, list_models
 from .conversation import Conversation, Conversation_from
 from .license import OwegaLicense
 from .OwegaFun import connectLTS, existingFunctions, functionlist_to_toollist
 from .OwegaSession import OwegaSession as ps
 from .OweHandlers import handle_help, handler_helps, handlers
-from .utils import (clrtxt, do_quit, estimated_tokens, get_home_dir,
+from .utils import (clrtxt, do_quit, estimated_tokens_and_cost, get_home_dir,
                     get_temp_file, info_print, play_tts, print_help,
                     set_term_title, success_msg)
 
 
 def get_oc_conf():
     """Get a copy of owega's config."""
     return baseConf.copy()
@@ -104,26 +104,21 @@
                     temp_file,
                     messages,
                     given,
                     temp_is_temp
                 )
         if not command_found:
             if baseConf.get("estimation", False):
-                etkn = estimated_tokens(
+                etkn, cost = estimated_tokens_and_cost(
                     user_input,
                     messages,
-                    functionlist_to_toollist(existingFunctions.getEnabled())
+                    functionlist_to_toollist(existingFunctions.getEnabled()),
+                    baseConf.get('model', ''),
+                    baseConf.get("max_tokens", 4096)
                 )
-                cost_per_token = [0.001, 0.002]  # prices for gpt3-turbo
-                if 'gpt-4' in baseConf.get('model', ''):
-                    cost_per_token = [0.03, 0.06]  # prices for gpt4
-                    if 'preview' in baseConf.get('model', ''):
-                        cost_per_token = [0.01, 0.03]  # prices for gpt4-turbo
-                cost_per_token = [i/1000 for i in cost_per_token]
-                cost = (cost_per_token[0] * etkn) + (4096 * cost_per_token[1])
                 print(f"\033[37mestimated tokens: {etkn}\033[0m")
                 print(f"\033[37mestimated cost: {cost:.5f}\033[0m")
             if baseConf.get("debug", False):
                 pre_time = time.time()
             messages = ask(
                 prompt=user_input,
                 messages=messages,
@@ -255,28 +250,23 @@
         print(msgs.generate_training())
         sys.exit(0)
     if (args.estimate and not args.history):
         do_quit(
             "Can't estimate token consumption/cost without a history", value=1)
     if args.estimate:
         msgs = Conversation_from(args.history)
-        etkn = estimated_tokens(
+        etkn, cost = estimated_tokens_and_cost(
             '',
             msgs,
-            ''
+            [],
+            baseConf.get('model', ''),
+            0
         )
-        cost_per_token = [0.001, 0.002]  # prices for gpt3-turbo
-        if 'gpt-4' in baseConf.get('model', ''):
-            cost_per_token = [0.03, 0.06]  # prices for gpt4
-            if 'preview' in baseConf.get('model', ''):
-                cost_per_token = [0.01, 0.03]  # prices for gpt4-turbo
-        cost_per_token = [i/1000 for i in cost_per_token]
-        cost = (cost_per_token[0] * etkn) + (4096 * cost_per_token[1])
         print(f"estimated tokens: {etkn}")
-        print(f"estimated cost: {cost:.5f}$ (gpt-3) / {cost*10:.5f}$ (gpt-4)")
+        print(f"estimated cost: {cost:.5f}$ ({baseConf.get('model', '')})")
         sys.exit(0)
 
     input_history = ""
     if (args.history):
         input_history = args.history
 
     temp_file = get_temp_file()
```

### Comparing `owega-5.7.2/owega/utils.py` & `owega-5.7.3/owega/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         input=text
     )
     tts_answer.stream_to_file(tmpfile.name)
     play_opus(tmpfile.name)
     os.remove(tmpfile.name)
 
 
-def estimated_tokens(ppt: str, messages: Conversation, functions):
+def estimated_tokens(ppt: str, messages: Conversation, functions: list):
     """Estimate the history tokens."""
     try:
         encoder = tiktoken.encoding_for_model("gpt-4")
         req = ""
         req += ppt
         req += json.dumps(messages.get_messages())
         req += json.dumps(functions)
@@ -98,14 +98,52 @@
     except Exception as e:
         logger = getLogger.getLogger(__name__, baseConf.baseConf.get("debug"))
         logger.info("An error has occured while estimating tokens:")
         logger.info(e)
         return 0
 
 
+def estimated_cost(input_tokens: int, model: str, output_tokens: int = 4096):
+    # ppt = price per token: tuple (input, output)
+    per_k = 1000
+    per_m = 1000 * per_k
+    ppt_table = {
+        '00:gpt-4o': (5 / per_m, 15 / per_m),
+        '01:gpt-3': (0.5 / per_m, 1.5 / per_m),
+        '02:gpt-4-turbo': (10 / per_m, 30 / per_m),
+        '03:gpt-4-32k': (60 / per_m, 120 / per_m),
+        '04:gpt-4-': (30 / per_m, 60 / per_m),
+        '05:open-mistral-7b': (0.25 / per_m, 0.25 / per_m),
+        '06:open-mixtral-8x7b': (0.7 / per_m, 0.7 / per_m),
+        '07:open-mixtral-8x22b': (2 / per_m, 6 / per_m),
+        '08:mistral-small': (1 / per_m, 3 / per_m),
+        '09:mistral-medium': (2.7 / per_m, 8.1 / per_m),
+        '10:mistral-large': (4 / per_m, 12 / per_m),
+    }
+    ppt_indexes_sorted = list(sorted(ppt_table.keys()))
+    for index in ppt_indexes_sorted:
+        model_start = ':'.join(index.split(':')[1:])
+        if model.startswith(model_start):
+            ppt = ppt_table[index]
+            return (input_tokens * ppt[0]) + (output_tokens * ppt[1])
+    return 0
+
+
+def estimated_tokens_and_cost(
+    ppt: str,
+    messages: Conversation,
+    functions: list,
+    model: str,
+    output_tokens: int = 4096
+):
+    input_tokens = estimated_tokens(ppt, messages, functions)
+    cost = estimated_cost(input_tokens, model, output_tokens)
+    return (input_tokens, cost)
+
+
 def get_temp_file() -> str:
     """Get a temp file location."""
     tmp = tempfile.NamedTemporaryFile(
         prefix="owega_temp.",
         suffix=".json",
         delete=False
     )
```

### Comparing `owega-5.7.2/owega.egg-info/PKG-INFO` & `owega-5.7.3/owega.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.7.2
+Version: 5.7.3
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: DGPL-1.0
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -135,15 +135,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.7.2 CHANGELOG:
+OWEGA v5.7.3 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -364,8 +364,12 @@
 5.6.3: Fixes config's api_key not being used.
        Better docstrings on handlers.
 5.6.4: Fix for ask.ask() crashing if OPENAI_API_KEY isn't set.
 
 5.7.0: Changed the license to the DarkGeem Public License v1.0.
 5.7.1: Fixed a non-ascii character in the DGPL.
 5.7.2: Added vision support for GPT-4o.
+5.7.3: Better cost estimation, including input/output costs.
+       (added support for all GPT model as of 2024-05-14)
+       (added support for all mistral API models as of today)
+       (all other models return a cost of 0)
 ```
```

### Comparing `owega-5.7.2/owega.egg-info/SOURCES.txt` & `owega-5.7.3/owega.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owega-5.7.2/setup.py` & `owega-5.7.3/setup.py`

 * *Files identical despite different names*


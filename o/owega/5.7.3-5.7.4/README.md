# Comparing `tmp/owega-5.7.3.tar.gz` & `tmp/owega-5.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owega-5.7.3.tar", last modified: Mon May 13 23:19:25 2024, max compression
+gzip compressed data, was "owega-5.7.4.tar", last modified: Tue May 14 00:09:03 2024, max compression
```

## Comparing `owega-5.7.3.tar` & `owega-5.7.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.100103 owega-5.7.3/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6076 2024-05-10 14:44:53.000000 owega-5.7.3/LICENSE
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16292 2024-05-13 23:19:25.100103 owega-5.7.3/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5023 2024-04-17 02:21:38.000000 owega-5.7.3/README.md
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.098103 owega-5.7.3/owega/
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.099103 owega-5.7.3/owega/OweHandlers/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-27 12:05:16.000000 owega-5.7.3/owega/OweHandlers/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      980 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_add_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1590 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_commands.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1185 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_context.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1601 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_del_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_dinput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3457 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_edit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1339 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_estimation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5059 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_finput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_frequency.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      521 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_genconf.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      523 2024-05-08 02:39:07.000000 owega-5.7.3/owega/OweHandlers/handle_history.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3246 2024-05-13 23:14:07.000000 owega-5.7.3/owega/OweHandlers/handle_image.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1118 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_load.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1698 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_model.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1791 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_presence.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      637 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_quit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1090 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_save.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      945 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_system.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1739 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_temperature.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1404 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_tokens.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1556 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_top_p.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1245 2024-05-08 02:39:08.000000 owega-5.7.3/owega/OweHandlers/handle_tts.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2407 2024-04-27 12:05:16.000000 owega-5.7.3/owega/OweHandlers/handlers.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.099103 owega-5.7.3/owega/OwegaFun/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-27 12:05:16.000000 owega-5.7.3/owega/OwegaFun/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-17 02:21:38.000000 owega-5.7.3/owega/OwegaFun/functions.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4342 2024-04-27 12:05:16.000000 owega-5.7.3/owega/OwegaFun/longTermSouvenirs.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5816 2024-04-27 12:05:16.000000 owega-5.7.3/owega/OwegaFun/utility.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.099103 owega-5.7.3/owega/OwegaSession/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.7.3/owega/OwegaSession/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2763 2024-04-27 12:05:16.000000 owega-5.7.3/owega/OwegaSession/main_bottom_toolbar.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5592 2024-04-27 12:05:16.000000 owega-5.7.3/owega/OwegaSession/promptsession.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      175 2024-05-08 02:39:08.000000 owega-5.7.3/owega/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.7.3/owega/__main__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10338 2024-05-13 22:30:06.000000 owega-5.7.3/owega/ask.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.099103 owega-5.7.3/owega/changelog/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-27 12:05:16.000000 owega-5.7.3/owega/changelog/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    24778 2024-05-13 23:16:47.000000 owega-5.7.3/owega/changelog/changelog.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1534 2024-04-27 12:05:16.000000 owega-5.7.3/owega/changelog/changelogEntry.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-17 02:21:38.000000 owega-5.7.3/owega/changelog/version.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.099103 owega-5.7.3/owega/config/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.7.3/owega/config/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1810 2024-04-27 12:05:16.000000 owega-5.7.3/owega/config/baseConf.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.100103 owega-5.7.3/owega/conversation/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.7.3/owega/conversation/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10105 2024-05-13 22:26:17.000000 owega-5.7.3/owega/conversation/conversation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1418 2024-05-10 10:34:51.000000 owega-5.7.3/owega/getLogger.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.7.3/owega/handlerBase.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6141 2024-05-10 14:44:53.000000 owega-5.7.3/owega/license.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    11378 2024-05-13 23:12:32.000000 owega-5.7.3/owega/owega.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     7504 2024-05-13 23:06:32.000000 owega-5.7.3/owega/utils.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-13 23:19:25.100103 owega-5.7.3/owega.egg-info/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16292 2024-05-13 23:19:25.000000 owega-5.7.3/owega.egg-info/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1656 2024-05-13 23:19:25.000000 owega-5.7.3/owega.egg-info/SOURCES.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-05-13 23:19:25.000000 owega-5.7.3/owega.egg-info/dependency_links.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-05-13 23:19:25.000000 owega-5.7.3/owega.egg-info/entry_points.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-05-13 23:19:25.000000 owega-5.7.3/owega.egg-info/requires.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-05-13 23:19:25.000000 owega-5.7.3/owega.egg-info/top_level.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.7.3/pyproject.toml
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-05-13 23:19:25.100103 owega-5.7.3/setup.cfg
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2085 2024-05-10 13:40:23.000000 owega-5.7.3/setup.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 00:09:03.605091 owega-5.7.4/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6076 2024-05-10 14:44:53.000000 owega-5.7.4/LICENSE
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16543 2024-05-14 00:09:03.604091 owega-5.7.4/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5183 2024-05-14 00:05:54.000000 owega-5.7.4/README.md
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 00:09:03.597091 owega-5.7.4/owega/
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 00:09:03.602091 owega-5.7.4/owega/OweHandlers/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-27 12:05:16.000000 owega-5.7.4/owega/OweHandlers/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      980 2024-05-08 02:39:07.000000 owega-5.7.4/owega/OweHandlers/handle_add_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1590 2024-05-08 02:39:07.000000 owega-5.7.4/owega/OweHandlers/handle_commands.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1185 2024-05-08 02:39:07.000000 owega-5.7.4/owega/OweHandlers/handle_context.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1601 2024-05-08 02:39:07.000000 owega-5.7.4/owega/OweHandlers/handle_del_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.7.4/owega/OweHandlers/handle_dinput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3457 2024-05-08 02:39:07.000000 owega-5.7.4/owega/OweHandlers/handle_edit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1339 2024-05-08 02:39:07.000000 owega-5.7.4/owega/OweHandlers/handle_estimation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5059 2024-05-08 02:39:07.000000 owega-5.7.4/owega/OweHandlers/handle_finput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.7.4/owega/OweHandlers/handle_frequency.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      521 2024-05-08 02:39:07.000000 owega-5.7.4/owega/OweHandlers/handle_genconf.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      523 2024-05-08 02:39:07.000000 owega-5.7.4/owega/OweHandlers/handle_history.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3246 2024-05-13 23:20:56.000000 owega-5.7.4/owega/OweHandlers/handle_image.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1118 2024-05-08 02:39:08.000000 owega-5.7.4/owega/OweHandlers/handle_load.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1698 2024-05-08 02:39:08.000000 owega-5.7.4/owega/OweHandlers/handle_model.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1791 2024-05-08 02:39:08.000000 owega-5.7.4/owega/OweHandlers/handle_presence.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      637 2024-05-08 02:39:08.000000 owega-5.7.4/owega/OweHandlers/handle_quit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1090 2024-05-08 02:39:08.000000 owega-5.7.4/owega/OweHandlers/handle_save.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      945 2024-05-08 02:39:08.000000 owega-5.7.4/owega/OweHandlers/handle_system.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1739 2024-05-08 02:39:08.000000 owega-5.7.4/owega/OweHandlers/handle_temperature.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1404 2024-05-08 02:39:08.000000 owega-5.7.4/owega/OweHandlers/handle_tokens.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1556 2024-05-08 02:39:08.000000 owega-5.7.4/owega/OweHandlers/handle_top_p.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1245 2024-05-08 02:39:08.000000 owega-5.7.4/owega/OweHandlers/handle_tts.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2407 2024-04-27 12:05:16.000000 owega-5.7.4/owega/OweHandlers/handlers.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 00:09:03.602091 owega-5.7.4/owega/OwegaFun/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-27 12:05:16.000000 owega-5.7.4/owega/OwegaFun/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-17 02:21:38.000000 owega-5.7.4/owega/OwegaFun/functions.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4342 2024-04-27 12:05:16.000000 owega-5.7.4/owega/OwegaFun/longTermSouvenirs.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5816 2024-04-27 12:05:16.000000 owega-5.7.4/owega/OwegaFun/utility.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 00:09:03.603091 owega-5.7.4/owega/OwegaSession/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.7.4/owega/OwegaSession/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2763 2024-04-27 12:05:16.000000 owega-5.7.4/owega/OwegaSession/main_bottom_toolbar.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5592 2024-04-27 12:05:16.000000 owega-5.7.4/owega/OwegaSession/promptsession.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      175 2024-05-08 02:39:08.000000 owega-5.7.4/owega/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.7.4/owega/__main__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10338 2024-05-13 22:30:06.000000 owega-5.7.4/owega/ask.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 00:09:03.603091 owega-5.7.4/owega/changelog/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-27 12:05:16.000000 owega-5.7.4/owega/changelog/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    24926 2024-05-13 23:58:54.000000 owega-5.7.4/owega/changelog/changelog.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1534 2024-04-27 12:05:16.000000 owega-5.7.4/owega/changelog/changelogEntry.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-17 02:21:38.000000 owega-5.7.4/owega/changelog/version.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 00:09:03.604091 owega-5.7.4/owega/config/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.7.4/owega/config/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1810 2024-04-27 12:05:16.000000 owega-5.7.4/owega/config/baseConf.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 00:09:03.604091 owega-5.7.4/owega/conversation/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.7.4/owega/conversation/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10105 2024-05-13 22:26:17.000000 owega-5.7.4/owega/conversation/conversation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1418 2024-05-10 10:34:51.000000 owega-5.7.4/owega/getLogger.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.7.4/owega/handlerBase.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6141 2024-05-10 14:44:53.000000 owega-5.7.4/owega/license.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    11604 2024-05-13 23:58:08.000000 owega-5.7.4/owega/owega.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     7504 2024-05-13 23:20:56.000000 owega-5.7.4/owega/utils.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 00:09:03.604091 owega-5.7.4/owega.egg-info/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16543 2024-05-14 00:09:03.000000 owega-5.7.4/owega.egg-info/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1656 2024-05-14 00:09:03.000000 owega-5.7.4/owega.egg-info/SOURCES.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-05-14 00:09:03.000000 owega-5.7.4/owega.egg-info/dependency_links.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-05-14 00:09:03.000000 owega-5.7.4/owega.egg-info/entry_points.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      173 2024-05-14 00:09:03.000000 owega-5.7.4/owega.egg-info/requires.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-05-14 00:09:03.000000 owega-5.7.4/owega.egg-info/top_level.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.7.4/pyproject.toml
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-05-14 00:09:03.605091 owega-5.7.4/setup.cfg
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2109 2024-05-13 23:47:31.000000 owega-5.7.4/setup.py
```

### Comparing `owega-5.7.3/LICENSE` & `owega-5.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/PKG-INFO` & `owega-5.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.7.3
+Version: 5.7.4
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: DGPL-1.0
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -29,14 +29,15 @@
 Requires-Dist: beautifulsoup4>=4.0
 Requires-Dist: lxml>=4.0
 Requires-Dist: tiktoken>=0.5.1
 Requires-Dist: json5>=0.9.0
 Requires-Dist: pygame>=2.0
 Requires-Dist: python-editor>=1.0
 Requires-Dist: markdownify>=0.11
+Requires-Dist: setuptools>=60.0
 
 # ΦωΦ (pronounced owega)
 ΦωΦ is a command-line interface for conversing with GPT models (from OpenAI)
 
 Pypi:
 [![PyPI - Status](https://img.shields.io/pypi/status/owega)](https://pypi.org/project/owega/)
 [![PyPI - Version](https://img.shields.io/pypi/v/owega)](https://pypi.org/project/owega/)
@@ -127,23 +128,29 @@
   -s TTSFILE, --ttsfile TTSFILE
                         Outputs a generated TTS file single-ask mode
   -T, --training        outputs training data from -i file
   -e, --estimate        shows estimate token usage / cost from a request from
                         -i file
 ```
 
+
+## Markdown formatting and syntax highlighting
+To allow ΦωΦ to print its output nicely, you can just install the rich python
+module: ``pip install rich``
+
+
 ## Showcase
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.7.3 CHANGELOG:
+OWEGA v5.7.4 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -368,8 +375,9 @@
 5.7.0: Changed the license to the DarkGeem Public License v1.0.
 5.7.1: Fixed a non-ascii character in the DGPL.
 5.7.2: Added vision support for GPT-4o.
 5.7.3: Better cost estimation, including input/output costs.
        (added support for all GPT model as of 2024-05-14)
        (added support for all mistral API models as of today)
        (all other models return a cost of 0)
+5.7.4: Added pretty print if the rich module is installed.
 ```
```

### Comparing `owega-5.7.3/README.md` & `owega-5.7.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -91,11 +91,17 @@
   -s TTSFILE, --ttsfile TTSFILE
                         Outputs a generated TTS file single-ask mode
   -T, --training        outputs training data from -i file
   -e, --estimate        shows estimate token usage / cost from a request from
                         -i file
 ```
 
+
+## Markdown formatting and syntax highlighting
+To allow ΦωΦ to print its output nicely, you can just install the rich python
+module: ``pip install rich``
+
+
 ## Showcase
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
```

### Comparing `owega-5.7.3/owega/OweHandlers/handle_add_sysmem.py` & `owega-5.7.4/owega/OweHandlers/handle_add_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_commands.py` & `owega-5.7.4/owega/OweHandlers/handle_commands.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_context.py` & `owega-5.7.4/owega/OweHandlers/handle_context.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_del_sysmem.py` & `owega-5.7.4/owega/OweHandlers/handle_del_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_dinput.py` & `owega-5.7.4/owega/OweHandlers/handle_dinput.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_edit.py` & `owega-5.7.4/owega/OweHandlers/handle_edit.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_estimation.py` & `owega-5.7.4/owega/OweHandlers/handle_estimation.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_finput.py` & `owega-5.7.4/owega/OweHandlers/handle_finput.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_frequency.py` & `owega-5.7.4/owega/OweHandlers/handle_frequency.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_genconf.py` & `owega-5.7.4/owega/OweHandlers/handle_genconf.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_history.py` & `owega-5.7.4/owega/OweHandlers/handle_history.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_image.py` & `owega-5.7.4/owega/OweHandlers/handle_image.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_load.py` & `owega-5.7.4/owega/OweHandlers/handle_load.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_model.py` & `owega-5.7.4/owega/OweHandlers/handle_model.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_presence.py` & `owega-5.7.4/owega/OweHandlers/handle_presence.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_quit.py` & `owega-5.7.4/owega/OweHandlers/handle_quit.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_save.py` & `owega-5.7.4/owega/OweHandlers/handle_save.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_system.py` & `owega-5.7.4/owega/OweHandlers/handle_system.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_temperature.py` & `owega-5.7.4/owega/OweHandlers/handle_temperature.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_tokens.py` & `owega-5.7.4/owega/OweHandlers/handle_tokens.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_top_p.py` & `owega-5.7.4/owega/OweHandlers/handle_top_p.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handle_tts.py` & `owega-5.7.4/owega/OweHandlers/handle_tts.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OweHandlers/handlers.py` & `owega-5.7.4/owega/OweHandlers/handlers.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OwegaFun/__init__.py` & `owega-5.7.4/owega/OwegaFun/__init__.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OwegaFun/functions.py` & `owega-5.7.4/owega/OwegaFun/functions.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OwegaFun/longTermSouvenirs.py` & `owega-5.7.4/owega/OwegaFun/longTermSouvenirs.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OwegaFun/utility.py` & `owega-5.7.4/owega/OwegaFun/utility.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OwegaSession/main_bottom_toolbar.py` & `owega-5.7.4/owega/OwegaSession/main_bottom_toolbar.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/OwegaSession/promptsession.py` & `owega-5.7.4/owega/OwegaSession/promptsession.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/ask.py` & `owega-5.7.4/owega/ask.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/changelog/changelog.py` & `owega-5.7.4/owega/changelog/changelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,18 @@
         self.version = Version(0, 0, 0)
         self.initLogs()
         self.genLog()
 
     def initLogs(self):
         """Fill the changelog."""
         self.logs.append(
+            ChangelogEntry(5, 7, 4)
+            .addLine("Added pretty print if the rich module is installed.")
+        )
+        self.logs.append(
             ChangelogEntry(5, 7, 3)
             .addLine("Better cost estimation, including input/output costs.")
             .addLine("(added support for all GPT model as of 2024-05-14)")
             .addLine("(added support for all mistral API models as of today)")
             .addLine("(all other models return a cost of 0)")
         )
         self.logs.append(
```

### Comparing `owega-5.7.3/owega/changelog/changelogEntry.py` & `owega-5.7.4/owega/changelog/changelogEntry.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/changelog/version.py` & `owega-5.7.4/owega/changelog/version.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/config/baseConf.py` & `owega-5.7.4/owega/config/baseConf.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/conversation/conversation.py` & `owega-5.7.4/owega/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/getLogger.py` & `owega-5.7.4/owega/getLogger.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/license.py` & `owega-5.7.4/owega/license.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega/owega.py` & `owega-5.7.4/owega/owega.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,24 @@
 from .OwegaFun import connectLTS, existingFunctions, functionlist_to_toollist
 from .OwegaSession import OwegaSession as ps
 from .OweHandlers import handle_help, handler_helps, handlers
 from .utils import (clrtxt, do_quit, estimated_tokens_and_cost, get_home_dir,
                     get_temp_file, info_print, play_tts, print_help,
                     set_term_title, success_msg)
 
+try:
+    import rich
+    from rich.markdown import Markdown
+except ModuleNotFoundError:
+    def markdown_print(s: str):
+        print(s)
+else:
+    def markdown_print(s: str):
+        rich.print(Markdown(s))
+
 
 def get_oc_conf():
     """Get a copy of owega's config."""
     return baseConf.copy()
 
 
 def user_interaction_loop(temp_file="", input_file="", temp_is_temp=False):
@@ -133,15 +143,15 @@
                 post_time = time.time()
                 print(f"\033[37mrequest took {post_time-pre_time:.3f}s\033[0m")
 
             # Print the generated response
             print()
             print(' ' + clrtxt("magenta", " Owega ") + ": ")
             print()
-            print(messages.last_answer())
+            markdown_print(messages.last_answer())
 
             if baseConf.get('tts_enabled', False):
                 play_tts(messages.last_answer())
 
 
 def parse_args():
     """Parse command-line arguments."""
@@ -216,15 +226,15 @@
         temperature=baseConf.get("temperature", 0.8),
         max_tokens=baseConf.get("max_tokens", 3000),
         top_p=baseConf.get('top_p', 1.0),
         frequency_penalty=baseConf.get('frequency_penalty', 0.0),
         presence_penalty=baseConf.get('presence_penalty', 0.0)
     )
     if should_print:
-        print(messages.last_answer())
+        markdown_print(messages.last_answer())
     if baseConf.get('tts_enabled', False):
         play_tts(messages.last_answer())
     return messages.last_answer()
     if not temp_is_temp:
         messages.save(temp_file)
```

### Comparing `owega-5.7.3/owega/utils.py` & `owega-5.7.4/owega/utils.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/owega.egg-info/PKG-INFO` & `owega-5.7.4/owega.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.7.3
+Version: 5.7.4
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: DGPL-1.0
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -29,14 +29,15 @@
 Requires-Dist: beautifulsoup4>=4.0
 Requires-Dist: lxml>=4.0
 Requires-Dist: tiktoken>=0.5.1
 Requires-Dist: json5>=0.9.0
 Requires-Dist: pygame>=2.0
 Requires-Dist: python-editor>=1.0
 Requires-Dist: markdownify>=0.11
+Requires-Dist: setuptools>=60.0
 
 # ΦωΦ (pronounced owega)
 ΦωΦ is a command-line interface for conversing with GPT models (from OpenAI)
 
 Pypi:
 [![PyPI - Status](https://img.shields.io/pypi/status/owega)](https://pypi.org/project/owega/)
 [![PyPI - Version](https://img.shields.io/pypi/v/owega)](https://pypi.org/project/owega/)
@@ -127,23 +128,29 @@
   -s TTSFILE, --ttsfile TTSFILE
                         Outputs a generated TTS file single-ask mode
   -T, --training        outputs training data from -i file
   -e, --estimate        shows estimate token usage / cost from a request from
                         -i file
 ```
 
+
+## Markdown formatting and syntax highlighting
+To allow ΦωΦ to print its output nicely, you can just install the rich python
+module: ``pip install rich``
+
+
 ## Showcase
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.7.3 CHANGELOG:
+OWEGA v5.7.4 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -368,8 +375,9 @@
 5.7.0: Changed the license to the DarkGeem Public License v1.0.
 5.7.1: Fixed a non-ascii character in the DGPL.
 5.7.2: Added vision support for GPT-4o.
 5.7.3: Better cost estimation, including input/output costs.
        (added support for all GPT model as of 2024-05-14)
        (added support for all mistral API models as of today)
        (all other models return a cost of 0)
+5.7.4: Added pretty print if the rich module is installed.
 ```
```

### Comparing `owega-5.7.3/owega.egg-info/SOURCES.txt` & `owega-5.7.4/owega.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owega-5.7.3/setup.py` & `owega-5.7.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     'beautifulsoup4>=4.0',
     'lxml>=4.0',
     'tiktoken>=0.5.1',
     'json5>=0.9.0',
     'pygame>=2.0',
     'python-editor>=1.0',
     'markdownify>=0.11',
+    'setuptools>=60.0',
 ]
 
 setup(
     name='owega',
     version=oc.version_str,
     description="A command-line interface for conversing with GPT models (from OpenAI)",
     long_description=desc,
```


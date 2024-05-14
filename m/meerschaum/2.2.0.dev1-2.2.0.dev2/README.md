# Comparing `tmp/meerschaum-2.2.0.dev1.tar.gz` & `tmp/meerschaum-2.2.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meerschaum-2.2.0.dev1.tar", last modified: Fri May 10 03:58:42 2024, max compression
+gzip compressed data, was "meerschaum-2.2.0.dev2.tar", last modified: Tue May 14 04:23:01 2024, max compression
```

## Comparing `meerschaum-2.2.0.dev1.tar` & `meerschaum-2.2.0.dev2.tar`

### file list

```diff
@@ -1,299 +1,299 @@
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.739412 meerschaum-2.2.0.dev1/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-2.2.0.dev1/LICENSE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-2.2.0.dev1/NOTICE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23460 2024-05-10 03:58:42.738412 meerschaum-2.2.0.dev1/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9183 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/README.md
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.689412 meerschaum-2.2.0.dev1/meerschaum/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1487 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2763 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/__main__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.690412 meerschaum-2.2.0.dev1/meerschaum/_internal/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.690412 meerschaum-2.2.0.dev1/meerschaum/_internal/arguments/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/arguments/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10249 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/arguments/_parse_arguments.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13719 2024-05-07 20:25:34.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/arguments/_parser.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.691412 meerschaum-2.2.0.dev1/meerschaum/_internal/docs/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/docs/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7076 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/docs/index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4824 2024-03-06 17:41:41.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/entry.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.691412 meerschaum-2.2.0.dev1/meerschaum/_internal/gui/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1313 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/gui/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.691412 meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/_windows.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      935 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1596 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.691412 meerschaum-2.2.0.dev1/meerschaum/_internal/shell/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32826 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/shell/Shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3114 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/shell/ShellCompleter.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/shell/ValidAutoSuggest.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/shell/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.691412 meerschaum-2.2.0.dev1/meerschaum/_internal/shell/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/shell/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.692412 meerschaum-2.2.0.dev1/meerschaum/_internal/term/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      520 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/term/TermPageHandler.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1594 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/term/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      716 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/term/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.695412 meerschaum-2.2.0.dev1/meerschaum/actions/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11360 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/actions/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12756 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/actions/api.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13396 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/actions/bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4851 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6213 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/copy.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1167 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15528 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/actions/delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2453 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9487 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7431 2024-05-07 20:26:48.000000 meerschaum-2.2.0.dev1/meerschaum/actions/install.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2023-09-21 17:52:19.000000 meerschaum-2.2.0.dev1/meerschaum/actions/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-2.2.0.dev1/meerschaum/actions/os.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-13 21:37:33.000000 meerschaum-2.2.0.dev1/meerschaum/actions/pause.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev1/meerschaum/actions/python.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11326 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/actions/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      508 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/actions/reload.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3205 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/setup.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-2.2.0.dev1/meerschaum/actions/sh.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    26212 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/actions/show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-10-27 06:03:46.000000 meerschaum-2.2.0.dev1/meerschaum/actions/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5886 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/actions/stack.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18384 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/actions/start.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/stop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    17518 2024-03-26 19:47:08.000000 meerschaum-2.2.0.dev1/meerschaum/actions/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3053 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/actions/tag.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6068 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/uninstall.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6302 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/upgrade.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4885 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/verify.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.695412 meerschaum-2.2.0.dev1/meerschaum/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7694 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev1/meerschaum/api/_chain.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1603 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/_events.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      961 2023-08-24 00:13:16.000000 meerschaum-2.2.0.dev1/meerschaum/api/_oauth2.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1609 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/api/_websockets.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.696412 meerschaum-2.2.0.dev1/meerschaum/api/dash/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2252 2024-03-20 22:38:46.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9418 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/actions.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.697412 meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/ansi_up.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/banner_1920x320.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/favicon.ico
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/logo_48x48.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/logo_500x500.png
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.698413 meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      325 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32206 2024-05-10 03:51:40.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7689 2024-05-10 01:45:18.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2613 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3600 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6364 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/components.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2046 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/graphs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7529 2024-05-10 02:30:25.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12591 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/keys.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.698413 meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-07-21 01:07:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3930 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      595 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/error.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4600 2023-10-04 04:03:08.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1549 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2364 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    17599 2024-05-10 02:32:14.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3115 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/websockets.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3298 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/webterm.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.699412 meerschaum-2.2.0.dev1/meerschaum/api/models/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/models/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/models/_interfaces.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/models/_locations.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/models/_metrics.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-2.2.0.dev1/meerschaum/api/models/_pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.699412 meerschaum-2.2.0.dev1/meerschaum/api/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.699412 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.699412 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/bootstrap.min.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1714 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/dash.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/dbc_dark.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/styles.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5383 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/xterm.css
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.700412 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/ico/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/ico/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/ico/logo.ico
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.700412 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/action_button.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/main.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1729 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/terminado.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   289441 2024-04-05 14:30:27.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/xterm.js
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.700412 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/png/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/png/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.701412 meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/old_index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/secret.html
--rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     4443 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/termpage.html
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.702412 meerschaum-2.2.0.dev1/meerschaum/api/routes/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      564 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1849 2023-10-04 04:03:08.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1935 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2469 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21677 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6151 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7204 2023-08-24 00:13:16.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_version.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_webterm.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.702412 meerschaum-2.2.0.dev1/meerschaum/api/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      482 2023-10-26 06:22:59.000000 meerschaum-2.2.0.dev1/meerschaum/api/tables/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.704412 meerschaum-2.2.0.dev1/meerschaum/config/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11517 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/config/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5184 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/config/_default.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8218 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/config/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4419 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/config/_environment.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6635 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/config/_formatting.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1073 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/config/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1526 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/config/_patch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7983 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/config/_paths.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev1/meerschaum/config/_preprocess.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14720 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/config/_read_config.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3551 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/config/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4120 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/config/_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       76 2024-05-10 03:56:14.000000 meerschaum-2.2.0.dev1/meerschaum/config/_version.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.704412 meerschaum-2.2.0.dev1/meerschaum/config/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/config/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.704412 meerschaum-2.2.0.dev1/meerschaum/config/stack/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9034 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/config/stack/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.704412 meerschaum-2.2.0.dev1/meerschaum/config/stack/grafana/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2022-11-01 03:52:40.000000 meerschaum-2.2.0.dev1/meerschaum/config/stack/grafana/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.704412 meerschaum-2.2.0.dev1/meerschaum/config/stack/mosquitto/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/config/stack/mosquitto/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.704412 meerschaum-2.2.0.dev1/meerschaum/config/stack/mosquitto/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/config/stack/mosquitto/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.704412 meerschaum-2.2.0.dev1/meerschaum/config/stack/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/config/stack/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.704412 meerschaum-2.2.0.dev1/meerschaum/config/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4361 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/config/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.705412 meerschaum-2.2.0.dev1/meerschaum/connectors/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/Connector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12023 2023-10-04 04:03:08.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.706412 meerschaum-2.2.0.dev1/meerschaum/connectors/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4355 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/APIConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2755 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2050 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1093 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20962 2023-11-10 05:44:22.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5217 2024-05-07 20:27:04.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6922 2023-10-04 04:03:08.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_request.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5275 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4044 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/parse.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.706412 meerschaum-2.2.0.dev1/meerschaum/connectors/plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/plugin/PluginConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/plugin/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7363 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/poll.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.707412 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11522 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/SQLConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4123 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_cli.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10375 2024-03-26 20:20:31.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_create_engine.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13086 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6447 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_instance.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   100925 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8323 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34262 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3460 2023-10-26 06:22:59.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10100 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_users.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.708412 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9001 2023-12-04 02:32:59.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/tables/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/tables/types.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.708412 meerschaum-2.2.0.dev1/meerschaum/core/
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.709412 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16230 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_attributes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2261 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20880 2023-12-04 02:32:59.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_data.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10267 2023-11-13 06:20:00.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2118 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3694 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_dtypes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5234 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    28038 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14262 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_verify.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.709412 meerschaum-2.2.0.dev1/meerschaum/core/Plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev1/meerschaum/core/Plugin/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.710412 meerschaum-2.2.0.dev1/meerschaum/core/User/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2448 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/core/User/_User.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      161 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev1/meerschaum/core/User/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev1/meerschaum/core/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.710412 meerschaum-2.2.0.dev1/meerschaum/plugins/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34013 2024-05-07 20:28:41.000000 meerschaum-2.2.0.dev1/meerschaum/plugins/_Plugin.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20760 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/plugins/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.711412 meerschaum-2.2.0.dev1/meerschaum/utils/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/utils/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11460 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/utils/_get_pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.712412 meerschaum-2.2.0.dev1/meerschaum/utils/daemon/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32192 2024-03-26 19:31:51.000000 meerschaum-2.2.0.dev1/meerschaum/utils/daemon/Daemon.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19362 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/utils/daemon/RotatingFile.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8174 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/utils/daemon/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4330 2023-09-26 04:28:45.000000 meerschaum-2.2.0.dev1/meerschaum/utils/daemon/_names.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31955 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/utils/dataframe.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-2.2.0.dev1/meerschaum/utils/debug.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.712412 meerschaum-2.2.0.dev1/meerschaum/utils/dtypes/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6261 2024-03-26 20:33:15.000000 meerschaum-2.2.0.dev1/meerschaum/utils/dtypes/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14638 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/utils/dtypes/sql.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.713412 meerschaum-2.2.0.dev1/meerschaum/utils/formatting/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13778 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/utils/formatting/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3294 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/utils/formatting/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19492 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/utils/formatting/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3096 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/utils/formatting/_pprint.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3677 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/utils/formatting/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3196 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/utils/interactive.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    43296 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/utils/misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev1/meerschaum/utils/networking.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.713412 meerschaum-2.2.0.dev1/meerschaum/utils/packages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    56534 2024-03-20 22:39:01.000000 meerschaum-2.2.0.dev1/meerschaum/utils/packages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7968 2024-03-26 20:22:08.000000 meerschaum-2.2.0.dev1/meerschaum/utils/packages/_packages.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-2.2.0.dev1/meerschaum/utils/packages/lazy_loader.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2655 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/utils/pool.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-10-04 03:17:38.000000 meerschaum-2.2.0.dev1/meerschaum/utils/process.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16490 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/utils/prompt.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1951 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/utils/schedule.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    46656 2023-12-04 02:32:59.000000 meerschaum-2.2.0.dev1/meerschaum/utils/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2472 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/utils/threading.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2807 2024-03-20 22:41:20.000000 meerschaum-2.2.0.dev1/meerschaum/utils/typing.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.713412 meerschaum-2.2.0.dev1/meerschaum/utils/venv/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3553 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/utils/venv/_Venv.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23183 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/utils/venv/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6535 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/utils/warnings.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-2.2.0.dev1/meerschaum/utils/yaml.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.714412 meerschaum-2.2.0.dev1/meerschaum.egg-info/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23460 2024-05-10 03:58:42.000000 meerschaum-2.2.0.dev1/meerschaum.egg-info/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8405 2024-05-10 03:58:42.000000 meerschaum-2.2.0.dev1/meerschaum.egg-info/SOURCES.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-10 03:58:42.000000 meerschaum-2.2.0.dev1/meerschaum.egg-info/dependency_links.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2024-05-10 03:58:42.000000 meerschaum-2.2.0.dev1/meerschaum.egg-info/entry_points.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4717 2024-05-10 03:58:42.000000 meerschaum-2.2.0.dev1/meerschaum.egg-info/requires.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2024-05-10 03:58:42.000000 meerschaum-2.2.0.dev1/meerschaum.egg-info/top_level.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-10 03:58:42.000000 meerschaum-2.2.0.dev1/meerschaum.egg-info/zip-safe
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2024-05-10 03:58:42.739412 meerschaum-2.2.0.dev1/setup.cfg
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3106 2023-08-28 22:18:03.000000 meerschaum-2.2.0.dev1/setup.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.714412 meerschaum-2.2.0.dev1/tests/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3139 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/tests/test_deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15351 2023-11-13 21:37:33.000000 meerschaum-2.2.0.dev1/tests/test_pipes_dtypes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3646 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/tests/test_sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21641 2023-12-04 02:32:59.000000 meerschaum-2.2.0.dev1/tests/test_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      744 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/tests/test_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3090 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/tests/test_verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.488708 meerschaum-2.2.0.dev2/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-2.2.0.dev2/LICENSE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-2.2.0.dev2/NOTICE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23381 2024-05-14 04:23:01.487708 meerschaum-2.2.0.dev2/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9183 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev2/README.md
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.447708 meerschaum-2.2.0.dev2/meerschaum/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1487 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev2/meerschaum/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2763 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev2/meerschaum/__main__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.448708 meerschaum-2.2.0.dev2/meerschaum/_internal/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.448708 meerschaum-2.2.0.dev2/meerschaum/_internal/arguments/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/arguments/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10249 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/arguments/_parse_arguments.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13719 2024-05-07 20:25:34.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/arguments/_parser.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.448708 meerschaum-2.2.0.dev2/meerschaum/_internal/docs/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/docs/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7076 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/docs/index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4824 2024-03-06 17:41:41.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/entry.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.448708 meerschaum-2.2.0.dev2/meerschaum/_internal/gui/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1313 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/gui/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.449708 meerschaum-2.2.0.dev2/meerschaum/_internal/gui/app/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/gui/app/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/gui/app/_windows.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      935 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/gui/app/actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1596 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/gui/app/pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.449708 meerschaum-2.2.0.dev2/meerschaum/_internal/shell/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32826 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/shell/Shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3114 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/shell/ShellCompleter.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/shell/ValidAutoSuggest.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/shell/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.449708 meerschaum-2.2.0.dev2/meerschaum/_internal/shell/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/shell/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.450708 meerschaum-2.2.0.dev2/meerschaum/_internal/term/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      520 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/term/TermPageHandler.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1594 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/term/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      716 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/_internal/term/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.452708 meerschaum-2.2.0.dev2/meerschaum/actions/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11360 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev2/meerschaum/actions/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12756 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev2/meerschaum/actions/api.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13396 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev2/meerschaum/actions/bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4851 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/actions/clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6213 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/actions/copy.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1167 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/actions/deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15528 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev2/meerschaum/actions/delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2453 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/actions/drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9487 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/actions/edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7431 2024-05-07 20:26:48.000000 meerschaum-2.2.0.dev2/meerschaum/actions/install.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2023-09-21 17:52:19.000000 meerschaum-2.2.0.dev2/meerschaum/actions/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-2.2.0.dev2/meerschaum/actions/os.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-13 21:37:33.000000 meerschaum-2.2.0.dev2/meerschaum/actions/pause.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev2/meerschaum/actions/python.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11326 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev2/meerschaum/actions/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      508 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev2/meerschaum/actions/reload.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3205 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/actions/setup.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-2.2.0.dev2/meerschaum/actions/sh.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    26212 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev2/meerschaum/actions/show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-10-27 06:03:46.000000 meerschaum-2.2.0.dev2/meerschaum/actions/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5886 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev2/meerschaum/actions/stack.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18384 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev2/meerschaum/actions/start.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/actions/stop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    17518 2024-03-26 19:47:08.000000 meerschaum-2.2.0.dev2/meerschaum/actions/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3053 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev2/meerschaum/actions/tag.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6068 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/actions/uninstall.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6302 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/actions/upgrade.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4885 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/actions/verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.453708 meerschaum-2.2.0.dev2/meerschaum/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7694 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev2/meerschaum/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev2/meerschaum/api/_chain.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1603 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/api/_events.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      961 2023-08-24 00:13:16.000000 meerschaum-2.2.0.dev2/meerschaum/api/_oauth2.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1609 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev2/meerschaum/api/_websockets.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.454708 meerschaum-2.2.0.dev2/meerschaum/api/dash/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2252 2024-03-20 22:38:46.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9418 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/actions.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.454708 meerschaum-2.2.0.dev2/meerschaum/api/dash/assets/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/assets/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/assets/ansi_up.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/assets/banner_1920x320.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/assets/favicon.ico
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/assets/logo_48x48.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/assets/logo_500x500.png
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.455708 meerschaum-2.2.0.dev2/meerschaum/api/dash/callbacks/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      325 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/callbacks/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32346 2024-05-10 18:44:59.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/callbacks/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7689 2024-05-10 01:45:18.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/callbacks/jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2613 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/callbacks/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/callbacks/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3600 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/callbacks/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6364 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/components.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2046 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/graphs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7529 2024-05-10 02:30:25.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12591 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/keys.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.455708 meerschaum-2.2.0.dev2/meerschaum/api/dash/pages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-07-21 01:07:38.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/pages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3930 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/pages/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      595 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/pages/error.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4600 2023-10-04 04:03:08.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/pages/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1549 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/pages/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2364 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/pages/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18496 2024-05-10 18:08:18.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3115 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/websockets.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3298 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev2/meerschaum/api/dash/webterm.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.456708 meerschaum-2.2.0.dev2/meerschaum/api/models/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/models/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/models/_interfaces.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/models/_locations.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/models/_metrics.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-2.2.0.dev2/meerschaum/api/models/_pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.456708 meerschaum-2.2.0.dev2/meerschaum/api/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.456708 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.456708 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/css/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/css/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/css/bootstrap.min.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1714 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/css/dash.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/css/dbc_dark.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/css/styles.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5383 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/css/xterm.css
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.456708 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/ico/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/ico/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/ico/logo.ico
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.457708 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/js/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/js/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/js/action_button.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/js/main.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1729 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/js/terminado.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   289441 2024-04-05 14:30:27.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/js/xterm.js
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.457708 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/png/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/static/png/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.457708 meerschaum-2.2.0.dev2/meerschaum/api/resources/templates/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/templates/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/templates/index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/templates/old_index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/templates/secret.html
+-rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     4443 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev2/meerschaum/api/resources/templates/termpage.html
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.458708 meerschaum-2.2.0.dev2/meerschaum/api/routes/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      564 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/api/routes/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-2.2.0.dev2/meerschaum/api/routes/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1849 2023-10-04 04:03:08.000000 meerschaum-2.2.0.dev2/meerschaum/api/routes/_connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev2/meerschaum/api/routes/_index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1935 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev2/meerschaum/api/routes/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2469 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/api/routes/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21677 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev2/meerschaum/api/routes/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6151 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/api/routes/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7204 2023-08-24 00:13:16.000000 meerschaum-2.2.0.dev2/meerschaum/api/routes/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-2.2.0.dev2/meerschaum/api/routes/_version.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev2/meerschaum/api/routes/_webterm.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.458708 meerschaum-2.2.0.dev2/meerschaum/api/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      482 2023-10-26 06:22:59.000000 meerschaum-2.2.0.dev2/meerschaum/api/tables/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.459708 meerschaum-2.2.0.dev2/meerschaum/config/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11517 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev2/meerschaum/config/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5184 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev2/meerschaum/config/_default.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8218 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev2/meerschaum/config/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4419 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev2/meerschaum/config/_environment.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6635 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev2/meerschaum/config/_formatting.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1073 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/config/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1526 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev2/meerschaum/config/_patch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7983 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev2/meerschaum/config/_paths.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev2/meerschaum/config/_preprocess.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14720 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/config/_read_config.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3551 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev2/meerschaum/config/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4120 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev2/meerschaum/config/_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       76 2024-05-10 11:42:49.000000 meerschaum-2.2.0.dev2/meerschaum/config/_version.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.459708 meerschaum-2.2.0.dev2/meerschaum/config/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/config/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.459708 meerschaum-2.2.0.dev2/meerschaum/config/stack/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9012 2024-05-10 20:46:41.000000 meerschaum-2.2.0.dev2/meerschaum/config/stack/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.460708 meerschaum-2.2.0.dev2/meerschaum/config/stack/grafana/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2022-11-01 03:52:40.000000 meerschaum-2.2.0.dev2/meerschaum/config/stack/grafana/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.460708 meerschaum-2.2.0.dev2/meerschaum/config/stack/mosquitto/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/config/stack/mosquitto/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.460708 meerschaum-2.2.0.dev2/meerschaum/config/stack/mosquitto/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/config/stack/mosquitto/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.460708 meerschaum-2.2.0.dev2/meerschaum/config/stack/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/config/stack/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.460708 meerschaum-2.2.0.dev2/meerschaum/config/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4361 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev2/meerschaum/config/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.460708 meerschaum-2.2.0.dev2/meerschaum/connectors/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/Connector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12023 2023-10-04 04:03:08.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.461708 meerschaum-2.2.0.dev2/meerschaum/connectors/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4355 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/api/APIConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2755 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/api/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/api/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2050 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/api/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1093 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/api/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20962 2023-11-10 05:44:22.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/api/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5217 2024-05-07 20:27:04.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/api/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6922 2023-10-04 04:03:08.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/api/_request.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/api/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5275 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/api/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4044 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/parse.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.461708 meerschaum-2.2.0.dev2/meerschaum/connectors/plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/plugin/PluginConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/plugin/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7363 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/poll.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.462708 meerschaum-2.2.0.dev2/meerschaum/connectors/sql/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11522 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/sql/SQLConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/sql/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4123 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_cli.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10375 2024-03-26 20:20:31.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_create_engine.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13086 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6447 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_instance.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   100925 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8323 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34262 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3460 2023-10-26 06:22:59.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10100 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_users.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.462708 meerschaum-2.2.0.dev2/meerschaum/connectors/sql/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9001 2023-12-04 02:32:59.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/sql/tables/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/sql/tables/types.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev2/meerschaum/connectors/sql/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.462708 meerschaum-2.2.0.dev2/meerschaum/core/
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.464708 meerschaum-2.2.0.dev2/meerschaum/core/Pipe/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16230 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev2/meerschaum/core/Pipe/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_attributes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2261 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20880 2023-12-04 02:32:59.000000 meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_data.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10267 2023-11-13 06:20:00.000000 meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2118 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3694 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_dtypes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5234 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    28038 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14262 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.464708 meerschaum-2.2.0.dev2/meerschaum/core/Plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev2/meerschaum/core/Plugin/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.464708 meerschaum-2.2.0.dev2/meerschaum/core/User/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2448 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev2/meerschaum/core/User/_User.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      161 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev2/meerschaum/core/User/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev2/meerschaum/core/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.464708 meerschaum-2.2.0.dev2/meerschaum/plugins/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34013 2024-05-07 20:28:41.000000 meerschaum-2.2.0.dev2/meerschaum/plugins/_Plugin.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20760 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev2/meerschaum/plugins/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.466708 meerschaum-2.2.0.dev2/meerschaum/utils/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev2/meerschaum/utils/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11460 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev2/meerschaum/utils/_get_pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.466708 meerschaum-2.2.0.dev2/meerschaum/utils/daemon/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32192 2024-03-26 19:31:51.000000 meerschaum-2.2.0.dev2/meerschaum/utils/daemon/Daemon.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19362 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev2/meerschaum/utils/daemon/RotatingFile.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8174 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev2/meerschaum/utils/daemon/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4330 2023-09-26 04:28:45.000000 meerschaum-2.2.0.dev2/meerschaum/utils/daemon/_names.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31955 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev2/meerschaum/utils/dataframe.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-2.2.0.dev2/meerschaum/utils/debug.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.467708 meerschaum-2.2.0.dev2/meerschaum/utils/dtypes/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6261 2024-03-26 20:33:15.000000 meerschaum-2.2.0.dev2/meerschaum/utils/dtypes/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14638 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev2/meerschaum/utils/dtypes/sql.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.467708 meerschaum-2.2.0.dev2/meerschaum/utils/formatting/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13778 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev2/meerschaum/utils/formatting/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3294 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/utils/formatting/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19492 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev2/meerschaum/utils/formatting/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3096 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/utils/formatting/_pprint.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3677 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/utils/formatting/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3196 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev2/meerschaum/utils/interactive.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    43296 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev2/meerschaum/utils/misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev2/meerschaum/utils/networking.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.467708 meerschaum-2.2.0.dev2/meerschaum/utils/packages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    56682 2024-05-13 18:49:36.000000 meerschaum-2.2.0.dev2/meerschaum/utils/packages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7970 2024-05-13 21:25:38.000000 meerschaum-2.2.0.dev2/meerschaum/utils/packages/_packages.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-2.2.0.dev2/meerschaum/utils/packages/lazy_loader.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2655 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev2/meerschaum/utils/pool.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-10-04 03:17:38.000000 meerschaum-2.2.0.dev2/meerschaum/utils/process.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16490 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/utils/prompt.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10350 2024-05-14 04:12:21.000000 meerschaum-2.2.0.dev2/meerschaum/utils/schedule.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    46656 2023-12-04 02:32:59.000000 meerschaum-2.2.0.dev2/meerschaum/utils/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2472 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/meerschaum/utils/threading.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2807 2024-03-20 22:41:20.000000 meerschaum-2.2.0.dev2/meerschaum/utils/typing.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.467708 meerschaum-2.2.0.dev2/meerschaum/utils/venv/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3553 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev2/meerschaum/utils/venv/_Venv.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23183 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev2/meerschaum/utils/venv/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6535 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev2/meerschaum/utils/warnings.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-2.2.0.dev2/meerschaum/utils/yaml.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.468708 meerschaum-2.2.0.dev2/meerschaum.egg-info/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23381 2024-05-14 04:23:01.000000 meerschaum-2.2.0.dev2/meerschaum.egg-info/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8405 2024-05-14 04:23:01.000000 meerschaum-2.2.0.dev2/meerschaum.egg-info/SOURCES.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-14 04:23:01.000000 meerschaum-2.2.0.dev2/meerschaum.egg-info/dependency_links.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2024-05-14 04:23:01.000000 meerschaum-2.2.0.dev2/meerschaum.egg-info/entry_points.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4701 2024-05-14 04:23:01.000000 meerschaum-2.2.0.dev2/meerschaum.egg-info/requires.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2024-05-14 04:23:01.000000 meerschaum-2.2.0.dev2/meerschaum.egg-info/top_level.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-14 04:23:01.000000 meerschaum-2.2.0.dev2/meerschaum.egg-info/zip-safe
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2024-05-14 04:23:01.488708 meerschaum-2.2.0.dev2/setup.cfg
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3106 2023-08-28 22:18:03.000000 meerschaum-2.2.0.dev2/setup.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:23:01.468708 meerschaum-2.2.0.dev2/tests/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3139 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev2/tests/test_deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15351 2023-11-13 21:37:33.000000 meerschaum-2.2.0.dev2/tests/test_pipes_dtypes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3646 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/tests/test_sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21818 2024-05-10 21:08:07.000000 meerschaum-2.2.0.dev2/tests/test_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      744 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/tests/test_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3090 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev2/tests/test_verify.py
```

### Comparing `meerschaum-2.2.0.dev1/LICENSE` & `meerschaum-2.2.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/PKG-INFO` & `meerschaum-2.2.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 2.2.0.dev1
+Version: 2.2.0.dev2
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
@@ -60,15 +60,15 @@
 Requires-Dist: more-itertools>=8.7.0; extra == "required"
 Requires-Dist: python-daemon>=0.2.3; extra == "required"
 Requires-Dist: fasteners>=0.18.0; extra == "required"
 Requires-Dist: psutil>=5.8.0; extra == "required"
 Requires-Dist: watchgod>=0.7.0; extra == "required"
 Requires-Dist: dill>=0.3.3; extra == "required"
 Requires-Dist: virtualenv>=20.1.0; extra == "required"
-Requires-Dist: rocketry>=2.5.1; extra == "required"
+Requires-Dist: apscheduler>=4.0.0a4; extra == "required"
 Provides-Extra: drivers
 Requires-Dist: cryptography>=38.0.1; extra == "drivers"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "drivers"
 Requires-Dist: PyMySQL>=0.9.0; extra == "drivers"
 Requires-Dist: aiomysql>=0.0.21; extra == "drivers"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "drivers"
 Requires-Dist: duckdb>=0.9.0; extra == "drivers"
@@ -79,18 +79,18 @@
 Provides-Extra: cli
 Requires-Dist: pgcli>=3.1.0; extra == "cli"
 Requires-Dist: mycli>=1.23.2; extra == "cli"
 Requires-Dist: litecli>=1.5.0; extra == "cli"
 Requires-Dist: mssql-cli>=1.0.0; extra == "cli"
 Requires-Dist: gadwall>=0.2.0; extra == "cli"
 Provides-Extra: stack
-Requires-Dist: docker-compose>=1.27.4; extra == "stack"
+Requires-Dist: docker-compose>=1.29.2; extra == "stack"
 Provides-Extra: build
-Requires-Dist: cx_Freeze>=6.5.1; extra == "build"
-Requires-Dist: pyinstaller>=5.0.0-dev0; extra == "build"
+Requires-Dist: cx_Freeze>=7.0.0; extra == "build"
+Requires-Dist: pyinstaller>6.6.0; extra == "build"
 Provides-Extra: dev-tools
 Requires-Dist: twine>=3.2.0; extra == "dev-tools"
 Requires-Dist: tuna>=0.5.3; extra == "dev-tools"
 Requires-Dist: snakeviz>=2.1.0; extra == "dev-tools"
 Requires-Dist: mypy>=0.812.0; extra == "dev-tools"
 Requires-Dist: pytest>=6.2.2; extra == "dev-tools"
 Requires-Dist: pytest-xdist>=3.2.1; extra == "dev-tools"
@@ -151,15 +151,15 @@
 Requires-Dist: more-itertools>=8.7.0; extra == "sql"
 Requires-Dist: python-daemon>=0.2.3; extra == "sql"
 Requires-Dist: fasteners>=0.18.0; extra == "sql"
 Requires-Dist: psutil>=5.8.0; extra == "sql"
 Requires-Dist: watchgod>=0.7.0; extra == "sql"
 Requires-Dist: dill>=0.3.3; extra == "sql"
 Requires-Dist: virtualenv>=20.1.0; extra == "sql"
-Requires-Dist: rocketry>=2.5.1; extra == "sql"
+Requires-Dist: apscheduler>=4.0.0a4; extra == "sql"
 Provides-Extra: dash
 Requires-Dist: Flask-Compress>=1.10.1; extra == "dash"
 Requires-Dist: dash>=2.6.2; extra == "dash"
 Requires-Dist: dash-bootstrap-components>=1.2.1; extra == "dash"
 Requires-Dist: dash-ace>=0.2.1; extra == "dash"
 Requires-Dist: dash-extensions>=1.0.4; extra == "dash"
 Requires-Dist: dash-daq>=0.5.0; extra == "dash"
@@ -170,15 +170,14 @@
 Requires-Dist: gunicorn>=20.1.0; extra == "api"
 Requires-Dist: python-dotenv>=0.20.0; extra == "api"
 Requires-Dist: websockets>=11.0.3; extra == "api"
 Requires-Dist: fastapi>=0.100.0; extra == "api"
 Requires-Dist: passlib>=1.7.4; extra == "api"
 Requires-Dist: fastapi-login>=1.7.2; extra == "api"
 Requires-Dist: python-multipart>=0.0.5; extra == "api"
-Requires-Dist: pydantic<2.0.0; extra == "api"
 Requires-Dist: httpx>=0.24.1; extra == "api"
 Requires-Dist: numpy>=1.18.5; extra == "api"
 Requires-Dist: pandas[parquet]>=2.0.1; extra == "api"
 Requires-Dist: pyarrow>=7.0.0; extra == "api"
 Requires-Dist: dask>=2023.5.0; extra == "api"
 Requires-Dist: pytz; extra == "api"
 Requires-Dist: joblib>=0.17.0; extra == "api"
@@ -210,15 +209,15 @@
 Requires-Dist: more-itertools>=8.7.0; extra == "api"
 Requires-Dist: python-daemon>=0.2.3; extra == "api"
 Requires-Dist: fasteners>=0.18.0; extra == "api"
 Requires-Dist: psutil>=5.8.0; extra == "api"
 Requires-Dist: watchgod>=0.7.0; extra == "api"
 Requires-Dist: dill>=0.3.3; extra == "api"
 Requires-Dist: virtualenv>=20.1.0; extra == "api"
-Requires-Dist: rocketry>=2.5.1; extra == "api"
+Requires-Dist: apscheduler>=4.0.0a4; extra == "api"
 Requires-Dist: pprintpp>=0.4.0; extra == "api"
 Requires-Dist: asciitree>=0.3.3; extra == "api"
 Requires-Dist: typing-extensions>=4.7.1; extra == "api"
 Requires-Dist: pygments>=2.7.2; extra == "api"
 Requires-Dist: colorama>=0.4.3; extra == "api"
 Requires-Dist: rich>=13.4.2; extra == "api"
 Requires-Dist: more-termcolor>=1.1.3; extra == "api"
@@ -257,15 +256,15 @@
 Requires-Dist: more-itertools>=8.7.0; extra == "full"
 Requires-Dist: python-daemon>=0.2.3; extra == "full"
 Requires-Dist: fasteners>=0.18.0; extra == "full"
 Requires-Dist: psutil>=5.8.0; extra == "full"
 Requires-Dist: watchgod>=0.7.0; extra == "full"
 Requires-Dist: dill>=0.3.3; extra == "full"
 Requires-Dist: virtualenv>=20.1.0; extra == "full"
-Requires-Dist: rocketry>=2.5.1; extra == "full"
+Requires-Dist: apscheduler>=4.0.0a4; extra == "full"
 Requires-Dist: cryptography>=38.0.1; extra == "full"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "full"
 Requires-Dist: PyMySQL>=0.9.0; extra == "full"
 Requires-Dist: aiomysql>=0.0.21; extra == "full"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "full"
 Requires-Dist: duckdb>=0.9.0; extra == "full"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "full"
@@ -294,15 +293,14 @@
 Requires-Dist: gunicorn>=20.1.0; extra == "full"
 Requires-Dist: python-dotenv>=0.20.0; extra == "full"
 Requires-Dist: websockets>=11.0.3; extra == "full"
 Requires-Dist: fastapi>=0.100.0; extra == "full"
 Requires-Dist: passlib>=1.7.4; extra == "full"
 Requires-Dist: fastapi-login>=1.7.2; extra == "full"
 Requires-Dist: python-multipart>=0.0.5; extra == "full"
-Requires-Dist: pydantic<2.0.0; extra == "full"
 Requires-Dist: httpx>=0.24.1; extra == "full"
 
 <img src="https://meerschaum.io/assets/banner_1920x320.png" alt="Meerschaum banner" style="width: 100%"/>
 
 | PyPI | GitHub | Info | Stats |
 |---|---|---|---|
 | ![PyPI]( https://img.shields.io/pypi/v/meerschaum?color=%2300cc66&label=Version ) | ![GitHub Repo stars](https://img.shields.io/github/stars/bmeares/Meerschaum?style=social) | ![License](https://img.shields.io/github/license/bmeares/Meerschaum?label=License) | ![Number of plugins]( https://img.shields.io/badge/dynamic/json?color=3098c1&label=Public%20Plugins&query=num_plugins&url=https%3A%2F%2Fapi.mrsm.io%2Finfo ) |
```

### Comparing `meerschaum-2.2.0.dev1/README.md` & `meerschaum-2.2.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/__main__.py` & `meerschaum-2.2.0.dev2/meerschaum/__main__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/_internal/arguments/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/_internal/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/_internal/arguments/_parse_arguments.py` & `meerschaum-2.2.0.dev2/meerschaum/_internal/arguments/_parse_arguments.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/_internal/arguments/_parser.py` & `meerschaum-2.2.0.dev2/meerschaum/_internal/arguments/_parser.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/_internal/docs/index.py` & `meerschaum-2.2.0.dev2/meerschaum/_internal/docs/index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/_internal/entry.py` & `meerschaum-2.2.0.dev2/meerschaum/_internal/entry.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/_internal/gui/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/_internal/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/_internal/gui/app/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/_windows.py` & `meerschaum-2.2.0.dev2/meerschaum/_internal/gui/app/_windows.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/actions.py` & `meerschaum-2.2.0.dev2/meerschaum/_internal/gui/app/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/pipes.py` & `meerschaum-2.2.0.dev2/meerschaum/_internal/gui/app/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/_internal/shell/Shell.py` & `meerschaum-2.2.0.dev2/meerschaum/_internal/shell/Shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/_internal/shell/ShellCompleter.py` & `meerschaum-2.2.0.dev2/meerschaum/_internal/shell/ShellCompleter.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/_internal/shell/ValidAutoSuggest.py` & `meerschaum-2.2.0.dev2/meerschaum/_internal/shell/ValidAutoSuggest.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/_internal/term/TermPageHandler.py` & `meerschaum-2.2.0.dev2/meerschaum/_internal/term/TermPageHandler.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/_internal/term/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/_internal/term/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/_internal/term/tools.py` & `meerschaum-2.2.0.dev2/meerschaum/_internal/term/tools.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/api.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/api.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/bootstrap.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/clear.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/copy.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/copy.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/deduplicate.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/delete.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/drop.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/edit.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/install.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/install.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/login.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/os.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/os.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/pause.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/pause.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/python.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/python.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/register.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/setup.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/setup.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/sh.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/sh.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/show.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/sql.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/stack.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/stack.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/start.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/start.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/stop.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/stop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/sync.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/tag.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/tag.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/uninstall.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/uninstall.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/upgrade.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/upgrade.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/actions/verify.py` & `meerschaum-2.2.0.dev2/meerschaum/actions/verify.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/api/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/_chain.py` & `meerschaum-2.2.0.dev2/meerschaum/api/_chain.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/_events.py` & `meerschaum-2.2.0.dev2/meerschaum/api/_events.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/_oauth2.py` & `meerschaum-2.2.0.dev2/meerschaum/api/_oauth2.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/_websockets.py` & `meerschaum-2.2.0.dev2/meerschaum/api/_websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/actions.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/ansi_up.js` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/assets/ansi_up.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/banner_1920x320.png` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/assets/banner_1920x320.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/favicon.ico` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/logo_48x48.png` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/assets/logo_48x48.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/logo_500x500.png` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/assets/logo_500x500.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/dashboard.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/callbacks/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -512,28 +512,31 @@
     if connector_keys:
         num_filter += 1
     if metric_keys:
         num_filter += 1
     if location_keys:
         num_filter += 1
 
-    _ck_alone, _mk_alone, _lk_alone = False, False, False
-    _ck_filter, _mk_filter, _lk_filter = connector_keys, metric_keys, location_keys
-
+    _ck_filter = connector_keys
+    _mk_filter = metric_keys
+    _lk_filter = location_keys
     _ck_alone = (connector_keys and num_filter == 1) or instance_click
     _mk_alone = (metric_keys and num_filter == 1) or instance_click
     _lk_alone = (location_keys and num_filter == 1) or instance_click
 
     from meerschaum.utils import fetch_pipes_keys
 
     try:
         _all_keys = fetch_pipes_keys('registered', get_web_connector(ctx.states))
         _keys = fetch_pipes_keys(
-            'registered', get_web_connector(ctx.states),
-            connector_keys=_ck_filter, metric_keys=_mk_filter, location_keys=_lk_filter
+            'registered',
+            get_web_connector(ctx.states),
+            connector_keys = _ck_filter,
+            metric_keys = _mk_filter,
+            location_keys = _lk_filter,
         )
     except Exception as e:
         instance_alerts += [alert_from_success_tuple((False, str(e)))]
         _all_keys, _keys = [], []
     _connectors_options = []
     _metrics_options = []
     _locations_options = []
@@ -547,38 +550,41 @@
                 _k = 'None' if k in (None, '[None]', 'None', 'null') else k
                 options.append({'label': _k, 'value': _k})
                 _seen_keys[key_type].add(k)
 
     add_options(_connectors_options, _all_keys if _ck_alone else _keys, 'ck')
     add_options(_metrics_options, _all_keys if _mk_alone else _keys, 'mk')
     add_options(_locations_options, _all_keys if _lk_alone else _keys, 'lk')
-    connector_keys = sorted([
+    _connectors_options.sort(key=lambda x: str(x).lower())
+    _metrics_options.sort(key=lambda x: str(x).lower())
+    _locations_options.sort(key=lambda x: str(x).lower())
+    connector_keys = [
         ck
-        for ck in connector_keys 
+        for ck in connector_keys
         if ck in [
             _ck['value']
             for _ck in _connectors_options
         ]
-    ])
-    metric_keys = sorted([
+    ]
+    metric_keys = [
         mk
         for mk in metric_keys
         if mk in [
             _mk['value']
             for _mk in _metrics_options
         ]
-    ])
-    location_keys = sorted([
+    ]
+    location_keys = [
         lk
         for lk in location_keys
         if lk in [
             _lk['value']
             for _lk in _locations_options
         ]
-    ])
+    ]
     _connectors_datalist = [html.Option(value=o['value']) for o in _connectors_options]
     _metrics_datalist = [html.Option(value=o['value']) for o in _metrics_options]
     _locations_datalist = [html.Option(value=o['value']) for o in _locations_options]
     return (
         _connectors_options,
         _connectors_datalist,
         connector_keys,
```

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/jobs.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/callbacks/jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/login.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/callbacks/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/plugins.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/callbacks/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/register.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/components.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/components.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/connectors.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/graphs.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/graphs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/jobs.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/keys.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/keys.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/dashboard.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/pages/dashboard.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/error.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/pages/error.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/login.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/pages/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/plugins.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/pages/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/register.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/pages/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/pipes.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/pipes.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,61 +120,66 @@
             [
                 dbc.Col(
                     (
                         dbc.DropdownMenu(
                             label = "Manage",
                             children = [
                                 dbc.DropdownMenuItem(
-                                    'Sync',
+                                    'Delete',
                                     id = {
                                         'type': 'manage-pipe-button',
                                         'index': meta_str,
-                                        'action': 'sync',
+                                        'action': 'delete',
                                     },
                                 ),
                                 dbc.DropdownMenuItem(
                                     'Drop',
                                     id = {
                                         'type': 'manage-pipe-button',
                                         'index': meta_str,
                                         'action': 'drop',
                                     },
                                 ),
                                 dbc.DropdownMenuItem(
-                                    'Delete',
+                                    'Clear',
                                     id = {
                                         'type': 'manage-pipe-button',
                                         'index': meta_str,
-                                        'action': 'delete',
+                                        'action': 'clear',
+                                    },
+                                ),
+                                dbc.DropdownMenuItem(
+                                    'Verify',
+                                    id = {
+                                        'type': 'manage-pipe-button',
+                                        'index': meta_str,
+                                        'action': 'verify',
+                                    },
+                                ),
+                                dbc.DropdownMenuItem(
+                                    'Sync',
+                                    id = {
+                                        'type': 'manage-pipe-button',
+                                        'index': meta_str,
+                                        'action': 'sync',
                                     },
                                 ),
                             ],
-                            direction = "end",
+                            direction = "up",
                             menu_variant = "dark",
                             size = 'sm',
                             color = 'secondary',
                         )
                     ) if authenticated else [],
                     width = 2,
                 ),
-                #  dbc.Col(
-                    #  (
-                        #  dbc.Button(
-                            #  'Sync',
-                            #  size = 'sm',
-                            #  style = {'width': '100%'},
-                            #  id = {'type': 'pipe-sync-button', 'index': meta_str},
-                        #  ) if authenticated else []
-                    #  ),
-                    #  width = 2,
-                #  ),
                 dbc.Col(width=6),
                 dbc.Col(
                     dbc.Button(
-                        'Download recent data',
+                        'Download CSV',
                         size = 'sm',
                         color = 'link',
                         style = {'float': 'right'},
                         id = {'type': 'pipe-download-csv-button', 'index': meta_str},
                     ),
                     width = 4,
                 ),
@@ -240,32 +245,46 @@
 
     ### Only generate items if they're in the `active_items` list.
     items_bodies = {}
     if 'overview' in active_items:
         overview_header = [html.Thead(html.Tr([html.Th("Attribute"), html.Th("Value")]))]
         dt_name, id_name, val_name = pipe.get_columns('datetime', 'id', 'value', error=False)
         overview_rows = [
-            html.Tr([html.Td("Connector"), html.Td(f"{pipe.connector_keys}")]),
-            html.Tr([html.Td("Metric"), html.Td(f"{pipe.metric_key}")]),
-            html.Tr([html.Td("Location"), html.Td(f"{pipe.location_key}")]),
-            html.Tr([html.Td("Instance"), html.Td(f"{pipe.instance_keys}")]),
-            html.Tr([html.Td("Target Table"), html.Td(f"{pipe.target}")]),
+            html.Tr([html.Td("Connector"), html.Td(html.Pre(f"{pipe.connector_keys}"))]),
+            html.Tr([html.Td("Metric"), html.Td(html.Pre(f"{pipe.metric_key}"))]),
+            html.Tr([html.Td("Location"), html.Td(html.Pre(f"{pipe.location_key}"))]),
+            html.Tr([html.Td("Instance"), html.Td(html.Pre(f"{pipe.instance_keys}"))]),
+            html.Tr([html.Td("Target Table"), html.Td(html.Pre(f"{pipe.target}"))]),
         ]
-        for col_key, col in pipe.columns.items():
-            overview_rows.append(html.Tr([html.Td(f"'{col_key}' Index"), html.Td(col)]))
+        columns = pipe.columns.copy()
+        if columns:
+            datetime_index = columns.pop('datetime', None)
+            columns_items = []
+            if datetime_index:
+                columns_items.append(html.Li(f"{datetime_index} (datetime)"))
+            columns_items.extend([
+                html.Li(f"{col}")
+                for col_key, col in columns.items()
+            ])
+            overview_rows.append(
+                html.Tr([
+                    html.Td("Indices" if len(columns_items) != 1 else "Index"),
+                    html.Td(html.Pre(html.Ul(columns_items))),
+                ])
+            )
         tags = pipe.tags
         if tags:
             tags_items = html.Ul([
                 html.Li(tag)
                 for tag in tags
             ])
             overview_rows.append(
                 html.Tr([
                     html.Td("Tags"),
-                    html.Td(tags_items),
+                    html.Td(html.Pre(tags_items)),
                 ])
             )
 
         items_bodies['overview'] = dbc.Table(
             overview_header + [html.Tbody(overview_rows)],
             bordered=False, hover=True, striped=False,
         )
```

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/plugins.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/users.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/websockets.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/dash/webterm.py` & `meerschaum-2.2.0.dev2/meerschaum/api/dash/webterm.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/bootstrap.min.css` & `meerschaum-2.2.0.dev2/meerschaum/api/resources/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/dash.css` & `meerschaum-2.2.0.dev2/meerschaum/api/resources/static/css/dash.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/dbc_dark.css` & `meerschaum-2.2.0.dev2/meerschaum/api/resources/static/css/dbc_dark.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/xterm.css` & `meerschaum-2.2.0.dev2/meerschaum/api/resources/static/css/xterm.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/resources/static/ico/logo.ico` & `meerschaum-2.2.0.dev2/meerschaum/api/resources/static/ico/logo.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/action_button.js` & `meerschaum-2.2.0.dev2/meerschaum/api/resources/static/js/action_button.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/terminado.js` & `meerschaum-2.2.0.dev2/meerschaum/api/resources/static/js/terminado.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/xterm.js` & `meerschaum-2.2.0.dev2/meerschaum/api/resources/static/js/xterm.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/index.html` & `meerschaum-2.2.0.dev2/meerschaum/api/resources/templates/index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/old_index.html` & `meerschaum-2.2.0.dev2/meerschaum/api/resources/templates/old_index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/termpage.html` & `meerschaum-2.2.0.dev2/meerschaum/api/resources/templates/termpage.html`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/routes/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/api/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/routes/_actions.py` & `meerschaum-2.2.0.dev2/meerschaum/api/routes/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/routes/_connectors.py` & `meerschaum-2.2.0.dev2/meerschaum/api/routes/_connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/routes/_index.py` & `meerschaum-2.2.0.dev2/meerschaum/api/routes/_index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/routes/_login.py` & `meerschaum-2.2.0.dev2/meerschaum/api/routes/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/routes/_misc.py` & `meerschaum-2.2.0.dev2/meerschaum/api/routes/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/routes/_pipes.py` & `meerschaum-2.2.0.dev2/meerschaum/api/routes/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/routes/_plugins.py` & `meerschaum-2.2.0.dev2/meerschaum/api/routes/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/routes/_users.py` & `meerschaum-2.2.0.dev2/meerschaum/api/routes/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/routes/_version.py` & `meerschaum-2.2.0.dev2/meerschaum/api/routes/_version.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/api/routes/_webterm.py` & `meerschaum-2.2.0.dev2/meerschaum/api/routes/_webterm.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/config/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/config/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/config/_default.py` & `meerschaum-2.2.0.dev2/meerschaum/config/_default.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/config/_edit.py` & `meerschaum-2.2.0.dev2/meerschaum/config/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/config/_environment.py` & `meerschaum-2.2.0.dev2/meerschaum/config/_environment.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/config/_formatting.py` & `meerschaum-2.2.0.dev2/meerschaum/config/_formatting.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/config/_jobs.py` & `meerschaum-2.2.0.dev2/meerschaum/config/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/config/_patch.py` & `meerschaum-2.2.0.dev2/meerschaum/config/_patch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/config/_paths.py` & `meerschaum-2.2.0.dev2/meerschaum/config/_paths.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/config/_preprocess.py` & `meerschaum-2.2.0.dev2/meerschaum/config/_preprocess.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/config/_read_config.py` & `meerschaum-2.2.0.dev2/meerschaum/config/_read_config.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/config/_shell.py` & `meerschaum-2.2.0.dev2/meerschaum/config/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/config/_sync.py` & `meerschaum-2.2.0.dev2/meerschaum/config/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/config/stack/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/config/stack/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,14 @@
 # `edit config stack` under the docker-compose.yaml section. #
 #                                                            #
 ##############################################################
 """
 
 
 default_docker_compose_config = {
-    'version': '3.9',
     'services': {
         'db': {
             'environment': {
                 'TIMESCALEDB_TELEMETRY': 'off',
                 'POSTGRES_USER': '<DOLLAR>POSTGRES_USER',
                 'POSTGRES_DB': '<DOLLAR>POSTGRES_DB',
                 'POSTGRES_PASSWORD': '<DOLLAR>POSTGRES_PASSWORD',
```

### Comparing `meerschaum-2.2.0.dev1/meerschaum/config/stack/grafana/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/config/stack/grafana/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/config/static/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/config/static/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/Connector.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/Connector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/api/APIConnector.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/api/APIConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_actions.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/api/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_fetch.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/api/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_login.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/api/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_misc.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/api/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_pipes.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/api/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_plugins.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/api/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_request.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/api/_request.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_uri.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/api/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_users.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/api/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/parse.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/parse.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/plugin/PluginConnector.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/plugin/PluginConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/poll.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/poll.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/SQLConnector.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/sql/SQLConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_cli.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_cli.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_create_engine.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_create_engine.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_fetch.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_instance.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_instance.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_pipes.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_plugins.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_sql.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_uri.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_users.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/sql/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/tables/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/sql/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/tables/types.py` & `meerschaum-2.2.0.dev2/meerschaum/connectors/sql/tables/types.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/core/Pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_attributes.py` & `meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_attributes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_bootstrap.py` & `meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_clear.py` & `meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_data.py` & `meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_data.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_deduplicate.py` & `meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_delete.py` & `meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_drop.py` & `meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_dtypes.py` & `meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_dtypes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_edit.py` & `meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_fetch.py` & `meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_register.py` & `meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_show.py` & `meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_sync.py` & `meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_verify.py` & `meerschaum-2.2.0.dev2/meerschaum/core/Pipe/_verify.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/core/User/_User.py` & `meerschaum-2.2.0.dev2/meerschaum/core/User/_User.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/plugins/_Plugin.py` & `meerschaum-2.2.0.dev2/meerschaum/plugins/_Plugin.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/plugins/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/_get_pipes.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/_get_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/daemon/Daemon.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/daemon/Daemon.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/daemon/RotatingFile.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/daemon/RotatingFile.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/daemon/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/daemon/_names.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/daemon/_names.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/dataframe.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/debug.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/debug.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/dtypes/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/dtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/dtypes/sql.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/dtypes/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/formatting/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/formatting/_jobs.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/formatting/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/formatting/_pipes.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/formatting/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/formatting/_pprint.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/formatting/_pprint.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/formatting/_shell.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/formatting/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/interactive.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/interactive.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/misc.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/networking.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/networking.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/packages/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/packages/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """
 Functions for managing packages and virtual environments reside here.
 """
 
 from __future__ import annotations
 
-import importlib.util, os, pathlib
+import importlib.util, os, pathlib, re
 from meerschaum.utils.typing import Any, List, SuccessTuple, Optional, Union, Tuple, Dict, Iterable
 from meerschaum.utils.threading import Lock, RLock
 from meerschaum.utils.packages._packages import packages, all_packages, get_install_names
 from meerschaum.utils.venv import (
     activate_venv,
     deactivate_venv,
     venv_executable,
@@ -636,14 +636,17 @@
             return (
                 packaging_version.parse(result.available_version) > 
                 packaging_version.parse(version)
             )
 
     ### We might be depending on a prerelease.
     ### Sanity check that the required version is not greater than the installed version. 
+    if 'a' in required_version:
+        required_version = required_version.replace('a', '-dev')
+        version = version.replace('a', '-dev')
     try:
         return (
             (not semver.Version.parse(version).match(required_version))
             if required_version else False
         )
     except AttributeError as e:
         pip_install(_import_to_install_name('semver'), venv='mrsm', debug=debug)
```

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/packages/_packages.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/packages/_packages.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         'more_itertools'             : 'more-itertools>=8.7.0',
         'daemon'                     : 'python-daemon>=0.2.3',
         'fasteners'                  : 'fasteners>=0.18.0',
         'psutil'                     : 'psutil>=5.8.0',
         'watchgod'                   : 'watchgod>=0.7.0',
         'dill'                       : 'dill>=0.3.3',
         'virtualenv'                 : 'virtualenv>=20.1.0',
-        'rocketry'                   : 'rocketry>=2.5.1',
+        'apscheduler'                : 'apscheduler>=4.0.0a4',
     },
     'drivers': {
         'cryptography'               : 'cryptography>=38.0.1',
         'psycopg'                    : 'psycopg[binary]>=3.1.18',
         'pymysql'                    : 'PyMySQL>=0.9.0',
         'aiomysql'                   : 'aiomysql>=0.0.21',
         'sqlalchemy_cockroachdb'     : 'sqlalchemy-cockroachdb>=2.0.0',
@@ -71,19 +71,19 @@
         'pgcli'                      : 'pgcli>=3.1.0',
         'mycli'                      : 'mycli>=1.23.2',
         'litecli'                    : 'litecli>=1.5.0',
         'mssqlcli'                   : 'mssql-cli>=1.0.0',
         'gadwall'                    : 'gadwall>=0.2.0',
     },
     'stack': {
-        'compose'                    : 'docker-compose>=1.27.4',
+        'compose'                    : 'docker-compose>=1.29.2',
     },
     'build': {
-        'cx_Freeze'                  : 'cx_Freeze>=6.5.1',
-        'PyInstaller'                : 'pyinstaller>=5.0.0-dev0',
+        'cx_Freeze'                  : 'cx_Freeze>=7.0.0',
+        'PyInstaller'                : 'pyinstaller>6.6.0',
     },
     'dev-tools': {
         'twine'                      : 'twine>=3.2.0',
         'tuna'                       : 'tuna>=0.5.3',
         'snakeviz'                   : 'snakeviz>=2.1.0',
         'mypy'                       : 'mypy>=0.812.0',
         'pytest'                     : 'pytest>=6.2.2',
@@ -145,15 +145,15 @@
     'gunicorn'                       : 'gunicorn>=20.1.0',
     'dotenv'                         : 'python-dotenv>=0.20.0',
     'websockets'                     : 'websockets>=11.0.3',
     'fastapi'                        : 'fastapi>=0.100.0',
     'passlib'                        : 'passlib>=1.7.4',
     'fastapi_login'                  : 'fastapi-login>=1.7.2',
     'multipart'                      : 'python-multipart>=0.0.5',
-    'pydantic'                       : 'pydantic<2.0.0',
+    #  'pydantic'                       : 'pydantic>2.0.0',
     'httpx'                          : 'httpx>=0.24.1',
     'websockets'                     : 'websockets>=11.0.3',
 }
 packages['api'].update(packages['sql'])
 packages['api'].update(packages['formatting'])
 packages['api'].update(packages['dash'])
```

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/packages/lazy_loader.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/packages/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/pool.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/pool.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/process.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/process.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/prompt.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/sql.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/threading.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/threading.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/typing.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/typing.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/venv/_Venv.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/venv/_Venv.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/venv/__init__.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/venv/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/warnings.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum/utils/yaml.py` & `meerschaum-2.2.0.dev2/meerschaum/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum.egg-info/PKG-INFO` & `meerschaum-2.2.0.dev2/meerschaum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 2.2.0.dev1
+Version: 2.2.0.dev2
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
@@ -60,15 +60,15 @@
 Requires-Dist: more-itertools>=8.7.0; extra == "required"
 Requires-Dist: python-daemon>=0.2.3; extra == "required"
 Requires-Dist: fasteners>=0.18.0; extra == "required"
 Requires-Dist: psutil>=5.8.0; extra == "required"
 Requires-Dist: watchgod>=0.7.0; extra == "required"
 Requires-Dist: dill>=0.3.3; extra == "required"
 Requires-Dist: virtualenv>=20.1.0; extra == "required"
-Requires-Dist: rocketry>=2.5.1; extra == "required"
+Requires-Dist: apscheduler>=4.0.0a4; extra == "required"
 Provides-Extra: drivers
 Requires-Dist: cryptography>=38.0.1; extra == "drivers"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "drivers"
 Requires-Dist: PyMySQL>=0.9.0; extra == "drivers"
 Requires-Dist: aiomysql>=0.0.21; extra == "drivers"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "drivers"
 Requires-Dist: duckdb>=0.9.0; extra == "drivers"
@@ -79,18 +79,18 @@
 Provides-Extra: cli
 Requires-Dist: pgcli>=3.1.0; extra == "cli"
 Requires-Dist: mycli>=1.23.2; extra == "cli"
 Requires-Dist: litecli>=1.5.0; extra == "cli"
 Requires-Dist: mssql-cli>=1.0.0; extra == "cli"
 Requires-Dist: gadwall>=0.2.0; extra == "cli"
 Provides-Extra: stack
-Requires-Dist: docker-compose>=1.27.4; extra == "stack"
+Requires-Dist: docker-compose>=1.29.2; extra == "stack"
 Provides-Extra: build
-Requires-Dist: cx_Freeze>=6.5.1; extra == "build"
-Requires-Dist: pyinstaller>=5.0.0-dev0; extra == "build"
+Requires-Dist: cx_Freeze>=7.0.0; extra == "build"
+Requires-Dist: pyinstaller>6.6.0; extra == "build"
 Provides-Extra: dev-tools
 Requires-Dist: twine>=3.2.0; extra == "dev-tools"
 Requires-Dist: tuna>=0.5.3; extra == "dev-tools"
 Requires-Dist: snakeviz>=2.1.0; extra == "dev-tools"
 Requires-Dist: mypy>=0.812.0; extra == "dev-tools"
 Requires-Dist: pytest>=6.2.2; extra == "dev-tools"
 Requires-Dist: pytest-xdist>=3.2.1; extra == "dev-tools"
@@ -151,15 +151,15 @@
 Requires-Dist: more-itertools>=8.7.0; extra == "sql"
 Requires-Dist: python-daemon>=0.2.3; extra == "sql"
 Requires-Dist: fasteners>=0.18.0; extra == "sql"
 Requires-Dist: psutil>=5.8.0; extra == "sql"
 Requires-Dist: watchgod>=0.7.0; extra == "sql"
 Requires-Dist: dill>=0.3.3; extra == "sql"
 Requires-Dist: virtualenv>=20.1.0; extra == "sql"
-Requires-Dist: rocketry>=2.5.1; extra == "sql"
+Requires-Dist: apscheduler>=4.0.0a4; extra == "sql"
 Provides-Extra: dash
 Requires-Dist: Flask-Compress>=1.10.1; extra == "dash"
 Requires-Dist: dash>=2.6.2; extra == "dash"
 Requires-Dist: dash-bootstrap-components>=1.2.1; extra == "dash"
 Requires-Dist: dash-ace>=0.2.1; extra == "dash"
 Requires-Dist: dash-extensions>=1.0.4; extra == "dash"
 Requires-Dist: dash-daq>=0.5.0; extra == "dash"
@@ -170,15 +170,14 @@
 Requires-Dist: gunicorn>=20.1.0; extra == "api"
 Requires-Dist: python-dotenv>=0.20.0; extra == "api"
 Requires-Dist: websockets>=11.0.3; extra == "api"
 Requires-Dist: fastapi>=0.100.0; extra == "api"
 Requires-Dist: passlib>=1.7.4; extra == "api"
 Requires-Dist: fastapi-login>=1.7.2; extra == "api"
 Requires-Dist: python-multipart>=0.0.5; extra == "api"
-Requires-Dist: pydantic<2.0.0; extra == "api"
 Requires-Dist: httpx>=0.24.1; extra == "api"
 Requires-Dist: numpy>=1.18.5; extra == "api"
 Requires-Dist: pandas[parquet]>=2.0.1; extra == "api"
 Requires-Dist: pyarrow>=7.0.0; extra == "api"
 Requires-Dist: dask>=2023.5.0; extra == "api"
 Requires-Dist: pytz; extra == "api"
 Requires-Dist: joblib>=0.17.0; extra == "api"
@@ -210,15 +209,15 @@
 Requires-Dist: more-itertools>=8.7.0; extra == "api"
 Requires-Dist: python-daemon>=0.2.3; extra == "api"
 Requires-Dist: fasteners>=0.18.0; extra == "api"
 Requires-Dist: psutil>=5.8.0; extra == "api"
 Requires-Dist: watchgod>=0.7.0; extra == "api"
 Requires-Dist: dill>=0.3.3; extra == "api"
 Requires-Dist: virtualenv>=20.1.0; extra == "api"
-Requires-Dist: rocketry>=2.5.1; extra == "api"
+Requires-Dist: apscheduler>=4.0.0a4; extra == "api"
 Requires-Dist: pprintpp>=0.4.0; extra == "api"
 Requires-Dist: asciitree>=0.3.3; extra == "api"
 Requires-Dist: typing-extensions>=4.7.1; extra == "api"
 Requires-Dist: pygments>=2.7.2; extra == "api"
 Requires-Dist: colorama>=0.4.3; extra == "api"
 Requires-Dist: rich>=13.4.2; extra == "api"
 Requires-Dist: more-termcolor>=1.1.3; extra == "api"
@@ -257,15 +256,15 @@
 Requires-Dist: more-itertools>=8.7.0; extra == "full"
 Requires-Dist: python-daemon>=0.2.3; extra == "full"
 Requires-Dist: fasteners>=0.18.0; extra == "full"
 Requires-Dist: psutil>=5.8.0; extra == "full"
 Requires-Dist: watchgod>=0.7.0; extra == "full"
 Requires-Dist: dill>=0.3.3; extra == "full"
 Requires-Dist: virtualenv>=20.1.0; extra == "full"
-Requires-Dist: rocketry>=2.5.1; extra == "full"
+Requires-Dist: apscheduler>=4.0.0a4; extra == "full"
 Requires-Dist: cryptography>=38.0.1; extra == "full"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "full"
 Requires-Dist: PyMySQL>=0.9.0; extra == "full"
 Requires-Dist: aiomysql>=0.0.21; extra == "full"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "full"
 Requires-Dist: duckdb>=0.9.0; extra == "full"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "full"
@@ -294,15 +293,14 @@
 Requires-Dist: gunicorn>=20.1.0; extra == "full"
 Requires-Dist: python-dotenv>=0.20.0; extra == "full"
 Requires-Dist: websockets>=11.0.3; extra == "full"
 Requires-Dist: fastapi>=0.100.0; extra == "full"
 Requires-Dist: passlib>=1.7.4; extra == "full"
 Requires-Dist: fastapi-login>=1.7.2; extra == "full"
 Requires-Dist: python-multipart>=0.0.5; extra == "full"
-Requires-Dist: pydantic<2.0.0; extra == "full"
 Requires-Dist: httpx>=0.24.1; extra == "full"
 
 <img src="https://meerschaum.io/assets/banner_1920x320.png" alt="Meerschaum banner" style="width: 100%"/>
 
 | PyPI | GitHub | Info | Stats |
 |---|---|---|---|
 | ![PyPI]( https://img.shields.io/pypi/v/meerschaum?color=%2300cc66&label=Version ) | ![GitHub Repo stars](https://img.shields.io/github/stars/bmeares/Meerschaum?style=social) | ![License](https://img.shields.io/github/license/bmeares/Meerschaum?label=License) | ![Number of plugins]( https://img.shields.io/badge/dynamic/json?color=3098c1&label=Public%20Plugins&query=num_plugins&url=https%3A%2F%2Fapi.mrsm.io%2Finfo ) |
```

### Comparing `meerschaum-2.2.0.dev1/meerschaum.egg-info/SOURCES.txt` & `meerschaum-2.2.0.dev2/meerschaum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/meerschaum.egg-info/requires.txt` & `meerschaum-2.2.0.dev2/meerschaum.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -21,26 +21,25 @@
 more-itertools>=8.7.0
 python-daemon>=0.2.3
 fasteners>=0.18.0
 psutil>=5.8.0
 watchgod>=0.7.0
 dill>=0.3.3
 virtualenv>=20.1.0
-rocketry>=2.5.1
+apscheduler>=4.0.0a4
 
 [api]
 uvicorn[standard]>=0.22.0
 gunicorn>=20.1.0
 python-dotenv>=0.20.0
 websockets>=11.0.3
 fastapi>=0.100.0
 passlib>=1.7.4
 fastapi-login>=1.7.2
 python-multipart>=0.0.5
-pydantic<2.0.0
 httpx>=0.24.1
 numpy>=1.18.5
 pandas[parquet]>=2.0.1
 pyarrow>=7.0.0
 dask>=2023.5.0
 pytz
 joblib>=0.17.0
@@ -72,15 +71,15 @@
 more-itertools>=8.7.0
 python-daemon>=0.2.3
 fasteners>=0.18.0
 psutil>=5.8.0
 watchgod>=0.7.0
 dill>=0.3.3
 virtualenv>=20.1.0
-rocketry>=2.5.1
+apscheduler>=4.0.0a4
 pprintpp>=0.4.0
 asciitree>=0.3.3
 typing-extensions>=4.7.1
 pygments>=2.7.2
 colorama>=0.4.3
 rich>=13.4.2
 more-termcolor>=1.1.3
@@ -91,16 +90,16 @@
 dash-ace>=0.2.1
 dash-extensions>=1.0.4
 dash-daq>=0.5.0
 terminado>=0.12.1
 tornado>=6.1.0
 
 [build]
-cx_Freeze>=6.5.1
-pyinstaller>=5.0.0-dev0
+cx_Freeze>=7.0.0
+pyinstaller>6.6.0
 
 [cli]
 pgcli>=3.1.0
 mycli>=1.23.2
 litecli>=1.5.0
 mssql-cli>=1.0.0
 gadwall>=0.2.0
@@ -187,15 +186,15 @@
 more-itertools>=8.7.0
 python-daemon>=0.2.3
 fasteners>=0.18.0
 psutil>=5.8.0
 watchgod>=0.7.0
 dill>=0.3.3
 virtualenv>=20.1.0
-rocketry>=2.5.1
+apscheduler>=4.0.0a4
 cryptography>=38.0.1
 psycopg[binary]>=3.1.18
 PyMySQL>=0.9.0
 aiomysql>=0.0.21
 sqlalchemy-cockroachdb>=2.0.0
 duckdb>=0.9.0
 duckdb-engine>=0.9.2
@@ -224,15 +223,14 @@
 gunicorn>=20.1.0
 python-dotenv>=0.20.0
 websockets>=11.0.3
 fastapi>=0.100.0
 passlib>=1.7.4
 fastapi-login>=1.7.2
 python-multipart>=0.0.5
-pydantic<2.0.0
 httpx>=0.24.1
 
 [gui]
 toga>=0.3.0-dev29
 pywebview>=3.6.3
 pycparser>=2.21.0
 
@@ -277,11 +275,11 @@
 more-itertools>=8.7.0
 python-daemon>=0.2.3
 fasteners>=0.18.0
 psutil>=5.8.0
 watchgod>=0.7.0
 dill>=0.3.3
 virtualenv>=20.1.0
-rocketry>=2.5.1
+apscheduler>=4.0.0a4
 
 [stack]
-docker-compose>=1.27.4
+docker-compose>=1.29.2
```

### Comparing `meerschaum-2.2.0.dev1/setup.py` & `meerschaum-2.2.0.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/tests/test_deduplicate.py` & `meerschaum-2.2.0.dev2/tests/test_deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/tests/test_pipes_dtypes.py` & `meerschaum-2.2.0.dev2/tests/test_pipes_dtypes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/tests/test_sql.py` & `meerschaum-2.2.0.dev2/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/tests/test_sync.py` & `meerschaum-2.2.0.dev2/tests/test_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,26 @@
 from tests.test_users import test_register_user
 import meerschaum as mrsm
 from meerschaum import Pipe
 from meerschaum.actions import actions
 
 @pytest.fixture(autouse=True)
 def run_before_and_after(flavor: str):
+    """
+    Ensure the test user is registered before running tests.
+    """
     test_register_user(flavor)
     yield
 
 
 @pytest.mark.parametrize("flavor", get_flavors())
 def test_register_and_delete(flavor: str):
+    """
+    Verify user registration and deletion.
+    """
     pipe = all_pipes[flavor][0]
     params = pipe.parameters.copy()
     assert params is not None
     output = pipe.delete()
     pipe.parameters = params
     assert pipe.parameters is not None
     success, msg = pipe.register(debug=debug)
@@ -35,14 +41,17 @@
     pipe.parameters = params
     success, msg = pipe.register(debug=debug)
     assert success, msg
     assert pipe.parameters is not None
 
 @pytest.mark.parametrize("flavor", get_flavors())
 def test_drop_and_sync(flavor: str):
+    """
+    Verify dropping and resyncing pipes.
+    """
     pipe = all_pipes[flavor][0]
     pipe.drop()
     assert pipe.exists(debug=debug) is False
     assert pipe.columns is not None
     now1 = datetime(2021, 1, 1, 12, 0)
     data = {'datetime' : [now1], 'id' : [1], 'val': [1]}
     success, msg = pipe.sync(data, debug=debug)
@@ -714,9 +723,8 @@
     assert success, msg
 
     docs = [
         {'dt': '2023-01-03', 'id': 3},
     ]
     success, msg = pipe.sync(docs, debug=debug)
     assert success, msg
-    return pipe
     assert pipe.get_rowcount() == 3
```

### Comparing `meerschaum-2.2.0.dev1/tests/test_users.py` & `meerschaum-2.2.0.dev2/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev1/tests/test_verify.py` & `meerschaum-2.2.0.dev2/tests/test_verify.py`

 * *Files identical despite different names*


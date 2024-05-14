# Comparing `tmp/binsync-4.1.6.tar.gz` & `tmp/binsync-4.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binsync-4.1.6.tar", last modified: Tue Apr  9 22:19:09 2024, max compression
+gzip compressed data, was "binsync-4.1.7.tar", last modified: Tue May 14 02:07:11 2024, max compression
```

## Comparing `binsync-4.1.6.tar` & `binsync-4.1.7.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:09.929123 binsync-4.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-09 22:19:05.000000 binsync-4.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 22:19:05.000000 binsync-4.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-04-09 22:19:09.929123 binsync-4.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-04-09 22:19:05.000000 binsync-4.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:09.921122 binsync-4.1.6/binsync/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/binsync_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    34776 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:09.921122 binsync-4.1.6/binsync/core/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/core/cache.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27287 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/core/scheduler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20405 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/core/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/core/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:09.921122 binsync-4.1.6/binsync/extras/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:09.925123 binsync-4.1.6/binsync/interface_overrides/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/interface_overrides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/interface_overrides/angr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/interface_overrides/binja.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/interface_overrides/ghidra.py
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/interface_overrides/ida.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/loggercfg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:09.925123 binsync-4.1.6/binsync/stub_files/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/stub_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:09.925123 binsync-4.1.6/binsync/stub_files/angr_files/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/stub_files/angr_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/stub_files/angr_files/plugin.toml
--rw-r--r--   0 runner    (1001) docker     (127)    22965 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/stub_files/binsync_binja_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/stub_files/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:09.925123 binsync-4.1.6/binsync/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19696 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/config_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/control_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:09.925123 binsync-4.1.6/binsync/ui/force_push/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/force_push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/force_push/force_push.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:09.925123 binsync-4.1.6/binsync/ui/force_push/panels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/force_push/panels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/force_push/panels/functions_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/force_push/panels/globals_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/force_push/panels/table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/magic_sync_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:09.929123 binsync-4.1.6/binsync/ui/panel_tabs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/panel_tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/panel_tabs/activity_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/panel_tabs/ctx_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/panel_tabs/functions_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/panel_tabs/globals_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/panel_tabs/table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/panel_tabs/util_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-04-09 22:19:05.000000 binsync-4.1.6/binsync/ui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:09.929123 binsync-4.1.6/binsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-04-09 22:19:09.000000 binsync-4.1.6/binsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-09 22:19:09.000000 binsync-4.1.6/binsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:19:09.000000 binsync-4.1.6/binsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-09 22:19:09.000000 binsync-4.1.6/binsync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-09 22:19:09.000000 binsync-4.1.6/binsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 22:19:09.000000 binsync-4.1.6/binsync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-09 22:19:05.000000 binsync-4.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:19:09.929123 binsync-4.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:09.929123 binsync-4.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    16369 2024-04-09 22:19:05.000000 binsync-4.1.6/tests/test_angr_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-04-09 22:19:05.000000 binsync-4.1.6/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-09 22:19:05.000000 binsync-4.1.6/tests/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:07:11.694407 binsync-4.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-14 02:07:07.000000 binsync-4.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 02:07:07.000000 binsync-4.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-05-14 02:07:11.694407 binsync-4.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-05-14 02:07:07.000000 binsync-4.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:07:11.682407 binsync-4.1.7/binsync/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/binsync_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34776 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:07:11.686407 binsync-4.1.7/binsync/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/core/cache.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27287 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/core/scheduler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20405 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/core/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:07:11.686407 binsync-4.1.7/binsync/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:07:11.686407 binsync-4.1.7/binsync/interface_overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/interface_overrides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/interface_overrides/angr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/interface_overrides/binja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/interface_overrides/ghidra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/interface_overrides/ida.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/loggercfg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:07:11.686407 binsync-4.1.7/binsync/stub_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/stub_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:07:11.686407 binsync-4.1.7/binsync/stub_files/angr_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/stub_files/angr_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/stub_files/angr_files/plugin.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    22965 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/stub_files/binsync_binja_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/stub_files/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:07:11.686407 binsync-4.1.7/binsync/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19696 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/config_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/control_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:07:11.690407 binsync-4.1.7/binsync/ui/force_push/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/force_push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/force_push/force_push.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:07:11.690407 binsync-4.1.7/binsync/ui/force_push/panels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/force_push/panels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/force_push/panels/functions_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/force_push/panels/globals_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/force_push/panels/table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/magic_sync_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:07:11.690407 binsync-4.1.7/binsync/ui/panel_tabs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/panel_tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/panel_tabs/activity_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/panel_tabs/ctx_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/panel_tabs/functions_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/panel_tabs/globals_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/panel_tabs/table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/panel_tabs/util_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-05-14 02:07:07.000000 binsync-4.1.7/binsync/ui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:07:11.690407 binsync-4.1.7/binsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-05-14 02:07:11.000000 binsync-4.1.7/binsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-14 02:07:11.000000 binsync-4.1.7/binsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 02:07:11.000000 binsync-4.1.7/binsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 02:07:11.000000 binsync-4.1.7/binsync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-14 02:07:11.000000 binsync-4.1.7/binsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 02:07:11.000000 binsync-4.1.7/binsync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-14 02:07:07.000000 binsync-4.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 02:07:11.694407 binsync-4.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:07:11.690407 binsync-4.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    16369 2024-05-14 02:07:07.000000 binsync-4.1.7/tests/test_angr_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-14 02:07:07.000000 binsync-4.1.7/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-14 02:07:07.000000 binsync-4.1.7/tests/test_state.py
```

### Comparing `binsync-4.1.6/LICENSE` & `binsync-4.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/PKG-INFO` & `binsync-4.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binsync
-Version: 4.1.6
+Version: 4.1.7
 Summary: A Collaboration framework for binary analysis tasks.
 License: BSD 2 Clause
 Project-URL: Homepage, https://github.com/angr/binsync
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 Requires-Dist: sortedcontainers
 Requires-Dist: toml
 Requires-Dist: GitPython
 Requires-Dist: filelock
 Requires-Dist: pycparser
 Requires-Dist: prompt_toolkit
 Requires-Dist: tqdm
-Requires-Dist: libbs>=1.2.5
+Requires-Dist: libbs>=1.3.1
 Provides-Extra: test
 Requires-Dist: angr-management; extra == "test"
 Requires-Dist: pytest-qt; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: ghidra
 Requires-Dist: ghidra_bridge; extra == "ghidra"
```

### Comparing `binsync-4.1.6/README.md` & `binsync-4.1.7/README.md`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/__init__.py` & `binsync-4.1.7/binsync/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "4.1.6"
+__version__ = "4.1.7"
 
 
 #
 # logging
 #
 
 import logging
```

### Comparing `binsync-4.1.6/binsync/__main__.py` & `binsync-4.1.7/binsync/__main__.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/binsync_plugin.py` & `binsync-4.1.7/binsync/binsync_plugin.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/configuration.py` & `binsync-4.1.7/binsync/configuration.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/controller.py` & `binsync-4.1.7/binsync/controller.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/core/cache.py` & `binsync-4.1.7/binsync/core/cache.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/core/client.py` & `binsync-4.1.7/binsync/core/client.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/core/scheduler.py` & `binsync-4.1.7/binsync/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/core/state.py` & `binsync-4.1.7/binsync/core/state.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/core/user.py` & `binsync-4.1.7/binsync/core/user.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/installer.py` & `binsync-4.1.7/binsync/installer.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/interface_overrides/angr.py` & `binsync-4.1.7/binsync/interface_overrides/angr.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/interface_overrides/binja.py` & `binsync-4.1.7/binsync/interface_overrides/binja.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/interface_overrides/ghidra.py` & `binsync-4.1.7/binsync/interface_overrides/ghidra.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/interface_overrides/ida.py` & `binsync-4.1.7/binsync/interface_overrides/ida.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/loggercfg.py` & `binsync-4.1.7/binsync/loggercfg.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/stub_files/binsync_binja_logo.png` & `binsync-4.1.7/binsync/stub_files/binsync_binja_logo.png`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/stub_files/plugin.json` & `binsync-4.1.7/binsync/stub_files/plugin.json`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/ui/config_dialog.py` & `binsync-4.1.7/binsync/ui/config_dialog.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/ui/control_panel.py` & `binsync-4.1.7/binsync/ui/control_panel.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/ui/force_push/force_push.py` & `binsync-4.1.7/binsync/ui/force_push/force_push.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/ui/force_push/panels/functions_table.py` & `binsync-4.1.7/binsync/ui/force_push/panels/functions_table.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/ui/force_push/panels/globals_table.py` & `binsync-4.1.7/binsync/ui/force_push/panels/globals_table.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/ui/force_push/panels/table_model.py` & `binsync-4.1.7/binsync/ui/force_push/panels/table_model.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/ui/magic_sync_dialog.py` & `binsync-4.1.7/binsync/ui/magic_sync_dialog.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/ui/panel_tabs/activity_table.py` & `binsync-4.1.7/binsync/ui/panel_tabs/activity_table.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/ui/panel_tabs/ctx_table.py` & `binsync-4.1.7/binsync/ui/panel_tabs/ctx_table.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/ui/panel_tabs/functions_table.py` & `binsync-4.1.7/binsync/ui/panel_tabs/functions_table.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/ui/panel_tabs/globals_table.py` & `binsync-4.1.7/binsync/ui/panel_tabs/globals_table.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/ui/panel_tabs/table_model.py` & `binsync-4.1.7/binsync/ui/panel_tabs/table_model.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/ui/panel_tabs/util_panel.py` & `binsync-4.1.7/binsync/ui/panel_tabs/util_panel.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync/ui/utils.py` & `binsync-4.1.7/binsync/ui/utils.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/binsync.egg-info/PKG-INFO` & `binsync-4.1.7/binsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binsync
-Version: 4.1.6
+Version: 4.1.7
 Summary: A Collaboration framework for binary analysis tasks.
 License: BSD 2 Clause
 Project-URL: Homepage, https://github.com/angr/binsync
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 Requires-Dist: sortedcontainers
 Requires-Dist: toml
 Requires-Dist: GitPython
 Requires-Dist: filelock
 Requires-Dist: pycparser
 Requires-Dist: prompt_toolkit
 Requires-Dist: tqdm
-Requires-Dist: libbs>=1.2.5
+Requires-Dist: libbs>=1.3.1
 Provides-Extra: test
 Requires-Dist: angr-management; extra == "test"
 Requires-Dist: pytest-qt; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: ghidra
 Requires-Dist: ghidra_bridge; extra == "ghidra"
```

### Comparing `binsync-4.1.6/binsync.egg-info/SOURCES.txt` & `binsync-4.1.7/binsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/pyproject.toml` & `binsync-4.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "sortedcontainers",
     "toml",
     "GitPython",
     "filelock",
     "pycparser",
     "prompt_toolkit",
     "tqdm",
-    "libbs>=1.2.5"
+    "libbs>=1.3.1"
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
```

### Comparing `binsync-4.1.6/tests/test_angr_gui.py` & `binsync-4.1.7/tests/test_angr_gui.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/tests/test_client.py` & `binsync-4.1.7/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.6/tests/test_state.py` & `binsync-4.1.7/tests/test_state.py`

 * *Files identical despite different names*

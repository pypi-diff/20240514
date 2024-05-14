# Comparing `tmp/pymodaq_plugins_physik_instrumente-1.1.1.tar.gz` & `tmp/pymodaq_plugins_physik_instrumente-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_physik_instrumente-1.1.1.tar", last modified: Mon Nov 20 15:30:23 2023, max compression
+gzip compressed data, was "pymodaq_plugins_physik_instrumente-1.2.0.tar", last modified: Tue May 14 09:31:20 2024, max compression
```

## Comparing `pymodaq_plugins_physik_instrumente-1.1.1.tar` & `pymodaq_plugins_physik_instrumente-1.2.0.tar`

### file list

```diff
@@ -1,52 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:30:23.669559 pymodaq_plugins_physik_instrumente-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2023-11-20 15:30:23.665559 pymodaq_plugins_physik_instrumente-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-20 15:30:23.669559 pymodaq_plugins_physik_instrumente-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:30:23.657559 pymodaq_plugins_physik_instrumente-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:30:23.661558 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:30:23.661558 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13512 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI.py
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI_E870.py
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI_MMC.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:30:23.661558 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:30:23.661558 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_0D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:30:23.661558 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_1D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:30:23.661558 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_2D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:30:23.661558 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_ND/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:30:23.661558 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:30:23.665559 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.H
--rw-r--r--   0 runner    (1001) docker     (127)    68608 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.dll
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.H
--rw-r--r--   0 runner    (1001) docker     (127)    12429 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.c
--rw-r--r--   0 runner    (1001) docker     (127)    22270 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.lib
--rw-r--r--   0 runner    (1001) docker     (127)    68608 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC_418.dll
--rw-r--r--   0 runner    (1001) docker     (127)   649494 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/MercuryNativeCommands_MS176E101.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   300347 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/Mercury_DLL-LV_MS177E500.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14667 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/mmc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:30:23.665559 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/resources/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/resources/config_template.toml
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:30:23.661558 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2023-11-20 15:30:23.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2023-11-20 15:30:23.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 15:30:23.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-11-20 15:30:23.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-11-20 15:30:23.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-20 15:30:23.000000 pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:30:23.665559 pymodaq_plugins_physik_instrumente-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2023-11-20 15:30:07.000000 pymodaq_plugins_physik_instrumente-1.1.1/tests/test_plugin_package_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:20.900982 pymodaq_plugins_physik_instrumente-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-14 09:31:20.896982 pymodaq_plugins_physik_instrumente-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 09:31:20.900982 pymodaq_plugins_physik_instrumente-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:20.888982 pymodaq_plugins_physik_instrumente-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:20.888982 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:20.892982 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12876 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PILegacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI_E870.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI_MMC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI_MMCLegacy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:20.892982 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:20.892982 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_0D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:20.892982 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_1D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:20.892982 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_2D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:20.892982 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:20.892982 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:20.896982 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.H
+-rw-r--r--   0 runner    (1001) docker     (127)    68608 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.dll
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.H
+-rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22270 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.lib
+-rw-r--r--   0 runner    (1001) docker     (127)    68608 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC_418.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   649494 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MercuryNativeCommands_MS176E101.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   300347 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/Mercury_DLL-LV_MS177E500.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17958 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/mmc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/mmc_wrapper_client64.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12692 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/pi_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:20.896982 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/resources/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/resources/config_template.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:20.896982 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-14 09:31:20.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-14 09:31:20.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 09:31:20.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-14 09:31:20.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 09:31:20.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 09:31:20.000000 pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:31:20.896982 pymodaq_plugins_physik_instrumente-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-14 09:31:07.000000 pymodaq_plugins_physik_instrumente-1.2.0/tests/test_plugin_package_structure.py
```

### Comparing `pymodaq_plugins_physik_instrumente-1.1.1/LICENSE` & `pymodaq_plugins_physik_instrumente-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-1.1.1/setup.py` & `pymodaq_plugins_physik_instrumente-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI.py` & `pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PILegacy.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,51 +10,23 @@
 import serial.tools.list_ports as list_ports
 
 from pymodaq.control_modules.move_utility_classes import DAQ_Move_base, main, comon_parameters_fun
 from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo, is_64bits, find_keys_from_val
 from pymodaq.utils.parameter.utils import iter_children
 
 
-from pymodaq_plugins_physik_instrumente.utils import Config
-
-config = Config()
+from pymodaq_plugins_physik_instrumente.utils import Config, get_devices_and_dlls
 
 
+config = Config()
 possible_dll_names = config['dll_names']
-
-dll_in_testing_order = []
-
-for dll_name in possible_dll_names:
-    if is_64bits():
-        filename = f'{dll_name}_x64.dll'
-    else:
-        filename = f'{dll_name}.dll'
-    file_path = Path(get_gcstranslator_dir()).joinpath(filename)
-    if file_path.is_file():
-        dll_in_testing_order.append(filename)
-
-devices = []
-dll_names = []
-devices_name = []
-for _dll_name in dll_in_testing_order:
-    gcs_device = GCSDevice(gcsdll=_dll_name)
-    _devices = []
-    _devices.extend(gcs_device.EnumerateUSB())
-    _devices.extend(gcs_device.EnumerateTCPIPDevices())
-    for dev in _devices:
-        dll_names.append(_dll_name)
-        devices.append(f'{dev}/{_dll_name}')
-    devices_name.extend(_devices)
-
-com_ports = list(list_ports.comports())
-devices.extend([str(port.name) for port in com_ports])
-dll_names.extend(['serial' for port in com_ports])
+devices, devices_name, dll_names = get_devices_and_dlls(possible_dll_names)
 
 
-class DAQ_Move_PI(DAQ_Move_base):
+class DAQ_Move_PILegacy(DAQ_Move_base):
     """
     Plugin using the pipython package wrapper. It is compatible with :
     DLLDEVICES = {
     'PI_GCS2_DLL': ['C-413', 'C-663.11', 'C-863.11', 'C-867', 'C-877', 'C-884', 'C-885', 'C-887',
                     'C-891', 'E-517', 'E-518', 'E-545', 'E-709', 'E-712', 'E-723', 'E-725',
                     'E-727', 'E-753', 'E-754', 'E-755', 'E-852B0076', 'E-861', 'E-870', 'E-871',
                     'E-873', 'C-663.12'],
@@ -148,24 +120,28 @@
         """
 
         try:
             self.close()
         except Exception as e:
             pass
         index = devices.index(self.settings['devices'])
-        return GCSDevice(gcsdll=dll_names[index])
+        gcsdll = dll_names[index]
+        if gcsdll == 'serial':
+            return GCSDevice()
+        else:
+            return GCSDevice(gcsdll=gcsdll)
 
     def connect_device(self):
         if not self.settings['dc_options', 'is_daisy']:  # simple connection
             if self.settings['connect_type'] == 'USB':
                 self.controller.ConnectUSB(self.device)
             elif self.settings['connect_type'] == 'TCP/IP':
                 self.controller.ConnectTCPIPByDescription(self.device)
             elif self.settings['connect_type'] == 'RS232':
-                self.controller.ConnectRS232(int(self.device[3:]))
+                self.controller.ConnectRS232(int(self.device[3:]), 19200)
                 # in this case device is a COM port, and one should use 1 for COM1 for instance
 
         else:  # one use a daisy chain connection with a master device and slaves
             if self.settings['dc_options', 'is_daisy_master']:  # init the master
 
                 if self.settings['connect_type'] == 'USB':
                     dev_ids = self.controller.OpenUSBDaisyChain(self.device)
```

### Comparing `pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI_E870.py` & `pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI_E870.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI_MMC.py` & `pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI_MMCLegacy.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #is64bit = sys.maxsize > 2**32
 if (sys.maxsize > 2**32):
     raise Exception("It must a python 32 bit version")
 
 ports = MMC_Wrapper.ports
 
 
-class DAQ_Move_PI_MMC(DAQ_Move_base):
+class DAQ_Move_PI_MMCLegacy(DAQ_Move_base):
     """
         Wrapper object to access the Physik Instrumente fonctionnalities, similar wrapper for all controllers.
 
         =============== =======================
         **Attributes**   **Type**
         *GCS_path*       string
         *gcs_device*     string
@@ -42,33 +42,28 @@
 
     _controller_units = 'mm'  # dependent on the stage type so to be updated accordingly using self.controller_units = new_unit
 
     com_ports = MMC_Wrapper.aliases
     controller_addresses = []
     is_multiaxes=False
     stage_names=[]
+    _epsilon = 0.1
 
     params= [{'title': 'COM Ports:', 'name': 'com_port', 'type': 'list', 'limits': com_ports},
            {'title': 'Controller_address:', 'name': 'controller_address', 'type': 'list', 'limits': controller_addresses},
            {'title': 'Stages:', 'name': 'stage', 'type': 'list', 'limits': list(MMC_Wrapper.stages.keys())},
            {'title': 'Closed loop?:', 'name': 'closed_loop', 'type': 'bool', 'value': True},
            {'title': 'Controller ID:', 'name': 'controller_id', 'type': 'str', 'value': '', 'readonly': True},
            ] + comon_parameters_fun(is_multiaxes, stage_names, epsilon=_epsilon)
 
-
-
-
-
     def __init__(self,parent=None,params_state=None):
 
         super().__init__(parent,params_state)
         self.settings.child(('epsilon')).setValue(0.01)
 
-
-
     def commit_settings(self,param):
         """
             | Activate any parameter changes on the PI_GCS2 hardware.
             |
             | Called after a param_tree_changed signal from DAQ_Move_main.
 
             =============== ================================ ========================
@@ -82,15 +77,15 @@
         """
         try:
             if param.name() == 'stage':
                 self.controller.stage = param.value()
 
             elif param.name() == 'controller_address':
                 self.controller.MMC_select(param.value())
-                self.check_position()
+                self.get_actuator_value()
 
 
         except Exception as e:
             self.emit_status(ThreadCommand("Update_Status", [getLineInfo()+ str(e), 'log']))
 
 
     def enumerate_devices(self):
@@ -130,15 +125,15 @@
                     self.controller=controller
             else: #Master stage
                 self.controller = MMC_Wrapper(com_port=self.settings.child('com_port').value())
                 self.controller.open()
                 devices = self.enumerate_devices()
                 self.controller.MMC_select(devices[0])
 
-            self.check_position()
+            self.get_actuator_value()
 
             self.status.controller=self.controller
             self.status.info=""
             self.status.controller=self.controller
             self.status.initialized=True
             return self.status
 
@@ -161,42 +156,38 @@
             See Also
             --------
             DAQ_Move_base.move_done
         """
         self.controller.MMC_globalBreak()
         self.move_done()
 
-    def check_position(self):
+    def get_actuator_value(self):
         """
             Get the current hardware position with scaling conversion of the PI_GCS2 instrument provided by get_position_with_scaling
 
             See Also
             --------
             DAQ_Move_base.get_position_with_scaling, daq_utils.ThreadCommand
         """
         pos = self.controller.getPos()
         pos=self.get_position_with_scaling(pos)
         self.current_position = pos
-        self.emit_status(ThreadCommand('check_position',[pos]))
         return pos
 
-    def move_Abs(self,position):
+    def move_abs(self,position):
         """
         """
 
         position=self.check_bound(position)
         self.target_position=position
 
         position=self.set_position_with_scaling(position)
         out=self.controller.moveAbs(self.settings.child('controller_address').value(), position)
 
-        self.poll_moving()
-
-
-    def move_Rel(self,position):
+    def move_rel(self,position):
         """
             Make the hardware relative move of the PI_GCS2 instrument from the given position after thread command signal was received in DAQ_Move_main.
 
             =============== ========= =======================
             **Parameters**  **Type**   **Description**
 
             *position*       float     The absolute position
@@ -208,31 +199,30 @@
 
         """
         position=self.check_bound(self.current_position+position)-self.current_position
         self.target_position=position+self.current_position
         position = self.set_position_relative_with_scaling(position)
 
         out=self.controller.moveRel(self.settings.child('controller_address').value(), position)
-        self.poll_moving()
 
-    def move_Home(self):
+    def move_home(self):
         """
 
             See Also
             --------
             DAQ_Move_PI.set_referencing, DAQ_Move_base.poll_moving
         """
         self.controller.find_home()
         moving = True
-        pos = self.check_position()
+        pos = self.get_actuator_value()
         while moving:
-            pos_tmp = self.check_position()
+            pos_tmp = self.get_actuator_value()
             moving = abs(pos - pos_tmp) > 0.001
             QThread.msleep(100)
             pos = pos_tmp
         self.controller.MMC_sendCommand('DH')  #to define it as home
         QThread.msleep(500)
-        self.check_position()
+        self.get_actuator_value()
 
 
 if __name__ == '__main__':
     main(__file__, init=True)
```

### Comparing `pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.H` & `pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.H`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.dll` & `pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.dll`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.H` & `pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.H`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.c` & `pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.c`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.lib` & `pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.lib`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC_418.dll` & `pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC_418.dll`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/MercuryNativeCommands_MS176E101.pdf` & `pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/MercuryNativeCommands_MS176E101.pdf`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/Mercury_DLL-LV_MS177E500.pdf` & `pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/Mercury_DLL-LV_MS177E500.pdf`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/hardware/PI/mmc_wrapper.py` & `pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/hardware/PI/mmc_wrapper.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 import sys
-from ctypes import windll, create_string_buffer, POINTER, byref, pointer
-from ctypes import c_uint, c_int, c_char, c_char_p, c_void_p, c_short, c_long, c_bool, c_double, c_uint64, c_uint32, Array, CFUNCTYPE, WINFUNCTYPE
-from ctypes import c_ushort, c_ulong, c_float
+
+from abc import ABC, abstractmethod
+from ctypes import windll, create_string_buffer, byref
 import os
+
 from pyvisa import ResourceManager
-from bitstring import Bits
 
-class MMC_Wrapper(object):
+try:
+    from msl.loadlib import Server32
+    server32 = True
+except ImportError:
+    Server32 = object
+    server32 = False
+
+
+def bitarray(integer: int):
+    binary_string = bin(integer)[2:]
+    return [int(bit) for bit in binary_string]
+
+
+class MMCBase(ABC):
     """
     Wrapper to the MMC dll from Physik Instrumente
 
     """
     stages = {'M521DG': dict(cts_units_num=2458624, cts_units_denom=81, units="mm")}
     VISA_rm = ResourceManager()
     ress = VISA_rm.list_resources_info()
@@ -20,26 +33,25 @@
         if ress[key].alias is not None:
             if 'COM' in ress[key].alias:
                 aliases.append(ress[key].alias)
                 ports.append(ress[key].interface_board_number)
 
     baudrates = [9600, 19200]
 
-    def __init__(self,stage='M521DG', com_port='COM1', baud_rate=9600):
+    def __init__(self, stage='M521DG', com_port='COM1', baud_rate=9600):
+
         if stage not in self.stages.keys():
             raise Exception('not valid stage')
         if com_port not in self.aliases:
             raise IOError('invalid com port')
         if baud_rate not in self.baudrates:
             raise IOError('invalid baudrate')
         self.stage = stage
-        super(MMC_Wrapper,self).__init__()
         self._comport = com_port
         self._baudrate = baud_rate
-        self._dll = windll.LoadLibrary(os.path.join(os.path.split(__file__)[0],'MMC.dll'))
 
     @property
     def comport(self):
         return self._comport
 
     @comport.setter
     def comport(self,port):
@@ -63,15 +75,15 @@
 
     def counts_to_units(self,counts):
         return counts*1/(self.stages[self.stage]['cts_units_num']/self.stages[self.stage]['cts_units_denom'])
 
     def units_to_counts(self,units):
         return int(units/(self.stages[self.stage]['cts_units_denom']/self.stages[self.stage]['cts_units_num']))
 
-    def moveAbs(self,axis, units):
+    def moveAbs(self, axis, units):
         """
         displacement in the selected stage units
         Parameters
         ----------
         units: (float)
         """
         self.MMC_moveA(axis, self.units_to_counts(units))
@@ -86,80 +98,163 @@
         self.MMC_moveR(axis, self.units_to_counts(units))
 
     def getPos(self):
         return self.counts_to_units(self.MMC_getPos())
 
     def open(self):
         port = self.ports[self.aliases.index(self._comport)]
-        self.MMC_COM_open(port,self._baudrate)
+        self.MMC_COM_open(port, self._baudrate)
+
+    def close(self):
+        self.MMC_COM_close()
+
+    def stop(self):
+        self.MMC_globalBreak()
 
     def find_home(self):
         self.MMC_sendCommand('FE1')
 
     def moving(self):
         target = self.MMC_getVal(2)
         self.MMC_sendCommand('TE')
         st = self.MMC_getStringCR()
         if '-' in st:
             pos = -int(st.split('E:-')[1])
         else:
             pos = int(st.split('E:+')[1])
         return abs(target - pos) > 100
 
+    @abstractmethod
+    def MMC_moveA(self, axis: int = 0, position: int = 0):
+        pass
+
+    @abstractmethod
+    def MMC_moveR(self, axis: int = 0, position: int = 0):
+        pass
+
+    @abstractmethod
+    def MMC_getPos(self):
+        pass
+
+    @abstractmethod
+    def MMC_COM_open(self, port: int, baudrate: int):
+        pass
+
+    @abstractmethod
+    def MMC_COM_close(self):
+        pass
+
+    @abstractmethod
+    def MMC_globalBreak(self):
+        pass
+
+    @abstractmethod
+    def MMC_sendCommand(self, cmd: str):
+        pass
+
+    @abstractmethod
+    def MMC_getVal(self, cmd: int):
+        pass
+
+    @abstractmethod
+    def MMC_getStringCR(self) -> str:
+        pass
+
+    @abstractmethod
+    def MMC_select(self, axis: int = 0):
+        """
+        Selects the specified axis (device) to enable communication with it.
+        Unlike the MMC_setDevice function, here the registration status is checked, so this function requires that the
+        MMC_initNetwork function have been called previously at the beginning of the program.
+        Parameters
+        ----------
+        axis: (int) range 1 to 16 Device number of the controller that is to be selected for communication.
+        """
+        pass
+
+    @abstractmethod
+    def MMC_initNetwork(self, maxAxis: int = 16):
+        """
+        Searches all addresses, starting at address maxAxis down to 1 for Mercury™ devices connected.
+        If a Mercury™ device (can be C-862, C-863, C-663 or C-170) is found, it is registered so as to allow access through the MMC_select() function.
+        The function MMC_initNetwork is optional. If it is not used, devices can be activated anyway using the MMC_setDevice function.
+        Parameters
+        ----------
+        maxAxis: (int) This parameter represents the highest device number from which the search is to run, continuing downwards.
+                        If you have 3 Mercury™s connected at the addresses 0,1 and 2 (this equals the device numbers 1,2 and 3) you may call the function as MMC_initNetwork(3).
+                        If you do no know what addresses the controllers are set to, call the function with maxAxis = 16 to find all devices connected. (Remember that valid device numbers range from 1 to 16.)
+                        The range of maxAxis is 1 to 16
+                        Because scanning each address takes about 0.5 seconds, it saves time to not start at device numbers higher than required.
+        Returns
+        -------
+        list: list of integers corresponding to the connected devices
+        """
+        pass
+
+
+
+class MMC_Wrapper(MMCBase, Server32):
+    def __init__(self, host='', port=0, stage='M521DG', com_port='COM1', baud_rate=9600):
+        if server32:
+            Server32.__init__(self, 'MMC.dll',
+                              'windll', host, port)
+        else:
+            Server32.__init__(self)
+            self._lib = windll.LoadLibrary(os.path.join(os.path.split(__file__)[0], 'MMC.dll'))
+        MMCBase.__init__(self, stage, com_port, baud_rate)
+
     def MMC_getStringCR(self):
         st = create_string_buffer(128)
-        res = self._dll.MMC_getStringCR(byref(st))
+        res = self.lib.MMC_getStringCR(byref(st))
         if res != 0:
             return st.decode()
         else:
             raise IOError('wrong return from dll')
 
     def MMC_COM_open(self, port_number, baudrate):
-        res = self._dll.MMC_COM_open(port_number, baudrate)
+        res = self.lib.MMC_COM_open(port_number, baudrate)
         if res != 0:
             raise IOError('wrong return from dll')
 
     def MMC_COM_close(self):
         """
         Closes the COM port previously opened by the MMC_COM_open function.
 
         """
-        res = self._dll.MMC_COM_close()
+        res = self.lib.MMC_COM_close()
         if res != 0:
             raise IOError('wrong return from dll')
 
     def MMC_COM_EOF(self):
         """
         Returns the number of characters available in the COM-port input buffer
         Returns
         -------
         int: Number of characters in the input buffer
         """
-        res = self._dll.MMC_COM_EOF()
+        res = self.lib.MMC_COM_EOF()
         return res
 
     def MMC_COM_clear(self):
         """
         Clears the COM-port input buffer.
         """
-        res = self._dll.MMC_COM_clear()
+        res = self.lib.MMC_COM_clear()
         if res != 0:
             raise IOError('wrong return from dll')
 
-
-
     def MMC_getDLLversion(self):
         """
         Delivers the version number of the DLL
         Returns
         -------
         int: version number as integer
 
         """
-        res = self._dll.MMC_getDLLversion()
+        res = self.lib.MMC_getDLLversion()
         return res
 
 
     def MMC_getPos(self):
         """
         Reads the current motor position of the currently selected Mercury™ controller.
         The reading process does not interrupt running compound commands.
@@ -168,15 +263,15 @@
         int:    Current motor position in counts/steps or error code.
                 The error code is derived from maximum integer value minus the error number:
                 2,147,483,647 (maxint) : Wrong Content
                 2,147,483,646 (maxint-1) : Error in _getString
                 2,147,483,645 (maxint-2) : Error in _sendString
                 2,147,483,644 (maxint-3) : Error during conversion
         """
-        res = self._dll.MMC_getPos()
+        res = self.lib.MMC_getPos()
         return res
 
     def MDC_getPosErr(self):
         """
         Reads the current motor-position error of the currently selected Mercury™ controller.
         Returns
         -------
@@ -184,15 +279,15 @@
                 The error code is derived from maximum integer value minus the error number:
                 2,147,483,647 (maxint) : Wrong Content
                 2,147,483,646 (maxint-1) : Error in _getString
                 2,147,483,645 (maxint-2) : Error in _sendString
                 2,147,483,644 (maxint-3) : Error during conversion
         """
 
-        res = self._dll.MDC_getPosErr()
+        res = self.lib.MDC_getPosErr()
         return res
 
     def MMC_getVal(self, command_ID: int):
         """
         Reads the value of the requested parameter.
         The function can be called on the fly. Running compound commands or macros are not interrupted.
         Parameters
@@ -213,15 +308,15 @@
         int: The requested value or error code is returned as 32-bit integer.
                 Error codes:
                 2,147,483,647 (MaxInt) = content error
                 2,147,483,646 (MaxInt-1) = getString error
                 2,147,483,645 (MaxInt-2) = sendString error
                 2,147,483,644 (MaxInt-3) = conversion error
         """
-        res = self._dll.MMC_getVal(command_ID)
+        res = self.lib.MMC_getVal(command_ID)
         return res
 
     def MMC_initNetwork(self, maxAxis: int=16):
         """
         Searches all addresses, starting at address maxAxis down to 1 for Mercury™ devices connected.
         If a Mercury™ device (can be C-862, C-863, C-663 or C-170) is found, it is registered so as to allow access through the MMC_select() function.
         The function MMC_initNetwork is optional. If it is not used, devices can be activated anyway using the MMC_setDevice function.
@@ -233,21 +328,21 @@
                         The range of maxAxis is 1 to 16
                         Because scanning each address takes about 0.5 seconds, it saves time to not start at device numbers higher than required.
         Returns
         -------
         list: list of integers corresponding to the connected devices
         """
         devices = []
-        res = self._dll.MMC_initNetwork(maxAxis)
+        res = self.lib.MMC_initNetwork(maxAxis)
         if res < 0:
             raise IOError('wrong return from dll')
         if res > 0:
-            bits = Bits(int=res, length=32).bin
-            for ind in range(maxAxis):
-                if bits[-1-ind] == '1':
+            bits = bitarray(res)
+            for ind in range(len(bits)):
+                if bits[-1-ind] == 1:
                     devices.append(ind+1)
         return devices
 
     def MMC_moveA(self, axis: int=0, position: int=0):
         """
         Moves the motor of the specified axis (device number) to specified position.
         Parameters
@@ -261,15 +356,15 @@
         -------
         int:    Error codes:
                     0: No error
                     1: Error, wrong axis
                     2: Error, not connected
                     3: Error, sendString
         """
-        res = self._dll.MMC_moveA(axis, position)
+        res = self.lib.MMC_moveA(axis, position)
         return res
 
     def MMC_moveR(self, axis: int=0, shift: int=0):
         """
         Moves the motor of the specified axis (device number) relative to its current position by shift counts or steps.
         Parameters
         ----------
@@ -281,30 +376,30 @@
         -------
         int:    Error codes:
                     0: No error
                     1: Error, wrong axis
                     2: Error, not connected
                     3: Error, sendString
         """
-        res = self._dll.MMC_moveR(axis, shift)
+        res = self.lib.MMC_moveR(axis, shift)
         return res
 
         
         
     def MDC_moving(self):
         """
         Returns the motion status of the currently selected C-862 or C-863 Mercury™ DC motor controller.
         For C-663 Mercury™-Step controllers, an equivalent function is available.
         Returns
         -------
         bool: moving status
                     0: Not moving
                     1: moving
         """
-        res = self._dll.MDC_moving()
+        res = self.lib.MDC_moving()
         if res < 0:
             raise IOError('wrong return from dll')
         else:
             return bool(res)
 
     def MST_moving(self):
         """
@@ -312,15 +407,15 @@
         For Mercury™ DC motor controllers, an equivalent function is available.
         Returns
         -------
         bool: moving status
                     0: Not moving
                     1: moving
         """
-        res = self._dll.MST_moving()
+        res = self.lib.MST_moving()
         if res < 0:
             raise IOError('wrong return from dll')
         else:
             return bool(res)
     
     def MMC_setDevice(self, axis: int=0):
         """
@@ -331,66 +426,80 @@
         MMC_select()
         Parameters
         ----------
         axis: (int) Range 1 to 16,
                 Device number of the controller that shall be selected for communication.
                 The device number or address can be set by the controller's front panel DIP switches.
         """
-        res = self._dll.MMC_setDevice(axis)
+        res = self.lib.MMC_setDevice(axis)
         if res ==1:
             raise IOError('Wrong axis number')
 
     def MMC_select(self, axis: int=0):
         """
         Selects the specified axis (device) to enable communication with it.
         Unlike the MMC_setDevice function, here the registration status is checked, so this function requires that the
         MMC_initNetwork function have been called previously at the beginning of the program.
         Parameters
         ----------
         axis: (int) range 1 to 16 Device number of the controller that is to be selected for communication.
         """
-        res = self._dll.MMC_select(axis)
+        res = self.lib.MMC_select(axis)
         if res == 1:
             raise IOError('Wrong axis number')
         elif res == 2:
             raise IOError('axis not registered')
 
     def MMC_sendCommand(self,cmd):
         c_cmd = create_string_buffer(cmd.encode())
-        res = self._dll.MMC_sendCommand(byref(c_cmd))
+        res = self.lib.MMC_sendCommand(byref(c_cmd))
         if res == 114:
             raise IOError('Write error')
         elif res == 116:
             raise IOError('Length Error')
 
 
     def MDC_waitStop(self):
         """
         For C-862 Mercury™ (DC motor) C-863 Mercury™ (DC motor)
         Waits until the current move has terminated or interrupted by user command (function MCC_GlobalBreak).
         """
-        res = self._dll.MDC_waitStop()
+        res = self.lib.MDC_waitStop()
         if res == 1:
             raise IOError('Error, query')
         elif res == 2:
             raise IOError('User break')
 
     def MST_waitStop(self):
         """
         For C-663 Mercury™-Step
         Waits until the current move has terminated or interrupted by user command (function MCC_GlobalBreak).
         """
-        res = self._dll.MST_waitStop()
+        res = self.lib.MST_waitStop()
         if res == 1:
             raise IOError('Error, query')
         elif res == 2:
             raise IOError('User break')
 
     def MMC_globalBreak(self):
         """
         This function interrupts pending operations waiting for termination of a move. Can be used with _moving()
         or _waitStop functions.
 
         """
-        res = self._dll.MMC_globalBreak()
+        res = self.lib.MMC_globalBreak()
         if res != 0:
             raise IOError('wrong return from dll')
+
+
+if __name__ == '__main__':
+    mmc = MMC_Wrapper(com_port='COM13')
+    try:
+        mmc.open()
+        devices = mmc.MMC_initNetwork(3)
+        mmc.MMC_select(devices[0])
+        print(mmc.getPos())
+    except Exception as e:
+        print(e)
+        pass
+    finally:
+        mmc.close()
```

### Comparing `pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente/resources/config_template.toml` & `pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente/resources/config_template.toml`

 * *Files 9% similar despite different names*

```diff
@@ -13,8 +13,11 @@
 #    'C880_DLL': ['C-880', ],
 #    'E816_DLL': ['E-621', 'E-625', 'E-665', 'E-816', 'E816', ],
 #    'E516_DLL': ['E-516', ],
 #    'PI_Mercury_GCS_DLL': ['C-663.10', 'C-863.10', 'MERCURY', 'MERCURY_GCS1', ],
 #    'PI_HydraPollux_GCS2_DLL': ['HYDRA', 'POLLUX', 'POLLUX2', 'POLLUXNT', ],
 #    'E7XX_GCS_DLL': ['DIGITAL PIEZO CONTROLLER', 'E-710', 'E-761', ],
 #    'HEX_GCS_DLL': ['HEXAPOD', 'HEXAPOD_GCS1', ],
-#    'PI_G_GCS2_DLL': ['UNKNOWN', ],
+#    'PI_G_GCS2_DLL': ['UNKNOWN', ],
+
+[mmc]
+com_port = 'COM13'
```

### Comparing `pymodaq_plugins_physik_instrumente-1.1.1/src/pymodaq_plugins_physik_instrumente.egg-info/SOURCES.txt` & `pymodaq_plugins_physik_instrumente-1.2.0/src/pymodaq_plugins_physik_instrumente.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,34 @@
 src/pymodaq_plugins_physik_instrumente.egg-info/SOURCES.txt
 src/pymodaq_plugins_physik_instrumente.egg-info/dependency_links.txt
 src/pymodaq_plugins_physik_instrumente.egg-info/entry_points.txt
 src/pymodaq_plugins_physik_instrumente.egg-info/requires.txt
 src/pymodaq_plugins_physik_instrumente.egg-info/top_level.txt
 src/pymodaq_plugins_physik_instrumente/daq_move_plugins/__init__.py
 src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI.py
+src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PILegacy.py
 src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI_E870.py
 src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI_MMC.py
+src/pymodaq_plugins_physik_instrumente/daq_move_plugins/daq_move_PI_MMCLegacy.py
 src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/__init__.py
 src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_0D/__init__.py
 src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_1D/__init__.py
 src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_2D/__init__.py
 src/pymodaq_plugins_physik_instrumente/daq_viewer_plugins/plugins_ND/__init__.py
 src/pymodaq_plugins_physik_instrumente/hardware/__init__.py
+src/pymodaq_plugins_physik_instrumente/hardware/pi_wrapper.py
 src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.H
 src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC.dll
 src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.H
 src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.c
 src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC413.lib
 src/pymodaq_plugins_physik_instrumente/hardware/PI/MMC_418.dll
 src/pymodaq_plugins_physik_instrumente/hardware/PI/MercuryNativeCommands_MS176E101.pdf
 src/pymodaq_plugins_physik_instrumente/hardware/PI/Mercury_DLL-LV_MS177E500.pdf
 src/pymodaq_plugins_physik_instrumente/hardware/PI/__init__.py
+src/pymodaq_plugins_physik_instrumente/hardware/PI/base.py
 src/pymodaq_plugins_physik_instrumente/hardware/PI/mmc_wrapper.py
+src/pymodaq_plugins_physik_instrumente/hardware/PI/mmc_wrapper_client64.py
 src/pymodaq_plugins_physik_instrumente/resources/VERSION
 src/pymodaq_plugins_physik_instrumente/resources/__init__.py
 src/pymodaq_plugins_physik_instrumente/resources/config_template.toml
 tests/test_plugin_package_structure.py
```

### Comparing `pymodaq_plugins_physik_instrumente-1.1.1/tests/test_plugin_package_structure.py` & `pymodaq_plugins_physik_instrumente-1.2.0/tests/test_plugin_package_structure.py`

 * *Files identical despite different names*


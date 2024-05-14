# Comparing `tmp/arrakis_nd-2.0.0.tar.gz` & `tmp/arrakis_nd-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrakis_nd-2.0.0.tar", last modified: Sun Mar 10 17:06:12 2024, max compression
+gzip compressed data, was "arrakis_nd-2.0.1.tar", last modified: Tue May 14 18:40:41 2024, max compression
```

## Comparing `arrakis_nd-2.0.0.tar` & `arrakis_nd-2.0.1.tar`

### file list

```diff
@@ -1,44 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 17:06:12.401951 arrakis_nd-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-03-10 17:06:12.401951 arrakis_nd-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 17:06:12.397951 arrakis_nd-2.0.0/arrakis_nd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 17:06:12.397951 arrakis_nd-2.0.0/arrakis_nd/arrakis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/arrakis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53668 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/arrakis/arrakis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/arrakis/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 17:06:12.397951 arrakis_nd-2.0.0/arrakis_nd/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/dataset/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 17:06:12.401951 arrakis_nd-2.0.0/arrakis_nd/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/plugins/daughter_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/plugins/empty_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/plugins/muon_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/plugins/trackid_hit_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 17:06:12.401951 arrakis_nd-2.0.0/arrakis_nd/programs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/programs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/programs/create_arrakis_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/programs/plugin_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/programs/run_arrakis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 17:06:12.401951 arrakis_nd-2.0.0/arrakis_nd/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/utils/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 17:06:12.401951 arrakis_nd-2.0.0/arrakis_nd/utils/display/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/utils/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/utils/display/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/arrakis_nd/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 17:06:12.401951 arrakis_nd-2.0.0/arrakis_nd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-03-10 17:06:12.000000 arrakis_nd-2.0.0/arrakis_nd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-10 17:06:12.000000 arrakis_nd-2.0.0/arrakis_nd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 17:06:12.000000 arrakis_nd-2.0.0/arrakis_nd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-10 17:06:12.000000 arrakis_nd-2.0.0/arrakis_nd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-10 17:06:12.000000 arrakis_nd-2.0.0/arrakis_nd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-10 17:06:12.000000 arrakis_nd-2.0.0/arrakis_nd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-10 17:06:12.401951 arrakis_nd-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-10 17:06:04.000000 arrakis_nd-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.483418 arrakis_nd-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-14 18:40:41.483418 arrakis_nd-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.471418 arrakis_nd-2.0.1/arrakis_nd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.475418 arrakis_nd-2.0.1/arrakis_nd/arrakis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/arrakis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62970 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/arrakis/arrakis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11118 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/arrakis/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.475418 arrakis_nd-2.0.1/arrakis_nd/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/dataset/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.479418 arrakis_nd-2.0.1/arrakis_nd/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/ancestor_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/blip_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/constraint_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/daughter_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14905 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/delta_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/empty_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19905 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/fragment_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/interaction_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/ion_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/michel_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/neutrino_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/neutron_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/parent_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/particle_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12525 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/photon_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/proton_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/segment_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/shower_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/track_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/trackid_hit_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.479418 arrakis_nd-2.0.1/arrakis_nd/programs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/programs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/programs/create_arrakis_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/programs/plugin_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/programs/run_arrakis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/programs/run_arrakis_display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.479418 arrakis_nd-2.0.1/arrakis_nd/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.483418 arrakis_nd-2.0.1/arrakis_nd/utils/display/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23538 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/display/arrakis_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14014 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/display/charge_light_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/display/marjolein_2x2_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/display/set_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19024 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/display/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/display/vis_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/shower_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/track_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.483418 arrakis_nd-2.0.1/arrakis_nd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-14 18:40:41.000000 arrakis_nd-2.0.1/arrakis_nd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-14 18:40:41.000000 arrakis_nd-2.0.1/arrakis_nd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:40:41.000000 arrakis_nd-2.0.1/arrakis_nd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 18:40:41.000000 arrakis_nd-2.0.1/arrakis_nd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-14 18:40:41.000000 arrakis_nd-2.0.1/arrakis_nd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 18:40:41.000000 arrakis_nd-2.0.1/arrakis_nd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 18:40:41.483418 arrakis_nd-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/setup.py
```

### Comparing `arrakis_nd-2.0.0/LICENSE` & `arrakis_nd-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.0/PKG-INFO` & `arrakis_nd-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrakis_nd
-Version: 2.0.0
+Version: 2.0.1
 Summary: Arrakis module for near detector data.
 Home-page: https://github.com/Neutron-Calibration-in-DUNE/ArrakisND
 Author: Nicholas Carrara, Marjolein van Nuland, Luis Lepin
 Author-email: ncarrara.physics@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -25,14 +25,16 @@
 Requires-Dist: charset-normalizer
 Requires-Dist: colorama
 Requires-Dist: colorcet==3.1.0
 Requires-Dist: comm
 Requires-Dist: contourpy
 Requires-Dist: cryptography==42.0.5
 Requires-Dist: cycler
+Requires-Dist: dash
+Requires-Dist: dash-bootstrap-components
 Requires-Dist: debugpy
 Requires-Dist: decorator
 Requires-Dist: docutils==0.20.1
 Requires-Dist: exceptiongroup
 Requires-Dist: executing
 Requires-Dist: fonttools
 Requires-Dist: h5py
```

### Comparing `arrakis_nd-2.0.0/README.md` & `arrakis_nd-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.0/arrakis_nd/arrakis/arrakis.py` & `arrakis_nd-2.0.1/arrakis_nd/arrakis/arrakis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,53 @@
 """
 """
 from mpi4py import MPI
 import h5py
 import os
 import importlib.util
-import traceback
 import sys
 import inspect
 import glob
 from tqdm import tqdm
 import torch
 import numpy as np
 from datetime import datetime
+import traceback
 from matplotlib import pyplot as plt
 from importlib.metadata import version
 
 from arrakis_nd.utils.logger import Logger
 from arrakis_nd.utils.utils import (
     profiler,
     timing_manager,
     memory_manager
 )
+from arrakis_nd.arrakis.common import (
+    tracklette_data_type,
+    track_data_type,
+    fragment_data_type,
+    shower_data_type,
+    blip_data_type,
+    particle_data_type,
+    interaction_data_type,
+    neutrino_data_type,
+    interaction_event_data_type,
+    neutrino_event_data_type,
+    nar_inelastic_data_type,
+    undefined_data_type,
+    output_error_data_type
+)
 from arrakis_nd.plugins.plugin import Plugin
 
 
 class Arrakis:
     """
     Main Arrakis class for running jobs. Arrakis is designed
     to work with MPI and H5.  The user must run Arrakis using mpirun
     with at least two processes (one master and N-1 workers).
-    
-    
     """
     @profiler
     def __init__(
         self,
         config: dict = {},
         meta:   dict = {},
     ):
@@ -47,82 +60,131 @@
         """
 
         """Get mpi communication parameters"""
         try:
             self.comm = MPI.COMM_WORLD
             self.rank = self.comm.Get_rank()
             self.size = self.comm.Get_size()
-        except Exception as e:
-            raise RuntimeError(f"unable to obtain MPI parameters: {e}")
+        except Exception as exception:
+            raise RuntimeError(f"unable to obtain MPI parameters: {exception}")
 
         """Set input parameters and set up loggers"""
         try:
             if self.rank == 0:
-                self.logger = Logger(f"master: {self.rank}", output="both")
+                self.logger = Logger(f"master: {self.rank}")
             else:
-                self.logger = Logger(f"worker: {self.rank}", output="both")
-        except Exception as e:
-            raise RuntimeError(f"unable to set up logging system: {e}")
+                self.logger = Logger(f"worker: {self.rank}")
+        except Exception as exception:
+            raise RuntimeError(f"unable to set up logging system: {exception}")
 
         self.config = config
         self.meta = meta
 
         """Setting error status for this node"""
         self.error_status = None
+        self.exc_type = None
+        self.exc_value = None
+        self.exc_traceback = None
+        self.line_number = None
+        self.file_name = None
+        self.tb_str = None
+        self.traceback_details = None
+        self.event_errors = []
+        self.plugin_errors = []
+        self.event_plugin_errors = []
+        self.event_plugin_exc_types = []
+        self.event_plugin_exc_values = []
+        self.event_plugin_exc_tracebacks = []
+        self.event_plugin_line_numbers = []
+        self.event_plugin_file_names = []
+        self.event_plugin_tb_strs = []
+        self.event_plugin_traceback_details = []
 
         """Parse config"""
         try:
             self.parse_config()
-        except Exception as e:
-            self.error_status = e
+        except Exception as exception:
+            self.report_error(exception=exception)
         self.barrier()
 
         """Construct plugins"""
         self.plugins = {}
         try:
             self.construct_plugins()
-        except Exception as e:
-            self.error_status = e
+        except Exception as exception:
+            self.report_error(exception=exception)
         self.barrier()
 
         self.flow_files = []
         """Distributed events and indices for various arrays"""
         self.distributed_events = {}
         self.distributed_interactions_indices = {}
         self.distributed_segments_indices = {}
         self.distributed_stack_indices = {}
         self.distributed_trajectories_indices = {}
         self.distributed_charge_indices = {}
         self.distributed_light_indices = {}
 
     @profiler
+    def clear_indices(self):
+        self.distributed_events.clear()
+        self.distributed_interactions_indices.clear()
+        self.distributed_segments_indices.clear()
+        self.distributed_stack_indices.clear()
+        self.distributed_trajectories_indices.clear()
+        self.distributed_charge_indices.clear()
+        self.distributed_light_indices.clear()
+
+    @profiler
+    def report_error(
+        self,
+        exception: Exception = None
+    ):
+        self.error_status = exception
+        self.exc_type, self.exc_value, self.exc_traceback = sys.exc_info()
+        # Extracting the line number from the traceback
+        self.line_number = self.exc_traceback.tb_lineno
+        self.file_name = self.exc_traceback.tb_frame.f_code.co_filename
+        # Optionally, use traceback to format a string of the entire traceback
+        self.tb_str = traceback.format_exception(self.exc_type, self.exc_value, self.exc_traceback)
+        self.traceback_details = "".join(self.tb_str)
+
+    @profiler
     def barrier(self):
         errors = self.comm.allgather(self.error_status)
+        exc_types = self.comm.allgather(self.exc_type)
+        line_numbers = self.comm.allgather(self.line_number)
+        file_names = self.comm.allgather(self.file_name)
         if any(errors):
             if self.rank == 0:
                 errors_count = sum(1 for error in errors if error is not None)
                 errors_indices = [index for index, error in enumerate(errors) if error is not None]
                 self.logger.critical(f"{errors_count} errors encountered in Arrakis program")
                 for index in errors_indices:
                     self.logger.critical(f"error encountered in worker {index}: ")
-                    self.logger.critical(errors[index])
+                    self.logger.critical(f"exception:   {errors[index]}")
+                    self.logger.critical(f"exc_type:    {exc_types[index]}")
+                    self.logger.critical(f"line_number:     {line_numbers[index]}")
+                    self.logger.critical(f"file_name:       {file_names[index]}")
                 self.comm.Abort(1)
         else:
             self.comm.Barrier()
 
     @profiler
     def parse_config(self):
         """
         Set up config parameters from input config file
         """
         if self.rank == 0:
             try:
                 """Startup main arrakis program"""
-                self.logger.info(f'############################ ARRAKIS  v. [{version("arrakis-nd")}] ############################')
-                
+                self.logger.info(
+                    f'############################ ARRAKIS  v. [{version("arrakis-nd")}] ############################'
+                )
+
                 """Check for main arrakis_nd parameters"""
                 if "arrakis_nd" not in self.config.keys():
                     self.logger.error("arrakis_nd section not in config!")
                 arrakis_nd_config = self.config["arrakis_nd"]
 
                 """Try to grab system info and display to the logger"""
                 system_info = self.logger.get_system_info()
@@ -185,23 +247,23 @@
                     self.logger.info("using cpu as device")
                     self.meta["device"] = torch.device("cpu")
                 self.meta["gpu"] = gpu
 
                 """Send new device meta data to workers"""
                 for ii in range(1, self.comm.size):
                     self.comm.send(self.meta, dest=ii, tag=0)
-            except Exception as e:
-                self.error_status = e
+            except Exception as exception:
+                self.report_error(exception=exception)
             self.barrier()
         else:
             self.barrier()
             try:
                 self.meta = self.comm.recv(source=0, tag=0)
-            except Exception as e:
-                self.error_status = e
+            except Exception as exception:
+                self.report_error(exception=exception)
 
     @profiler
     def construct_plugins(self):
         """
         Construct all plugin objects.  First, we look for all associated
         classes which inherit from plugins.  These include both the standard
         plugins which are merged into the plugins/ folder, as well as
@@ -219,16 +281,16 @@
 
         """Iterate over specified plugins and check that they exist"""
         for plugin, config in plugins_config.items():
             if plugin not in self.available_plugins.keys():
                 self.logger.error(f'specified plugin "{plugin}" not available!')
             try:
                 self.plugins[plugin] = self.available_plugins[plugin](config)
-            except Exception as e:
-                self.logger.error(f'failed to construct plugin {plugin} with config {config}: {e}')
+            except Exception as exception:
+                self.logger.error(f'failed to construct plugin {plugin} with config {config}: {exception}')
 
         """Check that intermediate products are set up correctly"""
         running_output_products = []
         for ii, plugin_name in enumerate(self.plugins.keys()):
             if ii == 0:
                 if self.plugins[plugin_name].input_products is not None:
                     self.logger.error(
@@ -253,15 +315,25 @@
                         for input_product in self.plugins[plugin_name].input_products:
                             if input_product not in running_output_products:
                                 self.logger.error(
                                     f'specified plugin "{plugin_name}" at location "{ii}" expects input_products \
                                     "{self.plugins[plugin_name].input_products}" but current products only contain \
                                     {running_output_products}!'
                                 )
-            running_output_products.append(self.plugins[plugin_name].output_product)
+            if isinstance(self.plugins[plugin_name].output_products, str):
+                running_output_products.append(self.plugins[plugin_name].output_products)
+            elif isinstance(self.plugins[plugin_name].output_products, list):
+                running_output_products += self.plugins[plugin_name].output_products
+            else:
+                if self.plugins[plugin_name].output_products is not None:
+                    self.logger.error(
+                        f'specified plugin "{plugin_name}" at location "{ii}" should have output_products == None, \
+                        or output_products == str, or output_products == list(str), but has type \
+                        "{type(self.plugins[plugin_name].output_products)}"!'
+                    )
 
     @profiler
     def collect_plugins(self):
         """
         This function collects all available plugins from the ArrakisND
         plugins folder, as well as any plugin locations specified in the
         config file.
@@ -289,16 +361,16 @@
                 ("__pycache__.py" in plugin_file) or
                 ("__pycache__" in plugin_file) or
                 (".py" not in plugin_file)
             ):
                 continue
             try:
                 self.load_plugin_function(plugin_file)
-            except Exception as e:
-                self.logger.warn(f'problem loading plugin from file: {plugin_file}: {e}')
+            except Exception as exception:
+                self.logger.warn(f'problem loading plugin from file: {plugin_file}: {exception}')
 
     @profiler
     def load_plugin_function(
         self,
         plugin_file: str
     ):
         """
@@ -324,46 +396,51 @@
     @profiler
     def set_up_input_files(self):
         """
         Iterate over flow_folder directory and determine
         if listed input files exist, or if "all" is selected for
         input files, construct the list of all .h5 files in the
         flow_folder.
+
+        We create the data members
+            self.flow_folder - location of the flow files specified in config
+            self.flow_files - names of all the flow files to process
+            self.arrakis_folder - location to put the arrakis files
         """
         if self.rank == 0:
             try:
                 arrakis_dict = self.config['arrakis_nd']
-                
+
                 """Check for parameters"""
                 if 'flow_folder' not in arrakis_dict.keys():
-                    self.logger.error(f'flow_folder not specified in config!')
+                    self.logger.error('flow_folder not specified in config!')
                 if 'flow_files' not in arrakis_dict.keys():
-                    self.logger.error(f'flow_files not specified in config!')
-                    
+                    self.logger.error('flow_files not specified in config!')
+
                 flow_folder = arrakis_dict['flow_folder']
                 flow_files = arrakis_dict["flow_files"]
-                
+
                 """Check for arrakis folder"""
                 if 'arrakis_folder' not in arrakis_dict.keys():
-                    self.logger.warn(f'arrakis_folder not specified in config! setting to "/local_scratch"')
+                    self.logger.warn('arrakis_folder not specified in config! setting to "/local_scratch"')
                     arrakis_dict['arrakis_folder'] = '/local_scratch'
                 arrakis_folder = arrakis_dict['arrakis_folder'].replace('flow', 'arrakis').replace('FLOW', 'ARRAKIS')
-                                
+
                 """Check that flow folder exists"""
                 if not os.path.isdir(flow_folder):
                     self.logger.error(f'specified flow_folder {flow_folder} does not exist!')
-                    
+
                 """Check that flow folder has a '/' at the end"""
                 if flow_folder[-1] != '/':
                     flow_folder += '/'
-                    
+
                 """Check that arrakis folder has a '/' at the end"""
                 if arrakis_folder[-1] != '/':
                     arrakis_folder += '/'
-                    
+
                 """Check that arrakis folder exists"""
                 if not os.path.isdir(arrakis_folder):
                     os.makedirs(arrakis_folder)
 
                 if isinstance(arrakis_dict["flow_files"], list):
                     """
                     If the flow_files parameter is a list, look through
@@ -371,15 +448,15 @@
                     in the flow_folder.
                     """
                     flow_files = [
                         input_file for input_file in arrakis_dict["flow_files"]
                         if input_file not in arrakis_dict["skip_files"]
                     ]
                     for flow_file in flow_files:
-                        if not os.path.isfile(flow_file):
+                        if not os.path.isfile(flow_folder + flow_file):
                             self.logger.error(
                                 f"specified file {flow_file} does not exist in directory {flow_folder}!"
                             )
                 elif isinstance(arrakis_dict["flow_files"], str):
                     """
                     If the flow_files parameter is a string, check if its
                     the phrase 'all', and if so, recursively grab all h5
@@ -402,15 +479,15 @@
                     else:
                         try:
                             self.logger.info(
                                 f'searching {flow_folder} recursively for all {arrakis_dict["flow_files"]} files.'
                             )
                             flow_files = [
                                 os.path.basename(input_file) for input_file in glob.glob(
-                                    f'{flow_folder}/{arrakis_dict["flow_files"]}',
+                                    f'{flow_folder}/*.{arrakis_dict["flow_files"]}',
                                     recursive=True,
                                 )
                                 if input_file not in arrakis_dict["skip_files"]
                             ]
                         except Exception as exception:
                             self.logger.error(
                                 f'specified "flow_files" parameter: {arrakis_dict["flow_files"]} incompatible!'
@@ -425,25 +502,82 @@
                 self.arrakis_folder = arrakis_folder
                 self.logger.info(f'setting arrakis_folder to {self.arrakis_folder}.')
                 for ii in range(1, self.comm.size):
                     self.comm.send(self.flow_folder, dest=ii, tag=80)
                     self.comm.send(self.flow_files, dest=ii, tag=81)
                     self.comm.send(self.arrakis_folder, dest=ii, tag=82)
                 self.logger.info(f'found {len(self.flow_files)} flow files for processing.')
-            except Exception as e:
-                self.error_status = e
+            except Exception as exception:
+                self.report_error(exception=exception)
             self.barrier()
         else:
             self.barrier()
             try:
                 self.flow_folder = self.comm.recv(source=0, tag=80)
                 self.flow_files = self.comm.recv(source=0, tag=81)
                 self.arrakis_folder = self.comm.recv(source=0, tag=82)
-            except Exception as e:
-                self.error_status = e
+            except Exception as exception:
+                self.report_error(exception=exception)
+
+    @profiler
+    def reset_event_errors(self):
+        self.event_errors = []
+        self.plugin_errors = []
+        self.event_plugin_errors = []
+        self.event_plugin_exc_types = []
+        self.event_plugin_exc_values = []
+        self.event_plugin_exc_tracebacks = []
+        self.event_plugin_line_numbers = []
+        self.event_plugin_file_names = []
+
+    @profiler
+    def report_event_errors(
+        self,
+        file_name: str
+    ):
+        """
+        Report any event/plugin errors that have occurred during
+        this file.  These errors, if there are any, are reported
+        and saved to the corresponding ARRAKIS file in the meta
+        information.
+        """
+        event_errors = np.concatenate(self.comm.allgather(self.event_errors))
+        plugin_errors = np.concatenate(self.comm.allgather(self.plugin_errors))
+        event_plugin_errors = np.concatenate(self.comm.allgather(self.event_plugin_errors))
+        event_plugin_line_numbers = np.concatenate(self.comm.allgather(self.event_plugin_line_numbers))
+        event_plugin_file_names = np.concatenate(self.comm.allgather(self.event_plugin_file_names))
+        if self.rank == 0:
+            if len(event_errors) > 0:
+                """Report event errors to log"""
+                self.logger.warn(f"event/plugin errors occurred when processing file {file_name}")
+                
+                """Display error information"""
+                for ii, event_error in enumerate(event_errors):
+                    self.logger.warn(f"event: {event_error} / plugin: {plugin_errors[ii]}")
+                    self.logger.warn(f" {' ':<{5}} exception: {event_plugin_errors[ii]}")
+                    self.logger.warn(f" {' ':<{5}} line_number: {event_plugin_line_numbers[ii]}")
+                    self.logger.warn(f" {' ':<{5}} file_name: {event_plugin_file_names[ii]}")
+                errors = np.empty(len(event_errors), dtype=output_error_data_type)
+                errors['event_id'] = event_errors.astype('i4')
+                errors['plugin_name'] = plugin_errors.astype('S50')
+                errors['plugin_error'] = event_plugin_errors.astype('S500')
+                errors['plugin_line_number'] = event_plugin_line_numbers.astype('S50')
+                errors['plugin_file_name'] = event_plugin_file_names.astype('S50')
+                
+                """Report error information to ARRAKIS file"""
+                arrakis_file_name = file_name.replace('FLOW', 'ARRAKIS').replace('flow', 'arrakis')
+                with h5py.File(self.arrakis_folder + arrakis_file_name, 'a') as arrakis_file:
+                    original_size = arrakis_file['arrakis/errors'].shape[0]
+                    additional_size = len(errors)
+                    new_size = original_size + additional_size
+                    """Insert the objects into the array"""
+                    arrakis_file['arrakis/errors'].resize((new_size,))
+                    arrakis_file['arrakis/errors'][original_size:new_size] = errors
+        else:
+            pass
 
     @profiler
     def run_begin_of_file(
         self,
         file_name: str
     ):
         """
@@ -471,303 +605,225 @@
         """
 
         """Determine the arrakis file name"""
         arrakis_file_name = file_name.replace('FLOW', 'ARRAKIS').replace('flow', 'arrakis')
 
         """Open the flow file and determine the output array shapes"""
         with h5py.File(self.flow_folder + file_name, 'r') as flow_file, \
-            h5py.File(self.arrakis_folder + arrakis_file_name, 'a') as arrakis_file:
+             h5py.File(self.arrakis_folder + arrakis_file_name, 'a') as arrakis_file:
             """
             First we make the labels for the charge dataset.  These consist of six
             main labels that we wish to generate with various plugins:
                 (1) topology - a descriptor of basic shapes
-                (2) physics_micro - a descriptor of local physics
-                (3) physics_macro - a descriptor of larger scale physics objects
+                (2) particle - the unique pdg of the particle
+                (3) physics - a descriptor of local physics
                 (4) unique_topology - unique labels for instances of topology
-                (5) unique_physics_micro - unique labels for instances of physics_micro
-                (6) unique_physics_macro - unique labels for instances of physics_macro
-                (7) vertex - binary variable denoting whether a vertex is at this hit
-                (8) tracklette_begin - binary variable denoting whether a track beginning is at this hit
-                (9) tracklette_end - binary variable denoting whether a track end is at this hit
-                (10) fragment_begin - binary variable denoting whether a fragment beginning is at this hit
-                (11) fragment_end - binary variable denoting whether a fragment end is at this hit
-                (12) shower_begin - binary variable denoting whether a shower beginning is at this hit
+                (5) vertex - binary variable denoting whether a vertex is at this hit
+                (6) tracklette_begin - binary variable denoting whether a track beginning is at this hit
+                (7) tracklette_end - binary variable denoting whether a track end is at this hit
+                (8) fragment_begin - binary variable denoting whether a fragment beginning is at this hit
+                (9) fragment_end - binary variable denoting whether a fragment end is at this hit
+                (10) shower_begin - binary variable denoting whether a shower beginning is at this hit
 
             These labels are assigned to each reconstructed charge hit and
             written in the corresponding ARRAKIS file.
             """
             charge_name = 'charge/calib_final_hits/data'
-
+            charge_segment_name = 'charge_segment/calib_final_hits/data'
+            charge_segments = flow_file['mc_truth/calib_final_hit_backtrack/data']['segment_id']
+            charge_segments_fraction = flow_file['mc_truth/calib_final_hit_backtrack/data']['fraction']
+            non_zero_charge_segments = [row[row != 0] for row in charge_segments]
+            max_length = len(max(non_zero_charge_segments, key=len))
             num_charge = len(flow_file[charge_name]['x'])
 
+            new_charge_segment_data_type = np.dtype([
+                ('event_id', 'i4'),
+                ('segment_id', 'i4', (max_length,)),
+                ('segment_fraction', 'f4', (max_length,)),
+                ('segment_distance', 'f4', (max_length,)),
+                ('segment_parent', 'i4', (max_length,)),
+                ('segment_start_process', 'i4', (max_length,)),
+                ('segment_start_subprocess', 'i4', (max_length,)),
+                ('topology', 'i4', (max_length,)),
+                ('particle', 'i4', (max_length,)),
+                ('physics', 'i4', (max_length,)),
+                ('unique_topology', 'i4', (max_length,)),
+                ('vertex', 'i4', (max_length,)),
+                ('tracklette_begin', 'i4', (max_length,)),
+                ('tracklette_end', 'i4', (max_length,)),
+                ('fragment_begin', 'i4', (max_length,)),
+                ('fragment_end', 'i4', (max_length,)),
+                ('shower_begin', 'i4', (max_length,))
+            ])
+
+            new_charge_segment_data = np.full(num_charge, -1, dtype=new_charge_segment_data_type)
+            new_charge_segment_data['segment_id'] = charge_segments[:, :max_length]
+            new_charge_segment_data['segment_fraction'] = charge_segments_fraction[:, :max_length]
+            new_charge_segment_data['segment_distance'][:, :max_length] = np.nan
+            new_charge_segment_data['vertex'][:, :max_length] = 0
+            new_charge_segment_data['tracklette_begin'][:, :max_length] = 0
+            new_charge_segment_data['tracklette_end'][:, :max_length] = 0
+            new_charge_segment_data['fragment_begin'][:, :max_length] = 0
+            new_charge_segment_data['fragment_end'][:, :max_length] = 0
+            new_charge_segment_data['shower_begin'][:, :max_length] = 0
+
+            if charge_segment_name in arrakis_file:
+                del arrakis_file[charge_segment_name]
+
+            arrakis_file.create_dataset(charge_segment_name, data=new_charge_segment_data)
+
             new_charge_data_type = np.dtype([
                 ('event_id', 'i4'),
                 ('topology', 'i4'),
-                ('physics_micro', 'i4'),
-                ('physics_macro', 'i4'),
+                ('particle', 'i4'),
+                ('physics', 'i4'),
                 ('unique_topology', 'i4'),
-                ('unique_physics_micro', 'i4'),
-                ('unique_physics_macro', 'i4'),
-                ('vertex', 'bool'),
-                ('tracklette_begin', 'bool'),
-                ('tracklette_end', 'bool'),
-                ('fragment_begin', 'bool'),
-                ('fragment_end', 'bool'),
-                ('shower_begin', 'bool')
+                ('vertex', 'i4'),
+                ('tracklette_begin', 'i4'),
+                ('tracklette_end', 'i4'),
+                ('fragment_begin', 'i4'),
+                ('fragment_end', 'i4'),
+                ('shower_begin', 'i4')
             ])
 
             new_charge_data = np.full(num_charge, -1, dtype=new_charge_data_type)
+            new_charge_data['vertex'][:] = 0
+            new_charge_data['tracklette_begin'][:] = 0
+            new_charge_data['tracklette_end'][:] = 0
+            new_charge_data['fragment_begin'][:] = 0
+            new_charge_data['fragment_end'][:] = 0
+            new_charge_data['shower_begin'][:] = 0
 
             if charge_name in arrakis_file:
                 del arrakis_file[charge_name]
 
             arrakis_file.create_dataset(charge_name, data=new_charge_data)
 
             """
             Second, we set up arrays for CAF-like reco objects which consist
             of the following types:
-                (1) tracklettes - pieces of contiguous track like objects.
-                    (a) start (x,y,z) - track start point
-                    (b) end (x,y,z) - track end point
-                    (c) dir (u_x,u_y,u_z) - estimate of track direction taken from start point
-                    (d) enddir (u_x,u_y,u_z) - estimate of track direction takend from end point
-                    (e) Evis - visible energy in voxels corresponding to this track
-                    (f) qual - reco specific quality metric
-                    (g) len_gcm2 - track length in g/cm2
-                    (h) len_cm - track length in centimeter
-                    (i) E - track energy estimate in MeV
-                    (j) truth - associated true particle in flow file (if relevant) (i.e. track_id)
-                    (k) truthOverlap - fractional overlap between this track and true particle
-                (2) tracks - collections of tracklettes which define a complete track.
-                (3) fragments - pieces of contiguous shower like objects.
-                    (a) start (x,y,z) - shower start point
-                    (b) dir (u_x,u_y,u_z) - shower direction
-                    (c) Evis - visible energy in voxels corresponding to this shower
-                    (d) qual - reco specific quality metric
-                    (e) len_gcm2 - track length in g/cm2
-                    (f) len_cm - track length in centimeter
-                    (g) E - track energy estimate in MeV
-                    (h) truth - associated true particle in flow file (if relevant) (i.e. track_id)
-                    (i) truthOverlap - fractional overlap between this shower and true particle
-                (4) showers - collections of fragments which define a complete shower.
-                (5) blips - collections of points associated to blip-like activity.
-                    (a) start (x,y,z) - start position of this blip object
-                    (b) Evis - visible energy in voxels corresponding to this blip
-                    (c) E - reconstructed energy (GeV)
-                    (d) bliphyp - hypothesis for this blip's identity
-                    (e) truth - associated true particle in flow file (if relevant) (i.e track_id)
-                    (f) truthOverlap - fractional overlap between this blip and true particle
-                (6) particles - particles within an event that are associated to tracks/showers/blips.
-                    (a) primary - is this reco particle a primary one (i.e. eminates directly from vertex)?
-                    (b) pdg - pdg code inferred for this particle
-                    (c) tgtA - atomic number of nucleus this particle was reconstructed in
-                    (d) score - PID score for this particle
-                    (e) E - reconstructed energy (GeV)
-                    (f) E_method - method used to determine energy for the particle
-                    (g) p (p_x,p_y,p_z) - reconstructed momentum for this particle
-                    (h) start (x,y,z) - reconstructed start point of this particle
-                    (i) end (x,y,z) - reconstructed end point of this particle
-                    (j) contained - contained in LAr TPC?
-                    (k) truth - associated true particle in flow file (if relevant) (i.e. track_id)
-                    (l) truthOverlap - fractional overlap between this reco particle and true particle
-                (7) interactions - collections of tracks/showers/blips which define interactions of interest.
-                    (a) vtx (x,y,z) - reconstructed vertex location
-                    (b) dir (u_x,u_y,u_z) - hypothesis for this interaction's parent particle direction
-                        (b.i) lngtrk - direction using longest track
-                        (b.ii) heshw - direction using highest energy shower
-                    (c) nuhyp - hypothesis for this interaction's neutrino identity
-                        (c.i) isnubar
-                        (c.ii) nue
-                        (c.iii) numu
-                        (c.iv) nutau
-                        (c.v) nc
-                        (c.vi) protons0
-                        (c.vii) protons1
-                        (c.viii) protons2
-                        (c.ix) protonsN
-                        (c.x) chgpi0
-                        (c.xi) chgpi1
-                        (c.xii) chgpi2
-                        (c.xiii) chgpiN
-                        (c.xiv) pizero0
-                        (c.xv) pizero1
-                        (c.xvi) pizero2
-                        (c.xvii) pizeroN
-                        (c.xviii) neutron0
-                        (c.xix) neutron1
-                        (c.xx) neutron2
-                        (c.xxi) neutronN
-                    (d) Enu - hypothesis for this interaction's neutrino energy
-                    (e) part - collections of reconstructed particles
-                    (f) truth - indicies of true_interactions in flow file (if relevant)
-                    (g) truthOverlap - fractional overlap between this reco interaction and each true interaction
             """
 
             """Construct track data types"""
             tracklette_name = 'standard_record/tracklette'
             track_name = 'standard_record/track'
-            tracklette_data_type = np.dtype([
-                ('event_id', 'i4'),
-                ('tracklette_id', 'i4'),
-                ('start', 'f4', (1, 3)),
-                ('end', 'f4', (1, 3)),
-                ('dir', 'f4', (1, 3)),
-                ('enddir', 'f4', (1, 3)),
-                ('Evis', 'f4'),
-                ('qual', 'f4'),
-                ('len_gcm2', 'f4'),
-                ('len_cm', 'f4'),
-                ('E', 'f4'),
-                ('truth', 'i4', (1, 20)),
-                ('truthOverlap', 'f4', (1, 20)),
-            ])
-            track_data_type = np.dtype([
-                ('event_id', 'i4'),
-                ('track_id', 'i4'),
-                ('tracklette_ids', 'i4', (1, 20)),
-                ('start', 'f4', (1, 3)),
-                ('end', 'f4', (1, 3)),
-                ('dir', 'f4', (1, 3)),
-                ('enddir', 'f4', (1, 3)),
-                ('Evis', 'f4'),
-                ('qual', 'f4'),
-                ('len_gcm2', 'f4'),
-                ('len_cm', 'f4'),
-                ('E', 'f4'),
-                ('truth', 'i4', (1, 20)),
-                ('truthOverlap', 'f4', (1, 20)),
-            ])
             if tracklette_name in arrakis_file:
                 del arrakis_file[tracklette_name]
             if track_name in arrakis_file:
                 del arrakis_file[track_name]
 
             arrakis_file.create_dataset(tracklette_name, shape=(0,), maxshape=(None,), dtype=tracklette_data_type)
             arrakis_file.create_dataset(track_name, shape=(0,), maxshape=(None,), dtype=track_data_type)
 
             """Construct shower data types"""
             fragment_name = 'standard_record/fragment'
             shower_name = 'standard_record/shower'
-            fragment_data_type = np.dtype([
-                ('event_id', 'i4'),
-                ('fragment_id', 'i4'),
-                ('start', 'f4', (1, 3)),
-                ('dir', 'f4', (1, 3)),
-                ('Evis', 'f4'),
-                ('qual', 'f4'),
-                ('len_gcm2', 'f4'),
-                ('len_cm', 'f4'),
-                ('E', 'f4'),
-                ('truth', 'i4', (1, 20)),
-                ('truthOverlap', 'f4', (1, 20)),
-            ])
-            shower_data_type = np.dtype([
-                ('event_id', 'i4'),
-                ('shower_id', 'i4'),
-                ('fragment_ids', 'i4', (1, 20)),
-                ('start', 'f4', (1, 3)),
-                ('dir', 'f4', (1, 3)),
-                ('Evis', 'f4'),
-                ('qual', 'f4'),
-                ('len_gcm2', 'f4'),
-                ('len_cm', 'f4'),
-                ('E', 'f4'),
-                ('truth', 'i4', (1, 20)),
-                ('truthOverlap', 'f4', (1, 20)),
-            ])
             if fragment_name in arrakis_file:
                 del arrakis_file[fragment_name]
             if shower_name in arrakis_file:
                 del arrakis_file[shower_name]
 
             arrakis_file.create_dataset(fragment_name, shape=(0,), maxshape=(None,), dtype=fragment_data_type)
             arrakis_file.create_dataset(shower_name, shape=(0,), maxshape=(None,), dtype=shower_data_type)
 
             """Construct blip data types"""
             blip_name = 'standard_record/blip'
-            blip_data_type = np.dtype([
-                ('event_id', 'i4'),
-                ('blip_id', 'i4'),
-                ('start', 'f4', (1, 3)),
-                ('Evis', 'f4'),
-                ('E', 'f4'),
-                ('bliphyp', 'i4'),
-                ('truth', 'i4', (1, 20)),
-                ('truthOverlap', 'f4', (1, 20)),
-            ])
             if blip_name in arrakis_file:
                 del arrakis_file[blip_name]
 
             arrakis_file.create_dataset(blip_name, shape=(0,), maxshape=(None,), dtype=blip_data_type)
 
             """Construct particle data types"""
             particle_name = 'standard_record/particle'
-            particle_data_type = np.dtype([
-                ('event_id', 'i4'),
-                ('particle_id', 'i4'),
-                ('primary', 'bool'),
-                ('pdg', 'i4'),
-                ('tgtA', 'i4'),
-                ('score', 'f4'),
-                ('E', 'f4'),
-                ('E_method', 'i4'),
-                ('p', 'f4', (1, 3)),
-                ('start', 'f4', (1, 3)),
-                ('end', 'f4', (1, 3)),
-                ('contained', 'bool'),
-                ('truth', 'i4', (1, 20)),
-                ('truthOverlap', 'f4', (1, 20)),
-            ])
             if particle_name in arrakis_file:
                 del arrakis_file[particle_name]
 
             arrakis_file.create_dataset(particle_name, shape=(0,), maxshape=(None,), dtype=particle_data_type)
 
             """Construct interaction data types"""
             interaction_name = 'standard_record/interaction'
-            interaction_data_type = np.dtype([
-                ('event_id', 'i4'),
-                ('interaction_id', 'i4'),
-                ('vtx', 'f4', (1, 3)),
-                ('dir_lngtrk', 'f4', (1, 3)),
-                ('dir_heshw', 'f4', (1, 3)),
-                ('nuhyp', 'f4', (1, 20)),
-                ('Enu', 'f4'),
-                ('E_method', 'i4'),
-                ('part', 'i4', (1, 20)),
-                ('truth', 'i4', (1, 20)),
-                ('truthOverlap', 'f4', (1, 20)),
-            ])
             if interaction_name in arrakis_file:
                 del arrakis_file[interaction_name]
 
             arrakis_file.create_dataset(interaction_name, shape=(0,), maxshape=(None,), dtype=interaction_data_type)
 
+            """Construct neutrino data types"""
+            neutrino_name = 'standard_record/neutrino'
+            if neutrino_name in arrakis_file:
+                del arrakis_file[neutrino_name]
+
+            arrakis_file.create_dataset(neutrino_name, shape=(0,), maxshape=(None,), dtype=neutrino_data_type)
+
+            """Construct interaction event label types"""
+            interaction_event_name = 'standard_record/interaction_event'
+            if interaction_event_name in arrakis_file:
+                del arrakis_file[interaction_event_name]
+
+            arrakis_file.create_dataset(
+                interaction_event_name, shape=(0,), maxshape=(None,), dtype=interaction_event_data_type
+            )
+
+            """Construct neutrino event label types"""
+            neutrino_event_name = 'standard_record/neutrino_event'
+            if neutrino_event_name in arrakis_file:
+                del arrakis_file[neutrino_event_name]
+
+            arrakis_file.create_dataset(neutrino_event_name, shape=(0,), maxshape=(None,), dtype=neutrino_event_data_type)
+
+            """Construct output error data types"""
+            output_error_name = 'arrakis/errors'
+            if output_error_name in arrakis_file:
+                del arrakis_file[output_error_name]
+
+            arrakis_file.create_dataset(output_error_name, shape=(0,), maxshape=(None,), dtype=output_error_data_type)
+
+            """Construct n-Ar inelastic data types"""
+            nar_inelastic_name = 'standard_record/nar_inelastic'
+            if nar_inelastic_name in arrakis_file:
+                del arrakis_file[nar_inelastic_name]
+
+            arrakis_file.create_dataset(nar_inelastic_name, shape=(0,), maxshape=(None,), dtype=nar_inelastic_data_type)
+            
+            """Construct undefined objects"""
+            undefined_name = 'standard_record/undefined'
+            if undefined_name in arrakis_file:
+                del arrakis_file[undefined_name]
+            
+            arrakis_file.create_dataset(undefined_name, shape=(0,), maxshape=(None,), dtype=undefined_data_type)
+
     @profiler
     def distribute_tasks(
         self,
         file_name: str
     ):
         """
         Determine the indices which correspond to unique
         events in the FLOW output files and distribute
         those indices among the workers.
 
+        The slowest part of this code is backtracking through hits->segments,
+        which must be done in order to create the reverse map from segments->hits.
+        This must be done since there is no way to determine what hits go
+        with what events with only the calib_final_hits data alone.
+
         Args:
             file_name (_str_): _description_
         """
         with h5py.File(self.flow_folder + file_name, 'r', driver='mpio', comm=self.comm) as file:
             if self.rank == 0:
                 """Collect event ids from mc_truth and charge/light data"""
                 interactions_events = file['mc_truth/interactions/data']['event_id']
                 segments_events = file['mc_truth/segments/data']['event_id']
                 stack_events = file['mc_truth/stack/data']['event_id']
                 trajectories_events = file['mc_truth/trajectories/data']['event_id']
-                charge_segments = file['mc_truth/calib_final_hit_backtrack/data']['segment_id']
-                non_zero_charge_segments = [row[row != 0] for row in charge_segments]
+                charge_segments = file['mc_truth/calib_final_hit_backtrack/data']['segment_id'].astype(int)
+                charge_fraction = file['mc_truth/calib_final_hit_backtrack/data']['fraction']
+                charge_fraction_mask = (charge_fraction == 0)
+                charge_segments[charge_fraction_mask] = -1
+                non_zero_charge_segments = [row[row != 0] for row in charge_fraction]
                 max_length = len(max(non_zero_charge_segments, key=len))
                 segments_ids = file['mc_truth/segments/data']['segment_id']
 
                 """Determine unique events and distribute among workers"""
                 unique_events = np.unique(trajectories_events)
                 self.num_events = len(unique_events)
                 self.distributed_events.clear()
@@ -783,37 +839,38 @@
                 self.distributed_segments_indices = {i: [] for i in range(1, self.size)}
                 self.distributed_stack_indices = {i: [] for i in range(1, self.size)}
                 self.distributed_trajectories_indices = {i: [] for i in range(1, self.size)}
                 self.distributed_charge_indices = {i: [] for i in range(1, self.size)}
                 self.distributed_light_indices = {i: [] for i in range(1, self.size)}
 
                 """Determine indices for mc_truth and charge/light data"""
-                for i, event_id in enumerate(unique_events):
-                    worker_rank = 1 + i % (self.size - 1)  # Distribute round-robin among wor
+                for ii, event_id in enumerate(unique_events):
+                    worker_rank = 1 + ii % (self.size - 1)  # Distribute round-robin among wor
                     self.distributed_events[worker_rank].append(event_id)
                     self.distributed_interactions_indices[worker_rank].append(
                         np.where(interactions_events == event_id)[0]
                     )
                     self.distributed_segments_indices[worker_rank].append(
                         np.where(segments_events == event_id)[0]
                     )
                     self.distributed_stack_indices[worker_rank].append(
                         np.where(stack_events == event_id)[0]
                     )
                     self.distributed_trajectories_indices[worker_rank].append(
                         np.where(trajectories_events == event_id)[0]
                     )
                     """For charge data we must backtrack through segments"""
+                    hits_to_segments = np.any(
+                        np.isin(
+                            charge_segments[:, :max_length], segments_ids[(segments_events == event_id)]
+                        ),
+                        axis=1,
+                    )
                     self.distributed_charge_indices[worker_rank].append(
-                        np.any(
-                            np.isin(
-                                charge_segments[:, :max_length], segments_ids[(segments_events == event_id)]
-                            ),
-                            axis=1,
-                        )
+                        hits_to_segments
                     )
                     """Likewise for light data, we must backtrack through segments"""
                     self.distributed_light_indices[worker_rank].append([])
 
                 """Distribute indices for events among workers"""
                 for ii in range(1, self.comm.size):
                     self.comm.send(self.distributed_events[ii], dest=ii, tag=2)
@@ -843,15 +900,30 @@
         which occurs before any of the workers.  Any work done
         here should be by plugins which create data that is
         needed by the other plugins.
 
         Args:
             flow_file (_h5py.File_): input flow_file
         """
-        pass
+        """Clear event indices so that file closes properly!"""
+        self.standard_record_objects = {
+            'tracklette': [],
+            'track': [],
+            'fragment': [],
+            'shower': [],
+            'blip': [],
+            'particle': [],
+            'interaction': [],
+            'neutrino': [],
+            'interaction_event': [],
+            'neutrino_event': [],
+            'nar_inelastic': [],
+            'undefined': [],
+        }
+        self.clear_indices()
 
     @profiler
     def process_events_worker(
         self,
         flow_file: h5py.File,
         arrakis_file: h5py.File,
     ):
@@ -859,34 +931,80 @@
         This function loops over all plugins and hands off the flow_file,
         arrakis_file and the associated indices for each that correspond
         to this workers event.
 
         Args:
             flow_file (_h5py.File_): input flow_file
         """
+        self.standard_record_objects = {
+            'tracklette': [],
+            'track': [],
+            'fragment': [],
+            'shower': [],
+            'blip': [],
+            'particle': [],
+            'interaction': [],
+            'neutrino': [],
+            'interaction_event': [],
+            'neutrino_event': [],
+            'nar_inelastic': [],
+            'undefined': [],
+        }
         for ii, event in enumerate(self.distributed_events[self.rank]):
             """Grab event index information"""
             event_indices = {
                 'interactions': self.distributed_interactions_indices[self.rank][ii],
                 'segments': self.distributed_segments_indices[self.rank][ii],
                 'stack': self.distributed_stack_indices[self.rank][ii],
                 'trajectories': self.distributed_trajectories_indices[self.rank][ii],
                 'charge': self.distributed_charge_indices[self.rank][ii],
                 'light': self.distributed_light_indices[self.rank][ii]
             }
-            event_products = {}
+            self.event_products = {
+                'tracklette': [],
+                'track': [],
+                'fragment': [],
+                'shower': [],
+                'blip': [],
+                'particle': [],
+                'interaction': [],
+                'neutrino': [],
+                'interaction_event': [],
+                'neutrino_event': [],
+                'nar_inelastic': [],
+                'undefined': [],
+            }
             """Iterate over plugins"""
             for plugin_name, plugin in self.plugins.items():
-                plugin.process_event(
-                    event=event,
-                    flow_file=flow_file,
-                    arrakis_file=arrakis_file,
-                    event_indices=event_indices,
-                    event_products=event_products,
-                )
+                try:
+                    plugin.process_event(
+                        event=event,
+                        flow_file=flow_file,
+                        arrakis_file=arrakis_file,
+                        event_indices=event_indices,
+                        event_products=self.event_products,
+                    )
+                except Exception as exception:
+                    self.event_errors.append(event)
+                    self.plugin_errors.append(plugin_name)
+                    self.event_plugin_errors.append(exception)
+                    exc_type, exc_value, exc_traceback = sys.exc_info()
+                    if exc_traceback.tb_next:
+                        exc_traceback = exc_traceback.tb_next
+                    if exc_traceback.tb_next:
+                        exc_traceback = exc_traceback.tb_next
+                    self.event_plugin_exc_types.append(exc_type)
+                    self.event_plugin_exc_values.append(exc_value)
+                    self.event_plugin_exc_tracebacks.append(exc_traceback)
+                    self.event_plugin_line_numbers.append(exc_traceback.tb_lineno)
+                    self.event_plugin_file_names.append(exc_traceback.tb_frame.f_code.co_filename)
+            for object in self.standard_record_objects.keys():
+                self.standard_record_objects[object] += self.event_products[object]
+        """Clear event indices so that file closes properly!"""
+        self.clear_indices()
 
     @profiler
     def run_end_of_file(
         self,
         file_name: str
     ):
         """
@@ -896,48 +1014,99 @@
         One required task is for the master node to gather up all
         reco object information and append it to the arrays in the
         ARRAKIS file.
 
         Args:
             file_name (_type_): _description_
         """
-        pass
+        standard_record_objects = self.comm.allgather(self.standard_record_objects)
+
+        if self.rank == 0:
+            """Add those standard record objects to the ARRAKIS file"""
+            arrakis_file_name = file_name.replace('FLOW', 'ARRAKIS').replace('flow', 'arrakis')
+
+            """Open the flow file and determine the output array shapes"""
+            with h5py.File(self.arrakis_folder + arrakis_file_name, 'a') as arrakis_file:
+                for object in self.standard_record_objects.keys():
+                    """Gather up all standard record objects"""
+                    objects = [
+                        standard_record_objects[ii][object]
+                        for ii in range(self.size)
+                        if len(standard_record_objects[ii][object]) != 0
+                    ]
+                    if len(objects):
+                        """Flatten the objects array"""
+                        flat_objects_list = [
+                            item for sublist in objects for item in sublist
+                        ]
+                        objects = np.concatenate(flat_objects_list)
+                        original_size = arrakis_file[f'standard_record/{object}'].shape[0]
+                        additional_size = len(objects)
+                        new_size = original_size + additional_size
+                        """Insert the objects into the array"""
+                        arrakis_file[f'standard_record/{object}'].resize((new_size,))
+                        arrakis_file[f'standard_record/{object}'][original_size:new_size] = objects
+        else:
+            pass
+    
+    @profiler
+    def run_undefined_check(
+        self,
+        file_name: str
+    ):
+        """
+        We check for undefined labels in the arrakis output file and report 
+        information about them.
+
+        Args:
+            file_name (str): _description_
+        """
+        arrakis_file_name = file_name.replace('FLOW', 'ARRAKIS').replace('flow', 'arrakis')
+        with h5py.File(self.flow_folder + file_name, 'r') as flow_file, \
+             h5py.File(self.arrakis_folder + arrakis_file_name, 'a') as arrakis_file:
+            arrakis_charge = arrakis_file['charge/calib_final_hits/data']
+            arrakis_topology = arrakis_charge['topology']
+            arrakis_physics = arrakis_charge['physics']
+            undefined_topology = np.where(arrakis_topology == -1)
+            undefined_physics = np.where(arrakis_physics == -1)
+            
 
     @profiler
     def run_end_of_arrakis(self):
         """
         Set of functions to be run at the end of the entire
         Arrakis job.  Some default operations are to create
         profiling plots.
         """
-        self.generate_timing_and_memory_plots()
+        if len(self.flow_files) != 0:
+            self.generate_timing_and_memory_plots()
         if self.rank == 0:
             try:
                 self.logger.info("Arrakis program ran successfully. Closing out.")
-            except Exception as e:
-                self.error_status = e
+            except Exception as exception:
+                self.report_error(exception=exception)
         else:
             pass
 
     @profiler
     def generate_timing_and_memory_plots(self):
         """Send over timing and memory information from each worker"""
         if self.rank == 0:
             try:
                 collected_timings = {ii: self.comm.recv(source=ii, tag=100) for ii in range(1, self.size)}
                 collected_memory = {ii: self.comm.recv(source=ii, tag=101) for ii in range(1, self.size)}
-            except Exception as e:
-                self.error_status = e
+            except Exception as exception:
+                self.report_error(exception=exception)
             self.barrier()
         else:
             try:
                 self.comm.send(timing_manager.timings, dest=0, tag=100)
                 self.comm.send(memory_manager.memory, dest=0, tag=101)
-            except Exception as e:
-                self.error_status = e
+            except Exception as exception:
+                self.report_error(exception=exception)
             self.barrier()
 
         """Generate timing and memory plots"""
         if self.rank == 0:
             try:
                 collected_timings[0] = timing_manager.timings
                 collected_memory[0] = memory_manager.memory
@@ -1062,16 +1231,16 @@
                 plugin_axs.set_ylabel(r"$\langle\Delta m\rangle$ (Mb)")
                 plugin_axs.set_xticklabels(plugin_labels, rotation=45, ha="right")
                 plugin_axs.set_yscale("log")
                 plt.title(r"Plugin $\langle\Delta m\rangle$ (Mb) vs. function")
                 plt.legend(bbox_to_anchor=(1.05, 1.0), loc="upper left")
                 plt.tight_layout()
                 plt.savefig("/local_scratch/arrakis_nd_plugin_memory_avg.png")
-            except Exception as e:
-                self.error_status = e
+            except Exception as exception:
+                self.report_error(exception=exception)
             self.barrier()
         else:
             self.barrier()
 
     @profiler
     def run_arrakis_nd(self):
         """
@@ -1094,16 +1263,16 @@
         II. Run end of program functions
         """
         self.barrier()
 
         """Set up input files"""
         try:
             self.set_up_input_files()
-        except Exception as e:
-            self.error_status = e
+        except Exception as exception:
+            self.report_error(exception=exception)
         self.barrier()
 
         """Set up progress bar"""
         if self.rank == 0:
             self.logger.info(f'running Arrakis with {self.size} workers.')
             self.progress_bar = tqdm(
                 total=len(self.flow_files),
@@ -1116,64 +1285,96 @@
         """Loop over files and call master/worker methods for each."""
         for ii, file_name in enumerate(self.flow_files):
             """First run begin of file"""
             if self.rank == 0:
                 try:
                     self.progress_bar.set_description_str(f'File [{ii+1}/{len(self.flow_files)}]')
                     self.run_begin_of_file(file_name)
-                except Exception as e:
-                    self.error_status = e
+                except Exception as exception:
+                    self.report_error(exception=exception)
+            self.barrier()
+
+            """Reset event/plugin errors"""
+            self.reset_event_errors()
             self.barrier()
 
             """Set up output arrays in ARRAKIS file"""
             if self.rank == 0:
                 try:
                     self.set_up_output_arrays(file_name)
-                except Exception as e:
-                    self.error_status = e
+                except Exception as exception:
+                    self.report_error(exception=exception)
             self.barrier()
 
             """Prepare indices for workers"""
             try:
                 self.distribute_tasks(file_name)
-            except Exception as e:
-                self.error_status = e
+            except Exception as exception:
+                self.report_error(exception=exception)
             self.barrier()
 
             """Now process the file"""
             try:
                 arrakis_file_name = file_name.replace('FLOW', 'ARRAKIS').replace('flow', 'arrakis')
                 with h5py.File(self.flow_folder + file_name, 'r', driver='mpio', comm=self.comm) as flow_file, \
                      h5py.File(self.arrakis_folder + arrakis_file_name, 'r+', driver='mpio', comm=self.comm) as arrakis_file:
                     self.barrier()
                     if self.rank == 0:
                         """Process event in master node"""
                         try:
                             self.progress_bar.set_postfix_str(f'# Events: [{self.num_events}]')
                             self.process_events_master(flow_file, arrakis_file)
-                        except Exception as e:
-                            self.error_status = e
+                        except Exception as exception:
+                            self.report_error(exception=exception)
                         self.barrier()
                     else:
                         """Process event in worker node"""
                         self.barrier()
                         try:
                             self.process_events_worker(flow_file, arrakis_file)
-                        except Exception as e:
-                            self.error_status = e
-            except Exception as e:
-                self.error_status = e
+                        except Exception as exception:
+                            self.report_error(exception=exception)
+                    """Ensure that changes are pushed to the arrakis file"""
+                    self.barrier()
+                    arrakis_file.flush()
+            except Exception as exception:
+                self.report_error(exception=exception)
             self.barrier()
 
             """Run end of file plugins"""
+            try:
+                self.run_end_of_file(file_name)
+            except Exception as exception:
+                self.report_error(exception=exception)
+            self.barrier()
+            
+            """Run undefined check"""
+            if self.rank == 0:
+                try:
+                    self.run_undefined_check(file_name)
+                except Exception as exception:
+                    self.report_error(exception=exception)
+            self.barrier()
+            
+            """Update progress bar"""
             if self.rank == 0:
                 try:
-                    self.run_end_of_file(file_name)
                     self.progress_bar.update(1)
-                except Exception as e:
-                    self.error_status = e
+                except Exception as exception:
+                    self.report_error(exception=exception)
+            self.barrier()
+
+            """Report any event errors"""
+            try:
+                self.report_event_errors(file_name)
+            except Exception as exception:
+                self.report_error(exception=exception)
             self.barrier()
 
         """Run end of program functions"""
         if self.rank == 0:
-            self.progress_bar.close()
+            try:
+                self.progress_bar.close()
+            except Exception as exception:
+                self.report_error(exception=exception)
+        self.barrier()
         self.run_end_of_arrakis()
```

### Comparing `arrakis_nd-2.0.0/arrakis_nd/plugins/daughter_plugin.py` & `arrakis_nd-2.0.1/arrakis_nd/plugins/daughter_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         config: dict = {}
     ):
         """
         """
         super(DaughterPlugin, self).__init__(config)
 
         self.input_products = None
-        self.output_product = 'daughters'
+        self.output_products = 'daughters'
 
     @profiler
     def process_event(
         self,
         event: int,
         flow_file: h5py.File,
         arrakis_file: h5py.File,
@@ -90,8 +90,8 @@
         for index, pair in enumerate(zip(parent_ids, vertex_ids)):
             pair_to_indices[pair].append(index)
 
         for ii, (traj_id, vertex_id) in enumerate(zip(traj_ids, vertex_ids)):
             # Direct lookup instead of np.where
             daughters[ii] = pair_to_indices.get((traj_id, vertex_id), [])
 
-        event_products['daughters'] = daughters
+        event_products['daughters'] = np.array(daughters, dtype=object)
```

### Comparing `arrakis_nd-2.0.0/arrakis_nd/plugins/empty_plugin.py` & `arrakis_nd-2.0.1/arrakis_nd/plugins/empty_plugin.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
     event_indices = {
         'interactions': indices of the "event" in the 'mc_truth/interactions/data' array
         'segments':     indices of the "event" in the 'mc_truth/segments/data' array
         'stack':        indices of the "event" in the 'mc_truth/stack/data' array
         'trajectories': indices of the "event" in the 'mc_truth/trajectories/data' array
         'charge':       indices of the "event" in the 'charge/calib_final_hits/data' array
+        'light':        indices of the "event" in the 'light/sipm_hits/data' array
     }
     """
     def __init__(
         self,
         config: dict = {}
     ):
         """
@@ -46,28 +47,35 @@
         have only a single input parameter "config", which is a dictionary
         that can contain any number of parameters that can be specified
         at run-time in the corresponding config file.
 
         The 'input_products' and 'output_produces' must be configured!
         The 'input_products' should be either 'None', 'str' or a list of 'str'.  The
         'str's tell Arrakis what plugin output_products that this plugin needs in
-        order to work properly.  For example, the 'daughter_plugin' creates the 
+        order to work properly.  For example, the 'daughter_plugin' creates the
         'daughters' output_product, which contains the indices of the daughters
         for each traj_id in trajectories.  To specify that this plugin needs
         that product, we would write,
 
             self.input_products = 'daughters'   -  or  -  self.input_products = ['daughters']
 
-        The 'output_product' should give the name of the intermediate product (if any)
+        The 'output_products' should give the name of the intermediate product (if any)
         that this plugin produces and appends to the "event_products" dictionary.
+
+        NB! Note that any changes one wishes to make to the arrakis_file happen
+            in a subtle way.  For example, if you index any dataset from the arrakis_file,
+            that will create a new numpy array and will NOT give you a reference
+            to the original dataset.  Therefore, any changes you make must be sent back to
+            the original arrakis_file in the end!  See the particle examples in the plugin
+            folder.
         """
         super(EmptyPlugin, self).__init__(config)
 
         self.input_products = None
-        self.output_product = None
+        self.output_products = None
 
     @profiler
     def process_event(
         self,
         event: int,
         flow_file: h5py.File,
         arrakis_file: h5py.File,
```

### Comparing `arrakis_nd-2.0.0/arrakis_nd/plugins/plugin.py` & `arrakis_nd-2.0.1/arrakis_nd/plugins/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,19 +18,21 @@
         All plugins must run super(CustomPlugin, self).__init__(config)
         and specify any required data_products and any output data_products
         so that Arrakis knows they are called in the correct sequence.
 
         Args:
             config (dict, optional): _description_. Defaults to {}.
         """
+        if config is None:
+            config = {}
         self.config = config
 
         """These should be set by the creator of the custom plugin"""
         self.input_products = None
-        self.output_product = None
+        self.output_products = None
 
     def process_event(
         self,
         event: int,
         flow_file: h5py.File,
         arrakis_file: h5py.File,
         event_indices: dict,
@@ -43,14 +45,21 @@
         both.  The event_products is a shared dictionary which
         can be updated with intermmediate data used by other
         plugins.
 
 
         This function must be overriden by the inherited class.
 
+        NB! Note that any changes one wishes to make to the arrakis_file happen
+            in a subtle way.  For example, if you index any dataset from the arrakis_file,
+            that will create a new numpy array and will NOT give you a reference
+            to the original dataset.  Therefore, any changes you make must be sent back to
+            the original arrakis_file in the end!  See the particle examples in the plugin
+            folder.
+
         Args:
             flow_file (h5py.File): _description_
             arrakis_file (h5py.File): _description_
             event_indices (dict): _description_
             event_products (dict): _description_
         """
         raise NotImplementedError("Plugin classes must implement this function!")
```

### Comparing `arrakis_nd-2.0.0/arrakis_nd/plugins/trackid_hit_map.py` & `arrakis_nd-2.0.1/arrakis_nd/plugins/trackid_hit_map.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 """
 import h5py
 import numpy as np
-from numba import jit
 
 from arrakis_nd.utils.utils import profiler
 from arrakis_nd.plugins.plugin import Plugin
 
 
 class TrackIDHitMapPlugin(Plugin):
     """
@@ -44,15 +43,19 @@
         This is unfortunately very slow, so instead we opt for the solution
         which is currently implemented in process_event.
 
         """
         super(TrackIDHitMapPlugin, self).__init__(config)
 
         self.input_products = None
-        self.output_product = 'track_id_hit_map'
+        self.output_products = [
+            'track_id_hit_map',
+            'track_id_hit_segment_map',
+            'track_id_hit_t0_map'
+        ]
 
     @profiler
     def process_event(
         self,
         event: int,
         flow_file: h5py.File,
         arrakis_file: h5py.File,
@@ -70,32 +73,52 @@
         charge_back_track = flow_file['mc_truth/calib_final_hit_backtrack/data'][event_indices['charge']]
 
         trajectories_traj_ids = trajectories['traj_id']
         trajectories_vertex_ids = trajectories['vertex_id']
         segments_traj_ids = segments['traj_id']
         segments_vertex_ids = segments['vertex_id']
         segments_segment_ids = segments['segment_id']
-        charge_segment_ids = charge_back_track['segment_id']
+        segments_t0s = segments['t0']
+        charge_segment_ids = charge_back_track['segment_id'].astype(int)
+        charge_segment_fraction = charge_back_track['fraction']
+        charge_segment_fraction_mask = (charge_segment_fraction == 0)
+        charge_segment_ids[charge_segment_fraction_mask] = -1
 
         """Create empty map with (traj_id, vertex_id) as keys"""
         track_id_hit_map = {
             (traj_id, vertex_id): []
             for (traj_id, vertex_id) in zip(trajectories_traj_ids, trajectories_vertex_ids)
         }
+        track_id_hit_segment_map = {
+            (traj_id, vertex_id): []
+            for (traj_id, vertex_id) in zip(trajectories_traj_ids, trajectories_vertex_ids)
+        }
+        track_id_hit_t0_map = {
+            (traj_id, vertex_id): []
+            for (traj_id, vertex_id) in zip(trajectories_traj_ids, trajectories_vertex_ids)
+        }
 
         """Loop over segment ids"""
         for ii, segment_ids in enumerate(charge_segment_ids):
             """Get segment_ids of segments of each hit"""
-            segment_ids = segment_ids[(segment_ids != 0)]
+            segment_ids = segment_ids[(segment_ids != -1)]
             """Determine where these ids are in the segments array"""
             segment_indices = np.array([
                 np.where(segments_segment_ids == segment_id)[0][0]
                 if segment_id in segments_segment_ids else -1
                 for segment_id in segment_ids
             ])
             """Associate this hit to the (traj_id, vertex_id) pairs"""
-            for segment_index in segment_indices:
+            for jj, segment_index in enumerate(segment_indices):
                 track_id_hit_map[
                     (segments_traj_ids[segment_index], segments_vertex_ids[segment_index])
                 ].append(ii)
+                track_id_hit_segment_map[
+                    (segments_traj_ids[segment_index], segments_vertex_ids[segment_index])
+                ].append(jj)
+                track_id_hit_t0_map[
+                    (segments_traj_ids[segment_index], segments_vertex_ids[segment_index])
+                ].append(segments_t0s[segment_index])
 
         event_products['track_id_hit_map'] = track_id_hit_map
+        event_products['track_id_hit_segment_map'] = track_id_hit_segment_map
+        event_products['track_id_hit_t0_map'] = track_id_hit_t0_map
```

### Comparing `arrakis_nd-2.0.0/arrakis_nd/programs/plugin_creator.py` & `arrakis_nd-2.0.1/arrakis_nd/programs/plugin_creator.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.0/arrakis_nd/programs/run_arrakis.py` & `arrakis_nd-2.0.1/arrakis_nd/programs/run_arrakis.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,87 +6,104 @@
 
 from arrakis_nd.utils.logger import Logger
 from arrakis_nd.utils.config import ConfigParser
 from arrakis_nd.arrakis.arrakis import Arrakis
 
 
 def run():
-    """_summary_
     """
+    This program runs the Arrakis module from a config file.
+    It utilizes MPI + H5 to distribute the processing of events
+    over multiple cores which greatly speeds up runtime.  When 
+    used in conjunction with the "create_arrakis_runs" program,
+    running a post-flow ARRAKIS can performed in minutes.
+    """
+
+    """Create a logger instance"""
+    logger = Logger("arrakis_runner")
 
     """
     We do a preliminary check to ensure that MPI is available
     and that the number of processes is at least 2.  Assuming
     that ArrakisND is being run on a system with more than one
     CPU core.
     """
-    logger = Logger("arrakis_runner", output="both")
-
     try:
         comm = MPI.COMM_WORLD
         size = comm.Get_size()
 
-        # check that size >= 2, which is required
-        # for Arrakis to run.  Otherwise we quit early
+        """Check that size >= 2, which is required for Arrakis to run.  Otherwise we quit early"""
         if size < 2:
-            logger.error(f"Number of processes must be >=2! Received {size} from MPI", "value")
+            logger.error(f"number of processes must be >=2! Received {size} from MPI", "value")
     except Exception as e:
-        logger.error(f"Error occurred with gathering MPI: {e}", "runtime")
+        logger.error(f"error occurred with gathering MPI: {e}", "runtime")
 
+    """Set up command line arguments"""
     parser = argparse.ArgumentParser(
         prog="Arrakis Module Runner",
-        description="This program runs the Arrakis module " + "from a config file.",
+        description="This program runs the Arrakis module from a config file. \
+            It utilizes MPI + H5 to distribute the processing of events \
+            over multiple cores which greatly speeds up runtime.  When \
+            used in conjunction with the 'create_arrakis_runs' program, \
+            running a post-flow ARRAKIS can performed in minutes.",
         epilog="...",
     )
     parser.add_argument(
         "config_file",
         metavar="<config_file>.yml",
         type=str,
-        help="config file specification for a BLIP module.",
+        help="config file specification for this Arrakis module.",
     )
     parser.add_argument(
         "-name",
         dest="name",
         default="arrakis",
         help='name for this run (default "arrakis").',
     )
     parser.add_argument(
         "-n",
         dest="number_of_files",
         default=None,
         help='number of files to process (default None).',
     )
-    args = parser.parse_args()
 
+    """Parse command line arguments"""
+    args = parser.parse_args()
     config_file = args.config_file
     name = args.name
     number_of_files = args.number_of_files
 
+    """Parse the config file"""
     try:
         config = ConfigParser(config_file).data
     except Exception as e:
         logger.error(f"failed to parse config: {e}")
 
+    """Determine whether to only pick a subset of files"""
     if number_of_files is not None:
         try:
             number_of_files = int(number_of_files)
         except Exception as e:
             logger.error(f"unable to convert number_of_files from {type(number_of_files)} to int: {e}")
 
         if isinstance(number_of_files, int):
             if number_of_files > 0:
                 config["arrakis_nd"]["number_of_files"] = number_of_files
+
+    """Construct meta dictionary"""
     meta = {
         "name": name,
         "config_file": config_file
     }
 
+    """Create the Arrakis instance"""
     try:
         arrakis = Arrakis(config, meta)
     except Exception as e:
         logger.error(f"failed to construct Arrakis object: {e}")
 
+    """Run Arrakis"""
     arrakis.run_arrakis_nd()
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `arrakis_nd-2.0.0/arrakis_nd/utils/config.py` & `arrakis_nd-2.0.1/arrakis_nd/utils/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Tools for parsing config files
 """
 import yaml
 
-from arrakis_nd.utils.logger import Logger
 from arrakis_nd.utils.utils import profiler
 
 
 class ConfigParser:
     """
     Config file parser for Arrakis.  This class simply
     wraps the pyyaml class with some added functionality,
@@ -83,10 +82,12 @@
             config_dictionary (_str_): The location of the config
             file to be loaded.
             output_file (_str_): The location and name of the output
             yaml file.
         """
         try:
             with open(output_file, 'w') as file:
-                yaml.dump(config_dictionary, file)
+                yaml.dump(config_dictionary, file, sort_keys=False)
         except Exception as e:
-            raise RuntimeError(f"Failed to save config dictionary {config_dictionary} to output file {output_file}: {e}")
+            raise RuntimeError(
+                f"Failed to save config dictionary {config_dictionary} to output file {output_file}: {e}"
+            )
```

### Comparing `arrakis_nd-2.0.0/arrakis_nd/utils/logger.py` & `arrakis_nd-2.0.1/arrakis_nd/utils/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,43 +10,51 @@
 import uuid
 import psutil
 import os
 
 
 class ArrakisError(Exception):
     """Custom default error for Arrakis"""
-    def __init__(self, message="An error occurred"):
+    def __init__(
+        self,
+        message="An error occurred"
+    ):
+        self.message = message
+        super().__init__(self.message)
+
+
+class EventError(Exception):
+    """Custom default error for an event"""
+    def __init__(
+        self,
+        message="An error occurred"
+    ):
         self.message = message
         super().__init__(self.message)
 
 
 logging_level = {
     "debug": logging.DEBUG,
     "info": logging.INFO,
     "warning": logging.WARNING,
     "error": logging.ERROR,
     "critical": logging.CRITICAL,
 }
 
-logging_output = [
-    "console",
-    "file",
-    "both",
-]
-
 warning_list = {
     "deprecation": DeprecationWarning,
     "import": ImportWarning,
     "resource": ResourceWarning,
     "user": UserWarning,
 }
 
 error_list = {
     "attribute": AttributeError,
     "arrakis": ArrakisError,
+    "event": EventError,
     "index": IndexError,
     "file": FileExistsError,
     "memory": MemoryError,
     "runtime": RuntimeError,
     "type": TypeError,
     "value": ValueError,
 }
@@ -94,17 +102,14 @@
         (3) debug
     """
 
     def __init__(
         self,
         name: str = "default",
         level: str = "debug",
-        output: str = "file",
-        output_file: str = "log",
-        file_mode: str = "a",
     ):
         """
         Initializer for the logger
 
         Args:
             name (str, optional): name for this logger (will appear
             after the log message type [ERROR] [name]). Defaults to "default".
@@ -115,36 +120,32 @@
 
             output_file (str, optional): name of the output file. Defaults to "log".
             file_mode (str, optional): whether to append, or rewrite
             log files for this run. Defaults to "a".
 
         Raises:
             ValueError: _description_
-            ValueError: _description_
         """
         # check for mistakes
         if level not in logging_level.keys():
             raise ValueError(f"Logging level {level} not in {logging_level}.")
-        if output not in logging_output:
-            raise ValueError(f"Logging handler {output} not in {logging_output}.")
 
         # create the logging directory
         if "LOCAL_SCRATCH" in os.environ.keys():
             self.local_log_dir = os.environ["LOCAL_SCRATCH"] + "/.logs/"
         else:
             self.local_log_dir = "/local_scratch/.logs/"
         if not os.path.isdir(self.local_log_dir):
             os.makedirs(self.local_log_dir)
 
         # use the name as the default output file name
         self.name = name
         self.level = logging_level[level]
-        self.output = output
-        self.output_file = output_file
-        self.file_mode = file_mode
+        self.output_file = "arrakis"
+        self.file_mode = "a"
 
         # create logger
         self.logger = logging.getLogger(self.name)
         self.debug_logger = logging.getLogger(self.name + "_debug")
 
         # set level
         self.logger.setLevel(self.level)
@@ -160,26 +161,24 @@
 
         self.debug = logging.FileHandler(
             self.local_log_dir + "/" + self.output_file + ".debug", mode="a"
         )
         self.debug.setLevel(self.level)
 
         # create handler
-        if self.output == "console" or self.output == "both":
-            self.console = logging.StreamHandler()
-            self.console.setLevel(self.level)
-            self.console.setFormatter(self.console_formatter)
-            self.logger.addHandler(self.console)
-        if self.output == "file" or self.output == "both":
-            self.file = logging.FileHandler(
-                self.local_log_dir + "/" + self.output_file + ".log", mode="a"
-            )
-            self.file.setLevel(logging.DEBUG)
-            self.file.setFormatter(self.file_formatter)
-            self.logger.addHandler(self.file)
+        self.console = logging.StreamHandler()
+        self.console.setLevel(self.level)
+        self.console.setFormatter(self.console_formatter)
+        self.logger.addHandler(self.console)
+        self.file = logging.FileHandler(
+            self.local_log_dir + "/" + self.output_file + ".log", mode="a"
+        )
+        self.file.setLevel(logging.DEBUG)
+        self.file.setFormatter(self.file_formatter)
+        self.logger.addHandler(self.file)
         self.debug.setFormatter(self.file)
         self.debug_logger.addHandler(self.debug)
         self.logger.propagate = False
 
     def info(
         self,
         message: str,
@@ -244,18 +243,14 @@
         if warning_type not in warning_list.keys():
             warning_type = "user"
         self.logger.warning(message)
         warnings.warn(
             f"traceback: {formatted_lines}\nerror: {message}",
             warning_list[warning_type],
         )
-        if self.output == "file":
-            return self.logger.warning(
-                f"traceback: {formatted_lines}\nerror: {message}"
-            )
         return
 
     def error(
         self,
         message: str,
         error_type: str = "arrakis",
     ):
@@ -269,18 +264,15 @@
             error_list: _description_
         """
         """Output to the standard logger "error" """
         formatted_traceback = ''.join(traceback.format_stack())
         if error_type not in error_list.keys():
             error_type = "arrakis"
         log_message = f"Traceback: \n{formatted_traceback}\nError: {message}"
-        if self.output == "file":
-            self.logger.error(log_message)
-        else:
-            self.logger.error(message)
+        self.logger.error(message)
         raise error_list[error_type](log_message)
 
     def critical(
         self,
         message: str
     ):
         """
```

### Comparing `arrakis_nd-2.0.0/arrakis_nd/utils/utils.py` & `arrakis_nd-2.0.1/arrakis_nd/utils/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 """
 from collections import defaultdict
 import functools
 from datetime import datetime
 import psutil
 import time
 import os
+import numpy as np
+from scipy.interpolate import splev
 
 
 def get_datetime():
     """
     Returns a datetime in the format of:
     YYYY.MM.DD.HH.MM.SS
 
@@ -18,14 +20,41 @@
         _type_: _description_
     """
     time = datetime.now()
     now = f"{time.year}.{time.month}.{time.day}.{time.hour}.{time.minute}.{time.second}"
     return now
 
 
+def integrand(t, tck):
+    dxdt, dydt, dzdt = splev(t, tck, der=1)
+    return np.sqrt(dxdt**2 + dydt**2 + dzdt**2)
+
+
+def fiducialized_vertex(vert_pos):
+    lar_x = [
+        (-63.9273, -3.0652),
+        (3.0652, 63.9273)
+    ]
+    lar_y = [(-62.055, 62.055)]
+    lar_z = [
+        (-64.51125, -2.48125),
+        (2.48125, 64.51125)
+    ]
+    for i in lar_z:
+        if vert_pos[2] < i[0] and vert_pos[2] > i[1]:
+            return False
+    for i in lar_x:
+        if vert_pos[0] < i[0] and vert_pos[0] > i[1]:
+            return False
+    for i in lar_y:
+        if vert_pos[1] < i[0] and vert_pos[1] > i[1]:
+            return False
+    return True
+
+
 class ResetableIterator:
     """_summary_
     """
     def __init__(self):
         self._value = 0
 
     def __iter__(self):
```

### Comparing `arrakis_nd-2.0.0/arrakis_nd.egg-info/PKG-INFO` & `arrakis_nd-2.0.1/arrakis_nd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrakis_nd
-Version: 2.0.0
+Version: 2.0.1
 Summary: Arrakis module for near detector data.
 Home-page: https://github.com/Neutron-Calibration-in-DUNE/ArrakisND
 Author: Nicholas Carrara, Marjolein van Nuland, Luis Lepin
 Author-email: ncarrara.physics@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -25,14 +25,16 @@
 Requires-Dist: charset-normalizer
 Requires-Dist: colorama
 Requires-Dist: colorcet==3.1.0
 Requires-Dist: comm
 Requires-Dist: contourpy
 Requires-Dist: cryptography==42.0.5
 Requires-Dist: cycler
+Requires-Dist: dash
+Requires-Dist: dash-bootstrap-components
 Requires-Dist: debugpy
 Requires-Dist: decorator
 Requires-Dist: docutils==0.20.1
 Requires-Dist: exceptiongroup
 Requires-Dist: executing
 Requires-Dist: fonttools
 Requires-Dist: h5py
```

### Comparing `arrakis_nd-2.0.0/arrakis_nd.egg-info/requires.txt` & `arrakis_nd-2.0.1/arrakis_nd.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 charset-normalizer
 colorama
 colorcet==3.1.0
 comm
 contourpy
 cryptography==42.0.5
 cycler
+dash
+dash-bootstrap-components
 debugpy
 decorator
 docutils==0.20.1
 exceptiongroup
 executing
 fonttools
 h5py
```

### Comparing `arrakis_nd-2.0.0/setup.py` & `arrakis_nd-2.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,31 +11,30 @@
 
 setup(
     # name
     name="arrakis_nd",
     # current version
     #   MAJOR VERSION:  02
     #   MINOR VERSION:  00
-    #   Maintenance:    00
-    version="2.00.00",
+    #   Maintenance:    01
+    version="2.00.01",
     # descriptions
     description="Arrakis module for near detector data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="",
     # my info
     author="Nicholas Carrara, Marjolein van Nuland, Luis Lepin",
     author_email="ncarrara.physics@gmail.com",
     # where to find the source
     url="https://github.com/Neutron-Calibration-in-DUNE/ArrakisND",
     # requirements
     install_requires=read_requirements(),
     # packages
     packages=find_packages(
-        # where='pointnet',
         exclude=["test"],
     ),
     include_package_data=True,
     # classifiers
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
@@ -45,12 +44,13 @@
         "Programming Language :: Python :: 3",
     ],
     python_requires=">3.7",
     # possible entry point
     entry_points={
         "console_scripts": [
             "arrakis_nd = arrakis_nd.programs.run_arrakis:run",
+            "arrakis_display = arrakis_nd.programs.run_arrakis_display:run",
             "create_arrakis_runs = arrakis_nd.programs.create_arrakis_runs:run",
             'create_plugin = arrakis_nd.programs.plugin_creator:run',
         ],
     },
 )
```


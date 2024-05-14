# Comparing `tmp/ecoscope-1.7.1.tar.gz` & `tmp/ecoscope-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoscope-1.7.1.tar", last modified: Thu May  9 09:59:22 2024, max compression
+gzip compressed data, was "ecoscope-1.7.2.tar", last modified: Tue May 14 13:43:06 2024, max compression
```

## Comparing `ecoscope-1.7.1.tar` & `ecoscope-1.7.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.313376 ecoscope-1.7.1/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1553 2024-05-09 09:56:48.000000 ecoscope-1.7.1/LICENSE
--rw-r--r--   0 gitonga   (1000) gitonga   (1000)     4438 2024-05-09 09:59:22.313376 ecoscope-1.7.1/PKG-INFO
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2946 2024-05-09 09:56:48.000000 ecoscope-1.7.1/README.rst
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.305375 ecoscope-1.7.1/ecoscope/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3762 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/__init__.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.305375 ecoscope-1.7.1/ecoscope/analysis/
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.305375 ecoscope-1.7.1/ecoscope/analysis/UD/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      105 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/UD/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7011 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/UD/etd_range.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      375 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1027 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/astronomy.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15978 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/ecograph.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3849 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/geofence.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2955 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/immobility.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3208 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/percentile.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2147 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/proximity.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4852 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/seasons.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2725 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/speed.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.309376 ecoscope-1.7.1/ecoscope/base/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      602 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/base/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1776 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/base/_dataclasses.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    25126 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/base/base.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7698 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/base/utils.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.309376 ecoscope-1.7.1/ecoscope/contrib/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       61 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/contrib/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    10988 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/contrib/basemaps.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)   123902 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/contrib/foliumap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5197 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/contrib/geemap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2359 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/contrib/legend.txt
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.309376 ecoscope-1.7.1/ecoscope/io/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      272 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/io/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    39308 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/io/earthranger.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15220 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/io/eetools.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6616 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/io/raster.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2652 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/io/utils.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.309376 ecoscope-1.7.1/ecoscope/mapping/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      324 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/mapping/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    32305 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/mapping/map.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.309376 ecoscope-1.7.1/ecoscope/plotting/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      268 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/plotting/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7390 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/plotting/plot.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       22 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/version.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.313376 ecoscope-1.7.1/ecoscope.egg-info/
--rw-r--r--   0 gitonga   (1000) gitonga   (1000)     4438 2024-05-09 09:59:22.000000 ecoscope-1.7.1/ecoscope.egg-info/PKG-INFO
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1372 2024-05-09 09:59:22.000000 ecoscope-1.7.1/ecoscope.egg-info/SOURCES.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2024-05-09 09:59:22.000000 ecoscope-1.7.1/ecoscope.egg-info/dependency_links.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2024-05-09 09:59:22.000000 ecoscope-1.7.1/ecoscope.egg-info/not-zip-safe
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      285 2024-05-09 09:59:22.000000 ecoscope-1.7.1/ecoscope.egg-info/requires.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        9 2024-05-09 09:59:22.000000 ecoscope-1.7.1/ecoscope.egg-info/top_level.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      591 2024-05-09 09:56:48.000000 ecoscope-1.7.1/pyproject.toml
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       38 2024-05-09 09:59:22.313376 ecoscope-1.7.1/setup.cfg
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1977 2024-05-09 09:56:48.000000 ecoscope-1.7.1/setup.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.313376 ecoscope-1.7.1/tests/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7084 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_base.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7182 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_earthranger_io.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4840 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_ecodataframe.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5198 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_ecograph.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6126 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_ecomap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5933 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_eetools.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1876 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_geofence.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      790 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_immobility.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2492 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_io_utils.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      962 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_seasons.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      306 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_speed.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2091 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_ud.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      443 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-14 13:43:06.136045 ecoscope-1.7.2/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1553 2024-05-14 13:37:42.000000 ecoscope-1.7.2/LICENSE
+-rw-r--r--   0 gitonga   (1000) gitonga   (1000)     4438 2024-05-14 13:43:06.136045 ecoscope-1.7.2/PKG-INFO
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2946 2024-05-14 13:37:42.000000 ecoscope-1.7.2/README.rst
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-14 13:43:06.128045 ecoscope-1.7.2/ecoscope/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3762 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/__init__.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-14 13:43:06.128045 ecoscope-1.7.2/ecoscope/analysis/
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-14 13:43:06.128045 ecoscope-1.7.2/ecoscope/analysis/UD/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      105 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/analysis/UD/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7011 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/analysis/UD/etd_range.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      375 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/analysis/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1027 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/analysis/astronomy.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15978 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/analysis/ecograph.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3849 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/analysis/geofence.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2955 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/analysis/immobility.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3208 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/analysis/percentile.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2147 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/analysis/proximity.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4852 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/analysis/seasons.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2725 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/analysis/speed.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-14 13:43:06.132045 ecoscope-1.7.2/ecoscope/base/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      602 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/base/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1776 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/base/_dataclasses.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    25126 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/base/base.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7698 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/base/utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-14 13:43:06.132045 ecoscope-1.7.2/ecoscope/contrib/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       61 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/contrib/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    10988 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/contrib/basemaps.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)   123902 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/contrib/foliumap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5197 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/contrib/geemap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2359 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/contrib/legend.txt
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-14 13:43:06.132045 ecoscope-1.7.2/ecoscope/io/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      272 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/io/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    39308 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/io/earthranger.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15220 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/io/eetools.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6616 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/io/raster.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2652 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/io/utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-14 13:43:06.132045 ecoscope-1.7.2/ecoscope/mapping/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      324 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/mapping/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    32305 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/mapping/map.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-14 13:43:06.132045 ecoscope-1.7.2/ecoscope/plotting/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      268 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/plotting/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7390 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/plotting/plot.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       22 2024-05-14 13:37:42.000000 ecoscope-1.7.2/ecoscope/version.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-14 13:43:06.136045 ecoscope-1.7.2/ecoscope.egg-info/
+-rw-r--r--   0 gitonga   (1000) gitonga   (1000)     4438 2024-05-14 13:43:06.000000 ecoscope-1.7.2/ecoscope.egg-info/PKG-INFO
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1372 2024-05-14 13:43:06.000000 ecoscope-1.7.2/ecoscope.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2024-05-14 13:43:06.000000 ecoscope-1.7.2/ecoscope.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2024-05-14 13:43:05.000000 ecoscope-1.7.2/ecoscope.egg-info/not-zip-safe
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      285 2024-05-14 13:43:06.000000 ecoscope-1.7.2/ecoscope.egg-info/requires.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        9 2024-05-14 13:43:06.000000 ecoscope-1.7.2/ecoscope.egg-info/top_level.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      591 2024-05-14 13:37:42.000000 ecoscope-1.7.2/pyproject.toml
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       38 2024-05-14 13:43:06.136045 ecoscope-1.7.2/setup.cfg
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1977 2024-05-14 13:37:42.000000 ecoscope-1.7.2/setup.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-14 13:43:06.136045 ecoscope-1.7.2/tests/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7084 2024-05-14 13:37:43.000000 ecoscope-1.7.2/tests/test_base.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7084 2024-05-14 13:37:43.000000 ecoscope-1.7.2/tests/test_earthranger_io.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4840 2024-05-14 13:37:43.000000 ecoscope-1.7.2/tests/test_ecodataframe.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5198 2024-05-14 13:37:43.000000 ecoscope-1.7.2/tests/test_ecograph.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6126 2024-05-14 13:37:43.000000 ecoscope-1.7.2/tests/test_ecomap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5933 2024-05-14 13:37:43.000000 ecoscope-1.7.2/tests/test_eetools.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1876 2024-05-14 13:37:43.000000 ecoscope-1.7.2/tests/test_geofence.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      790 2024-05-14 13:37:43.000000 ecoscope-1.7.2/tests/test_immobility.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2492 2024-05-14 13:37:43.000000 ecoscope-1.7.2/tests/test_io_utils.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      962 2024-05-14 13:37:43.000000 ecoscope-1.7.2/tests/test_seasons.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      306 2024-05-14 13:37:43.000000 ecoscope-1.7.2/tests/test_speed.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2091 2024-05-14 13:37:43.000000 ecoscope-1.7.2/tests/test_ud.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      443 2024-05-14 13:37:43.000000 ecoscope-1.7.2/tests/test_utils.py
```

### Comparing `ecoscope-1.7.1/LICENSE` & `ecoscope-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/PKG-INFO` & `ecoscope-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoscope
-Version: 1.7.1
+Version: 1.7.2
 Summary: Standard Analytical Reporting Framework for Conservation
 Home-page: http://github.com/wildlife-dynamics/ecoscope
 Author: Jake Wall
 Author-email: walljcg@gmail.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ecoscope-1.7.1/README.rst` & `ecoscope-1.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/__init__.py` & `ecoscope-1.7.2/ecoscope/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/analysis/UD/etd_range.py` & `ecoscope-1.7.2/ecoscope/analysis/UD/etd_range.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/analysis/astronomy.py` & `ecoscope-1.7.2/ecoscope/analysis/astronomy.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/analysis/ecograph.py` & `ecoscope-1.7.2/ecoscope/analysis/ecograph.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/analysis/geofence.py` & `ecoscope-1.7.2/ecoscope/analysis/geofence.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/analysis/immobility.py` & `ecoscope-1.7.2/ecoscope/analysis/immobility.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/analysis/percentile.py` & `ecoscope-1.7.2/ecoscope/analysis/percentile.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/analysis/proximity.py` & `ecoscope-1.7.2/ecoscope/analysis/proximity.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/analysis/seasons.py` & `ecoscope-1.7.2/ecoscope/analysis/seasons.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/analysis/speed.py` & `ecoscope-1.7.2/ecoscope/analysis/speed.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/base/__init__.py` & `ecoscope-1.7.2/ecoscope/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/base/_dataclasses.py` & `ecoscope-1.7.2/ecoscope/base/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/base/base.py` & `ecoscope-1.7.2/ecoscope/base/base.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/base/utils.py` & `ecoscope-1.7.2/ecoscope/base/utils.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/contrib/basemaps.py` & `ecoscope-1.7.2/ecoscope/contrib/basemaps.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/contrib/foliumap.py` & `ecoscope-1.7.2/ecoscope/contrib/foliumap.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/contrib/geemap.py` & `ecoscope-1.7.2/ecoscope/contrib/geemap.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/contrib/legend.txt` & `ecoscope-1.7.2/ecoscope/contrib/legend.txt`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/io/earthranger.py` & `ecoscope-1.7.2/ecoscope/io/earthranger.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/io/eetools.py` & `ecoscope-1.7.2/ecoscope/io/eetools.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/io/raster.py` & `ecoscope-1.7.2/ecoscope/io/raster.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/io/utils.py` & `ecoscope-1.7.2/ecoscope/io/utils.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/mapping/map.py` & `ecoscope-1.7.2/ecoscope/mapping/map.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope/plotting/plot.py` & `ecoscope-1.7.2/ecoscope/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/ecoscope.egg-info/PKG-INFO` & `ecoscope-1.7.2/ecoscope.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoscope
-Version: 1.7.1
+Version: 1.7.2
 Summary: Standard Analytical Reporting Framework for Conservation
 Home-page: http://github.com/wildlife-dynamics/ecoscope
 Author: Jake Wall
 Author-email: walljcg@gmail.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ecoscope-1.7.1/ecoscope.egg-info/SOURCES.txt` & `ecoscope-1.7.2/ecoscope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/pyproject.toml` & `ecoscope-1.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/setup.py` & `ecoscope-1.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/tests/test_base.py` & `ecoscope-1.7.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/tests/test_earthranger_io.py` & `ecoscope-1.7.2/tests/test_earthranger_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,15 +187,14 @@
     )
 
     result = er_io.patch_event(event_id=event_id, events=updated_event)
     result = result[["priority", "state", "location"]]
     pd.testing.assert_frame_equal(result, updated_event)
 
 
-@pytest.mark.skip(reason="Known issue: https://github.com/wildlife-dynamics/ecoscope/issues/109")
 def test_get_patrol_observations(er_io):
     patrols = er_io.get_patrols()
     observations = er_io.get_patrol_observations(
         patrols,
         include_source_details=False,
         include_subject_details=False,
         include_subjectsource_details=False,
```

### Comparing `ecoscope-1.7.1/tests/test_ecodataframe.py` & `ecoscope-1.7.2/tests/test_ecodataframe.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/tests/test_ecograph.py` & `ecoscope-1.7.2/tests/test_ecograph.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/tests/test_ecomap.py` & `ecoscope-1.7.2/tests/test_ecomap.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/tests/test_eetools.py` & `ecoscope-1.7.2/tests/test_eetools.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/tests/test_geofence.py` & `ecoscope-1.7.2/tests/test_geofence.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/tests/test_immobility.py` & `ecoscope-1.7.2/tests/test_immobility.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/tests/test_io_utils.py` & `ecoscope-1.7.2/tests/test_io_utils.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/tests/test_seasons.py` & `ecoscope-1.7.2/tests/test_seasons.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.1/tests/test_ud.py` & `ecoscope-1.7.2/tests/test_ud.py`

 * *Files identical despite different names*


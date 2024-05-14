# Comparing `tmp/pdstools-3.4.1.tar.gz` & `tmp/pdstools-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdstools-3.4.1.tar", last modified: Wed Mar  6 15:31:45 2024, max compression
+gzip compressed data, was "pdstools-3.4.3.tar", last modified: Tue May 14 12:54:08 2024, max compression
```

## Comparing `pdstools-3.4.1.tar` & `pdstools-3.4.3.tar`

### file list

```diff
@@ -1,65 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:45.078296 pdstools-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-06 15:31:33.000000 pdstools-3.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-03-06 15:31:45.078296 pdstools-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-03-06 15:31:33.000000 pdstools-3.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:45.078296 pdstools-3.4.1/pdstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-03-06 15:31:45.000000 pdstools-3.4.1/pdstools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-06 15:31:45.000000 pdstools-3.4.1/pdstools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 15:31:45.000000 pdstools-3.4.1/pdstools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-06 15:31:45.000000 pdstools-3.4.1/pdstools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-06 15:31:45.000000 pdstools-3.4.1/pdstools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-06 15:31:45.000000 pdstools-3.4.1/pdstools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-06 15:31:33.000000 pdstools-3.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:45.070296 pdstools-3.4.1/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:45.070296 pdstools-3.4.1/python/pdstools/
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:45.070296 pdstools-3.4.1/python/pdstools/adm/
--rw-r--r--   0 runner    (1001) docker     (127)    57007 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/adm/ADMDatamart.py
--rw-r--r--   0 runner    (1001) docker     (127)    40133 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/adm/ADMTrees.py
--rw-r--r--   0 runner    (1001) docker     (127)    37033 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/adm/BinAggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/adm/Tables.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/adm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:45.074296 pdstools-3.4.1/python/pdstools/app/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/app/Home.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/app/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:45.074296 pdstools-3.4.1/python/pdstools/app/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/app/pages/1-Data Import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/app/pages/2-Data Filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/app/pages/3-Reports.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/app/pages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:45.074296 pdstools-3.4.1/python/pdstools/ih/
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/ih/IHAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/ih/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/ih/legacy_IH.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:45.074296 pdstools-3.4.1/python/pdstools/pega_io/
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/pega_io/API.py
--rw-r--r--   0 runner    (1001) docker     (127)    14118 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/pega_io/File.py
--rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/pega_io/S3.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/pega_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:45.074296 pdstools-3.4.1/python/pdstools/plots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56144 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/plots/plot_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    30223 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/plots/plots_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:45.074296 pdstools-3.4.1/python/pdstools/reports/
--rw-r--r--   0 runner    (1001) docker     (127)    66890 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/reports/HealthCheck.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    21608 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/reports/ModelReport.qmd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:45.078296 pdstools-3.4.1/python/pdstools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26563 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/utils/cdh_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    18148 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/utils/hds_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22249 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/utils/hds_utils_experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/utils/pega_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/utils/polars_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/utils/show_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13806 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/utils/streamlit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/utils/table_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:45.078296 pdstools-3.4.1/python/pdstools/valuefinder/
--rw-r--r--   0 runner    (1001) docker     (127)    25325 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/valuefinder/ValueFinder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/pdstools/valuefinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-06 15:31:33.000000 pdstools-3.4.1/python/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 15:31:45.078296 pdstools-3.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:08.024422 pdstools-3.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 12:54:03.000000 pdstools-3.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-14 12:54:08.024422 pdstools-3.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-14 12:54:03.000000 pdstools-3.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:08.024422 pdstools-3.4.3/pdstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-14 12:54:08.000000 pdstools-3.4.3/pdstools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-14 12:54:08.000000 pdstools-3.4.3/pdstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:54:08.000000 pdstools-3.4.3/pdstools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 12:54:08.000000 pdstools-3.4.3/pdstools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-14 12:54:08.000000 pdstools-3.4.3/pdstools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 12:54:08.000000 pdstools-3.4.3/pdstools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-14 12:54:03.000000 pdstools-3.4.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:08.016422 pdstools-3.4.3/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:08.016422 pdstools-3.4.3/python/pdstools/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:08.016422 pdstools-3.4.3/python/pdstools/adm/
+-rw-r--r--   0 runner    (1001) docker     (127)    70935 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/adm/ADMDatamart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40133 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/adm/ADMTrees.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37033 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/adm/BinAggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/adm/Tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/adm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:08.016422 pdstools-3.4.3/python/pdstools/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/app/Home.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/app/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:08.016422 pdstools-3.4.3/python/pdstools/app/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/app/pages/1-Data Import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/app/pages/2-Data Filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/app/pages/3-Reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/app/pages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:08.016422 pdstools-3.4.3/python/pdstools/ih/
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/ih/IHAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/ih/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/ih/legacy_IH.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:08.020422 pdstools-3.4.3/python/pdstools/pega_io/
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/pega_io/API.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14118 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/pega_io/File.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/pega_io/S3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/pega_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:08.020422 pdstools-3.4.3/python/pdstools/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56393 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/plots/plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30155 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/plots/plots_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:08.020422 pdstools-3.4.3/python/pdstools/prediction/
+-rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/prediction/Prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/prediction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:08.020422 pdstools-3.4.3/python/pdstools/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)    73261 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/reports/HealthCheck.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    21608 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/reports/ModelReport.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:08.020422 pdstools-3.4.3/python/pdstools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26736 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/utils/cdh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18148 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/utils/hds_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22249 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/utils/hds_utils_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/utils/pega_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/utils/polars_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/utils/show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13806 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/utils/streamlit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/utils/table_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:08.024422 pdstools-3.4.3/python/pdstools/valuefinder/
+-rw-r--r--   0 runner    (1001) docker     (127)    25325 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/valuefinder/ValueFinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/pdstools/valuefinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 12:54:03.000000 pdstools-3.4.3/python/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:54:08.024422 pdstools-3.4.3/setup.cfg
```

### Comparing `pdstools-3.4.1/LICENSE` & `pdstools-3.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/PKG-INFO` & `pdstools-3.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.4.1
+Version: 3.4.3
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
@@ -18,15 +18,15 @@
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: tabulate
 Requires-Dist: plotly>=5.5.0
 Requires-Dist: requests
 Requires-Dist: pydot
 Requires-Dist: tqdm
-Requires-Dist: polars<=0.20.2,>=0.20.0
+Requires-Dist: polars~=0.20.0
 Requires-Dist: pyarrow
 Requires-Dist: pyyaml
 Requires-Dist: aioboto3>=11.0
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-autoapi; extra == "docs"
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.4.1 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.4.3 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
 pega,pegasystems,pds,pdstools,cdhtools,datascientist,tools Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pandas Requires-Dist: tabulate
 Requires-Dist: plotly>=5.5.0 Requires-Dist: requests Requires-Dist: pydot
-Requires-Dist: tqdm Requires-Dist: polars<=0.20.2,>=0.20.0 Requires-Dist:
-pyarrow Requires-Dist: pyyaml Requires-Dist: aioboto3>=11.0 Provides-Extra:
-docs Requires-Dist: sphinx; extra == "docs" Requires-Dist: furo; extra ==
-"docs" Requires-Dist: sphinx-autoapi; extra == "docs" Requires-Dist: nbsphinx;
-extra == "docs" Requires-Dist: sphinx-copybutton; extra == "docs" Requires-
-Dist: myst-parser; extra == "docs" Provides-Extra: app Requires-Dist:
+Requires-Dist: tqdm Requires-Dist: polars~=0.20.0 Requires-Dist: pyarrow
+Requires-Dist: pyyaml Requires-Dist: aioboto3>=11.0 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs" Requires-Dist: furo; extra == "docs"
+Requires-Dist: sphinx-autoapi; extra == "docs" Requires-Dist: nbsphinx; extra
+== "docs" Requires-Dist: sphinx-copybutton; extra == "docs" Requires-Dist:
+myst-parser; extra == "docs" Provides-Extra: app Requires-Dist:
 streamlit>=1.23; extra == "app" Requires-Dist: quarto; extra == "app" Requires-
 Dist: papermill; extra == "app" Requires-Dist: itables; extra == "app"
 Requires-Dist: jinja2>=3.1; extra == "app" Requires-Dist: xlsxwriter>=3.0;
 extra == "app" Requires-Dist: tabulate; extra == "app"
 ************ PPeeggaa DDaattaa SScciieennttiisstt TToooollss ************
                                   [Pega logo]
  _[_P_y_t_h_o_n_ _t_e_s_t_s_]_[_R_ _t_e_s_t_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_p_e_g_a_s_y_s_t_e_m_s_/_p_e_g_a_-_d_a_t_a_s_c_i_e_n_t_i_s_t_-
```

### Comparing `pdstools-3.4.1/README.md` & `pdstools-3.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/pdstools.egg-info/PKG-INFO` & `pdstools-3.4.3/pdstools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.4.1
+Version: 3.4.3
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
@@ -18,15 +18,15 @@
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: tabulate
 Requires-Dist: plotly>=5.5.0
 Requires-Dist: requests
 Requires-Dist: pydot
 Requires-Dist: tqdm
-Requires-Dist: polars<=0.20.2,>=0.20.0
+Requires-Dist: polars~=0.20.0
 Requires-Dist: pyarrow
 Requires-Dist: pyyaml
 Requires-Dist: aioboto3>=11.0
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-autoapi; extra == "docs"
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.4.1 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.4.3 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
 pega,pegasystems,pds,pdstools,cdhtools,datascientist,tools Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pandas Requires-Dist: tabulate
 Requires-Dist: plotly>=5.5.0 Requires-Dist: requests Requires-Dist: pydot
-Requires-Dist: tqdm Requires-Dist: polars<=0.20.2,>=0.20.0 Requires-Dist:
-pyarrow Requires-Dist: pyyaml Requires-Dist: aioboto3>=11.0 Provides-Extra:
-docs Requires-Dist: sphinx; extra == "docs" Requires-Dist: furo; extra ==
-"docs" Requires-Dist: sphinx-autoapi; extra == "docs" Requires-Dist: nbsphinx;
-extra == "docs" Requires-Dist: sphinx-copybutton; extra == "docs" Requires-
-Dist: myst-parser; extra == "docs" Provides-Extra: app Requires-Dist:
+Requires-Dist: tqdm Requires-Dist: polars~=0.20.0 Requires-Dist: pyarrow
+Requires-Dist: pyyaml Requires-Dist: aioboto3>=11.0 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs" Requires-Dist: furo; extra == "docs"
+Requires-Dist: sphinx-autoapi; extra == "docs" Requires-Dist: nbsphinx; extra
+== "docs" Requires-Dist: sphinx-copybutton; extra == "docs" Requires-Dist:
+myst-parser; extra == "docs" Provides-Extra: app Requires-Dist:
 streamlit>=1.23; extra == "app" Requires-Dist: quarto; extra == "app" Requires-
 Dist: papermill; extra == "app" Requires-Dist: itables; extra == "app"
 Requires-Dist: jinja2>=3.1; extra == "app" Requires-Dist: xlsxwriter>=3.0;
 extra == "app" Requires-Dist: tabulate; extra == "app"
 ************ PPeeggaa DDaattaa SScciieennttiisstt TToooollss ************
                                   [Pega logo]
  _[_P_y_t_h_o_n_ _t_e_s_t_s_]_[_R_ _t_e_s_t_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_p_e_g_a_s_y_s_t_e_m_s_/_p_e_g_a_-_d_a_t_a_s_c_i_e_n_t_i_s_t_-
```

### Comparing `pdstools-3.4.1/pdstools.egg-info/SOURCES.txt` & `pdstools-3.4.3/pdstools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 python/pdstools/pega_io/API.py
 python/pdstools/pega_io/File.py
 python/pdstools/pega_io/S3.py
 python/pdstools/pega_io/__init__.py
 python/pdstools/plots/__init__.py
 python/pdstools/plots/plot_base.py
 python/pdstools/plots/plots_plotly.py
+python/pdstools/prediction/Prediction.py
+python/pdstools/prediction/__init__.py
 python/pdstools/reports/HealthCheck.qmd
 python/pdstools/reports/ModelReport.qmd
 python/pdstools/reports/__init__.py
 python/pdstools/utils/__init__.py
 python/pdstools/utils/cdh_utils.py
 python/pdstools/utils/datasets.py
 python/pdstools/utils/errors.py
```

### Comparing `pdstools-3.4.1/pyproject.toml` & `pdstools-3.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/__init__.py` & `pdstools-3.4.3/python/pdstools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Python pdstools"""
 
-__version__ = "3.4.1"
+__version__ = "3.4.3"
 
 from polars import enable_string_cache
 
 enable_string_cache()
 
 import sys
 from pathlib import Path
 
 from .adm.ADMDatamart import ADMDatamart
 from .adm.ADMTrees import ADMTrees, MultiTrees
 from .adm.BinAggregator import BinAggregator
 from .pega_io import get_token, readDSExport
 from .pega_io import File, API, S3
 from .pega_io.API import setupAzureOpenAI
+from .prediction import Prediction
 from .utils import cdh_utils, datasets, errors, hds_utils
 from .utils.cdh_utils import defaultPredictorCategorization
 from .utils.show_versions import show_versions
 from .utils.datasets import CDHSample, SampleTrees, SampleValueFinder
 from .utils.hds_utils import Config, DataAnonymization
 from .utils.table_definitions import PegaDefaultTables
 from .valuefinder.ValueFinder import ValueFinder
```

### Comparing `pdstools-3.4.1/python/pdstools/adm/ADMDatamart.py` & `pdstools-3.4.3/python/pdstools/adm/ADMDatamart.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 import os
 import shutil
 import subprocess
 from io import BytesIO
 from pathlib import Path
 from typing import Any, Dict, List, Literal, NoReturn, Optional, Tuple, Union
+from collections import namedtuple
 
 import polars as pl
 import yaml
 import glob
 
 from ..plots.plot_base import Plots
 from ..plots.plots_plotly import ADMVisualisations as plotly_plot
@@ -99,31 +100,88 @@
                 predictor_filename = "Data-Decision-ADM-PredictorBinningSnapshot_PredictorBinningSnapshotRepo20201110T084825_GMT/data.json")
     >>> Data =  ADMDatamart("Data/files",
                 model_filename = "ModelData.csv",
                 predictor_filename = "PredictorData.csv")
 
     """
 
+    standardChannelGroups = [
+        "Web",
+        "Mobile",
+        "E-mail",
+        "Push",
+        "SMS",
+        "Retail",
+        "Call Center",
+        "IVR",
+    ]
+    standardDirections = ["Inbound", "Outbound"]
+
+    NBAD_configurations = namedtuple( 
+        "Configurations",
+        ["model_name", "channel", "direction", "standard", "multi_channel"],
+    ) 
+    standardNBADModelConfigurationList:List[NBAD_configurations] = [
+        ("Web_Click_Through_Rate", "Web", "Inbound", True, False),
+        ("WebTreatmentClickModel", "Web", "Inbound", True, False),
+        ("Mobile_Click_Through_Rate", "Mobile", "Inbound", True, False),
+        ("Email_Click_Through_Rate", "E-mail", "Outbound", True, False),
+        ("Push_Click_Through_Rate", "Push", "Outbound", True, False),
+        ("SMS_Click_Through_Rate", "SMS", "Outbound", True, False),
+        ("Retail_Click_Through_Rate", "Retail", "Inbound", True, False),
+        ("Retail_Click_Through_Rate_Outbound", "Retail", "Outbound", True, False),
+        ("CallCenter_Click_Through_Rate", "Call Center", "Inbound", True, False),
+        ("CallCenterAcceptRateOutbound", "Call Center", "Outbound", True, False),
+        (
+            "Assisted_Click_Through_Rate",
+            "Assisted",
+            "Inbound",
+            True,
+            False,
+        ),  # withdrawn record
+        (
+            "Assisted_Click_Through_Rate_Outbound",
+            "Assisted",
+            "Outbound",
+            True,
+            False,
+        ),  # withdrawn record
+        ("Default_Inbound_Model", "Default", "Inbound", True, False),
+        ("Default_Outbound_Model", "Default", "Outbound", True, False),
+        ("Default_Click_Through_Rate", "Other", "Inbound", True, False),
+        ("Other_Inbound_Click_Through_Rate", "Other", "Inbound", True, False),
+        ("OmniAdaptiveModel", "Multi-channel", "Multi-channel", True, True),
+    ]
+
+    NBAD_model_configurations = [
+        x[0].upper() for x in standardNBADModelConfigurationList
+    ]
+
     def __init__(
         self,
         path: Union[str, Path] = Path("."),
         import_strategy: Literal["eager", "lazy"] = "eager",
         *,
         model_filename: Optional[str] = "modelData",
         predictor_filename: Optional[str] = "predictorData",
         model_df: Optional[any_frame] = None,
         predictor_df: Optional[any_frame] = None,
         query: Optional[Union[pl.Expr, List[pl.Expr], str, Dict[str, list]]] = None,
         subset: bool = True,
         drop_cols: Optional[list] = None,
         include_cols: Optional[list] = None,
-        context_keys: list = ["Channel", "Direction", "Issue", "Group"],
+        context_keys: list = [
+            "Channel",
+            "Direction",
+            "Issue",
+            "Group",
+        ],  # TODO Name/Treatment are normally also part of context
         extract_keys: bool = False,  # TODO: should be True by default, extract should be efficiently using Configuration
         predictorCategorization: pl.Expr = cdh_utils.defaultPredictorCategorization,
-        plotting_engine: Union[str, Any] = "plotly",
+        plotting_engine: Union[str, Any] = "plotly", # TODO drop this, no plot engine abstraction
         verbose: bool = False,
         **reading_opts,
     ):
         self.import_strategy = import_strategy
         self.context_keys = context_keys
         self.verbose = verbose
         self.query = query
@@ -306,14 +364,18 @@
                     "Please check if they are available in the data,\n",
                     "and supply a custom mapping if the naming is different from default.\n",
                     f"Missing values: {total_missing}",
                 )
 
         return df1, df2
 
+    @property
+    def is_available(self) -> bool:
+        return len(self.modelData.head(1).collect()) > 0
+
     def _import_utils(
         self,
         name: Union[str, any_frame],
         path: Optional[str] = None,
         *,
         subset: bool = True,
         extract_keys: bool = False,
@@ -1022,29 +1084,23 @@
             by = by[0]
         if self.import_strategy == "lazy" and not allow_collect:
             raise NotEagerError("Pivot df.")
 
         df = df.filter(pl.col("PredictorName") != "Classifier").with_columns(
             pl.col("PerformanceBin").fill_nan(0.5),
         )
-        if top_n > 0:
-            top_n_xaxis = (
-                df.unique(subset=[by], keep="first")
-                .group_by(by)
+        if by not in ["ModelID", "Name"]:
+            df = (
+                df.unique(subset=[by] + ["PredictorName"], keep="first")
+                .group_by([by, "PredictorName"])
                 .agg(
-                    cdh_utils.weighted_average_polars("PerformanceBin", "ResponseCount")
+                    cdh_utils.weighted_average_polars(
+                        "PerformanceBin", "ResponseCountBin"
+                    )
                 )
-                .sort("PerformanceBin", descending=True)
-                .head(top_n)
-                .select(by)
-            )
-            df = top_n_xaxis.join(df, on=by, how="left")
-        if by not in ["ModelID", "Name"]:
-            df = df.group_by([by, "PredictorName"]).agg(
-                cdh_utils.weighted_average_polars("PerformanceBin", "ResponseCount")
             )
         df = (
             df.collect()
             .pivot(
                 index=by,
                 columns="PredictorName",
                 values="PerformanceBin",
@@ -1257,14 +1313,306 @@
                 .otherwise(pl.col(key))
                 .alias(key)
                 for key in self.context_keys
             ]
         )
         return self.processTables()
 
+    def summary_by_channel(self, custom_channels: Dict[str, str] = None, keep_lists: bool=False):
+        if not custom_channels:
+            custom_channels = {}
+
+        # Removes whitespace and capitalizes names for matching
+        def name_normalizer(x):
+            return pl.col(x).str.replace_all("[ \-_]", "").str.to_uppercase()
+
+        directionMapping = pl.DataFrame(
+            # Standard directions have a 1:1 mapping to channel groups
+            {
+                "Direction": self.standardDirections,
+                "DirectionGroup": self.standardDirections,
+            }
+        ).with_columns(normalizedDirection=name_normalizer("Direction"))
+
+        channelGroupMapping = (
+            pl.concat(
+                [
+                    pl.DataFrame(
+                        # Standard channels have a 1:1 mapping to channel groups
+                        {
+                            "Channel": self.standardChannelGroups,
+                            "ChannelGroup": self.standardChannelGroups,
+                        }
+                    ),
+                    pl.DataFrame(
+                        # feels like a convoluted way to put a dict into a polars dataframe
+                        # but that is just what this does in the end
+                        {
+                            "Channel": custom_channels.keys(),
+                            "ChannelGroup": [
+                                custom_channels[c] for c in custom_channels.keys()
+                            ],
+                        }
+                    ),
+                ],
+                how="diagonal",
+            )
+            .with_columns(normalizedChannel=name_normalizer("Channel"))
+            .unique()
+            .sort(["ChannelGroup", "Channel"])
+        )
+
+        actionIdentifierExpr = pl.concat_str(["Issue", "Group", "Name"], separator="/")
+        activeActionExpr = (pl.col("ResponseCount").sum() > 0).over(
+            ["Issue", "Group", "Name"]
+        )
+
+        # all these expressions needed because not every customer has Treatments and
+        # polars can't aggregate literals, so we have to be careful to pass on explicit
+        # values when there are no treatments
+        treatmentIdentifierExpr = (
+            pl.concat_str(["Issue", "Group", "Name", "Treatment"], separator="/")
+            if "Treatment" in self.modelData.columns
+            else pl.lit("")
+        )
+        activeTreatmentExpr = (
+            (
+                (pl.col("ResponseCount").sum() > 0)
+                & (pl.col("Treatment").is_not_null())
+            ).over(["Issue", "Group", "Name", "Treatment"])
+            if "Treatment" in self.modelData.columns
+            else pl.lit(False)
+        )
+        uniqueTreatmentExpr = (
+            treatmentIdentifierExpr.unique()
+            if "Treatment" in self.modelData.columns
+            else pl.lit([])
+        )
+        uniqueTreatmentCountExpr = (
+            treatmentIdentifierExpr.n_unique()
+            if "Treatment" in self.modelData.columns
+            else pl.lit(0)
+        )
+        uniqueUsedTreatmentExpr = (
+            treatmentIdentifierExpr.where(pl.col("isUsedTreatment")).unique()
+            if "Treatment" in self.modelData.columns
+            else pl.lit([])
+        )
+        uniqueUsedTreatmentCountExpr = (
+            treatmentIdentifierExpr.where(pl.col("isUsedTreatment")).n_unique()
+            if "Treatment" in self.modelData.columns
+            else pl.lit(0)
+        )
+
+        return (
+            self.modelData.with_columns(
+                activeActionExpr.alias("isUsedAction"),
+                activeTreatmentExpr.alias("isUsedTreatment"),
+            )
+            # .filter(
+            #     pl.col("Configuration").cast(pl.Utf8).str.to_uppercase()
+            #     # TODO maybe not here...
+            #     != "OMNIADAPTIVEMODEL"
+            # )
+            # .with_columns(
+            #     OriginalChannelDirection=pl.concat_str(
+            #         ["Channel", "Direction"], separator="/"
+            #     )
+            # )
+            .with_columns(
+                normalizedChannel=name_normalizer("Channel"),
+                normalizedDirection=name_normalizer("Direction"),
+            )
+            .join(
+                channelGroupMapping.lazy(),
+                on="normalizedChannel",
+                how="left",
+                # suffix="_standard",
+            )
+            .join(
+                directionMapping.lazy(),
+                on="normalizedDirection",
+                how="left",
+                # suffix="_standard",
+            )
+            .with_columns(
+                ChannelDirectionGroup=pl.when(
+                    pl.col("ChannelGroup").is_not_null()
+                    & pl.col("DirectionGroup").is_not_null()
+                )
+                .then(pl.concat_str(["ChannelGroup", "DirectionGroup"], separator="/"))
+                .otherwise(pl.lit("Other")),
+            )
+            .group_by(
+                [
+                    "Channel",
+                    "Direction",
+                    "ChannelDirectionGroup",
+                ]
+            )
+            .agg(
+                pl.col("SnapshotTime").min().cast(pl.Date).alias("DateRange Min"),
+                pl.col("SnapshotTime").max().cast(pl.Date).alias("DateRange Max"),
+                # pl.col("OriginalChannelDirection"),
+                pl.col("Positives").sum(),
+                pl.col("ResponseCount").sum(),
+                (cdh_utils.weighted_performance_polars() * 100).alias("Performance"),
+                pl.col("Configuration").cast(pl.Utf8),
+                pl.col("Configuration")
+                .cast(pl.Utf8)
+                .str.to_uppercase()
+                .is_in(self.NBAD_model_configurations)
+                .alias("isNBADModelConfiguration"),
+                actionIdentifierExpr.n_unique().alias("Total Number of Actions"),
+                uniqueTreatmentCountExpr.alias("Total Number of Treatments"),
+                # TODO use last update property instead
+                (actionIdentifierExpr.where(pl.col("isUsedAction")).n_unique()).alias(
+                    "Used Actions"
+                ),
+                uniqueUsedTreatmentCountExpr.alias("Used Treatments"),
+                # keep lists of unique values for aggregation over channels
+                AllIssues=pl.col("Issue").unique(),
+                AllGroups=pl.concat_str(["Issue", "Group"], separator="/").unique(),
+                AllActions=actionIdentifierExpr.unique(),
+                AllTreatments=uniqueTreatmentExpr,
+                AllUsedActions=actionIdentifierExpr.where(
+                    pl.col("isUsedAction")
+                ).unique(),
+                AllUsedTreatments=uniqueUsedTreatmentExpr,
+            )
+            .with_columns(
+                pl.when(pl.col("Used Actions").is_not_null())
+                .then(pl.col("Used Actions"))
+                .otherwise(pl.lit(0))
+                .alias("Used Actions"),
+                pl.when(pl.col("Used Treatments").is_not_null())
+                .then(pl.col("Used Treatments"))
+                .otherwise(pl.lit(0))
+                .alias("Used Treatments"),
+                ChannelDirection=pl.format(
+                    "{}/{}",
+                    pl.when(pl.col("Channel").is_not_null())
+                    .then(pl.col("Channel"))
+                    .otherwise(pl.lit("Empty")),
+                    pl.when(pl.col("Direction").is_not_null())
+                    .then(pl.col("Direction"))
+                    .otherwise(pl.lit("Empty")),
+                ),
+                isValid=(pl.col("Positives") > 200) & (pl.col("ResponseCount") > 1000),
+                Configuration=pl.col("Configuration")
+                .list.unique()
+                .list.sort()
+                .list.join(", "),
+                Issues=pl.col("AllIssues").list.len(),
+                Groups=pl.col("AllGroups").list.len(),
+                # TODO: NBAD detection is not entirely correct: if the only standard model is omniadaptive, we
+                # miss it, because that one got filtered out early on
+                usesNBAD=pl.col("isNBADModelConfiguration").list.any(),
+                usesNBADOnly=pl.col("isNBADModelConfiguration").list.any()
+                & pl.col("isNBADModelConfiguration").list.all(),
+            )
+            .with_columns(CTR=(pl.col("Positives")) / (pl.col("ResponseCount")))
+            .drop(
+                ["isNBADModelConfiguration"]
+                + (
+                    []
+                    if keep_lists
+                    else [
+                        "AllIssues",
+                        "AllGroups",
+                        "AllActions",
+                        "AllUsedActions",
+                        "AllTreatments",
+                        "AllUsedTreatments",
+                    ]
+                )
+            )
+            .sort(
+                [
+                    "ChannelDirectionGroup",
+                ]
+            )
+        )
+
+    def overall_summary(self, custom_channels: Dict[str, str] = None):
+        totalTreatments = (
+            pl.col("AllTreatments").list.explode().n_unique()
+            if "Treatment" in self.modelData.columns
+            else pl.lit(0)
+        )
+        totalUsedTreatments = (
+            pl.col("AllUsedTreatments").list.explode().n_unique()
+            if "Treatment" in self.modelData.columns
+            else pl.lit(0)
+        )
+
+        # Re-calculating here because the use of NBAD in the channel
+        # summary does not currently take into account the omni adaptive model
+        usesNBAD = (
+            self.modelData.select(
+                pl.col("Configuration")
+                .cast(pl.Utf8)
+                .str.to_uppercase()
+                .is_in(self.NBAD_model_configurations)
+                .any()
+            )
+            .collect()
+            .item()
+        )
+
+        usesNBADOnly = (
+            self.modelData.select(
+                pl.col("Configuration")
+                .cast(pl.Utf8)
+                .str.to_uppercase()
+                .is_in(self.NBAD_model_configurations)
+                .all()
+            )
+            .collect()
+            .item()
+        )
+
+        return (
+            self.summary_by_channel(custom_channels, keep_lists=True)
+            .filter(pl.col("isValid"))
+            .select(
+                pl.col("DateRange Min").min(),
+                pl.col("DateRange Max").max(),
+                pl.count().alias("Number of Valid Channels"),
+                cdh_utils.weighted_performance_polars().alias("Performance"),
+                pl.col("Positives").sum(),
+                pl.col("ResponseCount").sum(),
+                pl.col("Performance")
+                .where((pl.col("Performance") == pl.col("Performance").min()))
+                .first()
+                .alias("Minimum Performance"),
+                pl.col("ChannelDirection")
+                .where((pl.col("Performance") == pl.col("Performance").min()))
+                .first()
+                .alias("Channel with Minimum Performance"),
+                pl.col("AllIssues").list.explode().n_unique().alias("Issues"),
+                pl.col("AllGroups").list.explode().n_unique().alias("Groups"),
+                pl.col("AllActions")
+                .list.explode()
+                .n_unique()
+                .alias("Total Number of Actions"),
+                totalTreatments.alias("Total Number of Treatments"),
+                pl.col("AllUsedActions")
+                .list.explode()
+                .n_unique()
+                .alias("Used Actions"),
+                totalUsedTreatments.alias("Used Treatments"),
+                usesNBAD=pl.lit(usesNBAD),
+                usesNBADOnly=(pl.count() > 0) & pl.lit(usesNBAD and usesNBADOnly),
+            )
+            .with_columns(CTR=(pl.col("Positives")) / (pl.col("ResponseCount")))
+        )
+
+
+
     def generateReport(
         self,
         name: Optional[str] = None,
         working_dir: Path = Path("."),
         *,
         modelid: Optional[str] = "",
         delete_temp_files: bool = True,
```

### Comparing `pdstools-3.4.1/python/pdstools/adm/ADMTrees.py` & `pdstools-3.4.3/python/pdstools/adm/ADMTrees.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/adm/BinAggregator.py` & `pdstools-3.4.3/python/pdstools/adm/BinAggregator.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/adm/Tables.py` & `pdstools-3.4.3/python/pdstools/adm/Tables.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/app/Home.py` & `pdstools-3.4.3/python/pdstools/app/Home.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/app/cli.py` & `pdstools-3.4.3/python/pdstools/app/cli.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/app/pages/1-Data Import.py` & `pdstools-3.4.3/python/pdstools/app/pages/1-Data Import.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/app/pages/2-Data Filters.py` & `pdstools-3.4.3/python/pdstools/app/pages/2-Data Filters.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/app/pages/3-Reports.py` & `pdstools-3.4.3/python/pdstools/app/pages/3-Reports.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/ih/IHAnalysis.py` & `pdstools-3.4.3/python/pdstools/ih/IHAnalysis.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/ih/legacy_IH.py` & `pdstools-3.4.3/python/pdstools/ih/legacy_IH.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/pega_io/API.py` & `pdstools-3.4.3/python/pdstools/pega_io/API.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/pega_io/File.py` & `pdstools-3.4.3/python/pdstools/pega_io/File.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/pega_io/S3.py` & `pdstools-3.4.3/python/pdstools/pega_io/S3.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/plots/plot_base.py` & `pdstools-3.4.3/python/pdstools/plots/plot_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from typing import Optional, Union, Dict, List, Any
+from typing import Any, Dict, List, Optional, Union
+
+import plotly.express as px
+import plotly.graph_objs as go
+
 # from datetime import datetime
 import polars as pl
-from .plots_plotly import ADMVisualisations as plotly
-from ..utils.cdh_utils import (
-    weighted_performance_polars,
-    weighted_average_polars,
-    lift
-)
+from plotly.graph_objects import Figure
+
+from ..utils.cdh_utils import lift, weighted_average_polars, weighted_performance_polars
 from ..utils.errors import NotApplicableError
 from ..utils.types import any_frame
-import plotly.graph_objs as go
-import plotly.express as px
-from plotly.graph_objects import Figure
+from .plots_plotly import ADMVisualisations as plotly
 
 
 class Plots:
     """
     Base plotting class
 
     Attributes
@@ -1139,29 +1138,38 @@
         -------
         go.FigureWidget
         """
         plotting_engine = self.get_engine(
             kwargs.get("plotting_engine", self.plotting_engine)
         )()
         table = "combinedData"
-        required_columns = {"PredictorName", "Name", "PerformanceBin"}
+        required_columns = {
+            "PredictorName",
+            "Name",
+            "PerformanceBin",
+            "Performance",
+            "ResponseCountBin",
+        }
         if by is not None:
             required_columns = required_columns.union(
                 set([col for col in by.split("/")] + ["ResponseCount"])
             )
         df, facets = self._subset_data(
             table,
             required_columns,
             query,
             active_only=active_only,
             facets=facets,
             last=True,
         )
 
         df, facet_col = self._generateFacets(df, by)
+        df = df.filter(pl.col("ResponseCount") > 0)
+        if df.collect().shape[0] == 0:
+            raise ValueError("Models do not have any responses")
         df = self.pivot_df(df, by=facet_col, top_n=top_n)
         df = df.with_columns(pl.all().exclude(facet_col) * 100)
 
         if kwargs.pop("return_df", False):
             return df
 
         if kwargs.get("separate", False):
```

### Comparing `pdstools-3.4.1/python/pdstools/plots/plots_plotly.py` & `pdstools-3.4.3/python/pdstools/plots/plots_plotly.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         fig.update_layout(
             template="none", title=title, xaxis_title="Range", yaxis_title="Responses"
         )
         fig.update_yaxes(title_text="Propensity", secondary_y=True)
         fig.layout.yaxis2.tickformat = ",.3%"
         fig.layout.yaxis2.zeroline = False
         fig.update_yaxes(showgrid=False)
-        fig.update_xaxes(type='category')
+        fig.update_xaxes(type="category")
 
         return fig
 
     @staticmethod
     def post_plot(
         fig,
         name,
@@ -382,19 +382,15 @@
         px.Figure
         """
         title_suffix = (
             f"{kwargs.get('facet_val','over all models')}"
             if facet is None
             else f"per {facet}"
         )
-        title_prefix = (
-            "Predictor Importance"
-            if to_plot == "FeatureImportance"
-            else f"Predictor {to_plot}"
-        )
+        title_prefix = "Predictor Importance" if to_plot == "FeatureImportance" else ""
         df = df.to_pandas(use_pyarrow_extension_array=True)
         if order:
             df[y] = df[y].astype("category")
             df[y] = df[y].cat.set_categories(order)
         fig = px.box(
             df.sort_values([y]),
             x=to_plot,
```

### Comparing `pdstools-3.4.1/python/pdstools/reports/HealthCheck.qmd` & `pdstools-3.4.3/python/pdstools/reports/HealthCheck.qmd`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 title: "ADM Health Check"
 title-block-banner: true
-author: "Pega data scientist tools"
+author: "Pega Data Scientist tools"
 date: today
 subtitle: > 
   Summary of all ADM Models
 format:
   html:
     code-fold: true
     embed-resources: true
@@ -44,45 +44,51 @@
 import pandas as pd
 import numpy as np
 from pdstools.utils import pega_template
 import math
 
 # Convenience wrapper functions
 
-
 def quarto_print(text):
     display(Markdown(text))
 
-
 def quarto_callout_info(info):
     quarto_print(
         """
 ::: {.callout-note}
 %s
 :::
 """
         % info
     )
 
-
 def quarto_callout_important(info):
     quarto_print(
         """
 ::: {.callout-important}
 %s
 :::
 """
         % info
     )
 
-
 def quarto_callout_no_predictor_data_warning(extra=""):
     quarto_callout_important(f"Predictor Data is not available. {extra}")
 
 
+def update_fig_facet_height(fig, n_cols = 2, base_height = 250, step_height = 270):
+    n_rows = math.ceil(len(fig.layout.annotations) / n_cols)
+    height = base_height + (n_rows * step_height)
+    return (
+        fig
+        .for_each_annotation(lambda a: a.update(text=a.text.split("=")[1])) 
+        .update_layout(autosize=True, height=height)
+    )
+
+
 ```
 
 ```{python}
 # | tags: [parameters]
 # | echo: false
 
 # The kwargs argument is in support of the streamlit app specifically.
@@ -102,25 +108,29 @@
 predictorfilename = ""
 
 tables_max_rows = 200  # max number of rows for embedded tables
 barchart_max_bars = 20  # max number of bars showing in bar charts
 responsecount_analysis_threshold = (
     100  # min number of responses for response count analysis
 )
+predictor_analysis_threshold = (
+    200  # min number of responses for predictor analysis
+)
+channel_responses_threshold = 10000
 
 # globalQuery = None # TODO not used?
 ```
 
 ```{python}
 # | echo: false
 
 responsecount_analysis_query = (
     pl.col("ResponseCount") > responsecount_analysis_threshold
 )
-predictor_analysis_query = pl.col("ResponseCount") > 200
+predictor_analysis_query = pl.col("ResponseCount") > predictor_analysis_threshold
 ```
 
 ```{python}
 # | echo: false
 
 quarto_print(
     f"""
@@ -137,87 +147,92 @@
 ```{python}
 # | tags: [initialization]
 # | code-fold: true
 # | code-summary: Initialization of the datamart class.
 
 # Initialize the class after the parameters have been overwritten.
 
+def reset_datamart(dm):
+    global datamart
+    global last_data
+    global datamart_all_columns
+    datamart = dm
+    last_data = (
+        dm.last(strategy="lazy")
+        .with_columns(pl.col(pl.Categorical).cast(pl.Utf8))
+        .with_columns(
+            [
+                pl.col(pl.Utf8).fill_null("NA"),
+                pl.col(pl.Null).fill_null("NA"),
+                pl.col("SuccessRate").fill_nan(0).fill_null(0),
+                pl.col("Performance").fill_nan(0).fill_null(0),
+                pl.col("ResponseCount").fill_null(0),
+                (pl.concat_str("Channel/Direction".split("/"), separator="/")).alias(
+                    "Channel/Direction"
+                ),
+            ]
+        )
+    ).collect()
+    if dm.predictorData is not None:
+        datamart_all_columns = dm.combinedData.columns
+    else:
+        datamart_all_columns = dm.modelData.columns
+
 if len(kwargs) > 0:
     # Calling through function (in streamlit or in a notebook)
-    datamart = ADMDatamart(**kwargs, include_cols="pyFeatureImportance").fillMissing()
+    reset_datamart(ADMDatamart(**kwargs, include_cols="pyFeatureImportance").fillMissing())
 elif len(datafolder) > 0 or len(modelfilename) > 0 or len(predictorfilename) > 0:
     # Run through this qmd file
-    datamart = ADMDatamart(
+    reset_datamart(ADMDatamart(
         path="." if len(datafolder) == 0 else datafolder,
         model_filename="" if len(modelfilename) == 0 else modelfilename,
         predictor_filename="" if len(predictorfilename) == 0 else predictorfilename,
         extract_keys=True,
         include_cols="pyFeatureImportance",
-    ).fillMissing()
+    ).fillMissing())
 else:
     # fall back to sample data
-    datamart = datasets.CDHSample()
-
-last_data = (
-    datamart.last(strategy="lazy")
-    .with_columns(pl.col(pl.Categorical).cast(pl.Utf8))
-    .with_columns(
-        [
-            pl.col(pl.Utf8).fill_null("NA"),
-            pl.col(pl.Null).fill_null("NA"),
-            pl.col("SuccessRate").fill_nan(0).fill_null(0),
-            pl.col("Performance").fill_nan(0).fill_null(0),
-            pl.col("ResponseCount").fill_null(0),
-            (pl.concat_str("Channel/Direction".split("/"), separator="/")).alias(
-                "Channel/Direction"
-            ),
-        ]
-    )
-).collect()
-
-if datamart.predictorData is not None:
-    datamart_all_columns = datamart.combinedData.columns
-else:
-    datamart_all_columns = datamart.modelData.columns
-
+    reset_datamart(datasets.CDHSample())
 
 def columnExists(df, col):
     return col in df.columns and df.schema[col] != pl.Null
 
-
 def subsetToExistingColumns(cols):
     return [col for col in cols if col in datamart_all_columns]
 
-
-standardNBADNames = [
-    "Assisted_Click_Through_Rate",
-    "CallCenter_Click_Through_Rate",
-    "CallCenterAcceptRateOutbound",
-    "Default_Inbound_Model",
-    "Default_Outbound_Model",
-    "Email_Click_Through_Rate",
-    "Mobile_Click_Through_Rate",
-    "OmniAdaptiveModel",
-    "Other_Inbound_Click_Through_Rate",
-    "Push_Click_Through_Rate",
-    "Retail_Click_Through_Rate",
-    "Retail_Click_Through_Rate_Outbound",
-    "SMS_Click_Through_Rate",
-    "Web_Click_Through_Rate",
-]
+standardNBADNames = {
+            "Web_Click_Through_Rate": "Web",
+            "WebTreatmentClickModel": "Web",
+            "Mobile_Click_Through_Rate": "Mobile",
+            "Email_Click_Through_Rate": "E-mail",
+            "Push_Click_Through_Rate": "Push",
+            "SMS_Click_Through_Rate": "SMS",
+            "Retail_Click_Through_Rate": "Retail",
+            "Retail_Click_Through_Rate_Outbound": "Retail",
+            "CallCenter_Click_Through_Rate": "Call Center",
+            "CallCenterAcceptRateOutbound": "Call Center",
+            "Assisted_Click_Through_Rate": "Assisted",  # withdrawn record
+            "Assisted_Click_Through_Rate_Outbound": "Assisted",  # withdrawn record
+            "Default_Inbound_Model": "Inbound (default)",
+            "Default_Outbound_Model": "Outbound (default)",
+            "Default_Click_Through_Rate": "Inbound (other)",
+            "Other_Inbound_Click_Through_Rate": "Inbound (other)",
+            "OmniAdaptiveModel": "Multi-channel",
+        }
 
 currentConfigurationNames = (
     datamart.modelData.select(pl.col("Configuration"))
     .unique()
     .collect()
     .to_series(0)
     .to_list()
 )
+
 configurationNamesInStandardNBADModelNames = [
-    (c in standardNBADNames) for c in currentConfigurationNames
+    (c in standardNBADNames.keys()) for c in currentConfigurationNames
 ]
 ```
 
 This document gives a global overview of the Adaptive models and predictors. It is generated from a Python markdown file in the [Pega Data Scientist Tools](https://github.com/pegasystems/pega-datascientist-tools). This is open-source software and comes without guarantees. Off-line reports for individual
 models can be created as well, see [Wiki](https://github.com/pegasystems/pega-datascientist-tools/wiki).
 
 We provide guidance and best practices where possible. However these are  generic practices and may or may not be applicable to the specific use case and situation of the implementation. The recommendations are strongly geared towards the CDH use cases and may not apply to, for example, Process AI.
@@ -328,54 +343,99 @@
     )
     .sort(subsetToExistingColumns(["Channel", "Direction"]))
     .collect()
 )
 
 # TODO precision 0 is okay EXCEPT for the avg groups per issue, one decimal would be preferable, figure out the subset argument of format to do this
 
+def highlight_response_counts(v):
+    if v == 0:
+        color = "orangered"
+    elif v < 200:
+        color = "orange"
+    else:
+        color = ""
+    return "background-color: %s" % color
+
+def highlight_too_many_configurations(v):
+    if len(v) > 2:
+        color = "orangered"
+    else:
+        color = ""
+    return "background-color: %s" % color
+
+def highlight_context_not_defined(v):
+    if v == "ContextNotDefinedError":
+        color = "orangered"
+    else:
+        color = ""
+    return "background-color: %s" % color
+
 display(
-    channel_overview.to_pandas()
-    .style.set_caption("Channel Overview")
+    channel_overview
+    .to_pandas().style
+    .set_caption("Channel Overview")
     .hide(axis="index")
-    .format(precision=0)
-    # check positives and responses > 200, number of configurations <= 2
-    # TODO there are simpler ways to check the range
-    .apply(
-        lambda x: [
-            "background-color: orange" if (i >= 2 and i <= 3 and (v < 200)) else ""
-            for i, v in enumerate(x)
-        ],
-        axis=1,
+    # .format(precision=0, na_rep="") # errors out with some value error sometimes, prob related to the list of configurations
+    .format(
+        {
+            "Responses": "{:.3g}",
+            "Positives": "{:.3g}"
+        }
     )
-    .apply(
-        lambda x: [
-            "background-color: orangered" if (i >= 2 and i <= 3 and (v == 0)) else ""
-            for i, v in enumerate(x)
-        ],
-        axis=1,
-    )
-    .apply(
-        lambda x: [
-            "background-color: orange" if (i == 5 and len(v) > 2) else ""
-            for i, v in enumerate(x)
-        ],
-        axis=1,
+    .applymap(highlight_context_not_defined, subset=["Channel", "Direction"])
+    .applymap(highlight_response_counts, subset=["Responses", "Positives"])
+    .applymap(highlight_too_many_configurations, subset=["Supported by Configurations"])
+)
+```
+
+## Exclude unused Channels
+
+```{python}
+quarto_print(
+    f"""
+If there are any channels that have fewer than {channel_responses_threshold} responses in total or no positives at all, these will be excluded. However if no channels would be left, we don't do that.
+"""
+)
+
+all_channels = channel_overview.select(["Channel", "Direction"]).unique()
+
+unused_channels = (
+    channel_overview.filter(
+        (pl.col("Responses") < channel_responses_threshold) | (pl.col("Positives") == 0)
     )
+    .select(["Channel", "Direction", "Responses", "Positives"])
+    .unique()
 )
 
+if (unused_channels.shape[0] > 0) & (unused_channels.shape[0] != all_channels.shape[0]):
+    quarto_print(
+        """
+In the detailed analyses after the overviews, the following channels will be excluded:
+    """
+    )
 
+    display(
+        unused_channels.sort(["Channel", "Direction"])
+        .to_pandas()
+        .style.hide(axis="index")
+        .format(precision=0, na_rep="")
+    )
 ```
 
 
+
 # Overview of the Actions
 
 In a standard setup, the offers/conversations are presented as treatments for actions in a hierarchical structure setup in NBA Designer. Treatments are often channel specific and typically there are more unique treatments than there are actions.
 
 Adaptive Models are created per treatment (at least in the default setup) and the recommendation is to stick the default context keys of the models.
 
+The recommended Service and data health limits for Pega Customer Decision Hub on Pega Cloud are published in https://docs.pega.com/bundle/customer-decision-hub-241/page/customer-decision-hub/cdh-portal/cloud-service-health-limits.html.
+
 ```{python}
 def nUniqueValues(fld):
     if not isinstance(fld, list):
         fld = [fld]
     fld = subsetToExistingColumns(fld)
     if len(fld) == 0:
         return 0
@@ -437,22 +497,23 @@
         .to_series()
         .unique()
         .sort()
         .to_list()[:n]
     )
 
 
+# pd yuk, todo make pl
 df = pd.DataFrame(
     {
         "Item": [
             "Overall Number of Actions",
             "Max number of Actions within an Issue and Group",
             "Number of Treatments across all Actions",
             "Max number of Treatments per Channel",
-            "Max number of Treatments for any single Action",
+            "Max number of Treatments per Channel for any single Action",
             "Number of unique Issues",
             "Average number of Groups per Issue",
             "Max number of Groups per Issue",
             "Channels",
         ],
         "Number": [
             nUniqueValues("Name"),
@@ -472,21 +533,21 @@
             "-",
             "-",
             sampleValues("Issue"),
             sampleValues("Group"),
             "-",
             sampleValues(["Channel", "Direction"]),
         ],
-        "Best Practice": [1000, 100, 2500, 1000, 5, 5, 0, 5, 0],
+        "Best Practice": [1000, 100, 2500, 1000, 3, 5, 0, 5, 0],
         "Cloud Service Limit": [
             2500,
             250,
             5000,
             2500,
-            5,
+            10,
             25,
             float("inf"),
             25,
             float("inf"),
         ],
     }
 )
@@ -511,51 +572,45 @@
             else ""
             for i, v in enumerate(x)
         ],
         axis=0,
         subset=["Number"],
     )
 )
-#
-#
-#
-#
-#
-#
-#
-#
-#
-#
-#
-#
-#
-#
-#
-#
-#
-#
-#
-#
-#
-# | echo: false
+```
 
+
+```{python}
+if (unused_channels.shape[0] > 0) & (unused_channels.shape[0] != all_channels.shape[0]):
+    reset_datamart(
+        ADMDatamart(
+            model_df=datamart.modelData.join(
+                unused_channels.lazy(), on=["Channel", "Direction"], how="anti"
+            ),
+            predictor_df=datamart.predictorData,
+        )
+    )
+```
+
+```{python}
 quarto_print(
     f"""
 Just showing the top {barchart_max_bars} here and limiting to the propositions that have received at least {responsecount_analysis_threshold} responses (the rates reported by the models are unreliable otherwise).
 """
 )
 ```
 
 
 ::: {.callout-tip title="Guidance"}
 - Look out for actions that stand out, having a far higher success rate than the rest. Check with business if that is expected.
 
 - Variation in the set of offers across customers is also an important metric but not one that can be derived from the Adaptive Model data - this requires analysis of the actual interactions.
 :::
 
+
 ```{python}
 facet = "Channel/Direction"
 hover_columns = subsetToExistingColumns(["Issue", "Group", "Name", "Treatment"])
 
 df = (
     last_data.lazy()
     .with_columns(pl.concat_str(facet.split("/"), separator="/").alias(facet))
@@ -579,53 +634,41 @@
 hover_data = {
     "SuccessRate": ":.3%",
 }
 for col in hover_columns:
     hover_data[col] = ":.d"
 
 facet = "Channel/Direction"
-facet_col_wrap = 3
+facet_cols = 3
 fig = px.bar(
     df,
     x="SuccessRate",
     y="ModelID",
     color="SuccessRate",
     facet_col=facet,
-    facet_col_wrap=facet_col_wrap,
+    facet_col_wrap=facet_cols,
     template="pega",
     text="Label",
     title=(
         "Success Rates per Channel<br><sup>%s</sup>"
         % "/".join(subsetToExistingColumns(["Name", "Treatment"]))
     ),
     hover_data=hover_data,
 )
 
-# TODO: This counting of number of facets is generic, make common
-unique_count = (
-    last_data.lazy()
-    .with_columns(pl.concat_str(facet.split("/"), separator="/").alias(facet))
-    .select(facet)
-    .collect()
-    .to_series()
-    .n_unique()
-)
-height = 200 + (math.ceil(unique_count / facet_col_wrap) * 250)
+fig = update_fig_facet_height(fig, facet_cols, 200, 250) # 200/250
 
 fig = (
-    fig.update_xaxes(tickformat=",.2%", tickangle=45, title="", matches=None)
+    fig
+    .update_xaxes(tickformat=",.2%", tickangle=45, title="", matches=None)
     .update_yaxes(
         matches=None, showticklabels=False, visible=False, autorange="reversed"
     )
     .update_traces(textposition="inside")
-    .for_each_annotation(
-        lambda a: a.update(text=a.text.replace("Channel/Direction=", ""))
-    )
     .update(layout_coloraxis_showscale=False)
-    .update_layout(autosize=True, height=height)
 )
 
 display(fig)
 ```
 
 ## All Success Rates
 
@@ -655,54 +698,40 @@
 Showing how the overall channel success rates evolved over the time that the data export covers. Split by Channel and model configuration. Usually there are separate model configurations for different channels but sometimes there are also additional model configurations for different outcomes (e.g. conversion) or different customers (e.g. anonymous).
 
 ::: {.callout-tip title="Guidance"}
 - There shouldn’t be too sudden changes over time
 :::
 
 ```{python}
-facet = "Configuration"
-facet_col_wrap = 2
-
-# TODO check the color scheme used - pds tools to supply color schemes for channel dimension, for predictor categorization, etc etc
-# TODO: the faceting errors out when there are many configurations
-
-fig = datamart.plotOverTime(
-    "SuccessRate",
-    by="Channel/Direction",
-    # TODO this function does not have a proper title argument
-    facets=facet,
-    facet_col_wrap=facet_col_wrap,
-    query=responsecount_analysis_query,
-)
-
-# TODO this counting of # facets and determining the height can be shared
-unique_count = (
-    datamart.modelData.with_columns(
-        pl.concat_str(facet.split("/"), separator="/").alias(facet)
+facets = "Configuration"
+unique_count = datamart.modelData.select(pl.concat_str(facets.split("/"), separator="/").n_unique()).collect().item()
+# TODO: the faceting errors out when there are many configurations and too few facet columns resulting in very small facet rows
+facet_cols = max(2, int(unique_count**0.5))
+
+try:
+    fig = datamart.plotOverTime(
+        "SuccessRate",
+        by="Channel/Direction",
+        # TODO this function does not have a proper title argument
+        facets=facets,
+        facet_col_wrap=facet_cols,
+        query=responsecount_analysis_query,
     )
-    .select(facet)
-    .collect()
-    .unique()
-    .shape[0]
-)
-height = 200 + (math.ceil(unique_count / facet_col_wrap) * 250)
-
-fig = (
-    fig.update_yaxes(matches=None, title="", showticklabels=True)
-    .update_xaxes(showticklabels=True, title="")
-    .update_layout(autosize=True, height=height)
-    .for_each_annotation(lambda a: a.update(text=a.text.replace(f"{facet}=", "")))
-)
 
-# TODO title stuff doesnt need to be here if std plot supports it properly
-fig.update_layout(
-    title=f"Trend of Success Rates per Channel<br><sup>Query: {responsecount_analysis_query}</sup>"
-)
+    fig = update_fig_facet_height(fig, facet_cols, 200, 250)
+    fig = (
+        fig.update_yaxes(matches=None, title="", showticklabels=True)
+        .update_xaxes(showticklabels=True, title="")
+        # TODO title stuff doesnt need to be here if std plot supports it properly
+        .update_layout(title=f"Trend of Success Rates per Channel<br><sup>Query: {responsecount_analysis_query}</sup>")
+    )
 
-fig.show()
+    fig.show()
+except ValueError as e:
+    print(f"Error {str(e)}\nPossibly too many facets: {unique_count} for {facet_cols} columns.")
 ```
 
 # Overview of Adaptive Models
 
 ```{python}
 n_unique_models = len(last_data.select("ModelID").unique())  # TODO or uniqueN ?
 
@@ -720,42 +749,125 @@
 if columnExists(last_data, "Treatment"):
     action_dim_agg += [pl.col("Treatment").n_unique().alias("Number of Treatments")]
 
 model_overview = (
     last_data.group_by(
         ["Configuration"] + subsetToExistingColumns(["Channel", "Direction"])
     )
-    .agg(action_dim_agg + [pl.col("ModelID").n_unique().alias("Number of Models")])
+    .agg(
+        action_dim_agg + 
+        [
+            pl.col("ModelID").n_unique().alias("Number of Models"),
+            pl.max("ResponseCount").alias("Responses"),
+            pl.max("Positives")
+        ]
+    )
     .with_columns(
         [
             pl.col("Configuration")
-            .is_in(standardNBADNames)
+            .is_in(standardNBADNames.keys())
             .alias("Standard in NBAD Framework"),
             (pl.col("Number of Models") / pl.col("Number of Actions"))
             .round(2)
             .alias("Average number of Models per Action"),
         ]
     )
     .sort(["Configuration", "Channel", "Direction"])
 )
 
-# TODO apply background styling like in the R version
+def highlight_non_standard_channels(v):
+    if v not in set(standardNBADNames.values()):
+        color = "orange"
+    else:
+        color = ""
+    return "background-color: %s" % color
+
+def highlight_non_standard_configurations(v):
+    if v not in set(standardNBADNames.keys()):
+        color = "orange"
+    else:
+        color = ""
+    return "background-color: %s" % color
+
 display(
     model_overview.head(tables_max_rows)
     .to_pandas(use_pyarrow_extension_array=True)
     .style.set_caption("Model Overview")
     .hide(axis="index")
-    .format(precision=2)
+    .format(
+        {
+            "Responses": "{:.3g}",
+            "Positives": "{:.3g}"
+        },
+        precision=2)
+    .applymap(highlight_non_standard_channels, subset=["Channel"])
+    .applymap(highlight_non_standard_configurations, subset=["Configuration"])
 )
+```
 
+```{python}
+quarto_print(
+    f"""
+If there are any model configurations that have fewer than {channel_responses_threshold} responses in total or no positives at all, these will be excluded. However if no configurations would be left, we don't do that.
+"""
+)
+
+configuration_overview = (
+    datamart.modelData
+    # first, take max per model ID
+    .group_by("Configuration").agg(
+        pl.max("ResponseCount").alias("Responses"), pl.max("Positives")
+    )
+).collect()
+
+all_configurations = configuration_overview.select(["Configuration"]).unique()
+
+unused_configurations = (
+    configuration_overview.filter(
+        (pl.col("Responses") < channel_responses_threshold) | (pl.col("Positives") == 0)
+    )
+    .select(["Configuration", "Responses", "Positives"])
+    .unique()
+)
+
+if (unused_configurations.shape[0] > 0) & (
+    unused_configurations.shape[0] != all_configurations.shape[0]
+):
+    quarto_print(
+        f"""
+In the detailed analyses after the model overview, the following configurations will be excluded:
+    """
+    )
+
+    display(
+        unused_configurations.sort(["Configuration"])
+        .to_pandas()
+        .style.hide()
+        .format(precision=0, na_rep="")
+    )
+```
+
+```{python}
+if (unused_configurations.shape[0] > 0) and (
+    (unused_configurations.shape[0] != all_configurations.shape[0])
+):
+
+    reset_datamart(
+        ADMDatamart(
+            model_df=datamart.modelData.join(
+                unused_configurations.lazy(), on=["Configuration"], how="anti"
+            ),
+            predictor_df=datamart.predictorData,
+        )
+    )
 ```
 
 ## Model Performance 
 
-### Model Performance vs Action Success Rates (the Bubble Chart)
+### Model Performance vs Action Success Rates (the Bubble Charts)
 
 This “Bubble Chart” - similar to the standard ADM models overview in Pega Prediction Studio - shows the relation between model performance and proposition success rates. The size of the bubbles indicates the number of responses.
 
 ::: {.callout-tip title="Guidance"}
 
 -   Bubbles stacked up against the left-hand vertical axis represent
     actions/treatments for which the models are not predictive. These
@@ -781,36 +893,36 @@
 
 -   For small volumes of good models, see if the engagement rules in the
     Decision Strategy are overly restrictive or reconsider the
     arbitration of the propositions so they get more (or less) exposure.
 :::
 
 ```{python}
-facet_col_wrap = 2
+facet_cols = 2
 facet = "Configuration/Channel/Direction"
 
 fig = datamart.plotPerformanceSuccessRateBubbleChart(
-    facets=facet, facet_col_wrap=facet_col_wrap
+    facets=facet, facet_col_wrap=facet_cols
 )
 
 fig.layout.coloraxis.colorscale = pega_template.success
 
-height = 250 + (math.ceil(len(fig.layout.annotations) / facet_col_wrap) * 270)
+fig = set_fig_xaxis_modelperformance(fig, label="")
+fig = update_fig_facet_height(fig)
 
 fig = (
-    set_fig_xaxis_modelperformance(fig, label="")
-    .update_layout(autosize=True, height=height, title="All ADM Models")
-    .for_each_annotation(lambda a: a.update(text=a.text.replace(f"{facet}=", "")))
-    .update_layout(font=dict(size=10))
-    .for_each_annotation(lambda a: a.update(text="<br> ".join(a.text.split("/", 1))))
-    .update_yaxes(tickformat=",.3%", title="")
-    .update_coloraxes(
-        showscale=False,
-        colorbar_len=1 / math.ceil(len(fig.layout.annotations) / facet_col_wrap),
-    )
+    fig
+    .update_layout(title="All ADM Models", font=dict(size=10))
+    .for_each_annotation(lambda a: a.update(text="<br>".join(a.text.split("/", 1))))
+    .update_yaxes(tickformat=",.2%", title="")
+    .update_coloraxes(showscale=False)
+    # .update_coloraxes(
+    #     showscale=True,
+    #     colorbar_len=1 / math.ceil(len(fig.layout.annotations) / facet_cols),
+    # )
 )
 
 fig.show()
 ```
 
 On the x-axis Model Performance measured in AUC-ROC, on the y-axis the Success Rate of the models (#positives / #responses).
 
@@ -819,42 +931,42 @@
 The trend chart shows how model performance evolves over time. Note that ADM is by default configured to track performance over *all* time. You can configure a window for monitoring but this is not commonly done. In Pega Prediction Studio you can monitor models per month, year etc.
 
 ::: {.callout-tip title="Guidance"}
 - No abrupt changes but gradual upward trend is good
 :::
 
 ```{python}
-facet = "Configuration"
-facet_col_wrap = 3
-fig = datamart.plotOverTime(
-    # TODO: the faceting errors out when there are many configurations
-    "weighted_performance", by="Channel/Direction", facets=facet, facet_col_wrap=facet_col_wrap
-)
+datamart.modelData.select(pl.col("Configuration").n_unique()).collect()
+```
+
 
-# TODO below code is repeated, it just calculates the
-# number of facets
-unique_count = (
-    datamart.modelData.with_columns(
-        pl.concat_str(facet.split("/"), separator="/").alias(facet)
+```{python}
+facets = "Configuration"
+unique_count = datamart.modelData.select(pl.concat_str(facets.split("/"), separator="/").n_unique()).collect().item()
+# TODO: the faceting errors out when there are many configurations and too few facet columns resulting in very small facet rows
+facet_cols = max(2, int(unique_count**0.5))
+
+try:
+    fig = datamart.plotOverTime(
+        "weighted_performance", by="Channel/Direction", 
+        facets=facets, 
+        facet_col_wrap=facet_cols
+    )
+    fig = update_fig_facet_height(fig, facet_cols, 200, 250)
+    fig = (
+        fig.update_layout(title="Trend of Model Performance")
+        .update_yaxes(showticklabels=True, title="")
+        .update_xaxes(title="")
     )
-    .select(facet)
-    .collect()
-    .unique()
-    .shape[0]
-)
-height = 200 + (math.ceil(unique_count / facet_col_wrap) * 250)
 
-fig = (
-    fig.update_layout(autosize=True, height=height, title="Trend of Model Performance")
-    .for_each_annotation(lambda a: a.update(text=a.text.replace(f"{facet}=", "")))
-    .update_yaxes(showticklabels=True, title="")
-    .update_xaxes(title="")
-)
+    fig.show()
+except ValueError as e:
+    print(f"Error {str(e)}\nPossibly too many facets: {unique_count} for {facet_cols} columns.")
+
 
-fig.show()
 ```
 
 ### Model performance of all the actions
 
 Using an interactive treemap to visualize the performance. Red is lower performance, green is higher (better) performance.
 
 It can be interesting to see which issues, groups or channels can be better predicted than others. Identifying categories of items for which the predictions are poor can help to drive the search for better predictors, for example.
@@ -1070,30 +1182,22 @@
 ### Predictor Category performance per Channel/Direction/Issue 
 
 ```{python}
 # | error: true
 
 if datamart.predictorData is not None:
     facets = "Configuration/Channel/Direction"
-    facet_col_wrap = 3
+    facet_cols = 3
     fig = datamart.plotPredictorCategoryPerformance(
-        facets=facets, facet_col_wrap=facet_col_wrap
+        facets=facets, facet_col_wrap=facet_cols
     )
-
+    fig = update_fig_facet_height(fig, facet_cols, 200, 150)
     fig.update_layout(font=dict(size=10))
-    fig.for_each_annotation(lambda a: a.update(text=a.text.replace(f"{facets}=", "")))
-    fig.for_each_annotation(lambda a: a.update(text=" <br> ".join(a.text.split("/"))))
+    fig.for_each_annotation(lambda a: a.update(text="<br>".join(a.text.split("/"))))
 
-    facet_list = []
-    for data in fig.data:
-        facet_list.append(data["yaxis"][1:])
-    facet_count = len(set(facet_list))
-
-    height = 200 + (math.ceil(facet_count / facet_col_wrap) * 250)
-    fig.update_layout(autosize=True, height=height)
     fig.show()
 else:
     quarto_callout_no_predictor_data_warning()
 
 ```
 
 ### Relative Predictor Category importance per Configuration
@@ -1189,22 +1293,18 @@
 - We expect a few dozen active predictors for every model instance
 
 :::
 
 ```{python}
 if datamart.predictorData is not None:
     facets = ["Configuration"]
+    facet_cols = 2
     fig = datamart.plotPredictorCount(facets=facets)
-
-    height = 250 + (math.ceil(len(fig.layout.annotations) / 2) * 270)
-    fig.update_layout(autosize=True, height=height)
+    fig = update_fig_facet_height(fig, facet_cols, 250, 150)
     fig.update_yaxes(categoryorder="array", automargin=True, dtick=1)
-    fig.for_each_annotation(
-        lambda a: a.update(text=a.text.replace(f"{facets[0]}=", ""))
-    )
     fig.show()
 else:
     quarto_callout_no_predictor_data_warning()
 ```
 
 ## Predictor Performance across Actions
 
@@ -1224,14 +1324,15 @@
             fig = datamart.plotPredictorPerformanceHeatmap(
                 top_n=barchart_max_bars,
                 by="/".join(index_cols),
                 query=pl.col("Configuration") == conf,
                 tickangle=45,
             )
             fig.update_layout(
+                # TODO: make this a proper call to some abbreviation function
                 xaxis={
                     "tickmode": "array",
                     "tickvals": fig.data[0]["x"],
                     "ticktext": [
                         "..." + tick[-25:] if len(tick) > 25 else tick
                         for tick in fig.data[0]["x"]
                     ],
@@ -1240,18 +1341,20 @@
                 title=f"Top predictors over {conf}",
             )
 
             fig.update(layout_coloraxis_showscale=False)
 
             fig.show()
 
-        except:
-            # TODO: add error message instead of typing "an error"
-            # should we even handle the exception here?
-            print(f"Plot was not drawn for {conf} because of an error")
+        except ValueError as e:
+            print(f'Plot was not drawn for {conf} because of an error:"{e}"')
+        except Exception as e:
+            print(
+                f'Plot was not drawn for {conf} because of an unexpected error: "{e}"'
+            )
 else:
     quarto_callout_no_predictor_data_warning()
 ```
 
 ## Missing values
 
 If a predictor is low performing: are there too many missing values? This could point to a technical problem
@@ -1268,38 +1371,39 @@
 
     missing = (
         datamart.last(table="combinedData")
         .filter(pl.col("PredictorName") != "Classifier")
         .group_by(gb_cols)
         .agg(
             pl.col("BinResponseCount")
-            .where(pl.col("BinSymbol") == "MISSING")
+            .filter(pl.col("BinSymbol") == "MISSING")
             .sum()
             .alias("MissingCount"),
-            pl.sum("BinResponseCount").alias("BinResponseCount"),
+            pl.sum("BinResponseCount").alias("PredictorResponseCount"),
         )
         .with_columns(
-            (pl.col("MissingCount") / pl.col("BinResponseCount")).alias(
+            (pl.col("MissingCount") / pl.col("PredictorResponseCount")).alias(
                 "Percentage without responses"
             )
         )
         .filter((~pl.col("Percentage without responses").is_nan()))
     )
 
     hover_data = {
         "Percentage without responses": ":.2%",
+        "PredictorResponseCount": ":d"
     }
 
     fig = px.treemap(
         missing.to_pandas(),
         path=path,
         color="Percentage without responses",
         template="pega",
         hover_data=hover_data,
-        title="Missing Data in Adaptive Models",
+        title="Predictor Missing Data",
     )
 
     fig.layout.coloraxis.colorscale = pega_template.positive_negative
     fig.update_coloraxes(showscale=False)
 
     fig.show()
 else:
@@ -1491,69 +1595,64 @@
             (pl.col("Positives") == 0).sum().alias("Models w/o Positives"),
             (pl.col("ResponseCount") == 0).sum().alias("Empty Models"),
             # (pl.col("ResponseCount")!=0).sum().alias("Number of non-empty Models")
         ]
     )
     .sort(["Channel", "Direction", "SnapshotTime"], descending=True)
 )
-facet_col_wrap = 3
+facet_cols = 3
 facet = "Channel/Direction"
 df = df.with_columns(
     pl.concat_str(facet.split("/"), separator="/").alias(facet)
 ).with_columns(pl.col(facet).cast(pl.Utf8).fill_null("NA"))
 df_pd = df.collect().to_pandas()
 y = df_pd.iloc[:, len(by) :].columns.tolist()  # slice `df.columns` to get this easily
 fig = px.line(
     df_pd,
     x="SnapshotTime",
     y=y,
     facet_col=facet,
     title="Immature and Empty Models over Time",
     template="pega",
-    facet_col_wrap=facet_col_wrap,
+    facet_col_wrap=facet_cols,
     color_discrete_sequence=px.colors.sequential.Turbo,
 )
-fig.for_each_annotation(lambda a: a.update(text=a.text.replace(f"{facet}=", "")))
 fig.for_each_xaxis(lambda xaxis: xaxis.update(title=""))
 fig.update_layout(legend_title_text="Model Maturity")
-
-unique_count = len(fig.layout["annotations"])
-height = 200 + (math.ceil(unique_count / facet_col_wrap) * 250)
-fig.update_layout(autosize=True, height=height, yaxis_title="Number of Models")
+fig = update_fig_facet_height(fig, facet_cols, 200, 250)
+fig.update_layout(yaxis_title="Number of Models")
 
 fig.show()
 ```
 
 ## Number of Responses over time 
 
 
 ```{python}
-# TODO: make this daily so not continuously rising
-
 facets = "Configuration"
-facet_col_wrap = 3
-# TODO: the faceting errors out when there are many configurations
-response_counts = datamart.plotOverTime(
-    "ResponseCount",
-    by="Channel/Direction",
-    facets=facets,
-    facet_col_wrap=facet_col_wrap,
-    mode="Cumulative",
-)
-
-unique_count = datamart.modelData.select(facets).unique().collect().shape[0]
-height = 200 + (math.ceil(unique_count / facet_col_wrap) * 250)
-response_counts.update_layout(autosize=True, height=height)
-response_counts.for_each_annotation(
-    lambda a: a.update(text=a.text.replace(f"{facets}=", ""))
-)
-response_counts.for_each_xaxis(lambda xaxis: xaxis.update(title=""))
-response_counts.update_layout(yaxis_title="Response Count")
+unique_count = datamart.modelData.select(pl.concat_str(facets.split("/"), separator="/").n_unique()).collect().item()
+# TODO: the faceting errors out when there are many configurations and too few facet columns resulting in very small facet rows
+facet_cols = max(2, int(unique_count**0.5))
+
+try:
+    response_counts = datamart.plotOverTime(
+        "ResponseCount",
+        by="Channel/Direction",
+        facets=facets,
+        facet_col_wrap=facet_cols,
+        mode="Cumulative",
+    )
 
-response_counts.show()
+    response_counts = update_fig_facet_height(response_counts, facet_cols, 200, 250)
+    response_counts.for_each_xaxis(lambda xaxis: xaxis.update(title=""))
+    response_counts.update_layout(yaxis_title="Response Count")
+
+    response_counts.show()
+except ValueError as e:
+    print(f"Error {str(e)}\nPossibly too many facets: {unique_count} for {facet_cols} columns.")
 ```
 
 # Which Models drive most of the Volume
 
 ## Analysis of skewness of the Responses
 Showing the cumulative response count vs the number of models. Is there a larger percentage of models that take the vast majority of the responses?
 
@@ -1798,15 +1897,15 @@
     text=facet,
     hover_data=hover_data,
 )
 
 fig = (
     fig.update_yaxes(matches=None, showticklabels=False, visible=False)
     .update_traces(textposition="inside")
-    .for_each_annotation(lambda a: a.update(text=a.text.replace(facet, "")))
+    # .for_each_annotation(lambda a: a.update(text=a.text.replace(facet, "")))
     .update_layout(yaxis={"categoryorder": "total ascending"}, xaxis_title="Responses")
 )
 
 cdh_utils.legend_color_order(fig).show()  # ?
 ```
 
 ## Models with largest number of positive responses. 
@@ -1837,15 +1936,15 @@
     hover_data=hover_data,
 )
 
 fig = (
     fig.update_yaxes(matches=None, showticklabels=False, visible=False)
     .update_xaxes(matches=None)
     .update_traces(textposition="inside")
-    .for_each_annotation(lambda a: a.update(text=a.text.replace(facet, "")))
+    # .for_each_annotation(lambda a: a.update(text=a.text.replace(facet, "")))
     .update_layout(yaxis={"categoryorder": "total ascending"}, xaxis_title="Positives")
 )
 
 cdh_utils.legend_color_order(fig).show()  # ?
 ```
 
 ## Analysis of Performance vs Volume
@@ -1924,23 +2023,70 @@
 Ideally, all models have received plenty of responses which will make them “mature” and makes sure they are as predictive as possible.
 
 Often we see that there is a significant percentage of models that are still relatively new and have not received much feedback (yet). Below graph shows the percentages of models that have fewer than 200 positives.
 
 Having many on the left-hand side (with very low or perhaps no positives) may or not be a problem. The models may still be there in the datamart but might represent actions/treatments that are not active. 
 
 ```{python}
+# TODO this seems to be very large/expensive for some Data
+# not sure why exactly but we've seen 
+# PanicException: polars' maximum length reached. Consider installing 'polars-u64-idx'.: TryFromIntError(())
 fig = datamart.plotModelsByPositives()
 
 fig.update_layout(
     title="Positives vs Number of Models",
     xaxis_title="Number of Positives",
     yaxis_title="Percentage of Models",
 )
 
-fig = cdh_utils.legend_color_order(fig)
+# TODO remove this override and use cdhutils function again
+# when we've bumped up the pdstools version
+def legend_color_order(fig):
+    """Orders legend colors alphabetically in order to provide pega color
+    consistency among different categories"""
+
+    colorway = [
+        "#001F5F",  # dark blue
+        "#10A5AC",
+        "#F76923",  # orange
+        "#661D34",  # wine
+        "#86CAC6",  # mint
+        "#005154",  # forest
+        "#86CAC6",  # mint
+        "#5F67B9",  # violet
+        "#FFC836",  # yellow
+        "#E63690",  # pink
+        "#AC1361",  # berry
+        "#63666F",  # dark grey
+        "#A7A9B4",  # medium grey
+        "#D0D1DB",  # light grey
+    ]
+    colors = []
+    for trace in fig.data:
+        if trace.legendgroup is not None:
+            colors.append(trace.legendgroup)
+    colors.sort()
+
+    # https://github.com/pegasystems/pega-datascientist-tools/issues/201
+    if len(colors) >= len(colorway):
+        return fig
+
+    indexed_colors = {k: v for v, k in enumerate(colors)}
+    for trace in fig.data:
+        if trace.legendgroup is not None:
+            try:
+                trace.marker.color = colorway[indexed_colors[trace.legendgroup]]
+                trace.line.color = colorway[indexed_colors[trace.legendgroup]]
+            except AttributeError:  # pragma: no cover
+                pass
+
+    return fig
+
+# fig = cdh_utils.legend_color_order(fig)
+fig = legend_color_order(fig)
 
 fig.show()
 ```
 
 # Propensity Analysis
 
 The distribution of propensities returned by the models is yet a different angle.
@@ -1961,85 +2107,88 @@
 
 So when one of the graphs shows more volume on the left, that is to be interpreted as relative to the other graphs.
 
 ```{python}
 # | error: true
 
 # TODO: fix this. Also looks like a lot of code.
+if datamart.predictorData is not None:
+    to_plot = "Propensity"
+    if to_plot == "Propensity" and to_plot not in datamart.predictorData.columns:
+        to_plot = "BinPropensity"
+    df = (
+        datamart.combinedData.filter(pl.col("PredictorName") != "Classifier")
+        .group_by([to_plot, "Channel", "Direction"])
+        .agg(pl.sum("BinResponseCount"))
+        .with_columns(pl.col(to_plot).round(4).cast(pl.Float64))
+        .collect()
+    )
+    color_col = "Channel"
+    smallest_bin = 0
 
-to_plot = "Propensity"
-if to_plot == "Propensity" and to_plot not in datamart.predictorData.columns:
-    to_plot = "BinPropensity"
-df = (
-    datamart.combinedData.filter(pl.col("PredictorName") != "Classifier")
-    .group_by([to_plot, "Channel", "Direction"])
-    .agg(pl.sum("BinResponseCount"))
-    .with_columns(pl.col(to_plot).round(4).cast(pl.Float64))
-    .collect()
-)
-color_col = "Channel"
-smallest_bin = 0
-
-for color in df.get_column(color_col).unique().to_list():
-    color_df = df.filter(pl.col(color_col) == color)
-    propensity_list = list(
-        set(
-            color_df.select(to_plot)
-            .fill_null(0)
-            .fill_nan(0)
-            .filter(pl.col(to_plot) > 0)
-            .get_column(to_plot)
-            .to_list()
-        )
-    )
-    if len(propensity_list) > 0:
-        if np.percentile(propensity_list, 10) > smallest_bin:
-            smallest_bin = np.percentile(propensity_list, 10)
-            cut_off_value = np.percentile(
-                propensity_list, [percentile for percentile in range(0, 101, 5)]
+    for color in df.get_column(color_col).unique().to_list():
+        color_df = df.filter(pl.col(color_col) == color)
+        propensity_list = list(
+            set(
+                color_df.select(to_plot)
+                .fill_null(0)
+                .fill_nan(0)
+                .filter(pl.col(to_plot) > 0)
+                .get_column(to_plot)
+                .to_list()
             )
+        )
+        if len(propensity_list) > 0:
+            if np.percentile(propensity_list, 10) > smallest_bin:
+                smallest_bin = np.percentile(propensity_list, 10)
+                cut_off_value = np.percentile(
+                    propensity_list, [percentile for percentile in range(0, 101, 5)]
+                )
 
-df_pl = df.with_columns(
-    pl.col(to_plot)
-    .fill_null(0)
-    .fill_nan(0)
-    .cut(breaks=cut_off_value)
-    .alias(f"{to_plot}_range")
-)
+    df_pl = df.with_columns(
+        pl.col(to_plot)
+        .fill_null(0)
+        .fill_nan(0)
+        .cut(breaks=cut_off_value)
+        .alias(f"{to_plot}_range")
+    )
 
-grouped = df_pl.group_by(["Channel", f"{to_plot}_range"]).agg(
-    pl.sum("BinResponseCount"), pl.min(to_plot).alias("break_label")
-)
+    grouped = df_pl.group_by(["Channel", f"{to_plot}_range"]).agg(
+        pl.sum("BinResponseCount"), pl.min(to_plot).alias("break_label")
+    )
 
-out = (
-    grouped.sort(["Channel", "break_label"])
-    .select(
-        [
-            "Channel",
-            f"{to_plot}_range",
-            "break_label",
-            "BinResponseCount",
-            pl.col("BinResponseCount").sum().over("Channel").alias("sum"),
-        ]
+    out = (
+        grouped.sort(["Channel", "break_label"])
+        .select(
+            [
+                "Channel",
+                f"{to_plot}_range",
+                "break_label",
+                "BinResponseCount",
+                pl.col("BinResponseCount").sum().over("Channel").alias("sum"),
+            ]
+        )
+        .with_columns([(pl.col("BinResponseCount") / pl.col("sum")).alias("Responses")])
     )
-    .with_columns([(pl.col("BinResponseCount") / pl.col("sum")).alias("Responses")])
-)
 
-out = out.sort(["Channel", "break_label"])
-fig = px.bar(
-    out,
-    x=f"{to_plot}_range",
-    y="Responses",
-    color=color_col,
-    template="pega",
-    barmode="overlay",
-)
-fig.update_yaxes(tickformat=",.0%")
+    out = out.sort(["Channel", "break_label"])
+    fig = px.bar(
+        out,
+        x=f"{to_plot}_range",
+        y="Responses",
+        color=color_col,
+        template="pega",
+        barmode="overlay",
+    )
+    fig.update_yaxes(tickformat=",.0%")
 
-fig.show()
+    fig.show()
+else:
+    quarto_callout_no_predictor_data_warning()
+    
 ```
 
 ## Propensity Thresholding
 
 TODO: Implement like in the R version
 
 # Credits
```

### Comparing `pdstools-3.4.1/python/pdstools/reports/ModelReport.qmd` & `pdstools-3.4.3/python/pdstools/reports/ModelReport.qmd`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 title: "ADM Standalone Model Report"
 title-block-banner: true
-author: "Pega data scientist tools"
+author: "Pega Data Scientist tools"
 date: today
 subtitle: > 
   Details of one ADM model instance
 execute:
   echo: false
 format:
   html:
```

### Comparing `pdstools-3.4.1/python/pdstools/utils/cdh_utils.py` & `pdstools-3.4.3/python/pdstools/utils/cdh_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from .errors import NotEagerError
 from .table_definitions import PegaDefaultTables
 
 import pytz
 
 
 def defaultPredictorCategorization(
-    x: Union[str, pl.Expr] = pl.col("PredictorName")
+    x: Union[str, pl.Expr] = pl.col("PredictorName"),
 ) -> pl.Expr:
     """Function to determine the 'category' of a predictor.
 
     It is possible to supply a custom function.
     This function can accept an optional column as input
     And as output should be a Polars expression.
     The most straight-forward way to implement this is with
@@ -590,15 +590,18 @@
 def weighted_average_polars(
     vals: Union[str, pl.Expr], weights: Union[str, pl.Expr]
 ) -> pl.Expr:
     if isinstance(vals, str):
         vals = pl.col(vals)
     if isinstance(weights, str):
         weights = pl.col(weights)
-    return ((vals * weights).sum()) / weights.sum()
+
+    return (
+        (vals * weights).filter(vals.is_not_nan() & weights.is_not_null()).sum()
+    ) / weights.sum()
 
 
 def weighted_performance_polars() -> pl.Expr:
     """Polars function to return a weighted performance"""
     return weighted_average_polars("Performance", "ResponseCount")
 
 
@@ -669,17 +672,15 @@
     """
 
     def liftImpl(binPos, binNeg, totalPos, totalNeg):
         return (
             # TODO not sure how polars (mis)behaves when there are no positives at all
             # I would hope for a NaN but base python doesn't do that. Polars perhaps.
             # Stijn: It does have proper None value support, may work like you say
-            binPos
-            * (totalPos + totalNeg)
-            / ((binPos + binNeg) * totalPos)
+            binPos * (totalPos + totalNeg) / ((binPos + binNeg) * totalPos)
         ).alias("Lift")
 
     return liftImpl(posCol, negCol, posCol.sum(), negCol.sum())
 
 
 def LogOdds(
     Positives=pl.col("Positives"),
@@ -807,14 +808,19 @@
         "#D0D1DB",  # light grey
     ]
     colors = []
     for trace in fig.data:
         if trace.legendgroup is not None:
             colors.append(trace.legendgroup)
     colors.sort()
+
+    # https://github.com/pegasystems/pega-datascientist-tools/issues/201
+    if len(colors) >= len(colorway):
+        return fig
+
     indexed_colors = {k: v for v, k in enumerate(colors)}
     for trace in fig.data:
         if trace.legendgroup is not None:
             try:
                 trace.marker.color = colorway[indexed_colors[trace.legendgroup]]
                 trace.line.color = colorway[indexed_colors[trace.legendgroup]]
             except AttributeError:  # pragma: no cover
```

### Comparing `pdstools-3.4.1/python/pdstools/utils/datasets.py` & `pdstools-3.4.3/python/pdstools/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/utils/hds_utils.py` & `pdstools-3.4.3/python/pdstools/utils/hds_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/utils/hds_utils_experimental.py` & `pdstools-3.4.3/python/pdstools/utils/hds_utils_experimental.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/utils/pega_template.py` & `pdstools-3.4.3/python/pdstools/utils/pega_template.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/utils/polars_ext.py` & `pdstools-3.4.3/python/pdstools/utils/polars_ext.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/utils/show_versions.py` & `pdstools-3.4.3/python/pdstools/utils/show_versions.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/utils/streamlit_utils.py` & `pdstools-3.4.3/python/pdstools/utils/streamlit_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/utils/table_definitions.py` & `pdstools-3.4.3/python/pdstools/utils/table_definitions.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.4.1/python/pdstools/valuefinder/ValueFinder.py` & `pdstools-3.4.3/python/pdstools/valuefinder/ValueFinder.py`

 * *Files identical despite different names*


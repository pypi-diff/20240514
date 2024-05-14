# Comparing `tmp/silvimetric-1.1.1.tar.gz` & `tmp/silvimetric-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silvimetric-1.1.1.tar", last modified: Tue Apr 23 19:22:39 2024, max compression
+gzip compressed data, was "silvimetric-1.2.0.tar", last modified: Tue May 14 16:41:29 2024, max compression
```

## Comparing `silvimetric-1.1.1.tar` & `silvimetric-1.2.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:39.104859 silvimetric-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-23 19:22:24.000000 silvimetric-1.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-23 19:22:39.104859 silvimetric-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-23 19:22:24.000000 silvimetric-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-23 19:22:24.000000 silvimetric-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:22:39.104859 silvimetric-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:39.096859 silvimetric-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:39.100859 silvimetric-1.1.1/src/silvimetric/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:39.100859 silvimetric-1.1.1/src/silvimetric/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10000 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/cli/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:39.100859 silvimetric-1.1.1/src/silvimetric/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/commands/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/commands/initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/commands/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/commands/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/commands/shatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:39.104859 silvimetric-1.1.1/src/silvimetric/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/extents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/names.py
--rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:39.104859 silvimetric-1.1.1/src/silvimetric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-23 19:22:39.000000 silvimetric-1.1.1/src/silvimetric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-23 19:22:39.000000 silvimetric-1.1.1/src/silvimetric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:22:39.000000 silvimetric-1.1.1/src/silvimetric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 19:22:39.000000 silvimetric-1.1.1/src/silvimetric.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 19:22:39.000000 silvimetric-1.1.1/src/silvimetric.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:39.104859 silvimetric-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_shatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_western.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:29.466361 silvimetric-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-14 16:41:17.000000 silvimetric-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-14 16:41:29.466361 silvimetric-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-14 16:41:17.000000 silvimetric-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-14 16:41:17.000000 silvimetric-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:41:29.466361 silvimetric-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:29.458361 silvimetric-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:29.458361 silvimetric-1.2.0/src/silvimetric/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:29.462361 silvimetric-1.2.0/src/silvimetric/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/cli/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:29.462361 silvimetric-1.2.0/src/silvimetric/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/commands/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/commands/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/commands/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/commands/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/commands/shatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:29.462361 silvimetric-1.2.0/src/silvimetric/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10157 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/extents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12541 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:29.466361 silvimetric-1.2.0/src/silvimetric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-14 16:41:29.000000 silvimetric-1.2.0/src/silvimetric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-14 16:41:29.000000 silvimetric-1.2.0/src/silvimetric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:41:29.000000 silvimetric-1.2.0/src/silvimetric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 16:41:29.000000 silvimetric-1.2.0/src/silvimetric.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 16:41:29.000000 silvimetric-1.2.0/src/silvimetric.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:29.466361 silvimetric-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_extents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_fusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_shatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_western.py
```

### Comparing `silvimetric-1.1.1/LICENSE.txt` & `silvimetric-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `silvimetric-1.1.1/pyproject.toml` & `silvimetric-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `silvimetric-1.1.1/src/silvimetric/cli/cli.py` & `silvimetric-1.2.0/src/silvimetric/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import click
 from dask.distributed import performance_report
 import pyproj
 import logging
 
 
 from .. import __version__
-from ..resources import Attribute, Metric, Bounds, Log
-from ..resources import StorageConfig, ShatterConfig, ExtractConfig, ApplicationConfig
+from .. import Attribute, Metric, Bounds, Log
+from .. import StorageConfig, ShatterConfig, ExtractConfig, ApplicationConfig
 from ..commands import shatter, extract, scan, info, initialize, manage
 from .common import BoundsParamType, CRSParamType, AttrParamType, MetricParamType
 from .common import dask_handle, close_dask
 
 @click.group()
 @click.option("--database", '-d', type=click.Path(exists=False), help="Database path")
 @click.option("--debug", is_flag=True, default=False, help="Changes logging level from INFO to DEBUG.")
 @click.option("--log-dir", default=None, help="Directory for log output", type=str)
 @click.option("--progress", is_flag=True, default=True, type=bool, help="Report progress")
-@click.option("--workers", type=int, default=12, help="Number of workers for Dask")
+@click.option("--workers", type=int, default=10, help="Number of workers for Dask")
 @click.option("--threads", type=int, default=4, help="Number of threads per worker for Dask")
 @click.option("--watch", is_flag=True, default=False, type=bool,
         help="Open dask diagnostic page in default web browser.")
 @click.option("--dasktype", default='processes', type=click.Choice(['threads',
         'processes']), help="What Dask uses for parallelization. For more"
         "information see here https://docs.dask.org/en/stable/scheduling.html#local-threads")
 @click.option("--scheduler", default='distributed', type=click.Choice(['distributed',
@@ -144,15 +144,15 @@
     """Initialize silvimetrics DATABASE"""
 
     storageconfig = StorageConfig(tdb_dir = app.tdb_dir,
             log = app.log,
             root = bounds,
             crs = crs,
             attrs = attributes,
-            metrics = list(itertools.chain(*metrics)),
+            metrics = metrics,
             resolution = resolution)
     return initialize.initialize(storageconfig)
 
 
 @cli.command('shatter')
 @click.argument("pointcloud", type=str)
 @click.option("--bounds", type=BoundsParamType(), default=None,
@@ -176,29 +176,32 @@
 
     if date is not None and dates is not None:
         app.log.warning("Both 'date' and 'dates' specified. Prioritizing 'dates'")
 
     if date is None and dates is None:
         raise ValueError("One of '--date' or '--dates' must be provided.")
 
-    config = ShatterConfig(tdb_dir = app.tdb_dir,
+    config = ShatterConfig(tdb_dir=app.tdb_dir,
             date=dates if dates else tuple([date]),
-            log = app.log,
-            filename = pointcloud,
-            bounds = bounds,
+            log=app.log,
+            filename=pointcloud,
+            bounds=bounds,
             tile_size=tilesize)
 
     if report:
         if app.scheduler != 'distributed':
+            from dask.diagnostics import ProgressBar
             app.log.warning('Report option is incompatible with scheduler'
                             '{scheduler}, skipping.')
-        report_path = f'reports/{config.name}.html'
-        with performance_report(report_path) as pr:
             shatter.shatter(config)
-        print(f'Writing report to {report_path}.')
+        else:
+            report_path = f'reports/{config.name}.html'
+            with performance_report(report_path) as pr:
+                shatter.shatter(config)
+            print(f'Writing report to {report_path}.')
     else:
         shatter.shatter(config)
 
 
 @cli.command('extract')
 @click.option("--attributes", "-a", multiple=True, type=AttrParamType(), default=[],
         help="List of attributes to include output")
@@ -210,14 +213,16 @@
         help="Output directory.")
 @click.pass_obj
 def extract_cmd(app, attributes, metrics, outdir, bounds):
     """Extract silvimetric metrics from DATABASE """
 
     #TODO only allow metrics and attributes to be added if they're present
     # in the storage config.
+    dask_handle(app.dasktype, app.scheduler, app.workers, app.threads,
+        app.watch, app.log)
 
     config = ExtractConfig(tdb_dir = app.tdb_dir,
             log = app.log,
             out_dir= outdir,
             attrs = attributes,
             metrics = metrics,
             bounds = bounds)
```

### Comparing `silvimetric-1.1.1/src/silvimetric/cli/common.py` & `silvimetric-1.2.0/src/silvimetric/cli/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pyproj
 import webbrowser
 
 import dask
 from dask.diagnostics import ProgressBar
 from dask.distributed import Client, LocalCluster
 
-from ..resources import Bounds, Attribute, Metric, Attributes, Metrics, Log
+from .. import Bounds, Attribute, Metric, Attributes, Metrics, Log
 
 
 class BoundsParamType(click.ParamType):
     name = "Bounds"
 
     def convert(self, value, param, ctx):
         try:
```

### Comparing `silvimetric-1.1.1/src/silvimetric/commands/extract.py` & `silvimetric-1.2.0/src/silvimetric/commands/extract.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+from pathlib import Path
+from itertools import chain
+
+
 from osgeo import gdal, osr
+import dask
 import numpy as np
-from pathlib import Path
 import pandas as pd
-import dask
-import dask.dataframe as dd
 
-from typing import Dict
 
-from ..resources import Storage, ExtractConfig, Metric, Attribute
-from ..resources import Extents
+from .. import Storage, Extents, ExtractConfig
 
 np_to_gdal_types = {
     np.dtype(np.byte).str: gdal.GDT_Byte,
     np.dtype(np.int8).str: gdal.GDT_Int16,
     np.dtype(np.uint16).str: gdal.GDT_UInt16,
     np.dtype(np.int16).str: gdal.GDT_Int16,
     np.dtype(np.uint32).str: gdal.GDT_UInt32,
@@ -20,179 +20,144 @@
     np.dtype(np.uint64).str: gdal.GDT_UInt64,
     np.dtype(np.int64).str: gdal.GDT_Int64,
     np.dtype(np.float32).str: gdal.GDT_Float32,
     np.dtype(np.float64).str: gdal.GDT_Float64
 }
 
 def write_tif(xsize: int, ysize: int, data:np.ndarray, name: str,
-              config: ExtractConfig) -> None:
+        config: ExtractConfig) -> None:
     """
     Write out a raster with GDAL
 
     :param xsize: Length of X plane.
     :param ysize: Length of Y plane.
     :param data: Data to write to raster.
     :param name: Name of raster to write.
     :param config: ExtractConfig.
     """
     osr.UseExceptions()
     path = Path(config.out_dir) / f'{name}.tif'
     crs = config.crs
     srs = osr.SpatialReference()
     srs.ImportFromWkt(crs.to_wkt())
-    # transform = [x, res, 0, y, 0, res]
     b = config.bounds
 
     transform = [b.minx, config.resolution, 0,
-                 b.maxy, 0, -1* config.resolution]
+                 b.maxy, 0, -1*config.resolution]
 
     driver = gdal.GetDriverByName("GTiff")
     gdal_type = np_to_gdal_types[np.dtype(data.dtype).str]
     tif = driver.Create(str(path), int(xsize), int(ysize), 1, gdal_type)
     tif.SetGeoTransform(transform)
     tif.SetProjection(srs.ExportToWkt())
     tif.GetRasterBand(1).WriteArray(data)
-    tif.GetRasterBand(1).SetNoDataValue(np.nan)
+    tif.GetRasterBand(1).SetNoDataValue(-9999)
     tif.FlushCache()
     tif = None
 
-MetricDict = Dict[str, np.ndarray]
-def get_metrics(data_in: MetricDict, config: ExtractConfig) -> MetricDict:
+def get_metrics(data_in: pd.DataFrame, storage: Storage):
     """
     Reruns a metric over this cell. Only called if there is overlapping data.
 
-    :param data_in: Cell data to be rerun.
-    :param config: ExtractConfig.
+    :param data_in: Dataframe to be rerun.
+    :param storage: Base storage object.
     :return: Combined dict of attribute and newly derived metric data.
     """
+
+    #TODO should just use the metric calculation methods from shatter
     if data_in is None:
         return None
 
-    # make sure it's not empty. No empty writes
-    if not np.any(data_in['count']):
-        return None
+    exploded = data_in.agg(lambda x: x.explode())
+    metric_data = dask.persist(*[ m.do(exploded) for m in storage.config.metrics ])
 
-    # doing dask compute inside the dict array because it was too fine-grained
-    # when it was outside
-    #TODO move this operation to a dask bag and convert to dataframe and then
-    # to a dict for better efficiency?
-    metric_data = {
-        f'{m.entry_name(attr.name)}': [m(cell_data) for cell_data in data_in[attr.name]]
-        for attr in config.attrs for m in config.metrics
-    }
-    # md = dask.compute(metric_data)[0]
-    data_out = data_in | metric_data
+    data_out = data_in.set_index(['X','Y']).join([m for m in metric_data])
     return data_out
 
 def handle_overlaps(config: ExtractConfig, storage: Storage, indices: np.ndarray) -> pd.DataFrame:
     """
     Handle cells that have overlapping data. We have to re-run metrics over these
     cells as there's no other accurate way to determined metric values. If there
     are no overlaps, this will do nothing.
 
     :param config: ExtractConfig.
     :param storage: Database storage object.
     :param indices: Indices with overlap.
     :return: Dataframe of rerun data.
     """
 
-    ma_list = [ m.entry_name(a.name) for m in config.metrics for a in
-        config.attrs ]
-    att_list = [ a.name for a in config.attrs ] + [ 'count' ]
-    out_list = [ *ma_list, 'X', 'Y' ]
+    ma_list = storage.getDerivedNames()
+    att_list = [ a.name for a in config.attrs ]
 
     minx = indices['x'].min()
     maxx = indices['x'].max()
     miny = indices['y'].min()
     maxy = indices['y'].max()
 
     att_meta = {}
     att_meta['X'] = np.int32
     att_meta['Y'] = np.int32
     att_meta['count'] = np.int32
     for a in config.attrs:
         att_meta[a.name] =  a.dtype
 
     with storage.open("r") as tdb:
-        data = tdb.query(attrs=ma_list, order='F', coords=True).df[minx:maxx,
-                miny:maxy]
-        data['X'] = data['X'] - data['X'].min()
-        data['Y'] = data['Y'] - data['Y'].min()
-
-        # 1. should find values that are not unique, meaning they have multiple
-        # entries
-        recarray = data.to_records()
-        xys = recarray[['X', 'Y']]
-        unq, idx, counts = np.unique(xys, return_index=True, return_counts=True)
-        redos = np.where(counts >= 2)
-
-        if not np.any(redos):
-            return data
-
-        leaves = data.loc[idx[np.where(counts == 1)]]
-
-        # 2. then should combine the values of those attribute/cell combos
-        ridx = np.unique(unq[redos])
-        rxs = list(ridx['X'])
-        rys = list(ridx['Y'])
-        if np.any(rxs):
-            redo = pd.DataFrame(tdb.query(attrs=att_list).multi_index[[rxs], [rys]])
-            redo['X'] = redo['X'] - minx
-            redo['Y'] = redo['Y'] - miny
-
-        parts = min(int(redo['X'].max() * redo['Y'].max()), 1000)
-        r = dd.from_pandas(redo, npartitions=parts, name='MetricDataFrame')
-        def squash(x):
-            def s2(vals):
-                if vals.dtype == object:
-                    return np.array([*vals], vals.dtype).reshape(-1)
-                elif vals.name == 'X' or vals.name == 'Y':
-                    return vals.values[0]
-                else:
-                    return sum(vals)
-            val = x.aggregate(s2)
-            p = pd.DataFrame(val).T
-            return p
-
-        recs = r.groupby(['X','Y']).apply(squash, meta=att_meta)
-        rs = recs.compute().to_dict(orient='list')
-
-        # 3. Should rerun the metrics over them
-        metrics = get_metrics(rs, config)
-        ms = pd.DataFrame.from_dict(metrics)[out_list]
-        return pd.concat((ms, leaves[out_list]))
+        # TODO this can be more efficient. Use count to find indices, then work
+        # with that smaller set from there. Working as is for now, but slow.
+        dit = tdb.query(attrs=[*att_list, *ma_list], order='F', coords=True,
+                return_incomplete=True, use_arrow=False).df[minx:maxx, miny:maxy]
+        data = pd.DataFrame()
+
+        storage.config.log.info('Collecting database information...')
+        for d in dit:
+            if data.empty:
+                data = d
+            else:
+                data = pd.concat([data, d])
+
+
+        # should find values that are not unique, meaning they have multiple entries
+        data = data.set_index(['X','Y'])
+        redo_indices = data.index[data.index.duplicated(keep='first')]
+        if redo_indices.empty:
+            return data.reset_index()
+
+        # data with overlaps
+        redo_data = data.loc[redo_indices][att_list].groupby(['X','Y']).agg(lambda x: list(chain(*x)))
+        # data that has no overlaps
+        clean_data = data.loc[data.index[~data.index.duplicated(False)]]
+
+        storage.config.log.warning('Overlapping data detected. Rerunning metrics over these cells...')
+        new_metrics = get_metrics(redo_data.reset_index(), storage)
+        return pd.concat([clean_data, new_metrics]).reset_index()
 
 def extract(config: ExtractConfig) -> None:
     """
     Pull data from database for each desired metric and output them to rasters
 
     :param config: ExtractConfig.
     """
 
     dask.config.set({"dataframe.convert-string": False})
 
-    ma_list = [ m.entry_name(a.name) for m in config.metrics for a in
-        config.attrs ]
-
-
     storage = Storage.from_db(config.tdb_dir)
+    ma_list = storage.getDerivedNames()
+    config.log.debug(f'Extracting metrics {[m for m in ma_list]}')
     root_bounds=storage.config.root
 
     e = Extents(config.bounds, config.resolution, root=root_bounds)
     i = e.get_indices()
-    minx = i['x'].min()
-    maxx = i['x'].max()
-    miny = i['y'].min()
-    maxy = i['y'].max()
-    x1 = maxx - minx + 1
-    y1 = maxy - miny + 1
+    xsize = e.x2
+    ysize = e.y2
 
+    # figure out if there are any overlaps and handle them
     final = handle_overlaps(config, storage, i).sort_values(['Y', 'X'])
 
     # output metric data to tifs
     for ma in ma_list:
-        m_data = np.full(shape=(y1,x1), fill_value=np.nan, dtype=final[ma].dtype)
+        # TODO should output in sections so we don't run into memory problems
+        m_data = np.full(shape=(ysize,xsize), fill_value=np.nan, dtype=final[ma].dtype)
         a = final[['X','Y',ma]].to_numpy()
         for x,y,md in a[:]:
             m_data[int(y)][int(x)] = md
 
-        write_tif(x1, y1, m_data, ma, config)
+        write_tif(xsize, ysize, m_data, ma, config)
```

### Comparing `silvimetric-1.1.1/src/silvimetric/commands/info.py` & `silvimetric-1.2.0/src/silvimetric/commands/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 from uuid import UUID
 from typing import Union
 
-from ..resources import Storage, Bounds
+from .. import Storage, Bounds
 
 def check_values(start_time: datetime, end_time: datetime, bounds: Bounds,
         name: Union[UUID, str]):
     """
     Validate arguments for info command.
 
     :param start_time: Starting datetime object.
```

### Comparing `silvimetric-1.1.1/src/silvimetric/commands/manage.py` & `silvimetric-1.2.0/src/silvimetric/commands/manage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..resources import Storage, ShatterConfig
+from .. import Storage, ShatterConfig
 from .info import info
 from .shatter import shatter
 
 def delete(tdb_dir: str, name:str) -> ShatterConfig:
     """
     Delete Shatter process from database and return config for that process.
```

### Comparing `silvimetric-1.1.1/src/silvimetric/commands/scan.py` & `silvimetric-1.2.0/src/silvimetric/commands/scan.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import logging
 import dask.bag as db
 import dask
 import math
+import json
 
-from ..resources import Storage, Data, Extents, Bounds, Log
+from .. import Storage, Data, Extents, Bounds, Log
 
 def scan(tdb_dir: str, pointcloud: str, bounds: Bounds, point_count:int=600000, resolution:float=100,
         depth:int=6, filter:bool=False, log: Log=None):
     """
     Scan pointcloud and determine appropriate tile sizes.
 
     :param tdb_dir: TileDB database directory.
@@ -20,65 +21,50 @@
     :param filter: Remove empty Extents. This takes longer, but is more accurage., defaults to False
     :return: Returns list of point counts.
     """
 
     # TODO Scan should output other information about a file like bounds, pc, avg points per cell
     with Storage.from_db(tdb_dir) as tdb:
 
+
         if log is None:
             logger = logging.getLogger('silvimetric')
         else:
             logger = log
         data = Data(pointcloud, tdb.config, bounds)
 
-        #TODO add this section and print out information on only parts covered
-        # by the storage bounds
-
-        # shared_bounds = Bounds.shared_bounds(data.bounds, tdb.config.root)
-
-        # if shared_bounds != data.bounds:
-        #     logger.warning('Incoming bounds is not fully within the storage'
-        #         f' bounds. Adjusting incoming from {str(data.bounds)} to'
-        #         f' {str(shared_bounds)}')
-        #     extents = Extents.from_sub(tdb_dir, shared_bounds)
-        # else:
+        thresholds = dict(thresholds=dict(resolution=resolution, point_count=point_count, depth=depth))
+        logger.debug(json.dumps(thresholds, indent=2))
 
         extents = Extents.from_sub(tdb_dir, data.bounds)
+        count = dask.delayed(data.estimate_count)(extents.bounds).persist()
+
 
         if filter:
             chunks = extents.chunk(data, resolution, point_count, depth)
             cell_counts = [ch.cell_count for ch in chunks]
 
         else:
             cell_counts = extent_handle(extents, data, resolution, point_count,
                 depth, log)
 
-        count = data.count(extents.bounds)
 
         std = np.std(cell_counts)
         mean = np.mean(cell_counts)
         rec = int(mean + std)
 
+        pc_info = dict(pc_info=dict(storage_bounds=tdb.config.root.to_json(),
+                data_bounds=data.bounds.to_json(), count=dask.compute(count)))
+        tiling_info = dict(tile_info=dict(num_cells=len(cell_counts), mean=mean,
+                std_dev=std, recommended=rec))
 
-        logger.info('Pointcloud information:')
-        logger.info(f'  Storage Bounds: {str(tdb.config.root)}')
-        logger.info(f'  Pointcloud Bounds: {str(data.bounds)}')
-        logger.info(f'  Point Count: {count}')
-
-        logger.debug('Scan thresholds:')
-        logger.debug(f'  Resolution: {resolution}')
-        logger.debug(f'  Point count: {point_count}')
-        logger.debug(f'  Tree depth: {depth}')
-
-        logger.info('Tiling information:')
-        logger.info(f'  Mean tile size: {mean}')
-        logger.info(f'  Std deviation: {std}')
-        logger.info(f'  Recommended split size: {rec}')
+        final_info = pc_info | tiling_info
+        logger.info(json.dumps(final_info, indent=2))
 
-        return rec
+        return final_info
 
 
 def extent_handle(extent: Extents, data: Data, res_threshold:int=100,
         pc_threshold:int=600000, depth_threshold:int=6, log: Log = None) -> list[int]:
     """
     Recurisvely iterate through quad tree of this Extents object with given
     threshold parameters.
```

### Comparing `silvimetric-1.1.1/src/silvimetric/resources/bounds.py` & `silvimetric-1.2.0/src/silvimetric/resources/bounds.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import ast
-from typing import Self
 
+#TODO should these bounds have a buffer?
 class Bounds(dict): #for JSON serializing
     """Simple class to represent a 2 or 3-dimensional bounding box that can be
     generated from both JSON or PDAL bounds form."""
     def __init__(self, minx: float, miny: float, maxx: float, maxy: float):
         self.minx = float(minx)
         """minimum X Plane"""
         self.miny = float(miny)
@@ -22,17 +22,19 @@
                 other.maxy == self.maxy
     def __ne__(self, other):
         return not other.__eq__(self)
 
     def __bool__(self):
         return True
 
+    def __repr__(self) -> str:
+        return str(self.get())
 
     @staticmethod
-    def from_string(bbox_str: str) -> Self:
+    def from_string(bbox_str: str):
         """Create Bounds object from a PDAL bounds string in the form:
 
         "([1,101],[2,102],[3,103])"
         "{\"minx\": 1,\"miny\": 2,\"maxx\": 101,\"maxy\": 102}"
         "[1,2,101,102]"
         "[1,2,3,101,102,103]"
 
@@ -81,18 +83,14 @@
         """Return Bounds as a list of floats
 
         :return: list of floats in form [minx, miny, maxx, maxy]
         """
         return [self.minx, self.miny, self.maxx, self.maxy]
 
 
-    def __repr__(self) -> str:
-        return str(self.get())
-
-
     def to_string(self) -> str:
         """Return string representation of Bounds
 
         :return: string of a list of floats in form [minx, miny, maxx, maxy]
         """
         return self.__repr__()
 
@@ -126,16 +124,31 @@
         """
         if other.minx > self.maxx or other.maxx < self.minx:
             return True
         if other.miny > self.maxy or other.maxy < self.miny:
             return True
         return False
 
+    def adjust_to_cell_lines(self, resolution):
+        xmindif = self.minx % resolution
+        xmaxdif = self.maxx % resolution
+        ymaxdif = self.maxy % resolution
+        ymindif = self.miny % resolution
+
+        if xmindif:
+            self.minx = self.minx - xmindif
+        if xmaxdif:
+            self.maxx = self.maxx + (resolution - xmaxdif)
+        if ymindif:
+            self.miny = self.miny - ymindif
+        if ymaxdif:
+            self.maxy = self.maxy + (resolution - ymaxdif)
+
     @staticmethod
-    def shared_bounds(first: Self, second: Self) -> Self | None:
+    def shared_bounds(first, second):
         """Find the Bounds that is shared between two Bounds.
 
         :param first: First Bounds object for comparison.
         :param second: Second Bounds object for comparison.
         :returns: None if there is no overlap, otherwise the shared Bounds
         """
 
@@ -143,8 +156,8 @@
             return None
 
         minx = max(first.minx, second.minx)
         maxx = min(first.maxx, second.maxx)
         miny = max(first.miny, second.miny)
         maxy = min(first.maxy, second.maxy)
 
-        return Bounds(minx, miny, maxx, maxy)
+        return Bounds(minx, miny, maxx, maxy)
```

### Comparing `silvimetric-1.1.1/src/silvimetric/resources/config.py` & `silvimetric-1.2.0/src/silvimetric/resources/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,18 @@
         for k in keys:
             d[k] = self.__dict__[k]
         if not isinstance(d['log'], dict):
             d['log'] = d['log'].to_json()
         return d
 
     @classmethod
+    def from_json(self, data: str):
+        return self.from_string(json.dumps(data))
+
+    @classmethod
     @abstractmethod
     def from_string(self, data: str):
         raise NotImplementedError
 
     def __repr__(self):
         return json.dumps(self.to_json())
 
@@ -120,21 +124,21 @@
         return d
 
     @classmethod
     def from_string(cls, data: str):
         x = json.loads(data)
         root = Bounds(*x['root'])
         if 'metrics' in x:
-            ms = [ Metric.from_string(m) for m in x['metrics']]
+            ms = [ Metric.from_dict(m) for m in x['metrics']]
         else:
-            ms = None
+            ms = [ ]
         if 'attrs' in x:
-            attrs = [ Attribute.from_string(a) for a in x['attrs']]
+            attrs = [ Attribute.from_dict(a) for a in x['attrs']]
         else:
-            attrs = None
+            attrs = [ ]
         if 'crs' in x:
             crs = pyproj.CRS.from_user_input(json.dumps(x['crs']))
         else:
             crs = None
         n = cls(tdb_dir = x['tdb_dir'],
                 root = root,
                 log = Log(**x['log']),
@@ -144,15 +148,16 @@
                 metrics = ms,
                 capacity = x['capacity'],
                 version = x['version'])
 
         return n
 
     def __repr__(self):
-        return json.dumps(self.to_json())
+        j = self.to_json()
+        return json.dumps(j)
 
 @dataclass
 class ApplicationConfig(Config):
     """ Base application config """
 
     debug: bool = False,
     """Debug mode, defaults to False"""
@@ -229,14 +234,18 @@
     used as the timestamp in tiledb writes to better organize and manage
     processes., defaults to 0"""
 
     def __post_init__(self) -> None:
         from .storage import Storage
         s = Storage.from_db(self.tdb_dir)
 
+        if isinstance(self.tile_size, float):
+            self.tile_size = int(self.tile_size)
+            self.log.warning(f'Truncating tile size to integer({self.tile_size})')
+            pass
         if not self.attrs:
             self.attrs = s.getAttributes()
         if not self.metrics:
             self.metrics = s.getMetrics()
 
         del s
 
@@ -244,15 +253,15 @@
         d = super().to_json()
 
         d['name'] = str(self.name)
         d['time_slot'] = self.time_slot
         d['bounds'] = self.bounds.to_json() if self.bounds is not None else None
         d['attrs'] = [a.to_json() for a in self.attrs]
         d['metrics'] = [m.to_json() for m in self.metrics]
-        d['mbr'] = self.mbr
+        d['mbr'] = list(self.mbr)
 
         if isinstance(self.date, tuple):
             d['date'] = [ dt.strftime('%Y-%m-%dT%H:%M:%SZ') for dt in self.date]
         else:
             d['date'] = self.date.strftime('%Y-%m-%dT%H:%M:%SZ')
         return d
 
@@ -261,16 +270,16 @@
         x = json.loads(data)
         return cls.from_dict(x)
 
     @classmethod
     def from_dict(cls, data: dict):
         x = data
 
-        ms = list([ Metric.from_string(m) for m in x['metrics']])
-        attrs = list([ Attribute.from_string(a) for a in x['attrs']])
+        ms = list([ Metric.from_dict(m) for m in x['metrics']])
+        attrs = list([ Attribute.from_dict(a) for a in x['attrs']])
         if isinstance(x['date'], list):
             date = tuple(( datetime.strptime(d, '%Y-%m-%dT%H:%M:%SZ') for d in x['date']))
         else:
             date = datetime.strptime(x['date'], '%Y-%m-%dT%H:%M:%SZ')
         mbr = tuple(tuple(tuple(mb) for mb in m) for m in x['mbr'])
         # TODO key error if these aren't there. If we're calling from_string
         # then these keys need to exist.
@@ -336,17 +345,17 @@
         d['bounds'] = self.bounds.to_json()
         return d
 
     @classmethod
     def from_string(cls, data: str):
         x = json.loads(data)
         if 'metrics' in x:
-            ms = [ Metric.from_string(m) for m in x['metrics']]
+            ms = [ Metric.from_dict(m) for m in x['metrics']]
         if 'attrs' in x:
-            attrs = [ Attribute.from_string(a) for a in x['attrs']]
+            attrs = [ Attribute.from_dict(a) for a in x['attrs']]
         if 'bounds' in x:
             bounds = Bounds(*x['bounds'])
         if 'log' in x:
             l = x['log']
             log = Log(l['log_level'], l['logdir'], l['logtype'], l['logfilename'])
         else:
             log = Log("INFO")
```

### Comparing `silvimetric-1.1.1/src/silvimetric/resources/data.py` & `silvimetric-1.2.0/src/silvimetric/resources/data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from . import Bounds
+from .bounds import Bounds
 from .config import StorageConfig
 import numpy as np
+import copy
 
 import pdal
 
 import pathlib
 import json
 
 class Data:
@@ -13,29 +14,45 @@
 
     def __init__(self,
                  filename: str,
                  storageconfig: StorageConfig,
                  bounds: Bounds = None):
         self.filename = filename
         """Path to either PDAL pipeline or point cloud file"""
+
         self.bounds = bounds
         """Bounds of this section of data"""
 
         self.reader_thread_count = 2
         """Thread count for PDAL reader. Keep to 2 so we don't hog threads"""
 
-        self.storageconfig = storageconfig
-        """:class:`silvimetric.resources.StorageConfig`"""
         self.reader = self.get_reader()
         """PDAL reader"""
-        self.pipeline = self.get_pipeline()
-        """PDAL pipeline"""
+
         if self.bounds is None:
             self.bounds = Data.get_bounds(self.reader)
 
+        # adjust bounds if necessary
+        self.bounds.adjust_to_cell_lines(storageconfig.resolution)
+        self.bounds = Bounds.shared_bounds(self.bounds, storageconfig.root)
+
+        self.storageconfig = storageconfig
+        """:class:`silvimetric.resources.StorageConfig`"""
+        self.pipeline = self.get_pipeline()
+        """PDAL pipeline"""
+
+        self.log = storageconfig.log
+
+    def to_json(self):
+        j = dict(filename=self.filename, bounds=self.bounds.get(),
+                pipeline=json.loads(self.pipeline.pipeline), is_pipeline=self.is_pipeline())
+        return j
+
+    def __repr__(self):
+        return json.dumps(self.to_json(), indent=2)
 
     def is_pipeline(self) -> bool:
         """Does this instance represent a pdal.Pipeline or a simple filename
 
         :return: Return true if input is a pipeline
         """
 
@@ -54,22 +71,17 @@
         reader = pdal.Reader(self.filename, tag='reader')
         reader._options['threads'] = self.reader_thread_count
         if self.bounds:
             reader._options['bounds'] = str(self.bounds)
         class_zero = pdal.Filter.assign(value="Classification = 0")
         rn = pdal.Filter.assign(value="ReturnNumber = 1 WHERE ReturnNumber < 1")
         nor = pdal.Filter.assign(value="NumberOfReturns = 1 WHERE NumberOfReturns < 1")
-        ferry = pdal.Filter.ferry(dimensions="X=>xi, Y=>yi")
-
-        # assign_x = pdal.Filter.assign(
-        #     value=f"xi = (X - {self.root.minx}) / {resolution}")
-        # assign_y = pdal.Filter.assign(
-        #     value=f"yi = ({self.root.maxy} - Y) / {resolution}")
+        # ferry = pdal.Filter.ferry(dimensions="X=>xi, Y=>yi")
 
-        return reader | class_zero | rn | nor #| ferry | assign_x | assign_y #| smrf | hag
+        return reader | class_zero | rn | nor
 
     def get_pipeline(self) -> pdal.Pipeline:
         """Fetch the pipeline for the instance
 
         :raises Exception: File type isn't COPC or EPT
         :raises Exception: More than one reader detected
         :return: Return PDAL pipline
@@ -99,15 +111,23 @@
                 if not stage_kind in allowed_readers:
                     raise Exception(f"Readers for SilviMetric must be of type 'copc' or 'ept', not '{stage_kind}'")
                 readers.append(stage)
 
             # we only answer to copc or ept readers
             if stage_kind in allowed_readers:
                 if self.bounds:
-                    stage._options['bounds'] = str(self.bounds)
+                    res = self.storageconfig.resolution
+                    collar = Bounds(
+                        self.bounds.minx - res,
+                        self.bounds.miny - res,
+                        self.bounds.maxx + res,
+                        self.bounds.maxy + res
+                    )
+                    stage._options['bounds'] = str(collar)
+                    # stage._options['bounds'] = str(self.bounds)
 
             # We strip off any writers from the pipeline that were
             # given to us and drop them  on the floor
             if stage_type != 'writers':
                 stages.append(stage)
 
         # we don't support weird pipelines of shapes
@@ -115,31 +135,37 @@
         if len(readers) != 1:
             raise Exception(f"Pipelines can only have one reader of type {allowed_readers}")
 
         resolution = self.storageconfig.resolution
         # Add xi and yi – only need this for PDAL < 2.6
         ferry = pdal.Filter.ferry(dimensions="X=>xi, Y=>yi")
         assign_x = pdal.Filter.assign(value=f"xi = (X - {self.storageconfig.root.minx}) / {resolution}")
-        assign_y = pdal.Filter.assign(value=f"yi = ({self.storageconfig.root.maxy} - Y) / {resolution}")
+        assign_y = pdal.Filter.assign(value=f"yi = (({self.storageconfig.root.maxy} - Y) / {resolution}) - 1")
+        # hag = pdal.Filter.hag_nn()
+
         stages.append(ferry)
         stages.append(assign_x)
         stages.append(assign_y)
+        # stages.append(hag)
 
         # return our pipeline
         return pdal.Pipeline(stages)
 
     def execute(self):
         """Execute PDAL pipeline
 
         :raises Exception: PDAL error message passed from execution
         """
         try:
             self.pipeline.execute()
-            # self.storageconfig.log.debug(f"PDAL log: {self.pipeline.log}")
+            if self.pipeline.log and self.pipeline.log is not None:
+                self.log.debug(f"PDAL log: {self.pipeline.log}")
         except Exception as e:
+            if self.pipeline.log and self.pipeline.log is not None:
+                self.log.debug(f"PDAL log: {self.pipeline.log}")
             print(self.pipeline.pipeline, e)
             raise e
 
     def get_array(self) -> np.ndarray:
         """Fetch the array from the execute()'d pipeline
 
         :return: get data as a numpy ndarray
@@ -199,13 +225,13 @@
         """For the provided bounds, read and count the number of points that are
         inside them for this instance.
 
         :param bounds: query bounding box
         :return: point count
         """
 
-        reader = self.get_reader()
+        reader = copy.deepcopy(self.get_reader())
         if bounds:
             reader._options['bounds'] = str(bounds)
         pipeline = reader.pipeline()
         pipeline.execute()
         return len(pipeline.arrays[0])
```

### Comparing `silvimetric-1.1.1/src/silvimetric/resources/entry.py` & `silvimetric-1.2.0/src/silvimetric/resources/entry.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import json
 import numpy as np
 import pdal
-from typing import Self, Union
 from abc import ABC, abstractmethod
 from tiledb import Attr
 
 class Entry(ABC):
     """Base class for Attribute and Metric. These represent entries into the
     database."""
 
-    def __eq__(self, other: Self):
+    def __eq__(self, other):
         return self.name == other.name and \
-            self.dtype == other.dtype and \
-            self.dependencies == other.dependencies
+            self.dtype == other.dtype
 
     @abstractmethod
     def entry_name(self) -> str:
         raise NotImplementedError
 
     @abstractmethod
     def schema(self) -> Attr:
@@ -24,34 +22,37 @@
 
     @abstractmethod
     def to_json(self) -> object:
         raise NotImplementedError
 
     @staticmethod
     @abstractmethod
-    def from_string(data: str) -> Self:
+    def from_dict(data: dict):
+        raise NotImplementedError
+
+    @staticmethod
+    @abstractmethod
+    def from_string(data: str):
         raise NotImplementedError
 
     @abstractmethod
     def __repr__(self):
         raise NotImplementedError
 
 
 class Attribute(Entry):
     """Represents point data from a PDAL execution that has been binned, and
     provides the information necessary to transfer that data to the database."""
 
-    def __init__(self, name: str, dtype: np.dtype, deps: list[Self]=None):
+    def __init__(self, name: str, dtype: np.dtype):
         super().__init__()
         self.name = name
         """Name of the attribute, eg. Intensity."""
         self.dtype = dtype
         """Numpy data type."""
-        self.dependencies = deps
-        """Attributes/Metrics this is dependent on."""
 
     def entry_name(self) -> str:
         """Return TileDB attribute name."""
         return self.name
 
     def schema(self) -> Attr:
         """
@@ -59,37 +60,38 @@
         :return: TileDB attribute schema
         """
         return Attr(name=self.name, dtype=self.dtype, var=True)
 
     def to_json(self) -> object:
         return {
             'name': self.name,
-            'dtype': np.dtype(self.dtype).str,
-            'dependencies': self.dependencies,
+            'dtype': np.dtype(self.dtype).str
         }
 
     @staticmethod
-    def from_string(data: Union[str, dict]) -> Self:
+    def from_dict(data: dict):
+        """
+        Make an Attribute from a JSON like object
+        """
+        name = data['name']
+        dtype = data['dtype']
+        return Attribute(name, dtype)
+
+    @staticmethod
+    def from_string(data: str):
         """
         Create Attribute from string or dict version of it.
 
         :param data: Stringified or json object of attribute
         :raises TypeError: Incorrect type of incoming data, must be string or dict
         :return: Return derived Attribute
         """
-        if isinstance(data, str):
-            j = json.loads(data)
-        elif isinstance(data, dict):
-            j = data
-        else:
-            raise TypeError(f'Type of data, {data} is not str or dict')
-        name = j['name']
-        dtype = j['dtype']
-        deps = j['dependencies']
-        return Attribute(name, dtype, deps)
+        j = json.loads(data)
+        return Attribute.from_dict(j)
+
 
     def __repr__(self):
         return json.dumps(self.to_json())
 
 # A list of pdal dimensions can be found here https://pdal.io/en/2.6.0/dimensions.html
 Pdal_Attributes = { d['name']: Attribute(d['name'], d['dtype']) for d in pdal.dimensions }
 Attributes = Pdal_Attributes
```

### Comparing `silvimetric-1.1.1/src/silvimetric/resources/extents.py` & `silvimetric-1.2.0/src/silvimetric/resources/extents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import math
 import numpy as np
 
 import logging
 import dask
 import dask.bag as db
 
-from typing import Self
 from math import ceil
 
 from .log import Log
 from .bounds import Bounds
 from .storage import Storage
 from .data import Data
 
@@ -25,33 +24,37 @@
                  root: Bounds):
 
         self.bounds = bounds
         """Bounding box of this section of data."""
         self.root = root
         """Root bounding box of the database."""
 
+        # adjust bounds so they're matching up with cell lines
+        self.bounds.adjust_to_cell_lines(resolution)
         minx, miny, maxx, maxy = self.bounds.get()
 
+
         self.rangex = maxx - minx
         """Range of X Indices"""
         self.rangey = maxy - miny
         """Range of Y indices"""
         self.resolution = resolution
         """Resolution of database."""
         self.cell_count = int((self.rangex * self.rangey) / self.resolution ** 2)
         """Number of cells in this Extents"""
 
         self.x1 = math.floor((minx - self.root.minx) / resolution)
         """Minimum X index"""
-        self.y1 = math.floor((self.root.maxy - maxy) / resolution)
-        """Minimum Y index"""
         self.x2 = math.ceil((maxx - self.root.minx) / resolution)
         """Maximum X index"""
+
+        self.y1 = math.ceil((self.root.maxy - maxy) / resolution)
+        """Minimum Y index, or maximum Y value in point cloud"""
         self.y2 = math.ceil((self.root.maxy - miny) / resolution)
-        """Maximum Y index"""
+        """Maximum Y index, or minimum Y value in point cloud"""
         self.domain: IndexDomainList = ((self.x1, self.x2), (self.y1, self.y2))
         """Minimum bounding rectangle of this Extents"""
 
     def get_indices(self):
         """
         Create indices for this section of the database relative to the root
         bounds.
@@ -77,15 +80,15 @@
         y1, y2 = ys
         if x1 > self.x2 or x2 < self.x1:
             return True
         if y1 > self.y2 or y2 < self.y1:
             return True
         return False
 
-    def disjoint(self, other: Self):
+    def disjoint(self, other):
         """
         Determined if this Extents shares any points with another Extents object.
 
         :param other: Extents object to compare against.
         :return: True if no shared points, false otherwise.
         """
         return self.bounds.disjoint(other.bounds)
@@ -108,29 +111,29 @@
         else:
             bminx, bminy, bmaxx, bmaxy = self.bounds.get()
             r = self.bounds
 
         # make bounds in scale with the desired resolution
         minx = bminx + (self.x1 * self.resolution)
         maxx = bminx + (self.x2 * self.resolution)
+
         miny = bmaxy - (self.y2 * self.resolution)
         maxy = bmaxy - (self.y1 * self.resolution)
 
         chunk = Extents(Bounds(minx, miny, maxx, maxy), self.resolution, r)
 
         if self.bounds == self.root:
             self.root = chunk.bounds
 
         filtered = []
-        curr = db.from_delayed(chunk.filter(data, res_threshold, pc_threshold, depth_threshold))
-        curr_depth = 0
+        curr = db.from_delayed([ch.filter(data, res_threshold, pc_threshold,
+            depth_threshold, 1) for ch in chunk.split()])
+        curr_depth = 1
 
-        logger = logging.getLogger('silvimetric')
-        if not logger.handlers:
-            logger = Log('INFO')
+        logger = data.storageconfig.log
         while curr.npartitions > 0:
 
             logger.debug(f'Filtering {curr.npartitions} tiles at depth {curr_depth}')
             n = curr.compute()
             to_add = [ne for ne in n if isinstance(ne, Extents)]
             if to_add:
                 filtered = filtered + to_add
@@ -146,28 +149,29 @@
         Split this extent into 4 children along the cell lines
 
         :return: Returns 4 child extents
         """
         minx, miny, maxx, maxy = self.bounds.get()
 
         x_adjusted = math.floor((maxx - minx) / 2 / self.resolution)
-        y_adjusted = math.floor((maxy - miny) / 2 / self.resolution)
+        y_adjusted = math.ceil((maxy - miny) / 2 / self.resolution)
 
         midx = minx + (x_adjusted * self.resolution)
         midy = maxy - (y_adjusted * self.resolution)
 
-        return [
+        exts =  [
             Extents(Bounds(minx, miny, midx, midy), self.resolution, self.root), #lower left
             Extents(Bounds(midx, miny, maxx, midy), self.resolution, self.root), #lower right
             Extents(Bounds(minx, midy, midx, maxy), self.resolution, self.root), #top left
             Extents(Bounds(midx, midy, maxx, maxy), self.resolution, self.root)  #top right
         ]
+        return exts
 
     @dask.delayed
-    def filter(self, data: Data, res_threshold=100, pc_threshold=600000, depth_threshold=6, depth=0) -> Self:
+    def filter(self, data: Data, res_threshold=100, pc_threshold=600000, depth_threshold=6, depth=0):
         """
         Creates quad tree of chunks for this bounds, runs pdal quickinfo over
         this to determine if there are any points available. Uses a bottom resolution
         of 1km.
 
         :param data: Data object containing point cloud details.
         :param res_threshold: Resolution threshold., defaults to 100
```

### Comparing `silvimetric-1.1.1/src/silvimetric/resources/log.py` & `silvimetric-1.2.0/src/silvimetric/resources/log.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.1.1/src/silvimetric/resources/names.py` & `silvimetric-1.2.0/src/silvimetric/resources/names.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.1.1/src/silvimetric/resources/storage.py` & `silvimetric-1.2.0/src/silvimetric/resources/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import tiledb
 import numpy as np
 from datetime import datetime
 import pathlib
 import contextlib
 import json
 import urllib
-from typing import Any
+from typing import Generator
 
 from math import floor
 
 from .config import StorageConfig, ShatterConfig
 from .metric import Metric, Attribute
-from ..resources import Bounds
+from .bounds import Bounds
 
 class Storage:
     """ Handles storage of shattered data in a TileDB Database. """
 
     def __init__(self, config: StorageConfig, ctx:tiledb.Ctx=None):
 
         if not tiledb.object_type(config.tdb_dir) == "array":
@@ -55,32 +55,44 @@
         """
 
         # TODO make any changes to tiledb setup here.
 
         if not ctx:
             ctx = tiledb.default_ctx()
 
+        # adjust cell bounds if necessary
+        config.root.adjust_to_cell_lines(config.resolution)
+
         # dims = { d['name']: d['dtype'] for d in pdal.dimensions if d['name'] in config.attrs }
         xi = floor((config.root.maxx - config.root.minx) / float(config.resolution))
         yi = floor((config.root.maxy - config.root.miny) / float(config.resolution))
 
         dim_row = tiledb.Dim(name="X", domain=(0,xi), dtype=np.int32)
         dim_col = tiledb.Dim(name="Y", domain=(0,yi), dtype=np.int32)
         domain = tiledb.Domain(dim_row, dim_col)
 
         count_att = tiledb.Attr(name="count", dtype=np.int32)
         dim_atts = [attr.schema() for attr in config.attrs]
 
-        metric_atts = [m.schema(a) for m in config.metrics for a in config.attrs]
+        metric_atts = [m.schema(a) for m in config.metrics for a in config.attrs if a in m.attributes or not m.attributes]
+
+        # Check that all attributes required for metric usage are available
+        att_list = [a.name for a in config.attrs]
+        required_atts = [d.name for m in config.metrics for d in m.dependencies
+                if isinstance(d, Attribute)]
+        for ra in required_atts:
+            if ra not in att_list:
+                raise ValueError(f'Missing required dependency, {ra}.')
 
         # allows_duplicates lets us insert multiple values into each cell,
         # with each value representing a set of values from a shatter process
         # https://docs.tiledb.com/main/how-to/performance/performance-tips/summary-of-factors#allows-duplicates
         schema = tiledb.ArraySchema(domain=domain, sparse=True,
-            attrs=[count_att, *dim_atts, *metric_atts], allows_duplicates=True)
+            attrs=[count_att, *dim_atts, *metric_atts], allows_duplicates=True,
+            capacity=1000)
         schema.check()
 
         tiledb.SparseArray.create(config.tdb_dir, schema)
         with tiledb.SparseArray(config.tdb_dir, "w") as a:
             meta = str(config)
             a.meta['config'] = meta
 
@@ -160,16 +172,20 @@
         """
         Find List of metric names from storage config
 
         :return: List of metric names.
         """
         return self.getConfig().metrics
 
+    def getDerivedNames(self) -> list[str]:
+        # if no attributes are set in the metric, use all
+        return [m.entry_name(a.name) for m in self.config.metrics
+                for a in self.config.attrs if not m.attributes or a in m.attributes]
     @contextlib.contextmanager
-    def open(self, mode:str='r', timestamp=None) -> tiledb.SparseArray:
+    def open(self, mode:str='r', timestamp=None) -> Generator[tiledb.SparseArray, None, None]:
         """
         Open stream for TileDB database in given mode and at given timestamp.
 
         :param mode: Mode to open TileDB stream in. Valid options are
             'w', 'r', 'm', 'd'., defaults to 'r'.
         :param timestamp: Timestamp to open database at., defaults to None.
         :raises Exception: Incorrect Mode was given, only valid modes are 'w' and 'r'.
@@ -290,30 +306,46 @@
     def delete(self, proc_num: int) -> ShatterConfig:
         """
         Delete Shatter process and all associated data from database.
 
         :param proc_num: Shatter process time slot
         :return: Config of deleted Shatter process
         """
+
+        self.config.log.debug(f'Deleting time slot {proc_num}...')
         with self.open('r', (proc_num, proc_num)) as r:
             sh_cfg: ShatterConfig = ShatterConfig.from_string(r.meta['shatter'])
             sh_cfg.mbr = ()
             sh_cfg.finished = False
+
+        self.config.log.debug('Deleting fragments...')
         with self.open('m', (proc_num, proc_num)) as m:
             m.delete_fragments(proc_num, proc_num)
+        self.config.log.debug('Rewriting config.')
         with self.open('w', (proc_num, proc_num)) as w:
             w.meta['shatter'] = json.dumps(sh_cfg.to_json())
         return sh_cfg
 
-    def consolidate_shatter(self, proc_num: int) -> None:
+    def consolidate_shatter(self, proc_num: int, retries=0) -> None:
         """
         Consolidate the fragments from a shatter process into one fragment.
         This makes the database perform better, but reduces the granularity of
         time traveling.
 
         :param proc_num: Time slot associated with shatter process.
         """
-        # TODO move from timestamp to fragment_uris, timestamp is deprecated
-        # this is currently failing, I believe from a bug in tiledb
-        afs = self.get_fragments_by_time(proc_num)
-        uris = [ os.path.split(urllib.parse.urlparse(f.uri).path)[-1] for f in afs ]
-        tiledb.consolidate(self.config.tdb_dir, fragment_uris=uris)
+        try:
+            afs = self.get_fragments_by_time(proc_num)
+            uris = [ os.path.split(urllib.parse.urlparse(f.uri).path)[-1] for f in afs ]
+            tiledb.consolidate(self.config.tdb_dir, fragment_uris=uris)
+            c = tiledb.Config({"sm.vacuum.mode": "fragments"})
+            tiledb.vacuum(self.config.tdb_dir, c)
+            self.config.log.info(f"Consolidated time slot {proc_num}.")
+        except Exception as e:
+            if retries >= 3:
+                self.config.log.warning("Failed to consolidate time slot "
+                        f"{proc_num} {retries} time(s). Stopping.")
+                raise e
+            self.config.log.warning("Failed to consolidate time slot "
+                    f"{proc_num} {retries+1} time. Retrying...")
+            self.consolidate_shatter(proc_num, retries+1)
+
```

### Comparing `silvimetric-1.1.1/src/silvimetric.egg-info/SOURCES.txt` & `silvimetric-1.2.0/src/silvimetric.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -23,16 +23,18 @@
 src/silvimetric/resources/data.py
 src/silvimetric/resources/entry.py
 src/silvimetric/resources/extents.py
 src/silvimetric/resources/log.py
 src/silvimetric/resources/metric.py
 src/silvimetric/resources/names.py
 src/silvimetric/resources/storage.py
-tests/test_chunk.py
 tests/test_cli.py
 tests/test_commands.py
 tests/test_configuration.py
 tests/test_data.py
+tests/test_extents.py
 tests/test_extract.py
+tests/test_fusion.py
+tests/test_metrics.py
 tests/test_shatter.py
 tests/test_storage.py
 tests/test_western.py
```

### Comparing `silvimetric-1.1.1/tests/test_chunk.py` & `silvimetric-1.2.0/tests/test_extents.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import numpy as np
 import datetime
 
-from silvimetric.resources import Extents
+from silvimetric import Extents
 from silvimetric.commands.shatter import run
 
+def check_for_overlap(leaves: list[Extents], chunk: Extents):
+    idx = [i for l in leaves for i in l.get_indices() ]
+    u, c = np.unique(idx, return_counts=True)
+    assert not np.any(np.where(c > 1))
+
 def check_for_holes(leaves: list[Extents], chunk: Extents):
     ind = np.array([], dtype=chunk.get_indices().dtype)
     for leaf in leaves:
         a = leaf.get_indices()
         if ind.size == 0:
             ind = a
         else:
@@ -79,16 +84,18 @@
     assert b == False, f"Indices duplicated: {dup}"
 
 
 class TestExtents(object):
     def test_indexing(self, extents, filtered, unfiltered):
         check_indexing(extents, filtered)
         check_for_holes(filtered, extents)
+        check_for_overlap(filtered, extents)
         check_indexing(extents, unfiltered)
         check_for_holes(unfiltered, extents)
+        check_for_overlap(unfiltered, extents)
 
     # def test_cells(self, copc_filepath, unfiltered, resolution):
     #     flag = False
     #     bad_chunks = []
     #     for leaf in unfiltered:
     #         reader = pdal.Reader(copc_filepath)
     #         crop = pdal.Filter.crop(bounds=str(leaf))
```

### Comparing `silvimetric-1.1.1/tests/test_cli.py` & `silvimetric-1.2.0/tests/test_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,74 @@
 import numpy as np
-import pytest
+import os
 
 from silvimetric.cli import cli
 from silvimetric.commands import shatter, info
-from silvimetric.resources import ShatterConfig
+from silvimetric import ShatterConfig
 
 class TestCli(object):
-    def test_cli_init(self, tdb_filepath, runner, bounds):
-        res = runner.invoke(cli.cli, args=["-d", tdb_filepath, "--debug",
+    def test_cli_init(self, tmp_path_factory, runner, bounds):
+        path = tmp_path_factory.mktemp("test_tdb")
+        p = os.path.abspath(path)
+        res = runner.invoke(cli.cli, args=["-d", p, "--debug",
                 "--scheduler", "single-threaded", "initialize", "--resolution",
                 '10', '--crs', 'EPSG:3857', '--bounds', str(bounds)],
                 catch_exceptions=False)
         assert res.exit_code == 0
 
-    def test_cli_shatter(self, runner, storage, maxy, date, tdb_filepath,
-            copc_filepath):
+    def test_cli_shatter(self, runner, maxy, date, tdb_filepath,
+            copc_filepath, storage):
 
         res = runner.invoke(cli.cli, args=["-d", tdb_filepath,
                 "--scheduler", "single-threaded",
                 "shatter", copc_filepath,
                 "--date", date.isoformat()+'Z',
                 "--tilesize", '10'], catch_exceptions=False)
         assert res.exit_code == 0
 
         with storage.open('r') as a:
-            y = a[:,0]['Z'].shape[0]
-            x = a[0,:]['Z'].shape[0]
-            assert y == 10
-            assert x == 10
-            for xi in range(x):
-                for yi in range(y):
-                    a[xi, yi]['Z'].size == 1
-                    assert bool(np.all(a[xi, yi]['Z'][0] == ((maxy/storage.config.resolution)-yi)))
+            assert a[:,:]['Z'].shape[0] == 100
+            xdom = a.schema.domain.dim('X').domain[1]
+            ydom = a.schema.domain.dim('Y').domain[1]
+            assert xdom == 10
+            assert ydom == 10
 
-    def test_cli_scan(self, tdb_filepath, runner, copc_filepath, storage):
-        res = runner.invoke(cli.cli, args=['-d', tdb_filepath, '--scheduler', 'single-threaded', 'scan', copc_filepath])
+            for xi in range(xdom):
+                for yi in range(ydom):
+                    a[xi, yi]['Z'].size == 1
+                    a[xi, yi]['Z'][0].size == 900
+                    # this should have all indices from 0 to 9 filled.
+                    # if oob error, it's not this test's fault
+                    assert bool(np.all( a[xi, yi]['Z'][0] == ((maxy/storage.config.resolution) - (yi + 1)) ))
+
+    def test_cli_scan(self, runner, copc_filepath, storage_config):
+        tdb_dir = storage_config.tdb_dir
+        res = runner.invoke(cli.cli, args=['-d', tdb_dir, '--scheduler', 'single-threaded', 'scan', copc_filepath])
+        print(res.output)
         assert res.exit_code == 0
 
     def test_cli_info(self, tdb_filepath, runner, shatter_config):
         shatter.shatter(shatter_config)
         res = runner.invoke(cli.cli, args=['-d', tdb_filepath, '--scheduler', 'single-threaded', 'info'])
         assert res.exit_code == 0
 
-    def test_cli_extract(self, runner, extract_config):
-        atts = ' '.join([f'-a {a.name}' for a in extract_config.attrs])
-        ms = ' '.join([f'-m {m.name}' for m in extract_config.metrics])
+    def test_cli_extract(self, runner, extract_config, storage):
+        atts = []
+        for a in extract_config.attrs:
+            atts.append('-a')
+            atts.append(a.name)
+        ms = []
+        for m in extract_config.metrics:
+            ms.append('-m')
+            ms.append(m.name)
         out_dir = extract_config.out_dir
         tdb_dir = extract_config.tdb_dir
 
-        res = runner.invoke(cli.cli, args=(f'-d {tdb_dir} --scheduler '+
-            f'single-threaded extract {atts} {ms} --outdir {out_dir}'))
+        res = runner.invoke(cli.cli, args=['-d', tdb_dir, '--scheduler',
+            'single-threaded', 'extract', *atts, *ms, '--outdir' ,out_dir])
 
         assert res.exit_code == 0
 
     def test_cli_delete(self, runner, shatter_config, pre_shatter):
         i = shatter_config.name
         res = runner.invoke(cli.cli, ['-d', shatter_config.tdb_dir,
                 '--scheduler', 'single-threaded', 'delete', '--id', i])
```

### Comparing `silvimetric-1.1.1/tests/test_commands.py` & `silvimetric-1.2.0/tests/test_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import json
 
 from silvimetric.commands import scan, info, shatter, manage
-from silvimetric.resources import ShatterConfig, Storage
+from silvimetric import ShatterConfig, Storage
 
 class TestCommands(object):
 
     def test_scan(self, shatter_config):
         s = shatter_config
         res = scan.scan(s.tdb_dir, s.filename, s.bounds, 10, 10, 5)
-        assert res == 1
+        assert res['tile_info']['recommended'] == 1
+
         res = scan.scan(s.tdb_dir, s.filename, s.bounds, depth=5)
-        assert res == 100
+        assert res['tile_info']['recommended'] == 100
 
     def test_info(self, tdb_filepath, config_split):
         i = info.info(tdb_filepath)
         assert bool(i['history'])
         assert len(i['history']) == 4
 
         for idx, c in enumerate(i['history']):
```

### Comparing `silvimetric-1.1.1/tests/test_configuration.py` & `silvimetric-1.2.0/tests/test_configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from silvimetric.resources import StorageConfig, ShatterConfig, ExtractConfig
+from silvimetric import StorageConfig, ShatterConfig, ExtractConfig
 
 class Test_Configuration(object):
 
     def test_serialization(self, storage_config, shatter_config, extract_config):
 
         # storage
         j = str(storage_config)
         c = StorageConfig.from_string(j)
         mean = [ m for m in c.metrics if m.name == 'mean']
         assert len(mean) == 1
 
-        assert int(mean[0]([2,2,2,2])) == 2
+        assert int(mean[0]._method([2,2,2,2])) == 2
         assert storage_config == c
 
         # shatter
         sh_str = str(shatter_config)
         sh_cfg = ShatterConfig.from_string(sh_str)
         assert shatter_config == sh_cfg
 
         # extract
         ex_str = str(extract_config)
         ex_cfg = ExtractConfig.from_string(ex_str)
-        assert extract_config == ex_cfg
+        assert extract_config == ex_cfg
```

### Comparing `silvimetric-1.1.1/tests/test_extract.py` & `silvimetric-1.2.0/tests/test_extract.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 from pathlib import Path
 from osgeo import gdal
 from pyproj import CRS
 
-from silvimetric.commands.extract import extract
-from silvimetric.resources import Metrics, ExtractConfig, Extents, Log
+from silvimetric import Metrics, ExtractConfig, Extents, Log, extract, Storage
 
 def tif_test(extract_config):
     minx, miny, maxx, maxy = extract_config.bounds.get()
     resolution = extract_config.resolution
     filenames = [Metrics[m.name].entry_name(a.name)
                     for m in extract_config.metrics
                     for a in extract_config.attrs]
-    e = Extents.from_storage(extract_config.tdb_dir)
-    yimin = e.get_indices()['y'].min()
+    storage = Storage.from_db(extract_config.tdb_dir)
+    e = Extents(extract_config.bounds, extract_config.resolution, storage.config.root)
+    root_maxy = storage.config.root.maxy
 
     for f in filenames:
+        if 'Return' in f:
+            continue
         path = Path(extract_config.out_dir) / f'{f}.tif'
         assert path.exists()
 
         raster: gdal.Dataset = gdal.Open(str(path))
         derived = CRS.from_user_input(raster.GetProjection())
+        rminx, xres, xskew, rmaxy, yskew, yres  = raster.GetGeoTransform()
+        assert rminx == minx
+        assert rmaxy == maxy
+        assert xres == resolution
+        assert -yres == resolution
+
+
         assert derived == extract_config.crs
 
-        xsize = int((maxx - minx) / resolution)
-        ysize = int((maxy - miny) / resolution)
+        xsize = e.x2
+        ysize = e.y2
         assert raster.RasterXSize == xsize
         assert raster.RasterYSize == ysize
 
         r = raster.ReadAsArray()
-        assert all([ r[y,x] == ((maxy/resolution)-(y+yimin))  for y in range(ysize) for x in range(xsize)])
+        assert all([ r[y,x] == ((root_maxy/resolution)-y-1)  for y in range(e.y1, e.y2) for x in range(e.x1, e.x2)])
 
 class Test_Extract(object):
 
     def test_config(self, extract_config, tdb_filepath, tif_filepath, extract_attrs):
         assert all([a in [*extract_attrs, 'count'] for a in extract_config.attrs])
         assert all([a in extract_config.attrs for a in extract_attrs])
         assert extract_config.tdb_dir == tdb_filepath
```

### Comparing `silvimetric-1.1.1/tests/test_shatter.py` & `silvimetric-1.2.0/tests/test_shatter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import os
 import pytest
 import numpy as np
 import dask
 import json
 import uuid
 
-from silvimetric.commands.shatter import shatter
-from silvimetric.commands.info import info
-from silvimetric.resources import Storage, Extents, ShatterConfig, Log
+from silvimetric import Extents, Log, info, shatter, Bounds, Storage
+from silvimetric import StorageConfig, ShatterConfig
 
 
 @dask.delayed
-def write(x,y,val, s:Storage, attrs, dims, metrics):
+def write(x, y, val, s:Storage, attrs, dims, metrics):
     m_list = [m.entry_name(a.name) for m in metrics for a in attrs]
     data = { a.name: np.array([np.array([val], dims[a.name]), None], object)[:-1]
                 for a in attrs }
 
     for m in m_list:
         data[m] = [val]
 
@@ -24,41 +23,49 @@
         w[x,y] = data
 
 class Test_Shatter(object):
 
     def test_shatter(self, shatter_config, storage: Storage, maxy):
         shatter(shatter_config)
         with storage.open('r') as a:
-            y = a[:,0]['Z'].shape[0]
-            x = a[0,:]['Z'].shape[0]
-            assert y == 10
-            assert x == 10
-            for xi in range(x):
-                for yi in range(y):
+            assert a[:,:]['Z'].shape[0] == 100
+            xdom = a.schema.domain.dim('X').domain[1]
+            ydom = a.schema.domain.dim('Y').domain[1]
+            assert xdom == 10
+            assert ydom == 10
+
+            for xi in range(xdom):
+                for yi in range(ydom):
                     a[xi, yi]['Z'].size == 1
-                    assert bool(np.all(a[xi, yi]['Z'][0] == ((maxy/storage.config.resolution)-yi)))
+                    a[xi, yi]['Z'][0].size == 900
+                    # this should have all indices from 0 to 9 filled.
+                    # if oob error, it's not this test's fault
+                    assert bool(np.all( a[xi, yi]['Z'][0] == ((maxy/storage.config.resolution) - (yi + 1)) ))
 
         # change attributes to make it a new run
         shatter_config.name = uuid.uuid4()
         shatter_config.mbr = ()
         shatter_config.time_slot = 2
 
         shatter(shatter_config)
         with storage.open('r') as a:
             # querying flattens to 20, there will 10 pairs of values
+            assert a[:,:]['Z'].shape[0] == 200
             assert a[:,0]['Z'].shape[0] == 20
             assert a[0,:]['Z'].shape[0] == 20
             # now test that the second set is the same as the first set
             # and test that this value is still the same as the original
             # which was set at ((maxy/resolution)-yindex)
-            for xi in range(x):
-                for yi in range(y):
+            for xi in range(xdom):
+                for yi in range(ydom):
                     a[xi, yi]['Z'].size == 2
+                    a[xi, yi]['Z'][0].size == 900
+                    a[xi, yi]['Z'][1].size == 900
                     assert bool(np.all(a[xi, yi]['Z'][1] == a[xi,yi]['Z'][0]))
-                    assert bool(np.all(a[xi, yi]['Z'][1] == ((maxy/storage.config.resolution)-yi)))
+                    assert bool(np.all(a[xi, yi]['Z'][1] == ((maxy/storage.config.resolution) - (yi + 1))))
 
         m = info(storage.config.tdb_dir)
         assert len(m['history']) == 2
 
     def test_parallel(self, storage, attrs, dims, threaded_dask, metrics):
         # test that writing in parallel doesn't affect ordering of values
         # constrained by NumberOfReturns being uint8
@@ -82,15 +89,15 @@
         except BaseException as e:
             pytest.fail("Failed to retrieve 'shatter' metadata key." + e.args)
         meta_j = json.loads(meta)
         pc = meta_j['point_count']
         assert pc == test_point_count
 
     @pytest.mark.parametrize('sh_cfg', ['shatter_config', 'uneven_shatter_config'])
-    def test_sub_bounds(self, sh_cfg, test_point_count, request):
+    def test_sub_bounds(self, sh_cfg, test_point_count, request, maxy, resolution):
         s = request.getfixturevalue(sh_cfg)
         storage = Storage.from_db(s.tdb_dir)
         e = Extents.from_storage(s.tdb_dir)
 
         pc = 0
         for b in e.split():
             log = Log(20)
@@ -109,27 +116,53 @@
         history = info(s.tdb_dir)['history']
         assert len(history) == 4
         assert isinstance(history, list)
         pcs = [ h['point_count'] for h in history ]
         assert sum(pcs) == test_point_count
         assert pc == test_point_count
 
+        with storage.open('r') as a:
+            xdom = a.schema.domain.dim('X').domain[1]
+            ydom = a.schema.domain.dim('Y').domain[1]
+
+            data = a.query(attrs=['Z'], coords=True, use_arrow=False).df[:]
+            data = data.set_index(['X','Y'])
+
+            for xi in range(xdom):
+                for yi in range(ydom):
+                    curr = data.loc[xi,yi]
+                    # check that each cell only has one allocation
+                    curr.size == 1
+
+    def test_partial_overlap(self, partial_shatter_config, test_point_count):
+        pc = shatter(partial_shatter_config)
+        assert pc == test_point_count / 4
+
     @pytest.mark.skipif(
         os.environ.get('AWS_SECRET_ACCESS_KEY') is None or
         os.environ.get('AWS_ACCESS_KEY_ID') is None,
         reason='Missing necessary AWS environment variables'
     )
     def test_remote_creation(self, s3_shatter_config, s3_storage):
         # need processes scheduler to accurately test bug fix
         dask.config.set(scheduler="processes")
         resolution = s3_storage.config.resolution
         maxy = s3_storage.config.root.maxy
         shatter(s3_shatter_config)
         with s3_storage.open('r') as a:
-            y = a[:,0]['Z'].shape[0]
-            x = a[0,:]['Z'].shape[0]
-            assert y == 10
-            assert x == 10
-            for xi in range(x):
-                for yi in range(y):
-                    a[xi, yi]['Z'].size == 1
-                    assert bool(np.all(a[xi, yi]['Z'][0] == ((maxy/resolution)-yi)))
+            assert a[:,:]['Z'].shape[0] == 100
+            xdom = a.schema.domain.dim('X').domain[1]
+            ydom = a.schema.domain.dim('Y').domain[1]
+            assert xdom == 10
+            assert ydom == 10
+            # get all data local so we're not hittin s3 all the time
+            data = a.query(attrs=['Z'], coords=True, use_arrow=False).df[:]
+            data = data.set_index(['X','Y'])
+
+            for xi in range(xdom):
+                for yi in range(ydom):
+                    curr = data.loc[xi,yi]
+                    curr.size == 1
+                    curr.iloc[0].size == 900
+                    # this should have all indices from 0 to 9 filled.
+                    # if oob error, it's not this test's fault
+                    assert bool(np.all( curr.iloc[0] == ((maxy/resolution) - (yi + 1)) ))
```

